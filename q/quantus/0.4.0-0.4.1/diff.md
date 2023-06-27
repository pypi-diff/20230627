# Comparing `tmp/quantus-0.4.0.tar.gz` & `tmp/quantus-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantus-0.4.0.tar", last modified: Tue May  9 20:55:45 2023, max compression
+gzip compressed data, was "quantus-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quantus-0.4.0.tar` & `quantus-0.4.1.tar`

### file list

```diff
@@ -1,121 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.864278 quantus-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 20:55:32.000000 quantus-0.4.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-05-09 20:55:32.000000 quantus-0.4.0/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-09 20:55:32.000000 quantus-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-09 20:55:32.000000 quantus-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    30180 2023-05-09 20:55:45.864278 quantus-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    29516 2023-05-09 20:55:32.000000 quantus-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.852278 quantus-0.4.0/quantus/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.852278 quantus-0.4.0/quantus/functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/functions/discretise_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    32857 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/functions/explanation_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/functions/loss_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/functions/mosaic_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/functions/norm_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/functions/normalise_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    16936 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/functions/perturb_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/functions/similarity_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.852278 quantus-0.4.0/quantus/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/asserts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.852278 quantus-0.4.0/quantus/helpers/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/model/model_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/model/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/model/pytorch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16081 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/model/tf_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    32190 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/helpers/warn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.856279 quantus-0.4.0/quantus/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.856279 quantus-0.4.0/quantus/metrics/axiomatic/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/axiomatic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/axiomatic/completeness.py
--rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/axiomatic/input_invariance.py
--rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/axiomatic/non_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    33179 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20113 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/base_batched.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.856279 quantus-0.4.0/quantus/metrics/complexity/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/complexity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/complexity/complexity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/complexity/effective_complexity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/complexity/sparseness.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.856279 quantus-0.4.0/quantus/metrics/faithfulness/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15554 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/faithfulness_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/faithfulness_estimate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16959 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/infidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/irof.py
--rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/monotonicity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/monotonicity_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/pixel_flipping.py
--rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/region_perturbation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15473 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/road.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/selectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/sensitivity_n.py
--rw-r--r--   0 runner    (1001) docker     (123)    13951 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/faithfulness/sufficiency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.860278 quantus-0.4.0/quantus/metrics/localisation/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/localisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/localisation/attribution_localisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/localisation/auc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16014 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/localisation/focus.py
--rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/localisation/pointing_game.py
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/localisation/relevance_mass_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/localisation/relevance_rank_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/localisation/top_k_intersection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.860278 quantus-0.4.0/quantus/metrics/randomisation/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/randomisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17093 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/randomisation/model_parameter_randomisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/randomisation/random_logit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.860278 quantus-0.4.0/quantus/metrics/robustness/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/robustness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17232 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/robustness/avg_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/robustness/consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)    18914 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/robustness/continuity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/robustness/local_lipschitz_estimate.py
--rw-r--r--   0 runner    (1001) docker     (123)    17219 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/robustness/max_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    14250 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/robustness/relative_input_stability.py
--rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/robustness/relative_output_stability.py
--rw-r--r--   0 runner    (1001) docker     (123)    15810 2023-05-09 20:55:32.000000 quantus-0.4.0/quantus/metrics/robustness/relative_representation_stability.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.852278 quantus-0.4.0/quantus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30180 2023-05-09 20:55:45.000000 quantus-0.4.0/quantus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-09 20:55:45.000000 quantus-0.4.0/quantus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:55:45.000000 quantus-0.4.0/quantus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:55:45.000000 quantus-0.4.0/quantus.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-09 20:55:45.000000 quantus-0.4.0/quantus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 20:55:45.000000 quantus-0.4.0/quantus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-09 20:55:32.000000 quantus-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-09 20:55:32.000000 quantus-0.4.0/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 20:55:45.864278 quantus-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-09 20:55:32.000000 quantus-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.860278 quantus-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.860278 quantus-0.4.0/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34140 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_explanation_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_loss_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_mosaic_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_norm_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_normalise_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    12891 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_perturb_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_pytorch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_similarity_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_tf_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31385 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/helpers/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:45.864278 quantus-0.4.0/tests/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/metrics/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    21113 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/metrics/test_axiomatic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    16673 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/metrics/test_complexity_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    58855 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/metrics/test_faithfulness_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    53755 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/metrics/test_localisation_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    16183 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/metrics/test_randomisation_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/metrics/test_relative_stability.py
--rw-r--r--   0 runner    (1001) docker     (123)    30229 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/metrics/test_robustness_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-09 20:55:32.000000 quantus-0.4.0/tests/test_evaluation.py
+-rw-r--r--   0        0        0      386 2023-06-27 11:10:35.613694 quantus-0.4.1/LICENSE
+-rw-r--r--   0        0        0    29032 2023-06-27 11:10:35.617694 quantus-0.4.1/README.md
+-rw-r--r--   0        0        0     4189 2023-06-27 11:10:35.621694 quantus-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1175 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/__init__.py
+-rw-r--r--   0        0        0     6947 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/evaluation.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/functions/__init__.py
+-rw-r--r--   0        0        0     2823 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/functions/discretise_func.py
+-rw-r--r--   0        0        0    32857 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/functions/explanation_func.py
+-rw-r--r--   0        0        0     1711 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/functions/loss_func.py
+-rw-r--r--   0        0        0     6569 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/functions/mosaic_func.py
+-rw-r--r--   0        0        0     1923 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/functions/norm_func.py
+-rw-r--r--   0        0        0     8308 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/functions/normalise_func.py
+-rw-r--r--   0        0        0    16936 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/functions/perturb_func.py
+-rw-r--r--   0        0        0     7749 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/functions/similarity_func.py
+-rw-r--r--   0        0        0      965 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/helpers/__init__.py
+-rw-r--r--   0        0        0    11509 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/helpers/asserts.py
+-rw-r--r--   0        0        0     7165 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/helpers/constants.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/helpers/model/__init__.py
+-rw-r--r--   0        0        0     6250 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/helpers/model/model_interface.py
+-rw-r--r--   0        0        0     9772 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/helpers/model/models.py
+-rw-r--r--   0        0        0    14399 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/helpers/model/pytorch_model.py
+-rw-r--r--   0        0        0    16081 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/helpers/model/tf_model.py
+-rw-r--r--   0        0        0     9065 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/helpers/plotting.py
+-rw-r--r--   0        0        0    32190 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/helpers/utils.py
+-rw-r--r--   0        0        0     8662 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/helpers/warn.py
+-rw-r--r--   0        0        0     1034 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/metrics/__init__.py
+-rw-r--r--   0        0        0      951 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/metrics/axiomatic/__init__.py
+-rw-r--r--   0        0        0    12961 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/metrics/axiomatic/completeness.py
+-rw-r--r--   0        0        0    13611 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/metrics/axiomatic/input_invariance.py
+-rw-r--r--   0        0        0    14407 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/metrics/axiomatic/non_sensitivity.py
+-rw-r--r--   0        0        0    33179 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/metrics/base.py
+-rw-r--r--   0        0        0    20113 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/metrics/base_batched.py
+-rw-r--r--   0        0        0      949 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/metrics/complexity/__init__.py
+-rw-r--r--   0        0        0    10644 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/metrics/complexity/complexity.py
+-rw-r--r--   0        0        0    10425 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/metrics/complexity/effective_complexity.py
+-rw-r--r--   0        0        0    10997 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/metrics/complexity/sparseness.py
+-rw-r--r--   0        0        0     1609 2023-06-27 11:10:35.621694 quantus-0.4.1/quantus/metrics/faithfulness/__init__.py
+-rw-r--r--   0        0        0    15554 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/faithfulness/faithfulness_correlation.py
+-rw-r--r--   0        0        0    14825 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/faithfulness/faithfulness_estimate.py
+-rw-r--r--   0        0        0    16959 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/faithfulness/infidelity.py
+-rw-r--r--   0        0        0    15253 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/faithfulness/irof.py
+-rw-r--r--   0        0        0    14512 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/faithfulness/monotonicity.py
+-rw-r--r--   0        0        0    15378 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/faithfulness/monotonicity_correlation.py
+-rw-r--r--   0        0        0    14532 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/faithfulness/pixel_flipping.py
+-rw-r--r--   0        0        0    17103 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/faithfulness/region_perturbation.py
+-rw-r--r--   0        0        0    15472 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/faithfulness/road.py
+-rw-r--r--   0        0        0    15534 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/faithfulness/selectivity.py
+-rw-r--r--   0        0        0    17555 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/faithfulness/sensitivity_n.py
+-rw-r--r--   0        0        0    13951 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/faithfulness/sufficiency.py
+-rw-r--r--   0        0        0     2015 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/localisation/__init__.py
+-rw-r--r--   0        0        0    13006 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/localisation/attribution_localisation.py
+-rw-r--r--   0        0        0    11721 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/localisation/auc.py
+-rw-r--r--   0        0        0    16014 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/localisation/focus.py
+-rw-r--r--   0        0        0    12342 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/localisation/pointing_game.py
+-rw-r--r--   0        0        0    11992 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/localisation/relevance_mass_accuracy.py
+-rw-r--r--   0        0        0    12336 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/localisation/relevance_rank_accuracy.py
+-rw-r--r--   0        0        0    12803 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/localisation/top_k_intersection.py
+-rw-r--r--   0        0        0      923 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/randomisation/__init__.py
+-rw-r--r--   0        0        0    17093 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/randomisation/model_parameter_randomisation.py
+-rw-r--r--   0        0        0    12775 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/randomisation/random_logit.py
+-rw-r--r--   0        0        0      641 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/robustness/__init__.py
+-rw-r--r--   0        0        0    17232 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/robustness/avg_sensitivity.py
+-rw-r--r--   0        0        0    13230 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/robustness/consistency.py
+-rw-r--r--   0        0        0    18914 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/robustness/continuity.py
+-rw-r--r--   0        0        0    17878 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/robustness/local_lipschitz_estimate.py
+-rw-r--r--   0        0        0    17219 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/robustness/max_sensitivity.py
+-rw-r--r--   0        0        0    14250 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/robustness/relative_input_stability.py
+-rw-r--r--   0        0        0    14548 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/robustness/relative_output_stability.py
+-rw-r--r--   0        0        0    15810 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/metrics/robustness/relative_representation_stability.py
+-rw-r--r--   0        0        0       64 2023-06-27 11:10:35.625694 quantus-0.4.1/quantus/py.typed
+-rw-r--r--   0        0        0    34016 1970-01-01 00:00:00.000000 quantus-0.4.1/PKG-INFO
```

### Comparing `quantus-0.4.0/PKG-INFO` & `quantus-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: quantus
-Version: 0.4.0
-Summary: A toolkit to evaluate neural network explanations.
-Home-page: http://github.com/understandable-machine-intelligence-lab/Quantus
-Author: Anna Hedstrom
-Author-email: hedstroem.anna@gmail.com
-License: GNU LESSER GENERAL PUBLIC LICENSE VERSION 3
-Keywords: explainable ai,xai,machine learning,deep learning
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: torch
-Provides-Extra: tensorflow
-Provides-Extra: captum
-Provides-Extra: tf-explain
-Provides-Extra: zennit
-Provides-Extra: tests
-Provides-Extra: full
-License-File: LICENSE
-License-File: COPYING
-License-File: COPYING.LESSER
-
 <p align="center">
   <img width="350" src="https://raw.githubusercontent.com/understandable-machine-intelligence-lab/Quantus/main/quantus_logo.png">
 </p>
 <!--<h1 align="center"><b>Quantus</b></h1>-->
 <h3 align="center"><b>A toolkit to evaluate neural network explanations</b></h3>
 <p align="center">
   PyTorch and TensorFlow
@@ -41,15 +19,15 @@
 
 _Quantus is currently under active development so carefully note the Quantus release version to ensure reproducibility of your work._
 
 [📑 Shortcut to paper!](https://jmlr.org/papers/volume24/22-0142/22-0142.pdf)
         
 ## News and Highlights! :rocket:
 
-- Released a new version 0.4.0 that now supports Python 3.10 and 3.11, read more [here](https://github.com/understandable-machine-intelligence-lab/Quantus/releases)!
+- Released a new version v0.4.1 [here](https://github.com/understandable-machine-intelligence-lab/Quantus/releases)!
 - Accepted to Journal of Machine Learning Research (MLOSS), read the [paper](https://jmlr.org/papers/v24/22-0142.html)
 - Offers more than **30+ metrics in 6 categories** for XAI evaluation
 - Supports different data types (image, time-series, tabular, NLP next up!) and models (PyTorch, TensorFlow)
 - Extended built-in support for explanation methods ([captum](https://captum.ai/) and [tf-explain](https://tf-explain.readthedocs.io/en/latest/))
 - New optimisations to help speed up computation, see API reference [here](https://quantus.readthedocs.io/en/latest/docs_api/quantus.metrics.base_batched.html)
 
 See [here](https://github.com/understandable-machine-intelligence-lab/Quantus/releases) for the latest release(s).
@@ -202,32 +180,26 @@
 
 For TensorFlow, please run:
 
 ```setup
 pip install "quantus[tensorflow]"
 ```
 
-Alternatively, you can simply install Quantus with [requirements.txt](https://github.com/understandable-machine-intelligence-lab/Quantus/blob/main/requirements.txt).
-Note that this installation requires that either [PyTorch](https://pytorch.org/) or [TensorFlow](https://www.TensorFlow.org) are already installed on your machine.
-
-```setup
-pip install -r requirements.txt
-```
-
-For a more in-depth guide on how to install Quantus, please read more [here](https://quantus.readthedocs.io/en/latest/getting_started/installation.html). This includes instructions for how to install a desired deep learning framework such as PyTorch or TensorFlow together with Quantus.
-
 ### Package requirements
 
 The package requirements are as follows:
 ```
 python>=3.7.0
 torch>=1.11.0
 tensorflow>=2.5.0
 ```
-Please note that the exact [PyTorch](https://pytorch.org/) and/ or [TensorFlow](https://www.TensorFlow.org) versions to be installed depends on your Python version (3.7-3.11) and platform (`darwin`, `linux`, …). See `requirements_test.txt` to retrieve the exact versions of [PyTorch](https://pytorch.org/) and/ or [TensorFlow](https://www.TensorFlow.org).
+
+Please note that the exact [PyTorch](https://pytorch.org/) and/ or [TensorFlow](https://www.TensorFlow.org) versions
+to be installed depends on your Python version (3.7-3.11) and platform (`darwin`, `linux`, …).
+See `[project.optional-dependencies]` section in the `pyproject.toml` file.
 
 ## Getting started
 
 The following will give a short introduction to how to get started with Quantus. Note that this example is based on the [PyTorch](https://pytorch.org/) framework, but we also support 
 [TensorFlow](https://www.tensorflow.org), which would differ only in the loading of the model, data and explanations. To get started with Quantus, you need:
 * A model (`model`), inputs (`x_batch`) and labels (`y_batch`)
 * Some explanations you want to evaluate (`a_batch`)
@@ -253,15 +225,15 @@
 model = LeNet()
 if device.type == "cpu":
     model.load_state_dict(torch.load("tests/assets/mnist", map_location=torch.device('cpu')))
 else: 
     model.load_state_dict(torch.load("tests/assets/mnist"))
 
 # Load datasets and make loaders.
-test_set = torchvision.datasets.MNIST(root='./sample_data', download=True, transforms=transforms.Compose([transforms.ToTensor()]))
+test_set = torchvision.datasets.MNIST(root='./sample_data', download=True, transform=transforms.Compose([transforms.ToTensor()]))
 test_loader = torch.utils.data.DataLoader(test_set, batch_size=24)
 
 # Load a batch of inputs and outputs to use for XAI evaluation.
 x_batch, y_batch = iter(test_loader).next()
 x_batch, y_batch = x_batch.cpu().numpy(), y_batch.cpu().numpy()
 ```
 </details>
@@ -284,15 +256,15 @@
 already pre-computed.
 
 In that case, you can simply load these into corresponding variables `a_batch_saliency` 
 and `a_batch_intgrad`:
 
 ```python
 a_batch_saliency = load("path/to/precomputed/saliency/explanations")
-a_batch_saliency = load("path/to/precomputed/intgrad/explanations")
+a_batch_intgrad = load("path/to/precomputed/intgrad/explanations")
 ```
 
 Another option is to simply obtain the attributions using one of many XAI frameworks out there, 
 such as [Captum](https://captum.ai/), 
 [Zennit](https://github.com/chr5tphr/zennit), 
 [tf.explain](https://github.com/sicara/tf-explain),
 or [iNNvestigate](https://github.com/albermax/innvestigate). The following code example shows how to obtain explanations ([Saliency](https://arxiv.org/abs/1312.6034) 
@@ -340,44 +312,36 @@
 
 ```python
 metric = quantus.MaxSensitivity(nr_samples=10,
                                 lower_bound=0.2,
                                 norm_numerator=quantus.fro_norm,
                                 norm_denominator=quantus.fro_norm,
                                 perturb_func=quantus.uniform_noise,
-                                similarity_func=quantus.difference)
+                                similarity_func=quantus.difference,
+                                abs=True,
+                                normalise=True)
 ```
 
 and then applied to your model, data, and (pre-computed) explanations:
 
 ```python
 scores = metric(
     model=model,
     x_batch=x_batch,
     y_batch=y_batch,
     a_batch=a_batch_saliency,
-    device=device
+    device=device,
+    explain_func=quantus.explain,
+    explain_func_kwargs={"method": "Saliency"},
 )
 ```
 
 #### Use quantus.explain
 
-Alternatively, instead of providing pre-computed explanations, you can employ the `quantus.explain` function,
-which can be specified through a dictionary passed to `explain_func_kwargs`.
-
-```python
-scores = metric(
-    model=model,
-    x_batch=x_batch,
-    y_batch=y_batch,
-    device=device,
-    explain_func=quantus.explain,
-    explain_func_kwargs={"method": "Saliency"}
-)
-```
+Since a re-computation of the explanations is necessary for robustness evaluation, in this example, we also pass an explanation function (`explain_func`) to the metric call. Here, we rely on the built-in `quantus.explain` function to recompute the explanations. The hyperparameters are set with the `explain_func_kwargs` dictionary. Please find more details on how to use  `quantus.explain` at [API documentation](https://quantus.readthedocs.io/en/latest/docs_api/quantus.functions.explanation_func.html).
 
 #### Employ customised functions
 
 You can alternatively use your own customised explanation function
 (assuming it returns an `np.ndarray` in a shape that matches the input `x_batch`). This is done as follows:
 
 ```python
```

### Comparing `quantus-0.4.0/README.md` & `quantus-0.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,83 @@
+Metadata-Version: 2.1
+Name: quantus
+Version: 0.4.1
+Summary: A metrics toolkit to evaluate neural network explanations.
+Keywords: explainable ai,xai,machine learning,deep learning
+Author-email: Anna Hedstrom <hedstroem.anna@gmail.com>
+Maintainer-email: Anna Hedstrom <hedstroem.anna@gmail.com>
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Dist: numpy>=1.19.5
+Requires-Dist: opencv-python>=4.5.5.62
+Requires-Dist: scikit-image>=0.19.3
+Requires-Dist: scikit-learn>=0.24.2
+Requires-Dist: scipy>=1.7.3
+Requires-Dist: tqdm>=4.62.3
+Requires-Dist: matplotlib>=3.3.4
+Requires-Dist: quantus[torch] ; extra == "captum"
+Requires-Dist: captum>=0.6.0 ; extra == "captum"
+Requires-Dist: quantus[captum,tf_explain,zennit] ; extra == "full"
+Requires-Dist: tensorflow>=2.5.0 ; extra == "tensorflow" and ( python_version == '3.7')
+Requires-Dist: tensorflow>=2.12.0 ; extra == "tensorflow" and ( sys_platform != 'darwin' and python_version > '3.7')
+Requires-Dist: tensorflow_macos>=2.12.0 ; extra == "tensorflow" and ( sys_platform == 'darwin' and python_version > '3.7')
+Requires-Dist: captum>=0.6.0 ; extra == "tests"
+Requires-Dist: coverage>=7.2.3 ; extra == "tests"
+Requires-Dist: flake8<=4.0.1 ; extra == "tests" and ( python_version == '3.7')
+Requires-Dist: flake8>=6.0.0 ; extra == "tests" and ( python_version > '3.7')
+Requires-Dist: pandas<=1.3.3 ; extra == "tests" and ( python_version == '3.7')
+Requires-Dist: pandas>=2.0.1 ; extra == "tests" and ( python_version > '3.7')
+Requires-Dist: pytest>=7.3.1 ; extra == "tests"
+Requires-Dist: pytest-cov>=4.0.0 ; extra == "tests"
+Requires-Dist: pytest-lazy-fixture>=0.6.3 ; extra == "tests"
+Requires-Dist: pytest-mock==3.10.0 ; extra == "tests"
+Requires-Dist: pytest_xdist ; extra == "tests"
+Requires-Dist: tf-explain>=0.3.1 ; extra == "tests"
+Requires-Dist: zennit>=0.4.5 ; extra == "tests" and ( python_version >= '3.7')
+Requires-Dist: tensorflow>=2.5.0 ; extra == "tests" and ( python_version == '3.7')
+Requires-Dist: tensorflow>=2.12.0 ; extra == "tests" and ( sys_platform != 'darwin' and python_version > '3.7')
+Requires-Dist: tensorflow_macos>=2.9.0 ; extra == "tests" and ( sys_platform == 'darwin' and python_version > '3.7')
+Requires-Dist: torch<=1.9.0 ; extra == "tests" and ( python_version == '3.7')
+Requires-Dist: torch>=1.13.1 ; extra == "tests" and ( sys_platform != 'linux' and python_version > '3.7')
+Requires-Dist: torch>=1.13.1, <2.0.0 ; extra == "tests" and ( sys_platform == 'linux' and python_version > '3.7' and python_version <= '3.10')
+Requires-Dist: torch>=2.0.0 ; extra == "tests" and ( sys_platform == 'linux' and python_version >= '3.11')
+Requires-Dist: torchvision<=0.12.0 ; extra == "tests" and ( python_version == '3.7')
+Requires-Dist: torchvision>=0.15.1 ; extra == "tests" and ( sys_platform != 'linux' and python_version > '3.7')
+Requires-Dist: torchvision>=0.14.0, <0.15.1 ; extra == "tests" and ( sys_platform == 'linux' and python_version > '3.7' and python_version <= '3.10')
+Requires-Dist: torchvision>=0.15.1 ; extra == "tests" and ( sys_platform == 'linux' and python_version >= '3.11')
+Requires-Dist: quantus[tensorflow] ; extra == "tf_explain"
+Requires-Dist: tf-explain>=0.3.1 ; extra == "tf_explain"
+Requires-Dist: torch<=1.11.0 ; extra == "torch" and ( python_version == '3.7')
+Requires-Dist: torch>=1.13.1 ; extra == "torch" and ( sys_platform != 'linux' and python_version > '3.7')
+Requires-Dist: torch>=1.13.1, <2.0.0 ; extra == "torch" and ( sys_platform == 'linux' and python_version > '3.7' and python_version <= '3.10')
+Requires-Dist: torch>=2.0.0 ; extra == "torch" and ( sys_platform == 'linux' and python_version >= '3.11')
+Requires-Dist: torchvision<=0.12.0 ; extra == "torch" and ( python_version == '3.7')
+Requires-Dist: torchvision>=0.15.1 ; extra == "torch" and ( sys_platform != 'linux' and python_version > '3.7')
+Requires-Dist: torchvision>=0.14.0, <0.15.1 ; extra == "torch" and ( sys_platform == 'linux' and python_version > '3.7' and python_version <= '3.10')
+Requires-Dist: torchvision>=0.15.1 ; extra == "torch" and ( sys_platform == 'linux' and python_version >= '3.11')
+Requires-Dist: quantus[torch] ; extra == "zennit"
+Requires-Dist: zennit>=0.5.1 ; extra == "zennit"
+Project-URL: Documentation, https://quantus.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/understandable-machine-intelligence-lab/Quantus
+Provides-Extra: captum
+Provides-Extra: full
+Provides-Extra: tensorflow
+Provides-Extra: tests
+Provides-Extra: tf_explain
+Provides-Extra: torch
+Provides-Extra: zennit
+
 <p align="center">
   <img width="350" src="https://raw.githubusercontent.com/understandable-machine-intelligence-lab/Quantus/main/quantus_logo.png">
 </p>
 <!--<h1 align="center"><b>Quantus</b></h1>-->
 <h3 align="center"><b>A toolkit to evaluate neural network explanations</b></h3>
 <p align="center">
   PyTorch and TensorFlow
@@ -19,15 +95,15 @@
 
 _Quantus is currently under active development so carefully note the Quantus release version to ensure reproducibility of your work._
 
 [📑 Shortcut to paper!](https://jmlr.org/papers/volume24/22-0142/22-0142.pdf)
         
 ## News and Highlights! :rocket:
 
-- Released a new version 0.4.0 that now supports Python 3.10 and 3.11, read more [here](https://github.com/understandable-machine-intelligence-lab/Quantus/releases)!
+- Released a new version v0.4.1 [here](https://github.com/understandable-machine-intelligence-lab/Quantus/releases)!
 - Accepted to Journal of Machine Learning Research (MLOSS), read the [paper](https://jmlr.org/papers/v24/22-0142.html)
 - Offers more than **30+ metrics in 6 categories** for XAI evaluation
 - Supports different data types (image, time-series, tabular, NLP next up!) and models (PyTorch, TensorFlow)
 - Extended built-in support for explanation methods ([captum](https://captum.ai/) and [tf-explain](https://tf-explain.readthedocs.io/en/latest/))
 - New optimisations to help speed up computation, see API reference [here](https://quantus.readthedocs.io/en/latest/docs_api/quantus.metrics.base_batched.html)
 
 See [here](https://github.com/understandable-machine-intelligence-lab/Quantus/releases) for the latest release(s).
@@ -180,32 +256,26 @@
 
 For TensorFlow, please run:
 
 ```setup
 pip install "quantus[tensorflow]"
 ```
 
-Alternatively, you can simply install Quantus with [requirements.txt](https://github.com/understandable-machine-intelligence-lab/Quantus/blob/main/requirements.txt).
-Note that this installation requires that either [PyTorch](https://pytorch.org/) or [TensorFlow](https://www.TensorFlow.org) are already installed on your machine.
-
-```setup
-pip install -r requirements.txt
-```
-
-For a more in-depth guide on how to install Quantus, please read more [here](https://quantus.readthedocs.io/en/latest/getting_started/installation.html). This includes instructions for how to install a desired deep learning framework such as PyTorch or TensorFlow together with Quantus.
-
 ### Package requirements
 
 The package requirements are as follows:
 ```
 python>=3.7.0
 torch>=1.11.0
 tensorflow>=2.5.0
 ```
-Please note that the exact [PyTorch](https://pytorch.org/) and/ or [TensorFlow](https://www.TensorFlow.org) versions to be installed depends on your Python version (3.7-3.11) and platform (`darwin`, `linux`, …). See `requirements_test.txt` to retrieve the exact versions of [PyTorch](https://pytorch.org/) and/ or [TensorFlow](https://www.TensorFlow.org).
+
+Please note that the exact [PyTorch](https://pytorch.org/) and/ or [TensorFlow](https://www.TensorFlow.org) versions
+to be installed depends on your Python version (3.7-3.11) and platform (`darwin`, `linux`, …).
+See `[project.optional-dependencies]` section in the `pyproject.toml` file.
 
 ## Getting started
 
 The following will give a short introduction to how to get started with Quantus. Note that this example is based on the [PyTorch](https://pytorch.org/) framework, but we also support 
 [TensorFlow](https://www.tensorflow.org), which would differ only in the loading of the model, data and explanations. To get started with Quantus, you need:
 * A model (`model`), inputs (`x_batch`) and labels (`y_batch`)
 * Some explanations you want to evaluate (`a_batch`)
@@ -231,15 +301,15 @@
 model = LeNet()
 if device.type == "cpu":
     model.load_state_dict(torch.load("tests/assets/mnist", map_location=torch.device('cpu')))
 else: 
     model.load_state_dict(torch.load("tests/assets/mnist"))
 
 # Load datasets and make loaders.
-test_set = torchvision.datasets.MNIST(root='./sample_data', download=True, transforms=transforms.Compose([transforms.ToTensor()]))
+test_set = torchvision.datasets.MNIST(root='./sample_data', download=True, transform=transforms.Compose([transforms.ToTensor()]))
 test_loader = torch.utils.data.DataLoader(test_set, batch_size=24)
 
 # Load a batch of inputs and outputs to use for XAI evaluation.
 x_batch, y_batch = iter(test_loader).next()
 x_batch, y_batch = x_batch.cpu().numpy(), y_batch.cpu().numpy()
 ```
 </details>
@@ -262,15 +332,15 @@
 already pre-computed.
 
 In that case, you can simply load these into corresponding variables `a_batch_saliency` 
 and `a_batch_intgrad`:
 
 ```python
 a_batch_saliency = load("path/to/precomputed/saliency/explanations")
-a_batch_saliency = load("path/to/precomputed/intgrad/explanations")
+a_batch_intgrad = load("path/to/precomputed/intgrad/explanations")
 ```
 
 Another option is to simply obtain the attributions using one of many XAI frameworks out there, 
 such as [Captum](https://captum.ai/), 
 [Zennit](https://github.com/chr5tphr/zennit), 
 [tf.explain](https://github.com/sicara/tf-explain),
 or [iNNvestigate](https://github.com/albermax/innvestigate). The following code example shows how to obtain explanations ([Saliency](https://arxiv.org/abs/1312.6034) 
@@ -318,44 +388,36 @@
 
 ```python
 metric = quantus.MaxSensitivity(nr_samples=10,
                                 lower_bound=0.2,
                                 norm_numerator=quantus.fro_norm,
                                 norm_denominator=quantus.fro_norm,
                                 perturb_func=quantus.uniform_noise,
-                                similarity_func=quantus.difference)
+                                similarity_func=quantus.difference,
+                                abs=True,
+                                normalise=True)
 ```
 
 and then applied to your model, data, and (pre-computed) explanations:
 
 ```python
 scores = metric(
     model=model,
     x_batch=x_batch,
     y_batch=y_batch,
     a_batch=a_batch_saliency,
-    device=device
+    device=device,
+    explain_func=quantus.explain,
+    explain_func_kwargs={"method": "Saliency"},
 )
 ```
 
 #### Use quantus.explain
 
-Alternatively, instead of providing pre-computed explanations, you can employ the `quantus.explain` function,
-which can be specified through a dictionary passed to `explain_func_kwargs`.
-
-```python
-scores = metric(
-    model=model,
-    x_batch=x_batch,
-    y_batch=y_batch,
-    device=device,
-    explain_func=quantus.explain,
-    explain_func_kwargs={"method": "Saliency"}
-)
-```
+Since a re-computation of the explanations is necessary for robustness evaluation, in this example, we also pass an explanation function (`explain_func`) to the metric call. Here, we rely on the built-in `quantus.explain` function to recompute the explanations. The hyperparameters are set with the `explain_func_kwargs` dictionary. Please find more details on how to use  `quantus.explain` at [API documentation](https://quantus.readthedocs.io/en/latest/docs_api/quantus.functions.explanation_func.html).
 
 #### Employ customised functions
 
 You can alternatively use your own customised explanation function
 (assuming it returns an `np.ndarray` in a shape that matches the input `x_batch`). This is done as follows:
 
 ```python
@@ -430,7 +492,8 @@
 
 ## Contributing
 
 We welcome any sort of contribution to Quantus! For a detailed contribution guide, please refer to [Contributing](https://github.com/understandable-machine-intelligence-lab/Quantus/blob/main/CONTRIBUTING.md) documentation first. 
 
 If you have any developer-related questions, please [open an issue](https://github.com/understandable-machine-intelligence-lab/Quantus/issues/new/choose)
 or write us at [hedstroem.anna@gmail.com](mailto:hedstroem.anna@gmail.com).
+
```

### Comparing `quantus-0.4.0/quantus/__init__.py` & `quantus-0.4.1/quantus/__init__.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/evaluation.py` & `quantus-0.4.1/quantus/evaluation.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/functions/discretise_func.py` & `quantus-0.4.1/quantus/functions/discretise_func.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/functions/explanation_func.py` & `quantus-0.4.1/quantus/functions/explanation_func.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/functions/loss_func.py` & `quantus-0.4.1/quantus/functions/loss_func.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/functions/mosaic_func.py` & `quantus-0.4.1/quantus/functions/mosaic_func.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/functions/norm_func.py` & `quantus-0.4.1/quantus/functions/norm_func.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/functions/normalise_func.py` & `quantus-0.4.1/quantus/functions/normalise_func.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/functions/perturb_func.py` & `quantus-0.4.1/quantus/functions/perturb_func.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/functions/similarity_func.py` & `quantus-0.4.1/quantus/functions/similarity_func.py`

 * *Files 5% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         return float(abs(a - b) / (d2(c, d) + eps))
     else:
         return float(d1(a, b) / (d2(a=c, b=d) + eps))
 
 
 def abs_difference(a: np.array, b: np.array, **kwargs) -> float:
     """
-    Calculate the absolute difference between two images (or explanations).
+    Calculate the mean of the absolute differences between two images (or explanations).
 
     Parameters
     ----------
     a: np.ndarray
          The first array to use for similarity scoring.
     b: np.ndarray
          The second array to use for similarity scoring.
@@ -198,14 +198,35 @@
     -------
     float
         The similarity score.
     """
     return np.mean(abs(a - b))
 
 
+def squared_difference(a: np.array, b: np.array, **kwargs) -> float:
+    """
+    Calculate the sqaured differences between two images (or explanations).
+
+    Parameters
+    ----------
+    a: np.ndarray
+         The first array to use for similarity scoring.
+    b: np.ndarray
+         The second array to use for similarity scoring.
+    kwargs: optional
+        Keyword arguments.
+
+    Returns
+    -------
+    float
+        The similarity score.
+    """
+    return np.sum((a - b) ** 2)
+
+
 def cosine(a: np.array, b: np.array, **kwargs) -> float:
     """
     Calculate Cosine of two images (or explanations).
 
     Parameters
     ----------
     a: np.ndarray
@@ -246,26 +267,26 @@
     )
     data_range = float(np.abs(max_point - min_point))
     return skimage.metrics.structural_similarity(
         im1=a, im2=b, win_size=kwargs.get("win_size", None), data_range=data_range
     )
 
 
-def difference(a: np.array, b: np.array, **kwargs) -> float:
+def difference(a: np.array, b: np.array, **kwargs) -> np.array:
     """
     Calculate the difference between two images (or explanations).
 
     Parameters
     ----------
     a: np.ndarray
          The first array to use for similarity scoring.
     b: np.ndarray
          The second array to use for similarity scoring.
     kwargs: optional
         Keyword arguments.
 
     Returns
     -------
-    float
-        The similarity score.
+    np.array
+        The difference in each element.
     """
     return a - b
```

### Comparing `quantus-0.4.0/quantus/helpers/__init__.py` & `quantus-0.4.1/quantus/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/helpers/asserts.py` & `quantus-0.4.1/quantus/helpers/asserts.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     Returns
     -------
     None
     """
     assert order in [
         "random",
         "morf",
-        "lorf",
+        "lerf",
     ], "The order of sorting the attributions must be either random, morf, or lorf."
 
 
 def assert_nr_segments(nr_segments: int) -> None:
     """
     Assert that the number of segments given the segmentation algorithm is more than one.
```

### Comparing `quantus-0.4.0/quantus/helpers/constants.py` & `quantus-0.4.1/quantus/helpers/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,15 @@
     "correlation_pearson": correlation_pearson,
     "correlation_kendall_tau": correlation_kendall_tau,
     "distance_euclidean": distance_euclidean,
     "distance_manhattan": distance_manhattan,
     "distance_chebyshev": distance_chebyshev,
     "lipschitz_constant": lipschitz_constant,
     "abs_difference": abs_difference,
+    "squared_difference": squared_difference,
     "difference": difference,
     "cosine": cosine,
     "ssim": ssim,
     "mse": mse,
 }
 
 AVAILABLE_NORMALISATION_FUNCTIONS = {
```

### Comparing `quantus-0.4.0/quantus/helpers/model/model_interface.py` & `quantus-0.4.1/quantus/helpers/model/model_interface.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/helpers/model/models.py` & `quantus-0.4.1/quantus/helpers/model/models.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/helpers/model/pytorch_model.py` & `quantus-0.4.1/quantus/helpers/model/pytorch_model.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/helpers/model/tf_model.py` & `quantus-0.4.1/quantus/helpers/model/tf_model.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/helpers/plotting.py` & `quantus-0.4.1/quantus/helpers/plotting.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/helpers/utils.py` & `quantus-0.4.1/quantus/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/helpers/warn.py` & `quantus-0.4.1/quantus/helpers/warn.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/__init__.py` & `quantus-0.4.1/quantus/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/axiomatic/__init__.py` & `quantus-0.4.1/quantus/metrics/axiomatic/__init__.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/axiomatic/completeness.py` & `quantus-0.4.1/quantus/metrics/axiomatic/completeness.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/axiomatic/input_invariance.py` & `quantus-0.4.1/quantus/metrics/axiomatic/input_invariance.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/axiomatic/non_sensitivity.py` & `quantus-0.4.1/quantus/metrics/axiomatic/non_sensitivity.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/base.py` & `quantus-0.4.1/quantus/metrics/base.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/base_batched.py` & `quantus-0.4.1/quantus/metrics/base_batched.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/complexity/__init__.py` & `quantus-0.4.1/quantus/metrics/complexity/__init__.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/complexity/complexity.py` & `quantus-0.4.1/quantus/metrics/complexity/complexity.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/complexity/effective_complexity.py` & `quantus-0.4.1/quantus/metrics/complexity/effective_complexity.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/complexity/sparseness.py` & `quantus-0.4.1/quantus/metrics/complexity/sparseness.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/faithfulness/__init__.py` & `quantus-0.4.1/quantus/metrics/faithfulness/__init__.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/faithfulness/faithfulness_correlation.py` & `quantus-0.4.1/quantus/metrics/faithfulness/faithfulness_correlation.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/faithfulness/faithfulness_estimate.py` & `quantus-0.4.1/quantus/metrics/faithfulness/faithfulness_estimate.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/faithfulness/infidelity.py` & `quantus-0.4.1/quantus/metrics/faithfulness/infidelity.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/faithfulness/irof.py` & `quantus-0.4.1/quantus/metrics/faithfulness/irof.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/faithfulness/monotonicity.py` & `quantus-0.4.1/quantus/metrics/faithfulness/monotonicity.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/faithfulness/monotonicity_correlation.py` & `quantus-0.4.1/quantus/metrics/faithfulness/monotonicity_correlation.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/faithfulness/pixel_flipping.py` & `quantus-0.4.1/quantus/metrics/faithfulness/pixel_flipping.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/faithfulness/region_perturbation.py` & `quantus-0.4.1/quantus/metrics/faithfulness/region_perturbation.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/faithfulness/road.py` & `quantus-0.4.1/quantus/metrics/faithfulness/road.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,12 +360,11 @@
 
         Returns
         -------
         None
         """
 
         # Calculate accuracy for every number of most important pixels removed.
-
         self.last_results = {
             percentage: np.mean(np.array(self.last_results)[:, p_ix])
             for p_ix, percentage in enumerate(self.percentages)
         }
```

### Comparing `quantus-0.4.0/quantus/metrics/faithfulness/selectivity.py` & `quantus-0.4.1/quantus/metrics/faithfulness/selectivity.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/faithfulness/sensitivity_n.py` & `quantus-0.4.1/quantus/metrics/faithfulness/sensitivity_n.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/faithfulness/sufficiency.py` & `quantus-0.4.1/quantus/metrics/faithfulness/sufficiency.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/localisation/__init__.py` & `quantus-0.4.1/quantus/metrics/localisation/__init__.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/localisation/attribution_localisation.py` & `quantus-0.4.1/quantus/metrics/localisation/attribution_localisation.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/localisation/auc.py` & `quantus-0.4.1/quantus/metrics/localisation/auc.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/localisation/focus.py` & `quantus-0.4.1/quantus/metrics/localisation/focus.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/localisation/pointing_game.py` & `quantus-0.4.1/quantus/metrics/localisation/pointing_game.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/localisation/relevance_mass_accuracy.py` & `quantus-0.4.1/quantus/metrics/localisation/relevance_mass_accuracy.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/localisation/relevance_rank_accuracy.py` & `quantus-0.4.1/quantus/metrics/localisation/relevance_rank_accuracy.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/localisation/top_k_intersection.py` & `quantus-0.4.1/quantus/metrics/localisation/top_k_intersection.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/randomisation/__init__.py` & `quantus-0.4.1/quantus/metrics/randomisation/__init__.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/randomisation/model_parameter_randomisation.py` & `quantus-0.4.1/quantus/metrics/randomisation/model_parameter_randomisation.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/randomisation/random_logit.py` & `quantus-0.4.1/quantus/metrics/randomisation/random_logit.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/robustness/__init__.py` & `quantus-0.4.1/quantus/metrics/robustness/__init__.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/robustness/avg_sensitivity.py` & `quantus-0.4.1/quantus/metrics/robustness/avg_sensitivity.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/robustness/consistency.py` & `quantus-0.4.1/quantus/metrics/robustness/consistency.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/robustness/continuity.py` & `quantus-0.4.1/quantus/metrics/robustness/continuity.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/robustness/local_lipschitz_estimate.py` & `quantus-0.4.1/quantus/metrics/robustness/local_lipschitz_estimate.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/robustness/max_sensitivity.py` & `quantus-0.4.1/quantus/metrics/robustness/max_sensitivity.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/robustness/relative_input_stability.py` & `quantus-0.4.1/quantus/metrics/robustness/relative_input_stability.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/robustness/relative_output_stability.py` & `quantus-0.4.1/quantus/metrics/robustness/relative_output_stability.py`

 * *Files identical despite different names*

### Comparing `quantus-0.4.0/quantus/metrics/robustness/relative_representation_stability.py` & `quantus-0.4.1/quantus/metrics/robustness/relative_representation_stability.py`

 * *Files identical despite different names*

