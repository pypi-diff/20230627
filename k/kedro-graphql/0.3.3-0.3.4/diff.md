# Comparing `tmp/kedro-graphql-0.3.3.tar.gz` & `tmp/kedro-graphql-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-graphql-0.3.3.tar", last modified: Tue Jun 27 13:44:22 2023, max compression
+gzip compressed data, was "kedro-graphql-0.3.4.tar", last modified: Tue Jun 27 18:53:59 2023, max compression
```

## Comparing `kedro-graphql-0.3.3.tar` & `kedro-graphql-0.3.4.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:22.545398 kedro-graphql-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-06-27 13:44:22.545398 kedro-graphql-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 13:44:22.545398 kedro-graphql-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:22.533398 kedro-graphql-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:22.537398 kedro-graphql-0.3.3/src/kedro_graphql/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:22.541398 kedro-graphql-0.3.3/src/kedro_graphql/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/backends/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/celeryapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/celeryconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:22.541398 kedro-graphql-0.3.3/src/kedro_graphql/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/example/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:22.541398 kedro-graphql-0.3.3/src/kedro_graphql/logs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/logs/json_log_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/logs/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/pipeline_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:22.541398 kedro-graphql-0.3.3/src/kedro_graphql/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:22.541398 kedro-graphql-0.3.3/src/kedro_graphql/pipelines/example00/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/pipelines/example00/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/pipelines/example00/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/pipelines/example00/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:22.541398 kedro-graphql-0.3.3/src/kedro_graphql/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/plugins/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/kedro_graphql/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:22.537398 kedro-graphql-0.3.3/src/kedro_graphql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-06-27 13:44:22.000000 kedro-graphql-0.3.3/src/kedro_graphql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-27 13:44:22.000000 kedro-graphql-0.3.3/src/kedro_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:44:22.000000 kedro-graphql-0.3.3/src/kedro_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-27 13:44:22.000000 kedro-graphql-0.3.3/src/kedro_graphql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-27 13:44:22.000000 kedro-graphql-0.3.3/src/kedro_graphql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 13:44:22.000000 kedro-graphql-0.3.3/src/kedro_graphql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:22.545398 kedro-graphql-0.3.3/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:22.545398 kedro-graphql-0.3.3/src/tests/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/tests/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:22.545398 kedro-graphql-0.3.3/src/tests/pipelines/example00/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/tests/pipelines/example00/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/tests/pipelines/example00/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/tests/test_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/tests/test_schema_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/tests/test_schema_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-27 13:44:06.000000 kedro-graphql-0.3.3/src/tests/test_schema_subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.368808 kedro-graphql-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-06-27 18:53:59.368808 kedro-graphql-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 18:53:59.368808 kedro-graphql-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.360808 kedro-graphql-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.364808 kedro-graphql-0.3.4/src/kedro_graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.364808 kedro-graphql-0.3.4/src/kedro_graphql/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/backends/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/celeryapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.364808 kedro-graphql-0.3.4/src/kedro_graphql/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/example/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.364808 kedro-graphql-0.3.4/src/kedro_graphql/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/logs/json_log_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/logs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/pipeline_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.368808 kedro-graphql-0.3.4/src/kedro_graphql/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.368808 kedro-graphql-0.3.4/src/kedro_graphql/pipelines/example00/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/pipelines/example00/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/pipelines/example00/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/pipelines/example00/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.368808 kedro-graphql-0.3.4/src/kedro_graphql/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/plugins/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.364808 kedro-graphql-0.3.4/src/kedro_graphql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-06-27 18:53:59.000000 kedro-graphql-0.3.4/src/kedro_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-27 18:53:59.000000 kedro-graphql-0.3.4/src/kedro_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:53:59.000000 kedro-graphql-0.3.4/src/kedro_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-27 18:53:59.000000 kedro-graphql-0.3.4/src/kedro_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-27 18:53:59.000000 kedro-graphql-0.3.4/src/kedro_graphql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 18:53:59.000000 kedro-graphql-0.3.4/src/kedro_graphql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.368808 kedro-graphql-0.3.4/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.368808 kedro-graphql-0.3.4/src/tests/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.368808 kedro-graphql-0.3.4/src/tests/pipelines/example00/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/pipelines/example00/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/pipelines/example00/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/test_schema_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/test_schema_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/test_schema_subscription.py
```

### Comparing `kedro-graphql-0.3.3/LICENSE.txt` & `kedro-graphql-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/PKG-INFO` & `kedro-graphql-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-graphql
-Version: 0.3.3
+Version: 0.3.4
 Summary: A kedro plugin for serving any kedro project as a GraphQL api
 Author: opensean
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://github.com/opensean/kedro-graphql
 Project-URL: Source, https://github.com/opensean/kedro-graphql
 Keywords: pipelines,machine learning,data pipelines,data science,data engineering
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `kedro-graphql-0.3.3/README.md` & `kedro-graphql-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/pyproject.toml` & `kedro-graphql-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/kedro_graphql/__main__.py` & `kedro-graphql-0.3.4/src/kedro_graphql/__main__.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/kedro_graphql/asgi.py` & `kedro-graphql-0.3.4/src/kedro_graphql/asgi.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/kedro_graphql/backends/base.py` & `kedro-graphql-0.3.4/src/kedro_graphql/backends/base.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/kedro_graphql/backends/mongodb.py` & `kedro-graphql-0.3.4/src/kedro_graphql/backends/mongodb.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/kedro_graphql/commands.py` & `kedro-graphql-0.3.4/src/kedro_graphql/commands.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/kedro_graphql/config.py` & `kedro-graphql-0.3.4/src/kedro_graphql/config.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/kedro_graphql/decorators.py` & `kedro-graphql-0.3.4/src/kedro_graphql/decorators.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/kedro_graphql/events.py` & `kedro-graphql-0.3.4/src/kedro_graphql/events.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/kedro_graphql/example/app.py` & `kedro-graphql-0.3.4/src/kedro_graphql/example/app.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/kedro_graphql/logs/json_log_formatter.py` & `kedro-graphql-0.3.4/src/kedro_graphql/logs/json_log_formatter.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/kedro_graphql/logs/logger.py` & `kedro-graphql-0.3.4/src/kedro_graphql/logs/logger.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/kedro_graphql/models.py` & `kedro-graphql-0.3.4/src/kedro_graphql/models.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/kedro_graphql/plugins/plugins.py` & `kedro-graphql-0.3.4/src/kedro_graphql/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/kedro_graphql/schema.py` & `kedro-graphql-0.3.4/src/kedro_graphql/schema.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/kedro_graphql/settings.py` & `kedro-graphql-0.3.4/src/kedro_graphql/settings.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/kedro_graphql/tasks.py` & `kedro-graphql-0.3.4/src/kedro_graphql/tasks.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/kedro_graphql.egg-info/PKG-INFO` & `kedro-graphql-0.3.4/src/kedro_graphql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-graphql
-Version: 0.3.3
+Version: 0.3.4
 Summary: A kedro plugin for serving any kedro project as a GraphQL api
 Author: opensean
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://github.com/opensean/kedro-graphql
 Project-URL: Source, https://github.com/opensean/kedro-graphql
 Keywords: pipelines,machine learning,data pipelines,data science,data engineering
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `kedro-graphql-0.3.3/src/kedro_graphql.egg-info/SOURCES.txt` & `kedro-graphql-0.3.4/src/kedro_graphql.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 setup.cfg
 src/requirements.txt
 src/setup.py
 src/kedro_graphql/__init__.py
 src/kedro_graphql/__main__.py
 src/kedro_graphql/asgi.py
 src/kedro_graphql/celeryapp.py
-src/kedro_graphql/celeryconfig.py
 src/kedro_graphql/commands.py
 src/kedro_graphql/config.py
 src/kedro_graphql/decorators.py
 src/kedro_graphql/events.py
 src/kedro_graphql/models.py
 src/kedro_graphql/pipeline_registry.py
 src/kedro_graphql/schema.py
```

### Comparing `kedro-graphql-0.3.3/src/setup.py` & `kedro-graphql-0.3.4/src/setup.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/tests/conftest.py` & `kedro-graphql-0.3.4/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/tests/test_events.py` & `kedro-graphql-0.3.4/src/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/tests/test_logs.py` & `kedro-graphql-0.3.4/src/tests/test_logs.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/tests/test_models.py` & `kedro-graphql-0.3.4/src/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/tests/test_run.py` & `kedro-graphql-0.3.4/src/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/tests/test_schema_mutation.py` & `kedro-graphql-0.3.4/src/tests/test_schema_mutation.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/tests/test_schema_query.py` & `kedro-graphql-0.3.4/src/tests/test_schema_query.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.3/src/tests/test_schema_subscription.py` & `kedro-graphql-0.3.4/src/tests/test_schema_subscription.py`

 * *Files identical despite different names*

