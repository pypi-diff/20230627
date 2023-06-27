# Comparing `tmp/ml4h-0.0.5.tar.gz` & `tmp/ml4h-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml4h-0.0.5.tar", last modified: Mon Apr 10 17:29:18 2023, max compression
+gzip compressed data, was "ml4h-0.0.6.tar", last modified: Tue Jun 27 18:16:55 2023, max compression
```

## Comparing `ml4h-0.0.5.tar` & `ml4h-0.0.6.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.450923 ml4h-0.0.5/
--rw-r--r--   0 sam        (503) staff       (20)     1633 2023-01-26 10:40:07.000000 ml4h-0.0.5/LICENSE.txt
--rw-r--r--   0 sam        (503) staff       (20)     4491 2023-01-26 10:40:07.000000 ml4h-0.0.5/NOTICE.txt
--rw-r--r--   0 sam        (503) staff       (20)     6857 2023-04-10 17:29:18.450007 ml4h-0.0.5/PKG-INFO
--rw-r--r--   0 sam        (503) staff       (20)     6592 2023-03-08 12:42:24.000000 ml4h-0.0.5/README.md
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.360829 ml4h-0.0.5/ml4h/
--rw-r--r--   0 sam        (503) staff       (20)     2361 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/DatabaseClient.py
--rwxr-xr-x   0 sam        (503) staff       (20)    23803 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/TensorMap.py
--rw-r--r--   0 sam        (503) staff       (20)       22 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/__init__.py
--rw-r--r--   0 sam        (503) staff       (20)    35435 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/arguments.py
--rwxr-xr-x   0 sam        (503) staff       (20)     9464 2023-03-08 12:42:24.000000 ml4h-0.0.5/ml4h/defines.py
--rw-r--r--   0 sam        (503) staff       (20)    55869 2023-03-08 12:42:24.000000 ml4h-0.0.5/ml4h/explorations.py
--rw-r--r--   0 sam        (503) staff       (20)     7604 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/hypertuning.py
--rw-r--r--   0 sam        (503) staff       (20)     1846 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/logger.py
--rw-r--r--   0 sam        (503) staff       (20)     6325 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/make_tensor_maps_for_partners_ecg_labels.py
--rwxr-xr-x   0 sam        (503) staff       (20)    27628 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/metrics.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.370658 ml4h-0.0.5/ml4h/ml4ht_integration/
--rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/ml4ht_integration/__init__.py
--rw-r--r--   0 sam        (503) staff       (20)     4264 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/ml4ht_integration/tensor_generator.py
--rw-r--r--   0 sam        (503) staff       (20)     5358 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/ml4ht_integration/tensor_map.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.388059 ml4h-0.0.5/ml4h/models/
--rw-r--r--   0 sam        (503) staff       (20)      422 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/Block.py
--rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/__init__.py
--rw-r--r--   0 sam        (503) staff       (20)     7921 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/basic_blocks.py
--rw-r--r--   0 sam        (503) staff       (20)    23869 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/conv_blocks.py
--rw-r--r--   0 sam        (503) staff       (20)     6020 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/inspect.py
--rw-r--r--   0 sam        (503) staff       (20)     6368 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/layer_wrappers.py
--rwxr-xr-x   0 sam        (503) staff       (20)    67636 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/legacy_models.py
--rw-r--r--   0 sam        (503) staff       (20)    13249 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/merge_blocks.py
--rw-r--r--   0 sam        (503) staff       (20)    18364 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/model_factory.py
--rw-r--r--   0 sam        (503) staff       (20)     3642 2023-03-08 12:42:24.000000 ml4h-0.0.5/ml4h/models/pretrained_blocks.py
--rw-r--r--   0 sam        (503) staff       (20)     4144 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/train.py
--rw-r--r--   0 sam        (503) staff       (20)    14384 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/models/transformer_blocks.py
--rw-r--r--   0 sam        (503) staff       (20)     2848 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/normalizer.py
--rw-r--r--   0 sam        (503) staff       (20)     4238 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/optimizers.py
--rw-r--r--   0 sam        (503) staff       (20)   128766 2023-03-26 13:50:21.000000 ml4h-0.0.5/ml4h/plots.py
--rwxr-xr-x   0 sam        (503) staff       (20)    49510 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/recipes.py
--rw-r--r--   0 sam        (503) staff       (20)     5424 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/runtime_data_defines.py
--rwxr-xr-x   0 sam        (503) staff       (20)    40052 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensor_generators.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.393913 ml4h-0.0.5/ml4h/tensorize/
--rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensorize/__init__.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.395345 ml4h-0.0.5/ml4h/tensorize/dataflow/
--rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensorize/dataflow/__init__.py
--rw-r--r--   0 sam        (503) staff       (20)     7724 2023-03-08 12:42:24.000000 ml4h-0.0.5/ml4h/tensorize/dataflow/bigquery_ukb_queries.py
--rw-r--r--   0 sam        (503) staff       (20)     4257 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensorize/merge_hd5s.py
--rw-r--r--   0 sam        (503) staff       (20)    18759 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensorize/tensor_writer_mgb.py
--rw-r--r--   0 sam        (503) staff       (20)    61752 2023-03-25 15:36:49.000000 ml4h-0.0.5/ml4h/tensorize/tensor_writer_ukbb.py
--rw-r--r--   0 sam        (503) staff       (20)     3243 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensorize/tensorize_dataflow.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.402847 ml4h-0.0.5/ml4h/tensormap/
--rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/__init__.py
--rw-r--r--   0 sam        (503) staff       (20)     8657 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/celeba.py
--rw-r--r--   0 sam        (503) staff       (20)     2152 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/gatk.py
--rw-r--r--   0 sam        (503) staff       (20)     6283 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/general.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.406297 ml4h-0.0.5/ml4h/tensormap/mgb/
--rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/mgb/__init__.py
--rw-r--r--   0 sam        (503) staff       (20)    47783 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/mgb/dynamic.py
--rw-r--r--   0 sam        (503) staff       (20)    73630 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/mgb/ecg.py
--rw-r--r--   0 sam        (503) staff       (20)     4035 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/mnist.py
--rw-r--r--   0 sam        (503) staff       (20)    14184 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/tensor_map_maker.py
--rw-r--r--   0 sam        (503) staff       (20)     4154 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/text.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.437716 ml4h-0.0.5/ml4h/tensormap/ukb/
--rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/ukb/__init__.py
--rw-r--r--   0 sam        (503) staff       (20)   250867 2023-03-08 12:42:24.000000 ml4h-0.0.5/ml4h/tensormap/ukb/categorical.py
--rw-r--r--   0 sam        (503) staff       (20)   542886 2023-03-08 12:42:24.000000 ml4h-0.0.5/ml4h/tensormap/ukb/continuous.py
--rw-r--r--   0 sam        (503) staff       (20)    42508 2023-04-04 16:37:17.000000 ml4h-0.0.5/ml4h/tensormap/ukb/demographics.py
--rw-r--r--   0 sam        (503) staff       (20)   101606 2023-04-10 14:42:05.000000 ml4h-0.0.5/ml4h/tensormap/ukb/disease.py
--rw-r--r--   0 sam        (503) staff       (20)     4465 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/ukb/dxa.py
--rw-r--r--   0 sam        (503) staff       (20)    61466 2023-03-26 15:24:00.000000 ml4h-0.0.5/ml4h/tensormap/ukb/ecg.py
--rw-r--r--   0 sam        (503) staff       (20)    34805 2023-03-08 12:42:24.000000 ml4h-0.0.5/ml4h/tensormap/ukb/genetics.py
--rw-r--r--   0 sam        (503) staff       (20)   126679 2023-04-06 19:41:39.000000 ml4h-0.0.5/ml4h/tensormap/ukb/mri.py
--rw-r--r--   0 sam        (503) staff       (20)    12774 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/ukb/mri_brain.py
--rw-r--r--   0 sam        (503) staff       (20)     6557 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/ukb/mri_ecg.py
--rw-r--r--   0 sam        (503) staff       (20)    11925 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/tensormap/ukb/mri_vtk.py
--rw-r--r--   0 sam        (503) staff       (20)    14549 2023-03-20 19:08:05.000000 ml4h-0.0.5/ml4h/tensormap/ukb/survival.py
--rw-r--r--   0 sam        (503) staff       (20)     3316 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/test_utils.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.448454 ml4h-0.0.5/ml4h/visualization_tools/
--rw-r--r--   0 sam        (503) staff       (20)        0 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/__init__.py
--rw-r--r--   0 sam        (503) staff       (20)     7219 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/annotation_storage.py
--rw-r--r--   0 sam        (503) staff       (20)     5764 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/annotations.py
--rw-r--r--   0 sam        (503) staff       (20)    10397 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/batch_image_annotations.py
--rw-r--r--   0 sam        (503) staff       (20)    10420 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/dicom_interactive_plots.py
--rw-r--r--   0 sam        (503) staff       (20)    15258 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/dicom_plots.py
--rw-r--r--   0 sam        (503) staff       (20)     6203 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/ecg_interactive_plots.py
--rw-r--r--   0 sam        (503) staff       (20)     9855 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/ecg_reshape.py
--rw-r--r--   0 sam        (503) staff       (20)     3106 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/ecg_static_plots.py
--rw-r--r--   0 sam        (503) staff       (20)     3329 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/facets.py
--rw-r--r--   0 sam        (503) staff       (20)    14368 2023-01-26 10:40:08.000000 ml4h-0.0.5/ml4h/visualization_tools/hd5_mri_plots.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-04-10 17:29:18.366153 ml4h-0.0.5/ml4h.egg-info/
--rw-r--r--   0 sam        (503) staff       (20)     6857 2023-04-10 17:29:18.000000 ml4h-0.0.5/ml4h.egg-info/PKG-INFO
--rw-r--r--   0 sam        (503) staff       (20)     2372 2023-04-10 17:29:18.000000 ml4h-0.0.5/ml4h.egg-info/SOURCES.txt
--rw-r--r--   0 sam        (503) staff       (20)        1 2023-04-10 17:29:18.000000 ml4h-0.0.5/ml4h.egg-info/dependency_links.txt
--rw-r--r--   0 sam        (503) staff       (20)      556 2023-04-10 17:29:18.000000 ml4h-0.0.5/ml4h.egg-info/requires.txt
--rw-r--r--   0 sam        (503) staff       (20)        5 2023-04-10 17:29:18.000000 ml4h-0.0.5/ml4h.egg-info/top_level.txt
--rw-r--r--   0 sam        (503) staff       (20)       38 2023-04-10 17:29:18.451157 ml4h-0.0.5/setup.cfg
--rw-r--r--   0 sam        (503) staff       (20)      735 2023-04-10 16:51:22.000000 ml4h-0.0.5/setup.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-06-27 18:16:55.610963 ml4h-0.0.6/
+-rw-r--r--   0 sam        (503) staff       (20)     1633 2023-05-09 09:39:59.000000 ml4h-0.0.6/LICENSE.txt
+-rw-r--r--   0 sam        (503) staff       (20)     4491 2023-05-09 09:39:59.000000 ml4h-0.0.6/NOTICE.txt
+-rw-r--r--   0 sam        (503) staff       (20)     6954 2023-06-27 18:16:55.610604 ml4h-0.0.6/PKG-INFO
+-rw-r--r--   0 sam        (503) staff       (20)     6689 2023-05-09 09:39:59.000000 ml4h-0.0.6/README.md
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-06-27 18:16:55.564597 ml4h-0.0.6/ml4h/
+-rw-r--r--   0 sam        (503) staff       (20)     2361 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/DatabaseClient.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    23803 2023-05-09 09:39:59.000000 ml4h-0.0.6/ml4h/TensorMap.py
+-rw-r--r--   0 sam        (503) staff       (20)       22 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/__init__.py
+-rw-r--r--   0 sam        (503) staff       (20)    35435 2023-06-27 18:14:47.000000 ml4h-0.0.6/ml4h/arguments.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     9464 2023-05-09 09:39:59.000000 ml4h-0.0.6/ml4h/defines.py
+-rw-r--r--   0 sam        (503) staff       (20)    65687 2023-06-27 18:14:47.000000 ml4h-0.0.6/ml4h/explorations.py
+-rw-r--r--   0 sam        (503) staff       (20)     7604 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/hypertuning.py
+-rw-r--r--   0 sam        (503) staff       (20)     1846 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/logger.py
+-rw-r--r--   0 sam        (503) staff       (20)     6325 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/make_tensor_maps_for_partners_ecg_labels.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    27628 2023-05-09 09:39:59.000000 ml4h-0.0.6/ml4h/metrics.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-06-27 18:16:55.573347 ml4h-0.0.6/ml4h/ml4ht_integration/
+-rw-r--r--   0 sam        (503) staff       (20)        0 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/ml4ht_integration/__init__.py
+-rw-r--r--   0 sam        (503) staff       (20)     4264 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/ml4ht_integration/tensor_generator.py
+-rw-r--r--   0 sam        (503) staff       (20)     5358 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/ml4ht_integration/tensor_map.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-06-27 18:16:55.584405 ml4h-0.0.6/ml4h/models/
+-rw-r--r--   0 sam        (503) staff       (20)      422 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/models/Block.py
+-rw-r--r--   0 sam        (503) staff       (20)        0 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/models/__init__.py
+-rw-r--r--   0 sam        (503) staff       (20)     7921 2023-06-27 18:14:47.000000 ml4h-0.0.6/ml4h/models/basic_blocks.py
+-rw-r--r--   0 sam        (503) staff       (20)    23869 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/models/conv_blocks.py
+-rw-r--r--   0 sam        (503) staff       (20)     6020 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/models/inspect.py
+-rw-r--r--   0 sam        (503) staff       (20)     6368 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/models/layer_wrappers.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    67636 2023-06-27 18:14:47.000000 ml4h-0.0.6/ml4h/models/legacy_models.py
+-rw-r--r--   0 sam        (503) staff       (20)    13249 2023-06-27 18:14:47.000000 ml4h-0.0.6/ml4h/models/merge_blocks.py
+-rw-r--r--   0 sam        (503) staff       (20)    18364 2023-06-27 18:14:47.000000 ml4h-0.0.6/ml4h/models/model_factory.py
+-rw-r--r--   0 sam        (503) staff       (20)     3642 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/models/pretrained_blocks.py
+-rw-r--r--   0 sam        (503) staff       (20)     4144 2023-06-27 18:14:47.000000 ml4h-0.0.6/ml4h/models/train.py
+-rw-r--r--   0 sam        (503) staff       (20)    14384 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/models/transformer_blocks.py
+-rw-r--r--   0 sam        (503) staff       (20)     2848 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/normalizer.py
+-rw-r--r--   0 sam        (503) staff       (20)     4238 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/optimizers.py
+-rw-r--r--   0 sam        (503) staff       (20)   128766 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/plots.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    49510 2023-05-09 09:39:59.000000 ml4h-0.0.6/ml4h/recipes.py
+-rw-r--r--   0 sam        (503) staff       (20)     5424 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/runtime_data_defines.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    40052 2023-05-09 09:39:59.000000 ml4h-0.0.6/ml4h/tensor_generators.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-06-27 18:16:55.588098 ml4h-0.0.6/ml4h/tensorize/
+-rw-r--r--   0 sam        (503) staff       (20)        0 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensorize/__init__.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-06-27 18:16:55.589600 ml4h-0.0.6/ml4h/tensorize/dataflow/
+-rw-r--r--   0 sam        (503) staff       (20)        0 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensorize/dataflow/__init__.py
+-rw-r--r--   0 sam        (503) staff       (20)     7724 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensorize/dataflow/bigquery_ukb_queries.py
+-rw-r--r--   0 sam        (503) staff       (20)     4257 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensorize/merge_hd5s.py
+-rw-r--r--   0 sam        (503) staff       (20)    18759 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensorize/tensor_writer_mgb.py
+-rw-r--r--   0 sam        (503) staff       (20)    61752 2023-06-27 18:14:47.000000 ml4h-0.0.6/ml4h/tensorize/tensor_writer_ukbb.py
+-rw-r--r--   0 sam        (503) staff       (20)     3243 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensorize/tensorize_dataflow.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-06-27 18:16:55.592705 ml4h-0.0.6/ml4h/tensormap/
+-rw-r--r--   0 sam        (503) staff       (20)        0 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensormap/__init__.py
+-rw-r--r--   0 sam        (503) staff       (20)     8657 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensormap/celeba.py
+-rw-r--r--   0 sam        (503) staff       (20)     2152 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensormap/gatk.py
+-rw-r--r--   0 sam        (503) staff       (20)     6283 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensormap/general.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-06-27 18:16:55.594399 ml4h-0.0.6/ml4h/tensormap/mgb/
+-rw-r--r--   0 sam        (503) staff       (20)        0 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensormap/mgb/__init__.py
+-rw-r--r--   0 sam        (503) staff       (20)    47783 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensormap/mgb/dynamic.py
+-rw-r--r--   0 sam        (503) staff       (20)    73630 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensormap/mgb/ecg.py
+-rw-r--r--   0 sam        (503) staff       (20)     4035 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensormap/mnist.py
+-rw-r--r--   0 sam        (503) staff       (20)    14184 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensormap/tensor_map_maker.py
+-rw-r--r--   0 sam        (503) staff       (20)     4154 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensormap/text.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-06-27 18:16:55.604562 ml4h-0.0.6/ml4h/tensormap/ukb/
+-rw-r--r--   0 sam        (503) staff       (20)        0 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensormap/ukb/__init__.py
+-rw-r--r--   0 sam        (503) staff       (20)   250867 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensormap/ukb/categorical.py
+-rw-r--r--   0 sam        (503) staff       (20)   542886 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensormap/ukb/continuous.py
+-rw-r--r--   0 sam        (503) staff       (20)    42508 2023-06-27 18:14:47.000000 ml4h-0.0.6/ml4h/tensormap/ukb/demographics.py
+-rw-r--r--   0 sam        (503) staff       (20)   101606 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensormap/ukb/disease.py
+-rw-r--r--   0 sam        (503) staff       (20)     4465 2023-06-27 18:14:47.000000 ml4h-0.0.6/ml4h/tensormap/ukb/dxa.py
+-rw-r--r--   0 sam        (503) staff       (20)    61466 2023-06-27 18:14:47.000000 ml4h-0.0.6/ml4h/tensormap/ukb/ecg.py
+-rw-r--r--   0 sam        (503) staff       (20)    34805 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensormap/ukb/genetics.py
+-rw-r--r--   0 sam        (503) staff       (20)   126679 2023-06-27 18:14:47.000000 ml4h-0.0.6/ml4h/tensormap/ukb/mri.py
+-rw-r--r--   0 sam        (503) staff       (20)    12774 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensormap/ukb/mri_brain.py
+-rw-r--r--   0 sam        (503) staff       (20)     6557 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensormap/ukb/mri_ecg.py
+-rw-r--r--   0 sam        (503) staff       (20)    11925 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/tensormap/ukb/mri_vtk.py
+-rw-r--r--   0 sam        (503) staff       (20)    14549 2023-06-27 18:14:47.000000 ml4h-0.0.6/ml4h/tensormap/ukb/survival.py
+-rw-r--r--   0 sam        (503) staff       (20)     3316 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/test_utils.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-06-27 18:16:55.610128 ml4h-0.0.6/ml4h/visualization_tools/
+-rw-r--r--   0 sam        (503) staff       (20)        0 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/visualization_tools/__init__.py
+-rw-r--r--   0 sam        (503) staff       (20)     7219 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/visualization_tools/annotation_storage.py
+-rw-r--r--   0 sam        (503) staff       (20)     5764 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/visualization_tools/annotations.py
+-rw-r--r--   0 sam        (503) staff       (20)    10397 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/visualization_tools/batch_image_annotations.py
+-rw-r--r--   0 sam        (503) staff       (20)    10420 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/visualization_tools/dicom_interactive_plots.py
+-rw-r--r--   0 sam        (503) staff       (20)    15258 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/visualization_tools/dicom_plots.py
+-rw-r--r--   0 sam        (503) staff       (20)     6203 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/visualization_tools/ecg_interactive_plots.py
+-rw-r--r--   0 sam        (503) staff       (20)     9855 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/visualization_tools/ecg_reshape.py
+-rw-r--r--   0 sam        (503) staff       (20)     3106 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/visualization_tools/ecg_static_plots.py
+-rw-r--r--   0 sam        (503) staff       (20)     3329 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/visualization_tools/facets.py
+-rw-r--r--   0 sam        (503) staff       (20)    14368 2023-06-12 11:09:13.000000 ml4h-0.0.6/ml4h/visualization_tools/hd5_mri_plots.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-06-27 18:16:55.567783 ml4h-0.0.6/ml4h.egg-info/
+-rw-r--r--   0 sam        (503) staff       (20)     6954 2023-06-27 18:16:55.000000 ml4h-0.0.6/ml4h.egg-info/PKG-INFO
+-rw-r--r--   0 sam        (503) staff       (20)     2372 2023-06-27 18:16:55.000000 ml4h-0.0.6/ml4h.egg-info/SOURCES.txt
+-rw-r--r--   0 sam        (503) staff       (20)        1 2023-06-27 18:16:55.000000 ml4h-0.0.6/ml4h.egg-info/dependency_links.txt
+-rw-r--r--   0 sam        (503) staff       (20)      556 2023-06-27 18:16:55.000000 ml4h-0.0.6/ml4h.egg-info/requires.txt
+-rw-r--r--   0 sam        (503) staff       (20)        5 2023-06-27 18:16:55.000000 ml4h-0.0.6/ml4h.egg-info/top_level.txt
+-rw-r--r--   0 sam        (503) staff       (20)       38 2023-06-27 18:16:55.611041 ml4h-0.0.6/setup.cfg
+-rw-r--r--   0 sam        (503) staff       (20)      735 2023-06-27 18:15:25.000000 ml4h-0.0.6/setup.py
```

### Comparing `ml4h-0.0.5/LICENSE.txt` & `ml4h-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/NOTICE.txt` & `ml4h-0.0.6/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/PKG-INFO` & `ml4h-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml4h
-Version: 0.0.5
+Version: 0.0.6
 Summary: Machine Learning for Health python package
 Home-page: https://github.com/broadinstitute/ml4h
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
@@ -139,7 +139,10 @@
 	note = {original-date: 2019-04-10}
 }
 ```
 
 ## Command line interface
 The ml4h package is designed to be accessable through the command line using "recipes".
 To get started, please see [RECIPE_EXAMPLES](./RECIPE_EXAMPLES.md).
+
+
+[![DOI](https://zenodo.org/badge/180627543.svg)](https://zenodo.org/badge/latestdoi/180627543)
```

### Comparing `ml4h-0.0.5/README.md` & `ml4h-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -129,7 +129,10 @@
 	note = {original-date: 2019-04-10}
 }
 ```
 
 ## Command line interface
 The ml4h package is designed to be accessable through the command line using "recipes".
 To get started, please see [RECIPE_EXAMPLES](./RECIPE_EXAMPLES.md).
+
+
+[![DOI](https://zenodo.org/badge/180627543.svg)](https://zenodo.org/badge/latestdoi/180627543)
```

### Comparing `ml4h-0.0.5/ml4h/DatabaseClient.py` & `ml4h-0.0.6/ml4h/DatabaseClient.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/TensorMap.py` & `ml4h-0.0.6/ml4h/TensorMap.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/arguments.py` & `ml4h-0.0.6/ml4h/arguments.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/defines.py` & `ml4h-0.0.6/ml4h/defines.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/explorations.py` & `ml4h-0.0.6/ml4h/explorations.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,43 +4,278 @@
 import os
 import csv
 import math
 import copy
 import logging
 import operator
 import datetime
+from scipy import stats
 from functools import reduce
 from itertools import combinations
 from collections import defaultdict, Counter, OrderedDict
 from typing import Dict, List, Tuple, Generator, Optional, DefaultDict
 
 import h5py
 import numpy as np
 import pandas as pd
 import multiprocessing as mp
 from sklearn.decomposition import PCA
 from tensorflow.keras.models import Model
 
+
 import matplotlib
 matplotlib.use('Agg')  # Need this to write images from the GSA servers.  Order matters:
+import matplotlib.cm as cm
 import matplotlib.pyplot as plt  # First import matplotlib, then use Agg, then import plt
 
 from ml4h.models.legacy_models import legacy_multimodal_multitask_model
 from ml4h.TensorMap import TensorMap, Interpretation, decompress_data
 from ml4h.tensor_generators import TensorGenerator, test_train_valid_tensor_generators
 from ml4h.tensor_generators import BATCH_INPUT_INDEX, BATCH_OUTPUT_INDEX, BATCH_PATHS_INDEX
 from ml4h.plots import plot_histograms_in_pdf, plot_heatmap, plot_cross_reference, SUBPLOT_SIZE
 from ml4h.plots import evaluate_predictions, subplot_rocs, subplot_scatters, plot_categorical_tmap_over_time
 from ml4h.defines import JOIN_CHAR, MRI_SEGMENTED_CHANNEL_MAP, CODING_VALUES_MISSING, CODING_VALUES_LESS_THAN_ONE
 from ml4h.defines import TENSOR_EXT, IMAGE_EXT, ECG_CHAR_2_IDX, ECG_IDX_2_CHAR, PARTNERS_CHAR_2_IDX, PARTNERS_IDX_2_CHAR, PARTNERS_READ_TEXT
 
+from sklearn.pipeline import make_pipeline
+from sklearn.preprocessing import StandardScaler
+from sklearn.linear_model import LogisticRegression, LinearRegression, ElasticNet, Ridge, Lasso
+
 
 CSV_EXT = '.tsv'
 
 
+def stratify_and_project_latent_space(stratify_column: str,stratify_thresh: float,stratify_std: float,latent_cols: List[str],
+                                    latent_df: pd.DataFrame,
+                                    normalize: bool = False,
+                                    train_ratio: int = 1.0):
+    """
+    Stratify data and project it to new latent space.
+    Args:
+        stratify_column (str): Name of the column used for stratification.
+        stratify_thresh (float): Threshold value for stratification.
+        stratify_std (float): Standard deviation value for stratification.
+        latent_cols (List[str]): List of column names for the latent space.
+        latent_df (pd.DataFrame): DataFrame containing the latent space data.
+        normalize (bool): Flag indicating whether to normalize the data. Default is False.
+        train_ratio (int): Ratio of training data to be used. Default is 1.0.
+
+    Returns:
+        Dict[str, Tuple[float,float,float]]
+    """  
+    if train_ratio == 1.0:
+        train = latent_df
+        test = latent_df
+    else:
+        train = latent_df.sample(frac=train_ratio)
+        test = latent_df.drop(train.index)        
+    hit = train.loc[train[stratify_column] >= stratify_thresh+(1*stratify_std)]
+    miss = train.loc[train[stratify_column] < stratify_thresh-(1*stratify_std)]
+    hit_np = hit[latent_cols].to_numpy()
+    miss_np = miss[latent_cols].to_numpy()
+    miss_mean_vector = np.mean(miss_np, axis=0)
+    hit_mean_vector = np.mean(hit_np, axis=0)
+    angle = angle_between(miss_mean_vector, hit_mean_vector)
+        
+    hit_test = test.loc[test[stratify_column] >= stratify_thresh+(1*stratify_std)]
+    miss_test = test.loc[test[stratify_column] < stratify_thresh-(1*stratify_std)]
+    
+    if normalize:
+        phenotype_vector = unit_vector(hit_mean_vector-miss_mean_vector)
+        hit_dots = [np.dot(phenotype_vector, unit_vector(v)) for v in hit_test[latent_cols].to_numpy()]
+        miss_dots = [np.dot(phenotype_vector, unit_vector(v)) for v in miss_test[latent_cols].to_numpy()]
+    else:
+        phenotype_vector = hit_mean_vector-miss_mean_vector
+        hit_dots = [np.dot(phenotype_vector, v) for v in hit_test[latent_cols].to_numpy()]
+        miss_dots = [np.dot(phenotype_vector, v) for v in miss_test[latent_cols].to_numpy()]
+    t2, p2 = stats.ttest_ind(hit_dots, miss_dots, equal_var = False)
+    
+    return {f'{stratify_column}': (t2, p2, len(hit)) }
+
+
+
+def plot_nested_dictionary(all_scores: DefaultDict[str, DefaultDict[str, Tuple[float,float,float]]]) -> None:
+    """
+    Function to create a plot displaying T-statistics v/s Negative Log P-Value for each covariate.
+    Args:
+        all_scores (DefaultDict[str, DefaultDict[str, Tuple[float, float, float]]]): Nested dictionary containing the scores.
+    Returns:
+        None
+     """  
+    n = 4
+    eps = 1e-300
+    for model in all_scores:
+        n = max(n, len(all_scores[model]))
+    cols = max(2, int(math.ceil(math.sqrt(n))))
+    rows = max(2, int(math.ceil(n / cols)))
+    fig, axes = plt.subplots(rows, cols, figsize=(cols * 4, rows * 3), sharex=True, dpi=300)
+    renest = defaultdict(dict)
+    errors = defaultdict(dict)
+    lens = {}
+    max_tstat = 0
+    max_pval = 0
+    for model in all_scores:
+        for metric in all_scores[model]:
+            renest[metric][model] = all_scores[model][metric][0]
+            errors[metric][model] = all_scores[model][metric][1]
+            lens[metric] = all_scores[model][metric][2]
+            max_tstat = max(abs(all_scores[model][metric][0]), max_tstat)
+            max_pval = max(-np.log10(all_scores[model][metric][1]+eps), max_pval)
+    for metric, ax in zip(renest, axes.ravel()):
+
+        models = [k for k,v in sorted(renest[metric].items(), key=lambda x: x[0].lower())]
+        tstats = [abs(v) for k,v in sorted(renest[metric].items(), key=lambda x: x[0].lower())]
+        pvalues = [-np.log10(v) if v > 1e-4800 else 500 for k,v in sorted(errors[metric].items(), key=lambda x: x[0].lower())]
+        y_pos = np.arange(len(models))
+        x = np.linspace(0, 1, int(max_pval))
+        plt.imshow(x[:, np.newaxis], cmap=cm.jet)
+        cb = plt.colorbar(ax=ax, ticks=[0, 1.0])
+        cb.set_label('Negative Log P-Value')
+        cb.ax.set_yticklabels(['0', f'{max_pval:0.0f}'])
+        ax.barh(y_pos, tstats, color=[cm.jet(p/max_pval) for p in pvalues], align='center')
+        ax.set_yticks(y_pos)
+        ax.set_yticklabels(models)
+        ax.invert_yaxis()  # labels read top-to-bottom
+        ax.set_xlabel('T–Statistic')
+        ax.xaxis.set_tick_params(which='both', labelbottom=True)
+        ax.set_title(f'{metric}\n n={lens[metric]}')
+
+    plt.tight_layout()
+
+
+
+def angle_between(v1: np.ndarray, v2 : np.ndarray):
+    """ Returns the angle in radians between vectors 'v1' and 'v2'::
+            angle_between((1, 0, 0), (0, 1, 0))
+            90
+            angle_between((1, 0, 0), (1, 0, 0))
+            0.0
+            angle_between((1, 0, 0), (-1, 0, 0))
+            180
+    """
+    v1_u = unit_vector(v1)
+    v2_u = unit_vector(v2)
+    return np.arccos(np.clip(np.dot(v1_u, v2_u), -1.0, 1.0)) * 180 / 3.141592
+
+
+def unit_vector(vector : np.ndarray):
+    """ Returns the unit vector of the vector.  """
+    return vector / np.linalg.norm(vector)
+
+
+def latent_space_dataframe(infer_hidden_tsv: str, explore_csv: str):
+    """
+    Read raw data from a CSV file and generate a representation of the data in a latent space.
+
+    Args:
+        infer_hidden_tsv (str): Path to the TSV file containing the inferred hidden representations.
+        explore_csv (str): Path to the CSV file containing the data to be explored.
+
+    Returns:
+        pandas.DataFrame: Dataframe representing the data in the latent space.
+
+    """
+    df = pd.read_csv(explore_csv)
+    df['sample_id'] = pd.to_numeric(df['fpath'], errors='coerce')
+    df2 = pd.read_csv(infer_hidden_tsv, sep='\t', engine='python')
+    df2['sample_id'] = pd.to_numeric(df2['sample_id'], errors='coerce')
+    latent_df = pd.merge(df, df2, on='sample_id', how='inner')
+    return latent_df
+
+
+def confounder_vector(labels: pd.Series, space: np.ndarray):
+    """
+    Compute the confounder vector based on labels and latent space.
+
+    Args:
+        labels (numpy.ndarray or list): The labels representing the dependent variable.
+        space (numpy.ndarray or list): The latent space representing the independent variable.
+
+    Returns:
+        cv and r2
+
+    """
+    clf = make_pipeline(StandardScaler(with_mean=True), Ridge(solver='lsqr'))
+    clf.fit(space, labels)
+    train_score = clf.score(space, labels)
+    return clf[-1].coef_/clf[0].scale_, train_score
+
+
+def confounder_matrix(adjust_cols: List[str], df: pd.DataFrame, space: np.ndarray):
+    """
+    Compute the confounder matrix based on specified columns, a dataframe, and a latent space.
+
+    Args:
+        adjust_cols (list): List of column names to adjust for as confounders.
+        df (pandas.DataFrame): The dataframe containing the data.
+        space (numpy.ndarray): The latent space representing the independent variable.
+
+    Returns:
+        computed confounder matrix and scores.
+
+    """
+    vectors = []
+    scores = {}
+    for col in adjust_cols:
+        cv, r2 = confounder_vector(df[col], space)
+        scores[col] = r2
+        vectors.append(cv)
+    return np.array(vectors), scores
+
+def iterative_subspace_removal(adjust_cols: List[str], latent_df: pd.DataFrame, latent_cols: List[str],
+                               r2_thresh: float = 0.01, fit_pca: bool = False):
+    """
+    Perform iterative subspace removal based on specified columns, a latent dataframe, 
+    and other parameters to remove confounder variables.
+
+    Args:
+        adjust_cols (List[str]): List of column names to adjust for as confounders.
+        latent_df (pd.DataFrame): The dataframe containing the latent data.
+        latent_cols (List[str]): List of column names representing the latent variables.
+        r2_thresh (float, optional): The threshold for the coefficient of determination (R-squared).
+            Default is 0.01.
+        fit_pca (bool, optional): Whether to fit Principal Component Analysis (PCA) on the latent data.
+            Default is False.
+
+    Returns:
+        pd.DataFrame: The latent dataframe after performing iterative subspace removal.
+        List: List of new columns
+
+    """
+    new_cols = latent_cols
+    new_adjust_cols = adjust_cols
+    space = latent_df[latent_cols].to_numpy()
+
+    if fit_pca:
+        pca = PCA()
+        pca.fit(space)
+        space = pca.transform(space)
+
+    iteration = 0
+    while len(new_adjust_cols) > 0 and space.shape[-1] > len(new_adjust_cols):
+        cfm, scores = confounder_matrix(new_adjust_cols, latent_df, space)
+        u, s, vt = np.linalg.svd(cfm, full_matrices=True)
+        nspace = np.matmul(space, vt[:, len(new_adjust_cols):])
+        new_cols=[f'new_latent_{iteration}_{i}' for i in range(nspace.shape[-1])]
+        df2 = pd.DataFrame(nspace, columns=new_cols, index=latent_df.index)
+        latent_df = pd.concat([latent_df, df2], axis=1)
+
+        iteration += 1
+        space = nspace
+
+        new_adjust_cols = [col for col, score in scores.items() if score > r2_thresh]
+        keep_cols = new_cols + [c for c in latent_df.columns if 'latent' not in c]
+        latent_df = latent_df[keep_cols]
+        r_scores= {k:round(v,4) for k,v in scores.items()}
+        print(f'Scores were {r_scores}, remaining columns are {new_adjust_cols}')
+        print(f'After iteration {iteration} Space shape is: {space.shape}')
+    return new_cols, latent_df
+
+
+
 def predictions_to_pngs(
     predictions: np.ndarray, tensor_maps_in: List[TensorMap], tensor_maps_out: List[TensorMap], data: Dict[str, np.ndarray],
     labels: Dict[str, np.ndarray], paths: List[str], folder: str,
 ) -> None:
     # TODO Remove this command line order dependency
     input_map = tensor_maps_in[0]
     if not os.path.exists(folder):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ml4h-0.0.5/ml4h/hypertuning.py` & `ml4h-0.0.6/ml4h/hypertuning.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/logger.py` & `ml4h-0.0.6/ml4h/logger.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/make_tensor_maps_for_partners_ecg_labels.py` & `ml4h-0.0.6/ml4h/make_tensor_maps_for_partners_ecg_labels.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/metrics.py` & `ml4h-0.0.6/ml4h/metrics.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/ml4ht_integration/tensor_generator.py` & `ml4h-0.0.6/ml4h/ml4ht_integration/tensor_generator.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/ml4ht_integration/tensor_map.py` & `ml4h-0.0.6/ml4h/ml4ht_integration/tensor_map.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/models/basic_blocks.py` & `ml4h-0.0.6/ml4h/models/basic_blocks.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/models/conv_blocks.py` & `ml4h-0.0.6/ml4h/models/conv_blocks.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/models/inspect.py` & `ml4h-0.0.6/ml4h/models/inspect.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/models/layer_wrappers.py` & `ml4h-0.0.6/ml4h/models/layer_wrappers.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/models/legacy_models.py` & `ml4h-0.0.6/ml4h/models/legacy_models.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/models/merge_blocks.py` & `ml4h-0.0.6/ml4h/models/merge_blocks.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/models/model_factory.py` & `ml4h-0.0.6/ml4h/models/model_factory.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/models/pretrained_blocks.py` & `ml4h-0.0.6/ml4h/models/pretrained_blocks.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/models/train.py` & `ml4h-0.0.6/ml4h/models/train.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/models/transformer_blocks.py` & `ml4h-0.0.6/ml4h/models/transformer_blocks.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/normalizer.py` & `ml4h-0.0.6/ml4h/normalizer.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/optimizers.py` & `ml4h-0.0.6/ml4h/optimizers.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/plots.py` & `ml4h-0.0.6/ml4h/plots.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/recipes.py` & `ml4h-0.0.6/ml4h/recipes.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/runtime_data_defines.py` & `ml4h-0.0.6/ml4h/runtime_data_defines.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensor_generators.py` & `ml4h-0.0.6/ml4h/tensor_generators.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensorize/dataflow/bigquery_ukb_queries.py` & `ml4h-0.0.6/ml4h/tensorize/dataflow/bigquery_ukb_queries.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensorize/merge_hd5s.py` & `ml4h-0.0.6/ml4h/tensorize/merge_hd5s.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensorize/tensor_writer_mgb.py` & `ml4h-0.0.6/ml4h/tensorize/tensor_writer_mgb.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensorize/tensor_writer_ukbb.py` & `ml4h-0.0.6/ml4h/tensorize/tensor_writer_ukbb.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensorize/tensorize_dataflow.py` & `ml4h-0.0.6/ml4h/tensorize/tensorize_dataflow.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/celeba.py` & `ml4h-0.0.6/ml4h/tensormap/celeba.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/gatk.py` & `ml4h-0.0.6/ml4h/tensormap/gatk.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/general.py` & `ml4h-0.0.6/ml4h/tensormap/general.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/mgb/dynamic.py` & `ml4h-0.0.6/ml4h/tensormap/mgb/dynamic.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/mgb/ecg.py` & `ml4h-0.0.6/ml4h/tensormap/mgb/ecg.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/mnist.py` & `ml4h-0.0.6/ml4h/tensormap/mnist.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/tensor_map_maker.py` & `ml4h-0.0.6/ml4h/tensormap/tensor_map_maker.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/text.py` & `ml4h-0.0.6/ml4h/tensormap/text.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/ukb/categorical.py` & `ml4h-0.0.6/ml4h/tensormap/ukb/categorical.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/ukb/continuous.py` & `ml4h-0.0.6/ml4h/tensormap/ukb/continuous.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/ukb/demographics.py` & `ml4h-0.0.6/ml4h/tensormap/ukb/demographics.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/ukb/disease.py` & `ml4h-0.0.6/ml4h/tensormap/ukb/disease.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/ukb/dxa.py` & `ml4h-0.0.6/ml4h/tensormap/ukb/dxa.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/ukb/ecg.py` & `ml4h-0.0.6/ml4h/tensormap/ukb/ecg.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/ukb/genetics.py` & `ml4h-0.0.6/ml4h/tensormap/ukb/genetics.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/ukb/mri.py` & `ml4h-0.0.6/ml4h/tensormap/ukb/mri.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/ukb/mri_brain.py` & `ml4h-0.0.6/ml4h/tensormap/ukb/mri_brain.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/ukb/mri_ecg.py` & `ml4h-0.0.6/ml4h/tensormap/ukb/mri_ecg.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/ukb/mri_vtk.py` & `ml4h-0.0.6/ml4h/tensormap/ukb/mri_vtk.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/tensormap/ukb/survival.py` & `ml4h-0.0.6/ml4h/tensormap/ukb/survival.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/test_utils.py` & `ml4h-0.0.6/ml4h/test_utils.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/visualization_tools/annotation_storage.py` & `ml4h-0.0.6/ml4h/visualization_tools/annotation_storage.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/visualization_tools/annotations.py` & `ml4h-0.0.6/ml4h/visualization_tools/annotations.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/visualization_tools/batch_image_annotations.py` & `ml4h-0.0.6/ml4h/visualization_tools/batch_image_annotations.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/visualization_tools/dicom_interactive_plots.py` & `ml4h-0.0.6/ml4h/visualization_tools/dicom_interactive_plots.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/visualization_tools/dicom_plots.py` & `ml4h-0.0.6/ml4h/visualization_tools/dicom_plots.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/visualization_tools/ecg_interactive_plots.py` & `ml4h-0.0.6/ml4h/visualization_tools/ecg_interactive_plots.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/visualization_tools/ecg_reshape.py` & `ml4h-0.0.6/ml4h/visualization_tools/ecg_reshape.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/visualization_tools/ecg_static_plots.py` & `ml4h-0.0.6/ml4h/visualization_tools/ecg_static_plots.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/visualization_tools/facets.py` & `ml4h-0.0.6/ml4h/visualization_tools/facets.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h/visualization_tools/hd5_mri_plots.py` & `ml4h-0.0.6/ml4h/visualization_tools/hd5_mri_plots.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h.egg-info/PKG-INFO` & `ml4h-0.0.6/ml4h.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml4h
-Version: 0.0.5
+Version: 0.0.6
 Summary: Machine Learning for Health python package
 Home-page: https://github.com/broadinstitute/ml4h
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
@@ -139,7 +139,10 @@
 	note = {original-date: 2019-04-10}
 }
 ```
 
 ## Command line interface
 The ml4h package is designed to be accessable through the command line using "recipes".
 To get started, please see [RECIPE_EXAMPLES](./RECIPE_EXAMPLES.md).
+
+
+[![DOI](https://zenodo.org/badge/180627543.svg)](https://zenodo.org/badge/latestdoi/180627543)
```

### Comparing `ml4h-0.0.5/ml4h.egg-info/SOURCES.txt` & `ml4h-0.0.6/ml4h.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/ml4h.egg-info/requires.txt` & `ml4h-0.0.6/ml4h.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.5/setup.py` & `ml4h-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 # Get the requirements from the requirements file
 requirements =  (here / 'docker/vm_boot_images/config/tensorflow-requirements.txt').read_text(encoding='utf-8')
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 setup(
     name='ml4h',
-    version='0.0.5',
+    version='0.0.6',
     description='Machine Learning for Health python package',
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',
     url='https://github.com/broadinstitute/ml4h',
     python_requires='>=3.6',
     install_requires=requirements, #install_requires=["ml4ht", "tensorflow"],
     packages=find_packages(),
```

