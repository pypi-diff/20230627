# Comparing `tmp/manim_lamination_builder-0.2.6.tar.gz` & `tmp/manim_lamination_builder-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_lamination_builder-0.2.6.tar", last modified: Wed May 17 21:22:35 2023, max compression
+gzip compressed data, was "manim_lamination_builder-0.2.7.tar", last modified: Tue Jun 27 19:52:45 2023, max compression
```

## Comparing `manim_lamination_builder-0.2.6.tar` & `manim_lamination_builder-0.2.7.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-17 21:22:35.308981 manim_lamination_builder-0.2.6/
--rw-r--r--   0 forrest   (1000) forrest   (1000)    34523 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.6/LICENSE
--rw-r--r--   0 forrest   (1000) forrest   (1000)    43957 2023-05-17 21:22:35.308981 manim_lamination_builder-0.2.6/PKG-INFO
--rw-r--r--   0 forrest   (1000) forrest   (1000)     3590 2023-05-17 01:50:11.000000 manim_lamination_builder-0.2.6/README.md
-drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-17 21:22:35.308981 manim_lamination_builder-0.2.6/manim_lamination_builder/
--rw-r--r--   0 forrest   (1000) forrest   (1000)     1054 2023-05-17 21:22:09.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/__init__.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)      423 2023-05-16 01:05:30.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/__main__.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     4412 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/animation.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     3132 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/chord.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     2846 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/custom_json.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     4398 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/generate.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     3470 2023-05-14 20:26:30.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/lamination.py
--rwxr-xr-x   0 forrest   (1000) forrest   (1000)     1144 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/main.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     4464 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/morph.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     6826 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.6/manim_lamination_builder/points.py
-drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-05-17 21:22:35.308981 manim_lamination_builder-0.2.6/manim_lamination_builder.egg-info/
--rw-r--r--   0 forrest   (1000) forrest   (1000)    43957 2023-05-17 21:22:35.000000 manim_lamination_builder-0.2.6/manim_lamination_builder.egg-info/PKG-INFO
--rw-r--r--   0 forrest   (1000) forrest   (1000)      635 2023-05-17 21:22:35.000000 manim_lamination_builder-0.2.6/manim_lamination_builder.egg-info/SOURCES.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)        1 2023-05-17 21:22:35.000000 manim_lamination_builder-0.2.6/manim_lamination_builder.egg-info/dependency_links.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)       12 2023-05-17 21:22:35.000000 manim_lamination_builder-0.2.6/manim_lamination_builder.egg-info/requires.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)       25 2023-05-17 21:22:35.000000 manim_lamination_builder-0.2.6/manim_lamination_builder.egg-info/top_level.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)      693 2023-05-17 21:22:29.000000 manim_lamination_builder-0.2.6/pyproject.toml
--rw-r--r--   0 forrest   (1000) forrest   (1000)       38 2023-05-17 21:22:35.308981 manim_lamination_builder-0.2.6/setup.cfg
+drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-06-27 19:52:45.280686 manim_lamination_builder-0.2.7/
+-rw-r--r--   0 forrest   (1000) forrest   (1000)    34523 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.7/LICENSE
+-rw-r--r--   0 forrest   (1000) forrest   (1000)    43957 2023-06-27 19:52:45.280686 manim_lamination_builder-0.2.7/PKG-INFO
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     3590 2023-05-17 01:50:11.000000 manim_lamination_builder-0.2.7/README.md
+drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-06-27 19:52:45.277353 manim_lamination_builder-0.2.7/manim_lamination_builder/
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     1054 2023-05-17 21:22:09.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/__init__.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)      506 2023-05-17 21:59:01.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/__main__.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     4412 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/animation.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     3132 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/chord.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     2846 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/custom_json.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     4443 2023-06-21 01:11:35.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/generate.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     3470 2023-05-14 20:26:30.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/lamination.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     2035 2023-06-13 23:38:46.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/leaf_polygon_conversion.py
+-rwxr-xr-x   0 forrest   (1000) forrest   (1000)     1144 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/main.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     4225 2023-06-20 23:53:08.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/morph.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     1039 2023-06-19 18:18:30.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/new_generate.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     6900 2023-06-13 21:43:04.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/points.py
+drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-06-27 19:52:45.280686 manim_lamination_builder-0.2.7/manim_lamination_builder.egg-info/
+-rw-r--r--   0 forrest   (1000) forrest   (1000)    43957 2023-06-27 19:52:45.000000 manim_lamination_builder-0.2.7/manim_lamination_builder.egg-info/PKG-INFO
+-rw-r--r--   0 forrest   (1000) forrest   (1000)      728 2023-06-27 19:52:45.000000 manim_lamination_builder-0.2.7/manim_lamination_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)        1 2023-06-27 19:52:45.000000 manim_lamination_builder-0.2.7/manim_lamination_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)       12 2023-06-27 19:52:45.000000 manim_lamination_builder-0.2.7/manim_lamination_builder.egg-info/requires.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)       25 2023-06-27 19:52:45.000000 manim_lamination_builder-0.2.7/manim_lamination_builder.egg-info/top_level.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)      693 2023-06-27 19:44:53.000000 manim_lamination_builder-0.2.7/pyproject.toml
+-rw-r--r--   0 forrest   (1000) forrest   (1000)       38 2023-06-27 19:52:45.280686 manim_lamination_builder-0.2.7/setup.cfg
```

### Comparing `manim_lamination_builder-0.2.6/LICENSE` & `manim_lamination_builder-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.6/PKG-INFO` & `manim_lamination_builder-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim_lamination_builder
-Version: 0.2.6
+Version: 0.2.7
 Summary: a replacement to lamination builder that uses manim instead of the browser
 Author-email: Forrest Hilton <forrestmhilton@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `manim_lamination_builder-0.2.6/README.md` & `manim_lamination_builder-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.6/manim_lamination_builder/__init__.py` & `manim_lamination_builder-0.2.7/manim_lamination_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.6/manim_lamination_builder/animation.py` & `manim_lamination_builder-0.2.7/manim_lamination_builder/animation.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.6/manim_lamination_builder/chord.py` & `manim_lamination_builder-0.2.7/manim_lamination_builder/chord.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.6/manim_lamination_builder/custom_json.py` & `manim_lamination_builder-0.2.7/manim_lamination_builder/custom_json.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.6/manim_lamination_builder/generate.py` & `manim_lamination_builder-0.2.7/manim_lamination_builder/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,18 +67,19 @@
     def colorize(p: UnitPoint) -> Colors:
         colors = [
             Colors.pure_red,
             Colors.pure_green,
             Colors.pure_blue,
             Colors.yellow,
             Colors.purple,
-            Colors.black,
         ]
         x = p.after_sigma().cleared()
         if x in image:
+            if image.index(x) > 5:
+                return Colors.black
             return colors[image.index(x)]
         return Colors.black
 
     return colorize
 
 
 def generate_sibling_portraits(original_shape: List[NaryFraction]) -> List[Lamination]:
```

### Comparing `manim_lamination_builder-0.2.6/manim_lamination_builder/lamination.py` & `manim_lamination_builder-0.2.7/manim_lamination_builder/lamination.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.6/manim_lamination_builder/main.py` & `manim_lamination_builder-0.2.7/manim_lamination_builder/main.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.6/manim_lamination_builder/morph.py` & `manim_lamination_builder-0.2.7/manim_lamination_builder/morph.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,16 @@
         return ((x - b) / remaining_length) + midpoint
 
 
 def result(lam: Lamination) -> Lamination:
     assert lam.occlusion is not None
     remaining_degree = lam.radix
     if (
-        lam.occlusion[0].has_degree() and lam.occlusion[1].has_degree()
+        lam.occlusion[0].has_degree()
+        and lam.occlusion[1].has_degree()
         and lam.occlusion[0].after_sigma().cleared()
         == lam.occlusion[1].after_sigma().cleared()
     ):
         lost_criticalitys = int(
             lam.occlusion[1].after_sigma().to_float()
             - lam.occlusion[0].after_sigma().to_float()
         )
@@ -71,23 +72,16 @@
         return FloatWrapper(
             morph_function(p.to_float(), lam.occlusion), remaining_degree
         )
 
     ret = remove_occluded(lam, occlusion=lam.occlusion).apply_function(mapping)
 
     ret.occlusion = None
-
     ret.radix = remaining_degree
-
-    destination_points = []
-    for point in ret.points:  # ordered set with non-hash based equality?
-        image = point.after_sigma().cleared()
-        if image not in destination_points:
-            destination_points.append(image)
-    ret.colorizer = curried_colorize_with_respect_to(destination_points)
+    ret.colorizer = curried_colorize_with_respect_to(ret.points)
 
     return ret
 
 
 class MorphOcclusion(AnimateLamination):
     def __init__(
         self,
```

### Comparing `manim_lamination_builder-0.2.6/manim_lamination_builder/points.py` & `manim_lamination_builder-0.2.7/manim_lamination_builder/points.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Licensed under the The AGPLv3 License (AGPLv3)
 # Copyright (c) 2023 Forrest M. Hilton <forrestmhilton@gmail.com>
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from typing import List
 
-from math import cos, pi, sin
+from math import cos, pi, sin, floor
 
 from manim.animation.animation import deepcopy
 from abc import ABC, abstractmethod
 import numpy as np
 
 
 def angle_to_cartesian(angle: float):
@@ -31,15 +31,18 @@
     def to_angle(self) -> float:
         return self.to_float() * 2 * pi
 
     def to_cartesian(self):
         return angle_to_cartesian(self.to_angle())
 
     def __eq__(self, other):
-        return abs(self.to_float() - other.to_float()) < 0.0000001
+        return self.__hash__() == other.__hash__()
+
+    def __hash__(self):
+        return hash(floor(self.to_float() / 0.0000002))
 
     def has_degree(self):
         return True
 
 
 class FloatWrapper(UnitPoint):
     def __init__(self, value: float, degree: int = None):
@@ -172,15 +175,16 @@
         if ret.to_angle() < self.to_angle():
             ret = NaryFraction(ret.base, ret.exact, ret.repeating, 1)
         assert ret.to_angle() > self.to_angle()
         assert ret.to_float() - self.to_float() <= 1
         assert ret.overflow <= 1
         return ret
 
-def sigma(p:UnitPoint):
+
+def sigma(p: UnitPoint):
     return p.after_sigma()
 
 
 assert NaryFraction(3, [1], [1, 0, 1]).to_string() == "1_101"
 assert NaryFraction(2, [1], []).to_string() == "1"
 
 assert NaryFraction.from_string(3, "1_101") == NaryFraction(3, [1], [1, 0, 1])
```

### Comparing `manim_lamination_builder-0.2.6/manim_lamination_builder.egg-info/PKG-INFO` & `manim_lamination_builder-0.2.7/manim_lamination_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim-lamination-builder
-Version: 0.2.6
+Version: 0.2.7
 Summary: a replacement to lamination builder that uses manim instead of the browser
 Author-email: Forrest Hilton <forrestmhilton@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `manim_lamination_builder-0.2.6/manim_lamination_builder.egg-info/SOURCES.txt` & `manim_lamination_builder-0.2.7/manim_lamination_builder.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 manim_lamination_builder/__init__.py
 manim_lamination_builder/__main__.py
 manim_lamination_builder/animation.py
 manim_lamination_builder/chord.py
 manim_lamination_builder/custom_json.py
 manim_lamination_builder/generate.py
 manim_lamination_builder/lamination.py
+manim_lamination_builder/leaf_polygon_conversion.py
 manim_lamination_builder/main.py
 manim_lamination_builder/morph.py
+manim_lamination_builder/new_generate.py
 manim_lamination_builder/points.py
 manim_lamination_builder.egg-info/PKG-INFO
 manim_lamination_builder.egg-info/SOURCES.txt
 manim_lamination_builder.egg-info/dependency_links.txt
 manim_lamination_builder.egg-info/requires.txt
 manim_lamination_builder.egg-info/top_level.txt
```

### Comparing `manim_lamination_builder-0.2.6/pyproject.toml` & `manim_lamination_builder-0.2.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "manim_lamination_builder"
-version = "0.2.6"
+version = "0.2.7"
 authors = [
   { name="Forrest Hilton", email="forrestmhilton@gmail.com" },
 ]
 description = "a replacement to lamination builder that uses manim instead of the browser"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
```

