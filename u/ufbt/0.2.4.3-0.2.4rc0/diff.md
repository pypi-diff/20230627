# Comparing `tmp/ufbt-0.2.4.3.tar.gz` & `tmp/ufbt-0.2.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufbt-0.2.4.3.tar", last modified: Tue Jun 27 20:03:15 2023, max compression
+gzip compressed data, was "ufbt-0.2.4rc0.tar", last modified: Fri Jun  9 15:42:29 2023, max compression
```

## Comparing `ufbt-0.2.4.3.tar` & `ufbt-0.2.4rc0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:03:15.249457 ufbt-0.2.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-06-27 20:03:04.000000 ufbt-0.2.4.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-06-27 20:03:15.249457 ufbt-0.2.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-27 20:03:04.000000 ufbt-0.2.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-27 20:03:04.000000 ufbt-0.2.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 20:03:15.249457 ufbt-0.2.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:03:15.249457 ufbt-0.2.4.3/ufbt/
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-27 20:03:04.000000 ufbt-0.2.4.3/ufbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-27 20:03:04.000000 ufbt-0.2.4.3/ufbt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26133 2023-06-27 20:03:04.000000 ufbt-0.2.4.3/ufbt/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:03:15.249457 ufbt-0.2.4.3/ufbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-06-27 20:03:15.000000 ufbt-0.2.4.3/ufbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-27 20:03:15.000000 ufbt-0.2.4.3/ufbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 20:03:15.000000 ufbt-0.2.4.3/ufbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-27 20:03:15.000000 ufbt-0.2.4.3/ufbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-27 20:03:15.000000 ufbt-0.2.4.3/ufbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:42:29.864634 ufbt-0.2.4rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-06-09 15:42:16.000000 ufbt-0.2.4rc0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-06-09 15:42:29.864634 ufbt-0.2.4rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-09 15:42:16.000000 ufbt-0.2.4rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-09 15:42:16.000000 ufbt-0.2.4rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 15:42:29.864634 ufbt-0.2.4rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:42:29.864634 ufbt-0.2.4rc0/ufbt/
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-09 15:42:16.000000 ufbt-0.2.4rc0/ufbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-09 15:42:16.000000 ufbt-0.2.4rc0/ufbt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26503 2023-06-09 15:42:16.000000 ufbt-0.2.4rc0/ufbt/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:42:29.864634 ufbt-0.2.4rc0/ufbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-06-09 15:42:29.000000 ufbt-0.2.4rc0/ufbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-09 15:42:29.000000 ufbt-0.2.4rc0/ufbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 15:42:29.000000 ufbt-0.2.4rc0/ufbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-09 15:42:29.000000 ufbt-0.2.4rc0/ufbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 15:42:29.000000 ufbt-0.2.4rc0/ufbt.egg-info/top_level.txt
```

### Comparing `ufbt-0.2.4.3/LICENSE.md` & `ufbt-0.2.4rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.4.3/PKG-INFO` & `ufbt-0.2.4rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.4.3
+Version: 0.2.4rc0
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
```

### Comparing `ufbt-0.2.4.3/README.md` & `ufbt-0.2.4rc0/README.md`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.4.3/pyproject.toml` & `ufbt-0.2.4rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.4.3/ufbt/__init__.py` & `ufbt-0.2.4rc0/ufbt/__init__.py`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.4.3/ufbt/__main__.py` & `ufbt-0.2.4rc0/ufbt/__main__.py`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.4.3/ufbt/bootstrap.py` & `ufbt-0.2.4rc0/ufbt/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -593,19 +593,30 @@
         )
         mode_group = parser.add_mutually_exclusive_group(required=False)
         for loader_cls in all_boostrap_loader_cls:
             loader_cls.add_args_to_mode_group(mode_group)
 
     def _func(self, args) -> int:
         sdk_deployer = UfbtSdkDeployer(args.ufbt_home)
+        current_task = SdkDeployTask.from_args(args)
+        task_to_deploy = None
 
-        task_to_deploy = sdk_deployer.get_previous_task() or SdkDeployTask.default()
-        task_to_deploy.update_from(SdkDeployTask.from_args(args))
-
-        return 0 if sdk_deployer.deploy(task_to_deploy) else 1
+        if previous_task := sdk_deployer.get_previous_task():
+            previous_task.update_from(current_task)
+            task_to_deploy = previous_task
+        else:
+            if current_task.mode:
+                task_to_deploy = current_task
+            else:
+                log.warn("No previous SDK state was found, fetching latest release")
+                task_to_deploy = SdkDeployTask.default()
+
+        if not sdk_deployer.deploy(task_to_deploy):
+            return 1
+        return 0
 
 
 class CleanSubcommand(CliSubcommand):
     COMMAND = "clean"
 
     def __init__(self):
         super().__init__(self.COMMAND, "Clean uFBT SDK state")
```

### Comparing `ufbt-0.2.4.3/ufbt.egg-info/PKG-INFO` & `ufbt-0.2.4rc0/ufbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.4.3
+Version: 0.2.4rc0
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
```

