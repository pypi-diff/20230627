# Comparing `tmp/mplfooty-0.0.2.tar.gz` & `tmp/mplfooty-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mplfooty-0.0.2.tar", last modified: Wed Jun 21 07:38:40 2023, max compression
+gzip compressed data, was "mplfooty-0.0.3.tar", last modified: Mon Jun 26 23:17:19 2023, max compression
```

## Comparing `mplfooty-0.0.2.tar` & `mplfooty-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-06-21 07:38:40.405919 mplfooty-0.0.2/
--rw-r--r--   0 ciaran     (501) staff       (20)     1069 2023-06-20 07:00:35.000000 mplfooty-0.0.2/LICENSE
--rw-r--r--   0 ciaran     (501) staff       (20)     4799 2023-06-21 07:38:40.405771 mplfooty-0.0.2/PKG-INFO
--rw-r--r--   0 ciaran     (501) staff       (20)     3228 2023-06-21 07:32:42.000000 mplfooty-0.0.2/README.md
-drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-06-21 07:38:40.404553 mplfooty-0.0.2/mplfooty/
--rw-r--r--   0 ciaran     (501) staff       (20)        0 2023-06-20 06:57:42.000000 mplfooty-0.0.2/mplfooty/__init__.py
--rw-r--r--   0 ciaran     (501) staff       (20)     4111 2023-06-20 06:57:42.000000 mplfooty-0.0.2/mplfooty/dimensions.py
--rw-r--r--   0 ciaran     (501) staff       (20)     2762 2023-06-20 06:57:42.000000 mplfooty-0.0.2/mplfooty/pitch.py
--rw-r--r--   0 ciaran     (501) staff       (20)    35636 2023-06-20 06:57:42.000000 mplfooty-0.0.2/mplfooty/pitch_base.py
--rw-r--r--   0 ciaran     (501) staff       (20)    43682 2023-06-20 06:57:42.000000 mplfooty-0.0.2/mplfooty/pitch_plot.py
-drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-06-21 07:38:40.405561 mplfooty-0.0.2/mplfooty.egg-info/
--rw-r--r--   0 ciaran     (501) staff       (20)     4799 2023-06-21 07:38:40.000000 mplfooty-0.0.2/mplfooty.egg-info/PKG-INFO
--rw-r--r--   0 ciaran     (501) staff       (20)      299 2023-06-21 07:38:40.000000 mplfooty-0.0.2/mplfooty.egg-info/SOURCES.txt
--rw-r--r--   0 ciaran     (501) staff       (20)        1 2023-06-21 07:38:40.000000 mplfooty-0.0.2/mplfooty.egg-info/dependency_links.txt
--rw-r--r--   0 ciaran     (501) staff       (20)      206 2023-06-21 07:38:40.000000 mplfooty-0.0.2/mplfooty.egg-info/requires.txt
--rw-r--r--   0 ciaran     (501) staff       (20)        9 2023-06-21 07:38:40.000000 mplfooty-0.0.2/mplfooty.egg-info/top_level.txt
--rw-r--r--   0 ciaran     (501) staff       (20)      774 2023-06-21 07:38:05.000000 mplfooty-0.0.2/pyproject.toml
--rw-r--r--   0 ciaran     (501) staff       (20)       38 2023-06-21 07:38:40.405961 mplfooty-0.0.2/setup.cfg
+drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-06-26 23:17:19.133016 mplfooty-0.0.3/
+-rw-r--r--   0 ciaran     (501) staff       (20)     1069 2023-06-20 07:00:35.000000 mplfooty-0.0.3/LICENSE
+-rw-r--r--   0 ciaran     (501) staff       (20)     4799 2023-06-26 23:17:19.132834 mplfooty-0.0.3/PKG-INFO
+-rw-r--r--   0 ciaran     (501) staff       (20)     3228 2023-06-21 07:32:42.000000 mplfooty-0.0.3/README.md
+drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-06-26 23:17:19.131240 mplfooty-0.0.3/mplfooty/
+-rw-r--r--   0 ciaran     (501) staff       (20)        0 2023-06-20 06:57:42.000000 mplfooty-0.0.3/mplfooty/__init__.py
+-rw-r--r--   0 ciaran     (501) staff       (20)     4710 2023-06-26 23:09:13.000000 mplfooty-0.0.3/mplfooty/dimensions.py
+-rw-r--r--   0 ciaran     (501) staff       (20)     2762 2023-06-20 06:57:42.000000 mplfooty-0.0.3/mplfooty/pitch.py
+-rw-r--r--   0 ciaran     (501) staff       (20)    35636 2023-06-20 06:57:42.000000 mplfooty-0.0.3/mplfooty/pitch_base.py
+-rw-r--r--   0 ciaran     (501) staff       (20)    43682 2023-06-20 06:57:42.000000 mplfooty-0.0.3/mplfooty/pitch_plot.py
+drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-06-26 23:17:19.132524 mplfooty-0.0.3/mplfooty.egg-info/
+-rw-r--r--   0 ciaran     (501) staff       (20)     4799 2023-06-26 23:17:19.000000 mplfooty-0.0.3/mplfooty.egg-info/PKG-INFO
+-rw-r--r--   0 ciaran     (501) staff       (20)      299 2023-06-26 23:17:19.000000 mplfooty-0.0.3/mplfooty.egg-info/SOURCES.txt
+-rw-r--r--   0 ciaran     (501) staff       (20)        1 2023-06-26 23:17:19.000000 mplfooty-0.0.3/mplfooty.egg-info/dependency_links.txt
+-rw-r--r--   0 ciaran     (501) staff       (20)      206 2023-06-26 23:17:19.000000 mplfooty-0.0.3/mplfooty.egg-info/requires.txt
+-rw-r--r--   0 ciaran     (501) staff       (20)        9 2023-06-26 23:17:19.000000 mplfooty-0.0.3/mplfooty.egg-info/top_level.txt
+-rw-r--r--   0 ciaran     (501) staff       (20)      774 2023-06-26 23:16:52.000000 mplfooty-0.0.3/pyproject.toml
+-rw-r--r--   0 ciaran     (501) staff       (20)       38 2023-06-26 23:17:19.133090 mplfooty-0.0.3/setup.cfg
```

### Comparing `mplfooty-0.0.2/LICENSE` & `mplfooty-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mplfooty-0.0.2/PKG-INFO` & `mplfooty-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mplfooty
-Version: 0.0.2
+Version: 0.0.3
 Summary: AFL pitch plotting using matplotlib
 Author-email: Ciaran Grant <ciaran.grant@hotmail.co.uk>
 License: MIT License
         
         Copyright (c) 2023 ciaran-grant
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mplfooty-0.0.2/README.md` & `mplfooty-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mplfooty-0.0.2/mplfooty/dimensions.py` & `mplfooty-0.0.3/mplfooty/dimensions.py`

 * *Files 15% similar despite different names*

```diff
@@ -69,19 +69,34 @@
         
         bottom_boundary_arc = patches.Arc((0, self.behind_bottom), 
                                           width = self.pitch_length, 
                                           height = self.boundary_width, 
                                           theta1=180, theta2=360)
         
         vertices = bottom_boundary_arc.get_verts()
-        distance_to_50 = [abs((((v[0]-self.left)**2 + (v[1]-0)**2)**0.5)-50) for v in vertices]
-        closest_vertex_to_50 = vertices[distance_to_50.index(min(distance_to_50))]
+        interpolated_array = self.interpolate_points(vertices, 10)
+        distance_to_50 = [abs((((v[0]-self.left)**2 + (v[1]-0)**2)**0.5)-50) for v in interpolated_array]
+        closest_vertex_to_50 = interpolated_array[distance_to_50.index(min(distance_to_50))]
 
-        self.inside_50_angle = abs(np.arctan((closest_vertex_to_50[1] - 0) / (closest_vertex_to_50[0] - self.left)) * (180 / np.pi)) + 1
+        self.inside_50_angle = abs(np.arctan((closest_vertex_to_50[1] - 0) / (closest_vertex_to_50[0] - self.left)) * (180 / np.pi))
+
+    @staticmethod
+    def interpolate_points(vertices, num_points):
+        interpolated_points = []
+        
+        for i in range(len(vertices) - 1):
+            start_point = vertices[i]
+            end_point = vertices[i + 1]
+            
+            for j in range(num_points):
+                t = float(j) / (num_points + 1)
+                interpolated_point = (1 - t) * start_point + t * end_point
+                interpolated_points.append(interpolated_point)
         
+        return np.array(interpolated_points)
         
 @dataclass
 class VariableCentreDims(BaseDims):
     """ Dataclass holding dimensions for pitches where origin is the centre of the pitch. """
     def __post_init__(self):
         self.setup_dims()
```

### Comparing `mplfooty-0.0.2/mplfooty/pitch.py` & `mplfooty-0.0.3/mplfooty/pitch.py`

 * *Files identical despite different names*

### Comparing `mplfooty-0.0.2/mplfooty/pitch_base.py` & `mplfooty-0.0.3/mplfooty/pitch_base.py`

 * *Files identical despite different names*

### Comparing `mplfooty-0.0.2/mplfooty/pitch_plot.py` & `mplfooty-0.0.3/mplfooty/pitch_plot.py`

 * *Files identical despite different names*

### Comparing `mplfooty-0.0.2/mplfooty.egg-info/PKG-INFO` & `mplfooty-0.0.3/mplfooty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mplfooty
-Version: 0.0.2
+Version: 0.0.3
 Summary: AFL pitch plotting using matplotlib
 Author-email: Ciaran Grant <ciaran.grant@hotmail.co.uk>
 License: MIT License
         
         Copyright (c) 2023 ciaran-grant
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mplfooty-0.0.2/pyproject.toml` & `mplfooty-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mplfooty"
-version = "0.0.2"
+version = "0.0.3"
 description = "AFL pitch plotting using matplotlib"
 readme = "README.md"
 authors = [{name = "Ciaran Grant", email = "ciaran.grant@hotmail.co.uk"}]
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
 dependencies = [
     "pandas == 1.5.3",
```

