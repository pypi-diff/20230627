# Comparing `tmp/stepcount-2.1.5.tar.gz` & `tmp/stepcount-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepcount-2.1.5.tar", last modified: Wed Jun  7 14:20:33 2023, max compression
+gzip compressed data, was "stepcount-2.1.6.tar", last modified: Tue Jun 27 18:26:16 2023, max compression
```

## Comparing `stepcount-2.1.5.tar` & `stepcount-2.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:20:33.047146 stepcount-2.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-06-07 14:20:21.000000 stepcount-2.1.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-06-07 14:20:33.047146 stepcount-2.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-07 14:20:21.000000 stepcount-2.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-07 14:20:21.000000 stepcount-2.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 14:20:33.047146 stepcount-2.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-07 14:20:21.000000 stepcount-2.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:20:33.043146 stepcount-2.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:20:33.047146 stepcount-2.1.5/src/stepcount/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-07 14:20:21.000000 stepcount-2.1.5/src/stepcount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-07 14:20:33.047146 stepcount-2.1.5/src/stepcount/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-06-07 14:20:21.000000 stepcount-2.1.5/src/stepcount/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-06-07 14:20:21.000000 stepcount-2.1.5/src/stepcount/hmm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21831 2023-06-07 14:20:21.000000 stepcount-2.1.5/src/stepcount/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-06-07 14:20:21.000000 stepcount-2.1.5/src/stepcount/sslmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-06-07 14:20:21.000000 stepcount-2.1.5/src/stepcount/stepcount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:20:33.047146 stepcount-2.1.5/src/stepcount/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 14:20:21.000000 stepcount-2.1.5/src/stepcount/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-07 14:20:21.000000 stepcount-2.1.5/src/stepcount/utils/collate_outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:20:33.047146 stepcount-2.1.5/src/stepcount.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-06-07 14:20:32.000000 stepcount-2.1.5/src/stepcount.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-07 14:20:33.000000 stepcount-2.1.5/src/stepcount.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:20:32.000000 stepcount-2.1.5/src/stepcount.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-07 14:20:32.000000 stepcount-2.1.5/src/stepcount.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-07 14:20:32.000000 stepcount-2.1.5/src/stepcount.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 14:20:32.000000 stepcount-2.1.5/src/stepcount.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-07 14:20:21.000000 stepcount-2.1.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:26:16.508912 stepcount-2.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-06-27 18:26:06.000000 stepcount-2.1.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-06-27 18:26:16.508912 stepcount-2.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-27 18:26:06.000000 stepcount-2.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-27 18:26:06.000000 stepcount-2.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:26:16.508912 stepcount-2.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-27 18:26:06.000000 stepcount-2.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:26:16.504912 stepcount-2.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:26:16.508912 stepcount-2.1.6/src/stepcount/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-27 18:26:06.000000 stepcount-2.1.6/src/stepcount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-27 18:26:16.508912 stepcount-2.1.6/src/stepcount/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-06-27 18:26:06.000000 stepcount-2.1.6/src/stepcount/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-06-27 18:26:06.000000 stepcount-2.1.6/src/stepcount/hmm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21831 2023-06-27 18:26:06.000000 stepcount-2.1.6/src/stepcount/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-06-27 18:26:06.000000 stepcount-2.1.6/src/stepcount/sslmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12595 2023-06-27 18:26:06.000000 stepcount-2.1.6/src/stepcount/stepcount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:26:16.508912 stepcount-2.1.6/src/stepcount/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-27 18:26:06.000000 stepcount-2.1.6/src/stepcount/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-27 18:26:06.000000 stepcount-2.1.6/src/stepcount/utils/collate_outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:26:16.508912 stepcount-2.1.6/src/stepcount.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-06-27 18:26:16.000000 stepcount-2.1.6/src/stepcount.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-27 18:26:16.000000 stepcount-2.1.6/src/stepcount.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:26:16.000000 stepcount-2.1.6/src/stepcount.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-27 18:26:16.000000 stepcount-2.1.6/src/stepcount.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-27 18:26:16.000000 stepcount-2.1.6/src/stepcount.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 18:26:16.000000 stepcount-2.1.6/src/stepcount.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-27 18:26:06.000000 stepcount-2.1.6/versioneer.py
```

### Comparing `stepcount-2.1.5/LICENSE.md` & `stepcount-2.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.5/PKG-INFO` & `stepcount-2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepcount
-Version: 2.1.5
+Version: 2.1.6
 Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
 Home-page: https://github.com/OxWearables/stepcount
 Download-URL: https://github.com/OxWearables/stepcount
 Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE file.
```

### Comparing `stepcount-2.1.5/README.md` & `stepcount-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.5/pyproject.toml` & `stepcount-2.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.5/setup.py` & `stepcount-2.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Scientific/Engineering :: Medical Science Apps.",
     ],
     packages=setuptools.find_packages(where="src", exclude=("test", "tests")),
     package_dir={"": "src"},
     include_package_data=False,
     install_requires=[
-        "actipy==2.0.4",
+        "actipy==2.1.0",
         "numpy==1.24.*",
         "scipy==1.10.*",
         "pandas==1.5.*",
         "tqdm==4.64.*",
         "joblib==1.2.*",
         "scikit-learn==1.1.1",
         "imbalanced-learn==0.9.1",
```

### Comparing `stepcount-2.1.5/src/stepcount/__init__.py` & `stepcount-2.1.6/src/stepcount/__init__.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.5/src/stepcount/features.py` & `stepcount-2.1.6/src/stepcount/features.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.5/src/stepcount/hmm_utils.py` & `stepcount-2.1.6/src/stepcount/hmm_utils.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.5/src/stepcount/models.py` & `stepcount-2.1.6/src/stepcount/models.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.5/src/stepcount/sslmodel.py` & `stepcount-2.1.6/src/stepcount/sslmodel.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.5/src/stepcount/stepcount.py` & `stepcount-2.1.6/src/stepcount/stepcount.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,17 @@
             data = pd.read_pickle(filepath)
         else:
             raise ValueError(f"Unknown file format: {ftype}")
 
         freq = infer_freq(data.index)
         sample_rate = int(np.round(pd.Timedelta('1s') / freq))
 
+        # Quick fix: Drop duplicate indices. TODO: Maybe should be handled by actipy.
+        data = data[~data.index.duplicated(keep='first')]
+
         data, info = actipy.process(
             data, sample_rate,
             lowpass_hz=None,
             calibrate_gravity=True,
             detect_nonwear=True,
             resample_hz=resample_hz,
         )
```

### Comparing `stepcount-2.1.5/src/stepcount/utils/collate_outputs.py` & `stepcount-2.1.6/src/stepcount/utils/collate_outputs.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.5/src/stepcount.egg-info/PKG-INFO` & `stepcount-2.1.6/src/stepcount.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepcount
-Version: 2.1.5
+Version: 2.1.6
 Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
 Home-page: https://github.com/OxWearables/stepcount
 Download-URL: https://github.com/OxWearables/stepcount
 Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE file.
```

### Comparing `stepcount-2.1.5/src/stepcount.egg-info/SOURCES.txt` & `stepcount-2.1.6/src/stepcount.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.5/versioneer.py` & `stepcount-2.1.6/versioneer.py`

 * *Files identical despite different names*

