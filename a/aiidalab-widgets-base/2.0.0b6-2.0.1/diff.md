# Comparing `tmp/aiidalab_widgets_base-2.0.0b6.tar.gz` & `tmp/aiidalab_widgets_base-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiidalab_widgets_base-2.0.0b6.tar", last modified: Sun Mar 26 12:37:21 2023, max compression
+gzip compressed data, was "aiidalab_widgets_base-2.0.1.tar", last modified: Tue Jun 27 17:56:06 2023, max compression
```

## Comparing `aiidalab_widgets_base-2.0.0b6.tar` & `aiidalab_widgets_base-2.0.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 12:37:21.308571 aiidalab_widgets_base-2.0.0b6/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-03-26 12:37:21.308571 aiidalab_widgets_base-2.0.0b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 12:37:21.304571 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/bug_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    44666 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/computational_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 12:37:21.304571 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/elns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13169 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    29442 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    53221 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 12:37:21.308571 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    43261 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/viewers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 12:37:21.304571 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-03-26 12:37:21.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-26 12:37:21.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 12:37:21.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 12:37:21.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-26 12:37:21.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-26 12:37:21.000000 aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-03-26 12:37:21.308571 aiidalab_widgets_base-2.0.0b6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 12:37:21.308571 aiidalab_widgets_base-2.0.0b6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_bug_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_computational_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_elns.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_viewers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-03-26 12:37:05.000000 aiidalab_widgets_base-2.0.0b6/tests/test_wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:56:06.029977 aiidalab_widgets_base-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-27 17:56:06.029977 aiidalab_widgets_base-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:56:06.025977 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44663 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/computational_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:56:06.025977 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/elns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29590 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53250 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:56:06.029977 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43257 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:56:06.025977 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-27 17:56:06.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-27 17:56:06.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:56:06.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:56:05.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-27 17:56:06.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 17:56:06.000000 aiidalab_widgets_base-2.0.1/aiidalab_widgets_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-27 17:56:06.029977 aiidalab_widgets_base-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:56:06.029977 aiidalab_widgets_base-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/tests/test_bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/tests/test_computational_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/tests/test_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/tests/test_elns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/tests/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/tests/test_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-06-27 17:55:50.000000 aiidalab_widgets_base-2.0.1/tests/test_wizard.py
```

### Comparing `aiidalab_widgets_base-2.0.0b6/LICENSE.txt` & `aiidalab_widgets_base-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b6/PKG-INFO` & `aiidalab_widgets_base-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiidalab_widgets_base
-Version: 2.0.0b6
+Version: 2.0.1
 Summary: Reusable widgets for AiiDAlab applications.
 Home-page: https://github.com/aiidalab/aiidalab-widgets-base
 Author: The AiiDAlab team
 Author-email: aiidalab@materialscloud.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
```

### Comparing `aiidalab_widgets_base-2.0.0b6/README.md` & `aiidalab_widgets_base-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/__init__.py` & `aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,8 +72,8 @@
     "SubmitButtonWidget",
     "WizardAppWidget",
     "WizardAppWidgetStep",
     "register_viewer_widget",
     "viewer",
 ]
 
-__version__ = "2.0.0b6"
+__version__ = "2.0.1"
```

### Comparing `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/bug_report.py` & `aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/bug_report.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/computational_resources.py` & `aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/computational_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,14 @@
         "Connection refused",  # 6
         pexpect.EOF,  # 7
     ]
     message = traitlets.Unicode()
     password_message = traitlets.Unicode("The passwordless enabling log.")
 
     def __init__(self, **kwargs):
-
         self._ssh_connection_message = None
         self._password_message = ipw.HTML()
         ipw.dlink((self, "password_message"), (self._password_message, "value"))
         self._ssh_password = ipw.Password(layout={"width": "150px"}, disabled=True)
         self._continue_with_password_button = ipw.Button(
             description="Continue", layout={"width": "100px"}, disabled=True
         )
@@ -648,15 +647,14 @@
 class AiidaComputerSetup(ipw.VBox):
     """Inform AiiDA about a computer."""
 
     computer_setup = traitlets.Dict(allow_none=True)
     message = traitlets.Unicode()
 
     def __init__(self, **kwargs):
-
         self._on_setup_computer_success = []
 
         # List of widgets to be displayed.
         self.label = ipw.Text(
             value="",
             placeholder="Will only be used within AiiDA",
             description="Computer name:",
@@ -975,15 +973,14 @@
 class AiidaCodeSetup(ipw.VBox):
     """Class that allows to setup AiiDA code"""
 
     code_setup = traitlets.Dict(allow_none=True)
     message = traitlets.Unicode()
 
     def __init__(self, path_to_root="../", **kwargs):
-
         self._on_setup_code_success = []
 
         # Code label.
         self.label = ipw.Text(
             description="AiiDA code label:",
             layout=LAYOUT,
             style=STYLE,
```

### Comparing `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/data/__init__.py` & `aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/data/__init__.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/databases.py` & `aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/databases.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from aiida.tools.dbimporters.plugins.cod import CodDbImporter
 from optimade_client import default_parameters, query_filter, query_provider
 
 
 class CodQueryWidget(ipw.VBox):
     """Query structures in Crystallography Open Database (COD)
     Useful class members:
-    :ivar structure(Atoms): trait that contains the selected structure, None if structure is not selected."""
+    :ivar structure(Atoms): trait that contains the selected structure, None if structure is not selected.
+    """
 
     structure = tl.Instance(ase.Atoms, allow_none=True)
 
     def __init__(self, title="", **kwargs):
         description = ipw.HTML(
             """<h3>Get crystal structures from
     <a href="http://www.crystallography.net">Crystallography Open Database</a></h3>
```

### Comparing `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/dicts.py` & `aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/dicts.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/elns.py` & `aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/elns.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 ELN_CONFIG = Path.home() / ".aiidalab" / "aiidalab-eln-config.json"
 ELN_CONFIG.parent.mkdir(
     parents=True, exist_ok=True
 )  # making sure that the folder exists.
 
 
 def connect_to_eln(eln_instance=None, **kwargs):
-
     # assuming that the connection can only be established to the ELNs
     # with the stored configuration.
     try:
         with open(ELN_CONFIG) as file:
             config = json.load(file)
     except (FileNotFoundError, json.JSONDecodeError, KeyError):
         return (
@@ -83,15 +82,14 @@
             eln.import_data()
 
 
 class ElnExportWidget(ipw.VBox):
     node = tl.Instance(orm.Node, allow_none=True)
 
     def __init__(self, path_to_root="../", **kwargs):
-
         self.path_to_root = path_to_root
 
         # Send to ELN button.
         send_button = ipw.Button(description="Send to ELN")
         send_button.on_click(self.send_to_eln)
 
         # Use non-default destination.
```

### Comparing `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/export.py` & `aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/export.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/misc.py` & `aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/misc.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/nodes.py` & `aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,15 +291,14 @@
             if getattr(node, "pk", None) == pk:
                 return node
         raise KeyError(pk)
 
 
 class _AppIcon:
     def __init__(self, app, path_to_root, node):
-
         name = app["name"]
         app_object = _AiidaLabApp.from_id(name)
         self.logo = app_object.metadata["logo"]
         if app_object.is_installed():
             self.link = f"{path_to_root}{app['name']}/{app['notebook']}?{app['parameter_name']}={node.uuid}"
         else:
             self.link = f"{path_to_root}home/single_app.ipynb?app={app['name']}"
@@ -313,15 +312,14 @@
                 <td style="width:800px"> <p style="font-size:16px;">{self.description} </p></td>
             </tr>
             </table>
             """
 
 
 class OpenAiidaNodeInAppWidget(ipw.VBox):
-
     node = tl.Instance(orm.Node, allow_none=True)
 
     def __init__(self, path_to_root="../", **kwargs):
         self.path_to_root = path_to_root
         self.tab = ipw.Tab(style={"description_width": "initial"})
         self.tab_selection = ipw.RadioButtons(
             options=[],
@@ -348,15 +346,14 @@
             ]
 
             ipw.link((self.tab, "selected_index"), (self.tab_selection, "value"))
         else:
             self.tab.children = []
 
     def get_tab_content(self, apps_type):
-
         tab_content = ipw.HTML("")
 
         for app in SELECTED_APPS:
             if app["calculation_type"] != apps_type:
                 continue
             tab_content.value += _AppIcon(
                 app=app,
```

### Comparing `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/process.py` & `aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,17 @@
         if self.process is None:
             return
         string = format_call_graph(self.process, info_fn=self.calc_info)
         self.value = (
             string.replace("\n", "<br/>").replace(" ", "&nbsp;").replace("#space#", " ")
         )
 
-    def calc_info(self, node):
+    # The third parameter 'call_link_label', added in AiiDA 2.4, is not used here.
+    # https://github.com/aiidateam/aiida-core/pull/6056
+    def calc_info(self, node, _=False):
         """Return a string with the summary of the state of a CalculationNode."""
 
         if not isinstance(node, orm.ProcessNode):
             raise TypeError(f"Unknown type: {type(node)}")
 
         process_state = node.process_state.value.capitalize()
         pk = f"""<a#space#href={self.path_to_root}aiidalab-widgets-base/notebooks/process.ipynb?id={node.pk}#space#target="_blank">{node.pk}</a>"""
@@ -720,15 +722,15 @@
     """Monitor a process and execute callback functions at specified intervals."""
 
     value = tl.Unicode(allow_none=True)
 
     def __init__(self, callbacks=None, on_sealed=None, timeout=None, **kwargs):
         self.callbacks = [] if callbacks is None else list(callbacks)
         self.on_sealed = [] if on_sealed is None else list(on_sealed)
-        self.timeout = 0.1 if timeout is None else timeout
+        self.timeout = 1.0 if timeout is None else timeout
 
         self._monitor_thread = None
         self._monitor_thread_stop = threading.Event()
         self._monitor_thread_lock = threading.Lock()
 
         super().__init__(**kwargs)
```

### Comparing `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/structures.py` & `aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,14 @@
         self.structure_node.description = self.structure_description.value
         self.structure_description.disabled = True
 
         if (
             isinstance(self.input_structure, orm.Data)
             and self.input_structure.is_stored
         ):
-
             # Make a link between self.input_structure and self.structure_node
             @engine.calcfunction
             def user_modifications(source_structure):
                 return self.structure_node
 
             structure_node = user_modifications(self.input_structure)
 
@@ -721,15 +720,16 @@
         )
 
     def _make_ase(self, species, positions, smiles):
         """Create ase Atoms object."""
         from sklearn.decomposition import PCA
 
         # Get the principal axes and realign the molecule along z-axis.
-        positions = PCA(n_components=3).fit_transform(positions)
+        if len(species) > 2:
+            positions = PCA(n_components=3).fit_transform(positions)
         atoms = ase.Atoms(species, positions=positions, pbc=False)
         atoms.cell = np.ptp(atoms.positions, axis=0) + 10
         atoms.center()
         # We're attaching this info so that it
         # can be later stored as an extra on AiiDA Structure node.
         atoms.info["smiles"] = smiles
 
@@ -820,15 +820,14 @@
     arguments for structure and selection are passed by copy rather than
     reference. A pop-up warning message is shown in case that neither a
     structure or selection are set.
     """
 
     @functools.wraps(operator)
     def inner(ref, *args, **kwargs):
-
         if not ref.structure:
             ref._status_message.message = """
             <div class="alert alert-info">
             <strong>Please choose a structure first.</strong>
             </div>
             """
         else:
@@ -850,15 +849,14 @@
     arguments for structure and selection are passed by copy rather than
     reference. A pop-up warning message is shown in case that neither a
     structure or selection are set.
     """
 
     @functools.wraps(operator)
     def inner(ref, *args, **kwargs):
-
         if not ref.selection:
             ref._status_message.message = """
             <div class="alert alert-info">
             <strong>Please select atoms first.</strong>
             </div>
             """
         else:
@@ -949,15 +947,14 @@
 
     structure = tl.Instance(ase.Atoms, allow_none=True)
     input_selection = tl.List(tl.Int(), allow_none=True)
     selection = tl.List(tl.Int())
     camera_orientation = tl.List()
 
     def __init__(self, title=""):
-
         self.title = title
 
         # Define action vector.
         self.axis_p1 = ipw.Text(
             description="Starting point", value="0 0 0", layout={"width": "initial"}
         )
         self.axis_p2 = ipw.Text(
```

### Comparing `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/utils/__init__.py` & `aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/viewers.py` & `aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/viewers.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         warnings.warn(
             f"This viewer works only with AiiDA objects, got {type(obj)}", stacklevel=2
         )
         return obj
 
     try:
         _viewer = AIIDA_VIEWER_MAPPING[obj.node_type]
-    except (KeyError) as exc:
+    except KeyError as exc:
         if obj.node_type in str(exc):
             warnings.warn(
                 f"Did not find an appropriate viewer for the {type(obj)} object. Returning the object "
                 "itself.",
                 stacklevel=2,
             )
             return obj
@@ -81,15 +81,14 @@
                 clear_output()
                 if change["new"]:
                     display(viewer(change["new"]))
 
 
 @register_viewer_widget("data.core.dict.Dict.")
 class DictViewer(ipw.VBox):
-
     value = tl.Unicode()
     """Viewer class for Dict object.
 
     :param parameter: Dict object to be viewed
     :type parameter: Dict
     :param downloadable: If True, add link/button to download the content of the object
     :type downloadable: bool"""
@@ -300,15 +299,14 @@
             value=self._viewer.camera,
             layout={"align_self": "flex-start"},
             style={"button_width": "115.5px"},
             orientation="vertical",
         )
 
         def change_camera(change):
-
             self._viewer.camera = change["new"]
 
         camera_type.observe(change_camera, names="value")
 
         # 4. Center button.
         center_button = ipw.Button(description="Center molecule")
         center_button.on_click(lambda c: self._viewer.center())
```

### Comparing `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base/wizard.py` & `aiidalab_widgets_base-2.0.1/aiidalab_widgets_base/wizard.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """The wizard application allows the implication of a Wizard-like GUI.
 
 Authors:
 
     * Carl Simon Adorf <simon.adorf@epfl.ch>
 """
 import enum
-import threading
-import time
 
 import ipywidgets as ipw
 import traitlets as tl
 
 
 class AtLeastTwoStepsWizardError(ValueError):
     """Using WizardAppWidget only makes sense if the number of setps is at least two."""
@@ -78,28 +76,19 @@
 class WizardAppWidget(ipw.VBox):
     ICON_SEPARATOR = "\u2000"  # en-dash  (placed between title and icon)
 
     ICONS = {
         WizardAppWidgetStep.State.INIT: "\u25cb",
         WizardAppWidgetStep.State.READY: "\u25ce",
         WizardAppWidgetStep.State.CONFIGURED: "\u25cf",
-        WizardAppWidgetStep.State.ACTIVE: ["\u25dc", "\u25dd", "\u25de", "\u25df"],
+        WizardAppWidgetStep.State.ACTIVE: "\u231b",
         WizardAppWidgetStep.State.SUCCESS: "\u2713",
         WizardAppWidgetStep.State.FAIL: "\u00d7",
     }
 
-    @classmethod
-    def icons(cls):
-        """Return the icon set and return animated icons based on the current time stamp."""
-        t = time.time()
-        return {
-            key: item if isinstance(item, str) else item[int(t * len(item) % len(item))]
-            for key, item in cls.ICONS.items()
-        }
-
     selected_index = tl.Int(allow_none=True)
 
     def __init__(self, steps, **kwargs):
         # The number of steps must be greater than one
         # for this app's logic to make sense.
         if len(steps) < 2:
             raise AtLeastTwoStepsWizardError(steps)
@@ -110,25 +99,14 @@
         self.titles, widgets = zip(*steps)
 
         # Initialize the accordion with the widgets ...
         self.accordion = ipw.Accordion(children=widgets)
         self._update_titles()
         ipw.link((self.accordion, "selected_index"), (self, "selected_index"))
 
-        # Automatically update titles to implement the "spinner"
-
-        self._run_update_thread = True
-
-        def spinner_thread():
-            while self._run_update_thread:
-                time.sleep(0.1)
-                self._update_titles()
-
-        threading.Thread(target=spinner_thread).start()
-
         # Watch for changes to each step's state
         for widget in widgets:
             if not widget.has_trait("state"):
                 raise TypeError(
                     f"The provided '{widget}' as wizard app step has no `state` trait. "
                     "It is expected that step classes are derived from the WizardAppWidgetStep class."
                 )
@@ -167,15 +145,15 @@
             children=[self.back_button, self.reset_button, self.next_button]
         )
 
         super().__init__(children=[header, self.accordion], **kwargs)
 
     def _update_titles(self):
         for i, (title, widget) in enumerate(zip(self.titles, self.accordion.children)):
-            icon = self.icons().get(widget.state, str(widget.state).upper())
+            icon = self.ICONS.get(widget.state, str(widget.state).upper())
             self.accordion.set_title(i, f"{icon} Step {i+1}: {title}")
 
     def _consider_auto_advance(self, _=None):
         """Determine whether the app should automatically advance to the next step.
 
         This is performed whenever the current step is within the SUCCESS state and has
         the auto_advance attribute set to True.
@@ -206,20 +184,22 @@
         self._update_buttons()
 
     def can_reset(self):
         steps = [
             self.accordion.children[idx] for idx in range(len(self.accordion.children))
         ]
 
-        if any(not step.can_reset() for step in steps):
+        if not all(step.can_reset() for step in steps):
             return False
 
         if any(step.state is not WizardAppWidgetStep.State.INIT for step in steps):
             return True
 
+        return False
+
     def _update_buttons(self):
         with self.hold_trait_notifications():
             index = self.accordion.selected_index
             if index is None:
                 self.back_button.disabled = True
                 self.next_button.disabled = True
                 self.reset_button.disabled = True
```

### Comparing `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/PKG-INFO` & `aiidalab_widgets_base-2.0.1/aiidalab_widgets_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiidalab-widgets-base
-Version: 2.0.0b6
+Version: 2.0.1
 Summary: Reusable widgets for AiiDAlab applications.
 Home-page: https://github.com/aiidalab/aiidalab-widgets-base
 Author: The AiiDAlab team
 Author-email: aiidalab@materialscloud.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
```

### Comparing `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/SOURCES.txt` & `aiidalab_widgets_base-2.0.1/aiidalab_widgets_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b6/aiidalab_widgets_base.egg-info/requires.txt` & `aiidalab_widgets_base-2.0.1/aiidalab_widgets_base.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ipytree~=0.2
 ipywidgets~=7.7
 widgetsnbextension<3.6.3
 more-itertools~=8.0
 pymysql~=0.9
 nglview~=3.0
 optimade-client==2022.9.19
-spglib~=1.14
+spglib<3,>=1.14
 vapory~=0.1.2
 
 [dev]
 bumpver==2021.1114
 pgtest==1.3.1
 pre-commit==2.10.1
 pytest~=6.2
```

### Comparing `aiidalab_widgets_base-2.0.0b6/setup.cfg` & `aiidalab_widgets_base-2.0.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 	ipytree~=0.2
 	ipywidgets~=7.7
 	widgetsnbextension<3.6.3
 	more-itertools~=8.0
 	pymysql~=0.9
 	nglview~=3.0
 	optimade-client==2022.9.19
-	spglib~=1.14
+	spglib>=1.14,<3
 	vapory~=0.1.2
 python_requires = >=3.8
 include_package_data = True
 zip_safe = False
 
 [options.extras_require]
 dev = 
@@ -70,15 +70,15 @@
 per-file-ignores = 
 	aiidalab_widgets_base/__init__.py: E402
 exclude = 
 	docs/,
 	docs/source/conf.py
 
 [bumpver]
-current_version = "v2.0.0b6"
+current_version = "v2.0.1"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = True
 tag = True
 push = True
 
 [bumpver:file_patterns]
```

### Comparing `aiidalab_widgets_base-2.0.0b6/tests/test_bug_report.py` & `aiidalab_widgets_base-2.0.1/tests/test_bug_report.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b6/tests/test_computational_resources.py` & `aiidalab_widgets_base-2.0.1/tests/test_computational_resources.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b6/tests/test_databases.py` & `aiidalab_widgets_base-2.0.1/tests/test_databases.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b6/tests/test_elns.py` & `aiidalab_widgets_base-2.0.1/tests/test_elns.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b6/tests/test_export.py` & `aiidalab_widgets_base-2.0.1/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b6/tests/test_nodes.py` & `aiidalab_widgets_base-2.0.1/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.0.0b6/tests/test_process.py` & `aiidalab_widgets_base-2.0.1/tests/test_process.py`

 * *Files 14% similar despite different names*

```diff
@@ -80,103 +80,112 @@
 def test_process_follower_widget(multiply_add_process_builder_ready, daemon_client):
     """Test ProcessFollowerWidget with a simple `WorkChainNode`"""
     from aiidalab_widgets_base.process import ProcessFollowerWidget
 
     # Test the widget can be instantiated with empty inputs
     widget = ProcessFollowerWidget()
 
-    daemon_client.stop_daemon(wait=True)
+    if daemon_client.is_daemon_running:
+        daemon_client.stop_daemon(wait=True)
     process = engine.submit(multiply_add_process_builder_ready)
 
     # Test the widget can be instantiated with a process
     widget = ProcessFollowerWidget(process=process)
 
     daemon_client.start_daemon()
 
     # Follow the process till it is completed.
     widget.follow()
 
+    daemon_client.stop_daemon(wait=True)
+
 
 @pytest.mark.usefixtures("aiida_profile_clean")
 def test_process_report_widget(
     multiply_add_process_builder_ready, daemon_client, await_for_process_completeness
 ):
     """Test ProcessReportWidget with a simple `WorkChainNode`"""
     from aiidalab_widgets_base.process import ProcessReportWidget
 
     # Test the widget can be instantiated with empty inputs
     ProcessReportWidget()
 
     # Stopping the daemon and submitting the process.
-    daemon_client.stop_daemon(wait=True)
+    if daemon_client.is_daemon_running:
+        daemon_client.stop_daemon(wait=True)
     process = engine.submit(multiply_add_process_builder_ready)
 
     # Test the widget can be instantiated with a process
     widget = ProcessReportWidget(process=process)
     assert (
         widget.value == "No log messages recorded for this entry"
     )  # No report produced yet.
 
     # Starting the daemon and waiting for the process to complete.
     daemon_client.start_daemon()
     await_for_process_completeness(process)
 
     widget.update()
+    daemon_client.stop_daemon(wait=True)
 
 
 @pytest.mark.usefixtures("aiida_profile_clean")
 def test_process_call_stack_widget(
     multiply_add_process_builder_ready, daemon_client, await_for_process_completeness
 ):
     """Test ProcessCallStackWidget with a simple `WorkChainNode`"""
     from aiidalab_widgets_base.process import ProcessCallStackWidget
 
     # Test the widget can be instantiated with empty inputs
     ProcessCallStackWidget()
 
     # Stopping the daemon and submitting the process.
-    daemon_client.stop_daemon(wait=True)
+    if daemon_client.is_daemon_running:
+        daemon_client.stop_daemon(wait=True)
     process = engine.submit(multiply_add_process_builder_ready)
 
     # Test the widget can be instantiated with a process
     widget = ProcessCallStackWidget(process=process)
     assert widget.value.endswith("Created")
 
     # Starting the daemon and waiting for the process to complete.
     daemon_client.start_daemon()
     await_for_process_completeness(process)
 
     widget.update()
     assert "ArithmeticAddCalculation" in widget.value
+    daemon_client.stop_daemon(wait=True)
 
 
 @pytest.mark.usefixtures("aiida_profile_clean")
 def test_progress_bar_widget(
     multiply_add_process_builder_ready, daemon_client, await_for_process_completeness
 ):
     """Test ProgressBarWidget with a simple `WorkChainNode`"""
     from aiidalab_widgets_base import ProgressBarWidget
 
     # Test the widget can be instantiated with empty inputs
     ProgressBarWidget()
 
     # Stopping the daemon and submitting the process.
-    daemon_client.stop_daemon(wait=True)
+    if daemon_client.is_daemon_running:
+        daemon_client.stop_daemon(wait=True)
     process = engine.submit(multiply_add_process_builder_ready)
 
     # Test the widget can be instantiated with a process
     widget = ProgressBarWidget(process=process)
     assert widget.state.value == "Created"
 
     # Starting the daemon and waiting for the process to complete.
     daemon_client.start_daemon()
     await_for_process_completeness(process)
 
     widget.update()
     assert widget.state.value == "Finished"
+    daemon_client.stop_daemon(wait=True)
 
 
 @pytest.mark.usefixtures("aiida_profile_clean")
 def test_calcjob_output_widget(generate_calc_job_node):
     """Test CalcJobOutputWidget with a simple `WorkChainNode`"""
     from aiidalab_widgets_base.process import CalcJobOutputWidget
 
@@ -218,13 +227,45 @@
     """Test ProcessListWidget with a simple `WorkChainNode`"""
     from aiidalab_widgets_base.process import ProcessListWidget
 
     ProcessListWidget()
 
 
 @pytest.mark.usefixtures("aiida_profile_clean")
+def test_process_monitor(
+    multiply_add_process_builder_ready, daemon_client, await_for_process_completeness
+):
+    """Test ProcessMonitor with a simple `WorkChainNode`"""
+    from aiidalab_widgets_base.process import ProcessMonitor
+
+    ProcessMonitor()
+
+    # Stopping the daemon and submitting the process.
+    if daemon_client.is_daemon_running:
+        daemon_client.stop_daemon(wait=True)
+    process = engine.submit(multiply_add_process_builder_ready)
+
+    test_variable = False
+
+    def f():
+        nonlocal test_variable
+        test_variable = True
+
+    widget = ProcessMonitor(value=process.uuid, callbacks=[f])
+
+    # Starting the daemon and waiting for the process to complete.
+    daemon_client.start_daemon()
+    await_for_process_completeness(process)
+
+    widget.join()  # Make sure the thread is finished.
+
+    assert test_variable
+    daemon_client.stop_daemon(wait=True)
+
+
+@pytest.mark.usefixtures("aiida_profile_clean")
 def test_process_nodes_tree_widget(multiply_add_completed_workchain):
     """Test ProcessNodesTreeWidget with a simple `WorkChainNode`"""
 
     from aiidalab_widgets_base.process import ProcessNodesTreeWidget
 
     ProcessNodesTreeWidget(value=multiply_add_completed_workchain.uuid)
```

### Comparing `aiidalab_widgets_base-2.0.0b6/tests/test_structures.py` & `aiidalab_widgets_base-2.0.1/tests/test_structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,25 @@
 
     # Simulate the structure generation.
     widget.smiles.value = "C"
     widget._on_button_pressed()
     assert isinstance(widget.structure, ase.Atoms)
     assert widget.structure.get_chemical_formula() == "CH4"
 
+    # Regression test that we can generate 1-atom and 2-atom molecules
+    widget.smiles.value = "[O]"
+    widget._on_button_pressed()
+    assert isinstance(widget.structure, ase.Atoms)
+    assert widget.structure.get_chemical_formula() == "O"
+
+    widget.smiles.value = "N#N"
+    widget._on_button_pressed()
+    assert isinstance(widget.structure, ase.Atoms)
+    assert widget.structure.get_chemical_formula() == "N2"
+
 
 @pytest.mark.usefixtures("aiida_profile_clean")
 def test_basic_cell_editor_widget(structure_data_object):
     """Test the `BasicCellEditor`."""
     import aiidalab_widgets_base as awb
 
     widget = awb.BasicCellEditor()
```

### Comparing `aiidalab_widgets_base-2.0.0b6/tests/test_viewers.py` & `aiidalab_widgets_base-2.0.1/tests/test_viewers.py`

 * *Files identical despite different names*

