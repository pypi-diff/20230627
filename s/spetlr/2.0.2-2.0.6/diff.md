# Comparing `tmp/spetlr-2.0.2.tar.gz` & `tmp/spetlr-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spetlr-2.0.2.tar", last modified: Tue Jun 13 07:37:29 2023, max compression
+gzip compressed data, was "spetlr-2.0.6.tar", last modified: Tue Jun 27 13:57:52 2023, max compression
```

## Comparing `spetlr-2.0.2.tar` & `spetlr-2.0.6.tar`

### file list

```diff
@@ -1,258 +1,262 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.394148 spetlr-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-13 07:37:15.000000 spetlr-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-13 07:37:15.000000 spetlr-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-13 07:37:29.394148 spetlr-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-13 07:37:15.000000 spetlr-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-13 07:37:15.000000 spetlr-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-13 07:37:29.394148 spetlr-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:37:15.000000 spetlr-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.374148 spetlr-2.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/alias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr/cache/
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/cache/CachedLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/cache/CachedLoaderParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr/config_master/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/config_master/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr/configurator/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr/configurator/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/_cli/ConfiguratorCli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/_cli/generate_keys_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr/configurator/sql/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/StatementBlocks.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/init_sqlparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/parse_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/substructures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr/cosmos/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/cosmos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/cosmos/cosmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/cosmos/cosmos_base_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/cosmos/cosmos_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/db_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr/delta/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/delta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/delta/db_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/delta/delta_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr/eh/
--rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/eh/EventHubCapture.py
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/eh/EventHubCaptureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/eh/EventHubJsonPublisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/eh/EventHubStream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/eh/PartitionSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/eh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/eh/eh_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/entry_points/generalized_task_entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/entry_points/task_entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/etl/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/etl/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/extractors/incremental_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/extractors/schema_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/extractors/simple_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/etl/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/loaders/DeleteDataLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/loaders/UpsertLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/loaders/simple_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/loaders/simple_sql_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/exceptions/cli_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/exceptions/configurator_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/extractors/eventhub_stream_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/formatting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/formatting/git_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/mount/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/mount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/mount/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/orchestrators/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/orchestrators/eh2bronze/
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/eh2bronze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/orchestrators/eh2silver/
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/eh2silver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/orchestrators/ehjson2delta/
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/ehjson2delta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/reporting/JobReflection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/reporting/SlackNotifier.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/reporting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/schema_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/schema_manager/schema_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/schema_manager/spark_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.386148 spetlr-2.0.2/src/spetlr/singleton/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/singleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/singleton/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/spark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.386148 spetlr-2.0.2/src/spetlr/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/sql/BaseExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/sql/CommonBaseServer.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/sql/SqlBaseServer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/sql/SqlExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/sql/SqlServer.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/sql/SqlServerBaseOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/sql/sql_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.386148 spetlr-2.0.2/src/spetlr/tables/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/tables/TableHandle.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/tables/ThMaker.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.386148 spetlr-2.0.2/src/spetlr/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/country_to_alphacode_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/dropColumnsTransformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/drop_oldest_duplicate_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/fuzzy_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/generate_md5_column_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/join_dataframes_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/selectColumnsTransformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/simple_dataframe_filter_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/simple_dataframe_filter_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/simple_sql_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/timezone_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/union_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/validfromto_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.386148 spetlr-2.0.2/src/spetlr/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/utils/CheckDfMerge.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/utils/CleanupTestDatabases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/utils/DataframeCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/utils/DropOldestDuplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/utils/GetMergeStatement.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/utils/MockExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/utils/MockLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/utils/SelectAndCastColumns.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-13 07:37:29.000000 spetlr-2.0.2/src/spetlr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-06-13 07:37:29.000000 spetlr-2.0.2/src/spetlr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:37:29.000000 spetlr-2.0.2/src/spetlr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-13 07:37:29.000000 spetlr-2.0.2/src/spetlr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:37:29.000000 spetlr-2.0.2/src/spetlr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-13 07:37:29.000000 spetlr-2.0.2/src/spetlr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 07:37:29.000000 spetlr-2.0.2/src/spetlr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.374148 spetlr-2.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.374148 spetlr-2.0.2/tests/cluster/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.386148 spetlr-2.0.2/tests/cluster/cache/
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/cache/test_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.386148 spetlr-2.0.2/tests/cluster/cosmos/
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/cosmos/test_cosmos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.386148 spetlr-2.0.2/tests/cluster/db/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/db/test_db_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.386148 spetlr-2.0.2/tests/cluster/delta/
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/delta/test_cleanup_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/delta/test_delta_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/delta/test_sparkexecutor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/cluster/eh/
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/eh/test_eh_json_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/eh/test_eh_json_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/eh/test_eh_saving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/cluster/etl/
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/etl/test_delete_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/etl/test_deltaupsert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/etl/test_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/etl/test_incremental_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/etl/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/etl/test_orchestrator_etl_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/etl/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/etl/test_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/etl/test_upsertloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/cluster/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/reporting/test_slack_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/cluster/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/schema_manager/test_schema_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/cluster/sql/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/sql/test_deliveryexecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/sql/test_deliverysql.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/sql/test_deliverysqlspn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/sql/test_simple_sql_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/sql/test_sqlhandle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/cluster/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/transformations/test_merge_df_into_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/transformations/test_union_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/local/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/local/configurator/
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/configurator/test_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/configurator/test_configurator_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/local/eh/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/eh/test_EventHubCaptureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/eh/test_ehto_bronze_and_silver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/eh/test_ehtodeltabronze_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/eh/test_ehtodeltabronze_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/eh/test_ehtodeltasilver_orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/local/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/entry_points/test_task_entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/local/etl/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/etl/test_orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/local/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/extractors/test_eventhub_stream_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/local/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/reporting/test_slack_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/local/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/schema_manager/test_schema_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/local/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/sql/test_SqlExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/test_get_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/test_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/test_sqlServer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/test_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.394148 spetlr-2.0.2/tests/local/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_concat_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_country_to_alphacode_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_dropoldestduplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_fuzzy_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_generate_md5_column_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_join_dataframes_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_select_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_simple_dataframe_filter_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_simple_dataframe_filter_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_timezone_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_union_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_validfromto_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.394148 spetlr-2.0.2/tests/local/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/utils/test_cleandatabases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/utils/test_dataframe_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/utils/test_dropoldestduplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/utils/test_getmergestatement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/utils/test_mock_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/utils/test_selectandcastcolumns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.510244 spetlr-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-27 13:57:40.000000 spetlr-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-27 13:57:40.000000 spetlr-2.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-27 13:57:52.510244 spetlr-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-27 13:57:40.000000 spetlr-2.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-27 13:57:40.000000 spetlr-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-27 13:57:52.510244 spetlr-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:57:40.000000 spetlr-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.478244 spetlr-2.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.490244 spetlr-2.0.6/src/spetlr/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/alias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.490244 spetlr-2.0.6/src/spetlr/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/cache/CachedLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/cache/CachedLoaderParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.490244 spetlr-2.0.6/src/spetlr/config_master/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/config_master/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.490244 spetlr-2.0.6/src/spetlr/configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/configurator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.494244 spetlr-2.0.6/src/spetlr/configurator/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/configurator/_cli/ConfiguratorCli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/configurator/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/configurator/_cli/generate_keys_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/configurator/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.494244 spetlr-2.0.6/src/spetlr/configurator/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/configurator/sql/StatementBlocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/configurator/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/configurator/sql/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/configurator/sql/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/configurator/sql/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/configurator/sql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/configurator/sql/init_sqlparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/configurator/sql/parse_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/configurator/sql/substructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/configurator/sql/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/configurator/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/configurator/sql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.494244 spetlr-2.0.6/src/spetlr/cosmos/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/cosmos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/cosmos/cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/cosmos/cosmos_base_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/cosmos/cosmos_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/db_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.494244 spetlr-2.0.6/src/spetlr/delta/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/delta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/delta/db_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/delta/delta_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.494244 spetlr-2.0.6/src/spetlr/eh/
+-rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/eh/EventHubCapture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/eh/EventHubCaptureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/eh/EventHubJsonPublisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/eh/EventHubStream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/eh/PartitionSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/eh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/eh/eh_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.494244 spetlr-2.0.6/src/spetlr/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/entry_points/generalized_task_entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/entry_points/task_entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.494244 spetlr-2.0.6/src/spetlr/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/etl/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.494244 spetlr-2.0.6/src/spetlr/etl/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/etl/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/etl/extractors/incremental_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/etl/extractors/schema_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/etl/extractors/simple_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/etl/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.498244 spetlr-2.0.6/src/spetlr/etl/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/etl/loaders/DeleteDataLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/etl/loaders/UpsertLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/etl/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/etl/loaders/simple_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/etl/loaders/simple_sql_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/etl/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/etl/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/etl/transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/etl/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.498244 spetlr-2.0.6/src/spetlr/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/exceptions/cli_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/exceptions/configurator_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.498244 spetlr-2.0.6/src/spetlr/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/extractors/eventhub_stream_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.498244 spetlr-2.0.6/src/spetlr/formatting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/formatting/git_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.498244 spetlr-2.0.6/src/spetlr/mount/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/mount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/mount/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.498244 spetlr-2.0.6/src/spetlr/orchestrators/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/orchestrators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.498244 spetlr-2.0.6/src/spetlr/orchestrators/eh2bronze/
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/orchestrators/eh2bronze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.498244 spetlr-2.0.6/src/spetlr/orchestrators/eh2silver/
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/orchestrators/eh2silver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.498244 spetlr-2.0.6/src/spetlr/orchestrators/ehjson2delta/
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/orchestrators/ehjson2delta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.498244 spetlr-2.0.6/src/spetlr/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/reporting/JobReflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/reporting/SlackNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/reporting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.498244 spetlr-2.0.6/src/spetlr/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/schema_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/schema_manager/schema_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/schema_manager/spark_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.498244 spetlr-2.0.6/src/spetlr/singleton/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/singleton/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/spark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.498244 spetlr-2.0.6/src/spetlr/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/sql/BaseExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/sql/CommonBaseServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/sql/SqlBaseServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/sql/SqlExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/sql/SqlServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/sql/SqlServerBaseOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/sql/sql_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.498244 spetlr-2.0.6/src/spetlr/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/tables/TableHandle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/tables/ThMaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.502244 spetlr-2.0.6/src/spetlr/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/transformers/country_to_alphacode_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/transformers/dropColumnsTransformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/transformers/drop_oldest_duplicate_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/transformers/fuzzy_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/transformers/generate_md5_column_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/transformers/join_dataframes_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/transformers/selectColumnsTransformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/transformers/simple_dataframe_filter_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/transformers/simple_dataframe_filter_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/transformers/simple_sql_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/transformers/timezone_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/transformers/union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/transformers/union_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/transformers/validfromto_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.502244 spetlr-2.0.6/src/spetlr/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/utils/CheckDfMerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/utils/CleanupTestDatabases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/utils/DataframeCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/utils/DeleteMismatchedSchemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/utils/DropOldestDuplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/utils/GetMergeStatement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/utils/MockExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/utils/MockLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/utils/SelectAndCastColumns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 13:57:40.000000 spetlr-2.0.6/src/spetlr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.490244 spetlr-2.0.6/src/spetlr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-27 13:57:52.000000 spetlr-2.0.6/src/spetlr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-06-27 13:57:52.000000 spetlr-2.0.6/src/spetlr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:57:52.000000 spetlr-2.0.6/src/spetlr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-27 13:57:52.000000 spetlr-2.0.6/src/spetlr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:57:52.000000 spetlr-2.0.6/src/spetlr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-27 13:57:52.000000 spetlr-2.0.6/src/spetlr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 13:57:52.000000 spetlr-2.0.6/src/spetlr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.486244 spetlr-2.0.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.486244 spetlr-2.0.6/tests/cluster/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.502244 spetlr-2.0.6/tests/cluster/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/cache/test_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.502244 spetlr-2.0.6/tests/cluster/cosmos/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/cosmos/test_cosmos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.502244 spetlr-2.0.6/tests/cluster/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/db/test_db_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.502244 spetlr-2.0.6/tests/cluster/delta/
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/delta/test_cleanup_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/delta/test_delta_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/delta/test_sparkexecutor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.502244 spetlr-2.0.6/tests/cluster/eh/
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/eh/test_eh_json_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/eh/test_eh_json_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/eh/test_eh_saving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.502244 spetlr-2.0.6/tests/cluster/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/etl/test_delete_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/etl/test_deltaupsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/etl/test_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/etl/test_incremental_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/etl/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/etl/test_orchestrator_etl_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/etl/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/etl/test_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/etl/test_upsertloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.502244 spetlr-2.0.6/tests/cluster/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/reporting/test_slack_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.506244 spetlr-2.0.6/tests/cluster/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/schema_manager/test_schema_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.506244 spetlr-2.0.6/tests/cluster/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/sql/test_deliveryexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/sql/test_deliverysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/sql/test_deliverysqlspn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/sql/test_simple_sql_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/sql/test_sqlhandle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.506244 spetlr-2.0.6/tests/cluster/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/transformations/test_merge_df_into_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/transformations/test_union_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.506244 spetlr-2.0.6/tests/cluster/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/cluster/utils/test_delete_schema_mismatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.506244 spetlr-2.0.6/tests/local/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.506244 spetlr-2.0.6/tests/local/configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/configurator/test_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/configurator/test_configurator_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.506244 spetlr-2.0.6/tests/local/eh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/eh/test_EventHubCaptureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/eh/test_ehto_bronze_and_silver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/eh/test_ehtodeltabronze_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/eh/test_ehtodeltabronze_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/eh/test_ehtodeltasilver_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.506244 spetlr-2.0.6/tests/local/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/entry_points/test_generalized_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/entry_points/test_task_entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.506244 spetlr-2.0.6/tests/local/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/etl/test_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.506244 spetlr-2.0.6/tests/local/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/extractors/test_eventhub_stream_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.506244 spetlr-2.0.6/tests/local/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/reporting/test_slack_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.506244 spetlr-2.0.6/tests/local/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/schema_manager/test_schema_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.506244 spetlr-2.0.6/tests/local/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/sql/test_SqlExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/test_get_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/test_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/test_sqlServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/test_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.506244 spetlr-2.0.6/tests/local/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/transformers/test_concat_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/transformers/test_country_to_alphacode_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/transformers/test_drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/transformers/test_dropoldestduplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/transformers/test_fuzzy_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/transformers/test_generate_md5_column_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/transformers/test_join_dataframes_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/transformers/test_select_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/transformers/test_simple_dataframe_filter_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/transformers/test_simple_dataframe_filter_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/transformers/test_timezone_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/transformers/test_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/transformers/test_union_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/transformers/test_validfromto_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:52.510244 spetlr-2.0.6/tests/local/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/utils/test_cleandatabases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/utils/test_dataframe_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/utils/test_dropoldestduplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/utils/test_getmergestatement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/utils/test_mock_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-27 13:57:40.000000 spetlr-2.0.6/tests/local/utils/test_selectandcastcolumns.py
```

### Comparing `spetlr-2.0.2/LICENSE` & `spetlr-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/PKG-INFO` & `spetlr-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spetlr
-Version: 2.0.2
+Version: 2.0.6
 Summary: A python ETL libRary (SPETLR) for Databricks powered by Apache SPark.
 Home-page: https://github.com/spetlr-org/spetlr
 Author: Spetlr.Org
 Author-email: spetlr.org@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/spetlr-org/spetlr
 Project-URL: Bug Reports, https://github.com/spetlr-org/spetlr/issues
```

### Comparing `spetlr-2.0.2/README.md` & `spetlr-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/setup.cfg` & `spetlr-2.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/cache/CachedLoader.py` & `spetlr-2.0.6/src/spetlr/cache/CachedLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/cache/CachedLoaderParameters.py` & `spetlr-2.0.6/src/spetlr/cache/CachedLoaderParameters.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/configurator/_cli/ConfiguratorCli.py` & `spetlr-2.0.6/src/spetlr/configurator/_cli/ConfiguratorCli.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/configurator/_cli/generate_keys_file.py` & `spetlr-2.0.6/src/spetlr/configurator/_cli/generate_keys_file.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/configurator/configurator.py` & `spetlr-2.0.6/src/spetlr/configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/configurator/sql/StatementBlocks.py` & `spetlr-2.0.6/src/spetlr/configurator/sql/StatementBlocks.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/configurator/sql/comments.py` & `spetlr-2.0.6/src/spetlr/configurator/sql/comments.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/configurator/sql/create.py` & `spetlr-2.0.6/src/spetlr/configurator/sql/create.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/configurator/sql/db.py` & `spetlr-2.0.6/src/spetlr/configurator/sql/db.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/configurator/sql/init_sqlparse.py` & `spetlr-2.0.6/src/spetlr/configurator/sql/init_sqlparse.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/configurator/sql/parse_sql.py` & `spetlr-2.0.6/src/spetlr/configurator/sql/parse_sql.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/configurator/sql/substructures.py` & `spetlr-2.0.6/src/spetlr/configurator/sql/substructures.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/configurator/sql/table.py` & `spetlr-2.0.6/src/spetlr/configurator/sql/table.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/cosmos/cosmos.py` & `spetlr-2.0.6/src/spetlr/cosmos/cosmos.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/cosmos/cosmos_base_server.py` & `spetlr-2.0.6/src/spetlr/cosmos/cosmos_base_server.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/cosmos/cosmos_handle.py` & `spetlr-2.0.6/src/spetlr/cosmos/cosmos_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/db_auto.py` & `spetlr-2.0.6/src/spetlr/db_auto.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/delta/db_handle.py` & `spetlr-2.0.6/src/spetlr/delta/db_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/delta/delta_handle.py` & `spetlr-2.0.6/src/spetlr/delta/delta_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/eh/EventHubCapture.py` & `spetlr-2.0.6/src/spetlr/eh/EventHubCapture.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/eh/EventHubCaptureExtractor.py` & `spetlr-2.0.6/src/spetlr/eh/EventHubCaptureExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/eh/EventHubJsonPublisher.py` & `spetlr-2.0.6/src/spetlr/eh/EventHubJsonPublisher.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/eh/EventHubStream.py` & `spetlr-2.0.6/src/spetlr/eh/EventHubStream.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/eh/PartitionSpec.py` & `spetlr-2.0.6/src/spetlr/eh/PartitionSpec.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/entry_points/generalized_task_entry_point.py` & `spetlr-2.0.6/src/spetlr/entry_points/generalized_task_entry_point.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import importlib
+import inspect
 import sys
+from typing import Any, Callable, Dict
 
 ENTRY_POINT = "entry_point"
 
 
 def main():
     """This function is entry point from which another entry point can be called.
     If you want to call this function:
@@ -53,9 +55,38 @@
     modname, qualname_separator, qualname = entry_point.partition(":")
 
     obj = importlib.import_module(modname)
     if qualname_separator:
         for attr in qualname.split("."):
             obj = getattr(obj, attr)
 
+    kwargs = prepare_keyword_arguments(obj, kwargs)
+
     # call the callable with custom parameters
     return obj(**kwargs)
+
+
+def prepare_keyword_arguments(callable_obj: Callable, kwargs_dict: Dict[str, Any]):
+    """Reduce the dict down to a set of keys that the callable can actually be called
+    with. Any extra keys are dropped with a warning."""
+    signature = inspect.signature(callable_obj)
+    parameters = signature.parameters
+
+    if any(
+        parameter.kind == inspect.Parameter.VAR_KEYWORD
+        for parameter in parameters.values()
+    ):
+        # if any of the callable's parameters use the form **kwargs,
+        # then we don't need to check further, just pass everything,
+        return kwargs_dict
+
+    valid_kwargs = {}
+    for key, value in kwargs_dict.items():
+        if key in parameters:  # only proceed if the parameter exists on the callable
+            valid_kwargs[key] = value
+        else:
+            print(
+                f"WARNING: Ignoring job parameter: {key}. "
+                "The entry point cannot receive it."
+            )
+
+    return valid_kwargs
```

### Comparing `spetlr-2.0.2/src/spetlr/entry_points/task_entry_point.py` & `spetlr-2.0.6/src/spetlr/entry_points/task_entry_point.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/etl/extractor.py` & `spetlr-2.0.6/src/spetlr/etl/extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/etl/extractors/incremental_extractor.py` & `spetlr-2.0.6/src/spetlr/etl/extractors/incremental_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/etl/extractors/schema_extractor.py` & `spetlr-2.0.6/src/spetlr/etl/extractors/schema_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/etl/loader.py` & `spetlr-2.0.6/src/spetlr/etl/loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/etl/loaders/DeleteDataLoader.py` & `spetlr-2.0.6/src/spetlr/etl/loaders/DeleteDataLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/etl/loaders/UpsertLoader.py` & `spetlr-2.0.6/src/spetlr/etl/loaders/UpsertLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/etl/loaders/simple_loader.py` & `spetlr-2.0.6/src/spetlr/etl/loaders/simple_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/etl/orchestrator.py` & `spetlr-2.0.6/src/spetlr/etl/orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/etl/transformer.py` & `spetlr-2.0.6/src/spetlr/etl/transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/etl/transformer_nc.py` & `spetlr-2.0.6/src/spetlr/etl/transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/exceptions/__init__.py` & `spetlr-2.0.6/src/spetlr/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/extractors/eventhub_stream_extractor.py` & `spetlr-2.0.6/src/spetlr/extractors/eventhub_stream_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/formatting/git_hooks.py` & `spetlr-2.0.6/src/spetlr/formatting/git_hooks.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/functions.py` & `spetlr-2.0.6/src/spetlr/functions.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/mount/main.py` & `spetlr-2.0.6/src/spetlr/mount/main.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py` & `spetlr-2.0.6/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py` & `spetlr-2.0.6/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py` & `spetlr-2.0.6/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py` & `spetlr-2.0.6/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py` & `spetlr-2.0.6/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py` & `spetlr-2.0.6/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/reporting/JobReflection.py` & `spetlr-2.0.6/src/spetlr/reporting/JobReflection.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/reporting/SlackNotifier.py` & `spetlr-2.0.6/src/spetlr/reporting/SlackNotifier.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/schema_manager/schema_manager.py` & `spetlr-2.0.6/src/spetlr/schema_manager/schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/schema_manager/spark_schema.py` & `spetlr-2.0.6/src/spetlr/schema_manager/spark_schema.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/spark.py` & `spetlr-2.0.6/src/spetlr/spark.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/sql/CommonBaseServer.py` & `spetlr-2.0.6/src/spetlr/sql/CommonBaseServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/sql/SqlBaseServer.py` & `spetlr-2.0.6/src/spetlr/sql/SqlBaseServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/sql/SqlExecutor.py` & `spetlr-2.0.6/src/spetlr/sql/SqlExecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/sql/SqlServer.py` & `spetlr-2.0.6/src/spetlr/sql/SqlServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/sql/sql_handle.py` & `spetlr-2.0.6/src/spetlr/sql/sql_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/tables/TableHandle.py` & `spetlr-2.0.6/src/spetlr/tables/TableHandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/transformations.py` & `spetlr-2.0.6/src/spetlr/transformations.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/transformers/__init__.py` & `spetlr-2.0.6/src/spetlr/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/transformers/country_to_alphacode_transformer_nc.py` & `spetlr-2.0.6/src/spetlr/transformers/country_to_alphacode_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/transformers/dropColumnsTransformer_nc.py` & `spetlr-2.0.6/src/spetlr/transformers/dropColumnsTransformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/transformers/drop_oldest_duplicate_transformer.py` & `spetlr-2.0.6/src/spetlr/transformers/drop_oldest_duplicate_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/transformers/fuzzy_select.py` & `spetlr-2.0.6/src/spetlr/transformers/fuzzy_select.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/transformers/generate_md5_column_transformer_nc.py` & `spetlr-2.0.6/src/spetlr/transformers/generate_md5_column_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/transformers/join_dataframes_transformer.py` & `spetlr-2.0.6/src/spetlr/transformers/join_dataframes_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/transformers/selectColumnsTransformer_nc.py` & `spetlr-2.0.6/src/spetlr/transformers/selectColumnsTransformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py` & `spetlr-2.0.6/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/transformers/simple_dataframe_filter_transformer.py` & `spetlr-2.0.6/src/spetlr/transformers/simple_dataframe_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/transformers/simple_dataframe_filter_transformer_nc.py` & `spetlr-2.0.6/src/spetlr/transformers/simple_dataframe_filter_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/transformers/timezone_transformer_nc.py` & `spetlr-2.0.6/src/spetlr/transformers/timezone_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/transformers/union_transformer.py` & `spetlr-2.0.6/src/spetlr/transformers/union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/transformers/union_transformer_nc.py` & `spetlr-2.0.6/src/spetlr/transformers/union_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/transformers/validfromto_transformer.py` & `spetlr-2.0.6/src/spetlr/transformers/validfromto_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/utils/CheckDfMerge.py` & `spetlr-2.0.6/src/spetlr/utils/CheckDfMerge.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/utils/CleanupTestDatabases.py` & `spetlr-2.0.6/src/spetlr/utils/CleanupTestDatabases.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/utils/DataframeCreator.py` & `spetlr-2.0.6/src/spetlr/utils/DataframeCreator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/utils/DropOldestDuplicates.py` & `spetlr-2.0.6/src/spetlr/utils/DropOldestDuplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/utils/GetMergeStatement.py` & `spetlr-2.0.6/src/spetlr/utils/GetMergeStatement.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/utils/MockLoader.py` & `spetlr-2.0.6/src/spetlr/utils/MockLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr/utils/SelectAndCastColumns.py` & `spetlr-2.0.6/src/spetlr/utils/SelectAndCastColumns.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/src/spetlr.egg-info/PKG-INFO` & `spetlr-2.0.6/src/spetlr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spetlr
-Version: 2.0.2
+Version: 2.0.6
 Summary: A python ETL libRary (SPETLR) for Databricks powered by Apache SPark.
 Home-page: https://github.com/spetlr-org/spetlr
 Author: Spetlr.Org
 Author-email: spetlr.org@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/spetlr-org/spetlr
 Project-URL: Bug Reports, https://github.com/spetlr-org/spetlr/issues
```

### Comparing `spetlr-2.0.2/src/spetlr.egg-info/SOURCES.txt` & `spetlr-2.0.6/src/spetlr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 src/spetlr/transformers/timezone_transformer_nc.py
 src/spetlr/transformers/union_transformer.py
 src/spetlr/transformers/union_transformer_nc.py
 src/spetlr/transformers/validfromto_transformer.py
 src/spetlr/utils/CheckDfMerge.py
 src/spetlr/utils/CleanupTestDatabases.py
 src/spetlr/utils/DataframeCreator.py
+src/spetlr/utils/DeleteMismatchedSchemas.py
 src/spetlr/utils/DropOldestDuplicates.py
 src/spetlr/utils/GetMergeStatement.py
 src/spetlr/utils/MockExtractor.py
 src/spetlr/utils/MockLoader.py
 src/spetlr/utils/SelectAndCastColumns.py
 src/spetlr/utils/__init__.py
 tests/cluster/cache/test_cache.py
@@ -158,26 +159,28 @@
 tests/cluster/sql/test_deliveryexecutor.py
 tests/cluster/sql/test_deliverysql.py
 tests/cluster/sql/test_deliverysqlspn.py
 tests/cluster/sql/test_simple_sql_etl.py
 tests/cluster/sql/test_sqlhandle.py
 tests/cluster/transformations/test_merge_df_into_target.py
 tests/cluster/transformations/test_union_transformer.py
+tests/cluster/utils/test_delete_schema_mismatch.py
 tests/local/test_functions.py
 tests/local/test_get_schema.py
 tests/local/test_spark.py
 tests/local/test_sqlServer.py
 tests/local/test_transformations.py
 tests/local/configurator/test_configurator.py
 tests/local/configurator/test_configurator_cli.py
 tests/local/eh/test_EventHubCaptureExtractor.py
 tests/local/eh/test_ehto_bronze_and_silver.py
 tests/local/eh/test_ehtodeltabronze_orchestrator.py
 tests/local/eh/test_ehtodeltabronze_transformer.py
 tests/local/eh/test_ehtodeltasilver_orchestrator.py
+tests/local/entry_points/test_generalized_entry_points.py
 tests/local/entry_points/test_task_entry_point.py
 tests/local/etl/test_orchestrator.py
 tests/local/extractors/test_eventhub_stream_extractor.py
 tests/local/reporting/test_slack_reporting.py
 tests/local/schema_manager/test_schema_manager.py
 tests/local/sql/test_SqlExecutor.py
 tests/local/transformers/test_concat_df.py
```

### Comparing `spetlr-2.0.2/tests/cluster/cache/test_cache.py` & `spetlr-2.0.6/tests/cluster/cache/test_cache.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/cosmos/test_cosmos.py` & `spetlr-2.0.6/tests/cluster/cosmos/test_cosmos.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/delta/test_cleanup_databases.py` & `spetlr-2.0.6/tests/cluster/delta/test_cleanup_databases.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/delta/test_delta_class.py` & `spetlr-2.0.6/tests/cluster/delta/test_delta_class.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/delta/test_sparkexecutor.py` & `spetlr-2.0.6/tests/cluster/delta/test_sparkexecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/eh/test_eh_json_orchestrator.py` & `spetlr-2.0.6/tests/cluster/eh/test_eh_json_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/eh/test_eh_json_transformer.py` & `spetlr-2.0.6/tests/cluster/eh/test_eh_json_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/eh/test_eh_saving.py` & `spetlr-2.0.6/tests/cluster/eh/test_eh_saving.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/etl/test_delete_data_loader.py` & `spetlr-2.0.6/tests/cluster/etl/test_delete_data_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/etl/test_deltaupsert.py` & `spetlr-2.0.6/tests/cluster/etl/test_deltaupsert.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/etl/test_extractor.py` & `spetlr-2.0.6/tests/cluster/etl/test_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/etl/test_incremental_extractor.py` & `spetlr-2.0.6/tests/cluster/etl/test_incremental_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/etl/test_loader.py` & `spetlr-2.0.6/tests/cluster/etl/test_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/etl/test_orchestrator_etl_warning.py` & `spetlr-2.0.6/tests/cluster/etl/test_orchestrator_etl_warning.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/etl/test_transformer.py` & `spetlr-2.0.6/tests/cluster/etl/test_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/etl/test_transformer_nc.py` & `spetlr-2.0.6/tests/cluster/etl/test_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/etl/test_upsertloader.py` & `spetlr-2.0.6/tests/cluster/etl/test_upsertloader.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/reporting/test_slack_reporting.py` & `spetlr-2.0.6/tests/cluster/reporting/test_slack_reporting.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/schema_manager/test_schema_manager.py` & `spetlr-2.0.6/tests/cluster/schema_manager/test_schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/sql/test_deliveryexecutor.py` & `spetlr-2.0.6/tests/cluster/sql/test_deliveryexecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/sql/test_deliverysql.py` & `spetlr-2.0.6/tests/cluster/sql/test_deliverysql.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/sql/test_simple_sql_etl.py` & `spetlr-2.0.6/tests/cluster/sql/test_simple_sql_etl.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,27 +49,34 @@
         cls.tc.reset(debug=False)
 
     def test01_can_transform(self):
         self.create_test_table()
         df = self.create_data()
 
         # Test that timestamp before has miliseconds also
-        date_test = df.select("testcolumn4").collect()[0][0]
+        date_test_0 = df.select("testcolumn4").collect()[0][0]  # row 1
+        date_test_1 = df.select("testcolumn4").collect()[1][0]  # row 2
         self.assertEqual(
-            dt_utc(2021, 1, 1, 14, 45, 22, 32).replace(tzinfo=None), date_test
+            dt_utc(2021, 1, 1, 14, 45, 22, 32).replace(tzinfo=None), date_test_0
         )
+        self.assertEqual(dt_utc(1, 1, 2, 0, 0, 1, 1).replace(tzinfo=None), date_test_1)
 
         df_out = SimpleSqlServerTransformer(
             table_id=self.table_id, server=self.sql_server
         ).process(df)
 
         # Check that timestamp are truncated down to only seconds
-        # The 32 miliseconds should be gone.
-        date_test = df_out.select("testcolumn4").collect()[0][0]
-        self.assertEqual(dt_utc(2021, 1, 1, 14, 45, 22).replace(tzinfo=None), date_test)
+        # The 32 and 1 miliseconds from row 1 and 2, respectively should be gone.
+        # The 0001-01-01 date in row 2 should be converted to 1900-01-01
+        date_test_0 = df_out.select("testcolumn4").collect()[0][0]  # row 1
+        date_test_1 = df_out.select("testcolumn4").collect()[1][0]  # row 2
+        self.assertEqual(
+            dt_utc(2021, 1, 1, 14, 45, 22).replace(tzinfo=None), date_test_0
+        )
+        self.assertEqual(dt_utc(1900, 1, 1, 0, 0, 1).replace(tzinfo=None), date_test_1)
 
         schema_expected = StructType(
             [
                 StructField("testcolumn", IntegerType(), True),
                 StructField("testcolumn2", DecimalType(12, 3), True),
                 StructField("testcolumn3", StringType(), True),
                 StructField("testcolumn4", TimestampType(), True),
@@ -128,14 +135,17 @@
                 StructField("testcolumn2", DoubleType(), True),
                 StructField("testcolumn3", StringType(), True),
                 StructField("testcolumn4", TimestampType(), True),
             ]
         )
         cols = ["testcolumn", "testcolumn2", "testcolumn3", "testcolumn4"]
 
-        insert_data = (123, 1001.322, "Hello", dt_utc(2021, 1, 1, 14, 45, 22, 32))
+        insert_data = [
+            (123, 1001.322, "Hello", dt_utc(2021, 1, 1, 14, 45, 22, 32)),  # row 1
+            (456, 2002.123, "Hello_2", dt_utc(1, 1, 2, 0, 0, 1, 1)),  # row 2
+        ]
 
         df_new = DataframeCreator.make_partial(
-            schema=schema, columns=cols, data=[insert_data]
+            schema=schema, columns=cols, data=insert_data
         )
 
         return df_new.orderBy("testcolumn")
```

### Comparing `spetlr-2.0.2/tests/cluster/sql/test_sqlhandle.py` & `spetlr-2.0.6/tests/cluster/sql/test_sqlhandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/transformations/test_merge_df_into_target.py` & `spetlr-2.0.6/tests/cluster/transformations/test_merge_df_into_target.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/cluster/transformations/test_union_transformer.py` & `spetlr-2.0.6/tests/cluster/transformations/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/configurator/test_configurator.py` & `spetlr-2.0.6/tests/local/configurator/test_configurator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/configurator/test_configurator_cli.py` & `spetlr-2.0.6/tests/local/configurator/test_configurator_cli.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/eh/test_EventHubCaptureExtractor.py` & `spetlr-2.0.6/tests/local/eh/test_EventHubCaptureExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/eh/test_ehto_bronze_and_silver.py` & `spetlr-2.0.6/tests/local/eh/test_ehto_bronze_and_silver.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/eh/test_ehtodeltabronze_orchestrator.py` & `spetlr-2.0.6/tests/local/eh/test_ehtodeltabronze_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/eh/test_ehtodeltabronze_transformer.py` & `spetlr-2.0.6/tests/local/eh/test_ehtodeltabronze_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/eh/test_ehtodeltasilver_orchestrator.py` & `spetlr-2.0.6/tests/local/eh/test_ehtodeltasilver_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/extractors/test_eventhub_stream_extractor.py` & `spetlr-2.0.6/tests/local/extractors/test_eventhub_stream_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/reporting/test_slack_reporting.py` & `spetlr-2.0.6/tests/local/reporting/test_slack_reporting.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/schema_manager/test_schema_manager.py` & `spetlr-2.0.6/tests/local/schema_manager/test_schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/sql/test_SqlExecutor.py` & `spetlr-2.0.6/tests/local/sql/test_SqlExecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/test_functions.py` & `spetlr-2.0.6/tests/local/test_functions.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/test_get_schema.py` & `spetlr-2.0.6/tests/local/test_get_schema.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/test_sqlServer.py` & `spetlr-2.0.6/tests/local/test_sqlServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/test_transformations.py` & `spetlr-2.0.6/tests/local/test_transformations.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/transformers/test_concat_df.py` & `spetlr-2.0.6/tests/local/transformers/test_concat_df.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/transformers/test_country_to_alphacode_transformer.py` & `spetlr-2.0.6/tests/local/transformers/test_country_to_alphacode_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/transformers/test_drop_columns.py` & `spetlr-2.0.6/tests/local/transformers/test_drop_columns.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/transformers/test_dropoldestduplicates.py` & `spetlr-2.0.6/tests/local/transformers/test_dropoldestduplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/transformers/test_fuzzy_select.py` & `spetlr-2.0.6/tests/local/transformers/test_fuzzy_select.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/transformers/test_generate_md5_column_transformer_nc.py` & `spetlr-2.0.6/tests/local/transformers/test_generate_md5_column_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/transformers/test_join_dataframes_transformer.py` & `spetlr-2.0.6/tests/local/transformers/test_join_dataframes_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py` & `spetlr-2.0.6/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/transformers/test_select_columns.py` & `spetlr-2.0.6/tests/local/transformers/test_select_columns.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/transformers/test_simple_dataframe_filter_transformer.py` & `spetlr-2.0.6/tests/local/transformers/test_simple_dataframe_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/transformers/test_simple_dataframe_filter_transformer_nc.py` & `spetlr-2.0.6/tests/local/transformers/test_simple_dataframe_filter_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/transformers/test_timezone_transformer_nc.py` & `spetlr-2.0.6/tests/local/transformers/test_timezone_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/transformers/test_union_transformer.py` & `spetlr-2.0.6/tests/local/transformers/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/transformers/test_union_transformer_nc.py` & `spetlr-2.0.6/tests/local/transformers/test_union_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/transformers/test_validfromto_transformer.py` & `spetlr-2.0.6/tests/local/transformers/test_validfromto_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/utils/test_dataframe_creation.py` & `spetlr-2.0.6/tests/local/utils/test_dataframe_creation.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/utils/test_dropoldestduplicates.py` & `spetlr-2.0.6/tests/local/utils/test_dropoldestduplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/utils/test_getmergestatement.py` & `spetlr-2.0.6/tests/local/utils/test_getmergestatement.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/utils/test_mock_etl.py` & `spetlr-2.0.6/tests/local/utils/test_mock_etl.py`

 * *Files identical despite different names*

### Comparing `spetlr-2.0.2/tests/local/utils/test_selectandcastcolumns.py` & `spetlr-2.0.6/tests/local/utils/test_selectandcastcolumns.py`

 * *Files identical despite different names*

