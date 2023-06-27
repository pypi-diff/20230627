# Comparing `tmp/mimeograph-1.0.3.tar.gz` & `tmp/mimeograph-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimeograph-1.0.3.tar", last modified: Mon Jun 26 15:57:24 2023, max compression
+gzip compressed data, was "mimeograph-1.0.4.tar", last modified: Tue Jun 27 07:06:54 2023, max compression
```

## Comparing `mimeograph-1.0.3.tar` & `mimeograph-1.0.4.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.044392 mimeograph-1.0.3/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-1.0.3/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)       30 2023-05-11 05:33:09.000000 mimeograph-1.0.3/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)    34465 2023-06-26 15:57:24.044392 mimeograph-1.0.3/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)    32079 2023-06-26 13:54:19.000000 mimeograph-1.0.3/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)     4010 2023-06-26 15:56:55.000000 mimeograph-1.0.3/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-06-26 15:57:24.044392 mimeograph-1.0.3/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.036392 mimeograph-1.0.3/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.036392 mimeograph-1.0.3/src/mimeo/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1484 2023-06-26 15:56:55.000000 mimeograph-1.0.3/src/mimeo/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      408 2023-06-24 11:03:12.000000 mimeograph-1.0.3/src/mimeo/__main__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.036392 mimeograph-1.0.3/src/mimeo/cli/
--rw-rw-r--   0 tom       (1000) tom       (1000)      761 2023-05-11 05:33:09.000000 mimeograph-1.0.3/src/mimeo/cli/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2290 2023-05-17 08:57:29.000000 mimeograph-1.0.3/src/mimeo/cli/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4694 2023-06-26 13:54:19.000000 mimeograph-1.0.3/src/mimeo/cli/job.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    18152 2023-06-26 15:56:55.000000 mimeograph-1.0.3/src/mimeo/cli/parsers.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.036392 mimeograph-1.0.3/src/mimeo/config/
--rw-rw-r--   0 tom       (1000) tom       (1000)      837 2023-05-27 06:14:50.000000 mimeograph-1.0.3/src/mimeo/config/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6275 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/config/constants.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    12351 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/config/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    35693 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/config/mimeo_config.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.036392 mimeograph-1.0.3/src/mimeo/consumers/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1322 2023-05-11 05:33:09.000000 mimeograph-1.0.3/src/mimeo/consumers/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1402 2023-06-24 11:02:10.000000 mimeograph-1.0.3/src/mimeo/consumers/consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2146 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/consumers/consumer_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2374 2023-06-24 11:02:23.000000 mimeograph-1.0.3/src/mimeo/consumers/file_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3109 2023-06-26 13:54:19.000000 mimeograph-1.0.3/src/mimeo/consumers/http_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1018 2023-05-12 09:42:23.000000 mimeograph-1.0.3/src/mimeo/consumers/raw_consumer.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.036392 mimeograph-1.0.3/src/mimeo/context/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1001 2023-05-11 05:33:09.000000 mimeograph-1.0.3/src/mimeo/context/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4261 2023-05-11 05:33:09.000000 mimeograph-1.0.3/src/mimeo/context/decorators.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5087 2023-05-11 05:33:09.000000 mimeograph-1.0.3/src/mimeo/context/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    18276 2023-06-23 11:30:49.000000 mimeograph-1.0.3/src/mimeo/context/mimeo_context.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5164 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/context/mimeo_context_manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2911 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/context/mimeo_iteration.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.040392 mimeograph-1.0.3/src/mimeo/database/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1805 2023-05-16 10:04:29.000000 mimeograph-1.0.3/src/mimeo/database/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5638 2023-06-26 14:29:14.000000 mimeograph-1.0.3/src/mimeo/database/cities.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5885 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/database/countries.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5755 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/database/currencies.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6200 2023-05-22 07:52:53.000000 mimeograph-1.0.3/src/mimeo/database/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5599 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/database/first_names.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2235 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/database/last_names.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10234 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/database/mimeo_db.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      702 2023-06-26 13:54:19.000000 mimeograph-1.0.3/src/mimeo/exc.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.040392 mimeograph-1.0.3/src/mimeo/generators/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1221 2023-06-20 06:50:14.000000 mimeograph-1.0.3/src/mimeo/generators/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1149 2023-06-20 06:50:14.000000 mimeograph-1.0.3/src/mimeo/generators/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10680 2023-06-26 13:54:19.000000 mimeograph-1.0.3/src/mimeo/generators/generator.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1852 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/generators/generator_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    17137 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/generators/json_generator.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    14857 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/generators/xml_generator.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.040392 mimeograph-1.0.3/src/mimeo/logging/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2023-05-16 15:27:55.000000 mimeograph-1.0.3/src/mimeo/logging/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1743 2023-05-11 05:33:09.000000 mimeograph-1.0.3/src/mimeo/logging/filters.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.040392 mimeograph-1.0.3/src/mimeo/meta/
--rw-rw-r--   0 tom       (1000) tom       (1000)      652 2023-05-11 05:33:09.000000 mimeograph-1.0.3/src/mimeo/meta/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4083 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/meta/alive.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      656 2023-05-17 13:09:43.000000 mimeograph-1.0.3/src/mimeo/meta/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10889 2023-06-26 13:54:19.000000 mimeograph-1.0.3/src/mimeo/mimeo.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.040392 mimeograph-1.0.3/src/mimeo/resources/
--rw-rw-r--   0 tom       (1000) tom       (1000)      362 2023-05-17 13:09:43.000000 mimeograph-1.0.3/src/mimeo/resources/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)  1541655 2023-06-26 14:29:14.000000 mimeograph-1.0.3/src/mimeo/resources/cities.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     1579 2023-06-20 06:50:14.000000 mimeograph-1.0.3/src/mimeo/resources/constants.yaml
--rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-06-26 14:08:58.000000 mimeograph-1.0.3/src/mimeo/resources/countries.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     7268 2023-06-26 14:29:14.000000 mimeograph-1.0.3/src/mimeo/resources/currencies.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      783 2023-05-17 13:09:43.000000 mimeograph-1.0.3/src/mimeo/resources/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    66313 2023-06-26 14:05:34.000000 mimeograph-1.0.3/src/mimeo/resources/forenames.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      736 2023-06-26 13:54:19.000000 mimeograph-1.0.3/src/mimeo/resources/logging.yaml
--rw-rw-r--   0 tom       (1000) tom       (1000)  1197769 2023-06-26 14:05:38.000000 mimeograph-1.0.3/src/mimeo/resources/surnames.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)     1035 2023-05-17 13:09:43.000000 mimeograph-1.0.3/src/mimeo/tools.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.044392 mimeograph-1.0.3/src/mimeo/utils/
--rw-rw-r--   0 tom       (1000) tom       (1000)     2193 2023-05-16 10:04:29.000000 mimeograph-1.0.3/src/mimeo/utils/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6254 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/utils/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    29523 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/utils/mimeo_utils.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    20193 2023-06-23 07:36:58.000000 mimeograph-1.0.3/src/mimeo/utils/renderers.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.044392 mimeograph-1.0.3/src/mimeograph.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)    34465 2023-06-26 15:57:24.000000 mimeograph-1.0.3/src/mimeograph.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     2043 2023-06-26 15:57:24.000000 mimeograph-1.0.3/src/mimeograph.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-06-26 15:57:24.000000 mimeograph-1.0.3/src/mimeograph.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-06-26 15:57:24.000000 mimeograph-1.0.3/src/mimeograph.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)      222 2023-06-26 15:57:24.000000 mimeograph-1.0.3/src/mimeograph.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-06-26 15:57:24.000000 mimeograph-1.0.3/src/mimeograph.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-26 15:57:24.044392 mimeograph-1.0.3/tests/
--rw-rw-r--   0 tom       (1000) tom       (1000)    16690 2023-06-26 13:54:19.000000 mimeograph-1.0.3/tests/test_mimeograph.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      502 2023-05-22 07:52:53.000000 mimeograph-1.0.3/tests/test_tools.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.614524 mimeograph-1.0.4/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-1.0.4/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)       30 2023-05-11 05:33:09.000000 mimeograph-1.0.4/MANIFEST.in
+-rw-rw-r--   0 tom       (1000) tom       (1000)    34465 2023-06-27 07:06:54.610523 mimeograph-1.0.4/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)    32079 2023-06-26 13:54:19.000000 mimeograph-1.0.4/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4010 2023-06-27 07:06:22.000000 mimeograph-1.0.4/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-06-27 07:06:54.614524 mimeograph-1.0.4/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.606523 mimeograph-1.0.4/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.606523 mimeograph-1.0.4/src/mimeo/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1484 2023-06-27 07:06:22.000000 mimeograph-1.0.4/src/mimeo/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      408 2023-06-24 11:03:12.000000 mimeograph-1.0.4/src/mimeo/__main__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.606523 mimeograph-1.0.4/src/mimeo/cli/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      761 2023-05-11 05:33:09.000000 mimeograph-1.0.4/src/mimeo/cli/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2290 2023-05-17 08:57:29.000000 mimeograph-1.0.4/src/mimeo/cli/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4694 2023-06-26 13:54:19.000000 mimeograph-1.0.4/src/mimeo/cli/job.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18152 2023-06-27 07:06:22.000000 mimeograph-1.0.4/src/mimeo/cli/parsers.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.606523 mimeograph-1.0.4/src/mimeo/config/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      837 2023-05-27 06:14:50.000000 mimeograph-1.0.4/src/mimeo/config/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6275 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/config/constants.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    12351 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/config/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    35693 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/config/mimeo_config.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.606523 mimeograph-1.0.4/src/mimeo/consumers/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1322 2023-05-11 05:33:09.000000 mimeograph-1.0.4/src/mimeo/consumers/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1402 2023-06-24 11:02:10.000000 mimeograph-1.0.4/src/mimeo/consumers/consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2146 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/consumers/consumer_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2374 2023-06-24 11:02:23.000000 mimeograph-1.0.4/src/mimeo/consumers/file_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3109 2023-06-26 13:54:19.000000 mimeograph-1.0.4/src/mimeo/consumers/http_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1018 2023-05-12 09:42:23.000000 mimeograph-1.0.4/src/mimeo/consumers/raw_consumer.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.606523 mimeograph-1.0.4/src/mimeo/context/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1001 2023-05-11 05:33:09.000000 mimeograph-1.0.4/src/mimeo/context/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4261 2023-05-11 05:33:09.000000 mimeograph-1.0.4/src/mimeo/context/decorators.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5087 2023-05-11 05:33:09.000000 mimeograph-1.0.4/src/mimeo/context/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18276 2023-06-23 11:30:49.000000 mimeograph-1.0.4/src/mimeo/context/mimeo_context.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5164 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/context/mimeo_context_manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2911 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/context/mimeo_iteration.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.606523 mimeograph-1.0.4/src/mimeo/database/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1805 2023-05-16 10:04:29.000000 mimeograph-1.0.4/src/mimeo/database/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5638 2023-06-27 07:03:27.000000 mimeograph-1.0.4/src/mimeo/database/cities.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5885 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/database/countries.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5755 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/database/currencies.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6200 2023-05-22 07:52:53.000000 mimeograph-1.0.4/src/mimeo/database/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5599 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/database/first_names.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2235 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/database/last_names.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10234 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/database/mimeo_db.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      702 2023-06-26 13:54:19.000000 mimeograph-1.0.4/src/mimeo/exc.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.610523 mimeograph-1.0.4/src/mimeo/generators/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1221 2023-06-20 06:50:14.000000 mimeograph-1.0.4/src/mimeo/generators/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1149 2023-06-20 06:50:14.000000 mimeograph-1.0.4/src/mimeo/generators/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10680 2023-06-26 13:54:19.000000 mimeograph-1.0.4/src/mimeo/generators/generator.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1852 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/generators/generator_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    17137 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/generators/json_generator.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    14857 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/generators/xml_generator.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.610523 mimeograph-1.0.4/src/mimeo/logging/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2023-05-16 15:27:55.000000 mimeograph-1.0.4/src/mimeo/logging/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1743 2023-05-11 05:33:09.000000 mimeograph-1.0.4/src/mimeo/logging/filters.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.610523 mimeograph-1.0.4/src/mimeo/meta/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      652 2023-05-11 05:33:09.000000 mimeograph-1.0.4/src/mimeo/meta/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4083 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/meta/alive.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      656 2023-05-17 13:09:43.000000 mimeograph-1.0.4/src/mimeo/meta/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10889 2023-06-26 13:54:19.000000 mimeograph-1.0.4/src/mimeo/mimeo.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.610523 mimeograph-1.0.4/src/mimeo/resources/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      362 2023-05-17 13:09:43.000000 mimeograph-1.0.4/src/mimeo/resources/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1541630 2023-06-27 07:03:27.000000 mimeograph-1.0.4/src/mimeo/resources/cities.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1579 2023-06-20 06:50:14.000000 mimeograph-1.0.4/src/mimeo/resources/constants.yaml
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-06-27 06:51:54.000000 mimeograph-1.0.4/src/mimeo/resources/countries.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7267 2023-06-27 07:03:27.000000 mimeograph-1.0.4/src/mimeo/resources/currencies.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      783 2023-05-17 13:09:43.000000 mimeograph-1.0.4/src/mimeo/resources/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    66313 2023-06-27 06:51:59.000000 mimeograph-1.0.4/src/mimeo/resources/forenames.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      736 2023-06-26 13:54:19.000000 mimeograph-1.0.4/src/mimeo/resources/logging.yaml
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1197769 2023-06-27 06:52:05.000000 mimeograph-1.0.4/src/mimeo/resources/surnames.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1035 2023-05-17 13:09:43.000000 mimeograph-1.0.4/src/mimeo/tools.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.610523 mimeograph-1.0.4/src/mimeo/utils/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2193 2023-05-16 10:04:29.000000 mimeograph-1.0.4/src/mimeo/utils/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6254 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/utils/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    29523 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/utils/mimeo_utils.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    20193 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/utils/renderers.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.610523 mimeograph-1.0.4/src/mimeograph.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    34465 2023-06-27 07:06:54.000000 mimeograph-1.0.4/src/mimeograph.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2043 2023-06-27 07:06:54.000000 mimeograph-1.0.4/src/mimeograph.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-06-27 07:06:54.000000 mimeograph-1.0.4/src/mimeograph.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-06-27 07:06:54.000000 mimeograph-1.0.4/src/mimeograph.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)      222 2023-06-27 07:06:54.000000 mimeograph-1.0.4/src/mimeograph.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-06-27 07:06:54.000000 mimeograph-1.0.4/src/mimeograph.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.610523 mimeograph-1.0.4/tests/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    16690 2023-06-26 13:54:19.000000 mimeograph-1.0.4/tests/test_mimeograph.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      502 2023-05-22 07:52:53.000000 mimeograph-1.0.4/tests/test_tools.py
```

### Comparing `mimeograph-1.0.3/LICENSE` & `mimeograph-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/PKG-INFO` & `mimeograph-1.0.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeograph
-Version: 1.0.3
+Version: 1.0.4
 Summary: Generate NoSQL data based on a simple template
 Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Aniołowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mimeograph Version: 1.0.3 Summary: Generate NoSQL
+Metadata-Version: 2.1 Name: mimeograph Version: 1.0.4 Summary: Generate NoSQL
 data based on a simple template Author-email: "T.A. Programming Svcs."
 maciej.aniolowski@gmail.com> License: MIT License Copyright (c) 2023 Tomasz
 AnioÅowski Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
```

### Comparing `mimeograph-1.0.3/README.md` & `mimeograph-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/pyproject.toml` & `mimeograph-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mimeograph"
-version = "1.0.3"
+version = "1.0.4"
 description = "Generate NoSQL data based on a simple template"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{ name = "T.A. Programming Svcs.", email = "tomasz.maciej.aniolowski@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -61,15 +61,15 @@
     "pytest-asyncio"
 ]
 
 [project.scripts]
 mimeo = "mimeo.__main__:main"
 
 [tool.bumpver]
-current_version = "1.0.3"
+current_version = "1.0.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} to {new_version}"
 commit          = true
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `mimeograph-1.0.3/src/mimeo/__init__.py` & `mimeograph-1.0.4/src/mimeo/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,9 +48,9 @@
     from mimeo import MimeoConfig, Mimeograph
 """
 from __future__ import annotations
 
 from .config import MimeoConfig, MimeoConfigFactory
 from .mimeo import Mimeograph
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 __all__ = ["MimeoConfig", "MimeoConfigFactory", "Mimeograph"]
```

### Comparing `mimeograph-1.0.3/src/mimeo/cli/__init__.py` & `mimeograph-1.0.4/src/mimeo/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/cli/exc.py` & `mimeograph-1.0.4/src/mimeo/cli/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/cli/job.py` & `mimeograph-1.0.4/src/mimeo/cli/job.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/cli/parsers.py` & `mimeograph-1.0.4/src/mimeo/cli/parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             self,
     ):
         """Add positional arguments."""
         self.add_argument(
             "-v",
             "--version",
             action="version",
-            version="%(prog)s v1.0.3")
+            version="%(prog)s v1.0.4")
         self.add_argument(
             "paths",
             nargs="+",
             type=str,
             help="take paths to Mimeo Configuration files")
 
     def _add_mimeo_configuration_arguments(
```

### Comparing `mimeograph-1.0.3/src/mimeo/config/__init__.py` & `mimeograph-1.0.4/src/mimeo/config/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/config/constants.py` & `mimeograph-1.0.4/src/mimeo/config/constants.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/config/exc.py` & `mimeograph-1.0.4/src/mimeo/config/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/config/mimeo_config.py` & `mimeograph-1.0.4/src/mimeo/config/mimeo_config.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/consumers/__init__.py` & `mimeograph-1.0.4/src/mimeo/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/consumers/consumer.py` & `mimeograph-1.0.4/src/mimeo/consumers/consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/consumers/consumer_factory.py` & `mimeograph-1.0.4/src/mimeo/consumers/consumer_factory.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/consumers/file_consumer.py` & `mimeograph-1.0.4/src/mimeo/consumers/file_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/consumers/http_consumer.py` & `mimeograph-1.0.4/src/mimeo/consumers/http_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/consumers/raw_consumer.py` & `mimeograph-1.0.4/src/mimeo/consumers/raw_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/context/__init__.py` & `mimeograph-1.0.4/src/mimeo/context/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/context/decorators.py` & `mimeograph-1.0.4/src/mimeo/context/decorators.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/context/exc.py` & `mimeograph-1.0.4/src/mimeo/context/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/context/mimeo_context.py` & `mimeograph-1.0.4/src/mimeo/context/mimeo_context.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/context/mimeo_context_manager.py` & `mimeograph-1.0.4/src/mimeo/context/mimeo_context_manager.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/context/mimeo_iteration.py` & `mimeograph-1.0.4/src/mimeo/context/mimeo_iteration.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/database/__init__.py` & `mimeograph-1.0.4/src/mimeo/database/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/database/cities.py` & `mimeograph-1.0.4/src/mimeo/database/cities.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         Get all cities.
     get_cities_of(country_iso3: str) -> list[City]
         Get cities of a specific country.
     get_city_at(index: int) -> City
         Get a city at `index` position.
     """
 
-    NUM_OF_RECORDS: int = 42905
+    NUM_OF_RECORDS: int = 42904
     _CITIES_DB: str = "cities.csv"
     _CITIES_DF: DataFrame = None
     _CITIES: ClassVar[list] = None
     _COUNTRY_CITIES: ClassVar[dict] = {}
 
     def get_city_at(
             self,
```

### Comparing `mimeograph-1.0.3/src/mimeo/database/countries.py` & `mimeograph-1.0.4/src/mimeo/database/countries.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/database/currencies.py` & `mimeograph-1.0.4/src/mimeo/database/currencies.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/database/exc.py` & `mimeograph-1.0.4/src/mimeo/database/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/database/first_names.py` & `mimeograph-1.0.4/src/mimeo/database/first_names.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/database/last_names.py` & `mimeograph-1.0.4/src/mimeo/database/last_names.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/database/mimeo_db.py` & `mimeograph-1.0.4/src/mimeo/database/mimeo_db.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/exc.py` & `mimeograph-1.0.4/src/mimeo/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/generators/__init__.py` & `mimeograph-1.0.4/src/mimeo/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/generators/exc.py` & `mimeograph-1.0.4/src/mimeo/generators/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/generators/generator.py` & `mimeograph-1.0.4/src/mimeo/generators/generator.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/generators/generator_factory.py` & `mimeograph-1.0.4/src/mimeo/generators/generator_factory.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/generators/json_generator.py` & `mimeograph-1.0.4/src/mimeo/generators/json_generator.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/generators/xml_generator.py` & `mimeograph-1.0.4/src/mimeo/generators/xml_generator.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/logging/__init__.py` & `mimeograph-1.0.4/src/mimeo/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/logging/filters.py` & `mimeograph-1.0.4/src/mimeo/logging/filters.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/meta/__init__.py` & `mimeograph-1.0.4/src/mimeo/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/meta/alive.py` & `mimeograph-1.0.4/src/mimeo/meta/alive.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/meta/exc.py` & `mimeograph-1.0.4/src/mimeo/meta/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/mimeo.py` & `mimeograph-1.0.4/src/mimeo/mimeo.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/resources/cities.csv` & `mimeograph-1.0.4/src/mimeo/resources/cities.csv`

 * *Files 0% similar despite different names*

```diff
@@ -19152,15 +19152,14 @@
 1380596300,Bagnolo Piemonte,Bagnolo Piemonte,ITA
 1380596593,Borgaro Torinese,Borgaro Torinese,ITA
 1380596606,Lanciano,Lanciano,ITA
 1380597324,Ancona,Ancona,ITA
 1380598450,Brugine,Brugine,ITA
 1380599278,Cazzago San Martino,Cazzago San Martino,ITA
 1380600468,Minturno,Minturno,ITA
-1380601372,None,None,ITA
 1380601560,Alberobello,Alberobello,ITA
 1380602837,Adelfia,Adelfia,ITA
 1380603196,Mercogliano,Mercogliano,ITA
 1380604533,Monte Libretti,Monte Libretti,ITA
 1380605395,Ribera,Ribera,ITA
 1380605437,Noto,Noto,ITA
 1380605846,Castel Maggiore,Castel Maggiore,ITA
```

### Comparing `mimeograph-1.0.3/src/mimeo/resources/constants.yaml` & `mimeograph-1.0.4/src/mimeo/resources/constants.yaml`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/resources/countries.csv` & `mimeograph-1.0.4/src/mimeo/resources/countries.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/resources/currencies.csv` & `mimeograph-1.0.4/src/mimeo/resources/currencies.csv`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 UGX,Uganda Shilling,['Uganda']
 USD,US Dollar,"['American Samoa', 'Bonaire, Sint Eustatius And Saba', 'British Indian Ocean Territory', 'Ecuador', 'El Salvador', 'Guam', 'Haiti', 'Marshall Islands', 'Micronesia (Federated States Of)', 'Northern Mariana Islands', 'Palau', 'Panama', 'Puerto Rico', 'Timor-Leste', 'Turks And Caicos Islands', 'United States Minor Outlying Islands', 'United States Of America', 'Virgin Islands (British)', 'Virgin Islands (U.S.)']"
 USN,US Dollar (Next day),['United States Of America']
 UYI,Uruguay Peso en Unidades Indexadas (UI),['Uruguay']
 UYU,Peso Uruguayo,['Uruguay']
 UYW,Unidad Previsional,['Uruguay']
 UZS,Uzbekistan Sum,['Uzbekistan']
-VES,Bolívar Soberano,['Venezuela (Bolivarian Republic Of)']
+VES,Bolivar Soberano,['Venezuela (Bolivarian Republic Of)']
 VND,Dong,['Viet Nam']
 VUV,Vatu,['Vanuatu']
 WST,Tala,['Samoa']
 XAF,CFA Franc BEAC,"['Cameroon', 'Central African Republic', 'Chad', 'Congo', 'Equatorial Guinea', 'Gabon']"
 XCD,East Caribbean Dollar,"['Anguilla', 'Antigua And Barbuda', 'Dominica', 'Grenada', 'Montserrat', 'Saint Kitts And Nevis', 'Saint Lucia', 'Saint Vincent And The Grenadines']"
 XDR,SDR (Special Drawing Right),['International Monetary Fund (Imf)']
 XOF,CFA Franc BCEAO,"['Benin', 'Burkina Faso', ""Cote D'Ivoire"", 'Guinea-Bissau', 'Mali', 'Niger', 'Senegal', 'Togo']"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mimeograph-1.0.3/src/mimeo/resources/exc.py` & `mimeograph-1.0.4/src/mimeo/resources/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/resources/forenames.csv` & `mimeograph-1.0.4/src/mimeo/resources/forenames.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/resources/logging.yaml` & `mimeograph-1.0.4/src/mimeo/resources/logging.yaml`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/resources/surnames.txt` & `mimeograph-1.0.4/src/mimeo/resources/surnames.txt`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/tools.py` & `mimeograph-1.0.4/src/mimeo/tools.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/utils/__init__.py` & `mimeograph-1.0.4/src/mimeo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/utils/exc.py` & `mimeograph-1.0.4/src/mimeo/utils/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/utils/mimeo_utils.py` & `mimeograph-1.0.4/src/mimeo/utils/mimeo_utils.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeo/utils/renderers.py` & `mimeograph-1.0.4/src/mimeo/utils/renderers.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/src/mimeograph.egg-info/PKG-INFO` & `mimeograph-1.0.4/src/mimeograph.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeograph
-Version: 1.0.3
+Version: 1.0.4
 Summary: Generate NoSQL data based on a simple template
 Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Aniołowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mimeograph Version: 1.0.3 Summary: Generate NoSQL
+Metadata-Version: 2.1 Name: mimeograph Version: 1.0.4 Summary: Generate NoSQL
 data based on a simple template Author-email: "T.A. Programming Svcs."
 maciej.aniolowski@gmail.com> License: MIT License Copyright (c) 2023 Tomasz
 AnioÅowski Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
```

### Comparing `mimeograph-1.0.3/src/mimeograph.egg-info/SOURCES.txt` & `mimeograph-1.0.4/src/mimeograph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.3/tests/test_mimeograph.py` & `mimeograph-1.0.4/tests/test_mimeograph.py`

 * *Files identical despite different names*

