# Comparing `tmp/circlecigen-0.0.7.tar.gz` & `tmp/circlecigen-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circlecigen-0.0.7.tar", last modified: Fri Jun 23 06:47:21 2023, max compression
+gzip compressed data, was "circlecigen-0.0.8.tar", last modified: Tue Jun 27 05:19:46 2023, max compression
```

## Comparing `circlecigen-0.0.7.tar` & `circlecigen-0.0.8.tar`

### file list

```diff
@@ -1,58 +1,61 @@
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-23 06:47:21.290356 circlecigen-0.0.7/
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-23 06:47:21.286356 circlecigen-0.0.7/.circleci/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3975 2023-06-23 06:47:15.000000 circlecigen-0.0.7/.circleci/config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      350 2023-06-23 06:47:15.000000 circlecigen-0.0.7/.codeclimate.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-23 06:47:15.000000 circlecigen-0.0.7/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-06-23 06:47:15.000000 circlecigen-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18369 2023-06-23 06:47:15.000000 circlecigen-0.0.7/.pylintrc
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2023-06-23 06:47:15.000000 circlecigen-0.0.7/.python-version
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-06-23 06:47:15.000000 circlecigen-0.0.7/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22356 2023-06-23 06:47:21.290356 circlecigen-0.0.7/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      432 2023-06-23 06:47:15.000000 circlecigen-0.0.7/Pipfile
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21721 2023-06-23 06:47:15.000000 circlecigen-0.0.7/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-23 06:47:15.000000 circlecigen-0.0.7/__init__.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-23 06:47:21.286356 circlecigen-0.0.7/circlecigen.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22356 2023-06-23 06:47:21.000000 circlecigen-0.0.7/circlecigen.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1130 2023-06-23 06:47:21.000000 circlecigen-0.0.7/circlecigen.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-23 06:47:21.000000 circlecigen-0.0.7/circlecigen.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       52 2023-06-23 06:47:21.000000 circlecigen-0.0.7/circlecigen.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2023-06-23 06:47:21.000000 circlecigen-0.0.7/circlecigen.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2023-06-23 06:47:21.000000 circlecigen-0.0.7/circlecigen.egg-info/top_level.txt
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-23 06:47:21.290356 circlecigen-0.0.7/env_test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3037 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/default.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       39 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/dev.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5643 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/generated_config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/multi.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/nonprod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/nonprod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/nonprod.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      587 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/post-approve.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      312 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/pre-approve.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/prod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/prod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2023-06-23 06:47:15.000000 circlecigen-0.0.7/env_test/prod.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      313 2023-06-23 06:47:15.000000 circlecigen-0.0.7/notes.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-06-23 06:47:15.000000 circlecigen-0.0.7/op.env
--rw-r--r--   0 circleci  (3434) circleci  (3434)      711 2023-06-23 06:47:15.000000 circlecigen-0.0.7/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      365 2023-06-23 06:47:15.000000 circlecigen-0.0.7/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-23 06:47:21.290356 circlecigen-0.0.7/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      847 2023-06-23 06:47:15.000000 circlecigen-0.0.7/setup.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-23 06:47:21.290356 circlecigen-0.0.7/src/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-23 06:47:15.000000 circlecigen-0.0.7/src/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      160 2023-06-23 06:47:21.000000 circlecigen-0.0.7/src/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2585 2023-06-23 06:47:15.000000 circlecigen-0.0.7/src/circlecigen.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6019 2023-06-23 06:47:15.000000 circlecigen-0.0.7/src/template.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2428 2023-06-23 06:47:15.000000 circlecigen-0.0.7/src/tfvars.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-06-23 06:47:15.000000 circlecigen-0.0.7/src/utils.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-23 06:47:21.290356 circlecigen-0.0.7/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5643 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/generated_config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1592 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/generated_config_setup.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/nonprod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/nonprod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/prod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/prod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2266 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/test_circlecigen.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2338 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/test_template.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2340 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/test_tfvars.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1490 2023-06-23 06:47:15.000000 circlecigen-0.0.7/test/test_utils.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 05:19:46.029237 circlecigen-0.0.8/
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 05:19:46.025237 circlecigen-0.0.8/.circleci/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3995 2023-06-27 05:19:41.000000 circlecigen-0.0.8/.circleci/config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      350 2023-06-27 05:19:41.000000 circlecigen-0.0.8/.codeclimate.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-27 05:19:41.000000 circlecigen-0.0.8/.gitignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-06-27 05:19:41.000000 circlecigen-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18369 2023-06-27 05:19:41.000000 circlecigen-0.0.8/.pylintrc
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2023-06-27 05:19:41.000000 circlecigen-0.0.8/.python-version
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-06-27 05:19:41.000000 circlecigen-0.0.8/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26079 2023-06-27 05:19:46.029237 circlecigen-0.0.8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      432 2023-06-27 05:19:41.000000 circlecigen-0.0.8/Pipfile
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25444 2023-06-27 05:19:41.000000 circlecigen-0.0.8/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-27 05:19:41.000000 circlecigen-0.0.8/__init__.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 05:19:46.025237 circlecigen-0.0.8/circlecigen.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26079 2023-06-27 05:19:46.000000 circlecigen-0.0.8/circlecigen.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1224 2023-06-27 05:19:46.000000 circlecigen-0.0.8/circlecigen.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-27 05:19:46.000000 circlecigen-0.0.8/circlecigen.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       52 2023-06-27 05:19:46.000000 circlecigen-0.0.8/circlecigen.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2023-06-27 05:19:46.000000 circlecigen-0.0.8/circlecigen.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2023-06-27 05:19:46.000000 circlecigen-0.0.8/circlecigen.egg-info/top_level.txt
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 05:19:46.029237 circlecigen-0.0.8/env_test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3037 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      367 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/custom.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/default.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       39 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/dev.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6273 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/multi.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/nonprod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/nonprod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/nonprod.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      587 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/post-approve.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      312 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/pre-approve.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/prod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/prod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/prod.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3684 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/template_generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      313 2023-06-27 05:19:41.000000 circlecigen-0.0.8/notes.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-06-27 05:19:41.000000 circlecigen-0.0.8/op.env
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      711 2023-06-27 05:19:41.000000 circlecigen-0.0.8/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      365 2023-06-27 05:19:41.000000 circlecigen-0.0.8/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-27 05:19:46.029237 circlecigen-0.0.8/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      847 2023-06-27 05:19:41.000000 circlecigen-0.0.8/setup.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 05:19:46.029237 circlecigen-0.0.8/src/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-27 05:19:41.000000 circlecigen-0.0.8/src/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      160 2023-06-27 05:19:45.000000 circlecigen-0.0.8/src/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3028 2023-06-27 05:19:41.000000 circlecigen-0.0.8/src/circlecigen.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6770 2023-06-27 05:19:41.000000 circlecigen-0.0.8/src/template.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2428 2023-06-27 05:19:41.000000 circlecigen-0.0.8/src/tfvars.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-06-27 05:19:41.000000 circlecigen-0.0.8/src/utils.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 05:19:46.029237 circlecigen-0.0.8/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6273 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2222 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/generated_config_setup.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/nonprod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/nonprod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/prod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/prod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3684 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/template_generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2536 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/test_circlecigen.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3444 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/test_template.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2340 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/test_tfvars.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1490 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/test_utils.py
```

### Comparing `circlecigen-0.0.7/.circleci/config.yml` & `circlecigen-0.0.8/.circleci/config.yml`

 * *Files 3% similar despite different names*

```diff
@@ -93,16 +93,15 @@
           name: report test coverage
           command: |
             cc-test-reporter format-coverage -t coverage.py
             cc-test-reporter upload-coverage
       - run:
           name: cve scan
           command: |
-            pipenv update
-            snyk test
+            snyk test --package-manager=pip --file=requirements.txt
 
   build package and integration test:
     executor: python-builder
     steps:
       - checkout
       - setup_remote_docker
       - op/env:
```

### Comparing `circlecigen-0.0.7/.pre-commit-config.yaml` & `circlecigen-0.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.7/.pylintrc` & `circlecigen-0.0.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.7/LICENSE` & `circlecigen-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.7/PKG-INFO` & `circlecigen-0.0.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: circlecigen
-Version: 0.0.7
-Summary: Opinionated generation of continuation pipelines
-Home-page: https://github.com/ThoughtWorks-DPS/circlecigen
-Author: Nic Cheneweth
-Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
-Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/circlecigen
-Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/circlecigen/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 	<p>
 		<img alt="Thoughtworks Logo" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/thoughtworks_flamingo_wave.png?sanitize=true" width=200 />
     <br />
 		<img alt="DPS Title" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/EMPCPlatformStarterKitsImage.png?sanitize=true" width=350/>
 	</p>
   <br />
@@ -49,15 +33,18 @@
 In simplest terms, you define templates of _pre-approval_ and _post-approval_ circleci workflow jobs that include jinja2 style variable-substitution formatting. 
 
 For all instances of each desired Role, circlecigen will generate a deployment pipeline that has:  
 * a pre-approve job for each instance, followed by
 * an approval step, followed by
 * a post-approve job for each instance
 
-#### Setup example for a terraform EKS pipeline
+Optionally, a custom template of a CircleCI workflow job can be defined and circlecigen will generate a deployment pipeline with jobs for all the instances running in parallel.
+
+### Setup Examples
+#### 1. Setup example for a terraform EKS pipeline
 
 Let's stay with the EKS example mentioned above. Assume that Production requires six (6) clusters in six different regions, Nonproduction likewise requires cluster in each of the same six regions, and an additional three clusters spanning nearby global localities are required to support the software-defined lifecycle of this infrastructure. Therefore we have three environment Roles: infra-dev role that is deployed on git-push, and the nonprod and prod roles that release consequtively upon git-tag.  
 
 Given the output of the actual deployment pipelines, this tool also supports generating the tfvar files for each cluster deployment.  
 
 First, let's define the top level pipelines, roles, and instances definition.   
 
@@ -466,14 +453,30 @@
 
   after-deployment-commands:
     parameters:
       ...
     steps:
       ...
 
+jobs:
+
+  my-pre-deploy-jobs:
+    parameters:
+      ...
+    docker:
+      - image: ...
+    steps:
+      - setup-commands:
+          parameters: << parameters... >>
+      - static-code-test-commands:
+          parameters: << parameters... >>
+
+  launch-dynamic-pipeline:
+    parameters:
+      ...
 
 workflows:
   version: 2
 
   release-pipeline:
     jobs:
       - terraform/plan:
@@ -654,7 +657,122 @@
           filters: *on-tag-main
 
       - terraform/apply:
           name: apply nonprod-ap-southwest-1 change plan
           ...
           filters: *on-tag-main
 ```
+
+#### 2. Setup example for a job to run nightly integration tests
+
+In this example we start by setting up the `environments/multi.json` and `environments/default.json` as from before. We also set up any relevant role-specific overrides, and the CircleCI config file (`.circleci/config.yml`) as from before.
+
+We then create a custom template file which will be specified with the `--template` flag. Let's use the example below:
+```yaml
+      - integration-tests:
+          name: {{env_instance}} integration test
+          context: << pipeline.parameters.context >>
+          shell: << pipeline.parameters.shell-options >>
+          executor-image: << pipeline.parameters.executor-image >>
+          instance_name: {{env_instance}}
+          workspace: {{env_instance}}
+          filters: {{filters}}
+```
+
+The resulting pipeline from using the above custom template would then look like the following:
+```yaml
+---
+version: 2.1
+
+orbs:
+  continuation: circleci/continuation@0.3.1
+
+on-push-main: &on-push-main
+  branches:
+    only: /main/
+  tags:
+    ignore: /.*/
+
+commands:
+
+  setup-commands:
+    parameters:
+      ...
+    steps:
+      ...
+
+  static-code-test-commands:
+    parameters:
+      ...
+    steps:
+      ...
+
+  before-instance-specific-parallel-job-commands:
+    parameters:
+      ...
+    steps:
+      ...
+
+  after-instance-specific-parallel-job-commands:
+    parameters:
+      ...
+    steps:
+      ...
+
+jobs:
+
+  my-pre-deploy-jobs:
+    parameters:
+      ...
+    docker:
+      - image: ...
+    steps:
+      - setup-commands:
+          parameters: << parameters... >>
+      - static-code-test-commands:
+          parameters: << parameters... >>
+
+  launch-dynamic-pipeline:
+    parameters:
+      ...
+
+workflows:
+  version: 2
+
+  release-pipeline:
+    jobs:
+      - integration-tests:
+          name: nonprod-us-west-2 integration test
+          context: << pipeline.parameters.context >>
+          shell: << pipeline.parameters.shell-options >>
+          executor-image: << pipeline.parameters.executor-image >>
+          instance_name: nonprod-us-west-2
+          workspace: nonprod-us-west-2
+          filters: *on-push-main
+
+      - integration-tests:
+          name: nonprod-us-east-2 integration test
+          context: << pipeline.parameters.context >>
+          shell: << pipeline.parameters.shell-options >>
+          executor-image: << pipeline.parameters.executor-image >>
+          instance_name: nonprod-us-east-2
+          workspace: nonprod-us-east-2
+          filters: *on-push-main
+
+      - integration-tests:
+          name: prod-us-west-2 integration test
+          context: << pipeline.parameters.context >>
+          shell: << pipeline.parameters.shell-options >>
+          executor-image: << pipeline.parameters.executor-image >>
+          instance_name: prod-us-west-2
+          workspace: prod-us-west-2
+          filters: *on-push-main
+
+      - integration-tests:
+          name: prod-us-east-2 integration test
+          context: << pipeline.parameters.context >>
+          shell: << pipeline.parameters.shell-options >>
+          executor-image: << pipeline.parameters.executor-image >>
+          instance_name: prod-us-east-2
+          workspace: prod-us-east-2
+          filters: *on-push-main
+```
```

#### html2text {}

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1 Name: circlecigen Version: 0.0.7 Summary: Opinionated
-generation of continuation pipelines Home-page: https://github.com/
-ThoughtWorks-DPS/circlecigen Author: Nic Cheneweth Author-email: Nic Cheneweth
-thoughtworks.com> Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/
-circlecigen Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/
-circlecigen/issues Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
-License-File: LICENSE
                              [Thoughtworks Logo]
                                   [DPS Title]
 
                              **** circlecigen ****
 [https://dl.circleci.com/status-badge/img/gh/ThoughtWorks-DPS/circlecigen/tree/
   main.svg?style=shield] [https://img.shields.io/badge/license-MIT-blue.svg]
 
@@ -38,45 +29,47 @@
 in a single json file and the deployment pipeline is then generated to match at
 runtime? That is what this tool enables. Let's call the multi-instance
 environments `Roles`. In simplest terms, you define templates of _pre-approval_
 and _post-approval_ circleci workflow jobs that include jinja2 style variable-
 substitution formatting. For all instances of each desired Role, circlecigen
 will generate a deployment pipeline that has: * a pre-approve job for each
 instance, followed by * an approval step, followed by * a post-approve job for
-each instance #### Setup example for a terraform EKS pipeline Let's stay with
-the EKS example mentioned above. Assume that Production requires six (6)
-clusters in six different regions, Nonproduction likewise requires cluster in
-each of the same six regions, and an additional three clusters spanning nearby
-global localities are required to support the software-defined lifecycle of
-this infrastructure. Therefore we have three environment Roles: infra-dev role
-that is deployed on git-push, and the nonprod and prod roles that release
-consequtively upon git-tag. Given the output of the actual deployment
-pipelines, this tool also supports generating the tfvar files for each cluster
-deployment. First, let's define the top level pipelines, roles, and instances
-definition. **environments/multi.json** The top-level json definition groups
-roles by the circleci filter that will trigger the deployment of the associated
-Roles. Within each Role, define the instances that should exist. And finally
-list any particular settings associated with an individual instances. This
-multi-environment definition also defines the top-level pipeline structure for
-other pipelines with the same infrastructure path to production and should
-probably be maintained in a globally accessible location rather than
-duplicating the file in multiple repositories. For this example we assume this
-configuration has already been added locally as a file. ```json { "infradev":
-{ "filter": "*on-push-main", "infradev": { "infradev-us-east-2":
-{ "aws_region": "us-east-2", "aws_account_id": "10100000000" }, "infradev-eu-
-west-3": { "aws_region": "us-east-2", "aws_account_id": "10100000000" },
-"infradev-ap-southeast-3": { "aws_region": "eu-west-1", "aws_account_id":
-"10100000000" } } }, "release": { "filter": "*on-tag-main", "nonprod":
-{ "nonprod-us-west-2": { "aws_region": "us-west-2", "aws_account_id":
-"20100000000" }, "nonprod-us-east-2": { "aws_region": "us-east-2",
-"aws_account_id": "20100000000" }, "nonprod-eu-west-1": { "aws_region": "eu-
-west-1", "aws_account_id": "20100000000" }, "nonprod-eu-central-1":
-{ "aws_region": "eu-central-1", "aws_account_id": "20100000000" }, "nonprod-ap-
-southeast-2": { "aws_region": "ap-southeast-2", "aws_account_id": "20100000000"
-}, "nonprod-ap-southwest-1": { "aws_region": "ap-southwest-1",
+each instance Optionally, a custom template of a CircleCI workflow job can be
+defined and circlecigen will generate a deployment pipeline with jobs for all
+the instances running in parallel. ### Setup Examples #### 1. Setup example for
+a terraform EKS pipeline Let's stay with the EKS example mentioned above.
+Assume that Production requires six (6) clusters in six different regions,
+Nonproduction likewise requires cluster in each of the same six regions, and an
+additional three clusters spanning nearby global localities are required to
+support the software-defined lifecycle of this infrastructure. Therefore we
+have three environment Roles: infra-dev role that is deployed on git-push, and
+the nonprod and prod roles that release consequtively upon git-tag. Given the
+output of the actual deployment pipelines, this tool also supports generating
+the tfvar files for each cluster deployment. First, let's define the top level
+pipelines, roles, and instances definition. **environments/multi.json** The
+top-level json definition groups roles by the circleci filter that will trigger
+the deployment of the associated Roles. Within each Role, define the instances
+that should exist. And finally list any particular settings associated with an
+individual instances. This multi-environment definition also defines the top-
+level pipeline structure for other pipelines with the same infrastructure path
+to production and should probably be maintained in a globally accessible
+location rather than duplicating the file in multiple repositories. For this
+example we assume this configuration has already been added locally as a file.
+```json { "infradev": { "filter": "*on-push-main", "infradev": { "infradev-us-
+east-2": { "aws_region": "us-east-2", "aws_account_id": "10100000000" },
+"infradev-eu-west-3": { "aws_region": "us-east-2", "aws_account_id":
+"10100000000" }, "infradev-ap-southeast-3": { "aws_region": "eu-west-1",
+"aws_account_id": "10100000000" } } }, "release": { "filter": "*on-tag-main",
+"nonprod": { "nonprod-us-west-2": { "aws_region": "us-west-2",
+"aws_account_id": "20100000000" }, "nonprod-us-east-2": { "aws_region": "us-
+east-2", "aws_account_id": "20100000000" }, "nonprod-eu-west-1":
+{ "aws_region": "eu-west-1", "aws_account_id": "20100000000" }, "nonprod-eu-
+central-1": { "aws_region": "eu-central-1", "aws_account_id": "20100000000" },
+"nonprod-ap-southeast-2": { "aws_region": "ap-southeast-2", "aws_account_id":
+"20100000000" }, "nonprod-ap-southwest-1": { "aws_region": "ap-southwest-1",
 "aws_account_id": "20100000000" } }, "prod": { "prod-us-west-2":
 { "aws_region": "us-west-2", "aws_account_id": "30100000000" }, "prod-us-east-
 2": { "aws_region": "us-east-2", "aws_account_id": "30100000000" }, "prod-eu-
 west-1": { "aws_region": "eu-west-1", "aws_account_id": "30100000000" }, "prod-
 eu-central-1": { "aws_region": "eu-central-1", "aws_account_id": "30100000000"
 }, "prod-ap-southeast-2": { "aws_region": "ap-southeast-2", "aws_account_id":
 "30100000000" }, "prod-ap-southwest-1": { "aws_region": "ap-southwest-1",
@@ -202,16 +195,19 @@
 the more elaborate release system, but as is nearly always the case, the need
 to deploy will have deadlines that will be sooner than such an adoption.
 ```yaml version: 2.1 orbs: continuation: circleci/continuation@0.3.1 on-push-
 main: &on-push-main branches: only: /main/ tags: ignore: /.*/ on-tag-main: &on-
 tag-main branches: ignore: /.*/ tags: only: /.*/ commands: setup-commands:
 parameters: ... steps: ... static-code-test-commands: parameters: ... steps:
 ... before-deployment-commands: parameters: ... steps: ... after-deployment-
-commands: parameters: ... steps: ... workflows: version: 2 release-pipeline:
-jobs: - terraform/plan: name: nonprod-us-west-2 change plan context: <<
+commands: parameters: ... steps: ... jobs: my-pre-deploy-jobs: parameters: ...
+docker: - image: ... steps: - setup-commands: parameters: << parameters... >> -
+static-code-test-commands: parameters: << parameters... >> launch-dynamic-
+pipeline: parameters: ... workflows: version: 2 release-pipeline: jobs: -
+terraform/plan: name: nonprod-us-west-2 change plan context: <<
 pipeline.parameters.context >> workspace: nonprod-us-west-2 var-file: env_test/
 nonprod-us-west-2.tfvars.json before-terraform: - set-environment filters: *on-
 tag-main - terraform/plan: name: nonprod-us-east-2 change plan context: <<
 pipeline.parameters.context >> workspace: nonprod-us-east-2 var-file: env_test/
 nonprod-us-east-2.tfvars.json before-terraform: - set-environment filters: *on-
 tag-main - terraform/plan: name: nonprod-eu-west-1 change plan ... filters:
 *on-tag-main - terraform/plan: name: nonprod-eu-central-1 change plan ...
@@ -252,8 +248,43 @@
 terraform: - after-deployment-commands requires: - approve nonprod changes
 filters: *on-tag-main - terraform/apply: name: apply nonprod-us-east-2 change
 plan ... filters: *on-tag-main - terraform/apply: name: apply nonprod-eu-west-
 1 change plan ... filters: *on-tag-main - terraform/apply: name: apply nonprod-
 eu-central-1 change plan ... filters: *on-tag-main - terraform/apply: name:
 apply nonprod-ap-southeast-2 change plan ... filters: *on-tag-main - terraform/
 apply: name: apply nonprod-ap-southwest-1 change plan ... filters: *on-tag-main
-```
+``` #### 2. Setup example for a job to run nightly integration tests In this
+example we start by setting up the `environments/multi.json` and `environments/
+default.json` as from before. We also set up any relevant role-specific
+overrides, and the CircleCI config file (`.circleci/config.yml`) as from
+before. We then create a custom template file which will be specified with the
+`--template` flag. Let's use the example below: ```yaml - integration-tests:
+name: {{env_instance}} integration test context: << pipeline.parameters.context
+>> shell: << pipeline.parameters.shell-options >> executor-image: <<
+pipeline.parameters.executor-image >> instance_name: {{env_instance}}
+workspace: {{env_instance}} filters: {{filters}} ``` The resulting pipeline
+from using the above custom template would then look like the following:
+```yaml --- version: 2.1 orbs: continuation: circleci/continuation@0.3.1 on-
+push-main: &on-push-main branches: only: /main/ tags: ignore: /.*/ commands:
+setup-commands: parameters: ... steps: ... static-code-test-commands:
+parameters: ... steps: ... before-instance-specific-parallel-job-commands:
+parameters: ... steps: ... after-instance-specific-parallel-job-commands:
+parameters: ... steps: ... jobs: my-pre-deploy-jobs: parameters: ... docker: -
+image: ... steps: - setup-commands: parameters: << parameters... >> - static-
+code-test-commands: parameters: << parameters... >> launch-dynamic-pipeline:
+parameters: ... workflows: version: 2 release-pipeline: jobs: - integration-
+tests: name: nonprod-us-west-2 integration test context: <<
+pipeline.parameters.context >> shell: << pipeline.parameters.shell-options >>
+executor-image: << pipeline.parameters.executor-image >> instance_name:
+nonprod-us-west-2 workspace: nonprod-us-west-2 filters: *on-push-main -
+integration-tests: name: nonprod-us-east-2 integration test context: <<
+pipeline.parameters.context >> shell: << pipeline.parameters.shell-options >>
+executor-image: << pipeline.parameters.executor-image >> instance_name:
+nonprod-us-east-2 workspace: nonprod-us-east-2 filters: *on-push-main -
+integration-tests: name: prod-us-west-2 integration test context: <<
+pipeline.parameters.context >> shell: << pipeline.parameters.shell-options >>
+executor-image: << pipeline.parameters.executor-image >> instance_name: prod-
+us-west-2 workspace: prod-us-west-2 filters: *on-push-main - integration-tests:
+name: prod-us-east-2 integration test context: << pipeline.parameters.context
+>> shell: << pipeline.parameters.shell-options >> executor-image: <<
+pipeline.parameters.executor-image >> instance_name: prod-us-east-2 workspace:
+prod-us-east-2 filters: *on-push-main ```
```

### Comparing `circlecigen-0.0.7/README.md` & `circlecigen-0.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: circlecigen
+Version: 0.0.8
+Summary: Opinionated generation of continuation pipelines
+Home-page: https://github.com/ThoughtWorks-DPS/circlecigen
+Author: Nic Cheneweth
+Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
+Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/circlecigen
+Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/circlecigen/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 	<p>
 		<img alt="Thoughtworks Logo" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/thoughtworks_flamingo_wave.png?sanitize=true" width=200 />
     <br />
 		<img alt="DPS Title" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/EMPCPlatformStarterKitsImage.png?sanitize=true" width=350/>
 	</p>
   <br />
@@ -33,15 +49,18 @@
 In simplest terms, you define templates of _pre-approval_ and _post-approval_ circleci workflow jobs that include jinja2 style variable-substitution formatting. 
 
 For all instances of each desired Role, circlecigen will generate a deployment pipeline that has:  
 * a pre-approve job for each instance, followed by
 * an approval step, followed by
 * a post-approve job for each instance
 
-#### Setup example for a terraform EKS pipeline
+Optionally, a custom template of a CircleCI workflow job can be defined and circlecigen will generate a deployment pipeline with jobs for all the instances running in parallel.
+
+### Setup Examples
+#### 1. Setup example for a terraform EKS pipeline
 
 Let's stay with the EKS example mentioned above. Assume that Production requires six (6) clusters in six different regions, Nonproduction likewise requires cluster in each of the same six regions, and an additional three clusters spanning nearby global localities are required to support the software-defined lifecycle of this infrastructure. Therefore we have three environment Roles: infra-dev role that is deployed on git-push, and the nonprod and prod roles that release consequtively upon git-tag.  
 
 Given the output of the actual deployment pipelines, this tool also supports generating the tfvar files for each cluster deployment.  
 
 First, let's define the top level pipelines, roles, and instances definition.   
 
@@ -450,14 +469,30 @@
 
   after-deployment-commands:
     parameters:
       ...
     steps:
       ...
 
+jobs:
+
+  my-pre-deploy-jobs:
+    parameters:
+      ...
+    docker:
+      - image: ...
+    steps:
+      - setup-commands:
+          parameters: << parameters... >>
+      - static-code-test-commands:
+          parameters: << parameters... >>
+
+  launch-dynamic-pipeline:
+    parameters:
+      ...
 
 workflows:
   version: 2
 
   release-pipeline:
     jobs:
       - terraform/plan:
@@ -637,8 +672,123 @@
           ...
           filters: *on-tag-main
 
       - terraform/apply:
           name: apply nonprod-ap-southwest-1 change plan
           ...
           filters: *on-tag-main
-```
+```
+
+#### 2. Setup example for a job to run nightly integration tests
+
+In this example we start by setting up the `environments/multi.json` and `environments/default.json` as from before. We also set up any relevant role-specific overrides, and the CircleCI config file (`.circleci/config.yml`) as from before.
+
+We then create a custom template file which will be specified with the `--template` flag. Let's use the example below:
+```yaml
+      - integration-tests:
+          name: {{env_instance}} integration test
+          context: << pipeline.parameters.context >>
+          shell: << pipeline.parameters.shell-options >>
+          executor-image: << pipeline.parameters.executor-image >>
+          instance_name: {{env_instance}}
+          workspace: {{env_instance}}
+          filters: {{filters}}
+```
+
+The resulting pipeline from using the above custom template would then look like the following:
+```yaml
+---
+version: 2.1
+
+orbs:
+  continuation: circleci/continuation@0.3.1
+
+on-push-main: &on-push-main
+  branches:
+    only: /main/
+  tags:
+    ignore: /.*/
+
+commands:
+
+  setup-commands:
+    parameters:
+      ...
+    steps:
+      ...
+
+  static-code-test-commands:
+    parameters:
+      ...
+    steps:
+      ...
+
+  before-instance-specific-parallel-job-commands:
+    parameters:
+      ...
+    steps:
+      ...
+
+  after-instance-specific-parallel-job-commands:
+    parameters:
+      ...
+    steps:
+      ...
+
+jobs:
+
+  my-pre-deploy-jobs:
+    parameters:
+      ...
+    docker:
+      - image: ...
+    steps:
+      - setup-commands:
+          parameters: << parameters... >>
+      - static-code-test-commands:
+          parameters: << parameters... >>
+
+  launch-dynamic-pipeline:
+    parameters:
+      ...
+
+workflows:
+  version: 2
+
+  release-pipeline:
+    jobs:
+      - integration-tests:
+          name: nonprod-us-west-2 integration test
+          context: << pipeline.parameters.context >>
+          shell: << pipeline.parameters.shell-options >>
+          executor-image: << pipeline.parameters.executor-image >>
+          instance_name: nonprod-us-west-2
+          workspace: nonprod-us-west-2
+          filters: *on-push-main
+
+      - integration-tests:
+          name: nonprod-us-east-2 integration test
+          context: << pipeline.parameters.context >>
+          shell: << pipeline.parameters.shell-options >>
+          executor-image: << pipeline.parameters.executor-image >>
+          instance_name: nonprod-us-east-2
+          workspace: nonprod-us-east-2
+          filters: *on-push-main
+
+      - integration-tests:
+          name: prod-us-west-2 integration test
+          context: << pipeline.parameters.context >>
+          shell: << pipeline.parameters.shell-options >>
+          executor-image: << pipeline.parameters.executor-image >>
+          instance_name: prod-us-west-2
+          workspace: prod-us-west-2
+          filters: *on-push-main
+
+      - integration-tests:
+          name: prod-us-east-2 integration test
+          context: << pipeline.parameters.context >>
+          shell: << pipeline.parameters.shell-options >>
+          executor-image: << pipeline.parameters.executor-image >>
+          instance_name: prod-us-east-2
+          workspace: prod-us-east-2
+          filters: *on-push-main
+```
```

#### html2text {}

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1 Name: circlecigen Version: 0.0.8 Summary: Opinionated
+generation of continuation pipelines Home-page: https://github.com/
+ThoughtWorks-DPS/circlecigen Author: Nic Cheneweth Author-email: Nic Cheneweth
+thoughtworks.com> Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/
+circlecigen Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/
+circlecigen/issues Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE
                              [Thoughtworks Logo]
                                   [DPS Title]
 
                              **** circlecigen ****
 [https://dl.circleci.com/status-badge/img/gh/ThoughtWorks-DPS/circlecigen/tree/
   main.svg?style=shield] [https://img.shields.io/badge/license-MIT-blue.svg]
 
@@ -29,45 +38,47 @@
 in a single json file and the deployment pipeline is then generated to match at
 runtime? That is what this tool enables. Let's call the multi-instance
 environments `Roles`. In simplest terms, you define templates of _pre-approval_
 and _post-approval_ circleci workflow jobs that include jinja2 style variable-
 substitution formatting. For all instances of each desired Role, circlecigen
 will generate a deployment pipeline that has: * a pre-approve job for each
 instance, followed by * an approval step, followed by * a post-approve job for
-each instance #### Setup example for a terraform EKS pipeline Let's stay with
-the EKS example mentioned above. Assume that Production requires six (6)
-clusters in six different regions, Nonproduction likewise requires cluster in
-each of the same six regions, and an additional three clusters spanning nearby
-global localities are required to support the software-defined lifecycle of
-this infrastructure. Therefore we have three environment Roles: infra-dev role
-that is deployed on git-push, and the nonprod and prod roles that release
-consequtively upon git-tag. Given the output of the actual deployment
-pipelines, this tool also supports generating the tfvar files for each cluster
-deployment. First, let's define the top level pipelines, roles, and instances
-definition. **environments/multi.json** The top-level json definition groups
-roles by the circleci filter that will trigger the deployment of the associated
-Roles. Within each Role, define the instances that should exist. And finally
-list any particular settings associated with an individual instances. This
-multi-environment definition also defines the top-level pipeline structure for
-other pipelines with the same infrastructure path to production and should
-probably be maintained in a globally accessible location rather than
-duplicating the file in multiple repositories. For this example we assume this
-configuration has already been added locally as a file. ```json { "infradev":
-{ "filter": "*on-push-main", "infradev": { "infradev-us-east-2":
-{ "aws_region": "us-east-2", "aws_account_id": "10100000000" }, "infradev-eu-
-west-3": { "aws_region": "us-east-2", "aws_account_id": "10100000000" },
-"infradev-ap-southeast-3": { "aws_region": "eu-west-1", "aws_account_id":
-"10100000000" } } }, "release": { "filter": "*on-tag-main", "nonprod":
-{ "nonprod-us-west-2": { "aws_region": "us-west-2", "aws_account_id":
-"20100000000" }, "nonprod-us-east-2": { "aws_region": "us-east-2",
-"aws_account_id": "20100000000" }, "nonprod-eu-west-1": { "aws_region": "eu-
-west-1", "aws_account_id": "20100000000" }, "nonprod-eu-central-1":
-{ "aws_region": "eu-central-1", "aws_account_id": "20100000000" }, "nonprod-ap-
-southeast-2": { "aws_region": "ap-southeast-2", "aws_account_id": "20100000000"
-}, "nonprod-ap-southwest-1": { "aws_region": "ap-southwest-1",
+each instance Optionally, a custom template of a CircleCI workflow job can be
+defined and circlecigen will generate a deployment pipeline with jobs for all
+the instances running in parallel. ### Setup Examples #### 1. Setup example for
+a terraform EKS pipeline Let's stay with the EKS example mentioned above.
+Assume that Production requires six (6) clusters in six different regions,
+Nonproduction likewise requires cluster in each of the same six regions, and an
+additional three clusters spanning nearby global localities are required to
+support the software-defined lifecycle of this infrastructure. Therefore we
+have three environment Roles: infra-dev role that is deployed on git-push, and
+the nonprod and prod roles that release consequtively upon git-tag. Given the
+output of the actual deployment pipelines, this tool also supports generating
+the tfvar files for each cluster deployment. First, let's define the top level
+pipelines, roles, and instances definition. **environments/multi.json** The
+top-level json definition groups roles by the circleci filter that will trigger
+the deployment of the associated Roles. Within each Role, define the instances
+that should exist. And finally list any particular settings associated with an
+individual instances. This multi-environment definition also defines the top-
+level pipeline structure for other pipelines with the same infrastructure path
+to production and should probably be maintained in a globally accessible
+location rather than duplicating the file in multiple repositories. For this
+example we assume this configuration has already been added locally as a file.
+```json { "infradev": { "filter": "*on-push-main", "infradev": { "infradev-us-
+east-2": { "aws_region": "us-east-2", "aws_account_id": "10100000000" },
+"infradev-eu-west-3": { "aws_region": "us-east-2", "aws_account_id":
+"10100000000" }, "infradev-ap-southeast-3": { "aws_region": "eu-west-1",
+"aws_account_id": "10100000000" } } }, "release": { "filter": "*on-tag-main",
+"nonprod": { "nonprod-us-west-2": { "aws_region": "us-west-2",
+"aws_account_id": "20100000000" }, "nonprod-us-east-2": { "aws_region": "us-
+east-2", "aws_account_id": "20100000000" }, "nonprod-eu-west-1":
+{ "aws_region": "eu-west-1", "aws_account_id": "20100000000" }, "nonprod-eu-
+central-1": { "aws_region": "eu-central-1", "aws_account_id": "20100000000" },
+"nonprod-ap-southeast-2": { "aws_region": "ap-southeast-2", "aws_account_id":
+"20100000000" }, "nonprod-ap-southwest-1": { "aws_region": "ap-southwest-1",
 "aws_account_id": "20100000000" } }, "prod": { "prod-us-west-2":
 { "aws_region": "us-west-2", "aws_account_id": "30100000000" }, "prod-us-east-
 2": { "aws_region": "us-east-2", "aws_account_id": "30100000000" }, "prod-eu-
 west-1": { "aws_region": "eu-west-1", "aws_account_id": "30100000000" }, "prod-
 eu-central-1": { "aws_region": "eu-central-1", "aws_account_id": "30100000000"
 }, "prod-ap-southeast-2": { "aws_region": "ap-southeast-2", "aws_account_id":
 "30100000000" }, "prod-ap-southwest-1": { "aws_region": "ap-southwest-1",
@@ -193,16 +204,19 @@
 the more elaborate release system, but as is nearly always the case, the need
 to deploy will have deadlines that will be sooner than such an adoption.
 ```yaml version: 2.1 orbs: continuation: circleci/continuation@0.3.1 on-push-
 main: &on-push-main branches: only: /main/ tags: ignore: /.*/ on-tag-main: &on-
 tag-main branches: ignore: /.*/ tags: only: /.*/ commands: setup-commands:
 parameters: ... steps: ... static-code-test-commands: parameters: ... steps:
 ... before-deployment-commands: parameters: ... steps: ... after-deployment-
-commands: parameters: ... steps: ... workflows: version: 2 release-pipeline:
-jobs: - terraform/plan: name: nonprod-us-west-2 change plan context: <<
+commands: parameters: ... steps: ... jobs: my-pre-deploy-jobs: parameters: ...
+docker: - image: ... steps: - setup-commands: parameters: << parameters... >> -
+static-code-test-commands: parameters: << parameters... >> launch-dynamic-
+pipeline: parameters: ... workflows: version: 2 release-pipeline: jobs: -
+terraform/plan: name: nonprod-us-west-2 change plan context: <<
 pipeline.parameters.context >> workspace: nonprod-us-west-2 var-file: env_test/
 nonprod-us-west-2.tfvars.json before-terraform: - set-environment filters: *on-
 tag-main - terraform/plan: name: nonprod-us-east-2 change plan context: <<
 pipeline.parameters.context >> workspace: nonprod-us-east-2 var-file: env_test/
 nonprod-us-east-2.tfvars.json before-terraform: - set-environment filters: *on-
 tag-main - terraform/plan: name: nonprod-eu-west-1 change plan ... filters:
 *on-tag-main - terraform/plan: name: nonprod-eu-central-1 change plan ...
@@ -243,8 +257,43 @@
 terraform: - after-deployment-commands requires: - approve nonprod changes
 filters: *on-tag-main - terraform/apply: name: apply nonprod-us-east-2 change
 plan ... filters: *on-tag-main - terraform/apply: name: apply nonprod-eu-west-
 1 change plan ... filters: *on-tag-main - terraform/apply: name: apply nonprod-
 eu-central-1 change plan ... filters: *on-tag-main - terraform/apply: name:
 apply nonprod-ap-southeast-2 change plan ... filters: *on-tag-main - terraform/
 apply: name: apply nonprod-ap-southwest-1 change plan ... filters: *on-tag-main
-```
+``` #### 2. Setup example for a job to run nightly integration tests In this
+example we start by setting up the `environments/multi.json` and `environments/
+default.json` as from before. We also set up any relevant role-specific
+overrides, and the CircleCI config file (`.circleci/config.yml`) as from
+before. We then create a custom template file which will be specified with the
+`--template` flag. Let's use the example below: ```yaml - integration-tests:
+name: {{env_instance}} integration test context: << pipeline.parameters.context
+>> shell: << pipeline.parameters.shell-options >> executor-image: <<
+pipeline.parameters.executor-image >> instance_name: {{env_instance}}
+workspace: {{env_instance}} filters: {{filters}} ``` The resulting pipeline
+from using the above custom template would then look like the following:
+```yaml --- version: 2.1 orbs: continuation: circleci/continuation@0.3.1 on-
+push-main: &on-push-main branches: only: /main/ tags: ignore: /.*/ commands:
+setup-commands: parameters: ... steps: ... static-code-test-commands:
+parameters: ... steps: ... before-instance-specific-parallel-job-commands:
+parameters: ... steps: ... after-instance-specific-parallel-job-commands:
+parameters: ... steps: ... jobs: my-pre-deploy-jobs: parameters: ... docker: -
+image: ... steps: - setup-commands: parameters: << parameters... >> - static-
+code-test-commands: parameters: << parameters... >> launch-dynamic-pipeline:
+parameters: ... workflows: version: 2 release-pipeline: jobs: - integration-
+tests: name: nonprod-us-west-2 integration test context: <<
+pipeline.parameters.context >> shell: << pipeline.parameters.shell-options >>
+executor-image: << pipeline.parameters.executor-image >> instance_name:
+nonprod-us-west-2 workspace: nonprod-us-west-2 filters: *on-push-main -
+integration-tests: name: nonprod-us-east-2 integration test context: <<
+pipeline.parameters.context >> shell: << pipeline.parameters.shell-options >>
+executor-image: << pipeline.parameters.executor-image >> instance_name:
+nonprod-us-east-2 workspace: nonprod-us-east-2 filters: *on-push-main -
+integration-tests: name: prod-us-west-2 integration test context: <<
+pipeline.parameters.context >> shell: << pipeline.parameters.shell-options >>
+executor-image: << pipeline.parameters.executor-image >> instance_name: prod-
+us-west-2 workspace: prod-us-west-2 filters: *on-push-main - integration-tests:
+name: prod-us-east-2 integration test context: << pipeline.parameters.context
+>> shell: << pipeline.parameters.shell-options >> executor-image: <<
+pipeline.parameters.executor-image >> instance_name: prod-us-east-2 workspace:
+prod-us-east-2 filters: *on-push-main ```
```

### Comparing `circlecigen-0.0.7/circlecigen.egg-info/PKG-INFO` & `circlecigen-0.0.8/circlecigen.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circlecigen
-Version: 0.0.7
+Version: 0.0.8
 Summary: Opinionated generation of continuation pipelines
 Home-page: https://github.com/ThoughtWorks-DPS/circlecigen
 Author: Nic Cheneweth
 Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
 Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/circlecigen
 Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/circlecigen/issues
 Classifier: Programming Language :: Python :: 3
@@ -49,15 +49,18 @@
 In simplest terms, you define templates of _pre-approval_ and _post-approval_ circleci workflow jobs that include jinja2 style variable-substitution formatting. 
 
 For all instances of each desired Role, circlecigen will generate a deployment pipeline that has:  
 * a pre-approve job for each instance, followed by
 * an approval step, followed by
 * a post-approve job for each instance
 
-#### Setup example for a terraform EKS pipeline
+Optionally, a custom template of a CircleCI workflow job can be defined and circlecigen will generate a deployment pipeline with jobs for all the instances running in parallel.
+
+### Setup Examples
+#### 1. Setup example for a terraform EKS pipeline
 
 Let's stay with the EKS example mentioned above. Assume that Production requires six (6) clusters in six different regions, Nonproduction likewise requires cluster in each of the same six regions, and an additional three clusters spanning nearby global localities are required to support the software-defined lifecycle of this infrastructure. Therefore we have three environment Roles: infra-dev role that is deployed on git-push, and the nonprod and prod roles that release consequtively upon git-tag.  
 
 Given the output of the actual deployment pipelines, this tool also supports generating the tfvar files for each cluster deployment.  
 
 First, let's define the top level pipelines, roles, and instances definition.   
 
@@ -466,14 +469,30 @@
 
   after-deployment-commands:
     parameters:
       ...
     steps:
       ...
 
+jobs:
+
+  my-pre-deploy-jobs:
+    parameters:
+      ...
+    docker:
+      - image: ...
+    steps:
+      - setup-commands:
+          parameters: << parameters... >>
+      - static-code-test-commands:
+          parameters: << parameters... >>
+
+  launch-dynamic-pipeline:
+    parameters:
+      ...
 
 workflows:
   version: 2
 
   release-pipeline:
     jobs:
       - terraform/plan:
@@ -654,7 +673,122 @@
           filters: *on-tag-main
 
       - terraform/apply:
           name: apply nonprod-ap-southwest-1 change plan
           ...
           filters: *on-tag-main
 ```
+
+#### 2. Setup example for a job to run nightly integration tests
+
+In this example we start by setting up the `environments/multi.json` and `environments/default.json` as from before. We also set up any relevant role-specific overrides, and the CircleCI config file (`.circleci/config.yml`) as from before.
+
+We then create a custom template file which will be specified with the `--template` flag. Let's use the example below:
+```yaml
+      - integration-tests:
+          name: {{env_instance}} integration test
+          context: << pipeline.parameters.context >>
+          shell: << pipeline.parameters.shell-options >>
+          executor-image: << pipeline.parameters.executor-image >>
+          instance_name: {{env_instance}}
+          workspace: {{env_instance}}
+          filters: {{filters}}
+```
+
+The resulting pipeline from using the above custom template would then look like the following:
+```yaml
+---
+version: 2.1
+
+orbs:
+  continuation: circleci/continuation@0.3.1
+
+on-push-main: &on-push-main
+  branches:
+    only: /main/
+  tags:
+    ignore: /.*/
+
+commands:
+
+  setup-commands:
+    parameters:
+      ...
+    steps:
+      ...
+
+  static-code-test-commands:
+    parameters:
+      ...
+    steps:
+      ...
+
+  before-instance-specific-parallel-job-commands:
+    parameters:
+      ...
+    steps:
+      ...
+
+  after-instance-specific-parallel-job-commands:
+    parameters:
+      ...
+    steps:
+      ...
+
+jobs:
+
+  my-pre-deploy-jobs:
+    parameters:
+      ...
+    docker:
+      - image: ...
+    steps:
+      - setup-commands:
+          parameters: << parameters... >>
+      - static-code-test-commands:
+          parameters: << parameters... >>
+
+  launch-dynamic-pipeline:
+    parameters:
+      ...
+
+workflows:
+  version: 2
+
+  release-pipeline:
+    jobs:
+      - integration-tests:
+          name: nonprod-us-west-2 integration test
+          context: << pipeline.parameters.context >>
+          shell: << pipeline.parameters.shell-options >>
+          executor-image: << pipeline.parameters.executor-image >>
+          instance_name: nonprod-us-west-2
+          workspace: nonprod-us-west-2
+          filters: *on-push-main
+
+      - integration-tests:
+          name: nonprod-us-east-2 integration test
+          context: << pipeline.parameters.context >>
+          shell: << pipeline.parameters.shell-options >>
+          executor-image: << pipeline.parameters.executor-image >>
+          instance_name: nonprod-us-east-2
+          workspace: nonprod-us-east-2
+          filters: *on-push-main
+
+      - integration-tests:
+          name: prod-us-west-2 integration test
+          context: << pipeline.parameters.context >>
+          shell: << pipeline.parameters.shell-options >>
+          executor-image: << pipeline.parameters.executor-image >>
+          instance_name: prod-us-west-2
+          workspace: prod-us-west-2
+          filters: *on-push-main
+
+      - integration-tests:
+          name: prod-us-east-2 integration test
+          context: << pipeline.parameters.context >>
+          shell: << pipeline.parameters.shell-options >>
+          executor-image: << pipeline.parameters.executor-image >>
+          instance_name: prod-us-east-2
+          workspace: prod-us-east-2
+          filters: *on-push-main
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: circlecigen Version: 0.0.7 Summary: Opinionated
+Metadata-Version: 2.1 Name: circlecigen Version: 0.0.8 Summary: Opinionated
 generation of continuation pipelines Home-page: https://github.com/
 ThoughtWorks-DPS/circlecigen Author: Nic Cheneweth Author-email: Nic Cheneweth
 thoughtworks.com> Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/
 circlecigen Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/
 circlecigen/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
@@ -38,45 +38,47 @@
 in a single json file and the deployment pipeline is then generated to match at
 runtime? That is what this tool enables. Let's call the multi-instance
 environments `Roles`. In simplest terms, you define templates of _pre-approval_
 and _post-approval_ circleci workflow jobs that include jinja2 style variable-
 substitution formatting. For all instances of each desired Role, circlecigen
 will generate a deployment pipeline that has: * a pre-approve job for each
 instance, followed by * an approval step, followed by * a post-approve job for
-each instance #### Setup example for a terraform EKS pipeline Let's stay with
-the EKS example mentioned above. Assume that Production requires six (6)
-clusters in six different regions, Nonproduction likewise requires cluster in
-each of the same six regions, and an additional three clusters spanning nearby
-global localities are required to support the software-defined lifecycle of
-this infrastructure. Therefore we have three environment Roles: infra-dev role
-that is deployed on git-push, and the nonprod and prod roles that release
-consequtively upon git-tag. Given the output of the actual deployment
-pipelines, this tool also supports generating the tfvar files for each cluster
-deployment. First, let's define the top level pipelines, roles, and instances
-definition. **environments/multi.json** The top-level json definition groups
-roles by the circleci filter that will trigger the deployment of the associated
-Roles. Within each Role, define the instances that should exist. And finally
-list any particular settings associated with an individual instances. This
-multi-environment definition also defines the top-level pipeline structure for
-other pipelines with the same infrastructure path to production and should
-probably be maintained in a globally accessible location rather than
-duplicating the file in multiple repositories. For this example we assume this
-configuration has already been added locally as a file. ```json { "infradev":
-{ "filter": "*on-push-main", "infradev": { "infradev-us-east-2":
-{ "aws_region": "us-east-2", "aws_account_id": "10100000000" }, "infradev-eu-
-west-3": { "aws_region": "us-east-2", "aws_account_id": "10100000000" },
-"infradev-ap-southeast-3": { "aws_region": "eu-west-1", "aws_account_id":
-"10100000000" } } }, "release": { "filter": "*on-tag-main", "nonprod":
-{ "nonprod-us-west-2": { "aws_region": "us-west-2", "aws_account_id":
-"20100000000" }, "nonprod-us-east-2": { "aws_region": "us-east-2",
-"aws_account_id": "20100000000" }, "nonprod-eu-west-1": { "aws_region": "eu-
-west-1", "aws_account_id": "20100000000" }, "nonprod-eu-central-1":
-{ "aws_region": "eu-central-1", "aws_account_id": "20100000000" }, "nonprod-ap-
-southeast-2": { "aws_region": "ap-southeast-2", "aws_account_id": "20100000000"
-}, "nonprod-ap-southwest-1": { "aws_region": "ap-southwest-1",
+each instance Optionally, a custom template of a CircleCI workflow job can be
+defined and circlecigen will generate a deployment pipeline with jobs for all
+the instances running in parallel. ### Setup Examples #### 1. Setup example for
+a terraform EKS pipeline Let's stay with the EKS example mentioned above.
+Assume that Production requires six (6) clusters in six different regions,
+Nonproduction likewise requires cluster in each of the same six regions, and an
+additional three clusters spanning nearby global localities are required to
+support the software-defined lifecycle of this infrastructure. Therefore we
+have three environment Roles: infra-dev role that is deployed on git-push, and
+the nonprod and prod roles that release consequtively upon git-tag. Given the
+output of the actual deployment pipelines, this tool also supports generating
+the tfvar files for each cluster deployment. First, let's define the top level
+pipelines, roles, and instances definition. **environments/multi.json** The
+top-level json definition groups roles by the circleci filter that will trigger
+the deployment of the associated Roles. Within each Role, define the instances
+that should exist. And finally list any particular settings associated with an
+individual instances. This multi-environment definition also defines the top-
+level pipeline structure for other pipelines with the same infrastructure path
+to production and should probably be maintained in a globally accessible
+location rather than duplicating the file in multiple repositories. For this
+example we assume this configuration has already been added locally as a file.
+```json { "infradev": { "filter": "*on-push-main", "infradev": { "infradev-us-
+east-2": { "aws_region": "us-east-2", "aws_account_id": "10100000000" },
+"infradev-eu-west-3": { "aws_region": "us-east-2", "aws_account_id":
+"10100000000" }, "infradev-ap-southeast-3": { "aws_region": "eu-west-1",
+"aws_account_id": "10100000000" } } }, "release": { "filter": "*on-tag-main",
+"nonprod": { "nonprod-us-west-2": { "aws_region": "us-west-2",
+"aws_account_id": "20100000000" }, "nonprod-us-east-2": { "aws_region": "us-
+east-2", "aws_account_id": "20100000000" }, "nonprod-eu-west-1":
+{ "aws_region": "eu-west-1", "aws_account_id": "20100000000" }, "nonprod-eu-
+central-1": { "aws_region": "eu-central-1", "aws_account_id": "20100000000" },
+"nonprod-ap-southeast-2": { "aws_region": "ap-southeast-2", "aws_account_id":
+"20100000000" }, "nonprod-ap-southwest-1": { "aws_region": "ap-southwest-1",
 "aws_account_id": "20100000000" } }, "prod": { "prod-us-west-2":
 { "aws_region": "us-west-2", "aws_account_id": "30100000000" }, "prod-us-east-
 2": { "aws_region": "us-east-2", "aws_account_id": "30100000000" }, "prod-eu-
 west-1": { "aws_region": "eu-west-1", "aws_account_id": "30100000000" }, "prod-
 eu-central-1": { "aws_region": "eu-central-1", "aws_account_id": "30100000000"
 }, "prod-ap-southeast-2": { "aws_region": "ap-southeast-2", "aws_account_id":
 "30100000000" }, "prod-ap-southwest-1": { "aws_region": "ap-southwest-1",
@@ -202,16 +204,19 @@
 the more elaborate release system, but as is nearly always the case, the need
 to deploy will have deadlines that will be sooner than such an adoption.
 ```yaml version: 2.1 orbs: continuation: circleci/continuation@0.3.1 on-push-
 main: &on-push-main branches: only: /main/ tags: ignore: /.*/ on-tag-main: &on-
 tag-main branches: ignore: /.*/ tags: only: /.*/ commands: setup-commands:
 parameters: ... steps: ... static-code-test-commands: parameters: ... steps:
 ... before-deployment-commands: parameters: ... steps: ... after-deployment-
-commands: parameters: ... steps: ... workflows: version: 2 release-pipeline:
-jobs: - terraform/plan: name: nonprod-us-west-2 change plan context: <<
+commands: parameters: ... steps: ... jobs: my-pre-deploy-jobs: parameters: ...
+docker: - image: ... steps: - setup-commands: parameters: << parameters... >> -
+static-code-test-commands: parameters: << parameters... >> launch-dynamic-
+pipeline: parameters: ... workflows: version: 2 release-pipeline: jobs: -
+terraform/plan: name: nonprod-us-west-2 change plan context: <<
 pipeline.parameters.context >> workspace: nonprod-us-west-2 var-file: env_test/
 nonprod-us-west-2.tfvars.json before-terraform: - set-environment filters: *on-
 tag-main - terraform/plan: name: nonprod-us-east-2 change plan context: <<
 pipeline.parameters.context >> workspace: nonprod-us-east-2 var-file: env_test/
 nonprod-us-east-2.tfvars.json before-terraform: - set-environment filters: *on-
 tag-main - terraform/plan: name: nonprod-eu-west-1 change plan ... filters:
 *on-tag-main - terraform/plan: name: nonprod-eu-central-1 change plan ...
@@ -252,8 +257,43 @@
 terraform: - after-deployment-commands requires: - approve nonprod changes
 filters: *on-tag-main - terraform/apply: name: apply nonprod-us-east-2 change
 plan ... filters: *on-tag-main - terraform/apply: name: apply nonprod-eu-west-
 1 change plan ... filters: *on-tag-main - terraform/apply: name: apply nonprod-
 eu-central-1 change plan ... filters: *on-tag-main - terraform/apply: name:
 apply nonprod-ap-southeast-2 change plan ... filters: *on-tag-main - terraform/
 apply: name: apply nonprod-ap-southwest-1 change plan ... filters: *on-tag-main
-```
+``` #### 2. Setup example for a job to run nightly integration tests In this
+example we start by setting up the `environments/multi.json` and `environments/
+default.json` as from before. We also set up any relevant role-specific
+overrides, and the CircleCI config file (`.circleci/config.yml`) as from
+before. We then create a custom template file which will be specified with the
+`--template` flag. Let's use the example below: ```yaml - integration-tests:
+name: {{env_instance}} integration test context: << pipeline.parameters.context
+>> shell: << pipeline.parameters.shell-options >> executor-image: <<
+pipeline.parameters.executor-image >> instance_name: {{env_instance}}
+workspace: {{env_instance}} filters: {{filters}} ``` The resulting pipeline
+from using the above custom template would then look like the following:
+```yaml --- version: 2.1 orbs: continuation: circleci/continuation@0.3.1 on-
+push-main: &on-push-main branches: only: /main/ tags: ignore: /.*/ commands:
+setup-commands: parameters: ... steps: ... static-code-test-commands:
+parameters: ... steps: ... before-instance-specific-parallel-job-commands:
+parameters: ... steps: ... after-instance-specific-parallel-job-commands:
+parameters: ... steps: ... jobs: my-pre-deploy-jobs: parameters: ... docker: -
+image: ... steps: - setup-commands: parameters: << parameters... >> - static-
+code-test-commands: parameters: << parameters... >> launch-dynamic-pipeline:
+parameters: ... workflows: version: 2 release-pipeline: jobs: - integration-
+tests: name: nonprod-us-west-2 integration test context: <<
+pipeline.parameters.context >> shell: << pipeline.parameters.shell-options >>
+executor-image: << pipeline.parameters.executor-image >> instance_name:
+nonprod-us-west-2 workspace: nonprod-us-west-2 filters: *on-push-main -
+integration-tests: name: nonprod-us-east-2 integration test context: <<
+pipeline.parameters.context >> shell: << pipeline.parameters.shell-options >>
+executor-image: << pipeline.parameters.executor-image >> instance_name:
+nonprod-us-east-2 workspace: nonprod-us-east-2 filters: *on-push-main -
+integration-tests: name: prod-us-west-2 integration test context: <<
+pipeline.parameters.context >> shell: << pipeline.parameters.shell-options >>
+executor-image: << pipeline.parameters.executor-image >> instance_name: prod-
+us-west-2 workspace: prod-us-west-2 filters: *on-push-main - integration-tests:
+name: prod-us-east-2 integration test context: << pipeline.parameters.context
+>> shell: << pipeline.parameters.shell-options >> executor-image: <<
+pipeline.parameters.executor-image >> instance_name: prod-us-east-2 workspace:
+prod-us-east-2 filters: *on-push-main ```
```

### Comparing `circlecigen-0.0.7/circlecigen.egg-info/SOURCES.txt` & `circlecigen-0.0.8/circlecigen.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,35 +16,38 @@
 circlecigen.egg-info/PKG-INFO
 circlecigen.egg-info/SOURCES.txt
 circlecigen.egg-info/dependency_links.txt
 circlecigen.egg-info/entry_points.txt
 circlecigen.egg-info/requires.txt
 circlecigen.egg-info/top_level.txt
 env_test/config.yml
+env_test/custom.yml
 env_test/default.json
 env_test/dev.json
 env_test/generated_config.yml
 env_test/multi.json
 env_test/nonprod-us-east-2.tfvars.json
 env_test/nonprod-us-west-2.tfvars.json
 env_test/nonprod.json
 env_test/post-approve.yml
 env_test/pre-approve.yml
 env_test/prod-us-east-2.tfvars.json
 env_test/prod-us-west-2.tfvars.json
 env_test/prod.json
+env_test/template_generated_config.yml
 src/__init__.py
 src/_version.py
 src/circlecigen.py
 src/template.py
 src/tfvars.py
 src/utils.py
 test/generated_config.yml
 test/generated_config_setup.yml
 test/nonprod-us-east-2.tfvars.json
 test/nonprod-us-west-2.tfvars.json
 test/prod-us-east-2.tfvars.json
 test/prod-us-west-2.tfvars.json
+test/template_generated_config.yml
 test/test_circlecigen.py
 test/test_template.py
 test/test_tfvars.py
 test/test_utils.py
```

### Comparing `circlecigen-0.0.7/env_test/config.yml` & `circlecigen-0.0.8/env_test/config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.7/env_test/generated_config.yml` & `circlecigen-0.0.8/env_test/generated_config.yml`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,34 @@
             sudo tar -xvf teller_1.5.6_Linux_x86_64.tar.gz
             sudo mv teller /usr/local/bin/.
       - run:
           name: write cluster kubeconfig to secrets store
           command: bash scripts/write_cluster_credentials.sh << parameters.region >>
 
 
+jobs:
+
+  launch-dynamic-pipeline:
+    parameters:
+      workflow-name:
+        description: Custom name for the resulting workflow within the generated_config.yml
+        type: string
+      multi-config:
+        description: name of the multi-environment definition/configuration file to use
+        type: string
+        default: multi.json
+    executor: continuation/default
+    steps:
+      - checkout
+      - run:
+          name: generate continuation pipeline
+          command: circlecigen --workflow << parameters.workflow-name >>
+      - continuation/continue:
+          configuration_path: .circleci/generated_config.yml
+
 
 workflows:
   version: 2
 
   continuation-generated-workflow:
     jobs:
       - terraform/plan:
```

### Comparing `circlecigen-0.0.7/env_test/multi.json` & `circlecigen-0.0.8/env_test/multi.json`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.7/env_test/post-approve.yml` & `circlecigen-0.0.8/env_test/post-approve.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.7/pyproject.toml` & `circlecigen-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.7/setup.py` & `circlecigen-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.7/src/circlecigen.py` & `circlecigen-0.0.8/src/circlecigen.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,33 +12,38 @@
     callback=validate_filename_arg)
 @click.option("--envpath", default="environments",
     help="Environment config folder. Default is environments/",
     callback=validate_filepath_arg)
 @click.option("--multifile", default="multi.json",
     help="Multi-environment config file. Default is multi.json",
     callback=validate_filepath_arg)
+@click.option("--template", default=None,
+    help="""Custom CircleCI template file to use for generating jobs. This is optional.
+            If not provided, pre_approve.yml and post_approve.yml in the pipepath directory will be used""",
+    callback=validate_filepath_arg)
 @click.option("--defaultparams", default="default.json",
     help="Default parameters file. Default is default.tfvars.json",
     callback=validate_filepath_arg)
 @click.option("--tfvars", default=True,
     help="Generate tfvars.json files for all role/instances. Default is true")
 @click.option("--workflow", default="continuation-generated-workflow",
     help="Name for generated config. Default continuation-generated-workflow",
     callback=validate_filename_arg)
 @click.option("--pipepath", default=".circleci",
     help="Override default config.yml location for testing",
     callback=validate_filepath_arg)
 @click.argument('pipeline', nargs=1)
-def cli(pipeline, outfile, envpath, multifile, defaultparams, tfvars, workflow, pipepath):
+def cli(pipeline, outfile, envpath, multifile, defaultparams, tfvars, workflow, pipepath, template):
     """
 
     Inputs 
 
       .circleci/pre_approve.yml
       .circleci/post_approve.yml
+      .circleci/custom_template.yml (optional)
 
       environments/
 
         muilti.json
         default.json
 
         [role].json (optional)
@@ -55,21 +60,24 @@
 
     Opinionated generation of continuation pipelines.
     See https://github.com/ThoughtWorks-DPS/circlecigen
     for detailed usage instructions.
     """
     validate_filepath(envpath, "envpath")
     validate_filepath(pipepath, "pipepath")
+    validate_filepath(f"{pipepath}/{template}", "template")
 
     if tfvars:
         result = generate_environment_tfvar_files(pipeline, envpath,
                  read_json_file(envpath, multifile),
                  read_json_file(envpath, defaultparams))
         click.echo(f"{result} tfvars created in {envpath}/")
     else:
         click.echo("Not generating tfvars.json files")
-    generate_config(pipeline, 
+    generate_config(pipeline,
                     pipepath,
                     outfile,
                     envpath,
                     read_json_file(envpath, multifile),
-                    workflow)
+                    workflow,
+                    template
+                    )
```

### Comparing `circlecigen-0.0.7/src/template.py` & `circlecigen-0.0.8/src/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,29 +19,29 @@
 """
 
 PRIOR_APPROVAL="""
           requires:
             - approve {} changes
 """
 
-def generate_config(use_pipeline, pipepath, outfile, envpath, environs, workflow):
+def generate_config(use_pipeline, pipepath, outfile, envpath, environs, workflow, template):
     """create generated_config.yaml for continuation orb"""
 
     # use the specified filter to generate a pipeline only for the desired trigger
     pipeline = environs[use_pipeline]
 
     # copy everything but the jobs and workflows from config.yml into generated_config.yml
     # pipepath = where to find config.yml, default .circleci
     # outfile  = where to write generated_config.yml, default .circleci
     # workflow = what to name the generated workflow, default continuation-generated-workflow
     setup_generated_config_outfile(pipepath, outfile, workflow)
 
     # setup the jinja templates
     je = Environment(loader=FileSystemLoader(f"{pipepath}/"), autoescape=True)
-    pre, approve, post = get_templates(je, pipepath)
+    pre, approve, post, custom = get_templates(je, pipepath, template)
 
     # setup Dict for the approval job template 
     approve_vars = {}
     approve_vars["filter"] = pipeline["filter"]
 
     # all pre-approval jobs created accept for the first role must wait for
     # the prior role approval set this as blank to start then populate
@@ -52,25 +52,28 @@
     # open the outfile for appeand and start processing roles/instances
     with open(f"{pipepath}/{outfile}", 'a', encoding="utf-8") as f:
         for role in pipeline:
             # skip the filter definition
             if role == "filter":
                 continue
 
-            # when the approval template is generate, it must be populated with
-            # a list of all instances for which a pre-approval template is
-            # generated. That is returned by this job.
-            approvalrequiredjobs = generate_pre_approval_jobs(f, envpath, pre, pipeline, role, priorapprovalrequired)
-
-            # generate approval job for the current role, a human will trigger the post- phase
-            generate_approval_jobs(f, approve, approve_vars, approvalrequiredjobs, role)
-            generate_post_approval_jobs(f, envpath, post, pipeline, role)
+            if custom:
+                generate_custom_jobs(f, envpath, custom, pipeline, role)
+            else:
+                # when the approval template is generated, it must be populated with
+                # a list of all instances for which a pre-approval template will be
+                # generated. That is returned by this job.
+                approvalrequiredjobs = generate_pre_approval_jobs(f, envpath, pre, pipeline, role, priorapprovalrequired)
+
+                # generate approval job for the current role, a human will trigger the post- phase
+                generate_approval_jobs(f, approve, approve_vars, approvalrequiredjobs, role)
+                generate_post_approval_jobs(f, envpath, post, pipeline, role)
 
-            # record the current role, to provide 'requires:' list in any subsequent pre- jobs
-            priorapprovalrequired = role
+                # record the current role, to provide 'requires:' list in any subsequent pre- jobs
+                priorapprovalrequired = role
 
 def generate_pre_approval_jobs(f, envpath, pre, pipeline, role, priorapprovalrequired):
     # generate a pre-approval job for each instance in the role,
     # if a pre-approval.yml file exists
     if pre:
         approvalrequiredjobs = "requires:"
         for instance in pipeline[role]:
@@ -110,35 +113,51 @@
             instance_vars.update({
                 "filters": pipeline["filter"],
                 "role": role,
                 "envpath": envpath
             })
             f.write(post.render(instance_vars))
 
-def get_templates(je, pipepath):
+
+def generate_custom_jobs(f, envpath, custom, pipeline, role):
+    # generate a custom job for each instance in the role,
+    # if a custom template file (specified by the --template flag) exists
+    for instance in pipeline[role]:
+        instance_vars=read_json_file(envpath, f"{instance}.tfvars.json")
+        instance_vars.update({
+            "filters": pipeline["filter"],
+            "role": role,
+            "envpath": envpath
+        })
+        f.write(custom.render(instance_vars))
+
+
+def get_templates(je, pipepath, template=None):
     """setup the jinja templates"""
     pre = je.get_template("pre-approve.yml") if isfile(f"{pipepath}/pre-approve.yml") else 0
     post = je.get_template("post-approve.yml") if isfile(f"{pipepath}/post-approve.yml") else 0
+    custom = je.get_template(f"{template}") if isfile(f"{pipepath}/{template}") else 0
     approve = je.from_string(APPROVE_TEMPLATE)
-    return pre, approve, post
+    return pre, approve, post, custom
+
 
 def generate_config_lines(pipepath):
     """Read config.yml and yield lines that don't start with 'setup:' until it encounters a line starting with 'jobs:' or 'workflows:'"""
     config_file = f"{pipepath}/config.yml"
     with open(config_file, encoding="utf-8") as f:
         for line in _read_until_jobs_or_workflows(f):
             if not _line_starts_with_setup(line):
                 yield line
 
 
 def _read_until_jobs_or_workflows(f):
-    """Generator that reads lines from file object f until it encounters a line starting with 'jobs:' or 'workflows:'"""
+    """Generator that reads lines from file object f until it encounters a line starting with 'workflows:'"""
     for line in f:
         # initially, 
-        if line.startswith("jobs:") or line.startswith("workflows:"):
+        if line.startswith("workflows:"):
             break
         yield line
 
 def _line_starts_with_setup(line):
     """Return True if the given line starts with 'setup:', False otherwise"""
     return line.startswith("setup:")
```

### Comparing `circlecigen-0.0.7/src/tfvars.py` & `circlecigen-0.0.8/src/tfvars.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.7/src/utils.py` & `circlecigen-0.0.8/src/utils.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.7/test/generated_config.yml` & `circlecigen-0.0.8/test/generated_config.yml`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,34 @@
             sudo tar -xvf teller_1.5.6_Linux_x86_64.tar.gz
             sudo mv teller /usr/local/bin/.
       - run:
           name: write cluster kubeconfig to secrets store
           command: bash scripts/write_cluster_credentials.sh << parameters.region >>
 
 
+jobs:
+
+  launch-dynamic-pipeline:
+    parameters:
+      workflow-name:
+        description: Custom name for the resulting workflow within the generated_config.yml
+        type: string
+      multi-config:
+        description: name of the multi-environment definition/configuration file to use
+        type: string
+        default: multi.json
+    executor: continuation/default
+    steps:
+      - checkout
+      - run:
+          name: generate continuation pipeline
+          command: circlecigen --workflow << parameters.workflow-name >>
+      - continuation/continue:
+          configuration_path: .circleci/generated_config.yml
+
 
 workflows:
   version: 2
 
   continuation-generated-workflow:
     jobs:
       - terraform/plan:
```

### Comparing `circlecigen-0.0.7/test/generated_config_setup.yml` & `circlecigen-0.0.8/test/generated_config_setup.yml`

 * *Files 14% similar despite different names*

```diff
@@ -52,13 +52,33 @@
             sudo tar -xvf teller_1.5.6_Linux_x86_64.tar.gz
             sudo mv teller /usr/local/bin/.
       - run:
           name: write cluster kubeconfig to secrets store
           command: bash scripts/write_cluster_credentials.sh << parameters.region >>
 
 
+jobs:
+
+  launch-dynamic-pipeline:
+    parameters:
+      workflow-name:
+        description: Custom name for the resulting workflow within the generated_config.yml
+        type: string
+      multi-config:
+        description: name of the multi-environment definition/configuration file to use
+        type: string
+        default: multi.json
+    executor: continuation/default
+    steps:
+      - checkout
+      - run:
+          name: generate continuation pipeline
+          command: circlecigen --workflow << parameters.workflow-name >>
+      - continuation/continue:
+          configuration_path: .circleci/generated_config.yml
+
 
 workflows:
   version: 2
 
   continuation-generated-workflow:
     jobs:
```

### Comparing `circlecigen-0.0.7/test/test_circlecigen.py` & `circlecigen-0.0.8/test/test_circlecigen.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,21 +39,27 @@
 
 def test_circlecigen_with_invalid_pipepath_name():
   runner = CliRunner()
   result = runner.invoke(cli, ['sandbox', '--pipepath', 'invalid:pathname'])
   assert result.exit_code == 2
   assert "Invalid value for '--pipepath'" in result.output
 
+def test_circlecigen_with_invalid_template_name():
+  runner = CliRunner()
+  result = runner.invoke(cli, ['sandbox', '--template', 'invalid:template'])
+  assert result.exit_code == 2
+  assert "Invalid value for '--template'" in result.output
+
 def test_circlecigen_help():
   runner = CliRunner()
   result = runner.invoke(cli, ["--help"])
   assert "Usage:" in result.output
 
 def test_circlecigen_with_missing_pipeline_argument():
   runner = CliRunner()
   result = runner.invoke(cli)
   assert "Missing argument" in result.output
 
 def test_circlecigen_with_test_env_values():
   runner = CliRunner()
-  result = runner.invoke(cli, ["release", "--envpath", "env_test", "--pipepath", "env_test"])
+  result = runner.invoke(cli, ["release", "--envpath", "env_test", "--pipepath", "env_test", "--template", "custom.yml"])
   assert "4 tfvars created in env_test/" in result.output
```

### Comparing `circlecigen-0.0.7/test/test_template.py` & `circlecigen-0.0.8/test/test_template.py`

 * *Files 20% similar despite different names*

```diff
@@ -50,27 +50,58 @@
                        mock_outfile),
                        os.path.join("test", "generated_config_setup.yml"))
 
 def test_get_templates():
     envpath = "env_test"
     je = Environment(loader=FileSystemLoader(f"{envpath}/"))
 
-    pre, approve, post = get_templates(je, envpath)
+    pre, approve, post, custom = get_templates(je, envpath)
     
     assert isinstance(pre, Template)
     assert isinstance(post, Template)
     assert isinstance(approve, Template)
 
+
+def test_get_custom_template():
+    envpath = "env_test"
+    custom_template = "custom.yml"
+    je = Environment(loader=FileSystemLoader(f"{envpath}/"))
+
+    pre, approve, post, custom = get_templates(je, envpath, custom_template)
+
+    assert isinstance(pre, Template)
+    assert isinstance(post, Template)
+    assert isinstance(approve, Template)
+    assert isinstance(custom, Template)
+
+
 # this is as ugly as the tfvars file output tests
 def test_generate_config():
     mock_pipeline = "release"
     mock_pipepath = "env_test"
     mock_envpath = "env_test"
     mock_outfile = "generated_config.yml"
     mock_workflow = "continuation-generated-workflow"
+    mock_template = None
 
-    generate_config(mock_pipeline, mock_pipepath, mock_outfile, mock_envpath, mock_multi, mock_workflow)
+    generate_config(mock_pipeline, mock_pipepath, mock_outfile, mock_envpath, mock_multi, mock_workflow, mock_template)
     assert os.path.isfile(os.path.join(mock_pipepath, mock_outfile))
     assert filecmp.cmp(os.path.join(mock_pipepath,
                        mock_outfile),
                        os.path.join("test",
                        mock_outfile))
+
+
+def test_generate_config_with_custom_template():
+    mock_pipeline = "release"
+    mock_pipepath = "env_test"
+    mock_envpath = "env_test"
+    mock_outfile = "template_generated_config.yml"
+    mock_workflow = "continuation-generated-workflow"
+    mock_template = "custom.yml"
+
+    generate_config(mock_pipeline, mock_pipepath, mock_outfile, mock_envpath, mock_multi, mock_workflow, mock_template)
+    assert os.path.isfile(os.path.join(mock_pipepath, mock_outfile))
+    assert filecmp.cmp(os.path.join(mock_pipepath,
+                                    mock_outfile),
+                       os.path.join("test",
+                                    mock_outfile))
```

### Comparing `circlecigen-0.0.7/test/test_tfvars.py` & `circlecigen-0.0.8/test/test_tfvars.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.7/test/test_utils.py` & `circlecigen-0.0.8/test/test_utils.py`

 * *Files identical despite different names*

