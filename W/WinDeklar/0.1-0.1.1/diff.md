# Comparing `tmp/windeklar-0.1.tar.gz` & `tmp/windeklar-0.1.1.tar.gz`

## Comparing `windeklar-0.1.tar` & `windeklar-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.1/requirements.txt
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 windeklar-0.1/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.1/.idea/.gitignore
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.1/.idea/.name
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.1/.idea/WinDeklar.iml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.1/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.1/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.1/.idea/vcs.xml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1/src/__init__.py
--rwxr-xr-x   0        0        0    15884 2020-02-02 00:00:00.000000 windeklar-0.1/src/WinDeklar/QTAux.py
--rw-r--r--   0        0        0    42946 2020-02-02 00:00:00.000000 windeklar-0.1/src/WinDeklar/WindowForm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1/src/WinDeklar/__init__.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 windeklar-0.1/src/WinDeklar/graph_aux.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.1/src/WinDeklar/points_box.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 windeklar-0.1/src/WinDeklar/record.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.1/src/WinDeklar/signal_aux.py
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 windeklar-0.1/src/WinDeklar/test_animation.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.1/src/WinDeklar/test_pyqt.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 windeklar-0.1/src/WinDeklar/view_animation.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 windeklar-0.1/src/WinDeklar/view_animation.yaml
--rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 windeklar-0.1/src/WinDeklar/view_example.py
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 windeklar-0.1/src/WinDeklar/view_example.yaml
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 windeklar-0.1/src/WinDeklar/view_simple_graph.py
--rwxr-xr-x   0        0        0     6347 2020-02-02 00:00:00.000000 windeklar-0.1/src/WinDeklar/yaml_functions.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.1/LICENSE
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 windeklar-0.1/README.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 windeklar-0.1/pyproject.toml
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 windeklar-0.1/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.1.1/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.1.1/.idea/.gitignore
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.1.1/.idea/.name
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.1.1/.idea/WinDeklar.iml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.1.1/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.1.1/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.1.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.1.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/__init__.py
+-rwxr-xr-x   0        0        0    15884 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/QTAux.py
+-rw-r--r--   0        0        0    42946 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/WindowForm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/__init__.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/graph_aux.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/points_box.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/record.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/signal_aux.py
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/test_animation.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/test_pyqt.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/view_animation.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/view_animation.yaml
+-rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/view_example.py
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/view_example.yaml
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/view_simple_graph.py
+-rwxr-xr-x   0        0        0     6347 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/yaml_functions.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 windeklar-0.1.1/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 windeklar-0.1.1/PKG-INFO
```

### Comparing `windeklar-0.1/.github/workflows/python-publish.yml` & `windeklar-0.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1/.idea/inspectionProfiles/Project_Default.xml` & `windeklar-0.1.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1/src/WinDeklar/QTAux.py` & `windeklar-0.1.1/src/WinDeklar/QTAux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1/src/WinDeklar/WindowForm.py` & `windeklar-0.1.1/src/WinDeklar/WindowForm.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1/src/WinDeklar/graph_aux.py` & `windeklar-0.1.1/src/WinDeklar/graph_aux.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import random
 import math
 import matplotlib.lines as mlines
 
-import points_box as pb
+import WinDeklar.points_box as pb
 
 
 class RealTimeDataProvider(object):
     def __init__(self, dt=0.1, min_y=0.0, max_y=10.0, color='Red'):
         self.min_y = min_y
         self.max_y = max_y
         self.color = color
```

### Comparing `windeklar-0.1/src/WinDeklar/points_box.py` & `windeklar-0.1.1/src/WinDeklar/points_box.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1/src/WinDeklar/record.py` & `windeklar-0.1.1/src/WinDeklar/record.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1/src/WinDeklar/signal_aux.py` & `windeklar-0.1.1/src/WinDeklar/signal_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1/src/WinDeklar/test_animation.py` & `windeklar-0.1.1/src/WinDeklar/test_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1/src/WinDeklar/test_pyqt.py` & `windeklar-0.1.1/src/WinDeklar/test_pyqt.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1/src/WinDeklar/view_animation.py` & `windeklar-0.1.1/src/WinDeklar/view_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1/src/WinDeklar/view_animation.yaml` & `windeklar-0.1.1/src/WinDeklar/view_animation.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1/src/WinDeklar/view_example.py` & `windeklar-0.1.1/src/WinDeklar/view_example.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1/src/WinDeklar/view_example.yaml` & `windeklar-0.1.1/src/WinDeklar/view_example.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1/src/WinDeklar/view_simple_graph.py` & `windeklar-0.1.1/src/WinDeklar/view_simple_graph.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1/src/WinDeklar/yaml_functions.py` & `windeklar-0.1.1/src/WinDeklar/yaml_functions.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1/LICENSE` & `windeklar-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `windeklar-0.1/README.md` & `windeklar-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `windeklar-0.1/pyproject.toml` & `windeklar-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name    = "WinDeklar"
-version = "0.1"
+version = "0.1.1"
 authors = [
   { name="Nicolas Jodal", email="jnj@genexus.com" },
 ]
 description = "Create winforms in an easy, declarative way. Specially suited for Robotics applications"
 readme      = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `windeklar-0.1/PKG-INFO` & `windeklar-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinDeklar
-Version: 0.1
+Version: 0.1.1
 Summary: Create winforms in an easy, declarative way. Specially suited for Robotics applications
 Project-URL: Homepage, https://github.com/njodal/WinDeklar
 Project-URL: Bug Tracker, https://github.com/njodal/WinDeklar/issues
 Author-email: Nicolas Jodal <jnj@genexus.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

