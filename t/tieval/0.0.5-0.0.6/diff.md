# Comparing `tmp/tieval-0.0.5.tar.gz` & `tmp/tieval-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tieval-0.0.5.tar", last modified: Wed Jan 11 09:35:27 2023, max compression
+gzip compressed data, was "tieval-0.0.6.tar", last modified: Tue Jun 27 15:49:17 2023, max compression
```

## Comparing `tieval-0.0.5.tar` & `tieval-0.0.6.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-01-11 09:35:27.587662 tieval-0.0.5/
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     1377 2023-01-11 09:26:22.000000 tieval-0.0.5/LICENSE
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      149 2022-04-04 14:33:29.000000 tieval-0.0.5/MANIFEST.in
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     3029 2023-01-11 09:35:27.587662 tieval-0.0.5/PKG-INFO
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     2398 2023-01-11 09:32:35.000000 tieval-0.0.5/README.md
-drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-01-11 09:35:27.579662 tieval-0.0.5/imgs/
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    85616 2022-03-31 16:54:12.000000 tieval-0.0.5/imgs/tieval.png
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     3737 2023-01-11 09:34:43.000000 tieval-0.0.5/requirements.txt
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)       38 2023-01-11 09:35:27.587662 tieval-0.0.5/setup.cfg
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     1221 2023-01-11 09:33:23.000000 tieval-0.0.5/setup.py
-drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-01-11 09:35:27.579662 tieval-0.0.5/tests/
-drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-01-11 09:35:27.583662 tieval-0.0.5/tests/files/
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    26272 2022-09-17 19:07:39.000000 tieval-0.0.5/tests/files/ancient_time.tml
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     4322 2022-08-04 18:29:49.000000 tieval-0.0.5/tests/files/krauts.tml
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     7559 2022-09-12 20:52:17.000000 tieval-0.0.5/tests/files/professor_heideltime.json
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     2952 2022-04-18 16:41:08.000000 tieval-0.0.5/tests/files/sample.tml
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    14449 2022-05-17 15:21:27.000000 tieval-0.0.5/tests/files/tcr.tml
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)   137747 2022-03-31 16:54:12.000000 tieval-0.0.5/tests/files/tempeval_2.json
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)   151547 2022-04-18 11:11:11.000000 tieval-0.0.5/tests/files/tempeval_2_italian.json
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    54703 2022-05-17 15:21:18.000000 tieval-0.0.5/tests/files/tempeval_3.tml
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    13084 2022-03-31 16:54:12.000000 tieval-0.0.5/tests/files/timebank.tml
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    24076 2022-05-17 15:21:27.000000 tieval-0.0.5/tests/files/timebank12.tml
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     4028 2022-05-17 15:21:35.000000 tieval-0.0.5/tests/files/timebankpt.tml
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      510 2022-08-22 18:02:21.000000 tieval-0.0.5/tests/test_base.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     2976 2022-05-26 14:53:04.000000 tieval-0.0.5/tests/test_closure.py
-drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-01-11 09:35:27.583662 tieval-0.0.5/tests/test_datasets/
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    10300 2022-09-30 20:41:39.000000 tieval-0.0.5/tests/test_datasets/test_download_and_read.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     3022 2022-09-18 20:10:27.000000 tieval-0.0.5/tests/test_datasets/test_readers.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      742 2022-09-18 20:45:32.000000 tieval-0.0.5/tests/test_datasets/test_validate_data.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      976 2022-04-18 15:39:30.000000 tieval-0.0.5/tests/test_entities.py
-drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-01-11 09:35:27.583662 tieval-0.0.5/tests/test_evalaution/
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     1041 2022-10-03 21:12:48.000000 tieval-0.0.5/tests/test_evalaution/test_evalaute.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     2478 2022-08-23 14:50:46.000000 tieval-0.0.5/tests/test_evalaution/test_metrics.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     1909 2022-03-31 16:54:12.000000 tieval-0.0.5/tests/test_links.py
-drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-01-11 09:35:27.583662 tieval-0.0.5/tests/test_models/
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      234 2023-01-11 07:47:16.000000 tieval-0.0.5/tests/test_models/test_classification.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     1430 2023-01-11 09:01:24.000000 tieval-0.0.5/tests/test_models/test_identification.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     4691 2022-05-26 13:59:14.000000 tieval-0.0.5/tests/test_temporal_relation.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     1253 2022-08-22 18:02:21.000000 tieval-0.0.5/tests/test_utils.py
-drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-01-11 09:35:27.583662 tieval-0.0.5/tieval/
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)       83 2023-01-04 19:00:10.000000 tieval-0.0.5/tieval/__init__.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      941 2023-01-04 19:00:10.000000 tieval-0.0.5/tieval/__main__.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     5348 2023-01-04 19:00:10.000000 tieval-0.0.5/tieval/base.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     5578 2022-08-22 18:04:22.000000 tieval-0.0.5/tieval/closure.py
-drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-01-11 09:35:27.583662 tieval-0.0.5/tieval/datasets/
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     1306 2022-09-30 20:46:24.000000 tieval-0.0.5/tieval/datasets/__init__.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    12812 2022-09-30 11:08:31.000000 tieval-0.0.5/tieval/datasets/metadata.py
-drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-01-11 09:35:27.583662 tieval-0.0.5/tieval/datasets/readers/
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)       93 2022-08-22 17:39:41.000000 tieval-0.0.5/tieval/datasets/readers/__init__.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     8531 2022-09-30 20:46:24.000000 tieval-0.0.5/tieval/datasets/readers/dataset.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    44022 2022-09-19 10:13:49.000000 tieval-0.0.5/tieval/datasets/readers/document.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      762 2022-09-17 17:35:14.000000 tieval-0.0.5/tieval/datasets/utils.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     2411 2023-01-04 19:00:10.000000 tieval-0.0.5/tieval/entities.py
-drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-01-11 09:35:27.583662 tieval-0.0.5/tieval/evaluate/
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     8261 2023-01-04 19:00:10.000000 tieval-0.0.5/tieval/evaluate/__init__.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     1879 2022-08-31 11:28:40.000000 tieval-0.0.5/tieval/evaluate/metrics.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     3756 2023-01-04 19:00:10.000000 tieval-0.0.5/tieval/links.py
-drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-01-11 09:35:27.587662 tieval-0.0.5/tieval/models/
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      417 2023-01-04 19:00:10.000000 tieval-0.0.5/tieval/models/__init__.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      644 2023-01-04 19:00:10.000000 tieval-0.0.5/tieval/models/base.py
-drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-01-11 09:35:27.587662 tieval-0.0.5/tieval/models/classification/
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)       72 2022-08-22 17:39:41.000000 tieval-0.0.5/tieval/models/classification/__init__.py
-drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-01-11 09:35:27.587662 tieval-0.0.5/tieval/models/classification/temporal_relation/
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)       81 2022-08-22 17:39:41.000000 tieval-0.0.5/tieval/models/classification/temporal_relation/__init__.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    10257 2023-01-04 19:00:10.000000 tieval-0.0.5/tieval/models/classification/temporal_relation/cogcomp2.py
-drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-01-11 09:35:27.587662 tieval-0.0.5/tieval/models/identification/
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      208 2023-01-04 19:00:10.000000 tieval-0.0.5/tieval/models/identification/__init__.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     4278 2023-01-04 19:00:10.000000 tieval-0.0.5/tieval/models/identification/event.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     5529 2023-01-11 08:59:47.000000 tieval-0.0.5/tieval/models/identification/timex.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      334 2023-01-04 19:00:10.000000 tieval-0.0.5/tieval/models/metadata.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    10265 2022-08-22 18:02:21.000000 tieval-0.0.5/tieval/temporal_relation.py
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     2168 2023-01-04 19:00:12.000000 tieval-0.0.5/tieval/utils.py
-drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-01-11 09:35:27.583662 tieval-0.0.5/tieval.egg-info/
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     3029 2023-01-11 09:35:27.000000 tieval-0.0.5/tieval.egg-info/PKG-INFO
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     1693 2023-01-11 09:35:27.000000 tieval-0.0.5/tieval.egg-info/SOURCES.txt
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)        1 2023-01-11 09:35:27.000000 tieval-0.0.5/tieval.egg-info/dependency_links.txt
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)       89 2023-01-11 09:35:27.000000 tieval-0.0.5/tieval.egg-info/requires.txt
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)        7 2023-01-11 09:35:27.000000 tieval-0.0.5/tieval.egg-info/top_level.txt
--rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)       90 2022-04-19 14:40:53.000000 tieval-0.0.5/tox.ini
+drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-06-27 15:49:17.689479 tieval-0.0.6/
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     1377 2023-04-10 17:34:23.000000 tieval-0.0.6/LICENSE
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      149 2023-01-05 11:57:35.000000 tieval-0.0.6/MANIFEST.in
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     3528 2023-06-27 15:49:17.689479 tieval-0.0.6/PKG-INFO
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     2898 2023-04-11 11:38:00.000000 tieval-0.0.6/README.md
+drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-06-27 15:49:17.677479 tieval-0.0.6/imgs/
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    85616 2023-01-05 11:57:35.000000 tieval-0.0.6/imgs/tieval.png
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     3262 2023-04-11 11:19:14.000000 tieval-0.0.6/requirements.txt
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)       38 2023-06-27 15:49:17.689479 tieval-0.0.6/setup.cfg
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     1221 2023-06-27 15:48:15.000000 tieval-0.0.6/setup.py
+drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-06-27 15:49:17.681479 tieval-0.0.6/tests/
+drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-06-27 15:49:17.681479 tieval-0.0.6/tests/files/
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    26272 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/files/ancient_time.tml
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     4322 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/files/krauts.tml
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     7559 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/files/professor_heideltime.json
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     2952 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/files/sample.tml
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    14449 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/files/tcr.tml
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)   137747 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/files/tempeval_2.json
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)   151547 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/files/tempeval_2_italian.json
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    54703 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/files/tempeval_3.tml
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    13084 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/files/timebank.tml
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    24076 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/files/timebank12.tml
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     4028 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/files/timebankpt.tml
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      510 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/test_base.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     2976 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/test_closure.py
+drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-06-27 15:49:17.681479 tieval-0.0.6/tests/test_datasets/
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    10570 2023-06-27 15:20:15.000000 tieval-0.0.6/tests/test_datasets/test_download_and_read.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     3022 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/test_datasets/test_readers.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      742 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/test_datasets/test_validate_data.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      976 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/test_entities.py
+drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-06-27 15:49:17.685479 tieval-0.0.6/tests/test_evalaution/
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     1041 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/test_evalaution/test_evalaute.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     2478 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/test_evalaution/test_metrics.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     1909 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/test_links.py
+drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-06-27 15:49:17.685479 tieval-0.0.6/tests/test_models/
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      234 2023-04-10 17:34:23.000000 tieval-0.0.6/tests/test_models/test_classification.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     1430 2023-04-10 17:34:23.000000 tieval-0.0.6/tests/test_models/test_identification.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     4691 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/test_temporal_relation.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     1253 2023-01-05 11:57:35.000000 tieval-0.0.6/tests/test_utils.py
+drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-06-27 15:49:17.685479 tieval-0.0.6/tieval/
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)       83 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/__init__.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      941 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/__main__.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     5348 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/base.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     5578 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/closure.py
+drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-06-27 15:49:17.685479 tieval-0.0.6/tieval/datasets/
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     1306 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/datasets/__init__.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    12812 2023-06-27 15:32:54.000000 tieval-0.0.6/tieval/datasets/metadata.py
+drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-06-27 15:49:17.685479 tieval-0.0.6/tieval/datasets/readers/
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)       93 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/datasets/readers/__init__.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     8531 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/datasets/readers/dataset.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    44022 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/datasets/readers/document.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      762 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/datasets/utils.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     2411 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/entities.py
+drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-06-27 15:49:17.685479 tieval-0.0.6/tieval/evaluate/
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     8261 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/evaluate/__init__.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     1879 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/evaluate/metrics.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     3756 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/links.py
+drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-06-27 15:49:17.689479 tieval-0.0.6/tieval/models/
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      417 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/models/__init__.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      644 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/models/base.py
+drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-06-27 15:49:17.689479 tieval-0.0.6/tieval/models/classification/
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)       72 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/models/classification/__init__.py
+drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-06-27 15:49:17.689479 tieval-0.0.6/tieval/models/classification/temporal_relation/
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)       81 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/models/classification/temporal_relation/__init__.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    10257 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/models/classification/temporal_relation/cogcomp2.py
+drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-06-27 15:49:17.689479 tieval-0.0.6/tieval/models/identification/
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      208 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/models/identification/__init__.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     4278 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/models/identification/event.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     5529 2023-04-10 17:34:23.000000 tieval-0.0.6/tieval/models/identification/timex.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)      334 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/models/metadata.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)    10265 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/temporal_relation.py
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     2168 2023-01-05 11:57:35.000000 tieval-0.0.6/tieval/utils.py
+drwxrwxr-x   0 hugosousa  (1000) hugosousa  (1000)        0 2023-06-27 15:49:17.685479 tieval-0.0.6/tieval.egg-info/
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     3528 2023-06-27 15:49:17.000000 tieval-0.0.6/tieval.egg-info/PKG-INFO
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)     1693 2023-06-27 15:49:17.000000 tieval-0.0.6/tieval.egg-info/SOURCES.txt
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)        1 2023-06-27 15:49:17.000000 tieval-0.0.6/tieval.egg-info/dependency_links.txt
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)       89 2023-06-27 15:49:17.000000 tieval-0.0.6/tieval.egg-info/requires.txt
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)        7 2023-06-27 15:49:17.000000 tieval-0.0.6/tieval.egg-info/top_level.txt
+-rw-rw-r--   0 hugosousa  (1000) hugosousa  (1000)       90 2023-01-05 11:57:35.000000 tieval-0.0.6/tox.ini
```

### Comparing `tieval-0.0.5/LICENSE` & `tieval-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/PKG-INFO` & `tieval-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tieval
-Version: 0.0.5
+Version: 0.0.6
 Summary: This framework facilitates the development and test of temporal-aware models.
 Home-page: https://github.com/LIAAD/tieval
 Author: Hugo Sousa
 Author-email: hugo.o.sousa@inesctec.pt
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -15,19 +15,22 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tieval
 
 [![PyPI](https://img.shields.io/pypi/v/tieval)](https://pypi.org/project/tieval/)
+[![Documentation Status](https://readthedocs.org/projects/tieval/badge/?version=latest)](https://tieval.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tieval)
 [![PyPI - License](https://img.shields.io/pypi/l/tieval)](LICENSE)
 ![GitHub repo size](https://img.shields.io/github/repo-size/LIAAD/tieval)
 
-A framework for the development of temporally aware models.
+[![Paper](https://img.shields.io/badge/-paper-9cf)](https://arxiv.org/pdf/2301.04643.pdf)
+
+A framework for evaluation and development of temporally aware models.
 
 ![](imgs/tieval.png)
 
 ## Installation
 
 The package is available on [PyPI](https://pypi.org/project/tieval/):
 
@@ -110,7 +113,13 @@
 
 Hugo Sousa - hugo.o.sousa@inesctec.pt
 
 This framework is part of the [Text2Story](https://text2story.inesctec.pt/) project which is financed by the ERDF –
 European Regional Development Fund through the North Portugal Regional Operational Programme (NORTE 2020), under the
 PORTUGAL 2020 and by National Funds through the Portuguese funding agency, FCT - Fundação para a Ciência e a Tecnologia
 within project PTDC/CCI-COM/31857/2017 (NORTE-01-0145-FEDER-03185) 
+
+## Publications
+
+If you use `tieval` in your work please site the following article:
+
+Sousa, H., Jorge, A.M., & Campos, R. (2023). tieval: An Evaluation Framework for Temporal Information Extraction Systems. [pdf](https://arxiv.org/pdf/2301.04643.pdf)
```

### Comparing `tieval-0.0.5/README.md` & `tieval-0.0.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # tieval
 
 [![PyPI](https://img.shields.io/pypi/v/tieval)](https://pypi.org/project/tieval/)
+[![Documentation Status](https://readthedocs.org/projects/tieval/badge/?version=latest)](https://tieval.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tieval)
 [![PyPI - License](https://img.shields.io/pypi/l/tieval)](LICENSE)
 ![GitHub repo size](https://img.shields.io/github/repo-size/LIAAD/tieval)
 
-A framework for the development of temporally aware models.
+[![Paper](https://img.shields.io/badge/-paper-9cf)](https://arxiv.org/pdf/2301.04643.pdf)
+
+A framework for evaluation and development of temporally aware models.
 
 ![](imgs/tieval.png)
 
 ## Installation
 
 The package is available on [PyPI](https://pypi.org/project/tieval/):
 
@@ -91,8 +94,14 @@
 ## Meta
 
 Hugo Sousa - hugo.o.sousa@inesctec.pt
 
 This framework is part of the [Text2Story](https://text2story.inesctec.pt/) project which is financed by the ERDF –
 European Regional Development Fund through the North Portugal Regional Operational Programme (NORTE 2020), under the
 PORTUGAL 2020 and by National Funds through the Portuguese funding agency, FCT - Fundação para a Ciência e a Tecnologia
-within project PTDC/CCI-COM/31857/2017 (NORTE-01-0145-FEDER-03185) 
+within project PTDC/CCI-COM/31857/2017 (NORTE-01-0145-FEDER-03185) 
+
+## Publications
+
+If you use `tieval` in your work please site the following article:
+
+Sousa, H., Jorge, A.M., & Campos, R. (2023). tieval: An Evaluation Framework for Temporal Information Extraction Systems. [pdf](https://arxiv.org/pdf/2301.04643.pdf)
```

### Comparing `tieval-0.0.5/imgs/tieval.png` & `tieval-0.0.6/imgs/tieval.png`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/requirements.txt` & `tieval-0.0.6/requirements.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,207 +1,183 @@
-alabaster==0.7.12
+aiohttp==3.8.4
+aiosignal==1.3.1
+alabaster==0.7.13
 allennlp==2.9.3
-anyio==3.5.0
 argon2-cffi==21.3.0
 argon2-cffi-bindings==21.2.0
 asttokens==2.0.5
+async-timeout==4.0.2
 attrs==21.4.0
-Babel==2.10.1
+Babel==2.12.1
 backcall==0.2.0
 base58==2.1.1
 beautifulsoup4==4.11.1
-bleach==4.1.0
-blis==0.7.7
-boto3==1.22.9
-botocore==1.25.9
-build==0.7.0
-bump2version==1.0.1
-bumpversion==0.6.0
-cached-path==1.1.2
-cachetools==5.0.0
+bleach==5.0.1
+blis==0.7.8
+boto3==1.24.28
+botocore==1.27.28
+cached-path==1.1.5
+cachetools==5.2.0
 catalogue==2.0.7
-certifi==2021.10.8
-cffi==1.15.0
-charset-normalizer==2.0.12
-check-manifest==0.48
+certifi==2022.6.15
+cffi==1.15.1
+charset-normalizer==2.1.0
 click==8.0.4
-colorama==0.4.4
 commonmark==0.9.1
-cryptography==36.0.2
-cycler==0.11.0
 cymem==2.0.6
-debugpy==1.6.0
+debugpy==1.6.2
 decorator==5.1.1
 defusedxml==0.7.1
-dill==0.3.4
+dill==0.3.5.1
 docker-pycreds==0.4.0
-docutils==0.18.1
-emoji==1.7.0
+docutils==0.19
+emoji==2.0.0
 entrypoints==0.4
-executing==0.8.3
+executing==0.9.1
 fairscale==0.4.6
-fastjsonschema==2.15.3
+fastjsonschema==2.16.1
 filelock==3.6.0
-fonttools==4.33.3
-furo==2022.4.7
+frozenlist==1.3.3
+furo==2023.3.27
 gitdb==4.0.9
 GitPython==3.1.27
-google-api-core==2.7.3
-google-auth==2.6.6
-google-cloud-core==2.3.0
-google-cloud-storage==2.3.0
+google-api-core==2.8.2
+google-auth==2.9.1
+google-cloud-core==2.3.1
+google-cloud-storage==2.4.0
 google-crc32c==1.3.0
-google-resumable-media==2.3.2
-googleapis-common-protos==1.56.0
-h5py==3.6.0
-huggingface-hub==0.5.1
+google-resumable-media==2.3.3
+googleapis-common-protos==1.56.4
+h5py==3.7.0
+huggingface-hub==0.8.1
 idna==3.3
-imagesize==1.3.0
-importlib-metadata==4.11.3
-importlib-resources==5.7.1
+imagesize==1.4.1
+importlib-metadata==6.3.0
+importlib-resources==5.9.0
 iniconfig==1.1.1
-ipykernel==6.13.0
-ipython==8.3.0
+ipykernel==6.15.1
+ipython==8.4.0
 ipython-genutils==0.2.0
-ipywidgets==7.7.0
 jedi==0.18.1
-jeepney==0.8.0
-Jinja2==3.1.1
-jmespath==1.0.0
+Jinja2==3.1.2
+jmespath==1.0.1
 joblib==1.1.0
-json5==0.9.8
 jsonnet==0.18.0
-jsonschema==4.5.1
-jupyter==1.0.0
-jupyter-client==7.3.1
-jupyter-console==6.4.3
-jupyter-core==4.10.0
-jupyter-server==1.17.0
-jupyterlab==3.4.0
+jsonschema==4.9.0
+jupyter-client==7.3.4
+jupyter-core==4.11.1
 jupyterlab-pygments==0.2.2
-jupyterlab-server==2.13.0
-jupyterlab-widgets==1.1.0
-keyring==23.5.0
-kiwisolver==1.4.2
 langcodes==3.3.0
-livereload==2.6.3
 lmdb==1.3.0
 MarkupSafe==2.1.1
-matplotlib==3.5.2
 matplotlib-inline==0.1.3
 mistune==0.8.4
 more-itertools==8.13.0
-murmurhash==1.0.6
-nbclassic==0.3.7
-nbclient==0.6.3
+multidict==6.0.4
+murmurhash==1.0.7
+nbclient==0.6.6
 nbconvert==6.5.0
 nbformat==5.4.0
-nbsphinx==0.8.8
+nbsphinx==0.9.1
 nest-asyncio==1.5.5
 networkx==2.8.1
 nltk==3.6.7
-notebook==6.4.10
-notebook-shim==0.1.0
-numpy==1.22.3
+notebook==6.4.12
+numpy==1.23.1
+openai==0.27.2
 packaging==21.3
+pandas==1.4.3
+pandoc==2.3
 pandocfilters==1.5.0
 parso==0.8.3
 pathtools==0.1.2
-pathy==0.6.1
-pep517==0.12.0
+pathy==0.6.2
 pexpect==4.8.0
 pickleshare==0.7.5
-Pillow==9.1.0
-pkginfo==1.8.2
+Pillow==9.2.0
+pkgutil-resolve-name==1.3.10
 pluggy==1.0.0
+plumbum==1.8.1
+ply==3.11
 preshed==3.0.6
 prometheus-client==0.14.1
 promise==2.3
-prompt-toolkit==3.0.29
+prompt-toolkit==3.0.30
 protobuf==3.20.1
-psutil==5.9.0
+psutil==5.9.1
 ptyprocess==0.7.0
 pure-eval==0.2.2
 py==1.11.0
-py_heideltime
+py-heideltime==1.0.3
+py4j==0.10.9.5
 pyasn1==0.4.8
 pyasn1-modules==0.2.8
 pycparser==2.21
 pydantic==1.8.2
-Pygments==2.11.2
-Pyment==0.3.3
-pyparsing==3.0.7
+Pygments==2.15.0
+pyparsing==3.0.9
 pyrsistent==0.18.1
-pytest==6.2.5
+pyspark==3.3.0
+pytest==7.1.2
 python-dateutil==2.8.2
-pytz==2022.1
+pytz==2022.2
 PyYAML==6.0
-pyzmq==22.3.0
-qtconsole==5.3.0
-QtPy==2.1.0
-readme-renderer==34.0
-regex==2022.3.15
-requests==2.27.1
-requests-toolbelt==0.9.1
-rfc3986==2.0.0
-rich==12.1.0
+pyzmq==23.2.0
+regex==2022.7.9
+requests==2.28.1
+rich==12.5.1
 rsa==4.8
-s3transfer==0.5.2
+s3transfer==0.6.0
 sacremoses==0.0.53
-scikit-learn==1.0.2
-scipy==1.8.0
-SecretStorage==3.3.1
+scikit-learn==1.1.1
+scipy==1.8.1
 Send2Trash==1.8.0
 sentencepiece==0.1.96
-sentry-sdk==1.5.11
+sentry-sdk==1.7.1
 setproctitle==1.2.3
 shortuuid==1.0.9
 six==1.16.0
 smart-open==5.2.1
 smmap==5.0.0
-sniffio==1.2.0
 snowballstemmer==2.2.0
 soupsieve==2.3.2.post1
 spacy==3.2.4
 spacy-legacy==3.0.9
 spacy-loggers==1.0.2
-Sphinx==4.5.0
-sphinx-autobuild==2021.3.14
-sphinx-better-theme==0.1.5
-sphinx-copybutton==0.5.0
-sphinx-rtd-theme==1.0.0
-sphinxcontrib-applehelp==1.0.2
+spark-nlp==4.1.0
+sparknlp==1.0.0
+sphinx==6.1.3
+sphinx-basic-ng==1.0.0b1
+sphinx-copybutton==0.5.1
+sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-srsly==2.4.2
-stack-data==0.2.0
+srsly==2.4.3
+stack-data==0.3.0
 tabulate==0.8.9
-tensorboardX==2.5
+tensorboardX==2.5.1
 termcolor==1.1.0
-terminado==0.13.3
-thinc==8.0.15
+terminado==0.15.0
+thinc==8.0.17
 threadpoolctl==3.1.0
 tinycss2==1.1.1
 tokenizers==0.12.1
-toml==0.10.2
 tomli==2.0.1
 torch==1.11.0
 torchvision==0.12.0
-tornado==6.1
-tqdm==4.62.3
-traitlets==5.2.0
+tornado==6.2
+tqdm==4.64.0
+traitlets==5.3.0
 transformers==4.18.0
-twine==4.0.0
-typer==0.4.1
-typing_extensions==4.1.1
-urllib3==1.26.9
-wandb==0.12.16
+typer==0.4.2
+typing-extensions==4.3.0
+urllib3==1.26.10
+wandb==0.12.21
 wasabi==0.9.1
 wcwidth==0.2.5
 webencodings==0.5.1
-websocket-client==1.3.2
-widgetsnbextension==3.6.0
 xmltodict==0.12.0
-zipp==3.8.0
+yarl==1.8.2
+zipp==3.8.1
```

### Comparing `tieval-0.0.5/setup.py` & `tieval-0.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="tieval",
-    version="0.0.5",
+    version="0.0.6",
     url="https://github.com/LIAAD/tieval",
     license='MIT',
     author="Hugo Sousa",
     author_email="hugo.o.sousa@inesctec.pt",
     description=
     "This framework facilitates the development and test of temporal-aware models.",
     long_description_content_type='text/markdown',
```

### Comparing `tieval-0.0.5/tests/files/ancient_time.tml` & `tieval-0.0.6/tests/files/ancient_time.tml`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/files/krauts.tml` & `tieval-0.0.6/tests/files/krauts.tml`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/files/professor_heideltime.json` & `tieval-0.0.6/tests/files/professor_heideltime.json`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/files/sample.tml` & `tieval-0.0.6/tests/files/sample.tml`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/files/tcr.tml` & `tieval-0.0.6/tests/files/tcr.tml`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/files/tempeval_2.json` & `tieval-0.0.6/tests/files/tempeval_2.json`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/files/tempeval_2_italian.json` & `tieval-0.0.6/tests/files/tempeval_2_italian.json`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/files/tempeval_3.tml` & `tieval-0.0.6/tests/files/tempeval_3.tml`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/files/timebank.tml` & `tieval-0.0.6/tests/files/timebank.tml`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/files/timebank12.tml` & `tieval-0.0.6/tests/files/timebank12.tml`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/files/timebankpt.tml` & `tieval-0.0.6/tests/files/timebankpt.tml`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/test_closure.py` & `tieval-0.0.6/tests/test_closure.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/test_datasets/test_download_and_read.py` & `tieval-0.0.6/tests/test_datasets/test_download_and_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,7 +329,16 @@
 def test_download_and_read_eventtime(tmp_path):
     corpus = "eventtime"
     n_docs, n_events, n_timexs, n_tlinks = _test_download_and_read(corpus, tmp_path)
     assert n_docs == 36
     assert n_timexs == 0
     assert n_events == 1_498
     assert n_tlinks == 0
+
+
+def test_download_and_read_timebank(tmp_path):
+    corpus = "timebank"
+    n_docs, n_events, n_timexs, n_tlinks = _test_download_and_read(corpus, tmp_path)
+    assert n_docs == 183
+    assert n_timexs == 1_426
+    assert n_events == 6_681
+    assert n_tlinks == 5_120
```

### Comparing `tieval-0.0.5/tests/test_datasets/test_readers.py` & `tieval-0.0.6/tests/test_datasets/test_readers.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/test_datasets/test_validate_data.py` & `tieval-0.0.6/tests/test_datasets/test_validate_data.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/test_entities.py` & `tieval-0.0.6/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/test_evalaution/test_evalaute.py` & `tieval-0.0.6/tests/test_evalaution/test_evalaute.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/test_evalaution/test_metrics.py` & `tieval-0.0.6/tests/test_evalaution/test_metrics.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/test_links.py` & `tieval-0.0.6/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/test_models/test_identification.py` & `tieval-0.0.6/tests/test_models/test_identification.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/test_temporal_relation.py` & `tieval-0.0.6/tests/test_temporal_relation.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tests/test_utils.py` & `tieval-0.0.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tieval/__main__.py` & `tieval-0.0.6/tieval/__main__.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tieval/base.py` & `tieval-0.0.6/tieval/base.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tieval/closure.py` & `tieval-0.0.6/tieval/closure.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tieval/datasets/__init__.py` & `tieval-0.0.6/tieval/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tieval/datasets/metadata.py` & `tieval-0.0.6/tieval/datasets/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,21 +112,21 @@
     ),
 
     "aquaint": DatasetMetadata(
         name="AQUAINT",
         language="english",
         reader=XMLDatasetReader,
         doc_reader=TempEval3DocumentReader,
-        url="https://drive.inesctec.pt/s/fxRfPfLcKKJ74Dn/download",
+        url="https://drive.inesctec.pt/s/EsCsL6bayxsg5Co/download",
     ),
 
     "eventtime": DatasetMetadata(
         name="EventTime",
         language="english",
-        url="https://drive.inesctec.pt/s/wbGtJceye6ntkiS/download",
+        url="https://drive.inesctec.pt/s/8HyHGnLE7QbWRCF/download",
         reader=EventTimeDatasetReader,
         base=["timebank"]
     ),
 
     "fr_timebank": DatasetMetadata(
         name="FR_Timebank",
         language="french",
@@ -134,15 +134,15 @@
         reader=XMLDatasetReader,
         doc_reader=FRTimeBankDocumentReader,
     ),
 
     "grapheve": DatasetMetadata(
         name="GraphEve",
         language="english",
-        url="https://drive.inesctec.pt/s/eKSHKB6gMozCP4Q/download",
+        url="https://drive.inesctec.pt/s/ctPKsYbt5terqJS/download",
         reader=XMLDatasetReader,
         doc_reader=GraphEveDocumentReader
     ),
 
     "krauts": DatasetMetadata(
         name="KRAUTS",
         language="german",
@@ -174,48 +174,48 @@
         reader=XMLDatasetReader,
         doc_reader=KRAUTSDocumentReader
     ),
 
     "matres": DatasetMetadata(
         name="matres",
         language="english",
-        url="https://drive.inesctec.pt/s/7g68GBTECiD2XYK/download",
+        url="https://drive.inesctec.pt/s/9kpP6oy8y4jZPyN/download",
         base=["tempeval_3"],
         repo="https://github.com/qiangning/MATRES",
         reader=MATRESDatasetReader,
     ),
 
     "meantime_english": DatasetMetadata(
         name="meantime_english",
         language="english",
-        url="https://drive.inesctec.pt/s/QoLwqgdTLkfia7L/download",
+        url="https://drive.inesctec.pt/s/jbHfZYpb3Y3Cs5T/download",
         reader=XMLDatasetReader,
         doc_reader=MeanTimeDocumentReader
     ),
 
     "meantime_spanish": DatasetMetadata(
         name="meantime_spanish",
         language="spanish",
-        url="https://drive.inesctec.pt/s/xEPGnqygP6FEFkP/download",
+        url="https://drive.inesctec.pt/s/HE7qxH6BP6nPEkg/download",
         reader=XMLDatasetReader,
         doc_reader=MeanTimeDocumentReader
     ),
 
     "meantime_dutch": DatasetMetadata(
         name="meantime_dutch",
         language="dutch",
-        url="https://drive.inesctec.pt/s/HyFfxEwryj6Fffq/download",
+        url="https://drive.inesctec.pt/s/pQA3RcKiko2GcMX/download",
         reader=XMLDatasetReader,
         doc_reader=MeanTimeDocumentReader
     ),
 
     "meantime_italian": DatasetMetadata(
         name="meantime_italian",
         language="italian",
-        url="https://drive.inesctec.pt/s/kabifjEcQboKbBA/download",
+        url="https://drive.inesctec.pt/s/m4jckQLrYSxmTEq/download",
         reader=XMLDatasetReader,
         doc_reader=MeanTimeDocumentReader
     ),
 
     "narrative_container": DatasetMetadata(
         name="narrative_container",
         language="italian",
@@ -271,15 +271,15 @@
         reader=JSONDatasetReader,
         doc_reader=ProfessorHeidelTimeDocumentReader,
     ),
 
     "platinum": DatasetMetadata(
         name="Platinum",
         language="english",
-        url="https://drive.inesctec.pt/s/ppCdTWijAYFbRiL/download",
+        url="https://drive.inesctec.pt/s/jpj3iwBDqiW2rWM/download",
         reader=XMLDatasetReader,
         doc_reader=TempEval3DocumentReader,
     ),
 
     "spanish_timebank": DatasetMetadata(
         name="spanish_timebank",
         language="spanish",
@@ -287,121 +287,121 @@
         reader=JSONDatasetReader,
         doc_reader=TempEval2DocumentReader,
     ),
 
     "tcr": DatasetMetadata(
         name="TCR",
         language="english",
-        url="https://drive.inesctec.pt/s/mSGaNyYSiMRTfGH/download",
+        url="https://drive.inesctec.pt/s/WCFxDPc9JeQxG3e/download",
         reader=XMLDatasetReader,
         doc_reader=TCRDocumentReader,
     ),
 
     "tddiscourse": DatasetMetadata(
         name="TDDiscourse",
         language="english",
-        url="https://drive.inesctec.pt/s/9nXDNqt3Sa8bkDk/download",
+        url="https://drive.inesctec.pt/s/fqjsffnrk8TrCLg/download",
         base=["timebank_1.2"],
         reader=TDDiscourseDatasetReader,
     ),
 
     "tempeval_2_chinese": DatasetMetadata(
         name="tempeval_2_chinese",
         language="chinese",
-        url="https://drive.inesctec.pt/s/s4HMWnntet8z2bS/download",
+        url="https://drive.inesctec.pt/s/L7TqZeJC4cG7yfs/download",
         reader=JSONDatasetReader,
         doc_reader=TempEval2DocumentReader,
     ),
 
     "tempeval_2_english": DatasetMetadata(
         name="tempeval_2_english",
         language="english",
-        url="https://drive.inesctec.pt/s/Z2q5oEYf4cAM2ji/download",
+        url="https://drive.inesctec.pt/s/sgGpwHYjHNXqjmp/download",
         reader=JSONDatasetReader,
         doc_reader=TempEval2DocumentReader,
     ),
 
     "tempeval_2_french": DatasetMetadata(
         name="tempeval_2_french",
         language="french",
-        url="https://drive.inesctec.pt/s/mNoo2YFWG4X8tD4/download",
+        url="https://drive.inesctec.pt/s/nNeYpe9BCcj6aCg/download",
         reader=XMLDatasetReader,
         doc_reader=TempEval2FrenchDocumentReader,
     ),
 
     "tempeval_2_italian": DatasetMetadata(
         name="tempeval_2_italian",
         language="italian",
-        url="https://drive.inesctec.pt/s/PkADwaWEogapSWW/download",
+        url="https://drive.inesctec.pt/s/roFgne7kTCdgpoj/download",
         reader=JSONDatasetReader,
         doc_reader=TempEval2DocumentReader,
     ),
 
     "tempeval_2_korean": DatasetMetadata(
         name="tempeval_2_korean",
         language="korean",
-        url="https://drive.inesctec.pt/s/RwMLseDt4GnnfKr/download",
+        url="https://drive.inesctec.pt/s/HL9ie4nqebpLf8Q/download",
         reader=JSONDatasetReader,
         doc_reader=TempEval2DocumentReader,
     ),
 
     "tempeval_2_spanish": DatasetMetadata(
         name="tempeval_2_spanish",
         language="spanish",
-        url="https://drive.inesctec.pt/s/H7otpwJCFCsjM9r/download",
+        url="https://drive.inesctec.pt/s/MNBoR9w29kZTo9T/download",
         reader=JSONDatasetReader,
         doc_reader=TempEval2DocumentReader,
     ),
 
     "tempeval_3": DatasetMetadata(
         name="tempeval_3",
         language="english",
-        url="https://drive.inesctec.pt/s/ebp27ZjfCgDTxwG/download",
+        url="https://drive.inesctec.pt/s/yyDxHXpqkCZA6Cn/download",
         reader=XMLDatasetReader,
         doc_reader=TempEval3DocumentReader,
     ),
 
     "timebank_1.2": DatasetMetadata(
         name="TimeBank_1.2",
         language="english",
-        url="https://drive.inesctec.pt/s/QHiBgZmi45B72AB/download",
+        url="https://drive.inesctec.pt/s/AJKjcCwEED6X9ae/download",
         reader=XMLDatasetReader,
         doc_reader=TimeBank12DocumentReader,
 
     ),
 
     "timebank_dense": DatasetMetadata(
         name="TimeBank_Dense",
         language="english",
-        url="https://drive.inesctec.pt/s/dtztXXBpPPXyzLX/download",
+        url="https://drive.inesctec.pt/s/4AbX8n25Dc3MyGy/download",
         base=["timebank_1.2"],
         reader=TimeBankDenseDatasetReader,
 
     ),
 
     "timebankpt": DatasetMetadata(
         name="TimeBankPT",
         language="portuguese",
-        url="https://drive.inesctec.pt/s/jCcpQGXzLdnL9Tx/download",
+        url="https://drive.inesctec.pt/s/BBQmStdTCL5FSMA/download",
         reader=XMLDatasetReader,
         doc_reader=TimeBankPTDocumentReader,
     ),
 
     "timebank": DatasetMetadata(
         name="TimeBank",
         language="english",
-        url="https://drive.inesctec.pt/s/KmeTs6LqnmzRr2s/download",
+        url="https://drive.inesctec.pt/s/dAttMwk9TiESCt2/download",
         reader=XMLDatasetReader,
         doc_reader=TempEval3DocumentReader,
     ),
 
     "traint3": DatasetMetadata(
         name="Traint3",
         language="spanish",
-        url="https://drive.inesctec.pt/s/SaPzJxD2b9PzxY4/download",
+        url="https://drive.inesctec.pt/s/CFwAqZ8T8ZArHyC/download",
         reader=XMLDatasetReader,
         doc_reader=TempEval3DocumentReader
     ),
 
     "wikiwars": DatasetMetadata(
         name="wikiwars",
         language="english",
```

### Comparing `tieval-0.0.5/tieval/datasets/readers/dataset.py` & `tieval-0.0.6/tieval/datasets/readers/dataset.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tieval/datasets/readers/document.py` & `tieval-0.0.6/tieval/datasets/readers/document.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tieval/datasets/utils.py` & `tieval-0.0.6/tieval/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tieval/entities.py` & `tieval-0.0.6/tieval/entities.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tieval/evaluate/__init__.py` & `tieval-0.0.6/tieval/evaluate/__init__.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tieval/evaluate/metrics.py` & `tieval-0.0.6/tieval/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tieval/links.py` & `tieval-0.0.6/tieval/links.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tieval/models/base.py` & `tieval-0.0.6/tieval/models/base.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tieval/models/classification/temporal_relation/cogcomp2.py` & `tieval-0.0.6/tieval/models/classification/temporal_relation/cogcomp2.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tieval/models/identification/event.py` & `tieval-0.0.6/tieval/models/identification/event.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tieval/models/identification/timex.py` & `tieval-0.0.6/tieval/models/identification/timex.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tieval/temporal_relation.py` & `tieval-0.0.6/tieval/temporal_relation.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tieval/utils.py` & `tieval-0.0.6/tieval/utils.py`

 * *Files identical despite different names*

### Comparing `tieval-0.0.5/tieval.egg-info/PKG-INFO` & `tieval-0.0.6/tieval.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tieval
-Version: 0.0.5
+Version: 0.0.6
 Summary: This framework facilitates the development and test of temporal-aware models.
 Home-page: https://github.com/LIAAD/tieval
 Author: Hugo Sousa
 Author-email: hugo.o.sousa@inesctec.pt
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -15,19 +15,22 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tieval
 
 [![PyPI](https://img.shields.io/pypi/v/tieval)](https://pypi.org/project/tieval/)
+[![Documentation Status](https://readthedocs.org/projects/tieval/badge/?version=latest)](https://tieval.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tieval)
 [![PyPI - License](https://img.shields.io/pypi/l/tieval)](LICENSE)
 ![GitHub repo size](https://img.shields.io/github/repo-size/LIAAD/tieval)
 
-A framework for the development of temporally aware models.
+[![Paper](https://img.shields.io/badge/-paper-9cf)](https://arxiv.org/pdf/2301.04643.pdf)
+
+A framework for evaluation and development of temporally aware models.
 
 ![](imgs/tieval.png)
 
 ## Installation
 
 The package is available on [PyPI](https://pypi.org/project/tieval/):
 
@@ -110,7 +113,13 @@
 
 Hugo Sousa - hugo.o.sousa@inesctec.pt
 
 This framework is part of the [Text2Story](https://text2story.inesctec.pt/) project which is financed by the ERDF –
 European Regional Development Fund through the North Portugal Regional Operational Programme (NORTE 2020), under the
 PORTUGAL 2020 and by National Funds through the Portuguese funding agency, FCT - Fundação para a Ciência e a Tecnologia
 within project PTDC/CCI-COM/31857/2017 (NORTE-01-0145-FEDER-03185) 
+
+## Publications
+
+If you use `tieval` in your work please site the following article:
+
+Sousa, H., Jorge, A.M., & Campos, R. (2023). tieval: An Evaluation Framework for Temporal Information Extraction Systems. [pdf](https://arxiv.org/pdf/2301.04643.pdf)
```

### Comparing `tieval-0.0.5/tieval.egg-info/SOURCES.txt` & `tieval-0.0.6/tieval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

