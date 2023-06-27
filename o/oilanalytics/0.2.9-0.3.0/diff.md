# Comparing `tmp/oilanalytics-0.2.9.tar.gz` & `tmp/oilanalytics-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oilanalytics-0.2.9.tar", last modified: Mon May 30 14:11:42 2022, max compression
+gzip compressed data, was "oilanalytics-0.3.0.tar", last modified: Tue Jun 27 15:44:55 2023, max compression
```

## Comparing `oilanalytics-0.2.9.tar` & `oilanalytics-0.3.0.tar`

### file list

```diff
@@ -1,66 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:42.798296 oilanalytics-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-05-30 14:11:42.798296 oilanalytics-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:42.794296 oilanalytics-0.2.9/notebooks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/notebooks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:42.794296 oilanalytics-0.2.9/oilanalytics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:42.794296 oilanalytics-0.2.9/oilanalytics/balances/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/balances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/balances/balance_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3065 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/balances/balance_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7601 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/balances/global_oil_balances.py
--rw-r--r--   0 runner    (1001) docker     (121)     2028 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/balances/key_agency_comparisons.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:42.794296 oilanalytics-0.2.9/oilanalytics/eia/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/eia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/eia/eia.py
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/eia/steo.py
--rw-r--r--   0 runner    (1001) docker     (121)     7098 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/eia/weeklypetreport.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:42.794296 oilanalytics-0.2.9/oilanalytics/energyaspects/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/energyaspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/energyaspects/china_stats.py
--rw-r--r--   0 runner    (1001) docker     (121)     3941 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/energyaspects/tars.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:42.794296 oilanalytics-0.2.9/oilanalytics/euroilstock/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/euroilstock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2215 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/euroilstock/euroilstock.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:42.794296 oilanalytics-0.2.9/oilanalytics/geo/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/geo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:42.794296 oilanalytics-0.2.9/oilanalytics/highfreq/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/highfreq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/highfreq/ara.py
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/highfreq/singapore.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:42.798296 oilanalytics-0.2.9/oilanalytics/iea/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/iea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/iea/omr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:42.798296 oilanalytics-0.2.9/oilanalytics/jodi/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/jodi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/jodi/jodiapi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:42.798296 oilanalytics-0.2.9/oilanalytics/opec/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/opec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2309 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/opec/momr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:42.798296 oilanalytics-0.2.9/oilanalytics/prices/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6567 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/prices/futures_prices.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:42.798296 oilanalytics-0.2.9/oilanalytics/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2355 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/utils/chartutils.py
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/utils/eikonutils.py
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/oilanalytics/utils/fileutils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:42.794296 oilanalytics-0.2.9/oilanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-05-30 14:11:42.000000 oilanalytics-0.2.9/oilanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-05-30 14:11:42.000000 oilanalytics-0.2.9/oilanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-30 14:11:42.000000 oilanalytics-0.2.9/oilanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-05-30 14:11:42.000000 oilanalytics-0.2.9/oilanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-30 14:11:42.000000 oilanalytics-0.2.9/oilanalytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-30 14:11:42.798296 oilanalytics-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:42.798296 oilanalytics-0.2.9/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/test/test_ea_reports.py
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/test/test_eia.py
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/test/test_eia_weekly_rep.py
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/test/test_futures_prices.py
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/test/test_highfreq.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/test/test_iea.py
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/test/test_key_agency_comparison.py
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-05-30 14:11:30.000000 oilanalytics-0.2.9/test/test_opec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.833706 oilanalytics-0.3.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/notebooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.833706 oilanalytics-0.3.0/oilanalytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.833706 oilanalytics-0.3.0/oilanalytics/balances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/balances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/balances/balance_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/balances/balance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/balances/global_oil_balances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/balances/key_agency_comparisons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.833706 oilanalytics-0.3.0/oilanalytics/eia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/eia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/eia/eia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/eia/monthly_drilling_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/eia/steo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/eia/weeklypetreport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/oilanalytics/energyaspects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/energyaspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/energyaspects/china_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/energyaspects/europe_diesel_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/energyaspects/fsu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/energyaspects/tars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/oilanalytics/euroilstock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/euroilstock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/euroilstock/euroilstock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/oilanalytics/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/geo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/oilanalytics/highfreq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/highfreq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/highfreq/ara.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/highfreq/singapore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/oilanalytics/iea/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/iea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/iea/omr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/oilanalytics/jodi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/jodi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/jodi/jodiapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/oilanalytics/opec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/opec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/opec/momr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/oilanalytics/prices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/prices/futures_prices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/oilanalytics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/utils/chartutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/utils/eikonutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/utils/fileutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.833706 oilanalytics-0.3.0/oilanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-27 15:44:55.000000 oilanalytics-0.3.0/oilanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-27 15:44:55.000000 oilanalytics-0.3.0/oilanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 15:44:55.000000 oilanalytics-0.3.0/oilanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 15:44:55.000000 oilanalytics-0.3.0/oilanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 15:44:55.000000 oilanalytics-0.3.0/oilanalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/test/test_ea_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/test/test_eia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/test/test_eia_weekly_rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/test/test_futures_prices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/test/test_highfreq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/test/test_iea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/test/test_key_agency_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/test/test_opec.py
```

### Comparing `oilanalytics-0.2.9/oilanalytics/balances/balance_utils.py` & `oilanalytics-0.3.0/oilanalytics/balances/balance_utils.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.2.9/oilanalytics/balances/global_oil_balances.py` & `oilanalytics-0.3.0/oilanalytics/balances/global_oil_balances.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.2.9/oilanalytics/balances/key_agency_comparisons.py` & `oilanalytics-0.3.0/oilanalytics/balances/key_agency_comparisons.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.2.9/oilanalytics/eia/eia.py` & `oilanalytics-0.3.0/oilanalytics/eia/eia.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import typing as t
+from deprecated import deprecated
 from functools import reduce
 
+
+
 import pandas as pd
 from dotenv import load_dotenv
 from eiapy import Category, MultiSeries
 
 # Load environmental variables from '.env' file.
 load_dotenv()
 
-
+@deprecated(reason="EIAPY doesn't support V2 API.")
 def extract_dataframe(data: list, series_id: str, freq: str = "M") -> pd.DataFrame:
     df = pd.DataFrame(data, columns=["date", series_id]).set_index("date")
     f = None
     if freq == "M":
         f = "%Y%m"
     df.index = pd.to_datetime(df.index, format=f)
     return df
 
 
+@deprecated(reason="EIAPY doesn't support V2 API.")
 def get_data(series_ids: t.Tuple[str], last=10) -> pd.DataFrame:
     """
     Given a list of EIA series Id, call api, get the data and return as a DataFrame
     :param series_ids:
     :param last: how many data points going back are required
     :return:
     """
@@ -33,14 +37,15 @@
         ),
         dfs,
     )
     dfs.attrs["meta"] = {x["series_id"]: x for x in res["series"]}
     return dfs
 
 
+@deprecated(reason="EIAPY doesn't support V2 API.")
 def child_series(category_ids: t.Tuple[int], freq_filter: str = None) -> list:
     """
     Given a list of EIA category ids, get a list of series_ids that make up those categories
     :param category_ids:
     :param freq_filter: filter for frequency eg annual, monthly, quarterly
     :return:
     """
```

### Comparing `oilanalytics-0.2.9/oilanalytics/eia/steo.py` & `oilanalytics-0.3.0/oilanalytics/eia/steo.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.2.9/oilanalytics/eia/weeklypetreport.py` & `oilanalytics-0.3.0/oilanalytics/eia/weeklypetreport.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+import re
+from datetime import datetime
+from commodutil import pandasutil as pdu
 import pandas as pd
+import urllib3
 from commodplot import jinjautils as ju
 from commodplot.messaging import compose_and_send_jinja_report
 from excel_scraper import excel_scraper
-from datetime import datetime
-import urllib3
-import re
+
 from oilanalytics.utils import chartutils as cu
 
 fileloc = "https://ir.eia.gov/wpsr/psw09.xls"
 
+canada_importa_file_loc = (
+    "https://www.eia.gov/dnav/pet/hist_xls/W_EPC0_IM0_NUS-NCA_MBBLDw.xls"
+)
+
 eia_url = "https://www.eia.gov/opendata/qb.php?sdid=PET.%s.W"
 
 sheets_to_parse = [
     "Contents",
     "Data 1",
     "Data 2",
     "Data 3",
@@ -39,14 +45,21 @@
     for tab in sheets_to_parse:
         if "Data" in tab:
             d = ex.parse(tab, skiprows=[0]).head(1).iloc[0].to_dict()
             symbols = {**symbols, **d}
     return symbols
 
 
+def read_canada_imports():
+    df = excel_scraper.read_table(
+        canada_importa_file_loc, sheet_name="Data 1", skiprows=(0, 2), index_col=0
+    )
+    return df
+
+
 def read_report() -> pd.DataFrame:
     """
     Read all the timeseries in the report
     :return:
     """
     ex = excel_scraper.read_excel_file(fileloc)
     dfs = []
@@ -87,14 +100,16 @@
     ) * 100
     res["Dist Yield"] = (res["WDIRPUS2"] / res["WCRRIUS2"]) * 100
 
     res["mogas_dc"] = (res["WGTSTUS1"] / res["WGFUPUS2"]).rolling(window=4).mean()
     res["distillate_dc"] = (res["WDISTUS1"] / res["WDIRPUS2"]).rolling(window=4).mean()
     res["jet_dc"] = (res["WKJSTUS1"] / res["WKJUPUS2"]).rolling(window=4).mean()
 
+    res = pdu.mergets(res, read_canada_imports())
+
     return res, release_date
 
 
 def gen_page(
     title: str, template: str, filename: str = None, report_data: pd.DataFrame = None
 ):
     data = {"name": title, "title": title, "eia_url": eia_url}
```

### Comparing `oilanalytics-0.2.9/oilanalytics/energyaspects/china_stats.py` & `oilanalytics-0.3.0/oilanalytics/energyaspects/china_stats.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,73 @@
 import logging as logger
 from datetime import datetime
-from oilanalytics.utils import chartutils as cu
+
 from commodplot import jinjautils as ju
 from pyenergyaspects import eaapi
-import os
+
+from oilanalytics.utils import chartutils as cu
+
+china_stat_ids = [
+    3333,
+    3334,
+    3335,
+    3336,
+    3337,
+    3325,
+    3326,
+    3329,
+    3338,
+    3339,
+    3340,
+    3341,
+    3342,
+    3343,
+    3344,
+    3345,
+    3346,
+    3347,
+    3348,
+    3349,
+    3350,
+    3351,
+    3352,
+    3330,
+    3358,
+    3359,
+    3360,
+    3361,
+    3362,
+    3363,
+    3364,
+    3365,
+    3366,
+    3367,
+    3368,
+    3369,
+    3331,
+    3332,
+    1446,
+    1481,
+    1479,
+    1480,
+    3324,
+]
 
 
 def generate_page(
     file_path: str = None,
     title_url: str = None,
 ):
     data = {
         "name": "China Stats",
         "title": "China Stats",
     }
 
     date_from = datetime(2010, 1, 1)
 
-    china_stat_ids = [
-        3333,
-        3334,
-        3335,
-        3336,
-        3337,
-        3325,
-        3326,
-        3329,
-        3338,
-        3339,
-        3340,
-        3341,
-        3342,
-        3343,
-        3344,
-        3345,
-        3346,
-        3347,
-        3348,
-        3349,
-        3350,
-        3351,
-        3352,
-        3330,
-        3358,
-        3359,
-        3360,
-        3361,
-        3362,
-        3363,
-        3364,
-        3365,
-        3366,
-        3367,
-        3368,
-        3369,
-        3331,
-        3332,
-        1446,
-        1481,
-        1479,
-        1480,
-        3324,
-    ]
     data["df"] = eaapi.read_timeseries(dataset_id=china_stat_ids, date_from=date_from)
 
     data["title_url"] = title_url
 
     logger.info(f"generated page to {file_path}")
     return ju.render_html(
         data=data,
```

### Comparing `oilanalytics-0.2.9/oilanalytics/energyaspects/tars.py` & `oilanalytics-0.3.0/oilanalytics/energyaspects/tars.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.2.9/oilanalytics/euroilstock/euroilstock.py` & `oilanalytics-0.3.0/oilanalytics/euroilstock/euroilstock.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.2.9/oilanalytics/highfreq/ara.py` & `oilanalytics-0.3.0/oilanalytics/highfreq/ara.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.2.9/oilanalytics/highfreq/singapore.py` & `oilanalytics-0.3.0/oilanalytics/highfreq/singapore.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.2.9/oilanalytics/iea/omr.py` & `oilanalytics-0.3.0/oilanalytics/iea/omr.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.2.9/oilanalytics/opec/momr.py` & `oilanalytics-0.3.0/oilanalytics/opec/momr.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.2.9/oilanalytics/prices/futures_prices.py` & `oilanalytics-0.3.0/oilanalytics/prices/futures_prices.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,24 @@
 futures_dict = {
     "FB": "Brent",
     "CL": "WTI",
     "DME.OQ": "Dubai",
     "RB.UNL": "RBOB",
     "HO": "HO",
     "FP": "ULSD",
-    "C": "Corn",
-    "S": "Soybeans",
 }
 
 crude_futures = {"FB": "Brent", "CL": "WTI", "DME.OQ": "Dubai"}
 
 default_cust_charts = {"JunJun": "JunJun", "DecDec": "DecDec"}
 
 
 @cachetools.func.ttl_cache(ttl=100 * 60)
 def get_contracts(
-    limsymbol: str, start_year: int = 2019, end_year: int = 2023
+    limsymbol: str, start_year: int = 2019, end_year: int = 2024
 ) -> pd.DataFrame:
     contracts = lim.contracts(
         limsymbol,
         start_year=2019,
         end_year=end_year,
         start_date=pd.to_datetime(str(start_year)),
     )
@@ -200,17 +198,16 @@
 
     data["m1m2"] = cpl.line_plot(df[[x for x in df.columns if "M1M2" in x]])
     data["m1m6"] = cpl.line_plot(df[[x for x in df.columns if "M1M6" in x]])
     data["m1m12"] = cpl.line_plot(df[[x for x in df.columns if "M1M12" in x]])
     if file_path:
         logger.info(f"generated structure page to {file_path}")
     return ju.render_html(
-        data,
-        data,
-        "structure.html",
+        data=data,
+        template="structure.html",
         filename=file_path,
         package_loader_name="oilanalytics.prices",
     )
 
 
 if __name__ == "__main__":
     # print(get_prices(crude_futures))
```

### Comparing `oilanalytics-0.2.9/oilanalytics/utils/chartutils.py` & `oilanalytics-0.3.0/oilanalytics/utils/chartutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,53 +96,61 @@
 000005f0: 6861 7274 280a 2020 2020 2020 2020 6466  hart(.        df
 00000600: 3d64 662c 2073 6572 6965 733d 7365 7269  =df, series=seri
 00000610: 6573 2c20 7469 746c 653d 7469 746c 652c  es, title=title,
 00000620: 2074 6974 6c65 5f75 726c 3d74 6974 6c65   title_url=title
 00000630: 5f75 726c 2c20 6869 7374 6672 6571 3d22  _url, histfreq="
 00000640: 5722 0a20 2020 2029 0a0a 0a64 6566 2067  W".    )...def g
 00000650: 656e 5f77 6f77 5f73 756d 6d61 7279 5f74  en_wow_summary_t
-00000660: 6162 6c65 2864 665f 696e 7075 7429 3a0a  able(df_input):.
-00000670: 2020 2020 2222 220a 2020 2020 6765 6e65      """.    gene
-00000680: 7269 6320 6d65 7468 6f64 2074 6f20 6372  ric method to cr
-00000690: 6561 7465 2061 2073 756d 6d61 7279 2074  eate a summary t
-000006a0: 6162 6c65 2066 6f72 2069 6e64 6976 6964  able for individ
-000006b0: 7561 6c20 6c6f 6361 7469 6f6e 2070 6167  ual location pag
-000006c0: 650a 2020 2020 3a70 6172 616d 2064 665f  e.    :param df_
-000006d0: 696e 7075 743a 2044 6174 6146 7261 6d65  input: DataFrame
-000006e0: 2074 6f20 7375 6d6d 6172 6973 652e 204d   to summarise. M
-000006f0: 7573 7420 6861 7665 2064 6174 6574 696d  ust have datetim
-00000700: 6520 696e 6465 780a 2020 2020 3a72 6574  e index.    :ret
-00000710: 7572 6e3a 2068 746d 6c20 7461 626c 6520  urn: html table 
-00000720: 636f 6e74 6169 6e69 6e67 2073 756d 6d61  containing summa
-00000730: 7279 2064 6174 610a 2020 2020 2222 220a  ry data.    """.
-00000740: 2020 2020 6466 5f73 756d 203d 2062 752e      df_sum = bu.
-00000750: 6361 6c63 756c 6174 655f 6368 616e 6765  calculate_change
-00000760: 5f66 726f 6d5f 7072 6576 5f77 6565 6b28  _from_prev_week(
-00000770: 6466 5f69 6e70 7574 290a 2020 2020 2320  df_input).    # 
-00000780: 666f 726d 6174 2074 6865 2044 6174 6146  format the DataF
-00000790: 7261 6d65 0a20 2020 2064 665f 7375 6d20  rame.    df_sum 
-000007a0: 3d20 6466 5f73 756d 2e72 6f75 6e64 2832  = df_sum.round(2
-000007b0: 290a 2020 2020 6466 5f73 756d 2e69 6e64  ).    df_sum.ind
-000007c0: 6578 2e72 656e 616d 6528 2250 726f 6475  ex.rename("Produ
-000007d0: 6374 222c 2069 6e70 6c61 6365 3d54 7275  ct", inplace=Tru
-000007e0: 6529 0a20 2020 2064 665f 7375 6d20 3d20  e).    df_sum = 
-000007f0: 6466 5f73 756d 5b0a 2020 2020 2020 2020  df_sum[.        
-00000800: 5b64 665f 7375 6d2e 636f 6c75 6d6e 735b  [df_sum.columns[
-00000810: 315d 2c20 6466 5f73 756d 2e63 6f6c 756d  1], df_sum.colum
-00000820: 6e73 5b30 5d5d 202b 2064 665f 7375 6d2e  ns[0]] + df_sum.
-00000830: 636f 6c75 6d6e 735b 323a 5d2e 746f 6c69  columns[2:].toli
-00000840: 7374 2829 0a20 2020 205d 2020 2320 7377  st().    ]  # sw
-00000850: 6170 2066 6972 7374 2032 2063 6f6c 756d  ap first 2 colum
-00000860: 6e73 0a20 2020 2064 665f 7375 6d2e 636f  ns.    df_sum.co
-00000870: 6c75 6d6e 732e 6e61 6d65 203d 204e 6f6e  lumns.name = Non
-00000880: 650a 2020 2020 6466 5f73 756d 2e69 6e64  e.    df_sum.ind
-00000890: 6578 2e6e 616d 6520 3d20 4e6f 6e65 0a20  ex.name = None. 
-000008a0: 2020 2067 6574 5f73 756d 6d61 7279 5f74     get_summary_t
-000008b0: 6162 6c65 203d 2063 706c 742e 6765 6e65  able = cplt.gene
-000008c0: 7261 7465 5f74 6162 6c65 280a 2020 2020  rate_table(.    
-000008d0: 2020 2020 6466 5f73 756d 2c20 7072 6563      df_sum, prec
-000008e0: 6973 696f 6e3d 322c 2061 6363 6f75 6e74  ision=2, account
-000008f0: 696e 675f 636f 6c5f 636f 6c75 6d6e 733d  ing_col_columns=
-00000900: 5b22 4368 616e 6765 222c 2022 2522 5d0a  ["Change", "%"].
-00000910: 2020 2020 290a 2020 2020 7265 7475 726e      ).    return
-00000920: 2067 6574 5f73 756d 6d61 7279 5f74 6162   get_summary_tab
-00000930: 6c65 0a                                  le.
+00000660: 6162 6c65 2864 665f 696e 7075 742c 2070  able(df_input, p
+00000670: 7265 6369 7369 6f6e 3d32 2c20 7369 6e67  recision=2, sing
+00000680: 6c65 5f64 6174 653d 4661 6c73 6529 3a0a  le_date=False):.
+00000690: 2020 2020 2222 220a 2020 2020 6765 6e65      """.    gene
+000006a0: 7269 6320 6d65 7468 6f64 2074 6f20 6372  ric method to cr
+000006b0: 6561 7465 2061 2073 756d 6d61 7279 2074  eate a summary t
+000006c0: 6162 6c65 2066 6f72 2069 6e64 6976 6964  able for individ
+000006d0: 7561 6c20 6c6f 6361 7469 6f6e 2070 6167  ual location pag
+000006e0: 650a 2020 2020 3a70 6172 616d 2064 665f  e.    :param df_
+000006f0: 696e 7075 743a 2044 6174 6146 7261 6d65  input: DataFrame
+00000700: 2074 6f20 7375 6d6d 6172 6973 652e 204d   to summarise. M
+00000710: 7573 7420 6861 7665 2064 6174 6574 696d  ust have datetim
+00000720: 6520 696e 6465 780a 2020 2020 3a72 6574  e index.    :ret
+00000730: 7572 6e3a 2068 746d 6c20 7461 626c 6520  urn: html table 
+00000740: 636f 6e74 6169 6e69 6e67 2073 756d 6d61  containing summa
+00000750: 7279 2064 6174 610a 2020 2020 2222 220a  ry data.    """.
+00000760: 2020 2020 6466 5f73 756d 203d 2062 752e      df_sum = bu.
+00000770: 6361 6c63 756c 6174 655f 6368 616e 6765  calculate_change
+00000780: 5f66 726f 6d5f 7072 6576 5f77 6565 6b28  _from_prev_week(
+00000790: 6466 5f69 6e70 7574 290a 2020 2020 2320  df_input).    # 
+000007a0: 666f 726d 6174 2074 6865 2044 6174 6146  format the DataF
+000007b0: 7261 6d65 0a20 2020 2064 665f 7375 6d20  rame.    df_sum 
+000007c0: 3d20 6466 5f73 756d 2e72 6f75 6e64 2832  = df_sum.round(2
+000007d0: 290a 2020 2020 6466 5f73 756d 2e69 6e64  ).    df_sum.ind
+000007e0: 6578 2e72 656e 616d 6528 2250 726f 6475  ex.rename("Produ
+000007f0: 6374 222c 2069 6e70 6c61 6365 3d54 7275  ct", inplace=Tru
+00000800: 6529 0a20 2020 2064 665f 7375 6d20 3d20  e).    df_sum = 
+00000810: 6466 5f73 756d 5b0a 2020 2020 2020 2020  df_sum[.        
+00000820: 5b64 665f 7375 6d2e 636f 6c75 6d6e 735b  [df_sum.columns[
+00000830: 315d 2c20 6466 5f73 756d 2e63 6f6c 756d  1], df_sum.colum
+00000840: 6e73 5b30 5d5d 202b 2064 665f 7375 6d2e  ns[0]] + df_sum.
+00000850: 636f 6c75 6d6e 735b 323a 5d2e 746f 6c69  columns[2:].toli
+00000860: 7374 2829 0a20 2020 205d 2020 2320 7377  st().    ]  # sw
+00000870: 6170 2066 6972 7374 2032 2063 6f6c 756d  ap first 2 colum
+00000880: 6e73 0a20 2020 2064 665f 7375 6d2e 636f  ns.    df_sum.co
+00000890: 6c75 6d6e 732e 6e61 6d65 203d 204e 6f6e  lumns.name = Non
+000008a0: 650a 2020 2020 6466 5f73 756d 2e69 6e64  e.    df_sum.ind
+000008b0: 6578 2e6e 616d 6520 3d20 4e6f 6e65 0a20  ex.name = None. 
+000008c0: 2020 2069 6620 7369 6e67 6c65 5f64 6174     if single_dat
+000008d0: 653a 0a20 2020 2020 2020 2064 665f 7375  e:.        df_su
+000008e0: 6d2e 7265 6e61 6d65 2863 6f6c 756d 6e73  m.rename(columns
+000008f0: 3d7b 6466 5f73 756d 2e63 6f6c 756d 6e73  ={df_sum.columns
+00000900: 5b31 5d3a 2022 4c61 7374 2057 6565 6b22  [1]: "Last Week"
+00000910: 7d2c 2069 6e70 6c61 6365 3d54 7275 6529  }, inplace=True)
+00000920: 0a20 2020 2067 6574 5f73 756d 6d61 7279  .    get_summary
+00000930: 5f74 6162 6c65 203d 2063 706c 742e 6765  _table = cplt.ge
+00000940: 6e65 7261 7465 5f74 6162 6c65 280a 2020  nerate_table(.  
+00000950: 2020 2020 2020 6466 5f73 756d 2c20 7072        df_sum, pr
+00000960: 6563 6973 696f 6e3d 7072 6563 6973 696f  ecision=precisio
+00000970: 6e2c 2061 6363 6f75 6e74 696e 675f 636f  n, accounting_co
+00000980: 6c5f 636f 6c75 6d6e 733d 5b22 4368 616e  l_columns=["Chan
+00000990: 6765 222c 2022 2522 5d0a 2020 2020 290a  ge", "%"].    ).
+000009a0: 0a20 2020 2072 6574 7572 6e20 6765 745f  .    return get_
+000009b0: 7375 6d6d 6172 795f 7461 626c 650a       summary_table.
```

### Comparing `oilanalytics-0.2.9/oilanalytics.egg-info/SOURCES.txt` & `oilanalytics-0.3.0/oilanalytics.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,21 @@
 oilanalytics/balances/__init__.py
 oilanalytics/balances/balance_config.py
 oilanalytics/balances/balance_utils.py
 oilanalytics/balances/global_oil_balances.py
 oilanalytics/balances/key_agency_comparisons.py
 oilanalytics/eia/__init__.py
 oilanalytics/eia/eia.py
+oilanalytics/eia/monthly_drilling_report.py
 oilanalytics/eia/steo.py
 oilanalytics/eia/weeklypetreport.py
 oilanalytics/energyaspects/__init__.py
 oilanalytics/energyaspects/china_stats.py
+oilanalytics/energyaspects/europe_diesel_balance.py
+oilanalytics/energyaspects/fsu_stats.py
 oilanalytics/energyaspects/tars.py
 oilanalytics/euroilstock/__init__.py
 oilanalytics/euroilstock/euroilstock.py
 oilanalytics/geo/__init__.py
 oilanalytics/highfreq/__init__.py
 oilanalytics/highfreq/ara.py
 oilanalytics/highfreq/singapore.py
```

### Comparing `oilanalytics-0.2.9/setup.py` & `oilanalytics-0.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="oilanalytics",
-    version="0.2.9",
+    version="0.3.0",
     author="aeorxc",
     description="Utilities for oil analytics",
     url="https://github.com/aeorxc/oilanalytics",
     project_urls={
         "Source": "https://github.com/aeorxc/oilanalytics",
     },
     packages=setuptools.find_packages(),
```

### Comparing `oilanalytics-0.2.9/test/test_eia.py` & `oilanalytics-0.3.0/test/test_eia.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import pandas as pd
-
+import pytest
 from oilanalytics.eia import eia, steo
 
 
+@pytest.mark.skip(reason="EAIPY DOESN'T SUPPORT V2 OF EIA API")
 def test_get_data_1():
     res = eia.get_data(["STEO.PATC_NON_OECD.M", "STEO.PATC_OECD.M"])
     assert "STEO.PATC_OECD.M" in res.columns
     assert "STEO.PATC_NON_OECD.M" in res.columns
     assert isinstance(res.index, pd.DatetimeIndex)
 
 
+@pytest.mark.skip(reason="EAIPY DOESN'T SUPPORT V2 OF EIA API")
 def test_get_data_2():
     res = eia.get_data(["STEO.PATC_NON_OECD.Q", "STEO.PATC_OECD.M"])
     assert "STEO.PATC_OECD.M" in res.columns
     assert isinstance(res.index, pd.DatetimeIndex)
 
 
+@pytest.mark.skip(reason="EAIPY DOESN'T SUPPORT V2 OF EIA API")
 def test_child_series():
     categs = [
         829747,  # EIA Data Sets > Short-Term Energy Outlook > International Petroleum and Other Liquids > Consumption
         829748,  # EIA Data Sets > Short-Term Energy Outlook > International Petroleum and Other Liquids > Inventories
         829751,
         # EIA Data Sets > Short-Term Energy Outlook > International Petroleum and Other Liquids > Production > Non-OPEC
         1039874,
         # EIA Data Sets > Short-Term Energy Outlook > International Petroleum and Other Liquids > Production > OPEC
     ]
     res = eia.child_series(categs, freq_filter="M")
     assert "STEO.PATC_NON_OECD.M" in [x["series_id"] for x in res]
 
 
+@pytest.mark.skip(reason="EAIPY DOESN'T SUPPORT V2 OF EIA API")
 def test_steo_get_data():
     res = steo.get_data()
     assert "STEO.PATC_NON_OECD.M" in res.columns
```

### Comparing `oilanalytics-0.2.9/test/test_highfreq.py` & `oilanalytics-0.3.0/test/test_highfreq.py`

 * *Files identical despite different names*

