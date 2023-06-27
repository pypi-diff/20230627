# Comparing `tmp/BroadSword-0.1.1.tar.gz` & `tmp/BroadSword-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BroadSword-0.1.1.tar", last modified: Wed Jun 21 22:49:16 2023, max compression
+gzip compressed data, was "BroadSword-0.1.2.tar", last modified: Tue Jun 27 18:45:29 2023, max compression
```

## Comparing `BroadSword-0.1.1.tar` & `BroadSword-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:49:16.628856 BroadSword-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 22:49:05.000000 BroadSword-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-21 22:49:16.628856 BroadSword-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-06-21 22:49:05.000000 BroadSword-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-21 22:49:05.000000 BroadSword-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-21 22:49:16.628856 BroadSword-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:49:16.624856 BroadSword-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:49:16.624856 BroadSword-0.1.1/src/BroadSword/
--rw-r--r--   0 runner    (1001) docker     (123)    29345 2023-06-21 22:49:05.000000 BroadSword-0.1.1/src/BroadSword/BroadSword.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:49:05.000000 BroadSword-0.1.1/src/BroadSword/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20584 2023-06-21 22:49:05.000000 BroadSword-0.1.1/src/BroadSword/libmatrices.so
--rw-r--r--   0 runner    (1001) docker     (123)    33748 2023-06-21 22:49:05.000000 BroadSword-0.1.1/src/BroadSword/libmatrices_ARM64.dylib
--rw-r--r--   0 runner    (1001) docker     (123)    33320 2023-06-21 22:49:05.000000 BroadSword-0.1.1/src/BroadSword/libmatrices_x86_64.dylib
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-06-21 22:49:05.000000 BroadSword-0.1.1/src/BroadSword/matrices.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:49:16.628856 BroadSword-0.1.1/src/BroadSword.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-21 22:49:16.000000 BroadSword-0.1.1/src/BroadSword.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-21 22:49:16.000000 BroadSword-0.1.1/src/BroadSword.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:49:16.000000 BroadSword-0.1.1/src/BroadSword.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 22:49:16.000000 BroadSword-0.1.1/src/BroadSword.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 22:49:16.000000 BroadSword-0.1.1/src/BroadSword.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:49:16.000000 BroadSword-0.1.1/src/BroadSword.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:45:29.946602 BroadSword-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-27 18:45:20.000000 BroadSword-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-27 18:45:29.946602 BroadSword-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-06-27 18:45:20.000000 BroadSword-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 18:45:20.000000 BroadSword-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-27 18:45:29.946602 BroadSword-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:45:29.938602 BroadSword-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:45:29.942602 BroadSword-0.1.2/src/BroadSword/
+-rw-r--r--   0 runner    (1001) docker     (123)    29506 2023-06-27 18:45:20.000000 BroadSword-0.1.2/src/BroadSword/BroadSword.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:45:20.000000 BroadSword-0.1.2/src/BroadSword/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20584 2023-06-27 18:45:20.000000 BroadSword-0.1.2/src/BroadSword/libmatrices.so
+-rw-r--r--   0 runner    (1001) docker     (123)    33748 2023-06-27 18:45:20.000000 BroadSword-0.1.2/src/BroadSword/libmatrices_ARM64.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)    33320 2023-06-27 18:45:20.000000 BroadSword-0.1.2/src/BroadSword/libmatrices_x86_64.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-06-27 18:45:20.000000 BroadSword-0.1.2/src/BroadSword/matrices.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:45:29.946602 BroadSword-0.1.2/src/BroadSword.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-27 18:45:29.000000 BroadSword-0.1.2/src/BroadSword.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-27 18:45:29.000000 BroadSword-0.1.2/src/BroadSword.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:45:29.000000 BroadSword-0.1.2/src/BroadSword.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-27 18:45:29.000000 BroadSword-0.1.2/src/BroadSword.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 18:45:29.000000 BroadSword-0.1.2/src/BroadSword.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:45:29.000000 BroadSword-0.1.2/src/BroadSword.egg-info/zip-safe
```

### Comparing `BroadSword-0.1.1/LICENSE` & `BroadSword-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BroadSword-0.1.1/PKG-INFO` & `BroadSword-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BroadSword
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/Cody-Somers/BroadSword
 Author: Cody Somers
 Author-email: cas003@usask.ca
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `BroadSword-0.1.1/README.md` & `BroadSword-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `BroadSword-0.1.1/setup.cfg` & `BroadSword-0.1.2/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = BroadSword
-version = 0.1.1
+version = 0.1.2
 author = Cody Somers
 author_email = cas003@usask.ca
 description = Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Cody-Somers/BroadSword
 project_urls = 
@@ -21,14 +21,15 @@
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	numpy
 	pandas
 	bokeh>=2.3.3,<3
+	reixs
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 BroadSword = *.so, *.dylib, *.c
```

### Comparing `BroadSword-0.1.1/src/BroadSword/BroadSword.py` & `BroadSword-0.1.2/src/BroadSword/BroadSword.py`

 * *Files 2% similar despite different names*

```diff
@@ -523,15 +523,15 @@
             xesY[c1] = ExpSXS[1][c1][0]
         
         for c1 in range(ExpSXSCount[1]): # Experimental xanes spectra
             xanesX[c1] = ExpSXS[0][c1][1]
             xanesY[c1] = ExpSXS[1][c1][1]
         
         #p = figure()
-        p.line(xanesX,xanesY,line_color="red") # XANES plot
+        p.line(xanesX,xanesY,line_color="red",legend_label="Experimental XES/XANES") # XANES plot
         p.line(xesX,xesY,line_color="red") # XES plot
         #show(p)
         return
 
     def plotShiftCalc(self,p):
         """
         Plot the shifted calculated data.
@@ -583,17 +583,17 @@
     def plotCalc(self):
         """
         Plot the unshifted calculated data. This is purely the raw data read from .loadCalc()
         """
         p = figure()
         for c1 in range(CalcSXSCase): # Since this is np array you can use : to get all data points
             colour = COLORP[c1]
-            p.line(CalcSXS[0,:,0,c1], CalcSXS[1,:,0,c1],line_color=colour) # XES plot
-            p.line(CalcSXS[0,:,1,c1], CalcSXS[1,:,1,c1],line_color=colour) # XAS plot
-            p.line(CalcSXS[0,:,2,c1], CalcSXS[1,:,2,c1],line_color=colour) # XANES plot
+            p.line(CalcSXS[0,:,0,c1], CalcSXS[1,:,0,c1],line_color=colour,legend_label="XES") # XES plot
+            p.line(CalcSXS[0,:,1,c1], CalcSXS[1,:,1,c1],line_color=colour,legend_label="XAS") # XAS plot
+            p.line(CalcSXS[0,:,2,c1], CalcSXS[1,:,2,c1],line_color=colour,legend_label="XANES") # XANES plot
         show(p)
         return
 
     def plotBroadCalc(self,p):
         """
         Plot the final calculated and broadened data.
         The bokeh figure needs to be created and configured outside of the function. This simply adds the XANES, XAS, and XES to a figure.
@@ -623,16 +623,16 @@
             sumxasX[c2] = SumSXS[0][c2][1]
             sumxasY[c2] = SumSXS[1][c2][1] / MaxBroadSXS[1]
 
         for c2 in range(SumSXSCount[2]): # Calculated XANES spectra
             sumxanesX[c2] = SumSXS[0][c2][2]
             sumxanesY[c2] = SumSXS[1][c2][2] / MaxBroadSXS[2]
 
-        p.line(sumxesX,sumxesY,line_color="limegreen") # XES plot
-        p.line(sumxasX,sumxasY,line_color="blue") # XAS plot
+        p.line(sumxesX,sumxesY,line_color="limegreen",legend_label="Broadened XES/XANES") # XES plot
+        p.line(sumxasX,sumxasY,line_color="blue",legend_label="Broadened XAS") # XAS plot
         p.line(sumxanesX,sumxanesY,line_color="limegreen") # XANES plot
         #show(p)
         return
 
     def export(self, filename):
         """
         Export and write data to the specified files.
```

### Comparing `BroadSword-0.1.1/src/BroadSword/libmatrices.so` & `BroadSword-0.1.2/src/BroadSword/libmatrices.so`

 * *Files identical despite different names*

### Comparing `BroadSword-0.1.1/src/BroadSword/libmatrices_ARM64.dylib` & `BroadSword-0.1.2/src/BroadSword/libmatrices_ARM64.dylib`

 * *Files identical despite different names*

### Comparing `BroadSword-0.1.1/src/BroadSword/libmatrices_x86_64.dylib` & `BroadSword-0.1.2/src/BroadSword/libmatrices_x86_64.dylib`

 * *Files identical despite different names*

### Comparing `BroadSword-0.1.1/src/BroadSword/matrices.c` & `BroadSword-0.1.2/src/BroadSword/matrices.c`

 * *Files identical despite different names*

### Comparing `BroadSword-0.1.1/src/BroadSword.egg-info/PKG-INFO` & `BroadSword-0.1.2/src/BroadSword.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BroadSword
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/Cody-Somers/BroadSword
 Author: Cody Somers
 Author-email: cas003@usask.ca
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

