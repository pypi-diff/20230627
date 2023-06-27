# Comparing `tmp/connectome-0.6.1.tar.gz` & `tmp/connectome-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome-0.6.1.tar", last modified: Wed May 17 15:01:47 2023, max compression
+gzip compressed data, was "connectome-0.7.0.tar", last modified: Tue Jun 27 13:35:59 2023, max compression
```

## Comparing `connectome-0.6.1.tar` & `connectome-0.7.0.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:01:47.416990 connectome-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-05-17 15:01:42.000000 connectome-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-17 15:01:42.000000 connectome-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-17 15:01:47.416990 connectome-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-17 15:01:42.000000 connectome-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:01:47.412990 connectome-0.6.1/connectome/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:01:47.412990 connectome-0.6.1/connectome/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/cache/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/cache/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:01:47.412990 connectome-0.6.1/connectome/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/containers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/containers/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/containers/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/containers/reversible.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:01:47.412990 connectome-0.6.1/connectome/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/engine/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/engine/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/engine/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/engine/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/engine/node_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/engine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/engine/vm.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:01:47.416990 connectome-0.6.1/connectome/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/complex_edges.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/factory_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/metaclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/interface/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:01:47.416990 connectome-0.6.1/connectome/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/join.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/layers/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-17 15:01:42.000000 connectome-0.6.1/connectome/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:01:47.412990 connectome-0.6.1/connectome.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-17 15:01:47.000000 connectome-0.6.1/connectome.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-17 15:01:47.000000 connectome-0.6.1/connectome.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:01:47.000000 connectome-0.6.1/connectome.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-17 15:01:47.000000 connectome-0.6.1/connectome.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 15:01:47.000000 connectome-0.6.1/connectome.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-17 15:01:42.000000 connectome-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-17 15:01:42.000000 connectome-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 15:01:47.416990 connectome-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-17 15:01:42.000000 connectome-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:35:59.509663 connectome-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-06-27 13:35:52.000000 connectome-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-27 13:35:52.000000 connectome-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-06-27 13:35:59.509663 connectome-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-27 13:35:52.000000 connectome-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:35:59.497662 connectome-0.7.0/connectome/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:35:59.497662 connectome-0.7.0/connectome/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/cache/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/cache/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:35:59.497662 connectome-0.7.0/connectome/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/containers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/containers/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/containers/reversible.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:35:59.501663 connectome-0.7.0/connectome/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/engine/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/engine/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/engine/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/engine/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/engine/node_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/engine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/engine/vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:35:59.505663 connectome-0.7.0/connectome/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/complex_edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17546 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/factory_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/metaclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/interface/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:35:59.509663 connectome-0.7.0/connectome/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/layers/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-27 13:35:52.000000 connectome-0.7.0/connectome/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:35:59.497662 connectome-0.7.0/connectome.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-06-27 13:35:59.000000 connectome-0.7.0/connectome.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-27 13:35:59.000000 connectome-0.7.0/connectome.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:35:59.000000 connectome-0.7.0/connectome.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 13:35:59.000000 connectome-0.7.0/connectome.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 13:35:59.000000 connectome-0.7.0/connectome.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-27 13:35:52.000000 connectome-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 13:35:52.000000 connectome-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:35:59.509663 connectome-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-27 13:35:52.000000 connectome-0.7.0/setup.py
```

### Comparing `connectome-0.6.1/LICENSE` & `connectome-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome-0.6.1/PKG-INFO` & `connectome-0.7.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: connectome
-Version: 0.6.1
-Summary: A library for datasets containing heterogeneous data
-Home-page: https://github.com/neuro-ml/connectome
-License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/connectome/archive/v0.6.1.tar.gz
-Keywords: dag,dataset,cache,consistency
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![docs](https://img.shields.io/badge/-docs-success)](https://neuro-ml.github.io/connectome/)
 [![codecov](https://codecov.io/gh/neuro-ml/connectome/branch/master/graph/badge.svg)](https://codecov.io/gh/neuro-ml/connectome)
 [![pypi](https://img.shields.io/pypi/v/connectome?logo=pypi&label=PyPi)](https://pypi.org/project/connectome/)
 ![License](https://img.shields.io/github/license/neuro-ml/connectome)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/connectome)](https://pypi.org/project/connectome/)
 
 Connectome is a framework for datasets management with strong emphasis on simplicity, composability and reusability.
@@ -63,9 +40,7 @@
 Also, you can check out our `Intro to connectome` series of
 tutorials [here](https://neuro-ml.github.io/connectome/tutorials/00%20-%20Intro/)
 
 # Acknowledgements
 
 Some parts of our automatic cache invalidation machinery vere heavily inspired by
 the [cloudpickle](https://github.com/cloudpipe/cloudpickle) project.
-
-
```

### Comparing `connectome-0.6.1/connectome/cache/base.py` & `connectome-0.7.0/connectome/cache/base.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.1/connectome/cache/disk.py` & `connectome-0.7.0/connectome/cache/disk.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.1/connectome/cache/memory.py` & `connectome-0.7.0/connectome/cache/memory.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .base import Cache
 
 
 class MemoryCache(Cache):
     def __init__(self, size: Union[int, None]):
         super().__init__()
         self._lock = Lock()
+        self.size = size
         if size is not None:
             self._cache = lrucache(size)
         else:
             self._cache = {}
 
     def get(self, key: NodeHash, context) -> Tuple[Any, bool]:
         key = key.value
@@ -27,7 +28,10 @@
         key = key.value
         with self._lock:
             self._cache[key] = value
 
     def clear(self):
         with self._lock:
             self._cache = {}
+
+    def __reduce__(self):
+        return self.__class__, (self.size,)
```

### Comparing `connectome-0.6.1/connectome/containers/base.py` & `connectome-0.7.0/connectome/containers/base.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.1/connectome/containers/context.py` & `connectome-0.7.0/connectome/containers/context.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.1/connectome/containers/reversible.py` & `connectome-0.7.0/connectome/containers/reversible.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.1/connectome/engine/base.py` & `connectome-0.7.0/connectome/engine/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,66 +1,72 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import Any, Collection, Dict, Generator, Iterable, NamedTuple, Optional, Sequence, Set, Tuple, Type, Union
 
 from ..exceptions import GraphError
 from .node_hash import NodeHash, NodeHashes
 
 __all__ = (
     'Command', 'HashOutput', 'Request', 'Response', 'HashError',
     'Edge', 'Node', 'Nodes', 'NodeSet', 'BoundEdge', 'BoundEdges', 'TreeNode', 'TreeNodes', 'Details',
+    'EvalGen', 'HashGen',
 )
 
 
 class Command(Enum):
     ParentHash, CurrentHash, ParentValue, Payload, Await, Call = range(6)
     Send, Store, Item, ComputeHash, Evaluate, AwaitFuture, Tuple, Return = range(-8, 0)
 
 
 HashOutput = Tuple[NodeHash, Any]
 Request = Tuple  # [RequestType, Any, ...]
 Response = Union[NodeHash, Any, Tuple[NodeHash, Any]]
+HashGen = Generator[Request, Response, HashOutput]
+EvalGen = Generator[Request, Response, Any]
 
 
 class Edge(ABC):
     def __init__(self, arity: int):
         self.arity = arity
 
     @abstractmethod
-    def compute_hash(self) -> Generator[Request, Response, HashOutput]:
+    def compute_hash(self) -> HashGen:
         """ Computes the hash of the output given the input hashes. """
 
     @abstractmethod
-    def evaluate(self) -> Generator[Request, Response, Any]:
+    def evaluate(self) -> EvalGen:
         """ Computes the output value. """
 
     def hash_graph(self, inputs: NodeHashes) -> NodeHash:
         """ Propagates the graph's hash without any control flow. """
+        # TODO: remove this check
         assert len(inputs) == self.arity
         return self._hash_graph(inputs)
 
     @abstractmethod
     def _hash_graph(self, inputs: NodeHashes) -> NodeHash:
         """ Propagates the graph's hash without any control flow. """
 
-    def bind(self, inputs: Union['Node', 'Nodes'], output: 'Node') -> 'BoundEdge':
+    def bind(self, inputs: Union[Node, Nodes], output: Node) -> BoundEdge:
         if isinstance(inputs, Node):
             inputs = [inputs]
         assert len(inputs) == self.arity, (len(inputs), self.arity)
         return BoundEdge(self, inputs, output)
 
 
 class Details:
-    def __init__(self, layer: Union[str, Type], parent: Optional['Details'] = None):
+    def __init__(self, layer: Union[str, Type], parent: Optional[Details] = None):
         if isinstance(layer, type):
             layer = layer.__name__
         self.layer = layer
         self.parent = parent
 
-    def update(self, mapping: Dict['Details', 'Details'], parent: Union['Details', None]):
+    def update(self, mapping: Dict[Details, Details], parent: Union[Details, None]):
         """ Update the whole tree based on a mapping """
         assert isinstance(parent, Details) or parent is None, parent
         if self.parent is not None:
             if self.parent in mapping:
                 parent = mapping[self.parent]
             else:
                 parent = mapping[self.parent] = self.parent.update(mapping, parent)
@@ -73,15 +79,15 @@
             result += ' -> ' + str(self.parent)
         return result
 
 
 class TreeNode:
     __slots__ = 'name', '_edge', 'details'
 
-    def __init__(self, name: str, edge: Optional[Tuple[Edge, Sequence['TreeNode']]],
+    def __init__(self, name: str, edge: Optional[Tuple[Edge, Sequence[TreeNode]]],
                  details: Union[Details, None] = None):
         self.name, self._edge, self.details = name, edge, details
 
     @property
     def is_leaf(self):
         return self._edge is None
 
@@ -90,15 +96,15 @@
         return self._edge[0]
 
     @property
     def parents(self):
         return self._edge[1]
 
     @classmethod
-    def from_edges(cls, edges: Iterable['BoundEdge']) -> Dict['Node', 'TreeNode']:
+    def from_edges(cls, edges: Iterable[BoundEdge]) -> Dict[Node, TreeNode]:
         def update(node: Node):
             if node in mapping:
                 return mapping[node]
 
             bridge = bridges.get(node)
             if bridge is not None:
                 bridge = bridge.edge, tuple(map(update, bridge.inputs))
@@ -118,21 +124,21 @@
 
         mapping = {}
         for n in nodes:
             update(n)
         return mapping
 
     @staticmethod
-    def to_edges(nodes: Iterable['TreeNode']) -> Sequence['BoundEdge']:
+    def to_edges(nodes: Iterable[TreeNode]) -> Sequence[BoundEdge]:
         def reverse(node) -> Node:
             if node not in _reversed:
                 _reversed[node] = Node(node.name, node.details)
             return _reversed[node]
 
-        def visit(node: 'TreeNode'):
+        def visit(node: TreeNode):
             if node in visited or node.is_leaf:
                 return
             visited.add(node)
             for parent in node.parents:
                 visit(parent)
 
             result.append(BoundEdge(node.edge, list(map(reverse, node.parents)), reverse(node)))
@@ -162,15 +168,15 @@
 
     def __repr__(self):
         return f'<Node: {self.name}>'
 
 
 class BoundEdge(NamedTuple):
     edge: Edge
-    inputs: 'Nodes'
+    inputs: Nodes
     output: Node
 
 
 TreeNodes = Collection[TreeNode]
 Nodes = Collection[Node]
 NodeSet = Set[Node]
 BoundEdges = Collection[BoundEdge]
```

### Comparing `connectome-0.6.1/connectome/engine/compiler.py` & `connectome-0.7.0/connectome/engine/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     def fields(self):
         if self._outputs is None:
             self._validate_optionals()
 
         return list(self._outputs)
 
-    def compile(self, output: Union[str, Tuple[str]]):
+    def compile(self, output: Union[str, Tuple[str]]) -> Graph:
         if not isinstance(output, (str, tuple)):
             raise TypeError(f'The name must be either a string or a tuple of strings, not {type(output)}')
 
         if self._outputs is None:
             self._validate_optionals()
 
         if output not in self._cache:
@@ -67,27 +67,27 @@
 
         if isinstance(item, str):
             node = get_node(item)
             if node is None:
                 # TODO: signature
                 return identity
 
-            return Graph(self._inputs, node, self._executor).call
+            return Graph(self._inputs, node, self._executor)
 
         inputs, outputs = [], []
         for name in item:
             node = get_node(name)
             if node is None:
                 node = TreeNode(name, None, None)
                 inputs.append(node)
 
             outputs.append(node)
 
-        product = TreeNode('tuple', (ProductEdge(len(item)), outputs), None)
-        return Graph(self._inputs | set(inputs), product, self._executor).call
+        product = TreeNode(f'({", ".join(item)})', (ProductEdge(len(item)), outputs), None)
+        return Graph(self._inputs | set(inputs), product, self._executor)
 
     def __getitem__(self, item):
         # TODO: deprecate
         return self.compile(item)
 
     def _validate_optionals(self):
         self._dependencies = find_dependencies(self._all_outputs.values())
```

### Comparing `connectome-0.6.1/connectome/engine/edges.py` & `connectome-0.7.0/connectome/engine/edges.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,17 @@
     'ConstantEdge', 'ComputableHashBase', 'ProductEdge', 'HashBarrier',
 )
 
 
 class StaticHash(Edge):
     """ Computes the current hash from all the parents' hashes. """
 
+    def __init__(self, arity: int):
+        super().__init__(arity)
+
     def compute_hash(self) -> Generator[Request, Response, HashOutput]:
         inputs = yield (Command.Await, *(
             (Command.ParentHash, idx)
             for idx in range(self.arity)
         ))
         return self._compute_hash(inputs)
 
@@ -166,18 +169,15 @@
         output = yield Command.CurrentHash,
         key, context = self.cache.prepare(output)
         value, exists = self.cache.get(key, context)
         if exists:
             return value
 
         value = yield Command.ParentValue, 0
-        # TODO: what to do in case of a collision:
-        #   overwrite?
-        #   add consistency check?
-        #   get the value from cache?
+        # we can have a collision here, but it's up to the cache to handle them correctly
         self.cache.set(key, value, context)
         return value
 
 
 class ProductEdge(StaticGraph, StaticEdge):
     def _make_hash(self, inputs: NodeHashes) -> NodeHash:
         return ApplyHash(tuple, *inputs)
```

### Comparing `connectome-0.6.1/connectome/engine/executor.py` & `connectome-0.7.0/connectome/engine/executor.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.1/connectome/engine/graph.py` & `connectome-0.7.0/connectome/engine/graph.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,22 +20,29 @@
             inspect.Parameter(x.name, inspect.Parameter.POSITIONAL_OR_KEYWORD)
             for x in inputs
         ])
         self.inputs = inputs
         self.output = output
         self.counts = counts
         self.executor = DefaultExecutor if executor is None else executor
+        self.__signature__ = signature
+        # TODO: deprecate
+        self.call = self.__call__
 
-        def caller(*args, **kwargs):
-            scope = signature.bind(*args, **kwargs)
-            hashes, cache = self._prepare_cache(scope.arguments)
-            return evaluate(output, hashes, cache, self.executor)
+    def __call__(*args, **kwargs):
+        self, *args = args
+        scope = self.__signature__.bind(*args, **kwargs)
+        hashes, cache = self._prepare_cache(scope.arguments)
+        return evaluate(self.output, hashes, cache, self.executor)
 
-        caller.__signature__ = signature
-        self.call = caller
+    def __str__(self):
+        inputs = ', '.join(x.name for x in self.inputs)
+        if len(self.inputs) != 1:
+            inputs = f'({inputs})'
+        return f'Graph({inputs} -> {self.output.name})'
 
     def _prepare_cache(self, arguments):
         # put objects into inputs if hashes are not required
         hashes = EvictionCache(self.counts.copy(), {
             node: (LeafHash(arguments[node.name]), None)
             for node in self.inputs
         })
```

### Comparing `connectome-0.6.1/connectome/engine/node_hash.py` & `connectome-0.7.0/connectome/engine/node_hash.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 NODE_TYPES = set()
 
 
 class NodeHash:
     type: int
 
+    __slots__ = 'type', 'value', '_hash', '_hash_target'
+
     def __init__(self, value, hash_target):
         assert self.type is not None
         assert value[0] == self.type
         self.value = value
         self._hash_target = hash_target
         self._hash = None
```

### Comparing `connectome-0.6.1/connectome/engine/utils.py` & `connectome-0.7.0/connectome/engine/utils.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.1/connectome/engine/vm.py` & `connectome-0.7.0/connectome/engine/vm.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.1/connectome/interface/complex_edges.py` & `connectome-0.7.0/connectome/interface/complex_edges.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.1/connectome/interface/edges.py` & `connectome-0.7.0/connectome/interface/edges.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.1/connectome/interface/factory.py` & `connectome-0.7.0/connectome/interface/factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         super().__init__(container, properties)
 
 
 class GraphFactory:
     layer_cls: Type[Layer] = CallableLayer
 
     def __init__(self, layer: str, scope: MultiDict):
+        self.name = layer
         details = Details(layer)
         backward_details = Details(f'{layer}(backward)')
         self.scope = scope
         self.edges = []
         # layer inputs
         self.inputs = NodeStorage(details)
         self.backward_inputs = NodeStorage(backward_details)
@@ -182,15 +183,16 @@
                 self.magic_dispatch[name](value)
 
             elif is_private(name):
                 private[name] = list(group)
 
         # gather private fields from annotations
         # TODO: detect duplicates
-        for name, value in self.scope.get(ANN_MAGIC, [{}])[0].items():
+        annotations = self.scope.get(ANN_MAGIC, [{}])[0]
+        for name, value in annotations.items():
             if not is_private(name):
                 raise FieldError(f'Only private fields can be defined via type annotations ({name})')
             if name not in private:
                 private[name] = [inspect.Parameter.empty]
             # TODO: else make sure it's a constant parameter
 
         constants = set()
@@ -198,15 +200,37 @@
             if len(group) > 1:
                 raise GraphError(f'Private field "{name}" got multiple definitions')
             value, = group
             if isinstance(value, BUILTIN_DECORATORS):
                 raise FieldError(f"{type(value).__name__} objects can't be private ({name}).")
 
             self.parameters.add(name)
-            if not is_detectable(value) or value is inspect.Parameter.empty:
+            # we have 2 edge cases here:
+            is_argument = False
+            if callable(value):
+                #  1. a callable argument without annotation: x = some_func
+                inside_body = getattr(value, '__qualname__', '').startswith(self.name)
+                if name not in annotations:
+                    if not inside_body:
+                        warnings.warn(
+                            f'The parameter {name} is defined outside of the class body. Are you trying to pass '
+                            f'a default value for an argument? If so, add a type annotation: "{name}: Callable = ..."',
+                            UserWarning,
+                        )
+                # a function defined inside the body, which also has a type annotation
+                else:
+                    is_argument = True
+                    if not inside_body:
+                        warnings.warn(
+                            f'The default value for the argument {name} is a function, defined inside of the '
+                            f'class body. Did you forget to remove the type annotation?',
+                            UserWarning,
+                        )
+
+            if is_argument or not is_detectable(value) or value is inspect.Parameter.empty:
                 constants.add(name)
                 arg_name = to_argument(name)
                 self.edges.append(IdentityEdge().bind(self.arguments[arg_name], self.parameters[name]))
                 self.defaults[arg_name] = value
 
         self.arguments.freeze()
         assert set(self.arguments) == set(self.defaults), (self.arguments, self.defaults)
```

### Comparing `connectome-0.6.1/connectome/interface/metaclasses.py` & `connectome-0.7.0/connectome/interface/metaclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import logging
 from typing import Callable, Collection, Dict, Iterable, Tuple, Type, Union
 
 from ..layers import CallableLayer, Layer
 from ..utils import MultiDict
-from .compat import SafeMeta
 from .factory import GraphFactory, SourceFactory, TransformFactory, add_from_mixins, add_quals, items_to_container
 
 logger = logging.getLogger(__name__)
 BASES: Dict[Type[Layer], GraphFactory] = {}
 
 
-class APIMeta(SafeMeta):
+class APIMeta(type):
     @classmethod
     def __prepare__(mcs, *args, **kwargs):
         return MultiDict()
 
     def __new__(mcs, class_name, bases, namespace, **flags):
         if '__factory' in flags:
             factory = flags.pop('__factory')
```

### Comparing `connectome-0.6.1/connectome/interface/nodes.py` & `connectome-0.7.0/connectome/interface/nodes.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.1/connectome/interface/utils.py` & `connectome-0.7.0/connectome/interface/utils.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.1/connectome/layers/apply.py` & `connectome-0.7.0/connectome/layers/apply.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.1/connectome/layers/base.py` & `connectome-0.7.0/connectome/layers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             final = tuple(final)
         if isinstance(inputs, str):
             inputs = [inputs]
 
         def decorator(func: Callable) -> Callable:
             loopback = self._container.loopback(func, inputs, outputs).compile()
             logger.info('Loopback compiled: %s', loopback.fields())
-            return loopback[final]
+            return loopback.compile(final)
 
         return decorator
 
     def _compile(self, inputs: StringsLike):
         if not isinstance(inputs, str):
             inputs = tuple(inputs)
         return self._methods.compile(inputs)
```

### Comparing `connectome-0.6.1/connectome/layers/cache.py` & `connectome-0.7.0/connectome/layers/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,26 @@
 SerializersLike = Union[Serializer, Sequence[Serializer]]
 
 
 class CacheLayer(Layer, ABC):
     def __repr__(self):
         return self.__class__.__name__
 
+    @staticmethod
+    def _detect_impure(node: TreeNode, name: str):
+        if node.is_leaf:
+            return
+
+        if isinstance(node.edge, ImpureEdge):
+            raise ValueError(f'You are trying to cache the field "{name}", '
+                             f'which has an `impure` dependency - "{node.name}"')
+
+        for parent in node.parents:
+            CacheToStorage._detect_impure(parent, name)
+
 
 class CacheToStorage(DynamicConnectLayer, CacheLayer):
     def __init__(self, names: Union[ContainerType[str], None], impure: bool = False):
         super().__init__()
         if names is None:
             names = AntiSet()
         self.names = names
@@ -54,26 +66,14 @@
                 edges.append(CacheEdge(self._get_storage()).bind(inp, out))
 
         return EdgesBag(
             inputs, outputs, edges, IdentityContext(), persistent=None,
             virtual=AntiSet(node_to_dict(outputs)), optional=set(inputs) | set(outputs),
         )
 
-    @staticmethod
-    def _detect_impure(node: TreeNode, name: str):
-        if node.is_leaf:
-            return
-
-        if isinstance(node.edge, ImpureEdge):
-            raise ValueError(f'You are trying to cache the field "{name}", '
-                             f'which has an `impure` dependency - "{node.name}"')
-
-        for parent in node.parents:
-            CacheToStorage._detect_impure(parent, name)
-
 
 class CacheToRam(CacheToStorage):
     """
     Caches the fields from ``names`` to RAM.
 
     If ``size`` is not None - an LRU cache is used.
     """
@@ -106,29 +106,27 @@
         the storage which holds the actual data
     serializer
         the serializer used to save and load the data
     names
         field names that will be cached
     impure
         whether to allow caching of `impure` functions
-    remote
-        remote locations that are used to fetch the cache from (if available)
     """
 
     def __init__(self, index: PathLikes, storage: HashKeyStorage, serializer: SerializersLike, names: StringsLike, *,
                  impure: bool = False, labels: MaybeLabels = None):
         super().__init__(names=names, impure=impure)
         names, serializer = _normalize_disk_arguments(names, serializer)
         self.storage = DiskCache(PickleKeyStorage(index, storage, serializer), labels=labels)
 
     def _get_storage(self) -> Cache:
         return self.storage
 
     @classmethod
-    def simple(cls, *names, root: PathLike, serializer: Union[Serializer, Sequence[Serializer]] = None, 
+    def simple(cls, *names, root: PathLike, serializer: Union[Serializer, Sequence[Serializer]] = None,
                labels: MaybeLabels = None):
         """
         A simple version of caching to disk with adequate default settings.
 
         Parameters
         ----------
         names:
```

### Comparing `connectome-0.6.1/connectome/layers/columns.py` & `connectome-0.7.0/connectome/layers/columns.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,62 +27,69 @@
         the folder(s) where the cache index is stored
     storage
         the storage which holds the actual data
     serializer
         the serializer used to save and load the data
     names
         field names that will be cached
-    remote
-        remote locations that are used to fetch the cache from (if available)
     verbose
         whether to show a progressbar during cache generation
     shard_size
         the size of a disk storage shard. If int - an absolute size value is used,
         if float - a portion relative to the dataset is used,
         if None - all the entries are grouped in a single shard
+    impure
+        whether to allow caching of `impure` functions
     """
 
     def __init__(self, index: PathLikes, storage: HashKeyStorage, serializer: SerializersLike, names: StringsLike, *,
-                 verbose: bool = False, shard_size: Union[int, float, None] = None, labels: MaybeLabels = None):
+                 verbose: bool = False, shard_size: Union[int, float, None] = None, labels: MaybeLabels = None,
+                 impure: bool = False):
         if shard_size == 1:
             raise ValueError(f'Shard size of 1 is ambiguous. Use None if you want to have a single shard')
         names, serializer = _normalize_disk_arguments(names, serializer)
 
         super().__init__()
         self.names = names
         self.shard_size = shard_size
+        self.impure = impure
         self.verbose = verbose
         self.disk = DiskCache(PickleKeyStorage(index, storage, serializer), labels=labels)
         self.ram = MemoryCache(None)
 
     def _prepare_container(self, previous: EdgesBag) -> EdgesBag:
         details = Details(type(self))
         copy = previous.freeze(details)
         mapping = TreeNode.from_edges(copy.edges)
         outputs_copy = node_to_dict(copy.outputs)
 
         # TODO: containers must know about property names
         property_name = 'ids'
         if property_name not in outputs_copy:
             raise DependencyError(f'The previous layer must contain the "{property_name}" property.')
+        # TODO: drop all properties?
+        outputs_copy.pop(property_name)
         keys = Node(property_name, details)
 
         if len(copy.inputs) != 1:
             raise DependencyError(f'The previous layer must have exactly one input')
         key = Node(copy.inputs[0].name, details)
-        graph_inputs = [mapping[copy.inputs[0]]]
 
         inputs, outputs, edges = [key, keys], [], []
         for name in outputs_copy:
             if name in self.names:
+                if not self.impure:
+                    self._detect_impure(mapping[outputs_copy[name]], name)
+
                 inp, out = Node(name, details), Node(name, details)
                 inputs.append(inp)
                 outputs.append(out)
                 # build a graph for each node
-                graph = Graph(graph_inputs, mapping[outputs_copy[name]])
+                # TODO: this is ridiculous
+                graph = copy.compile().compile(name)
                 edges.append(
                     CachedColumn(self.disk, self.ram, graph, self.verbose, self.shard_size).bind([inp, key, keys], out)
                 )
 
         return EdgesBag(
             inputs, outputs, edges, IdentityContext(),
             persistent=None, optional=None, virtual=AntiSet(node_to_dict(outputs)),
```

### Comparing `connectome-0.6.1/connectome/layers/debug.py` & `connectome-0.7.0/connectome/layers/debug.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 
     def evaluate(self) -> Generator[Request, Response, Any]:
         result = []
         if self.return_value:
             value = yield Command.ParentValue, 0
             result.append(value)
 
-        node_hash = yield Command.CurrentHash,
-        node_hash = node_hash.value
+        node_hash = yield Command.ParentHash, 0
         result.append(node_hash)
+        node_hash = node_hash.value
 
         pickled = dumps(node_hash)
         result.append(pickled)
         if self.algorithm is not None:
             result.append(self.algorithm(pickled).digest())
 
         return tuple(result)
```

### Comparing `connectome-0.6.1/connectome/layers/filter.py` & `connectome-0.7.0/connectome/layers/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from tqdm.auto import tqdm
 
 from ..containers import BagContext
 from ..engine import Details, FunctionEdge, Graph, Node, StaticEdge, StaticGraph, TreeNode
 from ..engine.node_hash import ApplyHash
 from ..exceptions import DependencyError
 from ..utils import AntiSet, extract_signature, node_to_dict
-from .base import EdgesBag, Layer
+from .base import EdgesBag
 from .dynamic import DynamicConnectLayer
 
 
-class Filter(DynamicConnectLayer, Layer):
+class Filter(DynamicConnectLayer):
     """
     Filters the `keys` of the current pipeline given a `predicate`.
 
     Examples
     --------
     >>> dataset = Chain(
     ...   source,  # dataset with `image` and `spacing` attributes
@@ -90,10 +90,10 @@
 
     def _make_hash(self, hashes):
         keys, = hashes
         return ApplyHash(filter, self._hash, keys)
 
     def _evaluate(self, inputs: Sequence[Any]) -> Any:
         keys, = inputs
-        return tuple(filter(self.graph.call, tqdm(
+        return tuple(filter(self.graph, tqdm(
             keys, desc='Filtering', disable=not self.verbose,
         )))
```

### Comparing `connectome-0.6.1/connectome/layers/join.py` & `connectome-0.7.0/connectome/layers/join.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,19 +170,19 @@
 
     def evaluate(self) -> Generator[Request, Response, Any]:
         left_keys, right_keys = yield Command.Await, (Command.ParentValue, 0), (Command.ParentValue, 1)
         precomputed_left, precomputed_right = defaultdict(list), defaultdict(list)
         reverse_left, reverse_right = {}, {}
         # TODO: optimize these loops?
         for i in tqdm(left_keys, desc='Computing left join keys', disable=not self.verbose):
-            key = reverse_func(self.to_key, self.left.call(i), reverse_left)
+            key = reverse_func(self.to_key, self.left(i), reverse_left)
             precomputed_left[key].append(i)
 
         for i in tqdm(right_keys, desc='Computing right join keys', disable=not self.verbose):
-            key = reverse_func(self.to_key, self.right.call(i), reverse_right)
+            key = reverse_func(self.to_key, self.right(i), reverse_right)
             precomputed_right[key].append(i)
 
         left, right = set(precomputed_left), set(precomputed_right)
         common = left & right
 
         mapping = {}
         for key in common:
```

### Comparing `connectome-0.6.1/connectome/layers/merge.py` & `connectome-0.7.0/connectome/layers/merge.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.1/connectome/utils.py` & `connectome-0.7.0/connectome/utils.py`

 * *Files identical despite different names*

### Comparing `connectome-0.6.1/connectome.egg-info/SOURCES.txt` & `connectome-0.7.0/connectome.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,40 +17,41 @@
 connectome/cache/__init__.py
 connectome/cache/base.py
 connectome/cache/disk.py
 connectome/cache/memory.py
 connectome/containers/__init__.py
 connectome/containers/base.py
 connectome/containers/context.py
-connectome/containers/group.py
 connectome/containers/reversible.py
 connectome/engine/__init__.py
 connectome/engine/base.py
 connectome/engine/compiler.py
 connectome/engine/edges.py
 connectome/engine/executor.py
 connectome/engine/graph.py
 connectome/engine/node_hash.py
 connectome/engine/utils.py
 connectome/engine/vm.py
 connectome/interface/__init__.py
 connectome/interface/blocks.py
-connectome/interface/compat.py
 connectome/interface/complex_edges.py
 connectome/interface/decorators.py
 connectome/interface/edges.py
 connectome/interface/factory.py
 connectome/interface/factory_utils.py
 connectome/interface/metaclasses.py
 connectome/interface/nodes.py
+connectome/interface/split.py
 connectome/interface/utils.py
 connectome/layers/__init__.py
 connectome/layers/apply.py
 connectome/layers/base.py
 connectome/layers/cache.py
 connectome/layers/chain.py
 connectome/layers/columns.py
 connectome/layers/debug.py
 connectome/layers/dynamic.py
 connectome/layers/filter.py
+connectome/layers/group.py
 connectome/layers/join.py
-connectome/layers/merge.py
+connectome/layers/merge.py
+connectome/layers/split.py
```

### Comparing `connectome-0.6.1/pyproject.toml` & `connectome-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [project]
 name = 'connectome'
 dynamic = ['version', 'dependencies']
 description = 'A library for datasets containing heterogeneous data'
 readme = 'README.md'
-requires-python = '>=3.6'
+requires-python = '>=3.7'
 license = { file = 'LICENSE' }
 keywords = ['dag', 'dataset', 'cache', 'consistency']
 authors = [
-    { name = 'NeuroML Group', email = 'maxs987@gmail.com' }
+    { name = 'NeuroML Group', email = 'max@ira-labs.com' }
 ]
 classifiers = [
     'Development Status :: 4 - Beta',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3 :: Only',
 ]
```

### Comparing `connectome-0.6.1/setup.py` & `connectome-0.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from setuptools import setup, find_packages
 
 classifiers = [
     'Development Status :: 4 - Beta',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3 :: Only',
 ]
@@ -24,18 +23,20 @@
     long_description = file.read()
 version = runpy.run_path(root / name / '__version__.py')['__version__']
 
 setup(
     name=name,
     packages=find_packages(include=(name,)),
     include_package_data=True,
+    author='NeuroML Group',
+    author_email='max@ira-labs.com',
     version=version,
     description='A library for datasets containing heterogeneous data',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/neuro-ml/connectome',
     download_url='https://github.com/neuro-ml/connectome/archive/v%s.tar.gz' % version,
     keywords=['dag', 'dataset', 'cache', 'consistency'],
     classifiers=classifiers,
     install_requires=requirements,
-    python_requires='>=3.6',
+    python_requires='>=3.7',
 )
```

