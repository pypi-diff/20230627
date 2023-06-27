# Comparing `tmp/ms2pip-3.9.0.tar.gz` & `tmp/ms2pip-4.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms2pip-3.9.0.tar", last modified: Sat Mar 12 20:01:04 2022, max compression
+gzip compressed data, was "ms2pip-4.0.0.dev0.tar", last modified: Tue Jun 27 13:59:03 2023, max compression
```

## Comparing `ms2pip-3.9.0.tar` & `ms2pip-4.0.0.dev0.tar`

### file list

```diff
@@ -1,55 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 20:01:04.939563 ms2pip-3.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-03-12 20:00:52.000000 ms2pip-3.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-03-12 20:00:52.000000 ms2pip-3.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    17992 2022-03-12 20:01:04.939563 ms2pip-3.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16825 2022-03-12 20:00:52.000000 ms2pip-3.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 20:01:04.891563 ms2pip-3.9.0/fasta2speclib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 20:00:52.000000 ms2pip-3.9.0/fasta2speclib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17938 2022-03-12 20:00:52.000000 ms2pip-3.9.0/fasta2speclib/fasta2speclib.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 20:01:04.895563 ms2pip-3.9.0/ms2pip/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 20:00:52.000000 ms2pip-3.9.0/ms2pip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5661 2022-03-12 20:00:52.000000 ms2pip-3.9.0/ms2pip/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3646 2022-03-12 20:00:52.000000 ms2pip-3.9.0/ms2pip/config_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 20:01:04.895563 ms2pip-3.9.0/ms2pip/cython_modules/
--rw-r--r--   0 runner    (1001) docker     (121)     3529 2022-03-12 20:00:52.000000 ms2pip-3.9.0/ms2pip/cython_modules/ms2pip_features_c_catboost.c
--rw-r--r--   0 runner    (1001) docker     (121)     3541 2022-03-12 20:00:52.000000 ms2pip-3.9.0/ms2pip/cython_modules/ms2pip_features_c_ce.c
--rw-r--r--   0 runner    (1001) docker     (121)     3294 2022-03-12 20:00:52.000000 ms2pip-3.9.0/ms2pip/cython_modules/ms2pip_features_c_general.c
--rw-r--r--   0 runner    (1001) docker     (121)    13545 2022-03-12 20:00:52.000000 ms2pip-3.9.0/ms2pip/cython_modules/ms2pip_features_c_old.c
--rw-r--r--   0 runner    (1001) docker     (121)     2927 2022-03-12 20:00:52.000000 ms2pip-3.9.0/ms2pip/cython_modules/ms2pip_init_c.c
--rw-r--r--   0 runner    (1001) docker     (121)    19637 2022-03-12 20:00:52.000000 ms2pip-3.9.0/ms2pip/cython_modules/ms2pip_peaks_c.c
--rw-r--r--   0 runner    (1001) docker     (121)     8222 2022-03-12 20:00:52.000000 ms2pip-3.9.0/ms2pip/cython_modules/ms2pip_pyx.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-03-12 20:00:52.000000 ms2pip-3.9.0/ms2pip/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5691 2022-03-12 20:00:52.000000 ms2pip-3.9.0/ms2pip/feature_names.py
--rw-r--r--   0 runner    (1001) docker     (121)     5603 2022-03-12 20:00:52.000000 ms2pip-3.9.0/ms2pip/match_spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 20:01:04.895563 ms2pip-3.9.0/ms2pip/models/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 20:01:04.919563 ms2pip-3.9.0/ms2pip/models/HCD-2019/
--rw-r--r--   0 runner    (1001) docker     (121)  8726156 2022-03-12 20:00:53.000000 ms2pip-3.9.0/ms2pip/models/HCD-2019/model_20190107_HCD_train_B.c
--rw-r--r--   0 runner    (1001) docker     (121)  1664299 2022-03-12 20:00:53.000000 ms2pip-3.9.0/ms2pip/models/HCD-2019/model_20190107_HCD_train_B2.c
--rw-r--r--   0 runner    (1001) docker     (121)  9116794 2022-03-12 20:00:53.000000 ms2pip-3.9.0/ms2pip/models/HCD-2019/model_20190107_HCD_train_Y.c
--rw-r--r--   0 runner    (1001) docker     (121)  9063001 2022-03-12 20:00:53.000000 ms2pip-3.9.0/ms2pip/models/HCD-2019/model_20190107_HCD_train_Y2.c
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-03-12 20:00:52.000000 ms2pip-3.9.0/ms2pip/models/HCD-2019.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 20:01:04.931563 ms2pip-3.9.0/ms2pip/models/TMT/
--rw-r--r--   0 runner    (1001) docker     (121)  2348087 2022-03-12 20:00:53.000000 ms2pip-3.9.0/ms2pip/models/TMT/model_20190107_TMT_train_B.c
--rw-r--r--   0 runner    (1001) docker     (121)  4323734 2022-03-12 20:00:53.000000 ms2pip-3.9.0/ms2pip/models/TMT/model_20190107_TMT_train_Y.c
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-03-12 20:00:53.000000 ms2pip-3.9.0/ms2pip/models/TMT.h
--rw-r--r--   0 runner    (1001) docker     (121)    45727 2022-03-12 20:00:53.000000 ms2pip-3.9.0/ms2pip/ms2pipC.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 20:01:04.939563 ms2pip-3.9.0/ms2pip/ms2pip_tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 20:00:53.000000 ms2pip-3.9.0/ms2pip/ms2pip_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-03-12 20:00:53.000000 ms2pip-3.9.0/ms2pip/ms2pip_tools/calc_correlations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2967 2022-03-12 20:00:53.000000 ms2pip-3.9.0/ms2pip/ms2pip_tools/dlib.py
--rw-r--r--   0 runner    (1001) docker     (121)     4331 2022-03-12 20:00:53.000000 ms2pip-3.9.0/ms2pip/ms2pip_tools/get_elude_predictions.py
--rw-r--r--   0 runner    (1001) docker     (121)    29304 2022-03-12 20:00:53.000000 ms2pip-3.9.0/ms2pip/ms2pip_tools/spectrum_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     5325 2022-03-12 20:00:53.000000 ms2pip-3.9.0/ms2pip/peptides.py
--rw-r--r--   0 runner    (1001) docker     (121)     6200 2022-03-12 20:00:53.000000 ms2pip-3.9.0/ms2pip/predict_xgboost.py
--rw-r--r--   0 runner    (1001) docker     (121)     3870 2022-03-12 20:00:53.000000 ms2pip-3.9.0/ms2pip/retention_time.py
--rw-r--r--   0 runner    (1001) docker     (121)    11220 2022-03-12 20:00:53.000000 ms2pip-3.9.0/ms2pip/single_prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 20:01:04.895563 ms2pip-3.9.0/ms2pip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17992 2022-03-12 20:01:04.000000 ms2pip-3.9.0/ms2pip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-03-12 20:01:04.000000 ms2pip-3.9.0/ms2pip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-12 20:01:04.000000 ms2pip-3.9.0/ms2pip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-03-12 20:01:04.000000 ms2pip-3.9.0/ms2pip.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-03-12 20:01:04.000000 ms2pip-3.9.0/ms2pip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-03-12 20:01:04.000000 ms2pip-3.9.0/ms2pip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-03-12 20:00:53.000000 ms2pip-3.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-03-12 20:01:04.939563 ms2pip-3.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3364 2022-03-12 20:00:53.000000 ms2pip-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:03.065852 ms2pip-4.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-06-27 13:59:03.065852 ms2pip-4.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:03.029852 ms2pip-4.0.0.dev0/ms2pip/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:03.029852 ms2pip-4.0.0.dev0/ms2pip/_cython_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_cython_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_cython_modules/ms2pip_features_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_cython_modules/ms2pip_init_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19526 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_cython_modules/ms2pip_peaks_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_cython_modules/ms2pip_pyx.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:03.029852 ms2pip-4.0.0.dev0/ms2pip/_models_c/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:03.049852 ms2pip-4.0.0.dev0/ms2pip/_models_c/HCD-2019/
+-rw-r--r--   0 runner    (1001) docker     (123)  8726156 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_B.c
+-rw-r--r--   0 runner    (1001) docker     (123)  1664299 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_B2.c
+-rw-r--r--   0 runner    (1001) docker     (123)  9116794 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_Y.c
+-rw-r--r--   0 runner    (1001) docker     (123)  9063001 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_Y2.c
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_models_c/HCD-2019.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:03.061852 ms2pip-4.0.0.dev0/ms2pip/_models_c/TMT/
+-rw-r--r--   0 runner    (1001) docker     (123)  2348087 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_models_c/TMT/model_20190107_TMT_train_B.c
+-rw-r--r--   0 runner    (1001) docker     (123)  4323734 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_models_c/TMT/model_20190107_TMT_train_Y.c
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_models_c/TMT.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:03.065852 ms2pip-4.0.0.dev0/ms2pip/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_utils/dlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_utils/feature_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_utils/psm_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_utils/retention_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/_utils/xgb_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27561 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/spectrum_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29694 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/ms2pip/spectrum_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:03.029852 ms2pip-4.0.0.dev0/ms2pip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-06-27 13:59:03.000000 ms2pip-4.0.0.dev0/ms2pip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-27 13:59:03.000000 ms2pip-4.0.0.dev0/ms2pip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:59:03.000000 ms2pip-4.0.0.dev0/ms2pip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-27 13:59:03.000000 ms2pip-4.0.0.dev0/ms2pip.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-27 13:59:03.000000 ms2pip-4.0.0.dev0/ms2pip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 13:59:03.000000 ms2pip-4.0.0.dev0/ms2pip.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:59:03.065852 ms2pip-4.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:03.065852 ms2pip-4.0.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/tests/test_fasta2speclib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/tests/test_modifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/tests/test_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/tests/test_retention_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-27 13:58:48.000000 ms2pip-4.0.0.dev0/tests/test_spectrum_output.py
```

### Comparing `ms2pip-3.9.0/LICENSE` & `ms2pip-4.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms2pip-3.9.0/ms2pip/cython_modules/ms2pip_features_c_catboost.c` & `ms2pip-4.0.0.dev0/ms2pip/_cython_modules/ms2pip_features_c.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // Compute feature vectors from peptide
-unsigned int* get_v_ms2pip_catboost(int peplen, unsigned short* peptide, unsigned short* modpeptide, int charge)
+unsigned int* get_v_ms2pip(int peplen, unsigned short* peptide, unsigned short* modpeptide, int charge)
 	{
 	int i,j,k;
 
 	int fnum = 1; //first value in v is its length
 
 	for (i=0; i < 19; i++) {
 		count_n[i] = 0;
@@ -14,21 +14,21 @@
 	//important for sptms!!
 	peptide_buf[0] = peptide[0];
 	for (i=0; i < peplen; i++) {
 		if (peptide[i+1] > 18) {
 			peptide_buf[i+1] = sptm_mapper[peptide[i+1]];
 		}
 		else {
-			peptide_buf[i+1] = peptide[i+1]; 
+			peptide_buf[i+1] = peptide[i+1];
 		}
 		count_c[peptide_buf[i+1]]++;
 	}
-	
+
 	int num_shared = 0;
-	
+
 	shared_features[num_shared++] = peplen;
 	shared_features[num_shared++] = charge;
 
 	shared_features[num_shared] = 0;
 	if (charge == 1) {
 		shared_features[num_shared] = 1;
 		}
@@ -36,92 +36,88 @@
 	shared_features[num_shared] = 0;
 	if (charge == 2) {
 		shared_features[num_shared] =1;
 		}
 	num_shared++;
 	shared_features[num_shared] = 0;
 	if (charge == 3) {
-		shared_features[num_shared] =1;    
+		shared_features[num_shared] =1;
 		}
 	num_shared++;
 	shared_features[num_shared] = 0;
 	if (charge == 4) {
-		shared_features[num_shared] =1;    
+		shared_features[num_shared] =1;
 		}
 	num_shared++;
 	shared_features[num_shared] = 0;
 	if (charge >= 5) {
-		shared_features[num_shared]=1;    
+		shared_features[num_shared] =1;
 		}
 	num_shared++;
 
 	for (j=0; j < num_props; j++) {
 		for (i=0; i < peplen; i++) {
 			props_buffer[i] = props[j][peptide_buf[i+1]];
-		}   
+		}
 		qsort(props_buffer,peplen,sizeof(unsigned int),cmpfunc);
 		shared_features[num_shared++] = props_buffer[0];
 		shared_features[num_shared++] = props_buffer[(int)(0.25*(peplen-1))];
 		shared_features[num_shared++] = props_buffer[(int)(0.5*(peplen-1))];
 		shared_features[num_shared++] = props_buffer[(int)(0.75*(peplen-1))];
 		shared_features[num_shared++] = props_buffer[peplen-1];
 	}
 
 	for (i=0; i < peplen-1; i++) {
-		v[fnum++] = peptide_buf[1];
-		v[fnum++] = peptide_buf[peplen];
-		v[fnum++] = peptide_buf[i];
-		v[fnum++] = peptide_buf[i+1];
 		for (j=0; j<num_shared; j++) {
 			v[fnum++] = shared_features[j];
 		}
 		v[fnum++] = i+1;
-		v[fnum++] = peplen-i;       
+		v[fnum++] = peplen-i;
 		count_n[peptide_buf[i+1]]++;
 		count_c[peptide_buf[peplen-i]]--;
 
 		for (j=0; j < 19; j++) {
 			v[fnum++] = count_n[j];
 			v[fnum++] = count_c[j];
 		}
-				
+
 		for (j=0; j < num_props; j++) {
-			v[fnum++] = props[j][peptide_buf[1]];  
-			v[fnum++] = props[j][peptide_buf[peplen]];  
+			v[fnum++] = props[j][peptide_buf[1]];
+			v[fnum++] = props[j][peptide_buf[peplen]];
 			if (i==0) {
-				v[fnum++] = 0;  
+				v[fnum++] = 0;
 			}
-			else {  
-				v[fnum++] = props[j][peptide_buf[i-1]];  
+			else {
+				v[fnum++] = props[j][peptide_buf[i-1]];
 			}
-			v[fnum++] = props[j][peptide_buf[i]];  
-			v[fnum++] = props[j][peptide_buf[i+1]];  
+			v[fnum++] = props[j][peptide_buf[i]];
+			v[fnum++] = props[j][peptide_buf[i+1]];
 			if (i==(peplen-1)) {
-				v[fnum++] = 0;                          
+				v[fnum++] = 0;
 			}
 			else {
-				v[fnum++] = props[j][peptide_buf[i+2]];                         
+				v[fnum++] = props[j][peptide_buf[i+2]];
 			}
 			unsigned int s = 0;
 			for (k=0; k <= i; k++) {
 				props_buffer[k] = props[j][peptide_buf[k+1]];
 				s+= props_buffer[k];
-			}   
+			}
 			v[fnum++] = s;
 			qsort(props_buffer,i+1,sizeof(unsigned int),cmpfunc);
 			v[fnum++] = props_buffer[0];
 			v[fnum++] = props_buffer[(int)(0.25*i)];
 			v[fnum++] = props_buffer[(int)(0.5*i)];
 			v[fnum++] = props_buffer[(int)(0.75*i)];
 			v[fnum++] = props_buffer[i];
 			s = 0;
 			for (k=i+1; k < peplen; k++) {
 				props_buffer[k-i-1] = props[j][peptide_buf[k+1]];
 				s+= props_buffer[k-i-1];
-			}   
+			}
 			v[fnum++] = s;
 			qsort(props_buffer,peplen-i-1,sizeof(unsigned int),cmpfunc);
 			v[fnum++] = props_buffer[0];
 			v[fnum++] = props_buffer[(int)(0.25*(peplen-i-1))];
 			v[fnum++] = props_buffer[(int)(0.5*(peplen-i-1))];
 			v[fnum++] = props_buffer[(int)(0.75*(peplen-i-1))];
 			v[fnum++] = props_buffer[peplen-i-2];
```

### Comparing `ms2pip-3.9.0/ms2pip/cython_modules/ms2pip_init_c.c` & `ms2pip-4.0.0.dev0/ms2pip/_cython_modules/ms2pip_init_c.c`

 * *Files identical despite different names*

### Comparing `ms2pip-3.9.0/ms2pip/cython_modules/ms2pip_peaks_c.c` & `ms2pip-4.0.0.dev0/ms2pip/_cython_modules/ms2pip_peaks_c.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 #include <stdlib.h>
 #include <stdio.h>
 #include <string.h>
 
 #include "ms2pip_init_c.c"
-#include "ms2pip_features_c_general.c"
-#include "ms2pip_features_c_ce.c"
-#include "ms2pip_features_c_old.c"
-#include "ms2pip_features_c_catboost.c"
+#include "ms2pip_features_c.c"
 
-#include "../models/HCD-2019.h"
-#include "../models/TMT.h"
+#include "../_models_c/HCD-2019.h"
+#include "../_models_c/TMT.h"
 
 float membuffer[10000];
 float ions[2000];
 float mzs[2000];
 float predictions[1000];
 
 struct annotations{
```

### Comparing `ms2pip-3.9.0/ms2pip/cython_modules/ms2pip_pyx.pyx` & `ms2pip-4.0.0.dev0/ms2pip/_cython_modules/ms2pip_pyx.pyx`

 * *Files 11% similar despite different names*

```diff
@@ -12,17 +12,14 @@
 	ctypedef struct annotations:
 		float* peaks
 		float* msms
 
 	void init_ms2pip(char* amino_masses_fname, char* modifications_fname, char* modifications_fname_sptm)
 
 	unsigned int* get_v_ms2pip(int peplen, unsigned short* peptide, unsigned short* modpeptide, int charge)
-	unsigned int* get_v_ms2pip_ce(int peplen, unsigned short* peptide, unsigned short* modpeptide, int charge, int ce)
-	unsigned int* get_v_ms2pip_old(int peplen, unsigned short* peptide, unsigned short* modpeptide, int charge)
-	unsigned int* get_v_ms2pip_catboost(int peplen, unsigned short* peptide, unsigned short* modpeptide, int charge)
 
 	float* get_p_ms2pip(int peplen, unsigned short* peptide, unsigned short* modpeptide, int charge, int model_id, int ce)
 
 	float* get_mz_ms2pip_general(int peplen, unsigned short* modpeptide)
 	float* get_mz_ms2pip_etd(int peplen, unsigned short* modpeptide)
 	float* get_mz_ms2pip_ch2(int peplen, unsigned short* modpeptide)
 
@@ -57,52 +54,14 @@
 			v.append(results[j + 1 + offset])
 		offset += fnum
 		r.append(np.array(v, dtype=np.uint16))
 
 	return r
 
 
-def get_vector_ce(np.ndarray[unsigned short, ndim=1, mode="c"] peptide,
-			   np.ndarray[unsigned short, ndim=1, mode="c"] modpeptide,
-			   charge, ce):
-
-	cdef unsigned int* results = get_v_ms2pip_ce(len(peptide)-2, &peptide[0], &modpeptide[0], charge, ce)
-
-	r = []
-	offset = 0
-	fnum = int(results[0] / (len(peptide) - 3))
-	for i in range(len(peptide) - 3):
-		v = []
-		for j in range(fnum):
-			v.append(results[j + 1 + offset])
-		offset += fnum
-		r.append(np.array(v, dtype=np.uint16))
-
-	return r
-
-
-def get_vector_catboost(np.ndarray[unsigned short, ndim=1, mode="c"] peptide,
-						np.ndarray[unsigned short, ndim=1, mode="c"] modpeptide,
-						charge):
-
-	cdef unsigned int* results = get_v_ms2pip_catboost(len(peptide)-2, &peptide[0], &modpeptide[0], charge)
-
-	r = []
-	offset = 0
-	fnum = int(results[0] / (len(peptide) - 3))
-	for i in range(len(peptide) - 3):
-		v = []
-		for j in range(fnum):
-			v.append(results[j + 1 + offset])
-		offset += fnum
-		r.append(np.array(v, dtype=np.uint16))
-
-	return r
-
-
 def get_predictions(np.ndarray[unsigned short, ndim=1, mode="c"] peptide,
 					np.ndarray[unsigned short, ndim=1, mode="c"] modpeptide,
 					charge, model_id, peaks_version, ce):
 	cdef float* results = get_p_ms2pip(len(peptide)-2, &peptide[0], &modpeptide[0], charge, model_id, ce)
 	if results is NULL:
 		raise NotImplementedError(model_id)
 	result_parsed = []
@@ -134,18 +93,17 @@
 	results = get_t_ms2pip_all(len(modpeptide)-2, &modpeptide[0], len(peaks), &msms[0], &peaks[0], fragerror)
 	result_peaks = []
 	for i in range(NUM_ION_TYPES_MAPPING[peaks_version]*(len(modpeptide)-3)):
 		result_peaks.append(results.peaks[i])
 	result_mzs = []
 	for i in range(NUM_ION_TYPES_MAPPING[peaks_version]*(len(modpeptide)-3)):
 		result_mzs.append(results.msms[i])
-	#print(result_parsed)
-	#print()
 	return (result_mzs,result_peaks)
 
+
 def get_targets_general(np.ndarray[unsigned short, ndim=1, mode="c"] modpeptide,
 						np.ndarray[float, ndim=1, mode="c"] msms,
 						np.ndarray[float, ndim=1, mode="c"] peaks,
 						fragerror, peaks_version):
 	cdef float* results = get_t_ms2pip_general(len(modpeptide)-2, &modpeptide[0], len(peaks), &msms[0], &peaks[0], fragerror)
 	result_parsed = []
 	for i in range(NUM_ION_TYPES_MAPPING[peaks_version]): #SD: HAd to change this
```

### Comparing `ms2pip-3.9.0/ms2pip/models/HCD-2019/model_20190107_HCD_train_B.c` & `ms2pip-4.0.0.dev0/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_B.c`

 * *Files identical despite different names*

### Comparing `ms2pip-3.9.0/ms2pip/models/HCD-2019/model_20190107_HCD_train_B2.c` & `ms2pip-4.0.0.dev0/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_B2.c`

 * *Files identical despite different names*

### Comparing `ms2pip-3.9.0/ms2pip/models/HCD-2019/model_20190107_HCD_train_Y.c` & `ms2pip-4.0.0.dev0/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_Y.c`

 * *Files identical despite different names*

### Comparing `ms2pip-3.9.0/ms2pip/models/HCD-2019/model_20190107_HCD_train_Y2.c` & `ms2pip-4.0.0.dev0/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_Y2.c`

 * *Files identical despite different names*

### Comparing `ms2pip-3.9.0/ms2pip/models/TMT/model_20190107_TMT_train_B.c` & `ms2pip-4.0.0.dev0/ms2pip/_models_c/TMT/model_20190107_TMT_train_B.c`

 * *Files identical despite different names*

### Comparing `ms2pip-3.9.0/ms2pip/models/TMT/model_20190107_TMT_train_Y.c` & `ms2pip-4.0.0.dev0/ms2pip/_models_c/TMT/model_20190107_TMT_train_Y.c`

 * *Files identical despite different names*

### Comparing `ms2pip-3.9.0/ms2pip/ms2pip_tools/dlib.py` & `ms2pip-4.0.0.dev0/ms2pip/_utils/dlib.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,26 @@
+"""Database configuration for EncyclopeDIA DLIB SQLite format."""
+
 import zlib
 
 import numpy
 import sqlalchemy
-from sqlalchemy import (Boolean, Column, Float, Index, Integer, MetaData,
-                        String, Table, TypeDecorator)
+from sqlalchemy import (
+    Boolean,
+    Column,
+    Float,
+    Index,
+    Integer,
+    MetaData,
+    String,
+    Table,
+    TypeDecorator,
+)
 from sqlalchemy.dialects.sqlite import BLOB
 
-
 DLIB_VERSION = "0.1.14"
 
 
 class CompressedArray(TypeDecorator):
     """ Sqlite-like does not support arrays.
         Let's use a custom type decorator.
```

### Comparing `ms2pip-3.9.0/ms2pip/ms2pip_tools/spectrum_output.py` & `ms2pip-4.0.0.dev0/ms2pip/spectrum_output.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """
 Write spectrum files from MS2PIP predictions.
 """
+from __future__ import annotations
 
+import csv
 import itertools
 import logging
 import os
 from ast import literal_eval
 from functools import wraps
 from io import StringIO
 from operator import itemgetter
+from pathlib import Path
 from time import localtime, strftime
 from typing import Any, Dict, List
 
-from ms2pip.peptides import Modifications
 
-logger = logging.getLogger("ms2pip.spectrum_output")
+from ms2pip.result import ProcessingResult
+
+logger = logging.getLogger(__name__)
 
 
 class InvalidWriteModeError(ValueError):
     pass
 
 
 # Writer decorator
@@ -43,183 +47,152 @@
             owner.OUTPUT_FORMATS[self.output_format] = self.fn
             setattr(owner, name, self.fn)
 
     return OutputFormat
 
 
 class SpectrumOutput:
-    """
-    Write MS2PIP predictions to various output formats.
-
-    Parameters
-    ----------
-    all_preds: pd.DataFrame
-        MS2PIP predictions
-    peprec: pd.DataFrame
-        PEPREC with peptide information
-    params: dict
-        MS2PIP parameters
-    output_filename: str, optional
-        path and name for output files, will be suffexed with `_predictions` and the
-        relevant file extension (default: ms2pip_predictions)
-    write_mode: str, optional
-        write mode to use: "wt+" to append to start a new file, "at" to append to an
-        existing file (default: "wt+")
-    return_stringbuffer: bool, optional
-        If True, files are written to a StringIO object, which the write function
-        returns. If False, files are written to a file on disk.
-    is_log_space: bool, optional
-        Set to true if predicted intensities in `all_preds` are in log-space. In that
-        case, intensities will first be transformed to "normal"-space.
-
-    Methods
-    -------
-    write_msp()
-        Write predictions to MSP file
-    write_mgf()
-        Write predictions to MGF file
-    write_bibliospec()
-        Write predictions to Bibliospec SSL/MS2 files (also for Skyline)
-    write_spectronaut()
-        Write predictions to Spectronaut CSV file
-    write_dlib()
-        Write predictions to a DLIB SQLite file
-    write_csv()
-        Write predictions to CSV file
-    write_results(output_formats)
-        Write MS2PIP predictions in output formats defined by output_formats.
-
-    Example
-    -------
-    >>> so = ms2pip.spectrum_tools.spectrum_output.SpectrumOutput(
-            all_preds,
-            peprec,
-            params
-        )
-    >>> so.write_msp()
-    >>> so.write_spectronaut()
-
-    """
+    """Write MS2PIP predictions to various output formats."""
 
     OUTPUT_FORMATS = {}
 
     def __init__(
         self,
-        all_preds,
-        peprec,
-        params,
+        results: List["ProcessingResult"],
         output_filename="ms2pip_predictions",
         write_mode="wt+",
         return_stringbuffer=False,
         is_log_space=True,
     ):
-        self.all_preds = all_preds
-        self.peprec = peprec
-        self.params = params
+        """
+        Write MS2PIP predictions to various output formats.
+
+        Parameters
+        ----------
+        results:
+            List of ProcessingResult objects
+        output_filename: str, optional
+            path and name for output files, will be suffexed with `_predictions` and the
+            relevant file extension (default: ms2pip_predictions)
+        write_mode: str, optional
+            write mode to use: "wt+" to append to start a new file, "at" to append to an
+            existing file (default: "wt+")
+        return_stringbuffer: bool, optional
+            If True, files are written to a StringIO object, which the write function
+            returns. If False, files are written to a file on disk.
+        is_log_space: bool, optional
+            Set to true if predicted intensities in `all_preds` are in log-space. In that
+            case, intensities will first be transformed to "normal"-space.
+
+        Example
+        -------
+        >>> so = ms2pip.spectrum_tools.spectrum_output.SpectrumOutput(
+                results
+            )
+        >>> so.write_msp()
+        >>> so.write_spectronaut()
+
+        """
+
+        self.results = results
         self.output_filename = output_filename
         self.write_mode = write_mode
         self.return_stringbuffer = return_stringbuffer
         self.is_log_space = is_log_space
 
-        self.peprec_dict = None
-        self.preds_dict = None
-        self.normalization = None
         self.diff_modification_mapping = {}
 
         self.has_rt = "rt" in self.peprec.columns
         self.has_protein_list = "protein_list" in self.peprec.columns
 
-        self.mods = Modifications()
-        self.mods.add_from_ms2pip_modstrings(params["ptm"])
-
         if self.write_mode not in ["wt+", "wt", "at", "w", "a"]:
             raise InvalidWriteModeError(self.write_mode)
 
         if "a" in self.write_mode and self.return_stringbuffer:
             raise InvalidWriteModeError(self.write_mode)
 
-    def _generate_peprec_dict(self, rt_to_seconds=True):
-        """
-        Create easy to access dict from all_preds and peprec dataframes
-        """
-        peprec_tmp = self.peprec.copy()
-
-        if self.has_rt and rt_to_seconds:
-            peprec_tmp["rt"] = peprec_tmp["rt"] * 60
-
-        peprec_tmp.index = peprec_tmp["spec_id"]
-        peprec_tmp.drop("spec_id", axis=1, inplace=True)
-
-        self.peprec_dict = peprec_tmp.to_dict(orient="index")
-
-    def _generate_preds_dict(self):
-        """
-        Create easy to access dict from peprec dataframes
-        """
-        self.preds_dict = {}
-        preds_list = self.all_preds[
-            ["spec_id", "charge", "ion", "ionnumber", "mz", "prediction"]
-        ].values.tolist()
-
-        for row in preds_list:
-            spec_id = row[0]
-            if spec_id in self.preds_dict.keys():
-                if row[2] in self.preds_dict[spec_id]["peaks"]:
-                    self.preds_dict[spec_id]["peaks"][row[2]].append(tuple(row[3:]))
-                else:
-                    self.preds_dict[spec_id]["peaks"][row[2]] = [tuple(row[3:])]
-            else:
-                self.preds_dict[spec_id] = {
-                    "charge": row[1],
-                    "peaks": {row[2]: [tuple(row[3:])]},
-                }
-
-    def _normalize_spectra(self, method="basepeak_10000"):
-        """
-        Normalize spectra
-        """
-        if self.is_log_space:
-            self.all_preds["prediction"] = (
-                (2 ** self.all_preds["prediction"]) - 0.001
-            ).clip(lower=0)
-            self.is_log_space = False
-
-        if method == "basepeak_10000":
-            if self.normalization == "basepeak_10000":
-                pass
-            elif self.normalization == "basepeak_1":
-                self.all_preds["prediction"] *= 10000
-            else:
-                self.all_preds["prediction"] = self.all_preds.groupby(["spec_id"])[
-                    "prediction"
-                ].apply(lambda x: (x / x.max()) * 10000)
-            self.normalization = "basepeak_10000"
-
-        elif method == "basepeak_1":
-            if self.normalization == "basepeak_1":
-                pass
-            elif self.normalization == "basepeak_10000":
-                self.all_preds["prediction"] /= 10000
-            else:
-                self.all_preds["prediction"] = self.all_preds.groupby(["spec_id"])[
-                    "prediction"
-                ].apply(lambda x: (x / x.max()))
-            self.normalization = "basepeak_1"
-
-        elif method == "tic":
-            if self.normalization != "tic":
-                self.all_preds["prediction"] = self.all_preds.groupby(["spec_id"])[
-                    "prediction"
-                ].apply(lambda x: x / x.sum())
-            self.normalization = "tic"
+    # def _generate_peprec_dict(self, rt_to_seconds=True):
+    #     """
+    #     Create easy to access dict from all_preds and peprec dataframes
+    #     """
+    #     peprec_tmp = self.peprec.copy()
+
+    #     if self.has_rt and rt_to_seconds:
+    #         peprec_tmp["rt"] = peprec_tmp["rt"] * 60
+
+    #     peprec_tmp.index = peprec_tmp["spec_id"]
+    #     peprec_tmp.drop("spec_id", axis=1, inplace=True)
+
+    #     self.peprec_dict = peprec_tmp.to_dict(orient="index")
+
+    # def _generate_preds_dict(self):
+    #     """
+    #     Create easy to access dict from peprec dataframes
+    #     """
+    #     self.preds_dict = {}
+    #     preds_list = self.all_preds[
+    #         ["spec_id", "charge", "ion", "ionnumber", "mz", "prediction"]
+    #     ].values.tolist()
+
+    #     for row in preds_list:
+    #         spec_id = row[0]
+    #         if spec_id in self.preds_dict.keys():
+    #             if row[2] in self.preds_dict[spec_id]["peaks"]:
+    #                 self.preds_dict[spec_id]["peaks"][row[2]].append(tuple(row[3:]))
+    #             else:
+    #                 self.preds_dict[spec_id]["peaks"][row[2]] = [tuple(row[3:])]
+    #         else:
+    #             self.preds_dict[spec_id] = {
+    #                 "charge": row[1],
+    #                 "peaks": {row[2]: [tuple(row[3:])]},
+    #             }
+
+    # def _normalize_spectra(self, method="basepeak_10000"):
+    #     """
+    #     Normalize spectra
+    #     """
+    #     if self.is_log_space:
+    #         self.all_preds["prediction"] = ((2 ** self.all_preds["prediction"]) - 0.001).clip(
+    #             lower=0
+    #         )
+    #         self.is_log_space = False
+
+    #     if method == "basepeak_10000":
+    #         if self.normalization == "basepeak_10000":
+    #             pass
+    #         elif self.normalization == "basepeak_1":
+    #             self.all_preds["prediction"] *= 10000
+    #         else:
+    #             self.all_preds["prediction"] = self.all_preds.groupby(
+    #                 ["spec_id"], group_keys=False
+    #             )["prediction"].apply(lambda x: (x / x.max()) * 10000)
+    #         self.normalization = "basepeak_10000"
+
+    #     elif method == "basepeak_1":
+    #         if self.normalization == "basepeak_1":
+    #             pass
+    #         elif self.normalization == "basepeak_10000":
+    #             self.all_preds["prediction"] /= 10000
+    #         else:
+    #             self.all_preds["prediction"] = self.all_preds.groupby(
+    #                 ["spec_id"], group_keys=False
+    #             )["prediction"].apply(lambda x: (x / x.max()))
+    #         self.normalization = "basepeak_1"
+
+    #     elif method == "tic":
+    #         if self.normalization != "tic":
+    #             self.all_preds["prediction"] = self.all_preds.groupby(
+    #                 ["spec_id"], group_keys=False
+    #             )["prediction"].apply(lambda x: x / x.sum())
+    #         self.normalization = "tic"
 
-        else:
-            raise NotImplementedError
+    #     else:
+    #         raise NotImplementedError
 
-    def _get_peak_string(
+    def _get_msp_peak_annotation(
         self,
         peak_dict,
         sep="\t",
         include_zero=False,
         include_annotations=True,
         intensity_type=float,
     ):
@@ -231,15 +204,15 @@
             for peak in peaks:
                 if not include_zero and peak[2] == 0:
                     continue
                 if include_annotations:
                     all_peaks.append(
                         (
                             peak[1],
-                            f'{peak[1]:.6f}{sep}{intensity_type(peak[2])}{sep}"{ion_type.lower()}{peak[0]}"',
+                            f'{peak[1]:.6f}{sep}{intensity_type(peak[2])}{sep}"{ion_type.lower()}{peak[0]}/0.0"',
                         )
                     )
                 else:
                     all_peaks.append((peak[1], f"{peak[1]:.6f}{sep}{peak[2]}"))
 
         all_peaks = sorted(all_peaks, key=itemgetter(0))
         peak_string = "\n".join([peak[1] for peak in all_peaks])
@@ -248,20 +221,21 @@
 
     def _get_msp_modifications(self, sequence, modifications):
         """
         Format modifications in MSP-style, e.g. "1/0,E,Glu->pyro-Glu"
         """
 
         if isinstance(modifications, str):
-            if modifications == "-":
+            if not modifications or modifications == "-":
                 msp_modifications = "0"
             else:
                 mods = modifications.split("|")
                 mods = [(int(mods[i]), mods[i + 1]) for i in range(0, len(mods), 2)]
                 mods = [(x, y) if x == 0 else (x - 1, y) for (x, y) in mods]
+                mods = sorted(mods)
                 mods = [(str(x), sequence[x], y) for (x, y) in mods]
                 msp_modifications = "/".join([",".join(list(x)) for x in mods])
                 msp_modifications = f"{len(mods)}/{msp_modifications}"
         else:
             msp_modifications = "0"
 
         return msp_modifications
@@ -304,28 +278,37 @@
     def _get_diff_modified_sequence(self, sequence, modifications, precision=1):
         """
         Build BiblioSpec SSL modified sequence string.
         """
         pep = list(sequence)
         mapping = self.diff_modification_mapping[precision]
 
-        for loc, name in zip(
-            modifications.split("|")[::2], modifications.split("|")[1::2]
-        ):
+        for loc, name in zip(modifications.split("|")[::2], modifications.split("|")[1::2]):
             # C-term mod
             if loc == "-1":
                 pep[-1] = pep[-1] + "[{}]".format(mapping[name])
             # N-term mod
             elif loc == "0":
                 pep[0] = pep[0] + "[{}]".format(mapping[name])
             # Normal mod
             else:
                 pep[int(loc) - 1] = pep[int(loc) - 1] + "[{}]".format(mapping[name])
         return "".join(pep)
 
+    def write_results(self, output_formats: List[str]) -> Dict[str, Any]:
+        """
+        Write MS2PIP predictions in output formats defined by output_formats.
+        """
+        results = {}
+        for output_format in output_formats:
+            output_format = output_format.lower()
+            writer = self.OUTPUT_FORMATS[output_format]
+            results[output_format] = writer(self)
+        return results
+
     @output_format("msp")
     @writer(
         file_suffix="_predictions.msp",
         normalization_method="basepeak_10000",
         requires_dicts=True,
         requires_diff_modifications=False,
     )
@@ -337,39 +320,36 @@
         for spec_id in sorted(self.peprec_dict.keys()):
             seq = self.peprec_dict[spec_id]["peptide"]
             mods = self.peprec_dict[spec_id]["modifications"]
             charge = self.peprec_dict[spec_id]["charge"]
             prec_mass, prec_mz = self.mods.calc_precursor_mz(seq, mods, charge)
             msp_modifications = self._get_msp_modifications(seq, mods)
             num_peaks = sum(
-                [
-                    len(peaklist)
-                    for _, peaklist in self.preds_dict[spec_id]["peaks"].items()
-                ]
+                [len(peaklist) for _, peaklist in self.preds_dict[spec_id]["peaks"].items()]
             )
 
             comment_line = f" Mods={msp_modifications} Parent={prec_mz}"
 
             if self.has_protein_list:
                 protein_list = self.peprec_dict[spec_id]["protein_list"]
                 protein_string = self._parse_protein_string(protein_list)
                 comment_line += f' Protein="{protein_string}"'
 
             if self.has_rt:
                 rt = self.peprec_dict[spec_id]["rt"]
-                comment_line += f" RTINSECONDS={rt}"
+                comment_line += f" RetentionTime={rt}"
 
             comment_line += f' MS2PIP_ID="{spec_id}"'
 
             out = [
                 f"Name: {seq}/{charge}",
                 f"MW: {prec_mass}",
                 f"Comment:{comment_line}",
                 f"Num peaks: {num_peaks}",
-                self._get_peak_string(
+                self._get_msp_peak_annotation(
                     self.preds_dict[spec_id]["peaks"],
                     sep="\t",
                     include_annotations=True,
                     intensity_type=int,
                 ),
             ]
 
@@ -386,15 +366,15 @@
         """
         Construct MGF string and write to file_object
         """
         for spec_id in sorted(self.peprec_dict.keys()):
             seq = self.peprec_dict[spec_id]["peptide"]
             mods = self.peprec_dict[spec_id]["modifications"]
             charge = self.peprec_dict[spec_id]["charge"]
-            prec_mass, prec_mz = self.mods.calc_precursor_mz(seq, mods, charge)
+            _, prec_mz = self.mods.calc_precursor_mz(seq, mods, charge)
             msp_modifications = self._get_msp_modifications(seq, mods)
 
             if self.has_protein_list:
                 protein_list = self.peprec_dict[spec_id]["protein_list"]
                 protein_string = self._parse_protein_string(protein_list)
             else:
                 protein_string = ""
@@ -407,15 +387,15 @@
             ]
 
             if self.has_rt:
                 rt = self.peprec_dict[spec_id]["rt"]
                 out.append(f"RTINSECONDS={rt}")
 
             out.append(
-                self._get_peak_string(
+                self._get_msp_peak_annotation(
                     self.preds_dict[spec_id]["peaks"],
                     sep=" ",
                     include_annotations=False,
                 )
             )
             out.append("END IONS\n")
             file_object.writelines([line + "\n" for line in out])
@@ -438,28 +418,24 @@
         else:
             raise InvalidWriteModeError(self.write_mode)
 
         spectronaut_peprec = self.peprec.copy()
 
         # ModifiedPeptide and PrecursorMz columns
         spectronaut_peprec["ModifiedPeptide"] = spectronaut_peprec.apply(
-            lambda row: self._get_diff_modified_sequence(
-                row["peptide"], row["modifications"]
-            ),
+            lambda row: self._get_diff_modified_sequence(row["peptide"], row["modifications"]),
             axis=1,
         )
         spectronaut_peprec["PrecursorMz"] = spectronaut_peprec.apply(
             lambda row: self.mods.calc_precursor_mz(
                 row["peptide"], row["modifications"], row["charge"]
             )[1],
             axis=1,
         )
-        spectronaut_peprec["ModifiedPeptide"] = (
-            "_" + spectronaut_peprec["ModifiedPeptide"] + "_"
-        )
+        spectronaut_peprec["ModifiedPeptide"] = "_" + spectronaut_peprec["ModifiedPeptide"] + "_"
 
         # Additional columns
         spectronaut_peprec["FragmentLossType"] = "noloss"
 
         # Retention time
         if "rt" in spectronaut_peprec.columns:
             rt_cols = ["iRT"]
@@ -511,49 +487,52 @@
             "FragmentCharge",
             "FragmentMz",
             "RelativeIntensity",
             "FragmentType",
             "FragmentNumber",
         ]
         spectronaut_df = spectronaut_df[peptide_cols + fragment_cols]
-        spectronaut_df.to_csv(file_obj, index=False, header=header)
+        try:
+            spectronaut_df.to_csv(
+                file_obj, index=False, header=header, sep=";", lineterminator="\n"
+            )
+        except TypeError:  # Pandas < 1.5 (Required for Python 3.7 support)
+            spectronaut_df.to_csv(
+                file_obj, index=False, header=header, sep=";", line_terminator="\n"
+            )
 
         return file_obj
 
     def _write_bibliospec_core(self, file_obj_ssl, file_obj_ms2, start_scannr=0):
-        """
-        Construct Bibliospec SSL/MS2 strings and write to file_objects.
-        """
+        """Construct Bibliospec SSL/MS2 strings and write to file_objects."""
 
         for i, spec_id in enumerate(sorted(self.preds_dict.keys())):
             scannr = i + start_scannr
             seq = self.peprec_dict[spec_id]["peptide"]
             mods = self.peprec_dict[spec_id]["modifications"]
             charge = self.peprec_dict[spec_id]["charge"]
             prec_mass, prec_mz = self.mods.calc_precursor_mz(seq, mods, charge)
             ms2_filename = os.path.basename(self.output_filename) + "_predictions.ms2"
 
-            peaks = self._get_peak_string(
+            peaks = self._get_msp_peak_annotation(
                 self.preds_dict[spec_id]["peaks"],
                 sep="\t",
                 include_annotations=False,
             )
 
             if isinstance(mods, str) and mods != "-" and mods != "":
                 mod_seq = self._get_diff_modified_sequence(seq, mods)
             else:
                 mod_seq = seq
 
             rt = self.peprec_dict[spec_id]["rt"] if self.has_rt else ""
 
             # TODO: implement csv instead of manual writing
             file_obj_ssl.write(
-                "\t".join(
-                    [ms2_filename, str(scannr), str(charge), mod_seq, "", "", str(rt)]
-                )
+                "\t".join([ms2_filename, str(scannr), str(charge), mod_seq, "", "", str(rt)])
                 + "\n"
             )
             file_obj_ms2.write(
                 "\n".join(
                     [
                         f"S\t{scannr}\t{prec_mz}",
                         f"Z\t{charge}\t{prec_mass}",
@@ -595,31 +574,27 @@
             and diff_modification_precision not in self.diff_modification_mapping
         ):
             self._generate_diff_modification_mapping(diff_modification_precision)
 
         # Write to file or stringbuffer
         if self.return_stringbuffer:
             file_object = StringIO()
-            logger.info("writing results to StringIO using %s", write_function.__name__)
+            logger.info("Writing results to StringIO using %s", write_function.__name__)
         else:
             f_name = self.output_filename + file_suffix
             file_object = open(f_name, self.write_mode)
-            logger.info("writing results to %s", f_name)
+            logger.info("Writing results to %s", f_name)
 
         write_function(self, file_object)
 
         return file_object
 
     @output_format("bibliospec")
     def write_bibliospec(self):
-        """
-        Write MS2PIP predictions to BiblioSpec SSL and MS2 spectral library files
-        (For example for use in Skyline).
-        """
-
+        """Write MS2PIP predictions to BiblioSpec/Skyline SSL and MS2 spectral library files."""
         precision = 1
         if precision not in self.diff_modification_mapping:
             self._generate_diff_modification_mapping(precision)
 
         # Normalize if necessary and make dicts
         if not self.normalization == "basepeak_10000":
             self._normalize_spectra(method="basepeak_10000")
@@ -629,20 +604,16 @@
         if not self.peprec_dict:
             self._generate_peprec_dict()
 
         if self.return_stringbuffer:
             file_obj_ssl = StringIO()
             file_obj_ms2 = StringIO()
         else:
-            file_obj_ssl = open(
-                "{}_predictions.ssl".format(self.output_filename), self.write_mode
-            )
-            file_obj_ms2 = open(
-                "{}_predictions.ms2".format(self.output_filename), self.write_mode
-            )
+            file_obj_ssl = open("{}_predictions.ssl".format(self.output_filename), self.write_mode)
+            file_obj_ms2 = open("{}_predictions.ms2".format(self.output_filename), self.write_mode)
 
         # If a new file is written, write headers
         if "w" in self.write_mode:
             start_scannr = 0
             ssl_header = [
                 "file",
                 "scan",
@@ -651,66 +622,59 @@
                 "score-type",
                 "score",
                 "retention-time",
                 "\n",
             ]
             file_obj_ssl.write("\t".join(ssl_header))
             file_obj_ms2.write(
-                "H\tCreationDate\t{}\n".format(
-                    strftime("%Y-%m-%d %H:%M:%S", localtime())
-                )
+                "H\tCreationDate\t{}\n".format(strftime("%Y-%m-%d %H:%M:%S", localtime()))
             )
             file_obj_ms2.write("H\tExtractor\tMS2PIP predictions\n")
         else:
             # Get last scan number of ssl file, to continue indexing from there
             # because Bibliospec speclib scan numbers can only be integers
             start_scannr = self._get_last_ssl_scannr() + 1
 
-        self._write_bibliospec_core(
-            file_obj_ssl, file_obj_ms2, start_scannr=start_scannr
-        )
+        self._write_bibliospec_core(file_obj_ssl, file_obj_ms2, start_scannr=start_scannr)
 
         return file_obj_ssl, file_obj_ms2
 
     def _write_dlib_metadata(self, connection):
-        from ms2pip.ms2pip_tools.dlib import DLIB_VERSION, Metadata
         from sqlalchemy import select
 
+        from ms2pip._utils.dlib import DLIB_VERSION, Metadata
+
         with connection.begin():
             version = connection.execute(
                 select([Metadata.c.Value]).where(Metadata.c.Key == "version")
             ).scalar()
             if version is None:
                 connection.execute(
                     Metadata.insert().values(
                         Key="version",
                         Value=DLIB_VERSION,
                     )
                 )
 
     def _write_dlib_entries(self, connection, precision):
-        from ms2pip.ms2pip_tools.dlib import Entry
+        from ms2pip._utils.dlib import Entry
 
         peptide_to_proteins = set()
 
         with connection.begin():
             for spec_id, peprec in self.peprec_dict.items():
                 seq = peprec["peptide"]
                 mods = peprec["modifications"]
                 charge = peprec["charge"]
 
                 prec_mass, prec_mz = self.mods.calc_precursor_mz(seq, mods, charge)
-                mod_seq = self._get_diff_modified_sequence(
-                    seq, mods, precision=precision
-                )
+                mod_seq = self._get_diff_modified_sequence(seq, mods, precision=precision)
 
                 all_peaks = sorted(
-                    itertools.chain.from_iterable(
-                        self.preds_dict[spec_id]["peaks"].values()
-                    ),
+                    itertools.chain.from_iterable(self.preds_dict[spec_id]["peaks"].values()),
                     key=itemgetter(1),
                 )
                 mzs = [peak[1] for peak in all_peaks]
                 intensities = [peak[2] for peak in all_peaks]
 
                 connection.execute(
                     Entry.insert().values(
@@ -736,26 +700,24 @@
 
                     for protein in protein_list:
                         peptide_to_proteins.add((seq, protein))
 
         return peptide_to_proteins
 
     def _write_dlib_peptide_to_protein(self, connection, peptide_to_proteins):
-        from ms2pip.ms2pip_tools.dlib import PeptideToProtein
+        from ms2pip._utils.dlib import PeptideToProtein
 
         if not self.has_protein_list:
             return
 
         with connection.begin():
             sql_peptide_to_proteins = set()
             proteins = {protein for _, protein in peptide_to_proteins}
             for peptide_to_protein in connection.execute(
-                PeptideToProtein.select().where(
-                    PeptideToProtein.c.ProteinAccession.in_(proteins)
-                )
+                PeptideToProtein.select().where(PeptideToProtein.c.ProteinAccession.in_(proteins))
             ):
                 sql_peptide_to_proteins.add(
                     (
                         peptide_to_protein.PeptideSeq,
                         peptide_to_protein.ProteinAccession,
                     )
                 )
@@ -766,82 +728,95 @@
                     PeptideToProtein.insert().values(
                         PeptideSeq=seq, isDecoy=False, ProteinAccession=protein
                     )
                 )
 
     @output_format("dlib")
     def write_dlib(self):
-        """
-        Write MS2PIP predictions to a DLIB SQLite file.
-        """
-        from ms2pip.ms2pip_tools.dlib import metadata, open_sqlite
+        """Write MS2PIP predictions to a DLIB SQLite file."""
+        from ms2pip._utils.dlib import metadata, open_sqlite
 
         normalization = "basepeak_10000"
         precision = 5
         if not self.normalization == normalization:
             self._normalize_spectra(method=normalization)
             self._generate_preds_dict()
         if not self.peprec_dict:
             self._generate_peprec_dict()
         if precision not in self.diff_modification_mapping:
             self._generate_diff_modification_mapping(precision)
 
         filename = "{}.dlib".format(self.output_filename)
-        logger.info("writing results to %s", filename)
+        logger.info("Writing results to %s", filename)
 
         logger.debug(
             "write mode is ignored for DLIB at the file mode, although append or not is respected"
         )
         if "a" not in self.write_mode and os.path.exists(filename):
             os.remove(filename)
 
         if self.return_stringbuffer:
-            raise NotImplementedError(
-                "`return_stringbuffer` not implemented for DLIB output."
-            )
+            raise NotImplementedError("`return_stringbuffer` not implemented for DLIB output.")
 
         if not self.has_rt:
             raise NotImplementedError("Retention times required to write DLIB file.")
 
         with open_sqlite(filename) as connection:
             metadata.create_all()
             self._write_dlib_metadata(connection)
             peptide_to_proteins = self._write_dlib_entries(connection, precision)
             self._write_dlib_peptide_to_protein(connection, peptide_to_proteins)
 
     def get_normalized_predictions(self, normalization_method="tic"):
-        """
-        Return normalized copy of predictions.
-        """
+        """Return normalized copy of predictions."""
         self._normalize_spectra(method=normalization_method)
         return self.all_preds.copy()
 
     @output_format("csv")
     def write_csv(self):
-        """
-        Write MS2PIP predictions to CSV.
-        """
+        """Write MS2PIP predictions to CSV."""
 
         self._normalize_spectra(method="tic")
 
         # Write to file or stringbuffer
         if self.return_stringbuffer:
             file_object = StringIO()
-            logger.info("writing results to StringIO using %s", "write_csv")
+            logger.info("Writing results to StringIO using %s", "write_csv")
         else:
             f_name = "{}_predictions.csv".format(self.output_filename)
             file_object = open(f_name, self.write_mode)
-            logger.info("writing results to %s", f_name)
+            logger.info("Writing results to %s", f_name)
 
-        self.all_preds.to_csv(file_object, float_format="%.6g", index=False)
+        try:
+            self.all_preds.to_csv(
+                file_object, float_format="%.6g", index=False, lineterminator="\n"
+            )
+        except TypeError:  # Pandas < 1.5 (Required for Python 3.7 support)
+            self.all_preds.to_csv(
+                file_object, float_format="%.6g", index=False, line_terminator="\n"
+            )
         return file_object
 
-    def write_results(self, output_formats: List[str]) -> Dict[str, Any]:
-        """
-        Write MS2PIP predictions in output formats defined by output_formats.
-        """
-        results = {}
-        for output_format in output_formats:
-            output_format = output_format.lower()
-            writer = self.OUTPUT_FORMATS[output_format]
-            results[output_format] = writer(self)
-        return results
+
+def write_single_spectrum_csv(spectrum, filepath):
+    """Write a single spectrum to a CSV file."""
+    with open(filepath, "wt") as f:
+        writer = csv.writer(f, delimiter=",", lineterminator="\n")
+        writer.writerow(["mz", "intensity", "annotation"])
+        for mz, intensity, annotation in zip(
+            spectrum.mz,
+            spectrum.intensity,
+            spectrum.annotations,
+        ):
+            writer.writerow([mz, intensity, annotation])
+
+
+def write_single_spectrum_png(spectrum, filepath):
+    """Plot a single spectrum and write to a PNG file."""
+    import matplotlib.pyplot as plt
+    import spectrum_utils.plot as sup
+
+    ax = plt.gca()
+    ax.set_title("MS²PIP prediction for " + str(spectrum.peptidoform))
+    sup.spectrum(spectrum.to_spectrum_utils(), ax=ax)
+    plt.savefig(Path(filepath).with_suffix(".png"))
+    plt.close()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ms2pip-3.9.0/ms2pip.egg-info/SOURCES.txt` & `ms2pip-4.0.0.dev0/ms2pip.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 LICENSE
 MANIFEST.in
-README.md
+README.rst
 pyproject.toml
-setup.cfg
 setup.py
-fasta2speclib/__init__.py
-fasta2speclib/fasta2speclib.py
 ms2pip/__init__.py
 ms2pip/__main__.py
-ms2pip/config_parser.py
+ms2pip/constants.py
+ms2pip/core.py
+ms2pip/correlation.py
 ms2pip/exceptions.py
-ms2pip/feature_names.py
-ms2pip/match_spectra.py
-ms2pip/ms2pipC.py
-ms2pip/peptides.py
-ms2pip/predict_xgboost.py
-ms2pip/retention_time.py
-ms2pip/single_prediction.py
+ms2pip/result.py
+ms2pip/spectrum.py
+ms2pip/spectrum_input.py
+ms2pip/spectrum_output.py
 ms2pip.egg-info/PKG-INFO
 ms2pip.egg-info/SOURCES.txt
 ms2pip.egg-info/dependency_links.txt
 ms2pip.egg-info/entry_points.txt
 ms2pip.egg-info/requires.txt
 ms2pip.egg-info/top_level.txt
-ms2pip/cython_modules/ms2pip_features_c_catboost.c
-ms2pip/cython_modules/ms2pip_features_c_ce.c
-ms2pip/cython_modules/ms2pip_features_c_general.c
-ms2pip/cython_modules/ms2pip_features_c_old.c
-ms2pip/cython_modules/ms2pip_init_c.c
-ms2pip/cython_modules/ms2pip_peaks_c.c
-ms2pip/cython_modules/ms2pip_pyx.pyx
-ms2pip/models/HCD-2019.h
-ms2pip/models/TMT.h
-ms2pip/models/HCD-2019/model_20190107_HCD_train_B.c
-ms2pip/models/HCD-2019/model_20190107_HCD_train_B2.c
-ms2pip/models/HCD-2019/model_20190107_HCD_train_Y.c
-ms2pip/models/HCD-2019/model_20190107_HCD_train_Y2.c
-ms2pip/models/TMT/model_20190107_TMT_train_B.c
-ms2pip/models/TMT/model_20190107_TMT_train_Y.c
-ms2pip/ms2pip_tools/__init__.py
-ms2pip/ms2pip_tools/calc_correlations.py
-ms2pip/ms2pip_tools/dlib.py
-ms2pip/ms2pip_tools/get_elude_predictions.py
-ms2pip/ms2pip_tools/spectrum_output.py
+ms2pip/_cython_modules/__init__.py
+ms2pip/_cython_modules/ms2pip_features_c.c
+ms2pip/_cython_modules/ms2pip_init_c.c
+ms2pip/_cython_modules/ms2pip_peaks_c.c
+ms2pip/_cython_modules/ms2pip_pyx.pyx
+ms2pip/_models_c/HCD-2019.h
+ms2pip/_models_c/TMT.h
+ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_B.c
+ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_B2.c
+ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_Y.c
+ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_Y2.c
+ms2pip/_models_c/TMT/model_20190107_TMT_train_B.c
+ms2pip/_models_c/TMT/model_20190107_TMT_train_Y.c
+ms2pip/_utils/cli.py
+ms2pip/_utils/dlib.py
+ms2pip/_utils/encoder.py
+ms2pip/_utils/feature_names.py
+ms2pip/_utils/psm_input.py
+ms2pip/_utils/retention_time.py
+ms2pip/_utils/xgb_models.py
+tests/test_fasta2speclib.py
+tests/test_features.py
+tests/test_modifications.py
+tests/test_predictions.py
+tests/test_retention_time.py
+tests/test_spectrum_output.py
```

