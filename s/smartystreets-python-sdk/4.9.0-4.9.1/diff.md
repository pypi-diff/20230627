# Comparing `tmp/smartystreets_python_sdk-4.9.0.tar.gz` & `tmp/smartystreets_python_sdk-4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/smartystreets_python_sdk-4.9.0.tar", last modified: Thu Jul 15 16:23:39 2021, max compression
+gzip compressed data, was "dist/smartystreets_python_sdk-4.9.1.tar", last modified: Fri Aug 20 15:56:07 2021, max compression
```

## Comparing `smartystreets_python_sdk-4.9.0.tar` & `smartystreets_python_sdk-4.9.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-07-15 16:23:39.000000 smartystreets_python_sdk-4.9.0/
--rw-r--r--   0 duncan     (501) staff       (20)      868 2021-07-15 16:23:39.000000 smartystreets_python_sdk-4.9.0/PKG-INFO
-drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-07-15 16:23:39.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/
--rw-r--r--   0 duncan     (501) staff       (20)      654 2019-07-05 20:59:00.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/custom_header_sender.py
--rw-r--r--   0 duncan     (501) staff       (20)     6937 2021-05-26 21:13:24.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/client_builder.py
-drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-07-15 16:23:39.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_reverse_geo/
--rw-r--r--   0 duncan     (501) staff       (20)      352 2020-10-30 20:10:07.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_reverse_geo/address.py
--rw-r--r--   0 duncan     (501) staff       (20)     1195 2021-01-06 16:13:01.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_reverse_geo/client.py
--rw-r--r--   0 duncan     (501) staff       (20)      459 2020-10-30 20:10:07.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_reverse_geo/lookup.py
--rw-r--r--   0 duncan     (501) staff       (20)      176 2020-10-30 20:10:07.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_reverse_geo/__init__.py
--rw-r--r--   0 duncan     (501) staff       (20)      130 2020-10-30 20:10:07.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_reverse_geo/response.py
--rw-r--r--   0 duncan     (501) staff       (20)      507 2020-11-20 21:46:24.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_reverse_geo/coordinate.py
--rw-r--r--   0 duncan     (501) staff       (20)      427 2020-10-30 20:10:07.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_reverse_geo/result.py
--rw-r--r--   0 duncan     (501) staff       (20)      248 2021-05-26 20:01:13.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/shared_credentials.py
-drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-07-15 16:23:39.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_street/
--rw-r--r--   0 duncan     (501) staff       (20)     1098 2019-02-08 16:47:18.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_street/metadata.py
--rw-r--r--   0 duncan     (501) staff       (20)      846 2021-07-06 20:02:31.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_street/analysis.py
--rw-r--r--   0 duncan     (501) staff       (20)     2636 2020-08-21 21:43:45.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_street/client.py
--rw-r--r--   0 duncan     (501) staff       (20)     1036 2021-07-14 21:26:15.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_street/lookup.py
--rw-r--r--   0 duncan     (501) staff       (20)      185 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_street/__init__.py
--rw-r--r--   0 duncan     (501) staff       (20)       93 2021-07-15 16:20:28.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_street/match_type.py
--rw-r--r--   0 duncan     (501) staff       (20)     1109 2019-09-26 15:50:03.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_street/candidate.py
--rw-r--r--   0 duncan     (501) staff       (20)     1479 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_street/components.py
-drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-07-15 16:23:39.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_zipcode/
--rw-r--r--   0 duncan     (501) staff       (20)      411 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_zipcode/city.py
--rw-r--r--   0 duncan     (501) staff       (20)     2055 2019-09-26 16:20:58.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_zipcode/client.py
--rw-r--r--   0 duncan     (501) staff       (20)      536 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_zipcode/lookup.py
--rw-r--r--   0 duncan     (501) staff       (20)      179 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_zipcode/__init__.py
--rw-r--r--   0 duncan     (501) staff       (20)      938 2019-09-26 16:20:58.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_zipcode/result.py
--rw-r--r--   0 duncan     (501) staff       (20)      852 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_zipcode/zipcode.py
--rw-r--r--   0 duncan     (501) staff       (20)      353 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_zipcode/alternate_county.py
--rw-r--r--   0 duncan     (501) staff       (20)      280 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/static_credentials.py
--rw-r--r--   0 duncan     (501) staff       (20)      506 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/proxy.py
--rw-r--r--   0 duncan     (501) staff       (20)      313 2021-05-26 21:14:22.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/license_sender.py
--rw-r--r--   0 duncan     (501) staff       (20)     1371 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/batch.py
--rw-r--r--   0 duncan     (501) staff       (20)      251 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/request.py
--rw-r--r--   0 duncan     (501) staff       (20)      246 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/url_prefix_sender.py
--rw-r--r--   0 duncan     (501) staff       (20)      697 2021-03-23 16:51:56.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/__init__.py
--rw-r--r--   0 duncan     (501) staff       (20)      171 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/response.py
--rw-r--r--   0 duncan     (501) staff       (20)      220 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/signing_sender.py
-drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-07-15 16:23:39.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/international_street/
--rw-r--r--   0 duncan     (501) staff       (20)      226 2019-03-18 20:05:08.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/international_street/changes.py
--rw-r--r--   0 duncan     (501) staff       (20)      462 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/international_street/metadata.py
--rw-r--r--   0 duncan     (501) staff       (20)      437 2019-03-18 20:05:08.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/international_street/analysis.py
--rw-r--r--   0 duncan     (501) staff       (20)     2155 2021-01-06 16:13:01.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/international_street/client.py
--rw-r--r--   0 duncan     (501) staff       (20)       35 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/international_street/language_mode.py
--rw-r--r--   0 duncan     (501) staff       (20)     2719 2019-11-26 16:06:45.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/international_street/lookup.py
--rw-r--r--   0 duncan     (501) staff       (20)      759 2019-09-26 15:50:03.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/international_street/rootlevel.py
--rw-r--r--   0 duncan     (501) staff       (20)      184 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/international_street/__init__.py
--rw-r--r--   0 duncan     (501) staff       (20)      672 2019-03-18 20:05:08.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/international_street/candidate.py
--rw-r--r--   0 duncan     (501) staff       (20)     2957 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/international_street/components.py
-drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-07-15 16:23:39.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_autocomplete/
--rw-r--r--   0 duncan     (501) staff       (20)       46 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_autocomplete/geolocation_type.py
--rw-r--r--   0 duncan     (501) staff       (20)      345 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_autocomplete/suggestion.py
--rw-r--r--   0 duncan     (501) staff       (20)     2367 2021-01-06 16:13:01.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_autocomplete/client.py
--rw-r--r--   0 duncan     (501) staff       (20)     1783 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_autocomplete/lookup.py
--rw-r--r--   0 duncan     (501) staff       (20)       89 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_autocomplete/__init__.py
--rw-r--r--   0 duncan     (501) staff       (20)     2795 2021-05-26 21:17:18.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/requests_sender.py
--rw-r--r--   0 duncan     (501) staff       (20)      652 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/exceptions.py
--rw-r--r--   0 duncan     (501) staff       (20)     1197 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/errors.py
-drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-07-15 16:23:39.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_autocomplete_pro/
--rw-r--r--   0 duncan     (501) staff       (20)       29 2021-03-23 16:51:56.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_autocomplete_pro/geolocation_type.py
--rw-r--r--   0 duncan     (501) staff       (20)      451 2021-03-23 16:51:56.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_autocomplete_pro/suggestion.py
--rw-r--r--   0 duncan     (501) staff       (20)     2690 2021-05-26 20:16:56.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_autocomplete_pro/client.py
--rw-r--r--   0 duncan     (501) staff       (20)     3783 2021-03-23 16:51:56.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_autocomplete_pro/lookup.py
--rw-r--r--   0 duncan     (501) staff       (20)       89 2021-03-23 16:51:56.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_autocomplete_pro/__init__.py
--rw-r--r--   0 duncan     (501) staff       (20)     1731 2021-05-26 19:55:47.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/status_code_sender.py
--rw-r--r--   0 duncan     (501) staff       (20)      767 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/retry_sender.py
--rw-r--r--   0 duncan     (501) staff       (20)      225 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/native_serializer.py
-drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-07-15 16:23:39.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_extract/
--rw-r--r--   0 duncan     (501) staff       (20)      613 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_extract/address.py
--rw-r--r--   0 duncan     (501) staff       (20)      478 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_extract/metadata.py
--rw-r--r--   0 duncan     (501) staff       (20)     1789 2021-01-06 16:13:01.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_extract/client.py
--rw-r--r--   0 duncan     (501) staff       (20)      664 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_extract/lookup.py
--rw-r--r--   0 duncan     (501) staff       (20)      141 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_extract/__init__.py
--rw-r--r--   0 duncan     (501) staff       (20)      619 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_extract/result.py
--rw-r--r--   0 duncan     (501) staff       (20)     1670 2021-03-25 16:02:47.000000 smartystreets_python_sdk-4.9.0/setup.py
-drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-07-15 16:23:39.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk_version/
--rw-r--r--   0 duncan     (501) staff       (20)      122 2021-07-15 16:23:39.000000 smartystreets_python_sdk-4.9.0/smartystreets_python_sdk_version/__init__.py
--rw-r--r--   0 duncan     (501) staff       (20)       40 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.0/setup.cfg
+drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-08-20 15:56:07.000000 smartystreets_python_sdk-4.9.1/
+-rw-r--r--   0 duncan     (501) staff       (20)      868 2021-08-20 15:56:07.000000 smartystreets_python_sdk-4.9.1/PKG-INFO
+drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-08-20 15:56:07.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/
+-rw-r--r--   0 duncan     (501) staff       (20)      654 2019-07-05 20:59:00.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/custom_header_sender.py
+-rw-r--r--   0 duncan     (501) staff       (20)     6937 2021-05-26 21:13:24.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/client_builder.py
+drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-08-20 15:56:07.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_reverse_geo/
+-rw-r--r--   0 duncan     (501) staff       (20)      352 2020-10-30 20:10:07.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_reverse_geo/address.py
+-rw-r--r--   0 duncan     (501) staff       (20)     1195 2021-01-06 16:13:01.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_reverse_geo/client.py
+-rw-r--r--   0 duncan     (501) staff       (20)      459 2020-10-30 20:10:07.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_reverse_geo/lookup.py
+-rw-r--r--   0 duncan     (501) staff       (20)      176 2020-10-30 20:10:07.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_reverse_geo/__init__.py
+-rw-r--r--   0 duncan     (501) staff       (20)      130 2020-10-30 20:10:07.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_reverse_geo/response.py
+-rw-r--r--   0 duncan     (501) staff       (20)      507 2020-11-20 21:46:24.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_reverse_geo/coordinate.py
+-rw-r--r--   0 duncan     (501) staff       (20)      427 2020-10-30 20:10:07.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_reverse_geo/result.py
+-rw-r--r--   0 duncan     (501) staff       (20)      248 2021-05-26 20:01:13.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/shared_credentials.py
+drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-08-20 15:56:07.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_street/
+-rw-r--r--   0 duncan     (501) staff       (20)     1098 2019-02-08 16:47:18.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_street/metadata.py
+-rw-r--r--   0 duncan     (501) staff       (20)      846 2021-07-06 20:02:31.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_street/analysis.py
+-rw-r--r--   0 duncan     (501) staff       (20)     2636 2020-08-21 21:43:45.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_street/client.py
+-rw-r--r--   0 duncan     (501) staff       (20)     1036 2021-07-14 21:26:15.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_street/lookup.py
+-rw-r--r--   0 duncan     (501) staff       (20)      185 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_street/__init__.py
+-rw-r--r--   0 duncan     (501) staff       (20)       93 2021-07-15 16:20:28.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_street/match_type.py
+-rw-r--r--   0 duncan     (501) staff       (20)     1109 2019-09-26 15:50:03.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_street/candidate.py
+-rw-r--r--   0 duncan     (501) staff       (20)     1479 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_street/components.py
+drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-08-20 15:56:07.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_zipcode/
+-rw-r--r--   0 duncan     (501) staff       (20)      411 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_zipcode/city.py
+-rw-r--r--   0 duncan     (501) staff       (20)     2055 2019-09-26 16:20:58.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_zipcode/client.py
+-rw-r--r--   0 duncan     (501) staff       (20)      536 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_zipcode/lookup.py
+-rw-r--r--   0 duncan     (501) staff       (20)      179 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_zipcode/__init__.py
+-rw-r--r--   0 duncan     (501) staff       (20)      938 2019-09-26 16:20:58.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_zipcode/result.py
+-rw-r--r--   0 duncan     (501) staff       (20)      852 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_zipcode/zipcode.py
+-rw-r--r--   0 duncan     (501) staff       (20)      353 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_zipcode/alternate_county.py
+-rw-r--r--   0 duncan     (501) staff       (20)      280 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/static_credentials.py
+-rw-r--r--   0 duncan     (501) staff       (20)      506 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/proxy.py
+-rw-r--r--   0 duncan     (501) staff       (20)      313 2021-05-26 21:14:22.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/license_sender.py
+-rw-r--r--   0 duncan     (501) staff       (20)     1371 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/batch.py
+-rw-r--r--   0 duncan     (501) staff       (20)      251 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/request.py
+-rw-r--r--   0 duncan     (501) staff       (20)      246 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/url_prefix_sender.py
+-rw-r--r--   0 duncan     (501) staff       (20)      697 2021-03-23 16:51:56.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/__init__.py
+-rw-r--r--   0 duncan     (501) staff       (20)      171 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/response.py
+-rw-r--r--   0 duncan     (501) staff       (20)      220 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/signing_sender.py
+drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-08-20 15:56:07.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/international_street/
+-rw-r--r--   0 duncan     (501) staff       (20)      226 2019-03-18 20:05:08.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/international_street/changes.py
+-rw-r--r--   0 duncan     (501) staff       (20)      462 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/international_street/metadata.py
+-rw-r--r--   0 duncan     (501) staff       (20)      437 2019-03-18 20:05:08.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/international_street/analysis.py
+-rw-r--r--   0 duncan     (501) staff       (20)     2155 2021-01-06 16:13:01.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/international_street/client.py
+-rw-r--r--   0 duncan     (501) staff       (20)       35 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/international_street/language_mode.py
+-rw-r--r--   0 duncan     (501) staff       (20)     2719 2019-11-26 16:06:45.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/international_street/lookup.py
+-rw-r--r--   0 duncan     (501) staff       (20)      759 2019-09-26 15:50:03.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/international_street/rootlevel.py
+-rw-r--r--   0 duncan     (501) staff       (20)      184 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/international_street/__init__.py
+-rw-r--r--   0 duncan     (501) staff       (20)      672 2019-03-18 20:05:08.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/international_street/candidate.py
+-rw-r--r--   0 duncan     (501) staff       (20)     2957 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/international_street/components.py
+drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-08-20 15:56:07.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_autocomplete/
+-rw-r--r--   0 duncan     (501) staff       (20)       46 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_autocomplete/geolocation_type.py
+-rw-r--r--   0 duncan     (501) staff       (20)      345 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_autocomplete/suggestion.py
+-rw-r--r--   0 duncan     (501) staff       (20)     2367 2021-01-06 16:13:01.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_autocomplete/client.py
+-rw-r--r--   0 duncan     (501) staff       (20)     1783 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_autocomplete/lookup.py
+-rw-r--r--   0 duncan     (501) staff       (20)       89 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_autocomplete/__init__.py
+-rw-r--r--   0 duncan     (501) staff       (20)     2795 2021-05-26 21:17:18.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/requests_sender.py
+-rw-r--r--   0 duncan     (501) staff       (20)      652 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/exceptions.py
+-rw-r--r--   0 duncan     (501) staff       (20)     1197 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/errors.py
+drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-08-20 15:56:07.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_autocomplete_pro/
+-rw-r--r--   0 duncan     (501) staff       (20)       29 2021-03-23 16:51:56.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_autocomplete_pro/geolocation_type.py
+-rw-r--r--   0 duncan     (501) staff       (20)      451 2021-03-23 16:51:56.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_autocomplete_pro/suggestion.py
+-rw-r--r--   0 duncan     (501) staff       (20)     2690 2021-05-26 20:16:56.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_autocomplete_pro/client.py
+-rw-r--r--   0 duncan     (501) staff       (20)     3783 2021-03-23 16:51:56.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_autocomplete_pro/lookup.py
+-rw-r--r--   0 duncan     (501) staff       (20)       89 2021-03-23 16:51:56.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_autocomplete_pro/__init__.py
+-rw-r--r--   0 duncan     (501) staff       (20)     1731 2021-05-26 19:55:47.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/status_code_sender.py
+-rw-r--r--   0 duncan     (501) staff       (20)      767 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/retry_sender.py
+-rw-r--r--   0 duncan     (501) staff       (20)      225 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/native_serializer.py
+drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-08-20 15:56:07.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_extract/
+-rw-r--r--   0 duncan     (501) staff       (20)      613 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_extract/address.py
+-rw-r--r--   0 duncan     (501) staff       (20)      478 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_extract/metadata.py
+-rw-r--r--   0 duncan     (501) staff       (20)     1789 2021-01-06 16:13:01.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_extract/client.py
+-rw-r--r--   0 duncan     (501) staff       (20)      664 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_extract/lookup.py
+-rw-r--r--   0 duncan     (501) staff       (20)      141 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_extract/__init__.py
+-rw-r--r--   0 duncan     (501) staff       (20)      619 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_extract/result.py
+-rw-r--r--   0 duncan     (501) staff       (20)     1670 2021-03-25 16:02:47.000000 smartystreets_python_sdk-4.9.1/setup.py
+drwxr-xr-x   0 duncan     (501) staff       (20)        0 2021-08-20 15:56:07.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk_version/
+-rw-r--r--   0 duncan     (501) staff       (20)      122 2021-08-20 15:56:07.000000 smartystreets_python_sdk-4.9.1/smartystreets_python_sdk_version/__init__.py
+-rw-r--r--   0 duncan     (501) staff       (20)       40 2019-02-07 17:52:41.000000 smartystreets_python_sdk-4.9.1/setup.cfg
```

### Comparing `smartystreets_python_sdk-4.9.0/PKG-INFO` & `smartystreets_python_sdk-4.9.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: smartystreets_python_sdk
-Version: 4.9.0
+Version: 4.9.1
 Summary: An official library to help Python developers easily access the SmartyStreets APIs
 Home-page: https://github.com/smartystreets/smartystreets-python-sdk
 Author: SmartyStreets SDK Team
 Author-email: support@smartystreets.com
 License: Apache 2
-Download-URL: https://github.com/smartystreets/smartystreets-python-sdk/tarball/4.9.0
+Download-URL: https://github.com/smartystreets/smartystreets-python-sdk/tarball/4.9.1
 Description: Official Python library for SmartyStreets
 Keywords: smartystreets,smarty,address,validation,verification,street,sdk,library,geocode
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
```

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/custom_header_sender.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/custom_header_sender.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/client_builder.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/client_builder.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_reverse_geo/client.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_reverse_geo/client.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_street/metadata.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_street/metadata.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_street/analysis.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_street/analysis.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_street/client.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_street/client.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_street/lookup.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_street/lookup.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_street/candidate.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_street/candidate.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_street/components.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_street/components.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_zipcode/client.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_zipcode/client.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_zipcode/lookup.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_zipcode/lookup.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_zipcode/result.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_zipcode/result.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_zipcode/zipcode.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_zipcode/zipcode.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/batch.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/batch.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/__init__.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/international_street/client.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/international_street/client.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/international_street/lookup.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/international_street/lookup.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/international_street/rootlevel.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/international_street/rootlevel.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/international_street/candidate.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/international_street/candidate.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/international_street/components.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/international_street/components.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_autocomplete/client.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_autocomplete/client.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_autocomplete/lookup.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_autocomplete/lookup.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/requests_sender.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/requests_sender.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/exceptions.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/errors.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_autocomplete_pro/client.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_autocomplete_pro/client.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_autocomplete_pro/lookup.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_autocomplete_pro/lookup.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/status_code_sender.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/status_code_sender.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/retry_sender.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/retry_sender.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_extract/address.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_extract/address.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_extract/client.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_extract/client.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_extract/lookup.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_extract/lookup.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/smartystreets_python_sdk/us_extract/result.py` & `smartystreets_python_sdk-4.9.1/smartystreets_python_sdk/us_extract/result.py`

 * *Files identical despite different names*

### Comparing `smartystreets_python_sdk-4.9.0/setup.py` & `smartystreets_python_sdk-4.9.1/setup.py`

 * *Files identical despite different names*

