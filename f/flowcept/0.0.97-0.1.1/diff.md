# Comparing `tmp/flowcept-0.0.97.tar.gz` & `tmp/flowcept-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowcept-0.0.97.tar", last modified: Tue Dec  6 20:51:14 2022, max compression
+gzip compressed data, was "flowcept-0.1.1.tar", last modified: Tue Jun 27 18:58:40 2023, max compression
```

## Comparing `flowcept-0.0.97.tar` & `flowcept-0.1.1.tar`

### file list

```diff
@@ -1,61 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:14.224241 flowcept-0.0.97/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2022-12-06 20:51:02.000000 flowcept-0.0.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2022-12-06 20:51:14.224241 flowcept-0.0.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2022-12-06 20:51:02.000000 flowcept-0.0.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:14.220241 flowcept-0.0.97/flowcept/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:14.220241 flowcept-0.0.97/flowcept/commons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/commons/vocabulary.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:14.220241 flowcept-0.0.97/flowcept/flowcept_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowcept_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowcept_consumer/consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:14.220241 flowcept-0.0.97/flowcept/flowcept_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowcept_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowcept_server/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:14.220241 flowcept-0.0.97/flowcept/flowcept_server/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowcept_server/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:14.220241 flowcept-0.0.97/flowcept/flowcept_server/handlers/zambeze/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowcept_server/handlers/zambeze/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowcept_server/handlers/zambeze/zambeze_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:14.220241 flowcept-0.0.97/flowcept/flowceptor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowceptor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:14.220241 flowcept-0.0.97/flowcept/flowceptor/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowceptor/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowceptor/plugins/base_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowceptor/plugins/base_settings_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowceptor/plugins/interceptor_state_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:14.224241 flowcept-0.0.97/flowcept/flowceptor/plugins/mlflow/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowceptor/plugins/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowceptor/plugins/mlflow/interception_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowceptor/plugins/mlflow/mlflow_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowceptor/plugins/mlflow/mlflow_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowceptor/plugins/mlflow/mlflow_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowceptor/plugins/mlflow/mlflow_interceptor_state_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowceptor/plugins/settings_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:14.224241 flowcept-0.0.97/flowcept/flowceptor/plugins/tensorboard/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowceptor/plugins/tensorboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowceptor/plugins/tensorboard/tensorboard_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowceptor/plugins/tensorboard/tensorboard_interceptor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:14.224241 flowcept-0.0.97/flowcept/flowceptor/plugins/zambeze/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowceptor/plugins/zambeze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowceptor/plugins/zambeze/zambeze_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2022-12-06 20:51:02.000000 flowcept-0.0.97/flowcept/flowceptor/plugins/zambeze/zambeze_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2022-12-06 20:51:03.000000 flowcept-0.0.97/flowcept/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:14.220241 flowcept-0.0.97/flowcept.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2022-12-06 20:51:14.000000 flowcept-0.0.97/flowcept.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2022-12-06 20:51:14.000000 flowcept-0.0.97/flowcept.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 20:51:14.000000 flowcept-0.0.97/flowcept.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2022-12-06 20:51:14.000000 flowcept-0.0.97/flowcept.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-06 20:51:14.000000 flowcept-0.0.97/flowcept.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-06 20:51:02.000000 flowcept-0.0.97/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-06 20:51:14.224241 flowcept-0.0.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2022-12-06 20:51:02.000000 flowcept-0.0.97/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:14.224241 flowcept-0.0.97/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:02.000000 flowcept-0.0.97/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:14.224241 flowcept-0.0.97/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 20:51:02.000000 flowcept-0.0.97/tests/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2022-12-06 20:51:02.000000 flowcept-0.0.97/tests/plugins/test_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2022-12-06 20:51:02.000000 flowcept-0.0.97/tests/plugins/test_tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2022-12-06 20:51:02.000000 flowcept-0.0.97/tests/plugins/test_zambeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.940839 flowcept-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-27 18:58:30.000000 flowcept-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-27 18:58:40.940839 flowcept-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-27 18:58:30.000000 flowcept-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.932839 flowcept-0.1.1/flowcept/
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.932839 flowcept-0.1.1/flowcept/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/commons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.932839 flowcept-0.1.1/flowcept/commons/daos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/commons/daos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/commons/daos/document_db_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/commons/daos/mq_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/commons/flowcept_data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/commons/flowcept_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/commons/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/commons/vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.932839 flowcept-0.1.1/flowcept/flowcept_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowcept_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowcept_api/consumer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowcept_api/task_query_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.932839 flowcept-0.1.1/flowcept/flowcept_webserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowcept_webserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowcept_webserver/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.932839 flowcept-0.1.1/flowcept/flowcept_webserver/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowcept_webserver/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowcept_webserver/resources/query_rsrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowcept_webserver/resources/task_messages_rsrc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.932839 flowcept-0.1.1/flowcept/flowceptor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.936839 flowcept-0.1.1/flowcept/flowceptor/consumers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/consumers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/consumers/consumer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/consumers/document_inserter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.936839 flowcept-0.1.1/flowcept/flowceptor/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/base_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/base_settings_dataclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.936839 flowcept-0.1.1/flowcept/flowceptor/plugins/dask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/dask/dask_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/dask/dask_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/dask/dask_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/interceptor_state_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.936839 flowcept-0.1.1/flowcept/flowceptor/plugins/mlflow/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/mlflow/interception_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/mlflow/mlflow_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/mlflow/mlflow_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/mlflow/mlflow_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/settings_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.936839 flowcept-0.1.1/flowcept/flowceptor/plugins/tensorboard/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/tensorboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/tensorboard/tensorboard_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/tensorboard/tensorboard_interceptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.936839 flowcept-0.1.1/flowcept/flowceptor/plugins/zambeze/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/zambeze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/zambeze/zambeze_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/flowceptor/plugins/zambeze/zambeze_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-27 18:58:30.000000 flowcept-0.1.1/flowcept/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-27 18:58:31.000000 flowcept-0.1.1/flowcept/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.932839 flowcept-0.1.1/flowcept.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-27 18:58:40.000000 flowcept-0.1.1/flowcept.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-27 18:58:40.000000 flowcept-0.1.1/flowcept.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:58:40.000000 flowcept-0.1.1/flowcept.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-27 18:58:40.000000 flowcept-0.1.1/flowcept.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 18:58:40.000000 flowcept-0.1.1/flowcept.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-27 18:58:30.000000 flowcept-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:58:40.940839 flowcept-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-27 18:58:30.000000 flowcept-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.936839 flowcept-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:30.000000 flowcept-0.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.936839 flowcept-0.1.1/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:30.000000 flowcept-0.1.1/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-27 18:58:30.000000 flowcept-0.1.1/tests/api/query_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.936839 flowcept-0.1.1/tests/doc_db_inserter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:30.000000 flowcept-0.1.1/tests/doc_db_inserter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-27 18:58:30.000000 flowcept-0.1.1/tests/doc_db_inserter/doc_db_inserter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.940839 flowcept-0.1.1/tests/log_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:30.000000 flowcept-0.1.1/tests/log_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-27 18:58:30.000000 flowcept-0.1.1/tests/log_tests/log_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 18:58:30.000000 flowcept-0.1.1/tests/log_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:40.940839 flowcept-0.1.1/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:58:30.000000 flowcept-0.1.1/tests/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-27 18:58:30.000000 flowcept-0.1.1/tests/plugins/test_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-27 18:58:30.000000 flowcept-0.1.1/tests/plugins/test_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-06-27 18:58:30.000000 flowcept-0.1.1/tests/plugins/test_tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-27 18:58:30.000000 flowcept-0.1.1/tests/plugins/test_zambeze.py
```

### Comparing `flowcept-0.0.97/LICENSE` & `flowcept-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flowcept-0.0.97/flowcept/flowceptor/plugins/interceptor_state_manager.py` & `flowcept-0.1.1/flowcept/flowceptor/plugins/interceptor_state_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 class InterceptorStateManager(object):
     def __init__(self, settings: BaseSettings):
         self._set_name = settings.key
 
         if not hasattr(settings, "redis_host"):
             raise Exception(
-                f"This plugin setting {settings.key} "
-                f"does not have a Redis Host."
+                f"This plugin setting {settings.key} manages state in Redis, so"
+                f"Redis Host is required in the settings yaml file."
             )
 
         self._db = Redis(
             host=settings.redis_host,
             port=settings.redis_port,
             db=0,
         )
```

### Comparing `flowcept-0.0.97/flowcept/flowceptor/plugins/mlflow/mlflow_dao.py` & `flowcept-0.1.1/flowcept/flowceptor/plugins/mlflow/mlflow_dao.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from typing import List
 from sqlalchemy.engine import Row, create_engine
 from textwrap import dedent
+
+from flowcept.commons.flowcept_logger import FlowceptLogger
 from flowcept.flowceptor.plugins.mlflow.mlflow_dataclasses import (
     RunData,
     MLFlowSettings,
 )
 
 
 class MLFlowDAO:
-
     _LIMIT = 10
     # TODO: This should not at all be hard coded.
     # This value needs to be greater than the amount of
     # runs inserted in the Runs table at each data observation
 
     def __init__(self, mlflow_settings: MLFlowSettings):
         self._engine = MLFlowDAO._get_db_engine(mlflow_settings.file_path)
+        self.logger = FlowceptLogger().get_logger()
 
     @staticmethod
     def _get_db_engine(sqlite_file):
         try:
             db_uri = f"sqlite:///{sqlite_file}"
             engine = create_engine(db_uri)
             return engine
@@ -34,61 +36,76 @@
                 runs
             WHERE
                 status = 'FINISHED'
             ORDER BY end_time DESC
             LIMIT {MLFlowDAO._LIMIT}
             """
         )
-        conn = self._engine.connect()
-        results = conn.execute(sql).fetchall()
-        return results
+        try:
+            conn = self._engine.connect()
+            results = conn.execute(sql).fetchall()
+            return results
+        except Exception as e:
+            self.logger.debug(str(e))
+            return None
+        finally:
+            conn.close()
 
     def get_run_data(self, run_uuid: str) -> RunData:
         # TODO: consider outer joins to get the run data even if there's
-        #  no metric or param
+        #  no metric or param or if the task hasn't finished yet
         sql = dedent(
             f"""
             SELECT r.run_uuid, r.start_time, r.end_time, r.status,
                m.key as 'metric_key', m.value as 'metric_value',
                p.key as 'parameter_key', p.value as 'parameter_value'
             FROM
                 runs AS r,
                 metrics as m,
                 params as p
             WHERE
                 r.run_uuid = m.run_uuid AND
                 m.run_uuid = p.run_uuid AND
                 r.run_uuid = '{run_uuid}' AND
-                r.status = 'FINISHED'
+                r.status = 'FINISHED' 
             ORDER BY
                 end_time DESC,
                 metric_key, metric_value,
                 parameter_key, parameter_value
             LIMIT 30
 """
         )
-        conn = self._engine.connect()
-        result_set = conn.execute(sql).fetchall()
-        run_data_dict = {"metrics": {}, "parameters": {}}
+        try:
+            conn = self._engine.connect()
+            result_set = conn.execute(sql).fetchall()
+        except Exception as e:
+            self.logger.warning(e)
+            return None
+        finally:
+            conn.close()
+        run_data_dict = {"used": {}, "generated": {}}
         for tuple_ in result_set:
             tuple_dict = tuple_._asdict()
             metric_key = tuple_dict.get("metric_key", None)
             metric_value = tuple_dict.get("metric_value", None)
             if metric_key and metric_value:
-                if not (metric_key in run_data_dict["metrics"]):
-                    run_data_dict["metrics"][metric_key] = None
-                run_data_dict["metrics"][metric_key] = metric_value
+                if not (metric_key in run_data_dict["generated"]):
+                    run_data_dict["generated"][metric_key] = None
+                run_data_dict["generated"][metric_key] = metric_value
 
             param_key = tuple_dict.get("parameter_key", None)
             param_value = tuple_dict.get("parameter_value", None)
             if param_key and param_value:
-                if not (param_key in run_data_dict["parameters"]):
-                    run_data_dict["parameters"][param_key] = None
-                run_data_dict["parameters"][param_key] = param_value
+                if not (param_key in run_data_dict["used"]):
+                    run_data_dict["used"][param_key] = None
+                run_data_dict["used"][param_key] = param_value
 
-            run_data_dict["run_uuid"] = tuple_dict["run_uuid"]
+            run_data_dict["task_id"] = tuple_dict["run_uuid"]
             run_data_dict["start_time"] = tuple_dict["start_time"]
             run_data_dict["end_time"] = tuple_dict["end_time"]
             run_data_dict["status"] = tuple_dict["status"]
-
-        run_data = RunData(**run_data_dict)
-        return run_data
+        try:
+            run_data = RunData(**run_data_dict)
+            return run_data
+        except Exception as e:
+            self.logger.warning(e)
+            return None
```

### Comparing `flowcept-0.0.97/flowcept/flowceptor/plugins/mlflow/mlflow_dataclasses.py` & `flowcept-0.1.1/flowcept/flowceptor/plugins/mlflow/mlflow_dataclasses.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 from typing import List
 
 from flowcept.flowceptor.plugins.base_settings_dataclasses import BaseSettings
 
 
 @dataclass
 class MLFlowSettings(BaseSettings):
-
     file_path: str
     log_params: List[str]
     log_metrics: List[str]
     watch_interval_sec: int
     redis_port: int
     redis_host: str
     kind = "mlflow"
-    observer_type = "file"
-    observer_subtype = "sqlite"
+
+    def __post_init__(self):
+        self.observer_type = "file"
+        self.observer_subtype = "sqlite"
 
 
 @dataclass
 class RunData:
-
-    run_uuid: str
+    task_id: str
     start_time: int
     end_time: int
-    metrics: dict
-    parameters: dict
+    used: dict
+    generated: dict
     status: str
```

### Comparing `flowcept-0.0.97/flowcept/flowceptor/plugins/mlflow/mlflow_interceptor.py` & `flowcept-0.1.1/flowcept/flowcept_api/consumer_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,73 @@
-import sys
-import os
-import time
-from watchdog.observers import Observer
-from flowcept.flowceptor.plugins.base_interceptor import (
-    BaseInterceptor,
+from typing import List, Union
+from time import sleep
+import random
+
+from flowcept.commons.daos.mq_dao import MQDao
+from flowcept.configs import (
+    REDIS_INSERTION_BUFFER_TIME,
+    MONGO_INSERTION_BUFFER_TIME,
 )
-from flowcept.flowceptor.plugins.interceptor_state_manager import (
-    InterceptorStateManager,
-)
-
-from flowcept.flowceptor.plugins.mlflow.mlflow_dao import MLFlowDAO
-from flowcept.flowceptor.plugins.mlflow.interception_event_handler import (
-    InterceptionEventHandler,
-)
-
-
-class MLFlowInterceptor(BaseInterceptor):
-    def __init__(self, plugin_key="mlflow"):
-        super().__init__(plugin_key)
-        self.state_manager = InterceptorStateManager(self.settings)
-        self.dao = MLFlowDAO(self.settings)
-
-    def intercept(self, message: dict):
-        super().post_intercept(message)
-
-    def callback(self):
-        """
-        This function is called whenever a change is identified in the data.
-        It decides what to do in the event of a change.
-        If it's an interesting change, it calls self.intercept; otherwise,
-        let it go....
-        """
-        runs = self.dao.get_finished_run_uuids()
-        for run_uuid_tuple in runs:
-            run_uuid = run_uuid_tuple[0]
-            if not self.state_manager.has_element_id(run_uuid):
-                print(f"We need to intercept this Run: {run_uuid}")
-                run_data = self.dao.get_run_data(run_uuid)
-                self.state_manager.add_element_id(run_uuid)
-                self.intercept(run_data.__dict__)
-
-    def observe(self):
-        event_handler = InterceptionEventHandler(
-            self, self.__class__.callback
-        )
-        while not os.path.isfile(self.settings.file_path):
-            print(
-                f"I can't watch the file {self.settings.file_path},"
-                f" as it does not exist."
-            )
-            print(
-                f"\tI will sleep for {self.settings.watch_interval_sec} sec."
-                f" to see if it appears."
-            )
-            time.sleep(self.settings.watch_interval_sec)
-
-        observer = Observer()
-        observer.schedule(
-            event_handler, self.settings.file_path, recursive=True
+from flowcept.flowceptor.consumers.document_inserter import DocumentInserter
+from flowcept.commons.flowcept_logger import FlowceptLogger
+from flowcept.flowceptor.plugins.base_interceptor import BaseInterceptor
+
+
+class FlowceptConsumerAPI(object):
+    def __init__(
+        self,
+        interceptors: Union[BaseInterceptor, List[BaseInterceptor]] = None,
+    ):
+        self.logger = FlowceptLogger().get_logger()
+        self._document_inserter: DocumentInserter = None
+        self._mq_dao = MQDao()
+
+        if interceptors is not None and type(interceptors) != list:
+            interceptors = [interceptors]
+        self._interceptors: List[BaseInterceptor] = interceptors
+        self.is_started = False
+
+    def start(self):
+        if self.is_started:
+            self.logger.warning("Consumer is already started!")
+            return self
+
+        self._mq_dao.reset_started_mq_threads()
+        if self._interceptors and len(self._interceptors):
+            for interceptor in self._interceptors:
+                self.logger.debug(
+                    f"Flowceptor {interceptor.settings.key} starting..."
+                )
+                interceptor.start()
+                self.logger.debug("... ok!")
+
+        self.logger.debug("Flowcept Consumer starting...")
+        self._document_inserter = DocumentInserter(
+            check_safe_stops=True
+        ).start()
+        sleep(2)
+        self.logger.debug("Ok, we're consuming messages!")
+        self.is_started = True
+        return self
+
+    def stop(self):
+        if not self.is_started:
+            self.logger.warning("Consumer is already stopped!")
+            return
+
+        sleep_time = 5
+        self.logger.debug(
+            f"Received the stop signal. We're going to wait {sleep_time} secs."
+            f" before gracefully stopping..."
         )
-        observer.start()
-        print(f"Watching {self.settings.file_path}")
-
-
-if __name__ == "__main__":
-    try:
-        interceptor = MLFlowInterceptor()
-        interceptor.observe()
-        while True:
-            time.sleep(interceptor.settings.watch_interval_sec)
-    except KeyboardInterrupt:
-        print("Interrupted")
-        sys.exit(0)
+        sleep(sleep_time)
+        if self._interceptors and len(self._interceptors):
+            for interceptor in self._interceptors:
+                self.logger.debug(
+                    f"Flowceptor {interceptor.settings.key} stopping..."
+                )
+                interceptor.stop()
+                self.logger.debug("... ok!")
+        self.logger.debug("Stopping Consumer...")
+        self._document_inserter.stop()
+        self.is_started = False
+        self.logger.debug("All stopped!")
```

### Comparing `flowcept-0.0.97/flowcept/flowceptor/plugins/settings_factory.py` & `flowcept-0.1.1/flowcept/flowceptor/plugins/settings_factory.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 import yaml
 
 from flowcept.commons.vocabulary import Vocabulary
 from flowcept.configs import (
-    PROJECT_DIR_PATH,
     SETTINGS_PATH,
 )
 
 from flowcept.flowceptor.plugins.base_settings_dataclasses import (
     BaseSettings,
     KeyValue,
 )
@@ -16,39 +15,52 @@
 )
 from flowcept.flowceptor.plugins.mlflow.mlflow_dataclasses import (
     MLFlowSettings,
 )
 from flowcept.flowceptor.plugins.tensorboard.tensorboard_dataclasses import (
     TensorboardSettings,
 )
+from flowcept.flowceptor.plugins.dask.dask_dataclasses import (
+    DaskSettings,
+)
+
+
+SETTINGS_CLASSES = {
+    Vocabulary.Settings.ZAMBEZE_KIND: ZambezeSettings,
+    Vocabulary.Settings.MLFLOW_KIND: MLFlowSettings,
+    Vocabulary.Settings.TENSORBOARD_KIND: TensorboardSettings,
+    Vocabulary.Settings.DASK_KIND: DaskSettings,
+}
+
+
+def _build_base_settings(kind: str, settings_dict: dict) -> BaseSettings:
+    settings_obj = SETTINGS_CLASSES[kind](**settings_dict)
+    # if hasattr(settings_obj, "file_path") and not os.path.isabs(
+    #     settings_obj.file_path
+    # ):
+    #     settings_obj.file_path = SETTINGS_PATH
+
+    # # Add default values for abstract settings here:
+    # if settings_obj.enrich_messages is None:
+    #     settings_obj.enrich_messages = True
+    return settings_obj
 
 
 def get_settings(plugin_key: str) -> BaseSettings:
-    # TODO: use the factory pattern
     with open(SETTINGS_PATH) as f:
         data = yaml.load(f, Loader=yaml.FullLoader)
-    settings = data[Vocabulary.Settings.PLUGINS][plugin_key]
-    settings["key"] = plugin_key
-    settings_obj: BaseSettings = None
-    if settings[Vocabulary.Settings.KIND] == Vocabulary.Settings.ZAMBEZE_KIND:
-        settings_obj: ZambezeSettings = ZambezeSettings(**settings)
+    settings_dict = data[Vocabulary.Settings.PLUGINS][plugin_key]
+    if not settings_dict:
+        raise Exception(
+            f"You must specify the plugin <<{plugin_key}>> in"
+            f" the settings YAML file."
+        )
+    settings_dict["key"] = plugin_key
+    kind = settings_dict[Vocabulary.Settings.KIND]
+    settings_obj = _build_base_settings(kind, settings_dict)
+
+    # Add any specific setting builder below
+    if kind == Vocabulary.Settings.ZAMBEZE_KIND:
         settings_obj.key_values_to_filter = [
             KeyValue(**item) for item in settings_obj.key_values_to_filter
         ]
-    elif (
-        settings[Vocabulary.Settings.KIND] == Vocabulary.Settings.MLFLOW_KIND
-    ):
-        settings_obj: MLFlowSettings = MLFlowSettings(**settings)
-        if not os.path.isabs(settings_obj.file_path):
-            settings_obj.file_path = os.path.join(
-                PROJECT_DIR_PATH, settings_obj.file_path
-            )
-    elif (
-        settings[Vocabulary.Settings.KIND]
-        == Vocabulary.Settings.TENSORBOARD_KIND
-    ):
-        settings_obj: TensorboardSettings = TensorboardSettings(**settings)
-        if not os.path.isabs(settings_obj.file_path):
-            settings_obj.file_path = os.path.join(
-                PROJECT_DIR_PATH, settings_obj.file_path
-            )
     return settings_obj
```

### Comparing `flowcept-0.0.97/flowcept/flowceptor/plugins/tensorboard/tensorboard_interceptor.py` & `flowcept-0.1.1/flowcept/flowceptor/plugins/tensorboard/tensorboard_interceptor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,119 @@
-import sys
 import os
 import time
 
 from watchdog.observers import Observer
 from tbparse import SummaryReader
 
+from flowcept.commons.flowcept_data_classes import TaskMessage, Status
+from flowcept.commons.utils import get_utc_now
 from flowcept.flowceptor.plugins.interceptor_state_manager import (
     InterceptorStateManager,
 )
 from flowcept.flowceptor.plugins.base_interceptor import (
     BaseInterceptor,
 )
 from flowcept.flowceptor.plugins.mlflow.interception_event_handler import (
     InterceptionEventHandler,
 )
 
 
 class TensorboardInterceptor(BaseInterceptor):
     def __init__(self, plugin_key="tensorboard"):
         super().__init__(plugin_key)
+        self._observer = None
         self.state_manager = InterceptorStateManager(self.settings)
-
-    def intercept(self, message: dict):
-        print(f"Going to intercept: {message}")
-        super().post_intercept(message)
+        self.state_manager.reset()
+        self.log_metrics = set(self.settings.log_metrics)
 
     def callback(self):
         """
         This function is called whenever a change is identified in the data.
         It decides what to do in the event of a change.
         If it's an interesting change, it calls self.intercept; otherwise,
         let it go....
         """
-        print("New tensorboard event file changed!")
-        # TODO: we're waiting for the file to be completely written.
-        # Is there a better way to be informed when the file is finished?
+        self.logger.debug("New tensorboard directory event!")
+        # TODO: now we're waiting for the file to be completely written.
+        # Is there a better way to inform when the file writing is finished?
         time.sleep(self.settings.watch_interval_sec)
 
         reader = SummaryReader(self.settings.file_path)
         for child_event_file in reader.children:
             child_event = reader.children[child_event_file]
             if self.state_manager.has_element_id(child_event.log_path):
-                print(f"Already extracted metric from {child_event_file}.")
+                self.logger.debug(
+                    f"Already extracted metric from {child_event_file}."
+                )
                 continue
             event_tags = child_event.get_tags()
-            msg = dict()
-            found_metric = False
+
+            tracked_tags = {}
             for tag in self.settings.log_tags:
                 if len(event_tags[tag]):
-                    msg["event_file"] = child_event_file
-                    msg["log_path"] = child_event.log_path
                     df = child_event.__getattribute__(tag)
                     df_dict = dict(zip(df.tag, df.value))
-                    msg[tag] = df_dict
-                    if not found_metric:
-                        for tracked_metric in self.settings.log_metrics:
-                            if tracked_metric in df_dict:
-                                found_metric = True
-                                print("Found metric in this file!")
-                                break
-            if found_metric:
-                # Only intercept if we find a tracked metric in the event
-                self.intercept(msg)
+                    tracked_tags[tag] = df_dict
+
+            if tracked_tags.get("tensors") and len(
+                self.log_metrics.intersection(tracked_tags["tensors"].keys())
+            ):
+                task_msg = TaskMessage()
+                hparams = tracked_tags.get("hparams")
+                if "workflow_id" in hparams:
+                    task_msg.workflow_id = hparams.pop("workflow_id")
+                if "activity_id" in hparams:
+                    task_msg.activity_id = hparams.pop("activity_id")
+
+                task_msg.used = hparams
+                task_msg.generated = tracked_tags.pop("tensors")
+                task_msg.utc_timestamp = get_utc_now()
+                task_msg.status = Status.FINISHED
+                task_msg.custom_metadata = {
+                    "event_file": child_event_file,
+                    "log_path": child_event.log_path,
+                }
+
+                if os.path.isdir(child_event.log_path):
+                    event_files = os.listdir(child_event.log_path)
+                    if len(event_files):
+                        task_msg.task_id = event_files[0]
+
+                if task_msg.task_id is None:
+                    self.logger.error("This is an error")  # TODO: logger
+
+                self.intercept(task_msg)
                 self.state_manager.add_element_id(child_event.log_path)
 
+    def start(self) -> "TensorboardInterceptor":
+        super().start()
+        self.observe()
+        return self
+
+    def stop(self) -> bool:
+        self.logger.debug("Interceptor stopping...")
+        super().stop()
+        self._observer.stop()
+        self.logger.debug("Interceptor stopped.")
+        return True
+
     def observe(self):
         event_handler = InterceptionEventHandler(
             self, self.__class__.callback
         )
         while not os.path.isdir(self.settings.file_path):
-            print(
+            self.logger.debug(
                 f"I can't watch the file {self.settings.file_path},"
                 f" as it does not exist."
             )
-            print(
+            self.logger.debug(
                 f"\tI will sleep for {self.settings.watch_interval_sec} sec."
                 f" to see if it appears."
             )
             time.sleep(self.settings.watch_interval_sec)
 
-        observer = Observer()
-        observer.schedule(
+        self._observer = Observer()
+        self._observer.schedule(
             event_handler, self.settings.file_path, recursive=True
         )
-        observer.start()
-        print(f"Watching {self.settings.file_path}")
-
-
-if __name__ == "__main__":
-    try:
-        interceptor = TensorboardInterceptor()
-        interceptor.observe()
-        while True:
-            time.sleep(interceptor.settings.watch_interval_sec)
-    except KeyboardInterrupt:
-        print("Interrupted")
-        sys.exit(0)
+        self._observer.start()
+        self.logger.debug(f"Watching {self.settings.file_path}")
```

### Comparing `flowcept-0.0.97/setup.py` & `flowcept-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,79 @@
+from sys import platform
+import os
 from setuptools import setup, find_packages
 
-from flowcept import __version__
-from flowcept.configs import PROJECT_NAME
+with open("flowcept/version.py") as f:
+    exec(f.read())
+    version = locals()["__version__"]
 
 with open("README.md") as fh:
     long_description = fh.read()
 
-with open("requirements.txt") as f:
-    requirements = f.read().splitlines()
 
-with open("extra_requirements/zambeze-requirements.txt") as f:
-    zambeze_plugin_requirements = f.read().splitlines()
-
-with open("extra_requirements/mlflow-requirements.txt") as f:
-    mlflow_plugin_requirements = f.read().splitlines()
-
-with open("extra_requirements/tensorboard-requirements.txt") as f:
-    tensorboard_plugin_requirements = f.read().splitlines()
-
-full_requirements = (
-    requirements
-    + zambeze_plugin_requirements
-    + mlflow_plugin_requirements
-    + tensorboard_plugin_requirements
-)
+def get_requirements(file_path):
+    with open(file_path) as f:
+        __requirements = []
+        for line in f.read().splitlines():
+            if not line.startswith("#"):
+                __requirements.append(line)
+    return __requirements
+
+
+requirements = get_requirements("requirements.txt")
+full_requirements = requirements.copy()
+
+# We don't install dev requirements in the user lib.
+extras_requirement_keys = [
+    "zambeze",
+    "mlflow",
+    "tensorboard",
+    "mongo",
+    "dask",
+    "webserver",
+]
+
+MAC_REQUIRES = ["tensorboard"]
+extras_require = dict()
+for req in extras_requirement_keys:
+    if req in MAC_REQUIRES and platform == "darwin":
+        req_path = f"extra_requirements/{req}-requirements-mac.txt"
+        # These env vars are needed to install tensorflow on mac
+        # (at least on m1 chip)
+        # (because of the grpcio package). See:
+        # https://stackoverflow.com/questions/66640705/how-can-i-install-grpcio-on-an-apple-m1-silicon-laptop
+        os.environ["GRPC_PYTHON_BUILD_SYSTEM_OPENSSL"] = "1"
+        os.environ["GRPC_PYTHON_BUILD_SYSTEM_ZLIB"] = "1"
+    else:
+        req_path = f"extra_requirements/{req}-requirements.txt"
+    _requirements = get_requirements(req_path)
+    extras_require[req] = _requirements
+    full_requirements.extend(_requirements)
 
+extras_require["full"] = full_requirements
 setup(
-    name=PROJECT_NAME,
-    version=__version__,
+    name="flowcept",
+    version=version,
     license="MIT",
     author="Oak Ridge National Laboratory",
-    author_email="support@flowcept.org",
-    description="A tool to intercept dataflows",  # TODO: change later
+    # author_email="support@flowcept.org",
+    description="A system to integrate data from multiple workflows.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ORNL/flowcept",
     include_package_data=True,
     install_requires=requirements,
-    extras_require={
-        "full": full_requirements,
-        "mlflow": mlflow_plugin_requirements,
-        "zambeze": zambeze_plugin_requirements,
-        "tensorboard": tensorboard_plugin_requirements,
-    },
+    extras_require=extras_require,
     packages=find_packages(),
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.8",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
-        "Topic :: Documentation :: Sphinx",
+        # "Topic :: Documentation :: Sphinx",
         "Topic :: System :: Distributed Computing",
     ],
-    python_requires=">=3.9",  # TODO: Do we really need py3.9?
+    python_requires=">=3.8",
     # scripts=["bin/flowcept"],
 )
```

### Comparing `flowcept-0.0.97/tests/plugins/test_mlflow.py` & `flowcept-0.1.1/tests/plugins/test_mlflow.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,106 @@
 import unittest
-import threading
-import time
+from time import sleep
 
-from flowcept.flowcept_consumer.consumer import (
-    consume_intercepted_messages,
-)
-from flowcept.flowceptor.plugins.mlflow.mlflow_interceptor import (
-    MLFlowInterceptor,
-)
+from flowcept.commons.daos.document_db_dao import DocumentDBDao
+from flowcept.commons.flowcept_logger import FlowceptLogger
+from flowcept import MLFlowInterceptor, FlowceptConsumerAPI
+
+
+def _init_consumption():
+    TestMLFlow.consumer.start()
+    sleep(3)
 
 
 class TestMLFlow(unittest.TestCase):
+    interceptor = MLFlowInterceptor()
+    consumer: FlowceptConsumerAPI = FlowceptConsumerAPI(interceptor)
+
     def __init__(self, *args, **kwargs):
         super(TestMLFlow, self).__init__(*args, **kwargs)
-        self.interceptor = MLFlowInterceptor()
+        self.logger = FlowceptLogger().get_logger()
 
     def test_pure_run_mlflow(self):
         import uuid
         import mlflow
 
         # from mlflow.tracking import MlflowClient
         # client = MlflowClient()
         mlflow.set_tracking_uri(
-            f"sqlite:///" f"{self.interceptor.settings.file_path}"
+            f"sqlite:///" f"{TestMLFlow.interceptor.settings.file_path}"
         )
         experiment_name = "LinearRegression"
         experiment_id = mlflow.create_experiment(
             experiment_name + str(uuid.uuid4())
         )
         with mlflow.start_run(experiment_id=experiment_id) as run:
             mlflow.log_params({"number_epochs": 10})
             mlflow.log_params({"batch_size": 64})
 
-            print("\nTrained model")
+            self.logger.debug("\nTrained model")
             mlflow.log_metric("loss", 0.04)
 
             return run.info.run_uuid
 
+    def test_pure_run_mlflow_no_ctx_mgr(self):
+        import uuid
+        import mlflow
+
+        # from mlflow.tracking import MlflowClient
+        # client = MlflowClient()
+        mlflow.set_tracking_uri(
+            f"sqlite:///" f"{TestMLFlow.interceptor.settings.file_path}"
+        )
+        experiment_name = "LinearRegression"
+        experiment_id = mlflow.create_experiment(
+            experiment_name + str(uuid.uuid4())
+        )
+        run = mlflow.start_run(experiment_id=experiment_id)
+        mlflow.log_params({"number_epochs": 10})
+        mlflow.log_params({"batch_size": 64})
+        self.logger.debug("\nTrained model")
+        mlflow.log_metric("loss", 0.04)
+        mlflow.end_run()
+        return run.info.run_uuid
+
     def test_get_runs(self):
         runs = self.interceptor.dao.get_finished_run_uuids()
         assert len(runs) > 0
         for run in runs:
             assert type(run[0]) == str
-            print(run[0])
+            self.logger.debug(run[0])
 
     def test_get_run_data(self):
         run_uuid = self.test_pure_run_mlflow()
         run_data = self.interceptor.dao.get_run_data(run_uuid)
-        assert run_data.run_uuid == run_uuid
+        assert run_data.task_id == run_uuid
 
     def test_check_state_manager(self):
         self.interceptor.state_manager.reset()
         self.interceptor.state_manager.add_element_id("dummy-value")
         self.test_pure_run_mlflow()
         runs = self.interceptor.dao.get_finished_run_uuids()
         assert len(runs) > 0
         for run_tuple in runs:
             run_uuid = run_tuple[0]
             assert type(run_uuid) == str
             if not self.interceptor.state_manager.has_element_id(run_uuid):
-                print(f"We need to intercept {run_uuid}")
+                self.logger.debug(f"We need to intercept {run_uuid}")
                 self.interceptor.state_manager.add_element_id(run_uuid)
 
-    def _init_consumption(self):
-        threading.Thread(target=self.interceptor.observe, daemon=True).start()
-        threading.Thread(
-            target=consume_intercepted_messages, daemon=True
-        ).start()
-        time.sleep(3)
-
     def test_observer_and_consumption(self):
-        self._init_consumption()
+        doc_dao = DocumentDBDao()
+        _init_consumption()
         run_uuid = self.test_pure_run_mlflow()
-        time.sleep(10)
+        sleep(10)
         assert self.interceptor.state_manager.has_element_id(run_uuid) is True
+        assert len(doc_dao.find({"task_id": run_uuid})) > 0
+
+    @classmethod
+    def tearDownClass(cls):
+        if TestMLFlow.consumer is not None:
+            TestMLFlow.consumer.stop()
+            sleep(5)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `flowcept-0.0.97/tests/plugins/test_tensorboard.py` & `flowcept-0.1.1/tests/plugins/test_tensorboard.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 import unittest
-import threading
-import time
+from time import sleep
+from uuid import uuid4
 
-from flowcept.flowcept_consumer.consumer import (
-    consume_intercepted_messages,
-)
-from flowcept.flowceptor.plugins.tensorboard.tensorboard_interceptor import (
-    TensorboardInterceptor,
-)
+from flowcept.commons.daos.document_db_dao import DocumentDBDao
+from flowcept.commons.flowcept_logger import FlowceptLogger
+from flowcept import TensorboardInterceptor, FlowceptConsumerAPI
 
 
 class TestTensorboard(unittest.TestCase):
+    interceptor = TensorboardInterceptor()
+    consumer = FlowceptConsumerAPI(interceptor)
+
     def __init__(self, *args, **kwargs):
         super(TestTensorboard, self).__init__(*args, **kwargs)
-        self.interceptor = TensorboardInterceptor()
-        self.interceptor.state_manager.reset()
+        self.logger = FlowceptLogger().get_logger()
 
-    def run_tensorboard_hparam_tuning(self):
-        """
-        Code based on
-         https://www.tensorflow.org/tensorboard/hyperparameter_tuning_with_hparams
-        :return:
-        """
+    def _init_consumption(self):
+        TestTensorboard.consumer.start()
+        sleep(15)
+
+    def reset_log_dir(self):
+        logdir = self.interceptor.settings.file_path
         import os
         import shutil
 
-        logdir = self.interceptor.settings.file_path
         if os.path.exists(logdir):
-            print("Path exists, gonna delete")
+            self.logger.debug("Path exists, gonna delete")
             shutil.rmtree(logdir)
+            sleep(1)
+        os.mkdir(logdir)
+        self.logger.debug("Exists?" + str(os.path.exists(logdir)))
+        watch_interval_sec = self.interceptor.settings.watch_interval_sec
+        # Making sure we'll wait until next watch cycle
+        sleep(watch_interval_sec * 2)
 
+    def test_run_tensorboard_hparam_tuning(self):
+        """
+        Code based on
+         https://www.tensorflow.org/tensorboard/hyperparameter_tuning_with_hparams
+        :return:
+        """
+        logdir = self.interceptor.settings.file_path
+        wf_id = str(uuid4())
         import tensorflow as tf
         from tensorboard.plugins.hparams import api as hp
 
         fashion_mnist = tf.keras.datasets.fashion_mnist
 
         (x_train, y_train), (x_test, y_test) = fashion_mnist.load_data()
         x_train, x_test = x_train / 255.0, x_test / 255.0
@@ -77,15 +89,15 @@
                 loss="sparse_categorical_crossentropy",
                 metrics=["accuracy"],
             )
 
             model.fit(
                 x_train,
                 y_train,
-                epochs=2,
+                epochs=1,
                 callbacks=[
                     tf.keras.callbacks.TensorBoard(logdir),
                     # log metrics
                     hp.KerasCallback(logdir, hparams),  # log hparams
                 ],
                 batch_size=hparams[HP_BATCHSIZES],
             )  # Run with 1 epoch to speed things up for tests
@@ -103,47 +115,53 @@
         for num_units in HP_NUM_UNITS.domain.values:
             for dropout_rate in (
                 HP_DROPOUT.domain.min_value,
                 HP_DROPOUT.domain.max_value,
             ):
                 for optimizer in HP_OPTIMIZER.domain.values:
                     for batch_size in HP_BATCHSIZES.domain.values:
+                        # These two added ids below are optional and useful
+                        # just to contextualize this run.
                         hparams = {
+                            "workflow_id": wf_id,
+                            "activity_id": "hyperparam_evaluation",
                             HP_NUM_UNITS: num_units,
                             HP_DROPOUT: dropout_rate,
                             HP_OPTIMIZER: optimizer,
                             HP_BATCHSIZES: batch_size,
                         }
-                        run_name = "run-%d" % session_num
-                        print("--- Starting trial: %s" % run_name)
-                        print({h.name: hparams[h] for h in hparams})
+                        run_name = f"wf_id_{wf_id}_{session_num}"
+                        self.logger.debug("--- Starting trial: %s" % run_name)
+                        self.logger.debug(f"{hparams}")
                         run(f"{logdir}/" + run_name, hparams)
                         session_num += 1
 
-        return logdir
-
-    def _init_consumption(self):
-        threading.Thread(target=self.interceptor.observe, daemon=True).start()
-        threading.Thread(
-            target=consume_intercepted_messages, daemon=True
-        ).start()
-        time.sleep(3)
+        return wf_id
 
     def test_observer_and_consumption(self):
+        self.reset_log_dir()
         self._init_consumption()
-        self.run_tensorboard_hparam_tuning()
-        time.sleep(20)
+        wf_id = self.test_run_tensorboard_hparam_tuning()
+        self.logger.debug("Done training. Sleeping some time...")
+
+        watch_interval_sec = self.interceptor.settings.watch_interval_sec
+        # Making sure we'll wait until next watch cycle
+        sleep(watch_interval_sec * 2)
         assert self.interceptor.state_manager.count() == 16
+        doc_dao = DocumentDBDao()
+        docs = doc_dao.find({"workflow_id": wf_id})
+        assert len(docs) == 16
+        TestTensorboard.consumer.stop()
 
     def test_read_tensorboard_hparam_tuning(self):
-
-        logdir = self.run_tensorboard_hparam_tuning()
-
+        self.reset_log_dir()
+        self.test_run_tensorboard_hparam_tuning()
         from tbparse import SummaryReader
 
+        logdir = self.interceptor.settings.file_path
         reader = SummaryReader(logdir)
 
         TRACKED_TAGS = {"scalars", "hparams", "tensors"}
         TRACKED_METRICS = {"accuracy"}
 
         output = []
         for child_event_file in reader.children:
@@ -162,14 +180,20 @@
                     df_dict = dict(zip(df.tag, df.value))
                     msg[tag] = df_dict
 
                     if not found_metric:
                         for tracked_metric in TRACKED_METRICS:
                             if tracked_metric in df_dict:
                                 found_metric = True
-                                print("Found metric!")
+                                self.logger.debug("Found metric!")
                                 break
 
             if found_metric:
                 # Only append if we find a tracked metric in the event
                 output.append(msg)
         assert len(output) == 16
+
+    @classmethod
+    def tearDownClass(cls):
+        if TestTensorboard.consumer is not None:
+            TestTensorboard.consumer.stop()
+            sleep(2)
```

### Comparing `flowcept-0.0.97/tests/plugins/test_zambeze.py` & `flowcept-0.1.1/tests/plugins/test_zambeze.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,76 @@
+from time import sleep
 import unittest
 import json
-import threading
 import pika
+from uuid import uuid4
 
-from flowcept.flowcept_consumer.consumer import (
-    consume_intercepted_messages,
-)
-from flowcept.flowceptor.plugins.zambeze.zambeze_interceptor import (
-    ZambezeInterceptor,
-)
+from flowcept.commons.flowcept_logger import FlowceptLogger
+from flowcept.commons.daos.document_db_dao import DocumentDBDao
+from flowcept import ZambezeInterceptor, FlowceptConsumerAPI
 from flowcept.flowceptor.plugins.zambeze.zambeze_dataclasses import (
     ZambezeMessage,
 )
 
 
 class TestZambeze(unittest.TestCase):
     def __init__(self, *args, **kwargs):
         super(TestZambeze, self).__init__(*args, **kwargs)
-        self.interceptor = ZambezeInterceptor()
+        self.logger = FlowceptLogger().get_logger()
+        interceptor = ZambezeInterceptor()
+        self.consumer = FlowceptConsumerAPI(interceptor)
 
         self._connection = pika.BlockingConnection(
             pika.ConnectionParameters(
-                self.interceptor.settings.host,
-                self.interceptor.settings.port,
+                interceptor.settings.host,
+                interceptor.settings.port,
             )
         )
         self._channel = self._connection.channel()
-        self._channel.queue_declare(
-            queue=self.interceptor.settings.queue_name
-        )
-        threading.Thread(target=self.interceptor.observe, daemon=True).start()
-        threading.Thread(
-            target=consume_intercepted_messages, daemon=True
-        ).start()
+        self._queue_name = interceptor.settings.queue_name
+        self._channel.queue_declare(queue=self._queue_name)
+
+        self.consumer.start()
 
     def test_send_message(self):
+        another_act_id = str(uuid4())
+        act_id = str(uuid4())
         msg = ZambezeMessage(
             **{
                 "name": "ImageMagick",
-                "activity_id": "xyz-uuid",
-                "campaign_id": "abc-uuid",
+                "activity_id": act_id,
+                "campaign_id": "campaign-uuid",
                 "origin_agent_id": "def-uuid",
                 "files": ["globus://Users/6o1/file.txt"],
                 "command": "convert",
                 "activity_status": "CREATED",
                 "arguments": [
                     "-delay",
                     "20",
                     "-loop",
                     "0",
                     "~/tests/campaigns/imagesequence/*.jpg",
                     "a.gif",
                 ],
                 "kwargs": {},
-                "depends_on": [],
+                "depends_on": [another_act_id],
             }
         )
 
         self._channel.basic_publish(
             exchange="",
-            routing_key=self.interceptor.settings.queue_name,
+            routing_key=self._queue_name,
             body=json.dumps(msg.__dict__),
         )
 
-        print(" [x] Sent msg")
+        self.logger.debug(" [x] Sent msg")
+        sleep(5)
         self._connection.close()
-        import time
-
-        time.sleep(3)
+        sleep(10)
+        doc_dao = DocumentDBDao()
+        assert len(doc_dao.find({"task_id": act_id})) > 0
+        self.consumer.stop()
+        sleep(2)
 
 
 if __name__ == "__main__":
     unittest.main()
```

