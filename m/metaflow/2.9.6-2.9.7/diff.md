# Comparing `tmp/metaflow-2.9.6.tar.gz` & `tmp/metaflow-2.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-2.9.6.tar", last modified: Wed Jun 21 17:02:03 2023, max compression
+gzip compressed data, was "metaflow-2.9.7.tar", last modified: Tue Jun 27 10:22:04 2023, max compression
```

## Comparing `metaflow-2.9.6.tar` & `metaflow-2.9.7.tar`

### file list

```diff
@@ -1,334 +1,334 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.656867 metaflow-2.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-21 17:01:53.000000 metaflow-2.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-21 17:01:53.000000 metaflow-2.9.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-21 17:02:03.656867 metaflow-2.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-06-21 17:01:53.000000 metaflow-2.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.628867 metaflow-2.9.6/metaflow/
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/R.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.628867 metaflow-2.9.6/metaflow/_vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.632867 metaflow-2.9.6/metaflow/_vendor/click/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/click/_bashcomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/click/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/click/_termui_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/click/_textwrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/click/_unicodefun.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/click/_winconsole.py
--rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/click/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/click/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/click/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/click/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/click/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/click/termui.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/click/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/click/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.632867 metaflow-2.9.6/metaflow/_vendor/v3_5/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/v3_5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.632867 metaflow-2.9.6/metaflow/_vendor/v3_5/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/v3_5/zipp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.632867 metaflow-2.9.6/metaflow/_vendor/v3_6/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/v3_6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.632867 metaflow-2.9.6/metaflow/_vendor/v3_6/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/v3_6/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/v3_6/typing_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/_vendor/v3_6/zipp.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/cards.py
--rw-r--r--   0 runner    (1001) docker     (123)    35024 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/cli_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.632867 metaflow-2.9.6/metaflow/client/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69283 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/client/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/client/filecache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.632867 metaflow-2.9.6/metaflow/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33396 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/cmd/configure_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/cmd/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/cmd/tutorials_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/cmd/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/cmd_with_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/current.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.636867 metaflow-2.9.6/metaflow/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/datastore/content_addressed_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/datastore/datastore_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/datastore/datastore_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/datastore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/datastore/flow_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/datastore/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/datastore/task_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/event_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.636867 metaflow-2.9.6/metaflow/extension_support/
--rw-r--r--   0 runner    (1001) docker     (123)    49461 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/extension_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/extension_support/_empty_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/extension_support/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/extension_support/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/extension_support/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/flowspec.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19721 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/includefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.636867 metaflow-2.9.6/metaflow/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/metadata/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/metadata/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18895 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/metaflow_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/metaflow_config_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/metaflow_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/metaflow_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/metaflow_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.636867 metaflow-2.9.6/metaflow/mflog/
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/mflog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/mflog/mflog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/mflog/save_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/mflog/save_logs_periodically.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/mflog/tee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/multicore_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.636867 metaflow-2.9.6/metaflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.636867 metaflow-2.9.6/metaflow/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:53.000000 metaflow-2.9.6/metaflow/plugins/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31445 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/airflow/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/airflow/airflow_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/airflow/airflow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/airflow/airflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/airflow/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/airflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.640867 metaflow-2.9.6/metaflow/plugins/airflow/plumbing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/airflow/plumbing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/airflow/plumbing/set_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.640867 metaflow-2.9.6/metaflow/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/airflow/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/airflow/sensors/base_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/airflow/sensors/external_task_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/airflow/sensors/s3_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.640867 metaflow-2.9.6/metaflow/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/argo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/argo/argo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/argo/argo_events.py
--rw-r--r--   0 runner    (1001) docker     (123)   104799 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/argo/argo_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    20298 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/argo/argo_workflows_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/argo/argo_workflows_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/argo/process_input_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.640867 metaflow-2.9.6/metaflow/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/aws_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/aws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.640867 metaflow-2.9.6/metaflow/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16677 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/batch/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/batch/batch_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/batch/batch_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/batch/batch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.640867 metaflow-2.9.6/metaflow/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/secrets_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.640867 metaflow-2.9.6/metaflow/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/step_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/step_functions/dynamo_db_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/step_functions/event_bridge_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/step_functions/production_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/step_functions/schedule_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/step_functions/set_batch_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    42848 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/step_functions/step_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21420 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/step_functions/step_functions_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/step_functions/step_functions_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/aws/step_functions/step_functions_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.644867 metaflow-2.9.6/metaflow/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/azure/azure_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/azure/azure_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/azure/azure_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/azure/blob_service_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/azure/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.644867 metaflow-2.9.6/metaflow/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.644867 metaflow-2.9.6/metaflow/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_modules/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_modules/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_modules/bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_modules/card.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.644867 metaflow-2.9.6/metaflow/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_modules/chevron/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_modules/chevron/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_modules/chevron/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_modules/chevron/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_modules/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_modules/convert_to_native_type.py
--rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_modules/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_modules/renderer_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_modules/test_cards.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/card_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/component_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/cards/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/catch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.644867 metaflow-2.9.6/metaflow/plugins/conda/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/conda/batch_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/conda/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/conda/conda_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/conda/conda_flow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/conda/conda_step_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.648867 metaflow-2.9.6/metaflow/plugins/datastores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/datastores/azure_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/datastores/gs_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/datastores/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/datastores/s3_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.648867 metaflow-2.9.6/metaflow/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/datatools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/datatools/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.648867 metaflow-2.9.6/metaflow/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/datatools/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64840 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/datatools/s3/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    43171 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/datatools/s3/s3op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/datatools/s3/s3tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/datatools/s3/s3util.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/debug_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/debug_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.648867 metaflow-2.9.6/metaflow/plugins/env_escape/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/client_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.648867 metaflow-2.9.6/metaflow/plugins/env_escape/communication/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/communication/bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/communication/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/communication/socket_bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/communication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.648867 metaflow-2.9.6/metaflow/plugins/env_escape/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/configurations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.648867 metaflow-2.9.6/metaflow/plugins/env_escape/configurations/emulate_test_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.648867 metaflow-2.9.6/metaflow/plugins/env_escape/configurations/test_lib_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/data_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/exception_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/override_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/env_escape/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/environment_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17724 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/events_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.648867 metaflow-2.9.6/metaflow/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/frameworks/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.648867 metaflow-2.9.6/metaflow/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/gcp/gs_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/gcp/gs_storage_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/gcp/gs_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/gcp/gs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/gcp/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.652867 metaflow-2.9.6/metaflow/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16678 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/kubernetes/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/kubernetes/kubernetes_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/kubernetes/kubernetes_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19933 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/kubernetes/kubernetes_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/kubernetes/kubernetes_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.652867 metaflow-2.9.6/metaflow/plugins/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/metadata/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/metadata/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/package_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/parallel_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/project_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/resources_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/retry_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.652867 metaflow-2.9.6/metaflow/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/secrets/inline_secrets_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/secrets/secrets_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/storage_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/tag_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/test_unbounded_foreach_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/plugins/timeout_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/procpoll.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/pylint_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    55788 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.652867 metaflow-2.9.6/metaflow/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/sidecar/sidecar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/sidecar/sidecar_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/sidecar/sidecar_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/sidecar/sidecar_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tagging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25123 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.624867 metaflow-2.9.6/metaflow/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.652867 metaflow-2.9.6/metaflow/tutorials/00-helloworld/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/00-helloworld/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/00-helloworld/helloworld.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.652867 metaflow-2.9.6/metaflow/tutorials/01-playlist/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/01-playlist/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/01-playlist/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/01-playlist/playlist.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/01-playlist/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.652867 metaflow-2.9.6/metaflow/tutorials/02-statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/02-statistics/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/02-statistics/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/02-statistics/stats.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/02-statistics/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.652867 metaflow-2.9.6/metaflow/tutorials/03-playlist-redux/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/03-playlist-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/03-playlist-redux/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.652867 metaflow-2.9.6/metaflow/tutorials/04-playlist-plus/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/04-playlist-plus/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/04-playlist-plus/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.652867 metaflow-2.9.6/metaflow/tutorials/05-hello-cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/05-hello-cloud/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/05-hello-cloud/hello-cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.652867 metaflow-2.9.6/metaflow/tutorials/06-statistics-redux/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/06-statistics-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/06-statistics-redux/stats.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.656867 metaflow-2.9.6/metaflow/tutorials/07-worldview/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/07-worldview/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/07-worldview/worldview.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.656867 metaflow-2.9.6/metaflow/tutorials/08-autopilot/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/08-autopilot/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/tutorials/08-autopilot/autopilot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/unbounded_foreach.py
--rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-06-21 17:01:54.000000 metaflow-2.9.6/metaflow/vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:02:03.628867 metaflow-2.9.6/metaflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-21 17:02:03.000000 metaflow-2.9.6/metaflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-06-21 17:02:03.000000 metaflow-2.9.6/metaflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:02:03.000000 metaflow-2.9.6/metaflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-21 17:02:03.000000 metaflow-2.9.6/metaflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 17:02:03.000000 metaflow-2.9.6/metaflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 17:02:03.000000 metaflow-2.9.6/metaflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-21 17:02:03.656867 metaflow-2.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-21 17:01:54.000000 metaflow-2.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.482915 metaflow-2.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-27 10:21:55.000000 metaflow-2.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-27 10:21:55.000000 metaflow-2.9.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-27 10:22:04.482915 metaflow-2.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-06-27 10:21:55.000000 metaflow-2.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.458916 metaflow-2.9.7/metaflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/R.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.462916 metaflow-2.9.7/metaflow/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.462916 metaflow-2.9.7/metaflow/_vendor/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/click/_bashcomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/click/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/click/_termui_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/click/_textwrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/click/_unicodefun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/click/_winconsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/click/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/click/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/click/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/click/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/click/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/click/termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/click/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/click/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.462916 metaflow-2.9.7/metaflow/_vendor/v3_5/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/v3_5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.462916 metaflow-2.9.7/metaflow/_vendor/v3_5/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/v3_5/zipp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.462916 metaflow-2.9.7/metaflow/_vendor/v3_6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/v3_6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.462916 metaflow-2.9.7/metaflow/_vendor/v3_6/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/v3_6/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/v3_6/typing_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/_vendor/v3_6/zipp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35024 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/cli_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.462916 metaflow-2.9.7/metaflow/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69283 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/client/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/client/filecache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.462916 metaflow-2.9.7/metaflow/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33396 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/cmd/configure_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/cmd/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/cmd/tutorials_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/cmd/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/cmd_with_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/current.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.466915 metaflow-2.9.7/metaflow/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/datastore/content_addressed_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/datastore/datastore_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/datastore/datastore_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/datastore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/datastore/flow_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/datastore/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/datastore/task_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/event_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.466915 metaflow-2.9.7/metaflow/extension_support/
+-rw-r--r--   0 runner    (1001) docker     (123)    49461 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/extension_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/extension_support/_empty_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/extension_support/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/extension_support/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/extension_support/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/flowspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19721 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/includefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.466915 metaflow-2.9.7/metaflow/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/metadata/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/metadata/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18895 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/metaflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/metaflow_config_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/metaflow_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/metaflow_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/metaflow_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.466915 metaflow-2.9.7/metaflow/mflog/
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/mflog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/mflog/mflog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/mflog/save_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/mflog/save_logs_periodically.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/mflog/tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/multicore_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.466915 metaflow-2.9.7/metaflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.466915 metaflow-2.9.7/metaflow/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31445 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/airflow/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/airflow/airflow_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/airflow/airflow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/airflow/airflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/airflow/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/airflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.466915 metaflow-2.9.7/metaflow/plugins/airflow/plumbing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/airflow/plumbing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/airflow/plumbing/set_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.466915 metaflow-2.9.7/metaflow/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/airflow/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/airflow/sensors/base_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/airflow/sensors/external_task_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/airflow/sensors/s3_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.470916 metaflow-2.9.7/metaflow/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/argo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15266 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/argo/argo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/argo/argo_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108078 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/argo/argo_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31146 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/argo/argo_workflows_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/argo/argo_workflows_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/argo/process_input_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.470916 metaflow-2.9.7/metaflow/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/aws_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/aws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.470916 metaflow-2.9.7/metaflow/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16677 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/batch/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/batch/batch_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/batch/batch_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/batch/batch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.470916 metaflow-2.9.7/metaflow/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/secrets_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.470916 metaflow-2.9.7/metaflow/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/step_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/step_functions/dynamo_db_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/step_functions/event_bridge_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/step_functions/production_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/step_functions/schedule_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/step_functions/set_batch_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42848 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/step_functions/step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21420 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/step_functions/step_functions_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/step_functions/step_functions_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/aws/step_functions/step_functions_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.470916 metaflow-2.9.7/metaflow/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/azure/azure_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/azure/azure_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/azure/azure_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/azure/blob_service_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/azure/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.470916 metaflow-2.9.7/metaflow/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.474916 metaflow-2.9.7/metaflow/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_modules/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_modules/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_modules/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_modules/card.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.474916 metaflow-2.9.7/metaflow/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_modules/chevron/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_modules/chevron/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_modules/chevron/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_modules/chevron/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_modules/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_modules/convert_to_native_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_modules/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_modules/renderer_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_modules/test_cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/card_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/component_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/cards/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/catch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.474916 metaflow-2.9.7/metaflow/plugins/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/conda/batch_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/conda/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/conda/conda_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/conda/conda_flow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/conda/conda_step_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.474916 metaflow-2.9.7/metaflow/plugins/datastores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/datastores/azure_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/datastores/gs_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/datastores/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/datastores/s3_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.474916 metaflow-2.9.7/metaflow/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/datatools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/datatools/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.474916 metaflow-2.9.7/metaflow/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/datatools/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64840 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/datatools/s3/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43171 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/datatools/s3/s3op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/datatools/s3/s3tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/datatools/s3/s3util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/debug_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/debug_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.474916 metaflow-2.9.7/metaflow/plugins/env_escape/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/client_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.474916 metaflow-2.9.7/metaflow/plugins/env_escape/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/communication/bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/communication/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/communication/socket_bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/communication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.474916 metaflow-2.9.7/metaflow/plugins/env_escape/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/configurations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.478916 metaflow-2.9.7/metaflow/plugins/env_escape/configurations/emulate_test_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.478916 metaflow-2.9.7/metaflow/plugins/env_escape/configurations/test_lib_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/data_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/exception_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/override_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/env_escape/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/environment_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17724 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/events_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.478916 metaflow-2.9.7/metaflow/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/frameworks/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.478916 metaflow-2.9.7/metaflow/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/gcp/gs_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/gcp/gs_storage_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/gcp/gs_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/gcp/gs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/gcp/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.478916 metaflow-2.9.7/metaflow/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16678 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/kubernetes/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/kubernetes/kubernetes_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/kubernetes/kubernetes_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19933 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/kubernetes/kubernetes_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30448 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/kubernetes/kubernetes_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.478916 metaflow-2.9.7/metaflow/plugins/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/metadata/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/metadata/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/package_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/parallel_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/project_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/resources_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/retry_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.478916 metaflow-2.9.7/metaflow/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/secrets/inline_secrets_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/secrets/secrets_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/storage_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/tag_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/test_unbounded_foreach_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/plugins/timeout_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/procpoll.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/pylint_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55788 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.478916 metaflow-2.9.7/metaflow/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/sidecar/sidecar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/sidecar/sidecar_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/sidecar/sidecar_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/sidecar/sidecar_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tagging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25123 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.458916 metaflow-2.9.7/metaflow/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.478916 metaflow-2.9.7/metaflow/tutorials/00-helloworld/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/00-helloworld/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/00-helloworld/helloworld.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.478916 metaflow-2.9.7/metaflow/tutorials/01-playlist/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/01-playlist/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/01-playlist/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/01-playlist/playlist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/01-playlist/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.478916 metaflow-2.9.7/metaflow/tutorials/02-statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/02-statistics/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/02-statistics/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/02-statistics/stats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/02-statistics/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.478916 metaflow-2.9.7/metaflow/tutorials/03-playlist-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/03-playlist-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/03-playlist-redux/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.482915 metaflow-2.9.7/metaflow/tutorials/04-playlist-plus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/04-playlist-plus/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/04-playlist-plus/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.482915 metaflow-2.9.7/metaflow/tutorials/05-hello-cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/05-hello-cloud/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/05-hello-cloud/hello-cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.482915 metaflow-2.9.7/metaflow/tutorials/06-statistics-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/06-statistics-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/06-statistics-redux/stats.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.482915 metaflow-2.9.7/metaflow/tutorials/07-worldview/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/07-worldview/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/07-worldview/worldview.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.482915 metaflow-2.9.7/metaflow/tutorials/08-autopilot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/08-autopilot/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/tutorials/08-autopilot/autopilot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/unbounded_foreach.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-06-27 10:21:55.000000 metaflow-2.9.7/metaflow/vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:22:04.458916 metaflow-2.9.7/metaflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-27 10:22:04.000000 metaflow-2.9.7/metaflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-06-27 10:22:04.000000 metaflow-2.9.7/metaflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:22:04.000000 metaflow-2.9.7/metaflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-27 10:22:04.000000 metaflow-2.9.7/metaflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 10:22:04.000000 metaflow-2.9.7/metaflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 10:22:04.000000 metaflow-2.9.7/metaflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 10:22:04.482915 metaflow-2.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-27 10:21:55.000000 metaflow-2.9.7/setup.py
```

### Comparing `metaflow-2.9.6/LICENSE` & `metaflow-2.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/PKG-INFO` & `metaflow-2.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow
-Version: 2.9.6
+Version: 2.9.7
 Summary: Metaflow: More Data Science, Less Engineering
 Author: Metaflow Developers
 Author-email: help@metaflow.org
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow
 Project-URL: Issues, https://github.com/Netflix/metaflow/issues
 Project-URL: Documentation, https://docs.metaflow.org
```

### Comparing `metaflow-2.9.6/README.md` & `metaflow-2.9.7/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/R.py` & `metaflow-2.9.7/metaflow/R.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/__init__.py` & `metaflow-2.9.7/metaflow/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/click/__init__.py` & `metaflow-2.9.7/metaflow/_vendor/click/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/click/_bashcomplete.py` & `metaflow-2.9.7/metaflow/_vendor/click/_bashcomplete.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/click/_compat.py` & `metaflow-2.9.7/metaflow/_vendor/click/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/click/_termui_impl.py` & `metaflow-2.9.7/metaflow/_vendor/click/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/click/_textwrap.py` & `metaflow-2.9.7/metaflow/_vendor/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/click/_unicodefun.py` & `metaflow-2.9.7/metaflow/_vendor/click/_unicodefun.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/click/_winconsole.py` & `metaflow-2.9.7/metaflow/_vendor/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/click/core.py` & `metaflow-2.9.7/metaflow/_vendor/click/core.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/click/decorators.py` & `metaflow-2.9.7/metaflow/_vendor/click/decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/click/exceptions.py` & `metaflow-2.9.7/metaflow/_vendor/click/exceptions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/click/formatting.py` & `metaflow-2.9.7/metaflow/_vendor/click/formatting.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/click/globals.py` & `metaflow-2.9.7/metaflow/_vendor/click/globals.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/click/parser.py` & `metaflow-2.9.7/metaflow/_vendor/click/parser.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/click/termui.py` & `metaflow-2.9.7/metaflow/_vendor/click/termui.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/click/testing.py` & `metaflow-2.9.7/metaflow/_vendor/click/testing.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/click/types.py` & `metaflow-2.9.7/metaflow/_vendor/click/types.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/click/utils.py` & `metaflow-2.9.7/metaflow/_vendor/click/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/v3_5/importlib_metadata/__init__.py` & `metaflow-2.9.7/metaflow/_vendor/v3_5/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/v3_5/importlib_metadata/_compat.py` & `metaflow-2.9.7/metaflow/_vendor/v3_5/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/v3_5/zipp.py` & `metaflow-2.9.7/metaflow/_vendor/v3_5/zipp.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/v3_6/importlib_metadata/__init__.py` & `metaflow-2.9.7/metaflow/_vendor/v3_6/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py` & `metaflow-2.9.7/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/v3_6/importlib_metadata/_collections.py` & `metaflow-2.9.7/metaflow/_vendor/v3_6/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/v3_6/importlib_metadata/_compat.py` & `metaflow-2.9.7/metaflow/_vendor/v3_6/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/v3_6/importlib_metadata/_functools.py` & `metaflow-2.9.7/metaflow/_vendor/v3_6/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py` & `metaflow-2.9.7/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/v3_6/importlib_metadata/_meta.py` & `metaflow-2.9.7/metaflow/_vendor/v3_6/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/v3_6/importlib_metadata/_text.py` & `metaflow-2.9.7/metaflow/_vendor/v3_6/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/v3_6/typing_extensions.py` & `metaflow-2.9.7/metaflow/_vendor/v3_6/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/_vendor/v3_6/zipp.py` & `metaflow-2.9.7/metaflow/_vendor/v3_6/zipp.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/cli.py` & `metaflow-2.9.7/metaflow/cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/cli_args.py` & `metaflow-2.9.7/metaflow/cli_args.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/client/core.py` & `metaflow-2.9.7/metaflow/client/core.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/client/filecache.py` & `metaflow-2.9.7/metaflow/client/filecache.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/cmd/configure_cmd.py` & `metaflow-2.9.7/metaflow/cmd/configure_cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/cmd/main_cli.py` & `metaflow-2.9.7/metaflow/cmd/main_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/cmd/tutorials_cmd.py` & `metaflow-2.9.7/metaflow/cmd/tutorials_cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/cmd_with_io.py` & `metaflow-2.9.7/metaflow/cmd_with_io.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/current.py` & `metaflow-2.9.7/metaflow/current.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/datastore/content_addressed_store.py` & `metaflow-2.9.7/metaflow/datastore/content_addressed_store.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/datastore/datastore_set.py` & `metaflow-2.9.7/metaflow/datastore/datastore_set.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/datastore/datastore_storage.py` & `metaflow-2.9.7/metaflow/datastore/datastore_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/datastore/flow_datastore.py` & `metaflow-2.9.7/metaflow/datastore/flow_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/datastore/task_datastore.py` & `metaflow-2.9.7/metaflow/datastore/task_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/debug.py` & `metaflow-2.9.7/metaflow/debug.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/decorators.py` & `metaflow-2.9.7/metaflow/decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/event_logger.py` & `metaflow-2.9.7/metaflow/event_logger.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/events.py` & `metaflow-2.9.7/metaflow/events.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/exception.py` & `metaflow-2.9.7/metaflow/exception.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/extension_support/__init__.py` & `metaflow-2.9.7/metaflow/extension_support/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/extension_support/cmd.py` & `metaflow-2.9.7/metaflow/extension_support/cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/extension_support/integrations.py` & `metaflow-2.9.7/metaflow/extension_support/integrations.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/extension_support/plugins.py` & `metaflow-2.9.7/metaflow/extension_support/plugins.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/flowspec.py` & `metaflow-2.9.7/metaflow/flowspec.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/graph.py` & `metaflow-2.9.7/metaflow/graph.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/includefile.py` & `metaflow-2.9.7/metaflow/includefile.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/integrations.py` & `metaflow-2.9.7/metaflow/integrations.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/lint.py` & `metaflow-2.9.7/metaflow/lint.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/metadata/heartbeat.py` & `metaflow-2.9.7/metaflow/metadata/heartbeat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/metadata/metadata.py` & `metaflow-2.9.7/metaflow/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/metadata/util.py` & `metaflow-2.9.7/metaflow/metadata/util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/metaflow_config.py` & `metaflow-2.9.7/metaflow/metaflow_config.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/metaflow_config_funcs.py` & `metaflow-2.9.7/metaflow/metaflow_config_funcs.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/metaflow_environment.py` & `metaflow-2.9.7/metaflow/metaflow_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/metaflow_version.py` & `metaflow-2.9.7/metaflow/metaflow_version.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/mflog/__init__.py` & `metaflow-2.9.7/metaflow/mflog/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/mflog/mflog.py` & `metaflow-2.9.7/metaflow/mflog/mflog.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/mflog/save_logs.py` & `metaflow-2.9.7/metaflow/mflog/save_logs.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/mflog/save_logs_periodically.py` & `metaflow-2.9.7/metaflow/mflog/save_logs_periodically.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/mflog/tee.py` & `metaflow-2.9.7/metaflow/mflog/tee.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/monitor.py` & `metaflow-2.9.7/metaflow/monitor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/multicore_utils.py` & `metaflow-2.9.7/metaflow/multicore_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/package.py` & `metaflow-2.9.7/metaflow/package.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/parameters.py` & `metaflow-2.9.7/metaflow/parameters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/__init__.py` & `metaflow-2.9.7/metaflow/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/airflow/airflow.py` & `metaflow-2.9.7/metaflow/plugins/airflow/airflow.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/airflow/airflow_cli.py` & `metaflow-2.9.7/metaflow/plugins/airflow/airflow_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/airflow/airflow_decorator.py` & `metaflow-2.9.7/metaflow/plugins/airflow/airflow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/airflow/airflow_utils.py` & `metaflow-2.9.7/metaflow/plugins/airflow/airflow_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/airflow/plumbing/set_parameters.py` & `metaflow-2.9.7/metaflow/plugins/airflow/plumbing/set_parameters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/airflow/sensors/base_sensor.py` & `metaflow-2.9.7/metaflow/plugins/airflow/sensors/base_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/airflow/sensors/external_task_sensor.py` & `metaflow-2.9.7/metaflow/plugins/airflow/sensors/external_task_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/airflow/sensors/s3_sensor.py` & `metaflow-2.9.7/metaflow/plugins/airflow/sensors/s3_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/argo/argo_client.py` & `metaflow-2.9.7/metaflow/plugins/argo/argo_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,14 +13,32 @@
 class ArgoClient(object):
     def __init__(self, namespace=None):
         self._client = KubernetesClient()
         self._namespace = namespace or "default"
         self._group = "argoproj.io"
         self._version = "v1alpha1"
 
+    def get_workflow(self, name):
+        client = self._client.get()
+        try:
+            workflow = client.CustomObjectsApi().get_namespaced_custom_object(
+                group=self._group,
+                version=self._version,
+                namespace=self._namespace,
+                plural="workflows",
+                name=name,
+            )
+        except client.rest.ApiException as e:
+            if e.status == 404:
+                return None
+            raise ArgoClientException(
+                json.loads(e.body)["message"] if e.body is not None else e.reason
+            )
+        return workflow
+
     def get_workflow_template(self, name):
         client = self._client.get()
         try:
             return client.CustomObjectsApi().get_namespaced_custom_object(
                 group=self._group,
                 version=self._version,
                 namespace=self._namespace,
@@ -82,14 +100,148 @@
                 name=name,
             )
         except client.rest.ApiException as e:
             raise ArgoClientException(
                 json.loads(e.body)["message"] if e.body is not None else e.reason
             )
 
+    def delete_cronworkflow(self, name):
+        """
+        Issues an API call for deleting a cronworkflow
+
+        Returns either the successful API response, or None in case the resource was not found.
+        """
+        client = self._client.get()
+
+        try:
+            return client.CustomObjectsApi().delete_namespaced_custom_object(
+                group=self._group,
+                version=self._version,
+                namespace=self._namespace,
+                plural="cronworkflows",
+                name=name,
+            )
+        except client.rest.ApiException as e:
+            if e.status == 404:
+                return None
+            else:
+                raise ArgoClientException(
+                    json.loads(e.body)["message"] if e.body is not None else e.reason
+                )
+
+    def delete_workflow_template(self, name):
+        """
+        Issues an API call for deleting a cronworkflow
+
+        Returns either the successful API response, or None in case the resource was not found.
+        """
+        client = self._client.get()
+
+        try:
+            return client.CustomObjectsApi().delete_namespaced_custom_object(
+                group=self._group,
+                version=self._version,
+                namespace=self._namespace,
+                plural="workflowtemplates",
+                name=name,
+            )
+        except client.rest.ApiException as e:
+            if e.status == 404:
+                return None
+            else:
+                raise ArgoClientException(
+                    json.loads(e.body)["message"] if e.body is not None else e.reason
+                )
+
+    def terminate_workflow(self, run_id):
+        client = self._client.get()
+        try:
+            workflow = client.CustomObjectsApi().get_namespaced_custom_object(
+                group=self._group,
+                version=self._version,
+                namespace=self._namespace,
+                plural="workflows",
+                name=run_id,
+            )
+        except client.rest.ApiException as e:
+            raise ArgoClientException(
+                json.loads(e.body)["message"] if e.body is not None else e.reason
+            )
+
+        if workflow["status"]["finishedAt"] is not None:
+            raise ArgoClientException(
+                "Cannot terminate an execution that has already finished."
+            )
+        if workflow["spec"].get("shutdown") == "Terminate":
+            raise ArgoClientException("Execution has already been terminated.")
+
+        try:
+            body = {"spec": workflow["spec"]}
+            body["spec"]["shutdown"] = "Terminate"
+            return client.CustomObjectsApi().patch_namespaced_custom_object(
+                group=self._group,
+                version=self._version,
+                namespace=self._namespace,
+                plural="workflows",
+                name=run_id,
+                body=body,
+            )
+        except client.rest.ApiException as e:
+            raise ArgoClientException(
+                json.loads(e.body)["message"] if e.body is not None else e.reason
+            )
+
+    def suspend_workflow(self, name):
+        workflow = self.get_workflow(name)
+        if workflow is None:
+            raise ArgoClientException("Execution argo-%s was not found" % name)
+
+        if workflow["status"]["finishedAt"] is not None:
+            raise ArgoClientException(
+                "Cannot suspend an execution that has already finished."
+            )
+        if workflow["spec"].get("suspend") is True:
+            raise ArgoClientException("Execution has already been suspended.")
+
+        body = {"spec": workflow["spec"]}
+        body["spec"]["suspend"] = True
+        return self._patch_workflow(name, body)
+
+    def unsuspend_workflow(self, name):
+        workflow = self.get_workflow(name)
+        if workflow is None:
+            raise ArgoClientException("Execution argo-%s was not found" % name)
+
+        if workflow["status"]["finishedAt"] is not None:
+            raise ArgoClientException(
+                "Cannot unsuspend an execution that has already finished."
+            )
+        if not workflow["spec"].get("suspend", False):
+            raise ArgoClientException("Execution is already proceeding.")
+
+        body = {"spec": workflow["spec"]}
+        body["spec"]["suspend"] = False
+        return self._patch_workflow(name, body)
+
+    def _patch_workflow(self, name, body):
+        client = self._client.get()
+        try:
+            return client.CustomObjectsApi().patch_namespaced_custom_object(
+                group=self._group,
+                version=self._version,
+                namespace=self._namespace,
+                plural="workflows",
+                name=name,
+                body=body,
+            )
+        except client.rest.ApiException as e:
+            raise ArgoClientException(
+                json.loads(e.body)["message"] if e.body is not None else e.reason
+            )
+
     def trigger_workflow_template(self, name, parameters={}):
         client = self._client.get()
         body = {
             "apiVersion": "argoproj.io/v1alpha1",
             "kind": "Workflow",
             "metadata": {"generateName": name + "-"},
             "spec": {
@@ -203,16 +355,14 @@
                 "metadata"
             ][
                 "resourceVersion"
             ]
         except client.rest.ApiException as e:
             # Sensor does not exist and we want to add one
             if e.status == 404:
-                if sensor.get("kind") is None:
-                    return
                 try:
                     return client.CustomObjectsApi().create_namespaced_custom_object(
                         group=self._group,
                         version=self._version,
                         namespace=self._namespace,
                         plural="sensors",
                         body=sensor,
@@ -223,34 +373,43 @@
                         if e.body is not None
                         else e.reason
                     )
             else:
                 raise ArgoClientException(
                     json.loads(e.body)["message"] if e.body is not None else e.reason
                 )
-        # Since sensors occupy real resources, delete existing sensor if needed
-        if sensor.get("kind") is None:
-            try:
-                return client.CustomObjectsApi().delete_namespaced_custom_object(
-                    group=self._group,
-                    version=self._version,
-                    namespace=self._namespace,
-                    plural="sensors",
-                    name=name,
-                )
-            except client.rest.ApiException as e:
-                raise ArgoClientException(
-                    json.loads(e.body)["message"] if e.body is not None else e.reason
-                )
         try:
             return client.CustomObjectsApi().replace_namespaced_custom_object(
                 group=self._group,
                 version=self._version,
                 namespace=self._namespace,
                 plural="sensors",
                 body=sensor,
                 name=name,
             )
         except client.rest.ApiException as e:
             raise ArgoClientException(
                 json.loads(e.body)["message"] if e.body is not None else e.reason
             )
+
+    def delete_sensor(self, name):
+        """
+        Issues an API call for deleting a sensor
+
+        Returns either the successful API response, or None in case the resource was not found.
+        """
+        client = self._client.get()
+
+        try:
+            return client.CustomObjectsApi().delete_namespaced_custom_object(
+                group=self._group,
+                version=self._version,
+                namespace=self._namespace,
+                plural="sensors",
+                name=name,
+            )
+        except client.rest.ApiException as e:
+            if e.status == 404:
+                return None
+            raise ArgoClientException(
+                json.loads(e.body)["message"] if e.body is not None else e.reason
+            )
```

### Comparing `metaflow-2.9.6/metaflow/plugins/argo/argo_events.py` & `metaflow-2.9.7/metaflow/plugins/argo/argo_events.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/argo/argo_workflows.py` & `metaflow-2.9.7/metaflow/plugins/argo/argo_workflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,14 +171,68 @@
     @staticmethod
     def _sanitize(name):
         # Metaflow allows underscores in node names, which are disallowed in Argo
         # Workflow template names - so we swap them with hyphens which are not
         # allowed by Metaflow - guaranteeing uniqueness.
         return name.replace("_", "-")
 
+    @staticmethod
+    def delete(name):
+        client = ArgoClient(namespace=KUBERNETES_NAMESPACE)
+
+        # Always try to delete the schedule. Failure in deleting the schedule should not
+        # be treated as an error, due to any of the following reasons
+        # - there might not have been a schedule, or it was deleted by some other means
+        # - retaining these resources should have no consequences as long as the workflow deletion succeeds.
+        # - regarding cost and compute, the significant resources are part of the workflow teardown, not the schedule.
+        schedule_deleted = client.delete_cronworkflow(name)
+
+        # The workflow might have sensors attached to it, which consume actual resources.
+        # Try to delete these as well.
+        sensor_deleted = client.delete_sensor(name)
+
+        # After cleaning up related resources, delete the workflow in question.
+        # Failure in deleting is treated as critical and will be made visible to the user
+        # for further action.
+        workflow_deleted = client.delete_workflow_template(name)
+        if workflow_deleted is None:
+            raise ArgoWorkflowsException(
+                "The workflow *%s* doesn't exist on Argo Workflows." % name
+            )
+
+        return schedule_deleted, sensor_deleted, workflow_deleted
+
+    @staticmethod
+    def terminate(flow_name, name):
+        client = ArgoClient(namespace=KUBERNETES_NAMESPACE)
+
+        response = client.terminate_workflow(name)
+        if response is None:
+            raise ArgoWorkflowsException(
+                "No execution found for {flow_name}/{run_id} in Argo Workflows.".format(
+                    flow_name=flow_name, run_id=name
+                )
+            )
+
+    @staticmethod
+    def suspend(name):
+        client = ArgoClient(namespace=KUBERNETES_NAMESPACE)
+
+        client.suspend_workflow(name)
+
+        return True
+
+    @staticmethod
+    def unsuspend(name):
+        client = ArgoClient(namespace=KUBERNETES_NAMESPACE)
+
+        client.unsuspend_workflow(name)
+
+        return True
+
     @classmethod
     def trigger(cls, name, parameters=None):
         if parameters is None:
             parameters = {}
         try:
             workflow_template = ArgoClient(
                 namespace=KUBERNETES_NAMESPACE
@@ -227,24 +281,28 @@
             # Remove the field "Year" if it exists
             schedule = schedule[0]
             return " ".join(schedule.schedule.split()[:5]), schedule.timezone
         return None, None
 
     def schedule(self):
         try:
-            ArgoClient(namespace=KUBERNETES_NAMESPACE).schedule_workflow_template(
+            argo_client = ArgoClient(namespace=KUBERNETES_NAMESPACE)
+            argo_client.schedule_workflow_template(
                 self.name, self._schedule, self._timezone
             )
             # Register sensor. Unfortunately, Argo Events Sensor names don't allow for
             # dots (sensors run into an error) which rules out self.name :(
             # Metaflow will overwrite any existing sensor.
-            ArgoClient(namespace=KUBERNETES_NAMESPACE).register_sensor(
-                self.name.replace(".", "-"),
-                self._sensor.to_json() if self._sensor else {},
-            )
+            sensor_name = self.name.replace(".", "-")
+            if self._sensor:
+                argo_client.register_sensor(sensor_name, self._sensor.to_json())
+            else:
+                # Since sensors occupy real resources, delete existing sensor if needed
+                # Deregister sensors that might have existed before this deployment
+                argo_client.delete_sensor(sensor_name)
         except Exception as e:
             raise ArgoWorkflowsSchedulingException(str(e))
 
     def trigger_explanation(self):
         # Trigger explanation for cron workflows
         if self.flow._flow_decorators.get("schedule"):
             return (
@@ -297,14 +355,37 @@
                     "An existing non-metaflow workflow with the same name as "
                     "*%s* already exists in Argo Workflows. \nPlease modify the "
                     "name of this flow or delete your existing workflow on Argo "
                     "Workflows before proceeding." % name
                 )
         return None
 
+    @classmethod
+    def get_execution(cls, name):
+        workflow = ArgoClient(namespace=KUBERNETES_NAMESPACE).get_workflow(name)
+        if workflow is not None:
+            try:
+                return (
+                    workflow["metadata"]["annotations"]["metaflow/owner"],
+                    workflow["metadata"]["annotations"]["metaflow/production_token"],
+                    workflow["metadata"]["annotations"]["metaflow/flow_name"],
+                    workflow["metadata"]["annotations"].get(
+                        "metaflow/branch_name", None
+                    ),
+                    workflow["metadata"]["annotations"].get(
+                        "metaflow/project_name", None
+                    ),
+                )
+            except KeyError:
+                raise ArgoWorkflowsException(
+                    "A non-metaflow workflow *%s* already exists in Argo Workflows."
+                    % name
+                )
+        return None
+
     def _process_parameters(self):
         parameters = {}
         has_schedule = self.flow._flow_decorators.get("schedule") is not None
         seen = set()
         for var, param in self.flow._get_parameters():
             # Throw an exception if the parameter is specified twice.
             norm = param.name.lower()
```

### Comparing `metaflow-2.9.6/metaflow/plugins/argo/argo_workflows_cli.py` & `metaflow-2.9.7/metaflow/plugins/argo/argo_workflows_cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -33,14 +33,18 @@
 VALID_NAME = re.compile("^[a-z0-9]([a-z0-9\.\-]*[a-z0-9])?$")
 
 
 class IncorrectProductionToken(MetaflowException):
     headline = "Incorrect production token"
 
 
+class RunIdMismatch(MetaflowException):
+    headline = "Run ID mismatch"
+
+
 class IncorrectMetadataServiceVersion(MetaflowException):
     headline = "Incorrect version for metaflow service"
 
 
 class ArgoWorkflowsNameTooLong(MetaflowException):
     headline = "Argo Workflows name too long"
 
@@ -331,22 +335,15 @@
         if len(workflow_name) > 253:
             name_hash = to_unicode(
                 base64.b32encode(sha1(to_bytes(workflow_name)).digest())
             )[:8].lower()
             workflow_name = "%s-%s" % (workflow_name[:242], name_hash)
             obj._is_workflow_name_modified = True
         if not VALID_NAME.search(workflow_name):
-            workflow_name = (
-                re.compile(r"^[^A-Za-z0-9]+")
-                .sub("", workflow_name)
-                .replace("_", "")
-                .replace("@", "")
-                .replace("+", "")
-                .lower()
-            )
+            workflow_name = sanitize_for_argo(workflow_name)
             obj._is_workflow_name_modified = True
     else:
         if name and not VALID_NAME.search(name):
             raise MetaflowException(
                 "Name '%s' contains invalid characters. The "
                 "name must consist of lower case alphanumeric characters, '-' or '.'"
                 ", and must start and end with an alphanumeric character." % name
@@ -363,22 +360,15 @@
                 "To deploy this workflow to Argo Workflows, please "
                 "assign a shorter name\nusing the option\n"
                 "*argo-workflows --name <name> create*." % workflow_name
             )
             raise ArgoWorkflowsNameTooLong(msg)
 
         if not VALID_NAME.search(workflow_name):
-            workflow_name = (
-                re.compile(r"^[^A-Za-z0-9]+")
-                .sub("", workflow_name)
-                .replace("_", "")
-                .replace("@", "")
-                .replace("+", "")
-                .lower()
-            )
+            workflow_name = sanitize_for_argo(workflow_name)
             obj._is_workflow_name_modified = True
 
     return workflow_name, token_prefix.lower(), is_project
 
 
 def make_flow(
     obj,
@@ -596,7 +586,322 @@
     )
 
     if run_url:
         obj.echo(
             "See the run in the UI at %s" % run_url,
             bold=True,
         )
+
+
+@argo_workflows.command(help="Delete the flow on Argo Workflows.")
+@click.option(
+    "--authorize",
+    default=None,
+    type=str,
+    help="Authorize the deletion with a production token",
+)
+@click.pass_obj
+def delete(obj, authorize=None):
+    def _token_instructions(flow_name, prev_user):
+        obj.echo(
+            "There is an existing version of *%s* on Argo Workflows which was "
+            "deployed by the user *%s*." % (flow_name, prev_user)
+        )
+        obj.echo(
+            "To delete this flow, you need to use the same production token that they used."
+        )
+        obj.echo(
+            "Please reach out to them to get the token. Once you have it, call "
+            "this command:"
+        )
+        obj.echo("    argo-workflows delete --authorize MY_TOKEN", fg="green")
+        obj.echo(
+            'See "Organizing Results" at docs.metaflow.org for more information '
+            "about production tokens."
+        )
+
+    validate_token(obj.workflow_name, obj.token_prefix, authorize, _token_instructions)
+    obj.echo("Deleting workflow *{name}*...".format(name=obj.workflow_name), bold=True)
+
+    schedule_deleted, sensor_deleted, workflow_deleted = ArgoWorkflows.delete(
+        obj.workflow_name
+    )
+
+    if schedule_deleted:
+        obj.echo(
+            "Deleting cronworkflow *{name}*...".format(name=obj.workflow_name),
+            bold=True,
+        )
+
+    if sensor_deleted:
+        obj.echo(
+            "Deleting sensor *{name}*...".format(name=obj.workflow_name),
+            bold=True,
+        )
+
+    if workflow_deleted:
+        obj.echo(
+            "Deleting Kubernetes resources may take a while. "
+            "Deploying the flow again to Argo Workflows while the delete is in-flight will fail."
+        )
+        obj.echo(
+            "In-flight executions will not be affected. "
+            "If necessary, terminate them manually."
+        )
+
+
+@argo_workflows.command(help="Suspend flow execution on Argo Workflows.")
+@click.option(
+    "--authorize",
+    default=None,
+    type=str,
+    help="Authorize the suspension with a production token",
+)
+@click.argument("run-id", required=True, type=str)
+@click.pass_obj
+def suspend(obj, run_id, authorize=None):
+    def _token_instructions(flow_name, prev_user):
+        obj.echo(
+            "There is an existing version of *%s* on Argo Workflows which was "
+            "deployed by the user *%s*." % (flow_name, prev_user)
+        )
+        obj.echo(
+            "To suspend this flow, you need to use the same production token that they used."
+        )
+        obj.echo(
+            "Please reach out to them to get the token. Once you have it, call "
+            "this command:"
+        )
+        obj.echo("    argo-workflows suspend RUN_ID --authorize MY_TOKEN", fg="green")
+        obj.echo(
+            'See "Organizing Results" at docs.metaflow.org for more information '
+            "about production tokens."
+        )
+
+    validate_run_id(
+        obj.workflow_name, obj.token_prefix, authorize, run_id, _token_instructions
+    )
+
+    # Trim prefix from run_id
+    name = run_id[5:]
+
+    workflow_suspended = ArgoWorkflows.suspend(name)
+
+    if workflow_suspended:
+        obj.echo("Suspended execution of *%s*" % run_id)
+
+
+@argo_workflows.command(help="Unsuspend flow execution on Argo Workflows.")
+@click.option(
+    "--authorize",
+    default=None,
+    type=str,
+    help="Authorize the unsuspend with a production token",
+)
+@click.argument("run-id", required=True, type=str)
+@click.pass_obj
+def unsuspend(obj, run_id, authorize=None):
+    def _token_instructions(flow_name, prev_user):
+        obj.echo(
+            "There is an existing version of *%s* on Argo Workflows which was "
+            "deployed by the user *%s*." % (flow_name, prev_user)
+        )
+        obj.echo(
+            "To unsuspend this flow, you need to use the same production token that they used."
+        )
+        obj.echo(
+            "Please reach out to them to get the token. Once you have it, call "
+            "this command:"
+        )
+        obj.echo(
+            "    argo-workflows unsuspend RUN_ID --authorize MY_TOKEN",
+            fg="green",
+        )
+        obj.echo(
+            'See "Organizing Results" at docs.metaflow.org for more information '
+            "about production tokens."
+        )
+
+    validate_run_id(
+        obj.workflow_name, obj.token_prefix, authorize, run_id, _token_instructions
+    )
+
+    # Trim prefix from run_id
+    name = run_id[5:]
+
+    workflow_suspended = ArgoWorkflows.unsuspend(name)
+
+    if workflow_suspended:
+        obj.echo("Unsuspended execution of *%s*" % run_id)
+
+
+def validate_token(name, token_prefix, authorize, instructions_fn=None):
+    """
+    Validate that the production token matches that of the deployed flow.
+    In case both the user and token do not match, raises an error.
+    Optionally outputs instructions on token usage via the provided instruction_fn(flow_name, prev_user)
+    """
+    # TODO: Unify this with the existing resolve_token implementation.
+
+    # 1) retrieve the previous deployment, if one exists
+    workflow = ArgoWorkflows.get_existing_deployment(name)
+    if workflow is None:
+        prev_token = None
+    else:
+        prev_user, prev_token = workflow
+
+    # 2) authorize this deployment
+    if prev_token is not None:
+        if authorize is None:
+            authorize = load_token(token_prefix)
+        elif authorize.startswith("production:"):
+            authorize = authorize[11:]
+
+        # we allow the user who deployed the previous version to re-deploy,
+        # even if they don't have the token
+        # NOTE: The username is visible in multiple sources, and can be set by the user.
+        # Should we consider being stricter here?
+        if prev_user != get_username() and authorize != prev_token:
+            if instructions_fn:
+                instructions_fn(flow_name=name, prev_user=prev_user)
+            raise IncorrectProductionToken(
+                "Try again with the correct production token."
+            )
+
+    # 3) all validations passed, store the previous token for future use
+    token = prev_token
+
+    store_token(token_prefix, token)
+    return True
+
+
+@argo_workflows.command(help="Terminate flow execution on Argo Workflows.")
+@click.option(
+    "--authorize",
+    default=None,
+    type=str,
+    help="Authorize the termination with a production token",
+)
+@click.argument("run-id", required=True, type=str)
+@click.pass_obj
+def terminate(obj, run_id, authorize=None):
+    def _token_instructions(flow_name, prev_user):
+        obj.echo(
+            "There is an existing version of *%s* on Argo Workflows which was "
+            "deployed by the user *%s*." % (flow_name, prev_user)
+        )
+        obj.echo(
+            "To terminate this flow, you need to use the same production token that they used."
+        )
+        obj.echo(
+            "Please reach out to them to get the token. Once you have it, call "
+            "this command:"
+        )
+        obj.echo("    argo-workflows terminate --authorize MY_TOKEN RUN_ID", fg="green")
+        obj.echo(
+            'See "Organizing Results" at docs.metaflow.org for more information '
+            "about production tokens."
+        )
+
+    validate_run_id(
+        obj.workflow_name, obj.token_prefix, authorize, run_id, _token_instructions
+    )
+
+    # Trim prefix from run_id
+    name = run_id[5:]
+    obj.echo(
+        "Terminating run *{run_id}* for {flow_name} ...".format(
+            run_id=run_id, flow_name=obj.flow.name
+        ),
+        bold=True,
+    )
+
+    terminated = ArgoWorkflows.terminate(obj.flow.name, name)
+    if terminated:
+        obj.echo("\nRun terminated.")
+
+
+def validate_run_id(
+    workflow_name, token_prefix, authorize, run_id, instructions_fn=None
+):
+    """
+    Validates that a run_id adheres to the Argo Workflows naming rules, and
+    that it belongs to the current flow (accounting for project branch as well).
+    """
+    # Verify that user is trying to change an Argo workflow
+    if not run_id.startswith("argo-"):
+        raise RunIdMismatch(
+            "Run IDs for flows executed through Argo Workflows begin with 'argo-'"
+        )
+
+    # Verify that run_id belongs to the Flow, and that branches match
+    name = run_id[5:]
+    workflow = ArgoWorkflows.get_execution(name)
+    if workflow is None:
+        raise MetaflowException("Could not find workflow *%s* on Argo Workflows" % name)
+
+    owner, token, flow_name, branch_name, project_name = workflow
+
+    # Verify we are operating on the correct Flow file compared to the running one.
+    # Without this check, using --name could be used to run commands for arbitrary run_id's, disregarding the Flow in the file.
+    if current.flow_name != flow_name:
+        raise RunIdMismatch(
+            "The workflow with the run_id *%s* belongs to the flow *%s*, not for the flow *%s*."
+            % (run_id, flow_name, current.flow_name)
+        )
+
+    if project_name is not None:
+        # Verify we are operating on the correct project.
+        # Perform match with separators to avoid substrings matching
+        # e.g. 'test_proj' and 'test_project' should count as a mismatch.
+        project_part = "%s." % sanitize_for_argo(project_name)
+        if (
+            current.get("project_name") != project_name
+            and project_part not in workflow_name
+        ):
+            raise RunIdMismatch(
+                "The workflow belongs to the project *%s*. "
+                "Please use the project decorator or --name to target the correct project"
+                % project_name
+            )
+
+        # Verify we are operating on the correct branch.
+        # Perform match with separators to avoid substrings matching.
+        # e.g. 'user.tes' and 'user.test' should count as a mismatch.
+        branch_part = ".%s." % sanitize_for_argo(branch_name)
+        if (
+            current.get("branch_name") != branch_name
+            and branch_part not in workflow_name
+        ):
+            raise RunIdMismatch(
+                "The workflow belongs to the branch *%s*. "
+                "Please use --branch, --production or --name to target the correct branch"
+                % branch_name
+            )
+
+    # Verify that the production tokens match. We do not want to cache the token that was used though,
+    # as the operations that require run_id validation can target runs not authored from the local environment
+    if authorize is None:
+        authorize = load_token(token_prefix)
+    elif authorize.startswith("production:"):
+        authorize = authorize[11:]
+
+    if owner != get_username() and authorize != token:
+        if instructions_fn:
+            instructions_fn(flow_name=name, prev_user=owner)
+        raise IncorrectProductionToken("Try again with the correct production token.")
+
+    return True
+
+
+def sanitize_for_argo(text):
+    """
+    Sanitizes a string so it does not contain characters that are not permitted in Argo Workflow resource names.
+    """
+    return (
+        re.compile(r"^[^A-Za-z0-9]+")
+        .sub("", text)
+        .replace("_", "")
+        .replace("@", "")
+        .replace("+", "")
+        .lower()
+    )
```

### Comparing `metaflow-2.9.6/metaflow/plugins/argo/argo_workflows_decorator.py` & `metaflow-2.9.7/metaflow/plugins/argo/argo_workflows_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/argo/process_input_paths.py` & `metaflow-2.9.7/metaflow/plugins/argo/process_input_paths.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/aws/aws_client.py` & `metaflow-2.9.7/metaflow/plugins/aws/aws_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/aws/aws_utils.py` & `metaflow-2.9.7/metaflow/plugins/aws/aws_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/aws/batch/batch.py` & `metaflow-2.9.7/metaflow/plugins/aws/batch/batch.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/aws/batch/batch_cli.py` & `metaflow-2.9.7/metaflow/plugins/aws/batch/batch_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/aws/batch/batch_client.py` & `metaflow-2.9.7/metaflow/plugins/aws/batch/batch_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/aws/batch/batch_decorator.py` & `metaflow-2.9.7/metaflow/plugins/aws/batch/batch_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py` & `metaflow-2.9.7/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/aws/step_functions/dynamo_db_client.py` & `metaflow-2.9.7/metaflow/plugins/aws/step_functions/dynamo_db_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/aws/step_functions/event_bridge_client.py` & `metaflow-2.9.7/metaflow/plugins/aws/step_functions/event_bridge_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/aws/step_functions/production_token.py` & `metaflow-2.9.7/metaflow/plugins/aws/step_functions/production_token.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/aws/step_functions/schedule_decorator.py` & `metaflow-2.9.7/metaflow/plugins/aws/step_functions/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/aws/step_functions/set_batch_environment.py` & `metaflow-2.9.7/metaflow/plugins/aws/step_functions/set_batch_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/aws/step_functions/step_functions.py` & `metaflow-2.9.7/metaflow/plugins/aws/step_functions/step_functions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/aws/step_functions/step_functions_cli.py` & `metaflow-2.9.7/metaflow/plugins/aws/step_functions/step_functions_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/aws/step_functions/step_functions_client.py` & `metaflow-2.9.7/metaflow/plugins/aws/step_functions/step_functions_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/aws/step_functions/step_functions_decorator.py` & `metaflow-2.9.7/metaflow/plugins/aws/step_functions/step_functions_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/azure/azure_tail.py` & `metaflow-2.9.7/metaflow/plugins/azure/azure_tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/azure/azure_utils.py` & `metaflow-2.9.7/metaflow/plugins/azure/azure_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/azure/blob_service_client_factory.py` & `metaflow-2.9.7/metaflow/plugins/azure/blob_service_client_factory.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/azure/includefile_support.py` & `metaflow-2.9.7/metaflow/plugins/azure/includefile_support.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/card_cli.py` & `metaflow-2.9.7/metaflow/plugins/cards/card_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/card_client.py` & `metaflow-2.9.7/metaflow/plugins/cards/card_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/card_datastore.py` & `metaflow-2.9.7/metaflow/plugins/cards/card_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/card_decorator.py` & `metaflow-2.9.7/metaflow/plugins/cards/card_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/card_modules/__init__.py` & `metaflow-2.9.7/metaflow/plugins/cards/card_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/card_modules/base.html` & `metaflow-2.9.7/metaflow/plugins/cards/card_modules/base.html`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/card_modules/basic.py` & `metaflow-2.9.7/metaflow/plugins/cards/card_modules/basic.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/card_modules/bundle.css` & `metaflow-2.9.7/metaflow/plugins/cards/card_modules/bundle.css`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/card_modules/card.py` & `metaflow-2.9.7/metaflow/plugins/cards/card_modules/card.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/card_modules/chevron/main.py` & `metaflow-2.9.7/metaflow/plugins/cards/card_modules/chevron/main.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/card_modules/chevron/renderer.py` & `metaflow-2.9.7/metaflow/plugins/cards/card_modules/chevron/renderer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/card_modules/chevron/tokenizer.py` & `metaflow-2.9.7/metaflow/plugins/cards/card_modules/chevron/tokenizer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/card_modules/components.py` & `metaflow-2.9.7/metaflow/plugins/cards/card_modules/components.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/card_modules/convert_to_native_type.py` & `metaflow-2.9.7/metaflow/plugins/cards/card_modules/convert_to_native_type.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/card_modules/main.js` & `metaflow-2.9.7/metaflow/plugins/cards/card_modules/main.js`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/card_modules/renderer_tools.py` & `metaflow-2.9.7/metaflow/plugins/cards/card_modules/renderer_tools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/card_modules/test_cards.py` & `metaflow-2.9.7/metaflow/plugins/cards/card_modules/test_cards.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/card_resolver.py` & `metaflow-2.9.7/metaflow/plugins/cards/card_resolver.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/component_serializer.py` & `metaflow-2.9.7/metaflow/plugins/cards/component_serializer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/cards/exception.py` & `metaflow-2.9.7/metaflow/plugins/cards/exception.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/catch_decorator.py` & `metaflow-2.9.7/metaflow/plugins/catch_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/conda/__init__.py` & `metaflow-2.9.7/metaflow/plugins/conda/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/conda/batch_bootstrap.py` & `metaflow-2.9.7/metaflow/plugins/conda/batch_bootstrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/conda/conda.py` & `metaflow-2.9.7/metaflow/plugins/conda/conda.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/conda/conda_environment.py` & `metaflow-2.9.7/metaflow/plugins/conda/conda_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/conda/conda_flow_decorator.py` & `metaflow-2.9.7/metaflow/plugins/conda/conda_flow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/conda/conda_step_decorator.py` & `metaflow-2.9.7/metaflow/plugins/conda/conda_step_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/datastores/azure_storage.py` & `metaflow-2.9.7/metaflow/plugins/datastores/azure_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/datastores/gs_storage.py` & `metaflow-2.9.7/metaflow/plugins/datastores/gs_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/datastores/local_storage.py` & `metaflow-2.9.7/metaflow/plugins/datastores/local_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/datastores/s3_storage.py` & `metaflow-2.9.7/metaflow/plugins/datastores/s3_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/datatools/__init__.py` & `metaflow-2.9.7/metaflow/plugins/datatools/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/datatools/local.py` & `metaflow-2.9.7/metaflow/plugins/datatools/local.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/datatools/s3/s3.py` & `metaflow-2.9.7/metaflow/plugins/datatools/s3/s3.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/datatools/s3/s3op.py` & `metaflow-2.9.7/metaflow/plugins/datatools/s3/s3op.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/datatools/s3/s3tail.py` & `metaflow-2.9.7/metaflow/plugins/datatools/s3/s3tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/datatools/s3/s3util.py` & `metaflow-2.9.7/metaflow/plugins/datatools/s3/s3util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/debug_logger.py` & `metaflow-2.9.7/metaflow/plugins/debug_logger.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/debug_monitor.py` & `metaflow-2.9.7/metaflow/plugins/debug_monitor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/env_escape/__init__.py` & `metaflow-2.9.7/metaflow/plugins/env_escape/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/env_escape/client.py` & `metaflow-2.9.7/metaflow/plugins/env_escape/client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/env_escape/client_modules.py` & `metaflow-2.9.7/metaflow/plugins/env_escape/client_modules.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/env_escape/communication/bytestream.py` & `metaflow-2.9.7/metaflow/plugins/env_escape/communication/bytestream.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/env_escape/communication/channel.py` & `metaflow-2.9.7/metaflow/plugins/env_escape/communication/channel.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/env_escape/communication/socket_bytestream.py` & `metaflow-2.9.7/metaflow/plugins/env_escape/communication/socket_bytestream.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/env_escape/communication/utils.py` & `metaflow-2.9.7/metaflow/plugins/env_escape/communication/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py` & `metaflow-2.9.7/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py` & `metaflow-2.9.7/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py` & `metaflow-2.9.7/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/env_escape/consts.py` & `metaflow-2.9.7/metaflow/plugins/env_escape/consts.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/env_escape/data_transferer.py` & `metaflow-2.9.7/metaflow/plugins/env_escape/data_transferer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/env_escape/exception_transferer.py` & `metaflow-2.9.7/metaflow/plugins/env_escape/exception_transferer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/env_escape/override_decorators.py` & `metaflow-2.9.7/metaflow/plugins/env_escape/override_decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/env_escape/server.py` & `metaflow-2.9.7/metaflow/plugins/env_escape/server.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/env_escape/stub.py` & `metaflow-2.9.7/metaflow/plugins/env_escape/stub.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/env_escape/utils.py` & `metaflow-2.9.7/metaflow/plugins/env_escape/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/environment_decorator.py` & `metaflow-2.9.7/metaflow/plugins/environment_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/events_decorator.py` & `metaflow-2.9.7/metaflow/plugins/events_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/frameworks/pytorch.py` & `metaflow-2.9.7/metaflow/plugins/frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/gcp/gs_storage_client_factory.py` & `metaflow-2.9.7/metaflow/plugins/gcp/gs_storage_client_factory.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/gcp/gs_tail.py` & `metaflow-2.9.7/metaflow/plugins/gcp/gs_tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/gcp/gs_utils.py` & `metaflow-2.9.7/metaflow/plugins/gcp/gs_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/gcp/includefile_support.py` & `metaflow-2.9.7/metaflow/plugins/gcp/includefile_support.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/kubernetes/kubernetes.py` & `metaflow-2.9.7/metaflow/plugins/kubernetes/kubernetes.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/kubernetes/kubernetes_cli.py` & `metaflow-2.9.7/metaflow/plugins/kubernetes/kubernetes_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/kubernetes/kubernetes_client.py` & `metaflow-2.9.7/metaflow/plugins/kubernetes/kubernetes_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/kubernetes/kubernetes_decorator.py` & `metaflow-2.9.7/metaflow/plugins/kubernetes/kubernetes_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/kubernetes/kubernetes_job.py` & `metaflow-2.9.7/metaflow/plugins/kubernetes/kubernetes_job.py`

 * *Files 11% similar despite different names*

```diff
@@ -510,38 +510,32 @@
         if self._pod:
             self._pod_name = self._pod["metadata"]["name"]
             return self.id
         return "job %s" % self._name
 
     @property
     def is_done(self):
-        # Check if the job is done. As a side effect, also refreshes self._job and
+        # Check if the container is done. As a side effect, also refreshes self._job and
         # self._pod with the latest state
         def done():
-            # Either the job succeeds or fails naturally or else we may have
+            # Either the container succeeds or fails naturally or else we may have
             # forced the pod termination causing the job to still be in an
             # active state but for all intents and purposes dead to us.
             return (
                 bool(self._job["status"].get("succeeded"))
                 or bool(self._job["status"].get("failed"))
+                or self._are_pod_containers_done
                 or (self._job["spec"]["parallelism"] == 0)
             )
 
         if not done():
             # If not done, fetch newer status
             self._job = self._fetch_job()
-        if done():
-            return True
-        else:
-            # It is possible for the job metadata to not be updated yet, but the
-            # pod may have already succeeded or failed.
             self._pod = self._fetch_pod()
-            return self._pod and (
-                self._pod.get("status", {}).get("phase") in ("Succeeded", "Failed")
-            )
+        return done()
 
     @property
     def status(self):
         if not self.is_done:
             if bool(self._job["status"].get("active")):
                 if self._pod:
                     msg = (
@@ -573,36 +567,110 @@
                     return msg
                 return "Job is active"
             return "Job status is unknown"
         return "Job is done"
 
     @property
     def has_succeeded(self):
-        # Job is in a terminal state and the status is marked as succeeded
-        return self.is_done and (
-            bool(self._job["status"].get("succeeded"))
-            or (self._pod.get("status", {}).get("phase") == "Succeeded")
-        )
+        # The tasks container is in a terminal state and the status is marked as succeeded
+        return self.is_done and self._have_containers_succeeded
 
     @property
     def has_failed(self):
-        # Job is in a terminal state and either the status is marked as failed
-        # or the Job is not allowed to launch any more pods
-        return self.is_done and (
+        # Either the container is marked as failed or the Job is not allowed to
+        # any more pods
+        retval = self.is_done and (
             bool(self._job["status"].get("failed"))
+            or self._has_any_container_failed
             or (self._job["spec"]["parallelism"] == 0)
-            or (self._pod.get("status", {}).get("phase") == "Failed")
         )
+        return retval
+
+    @property
+    def _have_containers_succeeded(self):
+        container_statuses = self._pod.get("status", {}).get("container_statuses", [])
+        if not container_statuses:
+            return False
+
+        for cstatus in container_statuses:
+            # If the terminated field is not set, the pod is still running.
+            terminated = cstatus.get("state", {}).get("terminated", {})
+            if not terminated:
+                return False
+
+            # If the terminated field is set but the `finished_at` field is not set,
+            # the pod is still considered as running.
+            if not terminated.get("finished_at"):
+                return False
+
+            # If finished_at is set AND reason is Completed
+            if terminated.get("reason", "").lower() != "completed":
+                return False
+
+        return True
+
+    @property
+    def _has_any_container_failed(self):
+        container_statuses = self._pod.get("status", {}).get("container_statuses", [])
+        if not container_statuses:
+            return False
+
+        for cstatus in container_statuses:
+            # If the terminated field is not set, the pod is still running. Too early
+            # to determine if any container failed.
+            terminated = cstatus.get("state", {}).get("terminated", {})
+            if not terminated:
+                return False
+
+            # If the terminated field is set but the `finished_at` field is not set,
+            # the pod is still considered as running. Too early to determine if any
+            # container failed.
+            if not terminated.get("finished_at"):
+                return False
+
+            # If finished_at is set AND reason is Error, it means that the
+            # container failed.
+            if terminated.get("reason", "").lower() == "error":
+                return True
+
+        # If none of the containers are marked as failed, the pod is not
+        # considered failed.
+        return False
+
+    @property
+    def _are_pod_containers_done(self):
+        # All containers in the pod have a containerStatus that has a
+        # finishedAt set.
+        container_statuses = self._pod.get("status", {}).get("container_statuses", [])
+        if not container_statuses:
+            return False
+
+        for cstatus in container_statuses:
+            # If the terminated field is not set, the pod is still running. Too early
+            # to determine if any container failed.
+            terminated = cstatus.get("state", {}).get("terminated", {})
+            if not terminated:
+                return False
+
+            # If the terminated field is set but the `finished_at` field is not set,
+            # the pod is still considered as running.
+            if not terminated.get("finished_at"):
+                return False
+
+        # If we got until here, the containers were marked terminated and their
+        # finishedAt was set.
+        return True
 
     @property
     def is_running(self):
-        # Returns true if the pod is running.
-        return not self.is_done and (
-            self._pod.get("status", {}).get("phase") == "Running"
-        )
+        # Returns true if the container is running.
+        if self.is_done:
+            return False
+
+        return not self._are_pod_containers_done
 
     @property
     def is_waiting(self):
         return not self.is_done and not self.is_running
 
     @property
     def reason(self):
```

### Comparing `metaflow-2.9.6/metaflow/plugins/metadata/local.py` & `metaflow-2.9.7/metaflow/plugins/metadata/local.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/metadata/service.py` & `metaflow-2.9.7/metaflow/plugins/metadata/service.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/package_cli.py` & `metaflow-2.9.7/metaflow/plugins/package_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/parallel_decorator.py` & `metaflow-2.9.7/metaflow/plugins/parallel_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/project_decorator.py` & `metaflow-2.9.7/metaflow/plugins/project_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/resources_decorator.py` & `metaflow-2.9.7/metaflow/plugins/resources_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/retry_decorator.py` & `metaflow-2.9.7/metaflow/plugins/retry_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/secrets/secrets_decorator.py` & `metaflow-2.9.7/metaflow/plugins/secrets/secrets_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/storage_executor.py` & `metaflow-2.9.7/metaflow/plugins/storage_executor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/tag_cli.py` & `metaflow-2.9.7/metaflow/plugins/tag_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/test_unbounded_foreach_decorator.py` & `metaflow-2.9.7/metaflow/plugins/test_unbounded_foreach_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/plugins/timeout_decorator.py` & `metaflow-2.9.7/metaflow/plugins/timeout_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/procpoll.py` & `metaflow-2.9.7/metaflow/procpoll.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/pylint_wrapper.py` & `metaflow-2.9.7/metaflow/pylint_wrapper.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/runtime.py` & `metaflow-2.9.7/metaflow/runtime.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/sidecar/sidecar.py` & `metaflow-2.9.7/metaflow/sidecar/sidecar.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/sidecar/sidecar_messages.py` & `metaflow-2.9.7/metaflow/sidecar/sidecar_messages.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/sidecar/sidecar_subprocess.py` & `metaflow-2.9.7/metaflow/sidecar/sidecar_subprocess.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/sidecar/sidecar_worker.py` & `metaflow-2.9.7/metaflow/sidecar/sidecar_worker.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tagging_util.py` & `metaflow-2.9.7/metaflow/tagging_util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/task.py` & `metaflow-2.9.7/metaflow/task.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/00-helloworld/helloworld.py` & `metaflow-2.9.7/metaflow/tutorials/00-helloworld/helloworld.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/01-playlist/README.md` & `metaflow-2.9.7/metaflow/tutorials/01-playlist/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/01-playlist/movies.csv` & `metaflow-2.9.7/metaflow/tutorials/01-playlist/movies.csv`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/01-playlist/playlist.ipynb` & `metaflow-2.9.7/metaflow/tutorials/01-playlist/playlist.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/01-playlist/playlist.py` & `metaflow-2.9.7/metaflow/tutorials/01-playlist/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/02-statistics/README.md` & `metaflow-2.9.7/metaflow/tutorials/02-statistics/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/02-statistics/movies.csv` & `metaflow-2.9.7/metaflow/tutorials/02-statistics/movies.csv`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/02-statistics/stats.ipynb` & `metaflow-2.9.7/metaflow/tutorials/02-statistics/stats.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/02-statistics/stats.py` & `metaflow-2.9.7/metaflow/tutorials/02-statistics/stats.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/03-playlist-redux/README.md` & `metaflow-2.9.7/metaflow/tutorials/03-playlist-redux/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/03-playlist-redux/playlist.py` & `metaflow-2.9.7/metaflow/tutorials/03-playlist-redux/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/04-playlist-plus/README.md` & `metaflow-2.9.7/metaflow/tutorials/04-playlist-plus/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/04-playlist-plus/playlist.py` & `metaflow-2.9.7/metaflow/tutorials/04-playlist-plus/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/05-hello-cloud/README.md` & `metaflow-2.9.7/metaflow/tutorials/05-hello-cloud/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb` & `metaflow-2.9.7/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/05-hello-cloud/hello-cloud.py` & `metaflow-2.9.7/metaflow/tutorials/05-hello-cloud/hello-cloud.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/06-statistics-redux/README.md` & `metaflow-2.9.7/metaflow/tutorials/06-statistics-redux/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/06-statistics-redux/stats.ipynb` & `metaflow-2.9.7/metaflow/tutorials/06-statistics-redux/stats.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/07-worldview/worldview.ipynb` & `metaflow-2.9.7/metaflow/tutorials/07-worldview/worldview.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/08-autopilot/README.md` & `metaflow-2.9.7/metaflow/tutorials/08-autopilot/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/tutorials/08-autopilot/autopilot.ipynb` & `metaflow-2.9.7/metaflow/tutorials/08-autopilot/autopilot.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/util.py` & `metaflow-2.9.7/metaflow/util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow/vendor.py` & `metaflow-2.9.7/metaflow/vendor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/metaflow.egg-info/PKG-INFO` & `metaflow-2.9.7/metaflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow
-Version: 2.9.6
+Version: 2.9.7
 Summary: Metaflow: More Data Science, Less Engineering
 Author: Metaflow Developers
 Author-email: help@metaflow.org
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow
 Project-URL: Issues, https://github.com/Netflix/metaflow/issues
 Project-URL: Documentation, https://docs.metaflow.org
```

### Comparing `metaflow-2.9.6/metaflow.egg-info/SOURCES.txt` & `metaflow-2.9.7/metaflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.6/setup.py` & `metaflow-2.9.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "2.9.6"
+version = "2.9.7"
 
 setup(
     include_package_data=True,
     name="metaflow",
     version=version,
     description="Metaflow: More Data Science, Less Engineering",
     long_description=open("README.md").read(),
```

