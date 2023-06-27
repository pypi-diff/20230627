# Comparing `tmp/types-redis-4.5.5.2.tar.gz` & `tmp/types-redis-4.6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-redis-4.5.5.2.tar", last modified: Thu May 11 18:18:04 2023, max compression
+gzip compressed data, was "types-redis-4.6.0.0.tar", last modified: Tue Jun 27 21:14:22 2023, max compression
```

## Comparing `types-redis-4.5.5.2.tar` & `types-redis-4.6.0.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.314382 types-redis-4.5.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    12730 2023-05-11 18:18:03.000000 types-redis-4.5.5.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 18:18:03.000000 types-redis-4.5.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-11 18:18:04.314382 types-redis-4.5.5.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.306382 types-redis-4.5.5.2/redis-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-11 18:18:03.000000 types-redis-4.5.5.2/redis-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.310382 types-redis-4.5.5.2/redis-stubs/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/asyncio/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    47468 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/asyncio/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/asyncio/cluster.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/asyncio/connection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/asyncio/lock.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/asyncio/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/asyncio/retry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/asyncio/sentinel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/asyncio/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/backoff.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    41578 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/cluster.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.310382 types-redis-4.5.5.2/redis-stubs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.310382 types-redis-4.5.5.2/redis-stubs/commands/bf/
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/bf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/bf/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/bf/info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/cluster.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    72299 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/core.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.310382 types-redis-4.5.5.2/redis-stubs/commands/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/graph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/graph/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/graph/edge.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/graph/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/graph/node.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/graph/path.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/graph/query_result.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/helpers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.314382 types-redis-4.5.5.2/redis-stubs/commands/json/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/json/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/json/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/json/decoders.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/json/path.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/redismodules.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.314382 types-redis-4.5.5.2/redis-stubs/commands/search/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/search/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/search/aggregation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/search/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/search/query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/search/result.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/sentinel.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.314382 types-redis-4.5.5.2/redis-stubs/commands/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/timeseries/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/timeseries/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/timeseries/info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/commands/timeseries/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/connection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/crc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/credentials.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/lock.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/ocsp.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/retry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/sentinel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/typing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-11 18:17:40.000000 types-redis-4.5.5.2/redis-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 18:18:04.314382 types-redis-4.5.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-11 18:18:03.000000 types-redis-4.5.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:18:04.314382 types-redis-4.5.5.2/types_redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-11 18:18:04.000000 types-redis-4.5.5.2/types_redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-11 18:18:04.000000 types-redis-4.5.5.2/types_redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:18:04.000000 types-redis-4.5.5.2/types_redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-11 18:18:04.000000 types-redis-4.5.5.2/types_redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 18:18:04.000000 types-redis-4.5.5.2/types_redis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:14:22.259140 types-redis-4.6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-06-27 21:14:19.000000 types-redis-4.6.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 21:14:19.000000 types-redis-4.6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-27 21:14:22.259140 types-redis-4.6.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:14:22.255139 types-redis-4.6.0.0/redis-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-27 21:14:19.000000 types-redis-4.6.0.0/redis-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:14:22.259140 types-redis-4.6.0.0/redis-stubs/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/asyncio/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    47493 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/asyncio/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/asyncio/cluster.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/asyncio/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/asyncio/lock.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/asyncio/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/asyncio/retry.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/asyncio/sentinel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/asyncio/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/backoff.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    41603 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/cluster.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:14:22.259140 types-redis-4.6.0.0/redis-stubs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:14:22.259140 types-redis-4.6.0.0/redis-stubs/commands/bf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/bf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/bf/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/bf/info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/cluster.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    72349 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/core.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:14:22.259140 types-redis-4.6.0.0/redis-stubs/commands/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/graph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/graph/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/graph/edge.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/graph/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/graph/node.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/graph/path.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/graph/query_result.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/helpers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:14:22.259140 types-redis-4.6.0.0/redis-stubs/commands/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/json/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/json/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/json/decoders.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/json/path.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/redismodules.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:14:22.259140 types-redis-4.6.0.0/redis-stubs/commands/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/search/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/search/aggregation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/search/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/search/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/search/result.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/sentinel.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:14:22.259140 types-redis-4.6.0.0/redis-stubs/commands/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/timeseries/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/timeseries/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/timeseries/info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/commands/timeseries/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/crc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/credentials.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/lock.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/ocsp.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/retry.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/sentinel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/typing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-27 21:14:05.000000 types-redis-4.6.0.0/redis-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 21:14:22.259140 types-redis-4.6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-27 21:14:19.000000 types-redis-4.6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:14:22.259140 types-redis-4.6.0.0/types_redis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-27 21:14:22.000000 types-redis-4.6.0.0/types_redis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-27 21:14:22.000000 types-redis-4.6.0.0/types_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:14:22.000000 types-redis-4.6.0.0/types_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 21:14:22.000000 types-redis-4.6.0.0/types_redis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 21:14:22.000000 types-redis-4.6.0.0/types_redis.egg-info/top_level.txt
```

### Comparing `types-redis-4.5.5.2/CHANGELOG.md` & `types-redis-4.6.0.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 4.6.0.0 (2023-06-27)
+
+Bump redis to 4.6.0 (#10360)
+
+Closes: #10359
+
 ## 4.5.5.2 (2023-05-11)
 
 Bump `mypy` to `1.3.0` (#10173)
 
 Co-authored-by: AlexWaygood <alex.waygood@gmail.com>
 
 ## 4.5.5.1 (2023-05-10)
```

### Comparing `types-redis-4.5.5.2/PKG-INFO` & `types-redis-4.6.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-redis
-Version: 4.5.5.2
+Version: 4.6.0.0
 Summary: Typing stubs for redis
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/redis.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `redis`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/redis. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6c54c74a84642faf8ed9834bd1adbc10c1877326`.
+This package was generated from typeshed commit `d32754c336d56fdffbc7840218a557c869dcb9ca` and was tested
+with mypy 1.4.1, pyright 1.1.315, and
+pytype 2023.6.2.
```

### Comparing `types-redis-4.5.5.2/redis-stubs/__init__.pyi` & `types-redis-4.6.0.0/redis-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/asyncio/__init__.pyi` & `types-redis-4.6.0.0/redis-stubs/asyncio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/asyncio/client.pyi` & `types-redis-4.6.0.0/redis-stubs/asyncio/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -823,15 +823,15 @@
         max: _Value,
         min: _Value,
         start: int | None = None,
         num: int | None = None,
         withscores: bool = False,
         score_cast_func: Callable[[_StrType], Any] = ...,
     ) -> Any: ...
-    def zrank(self, name: _Key, value: _Value) -> Any: ...  # type: ignore[override]
+    def zrank(self, name: _Key, value: _Value, withscore: bool = False) -> Any: ...  # type: ignore[override]
     def zrem(self, name: _Key, *values: _Value) -> Any: ...  # type: ignore[override]
     def zremrangebylex(self, name: _Key, min: _Value, max: _Value) -> Any: ...  # type: ignore[override]
     def zremrangebyrank(self, name: _Key, min: int, max: int) -> Any: ...  # type: ignore[override]
     def zremrangebyscore(self, name: _Key, min: _Value, max: _Value) -> Any: ...  # type: ignore[override]
     def zrevrank(self, name: _Key, value: _Value, withscore: bool = False) -> Any: ...  # type: ignore[override]
     def zscore(self, name: _Key, value: _Value) -> Any: ...  # type: ignore[override]
     def zunion(self, keys, aggregate: Incomplete | None = None, withscores: bool = False) -> Any: ...  # type: ignore[override]
```

### Comparing `types-redis-4.5.5.2/redis-stubs/asyncio/cluster.pyi` & `types-redis-4.6.0.0/redis-stubs/asyncio/cluster.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/asyncio/connection.pyi` & `types-redis-4.6.0.0/redis-stubs/asyncio/connection.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     def decode(self, value: EncodableT, force: bool = False) -> EncodableT: ...
 
 ExceptionMappingT: TypeAlias = Mapping[str, type[Exception] | Mapping[str, type[Exception]]]
 
 class BaseParser:
     EXCEPTION_CLASSES: ExceptionMappingT
     def __init__(self, socket_read_size: int) -> None: ...
-    def __del__(self) -> None: ...
     @classmethod
     def parse_error(cls, response: str) -> ResponseError: ...
     def on_disconnect(self) -> None: ...
     def on_connect(self, connection: Connection): ...
     async def read_response(self, disable_decoding: bool = False) -> EncodableT | ResponseError | list[EncodableT] | None: ...
 
 class PythonParser(BaseParser):
@@ -77,16 +76,16 @@
     pid: Any
     host: Any
     port: Any
     db: Any
     username: Any
     client_name: Any
     password: Any
-    socket_timeout: Any
-    socket_connect_timeout: Any
+    socket_timeout: float | None
+    socket_connect_timeout: float | None
     socket_keepalive: Any
     socket_keepalive_options: Any
     socket_type: Any
     retry_on_timeout: Any
     retry_on_error: list[type[RedisError]]
     retry: Retry
     health_check_interval: Any
@@ -118,15 +117,14 @@
         username: str | None = None,
         retry: Retry | None = None,
         redis_connect_func: ConnectCallbackT | None = None,
         encoder_class: type[Encoder] = ...,
         credential_provider: CredentialProvider | None = None,
     ) -> None: ...
     def repr_pieces(self): ...
-    def __del__(self) -> None: ...
     @property
     def is_connected(self): ...
     def register_connect_callback(self, callback) -> None: ...
     def clear_connect_callbacks(self) -> None: ...
     def set_parser(self, parser_class) -> None: ...
     async def connect(self) -> None: ...
     async def on_connect(self) -> None: ...
@@ -192,16 +190,14 @@
 class UnixDomainSocketConnection(Connection):
     pid: Any
     path: Any
     db: Any
     username: Any
     client_name: Any
     password: Any
-    socket_timeout: Any
-    socket_connect_timeout: Any
     retry_on_timeout: Any
     retry_on_error: list[type[RedisError]]
     retry: Any
     health_check_interval: Any
     next_health_check: int
     redis_connect_func: ConnectCallbackT | None
     encoder: Any
```

### Comparing `types-redis-4.5.5.2/redis-stubs/asyncio/lock.pyi` & `types-redis-4.6.0.0/redis-stubs/asyncio/lock.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/asyncio/retry.pyi` & `types-redis-4.6.0.0/redis-stubs/asyncio/retry.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/asyncio/sentinel.pyi` & `types-redis-4.6.0.0/redis-stubs/asyncio/sentinel.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 
 class SentinelManagedConnection(Connection):
     connection_pool: Any
     def __init__(self, **kwargs) -> None: ...
     async def connect_to(self, address) -> None: ...
     async def connect(self): ...
     @overload  # type: ignore[override]
-    async def read_response(self, *, timeout: float) -> Incomplete | None: ...
+    async def read_response(self, *, timeout: float, disconnect_on_error: bool = True) -> Incomplete | None: ...
     @overload
-    async def read_response(self, disable_decoding: bool, timeout: float) -> Incomplete | None: ...
+    async def read_response(
+        self, disable_decoding: bool, timeout: float, *, disconnect_on_error: bool = True
+    ) -> Incomplete | None: ...
     @overload
-    async def read_response(self, disable_decoding: bool = False, timeout: None = None): ...
+    async def read_response(self, disable_decoding: bool = False, timeout: None = None, *, disconnect_on_error: bool = True): ...
 
 class SentinelManagedSSLConnection(SentinelManagedConnection, SSLConnection): ...
 
 class SentinelConnectionPool(ConnectionPool):
     is_master: Any
     check_connection: Any
     service_name: Any
```

### Comparing `types-redis-4.5.5.2/redis-stubs/asyncio/utils.pyi` & `types-redis-4.6.0.0/redis-stubs/asyncio/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/backoff.pyi` & `types-redis-4.6.0.0/redis-stubs/backoff.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/client.pyi` & `types-redis-4.6.0.0/redis-stubs/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -677,15 +677,15 @@
         min: _Value,
         max: _Value,
         start: int | None = None,
         num: int | None = None,
         withscores: bool = False,
         score_cast_func: Callable[[_StrType], Any] = ...,
     ) -> Pipeline[_StrType]: ...
-    def zrank(self, name: _Key, value: _Value) -> Pipeline[_StrType]: ...  # type: ignore[override]
+    def zrank(self, name: _Key, value: _Value, withscore: bool = False) -> Pipeline[_StrType]: ...  # type: ignore[override]
     def zrem(self, name: _Key, *values: _Value) -> Pipeline[_StrType]: ...  # type: ignore[override]
     def zremrangebylex(self, name: _Key, min: _Value, max: _Value) -> Pipeline[_StrType]: ...  # type: ignore[override]
     def zremrangebyrank(self, name: _Key, min: _Value, max: _Value) -> Pipeline[_StrType]: ...  # type: ignore[override]
     def zremrangebyscore(self, name: _Key, min: _Value, max: _Value) -> Pipeline[_StrType]: ...  # type: ignore[override]
     def zrevrange(  # type: ignore[override]
         self, name: _Key, start: int, end: int, withscores: bool = False, score_cast_func: Callable[[_StrType], Any] = ...
     ) -> Pipeline[_StrType]: ...
```

### Comparing `types-redis-4.5.5.2/redis-stubs/cluster.pyi` & `types-redis-4.6.0.0/redis-stubs/cluster.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/commands/__init__.pyi` & `types-redis-4.6.0.0/redis-stubs/commands/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/commands/bf/__init__.pyi` & `types-redis-4.6.0.0/redis-stubs/commands/bf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/commands/bf/commands.pyi` & `types-redis-4.6.0.0/redis-stubs/commands/bf/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/commands/bf/info.pyi` & `types-redis-4.6.0.0/redis-stubs/commands/bf/info.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/commands/cluster.pyi` & `types-redis-4.6.0.0/redis-stubs/commands/cluster.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/commands/core.pyi` & `types-redis-4.6.0.0/redis-stubs/commands/core.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1174,15 +1174,15 @@
         max: _Value,
         min: _Value,
         start: int | None = None,
         num: int | None = None,
         withscores: bool = False,
         score_cast_func: Callable[[_StrType], Any] = ...,
     ) -> list[_StrType]: ...
-    def zrank(self, name: _Key, value: _Value) -> int | None: ...
+    def zrank(self, name: _Key, value: _Value, withscore: bool = False) -> int | None: ...
     def zrem(self, name: _Key, *values: _Value) -> int: ...
     def zremrangebylex(self, name: _Key, min: _Value, max: _Value) -> int: ...
     def zremrangebyrank(self, name: _Key, min: int, max: int) -> int: ...
     def zremrangebyscore(self, name: _Key, min: _Value, max: _Value) -> int: ...
     def zrevrank(self, name: _Key, value: _Value, withscore: bool = False) -> int | None: ...
     def zscore(self, name: _Key, value: _Value) -> float | None: ...
     def zunion(self, keys, aggregate: Incomplete | None = None, withscores: bool = False): ...
@@ -1377,15 +1377,15 @@
         max: _Value,
         min: _Value,
         start: int | None = None,
         num: int | None = None,
         withscores: bool = False,
         score_cast_func: Callable[[_StrType], Any] = ...,
     ) -> list[_StrType]: ...
-    async def zrank(self, name: _Key, value: _Value) -> int | None: ...
+    async def zrank(self, name: _Key, value: _Value, withscore: bool = False) -> int | None: ...
     async def zrem(self, name: _Key, *values: _Value) -> int: ...
     async def zremrangebylex(self, name: _Key, min: _Value, max: _Value) -> int: ...
     async def zremrangebyrank(self, name: _Key, min: int, max: int) -> int: ...
     async def zremrangebyscore(self, name: _Key, min: _Value, max: _Value) -> int: ...
     async def zrevrank(self, name: _Key, value: _Value, withscore: bool = False) -> int | None: ...
     async def zscore(self, name: _Key, value: _Value) -> float | None: ...
     async def zunion(self, keys, aggregate: Incomplete | None = None, withscores: bool = False): ...
```

### Comparing `types-redis-4.5.5.2/redis-stubs/commands/graph/__init__.pyi` & `types-redis-4.6.0.0/redis-stubs/commands/graph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/commands/graph/commands.pyi` & `types-redis-4.6.0.0/redis-stubs/commands/graph/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/commands/graph/query_result.pyi` & `types-redis-4.6.0.0/redis-stubs/commands/graph/query_result.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/commands/json/__init__.pyi` & `types-redis-4.6.0.0/redis-stubs/commands/json/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/commands/json/commands.pyi` & `types-redis-4.6.0.0/redis-stubs/commands/json/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/commands/search/__init__.pyi` & `types-redis-4.6.0.0/redis-stubs/commands/search/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/commands/search/aggregation.pyi` & `types-redis-4.6.0.0/redis-stubs/commands/search/aggregation.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/commands/search/commands.pyi` & `types-redis-4.6.0.0/redis-stubs/commands/search/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/commands/search/query.pyi` & `types-redis-4.6.0.0/redis-stubs/commands/search/query.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/commands/sentinel.pyi` & `types-redis-4.6.0.0/redis-stubs/commands/sentinel.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/commands/timeseries/__init__.pyi` & `types-redis-4.6.0.0/redis-stubs/commands/timeseries/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/commands/timeseries/commands.pyi` & `types-redis-4.6.0.0/redis-stubs/commands/timeseries/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/commands/timeseries/info.pyi` & `types-redis-4.6.0.0/redis-stubs/commands/timeseries/info.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/connection.pyi` & `types-redis-4.6.0.0/redis-stubs/connection.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -85,26 +85,30 @@
 class AbstractConnection:
     pid: int
     db: int
     client_name: str | None
     credential_provider: CredentialProvider | None
     password: str | None
     username: str | None
+    socket_timeout: float | None
+    socket_connect_timeout: float | None
     retry_on_timeout: bool
     retry_on_error: list[type[Exception]]
     retry: Retry
     health_check_interval: int
     next_health_check: int
     redis_connect_func: _ConnectFunc | None
     encoder: Encoder
 
     def __init__(
         self,
         db: int = 0,
         password: str | None = None,
+        socket_timeout: float | None = None,
+        socket_connect_timeout: float | None = None,
         retry_on_timeout: bool = False,
         retry_on_error: list[type[Exception]] = ...,
         encoding: str = "utf-8",
         encoding_errors: str = "strict",
         decode_responses: bool = False,
         parser_class: type[BaseParser] = ...,
         socket_read_size: int = 65536,
@@ -133,31 +137,29 @@
     ) -> Any: ...  # `str | bytes` or `list[str | bytes]`
     def pack_command(self, *args) -> list[bytes]: ...
     def pack_commands(self, commands: Iterable[Iterable[Incomplete]]) -> list[bytes]: ...
 
 class Connection(AbstractConnection):
     host: str
     port: int
-    socket_timeout: float | None
-    socket_connect_timeout: float | None
     socket_keepalive: bool
     socket_keepalive_options: Mapping[str, int | str]
     socket_type: int
     def __init__(
         self,
         host: str = "localhost",
         port: int = 6379,
-        socket_timeout: float | None = None,
-        socket_connect_timeout: float | None = None,
         socket_keepalive: bool = False,
         socket_keepalive_options: Mapping[str, int | str] | None = None,
         socket_type: int = 0,
         *,
         db: int = 0,
         password: str | None = None,
+        socket_timeout: float | None = None,
+        socket_connect_timeout: float | None = None,
         retry_on_timeout: bool = False,
         retry_on_error: list[type[Exception]] = ...,
         encoding: str = "utf-8",
         encoding_errors: str = "strict",
         decode_responses: bool = False,
         parser_class: type[BaseParser] = ...,
         socket_read_size: int = 65536,
@@ -221,22 +223,22 @@
         redis_connect_func: _ConnectFunc | None = None,
         credential_provider: CredentialProvider | None = None,
         command_packer: Incomplete | None = None,
     ) -> None: ...
 
 class UnixDomainSocketConnection(AbstractConnection):
     path: str
-    socket_timeout: float | None
     def __init__(
         self,
         path: str = "",
-        socket_timeout: float | None = None,
         *,
         db: int = 0,
         password: str | None = None,
+        socket_timeout: float | None = None,
+        socket_connect_timeout: float | None = None,
         retry_on_timeout: bool = False,
         retry_on_error: list[type[Exception]] = ...,
         encoding: str = "utf-8",
         encoding_errors: str = "strict",
         decode_responses: bool = False,
         parser_class: type[BaseParser] = ...,
         socket_read_size: int = 65536,
```

### Comparing `types-redis-4.5.5.2/redis-stubs/exceptions.pyi` & `types-redis-4.6.0.0/redis-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/lock.pyi` & `types-redis-4.6.0.0/redis-stubs/lock.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/ocsp.pyi` & `types-redis-4.6.0.0/redis-stubs/ocsp.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/sentinel.pyi` & `types-redis-4.6.0.0/redis-stubs/sentinel.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 _SentinelState: TypeAlias = dict[str, Any]  # TODO: this can be a TypedDict
 
 class MasterNotFoundError(ConnectionError): ...
 class SlaveNotFoundError(ConnectionError): ...
 
 class SentinelManagedConnection(Connection):
     connection_pool: SentinelConnectionPool
-    def __init__(self, **kwargs) -> None: ...
+    def __init__(self, *, connection_pool: SentinelConnectionPool, **kwargs) -> None: ...
     def connect_to(self, address: _AddressAndPort) -> None: ...
     def connect(self) -> None: ...
     # The result can be either `str | bytes` or `list[str | bytes]`
-    def read_response(self, disable_decoding: bool = False) -> Any: ...  # type: ignore[override]
+    def read_response(self, disable_decoding: bool = False, *, disconnect_on_error: bool = False) -> Any: ...
 
 class SentinelManagedSSLConnection(SentinelManagedConnection, SSLConnection): ...
 
 class SentinelConnectionPool(ConnectionPool):
     is_master: bool
     check_connection: bool
     service_name: str
```

### Comparing `types-redis-4.5.5.2/redis-stubs/typing.pyi` & `types-redis-4.6.0.0/redis-stubs/typing.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/redis-stubs/utils.pyi` & `types-redis-4.6.0.0/redis-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.5.2/setup.py` & `types-redis-4.6.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,33 +11,39 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `redis`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/redis. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6c54c74a84642faf8ed9834bd1adbc10c1877326`.
+This package was generated from typeshed commit `d32754c336d56fdffbc7840218a557c869dcb9ca` and was tested
+with mypy 1.4.1, pyright 1.1.315, and
+pytype 2023.6.2.
 '''.lstrip()
 
 setup(name=name,
-      version="4.5.5.2",
+      version="4.6.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/redis.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['types-pyOpenSSL', 'cryptography>=35.0.0'],
       packages=['redis-stubs'],
-      package_data={'redis-stubs': ['__init__.pyi', 'asyncio/__init__.pyi', 'asyncio/client.pyi', 'asyncio/cluster.pyi', 'asyncio/connection.pyi', 'asyncio/lock.pyi', 'asyncio/parser.pyi', 'asyncio/retry.pyi', 'asyncio/sentinel.pyi', 'asyncio/utils.pyi', 'backoff.pyi', 'client.pyi', 'cluster.pyi', 'commands/__init__.pyi', 'commands/bf/__init__.pyi', 'commands/bf/commands.pyi', 'commands/bf/info.pyi', 'commands/cluster.pyi', 'commands/core.pyi', 'commands/graph/__init__.pyi', 'commands/graph/commands.pyi', 'commands/graph/edge.pyi', 'commands/graph/exceptions.pyi', 'commands/graph/node.pyi', 'commands/graph/path.pyi', 'commands/graph/query_result.pyi', 'commands/helpers.pyi', 'commands/json/__init__.pyi', 'commands/json/commands.pyi', 'commands/json/decoders.pyi', 'commands/json/path.pyi', 'commands/parser.pyi', 'commands/redismodules.pyi', 'commands/search/__init__.pyi', 'commands/search/aggregation.pyi', 'commands/search/commands.pyi', 'commands/search/query.pyi', 'commands/search/result.pyi', 'commands/sentinel.pyi', 'commands/timeseries/__init__.pyi', 'commands/timeseries/commands.pyi', 'commands/timeseries/info.pyi', 'commands/timeseries/utils.pyi', 'connection.pyi', 'crc.pyi', 'credentials.pyi', 'exceptions.pyi', 'lock.pyi', 'ocsp.pyi', 'retry.pyi', 'sentinel.pyi', 'typing.pyi', 'utils.pyi', 'METADATA.toml']},
+      package_data={'redis-stubs': ['__init__.pyi', 'asyncio/__init__.pyi', 'asyncio/client.pyi', 'asyncio/cluster.pyi', 'asyncio/connection.pyi', 'asyncio/lock.pyi', 'asyncio/parser.pyi', 'asyncio/retry.pyi', 'asyncio/sentinel.pyi', 'asyncio/utils.pyi', 'backoff.pyi', 'client.pyi', 'cluster.pyi', 'commands/__init__.pyi', 'commands/bf/__init__.pyi', 'commands/bf/commands.pyi', 'commands/bf/info.pyi', 'commands/cluster.pyi', 'commands/core.pyi', 'commands/graph/__init__.pyi', 'commands/graph/commands.pyi', 'commands/graph/edge.pyi', 'commands/graph/exceptions.pyi', 'commands/graph/node.pyi', 'commands/graph/path.pyi', 'commands/graph/query_result.pyi', 'commands/helpers.pyi', 'commands/json/__init__.pyi', 'commands/json/commands.pyi', 'commands/json/decoders.pyi', 'commands/json/path.pyi', 'commands/parser.pyi', 'commands/redismodules.pyi', 'commands/search/__init__.pyi', 'commands/search/aggregation.pyi', 'commands/search/commands.pyi', 'commands/search/query.pyi', 'commands/search/result.pyi', 'commands/sentinel.pyi', 'commands/timeseries/__init__.pyi', 'commands/timeseries/commands.pyi', 'commands/timeseries/info.pyi', 'commands/timeseries/utils.pyi', 'connection.pyi', 'crc.pyi', 'credentials.pyi', 'exceptions.pyi', 'lock.pyi', 'ocsp.pyi', 'retry.pyi', 'sentinel.pyi', 'typing.pyi', 'utils.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-redis-4.5.5.2/types_redis.egg-info/PKG-INFO` & `types-redis-4.6.0.0/types_redis.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-redis
-Version: 4.5.5.2
+Version: 4.6.0.0
 Summary: Typing stubs for redis
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/redis.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `redis`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/redis. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6c54c74a84642faf8ed9834bd1adbc10c1877326`.
+This package was generated from typeshed commit `d32754c336d56fdffbc7840218a557c869dcb9ca` and was tested
+with mypy 1.4.1, pyright 1.1.315, and
+pytype 2023.6.2.
```

### Comparing `types-redis-4.5.5.2/types_redis.egg-info/SOURCES.txt` & `types-redis-4.6.0.0/types_redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

