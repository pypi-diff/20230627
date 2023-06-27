# Comparing `tmp/opal-common-0.7.2.tar.gz` & `tmp/opal-common-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal-common-0.7.2.tar", last modified: Tue Jun 20 15:19:30 2023, max compression
+gzip compressed data, was "opal-common-0.7.3.tar", last modified: Tue Jun 27 11:25:34 2023, max compression
```

## Comparing `opal-common-0.7.2.tar` & `opal-common-0.7.3.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.834230 opal-common-0.7.2/
--rw-r--r--   0 roekatz    (501) staff       (20)     8924 2023-06-20 15:19:30.834034 opal-common-0.7.2/PKG-INFO
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.808308 opal-common-0.7.2/opal_common/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      797 2023-05-09 07:59:18.000000 opal-common-0.7.2/opal_common/async_utils.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.811322 opal-common-0.7.2/opal_common/authentication/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/authentication/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1477 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/authentication/authz.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3267 2023-05-09 07:59:18.000000 opal-common-0.7.2/opal_common/authentication/casting.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5016 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/authentication/deps.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4669 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/authentication/signer.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.811941 opal-common-0.7.2/opal_common/authentication/tests/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/authentication/tests/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)    17336 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/authentication/tests/jwt_signer_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)      958 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/authentication/types.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4225 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/authentication/verifier.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.814333 opal-common-0.7.2/opal_common/cli/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/cli/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6657 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/cli/commands.py
--rw-r--r--   0 roekatz    (501) staff       (20)      703 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/cli/docs.py
--rw-r--r--   0 roekatz    (501) staff       (20)      167 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/cli/typer_app.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.816198 opal-common-0.7.2/opal_common/confi/
--rw-r--r--   0 roekatz    (501) staff       (20)       21 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/confi/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2278 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/confi/cli.py
--rw-r--r--   0 roekatz    (501) staff       (20)    13780 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/confi/confi.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2719 2023-04-18 15:25:03.000000 opal-common-0.7.2/opal_common/confi/types.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6831 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/config.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1492 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/corn_utils.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6050 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/emport.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.817330 opal-common-0.7.2/opal_common/engine/
--rw-r--r--   0 roekatz    (501) staff       (20)       90 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/engine/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      576 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/engine/parsing.py
--rw-r--r--   0 roekatz    (501) staff       (20)      593 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/engine/paths.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.818840 opal-common-0.7.2/opal_common/fetcher/
--rw-r--r--   0 roekatz    (501) staff       (20)      143 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/fetcher/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.819816 opal-common-0.7.2/opal_common/fetcher/engine/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/fetcher/engine/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2653 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/fetcher/engine/base_fetching_engine.py
--rw-r--r--   0 roekatz    (501) staff       (20)      296 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/fetcher/engine/core_callbacks.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1536 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/fetcher/engine/fetch_worker.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8485 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/fetcher/engine/fetching_engine.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1191 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/fetcher/events.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2548 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/fetcher/fetch_provider.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3030 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/fetcher/fetcher_register.py
--rw-r--r--   0 roekatz    (501) staff       (20)      116 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/fetcher/logger.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.822090 opal-common-0.7.2/opal_common/fetcher/providers/
--rw-r--r--   0 roekatz    (501) staff       (20)       67 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/fetcher/providers/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1710 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3525 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/fetcher/providers/http_fetch_provider.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.823627 opal-common-0.7.2/opal_common/fetcher/tests/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/fetcher/tests/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1917 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/fetcher/tests/failure_handler_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4291 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/fetcher/tests/http_fetch_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2140 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/fetcher/tests/rpc_fetch_test.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.826015 opal-common-0.7.2/opal_common/git/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/git/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5461 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/git/branch_tracker.py
--rw-r--r--   0 roekatz    (501) staff       (20)    15557 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/git/bundle_maker.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1887 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/git/bundle_utils.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8684 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/git/commit_viewer.py
--rw-r--r--   0 roekatz    (501) staff       (20)     7948 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/git/diff_viewer.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1580 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/git/env.py
--rw-r--r--   0 roekatz    (501) staff       (20)      299 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/git/exceptions.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8535 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/git/repo_cloner.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4237 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/git/tar_file_to_local_git_extractor.py
--rw-r--r--   0 roekatz    (501) staff       (20)      182 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/http.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1832 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/logger.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.827164 opal-common-0.7.2/opal_common/logging/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/logging/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      412 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/logging/decorators.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1166 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/logging/filter.py
--rw-r--r--   0 roekatz    (501) staff       (20)      617 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/logging/formatter.py
--rw-r--r--   0 roekatz    (501) staff       (20)      700 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/logging/intercept.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1355 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/logging/thirdparty.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3520 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/middleware.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4067 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/paths.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.830128 opal-common-0.7.2/opal_common/schemas/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/schemas/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6313 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/schemas/data.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1387 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/schemas/policy.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1767 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/schemas/policy_source.py
--rw-r--r--   0 roekatz    (501) staff       (20)      508 2023-04-04 11:14:44.000000 opal-common-0.7.2/opal_common/schemas/scopes.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1573 2023-05-23 16:26:33.000000 opal-common-0.7.2/opal_common/schemas/security.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2003 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/schemas/store.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1438 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/schemas/webhook.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.830665 opal-common-0.7.2/opal_common/security/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/security/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      799 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/security/sslcontext.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3294 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/security/tarsafe.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.831486 opal-common-0.7.2/opal_common/sources/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/sources/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)    11067 2023-06-03 11:34:06.000000 opal-common-0.7.2/opal_common/sources/api_policy_source.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4283 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/sources/base_policy_source.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4238 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/sources/git_policy_source.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.832003 opal-common-0.7.2/opal_common/synchronization/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/synchronization/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1294 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/synchronization/expiring_redis_lock.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2990 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/synchronization/named_lock.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.833011 opal-common-0.7.2/opal_common/tests/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/tests/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     9622 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/tests/path_utils_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1223 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/tests/url_utils_test.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.833733 opal-common-0.7.2/opal_common/topics/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/topics/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2371 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/topics/listener.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6728 2023-06-20 13:37:00.000000 opal-common-0.7.2/opal_common/topics/publisher.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1054 2023-05-29 10:10:14.000000 opal-common-0.7.2/opal_common/topics/utils.py
--rw-r--r--   0 roekatz    (501) staff       (20)      988 2022-12-08 13:40:17.000000 opal-common-0.7.2/opal_common/urls.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8371 2023-06-03 11:34:06.000000 opal-common-0.7.2/opal_common/utils.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 15:19:30.809404 opal-common-0.7.2/opal_common.egg-info/
--rw-r--r--   0 roekatz    (501) staff       (20)     8924 2023-06-20 15:19:30.000000 opal-common-0.7.2/opal_common.egg-info/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)     3207 2023-06-20 15:19:30.000000 opal-common-0.7.2/opal_common.egg-info/SOURCES.txt
--rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-06-20 15:19:30.000000 opal-common-0.7.2/opal_common.egg-info/dependency_links.txt
--rw-r--r--   0 roekatz    (501) staff       (20)      471 2023-06-20 15:19:30.000000 opal-common-0.7.2/opal_common.egg-info/requires.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       12 2023-06-20 15:19:30.000000 opal-common-0.7.2/opal_common.egg-info/top_level.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       38 2023-06-20 15:19:30.834275 opal-common-0.7.2/setup.cfg
--rw-r--r--   0 roekatz    (501) staff       (20)     2601 2022-12-08 13:40:17.000000 opal-common-0.7.2/setup.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.736164 opal-common-0.7.3/
+-rw-r--r--   0 roekatz    (501) staff       (20)     8924 2023-06-27 11:25:34.735790 opal-common-0.7.3/PKG-INFO
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.714848 opal-common-0.7.3/opal_common/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      797 2023-05-09 07:59:18.000000 opal-common-0.7.3/opal_common/async_utils.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.717522 opal-common-0.7.3/opal_common/authentication/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/authentication/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1477 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/authentication/authz.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3267 2023-05-09 07:59:18.000000 opal-common-0.7.3/opal_common/authentication/casting.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5016 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/authentication/deps.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4669 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/authentication/signer.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.717915 opal-common-0.7.3/opal_common/authentication/tests/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/authentication/tests/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    17336 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/authentication/tests/jwt_signer_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      958 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/authentication/types.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4225 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/authentication/verifier.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.719108 opal-common-0.7.3/opal_common/cli/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/cli/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6657 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/cli/commands.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      703 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/cli/docs.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      167 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/cli/typer_app.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.720002 opal-common-0.7.3/opal_common/confi/
+-rw-r--r--   0 roekatz    (501) staff       (20)       21 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/confi/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2278 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/confi/cli.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    13780 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/confi/confi.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2719 2023-04-18 15:25:03.000000 opal-common-0.7.3/opal_common/confi/types.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6831 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/config.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1492 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/corn_utils.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6050 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/emport.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.720799 opal-common-0.7.3/opal_common/engine/
+-rw-r--r--   0 roekatz    (501) staff       (20)       90 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/engine/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      576 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/engine/parsing.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      593 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/engine/paths.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.722786 opal-common-0.7.3/opal_common/fetcher/
+-rw-r--r--   0 roekatz    (501) staff       (20)      143 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/fetcher/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.724265 opal-common-0.7.3/opal_common/fetcher/engine/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/fetcher/engine/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2653 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/fetcher/engine/base_fetching_engine.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      296 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/fetcher/engine/core_callbacks.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1536 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/fetcher/engine/fetch_worker.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8485 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/fetcher/engine/fetching_engine.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1191 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/fetcher/events.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2548 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/fetcher/fetch_provider.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3030 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/fetcher/fetcher_register.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      116 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/fetcher/logger.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.724953 opal-common-0.7.3/opal_common/fetcher/providers/
+-rw-r--r--   0 roekatz    (501) staff       (20)       67 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/fetcher/providers/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1710 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3525 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/fetcher/providers/http_fetch_provider.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.725768 opal-common-0.7.3/opal_common/fetcher/tests/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/fetcher/tests/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1917 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/fetcher/tests/failure_handler_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4291 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/fetcher/tests/http_fetch_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2140 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/fetcher/tests/rpc_fetch_test.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.728129 opal-common-0.7.3/opal_common/git/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/git/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5461 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/git/branch_tracker.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    15557 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/git/bundle_maker.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1887 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/git/bundle_utils.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8684 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/git/commit_viewer.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     7948 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/git/diff_viewer.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1580 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/git/env.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      299 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/git/exceptions.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8535 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/git/repo_cloner.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4237 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/git/tar_file_to_local_git_extractor.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      182 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/http.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1832 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/logger.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.729453 opal-common-0.7.3/opal_common/logging/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/logging/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      412 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/logging/decorators.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1166 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/logging/filter.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      617 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/logging/formatter.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      700 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/logging/intercept.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1355 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/logging/thirdparty.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3520 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/middleware.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4067 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/paths.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.731542 opal-common-0.7.3/opal_common/schemas/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/schemas/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6313 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/schemas/data.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1387 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/schemas/policy.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1767 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/schemas/policy_source.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      508 2023-04-04 11:14:44.000000 opal-common-0.7.3/opal_common/schemas/scopes.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1573 2023-05-23 16:26:33.000000 opal-common-0.7.3/opal_common/schemas/security.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2003 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/schemas/store.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1438 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/schemas/webhook.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.732289 opal-common-0.7.3/opal_common/security/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/security/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      799 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/security/sslcontext.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3294 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/security/tarsafe.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.733243 opal-common-0.7.3/opal_common/sources/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/sources/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    11067 2023-06-20 17:01:29.000000 opal-common-0.7.3/opal_common/sources/api_policy_source.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4283 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/sources/base_policy_source.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4238 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/sources/git_policy_source.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.733898 opal-common-0.7.3/opal_common/synchronization/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/synchronization/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1294 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/synchronization/expiring_redis_lock.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2990 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/synchronization/named_lock.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.734537 opal-common-0.7.3/opal_common/tests/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/tests/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     9622 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/tests/path_utils_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1223 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/tests/url_utils_test.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.735404 opal-common-0.7.3/opal_common/topics/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/topics/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2371 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/topics/listener.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6728 2023-06-27 10:36:06.000000 opal-common-0.7.3/opal_common/topics/publisher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1054 2023-05-29 10:10:14.000000 opal-common-0.7.3/opal_common/topics/utils.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      988 2022-12-08 13:40:17.000000 opal-common-0.7.3/opal_common/urls.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8371 2023-06-20 17:01:29.000000 opal-common-0.7.3/opal_common/utils.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-27 11:25:34.715965 opal-common-0.7.3/opal_common.egg-info/
+-rw-r--r--   0 roekatz    (501) staff       (20)     8924 2023-06-27 11:25:34.000000 opal-common-0.7.3/opal_common.egg-info/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)     3207 2023-06-27 11:25:34.000000 opal-common-0.7.3/opal_common.egg-info/SOURCES.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-06-27 11:25:34.000000 opal-common-0.7.3/opal_common.egg-info/dependency_links.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)      471 2023-06-27 11:25:34.000000 opal-common-0.7.3/opal_common.egg-info/requires.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       12 2023-06-27 11:25:34.000000 opal-common-0.7.3/opal_common.egg-info/top_level.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       38 2023-06-27 11:25:34.736232 opal-common-0.7.3/setup.cfg
+-rw-r--r--   0 roekatz    (501) staff       (20)     2601 2022-12-08 13:40:17.000000 opal-common-0.7.3/setup.py
```

### Comparing `opal-common-0.7.2/PKG-INFO` & `opal-common-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-common
-Version: 0.7.2
+Version: 0.7.3
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. opal-common contains common code used by both opal-client and opal-server.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opal-common Version: 0.7.2 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-common Version: 0.7.3 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. opal-common contains
 common code used by both opal-client and opal-server. Home-page: https://
 github.com/permitio/opal Author: Or Weis, Asaf Cohen Author-email: or@permit.io
 License: Apache 2.0 Classifier: Operating System :: OS Independent Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `opal-common-0.7.2/opal_common/async_utils.py` & `opal-common-0.7.3/opal_common/async_utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/authentication/authz.py` & `opal-common-0.7.3/opal_common/authentication/authz.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/authentication/casting.py` & `opal-common-0.7.3/opal_common/authentication/casting.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/authentication/deps.py` & `opal-common-0.7.3/opal_common/authentication/deps.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/authentication/signer.py` & `opal-common-0.7.3/opal_common/authentication/signer.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/authentication/tests/jwt_signer_test.py` & `opal-common-0.7.3/opal_common/authentication/tests/jwt_signer_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/authentication/types.py` & `opal-common-0.7.3/opal_common/authentication/types.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/authentication/verifier.py` & `opal-common-0.7.3/opal_common/authentication/verifier.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/cli/commands.py` & `opal-common-0.7.3/opal_common/cli/commands.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/cli/docs.py` & `opal-common-0.7.3/opal_common/cli/docs.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/confi/cli.py` & `opal-common-0.7.3/opal_common/confi/cli.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/confi/confi.py` & `opal-common-0.7.3/opal_common/confi/confi.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/confi/types.py` & `opal-common-0.7.3/opal_common/confi/types.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/config.py` & `opal-common-0.7.3/opal_common/config.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/corn_utils.py` & `opal-common-0.7.3/opal_common/corn_utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/emport.py` & `opal-common-0.7.3/opal_common/emport.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/engine/parsing.py` & `opal-common-0.7.3/opal_common/engine/parsing.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/engine/paths.py` & `opal-common-0.7.3/opal_common/engine/paths.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/fetcher/engine/base_fetching_engine.py` & `opal-common-0.7.3/opal_common/fetcher/engine/base_fetching_engine.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/fetcher/engine/fetch_worker.py` & `opal-common-0.7.3/opal_common/fetcher/engine/fetch_worker.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/fetcher/engine/fetching_engine.py` & `opal-common-0.7.3/opal_common/fetcher/engine/fetching_engine.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/fetcher/events.py` & `opal-common-0.7.3/opal_common/fetcher/events.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/fetcher/fetch_provider.py` & `opal-common-0.7.3/opal_common/fetcher/fetch_provider.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/fetcher/fetcher_register.py` & `opal-common-0.7.3/opal_common/fetcher/fetcher_register.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py` & `opal-common-0.7.3/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/fetcher/providers/http_fetch_provider.py` & `opal-common-0.7.3/opal_common/fetcher/providers/http_fetch_provider.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/fetcher/tests/failure_handler_test.py` & `opal-common-0.7.3/opal_common/fetcher/tests/failure_handler_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/fetcher/tests/http_fetch_test.py` & `opal-common-0.7.3/opal_common/fetcher/tests/http_fetch_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/fetcher/tests/rpc_fetch_test.py` & `opal-common-0.7.3/opal_common/fetcher/tests/rpc_fetch_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/git/branch_tracker.py` & `opal-common-0.7.3/opal_common/git/branch_tracker.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/git/bundle_maker.py` & `opal-common-0.7.3/opal_common/git/bundle_maker.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/git/bundle_utils.py` & `opal-common-0.7.3/opal_common/git/bundle_utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/git/commit_viewer.py` & `opal-common-0.7.3/opal_common/git/commit_viewer.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/git/diff_viewer.py` & `opal-common-0.7.3/opal_common/git/diff_viewer.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/git/env.py` & `opal-common-0.7.3/opal_common/git/env.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/git/repo_cloner.py` & `opal-common-0.7.3/opal_common/git/repo_cloner.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/git/tar_file_to_local_git_extractor.py` & `opal-common-0.7.3/opal_common/git/tar_file_to_local_git_extractor.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/logger.py` & `opal-common-0.7.3/opal_common/logger.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/logging/filter.py` & `opal-common-0.7.3/opal_common/logging/filter.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/logging/formatter.py` & `opal-common-0.7.3/opal_common/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/logging/intercept.py` & `opal-common-0.7.3/opal_common/logging/intercept.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/logging/thirdparty.py` & `opal-common-0.7.3/opal_common/logging/thirdparty.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/middleware.py` & `opal-common-0.7.3/opal_common/middleware.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/paths.py` & `opal-common-0.7.3/opal_common/paths.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/schemas/data.py` & `opal-common-0.7.3/opal_common/schemas/data.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/schemas/policy.py` & `opal-common-0.7.3/opal_common/schemas/policy.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/schemas/policy_source.py` & `opal-common-0.7.3/opal_common/schemas/policy_source.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/schemas/security.py` & `opal-common-0.7.3/opal_common/schemas/security.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/schemas/store.py` & `opal-common-0.7.3/opal_common/schemas/store.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/schemas/webhook.py` & `opal-common-0.7.3/opal_common/schemas/webhook.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/security/sslcontext.py` & `opal-common-0.7.3/opal_common/security/sslcontext.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/security/tarsafe.py` & `opal-common-0.7.3/opal_common/security/tarsafe.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/sources/api_policy_source.py` & `opal-common-0.7.3/opal_common/sources/api_policy_source.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/sources/base_policy_source.py` & `opal-common-0.7.3/opal_common/sources/base_policy_source.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/sources/git_policy_source.py` & `opal-common-0.7.3/opal_common/sources/git_policy_source.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/synchronization/expiring_redis_lock.py` & `opal-common-0.7.3/opal_common/synchronization/expiring_redis_lock.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/synchronization/named_lock.py` & `opal-common-0.7.3/opal_common/synchronization/named_lock.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/tests/path_utils_test.py` & `opal-common-0.7.3/opal_common/tests/path_utils_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/tests/url_utils_test.py` & `opal-common-0.7.3/opal_common/tests/url_utils_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/topics/listener.py` & `opal-common-0.7.3/opal_common/topics/listener.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/topics/publisher.py` & `opal-common-0.7.3/opal_common/topics/publisher.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/topics/utils.py` & `opal-common-0.7.3/opal_common/topics/utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/urls.py` & `opal-common-0.7.3/opal_common/urls.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common/utils.py` & `opal-common-0.7.3/opal_common/utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/opal_common.egg-info/PKG-INFO` & `opal-common-0.7.3/opal_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-common
-Version: 0.7.2
+Version: 0.7.3
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. opal-common contains common code used by both opal-client and opal-server.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opal-common Version: 0.7.2 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-common Version: 0.7.3 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. opal-common contains
 common code used by both opal-client and opal-server. Home-page: https://
 github.com/permitio/opal Author: Or Weis, Asaf Cohen Author-email: or@permit.io
 License: Apache 2.0 Classifier: Operating System :: OS Independent Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `opal-common-0.7.2/opal_common.egg-info/SOURCES.txt` & `opal-common-0.7.3/opal_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opal-common-0.7.2/setup.py` & `opal-common-0.7.3/setup.py`

 * *Files identical despite different names*

