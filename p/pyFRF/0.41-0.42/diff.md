# Comparing `tmp/pyFRF-0.41.tar.gz` & `tmp/pyFRF-0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyFRF-0.41.tar", last modified: Tue Jun 27 09:57:30 2023, max compression
+gzip compressed data, was "pyFRF-0.42.tar", last modified: Tue Jun 27 10:24:48 2023, max compression
```

## Comparing `pyFRF-0.41.tar` & `pyFRF-0.42.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 09:57:30.218121 pyFRF-0.41/
--rw-rw-rw-   0        0        0      753 2020-06-16 07:16:38.000000 pyFRF-0.41/LICENSE
--rw-rw-rw-   0        0        0      593 2023-06-27 09:57:30.218121 pyFRF-0.41/PKG-INFO
--rw-rw-rw-   0        0        0     8982 2020-06-16 07:16:38.000000 pyFRF-0.41/fft_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:57:30.216952 pyFRF-0.41/pyFRF.egg-info/
--rw-rw-rw-   0        0        0      593 2023-06-27 09:57:30.000000 pyFRF-0.41/pyFRF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-27 09:57:30.000000 pyFRF-0.41/pyFRF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 09:57:30.000000 pyFRF-0.41/pyFRF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-27 09:57:30.000000 pyFRF-0.41/pyFRF.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-27 09:57:30.000000 pyFRF-0.41/pyFRF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    24390 2023-06-27 09:55:12.000000 pyFRF-0.41/pyFRF.py
--rw-rw-rw-   0        0        0       42 2023-06-27 09:57:30.218121 pyFRF-0.41/setup.cfg
--rw-rw-rw-   0        0        0     1568 2020-06-16 07:16:38.000000 pyFRF-0.41/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:24:48.032498 pyFRF-0.42/
+-rw-rw-rw-   0        0        0      753 2020-06-16 07:16:38.000000 pyFRF-0.42/LICENSE
+-rw-rw-rw-   0        0        0      593 2023-06-27 10:24:47.996628 pyFRF-0.42/PKG-INFO
+-rw-rw-rw-   0        0        0     8982 2020-06-16 07:16:38.000000 pyFRF-0.42/fft_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-27 10:24:47.995629 pyFRF-0.42/pyFRF.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-06-27 10:24:47.000000 pyFRF-0.42/pyFRF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-27 10:24:47.000000 pyFRF-0.42/pyFRF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 10:24:47.000000 pyFRF-0.42/pyFRF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-27 10:24:47.000000 pyFRF-0.42/pyFRF.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-27 10:24:47.000000 pyFRF-0.42/pyFRF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    24393 2023-06-27 10:24:29.000000 pyFRF-0.42/pyFRF.py
+-rw-rw-rw-   0        0        0       42 2023-06-27 10:24:48.032498 pyFRF-0.42/setup.cfg
+-rw-rw-rw-   0        0        0     1568 2023-06-27 10:24:39.000000 pyFRF-0.42/setup.py
```

### Comparing `pyFRF-0.41/LICENSE` & `pyFRF-0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `pyFRF-0.41/PKG-INFO` & `pyFRF-0.42/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyFRF
-Version: 0.41
+Version: 0.42
 Summary: Frequency response function as used in structural dynamics.
 Home-page: https://github.com/openmodal/pyFRF
 Author: Janko Slavič et al.
 Author-email: janko.slavic@fs.uni-lj.si
 License: UNKNOWN
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `pyFRF-0.41/fft_tools.py` & `pyFRF-0.42/fft_tools.py`

 * *Files identical despite different names*

### Comparing `pyFRF-0.41/pyFRF.egg-info/PKG-INFO` & `pyFRF-0.42/pyFRF.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyFRF
-Version: 0.41
+Version: 0.42
 Summary: Frequency response function as used in structural dynamics.
 Home-page: https://github.com/openmodal/pyFRF
 Author: Janko Slavič et al.
 Author-email: janko.slavic@fs.uni-lj.si
 License: UNKNOWN
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `pyFRF-0.41/pyFRF.py` & `pyFRF-0.42/pyFRF.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     class FRF:      Handles 2 channel frequency response function.
 
 """
 
 import numpy as np
 import fft_tools
 
-__version__ = '0.41'
+__version__ = '0.42'
 _EXC_TYPES = ['f', 'a', 'v', 'd', 'e']  # force for EMA and kinematics for OMA
 _RESP_TYPES = ['a', 'v', 'd', 'e']  # acceleration, velocity, displacement, strain
 _FRF_TYPES = ['H1', 'H2', 'Hv', 'vector', 'ODS']
 _FRF_FORM = ['accelerance', 'mobility', 'receptance']
 _WGH_TYPES = ['None', 'Linear', 'Exponential']
 _WINDOWS = ['None', 'Hann', 'Hamming', 'Force', 'Exponential', 'Bartlett', 'Blackman', 'Kaiser']
 
@@ -340,15 +340,15 @@
             w = np.blackman(self.samples)
         elif window[0] in ['Kaiser']:
             beta = float(window[1])
             w = np.kaiser(self.samples, beta)
         elif window[0] == 'Force':
             w = np.zeros(self.samples)
             force_window = float(window[1])
-            to1 = np.long(force_window * self.samples)
+            to1 = np.float64(force_window * self.samples)
             w[:to1] = 1.
         elif window[0] == 'Exponential':
             w = np.arange(self.samples)
             exponential_window = float(window[1])
             w = np.exp(np.log(exponential_window) * w / (self.samples - 1))
         else:  # window = 'None'
             w = np.ones(self.samples)
```

### Comparing `pyFRF-0.41/setup.py` & `pyFRF-0.42/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 For a showcase see: https://github.com/openmodal/pyFRF/blob/master/Showcase%20pyFRF.ipynb
 """
 
 #from distutils.core import setup, Extension
 from setuptools import setup
 setup(name='pyFRF',
-      version='0.41',
+      version='0.42',
       author='Janko Slavič et al.',
       author_email='janko.slavic@fs.uni-lj.si',
       description='Frequency response function as used in structural dynamics.',
       url='https://github.com/openmodal/pyFRF',
       py_modules=['pyFRF','fft_tools'],
       #ext_modules=[Extension('lvm_read', ['data/short.lvm'])],
       long_description=desc,
```

