# Comparing `tmp/hsml-3.2.0rc0.tar.gz` & `tmp/hsml-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsml-3.2.0rc0.tar", last modified: Wed Apr 12 12:47:02 2023, max compression
+gzip compressed data, was "hsml-3.2.0rc1.tar", last modified: Wed Apr 26 08:37:45 2023, max compression
```

## Comparing `hsml-3.2.0rc0.tar` & `hsml-3.2.0rc1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.143006 hsml-3.2.0rc0/
--rw-r--r--   0     1006     1006       40 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/MANIFEST.in
--rw-r--r--   0     1006     1006     5178 2023-04-12 12:47:02.143006 hsml-3.2.0rc0/PKG-INFO
--rw-r--r--   0     1006     1006     3399 2023-04-12 12:47:01.000000 hsml-3.2.0rc0/README.md
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.135007 hsml-3.2.0rc0/hsml/
--rw-r--r--   0     1006     1006     1016 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/__init__.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.135007 hsml-3.2.0rc0/hsml/client/
--rw-r--r--   0     1006     1006     3684 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/__init__.py
--rw-r--r--   0     1006     1006     1876 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/auth.py
--rw-r--r--   0     1006     1006     3946 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/base.py
--rw-r--r--   0     1006     1006     2456 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/exceptions.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.135007 hsml-3.2.0rc0/hsml/client/hopsworks/
--rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/hopsworks/__init__.py
--rw-r--r--   0     1006     1006     3985 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/hopsworks/base.py
--rw-r--r--   0     1006     1006     2846 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/hopsworks/external.py
--rw-r--r--   0     1006     1006     7088 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/hopsworks/internal.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.135007 hsml-3.2.0rc0/hsml/client/istio/
--rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/istio/__init__.py
--rw-r--r--   0     1006     1006     3455 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/istio/base.py
--rw-r--r--   0     1006     1006     1663 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/istio/external.py
--rw-r--r--   0     1006     1006     6650 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/client/istio/internal.py
--rw-r--r--   0     1006     1006    10216 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/connection.py
--rw-r--r--   0     1006     1006     2594 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/constants.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.139006 hsml-3.2.0rc0/hsml/core/
--rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/core/__init__.py
--rw-r--r--   0     1006     1006    15187 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/core/dataset_api.py
--rw-r--r--   0     1006     1006     7327 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/core/model_api.py
--rw-r--r--   0     1006     1006     2745 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/core/model_registry_api.py
--rw-r--r--   0     1006     1006     5810 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/core/model_serving_api.py
--rw-r--r--   0     1006     1006     1188 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/core/native_hdfs_api.py
--rw-r--r--   0     1006     1006    11463 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/core/serving_api.py
--rw-r--r--   0     1006     1006     1656 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/decorators.py
--rw-r--r--   0     1006     1006     2899 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/deployable_component.py
--rw-r--r--   0     1006     1006     2936 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/deployable_component_logs.py
--rw-r--r--   0     1006     1006    13979 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/deployment.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.139006 hsml-3.2.0rc0/hsml/engine/
--rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/engine/__init__.py
--rw-r--r--   0     1006     1006     1536 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/engine/hopsworks_engine.py
--rw-r--r--   0     1006     1006      934 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/engine/local_engine.py
--rw-r--r--   0     1006     1006    14766 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/engine/model_engine.py
--rw-r--r--   0     1006     1006    22555 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/engine/serving_engine.py
--rw-r--r--   0     1006     1006     4387 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/inference_batcher.py
--rw-r--r--   0     1006     1006     4668 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/inference_endpoint.py
--rw-r--r--   0     1006     1006     4034 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/inference_logger.py
--rw-r--r--   0     1006     1006     4700 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/kafka_topic.py
--rw-r--r--   0     1006     1006    14300 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/model.py
--rw-r--r--   0     1006     1006     6574 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/model_registry.py
--rw-r--r--   0     1006     1006     1861 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/model_schema.py
--rw-r--r--   0     1006     1006    12706 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/model_serving.py
--rw-r--r--   0     1006     1006    15504 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/predictor.py
--rw-r--r--   0     1006     1006     5164 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/predictor_state.py
--rw-r--r--   0     1006     1006     2618 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/predictor_state_condition.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.139006 hsml-3.2.0rc0/hsml/python/
--rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/python/__init__.py
--rw-r--r--   0     1006     1006     2223 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/python/model.py
--rw-r--r--   0     1006     1006     1151 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/python/predictor.py
--rw-r--r--   0     1006     1006     2515 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/python/signature.py
--rw-r--r--   0     1006     1006    11756 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/resources.py
--rw-r--r--   0     1006     1006     2540 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/schema.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.139006 hsml-3.2.0rc0/hsml/sklearn/
--rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/sklearn/__init__.py
--rw-r--r--   0     1006     1006     2218 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/sklearn/model.py
--rw-r--r--   0     1006     1006      977 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/sklearn/predictor.py
--rw-r--r--   0     1006     1006     2510 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/sklearn/signature.py
--rw-r--r--   0     1006     1006     1937 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/tag.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.139006 hsml-3.2.0rc0/hsml/tensorflow/
--rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/tensorflow/__init__.py
--rw-r--r--   0     1006     1006     2223 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/tensorflow/model.py
--rw-r--r--   0     1006     1006     1169 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/tensorflow/predictor.py
--rw-r--r--   0     1006     1006     2515 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/tensorflow/signature.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.139006 hsml-3.2.0rc0/hsml/torch/
--rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/torch/__init__.py
--rw-r--r--   0     1006     1006     2213 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/torch/model.py
--rw-r--r--   0     1006     1006     1142 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/torch/predictor.py
--rw-r--r--   0     1006     1006     2505 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/torch/signature.py
--rw-r--r--   0     1006     1006     2968 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/transformer.py
--rw-r--r--   0     1006     1006     9842 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/util.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.139006 hsml-3.2.0rc0/hsml/utils/
--rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/utils/__init__.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.139006 hsml-3.2.0rc0/hsml/utils/schema/
--rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/utils/schema/__init__.py
--rw-r--r--   0     1006     1006      936 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/utils/schema/column.py
--rw-r--r--   0     1006     1006     3570 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/utils/schema/columnar_schema.py
--rw-r--r--   0     1006     1006      976 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/utils/schema/tensor.py
--rw-r--r--   0     1006     1006     2396 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/utils/schema/tensor_schema.py
--rw-r--r--   0     1006     1006      631 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/hsml/version.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.135007 hsml-3.2.0rc0/hsml.egg-info/
--rw-r--r--   0     1006     1006     5178 2023-04-12 12:47:01.000000 hsml-3.2.0rc0/hsml.egg-info/PKG-INFO
--rw-r--r--   0     1006     1006     2009 2023-04-12 12:47:02.000000 hsml-3.2.0rc0/hsml.egg-info/SOURCES.txt
--rw-r--r--   0     1006     1006        1 2023-04-12 12:47:01.000000 hsml-3.2.0rc0/hsml.egg-info/dependency_links.txt
--rw-r--r--   0     1006     1006      306 2023-04-12 12:47:01.000000 hsml-3.2.0rc0/hsml.egg-info/requires.txt
--rw-r--r--   0     1006     1006       11 2023-04-12 12:47:01.000000 hsml-3.2.0rc0/hsml.egg-info/top_level.txt
--rw-r--r--   0     1006     1006       38 2023-04-12 12:47:02.143006 hsml-3.2.0rc0/setup.cfg
--rw-r--r--   0     1006     1006     2478 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/setup.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.143006 hsml-3.2.0rc0/tests/
--rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/tests/__init__.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.143006 hsml-3.2.0rc0/tests/hsml/
--rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/tests/hsml/__init__.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:47:02.143006 hsml-3.2.0rc0/tests/hsml/core/
--rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc0/tests/hsml/core/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-04-26 08:37:45.556511 hsml-3.2.0rc1/
+-rw-r--r--   0     1006     1006       40 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/MANIFEST.in
+-rw-r--r--   0     1006     1006     5178 2023-04-26 08:37:45.556511 hsml-3.2.0rc1/PKG-INFO
+-rw-r--r--   0     1006     1006     3399 2023-04-26 08:37:44.000000 hsml-3.2.0rc1/README.md
+drwxr-xr-x   0     1006     1006        0 2023-04-26 08:37:45.544511 hsml-3.2.0rc1/hsml/
+-rw-r--r--   0     1006     1006     1016 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-04-26 08:37:45.548511 hsml-3.2.0rc1/hsml/client/
+-rw-r--r--   0     1006     1006     3684 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/client/__init__.py
+-rw-r--r--   0     1006     1006     1876 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/client/auth.py
+-rw-r--r--   0     1006     1006     3946 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/client/base.py
+-rw-r--r--   0     1006     1006     2456 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/client/exceptions.py
+drwxr-xr-x   0     1006     1006        0 2023-04-26 08:37:45.548511 hsml-3.2.0rc1/hsml/client/hopsworks/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/client/hopsworks/__init__.py
+-rw-r--r--   0     1006     1006     3985 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/client/hopsworks/base.py
+-rw-r--r--   0     1006     1006     2846 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/client/hopsworks/external.py
+-rw-r--r--   0     1006     1006     7088 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/client/hopsworks/internal.py
+drwxr-xr-x   0     1006     1006        0 2023-04-26 08:37:45.548511 hsml-3.2.0rc1/hsml/client/istio/
+-rw-r--r--   0     1006     1006      605 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/client/istio/__init__.py
+-rw-r--r--   0     1006     1006     3455 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/client/istio/base.py
+-rw-r--r--   0     1006     1006     1663 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/client/istio/external.py
+-rw-r--r--   0     1006     1006     6650 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/client/istio/internal.py
+-rw-r--r--   0     1006     1006    10216 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/connection.py
+-rw-r--r--   0     1006     1006     2627 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/constants.py
+drwxr-xr-x   0     1006     1006        0 2023-04-26 08:37:45.552511 hsml-3.2.0rc1/hsml/core/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/core/__init__.py
+-rw-r--r--   0     1006     1006    15187 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/core/dataset_api.py
+-rw-r--r--   0     1006     1006     7327 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/core/model_api.py
+-rw-r--r--   0     1006     1006     2745 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/core/model_registry_api.py
+-rw-r--r--   0     1006     1006     5810 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/core/model_serving_api.py
+-rw-r--r--   0     1006     1006     1188 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/core/native_hdfs_api.py
+-rw-r--r--   0     1006     1006    11463 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/core/serving_api.py
+-rw-r--r--   0     1006     1006     1656 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/decorators.py
+-rw-r--r--   0     1006     1006     2899 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/deployable_component.py
+-rw-r--r--   0     1006     1006     2936 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/deployable_component_logs.py
+-rw-r--r--   0     1006     1006    14408 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/deployment.py
+drwxr-xr-x   0     1006     1006        0 2023-04-26 08:37:45.552511 hsml-3.2.0rc1/hsml/engine/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/engine/__init__.py
+-rw-r--r--   0     1006     1006     1536 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/engine/hopsworks_engine.py
+-rw-r--r--   0     1006     1006      934 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/engine/local_engine.py
+-rw-r--r--   0     1006     1006    14766 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/engine/model_engine.py
+-rw-r--r--   0     1006     1006    23120 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/engine/serving_engine.py
+-rw-r--r--   0     1006     1006     4387 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/inference_batcher.py
+-rw-r--r--   0     1006     1006     4668 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/inference_endpoint.py
+-rw-r--r--   0     1006     1006     4034 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/inference_logger.py
+-rw-r--r--   0     1006     1006     4700 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/kafka_topic.py
+-rw-r--r--   0     1006     1006    14300 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/model.py
+-rw-r--r--   0     1006     1006     6574 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/model_registry.py
+-rw-r--r--   0     1006     1006     1861 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/model_schema.py
+-rw-r--r--   0     1006     1006    12706 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/model_serving.py
+-rw-r--r--   0     1006     1006    15504 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/predictor.py
+-rw-r--r--   0     1006     1006     5164 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/predictor_state.py
+-rw-r--r--   0     1006     1006     2618 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/predictor_state_condition.py
+drwxr-xr-x   0     1006     1006        0 2023-04-26 08:37:45.552511 hsml-3.2.0rc1/hsml/python/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/python/__init__.py
+-rw-r--r--   0     1006     1006     2223 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/python/model.py
+-rw-r--r--   0     1006     1006     1151 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/python/predictor.py
+-rw-r--r--   0     1006     1006     2515 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/python/signature.py
+-rw-r--r--   0     1006     1006    11756 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/resources.py
+-rw-r--r--   0     1006     1006     2540 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/schema.py
+drwxr-xr-x   0     1006     1006        0 2023-04-26 08:37:45.552511 hsml-3.2.0rc1/hsml/sklearn/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/sklearn/__init__.py
+-rw-r--r--   0     1006     1006     2218 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/sklearn/model.py
+-rw-r--r--   0     1006     1006      977 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/sklearn/predictor.py
+-rw-r--r--   0     1006     1006     2510 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/sklearn/signature.py
+-rw-r--r--   0     1006     1006     1937 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/tag.py
+drwxr-xr-x   0     1006     1006        0 2023-04-26 08:37:45.552511 hsml-3.2.0rc1/hsml/tensorflow/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/tensorflow/__init__.py
+-rw-r--r--   0     1006     1006     2223 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/tensorflow/model.py
+-rw-r--r--   0     1006     1006     1169 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/tensorflow/predictor.py
+-rw-r--r--   0     1006     1006     2515 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/tensorflow/signature.py
+drwxr-xr-x   0     1006     1006        0 2023-04-26 08:37:45.556511 hsml-3.2.0rc1/hsml/torch/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/torch/__init__.py
+-rw-r--r--   0     1006     1006     2213 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/torch/model.py
+-rw-r--r--   0     1006     1006     1142 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/torch/predictor.py
+-rw-r--r--   0     1006     1006     2505 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/torch/signature.py
+-rw-r--r--   0     1006     1006     2968 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/transformer.py
+-rw-r--r--   0     1006     1006     9842 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/util.py
+drwxr-xr-x   0     1006     1006        0 2023-04-26 08:37:45.556511 hsml-3.2.0rc1/hsml/utils/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/utils/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-04-26 08:37:45.556511 hsml-3.2.0rc1/hsml/utils/schema/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/utils/schema/__init__.py
+-rw-r--r--   0     1006     1006      936 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/utils/schema/column.py
+-rw-r--r--   0     1006     1006     3570 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/utils/schema/columnar_schema.py
+-rw-r--r--   0     1006     1006      976 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/utils/schema/tensor.py
+-rw-r--r--   0     1006     1006     2396 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/hsml/utils/schema/tensor_schema.py
+-rw-r--r--   0     1006     1006      631 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/hsml/version.py
+drwxr-xr-x   0     1006     1006        0 2023-04-26 08:37:45.548511 hsml-3.2.0rc1/hsml.egg-info/
+-rw-r--r--   0     1006     1006     5178 2023-04-26 08:37:45.000000 hsml-3.2.0rc1/hsml.egg-info/PKG-INFO
+-rw-r--r--   0     1006     1006     2009 2023-04-26 08:37:45.000000 hsml-3.2.0rc1/hsml.egg-info/SOURCES.txt
+-rw-r--r--   0     1006     1006        1 2023-04-26 08:37:45.000000 hsml-3.2.0rc1/hsml.egg-info/dependency_links.txt
+-rw-r--r--   0     1006     1006      306 2023-04-26 08:37:45.000000 hsml-3.2.0rc1/hsml.egg-info/requires.txt
+-rw-r--r--   0     1006     1006       11 2023-04-26 08:37:45.000000 hsml-3.2.0rc1/hsml.egg-info/top_level.txt
+-rw-r--r--   0     1006     1006       38 2023-04-26 08:37:45.556511 hsml-3.2.0rc1/setup.cfg
+-rw-r--r--   0     1006     1006     2478 2023-04-26 08:37:40.000000 hsml-3.2.0rc1/setup.py
+drwxr-xr-x   0     1006     1006        0 2023-04-26 08:37:45.556511 hsml-3.2.0rc1/tests/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/tests/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-04-26 08:37:45.556511 hsml-3.2.0rc1/tests/hsml/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/tests/hsml/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-04-26 08:37:45.556511 hsml-3.2.0rc1/tests/hsml/core/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:46:57.000000 hsml-3.2.0rc1/tests/hsml/core/__init__.py
```

### Comparing `hsml-3.2.0rc0/PKG-INFO` & `hsml-3.2.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsml
-Version: 3.2.0rc0
+Version: 3.2.0rc1
 Summary: HSML: An environment independent client to interact with the Hopsworks Model Registry
 Home-page: https://github.com/logicalclocks/machine-learning-api
 Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/machine-learning-api/releases/tag/3.2.0rc0
+Download-URL: https://github.com/logicalclocks/machine-learning-api/releases/tag/3.2.0rc1
 Description: # Hopsworks Model Management
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: hsml Version: 3.2.0rc0 Summary: HSML: An
+Metadata-Version: 2.1 Name: hsml Version: 3.2.0rc1 Summary: HSML: An
 environment independent client to interact with the Hopsworks Model Registry
 Home-page: https://github.com/logicalclocks/machine-learning-api Author:
 Logical Clocks AB Author-email: robin@logicalclocks.com License: Apache License
 2.0 Download-URL: https://github.com/logicalclocks/machine-learning-api/
-releases/tag/3.2.0rc0 Description: # Hopsworks Model Management
+releases/tag/3.2.0rc1 Description: # Hopsworks Model Management
 [Hopsworks_Community] [Hopsworks_Model_Management_Documentation] [PyPiStatus]
            [Scala/Java_Artifacts] [Downloads] [CodeStyle] [License]
 HSML is the library to interact with the Hopsworks Model Registry and Model
 Serving. The library makes it easy to export, manage and deploy models. The
 library automatically configures itself based on the environment it is run.
 However, to connect from an external Python environment additional connection
 information, such as host and port, is required. For more information about the
```

### Comparing `hsml-3.2.0rc0/README.md` & `hsml-3.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/__init__.py` & `hsml-3.2.0rc1/hsml/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/client/__init__.py` & `hsml-3.2.0rc1/hsml/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/client/auth.py` & `hsml-3.2.0rc1/hsml/client/auth.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/client/base.py` & `hsml-3.2.0rc1/hsml/client/base.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/client/exceptions.py` & `hsml-3.2.0rc1/hsml/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/client/hopsworks/__init__.py` & `hsml-3.2.0rc1/hsml/client/hopsworks/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/client/hopsworks/base.py` & `hsml-3.2.0rc1/hsml/client/hopsworks/base.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/client/hopsworks/external.py` & `hsml-3.2.0rc1/hsml/client/hopsworks/external.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/client/hopsworks/internal.py` & `hsml-3.2.0rc1/hsml/client/hopsworks/internal.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/client/istio/__init__.py` & `hsml-3.2.0rc1/hsml/client/istio/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/client/istio/base.py` & `hsml-3.2.0rc1/hsml/client/istio/base.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/client/istio/external.py` & `hsml-3.2.0rc1/hsml/client/istio/external.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/client/istio/internal.py` & `hsml-3.2.0rc1/hsml/client/istio/internal.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/connection.py` & `hsml-3.2.0rc1/hsml/connection.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/constants.py` & `hsml-3.2.0rc1/hsml/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     # serving tool
     SERVING_TOOL_DEFAULT = "DEFAULT"
     SERVING_TOOL_KSERVE = "KSERVE"
 
 
 class PREDICTOR_STATE:
     # status
+    STATUS_CREATING = "Creating"
     STATUS_CREATED = "Created"
     STATUS_STARTING = "Starting"
     STATUS_FAILED = "Failed"
     STATUS_RUNNING = "Running"
     STATUS_IDLE = "Idle"
     STATUS_UPDATING = "Updating"
     STATUS_STOPPING = "Stopping"
```

### Comparing `hsml-3.2.0rc0/hsml/core/__init__.py` & `hsml-3.2.0rc1/hsml/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/core/dataset_api.py` & `hsml-3.2.0rc1/hsml/core/dataset_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/core/model_api.py` & `hsml-3.2.0rc1/hsml/core/model_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/core/model_registry_api.py` & `hsml-3.2.0rc1/hsml/core/model_registry_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/core/model_serving_api.py` & `hsml-3.2.0rc1/hsml/core/model_serving_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/core/native_hdfs_api.py` & `hsml-3.2.0rc1/hsml/core/native_hdfs_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/core/serving_api.py` & `hsml-3.2.0rc1/hsml/core/serving_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/decorators.py` & `hsml-3.2.0rc1/hsml/decorators.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/deployable_component.py` & `hsml-3.2.0rc1/hsml/deployable_component.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/deployable_component_logs.py` & `hsml-3.2.0rc1/hsml/deployable_component_logs.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/deployment.py` & `hsml-3.2.0rc1/hsml/deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,26 @@
 
         # Returns
             `PredictorState`. The state of the deployment.
         """
 
         return self._serving_engine.get_state(self)
 
+    def is_created(self) -> bool:
+        """Check whether the deployment is created.
+
+        # Returns
+            `bool`. Whether the deployment is created or not.
+        """
+
+        return (
+            self._serving_engine.get_state(self).status
+            != PREDICTOR_STATE.STATUS_CREATING
+        )
+
     def is_running(self, or_idle=True, or_updating=True) -> bool:
         """Check whether the deployment is ready to handle inference requests
 
         # Arguments
             or_idle: Whether the idle state is considered as running (default is True)
             or_updating: Whether the updating state is considered as running (default is True)
 
@@ -128,23 +140,27 @@
             or (or_updating and status == PREDICTOR_STATE.STATUS_UPDATING)
         )
 
     def is_stopped(self, or_created=True) -> bool:
         """Check whether the deployment is stopped
 
         # Arguments
-            or_created: Whether the created state is considered as stopped (default is True)
+            or_created: Whether the creating and created state is considered as stopped (default is True)
 
         # Returns
             `bool`. Whether the deployment is stopped or not.
         """
 
         status = self._serving_engine.get_state(self).status
         return status == PREDICTOR_STATE.STATUS_STOPPED or (
-            or_created and status == PREDICTOR_STATE.STATUS_CREATED
+            or_created
+            and (
+                status == PREDICTOR_STATE.STATUS_CREATING
+                or status == PREDICTOR_STATE.STATUS_CREATED
+            )
         )
 
     def predict(self, data: dict = None, inputs: list = None):
         """Send inference requests to the deployment.
            One of data or inputs parameters must be set. If both are set, inputs will be ignored.
 
         !!! example
```

### Comparing `hsml-3.2.0rc0/hsml/engine/__init__.py` & `hsml-3.2.0rc1/hsml/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/engine/hopsworks_engine.py` & `hsml-3.2.0rc1/hsml/engine/hopsworks_engine.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/engine/local_engine.py` & `hsml-3.2.0rc1/hsml/engine/local_engine.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/engine/model_engine.py` & `hsml-3.2.0rc1/hsml/engine/model_engine.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/engine/serving_engine.py` & `hsml-3.2.0rc1/hsml/engine/serving_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,23 @@
                 )
                 pbar.update(progress)
                 if desc is not None:
                     pbar.set_description(desc)
 
             try:
                 update_progress(state, num_instances=0)
+
+                if state.status == PREDICTOR_STATE.STATUS_CREATING:
+                    state = self._poll_deployment_status(  # wait for preparation
+                        deployment_instance,
+                        PREDICTOR_STATE.STATUS_CREATED,
+                        await_status,
+                        update_progress,
+                    )
+
                 self._serving_api.post(
                     deployment_instance, DEPLOYMENT.ACTION_START
                 )  # start deployment
 
                 state = self._poll_deployment_status(  # wait for status
                     deployment_instance,
                     PREDICTOR_STATE.STATUS_RUNNING,
@@ -245,15 +254,16 @@
                 raise ModelServingException(
                     "Deployment is stopping, please wait until it completely stops"
                 )
 
         # desired status: stopped
         if desired_status == PREDICTOR_STATE.STATUS_STOPPED:
             if (
-                state.status == PREDICTOR_STATE.STATUS_CREATED
+                state.status == PREDICTOR_STATE.STATUS_CREATING
+                or state.status == PREDICTOR_STATE.STATUS_CREATED
                 or state.status == PREDICTOR_STATE.STATUS_STOPPED
             ):
                 print("Deployment is already stopped")
                 return (True, state)
             if state.status == PREDICTOR_STATE.STATUS_STOPPING:
                 print("Deployment is already stopping")
                 return (True, state)
@@ -334,14 +344,16 @@
         return (
             deployment_instance.requested_instances
             if deployment_instance.requested_instances >= min_start_instances
             else min_start_instances
         )
 
     def _get_available_instances(self, state):
+        if state.status == PREDICTOR_STATE.STATUS_CREATING:
+            return 0
         num_instances = state.available_predictor_instances
         if state.available_transformer_instances is not None:
             num_instances += state.available_transformer_instances
         return num_instances
 
     def _get_stopped_instances(self, available_instances, requested_instances):
         num_instances = requested_instances - available_instances
@@ -446,15 +458,16 @@
             )
         if state.status == PREDICTOR_STATE.STATUS_STOPPING:
             # if stopping, it cannot be updated yet
             raise ModelServingException(
                 "Deployment is stopping, please wait until it is stopped before applying changes"
             )
         if (
-            state.status == PREDICTOR_STATE.STATUS_CREATED
+            state.status == PREDICTOR_STATE.STATUS_CREATING
+            or state.status == PREDICTOR_STATE.STATUS_CREATED
             or state.status == PREDICTOR_STATE.STATUS_STOPPED
         ):
             # if stopped, it's fine
             self._serving_api.put(deployment_instance)
             print("Deployment updated, explore it at " + deployment_instance.get_url())
             return
```

### Comparing `hsml-3.2.0rc0/hsml/inference_batcher.py` & `hsml-3.2.0rc1/hsml/inference_batcher.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/inference_endpoint.py` & `hsml-3.2.0rc1/hsml/inference_endpoint.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/inference_logger.py` & `hsml-3.2.0rc1/hsml/inference_logger.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/kafka_topic.py` & `hsml-3.2.0rc1/hsml/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/model.py` & `hsml-3.2.0rc1/hsml/model.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/model_registry.py` & `hsml-3.2.0rc1/hsml/model_registry.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/model_schema.py` & `hsml-3.2.0rc1/hsml/model_schema.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/model_serving.py` & `hsml-3.2.0rc1/hsml/model_serving.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/predictor.py` & `hsml-3.2.0rc1/hsml/predictor.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/predictor_state.py` & `hsml-3.2.0rc1/hsml/predictor_state.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/predictor_state_condition.py` & `hsml-3.2.0rc1/hsml/predictor_state_condition.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/python/__init__.py` & `hsml-3.2.0rc1/hsml/python/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/python/model.py` & `hsml-3.2.0rc1/hsml/python/model.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/python/predictor.py` & `hsml-3.2.0rc1/hsml/python/predictor.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/python/signature.py` & `hsml-3.2.0rc1/hsml/python/signature.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/resources.py` & `hsml-3.2.0rc1/hsml/resources.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/schema.py` & `hsml-3.2.0rc1/hsml/schema.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/sklearn/__init__.py` & `hsml-3.2.0rc1/hsml/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/sklearn/model.py` & `hsml-3.2.0rc1/hsml/sklearn/model.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/sklearn/predictor.py` & `hsml-3.2.0rc1/hsml/sklearn/predictor.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/sklearn/signature.py` & `hsml-3.2.0rc1/hsml/sklearn/signature.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/tag.py` & `hsml-3.2.0rc1/hsml/tag.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/tensorflow/__init__.py` & `hsml-3.2.0rc1/hsml/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/tensorflow/model.py` & `hsml-3.2.0rc1/hsml/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/tensorflow/predictor.py` & `hsml-3.2.0rc1/hsml/tensorflow/predictor.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/tensorflow/signature.py` & `hsml-3.2.0rc1/hsml/tensorflow/signature.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/torch/__init__.py` & `hsml-3.2.0rc1/hsml/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/torch/model.py` & `hsml-3.2.0rc1/hsml/torch/model.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/torch/predictor.py` & `hsml-3.2.0rc1/hsml/torch/predictor.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/torch/signature.py` & `hsml-3.2.0rc1/hsml/torch/signature.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/transformer.py` & `hsml-3.2.0rc1/hsml/transformer.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/util.py` & `hsml-3.2.0rc1/hsml/util.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/utils/__init__.py` & `hsml-3.2.0rc1/hsml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/utils/schema/__init__.py` & `hsml-3.2.0rc1/hsml/utils/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/utils/schema/column.py` & `hsml-3.2.0rc1/hsml/utils/schema/column.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/utils/schema/columnar_schema.py` & `hsml-3.2.0rc1/hsml/utils/schema/columnar_schema.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/utils/schema/tensor.py` & `hsml-3.2.0rc1/hsml/utils/schema/tensor.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/utils/schema/tensor_schema.py` & `hsml-3.2.0rc1/hsml/utils/schema/tensor_schema.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/hsml/version.py` & `hsml-3.2.0rc1/hsml/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-__version__ = "3.2.0rc0"
+__version__ = "3.2.0rc1"
```

### Comparing `hsml-3.2.0rc0/hsml.egg-info/PKG-INFO` & `hsml-3.2.0rc1/hsml.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsml
-Version: 3.2.0rc0
+Version: 3.2.0rc1
 Summary: HSML: An environment independent client to interact with the Hopsworks Model Registry
 Home-page: https://github.com/logicalclocks/machine-learning-api
 Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/machine-learning-api/releases/tag/3.2.0rc0
+Download-URL: https://github.com/logicalclocks/machine-learning-api/releases/tag/3.2.0rc1
 Description: # Hopsworks Model Management
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: hsml Version: 3.2.0rc0 Summary: HSML: An
+Metadata-Version: 2.1 Name: hsml Version: 3.2.0rc1 Summary: HSML: An
 environment independent client to interact with the Hopsworks Model Registry
 Home-page: https://github.com/logicalclocks/machine-learning-api Author:
 Logical Clocks AB Author-email: robin@logicalclocks.com License: Apache License
 2.0 Download-URL: https://github.com/logicalclocks/machine-learning-api/
-releases/tag/3.2.0rc0 Description: # Hopsworks Model Management
+releases/tag/3.2.0rc1 Description: # Hopsworks Model Management
 [Hopsworks_Community] [Hopsworks_Model_Management_Documentation] [PyPiStatus]
            [Scala/Java_Artifacts] [Downloads] [CodeStyle] [License]
 HSML is the library to interact with the Hopsworks Model Registry and Model
 Serving. The library makes it easy to export, manage and deploy models. The
 library automatically configures itself based on the environment it is run.
 However, to connect from an external Python environment additional connection
 information, such as host and port, is required. For more information about the
```

### Comparing `hsml-3.2.0rc0/hsml.egg-info/SOURCES.txt` & `hsml-3.2.0rc1/hsml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/setup.py` & `hsml-3.2.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/tests/__init__.py` & `hsml-3.2.0rc1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/tests/hsml/__init__.py` & `hsml-3.2.0rc1/tests/hsml/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.2.0rc0/tests/hsml/core/__init__.py` & `hsml-3.2.0rc1/tests/hsml/core/__init__.py`

 * *Files identical despite different names*

