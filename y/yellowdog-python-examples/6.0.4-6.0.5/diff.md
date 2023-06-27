# Comparing `tmp/yellowdog-python-examples-6.0.4.tar.gz` & `tmp/yellowdog-python-examples-6.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowdog-python-examples-6.0.4.tar", last modified: Tue Jun 27 08:14:40 2023, max compression
+gzip compressed data, was "yellowdog-python-examples-6.0.5.tar", last modified: Tue Jun 27 15:22:09 2023, max compression
```

## Comparing `yellowdog-python-examples-6.0.4.tar` & `yellowdog-python-examples-6.0.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-27 08:14:40.543909 yellowdog-python-examples-6.0.4/
--rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-6.0.4/LICENSE
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-27 08:14:40.543984 yellowdog-python-examples-6.0.4/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-6.0.4/PYPI_README.md
--rw-r--r--   0 pwt        (501) staff       (20)   111863 2023-06-27 08:13:55.000000 yellowdog-python-examples-6.0.4/README.md
--rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-6.0.4/pyproject.toml
--rw-r--r--   0 pwt        (501) staff       (20)       62 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.4/requirements.txt
--rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-06-27 08:14:40.544294 yellowdog-python-examples-6.0.4/setup.cfg
--rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.4/setup.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-27 08:14:40.543080 yellowdog-python-examples-6.0.4/yd_commands/
--rw-r--r--   0 pwt        (501) staff       (20)       22 2023-06-27 08:13:55.000000 yellowdog-python-examples-6.0.4/yd_commands/__init__.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3415 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/abort.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-6.0.4/yd_commands/admin.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    18654 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.4/yd_commands/args.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     5114 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/cancel.py
--rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-6.0.4/yd_commands/check_imports.py
--rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-6.0.4/yd_commands/compact_json.py
--rw-r--r--   0 pwt        (501) staff       (20)    17539 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.4/yd_commands/config.py
--rw-r--r--   0 pwt        (501) staff       (20)     5062 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.4/yd_commands/config_keys.py
--rw-r--r--   0 pwt        (501) staff       (20)    12135 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.4/yd_commands/csv_data.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1657 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/delete.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3626 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/download.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     9251 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/instantiate.py
--rw-r--r--   0 pwt        (501) staff       (20)     3729 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/interactive.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-6.0.4/yd_commands/jsonnet2json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     7798 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/list.py
--rw-r--r--   0 pwt        (501) staff       (20)     3000 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/object_utilities.py
--rw-r--r--   0 pwt        (501) staff       (20)     9525 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/printing.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    13218 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.4/yd_commands/provision.py
--rw-r--r--   0 pwt        (501) staff       (20)     1248 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.4/yd_commands/provision_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.4/yd_commands/reformat_json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3232 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/shutdown.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    41866 2023-06-27 08:13:55.000000 yellowdog-python-examples-6.0.4/yd_commands/submit.py
--rw-r--r--   0 pwt        (501) staff       (20)     7748 2023-06-27 08:13:55.000000 yellowdog-python-examples-6.0.4/yd_commands/submit_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     2916 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/terminate.py
--rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-6.0.4/yd_commands/type_check.py
--rw-r--r--   0 pwt        (501) staff       (20)     2545 2023-06-27 08:13:55.000000 yellowdog-python-examples-6.0.4/yd_commands/upload.py
--rw-r--r--   0 pwt        (501) staff       (20)     3621 2023-06-21 15:20:23.000000 yellowdog-python-examples-6.0.4/yd_commands/upload_utils.py
--rw-r--r--   0 pwt        (501) staff       (20)     2177 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.4/yd_commands/validate_properties.py
--rw-r--r--   0 pwt        (501) staff       (20)    11037 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.4/yd_commands/variables.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-6.0.4/yd_commands/version.py
--rw-r--r--   0 pwt        (501) staff       (20)     2995 2023-06-21 15:20:23.000000 yellowdog-python-examples-6.0.4/yd_commands/wrapper.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-27 08:14:40.543811 yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-27 08:14:40.000000 yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-06-27 08:14:40.000000 yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/SOURCES.txt
--rw-r--r--   0 pwt        (501) staff       (20)        1 2023-06-27 08:14:40.000000 yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/dependency_links.txt
--rw-r--r--   0 pwt        (501) staff       (20)      574 2023-06-27 08:14:40.000000 yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/entry_points.txt
--rw-r--r--   0 pwt        (501) staff       (20)       75 2023-06-27 08:14:40.000000 yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/requires.txt
--rw-r--r--   0 pwt        (501) staff       (20)       12 2023-06-27 08:14:40.000000 yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/top_level.txt
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-27 15:22:09.155806 yellowdog-python-examples-6.0.5/
+-rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-6.0.5/LICENSE
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-27 15:22:09.155873 yellowdog-python-examples-6.0.5/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-6.0.5/PYPI_README.md
+-rw-r--r--   0 pwt        (501) staff       (20)   111863 2023-06-27 08:13:55.000000 yellowdog-python-examples-6.0.5/README.md
+-rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-6.0.5/pyproject.toml
+-rw-r--r--   0 pwt        (501) staff       (20)       62 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.5/requirements.txt
+-rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-06-27 15:22:09.156174 yellowdog-python-examples-6.0.5/setup.cfg
+-rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.5/setup.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-27 15:22:09.154988 yellowdog-python-examples-6.0.5/yd_commands/
+-rw-r--r--   0 pwt        (501) staff       (20)       22 2023-06-27 15:17:32.000000 yellowdog-python-examples-6.0.5/yd_commands/__init__.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3415 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.5/yd_commands/abort.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-6.0.5/yd_commands/admin.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    18991 2023-06-27 15:17:32.000000 yellowdog-python-examples-6.0.5/yd_commands/args.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     5114 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.5/yd_commands/cancel.py
+-rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-6.0.5/yd_commands/check_imports.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-6.0.5/yd_commands/compact_json.py
+-rw-r--r--   0 pwt        (501) staff       (20)    17539 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.5/yd_commands/config.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5062 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.5/yd_commands/config_keys.py
+-rw-r--r--   0 pwt        (501) staff       (20)    12135 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.5/yd_commands/csv_data.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1657 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.5/yd_commands/delete.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3626 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.5/yd_commands/download.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     9251 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.5/yd_commands/instantiate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3729 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.5/yd_commands/interactive.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-6.0.5/yd_commands/jsonnet2json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     7938 2023-06-27 15:17:32.000000 yellowdog-python-examples-6.0.5/yd_commands/list.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3000 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.5/yd_commands/object_utilities.py
+-rw-r--r--   0 pwt        (501) staff       (20)     9525 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.5/yd_commands/printing.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    13218 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.5/yd_commands/provision.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1248 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.5/yd_commands/provision_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.5/yd_commands/reformat_json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3232 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.5/yd_commands/shutdown.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    41866 2023-06-27 08:13:55.000000 yellowdog-python-examples-6.0.5/yd_commands/submit.py
+-rw-r--r--   0 pwt        (501) staff       (20)     7560 2023-06-27 15:17:32.000000 yellowdog-python-examples-6.0.5/yd_commands/submit_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     2916 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.5/yd_commands/terminate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-6.0.5/yd_commands/type_check.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2545 2023-06-27 08:13:55.000000 yellowdog-python-examples-6.0.5/yd_commands/upload.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3621 2023-06-21 15:20:23.000000 yellowdog-python-examples-6.0.5/yd_commands/upload_utils.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2177 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.5/yd_commands/validate_properties.py
+-rw-r--r--   0 pwt        (501) staff       (20)    11037 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.5/yd_commands/variables.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-6.0.5/yd_commands/version.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2995 2023-06-21 15:20:23.000000 yellowdog-python-examples-6.0.5/yd_commands/wrapper.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-27 15:22:09.155706 yellowdog-python-examples-6.0.5/yellowdog_python_examples.egg-info/
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-27 15:22:09.000000 yellowdog-python-examples-6.0.5/yellowdog_python_examples.egg-info/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-06-27 15:22:09.000000 yellowdog-python-examples-6.0.5/yellowdog_python_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 pwt        (501) staff       (20)        1 2023-06-27 15:22:09.000000 yellowdog-python-examples-6.0.5/yellowdog_python_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 pwt        (501) staff       (20)      574 2023-06-27 15:22:09.000000 yellowdog-python-examples-6.0.5/yellowdog_python_examples.egg-info/entry_points.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       75 2023-06-27 15:22:09.000000 yellowdog-python-examples-6.0.5/yellowdog_python_examples.egg-info/requires.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       12 2023-06-27 15:22:09.000000 yellowdog-python-examples-6.0.5/yellowdog_python_examples.egg-info/top_level.txt
```

### Comparing `yellowdog-python-examples-6.0.4/LICENSE` & `yellowdog-python-examples-6.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/PKG-INFO` & `yellowdog-python-examples-6.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 6.0.4
+Version: 6.0.5
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-6.0.4/PYPI_README.md` & `yellowdog-python-examples-6.0.5/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/README.md` & `yellowdog-python-examples-6.0.5/README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/pyproject.toml` & `yellowdog-python-examples-6.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/setup.cfg` & `yellowdog-python-examples-6.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/abort.py` & `yellowdog-python-examples-6.0.5/yd_commands/abort.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/admin.py` & `yellowdog-python-examples-6.0.5/yd_commands/admin.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/args.py` & `yellowdog-python-examples-6.0.5/yd_commands/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,14 +271,21 @@
                 "--object-paths",
                 "-o",
                 action="store_true",
                 required=False,
                 help="list YellowDog Object Store object paths",
             )
             parser.add_argument(
+                "--tree",
+                "-T",
+                action="store_true",
+                required=False,
+                help="when used with '--object-paths', list the full object tree",
+            )
+            parser.add_argument(
                 "--work-requirements",
                 "-w",
                 action="store_true",
                 required=False,
                 help="list Work Requirements",
             )
             parser.add_argument(
@@ -519,14 +526,18 @@
         return self.args.compute_requirements
 
     @property
     def live_only(self) -> Optional[bool]:
         return self.args.live_only
 
     @property
+    def object_tree(self) -> Optional[bool]:
+        return self.args.tree
+
+    @property
     def debug(self) -> Optional[bool]:
         return self.args.debug
 
     @property
     def use_pac(self) -> Optional[bool]:
         return self.args.pac
```

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/cancel.py` & `yellowdog-python-examples-6.0.5/yd_commands/cancel.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/check_imports.py` & `yellowdog-python-examples-6.0.5/yd_commands/check_imports.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/compact_json.py` & `yellowdog-python-examples-6.0.5/yd_commands/compact_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/config.py` & `yellowdog-python-examples-6.0.5/yd_commands/config.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/config_keys.py` & `yellowdog-python-examples-6.0.5/yd_commands/config_keys.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/csv_data.py` & `yellowdog-python-examples-6.0.5/yd_commands/csv_data.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/delete.py` & `yellowdog-python-examples-6.0.5/yd_commands/delete.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/download.py` & `yellowdog-python-examples-6.0.5/yd_commands/download.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/instantiate.py` & `yellowdog-python-examples-6.0.5/yd_commands/instantiate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/interactive.py` & `yellowdog-python-examples-6.0.5/yd_commands/interactive.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/jsonnet2json.py` & `yellowdog-python-examples-6.0.5/yd_commands/jsonnet2json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/list.py` & `yellowdog-python-examples-6.0.5/yd_commands/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,18 +142,22 @@
 def list_object_paths():
     print_log(
         f"Listing Object Paths in namespace '{CONFIG_COMMON.namespace}' and "
         f"names starting with '{CONFIG_COMMON.name_tag}'"
     )
     object_paths: List[ObjectPath] = (
         CLIENT.object_store_client.get_namespace_object_paths(
-            ObjectPathsRequest(CONFIG_COMMON.namespace)
+            ObjectPathsRequest(
+                CONFIG_COMMON.namespace,
+                prefix=CONFIG_COMMON.name_tag,
+                flat=ARGS_PARSER.object_tree,
+            )
         )
     )
-    print_numbered_object_list(CLIENT, object_paths)
+    print_numbered_object_list(CLIENT, sorted_objects(object_paths))
 
 
 def list_worker_pools():
     print_log(
         "Listing Provisioned Worker Pools with Compute Requirements in "
         f"namespace '{CONFIG_COMMON.namespace}' and "
         f"names starting with '{CONFIG_COMMON.name_tag}'"
```

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/object_utilities.py` & `yellowdog-python-examples-6.0.5/yd_commands/object_utilities.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/printing.py` & `yellowdog-python-examples-6.0.5/yd_commands/printing.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/provision.py` & `yellowdog-python-examples-6.0.5/yd_commands/provision.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/provision_utils.py` & `yellowdog-python-examples-6.0.5/yd_commands/provision_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/reformat_json.py` & `yellowdog-python-examples-6.0.5/yd_commands/reformat_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/shutdown.py` & `yellowdog-python-examples-6.0.5/yd_commands/shutdown.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/submit.py` & `yellowdog-python-examples-6.0.5/yd_commands/submit.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/submit_utils.py` & `yellowdog-python-examples-6.0.5/yd_commands/submit_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,18 +134,14 @@
             duplicate = False
             for uploaded_file in self._uploaded_files:
                 if (
                     upload_file == uploaded_file.local_file_path
                     and uploaded_file_path == uploaded_file.uploaded_file_path
                     and namespace == uploaded_file.upload_namespace
                 ):
-                    print_log(
-                        f"Not uploading duplicate: '{upload_file}' ->"
-                        f" '{namespace}::{uploaded_file_path}'"
-                    )
                     duplicate = True
                     break
             if duplicate:
                 continue
 
             if not ARGS_PARSER.dry_run:
                 upload_file_core(
@@ -153,15 +149,15 @@
                     url=self._config.url,
                     local_file=upload_file,
                     namespace=namespace,
                     remote_file=uploaded_file_path,
                 )
             else:
                 print_log(
-                    f"Dry-run: would upload '{upload_file}' to"
+                    f"Dry-run: Would upload '{upload_file}' to"
                     f" '{namespace}::{uploaded_file_path}'"
                 )
 
             self._uploaded_files.append(
                 UploadedFile(
                     local_file_path=upload_file,
                     upload_namespace=namespace,
```

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/terminate.py` & `yellowdog-python-examples-6.0.5/yd_commands/terminate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/type_check.py` & `yellowdog-python-examples-6.0.5/yd_commands/type_check.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/upload.py` & `yellowdog-python-examples-6.0.5/yd_commands/upload.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/upload_utils.py` & `yellowdog-python-examples-6.0.5/yd_commands/upload_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/validate_properties.py` & `yellowdog-python-examples-6.0.5/yd_commands/validate_properties.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/variables.py` & `yellowdog-python-examples-6.0.5/yd_commands/variables.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/version.py` & `yellowdog-python-examples-6.0.5/yd_commands/version.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yd_commands/wrapper.py` & `yellowdog-python-examples-6.0.5/yd_commands/wrapper.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/PKG-INFO` & `yellowdog-python-examples-6.0.5/yellowdog_python_examples.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 6.0.4
+Version: 6.0.5
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/SOURCES.txt` & `yellowdog-python-examples-6.0.5/yellowdog_python_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.4/yellowdog_python_examples.egg-info/entry_points.txt` & `yellowdog-python-examples-6.0.5/yellowdog_python_examples.egg-info/entry_points.txt`

 * *Files identical despite different names*

