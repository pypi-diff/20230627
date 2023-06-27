# Comparing `tmp/pyFRF-0.40.tar.gz` & `tmp/pyFRF-0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyFRF-0.40.tar", last modified: Tue Apr 23 05:27:46 2019, max compression
+gzip compressed data, was "pyFRF-0.41.tar", last modified: Tue Jun 27 09:57:30 2023, max compression
```

## Comparing `pyFRF-0.40.tar` & `pyFRF-0.41.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2019-04-23 05:27:46.000000 pyFRF-0.40/
--rw-rw-rw-   0        0        0      643 2019-04-23 05:27:46.000000 pyFRF-0.40/PKG-INFO
--rw-rw-rw-   0        0        0      493 2017-03-02 06:25:54.000000 pyFRF-0.40/README.rst
--rw-rw-rw-   0        0        0     8982 2019-04-18 13:09:30.000000 pyFRF-0.40/fft_tools.py
-drwxrwxrwx   0        0        0        0 2019-04-23 05:27:46.000000 pyFRF-0.40/pyFRF.egg-info/
--rw-rw-rw-   0        0        0      643 2019-04-23 05:27:44.000000 pyFRF-0.40/pyFRF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2019-04-23 05:27:44.000000 pyFRF-0.40/pyFRF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-04-23 05:27:44.000000 pyFRF-0.40/pyFRF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2019-04-23 05:27:44.000000 pyFRF-0.40/pyFRF.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2019-04-23 05:27:44.000000 pyFRF-0.40/pyFRF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    24393 2019-04-23 05:25:21.000000 pyFRF-0.40/pyFRF.py
--rw-rw-rw-   0        0        0       42 2019-04-23 05:27:46.000000 pyFRF-0.40/setup.cfg
--rw-rw-rw-   0        0        0     1568 2019-04-23 05:25:28.000000 pyFRF-0.40/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:57:30.218121 pyFRF-0.41/
+-rw-rw-rw-   0        0        0      753 2020-06-16 07:16:38.000000 pyFRF-0.41/LICENSE
+-rw-rw-rw-   0        0        0      593 2023-06-27 09:57:30.218121 pyFRF-0.41/PKG-INFO
+-rw-rw-rw-   0        0        0     8982 2020-06-16 07:16:38.000000 pyFRF-0.41/fft_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-27 09:57:30.216952 pyFRF-0.41/pyFRF.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-06-27 09:57:30.000000 pyFRF-0.41/pyFRF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-27 09:57:30.000000 pyFRF-0.41/pyFRF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 09:57:30.000000 pyFRF-0.41/pyFRF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-27 09:57:30.000000 pyFRF-0.41/pyFRF.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-27 09:57:30.000000 pyFRF-0.41/pyFRF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    24390 2023-06-27 09:55:12.000000 pyFRF-0.41/pyFRF.py
+-rw-rw-rw-   0        0        0       42 2023-06-27 09:57:30.218121 pyFRF-0.41/setup.cfg
+-rw-rw-rw-   0        0        0     1568 2020-06-16 07:16:38.000000 pyFRF-0.41/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyFRF-0.40/fft_tools.py` & `pyFRF-0.41/fft_tools.py`

 * *Files identical despite different names*

### Comparing `pyFRF-0.40/pyFRF.py` & `pyFRF-0.41/pyFRF.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     class FRF:      Handles 2 channel frequency response function.
 
 """
 
 import numpy as np
 import fft_tools
 
-__version__ = '0.40'
+__version__ = '0.41'
 _EXC_TYPES = ['f', 'a', 'v', 'd', 'e']  # force for EMA and kinematics for OMA
 _RESP_TYPES = ['a', 'v', 'd', 'e']  # acceleration, velocity, displacement, strain
 _FRF_TYPES = ['H1', 'H2', 'Hv', 'vector', 'ODS']
 _FRF_FORM = ['accelerance', 'mobility', 'receptance']
 _WGH_TYPES = ['None', 'Linear', 'Exponential']
 _WINDOWS = ['None', 'Hann', 'Hamming', 'Force', 'Exponential', 'Bartlett', 'Blackman', 'Kaiser']
 
@@ -166,15 +166,15 @@
             raise Exception('wrong excitation window type given %s (can be %s)'
                             % (self.exc_window, _WINDOWS))
 
         if not (self.resp_window.split(':')[0] in _WINDOWS):
             raise Exception('wrong response window type given %s (can be %s)'
                             % (self.resp_window, _WINDOWS))
 
-        self.curr_meas = np.int(0)
+        self.curr_meas = int(0)
 
         if exc is not None and resp is not None:
             self.add_data(exc, resp)
 
     def add_data_for_overlapping(self, exc, resp):
         """Adds data and prepares FRF with the overlapping options
 
@@ -373,15 +373,15 @@
                 self.fft_len = int(self.samples)
             self.w_axis = 2 * np.pi * np.fft.rfftfreq(self.fft_len, 1. / self.sampling_freq)
 
         self.Exc = np.fft.rfft(self.exc, self.fft_len)
         self.Resp = np.fft.rfft(self.resp, self.fft_len)
 
         if self.resp_type != 'e':  # if not strain
-            # convert H1 to receptance
+            # response to displacement
             self.Resp = fft_tools.convert_frf(self.Resp, self.w_axis, input_frf_type=self.resp_type,
                                               output_frf_type='d')
 
             # correct delay
         if self.resp_delay != 0.:
             self.Resp = fft_tools.correct_time_delay(self.Resp, self.w_axis, -self.resp_delay)
```

### Comparing `pyFRF-0.40/setup.py` & `pyFRF-0.41/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 For a showcase see: https://github.com/openmodal/pyFRF/blob/master/Showcase%20pyFRF.ipynb
 """
 
 #from distutils.core import setup, Extension
 from setuptools import setup
 setup(name='pyFRF',
-      version='0.40',
+      version='0.41',
       author='Janko Slavič et al.',
       author_email='janko.slavic@fs.uni-lj.si',
       description='Frequency response function as used in structural dynamics.',
       url='https://github.com/openmodal/pyFRF',
       py_modules=['pyFRF','fft_tools'],
       #ext_modules=[Extension('lvm_read', ['data/short.lvm'])],
       long_description=desc,
```

