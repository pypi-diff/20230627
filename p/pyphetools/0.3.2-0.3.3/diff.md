# Comparing `tmp/pyphetools-0.3.2.tar.gz` & `tmp/pyphetools-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphetools-0.3.2.tar", last modified: Mon Jun 26 12:02:34 2023, max compression
+gzip compressed data, was "pyphetools-0.3.3.tar", last modified: Mon Jun 26 23:11:11 2023, max compression
```

## Comparing `pyphetools-0.3.2.tar` & `pyphetools-0.3.3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 12:02:34.709173 pyphetools-0.3.2/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1079 2023-02-05 19:04:48.000000 pyphetools-0.3.2/LICENSE
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-12-16 00:09:56.000000 pyphetools-0.3.2/MANIFEST.in
--rw-rw-r--   0 peter     (1000) peter     (1000)     2658 2023-06-26 12:02:34.709173 pyphetools-0.3.2/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      600 2023-05-14 17:49:44.000000 pyphetools-0.3.2/README.md
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 12:02:34.169176 pyphetools-0.3.2/docs/
--rw-rw-r--   0 peter     (1000) peter     (1000)     4165 2023-06-25 22:31:24.000000 pyphetools-0.3.2/docs/conf.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 12:02:34.181176 pyphetools-0.3.2/pyphetools/
--rw-rw-r--   0 peter     (1000) peter     (1000)       11 2023-02-05 19:04:48.000000 pyphetools-0.3.2/pyphetools/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 12:02:34.205175 pyphetools-0.3.2/pyphetools/analyze/
--rw-rw-r--   0 peter     (1000) peter     (1000)       36 2023-02-05 19:04:48.000000 pyphetools-0.3.2/pyphetools/analyze/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3062 2023-06-25 22:31:24.000000 pyphetools-0.3.2/pyphetools/analyze/downsampler.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 12:02:34.505174 pyphetools-0.3.2/pyphetools/creation/
--rw-rw-r--   0 peter     (1000) peter     (1000)      794 2023-05-12 21:54:20.000000 pyphetools-0.3.2/pyphetools/creation/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4873 2023-05-11 10:59:47.000000 pyphetools-0.3.2/pyphetools/creation/age_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6558 2023-06-25 20:28:58.000000 pyphetools-0.3.2/pyphetools/creation/case_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     9043 2023-06-25 22:31:24.000000 pyphetools-0.3.2/pyphetools/creation/cohort_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      531 2023-05-10 19:30:33.000000 pyphetools-0.3.2/pyphetools/creation/column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2339 2023-06-25 22:31:24.000000 pyphetools-0.3.2/pyphetools/creation/constant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      308 2023-05-07 14:22:13.000000 pyphetools-0.3.2/pyphetools/creation/constants.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3014 2023-05-11 13:07:39.000000 pyphetools-0.3.2/pyphetools/creation/custom_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3281 2023-06-25 20:29:31.000000 pyphetools-0.3.2/pyphetools/creation/hp_term.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      740 2023-05-11 10:59:47.000000 pyphetools-0.3.2/pyphetools/creation/hpo_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7110 2023-05-11 11:50:47.000000 pyphetools-0.3.2/pyphetools/creation/hpo_exact_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6248 2023-06-25 22:31:24.000000 pyphetools-0.3.2/pyphetools/creation/hpo_parser.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7382 2023-06-25 22:44:11.000000 pyphetools-0.3.2/pyphetools/creation/individual.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5795 2023-06-25 22:31:24.000000 pyphetools-0.3.2/pyphetools/creation/metadata.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3541 2023-06-26 12:01:47.000000 pyphetools-0.3.2/pyphetools/creation/option_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2194 2023-05-17 14:42:11.000000 pyphetools-0.3.2/pyphetools/creation/sex_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4678 2023-05-13 00:28:58.000000 pyphetools-0.3.2/pyphetools/creation/simple_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2656 2023-05-11 11:04:54.000000 pyphetools-0.3.2/pyphetools/creation/thresholded_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4976 2023-06-25 17:17:47.000000 pyphetools-0.3.2/pyphetools/creation/variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4514 2023-05-11 20:00:55.000000 pyphetools-0.3.2/pyphetools/creation/variant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3229 2023-05-11 10:59:47.000000 pyphetools-0.3.2/pyphetools/creation/variant_validator.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 12:02:34.601173 pyphetools-0.3.2/pyphetools/output/
--rw-rw-r--   0 peter     (1000) peter     (1000)      327 2023-06-24 19:26:58.000000 pyphetools-0.3.2/pyphetools/output/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3067 2023-06-25 22:31:24.000000 pyphetools-0.3.2/pyphetools/output/detailed_suppl_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5727 2023-06-25 22:31:24.000000 pyphetools-0.3.2/pyphetools/output/focus_count_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2980 2023-02-05 19:04:49.000000 pyphetools-0.3.2/pyphetools/output/hpo_category.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      894 2023-02-05 19:04:49.000000 pyphetools-0.3.2/pyphetools/output/phenopacket_ingestor.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2154 2023-06-24 20:06:45.000000 pyphetools-0.3.2/pyphetools/output/phenopacket_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4960 2023-06-24 20:15:49.000000 pyphetools-0.3.2/pyphetools/output/simple_patient.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3310 2023-06-24 20:23:41.000000 pyphetools-0.3.2/pyphetools/output/simple_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      569 2023-05-11 10:59:47.000000 pyphetools-0.3.2/pyphetools/output/term_count.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 12:02:34.617173 pyphetools-0.3.2/pyphetools/validation/
--rw-rw-r--   0 peter     (1000) peter     (1000)        8 2023-06-25 22:31:24.000000 pyphetools-0.3.2/pyphetools/validation/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 12:02:34.193175 pyphetools-0.3.2/pyphetools.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)     2658 2023-06-26 12:02:34.000000 pyphetools-0.3.2/pyphetools.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     2083 2023-06-26 12:02:34.000000 pyphetools-0.3.2/pyphetools.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-06-26 12:02:34.000000 pyphetools-0.3.2/pyphetools.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       66 2023-06-26 12:02:34.000000 pyphetools-0.3.2/pyphetools.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       50 2023-06-26 12:02:34.000000 pyphetools-0.3.2/pyphetools.egg-info/top_level.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)     1318 2023-06-26 11:52:33.000000 pyphetools-0.3.2/pyproject.toml
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-06-26 12:02:34.709173 pyphetools-0.3.2/setup.cfg
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 12:02:34.669173 pyphetools-0.3.2/test/
--rw-rw-r--   0 peter     (1000) peter     (1000)     3297 2023-02-05 19:04:49.000000 pyphetools-0.3.2/test/test_age_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2956 2023-05-11 10:59:47.000000 pyphetools-0.3.2/test/test_case_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4553 2023-05-10 22:56:45.000000 pyphetools-0.3.2/test/test_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1156 2023-05-12 23:59:19.000000 pyphetools-0.3.2/test/test_constant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2745 2023-05-14 12:05:29.000000 pyphetools-0.3.2/test/test_custom_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1430 2023-06-23 21:44:02.000000 pyphetools-0.3.2/test/test_hp_term.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      914 2023-02-05 19:04:49.000000 pyphetools-0.3.2/test/test_hpo_category.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5966 2023-05-11 14:18:42.000000 pyphetools-0.3.2/test/test_hpo_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      439 2023-02-05 19:04:49.000000 pyphetools-0.3.2/test/test_hpo_parser.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5385 2023-06-26 12:00:47.000000 pyphetools-0.3.2/test/test_option_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1856 2023-05-11 14:18:42.000000 pyphetools-0.3.2/test/test_threshold_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1439 2023-05-11 14:18:42.000000 pyphetools-0.3.2/test/test_variant.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 12:02:34.169176 pyphetools-0.3.2/venv/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 12:02:34.709173 pyphetools-0.3.2/venv/bin/
--rwxrwxr-x   0 peter     (1000) peter     (1000)      621 2022-12-06 12:58:50.000000 pyphetools-0.3.2/venv/bin/rst2html.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      741 2022-12-06 12:58:50.000000 pyphetools-0.3.2/venv/bin/rst2html4.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1109 2022-12-06 12:58:50.000000 pyphetools-0.3.2/venv/bin/rst2html5.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      818 2022-12-06 12:58:50.000000 pyphetools-0.3.2/venv/bin/rst2latex.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      626 2022-12-06 12:58:50.000000 pyphetools-0.3.2/venv/bin/rst2man.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      791 2022-12-06 12:58:50.000000 pyphetools-0.3.2/venv/bin/rst2odt.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1753 2022-12-06 12:58:50.000000 pyphetools-0.3.2/venv/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      628 2022-12-06 12:58:50.000000 pyphetools-0.3.2/venv/bin/rst2pseudoxml.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      664 2022-12-06 12:58:50.000000 pyphetools-0.3.2/venv/bin/rst2s5.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      898 2022-12-06 12:58:50.000000 pyphetools-0.3.2/venv/bin/rst2xetex.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      629 2022-12-06 12:58:50.000000 pyphetools-0.3.2/venv/bin/rst2xml.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      697 2022-12-06 12:58:50.000000 pyphetools-0.3.2/venv/bin/rstpep2html.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.370327 pyphetools-0.3.3/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1079 2023-02-05 19:04:48.000000 pyphetools-0.3.3/LICENSE
+-rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-12-16 00:09:56.000000 pyphetools-0.3.3/MANIFEST.in
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2825 2023-06-26 23:11:11.370327 pyphetools-0.3.3/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      767 2023-06-26 23:11:02.000000 pyphetools-0.3.3/README.md
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.254326 pyphetools-0.3.3/docs/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4165 2023-06-25 22:31:24.000000 pyphetools-0.3.3/docs/conf.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.254326 pyphetools-0.3.3/pyphetools/
+-rw-rw-r--   0 peter     (1000) peter     (1000)       11 2023-02-05 19:04:48.000000 pyphetools-0.3.3/pyphetools/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.254326 pyphetools-0.3.3/pyphetools/analyze/
+-rw-rw-r--   0 peter     (1000) peter     (1000)       36 2023-02-05 19:04:48.000000 pyphetools-0.3.3/pyphetools/analyze/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3062 2023-06-25 22:31:24.000000 pyphetools-0.3.3/pyphetools/analyze/downsampler.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.258326 pyphetools-0.3.3/pyphetools/creation/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      794 2023-05-12 21:54:20.000000 pyphetools-0.3.3/pyphetools/creation/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4873 2023-05-11 10:59:47.000000 pyphetools-0.3.3/pyphetools/creation/age_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6558 2023-06-25 20:28:58.000000 pyphetools-0.3.3/pyphetools/creation/case_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     9043 2023-06-25 22:31:24.000000 pyphetools-0.3.3/pyphetools/creation/cohort_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      531 2023-05-10 19:30:33.000000 pyphetools-0.3.3/pyphetools/creation/column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2339 2023-06-25 22:31:24.000000 pyphetools-0.3.3/pyphetools/creation/constant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      308 2023-05-07 14:22:13.000000 pyphetools-0.3.3/pyphetools/creation/constants.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3014 2023-05-11 13:07:39.000000 pyphetools-0.3.3/pyphetools/creation/custom_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3281 2023-06-25 20:29:31.000000 pyphetools-0.3.3/pyphetools/creation/hp_term.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      740 2023-05-11 10:59:47.000000 pyphetools-0.3.3/pyphetools/creation/hpo_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7110 2023-05-11 11:50:47.000000 pyphetools-0.3.3/pyphetools/creation/hpo_exact_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6248 2023-06-25 22:31:24.000000 pyphetools-0.3.3/pyphetools/creation/hpo_parser.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7382 2023-06-25 22:44:11.000000 pyphetools-0.3.3/pyphetools/creation/individual.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5795 2023-06-25 22:31:24.000000 pyphetools-0.3.3/pyphetools/creation/metadata.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3541 2023-06-26 12:01:47.000000 pyphetools-0.3.3/pyphetools/creation/option_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2194 2023-05-17 14:42:11.000000 pyphetools-0.3.3/pyphetools/creation/sex_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4678 2023-05-13 00:28:58.000000 pyphetools-0.3.3/pyphetools/creation/simple_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2656 2023-05-11 11:04:54.000000 pyphetools-0.3.3/pyphetools/creation/thresholded_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4976 2023-06-25 17:17:47.000000 pyphetools-0.3.3/pyphetools/creation/variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4714 2023-06-26 23:11:02.000000 pyphetools-0.3.3/pyphetools/creation/variant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3229 2023-05-11 10:59:47.000000 pyphetools-0.3.3/pyphetools/creation/variant_validator.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.258326 pyphetools-0.3.3/pyphetools/output/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      327 2023-06-24 19:26:58.000000 pyphetools-0.3.3/pyphetools/output/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3067 2023-06-25 22:31:24.000000 pyphetools-0.3.3/pyphetools/output/detailed_suppl_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5727 2023-06-25 22:31:24.000000 pyphetools-0.3.3/pyphetools/output/focus_count_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2980 2023-02-05 19:04:49.000000 pyphetools-0.3.3/pyphetools/output/hpo_category.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      894 2023-02-05 19:04:49.000000 pyphetools-0.3.3/pyphetools/output/phenopacket_ingestor.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2154 2023-06-24 20:06:45.000000 pyphetools-0.3.3/pyphetools/output/phenopacket_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4960 2023-06-24 20:15:49.000000 pyphetools-0.3.3/pyphetools/output/simple_patient.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3310 2023-06-24 20:23:41.000000 pyphetools-0.3.3/pyphetools/output/simple_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      569 2023-05-11 10:59:47.000000 pyphetools-0.3.3/pyphetools/output/term_count.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.258326 pyphetools-0.3.3/pyphetools/validation/
+-rw-rw-r--   0 peter     (1000) peter     (1000)        8 2023-06-25 22:31:24.000000 pyphetools-0.3.3/pyphetools/validation/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.254326 pyphetools-0.3.3/pyphetools.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2825 2023-06-26 23:11:11.000000 pyphetools-0.3.3/pyphetools.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2083 2023-06-26 23:11:11.000000 pyphetools-0.3.3/pyphetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-06-26 23:11:11.000000 pyphetools-0.3.3/pyphetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       66 2023-06-26 23:11:11.000000 pyphetools-0.3.3/pyphetools.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       50 2023-06-26 23:11:11.000000 pyphetools-0.3.3/pyphetools.egg-info/top_level.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1318 2023-06-26 23:11:02.000000 pyphetools-0.3.3/pyproject.toml
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-06-26 23:11:11.370327 pyphetools-0.3.3/setup.cfg
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.262326 pyphetools-0.3.3/test/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3297 2023-02-05 19:04:49.000000 pyphetools-0.3.3/test/test_age_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2956 2023-05-11 10:59:47.000000 pyphetools-0.3.3/test/test_case_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4553 2023-05-10 22:56:45.000000 pyphetools-0.3.3/test/test_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1156 2023-05-12 23:59:19.000000 pyphetools-0.3.3/test/test_constant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2745 2023-05-14 12:05:29.000000 pyphetools-0.3.3/test/test_custom_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1430 2023-06-23 21:44:02.000000 pyphetools-0.3.3/test/test_hp_term.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      914 2023-02-05 19:04:49.000000 pyphetools-0.3.3/test/test_hpo_category.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5966 2023-05-11 14:18:42.000000 pyphetools-0.3.3/test/test_hpo_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      439 2023-02-05 19:04:49.000000 pyphetools-0.3.3/test/test_hpo_parser.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5385 2023-06-26 12:00:47.000000 pyphetools-0.3.3/test/test_option_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1856 2023-05-11 14:18:42.000000 pyphetools-0.3.3/test/test_threshold_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1439 2023-05-11 14:18:42.000000 pyphetools-0.3.3/test/test_variant.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.254326 pyphetools-0.3.3/venv/
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-26 23:11:11.370327 pyphetools-0.3.3/venv/bin/
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      621 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2html.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      741 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2html4.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1109 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2html5.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      818 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2latex.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      626 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2man.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      791 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2odt.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1753 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      628 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      664 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2s5.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      898 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2xetex.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      629 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rst2xml.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      697 2022-12-06 12:58:50.000000 pyphetools-0.3.3/venv/bin/rstpep2html.py
```

### Comparing `pyphetools-0.3.2/LICENSE` & `pyphetools-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/PKG-INFO` & `pyphetools-0.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.3.2
+Version: 0.3.3
 Summary: Generate and work with GA4GH phenopackets
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,14 +32,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![CI](https://github.com/monarch-initiative/genophenocorr/workflows/CI/badge.svg)](https://github.com/monarch-initiative/pyphetools/actions/workflows/python_ci.yml)
+
 # pyphetools
 Python Phenopacket Tools
 
 This package currently is designed to test how to use the Python version of the phenopackets package together with pandas to create phenopackets from typical supplemental tables.
 
 Development goals include making builder code similar to the Java package to create valid phenopackets and to perform JSON Schema-based validation.
```

### Comparing `pyphetools-0.3.2/docs/conf.py` & `pyphetools-0.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/analyze/downsampler.py` & `pyphetools-0.3.3/pyphetools/analyze/downsampler.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/creation/__init__.py` & `pyphetools-0.3.3/pyphetools/creation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/creation/age_column_mapper.py` & `pyphetools-0.3.3/pyphetools/creation/age_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/creation/case_encoder.py` & `pyphetools-0.3.3/pyphetools/creation/case_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/creation/cohort_encoder.py` & `pyphetools-0.3.3/pyphetools/creation/cohort_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/creation/column_mapper.py` & `pyphetools-0.3.3/pyphetools/creation/column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/creation/constant_column_mapper.py` & `pyphetools-0.3.3/pyphetools/creation/constant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/creation/custom_column_mapper.py` & `pyphetools-0.3.3/pyphetools/creation/custom_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/creation/hp_term.py` & `pyphetools-0.3.3/pyphetools/creation/hp_term.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/creation/hpo_cr.py` & `pyphetools-0.3.3/pyphetools/creation/hpo_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/creation/hpo_exact_cr.py` & `pyphetools-0.3.3/pyphetools/creation/hpo_exact_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/creation/hpo_parser.py` & `pyphetools-0.3.3/pyphetools/creation/hpo_parser.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/creation/individual.py` & `pyphetools-0.3.3/pyphetools/creation/individual.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/creation/metadata.py` & `pyphetools-0.3.3/pyphetools/creation/metadata.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/creation/option_column_mapper.py` & `pyphetools-0.3.3/pyphetools/creation/option_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/creation/sex_column_mapper.py` & `pyphetools-0.3.3/pyphetools/creation/sex_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/creation/simple_column_mapper.py` & `pyphetools-0.3.3/pyphetools/creation/simple_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/creation/thresholded_column_mapper.py` & `pyphetools-0.3.3/pyphetools/creation/thresholded_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/creation/variant.py` & `pyphetools-0.3.3/pyphetools/creation/variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/creation/variant_column_mapper.py` & `pyphetools-0.3.3/pyphetools/creation/variant_column_mapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,24 +46,29 @@
                     v.set_genotype(self._default_genotype)
                 results.extend(variant_list)
             else:
                 try:
                     variant = self._validator.encode_hgvs(item)
                     if genotype_contents is not None:
                         if 'hom' in genotype_contents.lower():
-                            variant.set_genotype('homozygous')
+                            variant.set_homozygous()
                         elif 'het' in genotype_contents.lower():
-                            variant.set_genotype('heterozygous')
+                            variant.set_heterozygous()
                         elif 'hemi' in genotype_contents.lower():
-                            variant.set_genotype('hemizygous')
-                        elif self._default_genotype is not None:
-                            variant.set_genotype(self._default_genotype)
-                    else:
-                        if self._default_genotype is not None:
-                            variant.set_genotype(self._default_genotype)
+                            variant.set_hemizygous()
+                        else:
+                            print(f"Did not recognize genotype {genotype_contents}")
+                    elif self._default_genotype is not None:
+                        def_gt = self._default_genotype
+                        if 'hom' in def_gt:
+                            variant.set_homozygous()
+                        elif 'het' in def_gt:
+                            variant.set_heterozygous()
+                        elif 'hemi' in def_gt:
+                            variant.set_hemizygous()
                     results.append(variant)
                 except Exception as exc:
                     print(f"Not able to get variant for {item}: {exc}")
         return results
 
     def preview_column(self, column) -> pd.DataFrame:
         if not isinstance(column, pd.Series):
```

### Comparing `pyphetools-0.3.2/pyphetools/creation/variant_validator.py` & `pyphetools-0.3.3/pyphetools/creation/variant_validator.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/output/detailed_suppl_table.py` & `pyphetools-0.3.3/pyphetools/output/detailed_suppl_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/output/focus_count_table.py` & `pyphetools-0.3.3/pyphetools/output/focus_count_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/output/hpo_category.py` & `pyphetools-0.3.3/pyphetools/output/hpo_category.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/output/phenopacket_ingestor.py` & `pyphetools-0.3.3/pyphetools/output/phenopacket_ingestor.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/output/phenopacket_table.py` & `pyphetools-0.3.3/pyphetools/output/phenopacket_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/output/simple_patient.py` & `pyphetools-0.3.3/pyphetools/output/simple_patient.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/output/simple_variant.py` & `pyphetools-0.3.3/pyphetools/output/simple_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools/output/term_count.py` & `pyphetools-0.3.3/pyphetools/output/term_count.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyphetools.egg-info/PKG-INFO` & `pyphetools-0.3.3/pyphetools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.3.2
+Version: 0.3.3
 Summary: Generate and work with GA4GH phenopackets
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,14 +32,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![CI](https://github.com/monarch-initiative/genophenocorr/workflows/CI/badge.svg)](https://github.com/monarch-initiative/pyphetools/actions/workflows/python_ci.yml)
+
 # pyphetools
 Python Phenopacket Tools
 
 This package currently is designed to test how to use the Python version of the phenopackets package together with pandas to create phenopackets from typical supplemental tables.
 
 Development goals include making builder code similar to the Java package to create valid phenopackets and to perform JSON Schema-based validation.
```

### Comparing `pyphetools-0.3.2/pyphetools.egg-info/SOURCES.txt` & `pyphetools-0.3.3/pyphetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/pyproject.toml` & `pyphetools-0.3.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 exclude = ["notebooks", "test"]
 
 [project]
 name = "pyphetools"
-version = "0.3.2"
+version = "0.3.3"
 requires-python = ">=3.5"
 description = "Generate and work with GA4GH phenopackets"
 readme = "README.md"
 authors = [
     {name = "Peter Robinson", email="peter.robinson@jax.org"},
      ]
 license = { file = "LICENSE" }
```

### Comparing `pyphetools-0.3.2/test/test_age_column_mapper.py` & `pyphetools-0.3.3/test/test_age_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/test/test_case_encoder.py` & `pyphetools-0.3.3/test/test_case_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/test/test_column_mapper.py` & `pyphetools-0.3.3/test/test_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/test/test_constant_column_mapper.py` & `pyphetools-0.3.3/test/test_constant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/test/test_custom_column_mapper.py` & `pyphetools-0.3.3/test/test_custom_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/test/test_hp_term.py` & `pyphetools-0.3.3/test/test_hp_term.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/test/test_hpo_category.py` & `pyphetools-0.3.3/test/test_hpo_category.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/test/test_hpo_cr.py` & `pyphetools-0.3.3/test/test_hpo_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/test/test_option_column_mapper.py` & `pyphetools-0.3.3/test/test_option_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/test/test_threshold_column_mapper.py` & `pyphetools-0.3.3/test/test_threshold_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/test/test_variant.py` & `pyphetools-0.3.3/test/test_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/venv/bin/rst2html.py` & `pyphetools-0.3.3/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/venv/bin/rst2html4.py` & `pyphetools-0.3.3/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/venv/bin/rst2html5.py` & `pyphetools-0.3.3/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/venv/bin/rst2latex.py` & `pyphetools-0.3.3/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/venv/bin/rst2man.py` & `pyphetools-0.3.3/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/venv/bin/rst2odt.py` & `pyphetools-0.3.3/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/venv/bin/rst2odt_prepstyles.py` & `pyphetools-0.3.3/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/venv/bin/rst2pseudoxml.py` & `pyphetools-0.3.3/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/venv/bin/rst2s5.py` & `pyphetools-0.3.3/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/venv/bin/rst2xetex.py` & `pyphetools-0.3.3/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/venv/bin/rst2xml.py` & `pyphetools-0.3.3/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.3.2/venv/bin/rstpep2html.py` & `pyphetools-0.3.3/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

