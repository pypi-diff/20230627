# Comparing `tmp/OpenFisca-France-Data-1.0.tar.gz` & `tmp/OpenFisca-France-Data-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFisca-France-Data-1.0.tar", last modified: Wed Jun 14 13:56:00 2023, max compression
+gzip compressed data, was "OpenFisca-France-Data-1.1.0.tar", last modified: Tue Jun 27 09:25:34 2023, max compression
```

## Comparing `OpenFisca-France-Data-1.0.tar` & `OpenFisca-France-Data-1.1.0.tar`

### file list

```diff
@@ -1,111 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.530484 OpenFisca-France-Data-1.0/
--rw-r--r--   0 runner    (1001) docker     (122)    10258 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.514484 OpenFisca-France-Data-1.0/OpenFisca_France_Data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11504 2023-06-14 13:56:00.000000 OpenFisca-France-Data-1.0/OpenFisca_France_Data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4160 2023-06-14 13:56:00.000000 OpenFisca-France-Data-1.0/OpenFisca_France_Data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 13:56:00.000000 OpenFisca-France-Data-1.0/OpenFisca_France_Data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      250 2023-06-14 13:56:00.000000 OpenFisca-France-Data-1.0/OpenFisca_France_Data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      373 2023-06-14 13:56:00.000000 OpenFisca-France-Data-1.0/OpenFisca_France_Data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-06-14 13:56:00.000000 OpenFisca-France-Data-1.0/OpenFisca_France_Data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    11504 2023-06-14 13:56:00.530484 OpenFisca-France-Data-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10702 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.514484 OpenFisca-France-Data-1.0/openfisca_france_data/
--rw-r--r--   0 runner    (1001) docker     (122)     7557 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2998 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/aggregates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.514484 OpenFisca-France-Data-1.0/openfisca_france_data/assets/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.514484 OpenFisca-France-Data-1.0/openfisca_france_data/assets/zone_apl_data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/assets/zone_apl_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/assets/zone_apl_data/codeAplReader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.514484 OpenFisca-France-Data-1.0/openfisca_france_data/assets/zone_apl_data/zone_apl/
--rw-r--r--   0 runner    (1001) docker     (122)      502 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/assets/zone_apl_data/zone_apl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1814 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/base_survey.py
--rw-r--r--   0 runner    (1001) docker     (122)    21046 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/common.py
--rw-r--r--   0 runner    (1001) docker     (122)    23221 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/comparator.py
--rw-r--r--   0 runner    (1001) docker     (122)      996 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.506484 OpenFisca-France-Data-1.0/openfisca_france_data/dads/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.518484 OpenFisca-France-Data-1.0/openfisca_france_data/dads/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/dads/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.518484 OpenFisca-France-Data-1.0/openfisca_france_data/erfs/
--rw-r--r--   0 runner    (1001) docker     (122)     1045 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.518484 OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2637 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/run_all.py
--rw-r--r--   0 runner    (1001) docker     (122)     8932 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py
--rw-r--r--   0 runner    (1001) docker     (122)    21783 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py
--rw-r--r--   0 runner    (1001) docker     (122)    11919 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py
--rw-r--r--   0 runner    (1001) docker     (122)    26165 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py
--rw-r--r--   0 runner    (1001) docker     (122)    13995 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py
--rw-r--r--   0 runner    (1001) docker     (122)    36615 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py
--rw-r--r--   0 runner    (1001) docker     (122)     8399 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py
--rw-r--r--   0 runner    (1001) docker     (122)    13216 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py
--rw-r--r--   0 runner    (1001) docker     (122)     1536 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.518484 OpenFisca-France-Data-1.0/openfisca_france_data/erfs/old/
--rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs/old/aggregates.py
--rw-r--r--   0 runner    (1001) docker     (122)    19211 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs/old/datatable.py
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs/scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.522484 OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4726 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/comparison.py
--rw-r--r--   0 runner    (1001) docker     (122)     7295 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.522484 OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (122)     6806 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15394 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (122)    25444 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py
--rw-r--r--   0 runner    (1001) docker     (122)    44658 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py
--rw-r--r--   0 runner    (1001) docker     (122)    35127 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_05_foyer.py
--rw-r--r--   0 runner    (1001) docker     (122)    11692 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py
--rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)     5791 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/test_case_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.510484 OpenFisca-France-Data-1.0/openfisca_france_data/felin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.522484 OpenFisca-France-Data-1.0/openfisca_france_data/felin/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/felin/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1869 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.522484 OpenFisca-France-Data-1.0/openfisca_france_data/model/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      541 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/model/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     8882 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/model/calage.py
--rw-r--r--   0 runner    (1001) docker     (122)    11373 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/model/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/model/id_variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/model/survey_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.526484 OpenFisca-France-Data-1.0/openfisca_france_data/reforms/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/reforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12440 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/reforms/inversion_directe_salaires.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.526484 OpenFisca-France-Data-1.0/openfisca_france_data/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/scripts/build_input_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     6701 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/smic.py
--rw-r--r--   0 runner    (1001) docker     (122)     7161 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/surveys.py
--rw-r--r--   0 runner    (1001) docker     (122)    15060 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/openfisca_france_data/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-06-14 13:56:00.530484 OpenFisca-France-Data-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.526484 OpenFisca-France-Data-1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.510484 OpenFisca-France-Data-1.0/tests/erfs_fpr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.530484 OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/
--rw-r--r--   0 runner    (1001) docker     (122)     2466 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_af.py
--rw-r--r--   0 runner    (1001) docker     (122)     8242 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_al.py
--rw-r--r--   0 runner    (1001) docker     (122)    10685 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_impot_revenu.py
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_inflation.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_input_variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_pivot_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_rebuild_input_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_rsa.py
--rw-r--r--   0 runner    (1001) docker     (122)     1532 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_salaire_imposable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 13:56:00.530484 OpenFisca-France-Data-1.0/tests/erfs_fpr/unit/
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/tests/erfs_fpr/unit/test_get_survey_scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)      215 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/tests/erfs_fpr/unit/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/tests/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)     7465 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/tests/test_fake_survey_simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/tests/test_get_baremes_salarie.py
--rw-r--r--   0 runner    (1001) docker     (122)      900 2023-06-14 13:55:34.000000 OpenFisca-France-Data-1.0/tests/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.033478 OpenFisca-France-Data-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    10500 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.025478 OpenFisca-France-Data-1.1.0/OpenFisca_France_Data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11506 2023-06-27 09:25:34.000000 OpenFisca-France-Data-1.1.0/OpenFisca_France_Data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4093 2023-06-27 09:25:34.000000 OpenFisca-France-Data-1.1.0/OpenFisca_France_Data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 09:25:34.000000 OpenFisca-France-Data-1.1.0/OpenFisca_France_Data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-06-27 09:25:34.000000 OpenFisca-France-Data-1.1.0/OpenFisca_France_Data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-06-27 09:25:34.000000 OpenFisca-France-Data-1.1.0/OpenFisca_France_Data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-06-27 09:25:34.000000 OpenFisca-France-Data-1.1.0/OpenFisca_France_Data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    11506 2023-06-27 09:25:34.033478 OpenFisca-France-Data-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10702 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.025478 OpenFisca-France-Data-1.1.0/openfisca_france_data/
+-rw-r--r--   0 runner    (1001) docker     (122)     7557 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2998 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/aggregates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.025478 OpenFisca-France-Data-1.1.0/openfisca_france_data/assets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.025478 OpenFisca-France-Data-1.1.0/openfisca_france_data/assets/zone_apl_data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/assets/zone_apl_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      334 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/assets/zone_apl_data/codeAplReader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.025478 OpenFisca-France-Data-1.1.0/openfisca_france_data/assets/zone_apl_data/zone_apl/
+-rw-r--r--   0 runner    (1001) docker     (122)      502 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/assets/zone_apl_data/zone_apl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1814 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/base_survey.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21046 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23221 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      996 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.021478 OpenFisca-France-Data-1.1.0/openfisca_france_data/dads/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.025478 OpenFisca-France-Data-1.1.0/openfisca_france_data/dads/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/dads/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.025478 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/
+-rw-r--r--   0 runner    (1001) docker     (122)     1045 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.029478 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2637 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/run_all.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8932 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21783 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11919 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26165 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13995 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36615 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8399 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13216 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1536 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.029478 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/old/
+-rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/old/aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19211 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/old/datatable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.029478 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4388 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7108 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.029478 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)     6660 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15394 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25444 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45059 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35127 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2286 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5791 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/test_case_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.021478 OpenFisca-France-Data-1.1.0/openfisca_france_data/felin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.029478 OpenFisca-France-Data-1.1.0/openfisca_france_data/felin/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/felin/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1869 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.029478 OpenFisca-France-Data-1.1.0/openfisca_france_data/model/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      541 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8882 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/model/calage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11373 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/model/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/model/id_variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/model/survey_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.029478 OpenFisca-France-Data-1.1.0/openfisca_france_data/reforms/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/reforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12440 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/reforms/inversion_directe_salaires.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.029478 OpenFisca-France-Data-1.1.0/openfisca_france_data/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/scripts/build_input_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6701 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/smic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7052 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/surveys.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15060 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/openfisca_france_data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-06-27 09:25:34.033478 OpenFisca-France-Data-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.033478 OpenFisca-France-Data-1.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.021478 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.033478 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)     2466 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_af.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8242 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_al.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10685 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_impot_revenu.py
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_input_variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_pivot_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_rebuild_input_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1532 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_salaire_imposable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 09:25:34.033478 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/unit/test_get_survey_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/erfs_fpr/unit/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7465 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/test_fake_survey_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/test_get_baremes_salarie.py
+-rw-r--r--   0 runner    (1001) docker     (122)      900 2023-06-27 09:25:12.000000 OpenFisca-France-Data-1.1.0/tests/test_misc.py
```

### Comparing `OpenFisca-France-Data-1.0/CHANGELOG.md` & `OpenFisca-France-Data-1.1.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+# 1.1.0 [#225](https://github.com/openfisca/openfisca-france-data/pull/225)
+
+
+* Technical changes
+- Ajoute des variables concernant le calcul des aides au logement, des non salariés et du handicap dans le builder de openfisca-france-data
+
+
+
 # 1.0.0 [#224](https://github.com/openfisca/openfisca-france-data/pull/224)
 
 * Breaking changes
 - dans model/common.py/salaire_brut:
   - Retire rev_microsocial
 
 - Détails
```

### Comparing `OpenFisca-France-Data-1.0/CONTRIBUTING.md` & `OpenFisca-France-Data-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/LICENSE` & `OpenFisca-France-Data-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/OpenFisca_France_Data.egg-info/PKG-INFO` & `OpenFisca-France-Data-1.1.0/OpenFisca_France_Data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-France-Data
-Version: 1.0
+Version: 1.1.0
 Summary: OpenFisca-France-Data module to work with French survey data
 Home-page: https://github.com/openfisca/openfisca-france-data
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit social survey data microsimulation
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-France-Data-1.0/OpenFisca_France_Data.egg-info/SOURCES.txt` & `OpenFisca-France-Data-1.1.0/OpenFisca_France_Data.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 openfisca_france_data/erfs_fpr/test_case_creation.py
 openfisca_france_data/erfs_fpr/input_data_builder/__init__.py
 openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py
 openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py
 openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py
 openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py
 openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py
-openfisca_france_data/erfs_fpr/input_data_builder/step_05_foyer.py
 openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py
 openfisca_france_data/felin/input_data_builder/__init__.py
 openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py
 openfisca_france_data/model/__init__.py
 openfisca_france_data/model/base.py
 openfisca_france_data/model/calage.py
 openfisca_france_data/model/common.py
```

### Comparing `OpenFisca-France-Data-1.0/PKG-INFO` & `OpenFisca-France-Data-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-France-Data
-Version: 1.0
+Version: 1.1.0
 Summary: OpenFisca-France-Data module to work with French survey data
 Home-page: https://github.com/openfisca/openfisca-france-data
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit social survey data microsimulation
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-France-Data-1.0/README.md` & `OpenFisca-France-Data-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/__init__.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/aggregates.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/base_survey.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/base_survey.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/common.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/common.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/comparator.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/comparator.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/config.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/config.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs/__init__.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/__init__.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/base.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/base.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/run_all.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/run_all.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs/old/aggregates.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/old/aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs/old/datatable.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/old/datatable.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs/scenario.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs/scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/comparison.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/comparison.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,25 +41,14 @@
         "retraite_imposable",
         # "ric",
         # "rnc",
        "salaire_imposable",
        "statut_occupation_logement",
         ]
 
-    from openfisca_france_data.erfs_fpr.get_survey_scenario import menage_projected_variables
-
-    target_menage_projected_variables = [
-        f"{menage_projected_variable}_menage"
-        for menage_projected_variable
-        in menage_projected_variables
-        ]
-
-    default_target_variables += target_menage_projected_variables
-
-
     def compute_test_dataframes(self):
         erfs_fpr_survey_collection = SurveyCollection.load(collection = "erfs_fpr")
         # infer names of the survey and data tables
         assert self.period is not None
         year = int(self.period)
         table_by_name = build_table_by_name(year, erfs_fpr_survey_collection)
```

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,16 @@
     "chomage_net",
     "retraite_nette",
     "ppa",
     ]
 
 
 menage_projected_variables = [
-    # "rev_financier_prelev_lib_imputes",
-    "revenu_categoriel_foncier",
-    "revenus_capitaux_prelevement_forfaitaire_unique_ir",
-    ]
+
+]
 
 
 class erfs_fpr_plugin(Reform):
     name = "ERFS-FPR ids plugin"
 
     def apply(self):
 
@@ -140,15 +138,14 @@
         # taux marginaux !!
         survey_scenario.variation_factor = variation_factor
         survey_scenario.varying_variable = varying_variable
 
     # S'il n'y a pas de données, on sait où les trouver.
     if data is None:
         input_data_table_by_entity = dict(
-            foyer_fiscal = f"foyer_fiscal_{year}",
             individu = f"individu_{year}",
             menage = f"menage_{year}",
             )
 
         input_data_table_by_entity_by_period = dict()
         input_data_table_by_entity_by_period[year] = input_data_table_by_entity
```

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 from openfisca_france_data.erfs_fpr.input_data_builder import (
     step_01_preprocessing as preprocessing,
     # step_02_imputation_loyer as imputation_loyer,
     step_02_menage as menage,
     step_03_variables_individuelles as variables_individuelles,
     step_04_famille as famille,
-    step_05_foyer as foyer,
     step_06_final as final,
     )
 
 log = logging.getLogger(__name__)
 log.setLevel(logging.DEBUG)
 
 # BCO : Il ne faut pas envoyer les logs dans ""../logs" car c'est un dossier qui n'existe pas.
@@ -46,48 +45,45 @@
 
     # Step 01 : le formattage OpenFisca
     #
     # - Formattage des différentes variables
     # - On merge les tables individus / menages
     #
     # Note : c'est ici où on objectivise les hypothèses, step 1
-    log.info('\n [[[ Year {} - Step 1 / 6 ]]] \n'.format(year))
+    log.info('\n [[[ Year {} - Step 1 / 5 ]]] \n'.format(year))
     preprocessing.build_merged_dataframes(year = year)
 
     # Step 02 : Si on veut calculer les allocations logement, il faut faire le matching avec une autre enquête (ENL)
     #
     # openfisca_survey_collection = SurveyCollection(name = 'openfisca')
     # stata_directory = openfisca_survey_collection.config.get('data', 'stata_directory')
     # stata_file = os.path.join(stata_directory, 'log_men_ERFS.dta')
     # imputation_loyer.merge_imputation_loyer(stata_file = stata_file, year = year)
-    log.info('\n [[[ Year {} - Step 2 / 6 SKIPPED ]]] \n'.format(year))
+    log.info('\n [[[ Year {} - Step 2 / 5 SKIPPED ]]] \n'.format(year))
     menage.build_variables_menage(year = year)
 
     # Step 03 : on commence par les variables indivuelles
-    log.info('\n [[[ Year {} - Step 3 / 6 ]]] \n'.format(year))
+    log.info('\n [[[ Year {} - Step 3 / 5 ]]] \n'.format(year))
     variables_individuelles.build_variables_individuelles(year = year)
 
     # Step 04 : ici on va constituer foyer et famille à partir d'invididu et ménage
     #
     # - On fait individu/ménage pour pouvoir faire des familles (foyers sociaux)
     # - On va faire des suppositions pour faire les familles
     # - On va faire les foyers fiscaux à partir des familles
     # - On va faire de suppositions pour faire les foyers fiscaux
-    log.info('\n [[[ Year {} - Step 4 / 6 ]]] \n'.format(year))
+    log.info('\n [[[ Year {} - Step 4 / 5 ]]] \n'.format(year))
     famille.build_famille(year = year)
 
-    log.info('\n [[[ Year {} - Step 5 / 6 ]]] \n'.format(year))
-    foyer.build_variables_foyers_fiscal(year = year)
-
     # Affreux ! On injectait tout dans un même DataFrame !!!
     # C'est très moche !
     #
     # On crée une df par entité par période.
     # Elles sont stockées dans un fichier h5
-    log.info('\n [[[ Year {} - Step 6 / 6 ]]] \n'.format(year))
+    log.info('\n [[[ Year {} - Step 5 / 5 ]]] \n'.format(year))
     final.create_input_data_frame(year = year, export_flattened_df_filepath = export_flattened_df_filepath)
 
 
 @click.command()
 @click.option('-y', '--year', default = REFERENCE_YEAR, help = "ERFS-FPR year", show_default = True, type = int, required = True)
 @click.option('-f', '--file', 'export_flattened_df_filepath', default = None, help = 'flattened dataframe filepath', show_default = True)
 @click.option('-c', '--configfile', default = None, help = 'raw_data.ini path to read years to process.', show_default = True)
```

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,20 +8,29 @@
 
 
 log = logging.getLogger(__name__)
 
 
 @temporary_store_decorator(file_name = 'erfs_fpr')
 def build_variables_menage(temporary_store = None, year = None):
+    menages = temporary_store[f'menages_{year}']
+
+    if "loyer" in menages.columns:
+        menages['loyer'] = menages['loyer'] * 12
+
     if year == 2018:
-        menages = temporary_store[f'menages_{year}']
         menages['statut_occupation_logement'] = menages['so'].copy()
 
     if year == 2019:  # SO ne fonctionne pas en 2019 bcp de 0 = non-renseigné
-        menages = temporary_store[f'menages_{year}']
         menages['statut_occupation_logement'] = menages['logt'].copy()
 
     if year >= 2018:
-        menages['zone_apl'] = 2
+        menages['zone_apl'] = 3
+        menages.loc[menages['tau2010'] == 10,'zone_apl'] = 1
+        menages.loc[menages['tau2010'] == 9,'zone_apl'] = 2
+        #menages.loc[menages['tau2010'] == 8,'zone_apl'] = 2
         # pour l'instant on met tout le monde à 2 mais à améliorer, peut être en fonction de la taille de l'aire urbaine ?
         menages.loc[(menages.statut_occupation_logement == 7), 'statut_occupation_logement'] = 2
+        menages['logement_conventionne'] = False
+        menages.loc[menages['statut_occupation_logement'] == 3 ,'logement_conventionne'] = True
         temporary_store['menages_{}'.format(year)] = menages
+
```

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     # Base pour constituer les familles, foyers, etc.
     create_statut_matrimonial(individus)
 
     # variable d'activite
     create_activite(individus)
     create_contrat_de_travail(individus, period = period, salaire_type = revenu_type)
     create_categorie_salarie(individus, period = period, survey_year = survey_year)
-
+    create_categorie_non_salarie(individus)
     # inversion des revenus pour retrouver le brut
     # pour les revenus de remplacement on a la csg et la crds dans l'erfs-fpr donc on peut avoir le brut directement
     create_revenus_remplacement_bruts(individus)
     # On n'a pas le salaire et le traitement_indiciaire brut, on doit l'inverser
     # comme on a la crds et la csg non déductible on recalcule l'imposable puis on inverse l'imposable pour avoir le brut
     #individus['salaire_imposable'] = individus.salaire_net + individus.csg_nd_crds_sal_i
     create_salaire_de_base(
@@ -485,26 +485,33 @@
         ])
 
     agriculteur = individus.cstot.isin([11, 12, 13])
     artisan = individus.cstot.isin([21])
     commercant = individus.cstot.isin([22])
     chef_entreprise = individus.cstot.isin([23])
     profession_liberale = individus.cstot.isin([31])
+    individus['categorie_non_salarie'] = 0
     individus.loc[
         agriculteur | artisan,
         'categorie_non_salarie'
         ] = 1
     individus.loc[
         commercant | chef_entreprise,
         'categorie_non_salarie'
         ] = 2
     individus.loc[
         profession_liberale,
         'categorie_non_salarie'
         ] = 3
+    #fix un peu crade : cstot ne semble pas recouvrir tout le champ des personnes qui ont du rpns
+    # on met par défaut ces gens là en chef d'entreprise
+    individus.loc[
+        ((individus['rpns_imposables'] != 0) & (individus['categorie_non_salarie'] == 0)),
+        'categorie_non_salarie'
+        ] = 2  
 
 
 def create_contrat_de_travail(individus, period, salaire_type = 'imposable'):
     """Création de la variable contrat_de_travail et heure_remunerees_volume.
 
     Ses modliatés sont:
         0 - temps_plein
```

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 @temporary_store_decorator(file_name = 'erfs_fpr')
 def create_input_data_frame(temporary_store = None, year = None, export_flattened_df_filepath = None):
     assert temporary_store is not None
     assert year is not None
 
     individus = temporary_store['individus_{}'.format(year)]
     menages = temporary_store['menages_{}'.format(year)]
-    foyers_fiscaux = temporary_store['foyers_fiscaux_{}'.format(year)]
 
     # ici : variables à garder
     var_individus = [
         'activite',
         'age',
         'categorie_salarie',
+        'categorie_non_salarie',
         'chomage_brut',
         'contrat_de_travail',
         'date_naissance',
         'effectif_entreprise',
         'heures_remunerees_volume',
         'idfam',
         'idfoy',
@@ -43,28 +43,24 @@
         'rnc',
         'rpns_imposables',
         'salaire_de_base',
         'statut_marital',
         "primes_fonction_publique",
         "traitement_indiciaire_brut",
         ]
-    var_foyers_fiscaux = [
-        'idfoy',
-        'rev_financier_prelev_lib_imputes',
-        'revenu_categoriel_foncier',
-        'revenus_capitaux_prelevement_forfaitaire_unique_ir',
-        ]
 
     var_menages = [
         'idmen',
         'loyer',
         'statut_occupation_logement',
         'taxe_habitation',
         'wprm',
         'zone_apl',
+        'logement_conventionne',
+        'prest_precarite_hand' # on récupère la variable de montant de aah / caah pour pouvoir faire une imputation du handicap
     ]
 
     individus = create_ids_and_roles(individus)
     individus = individus[var_individus].copy()
     gc.collect()
 
     # This looks like it could have a sizeable impact
@@ -76,45 +72,28 @@
     menages = extract_menages_variables(menages)
 
     # individus = create_collectives_foyer_variables(individus, menages)
 
     idmens = individus.idmen.unique()
     menages = menages.loc[
         menages.idmen.isin(idmens),
-        [
-            'idmen',
-            'loyer',
-            'statut_occupation_logement',
-            'taxe_habitation',
-            'wprm',
-            'zone_apl',
-            ]
+        var_menages
         ].copy()
     survey_name = 'openfisca_erfs_fpr_' + str(year)
 
     # Formats ids
     individus = format_ids_and_roles(individus)
     menages = menages.rename(columns = {'idmen':'idmen_original'})
     unique_idmen = individus[['idmen','idmen_original']].drop_duplicates()
     assert len(unique_idmen) == len(menages), "Number of idmen should be the same individus and menages tables."
 
     menages = menages.merge(unique_idmen,
                             how = 'inner',
                             on = 'idmen_original')
 
-    foyers_fiscaux = foyers_fiscaux.rename(columns = {'idfoy':'idfoy_original'})
-    unique_idfoy = individus[['idfoy','idfoy_original']].drop_duplicates()
-    assert len(unique_idmen) == len(menages), "Number of idfoy should be the same individus and foyers tables."
-
-    foyers_fiscaux = foyers_fiscaux.merge(unique_idfoy,
-                                          how = 'inner',
-                                          on = 'idfoy_original')
-
-    foyers_fiscaux = foyers_fiscaux[var_foyers_fiscaux]
-
     if export_flattened_df_filepath:
         supermerge = individus.merge(
             menages,
             right_index = True,
             left_on = "idmen",
             suffixes = ("", "_x"))
         log.debug(f"Saving to {export_flattened_df_filepath}")
@@ -127,25 +106,14 @@
         individus,
         entity = "individu",
         period = year,
         collection = "openfisca_erfs_fpr",
         survey_name = survey_name,
         )
 
-    foyers_fiscaux = foyers_fiscaux.sort_values(by = ['idfoy'])
-    log.debug(f"Saving entity 'foyers fiscaux' in collection 'openfisca_erfs_fpr' and survey name '{survey_name}' with set_table_in_survey")
-    set_table_in_survey(
-        foyers_fiscaux,
-        entity = "foyer_fiscal",
-        period = year,
-        collection = "openfisca_erfs_fpr",
-        survey_name = survey_name,
-        )
-    log.debug("End of create_input_data_frame")
-
     menages = menages.sort_values(by = ['idmen'])
     log.debug(f"Saving entity 'menage' in collection 'openfisca_erfs_fpr' and survey name '{survey_name}' with set_table_in_survey")
     set_table_in_survey(
         menages,
         entity = "menage",
         period = year,
         collection = "openfisca_erfs_fpr",
@@ -251,15 +219,15 @@
     assert year is not None
     menages = temporary_store['menages_{}'.format(year)]
     return extract_menages_variables(menages)
 
 
 def extract_menages_variables(menages):
     variables = ['ident', 'wprm', 'taxe_habitation']
-    external_variables = ['loyer', 'zone_apl', 'statut_occupation_logement']
+    external_variables = ['loyer', 'zone_apl', 'statut_occupation_logement','logement_conventionne', 'prest_precarite_hand']
     for external_variable in external_variables:
         if external_variable in menages.columns:
             log.debug("Found {} in menages table: we keep it".format(external_variable))
             variables.append(external_variable)
     menages = menages[variables].copy()
     menages.taxe_habitation = - menages.taxe_habitation  # taxes should be negative
     menages.rename(columns = dict(ident = 'idmen'), inplace = True)
```

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/scenario.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/scenario.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,32 +7,31 @@
     collection = "openfisca_erfs_fpr"
 
     # Les variables OpenFisca qu'on va utiliser avec les données en entrée.
     used_as_input_variables = [
         "activite",
         "autonomie_financiere",
         "categorie_salarie",
+        "categorie_non_salarie",
         "chomage_brut",
         "chomage_imposable",
         "contrat_de_travail",
         "cotisation_sociale_mode_recouvrement",
         "date_naissance",
         "effectif_entreprise",
         "f4ba",
         "heures_remunerees_volume",
+        "logement_conventionne",
         "loyer",
         "pensions_alimentaires_percues",
         "pensions_invalidite",
         "primes_fonction_publique",
         "rag",
         "retraite_brute",
         "retraite_imposable",
-        # "rev_financier_prelev_lib_imputes",
-        "revenu_categoriel_foncier",
-        "revenus_capitaux_prelevement_forfaitaire_unique_ir",
         "ric",
         "rnc",
         "rpns_imposables",
         "salaire_de_base",
         "statut_marital",
         "statut_occupation_logement",
         "taxe_habitation",
```

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/erfs_fpr/test_case_creation.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/erfs_fpr/test_case_creation.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/model/base.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/model/base.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/model/calage.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/model/calage.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/model/common.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/model/common.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/model/id_variables.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/model/id_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/model/survey_variables.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/model/survey_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/reforms/inversion_directe_salaires.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/reforms/inversion_directe_salaires.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/scripts/build_input_data.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/scripts/build_input_data.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/smic.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/smic.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/surveys.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/surveys.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,13 +189,10 @@
                             variable,
                             simulation_period.offset(offset),
                             permanent_value
                             )
 
 
     def custom_input_data_frame(self, input_data_frame, **kwargs):
-        if "loyer" in input_data_frame:
-            input_data_frame["loyer"] = 12 * input_data_frame.loyer
-
         for variable in ["quifam", "quifoy", "quimen"]:
             if variable in input_data_frame:
                 log.debug(input_data_frame[variable].value_counts(dropna = False))
```

### Comparing `OpenFisca-France-Data-1.0/openfisca_france_data/utils.py` & `OpenFisca-France-Data-1.1.0/openfisca_france_data/utils.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/setup.cfg` & `OpenFisca-France-Data-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/setup.py` & `OpenFisca-France-Data-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md') as file:
     long_description = file.read()
 
 setup(
     name = "OpenFisca-France-Data",
-    version = "1.0",
+    version = "1.1.0",
     description = "OpenFisca-France-Data module to work with French survey data",
     long_description = long_description,
     long_description_content_type="text/markdown",
     author = "OpenFisca Team",
     author_email = "contact@openfisca.fr",
     url = "https://github.com/openfisca/openfisca-france-data",
     license = "http://www.fsf.org/licensing/licenses/agpl-3.0.html",
```

### Comparing `OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_af.py` & `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_af.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_aggregates.py` & `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_al.py` & `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_al.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py` & `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_impot_revenu.py` & `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_impot_revenu.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_inflation.py` & `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_inflation.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_input_variables.py` & `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_input_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_pivot_table.py` & `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_pivot_table.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_rebuild_input_data.py` & `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_rebuild_input_data.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_rsa.py` & `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_rsa.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/tests/erfs_fpr/integration/test_salaire_imposable.py` & `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/integration/test_salaire_imposable.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/tests/erfs_fpr/unit/test_get_survey_scenario.py` & `OpenFisca-France-Data-1.1.0/tests/erfs_fpr/unit/test_get_survey_scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/tests/test_aggregate.py` & `OpenFisca-France-Data-1.1.0/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/tests/test_calibration.py` & `OpenFisca-France-Data-1.1.0/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/tests/test_fake_survey_simulation.py` & `OpenFisca-France-Data-1.1.0/tests/test_fake_survey_simulation.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/tests/test_get_baremes_salarie.py` & `OpenFisca-France-Data-1.1.0/tests/test_get_baremes_salarie.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.0/tests/test_misc.py` & `OpenFisca-France-Data-1.1.0/tests/test_misc.py`

 * *Files identical despite different names*

