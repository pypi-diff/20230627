# Comparing `tmp/helios-opentelemetry-sdk-1.0.94.tar.gz` & `tmp/helios-opentelemetry-sdk-1.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios-opentelemetry-sdk-1.0.94.tar", last modified: Mon Jun 26 05:08:34 2023, max compression
+gzip compressed data, was "helios-opentelemetry-sdk-1.0.95.tar", last modified: Tue Jun 27 16:23:18 2023, max compression
```

## Comparing `helios-opentelemetry-sdk-1.0.94.tar` & `helios-opentelemetry-sdk-1.0.95.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.823553 helios-opentelemetry-sdk-1.0.94/helios/
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.823553 helios-opentelemetry-sdk-1.0.94/helios/aiosmtplib_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/aiosmtplib_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.823553 helios-opentelemetry-sdk-1.0.94/helios/aiosmtplib_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/aiosmtplib_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.823553 helios-opentelemetry-sdk-1.0.94/helios/aiosmtplib_instrumentation/src/aiosmtplib/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/aiosmtplib_instrumentation/src/aiosmtplib/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.823553 helios-opentelemetry-sdk-1.0.94/helios/base/
--rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.823553 helios-opentelemetry-sdk-1.0.94/helios/base/data_obfuscator/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/data_obfuscator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/data_obfuscator/base_data_obfuscator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/data_obfuscator/redis_data_obfuscator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.823553 helios-opentelemetry-sdk-1.0.94/helios/base/span_attribute_dropper/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/span_attribute_dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/span_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.823553 helios-opentelemetry-sdk-1.0.94/helios/base/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.827553 helios-opentelemetry-sdk-1.0.94/helios/base/tracing/export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/tracing/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/tracing/export/conditional_span_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/tracing/export/fork_process_otlp_span_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/tracing/export/hooked_batch_span_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/tracing/export/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/tracing/suppress_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/helios.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/helios_test_trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.827553 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/aio_pika.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/aiosmtplib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/aws_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/base_http_instrumentor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.827553 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/ses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/sqs_message_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/confluent_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/helios_asgi_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/httpx.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/pika.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/psycopg2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/pyspark.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/raven.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/starlette.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/tornado.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/urllib3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.827553 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.827553 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.827553 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/src/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/src/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/src/kafka/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.827553 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/tests/test_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/src/pyspark/
--rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/src/pyspark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/src/pyspark/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/tests/test_pyspark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/raven/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/raven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/raven/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/sentry/
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/sentry/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-26 05:08:34.000000 helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-26 05:08:34.000000 helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 05:08:34.000000 helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-26 05:08:34.000000 helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-26 05:08:34.000000 helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 05:08:34.000000 helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/hstest/
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/hstest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/hstest/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.182585 helios-opentelemetry-sdk-1.0.95/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-27 16:23:18.182585 helios-opentelemetry-sdk-1.0.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.170584 helios-opentelemetry-sdk-1.0.95/helios/
+-rw-r--r--   0 runner    (1001) docker     (123)    13709 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.170584 helios-opentelemetry-sdk-1.0.95/helios/aiosmtplib_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/aiosmtplib_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.170584 helios-opentelemetry-sdk-1.0.95/helios/aiosmtplib_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/aiosmtplib_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.170584 helios-opentelemetry-sdk-1.0.95/helios/aiosmtplib_instrumentation/src/aiosmtplib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/aiosmtplib_instrumentation/src/aiosmtplib/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.170584 helios-opentelemetry-sdk-1.0.95/helios/base/
+-rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.174584 helios-opentelemetry-sdk-1.0.95/helios/base/data_obfuscator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/base/data_obfuscator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/base/data_obfuscator/base_data_obfuscator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/base/data_obfuscator/redis_data_obfuscator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.174584 helios-opentelemetry-sdk-1.0.95/helios/base/span_attribute_dropper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/base/span_attribute_dropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/base/span_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.174584 helios-opentelemetry-sdk-1.0.95/helios/base/tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/base/tracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.174584 helios-opentelemetry-sdk-1.0.95/helios/base/tracing/export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/base/tracing/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/base/tracing/export/conditional_span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/base/tracing/export/fork_process_otlp_span_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/base/tracing/export/hooked_batch_span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/base/tracing/export/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/base/tracing/suppress_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/helios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/helios_test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.178585 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/aio_pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/aiosmtplib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/aws_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/base_http_instrumentor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.178585 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/botocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/botocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/botocore/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/botocore/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/botocore/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/botocore/ses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/botocore/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/botocore/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/botocore/sqs_message_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/botocore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/confluent_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/helios_asgi_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/psycopg2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/raven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/starlette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/urllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/instrumentation/urllib3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.178585 helios-opentelemetry-sdk-1.0.95/helios/kafka_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/kafka_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.178585 helios-opentelemetry-sdk-1.0.95/helios/kafka_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/kafka_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.178585 helios-opentelemetry-sdk-1.0.95/helios/kafka_instrumentation/src/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/kafka_instrumentation/src/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/kafka_instrumentation/src/kafka/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.178585 helios-opentelemetry-sdk-1.0.95/helios/kafka_instrumentation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/kafka_instrumentation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/kafka_instrumentation/tests/test_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.178585 helios-opentelemetry-sdk-1.0.95/helios/pyspark_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/pyspark_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.178585 helios-opentelemetry-sdk-1.0.95/helios/pyspark_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/pyspark_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.178585 helios-opentelemetry-sdk-1.0.95/helios/pyspark_instrumentation/src/pyspark/
+-rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/pyspark_instrumentation/src/pyspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/pyspark_instrumentation/src/pyspark/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.178585 helios-opentelemetry-sdk-1.0.95/helios/pyspark_instrumentation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/pyspark_instrumentation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/pyspark_instrumentation/tests/test_pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.178585 helios-opentelemetry-sdk-1.0.95/helios/sentry_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/sentry_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.178585 helios-opentelemetry-sdk-1.0.95/helios/sentry_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/sentry_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.178585 helios-opentelemetry-sdk-1.0.95/helios/sentry_instrumentation/src/raven/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/sentry_instrumentation/src/raven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/sentry_instrumentation/src/raven/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.178585 helios-opentelemetry-sdk-1.0.95/helios/sentry_instrumentation/src/sentry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/sentry_instrumentation/src/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/sentry_instrumentation/src/sentry/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.178585 helios-opentelemetry-sdk-1.0.95/helios/sentry_instrumentation/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/sentry_instrumentation/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/helios/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.178585 helios-opentelemetry-sdk-1.0.95/helios_opentelemetry_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-27 16:23:18.000000 helios-opentelemetry-sdk-1.0.95/helios_opentelemetry_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-27 16:23:18.000000 helios-opentelemetry-sdk-1.0.95/helios_opentelemetry_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 16:23:18.000000 helios-opentelemetry-sdk-1.0.95/helios_opentelemetry_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 16:23:18.000000 helios-opentelemetry-sdk-1.0.95/helios_opentelemetry_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-27 16:23:18.000000 helios-opentelemetry-sdk-1.0.95/helios_opentelemetry_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 16:23:18.000000 helios-opentelemetry-sdk-1.0.95/helios_opentelemetry_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:23:18.182585 helios-opentelemetry-sdk-1.0.95/hstest/
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/hstest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/hstest/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-27 16:23:18.182585 helios-opentelemetry-sdk-1.0.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-27 16:22:59.000000 helios-opentelemetry-sdk-1.0.95/setup.py
```

### Comparing `helios-opentelemetry-sdk-1.0.94/LICENSE` & `helios-opentelemetry-sdk-1.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/PKG-INFO` & `helios-opentelemetry-sdk-1.0.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-opentelemetry-sdk
-Version: 1.0.94
+Version: 1.0.95
 Summary: Helios OpenTelemetry SDK
 Home-page: https://docs.gethelios.dev/docs/python
 Author: Helios
 Author-email: support@gethelios.dev
 License: Apache License 2.0
 Keywords: helios,heliosphere,microservices,tracing,distributed-tracing,debugging,testing
 Classifier: Intended Audience :: Developers
```

### Comparing `helios-opentelemetry-sdk-1.0.94/README.md` & `helios-opentelemetry-sdk-1.0.95/README.md`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/__init__.py` & `helios-opentelemetry-sdk-1.0.95/helios/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -306,14 +306,15 @@
     from helios.instrumentation.aws_lambda import wrap_lambda_function
 
     helios_instance = Helios.get_instance()
     return wrap_lambda_function(original_handler, helios_instance.tracer_provider, helios_instance.meter_provider)
 
 
 def auto_instrument_lambda():
+    print('Auto-instrumenting Lambda function')
     if not Helios.has_instance():
         _LOG.error('Cannot auto-instrument Lambda before initializing Helios')
         return
 
     from helios.instrumentation.aws_lambda import extract_lambda_module_and_function, wrap_lambda_function
     wrapped_module_name, wrapped_function_name = extract_lambda_module_and_function()
     if not wrapped_module_name or not wrapped_function_name:
@@ -321,14 +322,15 @@
 
     def _instrumented_lambda_handler_call(call_wrapped, _instance, args, kwargs):
         helios_instance = Helios.get_instance()
         wrapped_function = wrap_lambda_function(call_wrapped, helios_instance.tracer_provider, helios_instance.meter_provider)
         return wrapped_function(*args, **kwargs)
 
     wrap_function_wrapper(wrapped_module_name, wrapped_function_name, _instrumented_lambda_handler_call)
+    return wrapped_module_name, wrapped_function_name
 
 
 __all__ = [
     'initialize',
     'initialize_test',
     'extract_context',
     'inject_current_context',
```

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py` & `helios-opentelemetry-sdk-1.0.95/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/base/__init__.py` & `helios-opentelemetry-sdk-1.0.95/helios/base/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/base/data_obfuscator/__init__.py` & `helios-opentelemetry-sdk-1.0.95/helios/base/data_obfuscator/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/base/data_obfuscator/base_data_obfuscator.py` & `helios-opentelemetry-sdk-1.0.95/helios/base/data_obfuscator/base_data_obfuscator.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/base/data_obfuscator/redis_data_obfuscator.py` & `helios-opentelemetry-sdk-1.0.95/helios/base/data_obfuscator/redis_data_obfuscator.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/base/span_attribute_dropper/__init__.py` & `helios-opentelemetry-sdk-1.0.95/helios/base/span_attribute_dropper/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/base/tracing/export/conditional_span_processor.py` & `helios-opentelemetry-sdk-1.0.95/helios/base/tracing/export/conditional_span_processor.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/base/tracing/export/fork_process_otlp_span_exporter.py` & `helios-opentelemetry-sdk-1.0.95/helios/base/tracing/export/fork_process_otlp_span_exporter.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/base/tracing/export/hooked_batch_span_processor.py` & `helios-opentelemetry-sdk-1.0.95/helios/base/tracing/export/hooked_batch_span_processor.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/helios.py` & `helios-opentelemetry-sdk-1.0.95/helios/helios.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/helios_test_trace.py` & `helios-opentelemetry-sdk-1.0.95/helios/helios_test_trace.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/__init__.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/aio_pika.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/aio_pika.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/aiohttp.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/aiohttp.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/aiosmtplib.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/aiosmtplib.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/aws_lambda.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/base.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/base.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/base_http_instrumentor.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/base_http_instrumentor.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/__init__.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/botocore/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/consts.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/botocore/consts.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/dynamodb.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/botocore/dynamodb.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/s3.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/botocore/s3.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/ses.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/botocore/ses.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/sns.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/botocore/sns.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/sqs.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/botocore/sqs.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/sqs_message_context.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/botocore/sqs_message_context.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/utils.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/botocore/utils.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/confluent_kafka.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/confluent_kafka.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/django.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/django.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/elasticsearch.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/fastapi.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/fastapi.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/flask.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/flask.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/grpc.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/grpc.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/helios_asgi_middleware.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/helios_asgi_middleware.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/httpx.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/httpx.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/kafka.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/kafka.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/logging.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/logging.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/pika.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/pika.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/psycopg2.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/psycopg2.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/pymongo.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/pymongo.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/pyspark.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/pyspark.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/raven.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/raven.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/redis.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/redis.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/requests.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/requests.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/sentry.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/sentry.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/starlette.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/starlette.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/tornado.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/tornado.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/urllib.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/urllib.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/urllib3.py` & `helios-opentelemetry-sdk-1.0.95/helios/instrumentation/urllib3.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/src/kafka/__init__.py` & `helios-opentelemetry-sdk-1.0.95/helios/kafka_instrumentation/src/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/tests/test_kafka.py` & `helios-opentelemetry-sdk-1.0.95/helios/kafka_instrumentation/tests/test_kafka.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/src/pyspark/__init__.py` & `helios-opentelemetry-sdk-1.0.95/helios/pyspark_instrumentation/src/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/tests/test_pyspark.py` & `helios-opentelemetry-sdk-1.0.95/helios/pyspark_instrumentation/tests/test_pyspark.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/sampler.py` & `helios-opentelemetry-sdk-1.0.95/helios/sampler.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/raven/__init__.py` & `helios-opentelemetry-sdk-1.0.95/helios/sentry_instrumentation/src/raven/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/sentry/__init__.py` & `helios-opentelemetry-sdk-1.0.95/helios/sentry_instrumentation/src/sentry/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios/utils.py` & `helios-opentelemetry-sdk-1.0.95/helios/utils.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/PKG-INFO` & `helios-opentelemetry-sdk-1.0.95/helios_opentelemetry_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-opentelemetry-sdk
-Version: 1.0.94
+Version: 1.0.95
 Summary: Helios OpenTelemetry SDK
 Home-page: https://docs.gethelios.dev/docs/python
 Author: Helios
 Author-email: support@gethelios.dev
 License: Apache License 2.0
 Keywords: helios,heliosphere,microservices,tracing,distributed-tracing,debugging,testing
 Classifier: Intended Audience :: Developers
```

### Comparing `helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/SOURCES.txt` & `helios-opentelemetry-sdk-1.0.95/helios_opentelemetry_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/requires.txt` & `helios-opentelemetry-sdk-1.0.95/helios_opentelemetry_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/hstest/__init__.py` & `helios-opentelemetry-sdk-1.0.95/hstest/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.94/setup.py` & `helios-opentelemetry-sdk-1.0.95/setup.py`

 * *Files identical despite different names*

