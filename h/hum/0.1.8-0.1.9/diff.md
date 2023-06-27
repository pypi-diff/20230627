# Comparing `tmp/hum-0.1.8.tar.gz` & `tmp/hum-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hum-0.1.8.tar", last modified: Thu Jun 24 16:35:20 2021, max compression
+gzip compressed data, was "hum-0.1.9.tar", last modified: Fri Aug  6 17:41:48 2021, max compression
```

## Comparing `hum-0.1.8.tar` & `hum-0.1.9.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 16:35:20.919019 hum-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-06-24 16:34:28.000000 hum-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15620 2021-06-24 16:35:20.919019 hum-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10868 2021-06-24 16:34:28.000000 hum-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 16:35:20.915019 hum-0.1.8/hum/
--rw-r--r--   0 runner    (1001) docker     (121)      297 2021-06-24 16:34:28.000000 hum-0.1.8/hum/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 16:35:20.919019 hum-0.1.8/hum/gen/
--rw-r--r--   0 runner    (1001) docker     (121)      925 2021-06-24 16:34:28.000000 hum-0.1.8/hum/gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14620 2021-06-24 16:35:19.000000 hum-0.1.8/hum/gen/diagnosis_sounds.py
--rw-r--r--   0 runner    (1001) docker     (121)     4705 2021-06-24 16:34:28.000000 hum-0.1.8/hum/gen/signal_generators.py
--rw-r--r--   0 runner    (1001) docker     (121)     2036 2021-06-24 16:34:28.000000 hum-0.1.8/hum/gen/sine_mix.py
--rw-r--r--   0 runner    (1001) docker     (121)     4474 2021-06-24 16:34:28.000000 hum-0.1.8/hum/gen/voiced_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     6000 2021-06-24 16:35:19.000000 hum-0.1.8/hum/lite_sample_sounds.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 16:35:20.919019 hum-0.1.8/hum/sound/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-06-24 16:34:28.000000 hum-0.1.8/hum/sound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8811 2021-06-24 16:34:28.000000 hum-0.1.8/hum/sound/audio.py
--rw-r--r--   0 runner    (1001) docker     (121)     9151 2021-06-24 16:34:28.000000 hum-0.1.8/hum/sound/audio_librosa.py
--rw-r--r--   0 runner    (1001) docker     (121)      988 2021-06-24 16:34:28.000000 hum-0.1.8/hum/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 16:35:20.919019 hum-0.1.8/hum/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2021-06-24 16:34:28.000000 hum-0.1.8/hum/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3767 2021-06-24 16:34:28.000000 hum-0.1.8/hum/utils/date_ticks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2021-06-24 16:35:19.000000 hum-0.1.8/hum/utils/infinite_waveform.py
--rw-r--r--   0 runner    (1001) docker     (121)    38645 2021-06-24 16:34:28.000000 hum-0.1.8/hum/utils/librosa_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1791 2021-06-24 16:34:28.000000 hum-0.1.8/hum/utils/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 16:35:20.915019 hum-0.1.8/hum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15620 2021-06-24 16:35:20.000000 hum-0.1.8/hum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      564 2021-06-24 16:35:20.000000 hum-0.1.8/hum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-24 16:35:20.000000 hum-0.1.8/hum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-24 16:35:20.000000 hum-0.1.8/hum.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-06-24 16:35:20.000000 hum-0.1.8/hum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-06-24 16:35:20.000000 hum-0.1.8/hum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      566 2021-06-24 16:35:20.919019 hum-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      372 2021-06-24 16:34:28.000000 hum-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-06 17:41:48.090784 hum-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-08-06 17:40:46.000000 hum-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    15620 2021-08-06 17:41:48.090784 hum-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10868 2021-08-06 17:40:46.000000 hum-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-06 17:41:48.090784 hum-0.1.9/hum/
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2021-08-06 17:40:46.000000 hum-0.1.9/hum/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-06 17:41:48.090784 hum-0.1.9/hum/gen/
+-rw-r--r--   0 runner    (1001) docker     (121)      925 2021-08-06 17:40:46.000000 hum-0.1.9/hum/gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14620 2021-08-06 17:40:46.000000 hum-0.1.9/hum/gen/diagnosis_sounds.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4705 2021-08-06 17:40:46.000000 hum-0.1.9/hum/gen/signal_generators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2036 2021-08-06 17:40:46.000000 hum-0.1.9/hum/gen/sine_mix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4474 2021-08-06 17:40:46.000000 hum-0.1.9/hum/gen/voiced_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6000 2021-08-06 17:40:46.000000 hum-0.1.9/hum/lite_sample_sounds.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-06 17:41:48.090784 hum-0.1.9/hum/scrap/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-06 17:40:46.000000 hum-0.1.9/hum/scrap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-06 17:41:48.090784 hum-0.1.9/hum/sound/
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2021-08-06 17:40:46.000000 hum-0.1.9/hum/sound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8811 2021-08-06 17:40:46.000000 hum-0.1.9/hum/sound/audio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9151 2021-08-06 17:40:46.000000 hum-0.1.9/hum/sound/audio_librosa.py
+-rw-r--r--   0 runner    (1001) docker     (121)      988 2021-08-06 17:40:46.000000 hum-0.1.9/hum/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-06 17:41:48.090784 hum-0.1.9/hum/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2021-08-06 17:40:46.000000 hum-0.1.9/hum/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3767 2021-08-06 17:40:46.000000 hum-0.1.9/hum/utils/date_ticks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1789 2021-08-06 17:40:46.000000 hum-0.1.9/hum/utils/infinite_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38645 2021-08-06 17:40:46.000000 hum-0.1.9/hum/utils/librosa_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1791 2021-08-06 17:40:46.000000 hum-0.1.9/hum/utils/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-06 17:41:48.090784 hum-0.1.9/hum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    15620 2021-08-06 17:41:47.000000 hum-0.1.9/hum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      586 2021-08-06 17:41:47.000000 hum-0.1.9/hum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-06 17:41:47.000000 hum-0.1.9/hum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-06 17:41:47.000000 hum-0.1.9/hum.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2021-08-06 17:41:47.000000 hum-0.1.9/hum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2021-08-06 17:41:47.000000 hum-0.1.9/hum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      566 2021-08-06 17:41:48.094784 hum-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2021-08-06 17:40:46.000000 hum-0.1.9/setup.py
```

### Comparing `hum-0.1.8/LICENSE` & `hum-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hum-0.1.8/PKG-INFO` & `hum-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hum
-Version: 0.1.8
+Version: 0.1.9
 Summary: Generate synthetic signals for ML pipelines
 Home-page: https://github.com/otosense/hum
 Author: OtoSense
 License: mit
 Description: 
         # hum
         Generate synthetic signals for ML pipelines
```

### Comparing `hum-0.1.8/README.md` & `hum-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `hum-0.1.8/hum/gen/__init__.py` & `hum-0.1.9/hum/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `hum-0.1.8/hum/gen/diagnosis_sounds.py` & `hum-0.1.9/hum/gen/diagnosis_sounds.py`

 * *Files identical despite different names*

### Comparing `hum-0.1.8/hum/gen/signal_generators.py` & `hum-0.1.9/hum/gen/signal_generators.py`

 * *Files identical despite different names*

### Comparing `hum-0.1.8/hum/gen/sine_mix.py` & `hum-0.1.9/hum/gen/sine_mix.py`

 * *Files identical despite different names*

### Comparing `hum-0.1.8/hum/gen/voiced_time.py` & `hum-0.1.9/hum/gen/voiced_time.py`

 * *Files identical despite different names*

### Comparing `hum-0.1.8/hum/lite_sample_sounds.py` & `hum-0.1.9/hum/lite_sample_sounds.py`

 * *Files identical despite different names*

### Comparing `hum-0.1.8/hum/sound/audio.py` & `hum-0.1.9/hum/sound/audio.py`

 * *Files identical despite different names*

### Comparing `hum-0.1.8/hum/sound/audio_librosa.py` & `hum-0.1.9/hum/sound/audio_librosa.py`

 * *Files identical despite different names*

### Comparing `hum-0.1.8/hum/util.py` & `hum-0.1.9/hum/util.py`

 * *Files identical despite different names*

### Comparing `hum-0.1.8/hum/utils/date_ticks.py` & `hum-0.1.9/hum/utils/date_ticks.py`

 * *Files identical despite different names*

### Comparing `hum-0.1.8/hum/utils/infinite_waveform.py` & `hum-0.1.9/hum/utils/infinite_waveform.py`

 * *Files identical despite different names*

### Comparing `hum-0.1.8/hum/utils/librosa_utils.py` & `hum-0.1.9/hum/utils/librosa_utils.py`

 * *Files identical despite different names*

### Comparing `hum-0.1.8/hum/utils/plotting.py` & `hum-0.1.9/hum/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `hum-0.1.8/hum.egg-info/PKG-INFO` & `hum-0.1.9/hum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hum
-Version: 0.1.8
+Version: 0.1.9
 Summary: Generate synthetic signals for ML pipelines
 Home-page: https://github.com/otosense/hum
 Author: OtoSense
 License: mit
 Description: 
         # hum
         Generate synthetic signals for ML pipelines
```

### Comparing `hum-0.1.8/hum.egg-info/SOURCES.txt` & `hum-0.1.9/hum.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 hum.egg-info/requires.txt
 hum.egg-info/top_level.txt
 hum/gen/__init__.py
 hum/gen/diagnosis_sounds.py
 hum/gen/signal_generators.py
 hum/gen/sine_mix.py
 hum/gen/voiced_time.py
+hum/scrap/__init__.py
 hum/sound/__init__.py
 hum/sound/audio.py
 hum/sound/audio_librosa.py
 hum/utils/__init__.py
 hum/utils/date_ticks.py
 hum/utils/infinite_waveform.py
 hum/utils/librosa_utils.py
```

### Comparing `hum-0.1.8/setup.cfg` & `hum-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hum
-version = 0.1.8
+version = 0.1.9
 url = https://github.com/otosense/hum
 platforms = any
 description_file = README.md
 description = Generate synthetic signals for ML pipelines
 license = mit
 keywords = 
 	data
```

