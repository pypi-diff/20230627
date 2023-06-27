# Comparing `tmp/salure_helpers_azure-0.0.1.tar.gz` & `tmp/salure_helpers_azure-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_azure-0.0.1.tar", last modified: Mon Dec 19 16:11:22 2022, max compression
+gzip compressed data, was "dist/salure_helpers_azure-1.0.1.tar", last modified: Tue Jun 27 16:04:09 2023, max compression
```

## Comparing `salure_helpers_azure-0.0.1.tar` & `salure_helpers_azure-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:11:22.000000 salure_helpers_azure-0.0.1/
--rw-r--r--   0 root         (0) root         (0)      259 2022-12-19 16:11:22.000000 salure_helpers_azure-0.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:11:22.000000 salure_helpers_azure-0.0.1/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:11:22.000000 salure_helpers_azure-0.0.1/salure_helpers/azure/
--rw-rw-rw-   0 root         (0) root         (0)     5236 2022-12-19 16:11:07.000000 salure_helpers_azure-0.0.1/salure_helpers/azure/active_directory.py
--rw-rw-rw-   0 root         (0) root         (0)     4560 2022-12-19 16:11:07.000000 salure_helpers_azure-0.0.1/salure_helpers/azure/azure_connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:11:22.000000 salure_helpers_azure-0.0.1/salure_helpers_azure.egg-info/
--rw-r--r--   0 root         (0) root         (0)      259 2022-12-19 16:11:22.000000 salure_helpers_azure-0.0.1/salure_helpers_azure.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      352 2022-12-19 16:11:22.000000 salure_helpers_azure-0.0.1/salure_helpers_azure.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-19 16:11:22.000000 salure_helpers_azure-0.0.1/salure_helpers_azure.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-19 16:11:22.000000 salure_helpers_azure-0.0.1/salure_helpers_azure.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       78 2022-12-19 16:11:22.000000 salure_helpers_azure-0.0.1/salure_helpers_azure.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-12-19 16:11:22.000000 salure_helpers_azure-0.0.1/salure_helpers_azure.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-19 16:11:22.000000 salure_helpers_azure-0.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      489 2022-12-19 16:11:07.000000 salure_helpers_azure-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      259 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/salure_helpers/azure/
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-06-27 16:03:55.000000 salure_helpers_azure-1.0.1/salure_helpers/azure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15697 2023-06-27 16:03:55.000000 salure_helpers_azure-1.0.1/salure_helpers/azure/active_directory.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-06-27 16:03:55.000000 salure_helpers_azure-1.0.1/salure_helpers/azure/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     4560 2023-06-27 16:03:55.000000 salure_helpers_azure-1.0.1/salure_helpers/azure/azure_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-06-27 16:03:55.000000 salure_helpers_azure-1.0.1/salure_helpers/azure/blob_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/salure_helpers_azure.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      259 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/salure_helpers_azure.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      461 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/salure_helpers_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/salure_helpers_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/salure_helpers_azure.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       78 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/salure_helpers_azure.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/salure_helpers_azure.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 16:04:09.000000 salure_helpers_azure-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-06-27 16:03:55.000000 salure_helpers_azure-1.0.1/setup.py
```

### Comparing `salure_helpers_azure-0.0.1/salure_helpers/azure/azure_connection.py` & `salure_helpers_azure-1.0.1/salure_helpers/azure/azure_connection.py`

 * *Files identical despite different names*

