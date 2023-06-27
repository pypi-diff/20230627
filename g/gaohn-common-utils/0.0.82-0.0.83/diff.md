# Comparing `tmp/gaohn-common-utils-0.0.82.tar.gz` & `tmp/gaohn-common-utils-0.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.82.tar", last modified: Mon Jun 26 09:34:29 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.83.tar", last modified: Tue Jun 27 05:14:17 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.82.tar` & `gaohn-common-utils-0.0.83.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:29.401795 gaohn-common-utils-0.0.82/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-26 09:34:29.401795 gaohn-common-utils-0.0.82/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:29.397795 gaohn-common-utils-0.0.82/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:29.397795 gaohn-common-utils-0.0.82/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:29.397795 gaohn-common-utils-0.0.82/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:29.397795 gaohn-common-utils-0.0.82/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:29.397795 gaohn-common-utils-0.0.82/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:29.397795 gaohn-common-utils-0.0.82/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/core/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:29.397795 gaohn-common-utils-0.0.82/common_utils/core/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/core/decorators/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/core/decorators/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:29.397795 gaohn-common-utils-0.0.82/common_utils/data_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/data_validator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/data_validator/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:29.397795 gaohn-common-utils-0.0.82/common_utils/experiment_tracking/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:29.401795 gaohn-common-utils-0.0.82/common_utils/experiment_tracking/promoter/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/experiment_tracking/promoter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/experiment_tracking/promoter/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:29.401795 gaohn-common-utils-0.0.82/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/orchestrator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/orchestrator/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:29.397795 gaohn-common-utils-0.0.82/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:29.401795 gaohn-common-utils-0.0.82/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/versioning/dvc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/versioning/dvc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:29.401795 gaohn-common-utils-0.0.82/common_utils/versioning/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/versioning/git/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/common_utils/versioning/git/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:34:29.401795 gaohn-common-utils-0.0.82/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-26 09:34:29.000000 gaohn-common-utils-0.0.82/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-26 09:34:29.000000 gaohn-common-utils-0.0.82/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:34:29.000000 gaohn-common-utils-0.0.82/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-26 09:34:29.000000 gaohn-common-utils-0.0.82/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 09:34:29.000000 gaohn-common-utils-0.0.82/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-26 09:34:07.000000 gaohn-common-utils-0.0.82/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 09:34:29.401795 gaohn-common-utils-0.0.82/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.440505 gaohn-common-utils-0.0.83/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-27 05:14:17.440505 gaohn-common-utils-0.0.83/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.432505 gaohn-common-utils-0.0.83/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.432505 gaohn-common-utils-0.0.83/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.428505 gaohn-common-utils-0.0.83/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.432505 gaohn-common-utils-0.0.83/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.436505 gaohn-common-utils-0.0.83/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.436505 gaohn-common-utils-0.0.83/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/core/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.436505 gaohn-common-utils-0.0.83/common_utils/core/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/core/decorators/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/core/decorators/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.436505 gaohn-common-utils-0.0.83/common_utils/data_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/data_validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/data_validator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.432505 gaohn-common-utils-0.0.83/common_utils/experiment_tracking/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.436505 gaohn-common-utils-0.0.83/common_utils/experiment_tracking/promoter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/experiment_tracking/promoter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/experiment_tracking/promoter/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.440505 gaohn-common-utils-0.0.83/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/orchestrator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/orchestrator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.432505 gaohn-common-utils-0.0.83/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.440505 gaohn-common-utils-0.0.83/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/versioning/dvc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/versioning/dvc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.440505 gaohn-common-utils-0.0.83/common_utils/versioning/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/versioning/git/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/common_utils/versioning/git/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:14:17.440505 gaohn-common-utils-0.0.83/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-27 05:14:17.000000 gaohn-common-utils-0.0.83/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-27 05:14:17.000000 gaohn-common-utils-0.0.83/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 05:14:17.000000 gaohn-common-utils-0.0.83/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-27 05:14:17.000000 gaohn-common-utils-0.0.83/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 05:14:17.000000 gaohn-common-utils-0.0.83/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-27 05:13:54.000000 gaohn-common-utils-0.0.83/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 05:14:17.440505 gaohn-common-utils-0.0.83/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.82/LICENSE` & `gaohn-common-utils-0.0.83/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.82/PKG-INFO` & `gaohn-common-utils-0.0.83/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.82
+Version: 0.0.83
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.82/README.md` & `gaohn-common-utils-0.0.83/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.82/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.83/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.82/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.83/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.82/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.83/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.82/common_utils/core/base.py` & `gaohn-common-utils-0.0.83/common_utils/core/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.82/common_utils/core/common.py` & `gaohn-common-utils-0.0.83/common_utils/core/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import rich
 import torch
 import yaml
 from dotenv import load_dotenv
 from yaml import FullLoader
 
 from common_utils.core.base import DictPersistence
-
 from common_utils.core.logger import Logger
 
 # Setup logging
 # logging.basicConfig(
 #     level="INFO",
 #     format="%(asctime)s [%(levelname)s]: %(message)s",
 #     datefmt="%Y-%m-%d %H:%M:%S",
```

### Comparing `gaohn-common-utils-0.0.82/common_utils/core/decorators/decorators.py` & `gaohn-common-utils-0.0.83/common_utils/core/decorators/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.82/common_utils/core/decorators/timer.py` & `gaohn-common-utils-0.0.83/common_utils/core/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.82/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.83/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.82/common_utils/core/logger.py` & `gaohn-common-utils-0.0.83/common_utils/core/logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,30 @@
 import logging
 import os
 from dataclasses import dataclass, field
 from datetime import datetime
 from pathlib import Path
 from typing import Optional, Union
 
+from rich.console import Console
 from rich.logging import RichHandler
+from rich.theme import Theme
+
+console = Console(
+    theme=Theme(
+        {
+            "logging.level.debug": "magenta",
+            "logging.level.info": "green",
+            "logging.level.warning": "yellow",
+            "logging.level.error": "red",
+            "logging.level.critical": "bold red",
+            # "logging.level.remark": "bold blue",
+        }
+    )
+)
 
 
 class CustomFormatter(logging.Formatter):
     """This class overrides logging.Formatter's pathname to be relative path."""
 
     def format(self, record):
         record.pathname = os.path.relpath(record.pathname)
@@ -155,14 +170,15 @@
             rich_tracebacks=True,
             level=self.level,
             show_level=True,
             show_path=True,
             show_time=True,
             markup=True,
             log_time_format="[%Y-%m-%d %H:%M:%S]",
+            console=console,
         )
         # FIXME: If you set custom formatter, it will duplicate level and time.
         # stream_handler.setFormatter(
         #     CustomFormatter(
         #         "%(asctime)s [%(levelname)s] %(pathname)s %(funcName)s L%(lineno)d: %(message)s",
         #         "%Y-%m-%d %H:%M:%S",
         #     )
```

### Comparing `gaohn-common-utils-0.0.82/common_utils/data_validator/core.py` & `gaohn-common-utils-0.0.83/common_utils/data_validator/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.82/common_utils/experiment_tracking/promoter/base.py` & `gaohn-common-utils-0.0.83/common_utils/experiment_tracking/promoter/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.82/common_utils/experiment_tracking/promoter/core.py` & `gaohn-common-utils-0.0.83/common_utils/experiment_tracking/promoter/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.82/common_utils/orchestrator/core.py` & `gaohn-common-utils-0.0.83/common_utils/orchestrator/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
+import datetime
+import time
 from concurrent.futures import ThreadPoolExecutor
+from dataclasses import dataclass, field
 
 import matplotlib.pyplot as plt
 import networkx as nx
-from dataclasses import dataclass, field
-import time
-
-import datetime
 
 
 # TODO: how to do parallelism?
 class Task:
     """This is a Node in the graph."""
 
     def __init__(self, f, pipeline):
```

### Comparing `gaohn-common-utils-0.0.82/common_utils/versioning/dvc/core.py` & `gaohn-common-utils-0.0.83/common_utils/versioning/dvc/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.82/common_utils/versioning/git/core.py` & `gaohn-common-utils-0.0.83/common_utils/versioning/git/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.82/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.83/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.82
+Version: 0.0.83
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.82/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.83/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.82/pyproject.toml` & `gaohn-common-utils-0.0.83/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.82"
+version = "0.0.83"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

