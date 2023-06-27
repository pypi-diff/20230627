# Comparing `tmp/repid-1.2.0.tar.gz` & `tmp/repid-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repid-1.2.0.tar", last modified: Sat Jun 10 20:58:47 2023, max compression
+gzip compressed data, was "repid-1.3.0.tar", last modified: Tue Jun 27 00:53:56 2023, max compression
```

## Comparing `repid-1.2.0.tar` & `repid-1.3.0.tar`

### file list

```diff
@@ -1,79 +1,84 @@
--rw-r--r--   0        0        0     1069 2023-06-10 20:58:23.725708 repid-1.2.0/LICENSE
--rw-r--r--   0        0        0     2589 2023-06-10 20:58:23.725708 repid-1.2.0/README.md
--rw-r--r--   0        0        0     3704 2023-06-10 20:58:47.537941 repid-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      625 2023-06-10 20:58:23.729709 repid-1.2.0/repid/__init__.py
--rw-r--r--   0        0        0     1552 2023-06-10 20:58:23.729709 repid-1.2.0/repid/_asyncify.py
--rw-r--r--   0        0        0     5104 2023-06-10 20:58:23.729709 repid-1.2.0/repid/_processor.py
--rw-r--r--   0        0        0     4061 2023-06-10 20:58:23.729709 repid-1.2.0/repid/_runner.py
--rw-r--r--   0        0        0      509 2023-06-10 20:58:23.729709 repid-1.2.0/repid/actor.py
--rw-r--r--   0        0        0     2316 2023-06-10 20:58:23.729709 repid-1.2.0/repid/config.py
--rw-r--r--   0        0        0     4525 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connection.py
--rw-r--r--   0        0        0      760 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/__init__.py
--rw-r--r--   0        0        0     6594 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/abc.py
--rw-r--r--   0        0        0      314 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/dummy/__init__.py
--rw-r--r--   0        0        0      260 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/in_memory/__init__.py
--rw-r--r--   0        0        0     1823 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/in_memory/bucket_broker.py
--rw-r--r--   0        0        0     2765 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/in_memory/consumer.py
--rw-r--r--   0        0        0     4093 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/in_memory/message_broker.py
--rw-r--r--   0        0        0      860 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/in_memory/utils.py
--rw-r--r--   0        0        0       90 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/rabbitmq/__init__.py
--rw-r--r--   0        0        0     6161 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/rabbitmq/consumer.py
--rw-r--r--   0        0        0     7091 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/rabbitmq/message_broker.py
--rw-r--r--   0        0        0      362 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/rabbitmq/protocols.py
--rw-r--r--   0        0        0      910 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/rabbitmq/utils.py
--rw-r--r--   0        0        0      158 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/redis/__init__.py
--rw-r--r--   0        0        0     1513 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/redis/bucket_broker.py
--rw-r--r--   0        0        0     7593 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/redis/consumer.py
--rw-r--r--   0        0        0     7609 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/redis/message_broker.py
--rw-r--r--   0        0        0     3818 2023-06-10 20:58:23.729709 repid-1.2.0/repid/connections/redis/utils.py
--rw-r--r--   0        0        0     1944 2023-06-10 20:58:23.729709 repid-1.2.0/repid/converter.py
--rw-r--r--   0        0        0      355 2023-06-10 20:58:23.729709 repid-1.2.0/repid/data/__init__.py
--rw-r--r--   0        0        0     2275 2023-06-10 20:58:23.729709 repid-1.2.0/repid/data/_buckets.py
--rw-r--r--   0        0        0      819 2023-06-10 20:58:23.729709 repid-1.2.0/repid/data/_key.py
--rw-r--r--   0        0        0     5509 2023-06-10 20:58:23.729709 repid-1.2.0/repid/data/_parameters.py
--rw-r--r--   0        0        0       95 2023-06-10 20:58:23.729709 repid-1.2.0/repid/data/priorities.py
--rw-r--r--   0        0        0     3859 2023-06-10 20:58:23.729709 repid-1.2.0/repid/data/protocols.py
--rw-r--r--   0        0        0     7425 2023-06-10 20:58:23.729709 repid-1.2.0/repid/job.py
--rw-r--r--   0        0        0      546 2023-06-10 20:58:23.729709 repid-1.2.0/repid/logger.py
--rw-r--r--   0        0        0     1887 2023-06-10 20:58:23.729709 repid-1.2.0/repid/main.py
--rw-r--r--   0        0        0      257 2023-06-10 20:58:23.729709 repid-1.2.0/repid/middlewares/__init__.py
--rw-r--r--   0        0        0      347 2023-06-10 20:58:23.729709 repid-1.2.0/repid/middlewares/consts.py
--rw-r--r--   0        0        0     3696 2023-06-10 20:58:23.729709 repid-1.2.0/repid/middlewares/middleware.py
--rw-r--r--   0        0        0     3647 2023-06-10 20:58:23.729709 repid-1.2.0/repid/middlewares/wrapper.py
--rw-r--r--   0        0        0        0 2023-06-10 20:58:23.729709 repid-1.2.0/repid/py.typed
--rw-r--r--   0        0        0     1064 2023-06-10 20:58:23.729709 repid-1.2.0/repid/queue.py
--rw-r--r--   0        0        0     1319 2023-06-10 20:58:23.729709 repid-1.2.0/repid/retry_policy.py
--rw-r--r--   0        0        0     5021 2023-06-10 20:58:23.729709 repid-1.2.0/repid/router.py
--rw-r--r--   0        0        0      568 2023-06-10 20:58:23.729709 repid-1.2.0/repid/serializer.py
--rw-r--r--   0        0        0      844 2023-06-10 20:58:23.729709 repid-1.2.0/repid/testing/__init__.py
--rw-r--r--   0        0        0     3183 2023-06-10 20:58:23.729709 repid-1.2.0/repid/testing/modifiers.py
--rw-r--r--   0        0        0     6099 2023-06-10 20:58:23.729709 repid-1.2.0/repid/testing/plugin.py
--rw-r--r--   0        0        0     1524 2023-06-10 20:58:23.733708 repid-1.2.0/repid/utils.py
--rw-r--r--   0        0        0     3971 2023-06-10 20:58:23.733708 repid-1.2.0/repid/worker.py
--rw-r--r--   0        0        0        0 2023-06-10 20:58:23.733708 repid-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0      758 2023-06-10 20:58:23.733708 repid-1.2.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-10 20:58:23.733708 repid-1.2.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     3241 2023-06-10 20:58:23.733708 repid-1.2.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     1337 2023-06-10 20:58:23.733708 repid-1.2.0/tests/integration/test_buckets.py
--rw-r--r--   0        0        0     4335 2023-06-10 20:58:23.733708 repid-1.2.0/tests/integration/test_consumer.py
--rw-r--r--   0        0        0     4003 2023-06-10 20:58:23.733708 repid-1.2.0/tests/integration/test_default_flow.py
--rw-r--r--   0        0        0     1904 2023-06-10 20:58:23.733708 repid-1.2.0/tests/integration/test_no_messages_lost.py
--rw-r--r--   0        0        0      431 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_actor.py
--rw-r--r--   0        0        0     3110 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_config.py
--rw-r--r--   0        0        0     2986 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_connection.py
--rw-r--r--   0        0        0     3818 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_consumer.py
--rw-r--r--   0        0        0     2835 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_consumer_abc.py
--rw-r--r--   0        0        0    10233 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_default_data_models.py
--rw-r--r--   0        0        0     3003 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_hypothesis.py
--rw-r--r--   0        0        0     3591 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_job.py
--rw-r--r--   0        0        0     1366 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_main.py
--rw-r--r--   0        0        0     7842 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_middleware.py
--rw-r--r--   0        0        0     1097 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_multiprocessing.py
--rw-r--r--   0        0        0     1484 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_pydantic.py
--rw-r--r--   0        0        0     3819 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_pytest_plugin.py
--rw-r--r--   0        0        0      414 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_queue.py
--rw-r--r--   0        0        0     3194 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_router.py
--rw-r--r--   0        0        0      764 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_serializer.py
--rw-r--r--   0        0        0     1038 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_utils.py
--rw-r--r--   0        0        0     6887 2023-06-10 20:58:23.733708 repid-1.2.0/tests/test_worker.py
--rw-r--r--   0        0        0     3942 1970-01-01 00:00:00.000000 repid-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-27 00:53:31.608839 repid-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2589 2023-06-27 00:53:31.608839 repid-1.3.0/README.md
+-rw-r--r--   0        0        0     3872 2023-06-27 00:53:56.013052 repid-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      906 2023-06-27 00:53:31.612839 repid-1.3.0/repid/__init__.py
+-rw-r--r--   0        0        0     1552 2023-06-27 00:53:31.612839 repid-1.3.0/repid/_asyncify.py
+-rw-r--r--   0        0        0     5063 2023-06-27 00:53:31.612839 repid-1.3.0/repid/_processor.py
+-rw-r--r--   0        0        0     4061 2023-06-27 00:53:31.612839 repid-1.3.0/repid/_runner.py
+-rw-r--r--   0        0        0      434 2023-06-27 00:53:31.612839 repid-1.3.0/repid/_utils/__init__.py
+-rw-r--r--   0        0        0      501 2023-06-27 00:53:31.612839 repid-1.3.0/repid/_utils/args_bucket_in_message_id.py
+-rw-r--r--   0        0        0      272 2023-06-27 00:53:31.612839 repid-1.3.0/repid/_utils/dataclass_hacks.py
+-rw-r--r--   0        0        0     1268 2023-06-27 00:53:31.612839 repid-1.3.0/repid/_utils/is_installed.py
+-rw-r--r--   0        0        0      536 2023-06-27 00:53:31.612839 repid-1.3.0/repid/_utils/json_encoder.py
+-rw-r--r--   0        0        0      135 2023-06-27 00:53:31.612839 repid-1.3.0/repid/_utils/regex_validators.py
+-rw-r--r--   0        0        0      504 2023-06-27 00:53:31.612839 repid-1.3.0/repid/actor.py
+-rw-r--r--   0        0        0     2316 2023-06-27 00:53:31.612839 repid-1.3.0/repid/config.py
+-rw-r--r--   0        0        0     4525 2023-06-27 00:53:31.612839 repid-1.3.0/repid/connection.py
+-rw-r--r--   0        0        0      761 2023-06-27 00:53:31.612839 repid-1.3.0/repid/connections/__init__.py
+-rw-r--r--   0        0        0     6594 2023-06-27 00:53:31.612839 repid-1.3.0/repid/connections/abc.py
+-rw-r--r--   0        0        0      314 2023-06-27 00:53:31.612839 repid-1.3.0/repid/connections/dummy/__init__.py
+-rw-r--r--   0        0        0      260 2023-06-27 00:53:31.612839 repid-1.3.0/repid/connections/in_memory/__init__.py
+-rw-r--r--   0        0        0     1823 2023-06-27 00:53:31.612839 repid-1.3.0/repid/connections/in_memory/bucket_broker.py
+-rw-r--r--   0        0        0     2766 2023-06-27 00:53:31.612839 repid-1.3.0/repid/connections/in_memory/consumer.py
+-rw-r--r--   0        0        0     4093 2023-06-27 00:53:31.612839 repid-1.3.0/repid/connections/in_memory/message_broker.py
+-rw-r--r--   0        0        0      860 2023-06-27 00:53:31.612839 repid-1.3.0/repid/connections/in_memory/utils.py
+-rw-r--r--   0        0        0       90 2023-06-27 00:53:31.612839 repid-1.3.0/repid/connections/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     6161 2023-06-27 00:53:31.612839 repid-1.3.0/repid/connections/rabbitmq/consumer.py
+-rw-r--r--   0        0        0     7092 2023-06-27 00:53:31.616839 repid-1.3.0/repid/connections/rabbitmq/message_broker.py
+-rw-r--r--   0        0        0      362 2023-06-27 00:53:31.616839 repid-1.3.0/repid/connections/rabbitmq/protocols.py
+-rw-r--r--   0        0        0      910 2023-06-27 00:53:31.616839 repid-1.3.0/repid/connections/rabbitmq/utils.py
+-rw-r--r--   0        0        0      158 2023-06-27 00:53:31.616839 repid-1.3.0/repid/connections/redis/__init__.py
+-rw-r--r--   0        0        0     1513 2023-06-27 00:53:31.616839 repid-1.3.0/repid/connections/redis/bucket_broker.py
+-rw-r--r--   0        0        0     7593 2023-06-27 00:53:31.616839 repid-1.3.0/repid/connections/redis/consumer.py
+-rw-r--r--   0        0        0     7609 2023-06-27 00:53:31.616839 repid-1.3.0/repid/connections/redis/message_broker.py
+-rw-r--r--   0        0        0     3818 2023-06-27 00:53:31.616839 repid-1.3.0/repid/connections/redis/utils.py
+-rw-r--r--   0        0        0     7882 2023-06-27 00:53:31.616839 repid-1.3.0/repid/converter.py
+-rw-r--r--   0        0        0      355 2023-06-27 00:53:31.616839 repid-1.3.0/repid/data/__init__.py
+-rw-r--r--   0        0        0     2276 2023-06-27 00:53:31.616839 repid-1.3.0/repid/data/_buckets.py
+-rw-r--r--   0        0        0      820 2023-06-27 00:53:31.616839 repid-1.3.0/repid/data/_key.py
+-rw-r--r--   0        0        0     5510 2023-06-27 00:53:31.616839 repid-1.3.0/repid/data/_parameters.py
+-rw-r--r--   0        0        0       95 2023-06-27 00:53:31.616839 repid-1.3.0/repid/data/priorities.py
+-rw-r--r--   0        0        0     3859 2023-06-27 00:53:31.616839 repid-1.3.0/repid/data/protocols.py
+-rw-r--r--   0        0        0     7426 2023-06-27 00:53:31.616839 repid-1.3.0/repid/job.py
+-rw-r--r--   0        0        0      546 2023-06-27 00:53:31.616839 repid-1.3.0/repid/logger.py
+-rw-r--r--   0        0        0     1887 2023-06-27 00:53:31.616839 repid-1.3.0/repid/main.py
+-rw-r--r--   0        0        0      257 2023-06-27 00:53:31.616839 repid-1.3.0/repid/middlewares/__init__.py
+-rw-r--r--   0        0        0      347 2023-06-27 00:53:31.616839 repid-1.3.0/repid/middlewares/consts.py
+-rw-r--r--   0        0        0     3696 2023-06-27 00:53:31.616839 repid-1.3.0/repid/middlewares/middleware.py
+-rw-r--r--   0        0        0     3647 2023-06-27 00:53:31.616839 repid-1.3.0/repid/middlewares/wrapper.py
+-rw-r--r--   0        0        0        0 2023-06-27 00:53:31.616839 repid-1.3.0/repid/py.typed
+-rw-r--r--   0        0        0     1065 2023-06-27 00:53:31.616839 repid-1.3.0/repid/queue.py
+-rw-r--r--   0        0        0     1319 2023-06-27 00:53:31.616839 repid-1.3.0/repid/retry_policy.py
+-rw-r--r--   0        0        0     5022 2023-06-27 00:53:31.616839 repid-1.3.0/repid/router.py
+-rw-r--r--   0        0        0      719 2023-06-27 00:53:31.616839 repid-1.3.0/repid/serializer.py
+-rw-r--r--   0        0        0      845 2023-06-27 00:53:31.616839 repid-1.3.0/repid/testing/__init__.py
+-rw-r--r--   0        0        0     3184 2023-06-27 00:53:31.616839 repid-1.3.0/repid/testing/modifiers.py
+-rw-r--r--   0        0        0     6099 2023-06-27 00:53:31.616839 repid-1.3.0/repid/testing/plugin.py
+-rw-r--r--   0        0        0     3971 2023-06-27 00:53:31.616839 repid-1.3.0/repid/worker.py
+-rw-r--r--   0        0        0        0 2023-06-27 00:53:31.616839 repid-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      846 2023-06-27 00:53:31.616839 repid-1.3.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-27 00:53:31.616839 repid-1.3.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     3241 2023-06-27 00:53:31.616839 repid-1.3.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     1337 2023-06-27 00:53:31.616839 repid-1.3.0/tests/integration/test_buckets.py
+-rw-r--r--   0        0        0     4335 2023-06-27 00:53:31.616839 repid-1.3.0/tests/integration/test_consumer.py
+-rw-r--r--   0        0        0     4003 2023-06-27 00:53:31.616839 repid-1.3.0/tests/integration/test_default_flow.py
+-rw-r--r--   0        0        0     1904 2023-06-27 00:53:31.616839 repid-1.3.0/tests/integration/test_no_messages_lost.py
+-rw-r--r--   0        0        0      431 2023-06-27 00:53:31.616839 repid-1.3.0/tests/test_actor.py
+-rw-r--r--   0        0        0     3110 2023-06-27 00:53:31.616839 repid-1.3.0/tests/test_config.py
+-rw-r--r--   0        0        0     2986 2023-06-27 00:53:31.616839 repid-1.3.0/tests/test_connection.py
+-rw-r--r--   0        0        0     3834 2023-06-27 00:53:31.616839 repid-1.3.0/tests/test_consumer.py
+-rw-r--r--   0        0        0     2835 2023-06-27 00:53:31.616839 repid-1.3.0/tests/test_consumer_abc.py
+-rw-r--r--   0        0        0    10234 2023-06-27 00:53:31.616839 repid-1.3.0/tests/test_default_data_models.py
+-rw-r--r--   0        0        0     3004 2023-06-27 00:53:31.616839 repid-1.3.0/tests/test_hypothesis.py
+-rw-r--r--   0        0        0     3591 2023-06-27 00:53:31.616839 repid-1.3.0/tests/test_job.py
+-rw-r--r--   0        0        0     1366 2023-06-27 00:53:31.616839 repid-1.3.0/tests/test_main.py
+-rw-r--r--   0        0        0     7842 2023-06-27 00:53:31.616839 repid-1.3.0/tests/test_middleware.py
+-rw-r--r--   0        0        0     1097 2023-06-27 00:53:31.616839 repid-1.3.0/tests/test_multiprocessing.py
+-rw-r--r--   0        0        0     7388 2023-06-27 00:53:31.616839 repid-1.3.0/tests/test_pydantic.py
+-rw-r--r--   0        0        0     3819 2023-06-27 00:53:31.616839 repid-1.3.0/tests/test_pytest_plugin.py
+-rw-r--r--   0        0        0      414 2023-06-27 00:53:31.616839 repid-1.3.0/tests/test_queue.py
+-rw-r--r--   0        0        0     3180 2023-06-27 00:53:31.616839 repid-1.3.0/tests/test_router.py
+-rw-r--r--   0        0        0      764 2023-06-27 00:53:31.616839 repid-1.3.0/tests/test_serializer.py
+-rw-r--r--   0        0        0     1895 2023-06-27 00:53:31.616839 repid-1.3.0/tests/test_utils.py
+-rw-r--r--   0        0        0     6887 2023-06-27 00:53:31.616839 repid-1.3.0/tests/test_worker.py
+-rw-r--r--   0        0        0     4057 1970-01-01 00:00:00.000000 repid-1.3.0/PKG-INFO
```

### Comparing `repid-1.2.0/LICENSE` & `repid-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/README.md` & `repid-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/pyproject.toml` & `repid-1.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -17,35 +17,39 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Typing :: Typed",
 ]
 dependencies = [
     "typing-extensions>=4.3.0,<5.0.0; python_version < \"3.10\"",
+    "packaging>=22.0",
 ]
 description = "Repid framework: simple to use, fast to run and extensible to adopt job scheduler"
 dynamic = []
 name = "repid"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "1.2.0"
+version = "1.3.0"
 
 [project.license]
 text = "MIT"
 
 [project.entry-points.pytest11]
 repid = "repid.testing.plugin"
 
 [project.optional-dependencies]
 amqp = [
     "aiormq<7.0.0,>=6.4.0",
 ]
 cron = [
     "croniter<2.0.0,>=1.3.4",
 ]
+pydantic = [
+    "pydantic>=2.0a1,<3.0.0",
+]
 redis = [
     "redis<5.0.0,>=4.3.3",
 ]
 test = [
     "pytest",
     "pytest-asyncio",
 ]
@@ -67,14 +71,17 @@
 ]
 fail_under = 100
 
 [tool.coverage.run]
 omit = [
     "repid/connections/rabbitmq/protocols.py",
 ]
+source = [
+    "repid",
+]
 
 [tool.mypy]
 check_untyped_defs = true
 disallow_any_unimported = true
 disallow_untyped_defs = true
 exclude = [
     "benchmarks",
@@ -125,37 +132,36 @@
 tests = [
     "pytest",
     "pytest-asyncio",
     "pytest-pretty",
     "pytest-clarity",
     "pytest-lazy-fixture",
     "pytest-docker-tools",
-    "pytest-cov",
+    "pytest-timeout>=2.1.0",
+    "coverage[toml]>=7.2.7",
     "hypothesis",
-    "pydantic<2.0.0,>=1.10.0",
 ]
 
+[tool.pdm.scripts]
+erase-coverage = "coverage erase"
+only-test = "coverage run -m pytest --diff-symbols --hypothesis-verbosity=normal tests/"
+report-coverage = "coverage report --no-skip-covered --show-missing"
+xml-coverage = "coverage xml --fail-under=0"
+
 [tool.pdm.scripts.test]
-cmd = [
-    "pytest",
-    "--diff-symbols",
-    "--hypothesis-verbosity=normal",
-    "--cov-report=xml",
-    "--cov-report=term-missing",
-    "--cov=repid",
-    "--cov-append",
+composite = [
+    "erase-coverage",
+    "only-test",
+    "xml-coverage",
+    "report-coverage",
 ]
 
-[tool.pdm.scripts.test.env]
-COV_CORE_SOURCE = "repid"
-COV_CORE_CONFIG = ".coveragerc"
-COV_CORE_DATAFILE = ".coverage.eager"
-
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
+timeout = 150
 
 [tool.ruff]
 ignore = [
     "E501",
     "N999",
     "PLR0913",
 ]
```

### Comparing `repid-1.2.0/repid/_asyncify.py` & `repid-1.3.0/repid/_asyncify.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/_processor.py` & `repid-1.3.0/repid/_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import asyncio
 import time
 from datetime import datetime
 from typing import TYPE_CHECKING, Any
 
+from repid._utils import _ArgsBucketInMessageId
 from repid.actor import ActorData, ActorResult
 from repid.logger import logger
 from repid.middlewares import middleware_wrapper
-from repid.utils import _ArgsBucketInMessageId
 
 if TYPE_CHECKING:
     from repid.connection import Connection
     from repid.data import ParametersT, RoutingKeyT
     from repid.data.protocols import ResultPropertiesT
 
 
@@ -35,16 +35,15 @@
 
     @staticmethod
     @middleware_wrapper
     async def actor_run(
         actor: ActorData,
         key: RoutingKeyT,
         parameters: ParametersT,
-        args: list,
-        kwargs: dict,
+        payload: str,
     ) -> ActorResult:
         time_limit = parameters.execution_timeout.total_seconds()
 
         logger_extra = {
             "actor_name": actor.name,
             "message_id": key.id_,
             "time_limit": time_limit,
@@ -56,15 +55,17 @@
 
         logger.info("Running actor '{actor_name}' on message {message_id}.", extra=logger_extra)
         logger.debug("Time limit is set to {time_limit}.", extra=logger_extra)
 
         started_when = time.perf_counter_ns()
 
         try:
-            result = await asyncio.wait_for(actor.fn(*args, **kwargs), timeout=time_limit)
+            args, kwargs = actor.converter.convert_inputs(payload)
+            _result = await asyncio.wait_for(actor.fn(*args, **kwargs), timeout=time_limit)
+            result = actor.converter.convert_outputs(_result)
         except Exception as exc:  # noqa: BLE001
             exception = exc
             success = False
             logger.exception(
                 "Error inside of an actor '{actor_name}' on message {message_id}.",
                 extra=logger_extra,
             )
@@ -111,23 +112,22 @@
         # nack
         else:
             await self._conn.message_broker.nack(key)
 
     async def set_result_bucket(
         self,
         result_params: ResultPropertiesT | None,
-        returns: str,
         result_actor: ActorResult,
     ) -> None:
         if result_params is None:
             return
         await self._conn._rb.store_bucket(
             result_params.id_,
             self._conn._rb.BUCKET_CLASS(  # type: ignore[call-arg]
-                data=returns,
+                data=result_actor.data,
                 started_when=result_actor.started_when,
                 finished_when=result_actor.finished_when,
                 success=result_actor.success,
                 exception=str(result_actor.exception)
                 if result_actor.exception is not None
                 else None,
                 timestamp=datetime.now(),
@@ -139,17 +139,15 @@
         self,
         actor: ActorData,
         key: RoutingKeyT,
         payload: str,
         parameters: ParametersT,
     ) -> None:
         raw_payload = await self.get_payload(payload)
-        args, kwargs = actor.converter.convert_inputs(raw_payload)
-        result = await self.actor_run(actor, key, parameters, args, kwargs)
+        result = await self.actor_run(actor, key, parameters, raw_payload)
         await self.report_to_broker(actor, key, payload, parameters, result)
         self._processed += 1
-        returns = actor.converter.convert_outputs(result.data)
-        await self.set_result_bucket(parameters.result, returns, result)
+        await self.set_result_bucket(parameters.result, result)
 
     @property
     def processed(self) -> int:
         return self._processed  # pragma: no cover
```

### Comparing `repid-1.2.0/repid/_runner.py` & `repid-1.3.0/repid/_runner.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/config.py` & `repid-1.3.0/repid/config.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/connection.py` & `repid-1.3.0/repid/connection.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/connections/__init__.py` & `repid-1.3.0/repid/connections/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+from repid._utils import is_installed
 from repid.connections.abc import BucketBrokerT, ConsumerT, MessageBrokerT
 from repid.connections.in_memory import (
     DummyBucketBroker,
     DummyMessageBroker,
     InMemoryBucketBroker,
     InMemoryMessageBroker,
 )
-from repid.utils import is_installed
 
 __all__ = [
     "BucketBrokerT",
     "ConsumerT",
     "MessageBrokerT",
     "DummyBucketBroker",
     "DummyMessageBroker",
```

### Comparing `repid-1.2.0/repid/connections/abc.py` & `repid-1.3.0/repid/connections/abc.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/connections/in_memory/bucket_broker.py` & `repid-1.3.0/repid/connections/in_memory/bucket_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/connections/in_memory/consumer.py` & `repid-1.3.0/repid/connections/in_memory/consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         while True:
             await self.__update_delayed()
             with suppress(asyncio.TimeoutError):
                 msg = await asyncio.wait_for(self._queue.simple.get(), timeout=1.0)
                 if msg.parameters.is_overdue:
                     self._queue.dead.append(msg)
                 elif self.topics and msg.key.topic not in self.topics:
-                    await self._queue.simple.put(msg)
+                    self._queue.simple.put_nowait(msg)
                 else:
                     break
             await asyncio.sleep(0.001)
         self._queue.processing.add(msg)
 
         await asyncio.sleep(0)
         return (msg.key, msg.payload, msg.parameters)
```

### Comparing `repid-1.2.0/repid/connections/in_memory/message_broker.py` & `repid-1.3.0/repid/connections/in_memory/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/connections/in_memory/utils.py` & `repid-1.3.0/repid/connections/in_memory/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/connections/rabbitmq/consumer.py` & `repid-1.3.0/repid/connections/rabbitmq/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/connections/rabbitmq/message_broker.py` & `repid-1.3.0/repid/connections/rabbitmq/message_broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import asyncio
 from datetime import datetime
 from typing import TYPE_CHECKING
 
 import aiormq
 from aiormq.abc import Basic
 
+from repid._utils import JSON_ENCODER
 from repid.connections.abc import MessageBrokerT
 from repid.connections.rabbitmq.consumer import _RabbitConsumer
 from repid.connections.rabbitmq.utils import (
     MessageContent,
     durable_message_decider,
     qnc,
     wait_until,
 )
 from repid.logger import logger
-from repid.utils import JSON_ENCODER
 
 if TYPE_CHECKING:
     from repid.connections.rabbitmq.protocols import (
         DurableMessageDeciderT,
         QueueNameConstructorT,
     )
     from repid.data.protocols import ParametersT, RoutingKeyT
```

### Comparing `repid-1.2.0/repid/connections/rabbitmq/utils.py` & `repid-1.3.0/repid/connections/rabbitmq/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/connections/redis/bucket_broker.py` & `repid-1.3.0/repid/connections/redis/bucket_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/connections/redis/consumer.py` & `repid-1.3.0/repid/connections/redis/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/connections/redis/message_broker.py` & `repid-1.3.0/repid/connections/redis/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/connections/redis/utils.py` & `repid-1.3.0/repid/connections/redis/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/data/_buckets.py` & `repid-1.3.0/repid/data/_buckets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from dataclasses import asdict, dataclass, field
 from datetime import datetime, timedelta
 from typing import Any, Dict, Union
 
-from repid.utils import FROZEN_DATACLASS, JSON_ENCODER, SLOTS_DATACLASS
+from repid._utils import FROZEN_DATACLASS, JSON_ENCODER, SLOTS_DATACLASS
 
 
 @dataclass(**FROZEN_DATACLASS, **SLOTS_DATACLASS)
 class ArgsBucket:
     data: str
 
     timestamp: datetime = field(default_factory=datetime.now)
```

### Comparing `repid-1.2.0/repid/data/_key.py` & `repid-1.3.0/repid/data/_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass, field
 from uuid import uuid4
 
+from repid._utils import FROZEN_DATACLASS, SLOTS_DATACLASS, VALID_ID, VALID_NAME
 from repid.data.priorities import PrioritiesT
-from repid.utils import FROZEN_DATACLASS, SLOTS_DATACLASS, VALID_ID, VALID_NAME
 
 
 @dataclass(**FROZEN_DATACLASS, **SLOTS_DATACLASS)
 class RoutingKey:
     topic: str
     queue: str = "default"
     priority: int = PrioritiesT.MEDIUM.value
```

### Comparing `repid-1.2.0/repid/data/_parameters.py` & `repid-1.3.0/repid/data/_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from copy import deepcopy
 from dataclasses import asdict, dataclass, field
 from datetime import datetime, timedelta
 from typing import TYPE_CHECKING, Any, ClassVar, Dict, Type, Union
 from uuid import uuid4
 
-from repid.utils import FROZEN_DATACLASS, JSON_ENCODER, SLOTS_DATACLASS, is_installed
+from repid._utils import FROZEN_DATACLASS, JSON_ENCODER, SLOTS_DATACLASS, is_installed
 
 if TYPE_CHECKING:
     from repid.data.protocols import (
         DelayPropertiesT,
         ResultPropertiesT,
         RetriesPropertiesT,
     )
```

### Comparing `repid-1.2.0/repid/data/protocols.py` & `repid-1.3.0/repid/data/protocols.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/job.py` & `repid-1.3.0/repid/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import uuid
 from datetime import datetime, timedelta
 from typing import TYPE_CHECKING, Any
 
+from repid._utils import VALID_ID, VALID_NAME, _ArgsBucketInMessageId
 from repid.config import Config
 from repid.data import ParametersT, PrioritiesT, ResultBucketT, RoutingKeyT
 from repid.main import Repid
 from repid.queue import Queue
-from repid.utils import VALID_ID, VALID_NAME, _ArgsBucketInMessageId
 
 if TYPE_CHECKING:
     from repid.connection import Connection
 
 
 class Job:
     __slots__ = (
```

### Comparing `repid-1.2.0/repid/logger.py` & `repid-1.3.0/repid/logger.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/main.py` & `repid-1.3.0/repid/main.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/middlewares/middleware.py` & `repid-1.3.0/repid/middlewares/middleware.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/middlewares/wrapper.py` & `repid-1.3.0/repid/middlewares/wrapper.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/queue.py` & `repid-1.3.0/repid/queue.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
+from repid._utils import VALID_NAME
 from repid.main import Repid
-from repid.utils import VALID_NAME
 
 if TYPE_CHECKING:
     from repid.connection import Connection
 
 
 class Queue:
     __slots__ = ("name", "_conn")
```

### Comparing `repid-1.2.0/repid/retry_policy.py` & `repid-1.3.0/repid/retry_policy.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/router.py` & `repid-1.3.0/repid/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from collections import defaultdict
 from dataclasses import dataclass, field
 from functools import partial
 from typing import TYPE_CHECKING, Callable, TypeVar, overload
 
 from repid._asyncify import asyncify
+from repid._utils import VALID_NAME
 from repid.actor import ActorData
 from repid.config import Config
 from repid.retry_policy import default_retry_policy_factory
-from repid.utils import VALID_NAME
 
 if TYPE_CHECKING:
     from repid.converter import ConverterT
     from repid.retry_policy import RetryPolicyT
 
 YourFunc = TypeVar("YourFunc", bound=Callable)
```

### Comparing `repid-1.2.0/repid/testing/__init__.py` & `repid-1.3.0/repid/testing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from repid.utils import is_installed
+from repid._utils import is_installed
 
 __all__ = []
 
 if is_installed("pytest") and is_installed("pytest_asyncio"):
     from repid.testing.modifiers import EventLog
     from repid.testing.plugin import (
         GetEventLogT,
```

### Comparing `repid-1.2.0/repid/testing/modifiers.py` & `repid-1.3.0/repid/testing/modifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from functools import wraps
 from time import perf_counter, time
 from typing import TYPE_CHECKING, Any, Callable
 
+from repid._utils import FROZEN_DATACLASS, SLOTS_DATACLASS
 from repid.connections.abc import BucketBrokerT, ConsumerT, MessageBrokerT
-from repid.utils import FROZEN_DATACLASS, SLOTS_DATACLASS
 from repid.worker import Worker
 
 if TYPE_CHECKING:
     from repid.data.protocols import RoutingKeyT
 
 
 @dataclass(**SLOTS_DATACLASS, **FROZEN_DATACLASS)
```

### Comparing `repid-1.2.0/repid/testing/plugin.py` & `repid-1.3.0/repid/testing/plugin.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/repid/worker.py` & `repid-1.3.0/repid/worker.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/tests/integration/conftest.py` & `repid-1.3.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/tests/integration/test_buckets.py` & `repid-1.3.0/tests/integration/test_buckets.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/tests/integration/test_consumer.py` & `repid-1.3.0/tests/integration/test_consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,29 +26,29 @@
             await asyncio.gather(*[j.enqueue() for _ in range(amount_of_jobs)])
 
         yield conn
 
         await j.queue.delete()
 
 
-@pytest.mark.parametrize("seed_conn", [15], indirect=True)
+@pytest.mark.parametrize("seed_conn", [30], indirect=True)
 async def test_more_concurrent_tasks_than_limit() -> None:
-    w = Worker(messages_limit=15, tasks_limit=10)
+    w = Worker(messages_limit=30, tasks_limit=10)
 
     hit = 0
 
     @w.actor
     async def awesome_job() -> None:
         nonlocal hit
         await asyncio.sleep(1.0)
         hit += 1
 
     await asyncio.wait_for(w.run(), timeout=5.0)
 
-    assert hit == 15
+    assert hit == 30
 
 
 async def test_reject_on_sigint(seed_conn: Connection) -> None:
     hit = False
     never_hit = False
 
     w = Worker(graceful_shutdown_time=1)
```

### Comparing `repid-1.2.0/tests/integration/test_default_flow.py` & `repid-1.3.0/tests/integration/test_default_flow.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/tests/integration/test_no_messages_lost.py` & `repid-1.3.0/tests/integration/test_no_messages_lost.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/tests/test_config.py` & `repid-1.3.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/tests/test_connection.py` & `repid-1.3.0/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/tests/test_consumer.py` & `repid-1.3.0/tests/test_consumer.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,57 +44,58 @@
     assert hit == 15
 
 
 @pytest.mark.parametrize("seed_conn", [15], indirect=True)
 async def test_rejected_after_timeout(seed_conn: Connection) -> None:
     consumer = seed_conn.message_broker.get_consumer("default", ["awesome_job"])
     async with consumer:
-        await asyncio.sleep(1.0)
+        await asyncio.sleep(0)
 
     with pytest.raises(RuntimeError):
         # can't consume finished consumer
         await consumer.consume()
 
 
 @pytest.mark.parametrize("seed_conn", [15], indirect=True)
 async def test_paused_consumer(seed_conn: Connection) -> None:
     consumer = seed_conn.message_broker.get_consumer("default", ["awesome_job"])
     await consumer.pause()
     async with consumer:
         with pytest.raises(asyncio.TimeoutError):
             # there should be nothing to consume, since the consumer has been paused
-            await asyncio.wait_for(consumer.consume(), 1.0)
+            await asyncio.wait_for(consumer.consume(), 0.2)
 
 
 async def test_finishing_consumer_without_start(seed_conn: Connection) -> None:
     consumer = seed_conn.message_broker.get_consumer("default", ["awesome_job"])
     await consumer.finish()
 
 
 async def test_another_topic_is_not_consumed(seed_conn: Connection) -> None:
     consumer = seed_conn.message_broker.get_consumer("default", ["another_topic"])
-    async with consumer:
-        with pytest.raises(asyncio.TimeoutError):
-            # there should be nothing to consume, since the consumer is interested in another topic
-            await asyncio.wait_for(consumer.consume(), 1.0)
+    await consumer.start()
+    with pytest.raises(asyncio.TimeoutError):
+        # there should be nothing to consume, since the consumer is interested in another topic
+        await asyncio.wait_for(consumer.consume(), 0.2)
+    await consumer.finish()
 
 
 async def test_consume_without_ack(seed_conn: Connection) -> None:
     consumer = seed_conn.message_broker.get_consumer("default", ["awesome_job"])
     async with consumer:
-        key, _, _ = await asyncio.wait_for(consumer.consume(), 1.0)
+        key, _, _ = await asyncio.wait_for(consumer.consume(), 0.1)
         assert key.topic == "awesome_job"
 
     async with consumer:
-        key, _, _ = await asyncio.wait_for(consumer.consume(), 1.0)
+        key, _, _ = await asyncio.wait_for(consumer.consume(), 0.1)
         assert key.topic == "awesome_job"
         await seed_conn.message_broker.ack(key)
 
         with pytest.raises(asyncio.TimeoutError):
-            await asyncio.wait_for(consumer.consume(), 1.0)
+            await asyncio.wait_for(consumer.consume(), 0.2)
 
 
 @pytest.mark.parametrize("seed_conn", [0], indirect=True)
 async def test_ttl(seed_conn: Connection) -> None:
     j = Job("awesome_job", ttl=timedelta(seconds=4))
     await asyncio.gather(*[j.enqueue() for _ in range(2)])
```

### Comparing `repid-1.2.0/tests/test_consumer_abc.py` & `repid-1.3.0/tests/test_consumer_abc.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/tests/test_default_data_models.py` & `repid-1.3.0/tests/test_default_data_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
 from datetime import datetime, timedelta
 from uuid import UUID
 
 import pytest
 
+from repid._utils import JSON_ENCODER
 from repid.data import BucketT, ResultBucketT
 from repid.data._buckets import ArgsBucket, ResultBucket
 from repid.data._key import RoutingKey
 from repid.data._parameters import (
     DelayProperties,
     Parameters,
     ResultProperties,
     RetriesProperties,
 )
 from repid.data.priorities import PrioritiesT
-from repid.utils import JSON_ENCODER
 
 
 def test_routing_key() -> None:
     # Test valid values
     routing_key = RoutingKey(
         topic="test_topic",
         queue="test_queue",
```

### Comparing `repid-1.2.0/tests/test_hypothesis.py` & `repid-1.3.0/tests/test_hypothesis.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     recursive,
     sampled_from,
     text,
     timedeltas,
 )
 
 from repid import Job, PrioritiesT, Queue, default_retry_policy_factory
-from repid.utils import VALID_ID, VALID_NAME
+from repid._utils import VALID_ID, VALID_NAME
 
 MAX = 2**31 - 1
 MIN = -(2**31)
 
 json_st = recursive(
     none() | booleans() | floats() | text(printable),
     lambda children: lists(children) | dictionaries(text(printable), children),
```

### Comparing `repid-1.2.0/tests/test_job.py` & `repid-1.3.0/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/tests/test_main.py` & `repid-1.3.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/tests/test_middleware.py` & `repid-1.3.0/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/tests/test_multiprocessing.py` & `repid-1.3.0/tests/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/tests/test_pytest_plugin.py` & `repid-1.3.0/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/tests/test_router.py` & `repid-1.3.0/tests/test_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from collections import defaultdict
 
 import pytest
 
 from repid.actor import ActorData
-from repid.converter import DefaultConverter
+from repid.converter import BasicConverter
 from repid.retry_policy import RetryPolicyT, default_retry_policy_factory
 from repid.router import Router, RouterDefaults
 
 
 def test_empty_router() -> None:
     router = Router()
     assert router.actors == {}
@@ -29,15 +29,15 @@
 
     fn = lambda x: x  # noqa: E731
     actor1 = ActorData(
         fn=fn,
         name="actor1",
         queue="queue1",
         retry_policy=default_retry_policy_factory(),
-        converter=DefaultConverter(fn),
+        converter=BasicConverter(fn),
     )
     other_router.actors = {"actor1": actor1}
     temp = defaultdict(set)
     temp["queue1"].add("actor1")
     other_router.topics_by_queue = temp
 
     router.include_router(other_router)
@@ -69,23 +69,23 @@
     assert router.topics == frozenset({"actor1_renamed"})
 
 
 @pytest.mark.parametrize(
     ("queue", "retry_policy", "converter"),
     [
         (None, None, None),
-        ("actor1_queue", default_retry_policy_factory(), DefaultConverter),
-        (None, default_retry_policy_factory(), DefaultConverter),
-        (None, None, DefaultConverter),
+        ("actor1_queue", default_retry_policy_factory(), BasicConverter),
+        (None, default_retry_policy_factory(), BasicConverter),
+        (None, None, BasicConverter),
     ],
 )
 def test_router_decorator_registers_actor_with_defaults(
     queue: str | None,
     retry_policy: RetryPolicyT | None,
-    converter: type[DefaultConverter] | None,
+    converter: type[BasicConverter] | None,
 ) -> None:
     router = Router()
     defaults = RouterDefaults(queue="default_queue")
     router.defaults = defaults
 
     @router.actor(queue=queue, retry_policy=retry_policy, converter=converter)
     def actor1() -> None:
@@ -95,15 +95,15 @@
         assert router.actors["actor1"].queue == "default_queue"
     else:
         assert router.actors["actor1"].queue == queue
 
     if retry_policy is not None:
         assert router.actors["actor1"].retry_policy is retry_policy
 
-    assert isinstance(router.actors["actor1"].converter, DefaultConverter)
+    assert isinstance(router.actors["actor1"].converter, BasicConverter)
 
 
 def test_router_decorator_uses_default_retry_policy() -> None:
     expected_retry_policy = default_retry_policy_factory(min_backoff=1)
     defaults = RouterDefaults(retry_policy=expected_retry_policy)
 
     router = Router(defaults=defaults)
```

### Comparing `repid-1.2.0/tests/test_serializer.py` & `repid-1.3.0/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/tests/test_worker.py` & `repid-1.3.0/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `repid-1.2.0/PKG-INFO` & `repid-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repid
-Version: 1.2.0
+Version: 1.3.0
 Summary: Repid framework: simple to use, fast to run and extensible to adopt job scheduler
 Author-Email: aleksul <me@aleksul.space>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -15,21 +15,24 @@
 Classifier: Typing :: Typed
 Project-URL: Documentation, https://repid.aleksul.space
 Project-URL: Funding, https://github.com/sponsors/aleksul
 Project-URL: Repository, https://github.com/aleksul/repid
 Project-URL: Tracker, https://github.com/aleksul/repid/issues
 Requires-Python: >=3.8
 Requires-Dist: typing-extensions<5.0.0,>=4.3.0; python_version < "3.10"
+Requires-Dist: packaging>=22.0
 Requires-Dist: aiormq<7.0.0,>=6.4.0; extra == "amqp"
 Requires-Dist: croniter<2.0.0,>=1.3.4; extra == "cron"
+Requires-Dist: pydantic<3.0.0,>=2.0a1; extra == "pydantic"
 Requires-Dist: redis<5.0.0,>=4.3.3; extra == "redis"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Provides-Extra: amqp
 Provides-Extra: cron
+Provides-Extra: pydantic
 Provides-Extra: redis
 Provides-Extra: test
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-configure-file { "MD013": { "line_length": 100 } } -->
 <!-- markdownlint-disable MD033 -->
```

#### html2text {}

```diff
@@ -1,28 +1,30 @@
-Metadata-Version: 2.1 Name: repid Version: 1.2.0 Summary: Repid framework:
+Metadata-Version: 2.1 Name: repid Version: 1.3.0 Summary: Repid framework:
 simple to use, fast to run and extensible to adopt job scheduler Author-Email:
 aleksul
 aleksul.space> License: MIT Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
 CPython Classifier: Typing :: Typed Project-URL: Documentation, https://
 repid.aleksul.space Project-URL: Funding, https://github.com/sponsors/aleksul
 Project-URL: Repository, https://github.com/aleksul/repid Project-URL: Tracker,
 https://github.com/aleksul/repid/issues Requires-Python: >=3.8 Requires-Dist:
 typing-extensions<5.0.0,>=4.3.0; python_version < "3.10" Requires-Dist:
-aiormq<7.0.0,>=6.4.0; extra == "amqp" Requires-Dist: croniter<2.0.0,>=1.3.4;
-extra == "cron" Requires-Dist: redis<5.0.0,>=4.3.3; extra == "redis" Requires-
-Dist: pytest; extra == "test" Requires-Dist: pytest-asyncio; extra == "test"
-Provides-Extra: amqp Provides-Extra: cron Provides-Extra: redis Provides-Extra:
-test Description-Content-Type: text/markdown   # repid [Repid's_logo] [![PyPI
-version](https://img.shields.io/pypi/v/repid.svg)](https://pypi.org/project/
-repid/) [![codecov](https://codecov.io/gh/aleksul/repid/branch/main/graph/
+packaging>=22.0 Requires-Dist: aiormq<7.0.0,>=6.4.0; extra == "amqp" Requires-
+Dist: croniter<2.0.0,>=1.3.4; extra == "cron" Requires-Dist:
+pydantic<3.0.0,>=2.0a1; extra == "pydantic" Requires-Dist: redis<5.0.0,>=4.3.3;
+extra == "redis" Requires-Dist: pytest; extra == "test" Requires-Dist: pytest-
+asyncio; extra == "test" Provides-Extra: amqp Provides-Extra: cron Provides-
+Extra: pydantic Provides-Extra: redis Provides-Extra: test Description-Content-
+Type: text/markdown   # repid [Repid's_logo] [![PyPI version](https://
+img.shields.io/pypi/v/repid.svg)](https://pypi.org/project/repid/) [![codecov]
+(https://codecov.io/gh/aleksul/repid/branch/main/graph/
 badge.svg?token=IP3Z1VXB1G)](https://codecov.io/gh/aleksul/repid) [![Tests]
 (https://github.com/aleksul/repid/actions/workflows/tests.yaml/badge.svg)]
 (https://github.com/aleksul/repid/actions/workflows/tests.yaml) [![PyPI
 pyversions](https://img.shields.io/pypi/pyversions/repid.svg)](https://
 pypi.python.org/pypi/repid/) [![Code style: black](https://img.shields.io/
 badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Read
 documentation](https://img.shields.io/badge/read-documentation-
```

