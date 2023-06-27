# Comparing `tmp/UPAFuzzySystems-0.2.3.tar.gz` & `tmp/UPAFuzzySystems-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UPAFuzzySystems-0.2.3.tar", last modified: Sat Jun 24 16:48:50 2023, max compression
+gzip compressed data, was "UPAFuzzySystems-0.2.4.tar", last modified: Tue Jun 27 20:22:44 2023, max compression
```

## Comparing `UPAFuzzySystems-0.2.3.tar` & `UPAFuzzySystems-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 16:48:50.953575 UPAFuzzySystems-0.2.3/
--rw-rw-rw-   0        0        0     1099 2022-10-29 19:07:07.000000 UPAFuzzySystems-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     8329 2023-06-24 16:48:50.950592 UPAFuzzySystems-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     7273 2023-06-24 16:20:44.000000 UPAFuzzySystems-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 16:48:50.888573 UPAFuzzySystems-0.2.3/UPAFuzzySystems/
--rw-rw-rw-   0        0        0    34549 2023-06-24 16:22:01.000000 UPAFuzzySystems-0.2.3/UPAFuzzySystems/UPAFuzzySystems.py
--rw-rw-rw-   0        0        0      286 2022-11-03 19:51:00.000000 UPAFuzzySystems-0.2.3/UPAFuzzySystems/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 16:48:50.944582 UPAFuzzySystems-0.2.3/UPAFuzzySystems.egg-info/
--rw-rw-rw-   0        0        0     8329 2023-06-24 16:48:50.000000 UPAFuzzySystems-0.2.3/UPAFuzzySystems.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-24 16:48:50.000000 UPAFuzzySystems-0.2.3/UPAFuzzySystems.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 16:48:50.000000 UPAFuzzySystems-0.2.3/UPAFuzzySystems.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-24 16:48:50.000000 UPAFuzzySystems-0.2.3/UPAFuzzySystems.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-24 16:48:50.000000 UPAFuzzySystems-0.2.3/UPAFuzzySystems.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 16:48:50.954578 UPAFuzzySystems-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1574 2023-06-24 16:20:55.000000 UPAFuzzySystems-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 20:22:44.303451 UPAFuzzySystems-0.2.4/
+-rw-rw-rw-   0        0        0     1099 2022-10-29 19:07:07.000000 UPAFuzzySystems-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     8329 2023-06-27 20:22:44.302931 UPAFuzzySystems-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7273 2023-06-27 20:18:43.000000 UPAFuzzySystems-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 20:22:44.259157 UPAFuzzySystems-0.2.4/UPAFuzzySystems/
+-rw-rw-rw-   0        0        0    34625 2023-06-27 19:49:25.000000 UPAFuzzySystems-0.2.4/UPAFuzzySystems/UPAFuzzySystems.py
+-rw-rw-rw-   0        0        0      286 2022-11-03 19:51:00.000000 UPAFuzzySystems-0.2.4/UPAFuzzySystems/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 20:22:44.300718 UPAFuzzySystems-0.2.4/UPAFuzzySystems.egg-info/
+-rw-rw-rw-   0        0        0     8329 2023-06-27 20:22:43.000000 UPAFuzzySystems-0.2.4/UPAFuzzySystems.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-27 20:22:44.000000 UPAFuzzySystems-0.2.4/UPAFuzzySystems.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 20:22:43.000000 UPAFuzzySystems-0.2.4/UPAFuzzySystems.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-27 20:22:43.000000 UPAFuzzySystems-0.2.4/UPAFuzzySystems.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-27 20:22:43.000000 UPAFuzzySystems-0.2.4/UPAFuzzySystems.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 20:22:44.303451 UPAFuzzySystems-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1574 2023-06-27 20:19:01.000000 UPAFuzzySystems-0.2.4/setup.py
```

### Comparing `UPAFuzzySystems-0.2.3/LICENSE` & `UPAFuzzySystems-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `UPAFuzzySystems-0.2.3/PKG-INFO` & `UPAFuzzySystems-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UPAFuzzySystems
-Version: 0.2.3
+Version: 0.2.4
 Summary: UPAFuzzySystems package for definition and simulation of Fuzzy Inference Systems for general and control applications.
 Home-page: https://github.com/UniversidadPolitecnicaAguascalientes/UPAFuzzySystems/
 Author: Dr. Martin Montes Rivera (Universidad Politécnica de Aguascalientes)
 Author-email: <martin.montes@upa.edu.mx>
 License: MIT
 Keywords: python,fuzzy logic,fuzzy control,fuzzy inference systems,artificial intelligence
 Classifier: Development Status :: 4 - Beta
@@ -29,15 +29,15 @@
 
 ***Developed by Dr. Martín Montes Rivera***
 
 # Installation
 For installation, just run the command:
 
 ```
-pip install UPAFuzzySystems==0.2.3
+pip install UPAFuzzySystems==0.2.4
 ```
 # Documentation
 
 Here is an example for defining a one-input Mamdani controller, viewing the input and output fuzzy sets, obtaining its behavior surface, and simulating the controller with a transfer function defined by the Python control library.
 
 First, we import the required libraries for working with the transfer function, numpy arrays, and plotting and defining the fuzzy controller.
```

### Comparing `UPAFuzzySystems-0.2.3/README.md` & `UPAFuzzySystems-0.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 ***Developed by Dr. Martín Montes Rivera***
 
 # Installation
 For installation, just run the command:
 
 ```
-pip install UPAFuzzySystems==0.2.3
+pip install UPAFuzzySystems==0.2.4
 ```
 # Documentation
 
 Here is an example for defining a one-input Mamdani controller, viewing the input and output fuzzy sets, obtaining its behavior surface, and simulating the controller with a transfer function defined by the Python control library.
 
 First, we import the required libraries for working with the transfer function, numpy arrays, and plotting and defining the fuzzy controller.
```

### Comparing `UPAFuzzySystems-0.2.3/UPAFuzzySystems/UPAFuzzySystems.py` & `UPAFuzzySystems-0.2.4/UPAFuzzySystems/UPAFuzzySystems.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,16 @@
         membershipvalues=[]
         X = self.structure['universe']
         membershipfuntion = self.structure[name][0]
         vertices = self.structure[name][1]
         vertilist =list(vertices)
         if membershipfuntion =='gaussmf':
             exec('membershipvalues.append('+membershipfuntion+'(X,'+str(vertilist[0])+','+str(vertilist[1])+'))')
+        if membershipfuntion =='gbellmf':
+            exec('membershipvalues.append('+membershipfuntion+'(X,'+str(vertilist[0])+','+str(vertilist[1])+','+str(vertilist[2])+'))')
         elif membershipfuntion == 'raw':
              exec('membershipvalues.append('+str(vertilist)+')')
         else:
             exec('membershipvalues.append('+membershipfuntion+'(X,'+str(vertilist)+'))')
         return {'universe':X,'membership values':membershipvalues[0]}
     def view_fuzzy(self):
 
@@ -110,54 +112,55 @@
                     if (func == "gbellmf"):
                         fig.plot(universe,gbellmf(universe, vertex[0],vertex[1],vertex[2]),color,label =i)
                     if (func == "eq"):
                         textv = 'x'
                         if textv not in vertex:
                             v = eval(vertex)
                             singleton = [1 if i==v else 0 for i in universe]
-                            fig.stem(universe,singleton,color,color+'o',label =i+'='+vertex, use_line_collection = True)
+                            fig.stem(universe,singleton,linefmt=color,markerfmt=color+'o',label =i+'='+vertex)
                             plt.ylim([0, 1.1])
 
                         else:
                             avx = 0.02+len(vertex)*0.0015
                             singleton = [0.0001]*len(universe)
-                            fig.stem(universe,singleton,color,color+'o',label =i, use_line_collection = True)
+                            fig.stem(universe,singleton,linefmt=color,markerfmt=color+'o',label =i)
                             fig.text(-avx, avy, vertex, color=color,fontsize=24)
                             avy = avy-0.01
                             plt.xlim([-0.1,0.1])
                             plt.ylim([-0.1, 0.1])
                     if (func=="raw"):
                         fig.plot(universe,vertex,color,label =i)
 
                 if self.typeuniv == 'discrete':
                     if (func == 'trapmf'):
-                        fig.stem(universe,trapmf(universe, vertex),color,color+'o',label =i, use_line_collection = True)
+                        fig.stem(universe,trapmf(universe, vertex),linefmt=color,markerfmt=color+'o',label =i)
                     if (func == "trimf"):
-                        fig.stem(universe,trimf(universe, vertex),color,color+'o',label =i, use_line_collection = True)
+                        fig.stem(universe,trimf(universe, vertex),linefmt=color,markerfmt=color+'o',label =i)
                     if (func == "gaussmf"):
-                        fig.stem(universe,gaussmf(universe, vertex[0],vertex[1]),color,color+'o',label =i, use_line_collection = True)
+                        fig.stem(universe,gaussmf(universe, vertex[0],vertex[1]),linefmt=color,markerfmt=color+'o',label =i)
                     if (func == "gbellmf"):
-                        fig.stem(universe,gbellmf(universe, vertex[0],vertex[1],vertex[2]),color,color+'o',label =i, use_line_collection = True)
+                        fig.stem(universe,gbellmf(universe, vertex[0],vertex[1],vertex[2]),linefmt=color,markerfmt=color+'o',label =i)
                     if (func == "eq"):
                         textv = 'x'
                         if textv not in vertex:
                             v = eval(vertex)
                             singleton = [1 if i==v else 0 for i in universe]
-                            fig.stem(universe,singleton,color,color+'o',label =i+'='+vertex, use_line_collection = True)
+                            fig.stem(universe,singleton,linefmt=color,markerfmt=color+'o',label =i+'='+vertex)
                             plt.ylim([0, 1.1])
                         else:
                             avx = 0.02+len(vertex)*0.0015
                             singleton = [0.0001]*len(universe)
-                            fig.stem(universe,singleton,color,color+'o',label =i, use_line_collection = True)
+                            fig.stem(universe,singleton,linefmt=color,markerfmt=color+'o',label =i)
                             fig.text(-avx, avy, vertex, color=color,fontsize=24)
                             avy = avy-0.01
                             plt.xlim([-0.1,0.1])
                             plt.ylim([-0.1, 0.1])
                     if (func=="raw"):
-                        fig.stem(universe,vertex,color,color+'o',label =i, use_line_collection = True)
+                        fig.stem(universe,vertex,linefmt=color,markerfmt=color+'o',label =i)
+
 
                         
         plt.title(self.structure['name'])
         plt.legend()
         plt.show()
 
 
@@ -446,31 +449,30 @@
         surface_out = []
         if len(inputvals)==2:
             surfinputs = array([[([i,j]) for j in inputvals[1]] for i in inputvals[0]]).reshape(inputvals[0].shape[0]*inputvals[1].shape[0],len(inputvals))
             surface = self.fuzzy_system_sim(surfinputs).reshape(inputvals[0].shape[0],inputvals[1].shape[0]) 
             X, Y = meshgrid(inputvals[0], inputvals[1])
             plt.figure(figsize=figsizeU)
             ax = plt.axes(projection='3d')
-            print(X.shape)
-            print(Y.shape)
-            print(surface.shape)
             ax.plot_surface(X, Y, surface.transpose(), rstride=1, cstride=1,
                             cmap='viridis', edgecolor='none')
             ax.set_title('Surface Response: '+self.name)
             ax.set_xlabel(self.premises[0].name)
             ax.set_ylabel(self.premises[1].name)
             plt.show()
-        if len(inputvals)==1:
+        elif len(inputvals)==1:
             surface = self.fuzzy_system_sim(inputvals) 
             plt.figure(figsize=figsizeU)
             ax = plt.axes()
             ax.plot(inputvals[0], surface[0])
             ax.set_title('Surface Response: '+self.name)
             ax.set_xlabel(self.premises[0].name)
             plt.show()
+        else: 
+            print('Only available for 1D and 2D inputs')
 
 class fuzzy_controller():
 
     """Allows to implement a fuzzy controller system based on an inference system.
     
 
     Args:
```

### Comparing `UPAFuzzySystems-0.2.3/UPAFuzzySystems.egg-info/PKG-INFO` & `UPAFuzzySystems-0.2.4/UPAFuzzySystems.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UPAFuzzySystems
-Version: 0.2.3
+Version: 0.2.4
 Summary: UPAFuzzySystems package for definition and simulation of Fuzzy Inference Systems for general and control applications.
 Home-page: https://github.com/UniversidadPolitecnicaAguascalientes/UPAFuzzySystems/
 Author: Dr. Martin Montes Rivera (Universidad Politécnica de Aguascalientes)
 Author-email: <martin.montes@upa.edu.mx>
 License: MIT
 Keywords: python,fuzzy logic,fuzzy control,fuzzy inference systems,artificial intelligence
 Classifier: Development Status :: 4 - Beta
@@ -29,15 +29,15 @@
 
 ***Developed by Dr. Martín Montes Rivera***
 
 # Installation
 For installation, just run the command:
 
 ```
-pip install UPAFuzzySystems==0.2.3
+pip install UPAFuzzySystems==0.2.4
 ```
 # Documentation
 
 Here is an example for defining a one-input Mamdani controller, viewing the input and output fuzzy sets, obtaining its behavior surface, and simulating the controller with a transfer function defined by the Python control library.
 
 First, we import the required libraries for working with the transfer function, numpy arrays, and plotting and defining the fuzzy controller.
```

### Comparing `UPAFuzzySystems-0.2.3/setup.py` & `UPAFuzzySystems-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.2.3'
+VERSION = '0.2.4'
 DESCRIPTION = 'UPAFuzzySystems package for definition and simulation of Fuzzy Inference Systems for general and control applications.'
 LONG_DESCRIPTION = 'UPAFuzzySystems library allows defining Fuzzy Inference Systems for different applications with continuous and discrete universes, it also deploys structures for simulation of fuzzy control with transfer functions and state space models.'
 with open('README.md', 'r', encoding='utf-8') as file:
     LONG_DESCRIPTION = file.read()
 
 # Setting up
 setup(
```

