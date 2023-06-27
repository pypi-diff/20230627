# Comparing `tmp/windeklar-0.1.3.tar.gz` & `tmp/windeklar-0.1.4.tar.gz`

## Comparing `windeklar-0.1.3.tar` & `windeklar-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.1.3/requirements.txt
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.1.3/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.1.3/.idea/.gitignore
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.1.3/.idea/.name
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.1.3/.idea/WinDeklar.iml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.1.3/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.1.3/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.1.3/.idea/vcs.xml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.1.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.1.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/__init__.py
--rwxr-xr-x   0        0        0    15884 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/QTAux.py
--rw-r--r--   0        0        0    42995 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/WindowForm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/__init__.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/graph_aux.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/points_box.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/record.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/signal_aux.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/test_animation.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/test_pyqt.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/view_animation.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/view_animation.yaml
--rw-r--r--   0        0        0     5864 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/view_example.py
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/view_example.yaml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/view_simple_graph.py
--rwxr-xr-x   0        0        0     6347 2020-02-02 00:00:00.000000 windeklar-0.1.3/src/WinDeklar/yaml_functions.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.1.3/LICENSE
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 windeklar-0.1.3/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 windeklar-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.1.4/requirements.txt
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.1.4/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.1.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.1.4/.idea/.gitignore
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.1.4/.idea/.name
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.1.4/.idea/WinDeklar.iml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.1.4/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.1.4/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.1.4/.idea/vcs.xml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.1.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.1.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1.4/src/__init__.py
+-rwxr-xr-x   0        0        0    15884 2020-02-02 00:00:00.000000 windeklar-0.1.4/src/WinDeklar/QTAux.py
+-rw-r--r--   0        0        0    43182 2020-02-02 00:00:00.000000 windeklar-0.1.4/src/WinDeklar/WindowForm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.1.4/src/WinDeklar/__init__.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 windeklar-0.1.4/src/WinDeklar/graph_aux.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.1.4/src/WinDeklar/points_box.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.1.4/src/WinDeklar/record.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.1.4/src/WinDeklar/signal_aux.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.1.4/src/WinDeklar/test_animation.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.1.4/src/WinDeklar/test_pyqt.py
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 windeklar-0.1.4/src/WinDeklar/view_animation.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 windeklar-0.1.4/src/WinDeklar/view_animation.yaml
+-rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 windeklar-0.1.4/src/WinDeklar/view_example.py
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 windeklar-0.1.4/src/WinDeklar/view_example.yaml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.1.4/src/WinDeklar/view_simple_graph.py
+-rwxr-xr-x   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.1.4/src/WinDeklar/yaml_functions.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 windeklar-0.1.4/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 windeklar-0.1.4/PKG-INFO
```

### Comparing `windeklar-0.1.3/.github/workflows/python-publish.yml` & `windeklar-0.1.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.3/.idea/inspectionProfiles/Project_Default.xml` & `windeklar-0.1.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.3/src/WinDeklar/QTAux.py` & `windeklar-0.1.4/src/WinDeklar/QTAux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.3/src/WinDeklar/WindowForm.py` & `windeklar-0.1.4/src/WinDeklar/WindowForm.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 import WinDeklar.points_box as pb
 import WinDeklar.QTAux as QTAux
 import WinDeklar.record as rc
 import WinDeklar.signal_aux as sg
 import WinDeklar.yaml_functions as yaml
 
 
+def set_winform(file_path, provider, ext='yaml'):
+    win_config_name = yaml.get_file_name_with_other_extension(file_path, ext)
+    return ConfigurableWindow(win_config_name, provider)
+
+
 class ConfigurableWindow(QtWidgets.QMainWindow):
     """
     Defines a Window with many components inside in a declarative manner in a config file
     Notes:
         - a config_file_name is a yaml that has the definition (see view_map.yaml)
         - a typical windows has some controls in the left and a Figure in the right (like an ego view or a map)
     """
```

### Comparing `windeklar-0.1.3/src/WinDeklar/graph_aux.py` & `windeklar-0.1.4/src/WinDeklar/graph_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.3/src/WinDeklar/points_box.py` & `windeklar-0.1.4/src/WinDeklar/points_box.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.3/src/WinDeklar/record.py` & `windeklar-0.1.4/src/WinDeklar/record.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.3/src/WinDeklar/signal_aux.py` & `windeklar-0.1.4/src/WinDeklar/signal_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.3/src/WinDeklar/test_animation.py` & `windeklar-0.1.4/src/WinDeklar/test_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.3/src/WinDeklar/test_pyqt.py` & `windeklar-0.1.4/src/WinDeklar/test_pyqt.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.3/src/WinDeklar/view_animation.py` & `windeklar-0.1.4/src/WinDeklar/view_animation.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,11 +56,10 @@
             self.start_animation()
             self.set_control_title(self.start_stop_key, 'Pause Animation')
             self.set_control_title(self.start_stop_action_key, 'Pause Animation')
 
 
 if __name__ == '__main__':
     app = QTAux.def_app()
-    win_config_name = 'view_animation.yaml'  # window definition
-    provider        = ExampleHost()        # class to handle events
-    myGUI           = WinForm.ConfigurableWindow(win_config_name, provider)
+    provider = ExampleHost()        # class to handle events
+    WinForm.set_winform(__file__, provider)
     sys.exit(app.exec_())
```

### Comparing `windeklar-0.1.3/src/WinDeklar/view_animation.yaml` & `windeklar-0.1.4/src/WinDeklar/view_animation.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.3/src/WinDeklar/view_example.py` & `windeklar-0.1.4/src/WinDeklar/view_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,11 +151,10 @@
     for i in range(0, max_value, inc):
         progress_bar.set_value(i)
         time.sleep(sleep_time)
 
 
 if __name__ == '__main__':
     app = QTAux.def_app()
-    win_config_name = 'view_example.yaml'  # window definition
-    provider        = ExampleHost()        # class to handle events
-    myGUI           = WinForm.ConfigurableWindow(win_config_name, provider)
+    provider = ExampleHost()        # class to handle events
+    WinForm.set_winform(__file__, provider)
     sys.exit(app.exec_())
```

### Comparing `windeklar-0.1.3/src/WinDeklar/view_example.yaml` & `windeklar-0.1.4/src/WinDeklar/view_example.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.3/src/WinDeklar/view_simple_graph.py` & `windeklar-0.1.4/src/WinDeklar/view_simple_graph.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.3/src/WinDeklar/yaml_functions.py` & `windeklar-0.1.4/src/WinDeklar/yaml_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -188,7 +188,14 @@
 def directory_path(file_name):
     """
     Returns the directory path of a full file name
     :param file_name:
     :return:
     """
     return os.path.dirname(file_name)
+
+
+def get_file_name_with_other_extension(file_path, ext='yaml'):
+    dir_name      = os.path.dirname(os.path.abspath(file_path))
+    base_name     = file_name_without_extension(os.path.basename(file_path))
+    new_file_name = '%s/%s.%s' % (dir_name, base_name, ext)
+    return new_file_name
```

### Comparing `windeklar-0.1.3/LICENSE` & `windeklar-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.3/README.md` & `windeklar-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `windeklar-0.1.3/pyproject.toml` & `windeklar-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name    = "WinDeklar"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Nicolas Jodal", email="jnj@genexus.com" },
 ]
 description = "Create winforms in an easy, declarative way. Specially suited for Robotics applications"
 readme      = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `windeklar-0.1.3/PKG-INFO` & `windeklar-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinDeklar
-Version: 0.1.3
+Version: 0.1.4
 Summary: Create winforms in an easy, declarative way. Specially suited for Robotics applications
 Project-URL: Homepage, https://github.com/njodal/WinDeklar
 Project-URL: Bug Tracker, https://github.com/njodal/WinDeklar/issues
 Author-email: Nicolas Jodal <jnj@genexus.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

