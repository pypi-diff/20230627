# Comparing `tmp/pyrecdp-1.0.1b2023062716.tar.gz` & `tmp/pyrecdp-1.0.1b2023062717.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyrecdp-1.0.1b2023062716.tar", last modified: Tue Jun 27 08:59:34 2023, max compression
+gzip compressed data, was "dist/pyrecdp-1.0.1b2023062717.tar", last modified: Tue Jun 27 09:07:41 2023, max compression
```

## Comparing `pyrecdp-1.0.1b2023062716.tar` & `pyrecdp-1.0.1b2023062717.tar`

### file list

```diff
@@ -1,111 +1,112 @@
-drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/
-drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp.egg-info/
--rw-rw-r--   0 ht        (1000) docker     (998)     3355 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp.egg-info/SOURCES.txt
--rw-rw-r--   0 ht        (1000) docker     (998)        1 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp.egg-info/not-zip-safe
--rw-rw-r--   0 ht        (1000) docker     (998)       26 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp.egg-info/top_level.txt
--rw-rw-r--   0 ht        (1000) docker     (998)    10482 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp.egg-info/PKG-INFO
--rw-rw-r--   0 ht        (1000) docker     (998)        1 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp.egg-info/dependency_links.txt
--rw-rw-r--   0 ht        (1000) docker     (998)      221 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp.egg-info/requires.txt
--rw-rw-r--   0 ht        (1000) docker     (998)      189 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/MANIFEST.in
--rw-rw-r--   0 ht        (1000) docker     (998)       38 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/setup.cfg
--rw-rw-r--   0 ht        (1000) docker     (998)     1538 2023-06-27 08:47:21.000000 pyrecdp-1.0.1b2023062716/setup.py
--rw-rw-r--   0 ht        (1000) docker     (998)    10482 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/PKG-INFO
--rw-rw-r--   0 ht        (1000) docker     (998)     8315 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/README.md
-drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/ScalaProcessUtils/
--rw-rw-r--   0 ht        (1000) docker     (998)        0 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/ScalaProcessUtils/__init__.py
-drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/
-drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/
--rw-rw-r--   0 ht        (1000) docker     (998)      689 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/ibm_fraud_detect.py
--rw-rw-r--   0 ht        (1000) docker     (998)      428 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/twitter_recsys.py
--rw-rw-r--   0 ht        (1000) docker     (998)     1208 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/nyc_taxi.py
--rw-rw-r--   0 ht        (1000) docker     (998)      288 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/download.py
--rw-rw-r--   0 ht        (1000) docker     (998)      358 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/__init__.py
--rw-rw-r--   0 ht        (1000) docker     (998)      680 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/amazon_product_review.py
--rw-rw-r--   0 ht        (1000) docker     (998)     2942 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/CESM_breast_cancer.py
--rw-rw-r--   0 ht        (1000) docker     (998)     4186 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/base_api.py
--rw-rw-r--   0 ht        (1000) docker     (998)      905 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/outbrain.py
--rw-rw-r--   0 ht        (1000) docker     (998)      408 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/pretrained.py
-drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/core/
--rw-rw-r--   0 ht        (1000) docker     (998)     5696 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/core/schema.py
--rw-rw-r--   0 ht        (1000) docker     (998)     6782 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/core/utils.py
--rw-rw-r--   0 ht        (1000) docker     (998)      908 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/core/dataframe.py
--rw-rw-r--   0 ht        (1000) docker     (998)      186 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/core/__init__.py
--rw-rw-r--   0 ht        (1000) docker     (998)     2849 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/core/di_graph.py
-drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/
--rw-rw-r--   0 ht        (1000) docker     (998)      166 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/utils.py
--rw-rw-r--   0 ht        (1000) docker     (998)      821 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/TabWidget.py
--rw-rw-r--   0 ht        (1000) docker     (998)      221 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/__init__.py
--rw-rw-r--   0 ht        (1000) docker     (998)     1092 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/BaseWidget.py
--rw-rw-r--   0 ht        (1000) docker     (998)        0 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/PlotWidget.py
-drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/
--rw-rw-r--   0 ht        (1000) docker     (998)     7110 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/scripts.html
--rw-rw-r--   0 ht        (1000) docker     (998)      260 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/interactions.html
--rw-rw-r--   0 ht        (1000) docker     (998)    16515 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/styles.html
--rw-rw-r--   0 ht        (1000) docker     (998)      989 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/base.html
--rw-rw-r--   0 ht        (1000) docker     (998)     9250 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/variables.html
--rw-rw-r--   0 ht        (1000) docker     (998)       85 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/error.html
--rw-rw-r--   0 ht        (1000) docker     (998)     1340 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/overview.html
--rw-rw-r--   0 ht        (1000) docker     (998)     2103 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/TableViewWidget.py
--rw-rw-r--   0 ht        (1000) docker     (998)        0 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/ProfilerWidget.py
--rw-rw-r--   0 ht        (1000) docker     (998)     1142 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/__init__.py
-drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/autofe/
--rw-rw-r--   0 ht        (1000) docker     (998)     4030 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/autofe/AutoFE.py
--rw-rw-r--   0 ht        (1000) docker     (998)      218 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/autofe/__init__.py
--rw-rw-r--   0 ht        (1000) docker     (998)     4523 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/autofe/FeatureEstimator.py
--rw-rw-r--   0 ht        (1000) docker     (998)     3106 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/autofe/FeatureProfiler.py
--rw-rw-r--   0 ht        (1000) docker     (998)     3008 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/autofe/FeatureWrangler.py
--rw-rw-r--   0 ht        (1000) docker     (998)    13765 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/autofe/BasePipeline.py
--rw-rw-r--   0 ht        (1000) docker     (998)     1684 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/autofe/RelationalBuilder.py
-drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/
-drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/
--rw-rw-r--   0 ht        (1000) docker     (998)     4666 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/geograph.py
--rw-rw-r--   0 ht        (1000) docker     (998)     1854 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/__init__.py
--rw-rw-r--   0 ht        (1000) docker     (998)     4720 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/relation.py
--rw-rw-r--   0 ht        (1000) docker     (998)     4141 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/encode.py
--rw-rw-r--   0 ht        (1000) docker     (998)     1398 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/drop.py
--rw-rw-r--   0 ht        (1000) docker     (998)     2975 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/type.py
--rw-rw-r--   0 ht        (1000) docker     (998)     1334 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/featuretools_adaptor.py
--rw-rw-r--   0 ht        (1000) docker     (998)     1620 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/datetime.py
--rw-rw-r--   0 ht        (1000) docker     (998)     3100 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/nlp.py
--rw-rw-r--   0 ht        (1000) docker     (998)     1240 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/category.py
--rw-rw-r--   0 ht        (1000) docker     (998)     1180 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/fillna.py
--rw-rw-r--   0 ht        (1000) docker     (998)      269 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/binned.py
--rw-rw-r--   0 ht        (1000) docker     (998)      234 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/base.py
--rw-rw-r--   0 ht        (1000) docker     (998)     1221 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/feature_transform.py
--rw-rw-r--   0 ht        (1000) docker     (998)     1575 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/name.py
-drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/
--rw-rw-r--   0 ht        (1000) docker     (998)     2293 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/data.py
--rw-rw-r--   0 ht        (1000) docker     (998)      682 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/geograph.py
--rw-rw-r--   0 ht        (1000) docker     (998)     3291 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/dataframe.py
--rw-rw-r--   0 ht        (1000) docker     (998)      712 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/tuple.py
--rw-rw-r--   0 ht        (1000) docker     (998)      153 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/__init__.py
--rw-rw-r--   0 ht        (1000) docker     (998)     1376 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/merge.py
--rw-rw-r--   0 ht        (1000) docker     (998)     3735 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/encode.py
--rw-rw-r--   0 ht        (1000) docker     (998)      758 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/drop.py
--rw-rw-r--   0 ht        (1000) docker     (998)     1086 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/type.py
--rw-rw-r--   0 ht        (1000) docker     (998)      950 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/featuretools_adaptor.py
--rw-rw-r--   0 ht        (1000) docker     (998)     2233 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/category.py
--rw-rw-r--   0 ht        (1000) docker     (998)      351 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/custom.py
--rw-rw-r--   0 ht        (1000) docker     (998)      674 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/fillna.py
--rw-rw-r--   0 ht        (1000) docker     (998)     6028 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/base.py
--rw-rw-r--   0 ht        (1000) docker     (998)      709 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/name.py
--rw-rw-r--   0 ht        (1000) docker     (998)       76 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/__init__.py
-drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/spark_data_processor/
--rw-rw-r--   0 ht        (1000) docker     (998)     8145 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/spark_data_processor/encoder.py
--rw-rw-r--   0 ht        (1000) docker     (998)     8699 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/spark_data_processor/utils.py
--rw-rw-r--   0 ht        (1000) docker     (998)    54072 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/spark_data_processor/data_processor.py
--rw-rw-r--   0 ht        (1000) docker     (998)        0 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/spark_data_processor/__init__.py
-drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/profilers/
--rw-rw-r--   0 ht        (1000) docker     (998)      157 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/profilers/__init__.py
--rw-rw-r--   0 ht        (1000) docker     (998)     5674 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/profilers/statics.py
--rw-rw-r--   0 ht        (1000) docker     (998)     4398 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/profilers/type_infer.py
-drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/estimators/
--rw-rw-r--   0 ht        (1000) docker     (998)     2656 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/estimators/lightgbm.py
--rw-rw-r--   0 ht        (1000) docker     (998)        0 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/estimators/__init__.py
--rw-rw-r--   0 ht        (1000) docker     (998)     2091 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/estimators/base.py
-drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/ScalaProcessUtils/
--rw-rw-r--   0 ht        (1000) docker     (998)      624 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/ScalaProcessUtils/spark-defaults.conf
--rw-rw-r--   0 ht        (1000) docker     (998)        0 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/ScalaProcessUtils/__init__.py
--rw-rw-r--   0 ht        (1000) docker     (998)      559 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/ScalaProcessUtils/spark-env.sh
-drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/ScalaProcessUtils/target/
--rw-rw-r--   0 ht        (1000) docker     (998)   114879 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/
+-rw-rw-r--   0 ht        (1000) docker     (998)      189 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/MANIFEST.in
+-rw-rw-r--   0 ht        (1000) docker     (998)    10482 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/PKG-INFO
+-rw-rw-r--   0 ht        (1000) docker     (998)     8315 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/README.md
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/ScalaProcessUtils/
+-rw-rw-r--   0 ht        (1000) docker     (998)        0 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/ScalaProcessUtils/__init__.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      104 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyproject.toml
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp/
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp/ScalaProcessUtils/
+-rw-rw-r--   0 ht        (1000) docker     (998)        0 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/ScalaProcessUtils/__init__.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      624 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/ScalaProcessUtils/spark-defaults.conf
+-rw-rw-r--   0 ht        (1000) docker     (998)      559 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/ScalaProcessUtils/spark-env.sh
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp/ScalaProcessUtils/target/
+-rw-rw-r--   0 ht        (1000) docker     (998)   114879 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
+-rw-rw-r--   0 ht        (1000) docker     (998)     1142 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/__init__.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp/autofe/
+-rw-rw-r--   0 ht        (1000) docker     (998)     4030 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/autofe/AutoFE.py
+-rw-rw-r--   0 ht        (1000) docker     (998)    13765 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/autofe/BasePipeline.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     4523 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/autofe/FeatureEstimator.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     3106 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/autofe/FeatureProfiler.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     3008 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/autofe/FeatureWrangler.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1684 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/autofe/RelationalBuilder.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      218 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/autofe/__init__.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp/core/
+-rw-rw-r--   0 ht        (1000) docker     (998)      186 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/core/__init__.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      908 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/core/dataframe.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     2849 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/core/di_graph.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     5696 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/core/schema.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     6782 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/core/utils.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp/datasets/
+-rw-rw-r--   0 ht        (1000) docker     (998)     2942 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/datasets/CESM_breast_cancer.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      358 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/datasets/__init__.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      680 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/datasets/amazon_product_review.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     4186 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/datasets/base_api.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      288 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/datasets/download.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      689 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/datasets/ibm_fraud_detect.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1208 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/datasets/nyc_taxi.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      905 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/datasets/outbrain.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      408 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/datasets/pretrained.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      428 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/datasets/twitter_recsys.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/
+-rw-rw-r--   0 ht        (1000) docker     (998)       76 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/__init__.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/estimators/
+-rw-rw-r--   0 ht        (1000) docker     (998)        0 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/estimators/__init__.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     2091 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/estimators/base.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     2656 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/estimators/lightgbm.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/
+-rw-rw-r--   0 ht        (1000) docker     (998)     1854 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/__init__.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      234 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/base.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      269 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/binned.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1240 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/category.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1620 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/datetime.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1398 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/drop.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     4141 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/encode.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1221 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/feature_transform.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1334 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/featuretools_adaptor.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1180 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/fillna.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     4666 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/geograph.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1575 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/name.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     3100 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/nlp.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     4720 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/relation.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     2975 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/type.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/
+-rw-rw-r--   0 ht        (1000) docker     (998)      153 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/__init__.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     6028 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/base.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     2233 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/category.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      351 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/custom.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     2293 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/data.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     3291 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/dataframe.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      758 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/drop.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     3735 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/encode.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      950 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/featuretools_adaptor.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      674 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/fillna.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      682 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/geograph.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1376 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/merge.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      709 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/name.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      712 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/tuple.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1086 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/type.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/profilers/
+-rw-rw-r--   0 ht        (1000) docker     (998)      157 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/profilers/__init__.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     5674 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/profilers/statics.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     4398 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/profilers/type_infer.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/spark_data_processor/
+-rw-rw-r--   0 ht        (1000) docker     (998)        0 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/spark_data_processor/__init__.py
+-rw-rw-r--   0 ht        (1000) docker     (998)    54072 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/spark_data_processor/data_processor.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     8145 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/spark_data_processor/encoder.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     8699 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/primitives/spark_data_processor/utils.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp/widgets/
+-rw-rw-r--   0 ht        (1000) docker     (998)     1092 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/widgets/BaseWidget.py
+-rw-rw-r--   0 ht        (1000) docker     (998)        0 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/widgets/PlotWidget.py
+-rw-rw-r--   0 ht        (1000) docker     (998)        0 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/widgets/ProfilerWidget.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      821 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/widgets/TabWidget.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     2103 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/widgets/TableViewWidget.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      221 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/widgets/__init__.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp/widgets/templates/
+-rw-rw-r--   0 ht        (1000) docker     (998)      989 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/widgets/templates/base.html
+-rw-rw-r--   0 ht        (1000) docker     (998)       85 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/widgets/templates/error.html
+-rw-rw-r--   0 ht        (1000) docker     (998)      260 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/widgets/templates/interactions.html
+-rw-rw-r--   0 ht        (1000) docker     (998)     1340 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/widgets/templates/overview.html
+-rw-rw-r--   0 ht        (1000) docker     (998)     7110 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/widgets/templates/scripts.html
+-rw-rw-r--   0 ht        (1000) docker     (998)    16515 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/widgets/templates/styles.html
+-rw-rw-r--   0 ht        (1000) docker     (998)     9250 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/widgets/templates/variables.html
+-rw-rw-r--   0 ht        (1000) docker     (998)      166 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062717/pyrecdp/widgets/utils.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp.egg-info/
+-rw-rw-r--   0 ht        (1000) docker     (998)    10482 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp.egg-info/PKG-INFO
+-rw-rw-r--   0 ht        (1000) docker     (998)     3370 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp.egg-info/SOURCES.txt
+-rw-rw-r--   0 ht        (1000) docker     (998)        1 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp.egg-info/dependency_links.txt
+-rw-rw-r--   0 ht        (1000) docker     (998)        1 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp.egg-info/not-zip-safe
+-rw-rw-r--   0 ht        (1000) docker     (998)      221 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp.egg-info/requires.txt
+-rw-rw-r--   0 ht        (1000) docker     (998)       26 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/pyrecdp.egg-info/top_level.txt
+-rw-rw-r--   0 ht        (1000) docker     (998)       38 2023-06-27 09:07:41.000000 pyrecdp-1.0.1b2023062717/setup.cfg
+-rw-rw-r--   0 ht        (1000) docker     (998)     1538 2023-06-27 08:47:21.000000 pyrecdp-1.0.1b2023062717/setup.py
```

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp.egg-info/SOURCES.txt` & `pyrecdp-1.0.1b2023062717/pyrecdp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 ScalaProcessUtils/__init__.py
 pyrecdp/__init__.py
 pyrecdp.egg-info/PKG-INFO
 pyrecdp.egg-info/SOURCES.txt
 pyrecdp.egg-info/dependency_links.txt
 pyrecdp.egg-info/not-zip-safe
```

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp.egg-info/PKG-INFO` & `pyrecdp-1.0.1b2023062717/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.0.1b2023062716
+Version: 1.0.1b2023062717
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
 Description: # RecDP v2.0
```

### Comparing `pyrecdp-1.0.1b2023062716/setup.py` & `pyrecdp-1.0.1b2023062717/setup.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/PKG-INFO` & `pyrecdp-1.0.1b2023062717/pyrecdp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.0.1b2023062716
+Version: 1.0.1b2023062717
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
 Description: # RecDP v2.0
```

### Comparing `pyrecdp-1.0.1b2023062716/README.md` & `pyrecdp-1.0.1b2023062717/README.md`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/datasets/ibm_fraud_detect.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/datasets/ibm_fraud_detect.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/datasets/nyc_taxi.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/datasets/nyc_taxi.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/datasets/amazon_product_review.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/datasets/amazon_product_review.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/datasets/CESM_breast_cancer.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/datasets/CESM_breast_cancer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/datasets/base_api.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/datasets/base_api.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/datasets/outbrain.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/datasets/outbrain.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/core/schema.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/core/schema.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/core/utils.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/core/utils.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/core/dataframe.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/core/di_graph.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/core/di_graph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/widgets/TabWidget.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/widgets/TabWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/widgets/BaseWidget.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/widgets/BaseWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/scripts.html` & `pyrecdp-1.0.1b2023062717/pyrecdp/widgets/templates/scripts.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/styles.html` & `pyrecdp-1.0.1b2023062717/pyrecdp/widgets/templates/styles.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/base.html` & `pyrecdp-1.0.1b2023062717/pyrecdp/widgets/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/variables.html` & `pyrecdp-1.0.1b2023062717/pyrecdp/widgets/templates/variables.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/overview.html` & `pyrecdp-1.0.1b2023062717/pyrecdp/widgets/templates/overview.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/widgets/TableViewWidget.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/widgets/TableViewWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/__init__.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/autofe/AutoFE.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/autofe/AutoFE.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/autofe/FeatureEstimator.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/autofe/FeatureEstimator.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/autofe/FeatureProfiler.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/autofe/FeatureProfiler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/autofe/FeatureWrangler.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/autofe/FeatureWrangler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/autofe/BasePipeline.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/autofe/BasePipeline.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/autofe/RelationalBuilder.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/autofe/RelationalBuilder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/geograph.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/geograph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/__init__.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/relation.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/relation.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/encode.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/encode.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/drop.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/drop.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/type.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/featuretools_adaptor.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/featuretools_adaptor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/datetime.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/datetime.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/nlp.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/nlp.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/category.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/category.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/fillna.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/feature_transform.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/feature_transform.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/name.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/generators/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/data.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/data.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/geograph.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/geograph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/dataframe.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/tuple.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/tuple.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/merge.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/merge.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/encode.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/encode.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/drop.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/drop.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/type.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/featuretools_adaptor.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/featuretools_adaptor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/category.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/category.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/fillna.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/base.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/base.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/name.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/operations/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/spark_data_processor/encoder.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/spark_data_processor/encoder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/spark_data_processor/utils.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/spark_data_processor/utils.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/spark_data_processor/data_processor.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/spark_data_processor/data_processor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/profilers/statics.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/profilers/statics.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/profilers/type_infer.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/profilers/type_infer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/estimators/lightgbm.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/estimators/lightgbm.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/estimators/base.py` & `pyrecdp-1.0.1b2023062717/pyrecdp/primitives/estimators/base.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/ScalaProcessUtils/spark-defaults.conf` & `pyrecdp-1.0.1b2023062717/pyrecdp/ScalaProcessUtils/spark-defaults.conf`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/ScalaProcessUtils/spark-env.sh` & `pyrecdp-1.0.1b2023062717/pyrecdp/ScalaProcessUtils/spark-env.sh`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b2023062716/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar` & `pyrecdp-1.0.1b2023062717/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar`

 * *Files identical despite different names*

