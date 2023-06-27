# Comparing `tmp/adaboost_model-0.1.0.tar.gz` & `tmp/adaboost-model-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\adaboost_model-0.1.0.tar", last modified: Sun Nov  8 01:29:08 2020, max compression
+gzip compressed data, was "C:\Users\Lenovo\source\repos\sis-model\packaging\dist\.tmp-zmnm0qp6\adaboost-model-0.2.0.tar", last modified: Tue Jun 27 16:02:12 2023, max compression
```

## Comparing `adaboost_model-0.1.0.tar` & `adaboost-model-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,11 @@
-drwxrwxrwx   0        0        0        0 2020-11-08 01:29:08.000000 adaboost_model-0.1.0/
--rw-rw-rw-   0        0        0      369 2020-10-28 06:33:41.000000 adaboost_model-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      767 2020-11-08 01:29:08.000000 adaboost_model-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2020-11-08 01:29:07.000000 adaboost_model-0.1.0/adaboost_model/
--rw-rw-rw-   0        0        0        5 2020-07-01 23:15:51.000000 adaboost_model-0.1.0/adaboost_model/VERSION
--rw-rw-rw-   0        0        0      454 2020-10-28 07:18:45.000000 adaboost_model-0.1.0/adaboost_model/__init__.py
-drwxrwxrwx   0        0        0        0 2020-11-08 01:29:08.000000 adaboost_model-0.1.0/adaboost_model/config/
--rw-rw-rw-   0        0        0        0 2020-07-01 23:15:51.000000 adaboost_model-0.1.0/adaboost_model/config/__init__.py
--rw-rw-rw-   0        0        0     1678 2020-11-07 16:48:04.000000 adaboost_model-0.1.0/adaboost_model/config/config.py
--rw-rw-rw-   0        0        0      563 2020-07-01 23:15:51.000000 adaboost_model-0.1.0/adaboost_model/config/logging_config.py
-drwxrwxrwx   0        0        0        0 2020-11-08 01:29:08.000000 adaboost_model-0.1.0/adaboost_model/datasets/
--rw-rw-rw-   0        0        0        0 2020-07-01 23:15:51.000000 adaboost_model-0.1.0/adaboost_model/datasets/__init__.py
--rw-rw-rw-   0        0        0    35862 2020-10-30 14:32:38.000000 adaboost_model-0.1.0/adaboost_model/datasets/test.csv
--rw-rw-rw-   0        0        0    83272 2020-10-30 14:33:30.000000 adaboost_model-0.1.0/adaboost_model/datasets/train.csv
--rw-rw-rw-   0        0        0      852 2020-10-30 04:15:07.000000 adaboost_model-0.1.0/adaboost_model/pipeline.py
--rw-rw-rw-   0        0        0     1020 2020-11-08 01:28:23.000000 adaboost_model-0.1.0/adaboost_model/predict.py
-drwxrwxrwx   0        0        0        0 2020-11-08 01:29:08.000000 adaboost_model-0.1.0/adaboost_model/processing/
--rw-rw-rw-   0        0        0        0 2020-07-01 23:15:51.000000 adaboost_model-0.1.0/adaboost_model/processing/__init__.py
--rw-rw-rw-   0        0        0     1661 2020-11-07 16:14:25.000000 adaboost_model-0.1.0/adaboost_model/processing/data_management.py
--rw-rw-rw-   0        0        0      148 2020-07-01 23:15:51.000000 adaboost_model-0.1.0/adaboost_model/processing/errors.py
--rw-rw-rw-   0        0        0     2236 2020-10-28 06:40:58.000000 adaboost_model-0.1.0/adaboost_model/processing/preprocessors.py
--rw-rw-rw-   0        0        0      798 2020-11-07 16:57:23.000000 adaboost_model-0.1.0/adaboost_model/processing/validation.py
--rw-rw-rw-   0        0        0     1020 2020-10-30 04:27:00.000000 adaboost_model-0.1.0/adaboost_model/train_pipeline.py
-drwxrwxrwx   0        0        0        0 2020-11-08 01:29:08.000000 adaboost_model-0.1.0/adaboost_model/trained_models/
--rw-rw-rw-   0        0        0        0 2020-07-01 23:15:51.000000 adaboost_model-0.1.0/adaboost_model/trained_models/__init__.py
--rw-rw-rw-   0        0        0    46151 2020-11-08 01:29:01.000000 adaboost_model-0.1.0/adaboost_model/trained_models/adaboost_model_output_v0.1.0.pkl
-drwxrwxrwx   0        0        0        0 2020-11-08 01:29:08.000000 adaboost_model-0.1.0/adaboost_model.egg-info/
--rw-rw-rw-   0        0        0      767 2020-11-08 01:29:05.000000 adaboost_model-0.1.0/adaboost_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      878 2020-11-08 01:29:06.000000 adaboost_model-0.1.0/adaboost_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-11-08 01:29:05.000000 adaboost_model-0.1.0/adaboost_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      167 2020-11-08 01:29:05.000000 adaboost_model-0.1.0/adaboost_model.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2020-11-08 01:29:05.000000 adaboost_model-0.1.0/adaboost_model.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      611 2020-07-01 23:15:51.000000 adaboost_model-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2020-11-08 01:29:08.000000 adaboost_model-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2393 2020-10-30 14:18:25.000000 adaboost_model-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 16:02:12.163359 adaboost-model-0.2.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-27 15:55:58.000000 adaboost-model-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      588 2023-06-27 16:02:12.163359 adaboost-model-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-06-27 15:55:33.000000 adaboost-model-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 16:02:12.163359 adaboost-model-0.2.0/adaboost_model.egg-info/
+-rw-rw-rw-   0        0        0      588 2023-06-27 16:02:12.000000 adaboost-model-0.2.0/adaboost_model.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-06-27 16:02:12.000000 adaboost-model-0.2.0/adaboost_model.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 16:02:12.000000 adaboost-model-0.2.0/adaboost_model.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 16:02:12.000000 adaboost-model-0.2.0/adaboost_model.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      714 2023-06-27 16:00:49.000000 adaboost-model-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 16:02:12.163359 adaboost-model-0.2.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

