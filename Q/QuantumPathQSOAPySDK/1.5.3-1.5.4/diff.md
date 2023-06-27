# Comparing `tmp/QuantumPathQSOAPySDK-1.5.3.tar.gz` & `tmp/QuantumPathQSOAPySDK-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantumPathQSOAPySDK-1.5.3.tar", last modified: Tue Jun 20 09:13:30 2023, max compression
+gzip compressed data, was "QuantumPathQSOAPySDK-1.5.4.tar", last modified: Tue Jun 27 09:22:40 2023, max compression
```

## Comparing `QuantumPathQSOAPySDK-1.5.3.tar` & `QuantumPathQSOAPySDK-1.5.4.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 09:13:30.506298 QuantumPathQSOAPySDK-1.5.3/
--rw-rw-rw-   0        0        0       25 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0      928 2023-06-20 09:13:30.505298 QuantumPathQSOAPySDK-1.5.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 09:13:30.359526 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/
--rw-rw-rw-   0        0        0    41637 2023-06-14 10:34:16.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/QSOAPlatform.py
--rw-rw-rw-   0        0        0       38 2023-06-09 10:56:58.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:13:30.397425 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/circuit/
--rw-rw-rw-   0        0        0      145 2023-06-12 08:01:03.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/circuit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:13:30.406402 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/circuit/annealing/
--rw-rw-rw-   0        0        0     8778 2023-06-19 11:09:52.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py
--rw-rw-rw-   0        0        0       46 2023-06-12 08:43:39.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/circuit/annealing/__init__.py
--rw-rw-rw-   0        0        0    27502 2023-06-20 09:11:18.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/circuit/annealing/components.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:13:30.412489 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/circuit/flow/
--rw-rw-rw-   0        0        0     4884 2023-06-12 08:01:23.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py
--rw-rw-rw-   0        0        0       36 2023-06-12 08:44:11.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/circuit/flow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:13:30.417373 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/circuit/gates/
--rw-rw-rw-   0        0        0    53331 2023-06-20 08:30:05.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py
--rw-rw-rw-   0        0        0       38 2023-06-12 08:44:43.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/circuit/gates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:13:30.443463 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/objects/
--rw-rw-rw-   0        0        0      746 2022-11-24 16:14:18.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/objects/Application.py
--rw-rw-rw-   0        0        0     1542 2022-12-13 10:45:36.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/objects/Asset.py
--rw-rw-rw-   0        0        0     1448 2022-11-24 16:17:42.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/objects/AssetManagementData.py
--rw-rw-rw-   0        0        0     1861 2022-11-24 16:18:41.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/objects/AssetManagementResult.py
--rw-rw-rw-   0        0        0     1088 2023-06-06 09:11:13.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/objects/DeviceItem.py
--rw-rw-rw-   0        0        0     1289 2022-11-24 16:21:25.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/objects/Execution.py
--rw-rw-rw-   0        0        0      276 2022-11-24 16:21:43.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/objects/FlowItem.py
--rw-rw-rw-   0        0        0     2615 2022-11-24 16:24:27.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py
--rw-rw-rw-   0        0        0      280 2022-11-24 16:24:49.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/objects/SolutionItem.py
--rw-rw-rw-   0        0        0      280 2023-06-09 10:57:16.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/objects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:13:30.455433 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/qsoa/
--rw-rw-rw-   0        0        0      968 2023-06-13 07:53:10.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/qsoa/__init__.py
--rw-rw-rw-   0        0        0     9076 2023-06-09 09:56:38.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/qsoa/connectionPoints.py
--rw-rw-rw-   0        0        0    10099 2023-06-12 08:01:27.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py
--rw-rw-rw-   0        0        0     4077 2023-06-13 11:39:31.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:13:30.469397 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/utils/
--rw-rw-rw-   0        0        0     3764 2023-06-09 09:40:06.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/utils/Context.py
--rw-rw-rw-   0        0        0     1047 2022-11-30 08:30:03.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/utils/Exception.py
--rw-rw-rw-   0        0        0      144 2023-06-13 07:52:54.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/utils/__init__.py
--rw-rw-rw-   0        0        0     1514 2023-06-06 09:42:42.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/utils/apiConnection.py
--rw-rw-rw-   0        0        0     1734 2023-06-09 11:25:34.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/utils/checker.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:13:30.395645 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK.egg-info/
--rw-rw-rw-   0        0        0      928 2023-06-20 09:13:30.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1993 2023-06-20 09:13:30.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 09:13:30.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-20 09:13:30.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-20 09:13:30.000000 QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-20 09:13:30.506298 QuantumPathQSOAPySDK-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0      973 2023-06-20 09:13:18.000000 QuantumPathQSOAPySDK-1.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:13:30.472394 QuantumPathQSOAPySDK-1.5.3/test/
--rw-rw-rw-   0        0        0       83 2023-06-14 15:03:15.000000 QuantumPathQSOAPySDK-1.5.3/test/test.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:13:30.486369 QuantumPathQSOAPySDK-1.5.3/test/test_QSOAPlatform/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:50:59.000000 QuantumPathQSOAPySDK-1.5.3/test/test_QSOAPlatform/__init__.py
--rw-rw-rw-   0        0        0     2692 2023-06-14 10:56:41.000000 QuantumPathQSOAPySDK-1.5.3/test/test_QSOAPlatform/test_ContextMethods.py
--rw-rw-rw-   0        0        0    65272 2023-06-14 11:26:03.000000 QuantumPathQSOAPySDK-1.5.3/test/test_QSOAPlatform/test_DynamicMethods.py
--rw-rw-rw-   0        0        0     3244 2023-06-14 11:14:52.000000 QuantumPathQSOAPySDK-1.5.3/test/test_QSOAPlatform/test_QSOAPlatform.py
--rw-rw-rw-   0        0        0     8740 2023-06-14 11:02:20.000000 QuantumPathQSOAPySDK-1.5.3/test/test_QSOAPlatform/test_SecurityMethods.py
--rw-rw-rw-   0        0        0    28777 2023-06-14 11:23:11.000000 QuantumPathQSOAPySDK-1.5.3/test/test_QSOAPlatform/test_StaticMethods.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:13:30.502307 QuantumPathQSOAPySDK-1.5.3/test/test_circuit/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:31:46.000000 QuantumPathQSOAPySDK-1.5.3/test/test_circuit/__init__.py
--rw-rw-rw-   0        0        0   111685 2023-06-20 09:12:52.000000 QuantumPathQSOAPySDK-1.5.3/test/test_circuit/test_CircuitAnnealing.py
--rw-rw-rw-   0        0        0     7478 2023-05-22 11:55:54.000000 QuantumPathQSOAPySDK-1.5.3/test/test_circuit/test_CircuitFlow.py
--rw-rw-rw-   0        0        0   184849 2023-06-20 07:35:19.000000 QuantumPathQSOAPySDK-1.5.3/test/test_circuit/test_CircuitGates.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.439571 QuantumPathQSOAPySDK-1.5.4/
+-rw-rw-rw-   0        0        0       25 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      928 2023-06-27 09:22:40.439081 QuantumPathQSOAPySDK-1.5.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.292952 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/
+-rw-rw-rw-   0        0        0    42866 2023-06-27 06:40:09.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/QSOAPlatform.py
+-rw-rw-rw-   0        0        0       38 2023-06-09 10:56:58.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.330796 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/
+-rw-rw-rw-   0        0        0      145 2023-06-12 08:01:03.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.338775 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/annealing/
+-rw-rw-rw-   0        0        0     7907 2023-06-26 09:01:38.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py
+-rw-rw-rw-   0        0        0       46 2023-06-12 08:43:39.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/annealing/__init__.py
+-rw-rw-rw-   0        0        0    28762 2023-06-27 08:12:21.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/annealing/components.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.345878 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/flow/
+-rw-rw-rw-   0        0        0     4848 2023-06-26 09:03:51.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py
+-rw-rw-rw-   0        0        0       36 2023-06-12 08:44:11.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/flow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.351741 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/gates/
+-rw-rw-rw-   0        0        0    52810 2023-06-26 09:04:34.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py
+-rw-rw-rw-   0        0        0       38 2023-06-12 08:44:43.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/gates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.378679 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/
+-rw-rw-rw-   0        0        0      746 2022-11-24 16:14:18.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/Application.py
+-rw-rw-rw-   0        0        0     1542 2022-12-13 10:45:36.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/Asset.py
+-rw-rw-rw-   0        0        0     1448 2022-11-24 16:17:42.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/AssetManagementData.py
+-rw-rw-rw-   0        0        0     1861 2022-11-24 16:18:41.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/AssetManagementResult.py
+-rw-rw-rw-   0        0        0     1088 2023-06-06 09:11:13.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/DeviceItem.py
+-rw-rw-rw-   0        0        0     1289 2022-11-24 16:21:25.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/Execution.py
+-rw-rw-rw-   0        0        0      276 2022-11-24 16:21:43.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/FlowItem.py
+-rw-rw-rw-   0        0        0     2615 2022-11-24 16:24:27.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py
+-rw-rw-rw-   0        0        0      280 2022-11-24 16:24:49.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/SolutionItem.py
+-rw-rw-rw-   0        0        0      280 2023-06-09 10:57:16.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.387747 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/qsoa/
+-rw-rw-rw-   0        0        0      968 2023-06-13 07:53:10.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/qsoa/__init__.py
+-rw-rw-rw-   0        0        0     9076 2023-06-09 09:56:38.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/qsoa/connectionPoints.py
+-rw-rw-rw-   0        0        0    10099 2023-06-12 08:01:27.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py
+-rw-rw-rw-   0        0        0     4077 2023-06-13 11:39:31.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.401674 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/utils/
+-rw-rw-rw-   0        0        0     3764 2023-06-09 09:40:06.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/utils/Context.py
+-rw-rw-rw-   0        0        0     1047 2022-11-30 08:30:03.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/utils/Exception.py
+-rw-rw-rw-   0        0        0      160 2023-06-22 10:01:20.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/utils/__init__.py
+-rw-rw-rw-   0        0        0     1514 2023-06-06 09:42:42.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/utils/apiConnection.py
+-rw-rw-rw-   0        0        0     3216 2023-06-22 11:57:59.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/utils/checker.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.328803 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK.egg-info/
+-rw-rw-rw-   0        0        0      928 2023-06-27 09:22:40.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2085 2023-06-27 09:22:40.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 09:22:40.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-27 09:22:40.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-27 09:22:40.000000 QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 09:22:40.440570 QuantumPathQSOAPySDK-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      973 2023-06-27 09:14:38.000000 QuantumPathQSOAPySDK-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.403668 QuantumPathQSOAPySDK-1.5.4/test/
+-rw-rw-rw-   0        0        0       83 2023-06-26 09:17:26.000000 QuantumPathQSOAPySDK-1.5.4/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.420634 QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:50:59.000000 QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/__init__.py
+-rw-rw-rw-   0        0        0     2692 2023-06-14 10:56:41.000000 QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_ContextMethods.py
+-rw-rw-rw-   0        0        0    65272 2023-06-14 11:26:03.000000 QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_DynamicMethods.py
+-rw-rw-rw-   0        0        0     3244 2023-06-14 11:14:52.000000 QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_QSOAPlatform.py
+-rw-rw-rw-   0        0        0     8740 2023-06-14 11:02:20.000000 QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_SecurityMethods.py
+-rw-rw-rw-   0        0        0    28777 2023-06-14 11:23:11.000000 QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_StaticMethods.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:22:40.437577 QuantumPathQSOAPySDK-1.5.4/test/test_circuit/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:31:46.000000 QuantumPathQSOAPySDK-1.5.4/test/test_circuit/__init__.py
+-rw-rw-rw-   0        0        0   130207 2023-06-27 08:11:21.000000 QuantumPathQSOAPySDK-1.5.4/test/test_circuit/test_CircuitAnnealing.py
+-rw-rw-rw-   0        0        0     8004 2023-06-26 10:45:48.000000 QuantumPathQSOAPySDK-1.5.4/test/test_circuit/test_CircuitFlow.py
+-rw-rw-rw-   0        0        0     7331 2023-06-26 10:46:07.000000 QuantumPathQSOAPySDK-1.5.4/test/test_circuit/test_CircuitGates.py
+-rw-rw-rw-   0        0        0   157579 2023-06-26 10:26:09.000000 QuantumPathQSOAPySDK-1.5.4/test/test_circuit/test_CircuitGates_gates1.py
+-rw-rw-rw-   0        0        0    35843 2023-06-26 10:26:50.000000 QuantumPathQSOAPySDK-1.5.4/test/test_circuit/test_CircuitGates_gates2.py
```

### Comparing `QuantumPathQSOAPySDK-1.5.3/PKG-INFO` & `QuantumPathQSOAPySDK-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumPathQSOAPySDK
-Version: 1.5.3
+Version: 1.5.4
 Summary: QuantumPath qSOA Python SDK
 Home-page: https://core.quantumpath.app/
 Author: QuantumPath
 License: UNKNOWN
 Keywords: quantum,quantumpath,qSOA,sdk,quantum applications,quantum software
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/QSOAPlatform.py` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/QSOAPlatform.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,17 @@
         updateAsset as __updateAsset,
         updateAssetSync as __updateAssetSync,
         getAssetManagementResult as __getAssetManagementResult,
         deleteAsset as __deleteAsset,
         getQuantumExecutionHistoric as __getQuantumExecutionHistoric,
         getQuantumExecutionHistoricResult as __getQuantumExecutionHistoricResult,
     )
-    from .circuit.annealing.CircuitAnnealing import CircuitAnnealing
-    from .circuit.flow.CircuitFlow import CircuitFlow
-    from .circuit.gates.CircuitGates import CircuitGates
+    from .circuit.annealing.CircuitAnnealing import CircuitAnnealing as __CircuitAnnealing
+    from .circuit.flow.CircuitFlow import CircuitFlow as __CircuitFlow
+    from .circuit.gates.CircuitGates import CircuitGates as __CircuitGates
 
     # CONSTRUCTOR
     def __init__(self, username: str = None, password: str = None, configFile: bool = False):
         """
         QSOAPlatform object constructor.
 
         Prerequisites
@@ -880,15 +880,15 @@
         """
         checkUserSession(self.__context)
         checkInputTypes(
             ('idSolution', idSolution, (int,)),
             ('assetName', assetName, (str,)),
             ('assetNamespace', assetNamespace, (str,)),
             ('assetDescription', assetDescription, (str,)),
-            ('assetBody', assetBody, (str, self.CircuitGates, self.CircuitAnnealing, self.CircuitFlow)),
+            ('assetBody', assetBody, (str, self.__CircuitGates, self.__CircuitAnnealing, self.__CircuitFlow)),
             ('assetType', assetType, (str,)),
             ('assetLevel', assetLevel, (str,))
         )
         checkValues(
             ('assetType', assetType, ['GATES', 'ANNEAL', 'FLOW']),
             ('assetLevel', assetLevel, ['VL', 'IL'])
         )
@@ -929,15 +929,15 @@
         """
         checkUserSession(self.__context)
         checkInputTypes(
             ('idSolution', idSolution, (int,)),
             ('assetName', assetName, (str,)),
             ('assetNamespace', assetNamespace, (str,)),
             ('assetDescription', assetDescription, (str,)),
-            ('assetBody', assetBody, (str, self.CircuitGates, self.CircuitAnnealing, self.CircuitFlow)),
+            ('assetBody', assetBody, (str, self.__CircuitGates, self.__CircuitAnnealing, self.__CircuitFlow)),
             ('assetType', assetType, (str,)),
             ('assetLevel', assetLevel, (str,))
         )
         checkValues(
             ('assetType', assetType, ['GATES', 'ANNEAL', 'FLOW']),
             ('assetLevel', assetLevel, ['VL', 'IL'])
         )
@@ -978,15 +978,15 @@
         """
         checkUserSession(self.__context)
         checkInputTypes(
             ('idSolution', idSolution, (int,)),
             ('assetName', assetName, (str,)),
             ('assetNamespace', assetNamespace, (str,)),
             ('assetDescription', assetDescription, (str,)),
-            ('assetBody', assetBody, (str, self.CircuitFlow)),
+            ('assetBody', assetBody, (str, self.__CircuitFlow)),
             ('assetLevel', assetLevel, (str,)),
             ('publish', publish, (bool,))
         )
         checkValues(
             ('assetLevel', assetLevel, ['VL', 'IL'])
         )
 
@@ -1026,15 +1026,15 @@
         """
         checkUserSession(self.__context)
         checkInputTypes(
             ('idSolution', idSolution, (int,)),
             ('assetName', assetName, (str,)),
             ('assetNamespace', assetNamespace, (str,)),
             ('assetDescription', assetDescription, (str,)),
-            ('assetBody', assetBody, (str, self.CircuitFlow)),
+            ('assetBody', assetBody, (str, self.__CircuitFlow)),
             ('assetLevel', assetLevel, (str,)),
             ('publish', publish, (bool,))
         )
         checkValues(
             ('assetLevel', assetLevel, ['VL', 'IL'])
         )
 
@@ -1115,15 +1115,15 @@
             )
         if assetDescription:
             checkInputTypes(
                 ('assetDescription', assetDescription, (str,))
             )
         if assetBody:
             checkInputTypes(
-                ('assetBody', assetBody, (str, self.CircuitGates, self.CircuitAnnealing, self.CircuitFlow)),
+                ('assetBody', assetBody, (str, self.__CircuitGates, self.__CircuitAnnealing, self.__CircuitFlow)),
                 ('assetType', assetType, (str,)),
                 ('assetLevel', assetLevel, (str,))
             )
             checkValues(
                 ('assetType', assetType, ['GATES', 'ANNEAL', 'FLOW']),
                 ('assetLevel', assetLevel, ['VL', 'IL'])
             )
@@ -1176,15 +1176,15 @@
             )
         if assetDescription:
             checkInputTypes(
                 ('assetDescription', assetDescription, (str,))
             )
         if assetBody:
             checkInputTypes(
-                ('assetBody', assetBody, (str, self.CircuitGates, self.CircuitAnnealing, self.CircuitFlow)),
+                ('assetBody', assetBody, (str, self.__CircuitGates, self.__CircuitAnnealing, self.__CircuitFlow)),
                 ('assetType', assetType, (str,)),
                 ('assetLevel', assetLevel, (str,))
             )
             checkValues(
                 ('assetType', assetType, ['GATES', 'ANNEAL', 'FLOW']),
                 ('assetLevel', assetLevel, ['VL', 'IL'])
             )
@@ -1342,8 +1342,62 @@
         QuantumExecutionHistoryEntry obj
         """
         checkUserSession(self.__context)
         checkInputTypes(
             ('idResult', idResult, (int,))
         )
 
-        return self.__getQuantumExecutionHistoricResult(self.__context, idResult)
+        return self.__getQuantumExecutionHistoricResult(self.__context, idResult)
+
+
+    ##################_____CIRCUIT METHODS_____##################
+
+    # CIRCUIT ANNEALING
+    def CircuitAnnealing(self):
+        """
+        CircuitAnnealing object constructor.
+
+        Prerequisites
+        ----------
+        - User already authenticated.
+
+        Output
+        ----------
+        CircuitAnnealing obj
+        """
+        checkUserSession(self.__context)
+
+        return self.__CircuitAnnealing()
+    
+    # CIRCUIT FLOW
+    def CircuitFlow(self):
+        """
+        CircuitFlow object constructor.
+
+        Prerequisites
+        ----------
+        - User already authenticated.
+
+        Output
+        ----------
+        CircuitFlow obj
+        """
+        checkUserSession(self.__context)
+
+        return self.__CircuitFlow()
+    
+    # CIRCUIT GATES
+    def CircuitGates(self):
+        """
+        CircuitGates object constructor.
+
+        Prerequisites
+        ----------
+        - User already authenticated.
+
+        Output
+        ----------
+        CircuitGates obj
+        """
+        checkUserSession(self.__context)
+
+        return self.__CircuitGates()
```

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ...utils.checker import (checkInputTypes)
+from ...utils.checker import (checkInputTypes, checkListTypes)
 
 class CircuitAnnealing:
     from .components import (
         Parameter,
         AuxData,
         Class,
         Variable,
@@ -12,26 +12,14 @@
         QuadraticExp,
         SquaredExp,
         SummationExp
     )
     
     # CONSTRUCTOR
     def __init__(self):
-        """
-        CircuitAnnealing object constructor.
-
-        Prerequisites
-        ----------
-        None.
-
-        Output
-        ----------
-        CircuitAnnealing obj
-        """
-
         self.__parameters = []
         self.__auxData = []
         self.__classes = []
         self.__variables = []
         self.__rules = []
 
         self.__circuitBody = {
@@ -177,19 +165,15 @@
                 'Value': parameter.getValue()
             })
 
         checkInputTypes(
             ('parameter', parameter, (self.Parameter, list))
         )
         if isinstance(parameter, list):
-            if not parameter:
-                raise ValueError('List of parameters should not be empty')
-
-            for p in parameter:
-                checkInputTypes(('parameter', p, (self.Parameter,)))
+            checkListTypes(('parameter', parameter, (self.Parameter,)))
 
             for p in parameter:
                 appendParameter(p)
         
         else:
             appendParameter(parameter)
         
@@ -219,19 +203,15 @@
                 'Value': auxData.getValue()
             })
 
         checkInputTypes(
             ('auxData', auxData, (self.AuxData, list))
         )
         if isinstance(auxData, list):
-            if not auxData:
-                raise ValueError('List of auxiliary data should not be empty')
-
-            for a in auxData:
-                checkInputTypes(('auxData', a, (self.AuxData,)))
+            checkListTypes(('auxData', auxData, (self.AuxData,)))
 
             for a in auxData:
                 appendAuxData(a)
         
         else:
             appendAuxData(auxData)
         
@@ -260,22 +240,18 @@
                 'uiID': cls.getUiID(),
                 'Name': cls.getName(),
                 'NumberOfVars': cls.getNumberOfVars(),
                 'Description': cls.getDescription()
             })
 
         checkInputTypes(
-            ('circuitClass', cls, (self.Class, list))
+            ('cls', cls, (self.Class, list))
         )
         if isinstance(cls, list):
-            if not cls:
-                raise ValueError('List of classes should not be empty')
-
-            for c in cls:
-                checkInputTypes(('cls', c, (self.Class,)))
+            checkListTypes(('cls', cls, (self.Class,)))
 
             for c in cls:
                 appendClass(c)
         
         else:
             appendClass(cls)
 
@@ -306,19 +282,15 @@
                 'Description': variable.getDescription()
             })
 
         checkInputTypes(
             ('variable', variable, (self.Variable, list))
         )
         if isinstance(variable, list):
-            if not variable:
-                raise ValueError('List of variables should not be empty')
-
-            for v in variable:
-                checkInputTypes(('variable', v, (self.Variable,)))
+            checkListTypes(('variable', variable, (self.Variable,)))
 
             for v in variable:
                 appendVariable(v)
         
         else:
             appendVariable(variable)
         
@@ -351,19 +323,15 @@
                 'Disabled': rule.getDisabled()
             })
 
         checkInputTypes(
             ('rule', rule, (self.Rule, list))
         )
         if isinstance(rule, list):
-            if not rule:
-                raise ValueError('List of rules should not be empty')
-
-            for r in rule:
-                checkInputTypes(('rule', r, (self.Rule,)))
+            checkListTypes(('rule', rule, (self.Rule,)))
 
             for r in rule:
                 appendRule(r)
         
         else:
             appendRule(rule)
```

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/circuit/annealing/components.py` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/annealing/components.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ...utils.checker import (checkInputTypes, checkMathExpression)
+from ...utils.checker import (checkInputTypes, checkListTypes, checkMathExpression)
 import uuid
 
 
 ##################_____PRIVATE CLASSES_____##################
 
 # EXPRESSION
 class __Expression():
@@ -175,15 +175,15 @@
 
 ##################_____PUBLIC CLASSES_____##################
 
 # PARAMETER
 class Parameter:
 
     # CONSTRUCTOR
-    def __init__(self, name: str, value: int):
+    def __init__(self, name: str, value):
         """
         Create Circuit Parameter.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -200,14 +200,47 @@
         )
         if isinstance(value, str):
             checkMathExpression('value', value)
         
         self.__uiID = str(uuid.uuid4())
         self.__name = name
         self.__value = str(value)
+    
+    
+    # MAGIC METHODS
+    def __add__(self, other):
+        if isinstance(other, (int, float, str)):
+            return f'{self.__name} + {other}'
+
+        elif isinstance(other, Parameter):
+            return f'{self.__name} + {other.__name}'
+
+    def __sub__(self, other):
+        if isinstance(other, (int, float, str)):
+            return f'{self.__name} - {other}'
+
+        elif isinstance(other, Parameter):
+            return f'{self.__name} - {other.__name}'
+
+    def __mul__(self, other):
+        if isinstance(other, (int, float, str)):
+            return f'{self.__name} * {other}'
+
+        elif isinstance(other, Parameter):
+            return f'{self.__name} * {other.__name}'
+
+    def __truediv__(self, other):
+        if isinstance(other, (int, float, str)):
+            return f'{self.__name} / {other}'
+
+        elif isinstance(other, Parameter):
+            return f'{self.__name} / {other.__name}'
+
+    def __neg__(self):
+        return f'-{self.__name}'
 
 
     # GETTERS
     def getUiID(self):
         """
         Get Circuit Parameter uiID.
 
@@ -250,15 +283,15 @@
         return self.__value
 
 
 # AUXDATA
 class AuxData:
     
     # CONSTRUCTOR
-    def __init__(self, name: str, value: int):
+    def __init__(self, name: str, value):
         """
         Create Circuit Auxiliary Data.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -270,19 +303,15 @@
             Auxiliary Data value or list of values.
         """
         checkInputTypes(
             ('name', name, (str,)),
             ('value', value, (int, float, list))
         )
         if isinstance(value, list):
-            if not value:
-                raise ValueError('List of values should not be empty')
-
-            for v in value:
-                checkInputTypes(('value', v, (int, float)))
+            checkListTypes(('value', value, (int, float, list)))
 
         self.__uiID = str(uuid.uuid4())
         self.__name = name
         self.__value = str(value)
     
 
     # GETTERS
@@ -329,15 +358,15 @@
         return self.__value
     
 
 # CLASS
 class Class:
 
     # CONSTRUCTOR
-    def __init__(self, name: str, numberOfVars: int, description: str = ''):
+    def __init__(self, name: str, numberOfVars, description: str = ''):
         """
         Create Circuit Class.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -355,15 +384,16 @@
             ('numberOfVars', numberOfVars, (int, Parameter)),
             ('description', description, (str,))
         )
 
         self.__properties = []
         self.__uiID = str(uuid.uuid4())
         self.__name = name
-        self.__numberOfVars = str(numberOfVars) if isinstance(numberOfVars, int) else numberOfVars.getValue()
+        self.__numberOfVars = str(numberOfVars) if isinstance(numberOfVars, int) else numberOfVars.getName()
+        self.__intNumberOfVars = numberOfVars if isinstance(numberOfVars, int) else numberOfVars.getValue()
         self.__description = description
 
 
     # GETTERS
     def getProperties(self):
         """
         Get Circuit Class properties.
@@ -451,18 +481,17 @@
         value : list
             List of property values. It may be the same that Class number of variables.
         """
         checkInputTypes(
             ('name', name, (str,)),
             ('value', value, (list,))
         )
-        for v in value:
-            checkInputTypes(('value', v, (int,)))
+        checkListTypes(('value', value, (int,)))
 
-        if len(value) != int(self.__numberOfVars): # number of values and number of vars are not the same
+        if len(value) != int(self.__intNumberOfVars): # number of values and number of vars are not the same
             raise ValueError('Quantity of property values and number of variables must be the same')
         
         self.__properties.append({
             'uiID': str(uuid.uuid4()),
             'Name': name,
             'Values': list(map(str, value))
         })
@@ -496,19 +525,15 @@
             ('classes', classes, (Class, list)),
             ('description', description, (str,))
         )
 
         self.__classes = []
         
         if isinstance(classes, list):
-            if not classes:
-                raise ValueError('List of classes should not be empty')
-
-            for c in classes:
-                checkInputTypes(('classes', c, (Class,)))
+            checkListTypes(('classes', classes, (Class,)))
 
             for c in classes:
                 self.__classes.append(c.getUiID())
         
         else:
             self.__classes.append(classes.getUiID())
 
@@ -574,15 +599,15 @@
         return self.__description
 
 
 # RULE
 class Rule:
 
     # CONSTRUCTOR
-    def __init__(self, name: str, lambdaValue: int, description = '', disabled = False):
+    def __init__(self, name: str, lambdaValue, description = '', disabled = False):
         """
         Create Circuit Rule.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -737,150 +762,157 @@
                 'Childs': expression.getChilds()
             })
 
         checkInputTypes(
             ('expression', expression, (SummationExp, SquaredExp, LinearExp, QuadraticExp, OffsetExp, list))
         )
         if isinstance(expression, list):
-            if not expression:
-                raise ValueError('List of expressions should not be empty')
-            
-            for e in expression:
-                checkInputTypes(
-                    ('expression', e, (SummationExp, SquaredExp, LinearExp, QuadraticExp, OffsetExp, list))
-                )
+            checkListTypes(('expression', expression, (SummationExp, SquaredExp, LinearExp, QuadraticExp, OffsetExp)))
 
             for e in expression:
                 appendExpression(e)
         
         else:
             appendExpression(expression)
 
         return self
 
 
 # OFFSET EXPRESSION
 class OffsetExp(__Expression):
     
     # CONSTRUCTOR
-    def __init__(self, offset: int): 
+    def __init__(self, offset): 
         """
         Create Offset expression.
 
         Prerequisites
         ----------
         - Created rule.
 
         Parameters
         ----------
-        offset : int | float | str
+        offset : int | float | str | Parameter
             Offset value.
         """
         checkInputTypes(
-            ('offset', offset, (int, float, str))
+            ('offset', offset, (int, float, str, Parameter))
         )
 
+        if isinstance(offset, Parameter):
+            offset = offset.getName()
+
         super().__init__(expType='OFFSET', offset=str(offset))
 
 
 # LINEAR EXPRESSION
 class LinearExp(__Expression):
     
     # CONSTRUCTOR
-    def __init__(self, variable: tuple, coefficient: int = ''):
+    def __init__(self, variable: tuple, coefficient = ''):
         """
         Create Linear expression.
 
         Prerequisites
         ----------
         - Created rule.
 
         Parameters
         ----------
         variable: tuple
             Circuit variable and values. First element: Variable obj. Second element: value or list of values (One per class in variable).
-        coefficient : int | float | str
+        coefficient : int | float | str | Parameter
             Optional argument. Coefficient value.
         """
-        def appendIndex(term: dict, variable: Variable, index: int):
-            term['Indexes'].append({
+        def appendIndex(termIndexes: dict, variable: Variable, index: int):
+            if isinstance(variable[1], list):
+                value = variable[1][index].getName() if isinstance(variable[1][index], Parameter) else str(variable[1][index])
+            else:
+                value = variable[1].getName() if isinstance(variable[1], Parameter) else str(variable[1])
+
+            termIndexes.append({
                 'uiID': str(uuid.uuid4()),
-                'Value': str(variable[1][index]) if isinstance(variable[1], list) else str(variable[1]),
+                'Value': value,
                 'ClassID': variable[0].getClasses()[index]
             })
 
         def checkVariablesAndClasses(variable):
             numberOfClasses = len(variable[0].getClasses())
 
             if isinstance(variable[1], list):
                 if len(variable[1]) != numberOfClasses:
-                    raise ValueError(f'Expected {numberOfClasses} variable values, not {len(variable[1])}')
-                
+                    raise ValueError(f'Expected {numberOfClasses} variable values, not {len(variable[1])}')  
             else:
                 if numberOfClasses != 1:
                     raise ValueError(f'Expected {numberOfClasses} variable values, not 1')
         
         if isinstance(variable, tuple):
             if len(variable) != 2: # number of variable elements are not 2
                 raise ValueError('variable takes 2 positional arguments')
         
         checkInputTypes(
             ('variable', variable, (tuple,)),
             ('variable', variable[0], (Variable,)),
-            ('variable', variable[1], (int, float, str, list)),
-            ('coefficient', coefficient, (int, float, str))
+            ('variable', variable[1], (int, float, str, Parameter, list)),
+            ('coefficient', coefficient, (int, float, str, Parameter))
         )
         if isinstance(variable[1], list):
-            for v in variable[1]:
-                checkInputTypes(('variable', v, (int, float, str)))
+            checkListTypes(('variable', variable[1], (int, float, str, Parameter)))
         
         checkVariablesAndClasses(variable) # check number of variable numbers are the same that variable classes
 
         term1 = {
             'Indexes': [],
             'uiID': str(uuid.uuid4()),
             'VariableID': variable[0].getUiID()
         }
 
         if isinstance(variable[1], list):
             for index in range(0, len(variable[1])):
-                appendIndex(term1, variable, index)
-        
+                appendIndex(term1['Indexes'], variable, index)
         else:
-            appendIndex(term1, variable, 0)
+            appendIndex(term1['Indexes'], variable, 0)
+        
+        if isinstance(coefficient, Parameter):
+            coefficient = coefficient.getName()
 
         super().__init__(expType='LINEAR', coefficient=str(coefficient), term1=term1)
 
 
 # QUADRATIC EXPRESSION
 class QuadraticExp(__Expression):
     
     # CONSTRUCTOR
-    def __init__(self, variable1: tuple, variable2: tuple, coefficient: int = ''): 
+    def __init__(self, variable1: tuple, variable2: tuple, coefficient = ''): 
 
         """
         Add Quadratic expression.
 
         Prerequisites
         ----------
         - Created rule.
 
         Parameters
         ----------
         variable1: tuple
             Circuit variable and values. First element: Variable obj. Second element: value or list of values (One per class in variable).
         variable2: tuple
             Circuit variable and values. First element: Variable obj. Second element: value or list of values (One per class in variable).
-        coefficient : int | float | str
+        coefficient : int | float | str | Parameter
             Optional argument. Coefficient value.
         """
-        def appendIndex(term: dict, variable: Variable, index: int):
-            term['Indexes'].append({
+        def appendIndex(termIndexes: dict, variable: Variable, index: int):
+            if isinstance(variable[1], list):
+                value = variable[1][index].getName() if isinstance(variable[1][index], Parameter) else str(variable[1][index])
+            else:
+                value = variable[1].getName() if isinstance(variable[1], Parameter) else str(variable[1])
+
+            termIndexes.append({
                 'uiID': str(uuid.uuid4()),
-                'Value': str(variable[1][index]) if isinstance(variable[1], list) else str(variable[1]),
+                'Value': value,
                 'ClassID': variable[0].getClasses()[index]
             })
 
         def checkVariablesAndClasses(variable):
             numberOfClasses = len(variable[0].getClasses())
 
             if isinstance(variable[1], list):
@@ -897,26 +929,24 @@
         if isinstance(variable2, tuple):
             if len(variable2) != 2: # number of variable2 elements are not 2
                 raise ValueError('variable2 takes 2 positional arguments')
         
         checkInputTypes(
             ('variable1', variable1, (tuple,)),
             ('variable1', variable1[0], (Variable,)),
-            ('variable1', variable1[1], (int, float, str, list)),
+            ('variable1', variable1[1], (int, float, str, Parameter, list)),
             ('variable2', variable2, (tuple,)),
             ('variable2', variable2[0], (Variable,)),
-            ('variable2', variable2[1], (int, float, str, list)),
-            ('coefficient', coefficient, (int, float, str))
+            ('variable2', variable2[1], (int, float, str, Parameter, list)),
+            ('coefficient', coefficient, (int, float, str, Parameter))
         )
         if isinstance(variable1[1], list):
-            for v in variable1[1]:
-                checkInputTypes(('variable1', v, (int, float, str)))
+            checkListTypes(('variable1', variable1[1], (int, float, str, Parameter)))
         if isinstance(variable2[1], list):
-            for v in variable2[1]:
-                checkInputTypes(('variable2', v, (int, float, str)))
+            checkListTypes(('variable2', variable2[1], (int, float, str, Parameter)))
 
         checkVariablesAndClasses(variable1) # check number of variable numbers are the same that variable classes
         checkVariablesAndClasses(variable2)
 
         term1 = {
             'Indexes': [],
             'uiID': str(uuid.uuid4()),
@@ -927,23 +957,26 @@
             'Indexes': [],
             'uiID': str(uuid.uuid4()),
             'VariableID': variable2[0].getUiID()
         }
 
         if isinstance(variable1[1], list):
             for index in range(0, len(variable1[1])):
-                appendIndex(term1, variable1, index)
+                appendIndex(term1['Indexes'], variable1, index)
         else:
-            appendIndex(term1, variable1, 0)
+            appendIndex(term1['Indexes'], variable1, 0)
         
         if isinstance(variable2[1], list):
             for index in range(0, len(variable2[1])):
-                appendIndex(term2, variable2, index)
+                appendIndex(term2['Indexes'], variable2, index)
         else:
-            appendIndex(term2, variable2, 0)
+            appendIndex(term2['Indexes'], variable2, 0)
+        
+        if isinstance(coefficient, Parameter):
+            coefficient = coefficient.getName()
 
         super().__init__(expType='QUADRATIC', coefficient=str(coefficient), term1=term1, term2=term2)
 
 
 # SQUARED EXPRESSION
 class SquaredExp(__Expression):
     
@@ -976,45 +1009,42 @@
                 'Childs': expression.getChilds()
             })
 
         checkInputTypes(
             ('expression', expression, (SummationExp, LinearExp, OffsetExp, list))
         )
         if isinstance(expression, list):
-            if not expression:
-                raise ValueError('List of expressions should not be empty')
-            for e in expression:
-                checkInputTypes(('expression', e, (SummationExp, LinearExp, OffsetExp, list)))
-            if isinstance(expression, list):
-                for exp in expression:
-                    appendChild(exp)
+            checkListTypes(('expression', expression, (SummationExp, LinearExp, OffsetExp)))
+
+            for exp in expression:
+                appendChild(exp)
         
         else:
             appendChild(expression)
 
         super().__init__(expType='SQUARED', childs=childs)
 
 
 # SUMMATION EXPRESSION
 class SummationExp(__Expression):
     
     # CONSTRUCTOR
-    def __init__(self, fromValue: int, toValue: int, expression, iterator: str = 'i'): 
+    def __init__(self, fromValue, toValue, expression, iterator: str = 'i'): 
         """
         Create Summation expression.
 
         Prerequisites
         ----------
         - Created rule.
 
         Parameters
         ----------
-        fromValue: int | float | str
+        fromValue: int | float | str | Parameter
             Start value of the summation iteration.
-        toValue: int | float | str
+        toValue: int | float | str | Parameter
             End value of the summation iteration.
         expression: SummationExp obj | SquaredExp obj | LinearExp obj | QuadraticExp obj | OffsetExp obj | list
             Expression or list of expressions to be inside of the summation. It could be a Summation, Squared, Linear, Quadratic or Offset expression.
         iterator: str
             Iterator name.
         """
         childs = []
@@ -1029,27 +1059,27 @@
                 'Iterator': expression.getIterator(),
                 'Term1': expression.getTerm1(),
                 'Term2': expression.getTerm2(),
                 'Childs': expression.getChilds()
             })
 
         checkInputTypes(
-            ('fromValue', fromValue, (int, float, str)),
-            ('toValue', toValue, (int, float, str)),
+            ('fromValue', fromValue, (int, float, str, Parameter)),
+            ('toValue', toValue, (int, float, str, Parameter)),
             ('expression', expression, (SummationExp, SquaredExp, LinearExp, QuadraticExp, OffsetExp, list)),
             ('iterator', iterator, (str,)),
         )
         if isinstance(expression, list):
-            if not expression:
-                raise ValueError('List of expressions should not be empty')
-            for e in expression:
-                checkInputTypes(
-                    ('expression', e, (SummationExp, SquaredExp, LinearExp, QuadraticExp, OffsetExp, list))
-                )
-            if isinstance(expression, list):
-                for exp in expression:
-                    appendChild(exp)
+            checkListTypes(('expression', expression, (SummationExp, SquaredExp, LinearExp, QuadraticExp, OffsetExp)))
+
+            for exp in expression:
+                appendChild(exp)
         
         else:
             appendChild(expression)
+        
+        if isinstance(fromValue, Parameter):
+            fromValue = fromValue.getName()
+        if isinstance(toValue, Parameter):
+            toValue = toValue.getName()
 
         super().__init__(expType='SUMMATORY', fromValue=str(fromValue), toValue=str(toValue), iterator=iterator, childs=childs)
```

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from ...utils.checker import checkInputTypes
 
 class CircuitFlow:
-    """
-    Create Flow.
-    """
     
     # CONSTRUCTOR
     def __init__(self):
         self.__nodeData = []
         self.__linkData = []
         self.__keyValue = -1
```

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,13 @@
-from ...utils.checker import checkInputTypes, checkValues, checkMathExpression, checkDifferentPosition
+from ...utils.checker import (checkInputTypes, checkListTypes, checkValues, checkMathExpression, checkDifferentPosition)
 
 class CircuitGates:
 
     # CONSTRUCTOR
     def __init__(self):
-        """
-        CircuitGates object constructor.
-
-        Prerequisites
-        ----------
-        None.
-
-        Output
-        ----------
-        CircuitGates obj
-        """
-
         self.__circuitBody = [[]]
         self.__qubitStates = []
         self.__numerOfQubits = 0
         self.__defaultQubitState = '0'
 
         self.__circuitVLStructure = {
             'cols': self.__circuitBody,
@@ -252,15 +240,15 @@
             checkValues(('qubitStates', qubitState, ['0', '1', '+', '-', 'i', '-i']))
         
         if len(qubitStates) != self.__numerOfQubits:
             raise ValueError(f'Incorrect number of qubit states. Input states are {len(qubitStates)} and should be {self.__numerOfQubits}')
 
         self.__qubitStates = qubitStates
 
-    def h(self, position: int = None, add: bool = True) -> list: # hadamard gate
+    def h(self, position = None, add: bool = True) -> list: # hadamard gate
         """
         Add Hadamard gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -271,21 +259,20 @@
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('add', add, (bool,))
         )
 
         gateSymbol = 'H'
 
@@ -295,15 +282,15 @@
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
             
         self.__updateQubits()
         
         return positions
 
-    def x(self, position: int = None, add: bool = True) -> list: # not gate
+    def x(self, position = None, add: bool = True) -> list: # not gate
         """
         Add Pauli X gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -314,21 +301,20 @@
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('add', add, (bool,))
         )
         
         gateSymbol = 'X'
 
@@ -338,15 +324,15 @@
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
         self.__updateQubits()
         
         return positions
     
-    def y(self, position: int = None, add: bool = True) -> list: # pauli y gate
+    def y(self, position = None, add: bool = True) -> list: # pauli y gate
         """
         Add Pauli Y gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -357,21 +343,20 @@
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('add', add, (bool,))
         )
 
         gateSymbol = 'Y'
 
@@ -381,15 +366,15 @@
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
         self.__updateQubits()
         
         return positions
 
-    def z(self, position: int = None, add: bool = True) -> list: # pauli z gate
+    def z(self, position = None, add: bool = True) -> list: # pauli z gate
         """
         Add Pauli Z gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -400,21 +385,20 @@
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('add', add, (bool,))
         )
 
         gateSymbol = 'Z'
 
@@ -424,15 +408,15 @@
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
         self.__updateQubits()
         
         return positions
 
-    def s(self, position: int = None, add: bool = True) -> list: # square root of z, s gate
+    def s(self, position = None, add: bool = True) -> list: # square root of z, s gate
         """
         Add Square root of Z, S gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -443,21 +427,20 @@
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('add', add, (bool,))
         )
 
         gateSymbol = 'S'
 
@@ -467,15 +450,15 @@
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
         self.__updateQubits()
         
         return positions
 
-    def i_s(self, position: int = None, add: bool = True) -> list: # Adjoint square root z gate
+    def i_s(self, position = None, add: bool = True) -> list: # Adjoint square root z gate
         """
         Add Adjoint square root Z gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -486,21 +469,20 @@
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('add', add, (bool,))
         )
 
         gateSymbol = 'I_S'
 
@@ -510,15 +492,15 @@
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
         self.__updateQubits()
         
         return positions
 
-    def sx(self, position: int = None, add: bool = True) -> list: # square root of not gate
+    def sx(self, position = None, add: bool = True) -> list: # square root of not gate
         """
         Add Square root of X gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -529,21 +511,20 @@
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('add', add, (bool,))
         )
 
         gateSymbol = 'SX'
 
@@ -553,15 +534,15 @@
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
         self.__updateQubits()
         
         return positions
 
-    def i_sx(self, position: int = None, add: bool = True) -> list: # adjoint square root X gate
+    def i_sx(self, position = None, add: bool = True) -> list: # adjoint square root X gate
         """
         Add Adjoint square root X gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -572,21 +553,20 @@
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('add', add, (bool,))
         )
 
         gateSymbol = 'I_SX'
 
@@ -596,15 +576,15 @@
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
         self.__updateQubits()
         
         return positions
 
-    def sy(self, position: int = None, add: bool = True) -> list: # square root of y gate
+    def sy(self, position = None, add: bool = True) -> list: # square root of y gate
         """
         Add Square root of Y gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -615,21 +595,20 @@
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('add', add, (bool,))
         )
 
         gateSymbol = 'SY'
 
@@ -639,15 +618,15 @@
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
         self.__updateQubits()
         
         return positions
 
-    def i_sy(self, position: int = None, add: bool = True) -> list: # adjoint square root y gate
+    def i_sy(self, position = None, add: bool = True) -> list: # adjoint square root y gate
         """
         Add Adjoint square root Y gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -658,21 +637,20 @@
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('add', add, (bool,))
         )
 
         gateSymbol = 'I_SY'
 
@@ -682,15 +660,15 @@
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
         self.__updateQubits()
         
         return positions
 
-    def t(self, position: int = None, add: bool = True) -> list: # four root of z, t gate
+    def t(self, position = None, add: bool = True) -> list: # four root of z, t gate
         """
         Add Four root of Z, T gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -701,21 +679,20 @@
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('add', add, (bool,))
         )
 
         gateSymbol = 'T'
 
@@ -725,15 +702,15 @@
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
         self.__updateQubits()
         
         return positions
 
-    def i_t(self, position: int = None, add: bool = True) -> list: # adjoint four root z gate
+    def i_t(self, position = None, add: bool = True) -> list: # adjoint four root z gate
         """
         Add Adjoint four root Z gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -744,21 +721,20 @@
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('add', add, (bool,))
         )
 
         gateSymbol = 'I_T'
 
@@ -768,15 +744,15 @@
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
         self.__updateQubits()
         
         return positions
 
-    def tx(self, position: int = None, add: bool = True) -> list: # four root of x gate
+    def tx(self, position = None, add: bool = True) -> list: # four root of x gate
         """
         Add four root of X gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -787,21 +763,20 @@
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('add', add, (bool,))
         )
 
         gateSymbol = 'TX'
 
@@ -811,15 +786,15 @@
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
         self.__updateQubits()
         
         return positions
 
-    def i_tx(self, position: int = None, add: bool = True) -> list: # adjoint four root X gate
+    def i_tx(self, position = None, add: bool = True) -> list: # adjoint four root X gate
         """
         Add Adjoint four root X gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -830,21 +805,20 @@
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('add', add, (bool,))
         )
 
         gateSymbol = 'I_TX'
         
@@ -854,15 +828,15 @@
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
         self.__updateQubits()
         
         return positions
 
-    def ty(self, position: int = None, add: bool = True) -> list: # four root of y gate
+    def ty(self, position = None, add: bool = True) -> list: # four root of y gate
         """
         Add four root of Y gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -873,21 +847,20 @@
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('add', add, (bool,))
         )
 
         gateSymbol = 'TY'
 
@@ -897,40 +870,39 @@
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
         self.__updateQubits()
         
         return positions
 
-    def i_ty(self, position: int = None, add: bool = True) -> list: # adjoint four root y gate
+    def i_ty(self, position = None, add: bool = True) -> list: # adjoint four root y gate
         """
         Add Adjoint four root Y gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
-        position : int | list | list
+        position : int | list
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('add', add, (bool,))
         )
 
         gateSymbol = 'I_TY'
 
@@ -940,15 +912,15 @@
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
         self.__updateQubits()
         
         return positions
 
-    def p(self, position: int = None, argument = 'pi', add: bool = True) -> list: # phase gate
+    def p(self, position = None, argument = 'pi', add: bool = True) -> list: # phase gate
         """
         Add Phase gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -961,21 +933,20 @@
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('argument', argument, (str, int, float)),
             ('add', add, (bool,))
         )
         if isinstance(argument, str):
             checkMathExpression('argument', argument)
@@ -988,15 +959,15 @@
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
         self.__updateQubits()
         
         return positions
 
-    def rx(self, position: int = None, argument = 'pi', add: bool = True) -> list: # rotation x gate
+    def rx(self, position = None, argument = 'pi', add: bool = True) -> list: # rotation x gate
         """
         Add Rotation X gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -1009,21 +980,20 @@
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('argument', argument, (str, int, float)),
             ('add', add, (bool,))
         )
         if isinstance(argument, str):
             checkMathExpression('argument', argument)
@@ -1036,15 +1006,15 @@
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
         self.__updateQubits()
         
         return positions
 
-    def ry(self, position: int = None, argument = 'pi', add: bool = True) -> list: # rotation y gate
+    def ry(self, position = None, argument = 'pi', add: bool = True) -> list: # rotation y gate
         """
         Add Rotation Y gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -1057,21 +1027,20 @@
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('argument', argument, (str, int, float)),
             ('add', add, (bool,))
         )
         if isinstance(argument, str):
             checkMathExpression('argument', argument)
@@ -1084,15 +1053,15 @@
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
         self.__updateQubits()
         
         return positions
 
-    def rz(self, position: int = None, argument = 'pi', add: bool = True) -> list: # rotation z gate
+    def rz(self, position = None, argument = 'pi', add: bool = True) -> list: # rotation z gate
         """
         Add Rotation Z gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -1105,21 +1074,20 @@
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
             ('argument', argument, (str, int, float)),
             ('add', add, (bool,))
         )
         if isinstance(argument, str):
             checkMathExpression('argument', argument)
@@ -1292,15 +1260,15 @@
         if add:
             self.__addMultipleGate(positions, self.__circuitBody) # add to circuit
         
         self.__updateQubits()
         
         return positions
 
-    def measure(self, position: int = None) -> list: # measure
+    def measure(self, position = None) -> list: # measure
         """
         Add Measure.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -1309,53 +1277,51 @@
         position : int | list
             Optional argument. Qubit position to add the measurement. In the case that the position is not indicated, the measurement will be added in all qubits. It can also be a list of positions.
         
         Output
         ----------
         list
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
 
         gateSymbol = 'Measure'
         
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         self.__addMultipleGate(positions, self.__circuitBody) # add to circuit
 
         self.__updateQubits()
         
         return positions
 
-    def barrier(self, position: int = None): # barrier
+    def barrier(self, position = None): # barrier
         """
         Add Barrier.
 
         Prerequisites
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int | list
             Optional argument. Qubit position to add the barrier. In the case that the position is not indicated, the barrier will be added in all qubits. It can also be a list of positions.
         """
-        if position:
+        if position or isinstance(position, list):
             checkInputTypes(
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
-                for p in position:
-                    checkInputTypes(('position', p, (int,)))
+                checkListTypes(('position', position, (int,)))
                 checkDifferentPosition(position)
 
         gateSymbol = 'SPACER'
 
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
         
         if position is None:
@@ -1363,15 +1329,15 @@
         
         else:
             for gate in positions: # to all gates
                 self.__addSimpleGate(gate[0], gate[1], self.__circuitBody) # add to circuit
         
         self.__updateQubits()
 
-    def beginRepeat(self, position: int, repetitions: int) -> list: # begin repeat
+    def beginRepeat(self, position, repetitions: int) -> list: # begin repeat
         """
         Add Begin Repeat.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -1386,16 +1352,15 @@
         ----------
         list
         """
         checkInputTypes(
             ('position', position, (int, list))
         )
         if isinstance(position, list):
-            for p in position:
-                checkInputTypes(('position', p, (int,)))
+            checkListTypes(('position', position, (int,)))
             checkDifferentPosition(position)
         checkInputTypes(
             ('repetitions', repetitions, (int,))
         )
 
         gateSymbol = {'id': 'BEGIN_R', 'arg': str(repetitions)}
         
@@ -1403,15 +1368,15 @@
 
         self.__addMultipleGate(positions, self.__circuitBody) # add to circuit
 
         self.__updateQubits()
         
         return positions
 
-    def endRepeat(self, position: int) -> list: # begin repeat
+    def endRepeat(self, position) -> list: # begin repeat
         """
         Add End Repeat.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -1424,29 +1389,28 @@
         ----------
         list
         """
         checkInputTypes(
             ('position', position, (int, list))
         )
         if isinstance(position, list):
-            for p in position:
-                checkInputTypes(('position', p, (int,)))
+            checkListTypes(('position', position, (int,)))
             checkDifferentPosition(position)
 
         gateSymbol = 'END_R'
         
         positions = self.__definePositions(position, gateSymbol, self.__circuitBody) # get gate position structure
 
         self.__addMultipleGate(positions, self.__circuitBody) # add to circuit
 
         self.__updateQubits()
         
         return positions
 
-    def control(self, position: int, circuit: list) -> list: # control
+    def control(self, position, circuit: list) -> list: # control
         """
         Add Control.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -1462,16 +1426,15 @@
         list
         """
         checkInputTypes(
             ('position', position, (int, list)),
             ('circuit', circuit, (list,))
         )
         if isinstance(position, list):
-            for p in position:
-                checkInputTypes(('position', p, (int,)))
+            checkListTypes(('position', position, (int,)))
             checkDifferentPosition(position)
 
         correctPosition = True
 
         for gate in circuit:
             if position in gate:
                 correctPosition = False
@@ -1502,15 +1465,15 @@
             ('gate', gate, (list,))
         )
 
         self.__addMultipleGate(gate, self.__circuitBody) # add to circuit
 
         self.__updateQubits()
 
-    def mcg(self, position: int, circuit: list, add: bool = True) -> list: # multi control gate
+    def mcg(self, position, circuit: list, add: bool = True) -> list: # multi control gate
         """
         Add Multi Control gate.
 
         Prerequisites
         ----------
         - Created circuit.
 
@@ -1529,16 +1492,15 @@
         """
         checkInputTypes(
             ('position', position, (int, list)),
             ('circuit', circuit, (list,)),
             ('add', add, (bool,)),
         )
         if isinstance(position, list):
-            for p in position:
-                checkInputTypes(('position', p, (int,)))
+            checkListTypes(('position', position, (int,)))
             checkDifferentPosition(position)
         
         gateSymbol = 'CTRL'
 
         if isinstance(position, int): # one postion
             circuit.append((position, gateSymbol))
```

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/objects/Application.py` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/Application.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/objects/Asset.py` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/Asset.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/objects/AssetManagementData.py` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/AssetManagementData.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/objects/AssetManagementResult.py` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/AssetManagementResult.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/objects/DeviceItem.py` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/DeviceItem.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/objects/Execution.py` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/Execution.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/qsoa/__init__.py` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/qsoa/__init__.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/qsoa/connectionPoints.py` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/qsoa/connectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/utils/Context.py` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/utils/Context.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/utils/Exception.py` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/utils/Exception.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK/utils/apiConnection.py` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK/utils/apiConnection.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK.egg-info/PKG-INFO` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumPathQSOAPySDK
-Version: 1.5.3
+Version: 1.5.4
 Summary: QuantumPath qSOA Python SDK
 Home-page: https://core.quantumpath.app/
 Author: QuantumPath
 License: UNKNOWN
 Keywords: quantum,quantumpath,qSOA,sdk,quantum applications,quantum software
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `QuantumPathQSOAPySDK-1.5.3/QuantumPathQSOAPySDK.egg-info/SOURCES.txt` & `QuantumPathQSOAPySDK-1.5.4/QuantumPathQSOAPySDK.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -41,8 +41,10 @@
 test/test_QSOAPlatform/test_DynamicMethods.py
 test/test_QSOAPlatform/test_QSOAPlatform.py
 test/test_QSOAPlatform/test_SecurityMethods.py
 test/test_QSOAPlatform/test_StaticMethods.py
 test/test_circuit/__init__.py
 test/test_circuit/test_CircuitAnnealing.py
 test/test_circuit/test_CircuitFlow.py
-test/test_circuit/test_CircuitGates.py
+test/test_circuit/test_CircuitGates.py
+test/test_circuit/test_CircuitGates_gates1.py
+test/test_circuit/test_CircuitGates_gates2.py
```

### Comparing `QuantumPathQSOAPySDK-1.5.3/setup.py` & `QuantumPathQSOAPySDK-1.5.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   'Intended Audience :: Developers',
   'Intended Audience :: Education',
   'Intended Audience :: Information Technology'
 ]
 
 setup(
   name='QuantumPathQSOAPySDK',
-  version='1.5.3',
+  version='1.5.4',
   description='QuantumPath qSOA Python SDK',
   long_description=open('README.md').read(),
   long_description_content_type = 'text/markdown',
   url='https://core.quantumpath.app/',
   author='QuantumPath',
   classifiers=classifiers,
   keywords='quantum, quantumpath, qSOA, sdk, quantum applications, quantum software',
```

### Comparing `QuantumPathQSOAPySDK-1.5.3/test/test_QSOAPlatform/test_ContextMethods.py` & `QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_ContextMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.3/test/test_QSOAPlatform/test_DynamicMethods.py` & `QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_DynamicMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.3/test/test_QSOAPlatform/test_QSOAPlatform.py` & `QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_QSOAPlatform.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.3/test/test_QSOAPlatform/test_SecurityMethods.py` & `QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_SecurityMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.3/test/test_QSOAPlatform/test_StaticMethods.py` & `QuantumPathQSOAPySDK-1.5.4/test/test_QSOAPlatform/test_StaticMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.3/test/test_circuit/test_CircuitAnnealing.py` & `QuantumPathQSOAPySDK-1.5.4/test/test_circuit/test_CircuitAnnealing.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,64 +21,74 @@
 
 
 ##################_____CIRCUITANNEALING_____##################
 class Test_CircuitAnnealing(unittest.TestCase):
 
     # CIRCUIT ANNEALING
     def test_CircuitAnnealing(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
-        self.assertIsInstance(circuit, qsoa.CircuitAnnealing)
+        self.assertEqual(type(circuit).__name__, 'CircuitAnnealing')
+
+    # NOT LOGGED IN
+    def test_CircuitAnnealing_notloggedIn(self):
+        qsoa = QSOAPlatform()
 
+        try:
+            qsoa.CircuitAnnealing()
+            raise Exception
+
+        except Exception as e:
+            self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 ##################_____GET CIRCUIT BODY_____##################
 class Test_GetCircuitBody(unittest.TestCase):
 
     # GET CIRCUIT BODY
     def test_getCircuitBody(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         circuitBody = circuit.getCircuitBody()
 
         self.assertIsInstance(circuitBody, dict)
         self.assertEqual(circuitBody, {'Parameters': [], 'AuxData': [], 'Classes': [], 'Variables': [], 'Rules': []})
 
 
 ##################_____GET PARSED BODY_____##################
 class Test_GetParsedBody(unittest.TestCase):
 
     # GET PARSED BODY EMPTY
     def test_getParsedBody_empty(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         parsedBody = circuit.getParsedBody()
 
         self.assertIsInstance(parsedBody, str)
         self.assertEqual(parsedBody, '{"Parameters": [], "AuxData": [], "Classes": [], "Variables": [], "Rules": []}')
 
 
 ##################_____GET PARAMETERS_____##################
 class Test_GetParameters(unittest.TestCase):
 
     # GET PARAMETERS EMPTY
     def test_getParameters_empty(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         parameters = circuit.getParameters()
 
         self.assertIsInstance(parameters, list)
         self.assertEqual(parameters, [])
 
     # GET PARAMETERS
     def test_getParameters(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         circuit.addParameter(circuit.Parameter('Parameter', 1))
 
         parameters = circuit.getParameters()
         removeUiID(parameters) # remove random uiID to validate behaviour
 
         self.assertIsInstance(parameters, list)
@@ -87,25 +97,25 @@
 
 
 ##################_____GET AUXILIARY DATA_____##################
 class Test_GetAuxData(unittest.TestCase):
 
     # GET PARAMETERS EMPTY
     def test_getAuxData_empty(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         auxData = circuit.getAuxData()
 
         self.assertIsInstance(auxData, list)
         self.assertEqual(auxData, [])
 
     # GET AUXILIARY DATA
     def test_getAuxData(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         circuit.addAuxData(circuit.AuxData('AuxData', 1))
 
         auxData = circuit.getAuxData()
         removeUiID(auxData) # remove random uiID to validate behaviour
 
         self.assertIsInstance(auxData, list)
@@ -114,25 +124,25 @@
 
 
 ##################_____GET CLASSES_____##################
 class Test_GetClasses(unittest.TestCase):
 
     # GET CLASSES EMPTY
     def test_getClasses_empty(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         classes = circuit.getClasses()
 
         self.assertIsInstance(classes, list)
         self.assertEqual(classes, [])
 
     # GET CLASSES
     def test_getClasses(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         circuit.addClass(circuit.Class('Class', 1))
 
         classes = circuit.getClasses()
         removeUiID(classes) # remove random uiID to validate behaviour
 
         self.assertIsInstance(classes, list)
@@ -141,25 +151,25 @@
 
 
 ##################_____GET VARIABLES_____##################
 class Test_GetVariables(unittest.TestCase):
 
     # GET VARIABLES EMPTY
     def test_getVariables_empty(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         variables = circuit.getVariables()
 
         self.assertIsInstance(variables, list)
         self.assertEqual(variables, [])
 
     # GET VARIABLES
     def test_getVariables(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         cls = circuit.Class('Class', 1)
         circuit.addVariable(circuit.Variable('Variable', cls))
 
         variables = circuit.getVariables()
         removeUiID(variables) # remove random uiID to validate behaviour # remove random uiID to validate behaviour
 
@@ -168,25 +178,25 @@
 
 
 ##################_____GET RULES_____##################
 class Test_GetRules(unittest.TestCase):
 
     # GET RULES EMPTY
     def test_getRules_empty(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         rules = circuit.getRules()
 
         self.assertIsInstance(rules, list)
         self.assertEqual(rules, [])
 
     # GET RULES
     def test_getRules(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         rule = circuit.Rule('Rule', 1)
         circuit.addRule(rule)
 
         rules = circuit.getRules()
         removeUiID(rules) # remove random uiID to validate behaviour
 
@@ -196,69 +206,239 @@
 
 
 ##################_____PARAMETER_____##################
 class Test_Parameter(unittest.TestCase):
 
     # PARAMETER value INT
     def test_Parameter_value_int(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         parameter = circuit.Parameter('Parameter', 1)
 
         self.assertIsInstance(parameter, circuit.Parameter)
         self.assertEqual(parameter.getName(), 'Parameter')
         self.assertEqual(parameter.getValue(), '1')
 
     # PARAMETER value FLOAT
     def test_Parameter_value_float(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         parameter = circuit.Parameter('Parameter', 1.5)
 
         self.assertIsInstance(parameter, circuit.Parameter)
         self.assertEqual(parameter.getName(), 'Parameter')
         self.assertEqual(parameter.getValue(), '1.5')
 
     # PARAMETER value STRING EXPRESSION
     def test_Parameter_value_string_expression(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         parameter = circuit.Parameter('Parameter', 'pi/2')
 
         self.assertIsInstance(parameter, circuit.Parameter)
         self.assertEqual(parameter.getName(), 'Parameter')
         self.assertEqual(parameter.getValue(), 'pi/2')
 
+    # MAGIC METHOD ADD value INT
+    def test_Parameter_magicMethod_add_int(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        parameter = circuit.Parameter('Parameter', 1)
+
+        p = parameter + 1
+
+        self.assertEqual(p, 'Parameter + 1')
+
+    # MAGIC METHOD ADD value FLOAT
+    def test_Parameter_magicMethod_add_float(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        parameter = circuit.Parameter('Parameter', 1)
+
+        p = parameter + 1.5
+
+        self.assertEqual(p, 'Parameter + 1.5')
+
+    # MAGIC METHOD ADD value STRING
+    def test_Parameter_magicMethod_add_string(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        parameter = circuit.Parameter('Parameter', 1)
+
+        p = parameter + 'pi/2'
+
+        self.assertEqual(p, 'Parameter + pi/2')
+
+    # MAGIC METHOD ADD value PARAMETER
+    def test_Parameter_magicMethod_add_Parameter(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        parameter = circuit.Parameter('Parameter', 1)
+
+        p = parameter + parameter
+
+        self.assertEqual(p, 'Parameter + Parameter')
+
+    # MAGIC METHOD SUB value INT
+    def test_Parameter_magicMethod_sub_int(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        parameter = circuit.Parameter('Parameter', 1)
+
+        p = parameter - 1
+
+        self.assertEqual(p, 'Parameter - 1')
+
+    # MAGIC METHOD SUB value FLOAT
+    def test_Parameter_magicMethod_sub_float(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        parameter = circuit.Parameter('Parameter', 1)
+
+        p = parameter - 1.5
+
+        self.assertEqual(p, 'Parameter - 1.5')
+
+    # MAGIC METHOD SUB value STRING
+    def test_Parameter_magicMethod_sub_string(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        parameter = circuit.Parameter('Parameter', 1)
+
+        p = parameter - 'pi/2'
+
+        self.assertEqual(p, 'Parameter - pi/2')
+
+    # MAGIC METHOD SUB value PARAMETER
+    def test_Parameter_magicMethod_sub_Parameter(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        parameter = circuit.Parameter('Parameter', 1)
+
+        p = parameter - parameter
+
+        self.assertEqual(p, 'Parameter - Parameter')
+
+    # MAGIC METHOD MUL value INT
+    def test_Parameter_magicMethod_mul_int(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        parameter = circuit.Parameter('Parameter', 1)
+
+        p = parameter * 1
+
+        self.assertEqual(p, 'Parameter * 1')
+
+    # MAGIC METHOD MUL value FLOAT
+    def test_Parameter_magicMethod_mul_float(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        parameter = circuit.Parameter('Parameter', 1)
+
+        p = parameter * 1.5
+
+        self.assertEqual(p, 'Parameter * 1.5')
+
+    # MAGIC METHOD MUL value STRING
+    def test_Parameter_magicMethod_mul_string(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        parameter = circuit.Parameter('Parameter', 1)
+
+        p = parameter * 'pi/2'
+
+        self.assertEqual(p, 'Parameter * pi/2')
+
+    # MAGIC METHOD MUL value PARAMETER
+    def test_Parameter_magicMethod_mul_Parameter(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        parameter = circuit.Parameter('Parameter', 1)
+
+        p = parameter * parameter
+
+        self.assertEqual(p, 'Parameter * Parameter')
+
+    # MAGIC METHOD DIV value INT
+    def test_Parameter_magicMethod_div_int(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        parameter = circuit.Parameter('Parameter', 1)
+
+        p = parameter / 1
+
+        self.assertEqual(p, 'Parameter / 1')
+
+    # MAGIC METHOD DIV value FLOAT
+    def test_Parameter_magicMethod_div_float(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        parameter = circuit.Parameter('Parameter', 1)
+
+        p = parameter / 1.5
+
+        self.assertEqual(p, 'Parameter / 1.5')
+
+    # MAGIC METHOD DIV value STRING
+    def test_Parameter_magicMethod_div_string(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        parameter = circuit.Parameter('Parameter', 1)
+
+        p = parameter / 'pi'
+
+        self.assertEqual(p, 'Parameter / pi')
+
+    # MAGIC METHOD DIV value PARAMETER
+    def test_Parameter_magicMethod_div_Parameter(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        parameter = circuit.Parameter('Parameter', 1)
+
+        p = parameter / parameter
+
+        self.assertEqual(p, 'Parameter / Parameter')
+
+    # MAGIC METHOD NEG
+    def test_Parameter_magicMethod_add_int(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        parameter = circuit.Parameter('Parameter', 1)
+
+        p = -parameter
+
+        self.assertEqual(p, '-Parameter')
+
     # BAD ARGUMENT value
     def test_Parameter_badArgument_value(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.Parameter('Parameter', 'value')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE name
     def test_Parameter_badArgumentType_name(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.Parameter(1, 99)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE value
     def test_Parameter_badArgumentType_value(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.Parameter('Parameter', True)
             raise Exception
 
         except Exception as e:
@@ -266,84 +446,119 @@
 
 
 ##################_____AUXDATA_____##################
 class Test_AuxData(unittest.TestCase):
 
     # AUXDATA value INT
     def test_AuxData_value_int(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         auxData = circuit.AuxData('AuxData', 1)
 
         self.assertIsInstance(auxData, circuit.AuxData)
         self.assertEqual(auxData.getName(), 'AuxData')
         self.assertEqual(auxData.getValue(), '1')
 
     # AUXDATA value FLOAT
     def test_AuxData_value_float(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         auxData = circuit.AuxData('AuxData', 1.5)
 
         self.assertIsInstance(auxData, circuit.AuxData)
         self.assertEqual(auxData.getName(), 'AuxData')
         self.assertEqual(auxData.getValue(), '1.5')
 
     # AUXDATA value LIST INT, FLOAT
     def test_AuxData_value_list_int_float(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         auxData = circuit.AuxData('AuxData', [1, 1.5])
 
         self.assertIsInstance(auxData, circuit.AuxData)
         self.assertEqual(auxData.getName(), 'AuxData')
         self.assertEqual(auxData.getValue(), '[1, 1.5]')
 
+    # AUXDATA value LIST LIST
+    def test_AuxData_value_list_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+
+        auxData = circuit.AuxData('AuxData', [[1, 1.5], [1, 1.5]])
+
+        self.assertIsInstance(auxData, circuit.AuxData)
+        self.assertEqual(auxData.getName(), 'AuxData')
+        self.assertEqual(auxData.getValue(), '[[1, 1.5], [1, 1.5]]')
+
     # BAD ARGUMENT value LIST
     def test_AuxData_badArgument_value_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.AuxData('AuxData', [])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
+    # BAD ARGUMENT value LIST LIST
+    def test_AuxData_badArgument_value_list_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+
+        try:
+            circuit.AuxData('AuxData', [[]])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
+    # BAD ARGUMENT value LIST INT, LIST
+    def test_AuxData_badArgument_value_list_int_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+
+        try:
+            circuit.AuxData('AuxData', [1, []])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT TYPE name
     def test_AuxData_badArgumentType_name(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.AuxData(99, 1)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE value STRING
     def test_AuxData_badArgumentType_value_string(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.AuxData('AuxData', 'value')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE value LIST
     def test_AuxData_badArgumentType_value_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.AuxData('AuxData', [1, 'value'])
             raise Exception
 
         except Exception as e:
@@ -351,79 +566,79 @@
 
 
 ##################_____CLASS_____##################
 class Test_Class(unittest.TestCase):
 
     # CLASS numberOfVars INT
     def test_Class_numberOfVars_int(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         cls = circuit.Class('Class', 2)
 
         self.assertIsInstance(cls, circuit.Class)
         self.assertEqual(cls.getName(), 'Class')
         self.assertEqual(cls.getNumberOfVars(), '2')
         self.assertEqual(cls.getDescription(), '')
         self.assertEqual(cls.getProperties(), [])
 
     # CLASS numberOfVars PARAMETER
     def test_Class_numberOfVars_Parameter(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         parameter = circuit.Parameter('Parameter', 2)
 
         cls = circuit.Class('Class', parameter)
 
         self.assertIsInstance(cls, circuit.Class)
         self.assertEqual(cls.getName(), 'Class')
-        self.assertEqual(cls.getNumberOfVars(), '2')
+        self.assertEqual(cls.getNumberOfVars(), 'Parameter')
         self.assertEqual(cls.getDescription(), '')
         self.assertEqual(cls.getProperties(), [])
 
     # CLASS description
     def test_Class_description(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         cls = circuit.Class('Class', 2, description='description')
 
         self.assertIsInstance(cls, circuit.Class)
         self.assertEqual(cls.getName(), 'Class')
         self.assertEqual(cls.getNumberOfVars(), '2')
         self.assertEqual(cls.getDescription(), 'description')
         self.assertEqual(cls.getProperties(), [])
 
     # BAD ARGUMENT TYPE name
     def test_Class_badArgumentType_name(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.Class(99, 2)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE numberOfVars
     def test_Class_badArgumentType_numberOfVars(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.Class('Class', 'numberOfVars')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE description
     def test_Class_badArgumentType_description(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.Class('Class', 2, 99)
             raise Exception
 
         except Exception as e:
@@ -431,84 +646,84 @@
 
 
 ##################_____CLASS ADD PROPERTY_____##################
 class Test_Class_AddProperty(unittest.TestCase):
 
     # ADD PROPERTY CLASS numberOfVars INT
     def test_Class_addProperty_Class_numberOfVars_int(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         cls = circuit.Class('Class', 2)
         cls.addProperty('Property', [1, 2])
         circuit.addClass(cls)
         
         properties = circuit.getClasses()[0]['Properties']
         removeUiID(properties) # remove random uiID to validate behaviour
 
         self.assertIsInstance(properties, list)
         self.assertEqual(properties, [{'Name': 'Property', 'Values': ['1', '2']}])
 
     # ADD PROPERTY CLASS numberOfVars PARAMETER
     def test_Class_addProperty_Class_numberOfVars_Parameter(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         cls = circuit.Class('Class', circuit.Parameter('Parameter', 2))
         cls.addProperty('Property', [1, 2])
         circuit.addClass(cls)
         
         properties = circuit.getClasses()[0]['Properties']
         removeUiID(properties) # remove random uiID to validate behaviour
 
         self.assertIsInstance(properties, list)
         self.assertEqual(properties, [{'Name': 'Property', 'Values': ['1', '2']}])
 
     # BAD ARGUMENT value
     def test_Class_addProperty_badArgument_value(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         cls = circuit.Class('Class', 2)
 
         try:
             cls.addProperty('Property', [1, 2, 3])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE name
     def test_Class_addProperty_badArgumentType_name(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         cls = circuit.Class('Class', 2)
 
         try:
             cls.addProperty(99, [1, 2])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE value STRING
     def test_Class_addProperty_badArgumentType_value_string(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         cls = circuit.Class('Class', 2)
 
         try:
             cls.addProperty('Property', 'value')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
         
     # BAD ARGUMENT TYPE value LIST
     def test_Class_addProperty_badArgumentType_value_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         cls = circuit.Class('Class', 2)
 
         try:
             cls.addProperty('Property', [1, 'value'])
             raise Exception
 
@@ -517,107 +732,107 @@
 
 
 ##################_____VARIABLE_____##################
 class Test_Variable(unittest.TestCase):
 
     # VARIABLE classes CLASS
     def test_Variable_classes_Class(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         cls = circuit.Class('Class', 1)
 
         variable = circuit.Variable('Variable', cls)
         
         self.assertIsInstance(variable, circuit.Variable)
         self.assertEqual(variable.getName(), 'Variable')
         self.assertEqual(variable.getClasses(), [cls.getUiID()])
         self.assertEqual(variable.getDescription(), '')
 
     # VARIABLE classes LIST
     def test_Variable_classes_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         cls1 = circuit.Class('Class', 1)
         cls2 = circuit.Class('Class2', 2)
 
         variable = circuit.Variable('Variable', [cls1, cls2])
         
         self.assertIsInstance(variable, circuit.Variable)
         self.assertEqual(variable.getName(), 'Variable')
         self.assertEqual(variable.getClasses(), [cls1.getUiID(), cls2.getUiID()])
         self.assertEqual(variable.getDescription(), '')
 
     # VARIABLE description
     def test_Variable_description(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         cls = circuit.Class('Class', 1)
 
         variable = circuit.Variable('Variable', cls, description='description')
         
         self.assertIsInstance(variable, circuit.Variable)
         self.assertEqual(variable.getName(), 'Variable')
         self.assertEqual(variable.getClasses(), [cls.getUiID()])
         self.assertEqual(variable.getDescription(), 'description')
 
     # BAD ARGUMENT classes LIST
     def test_Variable_badArgument_classes_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.Variable('Variable', [])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE name
     def test_Variable_badArgumentType_name(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         cls = circuit.Class('Class', 1)
 
         try:
             circuit.Variable(99, cls)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE classes STRING
     def test_Variable_badArgumentType_classes_string(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.Variable('Variable', 'classes')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE classes LIST
     def test_Variable_badArgumentType_classes_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         cls = circuit.Class('Class', 1)
 
         try:
             circuit.Variable('Variable', [cls, 'cls'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE description
     def test_Variable_badArgumentType_description(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         cls = circuit.Class('Class', 1)
 
         try:
             circuit.Variable('Variable', cls, 1)
             raise Exception
 
@@ -626,133 +841,133 @@
 
 
 ##################_____RULE_____##################
 class Test_Rule(unittest.TestCase):
 
     # RULE lambdaValue INT
     def test_Rule_lambdaValue_int(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         rule = circuit.Rule('Rule', 1)
         
         self.assertIsInstance(rule, circuit.Rule)
         self.assertEqual(rule.getName(), 'Rule')
         self.assertEqual(rule.getLambda(), '1')
         self.assertEqual(rule.getDescription(), '')
         self.assertEqual(rule.getDisabled(), 'False')
         self.assertEqual(rule.getExpressions(), [])
 
     # RULE lambdaValue FLOAT
     def test_Rule_lambdaValue_float(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         rule = circuit.Rule('Rule', 1.5)
         
         self.assertIsInstance(rule, circuit.Rule)
         self.assertEqual(rule.getName(), 'Rule')
         self.assertEqual(rule.getLambda(), '1.5')
         self.assertEqual(rule.getDescription(), '')
         self.assertEqual(rule.getDisabled(), 'False')
         self.assertEqual(rule.getExpressions(), [])
 
     # RULE lambdaValue STRING
     def test_Rule_lambdaValue_string(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         rule = circuit.Rule('Rule', 'pi/2')
         
         self.assertIsInstance(rule, circuit.Rule)
         self.assertEqual(rule.getName(), 'Rule')
         self.assertEqual(rule.getLambda(), 'pi/2')
         self.assertEqual(rule.getDescription(), '')
         self.assertEqual(rule.getDisabled(), 'False')
         self.assertEqual(rule.getExpressions(), [])
 
     # RULE description
     def test_Rule_description(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         rule = circuit.Rule('Rule', 1, description='description')
         
         self.assertIsInstance(rule, circuit.Rule)
         self.assertEqual(rule.getName(), 'Rule')
         self.assertEqual(rule.getLambda(), '1')
         self.assertEqual(rule.getDescription(), 'description')
         self.assertEqual(rule.getDisabled(), 'False')
         self.assertEqual(rule.getExpressions(), [])
 
     # RULE disabled
     def test_Rule_disabled(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         rule = circuit.Rule('Rule', 1, disabled=True)
         
         self.assertIsInstance(rule, circuit.Rule)
         self.assertEqual(rule.getName(), 'Rule')
         self.assertEqual(rule.getLambda(), '1')
         self.assertEqual(rule.getDescription(), '')
         self.assertEqual(rule.getDisabled(), 'True')
         self.assertEqual(rule.getExpressions(), [])
 
     # BAD ARGUMENT lambdaValue STRING
     def test_Rule_badArgument_lambdaValue_string(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.Rule('Rule', 'lambdaValue')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE name
     def test_Rule_badArgumentType_name(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.Rule(1, 1)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE lambdaValue
     def test_Rule_badArgumentType_lambdaValue(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.Rule('Rule', True)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE description
     def test_Rule_badArgumentType_description(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.Rule('Rule', 1, description=99)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE disabled
     def test_Rule_badArgumentType_disabled(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.Rule('Rule', 1, disabled='disabled')
             raise Exception
 
         except Exception as e:
@@ -760,15 +975,15 @@
 
 
 ##################_____OFFSETEXP_____##################
 class Test_OffsetExp(unittest.TestCase):
 
     # OFFSET EXPRESSION offset INT
     def test_OffsetExp_offset_int(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         offsetExp = circuit.OffsetExp(1)
         
         self.assertIsInstance(offsetExp, circuit.OffsetExp)
         self.assertEqual(offsetExp.getExpType(), 'OFFSET')
         self.assertEqual(offsetExp.getCoefficient(), '')
@@ -778,15 +993,15 @@
         self.assertEqual(offsetExp.getIterator(), '')
         self.assertEqual(offsetExp.getTerm1(), {})
         self.assertEqual(offsetExp.getTerm2(), {})
         self.assertEqual(offsetExp.getChilds(), [])
 
     # OFFSET EXPRESSION offset FLOAT
     def test_OffsetExp_offset_float(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         offsetExp = circuit.OffsetExp(1.5)
         
         self.assertIsInstance(offsetExp, circuit.OffsetExp)
         self.assertEqual(offsetExp.getExpType(), 'OFFSET')
         self.assertEqual(offsetExp.getCoefficient(), '')
@@ -796,15 +1011,15 @@
         self.assertEqual(offsetExp.getIterator(), '')
         self.assertEqual(offsetExp.getTerm1(), {})
         self.assertEqual(offsetExp.getTerm2(), {})
         self.assertEqual(offsetExp.getChilds(), [])
 
     # OFFSET EXPRESSION offset STRING
     def test_OffsetExp_offset_string(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         offsetExp = circuit.OffsetExp('offset')
         
         self.assertIsInstance(offsetExp, circuit.OffsetExp)
         self.assertEqual(offsetExp.getExpType(), 'OFFSET')
         self.assertEqual(offsetExp.getCoefficient(), '')
@@ -812,17 +1027,36 @@
         self.assertEqual(offsetExp.getFrom(), '')
         self.assertEqual(offsetExp.getTo(), '')
         self.assertEqual(offsetExp.getIterator(), '')
         self.assertEqual(offsetExp.getTerm1(), {})
         self.assertEqual(offsetExp.getTerm2(), {})
         self.assertEqual(offsetExp.getChilds(), [])
 
+    # OFFSET EXPRESSION offset PARAMETER
+    def test_OffsetExp_offset_Parameter(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        parameter = circuit.Parameter('Parameter', 1)
+
+        offsetExp = circuit.OffsetExp(parameter)
+        
+        self.assertIsInstance(offsetExp, circuit.OffsetExp)
+        self.assertEqual(offsetExp.getExpType(), 'OFFSET')
+        self.assertEqual(offsetExp.getCoefficient(), '')
+        self.assertEqual(offsetExp.getOffset(), 'Parameter')
+        self.assertEqual(offsetExp.getFrom(), '')
+        self.assertEqual(offsetExp.getTo(), '')
+        self.assertEqual(offsetExp.getIterator(), '')
+        self.assertEqual(offsetExp.getTerm1(), {})
+        self.assertEqual(offsetExp.getTerm2(), {})
+        self.assertEqual(offsetExp.getChilds(), [])
+
     # BAD ARGUMENT TYPE offset
     def test_OffsetExp_badArgumentType_offset(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.OffsetExp(True)
             raise Exception
 
         except Exception as e:
@@ -830,15 +1064,15 @@
 
 
 ##################_____LINEAREXP_____##################
 class Test_LinearExp(unittest.TestCase):
 
     # LINEAR EXPRESSION variable[1] INT
     def test_LinearExp_variable1_int(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable = circuit.Variable('Variable', cls:=circuit.Class('Class', 1))
         
         linearExp = circuit.LinearExp((variable, 1))
         
         self.assertIsInstance(linearExp, circuit.LinearExp)
         self.assertEqual(linearExp.getExpType(), 'LINEAR')
@@ -851,15 +1085,15 @@
         removeUiID(term1) # remove random uiID to validate behaviour
         self.assertEqual(term1, {'Indexes': [{'Value': '1', 'ClassID': cls.getUiID()}], 'VariableID': variable.getUiID()})
         self.assertEqual(linearExp.getTerm2(), {})
         self.assertEqual(linearExp.getChilds(), [])
 
     # LINEAR EXPRESSION variable[1] FLOAT
     def test_LinearExp_variable1_float(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable = circuit.Variable('Variable', cls:=circuit.Class('Class', 1))
         
         linearExp = circuit.LinearExp((variable, 1.5))
         
         self.assertIsInstance(linearExp, circuit.LinearExp)
         self.assertEqual(linearExp.getExpType(), 'LINEAR')
@@ -872,15 +1106,15 @@
         removeUiID(term1) # remove random uiID to validate behaviour
         self.assertEqual(term1, {'Indexes': [{'Value': '1.5', 'ClassID': cls.getUiID()}], 'VariableID': variable.getUiID()})
         self.assertEqual(linearExp.getTerm2(), {})
         self.assertEqual(linearExp.getChilds(), [])
 
     # LINEAR EXPRESSION variable[1] STRING
     def test_LinearExp_variable1_string(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable = circuit.Variable('Variable', cls:=circuit.Class('Class', 1))
 
         linearExp = circuit.LinearExp((variable, 'value'))
         
         self.assertIsInstance(linearExp, circuit.LinearExp)
         self.assertEqual(linearExp.getExpType(), 'LINEAR')
@@ -891,40 +1125,65 @@
         self.assertEqual(linearExp.getIterator(), '')
         term1 = linearExp.getTerm1()
         removeUiID(term1) # remove random uiID to validate behaviour
         self.assertEqual(term1, {'Indexes': [{'Value': 'value', 'ClassID': cls.getUiID()}], 'VariableID': variable.getUiID()})
         self.assertEqual(linearExp.getTerm2(), {})
         self.assertEqual(linearExp.getChilds(), [])
 
-    # LINEAR EXPRESSION variable[1] LIST INT, FLOAT, STRING
-    def test_LinearExp_variable1_list_int_float_string(self):
-        qsoa = QSOAPlatform()
+    # LINEAR EXPRESSION variable[1] PARAMETER
+    def test_LinearExp_variable1_Parameter(self):
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
-        variable = circuit.Variable('Variable', cls:=[circuit.Class('Class', 1), circuit.Class('Class', 1), circuit.Class('Class', 1)])
+        variable = circuit.Variable('Variable', cls:=circuit.Class('Class', 1))
+        parameter = circuit.Parameter('Parameter', 1)
 
-        linearExp = circuit.LinearExp((variable, [1, 1.5, 'value']))
+        linearExp = circuit.LinearExp((variable, parameter))
+        
+        self.assertIsInstance(linearExp, circuit.LinearExp)
+        self.assertEqual(linearExp.getExpType(), 'LINEAR')
+        self.assertEqual(linearExp.getCoefficient(), '')
+        self.assertEqual(linearExp.getOffset(), '')
+        self.assertEqual(linearExp.getFrom(), '')
+        self.assertEqual(linearExp.getTo(), '')
+        self.assertEqual(linearExp.getIterator(), '')
+        term1 = linearExp.getTerm1()
+        removeUiID(term1) # remove random uiID to validate behaviour
+        self.assertEqual(term1, {'Indexes': [{'Value': 'Parameter', 'ClassID': cls.getUiID()}], 'VariableID': variable.getUiID()})
+        self.assertEqual(linearExp.getTerm2(), {})
+        self.assertEqual(linearExp.getChilds(), [])
+
+    # LINEAR EXPRESSION variable[1] LIST INT, FLOAT, STRING, PARAMETER
+    def test_LinearExp_variable1_list_int_float_string_Parameter(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        variable = circuit.Variable('Variable', cls:=[circuit.Class('Class', 1), circuit.Class('Class', 1), circuit.Class('Class', 1), circuit.Class('Class', 1)])
+        parameter = circuit.Parameter('Parameter', 1)
+
+        linearExp = circuit.LinearExp((variable, [1, 1.5, 'value', parameter]))
         
         self.assertIsInstance(linearExp, circuit.LinearExp)
         self.assertEqual(linearExp.getExpType(), 'LINEAR')
         self.assertEqual(linearExp.getCoefficient(), '')
         self.assertEqual(linearExp.getOffset(), '')
         self.assertEqual(linearExp.getFrom(), '')
         self.assertEqual(linearExp.getTo(), '')
         self.assertEqual(linearExp.getIterator(), '')
         term1 = linearExp.getTerm1()
         removeUiID(term1) # remove random uiID to validate behaviour
         self.assertEqual(term1, {'Indexes': [{'Value': '1', 'ClassID': cls[0].getUiID()},
                                              {'Value': '1.5', 'ClassID': cls[1].getUiID()},
-                                             {'Value': 'value', 'ClassID': cls[2].getUiID()}], 'VariableID': variable.getUiID()})
+                                             {'Value': 'value', 'ClassID': cls[2].getUiID()},
+                                             {'Value': 'Parameter', 'ClassID': cls[3].getUiID()}
+                                            ],'VariableID': variable.getUiID()})
         self.assertEqual(linearExp.getTerm2(), {})
         self.assertEqual(linearExp.getChilds(), [])
 
     # LINEAR EXPRESSION coefficient INT
     def test_LinearExp_coefficient_int(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable = circuit.Variable('Variable', cls:=circuit.Class('Class', 1))
 
         linearExp = circuit.LinearExp((variable, 1), coefficient=2)
         
         self.assertIsInstance(linearExp, circuit.LinearExp)
         self.assertEqual(linearExp.getExpType(), 'LINEAR')
@@ -937,15 +1196,15 @@
         removeUiID(term1) # remove random uiID to validate behaviour
         self.assertEqual(term1, {'Indexes': [{'Value': '1', 'ClassID': cls.getUiID()}], 'VariableID': variable.getUiID()})
         self.assertEqual(linearExp.getTerm2(), {})
         self.assertEqual(linearExp.getChilds(), [])
 
     # LINEAR EXPRESSION coefficient FLOAT
     def test_LinearExp_coefficient_float(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable = circuit.Variable('Variable', cls:=circuit.Class('Class', 1))
 
         linearExp = circuit.LinearExp((variable, 1), coefficient=1.5)
         
         self.assertIsInstance(linearExp, circuit.LinearExp)
         self.assertEqual(linearExp.getExpType(), 'LINEAR')
@@ -958,15 +1217,15 @@
         removeUiID(term1) # remove random uiID to validate behaviour
         self.assertEqual(term1, {'Indexes': [{'Value': '1', 'ClassID': cls.getUiID()}], 'VariableID': variable.getUiID()})
         self.assertEqual(linearExp.getTerm2(), {})
         self.assertEqual(linearExp.getChilds(), [])
 
     # LINEAR EXPRESSION coefficient STRING
     def test_LinearExp_coefficient_string(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable = circuit.Variable('Variable', cls:=circuit.Class('Class', 1))
 
         linearExp = circuit.LinearExp((variable, 1), coefficient='coefficient')
         
         self.assertIsInstance(linearExp, circuit.LinearExp)
         self.assertEqual(linearExp.getExpType(), 'LINEAR')
@@ -977,92 +1236,114 @@
         self.assertEqual(linearExp.getIterator(), '')
         term1 = linearExp.getTerm1()
         removeUiID(term1) # remove random uiID to validate behaviour
         self.assertEqual(term1, {'Indexes': [{'Value': '1', 'ClassID': cls.getUiID()}], 'VariableID': variable.getUiID()})
         self.assertEqual(linearExp.getTerm2(), {})
         self.assertEqual(linearExp.getChilds(), [])
 
+    # LINEAR EXPRESSION coefficient PARAMETER
+    def test_LinearExp_coefficient_Parameter(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        variable = circuit.Variable('Variable', cls:=circuit.Class('Class', 1))
+        parameter = circuit.Parameter('Parameter', 1)
+
+        linearExp = circuit.LinearExp((variable, 1), coefficient=parameter)
+        
+        self.assertIsInstance(linearExp, circuit.LinearExp)
+        self.assertEqual(linearExp.getExpType(), 'LINEAR')
+        self.assertEqual(linearExp.getCoefficient(), 'Parameter')
+        self.assertEqual(linearExp.getOffset(), '')
+        self.assertEqual(linearExp.getFrom(), '')
+        self.assertEqual(linearExp.getTo(), '')
+        self.assertEqual(linearExp.getIterator(), '')
+        term1 = linearExp.getTerm1()
+        removeUiID(term1) # remove random uiID to validate behaviour
+        self.assertEqual(term1, {'Indexes': [{'Value': '1', 'ClassID': cls.getUiID()}], 'VariableID': variable.getUiID()})
+        self.assertEqual(linearExp.getTerm2(), {})
+        self.assertEqual(linearExp.getChilds(), [])
+
     # BAD ARGUMENT variable
     def test_LinearExp_badArgument_variable(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.LinearExp(())
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT variable[1] LIST
     def test_LinearExp_badArgument_variable1_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable = circuit.Variable('Variable', circuit.Class('Class', 1))
 
         try:
             circuit.LinearExp((variable, []))
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE variable
     def test_LinearExp_badArgumentType_variable(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.LinearExp('variable')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE variable[0]
     def test_LinearExp_badArgumentType_variable0(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.LinearExp(('variable', 1))
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE variable[1] BOOL
     def test_LinearExp_badArgumentType_variable1_bool(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable = circuit.Variable('Variable', circuit.Class('Class', 1))
 
         try:
             circuit.LinearExp((variable, True))
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE variable[1] LIST
     def test_LinearExp_badArgumentType_variable1_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable = circuit.Variable('Variable', circuit.Class('Class', 1))
 
         try:
             circuit.LinearExp((variable, [1, True]))
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE coefficient
     def test_LinearExp_badArgumentType_coefficient(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable = circuit.Variable('Variable', circuit.Class('Class', 1))
 
         try:
             circuit.LinearExp((variable, 1), coefficient=True)
             raise Exception
 
@@ -1071,15 +1352,15 @@
 
 
 ##################_____QUADRATICEXP_____##################
 class Test_QuadraticExp(unittest.TestCase):
 
     # QUADRATIC EXPRESSION variable1[1] INT
     def test_QuadraticExp_variable11_int(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable1', cls1:=circuit.Class('Class1', 1))
         variable2 = circuit.Variable('Variable2', cls2:=circuit.Class('Class2', 1))
 
         quadraticExp = circuit.QuadraticExp((variable1, 1), (variable2, 2))
         
         self.assertIsInstance(quadraticExp, circuit.QuadraticExp)
@@ -1095,15 +1376,15 @@
         term2 = quadraticExp.getTerm2()
         removeUiID(term2) # remove random uiID to validate behaviour
         self.assertEqual(term2, {'Indexes': [{'Value': '2', 'ClassID': cls2.getUiID()}], 'VariableID': variable2.getUiID()})
         self.assertEqual(quadraticExp.getChilds(), [])
 
     # QUADRATIC EXPRESSION variable1[1] FLOAT
     def test_QuadraticExp_variable11_float(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable1', cls1:=circuit.Class('Class1', 1))
         variable2 = circuit.Variable('Variable2', cls2:=circuit.Class('Class2', 1))
 
         quadraticExp = circuit.QuadraticExp((variable1, 1.5), (variable2, 2))
         
         self.assertIsInstance(quadraticExp, circuit.QuadraticExp)
@@ -1119,15 +1400,15 @@
         term2 = quadraticExp.getTerm2()
         removeUiID(term2) # remove random uiID to validate behaviour
         self.assertEqual(term2, {'Indexes': [{'Value': '2', 'ClassID': cls2.getUiID()}], 'VariableID': variable2.getUiID()})
         self.assertEqual(quadraticExp.getChilds(), [])
 
     # QUADRATIC EXPRESSION variable1[1] STRING
     def test_QuadraticExp_variable11_string(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable1', cls1:=circuit.Class('Class1', 1))
         variable2 = circuit.Variable('Variable2', cls2:=circuit.Class('Class2', 1))
 
         quadraticExp = circuit.QuadraticExp((variable1, 'value'), (variable2, 2))
         
         self.assertIsInstance(quadraticExp, circuit.QuadraticExp)
@@ -1141,43 +1422,71 @@
         removeUiID(term1) # remove random uiID to validate behaviour
         self.assertEqual(term1, {'Indexes': [{'Value': 'value', 'ClassID': cls1.getUiID()}], 'VariableID': variable1.getUiID()})
         term2 = quadraticExp.getTerm2()
         removeUiID(term2) # remove random uiID to validate behaviour
         self.assertEqual(term2, {'Indexes': [{'Value': '2', 'ClassID': cls2.getUiID()}], 'VariableID': variable2.getUiID()})
         self.assertEqual(quadraticExp.getChilds(), [])
 
-    # QUADRATIC EXPRESSION variable1[1] LIST INT, FLOAT, STRING
-    def test_QuadraticExp_variable11_list_int_float_string(self):
-        qsoa = QSOAPlatform()
+    # QUADRATIC EXPRESSION variable1[1] PARAMETER
+    def test_QuadraticExp_variable11_Parameter(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        variable1 = circuit.Variable('Variable1', cls1:=circuit.Class('Class1', 1))
+        variable2 = circuit.Variable('Variable2', cls2:=circuit.Class('Class2', 1))
+        parameter = circuit.Parameter('Parameter', 1)
+
+        quadraticExp = circuit.QuadraticExp((variable1, parameter), (variable2, 2))
+        
+        self.assertIsInstance(quadraticExp, circuit.QuadraticExp)
+        self.assertEqual(quadraticExp.getExpType(), 'QUADRATIC')
+        self.assertEqual(quadraticExp.getCoefficient(), '')
+        self.assertEqual(quadraticExp.getOffset(), '')
+        self.assertEqual(quadraticExp.getFrom(), '')
+        self.assertEqual(quadraticExp.getTo(), '')
+        self.assertEqual(quadraticExp.getIterator(), '')
+        term1 = quadraticExp.getTerm1()
+        removeUiID(term1) # remove random uiID to validate behaviour
+        self.assertEqual(term1, {'Indexes': [{'Value': 'Parameter', 'ClassID': cls1.getUiID()}], 'VariableID': variable1.getUiID()})
+        term2 = quadraticExp.getTerm2()
+        removeUiID(term2) # remove random uiID to validate behaviour
+        self.assertEqual(term2, {'Indexes': [{'Value': '2', 'ClassID': cls2.getUiID()}], 'VariableID': variable2.getUiID()})
+        self.assertEqual(quadraticExp.getChilds(), [])
+
+    # QUADRATIC EXPRESSION variable1[1] LIST INT, FLOAT, STRING, PARAMETER
+    def test_QuadraticExp_variable11_list_int_float_string_Parameter(self):
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
-        variable1 = circuit.Variable('Variable1', cls1:=[circuit.Class('Class1', 1), circuit.Class('Class2', 1), circuit.Class('Class3', 1)])
+        variable1 = circuit.Variable('Variable1', cls1:=[circuit.Class('Class1', 1), circuit.Class('Class2', 1), circuit.Class('Class3', 1), circuit.Class('Class4', 1)])
         variable2 = circuit.Variable('Variable2', cls2:=circuit.Class('Class3', 1))
+        parameter = circuit.Parameter('Parameter', 1)
 
-        quadraticExp = circuit.QuadraticExp((variable1, [1, 1.5, 'value']), (variable2, 2))
+        quadraticExp = circuit.QuadraticExp((variable1, [1, 1.5, 'value', parameter]), (variable2, 2))
         
         self.assertIsInstance(quadraticExp, circuit.QuadraticExp)
         self.assertEqual(quadraticExp.getExpType(), 'QUADRATIC')
         self.assertEqual(quadraticExp.getCoefficient(), '')
         self.assertEqual(quadraticExp.getOffset(), '')
         self.assertEqual(quadraticExp.getFrom(), '')
         self.assertEqual(quadraticExp.getTo(), '')
         self.assertEqual(quadraticExp.getIterator(), '')
         term1 = quadraticExp.getTerm1()
         removeUiID(term1) # remove random uiID to validate behaviour
         self.assertEqual(term1, {'Indexes': [{'Value': '1', 'ClassID': cls1[0].getUiID()},
                                              {'Value': '1.5', 'ClassID': cls1[1].getUiID()},
-                                             {'Value': 'value', 'ClassID': cls1[2].getUiID()}], 'VariableID': variable1.getUiID()})
+                                             {'Value': 'value', 'ClassID': cls1[2].getUiID()},
+                                             {'Value': 'Parameter', 'ClassID': cls1[3].getUiID()}
+                                            ], 'VariableID': variable1.getUiID()})
         term2 = quadraticExp.getTerm2()
         removeUiID(term2) # remove random uiID to validate behaviour
         self.assertEqual(term2, {'Indexes': [{'Value': '2', 'ClassID': cls2.getUiID()}], 'VariableID': variable2.getUiID()})
         self.assertEqual(quadraticExp.getChilds(), [])
 
     # QUADRATIC EXPRESSION variable2[1] INT
     def test_QuadraticExp_variable21_int(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable1', cls1:=circuit.Class('Class1', 1))
         variable2 = circuit.Variable('Variable2', cls2:=circuit.Class('Class2', 1))
 
         quadraticExp = circuit.QuadraticExp((variable1, 1), (variable2, 2))
         
         self.assertIsInstance(quadraticExp, circuit.QuadraticExp)
@@ -1193,15 +1502,15 @@
         term2 = quadraticExp.getTerm2()
         removeUiID(term2) # remove random uiID to validate behaviour
         self.assertEqual(term2, {'Indexes': [{'Value': '2', 'ClassID': cls2.getUiID()}], 'VariableID': variable2.getUiID()})
         self.assertEqual(quadraticExp.getChilds(), [])
 
     # QUADRATIC EXPRESSION variable2[1] FLOAT
     def test_QuadraticExp_variable21_float(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable1', cls1:=circuit.Class('Class1', 1))
         variable2 = circuit.Variable('Variable2', cls2:=circuit.Class('Class2', 1))
 
         quadraticExp = circuit.QuadraticExp((variable1, 1), (variable2, 1.5))
         
         self.assertIsInstance(quadraticExp, circuit.QuadraticExp)
@@ -1217,15 +1526,15 @@
         term2 = quadraticExp.getTerm2()
         removeUiID(term2) # remove random uiID to validate behaviour
         self.assertEqual(term2, {'Indexes': [{'Value': '1.5', 'ClassID': cls2.getUiID()}], 'VariableID': variable2.getUiID()})
         self.assertEqual(quadraticExp.getChilds(), [])
 
     # QUADRATIC EXPRESSION variable2[1] STRING
     def test_QuadraticExp_variable21_string(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable1', cls1:=circuit.Class('Class1', 1))
         variable2 = circuit.Variable('Variable2', cls2:=circuit.Class('Class2', 1))
 
         quadraticExp = circuit.QuadraticExp((variable1, 1), (variable2, 'value'))
         
         self.assertIsInstance(quadraticExp, circuit.QuadraticExp)
@@ -1241,15 +1550,15 @@
         term2 = quadraticExp.getTerm2()
         removeUiID(term2) # remove random uiID to validate behaviour
         self.assertEqual(term2, {'Indexes': [{'Value': 'value', 'ClassID': cls2.getUiID()}], 'VariableID': variable2.getUiID()})
         self.assertEqual(quadraticExp.getChilds(), [])
 
     # QUADRATIC EXPRESSION variable2[1] LIST INT, FLOAT, STRING
     def test_QuadraticExp_variable21_list_int_float_string(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable1', cls1:=circuit.Class('Class1', 1))
         variable2 = circuit.Variable('Variable2', cls2:=[circuit.Class('Class2', 1), circuit.Class('Class3', 1), circuit.Class('Class4', 1)])
 
         quadraticExp = circuit.QuadraticExp((variable1, 1), (variable2, [1, 1.5, 'value']))
         
         self.assertIsInstance(quadraticExp, circuit.QuadraticExp)
@@ -1267,15 +1576,15 @@
         self.assertEqual(term2, {'Indexes': [{'Value': '1', 'ClassID': cls2[0].getUiID()},
                                              {'Value': '1.5', 'ClassID': cls2[1].getUiID()},
                                              {'Value': 'value', 'ClassID': cls2[2].getUiID()}], 'VariableID': variable2.getUiID()})
         self.assertEqual(quadraticExp.getChilds(), [])
 
     # QUADRATIC EXPRESSION coefficient INT
     def test_QuadraticExp_coefficient_int(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable1', cls1:=circuit.Class('Class1', 1))
         variable2 = circuit.Variable('Variable2', cls2:=circuit.Class('Class2', 1))
 
         quadraticExp = circuit.QuadraticExp((variable1, 1), (variable2, 2), coefficient=1)
         
         self.assertIsInstance(quadraticExp, circuit.QuadraticExp)
@@ -1291,15 +1600,15 @@
         term2 = quadraticExp.getTerm2()
         removeUiID(term2) # remove random uiID to validate behaviour
         self.assertEqual(term2, {'Indexes': [{'Value': '2', 'ClassID': cls2.getUiID()}], 'VariableID': variable2.getUiID()})
         self.assertEqual(quadraticExp.getChilds(), [])
 
     # QUADRATIC EXPRESSION coefficient FLOAT
     def test_QuadraticExp_coefficient_float(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable1', cls1:=circuit.Class('Class1', 1))
         variable2 = circuit.Variable('Variable2', cls2:=circuit.Class('Class2', 1))
 
         quadraticExp = circuit.QuadraticExp((variable1, 1), (variable2, 2), coefficient=1.5)
         
         self.assertIsInstance(quadraticExp, circuit.QuadraticExp)
@@ -1315,15 +1624,15 @@
         term2 = quadraticExp.getTerm2()
         removeUiID(term2) # remove random uiID to validate behaviour
         self.assertEqual(term2, {'Indexes': [{'Value': '2', 'ClassID': cls2.getUiID()}], 'VariableID': variable2.getUiID()})
         self.assertEqual(quadraticExp.getChilds(), [])
 
     # QUADRATIC EXPRESSION coefficient STRING
     def test_QuadraticExp_coefficient_string(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable1', cls1:=circuit.Class('Class1', 1))
         variable2 = circuit.Variable('Variable2', cls2:=circuit.Class('Class2', 1))
 
         quadraticExp = circuit.QuadraticExp((variable1, 1), (variable2, 2), coefficient='coefficient')
         
         self.assertIsInstance(quadraticExp, circuit.QuadraticExp)
@@ -1337,179 +1646,204 @@
         removeUiID(term1) # remove random uiID to validate behaviour
         self.assertEqual(term1, {'Indexes': [{'Value': '1', 'ClassID': cls1.getUiID()}], 'VariableID': variable1.getUiID()})
         term2 = quadraticExp.getTerm2()
         removeUiID(term2) # remove random uiID to validate behaviour
         self.assertEqual(term2, {'Indexes': [{'Value': '2', 'ClassID': cls2.getUiID()}], 'VariableID': variable2.getUiID()})
         self.assertEqual(quadraticExp.getChilds(), [])
 
+    # QUADRATIC EXPRESSION coefficient PARAMETER
+    def test_QuadraticExp_coefficient_Parameter(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        variable1 = circuit.Variable('Variable1', cls1:=circuit.Class('Class1', 1))
+        variable2 = circuit.Variable('Variable2', cls2:=circuit.Class('Class2', 1))
+        parameter = circuit.Parameter('Parameter', 1)
+
+        quadraticExp = circuit.QuadraticExp((variable1, 1), (variable2, 2), coefficient=parameter)
+        
+        self.assertIsInstance(quadraticExp, circuit.QuadraticExp)
+        self.assertEqual(quadraticExp.getExpType(), 'QUADRATIC')
+        self.assertEqual(quadraticExp.getCoefficient(), 'Parameter')
+        self.assertEqual(quadraticExp.getOffset(), '')
+        self.assertEqual(quadraticExp.getFrom(), '')
+        self.assertEqual(quadraticExp.getTo(), '')
+        self.assertEqual(quadraticExp.getIterator(), '')
+        term1 = quadraticExp.getTerm1()
+        removeUiID(term1) # remove random uiID to validate behaviour
+        self.assertEqual(term1, {'Indexes': [{'Value': '1', 'ClassID': cls1.getUiID()}], 'VariableID': variable1.getUiID()})
+        term2 = quadraticExp.getTerm2()
+        removeUiID(term2) # remove random uiID to validate behaviour
+        self.assertEqual(term2, {'Indexes': [{'Value': '2', 'ClassID': cls2.getUiID()}], 'VariableID': variable2.getUiID()})
+        self.assertEqual(quadraticExp.getChilds(), [])
+
     # BAD ARGUMENT variable1
     def test_QuadraticExp_badArgument_variable1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable2 = circuit.Variable('Variable2', circuit.Class('Class', 1))
 
         try:
             circuit.QuadraticExp((), (variable2, 2))
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT variable1[1] LIST
     def test_QuadraticExp_badArgument_variable11_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable1', circuit.Class('Class', 1))
         variable2 = circuit.Variable('Variable2', circuit.Class('Class', 1))
 
         try:
             circuit.QuadraticExp((variable1, []), (variable2, 1))
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT variable2
     def test_QuadraticExp_badArgument_variable2(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable1', circuit.Class('Class', 1))
 
         try:
             circuit.QuadraticExp((variable1, 1), ())
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT variable2[1] LIST
     def test_QuadraticExp_badArgument_variable21_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable1', circuit.Class('Class', 1))
         variable2 = circuit.Variable('Variable2', circuit.Class('Class', 1))
 
         try:
             circuit.QuadraticExp((variable1, 1), (variable2, []))
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE variable1
     def test_QuadraticExp_badArgumentType_variable1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable2 = circuit.Variable('Variable2', circuit.Class('Class', 1))
 
         try:
             circuit.QuadraticExp('variable1', (variable2, 1))
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE variable1[0]
     def test_QuadraticExp_badArgumentType_variable10(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable2 = circuit.Variable('Variable2', circuit.Class('Class', 1))
 
         try:
             circuit.QuadraticExp(('variable1', 1), (variable2, 1))
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE variable1[1] BOOL
     def test_QuadraticExp_badArgumentType_variable11_bool(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable', circuit.Class('Class', 1))
         variable2 = circuit.Variable('Variable2', circuit.Class('Class', 1))
 
         try:
             circuit.QuadraticExp((variable1, True), (variable2, 1))
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
         
     # BAD ARGUMENT TYPE variable1[1] LIST
     def test_QuadraticExp_badArgumentType_variable11_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable', circuit.Class('Class', 1))
         variable2 = circuit.Variable('Variable2', circuit.Class('Class', 1))
 
         try:
             circuit.QuadraticExp((variable1, [1, True]), (variable2, 1))
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE variable2
     def test_QuadraticExp_badArgumentType_variable2(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable1', circuit.Class('Class', 1))
 
         try:
             circuit.QuadraticExp((variable1, 1), 'variable2')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE variable2[0]
     def test_QuadraticExp_badArgumentType_variable20(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable1', circuit.Class('Class', 1))
 
         try:
             circuit.QuadraticExp((variable1, 1), ('variable2', 1))
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE variable2[1] BOOL
     def test_QuadraticExp_badArgumentType_variable21_bool(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable1', circuit.Class('Class', 1))
         variable2 = circuit.Variable('Variable2', circuit.Class('Class', 1))
 
         try:
             circuit.QuadraticExp((variable1, 1), (variable2, True))
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE variable2[1] LIST
     def test_QuadraticExp_badArgumentType_variable21_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable1', circuit.Class('Class', 1))
         variable2 = circuit.Variable('Variable2', circuit.Class('Class', 1))
 
         try:
             circuit.QuadraticExp((variable1, 1), (variable2, [1, True]))
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE coefficient
     def test_QuadraticExp_badArgumentType_coefficient(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         variable1 = circuit.Variable('Variable1', circuit.Class('Class', 1))
         variable2 = circuit.Variable('Variable2', circuit.Class('Class', 1))
 
         try:
             circuit.QuadraticExp((variable1, 1), (variable2, 1), coefficient=True)
             raise Exception
@@ -1519,15 +1853,15 @@
 
 
 ##################_____SQUAREDEXP_____##################
 class Test_SquaredExp(unittest.TestCase):
 
     # SQUARED EXPRESSION expression OFFSETEXP
     def test_SquaredExp_expression_OffsetExp(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
         squaredExp = circuit.SquaredExp(offsetExp)
         
         self.assertIsInstance(squaredExp, circuit.SquaredExp)
         self.assertEqual(squaredExp.getExpType(), 'SQUARED')
@@ -1549,15 +1883,15 @@
             'Term1': offsetExp.getTerm1(),
             'Term2': offsetExp.getTerm2(),
             'Childs': offsetExp.getChilds()
         }])
 
     # SQUARED EXPRESSION expression LINEAREXP
     def test_SquaredExp_expression_LinearExp(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         linearExp = circuit.LinearExp((circuit.Variable('Variable', circuit.Class('Class', 1)), 1))
 
         squaredExp = circuit.SquaredExp(linearExp)
         
         self.assertIsInstance(squaredExp, circuit.SquaredExp)
         self.assertEqual(squaredExp.getExpType(), 'SQUARED')
@@ -1579,15 +1913,15 @@
             'Term1': linearExp.getTerm1(),
             'Term2': linearExp.getTerm2(),
             'Childs': linearExp.getChilds()
         }])
 
     # SQUARED EXPRESSION expression SUMMATIONEXP
     def test_SquaredExp_expression_SummationExp(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         summation = circuit.SummationExp(1, 2, circuit.OffsetExp(1))
 
         squaredExp = circuit.SquaredExp(summation)
         
         self.assertIsInstance(squaredExp, circuit.SquaredExp)
         self.assertEqual(squaredExp.getExpType(), 'SQUARED')
@@ -1609,15 +1943,15 @@
             'Term1': summation.getTerm1(),
             'Term2': summation.getTerm2(),
             'Childs': summation.getChilds()
         }])
 
     # SQUARED EXPRESSION expression LIST OFFSETEXP, LINEAREXP, SUMMATIONEXP
     def test_SquaredExp_expression_list_OffsetExp_LinearExp_SummationExp(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
         linearExp = circuit.LinearExp((circuit.Variable('Variable', circuit.Class('Class', 1)), 1))
         summation = circuit.SummationExp(1, 2, offsetExp)
 
         squaredExp = circuit.SquaredExp([offsetExp, linearExp, summation])
         
@@ -1665,39 +1999,39 @@
             'Term1': summation.getTerm1(),
             'Term2': summation.getTerm2(),
             'Childs': summation.getChilds()
         }])
 
     # BAD ARGUMENT expression LIST
     def test_SquaredExp_badArgument_expression_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.SquaredExp([])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE expression STRING
     def test_SquaredExp_badArgumentType_expression_string(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.SquaredExp('expression')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE expression LIST
     def test_SquaredExp_badArgumentType_expression_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
         try:
             circuit.SquaredExp([offsetExp, 'expression'])
             raise Exception
 
@@ -1706,15 +2040,15 @@
 
 
 ##################_____SUMMATIONEXP_____##################
 class Test_SummationExp(unittest.TestCase):
 
     # SUMMATION EXPRESSION fromValue INT
     def test_SummationExp_fromValue_int(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
         summation = circuit.SummationExp(1, 2, offsetExp)
         
         self.assertIsInstance(summation, circuit.SummationExp)
         self.assertEqual(summation.getExpType(), 'SUMMATORY')
@@ -1736,15 +2070,15 @@
             'Term1': offsetExp.getTerm1(),
             'Term2': offsetExp.getTerm2(),
             'Childs': offsetExp.getChilds()
         }])
 
     # SUMMATION EXPRESSION fromValue FLOAT
     def test_SummationExp_fromValue_float(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
         summation = circuit.SummationExp(1.5, 2, offsetExp)
         
         self.assertIsInstance(summation, circuit.SummationExp)
         self.assertEqual(summation.getExpType(), 'SUMMATORY')
@@ -1766,15 +2100,15 @@
             'Term1': offsetExp.getTerm1(),
             'Term2': offsetExp.getTerm2(),
             'Childs': offsetExp.getChilds()
         }])
 
     # SUMMATION EXPRESSION fromValue STRING
     def test_SummationExp_fromValue_string(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
         summation = circuit.SummationExp('fromValue', 2, offsetExp)
         
         self.assertIsInstance(summation, circuit.SummationExp)
         self.assertEqual(summation.getExpType(), 'SUMMATORY')
@@ -1794,17 +2128,48 @@
             'To': offsetExp.getTo(),
             'Iterator': offsetExp.getIterator(),
             'Term1': offsetExp.getTerm1(),
             'Term2': offsetExp.getTerm2(),
             'Childs': offsetExp.getChilds()
         }])
 
+    # SUMMATION EXPRESSION fromValue PARAMETER
+    def test_SummationExp_fromValue_Parameter(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        offsetExp = circuit.OffsetExp(1)
+        parameter = circuit.Parameter('Parameter', 1)
+
+        summation = circuit.SummationExp(parameter, 2, offsetExp)
+        
+        self.assertIsInstance(summation, circuit.SummationExp)
+        self.assertEqual(summation.getExpType(), 'SUMMATORY')
+        self.assertEqual(summation.getCoefficient(), '')
+        self.assertEqual(summation.getOffset(), '')
+        self.assertEqual(summation.getFrom(), 'Parameter')
+        self.assertEqual(summation.getTo(), '2')
+        self.assertEqual(summation.getIterator(), 'i')
+        self.assertEqual(summation.getTerm1(), {})
+        self.assertEqual(summation.getTerm2(), {})
+        self.assertEqual(summation.getChilds(), [{
+            'uiID': offsetExp.getUiID(),
+            'Type': offsetExp.getExpType(),
+            'Coefficient': offsetExp.getCoefficient(),
+            'Offset': offsetExp.getOffset(),
+            'From': offsetExp.getFrom(),
+            'To': offsetExp.getTo(),
+            'Iterator': offsetExp.getIterator(),
+            'Term1': offsetExp.getTerm1(),
+            'Term2': offsetExp.getTerm2(),
+            'Childs': offsetExp.getChilds()
+        }])
+
     # SUMMATION EXPRESSION toValue INT
     def test_SummationExp_toValue_int(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
         summation = circuit.SummationExp(1, 2, offsetExp)
         
         self.assertIsInstance(summation, circuit.SummationExp)
         self.assertEqual(summation.getExpType(), 'SUMMATORY')
@@ -1826,15 +2191,15 @@
             'Term1': offsetExp.getTerm1(),
             'Term2': offsetExp.getTerm2(),
             'Childs': offsetExp.getChilds()
         }])
 
     # SUMMATION EXPRESSION toValue FLOAT
     def test_SummationExp_toValue_float(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
         summation = circuit.SummationExp(1, 2.5, offsetExp)
         
         self.assertIsInstance(summation, circuit.SummationExp)
         self.assertEqual(summation.getExpType(), 'SUMMATORY')
@@ -1856,15 +2221,15 @@
             'Term1': offsetExp.getTerm1(),
             'Term2': offsetExp.getTerm2(),
             'Childs': offsetExp.getChilds()
         }])
 
     # SUMMATION EXPRESSION toValue STRING
     def test_SummationExp_toValue_string(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
         summation = circuit.SummationExp(1, 'toValue', offsetExp)
         
         self.assertIsInstance(summation, circuit.SummationExp)
         self.assertEqual(summation.getExpType(), 'SUMMATORY')
@@ -1884,17 +2249,48 @@
             'To': offsetExp.getTo(),
             'Iterator': offsetExp.getIterator(),
             'Term1': offsetExp.getTerm1(),
             'Term2': offsetExp.getTerm2(),
             'Childs': offsetExp.getChilds()
         }])
 
+    # SUMMATION EXPRESSION toValue PARAMETER
+    def test_SummationExp_toValue_Parameter(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitAnnealing()
+        offsetExp = circuit.OffsetExp(1)
+        parameter = circuit.Parameter('Parameter', 1)
+
+        summation = circuit.SummationExp(1, parameter, offsetExp)
+        
+        self.assertIsInstance(summation, circuit.SummationExp)
+        self.assertEqual(summation.getExpType(), 'SUMMATORY')
+        self.assertEqual(summation.getCoefficient(), '')
+        self.assertEqual(summation.getOffset(), '')
+        self.assertEqual(summation.getFrom(), '1')
+        self.assertEqual(summation.getTo(), 'Parameter')
+        self.assertEqual(summation.getIterator(), 'i')
+        self.assertEqual(summation.getTerm1(), {})
+        self.assertEqual(summation.getTerm2(), {})
+        self.assertEqual(summation.getChilds(), [{
+            'uiID': offsetExp.getUiID(),
+            'Type': offsetExp.getExpType(),
+            'Coefficient': offsetExp.getCoefficient(),
+            'Offset': offsetExp.getOffset(),
+            'From': offsetExp.getFrom(),
+            'To': offsetExp.getTo(),
+            'Iterator': offsetExp.getIterator(),
+            'Term1': offsetExp.getTerm1(),
+            'Term2': offsetExp.getTerm2(),
+            'Childs': offsetExp.getChilds()
+        }])
+
     # SUMMATION EXPRESSION expression OFFSETEXP
     def test_SummationExp_expression_OffsetExp(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
         summation = circuit.SummationExp(1, 2, offsetExp)
         
         self.assertIsInstance(summation, circuit.SummationExp)
         self.assertEqual(summation.getExpType(), 'SUMMATORY')
@@ -1916,15 +2312,15 @@
             'Term1': offsetExp.getTerm1(),
             'Term2': offsetExp.getTerm2(),
             'Childs': offsetExp.getChilds()
         }])
 
     # SUMMATION EXPRESSION expression LINEAREXP
     def test_SummationExp_expression_LinearExp(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         linearExp = circuit.LinearExp((circuit.Variable('Variable', circuit.Class('Class', 1)), 1))
 
         summation = circuit.SummationExp(1, 2, linearExp)
         
         self.assertIsInstance(summation, circuit.SummationExp)
         self.assertEqual(summation.getExpType(), 'SUMMATORY')
@@ -1946,15 +2342,15 @@
             'Term1': linearExp.getTerm1(),
             'Term2': linearExp.getTerm2(),
             'Childs': linearExp.getChilds()
         }])
 
     # SUMMATION EXPRESSION expression QUADRATICEXP
     def test_SummationExp_expression_QuadraticExp(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         quadraticExp = circuit.QuadraticExp((variable:=circuit.Variable('Variable', circuit.Class('Class', 1)), 1), (variable, 2))
 
         summation = circuit.SummationExp(1, 2, quadraticExp)
         
         self.assertIsInstance(summation, circuit.SummationExp)
         self.assertEqual(summation.getExpType(), 'SUMMATORY')
@@ -1976,15 +2372,15 @@
             'Term1': quadraticExp.getTerm1(),
             'Term2': quadraticExp.getTerm2(),
             'Childs': quadraticExp.getChilds()
         }])
 
     # SUMMATION EXPRESSION expression SQUAREDEXP
     def test_SummationExp_expression_SquaredExp(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         squaredExp = circuit.SquaredExp(circuit.OffsetExp(1))
 
         summation = circuit.SummationExp(1, 2, squaredExp)
         
         self.assertIsInstance(summation, circuit.SummationExp)
         self.assertEqual(summation.getExpType(), 'SUMMATORY')
@@ -2006,15 +2402,15 @@
             'Term1': squaredExp.getTerm1(),
             'Term2': squaredExp.getTerm2(),
             'Childs': squaredExp.getChilds()
         }])
 
     # SUMMATION EXPRESSION expression SUMMATIONEXP
     def test_SummationExp_expression_SummationExp(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         summation1 = circuit.SummationExp(1, 2, circuit.OffsetExp(1))
 
         summation = circuit.SummationExp(1, 2, summation1)
         
         self.assertIsInstance(summation, circuit.SummationExp)
         self.assertEqual(summation.getExpType(), 'SUMMATORY')
@@ -2036,15 +2432,15 @@
             'Term1': summation1.getTerm1(),
             'Term2': summation1.getTerm2(),
             'Childs': summation1.getChilds()
         }])
 
     # SUMMATION EXPRESSION expression LIST OFFSETEXP, LINEAREXP, QUADRATICEXP, SQUAREDEXP, SUMMATIONEXP
     def test_SummationExp_expression_list_OffsetExp_LinearExp_QuadraticExp_SquaredExp_SummationExp(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
         linearExp = circuit.LinearExp((variable:=circuit.Variable('Variable', circuit.Class('Class', 1)), 1))
         quadraticExp = circuit.QuadraticExp((variable, 1), (variable, 2))
         squaredExp = circuit.SquaredExp(offsetExp)
         summation1 = circuit.SummationExp(1, 2, offsetExp)
 
@@ -2118,15 +2514,15 @@
             'Term1': summation1.getTerm1(),
             'Term2': summation1.getTerm2(),
             'Childs': summation1.getChilds()
         }])
 
     # SUMMATION EXPRESSION iterator
     def test_SummationExp_iterator(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
         summation = circuit.SummationExp(1, 2, offsetExp, iterator='x')
         
         self.assertIsInstance(summation, circuit.SummationExp)
         self.assertEqual(summation.getExpType(), 'SUMMATORY')
@@ -2148,78 +2544,78 @@
             'Term1': offsetExp.getTerm1(),
             'Term2': offsetExp.getTerm2(),
             'Childs': offsetExp.getChilds()
         }])
 
     # BAD ARGUMENT expression LIST
     def test_SummationExp_badArgument_expression_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.SummationExp(1, 2, [])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE fromValue
     def test_SummationExp_badArgumentType_fromValue(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
         try:
             circuit.SummationExp(True, 2, offsetExp)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE toValue
     def test_SummationExp_badArgumentType_toValue(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
         try:
             circuit.SummationExp(1, True, offsetExp)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE expression STRING
     def test_SummationExp_badArgumentType_expression_string(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.SummationExp(1, 2, 'expression')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE expression LIST
     def test_SummationExp_badArgumentType_expression_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
         try:
             circuit.SummationExp(1, 2, [offsetExp, 1])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE iterator
     def test_SummationExp_badArgumentType_iterator(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
         try:
             circuit.SummationExp(1, 2, offsetExp, iterator=99)
             raise Exception
 
@@ -2228,73 +2624,73 @@
 
 
 ##################_____ADD PARAMETER_____##################
 class Test_AddParameter(unittest.TestCase):
 
     # ADD PARAMETER parameter PARAMETER
     def test_addParameter_parameter_Parameter(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         parameter = circuit.Parameter('Parameter', 1)
 
         parameterAdded = circuit.addParameter(parameter)
 
         circuitParameters = circuit.getParameters()
         removeUiID(circuitParameters) # remove random uiID to validate behaviour
 
-        self.assertIsInstance(parameterAdded, qsoa.CircuitAnnealing.Parameter)
+        self.assertEqual(type(parameterAdded).__name__, 'Parameter')
         self.assertIsInstance(circuitParameters, list)
         self.assertEqual(circuitParameters, [{'Name': 'Parameter', 'Value': '1'}])
 
     # ADD PARAMETER parameter LIST
     def test_addParameter_parameter_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         parameter1 = circuit.Parameter('Parameter1', 1)
         parameter2 = circuit.Parameter('Parameter2', 2)
 
         circuit = qsoa.CircuitAnnealing()
 
         parameterAdded = circuit.addParameter([parameter1, parameter2])
 
         circuitParameters = circuit.getParameters()
         removeUiID(circuitParameters) # remove random uiID to validate behaviour
 
         self.assertIsInstance(parameterAdded, list)
-        for p in parameterAdded: self.assertIsInstance(p, qsoa.CircuitAnnealing.Parameter)
+        for p in parameterAdded: self.assertEqual(type(p).__name__, 'Parameter')
         self.assertIsInstance(circuitParameters, list)
         self.assertEqual(circuitParameters, [{'Name': 'Parameter1', 'Value': '1'}, {'Name': 'Parameter2', 'Value': '2'}])
 
     # BAD ARGUMENT parameter LIST
     def test_addParameter_badArgument_parameter_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.addParameter([])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE parameter STRING
     def test_addParameter_badArgumentType_parameter_string(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.addParameter('parameter')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
         
     # BAD ARGUMENT TYPE parameter LIST
     def test_addParameter_badArgumentType_parameter_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         parameter = circuit.Parameter('Parameter', 1)
 
         try:
             circuit.addParameter([parameter, 'parameter'])
             raise Exception
 
@@ -2302,71 +2698,71 @@
             self.assertIsInstance(e, TypeError)
 
 ##################_____ADD AUXILIARY DATA_____##################
 class Test_AddAuxData(unittest.TestCase):
 
     # ADD AUXDATA
     def test_addAuxData(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         auxData = circuit.AuxData('AuxData', 1)
 
         auxDataAdded = circuit.addAuxData(auxData)
 
         circuitAuxData = circuit.getAuxData()
         removeUiID(circuitAuxData) # remove random uiID to validate behaviour
 
-        self.assertIsInstance(auxDataAdded, qsoa.CircuitAnnealing.AuxData)
+        self.assertEqual(type(auxDataAdded).__name__, 'AuxData')
         self.assertIsInstance(circuitAuxData, list)
         self.assertEqual(circuitAuxData, [{'Name': 'AuxData', 'Value': '1'}])
 
     # ADD AUXDATA LIST
     def test_addAuxData_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         auxData1 = circuit.AuxData('AuxData1', 1)
         auxData2 = circuit.AuxData('AuxData2', 2)
 
         auxDataAdded = circuit.addAuxData([auxData1, auxData2])
 
         circuitAuxData = circuit.getAuxData()
         removeUiID(circuitAuxData) # remove random uiID to validate behaviour
 
         self.assertIsInstance(auxDataAdded, list)
-        for a in auxDataAdded: self.assertIsInstance(a, qsoa.CircuitAnnealing.AuxData)
+        for a in auxDataAdded: self.assertEqual(type(a).__name__, 'AuxData')
         self.assertIsInstance(circuitAuxData, list)
         self.assertEqual(circuitAuxData, [{'Name': 'AuxData1', 'Value': '1'}, {'Name': 'AuxData2', 'Value': '2'}])
 
     # BAD ARGUMENT auxData LIST
     def test_addAuxData_badArgument_auxData_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.addAuxData([])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE auxData
     def test_addAuxData_badArgumentType_auxData(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.addAuxData('auxData')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE parameter LIST
     def test_addAuxData_badArgumentType_parameter_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         auxData = circuit.AuxData('AuxData', 1)
 
         try:
             circuit.addAuxData([auxData, 'auxData'])
             raise Exception
 
@@ -2375,72 +2771,72 @@
 
 
 ##################_____ADD CLASS_____##################
 class Test_AddClass(unittest.TestCase):
 
     # ADD CLASS
     def test_addClass(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         cls = circuit.Class('Class', 2)
 
         clsAdded = circuit.addClass(cls)
 
         circuitClasses = circuit.getClasses()
         removeUiID(circuitClasses) # remove random uiID to validate behaviour
 
-        self.assertIsInstance(clsAdded, qsoa.CircuitAnnealing.Class)
+        self.assertEqual(type(clsAdded).__name__, 'Class')
         self.assertIsInstance(circuitClasses, list)
         self.assertEqual(circuitClasses, [{'Description': '', 'Name': 'Class', 'NumberOfVars': '2', 'Properties': []}])
 
     # ADD CLASS LIST
     def test_addClass_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         cls1 = circuit.Class('Class1', 1)
         cls2 = circuit.Class('Class2', 2)
 
         clsAdded = circuit.addClass([cls1, cls2])
 
         circuitClasses = circuit.getClasses()
         removeUiID(circuitClasses) # remove random uiID to validate behaviour
 
         self.assertIsInstance(clsAdded, list)
-        for c in clsAdded: self.assertIsInstance(c, qsoa.CircuitAnnealing.Class)
+        for c in clsAdded: self.assertEqual(type(c).__name__, 'Class')
         self.assertIsInstance(circuitClasses, list)
         self.assertEqual(circuitClasses, [{'Description': '', 'Name': 'Class1', 'NumberOfVars': '1', 'Properties': []},
                                           {'Description': '', 'Name': 'Class2', 'NumberOfVars': '2', 'Properties': []}])
 
     # BAD ARGUMENT cls LIST
     def test_addClass_badArgument_cls_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.addClass([])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE cls
     def test_addClass_badArgumentType_cls(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.addClass('cls')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE cls LIST
     def test_addClass_badArgumentType_cls_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         cls = circuit.Class('Class', 2)
 
         try:
             circuit.addAuxData([cls, 'cls'])
             raise Exception
 
@@ -2449,74 +2845,74 @@
 
 
 ##################_____ADD VARIABLE_____##################
 class Test_AddVariable(unittest.TestCase):
 
     # ADD VARIABLE
     def test_addVariable(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         cls = circuit.Class('Class', 1)
         variable = circuit.Variable('Variable', [cls])
 
         variableAdded = circuit.addVariable(variable)
 
         circuitVariables = circuit.getVariables()
         removeUiID(circuitVariables) # remove random uiID to validate behaviour
 
-        self.assertIsInstance(variableAdded, qsoa.CircuitAnnealing.Variable)
+        self.assertEqual(type(variableAdded).__name__, 'Variable')
         self.assertIsInstance(circuitVariables, list)
         self.assertEqual(circuitVariables, [{'Classes': [cls.getUiID()], 'Description': '', 'Name': 'Variable'}])
 
     # ADD VARIABLE LIST
     def test_addVariable_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         cls = circuit.Class('Class', 1)
         variable1 = circuit.Variable('Variable1', cls)
         variable2 = circuit.Variable('Variable2', cls)
 
         variableAdded = circuit.addVariable([variable1, variable2])
 
         circuitVariables = circuit.getVariables()
         removeUiID(circuitVariables) # remove random uiID to validate behaviour
 
         self.assertIsInstance(variableAdded, list)
-        for v in variableAdded: self.assertIsInstance(v, qsoa.CircuitAnnealing.Variable)
+        for v in variableAdded: self.assertEqual(type(v).__name__, 'Variable')
         self.assertIsInstance(circuitVariables, list)
         self.assertEqual(circuitVariables, [{'Classes': [cls.getUiID()], 'Description': '', 'Name': 'Variable1'},
                                             {'Classes': [cls.getUiID()], 'Description': '', 'Name': 'Variable2'}])
 
     # BAD ARGUMENT variable LIST
     def test_addVariable_badArgument_variable_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.addVariable([])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE variable
     def test_addVariable_badArgumentType_variable(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.addVariable('variable')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE variable LIST
     def test_addVariable_badArgumentType_variable_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         cls = circuit.Class('Class', 1)
         variable = circuit.Variable('Variable', cls)
 
         try:
             circuit.addVariable([variable, 'variable'])
             raise Exception
@@ -2526,187 +2922,187 @@
 
 
 ##################_____ADD RULE_____##################
 class Test_AddRule(unittest.TestCase):
 
     # ADD RULE
     def test_addRule(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         rule = circuit.Rule('Rule', 1)
 
         ruleAdded = circuit.addRule(rule)
 
         rules = circuit.getRules()
         removeUiID(rules) # remove random uiID to validate behaviour
 
-        self.assertIsInstance(ruleAdded, qsoa.CircuitAnnealing.Rule)
+        self.assertEqual(type(ruleAdded).__name__, 'Rule')
         self.assertIsInstance(rules, list)
         self.assertEqual(rules, [{'Expressions': [], 'Name': 'Rule', 'Lambda': '1', 'Description': '', 'Disabled': 'False'}])
 
     # ADD RULE LIST
     def test_addRule_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         rule1 = circuit.Rule('Rule1', 1)
         rule2 = circuit.Rule('Rule2', 2)
 
         ruleAdded = circuit.addRule([rule1, rule2])
 
         rules = circuit.getRules()
         removeUiID(rules) # remove random uiID to validate behaviour
 
         self.assertIsInstance(ruleAdded, list)
-        for r in ruleAdded: self.assertIsInstance(r, qsoa.CircuitAnnealing.Rule)
+        for r in ruleAdded: self.assertEqual(type(r).__name__, 'Rule')
         self.assertIsInstance(rules, list)
         self.assertEqual(rules, [{'Expressions': [], 'Name': 'Rule1', 'Lambda': '1', 'Description': '', 'Disabled': 'False'},
                                  {'Expressions': [], 'Name': 'Rule2', 'Lambda': '2', 'Description': '', 'Disabled': 'False'}])
 
     # BAD ARGUMENT rule LIST
     def test_addRule_badArgument_rule_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.addRule([])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE rule
     def test_addRule_badArgumentType_rule(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
 
         try:
             circuit.addRule('rule')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE rule LIST
     def test_addVariable_badArgumentType_rule_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         rule = circuit.Rule('Rule', 1)
 
         try:
             circuit.addVariable([rule, 'rule'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
 
-##################_____ADD EXPRESSION_____##################
-class Test_AddExpression(unittest.TestCase):
+##################_____RULE ADD EXPRESSION_____##################
+class Test_Rule_AddExpression(unittest.TestCase):
 
     # ADD EXPRESSION expression OFFSETEXP
-    def test_addExpression_expression_OffsetExp(self):
-        qsoa = QSOAPlatform()
+    def test_Rule_addExpression_expression_OffsetExp(self):
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         rule = circuit.Rule('Rule', 1)
         offsetExp = circuit.OffsetExp(1)
 
         ruleAdded = rule.addExpression(offsetExp)
 
         expressions = rule.getExpressions()
         removeUiID(expressions) # remove random uiID to validate behaviour
 
-        self.assertIsInstance(ruleAdded, qsoa.CircuitAnnealing.Rule)
+        self.assertEqual(type(ruleAdded).__name__, 'Rule')
         self.assertIsInstance(expressions, list)
         self.assertEqual(expressions, [{'Type': 'OFFSET', 'Coefficient': '', 'Offset': '1', 'From': '', 'To': '', 'Iterator': '', 'Term1': {}, 'Term2': {}, 'Childs': []}])
 
     # ADD EXPRESSION expression LINEAREXP
-    def test_addExpression_expression_LinearExp(self):
-        qsoa = QSOAPlatform()
+    def test_Rule_addExpression_expression_LinearExp(self):
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         rule = circuit.Rule('Rule', 1)
         linearExp = circuit.LinearExp((variable:=circuit.Variable('Variable', cls:=circuit.Class('Class', 1)), 1))
 
         ruleAdded = rule.addExpression(linearExp)
 
         expressions = rule.getExpressions()
 
-        self.assertIsInstance(ruleAdded, qsoa.CircuitAnnealing.Rule)
+        self.assertEqual(type(ruleAdded).__name__, 'Rule')
         self.assertIsInstance(expressions, list)
         removeUiID(expressions) # remove random uiID to validate behaviour
         self.assertEqual(expressions, [{'Type': 'LINEAR', 'Coefficient': '', 'Offset': '', 'From': '', 'To': '', 'Iterator': '',
                                         'Term1': {'Indexes': [{'Value': '1', 'ClassID': cls.getUiID()}], 'VariableID': variable.getUiID()},
                                         'Term2': {}, 'Childs': []}])
 
     # ADD EXPRESSION expression QUADRATICEXP
-    def test_addExpression_expression_QuadraticExp(self):
-        qsoa = QSOAPlatform()
+    def test_Rule_addExpression_expression_QuadraticExp(self):
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         rule = circuit.Rule('Rule', 1)
         quadraticExp = circuit.QuadraticExp((variable:=circuit.Variable('Variable1', cls:=circuit.Class('Class1', 1)), 1), (variable, 2))
 
         ruleAdded = rule.addExpression(quadraticExp)
 
         expressions = rule.getExpressions()
 
-        self.assertIsInstance(ruleAdded, qsoa.CircuitAnnealing.Rule)
+        self.assertEqual(type(ruleAdded).__name__, 'Rule')
         self.assertIsInstance(expressions, list)
         removeUiID(expressions) # remove random uiID to validate behaviour
         self.assertEqual(expressions, [{'Type': 'QUADRATIC', 'Coefficient': '', 'Offset': '', 'From': '', 'To': '', 'Iterator': '',
                                         'Term1': {'Indexes': [{'Value': '1', 'ClassID': cls.getUiID()}], 'VariableID': variable.getUiID()},
                                         'Term2': {'Indexes': [{'Value': '2', 'ClassID': cls.getUiID()}], 'VariableID': variable.getUiID()}, 'Childs': []}])
 
     # ADD EXPRESSION expression SQUAREDEXP
-    def test_addExpression_expression_SquaredExp(self):
-        qsoa = QSOAPlatform()
+    def test_Rule_addExpression_expression_SquaredExp(self):
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         rule = circuit.Rule('Rule', 1)
         squaredExp = circuit.SquaredExp(circuit.OffsetExp(1))
         
         ruleAdded = rule.addExpression(squaredExp)
 
         expressions = rule.getExpressions()
 
-        self.assertIsInstance(ruleAdded, qsoa.CircuitAnnealing.Rule)
+        self.assertEqual(type(ruleAdded).__name__, 'Rule')
         self.assertIsInstance(expressions, list)
         removeUiID(expressions) # remove random uiID to validate behaviour
         self.assertEqual(expressions, [{'Type': 'SQUARED', 'Coefficient': '', 'Offset': '', 'From': '', 'To': '', 'Iterator': '', 'Term1': {}, 'Term2': {},
                                         'Childs': [{'Type': 'OFFSET', 'Coefficient': '', 'Offset': '1', 'From': '', 'To': '', 'Iterator': '', 'Term1': {}, 'Term2': {}, 'Childs': []}]}])
 
-    # ADD EXPRESSION expression SQUAREDEXP
-    def test_addExpression_expression_SquaredExp(self):
-        qsoa = QSOAPlatform()
+    # ADD EXPRESSION expression SUMMATION
+    def test_Rule_addExpression_expression_Summation(self):
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         rule = circuit.Rule('Rule', 1)
         summation = circuit.SummationExp(1, 2, circuit.OffsetExp(1))
         
         ruleAdded = rule.addExpression(summation)
 
         expressions = rule.getExpressions()
 
-        self.assertIsInstance(ruleAdded, qsoa.CircuitAnnealing.Rule)
+        self.assertEqual(type(ruleAdded).__name__, 'Rule')
         self.assertIsInstance(expressions, list)
         removeUiID(expressions) # remove random uiID to validate behaviour
         self.assertEqual(expressions, [{'Type': 'SUMMATORY', 'Coefficient': '', 'Offset': '', 'From': '1', 'To': '2', 'Iterator': 'i', 'Term1': {}, 'Term2': {},
                                         'Childs': [{'Type': 'OFFSET', 'Coefficient': '', 'Offset': '1', 'From': '', 'To': '', 'Iterator': '', 'Term1': {}, 'Term2': {}, 'Childs': []}]}])
 
     # ADD EXPRESSION LIST OFFSETEXP, LINEAREXP, QUADRATICEXP, SQUAREDEXP, SUMMATIONEXP
-    def test_addExpression_list(self):
-        qsoa = QSOAPlatform()
+    def test_Rule_addExpression_list(self):
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         rule = circuit.Rule('Rule', 1)
         offsetExp = circuit.OffsetExp(1)
         linearExp = circuit.LinearExp((variable:=circuit.Variable('Variable', cls:=circuit.Class('Class', 1)), 1))
         quadraticExp = circuit.QuadraticExp((variable, 1), (variable, 2))
         squaredExp = circuit.SquaredExp(offsetExp)
         summation = circuit.SummationExp(1, 2, offsetExp)
 
         ruleAdded = rule.addExpression([offsetExp, linearExp, quadraticExp, squaredExp, summation])
 
         expressions = rule.getExpressions()
-        self.assertIsInstance(ruleAdded, qsoa.CircuitAnnealing.Rule)
+        self.assertEqual(type(ruleAdded).__name__, 'Rule')
         self.assertIsInstance(expressions, list)
         removeUiID(expressions) # remove random uiID to validate behaviour
         self.assertEqual(expressions, [{'Type': 'OFFSET', 'Coefficient': '', 'Offset': '1', 'From': '', 'To': '', 'Iterator': '', 'Term1': {}, 'Term2': {}, 'Childs': []},
                                        {'Type': 'LINEAR', 'Coefficient': '', 'Offset': '', 'From': '', 'To': '', 'Iterator': '',
                                         'Term1': {'Indexes': [{'Value': '1', 'ClassID': cls.getUiID()}], 'VariableID': variable.getUiID()},
                                         'Term2': {}, 'Childs': []}, 
                                        {'Type': 'QUADRATIC', 'Coefficient': '', 'Offset': '', 'From': '', 'To': '', 'Iterator': '',
@@ -2714,42 +3110,42 @@
                                         'Term2': {'Indexes': [{'Value': '2', 'ClassID': cls.getUiID()}], 'VariableID': variable.getUiID()}, 'Childs': []},
                                        {'Type': 'SQUARED', 'Coefficient': '', 'Offset': '', 'From': '', 'To': '', 'Iterator': '', 'Term1': {}, 'Term2': {},
                                         'Childs': [{'Type': 'OFFSET', 'Coefficient': '', 'Offset': '1', 'From': '', 'To': '', 'Iterator': '', 'Term1': {}, 'Term2': {}, 'Childs': []}]},
                                        {'Type': 'SUMMATORY', 'Coefficient': '', 'Offset': '', 'From': '1', 'To': '2', 'Iterator': 'i', 'Term1': {}, 'Term2': {},
                                         'Childs': [{'Type': 'OFFSET', 'Coefficient': '', 'Offset': '1', 'From': '', 'To': '', 'Iterator': '', 'Term1': {}, 'Term2': {}, 'Childs': []}]}])
 
     # BAD ARGUMENT expression LIST
-    def test_addExpression_badArgument_expression_list(self):
-        qsoa = QSOAPlatform()
+    def test_Rule_addExpression_badArgument_expression_list(self):
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         rule = circuit.Rule('Rule', 1)
 
         try:
             rule.addExpression([])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE expression
-    def test_addExpression_badArgumentType_expression(self):
-        qsoa = QSOAPlatform()
+    def test_Rule_addExpression_badArgumentType_expression(self):
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         rule = circuit.Rule('Rule', 1)
 
         try:
             rule.addExpression('expression')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE rule LIST
     def test_addVariable_badArgumentType_rule_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitAnnealing()
         rule = circuit.Rule('Rule', 1)
         offsetExp = circuit.OffsetExp(1)
 
         try:
             rule.addExpression([offsetExp, 'expression'])
             raise Exception
```

### Comparing `QuantumPathQSOAPySDK-1.5.3/test/test_circuit/test_CircuitFlow.py` & `QuantumPathQSOAPySDK-1.5.4/test/test_circuit/test_CircuitFlow.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,213 +2,223 @@
 from QuantumPathQSOAPySDK import QSOAPlatform
 
 ##################_____CIRCUITFLOW_____##################
 class Test_CircuitFlow(unittest.TestCase):
 
     # CIRCUIT FLOW
     def test_CircuitFlow(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         flow = qsoa.CircuitFlow()
 
-        self.assertIsInstance(flow, qsoa.CircuitFlow)
+        self.assertEqual(type(flow).__name__, 'CircuitFlow')
+
+    # NOT LOGGED IN
+    def test_CircuitFlow_notloggedIn(self):
+        qsoa = QSOAPlatform()
+
+        try:
+            qsoa.CircuitFlow()
+            raise Exception
 
+        except Exception as e:
+            self.assertEqual(type(e).__name__, 'AuthenticationError')
 
 ##################_____GET FLOW BODY_____##################
 class Test_GetFlowBody(unittest.TestCase):
 
     # GET FLOW BODY
     def test_getFlowBody(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         flow = qsoa.CircuitFlow()
 
         flowBody = flow.getFlowBody()
 
         self.assertIsInstance(flowBody, dict)
         self.assertEqual(flowBody, {'class': 'go.GraphLinksModel', 'nodeDataArray': [], 'linkDataArray': []})
 
 
 ##################_____GET PARSED BODY_____##################
 class Test_GetParsedBody(unittest.TestCase):
 
     # GET PARSED BODY
     def test_getParsedBody(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         flow = qsoa.CircuitFlow()
 
         parsedBody = flow.getParsedBody()
 
         self.assertIsInstance(parsedBody, str)
         self.assertEqual(parsedBody, '{"class":"go.GraphLinksModel","nodeDataArray":[],"linkDataArray":[]}')
 
 
 ##################_____START NODE_____##################
 class Test_StartNode(unittest.TestCase):
 
     # START NODE
     def test_startNode(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         flow = qsoa.CircuitFlow()
 
         startNode = flow.startNode()
 
         self.assertIsInstance(startNode, dict)
         self.assertEqual(startNode, {'category': 'Start', 'text': 'Start', 'key': -1, 'loc': ''})
         self.assertEqual(flow.getFlowBody(), {'class': 'go.GraphLinksModel', 'nodeDataArray': [{'category': 'Start', 'text': 'Start', 'key': -1, 'loc': ''}], 'linkDataArray': []})
 
 
 ##################_____INIT NODE_____##################
 class Test_InitNode(unittest.TestCase):
 
     # INIT NODE
     def test_initNode(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         flow = qsoa.CircuitFlow()
 
         initNode = flow.initNode(0)
 
         self.assertIsInstance(initNode, dict)
         self.assertEqual(initNode, {'category': 'Init', 'text': '0', 'key': -1, 'loc': ''})
         self.assertEqual(flow.getFlowBody(), {'class': 'go.GraphLinksModel', 'nodeDataArray': [{'category': 'Init', 'text': '0', 'key': -1, 'loc': ''}], 'linkDataArray': []})
     
     # BAD ARGUMENT TYPE startValue
     def test_initNode_badArgumentType_startValue(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         flow = qsoa.CircuitFlow()
 
         try:
             flow.initNode('startValue')
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
 
 ##################_____CIRCUIT NODE_____##################
 class Test_CircuitNode(unittest.TestCase):
 
     # CIRCUIT NODE
     def test_circuitNode(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         flow = qsoa.CircuitFlow()
 
         circuitNode = flow.circuitNode('circuitName')
 
         self.assertIsInstance(circuitNode, dict)
         self.assertEqual(circuitNode, {'category': 'Circuit', 'text': 'circuitName', 'key': -1, 'loc': ''})
         self.assertEqual(flow.getFlowBody(), {'class': 'go.GraphLinksModel', 'nodeDataArray': [{'category': 'Circuit', 'text': 'circuitName', 'key': -1, 'loc': ''}], 'linkDataArray': []})
     
     # BAD ARGUMENT TYPE circuitName
     def test_circuitNode_badArgumentType_circuitName(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         flow = qsoa.CircuitFlow()
 
         try:
             flow.circuitNode(99)
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
 
 ##################_____REPEAT NODE_____##################
 class Test_RepeatNode(unittest.TestCase):
 
     # REPEAT NODE
     def test_repeatNode(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         flow = qsoa.CircuitFlow()
 
         repeatNode = flow.repeatNode(1000)
 
         self.assertIsInstance(repeatNode, dict)
         self.assertEqual(repeatNode, {'category': 'Repeat', 'text': '1000', 'key': -1, 'loc': ''})
         self.assertEqual(flow.getFlowBody(), {'class': 'go.GraphLinksModel', 'nodeDataArray': [{'category': 'Repeat', 'text': '1000', 'key': -1, 'loc': ''}], 'linkDataArray': []})
     
     # BAD ARGUMENT TYPE numReps
     def test_repeatNode_badArgumentType_numReps(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         flow = qsoa.CircuitFlow()
 
         try:
             flow.repeatNode('numReps')
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
 
 ##################_____END NODE_____##################
 class Test_EndNode(unittest.TestCase):
 
     # END NODE
     def test_endNode(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         flow = qsoa.CircuitFlow()
 
         endNode = flow.endNode()
 
         self.assertIsInstance(endNode, dict)
         self.assertEqual(endNode, {'category': 'End', 'text': 'End', 'key': -1, 'loc': ''})
         self.assertEqual(flow.getFlowBody(), {'class': 'go.GraphLinksModel', 'nodeDataArray': [{'category': 'End', 'text': 'End', 'key': -1, 'loc': ''}], 'linkDataArray': []})
 
 
 ##################_____COMMENT NODE_____##################
 class Test_CommentNode(unittest.TestCase):
 
     # COMMENT NODE
     def test_commentNode(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         flow = qsoa.CircuitFlow()
 
         commentNode = flow.commentNode('comment')
 
         self.assertIsInstance(commentNode, dict)
         self.assertEqual(commentNode, {'category': 'Comment', 'text': 'comment', 'key': -1, 'loc': ''})
         self.assertEqual(flow.getFlowBody(), {'class': 'go.GraphLinksModel', 'nodeDataArray': [{'category': 'Comment', 'text': 'comment', 'key': -1, 'loc': ''}], 'linkDataArray': []})
     
     # BAD ARGUMENT TYPE numReps
     def test_commentNode_badArgumentType_numReps(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         flow = qsoa.CircuitFlow()
 
         try:
             flow.commentNode(99)
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
 
 ##################_____LINK NODES_____##################
 class Test_LinkNodes(unittest.TestCase):
 
     # LINK NODES
     def test_linkNodes(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         flow = qsoa.CircuitFlow()
         fromNode = flow.startNode()
         toNode = flow.startNode()
 
         link = flow.linkNodes(fromNode, toNode)
 
         self.assertIsInstance(link, dict)
         self.assertEqual(link, {'from': -1, 'to': -2, 'points': []})
         self.assertEqual(flow.getFlowBody(), {'class': 'go.GraphLinksModel', 'nodeDataArray': [{'category': 'Start', 'text': 'Start', 'key': -1, 'loc': ''}, {'category': 'Start', 'text': 'Start', 'key': -2, 'loc': ''}], 'linkDataArray': [{'from': -1, 'to': -2, 'points': []}]})
     
     # BAD ARGUMENT TYPE fromNode
     def test_linkNodes_badArgumentType_fromNode(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         flow = qsoa.CircuitFlow()
         toNode = flow.startNode()
 
         try:
             flow.linkNodes(99, toNode)
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE toNode
     def test_linkNodes_badArgumentType_toNode(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         flow = qsoa.CircuitFlow()
         fromNode = flow.startNode()
 
         try:
             flow.linkNodes(fromNode, 99)
 
         except Exception as e:
```

### Comparing `QuantumPathQSOAPySDK-1.5.3/test/test_circuit/test_CircuitGates.py` & `QuantumPathQSOAPySDK-1.5.4/test/test_circuit/test_CircuitGates_gates1.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,414 +1,205 @@
 import unittest
 from QuantumPathQSOAPySDK import QSOAPlatform
 
-##################_____CIRCUITGATES_____##################
-class Test_CircuitGates(unittest.TestCase):
-
-    # CIRCUIT GATES
-    def test_CircuitGates(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        self.assertIsInstance(circuit, qsoa.CircuitGates)
-
-
-##################_____GET CIRCUIT BODY_____##################
-class Test_GetCircuitBody(unittest.TestCase):
-
-    # GET CIRCUIT BODY EMPTY
-    def test_getCircuitBody_empty(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        circuitBody = circuit.getCircuitBody()
-
-        self.assertIsInstance(circuitBody, list)
-        self.assertEqual(circuitBody, [[]])
-
-
-##################_____GET PARSED BODY_____##################
-class Test_GetParsedBody(unittest.TestCase):
-
-    # GET PARSED BODY EMPTY
-    def test_getParsedBody_empty(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        parsedBody = circuit.getParsedBody()
-
-        self.assertIsInstance(parsedBody, str)
-        self.assertEqual(parsedBody, 'circuit={"cols": [[]], "init": []}')
-
-
-##################_____GET QUBIT STATES_____##################
-class Test_GetQubitStates(unittest.TestCase):
-
-    # GET QUBIT STATES EMPTY
-    def test_getQubitStates_empty(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        qubitStates = circuit.getQubitStates()
-
-        self.assertIsInstance(qubitStates, list)
-        self.assertEqual(qubitStates, [])
-    
-    # GET QUBIT STATES
-    def test_getQubitStates(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(2)
-
-        qubitStates = circuit.getQubitStates()
-
-        self.assertIsInstance(qubitStates, list)
-        self.assertEqual(qubitStates, ['0', '0', '0'])
-
-
-##################_____GET NUMBER OF QUBITS_____##################
-class Test_GetNumberOfQubits(unittest.TestCase):
-
-    # GET NUMBER OF QUBITS EMPTY
-    def test_getNumberOfQubits_empty(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        numberOfQubits = circuit.getNumberOfQubits()
-
-        self.assertIsInstance(numberOfQubits, int)
-        self.assertEqual(numberOfQubits, 0)
-    
-    # GET NUMBER OF QUBITS
-    def test_getNumberOfQubits(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(2)
-
-        numberOfQubits = circuit.getNumberOfQubits()
-
-        self.assertIsInstance(numberOfQubits, int)
-        self.assertEqual(numberOfQubits, 3)
-
-
-##################_____GET DEFAULT QUBIT STATE_____##################
-class Test_GetDefaultQubitState(unittest.TestCase):
-
-    # GET DEFAULT QUBIT STATE
-    def test_getDefaultQubitState(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        defaultQubitState = circuit.getDefaultQubitState()
-
-        self.assertIsInstance(defaultQubitState, str)
-        self.assertEqual(defaultQubitState, '0')
-
-
-##################_____SET DEFAULT QUBIT STATE_____##################
-class Test_SetDefaultQubitState(unittest.TestCase):
-
-    # SET DEFAULT QUBIT STATE
-    def test_setDefaultQubitState(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        circuit.setDefaultQubitState('1')
-
-        defaultQubitState = circuit.getDefaultQubitState()
-
-        self.assertIsInstance(defaultQubitState, str)
-        self.assertEqual(defaultQubitState, '1')
-
-    # SET DEFAULT STATE EXISTING CIRCUIT
-    def test_setDefaultQubitState_existingCircuit(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(0)
-        circuit.setDefaultQubitState('1')
-        circuit.h(2)
-
-        qubitStates = circuit.getQubitStates()
-
-        self.assertIsInstance(qubitStates, list)
-        self.assertEqual(qubitStates, ['0', '1', '1'])
-    
-    # BAD ARGUMENT qubitState
-    def test_setDefaultQubitState_badArgument_qubitState(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.setDefaultQubitState('state')
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, ValueError)
-    
-    # BAD ARGUMENT TYPE qubitState
-    def test_setDefaultQubitState_badArgumentType_qubitState(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.setDefaultQubitState(0)
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-
-##################_____INITIALIZE QUBIT STATES_____##################
-class Test_InitializeQubitStates(unittest.TestCase):
-
-    # INITIALIZE QUBIT STATES
-    def test_initializeQubitStates(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(2)
-
-        circuit.initializeQubitStates(['1', '1', '1'])
-
-        qubitStates = circuit.getQubitStates()
-
-        self.assertIsInstance(qubitStates, list)
-        self.assertEqual(qubitStates, ['1', '1', '1'])
-
-    # BAD ARGUMENT qubitStates
-    def test_initializeQubitStates_badArgument_qubitStates(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.initializeQubitStates(['1', '1', '1'])
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, ValueError)
-
-    # BAD ARGUMENT qubitStates LIST
-    def test_initializeQubitStates_badArgument_qubitStates_position_list(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.initializeQubitStates(['1', '1', 'state'])
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, ValueError)
-
-    # BAD ARGUMENT TYPE qubitStates
-    def test_initializeQubitStates_badArgumentType_qubitStates(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.initializeQubitStates('states')
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-    # BAD ARGUMENT TYPE qubitStates LIST
-    def test_initializeQubitStates_badArgumentType_qubitStates_position_list(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(2)
-
-        try:
-            circuit.initializeQubitStates(['1', '1', 1])
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
 
 ##################_____H_____##################
 class Test_H(unittest.TestCase):
 
     # H position 0
     def test_h_position_0(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.h(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [['H']])
 
     # H position 1
     def test_h_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.h(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [[1, 'H']])
 
     # H EXISTING CIRCUIT position NEW COLUMN
     def test_h_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.h(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], ['H']])
 
     # H EXISTING CIRCUIT position SAME COLUMN
     def test_h_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.h(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [['H', 'H']])
 
     # H EXISTING CIRCUIT position BETWEEN SWAP
     def test_h_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.h(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, 'H']])
 
     # H EXISTING CIRCUIT position UNDER SWAP
     def test_h_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.h(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'H']])
 
     # H position LIST
     def test_h_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.h([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'H'), (1, 'H'), (2, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [['H', 'H', 'H']])
     
     # H position position LIST EXISTING CIRCUIT
     def test_h_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(0)
 
         gate = circuit.h([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'H'), (1, 'H'), (2, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [['X', 'H', 'H'], ['H']])
 
     # H position position LIST EXISTING CIRCUIT WITH SWAP
     def test_h_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.h([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'H'), (1, 'H'), (2, 'H'), (3, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['H', 'H', 'H', 'H']])
 
     # H position ALL
     def test_h_position_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(1)
 
         gate = circuit.h()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'H'), (1, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [['H', 'X'], [1, 'H']])
     
     # H position position ALL BETWEEN SWAP
     def test_h_position_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.h()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'H'), (1, 'H'), (2, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['H', 'H', 'H']])
 
     # H add
     def test_h_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.h(0, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position LIST
+    def test_h_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.h([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_h_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.h([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_h_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.h('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_h_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.h([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_h_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.h(0, 'add')
             raise Exception
 
         except Exception as e:
@@ -416,192 +207,204 @@
 
 
 ##################_____X_____##################
 class Test_X(unittest.TestCase):
 
     # X position 0
     def test_x_position_0(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.x(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [['X']])
 
     # X position 1
     def test_x_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.x(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [[1, 'X']])
 
     # X EXISTING CIRCUIT position NEW COLUMN
     def test_x_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.x(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], ['X']])
 
     # X EXISTING CIRCUIT position SAME COLUMN
     def test_x_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.x(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [['H', 'X']])
 
     # X EXISTING CIRCUIT position BETWEEN SWAP
     def test_x_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.x(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, 'X']])
 
     # X EXISTING CIRCUIT position UNDER SWAP
     def test_x_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.x(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'X']])
 
     # X position LIST
     def test_x_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.x([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'X'), (1, 'X'), (2, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [['X', 'H', 'X'], [1, 'X']])
     
     # X position position LIST EXISTING CIRCUIT
     def test_x_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.x([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'X'), (1, 'X'), (2, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [['H', 'X', 'X'], ['X']])
 
     # X position position LIST EXISTING CIRCUIT WITH SWAP
     def test_x_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.x([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'X'), (1, 'X'), (2, 'X'), (3, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['X', 'X', 'X', 'X']])
 
     # X position ALL
     def test_x_position_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.x()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'X'), (1, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [['X', 'H'], [1, 'X']])
 
     # X position position ALL BETWEEN SWAP
     def test_x_position_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.x()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'X'), (1, 'X'), (2, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['X', 'X', 'X']])
 
     # X add
     def test_x_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.x(0, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position LIST
+    def test_x_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.x([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_x_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.x([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_x_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.x('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_x_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.x([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_x_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.x(0, 'add')
             raise Exception
 
         except Exception as e:
@@ -609,192 +412,204 @@
 
 
 ##################_____Y_____##################
 class Test_Y(unittest.TestCase):
 
     # Y position 0
     def test_y_position_0(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.y(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'Y')])
         self.assertEqual(circuit.getCircuitBody(), [['Y']])
 
     # Y position 1
     def test_y_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.y(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'Y')])
         self.assertEqual(circuit.getCircuitBody(), [[1, 'Y']])
 
     # Y EXISTING CIRCUIT position NEW COLUMN
     def test_y_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.y(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'Y')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], ['Y']])
 
     # Y EXISTING CIRCUIT position SAME COLUMN
     def test_y_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.y(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'Y')])
         self.assertEqual(circuit.getCircuitBody(), [['H', 'Y']])
 
     # Y EXISTING CIRCUIT position BETWEEN SWAP
     def test_y_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.y(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'Y')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, 'Y']])
 
     # Y EXISTING CIRCUIT position UNDER SWAP
     def test_y_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.y(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, 'Y')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'Y']])
 
     # Y position LIST
     def test_y_position_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.y([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'Y'), (1, 'Y'), (2, 'Y')])
         self.assertEqual(circuit.getCircuitBody(), [['Y', 'H', 'Y'], [1, 'Y']])
     
     # Y position position LIST EXISTING CIRCUIT
     def test_y_position_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(0)
 
         gate = circuit.y([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'Y'), (1, 'Y'), (2, 'Y')])
         self.assertEqual(circuit.getCircuitBody(), [['X', 'Y', 'Y'], ['Y']])
 
     # Y position position LIST EXISTING CIRCUIT WITH SWAP
     def test_y_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.y([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'Y'), (1, 'Y'), (2, 'Y'), (3, 'Y')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['Y', 'Y', 'Y', 'Y']])
 
     # Y position ALL
     def test_y_position_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.y()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'Y'), (1, 'Y')])
         self.assertEqual(circuit.getCircuitBody(), [['Y', 'H'], [1, 'Y']])
 
     # Y position position ALL BETWEEN SWAP
     def test_y_position_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.y()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'Y'), (1, 'Y'), (2, 'Y')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['Y', 'Y', 'Y']])
 
     # Y add
     def test_y_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.y(0, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'Y')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position LIST
+    def test_y_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.y([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_y_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.y([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_y_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.y('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_y_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.y([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_y_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.y(0, 'add')
             raise Exception
 
         except Exception as e:
@@ -802,192 +617,204 @@
 
 
 ##################_____Z_____##################
 class Test_Z(unittest.TestCase):
 
     # Z position 0
     def test_z_position_0(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.z(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'Z')])
         self.assertEqual(circuit.getCircuitBody(), [['Z']])
 
     # Z position 1
     def test_z_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.z(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'Z')])
         self.assertEqual(circuit.getCircuitBody(), [[1, 'Z']])
 
     # Z EXISTING CIRCUIT position NEW COLUMN
     def test_z_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.z(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'Z')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], ['Z']])
 
     # Z EXISTING CIRCUIT position SAME COLUMN
     def test_z_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.z(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'Z')])
         self.assertEqual(circuit.getCircuitBody(), [['H', 'Z']])
 
     # Z EXISTING CIRCUIT position BETWEEN SWAP
     def test_z_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.z(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'Z')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, 'Z']])
 
     # Z EXISTING CIRCUIT position UNDER SWAP
     def test_z_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.z(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, 'Z')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'Z']])
 
     # Z position LIST
     def test_z_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.z([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'Z'), (1, 'Z'), (2, 'Z')])
         self.assertEqual(circuit.getCircuitBody(), [['Z', 'H', 'Z'], [1, 'Z']])
     
     # Z position position LIST EXISTING CIRCUIT
     def test_z_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(0)
 
         gate = circuit.z([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'Z'), (1, 'Z'), (2, 'Z')])
         self.assertEqual(circuit.getCircuitBody(), [['X', 'Z', 'Z'], ['Z']])
 
     # Z position position LIST EXISTING CIRCUIT WITH SWAP
     def test_z_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.z([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'Z'), (1, 'Z'), (2, 'Z'), (3, 'Z')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['Z', 'Z', 'Z', 'Z']])
 
     # Z position ALL
     def test_z_position_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.z()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'Z'), (1, 'Z')])
         self.assertEqual(circuit.getCircuitBody(), [['Z', 'H'], [1, 'Z']])
 
     # Z position position ALL BETWEEN SWAP
     def test_z_position_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.z()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'Z'), (1, 'Z'), (2, 'Z')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['Z', 'Z', 'Z']])
 
     # Z add
     def test_z_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.z(0, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'Z')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position LIST
+    def test_z_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.z([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_z_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.z([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_z_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.z('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_z_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.z([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_z_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.z(0, 'add')
             raise Exception
 
         except Exception as e:
@@ -995,192 +822,204 @@
 
 
 ##################_____S_____##################
 class Test_S(unittest.TestCase):
 
     # S position 0
     def test_s_position_0(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.s(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'S')])
         self.assertEqual(circuit.getCircuitBody(), [['S']])
 
     # S position 1
     def test_s_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.s(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'S')])
         self.assertEqual(circuit.getCircuitBody(), [[1, 'S']])
 
     # S EXISTING CIRCUIT position NEW COLUMN
     def test_s_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.s(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'S')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], ['S']])
 
     # S EXISTING CIRCUIT position SAME COLUMN
     def test_s_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.s(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'S')])
         self.assertEqual(circuit.getCircuitBody(), [['H', 'S']])
 
     # S EXISTING CIRCUIT position BETWEEN SWAP
     def test_s_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.s(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'S')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, 'S']])
 
     # S EXISTING CIRCUIT position UNDER SWAP
     def test_s_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.s(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, 'S')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'S']])
 
     # S LIST
     def test_s_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.s([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'S'), (1, 'S'), (2, 'S')])
         self.assertEqual(circuit.getCircuitBody(), [['S', 'H', 'S'], [1, 'S']])
     
     # S position LIST EXISTING CIRCUIT
     def test_s_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(0)
 
         gate = circuit.s([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'S'), (1, 'S'), (2, 'S')])
         self.assertEqual(circuit.getCircuitBody(), [['X', 'S', 'S'], ['S']])
 
     # S position LIST EXISTING CIRCUIT WITH SWAP
     def test_s_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.s([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'S'), (1, 'S'), (2, 'S'), (3, 'S')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['S', 'S', 'S', 'S']])
 
     # S ALL
     def test_s_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.s()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'S'), (1, 'S')])
         self.assertEqual(circuit.getCircuitBody(), [['S', 'H'], [1, 'S']])
 
     # S position ALL BETWEEN SWAP
     def test_s_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.s()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'S'), (1, 'S'), (2, 'S')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['S', 'S', 'S']])
 
     # S add
     def test_s_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.s(0, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'S')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position LIST
+    def test_s_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.s([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_s_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.s([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_s_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.s('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_s_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.s([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_s_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.s(0, 'add')
             raise Exception
 
         except Exception as e:
@@ -1188,192 +1027,204 @@
 
 
 ##################_____I_S_____##################
 class Test_I_S(unittest.TestCase):
 
     # I_S
     def test_i_s(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.i_s(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_S')])
         self.assertEqual(circuit.getCircuitBody(), [['I_S']])
 
     # I_S Q1
     def test_i_s_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.i_s(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'I_S')])
         self.assertEqual(circuit.getCircuitBody(), [[1, 'I_S']])
 
     # I_S EXISTING CIRCUIT position NEW COLUMN
     def test_i_s_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.i_s(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_S')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], ['I_S']])
 
     # I_S EXISTING CIRCUIT position SAME COLUMN
     def test_i_s_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.i_s(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'I_S')])
         self.assertEqual(circuit.getCircuitBody(), [['H', 'I_S']])
 
     # I_S EXISTING CIRCUIT position BETWEEN SWAP
     def test_i_s_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.i_s(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'I_S')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, 'I_S']])
 
     # I_S EXISTING CIRCUIT position UNDER SWAP
     def test_i_s_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.i_s(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, 'I_S')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'I_S']])
 
     # I_S LIST
     def test_i_s_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.i_s([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_S'), (1, 'I_S'), (2, 'I_S')])
         self.assertEqual(circuit.getCircuitBody(), [['I_S', 'H', 'I_S'], [1, 'I_S']])
     
     # I_S position LIST EXISTING CIRCUIT
     def test_i_s_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(0)
 
         gate = circuit.i_s([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_S'), (1, 'I_S'), (2, 'I_S')])
         self.assertEqual(circuit.getCircuitBody(), [['X', 'I_S', 'I_S'], ['I_S']])
 
     # I_S position LIST EXISTING CIRCUIT WITH SWAP
     def test_i_s_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.i_s([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_S'), (1, 'I_S'), (2, 'I_S'), (3, 'I_S')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['I_S', 'I_S', 'I_S', 'I_S']])
 
     # I_S ALL
     def test_i_s_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.i_s()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_S'), (1, 'I_S')])
         self.assertEqual(circuit.getCircuitBody(), [['I_S', 'H'], [1, 'I_S']])
 
     # I_S position ALL BETWEEN SWAP
     def test_i_s_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.i_s()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_S'), (1, 'I_S'), (2, 'I_S')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['I_S', 'I_S', 'I_S']])
 
     # I_S add
     def test_i_s_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.i_s(0, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_S')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position LIST
+    def test_i_s_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.i_s([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_i_s_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_s([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_i_s_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_s('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_i_s_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_s([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_i_s_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_s(0, 'add')
             raise Exception
 
         except Exception as e:
@@ -1381,192 +1232,204 @@
 
 
 ##################_____SX_____##################
 class Test_SX(unittest.TestCase):
 
     # SX
     def test_sx(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.sx(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'SX')])
         self.assertEqual(circuit.getCircuitBody(), [['SX']])
 
     # SX Q1
     def test_sx_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.sx(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'SX')])
         self.assertEqual(circuit.getCircuitBody(), [[1, 'SX']])
 
     # SX EXISTING CIRCUIT position NEW COLUMN
     def test_sx_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.sx(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'SX')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], ['SX']])
 
     # SX EXISTING CIRCUIT position SAME COLUMN
     def test_sx_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.sx(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'SX')])
         self.assertEqual(circuit.getCircuitBody(), [['H', 'SX']])
 
     # SX EXISTING CIRCUIT position BETWEEN SWAP
     def test_sx_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.sx(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'SX')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, 'SX']])
 
     # SX EXISTING CIRCUIT position UNDER SWAP
     def test_sx_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.sx(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, 'SX')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'SX']])
 
     # SX LIST
     def test_sx_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.sx([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'SX'), (1, 'SX'), (2, 'SX')])
         self.assertEqual(circuit.getCircuitBody(), [['SX', 'H', 'SX'], [1, 'SX']])
     
     # SX position LIST EXISTING CIRCUIT
     def test_sx_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(0)
 
         gate = circuit.sx([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'SX'), (1, 'SX'), (2, 'SX')])
         self.assertEqual(circuit.getCircuitBody(), [['X', 'SX', 'SX'], ['SX']])
 
     # SX position LIST EXISTING CIRCUIT WITH SWAP
     def test_sx_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.sx([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'SX'), (1, 'SX'), (2, 'SX'), (3, 'SX')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['SX', 'SX', 'SX', 'SX']])
 
     # SX ALL
     def test_sx_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.sx()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'SX'), (1, 'SX')])
         self.assertEqual(circuit.getCircuitBody(), [['SX', 'H'], [1, 'SX']])
 
     # SX position ALL BETWEEN SWAP
     def test_sx_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.sx()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'SX'), (1, 'SX'), (2, 'SX')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['SX', 'SX', 'SX']])
 
     # SX add
     def test_sx_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.sx(0, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'SX')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position LIST
+    def test_sx_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.sx([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_sx_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.sx([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_sx_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.sx('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_sx_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.sx([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_sx_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.sx(0, 'add')
             raise Exception
 
         except Exception as e:
@@ -1574,192 +1437,204 @@
 
 
 ##################_____I_SX_____##################
 class Test_I_SX(unittest.TestCase):
 
     # I_SX
     def test_i_sx(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.i_sx(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_SX')])
         self.assertEqual(circuit.getCircuitBody(), [['I_SX']])
 
     # I_SX Q1
     def test_i_sx_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.i_sx(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'I_SX')])
         self.assertEqual(circuit.getCircuitBody(), [[1, 'I_SX']])
 
     # I_SX EXISTING CIRCUIT position NEW COLUMN
     def test_i_sx_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.i_sx(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_SX')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], ['I_SX']])
 
     # H EXISTING CIRCUIT position SAME COLUMN
     def test_i_sx_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.i_sx(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'I_SX')])
         self.assertEqual(circuit.getCircuitBody(), [['H', 'I_SX']])
 
     # H EXISTING CIRCUIT position BETWEEN SWAP
     def test_i_sx_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.i_sx(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'I_SX')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, 'I_SX']])
 
     # H EXISTING CIRCUIT position UNDER SWAP
     def test_i_sx_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.i_sx(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, 'I_SX')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'I_SX']])
 
     # I_SX LIST
     def test_i_sx_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.i_sx([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_SX'), (1, 'I_SX'), (2, 'I_SX')])
         self.assertEqual(circuit.getCircuitBody(), [['I_SX', 'H', 'I_SX'], [1, 'I_SX']])
     
     # I_SX position LIST EXISTING CIRCUIT
     def test_i_sx_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(0)
 
         gate = circuit.i_sx([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_SX'), (1, 'I_SX'), (2, 'I_SX')])
         self.assertEqual(circuit.getCircuitBody(), [['X', 'I_SX', 'I_SX'], ['I_SX']])
 
     # I_SX position LIST EXISTING CIRCUIT WITH SWAP
     def test_i_sx_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.i_sx([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_SX'), (1, 'I_SX'), (2, 'I_SX'), (3, 'I_SX')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['I_SX', 'I_SX', 'I_SX', 'I_SX']])
 
     # I_SX ALL
     def test_i_sx_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.i_sx()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_SX'), (1, 'I_SX')])
         self.assertEqual(circuit.getCircuitBody(), [['I_SX', 'H'], [1, 'I_SX']])
 
     # I_SX position ALL BETWEEN SWAP
     def test_i_sx_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.i_sx()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_SX'), (1, 'I_SX'), (2, 'I_SX')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['I_SX', 'I_SX', 'I_SX']])
 
     # I_SX add
     def test_i_sx_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.i_sx(0, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_SX')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position LIST
+    def test_i_sx_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.i_sx([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_i_sx_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_sx([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_i_sx_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_sx('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_i_sx_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_sx([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_i_sx_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_sx(0, 'add')
             raise Exception
 
         except Exception as e:
@@ -1767,192 +1642,204 @@
 
 
 ##################_____SY_____##################
 class Test_SY(unittest.TestCase):
 
     # SY
     def test_sy(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.sy(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'SY')])
         self.assertEqual(circuit.getCircuitBody(), [['SY']])
 
     # SY Q1
     def test_sy_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.sy(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'SY')])
         self.assertEqual(circuit.getCircuitBody(), [[1, 'SY']])
 
     # SY EXISTING CIRCUIT position NEW COLUMN
     def test_sy_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.sy(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'SY')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], ['SY']])
 
     # SY EXISTING CIRCUIT position SAME COLUMN
     def test_sy_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.sy(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'SY')])
         self.assertEqual(circuit.getCircuitBody(), [['H', 'SY']])
 
     # SY EXISTING CIRCUIT position BETWEEN SWAP
     def test_sy_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.sy(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'SY')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, 'SY']])
 
     # SY EXISTING CIRCUIT position UNDER SWAP
     def test_sy_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.sy(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, 'SY')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'SY']])
 
     # SY LIST
     def test_sy_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.sy([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'SY'), (1, 'SY'), (2, 'SY')])
         self.assertEqual(circuit.getCircuitBody(), [['SY', 'H', 'SY'], [1, 'SY']])
     
     # SY position LIST EXISTING CIRCUIT
     def test_sy_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(0)
 
         gate = circuit.sy([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'SY'), (1, 'SY'), (2, 'SY')])
         self.assertEqual(circuit.getCircuitBody(), [['X', 'SY', 'SY'], ['SY']])
 
     # SY position LIST EXISTING CIRCUIT WITH SWAP
     def test_sy_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.sy([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'SY'), (1, 'SY'), (2, 'SY'), (3, 'SY')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['SY', 'SY', 'SY', 'SY']])
 
     # SY ALL
     def test_sy_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.sy()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'SY'), (1, 'SY')])
         self.assertEqual(circuit.getCircuitBody(), [['SY', 'H'], [1, 'SY']])
 
     # SY position ALL BETWEEN SWAP
     def test_sy_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.sy()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'SY'), (1, 'SY'), (2, 'SY')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['SY', 'SY', 'SY']])
 
     # SY add
     def test_sy_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.sy(0, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'SY')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position LIST
+    def test_sy_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.sy([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_sy_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.sy([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_sy_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.sy('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_sy_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.sy([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_sy_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.sy(0, 'add')
             raise Exception
 
         except Exception as e:
@@ -1960,192 +1847,204 @@
 
 
 ##################_____I_SY_____##################
 class Test_I_SY(unittest.TestCase):
 
     # I_SY
     def test_i_sy(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.i_sy(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_SY')])
         self.assertEqual(circuit.getCircuitBody(), [['I_SY']])
 
     # I_SY Q1
     def test_i_sy_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.i_sy(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'I_SY')])
         self.assertEqual(circuit.getCircuitBody(), [[1, 'I_SY']])
 
     # I_SY EXISTING CIRCUIT position NEW COLUMN
     def test_i_sy_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.i_sy(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_SY')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], ['I_SY']])
 
     # I_SY EXISTING CIRCUIT position SAME COLUMN
     def test_i_sy_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.i_sy(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'I_SY')])
         self.assertEqual(circuit.getCircuitBody(), [['H', 'I_SY']])
 
     # I_SY EXISTING CIRCUIT position BETWEEN SWAP
     def test_i_sy_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.i_sy(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'I_SY')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, 'I_SY']])
 
     # I_SY EXISTING CIRCUIT position UNDER SWAP
     def test_i_sy_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.i_sy(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, 'I_SY')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'I_SY']])
 
     # I_SY position LIST
     def test_i_sy_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.i_sy([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_SY'), (1, 'I_SY'), (2, 'I_SY')])
         self.assertEqual(circuit.getCircuitBody(), [['I_SY', 'H', 'I_SY'], [1, 'I_SY']])
     
     # I_SY position position LIST EXISTING CIRCUIT
     def test_i_sy_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(0)
 
         gate = circuit.i_sy([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_SY'), (1, 'I_SY'), (2, 'I_SY')])
         self.assertEqual(circuit.getCircuitBody(), [['X', 'I_SY', 'I_SY'], ['I_SY']])
 
     # I_SY position position LIST EXISTING CIRCUIT WITH SWAP
     def test_i_sy_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.i_sy([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_SY'), (1, 'I_SY'), (2, 'I_SY'), (3, 'I_SY')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['I_SY', 'I_SY', 'I_SY', 'I_SY']])
 
     # I_SY position ALL
     def test_i_sy_position_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.i_sy()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_SY'), (1, 'I_SY')])
         self.assertEqual(circuit.getCircuitBody(), [['I_SY', 'H'], [1, 'I_SY']])
 
     # I_SY position position ALL BETWEEN SWAP
     def test_i_sy_position_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.i_sy()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_SY'), (1, 'I_SY'), (2, 'I_SY')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['I_SY', 'I_SY', 'I_SY']])
 
     # I_SY add
     def test_i_sy_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.i_sy(0, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_SY')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position LIST
+    def test_i_sy_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.i_sy([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_i_sy_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_sy([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_i_sy_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_sy('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_i_sy_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_sy([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_i_sy_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_sy(0, 'add')
             raise Exception
 
         except Exception as e:
@@ -2153,192 +2052,204 @@
 
 
 ##################_____T_____##################
 class Test_T(unittest.TestCase):
 
     # T position 0
     def test_t_position_0(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.t(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'T')])
         self.assertEqual(circuit.getCircuitBody(), [['T']])
 
     # T position 1
     def test_t_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.t(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'T')])
         self.assertEqual(circuit.getCircuitBody(), [[1, 'T']])
 
     # T EXISTING CIRCUIT position NEW COLUMN
     def test_t_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.t(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'T')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], ['T']])
 
     # T EXISTING CIRCUIT position SAME COLUMN
     def test_t_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.t(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'T')])
         self.assertEqual(circuit.getCircuitBody(), [['H', 'T']])
 
     # T EXISTING CIRCUIT position BETWEEN SWAP
     def test_t_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.t(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'T')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, 'T']])
 
     # T EXISTING CIRCUIT position UNDER SWAP
     def test_t_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.t(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, 'T')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'T']])
 
     # T position LIST
     def test_t_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.t([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'T'), (1, 'T'), (2, 'T')])
         self.assertEqual(circuit.getCircuitBody(), [['T', 'H', 'T'], [1, 'T']])
     
     # T position position LIST EXISTING CIRCUIT
     def test_t_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(0)
 
         gate = circuit.t([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'T'), (1, 'T'), (2, 'T')])
         self.assertEqual(circuit.getCircuitBody(), [['X', 'T', 'T'], ['T']])
 
     # T position position LIST EXISTING CIRCUIT WITH SWAP
     def test_t_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.t([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'T'), (1, 'T'), (2, 'T'), (3, 'T')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['T', 'T', 'T', 'T']])
 
     # T position ALL
     def test_t_position_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.t()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'T'), (1, 'T')])
         self.assertEqual(circuit.getCircuitBody(), [['T', 'H'], [1, 'T']])
 
     # T position position ALL BETWEEN SWAP
     def test_t_position_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.t()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'T'), (1, 'T'), (2, 'T')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['T', 'T', 'T']])
 
     # T add
     def test_t_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.t(0, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'T')])
         self.assertEqual(circuit.getCircuitBody(), [[]]) # check circuit body
 
+    # BAD ARGUMENT position LIST
+    def test_t_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.t([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_t_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.t([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_t_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.t('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_t_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.t([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_t_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.t(0, 'add')
             raise Exception
 
         except Exception as e:
@@ -2346,192 +2257,204 @@
 
 
 ##################_____I_T_____##################
 class Test_I_T(unittest.TestCase):
 
     # I_T position 0
     def test_i_t_position_0(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.i_t(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_T')])
         self.assertEqual(circuit.getCircuitBody(), [['I_T']])
 
     # I_T position 1
     def test_i_t_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.i_t(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'I_T')])
         self.assertEqual(circuit.getCircuitBody(), [[1, 'I_T']])
 
     # I_T EXISTING CIRCUIT position NEW COLUMN
     def test_i_t_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.i_t(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_T')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], ['I_T']])
 
     # I_T EXISTING CIRCUIT position SAME COLUMN
     def test_i_t_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.i_t(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'I_T')])
         self.assertEqual(circuit.getCircuitBody(), [['H', 'I_T']])
 
     # I_T EXISTING CIRCUIT position BETWEEN SWAP
     def test_i_t_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.i_t(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'I_T')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, 'I_T']])
 
     # I_T EXISTING CIRCUIT position UNDER SWAP
     def test_i_t_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.i_t(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, 'I_T')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'I_T']])
 
     # I_T position LIST
     def test_i_t_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.i_t([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_T'), (1, 'I_T'), (2, 'I_T')])
         self.assertEqual(circuit.getCircuitBody(), [['I_T', 'H', 'I_T'], [1, 'I_T']])
     
     # I_T position position LIST EXISTING CIRCUIT
     def test_i_t_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(0)
 
         gate = circuit.i_t([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_T'), (1, 'I_T'), (2, 'I_T')])
         self.assertEqual(circuit.getCircuitBody(), [['X', 'I_T', 'I_T'], ['I_T']])
 
     # I_T position position LIST EXISTING CIRCUIT WITH SWAP
     def test_i_t_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.i_t([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_T'), (1, 'I_T'), (2, 'I_T'), (3, 'I_T')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['I_T', 'I_T', 'I_T', 'I_T']])
 
     # I_T position ALL
     def test_i_t_position_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.i_t()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_T'), (1, 'I_T')])
         self.assertEqual(circuit.getCircuitBody(), [['I_T', 'H'], [1, 'I_T']])
 
     # I_T position position ALL BETWEEN SWAP
     def test_i_t_position_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.i_t()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_T'), (1, 'I_T'), (2, 'I_T')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['I_T', 'I_T', 'I_T']])
 
     # I_T add
     def test_i_t_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.i_t(0, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_T')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position LIST
+    def test_i_t_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.i_t([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_i_t_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_t([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_i_t_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_t('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_i_t_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_t([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_i_t_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_t(0, 'add')
             raise Exception
 
         except Exception as e:
@@ -2539,192 +2462,204 @@
 
 
 ##################_____TX_____##################
 class Test_TX(unittest.TestCase):
 
     # TX position 0
     def test_tx_position_0(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.tx(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'TX')])
         self.assertEqual(circuit.getCircuitBody(), [['TX']])
 
     # TX position 1
     def test_tx_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.tx(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'TX')])
         self.assertEqual(circuit.getCircuitBody(), [[1, 'TX']])
 
     # TX EXISTING CIRCUIT position NEW COLUMN
     def test_tx_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.tx(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'TX')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], ['TX']])
 
     # TX EXISTING CIRCUIT position SAME COLUMN
     def test_tx_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.tx(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'TX')])
         self.assertEqual(circuit.getCircuitBody(), [['H', 'TX']])
 
     # TX EXISTING CIRCUIT position BETWEEN SWAP
     def test_tx_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.tx(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'TX')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, 'TX']])
 
     # TX EXISTING CIRCUIT position UNDER SWAP
     def test_tx_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.tx(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, 'TX')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'TX']])
 
     # TX LIST
     def test_tx_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.tx([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'TX'), (1, 'TX'), (2, 'TX')])
         self.assertEqual(circuit.getCircuitBody(), [['TX', 'H', 'TX'], [1, 'TX']])
     
     # TX position LIST EXISTING CIRCUIT
     def test_tx_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(0)
 
         gate = circuit.tx([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'TX'), (1, 'TX'), (2, 'TX')])
         self.assertEqual(circuit.getCircuitBody(), [['X', 'TX', 'TX'], ['TX']])
 
     # TX position LIST EXISTING CIRCUIT WITH SWAP
     def test_tx_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.tx([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'TX'), (1, 'TX'), (2, 'TX'), (3, 'TX')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['TX', 'TX', 'TX', 'TX']])
 
     # TX position ALL
     def test_tx_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.tx()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'TX'), (1, 'TX')])
         self.assertEqual(circuit.getCircuitBody(), [['TX', 'H'], [1, 'TX']])
 
     # TX position ALL BETWEEN SWAP
     def test_tx_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.tx()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'TX'), (1, 'TX'), (2, 'TX')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['TX', 'TX', 'TX']])
 
     # TX add
     def test_tx_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.tx(0, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'TX')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position LIST
+    def test_tx_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.tx([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_tx_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.tx([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_tx_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.tx('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_tx_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.tx([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_tx_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.tx(0, 'add')
             raise Exception
 
         except Exception as e:
@@ -2732,192 +2667,204 @@
 
 
 ##################_____I_TX_____##################
 class Test_I_TX(unittest.TestCase):
 
     # I_TX position 0
     def test_i_tx_position_0(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.i_tx(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_TX')])
         self.assertEqual(circuit.getCircuitBody(), [['I_TX']])
 
     # I_TX position 1
     def test_i_tx_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.i_tx(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'I_TX')])
         self.assertEqual(circuit.getCircuitBody(), [[1, 'I_TX']])
 
     # I_TX EXISTING CIRCUIT position NEW COLUMN
     def test_i_tx_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.i_tx(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_TX')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], ['I_TX']])
 
     # I_TX EXISTING CIRCUIT position SAME COLUMN
     def test_i_tx_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.i_tx(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'I_TX')])
         self.assertEqual(circuit.getCircuitBody(), [['H', 'I_TX']])
 
     # I_TX EXISTING CIRCUIT position BETWEEN SWAP
     def test_i_tx_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.i_tx(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'I_TX')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, 'I_TX']])
 
     # I_TX EXISTING CIRCUIT position UNDER SWAP
     def test_i_tx_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.i_tx(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, 'I_TX')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'I_TX']])
 
     # I_TX position LIST
     def test_i_tx_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.i_tx([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_TX'), (1, 'I_TX'), (2, 'I_TX')])
         self.assertEqual(circuit.getCircuitBody(), [['I_TX', 'H', 'I_TX'], [1, 'I_TX']])
     
     # I_TX position LIST EXISTING CIRCUIT
     def test_i_tx_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(0)
 
         gate = circuit.i_tx([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_TX'), (1, 'I_TX'), (2, 'I_TX')])
         self.assertEqual(circuit.getCircuitBody(), [['X', 'I_TX', 'I_TX'], ['I_TX']])
 
     # I_TX position LIST EXISTING CIRCUIT WITH SWAP
     def test_i_tx_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.i_tx([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_TX'), (1, 'I_TX'), (2, 'I_TX'), (3, 'I_TX')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['I_TX', 'I_TX', 'I_TX', 'I_TX']])
 
     # I_TX position ALL
     def test_i_tx_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.i_tx()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_TX'), (1, 'I_TX')])
         self.assertEqual(circuit.getCircuitBody(), [['I_TX', 'H'], [1, 'I_TX']])
 
     # I_TX position ALL BETWEEN SWAP
     def test_i_tx_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.i_tx()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_TX'), (1, 'I_TX'), (2, 'I_TX')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['I_TX', 'I_TX', 'I_TX']])
 
     # I_TX add
     def test_i_tx_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.i_tx(0, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_TX')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position LIST
+    def test_i_tx_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.i_tx([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_i_tx_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_tx([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_i_tx_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_tx('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_i_tx_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_tx([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_i_tx_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_tx(0, 'add')
             raise Exception
 
         except Exception as e:
@@ -2925,192 +2872,204 @@
 
 
 ##################_____TY_____##################
 class Test_TY(unittest.TestCase):
 
     # TY position 0
     def test_ty_position_0(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.ty(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'TY')])
         self.assertEqual(circuit.getCircuitBody(), [['TY']])
 
     # TY position 1
     def test_ty_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.ty(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'TY')])
         self.assertEqual(circuit.getCircuitBody(), [[1, 'TY']])
 
     # TY EXISTING CIRCUIT position NEW COLUMN
     def test_ty_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.ty(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'TY')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], ['TY']])
 
     # TY EXISTING CIRCUIT position SAME COLUMN
     def test_ty_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.ty(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'TY')])
         self.assertEqual(circuit.getCircuitBody(), [['H', 'TY']])
 
     # TY EXISTING CIRCUIT position BETWEEN SWAP
     def test_ty_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.ty(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'TY')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, 'TY']])
 
     # TY EXISTING CIRCUIT position UNDER SWAP
     def test_ty_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.ty(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, 'TY')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'TY']])
 
     # TY position LIST
     def test_ty_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.ty([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'TY'), (1, 'TY'), (2, 'TY')])
         self.assertEqual(circuit.getCircuitBody(), [['TY', 'H', 'TY'], [1, 'TY']])
     
     # TY position LIST EXISTING CIRCUIT
     def test_ty_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(0)
 
         gate = circuit.ty([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'TY'), (1, 'TY'), (2, 'TY')])
         self.assertEqual(circuit.getCircuitBody(), [['X', 'TY', 'TY'], ['TY']])
 
     # TY position LIST EXISTING CIRCUIT WITH SWAP
     def test_ty_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.ty([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'TY'), (1, 'TY'), (2, 'TY'), (3, 'TY')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['TY', 'TY', 'TY', 'TY']])
 
     # TY position ALL
     def test_ty_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.ty()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'TY'), (1, 'TY')])
         self.assertEqual(circuit.getCircuitBody(), [['TY', 'H'], [1, 'TY']])
 
     # TY position ALL BETWEEN SWAP
     def test_ty_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.ty()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'TY'), (1, 'TY'), (2, 'TY')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['TY', 'TY', 'TY']])
 
     # TY add
     def test_ty_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.ty(0, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'TY')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position LIST
+    def test_ty_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.ty([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_ty_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.ty([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_ty_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.ty('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_ty_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.ty([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_ty_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.ty(0, 'add')
             raise Exception
 
         except Exception as e:
@@ -3118,192 +3077,204 @@
 
 
 ##################_____I_TY_____##################
 class Test_I_TY(unittest.TestCase):
 
     # I_TY position 0
     def test_i_ty_position_0(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.i_ty(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_TY')])
         self.assertEqual(circuit.getCircuitBody(), [['I_TY']])
 
     # I_TY position 1
     def test_i_ty_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.i_ty(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'I_TY')])
         self.assertEqual(circuit.getCircuitBody(), [[1, 'I_TY']])
 
     # I_TY EXISTING CIRCUIT position NEW COLUMN
     def test_i_ty_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.i_ty(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_TY')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], ['I_TY']])
 
     # I_TY EXISTING CIRCUIT position SAME COLUMN
     def test_i_ty_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.i_ty(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'I_TY')])
         self.assertEqual(circuit.getCircuitBody(), [['H', 'I_TY']])
 
     # I_TY EXISTING CIRCUIT position BETWEEN SWAP
     def test_i_ty_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.i_ty(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'I_TY')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, 'I_TY']])
 
     # I_TY EXISTING CIRCUIT position UNDER SWAP
     def test_i_ty_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.i_ty(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, 'I_TY')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'I_TY']])
 
     # I_TY position LIST
     def test_i_ty_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.i_ty([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_TY'), (1, 'I_TY'), (2, 'I_TY')])
         self.assertEqual(circuit.getCircuitBody(), [['I_TY', 'H', 'I_TY'], [1, 'I_TY']])
     
     # I_TY position LIST EXISTING CIRCUIT
     def test_i_ty_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(0)
 
         gate = circuit.i_ty([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_TY'), (1, 'I_TY'), (2, 'I_TY')])
         self.assertEqual(circuit.getCircuitBody(), [['X', 'I_TY', 'I_TY'], ['I_TY']])
 
     # I_TY position LIST EXISTING CIRCUIT WITH SWAP
     def test_i_ty_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.i_ty([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_TY'), (1, 'I_TY'), (2, 'I_TY'), (3, 'I_TY')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['I_TY', 'I_TY', 'I_TY', 'I_TY']])
 
     # I_TY position ALL
     def test_i_ty_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.i_ty()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_TY'), (1, 'I_TY')])
         self.assertEqual(circuit.getCircuitBody(), [['I_TY', 'H'], [1, 'I_TY']])
 
     # I_TY position ALL BETWEEN SWAP
     def test_i_ty_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.i_ty()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_TY'), (1, 'I_TY'), (2, 'I_TY')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['I_TY', 'I_TY', 'I_TY']])
 
     # I_TY add
     def test_i_ty_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.i_ty(0, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'I_TY')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position LIST
+    def test_i_ty_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.i_ty([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_i_ty_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_ty([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_i_ty_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_ty('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_i_ty_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_ty([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_i_ty_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.i_ty(0, 'add')
             raise Exception
 
         except Exception as e:
@@ -3311,260 +3282,272 @@
 
 
 ##################_____P_____##################
 class Test_P(unittest.TestCase):
 
     # P position 0
     def test_p_position_0(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.p(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'P', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[{'id': 'P', 'arg': 'pi'}]])
 
     # P position 1
     def test_p_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.p(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'P', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'P', 'arg': 'pi'}]])
 
     # P argument INT
     def test_p_argument_int(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.p(1, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'P', 'arg': '2'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'P', 'arg': '2'}]])
 
     # P argument FLOAT
     def test_p_argument_float(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.p(1, 1.5)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'P', 'arg': '1.5'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'P', 'arg': '1.5'}]])
 
     # P argument STRING NUMBER
     def test_p_argument_string_number(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.p(1, '2')
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'P', 'arg': '2'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'P', 'arg': '2'}]])
 
     # P argument STRING EXPRESSION
     def test_p_argument_string_expression(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.p(1, 'pi/2')
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'P', 'arg': 'pi/2'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'P', 'arg': 'pi/2'}]])
 
     # P EXISTING CIRCUIT position NEW COLUMN
     def test_p_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.p(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'P', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['H'], [{'id': 'P', 'arg': 'pi'}]])
 
     # P EXISTING CIRCUIT position SAME COLUMN
     def test_p_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.p(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'P', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['H', {'id': 'P', 'arg': 'pi'}]])
 
     # P EXISTING CIRCUIT position BETWEEN SWAP
     def test_p_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.p(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'P', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, {'id': 'P', 'arg': 'pi'}]])
 
     # P EXISTING CIRCUIT position UNDER SWAP
     def test_p_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.p(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, {'id': 'P', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, {'id': 'P', 'arg': 'pi'}]])
 
     # P position LIST
     def test_p_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.p([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'P', 'arg': 'pi'}), (1, {'id': 'P', 'arg': 'pi'}), (2, {'id': 'P', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[{'arg': 'pi', 'id': 'P'}, 'H', {'arg': 'pi', 'id': 'P'}], [1, {'arg': 'pi', 'id': 'P'}]])
     
     # P position LIST EXISTING CIRCUIT
     def test_p_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(0)
 
         gate = circuit.p([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'P', 'arg': 'pi'}), (1, {'id': 'P', 'arg': 'pi'}), (2, {'id': 'P', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['X', {'id': 'P', 'arg': 'pi'}, {'id': 'P', 'arg': 'pi'}], [{'id': 'P', 'arg': 'pi'}]])
 
     # P position LIST EXISTING CIRCUIT WITH SWAP
     def test_p_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.p([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'P', 'arg': 'pi'}), (1, {'id': 'P', 'arg': 'pi'}), (2, {'id': 'P', 'arg': 'pi'}), (3, {'id': 'P', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [{'id': 'P', 'arg': 'pi'}, {'id': 'P', 'arg': 'pi'}, {'id': 'P', 'arg': 'pi'}, {'id': 'P', 'arg': 'pi'}]])
 
     # P position ALL
     def test_p_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.p()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'P', 'arg': 'pi'}), (1, {'id': 'P', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[{'arg': 'pi', 'id': 'P'}, 'H'], [1, {'arg': 'pi', 'id': 'P'}]])
 
     # P position ALL BETWEEN SWAP
     def test_p_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.p()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'P', 'arg': 'pi'}), (1, {'id': 'P', 'arg': 'pi'}), (2, {'id': 'P', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [{'id': 'P', 'arg': 'pi'}, {'id': 'P', 'arg': 'pi'}, {'id': 'P', 'arg': 'pi'}]])
 
     # P add
     def test_p_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.p(0, add=False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'P', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position LIST
+    def test_p_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.p([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_p_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.p([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT argument
     def test_p_badArgument_argument(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.p(1, argument='argument')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_p_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.p('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_p_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.p([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE argument
     def test_p_badArgumentType_argument(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.p(0, True)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_p_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.p(0, add='add')
             raise Exception
 
         except Exception as e:
@@ -3572,260 +3555,272 @@
 
 
 ##################_____RX_____##################
 class Test_RX(unittest.TestCase):
 
     # RX position 0
     def test_rx_position_0(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.rx(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RX', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[{'id': 'RX', 'arg': 'pi'}]])
 
     # RX position 1
     def test_rx_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.rx(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RX', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RX', 'arg': 'pi'}]])
 
     # RX argument INT
     def test_rx_argument_int(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.rx(1, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RX', 'arg': '2'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RX', 'arg': '2'}]])
 
     # RX argument FLOAT
     def test_rx_argument_float(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.rx(1, 1.5)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RX', 'arg': '1.5'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RX', 'arg': '1.5'}]])
 
     # RX argument STRING NUMBER
     def test_rx_argument_string_number(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.rx(1, '2')
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RX', 'arg': '2'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RX', 'arg': '2'}]])
 
     # RX argument STRING EXPRESSION
     def test_rx_argument_string_expression(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.rx(1, 'pi/2')
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RX', 'arg': 'pi/2'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RX', 'arg': 'pi/2'}]])
 
     # RX EXISTING CIRCUIT position NEW COLUMN
     def test_rx_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.rx(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RX', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['H'], [{'id': 'RX', 'arg': 'pi'}]])
 
     # RX EXISTING CIRCUIT position SAME COLUMN
     def test_rx_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.rx(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RX', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['H', {'id': 'RX', 'arg': 'pi'}]])
 
     # RX EXISTING CIRCUIT position BETWEEN SWAP
     def test_rx_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.rx(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RX', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, {'id': 'RX', 'arg': 'pi'}]])
 
     # RX EXISTING CIRCUIT position UNDER SWAP
     def test_rx_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.rx(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, {'id': 'RX', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, {'id': 'RX', 'arg': 'pi'}]])
 
     # RX position LIST
     def test_rx_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.rx([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RX', 'arg': 'pi'}), (1, {'id': 'RX', 'arg': 'pi'}), (2, {'id': 'RX', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[{'arg': 'pi', 'id': 'RX'}, 'H', {'arg': 'pi', 'id': 'RX'}], [1, {'arg': 'pi', 'id': 'RX'}]])
     
     # RX position LIST EXISTING CIRCUIT
     def test_rx_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(0)
 
         gate = circuit.rx([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RX', 'arg': 'pi'}), (1, {'id': 'RX', 'arg': 'pi'}), (2, {'id': 'RX', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['X', {'id': 'RX', 'arg': 'pi'}, {'id': 'RX', 'arg': 'pi'}], [{'id': 'RX', 'arg': 'pi'}]])
 
     # RX position LIST EXISTING CIRCUIT WITH SWAP
     def test_rx_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.rx([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RX', 'arg': 'pi'}), (1, {'id': 'RX', 'arg': 'pi'}), (2, {'id': 'RX', 'arg': 'pi'}), (3, {'id': 'RX', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [{'id': 'RX', 'arg': 'pi'}, {'id': 'RX', 'arg': 'pi'}, {'id': 'RX', 'arg': 'pi'}, {'id': 'RX', 'arg': 'pi'}]])
 
     # RX position ALL
     def test_rx_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.rx()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RX', 'arg': 'pi'}), (1, {'id': 'RX', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[{'arg': 'pi', 'id': 'RX'}, 'H'], [1, {'arg': 'pi', 'id': 'RX'}]])
 
     # RX position ALL BETWEEN SWAP
     def test_rx_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.rx() 
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RX', 'arg': 'pi'}), (1, {'id': 'RX', 'arg': 'pi'}), (2, {'id': 'RX', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [{'id': 'RX', 'arg': 'pi'}, {'id': 'RX', 'arg': 'pi'}, {'id': 'RX', 'arg': 'pi'}]])
 
     # RX add
     def test_rx_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.rx(0, add=False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RX', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position LIST
+    def test_rx_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.rx([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_rx_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.rx([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT argument
     def test_rx_badArgument_argument(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.rx(1, argument='argument')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_rx_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.rx('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_rx_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.rx([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE argument
     def test_rx_badArgumentType_argument(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.rx(0, True)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_rx_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.rx(0, add='add')
             raise Exception
 
         except Exception as e:
@@ -3833,260 +3828,272 @@
 
 
 ##################_____RY_____##################
 class Test_RY(unittest.TestCase):
 
     # RY position 0
     def test_ry_position_0(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.ry(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RY', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[{'id': 'RY', 'arg': 'pi'}]])
 
     # RY position 1
     def test_ry_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.ry(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RY', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RY', 'arg': 'pi'}]])
 
     # RY argument INT
     def test_ry_argument_int(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.ry(1, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RY', 'arg': '2'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RY', 'arg': '2'}]])
 
     # RY argument FLOAT
     def test_ry_argument_float(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.ry(1, 1.5)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RY', 'arg': '1.5'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RY', 'arg': '1.5'}]])
 
     # RY argument STRING NUMBER
     def test_ry_argument_string_number(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.ry(1, '2')
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RY', 'arg': '2'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RY', 'arg': '2'}]])
 
     # P argument STRING EXPRESSION
     def test_ry_argument_string_expression(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.ry(1, 'pi/2')
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RY', 'arg': 'pi/2'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RY', 'arg': 'pi/2'}]])
 
     # RY EXISTING CIRCUIT position NEW COLUMN
     def test_ry_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.ry(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RY', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['H'], [{'id': 'RY', 'arg': 'pi'}]])
 
     # RY EXISTING CIRCUIT position SAME COLUMN
     def test_ry_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.ry(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RY', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['H', {'id': 'RY', 'arg': 'pi'}]])
 
     # RY EXISTING CIRCUIT position BETWEEN SWAP
     def test_ry_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.ry(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RY', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, {'id': 'RY', 'arg': 'pi'}]])
 
     # RY EXISTING CIRCUIT position UNDER SWAP
     def test_ry_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.ry(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, {'id': 'RY', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, {'id': 'RY', 'arg': 'pi'}]])
 
     # RY position LIST
     def test_ry_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.ry([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RY', 'arg': 'pi'}), (1, {'id': 'RY', 'arg': 'pi'}), (2, {'id': 'RY', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[{'arg': 'pi', 'id': 'RY'}, 'H', {'arg': 'pi', 'id': 'RY'}], [1, {'arg': 'pi', 'id': 'RY'}]])
     
     # RY position LIST EXISTING CIRCUIT
     def test_ry_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(0)
 
         gate = circuit.ry([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RY', 'arg': 'pi'}), (1, {'id': 'RY', 'arg': 'pi'}), (2, {'id': 'RY', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['X', {'id': 'RY', 'arg': 'pi'}, {'id': 'RY', 'arg': 'pi'}], [{'id': 'RY', 'arg': 'pi'}]])
 
     # RY position LIST EXISTING CIRCUIT WITH SWAP
     def test_ry_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.ry([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RY', 'arg': 'pi'}), (1, {'id': 'RY', 'arg': 'pi'}), (2, {'id': 'RY', 'arg': 'pi'}), (3, {'id': 'RY', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [{'id': 'RY', 'arg': 'pi'}, {'id': 'RY', 'arg': 'pi'}, {'id': 'RY', 'arg': 'pi'}, {'id': 'RY', 'arg': 'pi'}]])
 
     # RY position ALL
     def test_ry_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.ry()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RY', 'arg': 'pi'}), (1, {'id': 'RY', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[{'arg': 'pi', 'id': 'RY'}, 'H'], [1, {'arg': 'pi', 'id': 'RY'}]])
 
     # RY position ALL BETWEEN SWAP
     def test_ry_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.ry() 
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RY', 'arg': 'pi'}), (1, {'id': 'RY', 'arg': 'pi'}), (2, {'id': 'RY', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [{'id': 'RY', 'arg': 'pi'}, {'id': 'RY', 'arg': 'pi'}, {'id': 'RY', 'arg': 'pi'}]])
 
     # RY add
     def test_ry_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.ry(0, add=False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RY', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position LIST
+    def test_ry_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.ry([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_ry_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.ry([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT argument
     def test_ry_badArgument_argument(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.ry(1, argument='argument')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_ry_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.ry('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_ry_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.ry([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE argument
     def test_ry_badArgumentType_argument(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.ry(0, True)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_ry_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.ry(0, add='add')
             raise Exception
 
         except Exception as e:
@@ -4094,260 +4101,272 @@
 
 
 ##################_____RZ_____##################
 class Test_RZ(unittest.TestCase):
 
     # RZ position_0
     def test_rz_position_0(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.rz(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RZ', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[{'id': 'RZ', 'arg': 'pi'}]])
 
     # RZ position 1
     def test_rz_position_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.rz(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RZ', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RZ', 'arg': 'pi'}]])
 
     # RZ argument INT
     def test_rz_argument_int(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.rz(1, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RZ', 'arg': '2'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RZ', 'arg': '2'}]])
 
     # RZ argument FLOAT
     def test_rz_argument_float(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.rz(1, 1.5)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RZ', 'arg': '1.5'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RZ', 'arg': '1.5'}]])
 
     # RZ argument STRING NUMBER
     def test_rz_argument_string_number(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.rz(1, '2')
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RZ', 'arg': '2'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RZ', 'arg': '2'}]])
 
     # P argument STRING EXPRESSION
     def test_rz_argument_string_expression(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.rz(1, 'pi/2')
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RZ', 'arg': 'pi/2'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RZ', 'arg': 'pi/2'}]])
 
     # RZ EXISTING CIRCUIT position NEW COLUMN
     def test_rz_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.rz(0)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RZ', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['H'], [{'id': 'RZ', 'arg': 'pi'}]])
 
     # RZ EXISTING CIRCUIT position SAME COLUMN
     def test_rz_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.rz(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RZ', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['H', {'id': 'RZ', 'arg': 'pi'}]])
 
     # RZ EXISTING CIRCUIT position BETWEEN SWAP
     def test_rz_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.rz(1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RZ', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, {'id': 'RZ', 'arg': 'pi'}]])
 
     # RZ EXISTING CIRCUIT position UNDER SWAP
     def test_rz_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.rz(2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, {'id': 'RZ', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, {'id': 'RZ', 'arg': 'pi'}]])
 
     # RZ position LIST
     def test_rz_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.rz([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RZ', 'arg': 'pi'}), (1, {'id': 'RZ', 'arg': 'pi'}), (2, {'id': 'RZ', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[{'arg': 'pi', 'id': 'RZ'}, 'H', {'arg': 'pi', 'id': 'RZ'}], [1, {'arg': 'pi', 'id': 'RZ'}]])
     
     # RZ position LIST EXISTING CIRCUIT
     def test_rz_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.x(0)
 
         gate = circuit.rz([0, 1, 2])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RZ', 'arg': 'pi'}), (1, {'id': 'RZ', 'arg': 'pi'}), (2, {'id': 'RZ', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['X', {'id': 'RZ', 'arg': 'pi'}, {'id': 'RZ', 'arg': 'pi'}], [{'id': 'RZ', 'arg': 'pi'}]])
 
     # RZ position LIST EXISTING CIRCUIT WITH SWAP
     def test_rz_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.rz([0, 1, 2, 3])
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RZ', 'arg': 'pi'}), (1, {'id': 'RZ', 'arg': 'pi'}), (2, {'id': 'RZ', 'arg': 'pi'}), (3, {'id': 'RZ', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [{'id': 'RZ', 'arg': 'pi'}, {'id': 'RZ', 'arg': 'pi'}, {'id': 'RZ', 'arg': 'pi'}, {'id': 'RZ', 'arg': 'pi'}]])
 
     # RZ position ALL
     def test_rz_position_all(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(1)
 
         gate = circuit.rz()
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RZ', 'arg': 'pi'}), (1, {'id': 'RZ', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[{'arg': 'pi', 'id': 'RZ'}, 'H'], [1, {'arg': 'pi', 'id': 'RZ'}]])
 
     # RZ position ALL BETWEEN SWAP
     def test_rz_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 2)
 
         gate = circuit.rz() 
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RZ', 'arg': 'pi'}), (1, {'id': 'RZ', 'arg': 'pi'}), (2, {'id': 'RZ', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [{'id': 'RZ', 'arg': 'pi'}, {'id': 'RZ', 'arg': 'pi'}, {'id': 'RZ', 'arg': 'pi'}]])
 
     # RZ add
     def test_rz_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.rz(0, add=False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, {'id': 'RZ', 'arg': 'pi'})])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
+    # BAD ARGUMENT position LIST
+    def test_rz_badArgument_position_list(self):
+        qsoa = QSOAPlatform(configFile=True)
+        circuit = qsoa.CircuitGates()
+
+        try:
+            circuit.rz([])
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, ValueError)
+
     # BAD ARGUMENT position LIST DUPLICATED
     def test_rz_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.rz([0, 0])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT argument
     def test_rz_badArgument_argument(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.rz(1, argument='argument')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE position
     def test_rz_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.rz('position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position LIST
     def test_rz_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.rz([0, 'position'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE argument
     def test_rz_badArgumentType_argument(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.rz(0, True)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_rz_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.rz(0, add='add')
             raise Exception
 
         except Exception as e:
@@ -4355,131 +4374,131 @@
 
 
 ##################_____SWAP_____##################
 class Test_Swap(unittest.TestCase):
 
     # SWAP position 0, 1
     def test_swap_position_0_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.swap(0, 1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'Swap'), (1, 'Swap')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap']])
 
     # SWAP position 0, 2
     def test_swap_position_0_2(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.swap(0, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'Swap'), (2, 'Swap')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap']])
 
     # SWAP position 1, 2
     def test_swap_position_position_1_2(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.swap(1, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'Swap'), (2, 'Swap')])
         self.assertEqual(circuit.getCircuitBody(), [[1, 'Swap', 'Swap']])
 
     # SWAP EXISTING CIRCUIT position NEW COLUMN
     def test_swap_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.swap(0, 1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'Swap'), (1, 'Swap')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], ['Swap', 'Swap']])
 
     # SWAP EXISTING CIRCUIT position SAME COLUMN
     def test_swap_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.swap(1, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'Swap'), (2, 'Swap')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], [1, 'Swap', 'Swap']])
 
     # SWAP EXISTING CIRCUIT position BETWEEN SWAP
     def test_swap_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 3)
 
         gate = circuit.swap(1, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'Swap'), (2, 'Swap')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 1, 'Swap'], [1, 'Swap', 'Swap']])
 
     # SWAP EXISTING CIRCUIT position UNDER SWAP
     def test_swap_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.swap(2, 3)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, 'Swap'), (3, 'Swap')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'Swap', 'Swap']])
 
     # SWAP add
     def test_swap_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.swap(1, 3, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'Swap'), (3, 'Swap')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
     # BAD ARGUMENT TYPE position1
     def test_swap_badArgumentType_position1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.swap('position', 3)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position2
     def test_swap_badArgumentType_position2(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.swap(1, 'position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_swap_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.swap(1, 3, 'add')
             raise Exception
 
         except Exception as e:
@@ -4487,131 +4506,131 @@
 
 
 ##################_____CH_____##################
 class Test_CH(unittest.TestCase):
 
     # CH position 0, 1
     def test_ch_0_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.ch(0, 1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'CTRL'), (1, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [['CTRL', 'H']])
 
     # CH position 0, 2
     def test_ch_position_0_2(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.ch(0, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'CTRL'), (2, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [['CTRL', 1, 'H']])
 
     # CH position 1, 2
     def test_ch_position_position_1_2(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.ch(1, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'CTRL'), (2, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [[1, 'CTRL', 'H']])
 
     # CH EXISTING CIRCUIT position NEW COLUMN
     def test_ch_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.ch(0, 1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'CTRL'), (1, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], ['CTRL', 'H']])
 
     # CH EXISTING CIRCUIT position SAME COLUMN
     def test_ch_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.ch(1, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'CTRL'), (2, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], [1, 'CTRL', 'H']])
 
     # CH EXISTING CIRCUIT position BETWEEN SWAP
     def test_ch_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 3)
 
         gate = circuit.ch(1, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'CTRL'), (2, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 1, 'Swap'], [1, 'CTRL', 'H']])
 
     # CH EXISTING CIRCUIT position UNDER SWAP
     def test_ch_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.ch(2, 3)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, 'CTRL'), (3, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'CTRL', 'H']])
 
     # CH add
     def test_ch_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.ch(1, 3, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'CTRL'), (3, 'H')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
     # BAD ARGUMENT TYPE position1
     def test_ch_badArgumentType_position1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.ch('position', 3)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position2
     def test_ch_badArgumentType_position2(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.ch(1, 'position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_ch_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.ch(1, 3, 'add')
             raise Exception
 
         except Exception as e:
@@ -4619,1105 +4638,136 @@
 
 
 ##################_____CX_____##################
 class Test_CX(unittest.TestCase):
 
     # CX position 0, 1
     def test_cx_position_0_1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.cx(0, 1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'CTRL'), (1, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [['CTRL', 'X']])
 
     # CX position 0, 2
     def test_cx_position_0_2(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.cx(0, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'CTRL'), (2, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [['CTRL', 1, 'X']])
 
     # CX position 1, 2
     def test_cx_position_position_1_2(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.cx(1, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'CTRL'), (2, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [[1, 'CTRL', 'X']])
 
     # CX EXISTING CIRCUIT position NEW COLUMN
     def test_cx_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.cx(0, 1)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(0, 'CTRL'), (1, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], ['CTRL', 'X']])
 
     # CX EXISTING CIRCUIT position SAME COLUMN
     def test_cx_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.h(0)
 
         gate = circuit.cx(1, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'CTRL'), (2, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [['H'], [1, 'CTRL', 'X']])
 
     # CX EXISTING CIRCUIT position BETWEEN SWAP
     def test_cx_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 3)
 
         gate = circuit.cx(1, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'CTRL'), (2, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 1, 'Swap'], [1, 'CTRL', 'X']])
 
     # CX EXISTING CIRCUIT position UNDER SWAP
     def test_cx_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
         circuit.swap(0, 1)
 
         gate = circuit.cx(2, 3)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(2, 'CTRL'), (3, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'CTRL', 'X']])
 
     # CX add
     def test_cx_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         gate = circuit.cx(1, 3, False)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, 'CTRL'), (3, 'X')])
         self.assertEqual(circuit.getCircuitBody(), [[]])
 
     # BAD ARGUMENT TYPE position1
     def test_cx_badArgumentType_position1(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.cx('position', 3)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE position2
     def test_cx_badArgumentType_position2(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.cx(1, 'position')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE add
     def test_cx_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
+        qsoa = QSOAPlatform(configFile=True)
         circuit = qsoa.CircuitGates()
 
         try:
             circuit.cx(1, 3, 'add')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
 
-##################_____CCX_____##################
-class Test_CCX(unittest.TestCase):
-
-    # CCX position 0, 1, 2
-    def test_ccx_position_0_1_2(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        gate = circuit.ccx(0, 1, 2)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, 'CTRL'), (1, 'CTRL'), (2, 'X')])
-        self.assertEqual(circuit.getCircuitBody(), [['CTRL', 'CTRL', 'X']])
-
-    # CCX position 0, 1, 3
-    def test_ccx_position_0_1_3(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        gate = circuit.ccx(0, 1, 3)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, 'CTRL'), (1, 'CTRL'), (3, 'X')])
-        self.assertEqual(circuit.getCircuitBody(), [['CTRL', 'CTRL', 1, 'X']])
-
-    # CCX position 1, 2, 3
-    def test_ccx_position_position_1_2_3(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        gate = circuit.ccx(1, 2, 3)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(1, 'CTRL'), (2, 'CTRL'), (3, 'X')])
-        self.assertEqual(circuit.getCircuitBody(), [[1, 'CTRL', 'CTRL', 'X']])
-
-    # CCX EXISTING CIRCUIT position NEW COLUMN
-    def test_ccx_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(0)
-
-        gate = circuit.ccx(0, 1, 2)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, 'CTRL'), (1, 'CTRL'), (2, 'X')])
-        self.assertEqual(circuit.getCircuitBody(), [['H'], ['CTRL', 'CTRL', 'X']])
-
-    # CCX EXISTING CIRCUIT position SAME COLUMN
-    def test_ccx_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(0)
-
-        gate = circuit.ccx(1, 2, 3)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(1, 'CTRL'), (2, 'CTRL'), (3, 'X')])
-        self.assertEqual(circuit.getCircuitBody(), [['H'], [1, 'CTRL', 'CTRL', 'X']])
-
-    # CCX EXISTING CIRCUIT position BETWEEN SWAP
-    def test_ccx_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 4)
-
-        gate = circuit.ccx(1, 2, 3)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(1, 'CTRL'), (2, 'CTRL'), (3, 'X')])
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 1, 1, 'Swap'], [1, 'CTRL', 'CTRL', 'X']])
-
-    # CCX EXISTING CIRCUIT position UNDER SWAP
-    def test_ccx_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 1)
-
-        gate = circuit.ccx(2, 3, 4)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(2, 'CTRL'), (3, 'CTRL'), (4, 'X')])
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'CTRL', 'CTRL', 'X']])
-
-    # CCX add
-    def test_ccx_add(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        gate = circuit.ccx(1, 2, 3, False)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(1, 'CTRL'), (2, 'CTRL'), (3, 'X')])
-        self.assertEqual(circuit.getCircuitBody(), [[]])
-
-    # BAD ARGUMENT TYPE position1
-    def test_ccx_badArgumentType_position1(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.ccx('position', 2, 3)
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-    # BAD ARGUMENT TYPE position2
-    def test_ccx_badArgumentType_position2(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.ccx(1, 'position', 3)
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-    # BAD ARGUMENT TYPE position3
-    def test_ccx_badArgumentType_position3(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.ccx(1, 2, 'position')
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-    # BAD ARGUMENT TYPE add
-    def test_ccx_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.ccx(1, 2, 3, 'add')
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-
-##################_____MEASURE_____##################
-class Test_Measure(unittest.TestCase):
-
-    # MEASURE position 0
-    def test_measure_position_0(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        gate = circuit.measure(0)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, 'Measure')])
-        self.assertEqual(circuit.getCircuitBody(), [['Measure']])
-
-    # MEASURE EXISTING CIRCUIT position NEW COLUMN
-    def test_measure_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(0)
-
-        gate = circuit.measure(0)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, 'Measure')])
-        self.assertEqual(circuit.getCircuitBody(), [['H'], ['Measure']])
-
-    # MEASURE EXISTING CIRCUIT position SAME COLUMN
-    def test_measure_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(0)
-
-        gate = circuit.measure(1)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(1, 'Measure')])
-        self.assertEqual(circuit.getCircuitBody(), [['H'], [1, 'Measure']])
-
-    # MEASURE EXISTING CIRCUIT position BETWEEN SWAP
-    def test_measure_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 2)
-
-        gate = circuit.measure(1)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(1, 'Measure')])
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, 'Measure']])
-
-    # MEASURE EXISTING CIRCUIT position UNDER SWAP
-    def test_measure_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 1)
-
-        gate = circuit.measure(2)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(2, 'Measure')])
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'Measure']])
-
-    # MEASURE position LIST
-    def test_measure_position_list(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(1)
-
-        gate = circuit.measure([0, 1, 2])
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, 'Measure'), (1, 'Measure'), (2, 'Measure')])
-        self.assertEqual(circuit.getCircuitBody(), [[1, 'H'], ['Measure', 'Measure', 'Measure']])
-    
-    # MEASURE position LIST EXISTING CIRCUIT
-    def test_measure_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.x(0)
-
-        gate = circuit.measure([0, 1, 2])
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, 'Measure'), (1, 'Measure'), (2, 'Measure')])
-        self.assertEqual(circuit.getCircuitBody(), [['X'], ['Measure', 'Measure', 'Measure']])
-
-    # MEASURE position LIST EXISTING CIRCUIT WITH SWAP
-    def test_measure_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 2)
-
-        gate = circuit.measure([0, 1, 2, 3])
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, 'Measure'), (1, 'Measure'), (2, 'Measure'), (3, 'Measure')])
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['Measure', 'Measure', 'Measure', 'Measure']])
-
-    # MEASURE position ALL
-    def test_measure_position_all(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(1)
-
-        gate = circuit.measure()
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, 'Measure'), (1, 'Measure')])
-        self.assertEqual(circuit.getCircuitBody(), [[1, 'H'], ['Measure', 'Measure']])
-
-    # MEASURE position ALL BETWEEN SWAP
-    def test_measure_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 2)
-
-        gate = circuit.measure()
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, 'Measure'), (1, 'Measure'), (2, 'Measure')])
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['Measure', 'Measure', 'Measure']])
-    
-    # BAD ARGUMENT position LIST DUPLICATED
-    def test_measure_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.measure([0, 0])
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, ValueError)
-
-    # BAD ARGUMENT TYPE position
-    def test_measure_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.measure('position')
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-    # BAD ARGUMENT TYPE position LIST
-    def test_measure_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.measure([0, 'position'])
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-
-##################_____BARRIER_____##################
-class Test_Barrier(unittest.TestCase):
-
-    # BARRIER position 0
-    def test_barrier_position_0(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        gate = circuit.barrier(0)
-
-        self.assertIsNone(gate)
-        self.assertEqual(circuit.getCircuitBody(), [['SPACER']])
-
-    # BARRIER EXISTING CIRCUIT position NEW COLUMN
-    def test_barrier_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(0)
-
-        gate = circuit.barrier(0)
-
-        self.assertIsNone(gate)
-        self.assertEqual(circuit.getCircuitBody(), [['H'], ['SPACER']])
-
-    # BARRIER EXISTING CIRCUIT position SAME COLUMN
-    def test_barrier_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(0)
-
-        gate = circuit.barrier(1)
-
-        self.assertIsNone(gate)
-        self.assertEqual(circuit.getCircuitBody(), [['H', 'SPACER']])
-
-    # BARRIER EXISTING CIRCUIT position BETWEEN SWAP
-    def test_barrier_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 2)
-
-        gate = circuit.barrier(1)
-
-        self.assertIsNone(gate)
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, 'SPACER']])
-
-    # BARRIER EXISTING CIRCUIT position UNDER SWAP
-    def test_barrier_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 1)
-
-        gate = circuit.barrier(2)
-
-        self.assertIsNone(gate)
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'SPACER']])
-
-    # BARRIER position LIST
-    def test_barrier_position_list(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(1)
-
-        gate = circuit.barrier([0, 1, 2])
-
-        self.assertIsNone(gate)
-        self.assertEqual(circuit.getCircuitBody(), [['SPACER', 'H', 'SPACER'], [1, 'SPACER']])
-    
-    # BARRIER position LIST EXISTING CIRCUIT
-    def test_barrier_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.x(0)
-
-        gate = circuit.barrier([0, 1, 2])
-
-        self.assertIsNone(gate)
-        self.assertEqual(circuit.getCircuitBody(), [['X', 'SPACER', 'SPACER'], ['SPACER']])
-
-    # BARRIER position LIST EXISTING CIRCUIT WITH SWAP
-    def test_barrier_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 2)
-
-        gate = circuit.barrier([0, 1, 2, 3])
-
-        self.assertIsNone(gate)
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['SPACER', 'SPACER', 'SPACER', 'SPACER']])
-
-    # BARRIER position ALL
-    def test_barrier_position_all(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(1)
-
-        gate = circuit.barrier()
-
-        self.assertIsNone(gate)
-        self.assertEqual(circuit.getCircuitBody(), [[1, 'H'], ['SPACER', 'SPACER']])
-
-    # BARRIER position ALL BETWEEN SWAP
-    def test_barrier_position_all_betweenSwap(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 2)
-
-        gate = circuit.barrier()
-
-        self.assertIsNone(gate)
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['SPACER', 'SPACER', 'SPACER']])
-
-    # BAD ARGUMENT position LIST DUPLICATED
-    def test_barrier_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.barrier([0, 0])
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, ValueError)
-
-    # BAD ARGUMENT TYPE position
-    def test_barrier_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.barrier('position')
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-    # BAD ARGUMENT TYPE position LIST
-    def test_barrier_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.barrier([0, 'position'])
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-
-##################_____BEGIN REPEAT_____##################
-class Test_BeginRepeat(unittest.TestCase):
-
-    # BEGIN REPEAT position 0
-    def test_beginRepeat_position_0(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        gate = circuit.beginRepeat(0, 2)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, {'id': 'BEGIN_R', 'arg': '2'})])
-        self.assertEqual(circuit.getCircuitBody(), [[{'arg': '2', 'id': 'BEGIN_R'}]])
-
-    # BEGIN REPEAT EXISTING CIRCUIT position NEW COLUMN
-    def test_beginRepeat_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(0)
-
-        gate = circuit.beginRepeat(0, 2)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, {'id': 'BEGIN_R', 'arg': '2'})])
-        self.assertEqual(circuit.getCircuitBody(), [['H'], [{'id': 'BEGIN_R', 'arg': '2'}]])
-
-    # BEGIN REPEAT EXISTING CIRCUIT position SAME COLUMN
-    def test_beginRepeat_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(0)
-
-        gate = circuit.beginRepeat(1, 2)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(1, {'id': 'BEGIN_R', 'arg': '2'})])
-        self.assertEqual(circuit.getCircuitBody(), [['H'], [1, {'arg': '2', 'id': 'BEGIN_R'}]])
-
-    # BEGIN REPEAT EXISTING CIRCUIT position BETWEEN SWAP
-    def test_beginRepeat_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 2)
-
-        gate = circuit.beginRepeat(1, 2)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(1, {'id': 'BEGIN_R', 'arg': '2'})])
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, {'id': 'BEGIN_R', 'arg': '2'}]])
-
-    # BEGIN REPEAT EXISTING CIRCUIT position UNDER SWAP
-    def test_beginRepeat_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 1)
-
-        gate = circuit.beginRepeat(2, 2)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(2, {'id': 'BEGIN_R', 'arg': '2'})])
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, {'id': 'BEGIN_R', 'arg': '2'}]])
-
-    # BEGIN REPEAT position LIST
-    def test_beginRepeat_position_list(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(1)
-
-        gate = circuit.beginRepeat([0, 1], 2)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, {'id': 'BEGIN_R', 'arg': '2'}), (1, {'id': 'BEGIN_R', 'arg': '2'})])
-        self.assertEqual(circuit.getCircuitBody(), [[1, 'H'], [{'id': 'BEGIN_R', 'arg': '2'}, {'id': 'BEGIN_R', 'arg': '2'}]])
-
-    # BEGIN REPEAT position LIST EXISTING CIRCUIT
-    def test_beginRepeat_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.x(0)
-
-        gate = circuit.beginRepeat([0, 1, 2], 2)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, {'id': 'BEGIN_R', 'arg': '2'}), (1, {'id': 'BEGIN_R', 'arg': '2'}), (2, {'id': 'BEGIN_R', 'arg': '2'})])
-        self.assertEqual(circuit.getCircuitBody(), [['X'], [{'arg': '2', 'id': 'BEGIN_R'}, {'arg': '2', 'id': 'BEGIN_R'}, {'arg': '2', 'id': 'BEGIN_R'}]])
-
-    # BEGIN REPEAT position LIST EXISTING CIRCUIT WITH SWAP
-    def test_beginRepeat_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 2)
-
-        gate = circuit.beginRepeat([0, 1, 2, 3], 2)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, {'id': 'BEGIN_R', 'arg': '2'}), (1, {'id': 'BEGIN_R', 'arg': '2'}), (2, {'id': 'BEGIN_R', 'arg': '2'}), (3, {'id': 'BEGIN_R', 'arg': '2'})])
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [{'id': 'BEGIN_R', 'arg': '2'}, {'id': 'BEGIN_R', 'arg': '2'}, {'id': 'BEGIN_R', 'arg': '2'}, {'id': 'BEGIN_R', 'arg': '2'}]])
-
-    # BAD ARGUMENT position LIST DUPLICATED
-    def test_beginRepeat_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.beginRepeat([0, 0], 2)
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, ValueError)
-
-    # BAD ARGUMENT TYPE position
-    def test_beginRepeat_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.beginRepeat('position', 2)
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-    # BAD ARGUMENT TYPE position LIST
-    def test_beginRepeat_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.beginRepeat([0, 'position'], 2)
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-    # BAD ARGUMENT TYPE repetitions
-    def test_beginRepeat_badArgumentType_argument(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.beginRepeat(0, 'repetitions')
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-
-##################_____END REPEAT_____##################
-class Test_EndRepeat(unittest.TestCase):
-
-    # END REPEAT position 0
-    def test_endRepeat_position_0(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        gate = circuit.endRepeat(0)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, 'END_R')])
-        self.assertEqual(circuit.getCircuitBody(), [['END_R']])
-
-    # END REPEAT EXISTING CIRCUIT position NEW COLUMN
-    def test_endRepeat_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(0)
-
-        gate = circuit.endRepeat(0)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, 'END_R')])
-        self.assertEqual(circuit.getCircuitBody(), [['H'], ['END_R']])
-
-    # END REPEAT EXISTING CIRCUIT position SAME COLUMN
-    def test_endRepeat_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(0)
-
-        gate = circuit.endRepeat(1)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(1, 'END_R')])
-        self.assertEqual(circuit.getCircuitBody(), [['H'], [1, 'END_R']])
-
-    # END REPEAT EXISTING CIRCUIT position BETWEEN SWAP
-    def test_endRepeat_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 2)
-
-        gate = circuit.endRepeat(1)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(1, 'END_R')])
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], [1, 'END_R']])
-
-    # END REPEAT EXISTING CIRCUIT position UNDER SWAP
-    def test_endRepeat_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 1)
-
-        gate = circuit.endRepeat(2)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(2, 'END_R')])
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'END_R']])
-
-    # END REPEAT position LIST
-    def test_endRepeat_position_list(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(1)
-
-        gate = circuit.endRepeat([0, 1, 2])
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, 'END_R'), (1, 'END_R'), (2, 'END_R')])
-        self.assertEqual(circuit.getCircuitBody(), [[1, 'H'], ['END_R', 'END_R', 'END_R']])
-
-    # END REPEAT position LIST EXISTING CIRCUIT
-    def test_endRepeat_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.x(0)
-
-        gate = circuit.endRepeat([0, 1, 2])
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, 'END_R'), (1, 'END_R'), (2, 'END_R')])
-        self.assertEqual(circuit.getCircuitBody(), [['X'], ['END_R', 'END_R', 'END_R']])
-
-    # END REPEAT position LIST EXISTING CIRCUIT WITH SWAP
-    def test_endRepeat_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 2)
-
-        gate = circuit.endRepeat([0, 1, 2, 3])
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(0, 'END_R'), (1, 'END_R'), (2, 'END_R'), (3, 'END_R')])
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['END_R', 'END_R', 'END_R', 'END_R']])
-
-    # BAD ARGUMENT position LIST DUPLICATED
-    def test_endRepeat_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.endRepeat([0, 0])
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, ValueError)
-
-    # BAD ARGUMENT TYPE position
-    def test_endRepeat_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.endRepeat('position')
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-    # BAD ARGUMENT TYPE position LIST
-    def test_endRepeat_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.endRepeat([0, 'position'])
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-
-##################_____CONTROL_____##################
-class Test_Control(unittest.TestCase):
-
-    # CONTROL position 0
-    def test_control_position_0(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        cx = circuit.control(0, circuit.x(1, False))
-        circuit.addCreatedGate(cx)
-
-        self.assertEqual(cx, [(1, 'X'), (0, 'CTRL')])
-        self.assertEqual(circuit.getCircuitBody(), [['CTRL', 'X']])
-
-    # BAD ARGUMENT TYPE position
-    def test_control_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            cx = circuit.control('position', circuit.h(0, False))
-            circuit.addCreatedGate(cx)
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-    # BAD ARGUMENT TYPE circuit
-    def test_control_badArgumentType_circuit(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.control(0, 'circuit')
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-
-##################_____ADD CREATED GATE_____##################
-class Test_AddCreatedGate(unittest.TestCase):
-
-    # ADD CREATED GATE position 0
-    def test_addCreatedGate_position_0(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        cx = circuit.control(0, circuit.x(1, False))
-        circuit.addCreatedGate(cx)
-
-        self.assertEqual(circuit.getCircuitBody(), [['CTRL', 'X']])
-
-    # BAD ARGUMENT TYPE gate
-    def test_addCreatedGate_badArgumentType_gate(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.addCreatedGate('gate')
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-
-##################_____MULTI CONTROL GATE_____##################
-class Test_MCG(unittest.TestCase):
-
-    # MCG position 0
-    def test_mcg_position_0(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        gate = circuit.mcg(0, circuit.x(1, False))
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(1, 'X'), (0, 'CTRL')])
-        self.assertEqual(circuit.getCircuitBody(), [['CTRL', 'X']])
-
-    # MCG EXISTING CIRCUIT position NEW COLUMN
-    def test_mcg_existingCircuit_position_newColumn(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(0)
-
-        gate = circuit.mcg(0, circuit.x(1, False))
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(1, 'X'), (0, 'CTRL')])
-        self.assertEqual(circuit.getCircuitBody(), [['H'], ['CTRL', 'X']])
-
-    # MCG EXISTING CIRCUIT position SAME COLUMN
-    def test_mcg_existingCircuit_position_sameColumn(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(0)
-
-        gate = circuit.mcg(1, circuit.x(2, False))
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(2, 'X'), (1, 'CTRL')])
-        self.assertEqual(circuit.getCircuitBody(), [['H'], [1, 'CTRL', 'X']])
-
-    # MCG EXISTING CIRCUIT position BETWEEN SWAP
-    def test_mcg_existingCircuit_position_betweenSwap(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 3)
-
-        gate = circuit.mcg(1, circuit.x(2, False))
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(2, 'X'), (1, 'CTRL')])
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 1, 'Swap'], [1, 'CTRL', 'X']])
-
-    # MCG EXISTING CIRCUIT position UNDER SWAP
-    def test_mcg_existingCircuit_position_underSwap(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 1)
-
-        gate = circuit.mcg(2, circuit.x(3, False))
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(3, 'X'), (2, 'CTRL')])
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 'Swap'], [1, 1, 'CTRL', 'X']])
-
-    # MCG position LIST
-    def test_mcg_position_list(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.h(1)
-
-        gate = circuit.mcg([0, 2], circuit.x(3, False))
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(3, 'X'), (0, 'CTRL'), (2, 'CTRL')])
-        self.assertEqual(circuit.getCircuitBody(), [[1, 'H'], ['CTRL', 1, 'CTRL', 'X']])
-
-    # MCG position LIST EXISTING CIRCUIT
-    def test_mcg_position_list_existingCircuit(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.x(0)
-
-        gate = circuit.mcg([0, 1], circuit.x(2, False))
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(2, 'X'), (0, 'CTRL'), (1, 'CTRL')])
-        self.assertEqual(circuit.getCircuitBody(), [['X'], ['CTRL', 'CTRL', 'X']])
-
-    # MCG position LIST EXISTING CIRCUIT WITH SWAP
-    def test_mcg_position_list_existingCircuit_swap(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-        circuit.swap(0, 2)
-
-        gate = circuit.mcg([0, 1], circuit.x(2, False))
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(2, 'X'), (0, 'CTRL'), (1, 'CTRL')])
-        self.assertEqual(circuit.getCircuitBody(), [['Swap', 1, 'Swap'], ['CTRL', 'CTRL', 'X']])
-
-    # MCG add
-    def test_mcg_add(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        gate = circuit.mcg([0, 2], circuit.x(3, False), False)
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(3, 'X'), (0, 'CTRL'), (2, 'CTRL')])
-        self.assertEqual(circuit.getCircuitBody(), [[]])
-
-    # BAD ARGUMENT position LIST DUPLICATED
-    def test_mcg_badArgument_position_list_duplicated(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.mcg([0, 0], circuit.x(3))
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, ValueError)
-
-    # BAD ARGUMENT circuit
-    def test_mcg_badArgument_circuit(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        gate = circuit.mcg(1, circuit.x(3))
-
-        self.assertIsInstance(gate, list)
-        self.assertEqual(gate, [(3, 'X'), (1, 'CTRL')])
-        self.assertNotEqual(circuit.getCircuitBody(), [[1, 'CTRL', 1, 'X']])
-
-    # BAD ARGUMENT TYPE position
-    def test_mcg_badArgumentType_position(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.mcg('position', circuit.x(3, False))
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-    # BAD ARGUMENT TYPE position LIST
-    def test_mcg_badArgumentType_position_list(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.mcg([0, 'position'], circuit.x(3, False))
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-    # BAD ARGUMENT TYPE add
-    def test_mcg_badArgumentType_add(self):
-        qsoa = QSOAPlatform()
-        circuit = qsoa.CircuitGates()
-
-        try:
-            circuit.mcg([0, 2], circuit.x(3, False), 'add')
-            raise Exception
-
-        except Exception as e:
-            self.assertIsInstance(e, TypeError)
-
-
 if __name__ == '__main__':
     unittest.main()
```

