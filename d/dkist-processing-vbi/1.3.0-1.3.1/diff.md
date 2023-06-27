# Comparing `tmp/dkist_processing_vbi-1.3.0.tar.gz` & `tmp/dkist_processing_vbi-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_processing_vbi-1.3.0.tar", last modified: Wed May 17 23:50:16 2023, max compression
+gzip compressed data, was "dkist_processing_vbi-1.3.1.tar", last modified: Tue Jun 27 16:36:39 2023, max compression
```

## Comparing `dkist_processing_vbi-1.3.0.tar` & `dkist_processing_vbi-1.3.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 23:50:16.661265 dkist_processing_vbi-1.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     9868 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     6298 2023-05-17 23:50:16.661265 dkist_processing_vbi-1.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5696 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/SCIENCE_CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     3425 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 23:50:16.653265 dkist_processing_vbi-1.3.0/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 23:50:16.653265 dkist_processing_vbi-1.3.0/dkist_processing_vbi/
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 23:50:16.657265 dkist_processing_vbi-1.3.0/dkist_processing_vbi/models/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1512 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/models/filter.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 23:50:16.657265 dkist_processing_vbi-1.3.0/dkist_processing_vbi/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6939 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/parsers/mosaic_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     1144 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/parsers/vbi_l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/parsers/vbi_l1_fits_access.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 23:50:16.657265 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3008 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     4436 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/dark.py
--rw-rw-rw-   0 root         (0) root         (0)     6462 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/gain.py
--rw-rw-rw-   0 root         (0) root         (0)    13848 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/make_movie_frames.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 23:50:16.657265 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2141 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)     2665 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     2185 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/process_summit_processed.py
--rw-rw-rw-   0 root         (0) root         (0)     2224 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     5607 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/science.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/vbi_base.py
--rw-rw-rw-   0 root         (0) root         (0)     5013 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 23:50:16.661265 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9497 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    12936 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/grogu_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2437 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     4711 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_dark.py
--rw-rw-rw-   0 root         (0) root         (0)     4261 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_gain.py
--rw-rw-rw-   0 root         (0) root         (0)     3704 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_intermediate_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)    10054 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    12628 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_parse_l0.py
--rw-rw-rw-   0 root         (0) root         (0)     5518 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_parse_summit.py
--rw-rw-rw-   0 root         (0) root         (0)     8313 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_process_summit.py
--rw-rw-rw-   0 root         (0) root         (0)     2339 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     6722 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_science.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_vbi_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1332 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_vbi_constants.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     4746 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 23:50:16.661265 dkist_processing_vbi-1.3.0/dkist_processing_vbi/workflows/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2966 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/workflows/l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)     2787 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi/workflows/summit_data_processing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 23:50:16.657265 dkist_processing_vbi-1.3.0/dkist_processing_vbi.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6298 2023-05-17 23:50:16.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2574 2023-05-17 23:50:16.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-17 23:50:16.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-05-17 23:50:16.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-17 23:50:16.000000 dkist_processing_vbi-1.3.0/dkist_processing_vbi.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 23:50:16.661265 dkist_processing_vbi-1.3.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2026 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      655 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/docs/l0_to_l1_vbi_no-speckle.rst
--rw-rw-rw-   0 root         (0) root         (0)      613 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/docs/l0_to_l1_vbi_summit-calibrated.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      291 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/docs/requirements_table.rst
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/docs/scientific_changelog.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 23:50:16.661265 dkist_processing_vbi-1.3.0/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       60 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/science_towncrier.sh
--rw-rw-rw-   0 root         (0) root         (0)     1603 2023-05-17 23:50:16.665265 dkist_processing_vbi-1.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-05-17 23:50:08.000000 dkist_processing_vbi-1.3.0/towncrier_science.toml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 16:36:39.862444 dkist_processing_vbi-1.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    10126 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6298 2023-06-27 16:36:39.862444 dkist_processing_vbi-1.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5696 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/SCIENCE_CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3425 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 16:36:39.854444 dkist_processing_vbi-1.3.1/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 16:36:39.854444 dkist_processing_vbi-1.3.1/dkist_processing_vbi/
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 16:36:39.854444 dkist_processing_vbi-1.3.1/dkist_processing_vbi/models/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1512 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/models/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/models/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 16:36:39.854444 dkist_processing_vbi-1.3.1/dkist_processing_vbi/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6939 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/parsers/mosaic_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     1144 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/parsers/vbi_l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/parsers/vbi_l1_fits_access.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 16:36:39.858444 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3008 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     4436 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     6462 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/gain.py
+-rw-rw-rw-   0 root         (0) root         (0)    13834 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/make_movie_frames.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 16:36:39.858444 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2135 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)     2665 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2185 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/process_summit_processed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2224 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     5607 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/science.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/vbi_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5013 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 16:36:39.858444 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9497 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    12936 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/grogu_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2437 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     4708 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     4261 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_gain.py
+-rw-rw-rw-   0 root         (0) root         (0)     3704 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_intermediate_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)    10051 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    12628 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_parse_l0.py
+-rw-rw-rw-   0 root         (0) root         (0)     5518 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_parse_summit.py
+-rw-rw-rw-   0 root         (0) root         (0)     8313 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_process_summit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2339 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     6722 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_vbi_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_vbi_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     4746 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 16:36:39.858444 dkist_processing_vbi-1.3.1/dkist_processing_vbi/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2966 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/workflows/l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2787 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi/workflows/summit_data_processing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 16:36:39.854444 dkist_processing_vbi-1.3.1/dkist_processing_vbi.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6298 2023-06-27 16:36:39.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2574 2023-06-27 16:36:39.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-27 16:36:39.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      528 2023-06-27 16:36:39.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-27 16:36:39.000000 dkist_processing_vbi-1.3.1/dkist_processing_vbi.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 16:36:39.858444 dkist_processing_vbi-1.3.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2026 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      655 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/docs/l0_to_l1_vbi_no-speckle.rst
+-rw-rw-rw-   0 root         (0) root         (0)      613 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/docs/l0_to_l1_vbi_summit-calibrated.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/docs/requirements_table.rst
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/docs/scientific_changelog.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 16:36:39.862444 dkist_processing_vbi-1.3.1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       60 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/science_towncrier.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-06-27 16:36:39.862444 dkist_processing_vbi-1.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-06-27 16:36:34.000000 dkist_processing_vbi-1.3.1/towncrier_science.toml
```

### Comparing `dkist_processing_vbi-1.3.0/.gitignore` & `dkist_processing_vbi-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/.pre-commit-config.yaml` & `dkist_processing_vbi-1.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/CHANGELOG.rst` & `dkist_processing_vbi-1.3.1/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v1.3.1 (2023-06-27)
+===================
+
+Misc
+----
+
+- Update to support `dkist-processing-common` 3.0.0. Specifically the new signature of some of the `FitsDataMixin` methods. (`#47 <https://bitbucket.org/dkistdc/dkist-processing-vbi/pull-requests/47>`__)
+
+
 v1.3.0 (2023-05-17)
 ===================
 
 Misc
 ----
 
 - Bumping common to 2.7.0: ParseL0InputData --> ParseL0InputDataBase, constant_flowers --> constant_buds (`#46 <https://bitbucket.org/dkistdc/dkist-processing-vbi/pull-requests/46>`__)
```

### Comparing `dkist_processing_vbi-1.3.0/PKG-INFO` & `dkist_processing_vbi-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_processing_vbi
-Version: 1.3.0
+Version: 1.3.1
 Summary: Code that is used by the DKIST Science Data Processing Airflow pipelines to process VBI data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-vbi/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/vbi
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_vbi-1.3.0/README.rst` & `dkist_processing_vbi-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/bitbucket-pipelines.yml` & `dkist_processing_vbi-1.3.1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/check_changelog_updated.sh` & `dkist_processing_vbi-1.3.1/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/models/constants.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/models/filter.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/models/filter.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/models/tags.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/parsers/mosaic_repeats.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/parsers/mosaic_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/parsers/vbi_l0_fits_access.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/parsers/vbi_l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/parsers/vbi_l1_fits_access.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/parsers/vbi_l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/assemble_movie.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/dark.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/gain.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/gain.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/make_movie_frames.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/make_movie_frames.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                         VbiTag.spatial_step(step),
                         VbiTag.mosaic(mosaic),
                     ]
                 )
 
                 # We're doing it with a list right now to save having to construct a second generator just to get
                 # the first header. This may need to change if LOTS of exposures are taken.
-                output_hdus = [tup[1] for tup in output_hdu_generator]
+                output_hdus = list(output_hdu_generator)
                 # We're still keeping the data access in a generator, though
                 output_arrays = (h.data for h in output_hdus)
                 averaged_frame = average_numpy_arrays(output_arrays)
                 first_header = output_hdus[0].header
 
                 logger.info(f"writing averaged data for {apm_str}")
                 self.fits_data_write(
```

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         -------
         Generator:
             Generator of loaded intermediate arrays
 
         """
         if VbiTag.intermediate() not in tags:
             tags += [VbiTag.intermediate()]
-        for path, hdu in self.fits_data_read_hdu(tags=tags):
+        for hdu in self.fits_data_read_hdu(tags=tags):
             yield hdu.data
 
     def intermediate_dark_array(self, spatial_step: int, exposure_time: float) -> np.ndarray:
         """
         Load intermediate dark array for a single spatial step and exposure time.
 
         Parameters
```

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/parse.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/process_summit_processed.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/process_summit_processed.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/quality_metrics.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/science.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/vbi_base.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/vbi_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tasks/write_l1.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/conftest.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/grogu_test.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/grogu_test.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_assemble_movie.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_dark.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_dark.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                         VbiTag.spatial_step(p),
                         VbiTag.exposure_time(exp),
                     ]
                 )
             )
             assert len(hdu_list) == 1
             expected_array = np.ones((10, 10)) * 2 * 10.0**p * exp * 10
-            np.testing.assert_equal(expected_array, hdu_list[0][1].data)
+            np.testing.assert_equal(expected_array, hdu_list[0].data)
 
     unused_time_read = dark_calibration_task.read(
         tags=[
             VbiTag.task("DARK"),
             VbiTag.intermediate(),
             VbiTag.frame(),
             VbiTag.exposure_time(dark_calibration_task.unused_time),
```

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_gain.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_gain.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_intermediate_loaders.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_intermediate_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_make_movie_frames.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_make_movie_frames.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
                         VbiTag.task("AVG_MOVIE_FRAME"),
                         VbiTag.spatial_step(s),
                         VbiTag.mosaic(m),
                     ]
                 )
             )
             assert len(hdus) == 1
-            data = hdus[0][1].data
+            data = hdus[0].data
             expected = np.ones((10, 10)) * (s + m - 1)
             np.testing.assert_equal(data, expected)
 
 
 def test_find_ref_pos(make_movie_frames_task_with_averages):
     access_list = list(
         make_movie_frames_task_with_averages.fits_data_read_fits_access(
```

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_parse_l0.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_parse_l0.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_parse_summit.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_parse_summit.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_process_summit.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_process_summit.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_quality_metrics.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_science.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_vbi_base.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_vbi_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_vbi_constants.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_vbi_constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/tests/test_write_l1.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/workflows/l0_processing.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/workflows/l0_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi/workflows/summit_data_processing.py` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi/workflows/summit_data_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi.egg-info/PKG-INFO` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-vbi
-Version: 1.3.0
+Version: 1.3.1
 Summary: Code that is used by the DKIST Science Data Processing Airflow pipelines to process VBI data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-vbi/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/vbi
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi.egg-info/SOURCES.txt` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/dkist_processing_vbi.egg-info/requires.txt` & `dkist_processing_vbi-1.3.1/dkist_processing_vbi.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-dkist-processing-common==2.7.0
+dkist-processing-common==3.0.0
 dkist-processing-math==1.0.1
 dkist-header-validator==3.0.5
 dkist-fits-specifications==3.6.0
 astropy==5.1.1
 numpy==1.23.1
 sunpy==4.1.4
 scipy==1.9.0
@@ -18,15 +18,14 @@
 sphinx-autoapi
 pytest
 towncrier==22.12.0
 dkist-sphinx-theme
 
 [grogu]
 dkist==1.0.0b11
-asdf==2.10.1
 pyparsing
 dkist-inventory==0.16.0
 parfive<2.0.0
 
 [test]
 pytest
 pytest-cov
```

### Comparing `dkist_processing_vbi-1.3.0/docs/Makefile` & `dkist_processing_vbi-1.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/docs/conf.py` & `dkist_processing_vbi-1.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/docs/l0_to_l1_vbi_no-speckle.rst` & `dkist_processing_vbi-1.3.1/docs/l0_to_l1_vbi_no-speckle.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/docs/l0_to_l1_vbi_summit-calibrated.rst` & `dkist_processing_vbi-1.3.1/docs/l0_to_l1_vbi_summit-calibrated.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/docs/make.bat` & `dkist_processing_vbi-1.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/licenses/LICENSE.rst` & `dkist_processing_vbi-1.3.1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/pyproject.toml` & `dkist_processing_vbi-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.3.0/setup.cfg` & `dkist_processing_vbi-1.3.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [options]
 python_requires = >=3.10
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	dkist-processing-common == 2.7.0
+	dkist-processing-common == 3.0.0
 	dkist-processing-math == 1.0.1
 	dkist-header-validator == 3.0.5
 	dkist-fits-specifications == 3.6.0
 	astropy == 5.1.1
 	numpy == 1.23.1
 	sunpy == 4.1.4
 	scipy == 1.9.0
@@ -38,15 +38,14 @@
 	pytest-cov
 	pytest-mock
 	pytest-xdist
 	towncrier
 	dkist-data-simulator >= 2.1.0
 grogu = 
 	dkist == 1.0.0b11
-	asdf == 2.10.1
 	pyparsing
 	dkist-inventory == 0.16.0
 	parfive < 2.0.0
 docs = 
 	sphinx
 	sphinx-astropy
 	sphinx-changelog == 1.3.0
```

