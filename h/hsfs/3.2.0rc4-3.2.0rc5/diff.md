# Comparing `tmp/hsfs-3.2.0rc4.tar.gz` & `tmp/hsfs-3.2.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsfs-3.2.0rc4.tar", last modified: Tue Jun  6 09:54:01 2023, max compression
+gzip compressed data, was "hsfs-3.2.0rc5.tar", last modified: Mon Jun 19 21:29:01 2023, max compression
```

## Comparing `hsfs-3.2.0rc4.tar` & `hsfs-3.2.0rc5.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0     1006     1006        0 2023-06-06 09:54:01.291545 hsfs-3.2.0rc4/
--rw-r--r--   0     1006     1006       40 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/MANIFEST.in
--rw-r--r--   0     1006     1006     7714 2023-06-06 09:54:01.291545 hsfs-3.2.0rc4/PKG-INFO
--rw-r--r--   0     1006     1006     5539 2023-06-06 09:54:00.000000 hsfs-3.2.0rc4/README.md
-drwxr-xr-x   0     1006     1006        0 2023-06-06 09:54:01.271546 hsfs-3.2.0rc4/hsfs/
--rw-r--r--   0     1006     1006     1182 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/__init__.py
-drwxr-xr-x   0     1006     1006        0 2023-06-06 09:54:01.275546 hsfs-3.2.0rc4/hsfs/client/
--rw-r--r--   0     1006     1006     1694 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/client/__init__.py
--rw-r--r--   0     1006     1006     1132 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/client/auth.py
--rw-r--r--   0     1006     1006     6622 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/client/base.py
--rw-r--r--   0     1006     1006     2090 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/client/exceptions.py
--rw-r--r--   0     1006     1006    11621 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/client/external.py
--rw-r--r--   0     1006     1006     7924 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/client/hopsworks.py
--rw-r--r--   0     1006     1006     1536 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/code.py
--rw-r--r--   0     1006     1006    18899 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/connection.py
-drwxr-xr-x   0     1006     1006        0 2023-06-06 09:54:01.275546 hsfs-3.2.0rc4/hsfs/constructor/
--rw-r--r--   0     1006     1006      605 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/constructor/__init__.py
--rw-r--r--   0     1006     1006     1261 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/constructor/external_feature_group_alias.py
--rw-r--r--   0     1006     1006     5106 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/constructor/filter.py
--rw-r--r--   0     1006     1006     2981 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/constructor/fs_query.py
--rw-r--r--   0     1006     1006     1731 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/constructor/hudi_feature_group_alias.py
--rw-r--r--   0     1006     1006     2157 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/constructor/join.py
--rw-r--r--   0     1006     1006     1577 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/constructor/prepared_statement_parameter.py
--rw-r--r--   0     1006     1006    20138 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/constructor/query.py
--rw-r--r--   0     1006     1006     3331 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/constructor/serving_prepared_statement.py
-drwxr-xr-x   0     1006     1006        0 2023-06-06 09:54:01.291545 hsfs-3.2.0rc4/hsfs/core/
--rw-r--r--   0     1006     1006      605 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/__init__.py
--rw-r--r--   0     1006     1006     3688 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/builtin_transformation_function.py
--rw-r--r--   0     1006     1006     1853 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/code_api.py
--rw-r--r--   0     1006     1006     3292 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/code_engine.py
--rw-r--r--   0     1006     1006     3509 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/dataset_api.py
--rw-r--r--   0     1006     1006     1030 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/deltastreamer_jobconf.py
--rw-r--r--   0     1006     1006     1609 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/execution.py
--rw-r--r--   0     1006     1006     5396 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/expectation_api.py
--rw-r--r--   0     1006     1006     2632 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/expectation_engine.py
--rw-r--r--   0     1006     1006     6356 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/expectation_suite_api.py
--rw-r--r--   0     1006     1006     4002 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/expectation_suite_engine.py
--rw-r--r--   0     1006     1006     9792 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/explicit_provenance.py
--rw-r--r--   0     1006     1006     5418 2023-06-06 09:53:56.000000 hsfs-3.2.0rc4/hsfs/core/external_feature_group_engine.py
--rw-r--r--   0     1006     1006    13334 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/feature_group_api.py
--rw-r--r--   0     1006     1006     6610 2023-06-06 09:53:56.000000 hsfs-3.2.0rc4/hsfs/core/feature_group_base_engine.py
--rw-r--r--   0     1006     1006    13164 2023-06-06 09:53:56.000000 hsfs-3.2.0rc4/hsfs/core/feature_group_engine.py
--rw-r--r--   0     1006     1006     1238 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/feature_store_api.py
--rw-r--r--   0     1006     1006     9739 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/feature_view_api.py
--rw-r--r--   0     1006     1006    24896 2023-06-06 09:53:56.000000 hsfs-3.2.0rc4/hsfs/core/feature_view_engine.py
--rw-r--r--   0     1006     1006     5024 2023-06-06 09:53:56.000000 hsfs-3.2.0rc4/hsfs/core/great_expectation_engine.py
--rw-r--r--   0     1006     1006      828 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/hosts_api.py
--rw-r--r--   0     1006     1006    11546 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/hudi_engine.py
--rw-r--r--   0     1006     1006     1211 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/ingestion_job.py
--rw-r--r--   0     1006     1006     2262 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/ingestion_job_conf.py
--rw-r--r--   0     1006     1006     1077 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/inode.py
--rw-r--r--   0     1006     1006     2906 2023-06-06 09:53:56.000000 hsfs-3.2.0rc4/hsfs/core/job.py
--rw-r--r--   0     1006     1006     2004 2023-06-06 09:53:56.000000 hsfs-3.2.0rc4/hsfs/core/job_api.py
--rw-r--r--   0     1006     1006     2048 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/job_configuration.py
--rw-r--r--   0     1006     1006     1530 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/kafka_api.py
--rw-r--r--   0     1006     1006      898 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/project_api.py
--rw-r--r--   0     1006     1006     1093 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/query_constructor_api.py
--rw-r--r--   0     1006     1006      875 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/services_api.py
--rw-r--r--   0     1006     1006     4204 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/statistics_api.py
--rw-r--r--   0     1006     1006     8159 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/statistics_engine.py
--rw-r--r--   0     1006     1006     2325 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/storage_connector_api.py
--rw-r--r--   0     1006     1006     4696 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/tags_api.py
--rw-r--r--   0     1006     1006     6685 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/training_dataset_api.py
--rw-r--r--   0     1006     1006     6357 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/training_dataset_engine.py
--rw-r--r--   0     1006     1006     2148 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/training_dataset_job_conf.py
--rw-r--r--   0     1006     1006     4161 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/transformation_function_api.py
--rw-r--r--   0     1006     1006    14792 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/transformation_function_engine.py
--rw-r--r--   0     1006     1006     4773 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/validation_report_api.py
--rw-r--r--   0     1006     1006     3640 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/validation_report_engine.py
--rw-r--r--   0     1006     1006     2158 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/validation_result_api.py
--rw-r--r--   0     1006     1006     5469 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/validation_result_engine.py
--rw-r--r--   0     1006     1006     1261 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/core/variable_api.py
--rw-r--r--   0     1006     1006    18519 2023-06-06 09:53:56.000000 hsfs-3.2.0rc4/hsfs/core/vector_server.py
--rw-r--r--   0     1006     1006     1655 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/decorators.py
-drwxr-xr-x   0     1006     1006        0 2023-06-06 09:54:01.291545 hsfs-3.2.0rc4/hsfs/engine/
--rw-r--r--   0     1006     1006     2244 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/engine/__init__.py
--rw-r--r--   0     1006     1006    46955 2023-06-06 09:53:56.000000 hsfs-3.2.0rc4/hsfs/engine/python.py
--rw-r--r--   0     1006     1006    43466 2023-06-06 09:53:56.000000 hsfs-3.2.0rc4/hsfs/engine/spark.py
--rw-r--r--   0     1006     1006    21585 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/expectation_suite.py
--rw-r--r--   0     1006     1006     6857 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/feature.py
--rw-r--r--   0     1006     1006   110697 2023-06-06 09:53:56.000000 hsfs-3.2.0rc4/hsfs/feature_group.py
--rw-r--r--   0     1006     1006     3338 2023-06-06 09:53:56.000000 hsfs-3.2.0rc4/hsfs/feature_group_commit.py
--rw-r--r--   0     1006     1006     1986 2023-06-06 09:53:56.000000 hsfs-3.2.0rc4/hsfs/feature_group_writer.py
--rw-r--r--   0     1006     1006    62935 2023-06-06 09:53:56.000000 hsfs-3.2.0rc4/hsfs/feature_store.py
--rw-r--r--   0     1006     1006    95713 2023-06-06 09:53:56.000000 hsfs-3.2.0rc4/hsfs/feature_view.py
--rw-r--r--   0     1006     1006     4822 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/ge_expectation.py
--rw-r--r--   0     1006     1006     8633 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/ge_validation_result.py
--rw-r--r--   0     1006     1006     1450 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/split_statistics.py
--rw-r--r--   0     1006     1006     2893 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/statistics.py
--rw-r--r--   0     1006     1006     3313 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/statistics_config.py
--rw-r--r--   0     1006     1006    39092 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/storage_connector.py
--rw-r--r--   0     1006     1006     1850 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/tag.py
--rw-r--r--   0     1006     1006    35625 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/training_dataset.py
--rw-r--r--   0     1006     1006     3542 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/training_dataset_feature.py
--rw-r--r--   0     1006     1006     2759 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/training_dataset_split.py
--rw-r--r--   0     1006     1006     8929 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/transformation_function.py
--rw-r--r--   0     1006     1006     2179 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/transformation_function_attached.py
--rw-r--r--   0     1006     1006     3491 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/user.py
--rw-r--r--   0     1006     1006    11410 2023-06-06 09:53:56.000000 hsfs-3.2.0rc4/hsfs/util.py
--rw-r--r--   0     1006     1006     7519 2023-06-05 14:18:50.000000 hsfs-3.2.0rc4/hsfs/validation_report.py
--rw-r--r--   0     1006     1006      631 2023-06-06 09:53:56.000000 hsfs-3.2.0rc4/hsfs/version.py
-drwxr-xr-x   0     1006     1006        0 2023-06-06 09:54:01.271546 hsfs-3.2.0rc4/hsfs.egg-info/
--rw-r--r--   0     1006     1006     7714 2023-06-06 09:54:01.000000 hsfs-3.2.0rc4/hsfs.egg-info/PKG-INFO
--rw-r--r--   0     1006     1006     2805 2023-06-06 09:54:01.000000 hsfs-3.2.0rc4/hsfs.egg-info/SOURCES.txt
--rw-r--r--   0     1006     1006        1 2023-06-06 09:54:01.000000 hsfs-3.2.0rc4/hsfs.egg-info/dependency_links.txt
--rw-r--r--   0     1006     1006      679 2023-06-06 09:54:01.000000 hsfs-3.2.0rc4/hsfs.egg-info/requires.txt
--rw-r--r--   0     1006     1006        5 2023-06-06 09:54:01.000000 hsfs-3.2.0rc4/hsfs.egg-info/top_level.txt
--rw-r--r--   0     1006     1006       38 2023-06-06 09:54:01.291545 hsfs-3.2.0rc4/setup.cfg
--rw-r--r--   0     1006     1006     2756 2023-06-06 09:53:56.000000 hsfs-3.2.0rc4/setup.py
+drwxr-xr-x   0     1006     1006        0 2023-06-19 21:29:01.929939 hsfs-3.2.0rc5/
+-rw-r--r--   0     1006     1006       40 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/MANIFEST.in
+-rw-r--r--   0     1006     1006     7714 2023-06-19 21:29:01.929939 hsfs-3.2.0rc5/PKG-INFO
+-rw-r--r--   0     1006     1006     5539 2023-06-19 21:29:01.000000 hsfs-3.2.0rc5/README.md
+drwxr-xr-x   0     1006     1006        0 2023-06-19 21:29:01.917939 hsfs-3.2.0rc5/hsfs/
+-rw-r--r--   0     1006     1006     1182 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-06-19 21:29:01.921939 hsfs-3.2.0rc5/hsfs/client/
+-rw-r--r--   0     1006     1006     1694 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/client/__init__.py
+-rw-r--r--   0     1006     1006     1132 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/client/auth.py
+-rw-r--r--   0     1006     1006     6622 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/client/base.py
+-rw-r--r--   0     1006     1006     2090 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/client/exceptions.py
+-rw-r--r--   0     1006     1006    11621 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/client/external.py
+-rw-r--r--   0     1006     1006     7924 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/client/hopsworks.py
+-rw-r--r--   0     1006     1006     1536 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/code.py
+-rw-r--r--   0     1006     1006    18899 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/connection.py
+drwxr-xr-x   0     1006     1006        0 2023-06-19 21:29:01.921939 hsfs-3.2.0rc5/hsfs/constructor/
+-rw-r--r--   0     1006     1006      605 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/constructor/__init__.py
+-rw-r--r--   0     1006     1006     1261 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/constructor/external_feature_group_alias.py
+-rw-r--r--   0     1006     1006     5106 2023-06-19 21:28:58.000000 hsfs-3.2.0rc5/hsfs/constructor/filter.py
+-rw-r--r--   0     1006     1006     2981 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/constructor/fs_query.py
+-rw-r--r--   0     1006     1006     1731 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/constructor/hudi_feature_group_alias.py
+-rw-r--r--   0     1006     1006     2152 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/constructor/join.py
+-rw-r--r--   0     1006     1006     1577 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/constructor/prepared_statement_parameter.py
+-rw-r--r--   0     1006     1006    20138 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/constructor/query.py
+-rw-r--r--   0     1006     1006     3331 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/constructor/serving_prepared_statement.py
+drwxr-xr-x   0     1006     1006        0 2023-06-19 21:29:01.929939 hsfs-3.2.0rc5/hsfs/core/
+-rw-r--r--   0     1006     1006      605 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/__init__.py
+-rw-r--r--   0     1006     1006     3688 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/builtin_transformation_function.py
+-rw-r--r--   0     1006     1006     1853 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/code_api.py
+-rw-r--r--   0     1006     1006     3292 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/code_engine.py
+-rw-r--r--   0     1006     1006     3509 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/dataset_api.py
+-rw-r--r--   0     1006     1006     1030 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/deltastreamer_jobconf.py
+-rw-r--r--   0     1006     1006     1609 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/execution.py
+-rw-r--r--   0     1006     1006     5396 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/core/expectation_api.py
+-rw-r--r--   0     1006     1006     2632 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/core/expectation_engine.py
+-rw-r--r--   0     1006     1006     6356 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/core/expectation_suite_api.py
+-rw-r--r--   0     1006     1006     4002 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/core/expectation_suite_engine.py
+-rw-r--r--   0     1006     1006     9792 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/core/explicit_provenance.py
+-rw-r--r--   0     1006     1006     5418 2023-06-19 21:28:58.000000 hsfs-3.2.0rc5/hsfs/core/external_feature_group_engine.py
+-rw-r--r--   0     1006     1006    13334 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/core/feature_group_api.py
+-rw-r--r--   0     1006     1006     6610 2023-06-19 21:28:58.000000 hsfs-3.2.0rc5/hsfs/core/feature_group_base_engine.py
+-rw-r--r--   0     1006     1006    13164 2023-06-19 21:28:58.000000 hsfs-3.2.0rc5/hsfs/core/feature_group_engine.py
+-rw-r--r--   0     1006     1006     1238 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/feature_store_api.py
+-rw-r--r--   0     1006     1006     9739 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/core/feature_view_api.py
+-rw-r--r--   0     1006     1006    24896 2023-06-19 21:28:58.000000 hsfs-3.2.0rc5/hsfs/core/feature_view_engine.py
+-rw-r--r--   0     1006     1006     5024 2023-06-19 21:28:58.000000 hsfs-3.2.0rc5/hsfs/core/great_expectation_engine.py
+-rw-r--r--   0     1006     1006      828 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/hosts_api.py
+-rw-r--r--   0     1006     1006    11546 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/core/hudi_engine.py
+-rw-r--r--   0     1006     1006     1211 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/ingestion_job.py
+-rw-r--r--   0     1006     1006     2262 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/ingestion_job_conf.py
+-rw-r--r--   0     1006     1006     1077 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/core/inode.py
+-rw-r--r--   0     1006     1006     2906 2023-06-19 21:28:58.000000 hsfs-3.2.0rc5/hsfs/core/job.py
+-rw-r--r--   0     1006     1006     2004 2023-06-19 21:28:58.000000 hsfs-3.2.0rc5/hsfs/core/job_api.py
+-rw-r--r--   0     1006     1006     2048 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/core/job_configuration.py
+-rw-r--r--   0     1006     1006     1530 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/core/kafka_api.py
+-rw-r--r--   0     1006     1006      898 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/project_api.py
+-rw-r--r--   0     1006     1006     1093 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/query_constructor_api.py
+-rw-r--r--   0     1006     1006      875 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/services_api.py
+-rw-r--r--   0     1006     1006     4204 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/statistics_api.py
+-rw-r--r--   0     1006     1006     8159 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/core/statistics_engine.py
+-rw-r--r--   0     1006     1006     2325 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/storage_connector_api.py
+-rw-r--r--   0     1006     1006     4696 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/tags_api.py
+-rw-r--r--   0     1006     1006     6685 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/training_dataset_api.py
+-rw-r--r--   0     1006     1006     6357 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/training_dataset_engine.py
+-rw-r--r--   0     1006     1006     2148 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/core/training_dataset_job_conf.py
+-rw-r--r--   0     1006     1006     4161 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/core/transformation_function_api.py
+-rw-r--r--   0     1006     1006    14792 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/core/transformation_function_engine.py
+-rw-r--r--   0     1006     1006     4773 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/core/validation_report_api.py
+-rw-r--r--   0     1006     1006     3640 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/core/validation_report_engine.py
+-rw-r--r--   0     1006     1006     2158 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/core/validation_result_api.py
+-rw-r--r--   0     1006     1006     5469 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/core/validation_result_engine.py
+-rw-r--r--   0     1006     1006     1261 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/core/variable_api.py
+-rw-r--r--   0     1006     1006    18519 2023-06-19 21:28:58.000000 hsfs-3.2.0rc5/hsfs/core/vector_server.py
+-rw-r--r--   0     1006     1006     1655 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/decorators.py
+drwxr-xr-x   0     1006     1006        0 2023-06-19 21:29:01.929939 hsfs-3.2.0rc5/hsfs/engine/
+-rw-r--r--   0     1006     1006     2244 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/engine/__init__.py
+-rw-r--r--   0     1006     1006    46955 2023-06-19 21:28:58.000000 hsfs-3.2.0rc5/hsfs/engine/python.py
+-rw-r--r--   0     1006     1006    43466 2023-06-19 21:28:58.000000 hsfs-3.2.0rc5/hsfs/engine/spark.py
+-rw-r--r--   0     1006     1006    21585 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/expectation_suite.py
+-rw-r--r--   0     1006     1006     6857 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/feature.py
+-rw-r--r--   0     1006     1006   110697 2023-06-19 21:28:58.000000 hsfs-3.2.0rc5/hsfs/feature_group.py
+-rw-r--r--   0     1006     1006     3338 2023-06-19 21:28:58.000000 hsfs-3.2.0rc5/hsfs/feature_group_commit.py
+-rw-r--r--   0     1006     1006     1986 2023-06-19 21:28:58.000000 hsfs-3.2.0rc5/hsfs/feature_group_writer.py
+-rw-r--r--   0     1006     1006    62935 2023-06-19 21:28:58.000000 hsfs-3.2.0rc5/hsfs/feature_store.py
+-rw-r--r--   0     1006     1006    95713 2023-06-19 21:28:58.000000 hsfs-3.2.0rc5/hsfs/feature_view.py
+-rw-r--r--   0     1006     1006     4822 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/ge_expectation.py
+-rw-r--r--   0     1006     1006     8633 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/ge_validation_result.py
+-rw-r--r--   0     1006     1006     1450 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/split_statistics.py
+-rw-r--r--   0     1006     1006     2893 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/statistics.py
+-rw-r--r--   0     1006     1006     3313 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/statistics_config.py
+-rw-r--r--   0     1006     1006    39092 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/storage_connector.py
+-rw-r--r--   0     1006     1006     1850 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/tag.py
+-rw-r--r--   0     1006     1006    35625 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/training_dataset.py
+-rw-r--r--   0     1006     1006     3542 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/training_dataset_feature.py
+-rw-r--r--   0     1006     1006     2759 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/training_dataset_split.py
+-rw-r--r--   0     1006     1006     8929 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/transformation_function.py
+-rw-r--r--   0     1006     1006     2179 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/transformation_function_attached.py
+-rw-r--r--   0     1006     1006     3491 2023-06-05 14:18:50.000000 hsfs-3.2.0rc5/hsfs/user.py
+-rw-r--r--   0     1006     1006    11410 2023-06-19 21:28:58.000000 hsfs-3.2.0rc5/hsfs/util.py
+-rw-r--r--   0     1006     1006     7519 2023-06-19 21:22:26.000000 hsfs-3.2.0rc5/hsfs/validation_report.py
+-rw-r--r--   0     1006     1006      631 2023-06-19 21:28:58.000000 hsfs-3.2.0rc5/hsfs/version.py
+drwxr-xr-x   0     1006     1006        0 2023-06-19 21:29:01.921939 hsfs-3.2.0rc5/hsfs.egg-info/
+-rw-r--r--   0     1006     1006     7714 2023-06-19 21:29:01.000000 hsfs-3.2.0rc5/hsfs.egg-info/PKG-INFO
+-rw-r--r--   0     1006     1006     2805 2023-06-19 21:29:01.000000 hsfs-3.2.0rc5/hsfs.egg-info/SOURCES.txt
+-rw-r--r--   0     1006     1006        1 2023-06-19 21:29:01.000000 hsfs-3.2.0rc5/hsfs.egg-info/dependency_links.txt
+-rw-r--r--   0     1006     1006      679 2023-06-19 21:29:01.000000 hsfs-3.2.0rc5/hsfs.egg-info/requires.txt
+-rw-r--r--   0     1006     1006        5 2023-06-19 21:29:01.000000 hsfs-3.2.0rc5/hsfs.egg-info/top_level.txt
+-rw-r--r--   0     1006     1006       38 2023-06-19 21:29:01.929939 hsfs-3.2.0rc5/setup.cfg
+-rw-r--r--   0     1006     1006     2756 2023-06-19 21:28:58.000000 hsfs-3.2.0rc5/setup.py
```

### Comparing `hsfs-3.2.0rc4/PKG-INFO` & `hsfs-3.2.0rc5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsfs
-Version: 3.2.0rc4
+Version: 3.2.0rc5
 Summary: HSFS: An environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api
 Author: Hopsworks AB
 Author-email: moritz@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc4
+Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc5
 Description: # Hopsworks Feature Store
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hsfs Version: 3.2.0rc4 Summary: HSFS: An
+Metadata-Version: 2.1 Name: hsfs Version: 3.2.0rc5 Summary: HSFS: An
 environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api Author: Hopsworks
 AB Author-email: moritz@logicalclocks.com License: Apache License 2.0 Download-
-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc4
+URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc5
 Description: # Hopsworks Feature Store
   [Hopsworks_Community] [Hopsworks_Feature_Store_Documentation] [PyPiStatus]
            [Scala/Java_Artifacts] [Downloads] [CodeStyle] [License]
 HSFS is the library to interact with the Hopsworks Feature Store. The library
 makes creating new features, feature groups and training datasets easy. The
 library is environment independent and can be used in two modes: - Spark mode:
 For data engineering jobs that create and write features into the feature store
```

### Comparing `hsfs-3.2.0rc4/README.md` & `hsfs-3.2.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/__init__.py` & `hsfs-3.2.0rc5/hsfs/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/client/__init__.py` & `hsfs-3.2.0rc5/hsfs/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/client/auth.py` & `hsfs-3.2.0rc5/hsfs/client/auth.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/client/base.py` & `hsfs-3.2.0rc5/hsfs/client/base.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/client/exceptions.py` & `hsfs-3.2.0rc5/hsfs/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/client/external.py` & `hsfs-3.2.0rc5/hsfs/client/external.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/client/hopsworks.py` & `hsfs-3.2.0rc5/hsfs/client/hopsworks.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/code.py` & `hsfs-3.2.0rc5/hsfs/code.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/connection.py` & `hsfs-3.2.0rc5/hsfs/connection.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/constructor/__init__.py` & `hsfs-3.2.0rc5/hsfs/constructor/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/constructor/external_feature_group_alias.py` & `hsfs-3.2.0rc5/hsfs/constructor/external_feature_group_alias.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/constructor/filter.py` & `hsfs-3.2.0rc5/hsfs/constructor/filter.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/constructor/fs_query.py` & `hsfs-3.2.0rc5/hsfs/constructor/fs_query.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/constructor/hudi_feature_group_alias.py` & `hsfs-3.2.0rc5/hsfs/constructor/hudi_feature_group_alias.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/constructor/join.py` & `hsfs-3.2.0rc5/hsfs/constructor/join.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         json_decamelized = humps.decamelize(json_dict)
 
         return cls(
             query=query.Query.from_response_json(json_decamelized["query"]),
             on=json_decamelized.get("on", None),
             left_on=json_decamelized.get("left_on", None),
             right_on=json_decamelized.get("right_on", None),
-            join_type=json_decamelized.get("join_type", None),
+            join_type=json_decamelized.get("type", None),
             prefix=json_decamelized.get("prefix", None),
         )
 
     @property
     def query(self):
         return self._query
```

### Comparing `hsfs-3.2.0rc4/hsfs/constructor/prepared_statement_parameter.py` & `hsfs-3.2.0rc5/hsfs/constructor/prepared_statement_parameter.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/constructor/query.py` & `hsfs-3.2.0rc5/hsfs/constructor/query.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/constructor/serving_prepared_statement.py` & `hsfs-3.2.0rc5/hsfs/constructor/serving_prepared_statement.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/__init__.py` & `hsfs-3.2.0rc5/hsfs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/builtin_transformation_function.py` & `hsfs-3.2.0rc5/hsfs/core/builtin_transformation_function.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/code_api.py` & `hsfs-3.2.0rc5/hsfs/core/code_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/code_engine.py` & `hsfs-3.2.0rc5/hsfs/core/code_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/dataset_api.py` & `hsfs-3.2.0rc5/hsfs/core/dataset_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/deltastreamer_jobconf.py` & `hsfs-3.2.0rc5/hsfs/core/deltastreamer_jobconf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/execution.py` & `hsfs-3.2.0rc5/hsfs/core/execution.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/expectation_api.py` & `hsfs-3.2.0rc5/hsfs/core/expectation_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/expectation_engine.py` & `hsfs-3.2.0rc5/hsfs/core/expectation_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/expectation_suite_api.py` & `hsfs-3.2.0rc5/hsfs/core/expectation_suite_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/expectation_suite_engine.py` & `hsfs-3.2.0rc5/hsfs/core/expectation_suite_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/explicit_provenance.py` & `hsfs-3.2.0rc5/hsfs/core/explicit_provenance.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/external_feature_group_engine.py` & `hsfs-3.2.0rc5/hsfs/core/external_feature_group_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/feature_group_api.py` & `hsfs-3.2.0rc5/hsfs/core/feature_group_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/feature_group_base_engine.py` & `hsfs-3.2.0rc5/hsfs/core/feature_group_base_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/feature_group_engine.py` & `hsfs-3.2.0rc5/hsfs/core/feature_group_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/feature_store_api.py` & `hsfs-3.2.0rc5/hsfs/core/feature_store_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/feature_view_api.py` & `hsfs-3.2.0rc5/hsfs/core/feature_view_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/feature_view_engine.py` & `hsfs-3.2.0rc5/hsfs/core/feature_view_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/great_expectation_engine.py` & `hsfs-3.2.0rc5/hsfs/core/great_expectation_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/hosts_api.py` & `hsfs-3.2.0rc5/hsfs/core/hosts_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/hudi_engine.py` & `hsfs-3.2.0rc5/hsfs/core/hudi_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/ingestion_job.py` & `hsfs-3.2.0rc5/hsfs/core/ingestion_job.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/ingestion_job_conf.py` & `hsfs-3.2.0rc5/hsfs/core/ingestion_job_conf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/inode.py` & `hsfs-3.2.0rc5/hsfs/core/inode.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/job.py` & `hsfs-3.2.0rc5/hsfs/core/job.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/job_api.py` & `hsfs-3.2.0rc5/hsfs/core/job_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/job_configuration.py` & `hsfs-3.2.0rc5/hsfs/core/job_configuration.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/kafka_api.py` & `hsfs-3.2.0rc5/hsfs/core/kafka_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/project_api.py` & `hsfs-3.2.0rc5/hsfs/core/project_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/query_constructor_api.py` & `hsfs-3.2.0rc5/hsfs/core/query_constructor_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/services_api.py` & `hsfs-3.2.0rc5/hsfs/core/services_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/statistics_api.py` & `hsfs-3.2.0rc5/hsfs/core/statistics_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/statistics_engine.py` & `hsfs-3.2.0rc5/hsfs/core/statistics_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/storage_connector_api.py` & `hsfs-3.2.0rc5/hsfs/core/storage_connector_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/tags_api.py` & `hsfs-3.2.0rc5/hsfs/core/tags_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/training_dataset_api.py` & `hsfs-3.2.0rc5/hsfs/core/training_dataset_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/training_dataset_engine.py` & `hsfs-3.2.0rc5/hsfs/core/training_dataset_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/training_dataset_job_conf.py` & `hsfs-3.2.0rc5/hsfs/core/training_dataset_job_conf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/transformation_function_api.py` & `hsfs-3.2.0rc5/hsfs/core/transformation_function_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/transformation_function_engine.py` & `hsfs-3.2.0rc5/hsfs/core/transformation_function_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/validation_report_api.py` & `hsfs-3.2.0rc5/hsfs/core/validation_report_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/validation_report_engine.py` & `hsfs-3.2.0rc5/hsfs/core/validation_report_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/validation_result_api.py` & `hsfs-3.2.0rc5/hsfs/core/validation_result_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/validation_result_engine.py` & `hsfs-3.2.0rc5/hsfs/core/validation_result_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/variable_api.py` & `hsfs-3.2.0rc5/hsfs/core/variable_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/core/vector_server.py` & `hsfs-3.2.0rc5/hsfs/core/vector_server.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/decorators.py` & `hsfs-3.2.0rc5/hsfs/decorators.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/engine/__init__.py` & `hsfs-3.2.0rc5/hsfs/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/engine/python.py` & `hsfs-3.2.0rc5/hsfs/engine/python.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/engine/spark.py` & `hsfs-3.2.0rc5/hsfs/engine/spark.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/expectation_suite.py` & `hsfs-3.2.0rc5/hsfs/expectation_suite.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/feature.py` & `hsfs-3.2.0rc5/hsfs/feature.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/feature_group.py` & `hsfs-3.2.0rc5/hsfs/feature_group.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/feature_group_commit.py` & `hsfs-3.2.0rc5/hsfs/feature_group_commit.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/feature_group_writer.py` & `hsfs-3.2.0rc5/hsfs/feature_group_writer.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/feature_store.py` & `hsfs-3.2.0rc5/hsfs/feature_store.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/feature_view.py` & `hsfs-3.2.0rc5/hsfs/feature_view.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/ge_expectation.py` & `hsfs-3.2.0rc5/hsfs/ge_expectation.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/ge_validation_result.py` & `hsfs-3.2.0rc5/hsfs/ge_validation_result.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/split_statistics.py` & `hsfs-3.2.0rc5/hsfs/split_statistics.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/statistics.py` & `hsfs-3.2.0rc5/hsfs/statistics.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/statistics_config.py` & `hsfs-3.2.0rc5/hsfs/statistics_config.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/storage_connector.py` & `hsfs-3.2.0rc5/hsfs/storage_connector.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/tag.py` & `hsfs-3.2.0rc5/hsfs/tag.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/training_dataset.py` & `hsfs-3.2.0rc5/hsfs/training_dataset.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/training_dataset_feature.py` & `hsfs-3.2.0rc5/hsfs/training_dataset_feature.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/training_dataset_split.py` & `hsfs-3.2.0rc5/hsfs/training_dataset_split.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/transformation_function.py` & `hsfs-3.2.0rc5/hsfs/transformation_function.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/transformation_function_attached.py` & `hsfs-3.2.0rc5/hsfs/transformation_function_attached.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/user.py` & `hsfs-3.2.0rc5/hsfs/user.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/util.py` & `hsfs-3.2.0rc5/hsfs/util.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/validation_report.py` & `hsfs-3.2.0rc5/hsfs/validation_report.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs/version.py` & `hsfs-3.2.0rc5/hsfs/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-__version__ = "3.2.0rc4"
+__version__ = "3.2.0rc5"
```

### Comparing `hsfs-3.2.0rc4/hsfs.egg-info/PKG-INFO` & `hsfs-3.2.0rc5/hsfs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsfs
-Version: 3.2.0rc4
+Version: 3.2.0rc5
 Summary: HSFS: An environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api
 Author: Hopsworks AB
 Author-email: moritz@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc4
+Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc5
 Description: # Hopsworks Feature Store
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hsfs Version: 3.2.0rc4 Summary: HSFS: An
+Metadata-Version: 2.1 Name: hsfs Version: 3.2.0rc5 Summary: HSFS: An
 environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api Author: Hopsworks
 AB Author-email: moritz@logicalclocks.com License: Apache License 2.0 Download-
-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc4
+URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc5
 Description: # Hopsworks Feature Store
   [Hopsworks_Community] [Hopsworks_Feature_Store_Documentation] [PyPiStatus]
            [Scala/Java_Artifacts] [Downloads] [CodeStyle] [License]
 HSFS is the library to interact with the Hopsworks Feature Store. The library
 makes creating new features, feature groups and training datasets easy. The
 library is environment independent and can be used in two modes: - Spark mode:
 For data engineering jobs that create and write features into the feature store
```

### Comparing `hsfs-3.2.0rc4/hsfs.egg-info/SOURCES.txt` & `hsfs-3.2.0rc5/hsfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc4/hsfs.egg-info/requires.txt` & `hsfs-3.2.0rc5/hsfs.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 PyMySQL[rsa]
 avro==1.11.0
 boto3
 furl
-great_expectations==0.14.12
+great_expectations==0.14.13
 markupsafe<2.1.0
 mock
 numpy
 pandas<2.0.0,>=1.2.0
 pyhumps==1.6.1
 pyjks
 requests
```

### Comparing `hsfs-3.2.0rc4/setup.py` & `hsfs-3.2.0rc5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         "pandas>=1.2.0,<2.0.0",
         "numpy",
         "pyjks",
         "mock",
         "avro==1.11.0",
         "sqlalchemy",
         "PyMySQL[rsa]",
-        "great_expectations==0.14.12",
+        "great_expectations==0.14.13",
         "markupsafe<2.1.0",  # GE issue 1: jinja2==2.11.3, pulls in markupsafe 2.1.0 which is not compatible with jinja2==2.11.3.
         "tzlocal",
     ],
     extras_require={
         "dev": [
             "pytest==7.1.2",
             "pytest-mock==3.8.2",
```

