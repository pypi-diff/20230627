# Comparing `tmp/slingshot_ai-0.0.10.tar.gz` & `tmp/slingshot_ai-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slingshot_ai-0.0.10.tar", max compression
+gzip compressed data, was "slingshot_ai-0.0.11.tar", max compression
```

## Comparing `slingshot_ai-0.0.10.tar` & `slingshot_ai-0.0.11.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0      825 2023-06-23 17:36:03.506841 slingshot_ai-0.0.10/pyproject.toml
--rw-r--r--   0        0        0      156 2023-06-14 01:36:51.753575 slingshot_ai-0.0.10/src/slingshot/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.733834 slingshot_ai-0.0.10/src/slingshot/cli/__init__.py
--rw-r--r--   0        0        0    17098 2023-06-14 17:13:24.232346 slingshot_ai-0.0.10/src/slingshot/cli/add.py
--rw-r--r--   0        0        0     1509 2023-06-09 16:08:07.433961 slingshot_ai-0.0.10/src/slingshot/cli/apply.py
--rw-r--r--   0        0        0     5276 2023-06-14 17:13:24.232871 slingshot_ai-0.0.10/src/slingshot/cli/apps.py
--rw-r--r--   0        0        0     5916 2023-06-20 21:48:49.557285 slingshot_ai-0.0.10/src/slingshot/cli/artifact.py
--rw-r--r--   0        0        0     5275 2023-06-14 16:35:36.287394 slingshot_ai-0.0.10/src/slingshot/cli/auth.py
--rw-r--r--   0        0        0      970 2023-06-08 13:51:24.734880 slingshot_ai-0.0.10/src/slingshot/cli/code.py
--rw-r--r--   0        0        0        0 2023-06-12 16:23:44.406584 slingshot_ai-0.0.10/src/slingshot/cli/config/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.734966 slingshot_ai-0.0.10/src/slingshot/cli/config/py.typed
--rw-r--r--   0        0        0      850 2023-06-14 16:35:36.287763 slingshot_ai-0.0.10/src/slingshot/cli/config/sentry_setup.py
--rw-r--r--   0        0        0    13806 2023-06-14 16:35:36.288173 slingshot_ai-0.0.10/src/slingshot/cli/config/slingshot_cli.py
--rw-r--r--   0        0        0     1234 2023-06-08 13:51:24.735333 slingshot_ai-0.0.10/src/slingshot/cli/dev.py
--rw-r--r--   0        0        0     1123 2023-06-23 17:35:28.186738 slingshot_ai-0.0.10/src/slingshot/cli/environment.py
--rw-r--r--   0        0        0     4519 2023-06-13 20:59:00.706466 slingshot_ai-0.0.10/src/slingshot/cli/inference.py
--rw-r--r--   0        0        0     3059 2023-06-08 13:51:24.735634 slingshot_ai-0.0.10/src/slingshot/cli/logs.py
--rw-r--r--   0        0        0     2666 2023-06-23 17:35:28.188182 slingshot_ai-0.0.10/src/slingshot/cli/main.py
--rw-r--r--   0        0        0     2475 2023-06-09 16:08:07.434298 slingshot_ai-0.0.10/src/slingshot/cli/project.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.735998 slingshot_ai-0.0.10/src/slingshot/cli/py.typed
--rw-r--r--   0        0        0     7854 2023-06-08 13:51:24.736194 slingshot_ai-0.0.10/src/slingshot/cli/run.py
--rw-r--r--   0        0        0     3648 2023-06-08 14:01:51.180092 slingshot_ai-0.0.10/src/slingshot/cli/secret.py
--rw-r--r--   0        0        0     3816 2023-06-15 18:10:07.073951 slingshot_ai-0.0.10/src/slingshot/cli/session.py
--rw-r--r--   0        0        0       67 2023-06-08 13:51:24.737453 slingshot_ai-0.0.10/src/slingshot/cli/shared/__init__.py
--rw-r--r--   0        0        0     6260 2023-06-20 21:48:49.557743 slingshot_ai-0.0.10/src/slingshot/cli/shared/code_sync.py
--rw-r--r--   0        0        0     7029 2023-06-14 17:13:24.233681 slingshot_ai-0.0.10/src/slingshot/cli/shared/prompt.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.738086 slingshot_ai-0.0.10/src/slingshot/cli/shared/py.typed
--rw-r--r--   0        0        0      191 2023-06-08 13:51:24.738326 slingshot_ai-0.0.10/src/slingshot/cli/shared/settings.py
--rw-r--r--   0        0        0     5465 2023-06-20 04:02:42.853816 slingshot_ai-0.0.10/src/slingshot/cli/shared/utils.py
--rw-r--r--   0        0        0     1388 2023-06-08 13:51:24.738677 slingshot_ai-0.0.10/src/slingshot/cli/volume.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.738829 slingshot_ai-0.0.10/src/slingshot/code/__init__.py
--rw-r--r--   0        0        0        1 2023-06-08 13:51:24.739138 slingshot_ai-0.0.10/src/slingshot/code/annotation.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.739256 slingshot_ai-0.0.10/src/slingshot/code/py.typed
--rw-r--r--   0        0        0       56 2023-06-14 01:36:51.755302 slingshot_ai-0.0.10/src/slingshot/inference_model/__init__.py
--rw-r--r--   0        0        0     3941 2023-06-14 14:56:40.736423 slingshot_ai-0.0.10/src/slingshot/inference_model/inference_model.py
--rw-r--r--   0        0        0      205 2023-06-08 13:51:24.739905 slingshot_ai-0.0.10/src/slingshot/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740119 slingshot_ai-0.0.10/src/slingshot/schemas/generated/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740282 slingshot_ai-0.0.10/src/slingshot/schemas/generated/py.typed
--rw-r--r--   0        0        0    26116 2023-06-21 21:30:09.000000 slingshot_ai-0.0.10/src/slingshot/schemas/generated/schemas.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740843 slingshot_ai-0.0.10/src/slingshot/schemas/py.typed
--rw-r--r--   0        0        0    10225 2023-06-16 15:08:48.212246 slingshot_ai-0.0.10/src/slingshot/schemas/schema_extensions.py
--rw-r--r--   0        0        0    14117 2023-06-16 15:08:48.212870 slingshot_ai-0.0.10/src/slingshot/schemas/slingshot-schema.config.json
--rw-r--r--   0        0        0    18799 2023-06-16 15:08:48.213686 slingshot_ai-0.0.10/src/slingshot/schemas/slingshot_schema.py
--rw-r--r--   0        0        0       83 2023-06-08 13:51:24.742135 slingshot_ai-0.0.10/src/slingshot/sdk/__init__.py
--rw-r--r--   0        0        0    41081 2023-06-23 17:35:28.189726 slingshot_ai-0.0.10/src/slingshot/sdk/apply.py
--rw-r--r--   0        0        0     2217 2023-06-08 13:51:24.742861 slingshot_ai-0.0.10/src/slingshot/sdk/auth.py
--rw-r--r--   0        0        0     2075 2023-06-08 13:51:24.743078 slingshot_ai-0.0.10/src/slingshot/sdk/config.py
--rw-r--r--   0        0        0     1856 2023-06-14 17:13:24.234357 slingshot_ai-0.0.10/src/slingshot/sdk/config_utils.py
--rw-r--r--   0        0        0     5334 2023-06-08 13:51:24.743481 slingshot_ai-0.0.10/src/slingshot/sdk/errors.py
--rw-r--r--   0        0        0      126 2023-06-08 13:51:24.743741 slingshot_ai-0.0.10/src/slingshot/sdk/graphql/__init__.py
--rw-r--r--   0        0        0     3293 2023-06-08 13:51:24.743943 slingshot_ai-0.0.10/src/slingshot/sdk/graphql/base_graphql.py
--rw-r--r--   0        0        0    18105 2023-06-20 04:02:56.089500 slingshot_ai-0.0.10/src/slingshot/sdk/graphql/fragments.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.744284 slingshot_ai-0.0.10/src/slingshot/sdk/graphql/py.typed
--rw-r--r--   0        0        0      138 2023-06-08 13:51:24.744487 slingshot_ai-0.0.10/src/slingshot/sdk/graphql/queries/__init__.py
--rw-r--r--   0        0        0     5265 2023-06-08 13:51:24.744644 slingshot_ai-0.0.10/src/slingshot/sdk/graphql/queries/apps.py
--rw-r--r--   0        0        0      986 2023-06-08 13:51:24.744887 slingshot_ai-0.0.10/src/slingshot/sdk/graphql/queries/deployment.py
--rw-r--r--   0        0        0     3671 2023-06-08 13:51:24.745123 slingshot_ai-0.0.10/src/slingshot/sdk/graphql/queries/environment.py
--rw-r--r--   0        0        0     5815 2023-06-19 14:30:19.024645 slingshot_ai-0.0.10/src/slingshot/sdk/graphql/queries/project.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.745499 slingshot_ai-0.0.10/src/slingshot/sdk/graphql/queries/py.typed
--rw-r--r--   0        0        0     2388 2023-06-08 13:51:24.745704 slingshot_ai-0.0.10/src/slingshot/sdk/graphql/queries/run.py
--rw-r--r--   0        0        0     3578 2023-06-08 13:51:24.745899 slingshot_ai-0.0.10/src/slingshot/sdk/graphql/queries/storage.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.745963 slingshot_ai-0.0.10/src/slingshot/sdk/py.typed
--rw-r--r--   0        0        0    48274 2023-06-20 21:48:49.559792 slingshot_ai-0.0.10/src/slingshot/sdk/slingshot_api.py
--rw-r--r--   0        0        0    51597 2023-06-20 21:48:49.560762 slingshot_ai-0.0.10/src/slingshot/sdk/slingshot_sdk.py
--rw-r--r--   0        0        0     5420 2023-06-08 13:51:24.747044 slingshot_ai-0.0.10/src/slingshot/sdk/sync.py
--rw-r--r--   0        0        0     2862 2023-06-08 13:51:24.747244 slingshot_ai-0.0.10/src/slingshot/sdk/upload_download_utils.py
--rw-r--r--   0        0        0     2876 2023-06-14 14:56:40.739250 slingshot_ai-0.0.10/src/slingshot/sdk/utils.py
--rw-r--r--   0        0        0     4368 2023-06-08 13:51:24.747645 slingshot_ai-0.0.10/src/slingshot/sdk/web_path_util.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.747738 slingshot_ai-0.0.10/src/slingshot/shared/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.747833 slingshot_ai-0.0.10/src/slingshot/shared/py.typed
--rw-r--r--   0        0        0     3016 2023-06-08 13:51:24.748010 slingshot_ai-0.0.10/src/slingshot/shared/utils.py
--rw-r--r--   0        0        0       23 2023-06-23 17:35:42.015148 slingshot_ai-0.0.10/src/slingshot/slingshot_version.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.748427 slingshot_ai-0.0.10/src/slingshot/templates/__init__.py
--rw-r--r--   0        0        0     1206 2023-06-14 14:56:40.739937 slingshot_ai-0.0.10/src/slingshot/templates/inference_template.py
--rw-r--r--   0        0        0     1090 2023-06-08 13:51:24.748859 slingshot_ai-0.0.10/src/slingshot/templates/label_studio_data_export_template.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.748968 slingshot_ai-0.0.10/src/slingshot/templates/py.typed
--rw-r--r--   0        0        0      867 1970-01-01 00:00:00.000000 slingshot_ai-0.0.10/PKG-INFO
+-rw-r--r--   0        0        0      828 2023-06-27 16:29:44.921114 slingshot_ai-0.0.11/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-06-14 01:36:51.753575 slingshot_ai-0.0.11/src/slingshot/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.733834 slingshot_ai-0.0.11/src/slingshot/cli/__init__.py
+-rw-r--r--   0        0        0    17667 2023-06-27 15:26:50.732097 slingshot_ai-0.0.11/src/slingshot/cli/add.py
+-rw-r--r--   0        0        0     2091 2023-06-27 15:26:50.733379 slingshot_ai-0.0.11/src/slingshot/cli/apply.py
+-rw-r--r--   0        0        0     5723 2023-06-26 18:48:01.304541 slingshot_ai-0.0.11/src/slingshot/cli/apps.py
+-rw-r--r--   0        0        0     5916 2023-06-20 21:48:49.557285 slingshot_ai-0.0.11/src/slingshot/cli/artifact.py
+-rw-r--r--   0        0        0     5263 2023-06-27 15:26:50.737721 slingshot_ai-0.0.11/src/slingshot/cli/auth.py
+-rw-r--r--   0        0        0      970 2023-06-08 13:51:24.734880 slingshot_ai-0.0.11/src/slingshot/cli/code.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:23:44.406584 slingshot_ai-0.0.11/src/slingshot/cli/config/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.734966 slingshot_ai-0.0.11/src/slingshot/cli/config/py.typed
+-rw-r--r--   0        0        0      850 2023-06-14 16:35:36.287763 slingshot_ai-0.0.11/src/slingshot/cli/config/sentry_setup.py
+-rw-r--r--   0        0        0    13774 2023-06-27 15:26:50.739279 slingshot_ai-0.0.11/src/slingshot/cli/config/slingshot_cli.py
+-rw-r--r--   0        0        0     1234 2023-06-08 13:51:24.735333 slingshot_ai-0.0.11/src/slingshot/cli/dev.py
+-rw-r--r--   0        0        0     1123 2023-06-23 17:35:28.186738 slingshot_ai-0.0.11/src/slingshot/cli/environment.py
+-rw-r--r--   0        0        0     4519 2023-06-13 20:59:00.706466 slingshot_ai-0.0.11/src/slingshot/cli/inference.py
+-rw-r--r--   0        0        0     3059 2023-06-08 13:51:24.735634 slingshot_ai-0.0.11/src/slingshot/cli/logs.py
+-rw-r--r--   0        0        0     2694 2023-06-27 15:26:50.740752 slingshot_ai-0.0.11/src/slingshot/cli/main.py
+-rw-r--r--   0        0        0     2433 2023-06-27 15:26:50.741510 slingshot_ai-0.0.11/src/slingshot/cli/project.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.735998 slingshot_ai-0.0.11/src/slingshot/cli/py.typed
+-rw-r--r--   0        0        0     7855 2023-06-27 15:26:50.742904 slingshot_ai-0.0.11/src/slingshot/cli/run.py
+-rw-r--r--   0        0        0     3648 2023-06-08 14:01:51.180092 slingshot_ai-0.0.11/src/slingshot/cli/secret.py
+-rw-r--r--   0        0        0     3816 2023-06-15 18:10:07.073951 slingshot_ai-0.0.11/src/slingshot/cli/session.py
+-rw-r--r--   0        0        0       67 2023-06-08 13:51:24.737453 slingshot_ai-0.0.11/src/slingshot/cli/shared/__init__.py
+-rw-r--r--   0        0        0     6260 2023-06-20 21:48:49.557743 slingshot_ai-0.0.11/src/slingshot/cli/shared/code_sync.py
+-rw-r--r--   0        0        0     7029 2023-06-23 22:54:16.040274 slingshot_ai-0.0.11/src/slingshot/cli/shared/prompt.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.738086 slingshot_ai-0.0.11/src/slingshot/cli/shared/py.typed
+-rw-r--r--   0        0        0      191 2023-06-08 13:51:24.738326 slingshot_ai-0.0.11/src/slingshot/cli/shared/settings.py
+-rw-r--r--   0        0        0     6085 2023-06-27 15:26:50.745160 slingshot_ai-0.0.11/src/slingshot/cli/shared/utils.py
+-rw-r--r--   0        0        0     1388 2023-06-08 13:51:24.738677 slingshot_ai-0.0.11/src/slingshot/cli/volume.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.738829 slingshot_ai-0.0.11/src/slingshot/code/__init__.py
+-rw-r--r--   0        0        0        1 2023-06-08 13:51:24.739138 slingshot_ai-0.0.11/src/slingshot/code/annotation.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.739256 slingshot_ai-0.0.11/src/slingshot/code/py.typed
+-rw-r--r--   0        0        0       56 2023-06-14 01:36:51.755302 slingshot_ai-0.0.11/src/slingshot/inference_model/__init__.py
+-rw-r--r--   0        0        0     3941 2023-06-14 14:56:40.736423 slingshot_ai-0.0.11/src/slingshot/inference_model/inference_model.py
+-rw-r--r--   0        0        0      205 2023-06-08 13:51:24.739905 slingshot_ai-0.0.11/src/slingshot/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740119 slingshot_ai-0.0.11/src/slingshot/schemas/generated/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740282 slingshot_ai-0.0.11/src/slingshot/schemas/generated/py.typed
+-rw-r--r--   0        0        0    26055 2023-06-27 16:31:46.000000 slingshot_ai-0.0.11/src/slingshot/schemas/generated/schemas.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740843 slingshot_ai-0.0.11/src/slingshot/schemas/py.typed
+-rw-r--r--   0        0        0    10181 2023-06-27 15:26:50.747432 slingshot_ai-0.0.11/src/slingshot/schemas/schema_extensions.py
+-rw-r--r--   0        0        0    14117 2023-06-16 15:08:48.212870 slingshot_ai-0.0.11/src/slingshot/schemas/slingshot-schema.config.json
+-rw-r--r--   0        0        0    18799 2023-06-23 23:16:10.617109 slingshot_ai-0.0.11/src/slingshot/schemas/slingshot_schema.py
+-rw-r--r--   0        0        0       83 2023-06-08 13:51:24.742135 slingshot_ai-0.0.11/src/slingshot/sdk/__init__.py
+-rw-r--r--   0        0        0    44847 2023-06-27 15:26:50.748414 slingshot_ai-0.0.11/src/slingshot/sdk/apply.py
+-rw-r--r--   0        0        0     2217 2023-06-08 13:51:24.742861 slingshot_ai-0.0.11/src/slingshot/sdk/auth.py
+-rw-r--r--   0        0        0     2073 2023-06-27 15:26:50.749266 slingshot_ai-0.0.11/src/slingshot/sdk/config.py
+-rw-r--r--   0        0        0     1856 2023-06-14 17:13:24.234357 slingshot_ai-0.0.11/src/slingshot/sdk/config_utils.py
+-rw-r--r--   0        0        0     5334 2023-06-08 13:51:24.743481 slingshot_ai-0.0.11/src/slingshot/sdk/errors.py
+-rw-r--r--   0        0        0      126 2023-06-08 13:51:24.743741 slingshot_ai-0.0.11/src/slingshot/sdk/graphql/__init__.py
+-rw-r--r--   0        0        0     3293 2023-06-08 13:51:24.743943 slingshot_ai-0.0.11/src/slingshot/sdk/graphql/base_graphql.py
+-rw-r--r--   0        0        0    18027 2023-06-27 15:26:50.750182 slingshot_ai-0.0.11/src/slingshot/sdk/graphql/fragments.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.744284 slingshot_ai-0.0.11/src/slingshot/sdk/graphql/py.typed
+-rw-r--r--   0        0        0      138 2023-06-08 13:51:24.744487 slingshot_ai-0.0.11/src/slingshot/sdk/graphql/queries/__init__.py
+-rw-r--r--   0        0        0     5265 2023-06-08 13:51:24.744644 slingshot_ai-0.0.11/src/slingshot/sdk/graphql/queries/apps.py
+-rw-r--r--   0        0        0      986 2023-06-08 13:51:24.744887 slingshot_ai-0.0.11/src/slingshot/sdk/graphql/queries/deployment.py
+-rw-r--r--   0        0        0     3671 2023-06-08 13:51:24.745123 slingshot_ai-0.0.11/src/slingshot/sdk/graphql/queries/environment.py
+-rw-r--r--   0        0        0     5247 2023-06-27 15:26:50.751307 slingshot_ai-0.0.11/src/slingshot/sdk/graphql/queries/project.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.745499 slingshot_ai-0.0.11/src/slingshot/sdk/graphql/queries/py.typed
+-rw-r--r--   0        0        0     2388 2023-06-08 13:51:24.745704 slingshot_ai-0.0.11/src/slingshot/sdk/graphql/queries/run.py
+-rw-r--r--   0        0        0     3578 2023-06-08 13:51:24.745899 slingshot_ai-0.0.11/src/slingshot/sdk/graphql/queries/storage.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.745963 slingshot_ai-0.0.11/src/slingshot/sdk/py.typed
+-rw-r--r--   0        0        0    47781 2023-06-27 15:26:50.752556 slingshot_ai-0.0.11/src/slingshot/sdk/slingshot_api.py
+-rw-r--r--   0        0        0    51898 2023-06-27 15:26:50.753607 slingshot_ai-0.0.11/src/slingshot/sdk/slingshot_sdk.py
+-rw-r--r--   0        0        0     5420 2023-06-08 13:51:24.747044 slingshot_ai-0.0.11/src/slingshot/sdk/sync.py
+-rw-r--r--   0        0        0     2862 2023-06-08 13:51:24.747244 slingshot_ai-0.0.11/src/slingshot/sdk/upload_download_utils.py
+-rw-r--r--   0        0        0     2876 2023-06-14 14:56:40.739250 slingshot_ai-0.0.11/src/slingshot/sdk/utils.py
+-rw-r--r--   0        0        0     4348 2023-06-27 15:26:50.754696 slingshot_ai-0.0.11/src/slingshot/sdk/web_path_util.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.747738 slingshot_ai-0.0.11/src/slingshot/shared/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.747833 slingshot_ai-0.0.11/src/slingshot/shared/py.typed
+-rw-r--r--   0        0        0     3016 2023-06-08 13:51:24.748010 slingshot_ai-0.0.11/src/slingshot/shared/utils.py
+-rw-r--r--   0        0        0       23 2023-06-27 16:31:38.208032 slingshot_ai-0.0.11/src/slingshot/slingshot_version.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.748427 slingshot_ai-0.0.11/src/slingshot/templates/__init__.py
+-rw-r--r--   0        0        0     1206 2023-06-14 14:56:40.739937 slingshot_ai-0.0.11/src/slingshot/templates/inference_template.py
+-rw-r--r--   0        0        0     1090 2023-06-08 13:51:24.748859 slingshot_ai-0.0.11/src/slingshot/templates/label_studio_data_export_template.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.748968 slingshot_ai-0.0.11/src/slingshot/templates/py.typed
+-rw-r--r--   0        0        0      867 1970-01-01 00:00:00.000000 slingshot_ai-0.0.11/PKG-INFO
```

### Comparing `slingshot_ai-0.0.10/pyproject.toml` & `slingshot_ai-0.0.11/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
-name = "slingshot"
-version = "0.0.10"
+name = "slingshot-ai"
+version = "0.0.11"
 
 [tool.poetry]
 name = "slingshot-ai"
-version = "0.0.10"
+version = "0.0.11"
 description = ""
 authors = ["Slingshot AI <service-account@slingshot.xyz>"]
 packages = [ { include = "slingshot", from = "src" } ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = ">=3.8.1"
```

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/add.py` & `slingshot_ai-0.0.11/src/slingshot/cli/add.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 import json
+import re
 import shutil
+import uuid
 from pathlib import Path
 from typing import Any, Callable, Literal, Optional, Type, cast
 
 import typer
 from pydantic import BaseModel, ValidationError
 from ruamel import yaml as r_yaml
 
@@ -34,61 +36,69 @@
 
 
 def pydantic_to_dict(pydantic: BaseModel) -> dict[str, Any]:
     # Convert enums to strings
     return json.loads(pydantic.json(exclude_none=True))
 
 
+def _display_name_to_id(input_str: str) -> str:
+    """Converts a name to a valid project ID by removing special characters and replacing spaces with hyphens."""
+    lower = input_str.strip().lower()
+    single_space = re.sub(r"\s+", "-", lower)
+    single_hyphen = re.sub(r"-+", "-", single_space)
+    alphanumeric_hyphen_underscore = re.sub(r"[^a-z0-9-_]", "", single_hyphen)
+    return alphanumeric_hyphen_underscore
+
+
 async def _create_project(sdk: SlingshotSDK) -> str:
-    display_name = None
-    slug = None
+    new_id = None
+    display_name = typer.prompt("Enter a name for your project")
+    project_id_default = _display_name_to_id(display_name) + "-" + uuid.uuid4().hex[:5]
     while True:
-        display_name = display_name or typer.prompt("Enter a name for your project")
-        project_slug_default = display_name.lower().replace(" ", "-")
-        slug = slug or typer.prompt("Enter a slug for your project (used for URLs)", default=project_slug_default)
+        # Replace multiple spaces with a single space and spaces with hyphens
+        new_id = new_id or typer.prompt("Enter an ID for your project (used for URLs)", default=project_id_default)
         try:
-            project_response = await sdk.create_project(slug, display_name=display_name)
+            project_response = await sdk.create_project(new_id, display_name=display_name)
             if project_response.error:
                 console.print(f"[red]Error creating project[/red]: {project_response.error.message}")
                 display_name = None
-                slug = None
+                new_id = None
                 continue
-            assert project_response.data is not None
 
-            await sdk.use_project(slug)
-            console.print(f"Created project: {slug}")
-            await sdk.use_project(slug)
-            return slug
+            assert project_response.data is not None
+            console.print(f"Created project: {new_id}")
+            await sdk.use_project(project_response.data.project_id)
+            return project_response.data.project_id
         except ValidationError as e:
             for error in e.errors():
                 loc = error['loc']
-                if loc[0] == 'project_slug':
-                    console.print(f"[red]Slug is invalid[/red]: {error['msg']}")
-                    slug = None
+                if loc[0] == 'project_id':
+                    console.print(f"[red]Project ID is invalid[/red]: {error['msg']}")
+                    new_id = None
                 if loc[0] == 'project_display_name':
                     console.print(f"[red]Project name is invalid[/red]: {error['msg']}")
                     display_name = None
 
 
 @app.command(requires_auth=False, requires_project=False, top_level=True, name="init")
 async def init(*, sdk: SlingshotSDK) -> None:
     """Initialize a new project in the current directory"""
-    if not sdk.project_name:
-        # TODO: Doesn't handle the case where you want to create a new project
+    if not sdk.project_id:
         if prompt_confirm("No project selected. Do you want to create a new one?", default=False):
             await _create_project(sdk)
         else:
             "Okay, skipping. To use an existing project, run 'slingshot use'"
 
     # Check if the slingshot.yaml exists
     if client_settings.slingshot_config_path.exists() and client_settings.slingshot_config_path.stat().st_size > 0:
         console.print(
             "This project already has a `slingshot yaml`. You can add components to it with [bold]slingshot add[/bold]"
         )
         if not typer.confirm("Do you want to reinitialize this project from scratch?"):
+            await sdk.apply_project(and_wait=True)
             return
 
     # Touch the file
     client_settings.slingshot_config_path.touch()
 
     # Insert an empty schemas.SlingshotAppSpec
     doc = pydantic_to_dict(slingshot_yaml_schemas.ProjectManifest())
@@ -132,22 +142,22 @@
     if not await sdk.is_signed_in():
         console.print(
             "Skipping apply because you are not logged in. You can run 'slingshot login' and then "
             "'slingshot apply' later."
         )
         return
 
-    if not sdk.project_name:
+    if not sdk.project_id:
         console.print(
             "Skipping apply because your project is not set. You can run 'slingshot use' and then "
             "'slingshot apply' later."
         )
         return
 
-    await sdk.use_project(sdk.project_name)
+    await sdk.use_project(sdk.project_id)
     await sdk.apply_project()
 
 
 def _create_new_environment(name: str | None = None) -> str:
     current = load_slingshot_project_config()  # For raising if absent
     if not current:
         raise SlingshotException("No Slingshot manifest found. Run 'slingshot init' first.")
@@ -185,30 +195,30 @@
         if "environments" not in doc:
             doc["environments"] = {}
         doc["environments"][name] = pydantic_to_dict(environment)
     console.print(f"Environment '{name}' added", style="green")
     return name
 
 
-def _create_session() -> str:
+def _create_session(name: str | None = None) -> str:
     current = load_slingshot_project_config()
 
     current_session_environments = [
         key
         for key, value in current.environments.items()
         if any("jupyterlab" in package for package in value.python_packages)
     ]
 
     # Select an environment or create one if none exist
     env_name = _choose_or_create_environment(
         current_session_environments, new_env_name="session-env", new_env_auto_packages=["jupyterlab>=3.5.0"]
     )
 
     # Add a new session app if it doesn't already exist
-    app_name = "session"
+    app_name = name or typer.prompt("Name of the session", default="session")
     if any(existing_app.name == app_name for existing_app in current.apps):
         console.print(f"App '{app_name}' already exists, skipping creation", style="yellow")
     else:
         session_app = schemas.SessionAppSpec(name=app_name, environment=env_name, using="session")
         current.apps.append(session_app)
         with edit_slingshot_yaml() as doc:
             if not doc.get("apps"):
```

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/apply.py` & `slingshot_ai-0.0.11/src/slingshot/cli/apply.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,29 @@
     Applies the slingshot.yaml file in the current directory to the project on Slingshot
     """
     any_changes = await sdk.apply_project(and_wait=True, force=y)
     if not any_changes:
         console.print("No changes pushed")
 
 
+@app.command(name="pull", requires_project=True, top_level=True, requires_auth=True)
+async def pull(
+    *, sdk: SlingshotSDK, y: bool = typer.Option(False, "--yes", "-y", help="Skip confirmation and apply changes")
+) -> None:
+    """Pull the slingshot.yaml file to the current project
+
+    Pulls the slingshot.yaml file in the current directory to the project on Slingshot
+    """
+    any_changes_applied = await sdk.apply_to_local(force=y)
+    if not any_changes_applied:
+        console.print("No changes pulled")
+    else:
+        console.print("Changes pulled successfully")
+
+
 @app.command(name="plan", requires_project=True, top_level=True, requires_auth=True, hidden=True)
 async def plan(*, sdk: SlingshotSDK) -> None:
     """Plan what changes would be applied by the slingshot.yaml file, but don't apply them"""
     manifest = load_slingshot_project_config()
     remote_manifest = await remote_project_manifest(sdk)
 
     diff = DeepDiff(json.loads(remote_manifest.json()), json.loads(manifest.json()), ignore_order=True)
```

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/apps.py` & `slingshot_ai-0.0.11/src/slingshot/cli/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,16 +39,23 @@
         filter_fn = filter_for_sessions if sessions else filter_for_apps
         id_and_name_or_none = await prompt_for_app_spec(
             sdk, filter_fn, app_display_name='session' if sessions else 'app', raise_if_missing=False
         )
         if id_and_name_or_none:
             _, name = id_and_name_or_none
         elif sessions:
+            console.print("Creating a new session")
             name = _create_session()
             await sdk.apply_project(force=applied)  # If applied, the user was already prompted. Just quietly apply.
+
+            # If the user doesn't apply the prompt with the session, exit because there will not be a session to start.
+            all_app_specs = await sdk.list_apps()
+            session_specs = [app_spec for app_spec in all_app_specs if app_spec.app_type == schemas.AppType.SESSION]
+            if not session_specs:
+                raise SlingshotException("Session not created, exiting")
         else:
             raise typer.Exit(1)
 
     app_instance = await sdk.start_app(app_name=name, source_code_id=source_code_id)
     url = await sdk.web_path_util.app(app_spec=app_instance.app_spec_id)
     console.print(f"Starting app '{name}'. See details here: {url}")
```

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/artifact.py` & `slingshot_ai-0.0.11/src/slingshot/cli/artifact.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/auth.py` & `slingshot_ai-0.0.11/src/slingshot/cli/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,22 +46,22 @@
     console.print(f"Logged in successfully as {user.username}!")
     if not user.ssh_public_key:
         console.print(
             "You don't have an SSH public key set. You can set one by running 'slingshot auth set-ssh'", style="yellow"
         )
 
     await sdk.setup()
-    if sdk.project_name and any(p.project_name == sdk.project_name for p in user.projects):
-        await sdk.use_project(sdk.project_name)
-        console.print(f"Project is set to '{sdk.project_name}'.")
+    if sdk.project_id and any(p.project_id == sdk.project_id for p in user.projects):
+        await sdk.use_project(sdk.project_id)
+        console.print(f"Project is set to '{sdk.project_id}'.")
         return
 
     choice = prompt_confirm(f"Do you want to track an existing project?", default=False)
     if choice:
-        await project.list_and_set_project_name(sdk)
+        await project.list_and_set_project_id(sdk)
     else:
         console.print("You can run `slingshot open` to create a new project from the UI")
 
 
 @app.command("logout", requires_auth=False, requires_project=False, top_level=True)
 async def logout(sdk: SlingshotSDK) -> None:
     """Log out of Slingshot"""
```

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/code.py` & `slingshot_ai-0.0.11/src/slingshot/cli/code.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/config/sentry_setup.py` & `slingshot_ai-0.0.11/src/slingshot/cli/config/sentry_setup.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/config/slingshot_cli.py` & `slingshot_ai-0.0.11/src/slingshot/cli/config/slingshot_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 from typing_extensions import ParamSpec
 
 from ...sdk import SlingshotSDK
 from ...sdk.config import project_config
 from ...sdk.errors import SlingshotException, SlingshotUnauthenticatedError
 from ...sdk.utils import console
 
-PROJECT_NAME_OPTION_HELPER_TEXT = "Project name must be specified or configured in .slingshot/config.json."
-PROJECT_NAME_NOT_FOUND_MSG = f"No project name found. Configure it with 'slingshot use'."
-PROJECT_OPTION = typer.Option(None, "--project-name", "--project", "-p", help=PROJECT_NAME_OPTION_HELPER_TEXT)
+PROJECT_ID_OPTION_HELPER_TEXT = "Project name must be specified or configured in .slingshot/config.json."
+PROJECT_ID_NOT_FOUND_MSG = f"No project name found. Configure it with 'slingshot use'."
+PROJECT_OPTION = typer.Option(None, "--project-id", "--project", "-p", help=PROJECT_ID_OPTION_HELPER_TEXT)
 
 
 class SlingshotCLICommand:
-    PROJECT_NAME_PARAM = inspect.Parameter(
-        "project_name", kind=inspect.Parameter.KEYWORD_ONLY, annotation=Optional[str], default=PROJECT_OPTION
+    PROJECT_ID_PARAM = inspect.Parameter(
+        "project_id", kind=inspect.Parameter.KEYWORD_ONLY, annotation=Optional[str], default=PROJECT_OPTION
     )
 
     def __init__(
         self,
         name: str | None = None,
         top_level: bool = False,
         inject_sdk: bool | None = None,
@@ -114,20 +114,20 @@
                             )
                             if me.user and not me.user.is_activated:
                                 raise SlingshotException(
                                     "Your account is not yet activated. "
                                     "Contact Slingshot support to move up your spot on the waiting list!"
                                 )
                     if self._requires_project is True:
-                        project_name = kwargs.pop("project_name", None) or project_config.project_name
-                        if not project_name:
-                            raise SlingshotException(PROJECT_NAME_NOT_FOUND_MSG)
+                        project_id = kwargs.pop("project_id", None) or project_config.project_id
+                        if not project_id:
+                            raise SlingshotException(PROJECT_ID_NOT_FOUND_MSG)
 
-                        await sdk.use_project(project_name)
-                        scope.set_tag("project_name", project_name)
+                        await sdk.use_project(project_id)
+                        scope.set_tag("project_id", project_id)
 
                     if self._inject_sdk is True:
                         kwargs["sdk"] = sdk
                         async with sdk.use_session():
                             return await func(*args, **kwargs)
                     return await func(*args, **kwargs)
                 except SlingshotException as e:
@@ -142,15 +142,15 @@
         parameters = oldsig.parameters.copy()
         # Hide parameters from Typer:
         if self._inject_sdk:
             assert "sdk" in parameters, "Cannot inject SDK because `sdk` does not appear in the function's signature"
             del parameters["sdk"]
 
         if self._requires_project:
-            parameters["project_name"] = self.PROJECT_NAME_PARAM
+            parameters["project_id"] = self.PROJECT_ID_PARAM
 
         verbose_param = inspect.Parameter(
             "verbose",
             kind=inspect.Parameter.KEYWORD_ONLY,
             annotation=bool,
             default=typer.Option(False, "--verbose", "-v"),
         )
```

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/dev.py` & `slingshot_ai-0.0.11/src/slingshot/cli/dev.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/environment.py` & `slingshot_ai-0.0.11/src/slingshot/cli/environment.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/inference.py` & `slingshot_ai-0.0.11/src/slingshot/cli/inference.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/logs.py` & `slingshot_ai-0.0.11/src/slingshot/cli/logs.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/main.py` & `slingshot_ai-0.0.11/src/slingshot/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 cli = SlingshotCLIApp(no_args_is_help=True, help=f"Slingshot AI CLI 🚀 ({__version__})")
 
 cli.add_command(add.add_component)
 cli.add_command(add.init)
 cli.add_command(apply.apply)
 cli.add_command(apply.plan)
+cli.add_command(apply.pull)
 cli.add_command(logs.logs)
 
 cli.add_subcommands(auth.app, name="auth", help="Authenticate with Slingshot 👋", no_args_is_help=True)
 cli.add_subcommands(artifact.app, name="artifact", help="Manage artifacts 💾", no_args_is_help=True)
 cli.add_subcommands(code.app, name="code", help="Manage and push code 👩‍💻", no_args_is_help=True)
 cli.add_subcommands(environment.app, name="environment", help="Manage environments 🌱", no_args_is_help=True)
 cli.add_subcommands(project.app, name="project", help="Manage your Slingshot project 📊", no_args_is_help=True)
```

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/project.py` & `slingshot_ai-0.0.11/src/slingshot/cli/project.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,54 +20,54 @@
 async def list_projects(sdk: SlingshotSDK) -> None:
     """Lists all projects that the current user has access to."""
     projects = await sdk.list_projects()
     table = Table(title="Projects")
     table.add_column("Name", style="cyan")
     table.add_column("Project ID", style="cyan")
     for i, project in enumerate(projects):
-        table.add_row(project.display_name, project.project_name)
+        table.add_row(project.display_name, project.project_id)
     console.print(table)
 
 
 @app.command("open", requires_project=True)
 async def open_project(sdk: SlingshotSDK) -> None:
     """
     Opens the project in your default browser.
     """
     url = await sdk.web_path_util.project()
     console.print(f"Opening project in browser: [link={url}]{url}[/link]")
     typer.launch(url)
 
 
 @app.command("use", requires_auth=True, requires_project=False, top_level=True)
-async def set_tracked_project(project_name: Optional[str] = typer.Argument(None), *, sdk: SlingshotSDK) -> None:
+async def set_tracked_project(project_id: Optional[str] = typer.Argument(None), *, sdk: SlingshotSDK) -> None:
     """
     Select which project to use for the current directory.
     """
-    if project_name:
-        _set_project_name(project_name)
+    if project_id:
+        _set_project_id(project_id)
         return
-    await list_and_set_project_name(sdk)
+    await list_and_set_project_id(sdk)
 
 
-async def list_and_set_project_name(sdk: SlingshotSDK) -> None:
+async def list_and_set_project_id(sdk: SlingshotSDK) -> None:
     me = await sdk.me()
     if not me:
         raise SlingshotException("You must be logged in to use this command.")
     projects = me.projects
     if not projects:
         console.print("No projects found.")
         return  # Can't set a project ID if user has no projects
     choice = prompt_for_single_choice(
-        f"Select the project you want to work on", [i.project_name for i in projects], skip_if_one_value=True
+        f"Select the project you want to work on", [i.project_id for i in projects], skip_if_one_value=True
     )
 
-    project_name = projects[choice].project_name
-    _set_project_name(project_name)
+    project_id = projects[choice].project_id
+    _set_project_id(project_id)
 
 
-def _set_project_name(project_name: str) -> None:
-    old_project_name = project_config.project_name
-    project_config.project_name = project_name
-    if old_project_name != project_name:
+def _set_project_id(project_id: str) -> None:
+    old_project_id = project_config.project_id
+    project_config.project_id = project_id
+    if old_project_id != project_id:
         project_config.last_pushed_manifest = None
-    console.print(f"This directory is now associated with the project: [bold]{project_name}[/bold]")
+    console.print(f"This directory is now associated with the project: [bold]{project_id}[/bold]")
```

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/run.py` & `slingshot_ai-0.0.11/src/slingshot/cli/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 
 @app.command("list", requires_project=True)
 async def list_runs(sdk: SlingshotSDK) -> None:
     """List all runs in the project."""
     runs = await sdk.list_runs()
     if not runs:
         console.print(
-            "No runs found!"
+            "No runs found! "
             "Edit [yellow]slingshot.yaml[/yellow] or use [yellow]slingshot add[/yellow] to add a run template."
         )
         return
 
     table = Table(title="Runs")
     table.add_column("Run Name", style="cyan")
     table.add_column("Status", style="cyan")
```

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/secret.py` & `slingshot_ai-0.0.11/src/slingshot/cli/secret.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/session.py` & `slingshot_ai-0.0.11/src/slingshot/cli/session.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/shared/code_sync.py` & `slingshot_ai-0.0.11/src/slingshot/cli/shared/code_sync.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/shared/prompt.py` & `slingshot_ai-0.0.11/src/slingshot/cli/shared/prompt.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/shared/utils.py` & `slingshot_ai-0.0.11/src/slingshot/cli/shared/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -28,23 +28,39 @@
 
 async def follow_run_logs_until_done(sdk: SlingshotSDK, run_id: str) -> schemas.JobStatus:
     task_logs = asyncio.create_task(sdk.print_logs(run_id=run_id, follow=True))
     task_status = asyncio.create_task(_wait_for_run_finished(sdk=sdk, run_id=run_id))
     done, pending = await asyncio.wait([task_logs, task_status], return_when=asyncio.FIRST_COMPLETED)
     for task in pending:
         task.cancel()
+
+    # If task_status was cancelled or raised an exception, handle it
+    if task_status.cancelled():
+        raise SlingshotException("Something went wrong following logs")
+    elif exception := task_status.exception() is not None:
+        assert isinstance(exception, BaseException)
+        raise exception
+
     return task_status.result()
 
 
 async def follow_app_logs_until_ready(sdk: SlingshotSDK, app_spec_id: str) -> schemas.AppInstanceStatus:
     task_logs = asyncio.create_task(sdk.print_logs(app_spec_id=app_spec_id, follow=True))
     task_status = asyncio.create_task(_wait_for_app_ready(sdk=sdk, app_spec_id=app_spec_id))
     done, pending = await asyncio.wait([task_logs, task_status], return_when=asyncio.FIRST_COMPLETED)
     for task in pending:
         task.cancel()
+
+    # If task_status was cancelled or raised an exception, handle it
+    if task_status.cancelled():
+        raise SlingshotException("Something went wrong following logs")
+    elif exception := task_status.exception() is not None:
+        assert isinstance(exception, BaseException)
+        raise exception
+
     return task_status.result()
 
 
 def datetime_to_human_readable(dt: datetime) -> str:
     """Assumes UTC datetime and converts to local time in the format of: Mar 2, 2021 1:30AM EST"""
     date_str = dt.strftime('%b %d, %Y %I:%M:%S %p')
     return f'{date_str} UTC'
```

### Comparing `slingshot_ai-0.0.10/src/slingshot/cli/volume.py` & `slingshot_ai-0.0.11/src/slingshot/cli/volume.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/inference_model/inference_model.py` & `slingshot_ai-0.0.11/src/slingshot/inference_model/inference_model.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/schemas/generated/schemas.py` & `slingshot_ai-0.0.11/src/slingshot/schemas/generated/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,20 +79,20 @@
 
 class BodyLoginToken(BaseModel):
     token: str = Field(..., title='Auth0 ID token')
     cli: Optional[bool] = Field(False, title='Cli')
 
 
 class BodyNewProject(BaseModel):
-    project_slug: constr(
+    project_id: constr(
         regex=r'^[A-Za-z][A-Za-z0-9_-]*$', min_length=4, max_length=50
     ) = Field(
         ...,
         description='This is the unique name to be associated with your new project',
-        title='Project Name',
+        title='Project ID',
     )
     display_name: constr(min_length=4, max_length=20) = Field(
         ...,
         description='An optional name for your project that will be shown in the UI',
         title='Display Name',
     )
 
@@ -400,15 +400,14 @@
 
 
 class SourceCode(BaseModel):
     source_code_id: str = Field(..., title='Source Code Id')
     source_code_name: str = Field(..., title='Source Code Name')
     description: Optional[str] = Field(None, title='Description')
     project_id: str = Field(..., title='Project Id')
-    project_name: str = Field(..., title='Project Name')
     created_at: datetime = Field(..., title='Created At')
     blob_artifact: BlobArtifact
 
 
 class SourceCodeResponse(BaseModel):
     data: Optional[SourceCode] = None
     error: Optional[SlingshotLogicalError] = None
```

### Comparing `slingshot_ai-0.0.10/src/slingshot/schemas/schema_extensions.py` & `slingshot_ai-0.0.11/src/slingshot/schemas/schema_extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,21 +97,19 @@
 
     def __str__(self) -> str:
         return self.as_str()
 
 
 class Project(Protocol):
     project_id: str
-    project_name: str
     display_name: str
 
 
 class ProjectImpl(BaseModel):
     project_id: str
-    project_name: str
     display_name: str
 
 
 class HasRunId(Protocol):
     run_id: str
```

### Comparing `slingshot_ai-0.0.10/src/slingshot/schemas/slingshot-schema.config.json` & `slingshot_ai-0.0.11/src/slingshot/schemas/slingshot-schema.config.json`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/schemas/slingshot_schema.py` & `slingshot_ai-0.0.11/src/slingshot/schemas/slingshot_schema.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/sdk/apply.py` & `slingshot_ai-0.0.11/src/slingshot/sdk/apply.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import typer
 from deepdiff import DeepDiff
 from pydantic import parse_obj_as
 
 from slingshot import schemas
 from slingshot.cli.shared import prompt_confirm, prompt_for_single_choice
+from slingshot.schemas import ProjectManifest
 from slingshot.sdk import config
 from slingshot.sdk.errors import SlingshotException
 from slingshot.sdk.graphql import fragments
 from slingshot.sdk.utils import console, edit_slingshot_yaml
 from slingshot.shared.utils import get_data_or_raise, load_slingshot_project_config
 
 if TYPE_CHECKING:
@@ -334,93 +335,143 @@
     async def run(
         self,
         project_manifest: schemas.ProjectManifest,
         env_spec_plan: EnvSpecPlan,
         app_spec_plan: AppSpecPlan,
         and_wait: bool,
     ) -> None:
-        console.print(f"Applying 'slingshot.yaml' for project '{self._project.project_name}'.")
+        console.print(f"Applying 'slingshot.yaml' for project '{self._project.project_id}'.")
         env_specs_to_wait_for, env_spec_name_to_id = await self.apply_env_specs(
             project_manifest, env_spec_plan=env_spec_plan
         )
         await self.apply_app_specs(app_spec_plan=app_spec_plan, env_spec_name_to_id=env_spec_name_to_id)
         config.project_config.last_pushed_manifest = load_slingshot_project_config()
         if and_wait:
+            if env_specs_to_wait_for:
+                console.print("[green]Waiting for environments, you can safely exit with Ctrl+C...[/green]")
             for env in env_specs_to_wait_for:
                 await self._wait_for_environment(env)
 
-    async def apply_to_local(self, remote_manifest: schemas.ProjectManifest | None = None) -> None:
+    async def apply_to_local(self, remote_manifest: schemas.ProjectManifest | None = None, force: bool = False) -> bool:
+        """
+        Applies the remote manifest to the local slingshot.yaml.
+
+        The last pushed manifest is used as the base of the initial diff. If there is no last-pushed manifest,
+        the base is an empty manifest so that all remote changes are computed in the plan and can be applied.
+        Then, the local slingshot.yaml applied using the resulting diff. If there are conflicts, the user is
+        prompted to override either the local or remote changes.
+
+        Returns True if there were changes, False otherwise.
+        """
         current_manifest = load_slingshot_project_config()  # Reload local, in case it was changed
-        last_manifest = config.project_config.last_pushed_manifest
+        last_pushed_manifest = config.project_config.last_pushed_manifest
+        is_last_pushed_manifest_empty = last_pushed_manifest is None
+
+        diff_base = last_pushed_manifest or ProjectManifest()
+        if isinstance(diff_base, ProjectManifest):
+            diff_base = diff_base.dict()
+
         if not remote_manifest:
             remote_manifest = await remote_project_manifest(self._sdk)
-        if last_manifest is None:
-            logger.debug("No last pushed manifest found, skipping pull")
-            # Note that this means we don't yet support creating a slingshot.yaml from the frontend.
-            return
-        diff = DeepDiff(last_manifest, json.loads(remote_manifest.json()), ignore_order=True)
+
+        diff = DeepDiff(diff_base, remote_manifest.dict(), ignore_order=True)
         if not diff:
             logger.debug("No remote changes detected")
-            return
+            return False
 
         console.print("[red]Conflict detected[/red]. Changes found on the remote since your last push:")
         diff_formatted = diff_to_str(diff, remote_manifest)
         diff_formatted = "\n".join([f"  [yellow]*[/yellow] {line}" for line in diff_formatted.split('\n')])
         console.print(diff_formatted)
-        unable_to_synchronise_message = (
-            f"[yellow]Conflict resolution[/yellow]: Unable to synchronise remote changes to your local slingshot.yaml."
-        )
-        if not validate_if_changes_can_be_applied(diff, remote_manifest, current_manifest=current_manifest):
-            console.print(unable_to_synchronise_message)
-            if (
-                prompt_for_single_choice(
-                    "Do you want to use the local or remote version?", ["local", "remote"], default=0
-                )
-                == 1
-            ):
-                apply_to_local(diff, remote_manifest, force=True)
-            config.project_config.last_pushed_manifest = load_slingshot_project_config()
-            return
+        if not validate_if_changes_can_be_applied(diff, current_manifest=current_manifest):
+            return await prompt_override_local_remote(diff=diff, remote_manifest=remote_manifest, force=force)
+
         console.print("[yellow]Conflict resolution[/yellow]: ", end="")
-        if not prompt_confirm("Do you want to apply the above changes to your local slingshot.yaml?", default=True):
-            return
+        if not (
+            force
+            or prompt_confirm("Do you want to apply the above changes to your local slingshot.yaml?", default=True)
+        ):
+            return False
+
         try:
             apply_to_local(diff, remote_manifest)
-            config.project_config.last_pushed_manifest = load_slingshot_project_config()
-        except Exception as e:
-            # If the validation succeeded but the apply fails nonetheless, we should still prompt the user
-            console.print(unable_to_synchronise_message)
-            if (
-                prompt_for_single_choice(
-                    "Do you want to use the local or remote version?", ["local", "remote"], default=0
-                )
-                == 0
-            ):
-                config.project_config.last_pushed_manifest = load_slingshot_project_config()
+            # If the last pushed manifest was empty, we should set it to the remote manifest to avoid showing conflicts
+            if is_last_pushed_manifest_empty:
+                config.project_config.last_pushed_manifest = remote_manifest
             else:
-                apply_to_local(diff, remote_manifest, force=True)
-            config.project_config.last_pushed_manifest = load_slingshot_project_config()
-            return
+                config.project_config.last_pushed_manifest = load_slingshot_project_config()
+            return True
+        except Exception as e:
+            # If the validation succeeded but apply fails nonetheless, we should still prompt the user
+            return await prompt_override_local_remote(diff=diff, remote_manifest=remote_manifest, force=force)
 
     async def plan_prompt_apply(self, and_wait: bool, force: bool) -> bool:
-        """Plan, prompt and apply changes to the remote environment.
-        Unless force is true, user will first be prompted to apply remote changes since their last push.
-        If force is true, the changes will be applied without prompting."""
+        """
+        Plan, prompt and apply changes to the remote environment.
+
+        If force is true, the changes will be applied without prompting.
+
+        Returns True if any changes were applied, False otherwise.
+        """
+        # We use a "last-pushed-manifest" as a merge base to determine what changes to apply.
+        #  There are three cases to keep in mind:
+        #  - No last-pushed-manifest and no remote manifest: it's a new project -- can safely apply the diff and push
+        #  - No last-pushed-manifest and remote manifest: it's a new copy of a project -- user should pull first
+        #  - last-pushed-manifest and remote manifest: it's a normal case -- perform a three-way merge
+        last_pushed_manifest = config.project_config.last_pushed_manifest
+        is_last_pushed_manifest_empty = last_pushed_manifest is None
+
+        if last_pushed_manifest is None:
+            last_pushed_manifest = ProjectManifest()
+        if isinstance(last_pushed_manifest, ProjectManifest):
+            last_pushed_manifest = last_pushed_manifest.dict()
+
         remote_manifest = await remote_project_manifest(self._sdk)
+        remote_diff = DeepDiff(last_pushed_manifest, remote_manifest.dict(), ignore_order=True)
+        if is_last_pushed_manifest_empty and len(remote_diff.keys()) > 0 and not force:
+            raise SlingshotException("You have unmerged remote changes. Run 'slingshot pull' and then try apply again.")
+
+        current_manifest = load_slingshot_project_config()
+        if not validate_if_changes_can_be_applied(remote_diff, current_manifest=current_manifest):
+            raise SlingshotException(
+                "Cannot apply changes because local and remote changes conflict. Run 'slingshot pull' then try again."
+            )
+
+        any_changes_applied = False
         if not force:
-            await self.apply_to_local(remote_manifest)
+            any_changes_applied = await self.apply_to_local(remote_manifest)
+
         manifest = load_slingshot_project_config()  # Reload local, in case it was changed
         env_spec_plan, app_spec_plan = await self.plan(config=manifest)
         if any(env_spec_plan) or any(app_spec_plan):
             if force or prompt_confirm("Do you want to apply these changes?", default=True):
                 await self.run(manifest, env_spec_plan=env_spec_plan, app_spec_plan=app_spec_plan, and_wait=and_wait)
-            return True
+                return True
+            return any_changes_applied
         else:
             logger.debug("No changes detected ✅ ")
-            return False
+            return any_changes_applied
+
+
+async def prompt_override_local_remote(
+    diff: DeepDiff, remote_manifest: schemas.ProjectManifest, *, force: bool
+) -> bool:
+    unable_to_synchronise_message = (
+        f"[yellow]Conflict resolution[/yellow]: Unable to synchronise remote changes to your local slingshot.yaml."
+    )
+    console.print(unable_to_synchronise_message)
+    if not force and (
+        prompt_for_single_choice("Do you want to use the local or remote version?", ["local", "remote"], default=0) == 0
+    ):
+        config.project_config.last_pushed_manifest = load_slingshot_project_config()
+        return False
+
+    apply_to_local(diff, remote_manifest, force=True)
+    config.project_config.last_pushed_manifest = load_slingshot_project_config()
+    return True
 
 
 def apply_diff(local_slingshot_yaml: dict[str, Any], diff: DeepDiff, remote_manifest: schemas.ProjectManifest) -> None:
     """Applies a diff to the local slingshot.yaml, using the remote manifest as a reference."""
     for key_path, value in diff.get("values_changed", {}).items():
         keys = parse_keys(key_path)
         d = local_slingshot_yaml
@@ -541,101 +592,116 @@
         "iterable_item_removed",
     }:
         lines.append("Other changes detected, please see the diff below:")
         lines.append(str(diff))
     return "\n".join(lines)
 
 
-def validate_if_changes_can_be_applied(
-    diff: DeepDiff, reference_manifest: schemas.ProjectManifest, current_manifest: schemas.ProjectManifest
-) -> bool:
+def validate_if_changes_can_be_applied(diff: DeepDiff, current_manifest: schemas.ProjectManifest) -> bool:
     """
     Validates if the changes to reference manifest can be applied to current manifest.
-    This is useful so we can fail early if we can't merge in the changes from the reference manifest.
+    This is useful to fail early if we can't merge in the changes from the diff.
     """
     if not diff:
         return True
     if set(diff.keys()) - {
         "values_changed",
         "dictionary_item_added",
         "dictionary_item_removed",
         "iterable_item_added",
         "iterable_item_removed",
     }:
-        logger.warning(f"Unexpected changes detected, please see the diff below: {diff}")
+        logger.debug(f"Diff keys: {diff.keys()}")
+        logger.debug(f"Unexpected changes detected, please see the diff below: {diff}")
         return False
     current_manifest = current_manifest.dict()
 
     for key_path, value in diff.get("values_changed", {}).items():
         keys = parse_keys(key_path)
-        d = current_manifest
-        for k in keys[:-1]:
-            if isinstance(d, dict) and k not in d:  # Can't change a key that doesn't exist
+        current_root = current_manifest
+        for key in keys[:-1]:
+            if isinstance(current_root, dict) and key not in current_root:
+                logger.debug(f"Cannot change key that doesn't exist: {key}")
                 return False
-            if isinstance(d, list) and int(k) >= len(d):  # Can't change an index that doesn't exist
+            if isinstance(current_root, list) and int(key) >= len(current_root):
+                logger.debug(f"Cannot change index that doesn't exist: {key}")
                 return False
-            d = d[k]
-
-        if isinstance(d, dict) and not keys[-1] in d:  # Can't change a key that doesn't exist
+            current_root = current_root[key]
+        if isinstance(current_root, dict) and not keys[-1] in current_root:
+            logger.debug(f"Cannot change key that doesn't exist: {keys[-1]}")
             return False
-        if isinstance(d, list) and int(keys[-1]) >= len(d):  # Can't change an index that doesn't exist
+        if isinstance(current_root, list) and int(keys[-1]) >= len(current_root):
+            logger.debug(f"Cannot change index that doesn't exist: {keys[-1]}")
             return False
     for key_path in diff.get("dictionary_item_added", []):
         keys = parse_keys(key_path)
-        d = current_manifest
-        for k in keys[:-1]:
-            if isinstance(d, dict) and k not in d:  # Can't add within a key that doesn't exist
+        current_root = current_manifest
+        for key in keys[:-1]:
+            if isinstance(current_root, dict) and key not in current_root:
+                logger.debug(f"Cannot add within key that doesn't exist: {key}")
                 return False
-            if isinstance(d, list) and int(k) >= len(d):  # Can't add within an index that doesn't exist
+            if isinstance(current_root, list) and int(key) >= len(current_root):
+                logger.debug(f"Cannot add within index that doesn't exist: {key}")
                 return False
-            d = d[k]
-        if not isinstance(d, dict):  # Can't add a key to a list
+            current_root = current_root[key]
+        if not isinstance(current_root, dict):  # Can't add a key to a list
+            logger.debug(f"Cannot add a dictionary key to a list: {current_root}")
             return False
-        if keys[-1] in d:  # Can't add a key that already exists
+        if keys[-1] in current_root:
+            logger.debug(f"Cannot add a dictionary key that already exists: {keys[-1]}")
             return False
     for key_path in diff.get("dictionary_item_removed", []):
         keys = parse_keys(key_path)
-        d = current_manifest
-        for k in keys[:-1]:
-            if isinstance(d, dict) and k not in d:  # Can't remove within a key that doesn't exist
+        current_root = current_manifest
+        for key in keys[:-1]:
+            if isinstance(current_root, dict) and key not in current_root:
+                logger.debug(f"Cannot remove within dictionary key that doesn't exist: {key}")
                 return False
-            d = d[k]
-        if not isinstance(d, dict):  # Can't remove a key from a list
+            current_root = current_root[key]
+        if not isinstance(current_root, dict):
+            logger.debug(f"Cannot remove a dictionary key from a list: {current_root}")
             return False
-        if not keys[-1] in d:
+        if not keys[-1] in current_root:
+            logger.debug(f"Cannot remove a dictionary key that doesn't exist: {keys[-1]}")
             return False  # Can't remove a key that doesn't exist
     for key_path, value in diff.get("iterable_item_added", {}).items():
         keys = parse_keys(key_path)
-        d = current_manifest
-        for k in keys[:-1]:
-            if isinstance(d, dict) and k not in d:  # Can't add within a key that doesn't exist
+        current_root = current_manifest
+        for key in keys[:-1]:
+            if isinstance(current_root, dict) and key not in current_root:
+                logger.debug(f"Cannot add iterable item within key that doesn't exist: {key}")
                 return False
-            if isinstance(d, list) and int(k) >= len(d):  # Can't add within an index that doesn't exist
-                return False
-        if not isinstance(d, list):  # iterable_item_added can only be applied to lists
+            current_root = current_root[key]
+        if not isinstance(current_root, list):
+            logger.debug(f"iterable_item_added can only be applied to lists: {current_root}")
             return False
-        if value in d:  # Assume all lists are sets?
+        if value in current_root:
+            logger.debug(f"Cannot add an iterable item that already exists: {value}")
             return False
     for key_path, value in diff.get("iterable_item_removed", {}).items():
         keys = parse_keys(key_path)
-        d = current_manifest
-        for k in keys[:-1]:
-            if isinstance(d, dict) and k not in d:  # Can't remove within a key that doesn't exist
+        current_root = current_manifest
+        for key in keys[:-1]:
+            if isinstance(current_root, dict) and key not in current_root:
+                logger.debug(f"Cannot remove iterable item within key that doesn't exist: {key}")
                 return False
-            if isinstance(d, list) and int(k) >= len(d):  # Can't remove within an index that doesn't exist
+            if isinstance(current_root, list) and int(key) >= len(current_root):
+                logger.debug(f"Cannot remove iterable item within index that doesn't exist: {key}")
                 return False
-            d = d[k]
-        if not isinstance(d, list):  # iterable_item_removed can only be applied to lists
+            current_root = current_root[key]
+        if not isinstance(current_root, list):
+            logger.debug(f"iterable_item_removed can only be applied to lists: {current_root}")
+            return False
+        assert isinstance((key := keys[-1]), int)  # Must be an int if we're removing an iterable item
+        if len(current_root) <= key:
+            logger.debug(f"Cannot remove an iterable item index that doesn't exist: {key}")
+            return False
+        if not current_root[key] == value:
+            logger.debug(f"Cannot remove an iterable item that doesn't match the value to be removed: {value}")
             return False
-        assert isinstance((k := keys[-1]), int)  # iterable_item_removed can only be applied to lists
-        if len(d) <= k:
-            return False  # Can't remove an index that doesn't exist
-        if not d[k] == value:
-            return False  # Existing value doesn't match the value to be removed
-
     return True
 
 
 def apply_to_local(diff: DeepDiff, reference_manifest: schemas.ProjectManifest, force: bool = False) -> None:
     """
     Apply a diff to the local slingshot.yaml file.
     If force, just use the reference manifest - completely ignore the local slingshot.yaml file.
```

### Comparing `slingshot_ai-0.0.10/src/slingshot/sdk/auth.py` & `slingshot_ai-0.0.11/src/slingshot/sdk/auth.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/sdk/config.py` & `slingshot_ai-0.0.11/src/slingshot/sdk/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         return v
 
     class JSONConfig:
         settings_json_file: Path = client_settings.global_config_folder / "config.json"
 
 
 class ProjectConfig(BaseJSONSettings):
-    project_name: Optional[str] = None
+    project_id: Optional[str] = None
     last_pushed_manifest: Optional[dict[str, Any]] = None
 
     class JSONConfig:
         settings_json_file: Path = client_settings.project_config_folder / "config.json"
 
 
 global_config = GlobalConfig()
```

### Comparing `slingshot_ai-0.0.10/src/slingshot/sdk/config_utils.py` & `slingshot_ai-0.0.11/src/slingshot/sdk/config_utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/sdk/errors.py` & `slingshot_ai-0.0.11/src/slingshot/sdk/errors.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/sdk/graphql/base_graphql.py` & `slingshot_ai-0.0.11/src/slingshot/sdk/graphql/base_graphql.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/sdk/graphql/fragments.py` & `slingshot_ai-0.0.11/src/slingshot/sdk/graphql/fragments.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,19 +230,17 @@
 
 
 class ProjectFields(BaseGraphQLEntity):
     _depends_on = []
     _fragment = """
         fragment ProjectFields on Projects {
           projectId
-          projectName
           displayName
         } """
     project_id: str = Field(..., alias="projectId")
-    project_name: str = Field(..., alias="projectName")
     display_name: str = Field(..., alias="displayName")
 
 
 class BillingLineItem(BaseGraphQLEntity):
     _depends_on = []
     _fragment = """
         fragment BillingLineItem on BillingLineItems {
```

### Comparing `slingshot_ai-0.0.10/src/slingshot/sdk/graphql/queries/apps.py` & `slingshot_ai-0.0.11/src/slingshot/sdk/graphql/queries/apps.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/sdk/graphql/queries/deployment.py` & `slingshot_ai-0.0.11/src/slingshot/sdk/graphql/queries/deployment.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/sdk/graphql/queries/environment.py` & `slingshot_ai-0.0.11/src/slingshot/sdk/graphql/queries/environment.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/sdk/graphql/queries/project.py` & `slingshot_ai-0.0.11/src/slingshot/sdk/graphql/queries/project.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,32 +61,14 @@
 
     _depends_on = [fragments.ProjectFields]
 
     def __init__(self, project_id: str):
         super().__init__(variables={"projectId": project_id}, response_model=ProjectByIdResponse)
 
 
-class ProjectByNameResponse(BaseModel):
-    projects: list[fragments.ProjectFields] = Field(..., alias="projects")
-
-
-class ProjectByNameQuery(BaseGraphQLQuery[ProjectByNameResponse]):
-    _query = """
-        query ProjectByName($projectName: String!) {
-          projects(where: {projectName: {_eq: $projectName}}) {
-            ...ProjectFields
-          }
-        } """
-
-    _depends_on = [fragments.ProjectFields]
-
-    def __init__(self, project_name: str):
-        super().__init__(variables={"projectName": project_name}, response_model=ProjectByNameResponse)
-
-
 class BillingLineItemsResponse(BaseModel):
     billingLineItems: list[fragments.BillingLineItem] = Field(..., alias="billingLineItems")
 
 
 class BillingLineItemsByAppIdQuery(BaseGraphQLQuery[BillingLineItemsResponse]):
     _query = """
         query BillingLineItemsByAppIdQuery($appInstanceId: String!) {
```

### Comparing `slingshot_ai-0.0.10/src/slingshot/sdk/graphql/queries/run.py` & `slingshot_ai-0.0.11/src/slingshot/sdk/graphql/queries/run.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/sdk/graphql/queries/storage.py` & `slingshot_ai-0.0.11/src/slingshot/sdk/graphql/queries/storage.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/sdk/slingshot_api.py` & `slingshot_ai-0.0.11/src/slingshot/sdk/slingshot_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,23 +349,14 @@
             response_model=schemas.ResponseOK,
         )
 
     """
     Get API methods
     """
 
-    async def get_project_by_name(self, project_name: str) -> fragments.ProjectFields | None:
-        """Get a project by name."""
-        query = queries.ProjectByNameQuery(project_name=project_name)
-        resp = await self._client.make_graphql_request(query)
-        if resp.errors:
-            raise SlingshotException(f"Failed to get project by name: {resp.errors}")
-        project = resp.data.projects[0] if resp.data and resp.data.projects else None
-        return project
-
     async def get_billing_line_items_by_app_id(self, app_instance_id: str) -> list[fragments.BillingLineItem]:
         query = queries.BillingLineItemsByAppIdQuery(app_instance_id=app_instance_id)
         resp = await self._client.make_graphql_request(query)
         data = resp.get_data_or_raise()
         return data.billingLineItems
 
     async def get_billing_line_items_by_deployment_id(self, deployment_id: str) -> list[fragments.BillingLineItem]:
@@ -619,22 +610,22 @@
             yield schemas.AppInstanceStatus(deployment_instances[0].deployment_instance_status)
 
     """
     Create API methods
     """
 
     async def create_project(
-        self, project_slug: str, project_display_name: Optional[str] = None
+        self, project_id: str, project_display_name: Optional[str] = None
     ) -> schemas.Response[schemas.ProjectId]:
         """Create a new project."""
         return await self._client.make_request(
             url=f"project",
             method="post",
             response_model=schemas.Response[schemas.ProjectId],
-            json_data=schemas.BodyNewProject(project_slug=project_slug, display_name=project_display_name).dict(),
+            json_data=schemas.BodyNewProject(project_id=project_id, display_name=project_display_name).dict(),
         )
 
     async def create_app(
         self,
         name: str,
         command: str | None,
         app_type: schemas.AppType,
@@ -979,19 +970,19 @@
         )
 
     """
     Predict API methods
     """
 
     async def predict(
-        self, project_name: str, deployment_name: str, example_bytes: bytes, timeout_seconds: int = 60
+        self, project_id: str, deployment_name: str, example_bytes: bytes, timeout_seconds: int = 60
     ) -> schemas.PredictionResponse:
         """Make a prediction."""
         return await self._client.make_request(
-            url=f"predict/{project_name}/{deployment_name}",
+            url=f"predict/{project_id}/{deployment_name}",
             method="post",
             response_model=schemas.PredictionResponse,
             timeout=datetime.timedelta(seconds=timeout_seconds),
             data={"example": example_bytes},
         )
 
     @backoff.on_exception(backoff.expo, (Retry,), max_tries=3)
```

### Comparing `slingshot_ai-0.0.10/src/slingshot/sdk/slingshot_sdk.py` & `slingshot_ai-0.0.11/src/slingshot/sdk/slingshot_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     return typing.cast(Function, wrapper)
 
 
 class SlingshotSDK:
     def __init__(self, verbose: bool = False, slingshot_url: str = config.global_config.slingshot_backend_url) -> None:
         self._me: fragments.MeResponse | None = None
         self.verbose = verbose
-        self.project_name = project_config.project_name
+        self.project_id = project_config.project_id
         self.project: schemas.Project | None = None
         self._client = SlingshotClient(
             auth_token=global_config.auth_token, slingshot_url=slingshot_url, auto_setup_hook=self.setup
         )
         self._api = SlingshotAPI(client=self._client)
         self.web_path_util = WebPathUtil(self, slingshot_url=slingshot_url)
 
@@ -100,15 +100,15 @@
             and (project_id := os.environ.get("SLINGSHOT_PROJECT_ID", None))
         ):
             project = await self._api.get_project_by_id(project_id, _setup=False)
             if project is None:
                 logger.debug(f"Project with id {project_id} not found.")
                 return
             self.project = project
-            self.project_name = project.project_name
+            self.project_id = project.project_id
 
     async def check_for_updates(self) -> bool:
         """
         Check if the backend has a newer version of Slingshot than the SDK.
         Returns True if there is a newer version, False otherwise.
         """
         if global_config.last_checked_for_updates is not None and (
@@ -207,26 +207,34 @@
         """Set the SSH key for the current user"""
         await self._api.update_ssh_public_key(ssh_key)
 
     """
     Project SDK methods
     """
 
-    async def use_project(self, project_name: str) -> None:
+    async def use_project(self, project_id: str) -> None:
         """Set the current project"""
-        project_fields = await self._api.get_project_by_name(project_name)
+        project_fields = await self._api.get_project_by_id(project_id)
         if not project_fields:
-            raise SlingshotException(f"Project '{project_name}' not found.")
+            raise SlingshotException(f"Project '{project_id}' not found.")
         self.project = project_fields
-        project_config.project_name = project_name
+        project_config.project_id = project_id
 
     async def apply_project(self, and_wait: bool = False, force: bool = False) -> bool:
-        """Apply the YAML configuration in the current directory to the current project"""
+        """
+        Apply the YAML configuration in the current directory to the current project.
+
+        Returns True if any changes were applied, False otherwise.
+        """
         return await ApplyService(self).plan_prompt_apply(and_wait, force=force)
 
+    async def apply_to_local(self, force: bool = False) -> bool:
+        """Apply the YAML configuration from the remote project to the current project"""
+        return await ApplyService(self).apply_to_local(None, force=force)
+
     """
     Source code SDK methods
     """
 
     async def push_code(
         self, code_dir: str | None = None, description: Optional[str] = None, and_print: bool = False
     ) -> schemas.UploadedSourceCode:
@@ -465,15 +473,15 @@
 
     async def predict(
         self, deployment_name: str, example_bytes: bytes, timeout_seconds: int = 60
     ) -> dict[str, typing.Any]:
         """Make a prediction against a deployment."""
         project = await self._get_current_project_or_raise()
         resp = await self._api.predict(
-            project_name=project.project_name,
+            project_id=project.project_id,
             deployment_name=deployment_name,
             example_bytes=example_bytes,
             timeout_seconds=timeout_seconds,
         )
         return get_data_or_raise(resp)
 
     @staticmethod
@@ -856,17 +864,17 @@
         project_id = await self._get_current_project_id_or_raise()
         return await self._api.get_blob_artifact_by_name(blob_artifact_name, project_id=project_id)
 
     """
     Create SDK methods
     """
 
-    async def create_project(self, slug: str, display_name: str) -> schemas.Response[schemas.ProjectId]:
-        """Create a new project with the given slug and display name."""
-        return await self._api.create_project(project_slug=slug, project_display_name=display_name)
+    async def create_project(self, project_id: str, display_name: str) -> schemas.Response[schemas.ProjectId]:
+        """Create a new project with the given ID and display name."""
+        return await self._api.create_project(project_id=project_id, project_display_name=display_name)
 
     async def create_app(
         self,
         name: str,
         command: str | None,
         app_type: schemas.AppType,
         exec_env_spec_id: str,
```

### Comparing `slingshot_ai-0.0.10/src/slingshot/sdk/sync.py` & `slingshot_ai-0.0.11/src/slingshot/sdk/sync.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/sdk/upload_download_utils.py` & `slingshot_ai-0.0.11/src/slingshot/sdk/upload_download_utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/sdk/utils.py` & `slingshot_ai-0.0.11/src/slingshot/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/sdk/web_path_util.py` & `slingshot_ai-0.0.11/src/slingshot/sdk/web_path_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,18 +27,18 @@
     async def project(self) -> str:
         ...
 
     async def project(self, project: schemas.Project | str | None = None) -> str:
         if project is None:
             project = await self._sdk._get_current_project_or_raise()
         if isinstance(project, str):
-            project_name = project
+            project_id = project
         else:
-            project_name = project.project_name
-        return f"{self.homepage}/project/{project_name}/"
+            project_id = project.project_id
+        return f"{self.homepage}/project/{project_id}/"
 
     @typing.overload
     async def code(self, source_code: schemas.HasSourceCodeId) -> str:
         ...
 
     @typing.overload
     async def code(self, source_code: str) -> str:
@@ -46,15 +46,15 @@
 
     async def code(self, source_code: schemas.HasSourceCodeId | str) -> str:
         project = await self._sdk._get_current_project_or_raise()
         if isinstance(source_code, str):
             source_code_id = source_code
         else:
             source_code_id = source_code.source_code_id
-        return f"{self.homepage}/project/{project.project_name}/code/{source_code_id}"
+        return f"{self.homepage}/project/{project.project_id}/code/{source_code_id}"
 
     @typing.overload
     async def blob_artifact(self, blob_artifact: schemas.HasBlobArtifactId) -> str:
         ...
 
     @typing.overload
     async def blob_artifact(self, blob_artifact: str) -> str:
@@ -62,15 +62,15 @@
 
     async def blob_artifact(self, blob_artifact: schemas.HasBlobArtifactId | str) -> str:
         project = await self._sdk._get_current_project_or_raise()
         if isinstance(blob_artifact, str):
             blob_artifact_id = blob_artifact
         else:
             blob_artifact_id = blob_artifact.blob_artifact_id
-        return f"{self.homepage}/project/{project.project_name}/artifacts/{blob_artifact_id}"
+        return f"{self.homepage}/project/{project.project_id}/artifacts/{blob_artifact_id}"
 
     @typing.overload
     async def app(self, app_spec: schemas.HasAppSpecId) -> str:
         ...
 
     @typing.overload
     async def app(self, app_spec: str) -> str:
@@ -78,15 +78,15 @@
 
     async def app(self, app_spec: schemas.HasAppSpecId | str) -> str:
         project = await self._sdk._get_current_project_or_raise()
         if isinstance(app_spec, str):
             app_spec_id = app_spec
         else:
             app_spec_id = app_spec.app_spec_id
-        return f"{self.homepage}/project/{project.project_name}/apps/{app_spec_id}"
+        return f"{self.homepage}/project/{project.project_id}/apps/{app_spec_id}"
 
     @typing.overload
     async def run(self, run: schemas.HasRunId) -> str:
         ...
 
     @typing.overload
     async def run(self, run: str) -> str:
@@ -94,15 +94,15 @@
 
     async def run(self, run: schemas.HasRunId | str) -> str:
         project = await self._sdk._get_current_project_or_raise()
         if isinstance(run, str):
             run_id = run
         else:
             run_id = run.run_id
-        return f"{self.homepage}/project/{project.project_name}/runs/{run_id}"
+        return f"{self.homepage}/project/{project.project_id}/runs/{run_id}"
 
     @typing.overload
     async def deployment(self, deployment_spec: schemas.HasAppSpecId) -> str:
         ...
 
     @typing.overload
     async def deployment(self, deployment_spec: str) -> str:
@@ -110,15 +110,15 @@
 
     async def deployment(self, deployment_spec: schemas.HasAppSpecId | str) -> str:
         project = await self._sdk._get_current_project_or_raise()
         if isinstance(deployment_spec, str):
             app_spec_id = deployment_spec
         else:
             app_spec_id = deployment_spec.app_spec_id
-        return f"{self.homepage}/project/{project.project_name}/deployments/{app_spec_id}"
+        return f"{self.homepage}/project/{project.project_id}/deployments/{app_spec_id}"
 
     @typing.overload
     async def environment(self, env: schemas.HasExecutionEnvironmentId) -> str:
         ...
 
     @typing.overload
     async def environment(self, env: str) -> str:
@@ -126,8 +126,8 @@
 
     async def environment(self, env: schemas.HasExecutionEnvironmentId | str) -> str:
         project = await self._sdk._get_current_project_or_raise()
         if isinstance(env, str):
             env_id = env
         else:
             env_id = env.execution_environment_id
-        return f"{self.homepage}/project/{project.project_name}/environments/{env_id}"
+        return f"{self.homepage}/project/{project.project_id}/environments/{env_id}"
```

### Comparing `slingshot_ai-0.0.10/src/slingshot/shared/utils.py` & `slingshot_ai-0.0.11/src/slingshot/shared/utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/templates/inference_template.py` & `slingshot_ai-0.0.11/src/slingshot/templates/inference_template.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/src/slingshot/templates/label_studio_data_export_template.py` & `slingshot_ai-0.0.11/src/slingshot/templates/label_studio_data_export_template.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.10/PKG-INFO` & `slingshot_ai-0.0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slingshot-ai
-Version: 0.0.10
+Version: 0.0.11
 Summary: 
 Author: Slingshot AI
 Author-email: service-account@slingshot.xyz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

