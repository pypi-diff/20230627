# Comparing `tmp/pyrecdp-1.0.1b202306061.tar.gz` & `tmp/pyrecdp-1.0.1b2023062716.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrecdp-1.0.1b202306061.tar", last modified: Tue Jun  6 22:28:10 2023, max compression
+gzip compressed data, was "dist/pyrecdp-1.0.1b2023062716.tar", last modified: Tue Jun 27 08:59:34 2023, max compression
```

## Comparing `pyrecdp-1.0.1b202306061.tar` & `pyrecdp-1.0.1b2023062716.tar`

### file list

```diff
@@ -1,113 +1,111 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.151224 pyrecdp-1.0.1b202306061/
--rw-r--r--   0 root         (0) root         (0)    94051 2023-06-02 20:11:31.000000 pyrecdp-1.0.1b202306061/LICENSE
--rw-r--r--   0 root         (0) root         (0)      189 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8860 2023-06-06 22:28:10.151224 pyrecdp-1.0.1b202306061/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8315 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.143224 pyrecdp-1.0.1b202306061/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-02 20:11:31.000000 pyrecdp-1.0.1b202306061/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.143224 pyrecdp-1.0.1b202306061/pyrecdp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.143224 pyrecdp-1.0.1b202306061/pyrecdp/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/ScalaProcessUtils/spark-defaults.conf
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/ScalaProcessUtils/spark-env.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.143224 pyrecdp-1.0.1b202306061/pyrecdp/ScalaProcessUtils/target/
--rw-r--r--   0 root         (0) root         (0)   114879 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
--rw-r--r--   0 root         (0) root         (0)     1001 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/autofe/
--rw-r--r--   0 root         (0) root         (0)     4010 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/autofe/AutoFE.py
--rw-r--r--   0 root         (0) root         (0)    13436 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/autofe/BasePipeline.py
--rw-r--r--   0 root         (0) root         (0)     4496 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/autofe/FeatureEstimator.py
--rw-r--r--   0 root         (0) root         (0)     3106 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/autofe/FeatureProfiler.py
--rw-r--r--   0 root         (0) root         (0)     3008 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/autofe/FeatureWrangler.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/autofe/RelationalBuilder.py
--rw-r--r--   0 root         (0) root         (0)      218 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/autofe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/core/
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      742 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/core/dataframe.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/core/di_graph.py
--rw-r--r--   0 root         (0) root         (0)     5696 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/core/schema.py
--rw-r--r--   0 root         (0) root         (0)     6420 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/datasets/
--rw-r--r--   0 root         (0) root         (0)     2942 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/CESM_breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)      358 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      680 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/amazon_product_review.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/base_api.py
--rw-r--r--   0 root         (0) root         (0)      288 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/download.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/ibm_fraud_detect.py
--rw-r--r--   0 root         (0) root         (0)     1208 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/nyc_taxi.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/outbrain.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/pretrained.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/datasets/twitter_recsys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/primitives/
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/primitives/estimators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/estimators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2091 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/estimators/base.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/estimators/lightgbm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/
--rw-r--r--   0 root         (0) root         (0)     1855 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/base.py
--rw-r--r--   0 root         (0) root         (0)      269 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/binned.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/category.py
--rw-r--r--   0 root         (0) root         (0)     1620 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/datetime.py
--rw-r--r--   0 root         (0) root         (0)     1398 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/drop.py
--rw-r--r--   0 root         (0) root         (0)     4047 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/encode.py
--rw-r--r--   0 root         (0) root         (0)     1221 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/feature_transform.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/fillna.py
--rw-r--r--   0 root         (0) root         (0)     4666 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/geograph.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/name.py
--rw-r--r--   0 root         (0) root         (0)     3100 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/nlp.py
--rw-r--r--   0 root         (0) root         (0)     4720 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/relation.py
--rw-r--r--   0 root         (0) root         (0)     2975 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6028 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/base.py
--rw-r--r--   0 root         (0) root         (0)     2233 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/category.py
--rw-r--r--   0 root         (0) root         (0)      351 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/custom.py
--rw-r--r--   0 root         (0) root         (0)     1929 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/data.py
--rw-r--r--   0 root         (0) root         (0)     3291 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/dataframe.py
--rw-r--r--   0 root         (0) root         (0)      758 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/drop.py
--rw-r--r--   0 root         (0) root         (0)     3940 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/encode.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/fillna.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/geograph.py
--rw-r--r--   0 root         (0) root         (0)     1376 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/merge.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/name.py
--rw-r--r--   0 root         (0) root         (0)      712 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/tuple.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/primitives/profilers/
--rw-r--r--   0 root         (0) root         (0)      157 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/profilers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5757 2023-06-06 22:13:53.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/profilers/statics.py
--rw-r--r--   0 root         (0) root         (0)     4398 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/profilers/type_infer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/primitives/spark_data_processor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/spark_data_processor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54029 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/spark_data_processor/data_processor.py
--rw-r--r--   0 root         (0) root         (0)     8145 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/spark_data_processor/encoder.py
--rw-r--r--   0 root         (0) root         (0)     8115 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/primitives/spark_data_processor/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/widgets/
--rw-r--r--   0 root         (0) root         (0)     1092 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/BaseWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/PlotWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/ProfilerWidget.py
--rw-r--r--   0 root         (0) root         (0)      821 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/TabWidget.py
--rw-r--r--   0 root         (0) root         (0)     2103 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/TableViewWidget.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.147224 pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/
--rw-r--r--   0 root         (0) root         (0)      989 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/base.html
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/error.html
--rw-r--r--   0 root         (0) root         (0)      260 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/interactions.html
--rw-r--r--   0 root         (0) root         (0)     1340 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/overview.html
--rw-r--r--   0 root         (0) root         (0)     7110 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/scripts.html
--rw-r--r--   0 root         (0) root         (0)    16515 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/styles.html
--rw-r--r--   0 root         (0) root         (0)     9250 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/variables.html
--rw-r--r--   0 root         (0) root         (0)      166 2023-06-02 20:28:07.000000 pyrecdp-1.0.1b202306061/pyrecdp/widgets/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 22:28:10.143224 pyrecdp-1.0.1b202306061/pyrecdp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8860 2023-06-06 22:28:10.000000 pyrecdp-1.0.1b202306061/pyrecdp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3378 2023-06-06 22:28:10.000000 pyrecdp-1.0.1b202306061/pyrecdp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 22:28:10.000000 pyrecdp-1.0.1b202306061/pyrecdp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 20:27:26.000000 pyrecdp-1.0.1b202306061/pyrecdp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      221 2023-06-06 22:28:10.000000 pyrecdp-1.0.1b202306061/pyrecdp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-06 22:28:10.000000 pyrecdp-1.0.1b202306061/pyrecdp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 22:28:10.151224 pyrecdp-1.0.1b202306061/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1486 2023-06-06 22:27:24.000000 pyrecdp-1.0.1b202306061/setup.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp.egg-info/
+-rw-rw-r--   0 ht        (1000) docker     (998)     3355 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp.egg-info/SOURCES.txt
+-rw-rw-r--   0 ht        (1000) docker     (998)        1 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp.egg-info/not-zip-safe
+-rw-rw-r--   0 ht        (1000) docker     (998)       26 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp.egg-info/top_level.txt
+-rw-rw-r--   0 ht        (1000) docker     (998)    10482 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp.egg-info/PKG-INFO
+-rw-rw-r--   0 ht        (1000) docker     (998)        1 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp.egg-info/dependency_links.txt
+-rw-rw-r--   0 ht        (1000) docker     (998)      221 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp.egg-info/requires.txt
+-rw-rw-r--   0 ht        (1000) docker     (998)      189 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/MANIFEST.in
+-rw-rw-r--   0 ht        (1000) docker     (998)       38 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/setup.cfg
+-rw-rw-r--   0 ht        (1000) docker     (998)     1538 2023-06-27 08:47:21.000000 pyrecdp-1.0.1b2023062716/setup.py
+-rw-rw-r--   0 ht        (1000) docker     (998)    10482 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/PKG-INFO
+-rw-rw-r--   0 ht        (1000) docker     (998)     8315 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/README.md
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/ScalaProcessUtils/
+-rw-rw-r--   0 ht        (1000) docker     (998)        0 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/ScalaProcessUtils/__init__.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/
+-rw-rw-r--   0 ht        (1000) docker     (998)      689 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/ibm_fraud_detect.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      428 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/twitter_recsys.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1208 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/nyc_taxi.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      288 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/download.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      358 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/__init__.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      680 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/amazon_product_review.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     2942 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/CESM_breast_cancer.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     4186 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/base_api.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      905 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/outbrain.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      408 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/datasets/pretrained.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/core/
+-rw-rw-r--   0 ht        (1000) docker     (998)     5696 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/core/schema.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     6782 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/core/utils.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      908 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/core/dataframe.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      186 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/core/__init__.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     2849 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/core/di_graph.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/
+-rw-rw-r--   0 ht        (1000) docker     (998)      166 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/utils.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      821 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/TabWidget.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      221 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/__init__.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1092 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/BaseWidget.py
+-rw-rw-r--   0 ht        (1000) docker     (998)        0 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/PlotWidget.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/
+-rw-rw-r--   0 ht        (1000) docker     (998)     7110 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/scripts.html
+-rw-rw-r--   0 ht        (1000) docker     (998)      260 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/interactions.html
+-rw-rw-r--   0 ht        (1000) docker     (998)    16515 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/styles.html
+-rw-rw-r--   0 ht        (1000) docker     (998)      989 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/base.html
+-rw-rw-r--   0 ht        (1000) docker     (998)     9250 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/variables.html
+-rw-rw-r--   0 ht        (1000) docker     (998)       85 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/error.html
+-rw-rw-r--   0 ht        (1000) docker     (998)     1340 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/overview.html
+-rw-rw-r--   0 ht        (1000) docker     (998)     2103 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/TableViewWidget.py
+-rw-rw-r--   0 ht        (1000) docker     (998)        0 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/widgets/ProfilerWidget.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1142 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/__init__.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/autofe/
+-rw-rw-r--   0 ht        (1000) docker     (998)     4030 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/autofe/AutoFE.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      218 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/autofe/__init__.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     4523 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/autofe/FeatureEstimator.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     3106 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/autofe/FeatureProfiler.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     3008 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/autofe/FeatureWrangler.py
+-rw-rw-r--   0 ht        (1000) docker     (998)    13765 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/autofe/BasePipeline.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1684 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/autofe/RelationalBuilder.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/
+-rw-rw-r--   0 ht        (1000) docker     (998)     4666 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/geograph.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1854 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/__init__.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     4720 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/relation.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     4141 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/encode.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1398 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/drop.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     2975 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/type.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1334 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/featuretools_adaptor.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1620 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/datetime.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     3100 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/nlp.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1240 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/category.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1180 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/fillna.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      269 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/binned.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      234 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/base.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1221 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/feature_transform.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1575 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/name.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/
+-rw-rw-r--   0 ht        (1000) docker     (998)     2293 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/data.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      682 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/geograph.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     3291 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/dataframe.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      712 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/tuple.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      153 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/__init__.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1376 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/merge.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     3735 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/encode.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      758 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/drop.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     1086 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/type.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      950 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/featuretools_adaptor.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     2233 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/category.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      351 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/custom.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      674 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/fillna.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     6028 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/base.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      709 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/name.py
+-rw-rw-r--   0 ht        (1000) docker     (998)       76 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/__init__.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/spark_data_processor/
+-rw-rw-r--   0 ht        (1000) docker     (998)     8145 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/spark_data_processor/encoder.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     8699 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/spark_data_processor/utils.py
+-rw-rw-r--   0 ht        (1000) docker     (998)    54072 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/spark_data_processor/data_processor.py
+-rw-rw-r--   0 ht        (1000) docker     (998)        0 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/spark_data_processor/__init__.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/profilers/
+-rw-rw-r--   0 ht        (1000) docker     (998)      157 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/profilers/__init__.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     5674 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/profilers/statics.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     4398 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/profilers/type_infer.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/estimators/
+-rw-rw-r--   0 ht        (1000) docker     (998)     2656 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/estimators/lightgbm.py
+-rw-rw-r--   0 ht        (1000) docker     (998)        0 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/estimators/__init__.py
+-rw-rw-r--   0 ht        (1000) docker     (998)     2091 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/primitives/estimators/base.py
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/ScalaProcessUtils/
+-rw-rw-r--   0 ht        (1000) docker     (998)      624 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/ScalaProcessUtils/spark-defaults.conf
+-rw-rw-r--   0 ht        (1000) docker     (998)        0 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/ScalaProcessUtils/__init__.py
+-rw-rw-r--   0 ht        (1000) docker     (998)      559 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/ScalaProcessUtils/spark-env.sh
+drwxrwxr-x   0 ht        (1000) docker     (998)        0 2023-06-27 08:59:34.000000 pyrecdp-1.0.1b2023062716/pyrecdp/ScalaProcessUtils/target/
+-rw-rw-r--   0 ht        (1000) docker     (998)   114879 2023-06-27 08:38:49.000000 pyrecdp-1.0.1b2023062716/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pyrecdp-1.0.1b202306061/PKG-INFO` & `pyrecdp-1.0.1b2023062716/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: pyrecdp
-Version: 1.0.1b202306061
-Summary: A data processing bundle for spark based recommender system operations
-Home-page: https://github.com/intel/e2eAIOK/
-Author: INTEL AIA
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # RecDP v2.0
 
 # INTRODUCTION
 
 ## Problem Statement
 
 Data Preparation is an essential step to build AI pipelines 
@@ -214,9 +198,7 @@
 
 ## LICENSE
 * Apache 2.0
 
 ## Dependency
 * Spark 3.x
 * python 3.*
-
-
```

### Comparing `pyrecdp-1.0.1b202306061/README.md` & `pyrecdp-1.0.1b2023062716/pyrecdp.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,204 +1,219 @@
-# RecDP v2.0
-
-# INTRODUCTION
-
-## Problem Statement
-
-Data Preparation is an essential step to build AI pipelines 
-* key data preparation capabilities: data connector, cleaning, sampling, joining, profiling, feature engineering, low-code/no-code UI, lineage etc. 
-* exploration of optimal Data preparation consumes majority of Data Science time
-
-## Solution with RecDP v2.0
-
-* Auto pipeline
-    * only 3 lines of codes required
-* Pipeline Generator
-    * Data Profiling:
-        * Auto anomalies detection
-        * Auto missing value impute
-        * Profiling Visualizzation        
-    * Feature Wrangling:
-        * feature transformation(datetime, geo_info, text_nlp, url, etc.)
-        * multiple data auto joining
-        * feature cross(aggregation transformation - sum, avg, count, etc.)
-    * export pipeline as JSON file, can be import to other data platform
-* Pipeline Runner:
-    * spark engine: convert pipeline to spark codes to run
-    * pandas engine: convert pipeline to pandas codes to run
-    * sql engine: convert pipeline to sql
-* DataLoader:
-    * parquet, csv, json, database
-* FeatureWriter - ML/DL connector:
-    * Data Lineage
-    * Feature Store
-    * numpy, csv, parquet, dgl / pyG graph
-![RecDP v2.0 Overview](resources/recdp_intro.png)
-
-## This solution is intended for
-citizen data scientists, enterprise users, independent software vendor and partial of cloud service provider.
-
-# Getting Start
-## setup with pip
-```
-git clone --single-branch --branch RecDP_v2.0 https://github.com/intel-innersource/frameworks.bigdata.AIDK.git
-cd frameworks.bigdata.AIDK/RecDP
-# install dependencies
-apt-get update -y &&  DEBIAN_FRONTEND=noninteractive apt-get install -y python3 python3-pip python-is-python3 graphviz
-DEBIAN_FRONTEND=noninteractive apt-get install -y openjdk-8-jre
-# install recdp
-python setup.py sdist
-pip install dist/pyrecdp-1.0.1.tar.gz
-
-sh start-jupyter.sh
-# open browser with http://hostname:8888
-```
-
-## run
-![nyc taxi demo](https://github.com/intel-innersource/frameworks.bigdata.AIDK/assets/4355494/03d8c2fe-de47-41f9-9fef-8513bc4aaf42)
-
-## modify pipeline (add user defined function or remove operation)
-``` python
-def filter_with_cond(df):
-    df = df[df['Year'] <= 2018]
-    return df
-operation = {
-    "children": [6], # will to append this new op
-    "next": [7], # who will be connected to this new op
-    "inline_function": filter_with_cond, # function
-}
-pipeline.add_operation(operation)
-```
-``` python
-operation = {
-    "idx": 6, # OP id to be deleted
-    "next": [10] # who is connected to the to_be_deleted op
-}
-pipeline.delete_operation(operation)
-```
-
-## export pipeline
-``` python
-pipeline.export(file_path = "exported_pipeline.json")
-```
-``` json
-{
-    "0": {
-        "children": null,
-        "op": "DataFrame",
-        "config": "main_table"
-    },
-    "1": {
-        "children": [0],
-        "op": "type_infer",
-        "config": [
-            ["pickup_datetime",["is_string","is_datetime"]],
-            ["pickup_longitude",["is_numeric","is_float"]],
-            ["pickup_latitude",["is_numeric","is_float"]],
-            ["dropoff_longitude",["is_numeric","is_float"]],
-            ["dropoff_latitude",["is_numeric","is_float"]],
-            ["passenger_count",["is_numeric","is_int64","is_integer","is_categorical"]]
-        ]
-    },
-    "2": {
-        "children": [1],
-        "op": "tuple",
-        "config": {
-            "src": ["pickup_latitude","pickup_longitude"],"dst": "pickup_coordinates"
-        }
-    },
-    "3": {
-        "children": [2],
-        "op": "tuple",
-        "config": {
-            "src": ["dropoff_latitude","dropoff_longitude"],"dst": "dropoff_coordinates"
-        }
-    },
-    "4": {
-        "children": [3],
-        "op": "fillna",
-        "config": {
-            "pickup_longitude": -1,
-            "pickup_latitude": -1,
-            "dropoff_longitude": -1,
-            "dropoff_latitude": -1,
-            "passenger_count": -1
-        }
-    },
-    "5": {
-        "children": [4],
-        "op": "datetime_feature",
-        "config": {
-            "pickup_datetime": [
-                ["pickup_datetime__day",["featuretools.primitives.standard.transform.datetime.day", "Day"]],
-                ["pickup_datetime__month",["featuretools.primitives.standard.transform.datetime.month","Month"]],
-                ["pickup_datetime__weekday",["featuretools.primitives.standard.transform.datetime.weekday","Weekday"]],
-                ["pickup_datetime__year",["featuretools.primitives.standard.transform.datetime.year","Year"]],
-                ["pickup_datetime__hour",["featuretools.primitives.standard.transform.datetime.hour","Hour"]]
-            ]
-        }
-    },
-    "6": {
-        "children": [5],
-        "op": "haversine",
-        "config": {
-            "['pickup_coordinates', 'dropoff_coordinates']": ["haversine_pickup_coordinates_dropoff_coordinates",["featuretools.primitives.standard.transform.latlong.haversine","Haversine"]]
-        }
-    },
-    "7": {
-        "children": [6],
-        "op": "drop",
-        "config": [
-            "pickup_datetime",
-            "pickup_coordinates",
-            "dropoff_coordinates"
-        ]
-    },
-    "8": {
-        "children": [7],
-        "op": "lightgbm",
-        "config": {
-            "label": "fare_amount",
-            "metrics": "rmse",
-            "objective": "regression",
-            "model_file": "lightgbm_regression_label.mdl",
-            "method": "predict"
-        }
-    }
-}
-```
-
-
-## Quick Example
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/de044d606e6cdc44d3005db2a0ae968d/recdp_fare_prediction.ipynb) - [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_train.ipynb) - geographic, datetime, lgbm regression
-
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2b8acb3eda73028635072352560139ba/recdp_fraud_detect.ipynb) - [IBM Card Transaction Fraud Detect](examples/notebooks/autofe/demo/fraud_detect_train.ipynb) - onehot encode, lgbm, binary classification 
-
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/b039b8c0a40fec951b1b09c3fbb93a7b/recdp_social_media.ipynb) - [twitter recsys](examples/notebooks/autofe/demo/twitter_workflow_test.ipynb) - text nlp, datetime feature engineering  
-
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/1e08668ab0e15e1e98c592f284d79dad/recdp_click_through_rate_multiple_tables.ipynb) - [outbrain](examples/notebooks/autofe/demo/outbrain_ctr_workflow_test.ipynb) - multiple table joining
-
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2f942c30dbf9b63a64cc819a61966e34/recdp_rating_prediction_amazon_review.ipynb) - [amazon product review](examples/notebooks/autofe/demo/amazon_product_review_test.ipynb) - text nlp, datetime, feature-cross
-
-# More Examples - completed example including training
-
-## Auto Feature Engineering vs. featuretools
-* [NYC Taxi fare auto data prepration](examples/notebooks/autofe/FeatureWrangler.ipynb): An example to show how RecDP_v2.0 automatically generating datetime and geo features upon 55M records. Tested with both Spark and Pandas(featuretools) as compute engine, show 21x speedup by spark.
-
-## load PIPELINE and execute
-* [twitter pipeline re-load and execute](examples/notebooks/autofe/demo/custom_pipeline_twitter.ipynb): An example to show how RecDP_v2.0 reload pipeline from json and do execution - use RecDP as compute engine.
-
-## Realtime Inference pipeline
-* [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_predict.ipynb) - geographic, datetime feature engineering, lgbm
-
-## Data Profiler Examples
-* [NYC Taxi fare Profiler](resources/FeatureProfiler_NYC.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
-
-* [twitter Profiler](resources/FeatureProfiler_recsys.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
-
-
-## LICENSE
-* Apache 2.0
-
-## Dependency
-* Spark 3.x
-* python 3.*
+Metadata-Version: 2.1
+Name: pyrecdp
+Version: 1.0.1b2023062716
+Summary: A data processing bundle for spark based recommender system operations
+Home-page: https://github.com/intel/e2eAIOK/
+Author: INTEL AIA
+License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
+Description: # RecDP v2.0
+        
+        # INTRODUCTION
+        
+        ## Problem Statement
+        
+        Data Preparation is an essential step to build AI pipelines 
+        * key data preparation capabilities: data connector, cleaning, sampling, joining, profiling, feature engineering, low-code/no-code UI, lineage etc. 
+        * exploration of optimal Data preparation consumes majority of Data Science time
+        
+        ## Solution with RecDP v2.0
+        
+        * Auto pipeline
+            * only 3 lines of codes required
+        * Pipeline Generator
+            * Data Profiling:
+                * Auto anomalies detection
+                * Auto missing value impute
+                * Profiling Visualizzation        
+            * Feature Wrangling:
+                * feature transformation(datetime, geo_info, text_nlp, url, etc.)
+                * multiple data auto joining
+                * feature cross(aggregation transformation - sum, avg, count, etc.)
+            * export pipeline as JSON file, can be import to other data platform
+        * Pipeline Runner:
+            * spark engine: convert pipeline to spark codes to run
+            * pandas engine: convert pipeline to pandas codes to run
+            * sql engine: convert pipeline to sql
+        * DataLoader:
+            * parquet, csv, json, database
+        * FeatureWriter - ML/DL connector:
+            * Data Lineage
+            * Feature Store
+            * numpy, csv, parquet, dgl / pyG graph
+        ![RecDP v2.0 Overview](resources/recdp_intro.png)
+        
+        ## This solution is intended for
+        citizen data scientists, enterprise users, independent software vendor and partial of cloud service provider.
+        
+        # Getting Start
+        ## setup with pip
+        ```
+        git clone --single-branch --branch RecDP_v2.0 https://github.com/intel-innersource/frameworks.bigdata.AIDK.git
+        cd frameworks.bigdata.AIDK/RecDP
+        # install dependencies
+        apt-get update -y &&  DEBIAN_FRONTEND=noninteractive apt-get install -y python3 python3-pip python-is-python3 graphviz
+        DEBIAN_FRONTEND=noninteractive apt-get install -y openjdk-8-jre
+        # install recdp
+        python setup.py sdist
+        pip install dist/pyrecdp-1.0.1.tar.gz
+        
+        sh start-jupyter.sh
+        # open browser with http://hostname:8888
+        ```
+        
+        ## run
+        ![nyc taxi demo](https://github.com/intel-innersource/frameworks.bigdata.AIDK/assets/4355494/03d8c2fe-de47-41f9-9fef-8513bc4aaf42)
+        
+        ## modify pipeline (add user defined function or remove operation)
+        ``` python
+        def filter_with_cond(df):
+            df = df[df['Year'] <= 2018]
+            return df
+        operation = {
+            "children": [6], # will to append this new op
+            "next": [7], # who will be connected to this new op
+            "inline_function": filter_with_cond, # function
+        }
+        pipeline.add_operation(operation)
+        ```
+        ``` python
+        operation = {
+            "idx": 6, # OP id to be deleted
+            "next": [10] # who is connected to the to_be_deleted op
+        }
+        pipeline.delete_operation(operation)
+        ```
+        
+        ## export pipeline
+        ``` python
+        pipeline.export(file_path = "exported_pipeline.json")
+        ```
+        ``` json
+        {
+            "0": {
+                "children": null,
+                "op": "DataFrame",
+                "config": "main_table"
+            },
+            "1": {
+                "children": [0],
+                "op": "type_infer",
+                "config": [
+                    ["pickup_datetime",["is_string","is_datetime"]],
+                    ["pickup_longitude",["is_numeric","is_float"]],
+                    ["pickup_latitude",["is_numeric","is_float"]],
+                    ["dropoff_longitude",["is_numeric","is_float"]],
+                    ["dropoff_latitude",["is_numeric","is_float"]],
+                    ["passenger_count",["is_numeric","is_int64","is_integer","is_categorical"]]
+                ]
+            },
+            "2": {
+                "children": [1],
+                "op": "tuple",
+                "config": {
+                    "src": ["pickup_latitude","pickup_longitude"],"dst": "pickup_coordinates"
+                }
+            },
+            "3": {
+                "children": [2],
+                "op": "tuple",
+                "config": {
+                    "src": ["dropoff_latitude","dropoff_longitude"],"dst": "dropoff_coordinates"
+                }
+            },
+            "4": {
+                "children": [3],
+                "op": "fillna",
+                "config": {
+                    "pickup_longitude": -1,
+                    "pickup_latitude": -1,
+                    "dropoff_longitude": -1,
+                    "dropoff_latitude": -1,
+                    "passenger_count": -1
+                }
+            },
+            "5": {
+                "children": [4],
+                "op": "datetime_feature",
+                "config": {
+                    "pickup_datetime": [
+                        ["pickup_datetime__day",["featuretools.primitives.standard.transform.datetime.day", "Day"]],
+                        ["pickup_datetime__month",["featuretools.primitives.standard.transform.datetime.month","Month"]],
+                        ["pickup_datetime__weekday",["featuretools.primitives.standard.transform.datetime.weekday","Weekday"]],
+                        ["pickup_datetime__year",["featuretools.primitives.standard.transform.datetime.year","Year"]],
+                        ["pickup_datetime__hour",["featuretools.primitives.standard.transform.datetime.hour","Hour"]]
+                    ]
+                }
+            },
+            "6": {
+                "children": [5],
+                "op": "haversine",
+                "config": {
+                    "['pickup_coordinates', 'dropoff_coordinates']": ["haversine_pickup_coordinates_dropoff_coordinates",["featuretools.primitives.standard.transform.latlong.haversine","Haversine"]]
+                }
+            },
+            "7": {
+                "children": [6],
+                "op": "drop",
+                "config": [
+                    "pickup_datetime",
+                    "pickup_coordinates",
+                    "dropoff_coordinates"
+                ]
+            },
+            "8": {
+                "children": [7],
+                "op": "lightgbm",
+                "config": {
+                    "label": "fare_amount",
+                    "metrics": "rmse",
+                    "objective": "regression",
+                    "model_file": "lightgbm_regression_label.mdl",
+                    "method": "predict"
+                }
+            }
+        }
+        ```
+        
+        
+        ## Quick Example
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/de044d606e6cdc44d3005db2a0ae968d/recdp_fare_prediction.ipynb) - [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_train.ipynb) - geographic, datetime, lgbm regression
+        
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2b8acb3eda73028635072352560139ba/recdp_fraud_detect.ipynb) - [IBM Card Transaction Fraud Detect](examples/notebooks/autofe/demo/fraud_detect_train.ipynb) - onehot encode, lgbm, binary classification 
+        
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/b039b8c0a40fec951b1b09c3fbb93a7b/recdp_social_media.ipynb) - [twitter recsys](examples/notebooks/autofe/demo/twitter_workflow_test.ipynb) - text nlp, datetime feature engineering  
+        
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/1e08668ab0e15e1e98c592f284d79dad/recdp_click_through_rate_multiple_tables.ipynb) - [outbrain](examples/notebooks/autofe/demo/outbrain_ctr_workflow_test.ipynb) - multiple table joining
+        
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2f942c30dbf9b63a64cc819a61966e34/recdp_rating_prediction_amazon_review.ipynb) - [amazon product review](examples/notebooks/autofe/demo/amazon_product_review_test.ipynb) - text nlp, datetime, feature-cross
+        
+        # More Examples - completed example including training
+        
+        ## Auto Feature Engineering vs. featuretools
+        * [NYC Taxi fare auto data prepration](examples/notebooks/autofe/FeatureWrangler.ipynb): An example to show how RecDP_v2.0 automatically generating datetime and geo features upon 55M records. Tested with both Spark and Pandas(featuretools) as compute engine, show 21x speedup by spark.
+        
+        ## load PIPELINE and execute
+        * [twitter pipeline re-load and execute](examples/notebooks/autofe/demo/custom_pipeline_twitter.ipynb): An example to show how RecDP_v2.0 reload pipeline from json and do execution - use RecDP as compute engine.
+        
+        ## Realtime Inference pipeline
+        * [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_predict.ipynb) - geographic, datetime feature engineering, lgbm
+        
+        ## Data Profiler Examples
+        * [NYC Taxi fare Profiler](resources/FeatureProfiler_NYC.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
+        
+        * [twitter Profiler](resources/FeatureProfiler_recsys.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
+        
+        
+        ## LICENSE
+        * Apache 2.0
+        
+        ## Dependency
+        * Spark 3.x
+        * python 3.*
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/ScalaProcessUtils/spark-defaults.conf` & `pyrecdp-1.0.1b2023062716/pyrecdp/ScalaProcessUtils/spark-defaults.conf`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar` & `pyrecdp-1.0.1b2023062716/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/__init__.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,17 @@
     libpath = str(Path(__file__).parent.resolve())
     spark_home_dir = f"{libpath}/spark-3.2.1-bin-hadoop3.2"
     py4j_path = f"{spark_home_dir}/python/lib/py4j-0.10.9.3-src.zip"
     os.environ["SPARK_HOME"]=spark_home_dir
     # Add the PySpark classes to the Python path:
     os.environ["PYTHONPATH"]=os.environ["SPARK_HOME"]+"/python/:"+os.environ["PYTHONPATH"]+":"+py4j_path
 
-os.environ["JAVA_HOME"]="/usr/lib/jvm/java-8-openjdk-amd64/"
+if not os.environ.get('JAVA_HOME', None): 
+    os.environ['JAVA_HOME'] = "/usr/lib/jvm/java-8-openjdk-amd64/"
+    print(f"JAVA_HOME is not set, use default value of /usr/lib/jvm/java-8-openjdk-amd64/")
 os.environ["PYSPARK_PYTHON"]=sys.executable
 os.environ["PYSPARK_DRIVER_PYTHON"]=sys.executable
 os.environ["PYSPARK_WORKER_PYTHON"]=sys.executable
 
 import pyrecdp.primitives.spark_data_processor.utils as utils
 sys.modules['pyrecdp.utils'] = utils
 import pyrecdp.primitives.spark_data_processor.encoder as encoder
```

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/autofe/AutoFE.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/autofe/AutoFE.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,29 +19,29 @@
             print("AutoFE started to profile data")
             self.auto_pipeline['profiler'] = FeatureProfiler(dataset=dataset, label=label)
             print("AutoFE started to create data pipeline")
             self.auto_pipeline['wrangler'] = FeatureWrangler(dataset=dataset, label=label)
             pipeline = self.auto_pipeline['wrangler']
             config = {
                 'model_file': 'autofe_lightgbm.mdl',
-                'objective': infer_problem_type(pipeline.dataset[pipeline.main_table][label]),
+                'objective': infer_problem_type(pipeline.dataset[pipeline.main_table], label),
                 'model_name': 'lightgbm'}
             self.auto_pipeline['estimator'] = FeatureEstimator(data_pipeline = pipeline, config = config)
 
     def fit_transform(self, engine_type = 'pandas', no_cache = False, *args, **kwargs):
         print("AutoFE started to execute data")
         ret_df = None
         if self.auto_pipeline['relational']:
             pipeline = self.auto_pipeline['relational']
-            ret_df = pipeline.fit_transform(engine_type, data = ret_df)
+            ret_df = pipeline.fit_transform(engine_type, data = ret_df, **kwargs)
             print("AutoFE started to profile data")
 
         if self.auto_pipeline['estimator']:
             pipeline = self.auto_pipeline['estimator']
-            ret_df = pipeline.fit_transform(engine_type, data = ret_df)
+            ret_df = pipeline.fit_transform(engine_type, data = ret_df, **kwargs)
         return ret_df
     
     def profile(self, engine_type = 'pandas'):
         if isinstance(self.auto_pipeline['profiler'], type(None)):
             return "feature profile support for multiple table is WIP"
         return self.auto_pipeline['profiler'].visualize_analyze(engine_type)
```

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/autofe/BasePipeline.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/autofe/BasePipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pyrecdp.primitives.generators import *
 from pyrecdp.core import DataFrameSchema, SparkDataProcessor, DiGraph
-from pyrecdp.primitives.operations import Operation, DataFrameOperation, RDDToDataFrameConverter
+from pyrecdp.primitives.operations import Operation, DataFrameOperation, RDDToDataFrameConverter, TargetEncodeOperation
 import pandas as pd
 import logging
 import graphviz
 import json
 from pyrecdp.core.utils import Timer, sample_read, deepcopy
 from pyspark.sql import DataFrame as SparkDataFrame
 from pyspark import RDD as SparkRDD
@@ -263,14 +263,16 @@
                     if isinstance(op, DataFrameOperation):
                         if data:
                             input_df = data
                         else:
                             input_df = self.dataset if start_op_idx == -1 else {'main_table': self.transformed_cache}
                         input_df = deepcopy(input_df) if no_cache else input_df
                         op.set(input_df)
+                    if isinstance(op, TargetEncodeOperation):
+                        op.set(self.y)
                     with Timer(f"execute {op}"):
                         op.execute_pd(executable_pipeline)
             if transformed_end == -1:
                 df = executable_sequence[-1].cache
             else:
                 df = executable_pipeline[transformed_end].cache
         elif engine_type == 'spark':
@@ -309,15 +311,19 @@
 
     def fit_transform(self, engine_type = 'pandas', no_cache = False, data = None, *args, **kwargs):
         if not no_cache and hasattr(self, 'transformed_cache') and self.transformed_cache is not None:
             print("Detect pre-transformed cache, return cached data")
             print("If re-transform is required, please use fit_transform(no_cache = True)")
             return self.transformed_cache
         if engine_type == "spark":
-            self.rdp = SparkDataProcessor()
+            if "spark_master" in kwargs:
+                spark_master = kwargs["spark_master"]
+            else:
+                spark_master = "local[*]"
+            self.rdp = SparkDataProcessor(spark_mode='standalone', spark_master=spark_master)
         ret = self.execute(engine_type = engine_type, no_cache = no_cache, data = data)
         if engine_type == "spark":
             del self.rdp 
             self.rdp = None
         self.transformed_cache = ret
         return ret
```

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/autofe/FeatureEstimator.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/autofe/FeatureEstimator.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         elif isinstance(data_pipeline, BasePipeline):
             self.nested_pipeline_obj = data_pipeline
             self.pipeline = data_pipeline.pipeline
             self.dataset = data_pipeline.dataset
             self.rdp = data_pipeline.rdp
             self.transformed_cache = data_pipeline.transformed_cache if hasattr(data_pipeline, 'transformed_cache') else None
             label = data_pipeline.y if label is None else label
+            self.y = label
         else:
             raise NotImplementedError(f"Unsupport input datapipeline is {data_pipeline}")
         if label is None and method != 'predict':
             raise ValueError("Unable to find label for this pipeline, please provide it through API")
         
         max_idx = self.pipeline.get_max_idx()
         leaf_idx = self.pipeline.convert_to_node_chain()[-1]
```

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/autofe/FeatureProfiler.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/autofe/FeatureProfiler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/autofe/FeatureWrangler.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/autofe/FeatureWrangler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/autofe/RelationalBuilder.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/autofe/RelationalBuilder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/core/di_graph.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/core/di_graph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/core/schema.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/core/schema.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/core/utils.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/core/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,15 +122,24 @@
         ret = s
     elif isinstance(s, tuple) or isinstance(s, list):
         import importlib
         module = importlib.import_module(s[0])
         ret = eval("module." + s[1])
     return ret
 
-def infer_problem_type(y):
+def infer_problem_type(df, label):
+    if isinstance(df, str):
+        if df.endswith('.csv'):
+            y = pd.read_csv(df)[label]
+        elif df.endswith('.parquet'):
+            y = pd.read_parquet(df)[label]
+        else:
+            raise NotImplementedError("Load DataFrame based on path only support csv and parquet")
+    elif isinstance(df, pd.DataFrame):
+        y = df[label]
     unique_count = y.nunique()
     if unique_count == 2:
         problem_type = 'binary'
     elif y.dtype.name in ['object', 'category', 'string']:
         problem_type = 'multiclass'
     else:
         problem_type = 'regression'
```

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/datasets/CESM_breast_cancer.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/datasets/CESM_breast_cancer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/datasets/amazon_product_review.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/datasets/amazon_product_review.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/datasets/base_api.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/datasets/base_api.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/datasets/ibm_fraud_detect.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/datasets/ibm_fraud_detect.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/datasets/nyc_taxi.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/datasets/nyc_taxi.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/datasets/outbrain.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/datasets/outbrain.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/estimators/base.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/estimators/base.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/estimators/lightgbm.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/estimators/lightgbm.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/__init__.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 pre_enocode_feature_generator_list = [
     DropUselessFeatureGenerator,
 ]
 
 global_dict_index_generator_list = [
     BinnedFeatureGenerator,
     CategoryFeatureGenerator,
-    #TargetEncodeFeatureGenerator
+    TargetEncodeFeatureGenerator
 ]
 
 post_feature_generator_list = [
     RenameFeatureGenerator
 ]
 
 final_generator_list = [
```

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/category.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/category.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/datetime.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/datetime.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/drop.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/drop.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/encode.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/encode.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .base import BaseFeatureGenerator as super_class
 import pandas as pd
 from pyrecdp.core import SeriesSchema
 from pyrecdp.primitives.operations import Operation
+import copy
 
 class LabelEncodeFeatureGenerator(super_class):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     def fit_prepare(self, pipeline, children, max_idx):
         is_useful = False
@@ -77,21 +78,23 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.feature_in = []
 
     def fit_prepare(self, pipeline, children, max_idx):
         is_useful = False
         pa_schema = pipeline[children[0]].output
-        config = {}
+        feature_in_out = {}
+        ret_pa_schema = copy.deepcopy(pa_schema)
         for pa_field in pa_schema:
-            if pa_field.is_onehot:
+            if pa_field.is_categorical_and_string:
                 feature = pa_field.name
-                out_schema = [SeriesSchema(f"{feature}__{key}", int) for key in pa_field.config["is_onehot"]]
-                config[pa_field.name] = pa_field.config["is_onehot"]
+                out_schema = SeriesSchema(f"{feature}__TE", pd.CategoricalDtype())
+                feature_in_out[feature] = out_schema.name
                 is_useful = True
-                pa_schema.extend(out_schema)
+                ret_pa_schema.append(out_schema)
         if is_useful:
             cur_idx = max_idx + 1
-            pipeline[cur_idx] = Operation(cur_idx, children, pa_schema, op = 'categorify', config = config)
+            config = feature_in_out
+            pipeline[cur_idx] = Operation(cur_idx, children, ret_pa_schema, op = 'target_encode', config = config)
             return pipeline, cur_idx, cur_idx
         else:
             return pipeline, children[0], max_idx
```

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/feature_transform.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/feature_transform.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/featuretools_adaptor.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/featuretools_adaptor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/fillna.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/geograph.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/geograph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/name.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/nlp.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/nlp.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/relation.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/relation.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/generators/type.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/generators/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/base.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/base.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/category.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/category.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/data.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,8 +44,18 @@
             file_path = self.op.config['file_path']
             if file_path.endswith('.csv'):
                 return rdp.spark.read.csv(file_path, header=True, inferSchema=True)
             elif file_path.endswith('.parquet'):
                 return rdp.spark.read.parquet(file_path)
             else:
                 raise NotImplementedError("now sample read only support csv and parquet")
-        return get_dataframe
+        return get_dataframe
+    
+    def execute_pd(self, pipeline):
+        assert not self.op.children or len(self.op.children) == 0
+        _proc = self.get_function_pd()
+        self.cache = _proc()
+    
+    def execute_spark(self, pipeline, rdp):
+        assert not self.op.children or len(self.op.children) == 0
+        _proc = self.get_function_spark(rdp)
+        self.cache = _proc()
```

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/dataframe.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/drop.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/drop.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/encode.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/encode.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,30 +48,28 @@
             return df
         return encode
     
 
 class TargetEncodeOperation(BaseOperation):
     def __init__(self, op_base):
         super().__init__(op_base)
-        self.feature_in = self.op.config
+        self.feature_in_out = self.op.config
         self.support_spark_dataframe = False
         self.support_spark_rdd = True
     
+    def set(self, label):
+        self.label = label
+    
     def get_function_pd(self):
         from category_encoders import TargetEncoder
-        feature_in = copy.deepcopy(self.feature_in)
+        feature_in_out = copy.deepcopy(self.feature_in_out)
         def encode(df):
-            added_data = {}
-            for feature, (dict_path, target_label) in feature_in.items():
+            for feature, feature_out in feature_in_out.items():
                 encoder = TargetEncoder(cols=[feature], min_samples_leaf=20, smoothing=10)
-                encoder = get_encoder_np(encoder, dict_path)
-                added_data[f"{feature}_TE"] = encoder.fit_transform(df[feature], df[target_label])[feature]
-                save_encoder_np(encoder, dict_path)
-            to_concat_df = pd.DataFrame.from_dict(data = added_data)
-            df = pd.concat([df, to_concat_df], axis = 1)
+                df[f"{feature_out}"] = pd.Series(encoder.fit_transform(df[feature], df[self.label])[feature])
             return df
         return encode
     
 class CountEncodeOperation(BaseOperation):
     def __init__(self, op_base):
         super().__init__(op_base)
         self.feature_in = self.op.config
```

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/featuretools_adaptor.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/featuretools_adaptor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/fillna.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/geograph.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/geograph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/merge.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/merge.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/name.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/tuple.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/tuple.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/operations/type.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/operations/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/profilers/statics.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/profilers/statics.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 from pyrecdp.core import SeriesSchema
 from pyrecdp.core.utils import is_text_series
 from pyrecdp.core.utils import Timer
 import pandas as pd
 import numpy as np
 from tqdm import tqdm
 from pyrecdp.core.dataframe import DataFrameAPI
-import matplotlib.pyplot as plt
 
 def draw_xy_scatter_plot(xy_scatter_features, feature_data, y, row_height, n_plot_per_row):
+    from plotly.subplots import make_subplots
+    import plotly.graph_objs as go
     import math
     
     n_feat = len(xy_scatter_features)
     n_row = math.ceil(n_feat / n_plot_per_row)
     n_col = n_plot_per_row if n_feat > n_plot_per_row else n_feat
-    label = y.name
+    subplot_titles = xy_scatter_features
 
-    height = int(n_row * 3)
-    fig, axs = plt.subplots(nrows=n_row, ncols=n_col, figsize=(10,height))
+    fig_list = make_subplots(rows=n_row, cols=n_col, subplot_titles  = subplot_titles, y_title = y.name)
 
     X = DataFrameAPI().instiate(feature_data)
     sampled_data = X.may_sample(nrows = 1000)
     y = sampled_data[y.name]
 
     for idx, c_name in tqdm(enumerate(xy_scatter_features), total=len(xy_scatter_features)):
         feature = sampled_data[c_name]
         # if string, wrap when too long
         sch = SeriesSchema(feature)
         is_feature_string = True if (sch.is_string or sch.is_categorical_and_string) else False
         
-        row_id = int(idx / n_plot_per_row)
-        col_id = idx % n_plot_per_row
         if is_feature_string:
             tmp = feature.str.slice(0, 12, 1)
-            axs[row_id, col_id].scatter(x=tmp, y=y, s=5)
+            fig = go.Scatter(x=tmp, y=y, mode='markers', name=c_name, showlegend=False)
         else:
-            axs[row_id, col_id].scatter(x=feature, y=y, s=5)
-         
-        axs[row_id, col_id].set_xlabel(c_name)
-        axs[row_id, col_id].set_ylabel(label)
+            fig = go.Scatter(x=feature, y=y, mode='markers', name=c_name, showlegend=False)
+
+        fig_list.add_trace(fig, row = int(idx / n_plot_per_row) + 1, col = ((idx % n_plot_per_row) + 1))
 
+    print("prepare xy scatter subplot completed, start to add them as one global plot")
+    fig_list.update_layout(height=row_height * n_row, width=400 * n_col)
     print("prepare xy scatter plot completed")
     
-    fig.tight_layout()
-    return fig
+    return fig_list
 
 def draw_mapbox_plot(mapbox_scatter_features, feature_data):
     import plotly.graph_objs as go
 
     from shapely.geometry import MultiPoint
     fig_list = go.Figure()
 
@@ -115,16 +113,14 @@
         interactions_detail = self.get_interactive_plot(X, y)
         data_stats['interactions']=(dict(), interactions_detail)
         
         return data_stats
     
     def get_interactive_plot(self, feature_data, y):
         from plotly.offline import plot
-        import base64
-        from io import BytesIO
         row_height = 300
         n_plot_per_row = 2
         
         # we will create types of plot
         xy_scatter_features = []
         mapbox_scatter_features = []
         word_cloud_features = []
@@ -143,20 +139,16 @@
         
         ret = {}
         ret = {"error": False}
 
         # draw xy scatter
         if len(xy_scatter_features) > 0:
             with Timer("Draw xy scatter plot"):
-                fig = draw_xy_scatter_plot(xy_scatter_features, feature_data, y, row_height, n_plot_per_row)
-                tmpfile = BytesIO()
-                fig.savefig(tmpfile, format='png')
-                plt.close(fig)
-                encoded = base64.b64encode(tmpfile.getvalue()).decode('utf-8')
-                ret['html'] = '<div><img src=\'data:image/png;base64,{}\'></div>'.format(encoded)
+                fig_list = draw_xy_scatter_plot(xy_scatter_features, feature_data, y, row_height, n_plot_per_row)
+            ret['html'] = plot(fig_list, output_type='div')
         
         # draw mapbox
         if len(mapbox_scatter_features) > 0:
             with Timer("Draw mapbox plot"):
                 fig_list = draw_mapbox_plot(mapbox_scatter_features, feature_data)
             ret['html'] += plot(fig_list, output_type='div')
```

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/profilers/type_infer.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/profilers/type_infer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/spark_data_processor/data_processor.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/spark_data_processor/data_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -983,19 +983,19 @@
                     df = df.withColumn('max_hist_len', spk_func.col('row_cnt'))
                 df = df.withColumn(f'hist_{c}', spk_func.expr(f"slice(hist_{c}, 1, max_hist_len - 1)"))
             df = df.drop('row_id').drop('row_cnt').drop('max_hist_len')
         return df
 
 
 class DataProcessor:
-    def __init__(self, spark = None, path_prefix="file://", current_path="", shuffle_disk_capacity="unlimited", dicts_path="dicts", spark_mode='local', enable_gazelle=False):
+    def __init__(self, spark = None, path_prefix="file://", current_path="", shuffle_disk_capacity="unlimited", dicts_path="dicts", spark_mode='local', spark_master=None, enable_gazelle=False):
         self.ops = []
         self.stop_spark_in_del = False
         if not spark:
-            spark = create_spark_context()
+            spark = create_spark_context(spark_mode, spark_master)
             self.stop_spark_in_del = True
         self.spark = spark
         self.uuid = uuid.uuid1()
         self.tmp_id = 0
         self.path_prefix = path_prefix
         self.current_path = current_path
         self.dicts_path = dicts_path
```

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/spark_data_processor/encoder.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/spark_data_processor/encoder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/primitives/spark_data_processor/utils.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/primitives/spark_data_processor/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,30 +8,38 @@
 import pyspark.sql.types as spk_type
 import pyspark.sql.functions as spk_func
 import psutil
 
 from pathlib import Path
 pathlib = Path(__file__).parent.parent.resolve()
 
-def create_spark_context():
-    hname = os.uname()[1]
-    paral = psutil.cpu_count(logical=False)
-    total_mem = int((psutil.virtual_memory().total / (1 << 20)) * 0.8)
-    print(f"Will assign {paral} cores and {total_mem} M memory for spark")
-    spark = SparkSession.builder.master(f'local[{paral}]')\
-                .appName("pyrecdp_spark_local")\
-                .config("spark.executorEnv.HF_DATASETS_OFFLINE", "1")\
-                .config("spark.executorEnv.TRANSFORMERS_OFFLINE", "1")\
-                .config("spark.executorEnv.TF_CPP_MIN_LOG_LEVEL", "2")\
-                .config("spark.executorEnv.PYTHONPATH", pathlib)\
-                .config("spark.driver.memory", f"{total_mem}M")\
-                .config("spark.driver.maxResultSize","64g")\
-                .config("spark.sql.execution.arrow.pyspark.enabled","true")\
-                .config("spark.sql.parquet.int96RebaseModeInWrite","CORRECTED")\
-                .getOrCreate()
+def create_spark_context(spark_mode='local', spark_master=None):
+    if spark_mode == 'yarn' or spark_mode == 'standalone':
+        if spark_master is None:
+            raise ValueError("Spark master is None, please set correct spark master!")
+        spark = SparkSession.builder.master(spark_master)\
+                    .config("spark.sql.parquet.int96RebaseModeInWrite","CORRECTED")\
+                    .config("spark.sql.execution.arrow.pyspark.enabled","true")\
+                    .getOrCreate()
+    else:
+        hname = os.uname()[1]
+        paral = psutil.cpu_count(logical=False)
+        total_mem = int((psutil.virtual_memory().total / (1 << 20)) * 0.8)
+        print(f"Will assign {paral} cores and {total_mem} M memory for spark")
+        spark = SparkSession.builder.master(f'local[{paral}]')\
+                    .appName("pyrecdp_spark_local")\
+                    .config("spark.executorEnv.HF_DATASETS_OFFLINE", "1")\
+                    .config("spark.executorEnv.TRANSFORMERS_OFFLINE", "1")\
+                    .config("spark.executorEnv.TF_CPP_MIN_LOG_LEVEL", "2")\
+                    .config("spark.executorEnv.PYTHONPATH", pathlib)\
+                    .config("spark.driver.memory", f"{total_mem}M")\
+                    .config("spark.driver.maxResultSize","64g")\
+                    .config("spark.sql.execution.arrow.pyspark.enabled","true")\
+                    .config("spark.sql.parquet.int96RebaseModeInWrite","CORRECTED")\
+                    .getOrCreate()
     spark.sparkContext.setLogLevel("ERROR")
     # try:
     #     spark = SparkSession.builder.master(f'spark://{hname}:7077')\
     #             .appName("pyrecdp_spark_standalone").getOrCreate()
     #     SparkContext.addPyFile() //this need to be zip, implement later
     # except:
     #     spark = SparkSession.builder.master(f'local[*]')\
@@ -72,14 +80,16 @@
             else:
                 source_path_dict[files] = os.path.join(path, files)
     return source_path_dict
 
 
 def parse_size(size):
     units = {"B": 1, "KB": 2**10, "MB": 2**20, "GB": 2**30, "TB": 2**40, "K": 2**10, "M": 2**20, "G": 2**30, "T": 2**40}
+    if size is None:
+        return 0
     size = size.upper()
     number, unit = re.findall('(\d+)(\w*)', size)[0]
     return int(float(number)*units[unit])
 
 
 def parse_cores_num(local_str):
     number = re.findall('local\[(\d+)\]', local_str)
```

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/widgets/BaseWidget.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/widgets/BaseWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/widgets/TabWidget.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/widgets/TabWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/widgets/TableViewWidget.py` & `pyrecdp-1.0.1b2023062716/pyrecdp/widgets/TableViewWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/base.html` & `pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/overview.html` & `pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/overview.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/scripts.html` & `pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/scripts.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/styles.html` & `pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/styles.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp/widgets/templates/variables.html` & `pyrecdp-1.0.1b2023062716/pyrecdp/widgets/templates/variables.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp.egg-info/PKG-INFO` & `pyrecdp-1.0.1b2023062716/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,222 +1,219 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.0.1b202306061
+Version: 1.0.1b2023062716
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
+Description: # RecDP v2.0
+        
+        # INTRODUCTION
+        
+        ## Problem Statement
+        
+        Data Preparation is an essential step to build AI pipelines 
+        * key data preparation capabilities: data connector, cleaning, sampling, joining, profiling, feature engineering, low-code/no-code UI, lineage etc. 
+        * exploration of optimal Data preparation consumes majority of Data Science time
+        
+        ## Solution with RecDP v2.0
+        
+        * Auto pipeline
+            * only 3 lines of codes required
+        * Pipeline Generator
+            * Data Profiling:
+                * Auto anomalies detection
+                * Auto missing value impute
+                * Profiling Visualizzation        
+            * Feature Wrangling:
+                * feature transformation(datetime, geo_info, text_nlp, url, etc.)
+                * multiple data auto joining
+                * feature cross(aggregation transformation - sum, avg, count, etc.)
+            * export pipeline as JSON file, can be import to other data platform
+        * Pipeline Runner:
+            * spark engine: convert pipeline to spark codes to run
+            * pandas engine: convert pipeline to pandas codes to run
+            * sql engine: convert pipeline to sql
+        * DataLoader:
+            * parquet, csv, json, database
+        * FeatureWriter - ML/DL connector:
+            * Data Lineage
+            * Feature Store
+            * numpy, csv, parquet, dgl / pyG graph
+        ![RecDP v2.0 Overview](resources/recdp_intro.png)
+        
+        ## This solution is intended for
+        citizen data scientists, enterprise users, independent software vendor and partial of cloud service provider.
+        
+        # Getting Start
+        ## setup with pip
+        ```
+        git clone --single-branch --branch RecDP_v2.0 https://github.com/intel-innersource/frameworks.bigdata.AIDK.git
+        cd frameworks.bigdata.AIDK/RecDP
+        # install dependencies
+        apt-get update -y &&  DEBIAN_FRONTEND=noninteractive apt-get install -y python3 python3-pip python-is-python3 graphviz
+        DEBIAN_FRONTEND=noninteractive apt-get install -y openjdk-8-jre
+        # install recdp
+        python setup.py sdist
+        pip install dist/pyrecdp-1.0.1.tar.gz
+        
+        sh start-jupyter.sh
+        # open browser with http://hostname:8888
+        ```
+        
+        ## run
+        ![nyc taxi demo](https://github.com/intel-innersource/frameworks.bigdata.AIDK/assets/4355494/03d8c2fe-de47-41f9-9fef-8513bc4aaf42)
+        
+        ## modify pipeline (add user defined function or remove operation)
+        ``` python
+        def filter_with_cond(df):
+            df = df[df['Year'] <= 2018]
+            return df
+        operation = {
+            "children": [6], # will to append this new op
+            "next": [7], # who will be connected to this new op
+            "inline_function": filter_with_cond, # function
+        }
+        pipeline.add_operation(operation)
+        ```
+        ``` python
+        operation = {
+            "idx": 6, # OP id to be deleted
+            "next": [10] # who is connected to the to_be_deleted op
+        }
+        pipeline.delete_operation(operation)
+        ```
+        
+        ## export pipeline
+        ``` python
+        pipeline.export(file_path = "exported_pipeline.json")
+        ```
+        ``` json
+        {
+            "0": {
+                "children": null,
+                "op": "DataFrame",
+                "config": "main_table"
+            },
+            "1": {
+                "children": [0],
+                "op": "type_infer",
+                "config": [
+                    ["pickup_datetime",["is_string","is_datetime"]],
+                    ["pickup_longitude",["is_numeric","is_float"]],
+                    ["pickup_latitude",["is_numeric","is_float"]],
+                    ["dropoff_longitude",["is_numeric","is_float"]],
+                    ["dropoff_latitude",["is_numeric","is_float"]],
+                    ["passenger_count",["is_numeric","is_int64","is_integer","is_categorical"]]
+                ]
+            },
+            "2": {
+                "children": [1],
+                "op": "tuple",
+                "config": {
+                    "src": ["pickup_latitude","pickup_longitude"],"dst": "pickup_coordinates"
+                }
+            },
+            "3": {
+                "children": [2],
+                "op": "tuple",
+                "config": {
+                    "src": ["dropoff_latitude","dropoff_longitude"],"dst": "dropoff_coordinates"
+                }
+            },
+            "4": {
+                "children": [3],
+                "op": "fillna",
+                "config": {
+                    "pickup_longitude": -1,
+                    "pickup_latitude": -1,
+                    "dropoff_longitude": -1,
+                    "dropoff_latitude": -1,
+                    "passenger_count": -1
+                }
+            },
+            "5": {
+                "children": [4],
+                "op": "datetime_feature",
+                "config": {
+                    "pickup_datetime": [
+                        ["pickup_datetime__day",["featuretools.primitives.standard.transform.datetime.day", "Day"]],
+                        ["pickup_datetime__month",["featuretools.primitives.standard.transform.datetime.month","Month"]],
+                        ["pickup_datetime__weekday",["featuretools.primitives.standard.transform.datetime.weekday","Weekday"]],
+                        ["pickup_datetime__year",["featuretools.primitives.standard.transform.datetime.year","Year"]],
+                        ["pickup_datetime__hour",["featuretools.primitives.standard.transform.datetime.hour","Hour"]]
+                    ]
+                }
+            },
+            "6": {
+                "children": [5],
+                "op": "haversine",
+                "config": {
+                    "['pickup_coordinates', 'dropoff_coordinates']": ["haversine_pickup_coordinates_dropoff_coordinates",["featuretools.primitives.standard.transform.latlong.haversine","Haversine"]]
+                }
+            },
+            "7": {
+                "children": [6],
+                "op": "drop",
+                "config": [
+                    "pickup_datetime",
+                    "pickup_coordinates",
+                    "dropoff_coordinates"
+                ]
+            },
+            "8": {
+                "children": [7],
+                "op": "lightgbm",
+                "config": {
+                    "label": "fare_amount",
+                    "metrics": "rmse",
+                    "objective": "regression",
+                    "model_file": "lightgbm_regression_label.mdl",
+                    "method": "predict"
+                }
+            }
+        }
+        ```
+        
+        
+        ## Quick Example
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/de044d606e6cdc44d3005db2a0ae968d/recdp_fare_prediction.ipynb) - [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_train.ipynb) - geographic, datetime, lgbm regression
+        
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2b8acb3eda73028635072352560139ba/recdp_fraud_detect.ipynb) - [IBM Card Transaction Fraud Detect](examples/notebooks/autofe/demo/fraud_detect_train.ipynb) - onehot encode, lgbm, binary classification 
+        
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/b039b8c0a40fec951b1b09c3fbb93a7b/recdp_social_media.ipynb) - [twitter recsys](examples/notebooks/autofe/demo/twitter_workflow_test.ipynb) - text nlp, datetime feature engineering  
+        
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/1e08668ab0e15e1e98c592f284d79dad/recdp_click_through_rate_multiple_tables.ipynb) - [outbrain](examples/notebooks/autofe/demo/outbrain_ctr_workflow_test.ipynb) - multiple table joining
+        
+        * [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2f942c30dbf9b63a64cc819a61966e34/recdp_rating_prediction_amazon_review.ipynb) - [amazon product review](examples/notebooks/autofe/demo/amazon_product_review_test.ipynb) - text nlp, datetime, feature-cross
+        
+        # More Examples - completed example including training
+        
+        ## Auto Feature Engineering vs. featuretools
+        * [NYC Taxi fare auto data prepration](examples/notebooks/autofe/FeatureWrangler.ipynb): An example to show how RecDP_v2.0 automatically generating datetime and geo features upon 55M records. Tested with both Spark and Pandas(featuretools) as compute engine, show 21x speedup by spark.
+        
+        ## load PIPELINE and execute
+        * [twitter pipeline re-load and execute](examples/notebooks/autofe/demo/custom_pipeline_twitter.ipynb): An example to show how RecDP_v2.0 reload pipeline from json and do execution - use RecDP as compute engine.
+        
+        ## Realtime Inference pipeline
+        * [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_predict.ipynb) - geographic, datetime feature engineering, lgbm
+        
+        ## Data Profiler Examples
+        * [NYC Taxi fare Profiler](resources/FeatureProfiler_NYC.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
+        
+        * [twitter Profiler](resources/FeatureProfiler_recsys.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
+        
+        
+        ## LICENSE
+        * Apache 2.0
+        
+        ## Dependency
+        * Spark 3.x
+        * python 3.*
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# RecDP v2.0
-
-# INTRODUCTION
-
-## Problem Statement
-
-Data Preparation is an essential step to build AI pipelines 
-* key data preparation capabilities: data connector, cleaning, sampling, joining, profiling, feature engineering, low-code/no-code UI, lineage etc. 
-* exploration of optimal Data preparation consumes majority of Data Science time
-
-## Solution with RecDP v2.0
-
-* Auto pipeline
-    * only 3 lines of codes required
-* Pipeline Generator
-    * Data Profiling:
-        * Auto anomalies detection
-        * Auto missing value impute
-        * Profiling Visualizzation        
-    * Feature Wrangling:
-        * feature transformation(datetime, geo_info, text_nlp, url, etc.)
-        * multiple data auto joining
-        * feature cross(aggregation transformation - sum, avg, count, etc.)
-    * export pipeline as JSON file, can be import to other data platform
-* Pipeline Runner:
-    * spark engine: convert pipeline to spark codes to run
-    * pandas engine: convert pipeline to pandas codes to run
-    * sql engine: convert pipeline to sql
-* DataLoader:
-    * parquet, csv, json, database
-* FeatureWriter - ML/DL connector:
-    * Data Lineage
-    * Feature Store
-    * numpy, csv, parquet, dgl / pyG graph
-![RecDP v2.0 Overview](resources/recdp_intro.png)
-
-## This solution is intended for
-citizen data scientists, enterprise users, independent software vendor and partial of cloud service provider.
-
-# Getting Start
-## setup with pip
-```
-git clone --single-branch --branch RecDP_v2.0 https://github.com/intel-innersource/frameworks.bigdata.AIDK.git
-cd frameworks.bigdata.AIDK/RecDP
-# install dependencies
-apt-get update -y &&  DEBIAN_FRONTEND=noninteractive apt-get install -y python3 python3-pip python-is-python3 graphviz
-DEBIAN_FRONTEND=noninteractive apt-get install -y openjdk-8-jre
-# install recdp
-python setup.py sdist
-pip install dist/pyrecdp-1.0.1.tar.gz
-
-sh start-jupyter.sh
-# open browser with http://hostname:8888
-```
-
-## run
-![nyc taxi demo](https://github.com/intel-innersource/frameworks.bigdata.AIDK/assets/4355494/03d8c2fe-de47-41f9-9fef-8513bc4aaf42)
-
-## modify pipeline (add user defined function or remove operation)
-``` python
-def filter_with_cond(df):
-    df = df[df['Year'] <= 2018]
-    return df
-operation = {
-    "children": [6], # will to append this new op
-    "next": [7], # who will be connected to this new op
-    "inline_function": filter_with_cond, # function
-}
-pipeline.add_operation(operation)
-```
-``` python
-operation = {
-    "idx": 6, # OP id to be deleted
-    "next": [10] # who is connected to the to_be_deleted op
-}
-pipeline.delete_operation(operation)
-```
-
-## export pipeline
-``` python
-pipeline.export(file_path = "exported_pipeline.json")
-```
-``` json
-{
-    "0": {
-        "children": null,
-        "op": "DataFrame",
-        "config": "main_table"
-    },
-    "1": {
-        "children": [0],
-        "op": "type_infer",
-        "config": [
-            ["pickup_datetime",["is_string","is_datetime"]],
-            ["pickup_longitude",["is_numeric","is_float"]],
-            ["pickup_latitude",["is_numeric","is_float"]],
-            ["dropoff_longitude",["is_numeric","is_float"]],
-            ["dropoff_latitude",["is_numeric","is_float"]],
-            ["passenger_count",["is_numeric","is_int64","is_integer","is_categorical"]]
-        ]
-    },
-    "2": {
-        "children": [1],
-        "op": "tuple",
-        "config": {
-            "src": ["pickup_latitude","pickup_longitude"],"dst": "pickup_coordinates"
-        }
-    },
-    "3": {
-        "children": [2],
-        "op": "tuple",
-        "config": {
-            "src": ["dropoff_latitude","dropoff_longitude"],"dst": "dropoff_coordinates"
-        }
-    },
-    "4": {
-        "children": [3],
-        "op": "fillna",
-        "config": {
-            "pickup_longitude": -1,
-            "pickup_latitude": -1,
-            "dropoff_longitude": -1,
-            "dropoff_latitude": -1,
-            "passenger_count": -1
-        }
-    },
-    "5": {
-        "children": [4],
-        "op": "datetime_feature",
-        "config": {
-            "pickup_datetime": [
-                ["pickup_datetime__day",["featuretools.primitives.standard.transform.datetime.day", "Day"]],
-                ["pickup_datetime__month",["featuretools.primitives.standard.transform.datetime.month","Month"]],
-                ["pickup_datetime__weekday",["featuretools.primitives.standard.transform.datetime.weekday","Weekday"]],
-                ["pickup_datetime__year",["featuretools.primitives.standard.transform.datetime.year","Year"]],
-                ["pickup_datetime__hour",["featuretools.primitives.standard.transform.datetime.hour","Hour"]]
-            ]
-        }
-    },
-    "6": {
-        "children": [5],
-        "op": "haversine",
-        "config": {
-            "['pickup_coordinates', 'dropoff_coordinates']": ["haversine_pickup_coordinates_dropoff_coordinates",["featuretools.primitives.standard.transform.latlong.haversine","Haversine"]]
-        }
-    },
-    "7": {
-        "children": [6],
-        "op": "drop",
-        "config": [
-            "pickup_datetime",
-            "pickup_coordinates",
-            "dropoff_coordinates"
-        ]
-    },
-    "8": {
-        "children": [7],
-        "op": "lightgbm",
-        "config": {
-            "label": "fare_amount",
-            "metrics": "rmse",
-            "objective": "regression",
-            "model_file": "lightgbm_regression_label.mdl",
-            "method": "predict"
-        }
-    }
-}
-```
-
-
-## Quick Example
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/de044d606e6cdc44d3005db2a0ae968d/recdp_fare_prediction.ipynb) - [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_train.ipynb) - geographic, datetime, lgbm regression
-
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2b8acb3eda73028635072352560139ba/recdp_fraud_detect.ipynb) - [IBM Card Transaction Fraud Detect](examples/notebooks/autofe/demo/fraud_detect_train.ipynb) - onehot encode, lgbm, binary classification 
-
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/b039b8c0a40fec951b1b09c3fbb93a7b/recdp_social_media.ipynb) - [twitter recsys](examples/notebooks/autofe/demo/twitter_workflow_test.ipynb) - text nlp, datetime feature engineering  
-
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/1e08668ab0e15e1e98c592f284d79dad/recdp_click_through_rate_multiple_tables.ipynb) - [outbrain](examples/notebooks/autofe/demo/outbrain_ctr_workflow_test.ipynb) - multiple table joining
-
-* [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/xuechendi/2f942c30dbf9b63a64cc819a61966e34/recdp_rating_prediction_amazon_review.ipynb) - [amazon product review](examples/notebooks/autofe/demo/amazon_product_review_test.ipynb) - text nlp, datetime, feature-cross
-
-# More Examples - completed example including training
-
-## Auto Feature Engineering vs. featuretools
-* [NYC Taxi fare auto data prepration](examples/notebooks/autofe/FeatureWrangler.ipynb): An example to show how RecDP_v2.0 automatically generating datetime and geo features upon 55M records. Tested with both Spark and Pandas(featuretools) as compute engine, show 21x speedup by spark.
-
-## load PIPELINE and execute
-* [twitter pipeline re-load and execute](examples/notebooks/autofe/demo/custom_pipeline_twitter.ipynb): An example to show how RecDP_v2.0 reload pipeline from json and do execution - use RecDP as compute engine.
-
-## Realtime Inference pipeline
-* [nyc taxi fare](examples/notebooks/autofe/demo/nyc_taxi_workflow_predict.ipynb) - geographic, datetime feature engineering, lgbm
-
-## Data Profiler Examples
-* [NYC Taxi fare Profiler](resources/FeatureProfiler_NYC.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
-
-* [twitter Profiler](resources/FeatureProfiler_recsys.png): An example to show RecDP_v2.0 to profile data, including infer the potential data type, generate data distribution charts.
-
-
-## LICENSE
-* Apache 2.0
-
-## Dependency
-* Spark 3.x
-* python 3.*
-
-
```

### Comparing `pyrecdp-1.0.1b202306061/pyrecdp.egg-info/SOURCES.txt` & `pyrecdp-1.0.1b2023062716/pyrecdp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-LICENSE
 MANIFEST.in
 README.md
-pyproject.toml
 setup.py
 ScalaProcessUtils/__init__.py
 pyrecdp/__init__.py
 pyrecdp.egg-info/PKG-INFO
 pyrecdp.egg-info/SOURCES.txt
 pyrecdp.egg-info/dependency_links.txt
 pyrecdp.egg-info/not-zip-safe
```

### Comparing `pyrecdp-1.0.1b202306061/setup.py` & `pyrecdp-1.0.1b2023062716/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import setuptools
 from setuptools import find_packages
 from setuptools.command.install import install
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
-    
+
+with open("version", "r") as fh:
+    VERSION = fh.read().strip()
+
 setuptools.setup(
     name="pyrecdp",
-    version="1.0.1b202306061",
+    version=VERSION,
     author="INTEL AIA",
     description=
     "A data processing bundle for spark based recommender system operations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = "https://github.com/intel/e2eAIOK/",
     project_urls={
```

