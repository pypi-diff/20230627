# Comparing `tmp/voltage_imaging_analysis-0.1.8.tar.gz` & `tmp/voltage_imaging_analysis-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voltage_imaging_analysis-0.1.8.tar", last modified: Tue Jun 27 13:04:32 2023, max compression
+gzip compressed data, was "voltage_imaging_analysis-0.1.9.tar", last modified: Tue Jun 27 13:07:51 2023, max compression
```

## Comparing `voltage_imaging_analysis-0.1.8.tar` & `voltage_imaging_analysis-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 rrsims    (1000) rrsims    (1000)        0 2023-06-27 13:04:32.979092 voltage_imaging_analysis-0.1.8/
--rw-r--r--   0 rrsims    (1000) rrsims    (1000)     6148 2023-06-17 17:31:33.000000 voltage_imaging_analysis-0.1.8/.DS_Store
--rw-rw-r--   0 rrsims    (1000) rrsims    (1000)      470 2023-06-27 13:04:32.979092 voltage_imaging_analysis-0.1.8/PKG-INFO
--rw-r--r--   0 rrsims    (1000) rrsims    (1000)      101 2023-06-17 17:31:33.000000 voltage_imaging_analysis-0.1.8/README.md
-drwxrwxr-x   0 rrsims    (1000) rrsims    (1000)        0 2023-06-27 13:04:32.979092 voltage_imaging_analysis-0.1.8/dist/
--rw-r--r--   0 rrsims    (1000) rrsims    (1000)     9000 2023-06-17 17:31:33.000000 voltage_imaging_analysis-0.1.8/dist/voltage_imaging_analysis-0.1.0.tar.gz
--rw-r--r--   0 rrsims    (1000) rrsims    (1000)    23089 2023-06-17 17:31:33.000000 voltage_imaging_analysis-0.1.8/dist/voltage_imaging_analysis-0.1.5.tar.gz
--rw-r--r--   0 rrsims    (1000) rrsims    (1000)    44357 2023-06-17 17:31:33.000000 voltage_imaging_analysis-0.1.8/dist/voltage_imaging_analysis-0.1.6.tar.gz
--rw-rw-r--   0 rrsims    (1000) rrsims    (1000)       38 2023-06-27 13:04:32.979092 voltage_imaging_analysis-0.1.8/setup.cfg
--rw-r--r--   0 rrsims    (1000) rrsims    (1000)      697 2023-06-27 13:04:17.000000 voltage_imaging_analysis-0.1.8/setup.py
-drwxrwxr-x   0 rrsims    (1000) rrsims    (1000)        0 2023-06-27 13:04:32.979092 voltage_imaging_analysis-0.1.8/voltage_imaging_analysis/
--rw-r--r--   0 rrsims    (1000) rrsims    (1000)      125 2023-06-17 17:31:33.000000 voltage_imaging_analysis-0.1.8/voltage_imaging_analysis/__init__.py
-drwxrwxr-x   0 rrsims    (1000) rrsims    (1000)        0 2023-06-27 13:04:32.979092 voltage_imaging_analysis-0.1.8/voltage_imaging_analysis/__pycache__/
--rw-r--r--   0 rrsims    (1000) rrsims    (1000)      321 2023-06-17 17:31:33.000000 voltage_imaging_analysis-0.1.8/voltage_imaging_analysis/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rrsims    (1000) rrsims    (1000)     6150 2023-06-23 18:33:48.000000 voltage_imaging_analysis-0.1.8/voltage_imaging_analysis/test_1p_analysis.py
--rw-r--r--   0 rrsims    (1000) rrsims    (1000)    29799 2023-06-27 13:02:01.000000 voltage_imaging_analysis-0.1.8/voltage_imaging_analysis/voltage_imaging_analysis_fcts.py
-drwxrwxr-x   0 rrsims    (1000) rrsims    (1000)        0 2023-06-27 13:04:32.979092 voltage_imaging_analysis-0.1.8/voltage_imaging_analysis.egg-info/
--rw-r--r--   0 rrsims    (1000) rrsims    (1000)      470 2023-06-27 13:04:32.000000 voltage_imaging_analysis-0.1.8/voltage_imaging_analysis.egg-info/PKG-INFO
--rw-r--r--   0 rrsims    (1000) rrsims    (1000)      597 2023-06-27 13:04:32.000000 voltage_imaging_analysis-0.1.8/voltage_imaging_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 rrsims    (1000) rrsims    (1000)        1 2023-06-27 13:04:32.000000 voltage_imaging_analysis-0.1.8/voltage_imaging_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 rrsims    (1000) rrsims    (1000)        6 2023-06-27 13:04:32.000000 voltage_imaging_analysis-0.1.8/voltage_imaging_analysis.egg-info/requires.txt
--rw-r--r--   0 rrsims    (1000) rrsims    (1000)       25 2023-06-27 13:04:32.000000 voltage_imaging_analysis-0.1.8/voltage_imaging_analysis.egg-info/top_level.txt
+drwxrwxr-x   0 rrsims    (1000) rrsims    (1000)        0 2023-06-27 13:07:51.494606 voltage_imaging_analysis-0.1.9/
+-rw-r--r--   0 rrsims    (1000) rrsims    (1000)     6148 2023-06-17 17:31:33.000000 voltage_imaging_analysis-0.1.9/.DS_Store
+-rw-rw-r--   0 rrsims    (1000) rrsims    (1000)      470 2023-06-27 13:07:51.494606 voltage_imaging_analysis-0.1.9/PKG-INFO
+-rw-r--r--   0 rrsims    (1000) rrsims    (1000)      101 2023-06-17 17:31:33.000000 voltage_imaging_analysis-0.1.9/README.md
+drwxrwxr-x   0 rrsims    (1000) rrsims    (1000)        0 2023-06-27 13:07:51.494606 voltage_imaging_analysis-0.1.9/dist/
+-rw-r--r--   0 rrsims    (1000) rrsims    (1000)     9000 2023-06-17 17:31:33.000000 voltage_imaging_analysis-0.1.9/dist/voltage_imaging_analysis-0.1.0.tar.gz
+-rw-r--r--   0 rrsims    (1000) rrsims    (1000)    23089 2023-06-17 17:31:33.000000 voltage_imaging_analysis-0.1.9/dist/voltage_imaging_analysis-0.1.5.tar.gz
+-rw-r--r--   0 rrsims    (1000) rrsims    (1000)    44357 2023-06-17 17:31:33.000000 voltage_imaging_analysis-0.1.9/dist/voltage_imaging_analysis-0.1.6.tar.gz
+-rw-rw-r--   0 rrsims    (1000) rrsims    (1000)       38 2023-06-27 13:07:51.494606 voltage_imaging_analysis-0.1.9/setup.cfg
+-rw-r--r--   0 rrsims    (1000) rrsims    (1000)      697 2023-06-27 13:07:35.000000 voltage_imaging_analysis-0.1.9/setup.py
+drwxrwxr-x   0 rrsims    (1000) rrsims    (1000)        0 2023-06-27 13:07:51.494606 voltage_imaging_analysis-0.1.9/voltage_imaging_analysis/
+-rw-r--r--   0 rrsims    (1000) rrsims    (1000)      125 2023-06-17 17:31:33.000000 voltage_imaging_analysis-0.1.9/voltage_imaging_analysis/__init__.py
+drwxrwxr-x   0 rrsims    (1000) rrsims    (1000)        0 2023-06-27 13:07:51.494606 voltage_imaging_analysis-0.1.9/voltage_imaging_analysis/__pycache__/
+-rw-r--r--   0 rrsims    (1000) rrsims    (1000)      321 2023-06-17 17:31:33.000000 voltage_imaging_analysis-0.1.9/voltage_imaging_analysis/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rrsims    (1000) rrsims    (1000)     6150 2023-06-23 18:33:48.000000 voltage_imaging_analysis-0.1.9/voltage_imaging_analysis/test_1p_analysis.py
+-rw-r--r--   0 rrsims    (1000) rrsims    (1000)    29813 2023-06-27 13:06:54.000000 voltage_imaging_analysis-0.1.9/voltage_imaging_analysis/voltage_imaging_analysis_fcts.py
+drwxrwxr-x   0 rrsims    (1000) rrsims    (1000)        0 2023-06-27 13:07:51.494606 voltage_imaging_analysis-0.1.9/voltage_imaging_analysis.egg-info/
+-rw-r--r--   0 rrsims    (1000) rrsims    (1000)      470 2023-06-27 13:07:51.000000 voltage_imaging_analysis-0.1.9/voltage_imaging_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 rrsims    (1000) rrsims    (1000)      597 2023-06-27 13:07:51.000000 voltage_imaging_analysis-0.1.9/voltage_imaging_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 rrsims    (1000) rrsims    (1000)        1 2023-06-27 13:07:51.000000 voltage_imaging_analysis-0.1.9/voltage_imaging_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 rrsims    (1000) rrsims    (1000)        6 2023-06-27 13:07:51.000000 voltage_imaging_analysis-0.1.9/voltage_imaging_analysis.egg-info/requires.txt
+-rw-r--r--   0 rrsims    (1000) rrsims    (1000)       25 2023-06-27 13:07:51.000000 voltage_imaging_analysis-0.1.9/voltage_imaging_analysis.egg-info/top_level.txt
```

### Comparing `voltage_imaging_analysis-0.1.8/.DS_Store` & `voltage_imaging_analysis-0.1.9/.DS_Store`

 * *Files identical despite different names*

### Comparing `voltage_imaging_analysis-0.1.8/dist/voltage_imaging_analysis-0.1.0.tar.gz` & `voltage_imaging_analysis-0.1.9/dist/voltage_imaging_analysis-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `voltage_imaging_analysis-0.1.8/dist/voltage_imaging_analysis-0.1.5.tar.gz` & `voltage_imaging_analysis-0.1.9/dist/voltage_imaging_analysis-0.1.5.tar.gz`

 * *Files identical despite different names*

### Comparing `voltage_imaging_analysis-0.1.8/dist/voltage_imaging_analysis-0.1.6.tar.gz` & `voltage_imaging_analysis-0.1.9/dist/voltage_imaging_analysis-0.1.6.tar.gz`

 * *Files identical despite different names*

### Comparing `voltage_imaging_analysis-0.1.8/setup.py` & `voltage_imaging_analysis-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='voltage_imaging_analysis',
-    version='0.1.8',    
+    version='0.1.9',    
     description='Python package used for analysing voltage imaging data.',
     url='https://github.com/rrsims21/voltage_imaging_analysis/',
     author='Ruth Sims',
     author_email='ruth.sims@inserm.fr',
     license='BSD 2-clause',
     packages=['voltage_imaging_analysis'],
     install_requires=[
```

### Comparing `voltage_imaging_analysis-0.1.8/voltage_imaging_analysis/test_1p_analysis.py` & `voltage_imaging_analysis-0.1.9/voltage_imaging_analysis/test_1p_analysis.py`

 * *Files identical despite different names*

### Comparing `voltage_imaging_analysis-0.1.8/voltage_imaging_analysis/voltage_imaging_analysis_fcts.py` & `voltage_imaging_analysis-0.1.9/voltage_imaging_analysis/voltage_imaging_analysis_fcts.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,15 +440,15 @@
     # argsort_prominances = np.argsort(prominences)[::-1]
     # spike_idxs_for_template = peak_idxs[argsort_prominances]
     if min_distance is None:
         peak_idxs, _ = scipy.signal.find_peaks(timeseries, rel_height=0.5)
     else:
         peak_idxs, _ = scipy.signal.find_peaks(timeseries, rel_height=0.5, distance=min_distance)
 
-    spike_idxs_for_template = peak_idxs[timeseries[peak_idxs] > *min_prominencenp.max(timeseries[peak_idxs])]
+    spike_idxs_for_template = peak_idxs[timeseries[peak_idxs] > min_prominence*min_prominencenp.max(timeseries[peak_idxs])]
     prominences = scipy.signal.peak_prominences(timeseries, peak_idxs)[0]
 
     # estimate peak width
     spike_width = np.ceil(np.nanmean(scipy.signal.peak_widths(timeseries, spike_idxs_for_template, rel_height=0.85)[0])).astype(int)
     half_spike_width = np.ceil(np.divide(spike_width - 1, 2)).astype(int) + 3
 
     # crop peaks (make sure that array large enough)
```

### Comparing `voltage_imaging_analysis-0.1.8/voltage_imaging_analysis.egg-info/SOURCES.txt` & `voltage_imaging_analysis-0.1.9/voltage_imaging_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

