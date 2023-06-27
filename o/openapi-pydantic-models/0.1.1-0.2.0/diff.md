# Comparing `tmp/openapi-pydantic-models-0.1.1.tar.gz` & `tmp/openapi-pydantic-models-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi-pydantic-models-0.1.1.tar", last modified: Sun Jun 25 16:50:58 2023, max compression
+gzip compressed data, was "openapi-pydantic-models-0.2.0.tar", last modified: Tue Jun 27 06:25:28 2023, max compression
```

## Comparing `openapi-pydantic-models-0.1.1.tar` & `openapi-pydantic-models-0.2.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:50:58.140567 openapi-pydantic-models-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-25 16:50:58.140567 openapi-pydantic-models-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 16:50:58.140567 openapi-pydantic-models-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:50:58.136567 openapi-pydantic-models-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:50:58.136567 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:50:58.136567 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/commons/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/commons/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/commons/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:50:58.140567 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/callback_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/components_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/contact_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/encoding_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/example_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/external_documentation_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/header_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/info_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/license_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/link_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/media_type_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/oauth_flow_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/oauth_flows_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/openapi_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/operation_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/parameter_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/path_item_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/paths_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/reference_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/request_body_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/response_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/responses_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/schema_object.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/security_requirement_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/security_scheme_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/server_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/server_variable_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/specification_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/styles.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/tag_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:50:58.136567 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-25 16:50:58.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-25 16:50:58.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 16:50:58.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 16:50:57.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-25 16:50:58.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-25 16:50:58.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:25:28.663330 openapi-pydantic-models-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-27 06:25:28.663330 openapi-pydantic-models-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 06:25:28.663330 openapi-pydantic-models-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:25:28.659330 openapi-pydantic-models-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:25:28.659330 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:25:28.659330 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/commons/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/commons/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:25:28.663330 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/callback_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/components_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/contact_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/encoding_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/example_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/external_documentation_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/header_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/info_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/license_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/link_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/media_type_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/oauth_flow_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/oauth_flows_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/openapi_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/operation_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/parameter_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/path_item_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/paths_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/reference_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/request_body_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/response_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/responses_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/schema_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/security_requirement_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/security_scheme_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/server_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/server_variable_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/specification_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/tag_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:25:28.659330 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-27 06:25:28.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-27 06:25:28.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 06:25:28.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 06:25:28.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-27 06:25:28.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-27 06:25:28.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models.egg-info/top_level.txt
```

### Comparing `openapi-pydantic-models-0.1.1/.gitignore` & `openapi-pydantic-models-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.1/LICENSE` & `openapi-pydantic-models-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.1/MANIFEST.in` & `openapi-pydantic-models-0.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.1/PKG-INFO` & `openapi-pydantic-models-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-pydantic-models
-Version: 0.1.1
+Version: 0.2.0
 Summary: pydantic models for OpeanAPI Specification 3.1.0 objects.
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/openapi-pydantic-models
 Keywords: OpenAPI OAS
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -72,16 +72,16 @@
             encoding=None
         )
     },
     links=None
 )
 ```
 
-Any object from can always be exported back to OpenaAPI data (`dict`) via `dict()`
-method:
+Any object from object tree can always be exported back to OpenaAPI data (`dict`) via
+`dict()` method:
 
 ```py
 spec.paths["/pet/{petId}/uploadImage"].post.responses["200"].dict()
 
 {
     'description': 'successful operation',
      'content': {
@@ -132,14 +132,33 @@
 obj.extensions
 ExtensionsStorage({'x-foo': 'bar', 'x-bar': [42]})
 
 obj.dict()
 {'description': 'successful operation', 'x-foo': 'bar', 'x-bar': [42]}
 ```
 
+And of course, all objects can be edited:
+
+```py
+obj.description = "ZOMG!"
+obj.extensions["x-baz"] = {1: {2: 3}}
+obj.dict()
+{'description': 'ZOMG!', 'x-foo': 'bar', 'x-bar': [42], 'x-baz': {1: {2: 3}}}
+```
+
+where specification extensions are protected from invalid keys:
+
+```py
+obj.extensions["baz"] = 34
+# KeyError: 'baz'
+
+obj.extensions["x-baz"] = 34
+# OK
+```
+
 ## Where are the docs for this thing?
 
 Makes no sense writing them since [OpenAPI
 Specification](https://spec.openapis.org/oas/v3.1.0) is already fully and excellently
 documented.
 
 In OpenAPI docs, wherever you see "Foo Object" you can find `class FooObject` in
```

### Comparing `openapi-pydantic-models-0.1.1/README.md` & `openapi-pydantic-models-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -48,16 +48,16 @@
             encoding=None
         )
     },
     links=None
 )
 ```
 
-Any object from can always be exported back to OpenaAPI data (`dict`) via `dict()`
-method:
+Any object from object tree can always be exported back to OpenaAPI data (`dict`) via
+`dict()` method:
 
 ```py
 spec.paths["/pet/{petId}/uploadImage"].post.responses["200"].dict()
 
 {
     'description': 'successful operation',
      'content': {
@@ -108,14 +108,33 @@
 obj.extensions
 ExtensionsStorage({'x-foo': 'bar', 'x-bar': [42]})
 
 obj.dict()
 {'description': 'successful operation', 'x-foo': 'bar', 'x-bar': [42]}
 ```
 
+And of course, all objects can be edited:
+
+```py
+obj.description = "ZOMG!"
+obj.extensions["x-baz"] = {1: {2: 3}}
+obj.dict()
+{'description': 'ZOMG!', 'x-foo': 'bar', 'x-bar': [42], 'x-baz': {1: {2: 3}}}
+```
+
+where specification extensions are protected from invalid keys:
+
+```py
+obj.extensions["baz"] = 34
+# KeyError: 'baz'
+
+obj.extensions["x-baz"] = 34
+# OK
+```
+
 ## Where are the docs for this thing?
 
 Makes no sense writing them since [OpenAPI
 Specification](https://spec.openapis.org/oas/v3.1.0) is already fully and excellently
 documented.
 
 In OpenAPI docs, wherever you see "Foo Object" you can find `class FooObject` in
```

### Comparing `openapi-pydantic-models-0.1.1/pyproject.toml` & `openapi-pydantic-models-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel"]
 
 
 [project]
 name = "openapi-pydantic-models"
-version = "0.1.1"
+version = "0.2.0"
 description = "pydantic models for OpeanAPI Specification 3.1.0 objects."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
```

### Comparing `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/commons/utilities.py` & `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/commons/utilities.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,17 +9,39 @@
         return False
 
     if isinstance(data, (str, bytes)):
         return not bool(data.strip())
 
     retv = None
 
+    # security: list[SecurityRequirementObject] | None = None
+    #
+    # example:
+    #
+    #     data = {
+    #         "security": [{"refresh_token": []}]
+    #     }
+    #
+    # Is non-blank object in context of OpenAPI, although
+    #
+    #     is_blank(data) == True
+
     # Mapping
     try:
-        retv = all(is_blank(v) for v in data.values())
+        found_non_blank = False
+        for k, v in data.items():
+            if k == "security":
+                found_non_blank = bool(v and any(_.keys() for _ in v))
+            else:
+                found_non_blank = not is_blank(v)
+
+            if found_non_blank:
+                break
+
+        retv = not found_non_blank
     except AttributeError:
         pass
     if retv is not None:
         return retv
 
     # Iterable
     try:
@@ -61,17 +83,32 @@
     retv = strip_whitespace(data)
 
     if isinstance(retv, (str, bytes)):
         return retv if not is_blank(retv) else None
 
     # Mapping
     try:
-        retv = type(data)(
-            (k, v) for k, v in retv.items() if not is_blank(k) and not is_blank(v)
-        )
+        tuples = []
+        for k, v in retv.items():
+            if k == "security" and v:
+                tuples.append(
+                    (
+                        k,
+                        [_ for _ in v if _ and _.keys()],
+                    )
+                )
+            elif not is_blank(k) and not is_blank(v):
+                tuples.append(
+                    (
+                        k,
+                        v,
+                    )
+                )
+
+        retv = type(data)(_ for _ in tuples)
         return retv or None
     except (AttributeError, TypeError):
         pass
 
     # Iterable
     try:
         retv = type(data)(v for v in retv if not is_blank(v))
```

### Comparing `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/__init__.py` & `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/callback_object.py` & `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/callback_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import itertools
-from typing import Iterator, MutableMapping
+from typing import Any, Iterator, MutableMapping
 
 from pydantic import PrivateAttr
 
 from ..commons import BaseModel, exclude_blanks
 from .path_item_object import PathItemObject
 from .reference_object import ReferenceObject
 from .specification_extensions import ExtensionsStorage
@@ -96,15 +96,17 @@
                     else v
                     for k, v in self._data.items()
                 }
             )
             + ")"
         )
 
-    def dict(self, *, by_alias: bool = True, exclude_none: bool = True, **kwargs):
+    def dict(
+        self, *, by_alias: bool = True, exclude_none: bool = True, **kwargs
+    ) -> dict[str, Any]:
         retv = {
             k: (
                 v.dict(by_alias=by_alias, exclude_none=exclude_none, **kwargs)
                 if isinstance(v, (ReferenceObject, PathItemObject))
                 else v
             )
             for k, v in itertools.chain(self._data.items(), self._ext.items())
```

### Comparing `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/components_object.py` & `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/components_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/encoding_object.py` & `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/encoding_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/header_object.py` & `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/header_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/media_type_object.py` & `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/media_type_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/openapi_object.py` & `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/openapi_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/operation_object.py` & `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/operation_object.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
+
 from .external_documentation_object import ExternalDocumentationObject
 from .parameter_object import ParameterObject
 from .reference_object import ReferenceObject
 from .request_body_object import RequestBodyObject
 from .responses_object import ResponsesObject
 from .security_requirement_object import SecurityRequirementObject
 from .server_object import ServerObject
 from .specification_extensions import SpecificationExtendable
 
-from typing import TYPE_CHECKING
-
 if TYPE_CHECKING:
     from .callback_object import CallbackObject
 
 
 class OperationObject(SpecificationExtendable):
     tags: list[str] | None = None
     summary: str | None = None
```

### Comparing `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/parameter_object.py` & `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/parameter_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/path_item_object.py` & `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/path_item_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/paths_object.py` & `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/paths_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import itertools
-from typing import Iterator, MutableMapping
+from typing import Any, Iterator, MutableMapping
 
 from pydantic import PrivateAttr
 
 from ..commons import BaseModel, exclude_blanks
 from .path_item_object import PathItemObject
 from .specification_extensions import ExtensionsStorage
 
@@ -106,15 +106,17 @@
                     else v
                     for k, v in self._data.items()
                 }
             )
             + ")"
         )
 
-    def dict(self, *, by_alias: bool = True, exclude_none: bool = True, **kwargs):
+    def dict(
+        self, *, by_alias: bool = True, exclude_none: bool = True, **kwargs
+    ) -> dict[str, Any]:
         retv = {
             k: (
                 v.dict(by_alias=by_alias, exclude_none=exclude_none, **kwargs)
                 if isinstance(v, PathItemObject)
                 else v
             )
             for k, v in itertools.chain(self._data.items(), self._ext.items())
```

### Comparing `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/responses_object.py` & `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/responses_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import itertools
-from typing import Iterator, MutableMapping
+from typing import Any, Iterator, MutableMapping
 
 from pydantic import PrivateAttr
 
 from ..commons import BaseModel, exclude_blanks
 from .reference_object import ReferenceObject
 from .response_object import ResponseObject
 from .specification_extensions import ExtensionsStorage
@@ -101,15 +101,17 @@
             for k, v in self._data.items()
         }
         if self.default:
             data["default"] = self.default.dict(by_alias=True, exclude_none=False)
 
         return f"{self.__class__.__name__}({repr(data)})"
 
-    def dict(self, *, by_alias: bool = True, exclude_none: bool = True, **kwargs):
+    def dict(
+        self, *, by_alias: bool = True, exclude_none: bool = True, **kwargs
+    ) -> dict[str, Any]:
         retv = {
             k: (
                 v.dict(by_alias=by_alias, exclude_none=exclude_none, **kwargs)
                 if isinstance(v, (ReferenceObject, ResponseObject))
                 else v
             )
             for k, v in itertools.chain(self._data.items(), self._ext.items())
```

### Comparing `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/security_scheme_object.py` & `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/security_scheme_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/specification_extensions.py` & `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/specification_extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,17 @@
         )
         self._ext = ExtensionsStorage(data)
 
     @property
     def extensions(self) -> ExtensionsStorage:
         return self._ext
 
-    def dict(self, *, by_alias: bool = True, exclude_none: bool = True, **kwargs):
+    def dict(
+        self, *, by_alias: bool = True, exclude_none: bool = True, **kwargs
+    ) -> dict[str, Any]:
         retv = (
             super().dict(exclude_none=exclude_none, by_alias=by_alias, **kwargs)
             or dict()
         )
 
         for k, v in self._ext.items():
             retv[str(k)] = v
```

### Comparing `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models.egg-info/PKG-INFO` & `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-pydantic-models
-Version: 0.1.1
+Version: 0.2.0
 Summary: pydantic models for OpeanAPI Specification 3.1.0 objects.
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/openapi-pydantic-models
 Keywords: OpenAPI OAS
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -72,16 +72,16 @@
             encoding=None
         )
     },
     links=None
 )
 ```
 
-Any object from can always be exported back to OpenaAPI data (`dict`) via `dict()`
-method:
+Any object from object tree can always be exported back to OpenaAPI data (`dict`) via
+`dict()` method:
 
 ```py
 spec.paths["/pet/{petId}/uploadImage"].post.responses["200"].dict()
 
 {
     'description': 'successful operation',
      'content': {
@@ -132,14 +132,33 @@
 obj.extensions
 ExtensionsStorage({'x-foo': 'bar', 'x-bar': [42]})
 
 obj.dict()
 {'description': 'successful operation', 'x-foo': 'bar', 'x-bar': [42]}
 ```
 
+And of course, all objects can be edited:
+
+```py
+obj.description = "ZOMG!"
+obj.extensions["x-baz"] = {1: {2: 3}}
+obj.dict()
+{'description': 'ZOMG!', 'x-foo': 'bar', 'x-bar': [42], 'x-baz': {1: {2: 3}}}
+```
+
+where specification extensions are protected from invalid keys:
+
+```py
+obj.extensions["baz"] = 34
+# KeyError: 'baz'
+
+obj.extensions["x-baz"] = 34
+# OK
+```
+
 ## Where are the docs for this thing?
 
 Makes no sense writing them since [OpenAPI
 Specification](https://spec.openapis.org/oas/v3.1.0) is already fully and excellently
 documented.
 
 In OpenAPI docs, wherever you see "Foo Object" you can find `class FooObject` in
```

### Comparing `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models.egg-info/SOURCES.txt` & `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

