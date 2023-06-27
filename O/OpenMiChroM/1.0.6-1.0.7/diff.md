# Comparing `tmp/OpenMiChroM-1.0.6.tar.gz` & `tmp/OpenMiChroM-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenMiChroM-1.0.6.tar", last modified: Tue Feb  7 17:25:47 2023, max compression
+gzip compressed data, was "OpenMiChroM-1.0.7.tar", last modified: Tue Jun 27 17:12:58 2023, max compression
```

## Comparing `OpenMiChroM-1.0.6.tar` & `OpenMiChroM-1.0.7.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-02-07 17:25:47.256714 OpenMiChroM-1.0.6/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1131 2023-02-07 17:25:15.000000 OpenMiChroM-1.0.6/LICENSE
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       37 2023-02-07 17:25:15.000000 OpenMiChroM-1.0.6/MANIFEST.in
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-02-07 17:25:47.256714 OpenMiChroM-1.0.6/OpenMiChroM/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    90051 2023-02-07 17:25:15.000000 OpenMiChroM-1.0.6/OpenMiChroM/ChromDynamics.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23930 2023-02-07 17:25:15.000000 OpenMiChroM-1.0.6/OpenMiChroM/CndbTools.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    30979 2023-02-07 17:25:15.000000 OpenMiChroM-1.0.6/OpenMiChroM/Optimization.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      153 2023-02-07 17:25:15.000000 OpenMiChroM-1.0.6/OpenMiChroM/__init__.py
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-02-07 17:25:47.256714 OpenMiChroM-1.0.6/OpenMiChroM/share/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      517 2023-02-07 17:25:15.000000 OpenMiChroM-1.0.6/OpenMiChroM/share/MiChroM.ff
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-02-07 17:25:47.256714 OpenMiChroM-1.0.6/OpenMiChroM.egg-info/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     5947 2023-02-07 17:25:46.000000 OpenMiChroM-1.0.6/OpenMiChroM.egg-info/PKG-INFO
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      449 2023-02-07 17:25:47.000000 OpenMiChroM-1.0.6/OpenMiChroM.egg-info/SOURCES.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2023-02-07 17:25:46.000000 OpenMiChroM-1.0.6/OpenMiChroM.egg-info/dependency_links.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       50 2023-02-07 17:25:47.000000 OpenMiChroM-1.0.6/OpenMiChroM.egg-info/entry_points.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       41 2023-02-07 17:25:47.000000 OpenMiChroM-1.0.6/OpenMiChroM.egg-info/requires.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       18 2023-02-07 17:25:47.000000 OpenMiChroM-1.0.6/OpenMiChroM.egg-info/top_level.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2023-02-07 17:25:46.000000 OpenMiChroM-1.0.6/OpenMiChroM.egg-info/zip-safe
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     5947 2023-02-07 17:25:47.256714 OpenMiChroM-1.0.6/PKG-INFO
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     5089 2023-02-07 17:25:26.000000 OpenMiChroM-1.0.6/README.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       38 2023-02-07 17:25:47.256714 OpenMiChroM-1.0.6/setup.cfg
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1469 2023-02-07 17:25:15.000000 OpenMiChroM-1.0.6/setup.py
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-02-07 17:25:47.256714 OpenMiChroM-1.0.6/tests/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)        0 2023-02-07 17:25:15.000000 OpenMiChroM-1.0.6/tests/__init__.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     2799 2023-02-07 17:25:15.000000 OpenMiChroM-1.0.6/tests/tests.py
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-27 17:12:58.727846 OpenMiChroM-1.0.7/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1131 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/LICENSE
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       37 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/MANIFEST.in
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-27 17:12:58.727846 OpenMiChroM-1.0.7/OpenMiChroM/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    98399 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/OpenMiChroM/ChromDynamics.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    23952 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/OpenMiChroM/CndbTools.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2541 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/OpenMiChroM/Integrators.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    36993 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/OpenMiChroM/Optimization.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      153 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/OpenMiChroM/__init__.py
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-27 17:12:58.727846 OpenMiChroM-1.0.7/OpenMiChroM/share/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      517 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/OpenMiChroM/share/MiChroM.ff
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-27 17:12:58.727846 OpenMiChroM-1.0.7/OpenMiChroM.egg-info/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     5691 2023-06-27 17:12:58.000000 OpenMiChroM-1.0.7/OpenMiChroM.egg-info/PKG-INFO
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      476 2023-06-27 17:12:58.000000 OpenMiChroM-1.0.7/OpenMiChroM.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2023-06-27 17:12:58.000000 OpenMiChroM-1.0.7/OpenMiChroM.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       50 2023-06-27 17:12:58.000000 OpenMiChroM-1.0.7/OpenMiChroM.egg-info/entry_points.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       41 2023-06-27 17:12:58.000000 OpenMiChroM-1.0.7/OpenMiChroM.egg-info/requires.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       18 2023-06-27 17:12:58.000000 OpenMiChroM-1.0.7/OpenMiChroM.egg-info/top_level.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2023-06-27 17:12:34.000000 OpenMiChroM-1.0.7/OpenMiChroM.egg-info/zip-safe
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     5691 2023-06-27 17:12:58.727846 OpenMiChroM-1.0.7/PKG-INFO
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     5089 2023-06-27 17:12:56.000000 OpenMiChroM-1.0.7/README.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       38 2023-06-27 17:12:58.727846 OpenMiChroM-1.0.7/setup.cfg
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1254 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/setup.py
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-27 17:12:58.727846 OpenMiChroM-1.0.7/tests/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)        0 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/tests/__init__.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2799 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/tests/tests.py
```

### Comparing `OpenMiChroM-1.0.6/LICENSE` & `OpenMiChroM-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenMiChroM-1.0.6/OpenMiChroM/ChromDynamics.py` & `OpenMiChroM-1.0.7/OpenMiChroM/ChromDynamics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2022 The Center for Theoretical Biological Physics (CTBP) - Rice University
+# Copyright (c) 2020-2023 The Center for Theoretical Biological Physics (CTBP) - Rice University
 # This file is from the Open-MiChroM project, released under the MIT License. 
 
 R"""  
 The :class:`~.ChromDynamics` classes perform chromatin dynamics based on the compartment annotations sequence of chromosomes. The simulations can be performed either using the default parameters of MiChroM (Minimal Chromatin Model) or using custom values for the type-to-type and Ideal Chromosome parameters..
 """
 
 # with OpenMM 7.7.0, the import calls have changed. So, try both, if needed
@@ -27,14 +27,15 @@
 from six import string_types
 import os
 import time
 import random
 import h5py
 import pandas as pd
 from pathlib import Path
+import types
 
 
 class MiChroM:
     R"""
     The :class:`~.MiChroM` class performs chromatin dynamics employing the default MiChroM energy function parameters for the type-to-type and Ideal Chromosome interactions.
     
     Details about the MiChroM (Minimal Chromatin Model) energy function and the default parameters are decribed in "Di Pierro, M., Zhang, B., Aiden, E.L., Wolynes, P.G. and Onuchic, J.N., 2016. Transferable model for chromosome architecture. Proceedings of the National Academy of Sciences, 113(43), pp.12168-12173."
@@ -351,15 +352,32 @@
             m = int(chain[0])
             for t in range(len(pos)):
                 pos[t] = pos[t].split()
                 pos[t][0] = int(pos[t][0]) +m
                 pos[t][1] = int(pos[t][1]) +m
                 self.loopPosition.append(pos[t])
                 
+    
+    ##============================
+    ##      FORCES          
+    ##============================
+
+    def addCylindricalConfinement(self, r_conf=5.0, z_conf=10.0, kr=30.0):
+        cyl_conf_energy="step(r_xy-r_cyn) * 0.5 * k_cyn * (r_xy-r_cyn)^2 + step(z^2-zconf^2) * 0.5 * k_cyn * (z-zconf)^2; r_xy=sqrt(x*x+y*y)"
+        
+        cyl_conf_fg = self.mm.CustomExternalForce(cyl_conf_energy)
+        cyl_conf_fg.addGlobalParameter('r_cyn', r_conf)
+        cyl_conf_fg.addGlobalParameter('k_cyn', kr)
+        cyl_conf_fg.addGlobalParameter('zconf', z_conf)
+        
+        self.forceDict["CylindricalConfinement"]=cyl_conf_fg
 
+        for i in range(self.N):
+            self.forceDict["CylindricalConfinement"].addParticle(i, [])
+    
     def addFlatBottomHarmonic(self, kr=5*10**-3, n_rad=10.0):
         
         R"""
         Sets a Flat-Bottom Harmonic potential to collapse the chromosome chain inside the nucleus wall. The potential is defined as: :math:`step(r-r0) * (kr/2)*(r-r0)^2`.
 
         Args:
 
@@ -505,15 +523,15 @@
                 angles.addAngle(end - 1, end , start, [ka[end]])
                 angles.addAngle(end , start, start + 1, [ka[start]])
 
         self.metadata["AngleForce"] = repr({"stiffness": ka})
         self.forceDict["AngleForce"] = angles
         
         
-    def addRepulsiveSoftCore(self, Ecut=4.0):
+    def addRepulsiveSoftCore(self, Ecut=4.0,CutoffDistance=3.0):
         
         R"""
         Adds a soft-core repulsive interaction that allows chain crossing, which represents the activity of topoisomerase II. Details can be found in the following publications: 
         
             - Oliveira Jr., A.B., Contessoto, V.G., Mello, M.F. and Onuchic, J.N., 2021. A scalable computational approach for simulating complexes of multiple chromosomes. Journal of Molecular Biology, 433(6), p.166700.
             - Di Pierro, M., Zhang, B., Aiden, E.L., Wolynes, P.G. and Onuchic, J.N., 2016. Transferable model for chromosome architecture. Proceedings of the National Academy of Sciences, 113(43), pp.12168-12173.
             - Naumova, N., Imakaev, M., Fudenberg, G., Zhan, Y., Lajoie, B.R., Mirny, L.A. and Dekker, J., 2013. Organization of the mitotic chromosome. Science, 342(6161), pp.948-953.
@@ -538,15 +556,15 @@
             repul_energy)
         repulforceGr = self.forceDict["RepulsiveSoftCore"]
         repulforceGr.addGlobalParameter('Epsi', self.Epsilon)
         repulforceGr.addGlobalParameter('Sig', self.Sigma)
         repulforceGr.addGlobalParameter('Ecut', Ecut)
         repulforceGr.addGlobalParameter('r_0', r_0)
         repulforceGr.addGlobalParameter('CutOff', nbCutOffDist)
-        repulforceGr.setCutoffDistance(3.0)
+        repulforceGr.setCutoffDistance(CutoffDistance)
 
         for _ in range(self.N):
             repulforceGr.addParticle(())
         
     def addTypetoType(self, mu=3.22, rc = 1.78 ):
         R"""
         Adds the type-to-type interactions according to the MiChroM energy function parameters reported in "Di Pierro, M., Zhang, B., Aiden, E.L., Wolynes, P.G. and Onuchic, J.N., 2016. Transferable model for chromosome architecture. Proceedings of the National Academy of Sciences, 113(43), pp.12168-12173". 
@@ -566,28 +584,28 @@
         path = "share/MiChroM.ff"
         pt = os.path.dirname(os.path.realpath(__file__))
         filepath = os.path.join(pt,path)
 
         self.addCustomTypes(name="TypetoType", mu=mu, rc=rc, TypesTable=filepath)
         
 
-    def addCustomTypes(self, name="CustomTypes", mu=3.22, rc = 1.78, TypesTable=None):
+    def addCustomTypes(self, name="CustomTypes", mu=3.22, rc = 1.78, TypesTable=None,CutoffDistance=3.0):
         R"""
         Adds the type-to-type potential using custom values for interactions between the chromatin types. The parameters :math:`\mu` (mu) and rc are part of the probability of crosslink function :math:`f(r_{i,j}) = \frac{1}{2}\left( 1 + tanh\left[\mu(r_c - r_{i,j}\right] \right)`, where :math:`r_{i,j}` is the spatial distance between loci (beads) *i* and *j*.
         
         The function receives a txt/TSV/CSV file containing the upper triangular matrix of the type-to-type interactions. A file example can be found `here <https://github.com/junioreif/OpenMiChroM/blob/main/OpenMiChroM/share/MiChroM.ff>`__.
         
         +---+------+-------+-------+
-        |   |   A  |   B   |   C   |
+        |  |   A  |   B   |   C   |
         +---+------+-------+-------+
-        | A | -0.2 | -0.25 | -0.15 |
+        |  | -0.2 | -0.25 | -0.15 |
         +---+------+-------+-------+
-        | B |      |  -0.3 | -0.15 |
+        |  |      |  -0.3 | -0.15 |
         +---+------+-------+-------+
-        | C |      |       | -0.35 |
+        |  |      |       | -0.35 |
         +---+------+-------+-------+
         
         Args:
 
             name (string, required):
                 Name to customType Potential. (Default value = "CustomTypes") 
             mu (float, required):
@@ -607,15 +625,15 @@
         energy = "mapType(t1,t2)*0.5*(1. + tanh(mu*(rc - r)))*step(r-lim)"
         
         crossLP = self.mm.CustomNonbondedForce(energy)
     
         crossLP.addGlobalParameter('mu', mu)
         crossLP.addGlobalParameter('rc', rc)
         crossLP.addGlobalParameter('lim', 1.0)
-        crossLP.setCutoffDistance(3.0)
+        crossLP.setCutoffDistance(CutoffDistance)
 
         tab = pd.read_csv(TypesTable, sep=None, engine='python')
 
         header_types = list(tab.columns.values)
 
         if not set(self.diff_types).issubset(set(header_types)):
             errorlist = []
@@ -682,15 +700,15 @@
         self.getLoops(looplists)
         
         for p in self.loopPosition:
             Loop.addBond(p[0]-1,p[1]-1)
   
         self.forceDict["Loops"] = Loop  
         
-    def addCustomIC(self, mu=3.22, rc = 1.78, dinit=3, dend=200, IClist=None):
+    def addCustomIC(self, mu=3.22, rc = 1.78, dinit=3, dend=200, IClist=None,CutoffDistance=3.0):
         R"""
         Adds the Ideal Chromosome potential using custom values for interactions between beads separated by a genomic distance :math:`d`. The parameters :math:`\mu` (mu) and rc are part of the probability of crosslink function :math:`f(r_{i,j}) = \frac{1}{2}\left( 1 + tanh\left[\mu(r_c - r_{i,j}\right] \right)`, where :math:`r_{i,j}` is the spatial distance between loci (beads) *i* and *j*.
         
         Args:
         
             mu (float, required):
                 Parameter in the probability of crosslink function. (Default value = 3.22).
@@ -721,26 +739,26 @@
         IC.addGlobalParameter('dinit', dinit) 
         IC.addGlobalParameter('dend', dend)
         
         IC.addGlobalParameter('mu', mu)  
         IC.addGlobalParameter('rc', rc) 
         IC.addGlobalParameter('lim', 1.0)
         
-        IC.setCutoffDistance(3.0)
+        IC.setCutoffDistance(CutoffDistance)
 
 
         IC.addPerParticleParameter("idx")
 
         for i in range(self.N):
                 IC.addParticle([i])
         
         self.forceDict["CustomIC"] = IC
         
     def addIdealChromosome(self, mu=3.22, rc = 1.78, Gamma1=-0.030,Gamma2=-0.351,
-                           Gamma3=-3.727, dinit=3, dend=500):
+                           Gamma3=-3.727, dinit=3, dend=500,CutoffDistance=3.0):
         
         R"""
         Adds the Ideal Chromosome potential for interactions between beads separated by a genomic distance :math:`d` according to the MiChroM energy function parameters reported in "Di Pierro, M., Zhang, B., Aiden, E.L., Wolynes, P.G. and Onuchic, J.N., 2016. Transferable model for chromosome architecture. Proceedings of the National Academy of Sciences, 113(43), pp.12168-12173". 
         
         The set of parameters :math:`\{\gamma_d\}` of the Ideal Chromosome potential is fitted in a function: :math:`\gamma(d) = \frac{\gamma_1}{\log{(d)}} +\frac{\gamma_2}{d} +\frac{\gamma_3}{d^2}`. 
         
         The parameters :math:`\mu` (mu) and rc are part of the probability of crosslink function :math:`f(r_{i,j}) = \frac{1}{2}\left( 1 + tanh\left[\mu(r_c - r_{i,j}\right] \right)`, where :math:`r_{i,j}` is the spatial distance between loci (beads) *i* and *j*.
@@ -775,27 +793,27 @@
         IC.addGlobalParameter('gamma3', Gamma3)
         IC.addGlobalParameter('dinit', dinit) 
         IC.addGlobalParameter('dend', dend) 
         
         IC.addGlobalParameter('mu', mu)  
         IC.addGlobalParameter('rc', rc) 
         
-        IC.setCutoffDistance(3.0)
+        IC.setCutoffDistance(CutoffDistance)
 
 
         IC.addPerParticleParameter("idx")
 
         for i in range(self.N):
                 IC.addParticle([i])
         
         self.forceDict["IdealChromosome"] = IC
         
         
     def addMultiChainIC(self, mu=3.22, rc = 1.78, Gamma1=-0.030,Gamma2=-0.351,
-                           Gamma3=-3.727, dinit=3, dend=500, chainIndex=0):
+                           Gamma3=-3.727, dinit=3, dend=500, chainIndex=0,CutoffDistance=3.0):
         
         R"""
         Adds the Ideal Chromosome potential for multiple chromosome simulations. The interactions between beads separated by a genomic distance :math:`d` is applied according to the MiChroM energy function parameters reported in "Di Pierro, M., Zhang, B., Aiden, E.L., Wolynes, P.G. and Onuchic, J.N., 2016. Transferable model for chromosome architecture. Proceedings of the National Academy of Sciences, 113(43), pp.12168-12173". 
         
         The set of parameters :math:`\{\gamma_d\}` of the Ideal Chromosome potential is fitted in a function: :math:`\gamma(d) = \frac{\gamma_1}{\log{(d)}} +\frac{\gamma_2}{d} +\frac{\gamma_3}{d^2}`. 
         
         The parameters :math:`\mu` (mu) and rc are part of the probability of crosslink function :math:`f(r_{i,j}) = \frac{1}{2}\left( 1 + tanh\left[\mu(r_c - r_{i,j}\right] \right)`, where :math:`r_{i,j}` is the spatial distance between loci (beads) *i* and *j*.
@@ -832,15 +850,15 @@
         IC.addGlobalParameter('gamma3', Gamma3)
         IC.addGlobalParameter('dinit', dinit)
         IC.addGlobalParameter('dend', dend)
       
         IC.addGlobalParameter('mu', mu)  
         IC.addGlobalParameter('rc', rc) 
         
-        IC.setCutoffDistance(3)
+        IC.setCutoffDistance(CutoffDistance)
         
         chain = self.chains[chainIndex]
 
         groupList = list(range(chain[0],chain[1]+1))
         
         IC.addInteractionGroup(groupList,groupList)
         
@@ -848,14 +866,158 @@
 
         for i in range(self.N):
             IC.addParticle([i])
         
         self.forceDict["IdealChromosomeChain{0}".format(chainIndex)] = IC
 
 
+    def addCorrelatedNoise(self, act_seq='none', atol=1e-5):
+        R"""
+        This function assigns active force to monomers, as defined by the act_seq array.
+        Args:
+            
+            act_seq (list, required): 
+                This list should contain the same number of elements as the number of monomers, where the value at index i corresponds to the active force F for the bead i
+
+            atol (float, optional):
+                tolerance for force values. If force is less than atol then it is ignored.
+
+        Returns Error if act_seq is not the same length as the sequence file.
+        """
+        
+        try:
+            act_seq=np.asfarray(act_seq)
+
+            #ensure all the monomers are accounted for
+            assert len(act_seq)==self.N
+
+            #do not redistribute velocities based on Maxwell Boltzman since this is a non-equilbrium sim
+            self.velocityReinitialize = False
+
+            #define active force group
+            act_force = self.mm.CustomExternalForce(" - F_act * (x + y + z)")
+            act_force.addPerParticleParameter('F_act')
+            self.forceDict["ActiveForce"] = act_force
+
+            # Important for the active force group to be set to "0". 
+            # This assignment is however overrun by _applyForces() inside runSimBlock(). 
+            # Hence it is necessary that active force is the *first* force field added to the simulation.
+            self.forceDict["ActiveForce"].setForceGroup(0)
+            
+            #assign correlated noise to the monomers with non-zero active force
+            for bead_id, Fval in enumerate(act_seq):
+                if Fval>atol:    
+                    self.forceDict["ActiveForce"].addParticle(int(bead_id),[Fval])
+
+            print('\n\
+            ==================================\n\
+            Active Monomers (correlated noise) added.\n\
+            Active correlation time: {}\n\
+            Total number of active monomers: {}\n\
+            Total number of monomers: {}\n\
+            ==================================\n'.format(self.integrator.corrTime, self.forceDict["ActiveForce"].getNumParticles(), self.N))
+        
+        except (AttributeError):
+            print("Structure not loaded! Load structure before adding activity.\nCorrelated noise has NOT been added!")
+            
+        except (ValueError, AssertionError):
+            print('Active sequence (act_seq) either not defined or all the monomers are not accounted for!\nCorrelated noise has NOT been added!')
+
+
+    def addHarmonicBonds(self, kfb=30.0, r0=1.0):
+        R"""
+        This function adds harmonic bonds to all the monomers within a chain
+        Args:
+            kfb (float, required): 
+                bond stiffness
+            
+            r0 (float, required):
+                equilibrium distance for the bond
+        """
+
+        for start, end, isRing in self.chains:
+            for j in range(start, end):
+                self.addHarmonicBond_ij(j, j + 1, kfb=kfb, r0=r0)
+
+            if isRing:
+                self.addHarmonicBond_ij(start, end, kfb=kfb, r0=r0)
+
+        self.metadata["HarmonicBond"] = repr({"kfb": kfb})
+        
+
+    def _initHarmonicBond(self, kfb=30,r0=1.0):
+        R"""
+        Internal function used to initiate Harmonic Bond force group
+        Args:
+            kfb (float, required): 
+                bond stiffness
+            
+            r0 (float, required):
+                equilibrium distance for the bond
+        """
+        
+        if "HarmonicBond" not in list(self.forceDict.keys()):
+            force = ("0.5 * kfb * (r-r0)*(r-r0)")
+            bondforceGr = self.mm.CustomBondForce(force)
+            bondforceGr.addGlobalParameter("kfb", kfb)
+            bondforceGr.addGlobalParameter("r0", r0) 
+                
+            self.forceDict["HarmonicBond"] = bondforceGr
+        
+
+    def addHarmonicBond_ij(self, i, j, r0=1.0, kfb=30):
+        R"""
+        Internal function used to add bonds between i and j monomers
+        Args:
+            i,j (int, required):
+                monomers to be bonded
+
+            kfb (float, required): 
+                bond stiffness
+            
+            r0 (float, required):
+                equilibrium distance for the bond
+        """
+        
+        if (i >= self.N) or (j >= self.N):
+            raise ValueError("\n Cannot add a bond between beads  %d,%d that are beyond the chromosome length %d" % (i, j, self.N))
+        
+        self._initHarmonicBond(kfb=kfb, r0=r0)
+        self.forceDict["HarmonicBond"].addBond(int(i), int(j), [])
+        self.bondsForException.append((int(i), int(j)))
+
+
+    def addSelfAvoidance(self, Ecut=4.0, k_rep=20.0, r0=1.0):
+        R"""
+        This adds Soft-core self avoidance between all non-bonded monomers.
+        This force is well behaved across all distances (no diverging parts)
+        Args:
+            Ecut (float, required): 
+                energy associated with full overlap between monomers
+            k_rep (float, required):
+                steepness of the sigmoid repulsive potential
+
+            r0 (float, required):
+                distance from the center at which the sigmoid is half as strong
+        """
+
+        Ecut = Ecut*self.Epsilon
+        repul_energy = ("0.5 * Ecut * (1.0 + tanh(1.0 - (k_rep * (r - r0))))")
+        
+        self.forceDict["SelfAvoidance"] = self.mm.CustomNonbondedForce(repul_energy)
+        repulforceGr = self.forceDict["SelfAvoidance"]
+        repulforceGr.addGlobalParameter('Ecut', Ecut)
+        repulforceGr.addGlobalParameter('r0', r0)
+        repulforceGr.addGlobalParameter('k_rep', k_rep)
+        repulforceGr.setCutoffDistance(3.0)
+
+        for _ in range(self.N):
+            repulforceGr.addParticle(())
+
+
     def _getForceIndex(self, forceName):
         R""""
         Get the index of one of the forces in the force dictionary.
         """   
 
         forceObject = self.forceDict[forceName]
 
@@ -890,15 +1052,15 @@
         """
 
         if forceName in self.forceDict:
             self.system.removeForce(self._getForceIndex(forceName))
             del self.forceDict[forceName]
 
             self.context.reinitialize(preserveState=True) 
-
+            print(f"Removed {forceName} from the system!")
             assert self._isForceDictEqualSystemForces(), 'Forces in forceDict should be the same as in the system!'
 
         else:
             raise ValueError("The system does not have force {0}.\nThe forces applied in the system are: {}\n".format(forceName, self.forceDict.keys()))
 
 
     def removeFlatBottomHarmonic(self):
@@ -908,50 +1070,77 @@
 
         forceName = "FlatBottomHarmonic"
 
         self.removeForce(forceName)
 
 
     def addAdditionalForce(self, forceFunction, **args):
-        R""""
+        R"""
         Add an additional force after the system has already been initialized.
 
         Args:
 
             forceFunciton (function, required):
                 Force function to be added. Example: addSphericalConfinementLJ
             **args (collection of arguments, required):
                 Arguments of the function to add the force. Consult respective documentation.
         """
-
-        try:
-            forceFunction in dir(self)
-        except:
-            raise ValueError("No function with name '{:}' found!".format(forceFunction))
-
-        oldForceDictKeys = [x for x in self.forceDict.keys()]
-
+        
+        assert isinstance(forceFunction, types.MethodType), f"No function with name {forceFunction}! \
+                                                You can only add functions that are defined as a method of the simulation object"
+        #store old forcedict keys
+        oldForceDictKeys = list(self.forceDict.keys())
+        
+        # call the function --  
+        # the force name is added to the forceDict but not yet added to the system
         forceFunction(**args)
 
-        newForceDictKey = [i for i in self.forceDict.keys() if i not in oldForceDictKeys][0]
-
-        self.system.addForce(self.forceDict[newForceDictKey])
-        self.context.reinitialize(preserveState=True) 
+        # find the new forceDict name
+        newForceDictKey_list = list(set(oldForceDictKeys)^set(self.forceDict.keys()))
+        assert len(newForceDictKey_list)==1, "The force you are adding is already present! Try removing it first and then add"
+        newForceDictKey = newForceDictKey_list[0]
+        force = self.forceDict[newForceDictKey]
+        
+        # exclusion list
+        exc = self.bondsForException
 
-        forceGroups = [i.getForceGroup() for i in self.forceDict.values()]
+        # set all the attributes of the force (see _applyForces)
+        if hasattr(force, "addException"):
+            print('Add exceptions for {0} force'.format(newForceDictKey))
+            for pair in exc:
+                force.addException(int(pair[0]),
+                    int(pair[1]), 0, 0, 0, True)
+                
+        elif hasattr(force, "addExclusion"):
+            print('Add exclusions for {0} force'.format(newForceDictKey))
+            for pair in exc:
+                force.addExclusion(int(pair[0]), int(pair[1]))
+
+        if hasattr(force, "CutoffNonPeriodic") and hasattr(
+                                                force, "CutoffPeriodic"):
+            if self.PBC:
+                force.setNonbondedMethod(force.CutoffPeriodic)
+                print("Using periodic boundary conditions!!!!")
+            else:
+                force.setNonbondedMethod(force.CutoffNonPeriodic)
         
-        i = 0
-        while i in forceGroups:
-            i += 1
+        # add the force
+        print("adding force ", newForceDictKey, self.system.addForce(self.forceDict[newForceDictKey]))
 
-        if i < 32:
-            self.forceDict[newForceDictKey].setForceGroup(i)
-        else:
-            self.forceDict[newForceDictKey].setForceGroup(31)
-            print("Attention, force was added to Force Group 31 because no other was available.")
+        #assign force groups
+        for name in self.forceDict.keys():
+            force_group = self.forceDict[name].getForceGroup()
+            if force_group>31: 
+                force_group=31
+                print("Attention, force was added to Force Group 31 because no other was available.")
+            
+            self.forceDict[name].setForceGroup(force_group)
+
+        # reinitialize the system with the new force after force group assignments
+        self.context.reinitialize(preserveState=True) 
         
         assert self._isForceDictEqualSystemForces(), 'Forces in forceDict should be the same as in the system!'
 
 
     def _loadParticles(self):
         R"""
         Internal function that loads the chromosome beads into the simulations system.
@@ -1657,14 +1846,15 @@
                 gro_string.append(self.name +"_" + str(chainNum))
                 gro_string.append(len(data_chain))
                 
                 totalAtom = 1
                 for i, line in zip(types_chain, data_chain):
                     if not i in Res_conversion:
                         Res_conversion[i] = 'GLY'
+                        Type_conversion[i] = 'CA'
                     
                     gro_string.append(str(gro_style.format(totalAtom, Res_conversion[i],Type_conversion[i],totalAtom,
                                     float(line[0]), float(line[1]), float(line[2]))))
                     
                     totalAtom += 1
                         
                 gro_string.append(str(gro_box_string.format(0.000,0.000,0.000)))
@@ -2028,15 +2218,15 @@
         forceValues.append(self.context.getState(getEnergy=True).getPotentialEnergy().value_in_unit(units.kilojoules_per_mole)/self.N)
         df = pd.DataFrame(forceValues,forceNames)
         df.columns = ['Values']
         print(df)
 
     def printHeader(self):
         print('{:^96s}'.format("***************************************************************************************"))
-        print('{:^96s}'.format("**** **** *** *** *** *** *** *** OpenMiChroM-1.0.5 *** *** *** *** *** *** **** ****"))
+        print('{:^96s}'.format("**** **** *** *** *** *** *** *** OpenMiChroM-1.0.7 *** *** *** *** *** *** **** ****"))
         print('')
         print('{:^96s}'.format("OpenMiChroM is a Python library for performing chromatin dynamics simulations."))
         print('{:^96s}'.format("OpenMiChroM uses the OpenMM Python API,"))
         print('{:^96s}'.format("employing the MiChroM (Minimal Chromatin Model) energy function."))
         print('{:^96s}'.format("The chromatin dynamics simulations generate an ensemble of 3D chromosomal structures"))
         print('{:^96s}'.format("that are consistent with experimental Hi-C maps, also allows simulations of a single"))
         print('{:^96s}'.format("or multiple chromosome chain using High-Performance Computing "))
@@ -2047,11 +2237,11 @@
         print('{:^96s}'.format("A Scalable Computational Approach for Simulating Complexes of Multiple Chromosomes."))
         print('{:^96s}'.format("Journal of Molecular Biology. doi:10.1016/j.jmb.2020.10.034."))
         print('{:^96s}'.format("and"))
         print('{:^96s}'.format("Oliveira Junior, A. B. et al."))
         print('{:^96s}'.format("Chromosome Modeling on Downsampled Hi-C Maps Enhances the Compartmentalization Signal."))
         print('{:^96s}'.format("J. Phys. Chem. B, doi:10.1021/acs.jpcb.1c04174."))
         print('')
-        print('{:^96s}'.format("Copyright (c) 2022, The OpenMiChroM development team at"))
+        print('{:^96s}'.format("Copyright (c) 2023, The OpenMiChroM development team at"))
         print('{:^96s}'.format("Rice University"))
         print('{:^96s}'.format("***************************************************************************************"))
         stdout.flush()
```

### Comparing `OpenMiChroM-1.0.6/OpenMiChroM/CndbTools.py` & `OpenMiChroM-1.0.7/OpenMiChroM/CndbTools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2022 The Center for Theoretical Biological Physics (CTBP) - Rice University
+# Copyright (c) 2020-2023 The Center for Theoretical Biological Physics (CTBP) - Rice University
 # This file is from the Open-MiChroM project, released under the MIT License.
 
 R"""
 The :class:`~.cndbTools` class perform analysis from **cndb** or **ndb** - (Nucleome Data Bank) file format for storing an ensemble of chromosomal 3D structures.
 Details about the NDB/CNDB file format can be found at the `Nucleome Data Bank <https://ndb.rice.edu/ndb-format>`__.
 """
 
@@ -343,37 +343,37 @@
                        
         Returns:
             :class:`numpy.ndarray` (dim: NxT):
                 Returns the MSD of each particle over the trajectory.
 
         """
         
-        msd=[_msd_fft(xyz[:,mono_id,:]) for mono_id in range(xyz.shape[1])]
+        msd=[self._msd_fft(xyz[:,mono_id,:]) for mono_id in range(xyz.shape[1])]
         return np.array(msd)
         
 
-    def _autocorrFFT(x):
+    def _autocorrFFT(self, x):
         R"""
         Internal function. 
         """
         N=len(x)
         F = np.fft.fft(x,n=2*N)  #2*N because of zero-padding
         res = np.fft.ifft(F * F.conjugate()) #autocorrelation using Weiner Kinchin theorem
         res = (res[:N]).real   
         return res/(N-np.arange(0,N)) #this is the normalized autocorrelation
 
         #r is an (T,3) ndarray: [time stamps,dof]
-    def _msd_fft(r):
+    def _msd_fft(self, r):
         R"""
         Internal function. 
         """
         N=len(r)
         D=np.square(r).sum(axis=1)
         D=np.append(D,0)
-        S2=sum([_autocorrFFT(r[:, i]) for i in range(r.shape[1])])
+        S2=sum([self._autocorrFFT(r[:, i]) for i in range(r.shape[1])])
         Q=2*D.sum()
         S1=[]
         for m in range(N):
             Q=Q-D[m-1]-D[N-m]
             S1.append(Q/(N-m))
         return np.array(S1) - 2*S2
```

### Comparing `OpenMiChroM-1.0.6/OpenMiChroM/Optimization.py` & `OpenMiChroM-1.0.7/OpenMiChroM/Optimization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2022 The Center for Theoretical Biological Physics (CTBP) - Rice University
+# Copyright (c) 2020-2023 The Center for Theoretical Biological Physics (CTBP) - Rice University
 # This file is from the Open-MiChroM project, released under the MIT License.
 
 R"""  
 The :class:`~.Optimization` classes perform the energy function parameters training of the chromosomes based on experimental Hi-C data.
 """
 
 # with OpenMM 7.7.0, the import calls have changed. So, try both, if needed
@@ -13,24 +13,24 @@
     except:
         # earlier
         print('Unable to load OpenMM as \'openmm\'. Will try the older way \'simtk.openmm\'')
         from simtk.openmm.app import *
 except:
     print('Failed to load OpenMM. Check your configuration.')
 
-
 import numpy as np
 import random
 from scipy.spatial import distance
-import scipy as sp
+import scipy as sc
 import itertools
 from scipy.stats.stats import pearsonr
 from sklearn.preprocessing import normalize
 import os
 import pandas as pd
+import warnings
 
 class AdamTraining:
     R"""
     The :class:`~.AdamTraining` class performs the parameters training for each selected loci pair interaction. 
     
     Details about the methodology are decribed in "Zhang, Bin, and Peter G. Wolynes. "Topology, structures, and energy landscapes of human chromosomes." Proceedings of the National Academy of Sciences 112.19 (2015): 6062-6067."
     
@@ -89,61 +89,218 @@
 
         ## update weights and biases
         w = w - self.eta*(m_dw_corr/(np.sqrt(v_dw_corr)+self.epsilon))
         b = b - self.eta*(m_db_corr/(np.sqrt(v_db_corr)+self.epsilon))
         self.t += 1
         return w, b
 
-    def getPars(self, HiC, centerRemove=False, centrange=[0,0], cutoff= 0.0):
+    def knight_ruiz_balance(matrix, tol=1e-5, max_iter=100):
+        R"""
+        Perform the Knight-Ruiz matrix balancing.
+        """
+        A = np.array(matrix, dtype=float)
+        n = A.shape[0]
+        row_scaling = np.ones(n)
+        col_scaling = np.ones(n)
+
+        for _ in range(max_iter):
+            row_scaling = np.sqrt(np.sum(A, axis=1))
+            A /= row_scaling[:, None]
+            col_scaling = np.sqrt(np.sum(A, axis=0))
+            A /= col_scaling
+
+            if np.all(np.abs(row_scaling - 1) < tol) and np.all(np.abs(col_scaling - 1) < tol):
+                break
+
+        return A
+
+
+    def normalize_matrix(matrix):
+        R"""
+        Normalize the matrix for simulation optimization. Here the first neighbor should have the probability of contact P=1.0.
+        """
+        matrix = np.nan_to_num(matrix, nan=0, posinf=0, neginf=0)
+        np.fill_diagonal(matrix,0.0)
+
+        max_values = np.amax(np.triu(matrix), axis=1)
+        
+        # To avoid division by zero, replace zeros with ones
+        max_values[max_values == 0] = 0.0000001
+        
+        normalized_matrix = np.triu(matrix) / max_values[:, np.newaxis]
+        # return normalized_matrix
+        matrix= normalized_matrix + np.triu(normalized_matrix,k=1).T
+        np.fill_diagonal(matrix,1.0)
+
+        return matrix
+
+
+    def getPars(self, HiC, centerRemove=False, centrange=[0,0], cutoff='deprecate', norm=True, cutoff_low=0.0, cutoff_high=1.0, KR=False, neighbors=0):
         R"""
         Receives the experimental Hi-C map (Full dense matrix) in a text format and performs the data normalization from Hi-C frequency/counts/reads to probability.
         
         Args:
             HiC (file, required):
                 Experimental Hi-C map (Full dense matrix) in a text format.
             centerRemove (bool, optional):
                 Whether to set the contact probability of the centromeric region to zero. (Default value: :code:`False`).
             centrange (list, required if **centerRemove** = :code:`True`)):
                 Range of the centromeric region, *i.e.*, :code:`centrange=[i,j]`, where *i* and *j*  are the initial and final beads in the centromere. (Default value = :code:`[0,0]`).
             cutoff (float, optional):
                 Cutoff value for reducing the noise in the original data. Values lower than the **cutoff** are considered :math:`0.0`.
         """
-        allmap = np.loadtxt(HiC)
+        
+        warnings.warn("getPars is deprecated, use getHiCexp instead", DeprecationWarning)
+        # get the file extension
+        _, file_extension = os.path.splitext(HiC)
+        if file_extension == '.npy':
+            # use np.load if the file is a .npy file
+            allmap = np.load(HiC)
+        else:
+            allmap = np.loadtxt(HiC)
 
-        r=np.triu(allmap, k=1)
-        r[np.isinf(r)]= 0.0
-        r[np.isnan(r)]= 0.0
-        r = normalize(r, axis=1, norm='max')
+        if KR==True:
+            allmap = knight_ruiz_balance(allmap)
 
-        for i in range(len(r)-1):
-            maxElem = r[i][i+1]
-            if (maxElem != np.max(r[i])):
-                for j in range(len(r[i])):
-                    if maxElem != 0.0:
-                        r[i][j] = float(r[i][j] / maxElem)
-                    else:
-                        r[i][j] = 0.0 
-                    if r[i][j] > 1.0:
-                        r[i][j] = 0.5
+        if norm==True:
+            r=normalize_matrix(allmap)
 
-        rd = np.transpose(r) 
-        self.expHiC = r+rd + np.diag(np.ones(len(r)))
+            for i in range(len(r)-1):
+                maxElem = r[i][i+1]
+                if (maxElem != np.max(r[i])):
+                    for j in range(len(r[i])):
+                        if maxElem != 0.0:
+                            r[i][j] = float(r[i][j] / maxElem)
+                        else:
+                            r[i][j] = 0.0 
+                        if r[i][j] > 1.0:
+                            r[i][j] = 0.5
+
+            rd = np.transpose(r) 
+            self.expHiC = r+rd + np.diag(np.ones(len(r)))
+        else:
+            self.expHiC = allmap
         
         if (centerRemove):
             centrome = range(centrange[0],centrange[1])
             self.expHiC[centrome,:] = 0.0
             self.expHiC[:,centrome] = 0.0
         
         #remove noise by cutoff    
-        self.expHiC[self.expHiC<cutoff] = 0.0
+        if cutoff!='deprecate':
+            print('Depreaction warning!\nUsing `cutoff` in getPars is deprecated! Use either `cutoff_low` or `cutoff_high`. \nSetting cutoff_low=cutoff! \n')
+            assert type(cutoff)==float, 'Cut off must be a float'
+            cutoff_low = cutoff
+
+        if cutoff_low>0.0:
+            self.expHiC[self.expHiC<cutoff_low] = 0.0
+        
+        if cutoff_high<1.0:
+            self.expHiC[self.expHiC>cutoff_high] = 0.0
+
+        # Remove the number of Neighbors to optimize.
+        M=self.expHiC
+        neighbor_mask = np.abs(np.subtract.outer(np.arange(len(M)), np.arange(len(M)))) <= neighbors
+        M[neighbor_mask] = 0.0
+        self.expHiC = M
+
+        self.mask = self.expHiC == 0.0
+
+        self.phi_exp = self.expHiC
+        self.reset_Pi()
+    
+    def reset_Pi(self):
+        R"""
+        Resets Pi matrix to zeros
+        """
+        if not hasattr(self, "phi_exp"):
+            print("Cannot reset Pi; HiC map shape unknown. Load HiC map first!")
+        else:              
+            self.Pi = np.zeros(self.phi_exp.shape)
+            self.NFrames = 0
+
+
+    def getHiCexp(self, HiC, centerRemove=False, centrange=[0,0], norm=True, cutoff_low=0.0, cutoff_high=1.0, KR=False, neighbors=0):
+        R"""
+        Receives the experimental Hi-C map (Full dense matrix) in a text format and performs the data normalization from Hi-C frequency/counts/reads to probability.
+        
+        Args:
+            HiC (file, required):
+                Experimental Hi-C map (Full dense matrix) in a text format.
+            centerRemove (bool, optional):
+                Whether to set the contact probability of the centromeric region to zero. (Default value: :code:`False`).
+            centrange (list, required if **centerRemove** = :code:`True`)):
+                Range of the centromeric region, *i.e.*, :code:`centrange=[i,j]`, where *i* and *j*  are the initial and final beads in the centromere. (Default value = :code:`[0,0]`).
+            cutoff (float, optional):
+                Cutoff value for reducing the noise in the original data. Values lower than the **cutoff** are considered :math:`0.0`.
+        """
+
+        # get the file extension
+        _, file_extension = os.path.splitext(HiC)
+        if file_extension == '.npy':
+            # use np.load if the file is a .npy file
+            allmap = np.load(HiC)
+        else:
+            allmap = np.loadtxt(HiC)
+
+        if KR==True:
+            allmap = knight_ruiz_balance(allmap)
+
+        if norm==True:
+            r=normalize_matrix(allmap)
+
+            for i in range(len(r)-1):
+                maxElem = r[i][i+1]
+                if (maxElem != np.max(r[i])):
+                    for j in range(len(r[i])):
+                        if maxElem != 0.0:
+                            r[i][j] = float(r[i][j] / maxElem)
+                        else:
+                            r[i][j] = 0.0 
+                        if r[i][j] > 1.0:
+                            r[i][j] = 0.5
+
+            rd = np.transpose(r) 
+            self.expHiC = r+rd + np.diag(np.ones(len(r)))
+        else:
+            self.expHiC = allmap
+        
+        if (centerRemove):
+            centrome = range(centrange[0],centrange[1])
+            self.expHiC[centrome,:] = 0.0
+            self.expHiC[:,centrome] = 0.0
+        
+        #remove noise by cutoff 
+
+        if cutoff_low>0.0:
+            self.expHiC[self.expHiC<cutoff_low] = 0.0
+        
+        if cutoff_high<1.0:
+            self.expHiC[self.expHiC>cutoff_high] = 0.0
+
+        # Remove the number of Neighbors to optimize.
+        M=self.expHiC
+        neighbor_mask = np.abs(np.subtract.outer(np.arange(len(M)), np.arange(len(M)))) <= neighbors
+        M[neighbor_mask] = 0.0
+        self.expHiC = M
 
         self.mask = self.expHiC == 0.0
 
-        self.phi_exp = self.expHiC #np.triu(self.expHiC, k=1)
-        self.Pi = np.zeros(self.phi_exp.shape)
+        self.phi_exp = self.expHiC
+        self.reset_Pi()
+    
+    def reset_Pi(self):
+        R"""
+        Resets Pi matrix to zeros
+        """
+        if not hasattr(self, "phi_exp"):
+            print("Cannot reset Pi; HiC map shape unknown. Load HiC map first!")
+        else:              
+            self.Pi = np.zeros(self.phi_exp.shape)
+            self.NFrames = 0
 
     def probCalc(self, state):
         R"""
         Calculates the contact probability matrix for a given state.
         """
 
         Pi = 0.5*(1.0 + np.tanh(self.mu*(self.rc - distance.cdist(state,state, 'euclidean'))))
@@ -227,15 +384,15 @@
                 ):
             
         self.mi = mu
         self.rc = rc
         self.cutoff = cutoff
         
         self.getHiCexp(expHiC, centerRemove=False, centrange=[0,0])
-        self.hic_sparse = sp.sparse.csr_matrix(np.triu(self.expHiC, k=2))
+        self.hic_sparse = sc.sparse.csr_matrix(np.triu(self.expHiC, k=2))
         if (reduce):
             self.appCutoff(pair_h, c_h, pair_l, c_l)
        
 
         self.ind = self.get_indices(self.hic_sparse)
 
         self.size = len(self.ind)     
@@ -265,65 +422,40 @@
 
         values = [n for n in range(0,N,pair_h)]
         index =  [x for x in itertools.combinations_with_replacement(values, r=2)]
         for i in index:
             if (hic_full[i] > c_h):
                 hic_final[i] = hic_full[i]
 
-        high_cut_number =   sp.sparse.csr_matrix(np.triu(hic_final, k=2)).nnz
+        high_cut_number =   sc.sparse.csr_matrix(np.triu(hic_final, k=2)).nnz
         print('Non-zero interactions after high-resolution cutoff ({}): {}'.format( c_h, high_cut_number ))
 
         values = [n for n in range(1,N,pair_l)]
         index =  [x for x in itertools.combinations_with_replacement(values, r=2)]
         for i in index:
             if (hic_full[i] > c_l):
                 hic_final[i] = hic_full[i]
-        self.hic_sparse = sp.sparse.csr_matrix(np.triu(hic_final, k=2))
+        self.hic_sparse = sc.sparse.csr_matrix(np.triu(hic_final, k=2))
         print('Non-zero interactions after low-resolution cutoff ({}): {}'.format(c_l,  (self.hic_sparse.nnz-high_cut_number) ))
         print('Total Non-zero interactions: {}'.format(self.hic_sparse.nnz))
 
     
     def get_indices(self, hic):
         R"""
         Receives non-zero interaction indices, *i.e.*, the loci pair *i* and *j* which interaction will be optimized.
         """
-        index = sp.sparse.find(hic)
+        index = sc.sparse.find(hic)
         self.rows = index[0]
         self.cols = index[1]
         self.values = index[2]
         ind = []
         for i in range(len(index[0])):
             ind.append((self.rows[i], self.cols[i]))
         return(ind)
         
-    def getHiCexp(self, filename, centerRemove=False, centrange=[0,0]):
-        R"""
-        Receives the experimental Hi-C map (Full dense matrix) in a text format and performs the data normalization from Hi-C frequency/counts/reads to probability.
-        
-        Args:
-            centerRemove (bool, optional):
-                Whether to set the contact probability of the centromeric region to zero. (Default value: :code:`False`).
-            centrange (list, required if **centerRemove** = :code:`True`)):
-                Range of the centromeric region, *i.e.*, :code:`centrange=[i,j]`, where *i* and *j*  are the initial and final beads in the centromere. (Default value = :code:`[0,0]`).
-        """
-        allmap = np.loadtxt(filename)
-
-        r=np.triu(allmap, k=1)
-        r[np.isinf(r)]= 0.0
-        r[np.isnan(r)]= 0.0
-        r = normalize(r, axis=1, norm='max') 
-        rd = np.transpose(r) 
-        self.expHiC = r+rd + np.diag(np.ones(len(r)))
-        
-        if (centerRemove):
-            centrome = range(centrange[0],centrange[1])
-            self.expHiC[centrome,:] = 0.0
-            self.expHiC[:,centrome] = 0.0
-        self.expHiC[self.expHiC<self.cutoff] = 0.0
-        
     def probCalc(self, state):
         R"""
         Calculates the contact probability matrix and the cross term of the Hessian.
         """
 
         Prob = 0.5*(1.0 + np.tanh(self.mi*(self.rc - distance.cdist(state,state, 'euclidean'))))
     
@@ -341,15 +473,15 @@
         self.Pi += Pi
         self.NFrames += 1
         
     def getPearson(self):
         R"""
         Calculates the Pearson's Correlation between the experimental Hi-C used as a reference for the training and the *in silico* Hi-C obtained from the optimization step.
         """
-        r1 = sp.sparse.csr_matrix((self.Pi/self.NFrames,(self.rows,self.cols)), shape=(self.expHiC.shape[0],self.expHiC.shape[0])).todense()
+        r1 = sc.sparse.csr_matrix((self.Pi/self.NFrames,(self.rows,self.cols)), shape=(self.expHiC.shape[0],self.expHiC.shape[0])).todense()
         r2 = self.hic_sparse.todense()
 
         r1[np.isinf(r1)]= 0.0
         r1[np.isnan(r1)]= 0.0
         r1[r1 <= 0.001]= 0.0
         r2[np.isinf(r2)]= 0.0
         r2[np.isnan(r2)]= 0.0
@@ -392,26 +524,25 @@
 
         Pi2_mean = np.outer(self.phi_sim,self.phi_sim)
 
         PiPj_mean = self.PiPj/self.NFrames
 
         Bij = PiPj_mean - Pi2_mean
         
-        invBij = sp.linalg.pinvh(Bij)
+        invBij = sc.linalg.pinvh(Bij)
 
         lambdas = np.matmul(invBij, gij)
 
         
-        lamb_matrix = sp.sparse.csr_matrix((lambdas,(self.rows,self.cols)), shape=(self.expHiC.shape[0],self.expHiC.shape[0]))
+        lamb_matrix = sc.sparse.csr_matrix((lambdas,(self.rows,self.cols)), shape=(self.expHiC.shape[0],self.expHiC.shape[0]))
         
         self.error = (np.sum(np.absolute(gij)))/(np.sum(self.phi_exp))
         
         return(lamb_matrix)
 
-
 class CustomMiChroMTraining:
     R"""
     The :class:`~.CustomMiChroMTraining` class performs the parameters training employing MiChroM (Minimal Chromatin Model) energy function. 
     
     Details about the methodology are decribed in "Di Pierro, Michele, et al. "Transferable model for chromosome architecture." Proceedings of the National Academy of Sciences 113.43 (2016): 12168-12173."
     
     
@@ -426,28 +557,30 @@
                 A txt/TSV/CSV file containing the upper triangular matrix of the type-to-type interactions. (Default value: :code:`None`).
         mu (float, required):
             Parameter in the probability of crosslink function (Default value = 3.22, for human chromosomes in interphase).
         rc (float, required):
             Parameter in the probability of crosslink function, :math:`f(rc) = 0.5` (Default value = 1.78, for human chromosomes in interphase).
         cutoff (float, optional):
             Cutoff value for reducing the noise in the original data. Values lower than the **cutoff** are considered :math:`0.0`.
+        IClist (file, required for Ideal Chromosome training):
+            A one-column text file containing the energy interaction values for loci *i* and *j* separated by a genomic distance :math:`d`. The list should be at least of the size :math:`dend-dinit`. (Default value: :code:`None`).
         dinit (int, required):
             The first neighbor in sequence separation (Genomic Distance) to be considered in the Ideal Chromosome potential for training. (Default value = 3).
         dend (int, required):
             The last neighbor in sequence separation (Genomic Distance) to be considered in the Ideal Chromosome potential for training. (Default value = 200).
     """
    
-    def __init__(self, ChromSeq="chr_beads.txt", TypesTable=None, mu=3.22, rc=1.78, cutoff=0.0, dinit=3, dend=200): 
-        self.ChromSeq = self.getChromSeq(ChromSeq)
+    def __init__(self, ChromSeq="chr_beads.txt", TypesTable=None, mu=3.22, rc=1.78, cutoff=0.0, IClist=None, dinit=3, dend=200): 
+        self.ChromSeq = self._get_chrom_seq(ChromSeq)
         self.size = len(self.ChromSeq)
         self.P=np.zeros((self.size,self.size))
         self.Pold=np.zeros((self.size,self.size))
         self.r_cut = rc 
         self.mu  = mu
-        self.Bij = np.zeros((dend,dend))
+        
         tab = pd.read_csv(TypesTable, sep=None, engine='python')
         self.header_types = list(tab.columns.values) 
         self.diff_types = set(self.ChromSeq)
 
         if not self.diff_types.issubset(set(self.header_types)):
             errorlist = []
             for i in self.diff_types:
@@ -455,141 +588,161 @@
                     errorlist.append(i)
             raise ValueError("Types: {} are not present in TypesTables: {}\n".format(errorlist, self.header_types))
 
         self.lambdas_old = np.triu(tab.values) + np.triu(tab.values, k=1).T
 
         self.n_types = len(self.diff_types)
         self.n_inter = int(self.n_types*(self.n_types-1)/2 + self.n_types)
-        self.polds_type = np.zeros((self.n_types, self.n_types))
-        self.Bij_type = np.zeros((self.n_inter,self.n_inter))
+        self.Pold_type = np.zeros((self.n_types, self.n_types))
+        self.PiPj_type = np.zeros((self.n_inter,self.n_inter))
         self.Nframes = 0 
+        
+        self.PiPj_IC = np.zeros((dend-dinit,dend-dinit))
         self.dinit = dinit
+        self.dend = dend
         self.cutoff = cutoff
 
-    def getChromSeq(self, filename):
-        R"""Converts the letters of the types/compartments following the rule: 'A1':0, 'A2':1, 'B1':2, 'B2':3,'B3':4,'B4':5, 'NA' :6.
+        if not IClist == None:
+            try:
+                f = open(str(IClist),"r")
+                self.IClist = IClist
+            except IOError:
+                print("Error in opening the file containing the Ideal Chromosome interactions!")
+
+    def _get_chrom_seq(self, filename):
+        R"""Reads the chromatin sequence as letters of the types/compartments.
         
         Args:
 
             filename (file, required):
                 Chromatin sequence of types file. The first column should contain the locus index. The second column should have the locus type annotation. A template of the chromatin sequence of types file can be found at the `Nucleome Data Bank (NDB) <https://ndb.rice.edu/static/text/chr10_beads.txt>`_.
                 
         Returns:
             :math:`(N,1)` :class:`numpy.ndarray`:
                 Returns an array of the sequence of chromatin types.
 
-        """              
+        """
 
         my_list = []
         af = open(filename,'r')
         pos = af.read().splitlines()
         for t in range(len(pos)):
             pos[t] = pos[t].split()
             my_list.append(pos[t][1])
 
         return np.array(my_list)
         
-    
-    def probCalculation_IC(self, state, dmax=200):
+    def prob_calculation_IC(self, state):
         R"""
         Calculates the contact probability matrix and the cross term of the Hessian for the Ideal Chromosome optimization.
         """
+
+        dmax = self.dend - self.dinit
+
         self.Pold += self.P
         self.P = 0.5*(1.0 + np.tanh(self.mu*(self.r_cut - distance.cdist(state,state, 'euclidean'))))
         self.P[self.P<self.cutoff] = 0.0
-        Pi = []
+        
+        Pi = np.array([])
         for i in range(dmax):
-             Pi.append(np.mean(np.diagonal(self.P, offset=(i+self.dinit))))
+             Pi = np.append(Pi, np.mean(np.diagonal(self.P, offset=(i+self.dinit))))
+        
         PiPj = np.outer(Pi, Pi)
-      
-        self.Bij += PiPj
+        self.PiPj_IC += PiPj
         self.Nframes += 1 
         
-    
-    def calc_sim_phi(self, init=3, dmax=200):
+    def calc_phi_sim_IC(self):
         R"""
         Calculates the contact probability as a function of the genomic distance from simulations for the Ideal Chromosome optimization.
         """
+        dmax = self.dend - self.dinit
         phi = np.zeros(dmax)
-        pmean = self.Pold/self.Nframes
+        Pmean = self.Pold/self.Nframes
         for i in range(dmax):
-             phi[i] =  np.mean(np.diagonal(pmean, offset=(i+init)))
+             phi[i] =  np.mean(np.diagonal(Pmean, offset=(i+self.dinit)))
         return phi
     
-    def getBijsim(self):
+    def get_PiPj_sim_IC(self):
         R"""
         Normalizes the cross term of the Hessian by the number of frames in the simulation for the Ideal Chromosome optimization.
         """
-        return self.Bij/self.Nframes
+        return self.PiPj_IC/self.Nframes
     
-    def getHiCexp(self, filename):
+    def get_HiC_exp(self, filename):
         R"""
         Receives the experimental Hi-C map (Full dense matrix) in a text format and performs the data normalization from Hi-C frequency/counts/reads to probability.
         """
         allmap = np.loadtxt(filename)
 
         r=np.triu(allmap, k=1)
         r[np.isinf(r)]= 0.0
         r[np.isnan(r)]= 0.0
         r = normalize(r, axis=1, norm='max')
         rd = np.transpose(r)
         self.expHiC = r+rd + np.diag(np.ones(len(r)))
         self.expHiC[self.expHiC<self.cutoff] = 0.0
 
-    def calc_exp_phi(self, init=3, dmax=200):
+    def calc_phi_exp_IC(self):
         R"""
         Calculates the contact probability as a function of the genomic distance from the experimental Hi-C for the Ideal Chromosome optimization.
         """
+        dmax = self.dend - self.dinit
         phi = np.zeros(dmax)
         for i in range(dmax):
-             phi[i] =  np.mean(np.diagonal(self.expHiC, offset=(i+init)))
+             phi[i] =  np.mean(np.diagonal(self.expHiC, offset=(i+self.dinit)))
         return phi
     
-    def getlambfromfile(self, filename):
-        R"""
-        Receives the Lagrange multipliers of the Ideal Chromosome optimization from a text file.
-        """
-        aFile = open(filename,'r')
-        pos = aFile.read().splitlines()
-        for t in range(len(pos)):
-            pos[t] = float(pos[t])
-        return np.array(pos)
-    
-    def getLamb(self, dmax=200, exp_map='file.dense'):
+    def get_lambdas_IC(self, exp_map='file.dense', damp=3*10**-7, write_error=True):
         R"""
         Calculates the Lagrange multipliers for the Ideal Chromosome optimization and returns a array containing the energy values for the IC optimization step.
+        Args:
+            exp_map (file, required):
+                The experimental Hi-C map with the .dense file. (Default value: :code:`file.dense`).
+            damp (float):
+                The learning parameter for the new lambda. (Default value = :math:`3*10**-7`).
+            dmax (float):
+                The maximum distance in the sequence separation (Genomic Distance) to be considered for the convergence of the potential interations. (Default value = 200).    
+                The learning parameter for the new lambda. (Default value = :math:`3*10**-7`).
+            write_error (boolean):
+                Flag to write the tolerance and Pearson's correlation values. (Default value: :code:`True`). 
         """    
-        self.getHiCexp(exp_map)
+        
+        dmax = self.dend - self.dinit
 
+        self.get_HiC_exp(exp_map)
         
-        phi_exp = self.calc_exp_phi(init=self.dinit, dmax=dmax)
+        phi_exp = self.calc_phi_exp_IC()
         
-        phi_sim = self.calc_sim_phi(init=self.dinit, dmax=dmax)
+        phi_sim = self.calc_phi_sim_IC()
         
-        gij = -phi_sim + phi_exp   # *1/beta = 1     
+        g = -phi_sim + phi_exp   # *1/beta = 1     
     
-        Res = np.zeros((dmax,dmax))
-        Bijmean = self.getBijsim()
+        B = np.zeros((dmax,dmax))
+        PiPj_mean = self.get_PiPj_sim_IC()
 
         for i, j in itertools.product(range(dmax),range(dmax)):
-            Res[i,j] = Bijmean[i,j] - (phi_sim[i]*phi_sim[j])
+            B[i,j] = PiPj_mean[i,j] - (phi_sim[i]*phi_sim[j])
          
-        invRes = sp.linalg.pinv(Res)
+        invB = sc.linalg.pinv(B)
 
-        erro = np.sum(np.absolute(gij))/np.sum(phi_exp)
-        pear = self.getPearson()
+        self.lambdas_new = np.dot(invB,g)
+        self.lambdas_old = np.genfromtxt(str(self.IClist))
         
-                             
-        with open('error_and_pearsonC_IC','a') as tf:
-            tf.write("Error: %f  Pearson's Correlation: %f\n" % (erro, pear))
+        lambdas_final = self.lambdas_old[:dmax] - damp*self.lambdas_new
+
+        if write_error:
+            self.tolerance = np.sum(np.absolute(g))/np.sum(phi_exp)
+            self.pearson = self.get_Pearson()
+                                            
+            with open('tolerance_and_pearson_IC','a') as tf:
+                tf.write("Tolerance: %f  Pearson's Correlation: %f\n" % (self.tolerance, self.pearson))
         
-        return(np.dot(invRes,gij))
+        return(lambdas_final)
     
-
-    def probCalculation_types(self, state):
+    def prob_calculation_types(self, state):
         R"""
         Calculates the contact probability matrix and the cross term of the Hessian for the type-to-type interactions optimization.
         """    
         PiPj = np.zeros((self.n_types,self.n_types))
         n = int(self.n_types)
         p_instant = np.zeros((n,n))
         
@@ -608,64 +761,63 @@
         for pcount,q in enumerate(itertools.combinations_with_replacement(just.keys(), r=2)):
             p_instant[ind[0][pcount], ind[1][pcount]] = np.average(self.P[np.ix_(just[q[0]], just[q[1]])])
             vec.append(p_instant[ind[0][pcount], ind[1][pcount]])
         vec = np.array(vec)
 
         PiPj = np.outer(vec,vec)
         
-        self.polds_type += p_instant 
-        self.Bij_type += PiPj
+        self.Pold_type += p_instant 
+        self.PiPj_type += PiPj
         self.Nframes += 1  
     
-    def calc_exp_phi_types(self):
+    def calc_phi_exp_types(self):
         R"""
         Calculates the average of the contact probability for each chromatin type (compartment annotation) from the experimental Hi-C for the Types optimization.
         """
         n = int(self.n_types)
         phi = np.zeros((n,n))
         just = {}
         ind = np.triu_indices(n)
         
         for tt in self.header_types:
             just[tt] = ([i for i, e in enumerate(self.ChromSeq) if e == tt])
 
-
         for pcount,q in enumerate(itertools.combinations_with_replacement(just.keys(), r=2)):
             nt=0
             for i, j in itertools.product(just[q[0]],just[q[1]]):
                 phi[ind[0][pcount], ind[1][pcount]] += self.expHiC[i,j]
                 nt += 1
             phi[ind[0][pcount], ind[1][pcount]] = phi[ind[0][pcount], ind[1][pcount]]/nt
 
         return phi
     
     
-    def calc_sim_phi_types(self):
+    def calc_phi_sim_types(self):
         R"""
         Calculates the average of the contact probability for each chromatin type (compartment annotation) from simulation for the Types optimization.
         """
-        return self.polds_type/self.Nframes
+        return self.Pold_type/self.Nframes
     
-    def getPiPjsim_types(self):
+    def get_PiPj_sim_types(self):
         R"""
         Normalizes the cross term of the Hessian by the number of frames in the simulation for the Types optimization.
         """
-        return self.Bij_type/self.Nframes
+        return self.PiPj_type/self.Nframes
     
-    def getHiCSim(self):
+    def get_HiC_sim(self):
         R"""
         Calculates the *in silico* Hi-C map (Full dense matrix).
         """
         return self.Pold/self.Nframes
     
-    def getPearson(self):
+    def get_Pearson(self):
         R"""
         Calculates the Pearson's Correlation between the experimental Hi-C used as a reference for the training and the *in silico* Hi-C obtained from the optimization step.
         """
-        r1 = self.getHiCSim()
+        r1 = self.get_HiC_sim()
         r2 = self.expHiC
 
         r1[np.isinf(r1)]= 0.0
         r1[np.isnan(r1)]= 0.0
         r1[r1 <= 0.001]= 0.0
         r2[np.isinf(r2)]= 0.0
         r2[np.isnan(r2)]= 0.0
@@ -682,55 +834,55 @@
         random.seed(SEED)
         a2 = np.asarray(random.sample(list(r2[np.triu_indices(np.shape(r2)[0])]),int(0.1*np.shape(r2)[0]*np.shape(r2)[0])))
         a2 = r2[np.triu_indices(np.shape(r1)[0])]
 
 
         return(pearsonr(a1,a2)[0])
         
-    def getLamb_types(self, exp_map, damp=5*10**-7):
+    def get_lambdas_types(self, exp_map, damp=5*10**-7, write_error=True):
         R"""
         Calculates the Lagrange multipliers of each type-to-type interaction and returns the matrix containing the energy values for the optimization step.
         """
-        self.getHiCexp(exp_map)
+        self.get_HiC_exp(exp_map)
         
-        phi_exp = self.calc_exp_phi_types()
+        phi_exp = self.calc_phi_exp_types()
         
-        phi_sim = self.calc_sim_phi_types()
+        phi_sim = self.calc_phi_sim_types()
         
-        gij = -phi_sim + phi_exp
+        g = -phi_sim + phi_exp
 
-        PiPj_mean = self.getPiPjsim_types()
+        PiPj_mean = self.get_PiPj_sim_types()
         
-
         ind = np.triu_indices(self.n_types)
         phi_sim_linear = []
 
         for pcount,q in enumerate(itertools.combinations_with_replacement(range(self.n_types), r=2)):
             phi_sim_linear.append(phi_sim[ind[0][pcount], ind[1][pcount]])
            
         phi_sim_linear = np.array(phi_sim_linear)
 
         Pi2_mean = np.outer(phi_sim_linear,phi_sim_linear)
 
-        Bij_mean = PiPj_mean - Pi2_mean
+        B = PiPj_mean - Pi2_mean
     
-        invBij_mean = sp.linalg.pinv(Bij_mean)
+        invB = sc.linalg.pinv(B)
 
-        erro = np.sum(np.absolute(gij))/np.sum(phi_exp)
-        pear = self.getPearson()
-           
-        with open('error_and_pearsonC_types','a') as tf:
-            tf.write("Error: %f  Pearson's Correlation: %f\n" % (erro, pear))
+        if write_error:
+            tolerance = np.sum(np.absolute(g))/np.sum(phi_exp)
+            pearson = self.get_Pearson()
+
+            with open('tolerance_and_pearson_types','a') as tf:
+                    tf.write("Tolerance: %f  Pearson's Correlation: %f\n" % (tolerance, pearson))   
         
-        gij_vec = []
+        g_vec = []
         for pcount,q in enumerate(itertools.combinations_with_replacement(range(self.n_types), r=2)):
-            gij_vec.append(gij[ind[0][pcount], ind[1][pcount]])
-        gij_vec = np.array(gij_vec)
+            g_vec.append(g[ind[0][pcount], ind[1][pcount]])
+        g_vec = np.array(g_vec)
         
-        lambdas = np.matmul(invBij_mean, gij_vec)
+        lambdas = np.matmul(invB, g_vec)
         
         self.lambdas_new = np.zeros((self.n_types,self.n_types))
         
         inds = np.triu_indices_from(self.lambdas_new)
         self.lambdas_new[inds] = lambdas
         self.lambdas_new[(inds[1], inds[0])] = lambdas
```

### Comparing `OpenMiChroM-1.0.6/OpenMiChroM/share/MiChroM.ff` & `OpenMiChroM-1.0.7/OpenMiChroM/share/MiChroM.ff`

 * *Files identical despite different names*

### Comparing `OpenMiChroM-1.0.6/OpenMiChroM.egg-info/PKG-INFO` & `OpenMiChroM-1.0.7/OpenMiChroM.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 Metadata-Version: 2.1
 Name: OpenMiChroM
-Version: 1.0.6
+Version: 1.0.7
 Summary: Open-Michrom lib for chromosome simulations
 Home-page: https://ndb.rice.edu/Open-MiChroM
 Author: Antonio Bento de Oliveira Junior,Vinicius de Godoi Contessoto
 Author-email: antonio.oliveira@rice.edu,contessoto@rice.edu
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Natural Language :: English
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ============
 OpenMiChroM
@@ -121,9 +115,7 @@
 - `Python <https://www.python.org/>`__ (>=3.6)
 - `NumPy <https://www.numpy.org/>`__ (>=1.14)
 - `SciPy <https://www.scipy.org/>`__ (>=1.5.0)
 - `six <https://pypi.org/project/six/>`__ (>=1.14.0)
 - `h5py <https://www.h5py.org/>`__ (>=2.0.0)
 - `pandas <https://pandas.pydata.org/>`__ (>=1.0.0)
 - `scikit-learn <https://scikit-learn.org/>`__ (>=0.20.0)
-
-
```

### Comparing `OpenMiChroM-1.0.6/PKG-INFO` & `OpenMiChroM-1.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 Metadata-Version: 2.1
 Name: OpenMiChroM
-Version: 1.0.6
+Version: 1.0.7
 Summary: Open-Michrom lib for chromosome simulations
 Home-page: https://ndb.rice.edu/Open-MiChroM
 Author: Antonio Bento de Oliveira Junior,Vinicius de Godoi Contessoto
 Author-email: antonio.oliveira@rice.edu,contessoto@rice.edu
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Natural Language :: English
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ============
 OpenMiChroM
@@ -121,9 +115,7 @@
 - `Python <https://www.python.org/>`__ (>=3.6)
 - `NumPy <https://www.numpy.org/>`__ (>=1.14)
 - `SciPy <https://www.scipy.org/>`__ (>=1.5.0)
 - `six <https://pypi.org/project/six/>`__ (>=1.14.0)
 - `h5py <https://www.h5py.org/>`__ (>=2.0.0)
 - `pandas <https://pandas.pydata.org/>`__ (>=1.0.0)
 - `scikit-learn <https://scikit-learn.org/>`__ (>=0.20.0)
-
-
```

### Comparing `OpenMiChroM-1.0.6/README.rst` & `OpenMiChroM-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `OpenMiChroM-1.0.6/tests/tests.py` & `OpenMiChroM-1.0.7/tests/tests.py`

 * *Files identical despite different names*

