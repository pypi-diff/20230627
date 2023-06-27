# Comparing `tmp/SpecLab-4.0.6.tar.gz` & `tmp/SpecLab-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SpecLab-4.0.6.tar", last modified: Mon Jun 26 18:09:07 2023, max compression
+gzip compressed data, was "dist/SpecLab-4.0.7.tar", last modified: Tue Jun 27 18:07:16 2023, max compression
```

## Comparing `SpecLab-4.0.6.tar` & `SpecLab-4.0.7.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-26 18:09:07.000000 SpecLab-4.0.6/
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-26 18:09:07.000000 SpecLab-4.0.6/SpecLab/
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-26 18:09:07.000000 SpecLab-4.0.6/SpecLab/imXam/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-05-30 23:51:42.000000 SpecLab-4.0.6/SpecLab/imXam/__init__.py
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)    48679 2023-06-26 18:03:14.000000 SpecLab-4.0.6/SpecLab/imXam/imXam.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-26 18:09:07.000000 SpecLab-4.0.6/SpecLab/cfg/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     2025 2023-06-14 20:25:01.000000 SpecLab-4.0.6/SpecLab/cfg/SpecLab_config.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      379 2023-06-15 15:54:47.000000 SpecLab-4.0.6/SpecLab/cfg/epar_imXam.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-26 18:09:07.000000 SpecLab-4.0.6/SpecLab/gen/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    53071 2023-06-14 20:52:49.000000 SpecLab-4.0.6/SpecLab/gen/SpecLabFunctions.py
--rwxr--r--   0 adamkowalski  (1000) adamkowalski  (1000)      656 2023-06-02 18:44:11.000000 SpecLab-4.0.6/SpecLab/gen/globals.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:30.000000 SpecLab-4.0.6/SpecLab/gen/__init__.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    20199 2023-06-14 19:40:28.000000 SpecLab-4.0.6/SpecLab/gen/myfunc.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-01 23:14:48.000000 SpecLab-4.0.6/SpecLab/__init__.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-26 18:09:07.000000 SpecLab-4.0.6/SpecLab/aux/
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-26 18:09:07.000000 SpecLab-4.0.6/SpecLab/aux/param_files/
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2133 2023-06-26 18:07:15.000000 SpecLab-4.0.6/SpecLab/aux/param_files/imXam_param.default.dat
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:07.000000 SpecLab-4.0.6/SpecLab/aux/param_files/__init__.py
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2130 2023-06-26 18:06:59.000000 SpecLab-4.0.6/SpecLab/aux/param_files/imXam_param_ARCES.dat
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2134 2023-06-26 18:06:44.000000 SpecLab-4.0.6/SpecLab/aux/param_files/imXam_param.dat
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:21:46.000000 SpecLab-4.0.6/SpecLab/aux/__init__.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)   625389 2023-05-30 23:11:52.000000 SpecLab-4.0.6/SpecLab/aux/pyqtgraph10_speclab.tar.gz
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-26 18:09:07.000000 SpecLab-4.0.6/SpecLab/doc/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:19.000000 SpecLab-4.0.6/SpecLab/doc/__init__.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      420 2023-06-26 17:45:13.000000 SpecLab-4.0.6/SpecLab/doc/CHANGELOG.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     4403 2023-06-26 18:04:52.000000 SpecLab-4.0.6/SpecLab/doc/README.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1072 2023-06-26 17:41:16.000000 SpecLab-4.0.6/SpecLab/doc/KNOWN_ISSUES.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1119 2023-06-14 15:39:40.000000 SpecLab-4.0.6/SpecLab/doc/LICENSE.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      213 2023-06-26 18:09:07.000000 SpecLab-4.0.6/PKG-INFO
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1161 2023-06-26 18:08:59.000000 SpecLab-4.0.6/setup.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:07:16.000000 SpecLab-4.0.7/
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:07:16.000000 SpecLab-4.0.7/SpecLab/
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:07:16.000000 SpecLab-4.0.7/SpecLab/imXam/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-05-30 23:51:42.000000 SpecLab-4.0.7/SpecLab/imXam/__init__.py
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)    48678 2023-06-27 18:04:41.000000 SpecLab-4.0.7/SpecLab/imXam/imXam.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:07:16.000000 SpecLab-4.0.7/SpecLab/cfg/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     2025 2023-06-14 20:25:01.000000 SpecLab-4.0.7/SpecLab/cfg/SpecLab_config.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      379 2023-06-15 15:54:47.000000 SpecLab-4.0.7/SpecLab/cfg/epar_imXam.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:07:16.000000 SpecLab-4.0.7/SpecLab/gen/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    53071 2023-06-14 20:52:49.000000 SpecLab-4.0.7/SpecLab/gen/SpecLabFunctions.py
+-rwxr--r--   0 adamkowalski  (1000) adamkowalski  (1000)      656 2023-06-02 18:44:11.000000 SpecLab-4.0.7/SpecLab/gen/globals.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:30.000000 SpecLab-4.0.7/SpecLab/gen/__init__.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    20199 2023-06-14 19:40:28.000000 SpecLab-4.0.7/SpecLab/gen/myfunc.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-01 23:14:48.000000 SpecLab-4.0.7/SpecLab/__init__.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:07:16.000000 SpecLab-4.0.7/SpecLab/aux/
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:07:16.000000 SpecLab-4.0.7/SpecLab/aux/param_files/
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2133 2023-06-26 18:07:15.000000 SpecLab-4.0.7/SpecLab/aux/param_files/imXam_param.default.dat
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:07.000000 SpecLab-4.0.7/SpecLab/aux/param_files/__init__.py
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2130 2023-06-26 18:06:59.000000 SpecLab-4.0.7/SpecLab/aux/param_files/imXam_param_ARCES.dat
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2134 2023-06-26 18:06:44.000000 SpecLab-4.0.7/SpecLab/aux/param_files/imXam_param.dat
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:21:46.000000 SpecLab-4.0.7/SpecLab/aux/__init__.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)   625389 2023-05-30 23:11:52.000000 SpecLab-4.0.7/SpecLab/aux/pyqtgraph10_speclab.tar.gz
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-27 18:07:16.000000 SpecLab-4.0.7/SpecLab/doc/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:19.000000 SpecLab-4.0.7/SpecLab/doc/__init__.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      420 2023-06-26 17:45:13.000000 SpecLab-4.0.7/SpecLab/doc/CHANGELOG.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1072 2023-06-26 17:41:16.000000 SpecLab-4.0.7/SpecLab/doc/KNOWN_ISSUES.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1119 2023-06-14 15:39:40.000000 SpecLab-4.0.7/SpecLab/doc/LICENSE.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     6325 2023-06-27 18:07:16.000000 SpecLab-4.0.7/PKG-INFO
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1424 2023-06-27 18:06:04.000000 SpecLab-4.0.7/setup.py
```

### Comparing `SpecLab-4.0.6/SpecLab/imXam/imXam.py` & `SpecLab-4.0.7/SpecLab/imXam/imXam.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     z2_zscale = imclean[midpoint] + (coeffsz[0] / 1.0) * (npoints - midpoint)
     return z1_zscale, z2_zscale
 
 
 
 print('======================================================')
 print('======================================================')
-print('imXam: adam f kowalski, v4.0.6: June 26, 2023')
+print('imXam: adam f kowalski, v4.0.7: June 27, 2023')
 print(' To shut down gui, type q into terminal, type h for interactive commands, use middle mouse wheel to zoom in and out')
 print(' You may have to click on gui with left mouse button in order to use interactive commands')
 print(' To get a list of command-line options, type imXam.py -h from a terminal.')
 print('======================================================')
 print('imXam.py located in ',your_site_packages_location[0]+'/SpecLab/imXam/')
 print(' and .../anaconda3/envs/<your_env_name>/bin/')
 print('Default param files located in ',your_site_packages_location[0]+'/SpecLab/aux/param_files/')
@@ -947,15 +947,15 @@
         except:
             print('Could not print header.')
     if val == 'q':
         QCoreApplication.exit()
     if val == 'h' or val == '?' or  val == 'help' or val == 'Help':
         print('           ')
         print('************************************************************')
-        print('q:  quit imexam.')
+        print('q:  quit imXam.')
         print('r:  plot radial profile, print fwhm, and print aperture photometry w/ sky annulus subtraction centered at cursor location; plot x-range can be set with RMax.')
         print('x:  trace and extract spectrum with sky subtraction, at cursor location (can change params in imXam_param.dat).')
         print('g:  fits a Gaussian to the spatial profile (uniform weighting in fit) of a spectrum at cursor location. An estimate of a constant background level (e.g., bias in a raw frame) is subtracted before the fit')
         print('T:  show (e.g., saturated) pixels above some threshold.  Prompts for a threshold (ENTER an INTEGER, not e.g., 1.5e4) above which to color red.')
         print('a:  print fwhm and apperture photometry w/ sky annulus subtraction centered at cursor location.')
         print('o:  plot contours at cursor location (not centroided) and shows in +/- Window.')
         print('z:  zoom in on cursor location (can change scaling with Zmax and Zmin and color table with Color).  Overplots the aperture photometry annuli.')
```

### Comparing `SpecLab-4.0.6/SpecLab/cfg/SpecLab_config.py` & `SpecLab-4.0.7/SpecLab/cfg/SpecLab_config.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.6/SpecLab/gen/SpecLabFunctions.py` & `SpecLab-4.0.7/SpecLab/gen/SpecLabFunctions.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.6/SpecLab/gen/globals.py` & `SpecLab-4.0.7/SpecLab/gen/globals.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.6/SpecLab/gen/myfunc.py` & `SpecLab-4.0.7/SpecLab/gen/myfunc.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.6/SpecLab/aux/param_files/imXam_param.default.dat` & `SpecLab-4.0.7/SpecLab/aux/param_files/imXam_param.default.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.6/SpecLab/aux/param_files/imXam_param_ARCES.dat` & `SpecLab-4.0.7/SpecLab/aux/param_files/imXam_param_ARCES.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.6/SpecLab/aux/param_files/imXam_param.dat` & `SpecLab-4.0.7/SpecLab/aux/param_files/imXam_param.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.6/SpecLab/aux/pyqtgraph10_speclab.tar.gz` & `SpecLab-4.0.7/SpecLab/aux/pyqtgraph10_speclab.tar.gz`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.6/SpecLab/doc/KNOWN_ISSUES.txt` & `SpecLab-4.0.7/SpecLab/doc/KNOWN_ISSUES.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.6/SpecLab/doc/LICENSE.txt` & `SpecLab-4.0.7/SpecLab/doc/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.6/setup.py` & `SpecLab-4.0.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 from distutils.core import setup
 
+try:
+   import pypandoc
+   long_desc = pypandoc.convert_file('README.md', 'rst')
+except(IOError, ImportError):
+   long_desc = open('README.md').read()
+
+
+#this_directory = Path(__file__).parent
+#long_desc = (this_directory / "README").read_text()
+
 setup(
     name='SpecLab',
-    version='4.0.6',
+    version='4.0.7',
     author='A. F. Kowalski',
     author_email='adam.f.kowalski@colorado.edu',
     packages=['SpecLab','SpecLab.aux','SpecLab.aux.param_files','SpecLab.imXam','SpecLab.doc','SpecLab.gen',],
     package_data = {'':['*.tar.gz', '*.txt', '*.dat'],},
    # include_package_data=True,
    # package_dir={"": ""},
     scripts=['SpecLab/cfg/SpecLab_config.py','SpecLab/imXam/imXam.py','SpecLab/cfg/epar_imXam.py',],
     #url='http://pypi.python.org/pypi/TowelStuff/',
-    license='LICENSE.txt',
-    #description='Imaxam GUI for Python.',
-    #long_description=open('README.txt').read(),
-    install_requires=['numpy', 'plotly>=5.2.1', 'pandas','astropy>=4.0.2','scipy','matplotlib','PyQt5>=5.15.6', 'photutils',],
+    description='IRAF imexam+DS9 replacement for Python',long_description_content_type='text/markdown',
+    long_description=long_desc,
+    install_requires=['numpy', 'plotly>=5.2.1', 'pandas','astropy>=4.0.2','scipy','matplotlib','PyQt5>=5.15.6', 'photutils',]
 )
 
 # python setup.py sdist
 # python -m twine upload --repository testpypi dist/*
 # pip install -i https://test.pypi.org/simple/ speclab-imXam==3.1.2
 # pip uninstall speclab-imXam==3.1.2
 #  I neeeded to put the #! crap at the top of any of the scripts=
```

