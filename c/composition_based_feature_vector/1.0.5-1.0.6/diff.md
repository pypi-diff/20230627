# Comparing `tmp/composition_based_feature_vector-1.0.5.tar.gz` & `tmp/composition_based_feature_vector-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composition_based_feature_vector-1.0.5.tar", last modified: Wed Nov 30 15:03:04 2022, max compression
+gzip compressed data, was "composition_based_feature_vector-1.0.6.tar", last modified: Tue Jun 27 00:06:18 2023, max compression
```

## Comparing `composition_based_feature_vector-1.0.5.tar` & `composition_based_feature_vector-1.0.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1331 2022-02-04 05:50:29.075208 composition_based_feature_vector-1.0.5/.github/workflows/cbfv_test_workflow.yml
--rw-r--r--   0        0        0     2022 2022-11-30 15:00:48.247368 composition_based_feature_vector-1.0.5/.gitignore
--rw-r--r--   0        0        0     1100 2022-11-30 15:00:48.251366 composition_based_feature_vector-1.0.5/LICENSE
--rw-r--r--   0        0        0     2455 2022-11-30 15:00:48.251366 composition_based_feature_vector-1.0.5/README.md
--rw-r--r--   0        0        0      172 2022-11-30 15:02:46.223655 composition_based_feature_vector-1.0.5/composition_based_feature_vector/__init__.py
--rw-r--r--   0        0        0    11737 2022-11-30 15:00:48.260367 composition_based_feature_vector-1.0.5/composition_based_feature_vector/composition.py
--rw-r--r--   0        0        0   400588 2022-11-30 15:00:48.265366 composition_based_feature_vector-1.0.5/composition_based_feature_vector/element_properties/jarvis.csv
--rw-r--r--   0        0        0    11013 2022-11-30 15:00:48.265366 composition_based_feature_vector-1.0.5/composition_based_feature_vector/element_properties/magpie.csv
--rw-r--r--   0        0        0   477010 2022-11-30 15:00:48.270366 composition_based_feature_vector-1.0.5/composition_based_feature_vector/element_properties/mat2vec.csv
--rw-r--r--   0        0        0    15385 2022-11-30 15:00:48.271369 composition_based_feature_vector-1.0.5/composition_based_feature_vector/element_properties/oliynyk.csv
--rw-r--r--   0        0        0    29638 2022-11-30 15:00:48.271369 composition_based_feature_vector-1.0.5/composition_based_feature_vector/element_properties/onehot.csv
--rw-r--r--   0        0        0   322952 2022-11-30 15:00:48.275368 composition_based_feature_vector-1.0.5/composition_based_feature_vector/element_properties/random_200.csv
--rw-r--r--   0        0        0      954 2022-11-30 15:00:48.278366 composition_based_feature_vector-1.0.5/composition_based_feature_vector/meta.yaml
--rw-r--r--   0        0        0     4830 2022-11-30 15:00:48.279368 composition_based_feature_vector-1.0.5/composition_based_feature_vector/tests/test.py
--rw-r--r--   0        0        0      519 2022-11-30 15:00:48.279368 composition_based_feature_vector-1.0.5/composition_based_feature_vector/tests/test_composition.py
--rw-r--r--   0        0        0    89734 2022-02-04 05:50:29.084964 composition_based_feature_vector-1.0.5/data/Egap/test.csv
--rw-r--r--   0        0        0   306863 2022-02-04 05:50:29.095121 composition_based_feature_vector-1.0.5/data/Egap/train.csv
--rw-r--r--   0        0        0    51135 2022-02-04 05:50:29.095121 composition_based_feature_vector-1.0.5/data/Egap/val.csv
--rw-r--r--   0        0        0    18532 2022-02-04 05:50:29.095121 composition_based_feature_vector-1.0.5/data/ael_bulk_modulus_vrh/test.csv
--rw-r--r--   0        0        0    62488 2022-02-04 05:50:29.095121 composition_based_feature_vector-1.0.5/data/ael_bulk_modulus_vrh/train.csv
--rw-r--r--   0        0        0    10504 2022-02-04 05:50:29.095121 composition_based_feature_vector-1.0.5/data/ael_bulk_modulus_vrh/val.csv
--rw-r--r--   0        0        0    21145 2022-02-04 05:50:29.095121 composition_based_feature_vector-1.0.5/data/ael_log10_debye_temperature/test.csv
--rw-r--r--   0        0        0    72685 2022-02-04 05:50:29.095121 composition_based_feature_vector-1.0.5/data/ael_log10_debye_temperature/train.csv
--rw-r--r--   0        0        0    12087 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.5/data/ael_log10_debye_temperature/val.csv
--rw-r--r--   0        0        0    17632 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.5/data/ael_shear_modulus_vrh/test.csv
--rw-r--r--   0        0        0    60398 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.5/data/ael_shear_modulus_vrh/train.csv
--rw-r--r--   0        0        0    10160 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.5/data/ael_shear_modulus_vrh/val.csv
--rw-r--r--   0        0        0    21608 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.5/data/agl_log10_thermal_conductivity_300K/test.csv
--rw-r--r--   0        0        0    74726 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.5/data/agl_log10_thermal_conductivity_300K/train.csv
--rw-r--r--   0        0        0    12415 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.5/data/agl_log10_thermal_conductivity_300K/val.csv
--rw-r--r--   0        0        0    21622 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.5/data/agl_log10_thermal_expansion_300K/test.csv
--rw-r--r--   0        0        0    76907 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.5/data/agl_log10_thermal_expansion_300K/train.csv
--rw-r--r--   0        0        0    15361 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.5/data/agl_log10_thermal_expansion_300K/val.csv
--rw-r--r--   0        0        0   123047 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.5/data/energy_atom/test.csv
--rw-r--r--   0        0        0   422071 2022-02-04 05:50:29.114975 composition_based_feature_vector-1.0.5/data/energy_atom/train.csv
--rw-r--r--   0        0        0    70849 2022-02-04 05:50:29.114975 composition_based_feature_vector-1.0.5/data/energy_atom/val.csv
--rw-r--r--   0        0        0      416 2022-02-04 05:50:29.114975 composition_based_feature_vector-1.0.5/data/process_data.py
--rw-r--r--   0        0        0     2732 2022-02-04 05:50:29.114975 composition_based_feature_vector-1.0.5/example_code.py
--rw-r--r--   0        0        0     1140 2022-02-04 05:50:29.114975 composition_based_feature_vector-1.0.5/featurize_file.py
--rw-r--r--   0        0        0  9212201 2022-02-04 05:50:29.163553 composition_based_feature_vector-1.0.5/featurized_data/X.csv
--rw-r--r--   0        0        0    20386 2022-02-04 05:50:29.164516 composition_based_feature_vector-1.0.5/predictions.csv
--rw-r--r--   0        0        0     1289 2022-11-30 15:00:48.280369 composition_based_feature_vector-1.0.5/pyproject.toml
--rw-r--r--   0        0        0       50 2022-11-30 15:00:48.284367 composition_based_feature_vector-1.0.5/requirements.txt
--rw-r--r--   0        0        0      734 2022-11-30 15:00:48.287366 composition_based_feature_vector-1.0.5/run_grayskull.py
--rw-r--r--   0        0        0    90761 2022-02-04 05:50:29.168520 composition_based_feature_vector-1.0.5/test_data_extended_feats.csv
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 composition_based_feature_vector-1.0.5/setup.py
--rw-r--r--   0        0        0     3496 1970-01-01 00:00:00.000000 composition_based_feature_vector-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1331 2022-02-04 05:50:29.075208 composition_based_feature_vector-1.0.6/.github/workflows/cbfv_test_workflow.yml
+-rw-r--r--   0        0        0     2022 2022-11-30 15:00:48.247368 composition_based_feature_vector-1.0.6/.gitignore
+-rw-r--r--   0        0        0     1100 2022-11-30 15:00:48.251366 composition_based_feature_vector-1.0.6/LICENSE
+-rw-r--r--   0        0        0     2455 2022-11-30 15:00:48.251366 composition_based_feature_vector-1.0.6/README.md
+-rw-r--r--   0        0        0      172 2023-06-27 00:04:27.129205 composition_based_feature_vector-1.0.6/composition_based_feature_vector/__init__.py
+-rw-r--r--   0        0        0    11737 2022-11-30 15:00:48.260367 composition_based_feature_vector-1.0.6/composition_based_feature_vector/composition.py
+-rw-r--r--   0        0        0   400588 2022-11-30 15:00:48.265366 composition_based_feature_vector-1.0.6/composition_based_feature_vector/element_properties/jarvis.csv
+-rw-r--r--   0        0        0    11013 2022-11-30 15:00:48.265366 composition_based_feature_vector-1.0.6/composition_based_feature_vector/element_properties/magpie.csv
+-rw-r--r--   0        0        0   477010 2022-11-30 15:00:48.270366 composition_based_feature_vector-1.0.6/composition_based_feature_vector/element_properties/mat2vec.csv
+-rw-r--r--   0        0        0    15385 2022-11-30 15:00:48.271369 composition_based_feature_vector-1.0.6/composition_based_feature_vector/element_properties/oliynyk.csv
+-rw-r--r--   0        0        0    29638 2022-11-30 15:00:48.271369 composition_based_feature_vector-1.0.6/composition_based_feature_vector/element_properties/onehot.csv
+-rw-r--r--   0        0        0   322952 2022-11-30 15:00:48.275368 composition_based_feature_vector-1.0.6/composition_based_feature_vector/element_properties/random_200.csv
+-rw-r--r--   0        0        0      954 2022-11-30 15:00:48.278366 composition_based_feature_vector-1.0.6/composition_based_feature_vector/meta.yaml
+-rw-r--r--   0        0        0     4830 2022-11-30 15:00:48.279368 composition_based_feature_vector-1.0.6/composition_based_feature_vector/tests/test.py
+-rw-r--r--   0        0        0      519 2022-11-30 15:00:48.279368 composition_based_feature_vector-1.0.6/composition_based_feature_vector/tests/test_composition.py
+-rw-r--r--   0        0        0    89734 2022-02-04 05:50:29.084964 composition_based_feature_vector-1.0.6/data/Egap/test.csv
+-rw-r--r--   0        0        0   306863 2022-02-04 05:50:29.095121 composition_based_feature_vector-1.0.6/data/Egap/train.csv
+-rw-r--r--   0        0        0    51135 2022-02-04 05:50:29.095121 composition_based_feature_vector-1.0.6/data/Egap/val.csv
+-rw-r--r--   0        0        0    18532 2022-02-04 05:50:29.095121 composition_based_feature_vector-1.0.6/data/ael_bulk_modulus_vrh/test.csv
+-rw-r--r--   0        0        0    62488 2022-02-04 05:50:29.095121 composition_based_feature_vector-1.0.6/data/ael_bulk_modulus_vrh/train.csv
+-rw-r--r--   0        0        0    10504 2022-02-04 05:50:29.095121 composition_based_feature_vector-1.0.6/data/ael_bulk_modulus_vrh/val.csv
+-rw-r--r--   0        0        0    21145 2022-02-04 05:50:29.095121 composition_based_feature_vector-1.0.6/data/ael_log10_debye_temperature/test.csv
+-rw-r--r--   0        0        0    72685 2022-02-04 05:50:29.095121 composition_based_feature_vector-1.0.6/data/ael_log10_debye_temperature/train.csv
+-rw-r--r--   0        0        0    12087 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.6/data/ael_log10_debye_temperature/val.csv
+-rw-r--r--   0        0        0    17632 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.6/data/ael_shear_modulus_vrh/test.csv
+-rw-r--r--   0        0        0    60398 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.6/data/ael_shear_modulus_vrh/train.csv
+-rw-r--r--   0        0        0    10160 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.6/data/ael_shear_modulus_vrh/val.csv
+-rw-r--r--   0        0        0    21608 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.6/data/agl_log10_thermal_conductivity_300K/test.csv
+-rw-r--r--   0        0        0    74726 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.6/data/agl_log10_thermal_conductivity_300K/train.csv
+-rw-r--r--   0        0        0    12415 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.6/data/agl_log10_thermal_conductivity_300K/val.csv
+-rw-r--r--   0        0        0    21622 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.6/data/agl_log10_thermal_expansion_300K/test.csv
+-rw-r--r--   0        0        0    76907 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.6/data/agl_log10_thermal_expansion_300K/train.csv
+-rw-r--r--   0        0        0    15361 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.6/data/agl_log10_thermal_expansion_300K/val.csv
+-rw-r--r--   0        0        0   123047 2022-02-04 05:50:29.104852 composition_based_feature_vector-1.0.6/data/energy_atom/test.csv
+-rw-r--r--   0        0        0   422071 2022-02-04 05:50:29.114975 composition_based_feature_vector-1.0.6/data/energy_atom/train.csv
+-rw-r--r--   0        0        0    70849 2022-02-04 05:50:29.114975 composition_based_feature_vector-1.0.6/data/energy_atom/val.csv
+-rw-r--r--   0        0        0      416 2022-02-04 05:50:29.114975 composition_based_feature_vector-1.0.6/data/process_data.py
+-rw-r--r--   0        0        0     2732 2022-02-04 05:50:29.114975 composition_based_feature_vector-1.0.6/example_code.py
+-rw-r--r--   0        0        0     1140 2022-02-04 05:50:29.114975 composition_based_feature_vector-1.0.6/featurize_file.py
+-rw-r--r--   0        0        0  9212201 2022-02-04 05:50:29.163553 composition_based_feature_vector-1.0.6/featurized_data/X.csv
+-rw-r--r--   0        0        0    20386 2022-02-04 05:50:29.164516 composition_based_feature_vector-1.0.6/predictions.csv
+-rw-r--r--   0        0        0     1384 2023-06-27 00:04:23.478170 composition_based_feature_vector-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0       50 2022-11-30 15:00:48.284367 composition_based_feature_vector-1.0.6/requirements.txt
+-rw-r--r--   0        0        0      734 2022-11-30 15:00:48.287366 composition_based_feature_vector-1.0.6/run_grayskull.py
+-rw-r--r--   0        0        0    90761 2022-02-04 05:50:29.168520 composition_based_feature_vector-1.0.6/test_data_extended_feats.csv
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 composition_based_feature_vector-1.0.6/setup.py
+-rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 composition_based_feature_vector-1.0.6/PKG-INFO
```

### Comparing `composition_based_feature_vector-1.0.5/.github/workflows/cbfv_test_workflow.yml` & `composition_based_feature_vector-1.0.6/.github/workflows/cbfv_test_workflow.yml`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/.gitignore` & `composition_based_feature_vector-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/LICENSE` & `composition_based_feature_vector-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/README.md` & `composition_based_feature_vector-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/composition_based_feature_vector/composition.py` & `composition_based_feature_vector-1.0.6/composition_based_feature_vector/composition.py`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/composition_based_feature_vector/element_properties/jarvis.csv` & `composition_based_feature_vector-1.0.6/composition_based_feature_vector/element_properties/jarvis.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/composition_based_feature_vector/element_properties/magpie.csv` & `composition_based_feature_vector-1.0.6/composition_based_feature_vector/element_properties/magpie.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/composition_based_feature_vector/element_properties/mat2vec.csv` & `composition_based_feature_vector-1.0.6/composition_based_feature_vector/element_properties/mat2vec.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/composition_based_feature_vector/element_properties/oliynyk.csv` & `composition_based_feature_vector-1.0.6/composition_based_feature_vector/element_properties/oliynyk.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/composition_based_feature_vector/element_properties/onehot.csv` & `composition_based_feature_vector-1.0.6/composition_based_feature_vector/element_properties/onehot.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/composition_based_feature_vector/element_properties/random_200.csv` & `composition_based_feature_vector-1.0.6/composition_based_feature_vector/element_properties/random_200.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/composition_based_feature_vector/meta.yaml` & `composition_based_feature_vector-1.0.6/composition_based_feature_vector/meta.yaml`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/composition_based_feature_vector/tests/test.py` & `composition_based_feature_vector-1.0.6/composition_based_feature_vector/tests/test.py`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/composition_based_feature_vector/tests/test_composition.py` & `composition_based_feature_vector-1.0.6/composition_based_feature_vector/tests/test_composition.py`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/Egap/test.csv` & `composition_based_feature_vector-1.0.6/data/Egap/test.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/Egap/train.csv` & `composition_based_feature_vector-1.0.6/data/Egap/train.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/Egap/val.csv` & `composition_based_feature_vector-1.0.6/data/Egap/val.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/ael_bulk_modulus_vrh/test.csv` & `composition_based_feature_vector-1.0.6/data/ael_bulk_modulus_vrh/test.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/ael_bulk_modulus_vrh/train.csv` & `composition_based_feature_vector-1.0.6/data/ael_bulk_modulus_vrh/train.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/ael_bulk_modulus_vrh/val.csv` & `composition_based_feature_vector-1.0.6/data/ael_bulk_modulus_vrh/val.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/ael_log10_debye_temperature/test.csv` & `composition_based_feature_vector-1.0.6/data/ael_log10_debye_temperature/test.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/ael_log10_debye_temperature/train.csv` & `composition_based_feature_vector-1.0.6/data/ael_log10_debye_temperature/train.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/ael_log10_debye_temperature/val.csv` & `composition_based_feature_vector-1.0.6/data/ael_log10_debye_temperature/val.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/ael_shear_modulus_vrh/test.csv` & `composition_based_feature_vector-1.0.6/data/ael_shear_modulus_vrh/test.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/ael_shear_modulus_vrh/train.csv` & `composition_based_feature_vector-1.0.6/data/ael_shear_modulus_vrh/train.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/ael_shear_modulus_vrh/val.csv` & `composition_based_feature_vector-1.0.6/data/ael_shear_modulus_vrh/val.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/agl_log10_thermal_conductivity_300K/test.csv` & `composition_based_feature_vector-1.0.6/data/agl_log10_thermal_conductivity_300K/test.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/agl_log10_thermal_conductivity_300K/train.csv` & `composition_based_feature_vector-1.0.6/data/agl_log10_thermal_conductivity_300K/train.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/agl_log10_thermal_conductivity_300K/val.csv` & `composition_based_feature_vector-1.0.6/data/agl_log10_thermal_conductivity_300K/val.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/agl_log10_thermal_expansion_300K/test.csv` & `composition_based_feature_vector-1.0.6/data/agl_log10_thermal_expansion_300K/test.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/agl_log10_thermal_expansion_300K/train.csv` & `composition_based_feature_vector-1.0.6/data/agl_log10_thermal_expansion_300K/train.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/agl_log10_thermal_expansion_300K/val.csv` & `composition_based_feature_vector-1.0.6/data/agl_log10_thermal_expansion_300K/val.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/energy_atom/test.csv` & `composition_based_feature_vector-1.0.6/data/energy_atom/test.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/energy_atom/train.csv` & `composition_based_feature_vector-1.0.6/data/energy_atom/train.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/data/energy_atom/val.csv` & `composition_based_feature_vector-1.0.6/data/energy_atom/val.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/example_code.py` & `composition_based_feature_vector-1.0.6/example_code.py`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/featurize_file.py` & `composition_based_feature_vector-1.0.6/featurize_file.py`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/featurized_data/X.csv` & `composition_based_feature_vector-1.0.6/featurized_data/X.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/predictions.csv` & `composition_based_feature_vector-1.0.6/predictions.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/pyproject.toml` & `composition_based_feature_vector-1.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -21,61 +21,67 @@
 00000140: 616d 653d 2253 7465 726c 696e 6720 472e  ame="Sterling G.
 00000150: 2042 6169 7264 222c 2065 6d61 696c 3d22   Baird", email="
 00000160: 7374 6572 6c69 6e67 2e62 6169 7264 4075  sterling.baird@u
 00000170: 7461 682e 6564 7522 7d0d 0a20 2020 205d  tah.edu"}..    ]
 00000180: 0d0a 7265 6164 6d65 203d 2022 5245 4144  ..readme = "READ
 00000190: 4d45 2e6d 6422 0d0a 0d0a 7265 7175 6972  ME.md"....requir
 000001a0: 6573 2d70 7974 686f 6e20 3d20 223e 3d33  es-python = ">=3
-000001b0: 2c3c 332e 3130 220d 0a0d 0a64 6570 656e  ,<3.10"....depen
-000001c0: 6465 6e63 6965 733d 5b0d 0a20 2020 2020  dencies=[..     
-000001d0: 2020 2020 2020 2020 2020 2022 6e75 6d70             "nump
-000001e0: 7922 2c0d 0a20 2020 2020 2020 2020 2020  y",..           
-000001f0: 2020 2020 2022 7061 6e64 6173 222c 0d0a       "pandas",..
-00000200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000210: 2274 7164 6d22 2c0d 0a20 2020 2020 2020  "tqdm",..       
-00000220: 2020 2020 2020 2020 2022 7079 7465 7374           "pytest
-00000230: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000240: 5d0d 0a0d 0a63 6c61 7373 6966 6965 7273  ]....classifiers
-00000250: 203d 205b 0d0a 2020 2020 2020 2020 224c   = [..        "L
-00000260: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-00000270: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
-00000280: 6365 6e73 6522 2c0d 0a20 2020 2020 2020  cense",..       
-00000290: 2022 4465 7665 6c6f 706d 656e 7420 5374   "Development St
-000002a0: 6174 7573 203a 3a20 3320 2d20 416c 7068  atus :: 3 - Alph
-000002b0: 6122 2c0d 0a20 2020 2020 2020 2022 496e  a",..        "In
-000002c0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
-000002d0: 3a3a 2053 6369 656e 6365 2f52 6573 6561  :: Science/Resea
-000002e0: 7263 6822 2c0d 0a20 2020 2020 2020 2022  rch",..        "
-000002f0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000300: 203a 3a20 504f 5349 5820 3a3a 204c 696e   :: POSIX :: Lin
-00000310: 7578 222c 0d0a 2020 2020 2020 2020 224f  ux",..        "O
-00000320: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000330: 3a3a 204d 6163 4f53 222c 0d0a 2020 2020  :: MacOS",..    
-00000340: 2020 2020 224f 7065 7261 7469 6e67 2053      "Operating S
-00000350: 7973 7465 6d20 3a3a 204d 6963 726f 736f  ystem :: Microso
-00000360: 6674 203a 3a20 5769 6e64 6f77 7322 2c0d  ft :: Windows",.
-00000370: 0a20 2020 2020 2020 2022 5072 6f67 7261  .        "Progra
-00000380: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000390: 3a20 5079 7468 6f6e 203a 3a20 3322 2c0d  : Python :: 3",.
-000003a0: 0a20 2020 2020 2020 2022 5072 6f67 7261  .        "Progra
-000003b0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000003c0: 3a20 5079 7468 6f6e 203a 3a20 332e 3422  : Python :: 3.4"
-000003d0: 2c0d 0a20 2020 2020 2020 2022 5072 6f67  ,..        "Prog
-000003e0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000003f0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000400: 3522 2c0d 0a20 2020 2020 2020 2022 5072  5",..        "Pr
-00000410: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000420: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000430: 332e 3622 2c0d 0a20 2020 2020 2020 2022  3.6",..        "
-00000440: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000450: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000460: 3a20 332e 3722 2c0d 0a20 2020 2020 2020  : 3.7",..       
-00000470: 2022 5072 6f67 7261 6d6d 696e 6720 4c61   "Programming La
-00000480: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000490: 203a 3a20 332e 3822 2c0d 0a20 2020 205d   :: 3.8",..    ]
-000004a0: 0d0a 6479 6e61 6d69 6320 3d20 5b22 7665  ..dynamic = ["ve
-000004b0: 7273 696f 6e22 2c20 2264 6573 6372 6970  rsion", "descrip
-000004c0: 7469 6f6e 225d 0d0a 0d0a 5b70 726f 6a65  tion"]....[proje
-000004d0: 6374 2e75 726c 735d 0d0a 486f 6d65 203d  ct.urls]..Home =
-000004e0: 2022 6874 7470 733a 2f2f 6769 7468 7562   "https://github
-000004f0: 2e63 6f6d 2f73 7061 726b 732d 6261 6972  .com/sparks-bair
-00000500: 642f 4342 4656 220d 0a                   d/CBFV"..
+000001b0: 220d 0a0d 0a64 6570 656e 6465 6e63 6965  "....dependencie
+000001c0: 733d 5b0d 0a20 2020 2020 2020 2020 2020  s=[..           
+000001d0: 2020 2020 2022 6e75 6d70 7922 2c0d 0a20       "numpy",.. 
+000001e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000001f0: 7061 6e64 6173 222c 0d0a 2020 2020 2020  pandas",..      
+00000200: 2020 2020 2020 2020 2020 2274 7164 6d22            "tqdm"
+00000210: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000220: 2020 2022 7079 7465 7374 222c 0d0a 2020     "pytest",..  
+00000230: 2020 2020 2020 2020 2020 5d0d 0a0d 0a63            ]....c
+00000240: 6c61 7373 6966 6965 7273 203d 205b 0d0a  lassifiers = [..
+00000250: 2020 2020 2020 2020 224c 6963 656e 7365          "License
+00000260: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+00000270: 203a 3a20 4d49 5420 4c69 6365 6e73 6522   :: MIT License"
+00000280: 2c0d 0a20 2020 2020 2020 2022 4465 7665  ,..        "Deve
+00000290: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
+000002a0: 3a20 3320 2d20 416c 7068 6122 2c0d 0a20  : 3 - Alpha",.. 
+000002b0: 2020 2020 2020 2022 496e 7465 6e64 6564         "Intended
+000002c0: 2041 7564 6965 6e63 6520 3a3a 2053 6369   Audience :: Sci
+000002d0: 656e 6365 2f52 6573 6561 7263 6822 2c0d  ence/Research",.
+000002e0: 0a20 2020 2020 2020 2022 4f70 6572 6174  .        "Operat
+000002f0: 696e 6720 5379 7374 656d 203a 3a20 504f  ing System :: PO
+00000300: 5349 5820 3a3a 204c 696e 7578 222c 0d0a  SIX :: Linux",..
+00000310: 2020 2020 2020 2020 224f 7065 7261 7469          "Operati
+00000320: 6e67 2053 7973 7465 6d20 3a3a 204d 6163  ng System :: Mac
+00000330: 4f53 222c 0d0a 2020 2020 2020 2020 224f  OS",..        "O
+00000340: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000350: 3a3a 204d 6963 726f 736f 6674 203a 3a20  :: Microsoft :: 
+00000360: 5769 6e64 6f77 7322 2c0d 0a20 2020 2020  Windows",..     
+00000370: 2020 2022 5072 6f67 7261 6d6d 696e 6720     "Programming 
+00000380: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000390: 6f6e 203a 3a20 3322 2c0d 0a20 2020 2020  on :: 3",..     
+000003a0: 2020 2022 5072 6f67 7261 6d6d 696e 6720     "Programming 
+000003b0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000003c0: 6f6e 203a 3a20 332e 3422 2c0d 0a20 2020  on :: 3.4",..   
+000003d0: 2020 2020 2022 5072 6f67 7261 6d6d 696e       "Programmin
+000003e0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000003f0: 7468 6f6e 203a 3a20 332e 3522 2c0d 0a20  thon :: 3.5",.. 
+00000400: 2020 2020 2020 2022 5072 6f67 7261 6d6d         "Programm
+00000410: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000420: 5079 7468 6f6e 203a 3a20 332e 3622 2c0d  Python :: 3.6",.
+00000430: 0a20 2020 2020 2020 2022 5072 6f67 7261  .        "Progra
+00000440: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000450: 3a20 5079 7468 6f6e 203a 3a20 332e 3722  : Python :: 3.7"
+00000460: 2c0d 0a20 2020 2020 2020 2022 5072 6f67  ,..        "Prog
+00000470: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000480: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000490: 3822 2c0d 0a20 2020 2020 2020 2022 5072  8",..        "Pr
+000004a0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000004b0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000004c0: 332e 3922 2c0d 0a20 2020 2020 2020 2022  3.9",..        "
+000004d0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000004e0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000004f0: 3a20 332e 3130 222c 0d0a 2020 2020 5d0d  : 3.10",..    ].
+00000500: 0a64 796e 616d 6963 203d 205b 2276 6572  .dynamic = ["ver
+00000510: 7369 6f6e 222c 2022 6465 7363 7269 7074  sion", "descript
+00000520: 696f 6e22 5d0d 0a0d 0a5b 7072 6f6a 6563  ion"]....[projec
+00000530: 742e 7572 6c73 5d0d 0a48 6f6d 6520 3d20  t.urls]..Home = 
+00000540: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000550: 636f 6d2f 7370 6172 6b73 2d62 6169 7264  com/sparks-baird
+00000560: 2f43 4246 5622 0d0a                      /CBFV"..
```

### Comparing `composition_based_feature_vector-1.0.5/run_grayskull.py` & `composition_based_feature_vector-1.0.6/run_grayskull.py`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/test_data_extended_feats.csv` & `composition_based_feature_vector-1.0.6/test_data_extended_feats.csv`

 * *Files identical despite different names*

### Comparing `composition_based_feature_vector-1.0.5/setup.py` & `composition_based_feature_vector-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 ['composition_based_feature_vector']
 
 package_data = \
 {'': ['*'],
  'composition_based_feature_vector': ['element_properties/*', 'tests/*']}
 
 setup(name='composition_based_feature_vector',
-      version='1.0.5',
+      version='1.0.6',
       description='Tool for quickly creating a composition-based feature vector.',
       author='Andrew Falkowski',
       author_email='Steven Kauwe <jkkauwe@gmail.com>, Anthony Wang <aytwang@alumni.uwaterloo.ca>, "Sterling G. Baird" <sterling.baird@utah.edu>',
       url=None,
       packages=packages,
       package_data=package_data,
-      python_requires='>=3,<3.10',
+      python_requires='>=3',
      )
```

### Comparing `composition_based_feature_vector-1.0.5/PKG-INFO` & `composition_based_feature_vector-1.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: composition_based_feature_vector
-Version: 1.0.5
+Version: 1.0.6
 Summary: Tool for quickly creating a composition-based feature vector.
 Author: Andrew Falkowski
 Author-email: Steven Kauwe <jkkauwe@gmail.com>, Anthony Wang <aytwang@alumni.uwaterloo.ca>, "Sterling G. Baird" <sterling.baird@utah.edu>
-Requires-Python: >=3,<3.10
+Requires-Python: >=3
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: tqdm
 Requires-Dist: pytest
 Project-URL: Home, https://github.com/sparks-baird/CBFV
 
 # CBFV Package
```

#### html2text {}

```diff
@@ -1,32 +1,33 @@
-Metadata-Version: 2.1 Name: composition_based_feature_vector Version: 1.0.5
+Metadata-Version: 2.1 Name: composition_based_feature_vector Version: 1.0.6
 Summary: Tool for quickly creating a composition-based feature vector. Author:
 Andrew Falkowski Author-email: Steven Kauwe
 gmail.com>, Anthony Wang
 alumni.uwaterloo.ca>, "Sterling G. Baird"
-baird@utah.edu> Requires-Python: >=3,<3.10 Description-Content-Type: text/
-markdown Classifier: License :: OSI Approved :: MIT License Classifier:
-Development Status :: 3 - Alpha Classifier: Intended Audience :: Science/
-Research Classifier: Operating System :: POSIX :: Linux Classifier: Operating
-System :: MacOS Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.4 Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: numpy Requires-Dist: pandas Requires-Dist: tqdm Requires-Dist:
-pytest Project-URL: Home, https://github.com/sparks-baird/CBFV # CBFV Package
-Tool to quickly create a composition-based feature vectors from materials
-datafiles. # Installation The source code is currently hosted on GitHub at:
-https://github.com/kaaiian/CBFV Binary installers for the latest released
-version are available at the Python_Package_Index_(PyPI) ``` # PyPI pip install
-CBFV ``` ## Making the composition-based feature vector The CBFV package
-assumes your data is stored in a pandas dataframe of the following structure:
-formula | target ---|--- Tc1V1 | 248.539 Cu1Dy1 | 66.8444 Cd3N2 | 91.5034 To
-featurize this data, the `generate_features` function can be called as follows:
-``` from CBFV import composition X, y, formulae, skipped =
+baird@utah.edu> Requires-Python: >=3 Description-Content-Type: text/markdown
+Classifier: License :: OSI Approved :: MIT License Classifier: Development
+Status :: 3 - Alpha Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: POSIX :: Linux Classifier: Operating System ::
+MacOS Classifier: Operating System :: Microsoft :: Windows Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.4 Classifier: Programming Language :: Python :: 3.5 Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Requires-Dist: numpy Requires-Dist: pandas Requires-Dist: tqdm
+Requires-Dist: pytest Project-URL: Home, https://github.com/sparks-baird/CBFV #
+CBFV Package Tool to quickly create a composition-based feature vectors from
+materials datafiles. # Installation The source code is currently hosted on
+GitHub at: https://github.com/kaaiian/CBFV Binary installers for the latest
+released version are available at the Python_Package_Index_(PyPI) ``` # PyPI
+pip install CBFV ``` ## Making the composition-based feature vector The CBFV
+package assumes your data is stored in a pandas dataframe of the following
+structure: formula | target ---|--- Tc1V1 | 248.539 Cu1Dy1 | 66.8444 Cd3N2 |
+91.5034 To featurize this data, the `generate_features` function can be called
+as follows: ``` from CBFV import composition X, y, formulae, skipped =
 composition.generate_features(df) ``` ## Extended Functionality The
 featurization scheme can be adjusted by calling the the `elem_prop` parameter.
 The following featurization schemes are included within CBFV: - jarvis - magpie
 - mat2vec - oliynyk (default) - onehot - random_200 Duplicate formula handeling
 is controlled by the `drop_duplicates` parameter. It is set to `False` by
 default to preserve datapoints containing variation outside of their formula.
 For example, heat capacity measurements performed for the same material at
```

