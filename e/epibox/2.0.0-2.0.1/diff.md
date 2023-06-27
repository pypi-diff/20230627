# Comparing `tmp/epibox-2.0.0.tar.gz` & `tmp/epibox-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epibox-2.0.0.tar", last modified: Tue Jun 27 17:15:12 2023, max compression
+gzip compressed data, was "epibox-2.0.1.tar", last modified: Tue Jun 27 17:31:38 2023, max compression
```

## Comparing `epibox-2.0.0.tar` & `epibox-2.0.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:12.003492 epibox-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-27 17:15:02.000000 epibox-2.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-27 17:15:02.000000 epibox-2.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-27 17:15:02.000000 epibox-2.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-27 17:15:02.000000 epibox-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-27 17:15:02.000000 epibox-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-27 17:15:12.003492 epibox-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-27 17:15:02.000000 epibox-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:11.999492 epibox-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 17:15:02.000000 epibox-2.0.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:11.999492 epibox-2.0.0/epibox/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:11.999492 epibox-2.0.0/epibox/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/common/create_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/common/get_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/common/open_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/common/process_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/common/read_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/common/run_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/common/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/common/write_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/config_debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:11.999492 epibox-2.0.0/epibox/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/devices/connect_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/devices/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/devices/manage_devices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:11.999492 epibox-2.0.0/epibox/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/exceptions/exception_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/exceptions/system_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:12.003492 epibox-2.0.0/epibox/mqtt_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/mqtt_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/mqtt_manager/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/mqtt_manager/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:12.003492 epibox-2.0.0/epibox/run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-06-27 17:15:02.000000 epibox-2.0.0/epibox/run/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:15:11.999492 epibox-2.0.0/epibox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-27 17:15:11.000000 epibox-2.0.0/epibox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-27 17:15:11.000000 epibox-2.0.0/epibox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:15:11.000000 epibox-2.0.0/epibox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-27 17:15:11.000000 epibox-2.0.0/epibox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:15:11.000000 epibox-2.0.0/epibox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-27 17:15:11.000000 epibox-2.0.0/epibox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 17:15:11.000000 epibox-2.0.0/epibox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:15:12.003492 epibox-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-27 17:15:02.000000 epibox-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:38.144710 epibox-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-27 17:31:22.000000 epibox-2.0.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-27 17:31:22.000000 epibox-2.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-27 17:31:22.000000 epibox-2.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-27 17:31:22.000000 epibox-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-27 17:31:22.000000 epibox-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-27 17:31:38.144710 epibox-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-27 17:31:22.000000 epibox-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:38.136710 epibox-2.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:38.136710 epibox-2.0.1/epibox/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:38.140710 epibox-2.0.1/epibox/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/common/create_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/common/get_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/common/open_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/common/process_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/common/read_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/common/run_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/common/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/common/write_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/config_debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:38.140710 epibox-2.0.1/epibox/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/devices/connect_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/devices/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/devices/manage_devices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:38.144710 epibox-2.0.1/epibox/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/exceptions/exception_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/exceptions/system_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:38.144710 epibox-2.0.1/epibox/mqtt_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/mqtt_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/mqtt_manager/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/mqtt_manager/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:38.144710 epibox-2.0.1/epibox/run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/run/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:38.140710 epibox-2.0.1/epibox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-27 17:31:38.000000 epibox-2.0.1/epibox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-27 17:31:38.000000 epibox-2.0.1/epibox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:31:38.000000 epibox-2.0.1/epibox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-27 17:31:38.000000 epibox-2.0.1/epibox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:31:37.000000 epibox-2.0.1/epibox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-27 17:31:38.000000 epibox-2.0.1/epibox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 17:31:38.000000 epibox-2.0.1/epibox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:31:38.144710 epibox-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-27 17:31:22.000000 epibox-2.0.1/setup.py
```

### Comparing `epibox-2.0.0/CONTRIBUTING.rst` & `epibox-2.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/LICENSE` & `epibox-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/PKG-INFO` & `epibox-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epibox
-Version: 2.0.0
+Version: 2.0.1
 Summary: EpiBOX is a Raspberry Pi tool for easy signal acquisition.
 Home-page: https://github.com/anascacais/epibox
 Author: Ana Sofia Carmo
 Author-email: anascacais@gmail.com
 License: MIT license
 Keywords: epibox,signal acquisition,Raspberry Pi
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `epibox-2.0.0/README.md` & `epibox-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/docs/Makefile` & `epibox-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/docs/conf.py` & `epibox-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/docs/installation.rst` & `epibox-2.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/docs/make.bat` & `epibox-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/epibox/common/get_defaults.py` & `epibox-2.0.1/epibox/common/get_defaults.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/epibox/common/open_file.py` & `epibox-2.0.1/epibox/common/open_file.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/epibox/common/process_data.py` & `epibox-2.0.1/epibox/common/process_data.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/epibox/common/read_modules.py` & `epibox-2.0.1/epibox/common/read_modules.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/epibox/common/run_system.py` & `epibox-2.0.1/epibox/common/run_system.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/epibox/common/setup.py` & `epibox-2.0.1/epibox/common/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
 def check_storage(client, opt):
     # Check if default storage is available | loop runs continuosly until it find the storage or until timeout
     # If timeout, setup loop and acquisition are terminated
 
     if platform == "linux" or platform == "linux2":
         # linux
-        drive_path = f"/media/{os.environ.get('USERNAME')}"
+        drive_path = os.path.join("media", os.getlogin())
     elif platform == "darwin":
         # macos
         drive_path = "/Volumes"
     else:
         # import win32api
         drive_path = ""
```

### Comparing `epibox-2.0.0/epibox/common/write_file.py` & `epibox-2.0.1/epibox/common/write_file.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/epibox/devices/connect_device.py` & `epibox-2.0.1/epibox/devices/connect_device.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/epibox/devices/header.py` & `epibox-2.0.1/epibox/devices/header.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/epibox/devices/manage_devices.py` & `epibox-2.0.1/epibox/devices/manage_devices.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/epibox/exceptions/exception_manager.py` & `epibox-2.0.1/epibox/exceptions/exception_manager.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/epibox/exceptions/system_exceptions.py` & `epibox-2.0.1/epibox/exceptions/system_exceptions.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/epibox/mqtt_manager/message_handler.py` & `epibox-2.0.1/epibox/mqtt_manager/message_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,27 +18,28 @@
 def send_default(client):
 
     ######## Available drives ########
     listDrives = ["DRIVES"]
 
     if platform == "linux" or platform == "linux2":
         # linux
-        drive_path = f"/media/{os.environ.get('USERNAME')}"
+        drive_path = os.path.join("media", os.getlogin())
         drives = os.listdir(f"/{drive_path}/")
     elif platform == "darwin":
         # macos
         drive_path = "/Volumes"
-        drives = os.listdir(f"/{drive_path}/")
+        drives = os.listdir(f"{drive_path}/")
     else:
         import win32api
         import win32con
         import win32file
         drives = [i for i in win32api.GetLogicalDriveStrings().split('\x00') if i]
-        drives = [d for d in drives if win32file.GetDriveType(d) == win32con.DRIVE_REMOVABLE]
-    
+        drives = [d for d in drives if win32file.GetDriveType(
+            d) == win32con.DRIVE_REMOVABLE]
+
     for drive in drives:
         total, _, free = shutil.disk_usage(f"/{drive_path}/{drive}")
         listDrives += ["{} ({:.1f}% livre)".format(drive,
                                                    (free / total) * 100)]
 
     message_info = client.publish(
         topic="rpi", qos=2, payload="{}".format(listDrives)
@@ -70,15 +71,15 @@
     )  # raises ValueError and TypeError
     if message_info.rc == 4:
         raise MQTTConnectionError
 
 
 def on_message(client, userdata, message):
 
-    username = os.environ.get("USERNAME")
+    username = os.getlogin()
     message = str(message.payload.decode("utf-8"))
     message = ast.literal_eval(message)
 
     if message[0] == "RESTART":
         # client.loop_stop()
         # client.keepAlive = False
         config_debug.log("Not sure what to do here yet")
@@ -112,15 +113,15 @@
         send_default(client)
 
     ######## New default configuration ########
 
     elif message[0] == "NEW CONFIG DEFAULT":
         defaults = get_default()
 
-        username = os.environ.get("USERNAME")
+        username = os.getlogin()
 
         for key in message[1].keys():
             defaults[key] = message[1][key]
 
         with open(
             "/home/{}/Documents/epibox/args.json".format(username), "w+"
         ) as json_file:
```

### Comparing `epibox-2.0.0/epibox/run/run.py` & `epibox-2.0.1/epibox/run/run.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/epibox.egg-info/PKG-INFO` & `epibox-2.0.1/epibox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epibox
-Version: 2.0.0
+Version: 2.0.1
 Summary: EpiBOX is a Raspberry Pi tool for easy signal acquisition.
 Home-page: https://github.com/anascacais/epibox
 Author: Ana Sofia Carmo
 Author-email: anascacais@gmail.com
 License: MIT license
 Keywords: epibox,signal acquisition,Raspberry Pi
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `epibox-2.0.0/epibox.egg-info/SOURCES.txt` & `epibox-2.0.1/epibox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `epibox-2.0.0/setup.py` & `epibox-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,10 +51,10 @@
     include_package_data=True,
     keywords=["epibox", "signal acquisition", "Raspberry Pi"],
     name="epibox",
     packages=find_packages(include=["epibox", "epibox.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/anascacais/epibox",
-    version="2.0.0",
+    version="2.0.1",
     zip_safe=False,
 )
```

