# Comparing `tmp/pydflow-1.7.5.tar.gz` & `tmp/pydflow-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydflow-1.7.5.tar", last modified: Mon Jun 19 08:48:12 2023, max compression
+gzip compressed data, was "pydflow-1.7.6.tar", last modified: Tue Jun 27 03:22:11 2023, max compression
```

## Comparing `pydflow-1.7.5.tar` & `pydflow-1.7.6.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:48:12.911081 pydflow-1.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-06-19 08:48:03.000000 pydflow-1.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 08:48:03.000000 pydflow-1.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-06-19 08:48:12.911081 pydflow-1.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32758 2023-06-19 08:48:03.000000 pydflow-1.7.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 08:48:03.000000 pydflow-1.7.5/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 08:48:12.911081 pydflow-1.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-19 08:48:03.000000 pydflow-1.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:48:12.899080 pydflow-1.7.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:48:12.903080 pydflow-1.7.5/src/dflow/
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/argo_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:48:12.903080 pydflow-1.7.5/src/dflow/client/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17690 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/client/v1alpha1_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/client/v1alpha1_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/client/v1alpha1_retry_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/client/v1alpha1_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/client/v1alpha1_value_from.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/context_syntax.py
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    51335 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    23997 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/op_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:48:12.907081 pydflow-1.7.5/src/dflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/plugins/bohrium.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/plugins/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    23061 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/plugins/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/plugins/launching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/plugins/lebesgue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/plugins/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/plugins/oss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/plugins/ray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:48:12.907081 pydflow-1.7.5/src/dflow/python/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/python/op.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/python/opio.py
--rw-r--r--   0 runner    (1001) docker     (123)    31751 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/python/python_op_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/python/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)   102981 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/util_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    25735 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    45198 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:48:12.907081 pydflow-1.7.5/src/pydflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-06-19 08:48:12.000000 pydflow-1.7.5/src/pydflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-19 08:48:12.000000 pydflow-1.7.5/src/pydflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:48:12.000000 pydflow-1.7.5/src/pydflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 08:48:12.000000 pydflow-1.7.5/src/pydflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-19 08:48:12.000000 pydflow-1.7.5/src/pydflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-19 08:48:12.000000 pydflow-1.7.5/src/pydflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:48:12.907081 pydflow-1.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_big_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_conditional_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_group_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_makevasp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_recurse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_reuse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_subpath_slices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:22:11.742232 pydflow-1.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-06-27 03:21:58.000000 pydflow-1.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 03:21:58.000000 pydflow-1.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-06-27 03:22:11.742232 pydflow-1.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32758 2023-06-27 03:21:58.000000 pydflow-1.7.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 03:21:58.000000 pydflow-1.7.6/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 03:22:11.742232 pydflow-1.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-27 03:21:58.000000 pydflow-1.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:22:11.734232 pydflow-1.7.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:22:11.738232 pydflow-1.7.6/src/dflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/argo_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:22:11.738232 pydflow-1.7.6/src/dflow/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17690 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/client/v1alpha1_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/client/v1alpha1_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/client/v1alpha1_retry_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/client/v1alpha1_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/client/v1alpha1_value_from.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/context_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51335 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23997 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/op_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:22:11.738232 pydflow-1.7.6/src/dflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/plugins/bohrium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/plugins/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23061 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/plugins/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/plugins/launching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/plugins/lebesgue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/plugins/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/plugins/oss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/plugins/ray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:22:11.738232 pydflow-1.7.6/src/dflow/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/python/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/python/opio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31751 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/python/python_op_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/python/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103446 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/util_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25735 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45198 2023-06-27 03:21:58.000000 pydflow-1.7.6/src/dflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:22:11.738232 pydflow-1.7.6/src/pydflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-06-27 03:22:11.000000 pydflow-1.7.6/src/pydflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-27 03:22:11.000000 pydflow-1.7.6/src/pydflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 03:22:11.000000 pydflow-1.7.6/src/pydflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-27 03:22:11.000000 pydflow-1.7.6/src/pydflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-27 03:22:11.000000 pydflow-1.7.6/src/pydflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-27 03:22:11.000000 pydflow-1.7.6/src/pydflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:22:11.742232 pydflow-1.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-27 03:21:58.000000 pydflow-1.7.6/tests/test_big_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-27 03:21:58.000000 pydflow-1.7.6/tests/test_conditional_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-27 03:21:58.000000 pydflow-1.7.6/tests/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-27 03:21:58.000000 pydflow-1.7.6/tests/test_group_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-06-27 03:21:58.000000 pydflow-1.7.6/tests/test_makevasp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-27 03:21:58.000000 pydflow-1.7.6/tests/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-27 03:21:58.000000 pydflow-1.7.6/tests/test_recurse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-27 03:21:58.000000 pydflow-1.7.6/tests/test_reuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-27 03:21:58.000000 pydflow-1.7.6/tests/test_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-27 03:21:58.000000 pydflow-1.7.6/tests/test_subpath_slices.py
```

### Comparing `pydflow-1.7.5/LICENSE` & `pydflow-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/PKG-INFO` & `pydflow-1.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydflow
-Version: 1.7.5
+Version: 1.7.6
 Summary: Dflow is a Python framework for constructing scientific computing workflows employing Argo Workflows as the workflow engine.
 Home-page: https://github.com/deepmodeling/dflow
 Author: Xinzijian Liu
 Author-email: liuxzj@dp.tech
 License: LGPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pydflow-1.7.5/README.md` & `pydflow-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/setup.py` & `pydflow-1.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/__init__.py` & `pydflow-1.7.6/src/dflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/argo_objects.py` & `pydflow-1.7.6/src/dflow/argo_objects.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/client/v1alpha1_artifact.py` & `pydflow-1.7.6/src/dflow/client/v1alpha1_artifact.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/client/v1alpha1_parameter.py` & `pydflow-1.7.6/src/dflow/client/v1alpha1_parameter.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/client/v1alpha1_retry_strategy.py` & `pydflow-1.7.6/src/dflow/client/v1alpha1_retry_strategy.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/client/v1alpha1_sequence.py` & `pydflow-1.7.6/src/dflow/client/v1alpha1_sequence.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/client/v1alpha1_value_from.py` & `pydflow-1.7.6/src/dflow/client/v1alpha1_value_from.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/common.py` & `pydflow-1.7.6/src/dflow/common.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/config.py` & `pydflow-1.7.6/src/dflow/config.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/context_syntax.py` & `pydflow-1.7.6/src/dflow/context_syntax.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/dag.py` & `pydflow-1.7.6/src/dflow/dag.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/executor.py` & `pydflow-1.7.6/src/dflow/executor.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/io.py` & `pydflow-1.7.6/src/dflow/io.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/main.py` & `pydflow-1.7.6/src/dflow/main.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/op_template.py` & `pydflow-1.7.6/src/dflow/op_template.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/plugins/bohrium.py` & `pydflow-1.7.6/src/dflow/plugins/bohrium.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/plugins/datasets.py` & `pydflow-1.7.6/src/dflow/plugins/datasets.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/plugins/dispatcher.py` & `pydflow-1.7.6/src/dflow/plugins/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/plugins/launching.py` & `pydflow-1.7.6/src/dflow/plugins/launching.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/plugins/lebesgue.py` & `pydflow-1.7.6/src/dflow/plugins/lebesgue.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/plugins/metadata.py` & `pydflow-1.7.6/src/dflow/plugins/metadata.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/plugins/oss.py` & `pydflow-1.7.6/src/dflow/plugins/oss.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/plugins/ray.py` & `pydflow-1.7.6/src/dflow/plugins/ray.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/python/op.py` & `pydflow-1.7.6/src/dflow/python/op.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/python/opio.py` & `pydflow-1.7.6/src/dflow/python/opio.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/python/python_op_template.py` & `pydflow-1.7.6/src/dflow/python/python_op_template.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/python/utils.py` & `pydflow-1.7.6/src/dflow/python/utils.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/resource.py` & `pydflow-1.7.6/src/dflow/resource.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/slurm.py` & `pydflow-1.7.6/src/dflow/slurm.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/step.py` & `pydflow-1.7.6/src/dflow/step.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import logging
 import os
 import re
+import shlex
 import shutil
 import sys
 from copy import deepcopy
 from typing import Any, Dict, List, Optional, Union
 
 import jsonpickle
 
@@ -175,38 +176,50 @@
     """
     if config["mode"] == "debug":
         return Expression("len(%s)" % to_expr(param))
     return ArgoLen(param)
 
 
 class ArgoEnumerate(ArgoVar):
-    def __init__(self, param: ArgoVar):
+    def __init__(self, **kwargs):
+        param = list(kwargs.values())[0]
+        if isinstance(param, ArgoVar):
+            length = "len(sprig.fromJson(%s))" % param.expr
+        else:
+            length = len(param)
+        values = ""
+        for k, v in kwargs.items():
+            values += ", '%s': jsonpath(%s, '$')[#]" % (
+                k, v.expr if isinstance(v, ArgoVar)
+                else shlex.quote(json.dumps(v)))
         super().__init__(
-            "toJson(map(sprig.untilStep(0, len(sprig.fromJson(%s)), 1),"
-            " { {'order': #, 'value': jsonpath(%s, '$')[#]} }))" % (
-                param.expr, param.expr))
+            "toJson(map(sprig.untilStep(0, %s, 1), "
+            "{ {'order': #%s} }))" % (length, values))
 
 
 def argo_enumerate(
-        param,
+        *args, **kwargs,
 ) -> ArgoVar:
     """
     Return the enumeration of a list which is an Argo parameter
 
     Args:
         param: the Argo parameter which is a list
     """
+    if len(args) == 1:
+        kwargs["value"] = args[0]
+    elif len(args) > 1:
+        for i, arg in enumerate(args):
+            kwargs["value" + str(i)] = arg
     if config["mode"] == "debug":
-        return Expression("[{'order': i, 'value': v} for i, v in "
-                          "enumerate(%s)]" % to_expr(param))
-    if isinstance(param, ArgoVar):
-        return ArgoEnumerate(param)
-    else:
-        return json.dumps([{'order': i, 'value': v} for i, v in
-                           enumerate(param)])
+        values = "".join([", '%s': %s[i]" % (k, to_expr(v))
+                          for k, v in kwargs.items()])
+        return Expression("[{'order': i%s} for i in range(len(%s))]" % (
+            values, to_expr(list(kwargs.values())[0])))
+    return ArgoEnumerate(**kwargs)
 
 
 class ArgoSum:
     def __init__(self, param):
         self.param = param
         self.expr = "sum(%s)" % param
```

### Comparing `pydflow-1.7.5/src/dflow/steps.py` & `pydflow-1.7.6/src/dflow/steps.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/task.py` & `pydflow-1.7.6/src/dflow/task.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/util_ops.py` & `pydflow-1.7.6/src/dflow/util_ops.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/utils.py` & `pydflow-1.7.6/src/dflow/utils.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/dflow/workflow.py` & `pydflow-1.7.6/src/dflow/workflow.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/src/pydflow.egg-info/PKG-INFO` & `pydflow-1.7.6/src/pydflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydflow
-Version: 1.7.5
+Version: 1.7.6
 Summary: Dflow is a Python framework for constructing scientific computing workflows employing Argo Workflows as the workflow engine.
 Home-page: https://github.com/deepmodeling/dflow
 Author: Xinzijian Liu
 Author-email: liuxzj@dp.tech
 License: LGPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pydflow-1.7.5/src/pydflow.egg-info/SOURCES.txt` & `pydflow-1.7.6/src/pydflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/tests/test_big_parameter.py` & `pydflow-1.7.6/tests/test_big_parameter.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/tests/test_conditional_outputs.py` & `pydflow-1.7.6/tests/test_conditional_outputs.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/tests/test_dag.py` & `pydflow-1.7.6/tests/test_dag.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/tests/test_group_size.py` & `pydflow-1.7.6/tests/test_group_size.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/tests/test_makevasp.py` & `pydflow-1.7.6/tests/test_makevasp.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/tests/test_python.py` & `pydflow-1.7.6/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/tests/test_recurse.py` & `pydflow-1.7.6/tests/test_recurse.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/tests/test_reuse.py` & `pydflow-1.7.6/tests/test_reuse.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/tests/test_slices.py` & `pydflow-1.7.6/tests/test_slices.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.5/tests/test_subpath_slices.py` & `pydflow-1.7.6/tests/test_subpath_slices.py`

 * *Files identical despite different names*

