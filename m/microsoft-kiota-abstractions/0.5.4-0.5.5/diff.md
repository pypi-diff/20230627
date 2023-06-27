# Comparing `tmp/microsoft_kiota_abstractions-0.5.4.tar.gz` & `tmp/microsoft_kiota_abstractions-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoft_kiota_abstractions-0.5.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "microsoft_kiota_abstractions-0.5.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `microsoft_kiota_abstractions-0.5.4.tar` & `microsoft_kiota_abstractions-0.5.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0       82 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/.github/CODEOWNERS
--rw-r--r--   0        0        0      240 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/.github/dependabot.yml
--rw-r--r--   0        0        0      792 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/.github/workflows/auto-merge-dependabot.yml
--rw-r--r--   0        0        0     1927 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/.github/workflows/build.yml
--rw-r--r--   0        0        0     2538 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1270 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/.github/workflows/conflicting-pr-label.yml
--rw-r--r--   0        0        0     1097 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1799 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/.gitignore
--rw-r--r--   0        0        0    15931 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/.pylintrc
--rw-r--r--   0        0        0     1027 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/CHANGELOG.md
--rw-r--r--   0        0        0      444 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/LICENSE
--rw-r--r--   0        0        0     2512 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/README.md
--rw-r--r--   0        0        0     2757 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/SECURITY.md
--rw-r--r--   0        0        0     1244 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/SUPPORT.md
--rw-r--r--   0        0        0      119 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/__init__.py
--rw-r--r--   0        0        0       23 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/_version.py
--rw-r--r--   0        0        0     3566 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/api_client_builder.py
--rw-r--r--   0        0        0      399 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/api_error.py
--rw-r--r--   0        0        0      346 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/authentication/__init__.py
--rw-r--r--   0        0        0      836 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/authentication/access_token_provider.py
--rw-r--r--   0        0        0     2120 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/authentication/allowed_hosts_validator.py
--rw-r--r--   0        0        0      607 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/authentication/anonymous_authentication_provider.py
--rw-r--r--   0        0        0      473 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/authentication/authentication_provider.py
--rw-r--r--   0        0        0     1231 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py
--rw-r--r--   0        0        0     1277 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/base_request_builder.py
--rw-r--r--   0        0        0      372 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/default_query_parameters.py
--rw-r--r--   0        0        0      453 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/get_path_parameters.py
--rw-r--r--   0        0        0      529 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/method.py
--rw-r--r--   0        0        0      938 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/native_response_handler.py
--rw-r--r--   0        0        0     5164 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/request_adapter.py
--rw-r--r--   0        0        0      663 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/request_configuration.py
--rw-r--r--   0        0        0     9048 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/request_information.py
--rw-r--r--   0        0        0      312 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/request_option.py
--rw-r--r--   0        0        0      965 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/response_handler.py
--rw-r--r--   0        0        0      679 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/__init__.py
--rw-r--r--   0        0        0      374 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/additional_data_holder.py
--rw-r--r--   0        0        0     1006 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/parsable.py
--rw-r--r--   0        0        0      642 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/parsable_factory.py
--rw-r--r--   0        0        0     5793 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/parse_node.py
--rw-r--r--   0        0        0      903 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/parse_node_factory.py
--rw-r--r--   0        0        0     1972 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/parse_node_factory_registry.py
--rw-r--r--   0        0        0      949 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/parse_node_helper.py
--rw-r--r--   0        0        0     2424 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/parse_node_proxy_factory.py
--rw-r--r--   0        0        0     9768 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/serialization_writer.py
--rw-r--r--   0        0        0      898 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/serialization_writer_factory.py
--rw-r--r--   0        0        0     2025 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/serialization_writer_factory_registry.py
--rw-r--r--   0        0        0     3132 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/serialization_writer_proxy_factory.py
--rw-r--r--   0        0        0      529 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/store/__init__.py
--rw-r--r--   0        0        0      398 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/store/backed_model.py
--rw-r--r--   0        0        0     3892 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/store/backing_store.py
--rw-r--r--   0        0        0      424 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/store/backing_store_factory.py
--rw-r--r--   0        0        0      237 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/store/backing_store_factory_singleton.py
--rw-r--r--   0        0        0     1166 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/store/backing_store_parse_node_factory.py
--rw-r--r--   0        0        0     1809 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py
--rw-r--r--   0        0        0     4488 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/store/in_memory_backing_store.py
--rw-r--r--   0        0        0      380 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/store/in_memory_backing_store_factory.py
--rw-r--r--   0        0        0      899 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/kiota_abstractions/utils.py
--rw-r--r--   0        0        0     1268 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     1130 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/requirements-dev.txt
--rw-r--r--   0        0        0        0 2023-06-26 05:24:30.907410 microsoft_kiota_abstractions-0.5.4/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-26 05:24:30.911410 microsoft_kiota_abstractions-0.5.4/tests/authentication/__init__.py
--rw-r--r--   0        0        0     1041 2023-06-26 05:24:30.911410 microsoft_kiota_abstractions-0.5.4/tests/authentication/test_base_bearer_token_authentication.py
--rw-r--r--   0        0        0      831 2023-06-26 05:24:30.911410 microsoft_kiota_abstractions-0.5.4/tests/conftest.py
--rw-r--r--   0        0        0     5109 2023-06-26 05:24:30.911410 microsoft_kiota_abstractions-0.5.4/tests/test_request_information.py
--rw-r--r--   0        0        0     3433 1970-01-01 00:00:00.000000 microsoft_kiota_abstractions-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0       82 2023-06-27 09:33:53.387362 microsoft_kiota_abstractions-0.5.5/.github/CODEOWNERS
+-rw-r--r--   0        0        0      240 2023-06-27 09:33:53.387362 microsoft_kiota_abstractions-0.5.5/.github/dependabot.yml
+-rw-r--r--   0        0        0      792 2023-06-27 09:33:53.387362 microsoft_kiota_abstractions-0.5.5/.github/workflows/auto-merge-dependabot.yml
+-rw-r--r--   0        0        0     1927 2023-06-27 09:33:53.387362 microsoft_kiota_abstractions-0.5.5/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2538 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1270 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/.github/workflows/conflicting-pr-label.yml
+-rw-r--r--   0        0        0     1097 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1799 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/.gitignore
+-rw-r--r--   0        0        0    15931 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/.pylintrc
+-rw-r--r--   0        0        0     1197 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/CHANGELOG.md
+-rw-r--r--   0        0        0      444 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/LICENSE
+-rw-r--r--   0        0        0     2512 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/README.md
+-rw-r--r--   0        0        0     2757 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/SECURITY.md
+-rw-r--r--   0        0        0     1244 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/SUPPORT.md
+-rw-r--r--   0        0        0      119 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/__init__.py
+-rw-r--r--   0        0        0       23 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/_version.py
+-rw-r--r--   0        0        0     3566 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/api_client_builder.py
+-rw-r--r--   0        0        0      399 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/api_error.py
+-rw-r--r--   0        0        0      346 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/__init__.py
+-rw-r--r--   0        0        0      836 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/access_token_provider.py
+-rw-r--r--   0        0        0     2120 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/allowed_hosts_validator.py
+-rw-r--r--   0        0        0      607 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/anonymous_authentication_provider.py
+-rw-r--r--   0        0        0      473 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/authentication_provider.py
+-rw-r--r--   0        0        0     1231 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py
+-rw-r--r--   0        0        0     1252 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/base_request_builder.py
+-rw-r--r--   0        0        0      667 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/base_request_configuration.py
+-rw-r--r--   0        0        0      372 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/default_query_parameters.py
+-rw-r--r--   0        0        0      453 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/get_path_parameters.py
+-rw-r--r--   0        0        0      529 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/method.py
+-rw-r--r--   0        0        0      938 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/native_response_handler.py
+-rw-r--r--   0        0        0     5164 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/request_adapter.py
+-rw-r--r--   0        0        0     9048 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/request_information.py
+-rw-r--r--   0        0        0      312 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/request_option.py
+-rw-r--r--   0        0        0      965 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/response_handler.py
+-rw-r--r--   0        0        0      679 2023-06-27 09:33:53.391362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/__init__.py
+-rw-r--r--   0        0        0      374 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/additional_data_holder.py
+-rw-r--r--   0        0        0     1006 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parsable.py
+-rw-r--r--   0        0        0      642 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parsable_factory.py
+-rw-r--r--   0        0        0     5793 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node.py
+-rw-r--r--   0        0        0      903 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node_factory.py
+-rw-r--r--   0        0        0     1972 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node_factory_registry.py
+-rw-r--r--   0        0        0      949 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node_helper.py
+-rw-r--r--   0        0        0     2424 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node_proxy_factory.py
+-rw-r--r--   0        0        0     9768 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/serialization_writer.py
+-rw-r--r--   0        0        0      898 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/serialization_writer_factory.py
+-rw-r--r--   0        0        0     2025 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/serialization_writer_factory_registry.py
+-rw-r--r--   0        0        0     3132 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/serialization_writer_proxy_factory.py
+-rw-r--r--   0        0        0      529 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/__init__.py
+-rw-r--r--   0        0        0      398 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/backed_model.py
+-rw-r--r--   0        0        0     3892 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/backing_store.py
+-rw-r--r--   0        0        0      424 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/backing_store_factory.py
+-rw-r--r--   0        0        0      237 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/backing_store_factory_singleton.py
+-rw-r--r--   0        0        0     1166 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/backing_store_parse_node_factory.py
+-rw-r--r--   0        0        0     1809 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py
+-rw-r--r--   0        0        0     4488 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/in_memory_backing_store.py
+-rw-r--r--   0        0        0      380 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/in_memory_backing_store_factory.py
+-rw-r--r--   0        0        0      899 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/kiota_abstractions/utils.py
+-rw-r--r--   0        0        0     1268 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     1130 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/tests/authentication/__init__.py
+-rw-r--r--   0        0        0     1041 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/tests/authentication/test_base_bearer_token_authentication.py
+-rw-r--r--   0        0        0      831 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/tests/conftest.py
+-rw-r--r--   0        0        0     5109 2023-06-27 09:33:53.395362 microsoft_kiota_abstractions-0.5.5/tests/test_request_information.py
+-rw-r--r--   0        0        0     3433 1970-01-01 00:00:00.000000 microsoft_kiota_abstractions-0.5.5/PKG-INFO
```

### Comparing `microsoft_kiota_abstractions-0.5.4/.github/workflows/auto-merge-dependabot.yml` & `microsoft_kiota_abstractions-0.5.5/.github/workflows/auto-merge-dependabot.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/.github/workflows/build.yml` & `microsoft_kiota_abstractions-0.5.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/.github/workflows/codeql-analysis.yml` & `microsoft_kiota_abstractions-0.5.5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/.github/workflows/conflicting-pr-label.yml` & `microsoft_kiota_abstractions-0.5.5/.github/workflows/conflicting-pr-label.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/.github/workflows/publish.yml` & `microsoft_kiota_abstractions-0.5.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/.gitignore` & `microsoft_kiota_abstractions-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/.pylintrc` & `microsoft_kiota_abstractions-0.5.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/CHANGELOG.md` & `microsoft_kiota_abstractions-0.5.5/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.5.5] - 2023-06-26
+
+### Added
+
+### Changed
+
+- Changed BaseRequesBuilder class to be instantiable.
+- Renamed RequestConfiguration class to BaseRequestConfiguration.
+
 ## [0.5.4] - 2023-06-22
 
 ### Added
 
 - Added a base request builder and a request configuration class to reduce the amount of code being generated.
 
 ### Changed
```

### Comparing `microsoft_kiota_abstractions-0.5.4/LICENSE` & `microsoft_kiota_abstractions-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/README.md` & `microsoft_kiota_abstractions-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/SECURITY.md` & `microsoft_kiota_abstractions-0.5.5/SECURITY.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/SUPPORT.md` & `microsoft_kiota_abstractions-0.5.5/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/api_client_builder.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/api_client_builder.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/authentication/access_token_provider.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/access_token_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/authentication/allowed_hosts_validator.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/allowed_hosts_validator.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/authentication/anonymous_authentication_provider.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/anonymous_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/base_request_builder.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/base_request_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # ------------------------------------
 # Copyright (c) Microsoft Corporation. All Rights Reserved.
 # Licensed under the MIT License.
 # See License in the project root for license information.
 # ------------------------------------
-from abc import ABC
 from typing import Any, Dict, Union
 
 from .request_adapter import RequestAdapter
 
 
-class BaseRequestBuilder(ABC):
+class BaseRequestBuilder:
     """Base class for all request builders"""
 
     def __init__(
         self, request_adapter: RequestAdapter, url_template: str,
         path_parameters: Union[Dict[str, Any], str]
     ) -> None:
         """Initializes a new instance of the BaseRequestBuilder class."""
```

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/method.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/method.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/native_response_handler.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/native_response_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/request_adapter.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/request_adapter.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/request_configuration.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/base_request_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from dataclasses import dataclass
 from typing import Dict, List, Optional, Union
 
 from .request_option import RequestOption
 
 
 @dataclass
-class RequestConfiguration:
+class BaseRequestConfiguration:
     """
     Configuration for the request such as headers, query parameters, and middleware options.
     """
     # Request headers
     headers: Optional[Dict[str, Union[str, List[str]]]] = None
 
     # Request options
```

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/request_information.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/request_information.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/response_handler.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/response_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/__init__.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/parsable.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parsable.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/parsable_factory.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parsable_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/parse_node.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/parse_node_factory.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/parse_node_factory_registry.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node_factory_registry.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/parse_node_helper.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node_helper.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/parse_node_proxy_factory.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/parse_node_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/serialization_writer.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/serialization_writer.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/serialization_writer_factory.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/serialization_writer_factory_registry.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/serialization_writer_factory_registry.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/serialization/serialization_writer_proxy_factory.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/serialization/serialization_writer_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/store/__init__.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/__init__.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/store/backing_store.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/backing_store.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/store/backing_store_parse_node_factory.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/backing_store_parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/store/in_memory_backing_store.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/store/in_memory_backing_store.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/kiota_abstractions/utils.py` & `microsoft_kiota_abstractions-0.5.5/kiota_abstractions/utils.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/pyproject.toml` & `microsoft_kiota_abstractions-0.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/requirements-dev.txt` & `microsoft_kiota_abstractions-0.5.5/requirements-dev.txt`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 isort==5.12.0
 
 lazy-object-proxy==1.9.0 ; python_version >= '3.7'
 
 mccabe==0.7.0 ; python_version >= '3.6'
 
-mypy==1.4.0
+mypy==1.4.1
 
 mypy-extensions==1.0.0 ; python_version >= '3.5'
 
 packaging==23.1 ; python_version >= '3.7'
 
 platformdirs==3.8.0 ; python_version >= '3.7'
```

### Comparing `microsoft_kiota_abstractions-0.5.4/tests/authentication/test_base_bearer_token_authentication.py` & `microsoft_kiota_abstractions-0.5.5/tests/authentication/test_base_bearer_token_authentication.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/tests/conftest.py` & `microsoft_kiota_abstractions-0.5.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/tests/test_request_information.py` & `microsoft_kiota_abstractions-0.5.5/tests/test_request_information.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-0.5.4/PKG-INFO` & `microsoft_kiota_abstractions-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microsoft-kiota-abstractions
-Version: 0.5.4
+Version: 0.5.5
 Summary: Core abstractions for kiota generated libraries in Python
 Keywords: kiota,openAPI,Microsoft,Graph
 Author-email: Microsoft <graphtooling+python@microsoft.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

