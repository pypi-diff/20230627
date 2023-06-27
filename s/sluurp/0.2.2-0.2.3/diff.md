# Comparing `tmp/sluurp-0.2.2.tar.gz` & `tmp/sluurp-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sluurp-0.2.2.tar", last modified: Wed Mar 29 09:29:39 2023, max compression
+gzip compressed data, was "sluurp-0.2.3.tar", last modified: Tue Jun 27 09:03:13 2023, max compression
```

## Comparing `sluurp-0.2.2.tar` & `sluurp-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-03-29 09:29:39.232258 sluurp-0.2.2/
--rw-r--r--   0 payno    (81067) soft      (3401)     1102 2022-12-13 14:10:00.000000 sluurp-0.2.2/LICENSE.md
--rw-r--r--   0 payno    (81067) soft      (3401)      784 2023-03-29 09:29:39.232258 sluurp-0.2.2/PKG-INFO
--rw-r--r--   0 payno    (81067) soft      (3401)       82 2023-02-07 07:43:19.000000 sluurp-0.2.2/README.md
--rw-r--r--   0 payno    (81067) soft      (3401)      107 2022-12-13 14:10:17.000000 sluurp-0.2.2/pyproject.toml
--rw-r--r--   0 payno    (81067) soft      (3401)      874 2023-03-29 09:29:39.232258 sluurp-0.2.2/setup.cfg
--rw-r--r--   0 payno    (81067) soft      (3401)       69 2022-12-13 14:20:28.000000 sluurp-0.2.2/setup.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-03-29 09:29:39.228258 sluurp-0.2.2/src/
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-03-29 09:29:39.232258 sluurp-0.2.2/src/sluurp/
--rw-r--r--   0 payno    (81067) soft      (3401)       65 2023-03-29 09:28:43.000000 sluurp-0.2.2/src/sluurp/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1200 2023-03-15 12:23:32.000000 sluurp-0.2.2/src/sluurp/executor.py
--rw-r--r--   0 payno    (81067) soft      (3401)    12589 2023-03-15 12:23:32.000000 sluurp-0.2.2/src/sluurp/job.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1509 2023-03-29 09:28:30.000000 sluurp-0.2.2/src/sluurp/utils.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-03-29 09:29:39.232258 sluurp-0.2.2/src/sluurp.egg-info/
--rw-r--r--   0 payno    (81067) soft      (3401)      784 2023-03-29 09:29:38.000000 sluurp-0.2.2/src/sluurp.egg-info/PKG-INFO
--rw-r--r--   0 payno    (81067) soft      (3401)      307 2023-03-29 09:29:38.000000 sluurp-0.2.2/src/sluurp.egg-info/SOURCES.txt
--rw-r--r--   0 payno    (81067) soft      (3401)        1 2023-03-29 09:29:38.000000 sluurp-0.2.2/src/sluurp.egg-info/dependency_links.txt
--rw-r--r--   0 payno    (81067) soft      (3401)       63 2023-03-29 09:29:38.000000 sluurp-0.2.2/src/sluurp.egg-info/requires.txt
--rw-r--r--   0 payno    (81067) soft      (3401)        7 2023-03-29 09:29:38.000000 sluurp-0.2.2/src/sluurp.egg-info/top_level.txt
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-27 09:03:13.730248 sluurp-0.2.3/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1102 2023-06-27 08:38:21.000000 sluurp-0.2.3/LICENSE.md
+-rw-r--r--   0 payno     (1001) payno     (1001)      784 2023-06-27 09:03:13.730248 sluurp-0.2.3/PKG-INFO
+-rw-r--r--   0 payno     (1001) payno     (1001)       82 2023-06-27 08:38:21.000000 sluurp-0.2.3/README.md
+-rw-r--r--   0 payno     (1001) payno     (1001)      107 2023-06-27 08:38:21.000000 sluurp-0.2.3/pyproject.toml
+-rw-r--r--   0 payno     (1001) payno     (1001)      874 2023-06-27 09:03:13.730248 sluurp-0.2.3/setup.cfg
+-rw-r--r--   0 payno     (1001) payno     (1001)       69 2023-06-27 08:38:21.000000 sluurp-0.2.3/setup.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-27 09:03:13.726248 sluurp-0.2.3/src/
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-27 09:03:13.730248 sluurp-0.2.3/src/sluurp/
+-rw-r--r--   0 payno     (1001) payno     (1001)       65 2023-06-27 09:02:46.000000 sluurp-0.2.3/src/sluurp/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1200 2023-06-27 08:38:21.000000 sluurp-0.2.3/src/sluurp/executor.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    12865 2023-06-27 09:02:09.000000 sluurp-0.2.3/src/sluurp/job.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1509 2023-06-27 08:38:21.000000 sluurp-0.2.3/src/sluurp/utils.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-27 09:03:13.730248 sluurp-0.2.3/src/sluurp.egg-info/
+-rw-r--r--   0 payno     (1001) payno     (1001)      784 2023-06-27 09:03:13.000000 sluurp-0.2.3/src/sluurp.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1001) payno     (1001)      307 2023-06-27 09:03:13.000000 sluurp-0.2.3/src/sluurp.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)        1 2023-06-27 09:03:13.000000 sluurp-0.2.3/src/sluurp.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)       63 2023-06-27 09:03:13.000000 sluurp-0.2.3/src/sluurp.egg-info/requires.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)        7 2023-06-27 09:03:13.000000 sluurp-0.2.3/src/sluurp.egg-info/top_level.txt
```

### Comparing `sluurp-0.2.2/LICENSE.md` & `sluurp-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sluurp-0.2.2/PKG-INFO` & `sluurp-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sluurp
-Version: 0.2.2
+Version: 0.2.3
 Summary: API to submit shell script through slurm SBATCH
 Home-page: https://gitlab.esrf.fr/tomotools/sluurp
 Author: ESRF
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/tomotools/sluurp
 Project-URL: Documentation, https://tomotools.gitlab-pages.esrf.fr/sluurp/
```

### Comparing `sluurp-0.2.2/setup.cfg` & `sluurp-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `sluurp-0.2.2/src/sluurp/executor.py` & `sluurp-0.2.3/src/sluurp/executor.py`

 * *Files identical despite different names*

### Comparing `sluurp-0.2.2/src/sluurp/job.py` & `sluurp-0.2.3/src/sluurp/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import tempfile
 from typing import Optional
 import os
 from sluurp.utils import SubProcessCommand
 from .utils import has_scancel_available, has_scontrol_available
 import time
 import logging
+from uuid import uuid4
 
 _logger = logging.getLogger(__name__)
 
 
 class Job:
     def __init__(self, working_directory) -> None:
         """
@@ -156,17 +157,20 @@
         super().__init__(*args, **kwargs)
         assert isinstance(slurm_config, (dict, type(None)))
         self._job_id = None
         self._status = "Under submission"
         self._slurm_config = slurm_config if slurm_config is not None else {}
 
         self._pycuda_cache_dir = os.path.join(
-            os.path.dirname(self.script_path), ".pycuda_cache_dir"
+            os.path.dirname(self.script_path), f".pycuda_cache_dir_{uuid4()}"
         )
         # as we can have some incoherent home directory we need for some computer to define the pycuda cache directory (for iccbm181 for example)
+        # uuid4: make sure it is unique each time. Else we can get conflict with different scripts
+        # using the same pycuda dir. And the first one ending it will delete it
+        # and the second script will not be able to process...
         self._script.insert(0, f"mkdir -p {self._pycuda_cache_dir}")
         self._script.insert(1, f"export PYCUDA_CACHE_DIR={self._pycuda_cache_dir}")
 
     def set_status(self, status):
         self._status = status
 
     @property
```

### Comparing `sluurp-0.2.2/src/sluurp/utils.py` & `sluurp-0.2.3/src/sluurp/utils.py`

 * *Files identical despite different names*

### Comparing `sluurp-0.2.2/src/sluurp.egg-info/PKG-INFO` & `sluurp-0.2.3/src/sluurp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sluurp
-Version: 0.2.2
+Version: 0.2.3
 Summary: API to submit shell script through slurm SBATCH
 Home-page: https://gitlab.esrf.fr/tomotools/sluurp
 Author: ESRF
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/tomotools/sluurp
 Project-URL: Documentation, https://tomotools.gitlab-pages.esrf.fr/sluurp/
```

