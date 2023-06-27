# Comparing `tmp/paradigm-flood-0.2.4.tar.gz` & `tmp/paradigm-flood-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradigm-flood-0.2.4.tar", last modified: Thu Jun 22 00:50:20 2023, max compression
+gzip compressed data, was "paradigm-flood-0.2.5.tar", last modified: Tue Jun 27 07:15:32 2023, max compression
```

## Comparing `paradigm-flood-0.2.4.tar` & `paradigm-flood-0.2.5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0      513 2023-06-06 19:32:53.475871 paradigm-flood-0.2.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      607 2023-06-06 19:32:53.476113 paradigm-flood-0.2.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      193 2023-06-06 19:32:53.476353 paradigm-flood-0.2.4/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0      781 2023-06-06 19:32:53.476534 paradigm-flood-0.2.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      165 2023-06-06 19:32:53.476751 paradigm-flood-0.2.4/.github/workflows/lint.yml
--rw-r--r--   0        0        0      513 2023-06-22 00:28:24.031464 paradigm-flood-0.2.4/.github/workflows/tests.yml
--rw-r--r--   0        0        0      225 2023-05-06 04:56:40.389625 paradigm-flood-0.2.4/.gitignore
--rw-r--r--   0        0        0    10332 2023-06-04 20:22:19.525565 paradigm-flood-0.2.4/CONTRIBUTING.md
--rw-r--r--   0        0        0      832 2023-06-02 00:45:29.473078 paradigm-flood-0.2.4/Dockerfile
--rw-r--r--   0        0        0    10839 2023-06-04 20:13:59.817606 paradigm-flood-0.2.4/LICENSE-APACHE
--rw-r--r--   0        0        0     1085 2023-06-04 20:13:48.830823 paradigm-flood-0.2.4/LICENSE-MIT
--rw-r--r--   0        0        0     2865 2023-06-06 19:32:53.477627 paradigm-flood-0.2.4/README.md
--rw-r--r--   0        0        0  3038209 2023-06-06 19:32:53.483637 paradigm-flood-0.2.4/assets/cover.png
--rw-r--r--   0        0        0      124 2023-06-06 21:20:36.150174 paradigm-flood-0.2.4/examples/equality_test.sh
--rwxr-xr-x   0        0        0     1905 2023-06-15 16:40:12.596585 paradigm-flood-0.2.4/examples/report.sh
--rw-r--r--   0        0        0      648 2023-06-22 00:49:45.056970 paradigm-flood-0.2.4/flood/__init__.py
--rw-r--r--   0        0        0      117 2023-06-04 23:14:01.291195 paradigm-flood-0.2.4/flood/__main__.py
--rw-r--r--   0        0        0     1556 2023-06-22 00:34:03.891521 paradigm-flood-0.2.4/flood/cli/cli_run.py
--rw-r--r--   0        0        0      877 2023-06-04 23:14:01.298637 paradigm-flood-0.2.4/flood/cli/ls_command.py
--rw-r--r--   0        0        0     1630 2023-06-22 00:34:03.891718 paradigm-flood-0.2.4/flood/cli/print_command.py
--rw-r--r--   0        0        0     1221 2023-06-04 23:14:01.302153 paradigm-flood-0.2.4/flood/cli/report_command.py
--rw-r--r--   0        0        0     6215 2023-06-22 00:34:03.891970 paradigm-flood-0.2.4/flood/cli/root_command.py
--rw-r--r--   0        0        0     1315 2023-06-04 23:14:01.307482 paradigm-flood-0.2.4/flood/cli/samples_collect_command.py
--rw-r--r--   0        0        0     1687 2023-06-06 20:39:09.158213 paradigm-flood-0.2.4/flood/cli/samples_download_command.py
--rw-r--r--   0        0        0     1874 2023-06-06 20:39:23.569867 paradigm-flood-0.2.4/flood/cli/samples_ls_command.py
--rw-r--r--   0        0        0      121 2023-06-03 19:54:58.405209 paradigm-flood-0.2.4/flood/generators/__init__.py
--rw-r--r--   0        0        0      199 2023-06-03 19:54:39.491471 paradigm-flood-0.2.4/flood/generators/object_generators/__init__.py
--rw-r--r--   0        0        0      603 2023-06-04 23:14:01.311234 paradigm-flood-0.2.4/flood/generators/object_generators/address_generators.py
--rw-r--r--   0        0        0     4815 2023-06-04 23:14:01.335388 paradigm-flood-0.2.4/flood/generators/object_generators/block_generators.py
--rw-r--r--   0        0        0    17256 2023-06-06 20:39:37.317485 paradigm-flood-0.2.4/flood/generators/object_generators/call_generators.py
--rw-r--r--   0        0        0      337 2023-06-04 23:14:01.306215 paradigm-flood-0.2.4/flood/generators/object_generators/slot_generators.py
--rw-r--r--   0        0        0     4156 2023-06-06 20:41:05.406418 paradigm-flood-0.2.4/flood/generators/object_generators/timing_generators.py
--rw-r--r--   0        0        0      346 2023-06-04 23:14:01.315806 paradigm-flood-0.2.4/flood/generators/object_generators/transaction_generators.py
--rw-r--r--   0        0        0      129 2023-06-02 06:40:02.759112 paradigm-flood-0.2.4/flood/generators/raw_data_sources/__init__.py
--rw-r--r--   0        0        0      465 2023-06-04 23:14:01.312615 paradigm-flood-0.2.4/flood/generators/raw_data_sources/raw_data_spec.py
--rw-r--r--   0        0        0     1935 2023-06-04 23:14:01.327302 paradigm-flood-0.2.4/flood/generators/raw_data_sources/raw_download_utils.py
--rw-r--r--   0        0        0     5688 2023-06-04 23:14:01.364193 paradigm-flood-0.2.4/flood/generators/raw_data_sources/raw_gather_utils.py
--rw-r--r--   0        0        0     4662 2023-06-04 23:14:01.352117 paradigm-flood-0.2.4/flood/generators/raw_data_sources/raw_sample_loading.py
--rw-r--r--   0        0        0      530 2023-06-04 23:14:01.322799 paradigm-flood-0.2.4/flood/generators/rng_utils.py
--rw-r--r--   0        0        0      307 2023-06-16 00:43:55.812056 paradigm-flood-0.2.4/flood/generators/test_generators/__init__.py
--rw-r--r--   0        0        0     1507 2023-06-04 23:14:01.337667 paradigm-flood-0.2.4/flood/generators/test_generators/address_test_generators.py
--rw-r--r--   0        0        0     1559 2023-06-04 23:14:01.331116 paradigm-flood-0.2.4/flood/generators/test_generators/block_test_generators.py
--rw-r--r--   0        0        0     2150 2023-06-04 23:14:01.346034 paradigm-flood-0.2.4/flood/generators/test_generators/contract_test_generators.py
--rw-r--r--   0        0        0     5333 2023-06-16 00:44:54.451370 paradigm-flood-0.2.4/flood/generators/test_generators/generic_test_generators.py
--rw-r--r--   0        0        0     3870 2023-06-04 23:14:01.341234 paradigm-flood-0.2.4/flood/generators/test_generators/log_test_generators.py
--rw-r--r--   0        0        0      162 2023-06-16 00:43:37.064471 paradigm-flood-0.2.4/flood/generators/test_generators/multi_test_generators.py
--rw-r--r--   0        0        0     5897 2023-06-04 23:14:01.413684 paradigm-flood-0.2.4/flood/generators/test_generators/trace_test_generators.py
--rw-r--r--   0        0        0     1512 2023-06-04 23:14:01.354881 paradigm-flood-0.2.4/flood/generators/test_generators/transaction_test_generators.py
--rw-r--r--   0        0        0       87 2023-06-15 23:24:24.125486 paradigm-flood-0.2.4/flood/runners/__init__.py
--rw-r--r--   0        0        0       40 2023-06-15 23:57:58.076473 paradigm-flood-0.2.4/flood/runners/generic_runner/__init__.py
--rw-r--r--   0        0        0     3437 2023-06-22 00:34:03.892257 paradigm-flood-0.2.4/flood/runners/generic_runner/generic_runner_execution.py
--rw-r--r--   0        0        0       31 2023-06-15 23:25:05.871130 paradigm-flood-0.2.4/flood/runners/multi_runner/__init__.py
--rw-r--r--   0        0        0     1081 2023-06-15 23:25:35.750693 paradigm-flood-0.2.4/flood/runners/multi_runner/multi_runner_io.py
--rw-r--r--   0        0        0       32 2023-06-15 23:24:48.633159 paradigm-flood-0.2.4/flood/runners/single_runner/__init__.py
--rw-r--r--   0        0        0     4845 2023-06-22 00:34:03.892502 paradigm-flood-0.2.4/flood/runners/single_runner/single_runner_execution.py
--rw-r--r--   0        0        0     4751 2023-06-22 00:34:03.892741 paradigm-flood-0.2.4/flood/runners/single_runner/single_runner_io.py
--rw-r--r--   0        0        0     6430 2023-06-15 23:32:29.744850 paradigm-flood-0.2.4/flood/runners/single_runner/single_runner_summary.py
--rw-r--r--   0        0        0     5117 2023-06-20 03:52:27.584215 paradigm-flood-0.2.4/flood/spec.py
--rw-r--r--   0        0        0       56 2023-06-15 23:55:07.358215 paradigm-flood-0.2.4/flood/tests/__init__.py
--rw-r--r--   0        0        0       34 2023-06-04 23:14:01.345292 paradigm-flood-0.2.4/flood/tests/equality_tests/__init__.py
--rw-r--r--   0        0        0     6200 2023-06-22 00:39:58.042086 paradigm-flood-0.2.4/flood/tests/equality_tests/equality_test_runs.py
--rw-r--r--   0        0        0     8501 2023-06-06 20:41:24.278488 paradigm-flood-0.2.4/flood/tests/equality_tests/equality_test_sets.py
--rw-r--r--   0        0        0      154 2023-06-02 00:45:29.480806 paradigm-flood-0.2.4/flood/tests/load_tests/__init__.py
--rw-r--r--   0        0        0     2682 2023-06-04 23:14:01.379714 paradigm-flood-0.2.4/flood/tests/load_tests/load_test_construction.py
--rw-r--r--   0        0        0     5740 2023-06-15 21:26:24.315199 paradigm-flood-0.2.4/flood/tests/load_tests/load_test_plots.py
--rw-r--r--   0        0        0    10242 2023-06-15 23:17:43.297886 paradigm-flood-0.2.4/flood/tests/load_tests/load_test_reports.py
--rw-r--r--   0        0        0    13410 2023-06-22 00:34:03.894287 paradigm-flood-0.2.4/flood/tests/load_tests/load_test_runs.py
--rw-r--r--   0        0        0    10443 2023-06-20 06:29:09.583999 paradigm-flood-0.2.4/flood/tests/load_tests/vegeta.py
--rw-r--r--   0        0        0       45 2023-06-15 23:20:48.386860 paradigm-flood-0.2.4/flood/user_io/__init__.py
--rw-r--r--   0        0        0     5903 2023-06-15 06:32:18.240729 paradigm-flood-0.2.4/flood/user_io/inputs.py
--rw-r--r--   0        0        0     4285 2023-06-04 23:14:01.438468 paradigm-flood-0.2.4/flood/user_io/notebook_io.py
--rw-r--r--   0        0        0     5864 2023-06-06 20:35:25.703304 paradigm-flood-0.2.4/flood/user_io/outputs.py
--rw-r--r--   0        0        0     1919 2023-06-22 00:43:46.791751 paradigm-flood-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      381 2023-06-04 20:35:57.569281 paradigm-flood-0.2.4/tests/README.md
--rw-r--r--   0        0        0      993 2023-06-06 21:03:30.304627 paradigm-flood-0.2.4/tests/conftest.py
--rw-r--r--   0        0        0      593 2023-06-04 20:53:58.379044 paradigm-flood-0.2.4/tests/test_env_vars.py
--rw-r--r--   0        0        0      269 2023-06-06 21:04:00.022725 paradigm-flood-0.2.4/tests/test_equality_tests.py
--rw-r--r--   0        0        0     1128 2023-06-06 21:03:47.012574 paradigm-flood-0.2.4/tests/test_load_tests.py
--rw-r--r--   0        0        0     1736 2023-06-04 16:00:15.996050 paradigm-flood-0.2.4/tests/test_node_parsing.py
--rw-r--r--   0        0        0     4526 1970-01-01 00:00:00.000000 paradigm-flood-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-06-06 19:32:53.475871 paradigm-flood-0.2.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      607 2023-06-06 19:32:53.476113 paradigm-flood-0.2.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      193 2023-06-06 19:32:53.476353 paradigm-flood-0.2.5/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0      781 2023-06-06 19:32:53.476534 paradigm-flood-0.2.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      165 2023-06-06 19:32:53.476751 paradigm-flood-0.2.5/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      513 2023-06-22 00:28:24.031464 paradigm-flood-0.2.5/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      225 2023-05-06 04:56:40.389625 paradigm-flood-0.2.5/.gitignore
+-rw-r--r--   0        0        0    10332 2023-06-04 20:22:19.525565 paradigm-flood-0.2.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0      832 2023-06-02 00:45:29.473078 paradigm-flood-0.2.5/Dockerfile
+-rw-r--r--   0        0        0    10839 2023-06-04 20:13:59.817606 paradigm-flood-0.2.5/LICENSE-APACHE
+-rw-r--r--   0        0        0     1085 2023-06-04 20:13:48.830823 paradigm-flood-0.2.5/LICENSE-MIT
+-rw-r--r--   0        0        0     2865 2023-06-06 19:32:53.477627 paradigm-flood-0.2.5/README.md
+-rw-r--r--   0        0        0  3038209 2023-06-06 19:32:53.483637 paradigm-flood-0.2.5/assets/cover.png
+-rw-r--r--   0        0        0      124 2023-06-06 21:20:36.150174 paradigm-flood-0.2.5/examples/equality_test.sh
+-rwxr-xr-x   0        0        0     1905 2023-06-15 16:40:12.596585 paradigm-flood-0.2.5/examples/report.sh
+-rw-r--r--   0        0        0      648 2023-06-27 07:14:54.717881 paradigm-flood-0.2.5/flood/__init__.py
+-rw-r--r--   0        0        0      117 2023-06-04 23:14:01.291195 paradigm-flood-0.2.5/flood/__main__.py
+-rw-r--r--   0        0        0     1556 2023-06-22 00:34:03.891521 paradigm-flood-0.2.5/flood/cli/cli_run.py
+-rw-r--r--   0        0        0      877 2023-06-04 23:14:01.298637 paradigm-flood-0.2.5/flood/cli/ls_command.py
+-rw-r--r--   0        0        0     1630 2023-06-22 00:34:03.891718 paradigm-flood-0.2.5/flood/cli/print_command.py
+-rw-r--r--   0        0        0     1221 2023-06-04 23:14:01.302153 paradigm-flood-0.2.5/flood/cli/report_command.py
+-rw-r--r--   0        0        0     6215 2023-06-22 00:34:03.891970 paradigm-flood-0.2.5/flood/cli/root_command.py
+-rw-r--r--   0        0        0     1315 2023-06-04 23:14:01.307482 paradigm-flood-0.2.5/flood/cli/samples_collect_command.py
+-rw-r--r--   0        0        0     1687 2023-06-06 20:39:09.158213 paradigm-flood-0.2.5/flood/cli/samples_download_command.py
+-rw-r--r--   0        0        0     1874 2023-06-06 20:39:23.569867 paradigm-flood-0.2.5/flood/cli/samples_ls_command.py
+-rw-r--r--   0        0        0      121 2023-06-03 19:54:58.405209 paradigm-flood-0.2.5/flood/generators/__init__.py
+-rw-r--r--   0        0        0      199 2023-06-03 19:54:39.491471 paradigm-flood-0.2.5/flood/generators/object_generators/__init__.py
+-rw-r--r--   0        0        0      603 2023-06-04 23:14:01.311234 paradigm-flood-0.2.5/flood/generators/object_generators/address_generators.py
+-rw-r--r--   0        0        0     4815 2023-06-04 23:14:01.335388 paradigm-flood-0.2.5/flood/generators/object_generators/block_generators.py
+-rw-r--r--   0        0        0    17256 2023-06-06 20:39:37.317485 paradigm-flood-0.2.5/flood/generators/object_generators/call_generators.py
+-rw-r--r--   0        0        0      337 2023-06-04 23:14:01.306215 paradigm-flood-0.2.5/flood/generators/object_generators/slot_generators.py
+-rw-r--r--   0        0        0     4156 2023-06-06 20:41:05.406418 paradigm-flood-0.2.5/flood/generators/object_generators/timing_generators.py
+-rw-r--r--   0        0        0      346 2023-06-04 23:14:01.315806 paradigm-flood-0.2.5/flood/generators/object_generators/transaction_generators.py
+-rw-r--r--   0        0        0      129 2023-06-02 06:40:02.759112 paradigm-flood-0.2.5/flood/generators/raw_data_sources/__init__.py
+-rw-r--r--   0        0        0      465 2023-06-04 23:14:01.312615 paradigm-flood-0.2.5/flood/generators/raw_data_sources/raw_data_spec.py
+-rw-r--r--   0        0        0     1935 2023-06-04 23:14:01.327302 paradigm-flood-0.2.5/flood/generators/raw_data_sources/raw_download_utils.py
+-rw-r--r--   0        0        0     5688 2023-06-04 23:14:01.364193 paradigm-flood-0.2.5/flood/generators/raw_data_sources/raw_gather_utils.py
+-rw-r--r--   0        0        0     4662 2023-06-04 23:14:01.352117 paradigm-flood-0.2.5/flood/generators/raw_data_sources/raw_sample_loading.py
+-rw-r--r--   0        0        0      530 2023-06-04 23:14:01.322799 paradigm-flood-0.2.5/flood/generators/rng_utils.py
+-rw-r--r--   0        0        0      307 2023-06-16 00:43:55.812056 paradigm-flood-0.2.5/flood/generators/test_generators/__init__.py
+-rw-r--r--   0        0        0     1507 2023-06-04 23:14:01.337667 paradigm-flood-0.2.5/flood/generators/test_generators/address_test_generators.py
+-rw-r--r--   0        0        0     1559 2023-06-04 23:14:01.331116 paradigm-flood-0.2.5/flood/generators/test_generators/block_test_generators.py
+-rw-r--r--   0        0        0     2150 2023-06-04 23:14:01.346034 paradigm-flood-0.2.5/flood/generators/test_generators/contract_test_generators.py
+-rw-r--r--   0        0        0     5333 2023-06-16 00:44:54.451370 paradigm-flood-0.2.5/flood/generators/test_generators/generic_test_generators.py
+-rw-r--r--   0        0        0     3870 2023-06-04 23:14:01.341234 paradigm-flood-0.2.5/flood/generators/test_generators/log_test_generators.py
+-rw-r--r--   0        0        0      162 2023-06-16 00:43:37.064471 paradigm-flood-0.2.5/flood/generators/test_generators/multi_test_generators.py
+-rw-r--r--   0        0        0     5897 2023-06-04 23:14:01.413684 paradigm-flood-0.2.5/flood/generators/test_generators/trace_test_generators.py
+-rw-r--r--   0        0        0     1512 2023-06-04 23:14:01.354881 paradigm-flood-0.2.5/flood/generators/test_generators/transaction_test_generators.py
+-rw-r--r--   0        0        0       87 2023-06-15 23:24:24.125486 paradigm-flood-0.2.5/flood/runners/__init__.py
+-rw-r--r--   0        0        0       40 2023-06-15 23:57:58.076473 paradigm-flood-0.2.5/flood/runners/generic_runner/__init__.py
+-rw-r--r--   0        0        0     3437 2023-06-22 00:34:03.892257 paradigm-flood-0.2.5/flood/runners/generic_runner/generic_runner_execution.py
+-rw-r--r--   0        0        0       31 2023-06-15 23:25:05.871130 paradigm-flood-0.2.5/flood/runners/multi_runner/__init__.py
+-rw-r--r--   0        0        0     1081 2023-06-15 23:25:35.750693 paradigm-flood-0.2.5/flood/runners/multi_runner/multi_runner_io.py
+-rw-r--r--   0        0        0       32 2023-06-15 23:24:48.633159 paradigm-flood-0.2.5/flood/runners/single_runner/__init__.py
+-rw-r--r--   0        0        0     4845 2023-06-22 00:34:03.892502 paradigm-flood-0.2.5/flood/runners/single_runner/single_runner_execution.py
+-rw-r--r--   0        0        0     4751 2023-06-22 00:34:03.892741 paradigm-flood-0.2.5/flood/runners/single_runner/single_runner_io.py
+-rw-r--r--   0        0        0     6430 2023-06-15 23:32:29.744850 paradigm-flood-0.2.5/flood/runners/single_runner/single_runner_summary.py
+-rw-r--r--   0        0        0     5117 2023-06-20 03:52:27.584215 paradigm-flood-0.2.5/flood/spec.py
+-rw-r--r--   0        0        0       56 2023-06-15 23:55:07.358215 paradigm-flood-0.2.5/flood/tests/__init__.py
+-rw-r--r--   0        0        0       34 2023-06-04 23:14:01.345292 paradigm-flood-0.2.5/flood/tests/equality_tests/__init__.py
+-rw-r--r--   0        0        0     6200 2023-06-22 00:39:58.042086 paradigm-flood-0.2.5/flood/tests/equality_tests/equality_test_runs.py
+-rw-r--r--   0        0        0     8699 2023-06-27 07:14:03.167951 paradigm-flood-0.2.5/flood/tests/equality_tests/equality_test_sets.py
+-rw-r--r--   0        0        0      154 2023-06-02 00:45:29.480806 paradigm-flood-0.2.5/flood/tests/load_tests/__init__.py
+-rw-r--r--   0        0        0     2682 2023-06-04 23:14:01.379714 paradigm-flood-0.2.5/flood/tests/load_tests/load_test_construction.py
+-rw-r--r--   0        0        0     5740 2023-06-15 21:26:24.315199 paradigm-flood-0.2.5/flood/tests/load_tests/load_test_plots.py
+-rw-r--r--   0        0        0    10242 2023-06-15 23:17:43.297886 paradigm-flood-0.2.5/flood/tests/load_tests/load_test_reports.py
+-rw-r--r--   0        0        0    13410 2023-06-22 00:34:03.894287 paradigm-flood-0.2.5/flood/tests/load_tests/load_test_runs.py
+-rw-r--r--   0        0        0    10443 2023-06-20 06:29:09.583999 paradigm-flood-0.2.5/flood/tests/load_tests/vegeta.py
+-rw-r--r--   0        0        0       45 2023-06-15 23:20:48.386860 paradigm-flood-0.2.5/flood/user_io/__init__.py
+-rw-r--r--   0        0        0     5903 2023-06-15 06:32:18.240729 paradigm-flood-0.2.5/flood/user_io/inputs.py
+-rw-r--r--   0        0        0     4285 2023-06-04 23:14:01.438468 paradigm-flood-0.2.5/flood/user_io/notebook_io.py
+-rw-r--r--   0        0        0     5864 2023-06-06 20:35:25.703304 paradigm-flood-0.2.5/flood/user_io/outputs.py
+-rw-r--r--   0        0        0     1919 2023-06-22 00:43:46.791751 paradigm-flood-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      381 2023-06-04 20:35:57.569281 paradigm-flood-0.2.5/tests/README.md
+-rw-r--r--   0        0        0      993 2023-06-06 21:03:30.304627 paradigm-flood-0.2.5/tests/conftest.py
+-rw-r--r--   0        0        0      593 2023-06-04 20:53:58.379044 paradigm-flood-0.2.5/tests/test_env_vars.py
+-rw-r--r--   0        0        0      269 2023-06-06 21:04:00.022725 paradigm-flood-0.2.5/tests/test_equality_tests.py
+-rw-r--r--   0        0        0     1128 2023-06-06 21:03:47.012574 paradigm-flood-0.2.5/tests/test_load_tests.py
+-rw-r--r--   0        0        0     1736 2023-06-04 16:00:15.996050 paradigm-flood-0.2.5/tests/test_node_parsing.py
+-rw-r--r--   0        0        0     4526 1970-01-01 00:00:00.000000 paradigm-flood-0.2.5/PKG-INFO
```

### Comparing `paradigm-flood-0.2.4/.github/ISSUE_TEMPLATE/bug_report.md` & `paradigm-flood-0.2.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/.github/ISSUE_TEMPLATE/feature_request.md` & `paradigm-flood-0.2.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/.github/PULL_REQUEST_TEMPLATE.md` & `paradigm-flood-0.2.5/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/.github/workflows/tests.yml` & `paradigm-flood-0.2.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/CONTRIBUTING.md` & `paradigm-flood-0.2.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/Dockerfile` & `paradigm-flood-0.2.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/LICENSE-APACHE` & `paradigm-flood-0.2.5/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/LICENSE-MIT` & `paradigm-flood-0.2.5/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/README.md` & `paradigm-flood-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/assets/cover.png` & `paradigm-flood-0.2.5/assets/cover.png`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/examples/report.sh` & `paradigm-flood-0.2.5/examples/report.sh`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/__init__.py` & `paradigm-flood-0.2.5/flood/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .generators import *
 from .runners import *
 from .spec import *
 from .tests import *
 from .user_io import *
 
 
-__version__ = '0.2.4'
+__version__ = '0.2.5'
 
 
 def _clean_package_imports() -> None:
     """remove deep nested modules from flood namespace"""
 
     import sys
```

### Comparing `paradigm-flood-0.2.4/flood/cli/cli_run.py` & `paradigm-flood-0.2.5/flood/cli/cli_run.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/cli/ls_command.py` & `paradigm-flood-0.2.5/flood/cli/ls_command.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/cli/print_command.py` & `paradigm-flood-0.2.5/flood/cli/print_command.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/cli/report_command.py` & `paradigm-flood-0.2.5/flood/cli/report_command.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/cli/root_command.py` & `paradigm-flood-0.2.5/flood/cli/root_command.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/cli/samples_collect_command.py` & `paradigm-flood-0.2.5/flood/cli/samples_collect_command.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/cli/samples_download_command.py` & `paradigm-flood-0.2.5/flood/cli/samples_download_command.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/cli/samples_ls_command.py` & `paradigm-flood-0.2.5/flood/cli/samples_ls_command.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/generators/object_generators/address_generators.py` & `paradigm-flood-0.2.5/flood/generators/object_generators/address_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/generators/object_generators/block_generators.py` & `paradigm-flood-0.2.5/flood/generators/object_generators/block_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/generators/object_generators/call_generators.py` & `paradigm-flood-0.2.5/flood/generators/object_generators/call_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/generators/object_generators/timing_generators.py` & `paradigm-flood-0.2.5/flood/generators/object_generators/timing_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/generators/raw_data_sources/raw_download_utils.py` & `paradigm-flood-0.2.5/flood/generators/raw_data_sources/raw_download_utils.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/generators/raw_data_sources/raw_gather_utils.py` & `paradigm-flood-0.2.5/flood/generators/raw_data_sources/raw_gather_utils.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/generators/raw_data_sources/raw_sample_loading.py` & `paradigm-flood-0.2.5/flood/generators/raw_data_sources/raw_sample_loading.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/generators/rng_utils.py` & `paradigm-flood-0.2.5/flood/generators/rng_utils.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/generators/test_generators/address_test_generators.py` & `paradigm-flood-0.2.5/flood/generators/test_generators/address_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/generators/test_generators/block_test_generators.py` & `paradigm-flood-0.2.5/flood/generators/test_generators/block_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/generators/test_generators/contract_test_generators.py` & `paradigm-flood-0.2.5/flood/generators/test_generators/contract_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/generators/test_generators/generic_test_generators.py` & `paradigm-flood-0.2.5/flood/generators/test_generators/generic_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/generators/test_generators/log_test_generators.py` & `paradigm-flood-0.2.5/flood/generators/test_generators/log_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/generators/test_generators/trace_test_generators.py` & `paradigm-flood-0.2.5/flood/generators/test_generators/trace_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/generators/test_generators/transaction_test_generators.py` & `paradigm-flood-0.2.5/flood/generators/test_generators/transaction_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/runners/generic_runner/generic_runner_execution.py` & `paradigm-flood-0.2.5/flood/runners/generic_runner/generic_runner_execution.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/runners/multi_runner/multi_runner_io.py` & `paradigm-flood-0.2.5/flood/runners/multi_runner/multi_runner_io.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/runners/single_runner/single_runner_execution.py` & `paradigm-flood-0.2.5/flood/runners/single_runner/single_runner_execution.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/runners/single_runner/single_runner_io.py` & `paradigm-flood-0.2.5/flood/runners/single_runner/single_runner_io.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/runners/single_runner/single_runner_summary.py` & `paradigm-flood-0.2.5/flood/runners/single_runner/single_runner_summary.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/spec.py` & `paradigm-flood-0.2.5/flood/spec.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/tests/equality_tests/equality_test_runs.py` & `paradigm-flood-0.2.5/flood/tests/equality_tests/equality_test_runs.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/tests/equality_tests/equality_test_sets.py` & `paradigm-flood-0.2.5/flood/tests/equality_tests/equality_test_sets.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,23 @@
                 },
                 'function_parameters': [
                     '0x5d3a536e4d6dbd6114cc1ead35777bab948e3643'
                 ],
                 'block_number': start_block,
             },
         ),
+        (
+            'eth_feeHistory',
+            ctc.rpc.construct_eth_fee_history,
+            [
+                512,
+                int(start_block),
+            ],
+            {},
+        ),
     ]
 
 
 def get_trace_equality_tests(
     start_block: int = 10_000_000,
     end_block: int = 16_000_000,
     random_seed: flood.RandomSeed | None = None,
```

### Comparing `paradigm-flood-0.2.4/flood/tests/load_tests/load_test_construction.py` & `paradigm-flood-0.2.5/flood/tests/load_tests/load_test_construction.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/tests/load_tests/load_test_plots.py` & `paradigm-flood-0.2.5/flood/tests/load_tests/load_test_plots.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/tests/load_tests/load_test_reports.py` & `paradigm-flood-0.2.5/flood/tests/load_tests/load_test_reports.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/tests/load_tests/load_test_runs.py` & `paradigm-flood-0.2.5/flood/tests/load_tests/load_test_runs.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/tests/load_tests/vegeta.py` & `paradigm-flood-0.2.5/flood/tests/load_tests/vegeta.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/user_io/inputs.py` & `paradigm-flood-0.2.5/flood/user_io/inputs.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/user_io/notebook_io.py` & `paradigm-flood-0.2.5/flood/user_io/notebook_io.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/flood/user_io/outputs.py` & `paradigm-flood-0.2.5/flood/user_io/outputs.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/pyproject.toml` & `paradigm-flood-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/tests/conftest.py` & `paradigm-flood-0.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/tests/test_env_vars.py` & `paradigm-flood-0.2.5/tests/test_env_vars.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/tests/test_load_tests.py` & `paradigm-flood-0.2.5/tests/test_load_tests.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/tests/test_node_parsing.py` & `paradigm-flood-0.2.5/tests/test_node_parsing.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.4/PKG-INFO` & `paradigm-flood-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradigm-flood
-Version: 0.2.4
+Version: 0.2.5
 Summary: tool for benchmarking RPC endpoints
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
```

