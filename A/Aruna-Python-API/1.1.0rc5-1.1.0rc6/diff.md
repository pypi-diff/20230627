# Comparing `tmp/Aruna-Python-API-1.1.0rc5.tar.gz` & `tmp/Aruna-Python-API-1.1.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Aruna-Python-API-1.1.0rc5.tar", last modified: Thu Jun 22 18:53:03 2023, max compression
+gzip compressed data, was "Aruna-Python-API-1.1.0rc6.tar", last modified: Tue Jun 27 06:58:53 2023, max compression
```

## Comparing `Aruna-Python-API-1.1.0rc5.tar` & `Aruna-Python-API-1.1.0rc6.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.386815 Aruna-Python-API-1.1.0rc5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.378815 Aruna-Python-API-1.1.0rc5/Aruna_Python_API.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-22 18:53:03.000000 Aruna-Python-API-1.1.0rc5/Aruna_Python_API.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-22 18:53:03.000000 Aruna-Python-API-1.1.0rc5/Aruna_Python_API.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:53:03.000000 Aruna-Python-API-1.1.0rc5/Aruna_Python_API.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-22 18:53:03.000000 Aruna-Python-API-1.1.0rc5/Aruna_Python_API.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 18:53:03.000000 Aruna-Python-API-1.1.0rc5/Aruna_Python_API.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-22 18:53:03.386815 Aruna-Python-API-1.1.0rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.378815 Aruna-Python-API-1.1.0rc5/aruna/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.378815 Aruna-Python-API-1.1.0rc5/aruna/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.378815 Aruna-Python-API-1.1.0rc5/aruna/api/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.382815 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/authorize_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/authorize_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/authorize_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/bundler_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/bundler_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/bundler_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/notification_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/notification_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/notification_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/proxy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/proxy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/proxy_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.382815 Aruna-Python-API-1.1.0rc5/aruna/api/notification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/notification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.382815 Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.382815 Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/v1/notification_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/v1/notification_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/v1/notification_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.382815 Aruna-Python-API-1.1.0rc5/aruna/api/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.382815 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.382815 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/auth_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/models_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21174 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/models_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/models_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/query_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/query_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/query_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.382815 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.386815 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/collection_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/collection_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/collection_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/endpoint_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/endpoint_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/info_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/info_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/info_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    31693 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/object_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25274 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/object_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    57329 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/object_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/objectgroup_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21104 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/project_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/project_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/project_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/service_account_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/service_account_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22042 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/user_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/user_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    29274 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/user_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 18:53:03.386815 Aruna-Python-API-1.1.0rc5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.157492 Aruna-Python-API-1.1.0rc6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.145492 Aruna-Python-API-1.1.0rc6/Aruna_Python_API.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-27 06:58:53.000000 Aruna-Python-API-1.1.0rc6/Aruna_Python_API.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-27 06:58:53.000000 Aruna-Python-API-1.1.0rc6/Aruna_Python_API.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 06:58:53.000000 Aruna-Python-API-1.1.0rc6/Aruna_Python_API.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-27 06:58:53.000000 Aruna-Python-API-1.1.0rc6/Aruna_Python_API.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 06:58:53.000000 Aruna-Python-API-1.1.0rc6/Aruna_Python_API.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-27 06:58:53.157492 Aruna-Python-API-1.1.0rc6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.145492 Aruna-Python-API-1.1.0rc6/aruna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.145492 Aruna-Python-API-1.1.0rc6/aruna/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.145492 Aruna-Python-API-1.1.0rc6/aruna/api/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.149492 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/authorize_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/authorize_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/authorize_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/bundler_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/bundler_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/bundler_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/notification_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/notification_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/notification_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/proxy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/proxy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/proxy_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.149492 Aruna-Python-API-1.1.0rc6/aruna/api/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/notification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.149492 Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.149492 Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/v1/notification_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/v1/notification_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/v1/notification_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.149492 Aruna-Python-API-1.1.0rc6/aruna/api/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.149492 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.149492 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/auth_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/models_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21174 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/models_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/models_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/query_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/query_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/query_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.149492 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:53.157492 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 06:58:21.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/collection_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/collection_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/collection_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/endpoint_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/endpoint_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/info_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/info_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/info_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/object_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25264 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/object_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/object_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/objectgroup_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21104 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/project_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/project_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/project_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/service_account_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/service_account_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22042 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/user_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/user_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    29274 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/user_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-27 06:58:53.157492 Aruna-Python-API-1.1.0rc6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-27 06:58:36.000000 Aruna-Python-API-1.1.0rc6/setup.py
```

### Comparing `Aruna-Python-API-1.1.0rc5/Aruna_Python_API.egg-info/PKG-INFO` & `Aruna-Python-API-1.1.0rc6/Aruna_Python_API.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aruna-Python-API
-Version: 1.1.0rc5
+Version: 1.1.0rc6
 Summary: Aruna Object Storage Python API builds
 Home-page: https://github.com/ArunaStorage/python-api
 Author: Marius Dieckmann, Jannis Hochmuth
 Author-email: marius.dieckmann@computational.bio.uni-giessen.de, jannis.hochmuth@computational.bio.uni-giessen.de
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Aruna-Python-API-1.1.0rc5/Aruna_Python_API.egg-info/SOURCES.txt` & `Aruna-Python-API-1.1.0rc6/Aruna_Python_API.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/LICENSE` & `Aruna-Python-API-1.1.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/PKG-INFO` & `Aruna-Python-API-1.1.0rc6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aruna-Python-API
-Version: 1.1.0rc5
+Version: 1.1.0rc6
 Summary: Aruna Object Storage Python API builds
 Home-page: https://github.com/ArunaStorage/python-api
 Author: Marius Dieckmann, Jannis Hochmuth
 Author-email: marius.dieckmann@computational.bio.uni-giessen.de, jannis.hochmuth@computational.bio.uni-giessen.de
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Aruna-Python-API-1.1.0rc5/README.md` & `Aruna-Python-API-1.1.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/authorize_pb2.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/authorize_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/authorize_pb2.pyi` & `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/authorize_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/authorize_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/authorize_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/bundler_pb2.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/bundler_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/bundler_pb2.pyi` & `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/bundler_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/bundler_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/bundler_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/notification_pb2.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/notification_pb2.pyi` & `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/notification_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/notification_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/proxy_pb2.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/proxy_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/proxy_pb2.pyi` & `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/proxy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/proxy_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/internal/v1/proxy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/v1/notification_service_pb2.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/v1/notification_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/v1/notification_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/v1/notification_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/v1/notification_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/notification/services/v1/notification_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/auth_pb2.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/auth_pb2.pyi` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/models_pb2.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/models_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/models_pb2.pyi` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/query_pb2.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/query_pb2.pyi` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/models/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/collection_service_pb2.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/collection_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/collection_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/collection_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/collection_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/collection_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/endpoint_service_pb2.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/endpoint_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/endpoint_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/endpoint_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/info_service_pb2.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/info_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/info_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/info_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/info_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/info_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/object_service_pb2.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/object_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 from aruna.api.storage.models.v1 import models_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_models__pb2
 from aruna.api.storage.models.v1 import query_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_query__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n2aruna/api/storage/services/v1/object_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a(aruna/api/storage/models/v1/models.proto\x1a\'aruna/api/storage/models/v1/query.proto\x1a\x1cgoogle/api/annotations.proto\"\x17\n\x03URL\x12\x10\n\x03url\x18\x01 \x01(\tR\x03url\"\xf0\x02\n\x0bStageObject\x12\x1a\n\x08\x66ilename\x18\x01 \x01(\tR\x08\x66ilename\x12\x1f\n\x0b\x63ontent_len\x18\x04 \x01(\x03R\ncontentLen\x12;\n\x06source\x18\x05 \x01(\x0b\x32#.aruna.api.storage.models.v1.SourceR\x06source\x12\x44\n\tdataclass\x18\x06 \x01(\x0e\x32&.aruna.api.storage.models.v1.DataClassR\tdataclass\x12=\n\x06labels\x18\x07 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x08 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12\x19\n\x08sub_path\x18\t \x01(\tR\x07subPathJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04\"\xb9\x02\n\x1aInitializeNewObjectRequest\x12\x42\n\x06object\x18\x01 \x01(\x0b\x32*.aruna.api.storage.services.v1.StageObjectR\x06object\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x32\n\x15preferred_endpoint_id\x18\x04 \x01(\tR\x13preferredEndpointId\x12\x1c\n\tmultipart\x18\x05 \x01(\x08R\tmultipart\x12)\n\x10is_specification\x18\x06 \x01(\x08R\x0fisSpecification\x12\x35\n\x04hash\x18\x07 \x01(\x0b\x32!.aruna.api.storage.models.v1.HashR\x04hash\"|\n\x1bInitializeNewObjectResponse\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12\x1b\n\tupload_id\x18\x02 \x01(\tR\x08uploadId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\"\xb3\x01\n\x13GetUploadURLRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12\x1b\n\tupload_id\x18\x02 \x01(\tR\x08uploadId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\x12\x1c\n\tmultipart\x18\x04 \x01(\x08R\tmultipart\x12\x1f\n\x0bpart_number\x18\x05 \x01(\x05R\npartNumber\"L\n\x14GetUploadURLResponse\x12\x34\n\x03url\x18\x01 \x01(\x0b\x32\".aruna.api.storage.services.v1.URLR\x03url\"8\n\x0e\x43ompletedParts\x12\x12\n\x04\x65tag\x18\x01 \x01(\tR\x04\x65tag\x12\x12\n\x04part\x18\x02 \x01(\x03R\x04part\"Y\n\x15GetDownloadURLRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\"N\n\x16GetDownloadURLResponse\x12\x34\n\x03url\x18\x01 \x01(\x0b\x32\".aruna.api.storage.services.v1.URLR\x03url\"]\n\x1cGetDownloadLinksBatchRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x18\n\x07objects\x18\x02 \x03(\tR\x07objects\"W\n\x1dGetDownloadLinksBatchResponse\x12\x36\n\x04urls\x18\x01 \x03(\x0b\x32\".aruna.api.storage.services.v1.URLR\x04urls\"a\n CreateDownloadLinksStreamRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x18\n\x07objects\x18\x02 \x03(\tR\x07objects\"Y\n!CreateDownloadLinksStreamResponse\x12\x34\n\x03url\x18\x01 \x01(\x0b\x32\".aruna.api.storage.services.v1.URLR\x03url\"\xc8\x02\n\x1a\x46inishObjectStagingRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12\x1b\n\tupload_id\x18\x02 \x01(\tR\x08uploadId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\x12\x35\n\x04hash\x18\x04 \x01(\x0b\x32!.aruna.api.storage.models.v1.HashR\x04hash\x12\x1b\n\tno_upload\x18\x05 \x01(\x08R\x08noUpload\x12V\n\x0f\x63ompleted_parts\x18\x06 \x03(\x0b\x32-.aruna.api.storage.services.v1.CompletedPartsR\x0e\x63ompletedParts\x12\x1f\n\x0b\x61uto_update\x18\x07 \x01(\x08R\nautoUpdate\"Z\n\x1b\x46inishObjectStagingResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\"\xf2\x02\n\x13UpdateObjectRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x42\n\x06object\x18\x03 \x01(\x0b\x32*.aruna.api.storage.services.v1.StageObjectR\x06object\x12\x1a\n\x08reupload\x18\x04 \x01(\x08R\x08reupload\x12\x32\n\x15preferred_endpoint_id\x18\x05 \x01(\tR\x13preferredEndpointId\x12\x1d\n\nmulti_part\x18\x06 \x01(\x08R\tmultiPart\x12)\n\x10is_specification\x18\x07 \x01(\x08R\x0fisSpecification\x12\x35\n\x04hash\x18\t \x01(\x0b\x32!.aruna.api.storage.models.v1.HashR\x04hashJ\x04\x08\x08\x10\t\"w\n\x14UpdateObjectResponse\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12\x1d\n\nstaging_id\x18\x02 \x01(\tR\tstagingId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\"\xec\x01\n\x1c\x43reateObjectReferenceRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x30\n\x14target_collection_id\x18\x03 \x01(\tR\x12targetCollectionId\x12\x1c\n\twriteable\x18\x04 \x01(\x08R\twriteable\x12\x1f\n\x0b\x61uto_update\x18\x05 \x01(\x08R\nautoUpdate\x12\x19\n\x08sub_path\x18\x06 \x01(\tR\x07subPath\"\x1f\n\x1d\x43reateObjectReferenceResponse\"\x88\x01\n\x12\x43loneObjectRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x30\n\x14target_collection_id\x18\x03 \x01(\tR\x12targetCollectionId\"R\n\x13\x43loneObjectResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\"\x94\x01\n\x13\x44\x65leteObjectRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12%\n\x0ewith_revisions\x18\x03 \x01(\x08R\rwithRevisions\x12\x14\n\x05\x66orce\x18\x04 \x01(\x08R\x05\x66orce\"\x16\n\x14\x44\x65leteObjectResponse\"\x97\x01\n\x14\x44\x65leteObjectsRequest\x12\x1d\n\nobject_ids\x18\x01 \x03(\tR\tobjectIds\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12%\n\x0ewith_revisions\x18\x03 \x01(\x08R\rwithRevisions\x12\x14\n\x05\x66orce\x18\x04 \x01(\x08R\x05\x66orce\"\x17\n\x15\x44\x65leteObjectsResponse\"t\n\rObjectWithURL\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\x12\x10\n\x03url\x18\x02 \x01(\tR\x03url\x12\x14\n\x05paths\x18\x03 \x03(\tR\x05paths\"s\n\x14GetObjectByIDRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12\x19\n\x08with_url\x18\x04 \x01(\x08R\x07withUrl\"]\n\x15GetObjectByIDResponse\x12\x44\n\x06object\x18\x01 \x01(\x0b\x32,.aruna.api.storage.services.v1.ObjectWithURLR\x06object\"\xf5\x01\n\x11GetObjectsRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12K\n\x0cpage_request\x18\x02 \x01(\x0b\x32(.aruna.api.storage.models.v1.PageRequestR\x0bpageRequest\x12S\n\x0flabel_id_filter\x18\x03 \x01(\x0b\x32+.aruna.api.storage.models.v1.LabelOrIDQueryR\rlabelIdFilter\x12\x19\n\x08with_url\x18\x04 \x01(\x08R\x07withUrl\"\\\n\x12GetObjectsResponse\x12\x46\n\x07objects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.services.v1.ObjectWithURLR\x07objects\"\xc5\x01\n\x19GetObjectRevisionsRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12K\n\x0cpage_request\x18\x03 \x01(\x0b\x32(.aruna.api.storage.models.v1.PageRequestR\x0bpageRequest\x12\x19\n\x08with_url\x18\x04 \x01(\x08R\x07withUrl\"d\n\x1aGetObjectRevisionsResponse\x12\x46\n\x07objects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.services.v1.ObjectWithURLR\x07objects\"}\n\x1eGetLatestObjectRevisionRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12\x19\n\x08with_url\x18\x03 \x01(\x08R\x07withUrl\"g\n\x1fGetLatestObjectRevisionResponse\x12\x44\n\x06object\x18\x01 \x01(\x0b\x32,.aruna.api.storage.services.v1.ObjectWithURLR\x06object\"]\n\x19GetObjectEndpointsRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\"a\n\x1aGetObjectEndpointsResponse\x12\x43\n\tendpoints\x18\x01 \x03(\x0b\x32%.aruna.api.storage.models.v1.EndpointR\tendpoints\"\xa7\x01\n\x18\x41\x64\x64LabelsToObjectRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12I\n\rlabels_to_add\x18\x03 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x0blabelsToAdd\"X\n\x19\x41\x64\x64LabelsToObjectResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\"\x98\x01\n\x17SetHooksOfObjectRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12;\n\x05hooks\x18\x03 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\"W\n\x18SetHooksOfObjectResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\"\x7f\n\x14GetReferencesRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12%\n\x0ewith_revisions\x18\x03 \x01(\x08R\rwithRevisions\"\x9f\x01\n\x0fObjectReference\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\'\n\x0frevision_number\x18\x03 \x01(\x03R\x0erevisionNumber\x12!\n\x0cis_writeable\x18\x04 \x01(\x08R\x0bisWriteable\"g\n\x15GetReferencesResponse\x12N\n\nreferences\x18\x01 \x03(\x0b\x32..aruna.api.storage.services.v1.ObjectReferenceR\nreferences\":\n\x04Path\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x1e\n\nvisibility\x18\x02 \x01(\x08R\nvisibility\"\x83\x01\n\x14GetObjectPathRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12)\n\x10include_inactive\x18\x03 \x01(\x08R\x0fincludeInactive\"_\n\x15GetObjectPathResponse\x12\x46\n\x0cobject_paths\x18\x01 \x03(\x0b\x32#.aruna.api.storage.services.v1.PathR\x0bobjectPaths\"g\n\x15GetObjectPathsRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12)\n\x10include_inactive\x18\x02 \x01(\x08R\x0fincludeInactive\"`\n\x16GetObjectPathsResponse\x12\x46\n\x0cobject_paths\x18\x01 \x03(\x0b\x32#.aruna.api.storage.services.v1.PathR\x0bobjectPaths\"v\n\x17\x43reateObjectPathRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12\x19\n\x08sub_path\x18\x03 \x01(\tR\x07subPath\"S\n\x18\x43reateObjectPathResponse\x12\x37\n\x04path\x18\x01 \x01(\x0b\x32#.aruna.api.storage.services.v1.PathR\x04path\"y\n\x1eSetObjectPathVisibilityRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x12\n\x04path\x18\x02 \x01(\tR\x04path\x12\x1e\n\nvisibility\x18\x03 \x01(\x08R\nvisibility\"Z\n\x1fSetObjectPathVisibilityResponse\x12\x37\n\x04path\x18\x01 \x01(\x0b\x32#.aruna.api.storage.services.v1.PathR\x04path\"T\n\x17GetObjectsByPathRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12%\n\x0ewith_revisions\x18\x02 \x01(\x08R\rwithRevisions\":\n$GetProjectCollectionIdsByPathRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\"k\n%GetProjectCollectionIdsByPathResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\"W\n\x18GetObjectsByPathResponse\x12;\n\x06object\x18\x03 \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\"\xba\x02\n\x19GetObjectsAsListV2Request\x12\x16\n\x06\x62ucket\x18\x01 \x01(\tR\x06\x62ucket\x12\x32\n\x12\x63ontinuation_token\x18\x02 \x01(\tH\x00R\x11\x63ontinuationToken\x88\x01\x01\x12!\n\tdelimiter\x18\x03 \x01(\tH\x01R\tdelimiter\x88\x01\x01\x12\x1e\n\x08max_keys\x18\x04 \x01(\rH\x02R\x07maxKeys\x88\x01\x01\x12\x1b\n\x06prefix\x18\x05 \x01(\tH\x03R\x06prefix\x88\x01\x01\x12$\n\x0bstart_after\x18\x06 \x01(\tH\x04R\nstartAfter\x88\x01\x01\x42\x15\n\x13_continuation_tokenB\x0c\n\n_delimiterB\x0b\n\t_max_keysB\t\n\x07_prefixB\x0e\n\x0c_start_after\"&\n\x0c\x43ommonPrefix\x12\x16\n\x06prefix\x18\x01 \x01(\tR\x06prefix\"\xee\x02\n\x1aGetObjectsAsListV2Response\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12!\n\x0cis_truncated\x18\x02 \x01(\x08R\x0bisTruncated\x12\x19\n\x08max_keys\x18\x04 \x01(\rR\x07maxKeys\x12\x1b\n\tkey_count\x18\x05 \x01(\rR\x08keyCount\x12?\n\x08\x63ontents\x18\x06 \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x08\x63ontents\x12G\n\x08prefixes\x18\x07 \x03(\x0b\x32+.aruna.api.storage.services.v1.CommonPrefixR\x08prefixes\x12;\n\x17next_continuation_token\x18\x08 \x01(\tH\x00R\x15nextContinuationToken\x88\x01\x01\x42\x1a\n\x18_next_continuation_token2\xc6(\n\rObjectService\x12\xbe\x01\n\x13InitializeNewObject\x12\x39.aruna.api.storage.services.v1.InitializeNewObjectRequest\x1a:.aruna.api.storage.services.v1.InitializeNewObjectResponse\"0\x82\xd3\xe4\x93\x02*:\x01*\"%/v1/collection/{collection_id}/object\x12\xcd\x01\n\x0cGetUploadURL\x12\x32.aruna.api.storage.services.v1.GetUploadURLRequest\x1a\x33.aruna.api.storage.services.v1.GetUploadURLResponse\"T\x82\xd3\xe4\x93\x02N\x12L/v1/collection/{collection_id}/object/{object_id}/staging/{upload_id}/upload\x12\xc1\x01\n\x0eGetDownloadURL\x12\x34.aruna.api.storage.services.v1.GetDownloadURLRequest\x1a\x35.aruna.api.storage.services.v1.GetDownloadURLResponse\"B\x82\xd3\xe4\x93\x02<\x12:/v1/collection/{collection_id}/object/{object_id}/download\x12\xc8\x01\n\x15GetDownloadLinksBatch\x12;.aruna.api.storage.services.v1.GetDownloadLinksBatchRequest\x1a<.aruna.api.storage.services.v1.GetDownloadLinksBatchResponse\"4\x82\xd3\xe4\x93\x02.\x12,/v1/collection/{collection_id}/objects/batch\x12\xda\x01\n\x19\x43reateDownloadLinksStream\x12?.aruna.api.storage.services.v1.CreateDownloadLinksStreamRequest\x1a@.aruna.api.storage.services.v1.CreateDownloadLinksStreamResponse\"8\x82\xd3\xe4\x93\x02\x32:\x01*\"-/v1/collection/{collection_id}/objects/stream0\x01\x12\xe5\x01\n\x13\x46inishObjectStaging\x12\x39.aruna.api.storage.services.v1.FinishObjectStagingRequest\x1a:.aruna.api.storage.services.v1.FinishObjectStagingResponse\"W\x82\xd3\xe4\x93\x02Q:\x01*2L/v1/collection/{collection_id}/object/{object_id}/staging/{upload_id}/finish\x12\xbc\x01\n\x0cUpdateObject\x12\x32.aruna.api.storage.services.v1.UpdateObjectRequest\x1a\x33.aruna.api.storage.services.v1.UpdateObjectResponse\"C\x82\xd3\xe4\x93\x02=:\x01*\"8/v1/collection/{collection_id}/object/{object_id}/update\x12\xf1\x01\n\x15\x43reateObjectReference\x12;.aruna.api.storage.services.v1.CreateObjectReferenceRequest\x1a<.aruna.api.storage.services.v1.CreateObjectReferenceResponse\"]\x82\xd3\xe4\x93\x02W:\x01*\"R/v1/collection/{collection_id}/object/{object_id}/reference/{target_collection_id}\x12\xb8\x01\n\x0b\x43loneObject\x12\x31.aruna.api.storage.services.v1.CloneObjectRequest\x1a\x32.aruna.api.storage.services.v1.CloneObjectResponse\"B\x82\xd3\xe4\x93\x02<:\x01*\"7/v1/collection/{collection_id}/object/{object_id}/clone\x12\xb5\x01\n\x0c\x44\x65leteObject\x12\x32.aruna.api.storage.services.v1.DeleteObjectRequest\x1a\x33.aruna.api.storage.services.v1.DeleteObjectResponse\"<\x82\xd3\xe4\x93\x02\x36:\x01**1/v1/collection/{collection_id}/object/{object_id}\x12\xad\x01\n\rDeleteObjects\x12\x33.aruna.api.storage.services.v1.DeleteObjectsRequest\x1a\x34.aruna.api.storage.services.v1.DeleteObjectsResponse\"1\x82\xd3\xe4\x93\x02+:\x01**&/v1/collection/{collection_id}/objects\x12\xb5\x01\n\rGetObjectByID\x12\x33.aruna.api.storage.services.v1.GetObjectByIDRequest\x1a\x34.aruna.api.storage.services.v1.GetObjectByIDResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/v1/collection/{collection_id}/object/{object_id}\x12\xa1\x01\n\nGetObjects\x12\x30.aruna.api.storage.services.v1.GetObjectsRequest\x1a\x31.aruna.api.storage.services.v1.GetObjectsResponse\".\x82\xd3\xe4\x93\x02(\x12&/v1/collection/{collection_id}/objects\x12\xce\x01\n\x12GetObjectRevisions\x12\x38.aruna.api.storage.services.v1.GetObjectRevisionsRequest\x1a\x39.aruna.api.storage.services.v1.GetObjectRevisionsResponse\"C\x82\xd3\xe4\x93\x02=\x12;/v1/collection/{collection_id}/object/{object_id}/revisions\x12\xda\x01\n\x17GetLatestObjectRevision\x12=.aruna.api.storage.services.v1.GetLatestObjectRevisionRequest\x1a>.aruna.api.storage.services.v1.GetLatestObjectRevisionResponse\"@\x82\xd3\xe4\x93\x02:\x12\x38/v1/collection/{collection_id}/object/{object_id}/latest\x12\xce\x01\n\x12GetObjectEndpoints\x12\x38.aruna.api.storage.services.v1.GetObjectEndpointsRequest\x1a\x39.aruna.api.storage.services.v1.GetObjectEndpointsResponse\"C\x82\xd3\xe4\x93\x02=\x12;/v1/collection/{collection_id}/object/{object_id}/endpoints\x12\xcf\x01\n\x11\x41\x64\x64LabelsToObject\x12\x37.aruna.api.storage.services.v1.AddLabelsToObjectRequest\x1a\x38.aruna.api.storage.services.v1.AddLabelsToObjectResponse\"G\x82\xd3\xe4\x93\x02\x41:\x01*2</v1/collection/{collection_id}/object/{object_id}/add_labels\x12\xcb\x01\n\x10SetHooksOfObject\x12\x36.aruna.api.storage.services.v1.SetHooksOfObjectRequest\x1a\x37.aruna.api.storage.services.v1.SetHooksOfObjectResponse\"F\x82\xd3\xe4\x93\x02@:\x01*2;/v1/collection/{collection_id}/object/{object_id}/set_hooks\x12\xc0\x01\n\rGetReferences\x12\x33.aruna.api.storage.services.v1.GetReferencesRequest\x1a\x34.aruna.api.storage.services.v1.GetReferencesResponse\"D\x82\xd3\xe4\x93\x02>\x12</v1/collection/{collection_id}/object/{object_id}/references\x12\xba\x01\n\rGetObjectPath\x12\x33.aruna.api.storage.services.v1.GetObjectPathRequest\x1a\x34.aruna.api.storage.services.v1.GetObjectPathResponse\">\x82\xd3\xe4\x93\x02\x38\x12\x36/v1/collection/{collection_id}/object/{object_id}/path\x12\xab\x01\n\x0eGetObjectPaths\x12\x34.aruna.api.storage.services.v1.GetObjectPathsRequest\x1a\x35.aruna.api.storage.services.v1.GetObjectPathsResponse\",\x82\xd3\xe4\x93\x02&\x12$/v1/collection/{collection_id}/paths\x12\xc6\x01\n\x10\x43reateObjectPath\x12\x36.aruna.api.storage.services.v1.CreateObjectPathRequest\x1a\x37.aruna.api.storage.services.v1.CreateObjectPathResponse\"A\x82\xd3\xe4\x93\x02;:\x01*\"6/v1/collection/{collection_id}/object/{object_id}/path\x12\xdd\x01\n\x17SetObjectPathVisibility\x12=.aruna.api.storage.services.v1.SetObjectPathVisibilityRequest\x1a>.aruna.api.storage.services.v1.SetObjectPathVisibilityResponse\"C\x82\xd3\xe4\x93\x02=:\x01*28/v1/collection/{collection_id}/path/{path=**}/visibility\x12\xa6\x01\n\x10GetObjectsByPath\x12\x36.aruna.api.storage.services.v1.GetObjectsByPathRequest\x1a\x37.aruna.api.storage.services.v1.GetObjectsByPathResponse\"!\x82\xd3\xe4\x93\x02\x1b\x12\x19/v1/path/object/{path=**}\x12\xd1\x01\n\x1dGetProjectCollectionIdsByPath\x12\x43.aruna.api.storage.services.v1.GetProjectCollectionIdsByPathRequest\x1a\x44.aruna.api.storage.services.v1.GetProjectCollectionIdsByPathResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/v1/path/collection/{path=**}\x12\xaa\x01\n\x12GetObjectsAsListV2\x12\x38.aruna.api.storage.services.v1.GetObjectsAsListV2Request\x1a\x39.aruna.api.storage.services.v1.GetObjectsAsListV2Response\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/v1/path/objects/listv2B\x8f\x01\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\rObjectServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n2aruna/api/storage/services/v1/object_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a(aruna/api/storage/models/v1/models.proto\x1a\'aruna/api/storage/models/v1/query.proto\x1a\x1cgoogle/api/annotations.proto\"\x17\n\x03URL\x12\x10\n\x03url\x18\x01 \x01(\tR\x03url\"\xf0\x02\n\x0bStageObject\x12\x1a\n\x08\x66ilename\x18\x01 \x01(\tR\x08\x66ilename\x12\x1f\n\x0b\x63ontent_len\x18\x04 \x01(\x03R\ncontentLen\x12;\n\x06source\x18\x05 \x01(\x0b\x32#.aruna.api.storage.models.v1.SourceR\x06source\x12\x44\n\tdataclass\x18\x06 \x01(\x0e\x32&.aruna.api.storage.models.v1.DataClassR\tdataclass\x12=\n\x06labels\x18\x07 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x08 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12\x19\n\x08sub_path\x18\t \x01(\tR\x07subPathJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04\"\xb9\x02\n\x1aInitializeNewObjectRequest\x12\x42\n\x06object\x18\x01 \x01(\x0b\x32*.aruna.api.storage.services.v1.StageObjectR\x06object\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x32\n\x15preferred_endpoint_id\x18\x04 \x01(\tR\x13preferredEndpointId\x12\x1c\n\tmultipart\x18\x05 \x01(\x08R\tmultipart\x12)\n\x10is_specification\x18\x06 \x01(\x08R\x0fisSpecification\x12\x35\n\x04hash\x18\x07 \x01(\x0b\x32!.aruna.api.storage.models.v1.HashR\x04hash\"|\n\x1bInitializeNewObjectResponse\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12\x1b\n\tupload_id\x18\x02 \x01(\tR\x08uploadId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\"\xb3\x01\n\x13GetUploadURLRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12\x1b\n\tupload_id\x18\x02 \x01(\tR\x08uploadId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\x12\x1c\n\tmultipart\x18\x04 \x01(\x08R\tmultipart\x12\x1f\n\x0bpart_number\x18\x05 \x01(\x05R\npartNumber\"L\n\x14GetUploadURLResponse\x12\x34\n\x03url\x18\x01 \x01(\x0b\x32\".aruna.api.storage.services.v1.URLR\x03url\"8\n\x0e\x43ompletedParts\x12\x12\n\x04\x65tag\x18\x01 \x01(\tR\x04\x65tag\x12\x12\n\x04part\x18\x02 \x01(\x03R\x04part\"Y\n\x15GetDownloadURLRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\"N\n\x16GetDownloadURLResponse\x12\x34\n\x03url\x18\x01 \x01(\x0b\x32\".aruna.api.storage.services.v1.URLR\x03url\"]\n\x1cGetDownloadLinksBatchRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x18\n\x07objects\x18\x02 \x03(\tR\x07objects\"W\n\x1dGetDownloadLinksBatchResponse\x12\x36\n\x04urls\x18\x01 \x03(\x0b\x32\".aruna.api.storage.services.v1.URLR\x04urls\"a\n CreateDownloadLinksStreamRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x18\n\x07objects\x18\x02 \x03(\tR\x07objects\"Y\n!CreateDownloadLinksStreamResponse\x12\x34\n\x03url\x18\x01 \x01(\x0b\x32\".aruna.api.storage.services.v1.URLR\x03url\"\xc8\x02\n\x1a\x46inishObjectStagingRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12\x1b\n\tupload_id\x18\x02 \x01(\tR\x08uploadId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\x12\x35\n\x04hash\x18\x04 \x01(\x0b\x32!.aruna.api.storage.models.v1.HashR\x04hash\x12\x1b\n\tno_upload\x18\x05 \x01(\x08R\x08noUpload\x12V\n\x0f\x63ompleted_parts\x18\x06 \x03(\x0b\x32-.aruna.api.storage.services.v1.CompletedPartsR\x0e\x63ompletedParts\x12\x1f\n\x0b\x61uto_update\x18\x07 \x01(\x08R\nautoUpdate\"Z\n\x1b\x46inishObjectStagingResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\"\xf2\x02\n\x13UpdateObjectRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x42\n\x06object\x18\x03 \x01(\x0b\x32*.aruna.api.storage.services.v1.StageObjectR\x06object\x12\x1a\n\x08reupload\x18\x04 \x01(\x08R\x08reupload\x12\x32\n\x15preferred_endpoint_id\x18\x05 \x01(\tR\x13preferredEndpointId\x12\x1d\n\nmulti_part\x18\x06 \x01(\x08R\tmultiPart\x12)\n\x10is_specification\x18\x07 \x01(\x08R\x0fisSpecification\x12\x35\n\x04hash\x18\t \x01(\x0b\x32!.aruna.api.storage.models.v1.HashR\x04hashJ\x04\x08\x08\x10\t\"w\n\x14UpdateObjectResponse\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12\x1d\n\nstaging_id\x18\x02 \x01(\tR\tstagingId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\"\xec\x01\n\x1c\x43reateObjectReferenceRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x30\n\x14target_collection_id\x18\x03 \x01(\tR\x12targetCollectionId\x12\x1c\n\twriteable\x18\x04 \x01(\x08R\twriteable\x12\x1f\n\x0b\x61uto_update\x18\x05 \x01(\x08R\nautoUpdate\x12\x19\n\x08sub_path\x18\x06 \x01(\tR\x07subPath\"\x1f\n\x1d\x43reateObjectReferenceResponse\"\x88\x01\n\x12\x43loneObjectRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x30\n\x14target_collection_id\x18\x03 \x01(\tR\x12targetCollectionId\"R\n\x13\x43loneObjectResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\"\x94\x01\n\x13\x44\x65leteObjectRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12%\n\x0ewith_revisions\x18\x03 \x01(\x08R\rwithRevisions\x12\x14\n\x05\x66orce\x18\x04 \x01(\x08R\x05\x66orce\"\x16\n\x14\x44\x65leteObjectResponse\"\x97\x01\n\x14\x44\x65leteObjectsRequest\x12\x1d\n\nobject_ids\x18\x01 \x03(\tR\tobjectIds\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12%\n\x0ewith_revisions\x18\x03 \x01(\x08R\rwithRevisions\x12\x14\n\x05\x66orce\x18\x04 \x01(\x08R\x05\x66orce\"\x17\n\x15\x44\x65leteObjectsResponse\"t\n\rObjectWithURL\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\x12\x10\n\x03url\x18\x02 \x01(\tR\x03url\x12\x14\n\x05paths\x18\x03 \x03(\tR\x05paths\"s\n\x14GetObjectByIDRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12\x19\n\x08with_url\x18\x04 \x01(\x08R\x07withUrl\"]\n\x15GetObjectByIDResponse\x12\x44\n\x06object\x18\x01 \x01(\x0b\x32,.aruna.api.storage.services.v1.ObjectWithURLR\x06object\"\xf5\x01\n\x11GetObjectsRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12K\n\x0cpage_request\x18\x02 \x01(\x0b\x32(.aruna.api.storage.models.v1.PageRequestR\x0bpageRequest\x12S\n\x0flabel_id_filter\x18\x03 \x01(\x0b\x32+.aruna.api.storage.models.v1.LabelOrIDQueryR\rlabelIdFilter\x12\x19\n\x08with_url\x18\x04 \x01(\x08R\x07withUrl\"\\\n\x12GetObjectsResponse\x12\x46\n\x07objects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.services.v1.ObjectWithURLR\x07objects\"\xc5\x01\n\x19GetObjectRevisionsRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12K\n\x0cpage_request\x18\x03 \x01(\x0b\x32(.aruna.api.storage.models.v1.PageRequestR\x0bpageRequest\x12\x19\n\x08with_url\x18\x04 \x01(\x08R\x07withUrl\"d\n\x1aGetObjectRevisionsResponse\x12\x46\n\x07objects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.services.v1.ObjectWithURLR\x07objects\"}\n\x1eGetLatestObjectRevisionRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12\x19\n\x08with_url\x18\x03 \x01(\x08R\x07withUrl\"g\n\x1fGetLatestObjectRevisionResponse\x12\x44\n\x06object\x18\x01 \x01(\x0b\x32,.aruna.api.storage.services.v1.ObjectWithURLR\x06object\"]\n\x19GetObjectEndpointsRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\"a\n\x1aGetObjectEndpointsResponse\x12\x43\n\tendpoints\x18\x01 \x03(\x0b\x32%.aruna.api.storage.models.v1.EndpointR\tendpoints\"\xa7\x01\n\x18\x41\x64\x64LabelsToObjectRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12I\n\rlabels_to_add\x18\x03 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x0blabelsToAdd\"X\n\x19\x41\x64\x64LabelsToObjectResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\"\x98\x01\n\x17SetHooksOfObjectRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12;\n\x05hooks\x18\x03 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\"W\n\x18SetHooksOfObjectResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\"\x7f\n\x14GetReferencesRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12%\n\x0ewith_revisions\x18\x03 \x01(\x08R\rwithRevisions\"\x9f\x01\n\x0fObjectReference\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\'\n\x0frevision_number\x18\x03 \x01(\x03R\x0erevisionNumber\x12!\n\x0cis_writeable\x18\x04 \x01(\x08R\x0bisWriteable\"g\n\x15GetReferencesResponse\x12N\n\nreferences\x18\x01 \x03(\x0b\x32..aruna.api.storage.services.v1.ObjectReferenceR\nreferences\":\n\x04Path\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x1e\n\nvisibility\x18\x02 \x01(\x08R\nvisibility\"\x83\x01\n\x14GetObjectPathRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12)\n\x10include_inactive\x18\x03 \x01(\x08R\x0fincludeInactive\"_\n\x15GetObjectPathResponse\x12\x46\n\x0cobject_paths\x18\x01 \x03(\x0b\x32#.aruna.api.storage.services.v1.PathR\x0bobjectPaths\"g\n\x15GetObjectPathsRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12)\n\x10include_inactive\x18\x02 \x01(\x08R\x0fincludeInactive\"`\n\x16GetObjectPathsResponse\x12\x46\n\x0cobject_paths\x18\x01 \x03(\x0b\x32#.aruna.api.storage.services.v1.PathR\x0bobjectPaths\"v\n\x17\x43reateObjectPathRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12\x19\n\x08sub_path\x18\x03 \x01(\tR\x07subPath\"S\n\x18\x43reateObjectPathResponse\x12\x37\n\x04path\x18\x01 \x01(\x0b\x32#.aruna.api.storage.services.v1.PathR\x04path\"y\n\x1eSetObjectPathVisibilityRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x12\n\x04path\x18\x02 \x01(\tR\x04path\x12\x1e\n\nvisibility\x18\x03 \x01(\x08R\nvisibility\"Z\n\x1fSetObjectPathVisibilityResponse\x12\x37\n\x04path\x18\x01 \x01(\x0b\x32#.aruna.api.storage.services.v1.PathR\x04path\"T\n\x17GetObjectsByPathRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12%\n\x0ewith_revisions\x18\x02 \x01(\x08R\rwithRevisions\":\n$GetProjectCollectionIdsByPathRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\"k\n%GetProjectCollectionIdsByPathResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\"W\n\x18GetObjectsByPathResponse\x12;\n\x06object\x18\x03 \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\"\xba\x02\n\x19GetObjectsAsListV2Request\x12\x16\n\x06\x62ucket\x18\x01 \x01(\tR\x06\x62ucket\x12\x32\n\x12\x63ontinuation_token\x18\x02 \x01(\tH\x00R\x11\x63ontinuationToken\x88\x01\x01\x12!\n\tdelimiter\x18\x03 \x01(\tH\x01R\tdelimiter\x88\x01\x01\x12\x1e\n\x08max_keys\x18\x04 \x01(\rH\x02R\x07maxKeys\x88\x01\x01\x12\x1b\n\x06prefix\x18\x05 \x01(\tH\x03R\x06prefix\x88\x01\x01\x12$\n\x0bstart_after\x18\x06 \x01(\tH\x04R\nstartAfter\x88\x01\x01\x42\x15\n\x13_continuation_tokenB\x0c\n\n_delimiterB\x0b\n\t_max_keysB\t\n\x07_prefixB\x0e\n\x0c_start_after\"&\n\x0c\x43ommonPrefix\x12\x16\n\x06prefix\x18\x01 \x01(\tR\x06prefix\"\xf7\x02\n\x1aGetObjectsAsListV2Response\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12!\n\x0cis_truncated\x18\x02 \x01(\x08R\x0bisTruncated\x12\x19\n\x08max_keys\x18\x04 \x01(\rR\x07maxKeys\x12\x1b\n\tkey_count\x18\x05 \x01(\rR\x08keyCount\x12H\n\x08\x63ontents\x18\x06 \x03(\x0b\x32,.aruna.api.storage.services.v1.ObjectWithURLR\x08\x63ontents\x12G\n\x08prefixes\x18\x07 \x03(\x0b\x32+.aruna.api.storage.services.v1.CommonPrefixR\x08prefixes\x12;\n\x17next_continuation_token\x18\x08 \x01(\tH\x00R\x15nextContinuationToken\x88\x01\x01\x42\x1a\n\x18_next_continuation_token2\xc6(\n\rObjectService\x12\xbe\x01\n\x13InitializeNewObject\x12\x39.aruna.api.storage.services.v1.InitializeNewObjectRequest\x1a:.aruna.api.storage.services.v1.InitializeNewObjectResponse\"0\x82\xd3\xe4\x93\x02*:\x01*\"%/v1/collection/{collection_id}/object\x12\xcd\x01\n\x0cGetUploadURL\x12\x32.aruna.api.storage.services.v1.GetUploadURLRequest\x1a\x33.aruna.api.storage.services.v1.GetUploadURLResponse\"T\x82\xd3\xe4\x93\x02N\x12L/v1/collection/{collection_id}/object/{object_id}/staging/{upload_id}/upload\x12\xc1\x01\n\x0eGetDownloadURL\x12\x34.aruna.api.storage.services.v1.GetDownloadURLRequest\x1a\x35.aruna.api.storage.services.v1.GetDownloadURLResponse\"B\x82\xd3\xe4\x93\x02<\x12:/v1/collection/{collection_id}/object/{object_id}/download\x12\xc8\x01\n\x15GetDownloadLinksBatch\x12;.aruna.api.storage.services.v1.GetDownloadLinksBatchRequest\x1a<.aruna.api.storage.services.v1.GetDownloadLinksBatchResponse\"4\x82\xd3\xe4\x93\x02.\x12,/v1/collection/{collection_id}/objects/batch\x12\xda\x01\n\x19\x43reateDownloadLinksStream\x12?.aruna.api.storage.services.v1.CreateDownloadLinksStreamRequest\x1a@.aruna.api.storage.services.v1.CreateDownloadLinksStreamResponse\"8\x82\xd3\xe4\x93\x02\x32:\x01*\"-/v1/collection/{collection_id}/objects/stream0\x01\x12\xe5\x01\n\x13\x46inishObjectStaging\x12\x39.aruna.api.storage.services.v1.FinishObjectStagingRequest\x1a:.aruna.api.storage.services.v1.FinishObjectStagingResponse\"W\x82\xd3\xe4\x93\x02Q:\x01*2L/v1/collection/{collection_id}/object/{object_id}/staging/{upload_id}/finish\x12\xbc\x01\n\x0cUpdateObject\x12\x32.aruna.api.storage.services.v1.UpdateObjectRequest\x1a\x33.aruna.api.storage.services.v1.UpdateObjectResponse\"C\x82\xd3\xe4\x93\x02=:\x01*\"8/v1/collection/{collection_id}/object/{object_id}/update\x12\xf1\x01\n\x15\x43reateObjectReference\x12;.aruna.api.storage.services.v1.CreateObjectReferenceRequest\x1a<.aruna.api.storage.services.v1.CreateObjectReferenceResponse\"]\x82\xd3\xe4\x93\x02W:\x01*\"R/v1/collection/{collection_id}/object/{object_id}/reference/{target_collection_id}\x12\xb8\x01\n\x0b\x43loneObject\x12\x31.aruna.api.storage.services.v1.CloneObjectRequest\x1a\x32.aruna.api.storage.services.v1.CloneObjectResponse\"B\x82\xd3\xe4\x93\x02<:\x01*\"7/v1/collection/{collection_id}/object/{object_id}/clone\x12\xb5\x01\n\x0c\x44\x65leteObject\x12\x32.aruna.api.storage.services.v1.DeleteObjectRequest\x1a\x33.aruna.api.storage.services.v1.DeleteObjectResponse\"<\x82\xd3\xe4\x93\x02\x36:\x01**1/v1/collection/{collection_id}/object/{object_id}\x12\xad\x01\n\rDeleteObjects\x12\x33.aruna.api.storage.services.v1.DeleteObjectsRequest\x1a\x34.aruna.api.storage.services.v1.DeleteObjectsResponse\"1\x82\xd3\xe4\x93\x02+:\x01**&/v1/collection/{collection_id}/objects\x12\xb5\x01\n\rGetObjectByID\x12\x33.aruna.api.storage.services.v1.GetObjectByIDRequest\x1a\x34.aruna.api.storage.services.v1.GetObjectByIDResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/v1/collection/{collection_id}/object/{object_id}\x12\xa1\x01\n\nGetObjects\x12\x30.aruna.api.storage.services.v1.GetObjectsRequest\x1a\x31.aruna.api.storage.services.v1.GetObjectsResponse\".\x82\xd3\xe4\x93\x02(\x12&/v1/collection/{collection_id}/objects\x12\xce\x01\n\x12GetObjectRevisions\x12\x38.aruna.api.storage.services.v1.GetObjectRevisionsRequest\x1a\x39.aruna.api.storage.services.v1.GetObjectRevisionsResponse\"C\x82\xd3\xe4\x93\x02=\x12;/v1/collection/{collection_id}/object/{object_id}/revisions\x12\xda\x01\n\x17GetLatestObjectRevision\x12=.aruna.api.storage.services.v1.GetLatestObjectRevisionRequest\x1a>.aruna.api.storage.services.v1.GetLatestObjectRevisionResponse\"@\x82\xd3\xe4\x93\x02:\x12\x38/v1/collection/{collection_id}/object/{object_id}/latest\x12\xce\x01\n\x12GetObjectEndpoints\x12\x38.aruna.api.storage.services.v1.GetObjectEndpointsRequest\x1a\x39.aruna.api.storage.services.v1.GetObjectEndpointsResponse\"C\x82\xd3\xe4\x93\x02=\x12;/v1/collection/{collection_id}/object/{object_id}/endpoints\x12\xcf\x01\n\x11\x41\x64\x64LabelsToObject\x12\x37.aruna.api.storage.services.v1.AddLabelsToObjectRequest\x1a\x38.aruna.api.storage.services.v1.AddLabelsToObjectResponse\"G\x82\xd3\xe4\x93\x02\x41:\x01*2</v1/collection/{collection_id}/object/{object_id}/add_labels\x12\xcb\x01\n\x10SetHooksOfObject\x12\x36.aruna.api.storage.services.v1.SetHooksOfObjectRequest\x1a\x37.aruna.api.storage.services.v1.SetHooksOfObjectResponse\"F\x82\xd3\xe4\x93\x02@:\x01*2;/v1/collection/{collection_id}/object/{object_id}/set_hooks\x12\xc0\x01\n\rGetReferences\x12\x33.aruna.api.storage.services.v1.GetReferencesRequest\x1a\x34.aruna.api.storage.services.v1.GetReferencesResponse\"D\x82\xd3\xe4\x93\x02>\x12</v1/collection/{collection_id}/object/{object_id}/references\x12\xba\x01\n\rGetObjectPath\x12\x33.aruna.api.storage.services.v1.GetObjectPathRequest\x1a\x34.aruna.api.storage.services.v1.GetObjectPathResponse\">\x82\xd3\xe4\x93\x02\x38\x12\x36/v1/collection/{collection_id}/object/{object_id}/path\x12\xab\x01\n\x0eGetObjectPaths\x12\x34.aruna.api.storage.services.v1.GetObjectPathsRequest\x1a\x35.aruna.api.storage.services.v1.GetObjectPathsResponse\",\x82\xd3\xe4\x93\x02&\x12$/v1/collection/{collection_id}/paths\x12\xc6\x01\n\x10\x43reateObjectPath\x12\x36.aruna.api.storage.services.v1.CreateObjectPathRequest\x1a\x37.aruna.api.storage.services.v1.CreateObjectPathResponse\"A\x82\xd3\xe4\x93\x02;:\x01*\"6/v1/collection/{collection_id}/object/{object_id}/path\x12\xdd\x01\n\x17SetObjectPathVisibility\x12=.aruna.api.storage.services.v1.SetObjectPathVisibilityRequest\x1a>.aruna.api.storage.services.v1.SetObjectPathVisibilityResponse\"C\x82\xd3\xe4\x93\x02=:\x01*28/v1/collection/{collection_id}/path/{path=**}/visibility\x12\xa6\x01\n\x10GetObjectsByPath\x12\x36.aruna.api.storage.services.v1.GetObjectsByPathRequest\x1a\x37.aruna.api.storage.services.v1.GetObjectsByPathResponse\"!\x82\xd3\xe4\x93\x02\x1b\x12\x19/v1/path/object/{path=**}\x12\xd1\x01\n\x1dGetProjectCollectionIdsByPath\x12\x43.aruna.api.storage.services.v1.GetProjectCollectionIdsByPathRequest\x1a\x44.aruna.api.storage.services.v1.GetProjectCollectionIdsByPathResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/v1/path/collection/{path=**}\x12\xaa\x01\n\x12GetObjectsAsListV2\x12\x38.aruna.api.storage.services.v1.GetObjectsAsListV2Request\x1a\x39.aruna.api.storage.services.v1.GetObjectsAsListV2Response\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/v1/path/objects/listv2B\x8f\x01\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\rObjectServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.services.v1.object_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\rObjectServiceP\001Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1'
@@ -189,11 +189,11 @@
   _GETOBJECTSBYPATHRESPONSE._serialized_start=7134
   _GETOBJECTSBYPATHRESPONSE._serialized_end=7221
   _GETOBJECTSASLISTV2REQUEST._serialized_start=7224
   _GETOBJECTSASLISTV2REQUEST._serialized_end=7538
   _COMMONPREFIX._serialized_start=7540
   _COMMONPREFIX._serialized_end=7578
   _GETOBJECTSASLISTV2RESPONSE._serialized_start=7581
-  _GETOBJECTSASLISTV2RESPONSE._serialized_end=7947
-  _OBJECTSERVICE._serialized_start=7950
-  _OBJECTSERVICE._serialized_end=13140
+  _GETOBJECTSASLISTV2RESPONSE._serialized_end=7956
+  _OBJECTSERVICE._serialized_start=7959
+  _OBJECTSERVICE._serialized_end=13149
 # @@protoc_insertion_point(module_scope)
```

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/object_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/object_service_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -303,22 +303,22 @@
     CONTENTS_FIELD_NUMBER: _ClassVar[int]
     IS_TRUNCATED_FIELD_NUMBER: _ClassVar[int]
     KEY_COUNT_FIELD_NUMBER: _ClassVar[int]
     MAX_KEYS_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     NEXT_CONTINUATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
     PREFIXES_FIELD_NUMBER: _ClassVar[int]
-    contents: _containers.RepeatedCompositeFieldContainer[_models_pb2.Object]
+    contents: _containers.RepeatedCompositeFieldContainer[ObjectWithURL]
     is_truncated: bool
     key_count: int
     max_keys: int
     name: str
     next_continuation_token: str
     prefixes: _containers.RepeatedCompositeFieldContainer[CommonPrefix]
-    def __init__(self, name: _Optional[str] = ..., is_truncated: bool = ..., max_keys: _Optional[int] = ..., key_count: _Optional[int] = ..., contents: _Optional[_Iterable[_Union[_models_pb2.Object, _Mapping]]] = ..., prefixes: _Optional[_Iterable[_Union[CommonPrefix, _Mapping]]] = ..., next_continuation_token: _Optional[str] = ...) -> None: ...
+    def __init__(self, name: _Optional[str] = ..., is_truncated: bool = ..., max_keys: _Optional[int] = ..., key_count: _Optional[int] = ..., contents: _Optional[_Iterable[_Union[ObjectWithURL, _Mapping]]] = ..., prefixes: _Optional[_Iterable[_Union[CommonPrefix, _Mapping]]] = ..., next_continuation_token: _Optional[str] = ...) -> None: ...
 
 class GetObjectsByPathRequest(_message.Message):
     __slots__ = ["path", "with_revisions"]
     PATH_FIELD_NUMBER: _ClassVar[int]
     WITH_REVISIONS_FIELD_NUMBER: _ClassVar[int]
     path: str
     with_revisions: bool
```

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/object_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/object_service_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,15 +471,15 @@
         raise NotImplementedError('Method not implemented!')
 
     def GetObjectsAsListV2(self, request, context):
         """GetObjectsAsListV2
 
         Status: ALPHA
 
-        Gets a list of objects represented similar to a S3 ListObjectsV2 request
+        Gets a list of ObjectWithURLs represented similar to a S3 ListObjectsV2 request
         !! Paths are collection specific !!
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
```

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/objectgroup_service_pb2.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/objectgroup_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/project_service_pb2.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/project_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 
 
 from aruna.api.storage.models.v1 import auth_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_auth__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3aruna/api/storage/services/v1/project_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a&aruna/api/storage/models/v1/auth.proto\x1a\x1cgoogle/api/annotations.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\"L\n\x14\x43reateProjectRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\"6\n\x15\x43reateProjectResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x91\x01\n\x17\x41\x64\x64UserToProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x03 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\x1a\n\x18\x41\x64\x64UserToProjectResponse\"2\n\x11GetProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\\\n\x12GetProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"\x14\n\x12GetProjectsRequest\"_\n\x13GetProjectsResponse\x12H\n\x08projects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x08projects\"6\n\x15\x44\x65stroyProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x18\n\x16\x44\x65stroyProjectResponse\"k\n\x14UpdateProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\"_\n\x15UpdateProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"V\n\x1cRemoveUserFromProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x1f\n\x1dRemoveUserFromProjectResponse\"]\n#GetUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x8a\x01\n$GetUserPermissionsForProjectResponse\x12\x62\n\x0fuser_permission\x18\x01 \x01(\x0b\x32\x39.aruna.api.storage.models.v1.ProjectPermissionDisplayNameR\x0euserPermission\"\x9e\x01\n$EditUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\'\n%EditUserPermissionsForProjectResponse\"\xae\x01\n\x1aUserWithProjectPermissions\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v1.UserR\x04user\x12Y\n\x10user_permissions\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0fuserPermissions\"G\n&GetAllUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"z\n\'GetAllUserPermissionsForProjectResponse\x12O\n\x05users\x18\x01 \x03(\x0b\x32\x39.aruna.api.storage.services.v1.UserWithProjectPermissionsR\x05users2\x90\x0e\n\x0eProjectService\x12\x92\x01\n\rCreateProject\x12\x33.aruna.api.storage.services.v1.CreateProjectRequest\x1a\x34.aruna.api.storage.services.v1.CreateProjectResponse\"\x16\x82\xd3\xe4\x93\x02\x10:\x01*\"\x0b/v1/project\x12\xb1\x01\n\x10\x41\x64\x64UserToProject\x12\x36.aruna.api.storage.services.v1.AddUserToProjectRequest\x1a\x37.aruna.api.storage.services.v1.AddUserToProjectResponse\",\x82\xd3\xe4\x93\x02&:\x01*\"!/v1/project/{project_id}/add_user\x12\x93\x01\n\nGetProject\x12\x30.aruna.api.storage.services.v1.GetProjectRequest\x1a\x31.aruna.api.storage.services.v1.GetProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x12\x18/v1/project/{project_id}\x12\x8a\x01\n\x0bGetProjects\x12\x31.aruna.api.storage.services.v1.GetProjectsRequest\x1a\x32.aruna.api.storage.services.v1.GetProjectsResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v1/projects\x12\x9f\x01\n\x0e\x44\x65stroyProject\x12\x34.aruna.api.storage.services.v1.DestroyProjectRequest\x1a\x35.aruna.api.storage.services.v1.DestroyProjectResponse\" \x82\xd3\xe4\x93\x02\x1a*\x18/v1/project/{project_id}\x12\x9c\x01\n\rUpdateProject\x12\x33.aruna.api.storage.services.v1.UpdateProjectRequest\x1a\x34.aruna.api.storage.services.v1.UpdateProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x1a\x18/v1/project/{project_id}\x12\xc0\x01\n\x15RemoveUserFromProject\x12;.aruna.api.storage.services.v1.RemoveUserFromProjectRequest\x1a<.aruna.api.storage.services.v1.RemoveUserFromProjectResponse\",\x82\xd3\xe4\x93\x02&*$/v1/project/{project_id}/remove_user\x12\xd2\x01\n\x1cGetUserPermissionsForProject\x12\x42.aruna.api.storage.services.v1.GetUserPermissionsForProjectRequest\x1a\x43.aruna.api.storage.services.v1.GetUserPermissionsForProjectResponse\")\x82\xd3\xe4\x93\x02#\x12!/v1/project/{project_id}/get_user\x12\xdc\x01\n\x1fGetAllUserPermissionsForProject\x12\x45.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectRequest\x1a\x46.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectResponse\"*\x82\xd3\xe4\x93\x02$\x12\"/v1/project/{project_id}/get_users\x12\xd9\x01\n\x1d\x45\x64itUserPermissionsForProject\x12\x43.aruna.api.storage.services.v1.EditUserPermissionsForProjectRequest\x1a\x44.aruna.api.storage.services.v1.EditUserPermissionsForProjectResponse\"-\x82\xd3\xe4\x93\x02\':\x01*2\"/v1/project/{project_id}/edit_userB\xe5\x02\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x0eProjectServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\x92\x41\xd1\x01\x12\x31\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.5*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonZ`\n^\n\rAccessKeyAuth\x12M\x08\x02\x12\x38\x41uthentication token, prefixed by Bearer: Bearer <token>\x1a\rAuthorization \x02\x62\x13\n\x11\n\rAccessKeyAuth\x12\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3aruna/api/storage/services/v1/project_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a&aruna/api/storage/models/v1/auth.proto\x1a\x1cgoogle/api/annotations.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\"L\n\x14\x43reateProjectRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\"6\n\x15\x43reateProjectResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x91\x01\n\x17\x41\x64\x64UserToProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x03 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\x1a\n\x18\x41\x64\x64UserToProjectResponse\"2\n\x11GetProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\\\n\x12GetProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"\x14\n\x12GetProjectsRequest\"_\n\x13GetProjectsResponse\x12H\n\x08projects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x08projects\"6\n\x15\x44\x65stroyProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x18\n\x16\x44\x65stroyProjectResponse\"k\n\x14UpdateProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\"_\n\x15UpdateProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"V\n\x1cRemoveUserFromProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x1f\n\x1dRemoveUserFromProjectResponse\"]\n#GetUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x8a\x01\n$GetUserPermissionsForProjectResponse\x12\x62\n\x0fuser_permission\x18\x01 \x01(\x0b\x32\x39.aruna.api.storage.models.v1.ProjectPermissionDisplayNameR\x0euserPermission\"\x9e\x01\n$EditUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\'\n%EditUserPermissionsForProjectResponse\"\xae\x01\n\x1aUserWithProjectPermissions\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v1.UserR\x04user\x12Y\n\x10user_permissions\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0fuserPermissions\"G\n&GetAllUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"z\n\'GetAllUserPermissionsForProjectResponse\x12O\n\x05users\x18\x01 \x03(\x0b\x32\x39.aruna.api.storage.services.v1.UserWithProjectPermissionsR\x05users2\x90\x0e\n\x0eProjectService\x12\x92\x01\n\rCreateProject\x12\x33.aruna.api.storage.services.v1.CreateProjectRequest\x1a\x34.aruna.api.storage.services.v1.CreateProjectResponse\"\x16\x82\xd3\xe4\x93\x02\x10:\x01*\"\x0b/v1/project\x12\xb1\x01\n\x10\x41\x64\x64UserToProject\x12\x36.aruna.api.storage.services.v1.AddUserToProjectRequest\x1a\x37.aruna.api.storage.services.v1.AddUserToProjectResponse\",\x82\xd3\xe4\x93\x02&:\x01*\"!/v1/project/{project_id}/add_user\x12\x93\x01\n\nGetProject\x12\x30.aruna.api.storage.services.v1.GetProjectRequest\x1a\x31.aruna.api.storage.services.v1.GetProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x12\x18/v1/project/{project_id}\x12\x8a\x01\n\x0bGetProjects\x12\x31.aruna.api.storage.services.v1.GetProjectsRequest\x1a\x32.aruna.api.storage.services.v1.GetProjectsResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v1/projects\x12\x9f\x01\n\x0e\x44\x65stroyProject\x12\x34.aruna.api.storage.services.v1.DestroyProjectRequest\x1a\x35.aruna.api.storage.services.v1.DestroyProjectResponse\" \x82\xd3\xe4\x93\x02\x1a*\x18/v1/project/{project_id}\x12\x9c\x01\n\rUpdateProject\x12\x33.aruna.api.storage.services.v1.UpdateProjectRequest\x1a\x34.aruna.api.storage.services.v1.UpdateProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x1a\x18/v1/project/{project_id}\x12\xc0\x01\n\x15RemoveUserFromProject\x12;.aruna.api.storage.services.v1.RemoveUserFromProjectRequest\x1a<.aruna.api.storage.services.v1.RemoveUserFromProjectResponse\",\x82\xd3\xe4\x93\x02&*$/v1/project/{project_id}/remove_user\x12\xd2\x01\n\x1cGetUserPermissionsForProject\x12\x42.aruna.api.storage.services.v1.GetUserPermissionsForProjectRequest\x1a\x43.aruna.api.storage.services.v1.GetUserPermissionsForProjectResponse\")\x82\xd3\xe4\x93\x02#\x12!/v1/project/{project_id}/get_user\x12\xdc\x01\n\x1fGetAllUserPermissionsForProject\x12\x45.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectRequest\x1a\x46.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectResponse\"*\x82\xd3\xe4\x93\x02$\x12\"/v1/project/{project_id}/get_users\x12\xd9\x01\n\x1d\x45\x64itUserPermissionsForProject\x12\x43.aruna.api.storage.services.v1.EditUserPermissionsForProjectRequest\x1a\x44.aruna.api.storage.services.v1.EditUserPermissionsForProjectResponse\"-\x82\xd3\xe4\x93\x02\':\x01*2\"/v1/project/{project_id}/edit_userB\xe5\x02\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x0eProjectServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\x92\x41\xd1\x01\x12\x31\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.6*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonZ`\n^\n\rAccessKeyAuth\x12M\x08\x02\x12\x38\x41uthentication token, prefixed by Bearer: Bearer <token>\x1a\rAuthorization \x02\x62\x13\n\x11\n\rAccessKeyAuth\x12\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.services.v1.project_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\016ProjectServiceP\001Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\222A\321\001\0221\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.5*\001\0022\020application/json:\020application/jsonZ`\n^\n\rAccessKeyAuth\022M\010\002\0228Authentication token, prefixed by Bearer: Bearer <token>\032\rAuthorization \002b\023\n\021\n\rAccessKeyAuth\022\000'
+  DESCRIPTOR._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\016ProjectServiceP\001Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\222A\321\001\0221\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.6*\001\0022\020application/json:\020application/jsonZ`\n^\n\rAccessKeyAuth\022M\010\002\0228Authentication token, prefixed by Bearer: Bearer <token>\032\rAuthorization \002b\023\n\021\n\rAccessKeyAuth\022\000'
   _PROJECTSERVICE.methods_by_name['CreateProject']._options = None
   _PROJECTSERVICE.methods_by_name['CreateProject']._serialized_options = b'\202\323\344\223\002\020:\001*\"\013/v1/project'
   _PROJECTSERVICE.methods_by_name['AddUserToProject']._options = None
   _PROJECTSERVICE.methods_by_name['AddUserToProject']._serialized_options = b'\202\323\344\223\002&:\001*\"!/v1/project/{project_id}/add_user'
   _PROJECTSERVICE.methods_by_name['GetProject']._options = None
   _PROJECTSERVICE.methods_by_name['GetProject']._serialized_options = b'\202\323\344\223\002\032\022\030/v1/project/{project_id}'
   _PROJECTSERVICE.methods_by_name['GetProjects']._options = None
```

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/project_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/project_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/project_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/project_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/service_account_service_pb2.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/service_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/service_account_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/service_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/user_service_pb2.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/user_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/user_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc6/aruna/api/storage/services/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc5/setup.py` & `Aruna-Python-API-1.1.0rc6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='Aruna-Python-API',
-    version="1.1.0-rc.5",
+    version="1.1.0-rc.6",
     description='Aruna Object Storage Python API builds',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ArunaStorage/python-api',
     license='Apache 2.0',
     author='Marius Dieckmann, Jannis Hochmuth',
     author_email='marius.dieckmann@computational.bio.uni-giessen.de, '
```

