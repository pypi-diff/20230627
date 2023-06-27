# Comparing `tmp/vizmath-0.0.3.tar.gz` & `tmp/vizmath-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vizmath-0.0.3.tar", last modified: Tue Jun 27 01:12:29 2023, max compression
+gzip compressed data, was "dist\vizmath-0.0.4.tar", last modified: Tue Jun 27 03:34:30 2023, max compression
```

## Comparing `vizmath-0.0.3.tar` & `vizmath-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 01:12:29.000000 vizmath-0.0.3/
--rw-rw-rw-   0        0        0      517 2023-06-27 01:12:29.000000 vizmath-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       78 2023-06-27 01:09:47.000000 vizmath-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 01:12:29.000000 vizmath-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-06-27 01:09:40.000000 vizmath-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 01:12:29.000000 vizmath-0.0.3/vizmath/
--rw-rw-rw-   0        0        0       67 2023-06-27 01:06:02.000000 vizmath-0.0.3/vizmath/__init__.py
--rw-rw-rw-   0        0        0    21082 2023-06-27 01:05:42.000000 vizmath-0.0.3/vizmath/vizmath.py
-drwxrwxrwx   0        0        0        0 2023-06-27 01:12:29.000000 vizmath-0.0.3/vizmath.egg-info/
--rw-rw-rw-   0        0        0      517 2023-06-27 01:12:29.000000 vizmath-0.0.3/vizmath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-06-27 01:12:29.000000 vizmath-0.0.3/vizmath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 01:12:29.000000 vizmath-0.0.3/vizmath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-27 01:12:29.000000 vizmath-0.0.3/vizmath.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-27 01:12:29.000000 vizmath-0.0.3/vizmath.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 03:34:30.000000 vizmath-0.0.4/
+-rw-rw-rw-   0        0        0      517 2023-06-27 03:34:30.000000 vizmath-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2023-06-27 01:09:47.000000 vizmath-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-27 03:34:30.000000 vizmath-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      785 2023-06-27 03:28:05.000000 vizmath-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:34:30.000000 vizmath-0.0.4/vizmath/
+-rw-rw-rw-   0        0        0       67 2023-06-27 03:21:13.000000 vizmath-0.0.4/vizmath/__init__.py
+-rw-rw-rw-   0        0        0    22137 2023-06-27 03:31:54.000000 vizmath-0.0.4/vizmath/vizmath.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:34:30.000000 vizmath-0.0.4/vizmath.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-06-27 03:34:29.000000 vizmath-0.0.4/vizmath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-06-27 03:34:29.000000 vizmath-0.0.4/vizmath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 03:34:29.000000 vizmath-0.0.4/vizmath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-27 03:34:29.000000 vizmath-0.0.4/vizmath.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-27 03:34:29.000000 vizmath-0.0.4/vizmath.egg-info/top_level.txt
```

### Comparing `vizmath-0.0.3/PKG-INFO` & `vizmath-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vizmath
-Version: 0.0.3
+Version: 0.0.4
 Summary: Visualization math toolkit.
 Home-page: https://github.com/nickgerend/vizmath
 Author: Nick Gerend
 Author-email: nickgerend@gmail.com
 License: MIT
 Description: # Welcome to vizmath
```

### Comparing `vizmath-0.0.3/setup.py` & `vizmath-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 import setuptools as st
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 setup(
     name="vizmath",
-    version="0.0.3",
+    version="0.0.4",
     description="Visualization math toolkit.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/nickgerend/vizmath",
     author="Nick Gerend",
     author_email="nickgerend@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.9",
     ],
     packages=st.find_namespace_packages(),
-    install_requires=["numpy", "scipy"],
+    install_requires=["numpy", "scipy", "matplotlib", "pandas"],
     include_package_data=True,
     package_data={'': ['data/*.csv']},
 )
```

### Comparing `vizmath-0.0.3/vizmath/vizmath.py` & `vizmath-0.0.4/vizmath/vizmath.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,113 +1,20 @@
 # vizmath
 # Author: Nick Gerend
 
+#%%
 from math import sin, cos, pi, exp, atan2, sqrt, atan, tan, radians
 import numpy as np
+import pandas as pd
 import scipy.optimize as optimize
+import os
+import matplotlib.pyplot as plt
 
 class vmath:
 
-    class point:
-        def __init__(self, id=None, x=0.0, y=0.0, path=1, **kwargs):
-            self.id = id
-            self.x = x
-            self.y = y
-            self.path = path
-            for key in kwargs.items():
-                self.__setattr__(key, kwargs.get(key))
-
-    #region binary tree
-
-    class full_bi_tree:
-        
-        def __init__(self, length, levels, angle, R_tag, L_tag, y_offset, Root_tag, lineage):
-            self.bi_tree_list = []
-            self.length = length
-            self.levels = levels
-            self.angle = angle
-            self.R_tag = R_tag
-            self.L_tag = L_tag
-            self.y_offset = y_offset
-            self.Root_tag = Root_tag
-            self.lineage = lineage
-            self.full_binary_tree()
-        
-        class bi_tree:
-            def __init__(self, level, side, x, y, lineage, group, tree=0): 
-                self.level = level
-                self.side = side
-                self.x = x
-                self.y = y
-                self.lineage = lineage
-                self.group = group
-                self.tree = tree
-            def to_dict(self):
-                return {
-                    'level' : self.level,
-                    'side' : self.side,
-                    'x' : self.x,
-                    'y' : self.y,
-                    'lineage' : self.lineage,
-                    'group' : self.group,
-                    'tree' : self.tree }
-
-        def generate_points(self, start_angle, start_x, start_y, angle, length, level):
-            #sides
-            length_a = length*cos(angle*pi/180.)
-            length_b = length*cos((90.-angle)*pi/180.)
-            #right
-            xs_a1 = start_x + (length/2.)*cos(-start_angle*pi/180.)
-            ys_a1 = start_y + (length/2.)*sin(-start_angle*pi/180.)
-            xs_a2 = xs_a1 + (length_a/2.)*cos((-start_angle-angle+180.)*pi/180.)
-            ys_a2 = ys_a1 + (length_a/2.)*sin((-start_angle-angle+180.)*pi/180.)
-            xa = xs_a2 + (length_a)*cos((-start_angle-angle+90.)*pi/180.)
-            ya = ys_a2 + (length_a)*sin((-start_angle-angle+90.)*pi/180.)
-            #left
-            xs_b1 = start_x + (length/2.)*cos((-start_angle+180.)*pi/180.)
-            ys_b1 = start_y + (length/2.)*sin((-start_angle+180.)*pi/180.)
-            xs_b2 = xs_b1 + (length_b/2.)*cos((-start_angle+(90.-angle))*pi/180.)
-            ys_b2 = ys_b1 + (length_b/2.)*sin((-start_angle+(90.-angle))*pi/180.)
-            xb = xs_b2 + (length_b)*cos((-start_angle+(90.-angle)+90.)*pi/180.)
-            yb = ys_b2 + (length_b)*sin((-start_angle+(90.-angle)+90.)*pi/180.)
-            #angles
-            aa = start_angle + angle
-            ab = 270. + start_angle + angle
-            return xa, ya, aa, length_a, xb, yb, ab, length_b, level + 1
-        
-        def binary_tree(self, start_angle, length, level, levels, x, y, angle, lineage, R_tag, L_tag):
-            if level == levels:
-                return
-            xa, ya, aa, length_a, xb, yb, ab, length_b, level = self.generate_points(start_angle, x, y, angle, length, level)
-            #output
-            #-- R-lines
-            self.bi_tree_list.append(self.bi_tree(level, self.R_tag, xa, ya, lineage + self.R_tag, lineage + '_' + lineage + self.R_tag))
-            self.bi_tree_list.append(self.bi_tree(level, self.R_tag, xa, ya, lineage + self.R_tag, lineage + self.R_tag + '_' + lineage + self.R_tag + self.R_tag)) #+'RR'
-            self.bi_tree_list.append(self.bi_tree(level, self.R_tag, xa, ya, lineage + self.R_tag, lineage + self.R_tag + '_' + lineage + self.R_tag + self.L_tag)) #+'RL'
-            #-- L-lines
-            self.bi_tree_list.append(self.bi_tree(level, self.L_tag, xb, yb, lineage + self.L_tag, lineage + '_' + lineage + self.L_tag))
-            self.bi_tree_list.append(self.bi_tree(level, self.L_tag, xb, yb, lineage + self.L_tag, lineage + self.L_tag + '_' + lineage + self.L_tag + self.R_tag)) #+'LR'
-            self.bi_tree_list.append(self.bi_tree(level, self.L_tag, xb, yb, lineage + self.L_tag, lineage + self.L_tag + '_' + lineage + self.L_tag + self.L_tag)) #+'LL'
-            #right
-            self.binary_tree(aa, length_a, level, self.levels, xa, ya, self.angle, lineage + R_tag, R_tag, L_tag)
-            #left
-            self.binary_tree(ab, length_b, level, self.levels, xb, yb, self.angle, lineage + L_tag, R_tag, L_tag)
-        
-        def full_binary_tree(self):
-            self.binary_tree(0., self.length, 0, self.levels, 0., 0., self.angle, self.lineage, self.R_tag, self.L_tag)
-            self.bi_tree_list.append(self.bi_tree(0, '', 0., -self.y_offset, self.Root_tag, '_'))
-            self.bi_tree_list.append(self.bi_tree(0, '', 0., 0., self.Root_tag, '_'))
-            self.bi_tree_list.append(self.bi_tree(0, '', 0., 0., self.Root_tag, '' + '_' + self.R_tag))
-            self.bi_tree_list.append(self.bi_tree(0, '', 0., 0., self.Root_tag, '' + '_' + self.L_tag))
-            for o in self.bi_tree_list: o.y += self.y_offset
-
-    #endregion
-
-    #region functions
-
     def angle_by_two_points(self, x1, y1, x2, y2):
         a = atan2(x2-x1, y2-y1)*180/pi
         if a < 0:
             a += 360. 
         return a
 
     def distance_between_two_points(self, x1, y1, x2, y2):
@@ -506,9 +413,134 @@
         Zout2_y0 = np.reshape(Zgrid2_y0, -1)
 
         Zout_x0 = np.concatenate([Zout1_x0, Zout2_x0])
         Zout_y0 = np.concatenate([Zout1_y0, Zout2_y0])
 
         zip(Yout,Xout,Zout,Zout_x0,Zout_y0)
 
-    #endregion
+class points:
 
+    viz=[]
+    df = pd.DataFrame()
+
+    class point:
+
+        def __init__(self, id=None, x=0.0, y=0.0, path=0, kwargs=None):
+            self.id = id
+            self.x = x
+            self.y = y
+            self.path = path
+            for key, value in kwargs.items():
+                self.__setattr__(key, value)
+        
+    def append(self, id, x, y, path, **kwargs):
+        self.viz.append(self.point(id=id,x=x,y=y,path=path,kwargs=kwargs))
+
+    def to_dataframe(self):
+        self.df = pd.DataFrame([{attr: getattr(p,attr) for attr in dir(p) if not attr.startswith('_')} for p in self.viz])
+    
+    def dataframe_rescale(self, xmin=None, xmax=None, ymin=None, ymax=None, nxmin=-1, nxmax=1, nymin=-1, nymax=1):
+        if not self.df.empty:
+            vm = vmath()
+            if xmin is None:
+                xmin = min(self.df['x'])
+            if xmax is None:
+                xmax = max(self.df['x'])
+            if ymin is None:
+                ymin = min(self.df['y'])
+            if ymax is None:
+                ymax = max(self.df['y'])
+            self.df['x'] = [vm.rescale(x,xmin,xmax,nxmin,nxmax) for x in self.df['x']]
+            self.df['y'] = [vm.rescale(y,ymin,ymax,nymin,nymax) for y in self.df['y']]
+
+    def dataframe_to_csv(self, file_name):
+        if not self.df.empty:
+            self.df.to_csv(os.path.dirname(__file__) + '/' + file_name + '.csv', encoding='utf-8', index=False)
+
+    def plot_xy(self):
+        x = [o.x for o in self.viz]
+        y = [o.y for o in self.viz]
+        plt.scatter(x, y)
+        plt.gca().set_aspect('equal', adjustable='box')
+        plt.show(block=True)
+
+class full_bi_tree:
+    
+    def __init__(self, length, levels, angle, R_tag, L_tag, y_offset, Root_tag, lineage):
+        self.bi_tree_list = []
+        self.length = length
+        self.levels = levels
+        self.angle = angle
+        self.R_tag = R_tag
+        self.L_tag = L_tag
+        self.y_offset = y_offset
+        self.Root_tag = Root_tag
+        self.lineage = lineage
+        self.full_binary_tree()
+    
+    class bi_tree:
+        def __init__(self, level, side, x, y, lineage, group, tree=0): 
+            self.level = level
+            self.side = side
+            self.x = x
+            self.y = y
+            self.lineage = lineage
+            self.group = group
+            self.tree = tree
+        def to_dict(self):
+            return {
+                'level' : self.level,
+                'side' : self.side,
+                'x' : self.x,
+                'y' : self.y,
+                'lineage' : self.lineage,
+                'group' : self.group,
+                'tree' : self.tree }
+
+    def generate_points(self, start_angle, start_x, start_y, angle, length, level):
+        #sides
+        length_a = length*cos(angle*pi/180.)
+        length_b = length*cos((90.-angle)*pi/180.)
+        #right
+        xs_a1 = start_x + (length/2.)*cos(-start_angle*pi/180.)
+        ys_a1 = start_y + (length/2.)*sin(-start_angle*pi/180.)
+        xs_a2 = xs_a1 + (length_a/2.)*cos((-start_angle-angle+180.)*pi/180.)
+        ys_a2 = ys_a1 + (length_a/2.)*sin((-start_angle-angle+180.)*pi/180.)
+        xa = xs_a2 + (length_a)*cos((-start_angle-angle+90.)*pi/180.)
+        ya = ys_a2 + (length_a)*sin((-start_angle-angle+90.)*pi/180.)
+        #left
+        xs_b1 = start_x + (length/2.)*cos((-start_angle+180.)*pi/180.)
+        ys_b1 = start_y + (length/2.)*sin((-start_angle+180.)*pi/180.)
+        xs_b2 = xs_b1 + (length_b/2.)*cos((-start_angle+(90.-angle))*pi/180.)
+        ys_b2 = ys_b1 + (length_b/2.)*sin((-start_angle+(90.-angle))*pi/180.)
+        xb = xs_b2 + (length_b)*cos((-start_angle+(90.-angle)+90.)*pi/180.)
+        yb = ys_b2 + (length_b)*sin((-start_angle+(90.-angle)+90.)*pi/180.)
+        #angles
+        aa = start_angle + angle
+        ab = 270. + start_angle + angle
+        return xa, ya, aa, length_a, xb, yb, ab, length_b, level + 1
+    
+    def binary_tree(self, start_angle, length, level, levels, x, y, angle, lineage, R_tag, L_tag):
+        if level == levels:
+            return
+        xa, ya, aa, length_a, xb, yb, ab, length_b, level = self.generate_points(start_angle, x, y, angle, length, level)
+        #output
+        #-- R-lines
+        self.bi_tree_list.append(self.bi_tree(level, self.R_tag, xa, ya, lineage + self.R_tag, lineage + '_' + lineage + self.R_tag))
+        self.bi_tree_list.append(self.bi_tree(level, self.R_tag, xa, ya, lineage + self.R_tag, lineage + self.R_tag + '_' + lineage + self.R_tag + self.R_tag)) #+'RR'
+        self.bi_tree_list.append(self.bi_tree(level, self.R_tag, xa, ya, lineage + self.R_tag, lineage + self.R_tag + '_' + lineage + self.R_tag + self.L_tag)) #+'RL'
+        #-- L-lines
+        self.bi_tree_list.append(self.bi_tree(level, self.L_tag, xb, yb, lineage + self.L_tag, lineage + '_' + lineage + self.L_tag))
+        self.bi_tree_list.append(self.bi_tree(level, self.L_tag, xb, yb, lineage + self.L_tag, lineage + self.L_tag + '_' + lineage + self.L_tag + self.R_tag)) #+'LR'
+        self.bi_tree_list.append(self.bi_tree(level, self.L_tag, xb, yb, lineage + self.L_tag, lineage + self.L_tag + '_' + lineage + self.L_tag + self.L_tag)) #+'LL'
+        #right
+        self.binary_tree(aa, length_a, level, self.levels, xa, ya, self.angle, lineage + R_tag, R_tag, L_tag)
+        #left
+        self.binary_tree(ab, length_b, level, self.levels, xb, yb, self.angle, lineage + L_tag, R_tag, L_tag)
+    
+    def full_binary_tree(self):
+        self.binary_tree(0., self.length, 0, self.levels, 0., 0., self.angle, self.lineage, self.R_tag, self.L_tag)
+        self.bi_tree_list.append(self.bi_tree(0, '', 0., -self.y_offset, self.Root_tag, '_'))
+        self.bi_tree_list.append(self.bi_tree(0, '', 0., 0., self.Root_tag, '_'))
+        self.bi_tree_list.append(self.bi_tree(0, '', 0., 0., self.Root_tag, '' + '_' + self.R_tag))
+        self.bi_tree_list.append(self.bi_tree(0, '', 0., 0., self.Root_tag, '' + '_' + self.L_tag))
+        for o in self.bi_tree_list: o.y += self.y_offset
```

### Comparing `vizmath-0.0.3/vizmath.egg-info/PKG-INFO` & `vizmath-0.0.4/vizmath.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vizmath
-Version: 0.0.3
+Version: 0.0.4
 Summary: Visualization math toolkit.
 Home-page: https://github.com/nickgerend/vizmath
 Author: Nick Gerend
 Author-email: nickgerend@gmail.com
 License: MIT
 Description: # Welcome to vizmath
```

