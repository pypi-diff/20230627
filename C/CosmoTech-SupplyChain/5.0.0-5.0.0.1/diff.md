# Comparing `tmp/CosmoTech-SupplyChain-5.0.0.tar.gz` & `tmp/CosmoTech-SupplyChain-5.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CosmoTech-SupplyChain-5.0.0.tar", last modified: Thu Jun 22 09:59:37 2023, max compression
+gzip compressed data, was "CosmoTech-SupplyChain-5.0.0.1.tar", last modified: Tue Jun 27 14:53:37 2023, max compression
```

## Comparing `CosmoTech-SupplyChain-5.0.0.tar` & `CosmoTech-SupplyChain-5.0.0.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.616733 CosmoTech-SupplyChain-5.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.608733 CosmoTech-SupplyChain-5.0.0/CosmoTech_SupplyChain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-06-22 09:59:37.000000 CosmoTech-SupplyChain-5.0.0/CosmoTech_SupplyChain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-06-22 09:59:37.000000 CosmoTech-SupplyChain-5.0.0/CosmoTech_SupplyChain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 09:59:37.000000 CosmoTech-SupplyChain-5.0.0/CosmoTech_SupplyChain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-22 09:59:37.000000 CosmoTech-SupplyChain-5.0.0/CosmoTech_SupplyChain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-22 09:59:37.000000 CosmoTech-SupplyChain-5.0.0/CosmoTech_SupplyChain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1195 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-06-22 09:59:37.616733 CosmoTech-SupplyChain-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.608733 CosmoTech-SupplyChain-5.0.0/Supplychain/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.608733 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3344 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/adt_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/adx_and_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6620 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/adx_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     4451 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/cosmo_api_parameters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3385 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/csv_folder_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/csv_folder_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/duration.py
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/excel_folder_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/excel_folder_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/folder_io.py
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/json_folder_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      780 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/json_folder_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/memory_folder_io.py
--rw-r--r--   0 runner    (1001) docker     (122)      679 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/simulator_io.py
--rw-r--r--   0 runner    (1001) docker     (122)      869 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/storage_queue_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.608733 CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/cmaes_optimization_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7621 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/default_transformation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4276 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/multiprocessing_optimization.py
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/objective_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2044 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.612733 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5391 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/cmaes_optimization.py
--rw-r--r--   0 runner    (1001) docker     (122)     3232 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/consumers.py
--rw-r--r--   0 runner    (1001) docker     (122)    31357 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/local_sensitivity_analysis_comets.py
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/simulation_comets.py
--rw-r--r--   0 runner    (1001) docker     (122)    20372 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/stochastic_optimization.py
--rw-r--r--   0 runner    (1001) docker     (122)     7760 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/uncertainty_analysis.py
--rw-r--r--   0 runner    (1001) docker     (122)    23910 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/uncertainty_analysis_comets.py
--rw-r--r--   0 runner    (1001) docker     (122)    22140 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/uncertainty_analysis_helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.612733 CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6223 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/adt_column_description.py
--rw-r--r--   0 runner    (1001) docker     (122)     5318 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/default_values.py
--rw-r--r--   0 runner    (1001) docker     (122)     3149 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/simulator_files_description.py
--rw-r--r--   0 runner    (1001) docker     (122)    23192 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/validation_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.612733 CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6539 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/complete_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)    39924 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/from_dict_to_simulator.py
--rw-r--r--   0 runner    (1001) docker     (122)    11669 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/from_dict_to_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     6822 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/from_table_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)    52415 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/from_table_to_dict_old.py
--rw-r--r--   0 runner    (1001) docker     (122)    15303 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/patch_dict_with_parameters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3058 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/production_route.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.612733 CosmoTech-SupplyChain-5.0.0/Supplychain/Validate/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21965 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Validate/validate_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.616733 CosmoTech-SupplyChain-5.0.0/Supplychain/Wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Wrappers/environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (122)    18535 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Wrappers/simulator.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-22 09:59:37.616733 CosmoTech-SupplyChain-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:53:37.465460 CosmoTech-SupplyChain-5.0.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:53:37.449460 CosmoTech-SupplyChain-5.0.0.1/CosmoTech_SupplyChain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-06-27 14:53:37.000000 CosmoTech-SupplyChain-5.0.0.1/CosmoTech_SupplyChain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-06-27 14:53:37.000000 CosmoTech-SupplyChain-5.0.0.1/CosmoTech_SupplyChain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 14:53:37.000000 CosmoTech-SupplyChain-5.0.0.1/CosmoTech_SupplyChain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-27 14:53:37.000000 CosmoTech-SupplyChain-5.0.0.1/CosmoTech_SupplyChain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-27 14:53:37.000000 CosmoTech-SupplyChain-5.0.0.1/CosmoTech_SupplyChain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1195 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-06-27 14:53:37.465460 CosmoTech-SupplyChain-5.0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:53:37.449460 CosmoTech-SupplyChain-5.0.0.1/Supplychain/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:53:37.457460 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3344 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/adt_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/adx_and_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6620 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/adx_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4451 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/cosmo_api_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3385 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/csv_folder_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/csv_folder_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/duration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/excel_folder_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/excel_folder_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/folder_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/json_folder_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      780 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/json_folder_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/memory_folder_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)      679 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/simulator_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/storage_queue_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:53:37.457460 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Protocol/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Protocol/cmaes_optimization_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7621 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Protocol/default_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4276 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Protocol/multiprocessing_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Protocol/objective_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2044 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Protocol/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:53:37.461460 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5391 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/cmaes_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3232 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/consumers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31357 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/local_sensitivity_analysis_comets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/simulation_comets.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20372 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/stochastic_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7760 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/uncertainty_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23910 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/uncertainty_analysis_comets.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22140 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/uncertainty_analysis_helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:53:37.461460 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Schema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6223 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Schema/adt_column_description.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5318 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Schema/default_values.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3149 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Schema/simulator_files_description.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23192 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Schema/validation_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:53:37.465460 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Transform/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6539 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Transform/complete_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39924 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Transform/from_dict_to_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11669 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Transform/from_dict_to_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6822 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Transform/from_table_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52415 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Transform/from_table_to_dict_old.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15664 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Transform/patch_dict_with_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3058 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Transform/production_route.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:53:37.465460 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Validate/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21965 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Validate/validate_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:53:37.465460 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Wrappers/environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18535 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/Wrappers/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/Supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-27 14:53:37.465460 CosmoTech-SupplyChain-5.0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      853 2023-06-27 14:53:29.000000 CosmoTech-SupplyChain-5.0.0.1/setup.py
```

### Comparing `CosmoTech-SupplyChain-5.0.0/CosmoTech_SupplyChain.egg-info/SOURCES.txt` & `CosmoTech-SupplyChain-5.0.0.1/CosmoTech_SupplyChain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/LICENSE` & `CosmoTech-SupplyChain-5.0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/README.md` & `CosmoTech-SupplyChain-5.0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/adt_writer.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/adt_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/adx_and_file_writer.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/adx_and_file_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/adx_wrapper.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/adx_wrapper.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/cosmo_api_parameters.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/cosmo_api_parameters.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/csv_folder_reader.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/csv_folder_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/csv_folder_writer.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/csv_folder_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/duration.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/duration.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/excel_folder_reader.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/excel_folder_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/excel_folder_writer.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/excel_folder_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/folder_io.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/folder_io.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/json_folder_reader.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/json_folder_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/json_folder_writer.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/json_folder_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/memory_folder_io.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/memory_folder_io.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/simulator_io.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/simulator_io.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/storage_queue_writer.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/storage_queue_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/timer.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Generic/timer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/cmaes_optimization_algorithm.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Protocol/cmaes_optimization_algorithm.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/default_transformation.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Protocol/default_transformation.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/multiprocessing_optimization.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Protocol/multiprocessing_optimization.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/objective_functions.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Protocol/objective_functions.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/protocol.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Run/cmaes_optimization.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/cmaes_optimization.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Run/consumers.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/consumers.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Run/local_sensitivity_analysis_comets.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/local_sensitivity_analysis_comets.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Run/simulation.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/simulation.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Run/simulation_comets.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/simulation_comets.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Run/stochastic_optimization.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/stochastic_optimization.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Run/uncertainty_analysis.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/uncertainty_analysis.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Run/uncertainty_analysis_comets.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/uncertainty_analysis_comets.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Run/uncertainty_analysis_helper_functions.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Run/uncertainty_analysis_helper_functions.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/adt_column_description.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Schema/adt_column_description.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/default_values.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Schema/default_values.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/simulator_files_description.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Schema/simulator_files_description.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/validation_schemas.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Schema/validation_schemas.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/complete_dict.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Transform/complete_dict.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/from_dict_to_simulator.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Transform/from_dict_to_simulator.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/from_dict_to_table.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Transform/from_dict_to_table.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/from_table_to_dict.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Transform/from_table_to_dict.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/from_table_to_dict_old.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Transform/from_table_to_dict_old.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/patch_dict_with_parameters.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Transform/patch_dict_with_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,20 @@
 
         self.__handle_demand_plan()
         self.__handle_transport_duration()
         self.__handle_production_resource_opening_time()
 
         self.__write_updated_files()
 
+    def handle_optimization_parameter(self):
+        parameters = (('optimization_objective', 'OptimizationObjective', 'Optimization Objective', None),)
+        for name, config_name, display_name, type_f in parameters:
+            self.__handle_configuration_parameter(name, config_name, display_name, type_f)
+        self.__write_updated_files()
+
     def handle_flow_management_policies(self):
         parameters = (
             ("stock_policy", "Stock", "StockPolicy"),
             ("sourcing_policy", "Stock", "SourcingPolicy"),
             ("stock_dispatch_policy", "Stock", "DispatchPolicy"),
             ("production_policy", "ProductionResource", "ProductionPolicy"),
         )
@@ -301,15 +307,15 @@
                 opening_changes.setdefault(_id, dict())
                 opening_changes[_id][timestep] = opening_time
         for e in self.memory.files.get("ProductionResource", []):
             change = opening_changes.get(e["id"])
             if change:
                 e["OpeningTimes"] = change
 
-    def handle_optimization_parameter(self, param_to_update: dict):
+    def handle_stochastic_optimization_parameters(self, param_to_update: dict):
         parameters = (
             (
                 "KPI",
                 "Kpi",
                 "KPI",
                 None,
             ),
```

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/production_route.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Transform/production_route.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Validate/validate_dict.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Validate/validate_dict.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Wrappers/environment_variables.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Wrappers/environment_variables.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/Supplychain/Wrappers/simulator.py` & `CosmoTech-SupplyChain-5.0.0.1/Supplychain/Wrappers/simulator.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.0/setup.py` & `CosmoTech-SupplyChain-5.0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-VERSION = "5.0.0"
+VERSION = "5.0.0.1"
 
 setuptools.setup(
     name='CosmoTech-SupplyChain',
     version=VERSION,
     author='Alexis Fossart',
     author_email='alexis.fossart@cosmotech.com',
     url='https://github.com/Cosmo-Tech/supplychain-python-library<',
```

