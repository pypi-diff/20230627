# Comparing `tmp/windeklar-0.1.5.tar.gz` & `tmp/windeklar-0.1.6.tar.gz`

## Comparing `windeklar-0.1.5.tar` & `windeklar-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.1.5/requirements.txt
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.1.5/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.1.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.1.5/.idea/.gitignore
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.1.5/.idea/.name
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.1.5/.idea/WinDeklar.iml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.1.5/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.1.5/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.1.5/.idea/vcs.xml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.1.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.1.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1.5/src/__init__.py
--rwxr-xr-x   0        0        0    15884 2020-02-02 00:00:00.000000 windeklar-0.1.5/src/WinDeklar/QTAux.py
--rw-r--r--   0        0        0    43483 2020-02-02 00:00:00.000000 windeklar-0.1.5/src/WinDeklar/WindowForm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1.5/src/WinDeklar/__init__.py
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 windeklar-0.1.5/src/WinDeklar/graph_aux.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.1.5/src/WinDeklar/points_box.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.1.5/src/WinDeklar/record.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.1.5/src/WinDeklar/signal_aux.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.1.5/src/WinDeklar/test_animation.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.1.5/src/WinDeklar/test_pyqt.py
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 windeklar-0.1.5/src/WinDeklar/view_animation.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 windeklar-0.1.5/src/WinDeklar/view_animation.yaml
--rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 windeklar-0.1.5/src/WinDeklar/view_example.py
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 windeklar-0.1.5/src/WinDeklar/view_example.yaml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.1.5/src/WinDeklar/view_simple_graph.py
--rwxr-xr-x   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.1.5/src/WinDeklar/yaml_functions.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.1.5/LICENSE
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 windeklar-0.1.5/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 windeklar-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.1.6/requirements.txt
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.1.6/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.1.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.1.6/.idea/.gitignore
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.1.6/.idea/.name
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.1.6/.idea/WinDeklar.iml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.1.6/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.1.6/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.1.6/.idea/vcs.xml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.1.6/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.1.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1.6/src/__init__.py
+-rwxr-xr-x   0        0        0    15884 2020-02-02 00:00:00.000000 windeklar-0.1.6/src/WinDeklar/QTAux.py
+-rw-r--r--   0        0        0    43483 2020-02-02 00:00:00.000000 windeklar-0.1.6/src/WinDeklar/WindowForm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1.6/src/WinDeklar/__init__.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 windeklar-0.1.6/src/WinDeklar/graph_aux.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.1.6/src/WinDeklar/points_box.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.1.6/src/WinDeklar/record.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.1.6/src/WinDeklar/signal_aux.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.1.6/src/WinDeklar/test_animation.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.1.6/src/WinDeklar/test_pyqt.py
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 windeklar-0.1.6/src/WinDeklar/view_animation.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 windeklar-0.1.6/src/WinDeklar/view_animation.yaml
+-rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 windeklar-0.1.6/src/WinDeklar/view_example.py
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 windeklar-0.1.6/src/WinDeklar/view_example.yaml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.1.6/src/WinDeklar/view_simple_graph.py
+-rwxr-xr-x   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.1.6/src/WinDeklar/yaml_functions.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 windeklar-0.1.6/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 windeklar-0.1.6/PKG-INFO
```

### Comparing `windeklar-0.1.5/.github/workflows/python-publish.yml` & `windeklar-0.1.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.5/.idea/inspectionProfiles/Project_Default.xml` & `windeklar-0.1.6/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.5/src/WinDeklar/QTAux.py` & `windeklar-0.1.6/src/WinDeklar/QTAux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.5/src/WinDeklar/WindowForm.py` & `windeklar-0.1.6/src/WinDeklar/WindowForm.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.5/src/WinDeklar/graph_aux.py` & `windeklar-0.1.6/src/WinDeklar/graph_aux.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         x      = self.t
         self.t += self.dt
         y = self.function(self.last_r)
         self.last_r += self.inc
         return x, y
 
 
-class RealTimeConstantDataProvider(ga.RealTimeDataProvider):
+class RealTimeConstantDataProvider(RealTimeDataProvider):
     def __init__(self, dt=0.1, min_y=0.0, max_y=10.0, color='Black'):
         self.reference = 0.0
         super(RealTimeConstantDataProvider, self).__init__(dt=dt, min_y=min_y, max_y=max_y, color=color)
 
     def set_reference(self, new_reference):
         self.reference = new_reference
```

### Comparing `windeklar-0.1.5/src/WinDeklar/points_box.py` & `windeklar-0.1.6/src/WinDeklar/points_box.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.5/src/WinDeklar/record.py` & `windeklar-0.1.6/src/WinDeklar/record.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.5/src/WinDeklar/signal_aux.py` & `windeklar-0.1.6/src/WinDeklar/signal_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.5/src/WinDeklar/test_animation.py` & `windeklar-0.1.6/src/WinDeklar/test_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.5/src/WinDeklar/test_pyqt.py` & `windeklar-0.1.6/src/WinDeklar/test_pyqt.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.5/src/WinDeklar/view_animation.py` & `windeklar-0.1.6/src/WinDeklar/view_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.5/src/WinDeklar/view_animation.yaml` & `windeklar-0.1.6/src/WinDeklar/view_animation.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.5/src/WinDeklar/view_example.py` & `windeklar-0.1.6/src/WinDeklar/view_example.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.5/src/WinDeklar/view_example.yaml` & `windeklar-0.1.6/src/WinDeklar/view_example.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.5/src/WinDeklar/view_simple_graph.py` & `windeklar-0.1.6/src/WinDeklar/view_simple_graph.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.5/src/WinDeklar/yaml_functions.py` & `windeklar-0.1.6/src/WinDeklar/yaml_functions.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.5/LICENSE` & `windeklar-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.5/README.md` & `windeklar-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.5/pyproject.toml` & `windeklar-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name    = "WinDeklar"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Nicolas Jodal", email="jnj@genexus.com" },
 ]
 description = "Create winforms in an easy, declarative way. Specially suited for Robotics applications"
 readme      = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `windeklar-0.1.5/PKG-INFO` & `windeklar-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinDeklar
-Version: 0.1.5
+Version: 0.1.6
 Summary: Create winforms in an easy, declarative way. Specially suited for Robotics applications
 Project-URL: Homepage, https://github.com/njodal/WinDeklar
 Project-URL: Bug Tracker, https://github.com/njodal/WinDeklar/issues
 Author-email: Nicolas Jodal <jnj@genexus.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

