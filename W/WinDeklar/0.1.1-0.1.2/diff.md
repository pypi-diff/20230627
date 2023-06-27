# Comparing `tmp/windeklar-0.1.1.tar.gz` & `tmp/windeklar-0.1.2.tar.gz`

## Comparing `windeklar-0.1.1.tar` & `windeklar-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.1.1/requirements.txt
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.1.1/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.1.1/.idea/.gitignore
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.1.1/.idea/.name
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.1.1/.idea/WinDeklar.iml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.1.1/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.1.1/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.1.1/.idea/vcs.xml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.1.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/__init__.py
--rwxr-xr-x   0        0        0    15884 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/QTAux.py
--rw-r--r--   0        0        0    42946 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/WindowForm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/__init__.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/graph_aux.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/points_box.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/record.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/signal_aux.py
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/test_animation.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/test_pyqt.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/view_animation.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/view_animation.yaml
--rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/view_example.py
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/view_example.yaml
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/view_simple_graph.py
--rwxr-xr-x   0        0        0     6347 2020-02-02 00:00:00.000000 windeklar-0.1.1/src/WinDeklar/yaml_functions.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.1.1/LICENSE
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 windeklar-0.1.1/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 windeklar-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.1.2/requirements.txt
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.1.2/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.1.2/.idea/.gitignore
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.1.2/.idea/.name
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.1.2/.idea/WinDeklar.iml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.1.2/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.1.2/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.1.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.1.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/__init__.py
+-rwxr-xr-x   0        0        0    15884 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/QTAux.py
+-rw-r--r--   0        0        0    42995 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/WindowForm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/__init__.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/graph_aux.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/points_box.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/record.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/signal_aux.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/test_animation.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/test_pyqt.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/view_animation.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/view_animation.yaml
+-rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/view_example.py
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/view_example.yaml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/view_simple_graph.py
+-rwxr-xr-x   0        0        0     6347 2020-02-02 00:00:00.000000 windeklar-0.1.2/src/WinDeklar/yaml_functions.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 windeklar-0.1.2/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 windeklar-0.1.2/PKG-INFO
```

### Comparing `windeklar-0.1.1/.github/workflows/python-publish.yml` & `windeklar-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.1/.idea/inspectionProfiles/Project_Default.xml` & `windeklar-0.1.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.1/src/WinDeklar/QTAux.py` & `windeklar-0.1.2/src/WinDeklar/QTAux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.1/src/WinDeklar/WindowForm.py` & `windeklar-0.1.2/src/WinDeklar/WindowForm.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import sys
 import matplotlib.pyplot as plt
 from matplotlib.figure import Figure
 from matplotlib import animation
 from PyQt5 import QtGui, QtWidgets
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 
-import points_box
-import QTAux
-import record as rc
-import signal_aux as sg
-import yaml_functions as yaml
+import WinDeklar.points_box as pb
+import WinDeklar.QTAux as QTAux
+import WinDeklar.record as rc
+import WinDeklar.signal_aux as sg
+import WinDeklar.yaml_functions as yaml
 
 
 class ConfigurableWindow(QtWidgets.QMainWindow):
     """
     Defines a Window with many components inside in a declarative manner in a config file
     Notes:
         - a config_file_name is a yaml that has the definition (see view_map.yaml)
@@ -317,15 +317,15 @@
         self.ax = plt.subplot(111)
         if scaled:
             self.ax.axis('scaled')
         self.ax.set_xlim([-size[0], size[0]])
         self.ax.set_ylim([-size[1], size[1]])
         self.inc        = inc
         self.set_bounds = adjust_size
-        self.box_size   = points_box.PointsBox()
+        self.box_size   = pb.PointsBox()
 
     def resize(self, points):
         self.box_size.add_points(points)
 
     def show(self):
         if self.set_bounds:
             self.box_size.set_bounds(self.ax, inc=self.inc)
@@ -419,15 +419,15 @@
 
     def __init__(self, initial_values=None):
         # keys
         self.zoom_key = 'zoom'
 
         self.state       = initial_values if initial_values is not None else {}
         self.main_window = None
-        self.box_size    = points_box.PointsBox()
+        self.box_size    = pb.PointsBox()
 
         self.zoom_center = None   # point where to center Zoom
         self.zoom_radius = 10.0   # radius around
 
     def set_main_window(self, main_window):
         self.main_window = main_window
```

### Comparing `windeklar-0.1.1/src/WinDeklar/graph_aux.py` & `windeklar-0.1.2/src/WinDeklar/graph_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.1/src/WinDeklar/points_box.py` & `windeklar-0.1.2/src/WinDeklar/points_box.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.1/src/WinDeklar/record.py` & `windeklar-0.1.2/src/WinDeklar/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from __future__ import print_function
 
 from datetime import datetime
 
-import yaml_functions as yaml
+import WinDeklar.yaml_functions as yaml
 
 
 class Record:
     def __init__(self, file_name, dir='/tmp', indent=2, ext='yaml', add_time_stamp=True):
         self.file          = None       # only use file if something is going to be writing
         self.file_name     = file_name
         self.ext           = ext
```

### Comparing `windeklar-0.1.1/src/WinDeklar/signal_aux.py` & `windeklar-0.1.2/src/WinDeklar/signal_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.1/src/WinDeklar/test_animation.py` & `windeklar-0.1.2/src/WinDeklar/test_animation.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 
 import matplotlib.pyplot as plt
 from matplotlib.animation import FuncAnimation
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from PyQt5.QtWidgets import QApplication, QMainWindow, QVBoxLayout, QWidget
 
-import signal_aux as sg
+import WinDeklar.signal_aux as sg
 
 
 class RealTimeGraph:
     def __init__(self, fig, data_provider, min_x=-1, repeat_length=50, frames=None, interval=100):
         self.repeat_length = repeat_length
         self.data_provider = data_provider if isinstance(data_provider, list) else [data_provider]
```

### Comparing `windeklar-0.1.1/src/WinDeklar/test_pyqt.py` & `windeklar-0.1.2/src/WinDeklar/test_pyqt.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.1/src/WinDeklar/view_animation.py` & `windeklar-0.1.2/src/WinDeklar/view_animation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 import sys
 import numpy as np
 
-import QTAux
-import WindowForm as WinForm
-import graph_aux as ga
+import WinDeklar.QTAux as QTAux
+import WinDeklar.WindowForm as WinForm
+import WinDeklar.graph_aux as ga
 
 
 class ExampleHost(WinForm.HostModel):
     """
     Shows tentacles
     """
```

### Comparing `windeklar-0.1.1/src/WinDeklar/view_animation.yaml` & `windeklar-0.1.2/src/WinDeklar/view_animation.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.1/src/WinDeklar/view_example.py` & `windeklar-0.1.2/src/WinDeklar/view_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 import sys
 import time
 
-import WindowForm as WinForm
-import graph_aux as ga
-import QTAux
+import WinDeklar.WindowForm as WinForm
+import WinDeklar.graph_aux as ga
+import WinDeklar.QTAux as QTAux
 import record as rc
 import yaml_functions
 
 
 class ExampleHost(WinForm.HostModel):
     """
     Example of a Form with many features:
```

### Comparing `windeklar-0.1.1/src/WinDeklar/view_example.yaml` & `windeklar-0.1.2/src/WinDeklar/view_example.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.1/src/WinDeklar/view_simple_graph.py` & `windeklar-0.1.2/src/WinDeklar/view_simple_graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from WindowForm import SimpleFigure
-import graph_aux as ga
+from WinDeklar.WindowForm import SimpleFigure
+import WinDeklar.graph_aux as ga
 
 
 def show_simple_window(title='Sine and Cosine graph', number_of_points=100, size=(5, 2),
                        functions=(('Sine', 'Blue'), ('Cosine', 'Red'))):
     window = SimpleFigure(title=title, size=size, adjust_size=False)
     for [function_name, color] in functions:
         graph_one_function(function_name, window.ax, number_of_points, color)
```

### Comparing `windeklar-0.1.1/src/WinDeklar/yaml_functions.py` & `windeklar-0.1.2/src/WinDeklar/yaml_functions.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.1/LICENSE` & `windeklar-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.1/README.md` & `windeklar-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.1/pyproject.toml` & `windeklar-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name    = "WinDeklar"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Nicolas Jodal", email="jnj@genexus.com" },
 ]
 description = "Create winforms in an easy, declarative way. Specially suited for Robotics applications"
 readme      = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `windeklar-0.1.1/PKG-INFO` & `windeklar-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinDeklar
-Version: 0.1.1
+Version: 0.1.2
 Summary: Create winforms in an easy, declarative way. Specially suited for Robotics applications
 Project-URL: Homepage, https://github.com/njodal/WinDeklar
 Project-URL: Bug Tracker, https://github.com/njodal/WinDeklar/issues
 Author-email: Nicolas Jodal <jnj@genexus.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

