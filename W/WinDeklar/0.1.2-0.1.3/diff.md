# Comparing `tmp/windeklar-0.1.2.tar.gz` & `tmp/windeklar-0.1.3.tar.gz`

## Comparing `windeklar-0.1.2.tar` & `windeklar-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.1.2/requirements.txt
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.1.2/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.1.2/.idea/.gitignore
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.1.2/.idea/.name
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.1.2/.idea/WinDeklar.iml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.1.2/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.1.2/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.1.2/.idea/vcs.xml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.1.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/__init__.py
--rwxr-xr-x   0        0        0    15884 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/QTAux.py
--rw-r--r--   0        0        0    42995 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/WindowForm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/__init__.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/graph_aux.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/points_box.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/record.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/signal_aux.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/test_animation.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/test_pyqt.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/view_animation.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/view_animation.yaml
--rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/view_example.py
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/view_example.yaml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/view_simple_graph.py
--rwxr-xr-x   0        0        0     6347 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/yaml_functions.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.1.2/LICENSE
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 windeklar-0.1.2/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 windeklar-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.1.3/requirements.txt
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.1.3/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.1.3/.idea/.gitignore
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.1.3/.idea/.name
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.1.3/.idea/WinDeklar.iml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.1.3/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.1.3/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.1.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.1.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.1.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/__init__.py
+-rwxr-xr-x   0        0        0    15884 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/QTAux.py
+-rw-r--r--   0        0        0    42995 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/WindowForm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/__init__.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/graph_aux.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/points_box.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/record.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/signal_aux.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/test_animation.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/test_pyqt.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/view_animation.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/view_animation.yaml
+-rw-r--r--   0        0        0     5864 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/view_example.py
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/view_example.yaml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/view_simple_graph.py
+-rwxr-xr-x   0        0        0     6347 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/yaml_functions.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 windeklar-0.1.3/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 windeklar-0.1.3/PKG-INFO
```

### Comparing `windeklar-0.1.2/.github/workflows/python-publish.yml` & `windeklar-0.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.2/.idea/inspectionProfiles/Project_Default.xml` & `windeklar-0.1.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.2/src/WinDeklar/QTAux.py` & `windeklar-0.1.3/src/WinDeklar/QTAux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.2/src/WinDeklar/WindowForm.py` & `windeklar-0.1.3/src/WinDeklar/WindowForm.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.2/src/WinDeklar/graph_aux.py` & `windeklar-0.1.3/src/WinDeklar/graph_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.2/src/WinDeklar/points_box.py` & `windeklar-0.1.3/src/WinDeklar/points_box.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.2/src/WinDeklar/record.py` & `windeklar-0.1.3/src/WinDeklar/record.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.2/src/WinDeklar/signal_aux.py` & `windeklar-0.1.3/src/WinDeklar/signal_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.2/src/WinDeklar/test_animation.py` & `windeklar-0.1.3/src/WinDeklar/test_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.2/src/WinDeklar/test_pyqt.py` & `windeklar-0.1.3/src/WinDeklar/test_pyqt.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.2/src/WinDeklar/view_animation.py` & `windeklar-0.1.3/src/WinDeklar/view_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.2/src/WinDeklar/view_animation.yaml` & `windeklar-0.1.3/src/WinDeklar/view_animation.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.2/src/WinDeklar/view_example.py` & `windeklar-0.1.3/src/WinDeklar/view_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import sys
 import time
 
 import WinDeklar.WindowForm as WinForm
 import WinDeklar.graph_aux as ga
 import WinDeklar.QTAux as QTAux
-import record as rc
-import yaml_functions
+import WinDeklar.record as rc
+import WinDeklar.yaml_functions as ya
 
 
 class ExampleHost(WinForm.HostModel):
     """
     Example of a Form with many features:
         * Open and Save files
         * Toolbar
@@ -100,15 +100,15 @@
     def open_yaml_file(self, file_name, progress_bar):
         """
         Example on how to use the progress bar
         :param file_name:
         :param progress_bar: use to give feedback about the opening process
         :return:
         """
-        file = yaml_functions.get_yaml_file(file_name, must_exist=True, verbose=True)
+        file = ya.get_yaml_file(file_name, must_exist=True, verbose=True)
         self.state.update(file['state'])
         print(self.state)
         self.refresh()
 
         # just an example of how to use the ProgressBar, no actually needed in this case
         progress_bar_example(progress_bar, max_value=100, inc=20, sleep_time=0.2)
```

### Comparing `windeklar-0.1.2/src/WinDeklar/view_example.yaml` & `windeklar-0.1.3/src/WinDeklar/view_example.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.2/src/WinDeklar/view_simple_graph.py` & `windeklar-0.1.3/src/WinDeklar/view_simple_graph.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.2/src/WinDeklar/yaml_functions.py` & `windeklar-0.1.3/src/WinDeklar/yaml_functions.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.2/LICENSE` & `windeklar-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.2/README.md` & `windeklar-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.2/pyproject.toml` & `windeklar-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name    = "WinDeklar"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Nicolas Jodal", email="jnj@genexus.com" },
 ]
 description = "Create winforms in an easy, declarative way. Specially suited for Robotics applications"
 readme      = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `windeklar-0.1.2/PKG-INFO` & `windeklar-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinDeklar
-Version: 0.1.2
+Version: 0.1.3
 Summary: Create winforms in an easy, declarative way. Specially suited for Robotics applications
 Project-URL: Homepage, https://github.com/njodal/WinDeklar
 Project-URL: Bug Tracker, https://github.com/njodal/WinDeklar/issues
 Author-email: Nicolas Jodal <jnj@genexus.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

