# Comparing `tmp/wop-2.5.2.tar.gz` & `tmp/wop-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\rlafage\workspace\WhatsOpt-CLI\dist\.tmp-oewp0oft\wop-2.5.2.tar", last modified: Tue Jun 27 13:05:59 2023, max compression
+gzip compressed data, was "wop-2.5.3.tar", last modified: Tue Jun 27 13:36:46 2023, max compression
```

## Comparing `wop-2.5.2.tar` & `wop-2.5.3.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.395113 wop-2.5.2/
-drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.194065 wop-2.5.2/.github/
-drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.215066 wop-2.5.2/.github/workflows/
--rw-rw-rw-   0        0        0      729 2023-06-27 09:24:47.000000 wop-2.5.2/.github/workflows/publish.yml
--rw-rw-rw-   0        0        0      926 2023-06-27 09:48:35.000000 wop-2.5.2/.github/workflows/tests.yml
--rw-rw-rw-   0        0        0     1395 2022-08-17 14:04:44.000000 wop-2.5.2/.gitignore
--rw-rw-rw-   0        0        0     9757 2023-06-27 09:01:10.000000 wop-2.5.2/CHANGELOG
--rw-rw-rw-   0        0        0    11558 2019-10-20 20:51:42.000000 wop-2.5.2/LICENSE
--rw-rw-rw-   0        0        0     2786 2023-06-27 13:05:59.394115 wop-2.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     1786 2021-05-16 20:10:24.000000 wop-2.5.2/README.md
--rw-rw-rw-   0        0        0     1538 2023-06-27 13:05:42.000000 wop-2.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-27 13:05:59.395113 wop-2.5.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.231068 wop-2.5.2/tests/
-drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.291598 wop-2.5.2/tests/data/
--rw-rw-rw-   0        0        0     1004 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/disc1.py
--rw-rw-rw-   0        0        0      650 2022-01-28 17:02:42.000000 wop-2.5.2/tests/data/disc1_base.py
--rw-rw-rw-   0        0        0      114 2021-05-16 16:24:08.000000 wop-2.5.2/tests/data/disc1_problem.py
--rw-rw-rw-   0        0        0      758 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/fonctions_base.py
--rw-rw-rw-   0        0        0      334 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/mda_init.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.320129 wop-2.5.2/tests/data/multipoint_beam/
--rw-rw-rw-   0        0        0       78 2020-06-08 09:44:01.000000 wop-2.5.2/tests/data/multipoint_beam/__init__.py
--rw-rw-rw-   0        0        0      918 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/i_comp.py
--rw-rw-rw-   0        0        0      603 2022-01-28 17:02:42.000000 wop-2.5.2/tests/data/multipoint_beam/i_comp_base.py
--rw-rw-rw-   0        0        0      933 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/interp.py
--rw-rw-rw-   0        0        0      619 2022-01-28 17:02:42.000000 wop-2.5.2/tests/data/multipoint_beam/interp_base.py
--rw-rw-rw-   0        0        0     1111 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/local_stiffness_matrix_comp.py
--rw-rw-rw-   0        0        0      671 2022-01-28 17:02:42.000000 wop-2.5.2/tests/data/multipoint_beam/local_stiffness_matrix_comp_base.py
--rw-rw-rw-   0        0        0     1656 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/multipoint_beam_group.py
--rw-rw-rw-   0        0        0     4093 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/multipoint_beam_group_base.py
--rw-rw-rw-   0        0        0     1070 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/obj_sum.py
--rw-rw-rw-   0        0        0      683 2022-01-28 17:02:42.000000 wop-2.5.2/tests/data/multipoint_beam/obj_sum_base.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.327112 wop-2.5.2/tests/data/multipoint_beam/parallel/
--rw-rw-rw-   0        0        0       78 2020-06-08 09:44:01.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/__init__.py
--rw-rw-rw-   0        0        0     1692 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/parallel.py
--rw-rw-rw-   0        0        0     2296 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/parallel_base.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.346114 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/
--rw-rw-rw-   0        0        0       78 2020-06-08 09:44:01.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/__init__.py
--rw-rw-rw-   0        0        0     1406 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/compliance_comp.py
--rw-rw-rw-   0        0        0      765 2022-01-28 17:02:42.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/compliance_comp_base.py
--rw-rw-rw-   0        0        0     1391 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/displacements_comp.py
--rw-rw-rw-   0        0        0      760 2022-01-28 17:02:42.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/displacements_comp_base.py
--rw-rw-rw-   0        0        0     1107 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/states_comp.py
--rw-rw-rw-   0        0        0    11260 2022-01-28 17:02:42.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/states_comp_base.py
--rw-rw-rw-   0        0        0     1645 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/sub0.py
--rw-rw-rw-   0        0        0     2677 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/sub0_base.py
--rw-rw-rw-   0        0        0      446 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/run_analysis.py
--rw-rw-rw-   0        0        0      381 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/run_parameters_init.py
--rw-rw-rw-   0        0        0      971 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/volume_comp.py
--rw-rw-rw-   0        0        0      622 2022-01-28 17:02:42.000000 wop-2.5.2/tests/data/multipoint_beam/volume_comp_base.py
--rw-rw-rw-   0        0        0    21993 2020-09-09 21:57:34.000000 wop-2.5.2/tests/data/multipoint_beam_group_d0.json
--rw-rw-rw-   0        0        0    10911 2020-09-09 21:57:28.000000 wop-2.5.2/tests/data/multipoint_beam_group_d1.json
--rw-rw-rw-   0        0        0    17820 2020-09-09 21:57:31.000000 wop-2.5.2/tests/data/multipoint_beam_group_d2.json
--rw-rw-rw-   0        0        0      222 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/run_mda.py
--rw-rw-rw-   0        0        0      161 2020-03-10 17:19:07.000000 wop-2.5.2/tests/data/sellar.py
--rw-rw-rw-   0        0        0     3224 2020-03-10 17:19:07.000000 wop-2.5.2/tests/data/test_doe.csv
--rw-rw-rw-   0        0        0   161472 2021-07-21 12:19:20.000000 wop-2.5.2/tests/data/test_doe.hdf5
--rw-rw-rw-   0        0        0    98304 2020-06-08 09:44:01.000000 wop-2.5.2/tests/data/test_doe.sqlite
--rw-rw-rw-   0        0        0    98304 2020-06-08 09:44:01.000000 wop-2.5.2/tests/data/test_parallel_doe.sqlite_0
--rw-rw-rw-   0        0        0    98304 2020-06-08 09:44:01.000000 wop-2.5.2/tests/data/test_parallel_doe.sqlite_1
--rw-rw-rw-   0        0        0    98304 2020-06-08 09:44:01.000000 wop-2.5.2/tests/data/test_parallel_doe.sqlite_2
--rw-rw-rw-   0        0        0     3779 2020-06-08 09:44:01.000000 wop-2.5.2/tests/data/test_push_cut_flatten.json
--rw-rw-rw-   0        0        0      222 2022-02-21 15:06:38.000000 wop-2.5.2/tests/data/wop_format_v1
--rw-rw-rw-   0        0        0      254 2022-02-21 15:06:38.000000 wop-2.5.2/tests/data/wop_format_v2
--rw-rw-rw-   0        0        0      394 2022-02-21 15:06:38.000000 wop-2.5.2/tests/data/wop_ref
--rw-rw-rw-   0        0        0      517 2023-03-20 14:35:21.000000 wop-2.5.2/tests/test_convert_utils.py
--rw-rw-rw-   0        0        0      476 2022-06-10 09:28:53.000000 wop-2.5.2/tests/test_mooptimization.py
--rw-rw-rw-   0        0        0     2170 2023-03-20 14:35:21.000000 wop-2.5.2/tests/test_push_command.py
--rw-rw-rw-   0        0        0     2960 2023-03-20 14:35:21.000000 wop-2.5.2/tests/test_push_utils.py
--rw-rw-rw-   0        0        0     3452 2023-03-20 14:35:21.000000 wop-2.5.2/tests/test_upload_utils.py
--rw-rw-rw-   0        0        0     3872 2023-03-20 14:35:21.000000 wop-2.5.2/tests/test_utils.py
--rw-rw-rw-   0        0        0      350 2022-02-21 15:06:38.000000 wop-2.5.2/tests/test_whatsopt_client.py
--rw-rw-rw-   0        0        0     2108 2023-03-20 14:35:21.000000 wop-2.5.2/tests/test_wop.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.376113 wop-2.5.2/whatsopt/
--rw-rw-rw-   0        0        0       23 2023-06-27 09:48:35.000000 wop-2.5.2/whatsopt/__init__.py
--rw-rw-rw-   0        0        0     1493 2021-10-07 14:47:53.000000 wop-2.5.2/whatsopt/convert_utils.py
--rw-rw-rw-   0        0        0      502 2022-06-02 07:27:07.000000 wop-2.5.2/whatsopt/logging.py
--rw-rw-rw-   0        0        0     3186 2022-06-10 09:28:53.000000 wop-2.5.2/whatsopt/mooptimization.py
--rw-rw-rw-   0        0        0    11578 2023-03-20 14:35:21.000000 wop-2.5.2/whatsopt/optimization.py
--rw-rw-rw-   0        0        0      422 2023-06-05 19:01:08.000000 wop-2.5.2/whatsopt/publish_utils.py
--rw-rw-rw-   0        0        0    15185 2023-03-20 14:35:21.000000 wop-2.5.2/whatsopt/push_command.py
--rw-rw-rw-   0        0        0     5644 2023-03-19 12:20:40.000000 wop-2.5.2/whatsopt/push_utils.py
--rw-rw-rw-   0        0        0     1483 2021-06-21 11:38:00.000000 wop-2.5.2/whatsopt/show_utils.py
--rw-rw-rw-   0        0        0     7448 2022-06-29 16:15:18.000000 wop-2.5.2/whatsopt/upload_utils.py
--rw-rw-rw-   0        0        0     6025 2023-05-15 12:58:25.000000 wop-2.5.2/whatsopt/utils.py
--rw-rw-rw-   0        0        0    40787 2023-06-27 09:01:10.000000 wop-2.5.2/whatsopt/whatsopt_client.py
--rw-rw-rw-   0        0        0    13395 2023-06-05 19:01:08.000000 wop-2.5.2/whatsopt/wop.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.392113 wop-2.5.2/wop.egg-info/
--rw-rw-rw-   0        0        0     2786 2023-06-27 13:05:58.000000 wop-2.5.2/wop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2738 2023-06-27 13:05:59.000000 wop-2.5.2/wop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 13:05:58.000000 wop-2.5.2/wop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-27 13:05:58.000000 wop-2.5.2/wop.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      146 2023-06-27 13:05:58.000000 wop-2.5.2/wop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-27 13:05:58.000000 wop-2.5.2/wop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:46.727261 wop-2.5.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:46.715261 wop-2.5.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:46.719261 wop-2.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-27 13:36:36.000000 wop-2.5.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-27 13:36:36.000000 wop-2.5.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-27 13:36:36.000000 wop-2.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-06-27 13:36:36.000000 wop-2.5.3/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 13:36:36.000000 wop-2.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-27 13:36:46.727261 wop-2.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-27 13:36:36.000000 wop-2.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-27 13:36:36.000000 wop-2.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:36:46.727261 wop-2.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:46.719261 wop-2.5.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:46.723261 wop-2.5.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/disc1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/disc1_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/disc1_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/fonctions_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/mda_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:46.723261 wop-2.5.3/tests/data/multipoint_beam/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/i_comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/i_comp_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/interp_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/local_stiffness_matrix_comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/local_stiffness_matrix_comp_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/multipoint_beam_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/multipoint_beam_group_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/obj_sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/obj_sum_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:46.723261 wop-2.5.3/tests/data/multipoint_beam/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/parallel/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/parallel/parallel_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:46.723261 wop-2.5.3/tests/data/multipoint_beam/parallel/sub0/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/parallel/sub0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/parallel/sub0/compliance_comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/parallel/sub0/compliance_comp_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/parallel/sub0/displacements_comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/parallel/sub0/displacements_comp_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/parallel/sub0/states_comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10930 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/parallel/sub0/states_comp_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/parallel/sub0/sub0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/parallel/sub0/sub0_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/run_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/run_parameters_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/volume_comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam/volume_comp_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21525 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam_group_d0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam_group_d1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/multipoint_beam_group_d2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/run_mda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/sellar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/test_doe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   161472 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/test_doe.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/test_doe.sqlite
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/test_parallel_doe.sqlite_0
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/test_parallel_doe.sqlite_1
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/test_parallel_doe.sqlite_2
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/test_push_cut_flatten.json
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/wop_format_v1
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/wop_format_v2
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-27 13:36:36.000000 wop-2.5.3/tests/data/wop_ref
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-27 13:36:36.000000 wop-2.5.3/tests/test_convert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-27 13:36:36.000000 wop-2.5.3/tests/test_mooptimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-27 13:36:36.000000 wop-2.5.3/tests/test_push_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-27 13:36:36.000000 wop-2.5.3/tests/test_push_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-27 13:36:36.000000 wop-2.5.3/tests/test_upload_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-06-27 13:36:36.000000 wop-2.5.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 13:36:36.000000 wop-2.5.3/tests/test_whatsopt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-27 13:36:36.000000 wop-2.5.3/tests/test_wop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:46.727261 wop-2.5.3/whatsopt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 13:36:36.000000 wop-2.5.3/whatsopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-27 13:36:36.000000 wop-2.5.3/whatsopt/convert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-27 13:36:36.000000 wop-2.5.3/whatsopt/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-27 13:36:36.000000 wop-2.5.3/whatsopt/mooptimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-06-27 13:36:36.000000 wop-2.5.3/whatsopt/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-27 13:36:36.000000 wop-2.5.3/whatsopt/publish_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-06-27 13:36:36.000000 wop-2.5.3/whatsopt/push_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-06-27 13:36:36.000000 wop-2.5.3/whatsopt/push_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-27 13:36:36.000000 wop-2.5.3/whatsopt/show_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-06-27 13:36:36.000000 wop-2.5.3/whatsopt/upload_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-27 13:36:36.000000 wop-2.5.3/whatsopt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39724 2023-06-27 13:36:36.000000 wop-2.5.3/whatsopt/whatsopt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12881 2023-06-27 13:36:36.000000 wop-2.5.3/whatsopt/wop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:36:46.727261 wop-2.5.3/wop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-27 13:36:46.000000 wop-2.5.3/wop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-27 13:36:46.000000 wop-2.5.3/wop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:36:46.000000 wop-2.5.3/wop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 13:36:46.000000 wop-2.5.3/wop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-27 13:36:46.000000 wop-2.5.3/wop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 13:36:46.000000 wop-2.5.3/wop.egg-info/top_level.txt
```

### Comparing `wop-2.5.2/.github/workflows/publish.yml` & `wop-2.5.3/.github/workflows/tests.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,41 @@
-name: publish to PyPI
-
-on:
-  workflow_dispatch:
-  release:
-    types: [published]
-
-jobs:
-  publish:
-    name: Publish
-    runs-on: ubuntu-latest
-    steps:
-      - name: Checkout sources
-        uses: actions/checkout@v3
-
-      - name: Set up Python
-        uses: actions/setup-python@v2
-        with:
-          python-version: "3.8"
-
-      - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          pip install build
-          
-      - name: Build package
-        run: python -m build
-
-      - name: Publish new distributions to PyPI
-        uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.PYPI_WOP_API_TOKEN }}
+name: Tests
+
+on:
+  push:
+    branches: [ master ]
+  pull_request:
+    branches: [ master ]
+
+jobs:
+  build:
+
+    runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        os: [ubuntu-latest, windows-latest, macos-latest]
+        python-version: ["3.8", "3.9", "3.10"]
+
+    steps:
+    - name: Checkout sources
+      uses: actions/checkout@v3
+
+    - name: Set up Python ${{ matrix.python-version }}
+      uses: actions/setup-python@v2
+      with:
+        python-version: ${{ matrix.python-version }}
+
+    - name: Install dependencies 
+      run: |
+        python -m pip install --upgrade pip
+        python -m pip install black pytest
+        if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
+        pip install .
+
+    - name: Format with black
+      run: |
+        black --version --diff --check whatsopt
+
+    - name: Test with pytest
+      run: |
+        pytest
+
```

### Comparing `wop-2.5.2/CHANGELOG` & `wop-2.5.3/CHANGELOG`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-* 2.5.1 (05/06/2023)
-  * `wop build`: Remove annoying `BetaConfiguration` warning  
-  * `wop pull <source_id>`: Fix bug pull source not working
-
-* 2.5.0 (16/05/2023) 
-  * `wop merge <source_id>`: Now only import the source analysis disciplines in the current 
-  analysis on WhatsOpt (previously was also doing the fetching).
-  * `wop pull`: 
-    * Now default is package mode (before `--package` option was required). 
-    Old plain mode is still available with `--plain` option. 
-    * `wop pull <source_id>`: was previously `wop merge <source_id>`. 
-    Now `wop pull <source_id>` is equivalent of `wop merge <source_id>` + `wop fetch <source_id>`
-  * `wop fetch`: Fixed when there is no package an error is raised, now just no-op.  
-
-* 2.4.0 (15/05/2023)
-  * `wop fetch <source_id>`: this command gets disciplines source code from source analysis and extract 
-  it within the current analysis Python module. The current analysis is untouched on WhatsOpt.
-  * `wop merge <source_id>`: this command import the source analysis discipline within the current one 
-  on WhatsOpt fetch source analysis code and finally update the code.
-
-* 2.3.0 (08/04/2023)
-  * `wop build`: Add command to build Python package with the analysis code.
-  * `wop publish`: Add command to build and publish the package on WhatsOpt.
-
-* 2.2.1 (20/03/2023)
-  * `wop upload mda_init.py`: Fix the upload of the parameter values of the analysis.
-
-* 2.2.0 (17/08/2022)
-  * requires: Python 3.7+, openmdao_extensions 1.1.0+
-  * `wop push`: When creating pseudo-variables related to connections created with OpenMDAO connect()
-  method, variable name length is now limited to 255.
-
-* 2.1.2 (30/06/2022)
-  * `wop upload`: Add checking on to-be-uploaded file existence and 
-  file content (have to contain design variables and output records)
-
-* 2.1.1 (23/06/2022)
-  * Fix `wop upload --parallel`: bad file extension check which prevents from uploading 
-  * Fix `wop convert <.sqlite_\d+>`: bad error message when used with sqlite generated in parallel  
-
-* 2.1.0 (19/06/2022)
-  * Refactor optimization REST API to use mixed-integer multi-objective ONERA in-house optimizer (WhatsOpt 1.23+)
-  
-* 2.0.2 (14/05/2022)
-  * Fix login handling in remote optimization
-  
-* 2.0.1 (12/04/2022)
-  * Fix login edge case logic and remote servers handling
-
-* 2.0.0 (14/03/2022)
-  * Now `wop` stores successful remote servers (a.k.a remotes) login infos. For instance, after a successful login sequence with `wop login https://remote.example.com` and API key input, next login to this url will be simply done automatically with `wop login remote`.
-  * New command options:
-    * `wop list/logout -r`: lists known remotes.
-    * `wop logout -r <name>`: remove remote info specified by its name.
-    * `wop logout --all`: remove all remotes infos. 
-  * API change: 
-    * `whatsopt_client.WhatsOpt()`: `login` keyword argument is deprecated. 
-      `WhatsOpt(login=False)` should be replaced by `WhatsOpt()` with further wop versions.
-  * **Breaking changes**: 
-    * Now `WhatsOpt()` does not "log in" automatically: 
-      * `WhatsOpt()` or `WhatsOpt(login=True)` has to be replaced by `WhatsOpt.login()`
-    * Remove `PROD_URL`, `INTRANET_SERVER_URL` constants
-    * Remove `default_url` property
-
-* 1.21.2 (12/02/2022)
-  * Fix `wop update` performance issue: avoid requesting package name when not required
-  * **wop versions < 1.21 are deprecated**, support will be removed with WhatsOpt 1.22
-
-* 1.21.1 (28/01/2022)
-  * Add short options `-h` and `-v` for respectively `--help` and `--version`
-  * Fixes:
-    - On update, when removed do not regenerate scripts and discipline unit tests 
-    unless relevant option (respectively `-r` or `-t`) is present. 
-    - On update, when removed do not regenerate user files: setup.py, README, .gitignore 
-
-* 1.21.0 (04/01/2022)
-  - `wop pull --package <id>`: allows to generate code in _package mode_ meaning 
-  generate proper directory structure and `setup.py` to allow code distribution as a Python package
-  (only available with OpenMDAO framework at the moment). 
-
-* 1.20.1 (15/12/2021)
-  - Creation of dedicated file `.wop` which contains wop pull/update state
-  (eg. whatsopt url, analysis id, etc.)  
-
-* 1.20.0 (22/11/2021)
-  - `wop push`: `--old` option triggering old deprecated implementation is removed  
-  - `wop pull / wop update -r`: with WhatsOpt > 1.18.0, pull / update `run_mda.py`, `run_mdo.py`, `mda_init.py` 
-    (`run_analysis.py`, `run_optimization.py`, `run_parameters_init.py` are removed). 
-  - `wop upload mda_init.py`: upload analysis variables initialization.
-
-* 1.19.0 (07/10/2021)
-  - `wop update --egmdo`: generate code and scripts related to EGMDO method.
-  - `wop convert <sqlite_filename>`: convert given OpenMDAO sqlite to csv file format  
-
-* 1.18.0 (06/08/2021)
-  - `wop pull --json --project-id <ident>`: pull project given its identifier as json on stdout
-  - `wop push --json <project.json>`: create project from project json file  
-
-* 1.17.0 (18/08/2021)
-  - `wop upload <datafile.hdf5>`: upload data generated from GEMSEO scenario execution. 
-
-* 1.16.1 (20/07/2021)
-  - Fix `push` command to take into account value-to-val renaming in `meta` dict in OpenMDAO 3.10
-
-* 1.16.0 (07/07/2021)
-  - Change `wop upload` by using case outputs (instead of objective and constraints)
-  to get all recorded responses. 
-
-* 1.15.4 (05/07/2021)
-  - Fix regexp using `import` keyword to detect execution framework 
-
-* 1.15.3 (01/07/2021)
-  - Fix `wop update` bug when the analysis is nested: server subdirectories were not updated
-
-* 1.15.2 (01/07/2021)
-  - Fix `wop update` bug when the analysis is nested: base files in subdirectories were not updated
-
-* 1.15.1 (21/06/2021)
-  - Fix `wop show [-a]` bug related to new source parameter used to be displayed in HTML footer
-  - deprecate PROD_URL constant, replaced by INTRANET_SERVER_URL (selene)
-  - add EXTRANET_SERVER_URL constant (ether)
-
-* 1.15.0 (18/06/2021)
-  - wop show -f <openmdao_problem.py> works without logging in WhatsOpt server
-
-* 1.14.0 (15/06/2021)
-  - Refactor push command:
-    - default becomes old: wop push --old <openmdao_problem.py> (--old is temporary and will be removed in a future release)
-    - experimental becomes default: -x/--experimental removed
-
-* 1.13.1 (28/05/2021)
-  - wop pull --dry-run <analysis_id>: list pull actions but do not execute
-  - wop update --gemseo/--openmdao: to switch between the two frameworks
-  - wop status: display detected framework, remove notes
-
-* 1.13.0 (25/05/2021)
-  - wop pull --gemseo <analysis_id>: to generate GEMSEO code instead of OpenMDAO one (default)
-  - wop serve -p <port_number>: to run analysis server on port port_number
-
-* 1.12.0 (05/10/2020)
-  - wop list: list analyses owned by the user
-  - wop list -a: list all analyses available for the user
-  - wop list -p project: list all analyses available for the user of the given project substring
-  - remove wop url (not really used and not relevant anymore with wop status)
-  - fix OpenMDAO 3.4 compatibility
-  - require OpenMDAO >= 3.4, xdsmjs>=1.0.0
-
-* 1.11.0 (23/09/2020)
-  - wop pull: add --json option to dump pushable analysis json format 
-  - wop push: add --json option to import analysis from json format 
-
-* 1.10.0 (18/06/2020)
-  - new wop status command: returns the current server and pulled analysis status
-  - wop push: default depth change from 3 to 2
-  - wop show: add --experimental option to allow showing any openmdao code
-
-* 1.9.0 (08/06/2020)
-  - wop push: 
-    - add --experimental (-x) push option allowing to push any code for reverse-engineering only
-    - add --depth <n> push only n levels of sub-analyses (0 means no limit, default is 3)
-    - Know bug: -d option using -x experimental push can lead to duplicate variables
-  - wop show:
-    - add --depth option (see push command above)  
-
-* 1.8.0 (20/04/2020)
-  - wop show: display XDSM of given analysis :
-    - either an existing on the remote server (-a option)
-    - or by specifying an openmdao problem python file (-f option)
-    - otherwise use current analysis from code (previously generated with wop pull)
-  - require openmdao_extensions >= 1.0.0, openmdao >= 3.0.0
-
-* 1.7.0 (15/04/2020)
-  - wop push: add -c component option allowing to push one OpenMDAO component
-
-* 1.6.0 (05/04/2020)
-  - add API for WhatsOpt SEGOMOE optimization
-
-* 1.5.0 (18/03/2020)
-  - fix upload and push commands using OpenMDAO >= 2.10 hooks
-  - drop Python 2.7 support
-
-* 1.4.0 (27/02/2020)
-  - wop upload: work with WhatsOpt >= 1.6
-  - wop upload: -p option to upload sqlite files generated by parallel doe run
-  - wop upload: user can upload run_parameter_init 
-  - wop upload: user can upload parallel doe results
-  - add short name options
-  - add message coloring
-  - refactoring and automated tests
-
-* 1.3.0 (04/10/2019)
-  - wop pull/update: download file as required by analysis definition
-  (e.g. download optimization script if an objective is defined or 
-  pull new files if a new discipline is defined, etc.)
-  - higlight messages according to their log level (info, warn or error)
-
-* 1.2.0 (24/09/2019)
-  - wop upload: filter nan and inf, add --only-success option
-
-* 1.1.0 (28/08/2019)
-  - add csv data upload as DOE execution of an existing analysis
-  - add csv data upload without any existing analysis (an ad hoc one is created)
-  - add --outvar-count upload option used to pass output variable number when uploading
-  data in csv format (default is 1).
-  - remove upload --cleanup option
-
-* 1.0.0 (20/06/2019)
-  - version for AIAA Aviation 2019 (17-21th Dallas TX)
+* 2.5.1 (05/06/2023)
+  * `wop build`: Remove annoying `BetaConfiguration` warning  
+  * `wop pull <source_id>`: Fix bug pull source not working
+
+* 2.5.0 (16/05/2023) 
+  * `wop merge <source_id>`: Now only import the source analysis disciplines in the current 
+  analysis on WhatsOpt (previously was also doing the fetching).
+  * `wop pull`: 
+    * Now default is package mode (before `--package` option was required). 
+    Old plain mode is still available with `--plain` option. 
+    * `wop pull <source_id>`: was previously `wop merge <source_id>`. 
+    Now `wop pull <source_id>` is equivalent of `wop merge <source_id>` + `wop fetch <source_id>`
+  * `wop fetch`: Fixed when there is no package an error is raised, now just no-op.  
+
+* 2.4.0 (15/05/2023)
+  * `wop fetch <source_id>`: this command gets disciplines source code from source analysis and extract 
+  it within the current analysis Python module. The current analysis is untouched on WhatsOpt.
+  * `wop merge <source_id>`: this command import the source analysis discipline within the current one 
+  on WhatsOpt fetch source analysis code and finally update the code.
+
+* 2.3.0 (08/04/2023)
+  * `wop build`: Add command to build Python package with the analysis code.
+  * `wop publish`: Add command to build and publish the package on WhatsOpt.
+
+* 2.2.1 (20/03/2023)
+  * `wop upload mda_init.py`: Fix the upload of the parameter values of the analysis.
+
+* 2.2.0 (17/08/2022)
+  * requires: Python 3.7+, openmdao_extensions 1.1.0+
+  * `wop push`: When creating pseudo-variables related to connections created with OpenMDAO connect()
+  method, variable name length is now limited to 255.
+
+* 2.1.2 (30/06/2022)
+  * `wop upload`: Add checking on to-be-uploaded file existence and 
+  file content (have to contain design variables and output records)
+
+* 2.1.1 (23/06/2022)
+  * Fix `wop upload --parallel`: bad file extension check which prevents from uploading 
+  * Fix `wop convert <.sqlite_\d+>`: bad error message when used with sqlite generated in parallel  
+
+* 2.1.0 (19/06/2022)
+  * Refactor optimization REST API to use mixed-integer multi-objective ONERA in-house optimizer (WhatsOpt 1.23+)
+  
+* 2.0.2 (14/05/2022)
+  * Fix login handling in remote optimization
+  
+* 2.0.1 (12/04/2022)
+  * Fix login edge case logic and remote servers handling
+
+* 2.0.0 (14/03/2022)
+  * Now `wop` stores successful remote servers (a.k.a remotes) login infos. For instance, after a successful login sequence with `wop login https://remote.example.com` and API key input, next login to this url will be simply done automatically with `wop login remote`.
+  * New command options:
+    * `wop list/logout -r`: lists known remotes.
+    * `wop logout -r <name>`: remove remote info specified by its name.
+    * `wop logout --all`: remove all remotes infos. 
+  * API change: 
+    * `whatsopt_client.WhatsOpt()`: `login` keyword argument is deprecated. 
+      `WhatsOpt(login=False)` should be replaced by `WhatsOpt()` with further wop versions.
+  * **Breaking changes**: 
+    * Now `WhatsOpt()` does not "log in" automatically: 
+      * `WhatsOpt()` or `WhatsOpt(login=True)` has to be replaced by `WhatsOpt.login()`
+    * Remove `PROD_URL`, `INTRANET_SERVER_URL` constants
+    * Remove `default_url` property
+
+* 1.21.2 (12/02/2022)
+  * Fix `wop update` performance issue: avoid requesting package name when not required
+  * **wop versions < 1.21 are deprecated**, support will be removed with WhatsOpt 1.22
+
+* 1.21.1 (28/01/2022)
+  * Add short options `-h` and `-v` for respectively `--help` and `--version`
+  * Fixes:
+    - On update, when removed do not regenerate scripts and discipline unit tests 
+    unless relevant option (respectively `-r` or `-t`) is present. 
+    - On update, when removed do not regenerate user files: setup.py, README, .gitignore 
+
+* 1.21.0 (04/01/2022)
+  - `wop pull --package <id>`: allows to generate code in _package mode_ meaning 
+  generate proper directory structure and `setup.py` to allow code distribution as a Python package
+  (only available with OpenMDAO framework at the moment). 
+
+* 1.20.1 (15/12/2021)
+  - Creation of dedicated file `.wop` which contains wop pull/update state
+  (eg. whatsopt url, analysis id, etc.)  
+
+* 1.20.0 (22/11/2021)
+  - `wop push`: `--old` option triggering old deprecated implementation is removed  
+  - `wop pull / wop update -r`: with WhatsOpt > 1.18.0, pull / update `run_mda.py`, `run_mdo.py`, `mda_init.py` 
+    (`run_analysis.py`, `run_optimization.py`, `run_parameters_init.py` are removed). 
+  - `wop upload mda_init.py`: upload analysis variables initialization.
+
+* 1.19.0 (07/10/2021)
+  - `wop update --egmdo`: generate code and scripts related to EGMDO method.
+  - `wop convert <sqlite_filename>`: convert given OpenMDAO sqlite to csv file format  
+
+* 1.18.0 (06/08/2021)
+  - `wop pull --json --project-id <ident>`: pull project given its identifier as json on stdout
+  - `wop push --json <project.json>`: create project from project json file  
+
+* 1.17.0 (18/08/2021)
+  - `wop upload <datafile.hdf5>`: upload data generated from GEMSEO scenario execution. 
+
+* 1.16.1 (20/07/2021)
+  - Fix `push` command to take into account value-to-val renaming in `meta` dict in OpenMDAO 3.10
+
+* 1.16.0 (07/07/2021)
+  - Change `wop upload` by using case outputs (instead of objective and constraints)
+  to get all recorded responses. 
+
+* 1.15.4 (05/07/2021)
+  - Fix regexp using `import` keyword to detect execution framework 
+
+* 1.15.3 (01/07/2021)
+  - Fix `wop update` bug when the analysis is nested: server subdirectories were not updated
+
+* 1.15.2 (01/07/2021)
+  - Fix `wop update` bug when the analysis is nested: base files in subdirectories were not updated
+
+* 1.15.1 (21/06/2021)
+  - Fix `wop show [-a]` bug related to new source parameter used to be displayed in HTML footer
+  - deprecate PROD_URL constant, replaced by INTRANET_SERVER_URL (selene)
+  - add EXTRANET_SERVER_URL constant (ether)
+
+* 1.15.0 (18/06/2021)
+  - wop show -f <openmdao_problem.py> works without logging in WhatsOpt server
+
+* 1.14.0 (15/06/2021)
+  - Refactor push command:
+    - default becomes old: wop push --old <openmdao_problem.py> (--old is temporary and will be removed in a future release)
+    - experimental becomes default: -x/--experimental removed
+
+* 1.13.1 (28/05/2021)
+  - wop pull --dry-run <analysis_id>: list pull actions but do not execute
+  - wop update --gemseo/--openmdao: to switch between the two frameworks
+  - wop status: display detected framework, remove notes
+
+* 1.13.0 (25/05/2021)
+  - wop pull --gemseo <analysis_id>: to generate GEMSEO code instead of OpenMDAO one (default)
+  - wop serve -p <port_number>: to run analysis server on port port_number
+
+* 1.12.0 (05/10/2020)
+  - wop list: list analyses owned by the user
+  - wop list -a: list all analyses available for the user
+  - wop list -p project: list all analyses available for the user of the given project substring
+  - remove wop url (not really used and not relevant anymore with wop status)
+  - fix OpenMDAO 3.4 compatibility
+  - require OpenMDAO >= 3.4, xdsmjs>=1.0.0
+
+* 1.11.0 (23/09/2020)
+  - wop pull: add --json option to dump pushable analysis json format 
+  - wop push: add --json option to import analysis from json format 
+
+* 1.10.0 (18/06/2020)
+  - new wop status command: returns the current server and pulled analysis status
+  - wop push: default depth change from 3 to 2
+  - wop show: add --experimental option to allow showing any openmdao code
+
+* 1.9.0 (08/06/2020)
+  - wop push: 
+    - add --experimental (-x) push option allowing to push any code for reverse-engineering only
+    - add --depth <n> push only n levels of sub-analyses (0 means no limit, default is 3)
+    - Know bug: -d option using -x experimental push can lead to duplicate variables
+  - wop show:
+    - add --depth option (see push command above)  
+
+* 1.8.0 (20/04/2020)
+  - wop show: display XDSM of given analysis :
+    - either an existing on the remote server (-a option)
+    - or by specifying an openmdao problem python file (-f option)
+    - otherwise use current analysis from code (previously generated with wop pull)
+  - require openmdao_extensions >= 1.0.0, openmdao >= 3.0.0
+
+* 1.7.0 (15/04/2020)
+  - wop push: add -c component option allowing to push one OpenMDAO component
+
+* 1.6.0 (05/04/2020)
+  - add API for WhatsOpt SEGOMOE optimization
+
+* 1.5.0 (18/03/2020)
+  - fix upload and push commands using OpenMDAO >= 2.10 hooks
+  - drop Python 2.7 support
+
+* 1.4.0 (27/02/2020)
+  - wop upload: work with WhatsOpt >= 1.6
+  - wop upload: -p option to upload sqlite files generated by parallel doe run
+  - wop upload: user can upload run_parameter_init 
+  - wop upload: user can upload parallel doe results
+  - add short name options
+  - add message coloring
+  - refactoring and automated tests
+
+* 1.3.0 (04/10/2019)
+  - wop pull/update: download file as required by analysis definition
+  (e.g. download optimization script if an objective is defined or 
+  pull new files if a new discipline is defined, etc.)
+  - higlight messages according to their log level (info, warn or error)
+
+* 1.2.0 (24/09/2019)
+  - wop upload: filter nan and inf, add --only-success option
+
+* 1.1.0 (28/08/2019)
+  - add csv data upload as DOE execution of an existing analysis
+  - add csv data upload without any existing analysis (an ad hoc one is created)
+  - add --outvar-count upload option used to pass output variable number when uploading
+  data in csv format (default is 1).
+  - remove upload --cleanup option
+
+* 1.0.0 (20/06/2019)
+  - version for AIAA Aviation 2019 (17-21th Dallas TX)
```

### Comparing `wop-2.5.2/LICENSE` & `wop-2.5.3/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `wop-2.5.2/PKG-INFO` & `wop-2.5.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-Metadata-Version: 2.1
-Name: wop
-Version: 2.5.2
-Summary: My package description
-Author-email: Rémi Lafage <remi.lafage@onera.fr>
-License: Apache License 2.0
-Project-URL: homepage, https://github.com/whatsopt
-Project-URL: repository, https://github.com/whatsopt/WhatsOpt-CLI
-Project-URL: documentation, https://github.com/whatsopt/WhatsOpt-Doc#whatsopt-documentation
-Keywords: WhatsOpt,command
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
-[![Tests](https://github.com/OneraHub/WhatsOpt-CLI/workflows/Tests/badge.svg)](https://github.com/OneraHub/WhatsOpt-CLI/actions?query=workflow%3ATests)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/78559b54a0db44e5aeb5b0a3f5dcf9e2)](https://www.codacy.com/gh/OneraHub/WhatsOpt-CLI/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=OneraHub/WhatsOpt-CLI&amp;utm_campaign=Badge_Grade)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
-
-# WhatsOpt command line interface
-
-Command line interface to interact with WhatsOpt web application. See [WhatsOpt documentation](https://github.com/OneraHub/WhatsOpt-Doc).
-
-## Citation
->Rémi  Lafage,  Sébastien  Defoort,  and  Thierry  Lefèbvre. Whatsopt: a web application for multidisciplinary design analysis and optimization. In 20th AIAA/ISSMO Multidisciplinary Analysis and Optimization Conference, Dallas, United States, 2019
-
-DOI: [10.2514/6.2019-2990](https://doi.org/10.2514/6.2019-2990)
-
-## Installation
-```bash
-pip install wop
-```
-
-## Usage
-```bash
-wop --help
-```
-
-```bash
-wop <COMMAND> --help
-```
-
-## License
-
-   Copyright 2020 Rémi Lafage
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+Metadata-Version: 2.1
+Name: wop
+Version: 2.5.3
+Summary: My package description
+Author-email: Rémi Lafage <remi.lafage@onera.fr>
+License: Apache License 2.0
+Project-URL: homepage, https://github.com/whatsopt
+Project-URL: repository, https://github.com/whatsopt/WhatsOpt-CLI
+Project-URL: documentation, https://github.com/whatsopt/WhatsOpt-Doc#whatsopt-documentation
+Keywords: WhatsOpt,command
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
+[![Tests](https://github.com/OneraHub/WhatsOpt-CLI/workflows/Tests/badge.svg)](https://github.com/OneraHub/WhatsOpt-CLI/actions?query=workflow%3ATests)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/78559b54a0db44e5aeb5b0a3f5dcf9e2)](https://www.codacy.com/gh/OneraHub/WhatsOpt-CLI/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=OneraHub/WhatsOpt-CLI&amp;utm_campaign=Badge_Grade)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+
+# WhatsOpt command line interface
+
+Command line interface to interact with WhatsOpt web application. See [WhatsOpt documentation](https://github.com/OneraHub/WhatsOpt-Doc).
+
+## Citation
+>Rémi  Lafage,  Sébastien  Defoort,  and  Thierry  Lefèbvre. Whatsopt: a web application for multidisciplinary design analysis and optimization. In 20th AIAA/ISSMO Multidisciplinary Analysis and Optimization Conference, Dallas, United States, 2019
+
+DOI: [10.2514/6.2019-2990](https://doi.org/10.2514/6.2019-2990)
+
+## Installation
+```bash
+pip install wop
+```
+
+## Usage
+```bash
+wop --help
+```
+
+```bash
+wop <COMMAND> --help
+```
+
+## License
+
+   Copyright 2020 Rémi Lafage
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `wop-2.5.2/README.md` & `wop-2.5.3/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-[![Tests](https://github.com/OneraHub/WhatsOpt-CLI/workflows/Tests/badge.svg)](https://github.com/OneraHub/WhatsOpt-CLI/actions?query=workflow%3ATests)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/78559b54a0db44e5aeb5b0a3f5dcf9e2)](https://www.codacy.com/gh/OneraHub/WhatsOpt-CLI/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=OneraHub/WhatsOpt-CLI&amp;utm_campaign=Badge_Grade)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
-
-# WhatsOpt command line interface
-
-Command line interface to interact with WhatsOpt web application. See [WhatsOpt documentation](https://github.com/OneraHub/WhatsOpt-Doc).
-
-## Citation
->Rémi  Lafage,  Sébastien  Defoort,  and  Thierry  Lefèbvre. Whatsopt: a web application for multidisciplinary design analysis and optimization. In 20th AIAA/ISSMO Multidisciplinary Analysis and Optimization Conference, Dallas, United States, 2019
-
-DOI: [10.2514/6.2019-2990](https://doi.org/10.2514/6.2019-2990)
-
-## Installation
-```bash
-pip install wop
-```
-
-## Usage
-```bash
-wop --help
-```
-
-```bash
-wop <COMMAND> --help
-```
-
-## License
-
-   Copyright 2020 Rémi Lafage
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+[![Tests](https://github.com/OneraHub/WhatsOpt-CLI/workflows/Tests/badge.svg)](https://github.com/OneraHub/WhatsOpt-CLI/actions?query=workflow%3ATests)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/78559b54a0db44e5aeb5b0a3f5dcf9e2)](https://www.codacy.com/gh/OneraHub/WhatsOpt-CLI/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=OneraHub/WhatsOpt-CLI&amp;utm_campaign=Badge_Grade)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+
+# WhatsOpt command line interface
+
+Command line interface to interact with WhatsOpt web application. See [WhatsOpt documentation](https://github.com/OneraHub/WhatsOpt-Doc).
+
+## Citation
+>Rémi  Lafage,  Sébastien  Defoort,  and  Thierry  Lefèbvre. Whatsopt: a web application for multidisciplinary design analysis and optimization. In 20th AIAA/ISSMO Multidisciplinary Analysis and Optimization Conference, Dallas, United States, 2019
+
+DOI: [10.2514/6.2019-2990](https://doi.org/10.2514/6.2019-2990)
+
+## Installation
+```bash
+pip install wop
+```
+
+## Usage
+```bash
+wop --help
+```
+
+```bash
+wop <COMMAND> --help
+```
+
+## License
+
+   Copyright 2020 Rémi Lafage
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `wop-2.5.2/pyproject.toml` & `wop-2.5.3/pyproject.toml`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-[build-system]
-requires = ["setuptools", "setuptools-scm"]
-build-backend = "setuptools.build_meta"
-
-[tools.setuptools-scm]
-
-[tool.setuptools]
-packages = ["whatsopt"]
-
-[project]
-name = "wop"
-dynamic = ["version"]
-authors = [
-    {name = "Rémi Lafage", email = "remi.lafage@onera.fr"},
-]
-description = "My package description"
-readme = "README.md"
-requires-python = ">=3.7"
-keywords = ["WhatsOpt", "command"]
-license = {text = "Apache License 2.0"}
-classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Science/Research",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3",
-    "Topic :: Software Development",
-    "Topic :: Scientific/Engineering",
-    "Operating System :: Microsoft :: Windows",
-    "Operating System :: Unix",
-    "Operating System :: MacOS",
-]
-dependencies = [
-    "build",
-    "click>=6.7",
-    "openmdao>=3.4.0",
-    "openmdao_extensions>=1.2.0",
-    "packaging",
-    "pkginfo",
-    "requests",
-    "tabulate>=0.8.2",
-    "tomli",
-    "tomli-w",
-    "xdsmjs>=1.0.0",
-]
-
-[tool.setuptools.dynamic]
-version = {attr = "whatsopt.__version__"}
-
-[project.optional-dependencies]
-test = ["pytest"]
-
-[project.urls]
-homepage = "https://github.com/whatsopt"
-repository = "https://github.com/whatsopt/WhatsOpt-CLI"
-documentation = "https://github.com/whatsopt/WhatsOpt-Doc#whatsopt-documentation"
-
-[project.scripts]
-wop = "whatsopt.wop:wop"
-
+[build-system]
+requires = ["setuptools", "setuptools-scm"]
+build-backend = "setuptools.build_meta"
+
+[tools.setuptools-scm]
+
+[tool.setuptools]
+packages = ["whatsopt"]
+
+[project]
+name = "wop"
+dynamic = ["version"]
+authors = [
+    {name = "Rémi Lafage", email = "remi.lafage@onera.fr"},
+]
+description = "My package description"
+readme = "README.md"
+requires-python = ">=3.7"
+keywords = ["WhatsOpt", "command"]
+license = {text = "Apache License 2.0"}
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Science/Research",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: Apache Software License",
+    "Programming Language :: Python :: 3",
+    "Topic :: Software Development",
+    "Topic :: Scientific/Engineering",
+    "Operating System :: Microsoft :: Windows",
+    "Operating System :: Unix",
+    "Operating System :: MacOS",
+]
+dependencies = [
+    "build",
+    "click>=6.7",
+    "openmdao>=3.4.0",
+    "openmdao_extensions>=1.2.0",
+    "packaging",
+    "pkginfo",
+    "requests",
+    "tabulate>=0.8.2",
+    "tomli",
+    "tomli-w",
+    "xdsmjs>=1.0.0",
+]
+
+[tool.setuptools.dynamic]
+version = {attr = "whatsopt.__version__"}
+
+[project.optional-dependencies]
+test = ["pytest"]
+
+[project.urls]
+homepage = "https://github.com/whatsopt"
+repository = "https://github.com/whatsopt/WhatsOpt-CLI"
+documentation = "https://github.com/whatsopt/WhatsOpt-Doc#whatsopt-documentation"
+
+[project.scripts]
+wop = "whatsopt.wop:wop"
+
```

### Comparing `wop-2.5.2/tests/data/disc1_base.py` & `wop-2.5.3/tests/data/disc1_base.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# -*- coding: utf-8 -*-
-"""
-  disc1_base.py generated by WhatsOpt 1.7.0
-"""
-# DO NOT EDIT unless you know what you are doing
-# whatsopt_url: http://192.168.99.100:3000
-# analysis_id: 34
-
-
-# import numpy as np
-from os import path
-from importlib import import_module
-from openmdao.api import ExplicitComponent
-
-
-class Disc1Base(ExplicitComponent):
-    """An OpenMDAO base component to encapsulate Disc1 discipline"""
-
-    def setup(self):
-        self.add_input("x", val=2, desc="")
-        self.add_input("y2", val=1.0, desc="")
-        self.add_input("z", val=[5, 2], desc="")
-
-        self.add_output("y1", val=1.0, desc="")
+# -*- coding: utf-8 -*-
+"""
+  disc1_base.py generated by WhatsOpt 1.7.0
+"""
+# DO NOT EDIT unless you know what you are doing
+# whatsopt_url: http://192.168.99.100:3000
+# analysis_id: 34
+
+
+# import numpy as np
+from os import path
+from importlib import import_module
+from openmdao.api import ExplicitComponent
+
+
+class Disc1Base(ExplicitComponent):
+    """An OpenMDAO base component to encapsulate Disc1 discipline"""
+
+    def setup(self):
+        self.add_input("x", val=2, desc="")
+        self.add_input("y2", val=1.0, desc="")
+        self.add_input("z", val=[5, 2], desc="")
+
+        self.add_output("y1", val=1.0, desc="")
```

### Comparing `wop-2.5.2/tests/data/fonctions_base.py` & `wop-2.5.3/tests/data/fonctions_base.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# -*- coding: utf-8 -*-
-"""
-  fonctions_base.py generated by WhatsOpt 1.4.0
-"""
-# DO NOT EDIT unless you know what you are doing
-# whatsopt_url: https://selene.onecert.fr/whatsopt
-# analysis_id: 213
-
-import numpy as np
-from openmdao.api import ExplicitComponent
-
-
-class FonctionsBase(ExplicitComponent):
-    """An OpenMDAO base component to encapsulate Fonctions discipline"""
-
-    def setup(self):
-        self.add_input("x", val=2, desc="")
-        self.add_input("y1", val=1.0, desc="")
-        self.add_input("y2", val=1.0, desc="")
-        self.add_input("z", val=[5, 2], desc="")
-
-        self.add_output("f", val=1.0, desc="")
-
-        self.add_output("g1", val=1.0, desc="")
-
-        self.add_output("g2", val=1.0, desc="")
+# -*- coding: utf-8 -*-
+"""
+  fonctions_base.py generated by WhatsOpt 1.4.0
+"""
+# DO NOT EDIT unless you know what you are doing
+# whatsopt_url: https://selene.onecert.fr/whatsopt
+# analysis_id: 213
+
+import numpy as np
+from openmdao.api import ExplicitComponent
+
+
+class FonctionsBase(ExplicitComponent):
+    """An OpenMDAO base component to encapsulate Fonctions discipline"""
+
+    def setup(self):
+        self.add_input("x", val=2, desc="")
+        self.add_input("y1", val=1.0, desc="")
+        self.add_input("y2", val=1.0, desc="")
+        self.add_input("z", val=[5, 2], desc="")
+
+        self.add_output("f", val=1.0, desc="")
+
+        self.add_output("g1", val=1.0, desc="")
+
+        self.add_output("g2", val=1.0, desc="")
```

### Comparing `wop-2.5.2/tests/data/multipoint_beam/i_comp.py` & `wop-2.5.3/tests/data/multipoint_beam/i_comp.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# -*- coding: utf-8 -*-
-"""
-  i_comp.py generated by WhatsOpt 1.8.2
-"""
-import numpy as np
-from i_comp_base import ICompBase
-
-
-class IComp(ICompBase):
-    """An OpenMDAO component to encapsulate IComp discipline"""
-
-    def compute(self, inputs, outputs):
-        """IComp computation"""
-        if self._impl:
-            # Docking mechanism: use implementation if referenced in .whatsopt_dock.yml file
-            self._impl.compute(inputs, outputs)
-        else:
-            outputs["I"] = np.ones((50,))
-
-
-# Reminder: inputs of compute()
-#
-#       inputs['h'] -> shape: (50,), type: Float
-
-# To declare partial derivatives computation ...
-#
-#    def setup(self):
-#        super(IComp, self).setup()
-#        self.declare_partials('*', '*')
-#
-#    def compute_partials(self, inputs, partials):
-#        """ Jacobian for IComp """
-#
-#       	partials['I', 'h'] = np.zeros((50, 50))
+# -*- coding: utf-8 -*-
+"""
+  i_comp.py generated by WhatsOpt 1.8.2
+"""
+import numpy as np
+from i_comp_base import ICompBase
+
+
+class IComp(ICompBase):
+    """An OpenMDAO component to encapsulate IComp discipline"""
+
+    def compute(self, inputs, outputs):
+        """IComp computation"""
+        if self._impl:
+            # Docking mechanism: use implementation if referenced in .whatsopt_dock.yml file
+            self._impl.compute(inputs, outputs)
+        else:
+            outputs["I"] = np.ones((50,))
+
+
+# Reminder: inputs of compute()
+#
+#       inputs['h'] -> shape: (50,), type: Float
+
+# To declare partial derivatives computation ...
+#
+#    def setup(self):
+#        super(IComp, self).setup()
+#        self.declare_partials('*', '*')
+#
+#    def compute_partials(self, inputs, partials):
+#        """ Jacobian for IComp """
+#
+#       	partials['I', 'h'] = np.zeros((50, 50))
```

### Comparing `wop-2.5.2/tests/data/multipoint_beam/i_comp_base.py` & `wop-2.5.3/tests/data/multipoint_beam/i_comp_base.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# -*- coding: utf-8 -*-
-"""
-  i_comp_base.py generated by WhatsOpt 1.8.2
-"""
-# DO NOT EDIT unless you know what you are doing
-# whatsopt_url: https://ether.onera.fr/whatsopt
-# analysis_id: 4
-
-
-import numpy as np
-from numpy import nan
-from os import path
-from importlib import import_module
-from openmdao.api import ExplicitComponent
-
-
-class ICompBase(ExplicitComponent):
-    """An OpenMDAO base component to encapsulate IComp discipline"""
-
-    def setup(self):
-        self.add_input("h", val=np.ones((1, 50)), desc="")
-
-        self.add_output("I", val=np.ones((50,)), desc="")
+# -*- coding: utf-8 -*-
+"""
+  i_comp_base.py generated by WhatsOpt 1.8.2
+"""
+# DO NOT EDIT unless you know what you are doing
+# whatsopt_url: https://ether.onera.fr/whatsopt
+# analysis_id: 4
+
+
+import numpy as np
+from numpy import nan
+from os import path
+from importlib import import_module
+from openmdao.api import ExplicitComponent
+
+
+class ICompBase(ExplicitComponent):
+    """An OpenMDAO base component to encapsulate IComp discipline"""
+
+    def setup(self):
+        self.add_input("h", val=np.ones((1, 50)), desc="")
+
+        self.add_output("I", val=np.ones((50,)), desc="")
```

### Comparing `wop-2.5.2/tests/data/multipoint_beam/interp.py` & `wop-2.5.3/tests/data/multipoint_beam/interp.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# -*- coding: utf-8 -*-
-"""
-  interp.py generated by WhatsOpt 1.8.2
-"""
-import numpy as np
-from interp_base import InterpBase
-
-
-class Interp(InterpBase):
-    """An OpenMDAO component to encapsulate Interp discipline"""
-
-    def compute(self, inputs, outputs):
-        """Interp computation"""
-        if self._impl:
-            # Docking mechanism: use implementation if referenced in .whatsopt_dock.yml file
-            self._impl.compute(inputs, outputs)
-        else:
-            outputs["h"] = np.ones((1, 50))
-
-
-# Reminder: inputs of compute()
-#
-#       inputs['h_cp'] -> shape: (1, 5), type: Float
-
-# To declare partial derivatives computation ...
-#
-#    def setup(self):
-#        super(Interp, self).setup()
-#        self.declare_partials('*', '*')
-#
-#    def compute_partials(self, inputs, partials):
-#        """ Jacobian for Interp """
-#
-#       	partials['h', 'h_cp'] = np.zeros((50, 5))
+# -*- coding: utf-8 -*-
+"""
+  interp.py generated by WhatsOpt 1.8.2
+"""
+import numpy as np
+from interp_base import InterpBase
+
+
+class Interp(InterpBase):
+    """An OpenMDAO component to encapsulate Interp discipline"""
+
+    def compute(self, inputs, outputs):
+        """Interp computation"""
+        if self._impl:
+            # Docking mechanism: use implementation if referenced in .whatsopt_dock.yml file
+            self._impl.compute(inputs, outputs)
+        else:
+            outputs["h"] = np.ones((1, 50))
+
+
+# Reminder: inputs of compute()
+#
+#       inputs['h_cp'] -> shape: (1, 5), type: Float
+
+# To declare partial derivatives computation ...
+#
+#    def setup(self):
+#        super(Interp, self).setup()
+#        self.declare_partials('*', '*')
+#
+#    def compute_partials(self, inputs, partials):
+#        """ Jacobian for Interp """
+#
+#       	partials['h', 'h_cp'] = np.zeros((50, 5))
```

### Comparing `wop-2.5.2/tests/data/multipoint_beam/interp_base.py` & `wop-2.5.3/tests/data/multipoint_beam/parallel/sub0/compliance_comp_base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-# -*- coding: utf-8 -*-
-"""
-  interp_base.py generated by WhatsOpt 1.8.2
-"""
-# DO NOT EDIT unless you know what you are doing
-# whatsopt_url: https://ether.onera.fr/whatsopt
-# analysis_id: 4
-
-
-import numpy as np
-from numpy import nan
-from os import path
-from importlib import import_module
-from openmdao.api import ExplicitComponent
-
-
-class InterpBase(ExplicitComponent):
-    """An OpenMDAO base component to encapsulate Interp discipline"""
-
-    def setup(self):
-        self.add_input("h_cp", val=[1.0, 1.0, 1.0, 1.0, 1.0], desc="")
-
-        self.add_output("h", val=np.ones((1, 50)), desc="")
+# -*- coding: utf-8 -*-
+"""
+  compliance_comp_base.py generated by WhatsOpt 1.8.2
+"""
+# DO NOT EDIT unless you know what you are doing
+# whatsopt_url:
+# analysis_id: 6
+
+
+import numpy as np
+from numpy import nan
+from os import path
+from importlib import import_module
+from openmdao.api import ExplicitComponent
+
+
+class ComplianceCompBase(ExplicitComponent):
+    """An OpenMDAO base component to encapsulate ComplianceComp discipline"""
+
+    def setup(self):
+        self.add_input("displacements_0", val=np.ones((102,)), desc="")
+        self.add_input("displacements_1", val=np.ones((102,)), desc="")
+
+        self.add_output("compliance_0", val=np.ones((1,)), desc="")
+
+        self.add_output("compliance_1", val=np.ones((1,)), desc="")
```

### Comparing `wop-2.5.2/tests/data/multipoint_beam/local_stiffness_matrix_comp.py` & `wop-2.5.3/tests/data/multipoint_beam/local_stiffness_matrix_comp.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# -*- coding: utf-8 -*-
-"""
-  local_stiffness_matrix_comp.py generated by WhatsOpt 1.8.2
-"""
-import numpy as np
-from local_stiffness_matrix_comp_base import LocalStiffnessMatrixCompBase
-
-
-class LocalStiffnessMatrixComp(LocalStiffnessMatrixCompBase):
-    """An OpenMDAO component to encapsulate LocalStiffnessMatrixComp discipline"""
-
-    def compute(self, inputs, outputs):
-        """LocalStiffnessMatrixComp computation"""
-        if self._impl:
-            # Docking mechanism: use implementation if referenced in .whatsopt_dock.yml file
-            self._impl.compute(inputs, outputs)
-        else:
-            outputs["K_local"] = np.ones((50, 4, 4))
-
-
-# Reminder: inputs of compute()
-#
-#       inputs['I'] -> shape: (50,), type: Float
-
-# To declare partial derivatives computation ...
-#
-#    def setup(self):
-#        super(LocalStiffnessMatrixComp, self).setup()
-#        self.declare_partials('*', '*')
-#
-#    def compute_partials(self, inputs, partials):
-#        """ Jacobian for LocalStiffnessMatrixComp """
-#
-#       	partials['K_local', 'I'] = np.zeros((800, 50))
+# -*- coding: utf-8 -*-
+"""
+  local_stiffness_matrix_comp.py generated by WhatsOpt 1.8.2
+"""
+import numpy as np
+from local_stiffness_matrix_comp_base import LocalStiffnessMatrixCompBase
+
+
+class LocalStiffnessMatrixComp(LocalStiffnessMatrixCompBase):
+    """An OpenMDAO component to encapsulate LocalStiffnessMatrixComp discipline"""
+
+    def compute(self, inputs, outputs):
+        """LocalStiffnessMatrixComp computation"""
+        if self._impl:
+            # Docking mechanism: use implementation if referenced in .whatsopt_dock.yml file
+            self._impl.compute(inputs, outputs)
+        else:
+            outputs["K_local"] = np.ones((50, 4, 4))
+
+
+# Reminder: inputs of compute()
+#
+#       inputs['I'] -> shape: (50,), type: Float
+
+# To declare partial derivatives computation ...
+#
+#    def setup(self):
+#        super(LocalStiffnessMatrixComp, self).setup()
+#        self.declare_partials('*', '*')
+#
+#    def compute_partials(self, inputs, partials):
+#        """ Jacobian for LocalStiffnessMatrixComp """
+#
+#       	partials['K_local', 'I'] = np.zeros((800, 50))
```

### Comparing `wop-2.5.2/tests/data/multipoint_beam/local_stiffness_matrix_comp_base.py` & `wop-2.5.3/tests/data/multipoint_beam/local_stiffness_matrix_comp_base.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# -*- coding: utf-8 -*-
-"""
-  local_stiffness_matrix_comp_base.py generated by WhatsOpt 1.8.2
-"""
-# DO NOT EDIT unless you know what you are doing
-# whatsopt_url: https://ether.onera.fr/whatsopt
-# analysis_id: 4
-
-
-import numpy as np
-from numpy import nan
-from os import path
-from importlib import import_module
-from openmdao.api import ExplicitComponent
-
-
-class LocalStiffnessMatrixCompBase(ExplicitComponent):
-    """An OpenMDAO base component to encapsulate LocalStiffnessMatrixComp discipline"""
-
-    def setup(self):
-        self.add_input("I", val=np.ones((50,)), desc="")
-
-        self.add_output("K_local", val=np.ones((50, 4, 4)), desc="")
+# -*- coding: utf-8 -*-
+"""
+  local_stiffness_matrix_comp_base.py generated by WhatsOpt 1.8.2
+"""
+# DO NOT EDIT unless you know what you are doing
+# whatsopt_url: https://ether.onera.fr/whatsopt
+# analysis_id: 4
+
+
+import numpy as np
+from numpy import nan
+from os import path
+from importlib import import_module
+from openmdao.api import ExplicitComponent
+
+
+class LocalStiffnessMatrixCompBase(ExplicitComponent):
+    """An OpenMDAO base component to encapsulate LocalStiffnessMatrixComp discipline"""
+
+    def setup(self):
+        self.add_input("I", val=np.ones((50,)), desc="")
+
+        self.add_output("K_local", val=np.ones((50, 4, 4)), desc="")
```

### Comparing `wop-2.5.2/tests/data/multipoint_beam/obj_sum.py` & `wop-2.5.3/tests/data/multipoint_beam/obj_sum.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# -*- coding: utf-8 -*-
-"""
-  obj_sum.py generated by WhatsOpt 1.8.2
-"""
-import numpy as np
-from obj_sum_base import ObjSumBase
-
-
-class ObjSum(ObjSumBase):
-    """An OpenMDAO component to encapsulate ObjSum discipline"""
-
-    def compute(self, inputs, outputs):
-        """ObjSum computation"""
-        if self._impl:
-            # Docking mechanism: use implementation if referenced in .whatsopt_dock.yml file
-            self._impl.compute(inputs, outputs)
-        else:
-            outputs["obj"] = np.ones((1,))
-
-
-# Reminder: inputs of compute()
-#
-#       inputs['compliance_0'] -> shape: (1,), type: Float
-#       inputs['compliance_1'] -> shape: (1,), type: Float
-
-# To declare partial derivatives computation ...
-#
-#    def setup(self):
-#        super(ObjSum, self).setup()
-#        self.declare_partials('*', '*')
-#
-#    def compute_partials(self, inputs, partials):
-#        """ Jacobian for ObjSum """
-#
-#       	partials['obj', 'compliance_0'] = np.zeros((1, 1))
-#       	partials['obj', 'compliance_1'] = np.zeros((1, 1))
+# -*- coding: utf-8 -*-
+"""
+  obj_sum.py generated by WhatsOpt 1.8.2
+"""
+import numpy as np
+from obj_sum_base import ObjSumBase
+
+
+class ObjSum(ObjSumBase):
+    """An OpenMDAO component to encapsulate ObjSum discipline"""
+
+    def compute(self, inputs, outputs):
+        """ObjSum computation"""
+        if self._impl:
+            # Docking mechanism: use implementation if referenced in .whatsopt_dock.yml file
+            self._impl.compute(inputs, outputs)
+        else:
+            outputs["obj"] = np.ones((1,))
+
+
+# Reminder: inputs of compute()
+#
+#       inputs['compliance_0'] -> shape: (1,), type: Float
+#       inputs['compliance_1'] -> shape: (1,), type: Float
+
+# To declare partial derivatives computation ...
+#
+#    def setup(self):
+#        super(ObjSum, self).setup()
+#        self.declare_partials('*', '*')
+#
+#    def compute_partials(self, inputs, partials):
+#        """ Jacobian for ObjSum """
+#
+#       	partials['obj', 'compliance_0'] = np.zeros((1, 1))
+#       	partials['obj', 'compliance_1'] = np.zeros((1, 1))
```

### Comparing `wop-2.5.2/tests/data/multipoint_beam/obj_sum_base.py` & `wop-2.5.3/tests/data/multipoint_beam/obj_sum_base.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# -*- coding: utf-8 -*-
-"""
-  obj_sum_base.py generated by WhatsOpt 1.8.2
-"""
-# DO NOT EDIT unless you know what you are doing
-# whatsopt_url: https://ether.onera.fr/whatsopt
-# analysis_id: 4
-
-
-import numpy as np
-from numpy import nan
-from os import path
-from importlib import import_module
-from openmdao.api import ExplicitComponent
-
-
-class ObjSumBase(ExplicitComponent):
-    """An OpenMDAO base component to encapsulate ObjSum discipline"""
-
-    def setup(self):
-        self.add_input("compliance_0", val=np.ones((1,)), desc="")
-        self.add_input("compliance_1", val=np.ones((1,)), desc="")
-
-        self.add_output("obj", val=np.ones((1,)), desc="")
+# -*- coding: utf-8 -*-
+"""
+  obj_sum_base.py generated by WhatsOpt 1.8.2
+"""
+# DO NOT EDIT unless you know what you are doing
+# whatsopt_url: https://ether.onera.fr/whatsopt
+# analysis_id: 4
+
+
+import numpy as np
+from numpy import nan
+from os import path
+from importlib import import_module
+from openmdao.api import ExplicitComponent
+
+
+class ObjSumBase(ExplicitComponent):
+    """An OpenMDAO base component to encapsulate ObjSum discipline"""
+
+    def setup(self):
+        self.add_input("compliance_0", val=np.ones((1,)), desc="")
+        self.add_input("compliance_1", val=np.ones((1,)), desc="")
+
+        self.add_output("obj", val=np.ones((1,)), desc="")
```

### Comparing `wop-2.5.2/tests/data/multipoint_beam/parallel/parallel.py` & `wop-2.5.3/tests/data/multipoint_beam/parallel/parallel.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-# -*- coding: utf-8 -*-
-"""
-  parallel.py generated by WhatsOpt 1.8.2
-"""
-from optparse import OptionParser
-from openmdao.api import Problem
-from openmdao.api import NonlinearBlockGS, ScipyKrylov
-
-# from openmdao_extensions.reckless_nonlinear_block_gs import RecklessNonlinearBlockGS
-from parallel.parallel_base import ParallelBase, ParallelFactoryBase
-
-
-class Parallel(ParallelBase):
-    """An OpenMDAO component to encapsulate Parallel analysis"""
-
-    def __init__(self, **kwargs):
-        super(Parallel, self).__init__(**kwargs)
-
-        # Example of manual solver adjusments (imports should be adjusted accordingly)
-        # self.nonlinear_solver = NewtonSolver()
-        # self.nonlinear_solver.options['maxiter'] = 20
-        # self.linear_solver = DirectSolver()
-
-    def setup(self):
-        super(Parallel, self).setup()
-
-
-class ParallelFactory(ParallelFactoryBase):
-    """A factory to create disciplines of Parallel analysis"""
-
-    pass
-
-
-if __name__ == "__main__":
-    parser = OptionParser()
-    parser.add_option(
-        "-n",
-        "--no-n2",
-        action="store_false",
-        dest="n2_view",
-        default=True,
-        help="display N2 openmdao viewer",
-    )
-    (options, args) = parser.parse_args()
-
-    problem = Problem()
-    problem.model = Parallel()
-
-    problem.setup()
-    problem.final_setup()
-
-    if options.n2_view:
-        from packaging import version
-
-        if version.parse(OPENMDAO_VERSION) < version.parse("2.10.0"):
-            from openmdao.api import view_model as n2
-        else:
-            from openmdao.visualization.n2_viewer.n2_viewer import n2
-
-            n2(problem)
+# -*- coding: utf-8 -*-
+"""
+  parallel.py generated by WhatsOpt 1.8.2
+"""
+from optparse import OptionParser
+from openmdao.api import Problem
+from openmdao.api import NonlinearBlockGS, ScipyKrylov
+
+# from openmdao_extensions.reckless_nonlinear_block_gs import RecklessNonlinearBlockGS
+from parallel.parallel_base import ParallelBase, ParallelFactoryBase
+
+
+class Parallel(ParallelBase):
+    """An OpenMDAO component to encapsulate Parallel analysis"""
+
+    def __init__(self, **kwargs):
+        super(Parallel, self).__init__(**kwargs)
+
+        # Example of manual solver adjusments (imports should be adjusted accordingly)
+        # self.nonlinear_solver = NewtonSolver()
+        # self.nonlinear_solver.options['maxiter'] = 20
+        # self.linear_solver = DirectSolver()
+
+    def setup(self):
+        super(Parallel, self).setup()
+
+
+class ParallelFactory(ParallelFactoryBase):
+    """A factory to create disciplines of Parallel analysis"""
+
+    pass
+
+
+if __name__ == "__main__":
+    parser = OptionParser()
+    parser.add_option(
+        "-n",
+        "--no-n2",
+        action="store_false",
+        dest="n2_view",
+        default=True,
+        help="display N2 openmdao viewer",
+    )
+    (options, args) = parser.parse_args()
+
+    problem = Problem()
+    problem.model = Parallel()
+
+    problem.setup()
+    problem.final_setup()
+
+    if options.n2_view:
+        from packaging import version
+
+        if version.parse(OPENMDAO_VERSION) < version.parse("2.10.0"):
+            from openmdao.api import view_model as n2
+        else:
+            from openmdao.visualization.n2_viewer.n2_viewer import n2
+
+            n2(problem)
```

### Comparing `wop-2.5.2/tests/data/multipoint_beam/parallel/parallel_base.py` & `wop-2.5.3/tests/data/multipoint_beam/parallel/parallel_base.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-# -*- coding: utf-8 -*-
-"""
-  parallel_base.py generated by WhatsOpt 1.8.2
-"""
-# DO NOT EDIT unless you know what you are doing
-# whatsopt_url:
-# analysis_id: 5
-
-
-import numpy as np
-from numpy import nan
-
-from openmdao.api import Problem, Group, ParallelGroup, IndepVarComp
-from openmdao.api import NonlinearBlockGS
-from openmdao.api import ScipyKrylov
-from openmdao import __version__ as OPENMDAO_VERSION
-
-from parallel.sub0.sub0 import Sub0
-from parallel.sub0.states_comp import StatesComp
-from parallel.sub0.displacements_comp import DisplacementsComp
-from parallel.sub0.compliance_comp import ComplianceComp
-
-
-class ParallelBase(Group):
-    """An OpenMDAO base component to encapsulate Parallel MDA"""
-
-    def __init__(self, thrift_client=None, **kwargs):
-        super(ParallelBase, self).__init__(**kwargs)
-
-        self.nonlinear_solver = NonlinearBlockGS()
-        self.nonlinear_solver.options["atol"] = 1.0e-10
-        self.nonlinear_solver.options["rtol"] = 1.0e-10
-        self.nonlinear_solver.options["err_on_non_converge"] = True
-        self.nonlinear_solver.options["reraise_child_analysiserror"] = False
-        self.nonlinear_solver.options["iprint"] = 1
-
-        self.linear_solver = ScipyKrylov()
-        self.linear_solver.options["atol"] = 1.0e-10
-        self.linear_solver.options["rtol"] = 1.0e-10
-        self.linear_solver.options["err_on_non_converge"] = True
-        self.linear_solver.options["iprint"] = 1
-
-    def setup(self):
-        self.add_subsystem(
-            "Sub0",
-            self.create_sub0(),
-            promotes=[
-                "compliance_0",
-                "compliance_1",
-                "displacements_0",
-                "displacements_1",
-                "d_0",
-                "d_1",
-                "K_local",
-            ],
-        )
-
-    def create_sub0(self):
-        return Sub0()
-
-
-# Used by Thrift server to serve disciplines
-class ParallelFactoryBase(object):
-    @staticmethod
-    def create_parallel_sub0_states_comp():
-        return StatesComp()
-
-    @staticmethod
-    def create_parallel_sub0_displacements_comp():
-        return DisplacementsComp()
-
-    @staticmethod
-    def create_parallel_sub0_compliance_comp():
-        return ComplianceComp()
+# -*- coding: utf-8 -*-
+"""
+  parallel_base.py generated by WhatsOpt 1.8.2
+"""
+# DO NOT EDIT unless you know what you are doing
+# whatsopt_url:
+# analysis_id: 5
+
+
+import numpy as np
+from numpy import nan
+
+from openmdao.api import Problem, Group, ParallelGroup, IndepVarComp
+from openmdao.api import NonlinearBlockGS
+from openmdao.api import ScipyKrylov
+from openmdao import __version__ as OPENMDAO_VERSION
+
+from parallel.sub0.sub0 import Sub0
+from parallel.sub0.states_comp import StatesComp
+from parallel.sub0.displacements_comp import DisplacementsComp
+from parallel.sub0.compliance_comp import ComplianceComp
+
+
+class ParallelBase(Group):
+    """An OpenMDAO base component to encapsulate Parallel MDA"""
+
+    def __init__(self, thrift_client=None, **kwargs):
+        super(ParallelBase, self).__init__(**kwargs)
+
+        self.nonlinear_solver = NonlinearBlockGS()
+        self.nonlinear_solver.options["atol"] = 1.0e-10
+        self.nonlinear_solver.options["rtol"] = 1.0e-10
+        self.nonlinear_solver.options["err_on_non_converge"] = True
+        self.nonlinear_solver.options["reraise_child_analysiserror"] = False
+        self.nonlinear_solver.options["iprint"] = 1
+
+        self.linear_solver = ScipyKrylov()
+        self.linear_solver.options["atol"] = 1.0e-10
+        self.linear_solver.options["rtol"] = 1.0e-10
+        self.linear_solver.options["err_on_non_converge"] = True
+        self.linear_solver.options["iprint"] = 1
+
+    def setup(self):
+        self.add_subsystem(
+            "Sub0",
+            self.create_sub0(),
+            promotes=[
+                "compliance_0",
+                "compliance_1",
+                "displacements_0",
+                "displacements_1",
+                "d_0",
+                "d_1",
+                "K_local",
+            ],
+        )
+
+    def create_sub0(self):
+        return Sub0()
+
+
+# Used by Thrift server to serve disciplines
+class ParallelFactoryBase(object):
+    @staticmethod
+    def create_parallel_sub0_states_comp():
+        return StatesComp()
+
+    @staticmethod
+    def create_parallel_sub0_displacements_comp():
+        return DisplacementsComp()
+
+    @staticmethod
+    def create_parallel_sub0_compliance_comp():
+        return ComplianceComp()
```

### Comparing `wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/compliance_comp.py` & `wop-2.5.3/tests/data/multipoint_beam/parallel/sub0/compliance_comp.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# -*- coding: utf-8 -*-
-"""
-  compliance_comp.py generated by WhatsOpt 1.8.2
-"""
-import numpy as np
-from parallel.sub0.compliance_comp_base import ComplianceCompBase
-
-
-class ComplianceComp(ComplianceCompBase):
-    """An OpenMDAO component to encapsulate ComplianceComp discipline"""
-
-    def compute(self, inputs, outputs):
-        """ComplianceComp computation"""
-        if self._impl:
-            # Docking mechanism: use implementation if referenced in .whatsopt_dock.yml file
-            self._impl.compute(inputs, outputs)
-        else:
-            outputs["compliance_0"] = np.ones((1,))
-            outputs["compliance_1"] = np.ones((1,))
-
-
-# Reminder: inputs of compute()
-#
-#       inputs['displacements_0'] -> shape: (102,), type: Float
-#       inputs['displacements_1'] -> shape: (102,), type: Float
-
-# To declare partial derivatives computation ...
-#
-#    def setup(self):
-#        super(ComplianceComp, self).setup()
-#        self.declare_partials('*', '*')
-#
-#    def compute_partials(self, inputs, partials):
-#        """ Jacobian for ComplianceComp """
-#
-#       	partials['compliance_0', 'displacements_0'] = np.zeros((1, 102))
-#       	partials['compliance_0', 'displacements_1'] = np.zeros((1, 102))
-#       	partials['compliance_1', 'displacements_0'] = np.zeros((1, 102))
-#       	partials['compliance_1', 'displacements_1'] = np.zeros((1, 102))
+# -*- coding: utf-8 -*-
+"""
+  compliance_comp.py generated by WhatsOpt 1.8.2
+"""
+import numpy as np
+from parallel.sub0.compliance_comp_base import ComplianceCompBase
+
+
+class ComplianceComp(ComplianceCompBase):
+    """An OpenMDAO component to encapsulate ComplianceComp discipline"""
+
+    def compute(self, inputs, outputs):
+        """ComplianceComp computation"""
+        if self._impl:
+            # Docking mechanism: use implementation if referenced in .whatsopt_dock.yml file
+            self._impl.compute(inputs, outputs)
+        else:
+            outputs["compliance_0"] = np.ones((1,))
+            outputs["compliance_1"] = np.ones((1,))
+
+
+# Reminder: inputs of compute()
+#
+#       inputs['displacements_0'] -> shape: (102,), type: Float
+#       inputs['displacements_1'] -> shape: (102,), type: Float
+
+# To declare partial derivatives computation ...
+#
+#    def setup(self):
+#        super(ComplianceComp, self).setup()
+#        self.declare_partials('*', '*')
+#
+#    def compute_partials(self, inputs, partials):
+#        """ Jacobian for ComplianceComp """
+#
+#       	partials['compliance_0', 'displacements_0'] = np.zeros((1, 102))
+#       	partials['compliance_0', 'displacements_1'] = np.zeros((1, 102))
+#       	partials['compliance_1', 'displacements_0'] = np.zeros((1, 102))
+#       	partials['compliance_1', 'displacements_1'] = np.zeros((1, 102))
```

### Comparing `wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/states_comp.py` & `wop-2.5.3/tests/data/multipoint_beam/parallel/sub0/states_comp.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# -*- coding: utf-8 -*-
-"""
-  states_comp.py generated by WhatsOpt 1.8.2
-"""
-import numpy as np
-from parallel.sub0.states_comp_base import StatesCompBase
-
-
-class StatesComp(StatesCompBase):
-    """An OpenMDAO component to encapsulate StatesComp discipline"""
-
-    def compute(self, inputs, outputs):
-        """StatesComp computation"""
-        if self._impl:
-            # Docking mechanism: use implementation if referenced in .whatsopt_dock.yml file
-            self._impl.compute(inputs, outputs)
-        else:
-            outputs["d_0"] = np.ones((104,))
-            outputs["d_1"] = np.ones((104,))
-
-
-# Reminder: inputs of compute()
-#
-#       inputs['K_local'] -> shape: (50, 4, 4), type: Float
-
-# To declare partial derivatives computation ...
-#
-#    def setup(self):
-#        super(StatesComp, self).setup()
-#        self.declare_partials('*', '*')
-#
-#    def compute_partials(self, inputs, partials):
-#        """ Jacobian for StatesComp """
-#
-#       	partials['d_0', 'K_local'] = np.zeros((104, 800))
-#       	partials['d_1', 'K_local'] = np.zeros((104, 800))
+# -*- coding: utf-8 -*-
+"""
+  states_comp.py generated by WhatsOpt 1.8.2
+"""
+import numpy as np
+from parallel.sub0.states_comp_base import StatesCompBase
+
+
+class StatesComp(StatesCompBase):
+    """An OpenMDAO component to encapsulate StatesComp discipline"""
+
+    def compute(self, inputs, outputs):
+        """StatesComp computation"""
+        if self._impl:
+            # Docking mechanism: use implementation if referenced in .whatsopt_dock.yml file
+            self._impl.compute(inputs, outputs)
+        else:
+            outputs["d_0"] = np.ones((104,))
+            outputs["d_1"] = np.ones((104,))
+
+
+# Reminder: inputs of compute()
+#
+#       inputs['K_local'] -> shape: (50, 4, 4), type: Float
+
+# To declare partial derivatives computation ...
+#
+#    def setup(self):
+#        super(StatesComp, self).setup()
+#        self.declare_partials('*', '*')
+#
+#    def compute_partials(self, inputs, partials):
+#        """ Jacobian for StatesComp """
+#
+#       	partials['d_0', 'K_local'] = np.zeros((104, 800))
+#       	partials['d_1', 'K_local'] = np.zeros((104, 800))
```

### Comparing `wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/states_comp_base.py` & `wop-2.5.3/tests/data/multipoint_beam/parallel/sub0/states_comp_base.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,330 +1,330 @@
-# -*- coding: utf-8 -*-
-"""
-  states_comp_base.py generated by WhatsOpt 1.8.2
-"""
-# DO NOT EDIT unless you know what you are doing
-# whatsopt_url:
-# analysis_id: 6
-
-
-import numpy as np
-from numpy import nan
-from os import path
-from importlib import import_module
-from openmdao.api import ExplicitComponent
-
-
-class StatesCompBase(ExplicitComponent):
-    """An OpenMDAO base component to encapsulate StatesComp discipline"""
-
-    def setup(self):
-        self.add_input(
-            "K_local",
-            val=[
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-                [
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                    [1.0, 1.0, 1.0, 1.0],
-                ],
-            ],
-            desc="",
-        )
-
-        self.add_output("d_0", val=np.ones((104,)), desc="")
-
-        self.add_output("d_1", val=np.ones((104,)), desc="")
+# -*- coding: utf-8 -*-
+"""
+  states_comp_base.py generated by WhatsOpt 1.8.2
+"""
+# DO NOT EDIT unless you know what you are doing
+# whatsopt_url:
+# analysis_id: 6
+
+
+import numpy as np
+from numpy import nan
+from os import path
+from importlib import import_module
+from openmdao.api import ExplicitComponent
+
+
+class StatesCompBase(ExplicitComponent):
+    """An OpenMDAO base component to encapsulate StatesComp discipline"""
+
+    def setup(self):
+        self.add_input(
+            "K_local",
+            val=[
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+                [
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                    [1.0, 1.0, 1.0, 1.0],
+                ],
+            ],
+            desc="",
+        )
+
+        self.add_output("d_0", val=np.ones((104,)), desc="")
+
+        self.add_output("d_1", val=np.ones((104,)), desc="")
```

### Comparing `wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/sub0.py` & `wop-2.5.3/tests/data/multipoint_beam/parallel/sub0/sub0.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-# -*- coding: utf-8 -*-
-"""
-  sub0.py generated by WhatsOpt 1.8.2
-"""
-from optparse import OptionParser
-from openmdao.api import Problem
-from openmdao.api import NonlinearBlockGS, ScipyKrylov
-
-# from openmdao_extensions.reckless_nonlinear_block_gs import RecklessNonlinearBlockGS
-from parallel.sub0.sub0_base import Sub0Base, Sub0FactoryBase
-
-
-class Sub0(Sub0Base):
-    """An OpenMDAO component to encapsulate Sub0 analysis"""
-
-    def __init__(self, **kwargs):
-        super(Sub0, self).__init__(**kwargs)
-
-        # Example of manual solver adjusments (imports should be adjusted accordingly)
-        # self.nonlinear_solver = NewtonSolver()
-        # self.nonlinear_solver.options['maxiter'] = 20
-        # self.linear_solver = DirectSolver()
-
-    def setup(self):
-        super(Sub0, self).setup()
-
-
-class Sub0Factory(Sub0FactoryBase):
-    """A factory to create disciplines of Sub0 analysis"""
-
-    pass
-
-
-if __name__ == "__main__":
-    parser = OptionParser()
-    parser.add_option(
-        "-n",
-        "--no-n2",
-        action="store_false",
-        dest="n2_view",
-        default=True,
-        help="display N2 openmdao viewer",
-    )
-    (options, args) = parser.parse_args()
-
-    problem = Problem()
-    problem.model = Sub0()
-
-    problem.setup()
-    problem.final_setup()
-
-    if options.n2_view:
-        from packaging import version
-
-        if version.parse(OPENMDAO_VERSION) < version.parse("2.10.0"):
-            from openmdao.api import view_model as n2
-        else:
-            from openmdao.visualization.n2_viewer.n2_viewer import n2
-
-            n2(problem)
+# -*- coding: utf-8 -*-
+"""
+  sub0.py generated by WhatsOpt 1.8.2
+"""
+from optparse import OptionParser
+from openmdao.api import Problem
+from openmdao.api import NonlinearBlockGS, ScipyKrylov
+
+# from openmdao_extensions.reckless_nonlinear_block_gs import RecklessNonlinearBlockGS
+from parallel.sub0.sub0_base import Sub0Base, Sub0FactoryBase
+
+
+class Sub0(Sub0Base):
+    """An OpenMDAO component to encapsulate Sub0 analysis"""
+
+    def __init__(self, **kwargs):
+        super(Sub0, self).__init__(**kwargs)
+
+        # Example of manual solver adjusments (imports should be adjusted accordingly)
+        # self.nonlinear_solver = NewtonSolver()
+        # self.nonlinear_solver.options['maxiter'] = 20
+        # self.linear_solver = DirectSolver()
+
+    def setup(self):
+        super(Sub0, self).setup()
+
+
+class Sub0Factory(Sub0FactoryBase):
+    """A factory to create disciplines of Sub0 analysis"""
+
+    pass
+
+
+if __name__ == "__main__":
+    parser = OptionParser()
+    parser.add_option(
+        "-n",
+        "--no-n2",
+        action="store_false",
+        dest="n2_view",
+        default=True,
+        help="display N2 openmdao viewer",
+    )
+    (options, args) = parser.parse_args()
+
+    problem = Problem()
+    problem.model = Sub0()
+
+    problem.setup()
+    problem.final_setup()
+
+    if options.n2_view:
+        from packaging import version
+
+        if version.parse(OPENMDAO_VERSION) < version.parse("2.10.0"):
+            from openmdao.api import view_model as n2
+        else:
+            from openmdao.visualization.n2_viewer.n2_viewer import n2
+
+            n2(problem)
```

### Comparing `wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/sub0_base.py` & `wop-2.5.3/tests/data/multipoint_beam/parallel/sub0/sub0_base.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-# -*- coding: utf-8 -*-
-"""
-  sub0_base.py generated by WhatsOpt 1.8.2
-"""
-# DO NOT EDIT unless you know what you are doing
-# whatsopt_url:
-# analysis_id: 6
-
-
-import numpy as np
-from numpy import nan
-
-from openmdao.api import Problem, Group, ParallelGroup, IndepVarComp
-from openmdao.api import NonlinearBlockGS
-from openmdao.api import ScipyKrylov
-from openmdao import __version__ as OPENMDAO_VERSION
-
-from parallel.sub0.states_comp import StatesComp
-from parallel.sub0.displacements_comp import DisplacementsComp
-from parallel.sub0.compliance_comp import ComplianceComp
-
-
-class Sub0Base(Group):
-    """An OpenMDAO base component to encapsulate Sub0 MDA"""
-
-    def __init__(self, thrift_client=None, **kwargs):
-        super(Sub0Base, self).__init__(**kwargs)
-
-        self.nonlinear_solver = NonlinearBlockGS()
-        self.nonlinear_solver.options["atol"] = 1.0e-10
-        self.nonlinear_solver.options["rtol"] = 1.0e-10
-        self.nonlinear_solver.options["err_on_non_converge"] = True
-        self.nonlinear_solver.options["reraise_child_analysiserror"] = False
-        self.nonlinear_solver.options["iprint"] = 1
-
-        self.linear_solver = ScipyKrylov()
-        self.linear_solver.options["atol"] = 1.0e-10
-        self.linear_solver.options["rtol"] = 1.0e-10
-        self.linear_solver.options["err_on_non_converge"] = True
-        self.linear_solver.options["iprint"] = 1
-
-    def setup(self):
-        self.add_subsystem(
-            "StatesComp", self.create_states_comp(), promotes=["d_0", "d_1", "K_local"]
-        )
-        self.add_subsystem(
-            "DisplacementsComp",
-            self.create_displacements_comp(),
-            promotes=["displacements_0", "displacements_1", "d_0", "d_1"],
-        )
-        self.add_subsystem(
-            "ComplianceComp",
-            self.create_compliance_comp(),
-            promotes=[
-                "compliance_0",
-                "compliance_1",
-                "displacements_0",
-                "displacements_1",
-            ],
-        )
-
-    def create_states_comp(self):
-        return StatesComp()
-
-    def create_displacements_comp(self):
-        return DisplacementsComp()
-
-    def create_compliance_comp(self):
-        return ComplianceComp()
-
-
-# Used by Thrift server to serve disciplines
-class Sub0FactoryBase(object):
-    @staticmethod
-    def create_parallel_sub0_states_comp():
-        return StatesComp()
-
-    @staticmethod
-    def create_parallel_sub0_displacements_comp():
-        return DisplacementsComp()
-
-    @staticmethod
-    def create_parallel_sub0_compliance_comp():
-        return ComplianceComp()
+# -*- coding: utf-8 -*-
+"""
+  sub0_base.py generated by WhatsOpt 1.8.2
+"""
+# DO NOT EDIT unless you know what you are doing
+# whatsopt_url:
+# analysis_id: 6
+
+
+import numpy as np
+from numpy import nan
+
+from openmdao.api import Problem, Group, ParallelGroup, IndepVarComp
+from openmdao.api import NonlinearBlockGS
+from openmdao.api import ScipyKrylov
+from openmdao import __version__ as OPENMDAO_VERSION
+
+from parallel.sub0.states_comp import StatesComp
+from parallel.sub0.displacements_comp import DisplacementsComp
+from parallel.sub0.compliance_comp import ComplianceComp
+
+
+class Sub0Base(Group):
+    """An OpenMDAO base component to encapsulate Sub0 MDA"""
+
+    def __init__(self, thrift_client=None, **kwargs):
+        super(Sub0Base, self).__init__(**kwargs)
+
+        self.nonlinear_solver = NonlinearBlockGS()
+        self.nonlinear_solver.options["atol"] = 1.0e-10
+        self.nonlinear_solver.options["rtol"] = 1.0e-10
+        self.nonlinear_solver.options["err_on_non_converge"] = True
+        self.nonlinear_solver.options["reraise_child_analysiserror"] = False
+        self.nonlinear_solver.options["iprint"] = 1
+
+        self.linear_solver = ScipyKrylov()
+        self.linear_solver.options["atol"] = 1.0e-10
+        self.linear_solver.options["rtol"] = 1.0e-10
+        self.linear_solver.options["err_on_non_converge"] = True
+        self.linear_solver.options["iprint"] = 1
+
+    def setup(self):
+        self.add_subsystem(
+            "StatesComp", self.create_states_comp(), promotes=["d_0", "d_1", "K_local"]
+        )
+        self.add_subsystem(
+            "DisplacementsComp",
+            self.create_displacements_comp(),
+            promotes=["displacements_0", "displacements_1", "d_0", "d_1"],
+        )
+        self.add_subsystem(
+            "ComplianceComp",
+            self.create_compliance_comp(),
+            promotes=[
+                "compliance_0",
+                "compliance_1",
+                "displacements_0",
+                "displacements_1",
+            ],
+        )
+
+    def create_states_comp(self):
+        return StatesComp()
+
+    def create_displacements_comp(self):
+        return DisplacementsComp()
+
+    def create_compliance_comp(self):
+        return ComplianceComp()
+
+
+# Used by Thrift server to serve disciplines
+class Sub0FactoryBase(object):
+    @staticmethod
+    def create_parallel_sub0_states_comp():
+        return StatesComp()
+
+    @staticmethod
+    def create_parallel_sub0_displacements_comp():
+        return DisplacementsComp()
+
+    @staticmethod
+    def create_parallel_sub0_compliance_comp():
+        return ComplianceComp()
```

### Comparing `wop-2.5.2/tests/data/multipoint_beam/volume_comp_base.py` & `wop-2.5.3/tests/data/multipoint_beam/volume_comp_base.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# -*- coding: utf-8 -*-
-"""
-  volume_comp_base.py generated by WhatsOpt 1.8.2
-"""
-# DO NOT EDIT unless you know what you are doing
-# whatsopt_url: https://ether.onera.fr/whatsopt
-# analysis_id: 4
-
-
-import numpy as np
-from numpy import nan
-from os import path
-from importlib import import_module
-from openmdao.api import ExplicitComponent
-
-
-class VolumeCompBase(ExplicitComponent):
-    """An OpenMDAO base component to encapsulate VolumeComp discipline"""
-
-    def setup(self):
-        self.add_input("h", val=np.ones((1, 50)), desc="")
-
-        self.add_output("volume", val=np.ones((1,)), desc="")
+# -*- coding: utf-8 -*-
+"""
+  volume_comp_base.py generated by WhatsOpt 1.8.2
+"""
+# DO NOT EDIT unless you know what you are doing
+# whatsopt_url: https://ether.onera.fr/whatsopt
+# analysis_id: 4
+
+
+import numpy as np
+from numpy import nan
+from os import path
+from importlib import import_module
+from openmdao.api import ExplicitComponent
+
+
+class VolumeCompBase(ExplicitComponent):
+    """An OpenMDAO base component to encapsulate VolumeComp discipline"""
+
+    def setup(self):
+        self.add_input("h", val=np.ones((1, 50)), desc="")
+
+        self.add_output("volume", val=np.ones((1,)), desc="")
```

### Comparing `wop-2.5.2/tests/data/multipoint_beam_group_d2.json` & `wop-2.5.3/tests/data/multipoint_beam_group_d2.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 23% similar despite different names*

```diff
@@ -1,1114 +1,1092 @@
-00000000: 7b0d 0a20 2022 6e61 6d65 223a 2022 4d75  {..  "name": "Mu
-00000010: 6c74 6970 6f69 6e74 4265 616d 4772 6f75  ltipointBeamGrou
-00000020: 7022 2c0d 0a20 2022 6469 7363 6970 6c69  p",..  "discipli
-00000030: 6e65 735f 6174 7472 6962 7574 6573 223a  nes_attributes":
-00000040: 205b 0d0a 2020 2020 7b0d 0a20 2020 2020   [..    {..     
-00000050: 2022 6e61 6d65 223a 2022 5f5f 4452 4956   "name": "__DRIV
-00000060: 4552 5f5f 222c 0d0a 2020 2020 2020 2276  ER__",..      "v
-00000070: 6172 6961 626c 6573 5f61 7474 7269 6275  ariables_attribu
-00000080: 7465 7322 3a20 5b0d 0a20 2020 2020 2020  tes": [..       
-00000090: 207b 0d0a 2020 2020 2020 2020 2020 226e   {..          "n
-000000a0: 616d 6522 3a20 2268 5f63 7022 2c0d 0a20  ame": "h_cp",.. 
-000000b0: 2020 2020 2020 2020 2022 696f 5f6d 6f64           "io_mod
-000000c0: 6522 3a20 226f 7574 222c 0d0a 2020 2020  e": "out",..    
-000000d0: 2020 2020 2020 2264 6573 6322 3a20 2222        "desc": ""
-000000e0: 2c0d 0a20 2020 2020 2020 2020 2022 7479  ,..          "ty
-000000f0: 7065 223a 2022 466c 6f61 7422 2c0d 0a20  pe": "Float",.. 
-00000100: 2020 2020 2020 2020 2022 7368 6170 6522           "shape"
-00000110: 3a20 2228 352c 2922 2c0d 0a20 2020 2020  : "(5,)",..     
-00000120: 2020 2020 2022 756e 6974 7322 3a20 6e75       "units": nu
-00000130: 6c6c 2c0d 0a20 2020 2020 2020 2020 2022  ll,..          "
-00000140: 7061 7261 6d65 7465 725f 6174 7472 6962  parameter_attrib
-00000150: 7574 6573 223a 207b 0d0a 2020 2020 2020  utes": {..      
-00000160: 2020 2020 2020 2269 6e69 7422 3a20 225b        "init": "[
-00000170: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00000180: 2e30 2c20 312e 305d 220d 0a20 2020 2020  .0, 1.0]"..     
-00000190: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-000001a0: 7d2c 0d0a 2020 2020 2020 2020 7b0d 0a20  },..        {.. 
-000001b0: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
-000001c0: 2022 6822 2c0d 0a20 2020 2020 2020 2020   "h",..         
-000001d0: 2022 696f 5f6d 6f64 6522 3a20 2269 6e22   "io_mode": "in"
-000001e0: 2c0d 0a20 2020 2020 2020 2020 2022 6465  ,..          "de
-000001f0: 7363 223a 2022 222c 0d0a 2020 2020 2020  sc": "",..      
-00000200: 2020 2020 2274 7970 6522 3a20 2246 6c6f      "type": "Flo
-00000210: 6174 222c 0d0a 2020 2020 2020 2020 2020  at",..          
-00000220: 2273 6861 7065 223a 2022 2831 2c20 3530  "shape": "(1, 50
-00000230: 2922 2c0d 0a20 2020 2020 2020 2020 2022  )",..          "
-00000240: 756e 6974 7322 3a20 6e75 6c6c 0d0a 2020  units": null..  
-00000250: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
-00000260: 2020 7b0d 0a20 2020 2020 2020 2020 2022    {..          "
-00000270: 6e61 6d65 223a 2022 4922 2c0d 0a20 2020  name": "I",..   
-00000280: 2020 2020 2020 2022 696f 5f6d 6f64 6522         "io_mode"
-00000290: 3a20 2269 6e22 2c0d 0a20 2020 2020 2020  : "in",..       
-000002a0: 2020 2022 6465 7363 223a 2022 222c 0d0a     "desc": "",..
-000002b0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-000002c0: 3a20 2246 6c6f 6174 222c 0d0a 2020 2020  : "Float",..    
-000002d0: 2020 2020 2020 2273 6861 7065 223a 2022        "shape": "
-000002e0: 2835 302c 2922 2c0d 0a20 2020 2020 2020  (50,)",..       
-000002f0: 2020 2022 756e 6974 7322 3a20 6e75 6c6c     "units": null
-00000300: 0d0a 2020 2020 2020 2020 7d2c 0d0a 2020  ..        },..  
-00000310: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-00000320: 2020 2022 6e61 6d65 223a 2022 4b5f 6c6f     "name": "K_lo
-00000330: 6361 6c22 2c0d 0a20 2020 2020 2020 2020  cal",..         
-00000340: 2022 696f 5f6d 6f64 6522 3a20 2269 6e22   "io_mode": "in"
-00000350: 2c0d 0a20 2020 2020 2020 2020 2022 6465  ,..          "de
-00000360: 7363 223a 2022 222c 0d0a 2020 2020 2020  sc": "",..      
-00000370: 2020 2020 2274 7970 6522 3a20 2246 6c6f      "type": "Flo
-00000380: 6174 222c 0d0a 2020 2020 2020 2020 2020  at",..          
-00000390: 2273 6861 7065 223a 2022 2835 302c 2034  "shape": "(50, 4
-000003a0: 2c20 3429 222c 0d0a 2020 2020 2020 2020  , 4)",..        
-000003b0: 2020 2275 6e69 7473 223a 206e 756c 6c0d    "units": null.
-000003c0: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-000003d0: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-000003e0: 2020 226e 616d 6522 3a20 2264 5f30 222c    "name": "d_0",
-000003f0: 0d0a 2020 2020 2020 2020 2020 2269 6f5f  ..          "io_
-00000400: 6d6f 6465 223a 2022 696e 222c 0d0a 2020  mode": "in",..  
-00000410: 2020 2020 2020 2020 2264 6573 6322 3a20          "desc": 
-00000420: 2222 2c0d 0a20 2020 2020 2020 2020 2022  "",..          "
-00000430: 7479 7065 223a 2022 466c 6f61 7422 2c0d  type": "Float",.
-00000440: 0a20 2020 2020 2020 2020 2022 7368 6170  .          "shap
-00000450: 6522 3a20 2228 3130 342c 2922 2c0d 0a20  e": "(104,)",.. 
-00000460: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
-00000470: 3a20 6e75 6c6c 0d0a 2020 2020 2020 2020  : null..        
-00000480: 7d2c 0d0a 2020 2020 2020 2020 7b0d 0a20  },..        {.. 
-00000490: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
-000004a0: 2022 645f 3122 2c0d 0a20 2020 2020 2020   "d_1",..       
-000004b0: 2020 2022 696f 5f6d 6f64 6522 3a20 2269     "io_mode": "i
-000004c0: 6e22 2c0d 0a20 2020 2020 2020 2020 2022  n",..          "
-000004d0: 6465 7363 223a 2022 222c 0d0a 2020 2020  desc": "",..    
-000004e0: 2020 2020 2020 2274 7970 6522 3a20 2246        "type": "F
-000004f0: 6c6f 6174 222c 0d0a 2020 2020 2020 2020  loat",..        
-00000500: 2020 2273 6861 7065 223a 2022 2831 3034    "shape": "(104
-00000510: 2c29 222c 0d0a 2020 2020 2020 2020 2020  ,)",..          
-00000520: 2275 6e69 7473 223a 206e 756c 6c0d 0a20  "units": null.. 
-00000530: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00000540: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-00000550: 226e 616d 6522 3a20 2264 6973 706c 6163  "name": "displac
-00000560: 656d 656e 7473 5f30 222c 0d0a 2020 2020  ements_0",..    
-00000570: 2020 2020 2020 2269 6f5f 6d6f 6465 223a        "io_mode":
-00000580: 2022 696e 222c 0d0a 2020 2020 2020 2020   "in",..        
-00000590: 2020 2264 6573 6322 3a20 2222 2c0d 0a20    "desc": "",.. 
-000005a0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-000005b0: 2022 466c 6f61 7422 2c0d 0a20 2020 2020   "Float",..     
-000005c0: 2020 2020 2022 7368 6170 6522 3a20 2228       "shape": "(
-000005d0: 3130 322c 2922 2c0d 0a20 2020 2020 2020  102,)",..       
-000005e0: 2020 2022 756e 6974 7322 3a20 6e75 6c6c     "units": null
-000005f0: 0d0a 2020 2020 2020 2020 7d2c 0d0a 2020  ..        },..  
-00000600: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-00000610: 2020 2022 6e61 6d65 223a 2022 6469 7370     "name": "disp
-00000620: 6c61 6365 6d65 6e74 735f 3122 2c0d 0a20  lacements_1",.. 
-00000630: 2020 2020 2020 2020 2022 696f 5f6d 6f64           "io_mod
-00000640: 6522 3a20 2269 6e22 2c0d 0a20 2020 2020  e": "in",..     
-00000650: 2020 2020 2022 6465 7363 223a 2022 222c       "desc": "",
-00000660: 0d0a 2020 2020 2020 2020 2020 2274 7970  ..          "typ
-00000670: 6522 3a20 2246 6c6f 6174 222c 0d0a 2020  e": "Float",..  
-00000680: 2020 2020 2020 2020 2273 6861 7065 223a          "shape":
-00000690: 2022 2831 3032 2c29 222c 0d0a 2020 2020   "(102,)",..    
-000006a0: 2020 2020 2020 2275 6e69 7473 223a 206e        "units": n
-000006b0: 756c 6c0d 0a20 2020 2020 2020 207d 2c0d  ull..        },.
-000006c0: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
-000006d0: 2020 2020 2020 226e 616d 6522 3a20 2263        "name": "c
-000006e0: 6f6d 706c 6961 6e63 655f 3022 2c0d 0a20  ompliance_0",.. 
-000006f0: 2020 2020 2020 2020 2022 696f 5f6d 6f64           "io_mod
-00000700: 6522 3a20 2269 6e22 2c0d 0a20 2020 2020  e": "in",..     
-00000710: 2020 2020 2022 6465 7363 223a 2022 222c       "desc": "",
-00000720: 0d0a 2020 2020 2020 2020 2020 2274 7970  ..          "typ
-00000730: 6522 3a20 2246 6c6f 6174 222c 0d0a 2020  e": "Float",..  
-00000740: 2020 2020 2020 2020 2273 6861 7065 223a          "shape":
-00000750: 2022 3122 2c0d 0a20 2020 2020 2020 2020   "1",..         
-00000760: 2022 756e 6974 7322 3a20 6e75 6c6c 0d0a   "units": null..
-00000770: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-00000780: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
-00000790: 2022 6e61 6d65 223a 2022 636f 6d70 6c69   "name": "compli
-000007a0: 616e 6365 5f31 222c 0d0a 2020 2020 2020  ance_1",..      
-000007b0: 2020 2020 2269 6f5f 6d6f 6465 223a 2022      "io_mode": "
-000007c0: 696e 222c 0d0a 2020 2020 2020 2020 2020  in",..          
-000007d0: 2264 6573 6322 3a20 2222 2c0d 0a20 2020  "desc": "",..   
-000007e0: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-000007f0: 466c 6f61 7422 2c0d 0a20 2020 2020 2020  Float",..       
-00000800: 2020 2022 7368 6170 6522 3a20 2231 222c     "shape": "1",
-00000810: 0d0a 2020 2020 2020 2020 2020 2275 6e69  ..          "uni
-00000820: 7473 223a 206e 756c 6c0d 0a20 2020 2020  ts": null..     
-00000830: 2020 207d 2c0d 0a20 2020 2020 2020 207b     },..        {
-00000840: 0d0a 2020 2020 2020 2020 2020 226e 616d  ..          "nam
-00000850: 6522 3a20 2276 6f6c 756d 6522 2c0d 0a20  e": "volume",.. 
-00000860: 2020 2020 2020 2020 2022 696f 5f6d 6f64           "io_mod
-00000870: 6522 3a20 2269 6e22 2c0d 0a20 2020 2020  e": "in",..     
-00000880: 2020 2020 2022 6465 7363 223a 2022 222c       "desc": "",
-00000890: 0d0a 2020 2020 2020 2020 2020 2274 7970  ..          "typ
-000008a0: 6522 3a20 2246 6c6f 6174 222c 0d0a 2020  e": "Float",..  
-000008b0: 2020 2020 2020 2020 2273 6861 7065 223a          "shape":
-000008c0: 2022 3122 2c0d 0a20 2020 2020 2020 2020   "1",..         
-000008d0: 2022 756e 6974 7322 3a20 6e75 6c6c 0d0a   "units": null..
-000008e0: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-000008f0: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
-00000900: 2022 6e61 6d65 223a 2022 6f62 6a22 2c0d   "name": "obj",.
-00000910: 0a20 2020 2020 2020 2020 2022 696f 5f6d  .          "io_m
-00000920: 6f64 6522 3a20 2269 6e22 2c0d 0a20 2020  ode": "in",..   
-00000930: 2020 2020 2020 2022 6465 7363 223a 2022         "desc": "
-00000940: 222c 0d0a 2020 2020 2020 2020 2020 2274  ",..          "t
-00000950: 7970 6522 3a20 2246 6c6f 6174 222c 0d0a  ype": "Float",..
-00000960: 2020 2020 2020 2020 2020 2273 6861 7065            "shape
-00000970: 223a 2022 3122 2c0d 0a20 2020 2020 2020  ": "1",..       
-00000980: 2020 2022 756e 6974 7322 3a20 6e75 6c6c     "units": null
-00000990: 0d0a 2020 2020 2020 2020 7d0d 0a20 2020  ..        }..   
-000009a0: 2020 205d 0d0a 2020 2020 7d2c 0d0a 2020     ]..    },..  
-000009b0: 2020 7b0d 0a20 2020 2020 2022 6e61 6d65    {..      "name
-000009c0: 223a 2022 496e 7465 7270 222c 0d0a 2020  ": "Interp",..  
-000009d0: 2020 2020 2276 6172 6961 626c 6573 5f61      "variables_a
-000009e0: 7474 7269 6275 7465 7322 3a20 5b0d 0a20  ttributes": [.. 
-000009f0: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-00000a00: 2020 2020 226e 616d 6522 3a20 2268 222c      "name": "h",
-00000a10: 0d0a 2020 2020 2020 2020 2020 2269 6f5f  ..          "io_
-00000a20: 6d6f 6465 223a 2022 6f75 7422 2c0d 0a20  mode": "out",.. 
-00000a30: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00000a40: 2022 466c 6f61 7422 2c0d 0a20 2020 2020   "Float",..     
-00000a50: 2020 2020 2022 7368 6170 6522 3a20 2228       "shape": "(
-00000a60: 312c 2035 3029 222c 0d0a 2020 2020 2020  1, 50)",..      
-00000a70: 2020 2020 2275 6e69 7473 223a 206e 756c      "units": nul
-00000a80: 6c2c 0d0a 2020 2020 2020 2020 2020 2264  l,..          "d
-00000a90: 6573 6322 3a20 2222 0d0a 2020 2020 2020  esc": ""..      
-00000aa0: 2020 7d2c 0d0a 2020 2020 2020 2020 7b0d    },..        {.
-00000ab0: 0a20 2020 2020 2020 2020 2022 6e61 6d65  .          "name
-00000ac0: 223a 2022 685f 6370 222c 0d0a 2020 2020  ": "h_cp",..    
-00000ad0: 2020 2020 2020 2269 6f5f 6d6f 6465 223a        "io_mode":
-00000ae0: 2022 696e 222c 0d0a 2020 2020 2020 2020   "in",..        
-00000af0: 2020 2274 7970 6522 3a20 2246 6c6f 6174    "type": "Float
-00000b00: 222c 0d0a 2020 2020 2020 2020 2020 2273  ",..          "s
-00000b10: 6861 7065 223a 2022 2835 2c29 222c 0d0a  hape": "(5,)",..
-00000b20: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
-00000b30: 223a 206e 756c 6c2c 0d0a 2020 2020 2020  ": null,..      
-00000b40: 2020 2020 2264 6573 6322 3a20 2222 0d0a      "desc": ""..
-00000b50: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-00000b60: 205d 0d0a 2020 2020 7d2c 0d0a 2020 2020   ]..    },..    
-00000b70: 7b0d 0a20 2020 2020 2022 6e61 6d65 223a  {..      "name":
-00000b80: 2022 4943 6f6d 7022 2c0d 0a20 2020 2020   "IComp",..     
-00000b90: 2022 7661 7269 6162 6c65 735f 6174 7472   "variables_attr
-00000ba0: 6962 7574 6573 223a 205b 0d0a 2020 2020  ibutes": [..    
-00000bb0: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
-00000bc0: 2022 6e61 6d65 223a 2022 4922 2c0d 0a20   "name": "I",.. 
-00000bd0: 2020 2020 2020 2020 2022 696f 5f6d 6f64           "io_mod
-00000be0: 6522 3a20 226f 7574 222c 0d0a 2020 2020  e": "out",..    
-00000bf0: 2020 2020 2020 2274 7970 6522 3a20 2246        "type": "F
-00000c00: 6c6f 6174 222c 0d0a 2020 2020 2020 2020  loat",..        
-00000c10: 2020 2273 6861 7065 223a 2022 2835 302c    "shape": "(50,
-00000c20: 2922 2c0d 0a20 2020 2020 2020 2020 2022  )",..          "
-00000c30: 756e 6974 7322 3a20 6e75 6c6c 2c0d 0a20  units": null,.. 
-00000c40: 2020 2020 2020 2020 2022 6465 7363 223a           "desc":
-00000c50: 2022 220d 0a20 2020 2020 2020 207d 2c0d   ""..        },.
-00000c60: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
-00000c70: 2020 2020 2020 226e 616d 6522 3a20 2268        "name": "h
-00000c80: 222c 0d0a 2020 2020 2020 2020 2020 2269  ",..          "i
-00000c90: 6f5f 6d6f 6465 223a 2022 696e 222c 0d0a  o_mode": "in",..
-00000ca0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00000cb0: 3a20 2246 6c6f 6174 222c 0d0a 2020 2020  : "Float",..    
-00000cc0: 2020 2020 2020 2273 6861 7065 223a 2022        "shape": "
-00000cd0: 2831 2c20 3530 2922 2c0d 0a20 2020 2020  (1, 50)",..     
-00000ce0: 2020 2020 2022 756e 6974 7322 3a20 6e75       "units": nu
-00000cf0: 6c6c 2c0d 0a20 2020 2020 2020 2020 2022  ll,..          "
-00000d00: 6465 7363 223a 2022 220d 0a20 2020 2020  desc": ""..     
-00000d10: 2020 207d 0d0a 2020 2020 2020 5d0d 0a20     }..      ].. 
-00000d20: 2020 207d 2c0d 0a20 2020 207b 0d0a 2020     },..    {..  
-00000d30: 2020 2020 226e 616d 6522 3a20 224c 6f63      "name": "Loc
-00000d40: 616c 5374 6966 666e 6573 734d 6174 7269  alStiffnessMatri
-00000d50: 7843 6f6d 7022 2c0d 0a20 2020 2020 2022  xComp",..      "
-00000d60: 7661 7269 6162 6c65 735f 6174 7472 6962  variables_attrib
-00000d70: 7574 6573 223a 205b 0d0a 2020 2020 2020  utes": [..      
-00000d80: 2020 7b0d 0a20 2020 2020 2020 2020 2022    {..          "
-00000d90: 6e61 6d65 223a 2022 4b5f 6c6f 6361 6c22  name": "K_local"
-00000da0: 2c0d 0a20 2020 2020 2020 2020 2022 696f  ,..          "io
-00000db0: 5f6d 6f64 6522 3a20 226f 7574 222c 0d0a  _mode": "out",..
-00000dc0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00000dd0: 3a20 2246 6c6f 6174 222c 0d0a 2020 2020  : "Float",..    
-00000de0: 2020 2020 2020 2273 6861 7065 223a 2022        "shape": "
-00000df0: 2835 302c 2034 2c20 3429 222c 0d0a 2020  (50, 4, 4)",..  
-00000e00: 2020 2020 2020 2020 2275 6e69 7473 223a          "units":
-00000e10: 206e 756c 6c2c 0d0a 2020 2020 2020 2020   null,..        
-00000e20: 2020 2264 6573 6322 3a20 2222 0d0a 2020    "desc": ""..  
-00000e30: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
-00000e40: 2020 7b0d 0a20 2020 2020 2020 2020 2022    {..          "
-00000e50: 6e61 6d65 223a 2022 4922 2c0d 0a20 2020  name": "I",..   
-00000e60: 2020 2020 2020 2022 696f 5f6d 6f64 6522         "io_mode"
-00000e70: 3a20 2269 6e22 2c0d 0a20 2020 2020 2020  : "in",..       
-00000e80: 2020 2022 7479 7065 223a 2022 466c 6f61     "type": "Floa
-00000e90: 7422 2c0d 0a20 2020 2020 2020 2020 2022  t",..          "
-00000ea0: 7368 6170 6522 3a20 2228 3530 2c29 222c  shape": "(50,)",
-00000eb0: 0d0a 2020 2020 2020 2020 2020 2275 6e69  ..          "uni
-00000ec0: 7473 223a 206e 756c 6c2c 0d0a 2020 2020  ts": null,..    
-00000ed0: 2020 2020 2020 2264 6573 6322 3a20 2222        "desc": ""
-00000ee0: 0d0a 2020 2020 2020 2020 7d0d 0a20 2020  ..        }..   
-00000ef0: 2020 205d 0d0a 2020 2020 7d2c 0d0a 2020     ]..    },..  
-00000f00: 2020 7b0d 0a20 2020 2020 2022 6e61 6d65    {..      "name
-00000f10: 223a 2022 5061 7261 6c6c 656c 222c 0d0a  ": "Parallel",..
-00000f20: 2020 2020 2020 2273 7562 5f61 6e61 6c79        "sub_analy
-00000f30: 7369 735f 6174 7472 6962 7574 6573 223a  sis_attributes":
-00000f40: 207b 0d0a 2020 2020 2020 2020 226e 616d   {..        "nam
-00000f50: 6522 3a20 2250 6172 616c 6c65 6c22 2c0d  e": "Parallel",.
-00000f60: 0a20 2020 2020 2020 2022 6469 7363 6970  .        "discip
-00000f70: 6c69 6e65 735f 6174 7472 6962 7574 6573  lines_attributes
-00000f80: 223a 205b 0d0a 2020 2020 2020 2020 2020  ": [..          
-00000f90: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
-00000fa0: 6e61 6d65 223a 2022 5f5f 4452 4956 4552  name": "__DRIVER
-00000fb0: 5f5f 222c 0d0a 2020 2020 2020 2020 2020  __",..          
-00000fc0: 2020 2276 6172 6961 626c 6573 5f61 7474    "variables_att
-00000fd0: 7269 6275 7465 7322 3a20 5b0d 0a20 2020  ributes": [..   
-00000fe0: 2020 2020 2020 2020 2020 207b 0d0a 2020             {..  
-00000ff0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00001000: 616d 6522 3a20 224b 5f6c 6f63 616c 222c  ame": "K_local",
-00001010: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001020: 2020 2269 6f5f 6d6f 6465 223a 2022 6f75    "io_mode": "ou
-00001030: 7422 2c0d 0a20 2020 2020 2020 2020 2020  t",..           
-00001040: 2020 2020 2022 6465 7363 223a 2022 222c       "desc": "",
-00001050: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001060: 2020 2274 7970 6522 3a20 2246 6c6f 6174    "type": "Float
-00001070: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00001080: 2020 2020 2273 6861 7065 223a 2022 2835      "shape": "(5
-00001090: 302c 2034 2c20 3429 222c 0d0a 2020 2020  0, 4, 4)",..    
-000010a0: 2020 2020 2020 2020 2020 2020 2275 6e69              "uni
-000010b0: 7473 223a 206e 756c 6c2c 0d0a 2020 2020  ts": null,..    
-000010c0: 2020 2020 2020 2020 2020 2020 2270 6172              "par
-000010d0: 616d 6574 6572 5f61 7474 7269 6275 7465  ameter_attribute
-000010e0: 7322 3a20 7b0d 0a20 2020 2020 2020 2020  s": {..         
-000010f0: 2020 2020 2020 2020 2022 696e 6974 223a           "init":
-00001100: 2022 5b5b 5b31 2e30 2c20 312e 302c 2031   "[[[1.0, 1.0, 1
-00001110: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-00001120: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-00001130: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00001140: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
-00001150: 2031 2e30 2c20 312e 305d 5d2c 205b 5b31   1.0, 1.0]], [[1
-00001160: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-00001170: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
-00001180: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-00001190: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-000011a0: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-000011b0: 312e 305d 5d2c 205b 5b31 2e30 2c20 312e  1.0]], [[1.0, 1.
-000011c0: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
-000011d0: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-000011e0: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
-000011f0: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-00001200: 312e 302c 2031 2e30 2c20 312e 305d 5d2c  1.0, 1.0, 1.0]],
-00001210: 205b 5b31 2e30 2c20 312e 302c 2031 2e30   [[1.0, 1.0, 1.0
-00001220: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
-00001230: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
-00001240: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-00001250: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
-00001260: 2e30 2c20 312e 305d 5d2c 205b 5b31 2e30  .0, 1.0]], [[1.0
-00001270: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-00001280: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
-00001290: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
-000012a0: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
-000012b0: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-000012c0: 305d 5d2c 205b 5b31 2e30 2c20 312e 302c  0]], [[1.0, 1.0,
-000012d0: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
-000012e0: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-000012f0: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
-00001300: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
-00001310: 302c 2031 2e30 2c20 312e 305d 5d2c 205b  0, 1.0, 1.0]], [
-00001320: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00001330: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
-00001340: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
-00001350: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-00001360: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
-00001370: 2c20 312e 305d 5d2c 205b 5b31 2e30 2c20  , 1.0]], [[1.0, 
-00001380: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-00001390: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-000013a0: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
-000013b0: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
-000013c0: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-000013d0: 5d2c 205b 5b31 2e30 2c20 312e 302c 2031  ], [[1.0, 1.0, 1
-000013e0: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-000013f0: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-00001400: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00001410: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
-00001420: 2031 2e30 2c20 312e 305d 5d2c 205b 5b31   1.0, 1.0]], [[1
-00001430: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-00001440: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
-00001450: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-00001460: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-00001470: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00001480: 312e 305d 5d2c 205b 5b31 2e30 2c20 312e  1.0]], [[1.0, 1.
-00001490: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
-000014a0: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-000014b0: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
-000014c0: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-000014d0: 312e 302c 2031 2e30 2c20 312e 305d 5d2c  1.0, 1.0, 1.0]],
-000014e0: 205b 5b31 2e30 2c20 312e 302c 2031 2e30   [[1.0, 1.0, 1.0
-000014f0: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
-00001500: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
-00001510: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-00001520: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
-00001530: 2e30 2c20 312e 305d 5d2c 205b 5b31 2e30  .0, 1.0]], [[1.0
-00001540: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-00001550: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
-00001560: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
-00001570: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
-00001580: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-00001590: 305d 5d2c 205b 5b31 2e30 2c20 312e 302c  0]], [[1.0, 1.0,
-000015a0: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
-000015b0: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-000015c0: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
-000015d0: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
-000015e0: 302c 2031 2e30 2c20 312e 305d 5d2c 205b  0, 1.0, 1.0]], [
-000015f0: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00001600: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
-00001610: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
-00001620: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-00001630: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
-00001640: 2c20 312e 305d 5d2c 205b 5b31 2e30 2c20  , 1.0]], [[1.0, 
-00001650: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-00001660: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00001670: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
-00001680: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
-00001690: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-000016a0: 5d2c 205b 5b31 2e30 2c20 312e 302c 2031  ], [[1.0, 1.0, 1
-000016b0: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-000016c0: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-000016d0: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-000016e0: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
-000016f0: 2031 2e30 2c20 312e 305d 5d2c 205b 5b31   1.0, 1.0]], [[1
-00001700: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-00001710: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
-00001720: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-00001730: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-00001740: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00001750: 312e 305d 5d2c 205b 5b31 2e30 2c20 312e  1.0]], [[1.0, 1.
-00001760: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
-00001770: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-00001780: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
-00001790: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-000017a0: 312e 302c 2031 2e30 2c20 312e 305d 5d2c  1.0, 1.0, 1.0]],
-000017b0: 205b 5b31 2e30 2c20 312e 302c 2031 2e30   [[1.0, 1.0, 1.0
-000017c0: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
-000017d0: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
-000017e0: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-000017f0: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
-00001800: 2e30 2c20 312e 305d 5d2c 205b 5b31 2e30  .0, 1.0]], [[1.0
-00001810: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-00001820: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
-00001830: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
-00001840: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
-00001850: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-00001860: 305d 5d2c 205b 5b31 2e30 2c20 312e 302c  0]], [[1.0, 1.0,
-00001870: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
-00001880: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-00001890: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
-000018a0: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
-000018b0: 302c 2031 2e30 2c20 312e 305d 5d2c 205b  0, 1.0, 1.0]], [
-000018c0: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-000018d0: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
-000018e0: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
-000018f0: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-00001900: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
-00001910: 2c20 312e 305d 5d2c 205b 5b31 2e30 2c20  , 1.0]], [[1.0, 
-00001920: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-00001930: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00001940: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
-00001950: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
-00001960: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-00001970: 5d2c 205b 5b31 2e30 2c20 312e 302c 2031  ], [[1.0, 1.0, 1
-00001980: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-00001990: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-000019a0: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-000019b0: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
-000019c0: 2031 2e30 2c20 312e 305d 5d2c 205b 5b31   1.0, 1.0]], [[1
-000019d0: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-000019e0: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
-000019f0: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-00001a00: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-00001a10: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00001a20: 312e 305d 5d2c 205b 5b31 2e30 2c20 312e  1.0]], [[1.0, 1.
-00001a30: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
-00001a40: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-00001a50: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
-00001a60: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-00001a70: 312e 302c 2031 2e30 2c20 312e 305d 5d2c  1.0, 1.0, 1.0]],
-00001a80: 205b 5b31 2e30 2c20 312e 302c 2031 2e30   [[1.0, 1.0, 1.0
-00001a90: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
-00001aa0: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
-00001ab0: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-00001ac0: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
-00001ad0: 2e30 2c20 312e 305d 5d2c 205b 5b31 2e30  .0, 1.0]], [[1.0
-00001ae0: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-00001af0: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
-00001b00: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
-00001b10: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
-00001b20: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-00001b30: 305d 5d2c 205b 5b31 2e30 2c20 312e 302c  0]], [[1.0, 1.0,
-00001b40: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
-00001b50: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-00001b60: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
-00001b70: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
-00001b80: 302c 2031 2e30 2c20 312e 305d 5d2c 205b  0, 1.0, 1.0]], [
-00001b90: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00001ba0: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
-00001bb0: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
-00001bc0: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-00001bd0: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
-00001be0: 2c20 312e 305d 5d2c 205b 5b31 2e30 2c20  , 1.0]], [[1.0, 
-00001bf0: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-00001c00: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00001c10: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
-00001c20: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
-00001c30: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-00001c40: 5d2c 205b 5b31 2e30 2c20 312e 302c 2031  ], [[1.0, 1.0, 1
-00001c50: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-00001c60: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-00001c70: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00001c80: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
-00001c90: 2031 2e30 2c20 312e 305d 5d2c 205b 5b31   1.0, 1.0]], [[1
-00001ca0: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-00001cb0: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
-00001cc0: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-00001cd0: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-00001ce0: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00001cf0: 312e 305d 5d2c 205b 5b31 2e30 2c20 312e  1.0]], [[1.0, 1.
-00001d00: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
-00001d10: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-00001d20: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
-00001d30: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-00001d40: 312e 302c 2031 2e30 2c20 312e 305d 5d2c  1.0, 1.0, 1.0]],
-00001d50: 205b 5b31 2e30 2c20 312e 302c 2031 2e30   [[1.0, 1.0, 1.0
-00001d60: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
-00001d70: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
-00001d80: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-00001d90: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
-00001da0: 2e30 2c20 312e 305d 5d2c 205b 5b31 2e30  .0, 1.0]], [[1.0
-00001db0: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-00001dc0: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
-00001dd0: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
-00001de0: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
-00001df0: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-00001e00: 305d 5d2c 205b 5b31 2e30 2c20 312e 302c  0]], [[1.0, 1.0,
-00001e10: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
-00001e20: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-00001e30: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
-00001e40: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
-00001e50: 302c 2031 2e30 2c20 312e 305d 5d2c 205b  0, 1.0, 1.0]], [
-00001e60: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00001e70: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
-00001e80: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
-00001e90: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-00001ea0: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
-00001eb0: 2c20 312e 305d 5d2c 205b 5b31 2e30 2c20  , 1.0]], [[1.0, 
-00001ec0: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-00001ed0: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00001ee0: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
-00001ef0: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
-00001f00: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-00001f10: 5d2c 205b 5b31 2e30 2c20 312e 302c 2031  ], [[1.0, 1.0, 1
-00001f20: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-00001f30: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-00001f40: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00001f50: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
-00001f60: 2031 2e30 2c20 312e 305d 5d2c 205b 5b31   1.0, 1.0]], [[1
-00001f70: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-00001f80: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
-00001f90: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-00001fa0: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-00001fb0: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00001fc0: 312e 305d 5d2c 205b 5b31 2e30 2c20 312e  1.0]], [[1.0, 1.
-00001fd0: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
-00001fe0: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-00001ff0: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
-00002000: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-00002010: 312e 302c 2031 2e30 2c20 312e 305d 5d2c  1.0, 1.0, 1.0]],
-00002020: 205b 5b31 2e30 2c20 312e 302c 2031 2e30   [[1.0, 1.0, 1.0
-00002030: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
-00002040: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
-00002050: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-00002060: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
-00002070: 2e30 2c20 312e 305d 5d2c 205b 5b31 2e30  .0, 1.0]], [[1.0
-00002080: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-00002090: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
-000020a0: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
-000020b0: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
-000020c0: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-000020d0: 305d 5d2c 205b 5b31 2e30 2c20 312e 302c  0]], [[1.0, 1.0,
-000020e0: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
-000020f0: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-00002100: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
-00002110: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
-00002120: 302c 2031 2e30 2c20 312e 305d 5d2c 205b  0, 1.0, 1.0]], [
-00002130: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00002140: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
-00002150: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
-00002160: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-00002170: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
-00002180: 2c20 312e 305d 5d2c 205b 5b31 2e30 2c20  , 1.0]], [[1.0, 
-00002190: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-000021a0: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-000021b0: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
-000021c0: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
-000021d0: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
-000021e0: 5d2c 205b 5b31 2e30 2c20 312e 302c 2031  ], [[1.0, 1.0, 1
-000021f0: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-00002200: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-00002210: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00002220: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
-00002230: 2031 2e30 2c20 312e 305d 5d2c 205b 5b31   1.0, 1.0]], [[1
-00002240: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
-00002250: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
-00002260: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
-00002270: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
-00002280: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
-00002290: 312e 305d 5d5d 220d 0a20 2020 2020 2020  1.0]]]"..       
-000022a0: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-000022b0: 2020 2020 2020 2020 2020 7d2c 0d0a 2020            },..  
-000022c0: 2020 2020 2020 2020 2020 2020 7b0d 0a20              {.. 
-000022d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000022e0: 6e61 6d65 223a 2022 645f 3022 2c0d 0a20  name": "d_0",.. 
-000022f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002300: 696f 5f6d 6f64 6522 3a20 2269 6e22 2c0d  io_mode": "in",.
-00002310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002320: 2022 6465 7363 223a 2022 222c 0d0a 2020   "desc": "",..  
-00002330: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00002340: 7970 6522 3a20 2246 6c6f 6174 222c 0d0a  ype": "Float",..
-00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002360: 2273 6861 7065 223a 2022 2831 3034 2c29  "shape": "(104,)
-00002370: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00002380: 2020 2020 2275 6e69 7473 223a 206e 756c      "units": nul
-00002390: 6c0d 0a20 2020 2020 2020 2020 2020 2020  l..             
-000023a0: 207d 2c0d 0a20 2020 2020 2020 2020 2020   },..           
-000023b0: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-000023c0: 2020 2020 2020 226e 616d 6522 3a20 2264        "name": "d
-000023d0: 5f31 222c 0d0a 2020 2020 2020 2020 2020  _1",..          
-000023e0: 2020 2020 2020 2269 6f5f 6d6f 6465 223a        "io_mode":
-000023f0: 2022 696e 222c 0d0a 2020 2020 2020 2020   "in",..        
-00002400: 2020 2020 2020 2020 2264 6573 6322 3a20          "desc": 
-00002410: 2222 2c0d 0a20 2020 2020 2020 2020 2020  "",..           
-00002420: 2020 2020 2022 7479 7065 223a 2022 466c       "type": "Fl
-00002430: 6f61 7422 2c0d 0a20 2020 2020 2020 2020  oat",..         
-00002440: 2020 2020 2020 2022 7368 6170 6522 3a20         "shape": 
-00002450: 2228 3130 342c 2922 2c0d 0a20 2020 2020  "(104,)",..     
-00002460: 2020 2020 2020 2020 2020 2022 756e 6974             "unit
-00002470: 7322 3a20 6e75 6c6c 0d0a 2020 2020 2020  s": null..      
-00002480: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-00002490: 2020 2020 2020 2020 2020 7b0d 0a20 2020            {..   
-000024a0: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
-000024b0: 6d65 223a 2022 6469 7370 6c61 6365 6d65  me": "displaceme
-000024c0: 6e74 735f 3022 2c0d 0a20 2020 2020 2020  nts_0",..       
-000024d0: 2020 2020 2020 2020 2022 696f 5f6d 6f64           "io_mod
-000024e0: 6522 3a20 2269 6e22 2c0d 0a20 2020 2020  e": "in",..     
-000024f0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-00002500: 223a 2022 222c 0d0a 2020 2020 2020 2020  ": "",..        
-00002510: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00002520: 2246 6c6f 6174 222c 0d0a 2020 2020 2020  "Float",..      
-00002530: 2020 2020 2020 2020 2020 2273 6861 7065            "shape
-00002540: 223a 2022 2831 3032 2c29 222c 0d0a 2020  ": "(102,)",..  
-00002550: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-00002560: 6e69 7473 223a 206e 756c 6c0d 0a20 2020  nits": null..   
-00002570: 2020 2020 2020 2020 2020 207d 2c0d 0a20             },.. 
-00002580: 2020 2020 2020 2020 2020 2020 207b 0d0a               {..
-00002590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025a0: 226e 616d 6522 3a20 2264 6973 706c 6163  "name": "displac
-000025b0: 656d 656e 7473 5f31 222c 0d0a 2020 2020  ements_1",..    
-000025c0: 2020 2020 2020 2020 2020 2020 2269 6f5f              "io_
-000025d0: 6d6f 6465 223a 2022 696e 222c 0d0a 2020  mode": "in",..  
-000025e0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-000025f0: 6573 6322 3a20 2222 2c0d 0a20 2020 2020  esc": "",..     
-00002600: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-00002610: 223a 2022 466c 6f61 7422 2c0d 0a20 2020  ": "Float",..   
-00002620: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
-00002630: 6170 6522 3a20 2228 3130 322c 2922 2c0d  ape": "(102,)",.
-00002640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002650: 2022 756e 6974 7322 3a20 6e75 6c6c 0d0a   "units": null..
-00002660: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-00002670: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002680: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00002690: 2020 2022 6e61 6d65 223a 2022 636f 6d70     "name": "comp
-000026a0: 6c69 616e 6365 5f30 222c 0d0a 2020 2020  liance_0",..    
-000026b0: 2020 2020 2020 2020 2020 2020 2269 6f5f              "io_
-000026c0: 6d6f 6465 223a 2022 696e 222c 0d0a 2020  mode": "in",..  
-000026d0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-000026e0: 6573 6322 3a20 2222 2c0d 0a20 2020 2020  esc": "",..     
-000026f0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-00002700: 223a 2022 466c 6f61 7422 2c0d 0a20 2020  ": "Float",..   
-00002710: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
-00002720: 6170 6522 3a20 2231 222c 0d0a 2020 2020  ape": "1",..    
+00000000: 7b0a 2020 226e 616d 6522 3a20 224d 756c  {.  "name": "Mul
+00000010: 7469 706f 696e 7442 6561 6d47 726f 7570  tipointBeamGroup
+00000020: 222c 0a20 2022 6469 7363 6970 6c69 6e65  ",.  "discipline
+00000030: 735f 6174 7472 6962 7574 6573 223a 205b  s_attributes": [
+00000040: 0a20 2020 207b 0a20 2020 2020 2022 6e61  .    {.      "na
+00000050: 6d65 223a 2022 5f5f 4452 4956 4552 5f5f  me": "__DRIVER__
+00000060: 222c 0a20 2020 2020 2022 7661 7269 6162  ",.      "variab
+00000070: 6c65 735f 6174 7472 6962 7574 6573 223a  les_attributes":
+00000080: 205b 0a20 2020 2020 2020 207b 0a20 2020   [.        {.   
+00000090: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
+000000a0: 685f 6370 222c 0a20 2020 2020 2020 2020  h_cp",.         
+000000b0: 2022 696f 5f6d 6f64 6522 3a20 226f 7574   "io_mode": "out
+000000c0: 222c 0a20 2020 2020 2020 2020 2022 6465  ",.          "de
+000000d0: 7363 223a 2022 222c 0a20 2020 2020 2020  sc": "",.       
+000000e0: 2020 2022 7479 7065 223a 2022 466c 6f61     "type": "Floa
+000000f0: 7422 2c0a 2020 2020 2020 2020 2020 2273  t",.          "s
+00000100: 6861 7065 223a 2022 2835 2c29 222c 0a20  hape": "(5,)",. 
+00000110: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
+00000120: 3a20 6e75 6c6c 2c0a 2020 2020 2020 2020  : null,.        
+00000130: 2020 2270 6172 616d 6574 6572 5f61 7474    "parameter_att
+00000140: 7269 6275 7465 7322 3a20 7b0a 2020 2020  ributes": {.    
+00000150: 2020 2020 2020 2020 2269 6e69 7422 3a20          "init": 
+00000160: 225b 312e 302c 2031 2e30 2c20 312e 302c  "[1.0, 1.0, 1.0,
+00000170: 2031 2e30 2c20 312e 305d 220a 2020 2020   1.0, 1.0]".    
+00000180: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00000190: 7d2c 0a20 2020 2020 2020 207b 0a20 2020  },.        {.   
+000001a0: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
+000001b0: 6822 2c0a 2020 2020 2020 2020 2020 2269  h",.          "i
+000001c0: 6f5f 6d6f 6465 223a 2022 696e 222c 0a20  o_mode": "in",. 
+000001d0: 2020 2020 2020 2020 2022 6465 7363 223a           "desc":
+000001e0: 2022 222c 0a20 2020 2020 2020 2020 2022   "",.          "
+000001f0: 7479 7065 223a 2022 466c 6f61 7422 2c0a  type": "Float",.
+00000200: 2020 2020 2020 2020 2020 2273 6861 7065            "shape
+00000210: 223a 2022 2831 2c20 3530 2922 2c0a 2020  ": "(1, 50)",.  
+00000220: 2020 2020 2020 2020 2275 6e69 7473 223a          "units":
+00000230: 206e 756c 6c0a 2020 2020 2020 2020 7d2c   null.        },
+00000240: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+00000250: 2020 2020 2022 6e61 6d65 223a 2022 4922       "name": "I"
+00000260: 2c0a 2020 2020 2020 2020 2020 2269 6f5f  ,.          "io_
+00000270: 6d6f 6465 223a 2022 696e 222c 0a20 2020  mode": "in",.   
+00000280: 2020 2020 2020 2022 6465 7363 223a 2022         "desc": "
+00000290: 222c 0a20 2020 2020 2020 2020 2022 7479  ",.          "ty
+000002a0: 7065 223a 2022 466c 6f61 7422 2c0a 2020  pe": "Float",.  
+000002b0: 2020 2020 2020 2020 2273 6861 7065 223a          "shape":
+000002c0: 2022 2835 302c 2922 2c0a 2020 2020 2020   "(50,)",.      
+000002d0: 2020 2020 2275 6e69 7473 223a 206e 756c      "units": nul
+000002e0: 6c0a 2020 2020 2020 2020 7d2c 0a20 2020  l.        },.   
+000002f0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00000300: 2022 6e61 6d65 223a 2022 4b5f 6c6f 6361   "name": "K_loca
+00000310: 6c22 2c0a 2020 2020 2020 2020 2020 2269  l",.          "i
+00000320: 6f5f 6d6f 6465 223a 2022 696e 222c 0a20  o_mode": "in",. 
+00000330: 2020 2020 2020 2020 2022 6465 7363 223a           "desc":
+00000340: 2022 222c 0a20 2020 2020 2020 2020 2022   "",.          "
+00000350: 7479 7065 223a 2022 466c 6f61 7422 2c0a  type": "Float",.
+00000360: 2020 2020 2020 2020 2020 2273 6861 7065            "shape
+00000370: 223a 2022 2835 302c 2034 2c20 3429 222c  ": "(50, 4, 4)",
+00000380: 0a20 2020 2020 2020 2020 2022 756e 6974  .          "unit
+00000390: 7322 3a20 6e75 6c6c 0a20 2020 2020 2020  s": null.       
+000003a0: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
+000003b0: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
+000003c0: 2264 5f30 222c 0a20 2020 2020 2020 2020  "d_0",.         
+000003d0: 2022 696f 5f6d 6f64 6522 3a20 2269 6e22   "io_mode": "in"
+000003e0: 2c0a 2020 2020 2020 2020 2020 2264 6573  ,.          "des
+000003f0: 6322 3a20 2222 2c0a 2020 2020 2020 2020  c": "",.        
+00000400: 2020 2274 7970 6522 3a20 2246 6c6f 6174    "type": "Float
+00000410: 222c 0a20 2020 2020 2020 2020 2022 7368  ",.          "sh
+00000420: 6170 6522 3a20 2228 3130 342c 2922 2c0a  ape": "(104,)",.
+00000430: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
+00000440: 223a 206e 756c 6c0a 2020 2020 2020 2020  ": null.        
+00000450: 7d2c 0a20 2020 2020 2020 207b 0a20 2020  },.        {.   
+00000460: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
+00000470: 645f 3122 2c0a 2020 2020 2020 2020 2020  d_1",.          
+00000480: 2269 6f5f 6d6f 6465 223a 2022 696e 222c  "io_mode": "in",
+00000490: 0a20 2020 2020 2020 2020 2022 6465 7363  .          "desc
+000004a0: 223a 2022 222c 0a20 2020 2020 2020 2020  ": "",.         
+000004b0: 2022 7479 7065 223a 2022 466c 6f61 7422   "type": "Float"
+000004c0: 2c0a 2020 2020 2020 2020 2020 2273 6861  ,.          "sha
+000004d0: 7065 223a 2022 2831 3034 2c29 222c 0a20  pe": "(104,)",. 
+000004e0: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
+000004f0: 3a20 6e75 6c6c 0a20 2020 2020 2020 207d  : null.        }
+00000500: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
+00000510: 2020 2020 2020 226e 616d 6522 3a20 2264        "name": "d
+00000520: 6973 706c 6163 656d 656e 7473 5f30 222c  isplacements_0",
+00000530: 0a20 2020 2020 2020 2020 2022 696f 5f6d  .          "io_m
+00000540: 6f64 6522 3a20 2269 6e22 2c0a 2020 2020  ode": "in",.    
+00000550: 2020 2020 2020 2264 6573 6322 3a20 2222        "desc": ""
+00000560: 2c0a 2020 2020 2020 2020 2020 2274 7970  ,.          "typ
+00000570: 6522 3a20 2246 6c6f 6174 222c 0a20 2020  e": "Float",.   
+00000580: 2020 2020 2020 2022 7368 6170 6522 3a20         "shape": 
+00000590: 2228 3130 322c 2922 2c0a 2020 2020 2020  "(102,)",.      
+000005a0: 2020 2020 2275 6e69 7473 223a 206e 756c      "units": nul
+000005b0: 6c0a 2020 2020 2020 2020 7d2c 0a20 2020  l.        },.   
+000005c0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+000005d0: 2022 6e61 6d65 223a 2022 6469 7370 6c61   "name": "displa
+000005e0: 6365 6d65 6e74 735f 3122 2c0a 2020 2020  cements_1",.    
+000005f0: 2020 2020 2020 2269 6f5f 6d6f 6465 223a        "io_mode":
+00000600: 2022 696e 222c 0a20 2020 2020 2020 2020   "in",.         
+00000610: 2022 6465 7363 223a 2022 222c 0a20 2020   "desc": "",.   
+00000620: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+00000630: 466c 6f61 7422 2c0a 2020 2020 2020 2020  Float",.        
+00000640: 2020 2273 6861 7065 223a 2022 2831 3032    "shape": "(102
+00000650: 2c29 222c 0a20 2020 2020 2020 2020 2022  ,)",.          "
+00000660: 756e 6974 7322 3a20 6e75 6c6c 0a20 2020  units": null.   
+00000670: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00000680: 7b0a 2020 2020 2020 2020 2020 226e 616d  {.          "nam
+00000690: 6522 3a20 2263 6f6d 706c 6961 6e63 655f  e": "compliance_
+000006a0: 3022 2c0a 2020 2020 2020 2020 2020 2269  0",.          "i
+000006b0: 6f5f 6d6f 6465 223a 2022 696e 222c 0a20  o_mode": "in",. 
+000006c0: 2020 2020 2020 2020 2022 6465 7363 223a           "desc":
+000006d0: 2022 222c 0a20 2020 2020 2020 2020 2022   "",.          "
+000006e0: 7479 7065 223a 2022 466c 6f61 7422 2c0a  type": "Float",.
+000006f0: 2020 2020 2020 2020 2020 2273 6861 7065            "shape
+00000700: 223a 2022 3122 2c0a 2020 2020 2020 2020  ": "1",.        
+00000710: 2020 2275 6e69 7473 223a 206e 756c 6c0a    "units": null.
+00000720: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00000730: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
+00000740: 6e61 6d65 223a 2022 636f 6d70 6c69 616e  name": "complian
+00000750: 6365 5f31 222c 0a20 2020 2020 2020 2020  ce_1",.         
+00000760: 2022 696f 5f6d 6f64 6522 3a20 2269 6e22   "io_mode": "in"
+00000770: 2c0a 2020 2020 2020 2020 2020 2264 6573  ,.          "des
+00000780: 6322 3a20 2222 2c0a 2020 2020 2020 2020  c": "",.        
+00000790: 2020 2274 7970 6522 3a20 2246 6c6f 6174    "type": "Float
+000007a0: 222c 0a20 2020 2020 2020 2020 2022 7368  ",.          "sh
+000007b0: 6170 6522 3a20 2231 222c 0a20 2020 2020  ape": "1",.     
+000007c0: 2020 2020 2022 756e 6974 7322 3a20 6e75       "units": nu
+000007d0: 6c6c 0a20 2020 2020 2020 207d 2c0a 2020  ll.        },.  
+000007e0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+000007f0: 2020 226e 616d 6522 3a20 2276 6f6c 756d    "name": "volum
+00000800: 6522 2c0a 2020 2020 2020 2020 2020 2269  e",.          "i
+00000810: 6f5f 6d6f 6465 223a 2022 696e 222c 0a20  o_mode": "in",. 
+00000820: 2020 2020 2020 2020 2022 6465 7363 223a           "desc":
+00000830: 2022 222c 0a20 2020 2020 2020 2020 2022   "",.          "
+00000840: 7479 7065 223a 2022 466c 6f61 7422 2c0a  type": "Float",.
+00000850: 2020 2020 2020 2020 2020 2273 6861 7065            "shape
+00000860: 223a 2022 3122 2c0a 2020 2020 2020 2020  ": "1",.        
+00000870: 2020 2275 6e69 7473 223a 206e 756c 6c0a    "units": null.
+00000880: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00000890: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
+000008a0: 6e61 6d65 223a 2022 6f62 6a22 2c0a 2020  name": "obj",.  
+000008b0: 2020 2020 2020 2020 2269 6f5f 6d6f 6465          "io_mode
+000008c0: 223a 2022 696e 222c 0a20 2020 2020 2020  ": "in",.       
+000008d0: 2020 2022 6465 7363 223a 2022 222c 0a20     "desc": "",. 
+000008e0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+000008f0: 2022 466c 6f61 7422 2c0a 2020 2020 2020   "Float",.      
+00000900: 2020 2020 2273 6861 7065 223a 2022 3122      "shape": "1"
+00000910: 2c0a 2020 2020 2020 2020 2020 2275 6e69  ,.          "uni
+00000920: 7473 223a 206e 756c 6c0a 2020 2020 2020  ts": null.      
+00000930: 2020 7d0a 2020 2020 2020 5d0a 2020 2020    }.      ].    
+00000940: 7d2c 0a20 2020 207b 0a20 2020 2020 2022  },.    {.      "
+00000950: 6e61 6d65 223a 2022 496e 7465 7270 222c  name": "Interp",
+00000960: 0a20 2020 2020 2022 7661 7269 6162 6c65  .      "variable
+00000970: 735f 6174 7472 6962 7574 6573 223a 205b  s_attributes": [
+00000980: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+00000990: 2020 2020 2022 6e61 6d65 223a 2022 6822       "name": "h"
+000009a0: 2c0a 2020 2020 2020 2020 2020 2269 6f5f  ,.          "io_
+000009b0: 6d6f 6465 223a 2022 6f75 7422 2c0a 2020  mode": "out",.  
+000009c0: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+000009d0: 2246 6c6f 6174 222c 0a20 2020 2020 2020  "Float",.       
+000009e0: 2020 2022 7368 6170 6522 3a20 2228 312c     "shape": "(1,
+000009f0: 2035 3029 222c 0a20 2020 2020 2020 2020   50)",.         
+00000a00: 2022 756e 6974 7322 3a20 6e75 6c6c 2c0a   "units": null,.
+00000a10: 2020 2020 2020 2020 2020 2264 6573 6322            "desc"
+00000a20: 3a20 2222 0a20 2020 2020 2020 207d 2c0a  : "".        },.
+00000a30: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00000a40: 2020 2020 226e 616d 6522 3a20 2268 5f63      "name": "h_c
+00000a50: 7022 2c0a 2020 2020 2020 2020 2020 2269  p",.          "i
+00000a60: 6f5f 6d6f 6465 223a 2022 696e 222c 0a20  o_mode": "in",. 
+00000a70: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00000a80: 2022 466c 6f61 7422 2c0a 2020 2020 2020   "Float",.      
+00000a90: 2020 2020 2273 6861 7065 223a 2022 2835      "shape": "(5
+00000aa0: 2c29 222c 0a20 2020 2020 2020 2020 2022  ,)",.          "
+00000ab0: 756e 6974 7322 3a20 6e75 6c6c 2c0a 2020  units": null,.  
+00000ac0: 2020 2020 2020 2020 2264 6573 6322 3a20          "desc": 
+00000ad0: 2222 0a20 2020 2020 2020 207d 0a20 2020  "".        }.   
+00000ae0: 2020 205d 0a20 2020 207d 2c0a 2020 2020     ].    },.    
+00000af0: 7b0a 2020 2020 2020 226e 616d 6522 3a20  {.      "name": 
+00000b00: 2249 436f 6d70 222c 0a20 2020 2020 2022  "IComp",.      "
+00000b10: 7661 7269 6162 6c65 735f 6174 7472 6962  variables_attrib
+00000b20: 7574 6573 223a 205b 0a20 2020 2020 2020  utes": [.       
+00000b30: 207b 0a20 2020 2020 2020 2020 2022 6e61   {.          "na
+00000b40: 6d65 223a 2022 4922 2c0a 2020 2020 2020  me": "I",.      
+00000b50: 2020 2020 2269 6f5f 6d6f 6465 223a 2022      "io_mode": "
+00000b60: 6f75 7422 2c0a 2020 2020 2020 2020 2020  out",.          
+00000b70: 2274 7970 6522 3a20 2246 6c6f 6174 222c  "type": "Float",
+00000b80: 0a20 2020 2020 2020 2020 2022 7368 6170  .          "shap
+00000b90: 6522 3a20 2228 3530 2c29 222c 0a20 2020  e": "(50,)",.   
+00000ba0: 2020 2020 2020 2022 756e 6974 7322 3a20         "units": 
+00000bb0: 6e75 6c6c 2c0a 2020 2020 2020 2020 2020  null,.          
+00000bc0: 2264 6573 6322 3a20 2222 0a20 2020 2020  "desc": "".     
+00000bd0: 2020 207d 2c0a 2020 2020 2020 2020 7b0a     },.        {.
+00000be0: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
+00000bf0: 3a20 2268 222c 0a20 2020 2020 2020 2020  : "h",.         
+00000c00: 2022 696f 5f6d 6f64 6522 3a20 2269 6e22   "io_mode": "in"
+00000c10: 2c0a 2020 2020 2020 2020 2020 2274 7970  ,.          "typ
+00000c20: 6522 3a20 2246 6c6f 6174 222c 0a20 2020  e": "Float",.   
+00000c30: 2020 2020 2020 2022 7368 6170 6522 3a20         "shape": 
+00000c40: 2228 312c 2035 3029 222c 0a20 2020 2020  "(1, 50)",.     
+00000c50: 2020 2020 2022 756e 6974 7322 3a20 6e75       "units": nu
+00000c60: 6c6c 2c0a 2020 2020 2020 2020 2020 2264  ll,.          "d
+00000c70: 6573 6322 3a20 2222 0a20 2020 2020 2020  esc": "".       
+00000c80: 207d 0a20 2020 2020 205d 0a20 2020 207d   }.      ].    }
+00000c90: 2c0a 2020 2020 7b0a 2020 2020 2020 226e  ,.    {.      "n
+00000ca0: 616d 6522 3a20 224c 6f63 616c 5374 6966  ame": "LocalStif
+00000cb0: 666e 6573 734d 6174 7269 7843 6f6d 7022  fnessMatrixComp"
+00000cc0: 2c0a 2020 2020 2020 2276 6172 6961 626c  ,.      "variabl
+00000cd0: 6573 5f61 7474 7269 6275 7465 7322 3a20  es_attributes": 
+00000ce0: 5b0a 2020 2020 2020 2020 7b0a 2020 2020  [.        {.    
+00000cf0: 2020 2020 2020 226e 616d 6522 3a20 224b        "name": "K
+00000d00: 5f6c 6f63 616c 222c 0a20 2020 2020 2020  _local",.       
+00000d10: 2020 2022 696f 5f6d 6f64 6522 3a20 226f     "io_mode": "o
+00000d20: 7574 222c 0a20 2020 2020 2020 2020 2022  ut",.          "
+00000d30: 7479 7065 223a 2022 466c 6f61 7422 2c0a  type": "Float",.
+00000d40: 2020 2020 2020 2020 2020 2273 6861 7065            "shape
+00000d50: 223a 2022 2835 302c 2034 2c20 3429 222c  ": "(50, 4, 4)",
+00000d60: 0a20 2020 2020 2020 2020 2022 756e 6974  .          "unit
+00000d70: 7322 3a20 6e75 6c6c 2c0a 2020 2020 2020  s": null,.      
+00000d80: 2020 2020 2264 6573 6322 3a20 2222 0a20      "desc": "". 
+00000d90: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00000da0: 2020 7b0a 2020 2020 2020 2020 2020 226e    {.          "n
+00000db0: 616d 6522 3a20 2249 222c 0a20 2020 2020  ame": "I",.     
+00000dc0: 2020 2020 2022 696f 5f6d 6f64 6522 3a20       "io_mode": 
+00000dd0: 2269 6e22 2c0a 2020 2020 2020 2020 2020  "in",.          
+00000de0: 2274 7970 6522 3a20 2246 6c6f 6174 222c  "type": "Float",
+00000df0: 0a20 2020 2020 2020 2020 2022 7368 6170  .          "shap
+00000e00: 6522 3a20 2228 3530 2c29 222c 0a20 2020  e": "(50,)",.   
+00000e10: 2020 2020 2020 2022 756e 6974 7322 3a20         "units": 
+00000e20: 6e75 6c6c 2c0a 2020 2020 2020 2020 2020  null,.          
+00000e30: 2264 6573 6322 3a20 2222 0a20 2020 2020  "desc": "".     
+00000e40: 2020 207d 0a20 2020 2020 205d 0a20 2020     }.      ].   
+00000e50: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
+00000e60: 226e 616d 6522 3a20 2250 6172 616c 6c65  "name": "Paralle
+00000e70: 6c22 2c0a 2020 2020 2020 2273 7562 5f61  l",.      "sub_a
+00000e80: 6e61 6c79 7369 735f 6174 7472 6962 7574  nalysis_attribut
+00000e90: 6573 223a 207b 0a20 2020 2020 2020 2022  es": {.        "
+00000ea0: 6e61 6d65 223a 2022 5061 7261 6c6c 656c  name": "Parallel
+00000eb0: 222c 0a20 2020 2020 2020 2022 6469 7363  ",.        "disc
+00000ec0: 6970 6c69 6e65 735f 6174 7472 6962 7574  iplines_attribut
+00000ed0: 6573 223a 205b 0a20 2020 2020 2020 2020  es": [.         
+00000ee0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00000ef0: 6e61 6d65 223a 2022 5f5f 4452 4956 4552  name": "__DRIVER
+00000f00: 5f5f 222c 0a20 2020 2020 2020 2020 2020  __",.           
+00000f10: 2022 7661 7269 6162 6c65 735f 6174 7472   "variables_attr
+00000f20: 6962 7574 6573 223a 205b 0a20 2020 2020  ibutes": [.     
+00000f30: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00000f40: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
+00000f50: 223a 2022 4b5f 6c6f 6361 6c22 2c0a 2020  ": "K_local",.  
+00000f60: 2020 2020 2020 2020 2020 2020 2020 2269                "i
+00000f70: 6f5f 6d6f 6465 223a 2022 6f75 7422 2c0a  o_mode": "out",.
+00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f90: 2264 6573 6322 3a20 2222 2c0a 2020 2020  "desc": "",.    
+00000fa0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00000fb0: 6522 3a20 2246 6c6f 6174 222c 0a20 2020  e": "Float",.   
+00000fc0: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+00000fd0: 6170 6522 3a20 2228 3530 2c20 342c 2034  ape": "(50, 4, 4
+00000fe0: 2922 2c0a 2020 2020 2020 2020 2020 2020  )",.            
+00000ff0: 2020 2020 2275 6e69 7473 223a 206e 756c      "units": nul
+00001000: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
+00001010: 2020 2022 7061 7261 6d65 7465 725f 6174     "parameter_at
+00001020: 7472 6962 7574 6573 223a 207b 0a20 2020  tributes": {.   
+00001030: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001040: 696e 6974 223a 2022 5b5b 5b31 2e30 2c20  init": "[[[1.0, 
+00001050: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+00001060: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+00001070: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+00001080: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
+00001090: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+000010a0: 5d2c 205b 5b31 2e30 2c20 312e 302c 2031  ], [[1.0, 1.0, 1
+000010b0: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
+000010c0: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+000010d0: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+000010e0: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+000010f0: 2031 2e30 2c20 312e 305d 5d2c 205b 5b31   1.0, 1.0]], [[1
+00001100: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+00001110: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
+00001120: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
+00001130: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+00001140: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+00001150: 312e 305d 5d2c 205b 5b31 2e30 2c20 312e  1.0]], [[1.0, 1.
+00001160: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
+00001170: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+00001180: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
+00001190: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
+000011a0: 312e 302c 2031 2e30 2c20 312e 305d 5d2c  1.0, 1.0, 1.0]],
+000011b0: 205b 5b31 2e30 2c20 312e 302c 2031 2e30   [[1.0, 1.0, 1.0
+000011c0: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
+000011d0: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
+000011e0: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+000011f0: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
+00001200: 2e30 2c20 312e 305d 5d2c 205b 5b31 2e30  .0, 1.0]], [[1.0
+00001210: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+00001220: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
+00001230: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
+00001240: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
+00001250: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+00001260: 305d 5d2c 205b 5b31 2e30 2c20 312e 302c  0]], [[1.0, 1.0,
+00001270: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
+00001280: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+00001290: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
+000012a0: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
+000012b0: 302c 2031 2e30 2c20 312e 305d 5d2c 205b  0, 1.0, 1.0]], [
+000012c0: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+000012d0: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+000012e0: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
+000012f0: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+00001300: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
+00001310: 2c20 312e 305d 5d2c 205b 5b31 2e30 2c20  , 1.0]], [[1.0, 
+00001320: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+00001330: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+00001340: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+00001350: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
+00001360: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+00001370: 5d2c 205b 5b31 2e30 2c20 312e 302c 2031  ], [[1.0, 1.0, 1
+00001380: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
+00001390: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+000013a0: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+000013b0: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+000013c0: 2031 2e30 2c20 312e 305d 5d2c 205b 5b31   1.0, 1.0]], [[1
+000013d0: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+000013e0: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
+000013f0: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
+00001400: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+00001410: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+00001420: 312e 305d 5d2c 205b 5b31 2e30 2c20 312e  1.0]], [[1.0, 1.
+00001430: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
+00001440: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+00001450: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
+00001460: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
+00001470: 312e 302c 2031 2e30 2c20 312e 305d 5d2c  1.0, 1.0, 1.0]],
+00001480: 205b 5b31 2e30 2c20 312e 302c 2031 2e30   [[1.0, 1.0, 1.0
+00001490: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
+000014a0: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
+000014b0: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+000014c0: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
+000014d0: 2e30 2c20 312e 305d 5d2c 205b 5b31 2e30  .0, 1.0]], [[1.0
+000014e0: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+000014f0: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
+00001500: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
+00001510: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
+00001520: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+00001530: 305d 5d2c 205b 5b31 2e30 2c20 312e 302c  0]], [[1.0, 1.0,
+00001540: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
+00001550: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+00001560: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
+00001570: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
+00001580: 302c 2031 2e30 2c20 312e 305d 5d2c 205b  0, 1.0, 1.0]], [
+00001590: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+000015a0: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+000015b0: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
+000015c0: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+000015d0: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
+000015e0: 2c20 312e 305d 5d2c 205b 5b31 2e30 2c20  , 1.0]], [[1.0, 
+000015f0: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+00001600: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+00001610: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+00001620: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
+00001630: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+00001640: 5d2c 205b 5b31 2e30 2c20 312e 302c 2031  ], [[1.0, 1.0, 1
+00001650: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
+00001660: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+00001670: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+00001680: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+00001690: 2031 2e30 2c20 312e 305d 5d2c 205b 5b31   1.0, 1.0]], [[1
+000016a0: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+000016b0: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
+000016c0: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
+000016d0: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+000016e0: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+000016f0: 312e 305d 5d2c 205b 5b31 2e30 2c20 312e  1.0]], [[1.0, 1.
+00001700: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
+00001710: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+00001720: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
+00001730: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
+00001740: 312e 302c 2031 2e30 2c20 312e 305d 5d2c  1.0, 1.0, 1.0]],
+00001750: 205b 5b31 2e30 2c20 312e 302c 2031 2e30   [[1.0, 1.0, 1.0
+00001760: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
+00001770: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
+00001780: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+00001790: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
+000017a0: 2e30 2c20 312e 305d 5d2c 205b 5b31 2e30  .0, 1.0]], [[1.0
+000017b0: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+000017c0: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
+000017d0: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
+000017e0: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
+000017f0: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+00001800: 305d 5d2c 205b 5b31 2e30 2c20 312e 302c  0]], [[1.0, 1.0,
+00001810: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
+00001820: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+00001830: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
+00001840: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
+00001850: 302c 2031 2e30 2c20 312e 305d 5d2c 205b  0, 1.0, 1.0]], [
+00001860: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+00001870: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+00001880: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
+00001890: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+000018a0: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
+000018b0: 2c20 312e 305d 5d2c 205b 5b31 2e30 2c20  , 1.0]], [[1.0, 
+000018c0: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+000018d0: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+000018e0: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+000018f0: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
+00001900: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+00001910: 5d2c 205b 5b31 2e30 2c20 312e 302c 2031  ], [[1.0, 1.0, 1
+00001920: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
+00001930: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+00001940: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+00001950: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+00001960: 2031 2e30 2c20 312e 305d 5d2c 205b 5b31   1.0, 1.0]], [[1
+00001970: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+00001980: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
+00001990: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
+000019a0: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+000019b0: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+000019c0: 312e 305d 5d2c 205b 5b31 2e30 2c20 312e  1.0]], [[1.0, 1.
+000019d0: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
+000019e0: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+000019f0: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
+00001a00: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
+00001a10: 312e 302c 2031 2e30 2c20 312e 305d 5d2c  1.0, 1.0, 1.0]],
+00001a20: 205b 5b31 2e30 2c20 312e 302c 2031 2e30   [[1.0, 1.0, 1.0
+00001a30: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
+00001a40: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
+00001a50: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+00001a60: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
+00001a70: 2e30 2c20 312e 305d 5d2c 205b 5b31 2e30  .0, 1.0]], [[1.0
+00001a80: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+00001a90: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
+00001aa0: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
+00001ab0: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
+00001ac0: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+00001ad0: 305d 5d2c 205b 5b31 2e30 2c20 312e 302c  0]], [[1.0, 1.0,
+00001ae0: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
+00001af0: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+00001b00: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
+00001b10: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
+00001b20: 302c 2031 2e30 2c20 312e 305d 5d2c 205b  0, 1.0, 1.0]], [
+00001b30: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+00001b40: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+00001b50: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
+00001b60: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+00001b70: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
+00001b80: 2c20 312e 305d 5d2c 205b 5b31 2e30 2c20  , 1.0]], [[1.0, 
+00001b90: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+00001ba0: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+00001bb0: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+00001bc0: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
+00001bd0: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+00001be0: 5d2c 205b 5b31 2e30 2c20 312e 302c 2031  ], [[1.0, 1.0, 1
+00001bf0: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
+00001c00: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+00001c10: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+00001c20: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+00001c30: 2031 2e30 2c20 312e 305d 5d2c 205b 5b31   1.0, 1.0]], [[1
+00001c40: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+00001c50: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
+00001c60: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
+00001c70: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+00001c80: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+00001c90: 312e 305d 5d2c 205b 5b31 2e30 2c20 312e  1.0]], [[1.0, 1.
+00001ca0: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
+00001cb0: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+00001cc0: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
+00001cd0: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
+00001ce0: 312e 302c 2031 2e30 2c20 312e 305d 5d2c  1.0, 1.0, 1.0]],
+00001cf0: 205b 5b31 2e30 2c20 312e 302c 2031 2e30   [[1.0, 1.0, 1.0
+00001d00: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
+00001d10: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
+00001d20: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+00001d30: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
+00001d40: 2e30 2c20 312e 305d 5d2c 205b 5b31 2e30  .0, 1.0]], [[1.0
+00001d50: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+00001d60: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
+00001d70: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
+00001d80: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
+00001d90: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+00001da0: 305d 5d2c 205b 5b31 2e30 2c20 312e 302c  0]], [[1.0, 1.0,
+00001db0: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
+00001dc0: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+00001dd0: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
+00001de0: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
+00001df0: 302c 2031 2e30 2c20 312e 305d 5d2c 205b  0, 1.0, 1.0]], [
+00001e00: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+00001e10: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+00001e20: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
+00001e30: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+00001e40: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
+00001e50: 2c20 312e 305d 5d2c 205b 5b31 2e30 2c20  , 1.0]], [[1.0, 
+00001e60: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+00001e70: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+00001e80: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+00001e90: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
+00001ea0: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+00001eb0: 5d2c 205b 5b31 2e30 2c20 312e 302c 2031  ], [[1.0, 1.0, 1
+00001ec0: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
+00001ed0: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+00001ee0: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+00001ef0: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+00001f00: 2031 2e30 2c20 312e 305d 5d2c 205b 5b31   1.0, 1.0]], [[1
+00001f10: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+00001f20: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
+00001f30: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
+00001f40: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+00001f50: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+00001f60: 312e 305d 5d2c 205b 5b31 2e30 2c20 312e  1.0]], [[1.0, 1.
+00001f70: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
+00001f80: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+00001f90: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
+00001fa0: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
+00001fb0: 312e 302c 2031 2e30 2c20 312e 305d 5d2c  1.0, 1.0, 1.0]],
+00001fc0: 205b 5b31 2e30 2c20 312e 302c 2031 2e30   [[1.0, 1.0, 1.0
+00001fd0: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
+00001fe0: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
+00001ff0: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+00002000: 305d 2c20 5b31 2e30 2c20 312e 302c 2031  0], [1.0, 1.0, 1
+00002010: 2e30 2c20 312e 305d 5d2c 205b 5b31 2e30  .0, 1.0]], [[1.0
+00002020: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+00002030: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
+00002040: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
+00002050: 302c 2031 2e30 2c20 312e 305d 2c20 5b31  0, 1.0, 1.0], [1
+00002060: 2e30 2c20 312e 302c 2031 2e30 2c20 312e  .0, 1.0, 1.0, 1.
+00002070: 305d 5d2c 205b 5b31 2e30 2c20 312e 302c  0]], [[1.0, 1.0,
+00002080: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
+00002090: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+000020a0: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
+000020b0: 2c20 312e 305d 2c20 5b31 2e30 2c20 312e  , 1.0], [1.0, 1.
+000020c0: 302c 2031 2e30 2c20 312e 305d 5d2c 205b  0, 1.0, 1.0]], [
+000020d0: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+000020e0: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+000020f0: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
+00002100: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+00002110: 2c20 5b31 2e30 2c20 312e 302c 2031 2e30  , [1.0, 1.0, 1.0
+00002120: 2c20 312e 305d 5d2c 205b 5b31 2e30 2c20  , 1.0]], [[1.0, 
+00002130: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+00002140: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+00002150: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+00002160: 2031 2e30 2c20 312e 305d 2c20 5b31 2e30   1.0, 1.0], [1.0
+00002170: 2c20 312e 302c 2031 2e30 2c20 312e 305d  , 1.0, 1.0, 1.0]
+00002180: 5d2c 205b 5b31 2e30 2c20 312e 302c 2031  ], [[1.0, 1.0, 1
+00002190: 2e30 2c20 312e 305d 2c20 5b31 2e30 2c20  .0, 1.0], [1.0, 
+000021a0: 312e 302c 2031 2e30 2c20 312e 305d 2c20  1.0, 1.0, 1.0], 
+000021b0: 5b31 2e30 2c20 312e 302c 2031 2e30 2c20  [1.0, 1.0, 1.0, 
+000021c0: 312e 305d 2c20 5b31 2e30 2c20 312e 302c  1.0], [1.0, 1.0,
+000021d0: 2031 2e30 2c20 312e 305d 5d5d 220a 2020   1.0, 1.0]]]".  
+000021e0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+000021f0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00002200: 0a20 2020 2020 2020 2020 2020 2020 207b  .              {
+00002210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002220: 2022 6e61 6d65 223a 2022 645f 3022 2c0a   "name": "d_0",.
+00002230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002240: 2269 6f5f 6d6f 6465 223a 2022 696e 222c  "io_mode": "in",
+00002250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002260: 2022 6465 7363 223a 2022 222c 0a20 2020   "desc": "",.   
+00002270: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
+00002280: 7065 223a 2022 466c 6f61 7422 2c0a 2020  pe": "Float",.  
+00002290: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+000022a0: 6861 7065 223a 2022 2831 3034 2c29 222c  hape": "(104,)",
+000022b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000022c0: 2022 756e 6974 7322 3a20 6e75 6c6c 0a20   "units": null. 
+000022d0: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+000022e0: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
+000022f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002300: 226e 616d 6522 3a20 2264 5f31 222c 0a20  "name": "d_1",. 
+00002310: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002320: 696f 5f6d 6f64 6522 3a20 2269 6e22 2c0a  io_mode": "in",.
+00002330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002340: 2264 6573 6322 3a20 2222 2c0a 2020 2020  "desc": "",.    
+00002350: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00002360: 6522 3a20 2246 6c6f 6174 222c 0a20 2020  e": "Float",.   
+00002370: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
+00002380: 6170 6522 3a20 2228 3130 342c 2922 2c0a  ape": "(104,)",.
+00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023a0: 2275 6e69 7473 223a 206e 756c 6c0a 2020  "units": null.  
+000023b0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+000023c0: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+000023d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000023e0: 6e61 6d65 223a 2022 6469 7370 6c61 6365  name": "displace
+000023f0: 6d65 6e74 735f 3022 2c0a 2020 2020 2020  ments_0",.      
+00002400: 2020 2020 2020 2020 2020 2269 6f5f 6d6f            "io_mo
+00002410: 6465 223a 2022 696e 222c 0a20 2020 2020  de": "in",.     
+00002420: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+00002430: 223a 2022 222c 0a20 2020 2020 2020 2020  ": "",.         
+00002440: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+00002450: 466c 6f61 7422 2c0a 2020 2020 2020 2020  Float",.        
+00002460: 2020 2020 2020 2020 2273 6861 7065 223a          "shape":
+00002470: 2022 2831 3032 2c29 222c 0a20 2020 2020   "(102,)",.     
+00002480: 2020 2020 2020 2020 2020 2022 756e 6974             "unit
+00002490: 7322 3a20 6e75 6c6c 0a20 2020 2020 2020  s": null.       
+000024a0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+000024b0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+000024c0: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
+000024d0: 3a20 2264 6973 706c 6163 656d 656e 7473  : "displacements
+000024e0: 5f31 222c 0a20 2020 2020 2020 2020 2020  _1",.           
+000024f0: 2020 2020 2022 696f 5f6d 6f64 6522 3a20       "io_mode": 
+00002500: 2269 6e22 2c0a 2020 2020 2020 2020 2020  "in",.          
+00002510: 2020 2020 2020 2264 6573 6322 3a20 2222        "desc": ""
+00002520: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002530: 2020 2274 7970 6522 3a20 2246 6c6f 6174    "type": "Float
+00002540: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002550: 2020 2022 7368 6170 6522 3a20 2228 3130     "shape": "(10
+00002560: 322c 2922 2c0a 2020 2020 2020 2020 2020  2,)",.          
+00002570: 2020 2020 2020 2275 6e69 7473 223a 206e        "units": n
+00002580: 756c 6c0a 2020 2020 2020 2020 2020 2020  ull.            
+00002590: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+000025a0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+000025b0: 2020 2020 2022 6e61 6d65 223a 2022 636f       "name": "co
+000025c0: 6d70 6c69 616e 6365 5f30 222c 0a20 2020  mpliance_0",.   
+000025d0: 2020 2020 2020 2020 2020 2020 2022 696f               "io
+000025e0: 5f6d 6f64 6522 3a20 2269 6e22 2c0a 2020  _mode": "in",.  
+000025f0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00002600: 6573 6322 3a20 2222 2c0a 2020 2020 2020  esc": "",.      
+00002610: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+00002620: 3a20 2246 6c6f 6174 222c 0a20 2020 2020  : "Float",.     
+00002630: 2020 2020 2020 2020 2020 2022 7368 6170             "shap
+00002640: 6522 3a20 2231 222c 0a20 2020 2020 2020  e": "1",.       
+00002650: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
+00002660: 3a20 6e75 6c6c 0a20 2020 2020 2020 2020  : null.         
+00002670: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00002680: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00002690: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
+000026a0: 2263 6f6d 706c 6961 6e63 655f 3122 2c0a  "compliance_1",.
+000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026c0: 2269 6f5f 6d6f 6465 223a 2022 696e 222c  "io_mode": "in",
+000026d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000026e0: 2022 6465 7363 223a 2022 222c 0a20 2020   "desc": "",.   
+000026f0: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
+00002700: 7065 223a 2022 466c 6f61 7422 2c0a 2020  pe": "Float",.  
+00002710: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00002720: 6861 7065 223a 2022 3122 2c0a 2020 2020  hape": "1",.    
 00002730: 2020 2020 2020 2020 2020 2020 2275 6e69              "uni
-00002740: 7473 223a 206e 756c 6c0d 0a20 2020 2020  ts": null..     
-00002750: 2020 2020 2020 2020 207d 2c0d 0a20 2020           },..   
-00002760: 2020 2020 2020 2020 2020 207b 0d0a 2020             {..  
-00002770: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00002780: 616d 6522 3a20 2263 6f6d 706c 6961 6e63  ame": "complianc
-00002790: 655f 3122 2c0d 0a20 2020 2020 2020 2020  e_1",..         
-000027a0: 2020 2020 2020 2022 696f 5f6d 6f64 6522         "io_mode"
-000027b0: 3a20 2269 6e22 2c0d 0a20 2020 2020 2020  : "in",..       
-000027c0: 2020 2020 2020 2020 2022 6465 7363 223a           "desc":
-000027d0: 2022 222c 0d0a 2020 2020 2020 2020 2020   "",..          
-000027e0: 2020 2020 2020 2274 7970 6522 3a20 2246        "type": "F
-000027f0: 6c6f 6174 222c 0d0a 2020 2020 2020 2020  loat",..        
-00002800: 2020 2020 2020 2020 2273 6861 7065 223a          "shape":
-00002810: 2022 3122 2c0d 0a20 2020 2020 2020 2020   "1",..         
-00002820: 2020 2020 2020 2022 756e 6974 7322 3a20         "units": 
-00002830: 6e75 6c6c 0d0a 2020 2020 2020 2020 2020  null..          
-00002840: 2020 2020 7d0d 0a20 2020 2020 2020 2020      }..         
-00002850: 2020 205d 0d0a 2020 2020 2020 2020 2020     ]..          
-00002860: 7d2c 0d0a 2020 2020 2020 2020 2020 7b0d  },..          {.
-00002870: 0a20 2020 2020 2020 2020 2020 2022 6e61  .            "na
-00002880: 6d65 223a 2022 5375 6230 222c 0d0a 2020  me": "Sub0",..  
-00002890: 2020 2020 2020 2020 2020 2276 6172 6961            "varia
-000028a0: 626c 6573 5f61 7474 7269 6275 7465 7322  bles_attributes"
-000028b0: 3a20 5b0d 0a20 2020 2020 2020 2020 2020  : [..           
-000028c0: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-000028d0: 2020 2020 2020 226e 616d 6522 3a20 224b        "name": "K
-000028e0: 5f6c 6f63 616c 222c 0d0a 2020 2020 2020  _local",..      
-000028f0: 2020 2020 2020 2020 2020 2269 6f5f 6d6f            "io_mo
-00002900: 6465 223a 2022 696e 222c 0d0a 2020 2020  de": "in",..    
-00002910: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-00002920: 6522 3a20 2246 6c6f 6174 222c 0d0a 2020  e": "Float",..  
-00002930: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00002940: 6861 7065 223a 2022 2835 302c 2034 2c20  hape": "(50, 4, 
-00002950: 3429 222c 0d0a 2020 2020 2020 2020 2020  4)",..          
-00002960: 2020 2020 2020 2275 6e69 7473 223a 206e        "units": n
-00002970: 756c 6c2c 0d0a 2020 2020 2020 2020 2020  ull,..          
-00002980: 2020 2020 2020 2264 6573 6322 3a20 2222        "desc": ""
-00002990: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000029a0: 2020 2022 7061 7261 6d65 7465 725f 6174     "parameter_at
-000029b0: 7472 6962 7574 6573 223a 207b 0d0a 2020  tributes": {..  
-000029c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029d0: 2269 6e69 7422 3a20 225b 5b5b 312e 302c  "init": "[[[1.0,
-000029e0: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-000029f0: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-00002a00: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-00002a10: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
-00002a20: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00002a30: 5d5d 2c20 5b5b 312e 302c 2031 2e30 2c20  ]], [[1.0, 1.0, 
-00002a40: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
-00002a50: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-00002a60: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-00002a70: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-00002a80: 2c20 312e 302c 2031 2e30 5d5d 2c20 5b5b  , 1.0, 1.0]], [[
-00002a90: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00002aa0: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
-00002ab0: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
-00002ac0: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-00002ad0: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-00002ae0: 2031 2e30 5d5d 2c20 5b5b 312e 302c 2031   1.0]], [[1.0, 1
-00002af0: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
-00002b00: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00002b10: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
-00002b20: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
-00002b30: 2031 2e30 2c20 312e 302c 2031 2e30 5d5d   1.0, 1.0, 1.0]]
-00002b40: 2c20 5b5b 312e 302c 2031 2e30 2c20 312e  , [[1.0, 1.0, 1.
-00002b50: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
-00002b60: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
-00002b70: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00002b80: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
-00002b90: 312e 302c 2031 2e30 5d5d 2c20 5b5b 312e  1.0, 1.0]], [[1.
-00002ba0: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00002bb0: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
-00002bc0: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
-00002bd0: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
-00002be0: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00002bf0: 2e30 5d5d 2c20 5b5b 312e 302c 2031 2e30  .0]], [[1.0, 1.0
-00002c00: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
-00002c10: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00002c20: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
-00002c30: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
-00002c40: 2e30 2c20 312e 302c 2031 2e30 5d5d 2c20  .0, 1.0, 1.0]], 
-00002c50: 5b5b 312e 302c 2031 2e30 2c20 312e 302c  [[1.0, 1.0, 1.0,
-00002c60: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-00002c70: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
-00002c80: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00002c90: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
-00002ca0: 302c 2031 2e30 5d5d 2c20 5b5b 312e 302c  0, 1.0]], [[1.0,
-00002cb0: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-00002cc0: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-00002cd0: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-00002ce0: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
-00002cf0: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00002d00: 5d5d 2c20 5b5b 312e 302c 2031 2e30 2c20  ]], [[1.0, 1.0, 
-00002d10: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
-00002d20: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-00002d30: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-00002d40: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-00002d50: 2c20 312e 302c 2031 2e30 5d5d 2c20 5b5b  , 1.0, 1.0]], [[
-00002d60: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00002d70: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
-00002d80: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
-00002d90: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-00002da0: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-00002db0: 2031 2e30 5d5d 2c20 5b5b 312e 302c 2031   1.0]], [[1.0, 1
-00002dc0: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
-00002dd0: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00002de0: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
-00002df0: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
-00002e00: 2031 2e30 2c20 312e 302c 2031 2e30 5d5d   1.0, 1.0, 1.0]]
-00002e10: 2c20 5b5b 312e 302c 2031 2e30 2c20 312e  , [[1.0, 1.0, 1.
-00002e20: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
-00002e30: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
-00002e40: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00002e50: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
-00002e60: 312e 302c 2031 2e30 5d5d 2c20 5b5b 312e  1.0, 1.0]], [[1.
-00002e70: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00002e80: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
-00002e90: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
-00002ea0: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
-00002eb0: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00002ec0: 2e30 5d5d 2c20 5b5b 312e 302c 2031 2e30  .0]], [[1.0, 1.0
-00002ed0: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
-00002ee0: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00002ef0: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
-00002f00: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
-00002f10: 2e30 2c20 312e 302c 2031 2e30 5d5d 2c20  .0, 1.0, 1.0]], 
-00002f20: 5b5b 312e 302c 2031 2e30 2c20 312e 302c  [[1.0, 1.0, 1.0,
-00002f30: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-00002f40: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
-00002f50: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00002f60: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
-00002f70: 302c 2031 2e30 5d5d 2c20 5b5b 312e 302c  0, 1.0]], [[1.0,
-00002f80: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-00002f90: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-00002fa0: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-00002fb0: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
-00002fc0: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00002fd0: 5d5d 2c20 5b5b 312e 302c 2031 2e30 2c20  ]], [[1.0, 1.0, 
-00002fe0: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
-00002ff0: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-00003000: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-00003010: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-00003020: 2c20 312e 302c 2031 2e30 5d5d 2c20 5b5b  , 1.0, 1.0]], [[
-00003030: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00003040: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
-00003050: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
-00003060: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-00003070: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-00003080: 2031 2e30 5d5d 2c20 5b5b 312e 302c 2031   1.0]], [[1.0, 1
-00003090: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
-000030a0: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-000030b0: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
-000030c0: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
-000030d0: 2031 2e30 2c20 312e 302c 2031 2e30 5d5d   1.0, 1.0, 1.0]]
-000030e0: 2c20 5b5b 312e 302c 2031 2e30 2c20 312e  , [[1.0, 1.0, 1.
-000030f0: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
-00003100: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
-00003110: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00003120: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
-00003130: 312e 302c 2031 2e30 5d5d 2c20 5b5b 312e  1.0, 1.0]], [[1.
-00003140: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00003150: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
-00003160: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
-00003170: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
-00003180: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00003190: 2e30 5d5d 2c20 5b5b 312e 302c 2031 2e30  .0]], [[1.0, 1.0
-000031a0: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
-000031b0: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-000031c0: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
-000031d0: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
-000031e0: 2e30 2c20 312e 302c 2031 2e30 5d5d 2c20  .0, 1.0, 1.0]], 
-000031f0: 5b5b 312e 302c 2031 2e30 2c20 312e 302c  [[1.0, 1.0, 1.0,
-00003200: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-00003210: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
-00003220: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00003230: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
-00003240: 302c 2031 2e30 5d5d 2c20 5b5b 312e 302c  0, 1.0]], [[1.0,
-00003250: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-00003260: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-00003270: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-00003280: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
-00003290: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-000032a0: 5d5d 2c20 5b5b 312e 302c 2031 2e30 2c20  ]], [[1.0, 1.0, 
-000032b0: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
-000032c0: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-000032d0: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-000032e0: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-000032f0: 2c20 312e 302c 2031 2e30 5d5d 2c20 5b5b  , 1.0, 1.0]], [[
-00003300: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00003310: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
-00003320: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
-00003330: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-00003340: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-00003350: 2031 2e30 5d5d 2c20 5b5b 312e 302c 2031   1.0]], [[1.0, 1
-00003360: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
-00003370: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00003380: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
-00003390: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
-000033a0: 2031 2e30 2c20 312e 302c 2031 2e30 5d5d   1.0, 1.0, 1.0]]
-000033b0: 2c20 5b5b 312e 302c 2031 2e30 2c20 312e  , [[1.0, 1.0, 1.
-000033c0: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
-000033d0: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
-000033e0: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-000033f0: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
-00003400: 312e 302c 2031 2e30 5d5d 2c20 5b5b 312e  1.0, 1.0]], [[1.
-00003410: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00003420: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
-00003430: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
-00003440: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
-00003450: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00003460: 2e30 5d5d 2c20 5b5b 312e 302c 2031 2e30  .0]], [[1.0, 1.0
-00003470: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
-00003480: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00003490: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
-000034a0: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
-000034b0: 2e30 2c20 312e 302c 2031 2e30 5d5d 2c20  .0, 1.0, 1.0]], 
-000034c0: 5b5b 312e 302c 2031 2e30 2c20 312e 302c  [[1.0, 1.0, 1.0,
-000034d0: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-000034e0: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
-000034f0: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00003500: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
-00003510: 302c 2031 2e30 5d5d 2c20 5b5b 312e 302c  0, 1.0]], [[1.0,
-00003520: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-00003530: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-00003540: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-00003550: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
-00003560: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00003570: 5d5d 2c20 5b5b 312e 302c 2031 2e30 2c20  ]], [[1.0, 1.0, 
-00003580: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
-00003590: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-000035a0: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-000035b0: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-000035c0: 2c20 312e 302c 2031 2e30 5d5d 2c20 5b5b  , 1.0, 1.0]], [[
-000035d0: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-000035e0: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
-000035f0: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
-00003600: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-00003610: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-00003620: 2031 2e30 5d5d 2c20 5b5b 312e 302c 2031   1.0]], [[1.0, 1
-00003630: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
-00003640: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00003650: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
-00003660: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
-00003670: 2031 2e30 2c20 312e 302c 2031 2e30 5d5d   1.0, 1.0, 1.0]]
-00003680: 2c20 5b5b 312e 302c 2031 2e30 2c20 312e  , [[1.0, 1.0, 1.
-00003690: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
-000036a0: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
-000036b0: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-000036c0: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
-000036d0: 312e 302c 2031 2e30 5d5d 2c20 5b5b 312e  1.0, 1.0]], [[1.
-000036e0: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-000036f0: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
-00003700: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
-00003710: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
-00003720: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00003730: 2e30 5d5d 2c20 5b5b 312e 302c 2031 2e30  .0]], [[1.0, 1.0
-00003740: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
-00003750: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00003760: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
-00003770: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
-00003780: 2e30 2c20 312e 302c 2031 2e30 5d5d 2c20  .0, 1.0, 1.0]], 
-00003790: 5b5b 312e 302c 2031 2e30 2c20 312e 302c  [[1.0, 1.0, 1.0,
-000037a0: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-000037b0: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
-000037c0: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-000037d0: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
-000037e0: 302c 2031 2e30 5d5d 2c20 5b5b 312e 302c  0, 1.0]], [[1.0,
-000037f0: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-00003800: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-00003810: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-00003820: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
-00003830: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00003840: 5d5d 2c20 5b5b 312e 302c 2031 2e30 2c20  ]], [[1.0, 1.0, 
-00003850: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
-00003860: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-00003870: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-00003880: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-00003890: 2c20 312e 302c 2031 2e30 5d5d 2c20 5b5b  , 1.0, 1.0]], [[
-000038a0: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-000038b0: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
-000038c0: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
-000038d0: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-000038e0: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-000038f0: 2031 2e30 5d5d 2c20 5b5b 312e 302c 2031   1.0]], [[1.0, 1
-00003900: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
-00003910: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00003920: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
-00003930: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
-00003940: 2031 2e30 2c20 312e 302c 2031 2e30 5d5d   1.0, 1.0, 1.0]]
-00003950: 2c20 5b5b 312e 302c 2031 2e30 2c20 312e  , [[1.0, 1.0, 1.
-00003960: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
-00003970: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
-00003980: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00003990: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
-000039a0: 312e 302c 2031 2e30 5d5d 2c20 5b5b 312e  1.0, 1.0]], [[1.
-000039b0: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-000039c0: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
-000039d0: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
-000039e0: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
-000039f0: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
-00003a00: 2e30 5d5d 2c20 5b5b 312e 302c 2031 2e30  .0]], [[1.0, 1.0
-00003a10: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
-00003a20: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00003a30: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
-00003a40: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
-00003a50: 2e30 2c20 312e 302c 2031 2e30 5d5d 2c20  .0, 1.0, 1.0]], 
-00003a60: 5b5b 312e 302c 2031 2e30 2c20 312e 302c  [[1.0, 1.0, 1.0,
-00003a70: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-00003a80: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
-00003a90: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00003aa0: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
-00003ab0: 302c 2031 2e30 5d5d 2c20 5b5b 312e 302c  0, 1.0]], [[1.0,
-00003ac0: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-00003ad0: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-00003ae0: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-00003af0: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
-00003b00: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
-00003b10: 5d5d 2c20 5b5b 312e 302c 2031 2e30 2c20  ]], [[1.0, 1.0, 
-00003b20: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
-00003b30: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
-00003b40: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
-00003b50: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
-00003b60: 2c20 312e 302c 2031 2e30 5d5d 5d22 0d0a  , 1.0, 1.0]]]"..
-00003b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b80: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
-00003b90: 207d 2c0d 0a20 2020 2020 2020 2020 2020   },..           
-00003ba0: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-00003bb0: 2020 2020 2020 226e 616d 6522 3a20 2263        "name": "c
-00003bc0: 6f6d 706c 6961 6e63 655f 3022 2c0d 0a20  ompliance_0",.. 
-00003bd0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003be0: 696f 5f6d 6f64 6522 3a20 226f 7574 222c  io_mode": "out",
-00003bf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003c00: 2020 2274 7970 6522 3a20 2246 6c6f 6174    "type": "Float
-00003c10: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00003c20: 2020 2020 2273 6861 7065 223a 2022 3122      "shape": "1"
-00003c30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003c40: 2020 2022 756e 6974 7322 3a20 6e75 6c6c     "units": null
-00003c50: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003c60: 2020 2022 6465 7363 223a 2022 220d 0a20     "desc": "".. 
-00003c70: 2020 2020 2020 2020 2020 2020 207d 2c0d               },.
-00003c80: 0a20 2020 2020 2020 2020 2020 2020 207b  .              {
-00003c90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003ca0: 2020 226e 616d 6522 3a20 2263 6f6d 706c    "name": "compl
-00003cb0: 6961 6e63 655f 3122 2c0d 0a20 2020 2020  iance_1",..     
-00003cc0: 2020 2020 2020 2020 2020 2022 696f 5f6d             "io_m
-00003cd0: 6f64 6522 3a20 226f 7574 222c 0d0a 2020  ode": "out",..  
-00003ce0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00003cf0: 7970 6522 3a20 2246 6c6f 6174 222c 0d0a  ype": "Float",..
-00003d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d10: 2273 6861 7065 223a 2022 3122 2c0d 0a20  "shape": "1",.. 
-00003d20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003d30: 756e 6974 7322 3a20 6e75 6c6c 2c0d 0a20  units": null,.. 
-00003d40: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003d50: 6465 7363 223a 2022 220d 0a20 2020 2020  desc": ""..     
-00003d60: 2020 2020 2020 2020 207d 2c0d 0a20 2020           },..   
-00003d70: 2020 2020 2020 2020 2020 207b 0d0a 2020             {..  
-00003d80: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00003d90: 616d 6522 3a20 2264 5f30 222c 0d0a 2020  ame": "d_0",..  
-00003da0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-00003db0: 6f5f 6d6f 6465 223a 2022 6f75 7422 2c0d  o_mode": "out",.
-00003dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003dd0: 2022 6465 7363 223a 2022 222c 0d0a 2020   "desc": "",..  
-00003de0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00003df0: 7970 6522 3a20 2246 6c6f 6174 222c 0d0a  ype": "Float",..
-00003e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e10: 2273 6861 7065 223a 2022 2831 3034 2c29  "shape": "(104,)
-00003e20: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00003e30: 2020 2020 2275 6e69 7473 223a 206e 756c      "units": nul
-00003e40: 6c0d 0a20 2020 2020 2020 2020 2020 2020  l..             
-00003e50: 207d 2c0d 0a20 2020 2020 2020 2020 2020   },..           
-00003e60: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-00003e70: 2020 2020 2020 226e 616d 6522 3a20 2264        "name": "d
-00003e80: 5f31 222c 0d0a 2020 2020 2020 2020 2020  _1",..          
-00003e90: 2020 2020 2020 2269 6f5f 6d6f 6465 223a        "io_mode":
-00003ea0: 2022 6f75 7422 2c0d 0a20 2020 2020 2020   "out",..       
-00003eb0: 2020 2020 2020 2020 2022 6465 7363 223a           "desc":
-00003ec0: 2022 222c 0d0a 2020 2020 2020 2020 2020   "",..          
-00003ed0: 2020 2020 2020 2274 7970 6522 3a20 2246        "type": "F
-00003ee0: 6c6f 6174 222c 0d0a 2020 2020 2020 2020  loat",..        
-00003ef0: 2020 2020 2020 2020 2273 6861 7065 223a          "shape":
-00003f00: 2022 2831 3034 2c29 222c 0d0a 2020 2020   "(104,)",..    
-00003f10: 2020 2020 2020 2020 2020 2020 2275 6e69              "uni
-00003f20: 7473 223a 206e 756c 6c0d 0a20 2020 2020  ts": null..     
-00003f30: 2020 2020 2020 2020 207d 2c0d 0a20 2020           },..   
-00003f40: 2020 2020 2020 2020 2020 207b 0d0a 2020             {..  
-00003f50: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00003f60: 616d 6522 3a20 2264 6973 706c 6163 656d  ame": "displacem
-00003f70: 656e 7473 5f30 222c 0d0a 2020 2020 2020  ents_0",..      
-00003f80: 2020 2020 2020 2020 2020 2269 6f5f 6d6f            "io_mo
-00003f90: 6465 223a 2022 6f75 7422 2c0d 0a20 2020  de": "out",..   
-00003fa0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00003fb0: 7363 223a 2022 222c 0d0a 2020 2020 2020  sc": "",..      
-00003fc0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00003fd0: 3a20 2246 6c6f 6174 222c 0d0a 2020 2020  : "Float",..    
-00003fe0: 2020 2020 2020 2020 2020 2020 2273 6861              "sha
-00003ff0: 7065 223a 2022 2831 3032 2c29 222c 0d0a  pe": "(102,)",..
-00004000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004010: 2275 6e69 7473 223a 206e 756c 6c0d 0a20  "units": null.. 
-00004020: 2020 2020 2020 2020 2020 2020 207d 2c0d               },.
-00004030: 0a20 2020 2020 2020 2020 2020 2020 207b  .              {
-00004040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004050: 2020 226e 616d 6522 3a20 2264 6973 706c    "name": "displ
-00004060: 6163 656d 656e 7473 5f31 222c 0d0a 2020  acements_1",..  
-00004070: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-00004080: 6f5f 6d6f 6465 223a 2022 6f75 7422 2c0d  o_mode": "out",.
-00004090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000040a0: 2022 6465 7363 223a 2022 222c 0d0a 2020   "desc": "",..  
-000040b0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-000040c0: 7970 6522 3a20 2246 6c6f 6174 222c 0d0a  ype": "Float",..
-000040d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040e0: 2273 6861 7065 223a 2022 2831 3032 2c29  "shape": "(102,)
-000040f0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00004100: 2020 2020 2275 6e69 7473 223a 206e 756c      "units": nul
-00004110: 6c0d 0a20 2020 2020 2020 2020 2020 2020  l..             
-00004120: 207d 0d0a 2020 2020 2020 2020 2020 2020   }..            
-00004130: 5d0d 0a20 2020 2020 2020 2020 207d 0d0a  ]..          }..
-00004140: 2020 2020 2020 2020 5d0d 0a20 2020 2020          ]..     
-00004150: 207d 0d0a 2020 2020 7d2c 0d0a 2020 2020   }..    },..    
-00004160: 7b0d 0a20 2020 2020 2022 6e61 6d65 223a  {..      "name":
-00004170: 2022 566f 6c75 6d65 436f 6d70 222c 0d0a   "VolumeComp",..
-00004180: 2020 2020 2020 2276 6172 6961 626c 6573        "variables
-00004190: 5f61 7474 7269 6275 7465 7322 3a20 5b0d  _attributes": [.
-000041a0: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
-000041b0: 2020 2020 2020 226e 616d 6522 3a20 2268        "name": "h
-000041c0: 222c 0d0a 2020 2020 2020 2020 2020 2269  ",..          "i
-000041d0: 6f5f 6d6f 6465 223a 2022 696e 222c 0d0a  o_mode": "in",..
-000041e0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-000041f0: 3a20 2246 6c6f 6174 222c 0d0a 2020 2020  : "Float",..    
-00004200: 2020 2020 2020 2273 6861 7065 223a 2022        "shape": "
-00004210: 2831 2c20 3530 2922 2c0d 0a20 2020 2020  (1, 50)",..     
-00004220: 2020 2020 2022 756e 6974 7322 3a20 6e75       "units": nu
-00004230: 6c6c 2c0d 0a20 2020 2020 2020 2020 2022  ll,..          "
-00004240: 6465 7363 223a 2022 220d 0a20 2020 2020  desc": ""..     
-00004250: 2020 207d 2c0d 0a20 2020 2020 2020 207b     },..        {
-00004260: 0d0a 2020 2020 2020 2020 2020 226e 616d  ..          "nam
-00004270: 6522 3a20 2276 6f6c 756d 6522 2c0d 0a20  e": "volume",.. 
-00004280: 2020 2020 2020 2020 2022 696f 5f6d 6f64           "io_mod
-00004290: 6522 3a20 226f 7574 222c 0d0a 2020 2020  e": "out",..    
-000042a0: 2020 2020 2020 2264 6573 6322 3a20 2222        "desc": ""
-000042b0: 2c0d 0a20 2020 2020 2020 2020 2022 7479  ,..          "ty
-000042c0: 7065 223a 2022 466c 6f61 7422 2c0d 0a20  pe": "Float",.. 
-000042d0: 2020 2020 2020 2020 2022 7368 6170 6522           "shape"
-000042e0: 3a20 2231 222c 0d0a 2020 2020 2020 2020  : "1",..        
-000042f0: 2020 2275 6e69 7473 223a 206e 756c 6c0d    "units": null.
-00004300: 0a20 2020 2020 2020 207d 0d0a 2020 2020  .        }..    
-00004310: 2020 5d0d 0a20 2020 207d 2c0d 0a20 2020    ]..    },..   
-00004320: 207b 0d0a 2020 2020 2020 226e 616d 6522   {..      "name"
-00004330: 3a20 224f 626a 5375 6d22 2c0d 0a20 2020  : "ObjSum",..   
-00004340: 2020 2022 7661 7269 6162 6c65 735f 6174     "variables_at
-00004350: 7472 6962 7574 6573 223a 205b 0d0a 2020  tributes": [..  
-00004360: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-00004370: 2020 2022 6e61 6d65 223a 2022 636f 6d70     "name": "comp
-00004380: 6c69 616e 6365 5f30 222c 0d0a 2020 2020  liance_0",..    
-00004390: 2020 2020 2020 2269 6f5f 6d6f 6465 223a        "io_mode":
-000043a0: 2022 696e 222c 0d0a 2020 2020 2020 2020   "in",..        
-000043b0: 2020 2274 7970 6522 3a20 2246 6c6f 6174    "type": "Float
-000043c0: 222c 0d0a 2020 2020 2020 2020 2020 2273  ",..          "s
-000043d0: 6861 7065 223a 2022 3122 2c0d 0a20 2020  hape": "1",..   
-000043e0: 2020 2020 2020 2022 756e 6974 7322 3a20         "units": 
-000043f0: 6e75 6c6c 2c0d 0a20 2020 2020 2020 2020  null,..         
-00004400: 2022 6465 7363 223a 2022 220d 0a20 2020   "desc": ""..   
-00004410: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-00004420: 207b 0d0a 2020 2020 2020 2020 2020 226e   {..          "n
-00004430: 616d 6522 3a20 2263 6f6d 706c 6961 6e63  ame": "complianc
-00004440: 655f 3122 2c0d 0a20 2020 2020 2020 2020  e_1",..         
-00004450: 2022 696f 5f6d 6f64 6522 3a20 2269 6e22   "io_mode": "in"
-00004460: 2c0d 0a20 2020 2020 2020 2020 2022 7479  ,..          "ty
-00004470: 7065 223a 2022 466c 6f61 7422 2c0d 0a20  pe": "Float",.. 
-00004480: 2020 2020 2020 2020 2022 7368 6170 6522           "shape"
-00004490: 3a20 2231 222c 0d0a 2020 2020 2020 2020  : "1",..        
-000044a0: 2020 2275 6e69 7473 223a 206e 756c 6c2c    "units": null,
-000044b0: 0d0a 2020 2020 2020 2020 2020 2264 6573  ..          "des
-000044c0: 6322 3a20 2222 0d0a 2020 2020 2020 2020  c": ""..        
-000044d0: 7d2c 0d0a 2020 2020 2020 2020 7b0d 0a20  },..        {.. 
-000044e0: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
-000044f0: 2022 6f62 6a22 2c0d 0a20 2020 2020 2020   "obj",..       
-00004500: 2020 2022 696f 5f6d 6f64 6522 3a20 226f     "io_mode": "o
-00004510: 7574 222c 0d0a 2020 2020 2020 2020 2020  ut",..          
-00004520: 2264 6573 6322 3a20 2222 2c0d 0a20 2020  "desc": "",..   
-00004530: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00004540: 466c 6f61 7422 2c0d 0a20 2020 2020 2020  Float",..       
-00004550: 2020 2022 7368 6170 6522 3a20 2231 222c     "shape": "1",
-00004560: 0d0a 2020 2020 2020 2020 2020 2275 6e69  ..          "uni
-00004570: 7473 223a 206e 756c 6c0d 0a20 2020 2020  ts": null..     
-00004580: 2020 207d 0d0a 2020 2020 2020 5d0d 0a20     }..      ].. 
-00004590: 2020 207d 0d0a 2020 5d0d 0a7d               }..  ]..}
+00002740: 7473 223a 206e 756c 6c0a 2020 2020 2020  ts": null.      
+00002750: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00002760: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+00002770: 2020 7d2c 0a20 2020 2020 2020 2020 207b    },.          {
+00002780: 0a20 2020 2020 2020 2020 2020 2022 6e61  .            "na
+00002790: 6d65 223a 2022 5375 6230 222c 0a20 2020  me": "Sub0",.   
+000027a0: 2020 2020 2020 2020 2022 7661 7269 6162           "variab
+000027b0: 6c65 735f 6174 7472 6962 7574 6573 223a  les_attributes":
+000027c0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+000027d0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+000027e0: 2020 2022 6e61 6d65 223a 2022 4b5f 6c6f     "name": "K_lo
+000027f0: 6361 6c22 2c0a 2020 2020 2020 2020 2020  cal",.          
+00002800: 2020 2020 2020 2269 6f5f 6d6f 6465 223a        "io_mode":
+00002810: 2022 696e 222c 0a20 2020 2020 2020 2020   "in",.         
+00002820: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+00002830: 466c 6f61 7422 2c0a 2020 2020 2020 2020  Float",.        
+00002840: 2020 2020 2020 2020 2273 6861 7065 223a          "shape":
+00002850: 2022 2835 302c 2034 2c20 3429 222c 0a20   "(50, 4, 4)",. 
+00002860: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002870: 756e 6974 7322 3a20 6e75 6c6c 2c0a 2020  units": null,.  
+00002880: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00002890: 6573 6322 3a20 2222 2c0a 2020 2020 2020  esc": "",.      
+000028a0: 2020 2020 2020 2020 2020 2270 6172 616d            "param
+000028b0: 6574 6572 5f61 7474 7269 6275 7465 7322  eter_attributes"
+000028c0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000028d0: 2020 2020 2020 2269 6e69 7422 3a20 225b        "init": "[
+000028e0: 5b5b 312e 302c 2031 2e30 2c20 312e 302c  [[1.0, 1.0, 1.0,
+000028f0: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+00002900: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+00002910: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00002920: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
+00002930: 302c 2031 2e30 5d5d 2c20 5b5b 312e 302c  0, 1.0]], [[1.0,
+00002940: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
+00002950: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
+00002960: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+00002970: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+00002980: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00002990: 5d5d 2c20 5b5b 312e 302c 2031 2e30 2c20  ]], [[1.0, 1.0, 
+000029a0: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
+000029b0: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
+000029c0: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
+000029d0: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+000029e0: 2c20 312e 302c 2031 2e30 5d5d 2c20 5b5b  , 1.0, 1.0]], [[
+000029f0: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+00002a00: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
+00002a10: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
+00002a20: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
+00002a30: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
+00002a40: 2031 2e30 5d5d 2c20 5b5b 312e 302c 2031   1.0]], [[1.0, 1
+00002a50: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
+00002a60: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+00002a70: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
+00002a80: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
+00002a90: 2031 2e30 2c20 312e 302c 2031 2e30 5d5d   1.0, 1.0, 1.0]]
+00002aa0: 2c20 5b5b 312e 302c 2031 2e30 2c20 312e  , [[1.0, 1.0, 1.
+00002ab0: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
+00002ac0: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
+00002ad0: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+00002ae0: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
+00002af0: 312e 302c 2031 2e30 5d5d 2c20 5b5b 312e  1.0, 1.0]], [[1.
+00002b00: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00002b10: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
+00002b20: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
+00002b30: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
+00002b40: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+00002b50: 2e30 5d5d 2c20 5b5b 312e 302c 2031 2e30  .0]], [[1.0, 1.0
+00002b60: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+00002b70: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00002b80: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
+00002b90: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
+00002ba0: 2e30 2c20 312e 302c 2031 2e30 5d5d 2c20  .0, 1.0, 1.0]], 
+00002bb0: 5b5b 312e 302c 2031 2e30 2c20 312e 302c  [[1.0, 1.0, 1.0,
+00002bc0: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+00002bd0: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+00002be0: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00002bf0: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
+00002c00: 302c 2031 2e30 5d5d 2c20 5b5b 312e 302c  0, 1.0]], [[1.0,
+00002c10: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
+00002c20: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
+00002c30: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+00002c40: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+00002c50: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00002c60: 5d5d 2c20 5b5b 312e 302c 2031 2e30 2c20  ]], [[1.0, 1.0, 
+00002c70: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
+00002c80: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
+00002c90: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
+00002ca0: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+00002cb0: 2c20 312e 302c 2031 2e30 5d5d 2c20 5b5b  , 1.0, 1.0]], [[
+00002cc0: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+00002cd0: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
+00002ce0: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
+00002cf0: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
+00002d00: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
+00002d10: 2031 2e30 5d5d 2c20 5b5b 312e 302c 2031   1.0]], [[1.0, 1
+00002d20: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
+00002d30: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+00002d40: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
+00002d50: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
+00002d60: 2031 2e30 2c20 312e 302c 2031 2e30 5d5d   1.0, 1.0, 1.0]]
+00002d70: 2c20 5b5b 312e 302c 2031 2e30 2c20 312e  , [[1.0, 1.0, 1.
+00002d80: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
+00002d90: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
+00002da0: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+00002db0: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
+00002dc0: 312e 302c 2031 2e30 5d5d 2c20 5b5b 312e  1.0, 1.0]], [[1.
+00002dd0: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00002de0: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
+00002df0: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
+00002e00: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
+00002e10: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+00002e20: 2e30 5d5d 2c20 5b5b 312e 302c 2031 2e30  .0]], [[1.0, 1.0
+00002e30: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+00002e40: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00002e50: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
+00002e60: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
+00002e70: 2e30 2c20 312e 302c 2031 2e30 5d5d 2c20  .0, 1.0, 1.0]], 
+00002e80: 5b5b 312e 302c 2031 2e30 2c20 312e 302c  [[1.0, 1.0, 1.0,
+00002e90: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+00002ea0: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+00002eb0: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00002ec0: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
+00002ed0: 302c 2031 2e30 5d5d 2c20 5b5b 312e 302c  0, 1.0]], [[1.0,
+00002ee0: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
+00002ef0: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
+00002f00: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+00002f10: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+00002f20: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00002f30: 5d5d 2c20 5b5b 312e 302c 2031 2e30 2c20  ]], [[1.0, 1.0, 
+00002f40: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
+00002f50: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
+00002f60: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
+00002f70: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+00002f80: 2c20 312e 302c 2031 2e30 5d5d 2c20 5b5b  , 1.0, 1.0]], [[
+00002f90: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+00002fa0: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
+00002fb0: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
+00002fc0: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
+00002fd0: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
+00002fe0: 2031 2e30 5d5d 2c20 5b5b 312e 302c 2031   1.0]], [[1.0, 1
+00002ff0: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
+00003000: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+00003010: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
+00003020: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
+00003030: 2031 2e30 2c20 312e 302c 2031 2e30 5d5d   1.0, 1.0, 1.0]]
+00003040: 2c20 5b5b 312e 302c 2031 2e30 2c20 312e  , [[1.0, 1.0, 1.
+00003050: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
+00003060: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
+00003070: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+00003080: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
+00003090: 312e 302c 2031 2e30 5d5d 2c20 5b5b 312e  1.0, 1.0]], [[1.
+000030a0: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+000030b0: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
+000030c0: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
+000030d0: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
+000030e0: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+000030f0: 2e30 5d5d 2c20 5b5b 312e 302c 2031 2e30  .0]], [[1.0, 1.0
+00003100: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+00003110: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00003120: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
+00003130: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
+00003140: 2e30 2c20 312e 302c 2031 2e30 5d5d 2c20  .0, 1.0, 1.0]], 
+00003150: 5b5b 312e 302c 2031 2e30 2c20 312e 302c  [[1.0, 1.0, 1.0,
+00003160: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+00003170: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+00003180: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00003190: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
+000031a0: 302c 2031 2e30 5d5d 2c20 5b5b 312e 302c  0, 1.0]], [[1.0,
+000031b0: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
+000031c0: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
+000031d0: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+000031e0: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+000031f0: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00003200: 5d5d 2c20 5b5b 312e 302c 2031 2e30 2c20  ]], [[1.0, 1.0, 
+00003210: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
+00003220: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
+00003230: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
+00003240: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+00003250: 2c20 312e 302c 2031 2e30 5d5d 2c20 5b5b  , 1.0, 1.0]], [[
+00003260: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+00003270: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
+00003280: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
+00003290: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
+000032a0: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
+000032b0: 2031 2e30 5d5d 2c20 5b5b 312e 302c 2031   1.0]], [[1.0, 1
+000032c0: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
+000032d0: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+000032e0: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
+000032f0: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
+00003300: 2031 2e30 2c20 312e 302c 2031 2e30 5d5d   1.0, 1.0, 1.0]]
+00003310: 2c20 5b5b 312e 302c 2031 2e30 2c20 312e  , [[1.0, 1.0, 1.
+00003320: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
+00003330: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
+00003340: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+00003350: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
+00003360: 312e 302c 2031 2e30 5d5d 2c20 5b5b 312e  1.0, 1.0]], [[1.
+00003370: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00003380: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
+00003390: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
+000033a0: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
+000033b0: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+000033c0: 2e30 5d5d 2c20 5b5b 312e 302c 2031 2e30  .0]], [[1.0, 1.0
+000033d0: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+000033e0: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+000033f0: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
+00003400: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
+00003410: 2e30 2c20 312e 302c 2031 2e30 5d5d 2c20  .0, 1.0, 1.0]], 
+00003420: 5b5b 312e 302c 2031 2e30 2c20 312e 302c  [[1.0, 1.0, 1.0,
+00003430: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+00003440: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+00003450: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00003460: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
+00003470: 302c 2031 2e30 5d5d 2c20 5b5b 312e 302c  0, 1.0]], [[1.0,
+00003480: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
+00003490: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
+000034a0: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+000034b0: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+000034c0: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+000034d0: 5d5d 2c20 5b5b 312e 302c 2031 2e30 2c20  ]], [[1.0, 1.0, 
+000034e0: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
+000034f0: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
+00003500: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
+00003510: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+00003520: 2c20 312e 302c 2031 2e30 5d5d 2c20 5b5b  , 1.0, 1.0]], [[
+00003530: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+00003540: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
+00003550: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
+00003560: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
+00003570: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
+00003580: 2031 2e30 5d5d 2c20 5b5b 312e 302c 2031   1.0]], [[1.0, 1
+00003590: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
+000035a0: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+000035b0: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
+000035c0: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
+000035d0: 2031 2e30 2c20 312e 302c 2031 2e30 5d5d   1.0, 1.0, 1.0]]
+000035e0: 2c20 5b5b 312e 302c 2031 2e30 2c20 312e  , [[1.0, 1.0, 1.
+000035f0: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
+00003600: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
+00003610: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+00003620: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
+00003630: 312e 302c 2031 2e30 5d5d 2c20 5b5b 312e  1.0, 1.0]], [[1.
+00003640: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00003650: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
+00003660: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
+00003670: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
+00003680: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+00003690: 2e30 5d5d 2c20 5b5b 312e 302c 2031 2e30  .0]], [[1.0, 1.0
+000036a0: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+000036b0: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+000036c0: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
+000036d0: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
+000036e0: 2e30 2c20 312e 302c 2031 2e30 5d5d 2c20  .0, 1.0, 1.0]], 
+000036f0: 5b5b 312e 302c 2031 2e30 2c20 312e 302c  [[1.0, 1.0, 1.0,
+00003700: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+00003710: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+00003720: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00003730: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
+00003740: 302c 2031 2e30 5d5d 2c20 5b5b 312e 302c  0, 1.0]], [[1.0,
+00003750: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
+00003760: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
+00003770: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+00003780: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+00003790: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+000037a0: 5d5d 2c20 5b5b 312e 302c 2031 2e30 2c20  ]], [[1.0, 1.0, 
+000037b0: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
+000037c0: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
+000037d0: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
+000037e0: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+000037f0: 2c20 312e 302c 2031 2e30 5d5d 2c20 5b5b  , 1.0, 1.0]], [[
+00003800: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+00003810: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
+00003820: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
+00003830: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
+00003840: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
+00003850: 2031 2e30 5d5d 2c20 5b5b 312e 302c 2031   1.0]], [[1.0, 1
+00003860: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
+00003870: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+00003880: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
+00003890: 312e 302c 2031 2e30 5d2c 205b 312e 302c  1.0, 1.0], [1.0,
+000038a0: 2031 2e30 2c20 312e 302c 2031 2e30 5d5d   1.0, 1.0, 1.0]]
+000038b0: 2c20 5b5b 312e 302c 2031 2e30 2c20 312e  , [[1.0, 1.0, 1.
+000038c0: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
+000038d0: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
+000038e0: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+000038f0: 2e30 5d2c 205b 312e 302c 2031 2e30 2c20  .0], [1.0, 1.0, 
+00003900: 312e 302c 2031 2e30 5d5d 2c20 5b5b 312e  1.0, 1.0]], [[1.
+00003910: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00003920: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
+00003930: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
+00003940: 2e30 2c20 312e 302c 2031 2e30 5d2c 205b  .0, 1.0, 1.0], [
+00003950: 312e 302c 2031 2e30 2c20 312e 302c 2031  1.0, 1.0, 1.0, 1
+00003960: 2e30 5d5d 2c20 5b5b 312e 302c 2031 2e30  .0]], [[1.0, 1.0
+00003970: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+00003980: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00003990: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
+000039a0: 302c 2031 2e30 5d2c 205b 312e 302c 2031  0, 1.0], [1.0, 1
+000039b0: 2e30 2c20 312e 302c 2031 2e30 5d5d 2c20  .0, 1.0, 1.0]], 
+000039c0: 5b5b 312e 302c 2031 2e30 2c20 312e 302c  [[1.0, 1.0, 1.0,
+000039d0: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+000039e0: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+000039f0: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00003a00: 5d2c 205b 312e 302c 2031 2e30 2c20 312e  ], [1.0, 1.0, 1.
+00003a10: 302c 2031 2e30 5d5d 2c20 5b5b 312e 302c  0, 1.0]], [[1.0,
+00003a20: 2031 2e30 2c20 312e 302c 2031 2e30 5d2c   1.0, 1.0, 1.0],
+00003a30: 205b 312e 302c 2031 2e30 2c20 312e 302c   [1.0, 1.0, 1.0,
+00003a40: 2031 2e30 5d2c 205b 312e 302c 2031 2e30   1.0], [1.0, 1.0
+00003a50: 2c20 312e 302c 2031 2e30 5d2c 205b 312e  , 1.0, 1.0], [1.
+00003a60: 302c 2031 2e30 2c20 312e 302c 2031 2e30  0, 1.0, 1.0, 1.0
+00003a70: 5d5d 5d22 0a20 2020 2020 2020 2020 2020  ]]]".           
+00003a80: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+00003a90: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00003aa0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00003ab0: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
+00003ac0: 2263 6f6d 706c 6961 6e63 655f 3022 2c0a  "compliance_0",.
+00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ae0: 2269 6f5f 6d6f 6465 223a 2022 6f75 7422  "io_mode": "out"
+00003af0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003b00: 2020 2274 7970 6522 3a20 2246 6c6f 6174    "type": "Float
+00003b10: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00003b20: 2020 2022 7368 6170 6522 3a20 2231 222c     "shape": "1",
+00003b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003b40: 2022 756e 6974 7322 3a20 6e75 6c6c 2c0a   "units": null,.
+00003b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b60: 2264 6573 6322 3a20 2222 0a20 2020 2020  "desc": "".     
+00003b70: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00003b80: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+00003b90: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
+00003ba0: 6522 3a20 2263 6f6d 706c 6961 6e63 655f  e": "compliance_
+00003bb0: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
+00003bc0: 2020 2020 2269 6f5f 6d6f 6465 223a 2022      "io_mode": "
+00003bd0: 6f75 7422 2c0a 2020 2020 2020 2020 2020  out",.          
+00003be0: 2020 2020 2020 2274 7970 6522 3a20 2246        "type": "F
+00003bf0: 6c6f 6174 222c 0a20 2020 2020 2020 2020  loat",.         
+00003c00: 2020 2020 2020 2022 7368 6170 6522 3a20         "shape": 
+00003c10: 2231 222c 0a20 2020 2020 2020 2020 2020  "1",.           
+00003c20: 2020 2020 2022 756e 6974 7322 3a20 6e75       "units": nu
+00003c30: 6c6c 2c0a 2020 2020 2020 2020 2020 2020  ll,.            
+00003c40: 2020 2020 2264 6573 6322 3a20 2222 0a20      "desc": "". 
+00003c50: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+00003c60: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
+00003c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c80: 226e 616d 6522 3a20 2264 5f30 222c 0a20  "name": "d_0",. 
+00003c90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003ca0: 696f 5f6d 6f64 6522 3a20 226f 7574 222c  io_mode": "out",
+00003cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003cc0: 2022 6465 7363 223a 2022 222c 0a20 2020   "desc": "",.   
+00003cd0: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
+00003ce0: 7065 223a 2022 466c 6f61 7422 2c0a 2020  pe": "Float",.  
+00003cf0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00003d00: 6861 7065 223a 2022 2831 3034 2c29 222c  hape": "(104,)",
+00003d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003d20: 2022 756e 6974 7322 3a20 6e75 6c6c 0a20   "units": null. 
+00003d30: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+00003d40: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
+00003d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d60: 226e 616d 6522 3a20 2264 5f31 222c 0a20  "name": "d_1",. 
+00003d70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003d80: 696f 5f6d 6f64 6522 3a20 226f 7574 222c  io_mode": "out",
+00003d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003da0: 2022 6465 7363 223a 2022 222c 0a20 2020   "desc": "",.   
+00003db0: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
+00003dc0: 7065 223a 2022 466c 6f61 7422 2c0a 2020  pe": "Float",.  
+00003dd0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00003de0: 6861 7065 223a 2022 2831 3034 2c29 222c  hape": "(104,)",
+00003df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003e00: 2022 756e 6974 7322 3a20 6e75 6c6c 0a20   "units": null. 
+00003e10: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+00003e20: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
+00003e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e40: 226e 616d 6522 3a20 2264 6973 706c 6163  "name": "displac
+00003e50: 656d 656e 7473 5f30 222c 0a20 2020 2020  ements_0",.     
+00003e60: 2020 2020 2020 2020 2020 2022 696f 5f6d             "io_m
+00003e70: 6f64 6522 3a20 226f 7574 222c 0a20 2020  ode": "out",.   
+00003e80: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00003e90: 7363 223a 2022 222c 0a20 2020 2020 2020  sc": "",.       
+00003ea0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00003eb0: 2022 466c 6f61 7422 2c0a 2020 2020 2020   "Float",.      
+00003ec0: 2020 2020 2020 2020 2020 2273 6861 7065            "shape
+00003ed0: 223a 2022 2831 3032 2c29 222c 0a20 2020  ": "(102,)",.   
+00003ee0: 2020 2020 2020 2020 2020 2020 2022 756e               "un
+00003ef0: 6974 7322 3a20 6e75 6c6c 0a20 2020 2020  its": null.     
+00003f00: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00003f10: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+00003f20: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
+00003f30: 6522 3a20 2264 6973 706c 6163 656d 656e  e": "displacemen
+00003f40: 7473 5f31 222c 0a20 2020 2020 2020 2020  ts_1",.         
+00003f50: 2020 2020 2020 2022 696f 5f6d 6f64 6522         "io_mode"
+00003f60: 3a20 226f 7574 222c 0a20 2020 2020 2020  : "out",.       
+00003f70: 2020 2020 2020 2020 2022 6465 7363 223a           "desc":
+00003f80: 2022 222c 0a20 2020 2020 2020 2020 2020   "",.           
+00003f90: 2020 2020 2022 7479 7065 223a 2022 466c       "type": "Fl
+00003fa0: 6f61 7422 2c0a 2020 2020 2020 2020 2020  oat",.          
+00003fb0: 2020 2020 2020 2273 6861 7065 223a 2022        "shape": "
+00003fc0: 2831 3032 2c29 222c 0a20 2020 2020 2020  (102,)",.       
+00003fd0: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
+00003fe0: 3a20 6e75 6c6c 0a20 2020 2020 2020 2020  : null.         
+00003ff0: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+00004000: 2020 205d 0a20 2020 2020 2020 2020 207d     ].          }
+00004010: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
+00004020: 207d 0a20 2020 207d 2c0a 2020 2020 7b0a   }.    },.    {.
+00004030: 2020 2020 2020 226e 616d 6522 3a20 2256        "name": "V
+00004040: 6f6c 756d 6543 6f6d 7022 2c0a 2020 2020  olumeComp",.    
+00004050: 2020 2276 6172 6961 626c 6573 5f61 7474    "variables_att
+00004060: 7269 6275 7465 7322 3a20 5b0a 2020 2020  ributes": [.    
+00004070: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00004080: 226e 616d 6522 3a20 2268 222c 0a20 2020  "name": "h",.   
+00004090: 2020 2020 2020 2022 696f 5f6d 6f64 6522         "io_mode"
+000040a0: 3a20 2269 6e22 2c0a 2020 2020 2020 2020  : "in",.        
+000040b0: 2020 2274 7970 6522 3a20 2246 6c6f 6174    "type": "Float
+000040c0: 222c 0a20 2020 2020 2020 2020 2022 7368  ",.          "sh
+000040d0: 6170 6522 3a20 2228 312c 2035 3029 222c  ape": "(1, 50)",
+000040e0: 0a20 2020 2020 2020 2020 2022 756e 6974  .          "unit
+000040f0: 7322 3a20 6e75 6c6c 2c0a 2020 2020 2020  s": null,.      
+00004100: 2020 2020 2264 6573 6322 3a20 2222 0a20      "desc": "". 
+00004110: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00004120: 2020 7b0a 2020 2020 2020 2020 2020 226e    {.          "n
+00004130: 616d 6522 3a20 2276 6f6c 756d 6522 2c0a  ame": "volume",.
+00004140: 2020 2020 2020 2020 2020 2269 6f5f 6d6f            "io_mo
+00004150: 6465 223a 2022 6f75 7422 2c0a 2020 2020  de": "out",.    
+00004160: 2020 2020 2020 2264 6573 6322 3a20 2222        "desc": ""
+00004170: 2c0a 2020 2020 2020 2020 2020 2274 7970  ,.          "typ
+00004180: 6522 3a20 2246 6c6f 6174 222c 0a20 2020  e": "Float",.   
+00004190: 2020 2020 2020 2022 7368 6170 6522 3a20         "shape": 
+000041a0: 2231 222c 0a20 2020 2020 2020 2020 2022  "1",.          "
+000041b0: 756e 6974 7322 3a20 6e75 6c6c 0a20 2020  units": null.   
+000041c0: 2020 2020 207d 0a20 2020 2020 205d 0a20       }.      ]. 
+000041d0: 2020 207d 2c0a 2020 2020 7b0a 2020 2020     },.    {.    
+000041e0: 2020 226e 616d 6522 3a20 224f 626a 5375    "name": "ObjSu
+000041f0: 6d22 2c0a 2020 2020 2020 2276 6172 6961  m",.      "varia
+00004200: 626c 6573 5f61 7474 7269 6275 7465 7322  bles_attributes"
+00004210: 3a20 5b0a 2020 2020 2020 2020 7b0a 2020  : [.        {.  
+00004220: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
+00004230: 2263 6f6d 706c 6961 6e63 655f 3022 2c0a  "compliance_0",.
+00004240: 2020 2020 2020 2020 2020 2269 6f5f 6d6f            "io_mo
+00004250: 6465 223a 2022 696e 222c 0a20 2020 2020  de": "in",.     
+00004260: 2020 2020 2022 7479 7065 223a 2022 466c       "type": "Fl
+00004270: 6f61 7422 2c0a 2020 2020 2020 2020 2020  oat",.          
+00004280: 2273 6861 7065 223a 2022 3122 2c0a 2020  "shape": "1",.  
+00004290: 2020 2020 2020 2020 2275 6e69 7473 223a          "units":
+000042a0: 206e 756c 6c2c 0a20 2020 2020 2020 2020   null,.         
+000042b0: 2022 6465 7363 223a 2022 220a 2020 2020   "desc": "".    
+000042c0: 2020 2020 7d2c 0a20 2020 2020 2020 207b      },.        {
+000042d0: 0a20 2020 2020 2020 2020 2022 6e61 6d65  .          "name
+000042e0: 223a 2022 636f 6d70 6c69 616e 6365 5f31  ": "compliance_1
+000042f0: 222c 0a20 2020 2020 2020 2020 2022 696f  ",.          "io
+00004300: 5f6d 6f64 6522 3a20 2269 6e22 2c0a 2020  _mode": "in",.  
+00004310: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00004320: 2246 6c6f 6174 222c 0a20 2020 2020 2020  "Float",.       
+00004330: 2020 2022 7368 6170 6522 3a20 2231 222c     "shape": "1",
+00004340: 0a20 2020 2020 2020 2020 2022 756e 6974  .          "unit
+00004350: 7322 3a20 6e75 6c6c 2c0a 2020 2020 2020  s": null,.      
+00004360: 2020 2020 2264 6573 6322 3a20 2222 0a20      "desc": "". 
+00004370: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00004380: 2020 7b0a 2020 2020 2020 2020 2020 226e    {.          "n
+00004390: 616d 6522 3a20 226f 626a 222c 0a20 2020  ame": "obj",.   
+000043a0: 2020 2020 2020 2022 696f 5f6d 6f64 6522         "io_mode"
+000043b0: 3a20 226f 7574 222c 0a20 2020 2020 2020  : "out",.       
+000043c0: 2020 2022 6465 7363 223a 2022 222c 0a20     "desc": "",. 
+000043d0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+000043e0: 2022 466c 6f61 7422 2c0a 2020 2020 2020   "Float",.      
+000043f0: 2020 2020 2273 6861 7065 223a 2022 3122      "shape": "1"
+00004400: 2c0a 2020 2020 2020 2020 2020 2275 6e69  ,.          "uni
+00004410: 7473 223a 206e 756c 6c0a 2020 2020 2020  ts": null.      
+00004420: 2020 7d0a 2020 2020 2020 5d0a 2020 2020    }.      ].    
+00004430: 7d0a 2020 5d0a 7d                        }.  ].}
```

### Comparing `wop-2.5.2/tests/data/test_doe.csv` & `wop-2.5.3/tests/data/test_doe.csv`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-success;x;z[1];z[0];f;g1
-1;6.7;2.7;9.7;146.60982587795195;-95.85982587775557
-1;5.700000000000001;7.9;0.7000000000000001;52.07630154666789;-8.526295515213691
-1;8.7;3.5;7.3;140.94827138735585;-58.59827137947353
-1;6.5;0.8999999999999999;2.3;54.52684773036366;-8.215449784095334
-1;7.5;5.300000000000001;5.700000000000001;103.34698821912461;-38.63698819312174
-1;8.5;8.5;4.9;117.86161395651092;-33.95161395308513
-1;7.9;1.6999999999999997;9.3;156.08195975647743;-88.81195975533512
-1;2.7;2.1;2.9000000000000004;20.921083500302274;-8.37085766659958
-1;4.1000000000000005;7.1;2.1;36.95757428011381;-9.8875715526605
-1;8.9;9.9;6.1;140.48645261415422;-48.216452614067435
-1;8.100000000000001;1.9;1.9;79.66346816015928;-8.9927831550186
-1;7.1;3.1;8.100000000000001;125.38442429716278;-68.71442429431829
-1;1.5000000000000002;0.7000000000000001;2.7;11.187922813863164;-5.0760302985478845
-1;5.5;4.1000000000000005;8.3;108.63621102207082;-71.12621102132681
-1;9.3;2.5;5.5;128.18783713054165;-36.03783648991407
-1;2.9000000000000004;5.1;0.3;20.0104471717548;-3.340094343185706
-1;1.6999999999999997;4.3;0.5;12.040475325447835;-1.689565422747302
-1;1.1;1.3;9.1;83.83637723526623;-78.16637723157798
-1;0.8999999999999999;4.9;6.9;55.35087439980805;-46.48087439327
-1;4.699999999999999;9.7;8.9;119.8036877891692;-84.8536877891685
-1;2.1;9.3;9.5;109.64111142437766;-92.77111142437728
-1;8.3;3.7;1.3;84.5874697988988;-8.837258810189379
-1;7.7;7.7;7.5;133.96325620495116;-63.81325620488123
-1;3.7;4.699999999999999;1.5000000000000002;27.206263824976315;-5.656159625332805
-1;0.1;7.5;1.6999999999999997;15.591448329148438;-4.921442442288347
-1;9.5;8.100000000000001;8.5;183.03946244286334;-81.52946244285712
-1;5.1;9.5;1.1;48.47973045783158;-9.809729777952658
-1;4.5;6.9;0.1;36.546954852531584;-6.236912328379468
-1;9.7;7.3;9.9;210.8673713054177;-106.31737130541676
-1;9.9;1.1;3.9000000000000004;123.33565872263962;-21.065609637381577
-1;4.3;5.5;0.8999999999999999;32.72885816640099;-5.578771733431092
-1;1.3;0.3;3.3000000000000003;13.09453575875515;-7.943559907572814
-1;0.7000000000000001;0.1;5.300000000000001;27.365132200885206;-23.61510664049846
-1;7.3;8.9;4.699999999999999;96.58702053762845;-31.237020534108776
-1;6.9;5.700000000000001;2.5;69.71006502937462;-13.240060242815648
-1;2.3;8.3;6.7;64.65086232456979;-47.900862324328656
-1;0.3;0.5;3.1;9.678444344100402;-5.927103535346944
-1;6.1;6.7;6.5;94.89196685121493;-47.82196684974811
-1;3.5;8.7;5.8999999999999995;63.73184338325432;-39.62184338259564
-1;9.1;6.1;5.1;126.65132072793612;-34.581320698569215
-1;5.8999999999999995;9.1;4.3;73.62968473533182;-26.559684728832558
-1;3.3000000000000003;3.3000000000000003;3.5;30.863358742185994;-13.51333997311368
-1;5.300000000000001;6.3;7.9;103.8926351901895;-66.34263519002643
-1;3.9000000000000004;6.5;3.7;42.840638889392174;-17.970638514567487
-1;3.1;2.3;7.7;73.03633338647133;-57.9663333682073
-1;6.3;1.5000000000000002;4.5;67.02348269903989;-22.673467322435645
-1;1.9;2.9000000000000004;6.3;47.87370769843603;-38.203707535753026
-1;4.9;3.9000000000000004;8.7;108.08914384912414;-77.01914384868853
-1;2.5;5.8999999999999995;4.1000000000000005;34.4162577069513;-19.106257301681786
-1;0.5;4.5;7.1;56.402605070331354;-48.49260506339836
+success;x;z[1];z[0];f;g1
+1;6.7;2.7;9.7;146.60982587795195;-95.85982587775557
+1;5.700000000000001;7.9;0.7000000000000001;52.07630154666789;-8.526295515213691
+1;8.7;3.5;7.3;140.94827138735585;-58.59827137947353
+1;6.5;0.8999999999999999;2.3;54.52684773036366;-8.215449784095334
+1;7.5;5.300000000000001;5.700000000000001;103.34698821912461;-38.63698819312174
+1;8.5;8.5;4.9;117.86161395651092;-33.95161395308513
+1;7.9;1.6999999999999997;9.3;156.08195975647743;-88.81195975533512
+1;2.7;2.1;2.9000000000000004;20.921083500302274;-8.37085766659958
+1;4.1000000000000005;7.1;2.1;36.95757428011381;-9.8875715526605
+1;8.9;9.9;6.1;140.48645261415422;-48.216452614067435
+1;8.100000000000001;1.9;1.9;79.66346816015928;-8.9927831550186
+1;7.1;3.1;8.100000000000001;125.38442429716278;-68.71442429431829
+1;1.5000000000000002;0.7000000000000001;2.7;11.187922813863164;-5.0760302985478845
+1;5.5;4.1000000000000005;8.3;108.63621102207082;-71.12621102132681
+1;9.3;2.5;5.5;128.18783713054165;-36.03783648991407
+1;2.9000000000000004;5.1;0.3;20.0104471717548;-3.340094343185706
+1;1.6999999999999997;4.3;0.5;12.040475325447835;-1.689565422747302
+1;1.1;1.3;9.1;83.83637723526623;-78.16637723157798
+1;0.8999999999999999;4.9;6.9;55.35087439980805;-46.48087439327
+1;4.699999999999999;9.7;8.9;119.8036877891692;-84.8536877891685
+1;2.1;9.3;9.5;109.64111142437766;-92.77111142437728
+1;8.3;3.7;1.3;84.5874697988988;-8.837258810189379
+1;7.7;7.7;7.5;133.96325620495116;-63.81325620488123
+1;3.7;4.699999999999999;1.5000000000000002;27.206263824976315;-5.656159625332805
+1;0.1;7.5;1.6999999999999997;15.591448329148438;-4.921442442288347
+1;9.5;8.100000000000001;8.5;183.03946244286334;-81.52946244285712
+1;5.1;9.5;1.1;48.47973045783158;-9.809729777952658
+1;4.5;6.9;0.1;36.546954852531584;-6.236912328379468
+1;9.7;7.3;9.9;210.8673713054177;-106.31737130541676
+1;9.9;1.1;3.9000000000000004;123.33565872263962;-21.065609637381577
+1;4.3;5.5;0.8999999999999999;32.72885816640099;-5.578771733431092
+1;1.3;0.3;3.3000000000000003;13.09453575875515;-7.943559907572814
+1;0.7000000000000001;0.1;5.300000000000001;27.365132200885206;-23.61510664049846
+1;7.3;8.9;4.699999999999999;96.58702053762845;-31.237020534108776
+1;6.9;5.700000000000001;2.5;69.71006502937462;-13.240060242815648
+1;2.3;8.3;6.7;64.65086232456979;-47.900862324328656
+1;0.3;0.5;3.1;9.678444344100402;-5.927103535346944
+1;6.1;6.7;6.5;94.89196685121493;-47.82196684974811
+1;3.5;8.7;5.8999999999999995;63.73184338325432;-39.62184338259564
+1;9.1;6.1;5.1;126.65132072793612;-34.581320698569215
+1;5.8999999999999995;9.1;4.3;73.62968473533182;-26.559684728832558
+1;3.3000000000000003;3.3000000000000003;3.5;30.863358742185994;-13.51333997311368
+1;5.300000000000001;6.3;7.9;103.8926351901895;-66.34263519002643
+1;3.9000000000000004;6.5;3.7;42.840638889392174;-17.970638514567487
+1;3.1;2.3;7.7;73.03633338647133;-57.9663333682073
+1;6.3;1.5000000000000002;4.5;67.02348269903989;-22.673467322435645
+1;1.9;2.9000000000000004;6.3;47.87370769843603;-38.203707535753026
+1;4.9;3.9000000000000004;8.7;108.08914384912414;-77.01914384868853
+1;2.5;5.8999999999999995;4.1000000000000005;34.4162577069513;-19.106257301681786
+1;0.5;4.5;7.1;56.402605070331354;-48.49260506339836
```

### Comparing `wop-2.5.2/tests/data/test_doe.hdf5` & `wop-2.5.3/tests/data/test_doe.hdf5`

 * *Files identical despite different names*

### Comparing `wop-2.5.2/tests/data/test_doe.sqlite` & `wop-2.5.3/tests/data/test_doe.sqlite`

 * *Files identical despite different names*

### Comparing `wop-2.5.2/tests/data/test_parallel_doe.sqlite_0` & `wop-2.5.3/tests/data/test_parallel_doe.sqlite_0`

 * *Files identical despite different names*

### Comparing `wop-2.5.2/tests/data/test_parallel_doe.sqlite_1` & `wop-2.5.3/tests/data/test_parallel_doe.sqlite_1`

 * *Files identical despite different names*

### Comparing `wop-2.5.2/tests/data/test_parallel_doe.sqlite_2` & `wop-2.5.3/tests/data/test_parallel_doe.sqlite_2`

 * *Files identical despite different names*

### Comparing `wop-2.5.2/tests/test_push_utils.py` & `wop-2.5.3/tests/test_push_utils.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import os
-import unittest
-import numpy as np
-
-from whatsopt.push_utils import (
-    build_variable_name,
-    simple_value,
-    format_shape,
-    to_camelcase,
-    extract_mda_var,
-    problem_pyfile,
-)
-
-
-class TestPushUtils(unittest.TestCase):
-    DATA_PATH = os.path.join(os.path.dirname(__file__), "data")
-
-    def test_format_shape(self):
-        self.assertEqual("_file", format_shape(False, "L_file"))
-        self.assertEqual("1", format_shape(True, "(1,)"))
-
-    def test_to_camelcase(self):
-        self.assertEqual("ToCamelCase", to_camelcase("to_camel_case"))
-        self.assertEqual("Camel", to_camelcase("camel"))
-
-    def test_simple_value(self):
-        dict1 = {"type": "Integer", "shape": "1", "value": 1}
-        dict2 = {"type": "Float", "shape": "(1,)", "value": 1.2}
-        dict3 = {"type": "Float", "shape": None, "value": np.array(["1.2", "2.3"])}
-        self.assertEqual("1", simple_value(dict1))
-        self.assertEqual("1.2", simple_value(dict2))
-        self.assertEqual("[1.2, 2.3]", simple_value(dict3))
-
-    def test_extract_mda_var(self):
-        val1, val2 = extract_mda_var("a.b.c.d")
-        self.assertEqual(["a", "b", "c"], val1)
-        self.assertEqual("d", val2)
-        # raise Exception
-        self.assertRaises(Exception, extract_mda_var, "a")
-
-    def test_generate_problem_pyfile(self):
-        with problem_pyfile(
-            os.path.join(self.DATA_PATH, "disc1.py"), "Disc1"
-        ) as pbfile:
-            self.assertTrue(os.path.exists(pbfile))
-            self.assertTrue(os.system("python {}".format(pbfile)) == 0)
-        self.assertFalse(os.path.exists(pbfile))
-
-    def test_build_varname(self):
-        name = build_variable_name("12", "ab", 7)
-        self.assertEqual("12==ab", name)
-        name = build_variable_name("123456789", "abcdefghi", 11)
-        self.assertEqual("...bcdefghi", name)
-        name = build_variable_name("123456789", "abcdefghi", 12)
-        self.assertEqual("1...9==a...i", name)
-        name = build_variable_name("123456789", "abcdefghi", 13)
-        self.assertEqual("1...9==a...i", name)
-        name = build_variable_name("123456789", "abcdefghi", 14)
-        self.assertEqual("1...9==a...i", name)
-        name = build_variable_name("123456789", "abcdefghi", 15)
-        self.assertEqual("1...9==a...i", name)
-        name = build_variable_name("123456789", "abcdefghi", 16)
-        self.assertEqual("12...89==ab...hi", name)
-        name = build_variable_name("123456789", "abcdefghi", 17)
-        self.assertEqual("12...89==ab...hi", name)
-        name = build_variable_name("123456789", "abcdefghi", 18)
-        self.assertEqual("12...89==ab...hi", name)
-        name = build_variable_name("123456789", "abcdefghi", 19)
-        self.assertEqual("12...89==ab...hi", name)
-        name = build_variable_name("123456789", "abcdefghi", 20)
-        self.assertEqual("123456789==abcdefghi", name)
+import os
+import unittest
+import numpy as np
+
+from whatsopt.push_utils import (
+    build_variable_name,
+    simple_value,
+    format_shape,
+    to_camelcase,
+    extract_mda_var,
+    problem_pyfile,
+)
+
+
+class TestPushUtils(unittest.TestCase):
+    DATA_PATH = os.path.join(os.path.dirname(__file__), "data")
+
+    def test_format_shape(self):
+        self.assertEqual("_file", format_shape(False, "L_file"))
+        self.assertEqual("1", format_shape(True, "(1,)"))
+
+    def test_to_camelcase(self):
+        self.assertEqual("ToCamelCase", to_camelcase("to_camel_case"))
+        self.assertEqual("Camel", to_camelcase("camel"))
+
+    def test_simple_value(self):
+        dict1 = {"type": "Integer", "shape": "1", "value": 1}
+        dict2 = {"type": "Float", "shape": "(1,)", "value": 1.2}
+        dict3 = {"type": "Float", "shape": None, "value": np.array(["1.2", "2.3"])}
+        self.assertEqual("1", simple_value(dict1))
+        self.assertEqual("1.2", simple_value(dict2))
+        self.assertEqual("[1.2, 2.3]", simple_value(dict3))
+
+    def test_extract_mda_var(self):
+        val1, val2 = extract_mda_var("a.b.c.d")
+        self.assertEqual(["a", "b", "c"], val1)
+        self.assertEqual("d", val2)
+        # raise Exception
+        self.assertRaises(Exception, extract_mda_var, "a")
+
+    def test_generate_problem_pyfile(self):
+        with problem_pyfile(
+            os.path.join(self.DATA_PATH, "disc1.py"), "Disc1"
+        ) as pbfile:
+            self.assertTrue(os.path.exists(pbfile))
+            self.assertTrue(os.system("python {}".format(pbfile)) == 0)
+        self.assertFalse(os.path.exists(pbfile))
+
+    def test_build_varname(self):
+        name = build_variable_name("12", "ab", 7)
+        self.assertEqual("12==ab", name)
+        name = build_variable_name("123456789", "abcdefghi", 11)
+        self.assertEqual("...bcdefghi", name)
+        name = build_variable_name("123456789", "abcdefghi", 12)
+        self.assertEqual("1...9==a...i", name)
+        name = build_variable_name("123456789", "abcdefghi", 13)
+        self.assertEqual("1...9==a...i", name)
+        name = build_variable_name("123456789", "abcdefghi", 14)
+        self.assertEqual("1...9==a...i", name)
+        name = build_variable_name("123456789", "abcdefghi", 15)
+        self.assertEqual("1...9==a...i", name)
+        name = build_variable_name("123456789", "abcdefghi", 16)
+        self.assertEqual("12...89==ab...hi", name)
+        name = build_variable_name("123456789", "abcdefghi", 17)
+        self.assertEqual("12...89==ab...hi", name)
+        name = build_variable_name("123456789", "abcdefghi", 18)
+        self.assertEqual("12...89==ab...hi", name)
+        name = build_variable_name("123456789", "abcdefghi", 19)
+        self.assertEqual("12...89==ab...hi", name)
+        name = build_variable_name("123456789", "abcdefghi", 20)
+        self.assertEqual("123456789==abcdefghi", name)
```

### Comparing `wop-2.5.2/whatsopt/convert_utils.py` & `wop-2.5.3/whatsopt/convert_utils.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import csv
-import openmdao.api as om
-from whatsopt.logging import log
-
-from whatsopt.upload_utils import load_sqlite_file
-
-
-def convert_sqlite_to_csv(sqlite_filename, basename):
-    cr = om.CaseReader(sqlite_filename)
-    driver_cases = cr.list_cases("driver", out_stream=None)
-    design_vars = sorted(cr.get_case(driver_cases[0]).get_design_vars())
-    driver_name, cases, statuses = load_sqlite_file(sqlite_filename)
-    all_vars = [v["varname"] for v in cases]
-    out_vars = sorted(list(set(all_vars) - set(design_vars)))
-
-    fieldnames = []
-    values = {}
-    nb_cases = len(statuses)
-    for name in design_vars + out_vars:
-        for case in cases:
-            if name == case["varname"]:
-                if case["coord_index"] == -1:
-                    fieldnames.append(name)
-                    values[name] = case["values"]
-                else:
-                    name_i = f"{name}[{case['coord_index']}]"
-                    fieldnames.append(name_i)
-                    values[name_i] = case["values"]
-
-    outfile = f"{basename}.csv"
-    with open(outfile, "w") as f:
-        writer = csv.writer(f, delimiter=";", lineterminator="\n")
-        writer.writerow(["success"] + fieldnames)
-
-        for i in range(nb_cases):
-            data = [statuses[i]]
-            for var in fieldnames:
-                data.append(values[var][i])
-            writer.writerow(data)
-    log(f"Convert {nb_cases} cases ({driver_name}) to {outfile}")
+import csv
+import openmdao.api as om
+from whatsopt.logging import log
+
+from whatsopt.upload_utils import load_sqlite_file
+
+
+def convert_sqlite_to_csv(sqlite_filename, basename):
+    cr = om.CaseReader(sqlite_filename)
+    driver_cases = cr.list_cases("driver", out_stream=None)
+    design_vars = sorted(cr.get_case(driver_cases[0]).get_design_vars())
+    driver_name, cases, statuses = load_sqlite_file(sqlite_filename)
+    all_vars = [v["varname"] for v in cases]
+    out_vars = sorted(list(set(all_vars) - set(design_vars)))
+
+    fieldnames = []
+    values = {}
+    nb_cases = len(statuses)
+    for name in design_vars + out_vars:
+        for case in cases:
+            if name == case["varname"]:
+                if case["coord_index"] == -1:
+                    fieldnames.append(name)
+                    values[name] = case["values"]
+                else:
+                    name_i = f"{name}[{case['coord_index']}]"
+                    fieldnames.append(name_i)
+                    values[name_i] = case["values"]
+
+    outfile = f"{basename}.csv"
+    with open(outfile, "w") as f:
+        writer = csv.writer(f, delimiter=";", lineterminator="\n")
+        writer.writerow(["success"] + fieldnames)
+
+        for i in range(nb_cases):
+            data = [statuses[i]]
+            for var in fieldnames:
+                data.append(values[var][i])
+            writer.writerow(data)
+    log(f"Convert {nb_cases} cases ({driver_name}) to {outfile}")
```

### Comparing `wop-2.5.2/whatsopt/mooptimization.py` & `wop-2.5.3/whatsopt/mooptimization.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-import numpy as np
-from .optimization import Optimization
-
-# from smt.applications.mixed_integer import FLOAT, INT, ORD, ENUM
-# To avoid smt dependency replicate SMT mixed integer types
-FLOAT = "float_type"
-INT = "int_type"
-ORD = "ord_type"
-ENUM = "enum_type"
-
-SEGMOOMOE = "SEGMOOMOE"
-
-
-class OptimizationError(Exception):
-    pass
-
-
-class MOOptimization(Optimization):
-    def __init__(
-        self, xtypes=None, n_obj=2, cstr_specs=None, options=None, xlimits=None
-    ):
-        """Creation of a mixed-integer multi-objectives optimization context
-
-        Parameters
-        ----------
-        xtypes: list of x inputs type specification (maybe optional if xlimits is specified, see below).
-            A type specification consists in a dictionary of two items {type: ... , limits: ...} where type is either
-            FLOAT, INT, ORD or ENUM and limits the corresponding bounds: for instance [-1.5, 3.0] for a FLOAT
-            [1, 3] for an INT [1, 5, 7, 12] for an ORD and ["red", "green", "blue"] for an ENUM.
-        n_obj: number of objectives (default=2)
-        cstrs_specs: list of inequality constraints specifications (optional)
-            A constraint specification is a dictionary of two items {type: ..., bound: ..., tol: ...}
-            where type is either '<' or '>', bound is a float value specifying a limit and tol the
-            acceptable tolerance before violation (ex if we want cstr_value < bound, we accept cstr_value < bound + tol)
-        options: dictionary containing options to be passed to the mixed-integer multi-objectives optimizer
-        xlimits: list of float limits in case we are dealing with float inputs
-            Convenient way when x inputs are floats to specify only [[lower bound, upper bound], ...].
-
-        Returns
-        -------
-        Optimizer handle allowing to trigger remote optimization operations
-
-        """
-        self._kind = SEGMOOMOE  # at the moment only one kind of MOO optimizer
-        self._n_obj = n_obj
-        self._cstr_specs = cstr_specs or []
-        self._options = options
-
-        if xtypes is None and xlimits is None:
-            raise OptimizationError(
-                "Configuration Error: you should specify either xtypes or xlimits"
-            )
-
-        if not (xtypes is None or xlimits is None):
-            raise OptimizationError(
-                "Configuration Error: you should specify either xtypes or xlimits exclusively, not both"
-            )
-
-        if xtypes is None and xlimits is not None:
-            self._xtypes = []
-            for xlim in xlimits:
-                xlim = np.asarray(xlim).tolist()
-                self._xtypes.append({"type": FLOAT, "limits": xlim})
-            print(f"Convert {xlimits} to {self._xtypes}")
-        else:
-            self._xtypes = xtypes
-
-        self._init_optimization()
-
-    def _init_config(self):
-        return {
-            "kind": self._kind,
-            "n_obj": self._n_obj,
-            "xlimits": [],  # not used
-            "xtypes": self._xtypes,
-            "cstr_specs": self._cstr_specs,
-            "options": self._options,
-        }
+import numpy as np
+from .optimization import Optimization
+
+# from smt.applications.mixed_integer import FLOAT, INT, ORD, ENUM
+# To avoid smt dependency replicate SMT mixed integer types
+FLOAT = "float_type"
+INT = "int_type"
+ORD = "ord_type"
+ENUM = "enum_type"
+
+SEGMOOMOE = "SEGMOOMOE"
+
+
+class OptimizationError(Exception):
+    pass
+
+
+class MOOptimization(Optimization):
+    def __init__(
+        self, xtypes=None, n_obj=2, cstr_specs=None, options=None, xlimits=None
+    ):
+        """Creation of a mixed-integer multi-objectives optimization context
+
+        Parameters
+        ----------
+        xtypes: list of x inputs type specification (maybe optional if xlimits is specified, see below).
+            A type specification consists in a dictionary of two items {type: ... , limits: ...} where type is either
+            FLOAT, INT, ORD or ENUM and limits the corresponding bounds: for instance [-1.5, 3.0] for a FLOAT
+            [1, 3] for an INT [1, 5, 7, 12] for an ORD and ["red", "green", "blue"] for an ENUM.
+        n_obj: number of objectives (default=2)
+        cstrs_specs: list of inequality constraints specifications (optional)
+            A constraint specification is a dictionary of two items {type: ..., bound: ..., tol: ...}
+            where type is either '<' or '>', bound is a float value specifying a limit and tol the
+            acceptable tolerance before violation (ex if we want cstr_value < bound, we accept cstr_value < bound + tol)
+        options: dictionary containing options to be passed to the mixed-integer multi-objectives optimizer
+        xlimits: list of float limits in case we are dealing with float inputs
+            Convenient way when x inputs are floats to specify only [[lower bound, upper bound], ...].
+
+        Returns
+        -------
+        Optimizer handle allowing to trigger remote optimization operations
+
+        """
+        self._kind = SEGMOOMOE  # at the moment only one kind of MOO optimizer
+        self._n_obj = n_obj
+        self._cstr_specs = cstr_specs or []
+        self._options = options
+
+        if xtypes is None and xlimits is None:
+            raise OptimizationError(
+                "Configuration Error: you should specify either xtypes or xlimits"
+            )
+
+        if not (xtypes is None or xlimits is None):
+            raise OptimizationError(
+                "Configuration Error: you should specify either xtypes or xlimits exclusively, not both"
+            )
+
+        if xtypes is None and xlimits is not None:
+            self._xtypes = []
+            for xlim in xlimits:
+                xlim = np.asarray(xlim).tolist()
+                self._xtypes.append({"type": FLOAT, "limits": xlim})
+            print(f"Convert {xlimits} to {self._xtypes}")
+        else:
+            self._xtypes = xtypes
+
+        self._init_optimization()
+
+    def _init_config(self):
+        return {
+            "kind": self._kind,
+            "n_obj": self._n_obj,
+            "xlimits": [],  # not used
+            "xtypes": self._xtypes,
+            "cstr_specs": self._cstr_specs,
+            "options": self._options,
+        }
```

### Comparing `wop-2.5.2/whatsopt/optimization.py` & `wop-2.5.3/whatsopt/optimization.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,323 +1,323 @@
-import sys
-import time
-import numpy as np
-from requests.exceptions import RequestException
-from .whatsopt_client import WhatsOpt
-
-
-SEGOMOE = "SEGOMOE"
-
-
-class OptimizationError(Exception):
-    pass
-
-
-class Optimization:
-    VALID_POINT = 0
-    INVALID_POINT = 1
-    RUNTIME_ERROR = 2
-    SOLUTION_REACHED = 3
-    RUNNING = 4
-    PENDING = -1
-
-    STATUSES = [
-        "valid point",
-        "invalid point",
-        "runtime error",
-        "solution reached",
-        "running",
-        "pending",
-    ]
-
-    DEFAULT_CSTR = {"type": "<", "bound": 0.0, "tol": 1e-4}
-    TIMEOUT = 60
-
-    def __init__(self, xlimits, cstr_specs=None, options=None):
-        """Creation of a continuous mono objective optimization context
-
-        Parameters
-        ----------
-        xlimits: list of float limits for x inputs eg [[lower bound, upper bound], ...]
-        cstrs_specs: list of inequality constraints specifications (optional)
-            A constraint specification is a dictionary of two items {type: ..., bound: ..., tol: ...}
-            where type is either '<' or '>', bound is a float value specifying a limit and tol the
-            acceptable tolerance before violation (ex if we want cstr_value < bound, we accept cstr_value < bound + tol).
-        options: dictionary containing options to be passed to the remote optimizer
-
-        Returns
-        -------
-        Optimizer handle allowing to trigger remote optimization operations
-
-        """
-        self._kind = SEGOMOE  # at the moment only one kind of Optimizer
-        self._xlimits = xlimits or []
-        self._cstr_specs = cstr_specs or []
-        self._options = options
-        self._init_optimization()
-
-    def _init_optimization(self):
-        try:
-            for cstr in self._cstr_specs:
-                for k in ["type", "bound", "tol"]:
-                    cstr[k] = cstr.get(k, self.DEFAULT_CSTR[k])
-
-            optim_config = self._init_config()
-
-            self._wop = WhatsOpt().login()
-            url = self._wop.endpoint("/api/v1/optimizations")
-            resp = self._wop.session.post(
-                url, headers=self._wop.headers, json={"optimization": optim_config}
-            )
-            if not resp.ok:
-                message = "Unexpected error"
-                if resp.json() and resp.json().get("message"):
-                    message = resp.json()["message"]
-                raise OptimizationError(
-                    f"Error {resp.reason} ({resp.status_code}): {message}"
-                )
-
-            self._id = resp.json()["id"]
-            self._x = np.array([])
-            self._y = np.array([])
-            self._x_suggested = None
-            self._status = self.PENDING
-            self._x_best = None
-            self._y_best = None
-        except RequestException as e:
-            raise OptimizationError("Connection failed during initialization")
-
-    def _init_config(self):
-        return {
-            "kind": self._kind,
-            "n_obj": 1,
-            "xlimits": self._xlimits,
-            "cstr_specs": self._cstr_specs,
-            "options": self._options,
-        }
-
-    def tell_doe(self, x, y):
-        """Send the initial DOE to the remote optimizer
-
-        This operation should be executed initially to set the initial data used
-        to model objectives and constraints.
-
-        Parameters
-        ----------
-        x : 2d array-like of inputs  [[x1, x2, ...], ...]
-        y : 2d array-like of outputs [[obj1, obj2, ..., objn, cstr1, cstr2, ... cstrn], ...]
-        """
-        self._x_best = None
-        self._status = self.PENDING
-        self._x = np.atleast_2d(x)
-        self._y = np.atleast_2d(y)
-        if self._x.shape[0] != self._y.shape[0]:
-            raise OptimizationError(
-                f"Bad DOE error: DOE x and y should of the same size, got x size = {self._x.shape[0]} and  x size = {self._y.shape[0]}"
-            )
-
-    def run(self, f_grouped, n_iter=1, with_best=False):
-        """Ask and tell the optimizer to get the optimum in n_iter iteration
-
-        Parameters
-        ----------
-        f_grouped : function under optimization y = f(x)
-            where y is of the form [obj1, obj2, ..., objn, cstr1, cstr2, ... cstrn]
-
-        n_iter : int, iteration budget
-
-        with_best : when set it compute the best point found at each iteration.
-
-        Returns
-        -------
-        x_opt, y_opt: 2d array, 2d array
-            an optimum in case of mono-objective or a list of optima in case
-            of multi-objective optimization (Pareto front).
-        """
-        self._x_best = None
-        for i in range(n_iter):
-            with_best = with_best or (i == n_iter - 1)
-            x_suggested, status, self._x_best, self._y_best = self.ask(with_best)
-            print(
-                f"{i} x suggested = {x_suggested} with status: {Optimization.STATUSES[status]}"
-            )
-
-            if with_best:
-                print(f"x_best={self._x_best}")
-                print(f"y_best={self._y_best}")
-
-            # compute objective function at the suggested point
-            new_y = f_grouped(x_suggested)
-            print("new y = {}".format(new_y))
-
-            self.tell(x_suggested, new_y)
-            if self.is_solution_reached():
-                print("Solution is reached")
-                x_suggested, status, self._x_best, self._y_best = self.ask(
-                    with_best=True
-                )
-                self._status = self.SOLUTION_REACHED
-                break
-
-        x_opt, y_opt = self.get_result()
-        print(f"Found optimum y_opt = {y_opt} at x_opt = {x_opt}")
-        return x_opt, y_opt
-
-    def tell(self, x, y):
-        """Gives (x, y) values such that y = f(x).
-
-        Parameters
-        ----------
-        x : 2d array-like of inputs  [x1, x2, ...]
-        y : 2d array-like of outputs [obj1, obj2, ..., objn, cstr1, cstr2, ... cstrn]
-        """
-
-        # check if already told
-        found = False
-        for i, v in enumerate(self._x):
-            if np.allclose(x, v):
-                print(
-                    "Value {} already told index {} with y = {}".format(
-                        x, i, self._y[i]
-                    )
-                )
-                found = True
-                break
-        if found:
-            self._status = self.SOLUTION_REACHED
-        else:
-            self._x = np.vstack((self._x, np.atleast_2d(x)))
-            self._y = np.vstack((self._y, np.atleast_2d(y)))
-
-    def ask(self, with_best=False):
-        """Trigger optimizer iteration to get next promising location of the optimum
-
-        Parameters
-        ----------
-        with_best: if set compute also the best (x_best, y_best) point so far among
-        points already computed.
-        In case of multi-objective the Pareto front is computed.
-
-        Returns
-        -------
-        status, x_suggested, x_best, y_best
-            where status is an status code (int) retuned by the optimizer
-                  x_suggested the next promising optimum location
-                  x_best, y_best the optima so far
-        """
-        self._status = self.RUNNING
-        self._optimizer_iteration(with_best)
-        retry = self.TIMEOUT
-        url = self._wop.endpoint("/api/v1/optimizations/{}".format(self._id))
-        resp = None
-        while retry > 0 and self.is_running():
-            resp = self._wop.session.get(url, headers=self._wop.headers)
-            if resp.ok:
-                result = resp.json()["outputs"]
-                self._x_suggested = result["x_suggested"]
-                self._status = result["status"]
-                if with_best:
-                    self._x_best = result["x_best"]
-                    self._y_best = result["y_best"]
-                else:
-                    self._x_best = None
-                    self._y_best = None
-            elif resp.status_code == 400:
-                message = "Unexpected error"
-                if resp.json() and resp.json().get("message"):
-                    message = resp.json()["message"]
-                raise OptimizationError(
-                    f"Error {resp.reason} ({resp.status_code}): {message}"
-                )
-
-            if self.is_running():
-                if retry + 1 % 10 == 0:
-                    print("Waiting for result...")
-                time.sleep(1)
-            retry = retry - 1
-
-        if retry <= 0:
-            self._x_suggested = None
-            self._status = self.RUNTIME_ERROR
-            self._x_best = None
-            self._y_best = None
-            raise OptimizationError(
-                "Time out: please check status and history and may be ask again."
-            )
-
-        self.status = self.PENDING
-
-        return self._x_suggested, self._status, self._x_best, self._y_best
-
-    def get_result(self):
-        """Retrieve optimum (or optima in case of moo) among the DOE with valid constraints
-
-        Returns
-        -------
-            x, y where x and y are 2d ndarrays
-        """
-        if not self._x_best:
-            _, _, self._x_best, self._y_best = self.ask(with_best=True)
-        x_opt = np.array(self._x_best)
-        y_opt = np.array(self._y_best)
-
-        return x_opt, y_opt
-
-    def get_history(self):
-        """Retrieve optimization history (initial doe + (x suggestions, y))
-
-        Returns
-        -------
-            x, y where x and y are 2d ndarrays
-        """
-        return self._x, self._y
-
-    def get_status(self):
-        """Retrieve status string"""
-        return self.STATUSES[self._status]
-
-    def is_solution_reached(self):
-        return self._status == self.SOLUTION_REACHED
-
-    def is_running(self):
-        return self._status == self.RUNNING
-
-    def _get_best_y(self, x):
-        y = None
-        x = np.array(x)
-        for i in range(self._x.shape[0]):
-            if np.equal(x, self._x[i]).all():
-                y = self._y[i].tolist()
-                break
-        return y
-
-    def _optimizer_iteration(self, with_best):
-        """Run optimizer iteration"""
-        if self._x.size == 0 or self._y.size == 0:
-            raise OptimizationError(
-                f"Empty DOE error: DOE should not be empty, got DOE x={self._x} and DOE y={self._y}"
-            )
-        if self._x.shape[0] != self._y.shape[0]:
-            raise OptimizationError(
-                f"Bad DOE error: DOE x and y should of the same size, got x size = {self._x.shape[0]} and  x size = {self._y.shape[0]}"
-            )
-        try:
-            url = self._wop.endpoint("/api/v1/optimizations/{}".format(self._id))
-            resp = self._wop.session.put(
-                url,
-                headers=self._wop.headers,
-                json={
-                    "optimization": {
-                        "x": self._x.tolist(),
-                        "y": self._y.tolist(),
-                        "with_best": with_best,
-                    }
-                },
-            )
-            if not resp.ok:
-                self._wop.err_msg(resp)
-                self._status = self.RUNTIME_ERROR
-                raise OptimizationError(
-                    f"Error {resp.reason} ({resp.status_code}): {resp.json()['message']}"
-                )
-        except RequestException as e:
-            raise OptimizationError(f"Connection failed: {e}")
+import sys
+import time
+import numpy as np
+from requests.exceptions import RequestException
+from .whatsopt_client import WhatsOpt
+
+
+SEGOMOE = "SEGOMOE"
+
+
+class OptimizationError(Exception):
+    pass
+
+
+class Optimization:
+    VALID_POINT = 0
+    INVALID_POINT = 1
+    RUNTIME_ERROR = 2
+    SOLUTION_REACHED = 3
+    RUNNING = 4
+    PENDING = -1
+
+    STATUSES = [
+        "valid point",
+        "invalid point",
+        "runtime error",
+        "solution reached",
+        "running",
+        "pending",
+    ]
+
+    DEFAULT_CSTR = {"type": "<", "bound": 0.0, "tol": 1e-4}
+    TIMEOUT = 60
+
+    def __init__(self, xlimits, cstr_specs=None, options=None):
+        """Creation of a continuous mono objective optimization context
+
+        Parameters
+        ----------
+        xlimits: list of float limits for x inputs eg [[lower bound, upper bound], ...]
+        cstrs_specs: list of inequality constraints specifications (optional)
+            A constraint specification is a dictionary of two items {type: ..., bound: ..., tol: ...}
+            where type is either '<' or '>', bound is a float value specifying a limit and tol the
+            acceptable tolerance before violation (ex if we want cstr_value < bound, we accept cstr_value < bound + tol).
+        options: dictionary containing options to be passed to the remote optimizer
+
+        Returns
+        -------
+        Optimizer handle allowing to trigger remote optimization operations
+
+        """
+        self._kind = SEGOMOE  # at the moment only one kind of Optimizer
+        self._xlimits = xlimits or []
+        self._cstr_specs = cstr_specs or []
+        self._options = options
+        self._init_optimization()
+
+    def _init_optimization(self):
+        try:
+            for cstr in self._cstr_specs:
+                for k in ["type", "bound", "tol"]:
+                    cstr[k] = cstr.get(k, self.DEFAULT_CSTR[k])
+
+            optim_config = self._init_config()
+
+            self._wop = WhatsOpt().login()
+            url = self._wop.endpoint("/api/v1/optimizations")
+            resp = self._wop.session.post(
+                url, headers=self._wop.headers, json={"optimization": optim_config}
+            )
+            if not resp.ok:
+                message = "Unexpected error"
+                if resp.json() and resp.json().get("message"):
+                    message = resp.json()["message"]
+                raise OptimizationError(
+                    f"Error {resp.reason} ({resp.status_code}): {message}"
+                )
+
+            self._id = resp.json()["id"]
+            self._x = np.array([])
+            self._y = np.array([])
+            self._x_suggested = None
+            self._status = self.PENDING
+            self._x_best = None
+            self._y_best = None
+        except RequestException as e:
+            raise OptimizationError("Connection failed during initialization")
+
+    def _init_config(self):
+        return {
+            "kind": self._kind,
+            "n_obj": 1,
+            "xlimits": self._xlimits,
+            "cstr_specs": self._cstr_specs,
+            "options": self._options,
+        }
+
+    def tell_doe(self, x, y):
+        """Send the initial DOE to the remote optimizer
+
+        This operation should be executed initially to set the initial data used
+        to model objectives and constraints.
+
+        Parameters
+        ----------
+        x : 2d array-like of inputs  [[x1, x2, ...], ...]
+        y : 2d array-like of outputs [[obj1, obj2, ..., objn, cstr1, cstr2, ... cstrn], ...]
+        """
+        self._x_best = None
+        self._status = self.PENDING
+        self._x = np.atleast_2d(x)
+        self._y = np.atleast_2d(y)
+        if self._x.shape[0] != self._y.shape[0]:
+            raise OptimizationError(
+                f"Bad DOE error: DOE x and y should of the same size, got x size = {self._x.shape[0]} and  x size = {self._y.shape[0]}"
+            )
+
+    def run(self, f_grouped, n_iter=1, with_best=False):
+        """Ask and tell the optimizer to get the optimum in n_iter iteration
+
+        Parameters
+        ----------
+        f_grouped : function under optimization y = f(x)
+            where y is of the form [obj1, obj2, ..., objn, cstr1, cstr2, ... cstrn]
+
+        n_iter : int, iteration budget
+
+        with_best : when set it compute the best point found at each iteration.
+
+        Returns
+        -------
+        x_opt, y_opt: 2d array, 2d array
+            an optimum in case of mono-objective or a list of optima in case
+            of multi-objective optimization (Pareto front).
+        """
+        self._x_best = None
+        for i in range(n_iter):
+            with_best = with_best or (i == n_iter - 1)
+            x_suggested, status, self._x_best, self._y_best = self.ask(with_best)
+            print(
+                f"{i} x suggested = {x_suggested} with status: {Optimization.STATUSES[status]}"
+            )
+
+            if with_best:
+                print(f"x_best={self._x_best}")
+                print(f"y_best={self._y_best}")
+
+            # compute objective function at the suggested point
+            new_y = f_grouped(x_suggested)
+            print("new y = {}".format(new_y))
+
+            self.tell(x_suggested, new_y)
+            if self.is_solution_reached():
+                print("Solution is reached")
+                x_suggested, status, self._x_best, self._y_best = self.ask(
+                    with_best=True
+                )
+                self._status = self.SOLUTION_REACHED
+                break
+
+        x_opt, y_opt = self.get_result()
+        print(f"Found optimum y_opt = {y_opt} at x_opt = {x_opt}")
+        return x_opt, y_opt
+
+    def tell(self, x, y):
+        """Gives (x, y) values such that y = f(x).
+
+        Parameters
+        ----------
+        x : 2d array-like of inputs  [x1, x2, ...]
+        y : 2d array-like of outputs [obj1, obj2, ..., objn, cstr1, cstr2, ... cstrn]
+        """
+
+        # check if already told
+        found = False
+        for i, v in enumerate(self._x):
+            if np.allclose(x, v):
+                print(
+                    "Value {} already told index {} with y = {}".format(
+                        x, i, self._y[i]
+                    )
+                )
+                found = True
+                break
+        if found:
+            self._status = self.SOLUTION_REACHED
+        else:
+            self._x = np.vstack((self._x, np.atleast_2d(x)))
+            self._y = np.vstack((self._y, np.atleast_2d(y)))
+
+    def ask(self, with_best=False):
+        """Trigger optimizer iteration to get next promising location of the optimum
+
+        Parameters
+        ----------
+        with_best: if set compute also the best (x_best, y_best) point so far among
+        points already computed.
+        In case of multi-objective the Pareto front is computed.
+
+        Returns
+        -------
+        status, x_suggested, x_best, y_best
+            where status is an status code (int) retuned by the optimizer
+                  x_suggested the next promising optimum location
+                  x_best, y_best the optima so far
+        """
+        self._status = self.RUNNING
+        self._optimizer_iteration(with_best)
+        retry = self.TIMEOUT
+        url = self._wop.endpoint("/api/v1/optimizations/{}".format(self._id))
+        resp = None
+        while retry > 0 and self.is_running():
+            resp = self._wop.session.get(url, headers=self._wop.headers)
+            if resp.ok:
+                result = resp.json()["outputs"]
+                self._x_suggested = result["x_suggested"]
+                self._status = result["status"]
+                if with_best:
+                    self._x_best = result["x_best"]
+                    self._y_best = result["y_best"]
+                else:
+                    self._x_best = None
+                    self._y_best = None
+            elif resp.status_code == 400:
+                message = "Unexpected error"
+                if resp.json() and resp.json().get("message"):
+                    message = resp.json()["message"]
+                raise OptimizationError(
+                    f"Error {resp.reason} ({resp.status_code}): {message}"
+                )
+
+            if self.is_running():
+                if retry + 1 % 10 == 0:
+                    print("Waiting for result...")
+                time.sleep(1)
+            retry = retry - 1
+
+        if retry <= 0:
+            self._x_suggested = None
+            self._status = self.RUNTIME_ERROR
+            self._x_best = None
+            self._y_best = None
+            raise OptimizationError(
+                "Time out: please check status and history and may be ask again."
+            )
+
+        self.status = self.PENDING
+
+        return self._x_suggested, self._status, self._x_best, self._y_best
+
+    def get_result(self):
+        """Retrieve optimum (or optima in case of moo) among the DOE with valid constraints
+
+        Returns
+        -------
+            x, y where x and y are 2d ndarrays
+        """
+        if not self._x_best:
+            _, _, self._x_best, self._y_best = self.ask(with_best=True)
+        x_opt = np.array(self._x_best)
+        y_opt = np.array(self._y_best)
+
+        return x_opt, y_opt
+
+    def get_history(self):
+        """Retrieve optimization history (initial doe + (x suggestions, y))
+
+        Returns
+        -------
+            x, y where x and y are 2d ndarrays
+        """
+        return self._x, self._y
+
+    def get_status(self):
+        """Retrieve status string"""
+        return self.STATUSES[self._status]
+
+    def is_solution_reached(self):
+        return self._status == self.SOLUTION_REACHED
+
+    def is_running(self):
+        return self._status == self.RUNNING
+
+    def _get_best_y(self, x):
+        y = None
+        x = np.array(x)
+        for i in range(self._x.shape[0]):
+            if np.equal(x, self._x[i]).all():
+                y = self._y[i].tolist()
+                break
+        return y
+
+    def _optimizer_iteration(self, with_best):
+        """Run optimizer iteration"""
+        if self._x.size == 0 or self._y.size == 0:
+            raise OptimizationError(
+                f"Empty DOE error: DOE should not be empty, got DOE x={self._x} and DOE y={self._y}"
+            )
+        if self._x.shape[0] != self._y.shape[0]:
+            raise OptimizationError(
+                f"Bad DOE error: DOE x and y should of the same size, got x size = {self._x.shape[0]} and  x size = {self._y.shape[0]}"
+            )
+        try:
+            url = self._wop.endpoint("/api/v1/optimizations/{}".format(self._id))
+            resp = self._wop.session.put(
+                url,
+                headers=self._wop.headers,
+                json={
+                    "optimization": {
+                        "x": self._x.tolist(),
+                        "y": self._y.tolist(),
+                        "with_best": with_best,
+                    }
+                },
+            )
+            if not resp.ok:
+                self._wop.err_msg(resp)
+                self._status = self.RUNTIME_ERROR
+                raise OptimizationError(
+                    f"Error {resp.reason} ({resp.status_code}): {resp.json()['message']}"
+                )
+        except RequestException as e:
+            raise OptimizationError(f"Connection failed: {e}")
```

### Comparing `wop-2.5.2/whatsopt/push_command.py` & `wop-2.5.3/whatsopt/push_command.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,354 +1,354 @@
-import re
-from itertools import chain
-from whatsopt.push_utils import (
-    build_variable_name,
-    cut,
-    find_indep_var_name,
-    simple_value,
-    extract_mda_var,
-    format_shape,
-)
-from whatsopt.logging import debug
-from openmdao.api import IndepVarComp
-
-from openmdao.visualization.n2_viewer.n2_viewer import _get_viewer_data
-
-# Special name for internal WhatsOpt discipline. cf. WhatsOpt Discipline model
-DRIVER_NAME = "__DRIVER__"
-# OpenMDAO 3.2+ component name (handles indep vars automatically)
-AUTO_IVC = "_auto_ivc"
-
-
-class PushCommand:
-    """
-    This push command allows to push any OpenMDAO problem
-    (as opposed to regular push command which works with "all vars promoted/no connect" assumption)
-    """
-
-    def __init__(self, problem, depth, scalar):
-        data = _get_viewer_data(problem)
-        self.problem = problem
-        self.depth = depth
-        self.scalar = scalar
-        self.tree = data["tree"]
-        self.connections = data["connections_list"]
-        self.vars = {"in": {}, "out": {}}
-        self.vardescs = {}
-        self.discmap = {}
-        self.mdas = {}
-
-    def get_mda_attributes(self, group, tree, use_depth=False):
-        self._collect_disc_infos(self.problem.model, self.tree)
-        self._collect_var_infos(self.problem)
-
-        mda_attrs = self._get_mda_hierarchy(group, tree)
-
-        mda_attrs["name"] = ""  # root -> ""
-        self._populate_varattrs_from_connections(mda_attrs)
-        self._populate_varattrs_from_outputs(mda_attrs)
-        self._populate_initial_values(mda_attrs)
-        for _, mda in self.mdas.items():
-            self._populate_initial_values(mda)
-
-        mda_attrs["name"] = group.__class__.__name__
-
-        if use_depth:
-            cut(mda_attrs, self.depth)
-
-        return mda_attrs
-
-    def _get_mda_hierarchy(self, group, tree, group_prefix=""):
-        name = tree["name"]
-
-        mda_attrs = {
-            "name": name,
-            "disciplines_attributes": [
-                {"name": DRIVER_NAME, "variables_attributes": []}
-            ],
-        }
-        self.mdas[group_prefix] = mda_attrs
-        for child in tree["children"]:
-            for s in group._subsystems_myproc:
-                if s.name == child["name"]:
-                    if (
-                        child["type"] == "subsystem"
-                        and child["subsystem_type"] == "group"
-                    ):
-                        prefix = child["name"]
-                        if group_prefix:
-                            prefix = group_prefix + "." + child["name"]
-                        sub_analysis_attrs = self._get_sub_analysis_attributes(
-                            s, child, prefix
-                        )
-                        mda_attrs["disciplines_attributes"].append(sub_analysis_attrs)
-                    else:
-                        if not isinstance(s, IndepVarComp):
-                            discattrs = {
-                                "name": child["name"],
-                                "variables_attributes": [],
-                            }
-                            mda_attrs["disciplines_attributes"].append(discattrs)
-
-        return mda_attrs
-
-    def _populate_varattrs_from_connections(self, mda_attrs):
-        for conn in self.connections:
-            mda_src, varname_src = extract_mda_var(conn["src"])
-            mda_tgt, varname_tgt = extract_mda_var(conn["tgt"])
-            hat = []
-            while mda_src and mda_tgt and mda_src[0] == mda_tgt[0]:
-                hat.append(mda_src[0])
-                mda_src = mda_src[1:]
-                mda_tgt = mda_tgt[1:]
-            conn_name = self._get_conn_name(conn)
-            for discattrs in self.mdas[".".join(hat)]["disciplines_attributes"]:
-                # mda hat: src
-                if (
-                    mda_src[0] != AUTO_IVC
-                    and self.discmap[mda_src[0]] == discattrs["name"]
-                ):
-                    self._set_varattr(
-                        discattrs, conn["src"], varname_src, conn_name, "out"
-                    )
-                    # src -> hat
-                    self._set_varattr_in_depth(
-                        discattrs.get("sub_analysis_attributes"),
-                        mda_src[1:],
-                        conn["src"],
-                        conn_name,
-                        upward=True,
-                    )
-
-                # mda hat: tgt
-                if self.discmap[mda_tgt[0]] == discattrs["name"]:
-                    self._set_varattr(
-                        discattrs, conn["tgt"], varname_tgt, conn_name, "in"
-                    )
-                    if mda_src[0] == AUTO_IVC:
-                        driver_attrs = mda_attrs["disciplines_attributes"][0]
-                        self._set_varattr(
-                            driver_attrs, conn["src"], varname_tgt, conn_name, "out"
-                        )
-
-                    # hat -> tgt
-                    self._set_varattr_in_depth(
-                        discattrs.get("sub_analysis_attributes"),
-                        mda_tgt[1:],
-                        conn["tgt"],
-                        conn_name,
-                        upward=False,
-                    )
-
-    def _populate_varattrs_from_outputs(self, mda_attrs, group_prefix=""):
-        mda_prefix = group_prefix
-        if mda_prefix:
-            mda_prefix += "."
-        if mda_attrs["name"]:
-            mda_prefix += mda_attrs["name"] + "."
-        for discattrs in mda_attrs["disciplines_attributes"]:
-            sub_mda_attrs = discattrs.get("sub_analysis_attributes")
-            if sub_mda_attrs is None:
-                for absname, varattrs in self.vars["out"].items():
-                    mda, _ = extract_mda_var(absname)
-                    scope = discattrs["name"]
-                    if mda_prefix:
-                        scope = mda_prefix + scope
-                    if ".".join(mda).startswith(scope):
-                        vattr = {
-                            "name": varattrs["name"],
-                            "desc": self.vardescs.get(absname, ""),
-                            "type": varattrs["type"],
-                            "shape": varattrs["shape"],
-                            "units": varattrs["units"],
-                        }
-                        self._set_varattrs_from_outputs(
-                            vattr, "out", discattrs["variables_attributes"]
-                        )
-                        dvattr = vattr.copy()
-                        dvattr["io_mode"] = "in"
-                        driver_attrs = mda_attrs["disciplines_attributes"][0]
-                        self._set_varattrs_from_outputs(
-                            dvattr, "in", driver_attrs["variables_attributes"]
-                        )
-            else:
-                self._populate_varattrs_from_outputs(sub_mda_attrs, mda_prefix[:-1])
-
-    def _populate_initial_values(self, mda_attrs):
-        driver_attrs = mda_attrs["disciplines_attributes"][0]
-        for vattr in driver_attrs["variables_attributes"]:
-            if vattr["io_mode"] == "out":
-                # set init value for design variables and parameters (outputs of driver)
-                conn_name = vattr["name"].split("==")[0]
-                if self.vars["out"].get(conn_name):
-                    v = self.vars["out"][conn_name]
-                    vattr["parameter_attributes"] = {"init": simple_value(v)}
-                else:  # indep comp promoted
-                    for _, v in self.vars["out"].items():
-                        if conn_name == v["name"]:
-                            vattr["parameter_attributes"] = {"init": simple_value(v)}
-                            break
-
-    def _set_varattr_in_depth(
-        self, mda_attrs, mda_endpoint, endpoint, conn_name, upward
-    ):
-        if mda_attrs:
-            io_mode = "out" if upward else "in"
-            var = self.vars[io_mode][endpoint]
-            varattrs = {
-                "name": conn_name,
-                "io_mode": io_mode,
-                "desc": self.vardescs.get(endpoint, ""),
-                "type": var["type"],
-                "shape": var["shape"],
-                "units": var["units"],
-            }
-            disc_endpoint = mda_endpoint[0]
-            for discattrs in mda_attrs["disciplines_attributes"]:
-                if self.discmap[disc_endpoint] == discattrs["name"]:
-                    if discattrs.get("variables_attributes") is not None:
-                        already_present = [
-                            varattr["name"]
-                            for varattr in discattrs["variables_attributes"]
-                        ]
-                        if conn_name not in already_present:
-                            discattrs["variables_attributes"].append(varattrs)
-                    submda_attrs = discattrs.get("sub_analysis_attributes")
-                    break
-            driver_varattrs = mda_attrs["disciplines_attributes"][0][
-                "variables_attributes"
-            ]
-            already_present = [varattr["name"] for varattr in driver_varattrs]
-            if conn_name not in already_present:
-                varattr_driver = varattrs.copy()
-                varattr_driver["io_mode"] = "in" if upward else "out"
-                driver_varattrs.append(varattr_driver)
-            self._set_varattr_in_depth(
-                submda_attrs, mda_endpoint[1:], endpoint, conn_name, upward
-            )
-
-    def _set_varattr(self, discattrs, endpoint, varname, conn_name, io_mode):
-        if discattrs.get("variables_attributes") is None:
-            return
-        already_present = [
-            varattr["name"] for varattr in discattrs["variables_attributes"]
-        ]
-        if conn_name not in already_present:
-            var = self.vars[io_mode][endpoint]
-            discattrs["variables_attributes"].append(
-                {
-                    "name": conn_name,
-                    "io_mode": io_mode,
-                    "desc": self.vardescs.get(endpoint, ""),
-                    "type": var["type"],
-                    "shape": var["shape"],
-                    "units": var["units"],
-                }
-            )
-
-    def _set_varattrs_from_outputs(self, varattr, io_mode, varattrs):
-        already_present = [varattr["name"] for varattr in varattrs]
-        if varattr["name"] not in already_present:
-            vattr = varattr.copy()
-            vattr["io_mode"] = io_mode
-            varattrs.append(vattr)
-
-    def _get_conn_name(self, conn):
-        if (
-            self.vars["out"][conn["src"]]["name"]
-            == self.vars["in"][conn["tgt"]]["name"]
-        ):
-            return self.vars["out"][conn["src"]]["name"]
-        elif conn["src"].startswith(
-            AUTO_IVC
-        ):  # special case take varname of target when auto_ivc
-            _, varname = extract_mda_var(conn["tgt"])
-            return varname
-        else:
-            return build_variable_name(conn["src"], conn["tgt"], limit=255)
-
-    def _get_sub_analysis_attributes(self, group, child, prefix):
-        submda_attrs = self._get_mda_hierarchy(group, child, prefix)
-        submda_attrs["name"] = child["name"]
-        submda_attrs["disciplines_attributes"] = submda_attrs["disciplines_attributes"]
-        self.mdas[prefix] = submda_attrs
-        superdisc_attrs = {
-            "name": child["name"],
-            # "variables_attributes": [],
-            "sub_analysis_attributes": submda_attrs,
-        }
-        return superdisc_attrs
-
-    # see _get_tree_dict at
-    # https://github.com/OpenMDAO/OpenMDAO/blob/master/openmdao/visualization/n2_viewer/n2_viewer.py
-    def _collect_disc_infos(self, system, tree):
-        if "children" not in tree:
-            return
-
-        for child in tree["children"]:
-            for s in system._subsystems_myproc:
-                if s.name == child["name"]:
-                    if (
-                        child["type"] == "subsystem"
-                        and child["subsystem_type"] == "group"
-                    ):
-                        self.discmap[child["name"]] = child["name"]
-                        self._collect_disc_infos(s, child)
-                    else:
-                        # do not represent IndepVarComp
-                        if isinstance(s, IndepVarComp):
-                            self.discmap[child["name"]] = DRIVER_NAME
-                        else:
-                            self.discmap[child["name"]] = child["name"]
-
-    # see _get_tree_dict at
-    # https://github.com/OpenMDAO/OpenMDAO/blob/master/openmdao/visualization/n2_viewer/n2_viewer.py
-    def _collect_var_infos(self, problem):
-        system = problem.model
-        for io in ("input", "output"):
-            for abs_name in system._var_abs2meta[io]:
-                if io == "input":
-                    io_mode = "in"
-                elif io == "output":
-                    io_mode = "out"
-                else:
-                    raise Exception("Unhandled variable type " + io)
-                meta = system._var_abs2meta[io][abs_name]
-
-                vtype = "Float"
-                val = meta.get("value", meta.get("val"))  # fix OpenMDAO < 3.10
-                if re.match("int", type(val).__name__):
-                    vtype = "Integer"
-                shape = str(meta["shape"])
-                shape = format_shape(self.scalar, shape)
-                name = system._var_abs2prom[io][abs_name]
-                # name = abs_name
-                if abs_name.startswith(AUTO_IVC):
-                    name = find_indep_var_name(problem, abs_name)
-                self.vars[io_mode][abs_name] = {
-                    "name": name,
-                    "type": vtype,
-                    "shape": shape,
-                    "units": meta["units"],
-                    "value": val,
-                }
-
-                # retrieve initial conditions
-                var = self.vars[io_mode][abs_name]
-                if abs_name in system._outputs._views:
-                    var["value"] = system._outputs[abs_name]
-                elif abs_name in system._inputs._views:
-                    var["value"] = system._inputs[abs_name]
-                elif abs_name in system._discrete_outputs:
-                    var["value"] = system._discrete_outputs[abs_name]
-                elif abs_name in system._discrete_inputs:
-                    var["value"] = system._discrete_inputs[abs_name]
-
-                desc = self.vardescs.setdefault(name, "")
-                if desc == "":
-                    self.vardescs[name] = meta["desc"]
-                elif desc != meta["desc"] and meta["desc"] != "":
-                    debug(
-                        'Find another description for {}: "{}", keep "{}"'.format(
-                            name, meta["desc"], self.vardescs[name]
-                        )
-                    )
+import re
+from itertools import chain
+from whatsopt.push_utils import (
+    build_variable_name,
+    cut,
+    find_indep_var_name,
+    simple_value,
+    extract_mda_var,
+    format_shape,
+)
+from whatsopt.logging import debug
+from openmdao.api import IndepVarComp
+
+from openmdao.visualization.n2_viewer.n2_viewer import _get_viewer_data
+
+# Special name for internal WhatsOpt discipline. cf. WhatsOpt Discipline model
+DRIVER_NAME = "__DRIVER__"
+# OpenMDAO 3.2+ component name (handles indep vars automatically)
+AUTO_IVC = "_auto_ivc"
+
+
+class PushCommand:
+    """
+    This push command allows to push any OpenMDAO problem
+    (as opposed to regular push command which works with "all vars promoted/no connect" assumption)
+    """
+
+    def __init__(self, problem, depth, scalar):
+        data = _get_viewer_data(problem)
+        self.problem = problem
+        self.depth = depth
+        self.scalar = scalar
+        self.tree = data["tree"]
+        self.connections = data["connections_list"]
+        self.vars = {"in": {}, "out": {}}
+        self.vardescs = {}
+        self.discmap = {}
+        self.mdas = {}
+
+    def get_mda_attributes(self, group, tree, use_depth=False):
+        self._collect_disc_infos(self.problem.model, self.tree)
+        self._collect_var_infos(self.problem)
+
+        mda_attrs = self._get_mda_hierarchy(group, tree)
+
+        mda_attrs["name"] = ""  # root -> ""
+        self._populate_varattrs_from_connections(mda_attrs)
+        self._populate_varattrs_from_outputs(mda_attrs)
+        self._populate_initial_values(mda_attrs)
+        for _, mda in self.mdas.items():
+            self._populate_initial_values(mda)
+
+        mda_attrs["name"] = group.__class__.__name__
+
+        if use_depth:
+            cut(mda_attrs, self.depth)
+
+        return mda_attrs
+
+    def _get_mda_hierarchy(self, group, tree, group_prefix=""):
+        name = tree["name"]
+
+        mda_attrs = {
+            "name": name,
+            "disciplines_attributes": [
+                {"name": DRIVER_NAME, "variables_attributes": []}
+            ],
+        }
+        self.mdas[group_prefix] = mda_attrs
+        for child in tree["children"]:
+            for s in group._subsystems_myproc:
+                if s.name == child["name"]:
+                    if (
+                        child["type"] == "subsystem"
+                        and child["subsystem_type"] == "group"
+                    ):
+                        prefix = child["name"]
+                        if group_prefix:
+                            prefix = group_prefix + "." + child["name"]
+                        sub_analysis_attrs = self._get_sub_analysis_attributes(
+                            s, child, prefix
+                        )
+                        mda_attrs["disciplines_attributes"].append(sub_analysis_attrs)
+                    else:
+                        if not isinstance(s, IndepVarComp):
+                            discattrs = {
+                                "name": child["name"],
+                                "variables_attributes": [],
+                            }
+                            mda_attrs["disciplines_attributes"].append(discattrs)
+
+        return mda_attrs
+
+    def _populate_varattrs_from_connections(self, mda_attrs):
+        for conn in self.connections:
+            mda_src, varname_src = extract_mda_var(conn["src"])
+            mda_tgt, varname_tgt = extract_mda_var(conn["tgt"])
+            hat = []
+            while mda_src and mda_tgt and mda_src[0] == mda_tgt[0]:
+                hat.append(mda_src[0])
+                mda_src = mda_src[1:]
+                mda_tgt = mda_tgt[1:]
+            conn_name = self._get_conn_name(conn)
+            for discattrs in self.mdas[".".join(hat)]["disciplines_attributes"]:
+                # mda hat: src
+                if (
+                    mda_src[0] != AUTO_IVC
+                    and self.discmap[mda_src[0]] == discattrs["name"]
+                ):
+                    self._set_varattr(
+                        discattrs, conn["src"], varname_src, conn_name, "out"
+                    )
+                    # src -> hat
+                    self._set_varattr_in_depth(
+                        discattrs.get("sub_analysis_attributes"),
+                        mda_src[1:],
+                        conn["src"],
+                        conn_name,
+                        upward=True,
+                    )
+
+                # mda hat: tgt
+                if self.discmap[mda_tgt[0]] == discattrs["name"]:
+                    self._set_varattr(
+                        discattrs, conn["tgt"], varname_tgt, conn_name, "in"
+                    )
+                    if mda_src[0] == AUTO_IVC:
+                        driver_attrs = mda_attrs["disciplines_attributes"][0]
+                        self._set_varattr(
+                            driver_attrs, conn["src"], varname_tgt, conn_name, "out"
+                        )
+
+                    # hat -> tgt
+                    self._set_varattr_in_depth(
+                        discattrs.get("sub_analysis_attributes"),
+                        mda_tgt[1:],
+                        conn["tgt"],
+                        conn_name,
+                        upward=False,
+                    )
+
+    def _populate_varattrs_from_outputs(self, mda_attrs, group_prefix=""):
+        mda_prefix = group_prefix
+        if mda_prefix:
+            mda_prefix += "."
+        if mda_attrs["name"]:
+            mda_prefix += mda_attrs["name"] + "."
+        for discattrs in mda_attrs["disciplines_attributes"]:
+            sub_mda_attrs = discattrs.get("sub_analysis_attributes")
+            if sub_mda_attrs is None:
+                for absname, varattrs in self.vars["out"].items():
+                    mda, _ = extract_mda_var(absname)
+                    scope = discattrs["name"]
+                    if mda_prefix:
+                        scope = mda_prefix + scope
+                    if ".".join(mda).startswith(scope):
+                        vattr = {
+                            "name": varattrs["name"],
+                            "desc": self.vardescs.get(absname, ""),
+                            "type": varattrs["type"],
+                            "shape": varattrs["shape"],
+                            "units": varattrs["units"],
+                        }
+                        self._set_varattrs_from_outputs(
+                            vattr, "out", discattrs["variables_attributes"]
+                        )
+                        dvattr = vattr.copy()
+                        dvattr["io_mode"] = "in"
+                        driver_attrs = mda_attrs["disciplines_attributes"][0]
+                        self._set_varattrs_from_outputs(
+                            dvattr, "in", driver_attrs["variables_attributes"]
+                        )
+            else:
+                self._populate_varattrs_from_outputs(sub_mda_attrs, mda_prefix[:-1])
+
+    def _populate_initial_values(self, mda_attrs):
+        driver_attrs = mda_attrs["disciplines_attributes"][0]
+        for vattr in driver_attrs["variables_attributes"]:
+            if vattr["io_mode"] == "out":
+                # set init value for design variables and parameters (outputs of driver)
+                conn_name = vattr["name"].split("==")[0]
+                if self.vars["out"].get(conn_name):
+                    v = self.vars["out"][conn_name]
+                    vattr["parameter_attributes"] = {"init": simple_value(v)}
+                else:  # indep comp promoted
+                    for _, v in self.vars["out"].items():
+                        if conn_name == v["name"]:
+                            vattr["parameter_attributes"] = {"init": simple_value(v)}
+                            break
+
+    def _set_varattr_in_depth(
+        self, mda_attrs, mda_endpoint, endpoint, conn_name, upward
+    ):
+        if mda_attrs:
+            io_mode = "out" if upward else "in"
+            var = self.vars[io_mode][endpoint]
+            varattrs = {
+                "name": conn_name,
+                "io_mode": io_mode,
+                "desc": self.vardescs.get(endpoint, ""),
+                "type": var["type"],
+                "shape": var["shape"],
+                "units": var["units"],
+            }
+            disc_endpoint = mda_endpoint[0]
+            for discattrs in mda_attrs["disciplines_attributes"]:
+                if self.discmap[disc_endpoint] == discattrs["name"]:
+                    if discattrs.get("variables_attributes") is not None:
+                        already_present = [
+                            varattr["name"]
+                            for varattr in discattrs["variables_attributes"]
+                        ]
+                        if conn_name not in already_present:
+                            discattrs["variables_attributes"].append(varattrs)
+                    submda_attrs = discattrs.get("sub_analysis_attributes")
+                    break
+            driver_varattrs = mda_attrs["disciplines_attributes"][0][
+                "variables_attributes"
+            ]
+            already_present = [varattr["name"] for varattr in driver_varattrs]
+            if conn_name not in already_present:
+                varattr_driver = varattrs.copy()
+                varattr_driver["io_mode"] = "in" if upward else "out"
+                driver_varattrs.append(varattr_driver)
+            self._set_varattr_in_depth(
+                submda_attrs, mda_endpoint[1:], endpoint, conn_name, upward
+            )
+
+    def _set_varattr(self, discattrs, endpoint, varname, conn_name, io_mode):
+        if discattrs.get("variables_attributes") is None:
+            return
+        already_present = [
+            varattr["name"] for varattr in discattrs["variables_attributes"]
+        ]
+        if conn_name not in already_present:
+            var = self.vars[io_mode][endpoint]
+            discattrs["variables_attributes"].append(
+                {
+                    "name": conn_name,
+                    "io_mode": io_mode,
+                    "desc": self.vardescs.get(endpoint, ""),
+                    "type": var["type"],
+                    "shape": var["shape"],
+                    "units": var["units"],
+                }
+            )
+
+    def _set_varattrs_from_outputs(self, varattr, io_mode, varattrs):
+        already_present = [varattr["name"] for varattr in varattrs]
+        if varattr["name"] not in already_present:
+            vattr = varattr.copy()
+            vattr["io_mode"] = io_mode
+            varattrs.append(vattr)
+
+    def _get_conn_name(self, conn):
+        if (
+            self.vars["out"][conn["src"]]["name"]
+            == self.vars["in"][conn["tgt"]]["name"]
+        ):
+            return self.vars["out"][conn["src"]]["name"]
+        elif conn["src"].startswith(
+            AUTO_IVC
+        ):  # special case take varname of target when auto_ivc
+            _, varname = extract_mda_var(conn["tgt"])
+            return varname
+        else:
+            return build_variable_name(conn["src"], conn["tgt"], limit=255)
+
+    def _get_sub_analysis_attributes(self, group, child, prefix):
+        submda_attrs = self._get_mda_hierarchy(group, child, prefix)
+        submda_attrs["name"] = child["name"]
+        submda_attrs["disciplines_attributes"] = submda_attrs["disciplines_attributes"]
+        self.mdas[prefix] = submda_attrs
+        superdisc_attrs = {
+            "name": child["name"],
+            # "variables_attributes": [],
+            "sub_analysis_attributes": submda_attrs,
+        }
+        return superdisc_attrs
+
+    # see _get_tree_dict at
+    # https://github.com/OpenMDAO/OpenMDAO/blob/master/openmdao/visualization/n2_viewer/n2_viewer.py
+    def _collect_disc_infos(self, system, tree):
+        if "children" not in tree:
+            return
+
+        for child in tree["children"]:
+            for s in system._subsystems_myproc:
+                if s.name == child["name"]:
+                    if (
+                        child["type"] == "subsystem"
+                        and child["subsystem_type"] == "group"
+                    ):
+                        self.discmap[child["name"]] = child["name"]
+                        self._collect_disc_infos(s, child)
+                    else:
+                        # do not represent IndepVarComp
+                        if isinstance(s, IndepVarComp):
+                            self.discmap[child["name"]] = DRIVER_NAME
+                        else:
+                            self.discmap[child["name"]] = child["name"]
+
+    # see _get_tree_dict at
+    # https://github.com/OpenMDAO/OpenMDAO/blob/master/openmdao/visualization/n2_viewer/n2_viewer.py
+    def _collect_var_infos(self, problem):
+        system = problem.model
+        for io in ("input", "output"):
+            for abs_name in system._var_abs2meta[io]:
+                if io == "input":
+                    io_mode = "in"
+                elif io == "output":
+                    io_mode = "out"
+                else:
+                    raise Exception("Unhandled variable type " + io)
+                meta = system._var_abs2meta[io][abs_name]
+
+                vtype = "Float"
+                val = meta.get("value", meta.get("val"))  # fix OpenMDAO < 3.10
+                if re.match("int", type(val).__name__):
+                    vtype = "Integer"
+                shape = str(meta["shape"])
+                shape = format_shape(self.scalar, shape)
+                name = system._var_abs2prom[io][abs_name]
+                # name = abs_name
+                if abs_name.startswith(AUTO_IVC):
+                    name = find_indep_var_name(problem, abs_name)
+                self.vars[io_mode][abs_name] = {
+                    "name": name,
+                    "type": vtype,
+                    "shape": shape,
+                    "units": meta["units"],
+                    "value": val,
+                }
+
+                # retrieve initial conditions
+                var = self.vars[io_mode][abs_name]
+                if abs_name in system._outputs._views:
+                    var["value"] = system._outputs[abs_name]
+                elif abs_name in system._inputs._views:
+                    var["value"] = system._inputs[abs_name]
+                elif abs_name in system._discrete_outputs:
+                    var["value"] = system._discrete_outputs[abs_name]
+                elif abs_name in system._discrete_inputs:
+                    var["value"] = system._discrete_inputs[abs_name]
+
+                desc = self.vardescs.setdefault(name, "")
+                if desc == "":
+                    self.vardescs[name] = meta["desc"]
+                elif desc != meta["desc"] and meta["desc"] != "":
+                    debug(
+                        'Find another description for {}: "{}", keep "{}"'.format(
+                            name, meta["desc"], self.vardescs[name]
+                        )
+                    )
```

### Comparing `wop-2.5.2/whatsopt/push_utils.py` & `wop-2.5.3/whatsopt/push_utils.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-import re
-import os
-import tempfile
-from contextlib import contextmanager
-
-
-def cut(mda_attrs, depth):
-    if depth <= 0:
-        return mda_attrs
-    elif depth == 1:
-        flatten(mda_attrs)
-    else:
-        for disc in mda_attrs["disciplines_attributes"]:
-            sub_mdattrs = disc.get("sub_analysis_attributes")
-            if sub_mdattrs:
-                cut(sub_mdattrs, depth - 1)
-
-
-def flatten(mda_attrs):
-    # print("-------- flatten ", mda_attrs["name"])
-    for disc in mda_attrs["disciplines_attributes"]:
-        # print("************** ", disc["name"])
-        sub_mdattrs = disc.get("sub_analysis_attributes")
-        if sub_mdattrs:
-            varattrs = disc.get("variables_attributes", [])
-            subdriver = sub_mdattrs["disciplines_attributes"][0]
-            # print("<<<< DRIVER ", subdriver["variables_attributes"])
-            for vattr in subdriver["variables_attributes"]:
-                v = vattr.copy()
-                v["io_mode"] = "out" if vattr["io_mode"] == "in" else "in"
-                varattrs.append(v)
-            del disc["sub_analysis_attributes"]
-            disc["variables_attributes"] = varattrs
-            # print(">>>>", disc["name"])
-            # print(disc["variables_attributes"])
-
-            driver = mda_attrs["disciplines_attributes"][0]
-            for vattr in subdriver["variables_attributes"]:
-                already_present = [v["name"] for v in driver["variables_attributes"]]
-                if vattr["name"] not in already_present:
-                    v = vattr.copy()
-                    # print("ADD DRIVER of ", mda_attrs["name"], v)
-                    driver["variables_attributes"].append(v)
-
-
-# push_command collect_var_infos
-def format_shape(scalar, shape):
-    shape = shape.replace("L", "")  # with py27 we can get (1L,)
-    if scalar and shape == "(1,)":
-        shape = "1"
-    return shape
-
-
-# push_command _get_sub_analysis_attributes & wop _get_discipline_attributes
-def to_camelcase(name):
-    return re.sub(r"(?:^|_)(\w)", lambda x: x.group(1).upper(), name)
-
-
-# push_command get_mda_attributes
-def simple_value(var):
-    typ = var["type"]
-    if var["shape"] == "1" or var["shape"] == "(1,)":
-        ret = float(var["value"])
-        if typ == "Integer":
-            ret = int(ret)
-    else:
-        if typ == "Integer":
-            var["value"] = var["value"].astype(int)
-        else:
-            var["value"] = var["value"].astype(float)
-        ret = var["value"].tolist()
-    return str(ret)
-
-
-# push_command _get_varattr_from_connection
-def extract_mda_var(fullname):
-    name_elts = fullname.split(".")
-    if len(name_elts) > 1:
-        mda, var = name_elts[:-1], name_elts[-1]
-    else:
-        raise Exception(
-            "Connection qualified name should contain"
-            + " at least one dot, but got %s" % fullname
-        )
-    return mda, var
-
-
-@contextmanager
-def problem_pyfile(py_filename, component):
-    dirname = os.path.dirname(py_filename)
-    filename = os.path.basename(py_filename)
-    module = os.path.splitext(filename)[0]
-    content = """from openmdao.api import Problem, Group, IndepVarComp
-from {} import {}
-
-comp = {}()
-comp_name = "{}"
-
-
-class {}ComponentDiscovery(Group):
-    pass
-
-
-class {}Component(Group):
-    pass
-
-
-model_discovery = {}ComponentDiscovery()
-model_discovery.add_subsystem(comp_name, comp, promotes=["*"])
-pb_discovery = Problem(model_discovery)
-pb_discovery.setup()
-
-
-inputs = comp.list_inputs(out_stream=None)
-indeps = IndepVarComp()
-for name, meta in inputs:
-    args = {{
-        "val": meta.get("value", meta.get("val")),   # fix OpenMDAO < 3.10
-        "shape": meta.get("shape"),
-        "desc": meta.get("desc", ""),
-        "units": meta.get("units", None)
-    }}
-    indeps.add_output(name, **args)
-
-model = {}Component()
-model.add_subsystem("indeps", indeps, promotes=["*"])
-model.add_subsystem(comp_name, comp, promotes=["*"])
-pb = Problem(model)
-pb.setup()
-pb.final_setup()
-""".format(
-        module,
-        component,
-        component,
-        component,
-        component,
-        component,
-        component,
-        component,
-    )
-    handle, pbfile = tempfile.mkstemp(suffix=".py", dir=dirname)
-    os.close(handle)
-    with open(pbfile, "w") as pbf:
-        pbf.write(content)
-
-    try:
-        yield pbfile
-    finally:
-        os.unlink(pbfile)
-
-
-def find_indep_var_name(pb, absname):
-    target = None
-    for tgt, src in pb.model._conn_global_abs_in2out.items():
-        if src == absname:
-            target = tgt
-            break
-    return pb.model._var_abs2prom["input"].get(target)
-
-
-def build_variable_name(varname1, varname2, limit=255):
-    varname_sep = "=="
-    ellipsis_sep = "..."
-
-    name = varname1 + "==" + varname2
-    ellipsed_name = name
-    if len(name) <= limit or limit < len(varname_sep) + 2 * len(ellipsis_sep) + 4:
-        ellipsed_name = name
-    else:
-        half_limit = (limit - len(varname_sep)) // 2
-        ellipsed_name = (
-            _ellipsize(varname1, half_limit)
-            + varname_sep
-            + _ellipsize(varname2, half_limit)
-        )
-
-    if len(ellipsed_name) > limit:
-        ellipsed_name = ellipsis_sep + varname2[-(limit - len(ellipsis_sep)) :]
-
-    return ellipsed_name
-
-
-def _ellipsize(name, limit):
-    ellipsis_sep = "..."
-
-    half_limit = (limit - len(ellipsis_sep)) // 2
-    if len(name) <= half_limit:
-        return name
-    else:
-        return name[:half_limit] + ellipsis_sep + name[-half_limit:]
+import re
+import os
+import tempfile
+from contextlib import contextmanager
+
+
+def cut(mda_attrs, depth):
+    if depth <= 0:
+        return mda_attrs
+    elif depth == 1:
+        flatten(mda_attrs)
+    else:
+        for disc in mda_attrs["disciplines_attributes"]:
+            sub_mdattrs = disc.get("sub_analysis_attributes")
+            if sub_mdattrs:
+                cut(sub_mdattrs, depth - 1)
+
+
+def flatten(mda_attrs):
+    # print("-------- flatten ", mda_attrs["name"])
+    for disc in mda_attrs["disciplines_attributes"]:
+        # print("************** ", disc["name"])
+        sub_mdattrs = disc.get("sub_analysis_attributes")
+        if sub_mdattrs:
+            varattrs = disc.get("variables_attributes", [])
+            subdriver = sub_mdattrs["disciplines_attributes"][0]
+            # print("<<<< DRIVER ", subdriver["variables_attributes"])
+            for vattr in subdriver["variables_attributes"]:
+                v = vattr.copy()
+                v["io_mode"] = "out" if vattr["io_mode"] == "in" else "in"
+                varattrs.append(v)
+            del disc["sub_analysis_attributes"]
+            disc["variables_attributes"] = varattrs
+            # print(">>>>", disc["name"])
+            # print(disc["variables_attributes"])
+
+            driver = mda_attrs["disciplines_attributes"][0]
+            for vattr in subdriver["variables_attributes"]:
+                already_present = [v["name"] for v in driver["variables_attributes"]]
+                if vattr["name"] not in already_present:
+                    v = vattr.copy()
+                    # print("ADD DRIVER of ", mda_attrs["name"], v)
+                    driver["variables_attributes"].append(v)
+
+
+# push_command collect_var_infos
+def format_shape(scalar, shape):
+    shape = shape.replace("L", "")  # with py27 we can get (1L,)
+    if scalar and shape == "(1,)":
+        shape = "1"
+    return shape
+
+
+# push_command _get_sub_analysis_attributes & wop _get_discipline_attributes
+def to_camelcase(name):
+    return re.sub(r"(?:^|_)(\w)", lambda x: x.group(1).upper(), name)
+
+
+# push_command get_mda_attributes
+def simple_value(var):
+    typ = var["type"]
+    if var["shape"] == "1" or var["shape"] == "(1,)":
+        ret = float(var["value"])
+        if typ == "Integer":
+            ret = int(ret)
+    else:
+        if typ == "Integer":
+            var["value"] = var["value"].astype(int)
+        else:
+            var["value"] = var["value"].astype(float)
+        ret = var["value"].tolist()
+    return str(ret)
+
+
+# push_command _get_varattr_from_connection
+def extract_mda_var(fullname):
+    name_elts = fullname.split(".")
+    if len(name_elts) > 1:
+        mda, var = name_elts[:-1], name_elts[-1]
+    else:
+        raise Exception(
+            "Connection qualified name should contain"
+            + " at least one dot, but got %s" % fullname
+        )
+    return mda, var
+
+
+@contextmanager
+def problem_pyfile(py_filename, component):
+    dirname = os.path.dirname(py_filename)
+    filename = os.path.basename(py_filename)
+    module = os.path.splitext(filename)[0]
+    content = """from openmdao.api import Problem, Group, IndepVarComp
+from {} import {}
+
+comp = {}()
+comp_name = "{}"
+
+
+class {}ComponentDiscovery(Group):
+    pass
+
+
+class {}Component(Group):
+    pass
+
+
+model_discovery = {}ComponentDiscovery()
+model_discovery.add_subsystem(comp_name, comp, promotes=["*"])
+pb_discovery = Problem(model_discovery)
+pb_discovery.setup()
+
+
+inputs = comp.list_inputs(out_stream=None)
+indeps = IndepVarComp()
+for name, meta in inputs:
+    args = {{
+        "val": meta.get("value", meta.get("val")),   # fix OpenMDAO < 3.10
+        "shape": meta.get("shape"),
+        "desc": meta.get("desc", ""),
+        "units": meta.get("units", None)
+    }}
+    indeps.add_output(name, **args)
+
+model = {}Component()
+model.add_subsystem("indeps", indeps, promotes=["*"])
+model.add_subsystem(comp_name, comp, promotes=["*"])
+pb = Problem(model)
+pb.setup()
+pb.final_setup()
+""".format(
+        module,
+        component,
+        component,
+        component,
+        component,
+        component,
+        component,
+        component,
+    )
+    handle, pbfile = tempfile.mkstemp(suffix=".py", dir=dirname)
+    os.close(handle)
+    with open(pbfile, "w") as pbf:
+        pbf.write(content)
+
+    try:
+        yield pbfile
+    finally:
+        os.unlink(pbfile)
+
+
+def find_indep_var_name(pb, absname):
+    target = None
+    for tgt, src in pb.model._conn_global_abs_in2out.items():
+        if src == absname:
+            target = tgt
+            break
+    return pb.model._var_abs2prom["input"].get(target)
+
+
+def build_variable_name(varname1, varname2, limit=255):
+    varname_sep = "=="
+    ellipsis_sep = "..."
+
+    name = varname1 + "==" + varname2
+    ellipsed_name = name
+    if len(name) <= limit or limit < len(varname_sep) + 2 * len(ellipsis_sep) + 4:
+        ellipsed_name = name
+    else:
+        half_limit = (limit - len(varname_sep)) // 2
+        ellipsed_name = (
+            _ellipsize(varname1, half_limit)
+            + varname_sep
+            + _ellipsize(varname2, half_limit)
+        )
+
+    if len(ellipsed_name) > limit:
+        ellipsed_name = ellipsis_sep + varname2[-(limit - len(ellipsis_sep)) :]
+
+    return ellipsed_name
+
+
+def _ellipsize(name, limit):
+    ellipsis_sep = "..."
+
+    half_limit = (limit - len(ellipsis_sep)) // 2
+    if len(name) <= half_limit:
+        return name
+    else:
+        return name[:half_limit] + ellipsis_sep + name[-half_limit:]
```

### Comparing `wop-2.5.2/whatsopt/show_utils.py` & `wop-2.5.3/whatsopt/show_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,89 @@
 00000000: 6672 6f6d 2078 6473 6d6a 7320 696d 706f  from xdsmjs impo
 00000010: 7274 2062 756e 646c 656a 732c 2063 7373  rt bundlejs, css
-00000020: 0d0a 6672 6f6d 2064 6174 6574 696d 6520  ..from datetime 
-00000030: 696d 706f 7274 2064 6174 650d 0a0d 0a48  import date....H
-00000040: 544d 4c5f 5445 4d50 4c41 5445 203d 2022  TML_TEMPLATE = "
-00000050: 2222 0d0a 3c21 646f 6374 7970 6520 6874  ""..<!doctype ht
-00000060: 6d6c 3e0d 0a0d 0a3c 6865 6164 3e0d 0a3c  ml>....<head>..<
-00000070: 6d65 7461 2068 7474 702d 6571 7569 763d  meta http-equiv=
-00000080: 2243 6f6e 7465 6e74 2d54 7970 6522 2063  "Content-Type" c
-00000090: 6f6e 7465 6e74 3d22 7465 7874 2f68 746d  ontent="text/htm
-000000a0: 6c3b 2063 6861 7273 6574 3d55 5446 2d38  l; charset=UTF-8
-000000b0: 223e 0d0a 3c73 7479 6c65 2074 7970 653d  ">..<style type=
-000000c0: 2274 6578 742f 6373 7322 3e0d 0a7b 7d0d  "text/css">..{}.
-000000d0: 0a0d 0a2e 666f 6f74 6572 207b 7b0d 0a20  ....footer {{.. 
-000000e0: 2020 2066 6f6e 742d 7374 796c 653a 2069     font-style: i
-000000f0: 7461 6c69 633b 0d0a 2020 2020 666f 6e74  talic;..    font
-00000100: 2d73 697a 653a 2073 6d61 6c6c 3b0d 0a20  -size: small;.. 
-00000110: 2020 2070 6f73 6974 696f 6e3a 2061 6273     position: abs
-00000120: 6f6c 7574 653b 0d0a 2020 2020 7269 6768  olute;..    righ
-00000130: 743a 2032 3070 783b 0d0a 7d7d 0d0a 3c2f  t: 20px;..}}..</
-00000140: 7374 796c 653e 0d0a 3c73 6372 6970 7420  style>..<script 
-00000150: 7479 7065 3d22 7465 7874 2f6a 6176 6173  type="text/javas
-00000160: 6372 6970 7422 3e0d 0a7b 7d0d 0a3c 2f73  cript">..{}..</s
-00000170: 6372 6970 743e 0d0a 3c73 6372 6970 7420  cript>..<script 
-00000180: 7479 7065 3d22 7465 7874 2f6a 6176 6173  type="text/javas
-00000190: 6372 6970 7422 3e0d 0a20 2020 2064 6f63  cript">..    doc
-000001a0: 756d 656e 742e 6164 6445 7665 6e74 4c69  ument.addEventLi
-000001b0: 7374 656e 6572 2827 444f 4d43 6f6e 7465  stener('DOMConte
-000001c0: 6e74 4c6f 6164 6564 272c 2028 2920 3d3e  ntLoaded', () =>
-000001d0: 207b 7b0d 0a20 2020 2020 2063 6f6e 7374   {{..      const
-000001e0: 206d 646f 203d 207b 7d3b 0d0a 2020 2020   mdo = {};..    
-000001f0: 2020 636f 6e73 7420 636f 6e66 6967 203d    const config =
-00000200: 207b 7b0d 0a20 2020 2020 2020 206c 6162   {{..        lab
-00000210: 656c 697a 6572 3a20 7b7b 0d0a 2020 2020  elizer: {{..    
-00000220: 2020 2020 2020 2020 656c 6c69 7073 6973          ellipsis
-00000230: 3a20 352c 0d0a 2020 2020 2020 2020 2020  : 5,..          
-00000240: 2020 7375 6253 7570 5363 7269 7074 3a20    subSupScript: 
-00000250: 6661 6c73 652c 0d0a 2020 2020 2020 2020  false,..        
-00000260: 2020 2020 7368 6f77 4c69 6e6b 4e62 4f6e      showLinkNbOn
-00000270: 6c79 3a20 7472 7565 2c0d 0a20 2020 2020  ly: true,..     
-00000280: 2020 207d 7d2c 0d0a 2020 2020 2020 2020     }},..        
-00000290: 6c61 796f 7574 3a20 7b7b 0d0a 2020 2020  layout: {{..    
-000002a0: 2020 2020 2020 2020 6f72 6967 696e 3a20          origin: 
-000002b0: 7b7b 2078 3a20 3530 2c20 793a 2032 3020  {{ x: 50, y: 20 
-000002c0: 7d7d 2c0d 0a20 2020 2020 2020 2020 2020  }},..           
-000002d0: 2063 656c 6c73 697a 653a 207b 7b20 773a   cellsize: {{ w:
-000002e0: 2031 3530 2c20 683a 2035 3020 7d7d 2c0d   150, h: 50 }},.
-000002f0: 0a20 2020 2020 2020 2020 2020 2070 6164  .            pad
-00000300: 6469 6e67 3a20 3130 2c0d 0a20 2020 2020  ding: 10,..     
-00000310: 2020 207d 7d2c 0d0a 2020 2020 2020 2020     }},..        
-00000320: 7769 7468 4465 6661 756c 7444 7269 7665  withDefaultDrive
-00000330: 723a 2066 616c 7365 2c0d 0a20 2020 2020  r: false,..     
-00000340: 207d 7d3b 0d0a 2020 2020 2020 7864 736d   }};..      xdsm
-00000350: 6a73 2e58 4453 4d6a 7328 636f 6e66 6967  js.XDSMjs(config
-00000360: 292e 6372 6561 7465 5864 736d 286d 646f  ).createXdsm(mdo
-00000370: 293b 0d0a 2020 2020 7d7d 293b 0d0a 3c2f  );..    }});..</
-00000380: 7363 7269 7074 3e0d 0a3c 2f68 6561 643e  script>..</head>
-00000390: 0d0a 0d0a 3c62 6f64 793e 0d0a 2020 2020  ....<body>..    
-000003a0: 3c64 6976 2063 6c61 7373 3d22 7864 736d  <div class="xdsm
-000003b0: 2d74 6f6f 6c62 6172 223e 3c2f 6469 763e  -toolbar"></div>
-000003c0: 0d0a 2020 2020 3c64 6976 2063 6c61 7373  ..    <div class
-000003d0: 3d22 7864 736d 3222 3e3c 2f64 6976 3e0d  ="xdsm2"></div>.
-000003e0: 0a20 2020 203c 6872 3e0d 0a20 2020 203c  .    <hr>..    <
-000003f0: 6469 7620 636c 6173 733d 2266 6f6f 7465  div class="foote
-00000400: 7222 3e7b 7d3c 2f64 6976 3e0d 0a3c 2f62  r">{}</div>..</b
-00000410: 6f64 793e 0d0a 0d0a 3c2f 6874 6d6c 3e0d  ody>....</html>.
-00000420: 0a22 2222 0d0a 0d0a 0d0a 6465 6620 6765  ."""......def ge
-00000430: 6e65 7261 7465 5f78 6473 6d5f 6874 6d6c  nerate_xdsm_html
-00000440: 2873 6f75 7263 652c 2078 6473 6d2c 206f  (source, xdsm, o
-00000450: 7574 6669 6c65 6e61 6d65 3d22 7864 736d  utfilename="xdsm
-00000460: 2e68 746d 6c22 293a 0d0a 2020 2020 6874  .html"):..    ht
-00000470: 6d6c 203d 205f 6765 6e65 7261 7465 5f68  ml = _generate_h
-00000480: 746d 6c28 736f 7572 6365 2c20 7864 736d  tml(source, xdsm
-00000490: 290d 0a0d 0a20 2020 2077 6974 6820 6f70  )....    with op
-000004a0: 656e 286f 7574 6669 6c65 6e61 6d65 2c20  en(outfilename, 
-000004b0: 2277 2229 2061 7320 663a 0d0a 2020 2020  "w") as f:..    
-000004c0: 2020 2020 662e 7772 6974 6528 6874 6d6c      f.write(html
-000004d0: 290d 0a0d 0a0d 0a64 6566 205f 6765 6e65  )......def _gene
-000004e0: 7261 7465 5f68 746d 6c28 736f 7572 6365  rate_html(source
-000004f0: 2c20 7864 736d 293a 0d0a 2020 2020 666f  , xdsm):..    fo
-00000500: 6f74 6572 203d 2022 5844 534d 2067 656e  oter = "XDSM gen
-00000510: 6572 6174 6564 2066 726f 6d20 7b7d 2c20  erated from {}, 
-00000520: 7b7d 2c20 4f4e 4552 4120 5768 6174 734f  {}, ONERA WhatsO
-00000530: 7074 222e 666f 726d 6174 280d 0a20 2020  pt".format(..   
-00000540: 2020 2020 2073 6f75 7263 652c 2064 6174       source, dat
-00000550: 652e 746f 6461 7928 292e 7374 7266 7469  e.today().strfti
-00000560: 6d65 2822 2562 2025 642c 2025 5922 290d  me("%b %d, %Y").
-00000570: 0a20 2020 2029 0d0a 2020 2020 6874 6d6c  .    )..    html
-00000580: 203d 2048 544d 4c5f 5445 4d50 4c41 5445   = HTML_TEMPLATE
-00000590: 2e66 6f72 6d61 7428 6373 7328 292c 2062  .format(css(), b
-000005a0: 756e 646c 656a 7328 292c 2078 6473 6d2c  undlejs(), xdsm,
-000005b0: 2066 6f6f 7465 7229 0d0a 2020 2020 7265   footer)..    re
-000005c0: 7475 726e 2068 746d 6c0d 0a              turn html..
+00000020: 0a66 726f 6d20 6461 7465 7469 6d65 2069  .from datetime i
+00000030: 6d70 6f72 7420 6461 7465 0a0a 4854 4d4c  mport date..HTML
+00000040: 5f54 454d 504c 4154 4520 3d20 2222 220a  _TEMPLATE = """.
+00000050: 3c21 646f 6374 7970 6520 6874 6d6c 3e0a  <!doctype html>.
+00000060: 0a3c 6865 6164 3e0a 3c6d 6574 6120 6874  .<head>.<meta ht
+00000070: 7470 2d65 7175 6976 3d22 436f 6e74 656e  tp-equiv="Conten
+00000080: 742d 5479 7065 2220 636f 6e74 656e 743d  t-Type" content=
+00000090: 2274 6578 742f 6874 6d6c 3b20 6368 6172  "text/html; char
+000000a0: 7365 743d 5554 462d 3822 3e0a 3c73 7479  set=UTF-8">.<sty
+000000b0: 6c65 2074 7970 653d 2274 6578 742f 6373  le type="text/cs
+000000c0: 7322 3e0a 7b7d 0a0a 2e66 6f6f 7465 7220  s">.{}...footer 
+000000d0: 7b7b 0a20 2020 2066 6f6e 742d 7374 796c  {{.    font-styl
+000000e0: 653a 2069 7461 6c69 633b 0a20 2020 2066  e: italic;.    f
+000000f0: 6f6e 742d 7369 7a65 3a20 736d 616c 6c3b  ont-size: small;
+00000100: 0a20 2020 2070 6f73 6974 696f 6e3a 2061  .    position: a
+00000110: 6273 6f6c 7574 653b 0a20 2020 2072 6967  bsolute;.    rig
+00000120: 6874 3a20 3230 7078 3b0a 7d7d 0a3c 2f73  ht: 20px;.}}.</s
+00000130: 7479 6c65 3e0a 3c73 6372 6970 7420 7479  tyle>.<script ty
+00000140: 7065 3d22 7465 7874 2f6a 6176 6173 6372  pe="text/javascr
+00000150: 6970 7422 3e0a 7b7d 0a3c 2f73 6372 6970  ipt">.{}.</scrip
+00000160: 743e 0a3c 7363 7269 7074 2074 7970 653d  t>.<script type=
+00000170: 2274 6578 742f 6a61 7661 7363 7269 7074  "text/javascript
+00000180: 223e 0a20 2020 2064 6f63 756d 656e 742e  ">.    document.
+00000190: 6164 6445 7665 6e74 4c69 7374 656e 6572  addEventListener
+000001a0: 2827 444f 4d43 6f6e 7465 6e74 4c6f 6164  ('DOMContentLoad
+000001b0: 6564 272c 2028 2920 3d3e 207b 7b0a 2020  ed', () => {{.  
+000001c0: 2020 2020 636f 6e73 7420 6d64 6f20 3d20      const mdo = 
+000001d0: 7b7d 3b0a 2020 2020 2020 636f 6e73 7420  {};.      const 
+000001e0: 636f 6e66 6967 203d 207b 7b0a 2020 2020  config = {{.    
+000001f0: 2020 2020 6c61 6265 6c69 7a65 723a 207b      labelizer: {
+00000200: 7b0a 2020 2020 2020 2020 2020 2020 656c  {.            el
+00000210: 6c69 7073 6973 3a20 352c 0a20 2020 2020  lipsis: 5,.     
+00000220: 2020 2020 2020 2073 7562 5375 7053 6372         subSupScr
+00000230: 6970 743a 2066 616c 7365 2c0a 2020 2020  ipt: false,.    
+00000240: 2020 2020 2020 2020 7368 6f77 4c69 6e6b          showLink
+00000250: 4e62 4f6e 6c79 3a20 7472 7565 2c0a 2020  NbOnly: true,.  
+00000260: 2020 2020 2020 7d7d 2c0a 2020 2020 2020        }},.      
+00000270: 2020 6c61 796f 7574 3a20 7b7b 0a20 2020    layout: {{.   
+00000280: 2020 2020 2020 2020 206f 7269 6769 6e3a           origin:
+00000290: 207b 7b20 783a 2035 302c 2079 3a20 3230   {{ x: 50, y: 20
+000002a0: 207d 7d2c 0a20 2020 2020 2020 2020 2020   }},.           
+000002b0: 2063 656c 6c73 697a 653a 207b 7b20 773a   cellsize: {{ w:
+000002c0: 2031 3530 2c20 683a 2035 3020 7d7d 2c0a   150, h: 50 }},.
+000002d0: 2020 2020 2020 2020 2020 2020 7061 6464              padd
+000002e0: 696e 673a 2031 302c 0a20 2020 2020 2020  ing: 10,.       
+000002f0: 207d 7d2c 0a20 2020 2020 2020 2077 6974   }},.        wit
+00000300: 6844 6566 6175 6c74 4472 6976 6572 3a20  hDefaultDriver: 
+00000310: 6661 6c73 652c 0a20 2020 2020 207d 7d3b  false,.      }};
+00000320: 0a20 2020 2020 2078 6473 6d6a 732e 5844  .      xdsmjs.XD
+00000330: 534d 6a73 2863 6f6e 6669 6729 2e63 7265  SMjs(config).cre
+00000340: 6174 6558 6473 6d28 6d64 6f29 3b0a 2020  ateXdsm(mdo);.  
+00000350: 2020 7d7d 293b 0a3c 2f73 6372 6970 743e    }});.</script>
+00000360: 0a3c 2f68 6561 643e 0a0a 3c62 6f64 793e  .</head>..<body>
+00000370: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
+00000380: 2278 6473 6d2d 746f 6f6c 6261 7222 3e3c  "xdsm-toolbar"><
+00000390: 2f64 6976 3e0a 2020 2020 3c64 6976 2063  /div>.    <div c
+000003a0: 6c61 7373 3d22 7864 736d 3222 3e3c 2f64  lass="xdsm2"></d
+000003b0: 6976 3e0a 2020 2020 3c68 723e 0a20 2020  iv>.    <hr>.   
+000003c0: 203c 6469 7620 636c 6173 733d 2266 6f6f   <div class="foo
+000003d0: 7465 7222 3e7b 7d3c 2f64 6976 3e0a 3c2f  ter">{}</div>.</
+000003e0: 626f 6479 3e0a 0a3c 2f68 746d 6c3e 0a22  body>..</html>."
+000003f0: 2222 0a0a 0a64 6566 2067 656e 6572 6174  ""...def generat
+00000400: 655f 7864 736d 5f68 746d 6c28 736f 7572  e_xdsm_html(sour
+00000410: 6365 2c20 7864 736d 2c20 6f75 7466 696c  ce, xdsm, outfil
+00000420: 656e 616d 653d 2278 6473 6d2e 6874 6d6c  ename="xdsm.html
+00000430: 2229 3a0a 2020 2020 6874 6d6c 203d 205f  "):.    html = _
+00000440: 6765 6e65 7261 7465 5f68 746d 6c28 736f  generate_html(so
+00000450: 7572 6365 2c20 7864 736d 290a 0a20 2020  urce, xdsm)..   
+00000460: 2077 6974 6820 6f70 656e 286f 7574 6669   with open(outfi
+00000470: 6c65 6e61 6d65 2c20 2277 2229 2061 7320  lename, "w") as 
+00000480: 663a 0a20 2020 2020 2020 2066 2e77 7269  f:.        f.wri
+00000490: 7465 2868 746d 6c29 0a0a 0a64 6566 205f  te(html)...def _
+000004a0: 6765 6e65 7261 7465 5f68 746d 6c28 736f  generate_html(so
+000004b0: 7572 6365 2c20 7864 736d 293a 0a20 2020  urce, xdsm):.   
+000004c0: 2066 6f6f 7465 7220 3d20 2258 4453 4d20   footer = "XDSM 
+000004d0: 6765 6e65 7261 7465 6420 6672 6f6d 207b  generated from {
+000004e0: 7d2c 207b 7d2c 204f 4e45 5241 2057 6861  }, {}, ONERA Wha
+000004f0: 7473 4f70 7422 2e66 6f72 6d61 7428 0a20  tsOpt".format(. 
+00000500: 2020 2020 2020 2073 6f75 7263 652c 2064         source, d
+00000510: 6174 652e 746f 6461 7928 292e 7374 7266  ate.today().strf
+00000520: 7469 6d65 2822 2562 2025 642c 2025 5922  time("%b %d, %Y"
+00000530: 290a 2020 2020 290a 2020 2020 6874 6d6c  ).    ).    html
+00000540: 203d 2048 544d 4c5f 5445 4d50 4c41 5445   = HTML_TEMPLATE
+00000550: 2e66 6f72 6d61 7428 6373 7328 292c 2062  .format(css(), b
+00000560: 756e 646c 656a 7328 292c 2078 6473 6d2c  undlejs(), xdsm,
+00000570: 2066 6f6f 7465 7229 0a20 2020 2072 6574   footer).    ret
+00000580: 7572 6e20 6874 6d6c 0a                   urn html.
```

### Comparing `wop-2.5.2/whatsopt/utils.py` & `wop-2.5.3/whatsopt/utils.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,210 +1,210 @@
-import os, re
-import sys
-import tomli_w
-from whatsopt.logging import error
-from shutil import move
-
-
-WOP_CONF_FILENAME = ".wop"
-
-WOP_FORMAT_VERSION_KEY = "wop_format_version"
-WHATSOPT_URL_KEY = "whatsopt_url"
-ANALYSIS_ID_KEY = "analysis_id"
-FRAMEWORK_KEY = "framework"
-PULL_MODE_KEY = "pull_mode"
-
-FRAMEWORK_OPENMDAO = "openmdao"
-FRAMEWORK_GEMSEO = "gemseo"
-
-MODE_PLAIN = "plain"
-MODE_PACKAGE = "package"
-
-
-def save_state(
-    state,
-    filename=WOP_CONF_FILENAME,
-):
-    comment = """# This file contains recorded state from wop pull/update commands
-# DO NOT EDIT unless you know what you are doing
-# Version history:
-# * version 2: use toml format, add wop_format_version
-# * version 1: initial format "key: val"
-# * version 0: no wop file
-#
-"""
-    _state = {}
-    _state[WOP_FORMAT_VERSION_KEY] = 2
-    _state[WHATSOPT_URL_KEY] = state[WHATSOPT_URL_KEY]
-    _state[ANALYSIS_ID_KEY] = int(state[ANALYSIS_ID_KEY])
-    _state[FRAMEWORK_KEY] = state[FRAMEWORK_KEY]
-    _state[PULL_MODE_KEY] = state[PULL_MODE_KEY]
-    content = tomli_w.dumps(_state)
-
-    with open(filename, "w") as f:
-        f.write(comment)
-        f.write(content)
-
-
-def load_state(filename=WOP_CONF_FILENAME):
-    # Should be able to load version 0, version 1 and version 2 format
-    state = {"wop_format_version": 0}
-    if not os.path.exists(filename):
-        return state
-    with open(filename, "r") as f:
-        for line in f.readlines():
-            line = line.strip()
-            if line == "" or line.startswith("#"):
-                continue
-            m = re.search(r"(\S+)\s*[:=]\s*(\S+)", line)
-            if m:
-                val = m.group(2)
-                if val.startswith('"') or val.startswith("'"):
-                    val = val[1:-1]
-                if re.match(r"\d+", val):
-                    val = int(val)
-
-                state[m.group(1)] = val
-            else:
-                error(f"Syntax error in {filename} file: line '{line}' invalid")
-                sys.exit(-1)
-    if not state.get("wop_format_version"):
-        state["wop_format_version"] = 1
-
-    return state
-
-
-def is_user_file(f):
-    return (
-        not re.match(r".*_base\.py$", f)
-        and not is_run_script_file(f)
-        and not is_test_file(f)
-        and not re.match(r"^.*server/", f)
-        and not re.match(r"^.*egmdo/", f)
-    )
-
-
-def is_run_script_file(f):
-    return f == "mda_init.py" or re.match(r"^run_.*\.py$", f)
-
-
-def is_test_file(f):
-    return re.match(r"^.*tests/test_.*\.py$", f)
-
-
-def is_analysis_user_file(name, f):
-    return bool(re.match(rf"^{name}\.py$", f))
-
-
-def find_analysis_base_files(directory="."):
-    files = []
-    for f in os.listdir(directory):
-        if f.endswith("_base.py"):
-            files.append(f)
-    return files
-
-
-def _extract_key(file, key):
-    ident = None
-    with open(file, "r") as f:
-        pattern = re.compile(rf"^# {key}: (.*)")
-        for line in f:
-            match = pattern.match(line)
-            if match:
-                ident = match.group(1)
-                break
-    return ident
-
-
-def extract_remote_name(url_or_name):
-    m = re.match(r"https?:\/\/(\w+)", url_or_name)
-    if m:  # url
-        return m.group(1)
-    elif re.match(r"^\w+$", url_or_name):  # name
-        return url_or_name
-    else:
-        print(f"Warning: Can not find remote name out of {url_or_name}")
-        return None
-
-
-def _get_key(key, directory="."):
-    files = find_analysis_base_files(directory)
-    val = None
-    for f in files:
-        newval = _extract_key(os.path.join(directory, f), key)
-        if val and val != newval:
-            raise ValueError(
-                "Several {} key detected. "
-                "Find #{} then #{}.\n"
-                "Check header comments in {} files.".format(
-                    key, val, newval, str(files)
-                )
-            )
-        val = newval
-    return val
-
-
-def get_analysis_id(directory="."):
-    state = load_state()
-    if state["wop_format_version"] > 0:
-        return state[ANALYSIS_ID_KEY]
-    else:
-        return _get_key(ANALYSIS_ID_KEY, directory)
-
-
-def get_whatsopt_url(directory="."):
-    state = load_state()
-    if state["wop_format_version"] > 0:
-        return state[WHATSOPT_URL_KEY]
-    else:
-        try:
-            return _get_key(WHATSOPT_URL_KEY, directory)
-        except ValueError:
-            return False
-
-
-def is_based_on(module, directory="."):
-    state = load_state()
-    if state["wop_format_version"] > 0:
-        return state[FRAMEWORK_KEY] == module
-    else:
-        files = find_analysis_base_files(directory)
-        return len(files) > 0 and all(
-            _detect_from_import(os.path.join(directory, f), module) for f in files
-        )
-
-
-def is_framework_switch(framework, directory="."):
-    return (
-        framework == FRAMEWORK_GEMSEO and is_based_on(FRAMEWORK_OPENMDAO, directory)
-    ) or (framework == FRAMEWORK_OPENMDAO and is_based_on(FRAMEWORK_GEMSEO, directory))
-
-
-def _detect_from_import(file, module):
-    detected = False
-    with open(file, "r") as f:
-        for line in f:
-            # TODO: Maybe would need more robust detection... We'll see!
-            # first from/import detected gives the framework.
-            match = re.match(rf"^(from|import) {module}\..*", line)
-            if match:
-                detected = True
-                break
-    return detected
-
-
-def is_package_mode():
-    state = load_state()
-    return state and state[PULL_MODE_KEY] == MODE_PACKAGE
-
-
-def move_files(file_to_move, tempdir):
-    for f in file_to_move.keys():
-        file_from = os.path.join(tempdir, f)
-        file_to = f
-        dir_to = os.path.dirname(f)
-        if dir_to == "":
-            dir_to = "."
-        elif not os.path.exists(dir_to):
-            os.makedirs(dir_to)
-        if file_to_move[file_to]:
-            move(file_from, dir_to)
+import os, re
+import sys
+import tomli_w
+from whatsopt.logging import error
+from shutil import move
+
+
+WOP_CONF_FILENAME = ".wop"
+
+WOP_FORMAT_VERSION_KEY = "wop_format_version"
+WHATSOPT_URL_KEY = "whatsopt_url"
+ANALYSIS_ID_KEY = "analysis_id"
+FRAMEWORK_KEY = "framework"
+PULL_MODE_KEY = "pull_mode"
+
+FRAMEWORK_OPENMDAO = "openmdao"
+FRAMEWORK_GEMSEO = "gemseo"
+
+MODE_PLAIN = "plain"
+MODE_PACKAGE = "package"
+
+
+def save_state(
+    state,
+    filename=WOP_CONF_FILENAME,
+):
+    comment = """# This file contains recorded state from wop pull/update commands
+# DO NOT EDIT unless you know what you are doing
+# Version history:
+# * version 2: use toml format, add wop_format_version
+# * version 1: initial format "key: val"
+# * version 0: no wop file
+#
+"""
+    _state = {}
+    _state[WOP_FORMAT_VERSION_KEY] = 2
+    _state[WHATSOPT_URL_KEY] = state[WHATSOPT_URL_KEY]
+    _state[ANALYSIS_ID_KEY] = int(state[ANALYSIS_ID_KEY])
+    _state[FRAMEWORK_KEY] = state[FRAMEWORK_KEY]
+    _state[PULL_MODE_KEY] = state[PULL_MODE_KEY]
+    content = tomli_w.dumps(_state)
+
+    with open(filename, "w") as f:
+        f.write(comment)
+        f.write(content)
+
+
+def load_state(filename=WOP_CONF_FILENAME):
+    # Should be able to load version 0, version 1 and version 2 format
+    state = {"wop_format_version": 0}
+    if not os.path.exists(filename):
+        return state
+    with open(filename, "r") as f:
+        for line in f.readlines():
+            line = line.strip()
+            if line == "" or line.startswith("#"):
+                continue
+            m = re.search(r"(\S+)\s*[:=]\s*(\S+)", line)
+            if m:
+                val = m.group(2)
+                if val.startswith('"') or val.startswith("'"):
+                    val = val[1:-1]
+                if re.match(r"\d+", val):
+                    val = int(val)
+
+                state[m.group(1)] = val
+            else:
+                error(f"Syntax error in {filename} file: line '{line}' invalid")
+                sys.exit(-1)
+    if not state.get("wop_format_version"):
+        state["wop_format_version"] = 1
+
+    return state
+
+
+def is_user_file(f):
+    return (
+        not re.match(r".*_base\.py$", f)
+        and not is_run_script_file(f)
+        and not is_test_file(f)
+        and not re.match(r"^.*server/", f)
+        and not re.match(r"^.*egmdo/", f)
+    )
+
+
+def is_run_script_file(f):
+    return f == "mda_init.py" or re.match(r"^run_.*\.py$", f)
+
+
+def is_test_file(f):
+    return re.match(r"^.*tests/test_.*\.py$", f)
+
+
+def is_analysis_user_file(name, f):
+    return bool(re.match(rf"^{name}\.py$", f))
+
+
+def find_analysis_base_files(directory="."):
+    files = []
+    for f in os.listdir(directory):
+        if f.endswith("_base.py"):
+            files.append(f)
+    return files
+
+
+def _extract_key(file, key):
+    ident = None
+    with open(file, "r") as f:
+        pattern = re.compile(rf"^# {key}: (.*)")
+        for line in f:
+            match = pattern.match(line)
+            if match:
+                ident = match.group(1)
+                break
+    return ident
+
+
+def extract_remote_name(url_or_name):
+    m = re.match(r"https?:\/\/(\w+)", url_or_name)
+    if m:  # url
+        return m.group(1)
+    elif re.match(r"^\w+$", url_or_name):  # name
+        return url_or_name
+    else:
+        print(f"Warning: Can not find remote name out of {url_or_name}")
+        return None
+
+
+def _get_key(key, directory="."):
+    files = find_analysis_base_files(directory)
+    val = None
+    for f in files:
+        newval = _extract_key(os.path.join(directory, f), key)
+        if val and val != newval:
+            raise ValueError(
+                "Several {} key detected. "
+                "Find #{} then #{}.\n"
+                "Check header comments in {} files.".format(
+                    key, val, newval, str(files)
+                )
+            )
+        val = newval
+    return val
+
+
+def get_analysis_id(directory="."):
+    state = load_state()
+    if state["wop_format_version"] > 0:
+        return state[ANALYSIS_ID_KEY]
+    else:
+        return _get_key(ANALYSIS_ID_KEY, directory)
+
+
+def get_whatsopt_url(directory="."):
+    state = load_state()
+    if state["wop_format_version"] > 0:
+        return state[WHATSOPT_URL_KEY]
+    else:
+        try:
+            return _get_key(WHATSOPT_URL_KEY, directory)
+        except ValueError:
+            return False
+
+
+def is_based_on(module, directory="."):
+    state = load_state()
+    if state["wop_format_version"] > 0:
+        return state[FRAMEWORK_KEY] == module
+    else:
+        files = find_analysis_base_files(directory)
+        return len(files) > 0 and all(
+            _detect_from_import(os.path.join(directory, f), module) for f in files
+        )
+
+
+def is_framework_switch(framework, directory="."):
+    return (
+        framework == FRAMEWORK_GEMSEO and is_based_on(FRAMEWORK_OPENMDAO, directory)
+    ) or (framework == FRAMEWORK_OPENMDAO and is_based_on(FRAMEWORK_GEMSEO, directory))
+
+
+def _detect_from_import(file, module):
+    detected = False
+    with open(file, "r") as f:
+        for line in f:
+            # TODO: Maybe would need more robust detection... We'll see!
+            # first from/import detected gives the framework.
+            match = re.match(rf"^(from|import) {module}\..*", line)
+            if match:
+                detected = True
+                break
+    return detected
+
+
+def is_package_mode():
+    state = load_state()
+    return state and state[PULL_MODE_KEY] == MODE_PACKAGE
+
+
+def move_files(file_to_move, tempdir):
+    for f in file_to_move.keys():
+        file_from = os.path.join(tempdir, f)
+        file_to = f
+        dir_to = os.path.dirname(f)
+        if dir_to == "":
+            dir_to = "."
+        elif not os.path.exists(dir_to):
+            os.makedirs(dir_to)
+        if file_to_move[file_to]:
+            move(file_from, dir_to)
```

### Comparing `wop-2.5.2/whatsopt/whatsopt_client.py` & `wop-2.5.3/whatsopt/whatsopt_client.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,1063 +1,1063 @@
-from http import HTTPStatus
-import os
-import sys
-import json
-import getpass
-import requests
-import copy
-import re
-import zipfile
-import tempfile
-import numpy as np
-import time
-from datetime import datetime
-import tomli
-import tomli_w
-from tabulate import tabulate
-from urllib.parse import urlparse
-from packaging.version import Version
-
-# push
-import openmdao.utils.hooks as hooks
-from openmdao.utils.file_utils import _load_and_exec
-
-from openmdao.utils.webview import webview
-from openmdao.api import IndepVarComp
-from whatsopt.convert_utils import convert_sqlite_to_csv
-
-from whatsopt.logging import log, info, warn, error, debug
-from whatsopt.publish_utils import build_package, get_pkg_metadata
-from whatsopt.utils import (
-    FRAMEWORK_GEMSEO,
-    FRAMEWORK_OPENMDAO,
-    MODE_PACKAGE,
-    MODE_PLAIN,
-    extract_remote_name,
-    is_analysis_user_file,
-    is_based_on,
-    is_framework_switch,
-    is_package_mode,
-    is_run_script_file,
-    is_test_file,
-    is_user_file,
-    get_analysis_id,
-    get_whatsopt_url,
-    move_files,
-    save_state,
-)
-from whatsopt.upload_utils import (
-    load_from_csv,
-    load_from_sqlite,
-    load_from_hdf5,
-    print_cases,
-)
-from whatsopt.push_utils import (
-    find_indep_var_name,
-    problem_pyfile,
-    to_camelcase,
-)
-from whatsopt.push_command import PushCommand
-from whatsopt.show_utils import generate_xdsm_html
-
-from whatsopt import __version__
-
-WHATSOPT_DIRNAME = os.path.join(os.path.expanduser("~"), ".whatsopt")
-API_KEY_FILENAME = os.path.join(WHATSOPT_DIRNAME, "api_key")
-URL_FILENAME = os.path.join(WHATSOPT_DIRNAME, "url")
-REMOTES_FILENAME = os.path.join(WHATSOPT_DIRNAME, "remotes")
-
-EXTRANET_SERVER_URL = "https://ether.onera.fr/whatsopt"
-
-
-class WhatsOptImportMdaError(Exception):
-    pass
-
-
-class AnalysisPushedException(Exception):
-    def __init__(self, xdsm):
-        self.xdsm = xdsm
-
-
-class WhatsOpt:
-    def __init__(self, url=None, api_key=None, login=None):
-        self._remotes = self._read_remotes()
-
-        remote = self._remotes.get(url)
-        debug(f"remote={remote}")
-        if remote:
-            self._url = remote["url"]
-            self._api_key = api_key if api_key else remote["api_key"]
-        else:
-            debug(f"url={url} logged?={self.is_logged()}")
-            if url:
-                self._url = url.strip("/")
-                current_url = self._read_url()
-                if current_url and self._url != current_url:
-                    self.logout(echo=False)
-            elif self.is_logged():
-                self._url = self._read_url()
-            else:
-                self._url = EXTRANET_SERVER_URL
-
-            if api_key:
-                self._api_key = api_key
-            else:
-                self._api_key = self._read_api_key()
-
-        # config session object
-        self.session = requests.Session()
-        urlinfos = urlparse(self._url)
-        self.session.trust_env = re.match(r"\w+.onera\.fr", urlinfos.netloc)
-        self.headers = {}
-
-    @property
-    def url(self):
-        return self._url
-
-    @property
-    def api_key(self):
-        return self._api_key
-
-    def endpoint(self, path):
-        return self._url + path
-
-    @staticmethod
-    def err_msg(resp):
-        error(
-            "{} ({}) : {}".format(
-                resp.status_code,
-                requests.status_codes._codes[resp.status_code][0],
-                resp.json()["message"],
-            )
-        )
-
-    @staticmethod
-    def _read_remotes():
-        remotes = {}
-        if os.path.exists(REMOTES_FILENAME):
-            with open(REMOTES_FILENAME, "rb") as f:
-                remotes = tomli.load(f)
-        return remotes
-
-    @staticmethod
-    def _write_remotes(remotes):
-        with open(REMOTES_FILENAME, "wb") as f:
-            tomli_w.dump(remotes, f)
-
-    def _ask_api_key(self):
-        log("You have to set your API key.")
-        log("You can get it in your profile page on WhatsOpt (%s)." % self.url)
-        info(
-            "Please, copy/paste your API key below then hit return (characters are hidden)."
-        )
-        api_key = getpass.getpass(prompt="Your API key: ")
-        return api_key
-
-    @staticmethod
-    def is_logged():
-        # Defensive programming: test on api_key should be enough but...
-        return os.path.exists(URL_FILENAME) and os.path.exists(API_KEY_FILENAME)
-
-    @staticmethod
-    def _read_url():
-        if os.path.exists(URL_FILENAME):
-            with open(URL_FILENAME, "r") as f:
-                return f.read()
-        else:
-            return None
-
-    @staticmethod
-    def _read_api_key():
-        if os.path.exists(API_KEY_FILENAME):
-            with open(API_KEY_FILENAME, "r") as f:
-                return f.read()
-        else:
-            return None
-
-    def _write_login_infos(self):
-        if not os.path.exists(WHATSOPT_DIRNAME):
-            os.makedirs(WHATSOPT_DIRNAME)
-        with open(API_KEY_FILENAME, "w") as f:
-            f.write(self.api_key)
-        with open(URL_FILENAME, "w") as f:
-            f.write(self.url)
-
-    def login(self, echo=False, retry=True):
-        debug(f"login(api_key={self.api_key}, echo={echo})")
-
-        # Check login with remote name
-        if not (
-            self.url.startswith("http://") or self.url.startswith("https://")
-        ) and not self._remotes.get(self.url):
-            error(f"Unknown remote server '{self.url}'")
-            WhatsOpt.list_remotes()
-            sys.exit(-1)
-
-        if self._api_key:
-            # api key is provided
-            pass
-        elif self.is_logged():
-            # check if logged in
-            self._api_key = self._read_api_key()
-        else:
-            # check if known remote
-            for _, v in self._remotes.items():
-                if self.url == v["url"]:
-                    self._api_key = v["api_key"]
-                    break
-            # ask for API key otherwise
-            debug("Ask for API key")
-            self._api_key = self._ask_api_key() if not self._api_key else self._api_key
-
-        debug(f"url={self.url}, api_key={self.api_key}")
-        ok = self._test_connection()
-        debug(f"ok={ok}")
-        if not ok and retry:
-            # try to log again
-            # log out silently as one may be logged on another server
-            self.logout(echo=False)
-            self._remotes = {
-                k: v for k, v in self._remotes.items() if v["url"] != self.url
-            }
-            # save url again as is has been wipe out by logout
-            with open(URL_FILENAME, "w") as f:
-                f.write(self._url)
-            return self.login(retry=False)
-
-        # make remote info
-        if ok:
-            self._write_login_infos()
-            remote_name = extract_remote_name(self.url)
-            if remote_name:
-                self._remotes[remote_name] = {"url": self.url, "api_key": self.api_key}
-
-        debug(self._remotes)
-        self._write_remotes(self._remotes)
-
-        if not ok:
-            error("Login to WhatsOpt ({}) failed.".format(self.url))
-            log("")
-            warn("You are not connected.")
-            info("  use `wop login <url>` to connect to a remote WhatsOpt server")
-            info(
-                "  use `wop login <name>` to connect to a known remote WhatsOpt server"
-            )
-            self.list_remotes()
-
-            sys.exit(-1)
-
-        if echo:
-            info(f"Successfully logged in to remote WhatsOpt {self.url}")
-            log("")
-        return self
-
-    @staticmethod
-    def logout(list=None, all=None, remote=None, echo=True):
-        if list:
-            WhatsOpt.list_remotes()
-        elif all:
-            WhatsOpt._write_remotes({})
-            if echo:
-                info("Sucessfully logged out from all WhatsOpt remotes")
-        elif remote:
-            remotes = WhatsOpt._read_remotes()
-            if remotes.get(remote):
-                del remotes[remote]
-                WhatsOpt._write_remotes(remotes)
-                if echo:
-                    info(f"Sucessfully logged out from remote WhatsOpt {remote}")
-        else:
-            if os.path.exists(API_KEY_FILENAME):
-                os.remove(API_KEY_FILENAME)
-            url = WhatsOpt._read_url()
-            if url:
-                os.remove(URL_FILENAME)
-            if echo:
-                if url:
-                    info(f"Sucessfully logged out from remote WhatsOpt {url}")
-                else:
-                    info("Not connected. You may want to connect to:")
-                    WhatsOpt.list_remotes()
-
-        if echo:
-            log("")
-
-    @staticmethod
-    def list_remotes():
-        remotes = WhatsOpt._read_remotes()
-        headers = ["name", "url"]
-        data = []
-        for name, rem in remotes.items():
-            data.append([name, rem["url"]])
-        info("Known remote servers")
-        log(tabulate(data, headers))
-
-    def list_analyses(self, all=False, project_query=None):
-        param = ""
-        if all:
-            param = "?all=true"
-        elif project_query:
-            param = "?design_project_query={}".format(project_query)
-        url = self.endpoint("/api/v1/analyses" + param)
-        resp = self.session.get(url, headers=self.headers)
-        if resp.ok:
-            mdas = resp.json()
-            headers = ["id", "name", "created at"]
-            data = []
-            for mda in mdas:
-                date = mda.get("created_at", None)
-                data.append([mda["id"], mda["name"], date])
-            log(tabulate(data, headers))
-            log("")
-        else:
-            resp.raise_for_status()
-
-    def is_connected(self):
-        return self._test_connection()
-
-    def get_status(self):
-        connected = self.is_connected()
-        whatsopt_url = get_whatsopt_url() or self.url
-        if connected:
-            info("You are logged in {}".format(self.url))
-        else:
-            info("You are not connected.")
-        mda_id = None
-        try:
-            mda_id = get_analysis_id()
-        except ValueError as err:
-            warn(str(err))
-        if mda_id:
-            if connected and whatsopt_url == self.url:
-                info("Found local analysis code (id=#{})".format(mda_id))
-                # connected to the right server from which the analysis was pulled
-                url = self.endpoint("/api/v1/analyses/{}".format(mda_id))
-                resp = self.session.get(url, headers=self.headers)
-
-                if resp.ok:
-                    mda = resp.json()
-                    if is_based_on(FRAMEWORK_GEMSEO):
-                        mda["framework"] = "GEMSEO"
-                    elif is_based_on(FRAMEWORK_OPENMDAO):
-                        mda["framework"] = "OpenMDAO"
-                    else:  # should not happen
-                        raise ValueError(
-                            "No framework detected. Check your *_base.py files."
-                        )
-                    headers = ["id", "name", "created_at", "owner_email", "framework"]
-                    data = [[mda[k] for k in headers]]
-                    log(tabulate(data, headers))
-                else:
-                    error("Analysis not found on the server anymore (probably deleted)")
-                    log(
-                        "  (use 'wop push <analysis.py>' to push from an OpenMDAO code to the server)"
-                    )
-            else:
-                info(
-                    "Found local analysis code (id=#{}) "
-                    "pulled from {}".format(mda_id, whatsopt_url)
-                )
-                if connected:
-                    # connected to another server with a pulled analysis
-                    warn("You are connected to a different server")
-                    log(
-                        "  (use 'wop push <analysis.py>' to push from the local "
-                        f"analysis code to the server {self.url})"
-                    )
-                    log(
-                        f"  (use 'wop logout' and 'wop login {whatsopt_url}' "
-                        "to log in to the original server)"
-                    )
-                else:
-                    log(f"  (use 'wop login {whatsopt_url}' command to log in)")
-        else:
-            info("No local analysis found")
-            if connected:
-                log(
-                    "  (use 'wop list' and 'wop pull <id>' to retrieve an existing analysis)\n"
-                    "  (use 'wop push <analysis.py>' to push from the local OpenMDAO code to the server)"
-                )
-        log("")
-
-    def push_component_cmd(self, py_filename, component, options):
-        with problem_pyfile(py_filename, component) as pyf:
-            if options["--dry-run"]:
-                with open(pyf, "r") as pbf:
-                    print(pbf.read())
-                    sys.exit()
-            self.push_mda_cmd(pyf, options)
-
-    def push_mda_cmd(self, py_filename, options):
-        def push_mda(prob):
-            name = options["--name"]
-            pbname = prob.model.__class__.__name__
-            if name and pbname != name:
-                info("Analysis %s skipped" % pbname)
-                # do not exit seeking for another problem (ie analysis)
-            else:
-                options["--pyfilename"] = py_filename
-                xdsm = self.push_mda(prob, options)
-                if options.get("--xdsm"):  # show command
-                    # required to interrupt pb execution
-                    raise AnalysisPushedException(xdsm=xdsm)
-                else:
-                    sys.exit()
-
-        hooks.use_hooks = True
-        hooks._register_hook("final_setup", "Problem", post=push_mda)
-        _load_and_exec(py_filename, [])
-        return push_mda
-
-    def push_mda(self, problem, options):
-        scalar = options.get("--scalar")
-        depth = options.get("--depth")
-        push_cmd = PushCommand(problem, depth, scalar)
-
-        mda_attrs = push_cmd.get_mda_attributes(
-            problem.model, push_cmd.tree, use_depth=True
-        )
-
-        if mda_attrs["name"] == "Group" and options.get("--pyfilename"):
-            mda_attrs["name"] = os.path.splitext(
-                to_camelcase(os.path.basename(options.get("--pyfilename")))
-            )[0]
-
-        if options["--dry-run"]:
-            log(json.dumps(mda_attrs, indent=2))
-        else:
-            suffix = ""
-            if options.get("--xdsm"):
-                suffix = ".xdsm"
-            url = self.endpoint("/api/v1/analyses{}".format(suffix))
-            resp = self.session.post(
-                url, headers=self.headers, json={"analysis": mda_attrs}
-            )
-            resp.raise_for_status()
-            log("Analysis %s pushed" % mda_attrs["name"])
-            return resp.json()
-
-    def push_json(self, filename):
-        with open(filename, "rb") as f:
-            attrs = json.load(f)
-        if "analyses_attributes" in attrs:  # project detection
-            url = self.endpoint("/api/v1/design_projects")
-            key = "Project"
-        else:
-            url = self.endpoint("/api/v1/analyses")
-            key = "Analysis"
-        params = {}
-        params[key.lower()] = attrs
-        resp = self.session.post(url, headers=self.headers, json=params)
-        resp.raise_for_status()
-        log("{} {} pushed".format(key, attrs["name"]))
-
-    def pull_mda(self, mda_id, options={}, msg=None, info_keep_run_ops=True):
-        if not msg:
-            msg = "Analysis %s pulled" % mda_id
-
-        framework = FRAMEWORK_OPENMDAO
-        if options.get("--gemseo"):
-            framework = FRAMEWORK_GEMSEO
-
-        param = ""
-        if options.get("--run-ops"):
-            param += "&with_runops=true"
-        if options.get("--server"):
-            if framework == FRAMEWORK_OPENMDAO:
-                param += "&with_server=true"
-            else:
-                warn(
-                    "Can not generate server with GEMSEO framework. --server is ignored"
-                )
-        if options.get("--egmdo"):
-            if framework == FRAMEWORK_OPENMDAO:
-                param += "&with_egmdo=true"
-            else:
-                warn("Can not generate EGMDO with GEMSEO framework. --egmdo is ignored")
-        if options.get("--test-units"):
-            if framework == FRAMEWORK_OPENMDAO:
-                param += "&with_unittests=true"
-            else:
-                warn(
-                    "Can not generate tests with GEMSEO framework. --test-units is ignored"
-                )
-        if param:
-            param = "?" + param[1:]
-
-        format_query = framework
-        if options.get("--package"):
-            format_query += "_pkg"
-
-        url = self.endpoint(
-            ("/api/v1/analyses/{}/exports/new.{}{}".format(mda_id, format_query, param))
-        )
-        resp = self.session.get(url, headers=self.headers, stream=True)
-        resp.raise_for_status()
-        name = None
-        with tempfile.NamedTemporaryFile(suffix=".zip", mode="wb", delete=False) as fd:
-            for chunk in resp.iter_content(chunk_size=128):
-                fd.write(chunk)
-            name = fd.name
-        zipf = zipfile.ZipFile(name, "r")
-        tempdir = tempfile.mkdtemp(suffix="wop", dir=tempfile.tempdir)
-        zipf.extractall(tempdir)
-        filenames = zipf.namelist()
-        zipf.close()
-        file_to_move = {}
-        if options.get("--dry-run"):
-            cmd = "Pull"
-            if options.get("--update"):
-                cmd = "Update"
-            info(
-                "***************************************************\n"
-                f"* DRY RUN mode (actions are listed but not done) *\n"
-                "***************************************************"
-            )
-
-        # Special case: When framework switch we have to update
-        # user analysis main file which name depends on package name
-        framework_switch = is_framework_switch(framework)
-        if framework_switch:
-            url = self.endpoint(f"/api/v1/analyses/{mda_id}/openmdao_impl")
-            resp = self.session.get(url, headers=self.headers, stream=True)
-            resp.raise_for_status()
-            mda_name = resp.json()["packaging"]["package_name"]
-        else:
-            mda_name = ""
-
-        for f in filenames:
-            file_to = f
-            file_to_move[file_to] = True
-            if os.path.exists(file_to):
-                if options.get("--force"):
-                    log(f"Update {file_to}")
-                    if options.get("--dry-run"):
-                        file_to_move[file_to] = False
-                    else:
-                        os.remove(file_to)
-                elif options.get("--update"):
-                    if is_run_script_file(f) and not options.get("--run-ops"):
-                        if info_keep_run_ops:
-                            info(f"Keep existing {file_to} (use -r to override)")
-                        file_to_move[file_to] = False
-                        continue
-                    if is_test_file(f) and not options.get("--test-units"):
-                        file_to_move[file_to] = False
-                        continue
-                    if is_user_file(f):
-                        file_to_move[file_to] = False
-                        # Have to update user analysis main file when switching frameworks
-                        if is_framework_switch and is_analysis_user_file(mda_name, f):
-                            file_to_move[file_to] = True
-                        else:
-                            continue
-                    log(f"Update {file_to}")
-                    if not options.get("--dry-run"):
-                        os.remove(file_to)
-                else:
-                    warn(
-                        f"File {file_to} in the way: remove it or use --force to override"
-                    )
-                    file_to_move[file_to] = False
-            else:
-                if options.get("--force"):
-                    log(f"Pull {file_to}")
-                    if options.get("--dry-run"):
-                        file_to_move[file_to] = False
-                elif options.get("--update") and (
-                    (is_run_script_file(f) and not options.get("--run-ops"))
-                    or (is_test_file(f) and not options.get("--test-units"))
-                    or is_user_file(f)
-                ):
-                    file_to_move[file_to] = False
-                else:
-                    log(f"Pull {file_to}")
-
-        if not options.get("--dry-run"):
-            move_files(file_to_move, tempdir)
-            state = {
-                "whatsopt_url": self._url,
-                "analysis_id": mda_id,
-                "framework": framework,
-                "pull_mode": MODE_PACKAGE if options.get("--package") else MODE_PLAIN,
-            }
-            save_state(state)
-            info(msg)
-
-    def pull_mda_json(self, mda_id):
-        url = self.endpoint(f"/api/v1/analyses/{mda_id}.wopjson")
-        resp = self.session.get(url, headers=self.headers, stream=True)
-        resp.raise_for_status()
-        print(json.dumps(resp.json()))
-
-    def pull_project_json(self, project_id):
-        url = self.endpoint(f"/api/v1/design_projects/{project_id}.wopjson")
-        resp = self.session.get(url, headers=self.headers, stream=True)
-        resp.raise_for_status()
-        print(json.dumps(resp.json()))
-
-    def update_mda(self, analysis_id=None, options={}, info_keep_run_ops=True):
-        mda_id = analysis_id or get_analysis_id()
-        if mda_id and not analysis_id:
-            url = get_whatsopt_url()
-            if url != self.url:
-                warn(
-                    f"You want to update code pulled from {url} while you are logged in {self.url}."
-                )
-                info(
-                    f"  use 'wop login {url}' and retry to update using the original remote."
-                )
-                info(
-                    f"  use 'wop update -a <id>' to update using analysis #<id> from {self.url}."
-                )
-                sys.exit(-1)
-        if mda_id is None:
-            error(
-                f"Unknown analysis with id=#{mda_id} (maybe use wop pull <analysis-id>)"
-            )
-            sys.exit(-1)
-        # keep options unchanged, work on a copy
-        opts = copy.deepcopy(options)
-        # sanity checks
-        if not (is_based_on(FRAMEWORK_OPENMDAO) or is_based_on(FRAMEWORK_GEMSEO)):
-            error("No framework detected. Check your *_base.py files.")
-            sys.exit(-1)
-        if opts["--openmdao"] and opts["--gemseo"]:
-            error("Please choose either --openmdao or --gemseo.")
-            sys.exit(-1)
-        opts.update(
-            {
-                "--base": True,
-                "--update": True,
-                "--gemseo": opts["--gemseo"]
-                or (not opts["--openmdao"] and is_based_on(FRAMEWORK_GEMSEO)),
-                "--openmdao": opts["--openmdao"]
-                or (not opts["--gemseo"] and is_based_on(FRAMEWORK_OPENMDAO)),
-                "--package": is_package_mode(),
-            }
-        )
-        self.pull_mda(
-            mda_id, opts, "Analysis #{} updated".format(mda_id), info_keep_run_ops
-        )
-
-    def show_mda(self, analysis_id, pbfile, name, outfile, batch, depth):
-        options = {
-            "--xdsm": True,
-            "--name": name,
-            "--dry-run": False,
-            "--depth": depth,
-        }
-        xdsm = None
-        if pbfile:
-            start = time.time()
-            try:
-                info("XDSM info retrieval...")
-                self.push_mda_cmd(pbfile, options)
-            except AnalysisPushedException as pushed:
-                xdsm = pushed.xdsm
-            end = time.time()
-            log("Retrieved in {:.2f}s".format(end - start))
-            source = os.path.basename(pbfile)
-        else:
-            mda_id = analysis_id or get_analysis_id()
-            if mda_id is None:
-                error(
-                    "Unknown analysis with id={} (maybe use wop pull <analysis-id>)".format(
-                        mda_id
-                    )
-                )
-                sys.exit(-1)
-            url = self.endpoint("/api/v1/analyses/{}.xdsm".format(mda_id))
-            resp = self.session.get(url, headers=self.headers)
-            resp.raise_for_status()
-            xdsm = resp.json()
-            source = f"{mda_id}@{self._url}"
-
-        info("XDSM building...")
-        generate_xdsm_html(source, xdsm, outfile)
-        if pbfile:
-            log("XDSM of analysis from {} generated in {}".format(pbfile, outfile))
-        else:
-            log("XDSM of analysis {} generated in {}".format(mda_id, outfile))
-        if not batch:
-            webview(outfile)
-
-    def upload(
-        self,
-        filename,
-        driver_kind=None,
-        analysis_id=None,
-        operation_id=None,
-        dry_run=False,
-        outvar_count=1,
-        only_success=False,
-        parallel=False,
-    ):
-        from socket import gethostname
-
-        mda_id = get_analysis_id() if not analysis_id else analysis_id
-
-        # Test sqlite files generated with MPI
-        _, extension = os.path.splitext(filename)
-        parallel_sqlite = re.match(r"\.sqlite_\d+$", extension)
-
-        name = cases = statuses = None
-        if not os.path.exists(filename):
-            error(f"File not found ({filename})")
-            sys.exit(-1)
-        if os.path.basename(filename) == "mda_init.py":
-            self.upload_vars_init_cmd(
-                filename, {"--dry-run": dry_run, "--analysis-id": mda_id}
-            )
-        elif filename.endswith(".csv"):
-            name, cases, statuses = load_from_csv(filename)
-        elif filename.endswith(".sqlite") or (parallel_sqlite and parallel):
-            name, cases, statuses = load_from_sqlite(filename, parallel)
-        elif filename.endswith(".hdf5"):
-            name, cases, statuses = load_from_hdf5(filename)
-        else:
-            error(
-                f"Can not upload file {filename}: extension not recognized"
-                " (should be either .csv, .sqlite or .hdf5)"
-            )
-            sys.exit(-1)
-
-        if only_success:
-            for c in cases:
-                c["values"] = [
-                    val for i, val in enumerate(c["values"]) if statuses[i] > 0
-                ]
-            statuses = [1 for s in statuses if s > 0]
-
-        for c in cases:
-            c["values"] = np.nan_to_num(np.array(c["values"])).tolist()
-
-        if dry_run:
-            print_cases(cases, statuses)
-            sys.exit()
-
-        resp = None
-        if operation_id:
-            url = self.endpoint(("/api/v1/operations/%s") % operation_id)
-            operation_params = {"cases": cases}
-            resp = self.session.patch(
-                url, headers=self.headers, json={"operation": operation_params}
-            )
-        else:
-            if mda_id:
-                url = self.endpoint(("/api/v1/analyses/%s/operations") % mda_id)
-            else:
-                url = self.endpoint("/api/v1/operations")
-            if driver_kind:
-                driver = "user_{}_algo".format(driver_kind)
-            else:
-                # suppose name well-formed <lib>-<doe|optimizer|screening>-<algoname>
-                # otherwise it will default to doe
-                m = re.match(r"(\w+)_(doe|optimizer|screening)_(\w+)", name.lower())
-                if m:
-                    driver = name.lower()
-                else:
-                    driver = "user_data_uploading"
-            operation_params = {
-                "name": name,
-                "driver": driver,
-                "host": gethostname(),
-                "cases": cases,
-                "success": statuses,
-            }
-            params = {"operation": operation_params}
-            if outvar_count > 0 and outvar_count < len(cases):
-                params["outvar_count_hint"] = outvar_count
-            resp = self.session.post(url, headers=self.headers, json=params)
-        resp.raise_for_status()
-        log("Results data from {} uploaded with driver {}".format(filename, driver))
-
-    def upload_vars_init_cmd(self, py_filename, options):
-        def upload_vars_init(prob):
-            self.upload_vars_init(prob, options)
-            sys.exit()
-
-        d = os.path.dirname(py_filename)
-        run_mda_filename = os.path.join(d, "run_mda.py")
-        if not os.path.exists(run_mda_filename):
-            error(f"Can not get analysis init: script {run_mda_filename} not found.")
-        hooks.use_hooks = True
-        hooks._register_hook("final_setup", "Problem", post=upload_vars_init)
-        _load_and_exec(run_mda_filename, [])
-
-    def upload_vars_init(self, problem, options):
-        mda_id = get_analysis_id() if get_analysis_id() else options["--analysis-id"]
-        if mda_id is None:
-            error("Unknown analysis with id={}".format(mda_id))
-            sys.exit(-1)
-        parameters = []
-        headers = ["variable", "init value"]
-        data = []
-        for s in problem.model._subsystems_myproc:
-            if isinstance(s, IndepVarComp):
-                for absname in s._var_abs2meta["output"]:
-                    name = find_indep_var_name(problem, absname)
-                    value = s._outputs._views[absname][:]
-                    if isinstance(value, np.ndarray):
-                        value = str(value.tolist())
-                    parameters.append({"varname": name, "value": value})
-        data = [[p["varname"], p["value"]] for p in parameters]
-        params = {"parameterization": {"parameters": parameters}}
-        log(tabulate(data, headers))
-        if not options["--dry-run"]:
-            url = self.endpoint(f"/api/v1/analyses/{mda_id}/parameterization")
-            resp = self.session.put(url, headers=self.headers, json=params)
-            resp.raise_for_status()
-            log("Variables init values uploaded")
-
-    def check_versions(self):
-        url = self.endpoint("/api/v1/versioning")
-        resp = self.session.get(url, headers=self.headers)
-        resp.raise_for_status()
-        version = resp.json()
-        log("WhatsOpt {} requires wop {}".format(version["whatsopt"], version["wop"]))
-        log(f"You are using wop {__version__}")
-
-    @staticmethod
-    def serve(port):
-        try:
-            import thrift
-        except ImportError:
-            error(
-                "Apache Thrift is not installed. You can install it with : 'pip install thrift'"
-            )
-            sys.exit(-1)
-        try:
-            import os, sys
-
-            # insert current dir first as another run_server exists under whatsopt/services
-            sys.path.insert(0, os.getcwd())
-            from run_server import run_server
-        except ImportError as err:
-            print(str(err))
-            error("Server not found!")
-            try:
-                mda_id = get_analysis_id()
-                if mda_id:
-                    log(
-                        f"  (use 'wop update -s' to generate server for current analysis #{mda_id})"
-                    )
-                else:
-                    warn("No local analysis found")
-                    log(
-                        "  (use 'wop pull -s <id>' to generate server for the analysis #id)"
-                    )
-            except ValueError as err:
-                warn(str(err))
-            sys.exit(-1)
-        run_server(port)
-
-    @staticmethod
-    def convert(filename):
-        if not os.path.exists(filename):
-            error(f"File {filename} not found.")
-        pathname, extension = os.path.splitext(filename)
-        if not (extension == ".sqlite" or re.match(r"\.sqlite_\d+$", extension)):
-            warn(
-                f"File {filename} should have '.sqlite[_n]' extension, got '{extension}'"
-            )
-        basename = os.path.basename(pathname)
-        convert_sqlite_to_csv(filename, basename)
-
-    def publish(self, force=False, analysis_id=None):
-        mda_id = analysis_id if analysis_id else get_analysis_id()
-        url = self.endpoint(f"/api/v1/analyses/{mda_id}/package")
-        if not force:
-            resp = self.session.get(url, headers=self.headers)
-            if resp.ok:
-                existing_meta = resp.json()
-            elif resp.status_code == HTTPStatus.NOT_FOUND:
-                existing_meta = None
-            else:
-                resp.raise_for_status()
-
-            if existing_meta:
-                warn(
-                    f"Existing package {existing_meta['name']} {existing_meta['version']} will be lost."
-                )
-                answer = input("Do you want to continue? (yes/no): ")
-                if answer.lower() == "yes":
-                    pass
-                else:
-                    info("Publishing aborted")
-                    exit(-1)
-
-        info("Package building...")
-        filename = self.build()
-        if not os.path.exists(filename):
-            error(f"File {filename} not found")
-            exit(-1)
-        meta = get_pkg_metadata(filename)
-        if (
-            not force
-            and existing_meta
-            and existing_meta["name"] == meta.name
-            and Version(existing_meta["version"]) >= Version(meta.version)
-        ):
-            error(f"You have to bump the version (> {existing_meta['version']})")
-            error("Publishing aborted")
-            exit(-1)
-
-        files = {
-            "package[description]": (None, meta.summary, "application/json"),
-            "package[archive]": (filename, open(filename, "rb"), "application/gzip"),
-        }
-        info("Package publishing...")
-        resp = self.session.post(url, headers=self.headers, files=files)
-        if resp.ok:
-            info(
-                f"Package {meta.name} v{meta.version} is published on WopStore({self.endpoint('/packages')})"
-            )
-        elif resp.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-            error(resp.json()["message"])
-            error("Duplicate detected! The package already exists on WopStore!")
-            exit(-1)
-        else:
-            resp.raise_for_status()
-
-    def build(self):
-        if not is_package_mode():
-            error("Package mode is required!")
-            exit(-1)
-        self._update_mda_base()
-        filename = build_package()
-        return filename
-
-    def fetch(self, source_id=None, options={}):
-        if not is_package_mode():
-            error("Package mode is required!")
-            exit(-1)
-        mda_id = get_analysis_id()
-        param = f"?src_id={source_id}"
-        format_query = "mda_pkg_content"
-        url = self.endpoint(
-            f"/api/v1/analyses/{mda_id}/exports/new.{format_query}{param}"
-        )
-        resp = self.session.get(url, headers=self.headers, stream=True)
-        if resp.ok:
-            name = None
-            with tempfile.NamedTemporaryFile(
-                suffix=".zip", mode="wb", delete=False
-            ) as fd:
-                for chunk in resp.iter_content(chunk_size=128):
-                    fd.write(chunk)
-                name = fd.name
-            zipf = zipfile.ZipFile(name, "r")
-            tempdir = tempfile.mkdtemp(suffix="wop", dir=tempfile.tempdir)
-            zipf.extractall(tempdir)
-            filenames = zipf.namelist()
-            if not filenames:
-                warn(
-                    f"Fetching but no package found for analysis #{source_id}, nothing to do"
-                )
-                return
-            zipf.close()
-
-            file_to_move = {}
-            for f in filenames:
-                file_to = f
-                file_to_move[file_to] = True
-                if os.path.exists(file_to):
-                    if options.get("--force"):
-                        log(f"Fetch {file_to}")
-                        if options.get("--dry-run"):
-                            file_to_move[file_to] = False
-                        else:
-                            os.remove(file_to)
-                    else:
-                        warn(
-                            f"File {file_to} in the way: remove it or use --force to override"
-                        )
-                        file_to_move[file_to] = False
-                else:
-                    log(f"Fetch {file_to}")
-            if not options.get("--dry-run"):
-                move_files(file_to_move, tempdir)
-                info(f"Analysis #{source_id} disciplines fetched")
-        else:
-            error(f"Error while fetching disciplines of analysis #{source_id}")
-            error(resp.json().get("message"))
-
-    def merge(self, source_id, options={}):
-        if not is_package_mode():
-            error("Package mode is required!")
-            exit(-1)
-        current_id = get_analysis_id()
-        if int(source_id) == current_id:
-            warn(f"Merging analysis #{current_id} in itself, nothing to do")
-            return
-        url = self.endpoint(f"/api/v1/analyses/{current_id}")
-        params = {
-            "analysis": {
-                "import": {"analysis": source_id},
-            },
-            "requested_at": str(datetime.now()),
-        }
-        if options.get("--dry-run"):
-            self.get_status()
-            url = self.endpoint("/api/v1/analyses/{}".format(source_id))
-            resp = self.session.get(url, headers=self.headers)
-            log(f"Analysis #{source_id} #{resp.json()} is selected to be merged")
-        else:
-            resp = self.session.put(url, headers=self.headers, json=params)
-        if resp.ok:
-            if not options.get("--dry-run"):
-                info(f"Analysis #{source_id} merged")
-        elif resp.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-            error(f"Error while merging analysis #{source_id}.")
-            error(
-                f"    Check analyses, maybe they are not compatible (same variable produced by different disciplines)"
-            )
-        elif resp.status_code == HTTPStatus.FORBIDDEN:
-            error(f"Error while merging analysis #{source_id}.")
-            error(
-                f"    You are not authorized to update the current analysis: either you do not own it or"
-                f" current analysis is already packaged or operated"
-            )
-        else:
-            error(f"Error while merging analysis #{source_id}")
-            resp.raise_for_status()
-
-    def pull_source_mda(self, source_id, options={}):
-        self.merge(source_id, options)
-        self.fetch(source_id, options)
-        self._update_mda_base(options.get("--dry-run"))
-
-    def _update_mda_base(self, dry_run=False, force=False):
-        update_options = {
-            "--dry-run": dry_run,
-            "--force": force,
-            "--server": False,
-            "--egmdo": False,
-            "--run-ops": False,
-            "--test-units": False,
-            "--gemseo": is_based_on(FRAMEWORK_GEMSEO),
-            "--openmdao": is_based_on(FRAMEWORK_OPENMDAO),
-        }
-        mda_id = get_analysis_id()
-        self.update_mda(mda_id, update_options, info_keep_run_ops=False)
-
-    def _test_connection(self):
-        if self.api_key:
-            self.headers = {
-                "Authorization": "Token token=" + self.api_key,
-                "User-Agent": "wop/{}".format(__version__),
-            }
-            url = self.endpoint("/api/v1/versioning")
-            debug(f"Test connect: {url}, {self.api_key}")
-            try:
-                resp = self.session.get(url, headers=self.headers)
-                # special case: bad wop version < minimal required version
-                if resp.status_code == requests.codes.forbidden:
-                    error(resp.json()["message"])
-                    sys.exit(-1)
-                return resp.ok
-            except requests.exceptions.ConnectionError:
-                return False
-        else:
-            return False
+from http import HTTPStatus
+import os
+import sys
+import json
+import getpass
+import requests
+import copy
+import re
+import zipfile
+import tempfile
+import numpy as np
+import time
+from datetime import datetime
+import tomli
+import tomli_w
+from tabulate import tabulate
+from urllib.parse import urlparse
+from packaging.version import Version
+
+# push
+import openmdao.utils.hooks as hooks
+from openmdao.utils.file_utils import _load_and_exec
+
+from openmdao.utils.webview import webview
+from openmdao.api import IndepVarComp
+from whatsopt.convert_utils import convert_sqlite_to_csv
+
+from whatsopt.logging import log, info, warn, error, debug
+from whatsopt.publish_utils import build_package, get_pkg_metadata
+from whatsopt.utils import (
+    FRAMEWORK_GEMSEO,
+    FRAMEWORK_OPENMDAO,
+    MODE_PACKAGE,
+    MODE_PLAIN,
+    extract_remote_name,
+    is_analysis_user_file,
+    is_based_on,
+    is_framework_switch,
+    is_package_mode,
+    is_run_script_file,
+    is_test_file,
+    is_user_file,
+    get_analysis_id,
+    get_whatsopt_url,
+    move_files,
+    save_state,
+)
+from whatsopt.upload_utils import (
+    load_from_csv,
+    load_from_sqlite,
+    load_from_hdf5,
+    print_cases,
+)
+from whatsopt.push_utils import (
+    find_indep_var_name,
+    problem_pyfile,
+    to_camelcase,
+)
+from whatsopt.push_command import PushCommand
+from whatsopt.show_utils import generate_xdsm_html
+
+from whatsopt import __version__
+
+WHATSOPT_DIRNAME = os.path.join(os.path.expanduser("~"), ".whatsopt")
+API_KEY_FILENAME = os.path.join(WHATSOPT_DIRNAME, "api_key")
+URL_FILENAME = os.path.join(WHATSOPT_DIRNAME, "url")
+REMOTES_FILENAME = os.path.join(WHATSOPT_DIRNAME, "remotes")
+
+EXTRANET_SERVER_URL = "https://ether.onera.fr/whatsopt"
+
+
+class WhatsOptImportMdaError(Exception):
+    pass
+
+
+class AnalysisPushedException(Exception):
+    def __init__(self, xdsm):
+        self.xdsm = xdsm
+
+
+class WhatsOpt:
+    def __init__(self, url=None, api_key=None, login=None):
+        self._remotes = self._read_remotes()
+
+        remote = self._remotes.get(url)
+        debug(f"remote={remote}")
+        if remote:
+            self._url = remote["url"]
+            self._api_key = api_key if api_key else remote["api_key"]
+        else:
+            debug(f"url={url} logged?={self.is_logged()}")
+            if url:
+                self._url = url.strip("/")
+                current_url = self._read_url()
+                if current_url and self._url != current_url:
+                    self.logout(echo=False)
+            elif self.is_logged():
+                self._url = self._read_url()
+            else:
+                self._url = EXTRANET_SERVER_URL
+
+            if api_key:
+                self._api_key = api_key
+            else:
+                self._api_key = self._read_api_key()
+
+        # config session object
+        self.session = requests.Session()
+        urlinfos = urlparse(self._url)
+        self.session.trust_env = re.match(r"\w+.onera\.fr", urlinfos.netloc)
+        self.headers = {}
+
+    @property
+    def url(self):
+        return self._url
+
+    @property
+    def api_key(self):
+        return self._api_key
+
+    def endpoint(self, path):
+        return self._url + path
+
+    @staticmethod
+    def err_msg(resp):
+        error(
+            "{} ({}) : {}".format(
+                resp.status_code,
+                requests.status_codes._codes[resp.status_code][0],
+                resp.json()["message"],
+            )
+        )
+
+    @staticmethod
+    def _read_remotes():
+        remotes = {}
+        if os.path.exists(REMOTES_FILENAME):
+            with open(REMOTES_FILENAME, "rb") as f:
+                remotes = tomli.load(f)
+        return remotes
+
+    @staticmethod
+    def _write_remotes(remotes):
+        with open(REMOTES_FILENAME, "wb") as f:
+            tomli_w.dump(remotes, f)
+
+    def _ask_api_key(self):
+        log("You have to set your API key.")
+        log("You can get it in your profile page on WhatsOpt (%s)." % self.url)
+        info(
+            "Please, copy/paste your API key below then hit return (characters are hidden)."
+        )
+        api_key = getpass.getpass(prompt="Your API key: ")
+        return api_key
+
+    @staticmethod
+    def is_logged():
+        # Defensive programming: test on api_key should be enough but...
+        return os.path.exists(URL_FILENAME) and os.path.exists(API_KEY_FILENAME)
+
+    @staticmethod
+    def _read_url():
+        if os.path.exists(URL_FILENAME):
+            with open(URL_FILENAME, "r") as f:
+                return f.read()
+        else:
+            return None
+
+    @staticmethod
+    def _read_api_key():
+        if os.path.exists(API_KEY_FILENAME):
+            with open(API_KEY_FILENAME, "r") as f:
+                return f.read()
+        else:
+            return None
+
+    def _write_login_infos(self):
+        if not os.path.exists(WHATSOPT_DIRNAME):
+            os.makedirs(WHATSOPT_DIRNAME)
+        with open(API_KEY_FILENAME, "w") as f:
+            f.write(self.api_key)
+        with open(URL_FILENAME, "w") as f:
+            f.write(self.url)
+
+    def login(self, echo=False, retry=True):
+        debug(f"login(api_key={self.api_key}, echo={echo})")
+
+        # Check login with remote name
+        if not (
+            self.url.startswith("http://") or self.url.startswith("https://")
+        ) and not self._remotes.get(self.url):
+            error(f"Unknown remote server '{self.url}'")
+            WhatsOpt.list_remotes()
+            sys.exit(-1)
+
+        if self._api_key:
+            # api key is provided
+            pass
+        elif self.is_logged():
+            # check if logged in
+            self._api_key = self._read_api_key()
+        else:
+            # check if known remote
+            for _, v in self._remotes.items():
+                if self.url == v["url"]:
+                    self._api_key = v["api_key"]
+                    break
+            # ask for API key otherwise
+            debug("Ask for API key")
+            self._api_key = self._ask_api_key() if not self._api_key else self._api_key
+
+        debug(f"url={self.url}, api_key={self.api_key}")
+        ok = self._test_connection()
+        debug(f"ok={ok}")
+        if not ok and retry:
+            # try to log again
+            # log out silently as one may be logged on another server
+            self.logout(echo=False)
+            self._remotes = {
+                k: v for k, v in self._remotes.items() if v["url"] != self.url
+            }
+            # save url again as is has been wipe out by logout
+            with open(URL_FILENAME, "w") as f:
+                f.write(self._url)
+            return self.login(retry=False)
+
+        # make remote info
+        if ok:
+            self._write_login_infos()
+            remote_name = extract_remote_name(self.url)
+            if remote_name:
+                self._remotes[remote_name] = {"url": self.url, "api_key": self.api_key}
+
+        debug(self._remotes)
+        self._write_remotes(self._remotes)
+
+        if not ok:
+            error("Login to WhatsOpt ({}) failed.".format(self.url))
+            log("")
+            warn("You are not connected.")
+            info("  use `wop login <url>` to connect to a remote WhatsOpt server")
+            info(
+                "  use `wop login <name>` to connect to a known remote WhatsOpt server"
+            )
+            self.list_remotes()
+
+            sys.exit(-1)
+
+        if echo:
+            info(f"Successfully logged in to remote WhatsOpt {self.url}")
+            log("")
+        return self
+
+    @staticmethod
+    def logout(list=None, all=None, remote=None, echo=True):
+        if list:
+            WhatsOpt.list_remotes()
+        elif all:
+            WhatsOpt._write_remotes({})
+            if echo:
+                info("Sucessfully logged out from all WhatsOpt remotes")
+        elif remote:
+            remotes = WhatsOpt._read_remotes()
+            if remotes.get(remote):
+                del remotes[remote]
+                WhatsOpt._write_remotes(remotes)
+                if echo:
+                    info(f"Sucessfully logged out from remote WhatsOpt {remote}")
+        else:
+            if os.path.exists(API_KEY_FILENAME):
+                os.remove(API_KEY_FILENAME)
+            url = WhatsOpt._read_url()
+            if url:
+                os.remove(URL_FILENAME)
+            if echo:
+                if url:
+                    info(f"Sucessfully logged out from remote WhatsOpt {url}")
+                else:
+                    info("Not connected. You may want to connect to:")
+                    WhatsOpt.list_remotes()
+
+        if echo:
+            log("")
+
+    @staticmethod
+    def list_remotes():
+        remotes = WhatsOpt._read_remotes()
+        headers = ["name", "url"]
+        data = []
+        for name, rem in remotes.items():
+            data.append([name, rem["url"]])
+        info("Known remote servers")
+        log(tabulate(data, headers))
+
+    def list_analyses(self, all=False, project_query=None):
+        param = ""
+        if all:
+            param = "?all=true"
+        elif project_query:
+            param = "?design_project_query={}".format(project_query)
+        url = self.endpoint("/api/v1/analyses" + param)
+        resp = self.session.get(url, headers=self.headers)
+        if resp.ok:
+            mdas = resp.json()
+            headers = ["id", "name", "created at"]
+            data = []
+            for mda in mdas:
+                date = mda.get("created_at", None)
+                data.append([mda["id"], mda["name"], date])
+            log(tabulate(data, headers))
+            log("")
+        else:
+            resp.raise_for_status()
+
+    def is_connected(self):
+        return self._test_connection()
+
+    def get_status(self):
+        connected = self.is_connected()
+        whatsopt_url = get_whatsopt_url() or self.url
+        if connected:
+            info("You are logged in {}".format(self.url))
+        else:
+            info("You are not connected.")
+        mda_id = None
+        try:
+            mda_id = get_analysis_id()
+        except ValueError as err:
+            warn(str(err))
+        if mda_id:
+            if connected and whatsopt_url == self.url:
+                info("Found local analysis code (id=#{})".format(mda_id))
+                # connected to the right server from which the analysis was pulled
+                url = self.endpoint("/api/v1/analyses/{}".format(mda_id))
+                resp = self.session.get(url, headers=self.headers)
+
+                if resp.ok:
+                    mda = resp.json()
+                    if is_based_on(FRAMEWORK_GEMSEO):
+                        mda["framework"] = "GEMSEO"
+                    elif is_based_on(FRAMEWORK_OPENMDAO):
+                        mda["framework"] = "OpenMDAO"
+                    else:  # should not happen
+                        raise ValueError(
+                            "No framework detected. Check your *_base.py files."
+                        )
+                    headers = ["id", "name", "created_at", "owner_email", "framework"]
+                    data = [[mda[k] for k in headers]]
+                    log(tabulate(data, headers))
+                else:
+                    error("Analysis not found on the server anymore (probably deleted)")
+                    log(
+                        "  (use 'wop push <analysis.py>' to push from an OpenMDAO code to the server)"
+                    )
+            else:
+                info(
+                    "Found local analysis code (id=#{}) "
+                    "pulled from {}".format(mda_id, whatsopt_url)
+                )
+                if connected:
+                    # connected to another server with a pulled analysis
+                    warn("You are connected to a different server")
+                    log(
+                        "  (use 'wop push <analysis.py>' to push from the local "
+                        f"analysis code to the server {self.url})"
+                    )
+                    log(
+                        f"  (use 'wop logout' and 'wop login {whatsopt_url}' "
+                        "to log in to the original server)"
+                    )
+                else:
+                    log(f"  (use 'wop login {whatsopt_url}' command to log in)")
+        else:
+            info("No local analysis found")
+            if connected:
+                log(
+                    "  (use 'wop list' and 'wop pull <id>' to retrieve an existing analysis)\n"
+                    "  (use 'wop push <analysis.py>' to push from the local OpenMDAO code to the server)"
+                )
+        log("")
+
+    def push_component_cmd(self, py_filename, component, options):
+        with problem_pyfile(py_filename, component) as pyf:
+            if options["--dry-run"]:
+                with open(pyf, "r") as pbf:
+                    print(pbf.read())
+                    sys.exit()
+            self.push_mda_cmd(pyf, options)
+
+    def push_mda_cmd(self, py_filename, options):
+        def push_mda(prob):
+            name = options["--name"]
+            pbname = prob.model.__class__.__name__
+            if name and pbname != name:
+                info("Analysis %s skipped" % pbname)
+                # do not exit seeking for another problem (ie analysis)
+            else:
+                options["--pyfilename"] = py_filename
+                xdsm = self.push_mda(prob, options)
+                if options.get("--xdsm"):  # show command
+                    # required to interrupt pb execution
+                    raise AnalysisPushedException(xdsm=xdsm)
+                else:
+                    sys.exit()
+
+        hooks.use_hooks = True
+        hooks._register_hook("final_setup", "Problem", post=push_mda)
+        _load_and_exec(py_filename, [])
+        return push_mda
+
+    def push_mda(self, problem, options):
+        scalar = options.get("--scalar")
+        depth = options.get("--depth")
+        push_cmd = PushCommand(problem, depth, scalar)
+
+        mda_attrs = push_cmd.get_mda_attributes(
+            problem.model, push_cmd.tree, use_depth=True
+        )
+
+        if mda_attrs["name"] == "Group" and options.get("--pyfilename"):
+            mda_attrs["name"] = os.path.splitext(
+                to_camelcase(os.path.basename(options.get("--pyfilename")))
+            )[0]
+
+        if options["--dry-run"]:
+            log(json.dumps(mda_attrs, indent=2))
+        else:
+            suffix = ""
+            if options.get("--xdsm"):
+                suffix = ".xdsm"
+            url = self.endpoint("/api/v1/analyses{}".format(suffix))
+            resp = self.session.post(
+                url, headers=self.headers, json={"analysis": mda_attrs}
+            )
+            resp.raise_for_status()
+            log("Analysis %s pushed" % mda_attrs["name"])
+            return resp.json()
+
+    def push_json(self, filename):
+        with open(filename, "rb") as f:
+            attrs = json.load(f)
+        if "analyses_attributes" in attrs:  # project detection
+            url = self.endpoint("/api/v1/design_projects")
+            key = "Project"
+        else:
+            url = self.endpoint("/api/v1/analyses")
+            key = "Analysis"
+        params = {}
+        params[key.lower()] = attrs
+        resp = self.session.post(url, headers=self.headers, json=params)
+        resp.raise_for_status()
+        log("{} {} pushed".format(key, attrs["name"]))
+
+    def pull_mda(self, mda_id, options={}, msg=None, info_keep_run_ops=True):
+        if not msg:
+            msg = "Analysis %s pulled" % mda_id
+
+        framework = FRAMEWORK_OPENMDAO
+        if options.get("--gemseo"):
+            framework = FRAMEWORK_GEMSEO
+
+        param = ""
+        if options.get("--run-ops"):
+            param += "&with_runops=true"
+        if options.get("--server"):
+            if framework == FRAMEWORK_OPENMDAO:
+                param += "&with_server=true"
+            else:
+                warn(
+                    "Can not generate server with GEMSEO framework. --server is ignored"
+                )
+        if options.get("--egmdo"):
+            if framework == FRAMEWORK_OPENMDAO:
+                param += "&with_egmdo=true"
+            else:
+                warn("Can not generate EGMDO with GEMSEO framework. --egmdo is ignored")
+        if options.get("--test-units"):
+            if framework == FRAMEWORK_OPENMDAO:
+                param += "&with_unittests=true"
+            else:
+                warn(
+                    "Can not generate tests with GEMSEO framework. --test-units is ignored"
+                )
+        if param:
+            param = "?" + param[1:]
+
+        format_query = framework
+        if options.get("--package"):
+            format_query += "_pkg"
+
+        url = self.endpoint(
+            ("/api/v1/analyses/{}/exports/new.{}{}".format(mda_id, format_query, param))
+        )
+        resp = self.session.get(url, headers=self.headers, stream=True)
+        resp.raise_for_status()
+        name = None
+        with tempfile.NamedTemporaryFile(suffix=".zip", mode="wb", delete=False) as fd:
+            for chunk in resp.iter_content(chunk_size=128):
+                fd.write(chunk)
+            name = fd.name
+        zipf = zipfile.ZipFile(name, "r")
+        tempdir = tempfile.mkdtemp(suffix="wop", dir=tempfile.tempdir)
+        zipf.extractall(tempdir)
+        filenames = zipf.namelist()
+        zipf.close()
+        file_to_move = {}
+        if options.get("--dry-run"):
+            cmd = "Pull"
+            if options.get("--update"):
+                cmd = "Update"
+            info(
+                "***************************************************\n"
+                f"* DRY RUN mode (actions are listed but not done) *\n"
+                "***************************************************"
+            )
+
+        # Special case: When framework switch we have to update
+        # user analysis main file which name depends on package name
+        framework_switch = is_framework_switch(framework)
+        if framework_switch:
+            url = self.endpoint(f"/api/v1/analyses/{mda_id}/openmdao_impl")
+            resp = self.session.get(url, headers=self.headers, stream=True)
+            resp.raise_for_status()
+            mda_name = resp.json()["packaging"]["package_name"]
+        else:
+            mda_name = ""
+
+        for f in filenames:
+            file_to = f
+            file_to_move[file_to] = True
+            if os.path.exists(file_to):
+                if options.get("--force"):
+                    log(f"Update {file_to}")
+                    if options.get("--dry-run"):
+                        file_to_move[file_to] = False
+                    else:
+                        os.remove(file_to)
+                elif options.get("--update"):
+                    if is_run_script_file(f) and not options.get("--run-ops"):
+                        if info_keep_run_ops:
+                            info(f"Keep existing {file_to} (use -r to override)")
+                        file_to_move[file_to] = False
+                        continue
+                    if is_test_file(f) and not options.get("--test-units"):
+                        file_to_move[file_to] = False
+                        continue
+                    if is_user_file(f):
+                        file_to_move[file_to] = False
+                        # Have to update user analysis main file when switching frameworks
+                        if is_framework_switch and is_analysis_user_file(mda_name, f):
+                            file_to_move[file_to] = True
+                        else:
+                            continue
+                    log(f"Update {file_to}")
+                    if not options.get("--dry-run"):
+                        os.remove(file_to)
+                else:
+                    warn(
+                        f"File {file_to} in the way: remove it or use --force to override"
+                    )
+                    file_to_move[file_to] = False
+            else:
+                if options.get("--force"):
+                    log(f"Pull {file_to}")
+                    if options.get("--dry-run"):
+                        file_to_move[file_to] = False
+                elif options.get("--update") and (
+                    (is_run_script_file(f) and not options.get("--run-ops"))
+                    or (is_test_file(f) and not options.get("--test-units"))
+                    or is_user_file(f)
+                ):
+                    file_to_move[file_to] = False
+                else:
+                    log(f"Pull {file_to}")
+
+        if not options.get("--dry-run"):
+            move_files(file_to_move, tempdir)
+            state = {
+                "whatsopt_url": self._url,
+                "analysis_id": mda_id,
+                "framework": framework,
+                "pull_mode": MODE_PACKAGE if options.get("--package") else MODE_PLAIN,
+            }
+            save_state(state)
+            info(msg)
+
+    def pull_mda_json(self, mda_id):
+        url = self.endpoint(f"/api/v1/analyses/{mda_id}.wopjson")
+        resp = self.session.get(url, headers=self.headers, stream=True)
+        resp.raise_for_status()
+        print(json.dumps(resp.json()))
+
+    def pull_project_json(self, project_id):
+        url = self.endpoint(f"/api/v1/design_projects/{project_id}.wopjson")
+        resp = self.session.get(url, headers=self.headers, stream=True)
+        resp.raise_for_status()
+        print(json.dumps(resp.json()))
+
+    def update_mda(self, analysis_id=None, options={}, info_keep_run_ops=True):
+        mda_id = analysis_id or get_analysis_id()
+        if mda_id and not analysis_id:
+            url = get_whatsopt_url()
+            if url != self.url:
+                warn(
+                    f"You want to update code pulled from {url} while you are logged in {self.url}."
+                )
+                info(
+                    f"  use 'wop login {url}' and retry to update using the original remote."
+                )
+                info(
+                    f"  use 'wop update -a <id>' to update using analysis #<id> from {self.url}."
+                )
+                sys.exit(-1)
+        if mda_id is None:
+            error(
+                f"Unknown analysis with id=#{mda_id} (maybe use wop pull <analysis-id>)"
+            )
+            sys.exit(-1)
+        # keep options unchanged, work on a copy
+        opts = copy.deepcopy(options)
+        # sanity checks
+        if not (is_based_on(FRAMEWORK_OPENMDAO) or is_based_on(FRAMEWORK_GEMSEO)):
+            error("No framework detected. Check your *_base.py files.")
+            sys.exit(-1)
+        if opts["--openmdao"] and opts["--gemseo"]:
+            error("Please choose either --openmdao or --gemseo.")
+            sys.exit(-1)
+        opts.update(
+            {
+                "--base": True,
+                "--update": True,
+                "--gemseo": opts["--gemseo"]
+                or (not opts["--openmdao"] and is_based_on(FRAMEWORK_GEMSEO)),
+                "--openmdao": opts["--openmdao"]
+                or (not opts["--gemseo"] and is_based_on(FRAMEWORK_OPENMDAO)),
+                "--package": is_package_mode(),
+            }
+        )
+        self.pull_mda(
+            mda_id, opts, "Analysis #{} updated".format(mda_id), info_keep_run_ops
+        )
+
+    def show_mda(self, analysis_id, pbfile, name, outfile, batch, depth):
+        options = {
+            "--xdsm": True,
+            "--name": name,
+            "--dry-run": False,
+            "--depth": depth,
+        }
+        xdsm = None
+        if pbfile:
+            start = time.time()
+            try:
+                info("XDSM info retrieval...")
+                self.push_mda_cmd(pbfile, options)
+            except AnalysisPushedException as pushed:
+                xdsm = pushed.xdsm
+            end = time.time()
+            log("Retrieved in {:.2f}s".format(end - start))
+            source = os.path.basename(pbfile)
+        else:
+            mda_id = analysis_id or get_analysis_id()
+            if mda_id is None:
+                error(
+                    "Unknown analysis with id={} (maybe use wop pull <analysis-id>)".format(
+                        mda_id
+                    )
+                )
+                sys.exit(-1)
+            url = self.endpoint("/api/v1/analyses/{}.xdsm".format(mda_id))
+            resp = self.session.get(url, headers=self.headers)
+            resp.raise_for_status()
+            xdsm = resp.json()
+            source = f"{mda_id}@{self._url}"
+
+        info("XDSM building...")
+        generate_xdsm_html(source, xdsm, outfile)
+        if pbfile:
+            log("XDSM of analysis from {} generated in {}".format(pbfile, outfile))
+        else:
+            log("XDSM of analysis {} generated in {}".format(mda_id, outfile))
+        if not batch:
+            webview(outfile)
+
+    def upload(
+        self,
+        filename,
+        driver_kind=None,
+        analysis_id=None,
+        operation_id=None,
+        dry_run=False,
+        outvar_count=1,
+        only_success=False,
+        parallel=False,
+    ):
+        from socket import gethostname
+
+        mda_id = get_analysis_id() if not analysis_id else analysis_id
+
+        # Test sqlite files generated with MPI
+        _, extension = os.path.splitext(filename)
+        parallel_sqlite = re.match(r"\.sqlite_\d+$", extension)
+
+        name = cases = statuses = None
+        if not os.path.exists(filename):
+            error(f"File not found ({filename})")
+            sys.exit(-1)
+        if os.path.basename(filename) == "mda_init.py":
+            self.upload_vars_init_cmd(
+                filename, {"--dry-run": dry_run, "--analysis-id": mda_id}
+            )
+        elif filename.endswith(".csv"):
+            name, cases, statuses = load_from_csv(filename)
+        elif filename.endswith(".sqlite") or (parallel_sqlite and parallel):
+            name, cases, statuses = load_from_sqlite(filename, parallel)
+        elif filename.endswith(".hdf5"):
+            name, cases, statuses = load_from_hdf5(filename)
+        else:
+            error(
+                f"Can not upload file {filename}: extension not recognized"
+                " (should be either .csv, .sqlite or .hdf5)"
+            )
+            sys.exit(-1)
+
+        if only_success:
+            for c in cases:
+                c["values"] = [
+                    val for i, val in enumerate(c["values"]) if statuses[i] > 0
+                ]
+            statuses = [1 for s in statuses if s > 0]
+
+        for c in cases:
+            c["values"] = np.nan_to_num(np.array(c["values"])).tolist()
+
+        if dry_run:
+            print_cases(cases, statuses)
+            sys.exit()
+
+        resp = None
+        if operation_id:
+            url = self.endpoint(("/api/v1/operations/%s") % operation_id)
+            operation_params = {"cases": cases}
+            resp = self.session.patch(
+                url, headers=self.headers, json={"operation": operation_params}
+            )
+        else:
+            if mda_id:
+                url = self.endpoint(("/api/v1/analyses/%s/operations") % mda_id)
+            else:
+                url = self.endpoint("/api/v1/operations")
+            if driver_kind:
+                driver = "user_{}_algo".format(driver_kind)
+            else:
+                # suppose name well-formed <lib>-<doe|optimizer|screening>-<algoname>
+                # otherwise it will default to doe
+                m = re.match(r"(\w+)_(doe|optimizer|screening)_(\w+)", name.lower())
+                if m:
+                    driver = name.lower()
+                else:
+                    driver = "user_data_uploading"
+            operation_params = {
+                "name": name,
+                "driver": driver,
+                "host": gethostname(),
+                "cases": cases,
+                "success": statuses,
+            }
+            params = {"operation": operation_params}
+            if outvar_count > 0 and outvar_count < len(cases):
+                params["outvar_count_hint"] = outvar_count
+            resp = self.session.post(url, headers=self.headers, json=params)
+        resp.raise_for_status()
+        log("Results data from {} uploaded with driver {}".format(filename, driver))
+
+    def upload_vars_init_cmd(self, py_filename, options):
+        def upload_vars_init(prob):
+            self.upload_vars_init(prob, options)
+            sys.exit()
+
+        d = os.path.dirname(py_filename)
+        run_mda_filename = os.path.join(d, "run_mda.py")
+        if not os.path.exists(run_mda_filename):
+            error(f"Can not get analysis init: script {run_mda_filename} not found.")
+        hooks.use_hooks = True
+        hooks._register_hook("final_setup", "Problem", post=upload_vars_init)
+        _load_and_exec(run_mda_filename, [])
+
+    def upload_vars_init(self, problem, options):
+        mda_id = get_analysis_id() if get_analysis_id() else options["--analysis-id"]
+        if mda_id is None:
+            error("Unknown analysis with id={}".format(mda_id))
+            sys.exit(-1)
+        parameters = []
+        headers = ["variable", "init value"]
+        data = []
+        for s in problem.model._subsystems_myproc:
+            if isinstance(s, IndepVarComp):
+                for absname in s._var_abs2meta["output"]:
+                    name = find_indep_var_name(problem, absname)
+                    value = s._outputs._views[absname][:]
+                    if isinstance(value, np.ndarray):
+                        value = str(value.tolist())
+                    parameters.append({"varname": name, "value": value})
+        data = [[p["varname"], p["value"]] for p in parameters]
+        params = {"parameterization": {"parameters": parameters}}
+        log(tabulate(data, headers))
+        if not options["--dry-run"]:
+            url = self.endpoint(f"/api/v1/analyses/{mda_id}/parameterization")
+            resp = self.session.put(url, headers=self.headers, json=params)
+            resp.raise_for_status()
+            log("Variables init values uploaded")
+
+    def check_versions(self):
+        url = self.endpoint("/api/v1/versioning")
+        resp = self.session.get(url, headers=self.headers)
+        resp.raise_for_status()
+        version = resp.json()
+        log("WhatsOpt {} requires wop {}".format(version["whatsopt"], version["wop"]))
+        log(f"You are using wop {__version__}")
+
+    @staticmethod
+    def serve(port):
+        try:
+            import thrift
+        except ImportError:
+            error(
+                "Apache Thrift is not installed. You can install it with : 'pip install thrift'"
+            )
+            sys.exit(-1)
+        try:
+            import os, sys
+
+            # insert current dir first as another run_server exists under whatsopt/services
+            sys.path.insert(0, os.getcwd())
+            from run_server import run_server
+        except ImportError as err:
+            print(str(err))
+            error("Server not found!")
+            try:
+                mda_id = get_analysis_id()
+                if mda_id:
+                    log(
+                        f"  (use 'wop update -s' to generate server for current analysis #{mda_id})"
+                    )
+                else:
+                    warn("No local analysis found")
+                    log(
+                        "  (use 'wop pull -s <id>' to generate server for the analysis #id)"
+                    )
+            except ValueError as err:
+                warn(str(err))
+            sys.exit(-1)
+        run_server(port)
+
+    @staticmethod
+    def convert(filename):
+        if not os.path.exists(filename):
+            error(f"File {filename} not found.")
+        pathname, extension = os.path.splitext(filename)
+        if not (extension == ".sqlite" or re.match(r"\.sqlite_\d+$", extension)):
+            warn(
+                f"File {filename} should have '.sqlite[_n]' extension, got '{extension}'"
+            )
+        basename = os.path.basename(pathname)
+        convert_sqlite_to_csv(filename, basename)
+
+    def publish(self, force=False, analysis_id=None):
+        mda_id = analysis_id if analysis_id else get_analysis_id()
+        url = self.endpoint(f"/api/v1/analyses/{mda_id}/package")
+        if not force:
+            resp = self.session.get(url, headers=self.headers)
+            if resp.ok:
+                existing_meta = resp.json()
+            elif resp.status_code == HTTPStatus.NOT_FOUND:
+                existing_meta = None
+            else:
+                resp.raise_for_status()
+
+            if existing_meta:
+                warn(
+                    f"Existing package {existing_meta['name']} {existing_meta['version']} will be lost."
+                )
+                answer = input("Do you want to continue? (yes/no): ")
+                if answer.lower() == "yes":
+                    pass
+                else:
+                    info("Publishing aborted")
+                    exit(-1)
+
+        info("Package building...")
+        filename = self.build()
+        if not os.path.exists(filename):
+            error(f"File {filename} not found")
+            exit(-1)
+        meta = get_pkg_metadata(filename)
+        if (
+            not force
+            and existing_meta
+            and existing_meta["name"] == meta.name
+            and Version(existing_meta["version"]) >= Version(meta.version)
+        ):
+            error(f"You have to bump the version (> {existing_meta['version']})")
+            error("Publishing aborted")
+            exit(-1)
+
+        files = {
+            "package[description]": (None, meta.summary, "application/json"),
+            "package[archive]": (filename, open(filename, "rb"), "application/gzip"),
+        }
+        info("Package publishing...")
+        resp = self.session.post(url, headers=self.headers, files=files)
+        if resp.ok:
+            info(
+                f"Package {meta.name} v{meta.version} is published on WopStore({self.endpoint('/packages')})"
+            )
+        elif resp.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+            error(resp.json()["message"])
+            error("Duplicate detected! The package already exists on WopStore!")
+            exit(-1)
+        else:
+            resp.raise_for_status()
+
+    def build(self):
+        if not is_package_mode():
+            error("Package mode is required!")
+            exit(-1)
+        self._update_mda_base()
+        filename = build_package()
+        return filename
+
+    def fetch(self, source_id=None, options={}):
+        if not is_package_mode():
+            error("Package mode is required!")
+            exit(-1)
+        mda_id = get_analysis_id()
+        param = f"?src_id={source_id}"
+        format_query = "mda_pkg_content"
+        url = self.endpoint(
+            f"/api/v1/analyses/{mda_id}/exports/new.{format_query}{param}"
+        )
+        resp = self.session.get(url, headers=self.headers, stream=True)
+        if resp.ok:
+            name = None
+            with tempfile.NamedTemporaryFile(
+                suffix=".zip", mode="wb", delete=False
+            ) as fd:
+                for chunk in resp.iter_content(chunk_size=128):
+                    fd.write(chunk)
+                name = fd.name
+            zipf = zipfile.ZipFile(name, "r")
+            tempdir = tempfile.mkdtemp(suffix="wop", dir=tempfile.tempdir)
+            zipf.extractall(tempdir)
+            filenames = zipf.namelist()
+            if not filenames:
+                warn(
+                    f"Fetching but no package found for analysis #{source_id}, nothing to do"
+                )
+                return
+            zipf.close()
+
+            file_to_move = {}
+            for f in filenames:
+                file_to = f
+                file_to_move[file_to] = True
+                if os.path.exists(file_to):
+                    if options.get("--force"):
+                        log(f"Fetch {file_to}")
+                        if options.get("--dry-run"):
+                            file_to_move[file_to] = False
+                        else:
+                            os.remove(file_to)
+                    else:
+                        warn(
+                            f"File {file_to} in the way: remove it or use --force to override"
+                        )
+                        file_to_move[file_to] = False
+                else:
+                    log(f"Fetch {file_to}")
+            if not options.get("--dry-run"):
+                move_files(file_to_move, tempdir)
+                info(f"Analysis #{source_id} disciplines fetched")
+        else:
+            error(f"Error while fetching disciplines of analysis #{source_id}")
+            error(resp.json().get("message"))
+
+    def merge(self, source_id, options={}):
+        if not is_package_mode():
+            error("Package mode is required!")
+            exit(-1)
+        current_id = get_analysis_id()
+        if int(source_id) == current_id:
+            warn(f"Merging analysis #{current_id} in itself, nothing to do")
+            return
+        url = self.endpoint(f"/api/v1/analyses/{current_id}")
+        params = {
+            "analysis": {
+                "import": {"analysis": source_id},
+            },
+            "requested_at": str(datetime.now()),
+        }
+        if options.get("--dry-run"):
+            self.get_status()
+            url = self.endpoint("/api/v1/analyses/{}".format(source_id))
+            resp = self.session.get(url, headers=self.headers)
+            log(f"Analysis #{source_id} #{resp.json()} is selected to be merged")
+        else:
+            resp = self.session.put(url, headers=self.headers, json=params)
+        if resp.ok:
+            if not options.get("--dry-run"):
+                info(f"Analysis #{source_id} merged")
+        elif resp.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+            error(f"Error while merging analysis #{source_id}.")
+            error(
+                f"    Check analyses, maybe they are not compatible (same variable produced by different disciplines)"
+            )
+        elif resp.status_code == HTTPStatus.FORBIDDEN:
+            error(f"Error while merging analysis #{source_id}.")
+            error(
+                f"    You are not authorized to update the current analysis: either you do not own it or"
+                f" current analysis is already packaged or operated"
+            )
+        else:
+            error(f"Error while merging analysis #{source_id}")
+            resp.raise_for_status()
+
+    def pull_source_mda(self, source_id, options={}):
+        self.merge(source_id, options)
+        self.fetch(source_id, options)
+        self._update_mda_base(options.get("--dry-run"))
+
+    def _update_mda_base(self, dry_run=False, force=False):
+        update_options = {
+            "--dry-run": dry_run,
+            "--force": force,
+            "--server": False,
+            "--egmdo": False,
+            "--run-ops": False,
+            "--test-units": False,
+            "--gemseo": is_based_on(FRAMEWORK_GEMSEO),
+            "--openmdao": is_based_on(FRAMEWORK_OPENMDAO),
+        }
+        mda_id = get_analysis_id()
+        self.update_mda(mda_id, update_options, info_keep_run_ops=False)
+
+    def _test_connection(self):
+        if self.api_key:
+            self.headers = {
+                "Authorization": "Token token=" + self.api_key,
+                "User-Agent": "wop/{}".format(__version__),
+            }
+            url = self.endpoint("/api/v1/versioning")
+            debug(f"Test connect: {url}, {self.api_key}")
+            try:
+                resp = self.session.get(url, headers=self.headers)
+                # special case: bad wop version < minimal required version
+                if resp.status_code == requests.codes.forbidden:
+                    error(resp.json()["message"])
+                    sys.exit(-1)
+                return resp.ok
+            except requests.exceptions.ConnectionError:
+                return False
+        else:
+            return False
```

### Comparing `wop-2.5.2/wop.egg-info/PKG-INFO` & `wop-2.5.3/wop.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-Metadata-Version: 2.1
-Name: wop
-Version: 2.5.2
-Summary: My package description
-Author-email: Rémi Lafage <remi.lafage@onera.fr>
-License: Apache License 2.0
-Project-URL: homepage, https://github.com/whatsopt
-Project-URL: repository, https://github.com/whatsopt/WhatsOpt-CLI
-Project-URL: documentation, https://github.com/whatsopt/WhatsOpt-Doc#whatsopt-documentation
-Keywords: WhatsOpt,command
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
-[![Tests](https://github.com/OneraHub/WhatsOpt-CLI/workflows/Tests/badge.svg)](https://github.com/OneraHub/WhatsOpt-CLI/actions?query=workflow%3ATests)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/78559b54a0db44e5aeb5b0a3f5dcf9e2)](https://www.codacy.com/gh/OneraHub/WhatsOpt-CLI/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=OneraHub/WhatsOpt-CLI&amp;utm_campaign=Badge_Grade)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
-
-# WhatsOpt command line interface
-
-Command line interface to interact with WhatsOpt web application. See [WhatsOpt documentation](https://github.com/OneraHub/WhatsOpt-Doc).
-
-## Citation
->Rémi  Lafage,  Sébastien  Defoort,  and  Thierry  Lefèbvre. Whatsopt: a web application for multidisciplinary design analysis and optimization. In 20th AIAA/ISSMO Multidisciplinary Analysis and Optimization Conference, Dallas, United States, 2019
-
-DOI: [10.2514/6.2019-2990](https://doi.org/10.2514/6.2019-2990)
-
-## Installation
-```bash
-pip install wop
-```
-
-## Usage
-```bash
-wop --help
-```
-
-```bash
-wop <COMMAND> --help
-```
-
-## License
-
-   Copyright 2020 Rémi Lafage
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+Metadata-Version: 2.1
+Name: wop
+Version: 2.5.3
+Summary: My package description
+Author-email: Rémi Lafage <remi.lafage@onera.fr>
+License: Apache License 2.0
+Project-URL: homepage, https://github.com/whatsopt
+Project-URL: repository, https://github.com/whatsopt/WhatsOpt-CLI
+Project-URL: documentation, https://github.com/whatsopt/WhatsOpt-Doc#whatsopt-documentation
+Keywords: WhatsOpt,command
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
+[![Tests](https://github.com/OneraHub/WhatsOpt-CLI/workflows/Tests/badge.svg)](https://github.com/OneraHub/WhatsOpt-CLI/actions?query=workflow%3ATests)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/78559b54a0db44e5aeb5b0a3f5dcf9e2)](https://www.codacy.com/gh/OneraHub/WhatsOpt-CLI/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=OneraHub/WhatsOpt-CLI&amp;utm_campaign=Badge_Grade)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+
+# WhatsOpt command line interface
+
+Command line interface to interact with WhatsOpt web application. See [WhatsOpt documentation](https://github.com/OneraHub/WhatsOpt-Doc).
+
+## Citation
+>Rémi  Lafage,  Sébastien  Defoort,  and  Thierry  Lefèbvre. Whatsopt: a web application for multidisciplinary design analysis and optimization. In 20th AIAA/ISSMO Multidisciplinary Analysis and Optimization Conference, Dallas, United States, 2019
+
+DOI: [10.2514/6.2019-2990](https://doi.org/10.2514/6.2019-2990)
+
+## Installation
+```bash
+pip install wop
+```
+
+## Usage
+```bash
+wop --help
+```
+
+```bash
+wop <COMMAND> --help
+```
+
+## License
+
+   Copyright 2020 Rémi Lafage
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `wop-2.5.2/wop.egg-info/SOURCES.txt` & `wop-2.5.3/wop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

