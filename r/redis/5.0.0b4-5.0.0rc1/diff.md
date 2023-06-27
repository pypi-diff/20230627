# Comparing `tmp/redis-5.0.0b4.tar.gz` & `tmp/redis-5.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-5.0.0b4.tar", last modified: Sun May 28 09:28:37 2023, max compression
+gzip compressed data, was "redis-5.0.0rc1.tar", last modified: Tue Jun 27 18:40:37 2023, max compression
```

## Comparing `redis-5.0.0b4.tar` & `redis-5.0.0rc1.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.120266 redis-5.0.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-28 09:28:22.000000 redis-5.0.0b4/INSTALL
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-28 09:28:22.000000 redis-5.0.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-28 09:28:22.000000 redis-5.0.0b4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-05-28 09:28:37.120266 redis-5.0.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-05-28 09:28:22.000000 redis-5.0.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.104266 redis-5.0.0b4/redis/
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.104266 redis-5.0.0b4/redis/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55393 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/asyncio/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    61198 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/asyncio/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    51222 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/asyncio/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/asyncio/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/asyncio/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/asyncio/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/asyncio/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/backoff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    83526 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    90431 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.108266 redis-5.0.0b4/redis/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.108266 redis-5.0.0b4/redis/commands/bf/
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/bf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/bf/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/bf/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    30844 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)   217363 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.108266 redis-5.0.0b4/redis/commands/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/graph/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/graph/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/graph/execution_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/graph/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/graph/query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.108266 redis-5.0.0b4/redis/commands/json/
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/json/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/json/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/json/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/json/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/redismodules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.112266 redis-5.0.0b4/redis/commands/search/
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35597 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/indexDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/querystring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/reducers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/sentinel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.112266 redis-5.0.0b4/redis/commands/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33438 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/timeseries/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/timeseries/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/timeseries/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    46593 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/crc.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/ocsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.112266 redis-5.0.0b4/redis/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/parsers/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/parsers/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/parsers/hiredis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/parsers/resp2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/parsers/resp3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/parsers/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.104266 redis-5.0.0b4/redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-05-28 09:28:37.000000 redis-5.0.0b4/redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-05-28 09:28:37.000000 redis-5.0.0b4/redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 09:28:37.000000 redis-5.0.0b4/redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-28 09:28:37.000000 redis-5.0.0b4/redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 09:28:37.000000 redis-5.0.0b4/redis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 09:28:37.120266 redis-5.0.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-28 09:28:22.000000 redis-5.0.0b4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.116266 redis-5.0.0b4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/asynctests
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/synctests
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.116266 redis-5.0.0b4/tests/test_asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    18706 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_bloom.py
--rw-r--r--   0 runner    (1001) docker     (123)   112337 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)   122627 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    34475 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    32971 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    38161 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)    35180 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_sentinel_managed_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.116266 redis-5.0.0b4/tests/test_asyncio/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/testdata/jsontestdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/testdata/titles.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/testdata/will_play_text.csv.bz2
--rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_bloom.py
--rw-r--r--   0 runner    (1001) docker     (123)   118948 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_command_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)   180759 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    30432 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    18914 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.120266 redis-5.0.0b4/tests/test_graph_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_graph_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_graph_utils/test_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_graph_utils/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_graph_utils/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    42822 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    42590 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)    53061 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24927 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.120266 redis-5.0.0b4/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/testdata/jsontestdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/testdata/titles.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/testdata/will_play_text.csv.bz2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.150637 redis-5.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-27 18:40:17.000000 redis-5.0.0rc1/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-27 18:40:17.000000 redis-5.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-27 18:40:17.000000 redis-5.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-06-27 18:40:37.150637 redis-5.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-06-27 18:40:17.000000 redis-5.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.118637 redis-5.0.0rc1/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.122637 redis-5.0.0rc1/redis/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55541 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/asyncio/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61437 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/asyncio/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52680 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/asyncio/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/asyncio/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/asyncio/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/asyncio/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/asyncio/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/backoff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    84080 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90814 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.122637 redis-5.0.0rc1/redis/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.122637 redis-5.0.0rc1/redis/commands/bf/
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/bf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21462 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/bf/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/bf/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30844 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)   217539 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.126637 redis-5.0.0rc1/redis/commands/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/graph/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/graph/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/graph/execution_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/graph/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/graph/query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.126637 redis-5.0.0rc1/redis/commands/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/json/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/json/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/json/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/json/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/redismodules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.126637 redis-5.0.0rc1/redis/commands/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/indexDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/querystring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/reducers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/search/suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/sentinel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.130637 redis-5.0.0rc1/redis/commands/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33438 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/timeseries/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/timeseries/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/commands/timeseries/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48046 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/crc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/ocsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.130637 redis-5.0.0rc1/redis/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/parsers/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/parsers/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/parsers/hiredis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/parsers/resp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/parsers/resp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/parsers/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-27 18:40:17.000000 redis-5.0.0rc1/redis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.118637 redis-5.0.0rc1/redis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-06-27 18:40:37.000000 redis-5.0.0rc1/redis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-06-27 18:40:37.000000 redis-5.0.0rc1/redis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:40:37.000000 redis-5.0.0rc1/redis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-27 18:40:37.000000 redis-5.0.0rc1/redis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 18:40:37.000000 redis-5.0.0rc1/redis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:40:37.150637 redis-5.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-27 18:40:17.000000 redis-5.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.138637 redis-5.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/asynctests
+-rw-r--r--   0 runner    (1001) docker     (123)    15601 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/synctests
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.142637 redis-5.0.0rc1/tests/test_asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19097 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113908 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122540 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34543 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35100 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13868 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38167 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57127 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_sentinel_managed_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27356 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.142637 redis-5.0.0rc1/tests/test_asyncio/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/testdata/jsontestdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/testdata/titles.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_asyncio/testdata/will_play_text.csv.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)    17948 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119547 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_command_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)   177287 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30431 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19024 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.146637 redis-5.0.0rc1/tests/test_graph_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_graph_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_graph_utils/test_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_graph_utils/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_graph_utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47244 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43246 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80154 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33464 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:40:37.146637 redis-5.0.0rc1/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/testdata/jsontestdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/testdata/titles.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-06-27 18:40:17.000000 redis-5.0.0rc1/tests/testdata/will_play_text.csv.bz2
```

### Comparing `redis-5.0.0b4/LICENSE` & `redis-5.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/PKG-INFO` & `redis-5.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis
-Version: 5.0.0b4
+Version: 5.0.0rc1
 Summary: Python client for Redis database and key-value store
 Home-page: https://github.com/redis/redis-py
 Author: Redis Inc.
 Author-email: oss@redis.com
 License: MIT
 Project-URL: Documentation, https://redis.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/redis/redis-py/releases
```

### Comparing `redis-5.0.0b4/README.md` & `redis-5.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/__init__.py` & `redis-5.0.0rc1/redis/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sys
 
+from redis import asyncio  # noqa
 from redis.backoff import default_backoff
 from redis.client import Redis, StrictRedis
 from redis.cluster import RedisCluster
 from redis.connection import (
     BlockingConnectionPool,
     Connection,
     ConnectionPool,
```

### Comparing `redis-5.0.0b4/redis/asyncio/__init__.py` & `redis-5.0.0rc1/redis/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/asyncio/client.py` & `redis-5.0.0rc1/redis/asyncio/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,14 +253,16 @@
         self.single_connection_client = single_connection_client
         self.connection: Optional[Connection] = None
 
         self.response_callbacks = CaseInsensitiveDict(self.__class__.RESPONSE_CALLBACKS)
 
         if self.connection_pool.connection_kwargs.get("protocol") in ["3", 3]:
             self.response_callbacks.update(self.__class__.RESP3_RESPONSE_CALLBACKS)
+        else:
+            self.response_callbacks.update(self.__class__.RESP2_RESPONSE_CALLBACKS)
 
         # If using a single connection client, we need to lock creation-of and use-of
         # the client in order to avoid race conditions such as using asyncio.gather
         # on a set of redis commands
         self._single_conn_lock = asyncio.Lock()
 
     def __repr__(self):
@@ -667,21 +669,21 @@
         # we need to know the encoding options for this connection in order
         # to lookup channel and pattern names for callback handlers.
         self.encoder = encoder
         self.push_handler_func = push_handler_func
         if self.encoder is None:
             self.encoder = self.connection_pool.get_encoder()
         if self.encoder.decode_responses:
-            self.health_check_response: Iterable[Union[str, bytes]] = [
-                "pong",
+            self.health_check_response = [
+                ["pong", self.HEALTH_CHECK_MESSAGE],
                 self.HEALTH_CHECK_MESSAGE,
             ]
         else:
             self.health_check_response = [
-                b"pong",
+                [b"pong", self.encoder.encode(self.HEALTH_CHECK_MESSAGE)],
                 self.encoder.encode(self.HEALTH_CHECK_MESSAGE),
             ]
         if self.push_handler_func is None:
             _set_info_logger()
         self.channels = {}
         self.pending_unsubscribe_channels = set()
         self.patterns = {}
@@ -803,15 +805,15 @@
             await conn.connect()
 
         read_timeout = None if block else timeout
         response = await self._execute(
             conn, conn.read_response, timeout=read_timeout, push_request=True
         )
 
-        if conn.health_check_interval and response == self.health_check_response:
+        if conn.health_check_interval and response in self.health_check_response:
             # ignore the health check message as user might not expect it
             return None
         return response
 
     async def check_health(self):
         conn = self.connection
         if conn is None:
```

### Comparing `redis-5.0.0b4/redis/asyncio/cluster.py` & `redis-5.0.0rc1/redis/asyncio/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,14 +315,18 @@
             if not retry_on_error:
                 # Default errors for retrying
                 retry_on_error = [ConnectionError, TimeoutError]
             self.retry.update_supported_errors(retry_on_error)
             kwargs.update({"retry": self.retry})
 
         kwargs["response_callbacks"] = self.__class__.RESPONSE_CALLBACKS.copy()
+        if kwargs.get("protocol") in ["3", 3]:
+            kwargs["response_callbacks"].update(self.__class__.RESP3_RESPONSE_CALLBACKS)
+        else:
+            kwargs["response_callbacks"].update(self.__class__.RESP2_RESPONSE_CALLBACKS)
         self.connection_kwargs = kwargs
 
         if startup_nodes:
             passed_nodes = []
             for node in startup_nodes:
                 passed_nodes.append(
                     ClusterNode(node.host, node.port, **self.connection_kwargs)
```

### Comparing `redis-5.0.0b4/redis/asyncio/connection.py` & `redis-5.0.0rc1/redis/asyncio/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 from urllib.parse import ParseResult, parse_qs, unquote, urlparse
 
 if sys.version_info.major >= 3 and sys.version_info.minor >= 11:
     from asyncio import timeout as async_timeout
 else:
     from async_timeout import timeout as async_timeout
 
-
 from redis.asyncio.retry import Retry
 from redis.backoff import NoBackoff
 from redis.compat import Protocol, TypedDict
+from redis.connection import DEFAULT_RESP_VERSION
 from redis.credentials import CredentialProvider, UsernamePasswordCredentialProvider
 from redis.exceptions import (
     AuthenticationError,
     AuthenticationWrongNumberOfArgsError,
     ChildDeadlockedError,
     ConnectionError,
     DataError,
@@ -199,15 +199,24 @@
         self.redis_connect_func = redis_connect_func
         self._reader: Optional[asyncio.StreamReader] = None
         self._writer: Optional[asyncio.StreamWriter] = None
         self._socket_read_size = socket_read_size
         self.set_parser(parser_class)
         self._connect_callbacks: List[weakref.WeakMethod[ConnectCallbackT]] = []
         self._buffer_cutoff = 6000
-        self.protocol = protocol
+        try:
+            p = int(protocol)
+        except TypeError:
+            p = DEFAULT_RESP_VERSION
+        except ValueError:
+            raise ConnectionError("protocol must be an integer")
+        finally:
+            if p < 2 or p > 3:
+                raise ConnectionError("protocol must be either 2 or 3")
+            self.protocol = protocol
 
     def __repr__(self):
         repr_args = ",".join((f"{k}={v}" for k, v in self.repr_pieces()))
         return f"{self.__class__.__name__}<{repr_args}>"
 
     def repr_pieces(self):
         pieces = [("host", self.host), ("port", self.port), ("db", self.db)]
@@ -329,24 +338,43 @@
                 f"Error {exception.args[0]} connecting to {self.host}:{self.port}. "
                 f"{exception.args[0]}."
             )
 
     async def on_connect(self) -> None:
         """Initialize the connection, authenticate and select a database"""
         self._parser.on_connect(self)
+        parser = self._parser
 
+        auth_args = None
         # if credential provider or username and/or password are set, authenticate
         if self.credential_provider or (self.username or self.password):
             cred_provider = (
                 self.credential_provider
                 or UsernamePasswordCredentialProvider(self.username, self.password)
             )
             auth_args = cred_provider.get_credentials()
-            # avoid checking health here -- PING will fail if we try
-            # to check the health prior to the AUTH
+            # if resp version is specified and we have auth args,
+            # we need to send them via HELLO
+        if auth_args and self.protocol not in [2, "2"]:
+            if isinstance(self._parser, _AsyncRESP2Parser):
+                self.set_parser(_AsyncRESP3Parser)
+                # update cluster exception classes
+                self._parser.EXCEPTION_CLASSES = parser.EXCEPTION_CLASSES
+                self._parser.on_connect(self)
+            if len(auth_args) == 1:
+                auth_args = ["default", auth_args[0]]
+            await self.send_command("HELLO", self.protocol, "AUTH", *auth_args)
+            response = await self.read_response()
+            if response.get(b"proto") != int(self.protocol) and response.get(
+                "proto"
+            ) != int(self.protocol):
+                raise ConnectionError("Invalid RESP version")
+        # avoid checking health here -- PING will fail if we try
+        # to check the health prior to the AUTH
+        elif auth_args:
             await self.send_command("AUTH", *auth_args, check_health=False)
 
             try:
                 auth_response = await self.read_response()
             except AuthenticationWrongNumberOfArgsError:
                 # a username and password were specified but the Redis
                 # server seems to be < 6.0.0 which expects a single password
@@ -355,24 +383,26 @@
                 await self.send_command("AUTH", auth_args[-1], check_health=False)
                 auth_response = await self.read_response()
 
             if str_if_bytes(auth_response) != "OK":
                 raise AuthenticationError("Invalid Username or Password")
 
         # if resp version is specified, switch to it
-        if self.protocol != 2:
+        elif self.protocol not in [2, "2"]:
             if isinstance(self._parser, _AsyncRESP2Parser):
                 self.set_parser(_AsyncRESP3Parser)
+                # update cluster exception classes
+                self._parser.EXCEPTION_CLASSES = parser.EXCEPTION_CLASSES
                 self._parser.on_connect(self)
             await self.send_command("HELLO", self.protocol)
             response = await self.read_response()
-            if response.get(b"proto") != int(self.protocol) and response.get(
-                "proto"
-            ) != int(self.protocol):
-                raise ConnectionError("Invalid RESP version")
+            # if response.get(b"proto") != self.protocol and response.get(
+            #     "proto"
+            # ) != self.protocol:
+            #     raise ConnectionError("Invalid RESP version")
 
         # if a client_name is given, set it
         if self.client_name:
             await self.send_command("CLIENT", "SETNAME", self.client_name)
             if str_if_bytes(await self.read_response()) != "OK":
                 raise ConnectionError("Error setting client name")
 
@@ -488,27 +518,27 @@
         push_request: Optional[bool] = False,
     ):
         """Read the response from a previously sent command"""
         read_timeout = timeout if timeout is not None else self.socket_timeout
         try:
             if (
                 read_timeout is not None
-                and self.protocol == "3"
+                and self.protocol in ["3", 3]
                 and not HIREDIS_AVAILABLE
             ):
                 async with async_timeout(read_timeout):
                     response = await self._parser.read_response(
                         disable_decoding=disable_decoding, push_request=push_request
                     )
             elif read_timeout is not None:
                 async with async_timeout(read_timeout):
                     response = await self._parser.read_response(
                         disable_decoding=disable_decoding
                     )
-            elif self.protocol == "3" and not HIREDIS_AVAILABLE:
+            elif self.protocol in ["3", 3] and not HIREDIS_AVAILABLE:
                 response = await self._parser.read_response(
                     disable_decoding=disable_decoding, push_request=push_request
                 )
             else:
                 response = await self._parser.read_response(
                     disable_decoding=disable_decoding
                 )
```

### Comparing `redis-5.0.0b4/redis/asyncio/lock.py` & `redis-5.0.0rc1/redis/asyncio/lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/asyncio/retry.py` & `redis-5.0.0rc1/redis/asyncio/retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/asyncio/sentinel.py` & `redis-5.0.0rc1/redis/asyncio/sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/asyncio/utils.py` & `redis-5.0.0rc1/redis/asyncio/utils.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/backoff.py` & `redis-5.0.0rc1/redis/backoff.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/client.py` & `redis-5.0.0rc1/redis/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -327,17 +327,23 @@
         if first is not None:
             data["first-entry"] = (first[0], pairs_to_dict(first[1]))
         last = data["last-entry"]
         if last is not None:
             data["last-entry"] = (last[0], pairs_to_dict(last[1]))
     else:
         data["entries"] = {_id: pairs_to_dict(entry) for _id, entry in data["entries"]}
-        data["groups"] = [
-            pairs_to_dict(group, decode_keys=True) for group in data["groups"]
-        ]
+        if isinstance(data["groups"][0], list):
+            data["groups"] = [
+                pairs_to_dict(group, decode_keys=True) for group in data["groups"]
+            ]
+        else:
+            data["groups"] = [
+                {str_if_bytes(k): v for k, v in group.items()}
+                for group in data["groups"]
+            ]
     return data
 
 
 def parse_xread(response):
     if response is None:
         return []
     return [[r[0], parse_stream_list(r[1])] for r in response]
@@ -577,22 +583,23 @@
 def parse_command_resp3(response, **options):
     commands = {}
     for command in response:
         cmd_dict = {}
         cmd_name = str_if_bytes(command[0])
         cmd_dict["name"] = cmd_name
         cmd_dict["arity"] = command[1]
-        cmd_dict["flags"] = command[2]
+        cmd_dict["flags"] = {str_if_bytes(flag) for flag in command[2]}
         cmd_dict["first_key_pos"] = command[3]
         cmd_dict["last_key_pos"] = command[4]
         cmd_dict["step_count"] = command[5]
         cmd_dict["acl_categories"] = command[6]
-        cmd_dict["tips"] = command[7]
-        cmd_dict["key_specifications"] = command[8]
-        cmd_dict["subcommands"] = command[9]
+        if len(command) > 7:
+            cmd_dict["tips"] = command[7]
+            cmd_dict["key_specifications"] = command[8]
+            cmd_dict["subcommands"] = command[9]
 
         commands[cmd_name] = cmd_dict
     return commands
 
 
 def parse_pubsub_numsub(response, **options):
     return list(zip(response[0::2], response[1::2]))
@@ -622,25 +629,28 @@
         data["keys"] = []
     if "channels" in data:
         if isinstance(data["channels"], str) or isinstance(data["channels"], bytes):
             data["channels"] = list(str_if_bytes(data["channels"]).split(" "))
         if data["channels"] == [""]:
             data["channels"] = []
     if "selectors" in data:
-        data["selectors"] = [
-            list(map(str_if_bytes, selector)) for selector in data["selectors"]
-        ]
+        if data["selectors"] != [] and isinstance(data["selectors"][0], list):
+            data["selectors"] = [
+                list(map(str_if_bytes, selector)) for selector in data["selectors"]
+            ]
+        elif data["selectors"] != []:
+            data["selectors"] = [
+                {str_if_bytes(k): str_if_bytes(v) for k, v in selector.items()}
+                for selector in data["selectors"]
+            ]
 
     # split 'commands' into separate 'categories' and 'commands' lists
     commands, categories = [], []
     for command in data["commands"].split(" "):
-        if "@" in command:
-            categories.append(command)
-        else:
-            commands.append(command)
+        categories.append(command) if "@" in command else commands.append(command)
 
     data["commands"] = commands
     data["categories"] = categories
     data["enabled"] = "on" in data["flags"]
     return data
 
 
@@ -712,170 +722,166 @@
         # See `setGenericCommand` in t_string.c
         return response
     return response and str_if_bytes(response) == "OK"
 
 
 class AbstractRedis:
     RESPONSE_CALLBACKS = {
-        **string_keys_to_dict(
-            "AUTH COPY EXPIRE EXPIREAT PEXPIRE PEXPIREAT "
-            "HEXISTS HMSET MOVE MSETNX PERSIST "
-            "PSETEX RENAMENX SISMEMBER SMOVE SETEX SETNX",
-            bool,
-        ),
-        **string_keys_to_dict(
-            "BITCOUNT BITPOS DECRBY DEL EXISTS GEOADD GETBIT HDEL HLEN "
-            "HSTRLEN INCRBY LINSERT LLEN LPUSHX PFADD PFCOUNT RPUSHX SADD "
-            "SCARD SDIFFSTORE SETBIT SETRANGE SINTERSTORE SREM STRLEN "
-            "SUNIONSTORE UNLINK XACK XDEL XLEN XTRIM ZCARD ZLEXCOUNT ZREM "
-            "ZREMRANGEBYLEX ZREMRANGEBYRANK ZREMRANGEBYSCORE",
-            int,
-        ),
+        **string_keys_to_dict("EXPIRE EXPIREAT PEXPIRE PEXPIREAT AUTH", bool),
+        **string_keys_to_dict("EXISTS", int),
         **string_keys_to_dict("INCRBYFLOAT HINCRBYFLOAT", float),
-        **string_keys_to_dict(
-            # these return OK, or int if redis-server is >=1.3.4
-            "LPUSH RPUSH",
-            lambda r: isinstance(r, int) and r or str_if_bytes(r) == "OK",
-        ),
-        **string_keys_to_dict("SORT", sort_return_tuples),
-        **string_keys_to_dict("ZSCORE ZINCRBY GEODIST", float_or_none),
-        **string_keys_to_dict(
-            "FLUSHALL FLUSHDB LSET LTRIM MSET PFMERGE ASKING READONLY READWRITE "
-            "RENAME SAVE SELECT SHUTDOWN SLAVEOF SWAPDB WATCH UNWATCH ",
-            bool_ok,
-        ),
-        **string_keys_to_dict("BLPOP BRPOP", lambda r: r and tuple(r) or None),
-        **string_keys_to_dict(
-            "SDIFF SINTER SMEMBERS SUNION", lambda r: r and set(r) or set()
-        ),
-        **string_keys_to_dict(
-            "ZPOPMAX ZPOPMIN ZINTER ZDIFF ZUNION ZRANGE ZRANGEBYSCORE "
-            "ZREVRANGE ZREVRANGEBYSCORE",
-            zset_score_pairs,
-        ),
-        **string_keys_to_dict(
-            "BZPOPMIN BZPOPMAX", lambda r: r and (r[0], r[1], float(r[2])) or None
-        ),
-        **string_keys_to_dict("ZRANK ZREVRANK", int_or_none),
-        **string_keys_to_dict("XREVRANGE XRANGE", parse_stream_list),
-        **string_keys_to_dict("XREAD XREADGROUP", parse_xread),
-        **string_keys_to_dict("BGREWRITEAOF BGSAVE", lambda r: True),
-        "ACL CAT": lambda r: list(map(str_if_bytes, r)),
-        "ACL DELUSER": int,
-        "ACL GENPASS": str_if_bytes,
-        "ACL GETUSER": parse_acl_getuser,
-        "ACL HELP": lambda r: list(map(str_if_bytes, r)),
-        "ACL LIST": lambda r: list(map(str_if_bytes, r)),
-        "ACL LOAD": bool_ok,
-        "ACL LOG": parse_acl_log,
-        "ACL SAVE": bool_ok,
-        "ACL SETUSER": bool_ok,
-        "ACL USERS": lambda r: list(map(str_if_bytes, r)),
-        "ACL WHOAMI": str_if_bytes,
-        "CLIENT GETNAME": str_if_bytes,
+        **string_keys_to_dict("READONLY MSET", bool_ok),
+        "CLUSTER DELSLOTS": bool_ok,
+        "CLUSTER ADDSLOTS": bool_ok,
+        "COMMAND": parse_command,
+        "INFO": parse_info,
+        "SET": parse_set_result,
         "CLIENT ID": int,
         "CLIENT KILL": parse_client_kill,
         "CLIENT LIST": parse_client_list,
         "CLIENT INFO": parse_client_info,
         "CLIENT SETNAME": bool_ok,
-        "CLIENT UNBLOCK": lambda r: r and int(r) == 1 or False,
-        "CLIENT PAUSE": bool_ok,
-        "CLIENT GETREDIR": int,
         "CLIENT TRACKINGINFO": lambda r: list(map(str_if_bytes, r)),
-        "CLUSTER ADDSLOTS": bool_ok,
-        "CLUSTER ADDSLOTSRANGE": bool_ok,
+        "LASTSAVE": timestamp_to_datetime,
+        "RESET": str_if_bytes,
+        "SLOWLOG GET": parse_slowlog_get,
+        "TIME": lambda x: (int(x[0]), int(x[1])),
+        **string_keys_to_dict("BLPOP BRPOP", lambda r: r and tuple(r) or None),
+        "SCAN": parse_scan,
+        "CLIENT GETNAME": str_if_bytes,
+        "SSCAN": parse_scan,
+        "ACL LOG": parse_acl_log,
+        "ACL WHOAMI": str_if_bytes,
+        "ACL GENPASS": str_if_bytes,
+        "ACL CAT": lambda r: list(map(str_if_bytes, r)),
+        "HSCAN": parse_hscan,
+        "ZSCAN": parse_zscan,
+        **string_keys_to_dict(
+            "BZPOPMIN BZPOPMAX", lambda r: r and (r[0], r[1], float(r[2])) or None
+        ),
         "CLUSTER COUNT-FAILURE-REPORTS": lambda x: int(x),
         "CLUSTER COUNTKEYSINSLOT": lambda x: int(x),
-        "CLUSTER DELSLOTS": bool_ok,
-        "CLUSTER DELSLOTSRANGE": bool_ok,
         "CLUSTER FAILOVER": bool_ok,
         "CLUSTER FORGET": bool_ok,
-        "CLUSTER GETKEYSINSLOT": lambda r: list(map(str_if_bytes, r)),
         "CLUSTER INFO": parse_cluster_info,
         "CLUSTER KEYSLOT": lambda x: int(x),
         "CLUSTER MEET": bool_ok,
         "CLUSTER NODES": parse_cluster_nodes,
-        "CLUSTER REPLICAS": parse_cluster_nodes,
         "CLUSTER REPLICATE": bool_ok,
         "CLUSTER RESET": bool_ok,
         "CLUSTER SAVECONFIG": bool_ok,
-        "CLUSTER SET-CONFIG-EPOCH": bool_ok,
         "CLUSTER SETSLOT": bool_ok,
         "CLUSTER SLAVES": parse_cluster_nodes,
-        "COMMAND": parse_command,
-        "COMMAND COUNT": int,
-        "COMMAND GETKEYS": lambda r: list(map(str_if_bytes, r)),
-        "CONFIG GET": parse_config_get,
-        "CONFIG RESETSTAT": bool_ok,
-        "CONFIG SET": bool_ok,
-        "DEBUG OBJECT": parse_debug_object,
-        "FUNCTION DELETE": bool_ok,
-        "FUNCTION FLUSH": bool_ok,
-        "FUNCTION RESTORE": bool_ok,
+        **string_keys_to_dict("GEODIST", float_or_none),
         "GEOHASH": lambda r: list(map(str_if_bytes, r)),
         "GEOPOS": lambda r: list(
             map(lambda ll: (float(ll[0]), float(ll[1])) if ll is not None else None, r)
         ),
         "GEOSEARCH": parse_geosearch_generic,
         "GEORADIUS": parse_geosearch_generic,
         "GEORADIUSBYMEMBER": parse_geosearch_generic,
-        "HGETALL": lambda r: r and pairs_to_dict(r) or {},
-        "HSCAN": parse_hscan,
-        "INFO": parse_info,
-        "LASTSAVE": timestamp_to_datetime,
-        "MEMORY PURGE": bool_ok,
-        "MEMORY STATS": parse_memory_stats,
-        "MEMORY USAGE": int_or_none,
-        "MODULE LOAD": parse_module_result,
-        "MODULE UNLOAD": parse_module_result,
-        "MODULE LIST": lambda r: [pairs_to_dict(m) for m in r],
-        "OBJECT": parse_object,
+        "XAUTOCLAIM": parse_xautoclaim,
+        "XINFO STREAM": parse_xinfo_stream,
+        "XPENDING": parse_xpending,
+        **string_keys_to_dict("XREAD XREADGROUP", parse_xread),
+        "COMMAND GETKEYS": lambda r: list(map(str_if_bytes, r)),
+        **string_keys_to_dict("SORT", sort_return_tuples),
         "PING": lambda r: str_if_bytes(r) == "PONG",
-        "QUIT": bool_ok,
-        "STRALGO": parse_stralgo,
+        "ACL SETUSER": bool_ok,
         "PUBSUB NUMSUB": parse_pubsub_numsub,
-        "PUBSUB SHARDNUMSUB": parse_pubsub_numsub,
-        "RANDOMKEY": lambda r: r and r or None,
-        "RESET": str_if_bytes,
-        "SCAN": parse_scan,
-        "SCRIPT EXISTS": lambda r: list(map(bool, r)),
         "SCRIPT FLUSH": bool_ok,
-        "SCRIPT KILL": bool_ok,
         "SCRIPT LOAD": str_if_bytes,
-        "SENTINEL CKQUORUM": bool_ok,
-        "SENTINEL FAILOVER": bool_ok,
-        "SENTINEL FLUSHCONFIG": bool_ok,
-        "SENTINEL GET-MASTER-ADDR-BY-NAME": parse_sentinel_get_master,
-        "SENTINEL MASTER": parse_sentinel_master,
-        "SENTINEL MASTERS": parse_sentinel_masters,
-        "SENTINEL MONITOR": bool_ok,
-        "SENTINEL RESET": bool_ok,
-        "SENTINEL REMOVE": bool_ok,
-        "SENTINEL SENTINELS": parse_sentinel_slaves_and_sentinels,
-        "SENTINEL SET": bool_ok,
-        "SENTINEL SLAVES": parse_sentinel_slaves_and_sentinels,
-        "SET": parse_set_result,
-        "SLOWLOG GET": parse_slowlog_get,
-        "SLOWLOG LEN": int,
-        "SLOWLOG RESET": bool_ok,
-        "SSCAN": parse_scan,
-        "TIME": lambda x: (int(x[0]), int(x[1])),
+        "ACL GETUSER": parse_acl_getuser,
+        "CONFIG SET": bool_ok,
+        **string_keys_to_dict("XREVRANGE XRANGE", parse_stream_list),
         "XCLAIM": parse_xclaim,
-        "XAUTOCLAIM": parse_xautoclaim,
-        "XGROUP CREATE": bool_ok,
-        "XGROUP DELCONSUMER": int,
-        "XGROUP DESTROY": bool,
-        "XGROUP SETID": bool_ok,
-        "XINFO CONSUMERS": parse_list_of_dicts,
-        "XINFO GROUPS": parse_list_of_dicts,
-        "XINFO STREAM": parse_xinfo_stream,
-        "XPENDING": parse_xpending,
+        "CLUSTER SET-CONFIG-EPOCH": bool_ok,
+        "CLUSTER REPLICAS": parse_cluster_nodes,
+        "ACL LIST": lambda r: list(map(str_if_bytes, r)),
+    }
+
+    RESP2_RESPONSE_CALLBACKS = {
+        "CONFIG GET": parse_config_get,
+        **string_keys_to_dict(
+            "SDIFF SINTER SMEMBERS SUNION", lambda r: r and set(r) or set()
+        ),
+        **string_keys_to_dict("READWRITE", bool_ok),
+        **string_keys_to_dict(
+            "ZPOPMAX ZPOPMIN ZINTER ZDIFF ZUNION ZRANGE ZRANGEBYSCORE "
+            "ZREVRANGE ZREVRANGEBYSCORE",
+            zset_score_pairs,
+        ),
+        **string_keys_to_dict("ZSCORE ZINCRBY", float_or_none),
         "ZADD": parse_zadd,
-        "ZSCAN": parse_zscan,
         "ZMSCORE": parse_zmscore,
+        "HGETALL": lambda r: r and pairs_to_dict(r) or {},
+        "MEMORY STATS": parse_memory_stats,
+        "MODULE LIST": lambda r: [pairs_to_dict(m) for m in r],
+        "STRALGO": parse_stralgo,
+        # **string_keys_to_dict(
+        #     "COPY "
+        #     "HEXISTS HMSET MOVE MSETNX PERSIST "
+        #     "PSETEX RENAMENX SMOVE SETEX SETNX",
+        #     bool,
+        # ),
+        # **string_keys_to_dict(
+        #     "HSTRLEN INCRBY LINSERT LLEN LPUSHX PFADD PFCOUNT RPUSHX SADD "
+        #     "SCARD SDIFFSTORE SETBIT SETRANGE SINTERSTORE SREM STRLEN "
+        #     "SUNIONSTORE UNLINK XACK XDEL XLEN XTRIM ZCARD ZLEXCOUNT ZREM "
+        #     "ZREMRANGEBYLEX ZREMRANGEBYRANK ZREMRANGEBYSCORE",
+        #     int,
+        # ),
+        # **string_keys_to_dict(
+        #     "FLUSHALL FLUSHDB LSET LTRIM PFMERGE ASKING "
+        #     "RENAME SAVE SELECT SHUTDOWN SLAVEOF SWAPDB WATCH UNWATCH ",
+        #     bool_ok,
+        # ),
+        # **string_keys_to_dict("ZRANK ZREVRANK", int_or_none),
+        # **string_keys_to_dict("BGREWRITEAOF BGSAVE", lambda r: True),
+        # "ACL HELP": lambda r: list(map(str_if_bytes, r)),
+        # "ACL LOAD": bool_ok,
+        # "ACL SAVE": bool_ok,
+        # "ACL USERS": lambda r: list(map(str_if_bytes, r)),
+        # "CLIENT UNBLOCK": lambda r: r and int(r) == 1 or False,
+        # "CLIENT PAUSE": bool_ok,
+        # "CLUSTER ADDSLOTSRANGE": bool_ok,
+        # "CLUSTER DELSLOTSRANGE": bool_ok,
+        # "CLUSTER GETKEYSINSLOT": lambda r: list(map(str_if_bytes, r)),
+        # "CONFIG RESETSTAT": bool_ok,
+        # "DEBUG OBJECT": parse_debug_object,
+        # "FUNCTION DELETE": bool_ok,
+        # "FUNCTION FLUSH": bool_ok,
+        # "FUNCTION RESTORE": bool_ok,
+        # "MEMORY PURGE": bool_ok,
+        # "MEMORY USAGE": int_or_none,
+        # "MODULE LOAD": parse_module_result,
+        # "MODULE UNLOAD": parse_module_result,
+        # "OBJECT": parse_object,
+        # "QUIT": bool_ok,
+        # "RANDOMKEY": lambda r: r and r or None,
+        # "SCRIPT EXISTS": lambda r: list(map(bool, r)),
+        # "SCRIPT KILL": bool_ok,
+        # "SENTINEL CKQUORUM": bool_ok,
+        # "SENTINEL FAILOVER": bool_ok,
+        # "SENTINEL FLUSHCONFIG": bool_ok,
+        # "SENTINEL GET-MASTER-ADDR-BY-NAME": parse_sentinel_get_master,
+        # "SENTINEL MASTER": parse_sentinel_master,
+        # "SENTINEL MASTERS": parse_sentinel_masters,
+        # "SENTINEL MONITOR": bool_ok,
+        # "SENTINEL RESET": bool_ok,
+        # "SENTINEL REMOVE": bool_ok,
+        # "SENTINEL SENTINELS": parse_sentinel_slaves_and_sentinels,
+        # "SENTINEL SET": bool_ok,
+        # "SENTINEL SLAVES": parse_sentinel_slaves_and_sentinels,
+        # "SLOWLOG RESET": bool_ok,
+        # "XGROUP CREATE": bool_ok,
+        # "XGROUP DESTROY": bool,
+        # "XGROUP SETID": bool_ok,
+        "XINFO CONSUMERS": parse_list_of_dicts,
+        "XINFO GROUPS": parse_list_of_dicts,
     }
 
     RESP3_RESPONSE_CALLBACKS = {
         **string_keys_to_dict(
             "ZRANGE ZINTER ZPOPMAX ZPOPMIN ZRANGEBYSCORE ZREVRANGE ZREVRANGEBYSCORE "
             "ZUNION HGETALL XREADGROUP",
             lambda r, **kwargs: r,
@@ -1108,14 +1114,16 @@
         if single_connection_client:
             self.connection = self.connection_pool.get_connection("_")
 
         self.response_callbacks = CaseInsensitiveDict(self.__class__.RESPONSE_CALLBACKS)
 
         if self.connection_pool.connection_kwargs.get("protocol") in ["3", 3]:
             self.response_callbacks.update(self.__class__.RESP3_RESPONSE_CALLBACKS)
+        else:
+            self.response_callbacks.update(self.__class__.RESP2_RESPONSE_CALLBACKS)
 
     def __repr__(self):
         return f"{type(self).__name__}<{repr(self.connection_pool)}>"
 
     def get_encoder(self):
         """Get the connection pool's encoder"""
         return self.connection_pool.get_encoder()
```

### Comparing `redis-5.0.0b4/redis/cluster.py` & `redis-5.0.0rc1/redis/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     TimeoutError,
     TryAgainError,
 )
 from redis.lock import Lock
 from redis.parsers import CommandsParser, Encoder
 from redis.retry import Retry
 from redis.utils import (
+    HIREDIS_AVAILABLE,
     dict_merge,
     list_keys_to_dict,
     merge_result,
     safe_str,
     str_if_bytes,
 )
 
@@ -246,15 +247,14 @@
                 "CLIENT UNBLOCK",
                 "CLIENT ID",
                 "CLIENT REPLY",
                 "CLIENT GETREDIR",
                 "CLIENT INFO",
                 "CLIENT KILL",
                 "READONLY",
-                "READWRITE",
                 "CLUSTER INFO",
                 "CLUSTER MEET",
                 "CLUSTER NODES",
                 "CLUSTER REPLICAS",
                 "CLUSTER RESET",
                 "CLUSTER SET-CONFIG-EPOCH",
                 "CLUSTER SLOTS",
@@ -1604,15 +1604,23 @@
     Wrapper for PubSub class.
 
     IMPORTANT: before using ClusterPubSub, read about the known limitations
     with pubsub in Cluster mode and learn how to workaround them:
     https://redis-py-cluster.readthedocs.io/en/stable/pubsub.html
     """
 
-    def __init__(self, redis_cluster, node=None, host=None, port=None, **kwargs):
+    def __init__(
+        self,
+        redis_cluster,
+        node=None,
+        host=None,
+        port=None,
+        push_handler_func=None,
+        **kwargs,
+    ):
         """
         When a pubsub instance is created without specifying a node, a single
         node will be transparently chosen for the pubsub connection on the
         first command execution. The node will be determined by:
          1. Hashing the channel name in the request to find its keyslot
          2. Selecting a node that handles the keyslot: If read_from_replicas is
             set to true, a replica can be selected.
@@ -1629,15 +1637,18 @@
             if self.node is None
             else redis_cluster.get_redis_connection(self.node).connection_pool
         )
         self.cluster = redis_cluster
         self.node_pubsub_mapping = {}
         self._pubsubs_generator = self._pubsubs_generator()
         super().__init__(
-            **kwargs, connection_pool=connection_pool, encoder=redis_cluster.encoder
+            connection_pool=connection_pool,
+            encoder=redis_cluster.encoder,
+            push_handler_func=push_handler_func,
+            **kwargs,
         )
 
     def set_pubsub_node(self, cluster, node=None, host=None, port=None):
         """
         The pubsub node will be set according to the passed node, host and port
         When none of the node, host, or port are specified - the node is set
         to None and will be determined by the keyslot of the channel in the
@@ -1713,22 +1724,26 @@
                 self.connection_pool = redis_connection.connection_pool
             self.connection = self.connection_pool.get_connection(
                 "pubsub", self.shard_hint
             )
             # register a callback that re-subscribes to any channels we
             # were listening to when we were disconnected
             self.connection.register_connect_callback(self.on_connect)
+            if self.push_handler_func is not None and not HIREDIS_AVAILABLE:
+                self.connection._parser.set_push_handler(self.push_handler_func)
         connection = self.connection
         self._execute(connection, connection.send_command, *args)
 
     def _get_node_pubsub(self, node):
         try:
             return self.node_pubsub_mapping[node.name]
         except KeyError:
-            pubsub = node.redis_connection.pubsub()
+            pubsub = node.redis_connection.pubsub(
+                push_handler_func=self.push_handler_func
+            )
             self.node_pubsub_mapping[node.name] = pubsub
             return pubsub
 
     def _sharded_message_generator(self):
         for _ in range(len(self.node_pubsub_mapping)):
             pubsub = next(self._pubsubs_generator)
             message = pubsub.get_message()
```

### Comparing `redis-5.0.0b4/redis/commands/__init__.py` & `redis-5.0.0rc1/redis/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/bf/commands.py` & `redis-5.0.0rc1/redis/commands/bf/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 TDIGEST_BYRANK = "TDIGEST.BYRANK"
 TDIGEST_BYREVRANK = "TDIGEST.BYREVRANK"
 
 
 class BFCommands:
     """Bloom Filter commands."""
 
-    # region Bloom Filter Functions
     def create(self, key, errorRate, capacity, expansion=None, noScale=None):
         """
         Create a new Bloom Filter `key` with desired probability of false positives
         `errorRate` expected entries to be inserted as `capacity`.
         Default expansion value is 2. By default, filter is auto-scaling.
         For more information see `BF.RESERVE <https://redis.io/commands/bf.reserve>`_.
         """  # noqa
@@ -174,15 +173,14 @@
         """  # noqa
         return self.execute_command(BF_CARD, key)
 
 
 class CFCommands:
     """Cuckoo Filter commands."""
 
-    # region Cuckoo Filter Functions
     def create(
         self, key, capacity, expansion=None, bucket_size=None, max_iterations=None
     ):
         """
         Create a new Cuckoo Filter `key` an initial `capacity` items.
         For more information see `CF.RESERVE <https://redis.io/commands/cf.reserve>`_.
         """  # noqa
@@ -484,15 +482,14 @@
         """  # noqa
         return self.execute_command(TDIGEST_BYREVRANK, key, rank, *ranks)
 
 
 class CMSCommands:
     """Count-Min Sketch Commands"""
 
-    # region Count-Min Sketch Functions
     def initbydim(self, key, width, depth):
         """
         Initialize a Count-Min Sketch `key` to dimensions (`width`, `depth`) specified by user.
         For more information see `CMS.INITBYDIM <https://redis.io/commands/cms.initbydim>`_.
         """  # noqa
         return self.execute_command(CMS_INITBYDIM, key, width, depth)
```

### Comparing `redis-5.0.0b4/redis/commands/bf/info.py` & `redis-5.0.0rc1/redis/commands/bf/info.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,14 +12,23 @@
         response = dict(zip(map(nativestr, args[::2]), args[1::2]))
         self.capacity = response["Capacity"]
         self.size = response["Size"]
         self.filterNum = response["Number of filters"]
         self.insertedNum = response["Number of items inserted"]
         self.expansionRate = response["Expansion rate"]
 
+    def get(self, item):
+        try:
+            return self.__getitem__(item)
+        except AttributeError:
+            return None
+
+    def __getitem__(self, item):
+        return getattr(self, item)
+
 
 class CFInfo(object):
     size = None
     bucketNum = None
     filterNum = None
     insertedNum = None
     deletedNum = None
@@ -34,40 +43,55 @@
         self.filterNum = response["Number of filters"]
         self.insertedNum = response["Number of items inserted"]
         self.deletedNum = response["Number of items deleted"]
         self.bucketSize = response["Bucket size"]
         self.expansionRate = response["Expansion rate"]
         self.maxIteration = response["Max iterations"]
 
+    def get(self, item):
+        try:
+            return self.__getitem__(item)
+        except AttributeError:
+            return None
+
+    def __getitem__(self, item):
+        return getattr(self, item)
+
 
 class CMSInfo(object):
     width = None
     depth = None
     count = None
 
     def __init__(self, args):
         response = dict(zip(map(nativestr, args[::2]), args[1::2]))
         self.width = response["width"]
         self.depth = response["depth"]
         self.count = response["count"]
 
+    def __getitem__(self, item):
+        return getattr(self, item)
+
 
 class TopKInfo(object):
     k = None
     width = None
     depth = None
     decay = None
 
     def __init__(self, args):
         response = dict(zip(map(nativestr, args[::2]), args[1::2]))
         self.k = response["k"]
         self.width = response["width"]
         self.depth = response["depth"]
         self.decay = response["decay"]
 
+    def __getitem__(self, item):
+        return getattr(self, item)
+
 
 class TDigestInfo(object):
     compression = None
     capacity = None
     merged_nodes = None
     unmerged_nodes = None
     merged_weight = None
@@ -81,7 +105,16 @@
         self.capacity = response["Capacity"]
         self.merged_nodes = response["Merged nodes"]
         self.unmerged_nodes = response["Unmerged nodes"]
         self.merged_weight = response["Merged weight"]
         self.unmerged_weight = response["Unmerged weight"]
         self.total_compressions = response["Total compressions"]
         self.memory_usage = response["Memory usage"]
+
+    def get(self, item):
+        try:
+            return self.__getitem__(item)
+        except AttributeError:
+            return None
+
+    def __getitem__(self, item):
+        return getattr(self, item)
```

### Comparing `redis-5.0.0b4/redis/commands/cluster.py` & `redis-5.0.0rc1/redis/commands/cluster.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/core.py` & `redis-5.0.0rc1/redis/commands/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -3335,17 +3335,21 @@
         set named ``dest``.  Returns the number of keys in the new set.
 
         For more information see https://redis.io/commands/sinterstore
         """
         args = list_or_args(keys, args)
         return self.execute_command("SINTERSTORE", dest, *args)
 
-    def sismember(self, name: str, value: str) -> Union[Awaitable[bool], bool]:
+    def sismember(
+        self, name: str, value: str
+    ) -> Union[Awaitable[Union[Literal[0], Literal[1]]], Union[Literal[0], Literal[1]]]:
         """
-        Return a boolean indicating if ``value`` is a member of set ``name``
+        Return whether ``value`` is a member of set ``name``:
+        - 1 if the value is a member of the set.
+        - 0 if the value is not a member of the set or if key does not exist.
 
         For more information see https://redis.io/commands/sismember
         """
         return self.execute_command("SISMEMBER", name, value)
 
     def smembers(self, name: str) -> Union[Awaitable[Set], Set]:
         """
```

### Comparing `redis-5.0.0b4/redis/commands/graph/__init__.py` & `redis-5.0.0rc1/redis/commands/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/graph/commands.py` & `redis-5.0.0rc1/redis/commands/graph/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/graph/edge.py` & `redis-5.0.0rc1/redis/commands/graph/edge.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/graph/execution_plan.py` & `redis-5.0.0rc1/redis/commands/graph/execution_plan.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/graph/node.py` & `redis-5.0.0rc1/redis/commands/graph/node.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/graph/path.py` & `redis-5.0.0rc1/redis/commands/graph/path.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/graph/query_result.py` & `redis-5.0.0rc1/redis/commands/graph/query_result.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/helpers.py` & `redis-5.0.0rc1/redis/commands/helpers.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/json/__init__.py` & `redis-5.0.0rc1/redis/commands/json/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,41 +28,58 @@
         :type json.JSONDecoder: An instance of json.JSONDecoder
 
         :param encoder:
         :type json.JSONEncoder: An instance of json.JSONEncoder
         """
         # Set the module commands' callbacks
         self.MODULE_CALLBACKS = {
-            "JSON.CLEAR": int,
-            "JSON.DEL": int,
-            "JSON.FORGET": int,
-            "JSON.GET": self._decode,
+            "JSON.ARRPOP": self._decode,
             "JSON.MGET": bulk_of_jsons(self._decode),
             "JSON.SET": lambda r: r and nativestr(r) == "OK",
-            "JSON.NUMINCRBY": self._decode,
-            "JSON.NUMMULTBY": self._decode,
+            "JSON.DEBUG": self._decode,
             "JSON.TOGGLE": self._decode,
-            "JSON.STRAPPEND": self._decode,
-            "JSON.STRLEN": self._decode,
+            "JSON.RESP": self._decode,
+        }
+
+        RESP2_MODULE_CALLBACKS = {
+            "JSON.ARRTRIM": self._decode,
+            "JSON.OBJLEN": self._decode,
             "JSON.ARRAPPEND": self._decode,
             "JSON.ARRINDEX": self._decode,
             "JSON.ARRINSERT": self._decode,
+            "JSON.TOGGLE": self._decode,
+            "JSON.STRAPPEND": self._decode,
+            "JSON.STRLEN": self._decode,
             "JSON.ARRLEN": self._decode,
-            "JSON.ARRPOP": self._decode,
-            "JSON.ARRTRIM": self._decode,
-            "JSON.OBJLEN": self._decode,
+            "JSON.CLEAR": int,
+            "JSON.DEL": int,
+            "JSON.FORGET": int,
+            "JSON.NUMINCRBY": self._decode,
+            "JSON.NUMMULTBY": self._decode,
             "JSON.OBJKEYS": self._decode,
-            "JSON.RESP": self._decode,
-            "JSON.DEBUG": self._decode,
+            "JSON.GET": self._decode,
+        }
+
+        RESP3_MODULE_CALLBACKS = {
+            "JSON.GET": lambda response: [
+                [self._decode(r) for r in res] for res in response
+            ]
+            if response
+            else response
         }
 
         self.client = client
         self.execute_command = client.execute_command
         self.MODULE_VERSION = version
 
+        if self.client.connection_pool.connection_kwargs.get("protocol") in ["3", 3]:
+            self.MODULE_CALLBACKS.update(RESP3_MODULE_CALLBACKS)
+        else:
+            self.MODULE_CALLBACKS.update(RESP2_MODULE_CALLBACKS)
+
         for key, value in self.MODULE_CALLBACKS.items():
             self.client.set_response_callback(key, value)
 
         self.__encoder__ = encoder
         self.__decoder__ = decoder
 
     def _decode(self, obj):
```

### Comparing `redis-5.0.0b4/redis/commands/json/commands.py` & `redis-5.0.0rc1/redis/commands/json/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/json/decoders.py` & `redis-5.0.0rc1/redis/commands/json/decoders.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/redismodules.py` & `redis-5.0.0rc1/redis/commands/redismodules.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/search/__init__.py` & `redis-5.0.0rc1/redis/commands/search/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 import redis
 
 from ...asyncio.client import Pipeline as AsyncioPipeline
-from .commands import AsyncSearchCommands, SearchCommands
+from .commands import (
+    AGGREGATE_CMD,
+    CONFIG_CMD,
+    INFO_CMD,
+    PROFILE_CMD,
+    SEARCH_CMD,
+    SPELLCHECK_CMD,
+    SYNDUMP_CMD,
+    AsyncSearchCommands,
+    SearchCommands,
+)
 
 
 class Search(SearchCommands):
     """
     Create a client for talking to search.
     It abstracts the API of the module and lets you just use the engine.
     """
@@ -86,14 +96,23 @@
         If conn is not None, we employ an already existing redis connection
         """
         self.MODULE_CALLBACKS = {}
         self.client = client
         self.index_name = index_name
         self.execute_command = client.execute_command
         self._pipeline = client.pipeline
+        self.RESP2_MODULE_CALLBACKS = {
+            INFO_CMD: self._parse_info,
+            SEARCH_CMD: self._parse_search,
+            AGGREGATE_CMD: self._parse_aggregate,
+            PROFILE_CMD: self._parse_profile,
+            SPELLCHECK_CMD: self._parse_spellcheck,
+            CONFIG_CMD: self._parse_config_get,
+            SYNDUMP_CMD: self._parse_syndump,
+        }
 
     def pipeline(self, transaction=True, shard_hint=None):
         """Creates a pipeline for the SEARCH module, that can be used for executing
         SEARCH commands, as well as classic core commands.
         """
         p = Pipeline(
             connection_pool=self.client.connection_pool,
```

### Comparing `redis-5.0.0b4/redis/commands/search/aggregation.py` & `redis-5.0.0rc1/redis/commands/search/aggregation.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/search/commands.py` & `redis-5.0.0rc1/redis/commands/search/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,94 @@
 FUZZY = "FUZZY"
 WITHPAYLOADS = "WITHPAYLOADS"
 
 
 class SearchCommands:
     """Search commands."""
 
+    def _parse_results(self, cmd, res, **kwargs):
+        if self.client.connection_pool.connection_kwargs.get("protocol") in ["3", 3]:
+            return res
+        else:
+            return self.RESP2_MODULE_CALLBACKS[cmd](res, **kwargs)
+
+    def _parse_info(self, res, **kwargs):
+        it = map(to_string, res)
+        return dict(zip(it, it))
+
+    def _parse_search(self, res, **kwargs):
+        return Result(
+            res,
+            not kwargs["query"]._no_content,
+            duration=kwargs["duration"],
+            has_payload=kwargs["query"]._with_payloads,
+            with_scores=kwargs["query"]._with_scores,
+        )
+
+    def _parse_aggregate(self, res, **kwargs):
+        return self._get_aggregate_result(res, kwargs["query"], kwargs["has_cursor"])
+
+    def _parse_profile(self, res, **kwargs):
+        query = kwargs["query"]
+        if isinstance(query, AggregateRequest):
+            result = self._get_aggregate_result(res[0], query, query._cursor)
+        else:
+            result = Result(
+                res[0],
+                not query._no_content,
+                duration=kwargs["duration"],
+                has_payload=query._with_payloads,
+                with_scores=query._with_scores,
+            )
+
+        return result, parse_to_dict(res[1])
+
+    def _parse_spellcheck(self, res, **kwargs):
+        corrections = {}
+        if res == 0:
+            return corrections
+
+        for _correction in res:
+            if isinstance(_correction, int) and _correction == 0:
+                continue
+
+            if len(_correction) != 3:
+                continue
+            if not _correction[2]:
+                continue
+            if not _correction[2][0]:
+                continue
+
+            # For spellcheck output
+            # 1)  1) "TERM"
+            #     2) "{term1}"
+            #     3)  1)  1)  "{score1}"
+            #             2)  "{suggestion1}"
+            #         2)  1)  "{score2}"
+            #             2)  "{suggestion2}"
+            #
+            # Following dictionary will be made
+            # corrections = {
+            #     '{term1}': [
+            #         {'score': '{score1}', 'suggestion': '{suggestion1}'},
+            #         {'score': '{score2}', 'suggestion': '{suggestion2}'}
+            #     ]
+            # }
+            corrections[_correction[1]] = [
+                {"score": _item[0], "suggestion": _item[1]} for _item in _correction[2]
+            ]
+
+        return corrections
+
+    def _parse_config_get(self, res, **kwargs):
+        return {kvs[0]: kvs[1] for kvs in res} if res else {}
+
+    def _parse_syndump(self, res, **kwargs):
+        return {res[i]: res[i + 1] for i in range(0, len(res), 2)}
+
     def batch_indexer(self, chunk_size=100):
         """
         Create a new batch indexer from the client with a given chunk size
         """
         return self.BatchIndexer(self, chunk_size=chunk_size)
 
     def create_index(
@@ -364,16 +444,15 @@
         Get info an stats about the the current index, including the number of
         documents, memory consumption, etc
 
         For more information see `FT.INFO <https://redis.io/commands/ft.info>`_.
         """
 
         res = self.execute_command(INFO_CMD, self.index_name)
-        it = map(to_string, res)
-        return dict(zip(it, it))
+        return self._parse_results(INFO_CMD, res)
 
     def get_params_args(
         self, query_params: Union[Dict[str, Union[str, int, float]], None]
     ):
         if query_params is None:
             return []
         args = []
@@ -418,20 +497,16 @@
         args, query = self._mk_query_args(query, query_params=query_params)
         st = time.time()
         res = self.execute_command(SEARCH_CMD, *args)
 
         if isinstance(res, Pipeline):
             return res
 
-        return Result(
-            res,
-            not query._no_content,
-            duration=(time.time() - st) * 1000.0,
-            has_payload=query._with_payloads,
-            with_scores=query._with_scores,
+        return self._parse_results(
+            SEARCH_CMD, res, query=query, duration=(time.time() - st) * 1000.0
         )
 
     def explain(
         self,
         query: Union[str, Query],
         query_params: Dict[str, Union[str, int, float]] = None,
     ):
@@ -469,15 +544,17 @@
             has_cursor = True
             cmd = [CURSOR_CMD, "READ", self.index_name] + query.build_args()
         else:
             raise ValueError("Bad query", query)
         cmd += self.get_params_args(query_params)
 
         raw = self.execute_command(*cmd)
-        return self._get_aggregate_result(raw, query, has_cursor)
+        return self._parse_results(
+            AGGREGATE_CMD, raw, query=query, has_cursor=has_cursor
+        )
 
     def _get_aggregate_result(self, raw, query, has_cursor):
         if has_cursor:
             if isinstance(query, Cursor):
                 query.cid = raw[1]
                 cursor = query
             else:
@@ -527,26 +604,17 @@
             cmd += query.get_args()
             cmd += self.get_params_args(query_params)
         else:
             raise ValueError("Must provide AggregateRequest object or Query object.")
 
         res = self.execute_command(*cmd)
 
-        if isinstance(query, AggregateRequest):
-            result = self._get_aggregate_result(res[0], query, query._cursor)
-        else:
-            result = Result(
-                res[0],
-                not query._no_content,
-                duration=(time.time() - st) * 1000.0,
-                has_payload=query._with_payloads,
-                with_scores=query._with_scores,
-            )
-
-        return result, parse_to_dict(res[1])
+        return self._parse_results(
+            PROFILE_CMD, res, query=query, duration=(time.time() - st) * 1000.0
+        )
 
     def spellcheck(self, query, distance=None, include=None, exclude=None):
         """
         Issue a spellcheck query
 
         ### Parameters
 
@@ -564,51 +632,17 @@
 
         if include:
             cmd.extend(["TERMS", "INCLUDE", include])
 
         if exclude:
             cmd.extend(["TERMS", "EXCLUDE", exclude])
 
-        raw = self.execute_command(*cmd)
-
-        corrections = {}
-        if raw == 0:
-            return corrections
-
-        for _correction in raw:
-            if isinstance(_correction, int) and _correction == 0:
-                continue
-
-            if len(_correction) != 3:
-                continue
-            if not _correction[2]:
-                continue
-            if not _correction[2][0]:
-                continue
-
-            # For spellcheck output
-            # 1)  1) "TERM"
-            #     2) "{term1}"
-            #     3)  1)  1)  "{score1}"
-            #             2)  "{suggestion1}"
-            #         2)  1)  "{score2}"
-            #             2)  "{suggestion2}"
-            #
-            # Following dictionary will be made
-            # corrections = {
-            #     '{term1}': [
-            #         {'score': '{score1}', 'suggestion': '{suggestion1}'},
-            #         {'score': '{score2}', 'suggestion': '{suggestion2}'}
-            #     ]
-            # }
-            corrections[_correction[1]] = [
-                {"score": _item[0], "suggestion": _item[1]} for _item in _correction[2]
-            ]
+        res = self.execute_command(*cmd)
 
-        return corrections
+        return self._parse_results(SPELLCHECK_CMD, res)
 
     def dict_add(self, name, *terms):
         """Adds terms to a dictionary.
 
         ### Parameters
 
         - **name**: Dictionary name.
@@ -666,20 +700,16 @@
         ### Parameters
 
         - **option**: the name of the configuration option.
 
         For more information see `FT.CONFIG GET <https://redis.io/commands/ft.config-get>`_.
         """  # noqa
         cmd = [CONFIG_CMD, "GET", option]
-        res = {}
-        raw = self.execute_command(*cmd)
-        if raw:
-            for kvs in raw:
-                res[kvs[0]] = kvs[1]
-        return res
+        res = self.execute_command(*cmd)
+        return self._parse_results(CONFIG_CMD, res)
 
     def tagvals(self, tagfield):
         """
         Return a list of all possible tag values
 
         ### Parameters
 
@@ -806,20 +836,20 @@
         if fuzzy:
             args.append(FUZZY)
         if with_scores:
             args.append(WITHSCORES)
         if with_payloads:
             args.append(WITHPAYLOADS)
 
-        ret = self.execute_command(*args)
+        res = self.execute_command(*args)
         results = []
-        if not ret:
+        if not res:
             return results
 
-        parser = SuggestionParser(with_scores, with_payloads, ret)
+        parser = SuggestionParser(with_scores, with_payloads, res)
         return [s for s in parser]
 
     def synupdate(self, groupid, skipinitial=False, *terms):
         """
         Updates a synonym group.
         The command is used to create or update a synonym group with
         additional terms.
@@ -847,30 +877,29 @@
         Dumps the contents of a synonym group.
 
         The command is used to dump the synonyms data structure.
         Returns a list of synonym terms and their synonym group ids.
 
         For more information see `FT.SYNDUMP <https://redis.io/commands/ft.syndump>`_.
         """  # noqa
-        raw = self.execute_command(SYNDUMP_CMD, self.index_name)
-        return {raw[i]: raw[i + 1] for i in range(0, len(raw), 2)}
+        res = self.execute_command(SYNDUMP_CMD, self.index_name)
+        return self._parse_results(SYNDUMP_CMD, res)
 
 
 class AsyncSearchCommands(SearchCommands):
     async def info(self):
         """
         Get info an stats about the the current index, including the number of
         documents, memory consumption, etc
 
         For more information see `FT.INFO <https://redis.io/commands/ft.info>`_.
         """
 
         res = await self.execute_command(INFO_CMD, self.index_name)
-        it = map(to_string, res)
-        return dict(zip(it, it))
+        return self._parse_results(INFO_CMD, res)
 
     async def search(
         self,
         query: Union[str, Query],
         query_params: Dict[str, Union[str, int, float]] = None,
     ):
         """
@@ -887,20 +916,16 @@
         args, query = self._mk_query_args(query, query_params=query_params)
         st = time.time()
         res = await self.execute_command(SEARCH_CMD, *args)
 
         if isinstance(res, Pipeline):
             return res
 
-        return Result(
-            res,
-            not query._no_content,
-            duration=(time.time() - st) * 1000.0,
-            has_payload=query._with_payloads,
-            with_scores=query._with_scores,
+        return self._parse_results(
+            SEARCH_CMD, res, query=query, duration=(time.time() - st) * 1000.0
         )
 
     async def aggregate(
         self,
         query: Union[str, Query],
         query_params: Dict[str, Union[str, int, float]] = None,
     ):
@@ -923,15 +948,17 @@
             has_cursor = True
             cmd = [CURSOR_CMD, "READ", self.index_name] + query.build_args()
         else:
             raise ValueError("Bad query", query)
         cmd += self.get_params_args(query_params)
 
         raw = await self.execute_command(*cmd)
-        return self._get_aggregate_result(raw, query, has_cursor)
+        return self._parse_results(
+            AGGREGATE_CMD, raw, query=query, has_cursor=has_cursor
+        )
 
     async def spellcheck(self, query, distance=None, include=None, exclude=None):
         """
         Issue a spellcheck query
 
         ### Parameters
 
@@ -949,36 +976,17 @@
 
         if include:
             cmd.extend(["TERMS", "INCLUDE", include])
 
         if exclude:
             cmd.extend(["TERMS", "EXCLUDE", exclude])
 
-        raw = await self.execute_command(*cmd)
-
-        corrections = {}
-        if raw == 0:
-            return corrections
-
-        for _correction in raw:
-            if isinstance(_correction, int) and _correction == 0:
-                continue
+        res = await self.execute_command(*cmd)
 
-            if len(_correction) != 3:
-                continue
-            if not _correction[2]:
-                continue
-            if not _correction[2][0]:
-                continue
-
-            corrections[_correction[1]] = [
-                {"score": _item[0], "suggestion": _item[1]} for _item in _correction[2]
-            ]
-
-        return corrections
+        return self._parse_results(SPELLCHECK_CMD, res)
 
     async def config_set(self, option, value):
         """Set runtime configuration option.
 
         ### Parameters
 
         - **option**: the name of the configuration option.
@@ -997,19 +1005,16 @@
 
         - **option**: the name of the configuration option.
 
         For more information see `FT.CONFIG GET <https://redis.io/commands/ft.config-get>`_.
         """  # noqa
         cmd = [CONFIG_CMD, "GET", option]
         res = {}
-        raw = await self.execute_command(*cmd)
-        if raw:
-            for kvs in raw:
-                res[kvs[0]] = kvs[1]
-        return res
+        res = await self.execute_command(*cmd)
+        return self._parse_results(CONFIG_CMD, res)
 
     async def load_document(self, id):
         """
         Load a single document by id
         """
         fields = await self.client.hgetall(id)
         f2 = {to_string(k): to_string(v) for k, v in fields.items()}
```

### Comparing `redis-5.0.0b4/redis/commands/search/field.py` & `redis-5.0.0rc1/redis/commands/search/field.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/search/indexDefinition.py` & `redis-5.0.0rc1/redis/commands/search/indexDefinition.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/search/query.py` & `redis-5.0.0rc1/redis/commands/search/query.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/search/querystring.py` & `redis-5.0.0rc1/redis/commands/search/querystring.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/search/reducers.py` & `redis-5.0.0rc1/redis/commands/search/reducers.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/search/result.py` & `redis-5.0.0rc1/redis/commands/search/result.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/search/suggestion.py` & `redis-5.0.0rc1/redis/commands/search/suggestion.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/sentinel.py` & `redis-5.0.0rc1/redis/commands/sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/timeseries/__init__.py` & `redis-5.0.0rc1/redis/commands/timeseries/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import redis
+from redis.client import bool_ok
 
 from ..helpers import parse_to_list
 from .commands import (
     ALTER_CMD,
     CREATE_CMD,
     CREATERULE_CMD,
     DEL_CMD,
@@ -29,34 +30,43 @@
     functionality.
     """
 
     def __init__(self, client=None, **kwargs):
         """Create a new RedisTimeSeries client."""
         # Set the module commands' callbacks
         self.MODULE_CALLBACKS = {
-            CREATE_CMD: redis.client.bool_ok,
-            ALTER_CMD: redis.client.bool_ok,
-            CREATERULE_CMD: redis.client.bool_ok,
+            CREATE_CMD: bool_ok,
+            ALTER_CMD: bool_ok,
+            CREATERULE_CMD: bool_ok,
+            DELETERULE_CMD: bool_ok,
+        }
+
+        RESP2_MODULE_CALLBACKS = {
             DEL_CMD: int,
-            DELETERULE_CMD: redis.client.bool_ok,
+            GET_CMD: parse_get,
+            QUERYINDEX_CMD: parse_to_list,
             RANGE_CMD: parse_range,
             REVRANGE_CMD: parse_range,
+            MGET_CMD: parse_m_get,
             MRANGE_CMD: parse_m_range,
             MREVRANGE_CMD: parse_m_range,
-            GET_CMD: parse_get,
-            MGET_CMD: parse_m_get,
             INFO_CMD: TSInfo,
-            QUERYINDEX_CMD: parse_to_list,
         }
+        RESP3_MODULE_CALLBACKS = {}
 
         self.client = client
         self.execute_command = client.execute_command
 
-        for key, value in self.MODULE_CALLBACKS.items():
-            self.client.set_response_callback(key, value)
+        if self.client.connection_pool.connection_kwargs.get("protocol") in ["3", 3]:
+            self.MODULE_CALLBACKS.update(RESP3_MODULE_CALLBACKS)
+        else:
+            self.MODULE_CALLBACKS.update(RESP2_MODULE_CALLBACKS)
+
+        for k, v in self.MODULE_CALLBACKS.items():
+            self.client.set_response_callback(k, v)
 
     def pipeline(self, transaction=True, shard_hint=None):
         """Creates a pipeline for the TimeSeries module, that can be used
         for executing only TimeSeries commands and core commands.
 
         Usage example:
```

### Comparing `redis-5.0.0b4/redis/commands/timeseries/commands.py` & `redis-5.0.0rc1/redis/commands/timeseries/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/commands/timeseries/info.py` & `redis-5.0.0rc1/redis/commands/timeseries/info.py`

 * *Files 15% similar despite different names*

```diff
@@ -76,7 +76,16 @@
             )  # backward compatible changes
         if "chunkSize" in response:
             self.chunk_size = response["chunkSize"]
         if "duplicatePolicy" in response:
             self.duplicate_policy = response["duplicatePolicy"]
             if type(self.duplicate_policy) == bytes:
                 self.duplicate_policy = self.duplicate_policy.decode()
+
+    def get(self, item):
+        try:
+            return self.__getitem__(item)
+        except AttributeError:
+            return None
+
+    def __getitem__(self, item):
+        return getattr(self, item)
```

### Comparing `redis-5.0.0b4/redis/commands/timeseries/utils.py` & `redis-5.0.0rc1/redis/commands/timeseries/utils.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/connection.py` & `redis-5.0.0rc1/redis/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     import hiredis
 
 SYM_STAR = b"*"
 SYM_DOLLAR = b"$"
 SYM_CRLF = b"\r\n"
 SYM_EMPTY = b""
 
+DEFAULT_RESP_VERSION = 2
+
 SENTINEL = object()
 
 DefaultParser: Type[Union[_RESP2Parser, _RESP3Parser, _HiredisParser]]
 if HIREDIS_AVAILABLE:
     DefaultParser = _HiredisParser
 else:
     DefaultParser = _RESP2Parser
@@ -185,15 +187,25 @@
         self.redis_connect_func = redis_connect_func
         self.encoder = Encoder(encoding, encoding_errors, decode_responses)
         self._sock = None
         self._socket_read_size = socket_read_size
         self.set_parser(parser_class)
         self._connect_callbacks = []
         self._buffer_cutoff = 6000
-        self.protocol = protocol
+        try:
+            p = int(protocol)
+        except TypeError:
+            p = DEFAULT_RESP_VERSION
+        except ValueError:
+            raise ConnectionError("protocol must be an integer")
+        finally:
+            if p < 2 or p > 3:
+                raise ConnectionError("protocol must be either 2 or 3")
+                # p = DEFAULT_RESP_VERSION
+            self.protocol = p
         self._command_packer = self._construct_command_packer(command_packer)
 
     def __repr__(self):
         repr_args = ",".join([f"{k}={v}" for k, v in self.repr_pieces()])
         return f"{self.__class__.__name__}<{repr_args}>"
 
     @abstractmethod
@@ -272,22 +284,42 @@
     @abstractmethod
     def _error_message(self, exception):
         pass
 
     def on_connect(self):
         "Initialize the connection, authenticate and select a database"
         self._parser.on_connect(self)
+        parser = self._parser
 
+        auth_args = None
         # if credential provider or username and/or password are set, authenticate
         if self.credential_provider or (self.username or self.password):
             cred_provider = (
                 self.credential_provider
                 or UsernamePasswordCredentialProvider(self.username, self.password)
             )
             auth_args = cred_provider.get_credentials()
+
+        # if resp version is specified and we have auth args,
+        # we need to send them via HELLO
+        if auth_args and self.protocol not in [2, "2"]:
+            if isinstance(self._parser, _RESP2Parser):
+                self.set_parser(_RESP3Parser)
+                # update cluster exception classes
+                self._parser.EXCEPTION_CLASSES = parser.EXCEPTION_CLASSES
+                self._parser.on_connect(self)
+            if len(auth_args) == 1:
+                auth_args = ["default", auth_args[0]]
+            self.send_command("HELLO", self.protocol, "AUTH", *auth_args)
+            response = self.read_response()
+            # if response.get(b"proto") != self.protocol and response.get(
+            #     "proto"
+            # ) != self.protocol:
+            #     raise ConnectionError("Invalid RESP version")
+        elif auth_args:
             # avoid checking health here -- PING will fail if we try
             # to check the health prior to the AUTH
             self.send_command("AUTH", *auth_args, check_health=False)
 
             try:
                 auth_response = self.read_response()
             except AuthenticationWrongNumberOfArgsError:
@@ -298,23 +330,26 @@
                 self.send_command("AUTH", auth_args[-1], check_health=False)
                 auth_response = self.read_response()
 
             if str_if_bytes(auth_response) != "OK":
                 raise AuthenticationError("Invalid Username or Password")
 
         # if resp version is specified, switch to it
-        if self.protocol != 2:
+        elif self.protocol not in [2, "2"]:
             if isinstance(self._parser, _RESP2Parser):
                 self.set_parser(_RESP3Parser)
+                # update cluster exception classes
+                self._parser.EXCEPTION_CLASSES = parser.EXCEPTION_CLASSES
                 self._parser.on_connect(self)
             self.send_command("HELLO", self.protocol)
             response = self.read_response()
-            if response.get(b"proto") != int(self.protocol) and response.get(
-                "proto"
-            ) != int(self.protocol):
+            if (
+                response.get(b"proto") != self.protocol
+                and response.get("proto") != self.protocol
+            ):
                 raise ConnectionError("Invalid RESP version")
 
         # if a client_name is given, set it
         if self.client_name:
             self.send_command("CLIENT", "SETNAME", self.client_name)
             if str_if_bytes(self.read_response()) != "OK":
                 raise ConnectionError("Error setting client name")
@@ -408,15 +443,15 @@
 
     def read_response(self, disable_decoding=False, push_request=False):
         """Read the response from a previously sent command"""
 
         host_error = self._host_error()
 
         try:
-            if self.protocol == "3" and not HIREDIS_AVAILABLE:
+            if self.protocol in ["3", 3] and not HIREDIS_AVAILABLE:
                 response = self._parser.read_response(
                     disable_decoding=disable_decoding, push_request=push_request
                 )
             else:
                 response = self._parser.read_response(disable_decoding=disable_decoding)
         except socket.timeout:
             self.disconnect()
```

### Comparing `redis-5.0.0b4/redis/crc.py` & `redis-5.0.0rc1/redis/crc.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/credentials.py` & `redis-5.0.0rc1/redis/credentials.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/exceptions.py` & `redis-5.0.0rc1/redis/exceptions.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/lock.py` & `redis-5.0.0rc1/redis/lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/ocsp.py` & `redis-5.0.0rc1/redis/ocsp.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from cryptography.hazmat.primitives.asymmetric.dsa import DSAPublicKey
 from cryptography.hazmat.primitives.asymmetric.ec import ECDSA, EllipticCurvePublicKey
 from cryptography.hazmat.primitives.asymmetric.padding import PKCS1v15
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey
 from cryptography.hazmat.primitives.hashes import SHA1, Hash
 from cryptography.hazmat.primitives.serialization import Encoding, PublicFormat
 from cryptography.x509 import ocsp
-
 from redis.exceptions import AuthorizationError, ConnectionError
 
 
 def _verify_response(issuer_cert, ocsp_response):
     pubkey = issuer_cert.public_key()
     try:
         if isinstance(pubkey, RSAPublicKey):
```

### Comparing `redis-5.0.0b4/redis/parsers/__init__.py` & `redis-5.0.0rc1/redis/parsers/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from .base import BaseParser
+from .base import BaseParser, _AsyncRESPBase
 from .commands import AsyncCommandsParser, CommandsParser
 from .encoders import Encoder
 from .hiredis import _AsyncHiredisParser, _HiredisParser
 from .resp2 import _AsyncRESP2Parser, _RESP2Parser
 from .resp3 import _AsyncRESP3Parser, _RESP3Parser
 
 __all__ = [
     "AsyncCommandsParser",
     "_AsyncHiredisParser",
+    "_AsyncRESPBase",
     "_AsyncRESP2Parser",
     "_AsyncRESP3Parser",
     "CommandsParser",
     "Encoder",
     "BaseParser",
     "_HiredisParser",
     "_RESP2Parser",
```

### Comparing `redis-5.0.0b4/redis/parsers/base.py` & `redis-5.0.0rc1/redis/parsers/base.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/parsers/commands.py` & `redis-5.0.0rc1/redis/parsers/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/parsers/encoders.py` & `redis-5.0.0rc1/redis/parsers/encoders.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/parsers/hiredis.py` & `redis-5.0.0rc1/redis/parsers/hiredis.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/parsers/resp2.py` & `redis-5.0.0rc1/redis/parsers/resp2.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/parsers/resp3.py` & `redis-5.0.0rc1/redis/parsers/resp3.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,17 +65,20 @@
             return int(response)
         # double value
         elif byte == b",":
             return float(response)
         # bool value
         elif byte == b"#":
             return response == b"t"
-        # bulk response and verbatim strings
-        elif byte in (b"$", b"="):
+        # bulk response
+        elif byte == b"$":
             response = self._buffer.read(int(response))
+        # verbatim string response
+        elif byte == b"=":
+            response = self._buffer.read(int(response))[4:]
         # array response
         elif byte == b"*":
             response = [
                 self._read_response(disable_decoding=disable_decoding)
                 for _ in range(int(response))
             ]
         # set response
@@ -191,17 +194,20 @@
             return int(response)
         # double value
         elif byte == b",":
             return float(response)
         # bool value
         elif byte == b"#":
             return response == b"t"
-        # bulk response and verbatim strings
-        elif byte in (b"$", b"="):
+        # bulk response
+        elif byte == b"$":
             response = await self._read(int(response))
+        # verbatim string response
+        elif byte == b"=":
+            response = (await self._read(int(response)))[4:]
         # array response
         elif byte == b"*":
             response = [
                 (await self._read_response(disable_decoding=disable_decoding))
                 for _ in range(int(response))
             ]
         # set response
```

### Comparing `redis-5.0.0b4/redis/parsers/socket.py` & `redis-5.0.0rc1/redis/parsers/socket.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/retry.py` & `redis-5.0.0rc1/redis/retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/sentinel.py` & `redis-5.0.0rc1/redis/sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/typing.py` & `redis-5.0.0rc1/redis/typing.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis/utils.py` & `redis-5.0.0rc1/redis/utils.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/redis.egg-info/PKG-INFO` & `redis-5.0.0rc1/redis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis
-Version: 5.0.0b4
+Version: 5.0.0rc1
 Summary: Python client for Redis database and key-value store
 Home-page: https://github.com/redis/redis-py
 Author: Redis Inc.
 Author-email: oss@redis.com
 License: MIT
 Project-URL: Documentation, https://redis.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/redis/redis-py/releases
```

### Comparing `redis-5.0.0b4/redis.egg-info/SOURCES.txt` & `redis-5.0.0rc1/redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/setup.py` & `redis-5.0.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 setup(
     name="redis",
     description="Python client for Redis database and key-value store",
     long_description=open("README.md").read().strip(),
     long_description_content_type="text/markdown",
     keywords=["Redis", "key-value store", "database"],
     license="MIT",
-    version="5.0.0b4",
+    version="5.0.0rc1",
     packages=find_packages(
         include=[
             "redis",
             "redis.asyncio",
             "redis.commands",
             "redis.commands.bf",
             "redis.commands.json",
```

### Comparing `redis-5.0.0b4/tests/asynctests` & `redis-5.0.0rc1/tests/asynctests`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/tests/conftest.py` & `redis-5.0.0rc1/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 import random
 import time
 from typing import Callable, TypeVar
 from unittest.mock import Mock
 from urllib.parse import urlparse
 
 import pytest
-from packaging.version import Version
-
 import redis
+from packaging.version import Version
 from redis.backoff import NoBackoff
 from redis.connection import parse_url
 from redis.exceptions import RedisClusterException
 from redis.retry import Retry
 
 REDIS_INFO = {}
 default_redis_url = "redis://localhost:6379/0"
-default_redismod_url = "redis://localhost:36379"
-default_redis_unstable_url = "redis://localhost:6378"
+default_protocol = "2"
+default_redismod_url = "redis://localhost:6379"
 
 # default ssl client ignores verification for the purpose of testing
 default_redis_ssl_url = "rediss://localhost:6666"
 default_cluster_nodes = 6
 
 _DecoratedTest = TypeVar("_DecoratedTest", bound="Callable")
 _TestDecorator = Callable[[_DecoratedTest], _DecoratedTest]
@@ -69,30 +68,28 @@
             setattr(namespace, self.dest, not option_string.startswith("--no-"))
 
     def format_usage(self):
         return " | ".join(self.option_strings)
 
 
 def pytest_addoption(parser):
+
     parser.addoption(
         "--redis-url",
         default=default_redis_url,
         action="store",
         help="Redis connection string, defaults to `%(default)s`",
     )
 
     parser.addoption(
-        "--redismod-url",
-        default=default_redismod_url,
+        "--protocol",
+        default=default_protocol,
         action="store",
-        help="Connection string to redis server"
-        " with loaded modules,"
-        " defaults to `%(default)s`",
+        help="Protocol version, defaults to `%(default)s`",
     )
-
     parser.addoption(
         "--redis-ssl-url",
         default=default_redis_ssl_url,
         action="store",
         help="Redis SSL connection string, defaults to `%(default)s`",
     )
 
@@ -102,21 +99,14 @@
         action="store",
         help="The number of cluster nodes that need to be "
         "available before the test can start,"
         " defaults to `%(default)s`",
     )
 
     parser.addoption(
-        "--redis-unstable-url",
-        default=default_redis_unstable_url,
-        action="store",
-        help="Redis unstable (latest version) connection string "
-        "defaults to %(default)s`",
-    )
-    parser.addoption(
         "--uvloop", action=BooleanOptionalAction, help="Run tests with uvloop"
     )
 
 
 def _get_info(redis_url):
     client = redis.Redis.from_url(redis_url)
     info = client.info()
@@ -148,18 +138,16 @@
     REDIS_INFO["version"] = version
     REDIS_INFO["arch_bits"] = arch_bits
     REDIS_INFO["cluster_enabled"] = cluster_enabled
     REDIS_INFO["enterprise"] = enterprise
     # store REDIS_INFO in config so that it is available from "condition strings"
     session.config.REDIS_INFO = REDIS_INFO
 
-    # module info, if the second redis is running
+    # module info
     try:
-        redismod_url = session.config.getoption("--redismod-url")
-        info = _get_info(redismod_url)
         REDIS_INFO["modules"] = info["modules"]
     except redis.exceptions.ConnectionError:
         pass
     except KeyError:
         pass
 
     if cluster_enabled:
@@ -285,14 +273,17 @@
     ConnectionPool.from_url, keyword arguments to this function override
     values specified in the URL.
     """
     if from_url is None:
         redis_url = request.config.getoption("--redis-url")
     else:
         redis_url = from_url
+    if "protocol" not in redis_url:
+        kwargs["protocol"] = request.config.getoption("--protocol")
+
     cluster_mode = REDIS_INFO["cluster_enabled"]
     if not cluster_mode:
         url_options = parse_url(redis_url)
         url_options.update(kwargs)
         pool = redis.ConnectionPool(**url_options)
         client = cls(connection_pool=pool)
     else:
@@ -328,28 +319,23 @@
             # handle cases where a test disconnected a client
             # just manually retry the flushdb
             client.flushdb(target_nodes="primaries")
     client.close()
     client.disconnect_connection_pools()
 
 
-# specifically set to the zero database, because creating
-# an index on db != 0 raises a ResponseError in redis
 @pytest.fixture()
-def modclient(request, **kwargs):
-    rmurl = request.config.getoption("--redismod-url")
-    with _get_client(
-        redis.Redis, request, from_url=rmurl, decode_responses=True, **kwargs
-    ) as client:
+def r(request):
+    with _get_client(redis.Redis, request) as client:
         yield client
 
 
 @pytest.fixture()
-def r(request):
-    with _get_client(redis.Redis, request) as client:
+def decoded_r(request):
+    with _get_client(redis.Redis, request, decode_responses=True) as client:
         yield client
 
 
 @pytest.fixture()
 def r_timeout(request):
     with _get_client(redis.Redis, request, socket_timeout=1) as client:
         yield client
@@ -440,23 +426,14 @@
 @pytest.fixture(scope="session")
 def master_host(request):
     url = request.config.getoption("--redis-url")
     parts = urlparse(url)
     yield parts.hostname, parts.port
 
 
-@pytest.fixture()
-def unstable_r(request):
-    url = request.config.getoption("--redis-unstable-url")
-    with _get_client(
-        redis.Redis, request, from_url=url, decode_responses=True
-    ) as client:
-        yield client
-
-
 def wait_for_command(client, monitor, command, key=None):
     # issue a command with a key name that's local to this process.
     # if we find a command with our key before the command we're waiting
     # for, something went wrong
     if key is None:
         # generate key
         redis_version = REDIS_INFO["version"]
@@ -471,12 +448,35 @@
         if command in monitor_response["command"]:
             return monitor_response
         if key in monitor_response["command"]:
             return None
 
 
 def is_resp2_connection(r):
-    if isinstance(r, redis.Redis):
+    if isinstance(r, redis.Redis) or isinstance(r, redis.asyncio.Redis):
         protocol = r.connection_pool.connection_kwargs.get("protocol")
-    elif isinstance(r, redis.RedisCluster):
+    elif isinstance(r, redis.cluster.AbstractRedisCluster):
         protocol = r.nodes_manager.connection_kwargs.get("protocol")
     return protocol in ["2", 2, None]
+
+
+def get_protocol_version(r):
+    if isinstance(r, redis.Redis) or isinstance(r, redis.asyncio.Redis):
+        return r.connection_pool.connection_kwargs.get("protocol")
+    elif isinstance(r, redis.cluster.AbstractRedisCluster):
+        return r.nodes_manager.connection_kwargs.get("protocol")
+
+
+def assert_resp_response(r, response, resp2_expected, resp3_expected):
+    protocol = get_protocol_version(r)
+    if protocol in [2, "2", None]:
+        assert response == resp2_expected
+    else:
+        assert response == resp3_expected
+
+
+def assert_resp_response_in(r, response, resp2_expected, resp3_expected):
+    protocol = get_protocol_version(r)
+    if protocol in [2, "2", None]:
+        assert response in resp2_expected
+    else:
+        assert response in resp3_expected
```

### Comparing `redis-5.0.0b4/tests/mocks.py` & `redis-5.0.0rc1/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/tests/synctests` & `redis-5.0.0rc1/tests/synctests`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/tests/test_asyncio/conftest.py` & `redis-5.0.0rc1/tests/test_asyncio/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import random
 from contextlib import asynccontextmanager as _asynccontextmanager
 from typing import Union
 from urllib.parse import urlparse
 
 import pytest
 import pytest_asyncio
-from packaging.version import Version
-
 import redis.asyncio as redis
+from packaging.version import Version
 from redis.asyncio.client import Monitor
 from redis.asyncio.connection import parse_url
 from redis.asyncio.retry import Retry
 from redis.backoff import NoBackoff
 from redis.parsers import _AsyncHiredisParser, _AsyncRESP2Parser
 from redis.utils import HIREDIS_AVAILABLE
 from tests.conftest import REDIS_INFO
@@ -67,16 +66,20 @@
 
     teardown_clients = []
 
     async def client_factory(
         url: str = request.config.getoption("--redis-url"),
         cls=redis.Redis,
         flushdb=True,
+        protocol=request.config.getoption("--protocol"),
         **kwargs,
     ):
+        if "protocol" not in url:
+            kwargs["protocol"] = request.config.getoption("--protocol")
+
         cluster_mode = REDIS_INFO["cluster_enabled"]
         if not cluster_mode:
             single = kwargs.pop("single_connection_client", False) or single_connection
             parser_class = kwargs.pop("parser_class", None) or parser_cls
             url_options = parse_url(url)
             url_options.update(kwargs)
             pool = redis.ConnectionPool(parser_class=parser_class, **url_options)
@@ -127,18 +130,16 @@
 @pytest_asyncio.fixture()
 async def r2(create_redis):
     """A second client for tests that need multiple"""
     return await create_redis()
 
 
 @pytest_asyncio.fixture()
-async def modclient(request, create_redis):
-    return await create_redis(
-        url=request.config.getoption("--redismod-url"), decode_responses=True
-    )
+async def decoded_r(create_redis):
+    return await create_redis(decode_responses=True)
 
 
 def _gen_cluster_mock_resp(r, response):
     connection = mock.AsyncMock()
     connection.retry = Retry(NoBackoff(), 0)
     connection.read_response.return_value = response
     r.connection = connection
@@ -232,37 +233,14 @@
         monitor_response = await monitor.next_command()
         if command in monitor_response["command"]:
             return monitor_response
         if key in monitor_response["command"]:
             return None
 
 
-def get_protocol_version(r):
-    if isinstance(r, redis.Redis):
-        return r.connection_pool.connection_kwargs.get("protocol")
-    elif isinstance(r, redis.RedisCluster):
-        return r.nodes_manager.connection_kwargs.get("protocol")
-
-
-def assert_resp_response(r, response, resp2_expected, resp3_expected):
-    protocol = get_protocol_version(r)
-    if protocol in [2, "2", None]:
-        assert response == resp2_expected
-    else:
-        assert response == resp3_expected
-
-
-def assert_resp_response_in(r, response, resp2_expected, resp3_expected):
-    protocol = get_protocol_version(r)
-    if protocol in [2, "2", None]:
-        assert response in resp2_expected
-    else:
-        assert response in resp3_expected
-
-
 # python 3.6 doesn't have the asynccontextmanager decorator.  Provide it here.
 class AsyncContextManager:
     def __init__(self, async_generator):
         self.gen = async_generator
 
     async def __aenter__(self):
         try:
```

### Comparing `redis-5.0.0b4/tests/test_asyncio/mocks.py` & `redis-5.0.0rc1/tests/test_asyncio/mocks.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/tests/test_asyncio/test_bloom.py` & `redis-5.0.0rc1/tests/test_bloom.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,248 +1,289 @@
 from math import inf
 
 import pytest
-
-import redis.asyncio as redis
+import redis.commands.bf
 from redis.exceptions import ModuleError, RedisError
 from redis.utils import HIREDIS_AVAILABLE
-from tests.conftest import skip_ifmodversion_lt
+
+from .conftest import assert_resp_response, is_resp2_connection, skip_ifmodversion_lt
 
 
 def intlist(obj):
     return [int(v) for v in obj]
 
 
-# @pytest.fixture
-# async def client(modclient):
-#     assert isinstance(modawait modclient.bf(), redis.commands.bf.BFBloom)
-#     assert isinstance(modawait modclient.cf(), redis.commands.bf.CFBloom)
-#     assert isinstance(modawait modclient.cms(), redis.commands.bf.CMSBloom)
-#     assert isinstance(modawait modclient.tdigest(), redis.commands.bf.TDigestBloom)
-#     assert isinstance(modawait modclient.topk(), redis.commands.bf.TOPKBloom)
+@pytest.fixture
+def client(decoded_r):
+    assert isinstance(decoded_r.bf(), redis.commands.bf.BFBloom)
+    assert isinstance(decoded_r.cf(), redis.commands.bf.CFBloom)
+    assert isinstance(decoded_r.cms(), redis.commands.bf.CMSBloom)
+    assert isinstance(decoded_r.tdigest(), redis.commands.bf.TDigestBloom)
+    assert isinstance(decoded_r.topk(), redis.commands.bf.TOPKBloom)
 
-#     modawait modclient.flushdb()
-#     return modclient
+    decoded_r.flushdb()
+    return decoded_r
 
 
 @pytest.mark.redismod
-async def test_create(modclient: redis.Redis):
+def test_create(client):
     """Test CREATE/RESERVE calls"""
-    assert await modclient.bf().create("bloom", 0.01, 1000)
-    assert await modclient.bf().create("bloom_e", 0.01, 1000, expansion=1)
-    assert await modclient.bf().create("bloom_ns", 0.01, 1000, noScale=True)
-    assert await modclient.cf().create("cuckoo", 1000)
-    assert await modclient.cf().create("cuckoo_e", 1000, expansion=1)
-    assert await modclient.cf().create("cuckoo_bs", 1000, bucket_size=4)
-    assert await modclient.cf().create("cuckoo_mi", 1000, max_iterations=10)
-    assert await modclient.cms().initbydim("cmsDim", 100, 5)
-    assert await modclient.cms().initbyprob("cmsProb", 0.01, 0.01)
-    assert await modclient.topk().reserve("topk", 5, 100, 5, 0.9)
+    assert client.bf().create("bloom", 0.01, 1000)
+    assert client.bf().create("bloom_e", 0.01, 1000, expansion=1)
+    assert client.bf().create("bloom_ns", 0.01, 1000, noScale=True)
+    assert client.cf().create("cuckoo", 1000)
+    assert client.cf().create("cuckoo_e", 1000, expansion=1)
+    assert client.cf().create("cuckoo_bs", 1000, bucket_size=4)
+    assert client.cf().create("cuckoo_mi", 1000, max_iterations=10)
+    assert client.cms().initbydim("cmsDim", 100, 5)
+    assert client.cms().initbyprob("cmsProb", 0.01, 0.01)
+    assert client.topk().reserve("topk", 5, 100, 5, 0.9)
+
+
+@pytest.mark.redismod
+def test_bf_reserve(client):
+    """Testing BF.RESERVE"""
+    assert client.bf().reserve("bloom", 0.01, 1000)
+    assert client.bf().reserve("bloom_e", 0.01, 1000, expansion=1)
+    assert client.bf().reserve("bloom_ns", 0.01, 1000, noScale=True)
+    assert client.cf().reserve("cuckoo", 1000)
+    assert client.cf().reserve("cuckoo_e", 1000, expansion=1)
+    assert client.cf().reserve("cuckoo_bs", 1000, bucket_size=4)
+    assert client.cf().reserve("cuckoo_mi", 1000, max_iterations=10)
+    assert client.cms().initbydim("cmsDim", 100, 5)
+    assert client.cms().initbyprob("cmsProb", 0.01, 0.01)
+    assert client.topk().reserve("topk", 5, 100, 5, 0.9)
 
 
 @pytest.mark.redismod
 @pytest.mark.experimental
-async def test_tdigest_create(modclient: redis.Redis):
-    assert await modclient.tdigest().create("tDigest", 100)
+def test_tdigest_create(client):
+    assert client.tdigest().create("tDigest", 100)
 
 
-# region Test Bloom Filter
 @pytest.mark.redismod
-async def test_bf_add(modclient: redis.Redis):
-    assert await modclient.bf().create("bloom", 0.01, 1000)
-    assert 1 == await modclient.bf().add("bloom", "foo")
-    assert 0 == await modclient.bf().add("bloom", "foo")
-    assert [0] == intlist(await modclient.bf().madd("bloom", "foo"))
-    assert [0, 1] == await modclient.bf().madd("bloom", "foo", "bar")
-    assert [0, 0, 1] == await modclient.bf().madd("bloom", "foo", "bar", "baz")
-    assert 1 == await modclient.bf().exists("bloom", "foo")
-    assert 0 == await modclient.bf().exists("bloom", "noexist")
-    assert [1, 0] == intlist(await modclient.bf().mexists("bloom", "foo", "noexist"))
+def test_bf_add(client):
+    assert client.bf().create("bloom", 0.01, 1000)
+    assert 1 == client.bf().add("bloom", "foo")
+    assert 0 == client.bf().add("bloom", "foo")
+    assert [0] == intlist(client.bf().madd("bloom", "foo"))
+    assert [0, 1] == client.bf().madd("bloom", "foo", "bar")
+    assert [0, 0, 1] == client.bf().madd("bloom", "foo", "bar", "baz")
+    assert 1 == client.bf().exists("bloom", "foo")
+    assert 0 == client.bf().exists("bloom", "noexist")
+    assert [1, 0] == intlist(client.bf().mexists("bloom", "foo", "noexist"))
 
 
 @pytest.mark.redismod
-async def test_bf_insert(modclient: redis.Redis):
-    assert await modclient.bf().create("bloom", 0.01, 1000)
-    assert [1] == intlist(await modclient.bf().insert("bloom", ["foo"]))
-    assert [0, 1] == intlist(await modclient.bf().insert("bloom", ["foo", "bar"]))
-    assert [1] == intlist(await modclient.bf().insert("captest", ["foo"], capacity=10))
-    assert [1] == intlist(await modclient.bf().insert("errtest", ["foo"], error=0.01))
-    assert 1 == await modclient.bf().exists("bloom", "foo")
-    assert 0 == await modclient.bf().exists("bloom", "noexist")
-    assert [1, 0] == intlist(await modclient.bf().mexists("bloom", "foo", "noexist"))
-    info = await modclient.bf().info("bloom")
-    assert 2 == info.insertedNum
-    assert 1000 == info.capacity
-    assert 1 == info.filterNum
+def test_bf_insert(client):
+    assert client.bf().create("bloom", 0.01, 1000)
+    assert [1] == intlist(client.bf().insert("bloom", ["foo"]))
+    assert [0, 1] == intlist(client.bf().insert("bloom", ["foo", "bar"]))
+    assert [1] == intlist(client.bf().insert("captest", ["foo"], capacity=10))
+    assert [1] == intlist(client.bf().insert("errtest", ["foo"], error=0.01))
+    assert 1 == client.bf().exists("bloom", "foo")
+    assert 0 == client.bf().exists("bloom", "noexist")
+    assert [1, 0] == intlist(client.bf().mexists("bloom", "foo", "noexist"))
+    info = client.bf().info("bloom")
+    assert_resp_response(
+        client,
+        2,
+        info.get("insertedNum"),
+        info.get("Number of items inserted"),
+    )
+    assert_resp_response(
+        client,
+        1000,
+        info.get("capacity"),
+        info.get("Capacity"),
+    )
+    assert_resp_response(
+        client,
+        1,
+        info.get("filterNum"),
+        info.get("Number of filters"),
+    )
 
 
 @pytest.mark.redismod
-async def test_bf_scandump_and_loadchunk(modclient: redis.Redis):
+def test_bf_scandump_and_loadchunk(client):
     # Store a filter
-    await modclient.bf().create("myBloom", "0.0001", "1000")
+    client.bf().create("myBloom", "0.0001", "1000")
 
     # test is probabilistic and might fail. It is OK to change variables if
     # certain to not break anything
-    async def do_verify():
+    def do_verify():
         res = 0
         for x in range(1000):
-            await modclient.bf().add("myBloom", x)
-            rv = await modclient.bf().exists("myBloom", x)
+            client.bf().add("myBloom", x)
+            rv = client.bf().exists("myBloom", x)
             assert rv
-            rv = await modclient.bf().exists("myBloom", f"nonexist_{x}")
+            rv = client.bf().exists("myBloom", f"nonexist_{x}")
             res += rv == x
         assert res < 5
 
-    await do_verify()
+    do_verify()
     cmds = []
     if HIREDIS_AVAILABLE:
         with pytest.raises(ModuleError):
-            cur = await modclient.bf().scandump("myBloom", 0)
+            cur = client.bf().scandump("myBloom", 0)
         return
 
-    cur = await modclient.bf().scandump("myBloom", 0)
+    cur = client.bf().scandump("myBloom", 0)
     first = cur[0]
     cmds.append(cur)
 
     while True:
-        cur = await modclient.bf().scandump("myBloom", first)
+        cur = client.bf().scandump("myBloom", first)
         first = cur[0]
         if first == 0:
             break
         else:
             cmds.append(cur)
-    prev_info = await modclient.bf().execute_command("bf.debug", "myBloom")
+    prev_info = client.bf().execute_command("bf.debug", "myBloom")
 
     # Remove the filter
-    await modclient.bf().client.delete("myBloom")
+    client.bf().client.delete("myBloom")
 
     # Now, load all the commands:
     for cmd in cmds:
-        await modclient.bf().loadchunk("myBloom", *cmd)
+        client.bf().loadchunk("myBloom", *cmd)
 
-    cur_info = await modclient.bf().execute_command("bf.debug", "myBloom")
+    cur_info = client.bf().execute_command("bf.debug", "myBloom")
     assert prev_info == cur_info
-    await do_verify()
+    do_verify()
 
-    await modclient.bf().client.delete("myBloom")
-    await modclient.bf().create("myBloom", "0.0001", "10000000")
+    client.bf().client.delete("myBloom")
+    client.bf().create("myBloom", "0.0001", "10000000")
 
 
 @pytest.mark.redismod
-async def test_bf_info(modclient: redis.Redis):
+def test_bf_info(client):
     expansion = 4
     # Store a filter
-    await modclient.bf().create("nonscaling", "0.0001", "1000", noScale=True)
-    info = await modclient.bf().info("nonscaling")
-    assert info.expansionRate is None
-
-    await modclient.bf().create("expanding", "0.0001", "1000", expansion=expansion)
-    info = await modclient.bf().info("expanding")
-    assert info.expansionRate == 4
+    client.bf().create("nonscaling", "0.0001", "1000", noScale=True)
+    info = client.bf().info("nonscaling")
+    assert_resp_response(
+        client,
+        None,
+        info.get("expansionRate"),
+        info.get("Expansion rate"),
+    )
+
+    client.bf().create("expanding", "0.0001", "1000", expansion=expansion)
+    info = client.bf().info("expanding")
+    assert_resp_response(
+        client,
+        4,
+        info.get("expansionRate"),
+        info.get("Expansion rate"),
+    )
 
     try:
         # noScale mean no expansion
-        await modclient.bf().create(
+        client.bf().create(
             "myBloom", "0.0001", "1000", expansion=expansion, noScale=True
         )
         assert False
     except RedisError:
         assert True
 
 
 @pytest.mark.redismod
-async def test_bf_card(modclient: redis.Redis):
+def test_bf_card(client):
     # return 0 if the key does not exist
-    assert await modclient.bf().card("not_exist") == 0
+    assert client.bf().card("not_exist") == 0
 
     # Store a filter
-    assert await modclient.bf().add("bf1", "item_foo") == 1
-    assert await modclient.bf().card("bf1") == 1
+    assert client.bf().add("bf1", "item_foo") == 1
+    assert client.bf().card("bf1") == 1
 
     # Error when key is of a type other than Bloom filter.
     with pytest.raises(redis.ResponseError):
-        await modclient.set("setKey", "value")
-        await modclient.bf().card("setKey")
+        client.set("setKey", "value")
+        client.bf().card("setKey")
 
 
-# region Test Cuckoo Filter
 @pytest.mark.redismod
-async def test_cf_add_and_insert(modclient: redis.Redis):
-    assert await modclient.cf().create("cuckoo", 1000)
-    assert await modclient.cf().add("cuckoo", "filter")
-    assert not await modclient.cf().addnx("cuckoo", "filter")
-    assert 1 == await modclient.cf().addnx("cuckoo", "newItem")
-    assert [1] == await modclient.cf().insert("captest", ["foo"])
-    assert [1] == await modclient.cf().insert("captest", ["foo"], capacity=1000)
-    assert [1] == await modclient.cf().insertnx("captest", ["bar"])
-    assert [1] == await modclient.cf().insertnx("captest", ["food"], nocreate="1")
-    assert [0, 0, 1] == await modclient.cf().insertnx("captest", ["foo", "bar", "baz"])
-    assert [0] == await modclient.cf().insertnx("captest", ["bar"], capacity=1000)
-    assert [1] == await modclient.cf().insert("empty1", ["foo"], capacity=1000)
-    assert [1] == await modclient.cf().insertnx("empty2", ["bar"], capacity=1000)
-    info = await modclient.cf().info("captest")
-    assert 5 == info.insertedNum
-    assert 0 == info.deletedNum
-    assert 1 == info.filterNum
+def test_cf_add_and_insert(client):
+    assert client.cf().create("cuckoo", 1000)
+    assert client.cf().add("cuckoo", "filter")
+    assert not client.cf().addnx("cuckoo", "filter")
+    assert 1 == client.cf().addnx("cuckoo", "newItem")
+    assert [1] == client.cf().insert("captest", ["foo"])
+    assert [1] == client.cf().insert("captest", ["foo"], capacity=1000)
+    assert [1] == client.cf().insertnx("captest", ["bar"])
+    assert [1] == client.cf().insertnx("captest", ["food"], nocreate="1")
+    assert [0, 0, 1] == client.cf().insertnx("captest", ["foo", "bar", "baz"])
+    assert [0] == client.cf().insertnx("captest", ["bar"], capacity=1000)
+    assert [1] == client.cf().insert("empty1", ["foo"], capacity=1000)
+    assert [1] == client.cf().insertnx("empty2", ["bar"], capacity=1000)
+    info = client.cf().info("captest")
+    assert_resp_response(
+        client, 5, info.get("insertedNum"), info.get("Number of items inserted")
+    )
+    assert_resp_response(
+        client, 0, info.get("deletedNum"), info.get("Number of items deleted")
+    )
+    assert_resp_response(
+        client, 1, info.get("filterNum"), info.get("Number of filters")
+    )
 
 
 @pytest.mark.redismod
-async def test_cf_exists_and_del(modclient: redis.Redis):
-    assert await modclient.cf().create("cuckoo", 1000)
-    assert await modclient.cf().add("cuckoo", "filter")
-    assert await modclient.cf().exists("cuckoo", "filter")
-    assert not await modclient.cf().exists("cuckoo", "notexist")
-    assert 1 == await modclient.cf().count("cuckoo", "filter")
-    assert 0 == await modclient.cf().count("cuckoo", "notexist")
-    assert await modclient.cf().delete("cuckoo", "filter")
-    assert 0 == await modclient.cf().count("cuckoo", "filter")
-
-
-# region Test Count-Min Sketch
-@pytest.mark.redismod
-async def test_cms(modclient: redis.Redis):
-    assert await modclient.cms().initbydim("dim", 1000, 5)
-    assert await modclient.cms().initbyprob("prob", 0.01, 0.01)
-    assert await modclient.cms().incrby("dim", ["foo"], [5])
-    assert [0] == await modclient.cms().query("dim", "notexist")
-    assert [5] == await modclient.cms().query("dim", "foo")
-    assert [10, 15] == await modclient.cms().incrby("dim", ["foo", "bar"], [5, 15])
-    assert [10, 15] == await modclient.cms().query("dim", "foo", "bar")
-    info = await modclient.cms().info("dim")
-    assert 1000 == info.width
-    assert 5 == info.depth
-    assert 25 == info.count
+def test_cf_exists_and_del(client):
+    assert client.cf().create("cuckoo", 1000)
+    assert client.cf().add("cuckoo", "filter")
+    assert client.cf().exists("cuckoo", "filter")
+    assert not client.cf().exists("cuckoo", "notexist")
+    assert [1, 0] == client.cf().mexists("cuckoo", "filter", "notexist")
+    assert 1 == client.cf().count("cuckoo", "filter")
+    assert 0 == client.cf().count("cuckoo", "notexist")
+    assert client.cf().delete("cuckoo", "filter")
+    assert 0 == client.cf().count("cuckoo", "filter")
 
 
 @pytest.mark.redismod
-@pytest.mark.onlynoncluster
-async def test_cms_merge(modclient: redis.Redis):
-    assert await modclient.cms().initbydim("A", 1000, 5)
-    assert await modclient.cms().initbydim("B", 1000, 5)
-    assert await modclient.cms().initbydim("C", 1000, 5)
-    assert await modclient.cms().incrby("A", ["foo", "bar", "baz"], [5, 3, 9])
-    assert await modclient.cms().incrby("B", ["foo", "bar", "baz"], [2, 3, 1])
-    assert [5, 3, 9] == await modclient.cms().query("A", "foo", "bar", "baz")
-    assert [2, 3, 1] == await modclient.cms().query("B", "foo", "bar", "baz")
-    assert await modclient.cms().merge("C", 2, ["A", "B"])
-    assert [7, 6, 10] == await modclient.cms().query("C", "foo", "bar", "baz")
-    assert await modclient.cms().merge("C", 2, ["A", "B"], ["1", "2"])
-    assert [9, 9, 11] == await modclient.cms().query("C", "foo", "bar", "baz")
-    assert await modclient.cms().merge("C", 2, ["A", "B"], ["2", "3"])
-    assert [16, 15, 21] == await modclient.cms().query("C", "foo", "bar", "baz")
+def test_cms(client):
+    assert client.cms().initbydim("dim", 1000, 5)
+    assert client.cms().initbyprob("prob", 0.01, 0.01)
+    assert client.cms().incrby("dim", ["foo"], [5])
+    assert [0] == client.cms().query("dim", "notexist")
+    assert [5] == client.cms().query("dim", "foo")
+    assert [10, 15] == client.cms().incrby("dim", ["foo", "bar"], [5, 15])
+    assert [10, 15] == client.cms().query("dim", "foo", "bar")
+    info = client.cms().info("dim")
+    assert info["width"]
+    assert 1000 == info["width"]
+    assert 5 == info["depth"]
+    assert 25 == info["count"]
 
 
-# endregion
+@pytest.mark.redismod
+@pytest.mark.onlynoncluster
+def test_cms_merge(client):
+    assert client.cms().initbydim("A", 1000, 5)
+    assert client.cms().initbydim("B", 1000, 5)
+    assert client.cms().initbydim("C", 1000, 5)
+    assert client.cms().incrby("A", ["foo", "bar", "baz"], [5, 3, 9])
+    assert client.cms().incrby("B", ["foo", "bar", "baz"], [2, 3, 1])
+    assert [5, 3, 9] == client.cms().query("A", "foo", "bar", "baz")
+    assert [2, 3, 1] == client.cms().query("B", "foo", "bar", "baz")
+    assert client.cms().merge("C", 2, ["A", "B"])
+    assert [7, 6, 10] == client.cms().query("C", "foo", "bar", "baz")
+    assert client.cms().merge("C", 2, ["A", "B"], ["1", "2"])
+    assert [9, 9, 11] == client.cms().query("C", "foo", "bar", "baz")
+    assert client.cms().merge("C", 2, ["A", "B"], ["2", "3"])
+    assert [16, 15, 21] == client.cms().query("C", "foo", "bar", "baz")
 
 
-# region Test Top-K
 @pytest.mark.redismod
-async def test_topk(modclient: redis.Redis):
+def test_topk(client):
     # test list with empty buckets
-    assert await modclient.topk().reserve("topk", 3, 50, 4, 0.9)
+    assert client.topk().reserve("topk", 3, 50, 4, 0.9)
     assert [
         None,
         None,
         None,
         "A",
         "C",
         "D",
@@ -253,15 +294,15 @@
         "B",
         "C",
         None,
         None,
         None,
         "D",
         None,
-    ] == await modclient.topk().add(
+    ] == client.topk().add(
         "topk",
         "A",
         "B",
         "C",
         "D",
         "E",
         "A",
@@ -273,25 +314,25 @@
         "B",
         "D",
         "A",
         "E",
         "E",
         1,
     )
-    assert [1, 1, 0, 0, 1, 0, 0] == await modclient.topk().query(
+    assert [1, 1, 0, 0, 1, 0, 0] == client.topk().query(
         "topk", "A", "B", "C", "D", "E", "F", "G"
     )
     with pytest.deprecated_call():
-        assert [4, 3, 2, 3, 3, 0, 1] == await modclient.topk().count(
+        assert [4, 3, 2, 3, 3, 0, 1] == client.topk().count(
             "topk", "A", "B", "C", "D", "E", "F", "G"
         )
 
     # test full list
-    assert await modclient.topk().reserve("topklist", 3, 50, 3, 0.9)
-    assert await modclient.topk().add(
+    assert client.topk().reserve("topklist", 3, 50, 3, 0.9)
+    assert client.topk().add(
         "topklist",
         "A",
         "B",
         "C",
         "D",
         "E",
         "A",
@@ -302,196 +343,191 @@
         "D",
         "B",
         "D",
         "A",
         "E",
         "E",
     )
-    assert ["A", "B", "E"] == await modclient.topk().list("topklist")
-    res = await modclient.topk().list("topklist", withcount=True)
-    assert ["A", 4, "B", 3, "E", 3] == res
-    info = await modclient.topk().info("topklist")
-    assert 3 == info.k
-    assert 50 == info.width
-    assert 3 == info.depth
-    assert 0.9 == round(float(info.decay), 1)
+    assert ["A", "B", "E"] == client.topk().list("topklist")
+    assert ["A", 4, "B", 3, "E", 3] == client.topk().list("topklist", withcount=True)
+    info = client.topk().info("topklist")
+    assert 3 == info["k"]
+    assert 50 == info["width"]
+    assert 3 == info["depth"]
+    assert 0.9 == round(float(info["decay"]), 1)
 
 
 @pytest.mark.redismod
-async def test_topk_incrby(modclient: redis.Redis):
-    await modclient.flushdb()
-    assert await modclient.topk().reserve("topk", 3, 10, 3, 1)
-    assert [None, None, None] == await modclient.topk().incrby(
+def test_topk_incrby(client):
+    client.flushdb()
+    assert client.topk().reserve("topk", 3, 10, 3, 1)
+    assert [None, None, None] == client.topk().incrby(
         "topk", ["bar", "baz", "42"], [3, 6, 2]
     )
-    res = await modclient.topk().incrby("topk", ["42", "xyzzy"], [8, 4])
-    assert [None, "bar"] == res
+    assert [None, "bar"] == client.topk().incrby("topk", ["42", "xyzzy"], [8, 4])
     with pytest.deprecated_call():
-        assert [3, 6, 10, 4, 0] == await modclient.topk().count(
+        assert [3, 6, 10, 4, 0] == client.topk().count(
             "topk", "bar", "baz", "42", "xyzzy", 4
         )
 
 
-# region Test T-Digest
 @pytest.mark.redismod
 @pytest.mark.experimental
-async def test_tdigest_reset(modclient: redis.Redis):
-    assert await modclient.tdigest().create("tDigest", 10)
+def test_tdigest_reset(client):
+    assert client.tdigest().create("tDigest", 10)
     # reset on empty histogram
-    assert await modclient.tdigest().reset("tDigest")
+    assert client.tdigest().reset("tDigest")
     # insert data-points into sketch
-    assert await modclient.tdigest().add("tDigest", list(range(10)))
+    assert client.tdigest().add("tDigest", list(range(10)))
 
-    assert await modclient.tdigest().reset("tDigest")
-    # assert we have 0 unmerged nodes
-    assert 0 == (await modclient.tdigest().info("tDigest")).unmerged_nodes
+    assert client.tdigest().reset("tDigest")
+    # assert we have 0 unmerged
+    info = client.tdigest().info("tDigest")
+    assert_resp_response(
+        client, 0, info.get("unmerged_nodes"), info.get("Unmerged nodes")
+    )
 
 
 @pytest.mark.redismod
 @pytest.mark.experimental
-async def test_tdigest_merge(modclient: redis.Redis):
-    assert await modclient.tdigest().create("to-tDigest", 10)
-    assert await modclient.tdigest().create("from-tDigest", 10)
+def test_tdigest_merge(client):
+    assert client.tdigest().create("to-tDigest", 10)
+    assert client.tdigest().create("from-tDigest", 10)
     # insert data-points into sketch
-    assert await modclient.tdigest().add("from-tDigest", [1.0] * 10)
-    assert await modclient.tdigest().add("to-tDigest", [2.0] * 10)
+    assert client.tdigest().add("from-tDigest", [1.0] * 10)
+    assert client.tdigest().add("to-tDigest", [2.0] * 10)
     # merge from-tdigest into to-tdigest
-    assert await modclient.tdigest().merge("to-tDigest", 1, "from-tDigest")
+    assert client.tdigest().merge("to-tDigest", 1, "from-tDigest")
     # we should now have 110 weight on to-histogram
-    info = await modclient.tdigest().info("to-tDigest")
-    total_weight_to = float(info.merged_weight) + float(info.unmerged_weight)
-    assert 20.0 == total_weight_to
+    info = client.tdigest().info("to-tDigest")
+    if is_resp2_connection(client):
+        assert 20 == float(info["merged_weight"]) + float(info["unmerged_weight"])
+    else:
+        assert 20 == float(info["Merged weight"]) + float(info["Unmerged weight"])
     # test override
-    assert await modclient.tdigest().create("from-override", 10)
-    assert await modclient.tdigest().create("from-override-2", 10)
-    assert await modclient.tdigest().add("from-override", [3.0] * 10)
-    assert await modclient.tdigest().add("from-override-2", [4.0] * 10)
-    assert await modclient.tdigest().merge(
+    assert client.tdigest().create("from-override", 10)
+    assert client.tdigest().create("from-override-2", 10)
+    assert client.tdigest().add("from-override", [3.0] * 10)
+    assert client.tdigest().add("from-override-2", [4.0] * 10)
+    assert client.tdigest().merge(
         "to-tDigest", 2, "from-override", "from-override-2", override=True
     )
-    assert 3.0 == await modclient.tdigest().min("to-tDigest")
-    assert 4.0 == await modclient.tdigest().max("to-tDigest")
+    assert 3.0 == client.tdigest().min("to-tDigest")
+    assert 4.0 == client.tdigest().max("to-tDigest")
 
 
 @pytest.mark.redismod
 @pytest.mark.experimental
-async def test_tdigest_min_and_max(modclient: redis.Redis):
-    assert await modclient.tdigest().create("tDigest", 100)
+def test_tdigest_min_and_max(client):
+    assert client.tdigest().create("tDigest", 100)
     # insert data-points into sketch
-    assert await modclient.tdigest().add("tDigest", [1, 2, 3])
+    assert client.tdigest().add("tDigest", [1, 2, 3])
     # min/max
-    assert 3 == await modclient.tdigest().max("tDigest")
-    assert 1 == await modclient.tdigest().min("tDigest")
+    assert 3 == client.tdigest().max("tDigest")
+    assert 1 == client.tdigest().min("tDigest")
 
 
 @pytest.mark.redismod
 @pytest.mark.experimental
 @skip_ifmodversion_lt("2.4.0", "bf")
-async def test_tdigest_quantile(modclient: redis.Redis):
-    assert await modclient.tdigest().create("tDigest", 500)
+def test_tdigest_quantile(client):
+    assert client.tdigest().create("tDigest", 500)
     # insert data-points into sketch
-    assert await modclient.tdigest().add(
-        "tDigest", list([x * 0.01 for x in range(1, 10000)])
-    )
+    assert client.tdigest().add("tDigest", list([x * 0.01 for x in range(1, 10000)]))
     # assert min min/max have same result as quantile 0 and 1
-    assert (
-        await modclient.tdigest().max("tDigest")
-        == (await modclient.tdigest().quantile("tDigest", 1))[0]
-    )
-    assert (
-        await modclient.tdigest().min("tDigest")
-        == (await modclient.tdigest().quantile("tDigest", 0.0))[0]
-    )
+    res = client.tdigest().quantile("tDigest", 1.0)
+    assert client.tdigest().max("tDigest") == res[0]
+    res = client.tdigest().quantile("tDigest", 0.0)
+    assert client.tdigest().min("tDigest") == res[0]
 
-    assert 1.0 == round((await modclient.tdigest().quantile("tDigest", 0.01))[0], 2)
-    assert 99.0 == round((await modclient.tdigest().quantile("tDigest", 0.99))[0], 2)
+    assert 1.0 == round(client.tdigest().quantile("tDigest", 0.01)[0], 2)
+    assert 99.0 == round(client.tdigest().quantile("tDigest", 0.99)[0], 2)
 
     # test multiple quantiles
-    assert await modclient.tdigest().create("t-digest", 100)
-    assert await modclient.tdigest().add("t-digest", [1, 2, 3, 4, 5])
-    res = await modclient.tdigest().quantile("t-digest", 0.5, 0.8)
-    assert [3.0, 5.0] == res
+    assert client.tdigest().create("t-digest", 100)
+    assert client.tdigest().add("t-digest", [1, 2, 3, 4, 5])
+    assert [3.0, 5.0] == client.tdigest().quantile("t-digest", 0.5, 0.8)
 
 
 @pytest.mark.redismod
 @pytest.mark.experimental
-async def test_tdigest_cdf(modclient: redis.Redis):
-    assert await modclient.tdigest().create("tDigest", 100)
+def test_tdigest_cdf(client):
+    assert client.tdigest().create("tDigest", 100)
     # insert data-points into sketch
-    assert await modclient.tdigest().add("tDigest", list(range(1, 10)))
-    assert 0.1 == round((await modclient.tdigest().cdf("tDigest", 1.0))[0], 1)
-    assert 0.9 == round((await modclient.tdigest().cdf("tDigest", 9.0))[0], 1)
-    res = await modclient.tdigest().cdf("tDigest", 1.0, 9.0)
+    assert client.tdigest().add("tDigest", list(range(1, 10)))
+    assert 0.1 == round(client.tdigest().cdf("tDigest", 1.0)[0], 1)
+    assert 0.9 == round(client.tdigest().cdf("tDigest", 9.0)[0], 1)
+    res = client.tdigest().cdf("tDigest", 1.0, 9.0)
     assert [0.1, 0.9] == [round(x, 1) for x in res]
 
 
 @pytest.mark.redismod
 @pytest.mark.experimental
 @skip_ifmodversion_lt("2.4.0", "bf")
-async def test_tdigest_trimmed_mean(modclient: redis.Redis):
-    assert await modclient.tdigest().create("tDigest", 100)
+def test_tdigest_trimmed_mean(client):
+    assert client.tdigest().create("tDigest", 100)
     # insert data-points into sketch
-    assert await modclient.tdigest().add("tDigest", list(range(1, 10)))
-    assert 5 == await modclient.tdigest().trimmed_mean("tDigest", 0.1, 0.9)
-    assert 4.5 == await modclient.tdigest().trimmed_mean("tDigest", 0.4, 0.5)
+    assert client.tdigest().add("tDigest", list(range(1, 10)))
+    assert 5 == client.tdigest().trimmed_mean("tDigest", 0.1, 0.9)
+    assert 4.5 == client.tdigest().trimmed_mean("tDigest", 0.4, 0.5)
 
 
 @pytest.mark.redismod
 @pytest.mark.experimental
-async def test_tdigest_rank(modclient: redis.Redis):
-    assert await modclient.tdigest().create("t-digest", 500)
-    assert await modclient.tdigest().add("t-digest", list(range(0, 20)))
-    assert -1 == (await modclient.tdigest().rank("t-digest", -1))[0]
-    assert 0 == (await modclient.tdigest().rank("t-digest", 0))[0]
-    assert 10 == (await modclient.tdigest().rank("t-digest", 10))[0]
-    assert [-1, 20, 9] == await modclient.tdigest().rank("t-digest", -20, 20, 9)
+def test_tdigest_rank(client):
+    assert client.tdigest().create("t-digest", 500)
+    assert client.tdigest().add("t-digest", list(range(0, 20)))
+    assert -1 == client.tdigest().rank("t-digest", -1)[0]
+    assert 0 == client.tdigest().rank("t-digest", 0)[0]
+    assert 10 == client.tdigest().rank("t-digest", 10)[0]
+    assert [-1, 20, 9] == client.tdigest().rank("t-digest", -20, 20, 9)
 
 
 @pytest.mark.redismod
 @pytest.mark.experimental
-async def test_tdigest_revrank(modclient: redis.Redis):
-    assert await modclient.tdigest().create("t-digest", 500)
-    assert await modclient.tdigest().add("t-digest", list(range(0, 20)))
-    assert -1 == (await modclient.tdigest().revrank("t-digest", 20))[0]
-    assert 19 == (await modclient.tdigest().revrank("t-digest", 0))[0]
-    assert [-1, 19, 9] == await modclient.tdigest().revrank("t-digest", 21, 0, 10)
+def test_tdigest_revrank(client):
+    assert client.tdigest().create("t-digest", 500)
+    assert client.tdigest().add("t-digest", list(range(0, 20)))
+    assert -1 == client.tdigest().revrank("t-digest", 20)[0]
+    assert 19 == client.tdigest().revrank("t-digest", 0)[0]
+    assert [-1, 19, 9] == client.tdigest().revrank("t-digest", 21, 0, 10)
 
 
 @pytest.mark.redismod
 @pytest.mark.experimental
-async def test_tdigest_byrank(modclient: redis.Redis):
-    assert await modclient.tdigest().create("t-digest", 500)
-    assert await modclient.tdigest().add("t-digest", list(range(1, 11)))
-    assert 1 == (await modclient.tdigest().byrank("t-digest", 0))[0]
-    assert 10 == (await modclient.tdigest().byrank("t-digest", 9))[0]
-    assert (await modclient.tdigest().byrank("t-digest", 100))[0] == inf
+def test_tdigest_byrank(client):
+    assert client.tdigest().create("t-digest", 500)
+    assert client.tdigest().add("t-digest", list(range(1, 11)))
+    assert 1 == client.tdigest().byrank("t-digest", 0)[0]
+    assert 10 == client.tdigest().byrank("t-digest", 9)[0]
+    assert client.tdigest().byrank("t-digest", 100)[0] == inf
     with pytest.raises(redis.ResponseError):
-        (await modclient.tdigest().byrank("t-digest", -1))[0]
+        client.tdigest().byrank("t-digest", -1)[0]
 
 
 @pytest.mark.redismod
 @pytest.mark.experimental
-async def test_tdigest_byrevrank(modclient: redis.Redis):
-    assert await modclient.tdigest().create("t-digest", 500)
-    assert await modclient.tdigest().add("t-digest", list(range(1, 11)))
-    assert 10 == (await modclient.tdigest().byrevrank("t-digest", 0))[0]
-    assert 1 == (await modclient.tdigest().byrevrank("t-digest", 9))[0]
-    assert (await modclient.tdigest().byrevrank("t-digest", 100))[0] == -inf
+def test_tdigest_byrevrank(client):
+    assert client.tdigest().create("t-digest", 500)
+    assert client.tdigest().add("t-digest", list(range(1, 11)))
+    assert 10 == client.tdigest().byrevrank("t-digest", 0)[0]
+    assert 1 == client.tdigest().byrevrank("t-digest", 9)[0]
+    assert client.tdigest().byrevrank("t-digest", 100)[0] == -inf
     with pytest.raises(redis.ResponseError):
-        (await modclient.tdigest().byrevrank("t-digest", -1))[0]
+        client.tdigest().byrevrank("t-digest", -1)[0]
 
 
 # @pytest.mark.redismod
-# async def test_pipeline(modclient: redis.Redis):
-#     pipeline = await modclient.bf().pipeline()
-#     assert not await modclient.bf().execute_command("get pipeline")
+# def test_pipeline(client):
+#     pipeline = client.bf().pipeline()
+#     assert not client.bf().execute_command("get pipeline")
 #
-#     assert await modclient.bf().create("pipeline", 0.01, 1000)
+#     assert client.bf().create("pipeline", 0.01, 1000)
 #     for i in range(100):
 #         pipeline.add("pipeline", i)
 #     for i in range(100):
-#         assert not (await modclient.bf().exists("pipeline", i))
+#         assert not (client.bf().exists("pipeline", i))
 #
 #     pipeline.execute()
 #
 #     for i in range(100):
-#         assert await modclient.bf().exists("pipeline", i)
+#         assert client.bf().exists("pipeline", i)
```

### Comparing `redis-5.0.0b4/tests/test_asyncio/test_cluster.py` & `redis-5.0.0rc1/tests/test_asyncio/test_cluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import warnings
 from typing import Any, Awaitable, Callable, Dict, List, Optional, Type, Union
 from urllib.parse import urlparse
 
 import pytest
 import pytest_asyncio
 from _pytest.fixtures import FixtureRequest
-
 from redis.asyncio.cluster import ClusterNode, NodesManager, RedisCluster
 from redis.asyncio.connection import Connection, SSLConnection
 from redis.asyncio.retry import Retry
 from redis.backoff import ExponentialBackoff, NoBackoff, default_backoff
 from redis.cluster import PIPELINE_BLOCKED_COMMANDS, PRIMARY, REPLICA, get_node_name
 from redis.crc import REDIS_CLUSTER_HASH_SLOTS, key_slot
 from redis.exceptions import (
@@ -27,14 +26,15 @@
     RedisClusterException,
     RedisError,
     ResponseError,
 )
 from redis.parsers import AsyncCommandsParser
 from redis.utils import str_if_bytes
 from tests.conftest import (
+    assert_resp_response,
     skip_if_redis_enterprise,
     skip_if_server_version_lt,
     skip_unless_arch_bits,
 )
 
 from .compat import mock
 
@@ -1609,104 +1609,121 @@
         assert await r.smembers("{foo}c") == {b"1", b"2", b"3"}
 
     @skip_if_server_version_lt("6.2.0")
     async def test_cluster_zdiff(self, r: RedisCluster) -> None:
         await r.zadd("{foo}a", {"a1": 1, "a2": 2, "a3": 3})
         await r.zadd("{foo}b", {"a1": 1, "a2": 2})
         assert await r.zdiff(["{foo}a", "{foo}b"]) == [b"a3"]
-        assert await r.zdiff(["{foo}a", "{foo}b"], withscores=True) == [b"a3", b"3"]
+        response = await r.zdiff(["{foo}a", "{foo}b"], withscores=True)
+        assert_resp_response(r, response, [b"a3", b"3"], [[b"a3", 3.0]])
 
     @skip_if_server_version_lt("6.2.0")
     async def test_cluster_zdiffstore(self, r: RedisCluster) -> None:
         await r.zadd("{foo}a", {"a1": 1, "a2": 2, "a3": 3})
         await r.zadd("{foo}b", {"a1": 1, "a2": 2})
         assert await r.zdiffstore("{foo}out", ["{foo}a", "{foo}b"])
         assert await r.zrange("{foo}out", 0, -1) == [b"a3"]
-        assert await r.zrange("{foo}out", 0, -1, withscores=True) == [(b"a3", 3.0)]
+        response = await r.zrange("{foo}out", 0, -1, withscores=True)
+        assert_resp_response(r, response, [(b"a3", 3.0)], [[b"a3", 3.0]])
 
     @skip_if_server_version_lt("6.2.0")
     async def test_cluster_zinter(self, r: RedisCluster) -> None:
         await r.zadd("{foo}a", {"a1": 1, "a2": 2, "a3": 1})
         await r.zadd("{foo}b", {"a1": 2, "a2": 2, "a3": 2})
         await r.zadd("{foo}c", {"a1": 6, "a3": 5, "a4": 4})
         assert await r.zinter(["{foo}a", "{foo}b", "{foo}c"]) == [b"a3", b"a1"]
         # invalid aggregation
         with pytest.raises(DataError):
             await r.zinter(
                 ["{foo}a", "{foo}b", "{foo}c"], aggregate="foo", withscores=True
             )
         # aggregate with SUM
-        assert await r.zinter(["{foo}a", "{foo}b", "{foo}c"], withscores=True) == [
-            (b"a3", 8),
-            (b"a1", 9),
-        ]
+        response = await r.zinter(["{foo}a", "{foo}b", "{foo}c"], withscores=True)
+        assert_resp_response(
+            r, response, [(b"a3", 8), (b"a1", 9)], [[b"a3", 8], [b"a1", 9]]
+        )
         # aggregate with MAX
-        assert await r.zinter(
+        response = await r.zinter(
             ["{foo}a", "{foo}b", "{foo}c"], aggregate="MAX", withscores=True
-        ) == [(b"a3", 5), (b"a1", 6)]
+        )
+        assert_resp_response(
+            r, response, [(b"a3", 5), (b"a1", 6)], [[b"a3", 5], [b"a1", 6]]
+        )
         # aggregate with MIN
-        assert await r.zinter(
+        response = await r.zinter(
             ["{foo}a", "{foo}b", "{foo}c"], aggregate="MIN", withscores=True
-        ) == [(b"a1", 1), (b"a3", 1)]
+        )
+        assert_resp_response(
+            r, response, [(b"a1", 1), (b"a3", 1)], [[b"a1", 1], [b"a3", 1]]
+        )
         # with weights
-        assert await r.zinter(
-            {"{foo}a": 1, "{foo}b": 2, "{foo}c": 3}, withscores=True
-        ) == [(b"a3", 20), (b"a1", 23)]
+        res = await r.zinter({"{foo}a": 1, "{foo}b": 2, "{foo}c": 3}, withscores=True)
+        assert_resp_response(
+            r, res, [(b"a3", 20), (b"a1", 23)], [[b"a3", 20], [b"a1", 23]]
+        )
 
     async def test_cluster_zinterstore_sum(self, r: RedisCluster) -> None:
         await r.zadd("{foo}a", {"a1": 1, "a2": 1, "a3": 1})
         await r.zadd("{foo}b", {"a1": 2, "a2": 2, "a3": 2})
         await r.zadd("{foo}c", {"a1": 6, "a3": 5, "a4": 4})
         assert await r.zinterstore("{foo}d", ["{foo}a", "{foo}b", "{foo}c"]) == 2
-        assert await r.zrange("{foo}d", 0, -1, withscores=True) == [
-            (b"a3", 8),
-            (b"a1", 9),
-        ]
+        assert_resp_response(
+            r,
+            await r.zrange("{foo}d", 0, -1, withscores=True),
+            [(b"a3", 8), (b"a1", 9)],
+            [[b"a3", 8.0], [b"a1", 9.0]],
+        )
 
     async def test_cluster_zinterstore_max(self, r: RedisCluster) -> None:
         await r.zadd("{foo}a", {"a1": 1, "a2": 1, "a3": 1})
         await r.zadd("{foo}b", {"a1": 2, "a2": 2, "a3": 2})
         await r.zadd("{foo}c", {"a1": 6, "a3": 5, "a4": 4})
         assert (
             await r.zinterstore(
                 "{foo}d", ["{foo}a", "{foo}b", "{foo}c"], aggregate="MAX"
             )
             == 2
         )
-        assert await r.zrange("{foo}d", 0, -1, withscores=True) == [
-            (b"a3", 5),
-            (b"a1", 6),
-        ]
+        assert_resp_response(
+            r,
+            await r.zrange("{foo}d", 0, -1, withscores=True),
+            [(b"a3", 5), (b"a1", 6)],
+            [[b"a3", 5.0], [b"a1", 6.0]],
+        )
 
     async def test_cluster_zinterstore_min(self, r: RedisCluster) -> None:
         await r.zadd("{foo}a", {"a1": 1, "a2": 2, "a3": 3})
         await r.zadd("{foo}b", {"a1": 2, "a2": 3, "a3": 5})
         await r.zadd("{foo}c", {"a1": 6, "a3": 5, "a4": 4})
         assert (
             await r.zinterstore(
                 "{foo}d", ["{foo}a", "{foo}b", "{foo}c"], aggregate="MIN"
             )
             == 2
         )
-        assert await r.zrange("{foo}d", 0, -1, withscores=True) == [
-            (b"a1", 1),
-            (b"a3", 3),
-        ]
+        assert_resp_response(
+            r,
+            await r.zrange("{foo}d", 0, -1, withscores=True),
+            [(b"a1", 1), (b"a3", 3)],
+            [[b"a1", 1.0], [b"a3", 3.0]],
+        )
 
     async def test_cluster_zinterstore_with_weight(self, r: RedisCluster) -> None:
         await r.zadd("{foo}a", {"a1": 1, "a2": 1, "a3": 1})
         await r.zadd("{foo}b", {"a1": 2, "a2": 2, "a3": 2})
         await r.zadd("{foo}c", {"a1": 6, "a3": 5, "a4": 4})
         assert (
             await r.zinterstore("{foo}d", {"{foo}a": 1, "{foo}b": 2, "{foo}c": 3}) == 2
         )
-        assert await r.zrange("{foo}d", 0, -1, withscores=True) == [
-            (b"a3", 20),
-            (b"a1", 23),
-        ]
+        assert_resp_response(
+            r,
+            await r.zrange("{foo}d", 0, -1, withscores=True),
+            [(b"a3", 20), (b"a1", 23)],
+            [[b"a3", 20.0], [b"a1", 23.0]],
+        )
 
     @skip_if_server_version_lt("4.9.0")
     async def test_cluster_bzpopmax(self, r: RedisCluster) -> None:
         await r.zadd("{foo}a", {"a1": 1, "a2": 2})
         await r.zadd("{foo}b", {"b1": 10, "b2": 20})
         assert await r.bzpopmax(["{foo}b", "{foo}a"], timeout=1) == (
             b"{foo}b",
@@ -1763,18 +1780,20 @@
     @skip_if_server_version_lt("6.2.0")
     async def test_cluster_zrangestore(self, r: RedisCluster) -> None:
         await r.zadd("{foo}a", {"a1": 1, "a2": 2, "a3": 3})
         assert await r.zrangestore("{foo}b", "{foo}a", 0, 1)
         assert await r.zrange("{foo}b", 0, -1) == [b"a1", b"a2"]
         assert await r.zrangestore("{foo}b", "{foo}a", 1, 2)
         assert await r.zrange("{foo}b", 0, -1) == [b"a2", b"a3"]
-        assert await r.zrange("{foo}b", 0, -1, withscores=True) == [
-            (b"a2", 2),
-            (b"a3", 3),
-        ]
+        assert_resp_response(
+            r,
+            await r.zrange("{foo}b", 0, -1, withscores=True),
+            [(b"a2", 2), (b"a3", 3)],
+            [[b"a2", 2.0], [b"a3", 3.0]],
+        )
         # reversed order
         assert await r.zrangestore("{foo}b", "{foo}a", 1, 2, desc=True)
         assert await r.zrange("{foo}b", 0, -1) == [b"a1", b"a2"]
         # by score
         assert await r.zrangestore(
             "{foo}b", "{foo}a", 2, 1, byscore=True, offset=0, num=1, desc=True
         )
@@ -1793,92 +1812,105 @@
         # sum
         assert await r.zunion(["{foo}a", "{foo}b", "{foo}c"]) == [
             b"a2",
             b"a4",
             b"a3",
             b"a1",
         ]
-        assert await r.zunion(["{foo}a", "{foo}b", "{foo}c"], withscores=True) == [
-            (b"a2", 3),
-            (b"a4", 4),
-            (b"a3", 8),
-            (b"a1", 9),
-        ]
+        assert_resp_response(
+            r,
+            await r.zunion(["{foo}a", "{foo}b", "{foo}c"], withscores=True),
+            [(b"a2", 3), (b"a4", 4), (b"a3", 8), (b"a1", 9)],
+            [[b"a2", 3.0], [b"a4", 4.0], [b"a3", 8.0], [b"a1", 9.0]],
+        )
         # max
-        assert await r.zunion(
-            ["{foo}a", "{foo}b", "{foo}c"], aggregate="MAX", withscores=True
-        ) == [(b"a2", 2), (b"a4", 4), (b"a3", 5), (b"a1", 6)]
+        assert_resp_response(
+            r,
+            await r.zunion(
+                ["{foo}a", "{foo}b", "{foo}c"], aggregate="MAX", withscores=True
+            ),
+            [(b"a2", 2), (b"a4", 4), (b"a3", 5), (b"a1", 6)],
+            [[b"a2", 2.0], [b"a4", 4.0], [b"a3", 5.0], [b"a1", 6.0]],
+        )
         # min
-        assert await r.zunion(
-            ["{foo}a", "{foo}b", "{foo}c"], aggregate="MIN", withscores=True
-        ) == [(b"a1", 1), (b"a2", 1), (b"a3", 1), (b"a4", 4)]
+        assert_resp_response(
+            r,
+            await r.zunion(
+                ["{foo}a", "{foo}b", "{foo}c"], aggregate="MIN", withscores=True
+            ),
+            [(b"a1", 1), (b"a2", 1), (b"a3", 1), (b"a4", 4)],
+            [[b"a1", 1.0], [b"a2", 1.0], [b"a3", 1.0], [b"a4", 4.0]],
+        )
         # with weight
-        assert await r.zunion(
-            {"{foo}a": 1, "{foo}b": 2, "{foo}c": 3}, withscores=True
-        ) == [(b"a2", 5), (b"a4", 12), (b"a3", 20), (b"a1", 23)]
+        assert_resp_response(
+            r,
+            await r.zunion({"{foo}a": 1, "{foo}b": 2, "{foo}c": 3}, withscores=True),
+            [(b"a2", 5), (b"a4", 12), (b"a3", 20), (b"a1", 23)],
+            [[b"a2", 5.0], [b"a4", 12.0], [b"a3", 20.0], [b"a1", 23.0]],
+        )
 
     async def test_cluster_zunionstore_sum(self, r: RedisCluster) -> None:
         await r.zadd("{foo}a", {"a1": 1, "a2": 1, "a3": 1})
         await r.zadd("{foo}b", {"a1": 2, "a2": 2, "a3": 2})
         await r.zadd("{foo}c", {"a1": 6, "a3": 5, "a4": 4})
         assert await r.zunionstore("{foo}d", ["{foo}a", "{foo}b", "{foo}c"]) == 4
-        assert await r.zrange("{foo}d", 0, -1, withscores=True) == [
-            (b"a2", 3),
-            (b"a4", 4),
-            (b"a3", 8),
-            (b"a1", 9),
-        ]
+        assert_resp_response(
+            r,
+            await r.zrange("{foo}d", 0, -1, withscores=True),
+            [(b"a2", 3), (b"a4", 4), (b"a3", 8), (b"a1", 9)],
+            [[b"a2", 3.0], [b"a4", 4.0], [b"a3", 8.0], [b"a1", 9.0]],
+        )
 
     async def test_cluster_zunionstore_max(self, r: RedisCluster) -> None:
         await r.zadd("{foo}a", {"a1": 1, "a2": 1, "a3": 1})
         await r.zadd("{foo}b", {"a1": 2, "a2": 2, "a3": 2})
         await r.zadd("{foo}c", {"a1": 6, "a3": 5, "a4": 4})
         assert (
             await r.zunionstore(
                 "{foo}d", ["{foo}a", "{foo}b", "{foo}c"], aggregate="MAX"
             )
             == 4
         )
-        assert await r.zrange("{foo}d", 0, -1, withscores=True) == [
-            (b"a2", 2),
-            (b"a4", 4),
-            (b"a3", 5),
-            (b"a1", 6),
-        ]
+        assert_resp_response(
+            r,
+            await r.zrange("{foo}d", 0, -1, withscores=True),
+            [(b"a2", 2), (b"a4", 4), (b"a3", 5), (b"a1", 6)],
+            [[b"a2", 2.0], [b"a4", 4.0], [b"a3", 5.0], [b"a1", 6.0]],
+        )
 
     async def test_cluster_zunionstore_min(self, r: RedisCluster) -> None:
         await r.zadd("{foo}a", {"a1": 1, "a2": 2, "a3": 3})
         await r.zadd("{foo}b", {"a1": 2, "a2": 2, "a3": 4})
         await r.zadd("{foo}c", {"a1": 6, "a3": 5, "a4": 4})
         assert (
             await r.zunionstore(
                 "{foo}d", ["{foo}a", "{foo}b", "{foo}c"], aggregate="MIN"
             )
             == 4
         )
-        assert await r.zrange("{foo}d", 0, -1, withscores=True) == [
-            (b"a1", 1),
-            (b"a2", 2),
-            (b"a3", 3),
-            (b"a4", 4),
-        ]
+        assert_resp_response(
+            r,
+            await r.zrange("{foo}d", 0, -1, withscores=True),
+            [(b"a1", 1), (b"a2", 2), (b"a3", 3), (b"a4", 4)],
+            [[b"a1", 1.0], [b"a2", 2.0], [b"a3", 3.0], [b"a4", 4.0]],
+        )
 
     async def test_cluster_zunionstore_with_weight(self, r: RedisCluster) -> None:
         await r.zadd("{foo}a", {"a1": 1, "a2": 1, "a3": 1})
         await r.zadd("{foo}b", {"a1": 2, "a2": 2, "a3": 2})
         await r.zadd("{foo}c", {"a1": 6, "a3": 5, "a4": 4})
         assert (
             await r.zunionstore("{foo}d", {"{foo}a": 1, "{foo}b": 2, "{foo}c": 3}) == 4
         )
-        assert await r.zrange("{foo}d", 0, -1, withscores=True) == [
-            (b"a2", 5),
-            (b"a4", 12),
-            (b"a3", 20),
-            (b"a1", 23),
-        ]
+        assert_resp_response(
+            r,
+            await r.zrange("{foo}d", 0, -1, withscores=True),
+            [(b"a2", 5), (b"a4", 12), (b"a3", 20), (b"a1", 23)],
+            [[b"a2", 5.0], [b"a4", 12.0], [b"a3", 20.0], [b"a1", 23.0]],
+        )
 
     @skip_if_server_version_lt("2.8.9")
     async def test_cluster_pfcount(self, r: RedisCluster) -> None:
         members = {b"1", b"2", b"3"}
         await r.pfadd("{foo}a", *members)
         assert await r.pfcount("{foo}a") == len(members)
         members_b = {b"2", b"3", b"4"}
@@ -2655,18 +2687,18 @@
     Tests for SSL connections.
 
     This relies on the --redis-ssl-url for building the client and connecting to the
     appropriate port.
     """
 
     ROOT = os.path.join(os.path.dirname(__file__), "../..")
-    CERT_DIR = os.path.abspath(os.path.join(ROOT, "docker", "stunnel", "keys"))
+    CERT_DIR = os.path.abspath(os.path.join(ROOT, "dockers", "stunnel", "keys"))
     if not os.path.isdir(CERT_DIR):  # github actions package validation case
         CERT_DIR = os.path.abspath(
-            os.path.join(ROOT, "..", "docker", "stunnel", "keys")
+            os.path.join(ROOT, "..", "dockers", "stunnel", "keys")
         )
         if not os.path.isdir(CERT_DIR):
             raise IOError(f"No SSL certificates found. They should be in {CERT_DIR}")
 
     SERVER_CERT = os.path.join(CERT_DIR, "server-cert.pem")
     SERVER_KEY = os.path.join(CERT_DIR, "server-key.pem")
```

### Comparing `redis-5.0.0b4/tests/test_asyncio/test_commands.py` & `redis-5.0.0rc1/tests/test_asyncio/test_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 import binascii
 import datetime
 import re
 from string import ascii_letters
 
 import pytest
 import pytest_asyncio
-
 import redis
 from redis import exceptions
 from redis.client import EMPTY_RESPONSE, NEVER_DECODE, parse_info
 from tests.conftest import (
+    assert_resp_response,
+    assert_resp_response_in,
+    is_resp2_connection,
     skip_if_server_version_gte,
     skip_if_server_version_lt,
     skip_unless_arch_bits,
 )
 
-from .conftest import assert_resp_response, assert_resp_response_in
-
 REDIS_6_VERSION = "5.9.0"
 
 
 @pytest_asyncio.fixture()
 async def r_teardown(r: redis.Redis):
     """
     A special fixture which removes the provided names from the database after use
@@ -69,22 +69,27 @@
 
 # RESPONSE CALLBACKS
 @pytest.mark.onlynoncluster
 class TestResponseCallbacks:
     """Tests for the response callback system"""
 
     async def test_response_callbacks(self, r: redis.Redis):
-        assert r.response_callbacks == redis.Redis.RESPONSE_CALLBACKS
+        callbacks = redis.Redis.RESPONSE_CALLBACKS
+        if is_resp2_connection(r):
+            callbacks.update(redis.Redis.RESP2_RESPONSE_CALLBACKS)
+        else:
+            callbacks.update(redis.Redis.RESP3_RESPONSE_CALLBACKS)
+        assert r.response_callbacks == callbacks
         assert id(r.response_callbacks) != id(redis.Redis.RESPONSE_CALLBACKS)
         r.set_response_callback("GET", lambda x: "static")
         await r.set("a", "foo")
         assert await r.get("a") == "static"
 
     async def test_case_insensitive_command_names(self, r: redis.Redis):
-        assert r.response_callbacks["del"] == r.response_callbacks["DEL"]
+        assert r.response_callbacks["ping"] == r.response_callbacks["PING"]
 
 
 class TestRedisCommands:
     async def test_command_on_invalid_key_type(self, r: redis.Redis):
         await r.lpush("a", "1")
         with pytest.raises(redis.ResponseError):
             await r.get("a")
@@ -112,60 +117,55 @@
         assert await r.acl_deluser(username) == 1
 
     @skip_if_server_version_lt(REDIS_6_VERSION)
     async def test_acl_genpass(self, r: redis.Redis):
         password = await r.acl_genpass()
         assert isinstance(password, str)
 
-    @skip_if_server_version_lt(REDIS_6_VERSION)
-    @skip_if_server_version_gte("7.0.0")
+    @skip_if_server_version_lt("7.0.0")
     async def test_acl_getuser_setuser(self, r_teardown):
         username = "redis-py-user"
         r = r_teardown(username)
         # test enabled=False
         assert await r.acl_setuser(username, enabled=False, reset=True)
-        assert await r.acl_getuser(username) == {
-            "categories": ["-@all"],
-            "commands": [],
-            "channels": [b"*"],
-            "enabled": False,
-            "flags": ["off", "allchannels", "sanitize-payload"],
-            "keys": [],
-            "passwords": [],
-        }
+        acl = await r.acl_getuser(username)
+        assert acl["categories"] == ["-@all"]
+        assert acl["commands"] == []
+        assert acl["keys"] == []
+        assert acl["passwords"] == []
+        assert "off" in acl["flags"]
+        assert acl["enabled"] is False
 
         # test nopass=True
         assert await r.acl_setuser(username, enabled=True, reset=True, nopass=True)
-        assert await r.acl_getuser(username) == {
-            "categories": ["-@all"],
-            "commands": [],
-            "channels": [b"*"],
-            "enabled": True,
-            "flags": ["on", "allchannels", "nopass", "sanitize-payload"],
-            "keys": [],
-            "passwords": [],
-        }
+        acl = await r.acl_getuser(username)
+        assert acl["categories"] == ["-@all"]
+        assert acl["commands"] == []
+        assert acl["keys"] == []
+        assert acl["passwords"] == []
+        assert "on" in acl["flags"]
+        assert "nopass" in acl["flags"]
+        assert acl["enabled"] is True
 
         # test all args
         assert await r.acl_setuser(
             username,
             enabled=True,
             reset=True,
             passwords=["+pass1", "+pass2"],
             categories=["+set", "+@hash", "-geo"],
             commands=["+get", "+mget", "-hset"],
             keys=["cache:*", "objects:*"],
         )
         acl = await r.acl_getuser(username)
-        assert set(acl["categories"]) == {"-@all", "+@set", "+@hash"}
+        assert set(acl["categories"]) == {"-@all", "+@set", "+@hash", "-@geo"}
         assert set(acl["commands"]) == {"+get", "+mget", "-hset"}
         assert acl["enabled"] is True
-        assert acl["channels"] == [b"*"]
-        assert acl["flags"] == ["on", "allchannels", "sanitize-payload"]
-        assert set(acl["keys"]) == {b"cache:*", b"objects:*"}
+        assert "on" in acl["flags"]
+        assert set(acl["keys"]) == {"~cache:*", "~objects:*"}
         assert len(acl["passwords"]) == 2
 
         # test reset=False keeps existing ACL and applies new ACL on top
         assert await r.acl_setuser(
             username,
             enabled=True,
             reset=True,
@@ -179,20 +179,18 @@
             enabled=True,
             passwords=["+pass2"],
             categories=["+@hash"],
             commands=["+mget"],
             keys=["objects:*"],
         )
         acl = await r.acl_getuser(username)
-        assert set(acl["categories"]) == {"-@all", "+@set", "+@hash"}
         assert set(acl["commands"]) == {"+get", "+mget"}
         assert acl["enabled"] is True
-        assert acl["channels"] == [b"*"]
-        assert acl["flags"] == ["on", "allchannels", "sanitize-payload"]
-        assert set(acl["keys"]) == {b"cache:*", b"objects:*"}
+        assert "on" in acl["flags"]
+        assert set(acl["keys"]) == {"~cache:*", "~objects:*"}
         assert len(acl["passwords"]) == 2
 
         # test removal of passwords
         assert await r.acl_setuser(
             username, enabled=True, reset=True, passwords=["+pass1", "+pass2"]
         )
         assert len((await r.acl_getuser(username))["passwords"]) == 2
@@ -220,22 +218,21 @@
         assert len((await r.acl_getuser(username))["passwords"]) == 2
         assert await r.acl_setuser(
             username, enabled=True, hashed_passwords=["-" + hashed_password]
         )
         assert len((await r.acl_getuser(username))["passwords"]) == 1
 
     @skip_if_server_version_lt(REDIS_6_VERSION)
-    @skip_if_server_version_gte("7.0.0")
     async def test_acl_list(self, r_teardown):
         username = "redis-py-user"
         r = r_teardown(username)
-
+        start = await r.acl_list()
         assert await r.acl_setuser(username, enabled=False, reset=True)
         users = await r.acl_list()
-        assert f"user {username} off sanitize-payload &* -@all" in users
+        assert len(users) == len(start) + 1
 
     @skip_if_server_version_lt(REDIS_6_VERSION)
     @pytest.mark.onlynoncluster
     async def test_acl_log(self, r_teardown, create_redis):
         username = "redis-py-user"
         r = r_teardown(username)
         await r.acl_setuser(
@@ -2712,15 +2709,15 @@
                 "last-delivered-id": message_id,
                 "entries-read": 2,
                 "lag": -1,
             }
         ]
         assert await r.xinfo_groups(stream) == expected
 
-    @skip_if_server_version_lt("5.0.0")
+    @skip_if_server_version_lt("7.2.0")
     async def test_xinfo_consumers(self, r: redis.Redis):
         stream = "stream"
         group = "group"
         consumer1 = "consumer1"
         consumer2 = "consumer2"
         await r.xadd(stream, {"foo": "bar"})
         await r.xadd(stream, {"foo": "bar"})
@@ -2728,16 +2725,16 @@
 
         await r.xgroup_create(stream, group, 0)
         await r.xreadgroup(group, consumer1, streams={stream: ">"}, count=1)
         await r.xreadgroup(group, consumer2, streams={stream: ">"})
         info = await r.xinfo_consumers(stream, group)
         assert len(info) == 2
         expected = [
-            {"name": consumer1.encode(), "pending": 1},
-            {"name": consumer2.encode(), "pending": 2},
+            {"name": consumer1.encode(), "pending": 1, "inactive": 2},
+            {"name": consumer2.encode(), "pending": 2, "inactive": 2},
         ]
 
         # we can't determine the idle time, so just make sure it's an int
         assert isinstance(info[0].pop("idle"), int)
         assert isinstance(info[1].pop("idle"), int)
         assert info == expected
 
@@ -2908,24 +2905,24 @@
         # xread starting after the last message returns an empty message list
         res = await r.xreadgroup(group, consumer, streams={stream: ">"})
         assert_resp_response(r, res, [], {})
 
         # xreadgroup with noack does not have any items in the PEL
         await r.xgroup_destroy(stream, group)
         await r.xgroup_create(stream, group, "0")
-        # res = r.xreadgroup(group, consumer, streams={stream: ">"}, noack=True)
-        # empty_res = r.xreadgroup(group, consumer, streams={stream: "0"})
-        # if is_resp2_connection(r):
-        #     assert len(res[0][1]) == 2
-        #     # now there should be nothing pending
-        #     assert len(empty_res[0][1]) == 0
-        # else:
-        #     assert len(res[strem_name][0]) == 2
-        #     # now there should be nothing pending
-        #     assert len(empty_res[strem_name][0]) == 0
+        res = await r.xreadgroup(group, consumer, streams={stream: ">"}, noack=True)
+        empty_res = await r.xreadgroup(group, consumer, streams={stream: "0"})
+        if is_resp2_connection(r):
+            assert len(res[0][1]) == 2
+            # now there should be nothing pending
+            assert len(empty_res[0][1]) == 0
+        else:
+            assert len(res[strem_name][0]) == 2
+            # now there should be nothing pending
+            assert len(empty_res[strem_name][0]) == 0
 
         await r.xgroup_destroy(stream, group)
         await r.xgroup_create(stream, group, "0")
         # delete all the messages in the stream
         expected_entries = [(m1, {}), (m2, {})]
         await r.xreadgroup(group, consumer, streams={stream: ">"})
         await r.xtrim(stream, 0)
```

### Comparing `redis-5.0.0b4/tests/test_asyncio/test_connection.py` & `redis-5.0.0rc1/tests/test_asyncio/test_connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 import asyncio
 import socket
 import types
 from unittest.mock import patch
 
 import pytest
-
 import redis
 from redis.asyncio import Redis
 from redis.asyncio.connection import Connection, UnixDomainSocketConnection
 from redis.asyncio.retry import Retry
 from redis.backoff import NoBackoff
 from redis.exceptions import ConnectionError, InvalidResponse, TimeoutError
-from redis.parsers import _AsyncHiredisParser, _AsyncRESP2Parser, _AsyncRESP3Parser
+from redis.parsers import (
+    _AsyncHiredisParser,
+    _AsyncRESP2Parser,
+    _AsyncRESP3Parser,
+    _AsyncRESPBase,
+)
 from redis.utils import HIREDIS_AVAILABLE
 from tests.conftest import skip_if_server_version_lt
 
 from .compat import mock
 from .mocks import MockStream
 
 
 @pytest.mark.onlynoncluster
 async def test_invalid_response(create_redis):
     r = await create_redis(single_connection_client=True)
 
     raw = b"x"
     fake_stream = MockStream(raw + b"\r\n")
 
-    parser: _AsyncRESP2Parser = r.connection._parser
+    parser: _AsyncRESPBase = r.connection._parser
     with mock.patch.object(parser, "_stream", fake_stream):
         with pytest.raises(InvalidResponse) as cm:
             await parser.read_response()
-    if isinstance(parser, _AsyncRESP2Parser):
+    if isinstance(parser, _AsyncRESPBase):
         assert str(cm.value) == f"Protocol Error: {raw!r}"
     else:
         assert (
             str(cm.value) == f'Protocol error, got "{raw.decode()}" as reply type byte'
         )
     await r.connection.disconnect()
 
@@ -103,30 +107,30 @@
     assert init_call_count == 1
     assert command_call_count == 2
 
 
 @skip_if_server_version_lt("4.0.0")
 @pytest.mark.redismod
 @pytest.mark.onlynoncluster
-async def test_loading_external_modules(modclient):
+async def test_loading_external_modules(r):
     def inner():
         pass
 
-    modclient.load_external_module("myfuncname", inner)
-    assert getattr(modclient, "myfuncname") == inner
-    assert isinstance(getattr(modclient, "myfuncname"), types.FunctionType)
+    r.load_external_module("myfuncname", inner)
+    assert getattr(r, "myfuncname") == inner
+    assert isinstance(getattr(r, "myfuncname"), types.FunctionType)
 
     # and call it
     from redis.commands import RedisModuleCommands
 
     j = RedisModuleCommands.json
-    modclient.load_external_module("sometestfuncname", j)
+    r.load_external_module("sometestfuncname", j)
 
     # d = {'hello': 'world!'}
-    # mod = j(modclient)
+    # mod = j(r)
     # mod.set("fookey", ".", d)
     # assert mod.get('fookey') == d
 
 
 async def test_socket_param_regression(r):
     """A regression test for issue #1060"""
     conn = UnixDomainSocketConnection()
```

### Comparing `redis-5.0.0b4/tests/test_asyncio/test_connection_pool.py` & `redis-5.0.0rc1/tests/test_asyncio/test_connection_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
 import os
 import re
 
 import pytest
 import pytest_asyncio
-
 import redis.asyncio as redis
 from redis.asyncio.connection import Connection, to_bool
 from tests.conftest import skip_if_redis_enterprise, skip_if_server_version_lt
 
 from .compat import mock
 from .conftest import asynccontextmanager
 from .test_pubsub import wait_for_message
@@ -242,16 +241,17 @@
             max_connections=1, timeout=0.1, connection_kwargs=connection_kwargs
         ) as pool:
             c1 = await pool.get_connection("_")
 
             start = asyncio.get_running_loop().time()
             with pytest.raises(redis.ConnectionError):
                 await pool.get_connection("_")
-            # we should have waited at least 0.1 seconds
-            assert asyncio.get_running_loop().time() - start >= 0.1
+
+            # we should have waited at least some period of time
+            assert asyncio.get_running_loop().time() - start >= 0.05
             await c1.disconnect()
 
     async def test_connection_pool_blocks_until_conn_available(self, master_host):
         """
         When out of connections, block until another connection is released
         to the pool
         """
@@ -263,15 +263,16 @@
 
             async def target():
                 await asyncio.sleep(0.1)
                 await pool.release(c1)
 
             start = asyncio.get_running_loop().time()
             await asyncio.gather(target(), pool.get_connection("_"))
-            assert asyncio.get_running_loop().time() - start >= 0.1
+            stop = asyncio.get_running_loop().time()
+            assert (stop - start) <= 0.2
 
     async def test_reuse_previously_released_connection(self, master_host):
         connection_kwargs = {"host": master_host}
         async with self.get_pool(connection_kwargs=connection_kwargs) as pool:
             c1 = await pool.get_connection("_")
             await pool.release(c1)
             c2 = await pool.get_connection("_")
@@ -654,14 +655,15 @@
     async def r(self, create_redis, server):
         redis = await create_redis(single_connection_client=False)
         yield redis
         await redis.flushall()
 
 
 @pytest.mark.onlynoncluster
+@pytest.mark.xfail(strict=False)
 class TestHealthCheck:
     interval = 60
 
     @pytest_asyncio.fixture()
     async def r(self, create_redis):
         redis = await create_redis(health_check_interval=self.interval)
         yield redis
```

### Comparing `redis-5.0.0b4/tests/test_asyncio/test_credentials.py` & `redis-5.0.0rc1/tests/test_asyncio/test_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import functools
 import random
 import string
 from typing import Optional, Tuple, Union
 
 import pytest
 import pytest_asyncio
-
 import redis
 from redis import AuthenticationError, DataError, ResponseError
 from redis.credentials import CredentialProvider, UsernamePasswordCredentialProvider
 from redis.utils import str_if_bytes
 from tests.conftest import skip_if_redis_enterprise
```

### Comparing `redis-5.0.0b4/tests/test_asyncio/test_encoding.py` & `redis-5.0.0rc1/tests/test_asyncio/test_encoding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pytest
 import pytest_asyncio
-
 import redis.asyncio as redis
 from redis.exceptions import DataError
 
 
 @pytest.mark.onlynoncluster
 class TestEncoding:
     @pytest_asyncio.fixture()
@@ -86,14 +85,15 @@
 class TestCommandsAreNotEncoded:
     @pytest_asyncio.fixture()
     async def r(self, create_redis):
         redis = await create_redis(encoding="utf-16")
         yield redis
         await redis.flushall()
 
+    @pytest.mark.xfail
     async def test_basic_command(self, r: redis.Redis):
         await r.set("hello", "world")
 
 
 class TestInvalidUserInput:
     async def test_boolean_fails(self, r: redis.Redis):
         with pytest.raises(DataError):
```

### Comparing `redis-5.0.0b4/tests/test_asyncio/test_graph.py` & `redis-5.0.0rc1/tests/test_asyncio/test_graph.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import pytest
-
 import redis.asyncio as redis
 from redis.commands.graph import Edge, Node, Path
 from redis.commands.graph.execution_plan import Operation
 from redis.exceptions import ResponseError
 from tests.conftest import skip_if_redis_enterprise
 
 
 @pytest.mark.redismod
-async def test_bulk(modclient):
+async def test_bulk(decoded_r):
     with pytest.raises(NotImplementedError):
-        await modclient.graph().bulk()
-        await modclient.graph().bulk(foo="bar!")
+        await decoded_r.graph().bulk()
+        await decoded_r.graph().bulk(foo="bar!")
 
 
 @pytest.mark.redismod
-async def test_graph_creation(modclient: redis.Redis):
-    graph = modclient.graph()
+async def test_graph_creation(decoded_r: redis.Redis):
+    graph = decoded_r.graph()
 
     john = Node(
         label="person",
         properties={
             "name": "John Doe",
             "age": 33,
             "gender": "male",
@@ -56,16 +55,16 @@
     assert [1, 2.3, "4", True, False, None] == result.result_set[0][0]
 
     # All done, remove graph.
     await graph.delete()
 
 
 @pytest.mark.redismod
-async def test_array_functions(modclient: redis.Redis):
-    graph = modclient.graph()
+async def test_array_functions(decoded_r: redis.Redis):
+    graph = decoded_r.graph()
 
     query = """CREATE (p:person{name:'a',age:32, array:[0,1,2]})"""
     await graph.query(query)
 
     query = """WITH [0,1,2] as x return x"""
     result = await graph.query(query)
     assert [0, 1, 2] == result.result_set[0][0]
@@ -79,95 +78,95 @@
         properties={"name": "a", "age": 32, "array": [0, 1, 2]},
     )
 
     assert [a] == result.result_set[0][0]
 
 
 @pytest.mark.redismod
-async def test_path(modclient: redis.Redis):
+async def test_path(decoded_r: redis.Redis):
     node0 = Node(node_id=0, label="L1")
     node1 = Node(node_id=1, label="L1")
     edge01 = Edge(node0, "R1", node1, edge_id=0, properties={"value": 1})
 
-    graph = modclient.graph()
+    graph = decoded_r.graph()
     graph.add_node(node0)
     graph.add_node(node1)
     graph.add_edge(edge01)
     await graph.flush()
 
     path01 = Path.new_empty_path().add_node(node0).add_edge(edge01).add_node(node1)
     expected_results = [[path01]]
 
     query = "MATCH p=(:L1)-[:R1]->(:L1) RETURN p ORDER BY p"
     result = await graph.query(query)
     assert expected_results == result.result_set
 
 
 @pytest.mark.redismod
-async def test_param(modclient: redis.Redis):
+async def test_param(decoded_r: redis.Redis):
     params = [1, 2.3, "str", True, False, None, [0, 1, 2]]
     query = "RETURN $param"
     for param in params:
-        result = await modclient.graph().query(query, {"param": param})
+        result = await decoded_r.graph().query(query, {"param": param})
         expected_results = [[param]]
         assert expected_results == result.result_set
 
 
 @pytest.mark.redismod
-async def test_map(modclient: redis.Redis):
+async def test_map(decoded_r: redis.Redis):
     query = "RETURN {a:1, b:'str', c:NULL, d:[1,2,3], e:True, f:{x:1, y:2}}"
 
-    actual = (await modclient.graph().query(query)).result_set[0][0]
+    actual = (await decoded_r.graph().query(query)).result_set[0][0]
     expected = {
         "a": 1,
         "b": "str",
         "c": None,
         "d": [1, 2, 3],
         "e": True,
         "f": {"x": 1, "y": 2},
     }
 
     assert actual == expected
 
 
 @pytest.mark.redismod
-async def test_point(modclient: redis.Redis):
+async def test_point(decoded_r: redis.Redis):
     query = "RETURN point({latitude: 32.070794860, longitude: 34.820751118})"
     expected_lat = 32.070794860
     expected_lon = 34.820751118
-    actual = (await modclient.graph().query(query)).result_set[0][0]
+    actual = (await decoded_r.graph().query(query)).result_set[0][0]
     assert abs(actual["latitude"] - expected_lat) < 0.001
     assert abs(actual["longitude"] - expected_lon) < 0.001
 
     query = "RETURN point({latitude: 32, longitude: 34.0})"
     expected_lat = 32
     expected_lon = 34
-    actual = (await modclient.graph().query(query)).result_set[0][0]
+    actual = (await decoded_r.graph().query(query)).result_set[0][0]
     assert abs(actual["latitude"] - expected_lat) < 0.001
     assert abs(actual["longitude"] - expected_lon) < 0.001
 
 
 @pytest.mark.redismod
-async def test_index_response(modclient: redis.Redis):
-    result_set = await modclient.graph().query("CREATE INDEX ON :person(age)")
+async def test_index_response(decoded_r: redis.Redis):
+    result_set = await decoded_r.graph().query("CREATE INDEX ON :person(age)")
     assert 1 == result_set.indices_created
 
-    result_set = await modclient.graph().query("CREATE INDEX ON :person(age)")
+    result_set = await decoded_r.graph().query("CREATE INDEX ON :person(age)")
     assert 0 == result_set.indices_created
 
-    result_set = await modclient.graph().query("DROP INDEX ON :person(age)")
+    result_set = await decoded_r.graph().query("DROP INDEX ON :person(age)")
     assert 1 == result_set.indices_deleted
 
     with pytest.raises(ResponseError):
-        await modclient.graph().query("DROP INDEX ON :person(age)")
+        await decoded_r.graph().query("DROP INDEX ON :person(age)")
 
 
 @pytest.mark.redismod
-async def test_stringify_query_result(modclient: redis.Redis):
-    graph = modclient.graph()
+async def test_stringify_query_result(decoded_r: redis.Redis):
+    graph = decoded_r.graph()
 
     john = Node(
         alias="a",
         label="person",
         properties={
             "name": "John Doe",
             "age": 33,
@@ -212,22 +211,22 @@
     assert str(visit) == """()-[:visited{purpose:"pleasure"}]->()"""
     assert str(country) == """(:country{name:"Japan"})"""
 
     await graph.delete()
 
 
 @pytest.mark.redismod
-async def test_optional_match(modclient: redis.Redis):
+async def test_optional_match(decoded_r: redis.Redis):
     # Build a graph of form (a)-[R]->(b)
     node0 = Node(node_id=0, label="L1", properties={"value": "a"})
     node1 = Node(node_id=1, label="L1", properties={"value": "b"})
 
     edge01 = Edge(node0, "R", node1, edge_id=0)
 
-    graph = modclient.graph()
+    graph = decoded_r.graph()
     graph.add_node(node0)
     graph.add_node(node1)
     graph.add_edge(edge01)
     await graph.flush()
 
     # Issue a query that collects all outgoing edges from both nodes
     # (the second has none)
@@ -237,143 +236,144 @@
     result = await graph.query(query)
     assert expected_results == result.result_set
 
     await graph.delete()
 
 
 @pytest.mark.redismod
-async def test_cached_execution(modclient: redis.Redis):
-    await modclient.graph().query("CREATE ()")
+async def test_cached_execution(decoded_r: redis.Redis):
+    await decoded_r.graph().query("CREATE ()")
 
-    uncached_result = await modclient.graph().query(
+    uncached_result = await decoded_r.graph().query(
         "MATCH (n) RETURN n, $param", {"param": [0]}
     )
     assert uncached_result.cached_execution is False
 
     # loop to make sure the query is cached on each thread on server
     for x in range(0, 64):
-        cached_result = await modclient.graph().query(
+        cached_result = await decoded_r.graph().query(
             "MATCH (n) RETURN n, $param", {"param": [0]}
         )
         assert uncached_result.result_set == cached_result.result_set
 
     # should be cached on all threads by now
     assert cached_result.cached_execution
 
 
 @pytest.mark.redismod
-async def test_slowlog(modclient: redis.Redis):
+async def test_slowlog(decoded_r: redis.Redis):
     create_query = """CREATE
     (:Rider {name:'Valentino Rossi'})-[:rides]->(:Team {name:'Yamaha'}),
     (:Rider {name:'Dani Pedrosa'})-[:rides]->(:Team {name:'Honda'}),
     (:Rider {name:'Andrea Dovizioso'})-[:rides]->(:Team {name:'Ducati'})"""
-    await modclient.graph().query(create_query)
+    await decoded_r.graph().query(create_query)
 
-    results = await modclient.graph().slowlog()
+    results = await decoded_r.graph().slowlog()
     assert results[0][1] == "GRAPH.QUERY"
     assert results[0][2] == create_query
 
 
 @pytest.mark.redismod
-async def test_query_timeout(modclient: redis.Redis):
+@pytest.mark.xfail(strict=False)
+async def test_query_timeout(decoded_r: redis.Redis):
     # Build a sample graph with 1000 nodes.
-    await modclient.graph().query("UNWIND range(0,1000) as val CREATE ({v: val})")
+    await decoded_r.graph().query("UNWIND range(0,1000) as val CREATE ({v: val})")
     # Issue a long-running query with a 1-millisecond timeout.
     with pytest.raises(ResponseError):
-        await modclient.graph().query("MATCH (a), (b), (c), (d) RETURN *", timeout=1)
+        await decoded_r.graph().query("MATCH (a), (b), (c), (d) RETURN *", timeout=1)
         assert False is False
 
     with pytest.raises(Exception):
-        await modclient.graph().query("RETURN 1", timeout="str")
+        await decoded_r.graph().query("RETURN 1", timeout="str")
         assert False is False
 
 
 @pytest.mark.redismod
-async def test_read_only_query(modclient: redis.Redis):
+async def test_read_only_query(decoded_r: redis.Redis):
     with pytest.raises(Exception):
         # Issue a write query, specifying read-only true,
         # this call should fail.
-        await modclient.graph().query("CREATE (p:person {name:'a'})", read_only=True)
+        await decoded_r.graph().query("CREATE (p:person {name:'a'})", read_only=True)
         assert False is False
 
 
 @pytest.mark.redismod
-async def test_profile(modclient: redis.Redis):
+async def test_profile(decoded_r: redis.Redis):
     q = """UNWIND range(1, 3) AS x CREATE (p:Person {v:x})"""
-    profile = (await modclient.graph().profile(q)).result_set
+    profile = (await decoded_r.graph().profile(q)).result_set
     assert "Create | Records produced: 3" in profile
     assert "Unwind | Records produced: 3" in profile
 
     q = "MATCH (p:Person) WHERE p.v > 1 RETURN p"
-    profile = (await modclient.graph().profile(q)).result_set
+    profile = (await decoded_r.graph().profile(q)).result_set
     assert "Results | Records produced: 2" in profile
     assert "Project | Records produced: 2" in profile
     assert "Filter | Records produced: 2" in profile
     assert "Node By Label Scan | (p:Person) | Records produced: 3" in profile
 
 
 @pytest.mark.redismod
 @skip_if_redis_enterprise()
-async def test_config(modclient: redis.Redis):
+async def test_config(decoded_r: redis.Redis):
     config_name = "RESULTSET_SIZE"
     config_value = 3
 
     # Set configuration
-    response = await modclient.graph().config(config_name, config_value, set=True)
+    response = await decoded_r.graph().config(config_name, config_value, set=True)
     assert response == "OK"
 
     # Make sure config been updated.
-    response = await modclient.graph().config(config_name, set=False)
+    response = await decoded_r.graph().config(config_name, set=False)
     expected_response = [config_name, config_value]
     assert response == expected_response
 
     config_name = "QUERY_MEM_CAPACITY"
     config_value = 1 << 20  # 1MB
 
     # Set configuration
-    response = await modclient.graph().config(config_name, config_value, set=True)
+    response = await decoded_r.graph().config(config_name, config_value, set=True)
     assert response == "OK"
 
     # Make sure config been updated.
-    response = await modclient.graph().config(config_name, set=False)
+    response = await decoded_r.graph().config(config_name, set=False)
     expected_response = [config_name, config_value]
     assert response == expected_response
 
     # reset to default
-    await modclient.graph().config("QUERY_MEM_CAPACITY", 0, set=True)
-    await modclient.graph().config("RESULTSET_SIZE", -100, set=True)
+    await decoded_r.graph().config("QUERY_MEM_CAPACITY", 0, set=True)
+    await decoded_r.graph().config("RESULTSET_SIZE", -100, set=True)
 
 
 @pytest.mark.redismod
 @pytest.mark.onlynoncluster
-async def test_list_keys(modclient: redis.Redis):
-    result = await modclient.graph().list_keys()
+async def test_list_keys(decoded_r: redis.Redis):
+    result = await decoded_r.graph().list_keys()
     assert result == []
 
-    await modclient.graph("G").query("CREATE (n)")
-    result = await modclient.graph().list_keys()
+    await decoded_r.graph("G").query("CREATE (n)")
+    result = await decoded_r.graph().list_keys()
     assert result == ["G"]
 
-    await modclient.graph("X").query("CREATE (m)")
-    result = await modclient.graph().list_keys()
+    await decoded_r.graph("X").query("CREATE (m)")
+    result = await decoded_r.graph().list_keys()
     assert result == ["G", "X"]
 
-    await modclient.delete("G")
-    await modclient.rename("X", "Z")
-    result = await modclient.graph().list_keys()
+    await decoded_r.delete("G")
+    await decoded_r.rename("X", "Z")
+    result = await decoded_r.graph().list_keys()
     assert result == ["Z"]
 
-    await modclient.delete("Z")
-    result = await modclient.graph().list_keys()
+    await decoded_r.delete("Z")
+    result = await decoded_r.graph().list_keys()
     assert result == []
 
 
 @pytest.mark.redismod
-async def test_multi_label(modclient: redis.Redis):
-    redis_graph = modclient.graph("g")
+async def test_multi_label(decoded_r: redis.Redis):
+    redis_graph = decoded_r.graph("g")
 
     node = Node(label=["l", "ll"])
     redis_graph.add_node(node)
     await redis_graph.commit()
 
     query = "MATCH (n) RETURN n"
     result = await redis_graph.query(query)
@@ -390,16 +390,16 @@
         Node(label=["l", 1])
         assert False
     except AssertionError:
         assert True
 
 
 @pytest.mark.redismod
-async def test_execution_plan(modclient: redis.Redis):
-    redis_graph = modclient.graph("execution_plan")
+async def test_execution_plan(decoded_r: redis.Redis):
+    redis_graph = decoded_r.graph("execution_plan")
     create_query = """CREATE
     (:Rider {name:'Valentino Rossi'})-[:rides]->(:Team {name:'Yamaha'}),
     (:Rider {name:'Dani Pedrosa'})-[:rides]->(:Team {name:'Honda'}),
     (:Rider {name:'Andrea Dovizioso'})-[:rides]->(:Team {name:'Ducati'})"""
     await redis_graph.query(create_query)
 
     result = await redis_graph.execution_plan(
@@ -409,16 +409,16 @@
     expected = "Results\n    Project\n        Conditional Traverse | (t)->(r:Rider)\n            Filter\n                Node By Label Scan | (t:Team)"  # noqa
     assert result == expected
 
     await redis_graph.delete()
 
 
 @pytest.mark.redismod
-async def test_explain(modclient: redis.Redis):
-    redis_graph = modclient.graph("execution_plan")
+async def test_explain(decoded_r: redis.Redis):
+    redis_graph = decoded_r.graph("execution_plan")
     # graph creation / population
     create_query = """CREATE
 (:Rider {name:'Valentino Rossi'})-[:rides]->(:Team {name:'Yamaha'}),
 (:Rider {name:'Dani Pedrosa'})-[:rides]->(:Team {name:'Honda'}),
 (:Rider {name:'Andrea Dovizioso'})-[:rides]->(:Team {name:'Ducati'})"""
     await redis_graph.query(create_query)
```

### Comparing `redis-5.0.0b4/tests/test_asyncio/test_lock.py` & `redis-5.0.0rc1/tests/test_asyncio/test_lock.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import asyncio
 
 import pytest
 import pytest_asyncio
-
 from redis.asyncio.lock import Lock
 from redis.exceptions import LockError, LockNotOwnedError
 
 
 class TestLock:
     @pytest_asyncio.fixture()
     async def r_decoded(self, create_redis):
```

### Comparing `redis-5.0.0b4/tests/test_asyncio/test_monitor.py` & `redis-5.0.0rc1/tests/test_asyncio/test_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from tests.conftest import skip_if_redis_enterprise, skip_ifnot_redis_enterprise
 
 from .conftest import wait_for_command
 
 
 @pytest.mark.onlynoncluster
 class TestMonitor:
```

### Comparing `redis-5.0.0b4/tests/test_asyncio/test_pipeline.py` & `redis-5.0.0rc1/tests/test_asyncio/test_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 import redis
 from tests.conftest import skip_if_server_version_lt
 
 from .conftest import wait_for_command
 
 
 class TestPipeline:
@@ -17,23 +16,21 @@
         async with r.pipeline() as pipe:
             (
                 pipe.set("a", "a1")
                 .get("a")
                 .zadd("z", {"z1": 1})
                 .zadd("z", {"z2": 4})
                 .zincrby("z", 1, "z1")
-                .zrange("z", 0, 5, withscores=True)
             )
             assert await pipe.execute() == [
                 True,
                 b"a1",
                 True,
                 True,
                 2.0,
-                [(b"z1", 2.0), (b"z2", 4)],
             ]
 
     async def test_pipeline_memoryview(self, r):
         async with r.pipeline() as pipe:
             (pipe.set("a", memoryview(b"a1")).get("a"))
             assert await pipe.execute() == [True, b"a1"]
```

### Comparing `redis-5.0.0b4/tests/test_asyncio/test_pubsub.py` & `redis-5.0.0rc1/tests/test_asyncio/test_pubsub.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,23 +8,21 @@
 if sys.version_info.major >= 3 and sys.version_info.minor >= 11:
     from asyncio import timeout as async_timeout
 else:
     from async_timeout import timeout as async_timeout
 
 import pytest
 import pytest_asyncio
-
 import redis.asyncio as redis
 from redis.exceptions import ConnectionError
 from redis.typing import EncodableT
 from redis.utils import HIREDIS_AVAILABLE
-from tests.conftest import skip_if_server_version_lt
+from tests.conftest import get_protocol_version, skip_if_server_version_lt
 
 from .compat import create_task, mock
-from .conftest import get_protocol_version
 
 
 def with_timeout(t):
     def wrapper(corofunc):
         @functools.wraps(corofunc)
         async def run(*args, **kwargs):
             async with async_timeout(t):
@@ -418,14 +416,15 @@
             await p.get_message()
         expect = (
             "connection not set: did you forget to call subscribe() or psubscribe()?"
         )
         assert expect in info.exconly()
 
 
+@pytest.mark.onlynoncluster
 class TestPubSubRESP3Handler:
     def my_handler(self, message):
         self.message = ["my handler", message]
 
     @pytest.mark.skipif(HIREDIS_AVAILABLE, reason="PythonParser only")
     async def test_push_handler(self, r):
         if get_protocol_version(r) in [2, "2", None]:
```

### Comparing `redis-5.0.0b4/tests/test_asyncio/test_retry.py` & `redis-5.0.0rc1/tests/test_asyncio/test_retry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from redis.asyncio import Redis
 from redis.asyncio.connection import Connection, UnixDomainSocketConnection
 from redis.asyncio.retry import Retry
 from redis.backoff import AbstractBackoff, ExponentialBackoff, NoBackoff
 from redis.exceptions import ConnectionError, TimeoutError
```

### Comparing `redis-5.0.0b4/tests/test_asyncio/test_scripting.py` & `redis-5.0.0rc1/tests/test_asyncio/test_scripting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pytest
 import pytest_asyncio
-
 from redis import exceptions
 from tests.conftest import skip_if_server_version_lt
 
 multiply_script = """
 local value = redis.call('GET', KEYS[1])
 value = tonumber(value)
 return value * ARGV[1]"""
```

### Comparing `redis-5.0.0b4/tests/test_asyncio/test_sentinel.py` & `redis-5.0.0rc1/tests/test_asyncio/test_sentinel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import socket
 
 import pytest
 import pytest_asyncio
-
 import redis.asyncio.sentinel
 from redis import exceptions
 from redis.asyncio.sentinel import (
     MasterNotFoundError,
     Sentinel,
     SentinelConnectionPool,
     SlaveNotFoundError,
```

### Comparing `redis-5.0.0b4/tests/test_asyncio/test_sentinel_managed_connection.py` & `redis-5.0.0rc1/tests/test_asyncio/test_sentinel_managed_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import socket
 
 import pytest
-
 from redis.asyncio.retry import Retry
 from redis.asyncio.sentinel import SentinelManagedConnection
 from redis.backoff import NoBackoff
 
 from .compat import mock
 
 pytestmark = pytest.mark.asyncio
```

### Comparing `redis-5.0.0b4/tests/test_asyncio/testdata/jsontestdata.py` & `redis-5.0.0rc1/tests/test_asyncio/testdata/jsontestdata.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/tests/test_asyncio/testdata/titles.csv` & `redis-5.0.0rc1/tests/test_asyncio/testdata/titles.csv`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/tests/test_asyncio/testdata/will_play_text.csv.bz2` & `redis-5.0.0rc1/tests/test_asyncio/testdata/will_play_text.csv.bz2`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/tests/test_cluster.py` & `redis-5.0.0rc1/tests/test_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import datetime
 import warnings
 from queue import LifoQueue, Queue
 from time import sleep
 from unittest.mock import DEFAULT, Mock, call, patch
 
 import pytest
-
 from redis import Redis
 from redis.backoff import ExponentialBackoff, NoBackoff, default_backoff
 from redis.cluster import (
     PRIMARY,
     REDIS_CLUSTER_HASH_SLOTS,
     REPLICA,
     ClusterNode,
@@ -35,15 +34,15 @@
 from redis.parsers import CommandsParser
 from redis.retry import Retry
 from redis.utils import str_if_bytes
 from tests.test_pubsub import wait_for_message
 
 from .conftest import (
     _get_client,
-    is_resp2_connection,
+    assert_resp_response,
     skip_if_redis_enterprise,
     skip_if_server_version_lt,
     skip_unless_arch_bits,
     wait_for_command,
 )
 
 default_host = "127.0.0.1"
@@ -1721,109 +1720,118 @@
         assert r.smembers("{foo}c") == {b"1", b"2", b"3"}
 
     @skip_if_server_version_lt("6.2.0")
     def test_cluster_zdiff(self, r):
         r.zadd("{foo}a", {"a1": 1, "a2": 2, "a3": 3})
         r.zadd("{foo}b", {"a1": 1, "a2": 2})
         assert r.zdiff(["{foo}a", "{foo}b"]) == [b"a3"]
-        if is_resp2_connection(r):
-            assert r.zdiff(["{foo}a", "{foo}b"], withscores=True) == [b"a3", b"3"]
-        else:
-            assert r.zdiff(["{foo}a", "{foo}b"], withscores=True) == [[b"a3", 3.0]]
+        response = r.zdiff(["{foo}a", "{foo}b"], withscores=True)
+        assert_resp_response(
+            r,
+            response,
+            [b"a3", b"3"],
+            [[b"a3", 3.0]],
+        )
 
     @skip_if_server_version_lt("6.2.0")
     def test_cluster_zdiffstore(self, r):
         r.zadd("{foo}a", {"a1": 1, "a2": 2, "a3": 3})
         r.zadd("{foo}b", {"a1": 1, "a2": 2})
         assert r.zdiffstore("{foo}out", ["{foo}a", "{foo}b"])
         assert r.zrange("{foo}out", 0, -1) == [b"a3"]
-        if is_resp2_connection(r):
-            assert r.zrange("{foo}out", 0, -1, withscores=True) == [(b"a3", 3.0)]
-        else:
-            assert r.zrange("{foo}out", 0, -1, withscores=True) == [[b"a3", 3.0]]
+        response = r.zrange("{foo}out", 0, -1, withscores=True)
+        assert_resp_response(r, response, [(b"a3", 3.0)], [[b"a3", 3.0]])
 
     @skip_if_server_version_lt("6.2.0")
     def test_cluster_zinter(self, r):
         r.zadd("{foo}a", {"a1": 1, "a2": 2, "a3": 1})
         r.zadd("{foo}b", {"a1": 2, "a2": 2, "a3": 2})
         r.zadd("{foo}c", {"a1": 6, "a3": 5, "a4": 4})
         assert r.zinter(["{foo}a", "{foo}b", "{foo}c"]) == [b"a3", b"a1"]
         # invalid aggregation
         with pytest.raises(DataError):
             r.zinter(["{foo}a", "{foo}b", "{foo}c"], aggregate="foo", withscores=True)
-        if is_resp2_connection(r):
-            # aggregate with SUM
-            assert r.zinter(["{foo}a", "{foo}b", "{foo}c"], withscores=True) == [
-                (b"a3", 8),
-                (b"a1", 9),
-            ]
-            # aggregate with MAX
-            assert r.zinter(
-                ["{foo}a", "{foo}b", "{foo}c"], aggregate="MAX", withscores=True
-            ) == [(b"a3", 5), (b"a1", 6)]
-            # aggregate with MIN
-            assert r.zinter(
-                ["{foo}a", "{foo}b", "{foo}c"], aggregate="MIN", withscores=True
-            ) == [(b"a1", 1), (b"a3", 1)]
-            # with weights
-            assert r.zinter(
-                {"{foo}a": 1, "{foo}b": 2, "{foo}c": 3}, withscores=True
-            ) == [(b"a3", 20), (b"a1", 23)]
-        else:
-            # aggregate with SUM
-            assert r.zinter(["{foo}a", "{foo}b", "{foo}c"], withscores=True) == [
-                [b"a3", 8],
-                [b"a1", 9],
-            ]
-            # aggregate with MAX
-            assert r.zinter(
-                ["{foo}a", "{foo}b", "{foo}c"], aggregate="MAX", withscores=True
-            ) == [[b"a3", 5], [b"a1", 6]]
-            # aggregate with MIN
-            assert r.zinter(
-                ["{foo}a", "{foo}b", "{foo}c"], aggregate="MIN", withscores=True
-            ) == [[b"a1", 1], [b"a3", 1]]
-            # with weights
-            assert r.zinter(
-                {"{foo}a": 1, "{foo}b": 2, "{foo}c": 3}, withscores=True
-            ) == [[b"a3", 2], [b"a1", 2]]
+        assert_resp_response(
+            r,
+            r.zinter(["{foo}a", "{foo}b", "{foo}c"], withscores=True),
+            [(b"a3", 8), (b"a1", 9)],
+            [[b"a3", 8], [b"a1", 9]],
+        )
+        assert_resp_response(
+            r,
+            r.zinter(["{foo}a", "{foo}b", "{foo}c"], withscores=True, aggregate="MAX"),
+            [(b"a3", 5), (b"a1", 6)],
+            [[b"a3", 5], [b"a1", 6]],
+        )
+        assert_resp_response(
+            r,
+            r.zinter(["{foo}a", "{foo}b", "{foo}c"], withscores=True, aggregate="MIN"),
+            [(b"a1", 1), (b"a3", 1)],
+            [[b"a1", 1], [b"a3", 1]],
+        )
+        assert_resp_response(
+            r,
+            r.zinter({"{foo}a": 1, "{foo}b": 2, "{foo}c": 3}, withscores=True),
+            [(b"a3", 20.0), (b"a1", 23.0)],
+            [[b"a3", 20.0], [b"a1", 23.0]],
+        )
 
     def test_cluster_zinterstore_sum(self, r):
         r.zadd("{foo}a", {"a1": 1, "a2": 1, "a3": 1})
         r.zadd("{foo}b", {"a1": 2, "a2": 2, "a3": 2})
         r.zadd("{foo}c", {"a1": 6, "a3": 5, "a4": 4})
         assert r.zinterstore("{foo}d", ["{foo}a", "{foo}b", "{foo}c"]) == 2
-        assert r.zrange("{foo}d", 0, -1, withscores=True) == [(b"a3", 8), (b"a1", 9)]
+        assert_resp_response(
+            r,
+            r.zrange("{foo}d", 0, -1, withscores=True),
+            [(b"a3", 8), (b"a1", 9)],
+            [[b"a3", 8.0], [b"a1", 9.0]],
+        )
 
     def test_cluster_zinterstore_max(self, r):
         r.zadd("{foo}a", {"a1": 1, "a2": 1, "a3": 1})
         r.zadd("{foo}b", {"a1": 2, "a2": 2, "a3": 2})
         r.zadd("{foo}c", {"a1": 6, "a3": 5, "a4": 4})
         assert (
             r.zinterstore("{foo}d", ["{foo}a", "{foo}b", "{foo}c"], aggregate="MAX")
             == 2
         )
-        assert r.zrange("{foo}d", 0, -1, withscores=True) == [(b"a3", 5), (b"a1", 6)]
+        assert_resp_response(
+            r,
+            r.zrange("{foo}d", 0, -1, withscores=True),
+            [(b"a3", 5), (b"a1", 6)],
+            [[b"a3", 5.0], [b"a1", 6.0]],
+        )
 
     def test_cluster_zinterstore_min(self, r):
         r.zadd("{foo}a", {"a1": 1, "a2": 2, "a3": 3})
         r.zadd("{foo}b", {"a1": 2, "a2": 3, "a3": 5})
         r.zadd("{foo}c", {"a1": 6, "a3": 5, "a4": 4})
         assert (
             r.zinterstore("{foo}d", ["{foo}a", "{foo}b", "{foo}c"], aggregate="MIN")
             == 2
         )
-        assert r.zrange("{foo}d", 0, -1, withscores=True) == [(b"a1", 1), (b"a3", 3)]
+        assert_resp_response(
+            r,
+            r.zrange("{foo}d", 0, -1, withscores=True),
+            [(b"a1", 1), (b"a3", 3)],
+            [[b"a1", 1.0], [b"a3", 3.0]],
+        )
 
     def test_cluster_zinterstore_with_weight(self, r):
         r.zadd("{foo}a", {"a1": 1, "a2": 1, "a3": 1})
         r.zadd("{foo}b", {"a1": 2, "a2": 2, "a3": 2})
         r.zadd("{foo}c", {"a1": 6, "a3": 5, "a4": 4})
         assert r.zinterstore("{foo}d", {"{foo}a": 1, "{foo}b": 2, "{foo}c": 3}) == 2
-        assert r.zrange("{foo}d", 0, -1, withscores=True) == [(b"a3", 20), (b"a1", 23)]
+        assert_resp_response(
+            r,
+            r.zrange("{foo}d", 0, -1, withscores=True),
+            [(b"a3", 20), (b"a1", 23)],
+            [[b"a3", 20.0], [b"a1", 23.0]],
+        )
 
     @skip_if_server_version_lt("4.9.0")
     def test_cluster_bzpopmax(self, r):
         r.zadd("{foo}a", {"a1": 1, "a2": 2})
         r.zadd("{foo}b", {"b1": 10, "b2": 20})
         assert r.bzpopmax(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}b", b"b2", 20)
         assert r.bzpopmax(["{foo}b", "{foo}a"], timeout=1) == (b"{foo}b", b"b1", 10)
@@ -1848,15 +1856,20 @@
     @skip_if_server_version_lt("6.2.0")
     def test_cluster_zrangestore(self, r):
         r.zadd("{foo}a", {"a1": 1, "a2": 2, "a3": 3})
         assert r.zrangestore("{foo}b", "{foo}a", 0, 1)
         assert r.zrange("{foo}b", 0, -1) == [b"a1", b"a2"]
         assert r.zrangestore("{foo}b", "{foo}a", 1, 2)
         assert r.zrange("{foo}b", 0, -1) == [b"a2", b"a3"]
-        assert r.zrange("{foo}b", 0, -1, withscores=True) == [(b"a2", 2), (b"a3", 3)]
+        assert_resp_response(
+            r,
+            r.zrange("{foo}b", 0, 1, withscores=True),
+            [(b"a2", 2), (b"a3", 3)],
+            [[b"a2", 2.0], [b"a3", 3.0]],
+        )
         # reversed order
         assert r.zrangestore("{foo}b", "{foo}a", 1, 2, desc=True)
         assert r.zrange("{foo}b", 0, -1) == [b"a1", b"a2"]
         # by score
         assert r.zrangestore(
             "{foo}b", "{foo}a", 2, 1, byscore=True, offset=0, num=1, desc=True
         )
@@ -1870,89 +1883,95 @@
     @skip_if_server_version_lt("6.2.0")
     def test_cluster_zunion(self, r):
         r.zadd("{foo}a", {"a1": 1, "a2": 1, "a3": 1})
         r.zadd("{foo}b", {"a1": 2, "a2": 2, "a3": 2})
         r.zadd("{foo}c", {"a1": 6, "a3": 5, "a4": 4})
         # sum
         assert r.zunion(["{foo}a", "{foo}b", "{foo}c"]) == [b"a2", b"a4", b"a3", b"a1"]
-        assert r.zunion(["{foo}a", "{foo}b", "{foo}c"], withscores=True) == [
-            (b"a2", 3),
-            (b"a4", 4),
-            (b"a3", 8),
-            (b"a1", 9),
-        ]
+        assert_resp_response(
+            r,
+            r.zunion(["{foo}a", "{foo}b", "{foo}c"], withscores=True),
+            [(b"a2", 3), (b"a4", 4), (b"a3", 8), (b"a1", 9)],
+            [[b"a2", 3.0], [b"a4", 4.0], [b"a3", 8.0], [b"a1", 9.0]],
+        )
         # max
-        assert r.zunion(
-            ["{foo}a", "{foo}b", "{foo}c"], aggregate="MAX", withscores=True
-        ) == [(b"a2", 2), (b"a4", 4), (b"a3", 5), (b"a1", 6)]
+        assert_resp_response(
+            r,
+            r.zunion(["{foo}a", "{foo}b", "{foo}c"], aggregate="MAX", withscores=True),
+            [(b"a2", 2), (b"a4", 4), (b"a3", 5), (b"a1", 6)],
+            [[b"a2", 2.0], [b"a4", 4.0], [b"a3", 5.0], [b"a1", 6.0]],
+        )
         # min
-        assert r.zunion(
-            ["{foo}a", "{foo}b", "{foo}c"], aggregate="MIN", withscores=True
-        ) == [(b"a1", 1), (b"a2", 1), (b"a3", 1), (b"a4", 4)]
+        assert_resp_response(
+            r,
+            r.zunion(["{foo}a", "{foo}b", "{foo}c"], aggregate="MIN", withscores=True),
+            [(b"a1", 1), (b"a2", 1), (b"a3", 1), (b"a4", 4)],
+            [[b"a1", 1.0], [b"a2", 1.0], [b"a3", 1.0], [b"a4", 4.0]],
+        )
         # with weight
-        assert r.zunion({"{foo}a": 1, "{foo}b": 2, "{foo}c": 3}, withscores=True) == [
-            (b"a2", 5),
-            (b"a4", 12),
-            (b"a3", 20),
-            (b"a1", 23),
-        ]
+        assert_resp_response(
+            r,
+            r.zunion({"{foo}a": 1, "{foo}b": 2, "{foo}c": 3}, withscores=True),
+            [(b"a2", 5), (b"a4", 12), (b"a3", 20), (b"a1", 23)],
+            [[b"a2", 5.0], [b"a4", 12.0], [b"a3", 20.0], [b"a1", 23.0]],
+        )
 
     def test_cluster_zunionstore_sum(self, r):
         r.zadd("{foo}a", {"a1": 1, "a2": 1, "a3": 1})
         r.zadd("{foo}b", {"a1": 2, "a2": 2, "a3": 2})
         r.zadd("{foo}c", {"a1": 6, "a3": 5, "a4": 4})
         assert r.zunionstore("{foo}d", ["{foo}a", "{foo}b", "{foo}c"]) == 4
-        assert r.zrange("{foo}d", 0, -1, withscores=True) == [
-            (b"a2", 3),
-            (b"a4", 4),
-            (b"a3", 8),
-            (b"a1", 9),
-        ]
+        assert_resp_response(
+            r,
+            r.zrange("{foo}d", 0, -1, withscores=True),
+            [(b"a2", 3), (b"a4", 4), (b"a3", 8), (b"a1", 9)],
+            [[b"a2", 3.0], [b"a4", 4.0], [b"a3", 8.0], [b"a1", 9.0]],
+        )
 
     def test_cluster_zunionstore_max(self, r):
         r.zadd("{foo}a", {"a1": 1, "a2": 1, "a3": 1})
         r.zadd("{foo}b", {"a1": 2, "a2": 2, "a3": 2})
         r.zadd("{foo}c", {"a1": 6, "a3": 5, "a4": 4})
         assert (
             r.zunionstore("{foo}d", ["{foo}a", "{foo}b", "{foo}c"], aggregate="MAX")
             == 4
         )
-        assert r.zrange("{foo}d", 0, -1, withscores=True) == [
-            (b"a2", 2),
-            (b"a4", 4),
-            (b"a3", 5),
-            (b"a1", 6),
-        ]
+        assert_resp_response(
+            r,
+            r.zrange("{foo}d", 0, -1, withscores=True),
+            [(b"a2", 2), (b"a4", 4), (b"a3", 5), (b"a1", 6)],
+            [[b"a2", 2.0], [b"a4", 4.0], [b"a3", 5.0], [b"a1", 6.0]],
+        )
 
     def test_cluster_zunionstore_min(self, r):
         r.zadd("{foo}a", {"a1": 1, "a2": 2, "a3": 3})
         r.zadd("{foo}b", {"a1": 2, "a2": 2, "a3": 4})
         r.zadd("{foo}c", {"a1": 6, "a3": 5, "a4": 4})
         assert (
             r.zunionstore("{foo}d", ["{foo}a", "{foo}b", "{foo}c"], aggregate="MIN")
             == 4
         )
-        assert r.zrange("{foo}d", 0, -1, withscores=True) == [
-            (b"a1", 1),
-            (b"a2", 2),
-            (b"a3", 3),
-            (b"a4", 4),
-        ]
+        assert_resp_response(
+            r,
+            r.zrange("{foo}d", 0, -1, withscores=True),
+            [(b"a1", 1), (b"a2", 2), (b"a3", 3), (b"a4", 4)],
+            [[b"a1", 1.0], [b"a2", 2.0], [b"a3", 3.0], [b"a4", 4.0]],
+        )
 
     def test_cluster_zunionstore_with_weight(self, r):
         r.zadd("{foo}a", {"a1": 1, "a2": 1, "a3": 1})
         r.zadd("{foo}b", {"a1": 2, "a2": 2, "a3": 2})
         r.zadd("{foo}c", {"a1": 6, "a3": 5, "a4": 4})
         assert r.zunionstore("{foo}d", {"{foo}a": 1, "{foo}b": 2, "{foo}c": 3}) == 4
-        assert r.zrange("{foo}d", 0, -1, withscores=True) == [
-            (b"a2", 5),
-            (b"a4", 12),
-            (b"a3", 20),
-            (b"a1", 23),
-        ]
+        assert_resp_response(
+            r,
+            r.zrange("{foo}d", 0, -1, withscores=True),
+            [(b"a2", 5), (b"a4", 12), (b"a3", 20), (b"a1", 23)],
+            [[b"a2", 5.0], [b"a4", 12.0], [b"a3", 20.0], [b"a1", 23.0]],
+        )
 
     @skip_if_server_version_lt("2.8.9")
     def test_cluster_pfcount(self, r):
         members = {b"1", b"2", b"3"}
         r.pfadd("{foo}a", *members)
         assert r.pfcount("{foo}a") == len(members)
         members_b = {b"2", b"3", b"4"}
@@ -2966,15 +2985,20 @@
         r.readonly(target_nodes="all")
         r.set("foo71", "a1")  # we assume this key is set on 127.0.0.1:7001
         r.zadd("foo88", {"z1": 1})  # we assume this key is set on 127.0.0.1:7002
         r.zadd("foo88", {"z2": 4})
 
         with r.pipeline() as readonly_pipe:
             readonly_pipe.get("foo71").zrange("foo88", 0, 5, withscores=True)
-            assert readonly_pipe.execute() == [b"a1", [(b"z1", 1.0), (b"z2", 4)]]
+            assert_resp_response(
+                r,
+                readonly_pipe.execute(),
+                [b"a1", [(b"z1", 1.0), (b"z2", 4)]],
+                [b"a1", [[b"z1", 1.0], [b"z2", 4.0]]],
+            )
 
     def test_moved_redirection_on_slave_with_default(self, r):
         """
         On Pipeline, we redirected once and finally get from master with
         readonly client when data is completely moved.
         """
         key = "bar"
```

### Comparing `redis-5.0.0b4/tests/test_command_parser.py` & `redis-5.0.0rc1/tests/test_command_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from redis.parsers import CommandsParser
 
 from .conftest import skip_if_redis_enterprise, skip_if_server_version_lt
 
 
 class TestCommandsParser:
     def test_init_commands(self, r):
```

### Comparing `redis-5.0.0b4/tests/test_commands.py` & `redis-5.0.0rc1/tests/test_commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 import datetime
 import re
 import time
 from string import ascii_letters
 from unittest import mock
 
 import pytest
-
 import redis
 from redis import exceptions
 from redis.client import EMPTY_RESPONSE, NEVER_DECODE, parse_info
 
 from .conftest import (
     _get_client,
+    assert_resp_response,
+    assert_resp_response_in,
     is_resp2_connection,
     skip_if_redis_enterprise,
     skip_if_server_version_gte,
     skip_if_server_version_lt,
     skip_unless_arch_bits,
 )
 
@@ -52,25 +53,31 @@
 
 # RESPONSE CALLBACKS
 @pytest.mark.onlynoncluster
 class TestResponseCallbacks:
     "Tests for the response callback system"
 
     def test_response_callbacks(self, r):
-        assert r.response_callbacks == redis.Redis.RESPONSE_CALLBACKS
+        callbacks = redis.Redis.RESPONSE_CALLBACKS
+        if is_resp2_connection(r):
+            callbacks.update(redis.Redis.RESP2_RESPONSE_CALLBACKS)
+        else:
+            callbacks.update(redis.Redis.RESP3_RESPONSE_CALLBACKS)
+        assert r.response_callbacks == callbacks
         assert id(r.response_callbacks) != id(redis.Redis.RESPONSE_CALLBACKS)
         r.set_response_callback("GET", lambda x: "static")
         r["a"] = "foo"
         assert r["a"] == "static"
 
     def test_case_insensitive_command_names(self, r):
-        assert r.response_callbacks["del"] == r.response_callbacks["DEL"]
+        assert r.response_callbacks["ping"] == r.response_callbacks["PING"]
 
 
 class TestRedisCommands:
+    @pytest.mark.onlynoncluster
     @skip_if_redis_enterprise()
     def test_auth(self, r, request):
         # sending an AUTH command before setting a user/password on the
         # server should return an AuthenticationError
         with pytest.raises(exceptions.AuthenticationError):
             r.auth("some_password")
 
@@ -97,15 +104,14 @@
                 # setting the password on the connection itself triggers the
                 # authentication in the connection's `on_connect` method
                 r.connection.password = temp_pass
             except AttributeError:
                 # connection field is not set in Redis Cluster, but that's ok
                 # because the problem discussed above does not apply to Redis Cluster
                 pass
-
             r.auth(temp_pass)
             r.config_set("requirepass", "")
             r.acl_deluser(username)
 
         request.addfinalizer(teardown)
 
         assert r.acl_setuser(
@@ -143,17 +149,16 @@
         def teardown():
             r.acl_deluser(username)
 
         request.addfinalizer(teardown)
 
         r.acl_setuser(username, keys=["*"], commands=["+set"])
         assert r.acl_dryrun(username, "set", "key", "value") == b"OK"
-        assert r.acl_dryrun(username, "get", "key").startswith(
-            b"This user has no permissions to run the"
-        )
+        no_permissions_message = b"user has no permissions to run the"
+        assert no_permissions_message in r.acl_dryrun(username, "get", "key")
 
     @skip_if_server_version_lt("6.0.0")
     @skip_if_redis_enterprise()
     def test_acl_deluser(self, r, request):
         username = "redis-py-user"
 
         def teardown():
@@ -189,14 +194,15 @@
 
         r.acl_genpass(555)
         assert isinstance(password, str)
 
     @skip_if_server_version_lt("7.0.0")
     @skip_if_redis_enterprise()
     def test_acl_getuser_setuser(self, r, request):
+        r.flushall()
         username = "redis-py-user"
 
         def teardown():
             r.acl_deluser(username)
 
         request.addfinalizer(teardown)
 
@@ -223,27 +229,27 @@
 
         # test all args
         assert r.acl_setuser(
             username,
             enabled=True,
             reset=True,
             passwords=["+pass1", "+pass2"],
-            categories=["+set", "+@hash", "-geo"],
+            categories=["+set", "+@hash", "-@geo"],
             commands=["+get", "+mget", "-hset"],
             keys=["cache:*", "objects:*"],
         )
         acl = r.acl_getuser(username)
-        assert set(acl["categories"]) == {"-@all", "+@set", "+@hash"}
+        assert set(acl["categories"]) == {"+@hash", "+@set", "-@all", "-@geo"}
         assert set(acl["commands"]) == {"+get", "+mget", "-hset"}
         assert acl["enabled"] is True
         assert "on" in acl["flags"]
         assert set(acl["keys"]) == {"~cache:*", "~objects:*"}
         assert len(acl["passwords"]) == 2
 
-        # test reset=False keeps existing ACL and applies new ACL on top
+        # # test reset=False keeps existing ACL and applies new ACL on top
         assert r.acl_setuser(
             username,
             enabled=True,
             reset=True,
             passwords=["+pass1"],
             categories=["+@set"],
             commands=["+get"],
@@ -254,30 +260,29 @@
             enabled=True,
             passwords=["+pass2"],
             categories=["+@hash"],
             commands=["+mget"],
             keys=["objects:*"],
         )
         acl = r.acl_getuser(username)
-        assert set(acl["categories"]) == {"-@all", "+@set", "+@hash"}
         assert set(acl["commands"]) == {"+get", "+mget"}
         assert acl["enabled"] is True
         assert "on" in acl["flags"]
         assert set(acl["keys"]) == {"~cache:*", "~objects:*"}
         assert len(acl["passwords"]) == 2
 
-        # test removal of passwords
+        # # test removal of passwords
         assert r.acl_setuser(
             username, enabled=True, reset=True, passwords=["+pass1", "+pass2"]
         )
         assert len(r.acl_getuser(username)["passwords"]) == 2
         assert r.acl_setuser(username, enabled=True, passwords=["-pass2"])
         assert len(r.acl_getuser(username)["passwords"]) == 1
 
-        # Resets and tests that hashed passwords are set properly.
+        # # Resets and tests that hashed passwords are set properly.
         hashed_password = (
             "5e884898da28047151d0e56f8dc6292773603d0d6aabbdd62a11ef721d1542d8"
         )
         assert r.acl_setuser(
             username, enabled=True, reset=True, hashed_passwords=["+" + hashed_password]
         )
         acl = r.acl_getuser(username)
@@ -293,57 +298,61 @@
         )
         assert len(r.acl_getuser(username)["passwords"]) == 2
         assert r.acl_setuser(
             username, enabled=True, hashed_passwords=["-" + hashed_password]
         )
         assert len(r.acl_getuser(username)["passwords"]) == 1
 
-        # test selectors
+        # # test selectors
         assert r.acl_setuser(
             username,
             enabled=True,
             reset=True,
             passwords=["+pass1", "+pass2"],
             categories=["+set", "+@hash", "-geo"],
             commands=["+get", "+mget", "-hset"],
             keys=["cache:*", "objects:*"],
             channels=["message:*"],
             selectors=[("+set", "%W~app*")],
         )
         acl = r.acl_getuser(username)
-        assert set(acl["categories"]) == {"-@all", "+@set", "+@hash"}
+        assert set(acl["categories"]) == {"+@hash", "+@set", "-@all", "-@geo"}
         assert set(acl["commands"]) == {"+get", "+mget", "-hset"}
         assert acl["enabled"] is True
         assert "on" in acl["flags"]
         assert set(acl["keys"]) == {"~cache:*", "~objects:*"}
         assert len(acl["passwords"]) == 2
         assert set(acl["channels"]) == {"&message:*"}
-        assert acl["selectors"] == [
-            ["commands", "-@all +set", "keys", "%W~app*", "channels", ""]
-        ]
+        assert_resp_response(
+            r,
+            acl["selectors"],
+            [["commands", "-@all +set", "keys", "%W~app*", "channels", ""]],
+            [{"commands": "-@all +set", "keys": "%W~app*", "channels": ""}],
+        )
 
     @skip_if_server_version_lt("6.0.0")
     def test_acl_help(self, r):
         res = r.acl_help()
         assert isinstance(res, list)
         assert len(res) != 0
 
     @skip_if_server_version_lt("6.0.0")
     @skip_if_redis_enterprise()
     def test_acl_list(self, r, request):
         username = "redis-py-user"
+        start = r.acl_list()
 
         def teardown():
             r.acl_deluser(username)
 
         request.addfinalizer(teardown)
 
         assert r.acl_setuser(username, enabled=False, reset=True)
         users = r.acl_list()
-        assert len(users) == 2
+        assert len(users) == len(start) + 1
 
     @skip_if_server_version_lt("6.0.0")
     @skip_if_redis_enterprise()
     @pytest.mark.onlynoncluster
     def test_acl_log(self, r, request):
         username = "redis-py-user"
 
@@ -377,19 +386,21 @@
         with pytest.raises(exceptions.NoPermissionError):
             user_client.hset("cache:0", "hkey", "hval")
 
         assert isinstance(r.acl_log(), list)
         assert len(r.acl_log()) == 2
         assert len(r.acl_log(count=1)) == 1
         assert isinstance(r.acl_log()[0], dict)
-        if is_resp2_connection(r):
-            assert "client-info" in r.acl_log(count=1)[0]
-        else:
-            assert "client-info" in r.acl_log(count=1)[0].keys()
-        assert r.acl_log_reset()
+        expected = r.acl_log(count=1)[0]
+        assert_resp_response_in(
+            r,
+            "client-info",
+            expected,
+            expected.keys(),
+        )
 
     @skip_if_server_version_lt("6.0.0")
     @skip_if_redis_enterprise()
     def test_acl_setuser_categories_without_prefix_fails(self, r, request):
         username = "redis-py-user"
 
         def teardown():
@@ -697,15 +708,15 @@
         with pytest.raises(TypeError):
             r.client_no_evict()
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("3.2.0")
     def test_client_reply(self, r, r_timeout):
         assert r_timeout.client_reply("ON") == b"OK"
-        with pytest.raises(exceptions.TimeoutError):
+        with pytest.raises(exceptions.RedisError):
             r_timeout.client_reply("OFF")
 
             r_timeout.client_reply("SKIP")
 
         assert r_timeout.set("foo", "bar")
 
         # validate it was set
@@ -1120,16 +1131,20 @@
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("7.0.0")
     def test_lcs(self, r):
         r.mset({"foo": "ohmytext", "bar": "mynewtext"})
         assert r.lcs("foo", "bar") == b"mytext"
         assert r.lcs("foo", "bar", len=True) == 6
-        result = [b"matches", [[[4, 7], [5, 8]]], b"len", 6]
-        assert r.lcs("foo", "bar", idx=True, minmatchlen=3) == result
+        assert_resp_response(
+            r,
+            r.lcs("foo", "bar", idx=True, minmatchlen=3),
+            [b"matches", [[[4, 7], [5, 8]]], b"len", 6],
+            {b"matches": [[[4, 7], [5, 8]]], b"len": 6},
+        )
         with pytest.raises(redis.ResponseError):
             assert r.lcs("foo", "bar", len=True, idx=True)
 
     @skip_if_server_version_lt("2.6.0")
     def test_dump_and_restore(self, r):
         r["a"] = "foo"
         dumped = r.dump("a")
@@ -1535,18 +1550,15 @@
     @skip_if_server_version_lt("6.2.0")
     def test_hrandfield(self, r):
         assert r.hrandfield("key") is None
         r.hset("key", mapping={"a": 1, "b": 2, "c": 3, "d": 4, "e": 5})
         assert r.hrandfield("key") is not None
         assert len(r.hrandfield("key", 2)) == 2
         # with values
-        if is_resp2_connection(r):
-            assert len(r.hrandfield("key", 2, True)) == 4
-        else:
-            assert len(r.hrandfield("key", 2, True)) == 2
+        assert_resp_response(r, len(r.hrandfield("key", 2, withvalues=True)), 4, 2)
         # without duplications
         assert len(r.hrandfield("key", 10)) == 5
         # with duplications
         assert len(r.hrandfield("key", -10)) == 10
 
     @pytest.mark.onlynoncluster
     def test_randomkey(self, r):
@@ -1691,38 +1703,34 @@
         # test LCS of strings
         assert r.stralgo("LCS", value1, value2) == res
         # test using keys
         r.mset({key1: value1, key2: value2})
         assert r.stralgo("LCS", key1, key2, specific_argument="keys") == res
         # test other labels
         assert r.stralgo("LCS", value1, value2, len=True) == len(res)
-        if is_resp2_connection(r):
-            assert r.stralgo("LCS", value1, value2, idx=True) == {
-                "len": len(res),
-                "matches": [[(4, 7), (5, 8)], [(2, 3), (0, 1)]],
-            }
-            assert r.stralgo("LCS", value1, value2, idx=True, withmatchlen=True) == {
-                "len": len(res),
-                "matches": [[4, (4, 7), (5, 8)], [2, (2, 3), (0, 1)]],
-            }
-            assert r.stralgo(
-                "LCS", value1, value2, idx=True, minmatchlen=4, withmatchlen=True
-            ) == {"len": len(res), "matches": [[4, (4, 7), (5, 8)]]}
-        else:
-            assert r.stralgo("LCS", value1, value2, idx=True) == {
-                "len": len(res),
-                "matches": [[[4, 7], [5, 8]], [[2, 3], [0, 1]]],
-            }
-            assert r.stralgo("LCS", value1, value2, idx=True, withmatchlen=True) == {
-                "len": len(res),
-                "matches": [[[4, 7], [5, 8], 4], [[2, 3], [0, 1], 2]],
-            }
-            assert r.stralgo(
-                "LCS", value1, value2, idx=True, minmatchlen=4, withmatchlen=True
-            ) == {"len": len(res), "matches": [[[4, 7], [5, 8], 4]]}
+        assert_resp_response(
+            r,
+            r.stralgo("LCS", value1, value2, idx=True),
+            {"len": len(res), "matches": [[(4, 7), (5, 8)], [(2, 3), (0, 1)]]},
+            {"len": len(res), "matches": [[[4, 7], [5, 8]], [[2, 3], [0, 1]]]},
+        )
+        assert_resp_response(
+            r,
+            r.stralgo("LCS", value1, value2, idx=True, withmatchlen=True),
+            {"len": len(res), "matches": [[4, (4, 7), (5, 8)], [2, (2, 3), (0, 1)]]},
+            {"len": len(res), "matches": [[[4, 7], [5, 8], 4], [[2, 3], [0, 1], 2]]},
+        )
+        assert_resp_response(
+            r,
+            r.stralgo(
+                "LCS", value1, value2, idx=True, withmatchlen=True, minmatchlen=4
+            ),
+            {"len": len(res), "matches": [[4, (4, 7), (5, 8)]]},
+            {"len": len(res), "matches": [[[4, 7], [5, 8], 4]]},
+        )
 
     @skip_if_server_version_lt("6.0.0")
     @skip_if_server_version_gte("7.0.0")
     @skip_if_redis_enterprise()
     def test_stralgo_negative(self, r):
         with pytest.raises(exceptions.DataError):
             r.stralgo("ISSUB", "value1", "value2")
@@ -2163,18 +2171,20 @@
         s = [b"1", b"2", b"3"]
         r.sadd("a", *s)
         values = r.spop("a", 2)
         assert len(values) == 2
 
         for value in values:
             assert value in s
-        if is_resp2_connection(r):
-            assert r.spop("a", 1) == list(set(s) - set(values))
-        else:
-            assert r.spop("a", 1) == set(s) - set(values)
+        assert_resp_response(
+            r,
+            r.spop("a", 1),
+            list(set(s) - set(values)),
+            set(s) - set(values),
+        )
 
     def test_srandmember(self, r):
         s = [b"1", b"2", b"3"]
         r.sadd("a", *s)
         assert r.srandmember("a") in s
 
     @skip_if_server_version_lt("2.6.0")
@@ -2217,26 +2227,20 @@
         with pytest.raises(NotImplementedError):
             r.script_debug()
 
     # SORTED SET COMMANDS
     def test_zadd(self, r):
         mapping = {"a1": 1.0, "a2": 2.0, "a3": 3.0}
         r.zadd("a", mapping)
-        if is_resp2_connection(r):
-            assert r.zrange("a", 0, -1, withscores=True) == [
-                (b"a1", 1.0),
-                (b"a2", 2.0),
-                (b"a3", 3.0),
-            ]
-        else:
-            assert r.zrange("a", 0, -1, withscores=True) == [
-                [b"a1", 1.0],
-                [b"a2", 2.0],
-                [b"a3", 3.0],
-            ]
+        assert_resp_response(
+            r,
+            r.zrange("a", 0, -1, withscores=True),
+            [(b"a1", 1.0), (b"a2", 2.0), (b"a3", 3.0)],
+            [[b"a1", 1.0], [b"a2", 2.0], [b"a3", 3.0]],
+        )
 
         # error cases
         with pytest.raises(exceptions.DataError):
             r.zadd("a", {})
 
         # cannot use both nx and xx options
         with pytest.raises(exceptions.DataError):
@@ -2245,40 +2249,40 @@
         # cannot use the incr options with more than one value
         with pytest.raises(exceptions.DataError):
             r.zadd("a", mapping, incr=True)
 
     def test_zadd_nx(self, r):
         assert r.zadd("a", {"a1": 1}) == 1
         assert r.zadd("a", {"a1": 99, "a2": 2}, nx=True) == 1
-        if is_resp2_connection(r):
-            assert r.zrange("a", 0, -1, withscores=True) == [(b"a1", 1.0), (b"a2", 2.0)]
-        else:
-            assert r.zrange("a", 0, -1, withscores=True) == [[b"a1", 1.0], [b"a2", 2.0]]
+        assert_resp_response(
+            r,
+            r.zrange("a", 0, -1, withscores=True),
+            [(b"a1", 1.0), (b"a2", 2.0)],
+            [[b"a1", 1.0], [b"a2", 2.0]],
+        )
 
     def test_zadd_xx(self, r):
         assert r.zadd("a", {"a1": 1}) == 1
         assert r.zadd("a", {"a1": 99, "a2": 2}, xx=True) == 0
-        if is_resp2_connection(r):
-            assert r.zrange("a", 0, -1, withscores=True) == [(b"a1", 99.0)]
-        else:
-            assert r.zrange("a", 0, -1, withscores=True) == [[b"a1", 99.0]]
+        assert_resp_response(
+            r,
+            r.zrange("a", 0, -1, withscores=True),
+            [(b"a1", 99.0)],
+            [[b"a1", 99.0]],
+        )
 
     def test_zadd_ch(self, r):
         assert r.zadd("a", {"a1": 1}) == 1
         assert r.zadd("a", {"a1": 99, "a2": 2}, ch=True) == 2
-        if is_resp2_connection(r):
-            assert r.zrange("a", 0, -1, withscores=True) == [
-                (b"a2", 2.0),
-                (b"a1", 99.0),
-            ]
-        else:
-            assert r.zrange("a", 0, -1, withscores=True) == [
-                [b"a2", 2.0],
-                [b"a1", 99.0],
-            ]
+        assert_resp_response(
+            r,
+            r.zrange("a", 0, -1, withscores=True),
+            [(b"a2", 2.0), (b"a1", 99.0)],
+            [[b"a2", 2.0], [b"a1", 99.0]],
+        )
 
     def test_zadd_incr(self, r):
         assert r.zadd("a", {"a1": 1}) == 1
         assert r.zadd("a", {"a1": 4.5}, incr=True) == 5.5
 
     def test_zadd_incr_with_xx(self, r):
         # this asks zadd to incr 'a1' only if it exists, but it clearly
@@ -2318,30 +2322,34 @@
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("6.2.0")
     def test_zdiff(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3})
         r.zadd("b", {"a1": 1, "a2": 2})
         assert r.zdiff(["a", "b"]) == [b"a3"]
-        if is_resp2_connection(r):
-            assert r.zdiff(["a", "b"], withscores=True) == [b"a3", b"3"]
-        else:
-            assert r.zdiff(["a", "b"], withscores=True) == [[b"a3", 3.0]]
+        assert_resp_response(
+            r,
+            r.zdiff(["a", "b"], withscores=True),
+            [b"a3", b"3"],
+            [[b"a3", 3.0]],
+        )
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("6.2.0")
     def test_zdiffstore(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3})
         r.zadd("b", {"a1": 1, "a2": 2})
         assert r.zdiffstore("out", ["a", "b"])
         assert r.zrange("out", 0, -1) == [b"a3"]
-        if is_resp2_connection(r):
-            assert r.zrange("out", 0, -1, withscores=True) == [(b"a3", 3.0)]
-        else:
-            assert r.zrange("out", 0, -1, withscores=True) == [[b"a3", 3.0]]
+        assert_resp_response(
+            r,
+            r.zrange("out", 0, -1, withscores=True),
+            [(b"a3", 3.0)],
+            [[b"a3", 3.0]],
+        )
 
     def test_zincrby(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3})
         assert r.zincrby("a", 1, "a2") == 3.0
         assert r.zincrby("a", 5, "a3") == 8.0
         assert r.zscore("a", "a2") == 3.0
         assert r.zscore("a", "a3") == 8.0
@@ -2358,56 +2366,42 @@
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 1})
         r.zadd("b", {"a1": 2, "a2": 2, "a3": 2})
         r.zadd("c", {"a1": 6, "a3": 5, "a4": 4})
         assert r.zinter(["a", "b", "c"]) == [b"a3", b"a1"]
         # invalid aggregation
         with pytest.raises(exceptions.DataError):
             r.zinter(["a", "b", "c"], aggregate="foo", withscores=True)
-        if is_resp2_connection(r):
-            # aggregate with SUM
-            assert r.zinter(["a", "b", "c"], withscores=True) == [
-                (b"a3", 8),
-                (b"a1", 9),
-            ]
-            # aggregate with MAX
-            assert r.zinter(["a", "b", "c"], aggregate="MAX", withscores=True) == [
-                (b"a3", 5),
-                (b"a1", 6),
-            ]
-            # aggregate with MIN
-            assert r.zinter(["a", "b", "c"], aggregate="MIN", withscores=True) == [
-                (b"a1", 1),
-                (b"a3", 1),
-            ]
-            # with weights
-            assert r.zinter({"a": 1, "b": 2, "c": 3}, withscores=True) == [
-                (b"a3", 20),
-                (b"a1", 23),
-            ]
-        else:
-            # aggregate with SUM
-            assert r.zinter(["a", "b", "c"], withscores=True) == [
-                [b"a3", 8],
-                [b"a1", 9],
-            ]
-            # aggregate with MAX
-            assert r.zinter(["a", "b", "c"], aggregate="MAX", withscores=True) == [
-                [b"a3", 5],
-                [b"a1", 6],
-            ]
-            # aggregate with MIN
-            assert r.zinter(["a", "b", "c"], aggregate="MIN", withscores=True) == [
-                [b"a1", 1],
-                [b"a3", 1],
-            ]
-            # with weights
-            assert r.zinter({"a": 1, "b": 2, "c": 3}, withscores=True) == [
-                [b"a3", 20],
-                [b"a1", 23],
-            ]
+        # aggregate with SUM
+        assert_resp_response(
+            r,
+            r.zinter(["a", "b", "c"], withscores=True),
+            [(b"a3", 8), (b"a1", 9)],
+            [[b"a3", 8], [b"a1", 9]],
+        )
+        # aggregate with MAX
+        assert_resp_response(
+            r,
+            r.zinter(["a", "b", "c"], aggregate="MAX", withscores=True),
+            [(b"a3", 5), (b"a1", 6)],
+            [[b"a3", 5], [b"a1", 6]],
+        )
+        # aggregate with MIN
+        assert_resp_response(
+            r,
+            r.zinter(["a", "b", "c"], aggregate="MIN", withscores=True),
+            [(b"a1", 1), (b"a3", 1)],
+            [[b"a1", 1], [b"a3", 1]],
+        )
+        # with weights
+        assert_resp_response(
+            r,
+            r.zinter({"a": 1, "b": 2, "c": 3}, withscores=True),
+            [(b"a3", 20), (b"a1", 23)],
+            [[b"a3", 20], [b"a1", 23]],
+        )
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("7.0.0")
     def test_zintercard(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 1})
         r.zadd("b", {"a1": 2, "a2": 2, "a3": 2})
         r.zadd("c", {"a1": 6, "a3": 5, "a4": 4})
@@ -2416,86 +2410,96 @@
 
     @pytest.mark.onlynoncluster
     def test_zinterstore_sum(self, r):
         r.zadd("a", {"a1": 1, "a2": 1, "a3": 1})
         r.zadd("b", {"a1": 2, "a2": 2, "a3": 2})
         r.zadd("c", {"a1": 6, "a3": 5, "a4": 4})
         assert r.zinterstore("d", ["a", "b", "c"]) == 2
-        if is_resp2_connection(r):
-            assert r.zrange("d", 0, -1, withscores=True) == [(b"a3", 8), (b"a1", 9)]
-        else:
-            assert r.zrange("d", 0, -1, withscores=True) == [[b"a3", 8], [b"a1", 9]]
+        assert_resp_response(
+            r,
+            r.zrange("d", 0, -1, withscores=True),
+            [(b"a3", 8), (b"a1", 9)],
+            [[b"a3", 8], [b"a1", 9]],
+        )
 
     @pytest.mark.onlynoncluster
     def test_zinterstore_max(self, r):
         r.zadd("a", {"a1": 1, "a2": 1, "a3": 1})
         r.zadd("b", {"a1": 2, "a2": 2, "a3": 2})
         r.zadd("c", {"a1": 6, "a3": 5, "a4": 4})
         assert r.zinterstore("d", ["a", "b", "c"], aggregate="MAX") == 2
-        if is_resp2_connection(r):
-            assert r.zrange("d", 0, -1, withscores=True) == [(b"a3", 5), (b"a1", 6)]
-        else:
-            assert r.zrange("d", 0, -1, withscores=True) == [[b"a3", 5], [b"a1", 6]]
+        assert_resp_response(
+            r,
+            r.zrange("d", 0, -1, withscores=True),
+            [(b"a3", 5), (b"a1", 6)],
+            [[b"a3", 5], [b"a1", 6]],
+        )
 
     @pytest.mark.onlynoncluster
     def test_zinterstore_min(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3})
         r.zadd("b", {"a1": 2, "a2": 3, "a3": 5})
         r.zadd("c", {"a1": 6, "a3": 5, "a4": 4})
         assert r.zinterstore("d", ["a", "b", "c"], aggregate="MIN") == 2
-        if is_resp2_connection(r):
-            assert r.zrange("d", 0, -1, withscores=True) == [(b"a1", 1), (b"a3", 3)]
-        else:
-            assert r.zrange("d", 0, -1, withscores=True) == [[b"a1", 1], [b"a3", 3]]
+        assert_resp_response(
+            r,
+            r.zrange("d", 0, -1, withscores=True),
+            [(b"a1", 1), (b"a3", 3)],
+            [[b"a1", 1], [b"a3", 3]],
+        )
 
     @pytest.mark.onlynoncluster
     def test_zinterstore_with_weight(self, r):
         r.zadd("a", {"a1": 1, "a2": 1, "a3": 1})
         r.zadd("b", {"a1": 2, "a2": 2, "a3": 2})
         r.zadd("c", {"a1": 6, "a3": 5, "a4": 4})
         assert r.zinterstore("d", {"a": 1, "b": 2, "c": 3}) == 2
-        if is_resp2_connection(r):
-            assert r.zrange("d", 0, -1, withscores=True) == [(b"a3", 20), (b"a1", 23)]
-        else:
-            assert r.zrange("d", 0, -1, withscores=True) == [[b"a3", 20], [b"a1", 23]]
+        assert_resp_response(
+            r,
+            r.zrange("d", 0, -1, withscores=True),
+            [(b"a3", 20), (b"a1", 23)],
+            [[b"a3", 20], [b"a1", 23]],
+        )
 
     @skip_if_server_version_lt("4.9.0")
     def test_zpopmax(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3})
-        if is_resp2_connection(r):
-            assert r.zpopmax("a") == [(b"a3", 3)]
-            # with count
-            assert r.zpopmax("a", count=2) == [(b"a2", 2), (b"a1", 1)]
-        else:
-            assert r.zpopmax("a") == [b"a3", 3.0]
-            # with count
-            assert r.zpopmax("a", count=2) == [[b"a2", 2], [b"a1", 1]]
+        assert_resp_response(r, r.zpopmax("a"), [(b"a3", 3)], [b"a3", 3.0])
+        # with count
+        assert_resp_response(
+            r,
+            r.zpopmax("a", count=2),
+            [(b"a2", 2), (b"a1", 1)],
+            [[b"a2", 2], [b"a1", 1]],
+        )
 
     @skip_if_server_version_lt("4.9.0")
     def test_zpopmin(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3})
-        if is_resp2_connection(r):
-            assert r.zpopmin("a") == [(b"a1", 1)]
-            # with count
-            assert r.zpopmin("a", count=2) == [(b"a2", 2), (b"a3", 3)]
-        else:
-            assert r.zpopmin("a") == [b"a1", 1.0]
-            # with count
-            assert r.zpopmin("a", count=2) == [[b"a2", 2], [b"a3", 3]]
+        assert_resp_response(r, r.zpopmin("a"), [(b"a1", 1)], [b"a1", 1.0])
+        # with count
+        assert_resp_response(
+            r,
+            r.zpopmin("a", count=2),
+            [(b"a2", 2), (b"a3", 3)],
+            [[b"a2", 2], [b"a3", 3]],
+        )
 
     @skip_if_server_version_lt("6.2.0")
     def test_zrandemember(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3, "a4": 4, "a5": 5})
         assert r.zrandmember("a") is not None
         assert len(r.zrandmember("a", 2)) == 2
         # with scores
-        if is_resp2_connection(r):
-            assert len(r.zrandmember("a", 2, True)) == 4
-        else:
-            assert len(r.zrandmember("a", 2, True)) == 2
+        assert_resp_response(
+            r,
+            len(r.zrandmember("a", 2, withscores=True)),
+            4,
+            2,
+        )
         # without duplications
         assert len(r.zrandmember("a", 10)) == 5
         # with duplications
         assert len(r.zrandmember("a", -10)) == 10
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("4.9.0")
@@ -2523,54 +2527,77 @@
         r.zadd("c", {"c1": 100})
         assert r.bzpopmin("c", timeout=1) == (b"c", b"c1", 100)
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("7.0.0")
     def test_zmpop(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3})
-        res = [b"a", [[b"a1", b"1"], [b"a2", b"2"]]]
-        assert r.zmpop("2", ["b", "a"], min=True, count=2) == res
+        assert_resp_response(
+            r,
+            r.zmpop("2", ["b", "a"], min=True, count=2),
+            [b"a", [[b"a1", b"1"], [b"a2", b"2"]]],
+            [b"a", [[b"a1", 1.0], [b"a2", 2.0]]],
+        )
         with pytest.raises(redis.DataError):
             r.zmpop("2", ["b", "a"], count=2)
         r.zadd("b", {"b1": 10, "ab": 9, "b3": 8})
-        assert r.zmpop("2", ["b", "a"], max=True) == [b"b", [[b"b1", b"10"]]]
+        assert_resp_response(
+            r,
+            r.zmpop("2", ["b", "a"], max=True),
+            [b"b", [[b"b1", b"10"]]],
+            [b"b", [[b"b1", 10.0]]],
+        )
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("7.0.0")
     def test_bzmpop(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3})
-        res = [b"a", [[b"a1", b"1"], [b"a2", b"2"]]]
-        assert r.bzmpop(1, "2", ["b", "a"], min=True, count=2) == res
+        assert_resp_response(
+            r,
+            r.bzmpop(1, "2", ["b", "a"], min=True, count=2),
+            [b"a", [[b"a1", b"1"], [b"a2", b"2"]]],
+            [b"a", [[b"a1", 1.0], [b"a2", 2.0]]],
+        )
         with pytest.raises(redis.DataError):
             r.bzmpop(1, "2", ["b", "a"], count=2)
         r.zadd("b", {"b1": 10, "ab": 9, "b3": 8})
-        res = [b"b", [[b"b1", b"10"]]]
-        assert r.bzmpop(0, "2", ["b", "a"], max=True) == res
+        assert_resp_response(
+            r,
+            r.bzmpop(0, "2", ["b", "a"], max=True),
+            [b"b", [[b"b1", b"10"]]],
+            [b"b", [[b"b1", 10.0]]],
+        )
         assert r.bzmpop(1, "2", ["foo", "bar"], max=True) is None
 
     def test_zrange(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3})
         assert r.zrange("a", 0, 1) == [b"a1", b"a2"]
         assert r.zrange("a", 1, 2) == [b"a2", b"a3"]
         assert r.zrange("a", 0, 2) == [b"a1", b"a2", b"a3"]
         assert r.zrange("a", 0, 2, desc=True) == [b"a3", b"a2", b"a1"]
 
         # withscores
-        if is_resp2_connection(r):
-            assert r.zrange("a", 0, 1, withscores=True) == [(b"a1", 1.0), (b"a2", 2.0)]
-            assert r.zrange("a", 1, 2, withscores=True) == [(b"a2", 2.0), (b"a3", 3.0)]
-
-            # custom score function
-            assert r.zrange("a", 0, 1, withscores=True, score_cast_func=int) == [
-                (b"a1", 1),
-                (b"a2", 2),
-            ]
-        else:
-            assert r.zrange("a", 0, 1, withscores=True) == [[b"a1", 1.0], [b"a2", 2.0]]
-            assert r.zrange("a", 1, 2, withscores=True) == [[b"a2", 2.0], [b"a3", 3.0]]
+        assert_resp_response(
+            r,
+            r.zrange("a", 0, 1, withscores=True),
+            [(b"a1", 1.0), (b"a2", 2.0)],
+            [[b"a1", 1.0], [b"a2", 2.0]],
+        )
+        assert_resp_response(
+            r,
+            r.zrange("a", 1, 2, withscores=True),
+            [(b"a2", 2.0), (b"a3", 3.0)],
+            [[b"a2", 2.0], [b"a3", 3.0]],
+        )
+
+        # # custom score function
+        # assert r.zrange("a", 0, 1, withscores=True, score_cast_func=int) == [
+        #     (b"a1", 1),
+        #     (b"a2", 2),
+        # ]
 
     def test_zrange_errors(self, r):
         with pytest.raises(exceptions.DataError):
             r.zrange("a", 0, 1, byscore=True, bylex=True)
         with pytest.raises(exceptions.DataError):
             r.zrange("a", 0, 1, bylex=True, withscores=True)
         with pytest.raises(exceptions.DataError):
@@ -2594,49 +2621,46 @@
         # byscore
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3, "a4": 4, "a5": 5})
         assert r.zrange("a", 2, 4, byscore=True, offset=1, num=2) == [b"a3", b"a4"]
         assert r.zrange("a", 4, 2, desc=True, byscore=True, offset=1, num=2) == [
             b"a3",
             b"a2",
         ]
-        if is_resp2_connection(r):
-            assert r.zrange("a", 2, 4, byscore=True, withscores=True) == [
-                (b"a2", 2.0),
-                (b"a3", 3.0),
-                (b"a4", 4.0),
-            ]
-            assert r.zrange(
-                "a", 4, 2, desc=True, byscore=True, withscores=True, score_cast_func=int
-            ) == [(b"a4", 4), (b"a3", 3), (b"a2", 2)]
-
-        else:
-            assert r.zrange("a", 2, 4, byscore=True, withscores=True) == [
-                [b"a2", 2.0],
-                [b"a3", 3.0],
-                [b"a4", 4.0],
-            ]
-            assert r.zrange(
+        assert_resp_response(
+            r,
+            r.zrange("a", 2, 4, byscore=True, withscores=True),
+            [(b"a2", 2.0), (b"a3", 3.0), (b"a4", 4.0)],
+            [[b"a2", 2.0], [b"a3", 3.0], [b"a4", 4.0]],
+        )
+        assert_resp_response(
+            r,
+            r.zrange(
                 "a", 4, 2, desc=True, byscore=True, withscores=True, score_cast_func=int
-            ) == [[b"a4", 4], [b"a3", 3], [b"a2", 2]]
+            ),
+            [(b"a4", 4), (b"a3", 3), (b"a2", 2)],
+            [[b"a4", 4], [b"a3", 3], [b"a2", 2]],
+        )
 
         # rev
         assert r.zrange("a", 0, 1, desc=True) == [b"a5", b"a4"]
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("6.2.0")
     def test_zrangestore(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3})
         assert r.zrangestore("b", "a", 0, 1)
         assert r.zrange("b", 0, -1) == [b"a1", b"a2"]
         assert r.zrangestore("b", "a", 1, 2)
         assert r.zrange("b", 0, -1) == [b"a2", b"a3"]
-        if is_resp2_connection(r):
-            assert r.zrange("b", 0, -1, withscores=True) == [(b"a2", 2), (b"a3", 3)]
-        else:
-            assert r.zrange("b", 0, -1, withscores=True) == [[b"a2", 2], [b"a3", 3]]
+        assert_resp_response(
+            r,
+            r.zrange("b", 0, -1, withscores=True),
+            [(b"a2", 2), (b"a3", 3)],
+            [[b"a2", 2], [b"a3", 3]],
+        )
         # reversed order
         assert r.zrangestore("b", "a", 1, 2, desc=True)
         assert r.zrange("b", 0, -1) == [b"a1", b"a2"]
         # by score
         assert r.zrangestore("b", "a", 2, 1, byscore=True, offset=0, num=1, desc=True)
         assert r.zrange("b", 0, -1) == [b"a2"]
         # by lex
@@ -2663,36 +2687,26 @@
 
     def test_zrangebyscore(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3, "a4": 4, "a5": 5})
         assert r.zrangebyscore("a", 2, 4) == [b"a2", b"a3", b"a4"]
         # slicing with start/num
         assert r.zrangebyscore("a", 2, 4, start=1, num=2) == [b"a3", b"a4"]
         # withscores
-        if is_resp2_connection(r):
-            assert r.zrangebyscore("a", 2, 4, withscores=True) == [
-                (b"a2", 2.0),
-                (b"a3", 3.0),
-                (b"a4", 4.0),
-            ]
-            assert r.zrangebyscore("a", 2, 4, withscores=True, score_cast_func=int) == [
-                (b"a2", 2),
-                (b"a3", 3),
-                (b"a4", 4),
-            ]
-        else:
-            assert r.zrangebyscore("a", 2, 4, withscores=True) == [
-                [b"a2", 2.0],
-                [b"a3", 3.0],
-                [b"a4", 4.0],
-            ]
-            assert r.zrangebyscore("a", 2, 4, withscores=True, score_cast_func=int) == [
-                [b"a2", 2],
-                [b"a3", 3],
-                [b"a4", 4],
-            ]
+        assert_resp_response(
+            r,
+            r.zrangebyscore("a", 2, 4, withscores=True),
+            [(b"a2", 2.0), (b"a3", 3.0), (b"a4", 4.0)],
+            [[b"a2", 2.0], [b"a3", 3.0], [b"a4", 4.0]],
+        )
+        assert_resp_response(
+            r,
+            r.zrangebyscore("a", 2, 4, withscores=True, score_cast_func=int),
+            [(b"a2", 2), (b"a3", 3), (b"a4", 4)],
+            [[b"a2", 2], [b"a3", 3], [b"a4", 4]],
+        )
 
     def test_zrank(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3, "a4": 4, "a5": 5})
         assert r.zrank("a", "a1") == 0
         assert r.zrank("a", "a2") == 1
         assert r.zrank("a", "a6") is None
 
@@ -2731,69 +2745,54 @@
         assert r.zrange("a", 0, -1) == [b"a1", b"a5"]
 
     def test_zrevrange(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3})
         assert r.zrevrange("a", 0, 1) == [b"a3", b"a2"]
         assert r.zrevrange("a", 1, 2) == [b"a2", b"a1"]
 
-        if is_resp2_connection(r):
-            # withscores
-            assert r.zrevrange("a", 0, 1, withscores=True) == [
-                (b"a3", 3.0),
-                (b"a2", 2.0),
-            ]
-            assert r.zrevrange("a", 1, 2, withscores=True) == [
-                (b"a2", 2.0),
-                (b"a1", 1.0),
-            ]
-
-            # custom score function
-            assert r.zrevrange("a", 0, 1, withscores=True, score_cast_func=int) == [
-                (b"a3", 3.0),
-                (b"a2", 2.0),
-            ]
-        else:
-            # withscores
-            assert r.zrevrange("a", 0, 1, withscores=True) == [
-                [b"a3", 3.0],
-                [b"a2", 2.0],
-            ]
-            assert r.zrevrange("a", 1, 2, withscores=True) == [
-                [b"a2", 2.0],
-                [b"a1", 1.0],
-            ]
+        # withscores
+        assert_resp_response(
+            r,
+            r.zrevrange("a", 0, 1, withscores=True),
+            [(b"a3", 3.0), (b"a2", 2.0)],
+            [[b"a3", 3.0], [b"a2", 2.0]],
+        )
+        assert_resp_response(
+            r,
+            r.zrevrange("a", 1, 2, withscores=True),
+            [(b"a2", 2.0), (b"a1", 1.0)],
+            [[b"a2", 2.0], [b"a1", 1.0]],
+        )
+
+        # # custom score function
+        # assert r.zrevrange("a", 0, 1, withscores=True, score_cast_func=int) == [
+        #     (b"a3", 3.0),
+        #     (b"a2", 2.0),
+        # ]
 
     def test_zrevrangebyscore(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3, "a4": 4, "a5": 5})
         assert r.zrevrangebyscore("a", 4, 2) == [b"a4", b"a3", b"a2"]
         # slicing with start/num
         assert r.zrevrangebyscore("a", 4, 2, start=1, num=2) == [b"a3", b"a2"]
 
-        if is_resp2_connection(r):
-            # withscores
-            assert r.zrevrangebyscore("a", 4, 2, withscores=True) == [
-                (b"a4", 4.0),
-                (b"a3", 3.0),
-                (b"a2", 2.0),
-            ]
-            # custom score function
-            assert r.zrevrangebyscore(
-                "a", 4, 2, withscores=True, score_cast_func=int
-            ) == [
-                (b"a4", 4),
-                (b"a3", 3),
-                (b"a2", 2),
-            ]
-        else:
-            # withscores
-            assert r.zrevrangebyscore("a", 4, 2, withscores=True) == [
-                [b"a4", 4.0],
-                [b"a3", 3.0],
-                [b"a2", 2.0],
-            ]
+        # withscores
+        assert_resp_response(
+            r,
+            r.zrevrangebyscore("a", 4, 2, withscores=True),
+            [(b"a4", 4.0), (b"a3", 3.0), (b"a2", 2.0)],
+            [[b"a4", 4.0], [b"a3", 3.0], [b"a2", 2.0]],
+        )
+        # custom score function
+        assert_resp_response(
+            r,
+            r.zrevrangebyscore("a", 4, 2, withscores=True, score_cast_func=int),
+            [(b"a4", 4.0), (b"a3", 3.0), (b"a2", 2.0)],
+            [[b"a4", 4.0], [b"a3", 3.0], [b"a2", 2.0]],
+        )
 
     def test_zrevrank(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3, "a4": 4, "a5": 5})
         assert r.zrevrank("a", "a1") == 4
         assert r.zrevrank("a", "a2") == 3
         assert r.zrevrank("a", "a6") is None
 
@@ -2807,156 +2806,93 @@
     @skip_if_server_version_lt("6.2.0")
     def test_zunion(self, r):
         r.zadd("a", {"a1": 1, "a2": 1, "a3": 1})
         r.zadd("b", {"a1": 2, "a2": 2, "a3": 2})
         r.zadd("c", {"a1": 6, "a3": 5, "a4": 4})
         # sum
         assert r.zunion(["a", "b", "c"]) == [b"a2", b"a4", b"a3", b"a1"]
-
-        if is_resp2_connection(r):
-            assert r.zunion(["a", "b", "c"], withscores=True) == [
-                (b"a2", 3),
-                (b"a4", 4),
-                (b"a3", 8),
-                (b"a1", 9),
-            ]
-            # max
-            assert r.zunion(["a", "b", "c"], aggregate="MAX", withscores=True) == [
-                (b"a2", 2),
-                (b"a4", 4),
-                (b"a3", 5),
-                (b"a1", 6),
-            ]
-            # min
-            assert r.zunion(["a", "b", "c"], aggregate="MIN", withscores=True) == [
-                (b"a1", 1),
-                (b"a2", 1),
-                (b"a3", 1),
-                (b"a4", 4),
-            ]
-            # with weight
-            assert r.zunion({"a": 1, "b": 2, "c": 3}, withscores=True) == [
-                (b"a2", 5),
-                (b"a4", 12),
-                (b"a3", 20),
-                (b"a1", 23),
-            ]
-        else:
-            assert r.zunion(["a", "b", "c"], withscores=True) == [
-                [b"a2", 3],
-                [b"a4", 4],
-                [b"a3", 8],
-                [b"a1", 9],
-            ]
-            # max
-            assert r.zunion(["a", "b", "c"], aggregate="MAX", withscores=True) == [
-                [b"a2", 2],
-                [b"a4", 4],
-                [b"a3", 5],
-                [b"a1", 6],
-            ]
-            # min
-            assert r.zunion(["a", "b", "c"], aggregate="MIN", withscores=True) == [
-                [b"a1", 1],
-                [b"a2", 1],
-                [b"a3", 1],
-                [b"a4", 4],
-            ]
-            # with weight
-            assert r.zunion({"a": 1, "b": 2, "c": 3}, withscores=True) == [
-                [b"a2", 5],
-                [b"a4", 12],
-                [b"a3", 20],
-                [b"a1", 23],
-            ]
+        assert_resp_response(
+            r,
+            r.zunion(["a", "b", "c"], withscores=True),
+            [(b"a2", 3), (b"a4", 4), (b"a3", 8), (b"a1", 9)],
+            [[b"a2", 3], [b"a4", 4], [b"a3", 8], [b"a1", 9]],
+        )
+        # max
+        assert_resp_response(
+            r,
+            r.zunion(["a", "b", "c"], aggregate="MAX", withscores=True),
+            [(b"a2", 2), (b"a4", 4), (b"a3", 5), (b"a1", 6)],
+            [[b"a2", 2], [b"a4", 4], [b"a3", 5], [b"a1", 6]],
+        )
+        # min
+        assert_resp_response(
+            r,
+            r.zunion(["a", "b", "c"], aggregate="MIN", withscores=True),
+            [(b"a1", 1), (b"a2", 1), (b"a3", 1), (b"a4", 4)],
+            [[b"a1", 1], [b"a2", 1], [b"a3", 1], [b"a4", 4]],
+        )
+        # with weight
+        assert_resp_response(
+            r,
+            r.zunion({"a": 1, "b": 2, "c": 3}, withscores=True),
+            [(b"a2", 5), (b"a4", 12), (b"a3", 20), (b"a1", 23)],
+            [[b"a2", 5], [b"a4", 12], [b"a3", 20], [b"a1", 23]],
+        )
 
     @pytest.mark.onlynoncluster
     def test_zunionstore_sum(self, r):
         r.zadd("a", {"a1": 1, "a2": 1, "a3": 1})
         r.zadd("b", {"a1": 2, "a2": 2, "a3": 2})
         r.zadd("c", {"a1": 6, "a3": 5, "a4": 4})
         assert r.zunionstore("d", ["a", "b", "c"]) == 4
-
-        if is_resp2_connection(r):
-            assert r.zrange("d", 0, -1, withscores=True) == [
-                (b"a2", 3),
-                (b"a4", 4),
-                (b"a3", 8),
-                (b"a1", 9),
-            ]
-        else:
-            assert r.zrange("d", 0, -1, withscores=True) == [
-                [b"a2", 3],
-                [b"a4", 4],
-                [b"a3", 8],
-                [b"a1", 9],
-            ]
+        assert_resp_response(
+            r,
+            r.zrange("d", 0, -1, withscores=True),
+            [(b"a2", 3), (b"a4", 4), (b"a3", 8), (b"a1", 9)],
+            [[b"a2", 3], [b"a4", 4], [b"a3", 8], [b"a1", 9]],
+        )
 
     @pytest.mark.onlynoncluster
     def test_zunionstore_max(self, r):
         r.zadd("a", {"a1": 1, "a2": 1, "a3": 1})
         r.zadd("b", {"a1": 2, "a2": 2, "a3": 2})
         r.zadd("c", {"a1": 6, "a3": 5, "a4": 4})
         assert r.zunionstore("d", ["a", "b", "c"], aggregate="MAX") == 4
-        if is_resp2_connection(r):
-            assert r.zrange("d", 0, -1, withscores=True) == [
-                (b"a2", 2),
-                (b"a4", 4),
-                (b"a3", 5),
-                (b"a1", 6),
-            ]
-        else:
-            assert r.zrange("d", 0, -1, withscores=True) == [
-                [b"a2", 2],
-                [b"a4", 4],
-                [b"a3", 5],
-                [b"a1", 6],
-            ]
+        assert_resp_response(
+            r,
+            r.zrange("d", 0, -1, withscores=True),
+            [(b"a2", 2), (b"a4", 4), (b"a3", 5), (b"a1", 6)],
+            [[b"a2", 2], [b"a4", 4], [b"a3", 5], [b"a1", 6]],
+        )
 
     @pytest.mark.onlynoncluster
     def test_zunionstore_min(self, r):
         r.zadd("a", {"a1": 1, "a2": 2, "a3": 3})
         r.zadd("b", {"a1": 2, "a2": 2, "a3": 4})
         r.zadd("c", {"a1": 6, "a3": 5, "a4": 4})
         assert r.zunionstore("d", ["a", "b", "c"], aggregate="MIN") == 4
-        if is_resp2_connection(r):
-            assert r.zrange("d", 0, -1, withscores=True) == [
-                (b"a1", 1),
-                (b"a2", 2),
-                (b"a3", 3),
-                (b"a4", 4),
-            ]
-        else:
-            assert r.zrange("d", 0, -1, withscores=True) == [
-                [b"a1", 1],
-                [b"a2", 2],
-                [b"a3", 3],
-                [b"a4", 4],
-            ]
+        assert_resp_response(
+            r,
+            r.zrange("d", 0, -1, withscores=True),
+            [(b"a1", 1), (b"a2", 2), (b"a3", 3), (b"a4", 4)],
+            [[b"a1", 1], [b"a2", 2], [b"a3", 3], [b"a4", 4]],
+        )
 
     @pytest.mark.onlynoncluster
     def test_zunionstore_with_weight(self, r):
         r.zadd("a", {"a1": 1, "a2": 1, "a3": 1})
         r.zadd("b", {"a1": 2, "a2": 2, "a3": 2})
         r.zadd("c", {"a1": 6, "a3": 5, "a4": 4})
         assert r.zunionstore("d", {"a": 1, "b": 2, "c": 3}) == 4
-        if is_resp2_connection(r):
-            assert r.zrange("d", 0, -1, withscores=True) == [
-                (b"a2", 5),
-                (b"a4", 12),
-                (b"a3", 20),
-                (b"a1", 23),
-            ]
-        else:
-            assert r.zrange("d", 0, -1, withscores=True) == [
-                [b"a2", 5],
-                [b"a4", 12],
-                [b"a3", 20],
-                [b"a1", 23],
-            ]
+        assert_resp_response(
+            r,
+            r.zrange("d", 0, -1, withscores=True),
+            [(b"a2", 5), (b"a4", 12), (b"a3", 20), (b"a1", 23)],
+            [[b"a2", 5], [b"a4", 12], [b"a3", 20], [b"a1", 23]],
+        )
 
     @skip_if_server_version_lt("6.1.240")
     def test_zmscore(self, r):
         with pytest.raises(exceptions.DataError):
             r.zmscore("invalid_key", [])
 
         assert r.zmscore("invalid_key", ["invalid_member"]) == [None]
@@ -4016,30 +3952,30 @@
     @skip_if_server_version_lt("7.0.0")
     def test_xadd_explicit_ms(self, r: redis.Redis):
         stream = "stream"
         message_id = r.xadd(stream, {"foo": "bar"}, "9999999999999999999-*")
         ms = message_id[: message_id.index(b"-")]
         assert ms == b"9999999999999999999"
 
-    @skip_if_server_version_lt("6.2.0")
+    @skip_if_server_version_lt("7.0.0")
     def test_xautoclaim(self, r):
         stream = "stream"
         group = "group"
         consumer1 = "consumer1"
         consumer2 = "consumer2"
 
         message_id1 = r.xadd(stream, {"john": "wick"})
         message_id2 = r.xadd(stream, {"johny": "deff"})
         message = get_stream_message(r, stream, message_id1)
         r.xgroup_create(stream, group, 0)
 
         # trying to claim a message that isn't already pending doesn't
         # do anything
         response = r.xautoclaim(stream, group, consumer2, min_idle_time=0)
-        assert response == [b"0-0", []]
+        assert response == [b"0-0", [], []]
 
         # read the group as consumer1 to initially claim the messages
         r.xreadgroup(group, consumer1, streams={stream: ">"})
 
         # claim one message as consumer2
         response = r.xautoclaim(stream, group, consumer2, min_idle_time=0, count=1)
         assert response[1] == [message]
@@ -4275,15 +4211,15 @@
                 "last-delivered-id": message_id,
                 "entries-read": 2,
                 "lag": -1,
             }
         ]
         assert r.xinfo_groups(stream) == expected
 
-    @skip_if_server_version_lt("5.0.0")
+    @skip_if_server_version_lt("7.2.0")
     def test_xinfo_consumers(self, r):
         stream = "stream"
         group = "group"
         consumer1 = "consumer1"
         consumer2 = "consumer2"
         r.xadd(stream, {"foo": "bar"})
         r.xadd(stream, {"foo": "bar"})
@@ -4291,16 +4227,16 @@
 
         r.xgroup_create(stream, group, 0)
         r.xreadgroup(group, consumer1, streams={stream: ">"}, count=1)
         r.xreadgroup(group, consumer2, streams={stream: ">"})
         info = r.xinfo_consumers(stream, group)
         assert len(info) == 2
         expected = [
-            {"name": consumer1.encode(), "pending": 1},
-            {"name": consumer2.encode(), "pending": 2},
+            {"name": consumer1.encode(), "pending": 1, "inactive": 2},
+            {"name": consumer2.encode(), "pending": 2, "inactive": 2},
         ]
 
         # we can't determine the idle time, so just make sure it's an int
         assert isinstance(info[0].pop("idle"), int)
         assert isinstance(info[1].pop("idle"), int)
         assert info == expected
 
@@ -4323,18 +4259,20 @@
         stream = "stream"
         group = "group"
         m1 = r.xadd(stream, {"foo": "bar"})
         r.xgroup_create(stream, group, 0)
         info = r.xinfo_stream(stream, full=True)
 
         assert info["length"] == 1
-        if is_resp2_connection(r):
-            assert m1 in info["entries"]
-        else:
-            assert m1 in info["entries"][0]
+        assert_resp_response_in(
+            r,
+            m1,
+            info["entries"],
+            info["entries"].keys(),
+        )
         assert len(info["groups"]) == 1
 
     @skip_if_server_version_lt("5.0.0")
     def test_xlen(self, r):
         stream = "stream"
         assert r.xlen(stream) == 0
         r.xadd(stream, {"foo": "bar"})
@@ -4467,120 +4405,121 @@
 
     @skip_if_server_version_lt("5.0.0")
     def test_xread(self, r):
         stream = "stream"
         m1 = r.xadd(stream, {"foo": "bar"})
         m2 = r.xadd(stream, {"bing": "baz"})
 
-        strem_name = stream.encode()
+        stream_name = stream.encode()
         expected_entries = [
             get_stream_message(r, stream, m1),
             get_stream_message(r, stream, m2),
         ]
         # xread starting at 0 returns both messages
-        res = r.xread(streams={stream: 0})
-        if is_resp2_connection(r):
-            assert res == [[strem_name, expected_entries]]
-        else:
-            assert res == {strem_name: [expected_entries]}
+        assert_resp_response(
+            r,
+            r.xread(streams={stream: 0}),
+            [[stream_name, expected_entries]],
+            {stream_name: [expected_entries]},
+        )
 
         expected_entries = [get_stream_message(r, stream, m1)]
         # xread starting at 0 and count=1 returns only the first message
-        res = r.xread(streams={stream: 0}, count=1)
-        if is_resp2_connection(r):
-            assert res == [[strem_name, expected_entries]]
-        else:
-            assert res == {strem_name: [expected_entries]}
+        assert_resp_response(
+            r,
+            r.xread(streams={stream: 0}, count=1),
+            [[stream_name, expected_entries]],
+            {stream_name: [expected_entries]},
+        )
 
         expected_entries = [get_stream_message(r, stream, m2)]
         # xread starting at m1 returns only the second message
-        res = r.xread(streams={stream: m1})
-        if is_resp2_connection(r):
-            assert res == [[strem_name, expected_entries]]
-        else:
-            assert res == {strem_name: [expected_entries]}
+        assert_resp_response(
+            r,
+            r.xread(streams={stream: m1}),
+            [[stream_name, expected_entries]],
+            {stream_name: [expected_entries]},
+        )
 
         # xread starting at the last message returns an empty list
-        res = r.xread(streams={stream: m2})
-        if is_resp2_connection(r):
-            assert res == []
-        else:
-            assert res == {}
+        assert_resp_response(r, r.xread(streams={stream: m2}), [], {})
 
     @skip_if_server_version_lt("5.0.0")
     def test_xreadgroup(self, r):
         stream = "stream"
         group = "group"
         consumer = "consumer"
         m1 = r.xadd(stream, {"foo": "bar"})
         m2 = r.xadd(stream, {"bing": "baz"})
         r.xgroup_create(stream, group, 0)
 
-        strem_name = stream.encode()
+        stream_name = stream.encode()
         expected_entries = [
             get_stream_message(r, stream, m1),
             get_stream_message(r, stream, m2),
         ]
 
         # xread starting at 0 returns both messages
-        res = r.xreadgroup(group, consumer, streams={stream: ">"})
-        if is_resp2_connection(r):
-            assert res == [[strem_name, expected_entries]]
-        else:
-            assert res == {strem_name: [expected_entries]}
+        assert_resp_response(
+            r,
+            r.xreadgroup(group, consumer, streams={stream: ">"}),
+            [[stream_name, expected_entries]],
+            {stream_name: [expected_entries]},
+        )
 
         r.xgroup_destroy(stream, group)
         r.xgroup_create(stream, group, 0)
 
         expected_entries = [get_stream_message(r, stream, m1)]
 
         # xread with count=1 returns only the first message
-        res = r.xreadgroup(group, consumer, streams={stream: ">"}, count=1)
-        if is_resp2_connection(r):
-            assert res == [[strem_name, expected_entries]]
-        else:
-            assert res == {strem_name: [expected_entries]}
+        assert_resp_response(
+            r,
+            r.xreadgroup(group, consumer, streams={stream: ">"}, count=1),
+            [[stream_name, expected_entries]],
+            {stream_name: [expected_entries]},
+        )
 
         r.xgroup_destroy(stream, group)
 
         # create the group using $ as the last id meaning subsequent reads
         # will only find messages added after this
         r.xgroup_create(stream, group, "$")
 
         # xread starting after the last message returns an empty message list
-        if is_resp2_connection(r):
-            assert r.xreadgroup(group, consumer, streams={stream: ">"}) == []
-        else:
-            assert r.xreadgroup(group, consumer, streams={stream: ">"}) == {}
+        assert_resp_response(
+            r, r.xreadgroup(group, consumer, streams={stream: ">"}), [], {}
+        )
 
         # xreadgroup with noack does not have any items in the PEL
         r.xgroup_destroy(stream, group)
         r.xgroup_create(stream, group, "0")
         res = r.xreadgroup(group, consumer, streams={stream: ">"}, noack=True)
         empty_res = r.xreadgroup(group, consumer, streams={stream: "0"})
         if is_resp2_connection(r):
             assert len(res[0][1]) == 2
             # now there should be nothing pending
             assert len(empty_res[0][1]) == 0
         else:
-            assert len(res[strem_name][0]) == 2
+            assert len(res[stream_name][0]) == 2
             # now there should be nothing pending
-            assert len(empty_res[strem_name][0]) == 0
+            assert len(empty_res[stream_name][0]) == 0
 
         r.xgroup_destroy(stream, group)
         r.xgroup_create(stream, group, "0")
         # delete all the messages in the stream
         expected_entries = [(m1, {}), (m2, {})]
         r.xreadgroup(group, consumer, streams={stream: ">"})
         r.xtrim(stream, 0)
-        res = r.xreadgroup(group, consumer, streams={stream: "0"})
-        if is_resp2_connection(r):
-            assert res == [[strem_name, expected_entries]]
-        else:
-            assert res == {strem_name: [expected_entries]}
+        assert_resp_response(
+            r,
+            r.xreadgroup(group, consumer, streams={stream: "0"}),
+            [[stream_name, expected_entries]],
+            {stream_name: [expected_entries]},
+        )
 
     @skip_if_server_version_lt("5.0.0")
     def test_xrevrange(self, r):
         stream = "stream"
         m1 = r.xadd(stream, {"foo": "bar"})
         m2 = r.xadd(stream, {"foo": "bar"})
         m3 = r.xadd(stream, {"foo": "bar"})
@@ -4865,20 +4804,25 @@
         assert "set" in cmds
         assert "get" in cmds
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("7.0.0")
     @skip_if_redis_enterprise()
     def test_command_getkeysandflags(self, r: redis.Redis):
-        res = [
-            [b"mylist1", [b"RW", b"access", b"delete"]],
-            [b"mylist2", [b"RW", b"insert"]],
-        ]
-        assert res == r.command_getkeysandflags(
-            "LMOVE", "mylist1", "mylist2", "left", "left"
+        assert_resp_response(
+            r,
+            r.command_getkeysandflags("LMOVE", "mylist1", "mylist2", "left", "left"),
+            [
+                [b"mylist1", [b"RW", b"access", b"delete"]],
+                [b"mylist2", [b"RW", b"insert"]],
+            ],
+            [
+                [b"mylist1", {b"RW", b"access", b"delete"}],
+                [b"mylist2", {b"RW", b"insert"}],
+            ],
         )
 
     @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("4.0.0")
     @skip_if_redis_enterprise()
     def test_module(self, r):
         with pytest.raises(redis.exceptions.ModuleError) as excinfo:
@@ -4966,14 +4910,16 @@
         r.execute_command("SHUTDOWN", "ABORT")
         r.execute_command.assert_called_with("SHUTDOWN", "ABORT")
 
     @pytest.mark.replica
     @skip_if_server_version_lt("2.8.0")
     @skip_if_redis_enterprise()
     def test_sync(self, r):
+        r.flushdb()
+        time.sleep(1)
         r2 = redis.Redis(port=6380, decode_responses=False)
         res = r2.sync()
         assert b"REDIS" in res
 
     @pytest.mark.replica
     @skip_if_server_version_lt("2.8.0")
     @skip_if_redis_enterprise()
```

### Comparing `redis-5.0.0b4/tests/test_connection.py` & `redis-5.0.0rc1/tests/test_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import socket
 import types
 from unittest import mock
 from unittest.mock import patch
 
 import pytest
-
 import redis
 from redis.backoff import NoBackoff
 from redis.connection import Connection, SSLConnection, UnixDomainSocketConnection
 from redis.exceptions import ConnectionError, InvalidResponse, TimeoutError
 from redis.parsers import _HiredisParser, _RESP2Parser, _RESP3Parser
 from redis.retry import Retry
 from redis.utils import HIREDIS_AVAILABLE
@@ -26,30 +25,30 @@
         with pytest.raises(InvalidResponse) as cm:
             parser.read_response()
     assert str(cm.value) == f"Protocol Error: {raw!r}"
 
 
 @skip_if_server_version_lt("4.0.0")
 @pytest.mark.redismod
-def test_loading_external_modules(modclient):
+def test_loading_external_modules(r):
     def inner():
         pass
 
-    modclient.load_external_module("myfuncname", inner)
-    assert getattr(modclient, "myfuncname") == inner
-    assert isinstance(getattr(modclient, "myfuncname"), types.FunctionType)
+    r.load_external_module("myfuncname", inner)
+    assert getattr(r, "myfuncname") == inner
+    assert isinstance(getattr(r, "myfuncname"), types.FunctionType)
 
     # and call it
     from redis.commands import RedisModuleCommands
 
     j = RedisModuleCommands.json
-    modclient.load_external_module("sometestfuncname", j)
+    r.load_external_module("sometestfuncname", j)
 
     # d = {'hello': 'world!'}
-    # mod = j(modclient)
+    # mod = j(r)
     # mod.set("fookey", ".", d)
     # assert mod.get('fookey') == d
 
 
 class TestConnection:
     def test_disconnect(self):
         conn = Connection()
```

### Comparing `redis-5.0.0b4/tests/test_connection_pool.py` & `redis-5.0.0rc1/tests/test_connection_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import re
 import time
 from threading import Thread
 from unittest import mock
 
 import pytest
-
 import redis
 from redis.connection import to_bool
 from redis.utils import SSL_AVAILABLE
 
 from .conftest import _get_client, skip_if_redis_enterprise, skip_if_server_version_lt
 from .test_pubsub import wait_for_message
```

### Comparing `redis-5.0.0b4/tests/test_credentials.py` & `redis-5.0.0rc1/tests/test_credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import functools
 import random
 import string
 from typing import Optional, Tuple, Union
 
 import pytest
-
 import redis
 from redis import AuthenticationError, DataError, ResponseError
 from redis.credentials import CredentialProvider, UsernamePasswordCredentialProvider
 from redis.utils import str_if_bytes
 from tests.conftest import _get_client, skip_if_redis_enterprise
 
 
@@ -194,14 +193,20 @@
 
     @pytest.mark.onlynoncluster
     def test_change_username_password_on_existing_connection(self, r, request):
         username = "origin_username"
         password = "origin_password"
         new_username = "new_username"
         new_password = "new_password"
+
+        def teardown():
+            r.acl_deluser(new_username)
+
+        request.addfinalizer(teardown)
+
         init_acl_user(r, request, username, password)
         r2 = _get_client(
             redis.Redis, request, flushdb=False, username=username, password=password
         )
         assert r2.ping() is True
         conn = r2.connection_pool.get_connection("_")
         conn.send_command("PING")
```

### Comparing `redis-5.0.0b4/tests/test_encoding.py` & `redis-5.0.0rc1/tests/test_encoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 import redis
 from redis.connection import Connection
 from redis.utils import HIREDIS_PACK_AVAILABLE
 
 from .conftest import _get_client
```

### Comparing `redis-5.0.0b4/tests/test_function.py` & `redis-5.0.0rc1/tests/test_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pytest
-
 from redis.exceptions import ResponseError
 
-from .conftest import skip_if_server_version_lt
+from .conftest import assert_resp_response, skip_if_server_version_lt
 
 engine = "lua"
 lib = "mylib"
 lib2 = "mylib2"
 function = "redis.register_function{function_name='myfunc', callback=function(keys, \
             args) return args[1] end, flags={ 'no-writes' }}"
 function2 = "redis.register_function('hello', function() return 'Hello World' end)"
@@ -60,20 +59,30 @@
                 b"mylib",
                 b"engine",
                 b"LUA",
                 b"functions",
                 [[b"name", b"myfunc", b"description", None, b"flags", [b"no-writes"]]],
             ]
         ]
-        assert r.function_list() == res
-        assert r.function_list(library="*lib") == res
-        assert (
-            r.function_list(withcode=True)[0][7]
-            == f"#!{engine} name={lib} \n {function}".encode()
+        resp3_res = [
+            {
+                b"library_name": b"mylib",
+                b"engine": b"LUA",
+                b"functions": [
+                    {b"name": b"myfunc", b"description": None, b"flags": {b"no-writes"}}
+                ],
+            }
+        ]
+        assert_resp_response(r, r.function_list(), res, resp3_res)
+        assert_resp_response(r, r.function_list(library="*lib"), res, resp3_res)
+        res[0].extend(
+            [b"library_code", f"#!{engine} name={lib} \n {function}".encode()]
         )
+        resp3_res[0][b"library_code"] = f"#!{engine} name={lib} \n {function}".encode()
+        assert_resp_response(r, r.function_list(withcode=True), res, resp3_res)
 
     @pytest.mark.onlycluster
     def test_function_list_on_cluster(self, r):
         r.function_load(f"#!{engine} name={lib} \n {function}")
         function_list = [
             [
                 b"library_name",
```

### Comparing `redis-5.0.0b4/tests/test_graph.py` & `redis-5.0.0rc1/tests/test_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from unittest.mock import patch
 
 import pytest
-
+from redis import Redis
 from redis.commands.graph import Edge, Node, Path
 from redis.commands.graph.execution_plan import Operation
 from redis.commands.graph.query_result import (
     CACHED_EXECUTION,
     INDICES_CREATED,
     INDICES_DELETED,
     INTERNAL_EXECUTION_TIME,
@@ -16,21 +16,22 @@
     PROPERTIES_REMOVED,
     PROPERTIES_SET,
     RELATIONSHIPS_CREATED,
     RELATIONSHIPS_DELETED,
     QueryResult,
 )
 from redis.exceptions import ResponseError
-from tests.conftest import skip_if_redis_enterprise
+from tests.conftest import _get_client, skip_if_redis_enterprise
 
 
 @pytest.fixture
-def client(modclient):
-    modclient.flushdb()
-    return modclient
+def client(request):
+    r = _get_client(Redis, request, decode_responses=True)
+    r.flushdb()
+    return r
 
 
 @pytest.mark.redismod
 def test_bulk(client):
     with pytest.raises(NotImplementedError):
         client.graph().bulk()
         client.graph().bulk(foo="bar!")
@@ -288,14 +289,15 @@
 
     results = client.graph().slowlog()
     assert results[0][1] == "GRAPH.QUERY"
     assert results[0][2] == create_query
 
 
 @pytest.mark.redismod
+@pytest.mark.xfail(strict=False)
 def test_query_timeout(client):
     # Build a sample graph with 1000 nodes.
     client.graph().query("UNWIND range(0,1000) as val CREATE ({v: val})")
     # Issue a long-running query with a 1-millisecond timeout.
     with pytest.raises(ResponseError):
         client.graph().query("MATCH (a), (b), (c), (d) RETURN *", timeout=1)
         assert False is False
```

### Comparing `redis-5.0.0b4/tests/test_graph_utils/test_edge.py` & `redis-5.0.0rc1/tests/test_graph_utils/test_edge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from redis.commands.graph import edge, node
 
 
 @pytest.mark.redismod
 def test_init():
 
     with pytest.raises(AssertionError):
```

### Comparing `redis-5.0.0b4/tests/test_graph_utils/test_node.py` & `redis-5.0.0rc1/tests/test_graph_utils/test_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from redis.commands.graph import node
 
 
 @pytest.fixture
 def fixture():
     no_args = node.Node()
     no_props = node.Node(node_id=1, alias="alias", label="l")
```

### Comparing `redis-5.0.0b4/tests/test_graph_utils/test_path.py` & `redis-5.0.0rc1/tests/test_graph_utils/test_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from redis.commands.graph import edge, node, path
 
 
 @pytest.mark.redismod
 def test_init():
     with pytest.raises(TypeError):
         path.Path(None, None)
```

### Comparing `redis-5.0.0b4/tests/test_helpers.py` & `redis-5.0.0rc1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/tests/test_json.py` & `redis-5.0.0rc1/tests/test_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,63 @@
 import pytest
-
 import redis
-from redis import exceptions
+from redis import Redis, exceptions
 from redis.commands.json.decoders import decode_list, unstring
 from redis.commands.json.path import Path
 
-from .conftest import skip_ifmodversion_lt
+from .conftest import _get_client, assert_resp_response, skip_ifmodversion_lt
 
 
 @pytest.fixture
-def client(modclient):
-    modclient.flushdb()
-    return modclient
+def client(request):
+    r = _get_client(Redis, request, decode_responses=True)
+    r.flushdb()
+    return r
 
 
 @pytest.mark.redismod
 def test_json_setbinarykey(client):
     d = {"hello": "world", b"some": "value"}
     with pytest.raises(TypeError):
         client.json().set("somekey", Path.root_path(), d)
     assert client.json().set("somekey", Path.root_path(), d, decode_keys=True)
 
 
 @pytest.mark.redismod
 def test_json_setgetdeleteforget(client):
     assert client.json().set("foo", Path.root_path(), "bar")
-    assert client.json().get("foo") == "bar"
+    assert_resp_response(client, client.json().get("foo"), "bar", [["bar"]])
     assert client.json().get("baz") is None
     assert client.json().delete("foo") == 1
     assert client.json().forget("foo") == 0  # second delete
     assert client.exists("foo") == 0
 
 
 @pytest.mark.redismod
 def test_jsonget(client):
     client.json().set("foo", Path.root_path(), "bar")
-    assert client.json().get("foo") == "bar"
+    assert_resp_response(client, client.json().get("foo"), "bar", [["bar"]])
 
 
 @pytest.mark.redismod
 def test_json_get_jset(client):
     assert client.json().set("foo", Path.root_path(), "bar")
-    assert "bar" == client.json().get("foo")
+    assert_resp_response(client, client.json().get("foo"), "bar", [["bar"]])
     assert client.json().get("baz") is None
     assert 1 == client.json().delete("foo")
     assert client.exists("foo") == 0
 
 
 @pytest.mark.redismod
 def test_nonascii_setgetdelete(client):
     assert client.json().set("notascii", Path.root_path(), "hyvää-élève")
-    assert "hyvää-élève" == client.json().get("notascii", no_escape=True)
+    res = "hyvää-élève"
+    assert_resp_response(
+        client, client.json().get("notascii", no_escape=True), res, [[res]]
+    )
     assert 1 == client.json().delete("notascii")
     assert client.exists("notascii") == 0
 
 
 @pytest.mark.redismod
 def test_jsonsetexistentialmodifiersshouldsucceed(client):
     obj = {"foo": "bar"}
@@ -83,40 +86,54 @@
 
 
 @pytest.mark.redismod
 @skip_ifmodversion_lt("99.99.99", "ReJSON")  # todo: update after the release
 def test_clear(client):
     client.json().set("arr", Path.root_path(), [0, 1, 2, 3, 4])
     assert 1 == client.json().clear("arr", Path.root_path())
-    assert [] == client.json().get("arr")
+    assert_resp_response(client, client.json().get("arr"), [], [[[]]])
 
 
 @pytest.mark.redismod
 def test_type(client):
     client.json().set("1", Path.root_path(), 1)
-    assert "integer" == client.json().type("1", Path.root_path())
-    assert "integer" == client.json().type("1")
+    assert_resp_response(
+        client, client.json().type("1", Path.root_path()), "integer", ["integer"]
+    )
+    assert_resp_response(client, client.json().type("1"), "integer", ["integer"])
 
 
 @pytest.mark.redismod
 def test_numincrby(client):
     client.json().set("num", Path.root_path(), 1)
-    assert 2 == client.json().numincrby("num", Path.root_path(), 1)
-    assert 2.5 == client.json().numincrby("num", Path.root_path(), 0.5)
-    assert 1.25 == client.json().numincrby("num", Path.root_path(), -1.25)
+    assert_resp_response(
+        client, client.json().numincrby("num", Path.root_path(), 1), 2, [2]
+    )
+    assert_resp_response(
+        client, client.json().numincrby("num", Path.root_path(), 0.5), 2.5, [2.5]
+    )
+    assert_resp_response(
+        client, client.json().numincrby("num", Path.root_path(), -1.25), 1.25, [1.25]
+    )
 
 
 @pytest.mark.redismod
 def test_nummultby(client):
     client.json().set("num", Path.root_path(), 1)
 
     with pytest.deprecated_call():
-        assert 2 == client.json().nummultby("num", Path.root_path(), 2)
-        assert 5 == client.json().nummultby("num", Path.root_path(), 2.5)
-        assert 2.5 == client.json().nummultby("num", Path.root_path(), 0.5)
+        assert_resp_response(
+            client, client.json().nummultby("num", Path.root_path(), 2), 2, [2]
+        )
+        assert_resp_response(
+            client, client.json().nummultby("num", Path.root_path(), 2.5), 5, [5]
+        )
+        assert_resp_response(
+            client, client.json().nummultby("num", Path.root_path(), 0.5), 2.5, [2.5]
+        )
 
 
 @pytest.mark.redismod
 @skip_ifmodversion_lt("99.99.99", "ReJSON")  # todo: update after the release
 def test_toggle(client):
     client.json().set("bool", Path.root_path(), False)
     assert client.json().toggle("bool", Path.root_path())
@@ -127,15 +144,17 @@
         client.json().toggle("num", Path.root_path())
 
 
 @pytest.mark.redismod
 def test_strappend(client):
     client.json().set("jsonkey", Path.root_path(), "foo")
     assert 6 == client.json().strappend("jsonkey", "bar")
-    assert "foobar" == client.json().get("jsonkey", Path.root_path())
+    assert_resp_response(
+        client, client.json().get("jsonkey", Path.root_path()), "foobar", [["foobar"]]
+    )
 
 
 # @pytest.mark.redismod
 # def test_debug(client):
 #    client.json().set("str", Path.root_path(), "foo")
 #    assert 24 == client.json().debug("MEMORY", "str", Path.root_path())
 #    assert 24 == client.json().debug("MEMORY", "str")
@@ -173,20 +192,22 @@
     assert -1 == client.json().arrindex("arr", Path.root_path(), 4, start=1, stop=3)
 
 
 @pytest.mark.redismod
 def test_arrinsert(client):
     client.json().set("arr", Path.root_path(), [0, 4])
     assert 5 - -client.json().arrinsert("arr", Path.root_path(), 1, *[1, 2, 3])
-    assert [0, 1, 2, 3, 4] == client.json().get("arr")
+    res = [0, 1, 2, 3, 4]
+    assert_resp_response(client, client.json().get("arr"), res, [[res]])
 
     # test prepends
     client.json().set("val2", Path.root_path(), [5, 6, 7, 8, 9])
     client.json().arrinsert("val2", Path.root_path(), 0, ["some", "thing"])
-    assert client.json().get("val2") == [["some", "thing"], 5, 6, 7, 8, 9]
+    res = [["some", "thing"], 5, 6, 7, 8, 9]
+    assert_resp_response(client, client.json().get("val2"), res, [[res]])
 
 
 @pytest.mark.redismod
 def test_arrlen(client):
     client.json().set("arr", Path.root_path(), [0, 1, 2, 3, 4])
     assert 5 == client.json().arrlen("arr", Path.root_path())
     assert 5 == client.json().arrlen("arr")
@@ -196,30 +217,30 @@
 @pytest.mark.redismod
 def test_arrpop(client):
     client.json().set("arr", Path.root_path(), [0, 1, 2, 3, 4])
     assert 4 == client.json().arrpop("arr", Path.root_path(), 4)
     assert 3 == client.json().arrpop("arr", Path.root_path(), -1)
     assert 2 == client.json().arrpop("arr", Path.root_path())
     assert 0 == client.json().arrpop("arr", Path.root_path(), 0)
-    assert [1] == client.json().get("arr")
+    assert_resp_response(client, client.json().get("arr"), [1], [[[1]]])
 
     # test out of bounds
     client.json().set("arr", Path.root_path(), [0, 1, 2, 3, 4])
     assert 4 == client.json().arrpop("arr", Path.root_path(), 99)
 
     # none test
     client.json().set("arr", Path.root_path(), [])
     assert client.json().arrpop("arr") is None
 
 
 @pytest.mark.redismod
 def test_arrtrim(client):
     client.json().set("arr", Path.root_path(), [0, 1, 2, 3, 4])
     assert 3 == client.json().arrtrim("arr", Path.root_path(), 1, 3)
-    assert [1, 2, 3] == client.json().get("arr")
+    assert_resp_response(client, client.json().get("arr"), [1, 2, 3], [[[1, 2, 3]]])
 
     # <0 test, should be 0 equivalent
     client.json().set("arr", Path.root_path(), [0, 1, 2, 3, 4])
     assert 0 == client.json().arrtrim("arr", Path.root_path(), -1, 3)
 
     # testing stop > end
     client.json().set("arr", Path.root_path(), [0, 1, 2, 3, 4])
@@ -273,45 +294,45 @@
 
 @pytest.mark.redismod
 def test_json_commands_in_pipeline(client):
     p = client.json().pipeline()
     p.set("foo", Path.root_path(), "bar")
     p.get("foo")
     p.delete("foo")
-    assert [True, "bar", 1] == p.execute()
+    assert_resp_response(client, p.execute(), [True, "bar", 1], [True, [["bar"]], 1])
     assert client.keys() == []
     assert client.get("foo") is None
 
     # now with a true, json object
     client.flushdb()
     p = client.json().pipeline()
     d = {"hello": "world", "oh": "snap"}
     with pytest.deprecated_call():
         p.jsonset("foo", Path.root_path(), d)
         p.jsonget("foo")
     p.exists("notarealkey")
     p.delete("foo")
-    assert [True, d, 0, 1] == p.execute()
+    assert_resp_response(client, p.execute(), [True, d, 0, 1], [True, [[d]], 0, 1])
     assert client.keys() == []
     assert client.get("foo") is None
 
 
 @pytest.mark.redismod
 def test_json_delete_with_dollar(client):
     doc1 = {"a": 1, "nested": {"a": 2, "b": 3}}
     assert client.json().set("doc1", "$", doc1)
     assert client.json().delete("doc1", "$..a") == 2
-    r = client.json().get("doc1", "$")
-    assert r == [{"nested": {"b": 3}}]
+    res = [{"nested": {"b": 3}}]
+    assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
 
     doc2 = {"a": {"a": 2, "b": 3}, "b": ["a", "b"], "nested": {"b": [True, "a", "b"]}}
     assert client.json().set("doc2", "$", doc2)
     assert client.json().delete("doc2", "$..a") == 1
-    res = client.json().get("doc2", "$")
-    assert res == [{"nested": {"b": [True, "a", "b"]}, "b": ["a", "b"]}]
+    res = [{"nested": {"b": [True, "a", "b"]}, "b": ["a", "b"]}]
+    assert_resp_response(client, client.json().get("doc2", "$"), res, [res])
 
     doc3 = [
         {
             "ciao": ["non ancora"],
             "nested": [
                 {"ciao": [1, "a"]},
                 {"ciao": [2, "a"]},
@@ -334,37 +355,36 @@
                     {"ciaoc": [3, "non", "ciao"]},
                     {},
                     {"e": [5, "non", "ciao"]},
                 ],
             }
         ]
     ]
-    res = client.json().get("doc3", "$")
-    assert res == doc3val
+    assert_resp_response(client, client.json().get("doc3", "$"), doc3val, [doc3val])
 
     # Test default path
     assert client.json().delete("doc3") == 1
     assert client.json().get("doc3", "$") is None
 
     client.json().delete("not_a_document", "..a")
 
 
 @pytest.mark.redismod
 def test_json_forget_with_dollar(client):
     doc1 = {"a": 1, "nested": {"a": 2, "b": 3}}
     assert client.json().set("doc1", "$", doc1)
     assert client.json().forget("doc1", "$..a") == 2
-    r = client.json().get("doc1", "$")
-    assert r == [{"nested": {"b": 3}}]
+    res = [{"nested": {"b": 3}}]
+    assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
 
     doc2 = {"a": {"a": 2, "b": 3}, "b": ["a", "b"], "nested": {"b": [True, "a", "b"]}}
     assert client.json().set("doc2", "$", doc2)
     assert client.json().forget("doc2", "$..a") == 1
-    res = client.json().get("doc2", "$")
-    assert res == [{"nested": {"b": [True, "a", "b"]}, "b": ["a", "b"]}]
+    res = [{"nested": {"b": [True, "a", "b"]}, "b": ["a", "b"]}]
+    assert_resp_response(client, client.json().get("doc2", "$"), res, [res])
 
     doc3 = [
         {
             "ciao": ["non ancora"],
             "nested": [
                 {"ciao": [1, "a"]},
                 {"ciao": [2, "a"]},
@@ -387,16 +407,15 @@
                     {"ciaoc": [3, "non", "ciao"]},
                     {},
                     {"e": [5, "non", "ciao"]},
                 ],
             }
         ]
     ]
-    res = client.json().get("doc3", "$")
-    assert res == doc3val
+    assert_resp_response(client, client.json().get("doc3", "$"), doc3val, [doc3val])
 
     # Test default path
     assert client.json().forget("doc3") == 1
     assert client.json().get("doc3", "$") is None
 
     client.json().forget("not_a_document", "..a")
 
@@ -411,16 +430,18 @@
     )
     client.json().set(
         "doc2",
         "$",
         {"a": 4, "b": 5, "nested": {"a": 6}, "c": None, "nested2": {"a": [None]}},
     )
     # Compare also to single JSON.GET
-    assert client.json().get("doc1", "$..a") == [1, 3, None]
-    assert client.json().get("doc2", "$..a") == [4, 6, [None]]
+    res = [1, 3, None]
+    assert_resp_response(client, client.json().get("doc1", "$..a"), res, [res])
+    res = [4, 6, [None]]
+    assert_resp_response(client, client.json().get("doc2", "$..a"), res, [res])
 
     # Test mget with single path
     client.json().mget("doc1", "$..a") == [1, 3, None]
     # Test mget with multi path
     client.json().mget(["doc1", "doc2"], "$..a") == [[1, 3, None], [4, 6, [None]]]
 
     # Test missing key
@@ -479,33 +500,31 @@
 
     client.json().set(
         "doc1", "$", {"a": "foo", "nested1": {"a": "hello"}, "nested2": {"a": 31}}
     )
     # Test multi
     client.json().strappend("doc1", "bar", "$..a") == [6, 8, None]
 
-    client.json().get("doc1", "$") == [
-        {"a": "foobar", "nested1": {"a": "hellobar"}, "nested2": {"a": 31}}
-    ]
+    # res = [{"a": "foobar", "nested1": {"a": "hellobar"}, "nested2": {"a": 31}}]
+    # assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
+
     # Test single
     client.json().strappend("doc1", "baz", "$.nested1.a") == [11]
 
-    client.json().get("doc1", "$") == [
-        {"a": "foobar", "nested1": {"a": "hellobarbaz"}, "nested2": {"a": 31}}
-    ]
+    # res = [{"a": "foobar", "nested1": {"a": "hellobarbaz"}, "nested2": {"a": 31}}]
+    # assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
 
     # Test missing key
     with pytest.raises(exceptions.ResponseError):
         client.json().strappend("non_existing_doc", "$..a", "err")
 
     # Test multi
     client.json().strappend("doc1", "bar", ".*.a") == 8
-    client.json().get("doc1", "$") == [
-        {"a": "foo", "nested1": {"a": "hellobar"}, "nested2": {"a": 31}}
-    ]
+    # res = [{"a": "foo", "nested1": {"a": "hellobar"}, "nested2": {"a": 31}}]
+    # assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
 
     # Test missing path
     with pytest.raises(exceptions.ResponseError):
         client.json().strappend("doc1", "piu")
 
 
 @pytest.mark.redismod
@@ -539,31 +558,33 @@
             "a": ["foo"],
             "nested1": {"a": ["hello", None, "world"]},
             "nested2": {"a": 31},
         },
     )
     # Test multi
     client.json().arrappend("doc1", "$..a", "bar", "racuda") == [3, 5, None]
-    assert client.json().get("doc1", "$") == [
+    res = [
         {
             "a": ["foo", "bar", "racuda"],
             "nested1": {"a": ["hello", None, "world", "bar", "racuda"]},
             "nested2": {"a": 31},
         }
     ]
+    assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
 
     # Test single
     assert client.json().arrappend("doc1", "$.nested1.a", "baz") == [6]
-    assert client.json().get("doc1", "$") == [
+    res = [
         {
             "a": ["foo", "bar", "racuda"],
             "nested1": {"a": ["hello", None, "world", "bar", "racuda", "baz"]},
             "nested2": {"a": 31},
         }
     ]
+    assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
 
     # Test missing key
     with pytest.raises(exceptions.ResponseError):
         client.json().arrappend("non_existing_doc", "$..a")
 
     # Test legacy
     client.json().set(
@@ -574,30 +595,33 @@
             "nested1": {"a": ["hello", None, "world"]},
             "nested2": {"a": 31},
         },
     )
     # Test multi (all paths are updated, but return result of last path)
     assert client.json().arrappend("doc1", "..a", "bar", "racuda") == 5
 
-    assert client.json().get("doc1", "$") == [
+    res = [
         {
             "a": ["foo", "bar", "racuda"],
             "nested1": {"a": ["hello", None, "world", "bar", "racuda"]},
             "nested2": {"a": 31},
         }
     ]
+    assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
+
     # Test single
     assert client.json().arrappend("doc1", ".nested1.a", "baz") == 6
-    assert client.json().get("doc1", "$") == [
+    res = [
         {
             "a": ["foo", "bar", "racuda"],
             "nested1": {"a": ["hello", None, "world", "bar", "racuda", "baz"]},
             "nested2": {"a": 31},
         }
     ]
+    assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
 
     # Test missing key
     with pytest.raises(exceptions.ResponseError):
         client.json().arrappend("non_existing_doc", "$..a")
 
 
 @pytest.mark.redismod
@@ -610,30 +634,33 @@
             "nested1": {"a": ["hello", None, "world"]},
             "nested2": {"a": 31},
         },
     )
     # Test multi
     assert client.json().arrinsert("doc1", "$..a", "1", "bar", "racuda") == [3, 5, None]
 
-    assert client.json().get("doc1", "$") == [
+    res = [
         {
             "a": ["foo", "bar", "racuda"],
             "nested1": {"a": ["hello", "bar", "racuda", None, "world"]},
             "nested2": {"a": 31},
         }
     ]
+    assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
+
     # Test single
     assert client.json().arrinsert("doc1", "$.nested1.a", -2, "baz") == [6]
-    assert client.json().get("doc1", "$") == [
+    res = [
         {
             "a": ["foo", "bar", "racuda"],
             "nested1": {"a": ["hello", "bar", "racuda", "baz", None, "world"]},
             "nested2": {"a": 31},
         }
     ]
+    assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
 
     # Test missing key
     with pytest.raises(exceptions.ResponseError):
         client.json().arrappend("non_existing_doc", "$..a")
 
 
 @pytest.mark.redismod
@@ -697,17 +724,16 @@
             "nested2": {"a": 31},
         },
     )
 
     # # # Test multi
     assert client.json().arrpop("doc1", "$..a", 1) == ['"foo"', None, None]
 
-    assert client.json().get("doc1", "$") == [
-        {"a": [], "nested1": {"a": ["hello", "world"]}, "nested2": {"a": 31}}
-    ]
+    res = [{"a": [], "nested1": {"a": ["hello", "world"]}, "nested2": {"a": 31}}]
+    assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
 
     # Test missing key
     with pytest.raises(exceptions.ResponseError):
         client.json().arrpop("non_existing_doc", "..a")
 
     # # Test legacy
     client.json().set(
@@ -717,17 +743,16 @@
             "a": ["foo"],
             "nested1": {"a": ["hello", None, "world"]},
             "nested2": {"a": 31},
         },
     )
     # Test multi (all paths are updated, but return result of last path)
     client.json().arrpop("doc1", "..a", "1") is None
-    assert client.json().get("doc1", "$") == [
-        {"a": [], "nested1": {"a": ["hello", "world"]}, "nested2": {"a": 31}}
-    ]
+    res = [{"a": [], "nested1": {"a": ["hello", "world"]}, "nested2": {"a": 31}}]
+    assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
 
     # # Test missing key
     with pytest.raises(exceptions.ResponseError):
         client.json().arrpop("non_existing_doc", "..a")
 
 
 @pytest.mark.redismod
@@ -740,27 +765,25 @@
             "a": ["foo"],
             "nested1": {"a": ["hello", None, "world"]},
             "nested2": {"a": 31},
         },
     )
     # Test multi
     assert client.json().arrtrim("doc1", "$..a", "1", -1) == [0, 2, None]
-    assert client.json().get("doc1", "$") == [
-        {"a": [], "nested1": {"a": [None, "world"]}, "nested2": {"a": 31}}
-    ]
+    res = [{"a": [], "nested1": {"a": [None, "world"]}, "nested2": {"a": 31}}]
+    assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
 
     assert client.json().arrtrim("doc1", "$..a", "1", "1") == [0, 1, None]
-    assert client.json().get("doc1", "$") == [
-        {"a": [], "nested1": {"a": ["world"]}, "nested2": {"a": 31}}
-    ]
+    res = [{"a": [], "nested1": {"a": ["world"]}, "nested2": {"a": 31}}]
+    assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
+
     # Test single
     assert client.json().arrtrim("doc1", "$.nested1.a", 1, 0) == [0]
-    assert client.json().get("doc1", "$") == [
-        {"a": [], "nested1": {"a": []}, "nested2": {"a": 31}}
-    ]
+    res = [{"a": [], "nested1": {"a": []}, "nested2": {"a": 31}}]
+    assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
 
     # Test missing key
     with pytest.raises(exceptions.ResponseError):
         client.json().arrtrim("non_existing_doc", "..a", "0", 1)
 
     # Test legacy
     client.json().set(
@@ -774,17 +797,16 @@
     )
 
     # Test multi (all paths are updated, but return result of last path)
     assert client.json().arrtrim("doc1", "..a", "1", "-1") == 2
 
     # Test single
     assert client.json().arrtrim("doc1", ".nested1.a", "1", "1") == 1
-    assert client.json().get("doc1", "$") == [
-        {"a": [], "nested1": {"a": ["world"]}, "nested2": {"a": 31}}
-    ]
+    res = [{"a": [], "nested1": {"a": ["world"]}, "nested2": {"a": 31}}]
+    assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
 
     # Test missing key
     with pytest.raises(exceptions.ResponseError):
         client.json().arrtrim("non_existing_doc", "..a", 1, 1)
 
 
 @pytest.mark.redismod
@@ -874,21 +896,25 @@
 
 
 @pytest.mark.redismod
 def test_type_dollar(client):
     jdata, jtypes = load_types_data("a")
     client.json().set("doc1", "$", jdata)
     # Test multi
-    assert client.json().type("doc1", "$..a") == jtypes
+    assert_resp_response(client, client.json().type("doc1", "$..a"), jtypes, [jtypes])
 
     # Test single
-    assert client.json().type("doc1", "$.nested2.a") == [jtypes[1]]
+    assert_resp_response(
+        client, client.json().type("doc1", "$.nested2.a"), [jtypes[1]], [[jtypes[1]]]
+    )
 
     # Test missing key
-    assert client.json().type("non_existing_doc", "..a") is None
+    assert_resp_response(
+        client, client.json().type("non_existing_doc", "..a"), None, [None]
+    )
 
 
 @pytest.mark.redismod
 def test_clear_dollar(client):
     client.json().set(
         "doc1",
         "$",
@@ -898,42 +924,44 @@
             "nested2": {"a": "claro"},
             "nested3": {"a": {"baz": 50}},
         },
     )
     # Test multi
     assert client.json().clear("doc1", "$..a") == 3
 
-    assert client.json().get("doc1", "$") == [
+    res = [
         {"nested1": {"a": {}}, "a": [], "nested2": {"a": "claro"}, "nested3": {"a": {}}}
     ]
+    assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
 
     # Test single
     client.json().set(
         "doc1",
         "$",
         {
             "nested1": {"a": {"foo": 10, "bar": 20}},
             "a": ["foo"],
             "nested2": {"a": "claro"},
             "nested3": {"a": {"baz": 50}},
         },
     )
     assert client.json().clear("doc1", "$.nested1.a") == 1
-    assert client.json().get("doc1", "$") == [
+    res = [
         {
             "nested1": {"a": {}},
             "a": ["foo"],
             "nested2": {"a": "claro"},
             "nested3": {"a": {"baz": 50}},
         }
     ]
+    assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
 
     # Test missing path (defaults to root)
     assert client.json().clear("doc1") == 1
-    assert client.json().get("doc1", "$") == [{}]
+    assert_resp_response(client, client.json().get("doc1", "$"), [{}], [[{}]])
 
     # Test missing key
     with pytest.raises(exceptions.ResponseError):
         client.json().clear("non_existing_doc", "$..a")
 
 
 @pytest.mark.redismod
@@ -946,22 +974,23 @@
             "nested1": {"a": False},
             "nested2": {"a": 31},
             "nested3": {"a": True},
         },
     )
     # Test multi
     assert client.json().toggle("doc1", "$..a") == [None, 1, None, 0]
-    assert client.json().get("doc1", "$") == [
+    res = [
         {
             "a": ["foo"],
             "nested1": {"a": True},
             "nested2": {"a": 31},
             "nested3": {"a": False},
         }
     ]
+    assert_resp_response(client, client.json().get("doc1", "$"), res, [res])
 
     # Test missing key
     with pytest.raises(exceptions.ResponseError):
         client.json().toggle("non_existing_doc", "$..a")
 
 
 # @pytest.mark.redismod
@@ -1029,15 +1058,15 @@
                 "A2_B4": {"A2_B4_C1": "bar"},
             }
         },
     }
     client.json().set("doc1", "$", data)
     # Test multi
     res = client.json().resp("doc1", "$..a")
-    assert res == [
+    resp2 = [
         [
             "{",
             "A1_B1",
             10,
             "A1_B2",
             "false",
             "A1_B3",
@@ -1085,18 +1114,75 @@
                 "A2_B3_C3",
                 ["[", 2],
             ],
             "A2_B4",
             ["{", "A2_B4_C1", "bar"],
         ],
     ]
+    resp3 = [
+        [
+            "{",
+            "A1_B1",
+            10,
+            "A1_B2",
+            "false",
+            "A1_B3",
+            [
+                "{",
+                "A1_B3_C1",
+                None,
+                "A1_B3_C2",
+                [
+                    "[",
+                    "A1_B3_C2_D1_1",
+                    "A1_B3_C2_D1_2",
+                    -19.5,
+                    "A1_B3_C2_D1_4",
+                    "A1_B3_C2_D1_5",
+                    ["{", "A1_B3_C2_D1_6_E1", "true"],
+                ],
+                "A1_B3_C3",
+                ["[", 1],
+            ],
+            "A1_B4",
+            ["{", "A1_B4_C1", "foo"],
+        ],
+        [
+            "{",
+            "A2_B1",
+            20,
+            "A2_B2",
+            "false",
+            "A2_B3",
+            [
+                "{",
+                "A2_B3_C1",
+                None,
+                "A2_B3_C2",
+                [
+                    "[",
+                    "A2_B3_C2_D1_1",
+                    "A2_B3_C2_D1_2",
+                    -37.5,
+                    "A2_B3_C2_D1_4",
+                    "A2_B3_C2_D1_5",
+                    ["{", "A2_B3_C2_D1_6_E1", "false"],
+                ],
+                "A2_B3_C3",
+                ["[", 2],
+            ],
+            "A2_B4",
+            ["{", "A2_B4_C1", "bar"],
+        ],
+    ]
+    assert_resp_response(client, res, resp2, resp3)
 
     # Test single
-    resSingle = client.json().resp("doc1", "$.L1.a")
-    assert resSingle == [
+    res = client.json().resp("doc1", "$.L1.a")
+    resp2 = [
         [
             "{",
             "A1_B1",
             10,
             "A1_B2",
             "false",
             "A1_B3",
@@ -1117,14 +1203,44 @@
                 "A1_B3_C3",
                 ["[", 1],
             ],
             "A1_B4",
             ["{", "A1_B4_C1", "foo"],
         ]
     ]
+    resp3 = [
+        [
+            "{",
+            "A1_B1",
+            10,
+            "A1_B2",
+            "false",
+            "A1_B3",
+            [
+                "{",
+                "A1_B3_C1",
+                None,
+                "A1_B3_C2",
+                [
+                    "[",
+                    "A1_B3_C2_D1_1",
+                    "A1_B3_C2_D1_2",
+                    -19.5,
+                    "A1_B3_C2_D1_4",
+                    "A1_B3_C2_D1_5",
+                    ["{", "A1_B3_C2_D1_6_E1", "true"],
+                ],
+                "A1_B3_C3",
+                ["[", 1],
+            ],
+            "A1_B4",
+            ["{", "A1_B4_C1", "foo"],
+        ]
+    ]
+    assert_resp_response(client, res, resp2, resp3)
 
     # Test missing path
     client.json().resp("doc1", "$.nowhere")
 
     # Test missing key
     # with pytest.raises(exceptions.ResponseError):
     client.json().resp("non_existing_doc", "$..a")
@@ -1171,18 +1287,21 @@
                     },
                 ],
                 "bicycle": {"color": "red", "price": 19.95},
             }
         },
     )
 
-    assert client.json().get("store", "$.store.book[?(@.price<10)].size") == [
-        [10, 20, 30, 40],
-        [5, 10, 20, 30],
-    ]
+    assert_resp_response(
+        client,
+        client.json().get("store", "$.store.book[?(@.price<10)].size"),
+        [[10, 20, 30, 40], [5, 10, 20, 30]],
+        [[[10, 20, 30, 40], [5, 10, 20, 30]]],
+    )
+
     assert client.json().arrindex(
         "store", "$.store.book[?(@.price<10)].size", "20"
     ) == [-1, -1]
 
     # Test index of int scalar in multi values
     client.json().set(
         "test_num",
@@ -1195,21 +1314,22 @@
             [
                 {"nested41_not_arr": {"arr_renamed": [1, 2, 3]}},
                 {"nested42_empty_arr": {"arr": []}},
             ],
         ],
     )
 
-    assert client.json().get("test_num", "$..arr") == [
+    res = [
         [0, 1, 3.0, 3, 2, 1, 0, 3],
         [5, 4, 3, 2, 1, 0, 1, 2, 3.0, 2, 4, 5],
         [2, 4, 6],
         "3",
         [],
     ]
+    assert_resp_response(client, client.json().get("test_num", "$..arr"), res, [res])
 
     assert client.json().arrindex("test_num", "$..arr", 3) == [3, 2, -1, None, -1]
 
     # Test index of double scalar in multi values
     assert client.json().arrindex("test_num", "$..arr", 3.0) == [2, 8, -1, None, -1]
 
     # Test index of string scalar in multi values
@@ -1227,21 +1347,22 @@
             {"nested3_scalar": {"arr": "3"}},
             [
                 {"nested41_arr": {"arr_renamed": [1, "baz", 3]}},
                 {"nested42_empty_arr": {"arr": []}},
             ],
         ],
     )
-    assert client.json().get("test_string", "$..arr") == [
+    res = [
         ["bazzz", "bar", 2, "baz", 2, "ba", "baz", 3],
         [None, "baz2", "buzz", 2, 1, 0, 1, "2", "baz", 2, 4, 5],
         ["baz2", 4, 6],
         "3",
         [],
     ]
+    assert_resp_response(client, client.json().get("test_string", "$..arr"), res, [res])
 
     assert client.json().arrindex("test_string", "$..arr", "baz") == [
         3,
         8,
         -1,
         None,
         -1,
@@ -1319,21 +1440,22 @@
             {"nested3_scalar": {"arr": None}},
             [
                 {"nested41_arr": {"arr_renamed": [1, None, 3]}},
                 {"nested42_empty_arr": {"arr": []}},
             ],
         ],
     )
-    assert client.json().get("test_None", "$..arr") == [
+    res = [
         ["bazzz", "None", 2, None, 2, "ba", "baz", 3],
         ["zaz", "baz2", "buzz", 2, 1, 0, 1, "2", None, 2, 4, 5],
         ["None", 4, 6],
         None,
         [],
     ]
+    assert_resp_response(client, client.json().get("test_None", "$..arr"), res, [res])
 
     # Test with none-scalar value
     assert client.json().arrindex(
         "test_None", "$..nested42_empty_arr.arr", {"arr": []}
     ) == [-1]
 
     # Test legacy (path begins with dot)
@@ -1366,15 +1488,15 @@
 def test_custom_decoder(client):
     import json
 
     import ujson
 
     cj = client.json(encoder=ujson, decoder=ujson)
     assert cj.set("foo", Path.root_path(), "bar")
-    assert "bar" == cj.get("foo")
+    assert_resp_response(client, cj.get("foo"), "bar", [["bar"]])
     assert cj.get("baz") is None
     assert 1 == cj.delete("foo")
     assert client.exists("foo") == 0
     assert not isinstance(cj.__encoder__, json.JSONEncoder)
     assert not isinstance(cj.__decoder__, json.JSONDecoder)
 
 
@@ -1388,15 +1510,15 @@
     with open(jsonfile.name, "w+") as fp:
         fp.write(json.dumps(obj))
 
     nojsonfile = tempfile.NamedTemporaryFile()
     nojsonfile.write(b"Hello World")
 
     assert client.json().set_file("test", Path.root_path(), jsonfile.name)
-    assert client.json().get("test") == obj
+    assert_resp_response(client, client.json().get("test"), obj, [[obj]])
     with pytest.raises(json.JSONDecodeError):
         client.json().set_file("test2", Path.root_path(), nojsonfile.name)
 
 
 @pytest.mark.redismod
 def test_set_path(client):
     import json
@@ -1410,8 +1532,11 @@
     with open(jsonfile, "w+") as fp:
         fp.write(json.dumps({"hello": "world"}))
     with open(nojsonfile, "a+") as fp:
         fp.write("hello")
 
     result = {jsonfile: True, nojsonfile: False}
     assert client.json().set_path(Path.root_path(), root) == result
-    assert client.json().get(jsonfile.rsplit(".")[0]) == {"hello": "world"}
+    res = {"hello": "world"}
+    assert_resp_response(
+        client, client.json().get(jsonfile.rsplit(".")[0]), res, [[res]]
+    )
```

### Comparing `redis-5.0.0b4/tests/test_lock.py` & `redis-5.0.0rc1/tests/test_lock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import time
 
 import pytest
-
 from redis.client import Redis
 from redis.exceptions import LockError, LockNotOwnedError
 from redis.lock import Lock
 
 from .conftest import _get_client
```

### Comparing `redis-5.0.0b4/tests/test_monitor.py` & `redis-5.0.0rc1/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/tests/test_multiprocessing.py` & `redis-5.0.0rc1/tests/test_multiprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import contextlib
 import multiprocessing
 
 import pytest
-
 import redis
 from redis.connection import Connection, ConnectionPool
 from redis.exceptions import ConnectionError
 
 from .conftest import _get_client
```

### Comparing `redis-5.0.0b4/tests/test_pipeline.py` & `redis-5.0.0rc1/tests/test_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 import redis
 
 from .conftest import skip_if_server_version_lt, wait_for_command
 
 
 class TestPipeline:
     def test_pipeline_is_true(self, r):
```

### Comparing `redis-5.0.0b4/tests/test_pubsub.py` & `redis-5.0.0rc1/tests/test_pubsub.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import threading
 import time
 from collections import defaultdict
 from unittest import mock
 from unittest.mock import patch
 
 import pytest
-
 import redis
 from redis.exceptions import ConnectionError
 from redis.utils import HIREDIS_AVAILABLE
 
 from .conftest import (
     _get_client,
     is_resp2_connection,
@@ -604,14 +603,27 @@
         p.subscribe("foo")
         assert wait_for_message(p) is None
         assert self.message == ["my handler", [b"subscribe", b"foo", 1]]
         assert r.publish("foo", "test message") == 1
         assert wait_for_message(p) is None
         assert self.message == ["my handler", [b"message", b"foo", b"test message"]]
 
+    @pytest.mark.skipif(HIREDIS_AVAILABLE, reason="PythonParser only")
+    @skip_if_server_version_lt("7.0.0")
+    def test_push_handler_sharded_pubsub(self, r):
+        if is_resp2_connection(r):
+            return
+        p = r.pubsub(push_handler_func=self.my_handler)
+        p.ssubscribe("foo")
+        assert wait_for_message(p, func=p.get_sharded_message) is None
+        assert self.message == ["my handler", [b"ssubscribe", b"foo", 1]]
+        assert r.spublish("foo", "test message") == 1
+        assert wait_for_message(p, func=p.get_sharded_message) is None
+        assert self.message == ["my handler", [b"smessage", b"foo", b"test message"]]
+
 
 class TestPubSubAutoDecoding:
     "These tests only validate that we get unicode values back"
 
     channel = "uni" + chr(4456) + "code"
     pattern = "uni" + chr(4456) + "*"
     data = "abc" + chr(4458) + "123"
```

### Comparing `redis-5.0.0b4/tests/test_retry.py` & `redis-5.0.0rc1/tests/test_retry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from unittest.mock import patch
 
 import pytest
-
 from redis.backoff import ExponentialBackoff, NoBackoff
 from redis.client import Redis
 from redis.connection import Connection, UnixDomainSocketConnection
 from redis.exceptions import (
     BusyLoadingError,
     ConnectionError,
     ReadOnlyError,
```

### Comparing `redis-5.0.0b4/tests/test_scripting.py` & `redis-5.0.0rc1/tests/test_scripting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 import redis
 from redis import exceptions
 from redis.commands.core import Script
 from tests.conftest import skip_if_redis_enterprise, skip_if_server_version_lt
 
 multiply_script = """
 local value = redis.call('GET', KEYS[1])
```

### Comparing `redis-5.0.0b4/tests/test_search.py` & `redis-5.0.0rc1/tests/test_search.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import bz2
 import csv
 import os
 import time
 from io import TextIOWrapper
 
 import pytest
-
 import redis
 import redis.commands.search
 import redis.commands.search.aggregation as aggregations
 import redis.commands.search.reducers as reducers
 from redis.commands.json.path import Path
 from redis.commands.search import Search
 from redis.commands.search.field import (
@@ -20,15 +19,21 @@
     VectorField,
 )
 from redis.commands.search.indexDefinition import IndexDefinition, IndexType
 from redis.commands.search.query import GeoFilter, NumericFilter, Query
 from redis.commands.search.result import Result
 from redis.commands.search.suggestion import Suggestion
 
-from .conftest import skip_if_redis_enterprise, skip_ifmodversion_lt
+from .conftest import (
+    _get_client,
+    assert_resp_response,
+    is_resp2_connection,
+    skip_if_redis_enterprise,
+    skip_ifmodversion_lt,
+)
 
 WILL_PLAY_TEXT = os.path.abspath(
     os.path.join(os.path.dirname(__file__), "testdata", "will_play_text.csv.bz2")
 )
 
 TITLES_CSV = os.path.abspath(
     os.path.join(os.path.dirname(__file__), "testdata", "titles.csv")
@@ -36,20 +41,24 @@
 
 
 def waitForIndex(env, idx, timeout=None):
     delay = 0.1
     while True:
         res = env.execute_command("FT.INFO", idx)
         try:
-            res.index("indexing")
+            if int(res[res.index("indexing") + 1]) == 0:
+                break
         except ValueError:
             break
-
-        if int(res[res.index("indexing") + 1]) == 0:
-            break
+        except AttributeError:
+            try:
+                if int(res["indexing"]) == 0:
+                    break
+            except ValueError:
+                break
 
         time.sleep(delay)
         if timeout is not None:
             timeout -= delay
             if timeout <= 0:
                 break
 
@@ -94,17 +103,18 @@
 
     for key, doc in chapters.items():
         indexer.client.client.hset(key, mapping=doc)
     indexer.commit()
 
 
 @pytest.fixture
-def client(modclient):
-    modclient.flushdb()
-    return modclient
+def client(request):
+    r = _get_client(redis.Redis, request, decode_responses=True)
+    r.flushdb()
+    return r
 
 
 @pytest.mark.redismod
 def test_client(client):
     num_docs = 500
     createIndex(client.ft(), num_docs=num_docs)
     waitForIndex(client, getattr(client.ft(), "index_name", "idx"))
@@ -129,124 +139,218 @@
     ]:
         assert k in info
 
     assert client.ft().index_name == info["index_name"]
     assert num_docs == int(info["num_docs"])
 
     res = client.ft().search("henry iv")
-    assert isinstance(res, Result)
-    assert 225 == res.total
-    assert 10 == len(res.docs)
-    assert res.duration > 0
-
-    for doc in res.docs:
-        assert doc.id
-        assert doc["id"]
-        assert doc.play == "Henry IV"
-        assert doc["play"] == "Henry IV"
+    if is_resp2_connection(client):
+        assert isinstance(res, Result)
+        assert 225 == res.total
+        assert 10 == len(res.docs)
+        assert res.duration > 0
+
+        for doc in res.docs:
+            assert doc.id
+            assert doc["id"]
+            assert doc.play == "Henry IV"
+            assert doc["play"] == "Henry IV"
+            assert len(doc.txt) > 0
+
+        # test no content
+        res = client.ft().search(Query("king").no_content())
+        assert 194 == res.total
+        assert 10 == len(res.docs)
+        for doc in res.docs:
+            assert "txt" not in doc.__dict__
+            assert "play" not in doc.__dict__
+
+        # test verbatim vs no verbatim
+        total = client.ft().search(Query("kings").no_content()).total
+        vtotal = client.ft().search(Query("kings").no_content().verbatim()).total
+        assert total > vtotal
+
+        # test in fields
+        txt_total = (
+            client.ft().search(Query("henry").no_content().limit_fields("txt")).total
+        )
+        play_total = (
+            client.ft().search(Query("henry").no_content().limit_fields("play")).total
+        )
+        both_total = (
+            client.ft()
+            .search(Query("henry").no_content().limit_fields("play", "txt"))
+            .total
+        )
+        assert 129 == txt_total
+        assert 494 == play_total
+        assert 494 == both_total
+
+        # test load_document
+        doc = client.ft().load_document("henry vi part 3:62")
+        assert doc is not None
+        assert "henry vi part 3:62" == doc.id
+        assert doc.play == "Henry VI Part 3"
         assert len(doc.txt) > 0
 
-    # test no content
-    res = client.ft().search(Query("king").no_content())
-    assert 194 == res.total
-    assert 10 == len(res.docs)
-    for doc in res.docs:
-        assert "txt" not in doc.__dict__
-        assert "play" not in doc.__dict__
-
-    # test verbatim vs no verbatim
-    total = client.ft().search(Query("kings").no_content()).total
-    vtotal = client.ft().search(Query("kings").no_content().verbatim()).total
-    assert total > vtotal
-
-    # test in fields
-    txt_total = (
-        client.ft().search(Query("henry").no_content().limit_fields("txt")).total
-    )
-    play_total = (
-        client.ft().search(Query("henry").no_content().limit_fields("play")).total
-    )
-    both_total = (
-        client.ft()
-        .search(Query("henry").no_content().limit_fields("play", "txt"))
-        .total
-    )
-    assert 129 == txt_total
-    assert 494 == play_total
-    assert 494 == both_total
-
-    # test load_document
-    doc = client.ft().load_document("henry vi part 3:62")
-    assert doc is not None
-    assert "henry vi part 3:62" == doc.id
-    assert doc.play == "Henry VI Part 3"
-    assert len(doc.txt) > 0
-
-    # test in-keys
-    ids = [x.id for x in client.ft().search(Query("henry")).docs]
-    assert 10 == len(ids)
-    subset = ids[:5]
-    docs = client.ft().search(Query("henry").limit_ids(*subset))
-    assert len(subset) == docs.total
-    ids = [x.id for x in docs.docs]
-    assert set(ids) == set(subset)
-
-    # test slop and in order
-    assert 193 == client.ft().search(Query("henry king")).total
-    assert 3 == client.ft().search(Query("henry king").slop(0).in_order()).total
-    assert 52 == client.ft().search(Query("king henry").slop(0).in_order()).total
-    assert 53 == client.ft().search(Query("henry king").slop(0)).total
-    assert 167 == client.ft().search(Query("henry king").slop(100)).total
-
-    # test delete document
-    client.hset("doc-5ghs2", mapping={"play": "Death of a Salesman"})
-    res = client.ft().search(Query("death of a salesman"))
-    assert 1 == res.total
-
-    assert 1 == client.ft().delete_document("doc-5ghs2")
-    res = client.ft().search(Query("death of a salesman"))
-    assert 0 == res.total
-    assert 0 == client.ft().delete_document("doc-5ghs2")
-
-    client.hset("doc-5ghs2", mapping={"play": "Death of a Salesman"})
-    res = client.ft().search(Query("death of a salesman"))
-    assert 1 == res.total
-    client.ft().delete_document("doc-5ghs2")
+        # test in-keys
+        ids = [x.id for x in client.ft().search(Query("henry")).docs]
+        assert 10 == len(ids)
+        subset = ids[:5]
+        docs = client.ft().search(Query("henry").limit_ids(*subset))
+        assert len(subset) == docs.total
+        ids = [x.id for x in docs.docs]
+        assert set(ids) == set(subset)
+
+        # test slop and in order
+        assert 193 == client.ft().search(Query("henry king")).total
+        assert 3 == client.ft().search(Query("henry king").slop(0).in_order()).total
+        assert 52 == client.ft().search(Query("king henry").slop(0).in_order()).total
+        assert 53 == client.ft().search(Query("henry king").slop(0)).total
+        assert 167 == client.ft().search(Query("henry king").slop(100)).total
+
+        # test delete document
+        client.hset("doc-5ghs2", mapping={"play": "Death of a Salesman"})
+        res = client.ft().search(Query("death of a salesman"))
+        assert 1 == res.total
+
+        assert 1 == client.ft().delete_document("doc-5ghs2")
+        res = client.ft().search(Query("death of a salesman"))
+        assert 0 == res.total
+        assert 0 == client.ft().delete_document("doc-5ghs2")
+
+        client.hset("doc-5ghs2", mapping={"play": "Death of a Salesman"})
+        res = client.ft().search(Query("death of a salesman"))
+        assert 1 == res.total
+        client.ft().delete_document("doc-5ghs2")
+    else:
+        assert isinstance(res, dict)
+        assert 225 == res["total_results"]
+        assert 10 == len(res["results"])
+
+        for doc in res["results"]:
+            assert doc["id"]
+            assert doc["extra_attributes"]["play"] == "Henry IV"
+            assert len(doc["extra_attributes"]["txt"]) > 0
+
+        # test no content
+        res = client.ft().search(Query("king").no_content())
+        assert 194 == res["total_results"]
+        assert 10 == len(res["results"])
+        for doc in res["results"]:
+            assert "extra_attributes" not in doc.keys()
+
+        # test verbatim vs no verbatim
+        total = client.ft().search(Query("kings").no_content())["total_results"]
+        vtotal = client.ft().search(Query("kings").no_content().verbatim())[
+            "total_results"
+        ]
+        assert total > vtotal
+
+        # test in fields
+        txt_total = client.ft().search(Query("henry").no_content().limit_fields("txt"))[
+            "total_results"
+        ]
+        play_total = client.ft().search(
+            Query("henry").no_content().limit_fields("play")
+        )["total_results"]
+        both_total = client.ft().search(
+            Query("henry").no_content().limit_fields("play", "txt")
+        )["total_results"]
+        assert 129 == txt_total
+        assert 494 == play_total
+        assert 494 == both_total
+
+        # test load_document
+        doc = client.ft().load_document("henry vi part 3:62")
+        assert doc is not None
+        assert "henry vi part 3:62" == doc.id
+        assert doc.play == "Henry VI Part 3"
+        assert len(doc.txt) > 0
+
+        # test in-keys
+        ids = [x["id"] for x in client.ft().search(Query("henry"))["results"]]
+        assert 10 == len(ids)
+        subset = ids[:5]
+        docs = client.ft().search(Query("henry").limit_ids(*subset))
+        assert len(subset) == docs["total_results"]
+        ids = [x["id"] for x in docs["results"]]
+        assert set(ids) == set(subset)
+
+        # test slop and in order
+        assert 193 == client.ft().search(Query("henry king"))["total_results"]
+        assert (
+            3
+            == client.ft().search(Query("henry king").slop(0).in_order())[
+                "total_results"
+            ]
+        )
+        assert (
+            52
+            == client.ft().search(Query("king henry").slop(0).in_order())[
+                "total_results"
+            ]
+        )
+        assert 53 == client.ft().search(Query("henry king").slop(0))["total_results"]
+        assert 167 == client.ft().search(Query("henry king").slop(100))["total_results"]
+
+        # test delete document
+        client.hset("doc-5ghs2", mapping={"play": "Death of a Salesman"})
+        res = client.ft().search(Query("death of a salesman"))
+        assert 1 == res["total_results"]
+
+        assert 1 == client.ft().delete_document("doc-5ghs2")
+        res = client.ft().search(Query("death of a salesman"))
+        assert 0 == res["total_results"]
+        assert 0 == client.ft().delete_document("doc-5ghs2")
+
+        client.hset("doc-5ghs2", mapping={"play": "Death of a Salesman"})
+        res = client.ft().search(Query("death of a salesman"))
+        assert 1 == res["total_results"]
+        client.ft().delete_document("doc-5ghs2")
 
 
 @pytest.mark.redismod
 @pytest.mark.onlynoncluster
 def test_scores(client):
     client.ft().create_index((TextField("txt"),))
 
     client.hset("doc1", mapping={"txt": "foo baz"})
     client.hset("doc2", mapping={"txt": "foo bar"})
 
     q = Query("foo ~bar").with_scores()
     res = client.ft().search(q)
-    assert 2 == res.total
-    assert "doc2" == res.docs[0].id
-    assert 3.0 == res.docs[0].score
-    assert "doc1" == res.docs[1].id
-    # todo: enable once new RS version is tagged
-    # self.assertEqual(0.2, res.docs[1].score)
+    if is_resp2_connection(client):
+        assert 2 == res.total
+        assert "doc2" == res.docs[0].id
+        assert 3.0 == res.docs[0].score
+        assert "doc1" == res.docs[1].id
+    else:
+        assert 2 == res["total_results"]
+        assert "doc2" == res["results"][0]["id"]
+        assert 3.0 == res["results"][0]["score"]
+        assert "doc1" == res["results"][1]["id"]
 
 
 @pytest.mark.redismod
 def test_stopwords(client):
     client.ft().create_index((TextField("txt"),), stopwords=["foo", "bar", "baz"])
     client.hset("doc1", mapping={"txt": "foo bar"})
     client.hset("doc2", mapping={"txt": "hello world"})
     waitForIndex(client, getattr(client.ft(), "index_name", "idx"))
 
     q1 = Query("foo bar").no_content()
     q2 = Query("foo bar hello world").no_content()
     res1, res2 = client.ft().search(q1), client.ft().search(q2)
-    assert 0 == res1.total
-    assert 1 == res2.total
+    if is_resp2_connection(client):
+        assert 0 == res1.total
+        assert 1 == res2.total
+    else:
+        assert 0 == res1["total_results"]
+        assert 1 == res2["total_results"]
 
 
 @pytest.mark.redismod
 def test_filters(client):
     client.ft().create_index((TextField("txt"), NumericField("num"), GeoField("loc")))
     client.hset(
         "doc1", mapping={"txt": "foo bar", "num": 3.141, "loc": "-0.441,51.458"}
@@ -258,55 +362,80 @@
     q1 = Query("foo").add_filter(NumericFilter("num", 0, 2)).no_content()
     q2 = (
         Query("foo")
         .add_filter(NumericFilter("num", 2, NumericFilter.INF, minExclusive=True))
         .no_content()
     )
     res1, res2 = client.ft().search(q1), client.ft().search(q2)
-
-    assert 1 == res1.total
-    assert 1 == res2.total
-    assert "doc2" == res1.docs[0].id
-    assert "doc1" == res2.docs[0].id
+    if is_resp2_connection(client):
+        assert 1 == res1.total
+        assert 1 == res2.total
+        assert "doc2" == res1.docs[0].id
+        assert "doc1" == res2.docs[0].id
+    else:
+        assert 1 == res1["total_results"]
+        assert 1 == res2["total_results"]
+        assert "doc2" == res1["results"][0]["id"]
+        assert "doc1" == res2["results"][0]["id"]
 
     # Test geo filter
     q1 = Query("foo").add_filter(GeoFilter("loc", -0.44, 51.45, 10)).no_content()
     q2 = Query("foo").add_filter(GeoFilter("loc", -0.44, 51.45, 100)).no_content()
     res1, res2 = client.ft().search(q1), client.ft().search(q2)
 
-    assert 1 == res1.total
-    assert 2 == res2.total
-    assert "doc1" == res1.docs[0].id
-
-    # Sort results, after RDB reload order may change
-    res = [res2.docs[0].id, res2.docs[1].id]
-    res.sort()
-    assert ["doc1", "doc2"] == res
+    if is_resp2_connection(client):
+        assert 1 == res1.total
+        assert 2 == res2.total
+        assert "doc1" == res1.docs[0].id
+
+        # Sort results, after RDB reload order may change
+        res = [res2.docs[0].id, res2.docs[1].id]
+        res.sort()
+        assert ["doc1", "doc2"] == res
+    else:
+        assert 1 == res1["total_results"]
+        assert 2 == res2["total_results"]
+        assert "doc1" == res1["results"][0]["id"]
+
+        # Sort results, after RDB reload order may change
+        res = [res2["results"][0]["id"], res2["results"][1]["id"]]
+        res.sort()
+        assert ["doc1", "doc2"] == res
 
 
 @pytest.mark.redismod
 def test_sort_by(client):
     client.ft().create_index((TextField("txt"), NumericField("num", sortable=True)))
     client.hset("doc1", mapping={"txt": "foo bar", "num": 1})
     client.hset("doc2", mapping={"txt": "foo baz", "num": 2})
     client.hset("doc3", mapping={"txt": "foo qux", "num": 3})
 
     # Test sort
     q1 = Query("foo").sort_by("num", asc=True).no_content()
     q2 = Query("foo").sort_by("num", asc=False).no_content()
     res1, res2 = client.ft().search(q1), client.ft().search(q2)
 
-    assert 3 == res1.total
-    assert "doc1" == res1.docs[0].id
-    assert "doc2" == res1.docs[1].id
-    assert "doc3" == res1.docs[2].id
-    assert 3 == res2.total
-    assert "doc1" == res2.docs[2].id
-    assert "doc2" == res2.docs[1].id
-    assert "doc3" == res2.docs[0].id
+    if is_resp2_connection(client):
+        assert 3 == res1.total
+        assert "doc1" == res1.docs[0].id
+        assert "doc2" == res1.docs[1].id
+        assert "doc3" == res1.docs[2].id
+        assert 3 == res2.total
+        assert "doc1" == res2.docs[2].id
+        assert "doc2" == res2.docs[1].id
+        assert "doc3" == res2.docs[0].id
+    else:
+        assert 3 == res1["total_results"]
+        assert "doc1" == res1["results"][0]["id"]
+        assert "doc2" == res1["results"][1]["id"]
+        assert "doc3" == res1["results"][2]["id"]
+        assert 3 == res2["total_results"]
+        assert "doc1" == res2["results"][2]["id"]
+        assert "doc2" == res2["results"][1]["id"]
+        assert "doc3" == res2["results"][0]["id"]
 
 
 @pytest.mark.redismod
 @skip_ifmodversion_lt("2.0.0", "search")
 def test_drop_index(client):
     """
     Ensure the index gets dropped by data remains by default
@@ -413,35 +542,58 @@
     )
     client.hset(
         "doc2",
         mapping={"field": "aab", "text": "2", "numeric": "2", "geo": "2,2", "tag": "2"},
     )
     waitForIndex(client, getattr(client.ft(), "index_name", "idx"))
 
-    res = client.ft().search(Query("@text:aa*"))
-    assert 0 == res.total
+    if is_resp2_connection(client):
+        res = client.ft().search(Query("@text:aa*"))
+        assert 0 == res.total
+
+        res = client.ft().search(Query("@field:aa*"))
+        assert 2 == res.total
+
+        res = client.ft().search(Query("*").sort_by("text", asc=False))
+        assert 2 == res.total
+        assert "doc2" == res.docs[0].id
+
+        res = client.ft().search(Query("*").sort_by("text", asc=True))
+        assert "doc1" == res.docs[0].id
+
+        res = client.ft().search(Query("*").sort_by("numeric", asc=True))
+        assert "doc1" == res.docs[0].id
+
+        res = client.ft().search(Query("*").sort_by("geo", asc=True))
+        assert "doc1" == res.docs[0].id
+
+        res = client.ft().search(Query("*").sort_by("tag", asc=True))
+        assert "doc1" == res.docs[0].id
+    else:
+        res = client.ft().search(Query("@text:aa*"))
+        assert 0 == res["total_results"]
 
-    res = client.ft().search(Query("@field:aa*"))
-    assert 2 == res.total
+        res = client.ft().search(Query("@field:aa*"))
+        assert 2 == res["total_results"]
 
-    res = client.ft().search(Query("*").sort_by("text", asc=False))
-    assert 2 == res.total
-    assert "doc2" == res.docs[0].id
+        res = client.ft().search(Query("*").sort_by("text", asc=False))
+        assert 2 == res["total_results"]
+        assert "doc2" == res["results"][0]["id"]
 
-    res = client.ft().search(Query("*").sort_by("text", asc=True))
-    assert "doc1" == res.docs[0].id
+        res = client.ft().search(Query("*").sort_by("text", asc=True))
+        assert "doc1" == res["results"][0]["id"]
 
-    res = client.ft().search(Query("*").sort_by("numeric", asc=True))
-    assert "doc1" == res.docs[0].id
+        res = client.ft().search(Query("*").sort_by("numeric", asc=True))
+        assert "doc1" == res["results"][0]["id"]
 
-    res = client.ft().search(Query("*").sort_by("geo", asc=True))
-    assert "doc1" == res.docs[0].id
+        res = client.ft().search(Query("*").sort_by("geo", asc=True))
+        assert "doc1" == res["results"][0]["id"]
 
-    res = client.ft().search(Query("*").sort_by("tag", asc=True))
-    assert "doc1" == res.docs[0].id
+        res = client.ft().search(Query("*").sort_by("tag", asc=True))
+        assert "doc1" == res["results"][0]["id"]
 
     # Ensure exception is raised for non-indexable, non-sortable fields
     with pytest.raises(Exception):
         TextField("name", no_index=True, sortable=False)
     with pytest.raises(Exception):
         NumericField("name", no_index=True, sortable=False)
     with pytest.raises(Exception):
@@ -468,29 +620,46 @@
     createIndex(client.ft())
     waitForIndex(client, getattr(client.ft(), "index_name", "idx"))
 
     q = Query("king henry").paging(0, 1)
     q.highlight(fields=("play", "txt"), tags=("<b>", "</b>"))
     q.summarize("txt")
 
-    doc = sorted(client.ft().search(q).docs)[0]
-    assert "<b>Henry</b> IV" == doc.play
-    assert (
-        "ACT I SCENE I. London. The palace. Enter <b>KING</b> <b>HENRY</b>, LORD JOHN OF LANCASTER, the EARL of WESTMORELAND, SIR... "  # noqa
-        == doc.txt
-    )
+    if is_resp2_connection(client):
+        doc = sorted(client.ft().search(q).docs)[0]
+        assert "<b>Henry</b> IV" == doc.play
+        assert (
+            "ACT I SCENE I. London. The palace. Enter <b>KING</b> <b>HENRY</b>, LORD JOHN OF LANCASTER, the EARL of WESTMORELAND, SIR... "  # noqa
+            == doc.txt
+        )
 
-    q = Query("king henry").paging(0, 1).summarize().highlight()
-
-    doc = sorted(client.ft().search(q).docs)[0]
-    assert "<b>Henry</b> ... " == doc.play
-    assert (
-        "ACT I SCENE I. London. The palace. Enter <b>KING</b> <b>HENRY</b>, LORD JOHN OF LANCASTER, the EARL of WESTMORELAND, SIR... "  # noqa
-        == doc.txt
-    )
+        q = Query("king henry").paging(0, 1).summarize().highlight()
+
+        doc = sorted(client.ft().search(q).docs)[0]
+        assert "<b>Henry</b> ... " == doc.play
+        assert (
+            "ACT I SCENE I. London. The palace. Enter <b>KING</b> <b>HENRY</b>, LORD JOHN OF LANCASTER, the EARL of WESTMORELAND, SIR... "  # noqa
+            == doc.txt
+        )
+    else:
+        doc = sorted(client.ft().search(q)["results"])[0]
+        assert "<b>Henry</b> IV" == doc["extra_attributes"]["play"]
+        assert (
+            "ACT I SCENE I. London. The palace. Enter <b>KING</b> <b>HENRY</b>, LORD JOHN OF LANCASTER, the EARL of WESTMORELAND, SIR... "  # noqa
+            == doc["extra_attributes"]["txt"]
+        )
+
+        q = Query("king henry").paging(0, 1).summarize().highlight()
+
+        doc = sorted(client.ft().search(q)["results"])[0]
+        assert "<b>Henry</b> ... " == doc["extra_attributes"]["play"]
+        assert (
+            "ACT I SCENE I. London. The palace. Enter <b>KING</b> <b>HENRY</b>, LORD JOHN OF LANCASTER, the EARL of WESTMORELAND, SIR... "  # noqa
+            == doc["extra_attributes"]["txt"]
+        )
 
 
 @pytest.mark.redismod
 @skip_ifmodversion_lt("2.0.0", "search")
 def test_alias(client):
     index1 = getClient(client)
     index2 = getClient(client)
@@ -502,83 +671,122 @@
     ftindex2 = index2.ft("testAlias2")
     ftindex1.create_index((TextField("name"),), definition=def1)
     ftindex2.create_index((TextField("name"),), definition=def2)
 
     index1.hset("index1:lonestar", mapping={"name": "lonestar"})
     index2.hset("index2:yogurt", mapping={"name": "yogurt"})
 
-    res = ftindex1.search("*").docs[0]
-    assert "index1:lonestar" == res.id
+    if is_resp2_connection(client):
+        res = ftindex1.search("*").docs[0]
+        assert "index1:lonestar" == res.id
+
+        # create alias and check for results
+        ftindex1.aliasadd("spaceballs")
+        alias_client = getClient(client).ft("spaceballs")
+        res = alias_client.search("*").docs[0]
+        assert "index1:lonestar" == res.id
+
+        # Throw an exception when trying to add an alias that already exists
+        with pytest.raises(Exception):
+            ftindex2.aliasadd("spaceballs")
+
+        # update alias and ensure new results
+        ftindex2.aliasupdate("spaceballs")
+        alias_client2 = getClient(client).ft("spaceballs")
+
+        res = alias_client2.search("*").docs[0]
+        assert "index2:yogurt" == res.id
+    else:
+        res = ftindex1.search("*")["results"][0]
+        assert "index1:lonestar" == res["id"]
+
+        # create alias and check for results
+        ftindex1.aliasadd("spaceballs")
+        alias_client = getClient(client).ft("spaceballs")
+        res = alias_client.search("*")["results"][0]
+        assert "index1:lonestar" == res["id"]
+
+        # Throw an exception when trying to add an alias that already exists
+        with pytest.raises(Exception):
+            ftindex2.aliasadd("spaceballs")
+
+        # update alias and ensure new results
+        ftindex2.aliasupdate("spaceballs")
+        alias_client2 = getClient(client).ft("spaceballs")
 
-    # create alias and check for results
-    ftindex1.aliasadd("spaceballs")
-    alias_client = getClient(client).ft("spaceballs")
-    res = alias_client.search("*").docs[0]
-    assert "index1:lonestar" == res.id
-
-    # Throw an exception when trying to add an alias that already exists
-    with pytest.raises(Exception):
-        ftindex2.aliasadd("spaceballs")
-
-    # update alias and ensure new results
-    ftindex2.aliasupdate("spaceballs")
-    alias_client2 = getClient(client).ft("spaceballs")
-
-    res = alias_client2.search("*").docs[0]
-    assert "index2:yogurt" == res.id
+        res = alias_client2.search("*")["results"][0]
+        assert "index2:yogurt" == res["id"]
 
     ftindex2.aliasdel("spaceballs")
     with pytest.raises(Exception):
         alias_client2.search("*").docs[0]
 
 
 @pytest.mark.redismod
+@pytest.mark.xfail(strict=False)
 def test_alias_basic(client):
     # Creating a client with one index
-    getClient(client).flushdb()
     index1 = getClient(client).ft("testAlias")
 
     index1.create_index((TextField("txt"),))
     index1.client.hset("doc1", mapping={"txt": "text goes here"})
 
     index2 = getClient(client).ft("testAlias2")
     index2.create_index((TextField("txt"),))
     index2.client.hset("doc2", mapping={"txt": "text goes here"})
 
     # add the actual alias and check
     index1.aliasadd("myalias")
     alias_client = getClient(client).ft("myalias")
-    res = sorted(alias_client.search("*").docs, key=lambda x: x.id)
-    assert "doc1" == res[0].id
-
-    # Throw an exception when trying to add an alias that already exists
-    with pytest.raises(Exception):
-        index2.aliasadd("myalias")
-
-    # update the alias and ensure we get doc2
-    index2.aliasupdate("myalias")
-    alias_client2 = getClient(client).ft("myalias")
-    res = sorted(alias_client2.search("*").docs, key=lambda x: x.id)
-    assert "doc1" == res[0].id
+    if is_resp2_connection(client):
+        res = sorted(alias_client.search("*").docs, key=lambda x: x.id)
+        assert "doc1" == res[0].id
+
+        # Throw an exception when trying to add an alias that already exists
+        with pytest.raises(Exception):
+            index2.aliasadd("myalias")
+
+        # update the alias and ensure we get doc2
+        index2.aliasupdate("myalias")
+        alias_client2 = getClient(client).ft("myalias")
+        res = sorted(alias_client2.search("*").docs, key=lambda x: x.id)
+        assert "doc1" == res[0].id
+    else:
+        res = sorted(alias_client.search("*")["results"], key=lambda x: x["id"])
+        assert "doc1" == res[0]["id"]
+
+        # Throw an exception when trying to add an alias that already exists
+        with pytest.raises(Exception):
+            index2.aliasadd("myalias")
+
+        # update the alias and ensure we get doc2
+        index2.aliasupdate("myalias")
+        alias_client2 = getClient(client).ft("myalias")
+        res = sorted(alias_client2.search("*")["results"], key=lambda x: x["id"])
+        assert "doc1" == res[0]["id"]
 
     # delete the alias and expect an error if we try to query again
     index2.aliasdel("myalias")
     with pytest.raises(Exception):
         _ = alias_client2.search("*").docs[0]
 
 
 @pytest.mark.redismod
 def test_textfield_sortable_nostem(client):
     # Creating the index definition with sortable and no_stem
     client.ft().create_index((TextField("txt", sortable=True, no_stem=True),))
 
     # Now get the index info to confirm its contents
     response = client.ft().info()
-    assert "SORTABLE" in response["attributes"][0]
-    assert "NOSTEM" in response["attributes"][0]
+    if is_resp2_connection(client):
+        assert "SORTABLE" in response["attributes"][0]
+        assert "NOSTEM" in response["attributes"][0]
+    else:
+        assert "SORTABLE" in response["attributes"][0]["flags"]
+        assert "NOSTEM" in response["attributes"][0]["flags"]
 
 
 @pytest.mark.redismod
 def test_alter_schema_add(client):
     # Creating the index definition and schema
     client.ft().create_index(TextField("title"))
 
@@ -591,54 +799,88 @@
     )
 
     # Searching with parameter only in the body (the added field)
     q = Query("only in the body")
 
     # Ensure we find the result searching on the added body field
     res = client.ft().search(q)
-    assert 1 == res.total
+    if is_resp2_connection(client):
+        assert 1 == res.total
+    else:
+        assert 1 == res["total_results"]
 
 
 @pytest.mark.redismod
 def test_spell_check(client):
     client.ft().create_index((TextField("f1"), TextField("f2")))
 
     client.hset(
         "doc1", mapping={"f1": "some valid content", "f2": "this is sample text"}
     )
     client.hset("doc2", mapping={"f1": "very important", "f2": "lorem ipsum"})
     waitForIndex(client, getattr(client.ft(), "index_name", "idx"))
 
-    # test spellcheck
-    res = client.ft().spellcheck("impornant")
-    assert "important" == res["impornant"][0]["suggestion"]
-
-    res = client.ft().spellcheck("contnt")
-    assert "content" == res["contnt"][0]["suggestion"]
-
-    # test spellcheck with Levenshtein distance
-    res = client.ft().spellcheck("vlis")
-    assert res == {}
-    res = client.ft().spellcheck("vlis", distance=2)
-    assert "valid" == res["vlis"][0]["suggestion"]
-
-    # test spellcheck include
-    client.ft().dict_add("dict", "lore", "lorem", "lorm")
-    res = client.ft().spellcheck("lorm", include="dict")
-    assert len(res["lorm"]) == 3
-    assert (
-        res["lorm"][0]["suggestion"],
-        res["lorm"][1]["suggestion"],
-        res["lorm"][2]["suggestion"],
-    ) == ("lorem", "lore", "lorm")
-    assert (res["lorm"][0]["score"], res["lorm"][1]["score"]) == ("0.5", "0")
-
-    # test spellcheck exclude
-    res = client.ft().spellcheck("lorm", exclude="dict")
-    assert res == {}
+    if is_resp2_connection(client):
+
+        # test spellcheck
+        res = client.ft().spellcheck("impornant")
+        assert "important" == res["impornant"][0]["suggestion"]
+
+        res = client.ft().spellcheck("contnt")
+        assert "content" == res["contnt"][0]["suggestion"]
+
+        # test spellcheck with Levenshtein distance
+        res = client.ft().spellcheck("vlis")
+        assert res == {}
+        res = client.ft().spellcheck("vlis", distance=2)
+        assert "valid" == res["vlis"][0]["suggestion"]
+
+        # test spellcheck include
+        client.ft().dict_add("dict", "lore", "lorem", "lorm")
+        res = client.ft().spellcheck("lorm", include="dict")
+        assert len(res["lorm"]) == 3
+        assert (
+            res["lorm"][0]["suggestion"],
+            res["lorm"][1]["suggestion"],
+            res["lorm"][2]["suggestion"],
+        ) == ("lorem", "lore", "lorm")
+        assert (res["lorm"][0]["score"], res["lorm"][1]["score"]) == ("0.5", "0")
+
+        # test spellcheck exclude
+        res = client.ft().spellcheck("lorm", exclude="dict")
+        assert res == {}
+    else:
+        # test spellcheck
+        res = client.ft().spellcheck("impornant")
+        assert "important" in res["results"]["impornant"][0].keys()
+
+        res = client.ft().spellcheck("contnt")
+        assert "content" in res["results"]["contnt"][0].keys()
+
+        # test spellcheck with Levenshtein distance
+        res = client.ft().spellcheck("vlis")
+        assert res == {"results": {"vlis": []}}
+        res = client.ft().spellcheck("vlis", distance=2)
+        assert "valid" in res["results"]["vlis"][0].keys()
+
+        # test spellcheck include
+        client.ft().dict_add("dict", "lore", "lorem", "lorm")
+        res = client.ft().spellcheck("lorm", include="dict")
+        assert len(res["results"]["lorm"]) == 3
+        assert "lorem" in res["results"]["lorm"][0].keys()
+        assert "lore" in res["results"]["lorm"][1].keys()
+        assert "lorm" in res["results"]["lorm"][2].keys()
+        assert (
+            res["results"]["lorm"][0]["lorem"],
+            res["results"]["lorm"][1]["lore"],
+        ) == (0.5, 0)
+
+        # test spellcheck exclude
+        res = client.ft().spellcheck("lorm", exclude="dict")
+        assert res == {"results": {}}
 
 
 @pytest.mark.redismod
 def test_dict_operations(client):
     client.ft().create_index((TextField("f1"), TextField("f2")))
     # Add three items
     res = client.ft().dict_add("custom_dict", "item1", "item2", "item3")
@@ -646,40 +888,50 @@
 
     # Remove one item
     res = client.ft().dict_del("custom_dict", "item2")
     assert 1 == res
 
     # Dump dict and inspect content
     res = client.ft().dict_dump("custom_dict")
-    assert ["item1", "item3"] == res
+    assert_resp_response(client, res, ["item1", "item3"], {"item1", "item3"})
 
     # Remove rest of the items before reload
     client.ft().dict_del("custom_dict", *res)
 
 
 @pytest.mark.redismod
 def test_phonetic_matcher(client):
     client.ft().create_index((TextField("name"),))
     client.hset("doc1", mapping={"name": "Jon"})
     client.hset("doc2", mapping={"name": "John"})
 
     res = client.ft().search(Query("Jon"))
-    assert 1 == len(res.docs)
-    assert "Jon" == res.docs[0].name
+    if is_resp2_connection(client):
+        assert 1 == len(res.docs)
+        assert "Jon" == res.docs[0].name
+    else:
+        assert 1 == res["total_results"]
+        assert "Jon" == res["results"][0]["extra_attributes"]["name"]
 
     # Drop and create index with phonetic matcher
     client.flushdb()
 
     client.ft().create_index((TextField("name", phonetic_matcher="dm:en"),))
     client.hset("doc1", mapping={"name": "Jon"})
     client.hset("doc2", mapping={"name": "John"})
 
     res = client.ft().search(Query("Jon"))
-    assert 2 == len(res.docs)
-    assert ["John", "Jon"] == sorted(d.name for d in res.docs)
+    if is_resp2_connection(client):
+        assert 2 == len(res.docs)
+        assert ["John", "Jon"] == sorted(d.name for d in res.docs)
+    else:
+        assert 2 == res["total_results"]
+        assert ["John", "Jon"] == sorted(
+            d["extra_attributes"]["name"] for d in res["results"]
+        )
 
 
 @pytest.mark.redismod
 @pytest.mark.onlynoncluster
 def test_scorer(client):
     client.ft().create_index((TextField("description"),))
 
@@ -690,28 +942,44 @@
         "doc2",
         mapping={
             "description": "Quick alice was beginning to get very tired of sitting by her quick sister on the bank, and of having nothing to do."  # noqa
         },
     )
 
     # default scorer is TFIDF
-    res = client.ft().search(Query("quick").with_scores())
-    assert 1.0 == res.docs[0].score
-    res = client.ft().search(Query("quick").scorer("TFIDF").with_scores())
-    assert 1.0 == res.docs[0].score
-    res = client.ft().search(Query("quick").scorer("TFIDF.DOCNORM").with_scores())
-    assert 0.1111111111111111 == res.docs[0].score
-    res = client.ft().search(Query("quick").scorer("BM25").with_scores())
-    assert 0.17699114465425977 == res.docs[0].score
-    res = client.ft().search(Query("quick").scorer("DISMAX").with_scores())
-    assert 2.0 == res.docs[0].score
-    res = client.ft().search(Query("quick").scorer("DOCSCORE").with_scores())
-    assert 1.0 == res.docs[0].score
-    res = client.ft().search(Query("quick").scorer("HAMMING").with_scores())
-    assert 0.0 == res.docs[0].score
+    if is_resp2_connection(client):
+        res = client.ft().search(Query("quick").with_scores())
+        assert 1.0 == res.docs[0].score
+        res = client.ft().search(Query("quick").scorer("TFIDF").with_scores())
+        assert 1.0 == res.docs[0].score
+        res = client.ft().search(Query("quick").scorer("TFIDF.DOCNORM").with_scores())
+        assert 0.1111111111111111 == res.docs[0].score
+        res = client.ft().search(Query("quick").scorer("BM25").with_scores())
+        assert 0.17699114465425977 == res.docs[0].score
+        res = client.ft().search(Query("quick").scorer("DISMAX").with_scores())
+        assert 2.0 == res.docs[0].score
+        res = client.ft().search(Query("quick").scorer("DOCSCORE").with_scores())
+        assert 1.0 == res.docs[0].score
+        res = client.ft().search(Query("quick").scorer("HAMMING").with_scores())
+        assert 0.0 == res.docs[0].score
+    else:
+        res = client.ft().search(Query("quick").with_scores())
+        assert 1.0 == res["results"][0]["score"]
+        res = client.ft().search(Query("quick").scorer("TFIDF").with_scores())
+        assert 1.0 == res["results"][0]["score"]
+        res = client.ft().search(Query("quick").scorer("TFIDF.DOCNORM").with_scores())
+        assert 0.1111111111111111 == res["results"][0]["score"]
+        res = client.ft().search(Query("quick").scorer("BM25").with_scores())
+        assert 0.17699114465425977 == res["results"][0]["score"]
+        res = client.ft().search(Query("quick").scorer("DISMAX").with_scores())
+        assert 2.0 == res["results"][0]["score"]
+        res = client.ft().search(Query("quick").scorer("DOCSCORE").with_scores())
+        assert 1.0 == res["results"][0]["score"]
+        res = client.ft().search(Query("quick").scorer("HAMMING").with_scores())
+        assert 0.0 == res["results"][0]["score"]
 
 
 @pytest.mark.redismod
 def test_get(client):
     client.ft().create_index((TextField("f1"), TextField("f2")))
 
     assert [None] == client.ft().get("doc1")
@@ -784,164 +1052,317 @@
             "title": "RedisJson",
             "body": "RedisJSON implements ECMA-404 The JSON Data Interchange Standard as a native data type.",  # noqa
             "parent": "redis",
             "random_num": 8,
         },
     )
 
-    req = aggregations.AggregateRequest("redis").group_by("@parent", reducers.count())
+    if is_resp2_connection(client):
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.count()
+        )
 
-    res = client.ft().aggregate(req).rows[0]
-    assert res[1] == "redis"
-    assert res[3] == "3"
+        res = client.ft().aggregate(req).rows[0]
+        assert res[1] == "redis"
+        assert res[3] == "3"
 
-    req = aggregations.AggregateRequest("redis").group_by(
-        "@parent", reducers.count_distinct("@title")
-    )
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.count_distinct("@title")
+        )
 
-    res = client.ft().aggregate(req).rows[0]
-    assert res[1] == "redis"
-    assert res[3] == "3"
+        res = client.ft().aggregate(req).rows[0]
+        assert res[1] == "redis"
+        assert res[3] == "3"
 
-    req = aggregations.AggregateRequest("redis").group_by(
-        "@parent", reducers.count_distinctish("@title")
-    )
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.count_distinctish("@title")
+        )
 
-    res = client.ft().aggregate(req).rows[0]
-    assert res[1] == "redis"
-    assert res[3] == "3"
+        res = client.ft().aggregate(req).rows[0]
+        assert res[1] == "redis"
+        assert res[3] == "3"
 
-    req = aggregations.AggregateRequest("redis").group_by(
-        "@parent", reducers.sum("@random_num")
-    )
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.sum("@random_num")
+        )
 
-    res = client.ft().aggregate(req).rows[0]
-    assert res[1] == "redis"
-    assert res[3] == "21"  # 10+8+3
+        res = client.ft().aggregate(req).rows[0]
+        assert res[1] == "redis"
+        assert res[3] == "21"  # 10+8+3
 
-    req = aggregations.AggregateRequest("redis").group_by(
-        "@parent", reducers.min("@random_num")
-    )
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.min("@random_num")
+        )
 
-    res = client.ft().aggregate(req).rows[0]
-    assert res[1] == "redis"
-    assert res[3] == "3"  # min(10,8,3)
+        res = client.ft().aggregate(req).rows[0]
+        assert res[1] == "redis"
+        assert res[3] == "3"  # min(10,8,3)
 
-    req = aggregations.AggregateRequest("redis").group_by(
-        "@parent", reducers.max("@random_num")
-    )
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.max("@random_num")
+        )
 
-    res = client.ft().aggregate(req).rows[0]
-    assert res[1] == "redis"
-    assert res[3] == "10"  # max(10,8,3)
+        res = client.ft().aggregate(req).rows[0]
+        assert res[1] == "redis"
+        assert res[3] == "10"  # max(10,8,3)
 
-    req = aggregations.AggregateRequest("redis").group_by(
-        "@parent", reducers.avg("@random_num")
-    )
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.avg("@random_num")
+        )
 
-    res = client.ft().aggregate(req).rows[0]
-    assert res[1] == "redis"
-    index = res.index("__generated_aliasavgrandom_num")
-    assert res[index + 1] == "7"  # (10+3+8)/3
+        res = client.ft().aggregate(req).rows[0]
+        assert res[1] == "redis"
+        index = res.index("__generated_aliasavgrandom_num")
+        assert res[index + 1] == "7"  # (10+3+8)/3
 
-    req = aggregations.AggregateRequest("redis").group_by(
-        "@parent", reducers.stddev("random_num")
-    )
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.stddev("random_num")
+        )
 
-    res = client.ft().aggregate(req).rows[0]
-    assert res[1] == "redis"
-    assert res[3] == "3.60555127546"
+        res = client.ft().aggregate(req).rows[0]
+        assert res[1] == "redis"
+        assert res[3] == "3.60555127546"
 
-    req = aggregations.AggregateRequest("redis").group_by(
-        "@parent", reducers.quantile("@random_num", 0.5)
-    )
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.quantile("@random_num", 0.5)
+        )
 
-    res = client.ft().aggregate(req).rows[0]
-    assert res[1] == "redis"
-    assert res[3] == "8"  # median of 3,8,10
+        res = client.ft().aggregate(req).rows[0]
+        assert res[1] == "redis"
+        assert res[3] == "8"  # median of 3,8,10
 
-    req = aggregations.AggregateRequest("redis").group_by(
-        "@parent", reducers.tolist("@title")
-    )
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.tolist("@title")
+        )
 
-    res = client.ft().aggregate(req).rows[0]
-    assert res[1] == "redis"
-    assert set(res[3]) == {"RediSearch", "RedisAI", "RedisJson"}
+        res = client.ft().aggregate(req).rows[0]
+        assert res[1] == "redis"
+        assert set(res[3]) == {"RediSearch", "RedisAI", "RedisJson"}
 
-    req = aggregations.AggregateRequest("redis").group_by(
-        "@parent", reducers.first_value("@title").alias("first")
-    )
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.first_value("@title").alias("first")
+        )
 
-    res = client.ft().aggregate(req).rows[0]
-    assert res == ["parent", "redis", "first", "RediSearch"]
+        res = client.ft().aggregate(req).rows[0]
+        assert res == ["parent", "redis", "first", "RediSearch"]
 
-    req = aggregations.AggregateRequest("redis").group_by(
-        "@parent", reducers.random_sample("@title", 2).alias("random")
-    )
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.random_sample("@title", 2).alias("random")
+        )
+
+        res = client.ft().aggregate(req).rows[0]
+        assert res[1] == "redis"
+        assert res[2] == "random"
+        assert len(res[3]) == 2
+        assert res[3][0] in ["RediSearch", "RedisAI", "RedisJson"]
+    else:
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.count()
+        )
+
+        res = client.ft().aggregate(req)["results"][0]
+        assert res["extra_attributes"]["parent"] == "redis"
+        assert res["extra_attributes"]["__generated_aliascount"] == "3"
+
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.count_distinct("@title")
+        )
+
+        res = client.ft().aggregate(req)["results"][0]
+        assert res["extra_attributes"]["parent"] == "redis"
+        assert res["extra_attributes"]["__generated_aliascount_distincttitle"] == "3"
+
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.count_distinctish("@title")
+        )
+
+        res = client.ft().aggregate(req)["results"][0]
+        assert res["extra_attributes"]["parent"] == "redis"
+        assert res["extra_attributes"]["__generated_aliascount_distinctishtitle"] == "3"
+
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.sum("@random_num")
+        )
+
+        res = client.ft().aggregate(req)["results"][0]
+        assert res["extra_attributes"]["parent"] == "redis"
+        assert res["extra_attributes"]["__generated_aliassumrandom_num"] == "21"
+
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.min("@random_num")
+        )
+
+        res = client.ft().aggregate(req)["results"][0]
+        assert res["extra_attributes"]["parent"] == "redis"
+        assert res["extra_attributes"]["__generated_aliasminrandom_num"] == "3"
+
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.max("@random_num")
+        )
+
+        res = client.ft().aggregate(req)["results"][0]
+        assert res["extra_attributes"]["parent"] == "redis"
+        assert res["extra_attributes"]["__generated_aliasmaxrandom_num"] == "10"
+
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.avg("@random_num")
+        )
+
+        res = client.ft().aggregate(req)["results"][0]
+        assert res["extra_attributes"]["parent"] == "redis"
+        assert res["extra_attributes"]["__generated_aliasavgrandom_num"] == "7"
 
-    res = client.ft().aggregate(req).rows[0]
-    assert res[1] == "redis"
-    assert res[2] == "random"
-    assert len(res[3]) == 2
-    assert res[3][0] in ["RediSearch", "RedisAI", "RedisJson"]
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.stddev("random_num")
+        )
+
+        res = client.ft().aggregate(req)["results"][0]
+        assert res["extra_attributes"]["parent"] == "redis"
+        assert (
+            res["extra_attributes"]["__generated_aliasstddevrandom_num"]
+            == "3.60555127546"
+        )
+
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.quantile("@random_num", 0.5)
+        )
+
+        res = client.ft().aggregate(req)["results"][0]
+        assert res["extra_attributes"]["parent"] == "redis"
+        assert res["extra_attributes"]["__generated_aliasquantilerandom_num,0.5"] == "8"
+
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.tolist("@title")
+        )
+
+        res = client.ft().aggregate(req)["results"][0]
+        assert res["extra_attributes"]["parent"] == "redis"
+        assert set(res["extra_attributes"]["__generated_aliastolisttitle"]) == {
+            "RediSearch",
+            "RedisAI",
+            "RedisJson",
+        }
+
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.first_value("@title").alias("first")
+        )
+
+        res = client.ft().aggregate(req)["results"][0]
+        assert res["extra_attributes"] == {"parent": "redis", "first": "RediSearch"}
+
+        req = aggregations.AggregateRequest("redis").group_by(
+            "@parent", reducers.random_sample("@title", 2).alias("random")
+        )
+
+        res = client.ft().aggregate(req)["results"][0]
+        assert res["extra_attributes"]["parent"] == "redis"
+        assert "random" in res["extra_attributes"].keys()
+        assert len(res["extra_attributes"]["random"]) == 2
+        assert res["extra_attributes"]["random"][0] in [
+            "RediSearch",
+            "RedisAI",
+            "RedisJson",
+        ]
 
 
 @pytest.mark.redismod
 def test_aggregations_sort_by_and_limit(client):
     client.ft().create_index((TextField("t1"), TextField("t2")))
 
     client.ft().client.hset("doc1", mapping={"t1": "a", "t2": "b"})
     client.ft().client.hset("doc2", mapping={"t1": "b", "t2": "a"})
 
-    # test sort_by using SortDirection
-    req = aggregations.AggregateRequest("*").sort_by(
-        aggregations.Asc("@t2"), aggregations.Desc("@t1")
-    )
-    res = client.ft().aggregate(req)
-    assert res.rows[0] == ["t2", "a", "t1", "b"]
-    assert res.rows[1] == ["t2", "b", "t1", "a"]
+    if is_resp2_connection(client):
+        # test sort_by using SortDirection
+        req = aggregations.AggregateRequest("*").sort_by(
+            aggregations.Asc("@t2"), aggregations.Desc("@t1")
+        )
+        res = client.ft().aggregate(req)
+        assert res.rows[0] == ["t2", "a", "t1", "b"]
+        assert res.rows[1] == ["t2", "b", "t1", "a"]
 
-    # test sort_by without SortDirection
-    req = aggregations.AggregateRequest("*").sort_by("@t1")
-    res = client.ft().aggregate(req)
-    assert res.rows[0] == ["t1", "a"]
-    assert res.rows[1] == ["t1", "b"]
+        # test sort_by without SortDirection
+        req = aggregations.AggregateRequest("*").sort_by("@t1")
+        res = client.ft().aggregate(req)
+        assert res.rows[0] == ["t1", "a"]
+        assert res.rows[1] == ["t1", "b"]
 
-    # test sort_by with max
-    req = aggregations.AggregateRequest("*").sort_by("@t1", max=1)
-    res = client.ft().aggregate(req)
-    assert len(res.rows) == 1
+        # test sort_by with max
+        req = aggregations.AggregateRequest("*").sort_by("@t1", max=1)
+        res = client.ft().aggregate(req)
+        assert len(res.rows) == 1
 
-    # test limit
-    req = aggregations.AggregateRequest("*").sort_by("@t1").limit(1, 1)
-    res = client.ft().aggregate(req)
-    assert len(res.rows) == 1
-    assert res.rows[0] == ["t1", "b"]
+        # test limit
+        req = aggregations.AggregateRequest("*").sort_by("@t1").limit(1, 1)
+        res = client.ft().aggregate(req)
+        assert len(res.rows) == 1
+        assert res.rows[0] == ["t1", "b"]
+    else:
+        # test sort_by using SortDirection
+        req = aggregations.AggregateRequest("*").sort_by(
+            aggregations.Asc("@t2"), aggregations.Desc("@t1")
+        )
+        res = client.ft().aggregate(req)["results"]
+        assert res[0]["extra_attributes"] == {"t2": "a", "t1": "b"}
+        assert res[1]["extra_attributes"] == {"t2": "b", "t1": "a"}
+
+        # test sort_by without SortDirection
+        req = aggregations.AggregateRequest("*").sort_by("@t1")
+        res = client.ft().aggregate(req)["results"]
+        assert res[0]["extra_attributes"] == {"t1": "a"}
+        assert res[1]["extra_attributes"] == {"t1": "b"}
+
+        # test sort_by with max
+        req = aggregations.AggregateRequest("*").sort_by("@t1", max=1)
+        res = client.ft().aggregate(req)
+        assert len(res["results"]) == 1
+
+        # test limit
+        req = aggregations.AggregateRequest("*").sort_by("@t1").limit(1, 1)
+        res = client.ft().aggregate(req)
+        assert len(res["results"]) == 1
+        assert res["results"][0]["extra_attributes"] == {"t1": "b"}
 
 
 @pytest.mark.redismod
 def test_aggregations_load(client):
     client.ft().create_index((TextField("t1"), TextField("t2")))
 
     client.ft().client.hset("doc1", mapping={"t1": "hello", "t2": "world"})
 
-    # load t1
-    req = aggregations.AggregateRequest("*").load("t1")
-    res = client.ft().aggregate(req)
-    assert res.rows[0] == ["t1", "hello"]
+    if is_resp2_connection(client):
+        # load t1
+        req = aggregations.AggregateRequest("*").load("t1")
+        res = client.ft().aggregate(req)
+        assert res.rows[0] == ["t1", "hello"]
 
-    # load t2
-    req = aggregations.AggregateRequest("*").load("t2")
-    res = client.ft().aggregate(req)
-    assert res.rows[0] == ["t2", "world"]
+        # load t2
+        req = aggregations.AggregateRequest("*").load("t2")
+        res = client.ft().aggregate(req)
+        assert res.rows[0] == ["t2", "world"]
 
-    # load all
-    req = aggregations.AggregateRequest("*").load()
-    res = client.ft().aggregate(req)
-    assert res.rows[0] == ["t1", "hello", "t2", "world"]
+        # load all
+        req = aggregations.AggregateRequest("*").load()
+        res = client.ft().aggregate(req)
+        assert res.rows[0] == ["t1", "hello", "t2", "world"]
+    else:
+        # load t1
+        req = aggregations.AggregateRequest("*").load("t1")
+        res = client.ft().aggregate(req)
+        assert res["results"][0]["extra_attributes"] == {"t1": "hello"}
+
+        # load t2
+        req = aggregations.AggregateRequest("*").load("t2")
+        res = client.ft().aggregate(req)
+        assert res["results"][0]["extra_attributes"] == {"t2": "world"}
+
+        # load all
+        req = aggregations.AggregateRequest("*").load()
+        res = client.ft().aggregate(req)
+        assert res["results"][0]["extra_attributes"] == {"t1": "hello", "t2": "world"}
 
 
 @pytest.mark.redismod
 def test_aggregations_apply(client):
     client.ft().create_index(
         (
             TextField("PrimaryKey", sortable=True),
@@ -958,16 +1379,25 @@
         mapping={"PrimaryKey": "9::362329", "CreatedDateTimeUTC": "637387875859270016"},
     )
 
     req = aggregations.AggregateRequest("*").apply(
         CreatedDateTimeUTC="@CreatedDateTimeUTC * 10"
     )
     res = client.ft().aggregate(req)
-    res_set = set([res.rows[0][1], res.rows[1][1]])
-    assert res_set == set(["6373878785249699840", "6373878758592700416"])
+    if is_resp2_connection(client):
+        res_set = set([res.rows[0][1], res.rows[1][1]])
+        assert res_set == set(["6373878785249699840", "6373878758592700416"])
+    else:
+        res_set = set(
+            [
+                res["results"][0]["extra_attributes"]["CreatedDateTimeUTC"],
+                res["results"][1]["extra_attributes"]["CreatedDateTimeUTC"],
+            ],
+        )
+        assert res_set == set(["6373878785249699840", "6373878758592700416"])
 
 
 @pytest.mark.redismod
 def test_aggregations_filter(client):
     client.ft().create_index(
         (TextField("name", sortable=True), NumericField("age", sortable=True))
     )
@@ -978,27 +1408,42 @@
     for dialect in [1, 2]:
         req = (
             aggregations.AggregateRequest("*")
             .filter("@name=='foo' && @age < 20")
             .dialect(dialect)
         )
         res = client.ft().aggregate(req)
-        assert len(res.rows) == 1
-        assert res.rows[0] == ["name", "foo", "age", "19"]
-
-        req = (
-            aggregations.AggregateRequest("*")
-            .filter("@age > 15")
-            .sort_by("@age")
-            .dialect(dialect)
-        )
-        res = client.ft().aggregate(req)
-        assert len(res.rows) == 2
-        assert res.rows[0] == ["age", "19"]
-        assert res.rows[1] == ["age", "25"]
+        if is_resp2_connection(client):
+            assert len(res.rows) == 1
+            assert res.rows[0] == ["name", "foo", "age", "19"]
+
+            req = (
+                aggregations.AggregateRequest("*")
+                .filter("@age > 15")
+                .sort_by("@age")
+                .dialect(dialect)
+            )
+            res = client.ft().aggregate(req)
+            assert len(res.rows) == 2
+            assert res.rows[0] == ["age", "19"]
+            assert res.rows[1] == ["age", "25"]
+        else:
+            assert len(res["results"]) == 1
+            assert res["results"][0]["extra_attributes"] == {"name": "foo", "age": "19"}
+
+            req = (
+                aggregations.AggregateRequest("*")
+                .filter("@age > 15")
+                .sort_by("@age")
+                .dialect(dialect)
+            )
+            res = client.ft().aggregate(req)
+            assert len(res["results"]) == 2
+            assert res["results"][0]["extra_attributes"] == {"age": "19"}
+            assert res["results"][1]["extra_attributes"] == {"age": "25"}
 
 
 @pytest.mark.redismod
 @skip_ifmodversion_lt("2.0.0", "search")
 def test_index_definition(client):
     """
     Create definition and test its args
@@ -1056,15 +1501,19 @@
 
 @pytest.mark.redismod
 def test_skip_initial_scan(client):
     client.hset("doc1", "foo", "bar")
     q = Query("@foo:bar")
 
     client.ft().create_index((TextField("foo"),), skip_initial_scan=True)
-    assert 0 == client.ft().search(q).total
+    res = client.ft().search(q)
+    if is_resp2_connection(client):
+        assert res.total == 0
+    else:
+        assert res["total_results"] == 0
 
 
 @pytest.mark.redismod
 def test_summarize_disabled_nooffset(client):
     client.ft().create_index((TextField("txt"),), no_term_offsets=True)
     client.hset("doc1", mapping={"txt": "foo bar"})
     with pytest.raises(Exception):
@@ -1144,18 +1593,23 @@
     definition = IndexDefinition(prefix=["king:"], index_type=IndexType.JSON)
     client.ft().create_index((TextField("$.name"),), definition=definition)
 
     client.json().set("king:1", Path.root_path(), {"name": "henry"})
     client.json().set("king:2", Path.root_path(), {"name": "james"})
 
     res = client.ft().search("henry")
-    assert res.docs[0].id == "king:1"
-    assert res.docs[0].payload is None
-    assert res.docs[0].json == '{"name":"henry"}'
-    assert res.total == 1
+    if is_resp2_connection(client):
+        assert res.docs[0].id == "king:1"
+        assert res.docs[0].payload is None
+        assert res.docs[0].json == '{"name":"henry"}'
+        assert res.total == 1
+    else:
+        assert res["results"][0]["id"] == "king:1"
+        assert res["results"][0]["extra_attributes"]["$"] == '{"name":"henry"}'
+        assert res["total_results"] == 1
 
 
 @pytest.mark.redismod
 @skip_ifmodversion_lt("2.2.0", "search")
 def test_fields_as_name(client):
     # create index
     SCHEMA = (
@@ -1165,44 +1619,59 @@
     definition = IndexDefinition(index_type=IndexType.JSON)
     client.ft().create_index(SCHEMA, definition=definition)
 
     # insert json data
     res = client.json().set("doc:1", Path.root_path(), {"name": "Jon", "age": 25})
     assert res
 
-    total = client.ft().search(Query("Jon").return_fields("name", "just_a_number")).docs
-    assert 1 == len(total)
-    assert "doc:1" == total[0].id
-    assert "Jon" == total[0].name
-    assert "25" == total[0].just_a_number
+    res = client.ft().search(Query("Jon").return_fields("name", "just_a_number"))
+    if is_resp2_connection(client):
+        assert 1 == len(res.docs)
+        assert "doc:1" == res.docs[0].id
+        assert "Jon" == res.docs[0].name
+        assert "25" == res.docs[0].just_a_number
+    else:
+        assert 1 == len(res["results"])
+        assert "doc:1" == res["results"][0]["id"]
+        assert "Jon" == res["results"][0]["extra_attributes"]["name"]
+        assert "25" == res["results"][0]["extra_attributes"]["just_a_number"]
 
 
 @pytest.mark.redismod
 def test_casesensitive(client):
     # create index
     SCHEMA = (TagField("t", case_sensitive=False),)
     client.ft().create_index(SCHEMA)
     client.ft().client.hset("1", "t", "HELLO")
     client.ft().client.hset("2", "t", "hello")
 
-    res = client.ft().search("@t:{HELLO}").docs
+    res = client.ft().search("@t:{HELLO}")
 
-    assert 2 == len(res)
-    assert "1" == res[0].id
-    assert "2" == res[1].id
+    if is_resp2_connection(client):
+        assert 2 == len(res.docs)
+        assert "1" == res.docs[0].id
+        assert "2" == res.docs[1].id
+    else:
+        assert 2 == len(res["results"])
+        assert "1" == res["results"][0]["id"]
+        assert "2" == res["results"][1]["id"]
 
     # create casesensitive index
     client.ft().dropindex()
     SCHEMA = (TagField("t", case_sensitive=True),)
     client.ft().create_index(SCHEMA)
     waitForIndex(client, getattr(client.ft(), "index_name", "idx"))
 
-    res = client.ft().search("@t:{HELLO}").docs
-    assert 1 == len(res)
-    assert "1" == res[0].id
+    res = client.ft().search("@t:{HELLO}")
+    if is_resp2_connection(client):
+        assert 1 == len(res.docs)
+        assert "1" == res.docs[0].id
+    else:
+        assert 1 == len(res["results"])
+        assert "1" == res["results"][0]["id"]
 
 
 @pytest.mark.redismod
 @skip_ifmodversion_lt("2.2.0", "search")
 def test_search_return_fields(client):
     res = client.json().set(
         "doc:1",
@@ -1213,23 +1682,34 @@
 
     # create index on
     definition = IndexDefinition(index_type=IndexType.JSON)
     SCHEMA = (TextField("$.t"), NumericField("$.flt"))
     client.ft().create_index(SCHEMA, definition=definition)
     waitForIndex(client, getattr(client.ft(), "index_name", "idx"))
 
-    total = client.ft().search(Query("*").return_field("$.t", as_field="txt")).docs
-    assert 1 == len(total)
-    assert "doc:1" == total[0].id
-    assert "riceratops" == total[0].txt
-
-    total = client.ft().search(Query("*").return_field("$.t2", as_field="txt")).docs
-    assert 1 == len(total)
-    assert "doc:1" == total[0].id
-    assert "telmatosaurus" == total[0].txt
+    if is_resp2_connection(client):
+        total = client.ft().search(Query("*").return_field("$.t", as_field="txt")).docs
+        assert 1 == len(total)
+        assert "doc:1" == total[0].id
+        assert "riceratops" == total[0].txt
+
+        total = client.ft().search(Query("*").return_field("$.t2", as_field="txt")).docs
+        assert 1 == len(total)
+        assert "doc:1" == total[0].id
+        assert "telmatosaurus" == total[0].txt
+    else:
+        total = client.ft().search(Query("*").return_field("$.t", as_field="txt"))
+        assert 1 == len(total["results"])
+        assert "doc:1" == total["results"][0]["id"]
+        assert "riceratops" == total["results"][0]["extra_attributes"]["txt"]
+
+        total = client.ft().search(Query("*").return_field("$.t2", as_field="txt"))
+        assert 1 == len(total["results"])
+        assert "doc:1" == total["results"][0]["id"]
+        assert "telmatosaurus" == total["results"][0]["extra_attributes"]["txt"]
 
 
 @pytest.mark.redismod
 def test_synupdate(client):
     definition = IndexDefinition(index_type=IndexType.HASH)
     client.ft().create_index(
         (TextField("title"), TextField("body")), definition=definition
@@ -1238,17 +1718,22 @@
     client.ft().synupdate("id1", True, "boy", "child", "offspring")
     client.hset("doc1", mapping={"title": "he is a baby", "body": "this is a test"})
 
     client.ft().synupdate("id1", True, "baby")
     client.hset("doc2", mapping={"title": "he is another baby", "body": "another test"})
 
     res = client.ft().search(Query("child").expander("SYNONYM"))
-    assert res.docs[0].id == "doc2"
-    assert res.docs[0].title == "he is another baby"
-    assert res.docs[0].body == "another test"
+    if is_resp2_connection(client):
+        assert res.docs[0].id == "doc2"
+        assert res.docs[0].title == "he is another baby"
+        assert res.docs[0].body == "another test"
+    else:
+        assert res["results"][0]["id"] == "doc2"
+        assert res["results"][0]["extra_attributes"]["title"] == "he is another baby"
+        assert res["results"][0]["extra_attributes"]["body"] == "another test"
 
 
 @pytest.mark.redismod
 def test_syndump(client):
     definition = IndexDefinition(index_type=IndexType.HASH)
     client.ft().create_index(
         (TextField("title"), TextField("body")), definition=definition
@@ -1280,23 +1765,36 @@
         (TextField("$.name", as_name="name"), NumericField("$.num", as_name="num")),
         definition=definition,
     )
 
     client.json().set("king:1", Path.root_path(), {"name": "henry", "num": 42})
     client.json().set("king:2", Path.root_path(), {"name": "james", "num": 3.14})
 
-    res = client.ft().search("@name:henry")
-    assert res.docs[0].id == "king:1"
-    assert res.docs[0].json == '{"name":"henry","num":42}'
-    assert res.total == 1
-
-    res = client.ft().search("@num:[0 10]")
-    assert res.docs[0].id == "king:2"
-    assert res.docs[0].json == '{"name":"james","num":3.14}'
-    assert res.total == 1
+    if is_resp2_connection(client):
+        res = client.ft().search("@name:henry")
+        assert res.docs[0].id == "king:1"
+        assert res.docs[0].json == '{"name":"henry","num":42}'
+        assert res.total == 1
+
+        res = client.ft().search("@num:[0 10]")
+        assert res.docs[0].id == "king:2"
+        assert res.docs[0].json == '{"name":"james","num":3.14}'
+        assert res.total == 1
+    else:
+        res = client.ft().search("@name:henry")
+        assert res["results"][0]["id"] == "king:1"
+        assert res["results"][0]["extra_attributes"]["$"] == '{"name":"henry","num":42}'
+        assert res["total_results"] == 1
+
+        res = client.ft().search("@num:[0 10]")
+        assert res["results"][0]["id"] == "king:2"
+        assert (
+            res["results"][0]["extra_attributes"]["$"] == '{"name":"james","num":3.14}'
+        )
+        assert res["total_results"] == 1
 
     # Tests returns an error if path contain special characters (user should
     # use an alias)
     with pytest.raises(Exception):
         client.ft().search("@$.name:henry")
 
 
@@ -1312,23 +1810,40 @@
         (TagField("$..name", as_name="name")), definition=definition
     )
 
     client.json().set(
         "king:1", Path.root_path(), {"name": "henry", "country": {"name": "england"}}
     )
 
-    res = client.ft().search("@name:{henry}")
-    assert res.docs[0].id == "king:1"
-    assert res.docs[0].json == '{"name":"henry","country":{"name":"england"}}'
-    assert res.total == 1
-
-    res = client.ft().search("@name:{england}")
-    assert res.docs[0].id == "king:1"
-    assert res.docs[0].json == '{"name":"henry","country":{"name":"england"}}'
-    assert res.total == 1
+    if is_resp2_connection(client):
+        res = client.ft().search("@name:{henry}")
+        assert res.docs[0].id == "king:1"
+        assert res.docs[0].json == '{"name":"henry","country":{"name":"england"}}'
+        assert res.total == 1
+
+        res = client.ft().search("@name:{england}")
+        assert res.docs[0].id == "king:1"
+        assert res.docs[0].json == '{"name":"henry","country":{"name":"england"}}'
+        assert res.total == 1
+    else:
+        res = client.ft().search("@name:{henry}")
+        assert res["results"][0]["id"] == "king:1"
+        assert (
+            res["results"][0]["extra_attributes"]["$"]
+            == '{"name":"henry","country":{"name":"england"}}'
+        )
+        assert res["total_results"] == 1
+
+        res = client.ft().search("@name:{england}")
+        assert res["results"][0]["id"] == "king:1"
+        assert (
+            res["results"][0]["extra_attributes"]["$"]
+            == '{"name":"henry","country":{"name":"england"}}'
+        )
+        assert res["total_results"] == 1
 
 
 @pytest.mark.redismod
 @skip_ifmodversion_lt("2.2.0", "search")
 def test_json_with_jsonpath(client):
     definition = IndexDefinition(index_type=IndexType.JSON)
     client.ft().create_index(
@@ -1337,302 +1852,418 @@
             TextField("$.prod:name", as_name="name_unsupported"),
         ),
         definition=definition,
     )
 
     client.json().set("doc:1", Path.root_path(), {"prod:name": "RediSearch"})
 
-    # query for a supported field succeeds
-    res = client.ft().search(Query("@name:RediSearch"))
-    assert res.total == 1
-    assert res.docs[0].id == "doc:1"
-    assert res.docs[0].json == '{"prod:name":"RediSearch"}'
-
-    # query for an unsupported field
-    res = client.ft().search("@name_unsupported:RediSearch")
-    assert res.total == 1
-
-    # return of a supported field succeeds
-    res = client.ft().search(Query("@name:RediSearch").return_field("name"))
-    assert res.total == 1
-    assert res.docs[0].id == "doc:1"
-    assert res.docs[0].name == "RediSearch"
+    if is_resp2_connection(client):
+        # query for a supported field succeeds
+        res = client.ft().search(Query("@name:RediSearch"))
+        assert res.total == 1
+        assert res.docs[0].id == "doc:1"
+        assert res.docs[0].json == '{"prod:name":"RediSearch"}'
+
+        # query for an unsupported field
+        res = client.ft().search("@name_unsupported:RediSearch")
+        assert res.total == 1
+
+        # return of a supported field succeeds
+        res = client.ft().search(Query("@name:RediSearch").return_field("name"))
+        assert res.total == 1
+        assert res.docs[0].id == "doc:1"
+        assert res.docs[0].name == "RediSearch"
+    else:
+        # query for a supported field succeeds
+        res = client.ft().search(Query("@name:RediSearch"))
+        assert res["total_results"] == 1
+        assert res["results"][0]["id"] == "doc:1"
+        assert (
+            res["results"][0]["extra_attributes"]["$"] == '{"prod:name":"RediSearch"}'
+        )
+
+        # query for an unsupported field
+        res = client.ft().search("@name_unsupported:RediSearch")
+        assert res["total_results"] == 1
+
+        # return of a supported field succeeds
+        res = client.ft().search(Query("@name:RediSearch").return_field("name"))
+        assert res["total_results"] == 1
+        assert res["results"][0]["id"] == "doc:1"
+        assert res["results"][0]["extra_attributes"]["name"] == "RediSearch"
 
 
 @pytest.mark.redismod
 @pytest.mark.onlynoncluster
 @skip_if_redis_enterprise()
 def test_profile(client):
     client.ft().create_index((TextField("t"),))
     client.ft().client.hset("1", "t", "hello")
     client.ft().client.hset("2", "t", "world")
 
     # check using Query
     q = Query("hello|world").no_content()
-    res, det = client.ft().profile(q)
-    assert det["Iterators profile"]["Counter"] == 2.0
-    assert len(det["Iterators profile"]["Child iterators"]) == 2
-    assert det["Iterators profile"]["Type"] == "UNION"
-    assert det["Parsing time"] < 0.5
-    assert len(res.docs) == 2  # check also the search result
-
-    # check using AggregateRequest
-    req = (
-        aggregations.AggregateRequest("*")
-        .load("t")
-        .apply(prefix="startswith(@t, 'hel')")
-    )
-    res, det = client.ft().profile(req)
-    assert det["Iterators profile"]["Counter"] == 2.0
-    assert det["Iterators profile"]["Type"] == "WILDCARD"
-    assert isinstance(det["Parsing time"], float)
-    assert len(res.rows) == 2  # check also the search result
+    if is_resp2_connection(client):
+        res, det = client.ft().profile(q)
+        assert det["Iterators profile"]["Counter"] == 2.0
+        assert len(det["Iterators profile"]["Child iterators"]) == 2
+        assert det["Iterators profile"]["Type"] == "UNION"
+        assert det["Parsing time"] < 0.5
+        assert len(res.docs) == 2  # check also the search result
+
+        # check using AggregateRequest
+        req = (
+            aggregations.AggregateRequest("*")
+            .load("t")
+            .apply(prefix="startswith(@t, 'hel')")
+        )
+        res, det = client.ft().profile(req)
+        assert det["Iterators profile"]["Counter"] == 2
+        assert det["Iterators profile"]["Type"] == "WILDCARD"
+        assert isinstance(det["Parsing time"], float)
+        assert len(res.rows) == 2  # check also the search result
+    else:
+        res = client.ft().profile(q)
+        assert res["profile"]["Iterators profile"][0]["Counter"] == 2.0
+        assert res["profile"]["Iterators profile"][0]["Type"] == "UNION"
+        assert res["profile"]["Parsing time"] < 0.5
+        assert len(res["results"]) == 2  # check also the search result
+
+        # check using AggregateRequest
+        req = (
+            aggregations.AggregateRequest("*")
+            .load("t")
+            .apply(prefix="startswith(@t, 'hel')")
+        )
+        res = client.ft().profile(req)
+        assert res["profile"]["Iterators profile"][0]["Counter"] == 2
+        assert res["profile"]["Iterators profile"][0]["Type"] == "WILDCARD"
+        assert isinstance(res["profile"]["Parsing time"], float)
+        assert len(res["results"]) == 2  # check also the search result
 
 
 @pytest.mark.redismod
 @pytest.mark.onlynoncluster
 def test_profile_limited(client):
     client.ft().create_index((TextField("t"),))
     client.ft().client.hset("1", "t", "hello")
     client.ft().client.hset("2", "t", "hell")
     client.ft().client.hset("3", "t", "help")
     client.ft().client.hset("4", "t", "helowa")
 
     q = Query("%hell% hel*")
-    res, det = client.ft().profile(q, limited=True)
-    assert (
-        det["Iterators profile"]["Child iterators"][0]["Child iterators"]
-        == "The number of iterators in the union is 3"
-    )
-    assert (
-        det["Iterators profile"]["Child iterators"][1]["Child iterators"]
-        == "The number of iterators in the union is 4"
-    )
-    assert det["Iterators profile"]["Type"] == "INTERSECT"
-    assert len(res.docs) == 3  # check also the search result
+    if is_resp2_connection(client):
+        res, det = client.ft().profile(q, limited=True)
+        assert (
+            det["Iterators profile"]["Child iterators"][0]["Child iterators"]
+            == "The number of iterators in the union is 3"
+        )
+        assert (
+            det["Iterators profile"]["Child iterators"][1]["Child iterators"]
+            == "The number of iterators in the union is 4"
+        )
+        assert det["Iterators profile"]["Type"] == "INTERSECT"
+        assert len(res.docs) == 3  # check also the search result
+    else:
+        res = client.ft().profile(q, limited=True)
+        iterators_profile = res["profile"]["Iterators profile"]
+        assert (
+            iterators_profile[0]["Child iterators"][0]["Child iterators"]
+            == "The number of iterators in the union is 3"
+        )
+        assert (
+            iterators_profile[0]["Child iterators"][1]["Child iterators"]
+            == "The number of iterators in the union is 4"
+        )
+        assert iterators_profile[0]["Type"] == "INTERSECT"
+        assert len(res["results"]) == 3  # check also the search result
 
 
 @pytest.mark.redismod
 @skip_ifmodversion_lt("2.4.3", "search")
-def test_profile_query_params(modclient: redis.Redis):
-    modclient.flushdb()
-    modclient.ft().create_index(
+def test_profile_query_params(client):
+    client.ft().create_index(
         (
             VectorField(
                 "v", "HNSW", {"TYPE": "FLOAT32", "DIM": 2, "DISTANCE_METRIC": "L2"}
             ),
         )
     )
-    modclient.hset("a", "v", "aaaaaaaa")
-    modclient.hset("b", "v", "aaaabaaa")
-    modclient.hset("c", "v", "aaaaabaa")
+    client.hset("a", "v", "aaaaaaaa")
+    client.hset("b", "v", "aaaabaaa")
+    client.hset("c", "v", "aaaaabaa")
     query = "*=>[KNN 2 @v $vec]"
     q = Query(query).return_field("__v_score").sort_by("__v_score", True).dialect(2)
-    res, det = modclient.ft().profile(q, query_params={"vec": "aaaaaaaa"})
-    assert det["Iterators profile"]["Counter"] == 2.0
-    assert det["Iterators profile"]["Type"] == "VECTOR"
-    assert res.total == 2
-    assert "a" == res.docs[0].id
-    assert "0" == res.docs[0].__getattribute__("__v_score")
+    if is_resp2_connection(client):
+        res, det = client.ft().profile(q, query_params={"vec": "aaaaaaaa"})
+        assert det["Iterators profile"]["Counter"] == 2.0
+        assert det["Iterators profile"]["Type"] == "VECTOR"
+        assert res.total == 2
+        assert "a" == res.docs[0].id
+        assert "0" == res.docs[0].__getattribute__("__v_score")
+    else:
+        res = client.ft().profile(q, query_params={"vec": "aaaaaaaa"})
+        assert res["profile"]["Iterators profile"][0]["Counter"] == 2
+        assert res["profile"]["Iterators profile"][0]["Type"] == "VECTOR"
+        assert res["total_results"] == 2
+        assert "a" == res["results"][0]["id"]
+        assert "0" == res["results"][0]["extra_attributes"]["__v_score"]
 
 
 @pytest.mark.redismod
 @skip_ifmodversion_lt("2.4.3", "search")
-def test_vector_field(modclient):
-    modclient.flushdb()
-    modclient.ft().create_index(
+def test_vector_field(client):
+    client.flushdb()
+    client.ft().create_index(
         (
             VectorField(
                 "v", "HNSW", {"TYPE": "FLOAT32", "DIM": 2, "DISTANCE_METRIC": "L2"}
             ),
         )
     )
-    modclient.hset("a", "v", "aaaaaaaa")
-    modclient.hset("b", "v", "aaaabaaa")
-    modclient.hset("c", "v", "aaaaabaa")
+    client.hset("a", "v", "aaaaaaaa")
+    client.hset("b", "v", "aaaabaaa")
+    client.hset("c", "v", "aaaaabaa")
 
     query = "*=>[KNN 2 @v $vec]"
     q = Query(query).return_field("__v_score").sort_by("__v_score", True).dialect(2)
-    res = modclient.ft().search(q, query_params={"vec": "aaaaaaaa"})
+    res = client.ft().search(q, query_params={"vec": "aaaaaaaa"})
 
-    assert "a" == res.docs[0].id
-    assert "0" == res.docs[0].__getattribute__("__v_score")
+    if is_resp2_connection(client):
+        assert "a" == res.docs[0].id
+        assert "0" == res.docs[0].__getattribute__("__v_score")
+    else:
+        assert "a" == res["results"][0]["id"]
+        assert "0" == res["results"][0]["extra_attributes"]["__v_score"]
 
 
 @pytest.mark.redismod
 @skip_ifmodversion_lt("2.4.3", "search")
-def test_vector_field_error(modclient):
-    modclient.flushdb()
+def test_vector_field_error(r):
+    r.flushdb()
 
     # sortable tag
     with pytest.raises(Exception):
-        modclient.ft().create_index((VectorField("v", "HNSW", {}, sortable=True),))
+        r.ft().create_index((VectorField("v", "HNSW", {}, sortable=True),))
 
     # not supported algorithm
     with pytest.raises(Exception):
-        modclient.ft().create_index((VectorField("v", "SORT", {}),))
+        r.ft().create_index((VectorField("v", "SORT", {}),))
 
 
 @pytest.mark.redismod
 @skip_ifmodversion_lt("2.4.3", "search")
-def test_text_params(modclient):
-    modclient.flushdb()
-    modclient.ft().create_index((TextField("name"),))
-
-    modclient.hset("doc1", mapping={"name": "Alice"})
-    modclient.hset("doc2", mapping={"name": "Bob"})
-    modclient.hset("doc3", mapping={"name": "Carol"})
+def test_text_params(client):
+    client.flushdb()
+    client.ft().create_index((TextField("name"),))
+
+    client.hset("doc1", mapping={"name": "Alice"})
+    client.hset("doc2", mapping={"name": "Bob"})
+    client.hset("doc3", mapping={"name": "Carol"})
 
     params_dict = {"name1": "Alice", "name2": "Bob"}
     q = Query("@name:($name1 | $name2 )").dialect(2)
-    res = modclient.ft().search(q, query_params=params_dict)
-    assert 2 == res.total
-    assert "doc1" == res.docs[0].id
-    assert "doc2" == res.docs[1].id
+    res = client.ft().search(q, query_params=params_dict)
+    if is_resp2_connection(client):
+        assert 2 == res.total
+        assert "doc1" == res.docs[0].id
+        assert "doc2" == res.docs[1].id
+    else:
+        assert 2 == res["total_results"]
+        assert "doc1" == res["results"][0]["id"]
+        assert "doc2" == res["results"][1]["id"]
 
 
 @pytest.mark.redismod
 @skip_ifmodversion_lt("2.4.3", "search")
-def test_numeric_params(modclient):
-    modclient.flushdb()
-    modclient.ft().create_index((NumericField("numval"),))
-
-    modclient.hset("doc1", mapping={"numval": 101})
-    modclient.hset("doc2", mapping={"numval": 102})
-    modclient.hset("doc3", mapping={"numval": 103})
+def test_numeric_params(client):
+    client.flushdb()
+    client.ft().create_index((NumericField("numval"),))
+
+    client.hset("doc1", mapping={"numval": 101})
+    client.hset("doc2", mapping={"numval": 102})
+    client.hset("doc3", mapping={"numval": 103})
 
     params_dict = {"min": 101, "max": 102}
     q = Query("@numval:[$min $max]").dialect(2)
-    res = modclient.ft().search(q, query_params=params_dict)
+    res = client.ft().search(q, query_params=params_dict)
 
-    assert 2 == res.total
-    assert "doc1" == res.docs[0].id
-    assert "doc2" == res.docs[1].id
+    if is_resp2_connection(client):
+        assert 2 == res.total
+        assert "doc1" == res.docs[0].id
+        assert "doc2" == res.docs[1].id
+    else:
+        assert 2 == res["total_results"]
+        assert "doc1" == res["results"][0]["id"]
+        assert "doc2" == res["results"][1]["id"]
 
 
 @pytest.mark.redismod
 @skip_ifmodversion_lt("2.4.3", "search")
-def test_geo_params(modclient):
+def test_geo_params(client):
 
-    modclient.flushdb()
-    modclient.ft().create_index((GeoField("g")))
-    modclient.hset("doc1", mapping={"g": "29.69465, 34.95126"})
-    modclient.hset("doc2", mapping={"g": "29.69350, 34.94737"})
-    modclient.hset("doc3", mapping={"g": "29.68746, 34.94882"})
+    client.ft().create_index((GeoField("g")))
+    client.hset("doc1", mapping={"g": "29.69465, 34.95126"})
+    client.hset("doc2", mapping={"g": "29.69350, 34.94737"})
+    client.hset("doc3", mapping={"g": "29.68746, 34.94882"})
 
     params_dict = {"lat": "34.95126", "lon": "29.69465", "radius": 1000, "units": "km"}
     q = Query("@g:[$lon $lat $radius $units]").dialect(2)
-    res = modclient.ft().search(q, query_params=params_dict)
-    assert 3 == res.total
-    assert "doc1" == res.docs[0].id
-    assert "doc2" == res.docs[1].id
-    assert "doc3" == res.docs[2].id
+    res = client.ft().search(q, query_params=params_dict)
+    if is_resp2_connection(client):
+        assert 3 == res.total
+        assert "doc1" == res.docs[0].id
+        assert "doc2" == res.docs[1].id
+        assert "doc3" == res.docs[2].id
+    else:
+        assert 3 == res["total_results"]
+        assert "doc1" == res["results"][0]["id"]
+        assert "doc2" == res["results"][1]["id"]
+        assert "doc3" == res["results"][2]["id"]
 
 
 @pytest.mark.redismod
 @skip_if_redis_enterprise()
 def test_search_commands_in_pipeline(client):
     p = client.ft().pipeline()
     p.create_index((TextField("txt"),))
     p.hset("doc1", mapping={"txt": "foo bar"})
     p.hset("doc2", mapping={"txt": "foo bar"})
     q = Query("foo bar").with_payloads()
     p.search(q)
     res = p.execute()
-    assert res[:3] == ["OK", True, True]
-    assert 2 == res[3][0]
-    assert "doc1" == res[3][1]
-    assert "doc2" == res[3][4]
-    assert res[3][5] is None
-    assert res[3][3] == res[3][6] == ["txt", "foo bar"]
+    if is_resp2_connection(client):
+        assert res[:3] == ["OK", True, True]
+        assert 2 == res[3][0]
+        assert "doc1" == res[3][1]
+        assert "doc2" == res[3][4]
+        assert res[3][5] is None
+        assert res[3][3] == res[3][6] == ["txt", "foo bar"]
+    else:
+        assert res[:3] == ["OK", True, True]
+        assert 2 == res[3]["total_results"]
+        assert "doc1" == res[3]["results"][0]["id"]
+        assert "doc2" == res[3]["results"][1]["id"]
+        assert res[3]["results"][0]["payload"] is None
+        assert (
+            res[3]["results"][0]["extra_attributes"]
+            == res[3]["results"][1]["extra_attributes"]
+            == {"txt": "foo bar"}
+        )
 
 
 @pytest.mark.redismod
 @pytest.mark.onlynoncluster
 @skip_ifmodversion_lt("2.4.3", "search")
-def test_dialect_config(modclient: redis.Redis):
-    assert modclient.ft().config_get("DEFAULT_DIALECT") == {"DEFAULT_DIALECT": "1"}
-    assert modclient.ft().config_set("DEFAULT_DIALECT", 2)
-    assert modclient.ft().config_get("DEFAULT_DIALECT") == {"DEFAULT_DIALECT": "2"}
+def test_dialect_config(client):
+    assert client.ft().config_get("DEFAULT_DIALECT")
+    client.ft().config_set("DEFAULT_DIALECT", 2)
+    assert client.ft().config_get("DEFAULT_DIALECT") == {"DEFAULT_DIALECT": "2"}
     with pytest.raises(redis.ResponseError):
-        modclient.ft().config_set("DEFAULT_DIALECT", 0)
+        client.ft().config_set("DEFAULT_DIALECT", 0)
 
 
 @pytest.mark.redismod
 @skip_ifmodversion_lt("2.4.3", "search")
-def test_dialect(modclient: redis.Redis):
-    modclient.ft().create_index(
+def test_dialect(client):
+    client.ft().create_index(
         (
             TagField("title"),
             TextField("t1"),
             TextField("t2"),
             NumericField("num"),
             VectorField(
                 "v", "HNSW", {"TYPE": "FLOAT32", "DIM": 1, "DISTANCE_METRIC": "COSINE"}
             ),
         )
     )
-    modclient.hset("h", "t1", "hello")
+    client.hset("h", "t1", "hello")
     with pytest.raises(redis.ResponseError) as err:
-        modclient.ft().explain(Query("(*)").dialect(1))
+        client.ft().explain(Query("(*)").dialect(1))
     assert "Syntax error" in str(err)
-    assert "WILDCARD" in modclient.ft().explain(Query("(*)").dialect(2))
+    assert "WILDCARD" in client.ft().explain(Query("(*)").dialect(2))
 
     with pytest.raises(redis.ResponseError) as err:
-        modclient.ft().explain(Query("$hello").dialect(1))
+        client.ft().explain(Query("$hello").dialect(1))
     assert "Syntax error" in str(err)
     q = Query("$hello").dialect(2)
     expected = "UNION {\n  hello\n  +hello(expanded)\n}\n"
-    assert expected in modclient.ft().explain(q, query_params={"hello": "hello"})
+    assert expected in client.ft().explain(q, query_params={"hello": "hello"})
 
     expected = "NUMERIC {0.000000 <= @num <= 10.000000}\n"
-    assert expected in modclient.ft().explain(Query("@title:(@num:[0 10])").dialect(1))
+    assert expected in client.ft().explain(Query("@title:(@num:[0 10])").dialect(1))
     with pytest.raises(redis.ResponseError) as err:
-        modclient.ft().explain(Query("@title:(@num:[0 10])").dialect(2))
+        client.ft().explain(Query("@title:(@num:[0 10])").dialect(2))
     assert "Syntax error" in str(err)
 
 
 @pytest.mark.redismod
-def test_expire_while_search(modclient: redis.Redis):
-    modclient.ft().create_index((TextField("txt"),))
-    modclient.hset("hset:1", "txt", "a")
-    modclient.hset("hset:2", "txt", "b")
-    modclient.hset("hset:3", "txt", "c")
-    assert 3 == modclient.ft().search(Query("*")).total
-    modclient.pexpire("hset:2", 300)
-    for _ in range(500):
-        modclient.ft().search(Query("*")).docs[1]
-    time.sleep(1)
-    assert 2 == modclient.ft().search(Query("*")).total
+def test_expire_while_search(client: redis.Redis):
+    client.ft().create_index((TextField("txt"),))
+    client.hset("hset:1", "txt", "a")
+    client.hset("hset:2", "txt", "b")
+    client.hset("hset:3", "txt", "c")
+    if is_resp2_connection(client):
+        assert 3 == client.ft().search(Query("*")).total
+        client.pexpire("hset:2", 300)
+        for _ in range(500):
+            client.ft().search(Query("*")).docs[1]
+        time.sleep(1)
+        assert 2 == client.ft().search(Query("*")).total
+    else:
+        assert 3 == client.ft().search(Query("*"))["total_results"]
+        client.pexpire("hset:2", 300)
+        for _ in range(500):
+            client.ft().search(Query("*"))["results"][1]
+        time.sleep(1)
+        assert 2 == client.ft().search(Query("*"))["total_results"]
 
 
 @pytest.mark.redismod
 @pytest.mark.experimental
-def test_withsuffixtrie(modclient: redis.Redis):
+def test_withsuffixtrie(client: redis.Redis):
     # create index
-    assert modclient.ft().create_index((TextField("txt"),))
-    waitForIndex(modclient, getattr(modclient.ft(), "index_name", "idx"))
-    info = modclient.ft().info()
-    assert "WITHSUFFIXTRIE" not in info["attributes"][0]
-    assert modclient.ft().dropindex("idx")
-
-    # create withsuffixtrie index (text fiels)
-    assert modclient.ft().create_index((TextField("t", withsuffixtrie=True)))
-    waitForIndex(modclient, getattr(modclient.ft(), "index_name", "idx"))
-    info = modclient.ft().info()
-    assert "WITHSUFFIXTRIE" in info["attributes"][0]
-    assert modclient.ft().dropindex("idx")
-
-    # create withsuffixtrie index (tag field)
-    assert modclient.ft().create_index((TagField("t", withsuffixtrie=True)))
-    waitForIndex(modclient, getattr(modclient.ft(), "index_name", "idx"))
-    info = modclient.ft().info()
-    assert "WITHSUFFIXTRIE" in info["attributes"][0]
+    assert client.ft().create_index((TextField("txt"),))
+    waitForIndex(client, getattr(client.ft(), "index_name", "idx"))
+    if is_resp2_connection(client):
+        info = client.ft().info()
+        assert "WITHSUFFIXTRIE" not in info["attributes"][0]
+        assert client.ft().dropindex("idx")
+
+        # create withsuffixtrie index (text fiels)
+        assert client.ft().create_index((TextField("t", withsuffixtrie=True)))
+        waitForIndex(client, getattr(client.ft(), "index_name", "idx"))
+        info = client.ft().info()
+        assert "WITHSUFFIXTRIE" in info["attributes"][0]
+        assert client.ft().dropindex("idx")
+
+        # create withsuffixtrie index (tag field)
+        assert client.ft().create_index((TagField("t", withsuffixtrie=True)))
+        waitForIndex(client, getattr(client.ft(), "index_name", "idx"))
+        info = client.ft().info()
+        assert "WITHSUFFIXTRIE" in info["attributes"][0]
+    else:
+        info = client.ft().info()
+        assert "WITHSUFFIXTRIE" not in info["attributes"][0]["flags"]
+        assert client.ft().dropindex("idx")
+
+        # create withsuffixtrie index (text fiels)
+        assert client.ft().create_index((TextField("t", withsuffixtrie=True)))
+        waitForIndex(client, getattr(client.ft(), "index_name", "idx"))
+        info = client.ft().info()
+        assert "WITHSUFFIXTRIE" in info["attributes"][0]["flags"]
+        assert client.ft().dropindex("idx")
+
+        # create withsuffixtrie index (tag field)
+        assert client.ft().create_index((TagField("t", withsuffixtrie=True)))
+        waitForIndex(client, getattr(client.ft(), "index_name", "idx"))
+        info = client.ft().info()
+        assert "WITHSUFFIXTRIE" in info["attributes"][0]["flags"]
 
 
 @pytest.mark.redismod
-def test_query_timeout(modclient: redis.Redis):
+def test_query_timeout(r: redis.Redis):
     q1 = Query("foo").timeout(5000)
     assert q1.get_args() == ["foo", "TIMEOUT", 5000, "LIMIT", 0, 10]
     q2 = Query("foo").timeout("not_a_number")
     with pytest.raises(redis.ResponseError):
-        modclient.ft().search(q2)
+        r.ft().search(q2)
```

### Comparing `redis-5.0.0b4/tests/test_sentinel.py` & `redis-5.0.0rc1/tests/test_sentinel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import socket
 
 import pytest
-
 import redis.sentinel
 from redis import exceptions
 from redis.sentinel import (
     MasterNotFoundError,
     Sentinel,
     SentinelConnectionPool,
     SlaveNotFoundError,
```

### Comparing `redis-5.0.0b4/tests/test_ssl.py` & `redis-5.0.0rc1/tests/test_ssl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import socket
 import ssl
 from urllib.parse import urlparse
 
 import pytest
-
 import redis
 from redis.exceptions import ConnectionError, RedisError
 
 from .conftest import skip_if_cryptography, skip_if_nocryptography
 
 
 @pytest.mark.ssl
@@ -16,18 +15,18 @@
     """Tests for SSL connections
 
     This relies on the --redis-ssl-url purely for rebuilding the client
     and connecting to the appropriate port.
     """
 
     ROOT = os.path.join(os.path.dirname(__file__), "..")
-    CERT_DIR = os.path.abspath(os.path.join(ROOT, "docker", "stunnel", "keys"))
+    CERT_DIR = os.path.abspath(os.path.join(ROOT, "dockers", "stunnel", "keys"))
     if not os.path.isdir(CERT_DIR):  # github actions package validation case
         CERT_DIR = os.path.abspath(
-            os.path.join(ROOT, "..", "docker", "stunnel", "keys")
+            os.path.join(ROOT, "..", "dockers", "stunnel", "keys")
         )
         if not os.path.isdir(CERT_DIR):
             raise IOError(f"No SSL certificates found. They should be in {CERT_DIR}")
 
     SERVER_CERT = os.path.join(CERT_DIR, "server-cert.pem")
     SERVER_KEY = os.path.join(CERT_DIR, "server-key.pem")
```

### Comparing `redis-5.0.0b4/tests/testdata/jsontestdata.py` & `redis-5.0.0rc1/tests/testdata/jsontestdata.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/tests/testdata/titles.csv` & `redis-5.0.0rc1/tests/testdata/titles.csv`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b4/tests/testdata/will_play_text.csv.bz2` & `redis-5.0.0rc1/tests/testdata/will_play_text.csv.bz2`

 * *Files identical despite different names*

