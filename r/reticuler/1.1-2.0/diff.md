# Comparing `tmp/reticuler-1.1.tar.gz` & `tmp/reticuler-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reticuler-1.1.tar", last modified: Thu Jun 22 12:11:00 2023, max compression
+gzip compressed data, was "reticuler-2.0.tar", last modified: Tue Jun 27 15:02:46 2023, max compression
```

## Comparing `reticuler-1.1.tar` & `reticuler-2.0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 12:11:00.457000 reticuler-1.1/
--rw-rw-rw-   0        0        0     1097 2022-11-09 13:08:57.000000 reticuler-1.1/LICENSE
--rw-rw-rw-   0        0        0     2368 2023-06-22 12:11:00.402000 reticuler-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1883 2023-06-22 12:07:52.000000 reticuler-1.1/README.md
--rw-rw-rw-   0        0        0     1112 2023-06-22 12:01:21.000000 reticuler-1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 12:11:00.438000 reticuler-1.1/setup.cfg
--rw-rw-rw-   0        0        0       91 2022-11-02 22:21:50.000000 reticuler-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:10:58.601000 reticuler-1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-22 12:10:58.916000 reticuler-1.1/src/reticuler/
--rw-rw-rw-   0        0        0      100 2023-06-16 08:54:04.000000 reticuler-1.1/src/reticuler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:10:59.571000 reticuler-1.1/src/reticuler/backward_evolution/
--rw-rw-rw-   0        0        0       53 2023-06-16 08:54:04.000000 reticuler-1.1/src/reticuler/backward_evolution/__init__.py
--rw-rw-rw-   0        0        0    19689 2023-06-22 11:27:48.000000 reticuler-1.1/src/reticuler/backward_evolution/system_back.py
--rw-rw-rw-   0        0        0    14065 2023-06-22 11:26:56.000000 reticuler-1.1/src/reticuler/backward_evolution/trimmers.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:10:59.864000 reticuler-1.1/src/reticuler/extending_kernels/
--rw-rw-rw-   0        0        0       93 2022-11-23 12:02:56.000000 reticuler-1.1/src/reticuler/extending_kernels/__init__.py
--rw-rw-rw-   0        0        0     8866 2023-06-16 08:54:04.000000 reticuler-1.1/src/reticuler/extending_kernels/extenders.py
--rw-rw-rw-   0        0        0    17017 2023-06-22 11:23:41.000000 reticuler-1.1/src/reticuler/extending_kernels/pde_solvers.py
--rw-rw-rw-   0        0        0     4980 2023-06-20 18:02:51.000000 reticuler-1.1/src/reticuler/extending_kernels/trajectory_integrators.py
--rw-rw-rw-   0        0        0    26659 2023-06-16 08:54:05.000000 reticuler-1.1/src/reticuler/system.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:11:00.331000 reticuler-1.1/src/reticuler/user_interface/
--rw-rw-rw-   0        0        0       50 2023-06-16 08:54:05.000000 reticuler-1.1/src/reticuler/user_interface/__init__.py
--rw-rw-rw-   0        0        0     4573 2023-06-20 15:51:45.000000 reticuler-1.1/src/reticuler/user_interface/clip_ret.py
--rw-rw-rw-   0        0        0     8719 2023-06-20 20:06:37.000000 reticuler-1.1/src/reticuler/user_interface/clippers.py
--rw-rw-rw-   0        0        0     2313 2023-06-16 08:54:05.000000 reticuler-1.1/src/reticuler/user_interface/graphics.py
--rw-rw-rw-   0        0        0     3574 2023-06-16 08:54:05.000000 reticuler-1.1/src/reticuler/user_interface/plot_ret.py
--rw-rw-rw-   0        0        0     7726 2023-06-16 08:54:05.000000 reticuler-1.1/src/reticuler/user_interface/reticulate.py
--rw-rw-rw-   0        0        0     4633 2023-06-21 10:39:10.000000 reticuler-1.1/src/reticuler/user_interface/reticulate_back.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:10:59.325000 reticuler-1.1/src/reticuler.egg-info/
--rw-rw-rw-   0        0        0     2368 2023-06-22 12:10:58.000000 reticuler-1.1/src/reticuler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      943 2023-06-22 12:10:58.000000 reticuler-1.1/src/reticuler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 12:10:58.000000 reticuler-1.1/src/reticuler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      236 2023-06-22 12:10:58.000000 reticuler-1.1/src/reticuler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2023-06-22 12:10:58.000000 reticuler-1.1/src/reticuler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-22 12:10:58.000000 reticuler-1.1/src/reticuler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 15:02:46.976944 reticuler-2.0/
+-rw-rw-rw-   0        0        0     1097 2022-11-09 13:08:57.000000 reticuler-2.0/LICENSE
+-rw-rw-rw-   0        0        0     2503 2023-06-27 15:02:46.976944 reticuler-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2018 2023-06-23 11:08:42.000000 reticuler-2.0/README.md
+-rw-rw-rw-   0        0        0     1112 2023-06-27 14:58:40.000000 reticuler-2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 15:02:46.976944 reticuler-2.0/setup.cfg
+-rw-rw-rw-   0        0        0       91 2022-11-02 22:21:50.000000 reticuler-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:02:46.898776 reticuler-2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-27 15:02:46.914462 reticuler-2.0/src/reticuler/
+-rw-rw-rw-   0        0        0      100 2023-06-22 12:32:07.000000 reticuler-2.0/src/reticuler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:02:46.945643 reticuler-2.0/src/reticuler/backward_evolution/
+-rw-rw-rw-   0        0        0       53 2023-06-22 12:32:07.000000 reticuler-2.0/src/reticuler/backward_evolution/__init__.py
+-rw-rw-rw-   0        0        0    19691 2023-06-27 14:58:40.000000 reticuler-2.0/src/reticuler/backward_evolution/system_back.py
+-rw-rw-rw-   0        0        0    14065 2023-06-22 12:32:07.000000 reticuler-2.0/src/reticuler/backward_evolution/trimmers.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:02:46.961260 reticuler-2.0/src/reticuler/extending_kernels/
+-rw-rw-rw-   0        0        0       54 2023-06-27 14:58:40.000000 reticuler-2.0/src/reticuler/extending_kernels/__init__.py
+-rw-rw-rw-   0        0        0    22898 2023-06-27 14:58:40.000000 reticuler-2.0/src/reticuler/extending_kernels/extenders.py
+-rw-rw-rw-   0        0        0    36762 2023-06-27 14:58:40.000000 reticuler-2.0/src/reticuler/extending_kernels/pde_solvers.py
+-rw-rw-rw-   0        0        0    28193 2023-06-27 14:58:40.000000 reticuler-2.0/src/reticuler/system.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:02:46.976944 reticuler-2.0/src/reticuler/user_interface/
+-rw-rw-rw-   0        0        0       50 2023-06-22 12:32:07.000000 reticuler-2.0/src/reticuler/user_interface/__init__.py
+-rw-rw-rw-   0        0        0     4573 2023-06-22 12:32:07.000000 reticuler-2.0/src/reticuler/user_interface/clip_ret.py
+-rw-rw-rw-   0        0        0     8719 2023-06-22 12:32:07.000000 reticuler-2.0/src/reticuler/user_interface/clippers.py
+-rw-rw-rw-   0        0        0     2341 2023-06-27 14:58:40.000000 reticuler-2.0/src/reticuler/user_interface/graphics.py
+-rw-rw-rw-   0        0        0     3574 2023-06-22 12:32:07.000000 reticuler-2.0/src/reticuler/user_interface/plot_ret.py
+-rw-rw-rw-   0        0        0     7280 2023-06-27 14:58:40.000000 reticuler-2.0/src/reticuler/user_interface/reticulate.py
+-rw-rw-rw-   0        0        0     4633 2023-06-22 12:32:07.000000 reticuler-2.0/src/reticuler/user_interface/reticulate_back.py
+drwxrwxrwx   0        0        0        0 2023-06-27 15:02:46.945643 reticuler-2.0/src/reticuler.egg-info/
+-rw-rw-rw-   0        0        0     2503 2023-06-27 15:02:46.000000 reticuler-2.0/src/reticuler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      885 2023-06-27 15:02:46.000000 reticuler-2.0/src/reticuler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 15:02:46.000000 reticuler-2.0/src/reticuler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      236 2023-06-27 15:02:46.000000 reticuler-2.0/src/reticuler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2023-06-27 15:02:46.000000 reticuler-2.0/src/reticuler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-27 15:02:46.000000 reticuler-2.0/src/reticuler.egg-info/top_level.txt
```

### Comparing `reticuler-1.1/LICENSE` & `reticuler-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reticuler-1.1/PKG-INFO` & `reticuler-2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reticuler
-Version: 1.1
+Version: 2.0
 Summary: Simulations of spatial networks growth
 Author: Stanisław Żukowski
 Author-email: zukowski.st@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/stzukowski/reticuler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -51,11 +51,12 @@
 - growth threshold type: maximum network height,
 - growth threshold: 2
 ```
 reticulate -out test --growth_params {\"growth_thresh_type\":1,\"growth_thresh\":2}
 ```
 
 ## How to cite
-*Through history to growth dynamics: backward evolution of spatial networks*, S. Żukowski, P. Morawiecki, H. Seybold, P. Szymczak, Sci. Rep. 12, 20407 (2022). https://doi.org/10.1038/s41598-022-24656-x
+[*Through history to growth dynamics: backward evolution of spatial networks*](https://doi.org/10.1038/s41598-022-24656-x), S. Żukowski, P. Morawiecki, H. Seybold, P. Szymczak, Sci. Rep. 12, 20407 (2022).
+[Materials](https://github.com/stzukowski/reticuler/tree/main/archive/papers/2022SciRep)
 
 ### References
-*Bifurcation dynamics of natural drainage networks*,  A. Petroff, O. Devauchelle, H. Seybold, and D. H. Rothman. Philos. Trans. Royal Soc. A 371, no. 2004 (2013): 20120365.
+[*Bifurcation dynamics of natural drainage networks*](https://doi.org/10.1098/rsta.2012.0365),  A. Petroff, O. Devauchelle, H. Seybold, and D. H. Rothman. Philos. Trans. Royal Soc. A 371, no. 2004 (2013): 20120365.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reticuler Version: 1.1 Summary: Simulations of
+Metadata-Version: 2.1 Name: reticuler Version: 2.0 Summary: Simulations of
 spatial networks growth Author: StanisÅaw Å»ukowski Author-email:
 zukowski.st@gmail.com License: MIT Project-URL: Source, https://github.com/
 stzukowski/reticuler Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown License-File: LICENSE # Reticuler
                [PyPI] [Documentation_Status] [Code_style:_black]
@@ -14,13 +14,15 @@
 simulation - *reticulate_back* - runs the the Backward Evolution Algorithm -
 *clip_ret* - clips the network to one of the growth thresholds (maximum forward
 evolution step, length, height, evolution time, or BEA step) - *plot_ret* -
 plots the network based on the *.json* file from the simulation To use just
 type in the command line: `reticulate -h` Typical network growth simulation: -
 output file: *test*, - growth threshold type: maximum network height, - growth
 threshold: 2 ``` reticulate -out test --growth_params {\"growth_thresh_type\":
-1,\"growth_thresh\":2} ``` ## How to cite *Through history to growth dynamics:
-backward evolution of spatial networks*, S. Å»ukowski, P. Morawiecki, H.
-Seybold, P. Szymczak, Sci. Rep. 12, 20407 (2022). https://doi.org/10.1038/
-s41598-022-24656-x ### References *Bifurcation dynamics of natural drainage
-networks*, A. Petroff, O. Devauchelle, H. Seybold, and D. H. Rothman. Philos.
-Trans. Royal Soc. A 371, no. 2004 (2013): 20120365.
+1,\"growth_thresh\":2} ``` ## How to cite [*Through history to growth dynamics:
+backward evolution of spatial networks*](https://doi.org/10.1038/s41598-022-
+24656-x), S. Å»ukowski, P. Morawiecki, H. Seybold, P. Szymczak, Sci. Rep. 12,
+20407 (2022). [Materials](https://github.com/stzukowski/reticuler/tree/main/
+archive/papers/2022SciRep) ### References [*Bifurcation dynamics of natural
+drainage networks*](https://doi.org/10.1098/rsta.2012.0365), A. Petroff, O.
+Devauchelle, H. Seybold, and D. H. Rothman. Philos. Trans. Royal Soc. A 371,
+no. 2004 (2013): 20120365.
```

### Comparing `reticuler-1.1/README.md` & `reticuler-2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -36,11 +36,12 @@
 - growth threshold type: maximum network height,
 - growth threshold: 2
 ```
 reticulate -out test --growth_params {\"growth_thresh_type\":1,\"growth_thresh\":2}
 ```
 
 ## How to cite
-*Through history to growth dynamics: backward evolution of spatial networks*, S. Żukowski, P. Morawiecki, H. Seybold, P. Szymczak, Sci. Rep. 12, 20407 (2022). https://doi.org/10.1038/s41598-022-24656-x
+[*Through history to growth dynamics: backward evolution of spatial networks*](https://doi.org/10.1038/s41598-022-24656-x), S. Żukowski, P. Morawiecki, H. Seybold, P. Szymczak, Sci. Rep. 12, 20407 (2022).
+[Materials](https://github.com/stzukowski/reticuler/tree/main/archive/papers/2022SciRep)
 
 ### References
-*Bifurcation dynamics of natural drainage networks*,  A. Petroff, O. Devauchelle, H. Seybold, and D. H. Rothman. Philos. Trans. Royal Soc. A 371, no. 2004 (2013): 20120365.
+[*Bifurcation dynamics of natural drainage networks*](https://doi.org/10.1098/rsta.2012.0365),  A. Petroff, O. Devauchelle, H. Seybold, and D. H. Rothman. Philos. Trans. Royal Soc. A 371, no. 2004 (2013): 20120365.
```

#### html2text {}

```diff
@@ -8,13 +8,15 @@
 simulation - *reticulate_back* - runs the the Backward Evolution Algorithm -
 *clip_ret* - clips the network to one of the growth thresholds (maximum forward
 evolution step, length, height, evolution time, or BEA step) - *plot_ret* -
 plots the network based on the *.json* file from the simulation To use just
 type in the command line: `reticulate -h` Typical network growth simulation: -
 output file: *test*, - growth threshold type: maximum network height, - growth
 threshold: 2 ``` reticulate -out test --growth_params {\"growth_thresh_type\":
-1,\"growth_thresh\":2} ``` ## How to cite *Through history to growth dynamics:
-backward evolution of spatial networks*, S. Å»ukowski, P. Morawiecki, H.
-Seybold, P. Szymczak, Sci. Rep. 12, 20407 (2022). https://doi.org/10.1038/
-s41598-022-24656-x ### References *Bifurcation dynamics of natural drainage
-networks*, A. Petroff, O. Devauchelle, H. Seybold, and D. H. Rothman. Philos.
-Trans. Royal Soc. A 371, no. 2004 (2013): 20120365.
+1,\"growth_thresh\":2} ``` ## How to cite [*Through history to growth dynamics:
+backward evolution of spatial networks*](https://doi.org/10.1038/s41598-022-
+24656-x), S. Å»ukowski, P. Morawiecki, H. Seybold, P. Szymczak, Sci. Rep. 12,
+20407 (2022). [Materials](https://github.com/stzukowski/reticuler/tree/main/
+archive/papers/2022SciRep) ### References [*Bifurcation dynamics of natural
+drainage networks*](https://doi.org/10.1098/rsta.2012.0365), A. Petroff, O.
+Devauchelle, H. Seybold, and D. H. Rothman. Philos. Trans. Royal Soc. A 371,
+no. 2004 (2013): 20120365.
```

### Comparing `reticuler-1.1/pyproject.toml` & `reticuler-2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]  # list of folders that contain the packages (["."] by default)
 include = ["reticuler*"]  # package names should match these glob patterns (["*"] by default)
 
 [project]
 name = "reticuler"
-version = "1.1"
+version = "2.0"
 authors = [
 	{name="Stanisław Żukowski"},
 	{email="zukowski.st@gmail.com"}
 ]
 description = "Simulations of spatial networks growth"
 readme = "README.md"
 license = { text = "MIT" }
```

### Comparing `reticuler-1.1/src/reticuler/backward_evolution/system_back.py` & `reticuler-2.0/src/reticuler/backward_evolution/system_back.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
         export_backward_branches = { "backward_branches": {**export_backward_branches} }
         
         to_export = export_general | export_trimmer | export_backward_bifurcations | export_backward_branches
         with open(self.exp_name + ".json", "w", encoding="utf-8") as f:
             json.dump(to_export, f, ensure_ascii=False,
                       indent=4, cls=NumpyEncoder)
 
-    def import_branches(self, network):
+    def __import_branches(self, network):
         """Reorganizing and importing branches from the networks.
         
         Parameters
         ----------
         network : Network
 
         Returns
```

### Comparing `reticuler-1.1/src/reticuler/backward_evolution/trimmers.py` & `reticuler-2.0/src/reticuler/backward_evolution/trimmers.py`

 * *Files identical despite different names*

### Comparing `reticuler-1.1/src/reticuler/system.py` & `reticuler-2.0/src/reticuler/system.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,16 +11,22 @@
 import numpy as np
 import datetime
 import time
 import copy
 import json
 import importlib.metadata
 
-from .extending_kernels import extenders, pde_solvers, trajectory_integrators
+from .extending_kernels import extenders, pde_solvers
 
+# Labels for boundary conditions
+DIRICHLET = 1
+NEUMANN = 2
+CONSTANT_FLUX = 3
+RIGHT_WALL_PBC = 999
+LEFT_WALL_PBC = 998
 
 class NumpyEncoder(json.JSONEncoder):
     """Special json encoder for numpy types.
 
     References
     ----------
     .. [1] https://stackoverflow.com/questions/26646362/numpy-array-is-not-json-serializable
@@ -164,17 +170,18 @@
         Parameters
         ----------
         initial_condition : int, default 0
             IC = 0 or 1. Rectangular box of dimensions ``width`` x ``height``,
             absorbing bottom wall, reflecting left and right, and:
                 - IC = 0: constant flux on top (Laplacian case)
                 - IC = 1: reflective top (Poissonian case)
+                - IC = 2: IC=1 + PBC right and left wall
         kwargs_construct:
-            IC = 0 or 1
-                seeds_x : array, default [0.1]
+            IC = 0, 1 or 2
+                seeds_x : array, default [0.5]
                     A 1-n array of x positions at the bottom boundary (y=0).
                 initial_lengths : array, default [0.01]
                     A 1-n array of seeds initial lengths.
                     Length must match seeds_x or be equal to 1 
                     (then the same initial length will be set for all seeds).
                 height : float, default 50.0
                     Height of the rectangular system.
@@ -186,41 +193,38 @@
         box : Box
             An object of class Box.
         branches : list
             A list of objects of class Branch.
 
 
         """
-        # Labels for boundary conditions
-        DIRICHLET = 1
-        NEUMANN = 2
-        CONSTANT_FLUX = 3
-
         # Build a box
         box = cls()
 
         # Rectangular box of specified width and height
         # IC==0: Constant flux on top (Laplace)
         # IC==1: Neumann on top (Poisson)
-        if initial_condition == 0 or initial_condition == 1:
+        if initial_condition == 0 or initial_condition == 1 or initial_condition == 2:
             options_construct = {
-                "seeds_x": [0.1],
+                "seeds_x": [0.5],
                 "initial_lengths": [0.01],
                 "height": 50.0,
                 "width": 2.0,
             }
             options_construct.update(kwargs_construct)
             box.__add_points(
                 [
                     [options_construct["width"], 0],
                     [options_construct["width"], options_construct["height"]],
                     [0, options_construct["height"]],
                     [0, 0],
                 ]
             )
+            
+            # seeds at the boundary
             box.seeds_connectivity = np.column_stack(
                 (
                     len(box.points) +
                     np.arange(len(options_construct["seeds_x"])),
                     np.arange(len(options_construct["seeds_x"])),
                 )
             )
@@ -244,14 +248,18 @@
             )
 
             # right, left, top Neumann:
             box.boundary_conditions[0:3] = NEUMANN
             # or top constant flux:
             if initial_condition == 0:
                 box.boundary_conditions[1] = CONSTANT_FLUX
+            if initial_condition == 2:
+                box.boundary_conditions[1] = CONSTANT_FLUX
+                box.boundary_conditions[0] = RIGHT_WALL_PBC
+                box.boundary_conditions[2] = LEFT_WALL_PBC
 
             # Creating initial branches
             branches = []
             if len(options_construct["initial_lengths"]) == 1:
                 options_construct["initial_lengths"] = (
                     np.ones(len(options_construct["seeds_x"]))
                     * options_construct["initial_lengths"][0]
@@ -387,17 +395,15 @@
     """A class containing all the elements to run a network simulation.
 
     Attributes
     ----------
     network : Network
         An object of class Network.
     extender : Extender
-        An object of one of the classes from reticuler.extending_kernels.extenders.
-    trajectory_integrator : TrajectoryIntegrator
-        One of the classes from reticuler.extending_kernels.trajectory_integrators.
+        One of the classes from reticuler.extending_kernels.extenders.
     growth_thresh_type : int, default 0
         Type of growth threshold.
             - 0: max step
             - 1: height
             - 2: network length
     growth_thresh : float, default 5
         A value of growth threshold. The simulation is stopped, when it's reached.
@@ -410,42 +416,39 @@
 
     """
 
     def __init__(
         self,
         network,
         extender,
-        trajectory_integrator,
         growth_thresh_type=0,
         growth_thresh=5,
         growth_gauges=None,
         dump_every=1,
         exp_name="",
     ):
         """Initialize System.
 
         Parameters
         ----------
         network : Network
-        extender : Extender
-        trajectory_integrator : function
+        extender : function
         growth_gauges : array, default array([0.,0.,0.,0.])
         growth_thresh_type : int, default 0
         growth_thresh : float, default 5
         dump_every : int, default 1
         exp_name: str, default ''
 
         Returns
         -------
         None.
 
         """
         self.network = network
         self.extender = extender
-        self.trajectory_integrator = trajectory_integrator
 
         # Growth limits:
         # 0: max step, 1: max height
         # 2: max length 3: max time
         self.growth_gauges = np.zeros(4) if growth_gauges is None else growth_gauges
         self.growth_thresh_type = growth_thresh_type
         self.growth_thresh = growth_thresh
@@ -473,49 +476,51 @@
                     "network_length": self.growth_gauges[2],
                     "time": self.growth_gauges[3],
                 },
                 "dump_every": self.dump_every,
             },
         }
 
-        if type(self.extender).__name__ == "Streamline":
-            if type(self.trajectory_integrator).__name__ == "ModifiedEulerMethod":
-                export_trajectory_integrator = {
-                    "type": type(self.trajectory_integrator).__name__,
-                    "max_approximation_step": self.trajectory_integrator.max_approximation_step,
-                }
+        if type(self.extender).__name__ == "ModifiedEulerMethod_Streamline" or \
+            type(self.extender).__name__ == "ModifiedEulerMethod_ThickFingers":
             if type(self.extender.pde_solver).__name__ == "FreeFEM":
                 equation_legend = ["Laplace", "Poisson"]
                 export_solver = {
                     "type": type(self.extender.pde_solver).__name__,
                     "equation": equation_legend[self.extender.pde_solver.equation],
                 }
-
-            bifurcation_type_legend = [
-                "no bifurcations", "a1", "a3/a1", "random"]
+                bifurcation_type_legend = [
+                    "no bifurcations", "a1", "a3/a1", "random"]
+            elif type(self.extender.pde_solver).__name__ == "FreeFEM_ThickFingers":
+                equation_legend = ["Laplace", "Poisson"]
+                export_solver = {
+                    "type": type(self.extender.pde_solver).__name__,
+                    "equation": equation_legend[self.extender.pde_solver.equation],
+                    "finger_width": self.extender.pde_solver.finger_width,
+                    "mobility_ratio":self.extender.pde_solver.mobility_ratio,
+                    "n_adapt": self.extender.pde_solver.n_adapt,
+                }
+                bifurcation_type_legend = [
+                    "no bifurcations", "a1", "random"]
             export_extender = {
-                "type": type(self.extender).__name__,
-                "eta": self.extender.eta,
-                "ds": self.extender.ds,
-                "bifurcations": {
-                    "type": bifurcation_type_legend[
-                        self.extender.bifurcation_type
-                    ],
-                    "threshold": self.extender.bifurcation_thresh,
-                    "angle": self.extender.bifurcation_angle,
-                },
-                "inflow_thresh": self.extender.inflow_thresh,
-                "distance_from_bif_thresh": self.extender.distance_from_bif_thresh,
-                "pde_solver": {**export_solver},
-            }
-
-            export_extending_kernel = {
-                "extending_kernel": {
-                    "trajectory_integrator": {**export_trajectory_integrator},
-                    "extender": {**export_extender},
+                "extender": {
+                    "type": type(self.extender).__name__,
+                    "eta": self.extender.eta,
+                    "ds": self.extender.ds,
+                    "bifurcations": {
+                        "type": bifurcation_type_legend[
+                            self.extender.bifurcation_type
+                        ],
+                        "threshold": self.extender.bifurcation_thresh,
+                        "angle": self.extender.bifurcation_angle,
+                    },
+                    "inflow_thresh": self.extender.inflow_thresh,
+                    "distance_from_bif_thresh": self.extender.distance_from_bif_thresh,
+                    "max_approximation_step": self.extender.max_approximation_step,
+                    "pde_solver": {**export_solver},
                 }
             }
 
         export_branches = {}
         for branch in self.network.branches[::-1]:
             if branch in self.network.active_branches:
                 state = "active"
@@ -541,15 +546,15 @@
                     "seeds_connectivity": self.network.box.seeds_connectivity,
                 },
                 "branch_connectivity": self.network.branch_connectivity,
                 "branches": {**export_branches},
             }
         }
 
-        to_export = export_general | export_extending_kernel | export_network
+        to_export = export_general | export_extender | export_network
         with open(self.exp_name + ".json", "w", encoding="utf-8") as f:
             json.dump(to_export, f, ensure_ascii=False,
                       indent=4, cls=NumpyEncoder)
 
     @classmethod
     def import_json(cls, input_file):
         """Construct an instance of class System based on the imported .json file.
@@ -602,50 +607,58 @@
             box=box,
             branches=branches,
             active_branches=active_branches,
             sleeping_branches=sleeping_branches,
             branch_connectivity=branch_connectivity,
         )
 
-        # Trajectory integrator
-        json_trajectory_integrator = json_load["extending_kernel"][
-            "trajectory_integrator"
-        ]
-        if json_trajectory_integrator["type"] == "ModifiedEulerMethod":
-            max_approximation_step = json_trajectory_integrator["max_approximation_step"]
-            trajectory_integrator = trajectory_integrators.ModifiedEulerMethod(
-                max_approximation_step=max_approximation_step)
-
+        # try:
         # Solver
-        json_solver = json_load["extending_kernel"]["extender"]["pde_solver"]
+        json_solver = json_load["extender"]["pde_solver"]
         if json_solver["type"] == "FreeFEM":
             equation_legend = ["Laplace", "Poisson"]
             equation = equation_legend.index(json_solver["equation"])
-            pde_solver = pde_solvers.FreeFEM(equation=equation)
-
+            pde_solver = pde_solvers.FreeFEM(network, equation=equation)
+        elif json_solver["type"] == "FreeFEM_ThickFingers":
+            equation_legend = ["Laplace", "Poisson"]
+            equation = equation_legend.index(json_solver["equation"])
+            pde_solver = pde_solvers.FreeFEM_ThickFingers(network, 
+                                             equation=equation,
+                                             finger_width=json_solver["finger_width"],
+                                             mobility_ratio=json_solver["mobility_ratio"], 
+                                             n_adapt=json_solver["n_adapt"],
+                                             )
         # Extender
-        json_extender = json_load["extending_kernel"]["extender"]
-        if json_extender["type"] == "Streamline":
+        json_extender = json_load["extender"]
+        if json_extender["type"] == "ModifiedEulerMethod_Streamline" or \
+            json_extender["type"] == "ModifiedEulerMethod_ThickFingers":
+                
+            if json_extender["type"] == "ModifiedEulerMethod_Streamline":
+                bifurcation_type_legend = [
+                    "no bifurcations", "a1", "a3/a1", "random"]
+                extender_class = extenders.ModifiedEulerMethod_Streamline
+            elif json_extender["type"] == "ModifiedEulerMethod_ThickFingers":
+                bifurcation_type_legend = [
+                    "no bifurcations", "a1", "random"]
+                extender_class = extenders.ModifiedEulerMethod_ThickFingers
+                
             json_bifurcation = json_extender["bifurcations"]
-            bifurcation_type_legend = [
-                "no bifurcations", "a1", "a3/a1", "random"]
             bifurcation_type = bifurcation_type_legend.index(
                 json_bifurcation["type"])
-            extender = extenders.Streamline(
+            extender = extender_class(
                 pde_solver=pde_solver,
                 eta=json_extender["eta"],
                 ds=json_extender["ds"],
                 bifurcation_type=bifurcation_type,
                 bifurcation_thresh=json_bifurcation["threshold"],
                 bifurcation_angle=json_bifurcation["angle"],
                 inflow_thresh=json_extender["inflow_thresh"],
-            )
-            extender.distance_from_bif_thresh = json_extender[
-                "distance_from_bif_thresh"
-            ]
+                distance_from_bif_thresh=json_extender["distance_from_bif_thresh"],
+                max_approximation_step=json_extender["max_approximation_step"],
+            )          
 
         # General
         json_growth = json_load["growth"]
         growth_type_legend = ["max step",
                               "max height", "max length", "max time"]
         growth_thresh_type = growth_type_legend.index(
             json_growth["threshold_type"])
@@ -661,21 +674,30 @@
                 json_growth_gauges["time"],
             ]
         )
 
         system = cls(
             network=network,
             extender=extender,
-            trajectory_integrator=trajectory_integrator,
             growth_gauges=growth_gauges,
             growth_thresh_type=growth_thresh_type,
             growth_thresh=growth_thresh,
             dump_every=dump_every,
             exp_name=input_file,
         )
+        # except:
+        #     print("!WARNING! Error during importing - only ``network`` imported!")
+        #     pde_solver = pde_solvers.FreeFEM(network)
+        #     extender = extenders.ModifiedEulerMethod_Streamline(
+        #         pde_solver=pde_solver,)
+        #     system = cls(
+        #         network=network,
+        #         extender=extender,
+        #         exp_name=input_file,
+        #     )
 
         return system
 
     def __update_growth_gauges(self, dt):
         """Update growth gauges."""
         self.growth_gauges[1], self.growth_gauges[2] = self.network.height_and_length(
         )
@@ -708,18 +730,17 @@
             print(
                 "\n-------------------   Growth step: {step:.0f}   -------------------\n".format(
                     step=self.growth_gauges[0]
                 )
             )
             print("Date and time: ", datetime.datetime.now())
 
-            dt, _ = self.trajectory_integrator.integrate(
-                extender=self.extender, network=self.network)
+            out_growth = self.extender.integrate(network=self.network)
             self.network.move_tips(step=self.growth_gauges[0])
-            self.__update_growth_gauges(dt)
+            self.__update_growth_gauges(out_growth[0])
 
             if not self.growth_gauges[0] % self.dump_every:
                 self.export_json()
 
         self.export_json()
 
         print(
```

### Comparing `reticuler-1.1/src/reticuler/user_interface/clip_ret.py` & `reticuler-2.0/src/reticuler/user_interface/clip_ret.py`

 * *Files identical despite different names*

### Comparing `reticuler-1.1/src/reticuler/user_interface/clippers.py` & `reticuler-2.0/src/reticuler/user_interface/clippers.py`

 * *Files identical despite different names*

### Comparing `reticuler-1.1/src/reticuler/user_interface/graphics.py` & `reticuler-2.0/src/reticuler/user_interface/graphics.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,30 +50,31 @@
         Arguments to plot the tree.
 
     Returns
     -------
     None.
 
     """
-    options_tree_plot = {"color": "#0066CC", "linewidth": 2.5}
+    options_tree_plot = {"color": "#0066CC", "linewidth": 1.25}
     options_tree_plot.update(kwargs_tree_plot)
 
     # PLOT LINES
     y_max = 2
     for branch in network.branches:
         line = branch.points
-        y_max = np.max((np.max(line[:, 1]), y_max))
+        if np.max(line[:, 1]) > y_max:
+            y_max = 1.05*np.max(line[:, 1])
         ax.plot(*line.T, **options_tree_plot)
     # PLOT BOX
     points_to_plot = network.box.points[network.box.connections]
     for pts in points_to_plot:
         ax.plot(*pts.T, linewidth=options_tree_plot["linewidth"] * 2, color="0")
 
     ax.axis("off")
     # colouring background
     ax.add_artist(ax.patch)
     ax.patch.set_zorder(-1)
     ax.set_facecolor("#def1ff")
     ax.set_aspect("equal")
     ax.set_xlim(0, xlim)
-    ylim = 1.05*y_max if ylim is None else ylim
+    ylim = y_max if ylim is None else ylim
     ax.set_ylim(0, ylim)
```

### Comparing `reticuler-1.1/src/reticuler/user_interface/plot_ret.py` & `reticuler-2.0/src/reticuler/user_interface/plot_ret.py`

 * *Files identical despite different names*

### Comparing `reticuler-1.1/src/reticuler/user_interface/reticulate.py` & `reticuler-2.0/src/reticuler/user_interface/reticulate.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 import json
 import textwrap
 import importlib.metadata
 import matplotlib.pyplot as plt
 
 from reticuler.system import Box, Network, System
-from reticuler.extending_kernels import extenders, pde_solvers, trajectory_integrators
+from reticuler.extending_kernels import extenders, pde_solvers
 from reticuler.user_interface import graphics
 
 # %%
 def main():
     parser = argparse.ArgumentParser(
         description="Grow a network.", formatter_class=argparse.RawTextHelpFormatter
     )
@@ -115,28 +115,14 @@
                 Box.construct.__doc__.find("kwargs_construct")
                 - 8 : Box.construct.__doc__.find("Returns")
             ]
         ),
         default=[{}],
     )
 
-    # Trajectory integrator
-    parser.add_argument(
-        "--trajectory_integrator",
-        type=str,
-        nargs=1,
-        metavar="name",
-        help=textwrap.dedent(
-            """\
-            Trajectory integrator
-            default = ModifiedEulerMethod"""
-        ),
-        default=["ModifiedEulerMethod"],
-    )
-
     # Solver
     parser.add_argument(
         "--pde_solver",
         type=str,
         nargs=1,
         metavar="name",
         help=textwrap.dedent(
@@ -177,17 +163,17 @@
         "--extender",
         type=str,
         nargs=1,
         metavar="name",
         help=textwrap.dedent(
             """\
             Extender
-            default = Streamline"""
+            default = ModifiedEulerMethod_Streamline"""
         ),
-        default=["Streamline"],
+        default=["ModifiedEulerMethod_Streamline"],
     )
     parser.add_argument(
         "--extender_params",
         type=json.loads,
         nargs=1,
         metavar="dict",
         help=textwrap.dedent(
@@ -197,19 +183,19 @@
             Pass dictionary in a form (no spaces, 
             backslash before quotes around `value`): 
                 "{\"value\":key}"
             default = {} (keeps default values as listed below)
             
             """
         )
-        + "1. Streamline\n"
+        + "1. ModifiedEulerMethod_Streamline\n"
         + textwrap.dedent(
-            extenders.Streamline.__doc__[
-                extenders.Streamline.__doc__.find("eta")
-                - 4 : extenders.Streamline.__doc__.find("References")
+            extenders.ModifiedEulerMethod_Streamline.__doc__[
+                extenders.ModifiedEulerMethod_Streamline.__doc__.find("eta")
+                - 4 : extenders.ModifiedEulerMethod_Streamline.__doc__.find("References")
             ]
         ),
         default=[{}],
     )
 
     # Plotting at the end
     parser.add_argument(
@@ -233,33 +219,27 @@
         box, branches = Box.construct(
             initial_condition=args.initial_condition[0], **args.kwargs_box[0]
         )
 
         # Network
         network = Network(box=box, branches=branches, active_branches=branches.copy())
 
-        # Trajectory integrator
-        if args.trajectory_integrator[0] == "ModifiedEulerMethod":
-            trajectory_integrator = trajectory_integrators.ModifiedEulerMethod()
-
         # Solver
         if args.pde_solver[0] == "FreeFEM":
-            pde_solver = pde_solvers.FreeFEM(**args.pde_solver_params[0])
-
+            pde_solver = pde_solvers.FreeFEM(network, **args.pde_solver_params[0])
         # Extender
-        if args.extender[0] == "Streamline":
-            extender = extenders.Streamline(
+        if args.extender[0] == "ModifiedEulerMethod_Streamline":
+            extender = extenders.ModifiedEulerMethod_Streamline(
                 pde_solver=pde_solver, **args.extender_params[0]
             )
 
         # General
         system = System(
             network=network,
             extender=extender,
-            trajectory_integrator=trajectory_integrator,
             exp_name=args.output_file[0],
             **args.growth_params[0]
         )
 
     else:
         # Import System from JSON file
         system = System.import_json(input_file=args.input_file[0])
```

### Comparing `reticuler-1.1/src/reticuler/user_interface/reticulate_back.py` & `reticuler-2.0/src/reticuler/user_interface/reticulate_back.py`

 * *Files identical despite different names*

### Comparing `reticuler-1.1/src/reticuler.egg-info/PKG-INFO` & `reticuler-2.0/src/reticuler.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reticuler
-Version: 1.1
+Version: 2.0
 Summary: Simulations of spatial networks growth
 Author: Stanisław Żukowski
 Author-email: zukowski.st@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/stzukowski/reticuler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -51,11 +51,12 @@
 - growth threshold type: maximum network height,
 - growth threshold: 2
 ```
 reticulate -out test --growth_params {\"growth_thresh_type\":1,\"growth_thresh\":2}
 ```
 
 ## How to cite
-*Through history to growth dynamics: backward evolution of spatial networks*, S. Żukowski, P. Morawiecki, H. Seybold, P. Szymczak, Sci. Rep. 12, 20407 (2022). https://doi.org/10.1038/s41598-022-24656-x
+[*Through history to growth dynamics: backward evolution of spatial networks*](https://doi.org/10.1038/s41598-022-24656-x), S. Żukowski, P. Morawiecki, H. Seybold, P. Szymczak, Sci. Rep. 12, 20407 (2022).
+[Materials](https://github.com/stzukowski/reticuler/tree/main/archive/papers/2022SciRep)
 
 ### References
-*Bifurcation dynamics of natural drainage networks*,  A. Petroff, O. Devauchelle, H. Seybold, and D. H. Rothman. Philos. Trans. Royal Soc. A 371, no. 2004 (2013): 20120365.
+[*Bifurcation dynamics of natural drainage networks*](https://doi.org/10.1098/rsta.2012.0365),  A. Petroff, O. Devauchelle, H. Seybold, and D. H. Rothman. Philos. Trans. Royal Soc. A 371, no. 2004 (2013): 20120365.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reticuler Version: 1.1 Summary: Simulations of
+Metadata-Version: 2.1 Name: reticuler Version: 2.0 Summary: Simulations of
 spatial networks growth Author: StanisÅaw Å»ukowski Author-email:
 zukowski.st@gmail.com License: MIT Project-URL: Source, https://github.com/
 stzukowski/reticuler Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown License-File: LICENSE # Reticuler
                [PyPI] [Documentation_Status] [Code_style:_black]
@@ -14,13 +14,15 @@
 simulation - *reticulate_back* - runs the the Backward Evolution Algorithm -
 *clip_ret* - clips the network to one of the growth thresholds (maximum forward
 evolution step, length, height, evolution time, or BEA step) - *plot_ret* -
 plots the network based on the *.json* file from the simulation To use just
 type in the command line: `reticulate -h` Typical network growth simulation: -
 output file: *test*, - growth threshold type: maximum network height, - growth
 threshold: 2 ``` reticulate -out test --growth_params {\"growth_thresh_type\":
-1,\"growth_thresh\":2} ``` ## How to cite *Through history to growth dynamics:
-backward evolution of spatial networks*, S. Å»ukowski, P. Morawiecki, H.
-Seybold, P. Szymczak, Sci. Rep. 12, 20407 (2022). https://doi.org/10.1038/
-s41598-022-24656-x ### References *Bifurcation dynamics of natural drainage
-networks*, A. Petroff, O. Devauchelle, H. Seybold, and D. H. Rothman. Philos.
-Trans. Royal Soc. A 371, no. 2004 (2013): 20120365.
+1,\"growth_thresh\":2} ``` ## How to cite [*Through history to growth dynamics:
+backward evolution of spatial networks*](https://doi.org/10.1038/s41598-022-
+24656-x), S. Å»ukowski, P. Morawiecki, H. Seybold, P. Szymczak, Sci. Rep. 12,
+20407 (2022). [Materials](https://github.com/stzukowski/reticuler/tree/main/
+archive/papers/2022SciRep) ### References [*Bifurcation dynamics of natural
+drainage networks*](https://doi.org/10.1098/rsta.2012.0365), A. Petroff, O.
+Devauchelle, H. Seybold, and D. H. Rothman. Philos. Trans. Royal Soc. A 371,
+no. 2004 (2013): 20120365.
```

### Comparing `reticuler-1.1/src/reticuler.egg-info/SOURCES.txt` & `reticuler-2.0/src/reticuler.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 src/reticuler.egg-info/top_level.txt
 src/reticuler/backward_evolution/__init__.py
 src/reticuler/backward_evolution/system_back.py
 src/reticuler/backward_evolution/trimmers.py
 src/reticuler/extending_kernels/__init__.py
 src/reticuler/extending_kernels/extenders.py
 src/reticuler/extending_kernels/pde_solvers.py
-src/reticuler/extending_kernels/trajectory_integrators.py
 src/reticuler/user_interface/__init__.py
 src/reticuler/user_interface/clip_ret.py
 src/reticuler/user_interface/clippers.py
 src/reticuler/user_interface/graphics.py
 src/reticuler/user_interface/plot_ret.py
 src/reticuler/user_interface/reticulate.py
 src/reticuler/user_interface/reticulate_back.py
```

