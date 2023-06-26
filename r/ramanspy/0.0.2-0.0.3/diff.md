# Comparing `tmp/ramanspy-0.0.2.tar.gz` & `tmp/ramanspy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramanspy-0.0.2.tar", last modified: Mon Jun 26 18:31:16 2023, max compression
+gzip compressed data, was "ramanspy-0.0.3.tar", last modified: Mon Jun 26 22:11:07 2023, max compression
```

## Comparing `ramanspy-0.0.2.tar` & `ramanspy-0.0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 18:31:16.296921 ramanspy-0.0.2/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1503 2023-06-26 11:18:57.000000 ramanspy-0.0.2/LICENSE
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       45 2023-06-26 12:05:50.000000 ramanspy-0.0.2/MANIFEST.in
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3983 2023-06-26 18:31:16.296805 ramanspy-0.0.2/PKG-INFO
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1534 2023-06-26 12:05:35.000000 ramanspy-0.0.2/README.md
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1118 2023-06-26 18:31:05.000000 ramanspy-0.0.2/pyproject.toml
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       38 2023-06-26 18:31:16.296969 ramanspy-0.0.2/setup.cfg
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 18:31:16.291777 ramanspy-0.0.2/src/
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 18:31:16.293201 ramanspy-0.0.2/src/ramanspy/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      471 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/__init__.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 18:31:16.294690 ramanspy-0.0.2/src/ramanspy/analysis/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3187 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/analysis/Step.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       85 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/analysis/__init__.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1035 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/analysis/cluster.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2140 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/analysis/decompose.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     6702 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/analysis/unmix.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    11990 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/core.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    18545 2023-06-26 13:07:02.000000 ramanspy-0.0.2/src/ramanspy/datasets.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    10006 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/load.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4974 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/metrics.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 18:31:16.295218 ramanspy-0.0.2/src/ramanspy/plot/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      196 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/plot/__init__.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     7777 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/plot/_core.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    25767 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/plot/plot.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 18:31:16.296600 ramanspy-0.0.2/src/ramanspy/preprocessing/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     5493 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/preprocessing/Pipeline.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4862 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/preprocessing/Step.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      262 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/preprocessing/__init__.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    16856 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/preprocessing/baseline.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4168 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/preprocessing/denoise.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2370 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/preprocessing/despike.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2138 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/preprocessing/misc.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3573 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/preprocessing/normalise.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3143 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/preprocessing/protocols.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      473 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/utils.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 18:31:16.294008 ramanspy-0.0.2/src/ramanspy.egg-info/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3983 2023-06-26 18:31:16.000000 ramanspy-0.0.2/src/ramanspy.egg-info/PKG-INFO
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      950 2023-06-26 18:31:16.000000 ramanspy-0.0.2/src/ramanspy.egg-info/SOURCES.txt
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        1 2023-06-26 18:31:16.000000 ramanspy-0.0.2/src/ramanspy.egg-info/dependency_links.txt
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       90 2023-06-26 18:31:16.000000 ramanspy-0.0.2/src/ramanspy.egg-info/requires.txt
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        9 2023-06-26 18:31:16.000000 ramanspy-0.0.2/src/ramanspy.egg-info/top_level.txt
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 22:11:07.282372 ramanspy-0.0.3/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1503 2023-06-26 11:18:57.000000 ramanspy-0.0.3/LICENSE
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       45 2023-06-26 12:05:50.000000 ramanspy-0.0.3/MANIFEST.in
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3983 2023-06-26 22:11:07.282273 ramanspy-0.0.3/PKG-INFO
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1534 2023-06-26 12:05:35.000000 ramanspy-0.0.3/README.md
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1118 2023-06-26 22:11:02.000000 ramanspy-0.0.3/pyproject.toml
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       38 2023-06-26 22:11:07.282407 ramanspy-0.0.3/setup.cfg
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 22:11:07.278118 ramanspy-0.0.3/src/
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 22:11:07.279434 ramanspy-0.0.3/src/ramanspy/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      471 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/__init__.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 22:11:07.280666 ramanspy-0.0.3/src/ramanspy/analysis/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3187 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/analysis/Step.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       85 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/analysis/__init__.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1035 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/analysis/cluster.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2140 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/analysis/decompose.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     6702 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/analysis/unmix.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    11990 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/core.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    18545 2023-06-26 13:07:02.000000 ramanspy-0.0.3/src/ramanspy/datasets.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    10385 2023-06-26 22:05:02.000000 ramanspy-0.0.3/src/ramanspy/load.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4974 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/metrics.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 22:11:07.281028 ramanspy-0.0.3/src/ramanspy/plot/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      196 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/plot/__init__.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     7777 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/plot/_core.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    25767 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/plot/plot.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 22:11:07.282117 ramanspy-0.0.3/src/ramanspy/preprocessing/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     5493 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/preprocessing/Pipeline.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4862 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/preprocessing/Step.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      262 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/preprocessing/__init__.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    16856 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/preprocessing/baseline.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4168 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/preprocessing/denoise.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2370 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/preprocessing/despike.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2138 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/preprocessing/misc.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3573 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/preprocessing/normalise.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3143 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/preprocessing/protocols.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      465 2023-06-26 22:05:02.000000 ramanspy-0.0.3/src/ramanspy/utils.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 22:11:07.280110 ramanspy-0.0.3/src/ramanspy.egg-info/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3983 2023-06-26 22:11:07.000000 ramanspy-0.0.3/src/ramanspy.egg-info/PKG-INFO
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      950 2023-06-26 22:11:07.000000 ramanspy-0.0.3/src/ramanspy.egg-info/SOURCES.txt
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        1 2023-06-26 22:11:07.000000 ramanspy-0.0.3/src/ramanspy.egg-info/dependency_links.txt
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       90 2023-06-26 22:11:07.000000 ramanspy-0.0.3/src/ramanspy.egg-info/requires.txt
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        9 2023-06-26 22:11:07.000000 ramanspy-0.0.3/src/ramanspy.egg-info/top_level.txt
```

### Comparing `ramanspy-0.0.2/LICENSE` & `ramanspy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.2/PKG-INFO` & `ramanspy-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramanspy
-Version: 0.0.2
+Version: 0.0.3
 Summary: RamanSPy: An open-source Python package for integrative Raman spectroscopy data analysis
 Author-email: Dimitar Georgiev <d.georgiev21@imperial.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Dimitar Georgiev
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `ramanspy-0.0.2/README.md` & `ramanspy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.2/pyproject.toml` & `ramanspy-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ramanspy"
-version = "0.0.2"
+version = "0.0.3"
 description = "RamanSPy: An open-source Python package for integrative Raman spectroscopy data analysis"
 readme = "README.md"
 authors = [{ name = "Dimitar Georgiev", email = "d.georgiev21@imperial.ac.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
```

### Comparing `ramanspy-0.0.2/src/ramanspy/analysis/Step.py` & `ramanspy-0.0.3/src/ramanspy/analysis/Step.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.2/src/ramanspy/analysis/cluster.py` & `ramanspy-0.0.3/src/ramanspy/analysis/cluster.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.2/src/ramanspy/analysis/decompose.py` & `ramanspy-0.0.3/src/ramanspy/analysis/decompose.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.2/src/ramanspy/analysis/unmix.py` & `ramanspy-0.0.3/src/ramanspy/analysis/unmix.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.2/src/ramanspy/core.py` & `ramanspy-0.0.3/src/ramanspy/core.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.2/src/ramanspy/datasets.py` & `ramanspy-0.0.3/src/ramanspy/datasets.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.2/src/ramanspy/load.py` & `ramanspy-0.0.3/src/ramanspy/load.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import numbers
+
 import numpy as np
 import scipy.io as spio
 from renishawWiRE import WDFReader
 
 from . import core
 from . import utils
 
@@ -46,24 +48,26 @@
         if isinstance(elem, spio.matlab.mio5_params.mat_struct):
             dict[strg] = _todict(elem)
         else:
             dict[strg] = elem
     return dict
 
 
-def witec(filename: str, preprocess: Pipeline = None) -> core.Spectrum or core.SpectralImage:
+def witec(filename: str, *, preprocess: Pipeline = None, laser_excitation: numbers.Number = 532) -> core.Spectrum or core.SpectralImage:
     """
     Loads MATLAB files exported from `WITec's WITec Suite software <https://raman.oxinst.com/products/software/witec-software-suite>`_.
 
     Parameters
     ----------
     filename : str
         The name of the MATLAB file to load. Full path or relative to working directory.
     preprocess : :class:`~ramanspy.preprocessing.Pipeline`, optional
         A preprocessing pipeline to apply to the loaded data. If not specified (default), no preprocessing is applied.
+    laser_excitation : numeric, optional
+        The excitation wavelength of the laser (in nm). Default is 532 nm.
 
     Returns
     ---------
     Union[core.Spectrum, core.SpectralImage] :
         The loaded data.
 
     Example
@@ -89,15 +93,15 @@
     # metadata = matlab_dict
     # metadata["filename"] = file_name
 
     struct_key = next(key for key in matlab_dict.keys() if 'Struct' in key)
     raman_matlab_struct = matlab_dict[struct_key]
 
     axis = raman_matlab_struct['axisscale'][1]
-    shift_values = utils.wavelength_to_wavenumber(axis[0]) if axis[1] != 'rel. 1/cm' else axis[0]
+    shift_values = utils.wavelength_to_wavenumber(axis[0], laser_excitation) if axis[1] != 'rel. 1/cm' else axis[0]
 
     spectral_data = raman_matlab_struct['data']
 
     if len(spectral_data.shape) == 1:  # i.e. single spectrum
         obj = core.Spectrum(spectral_data, shift_values)
 
     elif len(spectral_data.shape) == 2:
@@ -122,24 +126,26 @@
 
     if preprocess is not None:
         obj = preprocess.apply(obj)
 
     return obj
 
 
-def ocean_insight(filename: str, preprocess: Pipeline = None) -> core.Spectrum:
+def ocean_insight(filename: str, *, preprocess: Pipeline = None, laser_excitation: numbers.Number = 532) -> core.Spectrum:
     """
     Loads spectra data from `Ocean Insight's OceanView software <https://www.oceaninsight.com/products/software/>`_ .txt files.
 
     Parameters
     ----------
     filename : str
         The name of the .txt file to load. Full path or relative to working directory.
     preprocess : :class:`~ramanspy.preprocessing.Pipeline`, optional
         A preprocessing pipeline to apply to the loaded data. If not specified (default), no preprocessing is applied.
+    laser_excitation : numeric, optional
+        The excitation wavelength of the laser (in nm). Default is 532 nm.
 
     Returns
     ---------
     core.Spectrum :
         The loaded data.
 
     Example
@@ -173,25 +179,25 @@
 
             data.append(line)
 
     spectral_data = data[:, 1]
     shift_values = data[:, 0]
 
     if metadata["XAxis mode"].lower() == "wavelengths":
-        shift_values = utils.wavelength_to_wavenumber(shift_values)
+        shift_values = utils.wavelength_to_wavenumber(shift_values, laser_excitation)
 
     spectrum = core.Spectrum(spectral_data, shift_values)
 
     if preprocess is not None:
         spectrum = preprocess.apply(spectrum)
 
     return spectrum
 
 
-def renishaw(filename: str, preprocess: Pipeline = None) -> core.SpectralContainer or core.Spectrum or core.SpectralImage:
+def renishaw(filename: str, *, preprocess: Pipeline = None) -> core.SpectralContainer or core.Spectrum or core.SpectralImage:
     """
     Loads spectra data from `Ranishaw's WiRE software <https://www.renishaw.com/en/raman-software--9450>`_ .wdf  files.
 
     Parameters
     ----------
     filename : str
         The name of the .wdf file to load. Full path or relative to working directory.
@@ -227,15 +233,15 @@
 
     if preprocess is not None:
         obj = preprocess.apply(obj)
 
     return obj
 
 
-def opus(filename: str, preprocess: Pipeline = None) -> core.Spectrum:
+def opus(filename: str, *, preprocess: Pipeline = None) -> core.Spectrum:
     """
     Loads spectra data from `Bruker's OPUS software <https://www.bruker.com/en/products-and-solutions/infrared-and-raman/opus-spectroscopy-software.html>`_ files.
 
     Parameters
     ----------
     filename : str
         The name of the file to load. Full path or relative to working directory.
@@ -259,15 +265,15 @@
 
         # Loading a single spectrum
         raman_spectrum = rp.load.opus("path/to/file/ocean_insight_spectrum.O00")
     """
     raise NotImplemented()
 
 
-def labspec(filename: str, preprocess: Pipeline = None) -> core.SpectralContainer or core.Spectrum:
+def labspec(filename: str, *, preprocess: Pipeline = None) -> core.SpectralContainer or core.Spectrum:
     """
     Loads spectra data from `HORIBA's LabSpec software <https://www.horiba.com/int/scientific/products/detail/action/show/Product/labspec-6-spectroscopy-suite-software-1843/>`_ .txt files.
 
     Parameters
     ----------
     filename : str
         The name of the .txt file to load. Full path or relative to working directory.
```

### Comparing `ramanspy-0.0.2/src/ramanspy/metrics.py` & `ramanspy-0.0.3/src/ramanspy/metrics.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.2/src/ramanspy/plot/_core.py` & `ramanspy-0.0.3/src/ramanspy/plot/_core.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.2/src/ramanspy/plot/plot.py` & `ramanspy-0.0.3/src/ramanspy/plot/plot.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.2/src/ramanspy/preprocessing/Pipeline.py` & `ramanspy-0.0.3/src/ramanspy/preprocessing/Pipeline.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.2/src/ramanspy/preprocessing/Step.py` & `ramanspy-0.0.3/src/ramanspy/preprocessing/Step.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.2/src/ramanspy/preprocessing/baseline.py` & `ramanspy-0.0.3/src/ramanspy/preprocessing/baseline.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.2/src/ramanspy/preprocessing/denoise.py` & `ramanspy-0.0.3/src/ramanspy/preprocessing/denoise.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.2/src/ramanspy/preprocessing/despike.py` & `ramanspy-0.0.3/src/ramanspy/preprocessing/despike.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.2/src/ramanspy/preprocessing/misc.py` & `ramanspy-0.0.3/src/ramanspy/preprocessing/misc.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.2/src/ramanspy/preprocessing/normalise.py` & `ramanspy-0.0.3/src/ramanspy/preprocessing/normalise.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.2/src/ramanspy/preprocessing/protocols.py` & `ramanspy-0.0.3/src/ramanspy/preprocessing/protocols.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.2/src/ramanspy.egg-info/PKG-INFO` & `ramanspy-0.0.3/src/ramanspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramanspy
-Version: 0.0.2
+Version: 0.0.3
 Summary: RamanSPy: An open-source Python package for integrative Raman spectroscopy data analysis
 Author-email: Dimitar Georgiev <d.georgiev21@imperial.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Dimitar Georgiev
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `ramanspy-0.0.2/src/ramanspy.egg-info/SOURCES.txt` & `ramanspy-0.0.3/src/ramanspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

