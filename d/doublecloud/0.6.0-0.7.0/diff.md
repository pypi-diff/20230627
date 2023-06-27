# Comparing `tmp/doublecloud-0.6.0.tar.gz` & `tmp/doublecloud-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doublecloud-0.6.0.tar", last modified: Tue Jun 13 09:30:46 2023, max compression
+gzip compressed data, was "doublecloud-0.7.0.tar", last modified: Tue Jun 27 12:39:30 2023, max compression
```

## Comparing `doublecloud-0.6.0.tar` & `doublecloud-0.7.0.tar`

### file list

```diff
@@ -1,222 +1,225 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.797770 doublecloud-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 09:30:13.000000 doublecloud-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-13 09:30:46.797770 doublecloud-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-13 09:30:13.000000 doublecloud-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.781770 doublecloud-0.6.0/doublecloud/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_auth_fabric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_auth_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_backoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_operation_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_retry_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.781770 doublecloud-0.6.0/doublecloud/_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.781770 doublecloud-0.6.0/doublecloud/_wrappers/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_wrappers/clickhouse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.781770 doublecloud-0.6.0/doublecloud/_wrappers/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_wrappers/kafka/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.781770 doublecloud-0.6.0/doublecloud/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.781770 doublecloud-0.6.0/doublecloud/clickhouse/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24545 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17915 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/operation_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/operation_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/version_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/version_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/version_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/version_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/version_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/version_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.781770 doublecloud-0.6.0/doublecloud/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.785770 doublecloud-0.6.0/doublecloud/kafka/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/cluster_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/cluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/cluster_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/cluster_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/cluster_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20537 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/cluster_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/connector_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14894 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/connector_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/connector_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/connector_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/connector_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/connector_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/operation_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/operation_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/topic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/topic_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/topic_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/topic_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/topic_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/topic_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/user_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/user_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/user_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/user_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/version_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/version_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/version_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/version_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/version_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/version_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.785770 doublecloud-0.6.0/doublecloud/network/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.789770 doublecloud-0.6.0/doublecloud/network/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_connection_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_connection_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_connection_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_connection_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_connection_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_connection_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/operation_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/operation_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.789770 doublecloud-0.6.0/doublecloud/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.789770 doublecloud-0.6.0/doublecloud/transfer/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.793770 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.793770 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    24164 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/kafka_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/kafka_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/kafka_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/mongo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/mongo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/mongo_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/mysql_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/mysql_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/mysql_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/parsers_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/parsers_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/parsers_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/postgres_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/postgres_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/postgres_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/operation_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/operation_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/transfer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/transfer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/transfer_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/transfer_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/transfer_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19365 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/transfer_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.797770 doublecloud-0.6.0/doublecloud/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/cluster_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/cluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/cluster_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/maintenance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/maintenance_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/maintenance_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/operation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/operation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/operation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/paging_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/paging_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/paging_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.797770 doublecloud-0.6.0/doublecloud/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.797770 doublecloud-0.6.0/doublecloud/visualization/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/visualization/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/visualization/v1/workbook_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/visualization/v1/workbook_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/visualization/v1/workbook_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/visualization/v1/workbook_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/visualization/v1/workbook_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/visualization/v1/workbook_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.781770 doublecloud-0.6.0/doublecloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-13 09:30:46.000000 doublecloud-0.6.0/doublecloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-06-13 09:30:46.000000 doublecloud-0.6.0/doublecloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:30:46.000000 doublecloud-0.6.0/doublecloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:30:46.000000 doublecloud-0.6.0/doublecloud.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 09:30:46.000000 doublecloud-0.6.0/doublecloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 09:30:46.000000 doublecloud-0.6.0/doublecloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 09:30:13.000000 doublecloud-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:30:46.797770 doublecloud-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-13 09:30:42.000000 doublecloud-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.215382 doublecloud-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 12:38:54.000000 doublecloud-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-27 12:39:30.215382 doublecloud-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-27 12:38:54.000000 doublecloud-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.175380 doublecloud-0.7.0/doublecloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_auth_fabric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_auth_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_backoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_operation_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_retry_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.179380 doublecloud-0.7.0/doublecloud/_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.179380 doublecloud-0.7.0/doublecloud/_wrappers/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_wrappers/clickhouse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.179380 doublecloud-0.7.0/doublecloud/_wrappers/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_wrappers/kafka/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.179380 doublecloud-0.7.0/doublecloud/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.183380 doublecloud-0.7.0/doublecloud/clickhouse/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24545 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16265 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27580 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/operation_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/operation_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/version_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/version_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/version_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/version_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/version_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/version_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.183380 doublecloud-0.7.0/doublecloud/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.191381 doublecloud-0.7.0/doublecloud/kafka/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/cluster_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/cluster_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/cluster_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20537 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/cluster_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/connector_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14894 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/connector_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/connector_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/connector_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/connector_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/connector_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/operation_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/operation_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/topic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/topic_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/topic_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/topic_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/topic_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/topic_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/user_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/user_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/user_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/version_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/version_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/version_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/version_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/version_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/version_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.191381 doublecloud-0.7.0/doublecloud/network/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.191381 doublecloud-0.7.0/doublecloud/network/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_connection_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_connection_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_connection_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_connection_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_connection_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_connection_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/operation_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/operation_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.191381 doublecloud-0.7.0/doublecloud/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.195381 doublecloud-0.7.0/doublecloud/transfer/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.199381 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.207381 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24164 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/kafka_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/kafka_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/kafka_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mongo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mongo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mongo_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mysql_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mysql_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mysql_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/parsers_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/parsers_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/parsers_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/postgres_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/postgres_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/postgres_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/serializers_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/serializers_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/serializers_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/operation_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/operation_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/transfer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/transfer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/transfer_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/transfer_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/transfer_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19365 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/transfer_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.207381 doublecloud-0.7.0/doublecloud/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/cluster_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/maintenance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/maintenance_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/maintenance_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/operation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/operation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/operation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/paging_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/paging_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/paging_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.207381 doublecloud-0.7.0/doublecloud/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.215382 doublecloud-0.7.0/doublecloud/visualization/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/visualization/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/visualization/v1/workbook_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/visualization/v1/workbook_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/visualization/v1/workbook_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/visualization/v1/workbook_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/visualization/v1/workbook_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/visualization/v1/workbook_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.179380 doublecloud-0.7.0/doublecloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-27 12:39:30.000000 doublecloud-0.7.0/doublecloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-06-27 12:39:30.000000 doublecloud-0.7.0/doublecloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:39:30.000000 doublecloud-0.7.0/doublecloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:39:30.000000 doublecloud-0.7.0/doublecloud.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-27 12:39:30.000000 doublecloud-0.7.0/doublecloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 12:39:30.000000 doublecloud-0.7.0/doublecloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-27 12:38:54.000000 doublecloud-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 12:39:30.215382 doublecloud-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-27 12:39:25.000000 doublecloud-0.7.0/setup.py
```

### Comparing `doublecloud-0.6.0/LICENSE` & `doublecloud-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/PKG-INFO` & `doublecloud-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doublecloud
-Version: 0.6.0
+Version: 0.7.0
 Summary: The Double.Cloud official SDK
 Home-page: https://github.com/doublecloud/python-sdk
 Author: DoubleCloud GmbH
 Author-email: support@double.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doublecloud-0.6.0/README.md` & `doublecloud-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/_auth_fabric.py` & `doublecloud-0.7.0/doublecloud/_auth_fabric.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/_auth_plugin.py` & `doublecloud-0.7.0/doublecloud/_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/_backoff.py` & `doublecloud-0.7.0/doublecloud/_backoff.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/_channels.py` & `doublecloud-0.7.0/doublecloud/_channels.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/_operation_waiter.py` & `doublecloud-0.7.0/doublecloud/_operation_waiter.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/_retry_interceptor.py` & `doublecloud-0.7.0/doublecloud/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/_sdk.py` & `doublecloud-0.7.0/doublecloud/_sdk.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_pb2.py` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_pb2.pyi` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_service_pb2.py` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_service_pb2.pyi` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_service_pb2_grpc.py` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_pb2.py` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_pb2.pyi` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_service_pb2.py` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_service_pb2.pyi` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_service_pb2_grpc.py` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/config_pb2.py` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/config_pb2.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,49 +11,49 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&doublecloud/clickhouse/v1/config.proto\x12\x19\x64oublecloud.clickhouse.v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xdc,\n\x10\x43lickhouseConfig\x12Q\n\tlog_level\x18\x01 \x01(\x0e\x32\x34.doublecloud.clickhouse.v1.ClickhouseConfig.LogLevelR\x08logLevel\x12\x44\n\x0fmax_connections\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0emaxConnections\x12Q\n\x16max_concurrent_queries\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x14maxConcurrentQueries\x12G\n\x12keep_alive_timeout\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10keepAliveTimeout\x12S\n\x17uncompressed_cache_size\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x15uncompressedCacheSize\x12\x43\n\x0fmark_cache_size\x18\x06 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\rmarkCacheSize\x12O\n\x16max_table_size_to_drop\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12maxTableSizeToDrop\x12W\n\x1amax_partition_size_to_drop\x18\x08 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x16maxPartitionSizeToDrop\x12\x38\n\x08timezone\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08timezone\x12M\n\x14\x62\x61\x63kground_pool_size\x18\n \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12\x62\x61\x63kgroundPoolSize\x12^\n\x1d\x62\x61\x63kground_schedule_pool_size\x18\x0b \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1a\x62\x61\x63kgroundSchedulePoolSize\x12\\\n\x1c\x62\x61\x63kground_fetches_pool_size\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x19\x62\x61\x63kgroundFetchesPoolSize\x12V\n\x19\x62\x61\x63kground_move_pool_size\x18\r \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x16\x62\x61\x63kgroundMovePoolSize\x12Z\n\x1b\x62\x61\x63kground_common_pool_size\x18\x0e \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x18\x62\x61\x63kgroundCommonPoolSize\x12}\n-background_merges_mutations_concurrency_ratio\x18\x0f \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR)backgroundMergesMutationsConcurrencyRatio\x12X\n\x1atotal_memory_profiler_step\x18\x10 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x17totalMemoryProfilerStep\x12r\n\'total_memory_tracker_sample_probability\x18\x17 \x01(\x0b\x32\x1c.google.protobuf.DoubleValueR#totalMemoryTrackerSampleProbability\x12T\n\nmerge_tree\x18\x11 \x01(\x0b\x32\x35.doublecloud.clickhouse.v1.ClickhouseConfig.MergeTreeR\tmergeTree\x12Y\n\x0b\x63ompression\x18\x12 \x03(\x0b\x32\x37.doublecloud.clickhouse.v1.ClickhouseConfig.CompressionR\x0b\x63ompression\x12h\n\x0fgraphite_rollup\x18\x13 \x03(\x0b\x32?.doublecloud.clickhouse.v1.ClickhouseConfig.GraphiteRollupEntryR\x0egraphiteRollup\x12G\n\x05kafka\x18\x14 \x01(\x0b\x32\x31.doublecloud.clickhouse.v1.ClickhouseConfig.KafkaR\x05kafka\x12_\n\x0ckafka_topics\x18\x15 \x03(\x0b\x32<.doublecloud.clickhouse.v1.ClickhouseConfig.KafkaTopicsEntryR\x0bkafkaTopics\x12P\n\x08rabbitmq\x18\x16 \x01(\x0b\x32\x34.doublecloud.clickhouse.v1.ClickhouseConfig.RabbitmqR\x08rabbitmq\x1a\xab\x0c\n\tMergeTree\x12\x63\n\x1freplicated_deduplication_window\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1dreplicatedDeduplicationWindow\x12p\n\'replicated_deduplication_window_seconds\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR$replicatedDeduplicationWindowSeconds\x12N\n\x15parts_to_delay_insert\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12partsToDelayInsert\x12N\n\x15parts_to_throw_insert\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12partsToThrowInsert\x12_\n\x1einactive_parts_to_delay_insert\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1ainactivePartsToDelayInsert\x12_\n\x1einactive_parts_to_throw_insert\x18\r \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1ainactivePartsToThrowInsert\x12_\n\x1emax_replicated_merges_in_queue\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1amaxReplicatedMergesInQueue\x12\x8e\x01\n9number_of_free_entries_in_pool_to_lower_max_size_of_merge\x18\x06 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR.numberOfFreeEntriesInPoolToLowerMaxSizeOfMerge\x12m\n\'max_bytes_to_merge_at_min_space_in_pool\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1fmaxBytesToMergeAtMinSpaceInPool\x12m\n\'max_bytes_to_merge_at_max_space_in_pool\x18\x08 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1fmaxBytesToMergeAtMaxSpaceInPool\x12Q\n\x17min_bytes_for_wide_part\x18\t \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x13minBytesForWidePart\x12O\n\x16min_rows_for_wide_part\x18\n \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12minRowsForWidePart\x12I\n\x13ttl_only_drop_parts\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x10ttlOnlyDropParts\x12N\n\x16merge_with_ttl_timeout\x18\x0f \x01(\x0b\x32\x19.google.protobuf.DurationR\x13mergeWithTtlTimeout\x12i\n$merge_with_recompression_ttl_timeout\x18\x10 \x01(\x0b\x32\x19.google.protobuf.DurationR mergeWithRecompressionTtlTimeout\x12k\n%allow_remote_fs_zero_copy_replication\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.BoolValueR allowRemoteFsZeroCopyReplication\x1a\xae\x06\n\x05Kafka\x12o\n\x11security_protocol\x18\x01 \x01(\x0e\x32\x42.doublecloud.clickhouse.v1.ClickhouseConfig.Kafka.SecurityProtocolR\x10securityProtocol\x12\x66\n\x0esasl_mechanism\x18\x02 \x01(\x0e\x32?.doublecloud.clickhouse.v1.ClickhouseConfig.Kafka.SaslMechanismR\rsaslMechanism\x12\x41\n\rsasl_username\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0csaslUsername\x12\x41\n\rsasl_password\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0csaslPassword\x12i\n#enable_ssl_certificate_verification\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR enableSslCertificateVerification\"\xb3\x01\n\x10SecurityProtocol\x12\x1d\n\x19SECURITY_PROTOCOL_INVALID\x10\x00\x12\x1f\n\x1bSECURITY_PROTOCOL_PLAINTEXT\x10\x01\x12\x19\n\x15SECURITY_PROTOCOL_SSL\x10\x02\x12$\n SECURITY_PROTOCOL_SASL_PLAINTEXT\x10\x03\x12\x1e\n\x1aSECURITY_PROTOCOL_SASL_SSL\x10\x04\"\xa4\x01\n\rSaslMechanism\x12\x1a\n\x16SASL_MECHANISM_INVALID\x10\x00\x12\x19\n\x15SASL_MECHANISM_GSSAPI\x10\x01\x12\x18\n\x14SASL_MECHANISM_PLAIN\x10\x02\x12 \n\x1cSASL_MECHANISM_SCRAM_SHA_256\x10\x03\x12 \n\x1cSASL_MECHANISM_SCRAM_SHA_512\x10\x04\x1a\xb2\x01\n\x08Rabbitmq\x12\x38\n\x08username\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08username\x12\x38\n\x08password\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08password\x12\x32\n\x05vhost\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x05vhost\x1a\xbc\x02\n\x0b\x43ompression\x12V\n\x06method\x18\x01 \x01(\x0e\x32>.doublecloud.clickhouse.v1.ClickhouseConfig.Compression.MethodR\x06method\x12\"\n\rmin_part_size\x18\x02 \x01(\x03R\x0bminPartSize\x12-\n\x13min_part_size_ratio\x18\x03 \x01(\x01R\x10minPartSizeRatio\x12\x31\n\x05level\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x05level\"O\n\x06Method\x12\x12\n\x0eMETHOD_INVALID\x10\x00\x12\x0e\n\nMETHOD_LZ4\x10\x01\x12\x0f\n\x0bMETHOD_ZSTD\x10\x02\x12\x10\n\x0cMETHOD_LZ4HC\x10\x03\x1a\x95\x03\n\x0eGraphiteRollup\x12^\n\x08patterns\x18\x01 \x03(\x0b\x32\x42.doublecloud.clickhouse.v1.ClickhouseConfig.GraphiteRollup.PatternR\x08patterns\x1a\xa2\x02\n\x07Pattern\x12\x34\n\x06regexp\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x06regexp\x12\x38\n\x08\x66unction\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08\x66unction\x12j\n\tretention\x18\x03 \x03(\x0b\x32L.doublecloud.clickhouse.v1.ClickhouseConfig.GraphiteRollup.Pattern.RetentionR\tretention\x1a;\n\tRetention\x12\x10\n\x03\x61ge\x18\x01 \x01(\x03R\x03\x61ge\x12\x1c\n\tprecision\x18\x02 \x01(\x03R\tprecision\x1a}\n\x13GraphiteRollupEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12P\n\x05value\x18\x02 \x01(\x0b\x32:.doublecloud.clickhouse.v1.ClickhouseConfig.GraphiteRollupR\x05value:\x02\x38\x01\x1aq\n\x10KafkaTopicsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12G\n\x05value\x18\x02 \x01(\x0b\x32\x31.doublecloud.clickhouse.v1.ClickhouseConfig.KafkaR\x05value:\x02\x38\x01\"\x92\x01\n\x08LogLevel\x12\x15\n\x11LOG_LEVEL_INVALID\x10\x00\x12\x13\n\x0fLOG_LEVEL_TRACE\x10\x01\x12\x13\n\x0fLOG_LEVEL_DEBUG\x10\x02\x12\x19\n\x15LOG_LEVEL_INFORMATION\x10\x03\x12\x15\n\x11LOG_LEVEL_WARNING\x10\x04\x12\x13\n\x0fLOG_LEVEL_ERROR\x10\x05\x42IZGgithub.com/doublecloud/go-genproto/doublecloud/clickhouse/v1;clickhouseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&doublecloud/clickhouse/v1/config.proto\x12\x19\x64oublecloud.clickhouse.v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xdaI\n\x10\x43lickhouseConfig\x12Q\n\tlog_level\x18\x01 \x01(\x0e\x32\x34.doublecloud.clickhouse.v1.ClickhouseConfig.LogLevelR\x08logLevel\x12\x44\n\x0fmax_connections\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0emaxConnections\x12Q\n\x16max_concurrent_queries\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x14maxConcurrentQueries\x12G\n\x12keep_alive_timeout\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10keepAliveTimeout\x12S\n\x17uncompressed_cache_size\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x15uncompressedCacheSize\x12\x43\n\x0fmark_cache_size\x18\x06 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\rmarkCacheSize\x12O\n\x16max_table_size_to_drop\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12maxTableSizeToDrop\x12W\n\x1amax_partition_size_to_drop\x18\x08 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x16maxPartitionSizeToDrop\x12\x38\n\x08timezone\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08timezone\x12M\n\x14\x62\x61\x63kground_pool_size\x18\n \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12\x62\x61\x63kgroundPoolSize\x12^\n\x1d\x62\x61\x63kground_schedule_pool_size\x18\x0b \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1a\x62\x61\x63kgroundSchedulePoolSize\x12\\\n\x1c\x62\x61\x63kground_fetches_pool_size\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x19\x62\x61\x63kgroundFetchesPoolSize\x12V\n\x19\x62\x61\x63kground_move_pool_size\x18\r \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x16\x62\x61\x63kgroundMovePoolSize\x12Z\n\x1b\x62\x61\x63kground_common_pool_size\x18\x0e \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x18\x62\x61\x63kgroundCommonPoolSize\x12}\n-background_merges_mutations_concurrency_ratio\x18\x0f \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR)backgroundMergesMutationsConcurrencyRatio\x12X\n\x1atotal_memory_profiler_step\x18\x10 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x17totalMemoryProfilerStep\x12r\n\'total_memory_tracker_sample_probability\x18\x17 \x01(\x0b\x32\x1c.google.protobuf.DoubleValueR#totalMemoryTrackerSampleProbability\x12z\n,background_message_broker_schedule_pool_size\x18\x18 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\'backgroundMessageBrokerSchedulePoolSize\x12T\n\nmerge_tree\x18\x11 \x01(\x0b\x32\x35.doublecloud.clickhouse.v1.ClickhouseConfig.MergeTreeR\tmergeTree\x12Y\n\x0b\x63ompression\x18\x12 \x03(\x0b\x32\x37.doublecloud.clickhouse.v1.ClickhouseConfig.CompressionR\x0b\x63ompression\x12h\n\x0fgraphite_rollup\x18\x13 \x03(\x0b\x32?.doublecloud.clickhouse.v1.ClickhouseConfig.GraphiteRollupEntryR\x0egraphiteRollup\x12G\n\x05kafka\x18\x14 \x01(\x0b\x32\x31.doublecloud.clickhouse.v1.ClickhouseConfig.KafkaR\x05kafka\x12_\n\x0ckafka_topics\x18\x15 \x03(\x0b\x32<.doublecloud.clickhouse.v1.ClickhouseConfig.KafkaTopicsEntryR\x0bkafkaTopics\x12P\n\x08rabbitmq\x18\x16 \x01(\x0b\x32\x34.doublecloud.clickhouse.v1.ClickhouseConfig.RabbitmqR\x08rabbitmq\x12T\n\x18query_log_retention_size\x18\x19 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x15queryLogRetentionSize\x12R\n\x18query_log_retention_time\x18\x1a \x01(\x0b\x32\x19.google.protobuf.DurationR\x15queryLogRetentionTime\x12S\n\x18query_thread_log_enabled\x18\x1b \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x15queryThreadLogEnabled\x12\x61\n\x1fquery_thread_log_retention_size\x18\x1c \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1bqueryThreadLogRetentionSize\x12_\n\x1fquery_thread_log_retention_time\x18\x1d \x01(\x0b\x32\x19.google.protobuf.DurationR\x1bqueryThreadLogRetentionTime\x12Q\n\x17query_views_log_enabled\x18\x1e \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x14queryViewsLogEnabled\x12_\n\x1equery_views_log_retention_size\x18\x1f \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1aqueryViewsLogRetentionSize\x12]\n\x1equery_views_log_retention_time\x18  \x01(\x0b\x32\x19.google.protobuf.DurationR\x1aqueryViewsLogRetentionTime\x12R\n\x17part_log_retention_size\x18! \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x14partLogRetentionSize\x12P\n\x17part_log_retention_time\x18\" \x01(\x0b\x32\x19.google.protobuf.DurationR\x14partLogRetentionTime\x12H\n\x12metric_log_enabled\x18# \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x10metricLogEnabled\x12V\n\x19metric_log_retention_size\x18$ \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x16metricLogRetentionSize\x12T\n\x19metric_log_retention_time\x18% \x01(\x0b\x32\x19.google.protobuf.DurationR\x16metricLogRetentionTime\x12\x61\n\x1f\x61synchronous_metric_log_enabled\x18& \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x1c\x61synchronousMetricLogEnabled\x12o\n&asynchronous_metric_log_retention_size\x18\' \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\"asynchronousMetricLogRetentionSize\x12m\n&asynchronous_metric_log_retention_time\x18( \x01(\x0b\x32\x19.google.protobuf.DurationR\"asynchronousMetricLogRetentionTime\x12\x46\n\x11trace_log_enabled\x18) \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x0ftraceLogEnabled\x12T\n\x18trace_log_retention_size\x18* \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x15traceLogRetentionSize\x12R\n\x18trace_log_retention_time\x18+ \x01(\x0b\x32\x19.google.protobuf.DurationR\x15traceLogRetentionTime\x12\x44\n\x10text_log_enabled\x18, \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x0etextLogEnabled\x12R\n\x17text_log_retention_size\x18- \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x14textLogRetentionSize\x12P\n\x17text_log_retention_time\x18. \x01(\x0b\x32\x19.google.protobuf.DurationR\x14textLogRetentionTime\x12Z\n\x0etext_log_level\x18/ \x01(\x0e\x32\x34.doublecloud.clickhouse.v1.ClickhouseConfig.LogLevelR\x0ctextLogLevel\x12_\n\x1eopentelemetry_span_log_enabled\x18\x30 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x1bopentelemetrySpanLogEnabled\x12m\n%opentelemetry_span_log_retention_size\x18\x31 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR!opentelemetrySpanLogRetentionSize\x12k\n%opentelemetry_span_log_retention_time\x18\x32 \x01(\x0b\x32\x19.google.protobuf.DurationR!opentelemetrySpanLogRetentionTime\x12J\n\x13session_log_enabled\x18\x33 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x11sessionLogEnabled\x12X\n\x1asession_log_retention_size\x18\x34 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x17sessionLogRetentionSize\x12V\n\x1asession_log_retention_time\x18\x35 \x01(\x0b\x32\x19.google.protobuf.DurationR\x17sessionLogRetentionTime\x12N\n\x15zookeeper_log_enabled\x18\x36 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x13zookeeperLogEnabled\x12\\\n\x1czookeeper_log_retention_size\x18\x37 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x19zookeeperLogRetentionSize\x12Z\n\x1czookeeper_log_retention_time\x18\x38 \x01(\x0b\x32\x19.google.protobuf.DurationR\x19zookeeperLogRetentionTime\x12\x61\n\x1f\x61synchronous_insert_log_enabled\x18\x39 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x1c\x61synchronousInsertLogEnabled\x12o\n&asynchronous_insert_log_retention_size\x18: \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\"asynchronousInsertLogRetentionSize\x12m\n&asynchronous_insert_log_retention_time\x18; \x01(\x0b\x32\x19.google.protobuf.DurationR\"asynchronousInsertLogRetentionTime\x1a\xb4\x0f\n\tMergeTree\x12\x63\n\x1freplicated_deduplication_window\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1dreplicatedDeduplicationWindow\x12p\n\'replicated_deduplication_window_seconds\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR$replicatedDeduplicationWindowSeconds\x12N\n\x15parts_to_delay_insert\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12partsToDelayInsert\x12N\n\x15parts_to_throw_insert\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12partsToThrowInsert\x12_\n\x1einactive_parts_to_delay_insert\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1ainactivePartsToDelayInsert\x12_\n\x1einactive_parts_to_throw_insert\x18\r \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1ainactivePartsToThrowInsert\x12_\n\x1emax_replicated_merges_in_queue\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1amaxReplicatedMergesInQueue\x12\x8e\x01\n9number_of_free_entries_in_pool_to_lower_max_size_of_merge\x18\x06 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR.numberOfFreeEntriesInPoolToLowerMaxSizeOfMerge\x12m\n\'max_bytes_to_merge_at_min_space_in_pool\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1fmaxBytesToMergeAtMinSpaceInPool\x12m\n\'max_bytes_to_merge_at_max_space_in_pool\x18\x08 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1fmaxBytesToMergeAtMaxSpaceInPool\x12Q\n\x17min_bytes_for_wide_part\x18\t \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x13minBytesForWidePart\x12O\n\x16min_rows_for_wide_part\x18\n \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12minRowsForWidePart\x12I\n\x13ttl_only_drop_parts\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x10ttlOnlyDropParts\x12k\n%allow_remote_fs_zero_copy_replication\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.BoolValueR allowRemoteFsZeroCopyReplication\x12N\n\x16merge_with_ttl_timeout\x18\x0f \x01(\x0b\x32\x19.google.protobuf.DurationR\x13mergeWithTtlTimeout\x12i\n$merge_with_recompression_ttl_timeout\x18\x10 \x01(\x0b\x32\x19.google.protobuf.DurationR mergeWithRecompressionTtlTimeout\x12H\n\x12max_parts_in_total\x18\x11 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0fmaxPartsInTotal\x12j\n%max_number_of_merges_with_ttl_in_pool\x18\x12 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1emaxNumberOfMergesWithTtlInPool\x12K\n\x14\x63leanup_delay_period\x18\x13 \x01(\x0b\x32\x19.google.protobuf.DurationR\x12\x63leanupDelayPeriod\x12\x83\x01\n2number_of_free_entries_in_pool_to_execute_mutation\x18\x14 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR*numberOfFreeEntriesInPoolToExecuteMutation\x1a\xae\x06\n\x05Kafka\x12o\n\x11security_protocol\x18\x01 \x01(\x0e\x32\x42.doublecloud.clickhouse.v1.ClickhouseConfig.Kafka.SecurityProtocolR\x10securityProtocol\x12\x66\n\x0esasl_mechanism\x18\x02 \x01(\x0e\x32?.doublecloud.clickhouse.v1.ClickhouseConfig.Kafka.SaslMechanismR\rsaslMechanism\x12\x41\n\rsasl_username\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0csaslUsername\x12\x41\n\rsasl_password\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0csaslPassword\x12i\n#enable_ssl_certificate_verification\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR enableSslCertificateVerification\"\xb3\x01\n\x10SecurityProtocol\x12\x1d\n\x19SECURITY_PROTOCOL_INVALID\x10\x00\x12\x1f\n\x1bSECURITY_PROTOCOL_PLAINTEXT\x10\x01\x12\x19\n\x15SECURITY_PROTOCOL_SSL\x10\x02\x12$\n SECURITY_PROTOCOL_SASL_PLAINTEXT\x10\x03\x12\x1e\n\x1aSECURITY_PROTOCOL_SASL_SSL\x10\x04\"\xa4\x01\n\rSaslMechanism\x12\x1a\n\x16SASL_MECHANISM_INVALID\x10\x00\x12\x19\n\x15SASL_MECHANISM_GSSAPI\x10\x01\x12\x18\n\x14SASL_MECHANISM_PLAIN\x10\x02\x12 \n\x1cSASL_MECHANISM_SCRAM_SHA_256\x10\x03\x12 \n\x1cSASL_MECHANISM_SCRAM_SHA_512\x10\x04\x1a\xb2\x01\n\x08Rabbitmq\x12\x38\n\x08username\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08username\x12\x38\n\x08password\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08password\x12\x32\n\x05vhost\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x05vhost\x1a\xbc\x02\n\x0b\x43ompression\x12V\n\x06method\x18\x01 \x01(\x0e\x32>.doublecloud.clickhouse.v1.ClickhouseConfig.Compression.MethodR\x06method\x12\"\n\rmin_part_size\x18\x02 \x01(\x03R\x0bminPartSize\x12-\n\x13min_part_size_ratio\x18\x03 \x01(\x01R\x10minPartSizeRatio\x12\x31\n\x05level\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x05level\"O\n\x06Method\x12\x12\n\x0eMETHOD_INVALID\x10\x00\x12\x0e\n\nMETHOD_LZ4\x10\x01\x12\x0f\n\x0bMETHOD_ZSTD\x10\x02\x12\x10\n\x0cMETHOD_LZ4HC\x10\x03\x1a\x95\x03\n\x0eGraphiteRollup\x12^\n\x08patterns\x18\x01 \x03(\x0b\x32\x42.doublecloud.clickhouse.v1.ClickhouseConfig.GraphiteRollup.PatternR\x08patterns\x1a\xa2\x02\n\x07Pattern\x12\x34\n\x06regexp\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x06regexp\x12\x38\n\x08\x66unction\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08\x66unction\x12j\n\tretention\x18\x03 \x03(\x0b\x32L.doublecloud.clickhouse.v1.ClickhouseConfig.GraphiteRollup.Pattern.RetentionR\tretention\x1a;\n\tRetention\x12\x10\n\x03\x61ge\x18\x01 \x01(\x03R\x03\x61ge\x12\x1c\n\tprecision\x18\x02 \x01(\x03R\tprecision\x1a}\n\x13GraphiteRollupEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12P\n\x05value\x18\x02 \x01(\x0b\x32:.doublecloud.clickhouse.v1.ClickhouseConfig.GraphiteRollupR\x05value:\x02\x38\x01\x1aq\n\x10KafkaTopicsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12G\n\x05value\x18\x02 \x01(\x0b\x32\x31.doublecloud.clickhouse.v1.ClickhouseConfig.KafkaR\x05value:\x02\x38\x01\"\x92\x01\n\x08LogLevel\x12\x15\n\x11LOG_LEVEL_INVALID\x10\x00\x12\x13\n\x0fLOG_LEVEL_TRACE\x10\x01\x12\x13\n\x0fLOG_LEVEL_DEBUG\x10\x02\x12\x19\n\x15LOG_LEVEL_INFORMATION\x10\x03\x12\x15\n\x11LOG_LEVEL_WARNING\x10\x04\x12\x13\n\x0fLOG_LEVEL_ERROR\x10\x05\x42IZGgithub.com/doublecloud/go-genproto/doublecloud/clickhouse/v1;clickhouseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.clickhouse.v1.config_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZGgithub.com/doublecloud/go-genproto/doublecloud/clickhouse/v1;clickhouse'
   _CLICKHOUSECONFIG_GRAPHITEROLLUPENTRY._options = None
   _CLICKHOUSECONFIG_GRAPHITEROLLUPENTRY._serialized_options = b'8\001'
   _CLICKHOUSECONFIG_KAFKATOPICSENTRY._options = None
   _CLICKHOUSECONFIG_KAFKATOPICSENTRY._serialized_options = b'8\001'
   _globals['_CLICKHOUSECONFIG']._serialized_start=134
-  _globals['_CLICKHOUSECONFIG']._serialized_end=5858
-  _globals['_CLICKHOUSECONFIG_MERGETREE']._serialized_start=2163
-  _globals['_CLICKHOUSECONFIG_MERGETREE']._serialized_end=3742
-  _globals['_CLICKHOUSECONFIG_KAFKA']._serialized_start=3745
-  _globals['_CLICKHOUSECONFIG_KAFKA']._serialized_end=4559
-  _globals['_CLICKHOUSECONFIG_KAFKA_SECURITYPROTOCOL']._serialized_start=4213
-  _globals['_CLICKHOUSECONFIG_KAFKA_SECURITYPROTOCOL']._serialized_end=4392
-  _globals['_CLICKHOUSECONFIG_KAFKA_SASLMECHANISM']._serialized_start=4395
-  _globals['_CLICKHOUSECONFIG_KAFKA_SASLMECHANISM']._serialized_end=4559
-  _globals['_CLICKHOUSECONFIG_RABBITMQ']._serialized_start=4562
-  _globals['_CLICKHOUSECONFIG_RABBITMQ']._serialized_end=4740
-  _globals['_CLICKHOUSECONFIG_COMPRESSION']._serialized_start=4743
-  _globals['_CLICKHOUSECONFIG_COMPRESSION']._serialized_end=5059
-  _globals['_CLICKHOUSECONFIG_COMPRESSION_METHOD']._serialized_start=4980
-  _globals['_CLICKHOUSECONFIG_COMPRESSION_METHOD']._serialized_end=5059
-  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP']._serialized_start=5062
-  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP']._serialized_end=5467
-  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP_PATTERN']._serialized_start=5177
-  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP_PATTERN']._serialized_end=5467
-  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP_PATTERN_RETENTION']._serialized_start=5408
-  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP_PATTERN_RETENTION']._serialized_end=5467
-  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUPENTRY']._serialized_start=5469
-  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUPENTRY']._serialized_end=5594
-  _globals['_CLICKHOUSECONFIG_KAFKATOPICSENTRY']._serialized_start=5596
-  _globals['_CLICKHOUSECONFIG_KAFKATOPICSENTRY']._serialized_end=5709
-  _globals['_CLICKHOUSECONFIG_LOGLEVEL']._serialized_start=5712
-  _globals['_CLICKHOUSECONFIG_LOGLEVEL']._serialized_end=5858
+  _globals['_CLICKHOUSECONFIG']._serialized_end=9568
+  _globals['_CLICKHOUSECONFIG_MERGETREE']._serialized_start=5480
+  _globals['_CLICKHOUSECONFIG_MERGETREE']._serialized_end=7452
+  _globals['_CLICKHOUSECONFIG_KAFKA']._serialized_start=7455
+  _globals['_CLICKHOUSECONFIG_KAFKA']._serialized_end=8269
+  _globals['_CLICKHOUSECONFIG_KAFKA_SECURITYPROTOCOL']._serialized_start=7923
+  _globals['_CLICKHOUSECONFIG_KAFKA_SECURITYPROTOCOL']._serialized_end=8102
+  _globals['_CLICKHOUSECONFIG_KAFKA_SASLMECHANISM']._serialized_start=8105
+  _globals['_CLICKHOUSECONFIG_KAFKA_SASLMECHANISM']._serialized_end=8269
+  _globals['_CLICKHOUSECONFIG_RABBITMQ']._serialized_start=8272
+  _globals['_CLICKHOUSECONFIG_RABBITMQ']._serialized_end=8450
+  _globals['_CLICKHOUSECONFIG_COMPRESSION']._serialized_start=8453
+  _globals['_CLICKHOUSECONFIG_COMPRESSION']._serialized_end=8769
+  _globals['_CLICKHOUSECONFIG_COMPRESSION_METHOD']._serialized_start=8690
+  _globals['_CLICKHOUSECONFIG_COMPRESSION_METHOD']._serialized_end=8769
+  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP']._serialized_start=8772
+  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP']._serialized_end=9177
+  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP_PATTERN']._serialized_start=8887
+  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP_PATTERN']._serialized_end=9177
+  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP_PATTERN_RETENTION']._serialized_start=9118
+  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP_PATTERN_RETENTION']._serialized_end=9177
+  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUPENTRY']._serialized_start=9179
+  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUPENTRY']._serialized_end=9304
+  _globals['_CLICKHOUSECONFIG_KAFKATOPICSENTRY']._serialized_start=9306
+  _globals['_CLICKHOUSECONFIG_KAFKATOPICSENTRY']._serialized_end=9419
+  _globals['_CLICKHOUSECONFIG_LOGLEVEL']._serialized_start=9422
+  _globals['_CLICKHOUSECONFIG_LOGLEVEL']._serialized_end=9568
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/config_pb2.pyi` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/config_pb2.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class ClickhouseConfig(_message.Message):
-    __slots__ = ["log_level", "max_connections", "max_concurrent_queries", "keep_alive_timeout", "uncompressed_cache_size", "mark_cache_size", "max_table_size_to_drop", "max_partition_size_to_drop", "timezone", "background_pool_size", "background_schedule_pool_size", "background_fetches_pool_size", "background_move_pool_size", "background_common_pool_size", "background_merges_mutations_concurrency_ratio", "total_memory_profiler_step", "total_memory_tracker_sample_probability", "merge_tree", "compression", "graphite_rollup", "kafka", "kafka_topics", "rabbitmq"]
+    __slots__ = ["log_level", "max_connections", "max_concurrent_queries", "keep_alive_timeout", "uncompressed_cache_size", "mark_cache_size", "max_table_size_to_drop", "max_partition_size_to_drop", "timezone", "background_pool_size", "background_schedule_pool_size", "background_fetches_pool_size", "background_move_pool_size", "background_common_pool_size", "background_merges_mutations_concurrency_ratio", "total_memory_profiler_step", "total_memory_tracker_sample_probability", "background_message_broker_schedule_pool_size", "merge_tree", "compression", "graphite_rollup", "kafka", "kafka_topics", "rabbitmq", "query_log_retention_size", "query_log_retention_time", "query_thread_log_enabled", "query_thread_log_retention_size", "query_thread_log_retention_time", "query_views_log_enabled", "query_views_log_retention_size", "query_views_log_retention_time", "part_log_retention_size", "part_log_retention_time", "metric_log_enabled", "metric_log_retention_size", "metric_log_retention_time", "asynchronous_metric_log_enabled", "asynchronous_metric_log_retention_size", "asynchronous_metric_log_retention_time", "trace_log_enabled", "trace_log_retention_size", "trace_log_retention_time", "text_log_enabled", "text_log_retention_size", "text_log_retention_time", "text_log_level", "opentelemetry_span_log_enabled", "opentelemetry_span_log_retention_size", "opentelemetry_span_log_retention_time", "session_log_enabled", "session_log_retention_size", "session_log_retention_time", "zookeeper_log_enabled", "zookeeper_log_retention_size", "zookeeper_log_retention_time", "asynchronous_insert_log_enabled", "asynchronous_insert_log_retention_size", "asynchronous_insert_log_retention_time"]
     class LogLevel(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
         LOG_LEVEL_INVALID: _ClassVar[ClickhouseConfig.LogLevel]
         LOG_LEVEL_TRACE: _ClassVar[ClickhouseConfig.LogLevel]
         LOG_LEVEL_DEBUG: _ClassVar[ClickhouseConfig.LogLevel]
         LOG_LEVEL_INFORMATION: _ClassVar[ClickhouseConfig.LogLevel]
         LOG_LEVEL_WARNING: _ClassVar[ClickhouseConfig.LogLevel]
@@ -21,48 +21,56 @@
     LOG_LEVEL_INVALID: ClickhouseConfig.LogLevel
     LOG_LEVEL_TRACE: ClickhouseConfig.LogLevel
     LOG_LEVEL_DEBUG: ClickhouseConfig.LogLevel
     LOG_LEVEL_INFORMATION: ClickhouseConfig.LogLevel
     LOG_LEVEL_WARNING: ClickhouseConfig.LogLevel
     LOG_LEVEL_ERROR: ClickhouseConfig.LogLevel
     class MergeTree(_message.Message):
-        __slots__ = ["replicated_deduplication_window", "replicated_deduplication_window_seconds", "parts_to_delay_insert", "parts_to_throw_insert", "inactive_parts_to_delay_insert", "inactive_parts_to_throw_insert", "max_replicated_merges_in_queue", "number_of_free_entries_in_pool_to_lower_max_size_of_merge", "max_bytes_to_merge_at_min_space_in_pool", "max_bytes_to_merge_at_max_space_in_pool", "min_bytes_for_wide_part", "min_rows_for_wide_part", "ttl_only_drop_parts", "merge_with_ttl_timeout", "merge_with_recompression_ttl_timeout", "allow_remote_fs_zero_copy_replication"]
+        __slots__ = ["replicated_deduplication_window", "replicated_deduplication_window_seconds", "parts_to_delay_insert", "parts_to_throw_insert", "inactive_parts_to_delay_insert", "inactive_parts_to_throw_insert", "max_replicated_merges_in_queue", "number_of_free_entries_in_pool_to_lower_max_size_of_merge", "max_bytes_to_merge_at_min_space_in_pool", "max_bytes_to_merge_at_max_space_in_pool", "min_bytes_for_wide_part", "min_rows_for_wide_part", "ttl_only_drop_parts", "allow_remote_fs_zero_copy_replication", "merge_with_ttl_timeout", "merge_with_recompression_ttl_timeout", "max_parts_in_total", "max_number_of_merges_with_ttl_in_pool", "cleanup_delay_period", "number_of_free_entries_in_pool_to_execute_mutation"]
         REPLICATED_DEDUPLICATION_WINDOW_FIELD_NUMBER: _ClassVar[int]
         REPLICATED_DEDUPLICATION_WINDOW_SECONDS_FIELD_NUMBER: _ClassVar[int]
         PARTS_TO_DELAY_INSERT_FIELD_NUMBER: _ClassVar[int]
         PARTS_TO_THROW_INSERT_FIELD_NUMBER: _ClassVar[int]
         INACTIVE_PARTS_TO_DELAY_INSERT_FIELD_NUMBER: _ClassVar[int]
         INACTIVE_PARTS_TO_THROW_INSERT_FIELD_NUMBER: _ClassVar[int]
         MAX_REPLICATED_MERGES_IN_QUEUE_FIELD_NUMBER: _ClassVar[int]
         NUMBER_OF_FREE_ENTRIES_IN_POOL_TO_LOWER_MAX_SIZE_OF_MERGE_FIELD_NUMBER: _ClassVar[int]
         MAX_BYTES_TO_MERGE_AT_MIN_SPACE_IN_POOL_FIELD_NUMBER: _ClassVar[int]
         MAX_BYTES_TO_MERGE_AT_MAX_SPACE_IN_POOL_FIELD_NUMBER: _ClassVar[int]
         MIN_BYTES_FOR_WIDE_PART_FIELD_NUMBER: _ClassVar[int]
         MIN_ROWS_FOR_WIDE_PART_FIELD_NUMBER: _ClassVar[int]
         TTL_ONLY_DROP_PARTS_FIELD_NUMBER: _ClassVar[int]
+        ALLOW_REMOTE_FS_ZERO_COPY_REPLICATION_FIELD_NUMBER: _ClassVar[int]
         MERGE_WITH_TTL_TIMEOUT_FIELD_NUMBER: _ClassVar[int]
         MERGE_WITH_RECOMPRESSION_TTL_TIMEOUT_FIELD_NUMBER: _ClassVar[int]
-        ALLOW_REMOTE_FS_ZERO_COPY_REPLICATION_FIELD_NUMBER: _ClassVar[int]
+        MAX_PARTS_IN_TOTAL_FIELD_NUMBER: _ClassVar[int]
+        MAX_NUMBER_OF_MERGES_WITH_TTL_IN_POOL_FIELD_NUMBER: _ClassVar[int]
+        CLEANUP_DELAY_PERIOD_FIELD_NUMBER: _ClassVar[int]
+        NUMBER_OF_FREE_ENTRIES_IN_POOL_TO_EXECUTE_MUTATION_FIELD_NUMBER: _ClassVar[int]
         replicated_deduplication_window: _wrappers_pb2.Int64Value
         replicated_deduplication_window_seconds: _duration_pb2.Duration
         parts_to_delay_insert: _wrappers_pb2.Int64Value
         parts_to_throw_insert: _wrappers_pb2.Int64Value
         inactive_parts_to_delay_insert: _wrappers_pb2.Int64Value
         inactive_parts_to_throw_insert: _wrappers_pb2.Int64Value
         max_replicated_merges_in_queue: _wrappers_pb2.Int64Value
         number_of_free_entries_in_pool_to_lower_max_size_of_merge: _wrappers_pb2.Int64Value
         max_bytes_to_merge_at_min_space_in_pool: _wrappers_pb2.Int64Value
         max_bytes_to_merge_at_max_space_in_pool: _wrappers_pb2.Int64Value
         min_bytes_for_wide_part: _wrappers_pb2.Int64Value
         min_rows_for_wide_part: _wrappers_pb2.Int64Value
         ttl_only_drop_parts: _wrappers_pb2.BoolValue
+        allow_remote_fs_zero_copy_replication: _wrappers_pb2.BoolValue
         merge_with_ttl_timeout: _duration_pb2.Duration
         merge_with_recompression_ttl_timeout: _duration_pb2.Duration
-        allow_remote_fs_zero_copy_replication: _wrappers_pb2.BoolValue
-        def __init__(self, replicated_deduplication_window: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., replicated_deduplication_window_seconds: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., parts_to_delay_insert: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., parts_to_throw_insert: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., inactive_parts_to_delay_insert: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., inactive_parts_to_throw_insert: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., max_replicated_merges_in_queue: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., number_of_free_entries_in_pool_to_lower_max_size_of_merge: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., max_bytes_to_merge_at_min_space_in_pool: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., max_bytes_to_merge_at_max_space_in_pool: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., min_bytes_for_wide_part: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., min_rows_for_wide_part: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., ttl_only_drop_parts: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., merge_with_ttl_timeout: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., merge_with_recompression_ttl_timeout: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., allow_remote_fs_zero_copy_replication: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...) -> None: ...
+        max_parts_in_total: _wrappers_pb2.Int64Value
+        max_number_of_merges_with_ttl_in_pool: _wrappers_pb2.Int64Value
+        cleanup_delay_period: _duration_pb2.Duration
+        number_of_free_entries_in_pool_to_execute_mutation: _wrappers_pb2.Int64Value
+        def __init__(self, replicated_deduplication_window: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., replicated_deduplication_window_seconds: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., parts_to_delay_insert: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., parts_to_throw_insert: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., inactive_parts_to_delay_insert: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., inactive_parts_to_throw_insert: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., max_replicated_merges_in_queue: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., number_of_free_entries_in_pool_to_lower_max_size_of_merge: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., max_bytes_to_merge_at_min_space_in_pool: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., max_bytes_to_merge_at_max_space_in_pool: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., min_bytes_for_wide_part: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., min_rows_for_wide_part: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., ttl_only_drop_parts: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., allow_remote_fs_zero_copy_replication: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., merge_with_ttl_timeout: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., merge_with_recompression_ttl_timeout: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., max_parts_in_total: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., max_number_of_merges_with_ttl_in_pool: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., cleanup_delay_period: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., number_of_free_entries_in_pool_to_execute_mutation: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ...) -> None: ...
     class Kafka(_message.Message):
         __slots__ = ["security_protocol", "sasl_mechanism", "sasl_username", "sasl_password", "enable_ssl_certificate_verification"]
         class SecurityProtocol(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
             __slots__ = []
             SECURITY_PROTOCOL_INVALID: _ClassVar[ClickhouseConfig.Kafka.SecurityProtocol]
             SECURITY_PROTOCOL_PLAINTEXT: _ClassVar[ClickhouseConfig.Kafka.SecurityProtocol]
             SECURITY_PROTOCOL_SSL: _ClassVar[ClickhouseConfig.Kafka.SecurityProtocol]
@@ -174,20 +182,56 @@
     BACKGROUND_SCHEDULE_POOL_SIZE_FIELD_NUMBER: _ClassVar[int]
     BACKGROUND_FETCHES_POOL_SIZE_FIELD_NUMBER: _ClassVar[int]
     BACKGROUND_MOVE_POOL_SIZE_FIELD_NUMBER: _ClassVar[int]
     BACKGROUND_COMMON_POOL_SIZE_FIELD_NUMBER: _ClassVar[int]
     BACKGROUND_MERGES_MUTATIONS_CONCURRENCY_RATIO_FIELD_NUMBER: _ClassVar[int]
     TOTAL_MEMORY_PROFILER_STEP_FIELD_NUMBER: _ClassVar[int]
     TOTAL_MEMORY_TRACKER_SAMPLE_PROBABILITY_FIELD_NUMBER: _ClassVar[int]
+    BACKGROUND_MESSAGE_BROKER_SCHEDULE_POOL_SIZE_FIELD_NUMBER: _ClassVar[int]
     MERGE_TREE_FIELD_NUMBER: _ClassVar[int]
     COMPRESSION_FIELD_NUMBER: _ClassVar[int]
     GRAPHITE_ROLLUP_FIELD_NUMBER: _ClassVar[int]
     KAFKA_FIELD_NUMBER: _ClassVar[int]
     KAFKA_TOPICS_FIELD_NUMBER: _ClassVar[int]
     RABBITMQ_FIELD_NUMBER: _ClassVar[int]
+    QUERY_LOG_RETENTION_SIZE_FIELD_NUMBER: _ClassVar[int]
+    QUERY_LOG_RETENTION_TIME_FIELD_NUMBER: _ClassVar[int]
+    QUERY_THREAD_LOG_ENABLED_FIELD_NUMBER: _ClassVar[int]
+    QUERY_THREAD_LOG_RETENTION_SIZE_FIELD_NUMBER: _ClassVar[int]
+    QUERY_THREAD_LOG_RETENTION_TIME_FIELD_NUMBER: _ClassVar[int]
+    QUERY_VIEWS_LOG_ENABLED_FIELD_NUMBER: _ClassVar[int]
+    QUERY_VIEWS_LOG_RETENTION_SIZE_FIELD_NUMBER: _ClassVar[int]
+    QUERY_VIEWS_LOG_RETENTION_TIME_FIELD_NUMBER: _ClassVar[int]
+    PART_LOG_RETENTION_SIZE_FIELD_NUMBER: _ClassVar[int]
+    PART_LOG_RETENTION_TIME_FIELD_NUMBER: _ClassVar[int]
+    METRIC_LOG_ENABLED_FIELD_NUMBER: _ClassVar[int]
+    METRIC_LOG_RETENTION_SIZE_FIELD_NUMBER: _ClassVar[int]
+    METRIC_LOG_RETENTION_TIME_FIELD_NUMBER: _ClassVar[int]
+    ASYNCHRONOUS_METRIC_LOG_ENABLED_FIELD_NUMBER: _ClassVar[int]
+    ASYNCHRONOUS_METRIC_LOG_RETENTION_SIZE_FIELD_NUMBER: _ClassVar[int]
+    ASYNCHRONOUS_METRIC_LOG_RETENTION_TIME_FIELD_NUMBER: _ClassVar[int]
+    TRACE_LOG_ENABLED_FIELD_NUMBER: _ClassVar[int]
+    TRACE_LOG_RETENTION_SIZE_FIELD_NUMBER: _ClassVar[int]
+    TRACE_LOG_RETENTION_TIME_FIELD_NUMBER: _ClassVar[int]
+    TEXT_LOG_ENABLED_FIELD_NUMBER: _ClassVar[int]
+    TEXT_LOG_RETENTION_SIZE_FIELD_NUMBER: _ClassVar[int]
+    TEXT_LOG_RETENTION_TIME_FIELD_NUMBER: _ClassVar[int]
+    TEXT_LOG_LEVEL_FIELD_NUMBER: _ClassVar[int]
+    OPENTELEMETRY_SPAN_LOG_ENABLED_FIELD_NUMBER: _ClassVar[int]
+    OPENTELEMETRY_SPAN_LOG_RETENTION_SIZE_FIELD_NUMBER: _ClassVar[int]
+    OPENTELEMETRY_SPAN_LOG_RETENTION_TIME_FIELD_NUMBER: _ClassVar[int]
+    SESSION_LOG_ENABLED_FIELD_NUMBER: _ClassVar[int]
+    SESSION_LOG_RETENTION_SIZE_FIELD_NUMBER: _ClassVar[int]
+    SESSION_LOG_RETENTION_TIME_FIELD_NUMBER: _ClassVar[int]
+    ZOOKEEPER_LOG_ENABLED_FIELD_NUMBER: _ClassVar[int]
+    ZOOKEEPER_LOG_RETENTION_SIZE_FIELD_NUMBER: _ClassVar[int]
+    ZOOKEEPER_LOG_RETENTION_TIME_FIELD_NUMBER: _ClassVar[int]
+    ASYNCHRONOUS_INSERT_LOG_ENABLED_FIELD_NUMBER: _ClassVar[int]
+    ASYNCHRONOUS_INSERT_LOG_RETENTION_SIZE_FIELD_NUMBER: _ClassVar[int]
+    ASYNCHRONOUS_INSERT_LOG_RETENTION_TIME_FIELD_NUMBER: _ClassVar[int]
     log_level: ClickhouseConfig.LogLevel
     max_connections: _wrappers_pb2.Int64Value
     max_concurrent_queries: _wrappers_pb2.Int64Value
     keep_alive_timeout: _duration_pb2.Duration
     uncompressed_cache_size: _wrappers_pb2.Int64Value
     mark_cache_size: _wrappers_pb2.Int64Value
     max_table_size_to_drop: _wrappers_pb2.Int64Value
@@ -197,14 +241,50 @@
     background_schedule_pool_size: _wrappers_pb2.Int64Value
     background_fetches_pool_size: _wrappers_pb2.Int64Value
     background_move_pool_size: _wrappers_pb2.Int64Value
     background_common_pool_size: _wrappers_pb2.Int64Value
     background_merges_mutations_concurrency_ratio: _wrappers_pb2.Int64Value
     total_memory_profiler_step: _wrappers_pb2.Int64Value
     total_memory_tracker_sample_probability: _wrappers_pb2.DoubleValue
+    background_message_broker_schedule_pool_size: _wrappers_pb2.Int64Value
     merge_tree: ClickhouseConfig.MergeTree
     compression: _containers.RepeatedCompositeFieldContainer[ClickhouseConfig.Compression]
     graphite_rollup: _containers.MessageMap[str, ClickhouseConfig.GraphiteRollup]
     kafka: ClickhouseConfig.Kafka
     kafka_topics: _containers.MessageMap[str, ClickhouseConfig.Kafka]
     rabbitmq: ClickhouseConfig.Rabbitmq
-    def __init__(self, log_level: _Optional[_Union[ClickhouseConfig.LogLevel, str]] = ..., max_connections: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., max_concurrent_queries: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., keep_alive_timeout: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., uncompressed_cache_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., mark_cache_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., max_table_size_to_drop: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., max_partition_size_to_drop: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., timezone: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., background_pool_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., background_schedule_pool_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., background_fetches_pool_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., background_move_pool_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., background_common_pool_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., background_merges_mutations_concurrency_ratio: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., total_memory_profiler_step: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., total_memory_tracker_sample_probability: _Optional[_Union[_wrappers_pb2.DoubleValue, _Mapping]] = ..., merge_tree: _Optional[_Union[ClickhouseConfig.MergeTree, _Mapping]] = ..., compression: _Optional[_Iterable[_Union[ClickhouseConfig.Compression, _Mapping]]] = ..., graphite_rollup: _Optional[_Mapping[str, ClickhouseConfig.GraphiteRollup]] = ..., kafka: _Optional[_Union[ClickhouseConfig.Kafka, _Mapping]] = ..., kafka_topics: _Optional[_Mapping[str, ClickhouseConfig.Kafka]] = ..., rabbitmq: _Optional[_Union[ClickhouseConfig.Rabbitmq, _Mapping]] = ...) -> None: ...
+    query_log_retention_size: _wrappers_pb2.Int64Value
+    query_log_retention_time: _duration_pb2.Duration
+    query_thread_log_enabled: _wrappers_pb2.BoolValue
+    query_thread_log_retention_size: _wrappers_pb2.Int64Value
+    query_thread_log_retention_time: _duration_pb2.Duration
+    query_views_log_enabled: _wrappers_pb2.BoolValue
+    query_views_log_retention_size: _wrappers_pb2.Int64Value
+    query_views_log_retention_time: _duration_pb2.Duration
+    part_log_retention_size: _wrappers_pb2.Int64Value
+    part_log_retention_time: _duration_pb2.Duration
+    metric_log_enabled: _wrappers_pb2.BoolValue
+    metric_log_retention_size: _wrappers_pb2.Int64Value
+    metric_log_retention_time: _duration_pb2.Duration
+    asynchronous_metric_log_enabled: _wrappers_pb2.BoolValue
+    asynchronous_metric_log_retention_size: _wrappers_pb2.Int64Value
+    asynchronous_metric_log_retention_time: _duration_pb2.Duration
+    trace_log_enabled: _wrappers_pb2.BoolValue
+    trace_log_retention_size: _wrappers_pb2.Int64Value
+    trace_log_retention_time: _duration_pb2.Duration
+    text_log_enabled: _wrappers_pb2.BoolValue
+    text_log_retention_size: _wrappers_pb2.Int64Value
+    text_log_retention_time: _duration_pb2.Duration
+    text_log_level: ClickhouseConfig.LogLevel
+    opentelemetry_span_log_enabled: _wrappers_pb2.BoolValue
+    opentelemetry_span_log_retention_size: _wrappers_pb2.Int64Value
+    opentelemetry_span_log_retention_time: _duration_pb2.Duration
+    session_log_enabled: _wrappers_pb2.BoolValue
+    session_log_retention_size: _wrappers_pb2.Int64Value
+    session_log_retention_time: _duration_pb2.Duration
+    zookeeper_log_enabled: _wrappers_pb2.BoolValue
+    zookeeper_log_retention_size: _wrappers_pb2.Int64Value
+    zookeeper_log_retention_time: _duration_pb2.Duration
+    asynchronous_insert_log_enabled: _wrappers_pb2.BoolValue
+    asynchronous_insert_log_retention_size: _wrappers_pb2.Int64Value
+    asynchronous_insert_log_retention_time: _duration_pb2.Duration
+    def __init__(self, log_level: _Optional[_Union[ClickhouseConfig.LogLevel, str]] = ..., max_connections: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., max_concurrent_queries: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., keep_alive_timeout: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., uncompressed_cache_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., mark_cache_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., max_table_size_to_drop: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., max_partition_size_to_drop: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., timezone: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., background_pool_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., background_schedule_pool_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., background_fetches_pool_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., background_move_pool_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., background_common_pool_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., background_merges_mutations_concurrency_ratio: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., total_memory_profiler_step: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., total_memory_tracker_sample_probability: _Optional[_Union[_wrappers_pb2.DoubleValue, _Mapping]] = ..., background_message_broker_schedule_pool_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., merge_tree: _Optional[_Union[ClickhouseConfig.MergeTree, _Mapping]] = ..., compression: _Optional[_Iterable[_Union[ClickhouseConfig.Compression, _Mapping]]] = ..., graphite_rollup: _Optional[_Mapping[str, ClickhouseConfig.GraphiteRollup]] = ..., kafka: _Optional[_Union[ClickhouseConfig.Kafka, _Mapping]] = ..., kafka_topics: _Optional[_Mapping[str, ClickhouseConfig.Kafka]] = ..., rabbitmq: _Optional[_Union[ClickhouseConfig.Rabbitmq, _Mapping]] = ..., query_log_retention_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., query_log_retention_time: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., query_thread_log_enabled: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., query_thread_log_retention_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., query_thread_log_retention_time: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., query_views_log_enabled: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., query_views_log_retention_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., query_views_log_retention_time: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., part_log_retention_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., part_log_retention_time: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., metric_log_enabled: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., metric_log_retention_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., metric_log_retention_time: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., asynchronous_metric_log_enabled: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., asynchronous_metric_log_retention_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., asynchronous_metric_log_retention_time: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., trace_log_enabled: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., trace_log_retention_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., trace_log_retention_time: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., text_log_enabled: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., text_log_retention_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., text_log_retention_time: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., text_log_level: _Optional[_Union[ClickhouseConfig.LogLevel, str]] = ..., opentelemetry_span_log_enabled: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., opentelemetry_span_log_retention_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., opentelemetry_span_log_retention_time: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., session_log_enabled: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., session_log_retention_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., session_log_retention_time: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., zookeeper_log_enabled: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., zookeeper_log_retention_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., zookeeper_log_retention_time: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., asynchronous_insert_log_enabled: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., asynchronous_insert_log_retention_size: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., asynchronous_insert_log_retention_time: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ...) -> None: ...
```

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/operation_service_pb2.py` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/operation_service_pb2.pyi` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/operation_service_pb2_grpc.py` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/version_pb2.py` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/version_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/version_pb2.pyi` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/version_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/version_service_pb2.py` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/version_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/version_service_pb2.pyi` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/version_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/clickhouse/v1/version_service_pb2_grpc.py` & `doublecloud-0.7.0/doublecloud/clickhouse/v1/version_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/cluster_pb2.py` & `doublecloud-0.7.0/doublecloud/kafka/v1/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/cluster_pb2.pyi` & `doublecloud-0.7.0/doublecloud/kafka/v1/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/cluster_service_pb2.py` & `doublecloud-0.7.0/doublecloud/kafka/v1/cluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/cluster_service_pb2.pyi` & `doublecloud-0.7.0/doublecloud/kafka/v1/cluster_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/cluster_service_pb2_grpc.py` & `doublecloud-0.7.0/doublecloud/kafka/v1/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/config_pb2.py` & `doublecloud-0.7.0/doublecloud/kafka/v1/config_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/config_pb2.pyi` & `doublecloud-0.7.0/doublecloud/kafka/v1/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/connector_pb2.py` & `doublecloud-0.7.0/doublecloud/kafka/v1/connector_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/connector_pb2.pyi` & `doublecloud-0.7.0/doublecloud/kafka/v1/connector_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/connector_service_pb2.py` & `doublecloud-0.7.0/doublecloud/kafka/v1/connector_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/connector_service_pb2.pyi` & `doublecloud-0.7.0/doublecloud/kafka/v1/connector_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/connector_service_pb2_grpc.py` & `doublecloud-0.7.0/doublecloud/kafka/v1/connector_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/operation_service_pb2.py` & `doublecloud-0.7.0/doublecloud/kafka/v1/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/operation_service_pb2.pyi` & `doublecloud-0.7.0/doublecloud/kafka/v1/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/operation_service_pb2_grpc.py` & `doublecloud-0.7.0/doublecloud/kafka/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/topic_pb2.py` & `doublecloud-0.7.0/doublecloud/kafka/v1/topic_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/topic_pb2.pyi` & `doublecloud-0.7.0/doublecloud/kafka/v1/topic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/topic_service_pb2.py` & `doublecloud-0.7.0/doublecloud/kafka/v1/topic_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/topic_service_pb2.pyi` & `doublecloud-0.7.0/doublecloud/kafka/v1/topic_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/topic_service_pb2_grpc.py` & `doublecloud-0.7.0/doublecloud/kafka/v1/topic_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/user_pb2.py` & `doublecloud-0.7.0/doublecloud/kafka/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/user_pb2.pyi` & `doublecloud-0.7.0/doublecloud/kafka/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/user_service_pb2.py` & `doublecloud-0.7.0/doublecloud/kafka/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/user_service_pb2.pyi` & `doublecloud-0.7.0/doublecloud/kafka/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/user_service_pb2_grpc.py` & `doublecloud-0.7.0/doublecloud/kafka/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/version_pb2.py` & `doublecloud-0.7.0/doublecloud/kafka/v1/version_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/version_pb2.pyi` & `doublecloud-0.7.0/doublecloud/kafka/v1/version_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/version_service_pb2.py` & `doublecloud-0.7.0/doublecloud/kafka/v1/version_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/version_service_pb2.pyi` & `doublecloud-0.7.0/doublecloud/kafka/v1/version_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/kafka/v1/version_service_pb2_grpc.py` & `doublecloud-0.7.0/doublecloud/kafka/v1/version_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/network/v1/network_connection_pb2.py` & `doublecloud-0.7.0/doublecloud/network/v1/network_connection_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/doublecloud/network/v1/network_connection.proto\x12\x16\x64oublecloud.network.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"\xff\x04\n\x11NetworkConnection\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nnetwork_id\x18\x02 \x01(\tR\tnetworkId\x12\x44\n\x03\x61ws\x18\x04 \x01(\x0b\x32\x30.doublecloud.network.v1.AWSNetworkConnectionInfoH\x00R\x03\x61ws\x12;\n\x0b\x63reate_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ncreateTime\x12 \n\x0b\x64\x65scription\x18\x08 \x01(\tR\x0b\x64\x65scription\x12Y\n\x06status\x18\t \x01(\x0e\x32\x41.doublecloud.network.v1.NetworkConnection.NetworkConnectionStatusR\x06status\x12#\n\rstatus_reason\x18\n \x01(\tR\x0cstatusReason\"\x82\x02\n\x17NetworkConnectionStatus\x12%\n!NETWORK_CONNECTION_STATUS_INVALID\x10\x00\x12&\n\"NETWORK_CONNECTION_STATUS_CREATING\x10\x01\x12%\n!NETWORK_CONNECTION_STATUS_PENDING\x10\x02\x12$\n NETWORK_CONNECTION_STATUS_ACTIVE\x10\x03\x12&\n\"NETWORK_CONNECTION_STATUS_DELETING\x10\x04\x12#\n\x1fNETWORK_CONNECTION_STATUS_ERROR\x10\x05\x42\x11\n\x0f\x63onnection_info\"w\n\x18\x41WSNetworkConnectionInfo\x12S\n\x07peering\x18\x01 \x01(\x0b\x32\x37.doublecloud.network.v1.AWSNetworkConnectionPeeringInfoH\x00R\x07peeringB\x06\n\x04type\"\xe6\x02\n\x1f\x41WSNetworkConnectionPeeringInfo\x12\x15\n\x06vpc_id\x18\x01 \x01(\tR\x05vpcId\x12\x1d\n\naccount_id\x18\x02 \x01(\tR\taccountId\x12\x1b\n\tregion_id\x18\x03 \x01(\tR\x08regionId\x12&\n\x0fipv4_cidr_block\x18\x04 \x01(\tR\ripv4CidrBlock\x12&\n\x0fipv6_cidr_block\x18\x05 \x01(\tR\ripv6CidrBlock\x12\x32\n\x15peering_connection_id\x18\x06 \x01(\tR\x13peeringConnectionId\x12\x35\n\x17managed_ipv4_cidr_block\x18\x07 \x01(\tR\x14managedIpv4CidrBlock\x12\x35\n\x17managed_ipv6_cidr_block\x18\x08 \x01(\tR\x14managedIpv6CidrBlockBCZAgithub.com/doublecloud/go-genproto/doublecloud/network/v1;networkb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/doublecloud/network/v1/network_connection.proto\x12\x16\x64oublecloud.network.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"\xce\x05\n\x11NetworkConnection\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nnetwork_id\x18\x02 \x01(\tR\tnetworkId\x12\x44\n\x03\x61ws\x18\x04 \x01(\x0b\x32\x30.doublecloud.network.v1.AWSNetworkConnectionInfoH\x00R\x03\x61ws\x12M\n\x06google\x18\x05 \x01(\x0b\x32\x33.doublecloud.network.v1.GoogleNetworkConnectionInfoH\x00R\x06google\x12;\n\x0b\x63reate_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ncreateTime\x12 \n\x0b\x64\x65scription\x18\x08 \x01(\tR\x0b\x64\x65scription\x12Y\n\x06status\x18\t \x01(\x0e\x32\x41.doublecloud.network.v1.NetworkConnection.NetworkConnectionStatusR\x06status\x12#\n\rstatus_reason\x18\n \x01(\tR\x0cstatusReason\"\x82\x02\n\x17NetworkConnectionStatus\x12%\n!NETWORK_CONNECTION_STATUS_INVALID\x10\x00\x12&\n\"NETWORK_CONNECTION_STATUS_CREATING\x10\x01\x12%\n!NETWORK_CONNECTION_STATUS_PENDING\x10\x02\x12$\n NETWORK_CONNECTION_STATUS_ACTIVE\x10\x03\x12&\n\"NETWORK_CONNECTION_STATUS_DELETING\x10\x04\x12#\n\x1fNETWORK_CONNECTION_STATUS_ERROR\x10\x05\x42\x11\n\x0f\x63onnection_info\"w\n\x18\x41WSNetworkConnectionInfo\x12S\n\x07peering\x18\x01 \x01(\x0b\x32\x37.doublecloud.network.v1.AWSNetworkConnectionPeeringInfoH\x00R\x07peeringB\x06\n\x04type\"\xe6\x02\n\x1f\x41WSNetworkConnectionPeeringInfo\x12\x15\n\x06vpc_id\x18\x01 \x01(\tR\x05vpcId\x12\x1d\n\naccount_id\x18\x02 \x01(\tR\taccountId\x12\x1b\n\tregion_id\x18\x03 \x01(\tR\x08regionId\x12&\n\x0fipv4_cidr_block\x18\x04 \x01(\tR\ripv4CidrBlock\x12&\n\x0fipv6_cidr_block\x18\x05 \x01(\tR\ripv6CidrBlock\x12\x32\n\x15peering_connection_id\x18\x06 \x01(\tR\x13peeringConnectionId\x12\x35\n\x17managed_ipv4_cidr_block\x18\x07 \x01(\tR\x14managedIpv4CidrBlock\x12\x35\n\x17managed_ipv6_cidr_block\x18\x08 \x01(\tR\x14managedIpv6CidrBlock\"\x8b\x01\n\x1bGoogleNetworkConnectionInfo\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12(\n\x10peer_network_url\x18\x02 \x01(\tR\x0epeerNetworkUrl\x12.\n\x13managed_network_url\x18\x03 \x01(\tR\x11managedNetworkUrlBCZAgithub.com/doublecloud/go-genproto/doublecloud/network/v1;networkb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.network.v1.network_connection_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZAgithub.com/doublecloud/go-genproto/doublecloud/network/v1;network'
   _globals['_NETWORKCONNECTION']._serialized_start=109
-  _globals['_NETWORKCONNECTION']._serialized_end=748
-  _globals['_NETWORKCONNECTION_NETWORKCONNECTIONSTATUS']._serialized_start=471
-  _globals['_NETWORKCONNECTION_NETWORKCONNECTIONSTATUS']._serialized_end=729
-  _globals['_AWSNETWORKCONNECTIONINFO']._serialized_start=750
-  _globals['_AWSNETWORKCONNECTIONINFO']._serialized_end=869
-  _globals['_AWSNETWORKCONNECTIONPEERINGINFO']._serialized_start=872
-  _globals['_AWSNETWORKCONNECTIONPEERINGINFO']._serialized_end=1230
+  _globals['_NETWORKCONNECTION']._serialized_end=827
+  _globals['_NETWORKCONNECTION_NETWORKCONNECTIONSTATUS']._serialized_start=550
+  _globals['_NETWORKCONNECTION_NETWORKCONNECTIONSTATUS']._serialized_end=808
+  _globals['_AWSNETWORKCONNECTIONINFO']._serialized_start=829
+  _globals['_AWSNETWORKCONNECTIONINFO']._serialized_end=948
+  _globals['_AWSNETWORKCONNECTIONPEERINGINFO']._serialized_start=951
+  _globals['_AWSNETWORKCONNECTIONPEERINGINFO']._serialized_end=1309
+  _globals['_GOOGLENETWORKCONNECTIONINFO']._serialized_start=1312
+  _globals['_GOOGLENETWORKCONNECTIONINFO']._serialized_end=1451
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.6.0/doublecloud/network/v1/network_connection_pb2.pyi` & `doublecloud-0.7.0/doublecloud/network/v1/network_connection_service_pb2.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,85 @@
-from google.protobuf import timestamp_pb2 as _timestamp_pb2
-from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
+from doublecloud.network.v1 import network_connection_pb2 as _network_connection_pb2
+from doublecloud.v1 import operation_pb2 as _operation_pb2
+from doublecloud.v1 import paging_pb2 as _paging_pb2
+from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class NetworkConnection(_message.Message):
-    __slots__ = ["id", "network_id", "aws", "create_time", "description", "status", "status_reason"]
-    class NetworkConnectionStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-        NETWORK_CONNECTION_STATUS_INVALID: _ClassVar[NetworkConnection.NetworkConnectionStatus]
-        NETWORK_CONNECTION_STATUS_CREATING: _ClassVar[NetworkConnection.NetworkConnectionStatus]
-        NETWORK_CONNECTION_STATUS_PENDING: _ClassVar[NetworkConnection.NetworkConnectionStatus]
-        NETWORK_CONNECTION_STATUS_ACTIVE: _ClassVar[NetworkConnection.NetworkConnectionStatus]
-        NETWORK_CONNECTION_STATUS_DELETING: _ClassVar[NetworkConnection.NetworkConnectionStatus]
-        NETWORK_CONNECTION_STATUS_ERROR: _ClassVar[NetworkConnection.NetworkConnectionStatus]
-    NETWORK_CONNECTION_STATUS_INVALID: NetworkConnection.NetworkConnectionStatus
-    NETWORK_CONNECTION_STATUS_CREATING: NetworkConnection.NetworkConnectionStatus
-    NETWORK_CONNECTION_STATUS_PENDING: NetworkConnection.NetworkConnectionStatus
-    NETWORK_CONNECTION_STATUS_ACTIVE: NetworkConnection.NetworkConnectionStatus
-    NETWORK_CONNECTION_STATUS_DELETING: NetworkConnection.NetworkConnectionStatus
-    NETWORK_CONNECTION_STATUS_ERROR: NetworkConnection.NetworkConnectionStatus
-    ID_FIELD_NUMBER: _ClassVar[int]
+class GetNetworkConnectionRequest(_message.Message):
+    __slots__ = ["network_connection_id"]
+    NETWORK_CONNECTION_ID_FIELD_NUMBER: _ClassVar[int]
+    network_connection_id: str
+    def __init__(self, network_connection_id: _Optional[str] = ...) -> None: ...
+
+class ListNetworkConnectionsRequest(_message.Message):
+    __slots__ = ["project_id", "paging"]
+    PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
+    PAGING_FIELD_NUMBER: _ClassVar[int]
+    project_id: str
+    paging: _paging_pb2.Paging
+    def __init__(self, project_id: _Optional[str] = ..., paging: _Optional[_Union[_paging_pb2.Paging, _Mapping]] = ...) -> None: ...
+
+class ListNetworkConnectionsResponse(_message.Message):
+    __slots__ = ["network_connections", "next_page"]
+    NETWORK_CONNECTIONS_FIELD_NUMBER: _ClassVar[int]
+    NEXT_PAGE_FIELD_NUMBER: _ClassVar[int]
+    network_connections: _containers.RepeatedCompositeFieldContainer[_network_connection_pb2.NetworkConnection]
+    next_page: _paging_pb2.NextPage
+    def __init__(self, network_connections: _Optional[_Iterable[_Union[_network_connection_pb2.NetworkConnection, _Mapping]]] = ..., next_page: _Optional[_Union[_paging_pb2.NextPage, _Mapping]] = ...) -> None: ...
+
+class CreateNetworkConnectionRequest(_message.Message):
+    __slots__ = ["network_id", "aws", "google", "description"]
     NETWORK_ID_FIELD_NUMBER: _ClassVar[int]
     AWS_FIELD_NUMBER: _ClassVar[int]
-    CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
+    GOOGLE_FIELD_NUMBER: _ClassVar[int]
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
-    STATUS_REASON_FIELD_NUMBER: _ClassVar[int]
-    id: str
     network_id: str
-    aws: AWSNetworkConnectionInfo
-    create_time: _timestamp_pb2.Timestamp
+    aws: CreateAWSNetworkConnectionRequest
+    google: CreateGoogleNetworkConnectionRequest
     description: str
-    status: NetworkConnection.NetworkConnectionStatus
-    status_reason: str
-    def __init__(self, id: _Optional[str] = ..., network_id: _Optional[str] = ..., aws: _Optional[_Union[AWSNetworkConnectionInfo, _Mapping]] = ..., create_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., description: _Optional[str] = ..., status: _Optional[_Union[NetworkConnection.NetworkConnectionStatus, str]] = ..., status_reason: _Optional[str] = ...) -> None: ...
+    def __init__(self, network_id: _Optional[str] = ..., aws: _Optional[_Union[CreateAWSNetworkConnectionRequest, _Mapping]] = ..., google: _Optional[_Union[CreateGoogleNetworkConnectionRequest, _Mapping]] = ..., description: _Optional[str] = ...) -> None: ...
 
-class AWSNetworkConnectionInfo(_message.Message):
+class CreateAWSNetworkConnectionRequest(_message.Message):
     __slots__ = ["peering"]
     PEERING_FIELD_NUMBER: _ClassVar[int]
-    peering: AWSNetworkConnectionPeeringInfo
-    def __init__(self, peering: _Optional[_Union[AWSNetworkConnectionPeeringInfo, _Mapping]] = ...) -> None: ...
+    peering: CreateAWSNetworkConnectionPeeringRequest
+    def __init__(self, peering: _Optional[_Union[CreateAWSNetworkConnectionPeeringRequest, _Mapping]] = ...) -> None: ...
 
-class AWSNetworkConnectionPeeringInfo(_message.Message):
-    __slots__ = ["vpc_id", "account_id", "region_id", "ipv4_cidr_block", "ipv6_cidr_block", "peering_connection_id", "managed_ipv4_cidr_block", "managed_ipv6_cidr_block"]
+class CreateAWSNetworkConnectionPeeringRequest(_message.Message):
+    __slots__ = ["vpc_id", "account_id", "region_id", "ipv4_cidr_block", "ipv6_cidr_block"]
     VPC_ID_FIELD_NUMBER: _ClassVar[int]
     ACCOUNT_ID_FIELD_NUMBER: _ClassVar[int]
     REGION_ID_FIELD_NUMBER: _ClassVar[int]
     IPV4_CIDR_BLOCK_FIELD_NUMBER: _ClassVar[int]
     IPV6_CIDR_BLOCK_FIELD_NUMBER: _ClassVar[int]
-    PEERING_CONNECTION_ID_FIELD_NUMBER: _ClassVar[int]
-    MANAGED_IPV4_CIDR_BLOCK_FIELD_NUMBER: _ClassVar[int]
-    MANAGED_IPV6_CIDR_BLOCK_FIELD_NUMBER: _ClassVar[int]
     vpc_id: str
     account_id: str
     region_id: str
     ipv4_cidr_block: str
     ipv6_cidr_block: str
-    peering_connection_id: str
-    managed_ipv4_cidr_block: str
-    managed_ipv6_cidr_block: str
-    def __init__(self, vpc_id: _Optional[str] = ..., account_id: _Optional[str] = ..., region_id: _Optional[str] = ..., ipv4_cidr_block: _Optional[str] = ..., ipv6_cidr_block: _Optional[str] = ..., peering_connection_id: _Optional[str] = ..., managed_ipv4_cidr_block: _Optional[str] = ..., managed_ipv6_cidr_block: _Optional[str] = ...) -> None: ...
+    def __init__(self, vpc_id: _Optional[str] = ..., account_id: _Optional[str] = ..., region_id: _Optional[str] = ..., ipv4_cidr_block: _Optional[str] = ..., ipv6_cidr_block: _Optional[str] = ...) -> None: ...
+
+class CreateGoogleNetworkConnectionRequest(_message.Message):
+    __slots__ = ["name", "peer_network_url"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    PEER_NETWORK_URL_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    peer_network_url: str
+    def __init__(self, name: _Optional[str] = ..., peer_network_url: _Optional[str] = ...) -> None: ...
+
+class DeleteNetworkConnectionRequest(_message.Message):
+    __slots__ = ["network_connection_id"]
+    NETWORK_CONNECTION_ID_FIELD_NUMBER: _ClassVar[int]
+    network_connection_id: str
+    def __init__(self, network_connection_id: _Optional[str] = ...) -> None: ...
+
+class UpdateNetworkConnectionRequest(_message.Message):
+    __slots__ = ["network_connection_id", "description"]
+    NETWORK_CONNECTION_ID_FIELD_NUMBER: _ClassVar[int]
+    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+    network_connection_id: str
+    description: str
+    def __init__(self, network_connection_id: _Optional[str] = ..., description: _Optional[str] = ...) -> None: ...
```

### Comparing `doublecloud-0.6.0/doublecloud/network/v1/network_connection_service_pb2.py` & `doublecloud-0.7.0/doublecloud/network/v1/network_connection_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 from doublecloud.network.v1 import network_connection_pb2 as doublecloud_dot_network_dot_v1_dot_network__connection__pb2
 from doublecloud.v1 import operation_pb2 as doublecloud_dot_v1_dot_operation__pb2
 from doublecloud.v1 import paging_pb2 as doublecloud_dot_v1_dot_paging__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7doublecloud/network/v1/network_connection_service.proto\x12\x16\x64oublecloud.network.v1\x1a/doublecloud/network/v1/network_connection.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\"Q\n\x1bGetNetworkConnectionRequest\x12\x32\n\x15network_connection_id\x18\x01 \x01(\tR\x13networkConnectionId\"n\n\x1dListNetworkConnectionsRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\xb3\x01\n\x1eListNetworkConnectionsResponse\x12Z\n\x13network_connections\x18\x01 \x03(\x0b\x32).doublecloud.network.v1.NetworkConnectionR\x12networkConnections\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"\xba\x01\n\x1e\x43reateNetworkConnectionRequest\x12\x1d\n\nnetwork_id\x18\x01 \x01(\tR\tnetworkId\x12M\n\x03\x61ws\x18\x03 \x01(\x0b\x32\x39.doublecloud.network.v1.CreateAWSNetworkConnectionRequestH\x00R\x03\x61ws\x12 \n\x0b\x64\x65scription\x18\x06 \x01(\tR\x0b\x64\x65scriptionB\x08\n\x06params\"\x89\x01\n!CreateAWSNetworkConnectionRequest\x12\\\n\x07peering\x18\x01 \x01(\x0b\x32@.doublecloud.network.v1.CreateAWSNetworkConnectionPeeringRequestH\x00R\x07peeringB\x06\n\x04type\"\xcd\x01\n(CreateAWSNetworkConnectionPeeringRequest\x12\x15\n\x06vpc_id\x18\x01 \x01(\tR\x05vpcId\x12\x1d\n\naccount_id\x18\x02 \x01(\tR\taccountId\x12\x1b\n\tregion_id\x18\x03 \x01(\tR\x08regionId\x12&\n\x0fipv4_cidr_block\x18\x04 \x01(\tR\ripv4CidrBlock\x12&\n\x0fipv6_cidr_block\x18\x05 \x01(\tR\ripv6CidrBlock\"T\n\x1e\x44\x65leteNetworkConnectionRequest\x12\x32\n\x15network_connection_id\x18\x01 \x01(\tR\x13networkConnectionId\"v\n\x1eUpdateNetworkConnectionRequest\x12\x32\n\x15network_connection_id\x18\x01 \x01(\tR\x13networkConnectionId\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription2\xb2\x03\n\x18NetworkConnectionService\x12\x65\n\x03Get\x12\x33.doublecloud.network.v1.GetNetworkConnectionRequest\x1a).doublecloud.network.v1.NetworkConnection\x12u\n\x04List\x12\x35.doublecloud.network.v1.ListNetworkConnectionsRequest\x1a\x36.doublecloud.network.v1.ListNetworkConnectionsResponse\x12[\n\x06\x43reate\x12\x36.doublecloud.network.v1.CreateNetworkConnectionRequest\x1a\x19.doublecloud.v1.Operation\x12[\n\x06\x44\x65lete\x12\x36.doublecloud.network.v1.DeleteNetworkConnectionRequest\x1a\x19.doublecloud.v1.OperationBCZAgithub.com/doublecloud/go-genproto/doublecloud/network/v1;networkb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7doublecloud/network/v1/network_connection_service.proto\x12\x16\x64oublecloud.network.v1\x1a/doublecloud/network/v1/network_connection.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\"Q\n\x1bGetNetworkConnectionRequest\x12\x32\n\x15network_connection_id\x18\x01 \x01(\tR\x13networkConnectionId\"n\n\x1dListNetworkConnectionsRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\xb3\x01\n\x1eListNetworkConnectionsResponse\x12Z\n\x13network_connections\x18\x01 \x03(\x0b\x32).doublecloud.network.v1.NetworkConnectionR\x12networkConnections\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"\x92\x02\n\x1e\x43reateNetworkConnectionRequest\x12\x1d\n\nnetwork_id\x18\x01 \x01(\tR\tnetworkId\x12M\n\x03\x61ws\x18\x03 \x01(\x0b\x32\x39.doublecloud.network.v1.CreateAWSNetworkConnectionRequestH\x00R\x03\x61ws\x12V\n\x06google\x18\x04 \x01(\x0b\x32<.doublecloud.network.v1.CreateGoogleNetworkConnectionRequestH\x00R\x06google\x12 \n\x0b\x64\x65scription\x18\x06 \x01(\tR\x0b\x64\x65scriptionB\x08\n\x06params\"\x89\x01\n!CreateAWSNetworkConnectionRequest\x12\\\n\x07peering\x18\x01 \x01(\x0b\x32@.doublecloud.network.v1.CreateAWSNetworkConnectionPeeringRequestH\x00R\x07peeringB\x06\n\x04type\"\xcd\x01\n(CreateAWSNetworkConnectionPeeringRequest\x12\x15\n\x06vpc_id\x18\x01 \x01(\tR\x05vpcId\x12\x1d\n\naccount_id\x18\x02 \x01(\tR\taccountId\x12\x1b\n\tregion_id\x18\x03 \x01(\tR\x08regionId\x12&\n\x0fipv4_cidr_block\x18\x04 \x01(\tR\ripv4CidrBlock\x12&\n\x0fipv6_cidr_block\x18\x05 \x01(\tR\ripv6CidrBlock\"d\n$CreateGoogleNetworkConnectionRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12(\n\x10peer_network_url\x18\x02 \x01(\tR\x0epeerNetworkUrl\"T\n\x1e\x44\x65leteNetworkConnectionRequest\x12\x32\n\x15network_connection_id\x18\x01 \x01(\tR\x13networkConnectionId\"v\n\x1eUpdateNetworkConnectionRequest\x12\x32\n\x15network_connection_id\x18\x01 \x01(\tR\x13networkConnectionId\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription2\xb2\x03\n\x18NetworkConnectionService\x12\x65\n\x03Get\x12\x33.doublecloud.network.v1.GetNetworkConnectionRequest\x1a).doublecloud.network.v1.NetworkConnection\x12u\n\x04List\x12\x35.doublecloud.network.v1.ListNetworkConnectionsRequest\x1a\x36.doublecloud.network.v1.ListNetworkConnectionsResponse\x12[\n\x06\x43reate\x12\x36.doublecloud.network.v1.CreateNetworkConnectionRequest\x1a\x19.doublecloud.v1.Operation\x12[\n\x06\x44\x65lete\x12\x36.doublecloud.network.v1.DeleteNetworkConnectionRequest\x1a\x19.doublecloud.v1.OperationBCZAgithub.com/doublecloud/go-genproto/doublecloud/network/v1;networkb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.network.v1.network_connection_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -28,19 +28,21 @@
   _globals['_GETNETWORKCONNECTIONREQUEST']._serialized_start=193
   _globals['_GETNETWORKCONNECTIONREQUEST']._serialized_end=274
   _globals['_LISTNETWORKCONNECTIONSREQUEST']._serialized_start=276
   _globals['_LISTNETWORKCONNECTIONSREQUEST']._serialized_end=386
   _globals['_LISTNETWORKCONNECTIONSRESPONSE']._serialized_start=389
   _globals['_LISTNETWORKCONNECTIONSRESPONSE']._serialized_end=568
   _globals['_CREATENETWORKCONNECTIONREQUEST']._serialized_start=571
-  _globals['_CREATENETWORKCONNECTIONREQUEST']._serialized_end=757
-  _globals['_CREATEAWSNETWORKCONNECTIONREQUEST']._serialized_start=760
-  _globals['_CREATEAWSNETWORKCONNECTIONREQUEST']._serialized_end=897
-  _globals['_CREATEAWSNETWORKCONNECTIONPEERINGREQUEST']._serialized_start=900
-  _globals['_CREATEAWSNETWORKCONNECTIONPEERINGREQUEST']._serialized_end=1105
-  _globals['_DELETENETWORKCONNECTIONREQUEST']._serialized_start=1107
-  _globals['_DELETENETWORKCONNECTIONREQUEST']._serialized_end=1191
-  _globals['_UPDATENETWORKCONNECTIONREQUEST']._serialized_start=1193
-  _globals['_UPDATENETWORKCONNECTIONREQUEST']._serialized_end=1311
-  _globals['_NETWORKCONNECTIONSERVICE']._serialized_start=1314
-  _globals['_NETWORKCONNECTIONSERVICE']._serialized_end=1748
+  _globals['_CREATENETWORKCONNECTIONREQUEST']._serialized_end=845
+  _globals['_CREATEAWSNETWORKCONNECTIONREQUEST']._serialized_start=848
+  _globals['_CREATEAWSNETWORKCONNECTIONREQUEST']._serialized_end=985
+  _globals['_CREATEAWSNETWORKCONNECTIONPEERINGREQUEST']._serialized_start=988
+  _globals['_CREATEAWSNETWORKCONNECTIONPEERINGREQUEST']._serialized_end=1193
+  _globals['_CREATEGOOGLENETWORKCONNECTIONREQUEST']._serialized_start=1195
+  _globals['_CREATEGOOGLENETWORKCONNECTIONREQUEST']._serialized_end=1295
+  _globals['_DELETENETWORKCONNECTIONREQUEST']._serialized_start=1297
+  _globals['_DELETENETWORKCONNECTIONREQUEST']._serialized_end=1381
+  _globals['_UPDATENETWORKCONNECTIONREQUEST']._serialized_start=1383
+  _globals['_UPDATENETWORKCONNECTIONREQUEST']._serialized_end=1501
+  _globals['_NETWORKCONNECTIONSERVICE']._serialized_start=1504
+  _globals['_NETWORKCONNECTIONSERVICE']._serialized_end=1938
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.6.0/doublecloud/network/v1/network_connection_service_pb2.pyi` & `doublecloud-0.7.0/doublecloud/network/v1/network_service_pb2.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,75 +1,95 @@
-from doublecloud.network.v1 import network_connection_pb2 as _network_connection_pb2
+from doublecloud.network.v1 import network_pb2 as _network_pb2
 from doublecloud.v1 import operation_pb2 as _operation_pb2
 from doublecloud.v1 import paging_pb2 as _paging_pb2
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class GetNetworkConnectionRequest(_message.Message):
-    __slots__ = ["network_connection_id"]
-    NETWORK_CONNECTION_ID_FIELD_NUMBER: _ClassVar[int]
-    network_connection_id: str
-    def __init__(self, network_connection_id: _Optional[str] = ...) -> None: ...
+class GetNetworkRequest(_message.Message):
+    __slots__ = ["network_id"]
+    NETWORK_ID_FIELD_NUMBER: _ClassVar[int]
+    network_id: str
+    def __init__(self, network_id: _Optional[str] = ...) -> None: ...
 
-class ListNetworkConnectionsRequest(_message.Message):
-    __slots__ = ["project_id", "paging"]
+class ListNetworksRequest(_message.Message):
+    __slots__ = ["project_id", "paging", "filter"]
+    class Filter(_message.Message):
+        __slots__ = ["cloud_type", "region_id", "status", "is_external"]
+        CLOUD_TYPE_FIELD_NUMBER: _ClassVar[int]
+        REGION_ID_FIELD_NUMBER: _ClassVar[int]
+        STATUS_FIELD_NUMBER: _ClassVar[int]
+        IS_EXTERNAL_FIELD_NUMBER: _ClassVar[int]
+        cloud_type: _wrappers_pb2.StringValue
+        region_id: _wrappers_pb2.StringValue
+        status: _network_pb2.Network.NetworkStatus
+        is_external: _wrappers_pb2.BoolValue
+        def __init__(self, cloud_type: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., region_id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., status: _Optional[_Union[_network_pb2.Network.NetworkStatus, str]] = ..., is_external: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...) -> None: ...
     PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     PAGING_FIELD_NUMBER: _ClassVar[int]
+    FILTER_FIELD_NUMBER: _ClassVar[int]
     project_id: str
     paging: _paging_pb2.Paging
-    def __init__(self, project_id: _Optional[str] = ..., paging: _Optional[_Union[_paging_pb2.Paging, _Mapping]] = ...) -> None: ...
+    filter: ListNetworksRequest.Filter
+    def __init__(self, project_id: _Optional[str] = ..., paging: _Optional[_Union[_paging_pb2.Paging, _Mapping]] = ..., filter: _Optional[_Union[ListNetworksRequest.Filter, _Mapping]] = ...) -> None: ...
 
-class ListNetworkConnectionsResponse(_message.Message):
-    __slots__ = ["network_connections", "next_page"]
-    NETWORK_CONNECTIONS_FIELD_NUMBER: _ClassVar[int]
+class ListNetworksResponse(_message.Message):
+    __slots__ = ["networks", "next_page"]
+    NETWORKS_FIELD_NUMBER: _ClassVar[int]
     NEXT_PAGE_FIELD_NUMBER: _ClassVar[int]
-    network_connections: _containers.RepeatedCompositeFieldContainer[_network_connection_pb2.NetworkConnection]
+    networks: _containers.RepeatedCompositeFieldContainer[_network_pb2.Network]
     next_page: _paging_pb2.NextPage
-    def __init__(self, network_connections: _Optional[_Iterable[_Union[_network_connection_pb2.NetworkConnection, _Mapping]]] = ..., next_page: _Optional[_Union[_paging_pb2.NextPage, _Mapping]] = ...) -> None: ...
+    def __init__(self, networks: _Optional[_Iterable[_Union[_network_pb2.Network, _Mapping]]] = ..., next_page: _Optional[_Union[_paging_pb2.NextPage, _Mapping]] = ...) -> None: ...
 
-class CreateNetworkConnectionRequest(_message.Message):
-    __slots__ = ["network_id", "aws", "description"]
-    NETWORK_ID_FIELD_NUMBER: _ClassVar[int]
-    AWS_FIELD_NUMBER: _ClassVar[int]
+class CreateNetworkRequest(_message.Message):
+    __slots__ = ["project_id", "cloud_type", "region_id", "name", "description", "ipv4_cidr_block"]
+    PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
+    CLOUD_TYPE_FIELD_NUMBER: _ClassVar[int]
+    REGION_ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    network_id: str
-    aws: CreateAWSNetworkConnectionRequest
+    IPV4_CIDR_BLOCK_FIELD_NUMBER: _ClassVar[int]
+    project_id: str
+    cloud_type: str
+    region_id: str
+    name: str
     description: str
-    def __init__(self, network_id: _Optional[str] = ..., aws: _Optional[_Union[CreateAWSNetworkConnectionRequest, _Mapping]] = ..., description: _Optional[str] = ...) -> None: ...
+    ipv4_cidr_block: str
+    def __init__(self, project_id: _Optional[str] = ..., cloud_type: _Optional[str] = ..., region_id: _Optional[str] = ..., name: _Optional[str] = ..., description: _Optional[str] = ..., ipv4_cidr_block: _Optional[str] = ...) -> None: ...
+
+class DeleteNetworkRequest(_message.Message):
+    __slots__ = ["network_id"]
+    NETWORK_ID_FIELD_NUMBER: _ClassVar[int]
+    network_id: str
+    def __init__(self, network_id: _Optional[str] = ...) -> None: ...
 
-class CreateAWSNetworkConnectionRequest(_message.Message):
-    __slots__ = ["peering"]
-    PEERING_FIELD_NUMBER: _ClassVar[int]
-    peering: CreateAWSNetworkConnectionPeeringRequest
-    def __init__(self, peering: _Optional[_Union[CreateAWSNetworkConnectionPeeringRequest, _Mapping]] = ...) -> None: ...
+class ImportNetworkRequest(_message.Message):
+    __slots__ = ["project_id", "name", "description", "aws"]
+    PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+    AWS_FIELD_NUMBER: _ClassVar[int]
+    project_id: str
+    name: str
+    description: str
+    aws: ImportAWSVPCRequest
+    def __init__(self, project_id: _Optional[str] = ..., name: _Optional[str] = ..., description: _Optional[str] = ..., aws: _Optional[_Union[ImportAWSVPCRequest, _Mapping]] = ...) -> None: ...
 
-class CreateAWSNetworkConnectionPeeringRequest(_message.Message):
-    __slots__ = ["vpc_id", "account_id", "region_id", "ipv4_cidr_block", "ipv6_cidr_block"]
+class ImportAWSVPCRequest(_message.Message):
+    __slots__ = ["vpc_id", "region_id", "account_id", "iam_role_arn", "stack_id", "version"]
     VPC_ID_FIELD_NUMBER: _ClassVar[int]
-    ACCOUNT_ID_FIELD_NUMBER: _ClassVar[int]
     REGION_ID_FIELD_NUMBER: _ClassVar[int]
-    IPV4_CIDR_BLOCK_FIELD_NUMBER: _ClassVar[int]
-    IPV6_CIDR_BLOCK_FIELD_NUMBER: _ClassVar[int]
+    ACCOUNT_ID_FIELD_NUMBER: _ClassVar[int]
+    IAM_ROLE_ARN_FIELD_NUMBER: _ClassVar[int]
+    STACK_ID_FIELD_NUMBER: _ClassVar[int]
+    VERSION_FIELD_NUMBER: _ClassVar[int]
     vpc_id: str
-    account_id: str
     region_id: str
-    ipv4_cidr_block: str
-    ipv6_cidr_block: str
-    def __init__(self, vpc_id: _Optional[str] = ..., account_id: _Optional[str] = ..., region_id: _Optional[str] = ..., ipv4_cidr_block: _Optional[str] = ..., ipv6_cidr_block: _Optional[str] = ...) -> None: ...
-
-class DeleteNetworkConnectionRequest(_message.Message):
-    __slots__ = ["network_connection_id"]
-    NETWORK_CONNECTION_ID_FIELD_NUMBER: _ClassVar[int]
-    network_connection_id: str
-    def __init__(self, network_connection_id: _Optional[str] = ...) -> None: ...
-
-class UpdateNetworkConnectionRequest(_message.Message):
-    __slots__ = ["network_connection_id", "description"]
-    NETWORK_CONNECTION_ID_FIELD_NUMBER: _ClassVar[int]
-    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    network_connection_id: str
-    description: str
-    def __init__(self, network_connection_id: _Optional[str] = ..., description: _Optional[str] = ...) -> None: ...
+    account_id: str
+    iam_role_arn: str
+    stack_id: str
+    version: str
+    def __init__(self, vpc_id: _Optional[str] = ..., region_id: _Optional[str] = ..., account_id: _Optional[str] = ..., iam_role_arn: _Optional[str] = ..., stack_id: _Optional[str] = ..., version: _Optional[str] = ...) -> None: ...
```

### Comparing `doublecloud-0.6.0/doublecloud/network/v1/network_connection_service_pb2_grpc.py` & `doublecloud-0.7.0/doublecloud/network/v1/network_connection_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/network/v1/network_pb2.py` & `doublecloud-0.7.0/doublecloud/network/v1/network_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$doublecloud/network/v1/network.proto\x12\x16\x64oublecloud.network.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xb9\x05\n\x07Network\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1d\n\ncloud_type\x18\x03 \x01(\tR\tcloudType\x12\x1b\n\tregion_id\x18\x04 \x01(\tR\x08regionId\x12;\n\x0b\x63reate_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ncreateTime\x12\x12\n\x04name\x18\x06 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x07 \x01(\tR\x0b\x64\x65scription\x12&\n\x0fipv4_cidr_block\x18\x08 \x01(\tR\ripv4CidrBlock\x12&\n\x0fipv6_cidr_block\x18\t \x01(\tR\ripv6CidrBlock\x12\x45\n\x06status\x18\n \x01(\x0e\x32-.doublecloud.network.v1.Network.NetworkStatusR\x06status\x12#\n\rstatus_reason\x18\x0b \x01(\tR\x0cstatusReason\x12@\n\x03\x61ws\x18\x0c \x01(\x0b\x32,.doublecloud.network.v1.AwsExternalResourcesH\x00R\x03\x61ws\x12\x1f\n\x0bis_external\x18\r \x01(\x08R\nisExternal\"\x9a\x01\n\rNetworkStatus\x12\x1a\n\x16NETWORK_STATUS_INVALID\x10\x00\x12\x1b\n\x17NETWORK_STATUS_CREATING\x10\x01\x12\x19\n\x15NETWORK_STATUS_ACTIVE\x10\x02\x12\x1b\n\x17NETWORK_STATUS_DELETING\x10\x03\x12\x18\n\x14NETWORK_STATUS_ERROR\x10\x04\x42\x14\n\x12\x65xternal_resources\"\xdf\x03\n\x14\x41wsExternalResources\x12\x15\n\x06vpc_id\x18\x01 \x01(\tR\x05vpcId\x12M\n\x07subnets\x18\x02 \x03(\x0b\x32\x33.doublecloud.network.v1.AwsExternalResources.SubnetR\x07subnets\x12*\n\x11security_group_id\x18\x03 \x01(\tR\x0fsecurityGroupId\x12;\n\naccount_id\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\taccountId\x12>\n\x0ciam_role_arn\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\niamRoleArn\x12\x37\n\x08stack_id\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x07stackId\x12L\n\x13\x63\x66_template_version\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x11\x63\x66TemplateVersion\x1a\x31\n\x06Subnet\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x17\n\x07zone_id\x18\x02 \x01(\tR\x06zoneIdBCZAgithub.com/doublecloud/go-genproto/doublecloud/network/v1;networkb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$doublecloud/network/v1/network.proto\x12\x16\x64oublecloud.network.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xfb\x05\n\x07Network\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1d\n\ncloud_type\x18\x03 \x01(\tR\tcloudType\x12\x1b\n\tregion_id\x18\x04 \x01(\tR\x08regionId\x12;\n\x0b\x63reate_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ncreateTime\x12\x12\n\x04name\x18\x06 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x07 \x01(\tR\x0b\x64\x65scription\x12&\n\x0fipv4_cidr_block\x18\x08 \x01(\tR\ripv4CidrBlock\x12&\n\x0fipv6_cidr_block\x18\t \x01(\tR\ripv6CidrBlock\x12\x45\n\x06status\x18\n \x01(\x0e\x32-.doublecloud.network.v1.Network.NetworkStatusR\x06status\x12#\n\rstatus_reason\x18\x0b \x01(\tR\x0cstatusReason\x12@\n\x03\x61ws\x18\x0c \x01(\x0b\x32,.doublecloud.network.v1.AwsExternalResourcesH\x00R\x03\x61ws\x12@\n\x03gcp\x18\x0e \x01(\x0b\x32,.doublecloud.network.v1.GcpExternalResourcesH\x00R\x03gcp\x12\x1f\n\x0bis_external\x18\r \x01(\x08R\nisExternal\"\x9a\x01\n\rNetworkStatus\x12\x1a\n\x16NETWORK_STATUS_INVALID\x10\x00\x12\x1b\n\x17NETWORK_STATUS_CREATING\x10\x01\x12\x19\n\x15NETWORK_STATUS_ACTIVE\x10\x02\x12\x1b\n\x17NETWORK_STATUS_DELETING\x10\x03\x12\x18\n\x14NETWORK_STATUS_ERROR\x10\x04\x42\x14\n\x12\x65xternal_resources\"\xdf\x03\n\x14\x41wsExternalResources\x12\x15\n\x06vpc_id\x18\x01 \x01(\tR\x05vpcId\x12M\n\x07subnets\x18\x02 \x03(\x0b\x32\x33.doublecloud.network.v1.AwsExternalResources.SubnetR\x07subnets\x12*\n\x11security_group_id\x18\x03 \x01(\tR\x0fsecurityGroupId\x12;\n\naccount_id\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\taccountId\x12>\n\x0ciam_role_arn\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\niamRoleArn\x12\x37\n\x08stack_id\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x07stackId\x12L\n\x13\x63\x66_template_version\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x11\x63\x66TemplateVersion\x1a\x31\n\x06Subnet\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x17\n\x07zone_id\x18\x02 \x01(\tR\x06zoneId\"?\n\x14GcpExternalResources\x12\'\n\x0fsubnetwork_link\x18\x01 \x01(\tR\x0esubnetworkLinkBCZAgithub.com/doublecloud/go-genproto/doublecloud/network/v1;networkb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.network.v1.network_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZAgithub.com/doublecloud/go-genproto/doublecloud/network/v1;network'
   _globals['_NETWORK']._serialized_start=130
-  _globals['_NETWORK']._serialized_end=827
-  _globals['_NETWORK_NETWORKSTATUS']._serialized_start=651
-  _globals['_NETWORK_NETWORKSTATUS']._serialized_end=805
-  _globals['_AWSEXTERNALRESOURCES']._serialized_start=830
-  _globals['_AWSEXTERNALRESOURCES']._serialized_end=1309
-  _globals['_AWSEXTERNALRESOURCES_SUBNET']._serialized_start=1260
-  _globals['_AWSEXTERNALRESOURCES_SUBNET']._serialized_end=1309
+  _globals['_NETWORK']._serialized_end=893
+  _globals['_NETWORK_NETWORKSTATUS']._serialized_start=717
+  _globals['_NETWORK_NETWORKSTATUS']._serialized_end=871
+  _globals['_AWSEXTERNALRESOURCES']._serialized_start=896
+  _globals['_AWSEXTERNALRESOURCES']._serialized_end=1375
+  _globals['_AWSEXTERNALRESOURCES_SUBNET']._serialized_start=1326
+  _globals['_AWSEXTERNALRESOURCES_SUBNET']._serialized_end=1375
+  _globals['_GCPEXTERNALRESOURCES']._serialized_start=1377
+  _globals['_GCPEXTERNALRESOURCES']._serialized_end=1440
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.6.0/doublecloud/network/v1/network_pb2.pyi` & `doublecloud-0.7.0/doublecloud/network/v1/network_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Network(_message.Message):
-    __slots__ = ["id", "project_id", "cloud_type", "region_id", "create_time", "name", "description", "ipv4_cidr_block", "ipv6_cidr_block", "status", "status_reason", "aws", "is_external"]
+    __slots__ = ["id", "project_id", "cloud_type", "region_id", "create_time", "name", "description", "ipv4_cidr_block", "ipv6_cidr_block", "status", "status_reason", "aws", "gcp", "is_external"]
     class NetworkStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
         NETWORK_STATUS_INVALID: _ClassVar[Network.NetworkStatus]
         NETWORK_STATUS_CREATING: _ClassVar[Network.NetworkStatus]
         NETWORK_STATUS_ACTIVE: _ClassVar[Network.NetworkStatus]
         NETWORK_STATUS_DELETING: _ClassVar[Network.NetworkStatus]
         NETWORK_STATUS_ERROR: _ClassVar[Network.NetworkStatus]
@@ -30,29 +30,31 @@
     NAME_FIELD_NUMBER: _ClassVar[int]
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
     IPV4_CIDR_BLOCK_FIELD_NUMBER: _ClassVar[int]
     IPV6_CIDR_BLOCK_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     STATUS_REASON_FIELD_NUMBER: _ClassVar[int]
     AWS_FIELD_NUMBER: _ClassVar[int]
+    GCP_FIELD_NUMBER: _ClassVar[int]
     IS_EXTERNAL_FIELD_NUMBER: _ClassVar[int]
     id: str
     project_id: str
     cloud_type: str
     region_id: str
     create_time: _timestamp_pb2.Timestamp
     name: str
     description: str
     ipv4_cidr_block: str
     ipv6_cidr_block: str
     status: Network.NetworkStatus
     status_reason: str
     aws: AwsExternalResources
+    gcp: GcpExternalResources
     is_external: bool
-    def __init__(self, id: _Optional[str] = ..., project_id: _Optional[str] = ..., cloud_type: _Optional[str] = ..., region_id: _Optional[str] = ..., create_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., name: _Optional[str] = ..., description: _Optional[str] = ..., ipv4_cidr_block: _Optional[str] = ..., ipv6_cidr_block: _Optional[str] = ..., status: _Optional[_Union[Network.NetworkStatus, str]] = ..., status_reason: _Optional[str] = ..., aws: _Optional[_Union[AwsExternalResources, _Mapping]] = ..., is_external: bool = ...) -> None: ...
+    def __init__(self, id: _Optional[str] = ..., project_id: _Optional[str] = ..., cloud_type: _Optional[str] = ..., region_id: _Optional[str] = ..., create_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., name: _Optional[str] = ..., description: _Optional[str] = ..., ipv4_cidr_block: _Optional[str] = ..., ipv6_cidr_block: _Optional[str] = ..., status: _Optional[_Union[Network.NetworkStatus, str]] = ..., status_reason: _Optional[str] = ..., aws: _Optional[_Union[AwsExternalResources, _Mapping]] = ..., gcp: _Optional[_Union[GcpExternalResources, _Mapping]] = ..., is_external: bool = ...) -> None: ...
 
 class AwsExternalResources(_message.Message):
     __slots__ = ["vpc_id", "subnets", "security_group_id", "account_id", "iam_role_arn", "stack_id", "cf_template_version"]
     class Subnet(_message.Message):
         __slots__ = ["id", "zone_id"]
         ID_FIELD_NUMBER: _ClassVar[int]
         ZONE_ID_FIELD_NUMBER: _ClassVar[int]
@@ -70,7 +72,13 @@
     subnets: _containers.RepeatedCompositeFieldContainer[AwsExternalResources.Subnet]
     security_group_id: str
     account_id: _wrappers_pb2.StringValue
     iam_role_arn: _wrappers_pb2.StringValue
     stack_id: _wrappers_pb2.StringValue
     cf_template_version: _wrappers_pb2.StringValue
     def __init__(self, vpc_id: _Optional[str] = ..., subnets: _Optional[_Iterable[_Union[AwsExternalResources.Subnet, _Mapping]]] = ..., security_group_id: _Optional[str] = ..., account_id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., iam_role_arn: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., stack_id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., cf_template_version: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
+
+class GcpExternalResources(_message.Message):
+    __slots__ = ["subnetwork_link"]
+    SUBNETWORK_LINK_FIELD_NUMBER: _ClassVar[int]
+    subnetwork_link: str
+    def __init__(self, subnetwork_link: _Optional[str] = ...) -> None: ...
```

### Comparing `doublecloud-0.6.0/doublecloud/network/v1/network_service_pb2.py` & `doublecloud-0.7.0/doublecloud/network/v1/network_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/network/v1/network_service_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mysql_pb2.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,81 @@
-from doublecloud.network.v1 import network_pb2 as _network_pb2
-from doublecloud.v1 import operation_pb2 as _operation_pb2
-from doublecloud.v1 import paging_pb2 as _paging_pb2
-from google.protobuf import wrappers_pb2 as _wrappers_pb2
+from doublecloud.transfer.v1.endpoint import common_pb2 as _common_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class GetNetworkRequest(_message.Message):
-    __slots__ = ["network_id"]
-    NETWORK_ID_FIELD_NUMBER: _ClassVar[int]
-    network_id: str
-    def __init__(self, network_id: _Optional[str] = ...) -> None: ...
-
-class ListNetworksRequest(_message.Message):
-    __slots__ = ["project_id", "paging", "filter"]
-    class Filter(_message.Message):
-        __slots__ = ["cloud_type", "region_id", "status", "is_external"]
-        CLOUD_TYPE_FIELD_NUMBER: _ClassVar[int]
-        REGION_ID_FIELD_NUMBER: _ClassVar[int]
-        STATUS_FIELD_NUMBER: _ClassVar[int]
-        IS_EXTERNAL_FIELD_NUMBER: _ClassVar[int]
-        cloud_type: _wrappers_pb2.StringValue
-        region_id: _wrappers_pb2.StringValue
-        status: _network_pb2.Network.NetworkStatus
-        is_external: _wrappers_pb2.BoolValue
-        def __init__(self, cloud_type: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., region_id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., status: _Optional[_Union[_network_pb2.Network.NetworkStatus, str]] = ..., is_external: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...) -> None: ...
-    PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
-    PAGING_FIELD_NUMBER: _ClassVar[int]
-    FILTER_FIELD_NUMBER: _ClassVar[int]
-    project_id: str
-    paging: _paging_pb2.Paging
-    filter: ListNetworksRequest.Filter
-    def __init__(self, project_id: _Optional[str] = ..., paging: _Optional[_Union[_paging_pb2.Paging, _Mapping]] = ..., filter: _Optional[_Union[ListNetworksRequest.Filter, _Mapping]] = ...) -> None: ...
-
-class ListNetworksResponse(_message.Message):
-    __slots__ = ["networks", "next_page"]
-    NETWORKS_FIELD_NUMBER: _ClassVar[int]
-    NEXT_PAGE_FIELD_NUMBER: _ClassVar[int]
-    networks: _containers.RepeatedCompositeFieldContainer[_network_pb2.Network]
-    next_page: _paging_pb2.NextPage
-    def __init__(self, networks: _Optional[_Iterable[_Union[_network_pb2.Network, _Mapping]]] = ..., next_page: _Optional[_Union[_paging_pb2.NextPage, _Mapping]] = ...) -> None: ...
-
-class CreateNetworkRequest(_message.Message):
-    __slots__ = ["project_id", "cloud_type", "region_id", "name", "description", "ipv4_cidr_block"]
-    PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
-    CLOUD_TYPE_FIELD_NUMBER: _ClassVar[int]
-    REGION_ID_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    IPV4_CIDR_BLOCK_FIELD_NUMBER: _ClassVar[int]
-    project_id: str
-    cloud_type: str
-    region_id: str
-    name: str
-    description: str
-    ipv4_cidr_block: str
-    def __init__(self, project_id: _Optional[str] = ..., cloud_type: _Optional[str] = ..., region_id: _Optional[str] = ..., name: _Optional[str] = ..., description: _Optional[str] = ..., ipv4_cidr_block: _Optional[str] = ...) -> None: ...
-
-class DeleteNetworkRequest(_message.Message):
-    __slots__ = ["network_id"]
-    NETWORK_ID_FIELD_NUMBER: _ClassVar[int]
-    network_id: str
-    def __init__(self, network_id: _Optional[str] = ...) -> None: ...
-
-class ImportNetworkRequest(_message.Message):
-    __slots__ = ["project_id", "name", "description", "aws"]
-    PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    AWS_FIELD_NUMBER: _ClassVar[int]
-    project_id: str
-    name: str
-    description: str
-    aws: ImportAWSVPCRequest
-    def __init__(self, project_id: _Optional[str] = ..., name: _Optional[str] = ..., description: _Optional[str] = ..., aws: _Optional[_Union[ImportAWSVPCRequest, _Mapping]] = ...) -> None: ...
-
-class ImportAWSVPCRequest(_message.Message):
-    __slots__ = ["vpc_id", "region_id", "account_id", "iam_role_arn", "stack_id", "version"]
-    VPC_ID_FIELD_NUMBER: _ClassVar[int]
-    REGION_ID_FIELD_NUMBER: _ClassVar[int]
-    ACCOUNT_ID_FIELD_NUMBER: _ClassVar[int]
-    IAM_ROLE_ARN_FIELD_NUMBER: _ClassVar[int]
-    STACK_ID_FIELD_NUMBER: _ClassVar[int]
-    VERSION_FIELD_NUMBER: _ClassVar[int]
-    vpc_id: str
-    region_id: str
-    account_id: str
-    iam_role_arn: str
-    stack_id: str
-    version: str
-    def __init__(self, vpc_id: _Optional[str] = ..., region_id: _Optional[str] = ..., account_id: _Optional[str] = ..., iam_role_arn: _Optional[str] = ..., stack_id: _Optional[str] = ..., version: _Optional[str] = ...) -> None: ...
+class OnPremiseMysql(_message.Message):
+    __slots__ = ["hosts", "port", "tls_mode"]
+    HOSTS_FIELD_NUMBER: _ClassVar[int]
+    PORT_FIELD_NUMBER: _ClassVar[int]
+    TLS_MODE_FIELD_NUMBER: _ClassVar[int]
+    hosts: _containers.RepeatedScalarFieldContainer[str]
+    port: int
+    tls_mode: _common_pb2.TLSMode
+    def __init__(self, hosts: _Optional[_Iterable[str]] = ..., port: _Optional[int] = ..., tls_mode: _Optional[_Union[_common_pb2.TLSMode, _Mapping]] = ...) -> None: ...
+
+class MysqlConnection(_message.Message):
+    __slots__ = ["on_premise"]
+    ON_PREMISE_FIELD_NUMBER: _ClassVar[int]
+    on_premise: OnPremiseMysql
+    def __init__(self, on_premise: _Optional[_Union[OnPremiseMysql, _Mapping]] = ...) -> None: ...
+
+class MysqlObjectTransferSettings(_message.Message):
+    __slots__ = ["view", "routine", "trigger", "tables"]
+    VIEW_FIELD_NUMBER: _ClassVar[int]
+    ROUTINE_FIELD_NUMBER: _ClassVar[int]
+    TRIGGER_FIELD_NUMBER: _ClassVar[int]
+    TABLES_FIELD_NUMBER: _ClassVar[int]
+    view: _common_pb2.ObjectTransferStage
+    routine: _common_pb2.ObjectTransferStage
+    trigger: _common_pb2.ObjectTransferStage
+    tables: _common_pb2.ObjectTransferStage
+    def __init__(self, view: _Optional[_Union[_common_pb2.ObjectTransferStage, str]] = ..., routine: _Optional[_Union[_common_pb2.ObjectTransferStage, str]] = ..., trigger: _Optional[_Union[_common_pb2.ObjectTransferStage, str]] = ..., tables: _Optional[_Union[_common_pb2.ObjectTransferStage, str]] = ...) -> None: ...
+
+class MysqlSource(_message.Message):
+    __slots__ = ["connection", "database", "service_database", "user", "password", "include_tables_regex", "exclude_tables_regex", "timezone", "object_transfer_settings"]
+    CONNECTION_FIELD_NUMBER: _ClassVar[int]
+    DATABASE_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_DATABASE_FIELD_NUMBER: _ClassVar[int]
+    USER_FIELD_NUMBER: _ClassVar[int]
+    PASSWORD_FIELD_NUMBER: _ClassVar[int]
+    INCLUDE_TABLES_REGEX_FIELD_NUMBER: _ClassVar[int]
+    EXCLUDE_TABLES_REGEX_FIELD_NUMBER: _ClassVar[int]
+    TIMEZONE_FIELD_NUMBER: _ClassVar[int]
+    OBJECT_TRANSFER_SETTINGS_FIELD_NUMBER: _ClassVar[int]
+    connection: MysqlConnection
+    database: str
+    service_database: str
+    user: str
+    password: _common_pb2.Secret
+    include_tables_regex: _containers.RepeatedScalarFieldContainer[str]
+    exclude_tables_regex: _containers.RepeatedScalarFieldContainer[str]
+    timezone: str
+    object_transfer_settings: MysqlObjectTransferSettings
+    def __init__(self, connection: _Optional[_Union[MysqlConnection, _Mapping]] = ..., database: _Optional[str] = ..., service_database: _Optional[str] = ..., user: _Optional[str] = ..., password: _Optional[_Union[_common_pb2.Secret, _Mapping]] = ..., include_tables_regex: _Optional[_Iterable[str]] = ..., exclude_tables_regex: _Optional[_Iterable[str]] = ..., timezone: _Optional[str] = ..., object_transfer_settings: _Optional[_Union[MysqlObjectTransferSettings, _Mapping]] = ...) -> None: ...
+
+class MysqlTarget(_message.Message):
+    __slots__ = ["connection", "security_groups", "database", "user", "password", "sql_mode", "skip_constraint_checks", "timezone", "cleanup_policy", "service_database"]
+    CONNECTION_FIELD_NUMBER: _ClassVar[int]
+    SECURITY_GROUPS_FIELD_NUMBER: _ClassVar[int]
+    DATABASE_FIELD_NUMBER: _ClassVar[int]
+    USER_FIELD_NUMBER: _ClassVar[int]
+    PASSWORD_FIELD_NUMBER: _ClassVar[int]
+    SQL_MODE_FIELD_NUMBER: _ClassVar[int]
+    SKIP_CONSTRAINT_CHECKS_FIELD_NUMBER: _ClassVar[int]
+    TIMEZONE_FIELD_NUMBER: _ClassVar[int]
+    CLEANUP_POLICY_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_DATABASE_FIELD_NUMBER: _ClassVar[int]
+    connection: MysqlConnection
+    security_groups: _containers.RepeatedScalarFieldContainer[str]
+    database: str
+    user: str
+    password: _common_pb2.Secret
+    sql_mode: str
+    skip_constraint_checks: bool
+    timezone: str
+    cleanup_policy: _common_pb2.CleanupPolicy
+    service_database: str
+    def __init__(self, connection: _Optional[_Union[MysqlConnection, _Mapping]] = ..., security_groups: _Optional[_Iterable[str]] = ..., database: _Optional[str] = ..., user: _Optional[str] = ..., password: _Optional[_Union[_common_pb2.Secret, _Mapping]] = ..., sql_mode: _Optional[str] = ..., skip_constraint_checks: bool = ..., timezone: _Optional[str] = ..., cleanup_policy: _Optional[_Union[_common_pb2.CleanupPolicy, str]] = ..., service_database: _Optional[str] = ...) -> None: ...
```

### Comparing `doublecloud-0.6.0/doublecloud/network/v1/network_service_pb2_grpc.py` & `doublecloud-0.7.0/doublecloud/network/v1/network_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/network/v1/operation_service_pb2.py` & `doublecloud-0.7.0/doublecloud/network/v1/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/network/v1/operation_service_pb2.pyi` & `doublecloud-0.7.0/doublecloud/network/v1/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/network/v1/operation_service_pb2_grpc.py` & `doublecloud-0.7.0/doublecloud/network/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n?doublecloud/transfer/v1/endpoint/airbyte/snowflake_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"\xa5\x06\n\x0fSnowflakeSource\x12\x12\n\x04host\x18\x01 \x01(\tR\x04host\x12\x12\n\x04role\x18\x02 \x01(\tR\x04role\x12\x1c\n\twarehouse\x18\x03 \x01(\tR\twarehouse\x12\x1a\n\x08\x64\x61tabase\x18\x04 \x01(\tR\x08\x64\x61tabase\x12\x16\n\x06schema\x18\x05 \x01(\tR\x06schema\x12&\n\x0fjdbc_url_params\x18\x06 \x01(\tR\rjdbcUrlParams\x12g\n\x0b\x63redentials\x18\x07 \x01(\x0b\x32\x45.doublecloud.transfer.v1.endpoint.airbyte.SnowflakeSource.CredentialsR\x0b\x63redentials\x1a\x86\x04\n\x0b\x43redentials\x12\x63\n\x05oauth\x18\x01 \x01(\x0b\x32K.doublecloud.transfer.v1.endpoint.airbyte.SnowflakeSource.Credentials.OAuthH\x00R\x05oauth\x12p\n\nbasic_auth\x18\x02 \x01(\x0b\x32O.doublecloud.transfer.v1.endpoint.airbyte.SnowflakeSource.Credentials.BasicAuthH\x00R\tbasicAuth\x1a\xae\x01\n\x05OAuth\x12\x1b\n\tauth_type\x18\x01 \x01(\tR\x08\x61uthType\x12\x1b\n\tclient_id\x18\x02 \x01(\tR\x08\x63lientId\x12#\n\rclient_secret\x18\x03 \x01(\tR\x0c\x63lientSecret\x12!\n\x0c\x61\x63\x63\x65ss_token\x18\x04 \x01(\tR\x0b\x61\x63\x63\x65ssToken\x12#\n\rrefresh_token\x18\x05 \x01(\tR\x0crefreshToken\x1a`\n\tBasicAuth\x12\x1b\n\tauth_type\x18\x01 \x01(\tR\x08\x61uthType\x12\x1a\n\x08username\x18\x02 \x01(\tR\x08username\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08passwordB\r\n\x0b\x63redentialsB^Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n?doublecloud/transfer/v1/endpoint/airbyte/snowflake_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"\xeb\x05\n\x0fSnowflakeSource\x12\x12\n\x04host\x18\x01 \x01(\tR\x04host\x12\x12\n\x04role\x18\x02 \x01(\tR\x04role\x12\x1c\n\twarehouse\x18\x03 \x01(\tR\twarehouse\x12\x1a\n\x08\x64\x61tabase\x18\x04 \x01(\tR\x08\x64\x61tabase\x12\x16\n\x06schema\x18\x05 \x01(\tR\x06schema\x12&\n\x0fjdbc_url_params\x18\x06 \x01(\tR\rjdbcUrlParams\x12g\n\x0b\x63redentials\x18\x07 \x01(\x0b\x32\x45.doublecloud.transfer.v1.endpoint.airbyte.SnowflakeSource.CredentialsR\x0b\x63redentials\x1a\xcc\x03\n\x0b\x43redentials\x12\x63\n\x05oauth\x18\x01 \x01(\x0b\x32K.doublecloud.transfer.v1.endpoint.airbyte.SnowflakeSource.Credentials.OAuthH\x00R\x05oauth\x12p\n\nbasic_auth\x18\x02 \x01(\x0b\x32O.doublecloud.transfer.v1.endpoint.airbyte.SnowflakeSource.Credentials.BasicAuthH\x00R\tbasicAuth\x1a\x91\x01\n\x05OAuth\x12\x1b\n\tclient_id\x18\x02 \x01(\tR\x08\x63lientId\x12#\n\rclient_secret\x18\x03 \x01(\tR\x0c\x63lientSecret\x12!\n\x0c\x61\x63\x63\x65ss_token\x18\x04 \x01(\tR\x0b\x61\x63\x63\x65ssToken\x12#\n\rrefresh_token\x18\x05 \x01(\tR\x0crefreshToken\x1a\x43\n\tBasicAuth\x12\x1a\n\x08username\x18\x02 \x01(\tR\x08username\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08passwordB\r\n\x0b\x63redentialsB^Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint.airbyte.snowflake_source_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyte'
   _globals['_SNOWFLAKESOURCE']._serialized_start=110
-  _globals['_SNOWFLAKESOURCE']._serialized_end=915
+  _globals['_SNOWFLAKESOURCE']._serialized_end=857
   _globals['_SNOWFLAKESOURCE_CREDENTIALS']._serialized_start=397
-  _globals['_SNOWFLAKESOURCE_CREDENTIALS']._serialized_end=915
+  _globals['_SNOWFLAKESOURCE_CREDENTIALS']._serialized_end=857
   _globals['_SNOWFLAKESOURCE_CREDENTIALS_OAUTH']._serialized_start=628
-  _globals['_SNOWFLAKESOURCE_CREDENTIALS_OAUTH']._serialized_end=802
-  _globals['_SNOWFLAKESOURCE_CREDENTIALS_BASICAUTH']._serialized_start=804
-  _globals['_SNOWFLAKESOURCE_CREDENTIALS_BASICAUTH']._serialized_end=900
+  _globals['_SNOWFLAKESOURCE_CREDENTIALS_OAUTH']._serialized_end=773
+  _globals['_SNOWFLAKESOURCE_CREDENTIALS_BASICAUTH']._serialized_start=775
+  _globals['_SNOWFLAKESOURCE_CREDENTIALS_BASICAUTH']._serialized_end=842
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -5,35 +5,31 @@
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class SnowflakeSource(_message.Message):
     __slots__ = ["host", "role", "warehouse", "database", "schema", "jdbc_url_params", "credentials"]
     class Credentials(_message.Message):
         __slots__ = ["oauth", "basic_auth"]
         class OAuth(_message.Message):
-            __slots__ = ["auth_type", "client_id", "client_secret", "access_token", "refresh_token"]
-            AUTH_TYPE_FIELD_NUMBER: _ClassVar[int]
+            __slots__ = ["client_id", "client_secret", "access_token", "refresh_token"]
             CLIENT_ID_FIELD_NUMBER: _ClassVar[int]
             CLIENT_SECRET_FIELD_NUMBER: _ClassVar[int]
             ACCESS_TOKEN_FIELD_NUMBER: _ClassVar[int]
             REFRESH_TOKEN_FIELD_NUMBER: _ClassVar[int]
-            auth_type: str
             client_id: str
             client_secret: str
             access_token: str
             refresh_token: str
-            def __init__(self, auth_type: _Optional[str] = ..., client_id: _Optional[str] = ..., client_secret: _Optional[str] = ..., access_token: _Optional[str] = ..., refresh_token: _Optional[str] = ...) -> None: ...
+            def __init__(self, client_id: _Optional[str] = ..., client_secret: _Optional[str] = ..., access_token: _Optional[str] = ..., refresh_token: _Optional[str] = ...) -> None: ...
         class BasicAuth(_message.Message):
-            __slots__ = ["auth_type", "username", "password"]
-            AUTH_TYPE_FIELD_NUMBER: _ClassVar[int]
+            __slots__ = ["username", "password"]
             USERNAME_FIELD_NUMBER: _ClassVar[int]
             PASSWORD_FIELD_NUMBER: _ClassVar[int]
-            auth_type: str
             username: str
             password: str
-            def __init__(self, auth_type: _Optional[str] = ..., username: _Optional[str] = ..., password: _Optional[str] = ...) -> None: ...
+            def __init__(self, username: _Optional[str] = ..., password: _Optional[str] = ...) -> None: ...
         OAUTH_FIELD_NUMBER: _ClassVar[int]
         BASIC_AUTH_FIELD_NUMBER: _ClassVar[int]
         oauth: SnowflakeSource.Credentials.OAuth
         basic_auth: SnowflakeSource.Credentials.BasicAuth
         def __init__(self, oauth: _Optional[_Union[SnowflakeSource.Credentials.OAuth, _Mapping]] = ..., basic_auth: _Optional[_Union[SnowflakeSource.Credentials.BasicAuth, _Mapping]] = ...) -> None: ...
     HOST_FIELD_NUMBER: _ClassVar[int]
     ROLE_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/common_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/common_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/common_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/kafka_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/kafka_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,37 +9,38 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from doublecloud.transfer.v1.endpoint import common_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_common__pb2
 from doublecloud.transfer.v1.endpoint import parsers_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_parsers__pb2
+from doublecloud.transfer.v1.endpoint import serializers_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_serializers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,doublecloud/transfer/v1/endpoint/kafka.proto\x12 doublecloud.transfer.v1.endpoint\x1a-doublecloud/transfer/v1/endpoint/common.proto\x1a.doublecloud/transfer/v1/endpoint/parsers.proto\"\x9a\x01\n\x16KafkaConnectionOptions\x12\x1f\n\ncluster_id\x18\x01 \x01(\tH\x00R\tclusterId\x12Q\n\non_premise\x18\x02 \x01(\x0b\x32\x30.doublecloud.transfer.v1.endpoint.OnPremiseKafkaH\x00R\tonPremiseB\x0c\n\nconnection\"w\n\x0eOnPremiseKafka\x12\x1f\n\x0b\x62roker_urls\x18\x01 \x03(\tR\nbrokerUrls\x12\x44\n\x08tls_mode\x18\x05 \x01(\x0b\x32).doublecloud.transfer.v1.endpoint.TLSModeR\x07tlsMode\"\xa7\x01\n\tKafkaAuth\x12I\n\x04sasl\x18\x01 \x01(\x0b\x32\x33.doublecloud.transfer.v1.endpoint.KafkaSaslSecurityH\x00R\x04sasl\x12\x43\n\x07no_auth\x18\x02 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.NoAuthH\x00R\x06noAuthB\n\n\x08security\"\xbd\x01\n\x11KafkaSaslSecurity\x12\x12\n\x04user\x18\x01 \x01(\tR\x04user\x12\x44\n\x08password\x18\x04 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.SecretR\x08password\x12N\n\tmechanism\x18\x03 \x01(\x0e\x32\x30.doublecloud.transfer.v1.endpoint.KafkaMechanismR\tmechanism\"\x89\x02\n\x0bKafkaSource\x12X\n\nconnection\x18\x01 \x01(\x0b\x32\x38.doublecloud.transfer.v1.endpoint.KafkaConnectionOptionsR\nconnection\x12?\n\x04\x61uth\x18\x02 \x01(\x0b\x32+.doublecloud.transfer.v1.endpoint.KafkaAuthR\x04\x61uth\x12\x1d\n\ntopic_name\x18\x04 \x01(\tR\ttopicName\x12@\n\x06parser\x18\x07 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.ParserR\x06parser\"\x8b\x02\n\x0bKafkaTarget\x12X\n\nconnection\x18\x01 \x01(\x0b\x32\x38.doublecloud.transfer.v1.endpoint.KafkaConnectionOptionsR\nconnection\x12?\n\x04\x61uth\x18\x02 \x01(\x0b\x32+.doublecloud.transfer.v1.endpoint.KafkaAuthR\x04\x61uth\x12\x61\n\x0etopic_settings\x18\x07 \x01(\x0b\x32:.doublecloud.transfer.v1.endpoint.KafkaTargetTopicSettingsR\rtopicSettings\"\x9d\x01\n\x18KafkaTargetTopicSettings\x12J\n\x05topic\x18\x01 \x01(\x0b\x32\x32.doublecloud.transfer.v1.endpoint.KafkaTargetTopicH\x00R\x05topic\x12#\n\x0ctopic_prefix\x18\x02 \x01(\tH\x00R\x0btopicPrefixB\x10\n\x0etopic_settings\"U\n\x10KafkaTargetTopic\x12\x1d\n\ntopic_name\x18\x01 \x01(\tR\ttopicName\x12\"\n\rsave_tx_order\x18\x02 \x01(\x08R\x0bsaveTxOrder*i\n\x0eKafkaMechanism\x12\x1f\n\x1bKAFKA_MECHANISM_UNSPECIFIED\x10\x00\x12\x1a\n\x16KAFKA_MECHANISM_SHA256\x10\x01\x12\x1a\n\x16KAFKA_MECHANISM_SHA512\x10\x02\x42NZLgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint;endpointb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,doublecloud/transfer/v1/endpoint/kafka.proto\x12 doublecloud.transfer.v1.endpoint\x1a-doublecloud/transfer/v1/endpoint/common.proto\x1a.doublecloud/transfer/v1/endpoint/parsers.proto\x1a\x32\x64oublecloud/transfer/v1/endpoint/serializers.proto\"\x9a\x01\n\x16KafkaConnectionOptions\x12\x1f\n\ncluster_id\x18\x01 \x01(\tH\x00R\tclusterId\x12Q\n\non_premise\x18\x02 \x01(\x0b\x32\x30.doublecloud.transfer.v1.endpoint.OnPremiseKafkaH\x00R\tonPremiseB\x0c\n\nconnection\"w\n\x0eOnPremiseKafka\x12\x1f\n\x0b\x62roker_urls\x18\x01 \x03(\tR\nbrokerUrls\x12\x44\n\x08tls_mode\x18\x05 \x01(\x0b\x32).doublecloud.transfer.v1.endpoint.TLSModeR\x07tlsMode\"\xa7\x01\n\tKafkaAuth\x12I\n\x04sasl\x18\x01 \x01(\x0b\x32\x33.doublecloud.transfer.v1.endpoint.KafkaSaslSecurityH\x00R\x04sasl\x12\x43\n\x07no_auth\x18\x02 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.NoAuthH\x00R\x06noAuthB\n\n\x08security\"\xbd\x01\n\x11KafkaSaslSecurity\x12\x12\n\x04user\x18\x01 \x01(\tR\x04user\x12\x44\n\x08password\x18\x04 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.SecretR\x08password\x12N\n\tmechanism\x18\x03 \x01(\x0e\x32\x30.doublecloud.transfer.v1.endpoint.KafkaMechanismR\tmechanism\"\x89\x02\n\x0bKafkaSource\x12X\n\nconnection\x18\x01 \x01(\x0b\x32\x38.doublecloud.transfer.v1.endpoint.KafkaConnectionOptionsR\nconnection\x12?\n\x04\x61uth\x18\x02 \x01(\x0b\x32+.doublecloud.transfer.v1.endpoint.KafkaAuthR\x04\x61uth\x12\x1d\n\ntopic_name\x18\x04 \x01(\tR\ttopicName\x12@\n\x06parser\x18\x07 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.ParserR\x06parser\"\xd9\x02\n\x0bKafkaTarget\x12X\n\nconnection\x18\x01 \x01(\x0b\x32\x38.doublecloud.transfer.v1.endpoint.KafkaConnectionOptionsR\nconnection\x12?\n\x04\x61uth\x18\x02 \x01(\x0b\x32+.doublecloud.transfer.v1.endpoint.KafkaAuthR\x04\x61uth\x12\x61\n\x0etopic_settings\x18\x07 \x01(\x0b\x32:.doublecloud.transfer.v1.endpoint.KafkaTargetTopicSettingsR\rtopicSettings\x12L\n\nserializer\x18\x08 \x01(\x0b\x32,.doublecloud.transfer.v1.endpoint.SerializerR\nserializer\"\x9d\x01\n\x18KafkaTargetTopicSettings\x12J\n\x05topic\x18\x01 \x01(\x0b\x32\x32.doublecloud.transfer.v1.endpoint.KafkaTargetTopicH\x00R\x05topic\x12#\n\x0ctopic_prefix\x18\x02 \x01(\tH\x00R\x0btopicPrefixB\x10\n\x0etopic_settings\"U\n\x10KafkaTargetTopic\x12\x1d\n\ntopic_name\x18\x01 \x01(\tR\ttopicName\x12\"\n\rsave_tx_order\x18\x02 \x01(\x08R\x0bsaveTxOrder*i\n\x0eKafkaMechanism\x12\x1f\n\x1bKAFKA_MECHANISM_UNSPECIFIED\x10\x00\x12\x1a\n\x16KAFKA_MECHANISM_SHA256\x10\x01\x12\x1a\n\x16KAFKA_MECHANISM_SHA512\x10\x02\x42NZLgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint;endpointb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint.kafka_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZLgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint;endpoint'
-  _globals['_KAFKAMECHANISM']._serialized_start=1602
-  _globals['_KAFKAMECHANISM']._serialized_end=1707
-  _globals['_KAFKACONNECTIONOPTIONS']._serialized_start=178
-  _globals['_KAFKACONNECTIONOPTIONS']._serialized_end=332
-  _globals['_ONPREMISEKAFKA']._serialized_start=334
-  _globals['_ONPREMISEKAFKA']._serialized_end=453
-  _globals['_KAFKAAUTH']._serialized_start=456
-  _globals['_KAFKAAUTH']._serialized_end=623
-  _globals['_KAFKASASLSECURITY']._serialized_start=626
-  _globals['_KAFKASASLSECURITY']._serialized_end=815
-  _globals['_KAFKASOURCE']._serialized_start=818
-  _globals['_KAFKASOURCE']._serialized_end=1083
-  _globals['_KAFKATARGET']._serialized_start=1086
-  _globals['_KAFKATARGET']._serialized_end=1353
-  _globals['_KAFKATARGETTOPICSETTINGS']._serialized_start=1356
-  _globals['_KAFKATARGETTOPICSETTINGS']._serialized_end=1513
-  _globals['_KAFKATARGETTOPIC']._serialized_start=1515
-  _globals['_KAFKATARGETTOPIC']._serialized_end=1600
+  _globals['_KAFKAMECHANISM']._serialized_start=1732
+  _globals['_KAFKAMECHANISM']._serialized_end=1837
+  _globals['_KAFKACONNECTIONOPTIONS']._serialized_start=230
+  _globals['_KAFKACONNECTIONOPTIONS']._serialized_end=384
+  _globals['_ONPREMISEKAFKA']._serialized_start=386
+  _globals['_ONPREMISEKAFKA']._serialized_end=505
+  _globals['_KAFKAAUTH']._serialized_start=508
+  _globals['_KAFKAAUTH']._serialized_end=675
+  _globals['_KAFKASASLSECURITY']._serialized_start=678
+  _globals['_KAFKASASLSECURITY']._serialized_end=867
+  _globals['_KAFKASOURCE']._serialized_start=870
+  _globals['_KAFKASOURCE']._serialized_end=1135
+  _globals['_KAFKATARGET']._serialized_start=1138
+  _globals['_KAFKATARGET']._serialized_end=1483
+  _globals['_KAFKATARGETTOPICSETTINGS']._serialized_start=1486
+  _globals['_KAFKATARGETTOPICSETTINGS']._serialized_end=1643
+  _globals['_KAFKATARGETTOPIC']._serialized_start=1645
+  _globals['_KAFKATARGETTOPIC']._serialized_end=1730
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/kafka_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/kafka_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from doublecloud.transfer.v1.endpoint import common_pb2 as _common_pb2
 from doublecloud.transfer.v1.endpoint import parsers_pb2 as _parsers_pb2
+from doublecloud.transfer.v1.endpoint import serializers_pb2 as _serializers_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
@@ -60,22 +61,24 @@
     connection: KafkaConnectionOptions
     auth: KafkaAuth
     topic_name: str
     parser: _parsers_pb2.Parser
     def __init__(self, connection: _Optional[_Union[KafkaConnectionOptions, _Mapping]] = ..., auth: _Optional[_Union[KafkaAuth, _Mapping]] = ..., topic_name: _Optional[str] = ..., parser: _Optional[_Union[_parsers_pb2.Parser, _Mapping]] = ...) -> None: ...
 
 class KafkaTarget(_message.Message):
-    __slots__ = ["connection", "auth", "topic_settings"]
+    __slots__ = ["connection", "auth", "topic_settings", "serializer"]
     CONNECTION_FIELD_NUMBER: _ClassVar[int]
     AUTH_FIELD_NUMBER: _ClassVar[int]
     TOPIC_SETTINGS_FIELD_NUMBER: _ClassVar[int]
+    SERIALIZER_FIELD_NUMBER: _ClassVar[int]
     connection: KafkaConnectionOptions
     auth: KafkaAuth
     topic_settings: KafkaTargetTopicSettings
-    def __init__(self, connection: _Optional[_Union[KafkaConnectionOptions, _Mapping]] = ..., auth: _Optional[_Union[KafkaAuth, _Mapping]] = ..., topic_settings: _Optional[_Union[KafkaTargetTopicSettings, _Mapping]] = ...) -> None: ...
+    serializer: _serializers_pb2.Serializer
+    def __init__(self, connection: _Optional[_Union[KafkaConnectionOptions, _Mapping]] = ..., auth: _Optional[_Union[KafkaAuth, _Mapping]] = ..., topic_settings: _Optional[_Union[KafkaTargetTopicSettings, _Mapping]] = ..., serializer: _Optional[_Union[_serializers_pb2.Serializer, _Mapping]] = ...) -> None: ...
 
 class KafkaTargetTopicSettings(_message.Message):
     __slots__ = ["topic", "topic_prefix"]
     TOPIC_FIELD_NUMBER: _ClassVar[int]
     TOPIC_PREFIX_FIELD_NUMBER: _ClassVar[int]
     topic: KafkaTargetTopic
     topic_prefix: str
```

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/mongo_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mongo_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/mongo_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mongo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/mysql_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mysql_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/parsers_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/parsers_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/parsers_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/parsers_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/postgres_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/postgres_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/postgres_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/postgres_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_service_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_service_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_service_pb2_grpc.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/operation_service_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/operation_service_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/operation_service_pb2_grpc.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/transfer_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/transfer_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/transfer_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/transfer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/transfer_service_pb2.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/transfer_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/transfer_service_pb2.pyi` & `doublecloud-0.7.0/doublecloud/transfer/v1/transfer_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/transfer/v1/transfer_service_pb2_grpc.py` & `doublecloud-0.7.0/doublecloud/transfer/v1/transfer_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/v1/cluster_pb2.py` & `doublecloud-0.7.0/doublecloud/v1/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/v1/cluster_pb2.pyi` & `doublecloud-0.7.0/doublecloud/v1/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/v1/maintenance_pb2.py` & `doublecloud-0.7.0/doublecloud/v1/maintenance_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/v1/maintenance_pb2.pyi` & `doublecloud-0.7.0/doublecloud/v1/maintenance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/v1/operation_pb2.py` & `doublecloud-0.7.0/doublecloud/v1/operation_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/v1/operation_pb2.pyi` & `doublecloud-0.7.0/doublecloud/v1/operation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/v1/paging_pb2.py` & `doublecloud-0.7.0/doublecloud/v1/paging_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/v1/paging_pb2.pyi` & `doublecloud-0.7.0/doublecloud/v1/paging_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/visualization/v1/workbook_pb2.py` & `doublecloud-0.7.0/doublecloud/visualization/v1/workbook_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/visualization/v1/workbook_pb2.pyi` & `doublecloud-0.7.0/doublecloud/visualization/v1/workbook_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/visualization/v1/workbook_service_pb2.py` & `doublecloud-0.7.0/doublecloud/visualization/v1/workbook_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/visualization/v1/workbook_service_pb2.pyi` & `doublecloud-0.7.0/doublecloud/visualization/v1/workbook_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud/visualization/v1/workbook_service_pb2_grpc.py` & `doublecloud-0.7.0/doublecloud/visualization/v1/workbook_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/doublecloud.egg-info/PKG-INFO` & `doublecloud-0.7.0/doublecloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doublecloud
-Version: 0.6.0
+Version: 0.7.0
 Summary: The Double.Cloud official SDK
 Home-page: https://github.com/doublecloud/python-sdk
 Author: DoubleCloud GmbH
 Author-email: support@double.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doublecloud-0.6.0/doublecloud.egg-info/SOURCES.txt` & `doublecloud-0.7.0/doublecloud.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,17 @@
 doublecloud/transfer/v1/endpoint/mysql_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/parsers_pb2.py
 doublecloud/transfer/v1/endpoint/parsers_pb2.pyi
 doublecloud/transfer/v1/endpoint/parsers_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/postgres_pb2.py
 doublecloud/transfer/v1/endpoint/postgres_pb2.pyi
 doublecloud/transfer/v1/endpoint/postgres_pb2_grpc.py
+doublecloud/transfer/v1/endpoint/serializers_pb2.py
+doublecloud/transfer/v1/endpoint/serializers_pb2.pyi
+doublecloud/transfer/v1/endpoint/serializers_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/airbyte/__init__.py
 doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.py
 doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.pyi
 doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.py
 doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.pyi
 doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2_grpc.py
```

### Comparing `doublecloud-0.6.0/pyproject.toml` & `doublecloud-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doublecloud-0.6.0/setup.py` & `doublecloud-0.7.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 packages = find_packages(".", include=["doublecloud*"])
 
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 
 setup(
     name="doublecloud",
     version=__version__,
     description="The Double.Cloud official SDK",
     url="https://github.com/doublecloud/python-sdk",
     author="DoubleCloud GmbH",
```

