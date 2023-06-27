# Comparing `tmp/dkist_processing_visp-2.3.1.tar.gz` & `tmp/dkist_processing_visp-2.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_processing_visp-2.3.1.tar", last modified: Thu Jun 15 16:50:48 2023, max compression
+gzip compressed data, was "dkist_processing_visp-2.4.0rc1.tar", last modified: Tue Jun 27 19:33:29 2023, max compression
```

## Comparing `dkist_processing_visp-2.3.1.tar` & `dkist_processing_visp-2.4.0rc1.tar`

### file list

```diff
@@ -1,109 +1,116 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.513040 dkist_processing_visp-2.3.1/
--rw-rw-rw-   0 root         (0) root         (0)     2461 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    20825 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     6213 2023-06-15 16:50:48.513040 dkist_processing_visp-2.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5645 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3652 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/SCIENCE_CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     3428 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.501040 dkist_processing_visp-2.3.1/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.501040 dkist_processing_visp-2.3.1/dkist_processing_visp/
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.501040 dkist_processing_visp-2.3.1/dkist_processing_visp/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/fonts/Lato-Regular.ttf
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.505040 dkist_processing_visp-2.3.1/dkist_processing_visp/models/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3440 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    11306 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.505040 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5370 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/polarimeter_mode.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/raster_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1869 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/visp_l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/visp_l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      843 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.505040 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3296 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    14365 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     4137 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/dark.py
--rw-rw-rw-   0 root         (0) root         (0)    40623 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    20011 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)      395 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5343 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     7068 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/make_movie_frames.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.505040 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5656 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/corrections.py
--rw-rw-rw-   0 root         (0) root         (0)     1343 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/downsample.py
--rw-rw-rw-   0 root         (0) root         (0)     7112 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)    10422 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     4604 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     7944 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    28173 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/science.py
--rw-rw-rw-   0 root         (0) root         (0)    27922 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6846 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.509040 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16332 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     6595 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/e2e_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    17553 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/e2e_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2514 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    18443 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     1171 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_build_quality_report.py
--rw-rw-rw-   0 root         (0) root         (0)     5272 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_dark.py
--rw-rw-rw-   0 root         (0) root         (0)     2173 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_downsample.py
--rw-rw-rw-   0 root         (0) root         (0)    14009 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    12613 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)     5651 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     4021 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    11818 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    16234 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_parse.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    19734 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_science.py
--rw-rw-rw-   0 root         (0) root         (0)     9883 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_submit_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     5097 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_visp_constants.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     5752 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.509040 dkist_processing_visp-2.3.1/dkist_processing_visp/workflows/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3280 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/workflows/l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/workflows/single_task_workflows.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.501040 dkist_processing_visp-2.3.1/dkist_processing_visp.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6213 2023-06-15 16:50:48.000000 dkist_processing_visp-2.3.1/dkist_processing_visp.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3605 2023-06-15 16:50:48.000000 dkist_processing_visp-2.3.1/dkist_processing_visp.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-15 16:50:48.000000 dkist_processing_visp-2.3.1/dkist_processing_visp.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-06-15 16:50:48.000000 dkist_processing_visp-2.3.1/dkist_processing_visp.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-15 16:50:48.000000 dkist_processing_visp-2.3.1/dkist_processing_visp.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.513040 dkist_processing_visp-2.3.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     4844 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/background_light.rst
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2028 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     6427 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/gain_correction.rst
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/l0_to_l1_visp.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     4995 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/polarization_calibration.rst
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/requirements_table.rst
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/science_calibration.rst
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/scientific_changelog.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.513040 dkist_processing_visp-2.3.1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       60 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/science_towncrier.sh
--rw-rw-rw-   0 root         (0) root         (0)     1705 2023-06-15 16:50:48.513040 dkist_processing_visp-2.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/towncrier_science.toml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:33:29.817840 dkist_processing_visp-2.4.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     2461 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    20545 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6216 2023-06-27 19:33:29.817840 dkist_processing_visp-2.4.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5645 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3652 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/SCIENCE_CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3428 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:33:29.785840 dkist_processing_visp-2.4.0rc1/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/changelog/116.feature.rst
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/changelog/117.misc.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:33:29.785840 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:33:29.785840 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/fonts/Lato-Regular.ttf
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:33:29.789840 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/models/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3440 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    11306 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/models/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:33:29.789840 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5370 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/parsers/map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/parsers/polarimeter_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/parsers/raster_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/parsers/visp_l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/parsers/visp_l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      843 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/parsers/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:33:29.801840 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3296 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    14744 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     4137 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/dark.py
+-rw-rw-rw-   0 root         (0) root         (0)    40558 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    20368 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5343 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7068 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/make_movie_frames.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:33:29.805840 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5656 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/mixin/corrections.py
+-rw-rw-rw-   0 root         (0) root         (0)     1343 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/mixin/downsample.py
+-rw-rw-rw-   0 root         (0) root         (0)     7112 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)    10506 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4604 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     7944 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    28173 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/science.py
+-rw-rw-rw-   0 root         (0) root         (0)    28801 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6846 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:33:29.809840 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16332 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:33:29.809840 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/local_trial_workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/local_trial_workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18994 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py
+-rw-rw-rw-   0 root         (0) root         (0)     8247 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    18443 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_build_quality_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     5272 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_downsample.py
+-rw-rw-rw-   0 root         (0) root         (0)    14009 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    12613 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)     5651 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    11818 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    16234 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    19734 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     9883 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_submit_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     5340 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5091 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_visp_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     5752 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:33:29.813840 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3280 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/workflows/l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/workflows/single_task_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     3574 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp/workflows/trial_workflows.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:33:29.785840 dkist_processing_visp-2.4.0rc1/dkist_processing_visp.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6216 2023-06-27 19:33:29.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3922 2023-06-27 19:33:29.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-27 19:33:29.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-06-27 19:33:29.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-27 19:33:29.000000 dkist_processing_visp-2.4.0rc1/dkist_processing_visp.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:33:29.813840 dkist_processing_visp-2.4.0rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     4844 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/docs/background_light.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6427 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/docs/gain_correction.rst
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/docs/l0_to_l1_visp.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     4995 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/docs/polarization_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/docs/requirements_table.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/docs/science_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/docs/scientific_changelog.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 19:33:29.817840 dkist_processing_visp-2.4.0rc1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       60 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/science_towncrier.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1705 2023-06-27 19:33:29.817840 dkist_processing_visp-2.4.0rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2023-06-27 19:33:20.000000 dkist_processing_visp-2.4.0rc1/towncrier_science.toml
```

### Comparing `dkist_processing_visp-2.3.1/.gitignore` & `dkist_processing_visp-2.4.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/.pre-commit-config.yaml` & `dkist_processing_visp-2.4.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/CHANGELOG.rst` & `dkist_processing_visp-2.4.0rc1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-v2.3.1 (2023-06-15)
-===================
-
-Bugfixes
---------
-
-- Fix failure in Geometric task that happened when some modstates had a a different number of identified hairline regions than others. (`#118 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/118>`__)
-
-
 v2.3.0 (2023-05-17)
 ===================
 
 Misc
 ----
 
 - Bumping common to 2.7.0: ParseL0InputData --> ParseL0InputDataBase, constant_flowers --> constant_buds (`#115 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/115>`__)
```

### Comparing `dkist_processing_visp-2.3.1/PKG-INFO` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dkist_processing_visp
-Version: 2.3.1
+Name: dkist-processing-visp
+Version: 2.4.0rc1
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_visp-2.3.1/README.rst` & `dkist_processing_visp-2.4.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/SCIENCE_CHANGELOG.rst` & `dkist_processing_visp-2.4.0rc1/SCIENCE_CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/bitbucket-pipelines.yml` & `dkist_processing_visp-2.4.0rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/check_changelog_updated.sh` & `dkist_processing_visp-2.4.0rc1/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/fonts/Lato-Regular.ttf` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/models/constants.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/models/parameters.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/models/tags.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/map_repeats.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/parsers/map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/polarimeter_mode.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/parsers/polarimeter_mode.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/raster_step.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/parsers/raster_step.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/task.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/parsers/task.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/time.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/visp_l0_fits_access.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/parsers/visp_l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/visp_l1_fits_access.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/parsers/visp_l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/wavelength.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/parsers/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/assemble_movie.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/background_light.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/background_light.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """ViSP background light calibration task."""
 import gc
 import time
 
 import numpy as np
 import scipy.optimize as spo
 from astropy.io import fits
+from dkist_processing_common.codecs.fits import fits_array_encoder
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
 from dkist_processing_math.transform.binning import resize_arrays
 from logging42 import logger
 
+from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.tasks.mixin.corrections import CorrectionsMixin
 from dkist_processing_visp.tasks.mixin.downsample import DownsampleMixin
 from dkist_processing_visp.tasks.mixin.input_frame_loaders import InputFrameLoadersMixin
 from dkist_processing_visp.tasks.mixin.intermediate_frame_helpers import (
     IntermediateFrameHelpersMixin,
 )
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
@@ -69,23 +71,31 @@
         for beam in range(1, self.constants.num_beams + 1):
 
             logger.info(f"Dark-subtracting and spatially resampling raw polcals for {beam = }")
             full_num_wave, full_name_slit_pos, resampled_data = self.reduce_and_resample_polcals(
                 beam=beam, num_bins=num_bins
             )
 
-            self.intermediate_frame_helpers_write_arrays(
-                arrays=resampled_data, beam=beam, task="BL_DEBUG_RESAMP_ARR"
+            self.write(
+                data=resampled_data,
+                encoder=fits_array_encoder,
+                tags=[VispTag.debug(), VispTag.frame()],
+                relative_path=f"DEBUG_BG_RESAMP_ARR_BEAM_{beam}.dat",
+                overwrite=True,
             )
 
             logger.info(f"Computing background light for {beam = }")
             small_background_light = self.compute_background_light(resampled_data)
 
-            self.intermediate_frame_helpers_write_arrays(
-                arrays=small_background_light, beam=beam, task="BL_DEBUG_SMALL_ARR"
+            self.write(
+                data=small_background_light,
+                encoder=fits_array_encoder,
+                tags=[VispTag.debug(), VispTag.frame()],
+                relative_path=f"DEBUG_BG_SMALL_ARR_BEAM_{beam}.dat",
+                overwrite=True,
             )
 
             logger.info(f"Resampling background light to full-frame for {beam = }")
             full_background_light = self.upsample_background_light(
                 small_background_light, full_shape=(full_num_wave, full_name_slit_pos)
             )
```

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/dark.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/geometric.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/geometric.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import scipy.optimize as spo
 import skimage.metrics as skim
 import skimage.morphology as skimo
 import skimage.registration as skir
 from astropy.modeling import fitting
 from astropy.modeling import models
 from astropy.stats import sigma_clip
+from dkist_processing_common.codecs.fits import fits_array_encoder
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
 from logging42 import logger
 from scipy.fft import fftn
 from scipy.optimize import minimize
 from skimage.registration._phase_cross_correlation import _upsampled_dft
@@ -362,19 +363,15 @@
         angle_list = []
         for modstate in range(1, self.constants.num_modstates + 1):
             data = self.basic_corrected_lamp_data(beam=beam, modstate=modstate)
             angle = self._compute_single_modstate_angles(data)
             logger.info(f"Angles for {beam = } and {modstate = } = {np.rad2deg(angle)} deg")
             angle_list.append(angle)
 
-        # Flatten the list just in case we got different numbers of hairline regions for the different modstates
-        # (which can happen in data with strong higher-order hairline leaks).
-        flat_angle_list = np.hstack(angle_list)
-
-        theta = float(np.nanmedian(flat_angle_list))
+        theta = float(np.nanmedian(angle_list))
         logger.info(f"Beam angle for {beam = }: {np.rad2deg(theta):0.4f} deg")
         return theta
 
     def _identify_hairlines_and_bad_pixels(
         self, input_array: np.ndarray
     ) -> tuple[np.ndarray, np.ndarray]:
         """
@@ -773,16 +770,20 @@
         poly_fit_order = self.parameters.geo_poly_fit_order
 
         logger.info(f"Computing spectral shifts for beam {beam}")
         beam_generator = self.offset_corrected_array_generator(beam=beam)
         avg_beam_array = average_numpy_arrays(beam_generator)
         num_spec = avg_beam_array.shape[1]
 
-        self.intermediate_frame_helpers_write_arrays(
-            arrays=avg_beam_array, beam=beam, task="DEBUG_GC_AVG_OFFSET"
+        self.write(
+            data=avg_beam_array,
+            encoder=fits_array_encoder,
+            tags=[VispTag.debug(), VispTag.frame()],
+            relative_path=f"DEBUG_GC_AVG_OFFSET_BEAM_{beam}.dat",
+            overwrite=True,
         )
 
         ref_spec = avg_beam_array[:, num_spec // 2]
         beam_shifts = np.empty(num_spec) * np.nan
         for j in range(num_spec):
             target_spec = avg_beam_array[:, j]
```

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/instrument_polarization.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/instrument_polarization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ViSP instrument polarization task. See :doc:`this page </polarization_calibration>` for more information."""
 from collections import defaultdict
 
 import numpy as np
 import scipy.ndimage as spnd
 from astropy.io import fits
+from dkist_processing_common.codecs.fits import fits_array_encoder
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import divide_arrays_by_array
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
 from dkist_processing_math.transform.binning import resize_arrays
 from dkist_processing_pac.fitter.polcal_fitter import PolcalFitter
 from dkist_processing_pac.input_data.drawer import Drawer
@@ -99,22 +100,30 @@
                     suppress_local_starting_values=True,
                     fit_TM=False,
                 )
 
             with self.apm_processing_step(f"Resampling demodulation matrices for {beam = }"):
                 demod_matrices = pac_fitter.demodulation_matrices
 
-                self.intermediate_frame_helpers_write_arrays(
-                    arrays=demod_matrices, task="IPC_DEBUG_RAW_DEMOD", beam=beam
+                self.write(
+                    data=demod_matrices,
+                    encoder=fits_array_encoder,
+                    tags=[VispTag.debug(), VispTag.frame()],
+                    relative_path=f"DEBUG_IPC_RAW_DEMOD_BEAM_{beam}.dat",
+                    overwrite=True,
                 )
 
                 logger.info(f"Smoothing demodulation matrices for {beam = }")
                 smoothed_demod = self.smooth_demod_matrices(demod_matrices)
-                self.intermediate_frame_helpers_write_arrays(
-                    arrays=smoothed_demod, task="IPC_DEBUG_SMOOTH_DEMOD", beam=beam
+                self.write(
+                    data=smoothed_demod,
+                    encoder=fits_array_encoder,
+                    tags=[VispTag.debug(), VispTag.frame()],
+                    relative_path=f"DEBUG_IPC_SMOOTH_DEMOD_BEAM_{beam}.dat",
+                    overwrite=True,
                 )
 
                 # Reshaping the demodulation matrix to get rid of unit length dimensions
                 logger.info(f"Resampling demodulation matrices for {beam = }")
                 demod_matrices = self.reshape_demod_matrices(smoothed_demod)
                 logger.info(f"Shape of resampled demodulation matrices: {demod_matrices.shape}")
```

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/lamp.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/lamp.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/make_movie_frames.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/corrections.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/mixin/corrections.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/downsample.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/mixin/downsample.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import itertools
 from typing import Generator
 from typing import Iterable
 from typing import TypeVar
 
 import numpy as np
 from astropy.io import fits
+from dkist_processing_common.codecs.fits import fits_array_decoder
+from dkist_processing_common.codecs.fits import fits_array_encoder
 from dkist_processing_common.models.fits_access import FitsAccessBase
 from logging42 import logger
 
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
 
 
@@ -49,16 +51,15 @@
         # is to add a kwarg that has the same name as a tag
         passed_args = locals()
         tags = [VispTag.intermediate(), VispTag.frame()]
         for t, v in passed_args.items():
             if t not in ["self"] and v is not None:
                 tags.append(getattr(VispTag, t)(v))
 
-        for path, hdu in self.fits_data_read_hdu(tags=tags):
-            yield hdu.data
+        yield from self.read(decoder=fits_array_decoder, tags=tags)
 
     def intermediate_frame_helpers_load_dark_array(
         self, beam: int | None = None, exposure_time: float | None = None
     ) -> np.ndarray:
         """
         Produce dark ndarrays for the requested tags.
 
@@ -227,19 +228,19 @@
 
         arrays = [arrays] if isinstance(arrays, np.ndarray) else arrays
         if headers is not None:
             headers = [headers] if isinstance(headers, fits.Header) else headers
         else:
             headers = itertools.repeat(None)
 
+        filenames = []
         for array, header in zip(arrays, headers):
-            hdul = fits.HDUList([fits.PrimaryHDU(data=array, header=header)])
-            self.fits_data_write(hdu_list=hdul, tags=tags)
+            path = self.write(data=array, header=header, encoder=fits_array_encoder, tags=tags)
+            filenames.append(str(path))
 
-        filenames = [str(p) for p in self.read(tags=tags)]
         logger.info(f"Wrote intermediate file for {tags = } to {filenames}")
 
     def intermediate_frame_helpers_load_demod_matrices(self, beam_num: int) -> np.ndarray:
         """
         Load demodulated matrices.
 
         Parameters
@@ -254,16 +255,16 @@
             Demodulated matrix data
         """
         tags = [
             VispTag.intermediate(),
             VispTag.task("DEMOD_MATRICES"),
             VispTag.beam(beam_num),
         ]
-        path, hdu = next(self.fits_data_read_hdu(tags=tags))
-        return hdu.data
+        array = next(self.read(decoder=fits_array_decoder, tags=tags))
+        return array
 
     def intermediate_frame_helpers_fits_access_generator(
         self,
         tags: Iterable[str],
     ) -> Generator[F, None, None]:
         """
         Load a generator of intermediate frames.
```

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/parse.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/quality_metrics.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/science.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/solar.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/solar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ViSP solar calibration task. See :doc:`this page </gain_correction>` for more information."""
 import numpy as np
 import peakutils
 import scipy.ndimage as spnd
 import scipy.optimize as spo
 import scipy.signal as sps
+from dkist_processing_common.codecs.fits import fits_array_encoder
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import divide_arrays_by_array
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
 from logging42 import logger
 
 from dkist_processing_visp.models.tags import VispTag
@@ -67,68 +68,86 @@
                 apm_str = f"{beam = } and {modstate = }"
                 logger.info(f"Dark/lamp/geometric corrections for {apm_str}")
                 with self.apm_processing_step(f"Initial corrections for {apm_str}"):
                     self.do_initial_corrections(beam=beam, modstate=modstate)
 
                 with self.apm_processing_step(f"Computing characteristic spectra for {apm_str}"):
                     char_spec = self.compute_characteristic_spectra(beam=beam, modstate=modstate)
-                    self.intermediate_frame_helpers_write_arrays(
-                        arrays=char_spec, beam=beam, modstate=modstate, task="SC_DEBUG_CHAR_SPEC"
+                    self.write(
+                        data=char_spec,
+                        encoder=fits_array_encoder,
+                        tags=[VispTag.debug(), VispTag.frame()],
+                        relative_path=f"DEBUG_SC_CHAR_SPEC_BEAM_{beam}_MODSTATE_{modstate}.dat",
+                        overwrite=True,
                     )
 
                 with self.apm_processing_step(
                     f"Re-distorting characteristic spectra for {apm_str}"
                 ):
                     spec_shift = self.intermediate_frame_helpers_load_spec_shift(beam=beam)
                     redistorted_char_spec = next(
                         self.corrections_remove_spec_geometry(
                             arrays=char_spec, spec_shift=-1 * spec_shift
                         )
                     )
-                    self.intermediate_frame_helpers_write_arrays(
-                        arrays=redistorted_char_spec,
-                        beam=beam,
-                        modstate=modstate,
-                        task="SC_DEBUG_CHAR_DISTORT",
+                    self.write(
+                        data=redistorted_char_spec,
+                        encoder=fits_array_encoder,
+                        tags=[VispTag.debug(), VispTag.frame()],
+                        relative_path=f"DEBUG_SC_CHAR_DISTORT_BEAM_{beam}_MODSTATE_{modstate}.dat",
+                        overwrite=True,
                     )
 
                 with self.apm_processing_step(f"Re-shifting characteristic spectra for {apm_str}"):
                     reshifted_char_spec = self.distort_characteristic_spectra(
                         char_spec=redistorted_char_spec, beam=beam, modstate=modstate
                     )
-                    self.intermediate_frame_helpers_write_arrays(
-                        arrays=reshifted_char_spec,
-                        beam=beam,
-                        modstate=modstate,
-                        task="SC_DEBUG_CHAR_SPEC_DISTORT_SHIFT",
+                    self.write(
+                        data=reshifted_char_spec,
+                        encoder=fits_array_encoder,
+                        tags=[
+                            VispTag.beam(beam),
+                            VispTag.modstate(modstate),
+                            VispTag.task("CHAR_SPEC_DISTORT_SHIFT"),
+                        ],
+                        relative_path=f"DEBUG_SC_CHAR_SPEC_DISTORT_SHIFT_BEAM_{beam}_MODSTATE_{modstate}.dat",
+                        overwrite=True,
                     )
 
                 with self.apm_processing_step(
                     f"Refining characteristic spectral shifts for {apm_str}"
                 ):
                     refined_char_spec = self.refine_gain_shifts(
                         char_spec=reshifted_char_spec, beam=beam, modstate=modstate
                     )
-                    self.intermediate_frame_helpers_write_arrays(
-                        arrays=refined_char_spec,
-                        beam=beam,
-                        modstate=modstate,
-                        task="SC_DEBUG_CHAR_SPEC_REFINE",
+                    self.write(
+                        data=refined_char_spec,
+                        encoder=fits_array_encoder,
+                        tags=[VispTag.debug(), VispTag.frame()],
+                        relative_path=f"DEBUG_SC_CHAR_SPEC_REFINE_BEAM_{beam}_MODSTATE_{modstate}.dat",
+                        overwrite=True,
                     )
 
                 with self.apm_processing_step(f"Removing solar signal from {apm_str}"):
                     gain = self.remove_solar_signal(
                         char_solar_spectra=refined_char_spec, beam=beam, modstate=modstate
                     )
 
                 with self.apm_processing_step(f"Masking hairlines from {apm_str}"):
                     gain = self.corrections_mask_hairlines(gain)
 
-                self.intermediate_frame_helpers_write_arrays(
-                    arrays=gain, beam=beam, modstate=modstate, task="SC_DEBUG_PRE_EQ_SOLAR_GAIN"
+                self.write(
+                    data=gain,
+                    encoder=fits_array_encoder,
+                    tags=[
+                        VispTag.debug(),
+                        VispTag.frame(),
+                    ],
+                    relative_path=f"DEBUG_SC_PRE_EQ_SOLAR_GAIN_BEAM_{beam}_MODSTATE_{modstate}.dat",
+                    overwrite=True,
                 )
 
                 pre_equalized_gain_dict[modstate] = gain
 
             with self.apm_processing_step(f"Equalizing modstates for {beam = }"):
                 logger.info(f"Equalizing modstate for {beam = }")
                 equalized_gain_dict = self.equalize_modstates(pre_equalized_gain_dict)
```

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/visp_base.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/visp_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/write_l1.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/conftest.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/e2e_helpers.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 import shutil
 from pathlib import Path
 
 import asdf
 from dkist_processing_common.tasks import WorkflowTaskBase
+from dkist_processing_common.tasks.mixin.globus import GlobusTransferItem
 from logging42 import logger
 
 from dkist_processing_visp.models.tags import VispTag
+from dkist_processing_visp.tasks.trial_output_data import TransferVispTrialData
 
 
 class SaveInputParsing(WorkflowTaskBase):
     """Dump redis db to file"""
 
     @property
     def relative_save_file(self) -> str:
@@ -219,7 +221,56 @@
         return "inst_pol_cal.asdf"
 
 
 class LoadInstPolCal(LoadTaskTags):
     @property
     def relative_save_file(self) -> str:
         return "inst_pol_cal.asdf"
+
+
+def transfer_trial_data_locally_task(
+    trial_dir: str | Path,
+    debug_switch: bool = True,
+    intermediate_switch: bool = True,
+    output_swtich: bool = True,
+    tag_lists: list | None = None,
+):
+    class LocalTrialData(TransferVispTrialData):
+        @property
+        def destination_folder(self) -> Path:
+            return Path(trial_dir)
+
+        @property
+        def debug_frame_switch(self) -> bool:
+            return debug_switch
+
+        @property
+        def intermediate_frame_switch(self) -> bool:
+            return intermediate_switch
+
+        @property
+        def output_frame_switch(self) -> bool:
+            return output_swtich
+
+        @property
+        def specific_frame_tag_lists(self) -> list:
+            return tag_lists or []
+
+        def remove_folder_objects(self):
+            logger.info("Would have removed folder objects here")
+
+        def globus_transfer_scratch_to_object_store(
+            self,
+            transfer_items: list[GlobusTransferItem],
+            label: str = None,
+            sync_level: str = None,
+            verify_checksum: bool = True,
+        ) -> None:
+            if label:
+                logger.info(f"Transferring files with {label = }")
+
+            for frame in transfer_items:
+                if not frame.destination_path.parent.exists():
+                    frame.destination_path.parent.mkdir(parents=True)
+                os.system(f"cp {frame.source_path} {frame.destination_path}")
+
+    return LocalTrialData
```

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/e2e_test.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import os
 import sys
 from dataclasses import asdict
 from datetime import datetime
 from pathlib import Path
 from random import randint
+from unittest.mock import patch
 
 from astropy.io import fits
 from dkist_header_validator import spec122_validator
 from dkist_header_validator import spec214_validator
 from dkist_processing_common.manual import ManualProcessing
 from dkist_processing_common.tasks import QualityL1Metrics
 from dkist_processing_common.tasks import WorkflowTaskBase
@@ -29,28 +30,31 @@
 from dkist_processing_visp.tasks.quality_metrics import VispL0QualityMetrics
 from dkist_processing_visp.tasks.quality_metrics import VispL1QualityMetrics
 from dkist_processing_visp.tasks.science import ScienceCalibration
 from dkist_processing_visp.tasks.solar import SolarCalibration
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
 from dkist_processing_visp.tasks.write_l1 import VispWriteL1Frame
 from dkist_processing_visp.tests.conftest import VispTestingParameters
-from dkist_processing_visp.tests.e2e_helpers import LoadBackgroundCal
-from dkist_processing_visp.tests.e2e_helpers import LoadDarkCal
-from dkist_processing_visp.tests.e2e_helpers import LoadGeometricCal
-from dkist_processing_visp.tests.e2e_helpers import LoadInputParsing
-from dkist_processing_visp.tests.e2e_helpers import LoadInstPolCal
-from dkist_processing_visp.tests.e2e_helpers import LoadLampCal
-from dkist_processing_visp.tests.e2e_helpers import LoadSolarCal
-from dkist_processing_visp.tests.e2e_helpers import SaveBackgroundCal
-from dkist_processing_visp.tests.e2e_helpers import SaveDarkCal
-from dkist_processing_visp.tests.e2e_helpers import SaveGeometricCal
-from dkist_processing_visp.tests.e2e_helpers import SaveInputParsing
-from dkist_processing_visp.tests.e2e_helpers import SaveInstPolCal
-from dkist_processing_visp.tests.e2e_helpers import SaveLampCal
-from dkist_processing_visp.tests.e2e_helpers import SaveSolarCal
+from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import LoadBackgroundCal
+from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import LoadDarkCal
+from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import LoadGeometricCal
+from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import LoadInputParsing
+from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import LoadInstPolCal
+from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import LoadLampCal
+from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import LoadSolarCal
+from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import SaveBackgroundCal
+from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import SaveDarkCal
+from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import SaveGeometricCal
+from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import SaveInputParsing
+from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import SaveInstPolCal
+from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import SaveLampCal
+from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import SaveSolarCal
+from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import (
+    transfer_trial_data_locally_task,
+)
 
 INV = False
 try:
     from dkist_inventory.asdf_generator import dataset_from_fits
 
     INV = True
 except ModuleNotFoundError:
@@ -283,14 +287,15 @@
     load_dark: bool = False,
     load_background: bool = False,
     load_lamp: bool = False,
     load_geometric: bool = False,
     load_solar: bool = False,
     load_inst_pol: bool = False,
     use_apm: bool = False,
+    transfer_trial_data: str | None = None,
 ):
     if use_apm:
         setup_APM_config()
     with ManualProcessing(
         workflow_path=scratch_path,
         recipe_run_id=recipe_run_id,
         testing=True,
@@ -356,14 +361,26 @@
         manual_processing_run.run_task(task=QualityL1Metrics)
         manual_processing_run.run_task(task=VispL1QualityMetrics)
         manual_processing_run.run_task(task=SubmitAndExposeQuality)
         manual_processing_run.run_task(task=ValidateL1Output)
         manual_processing_run.run_task(task=MakeVispMovieFrames)
         manual_processing_run.run_task(task=AssembleVispMovie)
 
+        if transfer_trial_data:
+            if transfer_trial_data == "default":
+                trial_output_dir = (
+                    Path(manual_processing_run.workflow_path) / str(recipe_run_id) / "trial_output"
+                )
+            else:
+                trial_output_dir = Path(transfer_trial_data).absolute()
+
+            logger.info(f"Writing trial output to {trial_output_dir}")
+            transfer_local_task = transfer_trial_data_locally_task(trial_dir=trial_output_dir)
+            manual_processing_run.run_task(transfer_local_task)
+
         # Test some downstream services
         make_pdf_report(scratch_path, recipe_run_id)
         make_dataset_asdf(recipe_run_id, scratch_path)
 
         if any([load_dark, load_lamp, load_geometric, load_solar, load_inst_pol]):
             logger.info("NOT counting provenance records because some tasks were skipped")
         else:
@@ -389,14 +406,22 @@
         help="Skip the translation of raw 122 l0 frames to 214 l0",
         action="store_true",
     )
     parser.add_argument(
         "-t", "--only-translate", help="Do ONLY the translation step", action="store_true"
     )
     parser.add_argument(
+        "-X",
+        "--transfer-trial-data",
+        help="Transfer trial data to a different location.",
+        nargs="?",
+        const="default",
+        default=None,
+    )
+    parser.add_argument(
         "-I", "--load-input-parsing", help="Load tags on input files", action="store_true"
     )
     parser.add_argument(
         "-D",
         "--load-dark",
         help="Load dark calibration from previously saved run",
         action="store_true",
@@ -444,9 +469,10 @@
             load_dark=args.load_dark,
             load_background=args.load_background,
             load_lamp=args.load_lamp,
             load_geometric=args.load_geometric,
             load_solar=args.load_solar,
             load_inst_pol=args.load_inst_pol,
             use_apm=args.use_apm,
+            transfer_trial_data=args.transfer_trial_data,
         )
     )
```

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_assemble_movie.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_background_light.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_background_light.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_build_quality_report.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_build_quality_report.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_dark.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_downsample.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_geometric.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_geometric.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_instrument_polarization.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_instrument_polarization.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_lamp.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_lamp.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_make_movie_frames.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_map_repeats.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_parameters.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_parse.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_quality.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_science.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_solar.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_solar.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_submit_quality.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_submit_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_visp_base.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_visp_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                 VispTag.map_scan(2),
                 VispTag.raster_step(3),
                 VispTag.task("BAR"),
             ]
         )
     )
     assert len(loaded_list) == 1
-    hdu = loaded_list[0][1]
+    hdu = loaded_list[0]
     np.testing.assert_equal(hdu.data, data)
     assert hdu.header["TEST"] == "foo"
 
 
 def test_write_intermediate_arrays_none_header(visp_science_task):
     """
     Given: A VispTaskBase task
@@ -93,15 +93,15 @@
                 VispTag.map_scan(2),
                 VispTag.raster_step(3),
                 VispTag.task("BAR"),
             ]
         )
     )
     assert len(loaded_list) == 1
-    hdu = loaded_list[0][1]
+    hdu = loaded_list[0]
     np.testing.assert_equal(hdu.data, data)
 
 
 @pytest.fixture
 def visp_science_task_with_tagged_intermediates(
     recipe_run_id, tmpdir_factory, init_visp_constants_db
 ):
```

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_visp_constants.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_visp_constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_write_l1.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp/workflows/l0_processing.py` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp/workflows/l0_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp.egg-info/PKG-INFO` & `dkist_processing_visp-2.4.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dkist-processing-visp
-Version: 2.3.1
+Name: dkist_processing_visp
+Version: 2.4.0rc1
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp.egg-info/SOURCES.txt` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 check_changelog_updated.sh
 pyproject.toml
 science_towncrier.sh
 setup.cfg
 setup.py
 towncrier_science.toml
 changelog/.gitempty
+changelog/116.feature.rst
+changelog/117.misc.rst
 dkist_processing_visp/__init__.py
 dkist_processing_visp.egg-info/PKG-INFO
 dkist_processing_visp.egg-info/SOURCES.txt
 dkist_processing_visp.egg-info/dependency_links.txt
 dkist_processing_visp.egg-info/requires.txt
 dkist_processing_visp.egg-info/top_level.txt
 dkist_processing_visp/fonts/Lato-Regular.ttf
@@ -41,25 +43,24 @@
 dkist_processing_visp/tasks/l1_output_data.py
 dkist_processing_visp/tasks/lamp.py
 dkist_processing_visp/tasks/make_movie_frames.py
 dkist_processing_visp/tasks/parse.py
 dkist_processing_visp/tasks/quality_metrics.py
 dkist_processing_visp/tasks/science.py
 dkist_processing_visp/tasks/solar.py
+dkist_processing_visp/tasks/trial_output_data.py
 dkist_processing_visp/tasks/visp_base.py
 dkist_processing_visp/tasks/write_l1.py
 dkist_processing_visp/tasks/mixin/__init__.py
 dkist_processing_visp/tasks/mixin/corrections.py
 dkist_processing_visp/tasks/mixin/downsample.py
 dkist_processing_visp/tasks/mixin/input_frame_loaders.py
 dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
 dkist_processing_visp/tests/__init__.py
 dkist_processing_visp/tests/conftest.py
-dkist_processing_visp/tests/e2e_helpers.py
-dkist_processing_visp/tests/e2e_test.py
 dkist_processing_visp/tests/test_assemble_movie.py
 dkist_processing_visp/tests/test_background_light.py
 dkist_processing_visp/tests/test_build_quality_report.py
 dkist_processing_visp/tests/test_dark.py
 dkist_processing_visp/tests/test_downsample.py
 dkist_processing_visp/tests/test_geometric.py
 dkist_processing_visp/tests/test_instrument_polarization.py
@@ -68,21 +69,26 @@
 dkist_processing_visp/tests/test_map_repeats.py
 dkist_processing_visp/tests/test_parameters.py
 dkist_processing_visp/tests/test_parse.py
 dkist_processing_visp/tests/test_quality.py
 dkist_processing_visp/tests/test_science.py
 dkist_processing_visp/tests/test_solar.py
 dkist_processing_visp/tests/test_submit_quality.py
+dkist_processing_visp/tests/test_trial_output_data.py
 dkist_processing_visp/tests/test_visp_base.py
 dkist_processing_visp/tests/test_visp_constants.py
 dkist_processing_visp/tests/test_workflows.py
 dkist_processing_visp/tests/test_write_l1.py
+dkist_processing_visp/tests/local_trial_workflows/__init__.py
+dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py
+dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py
 dkist_processing_visp/workflows/__init__.py
 dkist_processing_visp/workflows/l0_processing.py
 dkist_processing_visp/workflows/single_task_workflows.py
+dkist_processing_visp/workflows/trial_workflows.py
 docs/Makefile
 docs/background_light.rst
 docs/changelog.rst
 docs/conf.py
 docs/gain_correction.rst
 docs/index.rst
 docs/l0_to_l1_visp.rst
```

### Comparing `dkist_processing_visp-2.3.1/dkist_processing_visp.egg-info/requires.txt` & `dkist_processing_visp-2.4.0rc1/dkist_processing_visp.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-dkist-processing-common==2.7.0
+dkist-processing-common==3.0.0
 dkist-processing-math==1.0.1
 dkist-processing-pac==2.1.1
 dkist-header-validator==3.0.5
 dkist-fits-specifications==3.6.0
 astropy==5.1.1
 numpy==1.23.1
 sunpy==4.1.4
```

### Comparing `dkist_processing_visp-2.3.1/docs/Makefile` & `dkist_processing_visp-2.4.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/docs/background_light.rst` & `dkist_processing_visp-2.4.0rc1/docs/background_light.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/docs/conf.py` & `dkist_processing_visp-2.4.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/docs/gain_correction.rst` & `dkist_processing_visp-2.4.0rc1/docs/gain_correction.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/docs/l0_to_l1_visp.rst` & `dkist_processing_visp-2.4.0rc1/docs/l0_to_l1_visp.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/docs/make.bat` & `dkist_processing_visp-2.4.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/docs/polarization_calibration.rst` & `dkist_processing_visp-2.4.0rc1/docs/polarization_calibration.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/docs/science_calibration.rst` & `dkist_processing_visp-2.4.0rc1/docs/science_calibration.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/licenses/LICENSE.rst` & `dkist_processing_visp-2.4.0rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/pyproject.toml` & `dkist_processing_visp-2.4.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.1/setup.cfg` & `dkist_processing_visp-2.4.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

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
 	dkist-processing-pac == 2.1.1
 	dkist-header-validator == 3.0.5
 	dkist-fits-specifications == 3.6.0
 	astropy == 5.1.1
 	numpy == 1.23.1
 	sunpy == 4.1.4
```

