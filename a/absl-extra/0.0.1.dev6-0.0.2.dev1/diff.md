# Comparing `tmp/absl_extra-0.0.1.dev6.tar.gz` & `tmp/absl_extra-0.0.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absl_extra-0.0.1.dev6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absl_extra-0.0.2.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absl_extra-0.0.1.dev6.tar` & `absl_extra-0.0.2.dev1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1588 2023-06-21 23:46:55.595668 absl_extra-0.0.1.dev6/Readme.md
--rw-r--r--   0        0        0      670 2023-06-21 23:46:55.595668 absl_extra-0.0.1.dev6/absl_extra/__init__.py
--rw-r--r--   0        0        0     2061 2023-06-21 23:46:55.595668 absl_extra-0.0.1.dev6/absl_extra/logging_utils.py
--rw-r--r--   0        0        0     2487 2023-06-21 23:46:55.595668 absl_extra-0.0.1.dev6/absl_extra/notifier.py
--rw-r--r--   0        0        0     4175 2023-06-21 23:46:55.595668 absl_extra-0.0.1.dev6/absl_extra/tasks.py
--rw-r--r--   0        0        0     4522 2023-06-21 23:46:55.595668 absl_extra-0.0.1.dev6/absl_extra/tf_utils.py
--rw-r--r--   0        0        0      880 2023-06-21 23:46:55.595668 absl_extra-0.0.1.dev6/pyproject.toml
--rw-r--r--   0        0        0     2598 1970-01-01 00:00:00.000000 absl_extra-0.0.1.dev6/PKG-INFO
+-rw-r--r--   0        0        0     1588 2023-06-27 21:02:23.720877 absl_extra-0.0.2.dev1/Readme.md
+-rw-r--r--   0        0        0      694 2023-06-27 21:02:23.720877 absl_extra-0.0.2.dev1/absl_extra/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-27 21:02:23.720877 absl_extra-0.0.2.dev1/absl_extra/py.typed
+-rw-r--r--   0        0        0     2061 2023-06-27 21:02:23.720877 absl_extra-0.0.2.dev1/absl_extra/src/logging_utils.py
+-rw-r--r--   0        0        0     2487 2023-06-27 21:02:23.720877 absl_extra-0.0.2.dev1/absl_extra/src/notifier.py
+-rw-r--r--   0        0        0     4175 2023-06-27 21:02:23.720877 absl_extra-0.0.2.dev1/absl_extra/src/tasks.py
+-rw-r--r--   0        0        0     4522 2023-06-27 21:02:23.720877 absl_extra-0.0.2.dev1/absl_extra/src/tf_utils.py
+-rw-r--r--   0        0        0      880 2023-06-27 21:02:23.720877 absl_extra-0.0.2.dev1/pyproject.toml
+-rw-r--r--   0        0        0     2598 1970-01-01 00:00:00.000000 absl_extra-0.0.2.dev1/PKG-INFO
```

### Comparing `absl_extra-0.0.1.dev6/Readme.md` & `absl_extra-0.0.2.dev1/Readme.md`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.1.dev6/absl_extra/__init__.py` & `absl_extra-0.0.2.dev1/absl_extra/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from importlib import util
 
 
 def is_lib_installed(name: str) -> bool:
     return util.find_spec(name) is not None
 
 
-from absl_extra.tasks import run, register_task
-from absl_extra.notifier import BaseNotifier
+from absl_extra.src.tasks import run, register_task
+from absl_extra.src.notifier import BaseNotifier
 
 if is_lib_installed("slack_sdk"):
-    from absl_extra.notifier import SlackNotifier
-from absl_extra.logging_utils import log_before, log_after, setup_logging
+    from absl_extra.src.notifier import SlackNotifier
+from absl_extra.src.logging_utils import log_before, log_after, setup_logging
 
 if is_lib_installed("pymongo"):
-    from absl_extra.tasks import MongoConfig
+    from absl_extra.src.tasks import MongoConfig
 if is_lib_installed("tensorflow"):
-    from absl_extra.tf_utils import (
+    from absl_extra.src.tf_utils import (
         supports_mixed_precision,
         make_gpu_strategy,
         make_tpu_strategy,
         requires_gpu,
     )
```

### Comparing `absl_extra-0.0.1.dev6/absl_extra/logging_utils.py` & `absl_extra-0.0.2.dev1/absl_extra/src/logging_utils.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.1.dev6/absl_extra/notifier.py` & `absl_extra-0.0.2.dev1/absl_extra/src/notifier.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.1.dev6/absl_extra/tasks.py` & `absl_extra-0.0.2.dev1/absl_extra/src/tasks.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.1.dev6/absl_extra/tf_utils.py` & `absl_extra-0.0.2.dev1/absl_extra/src/tf_utils.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.1.dev6/pyproject.toml` & `absl_extra-0.0.2.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "absl_extra"
-version = "0.0.1dev6"
+version = "0.0.2dev1"
 description = "A wrapper to run and monitor absl app."
 readme = "Readme.md"
 requires-python = ">=3.8"
 authors = [
     { name = "Artem Sereda", email = "artem.sereda.tub@gmail.com" }
 ]
 maintainers = [
```

### Comparing `absl_extra-0.0.1.dev6/PKG-INFO` & `absl_extra-0.0.2.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absl_extra
-Version: 0.0.1.dev6
+Version: 0.0.2.dev1
 Summary: A wrapper to run and monitor absl app.
 Author-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Maintainer-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: absl_py
```

