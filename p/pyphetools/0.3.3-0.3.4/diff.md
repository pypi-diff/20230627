# Comparing `tmp/pyphetools-0.3.3.tar.gz` & `tmp/pyphetools-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphetools-0.3.3.tar", last modified: Mon Jun 26 23:11:11 2023, max compression
+gzip compressed data, was "pyphetools-0.3.4.tar", last modified: Tue Jun 27 20:24:45 2023, max compression
```

## Comparing `pyphetools-0.3.3.tar` & `pyphetools-0.3.4.tar`

### file list

```diff
@@ -1,81 +1,83 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.370327 pyphetools-0.3.3/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1079 2023-02-05 19:04:48.000000 pyphetools-0.3.3/LICENSE
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-12-16 00:09:56.000000 pyphetools-0.3.3/MANIFEST.in
--rw-rw-r--   0 peter     (1000) peter     (1000)     2825 2023-06-26 23:11:11.370327 pyphetools-0.3.3/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      767 2023-06-26 23:11:02.000000 pyphetools-0.3.3/README.md
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.254326 pyphetools-0.3.3/docs/
--rw-rw-r--   0 peter     (1000) peter     (1000)     4165 2023-06-25 22:31:24.000000 pyphetools-0.3.3/docs/conf.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.254326 pyphetools-0.3.3/pyphetools/
--rw-rw-r--   0 peter     (1000) peter     (1000)       11 2023-02-05 19:04:48.000000 pyphetools-0.3.3/pyphetools/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.254326 pyphetools-0.3.3/pyphetools/analyze/
--rw-rw-r--   0 peter     (1000) peter     (1000)       36 2023-02-05 19:04:48.000000 pyphetools-0.3.3/pyphetools/analyze/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3062 2023-06-25 22:31:24.000000 pyphetools-0.3.3/pyphetools/analyze/downsampler.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.258326 pyphetools-0.3.3/pyphetools/creation/
--rw-rw-r--   0 peter     (1000) peter     (1000)      794 2023-05-12 21:54:20.000000 pyphetools-0.3.3/pyphetools/creation/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4873 2023-05-11 10:59:47.000000 pyphetools-0.3.3/pyphetools/creation/age_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6558 2023-06-25 20:28:58.000000 pyphetools-0.3.3/pyphetools/creation/case_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     9043 2023-06-25 22:31:24.000000 pyphetools-0.3.3/pyphetools/creation/cohort_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      531 2023-05-10 19:30:33.000000 pyphetools-0.3.3/pyphetools/creation/column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2339 2023-06-25 22:31:24.000000 pyphetools-0.3.3/pyphetools/creation/constant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      308 2023-05-07 14:22:13.000000 pyphetools-0.3.3/pyphetools/creation/constants.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3014 2023-05-11 13:07:39.000000 pyphetools-0.3.3/pyphetools/creation/custom_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3281 2023-06-25 20:29:31.000000 pyphetools-0.3.3/pyphetools/creation/hp_term.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      740 2023-05-11 10:59:47.000000 pyphetools-0.3.3/pyphetools/creation/hpo_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7110 2023-05-11 11:50:47.000000 pyphetools-0.3.3/pyphetools/creation/hpo_exact_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6248 2023-06-25 22:31:24.000000 pyphetools-0.3.3/pyphetools/creation/hpo_parser.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7382 2023-06-25 22:44:11.000000 pyphetools-0.3.3/pyphetools/creation/individual.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5795 2023-06-25 22:31:24.000000 pyphetools-0.3.3/pyphetools/creation/metadata.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3541 2023-06-26 12:01:47.000000 pyphetools-0.3.3/pyphetools/creation/option_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2194 2023-05-17 14:42:11.000000 pyphetools-0.3.3/pyphetools/creation/sex_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4678 2023-05-13 00:28:58.000000 pyphetools-0.3.3/pyphetools/creation/simple_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2656 2023-05-11 11:04:54.000000 pyphetools-0.3.3/pyphetools/creation/thresholded_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4976 2023-06-25 17:17:47.000000 pyphetools-0.3.3/pyphetools/creation/variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4714 2023-06-26 23:11:02.000000 pyphetools-0.3.3/pyphetools/creation/variant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3229 2023-05-11 10:59:47.000000 pyphetools-0.3.3/pyphetools/creation/variant_validator.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.258326 pyphetools-0.3.3/pyphetools/output/
--rw-rw-r--   0 peter     (1000) peter     (1000)      327 2023-06-24 19:26:58.000000 pyphetools-0.3.3/pyphetools/output/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3067 2023-06-25 22:31:24.000000 pyphetools-0.3.3/pyphetools/output/detailed_suppl_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5727 2023-06-25 22:31:24.000000 pyphetools-0.3.3/pyphetools/output/focus_count_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2980 2023-02-05 19:04:49.000000 pyphetools-0.3.3/pyphetools/output/hpo_category.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      894 2023-02-05 19:04:49.000000 pyphetools-0.3.3/pyphetools/output/phenopacket_ingestor.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2154 2023-06-24 20:06:45.000000 pyphetools-0.3.3/pyphetools/output/phenopacket_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4960 2023-06-24 20:15:49.000000 pyphetools-0.3.3/pyphetools/output/simple_patient.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3310 2023-06-24 20:23:41.000000 pyphetools-0.3.3/pyphetools/output/simple_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      569 2023-05-11 10:59:47.000000 pyphetools-0.3.3/pyphetools/output/term_count.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.258326 pyphetools-0.3.3/pyphetools/validation/
--rw-rw-r--   0 peter     (1000) peter     (1000)        8 2023-06-25 22:31:24.000000 pyphetools-0.3.3/pyphetools/validation/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.254326 pyphetools-0.3.3/pyphetools.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)     2825 2023-06-26 23:11:11.000000 pyphetools-0.3.3/pyphetools.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     2083 2023-06-26 23:11:11.000000 pyphetools-0.3.3/pyphetools.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-06-26 23:11:11.000000 pyphetools-0.3.3/pyphetools.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       66 2023-06-26 23:11:11.000000 pyphetools-0.3.3/pyphetools.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       50 2023-06-26 23:11:11.000000 pyphetools-0.3.3/pyphetools.egg-info/top_level.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)     1318 2023-06-26 23:11:02.000000 pyphetools-0.3.3/pyproject.toml
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-06-26 23:11:11.370327 pyphetools-0.3.3/setup.cfg
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.262326 pyphetools-0.3.3/test/
--rw-rw-r--   0 peter     (1000) peter     (1000)     3297 2023-02-05 19:04:49.000000 pyphetools-0.3.3/test/test_age_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2956 2023-05-11 10:59:47.000000 pyphetools-0.3.3/test/test_case_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4553 2023-05-10 22:56:45.000000 pyphetools-0.3.3/test/test_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1156 2023-05-12 23:59:19.000000 pyphetools-0.3.3/test/test_constant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2745 2023-05-14 12:05:29.000000 pyphetools-0.3.3/test/test_custom_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1430 2023-06-23 21:44:02.000000 pyphetools-0.3.3/test/test_hp_term.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      914 2023-02-05 19:04:49.000000 pyphetools-0.3.3/test/test_hpo_category.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5966 2023-05-11 14:18:42.000000 pyphetools-0.3.3/test/test_hpo_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      439 2023-02-05 19:04:49.000000 pyphetools-0.3.3/test/test_hpo_parser.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5385 2023-06-26 12:00:47.000000 pyphetools-0.3.3/test/test_option_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1856 2023-05-11 14:18:42.000000 pyphetools-0.3.3/test/test_threshold_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1439 2023-05-11 14:18:42.000000 pyphetools-0.3.3/test/test_variant.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.254326 pyphetools-0.3.3/venv/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.370327 pyphetools-0.3.3/venv/bin/
--rwxrwxr-x   0 peter     (1000) peter     (1000)      621 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2html.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      741 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2html4.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1109 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2html5.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      818 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2latex.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      626 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2man.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      791 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2odt.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1753 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      628 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2pseudoxml.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      664 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2s5.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      898 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2xetex.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      629 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2xml.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      697 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rstpep2html.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-27 20:24:45.161367 pyphetools-0.3.4/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1079 2023-02-05 19:04:48.000000 pyphetools-0.3.4/LICENSE
+-rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-12-16 00:09:56.000000 pyphetools-0.3.4/MANIFEST.in
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-06-27 20:24:45.161367 pyphetools-0.3.4/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      767 2023-06-26 23:11:02.000000 pyphetools-0.3.4/README.md
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-27 20:24:45.157367 pyphetools-0.3.4/docs/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4165 2023-06-25 22:31:24.000000 pyphetools-0.3.4/docs/conf.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-27 20:24:45.157367 pyphetools-0.3.4/pyphetools/
+-rw-rw-r--   0 peter     (1000) peter     (1000)       11 2023-02-05 19:04:48.000000 pyphetools-0.3.4/pyphetools/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-27 20:24:45.157367 pyphetools-0.3.4/pyphetools/analyze/
+-rw-rw-r--   0 peter     (1000) peter     (1000)       36 2023-02-05 19:04:48.000000 pyphetools-0.3.4/pyphetools/analyze/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3062 2023-06-25 22:31:24.000000 pyphetools-0.3.4/pyphetools/analyze/downsampler.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-27 20:24:45.157367 pyphetools-0.3.4/pyphetools/creation/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      844 2023-06-27 19:48:45.000000 pyphetools-0.3.4/pyphetools/creation/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4873 2023-05-11 10:59:47.000000 pyphetools-0.3.4/pyphetools/creation/age_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6558 2023-06-25 20:28:58.000000 pyphetools-0.3.4/pyphetools/creation/case_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     9293 2023-06-27 16:45:59.000000 pyphetools-0.3.4/pyphetools/creation/cohort_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      531 2023-05-10 19:30:33.000000 pyphetools-0.3.4/pyphetools/creation/column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2339 2023-06-25 22:31:24.000000 pyphetools-0.3.4/pyphetools/creation/constant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      308 2023-05-07 14:22:13.000000 pyphetools-0.3.4/pyphetools/creation/constants.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3014 2023-05-11 13:07:39.000000 pyphetools-0.3.4/pyphetools/creation/custom_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3281 2023-06-25 20:29:31.000000 pyphetools-0.3.4/pyphetools/creation/hp_term.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      740 2023-05-11 10:59:47.000000 pyphetools-0.3.4/pyphetools/creation/hpo_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7207 2023-06-27 16:06:41.000000 pyphetools-0.3.4/pyphetools/creation/hpo_exact_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6926 2023-06-27 17:37:13.000000 pyphetools-0.3.4/pyphetools/creation/hpo_parser.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7382 2023-06-25 22:44:11.000000 pyphetools-0.3.4/pyphetools/creation/individual.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5795 2023-06-25 22:31:24.000000 pyphetools-0.3.4/pyphetools/creation/metadata.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3541 2023-06-26 12:01:47.000000 pyphetools-0.3.4/pyphetools/creation/option_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2194 2023-05-17 14:42:11.000000 pyphetools-0.3.4/pyphetools/creation/sex_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4678 2023-05-13 00:28:58.000000 pyphetools-0.3.4/pyphetools/creation/simple_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6865 2023-06-27 20:07:27.000000 pyphetools-0.3.4/pyphetools/creation/structural_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2656 2023-05-11 11:04:54.000000 pyphetools-0.3.4/pyphetools/creation/thresholded_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4976 2023-06-25 17:17:47.000000 pyphetools-0.3.4/pyphetools/creation/variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4714 2023-06-26 23:11:02.000000 pyphetools-0.3.4/pyphetools/creation/variant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3227 2023-06-27 16:40:26.000000 pyphetools-0.3.4/pyphetools/creation/variant_validator.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-27 20:24:45.157367 pyphetools-0.3.4/pyphetools/output/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      327 2023-06-24 19:26:58.000000 pyphetools-0.3.4/pyphetools/output/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3067 2023-06-25 22:31:24.000000 pyphetools-0.3.4/pyphetools/output/detailed_suppl_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5727 2023-06-25 22:31:24.000000 pyphetools-0.3.4/pyphetools/output/focus_count_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2980 2023-02-05 19:04:49.000000 pyphetools-0.3.4/pyphetools/output/hpo_category.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      894 2023-02-05 19:04:49.000000 pyphetools-0.3.4/pyphetools/output/phenopacket_ingestor.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2154 2023-06-24 20:06:45.000000 pyphetools-0.3.4/pyphetools/output/phenopacket_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4960 2023-06-24 20:15:49.000000 pyphetools-0.3.4/pyphetools/output/simple_patient.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3310 2023-06-24 20:23:41.000000 pyphetools-0.3.4/pyphetools/output/simple_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      569 2023-05-11 10:59:47.000000 pyphetools-0.3.4/pyphetools/output/term_count.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-27 20:24:45.157367 pyphetools-0.3.4/pyphetools/validation/
+-rw-rw-r--   0 peter     (1000) peter     (1000)        8 2023-06-25 22:31:24.000000 pyphetools-0.3.4/pyphetools/validation/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-27 20:24:45.157367 pyphetools-0.3.4/pyphetools.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-06-27 20:24:45.000000 pyphetools-0.3.4/pyphetools.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2157 2023-06-27 20:24:45.000000 pyphetools-0.3.4/pyphetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-06-27 20:24:45.000000 pyphetools-0.3.4/pyphetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       81 2023-06-27 20:24:45.000000 pyphetools-0.3.4/pyphetools.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       50 2023-06-27 20:24:45.000000 pyphetools-0.3.4/pyphetools.egg-info/top_level.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1367 2023-06-27 16:09:41.000000 pyphetools-0.3.4/pyproject.toml
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-06-27 20:24:45.161367 pyphetools-0.3.4/setup.cfg
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-27 20:24:45.161367 pyphetools-0.3.4/test/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3297 2023-02-05 19:04:49.000000 pyphetools-0.3.4/test/test_age_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2956 2023-05-11 10:59:47.000000 pyphetools-0.3.4/test/test_case_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4553 2023-05-10 22:56:45.000000 pyphetools-0.3.4/test/test_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1156 2023-05-12 23:59:19.000000 pyphetools-0.3.4/test/test_constant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2745 2023-05-14 12:05:29.000000 pyphetools-0.3.4/test/test_custom_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1430 2023-06-23 21:44:02.000000 pyphetools-0.3.4/test/test_hp_term.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      914 2023-02-05 19:04:49.000000 pyphetools-0.3.4/test/test_hpo_category.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5966 2023-05-11 14:18:42.000000 pyphetools-0.3.4/test/test_hpo_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      835 2023-06-27 16:07:00.000000 pyphetools-0.3.4/test/test_hpo_parser.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5385 2023-06-26 12:00:47.000000 pyphetools-0.3.4/test/test_option_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1625 2023-06-27 20:22:15.000000 pyphetools-0.3.4/test/test_structural_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1856 2023-05-11 14:18:42.000000 pyphetools-0.3.4/test/test_threshold_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1439 2023-05-11 14:18:42.000000 pyphetools-0.3.4/test/test_variant.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-27 20:24:45.153367 pyphetools-0.3.4/venv/
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-27 20:24:45.161367 pyphetools-0.3.4/venv/bin/
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      621 2022-12-06 12:58:50.000000 pyphetools-0.3.4/venv/bin/rst2html.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      741 2022-12-06 12:58:50.000000 pyphetools-0.3.4/venv/bin/rst2html4.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1109 2022-12-06 12:58:50.000000 pyphetools-0.3.4/venv/bin/rst2html5.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      818 2022-12-06 12:58:50.000000 pyphetools-0.3.4/venv/bin/rst2latex.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      626 2022-12-06 12:58:50.000000 pyphetools-0.3.4/venv/bin/rst2man.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      791 2022-12-06 12:58:50.000000 pyphetools-0.3.4/venv/bin/rst2odt.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1753 2022-12-06 12:58:50.000000 pyphetools-0.3.4/venv/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      628 2022-12-06 12:58:50.000000 pyphetools-0.3.4/venv/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      664 2022-12-06 12:58:50.000000 pyphetools-0.3.4/venv/bin/rst2s5.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      898 2022-12-06 12:58:50.000000 pyphetools-0.3.4/venv/bin/rst2xetex.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      629 2022-12-06 12:58:50.000000 pyphetools-0.3.4/venv/bin/rst2xml.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      697 2022-12-06 12:58:50.000000 pyphetools-0.3.4/venv/bin/rstpep2html.py
```

### Comparing `pyphetools-0.3.3/LICENSE` & `pyphetools-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/PKG-INFO` & `pyphetools-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.3.3
+Version: 0.3.4
 Summary: Generate and work with GA4GH phenopackets
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,14 +30,15 @@
 Project-URL: bugtracker, https://github.com/monarch-initiative/pyphetools/issues
 Keywords: Global Alliance for Genomics and Health,GA4GH Phenopacket Schema,Human Phenotype Ontology,GA4GH,HPO
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 [![CI](https://github.com/monarch-initiative/genophenocorr/workflows/CI/badge.svg)](https://github.com/monarch-initiative/pyphetools/actions/workflows/python_ci.yml)
 
 # pyphetools
 Python Phenopacket Tools
```

### Comparing `pyphetools-0.3.3/README.md` & `pyphetools-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/docs/conf.py` & `pyphetools-0.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/analyze/downsampler.py` & `pyphetools-0.3.4/pyphetools/analyze/downsampler.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/creation/__init__.py` & `pyphetools-0.3.4/pyphetools/creation/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,11 +8,12 @@
 from .hpo_parser import HpoParser
 from .hp_term import HpTerm
 from .individual import Individual
 from .metadata import MetaData
 from .option_column_mapper import OptionColumnMapper
 from .sex_column_mapper import SexColumnMapper
 from .simple_column_mapper import SimpleColumnMapper
+from .structural_variant import StructuralVariant
 from .thresholded_column_mapper import ThresholdedColumnMapper
 from .variant_validator import VariantValidator
 from .variant_column_mapper import VariantColumnMapper
 from .variant import Variant
```

### Comparing `pyphetools-0.3.3/pyphetools/creation/age_column_mapper.py` & `pyphetools-0.3.4/pyphetools/creation/age_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/creation/case_encoder.py` & `pyphetools-0.3.4/pyphetools/creation/case_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/creation/cohort_encoder.py` & `pyphetools-0.3.4/pyphetools/creation/cohort_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 from .constants import Constants
 from .hpo_cr import HpoConceptRecognizer
 from .individual import Individual
 from .variant_column_mapper import VariantColumnMapper
 
 
 class CohortEncoder:
+    """Encode a cohort of individuals with clinical data in a table as a collection of GA4GH Phenopackets
+    This classes uses a collection of ColumnMapper objects to map a table using the
+    get_individuals or output_phenopackets methods.
+    """
 
     def __init__(self, df, hpo_cr, column_mapper_d, individual_column_name, metadata,
                  agemapper=AgeColumnMapper.not_provided(), sexmapper=None, variant_mapper=None, pmid=None):
         if not isinstance(hpo_cr, HpoConceptRecognizer):
             raise ValueError(
                 "concept_recognizer argument must be HpoConceptRecognizer but was {type(concept_recognizer)}")
         self._hpo_concept_recognizer = hpo_cr
```

### Comparing `pyphetools-0.3.3/pyphetools/creation/column_mapper.py` & `pyphetools-0.3.4/pyphetools/creation/column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/creation/constant_column_mapper.py` & `pyphetools-0.3.4/pyphetools/creation/constant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/creation/custom_column_mapper.py` & `pyphetools-0.3.4/pyphetools/creation/custom_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/creation/hp_term.py` & `pyphetools-0.3.4/pyphetools/creation/hp_term.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/creation/hpo_cr.py` & `pyphetools-0.3.4/pyphetools/creation/hpo_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/creation/hpo_exact_cr.py` & `pyphetools-0.3.4/pyphetools/creation/hpo_exact_cr.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,26 +132,29 @@
         regex_pattern = '|'.join(map(re.escape, delimiters))
         chunks = re.split(regex_pattern, line)
         return [chunk.strip().lower() for chunk in chunks]
 
     def get_term_from_id(self, hpo_id) -> HpTerm:
         if not hpo_id.startswith("HP:"):
             raise ValueError(f"Malformed HP id '{hpo_id}' - must start with HP:")
-        if not hpo_id in self._id_to_primary_label:
+        if hpo_id not in self._id_to_primary_label:
             raise ValueError(f"Could not find id {hpo_id} in dictionary")
         label = self._id_to_primary_label.get(hpo_id)
         return HpTerm(hpo_id=hpo_id, label=label)
 
     def get_term_from_label(self, label) -> HpTerm:
         label_lc = label.lower()  # the dictionary was constructed in lower case!
         if label_lc not in self._label_to_id:
             raise ValueError(f"Could not find HPO id for {label}")
         hpo_id = self._label_to_id.get(label_lc)
         return HpTerm(hpo_id=hpo_id, label=label)
 
+    def contains_term(self, hpo_id) -> bool:
+        return hpo_id in self._id_to_primary_label
+
     def initialize_simple_column_maps(self, column_name_to_hpo_label_map, observed, excluded, non_measured=None):
         if observed is None or excluded is None:
             raise ValueError("Symbols for observed (e.g., +, Y, yes) and excluded (e.g., -, N, no) required")
         if not isinstance(column_name_to_hpo_label_map, dict):
             raise ValueError("column_name_to_hpo_label_map must be a dict with column to HPO label mappings")
         simple_mapper_d = defaultdict(ColumnMapper)
         for column_name, hpo_label_and_id in column_name_to_hpo_label_map.items():
```

### Comparing `pyphetools-0.3.3/pyphetools/creation/hpo_parser.py` & `pyphetools-0.3.4/pyphetools/creation/hpo_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -102,16 +102,18 @@
         nodes = hpo.get("nodes")
         edges = hpo.get("edges")
         valid_node_curies = extract_phenotype_descendant_ids(nodes=nodes, edges=edges)
         id_to_primary_label = defaultdict()
         label_to_id = defaultdict()
         for n in nodes:
             if 'id' in n and 'HP_' in n.get('id'):
+                if self._is_deprecated_node(n):
+                    continue
                 hpo_id, label, all_labels = self._extract_node_data(n)
-                if not hpo_id in valid_node_curies:
+                if hpo_id not in valid_node_curies:
                     continue  # This restricts us to descendants of Phenotypic abnormality
                 id_to_primary_label[hpo_id] = label
                 for lab in all_labels:
                     label_to_id[lab.lower()] = hpo_id
         self._id_to_primary_label = id_to_primary_label
         self._label_to_id = label_to_id
         meta = hpo.get('meta')
@@ -119,25 +121,39 @@
         if 'http://purl.obolibrary.org/obo/hp/releases/' in long_version:
             version = long_version[43:].split('/')[0]
         else:
             version = long_version
         self._long_version = long_version
         self._version = version
 
+
+    def _is_deprecated_node(self, json_node):
+        """check if a node was obsoleted
+        Skip obsoleted nodes such as "lbl": "obsolete Abnormality of the ocular region",
+        obsoleted nodes have a "deprecated" attribute whose value is always true (and this is not checked here)
+        """
+        metadata = json_node.get('meta')
+        if metadata is not None:
+            if "deprecated" in metadata:
+                # This is a sign that the term has been obsoleted
+                # We want to skip such terms
+                return True
+        return False
+
     def _extract_node_data(self, json_node):
         if not isinstance(json_node, dict):
             raise ValueError("HpoNode obhject must be constructed from JSON-derived dictionary")
-        if not 'id' in json_node.keys():
+        if 'id' not in json_node.keys():
             raise ValueError("HpoNode object must have id attribute")
-        id = json_node.get('id')
+        node_id = json_node.get('id')
         if 'lbl' not in json_node.keys():
-            raise ValueError(f"HpoNode object must have lbl attribute but {id} did not")
-        if  'http://purl.obolibrary.org/obo/HP' not in id:
-            raise ValueError(f"HpoNode id must begin with 'http://purl.obolibrary.org/obo/' but we got {id}")
-        hpo_id = id[31:].replace("_", ":")
+            raise ValueError(f"HpoNode object must have lbl attribute but {node_id} did not")
+        if 'http://purl.obolibrary.org/obo/HP' not in node_id:
+            raise ValueError(f"HpoNode id must begin with 'http://purl.obolibrary.org/obo/' but we got {node_id}")
+        hpo_id = node_id[31:].replace("_", ":")
         label = json_node.get("lbl", "NA")
         all_labels = set()
         all_labels.add(label)
         # synonyms are nest
         metadata = json_node.get('meta')
         if metadata is not None:
             synonyms = metadata.get('synonyms', None)
```

### Comparing `pyphetools-0.3.3/pyphetools/creation/individual.py` & `pyphetools-0.3.4/pyphetools/creation/individual.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/creation/metadata.py` & `pyphetools-0.3.4/pyphetools/creation/metadata.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/creation/option_column_mapper.py` & `pyphetools-0.3.4/pyphetools/creation/option_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/creation/sex_column_mapper.py` & `pyphetools-0.3.4/pyphetools/creation/sex_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/creation/simple_column_mapper.py` & `pyphetools-0.3.4/pyphetools/creation/simple_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/creation/thresholded_column_mapper.py` & `pyphetools-0.3.4/pyphetools/creation/thresholded_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/creation/variant.py` & `pyphetools-0.3.4/pyphetools/creation/variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/creation/variant_column_mapper.py` & `pyphetools-0.3.4/pyphetools/creation/variant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/creation/variant_validator.py` & `pyphetools-0.3.4/pyphetools/creation/variant_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         
     def encode_hgvs(self, hgvs, custom_transcript=None):
         if custom_transcript is not None:
             transcript = custom_transcript
         elif self._transcript is not None:
             transcript = self._transcript
         else:
-            raise ValueError("Cannot run variant valididator without transcript")
+            raise ValueError("Cannot run variant validator without transcript")
         api_url = URL_SCHEME % (self._genome_assembly, transcript, hgvs, transcript)
         #f"https://rest.variantvalidator.org/VariantValidator/variantvalidator/{self._genome_assembly}/{transcript}%3A{hgvs}/{transcript}"
         #
         print(api_url)
         response = requests.get(api_url)
         # We expect to get a dictionary with three keys. The first is the name of the variant, e.g., ACC:HGVS, then we
         # get flag and metadata
```

### Comparing `pyphetools-0.3.3/pyphetools/output/detailed_suppl_table.py` & `pyphetools-0.3.4/pyphetools/output/detailed_suppl_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/output/focus_count_table.py` & `pyphetools-0.3.4/pyphetools/output/focus_count_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/output/hpo_category.py` & `pyphetools-0.3.4/pyphetools/output/hpo_category.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/output/phenopacket_ingestor.py` & `pyphetools-0.3.4/pyphetools/output/phenopacket_ingestor.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/output/phenopacket_table.py` & `pyphetools-0.3.4/pyphetools/output/phenopacket_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/output/simple_patient.py` & `pyphetools-0.3.4/pyphetools/output/simple_patient.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/output/simple_variant.py` & `pyphetools-0.3.4/pyphetools/output/simple_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools/output/term_count.py` & `pyphetools-0.3.4/pyphetools/output/term_count.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/pyphetools.egg-info/PKG-INFO` & `pyphetools-0.3.4/pyphetools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.3.3
+Version: 0.3.4
 Summary: Generate and work with GA4GH phenopackets
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,14 +30,15 @@
 Project-URL: bugtracker, https://github.com/monarch-initiative/pyphetools/issues
 Keywords: Global Alliance for Genomics and Health,GA4GH Phenopacket Schema,Human Phenotype Ontology,GA4GH,HPO
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 [![CI](https://github.com/monarch-initiative/genophenocorr/workflows/CI/badge.svg)](https://github.com/monarch-initiative/pyphetools/actions/workflows/python_ci.yml)
 
 # pyphetools
 Python Phenopacket Tools
```

### Comparing `pyphetools-0.3.3/pyphetools.egg-info/SOURCES.txt` & `pyphetools-0.3.4/pyphetools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 pyphetools/creation/hpo_exact_cr.py
 pyphetools/creation/hpo_parser.py
 pyphetools/creation/individual.py
 pyphetools/creation/metadata.py
 pyphetools/creation/option_column_mapper.py
 pyphetools/creation/sex_column_mapper.py
 pyphetools/creation/simple_column_mapper.py
+pyphetools/creation/structural_variant.py
 pyphetools/creation/thresholded_column_mapper.py
 pyphetools/creation/variant.py
 pyphetools/creation/variant_column_mapper.py
 pyphetools/creation/variant_validator.py
 pyphetools/output/__init__.py
 pyphetools/output/detailed_suppl_table.py
 pyphetools/output/focus_count_table.py
@@ -48,14 +49,15 @@
 test/test_constant_column_mapper.py
 test/test_custom_column_mapper.py
 test/test_hp_term.py
 test/test_hpo_category.py
 test/test_hpo_cr.py
 test/test_hpo_parser.py
 test/test_option_column_mapper.py
+test/test_structural_variant.py
 test/test_threshold_column_mapper.py
 test/test_variant.py
 venv/bin/rst2html.py
 venv/bin/rst2html4.py
 venv/bin/rst2html5.py
 venv/bin/rst2latex.py
 venv/bin/rst2man.py
```

### Comparing `pyphetools-0.3.3/pyproject.toml` & `pyphetools-0.3.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 exclude = ["notebooks", "test"]
 
 [project]
 name = "pyphetools"
-version = "0.3.3"
+version = "0.3.4"
 requires-python = ">=3.5"
 description = "Generate and work with GA4GH phenopackets"
 readme = "README.md"
 authors = [
     {name = "Peter Robinson", email="peter.robinson@jax.org"},
      ]
 license = { file = "LICENSE" }
@@ -35,15 +35,16 @@
     "hpo-toolkit>=0.2.0",
     "openpyxl",
     "pandas",
     "phenopackets",
     "protobuf",
     "requests"
 ]
-
+[project.optional-dependencies]
+test = ["pytest"]
 
 
 
 #[project.optional-dependencies]
 #dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
```

### Comparing `pyphetools-0.3.3/test/test_age_column_mapper.py` & `pyphetools-0.3.4/test/test_age_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/test/test_case_encoder.py` & `pyphetools-0.3.4/test/test_case_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/test/test_column_mapper.py` & `pyphetools-0.3.4/test/test_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/test/test_constant_column_mapper.py` & `pyphetools-0.3.4/test/test_constant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/test/test_custom_column_mapper.py` & `pyphetools-0.3.4/test/test_custom_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/test/test_hp_term.py` & `pyphetools-0.3.4/test/test_hp_term.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/test/test_hpo_category.py` & `pyphetools-0.3.4/test/test_hpo_category.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/test/test_hpo_cr.py` & `pyphetools-0.3.4/test/test_hpo_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/test/test_option_column_mapper.py` & `pyphetools-0.3.4/test/test_option_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/test/test_threshold_column_mapper.py` & `pyphetools-0.3.4/test/test_threshold_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/test/test_variant.py` & `pyphetools-0.3.4/test/test_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/venv/bin/rst2html.py` & `pyphetools-0.3.4/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/venv/bin/rst2html4.py` & `pyphetools-0.3.4/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/venv/bin/rst2html5.py` & `pyphetools-0.3.4/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/venv/bin/rst2latex.py` & `pyphetools-0.3.4/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/venv/bin/rst2man.py` & `pyphetools-0.3.4/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/venv/bin/rst2odt.py` & `pyphetools-0.3.4/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/venv/bin/rst2odt_prepstyles.py` & `pyphetools-0.3.4/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/venv/bin/rst2pseudoxml.py` & `pyphetools-0.3.4/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/venv/bin/rst2s5.py` & `pyphetools-0.3.4/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/venv/bin/rst2xetex.py` & `pyphetools-0.3.4/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/venv/bin/rst2xml.py` & `pyphetools-0.3.4/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.3/venv/bin/rstpep2html.py` & `pyphetools-0.3.4/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

