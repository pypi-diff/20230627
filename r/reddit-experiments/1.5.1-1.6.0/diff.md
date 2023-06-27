# Comparing `tmp/reddit_experiments-1.5.1.tar.gz` & `tmp/reddit_experiments-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit_experiments-1.5.1.tar", last modified: Thu Jun 15 08:10:43 2023, max compression
+gzip compressed data, was "reddit_experiments-1.6.0.tar", last modified: Tue Jun 27 21:43:19 2023, max compression
```

## Comparing `reddit_experiments-1.5.1.tar` & `reddit_experiments-1.6.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:43.178412 reddit_experiments-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:43.154412 reddit_experiments-1.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:43.162412 reddit_experiments-1.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/.github/workflows/python-package.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-15 08:10:43.182412 reddit_experiments-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:43.162412 reddit_experiments-1.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:43.162412 reddit_experiments-1.5.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    53651 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/docs/images/ddg-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/docs/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:43.162412 reddit_experiments-1.5.1/docs/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/docs/legacy/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:43.162412 reddit_experiments-1.5.1/reddit_decider/
--rw-r--r--   0 runner    (1001) docker     (123)    45652 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/reddit_decider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/reddit_decider/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:43.162412 reddit_experiments-1.5.1/reddit_experiments/
--rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/reddit_experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:43.162412 reddit_experiments-1.5.1/reddit_experiments/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/reddit_experiments/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/reddit_experiments/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/reddit_experiments/providers/feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/reddit_experiments/providers/forced_variant.py
--rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/reddit_experiments/providers/r2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/reddit_experiments/providers/simple_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/reddit_experiments/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:43.162412 reddit_experiments-1.5.1/reddit_experiments/targeting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/reddit_experiments/targeting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/reddit_experiments/targeting/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/reddit_experiments/targeting/tree_targeting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:43.162412 reddit_experiments-1.5.1/reddit_experiments/variant_sets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/reddit_experiments/variant_sets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/reddit_experiments/variant_sets/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/reddit_experiments/variant_sets/multi_variant_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/reddit_experiments/variant_sets/range_variant_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/reddit_experiments/variant_sets/rollout_variant_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/reddit_experiments/variant_sets/single_variant_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:43.162412 reddit_experiments-1.5.1/reddit_experiments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-15 08:10:42.000000 reddit_experiments-1.5.1/reddit_experiments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-15 08:10:43.000000 reddit_experiments-1.5.1/reddit_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:10:42.000000 reddit_experiments-1.5.1/reddit_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 08:10:42.000000 reddit_experiments-1.5.1/reddit_experiments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 08:10:42.000000 reddit_experiments-1.5.1/reddit_experiments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:10:42.000000 reddit_experiments-1.5.1/reddit_experiments.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/requirements-transitive.txt
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-15 08:10:43.182412 reddit_experiments-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:43.162412 reddit_experiments-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    79965 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/tests/decider_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    38015 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/tests/experiment_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:43.166412 reddit_experiments-1.5.1/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/tests/providers/feature_flag_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/tests/providers/forced_variant_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    29866 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/tests/providers/r2_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/tests/providers/simple_experiment_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:43.166412 reddit_experiments-1.5.1/tests/providers/variant_sets/
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/tests/providers/variant_sets/multi_variant_set_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/tests/providers/variant_sets/range_variant_set_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/tests/providers/variant_sets/rollout_variant_set_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/tests/providers/variant_sets/single_variant_set_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:43.166412 reddit_experiments-1.5.1/tests/range_variant_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:43.178412 reddit_experiments-1.5.1/tests/range_variant_tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   154451 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/tests/range_variant_tests/data/original_zk_config.json
--rw-r--r--   0 runner    (1001) docker     (123) 14213529 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/tests/range_variant_tests/data/output.json
--rw-r--r--   0 runner    (1001) docker     (123)   163729 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/tests/range_variant_tests/data/range_variant_zk_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/tests/range_variant_tests/range_variant_parity_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:10:43.178412 reddit_experiments-1.5.1/tests/targeting/
--rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-06-15 08:10:28.000000 reddit_experiments-1.5.1/tests/targeting/tree_targeting_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.843564 reddit_experiments-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.811563 reddit_experiments-1.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.815563 reddit_experiments-1.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/.github/workflows/python-package.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-27 21:43:19.843564 reddit_experiments-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.819563 reddit_experiments-1.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.819563 reddit_experiments-1.6.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    53651 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/docs/images/ddg-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/docs/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.819563 reddit_experiments-1.6.0/docs/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/docs/legacy/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.819563 reddit_experiments-1.6.0/reddit_decider/
+-rw-r--r--   0 runner    (1001) docker     (123)    46119 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_decider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_decider/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.819563 reddit_experiments-1.6.0/reddit_experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.819563 reddit_experiments-1.6.0/reddit_experiments/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/providers/feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/providers/forced_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/providers/r2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/providers/simple_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.819563 reddit_experiments-1.6.0/reddit_experiments/targeting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/targeting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/targeting/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/targeting/tree_targeting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.823563 reddit_experiments-1.6.0/reddit_experiments/variant_sets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/variant_sets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/variant_sets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/variant_sets/multi_variant_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/variant_sets/range_variant_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/variant_sets/rollout_variant_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/reddit_experiments/variant_sets/single_variant_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.819563 reddit_experiments-1.6.0/reddit_experiments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-27 21:43:19.000000 reddit_experiments-1.6.0/reddit_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-27 21:43:19.000000 reddit_experiments-1.6.0/reddit_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:43:19.000000 reddit_experiments-1.6.0/reddit_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-27 21:43:19.000000 reddit_experiments-1.6.0/reddit_experiments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-27 21:43:19.000000 reddit_experiments-1.6.0/reddit_experiments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:43:19.000000 reddit_experiments-1.6.0/reddit_experiments.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/requirements-transitive.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-27 21:43:19.843564 reddit_experiments-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.823563 reddit_experiments-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    78782 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/decider_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38015 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/experiment_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.823563 reddit_experiments-1.6.0/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/providers/feature_flag_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/providers/forced_variant_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29866 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/providers/r2_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/providers/simple_experiment_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.823563 reddit_experiments-1.6.0/tests/providers/variant_sets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/providers/variant_sets/multi_variant_set_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/providers/variant_sets/range_variant_set_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/providers/variant_sets/rollout_variant_set_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/providers/variant_sets/single_variant_set_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.823563 reddit_experiments-1.6.0/tests/range_variant_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.843564 reddit_experiments-1.6.0/tests/range_variant_tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   154451 2023-06-27 21:43:03.000000 reddit_experiments-1.6.0/tests/range_variant_tests/data/original_zk_config.json
+-rw-r--r--   0 runner    (1001) docker     (123) 14213529 2023-06-27 21:43:04.000000 reddit_experiments-1.6.0/tests/range_variant_tests/data/output.json
+-rw-r--r--   0 runner    (1001) docker     (123)   163729 2023-06-27 21:43:04.000000 reddit_experiments-1.6.0/tests/range_variant_tests/data/range_variant_zk_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-27 21:43:04.000000 reddit_experiments-1.6.0/tests/range_variant_tests/range_variant_parity_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:19.843564 reddit_experiments-1.6.0/tests/targeting/
+-rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-06-27 21:43:04.000000 reddit_experiments-1.6.0/tests/targeting/tree_targeting_tests.py
```

### Comparing `reddit_experiments-1.5.1/.github/workflows/python-package.yaml` & `reddit_experiments-1.6.0/.github/workflows/python-package.yaml`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/.github/workflows/python-publish.yaml` & `reddit_experiments-1.6.0/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/.readthedocs.yaml` & `reddit_experiments-1.6.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/LICENSE` & `reddit_experiments-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/Makefile` & `reddit_experiments-1.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/PKG-INFO` & `reddit_experiments-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit_experiments
-Version: 1.5.1
+Version: 1.6.0
 Summary: reddit's python experiments framework
 Home-page: https://github.com/reddit/experiments.py
 Author: reddit
 License: BSD
 Project-URL: Documentation, https://reddit-experiments.readthedocs.io/
 Description: # experiments.py
```

### Comparing `reddit_experiments-1.5.1/README.md` & `reddit_experiments-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/docs/conf.py` & `reddit_experiments-1.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/docs/images/ddg-logo.png` & `reddit_experiments-1.6.0/docs/images/ddg-logo.png`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/docs/images/favicon.png` & `reddit_experiments-1.6.0/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/docs/index.rst` & `reddit_experiments-1.6.0/docs/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
  .. _reddit_decider:
 
 ``reddit_decider``
-===============================
+==================
 
 .. automodule:: reddit_decider
 
 
 Prerequisite packages
 ---------------------
 .. code-block:: python
@@ -99,14 +99,32 @@
 
 Make sure :code:`EdgeContext` is accessible on :code:`request` object like so:
 
 .. code-block:: python
 
     request.edge_context
 
+If you **don't have access** to :code:`edge_context` in your service/request, you can access the SDK’s internal decider instance for a lower level API,
+allowing you to pass in targeting context fields as a :code:`dict` param,
+e.g. "user_is_employee", "country_code", or other targeting fields (instead of them being auto-derived from :code:`edge_context`).
+
+See full API in `readme <https://github.snooguts.net/reddit/decider/tree/master/decider-py#class-decider>`_ (reddit internal).
+
+The internal decider instance can be accessed from the SDK's top-level decider instance via:
+
+.. code-block:: python
+
+    internal_decider = request.decider.internal_decider()  # requires `reddit-experiments >= 1.4.1`
+    internal_decider.choose("experiment_name", {
+            "user_id": "t2_abc",
+            "user_is_employee": True,
+            "other_info": { "arbitrary_field": "some_val" }
+        }
+    )
+
 
 [Optional] Define request field extractor function (`example <https://github.snooguts.net/reddit/reddit-service-graphql/blob/master/graphql-py/graphql_api/models/experiment.py#L67-L92>`_)
 
 .. code-block:: python
 
     # Baseplate calls `make_object_for_context()` and creates a `DeciderContext`
     # which fetches the following fields from EdgeContext automatically:
@@ -128,34 +146,35 @@
     def my_field_extractor(request):
         # an example of customized baseplate request field extractor:
         return {"foo": request.headers.get("Foo"), "bar": "something"}
 
 
 Basic Usage
 -----------
-Use the attached :py:class:`~reddit_decider.Decider` object in request to call
+Use the attached :py:class:`~reddit_decider.Decider` instance in request to call
 :code:`decider.get_variant()` (automatically sends an expose event)::
 
     def my_method(request):
         if request.decider.get_variant("foo") == "bar":
             ...
 
 or optionally, if manual exposure is necessary, use::
 
     def my_method(request):
         variant = request.decider.get_variant_without_expose(experiment_name='experiment_name')
         ...
         request.decider.expose(experiment_name='experiment_name', variant_name=variant)
 
-and this is an example of using a dynamic configuration::
+This is an example of using a dynamic configuration::
 
     def my_method(request):
         if request.decider.get_bool("foo") == True:
             ...
 
+
 Decider API
 -----------
 
 .. autoclass:: Decider
    :members:
 
 Configuration Class
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `reddit_experiments-1.5.1/docs/legacy/index.rst` & `reddit_experiments-1.6.0/docs/legacy/index.rst`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/reddit_decider/__init__.py` & `reddit_experiments-1.6.0/reddit_decider/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from baseplate import RequestContext
 from baseplate import Span
 from baseplate.clients import ContextFactory
 from baseplate.lib import config
 from baseplate.lib.events import DebugLogger
 from baseplate.lib.events import EventLogger
 from baseplate.lib.file_watcher import FileWatcher
-from baseplate.lib.file_watcher import T
 from baseplate.lib.file_watcher import WatchedFileNotAvailableError
 from reddit_edgecontext import ValidatedAuthenticationToken
 from rust_decider import Decider as RustDecider
 from rust_decider import DeciderException
 from rust_decider import Decision
 from rust_decider import FeatureNotFoundException
 from rust_decider import ValueTypeMismatchException
@@ -58,57 +57,67 @@
     start_ts: int
     stop_ts: int
     owner: str
     emit_event: Optional[bool] = None
 
 
 class DeciderContext:
-    """DeciderContext() is used to contain all fields necessary for
+    """:code:`DeciderContext` is used to contain all fields necessary for
     bucketing, targeting, and overrides.
-    :code:`DeciderContext()` is populated in :code:`make_object_for_context()`.
-    """
+    :code:`DeciderContext` is populated in :code:`make_object_for_context()`
 
-    T = TypeVar("T")
+    :param user_id: user's t2 id
+    :param device_id: device installation uuid
+    :param country_code: 2-letter country codes
+    :param locale: ISO 639-1 primary language subtag and an optional ISO 3166-1 alpha-2 region subtag
+    :param user_is_employee:
+    :param logged_in: is user logged in
+    :param oauth_client_id: OAuth Client ID
+    :param origin_service: Service where request originated
+    :param cookie_created_timestamp: When the authentication cookie was created
+    :param loid_created_timestamp: Epoch milliseconds when the current LoID cookie was created
+    :param extracted_fields: Optional dict of additional fields, e.g. app_name & build_number
+    """
 
     def __init__(
         self,
         user_id: Optional[str] = None,
+        device_id: Optional[str] = None,
         country_code: Optional[str] = None,
         locale: Optional[str] = None,
         user_is_employee: Optional[bool] = None,
         logged_in: Optional[bool] = None,
-        device_id: Optional[str] = None,
         oauth_client_id: Optional[str] = None,
         origin_service: Optional[str] = None,
         cookie_created_timestamp: Optional[float] = None,
         loid_created_timestamp: Optional[float] = None,
         extracted_fields: Optional[dict] = None,
     ):
         self._user_id = user_id
+        self._device_id = device_id
         self._country_code = country_code
         self._locale = locale
         self._user_is_employee = user_is_employee
         self._logged_in = logged_in
-        self._device_id = device_id
         self._oauth_client_id = oauth_client_id
         self._origin_service = origin_service
         self._cookie_created_timestamp = cookie_created_timestamp
         self._loid_created_timestamp = loid_created_timestamp
         self._extracted_fields = extracted_fields
 
     def to_dict(self) -> Dict:
         ef = deepcopy(self._extracted_fields or {})
 
         return {
             "user_id": self._user_id,
+            "device_id": self._device_id,
             "country_code": self._country_code,
             "locale": self._locale,
             "user_is_employee": self._user_is_employee,
             "logged_in": self._logged_in,
-            "device_id": self._device_id,
             "oauth_client_id": self._oauth_client_id,
             "origin_service": self._origin_service,
             "cookie_created_timestamp": self._cookie_created_timestamp,
             "loid_created_timestamp": self._loid_created_timestamp,
             "other_fields": ef,
             **ef,
         }
@@ -171,14 +180,16 @@
     """Access to experiments with automatic refresh when changed.
 
     This decider client allows access to the experiments cached on disk by
     the experiment configuration fetcher daemon.
     It will automatically reload the cache when changed.
     """
 
+    T = TypeVar("T")
+
     def __init__(
         self,
         decider_context: DeciderContext,
         internal: Optional[RustDecider],
         server_span: Span,
         context_name: str,
         event_logger: Optional[EventLogger] = None,
@@ -379,16 +390,15 @@
 
         if self._internal is None:
             logger.error("RustDecider is None--did not initialize.")
             return
 
         try:
             feature = self._internal.get_feature(experiment_name)
-        except FeatureNotFoundException as exc:
-            logger.debug(str(exc))
+        except FeatureNotFoundException:
             return
         except DeciderException as exc:
             logger.info(str(exc))
             return
 
         # drop exposure for feature rollouts
         if not feature.emit_event:
@@ -790,16 +800,15 @@
     ) -> Optional[Decision]:
         if self._internal is None:
             logger.error("RustDecider is None--did not initialize.")
             return None
 
         try:
             return self._internal.choose(experiment_name, ctx)
-        except FeatureNotFoundException as exc:
-            logger.debug(str(exc))
+        except FeatureNotFoundException:
             return None
         except DeciderException as exc:
             logger.info(str(exc))
             return None
 
     def _get_all_decisions(
         self, ctx: Dict[str, Any], bucketing_field_filter: Optional[str] = None
@@ -825,16 +834,15 @@
             logger.error("rs_decider is None--did not initialize.")
             return default
 
         ctx = self._decider_context.to_dict()
 
         try:
             value = get_fn(feature_name=feature_name, context=ctx)
-        except FeatureNotFoundException as exc:
-            logger.debug(str(exc))
+        except FeatureNotFoundException:
             return default
         except ValueTypeMismatchException as exc:
             logger.info(str(exc))
             return default
         except DeciderException as exc:
             logger.info(str(exc))
             return default
@@ -862,16 +870,15 @@
         """
         if self._internal is None:
             logger.error("RustDecider is None--did not initialize.")
             return None
 
         try:
             feature = self._internal.get_feature(experiment_name)
-        except FeatureNotFoundException as exc:
-            logger.debug(str(exc))
+        except FeatureNotFoundException:
             return None
         except DeciderException as exc:
             logger.info(str(exc))
             return None
 
         return ExperimentConfig(
             id=feature.id,
```

### Comparing `reddit_experiments-1.5.1/reddit_experiments/__init__.py` & `reddit_experiments-1.6.0/reddit_experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/reddit_experiments/providers/__init__.py` & `reddit_experiments-1.6.0/reddit_experiments/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/reddit_experiments/providers/base.py` & `reddit_experiments-1.6.0/reddit_experiments/providers/base.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/reddit_experiments/providers/feature_flag.py` & `reddit_experiments-1.6.0/reddit_experiments/providers/feature_flag.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/reddit_experiments/providers/forced_variant.py` & `reddit_experiments-1.6.0/reddit_experiments/providers/forced_variant.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/reddit_experiments/providers/r2.py` & `reddit_experiments-1.6.0/reddit_experiments/providers/r2.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/reddit_experiments/providers/simple_experiment.py` & `reddit_experiments-1.6.0/reddit_experiments/providers/simple_experiment.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/reddit_experiments/targeting/tree_targeting.py` & `reddit_experiments-1.6.0/reddit_experiments/targeting/tree_targeting.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/reddit_experiments/variant_sets/base.py` & `reddit_experiments-1.6.0/reddit_experiments/variant_sets/base.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/reddit_experiments/variant_sets/multi_variant_set.py` & `reddit_experiments-1.6.0/reddit_experiments/variant_sets/multi_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/reddit_experiments/variant_sets/range_variant_set.py` & `reddit_experiments-1.6.0/reddit_experiments/variant_sets/range_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/reddit_experiments/variant_sets/rollout_variant_set.py` & `reddit_experiments-1.6.0/reddit_experiments/variant_sets/rollout_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/reddit_experiments/variant_sets/single_variant_set.py` & `reddit_experiments-1.6.0/reddit_experiments/variant_sets/single_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/reddit_experiments.egg-info/PKG-INFO` & `reddit_experiments-1.6.0/reddit_experiments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-experiments
-Version: 1.5.1
+Version: 1.6.0
 Summary: reddit's python experiments framework
 Home-page: https://github.com/reddit/experiments.py
 Author: reddit
 License: BSD
 Project-URL: Documentation, https://reddit-experiments.readthedocs.io/
 Description: # experiments.py
```

### Comparing `reddit_experiments-1.5.1/reddit_experiments.egg-info/SOURCES.txt` & `reddit_experiments-1.6.0/reddit_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/requirements-transitive.txt` & `reddit_experiments-1.6.0/requirements-transitive.txt`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/setup.cfg` & `reddit_experiments-1.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/setup.py` & `reddit_experiments-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/tests/decider_tests.py` & `reddit_experiments-1.6.0/tests/decider_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import contextlib
 import json
 import logging
 import tempfile
 import unittest
-import warnings
 
 from unittest import mock
 
 from baseplate import RequestContext
 from baseplate import ServerSpan
 from baseplate.lib.events import DebugLogger
-from baseplate.lib.file_watcher import FileWatcher
 from reddit_edgecontext import ValidatedAuthenticationToken
 
 from reddit_decider import Decider
 from reddit_decider import decider_client_from_config
 from reddit_decider import DeciderContext
 from reddit_decider import DeciderContextFactory
 from reddit_decider import EventType
@@ -554,32 +552,14 @@
             # get_variant()
             variant = decider.get_variant("test")
             self.assertEqual(variant, None)
 
             variant = decider.get_variant("exp_1")
             self.assertEqual(variant, "variant_4")
 
-    def test_none_returned_on_get_variant_call_with_experiment_not_found(self):
-        with create_temp_config_file({}) as f:
-            decider = setup_decider(
-                f, self.minimal_decider_context, self.mock_span, self.event_logger
-            )
-
-            self.assertEqual(self.event_logger.log.call_count, 0)
-            with self.assertLogs(logger, logging.DEBUG) as captured:
-                variant = decider.get_variant("anything")
-
-                assert any(
-                    'Feature "anything" not found.' in x.getMessage() for x in captured.records
-                )
-            self.assertEqual(variant, None)
-
-            # no exposures should be triggered
-            self.assertEqual(self.event_logger.log.call_count, 0)
-
     def test_get_variant_without_expose(self):
         with create_temp_config_file(self.exp_base_config) as f:
             decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant = decider.get_variant_without_expose(experiment_name="exp_1")
             self.assertEqual(variant, "variant_4")
@@ -604,32 +584,14 @@
             event_fields = self.event_logger.log.call_args[1]
 
             # `variant == None` for holdout but event will fire with `variant == "holdout"` for analysis
             self.assert_exposure_event_fields(
                 experiment_name="hg", variant="holdout", event_fields=event_fields
             )
 
-    def test_none_returned_on_get_variant_without_expose_call_with_experiment_not_found(self):
-        with create_temp_config_file({}) as f:
-            decider = setup_decider(
-                f, self.minimal_decider_context, self.mock_span, self.event_logger
-            )
-
-            self.assertEqual(self.event_logger.log.call_count, 0)
-            with self.assertLogs(logger, logging.DEBUG) as captured:
-                variant = decider.get_variant_without_expose("anything")
-
-                assert any(
-                    'Feature "anything" not found.' in x.getMessage() for x in captured.records
-                )
-            self.assertEqual(variant, None)
-
-            # no exposures should be triggered
-            self.assertEqual(self.event_logger.log.call_count, 0)
-
     def test_get_variant_for_identifier_user_id(self):
         identifier = USER_ID
         bucket_val = "user_id"
         self.exp_base_config["exp_1"]["experiment"].update({"bucket_val": bucket_val})
 
         with create_temp_config_file(self.exp_base_config) as f:
             decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
@@ -733,14 +695,25 @@
                 bucket_val=bucket_val,
                 identifier=identifier,
             )
 
             # `identifier` passed to correct event field of experiment's `bucket_val` config
             self.assertEqual(event_fields["subreddit_id"], identifier)
 
+            # exposure assertions
+            self.assertEqual(self.event_logger.log.call_count, 1)
+            event_fields = self.event_logger.log.call_args[1]
+            self.assert_exposure_event_fields(
+                experiment_name="exp_1",
+                variant=variant,
+                event_fields=event_fields,
+                bucket_val=bucket_val,
+                identifier=identifier,
+            )
+
     def test_get_variant_for_identifier_ad_account_id(self):
         identifier = AD_ACCOUNT_ID
         bucket_val = "ad_account_id"
         self.exp_base_config["exp_1"]["experiment"].update({"bucket_val": bucket_val})
 
         with create_temp_config_file(self.exp_base_config) as f:
             decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
@@ -1405,15 +1378,15 @@
         with create_temp_config_file(self.exp_base_config) as f:
             decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
 
             with self.assertLogs() as captured:
                 variant_arr = decider.get_all_variants_for_identifier_without_expose(
-                    identifier=identifier, identifier_type="blah"
+                    identifier=identifier, identifier_type=identifier_type
                 )
 
                 self.assertEqual(len(variant_arr), 0)
 
                 assert any(
                     "\"blah\" is not one of supported \"identifier_type\": ['user_id', 'device_id', 'canonical_url', 'subreddit_id', 'ad_account_id', 'business_id']."
                     in x.getMessage()
@@ -1493,15 +1466,15 @@
 
         with create_temp_config_file(self.exp_base_config) as f:
             decider = setup_decider(f, self.dc, self.mock_span, self.event_logger)
 
             self.assertEqual(self.event_logger.log.call_count, 0)
             variant = decider.get_variant_without_expose("exp_1")
 
-            assert variant == None
+            assert variant is None
 
             # exposure from control_1 of "hg"
             self.assertEqual(self.event_logger.log.call_count, 1)
             event_fields = self.event_logger.log.call_args[1]
 
             # `variant == None` for child but event will fire with `variant == "control_1"` for analysis
             self.assert_exposure_event_fields(
```

### Comparing `reddit_experiments-1.5.1/tests/experiment_tests.py` & `reddit_experiments-1.6.0/tests/experiment_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/tests/providers/feature_flag_tests.py` & `reddit_experiments-1.6.0/tests/providers/feature_flag_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/tests/providers/forced_variant_tests.py` & `reddit_experiments-1.6.0/tests/providers/forced_variant_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/tests/providers/r2_tests.py` & `reddit_experiments-1.6.0/tests/providers/r2_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/tests/providers/simple_experiment_tests.py` & `reddit_experiments-1.6.0/tests/providers/simple_experiment_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/tests/providers/variant_sets/multi_variant_set_tests.py` & `reddit_experiments-1.6.0/tests/providers/variant_sets/multi_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/tests/providers/variant_sets/range_variant_set_tests.py` & `reddit_experiments-1.6.0/tests/providers/variant_sets/range_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/tests/providers/variant_sets/rollout_variant_set_tests.py` & `reddit_experiments-1.6.0/tests/providers/variant_sets/rollout_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/tests/providers/variant_sets/single_variant_set_tests.py` & `reddit_experiments-1.6.0/tests/providers/variant_sets/single_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/tests/range_variant_tests/data/original_zk_config.json` & `reddit_experiments-1.6.0/tests/range_variant_tests/data/original_zk_config.json`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/tests/range_variant_tests/data/output.json` & `reddit_experiments-1.6.0/tests/range_variant_tests/data/output.json`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/tests/range_variant_tests/data/range_variant_zk_config.json` & `reddit_experiments-1.6.0/tests/range_variant_tests/data/range_variant_zk_config.json`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/tests/range_variant_tests/range_variant_parity_tests.py` & `reddit_experiments-1.6.0/tests/range_variant_tests/range_variant_parity_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.5.1/tests/targeting/tree_targeting_tests.py` & `reddit_experiments-1.6.0/tests/targeting/tree_targeting_tests.py`

 * *Files identical despite different names*

