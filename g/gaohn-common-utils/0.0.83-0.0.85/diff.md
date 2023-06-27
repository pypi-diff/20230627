# Comparing `tmp/gaohn-common-utils-0.0.83.tar.gz` & `tmp/gaohn-common-utils-0.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.83.tar", last modified: Tue Jun 27 05:14:17 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.85.tar", last modified: Tue Jun 27 12:36:54 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.83.tar` & `gaohn-common-utils-0.0.85.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.440505 gaohn-common-utils-0.0.83/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-27 05:14:17.440505 gaohn-common-utils-0.0.83/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.432505 gaohn-common-utils-0.0.83/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.432505 gaohn-common-utils-0.0.83/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.428505 gaohn-common-utils-0.0.83/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.432505 gaohn-common-utils-0.0.83/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.436505 gaohn-common-utils-0.0.83/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.436505 gaohn-common-utils-0.0.83/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/core/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.436505 gaohn-common-utils-0.0.83/common_utils/core/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/core/decorators/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/core/decorators/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.436505 gaohn-common-utils-0.0.83/common_utils/data_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/data_validator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/data_validator/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.432505 gaohn-common-utils-0.0.83/common_utils/experiment_tracking/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.436505 gaohn-common-utils-0.0.83/common_utils/experiment_tracking/promoter/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/experiment_tracking/promoter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/experiment_tracking/promoter/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.440505 gaohn-common-utils-0.0.83/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/orchestrator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/orchestrator/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.432505 gaohn-common-utils-0.0.83/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.440505 gaohn-common-utils-0.0.83/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/versioning/dvc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/versioning/dvc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.440505 gaohn-common-utils-0.0.83/common_utils/versioning/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/versioning/git/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/versioning/git/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.440505 gaohn-common-utils-0.0.83/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-27 05:14:17.000000 gaohn-common-utils-0.0.83/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-27 05:14:17.000000 gaohn-common-utils-0.0.83/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 05:14:17.000000 gaohn-common-utils-0.0.83/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-27 05:14:17.000000 gaohn-common-utils-0.0.83/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 05:14:17.000000 gaohn-common-utils-0.0.83/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 05:14:17.440505 gaohn-common-utils-0.0.83/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:54.286560 gaohn-common-utils-0.0.85/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-27 12:36:54.286560 gaohn-common-utils-0.0.85/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:54.282560 gaohn-common-utils-0.0.85/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:54.282560 gaohn-common-utils-0.0.85/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:54.278560 gaohn-common-utils-0.0.85/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:54.282560 gaohn-common-utils-0.0.85/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:54.282560 gaohn-common-utils-0.0.85/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:54.282560 gaohn-common-utils-0.0.85/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/core/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:54.282560 gaohn-common-utils-0.0.85/common_utils/core/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/core/decorators/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/core/decorators/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:54.282560 gaohn-common-utils-0.0.85/common_utils/data_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/data_validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/data_validator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:54.278560 gaohn-common-utils-0.0.85/common_utils/experiment_tracking/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:54.282560 gaohn-common-utils-0.0.85/common_utils/experiment_tracking/promoter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/experiment_tracking/promoter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/experiment_tracking/promoter/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:54.282560 gaohn-common-utils-0.0.85/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/orchestrator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/orchestrator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:54.278560 gaohn-common-utils-0.0.85/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:54.286560 gaohn-common-utils-0.0.85/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/versioning/dvc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/versioning/dvc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:54.286560 gaohn-common-utils-0.0.85/common_utils/versioning/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/versioning/git/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/common_utils/versioning/git/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:36:54.286560 gaohn-common-utils-0.0.85/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-27 12:36:54.000000 gaohn-common-utils-0.0.85/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-27 12:36:54.000000 gaohn-common-utils-0.0.85/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:36:54.000000 gaohn-common-utils-0.0.85/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-27 12:36:54.000000 gaohn-common-utils-0.0.85/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 12:36:54.000000 gaohn-common-utils-0.0.85/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-27 12:36:24.000000 gaohn-common-utils-0.0.85/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 12:36:54.286560 gaohn-common-utils-0.0.85/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.83/LICENSE` & `gaohn-common-utils-0.0.85/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.83/PKG-INFO` & `gaohn-common-utils-0.0.85/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.83
+Version: 0.0.85
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.83/README.md` & `gaohn-common-utils-0.0.85/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.83/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.85/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.83/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.85/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.83/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.85/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.83/common_utils/core/base.py` & `gaohn-common-utils-0.0.85/common_utils/core/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.83/common_utils/core/common.py` & `gaohn-common-utils-0.0.85/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.83/common_utils/core/decorators/decorators.py` & `gaohn-common-utils-0.0.85/common_utils/core/decorators/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.83/common_utils/core/decorators/timer.py` & `gaohn-common-utils-0.0.85/common_utils/core/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.83/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.85/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.83/common_utils/core/logger.py` & `gaohn-common-utils-0.0.85/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.83/common_utils/data_validator/core.py` & `gaohn-common-utils-0.0.85/common_utils/data_validator/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.83/common_utils/experiment_tracking/promoter/base.py` & `gaohn-common-utils-0.0.85/common_utils/experiment_tracking/promoter/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.83/common_utils/experiment_tracking/promoter/core.py` & `gaohn-common-utils-0.0.85/common_utils/experiment_tracking/promoter/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.83/common_utils/orchestrator/core.py` & `gaohn-common-utils-0.0.85/common_utils/orchestrator/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
+from __future__ import annotations
 import datetime
 import time
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass, field
-
+from typing import Callable, Any, Dict
 import matplotlib.pyplot as plt
 import networkx as nx
 
 
 # TODO: how to do parallelism?
 class Task:
     """This is a Node in the graph."""
 
-    def __init__(self, f, pipeline):
-        self.f = f
+    def __init__(self, func: Callable, pipeline: Pipeline) -> None:
+        self.func = func
         self.pipeline = pipeline
-        self.name = f.__name__
 
-    def __call__(self, *args, **kwargs):
-        return self.f(*args, **kwargs)
+        self.name: str = func.__name__
+
+    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+        return self.func(*args, **kwargs)
 
-    def __rshift__(self, other):
+    def __rshift__(self, other: Task) -> Task:
         self.pipeline.add_dependency(self, other)
         return other
 
 
 class Pipeline:
     def __init__(self):
         self.graph = nx.DiGraph()
@@ -52,15 +54,15 @@
                     args = ()
                 future = executor.submit(task_func, *args)
                 result = future.result()
                 for successor in self.graph.successors(task_name):
                     self.task_data[successor] = (result,)
             return self.task_data
 
-    def visualize(self):
+    def visualize(self) -> None:
         pos = nx.spring_layout(self.graph)
         for node in self.graph.nodes:
             plt.text(
                 pos[node][0],
                 pos[node][1],
                 node,
                 fontsize=12,
```

### Comparing `gaohn-common-utils-0.0.83/common_utils/versioning/dvc/core.py` & `gaohn-common-utils-0.0.85/common_utils/versioning/dvc/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.83/common_utils/versioning/git/core.py` & `gaohn-common-utils-0.0.85/common_utils/versioning/git/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.83/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.85/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.83
+Version: 0.0.85
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.83/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.85/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.83/pyproject.toml` & `gaohn-common-utils-0.0.85/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.83"
+version = "0.0.85"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

