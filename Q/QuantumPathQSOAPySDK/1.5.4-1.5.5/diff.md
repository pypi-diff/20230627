# Comparing `tmp/QuantumPathQSOAPySDK-1.5.4.tar.gz` & `tmp/QuantumPathQSOAPySDK-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantumPathQSOAPySDK-1.5.4.tar", last modified: Tue Jun 27 09:22:40 2023, max compression
+gzip compressed data, was "QuantumPathQSOAPySDK-1.5.5.tar", last modified: Tue Jun 27 11:54:45 2023, max compression
```

## Comparing `QuantumPathQSOAPySDK-1.5.4.tar` & `QuantumPathQSOAPySDK-1.5.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.439571 QuantumPathQSOAPySDK-1.5.4/
--rw-rw-rw-   0        0        0       25 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.4/MANIFEST.in
--rw-rw-rw-   0        0        0      928 2023-06-27 09:22:40.439081 QuantumPathQSOAPySDK-1.5.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.292952 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/
--rw-rw-rw-   0        0        0    42866 2023-06-27 06:40:09.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/QSOAPlatform.py
--rw-rw-rw-   0        0        0       38 2023-06-09 10:56:58.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.330796 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/
--rw-rw-rw-   0        0        0      145 2023-06-12 08:01:03.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.338775 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/annealing/
--rw-rw-rw-   0        0        0     7907 2023-06-26 09:01:38.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py
--rw-rw-rw-   0        0        0       46 2023-06-12 08:43:39.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/annealing/__init__.py
--rw-rw-rw-   0        0        0    28762 2023-06-27 08:12:21.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/annealing/components.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.345878 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/flow/
--rw-rw-rw-   0        0        0     4848 2023-06-26 09:03:51.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py
--rw-rw-rw-   0        0        0       36 2023-06-12 08:44:11.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/flow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.351741 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/gates/
--rw-rw-rw-   0        0        0    52810 2023-06-26 09:04:34.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py
--rw-rw-rw-   0        0        0       38 2023-06-12 08:44:43.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/gates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.378679 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/
--rw-rw-rw-   0        0        0      746 2022-11-24 16:14:18.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/Application.py
--rw-rw-rw-   0        0        0     1542 2022-12-13 10:45:36.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/Asset.py
--rw-rw-rw-   0        0        0     1448 2022-11-24 16:17:42.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/AssetManagementData.py
--rw-rw-rw-   0        0        0     1861 2022-11-24 16:18:41.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/AssetManagementResult.py
--rw-rw-rw-   0        0        0     1088 2023-06-06 09:11:13.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/DeviceItem.py
--rw-rw-rw-   0        0        0     1289 2022-11-24 16:21:25.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/Execution.py
--rw-rw-rw-   0        0        0      276 2022-11-24 16:21:43.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/FlowItem.py
--rw-rw-rw-   0        0        0     2615 2022-11-24 16:24:27.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py
--rw-rw-rw-   0        0        0      280 2022-11-24 16:24:49.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/SolutionItem.py
--rw-rw-rw-   0        0        0      280 2023-06-09 10:57:16.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.387747 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/qsoa/
--rw-rw-rw-   0        0        0      968 2023-06-13 07:53:10.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/qsoa/__init__.py
--rw-rw-rw-   0        0        0     9076 2023-06-09 09:56:38.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/qsoa/connectionPoints.py
--rw-rw-rw-   0        0        0    10099 2023-06-12 08:01:27.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py
--rw-rw-rw-   0        0        0     4077 2023-06-13 11:39:31.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.401674 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/utils/
--rw-rw-rw-   0        0        0     3764 2023-06-09 09:40:06.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/utils/Context.py
--rw-rw-rw-   0        0        0     1047 2022-11-30 08:30:03.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/utils/Exception.py
--rw-rw-rw-   0        0        0      160 2023-06-22 10:01:20.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/utils/__init__.py
--rw-rw-rw-   0        0        0     1514 2023-06-06 09:42:42.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/utils/apiConnection.py
--rw-rw-rw-   0        0        0     3216 2023-06-22 11:57:59.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/utils/checker.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.328803 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK.egg-info/
--rw-rw-rw-   0        0        0      928 2023-06-27 09:22:40.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2085 2023-06-27 09:22:40.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 09:22:40.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-27 09:22:40.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-27 09:22:40.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 09:22:40.440570 QuantumPathQSOAPySDK-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0      973 2023-06-27 09:14:38.000000 QuantumPathQSOAPySDK-1.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.403668 QuantumPathQSOAPySDK-1.5.4/test/
--rw-rw-rw-   0        0        0       83 2023-06-26 09:17:26.000000 QuantumPathQSOAPySDK-1.5.4/test/test.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.420634 QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:50:59.000000 QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/__init__.py
--rw-rw-rw-   0        0        0     2692 2023-06-14 10:56:41.000000 QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_ContextMethods.py
--rw-rw-rw-   0        0        0    65272 2023-06-14 11:26:03.000000 QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_DynamicMethods.py
--rw-rw-rw-   0        0        0     3244 2023-06-14 11:14:52.000000 QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_QSOAPlatform.py
--rw-rw-rw-   0        0        0     8740 2023-06-14 11:02:20.000000 QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_SecurityMethods.py
--rw-rw-rw-   0        0        0    28777 2023-06-14 11:23:11.000000 QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_StaticMethods.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.437577 QuantumPathQSOAPySDK-1.5.4/test/test_circuit/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:31:46.000000 QuantumPathQSOAPySDK-1.5.4/test/test_circuit/__init__.py
--rw-rw-rw-   0        0        0   130207 2023-06-27 08:11:21.000000 QuantumPathQSOAPySDK-1.5.4/test/test_circuit/test_CircuitAnnealing.py
--rw-rw-rw-   0        0        0     8004 2023-06-26 10:45:48.000000 QuantumPathQSOAPySDK-1.5.4/test/test_circuit/test_CircuitFlow.py
--rw-rw-rw-   0        0        0     7331 2023-06-26 10:46:07.000000 QuantumPathQSOAPySDK-1.5.4/test/test_circuit/test_CircuitGates.py
--rw-rw-rw-   0        0        0   157579 2023-06-26 10:26:09.000000 QuantumPathQSOAPySDK-1.5.4/test/test_circuit/test_CircuitGates_gates1.py
--rw-rw-rw-   0        0        0    35843 2023-06-26 10:26:50.000000 QuantumPathQSOAPySDK-1.5.4/test/test_circuit/test_CircuitGates_gates2.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:45.060810 QuantumPathQSOAPySDK-1.5.5/
+-rw-rw-rw-   0        0        0       25 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      928 2023-06-27 11:54:45.059813 QuantumPathQSOAPySDK-1.5.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:44.921137 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/
+-rw-rw-rw-   0        0        0    42866 2023-06-27 06:40:09.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/QSOAPlatform.py
+-rw-rw-rw-   0        0        0       38 2023-06-09 10:56:58.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:44.958208 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/
+-rw-rw-rw-   0        0        0      145 2023-06-12 08:01:03.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:44.966019 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/annealing/
+-rw-rw-rw-   0        0        0     7907 2023-06-26 09:01:38.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py
+-rw-rw-rw-   0        0        0       46 2023-06-12 08:43:39.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/annealing/__init__.py
+-rw-rw-rw-   0        0        0    28762 2023-06-27 08:12:21.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/annealing/components.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:44.971007 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/flow/
+-rw-rw-rw-   0        0        0     4848 2023-06-26 09:03:51.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py
+-rw-rw-rw-   0        0        0       36 2023-06-12 08:44:11.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/flow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:44.989012 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/gates/
+-rw-rw-rw-   0        0        0    53330 2023-06-27 11:39:45.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py
+-rw-rw-rw-   0        0        0       38 2023-06-12 08:44:43.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/gates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:45.009902 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/
+-rw-rw-rw-   0        0        0      746 2022-11-24 16:14:18.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/Application.py
+-rw-rw-rw-   0        0        0     1542 2022-12-13 10:45:36.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/Asset.py
+-rw-rw-rw-   0        0        0     1448 2022-11-24 16:17:42.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/AssetManagementData.py
+-rw-rw-rw-   0        0        0     1861 2022-11-24 16:18:41.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/AssetManagementResult.py
+-rw-rw-rw-   0        0        0     1088 2023-06-06 09:11:13.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/DeviceItem.py
+-rw-rw-rw-   0        0        0     1289 2022-11-24 16:21:25.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/Execution.py
+-rw-rw-rw-   0        0        0      276 2022-11-24 16:21:43.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/FlowItem.py
+-rw-rw-rw-   0        0        0     2615 2022-11-24 16:24:27.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py
+-rw-rw-rw-   0        0        0      280 2022-11-24 16:24:49.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/SolutionItem.py
+-rw-rw-rw-   0        0        0      280 2023-06-09 10:57:16.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:45.019872 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/qsoa/
+-rw-rw-rw-   0        0        0      968 2023-06-13 07:53:10.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/qsoa/__init__.py
+-rw-rw-rw-   0        0        0     9076 2023-06-09 09:56:38.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/qsoa/connectionPoints.py
+-rw-rw-rw-   0        0        0    10099 2023-06-12 08:01:27.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py
+-rw-rw-rw-   0        0        0     4077 2023-06-13 11:39:31.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:45.028848 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/
+-rw-rw-rw-   0        0        0     3764 2023-06-09 09:40:06.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/Context.py
+-rw-rw-rw-   0        0        0     1047 2022-11-30 08:30:03.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/Exception.py
+-rw-rw-rw-   0        0        0      160 2023-06-22 10:01:20.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/__init__.py
+-rw-rw-rw-   0        0        0     1514 2023-06-06 09:42:42.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/apiConnection.py
+-rw-rw-rw-   0        0        0     3216 2023-06-22 11:57:59.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/checker.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:44.956044 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK.egg-info/
+-rw-rw-rw-   0        0        0      928 2023-06-27 11:54:44.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2085 2023-06-27 11:54:44.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 11:54:44.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-27 11:54:44.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-27 11:54:44.000000 QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 11:54:45.060810 QuantumPathQSOAPySDK-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      973 2023-06-27 11:54:12.000000 QuantumPathQSOAPySDK-1.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:45.032887 QuantumPathQSOAPySDK-1.5.5/test/
+-rw-rw-rw-   0        0        0       83 2023-06-27 11:27:42.000000 QuantumPathQSOAPySDK-1.5.5/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:45.043856 QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:50:59.000000 QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/__init__.py
+-rw-rw-rw-   0        0        0     2692 2023-06-14 10:56:41.000000 QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/test_ContextMethods.py
+-rw-rw-rw-   0        0        0    65272 2023-06-14 11:26:03.000000 QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/test_DynamicMethods.py
+-rw-rw-rw-   0        0        0     3244 2023-06-14 11:14:52.000000 QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/test_QSOAPlatform.py
+-rw-rw-rw-   0        0        0     8740 2023-06-14 11:02:20.000000 QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/test_SecurityMethods.py
+-rw-rw-rw-   0        0        0    28777 2023-06-14 11:23:11.000000 QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/test_StaticMethods.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:54:45.058122 QuantumPathQSOAPySDK-1.5.5/test/test_circuit/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:31:46.000000 QuantumPathQSOAPySDK-1.5.5/test/test_circuit/__init__.py
+-rw-rw-rw-   0        0        0   130207 2023-06-27 08:11:21.000000 QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitAnnealing.py
+-rw-rw-rw-   0        0        0     8004 2023-06-26 10:45:48.000000 QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitFlow.py
+-rw-rw-rw-   0        0        0     7331 2023-06-26 10:46:07.000000 QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitGates.py
+-rw-rw-rw-   0        0        0   153999 2023-06-27 11:33:39.000000 QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitGates_gates1.py
+-rw-rw-rw-   0        0        0    41572 2023-06-27 11:33:49.000000 QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitGates_gates2.py
```

### Comparing `QuantumPathQSOAPySDK-1.5.4/PKG-INFO` & `QuantumPathQSOAPySDK-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumPathQSOAPySDK
-Version: 1.5.4
+Version: 1.5.5
 Summary: QuantumPath qSOA Python SDK
 Home-page: https://core.quantumpath.app/
 Author: QuantumPath
 License: UNKNOWN
 Keywords: quantum,quantumpath,qSOA,sdk,quantum applications,quantum software
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/QSOAPlatform.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/QSOAPlatform.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/annealing/components.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/annealing/components.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1126,14 +1126,15 @@
         list
         """
         checkInputTypes(
             ('position1', position1, (int,)),
             ('position2', position2, (int,)),
             ('add', add, (bool,)),
         )
+        checkDifferentPosition([position1, position2])
 
         positions = [
             (position1, 'Swap'),
             (position2, 'Swap')
         ]
 
         if add:
@@ -1165,14 +1166,15 @@
         list
         """
         checkInputTypes(
             ('position1', position1, (int,)),
             ('position2', position2, (int,)),
             ('add', add, (bool,)),
         )
+        checkDifferentPosition([position1, position2])
 
         positions = [
             (position1, 'CTRL'),
             (position2, 'H')
         ]
 
         if add:
@@ -1204,14 +1206,15 @@
         list
         """
         checkInputTypes(
             ('position1', position1, (int,)),
             ('position2', position2, (int,)),
             ('add', add, (bool,)),
         )
+        checkDifferentPosition([position1, position2])
 
         positions = [
             (position1, 'CTRL'),
             (position2, 'X')
         ]
 
         if add:
@@ -1246,14 +1249,15 @@
         """
         checkInputTypes(
             ('position1', position1, (int,)),
             ('position2', position2, (int,)),
             ('position3', position3, (int,)),
             ('add', add, (bool,)),
         )
+        checkDifferentPosition([position1, position2, position3])
 
         positions = [
             (position1, 'CTRL'),
             (position2, 'CTRL'),
             (position3, 'X')
         ]
 
@@ -1493,16 +1497,25 @@
         checkInputTypes(
             ('position', position, (int, list)),
             ('circuit', circuit, (list,)),
             ('add', add, (bool,)),
         )
         if isinstance(position, list):
             checkListTypes(('position', position, (int,)))
-            checkDifferentPosition(position)
         
+        circuitPositions = []
+        for gate in circuit:
+            circuitPositions.append(gate[0])
+
+        if isinstance(position, int):
+            circuitPositions.append(position)
+            checkDifferentPosition(circuitPositions)
+        else:
+            checkDifferentPosition(position + circuitPositions)
+
         gateSymbol = 'CTRL'
 
         if isinstance(position, int): # one postion
             circuit.append((position, gateSymbol))
 
         elif isinstance(position, list): # multiple positions
             for i in position:
```

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/Application.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/Application.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/Asset.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/Asset.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/AssetManagementData.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/AssetManagementData.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/AssetManagementResult.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/AssetManagementResult.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/DeviceItem.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/DeviceItem.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/Execution.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/Execution.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/qsoa/__init__.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/qsoa/__init__.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/qsoa/connectionPoints.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/qsoa/connectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/utils/Context.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/Context.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/utils/Exception.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/Exception.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/utils/apiConnection.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/apiConnection.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/utils/checker.py` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK/utils/checker.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK.egg-info/PKG-INFO` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumPathQSOAPySDK
-Version: 1.5.4
+Version: 1.5.5
 Summary: QuantumPath qSOA Python SDK
 Home-page: https://core.quantumpath.app/
 Author: QuantumPath
 License: UNKNOWN
 Keywords: quantum,quantumpath,qSOA,sdk,quantum applications,quantum software
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK.egg-info/SOURCES.txt` & `QuantumPathQSOAPySDK-1.5.5/QuantumPathQSOAPySDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/setup.py` & `QuantumPathQSOAPySDK-1.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   'Intended Audience :: Developers',
   'Intended Audience :: Education',
   'Intended Audience :: Information Technology'
 ]
 
 setup(
   name='QuantumPathQSOAPySDK',
-  version='1.5.4',
+  version='1.5.5',
   description='QuantumPath qSOA Python SDK',
   long_description=open('README.md').read(),
   long_description_content_type = 'text/markdown',
   url='https://core.quantumpath.app/',
   author='QuantumPath',
   classifiers=classifiers,
   keywords='quantum, quantumpath, qSOA, sdk, quantum applications, quantum software',
```

### Comparing `QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_ContextMethods.py` & `QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/test_ContextMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_DynamicMethods.py` & `QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/test_DynamicMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_QSOAPlatform.py` & `QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/test_QSOAPlatform.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_SecurityMethods.py` & `QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/test_SecurityMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_StaticMethods.py` & `QuantumPathQSOAPySDK-1.5.5/test/test_QSOAPlatform/test_StaticMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/test/test_circuit/test_CircuitAnnealing.py` & `QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitAnnealing.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/test/test_circuit/test_CircuitFlow.py` & `QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitFlow.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/test/test_circuit/test_CircuitGates.py` & `QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitGates.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.4/test/test_circuit/test_CircuitGates_gates1.py` & `QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitGates_gates1.py`

 * *Files 1% similar despite different names*

```diff
@@ -4464,14 +4464,26 @@
 
         gate = circuit.swap(1, 3, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'Swap'), (3, 'Swap')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position1, position2
+    def test_swap_badArgument_position1_position2(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.swap(0, 0)
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT TYPE position1
     def test_swap_badArgumentType_position1(self):
         qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.swap('position', 3)
@@ -4596,177 +4608,57 @@
 
         gate = circuit.ch(1, 3, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'CTRL'), (3, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
-    # BAD ARGUMENT TYPE position1
-    def test_ch_badArgumentType_position1(self):
+    # BAD ARGUMENT position1, position2
+    def test_ch_badArgument_position1_position2(self):
         qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
-            circuit.ch('position', 3)
+            circuit.ch(0, 0)
             raise Exception
 
         except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-    # BAD ARGUMENT TYPE position2
-    def test_ch_badArgumentType_position2(self):
-        qsoa = QSOAPlatform(configFile=True)
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.ch(1, 'position')
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-    # BAD ARGUMENT TYPE add
-    def test_ch_badArgumentType_add(self):
-        qsoa = QSOAPlatform(configFile=True)
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.ch(1, 3, 'add')
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-
-##################_____CX_____##################
-class Test_CX(unittest.TestCase):
-
-    # CX position 0, 1
-    def test_cx_position_0_1(self):
-        qsoa = QSOAPlatform(configFile=True)
-        circuit = qsoa.CircuitGates()
-
-        gate = circuit.cx(0, 1)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, 'CTRL'), (1, 'X')])
-        self.assertEqual(circuit.getCircuitBody(), [['CTRL', 'X']])
-
-    # CX position 0, 2
-    def test_cx_position_0_2(self):
-        qsoa = QSOAPlatform(configFile=True)
-        circuit = qsoa.CircuitGates()
-
-        gate = circuit.cx(0, 2)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, 'CTRL'), (2, 'X')])
-        self.assertEqual(circuit.getCircuitBody(), [['CTRL', 1, 'X']])
-
-    # CX position 1, 2
-    def test_cx_position_position_1_2(self):
-        qsoa = QSOAPlatform(configFile=True)
-        circuit = qsoa.CircuitGates()
-
-        gate = circuit.cx(1, 2)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(1, 'CTRL'), (2, 'X')])
-        self.assertEqual(circuit.getCircuitBody(), [[1, 'CTRL', 'X']])
-
-    # CX EXISTING CIRCUIT position NEW COLUMN
-    def test_cx_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform(configFile=True)
-        circuit = qsoa.CircuitGates()
-        circuit.h(0)
-
-        gate = circuit.cx(0, 1)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, 'CTRL'), (1, 'X')])
-        self.assertEqual(circuit.getCircuitBody(), [['H'], ['CTRL', 'X']])
-
-    # CX EXISTING CIRCUIT position SAME COLUMN
-    def test_cx_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform(configFile=True)
-        circuit = qsoa.CircuitGates()
-        circuit.h(0)
-
-        gate = circuit.cx(1, 2)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(1, 'CTRL'), (2, 'X')])
-        self.assertEqual(circuit.getCircuitBody(), [['H'], [1, 'CTRL', 'X']])
-
-    # CX EXISTING CIRCUIT position BETWEEN SWAP
-    def test_cx_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform(configFile=True)
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 3)
-
-        gate = circuit.cx(1, 2)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(1, 'CTRL'), (2, 'X')])
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 1, 'Swap'], [1, 'CTRL', 'X']])
-
-    # CX EXISTING CIRCUIT position UNDER SWAP
-    def test_cx_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform(configFile=True)
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 1)
-
-        gate = circuit.cx(2, 3)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(2, 'CTRL'), (3, 'X')])
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'CTRL', 'X']])
-
-    # CX add
-    def test_cx_add(self):
-        qsoa = QSOAPlatform(configFile=True)
-        circuit = qsoa.CircuitGates()
-
-        gate = circuit.cx(1, 3, False)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(1, 'CTRL'), (3, 'X')])
-        self.assertEqual(circuit.getCircuitBody(), [[]])
+            self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position1
-    def test_cx_badArgumentType_position1(self):
+    def test_ch_badArgumentType_position1(self):
         qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
-            circuit.cx('position', 3)
+            circuit.ch('position', 3)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position2
-    def test_cx_badArgumentType_position2(self):
+    def test_ch_badArgumentType_position2(self):
         qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
-            circuit.cx(1, 'position')
+            circuit.ch(1, 'position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
-    def test_cx_badArgumentType_add(self):
+    def test_ch_badArgumentType_add(self):
         qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
-            circuit.cx(1, 3, 'add')
+            circuit.ch(1, 3, 'add')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
 
 if __name__ == '__main__':
```

### Comparing `QuantumPathQSOAPySDK-1.5.4/test/test_circuit/test_CircuitGates_gates2.py` & `QuantumPathQSOAPySDK-1.5.5/test/test_circuit/test_CircuitGates_gates2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,155 @@
 import unittest
 from QuantumPathQSOAPySDK import QSOAPlatform
 
 
+##################_____CX_____##################
+class Test_CX(unittest.TestCase):
+
+    # CX position 0, 1
+    def test_cx_position_0_1(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        gate = circuit.cx(0, 1)
+
+        self.assertIsInstance(gate, list)
+        self.assertEqual(gate, [(0, 'CTRL'), (1, 'X')])
+        self.assertEqual(circuit.getCircuitBody(), [['CTRL', 'X']])
+
+    # CX position 0, 2
+    def test_cx_position_0_2(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        gate = circuit.cx(0, 2)
+
+        self.assertIsInstance(gate, list)
+        self.assertEqual(gate, [(0, 'CTRL'), (2, 'X')])
+        self.assertEqual(circuit.getCircuitBody(), [['CTRL', 1, 'X']])
+
+    # CX position 1, 2
+    def test_cx_position_position_1_2(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        gate = circuit.cx(1, 2)
+
+        self.assertIsInstance(gate, list)
+        self.assertEqual(gate, [(1, 'CTRL'), (2, 'X')])
+        self.assertEqual(circuit.getCircuitBody(), [[1, 'CTRL', 'X']])
+
+    # CX EXISTING CIRCUIT position NEW COLUMN
+    def test_cx_existingCircuit_position_newColumn(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+        circuit.h(0)
+
+        gate = circuit.cx(0, 1)
+
+        self.assertIsInstance(gate, list)
+        self.assertEqual(gate, [(0, 'CTRL'), (1, 'X')])
+        self.assertEqual(circuit.getCircuitBody(), [['H'], ['CTRL', 'X']])
+
+    # CX EXISTING CIRCUIT position SAME COLUMN
+    def test_cx_existingCircuit_position_sameColumn(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+        circuit.h(0)
+
+        gate = circuit.cx(1, 2)
+
+        self.assertIsInstance(gate, list)
+        self.assertEqual(gate, [(1, 'CTRL'), (2, 'X')])
+        self.assertEqual(circuit.getCircuitBody(), [['H'], [1, 'CTRL', 'X']])
+
+    # CX EXISTING CIRCUIT position BETWEEN SWAP
+    def test_cx_existingCircuit_position_betweenSwap(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+        circuit.swap(0, 3)
+
+        gate = circuit.cx(1, 2)
+
+        self.assertIsInstance(gate, list)
+        self.assertEqual(gate, [(1, 'CTRL'), (2, 'X')])
+        self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 1, 'Swap'], [1, 'CTRL', 'X']])
+
+    # CX EXISTING CIRCUIT position UNDER SWAP
+    def test_cx_existingCircuit_position_underSwap(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+        circuit.swap(0, 1)
+
+        gate = circuit.cx(2, 3)
+
+        self.assertIsInstance(gate, list)
+        self.assertEqual(gate, [(2, 'CTRL'), (3, 'X')])
+        self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'CTRL', 'X']])
+
+    # CX add
+    def test_cx_add(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        gate = circuit.cx(1, 3, False)
+
+        self.assertIsInstance(gate, list)
+        self.assertEqual(gate, [(1, 'CTRL'), (3, 'X')])
+        self.assertEqual(circuit.getCircuitBody(), [[]])
+
+    # BAD ARGUMENT position1, position2
+    def test_cx_badArgument_position1_position2(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.cx(0, 0)
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
+    # BAD ARGUMENT TYPE position1
+    def test_cx_badArgumentType_position1(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.cx('position', 3)
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, TypeError)
+
+    # BAD ARGUMENT TYPE position2
+    def test_cx_badArgumentType_position2(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.cx(1, 'position')
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, TypeError)
+
+    # BAD ARGUMENT TYPE add
+    def test_cx_badArgumentType_add(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.cx(1, 3, 'add')
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, TypeError)
+
+
 ##################_____CCX_____##################
 class Test_CCX(unittest.TestCase):
 
     # CCX position 0, 1, 2
     def test_ccx_position_0_1_2(self):
         qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
@@ -93,14 +237,26 @@
 
         gate = circuit.ccx(1, 2, 3, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'CTRL'), (2, 'CTRL'), (3, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position1, position2, position3
+    def test_ccx_badArgument_position1_position2(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.ccx(0, 0, 1)
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT TYPE position1
     def test_ccx_badArgumentType_position1(self):
         qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.ccx('position', 2, 3)
@@ -955,14 +1111,26 @@
 
         gate = circuit.mcg([0, 2], circuit.x(3, False), False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(3, 'X'), (0, 'CTRL'), (2, 'CTRL')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position DUPLICATED CIRCUIT
+    def test_mcg_badArgument_position_duplicated_circuit(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.mcg(0, circuit.x(0))
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST
     def test_mcg_badArgument_position_list(self):
         qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.mcg([], circuit.x(3))
@@ -979,14 +1147,26 @@
         try:
             circuit.mcg([0, 0], circuit.x(3))
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
+    # BAD ARGUMENT position LIST DUPLICATED CIRCUIT
+    def test_mcg_badArgument_position_list_duplicated_circuit(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.mcg([0, 1], circuit.x(1))
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT circuit
     def test_mcg_badArgument_circuit(self):
         qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.mcg(1, circuit.x(3))
```

