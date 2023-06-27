# Comparing `tmp/momento-1.6.0.tar.gz` & `tmp/momento-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momento-1.6.0.tar", max compression
+gzip compressed data, was "momento-1.6.1.tar", max compression
```

## Comparing `momento-1.6.0.tar` & `momento-1.6.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
--rw-r--r--   0        0        0    11357 2023-06-09 22:36:27.728766 momento-1.6.0/LICENSE
--rw-r--r--   0        0        0     4142 2023-06-09 22:36:27.728766 momento-1.6.0/README.md
--rw-r--r--   0        0        0     3805 2023-06-09 22:36:50.288958 momento-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      619 2023-06-09 22:36:27.728766 momento-1.6.0/src/momento/__init__.py
--rw-r--r--   0        0        0       86 2023-06-09 22:36:27.728766 momento-1.6.0/src/momento/auth/__init__.py
--rw-r--r--   0        0        0     2868 2023-06-09 22:36:27.728766 momento-1.6.0/src/momento/auth/credential_provider.py
--rw-r--r--   0        0        0     2003 2023-06-09 22:36:27.728766 momento-1.6.0/src/momento/auth/momento_endpoint_resolver.py
--rw-r--r--   0        0        0    43798 2023-06-09 22:36:27.728766 momento-1.6.0/src/momento/cache_client.py
--rw-r--r--   0        0        0    44449 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/cache_client_async.py
--rw-r--r--   0        0        0      176 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/config/__init__.py
--rw-r--r--   0        0        0     3250 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/config/configuration.py
--rw-r--r--   0        0        0     4290 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/config/configurations.py
--rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/config/transport/__init__.py
--rw-r--r--   0        0        0      314 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/config/transport/grpc_configuration.py
--rw-r--r--   0        0        0     2358 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/config/transport/transport_strategy.py
--rw-r--r--   0        0        0     1503 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/errors/__init__.py
--rw-r--r--   0        0        0     3991 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/errors/error_converter.py
--rw-r--r--   0        0        0     2329 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/errors/error_details.py
--rw-r--r--   0        0        0     8799 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/errors/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/__init__.py
--rw-r--r--   0        0        0      406 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/_utilities/__init__.py
--rw-r--r--   0        0        0     4735 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/_utilities/_data_validation.py
--rw-r--r--   0        0        0      531 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/_utilities/_momento_version.py
--rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/aio/__init__.py
--rw-r--r--   0        0        0     4377 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/aio/_add_header_client_interceptor.py
--rw-r--r--   0        0        0     1856 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/aio/_retry_interceptor.py
--rw-r--r--   0        0        0     5794 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/aio/_scs_control_client.py
--rw-r--r--   0        0        0    47789 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/aio/_scs_data_client.py
--rw-r--r--   0        0        0     3206 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/aio/_scs_grpc_manager.py
--rw-r--r--   0        0        0      123 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/aio/_utilities.py
--rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/synchronous/__init__.py
--rw-r--r--   0        0        0     3714 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/synchronous/_add_header_client_interceptor.py
--rw-r--r--   0        0        0     1829 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/synchronous/_retry_interceptor.py
--rw-r--r--   0        0        0     5700 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/synchronous/_scs_control_client.py
--rw-r--r--   0        0        0    47409 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/synchronous/_scs_data_client.py
--rw-r--r--   0        0        0     2436 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/synchronous/_scs_grpc_manager.py
--rw-r--r--   0        0        0      159 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/synchronous/_utilities.py
--rw-r--r--   0        0        0     2790 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/logs.py
--rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/py.typed
--rw-r--r--   0        0        0      154 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/requests/__init__.py
--rw-r--r--   0        0        0     3800 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/requests/collection_ttl.py
--rw-r--r--   0        0        0       91 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/requests/sort_order.py
--rw-r--r--   0        0        0     6841 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/cache/__init__.py
--rw-r--r--   0        0        0     1758 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/cache/create.py
--rw-r--r--   0        0        0     1405 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/cache/delete.py
--rw-r--r--   0        0        0      849 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/cache/flush.py
--rw-r--r--   0        0        0     2275 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/cache/list.py
--rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/signing_key/__init__.py
--rw-r--r--   0        0        0     1764 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/signing_key/create.py
--rw-r--r--   0        0        0     2479 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/signing_key/list.py
--rw-r--r--   0        0        0      979 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/signing_key/revoke.py
--rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/dictionary/__init__.py
--rw-r--r--   0        0        0     2047 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/dictionary/fetch.py
--rw-r--r--   0        0        0     1678 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/dictionary/get_field.py
--rw-r--r--   0        0        0     3320 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/dictionary/get_fields.py
--rw-r--r--   0        0        0     1050 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/dictionary/increment.py
--rw-r--r--   0        0        0      945 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/dictionary/remove_field.py
--rw-r--r--   0        0        0      953 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/dictionary/remove_fields.py
--rw-r--r--   0        0        0      921 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/dictionary/set_field.py
--rw-r--r--   0        0        0      929 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/dictionary/set_fields.py
--rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/list/__init__.py
--rw-r--r--   0        0        0     1052 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/list/concatenate_back.py
--rw-r--r--   0        0        0     1060 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/list/concatenate_front.py
--rw-r--r--   0        0        0     1402 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/list/fetch.py
--rw-r--r--   0        0        0     1070 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/list/length.py
--rw-r--r--   0        0        0     1189 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/list/pop_back.py
--rw-r--r--   0        0        0     1199 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/list/pop_front.py
--rw-r--r--   0        0        0      977 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/list/push_back.py
--rw-r--r--   0        0        0      985 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/list/push_front.py
--rw-r--r--   0        0        0      874 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/list/remove_value.py
--rw-r--r--   0        0        0        0 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/scalar/__init__.py
--rw-r--r--   0        0        0      823 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/scalar/delete.py
--rw-r--r--   0        0        0     1155 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/scalar/get.py
--rw-r--r--   0        0        0     1141 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/scalar/increment.py
--rw-r--r--   0        0        0      799 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/scalar/set.py
--rw-r--r--   0        0        0     1056 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/scalar/set_if_not_exists.py
--rw-r--r--   0        0        0        0 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/set/__init__.py
--rw-r--r--   0        0        0      870 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/set/add_element.py
--rw-r--r--   0        0        0      880 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/set/add_elements.py
--rw-r--r--   0        0        0     1452 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/set/fetch.py
--rw-r--r--   0        0        0      896 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/set/remove_element.py
--rw-r--r--   0        0        0      906 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/set/remove_elements.py
--rw-r--r--   0        0        0        0 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/__init__.py
--rw-r--r--   0        0        0     1616 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/fetch.py
--rw-r--r--   0        0        0     1205 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/get_rank.py
--rw-r--r--   0        0        0     1581 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/get_score.py
--rw-r--r--   0        0        0     2323 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/get_scores.py
--rw-r--r--   0        0        0     1087 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/increment_score.py
--rw-r--r--   0        0        0      944 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/put_element.py
--rw-r--r--   0        0        0      952 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/put_elements.py
--rw-r--r--   0        0        0      971 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/remove_element.py
--rw-r--r--   0        0        0      979 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/remove_elements.py
--rw-r--r--   0        0        0     1460 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/mixins.py
--rw-r--r--   0        0        0     4724 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/response.py
--rw-r--r--   0        0        0      423 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/retry/__init__.py
--rw-r--r--   0        0        0     2900 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/retry/default_eligibility_strategy.py
--rw-r--r--   0        0        0      216 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/retry/eligibility_strategy.py
--rw-r--r--   0        0        0     2181 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/retry/fixed_count_retry_strategy.py
--rw-r--r--   0        0        0      251 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/retry/retry_strategy.py
--rw-r--r--   0        0        0      291 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/retry/retryable_props.py
--rw-r--r--   0        0        0     1722 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/typing.py
--rw-r--r--   0        0        0     5650 1970-01-01 00:00:00.000000 momento-1.6.0/setup.py
--rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 momento-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-27 19:56:11.222096 momento-1.6.1/LICENSE
+-rw-r--r--   0        0        0     4282 2023-06-27 19:56:11.222096 momento-1.6.1/README.md
+-rw-r--r--   0        0        0     3805 2023-06-27 19:56:31.462333 momento-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0      619 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/__init__.py
+-rw-r--r--   0        0        0       86 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/auth/__init__.py
+-rw-r--r--   0        0        0     2868 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/auth/credential_provider.py
+-rw-r--r--   0        0        0     2003 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/auth/momento_endpoint_resolver.py
+-rw-r--r--   0        0        0    43798 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/cache_client.py
+-rw-r--r--   0        0        0    44449 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/cache_client_async.py
+-rw-r--r--   0        0        0      176 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/config/__init__.py
+-rw-r--r--   0        0        0     3250 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/config/configuration.py
+-rw-r--r--   0        0        0     4290 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/config/configurations.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/config/transport/__init__.py
+-rw-r--r--   0        0        0      314 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/config/transport/grpc_configuration.py
+-rw-r--r--   0        0        0     2358 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/config/transport/transport_strategy.py
+-rw-r--r--   0        0        0     1503 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/errors/__init__.py
+-rw-r--r--   0        0        0     3991 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/errors/error_converter.py
+-rw-r--r--   0        0        0     2329 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/errors/error_details.py
+-rw-r--r--   0        0        0     8799 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/errors/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/__init__.py
+-rw-r--r--   0        0        0      406 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/_utilities/__init__.py
+-rw-r--r--   0        0        0     4735 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/_utilities/_data_validation.py
+-rw-r--r--   0        0        0      531 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/_utilities/_momento_version.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/aio/__init__.py
+-rw-r--r--   0        0        0     4377 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/aio/_add_header_client_interceptor.py
+-rw-r--r--   0        0        0     1856 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/aio/_retry_interceptor.py
+-rw-r--r--   0        0        0     5794 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/aio/_scs_control_client.py
+-rw-r--r--   0        0        0    47792 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/aio/_scs_data_client.py
+-rw-r--r--   0        0        0     3206 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/aio/_scs_grpc_manager.py
+-rw-r--r--   0        0        0      123 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/aio/_utilities.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:56:11.222096 momento-1.6.1/src/momento/internal/synchronous/__init__.py
+-rw-r--r--   0        0        0     3714 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/internal/synchronous/_add_header_client_interceptor.py
+-rw-r--r--   0        0        0     1829 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/internal/synchronous/_retry_interceptor.py
+-rw-r--r--   0        0        0     5700 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/internal/synchronous/_scs_control_client.py
+-rw-r--r--   0        0        0    47412 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/internal/synchronous/_scs_data_client.py
+-rw-r--r--   0        0        0     2436 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/internal/synchronous/_scs_grpc_manager.py
+-rw-r--r--   0        0        0      159 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/internal/synchronous/_utilities.py
+-rw-r--r--   0        0        0     2790 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/logs.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/py.typed
+-rw-r--r--   0        0        0      154 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/requests/__init__.py
+-rw-r--r--   0        0        0     3800 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/requests/collection_ttl.py
+-rw-r--r--   0        0        0       91 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/requests/sort_order.py
+-rw-r--r--   0        0        0     6841 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/cache/__init__.py
+-rw-r--r--   0        0        0     1758 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/cache/create.py
+-rw-r--r--   0        0        0     1405 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/cache/delete.py
+-rw-r--r--   0        0        0      849 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/cache/flush.py
+-rw-r--r--   0        0        0     2275 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/cache/list.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/signing_key/__init__.py
+-rw-r--r--   0        0        0     1764 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/signing_key/create.py
+-rw-r--r--   0        0        0     2479 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/signing_key/list.py
+-rw-r--r--   0        0        0      979 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/control/signing_key/revoke.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/dictionary/__init__.py
+-rw-r--r--   0        0        0     2047 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/dictionary/fetch.py
+-rw-r--r--   0        0        0     1678 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/dictionary/get_field.py
+-rw-r--r--   0        0        0     3320 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/dictionary/get_fields.py
+-rw-r--r--   0        0        0     1050 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/dictionary/increment.py
+-rw-r--r--   0        0        0      945 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/dictionary/remove_field.py
+-rw-r--r--   0        0        0      953 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/dictionary/remove_fields.py
+-rw-r--r--   0        0        0      921 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/dictionary/set_field.py
+-rw-r--r--   0        0        0      929 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/dictionary/set_fields.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/__init__.py
+-rw-r--r--   0        0        0     1052 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/concatenate_back.py
+-rw-r--r--   0        0        0     1060 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/concatenate_front.py
+-rw-r--r--   0        0        0     1402 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/fetch.py
+-rw-r--r--   0        0        0     1070 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/length.py
+-rw-r--r--   0        0        0     1189 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/pop_back.py
+-rw-r--r--   0        0        0     1199 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/pop_front.py
+-rw-r--r--   0        0        0      977 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/push_back.py
+-rw-r--r--   0        0        0      985 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/push_front.py
+-rw-r--r--   0        0        0      874 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/list/remove_value.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/scalar/__init__.py
+-rw-r--r--   0        0        0      823 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/scalar/delete.py
+-rw-r--r--   0        0        0     1155 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/scalar/get.py
+-rw-r--r--   0        0        0     1141 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/scalar/increment.py
+-rw-r--r--   0        0        0      799 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/scalar/set.py
+-rw-r--r--   0        0        0     1056 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/scalar/set_if_not_exists.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/set/__init__.py
+-rw-r--r--   0        0        0      870 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/set/add_element.py
+-rw-r--r--   0        0        0      880 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/set/add_elements.py
+-rw-r--r--   0        0        0     1452 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/set/fetch.py
+-rw-r--r--   0        0        0      896 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/set/remove_element.py
+-rw-r--r--   0        0        0      906 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/set/remove_elements.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/__init__.py
+-rw-r--r--   0        0        0     1616 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/fetch.py
+-rw-r--r--   0        0        0     1205 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/get_rank.py
+-rw-r--r--   0        0        0     1581 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/get_score.py
+-rw-r--r--   0        0        0     2323 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/get_scores.py
+-rw-r--r--   0        0        0     1087 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/increment_score.py
+-rw-r--r--   0        0        0      944 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/put_element.py
+-rw-r--r--   0        0        0      952 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/put_elements.py
+-rw-r--r--   0        0        0      971 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/remove_element.py
+-rw-r--r--   0        0        0      979 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/data/sorted_set/remove_elements.py
+-rw-r--r--   0        0        0     1460 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/mixins.py
+-rw-r--r--   0        0        0     4724 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/responses/response.py
+-rw-r--r--   0        0        0      423 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/retry/__init__.py
+-rw-r--r--   0        0        0     2900 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/retry/default_eligibility_strategy.py
+-rw-r--r--   0        0        0      216 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/retry/eligibility_strategy.py
+-rw-r--r--   0        0        0     2181 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/retry/fixed_count_retry_strategy.py
+-rw-r--r--   0        0        0      251 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/retry/retry_strategy.py
+-rw-r--r--   0        0        0      291 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/retry/retryable_props.py
+-rw-r--r--   0        0        0     1722 2023-06-27 19:56:11.226096 momento-1.6.1/src/momento/typing.py
+-rw-r--r--   0        0        0     5792 1970-01-01 00:00:00.000000 momento-1.6.1/setup.py
+-rw-r--r--   0        0        0     5580 1970-01-01 00:00:00.000000 momento-1.6.1/PKG-INFO
```

### Comparing `momento-1.6.0/LICENSE` & `momento-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/README.md` & `momento-1.6.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 [![project stability](https://momentohq.github.io/standards-and-practices/badges/project-stability-stable.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md)
 
 # Momento Python Client Library
 
 Momento Cache is a fast, simple, pay-as-you-go caching solution without any of the operational overhead
 required by traditional caching solutions.  This repo contains the source code for the Momento Python client library.
 
+To get started with Momento you will need a Momento Auth Token. You can get one from the [Momento Console](https://console.gomomento.com).
+
 * Website: [https://www.gomomento.com/](https://www.gomomento.com/)
 * Momento Documentation: [https://docs.momentohq.com/](https://docs.momentohq.com/)
 * Getting Started: [https://docs.momentohq.com/getting-started](https://docs.momentohq.com/getting-started)
 * Python SDK Documentation: [https://docs.momentohq.com/develop/sdks/python](https://docs.momentohq.com/develop/sdks/python)
 * Discuss: [Momento Discord](https://discord.gg/3HkAKjUZGq)
 
 ## Packages
```

### Comparing `momento-1.6.0/pyproject.toml` & `momento-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "momento"
-version = "1.6.0"
+version = "1.6.1"
 
 authors = ["Momento <hello@momentohq.com>"]
 description = "SDK for Momento"
 
 license = "Apache-2.0"
 
 documentation = "https://docs.momentohq.com/"
```

### Comparing `momento-1.6.0/src/momento/__init__.py` & `momento-1.6.1/src/momento/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/auth/credential_provider.py` & `momento-1.6.1/src/momento/auth/credential_provider.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/auth/momento_endpoint_resolver.py` & `momento-1.6.1/src/momento/auth/momento_endpoint_resolver.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/cache_client.py` & `momento-1.6.1/src/momento/cache_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/cache_client_async.py` & `momento-1.6.1/src/momento/cache_client_async.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/config/configuration.py` & `momento-1.6.1/src/momento/config/configuration.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/config/configurations.py` & `momento-1.6.1/src/momento/config/configurations.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/config/transport/transport_strategy.py` & `momento-1.6.1/src/momento/config/transport/transport_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/errors/__init__.py` & `momento-1.6.1/src/momento/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/errors/error_converter.py` & `momento-1.6.1/src/momento/errors/error_converter.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/errors/error_details.py` & `momento-1.6.1/src/momento/errors/error_details.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/errors/exceptions.py` & `momento-1.6.1/src/momento/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/internal/_utilities/_data_validation.py` & `momento-1.6.1/src/momento/internal/_utilities/_data_validation.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/internal/_utilities/_momento_version.py` & `momento-1.6.1/src/momento/internal/_utilities/_momento_version.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/internal/aio/_add_header_client_interceptor.py` & `momento-1.6.1/src/momento/internal/aio/_add_header_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/internal/aio/_retry_interceptor.py` & `momento-1.6.1/src/momento/internal/aio/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/internal/aio/_scs_control_client.py` & `momento-1.6.1/src/momento/internal/aio/_scs_control_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/internal/aio/_scs_data_client.py` & `momento-1.6.1/src/momento/internal/aio/_scs_data_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
             if response.result == cache_pb.Hit:
                 return CacheGet.Hit(response.cache_body)
             elif response.result == cache_pb.Miss:
                 return CacheGet.Miss()
             else:
                 raise UnknownException("Get responded with an unknown result")
         except Exception as e:
-            self._log_request_error("set_if_not_exists", e)
+            self._log_request_error("get", e)
             return CacheGet.Error(convert_error(e))
 
     async def delete(self, cache_name: str, key: TScalarKey) -> CacheDeleteResponse:
         try:
             self._log_issuing_request("Delete", {"key": str(key)})
             _validate_cache_name(cache_name)
             request = cache_pb._DeleteRequest(cache_key=_as_bytes(key, "Unsupported type for key: "))
@@ -279,15 +279,15 @@
             await self._build_stub().Delete(
                 request, metadata=make_metadata(cache_name), timeout=self._default_deadline_seconds
             )
 
             self._log_received_response("Delete", {"key": str(key)})
             return CacheDelete.Success()
         except Exception as e:
-            self._log_request_error("set", e)
+            self._log_request_error("delete", e)
             return CacheDelete.Error(convert_error(e))
 
     # DICTIONARY COLLECTION METHODS
     async def dictionary_get_fields(
         self,
         cache_name: TCacheName,
         dictionary_name: TDictionaryName,
@@ -725,15 +725,15 @@
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SetAddElements", {"set_name": str(request.set_name)})
             return CacheSetAddElements.Success()
         except Exception as e:
-            self._log_request_error("set_remove_elements", e)
+            self._log_request_error("set_add_elements", e)
             return CacheSetAddElements.Error(convert_error(e))
 
     async def set_fetch(
         self,
         cache_name: TCacheName,
         set_name: TSetName,
     ) -> CacheSetFetchResponse:
@@ -879,15 +879,15 @@
             elif type == "found":
                 return CacheSortedSetFetch.Hit(
                     list((e.value, e.score) for e in response.found.values_with_scores.elements)
                 )
             else:
                 raise UnknownException(f"Unknown set field in response: {type}")
         except Exception as e:
-            self._log_request_error("sorted_set_fetch", e)
+            self._log_request_error("sorted_set_fetch_by_score", e)
             return CacheSortedSetFetch.Error(convert_error(e))
 
     async def sorted_set_fetch_by_rank(
         self,
         cache_name: TCacheName,
         sorted_set_name: TSortedSetName,
         start_rank: Optional[int],
@@ -931,15 +931,15 @@
             elif type == "found":
                 return CacheSortedSetFetch.Hit(
                     list((e.value, e.score) for e in response.found.values_with_scores.elements)
                 )
             else:
                 raise UnknownException(f"Unknown set field in response: {type}")
         except Exception as e:
-            self._log_request_error("sorted_set_fetch", e)
+            self._log_request_error("sorted_set_fetch_by_rank", e)
             return CacheSortedSetFetch.Error(convert_error(e))
 
     async def sorted_set_get_scores(
         self, cache_name: TCacheName, sorted_set_name: TSortedSetName, values: TSortedSetValues
     ) -> CacheSortedSetGetScoresResponse:
         try:
             self._log_issuing_request("SortedSetGetScores", {"sorted_set_name": str(sorted_set_name)})
```

### Comparing `momento-1.6.0/src/momento/internal/aio/_scs_grpc_manager.py` & `momento-1.6.1/src/momento/internal/aio/_scs_grpc_manager.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/internal/synchronous/_add_header_client_interceptor.py` & `momento-1.6.1/src/momento/internal/synchronous/_add_header_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/internal/synchronous/_retry_interceptor.py` & `momento-1.6.1/src/momento/internal/synchronous/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/internal/synchronous/_scs_control_client.py` & `momento-1.6.1/src/momento/internal/synchronous/_scs_control_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/internal/synchronous/_scs_data_client.py` & `momento-1.6.1/src/momento/internal/synchronous/_scs_data_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
             if response.result == cache_pb.Hit:
                 return CacheGet.Hit(response.cache_body)
             elif response.result == cache_pb.Miss:
                 return CacheGet.Miss()
             else:
                 raise UnknownException("Get responded with an unknown result")
         except Exception as e:
-            self._log_request_error("set_if_not_exists", e)
+            self._log_request_error("get", e)
             return CacheGet.Error(convert_error(e))
 
     def delete(self, cache_name: str, key: TScalarKey) -> CacheDeleteResponse:
         try:
             self._log_issuing_request("Delete", {"key": str(key)})
             _validate_cache_name(cache_name)
             request = cache_pb._DeleteRequest(cache_key=_as_bytes(key, "Unsupported type for key: "))
@@ -277,15 +277,15 @@
             self._build_stub().Delete(
                 request, metadata=make_metadata(cache_name), timeout=self._default_deadline_seconds
             )
 
             self._log_received_response("Delete", {"key": str(key)})
             return CacheDelete.Success()
         except Exception as e:
-            self._log_request_error("set", e)
+            self._log_request_error("delete", e)
             return CacheDelete.Error(convert_error(e))
 
     # DICTIONARY COLLECTION METHODS
     def dictionary_get_fields(
         self,
         cache_name: TCacheName,
         dictionary_name: TDictionaryName,
@@ -723,15 +723,15 @@
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SetAddElements", {"set_name": str(request.set_name)})
             return CacheSetAddElements.Success()
         except Exception as e:
-            self._log_request_error("set_remove_elements", e)
+            self._log_request_error("set_add_elements", e)
             return CacheSetAddElements.Error(convert_error(e))
 
     def set_fetch(
         self,
         cache_name: TCacheName,
         set_name: TSetName,
     ) -> CacheSetFetchResponse:
@@ -877,15 +877,15 @@
             elif type == "found":
                 return CacheSortedSetFetch.Hit(
                     list((e.value, e.score) for e in response.found.values_with_scores.elements)
                 )
             else:
                 raise UnknownException(f"Unknown set field in response: {type}")
         except Exception as e:
-            self._log_request_error("sorted_set_fetch", e)
+            self._log_request_error("sorted_set_fetch_by_score", e)
             return CacheSortedSetFetch.Error(convert_error(e))
 
     def sorted_set_fetch_by_rank(
         self,
         cache_name: TCacheName,
         sorted_set_name: TSortedSetName,
         start_rank: Optional[int],
@@ -929,15 +929,15 @@
             elif type == "found":
                 return CacheSortedSetFetch.Hit(
                     list((e.value, e.score) for e in response.found.values_with_scores.elements)
                 )
             else:
                 raise UnknownException(f"Unknown set field in response: {type}")
         except Exception as e:
-            self._log_request_error("sorted_set_fetch", e)
+            self._log_request_error("sorted_set_fetch_by_rank", e)
             return CacheSortedSetFetch.Error(convert_error(e))
 
     def sorted_set_get_scores(
         self, cache_name: TCacheName, sorted_set_name: TSortedSetName, values: TSortedSetValues
     ) -> CacheSortedSetGetScoresResponse:
         try:
             self._log_issuing_request("SortedSetGetScores", {"sorted_set_name": str(sorted_set_name)})
```

### Comparing `momento-1.6.0/src/momento/internal/synchronous/_scs_grpc_manager.py` & `momento-1.6.1/src/momento/internal/synchronous/_scs_grpc_manager.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/logs.py` & `momento-1.6.1/src/momento/logs.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/requests/collection_ttl.py` & `momento-1.6.1/src/momento/requests/collection_ttl.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/__init__.py` & `momento-1.6.1/src/momento/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/control/cache/create.py` & `momento-1.6.1/src/momento/responses/control/cache/create.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/control/cache/delete.py` & `momento-1.6.1/src/momento/responses/control/cache/delete.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/control/cache/flush.py` & `momento-1.6.1/src/momento/responses/control/cache/flush.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/control/cache/list.py` & `momento-1.6.1/src/momento/responses/control/cache/list.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/control/signing_key/create.py` & `momento-1.6.1/src/momento/responses/control/signing_key/create.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/control/signing_key/list.py` & `momento-1.6.1/src/momento/responses/control/signing_key/list.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/control/signing_key/revoke.py` & `momento-1.6.1/src/momento/responses/control/signing_key/revoke.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/dictionary/fetch.py` & `momento-1.6.1/src/momento/responses/data/dictionary/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/dictionary/get_field.py` & `momento-1.6.1/src/momento/responses/data/dictionary/get_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/dictionary/get_fields.py` & `momento-1.6.1/src/momento/responses/data/dictionary/get_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/dictionary/increment.py` & `momento-1.6.1/src/momento/responses/data/dictionary/increment.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/dictionary/remove_field.py` & `momento-1.6.1/src/momento/responses/data/dictionary/remove_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/dictionary/remove_fields.py` & `momento-1.6.1/src/momento/responses/data/dictionary/remove_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/dictionary/set_field.py` & `momento-1.6.1/src/momento/responses/data/dictionary/set_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/dictionary/set_fields.py` & `momento-1.6.1/src/momento/responses/data/dictionary/set_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/list/concatenate_back.py` & `momento-1.6.1/src/momento/responses/data/list/concatenate_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/list/concatenate_front.py` & `momento-1.6.1/src/momento/responses/data/list/concatenate_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/list/fetch.py` & `momento-1.6.1/src/momento/responses/data/list/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/list/length.py` & `momento-1.6.1/src/momento/responses/data/list/length.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/list/pop_back.py` & `momento-1.6.1/src/momento/responses/data/list/pop_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/list/pop_front.py` & `momento-1.6.1/src/momento/responses/data/list/pop_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/list/push_back.py` & `momento-1.6.1/src/momento/responses/data/list/push_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/list/push_front.py` & `momento-1.6.1/src/momento/responses/data/list/push_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/list/remove_value.py` & `momento-1.6.1/src/momento/responses/data/list/remove_value.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/scalar/delete.py` & `momento-1.6.1/src/momento/responses/data/scalar/delete.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/scalar/get.py` & `momento-1.6.1/src/momento/responses/data/scalar/get.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/scalar/increment.py` & `momento-1.6.1/src/momento/responses/data/scalar/increment.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/scalar/set.py` & `momento-1.6.1/src/momento/responses/data/scalar/set.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/scalar/set_if_not_exists.py` & `momento-1.6.1/src/momento/responses/data/scalar/set_if_not_exists.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/set/add_element.py` & `momento-1.6.1/src/momento/responses/data/set/add_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/set/add_elements.py` & `momento-1.6.1/src/momento/responses/data/set/add_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/set/fetch.py` & `momento-1.6.1/src/momento/responses/data/set/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/set/remove_element.py` & `momento-1.6.1/src/momento/responses/data/set/remove_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/set/remove_elements.py` & `momento-1.6.1/src/momento/responses/data/set/remove_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/sorted_set/fetch.py` & `momento-1.6.1/src/momento/responses/data/sorted_set/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/sorted_set/get_rank.py` & `momento-1.6.1/src/momento/responses/data/sorted_set/get_rank.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/sorted_set/get_score.py` & `momento-1.6.1/src/momento/responses/data/sorted_set/get_score.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/sorted_set/get_scores.py` & `momento-1.6.1/src/momento/responses/data/sorted_set/get_scores.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/sorted_set/increment_score.py` & `momento-1.6.1/src/momento/responses/data/sorted_set/increment_score.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/sorted_set/put_element.py` & `momento-1.6.1/src/momento/responses/data/sorted_set/put_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/sorted_set/put_elements.py` & `momento-1.6.1/src/momento/responses/data/sorted_set/put_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/sorted_set/remove_element.py` & `momento-1.6.1/src/momento/responses/data/sorted_set/remove_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/data/sorted_set/remove_elements.py` & `momento-1.6.1/src/momento/responses/data/sorted_set/remove_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/mixins.py` & `momento-1.6.1/src/momento/responses/mixins.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/responses/response.py` & `momento-1.6.1/src/momento/responses/response.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/retry/default_eligibility_strategy.py` & `momento-1.6.1/src/momento/retry/default_eligibility_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/retry/fixed_count_retry_strategy.py` & `momento-1.6.1/src/momento/retry/fixed_count_retry_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/src/momento/typing.py` & `momento-1.6.1/src/momento/typing.py`

 * *Files identical despite different names*

### Comparing `momento-1.6.0/setup.py` & `momento-1.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,17 @@
  'pyjwt>=2.4.0,<3.0.0']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib-metadata>=4']}
 
 setup_kwargs = {
     'name': 'momento',
-    'version': '1.6.0',
+    'version': '1.6.1',
     'description': 'SDK for Momento',
-    'long_description': '<head>\n  <meta name="Momento Python Client Library Documentation" content="Python client software development kit for Momento Cache">\n</head>\n<img src="https://docs.momentohq.com/img/logo.svg" alt="logo" width="400"/>\n\n[![project status](https://momentohq.github.io/standards-and-practices/badges/project-status-official.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md)\n[![project stability](https://momentohq.github.io/standards-and-practices/badges/project-stability-stable.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md)\n\n# Momento Python Client Library\n\nMomento Cache is a fast, simple, pay-as-you-go caching solution without any of the operational overhead\nrequired by traditional caching solutions.  This repo contains the source code for the Momento Python client library.\n\n* Website: [https://www.gomomento.com/](https://www.gomomento.com/)\n* Momento Documentation: [https://docs.momentohq.com/](https://docs.momentohq.com/)\n* Getting Started: [https://docs.momentohq.com/getting-started](https://docs.momentohq.com/getting-started)\n* Python SDK Documentation: [https://docs.momentohq.com/develop/sdks/python](https://docs.momentohq.com/develop/sdks/python)\n* Discuss: [Momento Discord](https://discord.gg/3HkAKjUZGq)\n\n## Packages\n\nThe Momento Python SDK package is available on pypi: [momento](https://pypi.org/project/momento/).\n\n## Usage\n\nThe examples below require an environment variable named MOMENTO_AUTH_TOKEN which must\nbe set to a valid [Momento authentication token](https://docs.momentohq.com/docs/getting-started#obtain-an-auth-token).\n\nPython 3.10 introduced the `match` statement, which allows for [structural pattern matching on objects](https://peps.python.org/pep-0636/#adding-a-ui-matching-objects).\nIf you are running python 3.10 or greater, here is a quickstart you can use in your own project:\n\n```python\nfrom datetime import timedelta\n\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache, ListCaches\n\ncache_client = CacheClient(\n    Configurations.Laptop.v1(),\n    CredentialProvider.from_environment_variable("MOMENTO_AUTH_TOKEN"),\n    timedelta(seconds=60)\n)\n\ncreate_cache_response = cache_client.create_cache("cache")\nset_response = cache_client.set("cache", "my-key", "my-value")\nget_response = cache_client.get(_CACHE_NAME, _KEY)\nmatch get_response:\n    case CacheGet.Hit() as hit:\n        print(f"Got value: {hit.value_string}")\n    case _:\n        print(f"Response was not a hit: {get_response}")\n\n```\n\nThe above code uses [structural pattern matching](https://peps.python.org/pep-0636/), a feature introduced in Python 3.10.\nUsing a Python version less than 3.10? No problem. Here is the same example compatible across all versions of Python:\n\n```python\nfrom datetime import timedelta\n\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache\n\ncache_client = CacheClient(\n    configuration=Configurations.Laptop.v1(),\n    credential_provider=CredentialProvider.from_environment_variable(\'MOMENTO_AUTH_TOKEN\'),\n    default_ttl=timedelta(seconds=60)\n)\ncache_client.create_cache("cache")\ncache_client.set("cache", "myKey", "myValue")\nget_response = cache_client.get("cache", "myKey")\nif isinstance(get_response, CacheGet.Hit):\n    print(f"Got value: {get_response.value_string}")\n\n```\n\n## Getting Started and Documentation\n\nDocumentation is available on the [Momento Docs website](https://docs.momentohq.com).\n\n## Examples\n\nWorking example projects, with all required build configuration files, are available for both Python 3.10 and up\nand Python versions before 3.10:\n\n* [Python 3.10+ examples](./examples/py310)\n* [Pre-3.10 Python examples](./examples/prepy310)\n\n## Developing\n\nIf you are interested in contributing to the SDK, please see the [CONTRIBUTING](./CONTRIBUTING.md) docs.\n\n----------------------------------------------------------------------------------------\nFor more info, visit our website at [https://gomomento.com](https://gomomento.com)!\n',
+    'long_description': '<head>\n  <meta name="Momento Python Client Library Documentation" content="Python client software development kit for Momento Cache">\n</head>\n<img src="https://docs.momentohq.com/img/logo.svg" alt="logo" width="400"/>\n\n[![project status](https://momentohq.github.io/standards-and-practices/badges/project-status-official.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md)\n[![project stability](https://momentohq.github.io/standards-and-practices/badges/project-stability-stable.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md)\n\n# Momento Python Client Library\n\nMomento Cache is a fast, simple, pay-as-you-go caching solution without any of the operational overhead\nrequired by traditional caching solutions.  This repo contains the source code for the Momento Python client library.\n\nTo get started with Momento you will need a Momento Auth Token. You can get one from the [Momento Console](https://console.gomomento.com).\n\n* Website: [https://www.gomomento.com/](https://www.gomomento.com/)\n* Momento Documentation: [https://docs.momentohq.com/](https://docs.momentohq.com/)\n* Getting Started: [https://docs.momentohq.com/getting-started](https://docs.momentohq.com/getting-started)\n* Python SDK Documentation: [https://docs.momentohq.com/develop/sdks/python](https://docs.momentohq.com/develop/sdks/python)\n* Discuss: [Momento Discord](https://discord.gg/3HkAKjUZGq)\n\n## Packages\n\nThe Momento Python SDK package is available on pypi: [momento](https://pypi.org/project/momento/).\n\n## Usage\n\nThe examples below require an environment variable named MOMENTO_AUTH_TOKEN which must\nbe set to a valid [Momento authentication token](https://docs.momentohq.com/docs/getting-started#obtain-an-auth-token).\n\nPython 3.10 introduced the `match` statement, which allows for [structural pattern matching on objects](https://peps.python.org/pep-0636/#adding-a-ui-matching-objects).\nIf you are running python 3.10 or greater, here is a quickstart you can use in your own project:\n\n```python\nfrom datetime import timedelta\n\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache, ListCaches\n\ncache_client = CacheClient(\n    Configurations.Laptop.v1(),\n    CredentialProvider.from_environment_variable("MOMENTO_AUTH_TOKEN"),\n    timedelta(seconds=60)\n)\n\ncreate_cache_response = cache_client.create_cache("cache")\nset_response = cache_client.set("cache", "my-key", "my-value")\nget_response = cache_client.get(_CACHE_NAME, _KEY)\nmatch get_response:\n    case CacheGet.Hit() as hit:\n        print(f"Got value: {hit.value_string}")\n    case _:\n        print(f"Response was not a hit: {get_response}")\n\n```\n\nThe above code uses [structural pattern matching](https://peps.python.org/pep-0636/), a feature introduced in Python 3.10.\nUsing a Python version less than 3.10? No problem. Here is the same example compatible across all versions of Python:\n\n```python\nfrom datetime import timedelta\n\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache\n\ncache_client = CacheClient(\n    configuration=Configurations.Laptop.v1(),\n    credential_provider=CredentialProvider.from_environment_variable(\'MOMENTO_AUTH_TOKEN\'),\n    default_ttl=timedelta(seconds=60)\n)\ncache_client.create_cache("cache")\ncache_client.set("cache", "myKey", "myValue")\nget_response = cache_client.get("cache", "myKey")\nif isinstance(get_response, CacheGet.Hit):\n    print(f"Got value: {get_response.value_string}")\n\n```\n\n## Getting Started and Documentation\n\nDocumentation is available on the [Momento Docs website](https://docs.momentohq.com).\n\n## Examples\n\nWorking example projects, with all required build configuration files, are available for both Python 3.10 and up\nand Python versions before 3.10:\n\n* [Python 3.10+ examples](./examples/py310)\n* [Pre-3.10 Python examples](./examples/prepy310)\n\n## Developing\n\nIf you are interested in contributing to the SDK, please see the [CONTRIBUTING](./CONTRIBUTING.md) docs.\n\n----------------------------------------------------------------------------------------\nFor more info, visit our website at [https://gomomento.com](https://gomomento.com)!\n',
     'author': 'Momento',
     'author_email': 'hello@momentohq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gomomento.com',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `momento-1.6.0/PKG-INFO` & `momento-1.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momento
-Version: 1.6.0
+Version: 1.6.1
 Summary: SDK for Momento
 Home-page: https://gomomento.com
 License: Apache-2.0
 Keywords: Momento,caching,key-value store,serverless
 Author: Momento
 Author-email: hello@momentohq.com
 Requires-Python: >=3.7,<4.0
@@ -40,14 +40,16 @@
 [![project stability](https://momentohq.github.io/standards-and-practices/badges/project-stability-stable.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md)
 
 # Momento Python Client Library
 
 Momento Cache is a fast, simple, pay-as-you-go caching solution without any of the operational overhead
 required by traditional caching solutions.  This repo contains the source code for the Momento Python client library.
 
+To get started with Momento you will need a Momento Auth Token. You can get one from the [Momento Console](https://console.gomomento.com).
+
 * Website: [https://www.gomomento.com/](https://www.gomomento.com/)
 * Momento Documentation: [https://docs.momentohq.com/](https://docs.momentohq.com/)
 * Getting Started: [https://docs.momentohq.com/getting-started](https://docs.momentohq.com/getting-started)
 * Python SDK Documentation: [https://docs.momentohq.com/develop/sdks/python](https://docs.momentohq.com/develop/sdks/python)
 * Discuss: [Momento Discord](https://discord.gg/3HkAKjUZGq)
 
 ## Packages
```

