# Comparing `tmp/th2_grpc_sim-5.0.0.dev5376623916.tar.gz` & `tmp/th2_grpc_sim-5.0.0.dev5377566930.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_sim-5.0.0.dev5376623916.tar", last modified: Mon Jun 26 09:43:26 2023, max compression
+gzip compressed data, was "dist/th2_grpc_sim-5.0.0.dev5377566930.tar", last modified: Mon Jun 26 11:26:53 2023, max compression
```

## Comparing `th2_grpc_sim-5.0.0.dev5376623916.tar` & `th2_grpc_sim-5.0.0.dev5377566930.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/
--rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1914 2023-06-26 09:42:34.000000 th2_grpc_sim-5.0.0.dev5376623916/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-26 09:42:35.000000 th2_grpc_sim-5.0.0.dev5376623916/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4549 2023-06-26 09:42:34.000000 th2_grpc_sim-5.0.0.dev5376623916/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-06-26 09:42:34.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     4355 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     7291 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-26 09:43:06.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim_service.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      391 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-06-26 09:43:26.000000 th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:26:53.000000 th2_grpc_sim-5.0.0.dev5377566930/
+-rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-06-26 11:26:53.000000 th2_grpc_sim-5.0.0.dev5377566930/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1914 2023-06-26 11:25:56.000000 th2_grpc_sim-5.0.0.dev5377566930/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-26 11:25:56.000000 th2_grpc_sim-5.0.0.dev5377566930/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 11:26:53.000000 th2_grpc_sim-5.0.0.dev5377566930/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4549 2023-06-26 11:25:56.000000 th2_grpc_sim-5.0.0.dev5377566930/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:26:53.000000 th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 11:26:53.000000 th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 11:26:53.000000 th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-06-26 11:25:56.000000 th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim/sim.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-06-26 11:26:53.000000 th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim/sim_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4355 2023-06-26 11:26:53.000000 th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim/sim_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     7291 2023-06-26 11:26:53.000000 th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim/sim_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-26 11:26:29.000000 th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim/sim_service.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 11:26:53.000000 th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-06-26 11:26:53.000000 th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      391 2023-06-26 11:26:53.000000 th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 11:26:53.000000 th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-26 11:26:53.000000 th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-06-26 11:26:53.000000 th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim.egg-info/top_level.txt
```

### Comparing `th2_grpc_sim-5.0.0.dev5376623916/PKG-INFO` & `th2_grpc_sim-5.0.0.dev5377566930/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_grpc_sim
-Version: 5.0.0.dev5376623916
+Version: 5.0.0.dev5377566930
 Summary: th2_grpc_sim
 Home-page: https://github.com/th2-net/th2-grpc-sim
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC sim library
```

### Comparing `th2_grpc_sim-5.0.0.dev5376623916/README.md` & `th2_grpc_sim-5.0.0.dev5377566930/README.md`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-5.0.0.dev5376623916/setup.py` & `th2_grpc_sim-5.0.0.dev5377566930/setup.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim.proto` & `th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim/sim.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim_pb2.py` & `th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim/sim_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim_pb2.pyi` & `th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim/sim_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim_pb2_grpc.py` & `th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim/sim_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim/sim_service.py` & `th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim/sim_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_sim-5.0.0.dev5376623916/th2_grpc_sim.egg-info/PKG-INFO` & `th2_grpc_sim-5.0.0.dev5377566930/th2_grpc_sim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-grpc-sim
-Version: 5.0.0.dev5376623916
+Version: 5.0.0.dev5377566930
 Summary: th2_grpc_sim
 Home-page: https://github.com/th2-net/th2-grpc-sim
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC sim library
```

