# Comparing `tmp/propan-0.1.4.0.tar.gz` & `tmp/propan-0.1.4.1.tar.gz`

## Comparing `propan-0.1.4.0.tar` & `propan-0.1.4.1.tar`

### file list

```diff
@@ -1,185 +1,185 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.4.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.4.0/SECURITY.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.4.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.4.0/.github/dependantbot.yml
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.4.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.4.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.4.0/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.4.0/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 propan-0.1.4.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/kafka/1_direct.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/nats/1_basic.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/redis/pattern.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/scheduling/rocketry.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/serialization/gen_py_code.sh
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/serialization/message.proto
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/serialization/protobuf.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/serialization/requirements.txt
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/sqs/1_basic.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/__about__.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/__main__.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/_compat.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/py.typed
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/types.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/__init__.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/channels.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/info.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/main.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/message.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/security.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/servers.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/subscription.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/utils.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/bindings/__init__.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/bindings/amqp.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/bindings/kafka.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/bindings/main.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/bindings/nats.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/bindings/redis.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/bindings/sqs.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/exceptions.py
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/_model/__init__.py
--rw-r--r--   0        0        0    12879 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/_model/broker_usecase.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/_model/routing.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/_model/schemas.py
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/_model/utils.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0    12851 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/kafka/routing.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/kafka/routing.pyi
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/nats/routing.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/nats/routing.pyi
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    14261 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/rabbit/routing.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/rabbit/routing.pyi
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     9193 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/redis/routing.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/redis/routing.pyi
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/sqs/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/sqs/routing.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/sqs/routing.pyi
--rw-r--r--   0        0        0     9544 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/sqs/schema.py
--rw-r--r--   0        0        0    12833 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/sqs/sqs_broker.py
--rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/sqs/sqs_broker.pyi
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/__init__.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/app.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/main.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/docs/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/docs/app.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/docs/gen.py
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/docs/serving.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/async_app/sqs.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     7591 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/sqs/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/sqs/router.py
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/sqs/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/log/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/log/formatter.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/log/logging.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/test/kafka.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/test/nats.py
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/test/rabbit.py
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/test/redis.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/test/sqs.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/test/utils.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/utils/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/utils/classes.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/utils/functions.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/utils/no_cast.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/utils/context/main.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.4.0/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.4.0/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.4.0/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       58 2020-02-02 00:00:00.000000 propan-0.1.4.0/scripts/test.sh
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.4.0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.4.0/LICENSE
--rw-r--r--   0        0        0    13471 2020-02-02 00:00:00.000000 propan-0.1.4.0/README.md
--rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 propan-0.1.4.0/pyproject.toml
--rw-r--r--   0        0        0    17710 2020-02-02 00:00:00.000000 propan-0.1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.4.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.4.1/SECURITY.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.4.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.4.1/.github/dependantbot.yml
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.4.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.4.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.4.1/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.4.1/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.4.1/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 propan-0.1.4.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/redis/pattern.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/scheduling/rocketry.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/serialization/gen_py_code.sh
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/serialization/message.proto
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/serialization/protobuf.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/serialization/requirements.txt
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.4.1/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/__about__.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/__main__.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/_compat.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/py.typed
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/types.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/asyncapi/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/asyncapi/channels.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/asyncapi/info.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/asyncapi/main.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/asyncapi/message.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/asyncapi/security.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/asyncapi/servers.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/asyncapi/subscription.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/asyncapi/utils.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/asyncapi/bindings/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/asyncapi/bindings/amqp.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/asyncapi/bindings/kafka.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/asyncapi/bindings/main.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/asyncapi/bindings/nats.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/asyncapi/bindings/redis.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/asyncapi/bindings/sqs.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/exceptions.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0    13237 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/_model/routing.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0    13099 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     8419 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/kafka/routing.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/kafka/routing.pyi
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     8447 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/nats/routing.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/nats/routing.pyi
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    14769 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0    11026 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/rabbit/routing.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/rabbit/routing.pyi
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     9657 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/redis/routing.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/redis/routing.pyi
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/sqs/routing.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/sqs/routing.pyi
+-rw-r--r--   0        0        0     9544 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    13079 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/app.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/main.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/docs/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/docs/app.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/docs/gen.py
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/docs/serving.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     7591 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/log/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/log/formatter.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/log/logging.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/test/kafka.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/test/nats.py
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/test/redis.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/test/sqs.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/test/utils.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/utils/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/utils/classes.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/utils/functions.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/utils/no_cast.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/utils/context/main.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 propan-0.1.4.1/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.4.1/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.4.1/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.4.1/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       58 2020-02-02 00:00:00.000000 propan-0.1.4.1/scripts/test.sh
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.4.1/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.4.1/LICENSE
+-rw-r--r--   0        0        0    13633 2020-02-02 00:00:00.000000 propan-0.1.4.1/README.md
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 propan-0.1.4.1/pyproject.toml
+-rw-r--r--   0        0        0    17872 2020-02-02 00:00:00.000000 propan-0.1.4.1/PKG-INFO
```

### Comparing `propan-0.1.4.0/CONTRIBUTING.md` & `propan-0.1.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/SECURITY.md` & `propan-0.1.4.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/.github/PULL_REQUEST_TEMPLATE.md` & `propan-0.1.4.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/.github/ISSUE_TEMPLATE/bug_report.md` & `propan-0.1.4.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/.github/ISSUE_TEMPLATE/config.yml` & `propan-0.1.4.1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/.github/workflows/documentation.yml` & `propan-0.1.4.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/.github/workflows/publish_coverage.yml` & `propan-0.1.4.1/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/.github/workflows/publish_pypi.yml` & `propan-0.1.4.1/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/.github/workflows/tests.yml` & `propan-0.1.4.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/3_lifespan_events.py` & `propan-0.1.4.1/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/4_cli_attributes_promotion.py` & `propan-0.1.4.1/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/5_publishing.py` & `propan-0.1.4.1/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/6_arguments_casting.py` & `propan-0.1.4.1/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/7_handler_errors_processing.py` & `propan-0.1.4.1/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/dependencies/1_dependency_injection.py` & `propan-0.1.4.1/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.4.1/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.4.1/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.4.1/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.4.1/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/dependencies/7_annotated.py` & `propan-0.1.4.1/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.4.1/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.4.1/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.4.1/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.4.1/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/http_frameworks_integrations/quart.py` & `propan-0.1.4.1/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.4.1/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.4.1/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/rabbit/direct.py` & `propan-0.1.4.1/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/rabbit/fanout.py` & `propan-0.1.4.1/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/rabbit/header.py` & `propan-0.1.4.1/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/rabbit/topic.py` & `propan-0.1.4.1/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/redis/direct.py` & `propan-0.1.4.1/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/redis/pattern.py` & `propan-0.1.4.1/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/examples/serialization/protobuf.py` & `propan-0.1.4.1/examples/serialization/protobuf.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/__about__.py` & `propan-0.1.4.1/propan/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Simple and fast framework to create message brokers based microservices"""
 
 from unittest.mock import Mock
 
-__version__ = "0.1.4.0"
+__version__ = "0.1.4.1"
 
 
 INSTALL_MESSAGE = (
     "You should specify using broker!\n"
     "Install it using one of the following commands:\n"
     'pip install "propan[async-rabbit]"\n'
     'pip install "propan[async-nats]"\n'
```

### Comparing `propan-0.1.4.0/propan/__init__.py` & `propan-0.1.4.1/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/_compat.py` & `propan-0.1.4.1/propan/_compat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,26 @@
+import importlib.util
 import json
 import sys
 from typing import Any, Dict, List, Type
 
 from fast_depends._compat import PYDANTIC_V2, FieldInfo
 from fastapi import __version__ as FASTAPI_VERSION
 from pydantic import BaseModel
 from typing_extensions import Never
 
 from propan.types import AnyDict
 
 FASTAPI_V2 = FASTAPI_VERSION.startswith("0.10")
 
+
+def is_installed(package: str) -> bool:
+    return importlib.util.find_spec(package)
+
+
 if FASTAPI_V2:
     from fastapi._compat import _normalize_errors
     from fastapi.exceptions import ResponseValidationError
 
     def raise_fastapi_validation_error(errors: List[Any], body: AnyDict) -> Never:
         raise ResponseValidationError(_normalize_errors(errors), body=body)
 
@@ -67,15 +73,16 @@
 
 else:
     from pydantic.config import BaseConfig
     from pydantic.config import ConfigDict as CD
     from pydantic.config import get_config
     from pydantic.json import pydantic_encoder
 
-    def ConfigDict(**kwargs: Dict[str, Any]) -> Type[BaseConfig]:  # type: ignore[no-redef]
+    # type: ignore[no-redef]
+    def ConfigDict(**kwargs: Dict[str, Any]) -> Type[BaseConfig]:
         return get_config(CD(**kwargs))  # type: ignore
 
     SCHEMA_FIELD = "schema_extra"
 
     def dump_json(data: Any) -> str:
         return json.dumps(data, default=pydantic_encoder)
```

### Comparing `propan-0.1.4.0/propan/annotations.py` & `propan-0.1.4.1/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/types.py` & `propan-0.1.4.1/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/asyncapi/__init__.py` & `propan-0.1.4.1/propan/asyncapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/asyncapi/channels.py` & `propan-0.1.4.1/propan/asyncapi/channels.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/asyncapi/info.py` & `propan-0.1.4.1/propan/asyncapi/bindings/redis.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,23 @@
-import importlib.util
 from typing import Optional
 
-from pydantic import BaseModel, Field, HttpUrl
+from pydantic import BaseModel, Field
+from typing_extensions import Literal
 
-if importlib.util.find_spec("email_validator"):
-    from pydantic import EmailStr
-else:  # pragma: no cover
-    EmailStr = str  # type: ignore
+from propan.types import AnyDict
 
 
-class AsyncAPIContact(BaseModel):
-    name: str
-    url: HttpUrl
-    email: Optional[EmailStr] = None
-
-
-class AsyncAPILicense(BaseModel):
-    name: str
-    url: HttpUrl
+class AsyncAPIRedisChannelBinding(BaseModel):
+    channel: str
+    method: Literal["ssubscribe", "psubscribe", "subscribe"] = "subscribe"
+    version: str = Field(
+        default="custom",
+        alias="bindingVersion",
+    )
 
 
-class AsyncAPIInfo(BaseModel):
-    title: str
-    version: str = "1.0.0"
-    description: str = ""
-    terms: Optional[HttpUrl] = Field(
-        default=None,
-        alias="termsOfService",
+class AsyncAPIRedisOperationBinding(BaseModel):
+    reply_to: Optional[AnyDict] = Field(default=None, alias="replyTo")
+    version: str = Field(
+        default="custom",
+        alias="bindingVersion",
     )
-    contact: Optional[AsyncAPIContact] = None
-    license: Optional[AsyncAPILicense] = None
```

### Comparing `propan-0.1.4.0/propan/asyncapi/main.py` & `propan-0.1.4.1/propan/asyncapi/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/asyncapi/message.py` & `propan-0.1.4.1/propan/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/asyncapi/security.py` & `propan-0.1.4.1/propan/asyncapi/security.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/asyncapi/subscription.py` & `propan-0.1.4.1/propan/asyncapi/subscription.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/asyncapi/bindings/amqp.py` & `propan-0.1.4.1/propan/asyncapi/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/asyncapi/bindings/kafka.py` & `propan-0.1.4.1/propan/asyncapi/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/asyncapi/bindings/main.py` & `propan-0.1.4.1/propan/asyncapi/bindings/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/brokers/push_back_watcher.py` & `propan-0.1.4.1/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/brokers/_model/broker_usecase.py` & `propan-0.1.4.1/propan/brokers/_model/broker_usecase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import json
 import logging
 import warnings
 from abc import ABC, abstractmethod
 from functools import wraps
 from itertools import chain
+from types import TracebackType
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
     Generic,
     List,
     Mapping,
     Optional,
     Sequence,
     Tuple,
+    Type,
     Union,
     cast,
 )
 
 from fast_depends._compat import PYDANTIC_V2
 from fast_depends.core import CallModel, build_call_model
 from fast_depends.dependencies import Depends
@@ -146,15 +148,20 @@
         callback_timeout: Optional[float] = None,
         raise_timeout: bool = False,
         **kwargs: Any,
     ) -> Optional[DecodedMessage]:
         raise NotImplementedError()
 
     @abstractmethod
-    async def close(self) -> None:
+    async def close(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_val: Optional[BaseException] = None,
+        exec_tb: Optional[TracebackType] = None,
+    ) -> None:
         self.started = False
 
     @abstractmethod
     async def _parse_message(self, message: MsgType) -> PropanMessage[MsgType]:
         raise NotImplementedError()
 
     @abstractmethod
@@ -224,16 +231,21 @@
 
         await self.connect()
 
     async def __aenter__(self) -> Self:
         await self.connect()
         return self
 
-    async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
-        await self.close()
+    async def __aexit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc_val: Optional[BaseException],
+        exec_tb: Optional[TracebackType],
+    ) -> None:
+        await self.close(exc_type, exc_val, exec_tb)
 
     def _wrap_handler(
         self,
         func: Union[Callable[..., T], Callable[..., Awaitable[T]]],
         retry: Union[bool, int] = False,
         extra_dependencies: Sequence[Depends] = (),
         decode_message: CustomDecoder[MsgType] = None,
```

### Comparing `propan-0.1.4.0/propan/brokers/_model/routing.py` & `propan-0.1.4.1/propan/brokers/_model/routing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/brokers/_model/schemas.py` & `propan-0.1.4.1/propan/brokers/_model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/brokers/_model/utils.py` & `propan-0.1.4.1/propan/brokers/_model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.4.1/propan/brokers/kafka/kafka_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import asyncio
 import logging
 from functools import partial, wraps
+from types import TracebackType
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
     List,
     NoReturn,
     Optional,
     Sequence,
     Tuple,
+    Type,
     Union,
 )
 from uuid import uuid4
 
+import anyio
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from aiokafka.structs import ConsumerRecord
 from fast_depends.dependencies import Depends
 from kafka.coordinator.assignors.abstract import AbstractPartitionAssignor
 from kafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
 from typing_extensions import Literal, TypeAlias, TypeVar
 
@@ -106,16 +109,21 @@
                 "sasl_kerberos_domain_name",
                 "sasl_oauth_token_provider",
             }
             and v
         }
         return partial(AIOKafkaConsumer, **consumer_kwargs)
 
-    async def close(self) -> None:
-        await super().close()
+    async def close(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_val: Optional[BaseException] = None,
+        exec_tb: Optional[TracebackType] = None,
+    ) -> None:
+        await super().close(exc_type, exc_val, exec_tb)
 
         for f in self.response_callbacks.values():
             f.cancel()
         self.response_callbacks = {}
 
         for handler in self.handlers:
             if handler.task is not None:
@@ -324,22 +332,25 @@
             key=key,
             partition=partition,
             timestamp_ms=timestamp_ms,
             headers=[(i, j.encode()) for i, j in headers_to_send.items()],
         )
 
         if response_future is not None:
-            try:
-                response = await asyncio.wait_for(response_future, callback_timeout)
-            except asyncio.TimeoutError as e:
-                if raise_timeout is True:
-                    raise e
-                return None
+            if raise_timeout:
+                scope = anyio.fail_after
             else:
-                return response
+                scope = anyio.move_on_after
+
+            msg: Any = None
+            with scope(callback_timeout):
+                msg = await response_future
+
+            if msg:
+                return await self._decode_message(msg)
 
     @property
     def fmt(self) -> str:
         return self._fmt or (
             "%(asctime)s %(levelname)s - "
             f"%(topic)-{self.__max_topic_len}s | "
             "%(message_id)-10s "
@@ -369,26 +380,26 @@
         connected = True
         while True:
             try:
                 msg = await handler.consumer.getone()
 
             except Exception as e:
                 if connected is True:
-                    self._log(e, logging.WATNING, c)
+                    self._log(e, logging.WARNING, c)
                     connected = False
-                await asyncio.sleep(5)
+                await anyio.sleep(5)
 
             else:
                 if connected is False:
                     self._log("Connection established", logging.INFO, c)
                     connected = True
 
                 await handler.callback(msg)
 
     async def _consume_response(self, message: KafkaMessage):
         correlation_id = message.headers.get("correlation_id")
         if correlation_id is not None:
             callback = self.response_callbacks.pop(correlation_id, None)
             if callback is not None:
-                callback.set_result(await self._decode_message(message))
+                callback.set_result(message)
 
         raise SkipMessage()
```

### Comparing `propan-0.1.4.0/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.4.1/propan/brokers/kafka/kafka_broker.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import logging
 from asyncio import AbstractEventLoop, Future
 from ssl import SSLContext
+from types import TracebackType
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
     List,
     Optional,
     Sequence,
     Tuple,
+    Type,
     Union,
 )
 
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from aiokafka.abc import AbstractTokenProvider
 from aiokafka.producer.producer import _missing
 from aiokafka.structs import ConsumerRecord
@@ -148,15 +150,20 @@
         send_backoff_ms: int = 100,
         ssl_context: Optional[SSLContext] = None,
         enable_idempotence: bool = False,
         transactional_id: Optional[str] = None,
         transaction_timeout_ms: int = 60000,
     ) -> AIOKafkaConsumer: ...
     async def _connect(self, *args: Any, **kwargs: Any) -> AIOKafkaConsumer: ...
-    async def close(self) -> None: ...
+    async def close(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_val: Optional[BaseException] = None,
+        exec_tb: Optional[TracebackType] = None,
+    ) -> None: ...
     def handle(  # type: ignore[override]
         self,
         *topics: str,
         group_id: Optional[str] = None,
         key_deserializer: Optional[Callable[[bytes], Any]] = None,
         value_deserializer: Optional[Callable[[bytes], Any]] = None,
         fetch_max_wait_ms: int = 500,
```

### Comparing `propan-0.1.4.0/propan/brokers/kafka/routing.pyi` & `propan-0.1.4.1/propan/brokers/kafka/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/brokers/kafka/schemas.py` & `propan-0.1.4.1/propan/brokers/kafka/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/brokers/nats/nats_broker.py` & `propan-0.1.4.1/propan/brokers/nats/nats_broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import asyncio
 import logging
 from functools import wraps
 from secrets import token_hex
+from types import TracebackType
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
     List,
     Optional,
     Sequence,
+    Type,
     TypeVar,
     Union,
 )
 
+import anyio
 import nats
 from fast_depends.dependencies import Depends
 from nats.aio.client import Callback, Client, ErrorCallback
 from nats.aio.msg import Msg
 from typing_extensions import TypeAlias
 
 from propan.brokers._model import BrokerUsecase
@@ -169,33 +172,39 @@
             headers={
                 **(headers or {}),
                 "content-type": content_type or "",
             },
         )
 
         if reply_to:
-            try:
-                msg = await asyncio.wait_for(future, callback_timeout)
+            if raise_timeout:
+                scope = anyio.fail_after
+            else:
+                scope = anyio.move_on_after
+
+            msg: Any = None
+            with scope(callback_timeout):
+                msg = await future
+
+            if msg:
                 if msg.headers:  # pragma: no branch
                     if (
                         msg.headers.get(nats.js.api.Header.STATUS)
                         == nats.aio.client.NO_RESPONDERS_STATUS
                     ):
                         raise nats.errors.NoRespondersError
-            except asyncio.TimeoutError as e:
-                await sub.unsubscribe()
-                future.cancel()
-                if raise_timeout is True:
-                    raise e
-                return None
-            else:
                 return await self._decode_message(await self._parse_message(msg))
 
-    async def close(self) -> None:
-        await super().close()
+    async def close(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_val: Optional[BaseException] = None,
+        exec_tb: Optional[TracebackType] = None,
+    ) -> None:
+        await super().close(exc_type, exc_val, exec_tb)
         for h in self.handlers:
             if h.subscription is not None:
                 await h.subscription.unsubscribe()
                 h.subscription = None
 
         if self._connection is not None:
             await self._connection.drain()
```

### Comparing `propan-0.1.4.0/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.4.1/propan/brokers/nats/nats_broker.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import logging
 import ssl
+from types import TracebackType
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
     List,
     Optional,
     Sequence,
+    Type,
     TypeVar,
     Union,
 )
 
 from fast_depends.dependencies import Depends
 from nats.aio.client import (
     DEFAULT_CONNECT_TIMEOUT,
@@ -158,14 +160,19 @@
         self,
         *,
         url: Optional[str] = None,
         error_cb: Optional[ErrorCallback] = None,
         reconnected_cb: Optional[Callback] = None,
         **kwargs: Any,
     ) -> Client: ...
-    async def close(self) -> None: ...
+    async def close(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_val: Optional[BaseException] = None,
+        exec_tb: Optional[TracebackType] = None,
+    ) -> None: ...
     async def _parse_message(self, message: Msg) -> NatsMessage: ...
     def _process_message(
         self,
         func: Callable[[NatsMessage], Awaitable[T]],
         watcher: Optional[BaseWatcher] = None,
     ) -> Callable[[NatsMessage], Awaitable[T]]: ...
```

### Comparing `propan-0.1.4.0/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.4.1/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/brokers/nats/routing.pyi` & `propan-0.1.4.1/propan/brokers/nats/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/brokers/nats/schemas.py` & `propan-0.1.4.1/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.4.1/propan/brokers/rabbit/rabbit_broker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import asyncio
 from contextlib import asynccontextmanager
 from functools import wraps
+from types import TracebackType
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
     List,
     Optional,
@@ -14,15 +14,17 @@
     TypeVar,
     Union,
 )
 from uuid import uuid4
 
 import aio_pika
 import aiormq
+import anyio
 from aio_pika.abc import DeliveryMode
+from anyio.streams.memory import MemoryObjectReceiveStream
 from fast_depends.dependencies import Depends
 from typing_extensions import TypeAlias
 from yarl import URL
 
 from propan._compat import model_to_dict
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
@@ -44,15 +46,15 @@
     _connection: Optional[aio_pika.RobustConnection]
     _channel: Optional[aio_pika.RobustChannel]
     _queues: Dict[RabbitQueue, aio_pika.RobustQueue]
     _exchanges: Dict[RabbitExchange, aio_pika.RobustExchange]
 
     __max_queue_len: int
     __max_exchange_len: int
-    _rpc_lock: asyncio.Lock
+    _rpc_lock: anyio.Lock
 
     def __init__(
         self,
         url: Union[str, URL, None] = None,
         *,
         log_fmt: Optional[str] = None,
         consumers: Optional[int] = None,
@@ -67,23 +69,28 @@
             protocol=protocol,
             protocol_version=protocol_version,
             **kwargs,
         )
         self._max_consumers = consumers
 
         self._channel = None
-        self._rpc_lock = asyncio.Lock()
+        self._rpc_lock = anyio.Lock()
 
         self.__max_queue_len = 4
         self.__max_exchange_len = 4
         self._queues = {}
         self._exchanges = {}
 
-    async def close(self) -> None:
-        await super().close()
+    async def close(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_val: Optional[BaseException] = None,
+        exec_tb: Optional[TracebackType] = None,
+    ) -> None:
+        await super().close(exc_type, exc_val, exec_tb)
         if self._channel is not None:
             await self._channel.close()
             self._channel = None
 
         if self._connection is not None:
             await self._connection.close()
             self._connection = None
@@ -91,17 +98,15 @@
         self._queues = {}
         self._exchanges = {}
 
     async def _connect(
         self,
         **kwargs: Any,
     ) -> aio_pika.RobustConnection:
-        connection = await aio_pika.connect_robust(
-            **kwargs, loop=asyncio.get_event_loop()
-        )
+        connection = await aio_pika.connect_robust(**kwargs)
 
         if self._channel is None:  # pragma: no branch
             max_consumers = self._max_consumers
             self._channel = await connection.channel()
 
             if max_consumers:
                 c = self._get_log_context(None, RabbitQueue(""), RabbitExchange(""))
@@ -218,20 +223,24 @@
                 timeout=timeout,
             )
 
             if response_queue is None:
                 return r
 
             else:
-                try:
-                    msg = await asyncio.wait_for(response_queue.get(), callback_timeout)
-                except asyncio.TimeoutError as e:
-                    if raise_timeout is True:  # pragma: no branch
-                        raise e
+                if raise_timeout:
+                    scope = anyio.fail_after
                 else:
+                    scope = anyio.move_on_after
+
+                msg: Any = None
+                with scope(callback_timeout):
+                    msg = await response_queue.receive()
+
+                if msg:
                     return await self._decode_message(msg)
 
     async def _init_handler(
         self,
         handler: Handler,
     ) -> aio_pika.abc.AbstractRobustQueue:
         queue = await self.declare_queue(handler.queue)
@@ -412,33 +421,41 @@
             raise ValueError(
                 f"Queue '{queue}' should be 'str' | 'RabbitQueue' instance"
             )
     return queue
 
 
 class RPCCallback:
-    def __init__(self, lock: asyncio.Lock, broker: RabbitBroker):
+    def __init__(self, lock: anyio.Lock, broker: RabbitBroker):
         self.lock = lock
         self.broker = broker
 
-    async def __aenter__(self) -> Tuple[str, asyncio.Queue]:
-        response_queue: asyncio.Queue[PropanMessage] = asyncio.Queue(1)
+    async def __aenter__(self) -> Tuple[str, MemoryObjectReceiveStream]:
+        (
+            send_response_stream,
+            receive_response_stream,
+        ) = anyio.create_memory_object_stream(max_buffer_size=1)
         await self.lock.acquire()
 
         self.queue = callback_queue = await self.broker._channel.get_queue(RABBIT_REPLY)
 
         async def handle_response(msg: RabbitMessage) -> None:
             propan_message = await self.broker._parse_message(msg)
-            await response_queue.put(propan_message)
+            await send_response_stream.send(propan_message)
 
         self.consumer_tag = await callback_queue.consume(handle_response, no_ack=True)
 
-        return callback_queue.name, response_queue
+        return callback_queue.name, receive_response_stream
 
-    async def __aexit__(self, *args, **kwargs):
+    async def __aexit__(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_val: Optional[BaseException] = None,
+        exec_tb: Optional[TracebackType] = None,
+    ):
         self.lock.release()
         await self.queue.cancel(self.consumer_tag)
 
 
 @asynccontextmanager
 async def fake_context(reply_to: str) -> Tuple[str, None]:
     yield reply_to, None
```

### Comparing `propan-0.1.4.0/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.4.1/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 from ssl import SSLContext
+from types import TracebackType
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
     List,
     Optional,
@@ -189,15 +190,15 @@
             timestamp: message sending time
             expiration: message lifetime (in seconds)
             type: message type (for consumers)
             user_id: RabbitMQ user who sent the message
             app_id: application identifier (for consumers)
             callback: wait for response
             callback_timeout: response waiting time
-            raise_timeout: if False timeout returns None instead asyncio.TimeoutError
+            raise_timeout: if False timeout returns None instead TimeoutError
 
         Returns:
             `aiormq.abc.ConfirmationFrameType` if you are not waiting for response
             (reply_to and callback are not specified)
 
             `DecodedMessage` | `None` if response is expected
 
@@ -235,15 +236,20 @@
             description: AsyncAPI channel object description
 
         Returns:
             Async or sync function decorator
         """
     async def start(self) -> None:
         """Initialize RabbitMQ connection and startup all consumers"""
-    async def close(self) -> None:
+    async def close(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_val: Optional[BaseException] = None,
+        exec_tb: Optional[TracebackType] = None,
+    ) -> None:
         """Close RabbitMQ connection"""
     async def declare_queue(self, queue: RabbitQueue) -> aio_pika.RobustQueue:
         """Check existence or create RabbitMQ queue"""
     async def declare_exchange(
         self, exchange: RabbitExchange
     ) -> aio_pika.RobustExchange:
         """Check existence or create RabbitMQ exchange"""
```

### Comparing `propan-0.1.4.0/propan/brokers/rabbit/routing.pyi` & `propan-0.1.4.1/propan/brokers/rabbit/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/brokers/rabbit/schemas.py` & `propan-0.1.4.1/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/brokers/redis/redis_broker.py` & `propan-0.1.4.1/propan/brokers/redis/redis_broker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import asyncio
 import logging
 from functools import wraps
+from types import TracebackType
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
     List,
     NoReturn,
     Optional,
     Sequence,
+    Type,
     TypeVar,
 )
 from uuid import uuid4
 
+import anyio
+from anyio.streams.memory import MemoryObjectSendStream
 from fast_depends.dependencies import Depends
 from redis.asyncio.client import PubSub, Redis
 from redis.asyncio.connection import ConnectionPool, parse_url
 from typing_extensions import TypeAlias
 
 from propan._compat import model_parse, model_to_json
 from propan.brokers._model import BrokerUsecase
@@ -70,16 +74,21 @@
         **kwargs: Any,
     ) -> Redis:
         url_options = parse_url(url)
         url_options.update(kwargs)
         pool = ConnectionPool(**url_options)
         return Redis(connection_pool=pool)
 
-    async def close(self) -> None:
-        await super().close()
+    async def close(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_val: Optional[BaseException] = None,
+        exec_tb: Optional[TracebackType] = None,
+    ) -> None:
+        await super().close(exc_type, exc_val, exec_tb)
         for h in self.handlers:
             if h.task is not None:  # pragma: no branch
                 h.task.cancel()
                 h.task = None
 
             if h.subscription is not None:  # pragma: no branch
                 await h.subscription.unsubscribe()
@@ -182,21 +191,24 @@
                 raise ValueError(
                     "You should use `reply_to` to send response to long-living queue "
                     "and `callback` to get response in sync mode."
                 )
 
             callback_channel = str(uuid4())
             psub = self._connection.pubsub()
-            response_queue = asyncio.Queue(maxsize=1)
+            (
+                send_response_stream,
+                receive_response_stream,
+            ) = anyio.create_memory_object_stream(max_buffer_size=1)
             await psub.subscribe(callback_channel)
-            task = asyncio.create_task(_consume_one(response_queue, psub))
+            task = asyncio.create_task(_consume_one(send_response_stream, psub))
         else:
             callback_channel = reply_to
             psub = None
-            response_queue = None
+            send_response_stream = receive_response_stream = None
             task = None
 
         await self._connection.publish(
             channel,
             model_to_json(
                 RM(
                     data=msg,
@@ -205,20 +217,19 @@
                         **(headers or {}),
                     },
                     reply_to=callback_channel,
                 )
             ),
         )
 
-        if psub and response_queue and task:
+        if psub and receive_response_stream and task:
             try:
-                response = await asyncio.wait_for(
-                    response_queue.get(), callback_timeout
-                )
-            except asyncio.TimeoutError as e:
+                with anyio.fail_after(callback_timeout):
+                    response = await receive_response_stream.receive()
+            except TimeoutError as e:
                 if raise_timeout is True:
                     raise e
                 return None
             else:
                 return await self._decode_message(await self._parse_message(response))
             finally:
                 await psub.unsubscribe(callback_channel)
@@ -281,25 +292,25 @@
                     ignore_subscribe_messages=True,
                     timeout=self._polling_interval,
                 )
             except Exception:
                 if connected is True:
                     self._log("Connection broken", logging.WARNING, c)
                     connected = False
-                await asyncio.sleep(5)
+                await anyio.sleep(5)
             else:
                 if connected is False:
                     self._log("Connection established", logging.INFO, c)
                     connected = True
 
                 if m:  # pragma: no branch
                     await handler.callback(m)
             finally:
-                await asyncio.sleep(0.01)
+                await anyio.sleep(0.01)
 
 
-async def _consume_one(queue: asyncio.Queue, psub: PubSub) -> NoReturn:
+async def _consume_one(queue: MemoryObjectSendStream[any], psub: PubSub) -> NoReturn:
     async for m in psub.listen():
         t = m.get("type")
         if t and "message" in t:  # pragma: no branch
-            await queue.put(m)
+            await queue.send(m)
             break
```

### Comparing `propan-0.1.4.0/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.4.1/propan/brokers/redis/redis_broker.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from types import TracebackType
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
     List,
     Mapping,
@@ -130,15 +131,20 @@
         - `unix://`: creates a Unix Domain Socket connection.
 
         Url will be parsed to kwargs and partially replaced by keywords arguments if they specified.
         """
     async def _connect(self, *args: Any, **kwargs: Any) -> Redis[bytes]: ...
     async def start(self) -> None:
         """Initialize Redis connection and startup all consumers"""
-    async def close(self) -> None:
+    async def close(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_val: Optional[BaseException] = None,
+        exec_tb: Optional[TracebackType] = None,
+    ) -> None:
         """Cancel all consumers tasks and subscribtions, close Redis connection"""
     def handle(  # type: ignore[override]
         self,
         channel: str,
         *,
         pattern: bool = False,
         dependencies: Sequence[Depends] = (),
@@ -175,15 +181,15 @@
         Args:
             message: encodable message to send
             channel: channel to publish message
             reply_to: queue to send response
             headers: message headers (for consumers)
             callback: wait for response
             callback_timeout: response waiting time
-            raise_timeout: if False timeout returns None instead asyncio.TimeoutError
+            raise_timeout: if False timeout returns None instead TimeoutError
 
         Returns:
             `None` if you are not waiting for response
             (reply_to and callback are not specified)
 
             `DecodedMessage` | `None` if response is expected
         """
```

### Comparing `propan-0.1.4.0/propan/brokers/redis/routing.pyi` & `propan-0.1.4.1/propan/brokers/redis/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/brokers/redis/schemas.py` & `propan-0.1.4.1/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/brokers/sqs/routing.pyi` & `propan-0.1.4.1/propan/brokers/sqs/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/brokers/sqs/schema.py` & `propan-0.1.4.1/propan/brokers/sqs/schema.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/brokers/sqs/sqs_broker.py` & `propan-0.1.4.1/propan/brokers/sqs/sqs_broker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import asyncio
 import logging
 from functools import wraps
+from types import TracebackType
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
     List,
     NoReturn,
     Optional,
     Sequence,
+    Type,
     TypeVar,
     Union,
 )
 from uuid import uuid4
 
+import anyio
 from aiobotocore.client import AioBaseClient
 from aiobotocore.session import get_session
 from fast_depends.dependencies import Depends
 from typing_extensions import TypeAlias
 
 from propan._compat import model_to_dict
 from propan.brokers._model import BrokerUsecase
@@ -82,16 +85,21 @@
         client: AioBaseClient = await session._create_client(
             service_name="sqs", endpoint_url=url, **kwargs
         )
         context.set_global("client", client)
         await client.__aenter__()
         return client
 
-    async def close(self) -> None:
-        await super().close()
+    async def close(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_val: Optional[BaseException] = None,
+        exec_tb: Optional[TracebackType] = None,
+    ) -> None:
+        await super().close(exc_type, exc_val, exec_tb)
         for f in self.response_callbacks.values():
             f.cancel()
         self.response_callbacks = {}
 
         for h in self.handlers:
             if h.task is not None:
                 h.task.cancel()
@@ -275,22 +283,25 @@
             reply_to=reply_to,
             correlation_id=correlation_id,
         )
 
         await self._connection.send_message(QueueUrl=queue_url, **params)
 
         if response_future is not None:
-            try:
-                response = await asyncio.wait_for(response_future, callback_timeout)
-            except asyncio.TimeoutError as e:
-                if raise_timeout is True:
-                    raise e
-                return None
+            if raise_timeout:
+                scope = anyio.fail_after
             else:
-                return response
+                scope = anyio.move_on_after
+
+            msg: Any = None
+            with scope(callback_timeout):
+                msg = await response_future
+
+            if msg:
+                return await self._decode_message(msg)
 
     async def create_queue(self, queue: SQSQueue) -> QueueUrl:
         url = self._queues.get(queue.name)
         if url is None:  # pragma: no branch
             url = (
                 await self._connection.create_queue(
                     QueueName=queue.name,
@@ -347,15 +358,15 @@
 
                 except Exception as e:
                     if connected is True:
                         self._log(e, logging.WARNING, c)
                         self._queues.pop(handler.queue.name)
                         connected = False
 
-                    await asyncio.sleep(5)
+                    await anyio.sleep(5)
 
                 else:
                     if connected is False:
                         self._log("Connection established", logging.INFO, c)
                         connected = True
 
                     messages = r.get("Messages", [])
@@ -364,24 +375,24 @@
                             await handler.callback(msg, True)
                         except Exception:
                             has_trash_messages = True
                         else:
                             has_trash_messages = False
 
                     if has_trash_messages is True:
-                        await asyncio.sleep(
+                        await anyio.sleep(
                             handler.consumer_params.get("WaitTimeSeconds", 1.0)
                         )
 
     async def _consume_response(self, message: SQSMessage):
         correlation_id = message.headers.get("correlation_id")
         if correlation_id is not None:
             callback = self.response_callbacks.pop(correlation_id, None)
             if callback is not None:
-                callback.set_result(await self._decode_message(message))
+                callback.set_result(message)
                 return
 
         raise SkipMessage()
 
     @property
     def fmt(self) -> str:
         return self._fmt or (
```

### Comparing `propan-0.1.4.0/propan/brokers/sqs/sqs_broker.pyi` & `propan-0.1.4.1/propan/brokers/sqs/sqs_broker.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import asyncio
 import logging
+from types import TracebackType
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     NoReturn,
     Optional,
     Sequence,
+    Type,
     TypeVar,
     Union,
 )
 
 from aiobotocore.client import AioBaseClient
 from aiobotocore.config import AioConfig
 from fast_depends.dependencies import Depends
@@ -69,15 +71,20 @@
         verify: Optional[bool] = None,
         aws_access_key_id: Optional[str] = None,
         aws_secret_access_key: Optional[str] = None,
         aws_session_token: Optional[str] = None,
         config: Optional[AioConfig] = None,
     ) -> AioBaseClient:
         """"""
-    async def close(self) -> None:
+    async def close(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_val: Optional[BaseException] = None,
+        exec_tb: Optional[TracebackType] = None,
+    ) -> None:
         """"""
     async def publish(  # type: ignore[override]
         self,
         message: SendableMessage,
         queue: str,
         *,
         headers: Optional[Dict[str, str]] = None,
```

### Comparing `propan-0.1.4.0/propan/cli/app.py` & `propan-0.1.4.1/propan/cli/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 import logging
 from typing import Dict, List, Optional
 
 from anyio import create_memory_object_stream, create_task_group
 from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
 from typing_extensions import Protocol
 
@@ -83,15 +82,14 @@
         self._init_async_cycle()
         async with create_task_group() as tg:
             set_exit(lambda *_: tg.start_soon(self.__exit, True))
             tg.start_soon(self._stop, log_level)
             tg.start_soon(self._start, log_level)
 
     def _init_async_cycle(self) -> None:
-        self.loop = asyncio.get_event_loop()
         if not self._stop_stream and not self._receive_stream:
             self._stop_stream, self._receive_stream = create_memory_object_stream(1)
 
     async def _start(self, log_level: int = logging.INFO) -> None:
         self._log(log_level, "Propan app starting...")
         await self._startup()
         self._log(log_level, "Propan app started successfully! To exit press CTRL+C")
```

### Comparing `propan-0.1.4.0/propan/cli/main.py` & `propan-0.1.4.1/propan/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import asyncio
 import logging
 import sys
 from pathlib import Path
 from typing import Dict, Optional
 
+import anyio
 import typer
 
 from propan.__about__ import __version__
 from propan.cli.docs import docs_app
 from propan.cli.startproject import create_app
 from propan.cli.utils.imports import get_app_path, try_import_propan
 from propan.cli.utils.logs import LogLevels, get_log_level, set_log_level
@@ -116,8 +116,8 @@
         try:
             import uvloop
         except ImportError:
             logger.warning("You have no installed `uvloop`")
         else:
             uvloop.install()
 
-    asyncio.run(propan_app.run(log_level=app_level))
+    anyio.run(propan_app.run, app_level)
```

### Comparing `propan-0.1.4.0/propan/cli/docs/app.py` & `propan-0.1.4.1/propan/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/cli/docs/gen.py` & `propan-0.1.4.1/propan/cli/docs/gen.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/cli/docs/serving.py` & `propan-0.1.4.1/propan/cli/docs/serving.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/cli/startproject/core.py` & `propan-0.1.4.1/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/cli/startproject/async_app/app.py` & `propan-0.1.4.1/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/cli/startproject/async_app/core.py` & `propan-0.1.4.1/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.4.1/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/cli/startproject/async_app/nats.py` & `propan-0.1.4.1/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.4.1/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/cli/startproject/async_app/redis.py` & `propan-0.1.4.1/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/cli/startproject/async_app/sqs.py` & `propan-0.1.4.1/propan/cli/startproject/async_app/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/cli/supervisors/basereload.py` & `propan-0.1.4.1/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/cli/supervisors/multiprocess.py` & `propan-0.1.4.1/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/cli/supervisors/utils.py` & `propan-0.1.4.1/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/cli/supervisors/watchfiles.py` & `propan-0.1.4.1/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/cli/utils/imports.py` & `propan-0.1.4.1/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/cli/utils/logs.py` & `propan-0.1.4.1/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/cli/utils/parser.py` & `propan-0.1.4.1/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/fastapi/__init__.py` & `propan-0.1.4.1/propan/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/fastapi/core/route.py` & `propan-0.1.4.1/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/fastapi/core/router.py` & `propan-0.1.4.1/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/fastapi/kafka/router.pyi` & `propan-0.1.4.1/propan/fastapi/kafka/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/fastapi/nats/router.pyi` & `propan-0.1.4.1/propan/fastapi/nats/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/fastapi/rabbit/router.pyi` & `propan-0.1.4.1/propan/fastapi/rabbit/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/fastapi/redis/router.pyi` & `propan-0.1.4.1/propan/fastapi/redis/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/fastapi/sqs/router.pyi` & `propan-0.1.4.1/propan/fastapi/sqs/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/log/formatter.py` & `propan-0.1.4.1/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/log/logging.py` & `propan-0.1.4.1/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/test/__init__.py` & `propan-0.1.4.1/propan/test/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/test/kafka.py` & `propan-0.1.4.1/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/test/nats.py` & `propan-0.1.4.1/propan/test/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/test/rabbit.py` & `propan-0.1.4.1/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/test/redis.py` & `propan-0.1.4.1/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/test/sqs.py` & `propan-0.1.4.1/propan/test/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/utils/functions.py` & `propan-0.1.4.1/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/utils/context/main.py` & `propan-0.1.4.1/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/propan/utils/context/types.py` & `propan-0.1.4.1/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/LICENSE` & `propan-0.1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/README.md` & `propan-0.1.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -24,19 +24,19 @@
     <a href="https://github.com/Lancetnik/Propan/blob/main/LICENSE" target="_blank">
         <img alt="GitHub" src="https://img.shields.io/github/license/Lancetnik/Propan?color=%23007ec6">
     </a>
 </p>
 
 # Propan
 
-**Propan** - just *~~an another one HTTP~~* a **declarative Python MQ framework**. It's following by <a href="https://fastapi.tiangolo.com/ru/" target="_blank">*fastapi*</a>, simplify Message Brokers around code writing and provides a helpful development toolkit, which existed only in HTTP-frameworks world until now.
+**Propan** - just *~~an another one HTTP~~* a **declarative Python MQ framework**. It's following by <a href="https://FastAPI.tiangolo.com/ru/" target="_blank">*FastAPI*</a>, simplify Message Brokers around code writing and provides a helpful development toolkit, which existed only in HTTP-frameworks world until now.
 
 It's designed to create reactive microservices around <a href="https://microservices.io/patterns/communication-style/messaging.html" target="_blank">Messaging Architecture</a>.
 
-It is a modern, high-level framework on top of popular specific Python brokers libraries, based on <a href="https://docs.pydantic.dev/" target="_blank">*pydantic*</a> and <a href="https://fastapi.tiangolo.com/ru/" target="_blank">*fastapi*</a>, <a href="https://docs.pytest.org/en/latest/" target="_blank">*pytest*</a> concepts.
+It is a modern, high-level framework on top of popular specific Python brokers libraries, based on <a href="https://docs.pydantic.dev/" target="_blank">*pydantic*</a> and <a href="https://FastAPI.tiangolo.com/ru/" target="_blank">*FastAPI*</a>, <a href="https://docs.pytest.org/en/latest/" target="_blank">*pytest*</a> concepts.
 
 ---
 
 **Documentation**: <a href="https://lancetnik.github.io/Propan/" target="_blank">https://lancetnik.github.io/Propan/</a>
 
 ---
 
@@ -70,19 +70,29 @@
 | **Kafka**         | :warning: **beta** :warning:                            | :mag: planning :mag: |
 | **SQS**           | :warning: **beta** :warning:                            | :mag: planning :mag: |
 | **NatsJS**        | :hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag: |
 | **MQTT**          | :mag: planning :mag:                                    | :mag: planning :mag: |
 | **Redis Streams** | :mag: planning :mag:                                    | :mag: planning :mag: |
 | **Pulsar**        | :mag: planning :mag:                                    | :mag: planning :mag: |
 
-### Community
+---
+
+### ⭐ Support the project ⭐
+
+If you are interested in this project, please give me feedback by:
 
-If you are interested in this project, please give me feedback by star or/and watch repository.
+- giving the [repository](https://github.com/Lancetnik/Propan) a star
 
-If you have any questions or ideas about features to implement, welcome to [discussions](https://github.com/Lancetnik/Propan/discussions).
+- tweet about <a href="https://twitter.com/PropanFramework" target="_blank">**Propan**</a> and let me and others know why you use it.
+
+- joining <a href="https://discord.gg/ChhMXJpvz7" target="_blank">Discord server</a>.
+
+Your support helps me to stay in touch with you and encourages us to
+continue developing and improving the library. Thank you for your
+support!
 
 ---
 
 ## Declarative?
 
 With declarative tools you can define **what you need to get**. With traditional imperative tools you must write **what you need to do**.
 
@@ -208,18 +218,15 @@
 
 ## Dependencies
 
 **Propan** a has dependencies management policy close to `pytest fixtures`.
 You can specify in functions arguments which dependencies
 you would to use. Framework passes them from the global Context object.
 
-Already existed context fields are: *app*, *broker*, *context* (itself), *logger* and *message*.
-If you call not existing field, raises *pydantic.ValidationError* value.
-
-But you can specify your own dependencies, call dependencies functions (like `Fastapi Depends`)
+Also, you can specify your own dependencies, call dependencies functions (like `FastAPI Depends`)
 and [more](https://github.com/Lancetnik/Propan/tree/main/examples/dependencies).
 
 ```python
 import aio_pika
 from propan import PropanApp, RabbitBroker, Context, Depends
 
 rabbit_broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
@@ -252,14 +259,15 @@
 ## CLI power
 
 **Propan** has its own CLI tool that provided the following features:
 
 * project generation
 * multiprocessing workers
 * project hot reloading
+* documentation generating and hosting
 * custom command line arguments passing
 
 ### Context passing
 
 For example: pass your current *.env* project setting to context
 
 ```bash
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
                                  [Propan_logo]
           [Tests_coverage] [Coverage] [Package_version] [downloads]
                      [Supported_Python_versions] [GitHub]
 # Propan **Propan** - just *~~an another one HTTP~~* a **declarative Python MQ
-framework**. It's following by *fastapi*, simplify Message Brokers around code
+framework**. It's following by *FastAPI*, simplify Message Brokers around code
 writing and provides a helpful development toolkit, which existed only in HTTP-
 frameworks world until now. It's designed to create reactive microservices
 around Messaging_Architecture. It is a modern, high-level framework on top of
-popular specific Python brokers libraries, based on *pydantic* and *fastapi*,
+popular specific Python brokers libraries, based on *pydantic* and *FastAPI*,
 *pytest* concepts. --- **Documentation**: https://lancetnik.github.io/Propan/ -
 -- ### The key features are * **Simple**: Designed to be easy to use and learn.
 * **Intuitive**: Great editor support. Autocompletion everywhere. *
 [**Dependencies management**](#dependencies): Minimization of code duplication.
 Access to dependencies at any level of the call stack. * [**Integrations**]
 (#http-frameworks-integrations): **Propan** is fully compatible with any_HTTP
 framework you want * **MQ independent**: Single interface to popular MQ: *
@@ -31,18 +31,20 @@
 heavy_check_mark: **stable** :heavy_check_mark: | :mag: planning :mag: | |
 **Nats** | :heavy_check_mark: **stable** :heavy_check_mark: | :mag: planning :
 mag: | | **Kafka** | :warning: **beta** :warning: | :mag: planning :mag: | |
 **SQS** | :warning: **beta** :warning: | :mag: planning :mag: | | **NatsJS** |
 :hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag:
 | | **MQTT** | :mag: planning :mag: | :mag: planning :mag: | | **Redis
 Streams** | :mag: planning :mag: | :mag: planning :mag: | | **Pulsar** | :mag:
-planning :mag: | :mag: planning :mag: | ### Community If you are interested in
-this project, please give me feedback by star or/and watch repository. If you
-have any questions or ideas about features to implement, welcome to
-[discussions](https://github.com/Lancetnik/Propan/discussions). --- ##
+planning :mag: | :mag: planning :mag: | --- ### â­ Support the project â­ If
+you are interested in this project, please give me feedback by: - giving the
+[repository](https://github.com/Lancetnik/Propan) a star - tweet about
+**Propan** and let me and others know why you use it. - joining Discord_server.
+Your support helps me to stay in touch with you and encourages us to continue
+developing and improving the library. Thank you for your support! --- ##
 Declarative? With declarative tools you can define **what you need to get**.
 With traditional imperative tools you must write **what you need to do**. Take
 a look at classic imperative tools, such as aio-pika, pika, redis-py, nats-py,
 etc. This is the **Quickstart** with the *aio-pika*: ```python import asyncio
 import aio_pika async def main(): connection = await aio_pika.connect_robust
 ( "amqp://guest:guest@127.0.0.1/" ) queue_name = "test_queue" async with
 connection: channel = await connection.channel() queue = await
@@ -73,46 +75,44 @@
 function arguments to types according to their annotation. ```python from
 pydantic import BaseModel from propan import PropanApp, Context, RabbitBroker
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp
 (broker) class SimpleMessage(BaseModel): key: int @broker.handle("test2") async
 def second_handler(body: SimpleMessage): assert isinstance(body.key, int) ``` -
 -- ## Dependencies **Propan** a has dependencies management policy close to
 `pytest fixtures`. You can specify in functions arguments which dependencies
-you would to use. Framework passes them from the global Context object. Already
-existed context fields are: *app*, *broker*, *context* (itself), *logger* and
-*message*. If you call not existing field, raises *pydantic.ValidationError*
-value. But you can specify your own dependencies, call dependencies functions
-(like `Fastapi Depends`) and [more](https://github.com/Lancetnik/Propan/tree/
-main/examples/dependencies). ```python import aio_pika from propan import
-PropanApp, RabbitBroker, Context, Depends rabbit_broker = RabbitBroker("amqp://
-guest:guest@localhost:5672/") app = PropanApp(rabbit_broker) async def
-dependency(body: dict) -> bool: return True @rabbit_broker.handle("test") async
-def base_handler(body: dict, dep: bool = Depends(dependency), broker:
-RabbitBroker = Context()): assert dep is True assert broker is rabbit_broker
-``` --- ## Project Documentation **Propan** automatically generates
-documentation for your project according to the **AsyncAPI** specification. You
-can work with both generated artifacts and place a Web view of your
-documentation on resources available to related teams. The availability of such
-documentation significantly simplifies the integration of services: you can
-immediately see what channels and message format the application works with.
-And most importantly, it doesn't cost you anything - **Propan** has already
-done everything for you! ![HTML-page](https://lancetnik.github.io/Propan/
-assets/img/docs-html-short.png) --- ## CLI power **Propan** has its own CLI
-tool that provided the following features: * project generation *
-multiprocessing workers * project hot reloading * custom command line arguments
-passing ### Context passing For example: pass your current *.env* project
-setting to context ```bash propan run serve:app --env=.env.dev ``` ```python
-from propan import PropanApp, RabbitBroker from propan.annotations import
-ContextRepo from pydantic import BaseSettings broker = RabbitBroker("amqp://
-guest:guest@localhost:5672/") app = PropanApp(broker) class Settings
-(BaseSettings): ... @app.on_startup async def setup(env: str, context:
-ContextRepo): settings = Settings(_env_file=env) context.set_global("settings",
-settings) ``` ### Project template Also, **Propan CLI** is able to generate a
-production-ready application template: ```bash propan create async rabbit
-[projectname] ``` *Notice: project template require* `pydantic[dotenv]`
+you would to use. Framework passes them from the global Context object. Also,
+you can specify your own dependencies, call dependencies functions (like
+`FastAPI Depends`) and [more](https://github.com/Lancetnik/Propan/tree/main/
+examples/dependencies). ```python import aio_pika from propan import PropanApp,
+RabbitBroker, Context, Depends rabbit_broker = RabbitBroker("amqp://guest:
+guest@localhost:5672/") app = PropanApp(rabbit_broker) async def dependency
+(body: dict) -> bool: return True @rabbit_broker.handle("test") async def
+base_handler(body: dict, dep: bool = Depends(dependency), broker: RabbitBroker
+= Context()): assert dep is True assert broker is rabbit_broker ``` --- ##
+Project Documentation **Propan** automatically generates documentation for your
+project according to the **AsyncAPI** specification. You can work with both
+generated artifacts and place a Web view of your documentation on resources
+available to related teams. The availability of such documentation
+significantly simplifies the integration of services: you can immediately see
+what channels and message format the application works with. And most
+importantly, it doesn't cost you anything - **Propan** has already done
+everything for you! ![HTML-page](https://lancetnik.github.io/Propan/assets/img/
+docs-html-short.png) --- ## CLI power **Propan** has its own CLI tool that
+provided the following features: * project generation * multiprocessing workers
+* project hot reloading * documentation generating and hosting * custom command
+line arguments passing ### Context passing For example: pass your current
+*.env* project setting to context ```bash propan run serve:app --env=.env.dev
+``` ```python from propan import PropanApp, RabbitBroker from
+propan.annotations import ContextRepo from pydantic import BaseSettings broker
+= RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp(broker)
+class Settings(BaseSettings): ... @app.on_startup async def setup(env: str,
+context: ContextRepo): settings = Settings(_env_file=env) context.set_global
+("settings", settings) ``` ### Project template Also, **Propan CLI** is able to
+generate a production-ready application template: ```bash propan create async
+rabbit [projectname] ``` *Notice: project template require* `pydantic[dotenv]`
 *installation.* Run the created project: ```bash # Run rabbimq first docker
 compose --file [projectname]/docker-compose.yaml up -d # Run project propan run
 [projectname].app.serve:app --env=.env --reload ``` Now you can enjoy a new
 development experience! --- ## HTTP Frameworks integrations ### Any Framework
 You can use **Propan** `MQBrokers` without `PropanApp`. Just *start* and *stop*
 them according to your application lifespan. ```python from propan import
 NatsBroker from sanic import Sanic app = Sanic("MyHelloWorldApp") broker =
```

### Comparing `propan-0.1.4.0/pyproject.toml` & `propan-0.1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.0/PKG-INFO` & `propan-0.1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.4.0
+Version: 0.1.4.1
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
@@ -116,19 +116,19 @@
     <a href="https://github.com/Lancetnik/Propan/blob/main/LICENSE" target="_blank">
         <img alt="GitHub" src="https://img.shields.io/github/license/Lancetnik/Propan?color=%23007ec6">
     </a>
 </p>
 
 # Propan
 
-**Propan** - just *~~an another one HTTP~~* a **declarative Python MQ framework**. It's following by <a href="https://fastapi.tiangolo.com/ru/" target="_blank">*fastapi*</a>, simplify Message Brokers around code writing and provides a helpful development toolkit, which existed only in HTTP-frameworks world until now.
+**Propan** - just *~~an another one HTTP~~* a **declarative Python MQ framework**. It's following by <a href="https://FastAPI.tiangolo.com/ru/" target="_blank">*FastAPI*</a>, simplify Message Brokers around code writing and provides a helpful development toolkit, which existed only in HTTP-frameworks world until now.
 
 It's designed to create reactive microservices around <a href="https://microservices.io/patterns/communication-style/messaging.html" target="_blank">Messaging Architecture</a>.
 
-It is a modern, high-level framework on top of popular specific Python brokers libraries, based on <a href="https://docs.pydantic.dev/" target="_blank">*pydantic*</a> and <a href="https://fastapi.tiangolo.com/ru/" target="_blank">*fastapi*</a>, <a href="https://docs.pytest.org/en/latest/" target="_blank">*pytest*</a> concepts.
+It is a modern, high-level framework on top of popular specific Python brokers libraries, based on <a href="https://docs.pydantic.dev/" target="_blank">*pydantic*</a> and <a href="https://FastAPI.tiangolo.com/ru/" target="_blank">*FastAPI*</a>, <a href="https://docs.pytest.org/en/latest/" target="_blank">*pytest*</a> concepts.
 
 ---
 
 **Documentation**: <a href="https://lancetnik.github.io/Propan/" target="_blank">https://lancetnik.github.io/Propan/</a>
 
 ---
 
@@ -162,19 +162,29 @@
 | **Kafka**         | :warning: **beta** :warning:                            | :mag: planning :mag: |
 | **SQS**           | :warning: **beta** :warning:                            | :mag: planning :mag: |
 | **NatsJS**        | :hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag: |
 | **MQTT**          | :mag: planning :mag:                                    | :mag: planning :mag: |
 | **Redis Streams** | :mag: planning :mag:                                    | :mag: planning :mag: |
 | **Pulsar**        | :mag: planning :mag:                                    | :mag: planning :mag: |
 
-### Community
+---
+
+### ⭐ Support the project ⭐
+
+If you are interested in this project, please give me feedback by:
 
-If you are interested in this project, please give me feedback by star or/and watch repository.
+- giving the [repository](https://github.com/Lancetnik/Propan) a star
 
-If you have any questions or ideas about features to implement, welcome to [discussions](https://github.com/Lancetnik/Propan/discussions).
+- tweet about <a href="https://twitter.com/PropanFramework" target="_blank">**Propan**</a> and let me and others know why you use it.
+
+- joining <a href="https://discord.gg/ChhMXJpvz7" target="_blank">Discord server</a>.
+
+Your support helps me to stay in touch with you and encourages us to
+continue developing and improving the library. Thank you for your
+support!
 
 ---
 
 ## Declarative?
 
 With declarative tools you can define **what you need to get**. With traditional imperative tools you must write **what you need to do**.
 
@@ -300,18 +310,15 @@
 
 ## Dependencies
 
 **Propan** a has dependencies management policy close to `pytest fixtures`.
 You can specify in functions arguments which dependencies
 you would to use. Framework passes them from the global Context object.
 
-Already existed context fields are: *app*, *broker*, *context* (itself), *logger* and *message*.
-If you call not existing field, raises *pydantic.ValidationError* value.
-
-But you can specify your own dependencies, call dependencies functions (like `Fastapi Depends`)
+Also, you can specify your own dependencies, call dependencies functions (like `FastAPI Depends`)
 and [more](https://github.com/Lancetnik/Propan/tree/main/examples/dependencies).
 
 ```python
 import aio_pika
 from propan import PropanApp, RabbitBroker, Context, Depends
 
 rabbit_broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
@@ -344,14 +351,15 @@
 ## CLI power
 
 **Propan** has its own CLI tool that provided the following features:
 
 * project generation
 * multiprocessing workers
 * project hot reloading
+* documentation generating and hosting
 * custom command line arguments passing
 
 ### Context passing
 
 For example: pass your current *.env* project setting to context
 
 ```bash
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

