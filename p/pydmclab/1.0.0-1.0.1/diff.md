# Comparing `tmp/pydmclab-1.0.0.tar.gz` & `tmp/pydmclab-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydmclab-1.0.0.tar", last modified: Sat Apr 29 17:44:37 2023, max compression
+gzip compressed data, was "pydmclab-1.0.1.tar", last modified: Mon Jun 26 22:25:05 2023, max compression
```

## Comparing `pydmclab-1.0.0.tar` & `pydmclab-1.0.1.tar`

### file list

```diff
@@ -1,81 +1,87 @@
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.461262 pydmclab-1.0.0/
--rw-------   0 cbartel    (503) staff       (20)     1071 2023-04-03 21:26:17.000000 pydmclab-1.0.0/LICENSE.txt
--rw-------   0 cbartel    (503) staff       (20)      173 2023-04-03 21:38:56.000000 pydmclab-1.0.0/MANIFEST.in
--rw-r--r--   0 cbartel    (503) staff       (20)      642 2023-04-29 17:44:37.461028 pydmclab-1.0.0/PKG-INFO
--rw-------   0 cbartel    (503) staff       (20)      170 2023-04-05 14:50:32.000000 pydmclab-1.0.0/README.md
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.363164 pydmclab-1.0.0/pydmclab/
--rw-------   0 cbartel    (503) staff       (20)      245 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/__init__.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.379480 pydmclab-1.0.0/pydmclab/core/
--rw-------   0 cbartel    (503) staff       (20)      398 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/core/README.md
--rw-------   0 cbartel    (503) staff       (20)      176 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/core/__init__.py
--rw-------   0 cbartel    (503) staff       (20)     3895 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/core/comp.py
--rw-r--r--   0 cbartel    (503) staff       (20)    12187 2023-04-03 21:34:13.000000 pydmclab-1.0.0/pydmclab/core/energies.py
--rw-------   0 cbartel    (503) staff       (20)    52660 2023-04-29 17:43:03.000000 pydmclab-1.0.0/pydmclab/core/hulls.py
--rw-------   0 cbartel    (503) staff       (20)    12067 2023-04-03 21:34:25.000000 pydmclab-1.0.0/pydmclab/core/mag.py
--rw-------   0 cbartel    (503) staff       (20)    15189 2023-04-03 21:34:29.000000 pydmclab-1.0.0/pydmclab/core/query.py
--rw-------   0 cbartel    (503) staff       (20)    13148 2023-04-10 22:21:48.000000 pydmclab-1.0.0/pydmclab/core/struc.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.394135 pydmclab-1.0.0/pydmclab/data/
--rw-r--r--   0 cbartel    (503) staff       (20)     6148 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/.DS_Store
--rw-------   0 cbartel    (503) staff       (20)      346 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/README.md
--rw-------   0 cbartel    (503) staff       (20)      331 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/__init__.py
--rw-------   0 cbartel    (503) staff       (20)      916 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/configs.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.437059 pydmclab-1.0.0/pydmclab/data/data/
--rw-r--r--   0 cbartel    (503) staff       (20)    15963 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/221220_dmc-mus.json
--rw-r--r--   0 cbartel    (503) staff       (20)     7720 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/230122_dmc-mus.json
--rw-r--r--   0 cbartel    (503) staff       (20)     1241 2023-04-17 14:02:36.000000 pydmclab-1.0.0/pydmclab/data/data/_batch_vasp_analysis_configs.yaml
--rw-------   0 cbartel    (503) staff       (20)      437 2023-04-17 14:52:59.000000 pydmclab-1.0.0/pydmclab/data/data/_launch_configs.yaml
--rw-------   0 cbartel    (503) staff       (20)     1496 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/_partition_configs.yaml
--rw-------   0 cbartel    (503) staff       (20)      573 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/_slurm_configs.yaml
--rw-r--r--   0 cbartel    (503) staff       (20)     1414 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/_sub_configs.yaml
--rw-------   0 cbartel    (503) staff       (20)     1561 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/_vasp_configs.yaml
--rw-------   0 cbartel    (503) staff       (20)     1570 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/atomic_masses.json
--rw-r--r--   0 cbartel    (503) staff       (20)     3140 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/bartel2019_npj_reference-energies.csv
--rw-r--r--   0 cbartel    (503) staff       (20)     2596 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/colors.json
--rw-------   0 cbartel    (503) staff       (20)    40326 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/elemental_gibbs_energies_T.json
--rw-r--r--   0 cbartel    (503) staff       (20)     3788 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/mus_from_bartel2019_npj.json
--rw-r--r--   0 cbartel    (503) staff       (20)     7719 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/mus_from_dmc_no_corrections.json
--rw-------   0 cbartel    (503) staff       (20)     1710 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/mus_from_mp_no_corrections.json
--rw-------   0 cbartel    (503) staff       (20)    43287 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/ssub.dat
--rw-r--r--   0 cbartel    (503) staff       (20)    45994 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/data/ssub.json
--rw-------   0 cbartel    (503) staff       (20)      246 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/data/features.py
--rw-r--r--   0 cbartel    (503) staff       (20)     2252 2023-04-03 21:35:30.000000 pydmclab-1.0.0/pydmclab/data/plotting_configs.py
--rw-r--r--   0 cbartel    (503) staff       (20)     4026 2023-04-03 21:35:26.000000 pydmclab-1.0.0/pydmclab/data/thermochem.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.445374 pydmclab-1.0.0/pydmclab/demos/
--rw-------   0 cbartel    (503) staff       (20)     2990 2023-04-03 21:35:25.000000 pydmclab-1.0.0/pydmclab/demos/demo_comp.py
--rw-------   0 cbartel    (503) staff       (20)    10887 2023-04-26 22:19:29.000000 pydmclab-1.0.0/pydmclab/demos/demo_hulls.py
--rw-r--r--   0 cbartel    (503) staff       (20)    32860 2023-04-17 22:09:59.000000 pydmclab-1.0.0/pydmclab/demos/demo_launcher_template.py
--rw-------   0 cbartel    (503) staff       (20)     4333 2023-04-03 21:35:45.000000 pydmclab-1.0.0/pydmclab/demos/demo_query.py
--rw-------   0 cbartel    (503) staff       (20)     2494 2023-04-03 21:35:23.000000 pydmclab-1.0.0/pydmclab/demos/demo_struc.py
--rw-------   0 cbartel    (503) staff       (20)    27730 2023-04-17 14:10:29.000000 pydmclab-1.0.0/pydmclab/demos/demo_vasp_template.py
--rw-------   0 cbartel    (503) staff       (20)    28183 2023-04-04 14:55:15.000000 pydmclab-1.0.0/pydmclab/demos/demo_vasp_test-mp-chemsys.py
--rw-------   0 cbartel    (503) staff       (20)    28075 2023-04-03 21:55:19.000000 pydmclab-1.0.0/pydmclab/demos/demo_vasp_test-template.py
--rw-------   0 cbartel    (503) staff       (20)    28376 2023-04-03 21:55:14.000000 pydmclab-1.0.0/pydmclab/demos/demo_vasp_test-transform-strucs.py
--rw-------   0 cbartel    (503) staff       (20)    28254 2023-04-03 21:55:09.000000 pydmclab-1.0.0/pydmclab/demos/demo_vasp_test-typical-dmc.py
--rw-r--r--   0 cbartel    (503) staff       (20)    23914 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/demos/tmp.png
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.449517 pydmclab-1.0.0/pydmclab/dev/
--rw-r--r--   0 cbartel    (503) staff       (20)      153 2023-04-19 19:26:44.000000 pydmclab-1.0.0/pydmclab/dev/Untitled-2.py
--rw-------   0 cbartel    (503) staff       (20)       48 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/dev/__init__.py
--rw-r--r--   0 cbartel    (503) staff       (20)     7018 2023-04-29 17:42:52.000000 pydmclab-1.0.0/pydmclab/dev/echem.py
--rw-------   0 cbartel    (503) staff       (20)     3091 2023-04-03 21:37:38.000000 pydmclab-1.0.0/pydmclab/dev/entries.py
--rw-------   0 cbartel    (503) staff       (20)      170 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/dev/grand.py
--rw-r--r--   0 cbartel    (503) staff       (20)     3911 2023-04-03 21:36:53.000000 pydmclab-1.0.0/pydmclab/dev/reactions.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.455356 pydmclab-1.0.0/pydmclab/hpc/
--rw-------   0 cbartel    (503) staff       (20)      707 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/hpc/README.md
--rw-------   0 cbartel    (503) staff       (20)      156 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/hpc/__init__.py
--rw-r--r--   0 cbartel    (503) staff       (20)    50350 2023-04-17 17:05:40.000000 pydmclab-1.0.0/pydmclab/hpc/analyze.py
--rw-------   0 cbartel    (503) staff       (20)    13255 2023-04-17 14:57:25.000000 pydmclab-1.0.0/pydmclab/hpc/launch.py
--rw-r--r--   0 cbartel    (503) staff       (20)    43385 2023-04-17 17:05:40.000000 pydmclab-1.0.0/pydmclab/hpc/submit.py
--rw-r--r--   0 cbartel    (503) staff       (20)    26676 2023-04-03 21:37:28.000000 pydmclab-1.0.0/pydmclab/hpc/vasp.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.460101 pydmclab-1.0.0/pydmclab/utils/
--rw-------   0 cbartel    (503) staff       (20)      271 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/utils/README.md
--rw-r--r--   0 cbartel    (503) staff       (20)      201 2023-04-03 21:26:17.000000 pydmclab-1.0.0/pydmclab/utils/__init__.py
--rw-r--r--   0 cbartel    (503) staff       (20)     4097 2023-04-03 21:38:03.000000 pydmclab-1.0.0/pydmclab/utils/handy.py
--rw-------   0 cbartel    (503) staff       (20)     1659 2023-04-03 21:38:07.000000 pydmclab-1.0.0/pydmclab/utils/plotting.py
-drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-04-29 17:44:37.366552 pydmclab-1.0.0/pydmclab.egg-info/
--rw-r--r--   0 cbartel    (503) staff       (20)      642 2023-04-29 17:44:37.000000 pydmclab-1.0.0/pydmclab.egg-info/PKG-INFO
--rw-r--r--   0 cbartel    (503) staff       (20)     2095 2023-04-29 17:44:37.000000 pydmclab-1.0.0/pydmclab.egg-info/SOURCES.txt
--rw-r--r--   0 cbartel    (503) staff       (20)        1 2023-04-29 17:44:37.000000 pydmclab-1.0.0/pydmclab.egg-info/dependency_links.txt
--rw-r--r--   0 cbartel    (503) staff       (20)       15 2023-04-29 17:44:37.000000 pydmclab-1.0.0/pydmclab.egg-info/requires.txt
--rw-r--r--   0 cbartel    (503) staff       (20)        9 2023-04-29 17:44:37.000000 pydmclab-1.0.0/pydmclab.egg-info/top_level.txt
--rw-r--r--   0 cbartel    (503) staff       (20)       38 2023-04-29 17:44:37.461324 pydmclab-1.0.0/setup.cfg
--rw-r--r--   0 cbartel    (503) staff       (20)     2539 2023-04-17 17:59:25.000000 pydmclab-1.0.0/setup.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-06-26 22:25:04.996508 pydmclab-1.0.1/
+-rw-------   0 cbartel    (503) staff       (20)     1071 2023-04-03 21:26:17.000000 pydmclab-1.0.1/LICENSE.txt
+-rw-------   0 cbartel    (503) staff       (20)      173 2023-04-03 21:38:56.000000 pydmclab-1.0.1/MANIFEST.in
+-rw-r--r--   0 cbartel    (503) staff       (20)      642 2023-06-26 22:25:04.996297 pydmclab-1.0.1/PKG-INFO
+-rw-------   0 cbartel    (503) staff       (20)      170 2023-04-05 14:50:32.000000 pydmclab-1.0.1/README.md
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-06-26 22:25:04.908798 pydmclab-1.0.1/pydmclab/
+-rw-------   0 cbartel    (503) staff       (20)      282 2023-05-24 19:08:50.000000 pydmclab-1.0.1/pydmclab/__init__.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-06-26 22:25:04.961631 pydmclab-1.0.1/pydmclab/core/
+-rw-------   0 cbartel    (503) staff       (20)      398 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/core/README.md
+-rw-------   0 cbartel    (503) staff       (20)      176 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/core/__init__.py
+-rw-------   0 cbartel    (503) staff       (20)     4582 2023-06-23 18:39:46.000000 pydmclab-1.0.1/pydmclab/core/comp.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    26408 2023-06-26 22:24:18.000000 pydmclab-1.0.1/pydmclab/core/energies.py
+-rw-------   0 cbartel    (503) staff       (20)    46413 2023-06-26 22:17:04.000000 pydmclab-1.0.1/pydmclab/core/hulls.py
+-rw-------   0 cbartel    (503) staff       (20)    12206 2023-06-23 20:18:22.000000 pydmclab-1.0.1/pydmclab/core/mag.py
+-rw-------   0 cbartel    (503) staff       (20)    13935 2023-06-23 20:55:51.000000 pydmclab-1.0.1/pydmclab/core/query.py
+-rw-r--r--   0 cbartel    (503) staff       (20)      470 2023-06-26 21:33:47.000000 pydmclab-1.0.1/pydmclab/core/reactions.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    17074 2023-06-23 18:55:25.000000 pydmclab-1.0.1/pydmclab/core/struc.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-06-26 22:25:04.969598 pydmclab-1.0.1/pydmclab/data/
+-rw-r--r--   0 cbartel    (503) staff       (20)     6148 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/data/.DS_Store
+-rw-------   0 cbartel    (503) staff       (20)      346 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/data/README.md
+-rw-------   0 cbartel    (503) staff       (20)      331 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/data/__init__.py
+-rw-------   0 cbartel    (503) staff       (20)      916 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/data/configs.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-06-26 22:25:04.981349 pydmclab-1.0.1/pydmclab/data/data/
+-rw-r--r--   0 cbartel    (503) staff       (20)    15963 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/data/data/221220_dmc-mus.json
+-rw-r--r--   0 cbartel    (503) staff       (20)     7720 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/data/data/230122_dmc-mus.json
+-rw-------   0 cbartel    (503) staff       (20)     4723 2023-06-14 19:59:43.000000 pydmclab-1.0.1/pydmclab/data/data/230614_dmc-mus.json
+-rw-r--r--   0 cbartel    (503) staff       (20)     1241 2023-04-17 14:02:36.000000 pydmclab-1.0.1/pydmclab/data/data/_batch_vasp_analysis_configs.yaml
+-rw-------   0 cbartel    (503) staff       (20)      437 2023-04-17 14:52:59.000000 pydmclab-1.0.1/pydmclab/data/data/_launch_configs.yaml
+-rw-------   0 cbartel    (503) staff       (20)     1954 2023-06-15 17:40:25.000000 pydmclab-1.0.1/pydmclab/data/data/_partition_configs.yaml
+-rw-r--r--   0 cbartel    (503) staff       (20)      598 2023-05-29 16:46:31.000000 pydmclab-1.0.1/pydmclab/data/data/_slurm_configs.yaml
+-rw-r--r--   0 cbartel    (503) staff       (20)     1450 2023-06-15 16:27:58.000000 pydmclab-1.0.1/pydmclab/data/data/_sub_configs.yaml
+-rw-------   0 cbartel    (503) staff       (20)     1561 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/data/data/_vasp_configs.yaml
+-rw-------   0 cbartel    (503) staff       (20)     1570 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/data/data/atomic_masses.json
+-rw-r--r--   0 cbartel    (503) staff       (20)     3140 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/data/data/bartel2019_npj_reference-energies.csv
+-rw-r--r--   0 cbartel    (503) staff       (20)     2596 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/data/data/colors.json
+-rw-------   0 cbartel    (503) staff       (20)    40326 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/data/data/elemental_gibbs_energies_T.json
+-rw-r--r--   0 cbartel    (503) staff       (20)     1302 2023-05-31 16:34:05.000000 pydmclab-1.0.1/pydmclab/data/data/gas_thermo_data_nist.json
+-rw-r--r--   0 cbartel    (503) staff       (20)     3788 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/data/data/mus_from_bartel2019_npj.json
+-rw-r--r--   0 cbartel    (503) staff       (20)     4722 2023-06-14 19:59:59.000000 pydmclab-1.0.1/pydmclab/data/data/mus_from_dmc_no_corrections.json
+-rw-------   0 cbartel    (503) staff       (20)     1710 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/data/data/mus_from_mp_no_corrections.json
+-rw-------   0 cbartel    (503) staff       (20)    43287 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/data/data/ssub.dat
+-rw-r--r--   0 cbartel    (503) staff       (20)    45994 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/data/data/ssub.json
+-rw-------   0 cbartel    (503) staff       (20)      246 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/data/features.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     2252 2023-04-03 21:35:30.000000 pydmclab-1.0.1/pydmclab/data/plotting_configs.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     4186 2023-06-14 20:00:50.000000 pydmclab-1.0.1/pydmclab/data/thermochem.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-06-26 22:25:04.985732 pydmclab-1.0.1/pydmclab/demos/
+-rw-------   0 cbartel    (503) staff       (20)     3762 2023-06-23 16:29:29.000000 pydmclab-1.0.1/pydmclab/demos/demo_comp.py
+-rw-------   0 cbartel    (503) staff       (20)     6435 2023-06-23 22:02:01.000000 pydmclab-1.0.1/pydmclab/demos/demo_energies.py
+-rw-------   0 cbartel    (503) staff       (20)    13928 2023-06-26 20:01:49.000000 pydmclab-1.0.1/pydmclab/demos/demo_hulls.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    10419 2023-06-20 17:29:25.000000 pydmclab-1.0.1/pydmclab/demos/demo_launcher_template.py
+-rw-------   0 cbartel    (503) staff       (20)      685 2023-06-23 20:18:25.000000 pydmclab-1.0.1/pydmclab/demos/demo_mag.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     1665 2023-06-20 18:30:53.000000 pydmclab-1.0.1/pydmclab/demos/demo_plot_dos.py
+-rw-------   0 cbartel    (503) staff       (20)     3167 2023-06-23 20:33:44.000000 pydmclab-1.0.1/pydmclab/demos/demo_query.py
+-rw-------   0 cbartel    (503) staff       (20)     3848 2023-06-23 18:34:28.000000 pydmclab-1.0.1/pydmclab/demos/demo_struc.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-06-26 22:25:04.988894 pydmclab-1.0.1/pydmclab/dev/
+-rw-r--r--   0 cbartel    (503) staff       (20)      153 2023-04-19 19:26:44.000000 pydmclab-1.0.1/pydmclab/dev/Untitled-2.py
+-rw-------   0 cbartel    (503) staff       (20)       48 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/dev/__init__.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     7018 2023-04-29 17:42:52.000000 pydmclab-1.0.1/pydmclab/dev/echem.py
+-rw-------   0 cbartel    (503) staff       (20)     3091 2023-06-26 21:35:16.000000 pydmclab-1.0.1/pydmclab/dev/entries.py
+-rw-------   0 cbartel    (503) staff       (20)      170 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/dev/grand.py
+-rw-r--r--   0 cbartel    (503) staff       (20)      966 2023-06-26 20:47:07.000000 pydmclab-1.0.1/pydmclab/dev/mixing_pmg.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     2483 2023-06-23 20:34:26.000000 pydmclab-1.0.1/pydmclab/dev/query_new_mp_api.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-06-26 22:25:04.991805 pydmclab-1.0.1/pydmclab/hpc/
+-rw-------   0 cbartel    (503) staff       (20)      707 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/hpc/README.md
+-rw-------   0 cbartel    (503) staff       (20)      156 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/hpc/__init__.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    46832 2023-05-31 17:45:11.000000 pydmclab-1.0.1/pydmclab/hpc/analyze.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    45124 2023-06-23 20:51:57.000000 pydmclab-1.0.1/pydmclab/hpc/helpers.py
+-rw-------   0 cbartel    (503) staff       (20)    11678 2023-05-29 19:33:08.000000 pydmclab-1.0.1/pydmclab/hpc/launch.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    38168 2023-06-15 18:06:04.000000 pydmclab-1.0.1/pydmclab/hpc/submit.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    26870 2023-05-26 17:13:12.000000 pydmclab-1.0.1/pydmclab/hpc/vasp.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-06-26 22:25:04.993639 pydmclab-1.0.1/pydmclab/plotting/
+-rw-r--r--   0 cbartel    (503) staff       (20)        7 2023-06-20 19:00:10.000000 pydmclab-1.0.1/pydmclab/plotting/__init__.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    13934 2023-06-23 15:24:04.000000 pydmclab-1.0.1/pydmclab/plotting/dos.py
+-rw-r--r--   0 cbartel    (503) staff       (20)    21966 2023-06-23 15:24:04.000000 pydmclab-1.0.1/pydmclab/plotting/pd.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     2430 2023-06-20 18:56:12.000000 pydmclab-1.0.1/pydmclab/plotting/utils.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-06-26 22:25:04.995762 pydmclab-1.0.1/pydmclab/utils/
+-rw-------   0 cbartel    (503) staff       (20)      271 2023-04-03 21:26:17.000000 pydmclab-1.0.1/pydmclab/utils/README.md
+-rw-r--r--   0 cbartel    (503) staff       (20)      205 2023-05-29 20:02:40.000000 pydmclab-1.0.1/pydmclab/utils/__init__.py
+-rw-r--r--   0 cbartel    (503) staff       (20)     3421 2023-05-29 19:36:18.000000 pydmclab-1.0.1/pydmclab/utils/handy.py
+drwxr-xr-x   0 cbartel    (503) staff       (20)        0 2023-06-26 22:25:04.923051 pydmclab-1.0.1/pydmclab.egg-info/
+-rw-r--r--   0 cbartel    (503) staff       (20)      642 2023-06-26 22:25:04.000000 pydmclab-1.0.1/pydmclab.egg-info/PKG-INFO
+-rw-r--r--   0 cbartel    (503) staff       (20)     2193 2023-06-26 22:25:04.000000 pydmclab-1.0.1/pydmclab.egg-info/SOURCES.txt
+-rw-r--r--   0 cbartel    (503) staff       (20)        1 2023-06-26 22:25:04.000000 pydmclab-1.0.1/pydmclab.egg-info/dependency_links.txt
+-rw-r--r--   0 cbartel    (503) staff       (20)       15 2023-06-26 22:25:04.000000 pydmclab-1.0.1/pydmclab.egg-info/requires.txt
+-rw-r--r--   0 cbartel    (503) staff       (20)        9 2023-06-26 22:25:04.000000 pydmclab-1.0.1/pydmclab.egg-info/top_level.txt
+-rw-r--r--   0 cbartel    (503) staff       (20)       38 2023-06-26 22:25:04.996565 pydmclab-1.0.1/setup.cfg
+-rw-r--r--   0 cbartel    (503) staff       (20)     2539 2023-06-26 22:24:53.000000 pydmclab-1.0.1/setup.py
```

### Comparing `pydmclab-1.0.0/LICENSE.txt` & `pydmclab-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.0/PKG-INFO` & `pydmclab-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydmclab
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package to facilitate DFT calculations and analysis
 Home-page: https://github.umn.edu/bartel-group/pydmclab
 Author: Chris Bartel
 Author-email: cbartel@umn.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pydmclab-1.0.0/pydmclab/core/comp.py` & `pydmclab-1.0.1/pydmclab/core/comp.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,141 +1,173 @@
 from pymatgen.core.composition import Composition
 import numpy as np
 
 
 class CompTools(object):
-    
     def __init__(self, formula):
         """
-        Args: 
+        Args:
             formula (str) - chemical formula
+
+        Returns:
+            formula
         """
         self.formula = formula
-    
+
     @property
     def clean(self):
         """
         Returns:
             formula (str) that has been:
                 - sorted by elements
                 - parentheses removed
                 - fractions --> integers
-                
+
         In general, we want to use this for maximum consistency
         """
+        # reduce
         formula = Composition(self.formula).reduced_formula
+
+        # alphabetize
         formula = Composition(formula).alphabetical_formula
-        if '.' in formula:
+
+        # expand if it has decimals
+        if "." in formula:
             formula = Composition(formula).get_integer_formula_and_factor()[0]
+
+        # alphabetize
         formula = Composition(formula).alphabetical_formula
+
+        # remove parentheses
         formula = Composition(formula).to_pretty_string()
 
-        if (len(formula) <= 3) and (formula[-1] == '2'):
-            formula = formula.replace('2', '1')
+        # remove "2" for diatomic elements
+        if (len(formula) <= 3) and (formula[-1] == "2"):
+            formula = formula.replace("2", "1")
         return formula
-    
+
     @property
     def pretty(self):
         """
         Returns:
             formula (str) that is visually pleasing (chemically meaningful)
                 - note: reduces the formula
         """
         return Composition(self.formula).reduced_formula
-    
+
     @property
     def amts(self):
         """
         Returns:
             dictionary of elements (str) and their amounts (float)
                 - note: starts with "clean" formula
+                {el (str) : amt (float)}
+
+            CompTools('Al4O6').amts = {'Al' : 2, 'O' : 3}
         """
-        
+
         return Composition(self.clean).get_el_amt_dict()
-    
+
     def mol_frac(self, el):
         """
         Returns:
             the molar fraction (float) of an element (str)
                 - note: starts with "clean" formula
+
+            CompTools('Al4O6').mol_frac('Al') = 0.4
         """
         return Composition(self.clean).get_atomic_fraction(el)
-    
+
     def stoich(self, el):
         """
         Returns:
             the stoichiometry of an element (int)
                 - note: starts with "clean" formula
             e.g., if CompTools(c).clean == 'Al2Mg1O4', then CompTools(c).stoich('O') = 4
-        """ 
+        """
         stoich = self.mol_frac(el) * self.n_atoms
         stoich = np.round(stoich, 0)
         return int(stoich)
-    
+
     @property
     def chemsys(self):
         """
         Returns:
             chemical system (str) of the formula
                 - sorted
                 - elements (str) joined by "-"
+
+            CompTools('Al4O6').chemsys = 'Al-O'
         """
         return Composition(self.clean).chemical_system
-    
+
     @property
     def els(self):
         """
         Returns:
             list of elements (str) in the formula
                 - sorted
+
+            CompTools('Al4O6').els = ['Al', 'O']
         """
-        return list(sorted(self.chemsys.split('-')))
-    
+        return list(sorted(self.chemsys.split("-")))
+
     @property
     def n_els(self):
         """
         Returns:
             number of elements (int) in the formula
+
+            CompTools('Al4O6').n_els = 2
         """
         return len(self.els)
-    
+
     @property
     def n_atoms(self):
         """
         Returns:
             number of atoms (int) in the formula
                 - note: starts with "clean" formula
+
+            CompTools('Al4O6').n_atoms = 5
         """
         return np.sum(list(self.amts.values()))
-    
-    def label_for_plot(self, el_order=None, reduce=True):
+
+    def label_for_plot(self, el_order=None):
         """
+        @NOTE:
+            this is redundant w/ pydmclab.plotting.utils.get_label ?
+
+        @FEATURE:
+            - would be great if this worked for decimal formulas
+
+        Args:
+            el_order (list) - order of elements (str) for plotting
+
         Returns:
             label (str) for plotting (includes $ for subscripts)
         """
-        #formula = self.clean if reduce else self.formula
+        # formula = self.clean if reduce else self.formula
         if not el_order:
             el_order = self.els
         amts = self.amts
-        label = r'$'
+        label = r"$"
         for el in el_order:
             if el in amts:
                 n_el = amts[el]
                 if n_el == 1:
                     label += el
                 elif n_el > 1:
                     if int(n_el) - n_el == 0:
-                        label += el + '_{%s}' % str(int(n_el))
+                        label += el + "_{%s}" % str(int(n_el))
                     else:
-                        label += el + '_{%.1f}' % float(n_el)
-        label += '$'
+                        label += el + "_{%.1f}" % float(n_el)
+        label += "$"
         return label
-        
-    
-    
-    
+
+
 def main():
-    return 
-    
+    return
+
 
-if __name__ == '__main__':
-    o = main()
+if __name__ == "__main__":
+    main()
```

### Comparing `pydmclab-1.0.0/pydmclab/core/hulls.py` & `pydmclab-1.0.1/pydmclab/core/hulls.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,25 @@
     mus_at_0K,
     mus_at_T,
     mp2020_compatibility_dmus,
     mus_from_mp_no_corrections,
 )
 from pydmclab.data.features import atomic_masses
 
+from pymatgen.analysis.phase_diagram import PDEntry, PhaseDiagram, CompoundPhaseDiagram
+from pymatgen.core.composition import Composition
+
+from pydmclab.core.energies import ReactionEnergy
+
 import os
 import numpy as np
 from scipy.spatial import ConvexHull
 from scipy.optimize import minimize
 import multiprocessing as multip
-import math
-from itertools import combinations
+
 
 HERE = os.path.dirname(os.path.abspath(__file__))
 
 """
 Contents:
 
     1) Classes allowing you to compute decomposition energies using the convex hull analysis
@@ -643,15 +647,15 @@
         if not data_dir:
             self.data_dir = os.getcwd()
         else:
             self.data_dir = data_dir
         self.fresh_restart = fresh_restart
 
         self.compound_to_energy = {
-            k: compound_to_energy[k][formation_energy_key]
+            CompTools(k).clean: compound_to_energy[k][formation_energy_key]
             for k in compound_to_energy
             if len(CompTools(k).els) > 1
         }
 
     @property
     def compounds(self):
         """
@@ -890,17 +894,15 @@
 
 
     """
 
     def __init__(
         self,
         input_energies,
-        varying_element,
         end_members,
-        shared_element_basis,
         energy_key="E_per_at",
     ):
         """
 
         Args:
             input_energies (dict):
                 - the energies you collected from DFT calculations
@@ -942,218 +944,69 @@
             CompTools(k).clean: {"E": input_energies[k][energy_key]}
             for k in input_energies
         }
 
         # sanitize the end_members
         self.end_members = [CompTools(c).clean for c in end_members]
 
-        self.varying_element = varying_element
-        self.shared_element_basis = shared_element_basis
         self.input_energies = input_energies
 
     @property
-    def shared_element_amt_basis(self):
-        """
-
-        using the shared_element_basis, determine how many of that element they're should be
-            - usually we specify the end-members to have the same number of this element already
-            - this is in case we don't do that for some reason.
-                - e.g., if our end-members are ['Li2FeP2S6', 'Li3Fe2P4S12']
-                    - and our shared_element_basis is 'Fe'
-                    - we need to decide whether a "formula unit" has 1 Fe or 2 Fe
-                    - this code will choose the larger of the two
-
-        Returns:
-            the amount (int) of the shared element basis
-        """
-        end_members = self.end_members
-        shared_element_basis = self.shared_element_basis
-
-        # get the amt of the shared element in the first end member
-        amt_1 = CompTools(end_members[0]).stoich(shared_element_basis)
-
-        # get the amt of the shared element in the second end member
-        amt_2 = CompTools(end_members[1]).stoich(shared_element_basis)
-
-        # choose the larger one
-        if amt_2 > amt_1:
-            return amt_2
-        else:
-            return amt_1
-
-    @property
     def relevant_compounds(self):
-        """
-
-        some of the formulas in input_energies might not be relevant to the specified hull
-            - e.g., if I had mixed phases pertaining to Li2MP2S6 (M = Fe, Mn, Co, ...) in one dictionary,
-                - this code will use the end-members to ignore the irrelevant compounds
-
-        Returns:
-            list of unique compounds (str) that are relevant to the mixing hull
-        """
-        # get all my compounds
-        compounds = list(self.input_energies.keys())
-
-        endmembers = self.end_members
-        varying_element = self.varying_element
-
-        # get all the elements that are in the end members
-        elements_in_relevant_compounds = [CompTools(e).els for e in endmembers]
-
-        # flatten the list and make it unique
-        elements_in_relevant_compounds = list(
-            set(
-                [item for sublist in elements_in_relevant_compounds for item in sublist]
-            )
-        )
-
-        # figure out what elements must be present in a relevant compound
-        elements_that_must_be_present = [
-            el for el in elements_in_relevant_compounds if el != varying_element
+        input_energies = self.input_energies
+        pd_entries = [
+            PDEntry(Composition(c), input_energies[c]["E"]) for c in input_energies
         ]
-
-        # determine the relevant compounds
-        relevant_compounds = []
-        for c in compounds:
-            # end members must be relevant
-            if c in endmembers:
-                relevant_compounds.append(c)
-                continue
-
-            els = CompTools(c).els
-
-            # make sure the compound we're checking doesn't have elements that are not in the endmembers
-            has_other_els = False
-            for el in els:
-                if el not in elements_in_relevant_compounds:
-                    has_other_els = True
-            if has_other_els:
-                continue
-
-            # make sure the compound we're checking has all the elements that are in the endmembers (except perhaps the varying element)
-            counter = 0
-            for el in elements_that_must_be_present:
-                if el in els:
-                    counter += 1
-            if counter == len(elements_that_must_be_present):
-                relevant_compounds.append(c)
-            elif counter == len(elements_in_relevant_compounds) - 1:
-                if varying_element in els:
-                    relevant_compounds.append(c)
-
-        return relevant_compounds
+        end_members = self.end_members
+        cpd = CompoundPhaseDiagram(
+            pd_entries, [Composition(c) for c in end_members], False
+        )
+        entries = cpd.entries
+        return [CompTools(e.name).clean for e in entries]
 
     @property
-    def energies_with_fractional_composition(self):
-        """
-        re-configure input_energies to make it amenable to mixing calculations
-            - also make it include only relevant compounds
-
-        Returns:
-
-            {formula (str) :
-                {'E' : total energy per atom (float, eV/atom),
-                 'factor' : factor to multiply by to convert the maximally reduced formula unit into the appropriate basis formula unit (float),
-                 'n_varying' : number of varying element atoms in the basis formula unit (float),
-                 'n_atoms_basis' : number of atoms in the basis formula unit (float)}
-        """
-        shared_element_amt_basis = self.shared_element_amt_basis
-        shared_element_basis = self.shared_element_basis
-        varying_element = self.varying_element
+    def reactions(self):
+        targets = self.relevant_compounds
+        reactants = self.end_members
         input_energies = self.input_energies
-        relevant_compounds = self.relevant_compounds
-
-        # use only the relevant compounds
-        input_energies = {c: input_energies[c] for c in relevant_compounds}
-
-        for c in input_energies:
-            # figure out how to convert the reduced f.u. into the basis f.u.
-            amt_of_shared_el = CompTools(c).stoich(shared_element_basis)
-            factor = shared_element_amt_basis / amt_of_shared_el
-            input_energies[c]["factor"] = factor
-
-            # convert the number of the varying element into the basis f.u.
-            n_varying = CompTools(c).stoich(varying_element) * factor
-
-            # count the number of atoms in the basis f.u.
-            n_atoms_basis = CompTools(c).n_atoms * factor
-
-            input_energies[c]["factor"] = factor
-            input_energies[c]["n_varying"] = n_varying
-            input_energies[c]["n_atoms_basis"] = n_atoms_basis
-        return input_energies
+        reactions = {
+            t: ReactionEnergy(input_energies, reactants, [t], energy_key="E")
+            for t in targets
+        }
+        return reactions
 
     @property
     def mixing_energies(self):
-        """
-        compute the mixing energies
-
-        Returns:
-
-            {formula (str) :
-                {'E' : total energy per atom (float, eV/atom),
-                 'factor' : factor to multiply by to convert the maximally reduced formula unit into the appropriate basis formula unit (float),
-                 'n_varying' : number of varying element atoms in the basis formula unit (float),
-                 'n_atoms_basis' : number of atoms in the basis formula unit (float),
-                 'E_mix' : mixing energy (float, eV/atom),
-                 'x' : fraction of the varying element (float),
-                 'zero' : which end member has x == 0 (str, formula)}
-        """
-        input_energies = self.energies_with_fractional_composition
-        end_members = self.end_members
-
-        # get the energies, number of varying element, and basis for both end members
-        E_left = input_energies[end_members[0]]["E"]
-        E_right = input_energies[end_members[1]]["E"]
-        n_left = input_energies[end_members[0]]["n_varying"]
-        n_right = input_energies[end_members[1]]["n_varying"]
-        basis_left = input_energies[end_members[0]]["n_atoms_basis"]
-        basis_right = input_energies[end_members[1]]["n_atoms_basis"]
-
-        for c in input_energies:
-            E = input_energies[c]["E"]
-            n = input_energies[c]["n_varying"]
-            basis = input_energies[c]["n_atoms_basis"]
-
-            # determine which end member is "zero" (the left side of a traditional mixing hull)
-            # this affects which end member gets (1-x) and which gets (x) as a coef in the mixing energy calculation
-            # this also allows us to compute the fractional amount of the varying element (from n_varying --> x)
-            if n_left != 0:
-                x = n / n_left
-                zero = "right"
-            elif n_right != 0:
-                x = n / n_right
-                zero = "left"
-
-            # compute the mixing energy per basis f.u.
-            if zero == "right":
-                E_mix = E * basis - (
-                    x * E_left * basis_left + (1 - x) * E_right * basis_right
-                )
-            elif zero == "left":
-                E_mix = E * basis - (
-                    (1 - x) * E_left * basis_left + x * E_right * basis_right
-                )
-
-            # convert the mixing energy to eV/atom
-            E_mix = E_mix / basis
-
-            input_energies[c]["E_mix"] = E_mix
-            input_energies[c]["x"] = x
-
-            if zero == "left":
-                zero_compound = end_members[0]
-
-            elif zero == "right":
-                zero_compound = end_members[1]
-
-            input_energies[c]["zero"] = zero_compound
+        energies = {}
+        reactions = self.reactions
+        input_energies = self.input_energies
+        left, right = self.end_members
+        for target in reactions:
+            if target in [left, right]:
+                E_mix = 0
+                x = 0 if target == left else 1
+                rxn = None
+                E = input_energies[target]["E"]
+            else:
+                coefs = reactions[target].coefs
+                dE_rxn = reactions[target].dE_rxn
+                E_mix = dE_rxn / CompTools(target).n_atoms / coefs[target]
+                E = input_energies[target]["E"]
+                rxn = reactions[target].rxn_string
+                n_left = coefs[left] if left in coefs else 0
+                n_right = coefs[right] if right in coefs else 0
+                x = n_right / (n_left + n_right)
+            energies[target] = {
+                "x": x,
+                "E_mix": E_mix,
+                "E": E,
+                "mixing_rxn": rxn,
+            }
 
-        return input_energies
+        return energies
 
     @property
     def sorted_compounds(self):
         """
         Returns:
             alphabetized list of relevant compounds (str) in the mixing hull
         """
@@ -1269,21 +1122,24 @@
                     2) assuming that there are no other stable compounds in the chemical space that are orthogonal to the mixing axis
                         - e.g., we might be mixing RuO2 and IrO2, but RuIrO5 would not appear on this hull because it is orthogonal
 
         """
         mixing_energies = self.mixing_energies
         hull_vertices = self.hull_vertices
         compounds = self.sorted_compounds
+        end_members = self.end_members
 
         # compounds are stable if they have negative mixing energy and are on the hull
-        return [
+        vertices = [
             compounds[i]
             for i in hull_vertices
             if mixing_energies[compounds[i]]["E_mix"] <= 0
         ]
+        vertices += end_members
+        return sorted(list(set(vertices)))
 
     @property
     def unstable_compounds(self):
         """
         Returns:
             list of compounds that do not correspond with vertices (str)
                 - these are "above" the mixing hull
@@ -1298,25 +1154,38 @@
         """
 
         this is the only method that really needs to be called by the user
 
         Returns:
 
             {formula (str) :
-                {'E' : total energy per atom (float, eV/atom),
-                 'factor' : factor to multiply by to convert the maximally reduced formula unit into the appropriate basis formula unit (float),
-                 'n_varying' : number of varying element atoms in the basis formula unit (float),
-                 'n_atoms_basis' : number of atoms in the basis formula unit (float),
+                {'E' : total (or formation) energy per atom (float, eV/atom),
                  'E_mix' : mixing energy (float, eV/atom),
-                 'x' : fraction of the varying element (float),
-                 'zero' : which end member has x == 0 (str, formula),
-                 'stability' : True if the compound is on the mixing hull else False}
+                 'x' : fraction of the right end member (float),
+                 'stability' : True if the compound is on the mixing hull else False,
+                 'mixing_rxn' : mixing reaction (molar basis)}
         """
         stable_compounds = self.stable_compounds
         unstable_compounds = self.unstable_compounds
         mixing_energies = self.mixing_energies
         for c in stable_compounds:
             mixing_energies[c]["stability"] = True
         for c in unstable_compounds:
             mixing_energies[c]["stability"] = False
 
         return mixing_energies
+
+
+def main():
+    gs = read_json("../demos/output/hulls/data/query_Li-Mn-Fe-O.json")
+    # return gs
+    mix = MixingHull(
+        input_energies=gs,
+        end_members=["LiMnO2", "MnO2"],
+        energy_key="Ef_mp",
+    )
+
+    return mix, mix.results
+
+
+if __name__ == "__main__":
+    mix, out = main()
```

### Comparing `pydmclab-1.0.0/pydmclab/core/mag.py` & `pydmclab-1.0.1/pydmclab/core/mag.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,57 +4,64 @@
 from pymatgen.core.structure import Structure
 from pymatgen.transformations.site_transformations import (
     ReplaceSiteSpeciesTransformation,
 )
 from pymatgen.analysis.structure_matcher import StructureMatcher
 
 
-"""
-Using enumlib:
-    - install enumlib from https://github.com/msg-byu/enumlib
-    - for MAC
-        - install xcode ($ xcode-select --install)
-        - install gfortran (https://github.com/fxcoudert/gfortran-for-macOS/releases)
-    - follow enumlib instructions
-    - mkdir */enumlib.bin
-    - move */enumlib/src/enum.x and */enumlib/aux_src/makeStr.py to */enumlib/bin
-    - add #! /usr/bin/env python to top of */enumlib/bin/makeStr.py
-    - add */enumlib/bin to PATH (PATH=$PATH:*/enumlib/bin)
-"""
-
-
 class MagTools(object):
+    """
+    For generating magnetic orderings for structures
+    """
+
     def __init__(
         self,
         structure,
         max_afm_combos=100,
         afm_spins=(-5, 5),
         fm_spins=(0.6, 5),
         randomize_afm=True,
         treat_as_nm=[],
     ):
         """
         Args:
-            structure (Structure): pymatgen Structure object
-            max_afm_combos (int): maximum number of AFM spin configurations to generate
-            afm_spins (tuple): low and high spin for AFM initialization
-            fm_spins (tuple): zero and non-zero spin for FM initialization
-            randomize_afm (bool): randomize AFM spin configurations
-                - randomization occurs in two different steps
-                    - when AFM combinations are enumerated,
-                        if the number of combinations is greater than max_afm_combos,
-                        then we randomly select max_afm_combos combinations
-                    - when the unique AFM structures are generated,
-                        we randomly order them to avoid having the same "kinds" of AFM orderings always appearing first
-                    - random seeds are being used so both operations should be deterministic
-            treat_as_nm (list): list of elements to treat as non-magnetic
-                - e.g., if you want to only explore various initial configurations for other element(s)
+            structure (Structure):
+                pymatgen Structure object
+
+            max_afm_combos (int):
+                maximum number of AFM spin configurations to generate
+                    this is useful when there are a tremendous number of plausible AFM orderings (e.g., for structures w/ many magnetic elements)
+                    100 is usually reasonable
+
+            afm_spins (tuple):
+                low and high spin for AFM initialization
+                    -5 and 5 are usually safe initializations
+
+            fm_spins (tuple):
+                zero and non-zero spin for FM initialization
+                    0.6 and 5 are usually safe initializations
+
+            randomize_afm (bool):
+                randomize AFM spin configurations
+                    randomization occurs in two different steps
+                        1) when AFM combinations are enumerated,
+                            if the number of combinations is greater than max_afm_combos,
+                            then we randomly select max_afm_combos combinations
+                        2) when the unique AFM structures are generated,
+                            we randomly order them to avoid having the same "kinds" of AFM orderings always appearing first
+                    random seeds are being used so both operations should be deterministic
+
+            treat_as_nm (list):
+                list of elements to treat as non-magnetic
+                    e.g., if you want to only explore various initial configurations for other element(s)
         """
         if isinstance(structure, dict):
             structure = Structure.from_dict(structure)
+
+        # purge oxidation states (makes life easier later)
         structure.remove_oxidation_states()
         self.structure = structure
         self.max_afm_combos = max_afm_combos
         self.fm_spins = fm_spins
         self.afm_spins = afm_spins
         self.randomize_afm = randomize_afm
         self.treat_as_nm = treat_as_nm
@@ -62,14 +69,18 @@
     @property
     def magnetic_ions(self):
         """
         Aggregated from MP + matminer (**propably a better list to use somewhere**)
 
         from_MP = https://github.com/materialsproject/pymatgen/blob/master/pymatgen/analysis/magnetism/default_magmoms.yaml
         from_matminer = https://github.com/hackingmaterials/matminer/blob/main/matminer/featurizers/composition/element.py
+
+        Returns:
+            list of elements (str) that could be magnetic
+                note removes those you've said to "treat_as_nm"
         """
         from_matminer = [
             "Ti",
             "V",
             "Cr",
             "Mn",
             "Fe",
@@ -145,15 +156,15 @@
         True if any magnetic ions are in structure else False
         """
         return True if len(self.magnetic_ions_in_struc) > 0 else False
 
     @property
     def could_be_afm(self):
         """
-        True if there are at least two magnetic sites in structure
+        True if there are at least two magnetic sites in structure and the number of magnetic sites is even
         """
         if not self.could_be_magnetic:
             return False
 
         magnetic_ions = self.magnetic_ions_in_struc
         magnetic_sites = 0
         structure = self.structure
@@ -164,15 +175,15 @@
         if magnetic_sites > 1:
             if magnetic_sites % 2 == 0:
                 return True
 
     @property
     def get_nonmagnetic_structure(self):
         """
-        Returns nonmagnetic Structure with magmom of zeros
+        Returns nonmagnetic Structure with magmoms of zeros
         """
         s = self.structure
         magmom = [0 for i in range(len(s))]
         s_tmp = s.copy()
         s_tmp.add_site_property("magmom", magmom)
         return s_tmp
 
@@ -184,15 +195,14 @@
             - magnetic ions are given spin = spins[1] (default: 5)
         """
         spins = self.fm_spins
         magnetic_ions_in_struc = self.magnetic_ions_in_struc
         if len(magnetic_ions_in_struc) == 0:
             return None
         s = self.structure
-        # magnetic_sites = [i for i in range(len(s)) if s[i].species_string in magnetic_ions_in_struc]
         magmom = [
             spins[0] if s[i].species_string not in magnetic_ions_in_struc else spins[1]
             for i in range(len(s))
         ]
         s_tmp = s.copy()
         s_tmp.add_site_property("magmom", magmom)
         return s_tmp
@@ -200,15 +210,15 @@
     @property
     def get_antiferromagnetic_structures(self):
         """
         This is a chaotic way to get antiferromagnetic configurations
             - but it doesn't require enumlib interaction with pymatgen
             - it seems reasonably efficient, might break down for large/complex structures
             - note 1: it has no idea which configurations are "most likely" to be low energy
-            - note 2: it may require execution on MSI compute nodes
+            - note 2: it may require execution on compute nodes
 
         Basic workflow:
             - start from the NM structure
             - for all sites containing ions in magnetic_ions
                 - generate all possible combinations of 0 (spin down) or 1 (spin up) for each site
                     - if I had four sites w/ mag ions this might be: [(0,0,0,1), (0,0,1,1), ...]
                 - retain only the combinations that have average = 0.5 (ie half spin down, half spin up)
@@ -323,13 +333,12 @@
             for i in range(len(afm_strucs)):
                 magmoms[i] = afm_strucs[i].site_properties["magmom"]
 
         return magmoms
 
 
 def main():
-
     return
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pydmclab-1.0.0/pydmclab/core/query.py` & `pydmclab-1.0.1/pydmclab/core/query.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,109 +4,39 @@
 from pymatgen.ext.matproj import MPRester
 
 # from mp_api.client import MPRester as new_MPRester
 
 import itertools
 import numpy as np
 
-
-class NewMPQuery(object):
-    # Chris B key = E4p0iuBO8rX7XTaPe5c4O8WO5YpikMB1
-
-    """
-    Trying to transition to new API but running into many issues
-    """
-
-    def __init__(self, api_key):
-        """
-        Args:
-            api_key (str) - Materials Project API key
-
-        Returns:
-            self.mpr (MPRester) - Materials Project REST interface
-        """
-
-        api_key = api_key if api_key else "YOUR_API_KEY"
-
-        self.api_key = api_key
-        self.mpr = new_MPRester(api_key)
-
-    @property
-    def available_fields(self):
-        return self.mpr.summary.available_fields
-
-    @property
-    def typical_fields(self):
-        return [
-            "formula_pretty",
-            "volume",
-            "nsites",
-            "material_id",
-            "energy_per_atom",
-            "uncorrected_energy_per_atom",
-            "formation_energy_per_atom",
-            "energy_above_hull",
-            "equilibrium_reaction_energy_per_atom",
-            "decomposes_to",
-            "band_gap",
-            "is_magnetic",
-            "symmetry",
-        ]
-
-    def get_data_for_comp(self, comp):
-
-        all_chemsyses = None
-        all_formulas = None
-        if isinstance(comp, str):
-            if "-" in comp:
-                chemsys = comp
-                all_chemsyses = []
-                elements = chemsys.split("-")
-                for i in range(len(elements)):
-                    for els in itertools.combinations(elements, i + 1):
-                        all_chemsyses.append("-".join(sorted(els)))
-            else:
-                all_formulas = [CompTools(comp).clean]
-        elif isinstance(comp, list):
-            if "-" in comp[0]:
-                all_chemsyses = []
-                for chemsys in comp:
-                    elements = chemsys.split("-")
-                    for i in range(len(elements)):
-                        for els in itertools.combinations(elements, i + 1):
-                            all_chemsyses.append("-".join(sorted(els)))
-                all_chemsyses = sorted(list(set(all_chemsyses)))
-            else:
-                all_formulas = [CompTools(c).pretty for c in comp]
-        if all_formulas:
-            from_mp = self.mpr.summary.search(
-                formula_pretty=all_formulas, fields=self.typical_fields
-            )
-        elif all_chemsyses:
-            from_mp = self.mpr.summary.search(
-                chemsys=all_chemsyses, fields=self.typical_fields
-            )
-
-        return from_mp
+""" 
+Purpose:
+    - query the Materials Project database for data
+    
+Typical use:
+    MPQuery.get_data_for_comp(...)
+"""
 
 
 class MPQuery(object):
     # Chris B API KEY =
     """
     class to assist with downloading data from Materials Project
 
     """
 
     def __init__(self, api_key=None):
         """
         Args:
-            api_key (str) - Materials Project API key
+            api_key (str)
+                Materials Project API key
 
         Returns:
-            self.mpr (MPRester) - Materials Project REST interface
+            self.mpr (MPRester)
+                Materials Project REST interface
         """
 
         api_key = api_key if api_key else "YOUR_API_KEY"
 
         self.api_key = api_key
         self.mpr = MPRester(api_key)
 
@@ -258,122 +188,134 @@
 
             max_strucs_per_cmpd (int)
                 if not None, only retain the lowest energy structures for each composition until you reach max_strucs_per_cmpd
 
         Returns:
             {mpid : {DATA}}
         """
+        # convert MP keys into shorter keys
         key_map = self.long_to_short_keys
         if properties == "all":
+            # use all supported properties
             properties = self.supported_properties
         if properties == None:
+            # use our typical properties
             properties = self.typical_properties
         else:
+            # make sure properties are supported
             for prop in properties:
                 if prop not in self.supported_properties:
                     raise ValueError("Property %s is not supported!" % prop)
 
         if criteria == None:
+            # make criteria an empty dictionary
             criteria = {}
 
         if isinstance(comp, str):
+            # just working with one compound or chemical system
             if "-" in comp:
+                # must be a chemical system
                 chemsys = comp
+                # need to get all chemical (sub)systems
                 all_chemsyses = []
                 elements = chemsys.split("-")
                 for i in range(len(elements)):
                     for els in itertools.combinations(elements, i + 1):
                         all_chemsyses.append("-".join(sorted(els)))
-
+                # add these chemical spaces to our criteria
                 criteria["chemsys"] = {"$in": all_chemsyses}
             else:
+                # just working with one formula
                 formula = comp
+                # query only for that formula
                 criteria["pretty_formula"] = {"$in": [CompTools(formula).pretty]}
 
         elif isinstance(comp, list):
+            # now we have a list of compounds or chemical systems (should be one or the other)
             if "-" in comp[0]:
+                # must be a list of chemical systems, let's get em all
                 all_chemsyses = []
                 for chemsys in comp:
                     elements = chemsys.split("-")
                     for i in range(len(elements)):
                         for els in itertools.combinations(elements, i + 1):
                             all_chemsyses.append("-".join(sorted(els)))
                 all_chemsyses = sorted(list(set(all_chemsyses)))
                 criteria["chemsys"] = {"$in": all_chemsyses}
             else:
+                # get the entire list of formulas
                 all_formulas = [CompTools(c).pretty for c in comp]
                 criteria["pretty_formula"] = {"$in": all_formulas}
 
-        list_from_mp = self.mpr.query(criteria, properties)
-        extra_keys = [k for k in list_from_mp[0] if k not in key_map]
+        # initalize the rester and query
+        mpr = self.mpr
+        list_from_mp = mpr.query(criteria, properties)
+        if not list_from_mp:
+            raise ValueError("No entries found for criteria %s" % criteria)
+
+        # shorten the keys we can shorten
         cleaned_list_from_mp = [
             {key_map[old_key]: entry[old_key] for old_key in key_map}
             for entry in list_from_mp
         ]
+
+        # grab the keys that won't get mapped to short keys
+        extra_keys = [k for k in list_from_mp[0] if k not in key_map]
+
+        # assemble all the chunked queries into one query
         query = []
         for i in range(len(list_from_mp)):
             query.append(
                 {
                     **cleaned_list_from_mp[i],
                     **{k: list_from_mp[i][k] for k in extra_keys},
                     **{"cmpd": CompTools(list_from_mp[i]["pretty_formula"]).clean},
                 }
             )
 
         if only_gs:
-
+            # grab only the lowest energy entry for each composition
             gs = {}
             for entry in query:
                 cmpd = CompTools(entry["pretty_formula"]).clean
                 if cmpd not in gs:
                     gs[cmpd] = entry
                 else:
                     energy_key = "E_mp" if len(CompTools(cmpd).els) == 1 else "Ef_mp"
                     Ef_stored = gs[cmpd][energy_key]
                     Ef_check = entry[energy_key]
                     if Ef_check < Ef_stored:
                         gs[cmpd] = entry
             query = [gs[k] for k in gs]
-            query = {entry["mpid"]: entry for entry in query}
 
-        else:
-            query = {entry["mpid"]: entry for entry in query}
+        # orient our query into a dictionary keyed by MP ID
+        query = {entry["mpid"]: entry for entry in query}
 
         if include_structure:
-            for entry in query:
-                mpid = query[entry]["mpid"]
+            for mpid in query:
+                # grab the structure for each MPID
                 structure = self.get_structure_by_material_id(mpid)
                 if supercell_structure:
                     if len(supercell_structure) == 3:
                         structure = StrucTools(structure).make_supercell(
                             supercell_structure
                         )
-                query[entry]["structure"] = structure.as_dict()
+                query[mpid]["structure"] = structure.as_dict()
 
         if max_sites_per_structure:
+            # remove entries that have too many sites
             query = {
                 e: query[e]
                 for e in query
                 if query[e]["nsites"] <= max_sites_per_structure
             }
 
         if max_Ehull:
-            if only_gs:
-                query = {
-                    e: query[e] for e in query if query[e]["Ehull_mp"] <= max_Ehull
-                }
-            else:
-                cmpds = sorted(list(set([query[e]["cmpd"] for e in query])))
-                mpids = [
-                    e
-                    for e in query
-                    if query[e]["Ehull_mp"] <= max_Ehull
-                    if query[e]["cmpd"] in cmpds
-                ]
-                query = {e: query[e] for e in mpids}
+            # remove entries that are too far above the hull
+            query = {e: query[e] for e in query if query[e]["Ehull_mp"] <= max_Ehull}
 
         if max_strucs_per_cmpd:
             if not only_gs:
                 trimmed_query = {}
                 cmpds = sorted(list(set([query[e]["cmpd"] for e in query])))
                 for cmpd in cmpds:
                     mpids = [e for e in query if query[e]["cmpd"] == cmpd]
@@ -383,85 +325,103 @@
                     if len(relevant_ids) > max_strucs_per_cmpd:
                         relevant_ids = relevant_ids[:max_strucs_per_cmpd]
                     for mpid in relevant_ids:
                         trimmed_query[mpid] = query[mpid]
 
                 return trimmed_query
 
+        # close rester
+        mpr.session.close()
         return query
 
     def get_entry_by_material_id(
         self,
         material_id,
         properties=None,
         incl_structure=True,
         conventional=False,
         compatible_only=True,
     ):
         """
         Args:
-            material_id (str) - MP ID of entry
-            properties (list) - list of properties to query
-            incl_structure (bool) - whether to include structure in entry
-            conventional (bool) - whether to use conventional unit cell
-            compatible_only (bool) - whether to only include compatible entries (related to MP formation energies)
+            material_id (str)
+                MP ID of entry
+
+            properties (list)
+                list of properties to query
+
+            incl_structure (bool)
+                whether to include structure in entry
+
+            conventional (bool)
+                whether to use conventional unit cell
+
+            compatible_only (bool)
+                whether to only include compatible entries (related to MP formation energies)
 
         Returns:
             ComputedEntry object
         """
-        return self.mpr.get_entry_by_material_id(
+        mpr = self.mpr
+        return mpr.get_entry_by_material_id(
             material_id, compatible_only, incl_structure, properties, conventional
         )
 
     def get_structure_by_material_id(self, material_id):
         """
         Args:
-            material_id (str) - MP ID of entry
+            material_id (str)
+                MP ID of entry
 
         Returns:
             Structure object
         """
-        return self.mpr.get_structure_by_material_id(material_id)
+        mpr = self.mpr
+        return mpr.get_structure_by_material_id(material_id)
 
     def get_incar(self, material_id):
         """
         Args:
-            material_id (str) - MP ID of entry
+            material_id (str)
+                MP ID of entry
 
         Returns:
             dict of incar settings
         """
-        return self.mpr.query(material_id, ["input.incar"])[0]
+        mpr = self.mpr
+        return mpr.query(material_id, ["input.incar"])[0]
 
     def get_kpoints(self, material_id):
         """
         Args:
-            material_id (str) - MP ID of entry
+            material_id (str)
+                MP ID of entry
 
         Returns:
             dict of kpoint settings
         """
-        return self.mpr.query(material_id, ["input.kpoints"])[0][
-            "input.kpoints"
-        ].as_dict()
+        mpr = self.mpr
+        return mpr.query(material_id, ["input.kpoints"])[0]["input.kpoints"].as_dict()
 
     def get_vasp_inputs(self, material_id):
         """
         Args:
-            material_id (str) - MP ID of entry
+            material_id (str)
+                MP ID of entry
 
         Returns:
             dict of vasp inputs
                 - 'incar' : {setting (str) : value (mixed type)}
                 - 'kpoints' : {'scheme' : (str), 'grid' : list of lists for 'A B C'}
                 - 'potcar' : [list of TITELs]
                 - 'structure' : Structure object as dict
         """
 
-        d = self.mpr.query(material_id, ["input"])[0]["input"]
+        mpr = self.mpr
+        d = mpr.query(material_id, ["input"])[0]["input"]
         d["kpoints"] = d["kpoints"].as_dict()
         d["kpoints"] = {
             "scheme": d["kpoints"]["generation_style"],
             "grid": d["kpoints"]["kpoints"],
         }
         d["potcar"] = [
             d["potcar_spec"][i]["titel"] for i in range(len(d["potcar_spec"]))
@@ -469,13 +429,12 @@
         d["poscar"] = self.get_structure_by_material_id(material_id).as_dict()
         del d["potcar_spec"]
 
         return d
 
 
 def main():
-
     return
 
 
 if __name__ == "__main__":
-    mpq = main()
+    out = main()
```

### Comparing `pydmclab-1.0.0/pydmclab/core/struc.py` & `pydmclab-1.0.1/pydmclab/core/struc.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from pymatgen.core.structure import Structure
 from pymatgen.transformations.standard_transformations import (
     OrderDisorderedStructureTransformation,
     AutoOxiStateDecorationTransformation,
     OxidationStateDecorationTransformation,
 )
 from pymatgen.analysis.structure_matcher import StructureMatcher
-from pymatgen.core.composition import Element, Composition
-from pymatgen.core.ion import Ion
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 
 import os
 import numpy as np
 
 
 class StrucTools(object):
@@ -26,16 +24,19 @@
             structure (Structure): pymatgen Structure object
                 - if dict, assumes it is Structure.as_dict(); converts to Structure object
                 - if str, assumes it is a path to a structure file, converts to Structure object
             ox_states (dict): dictionary of oxidation states {el (str) : oxidation state (int)}
                 - or None
 
         """
+        # convert Structure.as_dict() to Structure
         if isinstance(structure, dict):
             structure = Structure.from_dict(structure)
+
+        # convert file into Structure
         if isinstance(structure, str):
             if os.path.exists(structure):
                 structure = Structure.from_file(structure)
             else:
                 raise ValueError(
                     "you passed a string to StrucTools > this means a path to a structure > but the path is empty ..."
                 )
@@ -68,14 +69,29 @@
     @property
     def els(self):
         """
         list of unique elements (str) in structure
         """
         return CompTools(self.compact_formula).els
 
+    @property
+    def amts(self):
+        """
+        Returns:
+            {el (str): number of el in struc (int)}
+        """
+        els = self.els
+        amts = {el: 0 for el in els}
+        structure = self.structure
+        for i, site in enumerate(structure):
+            el = SiteTools(structure, i).el
+            if el:
+                amts[el] += 1
+        return amts
+
     def make_supercell(self, grid):
         """
         Args:
             grid (list) - [nx, ny, nz]
 
         Returns:
             Structure repeated nx, ny, nz
@@ -96,43 +112,71 @@
         Returns:
             Structure w/ perturbations
         """
         structure = self.structure
         structure.perturb(perturbation)
         return structure
 
-    def change_occ(self, site_idx, new_occ, structure=None):
+    def change_occ_for_site(self, site_idx, new_occ, structure=None):
         """
 
         return a structure with a new occupation for some site
 
         Args:
-            site_idx (int): index of site in structure to change
-            new_occ (dict): dictionary telling me the new occupation on that site
-                e.g., {'Li' : 0.5, 'Fe' : 0.5}
+            site_idx (int):
+                index of site in structure to change
+
+            new_occ (dict):
+                dictionary telling me the new occupation on that site
+                    e.g., {'Li' : 0.5, 'Fe' : 0.5}
 
             structure (None or pymatgen Structure object):
                 if None, start from self.structure
                 else, start from structure
+                    (in case you don't want to start from the structure that initialized StrucTools)
 
         Returns:
             pymatgen Structure object with new occupation
         """
 
         if not structure:
             structure = self.structure
 
         s = structure.copy()
 
         if np.sum(list(new_occ.values())) == 0:
+            # if new occupation is 0, remove that site
             s.remove_sites([site_idx])
         else:
+            # otherwise, update the occupation
             s[site_idx].species = new_occ
         return s
 
+    def change_occ_for_el(self, el, new_occ, structure=None):
+        """
+        Args:
+            el (str)
+                element to change occupation for
+
+            new_occ (dict)
+                {el : new occupation (float)}
+
+            structure (None or pymatgen Structure object)
+                if None, start from self.structure
+        """
+        if not structure:
+            structure = self.structure
+
+        # for all sites having that element, change the occupation
+        for i, site in enumerate(structure):
+            if SiteTools(structure, i).el == el:
+                structure = self.change_occ_for_site(i, new_occ, structure=structure)
+
+        return structure
+
     @property
     def decorate_with_ox_states(self):
         """
         Returns oxidation state decorated structure
             - uses Auto algorithm if no ox_states are provided
             - otherwise, applies ox_states
         """
@@ -148,118 +192,140 @@
             )
             print("     using %s" % str(ox_states))
         return transformer.apply_transformation(structure)
 
     def get_ordered_structures(self, algo=0, decorate=True, n_strucs=1):
         """
         Args:
-            algo (int) - 0 = fast, 1 = complete, 2 = best first
-                - see pymatgen.transformations.standard_transformations.OrderDisorderedStructureTransformation
-                - 0 usually OK
-            decorate (bool) - whether to decorate with oxidation states
-                - if False, self.structure must already have them
-            n_strucs (int) - number of ordered structures to return
+            algo (int):
+                method for enumeration
+                    0 = fast, 1 = complete, 2 = best first
+                        see pymatgen.transformations.standard_transformations.OrderDisorderedStructureTransformation
+                        0 usually OK
+
+            decorate (bool)
+                whether to decorate with oxidation states
+                    if False, self.structure must already have them
+
+            n_strucs (int)
+                number of ordered structures to return
 
         Returns:
-            dict of ordered structures {index : structure (Structure.as_dict())}
+            dict of ordered structures
+            {index : structure (Structure.as_dict())}
                 - index = 0 has lowest Ewald energy
         """
+
+        # initialize ordering engine
         transformer = OrderDisorderedStructureTransformation(algo=algo)
+
+        # decorat with oxidation states or not
         if decorate:
             structure = self.decorate_with_ox_states
         else:
             structure = self.structure
+
+        # only return one structure if n_strucs = 1
         return_ranked_list = n_strucs if n_strucs > 1 else False
 
+        # generate ordered structure
         print("ordering disordered structures\n")
         out = transformer.apply_transformation(
             structure, return_ranked_list=return_ranked_list
         )
-        out = [i["structure"] for i in out]
-        # print(out[0])
+
         if isinstance(out, list):
+            # more than 1 structure, so check for duplicates (symmetrically equivalent structures) and remove them
             print("getting unique structures\n")
             matcher = StructureMatcher()
+            out = [i["structure"] for i in out]
+            # find unique groups of structures
             groups = matcher.group_structures(out)
             out = [groups[i][0] for i in range(len(groups))]
             return {i: out[i].as_dict() for i in range(len(out))}
         else:
+            # if only one structure is made, return in same formation (dict)
             return {0: out.as_dict()}
 
-    def replace_species(self, species_mapping, n_strucs=1):
+    def replace_species(
+        self,
+        species_mapping,
+        n_strucs=1,
+        use_ox_states_in_mapping=False,
+        use_occ_in_mapping=True,
+    ):
         """
         Args:
-            species_mapping (dict) - {Element(el) :
-                                        {Element(el1) : fraction el1,
-                                                        fraction el2}}
-            n_strucs (int) - number of ordered structures to return if disordered
-
-        Returns:
-            dict of ordered structures {index : structure (Structure.as_dict())}
-                - index = 0 has lowest Ewald energy
+            species_mapping (dict)
+                {Element(el) :
+                    {Element(el1) : fraction el1,
+                     Element(el2) : fraction el2,
+                     ...},
+                 ...}
+
+            n_strucs (int)
+                number of ordered structures to return if disordered
+
+            use_ox_states_in_mapping (bool)
+                if False, will remove oxidation states before doing replacements
+
+            use_occ_in_mapping (bool)
+                if False, will set all occupancies to 1.0 before doing replacements
+
+        Returns:
+            dict of ordered structures
+                {index : structure (Structure.as_dict())}
+                    index = 0 has lowest Ewald energy
         """
         structure = self.structure
         print("replacing species with %s\n" % str(species_mapping))
 
+        # purge oxidation states if you'd like
+        if not use_ox_states_in_mapping:
+            structure.remove_oxidation_states()
+
+        # ignore the original occupancies if you'd like (sometimes convenient)
+        if not use_occ_in_mapping:
+            els = self.els
+            for el in els:
+                structure = self.change_occ_for_el(el, {el: 1.0}, structure=structure)
+
+        # figure out which elements have occupancy becoming 0
         disappearing_els = []
         for el_to_replace in species_mapping:
             if (len(species_mapping[el_to_replace]) == 1) and (
                 list(species_mapping[el_to_replace].values())[0] == 0
             ):
                 structure.remove_species(species=[el_to_replace])
                 disappearing_els.append(el_to_replace)
 
+        # remove these no longer existing elements
         if disappearing_els:
             for el in disappearing_els:
                 del species_mapping[el]
 
+        # replace species according to mapping
         if species_mapping:
             structure.replace_species(species_mapping)
+
         if structure.is_ordered:
+            # if the replacement leads to an ordered structure, return it (in a dict)
             return {0: structure.as_dict()}
         else:
+            # otherwise, need to order this partially occupied structure
             structools = StrucTools(structure, self.ox_states)
             return structools.get_ordered_structures(n_strucs=n_strucs)
 
-    def BROKEN_get_structures_with_dilute_vacancy(
-        self, el_to_replace, n_strucs=1, structure=None
-    ):
-        """
-        @TODO: revisit this
-
-
-        Args:
-            el_to_replace (str) - element to replace with vacancy
-            n_strucs (int) - number of ordered structures to return if disordered
-            structure (Structure) - structure to create vacancy in
-                - if None, use self.structure
-
-        Returns:
-            dict of ordered structures {index : structure (Structure.as_dict())}
-                - each structure will be missing 1 el_to_replace
-        """
-        if not structure:
-            s = self.structure
-        else:
-            s = structure
-        species_mapping = {
-            Element(el_to_replace): {Element(el_to_replace): 1 - 1 / len(s)}
-        }
-        if not structure:
-            return self.replace_species(species_mapping, n_strucs=n_strucs)
-        else:
-            return StrucTools(structure).replace_species(
-                species_mapping, n_strucs=n_strucs
-            )
-
     @property
     def spacegroup_info(self):
         """
         Returns:
             dict of spacegroup info with 'tight' or 'loose' symmetry tolerance
+                tight means symprec = 0.01
+                loose means symprec = 0.1
             e.g.,
                 data['tight']['number'] returns spacegroup number with tight tolerance
                 data['loose']['symbol'] returns spacegroup symbol with loose tolerance
 
         """
         data = {
             "tight": {"symprec": 0.01, "number": None, "symbol": None},
@@ -282,25 +348,30 @@
 
     def sg(self, number_or_symbol="symbol", loose_or_tight="loose"):
         """
 
         returns spacegroup number of symbol with loose or tight tolerance
 
         Args:
-            number_or_symbol (str, optional): _description_. Defaults to 'symbol'.
-            loose_or_tight (str, optional): _description_. Defaults to 'loose'.
+            number_or_symbol (str):
+                whether to return the number or the symbol
+
+            loose_or_tight (str):
+                whether to use the loose or tight tolerance
 
         Returns:
-            spacegroup number or symbol with loose or tight tolerance
+            spacegroup number (int) or symbol (str) with loose or tight tolerance
         """
         sg_info = self.spacegroup_info
         return sg_info[loose_or_tight][number_or_symbol]
 
     def scale_structure(self, scale_factor, structure=None):
-        """_summary_
+        """
+
+        Isotropically scale a structure
 
         Args:
             scale_factor (float): fractional scaling of the structure volume
                 - e.g., 1.2 will increase each lattice vector by 20%
                 - e.g., 0.8 will make eaech lattice vector 80% of the initial length
                 - e.g., 1.0 will do nothing
 
@@ -312,43 +383,51 @@
         """
         if not structure:
             structure = self.structure.copy()
         else:
             structure = structure.copy()
         orig_vol = structure.volume
         new_vol = orig_vol * scale_factor
+
+        # scaling occurs only on the lattice (i.e., the top of POSCAR)
         structure.scale_lattice(new_vol)
 
         return structure
 
 
 class SiteTools(object):
     """
-    make it a little easier to get site info from structures
+    Purpose: make it a little easier to get site info from structures
 
     """
 
     def __init__(self, structure, index):
         """
         Args:
-            structure (Structure) - pymatgen structure
-            index (int) - index of site in structure
+            structure (Structure)
+                pymatgen Structure
+
+            index (int)
+                index of site in structure
 
         Returns:
             pymatgen Site object
         """
-        if isinstance(structure, dict):
-            structure = Structure.from_dict(structure)
+        structure = StrucTools(structure).structure
         self.site = structure[index]
 
     @property
     def site_dict(self):
         """
         Returns:
             dict of site info (from Pymatgen)
+                {'species' : [{'element' : element, 'occu' : occupation, ...}, {...}}],
+                 'abc' : fractional coordinates ([a, b, c])
+                 'lattice' : Lattice object,
+                 'properties' : dict (e.g., {'magmom' : 3})}
         """
         return self.site.as_dict()
 
     @property
     def coords(self):
         """
         Returns:
@@ -373,43 +452,95 @@
         """
         Returns:
             True if site is fully occupied else False
         """
         return self.site.is_ordered
 
     @property
+    def site_string(self):
+        """
+        unique string to represent a complex site
+
+        Returns:
+            occupation_element_oxstate__occupation_element_oxstate__... for each ion occupying a site
+        """
+        d = self.site_dict
+        species = d["species"]
+        ions = []
+        for entry in species:
+            el = entry["element"]
+            if "oxidation_state" in entry:
+                ox = float(entry["oxidation_state"])
+            else:
+                ox = None
+            occ = float(entry["occu"])
+            if ox:
+                if ox < 0:
+                    ox = str(abs(ox)) + "-"
+                else:
+                    ox = str(ox) + "+"
+            else:
+                ox = "0.0+"
+            occ = str(occ)
+            name_to_join = []
+            for thing in [occ, el, ox]:
+                if thing:
+                    name_to_join.append(thing)
+            name = "_".join(name_to_join)
+            ions.append(name)
+        if len(ions) == 1:
+            return ions[0]
+        else:
+            return "__".join(ions)
+
+    @property
     def ion(self):
         """
         Returns:
-            whatever is occupying site (str)
-                - could be multiple ions, multiple elements, one element, one ion, etc
+            the ion (element + oxidation state) occupying the site (str)
+                None if > 1 ion
         """
-        return self.site.species_string
+        site_string = self.site_string
+        if "__" in site_string:
+            print("Multiple ions in site, returning None")
+            return None
+
+        return "".join([site_string.split("_")[1], site_string.split("_")[2]])
 
     @property
     def el(self):
         """
         Returns:
-            just the element occupying the site (even if it has an oxidation state)
+            just the element occupying the site (str)
+                even if it has an oxidation state)
+
+            None if more than one element occupies a site
         """
-        return CompTools(Composition(self.ion).formula).els[0]
+        site_string = self.site_string
+        if "__" in site_string:
+            print("Multiple ions in site, returning None")
+            return None
+
+        return site_string.split("_")[1]
 
     @property
     def ox_state(self):
         """
         Returns:
             oxidation state (float) of site
+                averaged over all ions occupying the site
         """
-        if self.is_fully_occ:
-            return self.site_dict["species"][0]["oxidation_state"]
-        else:
-            print("cant determine ox state for partially occ site")
-            return None
+        d = self.site_dict
+        ox = 0
+        species = d["species"]
+        for entry in species:
+            if entry["oxidation_state"]:
+                ox += entry["oxidation_state"] * entry["occu"]
+        return ox
 
 
 def main():
-
     return
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pydmclab-1.0.0/pydmclab/data/.DS_Store` & `pydmclab-1.0.1/pydmclab/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.0/pydmclab/data/configs.py` & `pydmclab-1.0.1/pydmclab/data/configs.py`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.0/pydmclab/data/data/221220_dmc-mus.json` & `pydmclab-1.0.1/pydmclab/data/data/221220_dmc-mus.json`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.0/pydmclab/data/data/230122_dmc-mus.json` & `pydmclab-1.0.1/pydmclab/data/data/230122_dmc-mus.json`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.0/pydmclab/data/data/_batch_vasp_analysis_configs.yaml` & `pydmclab-1.0.1/pydmclab/data/data/_batch_vasp_analysis_configs.yaml`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.0/pydmclab/data/data/_partition_configs.yaml` & `pydmclab-1.0.1/pydmclab/data/data/_partition_configs.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+RM:
+  cores_per_node: 128
+  sharing: False
+  max_wall: 48:00:00
+  mem_per_core: 2GB
+  max_nodes: 50
+  proc: cpu
+RM-shared:
+  cores_per_node: 128
+  sharing: True
+  max_wall: 48:00:00
+  mem_per_core: 2GB
+  max_nodes: 1
+  proc: cpu
+RM-512:
+  cores_per_node: 128
+  sharing: False
+  max_wall: 48:00:00
+  mem_per_core: 4GB
+  max_nodes: 2
+  proc: cpu
+msidmc:
+  cores_per_node: 128
+  sharing: True
+  max_wall: 96:00:00
+  mem_per_core: 4GB
+  max_nodes: 1
+  proc: cpu
 agsmall:
   cores_per_node: 128
   sharing: True
   max_wall: 96:00:00
   mem_per_core: 4GB
   max_nodes: 1
   proc: cpu
```

### Comparing `pydmclab-1.0.0/pydmclab/data/data/_slurm_configs.yaml` & `pydmclab-1.0.1/pydmclab/data/data/_slurm_configs.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -2,10 +2,10 @@
 ntasks: 8 # how many total cores
 time: 1440 # how long in minutes before hitting walltime 
 error: log.e # where to write slurm errors to in launch_dir
 output: log.o # where to write slurm output to in launch_dir
 account: cbartel # account to charge
 partition: msismall # partition to use
 job-name: # unique job name; if none provided, will default to formula.id.standard.mag.xc
-mem: # if you need more memory specify here (e.g., 128GB)
+mem: # if you need more memory specify here (e.g., 128GB) (total requested memory)
 constraint: # may not need this ever on MSI
 qos: # may not need this ever on MSI
```

### Comparing `pydmclab-1.0.0/pydmclab/data/data/_sub_configs.yaml` & `pydmclab-1.0.1/pydmclab/data/data/_sub_configs.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 vasp: vasp_std # use vasp_gam for "loose" calcs (havent implemented yet)
-vasp_dir: /home/cbartel/shared/bin/vasp/ # where vasp executable lives
+#vasp_dir: /home/cbartel/shared/bin/vasp/ # where vasp executable lives
 mpi_command: mpirun # how to launch on multicore/multinode (may be mpirun depending on compilation)
 manager: '#SBATCH' # how to manage interactions with the queue (some machines dont use slurm)
+machine: msi # which supercomputer
 
 fqueue: q.o # this will be created in the folder where you execute python
 
 fresh_restart: False # True if you want to re-run all calculations; False if you want to pick up where you left off
 force_postprocess: False # if True, run LOBSTER and Bader again if vasp_configs.lobster_static = True even if output files exist
 
 files_to_inherit: ['WAVECAR', 'CONTCAR'] # usually no need to change
```

### Comparing `pydmclab-1.0.0/pydmclab/data/data/_vasp_configs.yaml` & `pydmclab-1.0.1/pydmclab/data/data/_vasp_configs.yaml`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.0/pydmclab/data/data/atomic_masses.json` & `pydmclab-1.0.1/pydmclab/data/data/atomic_masses.json`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.0/pydmclab/data/data/bartel2019_npj_reference-energies.csv` & `pydmclab-1.0.1/pydmclab/data/data/bartel2019_npj_reference-energies.csv`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.0/pydmclab/data/data/colors.json` & `pydmclab-1.0.1/pydmclab/data/data/colors.json`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.0/pydmclab/data/data/elemental_gibbs_energies_T.json` & `pydmclab-1.0.1/pydmclab/data/data/elemental_gibbs_energies_T.json`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.0/pydmclab/data/data/mus_from_bartel2019_npj.json` & `pydmclab-1.0.1/pydmclab/data/data/mus_from_bartel2019_npj.json`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.0/pydmclab/data/data/mus_from_mp_no_corrections.json` & `pydmclab-1.0.1/pydmclab/data/data/mus_from_mp_no_corrections.json`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.0/pydmclab/data/data/ssub.dat` & `pydmclab-1.0.1/pydmclab/data/data/ssub.dat`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.0/pydmclab/data/data/ssub.json` & `pydmclab-1.0.1/pydmclab/data/data/ssub.json`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.0/pydmclab/data/plotting_configs.py` & `pydmclab-1.0.1/pydmclab/data/plotting_configs.py`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.0/pydmclab/data/thermochem.py` & `pydmclab-1.0.1/pydmclab/data/thermochem.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     """
     These were run by Bartel in January 20223
     """
     fjson = os.path.join(DATA_PATH, "mus_from_dmc_no_corrections.json")
     if os.path.exists(fjson):
         return read_json(fjson)
     mus = {}
-    d = read_json(os.path.join(DATA_PATH, "230122_dmc-mus.json"))
+    d = read_json(os.path.join(DATA_PATH, "230614_dmc-mus.json"))
     for xc in d:
         if xc == "gga":
             functional = "pbe"
         elif xc == "metagga":
             functional = "r2scan"
         mus[functional] = d[xc]
     return write_json(mus, fjson)
@@ -146,17 +146,23 @@
         "scan_fit": metagga_fit,
     }
 
     data = {xc: {el: xcs[xc][i] for i, el in enumerate(els)} for xc in xcs}
     return write_json(data, fjson)
 
 
+def gas_thermo_data():
+    fjson = os.path.join(DATA_PATH, "gas_thermo_data_nist.json")
+    if os.path.exists(fjson):
+        return read_json(fjson)
+
+
 def main():
-    mus_from_bartel2019_npj()
-    ssub()
-    mus_from_mp_no_corrections()
+    # mus_from_bartel2019_npj()
+    # ssub()
+    # mus_from_mp_no_corrections()
     mus_at_0K()
-    mus_at_T()
+    # mus_at_T()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pydmclab-1.0.0/pydmclab/demos/demo_hulls.py` & `pydmclab-1.0.1/pydmclab/demos/demo_hulls.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,194 +1,279 @@
 from pydmclab.core.comp import CompTools
 from pydmclab.core.query import MPQuery
-from pydmclab.core.hulls import GetHullInputData, AnalyzeHull, ParallelHulls
+from pydmclab.core.hulls import GetHullInputData, AnalyzeHull, ParallelHulls, MixingHull
 from pydmclab.utils.handy import read_json, write_json
-from pydmclab.utils.plotting import set_rc_params, get_colors
-from pydmclab.data.thermochem import mus_at_0K, mus_at_T
-
+from pydmclab.plotting.utils import set_rc_params, get_colors
 import matplotlib.pyplot as plt
 
 import os
 import numpy as np
 
 set_rc_params()
 
-"""
-This file currently tests the following classes in ThermoTools
-    - GetHullInputData
-    - AnalyzeHull
-    - ParallelHulls
+""" 
+Purpose: 
+    The convex hull analysis is central to understanding the stability of materials
+        Convex hulls are made from formation energy vs composition analyses for a given chemical space
+          Standard hulls using formation energies, which are referenced to elemental phases
+            These formation energies can be DFT dEf(0 K), dGf(T, p), dphi_f(T, p, mu) etc
+          Hulls can also be made from an arbitrary reference (e.g., energies relative to chosen end-member compounds)
+            In pydmclab, these are called "Mixing Hulls"
+    
+    Typical hulls (elemental end-members, n-dimensional for n elements in a chemical space)
+        Serial mode:
+          - GetHullInputData prepares the input
+          - AnalyzeHull processes it
+        Parallel mode:
+          - ParallelHulls does it all
+    
+    Mixing hulls (compound end-members, 2D supported, n-d coming later)
+        MixingHulls
+  
+Unit tests:
+  - see pydmclab/tests/test_hulls.py
 
-TO-DO:
-    - convert into formal "tests"
 """
 # Chris B's API key for MP query
 API_KEY = "N3KdATtMmcsUL94g"
 
 # chemical system to test on
-CHEMSYS = "Ca-Al-Ti-F"
+CHEMSYS = "Li-Nb-O-F"
 
 # where to save data
 DATA_DIR = os.path.join("output", "hulls", "data")
 if not os.path.exists(DATA_DIR):
     os.mkdir(DATA_DIR)
 
 # where to save figures
 FIG_DIR = os.path.join("output", "hulls", "figures")
 if not os.path.exists(FIG_DIR):
     os.mkdir(FIG_DIR)
 
 
 def get_mp_data_for_chemsys(
     comp=CHEMSYS,
-    properties=None,
-    criteria={},
     only_gs=True,
-    include_structure=True,
-    supercell_structure=False,
-    max_Ehull=0.1,
-    max_sites_per_structure=100,
-    max_strucs_per_cmpd=5,
     data_dir=DATA_DIR,
     remake=False,
 ):
     """
+    Query MP to get some data for a chemical system to paly around with
+
     Args:
-        chemsys (str): chemical system to query ('-'.join([elements]))
-        only_gs (bool): if True, remove non-ground state polymorphs from MP query
-            - good practice to do this before doing hull analysis b/c non-gs polymorphs trivially have Ehull=Ehull_gs + dE_polymorph-gs
-        dict_key (str): key to use to orient dictionary of MPQuery results
-            - 'cmpd' is the default behavior in MPQuery, meaning we get a dictionary that looks like {CHEMICAL_FORMULA : {DATA}}
-        remake (bool): if True, re-query MP
+        chemsys (str)
+            chemical system to query ('-'.join([elements]))
+
+        only_gs (bool):
+            if True, remove non-ground state polymorphs from MP query
+                good practice to do this before doing hull analysis b/c non-gs polymorphs trivially have Ehull=Ehull_gs + dE_polymorph-gs
+
+        data_dir (str):
+            directory to save data
+
+        remake (bool):
+            if True, re-query MP
 
     Returns:
-        gs (dict): dictionary of ground state data from MPQuery for chemsys
+        gs (dict)
+            dictionary of ground state data from MPQuery for chemsys
+                {formula (str) : {'Ef_mp' : formation energy (eV/atom)}
     """
     fjson = os.path.join(data_dir, "query_" + comp + ".json")
     if not remake and os.path.exists(fjson):
         return read_json(fjson)
 
     mpq = MPQuery(API_KEY)
     d = mpq.get_data_for_comp(comp=comp, only_gs=only_gs)
 
+    # data is MPID-keyed, let's make it formula-keyed
     out = {}
     formulas = list(set([d[k]["cmpd"] for k in d]))
     for formula in formulas:
         # NOTE: this only works because I know my query only has 1 structure per formula (only_gs = True)
         gs_key = [k for k in d if d[k]["cmpd"] == formula][0]
         out[formula] = d[gs_key]
     return write_json(out, fjson)
 
 
 def serial_get_hull_input_data(
     gs, formation_energy_key="Ef_mp", remake=False, data_dir=DATA_DIR, chemsys=CHEMSYS
 ):
     """
+    Let's prepare the hull input file for a "typical" (element-bounded) nD hull
+
     Args:
-        gs (dict): dictionary of ground state data from MPQuery for chemsys
-            - generated with get_mp_data_for_chemsys()
-        formation_energy_key (str): key to use for formation energy in gs
-            - 'Ef_mp' is default behavior in MPQuery
-        remake (bool): if True, re-calculate hull input data
-        data_dir (str): directory to save data
-        chemsys (str): chemical system to query ('-'.join([elements]))
+        gs (dict)
+            dictionary of ground state data from MPQuery for chemsys
+                {formula (str) : {'Ef_mp' : formation energy (eV/atom)}
+
+        formation_energy_key (str):
+            key to use for formation energy in gs
+                'Ef_mp' is default behavior in MPQuery
+
+        remake (bool)
+            if True, re-calculate hull input data
+
+        data_dir (str)
+            directory to save data
+
+        chemsys (str)
+            chemical system to query ('-'.join([elements]))
+                just used to generate the savename for the .json
 
     Returns:
-        hullin (dict): dictionary of hull input data for gs
-            dict of {chemical space (str) : {formula (str) : {'E' : formation energy (float),
-                                                              'amts' : {el (str) : fractional amt of el in formula (float) for el in space}}
-                                            for all relevant formulas including elements}
-                - elements are automatically given formation energy = 0
-                - chemical space is now in 'el1_el2_...' format to be jsonable
-                - each "chemical space" is a convex hull that must be computed
+        hullin (dict):
+            dictionary of hull input data for gs
+                {chemical space (str) :
+                    {formula (str) :
+                        {'E' : formation energy (float),
+                         'amts' :
+                            {el (str) :
+                                fractional amt of el in formula (float) for el in space
+                                }
+                            }
+                                for all relevant formulas including elements}
+                    - elements are automatically given formation energy = 0
+                    - chemical space is now in 'el1_el2_...' format to be jsonable
+                    - each "chemical space" is a convex hull that must be computed
     """
     fjson = os.path.join(data_dir, "hullin_serial_" + chemsys + ".json")
     if not remake and os.path.exists(fjson):
         return read_json(fjson)
 
     ghid = GetHullInputData(gs, formation_energy_key=formation_energy_key)
     return ghid.hullin_data(fjson=fjson, remake=remake)
 
 
 def serial_get_hull_output_data(
     hullin, remake=False, chemsys=CHEMSYS, data_dir=DATA_DIR
 ):
     """
+    Now, let's solve the hull we initialized
+
     Args:
-        hullin (dict): dictionary of hull input data for gs
-        remake (bool): if True, re-calculate hull output data
-        chemsys (str): chemical system to query ('-'.join([elements]))
-        data_dir (str): directory to save data
+        hullin (dict)
+            dictionary of hull input data for chemical system
+
+        remake (bool)
+            if True, re-calculate hull output data
+
+        chemsys (str)
+            chemical system to query ('-'.join([elements]))
+                only used for savename
+
+        data_dir (str)
+            directory to save data
 
     Returns:
         stability data (dict) for all compounds in the specified chemical space
-            {compound (str) : {'Ef' : formation energy (float),
-                                'Ed' : decomposition energy (float),
-                                'rxn' : decomposition reaction (str),
-                                'stability' : stable (True) or unstable (False)}}
+            {compound (str) :
+                {'Ef' : formation energy (float),
+                 'Ed' : decomposition energy (float),
+                 'rxn' : decomposition reaction (str),
+                 'stability' : stable (True) or unstable (False)
+                 }
+                 for all compounds in the chemical space
+            }
     """
     fjson = os.path.join(data_dir, "hullout_serial_" + chemsys + ".json")
     if not remake and os.path.exists(fjson):
         return read_json(fjson)
 
     hullout = {}
+    # loop through each chemical (sub)space in the hullin dictionary
     for space in hullin:
         ah = AnalyzeHull(hullin, space)
+        # loop through every compound in that space
         for cmpd in hullin[space]:
             print("\n%s" % cmpd)
+            # get the stability data for that compound
             hullout[cmpd] = ah.cmpd_hull_output_data(cmpd)
     return write_json(hullout, fjson)
 
 
 def parallel_get_hull_input_and_output_data(
     gs, remake=False, chemsys=CHEMSYS, data_dir=DATA_DIR, n_procs=2, fresh_restart=True
 ):
     """
+    Repeat what we did with GetHullInputData + AnalyzeHull, but now in parallel
+
     Args:
-        gs (dict): dictionary of ground state data from MPQuery for chemsys
-        remake (bool): if True, re-calculate hull input and output data
-        chemsys (str): chemical system to query ('-'.join([elements]))
-        data_dir (str): directory to save data
-        n_procs (int): number of processors to use (could also be 'all' to use multip.cpu_count()-1 procs)
-        fresh_restart (bool): if True, restart ParallelHull process from scratch
+        gs (dict)
+            dictionary of ground state data from MPQuery for chemsys
+                {formula (str) : {'Ef_mp' : formation energy (eV/atom)}}
+                }
+        remake (bool)
+            if True, re-calculate hull input and output data
+
+        chemsys (str)
+            chemical system to query ('-'.join([elements]))
+                only for savename
+
+        data_dir (str)
+            directory to save data
+
+        n_procs (int)
+            number of processors to use
+                could also be 'all' to use multip.cpu_count()-1 procs
+
+        fresh_restart (bool)
+            if True, restart ParallelHull process from scratch
+            if False, use the files we've already written from a previous execution
 
     Returns:
         stability data (dict) for all compounds in the specified chemical space
-            {compound (str) : {'Ef' : formation energy (float),
-                                'Ed' : decomposition energy (float),
-                                'rxn' : decomposition reaction (str),
-                                'stability' : stable (True) or unstable (False)}}
-            written to fjson
-            also writes small_spaces and hullin data resulting from ParallelHull to json
+            {compound (str) :
+                {'Ef' : formation energy (float),
+                 'Ed' : decomposition energy (float),
+                 'rxn' : decomposition reaction (str),
+                 'stability' : stable (True) or unstable (False)
+                 }
+                 for all compounds in the chemical space
+            }
     """
     fjson = os.path.join(data_dir, "hullout_parallel_" + chemsys + ".json")
     if not remake and os.path.exists(fjson):
         return read_json(fjson)
+
     ph = ParallelHulls(gs, n_procs=n_procs, fresh_restart=fresh_restart)
+
+    # prepare hull input data
     hullin = ph.parallel_hullin(fjson=fjson.replace("hullout", "hullin"))
+
+    # identify the simplest hull that can be solved for each compound
     smallest_spaces = ph.smallest_spaces(
         hullin=hullin, fjson=fjson.replace("hullout", "small_spaces")
     )
+
+    # solve these minimally complex hulls for every compound
     return ph.parallel_hullout(
         hullin=hullin, smallest_spaces=smallest_spaces, fjson=fjson, remake=True
     )
 
 
 def plot_to_check_success(gs, serial_hullout, parallel_hullout):
     """
+    Let's make sure things worked
+        1) Parallel and serial should give the same results
+        2) For unstable compounds (above the hull), our Ed results and MP E above hull should be the same
+        3) For stable compounds, our Ed results will be negative; MP's should be E above hull = 0
+
     Args:
-        gs (dict): dictionary of ground state data from MPQuery for chemsys
-        serial_hullout (dict): dictionary of hull output data for gs (run serially)
-        parallel_hullout (dict): dictionary of hull output data for gs (run in parallel)
+        gs (dict)
+            dictionary of ground state data from MPQuery for chemsys
+
+        serial_hullout (dict)
+            dictionary of hull output data for gs (run serially)
+
+        parallel_hullout (dict)
+            dictionary of hull output data for gs (run in parallel)
 
     Returns:
-        compares serial and parallel hull output data (should be identica)
-        compares serial and MP hull output data
-            - should be identical (or very close) for unstable compounds
-            - for stable compounds, MP will have Ehull = 0, whereas our code will compure Ed < 0
+        a couple scatter plots
 
     """
     set_rc_params()
 
     fig = plt.figure(figsize=(8, 3))
 
     params = {
@@ -256,25 +341,64 @@
         print("mp hull = %.3f" % gs[k]["Ehull_mp"])
 
     # plt.show()
 
     fig.savefig(os.path.join(FIG_DIR, "pd_demo_check.png"))
 
 
+def demo_mixing_hull(gs, end_members, remake=False):
+    """
+    Now, we'll do a "mixing hull"
+        A convex hull with compounds as end members
+
+    e.g., a 2D hull bounded by LiNbO3-Li2NbO3
+
+    Args:
+        gs (dict)
+            dictionary of ground state data from MPQuery for chemsys
+
+        end_members (list)
+            list of end members to use for mixing hull
+
+        remake (bool)
+
+    """
+    fjson = os.path.join(
+        DATA_DIR, "pd_demo_mixing_hull_%s-%s.json" % (end_members[0], end_members[1])
+    )
+    if not remake and os.path.exists(fjson):
+        return read_json(fjson)
+
+    mh = MixingHull(
+        input_energies=gs,
+        varying_element="Li",
+        end_members=end_members,
+        shared_element_basis="Nb",
+        energy_key="Ef_mp",
+    )
+    out = mh.results
+    for k in out:
+        if out[k]["stability"]:
+            print(k)
+            print(out[k]["x"])
+
+
 def main():
     # if True, re-grab data from MP
-    remake_query = True
+    remake_query = False
     # if True, re-calculate hull input data
-    remake_serial_hullin = True
+    remake_serial_hullin = False
     # if True, re-calculate hull output data
-    remake_serial_hullout = True
+    remake_serial_hullout = False
     # if True, re-calculate hull output data in parallel
-    remake_parallel_hullout = True
+    remake_parallel_hullout = False
     # if True, generate figure to check results
-    remake_hull_figure_check = True
+    remake_hull_figure_check = False
+    # if True, remake mixing hull
+    remake_mixing_hull = False
 
     # MP query for CHEMSYS
     gs = get_mp_data_for_chemsys(CHEMSYS, remake=remake_query)
 
     # hull input data for CHEMSYS
     hullin = serial_get_hull_input_data(gs, remake=remake_serial_hullin)
 
@@ -284,17 +408,17 @@
     # hull output data for CHEMSYS (generated using parallelization)
     p_hullout = parallel_get_hull_input_and_output_data(
         gs, remake=remake_parallel_hullout
     )
 
     # generate a graph that compares serial vs parallel hull output and also compares ThermoTools hull output to MP hull data
     if remake_hull_figure_check:
-        # %%
         plot_to_check_success(gs, hullout, p_hullout)
-        # %%
 
+    # generate a mixing hull
+    mixing = demo_mixing_hull(gs, ["NbO2", "LiNbO2"], remake=remake_mixing_hull)
     return gs, hullin, hullout, p_hullout
 
 
 if __name__ == "__main__":
     # MP Query --> hull input data (serial) --> hull output data (serial) --> hull output data (parallel)
     gs = main()
```

### Comparing `pydmclab-1.0.0/pydmclab/demos/demo_launcher_template.py` & `pydmclab-1.0.1/pydmclab/hpc/helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,159 +1,426 @@
-import os
-import numpy as np
 import multiprocessing as multip
-
-from pydmclab.utils.handy import read_json, write_json, make_sub_for_launcher
+import os
+from pydmclab.hpc.launch import LaunchTools
+from pydmclab.hpc.submit import SubmitTools
+from pydmclab.hpc.analyze import AnalyzeVASP, AnalyzeBatch
 from pydmclab.core.query import MPQuery
-from pydmclab.core.mag import MagTools
 from pydmclab.core.struc import StrucTools
-from pydmclab.hpc.launch import LaunchTools, get_launch_configs
-from pydmclab.hpc.submit import (
-    SubmitTools,
-    get_vasp_configs,
-    get_slurm_configs,
-    get_sub_configs,
-)
-from pydmclab.hpc.analyze import AnalyzeBatch, get_analysis_configs
-
+from pydmclab.core.mag import MagTools
 from pydmclab.core.energies import ChemPots, FormationEnthalpy
+from pydmclab.utils.handy import read_json, write_json
+
+
+def get_vasp_configs(
+    run_lobster=False,
+    modify_loose_incar=False,
+    modify_relax_incar=False,
+    modify_static_incar=False,
+    modify_loose_kpoints=False,
+    modify_relax_kpoints=False,
+    modify_static_kpoints=False,
+    modify_loose_potcar=False,
+    modify_relax_potcar=False,
+    modify_static_potcar=False,
+):
+    """
+
+    how to modify VASP calculations from the defaults (see pydmclab.hpc.vasp for defaults)
+
+    Args:
+        run_lobster (bool, optional): True to run LOBSTER
+
+        modify_loose_incar (bool, optional):
+            - dictionary of {incar flag (str) : setting for that flag}
+            - modifies only the "loose" calculations
+        modify_relax_incar (bool, optional):
+            - dictionary of {incar flag (str) : setting for that flag}
+            - modifies only the "relax" calculations
+        modify_static_incar (bool, optional):
+            - dictionary of {incar flag (str) : setting for that flag}
+            - modifies only the "static" calculations
+
+
+        modify_loose_kpoints (bool, optional):
+            - dictionary of non-default K-point setting. see pydmclab.hpc.vasp for format
+            - modifies only the "loose" calculations
+        modify_relax_kpoints (bool, optional):
+            - dictionary of non-default K-point setting. see pydmclab.hpc.vasp for format
+            - modifies only the "relax" calculations
+        modify_static_kpoints (bool, optional):
+            - dictionary of non-default K-point setting. see pydmclab.hpc.vasp for format
+            - modifies only the "static" calculations
+
+
+        modify_loose_potcar (bool, optional):
+            - dictionary of non-default POTCAR in format {element (str) : POTCAR to use (str)}
+            - modifies only the "loose" calculations
+        modify_relax_potcar (bool, optional):
+            - dictionary of non-default POTCAR in format {element (str) : POTCAR to use (str)}
+            - modifies only the "loose" calculations
+        modify_static_potcar (bool, optional):
+            - dictionary of non-default POTCAR in format {element (str) : POTCAR to use (str)}
+            - modifies only the "static" calculations
+
+    Returns:
+        dictionary of VASP_CONFIGS
+    """
+    vasp_configs = {"lobster_static": run_lobster}
+
+    if modify_loose_incar:
+        vasp_configs["loose_incar"] = modify_loose_incar
+    if modify_relax_incar:
+        vasp_configs["relax_incar"] = modify_relax_incar
+    if modify_static_incar:
+        vasp_configs["static_incar"] = modify_static_incar
+
+    if modify_loose_kpoints:
+        vasp_configs["loose_kpoints"] = modify_loose_kpoints
+    if modify_relax_kpoints:
+        vasp_configs["relax_kpoints"] = modify_relax_kpoints
+    if modify_static_kpoints:
+        vasp_configs["static_kpoints"] = modify_static_kpoints
+
+    if modify_loose_potcar:
+        vasp_configs["loose_potcar"] = modify_loose_potcar
+    if modify_relax_potcar:
+        vasp_configs["relax_potcar"] = modify_relax_potcar
+    if modify_static_potcar:
+        vasp_configs["static_potcar"] = modify_static_potcar
+
+    return vasp_configs
+
+
+def get_slurm_configs(
+    total_nodes=1,
+    cores_per_node=8,
+    walltime_in_hours=95,
+    mem_per_core="all",
+    partition="agsmall,msidmc",
+    error_file="log.e",
+    output_file="log.o",
+    account="cbartel",
+):
+    """
+
+    how to modify slurm configurations for each VASP job (see pydmclab.data.data._slurm_configs.yaml for defaults)
+
+    Args:
+        total_nodes (int, optional):
+            how many nodes to run each VASP job on
+
+        cores_per_node (int, optional):
+            how many cores per node to use for each VASP job
+
+        walltime_in_hours (int, optional):
+            how long to run each VASP job
+
+        mem_per_core (str, optional):
+            if 'all', try to use all avaiable mem; otherwise use specified memory per core (cpu)
+
+        partition (str, optional):
+            what part of the cluster to run each VASP job on
+
+        error_file (str, optional):
+            where to send each VASP job error
+
+        output_file (str, optional):
+            where to send each VASP job output
+
+        account (str, optional):
+            what account to charge for your VASP jobs
+
+    Returns:
+        {slurm config name : slurm config value}
+    """
+    slurm_configs = {}
+
+    slurm_configs["nodes"] = total_nodes
+    slurm_configs["ntasks"] = int(total_nodes * cores_per_node)
+
+    if account == "cbartel":
+        slurm_configs["time"] = int(walltime_in_hours * 60)
+
+    if total_nodes > 1:
+        if "small" in partition:
+            print("WARNING: cant use small partition on > 1 node; switching to large")
+        partition = partition.replace("small", "large")
+
+    slurm_configs["partition"] = partition
+
+    slurm_configs["error_file"] = error_file
+    slurm_configs["output_file"] = output_file
+    slurm_configs["account"] = account
+
+    if total_nodes > 4:
+        print("WARNING: are you sure you need more than 4 nodes??")
+
+    if (total_nodes > 1) and (cores_per_node < 32):
+        print("WARNING: this seems like a small job. are you sure you need > 1 node??")
+
+    if mem_per_core == "all":
+        if partition in [
+            "msismall",
+            "small",
+            "msilarge",
+            "large",
+            "amdsmall",
+            "amdlarge",
+            "RM-small",
+            "RM",
+        ]:
+            mem_per_cpu = 1900
+        elif partition in ["agsmall", "msidmc", "aglarge", "agsmall,msidmd", "RM-512"]:
+            mem_per_cpu = 4000
+        else:
+            mem_per_cpu = 1900
+    else:
+        mem_per_cpu = mem_per_core
+
+    slurm_configs["mem"] = str(int(mem_per_cpu * slurm_configs["ntasks"])) + "M"
+    return slurm_configs
+
+
+def get_sub_configs(
+    machine="msi",
+    submit_calculations_in_parallel=False,
+    delete_all_calculations_and_start_over=False,
+    rerun_lobster=False,
+    mpi_command="mpirun",
+    special_packing=False,
+):
+    """
 
-"""
-see [pydmclab docs](https://github.umn.edu/bartel-group/pydmclab/blob/main/docs.md) for help
-"""
+    configs related to preparing submission scripts and submitting VASP calculations
+        - see defaults in pydmclab.data.data._sub_configs.yaml
 
-# where is this file
-SCRIPTS_DIR = os.getcwd()
+    Args:
+        submit_calculations_in_parallel (bool or int): whether to prepare submission scripts in parallel or not
+            - False: use 1 processor
+            - True: use all available processors
+            - int: use that many processors
+
+        delete_all_calculations_and_start_over (bool):
+            if True, start all calculations over (ie delete all outputs)
+
+        rerun_lobster (bool) :
+            if True, rerun lobster even if it has already been run
+
+        mpi_command (str):
+            the command to use for mpi (eg mpirun, srun, etc)
+
+        special_packing (dict):
+            if you want to change the loose --> relax --> static flow for some functional
+                e.g., {'metagga' : ['loose', 'static']}
+
+    Returns:
+        {config_name : config_value}
+
+    """
+    sub_configs = {}
+
+    if not submit_calculations_in_parallel:
+        n_procs = 1
+    else:
+        if submit_calculations_in_parallel == True:
+            n_procs = multip.cpu_count() - 1
+        elif submit_calculations_in_parallel == False:
+            n_procs = 1
+        else:
+            n_procs = submit_calculations_in_parallel
 
-# where are my calculations going to live
-CALCS_DIR = SCRIPTS_DIR.replace("scripts", "calcs")
+    sub_configs["n_procs"] = n_procs
 
-# where is my data going to live
-DATA_DIR = SCRIPTS_DIR.replace("scripts", "data")
+    if delete_all_calculations_and_start_over:
+        sub_configs["fresh_restart"] = True
 
-for d in [CALCS_DIR, DATA_DIR]:
-    if not os.path.exists(d):
-        os.makedirs(d)
+    if rerun_lobster:
+        sub_configs["force_postprocess"] = True
 
-# if you need data from MP as a starting point (often the case), you need your API key
-API_KEY = "__YOUR API KEY__"
+    sub_configs["mpi_command"] = mpi_command
 
-# lets put a tag on all the files we save
-FILE_TAG = CALCS_DIR.split("/")[-2]
+    if special_packing:
+        sub_configs["packing"] = {}
+        for xc in special_packing:
+            sub_configs["packing"]["xc"] = special_packing[xc]
 
-# what to query MP for
-## e.g., 'MnO2', ['MnO2', 'TiO2'], 'Ca-Ti-O, etc
-COMPOSITIONS = None
+    sub_configs["machine"] = machine
 
-# how to transform MP structures
-## e.g., [x/8 for x in range(9)]
-## NOTE: you need to modify get_strucs to make this work (hard to generalize)
-TRANSFORM_STRUCS = False
+    return sub_configs
 
-# any configurations related to LaunchTools
-## e.g., {'compare_to_mp' : True, 'n_afm_configs' : 4}
-LAUNCH_CONFIGS = get_launch_configs(
+
+def get_launch_configs(
     standards=["dmc"],
     xcs=["metagga"],
     use_mp_thermo_data=False,
     n_afm_configs=0,
     skip_xcs_for_standards={"mp": ["gga", "metagga"]},
-)
+):
+    """
 
-# any configurations related to SubmitTools
-## usually no need to change anything but n_procs... n_procs will determine how to parallelize over launch_dirs
-## NOTE: do not set n_procs = 'all' unless you are running on a compute node (ie not a login node)
-SUB_CONFIGS = get_sub_configs(
-    submit_calculations_in_parallel=False,
-    start_all_calculations_from_scratch=False,
-    rerun_lobster=False,
-    mpi_command="mpirun",
-    special_packing=False,
-)
+    configs related to launching  chains of calculations
 
-# any configurations related to Slurm
-## e.g., {'ntasks' : 16, 'time' : int(24*60)}
-SLURM_CONFIGS = get_slurm_configs(
-    total_nodes=1,
-    cores_per_node=32,
-    walltime_in_hours=23,
-    partition="msismall",
-    error_file="log.e",
-    output_file="log.o",
-    account="cbartel",
-)
+    Args:
+        standards (list, optional):
+            list of standards you'd like to calculate
 
-# any configurations related to VASPSetUp
-## e.g., {'lobster_static' : True, 'relax_incar' : {'ENCUT' : 555}}
-VASP_CONFIGS = get_vasp_configs(
-    run_lobster=False,
-    modify_loose_incar=False,
-    modify_relax_incar=False,
-    modify_static_incar=False,
-    modify_loose_kpoints=False,
-    modify_relax_kpoints=False,
-    modify_static_kpoints=False,
-    modify_loose_potcar=False,
-    modify_relax_potcar=False,
-    modify_static_potcar=False,
-)
+        xcs (list, optional):
+            list of xcs you'd like to calculate for each standard
+
+        use_mp_thermo_data (bool, optional):
+            True if you are going to use formation energies provided in Materials Project for phase stability analysis
+
+        n_afm_configs (int, optional):
+            number of antiferromagnetic configurations to run for each structure (0 if you don't want to run AFM)
+
+        skip_xcs_for_standards (dict, optional):
+            dictionary of xcs to skip for a given standard.
+                Defaults to {"mp": ["gga", "metagga"]}.
+                    - e.g., we don't want to run GGA or MetaGGA MP calculations because MP uses GGA+U (for now)
 
-# any configurations related to AnalyzeBatch
-## e.g., {'include_meta' : True, 'include_mag' : True, 'n_procs' : 4}
-## NOTE: do not set n_procs = 'all' unless you are running on a compute node (ie not a login node)
-ANALYSIS_CONFIGS = get_analysis_configs(
+    Returns:
+        dictionary of launch configurations
+    """
+
+    launch_configs = {}
+
+    to_launch = {}
+
+    for standard in standards:
+        to_launch[standard] = xcs
+
+    if use_mp_thermo_data:
+        to_launch["mp"] = ["ggau"]
+
+    for standard in skip_xcs_for_standards:
+        if standard not in to_launch:
+            continue
+        for xc in skip_xcs_for_standards[standard]:
+            if xc in to_launch[standard]:
+                to_launch[standard].remove(xc)
+
+    launch_configs["to_launch"] = to_launch
+
+    launch_configs["compare_to_mp"] = use_mp_thermo_data
+
+    launch_configs["n_afm_configs"] = n_afm_configs
+
+    return launch_configs
+
+
+def get_analysis_configs(
     analyze_calculations_in_parallel=False,
     analyze_structure=True,
     analyze_mag=False,
     analyze_charge=False,
     analyze_dos=False,
     analyze_bonding=False,
     exclude=[],
-)
+):
+    """
+
+    function for modifying analysis configs from the defaults (see pydmclab.data.data._batch_analysis_configs.yaml for defaults)
+
+    Args:
+        analyze_calculations_in_parallel (bool or int): whether to analyze calculation results in parallel or not
+            - False: use 1 processor
+            - True: use all available processors
+            - int: use that many processors
+
+        analyze_structure (bool, optional):
+            True to include structure in your results
+
+        analyze_mag (bool, optional):
+            True to include magnetization in your results
+
+        analyze_charge (bool, optional):
+            True to include bader charge + lobster charges + madelung in your results
+
+        analyze_dos (bool, optional):
+            True to include pdos, tdos in your results
+
+        analyze_bonding (bool, optional):
+            True to include tcohp, pcohp, tcoop, pcoop, tcobi, pcobi in your results
+
+        exclude (list, optional):
+            list of strings to exclude from analysis. Defaults to [].
+                - overwrites other options
+    Returns:
+        dictionary of ANALYSIS_CONFIGS
+            {'include_*' : True or False}
+    """
+
+    analysis_configs = {}
+
+    if not analyze_calculations_in_parallel:
+        n_procs = 1
+    else:
+        if analyze_calculations_in_parallel == True:
+            n_procs = multip.cpu_count() - 1
+        elif analyze_calculations_in_parallel == False:
+            n_procs = 1
+        else:
+            n_procs = analyze_calculations_in_parallel
 
-# whether or not you want to generate MAGMOMs
-## True if you're running AFM, else False
-GEN_MAGMOMS = True if LAUNCH_CONFIGS["n_afm_configs"] else False
-
-"""
-Don't forget to inspect the arguments to:
-    get_query
-    get_strucs
-    get_magmoms
-    get_launch_dirs
-    submit_calcs
-    get_results
+    analysis_configs["n_procs"] = n_procs
 
-You'll want to customize these depending on your calculations
-"""
+    includes = []
+    if analyze_structure:
+        includes.append("structure")
+
+    if analyze_mag:
+        includes.append("mag")
+
+    if analyze_charge:
+        includes.extend(["charge", "madelung"])
+
+    if analyze_dos:
+        includes.extend(["tdos", "pdos"])
+
+    if analyze_bonding:
+        includes.extend(["tcohp", "pcohp", "tcoop", "pcoop", "tcobi", "pcobi"])
+
+    for include in includes:
+        analysis_configs["include_" + include] = True
+
+    if exclude:
+        for ex in exclude:
+            analysis_configs["include_" + ex] = False
+
+    return analysis_configs
 
 
 def get_query(
     comp,
+    api_key,
     properties=None,
     criteria=None,
     only_gs=True,
     include_structure=True,
     supercell_structure=False,
     max_Ehull=0.05,
     max_sites_per_structure=65,
     max_strucs_per_cmpd=4,
-    savename="query_%s.json" % FILE_TAG,
+    data_dir=os.getcwd().replace("scripts", "data"),
+    savename="query.json",
     remake=False,
 ):
     """
     Args:
         comp (list or str)
             can either be:
                 - a chemical system (str) of elements joined by "-"
                 - a chemical formula (str)
             can either be a list of:
                 - chemical systems (str) of elements joined by "-"
                 - chemical formulas (str)
 
+        api_key (str):
+            your API key for Materials Project
+
         properties (list or None)
             list of properties to query
                 - if None, then use typical_properties
                 - if 'all', then use supported_properties
 
         criteria (dict or None)
             dictionary of criteria to query
@@ -175,28 +442,34 @@
 
         max_sites_per_structure (int)
             if not None, remove entries with more than max_sites_per_structure sites
 
         max_strucs_per_cmpd (int)
             if not None, only retain the lowest energy structures for each composition until you reach max_strucs_per_cmpd
 
-        savename (str) - filename for fjson in DATA_DIR
+        data_dir (str)
+            directory to save fjson
 
-        remake (bool) - write (True) or just read (False) fjson
+        savename (str)
+            filename for fjson in data_dir
+
+        remake (bool)
+            write (True) or just read (False) fjson
 
     Returns:
-        {mpid : {DATA}}
+        {ID (str) : {'structure' : Pymatgen Structure as dict,
+                    < any other data you want to keep track of >}}
     """
 
-    fjson = os.path.join(DATA_DIR, savename)
+    fjson = os.path.join(data_dir, savename)
     if os.path.exists(fjson) and not remake:
         return read_json(fjson)
 
     # initialize MPQuery with your API key
-    mpq = MPQuery(api_key=API_KEY)
+    mpq = MPQuery(api_key=api_key)
 
     # get the data from MP
     data = mpq.get_data_for_comp(
         comp=comp,
         properties=properties,
         criteria=criteria,
         only_gs=only_gs,
@@ -216,82 +489,50 @@
         print("\nmpid: %s" % mpid)
         print("\tcmpd: %s" % query[mpid]["cmpd"])
         print("\tstructure formula: %s" % StrucTools(query[mpid]["structure"]).formula)
 
 
 def get_strucs(
     query,
-    transform_strucs,
-    max_strucs_per_starting_struc=1,
-    ox_states=None,
-    savename="strucs_%s.json" % FILE_TAG,
+    data_dir=os.getcwd().replace("scripts", "data"),
+    savename="strucs.json",
     remake=False,
 ):
     """
     Args:
-        query (dict) - {mpid : {DATA}}
-        transform_strucs (bool or list):
-            - if False, just use the structures from MP
-            - if not False:
-                - this should be customized to perform whatever transformations you'd like to perform
-                - *NOTE*: you should also customize species_mapping in this function
-        max_strucs_per_starting_struc (int) - max number of structures to keep for each starting structure
-        ox_states (dict) - {element : oxidation state} for transformations
-            - if None, use AutoOxidationState algo in pymatgen
-        savename (str) - filename for fjson in DATA_DIR
-        remake (bool) - write (True) or just read (False) fjson
-
-    Returns:
-        if not transform_strucs:
-            {formula : {mpid : structure}
-        if transform_strucs:
-            {formula_identifier : {index_identifier : structure}}
+        query (dict)
+            {mpid : {DATA}}
+
+        data_dir (str)
+            directory to save fjson
+
+        savename (str)
+            filename for fjson in DATA_DIR
+
+        remake (bool)
+            write (True) or just read (False) fjson
+
+    Returns:
+        {formula identifier (str) :
+            {structure identifier for that formula (str) :
+                Pymatgen Structure object as dict}}
     """
 
-    fjson = os.path.join(DATA_DIR, savename)
+    fjson = os.path.join(data_dir, savename)
     if os.path.exists(fjson) and not remake:
         return read_json(fjson)
 
     # get all unique chemical formulas in the query
     formulas_in_query = sorted(list(set([query[mpid]["cmpd"] for mpid in query])))
 
     data = {}
     for formula in formulas_in_query:
         # get all MP IDs in your query having that formula
         mpids = [mpid for mpid in query if query[mpid]["cmpd"] == formula]
-        if not transform_strucs:
-            # if no transformations, just return the structures from MP
-            data[formula] = {mpid: query[mpid]["structure"] for mpid in mpids}
-        else:
-            # now you need to customize this for whatever transformations you want
-            if len(mpids) > 1:
-                print("WARNING: %s has %i mpids" % (formula, len(mpids)))
-                raise NotImplementedError(
-                    "folder structure is not super amenable to this... Reconfiguring recommended"
-                )
-
-            # take our 1 MP ID of interest and transform it
-            mpid = mpids[0]
-            initial_structure = query[mpid]["structure"]
-            for x in transform_strucs:
-                # make a new "formula" that includes are iterator in the transformation
-                key = "_".join([formula, str(x)])
-                structools = StrucTools(
-                    structure=initial_structure, ox_states=ox_states
-                )
-
-                species_mapping = None  # *NOTE*: you should customize this for your desired transformation
-
-                # strucs will have the form {index_identifier : structure}
-                strucs = structools.replace_species(
-                    species_mapping=species_mapping,
-                    n_strucs=max_strucs_per_starting_struc,
-                )
-
-                data[key] = strucs
+        data[formula] = {mpid: query[mpid]["structure"] for mpid in mpids}
 
     write_json(data, fjson)
     return read_json(fjson)
 
 
 def check_strucs(strucs):
     for formula in strucs:
@@ -302,30 +543,45 @@
             print("\tstructure formula: %s" % StrucTools(struc).formula)
 
 
 def get_magmoms(
     strucs,
     max_afm_combos=50,
     treat_as_nm=[],
-    savename="magmoms_%s.json" % FILE_TAG,
+    data_dir=os.getcwd().replace("scripts", "data"),
+    savename="magmoms.json",
     remake=False,
 ):
     """
     Args:
-        strucs (dict) - {formula : {ID : structure}}
-        max_afm_combos (int): maximum number of AFM spin configurations to generate
-        treat_as_nm (list): any normally mag els you'd like to treat as nonmagnetic for AFM enumeration
-        savename (str) - filename for fjson in DATA_DIR
-        remake (bool) - write (True) or just read (False) fjson
+        strucs (dict)
+            {formula : {ID : structure}}
+
+        max_afm_combos (int)
+            maximum number of AFM spin configurations to generate
+
+        treat_as_nm (list)
+            any normally mag els you'd like to treat as nonmagnetic for AFM enumeration
+
+        data_dir (str)
+            directory to save fjson
+
+        savename (str)
+            filename for fjson in data_dir
+
+        remake (bool)
+            write (True) or just read (False) fjson
 
     Returns:
-        {formula : {ID : {AFM configuration index : [list of magmoms on each site]}
-    """
+        {formula identifier (str) :
+            {structure identifier for that formula (str) :
+                {AFM ordering identifier (str) :
+                    [list of magmoms (floats) for each site in the structure]}}}"""
 
-    fjson = os.path.join(DATA_DIR, savename)
+    fjson = os.path.join(data_dir, savename)
     if not remake and os.path.exists(fjson):
         return read_json(fjson)
 
     magmoms = {}
     for formula in strucs:
         magmoms[formula] = {}
         for ID in strucs[formula]:
@@ -353,36 +609,58 @@
 
 def get_launch_dirs(
     strucs,
     magmoms,
     user_configs,
     make_launch_dirs=True,
     refresh_configs=True,
-    savename="launch_dirs_%s.json" % FILE_TAG,
+    data_dir=os.getcwd().replace("scripts", "data"),
+    calcs_dir=os.getcwd().replace("scripts", "calcs"),
+    savename="launch_dirs.json",
     remake=False,
 ):
     """
     Args:
-        strucs (dict) - {formula : {ID : structure}}
-        magmoms (dict) - {formula : {ID : {AFM configuration index : [list of magmoms on each site]}}
-        user_configs (dict) - optional launch configurations
-        make_launch_dirs (bool) - make launch directories (True) or just return launch dict (False)
-        refresh_configs (bool) - refresh configs (True) or just use existing configs (False)
-        savename (str) - filename for fjson in DATA_DIR
-        remake (bool) - write (True) or just read (False) fjson
+        strucs (dict)
+            {formula : {ID : structure}}
+
+        magmoms (dict)
+            {formula : {ID : {AFM configuration index : [list of magmoms on each site]}}
+
+        user_configs (dict)
+            optional launch configurations
+
+        make_launch_dirs (bool)
+            make launch directories (True) or just return launch dict (False)
+
+        refresh_configs (bool)
+            refresh configs (True) or just use existing configs (False)
+
+        data_dir (str)
+            directory to save fjson
+
+        calcs_dir (str)
+            directory above all your calculations
+
+        savename (str)
+            filename for fjson in data_dir
+
+        remake (bool)
+            write (True) or just read (False) fjson
 
     Returns:
-        {launch_dir (formula/ID/standard/mag) : {'xcs' : [list of final_xcs],
-                                                 'magmoms' : [list of magmoms for each site in structure in launch_dir]}}
+        {launch dir (str, formula/ID/standard/mag) :
+            {'xcs' : [list of final xcs to run (str)],
+            'magmoms' : [list of magmoms (floats) for each site in the structure]}}
 
         also makes launch_dir and populates with POSCAR using strucs if make_dirs=True
 
     """
 
-    fjson = os.path.join(DATA_DIR, savename)
+    fjson = os.path.join(data_dir, savename)
     if os.path.exists(fjson) and not remake:
         return read_json(fjson)
 
     all_launch_dirs = {}
     for formula in strucs:
         for ID in strucs[formula]:
             # for each unique structure, generate our launch directories
@@ -391,15 +669,15 @@
                 curr_magmoms = magmoms[formula][ID]
             else:
                 curr_magmoms = None
             top_level = formula
             unique_ID = ID
 
             launch = LaunchTools(
-                calcs_dir=CALCS_DIR,
+                calcs_dir=calcs_dir,
                 user_configs=user_configs,
                 magmoms=curr_magmoms,
                 structure=structure,
                 top_level=top_level,
                 unique_ID=unique_ID,
                 refresh_configs=refresh_configs,
             )
@@ -417,31 +695,35 @@
     print("\nanalyzing launch directories")
     for d in launch_dirs:
         print("\nlaunching from %s" % d)
         print("   these final xcs: %s" % launch_dirs[d]["xcs"])
 
 
 def submit_one_calc(submit_args):
-
     """
     Prepares VASP inputs, writes submission script, and launches job for one launch_dir
 
     Args:
         submit_args (dict) should contain:
-        {'launch_dir' :
-            launch_dir (str) - (formula/ID/standard/mag) to write and launch submission script in,
-         'launch_dirs' :
-            launch_dirs (dict) - {launch_dir (formula/ID/standard/mag) : {'xcs' : [list of final_xcs], 'magmoms' : [list of magmoms for each site in structure in launch_dir]}},
-         'user_configs' :
-            user_configs (dict) - optional sub, slurm, or VASP configurations,
-         'refresh_configs' :
-            refresh_configs (list) - list of which configs to refresh,
-         'ready_to_launch':
-            ready_to_launch (bool) - write (True) and launch (True) or just write (False) submission scripts (False)
-            }
+            {'launch_dir' :
+                launch_dir (str)
+                    (formula/ID/standard/mag) to write and launch submission script in,
+            'launch_dirs' :
+                launch_dirs (dict)
+                    {launch_dir (formula/ID/standard/mag) : {'xcs' : [list of final_xcs], 'magmoms' : [list of magmoms for each site in structure in launch_dir]}},
+            'user_configs' :
+                user_configs (dict)
+                    optional sub, slurm, or VASP configurations,
+            'refresh_configs' :
+                refresh_configs (list)
+                    list of which configs to refresh,
+            'ready_to_launch':
+                ready_to_launch (bool)
+                    write and launch (True) or just write submission scripts (False)
+                }
 
     Returns:
         None
 
     """
     launch_dir = submit_args["launch_dir"]
     launch_dirs = submit_args["launch_dirs"]
@@ -486,18 +768,25 @@
     ready_to_launch=True,
     n_procs=1,
 ):
     """
     Prepares VASP inputs, writes submission script, and launches job for all launch_dirs
 
     Args:
-        launch_dirs (dict) - {launch_dir (formula/ID/standard/mag) : {'xcs' : [list of final_xcs], 'magmoms' : [list of magmoms for each site in structure in launch_dir]}}
-        user_configs (dict) - optional sub, slurm, or VASP configurations
-        refresh_configs (list) - list of which configs to refresh
-        ready_to_launch (bool) - write (True) and launch (True) or just write (False) submission scripts (False
+        launch_dirs (dict)
+            {launch_dir (formula/ID/standard/mag) : {'xcs' : [list of final_xcs], 'magmoms' : [list of magmoms for each site in structure in launch_dir]}}
+
+        user_configs (dict)
+            optional sub, slurm, or VASP configurations
+
+        refresh_configs (list)
+            list of which configs to refresh
+
+        ready_to_launch (bool)
+            write and launch (True) or just write submission scripts (False
 
     Returns:
         None
 
     """
 
     submit_args = {
@@ -545,45 +834,58 @@
     return
 
 
 def get_results(
     launch_dirs,
     user_configs,
     refresh_configs=True,
-    savename="results_%s.json" % FILE_TAG,
+    data_dir=os.getcwd().replace("scripts", "data"),
+    savename="results.json",
     remake=False,
 ):
     """
     Args:
-        launch_dirs (dict) - {launch_dir (formula/ID/standard/mag) : {'xcs' : [list of final_xcs], 'magmoms' : [list of magmoms for each site in structure in launch_dir]}}
-        user_configs (dict) - optional analysis configurations
-        refresh_configs (bool) - refresh configs (True) or just use existing configs (False)
-        savename (str) - filename for fjson in DATA_DIR
-        remake (bool) - write (True) or just read (False) fjson
+        launch_dirs (dict)
+            {launch_dir (formula/ID/standard/mag) : {'xcs' : [list of final_xcs], 'magmoms' : [list of magmoms for each site in structure in launch_dir]}}
+
+        user_configs (dict)
+            optional analysis configurations
+
+        refresh_configs (bool)
+            refresh configs (True) or just use existing configs (False)
+
+        data_dir (str)
+            directory to save fjson
+
+        savename (str)
+            filename for fjson in data_dir
+
+        remake (bool)
+            write (True) or just read (False) fjson
 
     Returns:
-        {'formula.ID.standard.mag.xc_calc' : {scraped results from VASP calculation}}
+        {formula--ID--standard--mag--xc-calc (str) :
+            {scraped results from VASP calculation}}
     """
 
-    fjson = os.path.join(DATA_DIR, savename)
+    fjson = os.path.join(data_dir, savename)
     if os.path.exists(fjson) and not remake:
         return read_json(fjson)
 
     analyzer = AnalyzeBatch(
         launch_dirs, user_configs=user_configs, refresh_configs=refresh_configs
     )
 
     data = analyzer.results
 
     write_json(data, fjson)
     return read_json(fjson)
 
 
 def check_results(results):
-
     keys_to_check = list(results.keys())
 
     converged = 0
     for key in keys_to_check:
         if "--" in key:
             delimiter = "--"
         else:
@@ -598,35 +900,58 @@
             # print("\n%s" % key)
             print("E (static) = %.2f" % data["results"]["E_per_at"])
 
     print("\n\n SUMMARY: %i/%i converged" % (converged, len(keys_to_check)))
 
 
 def get_gs(
-    results, include_structure=False, savename="gs_%s.json" % FILE_TAG, remake=False
+    results,
+    include_structure=False,
+    non_default_functional=None,
+    compute_Ef=True,
+    data_dir=os.getcwd().replace("scripts", "data"),
+    savename="gs.json",
+    remake=False,
 ):
     """
     Args:
-        results (dict) - {'formula.ID.standard.mag.xc_calc' : {scraped results from VASP calculation}}
-        include_structure (bool) - include the structure or not
-        savename (str) - filename for fjson in DATA_DIR
-        remake (bool) - write (True) or just read (False) fjson
+        results (dict)
+            {formula--ID--standard--mag--xc-calc (str) : {scraped results from VASP calculation}}
+
+        include_structure (bool)
+            include the structure or not
+
+        non_default_functional (str)
+            if you're not using r2SCAN or PBE
+
+        compute_Ef (bool)
+            if True, compute formation enthalpy
+
+        data_dir (str)
+            directory to save fjson
+
+        savename (str)
+            filename for fjson in data_dir
+
+        remake (bool)
+            write (True) or just read (False) fjson
 
     Returns:
     {standard (str, the calculation standard) :
         {xc (str, the exchange-correlation method) :
             {formula (str) :
                 {'E' : energy of the ground-structure,
                 'key' : formula.ID.standard.mag.xc_calc for the ground-state structure,
                 'structure' : structure of the ground-state structure,
                 'n_started' : how many polymorphs you tried to calculate,
                 'n_converged' : how many polymorphs are converged,
-                'complete' : True if n_converged = n_started (i.e., all structures for this formula at this xc are done)}
+                'complete' : True if n_converged = n_started (i.e., all structures for this formula at this xc are done),
+                'Ef' : formation enthalpy at 0 K}
     """
-    fjson = os.path.join(DATA_DIR, savename)
+    fjson = os.path.join(data_dir, savename)
     if os.path.exists(fjson) and not remake:
         return read_json(fjson)
 
     standards = sorted(
         list(set([results[key]["meta"]["setup"]["standard"] for key in results]))
     )
 
@@ -684,14 +1009,31 @@
                     "n_started": len(formula_keys),
                     "n_converged": len(converged_keys),
                     "complete": complete,
                 }
                 if include_structure:
                     gs[standard][xc][formula]["structure"] = gs_structure
 
+    if compute_Ef:
+        for standard in gs:
+            for xc in gs[standard]:
+                if not non_default_functional:
+                    functional = "r2scan" if xc == "metagga" else "pbe"
+                else:
+                    functional = non_default_functional
+                mus = ChemPots(functional=functional, standard=standard).chempots
+                for formula in gs[standard][xc]:
+                    E = gs[standard][xc][formula]["E"]
+                    if E:
+                        Ef = FormationEnthalpy(
+                            formula=formula, E_DFT=E, chempots=mus
+                        ).Ef
+                    else:
+                        Ef = None
+                    gs[standard][xc][formula]["Ef"] = Ef
     write_json(gs, fjson)
     return read_json(fjson)
 
 
 def check_gs(gs):
     """
     checks that this dictionary is generated properly
@@ -714,129 +1056,115 @@
             n_formulas_complete = len(
                 [k for k in formulas if gs[standard][xc][k]["complete"]]
             )
             print(
                 "%i/%i formulas with all calculations completed"
                 % (n_formulas_complete, n_formulas)
             )
+            for formula in gs[standard][xc]:
+                if "Ef" in gs[standard][xc][formula]:
+                    if gs[standard][xc][formula]["Ef"]:
+                        print(
+                            "%s : %.2f eV/at"
+                            % (formula, gs[standard][xc][formula]["Ef"])
+                        )
 
 
-def get_Efs(
-    gs, non_default_functional=None, savename="Efs_%s.json" % FILE_TAG, remake=False
+def get_thermo_results(
+    results,
+    gs,
+    data_dir=os.getcwd().replace("scripts", "data"),
+    savename="thermo_results.json",
+    remake=False,
 ):
     """
-    Args:
-        gs (dict) - {formula (str) : {basic stuff for ground-states}}
-        non_default_functional (str or None) - if None, use default functionals
-        savename (str) - filename for fjson in DATA_DIR
-        remake (bool) - write (True) or just read (False) fjson
-
-    Returns:
-    {xc (str, the exchange-correlation method) :}
-        {formula (str) :
-            {'E' : energy of the ground-structure,
-             'key' : formula.ID.standard.mag.xc_calc for the ground-state structure,
-             'structure' : structure of the ground-state structure,
-             'n_started' : how many polymorphs you tried to calculate,
-             'n_converged' : how many polymorphs are converged,
-             'complete' : True if n_converged = n_started (i.e., all structures for this formula at this xc are done),
-             'Ef' : formation enthalpy at 0 K (float)}
-    """
-    fjson = os.path.join(DATA_DIR, savename)
-    if os.path.exists(fjson) and not remake:
-        return read_json(fjson)
-    for standard in gs:
-        for xc in gs[standard]:
-            if not non_default_functional:
-                functional = "r2scan" if xc == "metagga" else "pbe"
-            else:
-                functional = non_default_functional
-            mus = ChemPots(functional=functional, standard=standard).chempots
-            for formula in gs[standard][xc]:
-                E = gs[standard][xc][formula]["E"]
-                if E:
-                    Ef = FormationEnthalpy(formula=formula, E_DFT=E, chempots=mus).Ef
-                else:
-                    Ef = None
-                gs[standard][xc][formula]["Ef"] = Ef
-
-    write_json(gs, fjson)
-    return read_json(fjson)
 
+    Args:
+        results (dict):
+            full results dictionary
 
-def check_Efs(Efs):
-    print("\nchecking formation enthalpies")
-
-    for standard in Efs:
-        print("\n\nworking on %s standard" % standard)
-        for xc in Efs[standard]:
-            print("\nxc = %s" % xc)
-            for formula in Efs[standard][xc]:
-                print("%s : %.2f eV/at" % (formula, Efs[standard][xc][formula]["Ef"]))
-    return
+        gs (dict):
+            dictionary of ground-state data
 
+        data_dir (str)
+            directory to save fjson
 
-def get_thermo_results(
-    results, Efs, savename="thermo_results_%s.json" % FILE_TAG, remake=False
-):
-    """
+        savename (str)
+            fjson name in data_dir
 
-    Args:
-        results (dict): full results dictionary
-        Efs (dict): dictionary of formation enthalpies
-        savename (str, optional): Defaults to "thermo_results_%s.json"%FILE_TAG.
-        remake (bool, optional): Defaults to False.
+        remake (bool)
+            Read (False) or write (True) json
 
     Returns:
         {standard (str) :
             {xc (str) :
                 {formula (str) :
-                    {'E' (float) : energy of the structure,
-                     'Ef' : formation enthalpy,
-                     'is_gs' : True if this is the lowest energy polymorph for this formula,
-                     'dE_gs' : how high above the ground-state this structure is in energy
-                     'all_polymorphs_converged' : True if every structure that was computed for this formula is converged}
+                    {ID (str) :
+                        {'E' : energy of the structure (DFT total energy in eV/atom),
+                        'Ef' : formation enthalpy at 0 K (eV/atom),
+                        'is_gs' : True if this is the lowest energy polymorph for this formula,
+                        'dE_gs' : how high above the ground-state this structure is in energy (eV/atom)
+                        'all_polymorphs_converged' : True if every structure that was computed for this formula is converged}}
     """
-    fjson = os.path.join(DATA_DIR, savename)
+    fjson = os.path.join(data_dir, savename)
     if os.path.exists(fjson) and not remake:
         return read_json(fjson)
 
     thermo_results = {
         standard: {
-            xc: {formula: {} for formula in Efs[standard][xc]} for xc in Efs[standard]
+            xc: {formula: {} for formula in gs[standard][xc]} for xc in gs[standard]
         }
-        for standard in Efs
+        for standard in gs
     }
 
     for key in results:
         tmp_thermo = {}
 
         standard = results[key]["meta"]["setup"]["standard"]
         xc = results[key]["meta"]["setup"]["xc"]
         formula = results[key]["results"]["formula"]
-        ID = results[key]["meta"]["setup"]["ID"]
+        ID = "__".join(
+            [
+                results[key]["meta"]["setup"]["formula_tag"],
+                results[key]["meta"]["setup"]["ID"],
+                results[key]["meta"]["setup"]["mag"],
+            ]
+        )
         E = results[key]["results"]["E_per_at"]
-
+        formula = results[key]["results"]["formula"]
+        structure = results[key]["structure"]
+        if structure:
+            calcd_formula = StrucTools(structure).formula
+        else:
+            calcd_formula = None
         tmp_thermo["E"] = E
         tmp_thermo["key"] = key
+        tmp_thermo["formula"] = formula
+        tmp_thermo["calculated_formula"] = calcd_formula
 
         if E:
-            gs_key = Efs[standard][xc][formula]["key"]
-            gs_Ef = Efs[standard][xc][formula]["Ef"]
-            gs_E = Efs[standard][xc][formula]["E"]
+            gs_key = gs[standard][xc][formula]["key"]
+            if "Ef" in gs[standard][xc][formula]:
+                gs_Ef = gs[standard][xc][formula]["Ef"]
+            else:
+                gs_Ef = None
+            gs_E = gs[standard][xc][formula]["E"]
             delta_E_gs = E - gs_E
 
             if key == gs_key:
                 tmp_thermo["is_gs"] = True
             else:
                 tmp_thermo["is_gs"] = False
 
             tmp_thermo["dE_gs"] = delta_E_gs
-            tmp_thermo["Ef"] = gs_Ef + delta_E_gs
-            tmp_thermo["all_polymorphs_converged"] = Efs[standard][xc][formula][
+            if gs_Ef:
+                tmp_thermo["Ef"] = gs_Ef + delta_E_gs
+            else:
+                tmp_thermo["Ef"] = None
+            tmp_thermo["all_polymorphs_converged"] = gs[standard][xc][formula][
                 "complete"
             ]
 
         else:
             tmp_thermo["dE_gs"] = None
             tmp_thermo["Ef"] = None
             tmp_thermo["is_gs"] = False
@@ -889,109 +1217,214 @@
             converged_formulas = list(set(converged_formulas))
             print(
                 "%i/%i formulas have all polymorphs converged"
                 % (len(converged_formulas), len(thermo[standard][xc].keys()))
             )
 
 
-def main():
-
-    remake_sub_for_launcher = False
-
-    remake_query = False
-    print_query_check = True
-
-    remake_strucs = False
-    print_strucs_check = True
-
-    remake_magmoms = False
-    print_magmoms_check = True
+def get_dos_results(
+    results,
+    thermo_results,
+    only_gs=True,
+    only_xc="metagga",
+    only_formulas=[],
+    only_standard="dmc",
+    dos_to_store=["tdos", "tcohp"],
+    regenerate_dos=False,
+    regenerate_cohp=False,
+    data_dir=os.getcwd().replace("scripts", "data"),
+    savename="dos_results.json",
+    remake=False,
+):
+    """
+    Args:
+        results (dict)
+            from get_results
 
-    remake_launch_dirs = False
-    print_launch_dirs_check = True
+        thermo_results (dict)
+            from get_thermo_results
 
-    remake_subs = True
-    ready_to_launch = True
+        only_gs (bool)
+            if True, only get DOS/COHP for the ground-state polymorphs
 
-    remake_results = True
-    print_results_check = True
+        only_xc (str)
+            if not None, only get DOS/COHP for this XC
 
-    remake_gs = True
-    print_gs_check = True
+        only_formulas (list)
+            if not None, only get DOS/COHP for these formulas
 
-    remake_Efs = True
-    print_Efs_check = True
+        only_standard (str)
+            if not None, only get DOS/COHP for this standard
 
-    remake_thermo_results = True
-    print_thermo_results_check = True
+        dos_to_store (list)
+            which DOS/COHP to store ['tcohp', 'pcohp', 'tdos', 'pdos', etc]
 
-    if remake_sub_for_launcher:
-        make_sub_for_launcher()
+        regenerate_dos (bool)
+            if True, make pdos/tdos jsons again even if it exists
 
-    comp = COMPOSITIONS
-    query = get_query(comp=comp, remake=remake_query)
-    if print_query_check:
-        check_query(query)
+        regenerate_cohp (bool)
+            if True, make pcohp/tcohp jsons again even if it exists
 
-    transform_strucs = TRANSFORM_STRUCS
-    strucs = get_strucs(
-        query=query, transform_strucs=transform_strucs, remake=remake_strucs
-    )
-    if print_strucs_check:
-        check_strucs(strucs)
+        data_dir (str)
+            path to data directory
 
-    if GEN_MAGMOMS:
-        magmoms = get_magmoms(strucs=strucs, remake=remake_magmoms)
-        if print_magmoms_check:
-            check_magmoms(strucs=strucs, magmoms=magmoms)
-    else:
-        magmoms = None
+        savename (str)
+            name of json file to save results to
 
-    launch_configs = LAUNCH_CONFIGS
-    launch_dirs = get_launch_dirs(
-        strucs=strucs,
-        magmoms=magmoms,
-        user_configs=launch_configs,
-        remake=remake_launch_dirs,
-    )
-    if print_launch_dirs_check:
-        check_launch_dirs(launch_dirs)
+        remake (bool)
+            if True, remake the json file
+    """
+    fjson = os.path.join(data_dir, savename)
+    if os.path.exists(fjson) and not remake:
+        return read_json(fjson)
 
-    sub_configs = SUB_CONFIGS
-    slurm_configs = SLURM_CONFIGS
-    vasp_configs = VASP_CONFIGS
-    user_sub_configs = {**sub_configs, **slurm_configs, **vasp_configs}
-    if remake_subs:
-        submit_calcs(
-            launch_dirs=launch_dirs,
-            user_configs=user_sub_configs,
-            ready_to_launch=ready_to_launch,
-            n_procs=sub_configs["n_procs"],
+    for key in results:
+        calc_dir = results[key]["meta"]["calc_dir"]
+        standard, xc = (
+            results[key]["meta"]["setup"]["standard"],
+            results[key]["meta"]["setup"]["xc"],
         )
+        ID = "__".join(
+            [
+                results[key]["meta"]["setup"]["formula_tag"],
+                results[key]["meta"]["setup"]["ID"],
+                results[key]["meta"]["setup"]["mag"],
+            ]
+        )
+        formula = results[key]["results"]["formula"]
+        thermo_result = thermo_results[standard][xc][formula][ID]
+        if only_gs:
+            if not thermo_result["is_gs"]:
+                continue
+        if only_formulas:
+            if thermo_result["formula"] not in only_formulas:
+                continue
+        if only_xc:
+            if xc != only_xc:
+                continue
+        if only_standard:
+            if standard != only_standard:
+                continue
+        av = AnalyzeVASP(calc_dir)
+        if "tdos" in dos_to_store:
+            pdos = av.pdos(remake=regenerate_dos)
+            tdos = av.tdos(pdos=pdos, remake=regenerate_dos)
+            thermo_results[standard][xc][formula][ID]["tdos"] = tdos
+        if "pdos" in dos_to_store:
+            thermo_results[standard][xc][formula][ID]["pdos"] = pdos
+        if "tcohp" in dos_to_store:
+            pcohp = av.pcohp(remake=regenerate_cohp)
+            tcohp = av.tcohp(pcohp=pcohp, remake=regenerate_cohp)
+            thermo_results[standard][xc][formula][ID]["tcohp"] = tcohp
+        if "pcohp" in dos_to_store:
+            thermo_results[standard][xc][formula][ID]["pcohp"] = pcohp
+        if "tcoop" in dos_to_store:
+            pcohp = av.pcohp(are_coops=True, remake=regenerate_cohp)
+            tcohp = av.tcohp(pcohp=pcohp, remake=regenerate_cohp)
+            thermo_results[standard][xc][formula][ID]["tcoop"] = tcohp
+        if "pcoop" in dos_to_store:
+            thermo_results[standard][xc][formula][ID]["pcoop"] = pcohp
+        if "tcobi" in dos_to_store:
+            pcohp = av.pcohp(are_cobis=True, remake=regenerate_cohp)
+            tcohp = av.tcohp(pcohp=pcohp, remake=regenerate_cohp)
+            thermo_results[standard][xc][formula][ID]["tcobi"] = tcohp
+        if "pcobi" in dos_to_store:
+            thermo_results[standard][xc][formula][ID]["pcobi"] = pcohp
 
-    analysis_configs = ANALYSIS_CONFIGS
-    results = get_results(
-        launch_dirs=launch_dirs, user_configs=analysis_configs, remake=remake_results
-    )
-    if print_results_check:
-        check_results(results)
+    write_json(thermo_results, fjson)
+    return read_json(fjson)
 
-    gs = get_gs(results=results, remake=remake_gs)
 
-    if print_gs_check:
-        check_gs(gs)
+def crawl_and_purge(
+    head_dir,
+    files_to_purge=[
+        "WAVECAR",
+        "CHGCAR",
+        "CHG",
+        "PROCAR",
+        "LOCPOT",
+        "AECCAR0",
+        "AECCAR1",
+        "AECCAR2",
+    ],
+    safety="on",
+    check_convergence=True,
+    verbose=False,
+):
+    """
+    Args:
+        head_dir (str)
+            directory to start crawling beneath
 
-    Efs = get_Efs(gs=gs, remake=remake_Efs)
+        files_to_purge (list)
+            list of file names to purge
 
-    if print_Efs_check:
-        check_Efs(Efs)
+        safety (str)
+            'on' or 'off' to turn on/off safety
+                - if safety is on, won't actually delete files
+    """
+    purged_files = []
+    mem_created = 0
+    for subdir, dirs, files in os.walk(head_dir):
+        ready = False
+        if check_convergence:
+            if "POTCAR" in files:
+                av = AnalyzeVASP(subdir)
+                if av.is_converged:
+                    ready = True
+                else:
+                    ready = False
+            else:
+                ready = False
+        else:
+            ready = True
+        if ready:
+            for f in files:
+                if f in files_to_purge:
+                    path_to_f = os.path.join(subdir, f)
+                    if verbose:
+                        print(path_to_f)
+                    mem_created += os.stat(path_to_f).st_size
+                    purged_files.append(path_to_f)
+                    if safety == "off":
+                        os.remove(path_to_f)
+    if safety == "off":
+        print(
+            "You purged %i files, freeing up %.2f GB of memory"
+            % (len(purged_files), mem_created / 1e9)
+        )
+    if safety == "on":
+        print(
+            "You had the safety on\n If it were off, you would have purged %i files, freeing up %.2f GB of memory"
+            % (len(purged_files), mem_created / 1e9)
+        )
 
-    thermo = get_thermo_results(results=results, Efs=Efs, remake=remake_thermo_results)
 
-    if print_thermo_results_check:
-        check_thermo_results(thermo)
+def make_sub_for_launcher():
+    """
+    Creates sub_launcher.sh file to launch launcher on compute node
+    """
+    flauncher_sub = os.path.join(os.getcwd(), "sub_launcher.sh")
+    launch_job_name = "-".join([os.getcwd().split("/")[-2], "launcher"])
+    with open(flauncher_sub, "w") as f:
+        f.write("#!/bin/bash -l\n")
+        f.write("#SBATCH --nodes=1\n")
+        f.write("#SBATCH --ntasks=8\n")
+        f.write("#SBATCH --time=4:00:00\n")
+        f.write("#SBATCH --mem=8G\n")
+        f.write("#SBATCH --error=_log_launcher.e\n")
+        f.write("#SBATCH --output=_log_launcher.o\n")
+        f.write("#SBATCH --account=cbartel\n")
+        f.write("#SBATCH --job-name=%s\n" % launch_job_name)
+        f.write("#SBATCH --partition=msismall\n")
+        f.write("\npython launcher.py\n")
 
-    return
+
+def main():
+    mus = ChemPots(functional="r2scan", standard="dmc").chempots
+    for el in mus:
+        if not mus[el]:
+            print(el)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pydmclab-1.0.0/pydmclab/demos/demo_struc.py` & `pydmclab-1.0.1/pydmclab/demos/demo_struc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,96 +1,134 @@
 from pydmclab.core.struc import StrucTools, SiteTools
 from pydmclab.core.query import MPQuery
 
 from pymatgen.core.structure import Structure
 
+
+""" 
+Purpose: 
+  StrucTools is used to perform manipulations to crystal structures
+  SiteTools helps you do this by extracting information for individual sites in a structure
+  
+Unit tests:
+  - see pydmclab/tests/test_struc.py
+
+"""
+
 MPID = "mp-19417"
 API_KEY = "N3KdATtMmcsUL94g"
 
 
 def demo_basic_structure_manipulations(mpid=MPID):
-    print("\n")
+    """
+    - get the structure formula
+    - reduce that formula (get the clean version)
+    - get the elements in the structure
+    - count the number of sites
+    - make a supercell
+    """
+
+    print("\n ~~ demoing basic manipulations ~~ \n")
 
     s = MPQuery(API_KEY).get_structure_by_material_id(mpid)
     st = StrucTools(s)
 
     print("\nformula = %s" % st.formula)
     print("compact formula = %s" % st.compact_formula)
     print("structure has %s" % st.els)
     print("downloaded structure has %i sites" % len(st.structure))
     st.make_supercell([1, 2, 3])
     print("supercell has %i sites" % len(st.structure))
 
 
 def demo_ox_state_decoration(mpid=MPID):
-    print("\n")
+    """
+    - decorate w/ oxidation states using pymatgen's automatic algorithm
+    - decorate w/ user-specified oxidation states
+    - inspect the oxidation state using SiteTools.ion
+    """
+    print("\n ~~ demoing oxidation state decoration ~~ \n")
     s = MPQuery(API_KEY).get_structure_by_material_id(mpid)
     st = StrucTools(s)
 
     site = SiteTools(s, 0)
     print("from MP, site 0 is %s" % site.ion)
 
     s = st.decorate_with_ox_states
 
-    print("after auto oxi state decoration, site 10 is %s" % SiteTools(s, 10).ion)
+    print("after auto oxi state decoration, site 0 is %s" % SiteTools(s, 0).ion)
 
-    st = StrucTools(s, ox_states={"Fe": 2, "Ti": 4, "O": -2})
+    st = StrucTools(s, ox_states={"Fe": 3, "Ti": 3, "O": -2})
 
     s = st.decorate_with_ox_states
 
     print(
-        "after forcing Fe to be ox state = 2 (bad idea)!, site 10 is %s"
-        % SiteTools(s, 10).ion
+        "after forcing Fe and Ti to be ox state = 3, site 0 is %s" % SiteTools(s, 0).ion
     )
 
-    print(s[0].species)
-
 
 def demo_replace_species_and_order(mpid=MPID):
-    print("\n")
+    """
+    - make a supercell
+    - replace a fullly occupied site with a mixed occupancy site
+    - generate ordered versions of this mixed occupancy structure
+    - inspect some sites in one of the ordered structures
+    """
+    print("\n ~~ demoing replace species ~~ \n")
     s = MPQuery(API_KEY).get_structure_by_material_id(mpid)
     st = StrucTools(s)
     st.make_supercell([1, 2, 3])
 
     species_map = {"Fe": {"Fe": 0.875, "Cr": 0.125}}
 
     ordered_strucs = st.replace_species(species_map, n_strucs=10)
 
     print("generated %i structures" % len(ordered_strucs))
 
-    for idx in ordered_strucs:
-        s = Structure.from_dict(ordered_strucs[idx])
-        print("\nstructure %i has formula %s" % (idx, StrucTools(s).formula))
-        site = SiteTools(s, 12)
-        print(
-            "site 13 has ion = %s, coords = %s with ox state = %s"
-            % (site.ion, site.coords, site.ox_state)
-        )
+    struc_idx = 3
+    struc = ordered_strucs[struc_idx]
+    print("\nstructure %i has formula %s" % (struc_idx, StrucTools(struc).formula))
+    site_idx = 12
+    site = SiteTools(struc, site_idx)
+    print(
+        "site %i has el = %s, coords = %s with ox state = %s"
+        % (site_idx, site.el, site.coords, site.ox_state)
+    )
 
 
 def demo_dilute_vacancy(mpid=MPID):
     """
-    Broken right now...
+    - change the occupancy of an element from 1 (fully occupied) to some value that leads to 1 vacancy
+
     """
-    print("\n")
+    print("\n ~~ demoing dilute vacancy ~~ \n")
     s = MPQuery(API_KEY).get_structure_by_material_id(mpid)
     st = StrucTools(s)
 
-    out = st.get_structures_with_dilute_vacancy(
-        el_to_replace="O", n_strucs=10, structure=None
+    print("initial formula = ", st.formula)
+
+    el_to_remove = "O"
+    n_el_in_struc = st.amts["O"]
+    n_el_to_remove = 1
+    new_occ = (n_el_in_struc - n_el_to_remove) / n_el_in_struc
+
+    s_with_vac = st.change_occ_for_el(
+        el_to_remove, {el_to_remove: new_occ}, structure=None
     )
 
-    struc = Structure.from_dict(out[0])
+    ordered_strucs = StrucTools(
+        s_with_vac, ox_states={"O": -2, "Fe": 3, "Ti": 3}
+    ).get_ordered_structures(n_strucs=10)
 
-    print(struc)
+    print("final formula = ", StrucTools(ordered_strucs[0]).formula)
 
 
 def main():
     demo_basic_structure_manipulations()
     demo_ox_state_decoration(mpid=MPID)
     demo_replace_species_and_order(mpid=MPID)
-    # demo_dilute_vacancy(mpid=MPID)
+    demo_dilute_vacancy(mpid=MPID)
     return
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pydmclab-1.0.0/pydmclab/demos/demo_vasp_test-typical-dmc.py` & `pydmclab-1.0.1/pydmclab/hpc/vasp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,796 +1,675 @@
-import os
-import numpy as np
-import multiprocessing as multip
-
-from pydmclab.utils.handy import read_json, write_json, make_sub_for_launcher
-from pydmclab.core.query import MPQuery
 from pydmclab.core.mag import MagTools
 from pydmclab.core.struc import StrucTools
-from pydmclab.hpc.launch import LaunchTools
-from pydmclab.hpc.submit import SubmitTools
-from pydmclab.hpc.analyze import AnalyzeBatch
-
-"""
-Basic framework
-
-Initial crystal structures
-    a) Sometimes these are entries in Materials Project meeting some criteria:
-        - e.g., certain chemical space, chemical formula, E above hull, etc
-    b) Other times, we might start with an MP structure then perform some transformations to generate new structures
-        - e.g., replace x % of Ru with Ir in Ru_{1-x}Ir_{x}O_2 or extract x Li from Li_{1-x}CoO_2
-            - note: now we are disordering structures, so each chemical formula will have >= 1 enumerated structure
-                - i.e., Ru_0.5Ir_0.5O_2 has > 1 way to configure Ru/Ir on the cation sublattice
-    
-    The first two levels of our caculation directories will correspond to information relating to the crystal structure:
-        - top_level: the chemical formula (or some surrogate for the chemical formula)
-            - e.g., this could be RuO2 in 1(a) or it could be x in 1(b)
-        - unique_ID: some unique identifier for a crystal structure belonging to that "top_level"
-            - e.g., the Materials Project ID for the 1(a) case; or the index of 
-        
-    Each unique initial crytsal structure will be used for all directories below top_level/unique_ID
-    
-    Example tree #1:
-    calculating RuO2 and IrO2 ground-state polymorphs
-    -calcs
-     -RuO2
-      -mp-1234
-     -IrO2
-      -mp-5678
-      
-    Example tree #2:
-    calculating Ru_{2-x}Ir_{x}O4 for x = 0, 1, 2 for 2 ordered structures at each x
-    -calcs
-     -0
-      -0
-      -1
-     -1
-      -0
-      -1
-     -2
-      -0
-      -1
-         
-VASP input settings ("standard")
-
-    Usually we want to compute a group of structures with similar settings so that we can safely compare the resulting energies
-    
-    - right now, we have two standards:
-        - dmc: our group standard (to be evolved collectively)
-            - these are best practice settings for our group
-        - mp: settings to use for strict comparison to Materials Project data
-    - standards define the non-structure VASP input files (INCAR, KPOINTS, POTCAR)
-    
-    This will be the third level of our calculation directory: top_level/unique_ID/standard
-    
-    If we were calculating with dmc and mp standards, a part of the tree might look like:
-    
-    -calcs
-     -RuO2
-      -mp-1234
-       -dmc
-       -mp
-    
-Magnetic configuration (mag)
-
-    We need to define what initial magnetic configuration we want to calculate for each initial structure
-    - nm: non-magnetic (no spins)
-    - fm: ferromagnetic (all spins > 0)
-    - afm_*: antiferromagnetic (spins up and down with sum(spins) = 0)
-        - * is a unique identifier for the ordering of spins
-            - much like partially occupied / disordered structures have multiple ways to configure ions on the lattice,
-                - there are often many ways to configure spins on the lattice while still being AFM (sum(spins) = 0)
-        - if we want to do AFM calculations, we should first generate a "MAGMOM" (AFM ordering) file for each unique structure and save that data
-        - note: if we are computing AFM, we will also compute FM
-        
-    This will be the fourth level of our calculation directory: top_level/unique_ID/standard/mag
-    
-    -calcs
-     -RuO2
-      -mp-1234
-       -dmc
-        -afm_0
-
-        
-Exchange-correlation functional (xc)
-
-Now, we need to decide what flavor of DFT we want to use. Materials Project uses GGA+U. We will often use METAGGA.
-
-For each xc that we use, it's generally a good idea to run calculations in a sequence:
-    - a "loose" calculation that has fast-converging standards but not super accurate
-    - a "relax" calculation that will optimize the crystal structure with stricter standards
-    - a "static" calculation that will give us a better energy/electronic structure at that optimized geometry
-    - for METAGGA calculations, we need to first converge a GGA calculation before we start to optimize the geometry with metagga
-    
-We don't want to have to submit each of these individually to the queue, so we will "pack" them together:
-
-    So, if we're running gga, that means three calculations will get packed together: gga-loose --> gga-relax --> gga-static
-        - if we're running metagga, we'll have 5 calcs: gga-loose --> gga-relax --> gga-static --> metagga-relax --> metagga-static
-        - each packing or chain of jobs will need a submission script (i.e., something that gets submitted to the queue)
-        
-Each one of these "xc-calcs" (e.g., gga-relax) will require a VASP execution, meaning it needs VASP inputs and will generate VASP outputs,
-    so each xc-calc gets its own directory, becoming the 5th level of our calculation directory:
-    
-    top_level/unique_ID/standard/mag/xc-calc
-    
-    -calcs
-     -RuO2
-      -mp-1234
-       -dmc
-        -afm_0
-         -gga-loose
-         -gga-relax
-         -gga-static
-
-"""
-
-"""
-Most of this is taken care of automatically in pydmc
+from pydmclab.hpc.analyze import AnalyzeVASP, VASPOutputs
+from pydmclab.data.configs import load_vasp_configs
+from pydmclab.utils.handy import read_yaml, write_yaml, dotdict
 
-1) Use MPQuery to get crystal structures from Materials Project
-    - write to a dictionary: query.json
-2) [OPTIONAL] Transform those structures to generate new structures using StrucTools
-    - write to a dictionary: strucs.json
-3) [OPTIONAL] Create AFM orderings ("magmoms") for each structure using MagTools(structure).get_afm_magmoms
-    - write to a dictionary: magmoms.json
-4) Create a dictionary of "launch directories" using LaunchTools
-    - customizable with various _launch_configs
-    - launch directories are the directories that hold submission scripts
-        - these launch directories are defined by the top_level, unique_ID, standard, and mag
-    - this will look like: {top_level/unique_ID/standard/mag : 
-                                {'xcs' : [XCs to use for that standard],
-                                'magmom' : [magmoms to use for that structure]}
-    - write to a dictionary: launch_dirs.json
-5) Loop through the launch directories and prepare VASP inputs + submission files and launch each chain of VASP jobs using SubmitTools
-    - customizable with _sub_configs, _vasp_configs, and _slurm_configs
-    - SubmitTools will figure out which jobs can be submitted together and how to order them for submission
-    - It will also prepare each VASP job accordingly
-6) Crawl through the launch directories, and analyze every VASP calculation using AnalyzeBatch
-    - customizable with _analysis_configs
-    - write to a dictionary: results.json
-"""
-
-# where is this file
-SCRIPTS_DIR = os.getcwd()
-
-# where are my calculations going to live
-CALCS_DIR = SCRIPTS_DIR.replace("scripts", "calcs")
-
-# where is my data going to live
-DATA_DIR = SCRIPTS_DIR.replace("scripts", "data")
+import os
+import warnings
+from shutil import copyfile
 
-for d in [CALCS_DIR, DATA_DIR]:
-    if not os.path.exists(d):
-        os.makedirs(d)
-
-# if you need data from MP as a starting point (often the case), you need your API key
-API_KEY = "N3KdATtMmcsUL94g"
-
-# lets put a tag on all the files we save
-FILE_TAG = CALCS_DIR.split("/")[-2]
-
-# what to query MP for
-## e.g., 'MnO2', ['MnO2', 'TiO2'], 'Ca-Ti-O, etc
-COMPOSITIONS = ["Zn3MoN4", "ZnMoN2"]
-
-# how to transform MP structures
-## e.g., [x for x in range(5)] ([0,1,2,3,4])
-## NOTE: you need to modify get_strucs to make this work (hard to generalize)
-TRANSFORM_STRUCS = False
-
-# whether or not you want to generate MAGMOMs
-## True if you're running AFM, else False
-GEN_MAGMOMS = True
-
-# what {standard : [final_xcs]} to calculate
-## e.g., {'dmc' : ['metagga', 'ggau']} if you want to run METAGGA + GGA+U at DMC standards
-TO_LAUNCH = {"dmc": ["metagga"]}
-
-# any configurations related to LaunchTools
-## e.g., {'compare_to_mp' : True, 'n_afm_configs' : 4}
-LAUNCH_CONFIGS = {"compare_to_mp": False, "n_afm_configs": 2}
-
-# any configurations related to SubmitTools
-## usually no need to change anything but n_procs... n_procs will determine how to parallelize over launch_dirs
-## NOTE: do not set n_procs = 'all' unless you are running on a compute node (ie not a login node)
-SUB_CONFIGS = {"n_procs": 1}
-
-# any configurations related to Slurm
-## e.g., {'ntasks' : 16, 'time' : int(24*60)}
-SLURM_CONFIGS = {"ntasks": 16, "time": int(24 * 60)}
-
-# any configurations related to VASPSetUp
-## e.g., {'lobster_static' : True, 'relax_incar' : {'ENCUT' : 555}}
-VASP_CONFIGS = {"lobster_static": True}
-
-# any configurations related to AnalyzeBatch
-## e.g., {'include_meta' : True, 'include_mag' : True, 'n_procs' : 4}
-## NOTE: do not set n_procs = 'all' unless you are running on a compute node (ie not a login node)
-ANALYSIS_CONFIGS = {"include_meta": True, "include_mag": True, "n_procs": 4}
+from pymatgen.io.vasp.sets import MPRelaxSet, MPScanRelaxSet
+from pymatgen.core.structure import Structure
+from pymatgen.io.vasp.inputs import Kpoints
+from pymatgen.io.lobster.inputs import Lobsterin
 
 """
-Don't forget to inspect the arguments to:
-    get_query
-    get_strucs
-    get_magmoms
-    get_launch_dirs
-    submit_calcs
-    get_results
+Holey Moley, getting pymatgen to find your POTCARs is not trivial...
+Here's the workflow I used:
+    1) Download potpaw_LDA_PBE_52_54_orig.tar.gz from VASP
+    2) Extract the tar into a directory, we'll call it FULL_PATH/bin/pp
+    3) Download potpaw_PBE.tgz from VASP
+    4) Extract the tar INSIDE a directory: FULL_PATH/bin/pp/potpaw_PBE
+    5) $ cd FULL_PATH/bin
+    6) $ pmg config -p FULL_PATH/bin/pp pymatgen_pot
+    7) $ pmg config --add PMG_VASP_PSP_DIR FULL_PATH/bin/pymatgen_pot
+    8) $ pmg config --add PMG_DEFAULT_FUNCTIONAL PBE_54
+    
+Now that this has been done, new users must just do:
+    1) $ pmg config --add PMG_VASP_PSP_DIR FULL_PATH/bin/pymatgen_pot
+    2) $ pmg config --add PMG_DEFAULT_FUNCTIONAL PBE_54
 
-You'll want to customize these depending on your calculations
 """
 
 
-def get_query(
-    comp,
-    properties=None,
-    criteria=None,
-    only_gs=True,
-    include_structure=True,
-    supercell_structure=[2, 1, 1],
-    max_Ehull=0.05,
-    max_sites_per_structure=65,
-    max_strucs_per_cmpd=4,
-    savename="query_%s.json" % FILE_TAG,
-    remake=False,
-):
-    """
-    Args:
-        comp (list or str)
-            can either be:
-                - a chemical system (str) of elements joined by "-"
-                - a chemical formula (str)
-            can either be a list of:
-                - chemical systems (str) of elements joined by "-"
-                - chemical formulas (str)
-
-        properties (list or None)
-            list of properties to query
-                - if None, then use typical_properties
-                - if 'all', then use supported_properties
-
-        criteria (dict or None)
-            dictionary of criteria to query
-                - if None, then use {}
-
-        only_gs (bool)
-            if True, remove non-ground state polymorphs for each unique composition
-
-        include_structure (bool)
-            if True, include the structure (as a dictionary) for each entry
-
-        supercell_structure (bool)
-            only runs if include_structure = True
-            if False, just retrieve the MP structure
-            if not False, must be specified as [a,b,c] to make an a x b x c supercell of the MP structure
-
-        max_Ehull (float)
-            if not None, remove entries with Ehull_mp > max_Ehull
-
-        max_sites_per_structure (int)
-            if not None, remove entries with more than max_sites_per_structure sites
-
-        max_strucs_per_cmpd (int)
-            if not None, only retain the lowest energy structures for each composition until you reach max_strucs_per_cmpd
-
-        savename (str) - filename for fjson in DATA_DIR
-
-        remake (bool) - write (True) or just read (False) fjson
-
-    Returns:
-        {mpid : {DATA}}
-    """
-
-    fjson = os.path.join(DATA_DIR, savename)
-    if os.path.exists(fjson) and not remake:
-        return read_json(fjson)
-
-    # initialize MPQuery with your API key
-    mpq = MPQuery(api_key=API_KEY)
-
-    # get the data from MP
-    data = mpq.get_data_for_comp(
-        comp=comp,
-        properties=properties,
-        criteria=criteria,
-        only_gs=only_gs,
-        include_structure=include_structure,
-        supercell_structure=supercell_structure,
-        max_Ehull=max_Ehull,
-        max_sites_per_structure=max_sites_per_structure,
-        max_strucs_per_cmpd=max_strucs_per_cmpd,
-    )
-
-    write_json(data, fjson)
-    return read_json(fjson)
-
-
-def check_query(query):
-    for mpid in query:
-        print("\nmpid: %s" % mpid)
-        print("\tcmpd: %s" % query[mpid]["cmpd"])
-        print(
-            "\tstructure formula: %s"
-            % len(StrucTools(query[mpid]["structure"]).formula)
-        )
-
-
-def get_strucs(
-    query,
-    transform_strucs,
-    max_strucs_per_starting_struc=2,
-    ox_states={"Ru": 4, "Ir": 4, "O": -2},
-    savename="strucs_%s.json" % FILE_TAG,
-    remake=False,
-):
+class VASPSetUp(object):
     """
-    Args:
-        query (dict) - {mpid : {DATA}}
-        transform_strucs (bool or list):
-            - if False, just use the structures from MP
-            - if not False:
-                - this should be customized to perform whatever transformations you'd like to perform
-                - *NOTE*: you should also customize species_mapping in this function
-        max_strucs_per_starting_struc (int) - max number of structures to keep for each starting structure
-        ox_states (dict) - {element : oxidation state} for transformations
-            - if None, use AutoOxidationState algo in pymatgen
-        savename (str) - filename for fjson in DATA_DIR
-        remake (bool) - write (True) or just read (False) fjson
-
-    Returns:
-        if not transform_strucs:
-            {formula : {mpid : structure}
-        if transform_strucs:
-            {formula_identifier : {index_identifier : structure}}
-    """
-
-    fjson = os.path.join(DATA_DIR, savename)
-    if os.path.exists(fjson) and not remake:
-        return read_json(fjson)
-
-    # get all unique chemical formulas in the query
-    formulas_in_query = sorted(list(set([query[mpid]["cmpd"] for mpid in query])))
-
-    data = {}
-    for formula in formulas_in_query:
-        # get all MP IDs in your query having that formula
-        mpids = [mpid for mpid in query if query[mpid]["cmpd"] == formula]
-        if not transform_strucs:
-            # if no transformations, just return the structures from MP
-            data[formula] = {mpid: query[mpid]["structure"] for mpid in mpids}
+    Use to write VASP inputs for a single VASP calculation
+        - a calculation here might be defined as the same:
+            - initial structure
+            - initial magnetic configurations
+            - input settings (INCAR, KPOINTS, POTCAR)
+            - etc.
+
+    Also changes inputs based on errors that are encountered
+
+    Note that we rarely need to call this class directly
+        - instead we'll manage things through pydmc.hpc.submit.SubmitTools and pydmc.hpc.launch.LaunchTools
+    """
+
+    def __init__(
+        self,
+        calc_dir,
+        user_configs={},
+        vasp_configs_yaml=os.path.join(
+            os.getcwd(),
+            "_vasp_configs.yaml",
+        ),
+        refresh_configs=True,
+    ):
+        """
+        Args:
+            calc_dir (os.PathLike) - directory where I want to execute VASP
+                - there must be a POSCAR in calc_dir
+                - the other input files will be added automatically within this code
+            user_configs (dict) - user-defined configs
+                - options in vasp_configs_yaml
+            vasp_configs_yaml (os.PathLike) - path to yaml file with possible user_configs and default values
+            refresh_configs (bool) - if True, will copy pydmc baseline configs to your local directory
+                - this is useful if you've made changes to the configs files in the directory you're working in and want to start over
+
+        Returns:
+            calc_dir (os.PathLike) - directory where I want to execute VASP
+            structure (pymatgen.Structure) - structure to be used for VASP calculation
+                - note: raises error if no POSCAR in calc_dir
+            configs (dict)
+                # VASPSetUp (general)
+                # these should get passed through LaunchTools
+                standard: # make mp if comparing to MP data
+                mag:  # **change** as desired
+                magmom: # you will need to pass this for AFM calcs {'magmom' : [list of magmoms (float)]}
+
+                # these should get passed through SubmitTools
+                xc_to_run:  # gga, ggau, or metagga
+                calc_to_run: # usually this is what we want unless you want an independent "static" or "loose" calc
+
+                fun: # usually this is fine
+                lobster_static: True # can make False if you don't want to run LOBSTER
+
+                # some output files
+                fvaspout: vasp.o # where vasp output goes in calc_dir for each vasp run
+                fvasperrors: errors.o # where vasp errors go in calc_dir for each vasp run
+
+                # may be desirable to pass various configs for each type of calculation
+                # INCARs should be {INCAR_FLAG : value}
+                # KPOINTs should be Kpoints object
+                # POTCARs should be {el (str) : potcar flag (str)}
+
+                # loose calculations
+                loose_incar: {} # e.g., {'ENCUT' : 555}
+                loose_kpoints: {} # e.g., {'length' : 25}
+                loose_potcar: {} # e.g., {'W' : 'W_pv'}
+
+                # relax calculations
+                relax_incar: {}
+                relax_kpoints: {}
+                relax_potcar: {}
+
+                # static calculations
+                static_incar: {}
+                static_kpoints: {}
+                static_potcar: {}
+
+                # lobster calculations
+                lobster_incar: {}
+                lobster_kpoints: {}
+                lobster_potcar: {}
+
+                # rarely need to change these:
+                mag_override: False # if True, allows user to run nm calcs for mag systems and vice versa
+                potcar_functional: PBE_54 # probably don't change
+                validate_magmom: False # probably don't change
+        """
+
+        # this is where we will execute VASP
+        self.calc_dir = calc_dir
+
+        # we should have a POSCAR in calc_dir already
+        # e.g., LaunchTools will set this up for you
+        fpos = os.path.join(calc_dir, "POSCAR")
+        if not os.path.exists(fpos):
+            raise FileNotFoundError("POSCAR not found in {}".format(calc_dir))
         else:
-            # now you need to customize this for whatever transformations you want
-            if len(mpids) > 1:
-                print("WARNING: %s has %i mpids" % (formula, len(mpids)))
-                raise NotImplementedError(
-                    "folder structure is not super amenable to this... Reconfiguring recommended"
-                )
-
-            # take our 1 MP ID of interest and transform it
-            mpid = mpids[0]
-            initial_structure = query[mpid]["structure"]
-            for x in transform_strucs:
-                # make a new "formula" that includes are iterator in the transformation
-                key = "_".join([formula, str(x)])
-                structools = StrucTools(
-                    structure=initial_structure, ox_states=ox_states
-                )
-
-                species_mapping = {
-                    "Ru": {"Ru": 1 - x / max(x), "Ir": x / (max(x))}
-                }  # *NOTE*: you should customize this for your desired transformation
-
-                # strucs will have the form {index_identifier : structure}
-                strucs = structools.replace_species(
-                    species_mapping=species_mapping,
-                    n_strucs=max_strucs_per_starting_struc,
-                )
-
-                data[key] = strucs
+            self.structure = Structure.from_file(fpos)
 
-    write_json(data, fjson)
-    return read_json(fjson)
-
-
-def check_strucs(strucs):
-    for formula in strucs:
-        for ID in strucs[formula]:
-            print("\nformula: %s" % formula)
-            print("\tID: %s" % ID)
-            struc = strucs[formula][ID]
-            print("\tstructure formula: %s" % StrucTools(struc).formula)
-
-
-def get_magmoms(
-    strucs,
-    max_afm_combos=50,
-    treat_as_nm=[],
-    savename="magmoms_%s.json" % FILE_TAG,
-    remake=False,
-):
-    """
-    Args:
-        strucs (dict) - {formula : {ID : structure}}
-        max_afm_combos (int): maximum number of AFM spin configurations to generate
-        treat_as_nm (list): any normally mag els you'd like to treat as nonmagnetic for AFM enumeration
-        savename (str) - filename for fjson in DATA_DIR
-        remake (bool) - write (True) or just read (False) fjson
-
-    Returns:
-        {formula : {ID : {AFM configuration index : [list of magmoms on each site]}
-    """
-
-    fjson = os.path.join(DATA_DIR, savename)
-    if not remake and os.path.exists(fjson):
-        return read_json(fjson)
-
-    magmoms = {}
-    for formula in strucs:
-        magmoms[formula] = {}
-        for ID in strucs[formula]:
-            # for each unique structure, get AFM magmom orderings
-            structure = strucs[formula][ID]
-            magtools = MagTools(
-                structure=structure,
-                max_afm_combos=max_afm_combos,
-                treat_as_nm=treat_as_nm,
+        # write a local yaml with vasp configs
+        # if you don't have one or
+        # if you want to "refresh" them
+        if not os.path.exists(vasp_configs_yaml) or refresh_configs:
+            _vasp_configs = load_vasp_configs()
+            write_yaml(_vasp_configs, vasp_configs_yaml)
+
+        # read local yaml to get baseline vasp_configs
+        _vasp_configs = read_yaml(vasp_configs_yaml)
+
+        # augment baseline vasp_configs with user_configs
+        # NOTE: user_configs will overwrite any keys shared with vasp_configs
+        configs = {**_vasp_configs, **user_configs}
+
+        essential_configs = ["xc_to_run", "calc_to_run", "standard", "mag"]
+        for essential in essential_configs:
+            if essential not in configs.keys():
+                raise KeyError("{} must be specified in user_configs".format(essential))
+
+        # copy configs to prevent further changes
+        self.configs = configs.copy()
+
+        perturbation = self.configs["perturb_struc"]
+        if perturbation:
+            initial_structure = self.structure.copy()
+            perturbed_structure = StrucTools(initial_structure).perturb(perturbation)
+            self.structure = perturbed_structure
+
+    @property
+    def get_vasp_input(self):
+        """
+        Returns:
+            vasp_input (pymatgen.io.vasp.sets.VaspInputSet
+
+        Uses configs to modify pymatgen's VaspInputSets as required
+        """
+
+        # copy configs to prevent unwanted updates
+        configs = self.configs.copy()
+
+        # initialize how we're going to modify each vasp input file with configs specs
+        modify_incar = configs["%s_incar" % configs["calc_to_run"]].copy()
+        modify_kpoints = configs["%s_kpoints" % configs["calc_to_run"]].copy()
+        modify_potcar = configs["%s_potcar" % configs["calc_to_run"]].copy()
+
+        # initialize potcar functional
+        potcar_functional = configs["potcar_functional"]
+
+        # this should be kept off in general, gives unuseful warnings (I think)
+        validate_magmom = configs["validate_magmom"]
+
+        # tell user what they are modifying in case they are trying to match MP or other people's calculations
+        if configs["standard"] and modify_incar:
+            warnings.warn(
+                "you are attempting to generate consistent data, but modifying things in the INCAR\n"
             )
-            curr_magmoms = magtools.get_afm_magmoms
-            magmoms[formula][ID] = curr_magmoms
+            # print('e.g., %s' % str(modify_incar))
 
-    write_json(magmoms, fjson)
-    return read_json(fjson)
-
-
-def check_magmoms(strucs, magmoms):
-    for formula in strucs:
-        for ID in strucs[formula]:
-            structure_formula = StrucTools(strucs[formula][ID]).formula
-            n_afm_configs = len(magmoms[formula][ID])
-            print("%s: %i AFM configs\n" % (structure_formula, n_afm_configs))
-
-
-def get_launch_dirs(
-    strucs,
-    magmoms,
-    to_launch,
-    user_configs,
-    make_launch_dirs=True,
-    refresh_configs=True,
-    savename="launch_dirs_%s.json" % FILE_TAG,
-    remake=False,
-):
-    """
-    Args:
-        strucs (dict) - {formula : {ID : structure}}
-        magmoms (dict) - {formula : {ID : {AFM configuration index : [list of magmoms on each site]}}
-        to_launch (dict) - {standard (str) : [list of final_xcs of interest]}
-        user_configs (dict) - optional launch configurations
-        make_launch_dirs (bool) - make launch directories (True) or just return launch dict (False)
-        refresh_configs (bool) - refresh configs (True) or just use existing configs (False)
-        savename (str) - filename for fjson in DATA_DIR
-        remake (bool) - write (True) or just read (False) fjson
-
-    Returns:
-        {launch_dir (formula/ID/standard/mag) : {'xcs' : [list of final_xcs],
-                                                 'magmoms' : [list of magmoms for each site in structure in launch_dir]}}
-
-        also makes launch_dir and populates with POSCAR using strucs if make_dirs=True
-
-    """
-
-    fjson = os.path.join(DATA_DIR, savename)
-    if os.path.exists(fjson) and not remake:
-        return read_json(fjson)
-
-    all_launch_dirs = {}
-    for formula in strucs:
-        for ID in strucs[formula]:
-            # for each unique structure, generate our launch directories
-            structure = strucs[formula][ID]
-            if magmoms:
-                curr_magmoms = magmoms[formula][ID]
-            else:
-                curr_magmoms = None
-            top_level = formula
-            unique_ID = ID
-
-            launch = LaunchTools(
-                calcs_dir=CALCS_DIR,
-                to_launch=to_launch,
-                user_configs=user_configs,
-                magmoms=curr_magmoms,
-                structure=structure,
-                top_level=top_level,
-                unique_ID=unique_ID,
-                refresh_configs=refresh_configs,
+        if configs["standard"] and modify_kpoints:
+            warnings.warn(
+                "you are attempting to generate consistent data, but modifying things in the KPOINTS\n"
             )
+            # print('e.g., %s' % str(modify_kpoints))
 
-            launch_dirs = launch.launch_dirs(make_dirs=make_launch_dirs)
-
-            for launch_dir in launch_dirs:
-                all_launch_dirs[launch_dir] = launch_dirs[launch_dir]
-
-    write_json(all_launch_dirs, fjson)
-    return read_json(fjson)
-
-
-def check_launch_dirs(launch_dirs):
-    print("\nanalyzing launch directories")
-    for d in launch_dirs:
-        print("\nlaunching from %s" % d)
-        print("   these final xcs: %s" % launch_dirs[d]["xcs"])
+        if configs["standard"] and modify_potcar:
+            warnings.warn(
+                "you are attempting to generate consistent data, but modifying things in the POTCAR\n"
+            )
+            # print('e.g., %s' % str(modify_potcar))
 
+        # tell user they are doing a nonmagnetic calculation for a compound w/ magnetic elements
+        if MagTools(self.structure).could_be_magnetic and (configs["mag"] == "nm"):
+            warnings.warn(
+                "structure could be magnetic, but you are performing a nonmagnetic calculation\n"
+            )
 
-def submit_one_calc(submit_args):
+        structure = self.structure
 
-    """
-    Prepares VASP inputs, writes submission script, and launches job for one launch_dir
+        # add MAGMOM to structure
+        if configs["mag"] == "nm":
+            # if non-magnetic, MagTools takes care of this
+            structure = MagTools(structure).get_nonmagnetic_structure
+        elif configs["mag"] == "fm":
+            # if ferromagnetic, MagTools takes care of this
+            structure = MagTools(structure).get_ferromagnetic_structure
+        elif "afm" in configs["mag"]:
+            # if antiferromagnetic, we need to aprovide a MAGMOM
+            magmom = configs["magmom"]
+            if not magmom:
+                raise ValueError("you must specify a magmom for an AFM calculation\n")
+            if (min(magmom) >= 0) and (max(magmom) <= 0):
+                raise ValueError(
+                    "provided magmom that is not AFM, but you are trying to run an AFM calculation\n"
+                )
+            structure.add_site_property("magmom", magmom)
 
-    Args:
-        submit_args (dict) should contain:
-        {'launch_dir' :
-            launch_dir (str) - (formula/ID/standard/mag) to write and launch submission script in,
-         'launch_dirs' :
-            launch_dirs (dict) - {launch_dir (formula/ID/standard/mag) : {'xcs' : [list of final_xcs], 'magmoms' : [list of magmoms for each site in structure in launch_dir]}},
-         'user_configs' :
-            user_configs (dict) - optional sub, slurm, or VASP configurations,
-         'refresh_configs' :
-            refresh_configs (list) - list of which configs to refresh,
-         'ready_to_launch':
-            ready_to_launch (bool) - write (True) and launch (True) or just write (False) submission scripts (False)
+        # MP wants to set W_pv but we don't have that one in PBE54 (no biggie)
+        """
+        if configs["standard"] != "mp":
+            modify_potcar["W"] = "W"
+        """
+
+        # don't mess with much if trying to match Materials Project
+        if configs["standard"] == "mp":
+            # use our default functional
+            fun = None
+            # set KPOINTS to be MP-consistent
+            if not isinstance(modify_kpoints, dict):
+                modify_kpoints = {}
+                modify_kpoints["reciprocal_density"] = 64
+
+        # setting DMC standards --> what to do on top of MPRelaxSet or MPScanRelaxSet (pymatgen defaults)
+        if configs["standard"] == "dmc":
+            # use our default functional
+            fun = None
+
+            # tweak a few INCAR settings
+            # converge using forces (EDIFFG < 0)
+            # stricter EDIFF
+            # ISMEAR = 0 (less convergence errors)
+            # fix ENCUT, ENAUG to be reasonable
+            # turn off symmetry (mostly, ISYM = 0)
+            dmc_standard_settings = {
+                "EDIFF": 1e-6,
+                "EDIFFG": -0.03,
+                "ISMEAR": 0,
+                "ENCUT": 520,
+                "ENAUG": 1040,
+                "ISYM": 0,
+                "SIGMA": 0.01,
+            }
+            for key in dmc_standard_settings:
+                if key not in modify_incar:
+                    modify_incar[key] = dmc_standard_settings[key]
+
+            # use length = 25 means reciprocal space discretization of 25 K-points per Å−1
+            if configs["calc_to_run"] != "loose":
+                if not modify_kpoints:
+                    modify_kpoints = {"length": 25}
+
+            # turn off +U unless we are specifying GGA+U
+            if configs["xc_to_run"] != "ggau":
+                if "LDAU" not in modify_incar:
+                    modify_incar["LDAU"] = False
+
+            # turn off ISPIN for nonmagnetic calculations
+            if "ISPIN" not in modify_incar:
+                modify_incar["ISPIN"] = 1 if configs["mag"] == "nm" else 2
+
+        # start from MPRelaxSet for GGA or GGA+U
+        if configs["xc_to_run"] in ["gga", "ggau"]:
+            vaspset = MPRelaxSet
+
+            # use custom functional (eg PBEsol) if you want
+            # needs to be specified in user_configs['fun']
+            # otherwise use PBE for gga, gga+u
+            if "GGA" not in modify_incar:
+                if fun:
+                    modify_incar["GGA"] = fun.upper()
+                else:
+                    modify_incar["GGA"] = "PE"
+
+            # for strict comparison to Materials Project GGA(+U) calculations, we need to use the old POTCARs
+            if configs["standard"] == "mp":
+                potcar_functional = "PBE"
+
+        # start from MPScanRelaxSet for meta-GGA
+        elif configs["xc_to_run"] == "metagga":
+            vaspset = MPScanRelaxSet
+
+            # use custom functional (eg SCAN) if you want
+            # needs to be specified in user_configs['fun']
+            # otherwise use r2SCAN for metagga
+            if "METAGGA" not in modify_incar:
+                if fun:
+                    modify_incar["METAGGA"] = fun.upper()
+                else:
+                    modify_incar["METAGGA"] = "R2SCAN"
+
+        # default "loose" relax
+        if configs["calc_to_run"] == "loose":
+            # use only 1 kpoint
+            modify_kpoints = Kpoints()
+            # make the settings a little looser
+            loose_settings = {
+                "ENCUT": 400,
+                "ENAUG": 800,
+                "ISIF": 3,
+                "EDIFF": 1e-5,
+                "NELM": 40,
             }
+            for key in loose_settings:
+                if key not in modify_incar:
+                    modify_incar[key] = loose_settings[key]
+
+        # default "static" claculation
+        if configs["calc_to_run"] == "static":
+            # don't optimize the geometry
+            # do save things like charge density
+            static_settings = {
+                "LCHARG": True,
+                "LREAL": False,
+                "NSW": 0,
+                "LORBIT": 0,
+                "LVHAR": True,
+                "ICHARG": 0,
+                "LAECHG": True,
+            }
+            for key in static_settings:
+                if key not in static_settings:
+                    modify_incar[key] = static_settings[key]
+
+        # make sure WAVECAR is written unless told user specified not to
+        if "LWAVE" not in modify_incar:
+            modify_incar["LWAVE"] = True
+
+        # use better parallelization
+        if ("NCORE" not in modify_incar) and ("NPAR" not in modify_incar):
+            modify_incar["NCORE"] = 4
+
+        # add more ionic steps
+        if "NSW" not in modify_incar:
+            if configs["calc_to_run"] == "static":
+                modify_incar["NSW"] = 0
+            else:
+                modify_incar["NSW"] = 199
 
-    Returns:
-        None
+        # make sure spin is off for nm calculations
+        if configs["mag"] == "nm":
+            modify_incar["ISPIN"] = 1
+        else:
+            # make sure magnetization is written to OUTCAR for magnetic calcs
+            modify_incar["LORBIT"] = 11
 
-    """
-    launch_dir = submit_args["launch_dir"]
-    launch_dirs = submit_args["launch_dirs"]
-    user_configs = submit_args["user_configs"]
-    refresh_configs = submit_args["refresh_configs"]
-    ready_to_launch = submit_args["ready_to_launch"]
-
-    # what are our terminal xcs for that launch_dir
-    final_xcs = launch_dirs[launch_dir]["xcs"]
-
-    # what magmoms apply to that launch_dir
-    magmom = launch_dirs[launch_dir]["magmom"]
-
-    try:
-        sub = SubmitTools(
-            launch_dir=launch_dir,
-            final_xcs=final_xcs,
-            magmom=magmom,
-            user_configs=user_configs,
-            refresh_configs=refresh_configs,
+        # if we are doing LOBSTER, need special parameters
+        # note: some of this gets handled later for us
+        if configs["lobster_static"] and (configs["calc_to_run"] == "static"):
+            if configs["standard"] != "mp":
+                # want more DOS points
+                # want to write charge densities
+                # new NBANDS so don't want to start from WAVECAR
+                lobster_incar_settings = {"NEDOS": 4000, "ISTART": 0, "LAECHG": True}
+                for key in lobster_incar_settings:
+                    if key not in configs["lobster_incar"]:
+                        modify_incar[key] = lobster_incar_settings[key]
+
+                for key in configs["lobster_incar"]:
+                    modify_incar[key] = configs["lobster_incar"][key]
+
+                if not configs["lobster_kpoints"]:
+                    # need KPOINTS file for LOBSTER
+                    modify_kpoints = {"length": 25}
+                else:
+                    modify_kpoints = configs["lobster_kpoints"]
+
+        if configs["lobster_static"]:
+            if configs["xc_to_run"] == "metagga":
+                # gga-static will get ISYM = -1, so need to pass that to metagga relax otherwise WAVECAR from GGA doesnt help metagga
+                modify_incar["ISYM"] = -1
+
+        print("modify_incar = %s" % modify_incar)
+        # initialize new VASPSet with all our settings
+        vasp_input = vaspset(
+            structure,
+            user_incar_settings=modify_incar,
+            user_kpoints_settings=modify_kpoints,
+            user_potcar_settings=modify_potcar,
+            user_potcar_functional=potcar_functional,
+            validate_magmom=validate_magmom,
         )
 
-        # prepare VASP directories and write submission script
-        sub.write_sub
-
-        # submit submission script to the queue
-        if ready_to_launch:
-            sub.launch_sub
-
-        success = True
-    except TypeError:
-        print("\nERROR: %s\n   will submit without multiprocessing" % launch_dir)
-        success = False
-
-    return {"launch_dir": launch_dir, "success": success}
-
-
-def submit_calcs(
-    launch_dirs,
-    user_configs={},
-    refresh_configs=["vasp", "sub", "slurm"],
-    ready_to_launch=True,
-    n_procs=1,
-):
-    """
-    Prepares VASP inputs, writes submission script, and launches job for all launch_dirs
+        return vasp_input
 
-    Args:
-        launch_dirs (dict) - {launch_dir (formula/ID/standard/mag) : {'xcs' : [list of final_xcs], 'magmoms' : [list of magmoms for each site in structure in launch_dir]}}
-        user_configs (dict) - optional sub, slurm, or VASP configurations
-        refresh_configs (list) - list of which configs to refresh
-        ready_to_launch (bool) - write (True) and launch (True) or just write (False) submission scripts (False
-
-    Returns:
-        None
-
-    """
+    @property
+    def prepare_calc(self):
+        """
+        Write input files (INCAR, KPOINTS, POTCAR)
+        """
+
+        configs = self.configs.copy()
+        calc_dir = self.calc_dir
+
+        vasp_input = self.get_vasp_input
+        if not vasp_input:
+            return None
+
+        # write input files
+        vasp_input.write_input(calc_dir)
+
+        # for LOBSTER, use Janine George's Lobsterin approach (mainly to get NBANDS)
+        if (configs["lobster_static"]) and (configs["calc_to_run"] == "static"):
+            INCAR_input = os.path.join(calc_dir, "INCAR_input")
+            INCAR_output = os.path.join(calc_dir, "INCAR")
+            copyfile(INCAR_output, INCAR_input)
+            POSCAR_input = os.path.join(calc_dir, "POSCAR")
+            POTCAR_input = os.path.join(calc_dir, "POTCAR")
+            lobsterin = Lobsterin.standard_calculations_from_vasp_files(
+                POSCAR_input=POSCAR_input,
+                INCAR_input=INCAR_input,
+                POTCAR_input=POTCAR_input,
+                option="standard",
+            )
 
-    submit_args = {
-        "launch_dirs": launch_dirs,
-        "user_configs": user_configs,
-        "refresh_configs": refresh_configs,
-        "ready_to_launch": ready_to_launch,
-    }
-
-    if n_procs == 1:
-        print("\n\n submitting calculations in serial\n\n")
-        for launch_dir in launch_dirs:
-            curr_submit_args = submit_args.copy()
-            curr_submit_args["launch_dir"] = launch_dir
-            submit_one_calc(curr_submit_args)
-        return
-    elif n_procs == "all":
-        n_procs = multip.cpu_count() - 1
-
-    print("\n\n submitting calculations in parallel\n\n")
-    print("not refreshing configs for parallel --> causes trouble")
-    submit_args["refresh_configs"] = refresh_configs
-    list_of_submit_args = []
-    for launch_dir in launch_dirs:
-        curr_submit_args = submit_args.copy()
-        curr_submit_args["launch_dir"] = launch_dir
-        list_of_submit_args.append(curr_submit_args)
-    pool = multip.Pool(processes=n_procs)
-    statuses = pool.map(submit_one_calc, list_of_submit_args)
-    pool.close()
-
-    submitted_w_multiprorcessing = [status for status in statuses if status["success"]]
-    failed_w_multiprocessing = [status for status in statuses if not status["success"]]
-
-    print(
-        "%i/%i calculations submitted with multiprocessing"
-        % (len(submitted_w_multiprorcessing), len(statuses))
-    )
-    for status in failed_w_multiprocessing:
-        launch_dir = status["launch_dir"]
-        curr_submit_args = submit_args.copy()
-        curr_submit_args["launch_dir"] = launch_dir
-        submit_one_calc(curr_submit_args)
+            lobsterin_dict = lobsterin.as_dict()
 
-    return
+            lobsterin_dict["COHPSteps"] = 4000
+            lobsterin = Lobsterin.from_dict(lobsterin_dict)
 
+            flobsterin = os.path.join(calc_dir, "lobsterin")
+            lobsterin.write_lobsterin(flobsterin)
 
-def get_results(
-    launch_dirs,
-    user_configs,
-    refresh_configs=True,
-    savename="results_%s.json" % FILE_TAG,
-    remake=False,
-):
-    """
-    Args:
-        launch_dirs (dict) - {launch_dir (formula/ID/standard/mag) : {'xcs' : [list of final_xcs], 'magmoms' : [list of magmoms for each site in structure in launch_dir]}}
-        user_configs (dict) - optional analysis configurations
-        refresh_configs (bool) - refresh configs (True) or just use existing configs (False)
-        savename (str) - filename for fjson in DATA_DIR
-        remake (bool) - write (True) or just read (False) fjson
+            lobsterin.write_INCAR(
+                incar_input=INCAR_input,
+                incar_output=INCAR_output,
+                poscar_input=POSCAR_input,
+            )
 
-    Returns:
-        {'formula.ID.standard.mag.xc_calc' : {scraped results from VASP calculation}}
-    """
+        return vasp_input
 
-    fjson = os.path.join(DATA_DIR, savename)
-    if os.path.exists(fjson) and not remake:
-        return read_json(fjson)
-
-    analyzer = AnalyzeBatch(
-        launch_dirs, user_configs=user_configs, refresh_configs=refresh_configs
-    )
-
-    data = analyzer.results
-
-    write_json(data, fjson)
-    return read_json(fjson)
-
-
-def check_results(results):
-
-    keys_to_check = list(results.keys())
-
-    converged = 0
-    for key in keys_to_check:
-        top_level, ID, standard, mag, xc_calc = key.split(".")
-        data = results[key]
-        convergence = results[key]["results"]["convergence"]
-        print("\n%s" % key)
-        print("convergence = %s" % convergence)
-        if convergence:
-            converged += 1
-            print("E (static) = %.2f" % data["results"]["E_per_at"])
-            continue
-            if ANALYSIS_CONFIGS["include_meta"]:
-                print("E (relax) = %.2f" % data["meta"]["E_relax"])
-                print("EDIFFG = %i" % data["meta"]["incar"]["EDIFFG"])
-                print("1st POTCAR = %s" % data["meta"]["potcar"][0])
-            if (
-                (mag != "nm")
-                and ("include_mag" in ANALYSIS_CONFIGS)
-                and (ANALYSIS_CONFIGS["include_mag"])
-            ):
-                magnetization = data["magnetization"]
-                an_el = list(magnetization.keys())[0]
-                an_idx = list(magnetization[an_el].keys())[0]
-                that_mag = magnetization[an_el][an_idx]["mag"]
-                print("mag on %s (%s) = %.2f" % (an_el, str(an_idx), that_mag))
-            if ("include_structure" not in ANALYSIS_CONFIGS) or (
-                ANALYSIS_CONFIGS["include_structure"]
-            ):
-                print(data["structure"])
+    @property
+    def error_msgs(self):
+        """
+        Dict of {group of errors (str) : [list of error messages (str) in group]}
+            - the error messages are things that VASP will write to fvaspout
+            - we'll crawl fvaspout and assemble what errors made VASP fail,
+                then we'll make edits to VASP calculation to clean them up for re-launch
+        """
+        return {
+            "tet": [
+                "Tetrahedron method fails for NKPT<4",
+                "Fatal error detecting k-mesh",
+                "Fatal error: unable to match k-point",
+                "Routine TETIRR needs special values",
+                "Tetrahedron method fails (number of k-points < 4)",
+            ],
+            "inv_rot_mat": [
+                "inverse of rotation matrix was not found (increase " "SYMPREC)"
+            ],
+            "brmix": ["BRMIX: very serious problems"],
+            "subspacematrix": ["WARNING: Sub-Space-Matrix is not hermitian in " "DAV"],
+            "tetirr": ["Routine TETIRR needs special values"],
+            "incorrect_shift": ["Could not get correct shifts"],
+            "real_optlay": ["REAL_OPTLAY: internal error", "REAL_OPT: internal ERROR"],
+            "rspher": ["ERROR RSPHER"],
+            "dentet": ["DENTET"],
+            "too_few_bands": ["TOO FEW BANDS"],
+            "triple_product": ["ERROR: the triple product of the basis vectors"],
+            "rot_matrix": ["Found some non-integer element in rotation matrix"],
+            "brions": ["BRIONS problems: POTIM should be increased"],
+            "pricel": ["internal error in subroutine PRICEL"],
+            "zpotrf": ["LAPACK: Routine ZPOTRF failed"],
+            "amin": ["One of the lattice vectors is very long (>50 A), but AMIN"],
+            "zbrent": [
+                "ZBRENT: fatal internal in",
+                "ZBRENT: fatal error in bracketing",
+            ],
+            "pssyevx": ["ERROR in subspace rotation PSSYEVX"],
+            "eddrmm": ["WARNING in EDDRMM: call to ZHEGV failed"],
+            "edddav": ["Error EDDDAV: Call to ZHEGV failed"],
+            "grad_not_orth": ["EDWAV: internal error, the gradient is not orthogonal"],
+            "nicht_konv": ["ERROR: SBESSELITER : nicht konvergent"],
+            "zheev": ["ERROR EDDIAG: Call to routine ZHEEV failed!"],
+            "elf_kpar": ["ELF: KPAR>1 not implemented"],
+            "elf_ncl": ["WARNING: ELF not implemented for non collinear case"],
+            "rhosyg": ["RHOSYG internal error"],
+            "posmap": ["POSMAP internal error: symmetry equivalent atom not found"],
+            "point_group": ["Error: point group operation missing"],
+            "ibzkpt": ["internal error in subroutine IBZKPT"],
+            "bad_sym": [
+                "ERROR: while reading WAVECAR, plane wave coefficients changed"
+            ],
+        }
+
+    @property
+    def unconverged_log(self):
+        """
+        checks to see if both ionic and electronic convergence have been reached
+            if calculation had NELM # electronic steps, electronic convergence may not be met
+            if calculation had NSW # ionic steps, ionic convergence may not be met
+
+        returns a list, unconverged, that can have 0, 1, or 2 items
+
+            if unconverged = []:
+                the calculation either:
+                    1) didn't finish (vasprun.xml not found or incomplete)
+                    2) both ionic and electronic convergence were met
+            if 'nelm_too_low' in unconverged:
+                the calculation didn't reach electronic convergence
+            if 'nsw_too_low' in unconverged:
+                the calculation didn't reach ionic convergence
+        """
+        calc_dir = self.calc_dir
+        configs = self.configs.copy()
+        analyzer = AnalyzeVASP(calc_dir)
+        outputs = VASPOutputs(calc_dir)
+        unconverged = []
+
+        # if calc is fully converged, return empty list (calc is done)
+        if analyzer.is_converged:
+            return unconverged
+
+        # if vasprun doesnt exist, return empty list (calc errored out or didnt start yet)
+        vr = outputs.vasprun
+        if not vr:
+            return unconverged
+
+        # make sure last electronic loop converged in calc
+        electronic_convergence = vr.converged_electronic
+
+        # if we're relaxing the geometry, make sure last ionic loop converged
+        if configs["calc_to_run"] == "relax":
+            ionic_convergence = vr.converged_ionic
+        else:
+            ionic_convergence = True
 
-    print("\n\n SUMMARY: %i/%i converged" % (converged, len(keys_to_check)))
+        if not electronic_convergence:
+            unconverged.append("nelm_too_low")
+        if not ionic_convergence:
+            unconverged.append("nsw_too_low")
+
+        return unconverged
+
+    @property
+    def error_log(self):
+        """
+        Parse fvaspout for error messages
+
+        Returns list of errors (str)
+        """
+        error_msgs = self.error_msgs
+        out_file = os.path.join(self.calc_dir, self.configs["fvaspout"])
+        errors = []
+        with open(out_file) as f:
+            contents = f.read()
+        for e in error_msgs:
+            for t in error_msgs[e]:
+                if t in contents:
+                    errors.append(e)
+        return errors
+
+    @property
+    def is_clean(self):
+        """
+        True if no errors found and calc is fully converged, else False
+        """
+        configs = self.configs.copy()
+        calc_dir = self.calc_dir
+        clean = False
+        if AnalyzeVASP(calc_dir).is_converged:
+            clean = True
+        if not os.path.exists(os.path.join(calc_dir, configs["fvaspout"])):
+            clean = True
+        if clean == True:
+            with open(os.path.join(calc_dir, configs["fvasperrors"]), "w") as f:
+                f.write("")
+            return clean
+        errors = self.error_log + self.unconverged_log
+        if len(errors) == 0:
+            return True
+        with open(os.path.join(calc_dir, configs["fvasperrors"]), "w") as f:
+            for e in errors:
+                f.write(e + "\n")
+        return clean
+
+    @property
+    def incar_changes_from_errors(self):
+        """
+        Automatic INCAR changes based on errors
+            - note: also may remove WAVECAR and/or CHGCAR as needed
+
+        Returns {INCAR key (str) : INCAR value (str)}
+
+        This will get passed to VASPSetUp the next time we launch (using SubmitTools)
+
+        These error fixes are mostly taken from custodian (https://github.com/materialsproject/custodian/blob/809d8047845ee95cbf0c9ba45f65c3a94840f168/custodian/vasp/handlers.py)
+            + a few of my own fixes I've added over the years
+        """
+        calc_dir = self.calc_dir
+        errors = self.error_log
+        unconverged_log = self.unconverged_log
+        chgcar = os.path.join(calc_dir, "CHGCAR")
+        wavecar = os.path.join(calc_dir, "WAVECAR")
+
+        incar_changes = {}
+        if "grad_not_orth" in errors:
+            incar_changes["SIGMA"] = 0.05
+            if os.path.exists(wavecar):
+                os.remove(wavecar)
+            incar_changes["ALGO"] = "Exact"
+        if "edddav" in errors:
+            incar_changes["ALGO"] = "All"
+            if os.path.exists(chgcar):
+                os.remove(chgcar)
+        if "eddrmm" in errors:
+            if os.path.exists(wavecar):
+                os.remove(wavecar)
+            incar_changes["ALGO"] = "Normal"
+        if "subspacematrix" in errors:
+            incar_changes["LREAL"] = False
+            incar_changes["PREC"] = "Accurate"
+        if "inv_rot_mat" in errors:
+            incar_changes["SYMPREC"] = 1e-8
+        if "zheev" in errors:
+            incar_changes["ALGO"] = "Exact"
+        if "zpotrf" in errors:
+            incar_changes["ISYM"] = -1
+        if "zbrent" in errors:
+            incar_changes["IBRION"] = 1
+        if "brmix" in errors:
+            incar_changes["IMIX"] = 1
+        if "ibzkpt" in errors:
+            incar_changes["SYMPREC"] = 1e-10
+            incar_changes["ISMEAR"] = 0
+            incar_changes["ISYM"] = -1
+        if "posmap" in errors:
+            incar_changes["SYMPREC"] = 1e-5
+            incar_changes["ISMEAR"] = 0
+            incar_changes["ISYM"] = -1
+        if "nelm_too_low" in unconverged_log:
+            incar_changes["NELM"] = 399
+            incar_changes["ALGO"] = "All"
+        if "nsw_too_low" in unconverged_log:
+            incar_changes["NSW"] = 399
+        if "real_optlay" in errors:
+            incar_changes["LREAL"] = False
+        if "bad_sym" in errors:
+            incar_changes["ISYM"] = -1
+        if "amin" in errors:
+            incar_changes["AMIN"] = 0.01
+        if "pricel" in errors:
+            incar_changes["SYMPREC"] = 1e-8
+            incar_changes["ISYM"] = 0
+        return incar_changes
 
 
 def main():
-
-    if not os.path.exists("sub_launcher.sh"):
-        make_sub_for_launcher()
-
-    remake_query = False
-    print_query_check = True
-
-    remake_strucs = False
-    print_strucs_check = True
-
-    remake_magmoms = False
-    print_magmoms_check = True
-
-    remake_launch_dirs = False
-    print_launch_dirs_check = True
-
-    remake_subs = True
-    ready_to_launch = True
-
-    remake_results = True
-    print_results_check = True
-
-    comp = COMPOSITIONS
-    query = get_query(comp=comp, remake=remake_query)
-    if print_query_check:
-        check_query(query)
-
-    transform_strucs = TRANSFORM_STRUCS
-    strucs = get_strucs(
-        query=query, transform_strucs=transform_strucs, remake=remake_strucs
-    )
-    if print_strucs_check:
-        check_strucs(strucs)
-
-    if GEN_MAGMOMS:
-        magmoms = get_magmoms(strucs=strucs, remake=remake_magmoms)
-        if print_magmoms_check:
-            check_magmoms(strucs=strucs, magmoms=magmoms)
-    else:
-        magmoms = None
-
-    to_launch = TO_LAUNCH
-    launch_configs = LAUNCH_CONFIGS
-    launch_dirs = get_launch_dirs(
-        strucs=strucs,
-        magmoms=magmoms,
-        to_launch=to_launch,
-        user_configs=launch_configs,
-        remake=remake_launch_dirs,
-    )
-    if print_launch_dirs_check:
-        check_launch_dirs(launch_dirs)
-
-    sub_configs = SUB_CONFIGS
-    slurm_configs = SLURM_CONFIGS
-    vasp_configs = VASP_CONFIGS
-    user_sub_configs = {**sub_configs, **slurm_configs, **vasp_configs}
-    if remake_subs:
-        submit_calcs(
-            launch_dirs=launch_dirs,
-            user_configs=user_sub_configs,
-            ready_to_launch=ready_to_launch,
-            n_procs=sub_configs["n_procs"],
-        )
-
-    analysis_configs = ANALYSIS_CONFIGS
-    results = get_results(
-        launch_dirs=launch_dirs, user_configs=analysis_configs, remake=remake_results
-    )
-    if print_results_check:
-        check_results(results)
-
     return
 
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pydmclab-1.0.0/pydmclab/dev/echem.py` & `pydmclab-1.0.1/pydmclab/dev/echem.py`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.0/pydmclab/dev/entries.py` & `pydmclab-1.0.1/pydmclab/dev/entries.py`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.0/pydmclab/hpc/README.md` & `pydmclab-1.0.1/pydmclab/hpc/README.md`

 * *Files identical despite different names*

### Comparing `pydmclab-1.0.0/pydmclab/hpc/analyze.py` & `pydmclab-1.0.1/pydmclab/hpc/analyze.py`

 * *Files 3% similar despite different names*

```diff
@@ -647,16 +647,16 @@
                 sorted_sites = (sites[1], sites[0])
             el_tag = "-".join(sorted(els))
             site_tag = "-".join([str(site) for site in sorted_sites])
             bond_length = cohp[bond_idx]["length"]
             if el_tag not in out:
                 out[el_tag] = {}
             out[el_tag][site_tag] = {
-                "cohp": {"1": {}, "-1": {}},
-                "icohp": {"-1": {}, "1": {}},
+                "cohp": {"1": list(np.zeros(len(energies))), "-1": list(np.zeros(len(energies)))},
+                "icohp": {"-1": list(np.zeros(len(energies))), "1": list(np.zeros(len(energies)))},
                 "length": bond_length,
             }
             out[el_tag][site_tag]["cohp"]["total"] = np.zeros(len(energies))
             out[el_tag][site_tag]["icohp"]["total"] = np.zeros(len(energies))
             for spin in cohp[bond_idx]["COHP"]:
                 if spin.name == "up":
                     spin_tag = "1"
@@ -743,24 +743,34 @@
             return None
 
         out = {"E": pcohp["E"]}
         for el_tag in pcohp:
             if el_tag == "E":
                 continue
             out[el_tag] = {}
-            out[el_tag]["cohp"] = np.zeros(len(out["E"]))
-            out[el_tag]["icohp"] = np.zeros(len(out["E"]))
+            tmp_cohp = np.zeros(len(out["E"]))
+            tmp_icohp = np.zeros(len(out["E"]))
             for site_tag in pcohp[el_tag]:
                 for spin in pcohp[el_tag][site_tag]["cohp"]:
-                    out[el_tag]["cohp"] += np.array(
-                        pcohp[el_tag][site_tag]["cohp"][spin]
-                    )
-                    out[el_tag]["icohp"] += np.array(
-                        pcohp[el_tag][site_tag]["cohp"][spin]
-                    )
+
+                    cohp_to_add = np.array(pcohp[el_tag][site_tag]["cohp"][spin])
+#                    print(cohp_to_add)
+                    if len(cohp_to_add) == len(tmp_cohp):
+                        tmp_cohp = np.add(cohp_to_add
+                                          , tmp_cohp
+                        )
+                    
+                    icohp_to_add = np.array(pcohp[el_tag][site_tag]["icohp"][spin])
+                    if len(icohp_to_add) == len(tmp_icohp):
+                        tmp_icohp = np.add(
+                            icohp_to_add, tmp_icohp
+                        )
+
+            out[el_tag]["cohp"] = tmp_cohp
+            out[el_tag]["icohp"] = tmp_icohp
 
         for el_tag in out:
             if el_tag == "E":
                 continue
             for key in ["cohp", "icohp"]:
                 tmp = out[el_tag][key]
                 out[el_tag][key] = list(tmp)
@@ -1302,136 +1312,7 @@
         # we'll map to a dictionary of {key : data for that key} for all keys
         out = {}
         for d in data:
             for key in d:
                 out[key] = d[key]
 
         return out
-
-
-def crawl_and_purge(
-    head_dir,
-    files_to_purge=[
-        "WAVECAR",
-        "CHGCAR",
-        "CHG",
-        "PROCAR",
-        "LOCPOT",
-        "AECCAR0",
-        "AECCAR1",
-        "AECCAR2",
-    ],
-    safety="on",
-    check_convergence=True,
-    verbose=False,
-):
-    """
-    Args:
-        head_dir (str) - directory to start crawling beneath
-        files_to_purge (list) - list of file names to purge
-        safety (str) - 'on' or 'off' to turn on/off safety
-            - if safety is on, won't actually delete files
-    """
-    purged_files = []
-    mem_created = 0
-    for subdir, dirs, files in os.walk(head_dir):
-        ready = False
-        if check_convergence:
-            if "POTCAR" in files:
-                av = AnalyzeVASP(subdir)
-                if av.is_converged:
-                    ready = True
-                else:
-                    ready = False
-            else:
-                ready = False
-        else:
-            ready = True
-        if ready:
-            for f in files:
-                if f in files_to_purge:
-                    path_to_f = os.path.join(subdir, f)
-                    if verbose:
-                        print(path_to_f)
-                    mem_created += os.stat(path_to_f).st_size
-                    purged_files.append(path_to_f)
-                    if safety == "off":
-                        os.remove(path_to_f)
-    if safety == "off":
-        print(
-            "You purged %i files, freeing up %.2f GB of memory"
-            % (len(purged_files), mem_created / 1e9)
-        )
-    if safety == "on":
-        print(
-            "You had the safety on\n If it were off, you would have purged %i files, freeing up %.2f GB of memory"
-            % (len(purged_files), mem_created / 1e9)
-        )
-
-def get_analysis_configs(
-    analyze_calculations_in_parallel=False,
-    analyze_structure=True,
-    analyze_mag=False,
-    analyze_charge=False,
-    analyze_dos=False,
-    analyze_bonding=False,
-    exclude=[],
-):
-    """
-
-    function for modifying analysis configs from the defaults (see *** for defaults)
-
-    Args:
-        analyze_calculations_in_parallel (bool or int): whether to analyze calculation results in parallel or not
-            False: use 1 processor
-            True: use all available processors
-            int: use that many processors
-        analyze_structure (bool, optional): True to include structure in your results
-        analyze_mag (bool, optional): True to include magnetization in your results
-        analyze_charge (bool, optional): True to include bader charge + lobster charges + madelung in your results
-        analyze_dos (bool, optional): True to include pdos, tdos in your results
-        analyze_bonding (bool, optional): True to include tcohp, pcohp, tcoop, pcoop, tcobi, pcobi in your results
-        exclude (list, optional): list of strings to exclude from analysis. Defaults to [].
-            - overwrites other options
-    Returns:
-        dictionary of ANALYSIS_CONFIGS
-            {'include_*' : True or False}
-    """
-
-    analysis_configs = {}
-
-    if not analyze_calculations_in_parallel:
-        n_procs = 1
-    else:
-        if analyze_calculations_in_parallel == True:
-            n_procs = multip.cpu_count() - 1
-        elif analyze_calculations_in_paralle == False:
-            n_procs = 1
-        else:
-            n_procs = analyze_calculations_in_parallel
-
-    analysis_configs["n_procs"] = n_procs
-
-    includes = []
-    if analyze_structure:
-        includes.append("structure")
-
-    if analyze_mag:
-        includes.append("mag")
-
-    if analyze_charge:
-        includes.extend(["charge", "madelung"])
-
-    if analyze_dos:
-        includes.extend(["tdos", "pdos"])
-
-    if analyze_bonding:
-        includes.extend(["tcohp", "pcohp", "tcoop", "pcoop", "tcobi", "pcobi"])
-
-    for include in includes:
-        analysis_configs["include_" + include] = True
-
-    if exclude:
-        for ex in exclude:
-            analysis_configs["include_" + ex] = False
-
-    return analysis_configs
```

### Comparing `pydmclab-1.0.0/pydmclab/hpc/launch.py` & `pydmclab-1.0.1/pydmclab/hpc/launch.py`

 * *Files 12% similar despite different names*

```diff
@@ -264,55 +264,7 @@
                                 perturbation
                             )
                             perturbed_structure.to(fmt="poscar", filename=fposcar)
                         else:
                             struc.to(fmt="poscar", filename=fposcar)
 
         return launch_dirs
-
-
-def get_launch_configs(
-    standards=["dmc"],
-    xcs=["metagga"],
-    use_mp_thermo_data=False,
-    n_afm_configs=0,
-    skip_xcs_for_standards={"mp": ["gga", "metagga"]},
-):
-    """
-
-    configs related to launching  chains of calculations
-
-    Args:
-        standards (list, optional): list of standards you'd like to calculate
-        xcs (list, optional): list of xcs you'd like to calculate for each standard
-        use_mp_thermo_data (bool, optional): True if you are going to use formation energies provided in Materials Project for phase stability analysis
-        n_afm_configs (int, optional): number of antiferromagnetic configurations to run for each structure (0 if you don't want to run AFM)
-        skip_xcs_for_standards (dict, optional): dictionary of xcs to skip for a given standard.
-            Defaults to {"mp": ["gga", "metagga"]}.
-                - e.g., we don't want to run GGA or MetaGGA MP calculations because MP uses GGA+U (for now)
-
-    Returns:
-        dictionary of launch configurations
-    """
-
-    launch_configs = {}
-
-    to_launch = {}
-
-    for standard in standards:
-        to_launch[standard] = xcs
-
-    if use_mp_thermo_data:
-        to_launch["mp"] = ["ggau"]
-
-    for standard in skip_xcs_for_standards:
-        for xc in skip_xcs_for_standards[standard]:
-            if xc in to_launch[standard]:
-                to_launch[standard].remove(xc)
-
-    launch_configs["to_launch"] = to_launch
-
-    launch_configs["compare_to_mp"] = use_mp_thermo_data
-
-    launch_configs["n_afm_configs"] = n_afm_configs
-
-    return launch_configs
```

### Comparing `pydmclab-1.0.0/pydmclab/hpc/submit.py` & `pydmclab-1.0.1/pydmclab/hpc/submit.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         magmom,
         user_configs={},
         refresh_configs=["vasp", "sub", "slurm"],
         vasp_configs_yaml=os.path.join(os.getcwd(), "_vasp_configs.yaml"),
         slurm_configs_yaml=os.path.join(os.getcwd(), "_slurm_configs.yaml"),
         sub_configs_yaml=os.path.join(os.getcwd(), "_sub_configs.yaml"),
     ):
-
         """
         Args:
             launch_dir (str) - directory to launch calculations from (to submit the submission file)
                 - assumes initial structure is POSCAR in launch_dir
                     - LaunchTools will put it there
                 - within this directory, various VASP calculation directories (calc_dirs) will be created
                         - gga-loose, gga-relax, gga-static, etc
@@ -257,67 +256,99 @@
         slurm_configs = self.slurm_configs.copy()
         options = {
             option: slurm_configs[option]
             for option in slurm_configs
             if slurm_configs[option]
         }
         partitions = self.partitions.copy()
-        partition_specs = partitions[options["partition"]]
+        if options["partition"] in partitions:
+            partition_specs = partitions[options["partition"]]
 
-        # make sure slurm_options align with partition configurations
-        if partition_specs["proc"] == "gpu":
-            options["nodes"] = 1
-            options["ntasks"] = 1
-            options["gres"] = "gpu:%s:%s" % (
-                options["partition"].split("-")[0],
-                str(options["nodes"]),
-            )
-        if not partition_specs["sharing"]:
-            options["ntasks"] = partition_specs["cores_per_node"]
+            # make sure slurm_options align with partition configurations
+            if partition_specs["proc"] == "gpu":
+                options["nodes"] = 1
+                options["ntasks"] = 1
+                options["gres"] = "gpu:%s:%s" % (
+                    options["partition"].split("-")[0],
+                    str(options["nodes"]),
+                )
+            if not partition_specs["sharing"]:
+                options["ntasks"] = partition_specs["cores_per_node"]
         return options
 
     @property
+    def bin_dir(self):
+        """
+        Returns bin directory where things (eg LOBSTER) are located
+        """
+        sub_configs = self.sub_configs.copy()
+        machine = sub_configs["machine"]
+        if machine == "msi":
+            return "/home/cbartel/shared/bin"
+        elif machine == "bridges2":
+            return "/ocean/projects/mat230011p/shared/bin"
+        elif machine == "expanse":
+            return "/home/%s/bin/" % os.getlogin()
+
+    @property
+    def vasp_dir(self):
+        """
+        Returns directory containing vasp executable
+        """
+        machine = self.sub_configs["machine"]
+        if machine == "msi":
+            return "%s/vasp" % self.bin_dir
+        elif machine == "bridges2":
+            return "/opt/packages/VASP/VASP6/6.3+VTST"
+        else:
+            raise NotImplementedError('dont have VASP path for machine "%s"' % machine)
+
+    @property
     def vasp_command(self):
         """
         Returns command used to execute vasp
             e.g., 'srun -n 24 PATH_TO_VASP/vasp_std > vasp.o'
         """
         sub_configs = self.sub_configs.copy()
         vasp_configs = self.vasp_configs.copy()
-        vasp_exec = os.path.join(sub_configs["vasp_dir"], sub_configs["vasp"])
+        vasp_exec = os.path.join(self.vasp_dir, sub_configs["vasp"])
+        slurm_options = self.slurm_options.copy()
+
         if sub_configs["mpi_command"] == "srun":
             return "\n%s --ntasks=%s --mpi=pmi2 %s > %s\n" % (
                 sub_configs["mpi_command"],
-                str(self.slurm_options["ntasks"]),
+                str(slurm_options["ntasks"]),
                 vasp_exec,
                 vasp_configs["fvaspout"],
             )
         elif sub_configs["mpi_command"] == "mpirun":
             return "\n%s -np=%s %s > %s\n" % (
                 sub_configs["mpi_command"],
-                str(self.slurm_options["ntasks"]),
+                str(slurm_options["ntasks"]),
                 vasp_exec,
                 vasp_configs["fvaspout"],
             )
 
     @property
     def lobster_command(self):
         """
         Returns command used to execute lobster
         """
-        lobster = "/home/cbartel/shared/bin/lobster/lobster-4.1.0/lobster-4.1.0"
-        return "\n%s\n" % lobster
+        lobster_path = os.path.join(
+            self.bin_dir, "lobster", "lobster-4.1.0", "lobster-4.1.0"
+        )
+        return "\n%s\n" % lobster_path
 
     @property
     def bader_command(self):
         """
         Returns command used to execute bader
         """
-        chgsum = "/home/cbartel/shared/bin/bader/chgsum.pl AECCAR0 AECCAR2"
-        bader = "/home/cbartel/shared/bin/bader/bader CHGCAR -ref CHGCAR_sum"
+        chgsum = "%s/bader/chgsum.pl AECCAR0 AECCAR2" % self.bin_dir
+        bader = "%s/bader/bader CHGCAR -ref CHGCAR_sum" % self.bin_dir
         return "\n%s\n%s\n" % (chgsum, bader)
 
     def is_job_in_queue(self, job_name):
         """
         Returns:
             True if this job-name is already in the queue, else False
 
@@ -464,14 +495,15 @@
 
                 # if parents + current calc are converged, give it status = done
                 if (
                     convergence
                     and parent_convergence
                     and not fresh_restart
                     and not large_E_diff_between_relax_and_static
+                    and not sub_configs["force_postprocess"]
                 ):
                     print("     %s is already converged; skipping" % xc_calc)
                     status = "done"
                     statuses[final_xc][xc_calc] = status
                     continue
 
                 # for jobs that are not DONE:
@@ -623,15 +655,18 @@
                     if slurm_option:
                         f.write(
                             "%s --%s=%s\n" % (queue_manager, key, str(slurm_option))
                         )
                 f.write("\n\n")
                 f.write("ulimit -s unlimited\n")
                 if sub_configs["mpi_command"] == "mpirun":
-                    f.write("module load impi/2018/release_multithread\n")
+                    if sub_configs["machine"] == "msi":
+                        f.write("module load impi/2018/release_multithread\n")
+                    elif sub_configs["machine"] == "bridges2":
+                        f.write("module load intelmpi\nexport OMP_NUM_THREADS=1\n")
                 # now write what is needed for the chain of VASP calcs + postprocessing
                 print("\n:::: writing sub now - %s ::::" % fsub)
 
                 # use this counter to figure if there are parents for a given calc and who those parents are
                 xc_calc_counter = -1
                 for xc_calc in packing[final_xc]:
                     # loop through the calculations that should be chained together for a given final_xc
@@ -648,20 +683,22 @@
                         if vasp_configs["lobster_static"]:
                             if calc_to_run == "static":
                                 if sub_configs[
                                     "force_postprocess"
                                 ] or not os.path.exists(
                                     os.path.join(calc_dir, "lobsterout")
                                 ):
+                                    f.write("cd %s\n" % calc_dir)
                                     f.write(self.lobster_command)
                                 if sub_configs[
                                     "force_postprocess"
                                 ] or not os.path.exists(
                                     os.path.join(calc_dir, "ACF.dat")
                                 ):
+                                    f.write("cd %s\n" % calc_dir)
                                     f.write(self.bader_command)
                         f.write("echo %s is done >> %s\n" % (xc_calc, fstatus))
                     else:
                         if status == "continue":
                             # copy the CONTCAR to the POSCAR
                             f.write(
                                 "cp %s %s\n"
@@ -749,15 +786,14 @@
         scripts_dir = os.getcwd()
         launch_dir = self.launch_dir
 
         # determine what keywords to look for to see if job needs to be launched
         flags_that_need_to_be_executed = self.sub_configs["execute_flags"]
 
         for final_xc in final_xcs:
-
             # identify the submission script for this chain
             fsub = os.path.join(launch_dir, "sub_%s.sh" % final_xc)
             with open(fsub) as f:
                 for line in f:
                     if "job-name" in line:
                         job_name = line[:-1].split("=")[-1]
             # see if jobs in queue
@@ -776,207 +812,13 @@
 
             # if we made it this far, launch it
             os.chdir(launch_dir)
             subprocess.call(["sbatch", "sub_%s.sh" % final_xc])
             os.chdir(scripts_dir)
 
 
-def get_sub_configs(
-    submit_calculations_in_parallel=False,
-    start_all_calculations_from_scratch=False,
-    rerun_lobster=False,
-    mpi_command="mpirun",
-    special_packing=False,
-):
-    """
-
-    configs related to preparing submission scripts and submitting VASP calculations
-        - see defaults in ***
-
-
-    Args:
-        submit_calculations_in_parallel (bool or int): whether to prepare submission scripts in parallel or not
-            False: use 1 processor
-            True: use all available processors
-            int: use that many processors
-
-        start_all_calculations_from_scratch (bool): if True, start all calculations over (ie delete all outputs)
-
-        rerun_lobster (bool) : if True, rerun lobster even if it has already been run
-
-        mpi_command (str): the command to use for mpi (eg mpirun, srun, etc)
-
-        special_packing (dict): if you want to change the loose --> relax --> static flow for some functional
-            e.g., {'metagga' : ['loose', 'static']}
-
-    Returns:
-        {config_name : config_value}
-
-    """
-    sub_configs = {}
-
-    if not submit_calculations_in_parallel:
-        n_procs = 1
-    else:
-        if submit_calculations_in_parallel == True:
-            n_procs = multip.cpu_count() - 1
-        elif submit_calculations_in_parallel == False:
-            n_procs = 1
-        else:
-            n_procs = submit_calculations_in_parallel
-
-    sub_configs["n_procs"] = n_procs
-
-    if start_all_calculations_from_scratch:
-        sub_configs["fresh_restart"] = True
-
-    if rerun_lobster:
-        sub_configs["force_postprocess"] = True
-
-    sub_configs["mpi_command"] = mpi_command
-
-    if special_packing:
-        sub_configs["packing"] = {}
-        for xc in special_packing:
-            sub_configs["packing"]["xc"] = special_packing[xc]
-
-    return sub_configs
-
-
-def get_slurm_configs(
-    total_nodes=1,
-    cores_per_node=32,
-    walltime_in_hours=23,
-    partition="msismall",
-    error_file="log.e",
-    output_file="log.o",
-    account="cbartel",
-):
-    """
-
-    how to modify slurm configurations for each VASP job (see *** for defaults)
-
-    Args:
-        total_nodes (int, optional): how many nodes to run each VASP job on
-        cores_per_node (int, optional): how many cores per node to use for each VASP job
-        walltime_in_hours (int, optional): how long to run each VASP job
-        partition (str, optional): what part of the cluster to run each VASP job on
-        error_file (str, optional): where to send each VASP job error
-        output_file (str, optional): where to send each VASP job output
-        account (str, optional): what account to charge for your VASP jobs
-
-    Returns:
-        {slurm config name : slurm config value}
-    """
-    slurm_configs = {}
-
-    slurm_configs["nodes"] = total_nodes
-    slurm_configs["ntasks"] = int(total_nodes * cores_per_node)
-
-    slurm_configs["time"] = int(walltime_in_hours * 60)
-
-    if total_nodes > 1:
-        if "small" in partition:
-            print("WARNING: cant use small partition on > 1 node; switching to large")
-        partition = partition.replace("small", "large")
-        slurm_configs["partition"] = partition
-
-    slurm_configs["error_file"] = error_file
-    slurm_configs["output_file"] = output_file
-    slurm_configs["account"] = account
-
-    if total_nodes > 4:
-        print("WARNING: are you sure you need more than 4 nodes??")
-
-    if (total_nodes > 1) and (cores_per_node < 32):
-        print("WARNING: this seems like a small job. are you sure you need > 1 node??")
-
-    return slurm_configs
-
-
-def get_vasp_configs(
-    run_lobster=False,
-    modify_loose_incar=False,
-    modify_relax_incar=False,
-    modify_static_incar=False,
-    modify_loose_kpoints=False,
-    modify_relax_kpoints=False,
-    modify_static_kpoints=False,
-    modify_loose_potcar=False,
-    modify_relax_potcar=False,
-    modify_static_potcar=False,
-):
-    """
-
-    how to modify VASP calculations from the defaults (see pydmclab.hpc.vasp for defaults)
-
-    Args:
-        run_lobster (bool, optional): True to run LOBSTER
-
-        modify_loose_incar (bool, optional):
-            - dictionary of {incar flag (str) : setting for that flag}
-            - modifies only the "loose" calculations
-        modify_relax_incar (bool, optional):
-            - dictionary of {incar flag (str) : setting for that flag}
-            - modifies only the "relax" calculations
-        modify_static_incar (bool, optional):
-            - dictionary of {incar flag (str) : setting for that flag}
-            - modifies only the "static" calculations
-
-
-        modify_loose_kpoints (bool, optional):
-            - dictionary of non-default K-point setting. see pydmclab.hpc.vasp for format
-            - modifies only the "loose" calculations
-        modify_relax_kpoints (bool, optional):
-            - dictionary of non-default K-point setting. see pydmclab.hpc.vasp for format
-            - modifies only the "relax" calculations
-        modify_static_kpoints (bool, optional):
-            - dictionary of non-default K-point setting. see pydmclab.hpc.vasp for format
-            - modifies only the "static" calculations
-
-
-        modify_loose_potcar (bool, optional):
-            - dictionary of non-default POTCAR in format {element (str) : POTCAR to use (str)}
-            - modifies only the "loose" calculations
-        modify_relax_potcar (bool, optional):
-            - dictionary of non-default POTCAR in format {element (str) : POTCAR to use (str)}
-            - modifies only the "loose" calculations
-        modify_static_potcar (bool, optional):
-            - dictionary of non-default POTCAR in format {element (str) : POTCAR to use (str)}
-            - modifies only the "static" calculations
-
-    Returns:
-        dictionary of VASP_CONFIGS
-    """
-    vasp_configs = {"lobster_static": run_lobster}
-
-    if modify_loose_incar:
-        vasp_configs["loose_incar"] = modify_loose_incar
-    if modify_relax_incar:
-        vasp_configs["relax_incar"] = modify_relax_incar
-    if modify_static_incar:
-        vasp_configs["static_incar"] = modify_static_incar
-
-    if modify_loose_kpoints:
-        vasp_configs["loose_kpoints"] = modify_loose_kpoints
-    if modify_relax_kpoints:
-        vasp_configs["relax_kpoints"] = modify_relax_kpoints
-    if modify_static_kpoints:
-        vasp_configs["static_kpoints"] = modify_static_kpoints
-
-    if modify_loose_potcar:
-        vasp_configs["loose_potcar"] = modify_loose_potcar
-    if modify_relax_potcar:
-        vasp_configs["relax_potcar"] = modify_relax_potcar
-    if modify_static_potcar:
-        vasp_configs["static_potcar"] = modify_static_potcar
-
-    return vasp_configs
-
-
 def main():
-
     return
 
 
 if __name__ == "__main__":
     sub = main()
```

### Comparing `pydmclab-1.0.0/pydmclab/utils/handy.py` & `pydmclab-1.0.1/pydmclab/utils/handy.py`

 * *Files 17% similar despite different names*

```diff
@@ -74,15 +74,14 @@
     if len(names_in_q) == 0:
         return False
     else:
         return True
 
 
 def make_project_tree():
-
     project_dir = os.getcwd()
     tree = {
         "dev": ["scripts", "data", "figures"],
         "results": ["scripts", "data", "figures"],
         "prep": ["notes", "background"],
         "products": ["drafts", "slides", "other"],
     }
@@ -94,30 +93,14 @@
                 os.makedirs(that_layer)
             freadme = os.path.join(that_layer, "README.md")
             if not os.path.exists(freadme):
                 with open(freadme, "w") as f:
                     f.write("This is a placeholder for the %s directory" % that_layer)
 
 
-def make_sub_for_launcher():
-    flauncher_sub = os.path.join(os.getcwd(), "sub_launcher.sh")
-    launch_job_name = "-".join([os.getcwd().split("/")[-2], "launcher"])
-    with open(flauncher_sub, "w") as f:
-        f.write("#!/bin/bash -l\n")
-        f.write("#SBATCH --nodes=1\n")
-        f.write("#SBATCH --ntasks=8\n")
-        f.write("#SBATCH --time=4:00:00\n")
-        f.write("#SBATCH --error=_log_launcher.e\n")
-        f.write("#SBATCH --output=_log_launcher.o\n")
-        f.write("#SBATCH --account=cbartel\n")
-        f.write("#SBATCH --job-name=%s\n" % launch_job_name)
-        f.write("#SBATCH --partition=msismall\n")
-        f.write("\npython launcher.py\n")
-
-
 def is_calc_valid(structure, standard, xc, calc, mag, magmom, mag_override):
     """
     Returns:
         True if calculation should be launched;
         False if some logic is violated
     """
```

### Comparing `pydmclab-1.0.0/pydmclab/utils/plotting.py` & `pydmclab-1.0.1/pydmclab/plotting/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,23 @@
-import matplotlib as mpl
+import os
+
 from pydmclab.data.plotting_configs import get_color_palettes
 
 
+from pydmclab.core.comp import CompTools
+from pydmclab.core.struc import StrucTools
+from pydmclab.utils.handy import read_json, write_json
+
+import matplotlib as mpl
+import matplotlib.pyplot as plt
+
+import numpy as np
+import random
+
+
 def get_colors(palette):
     """
 
     returns rgb colors that are nicer than matplotlibs defaults
 
     Args:
         palette (str):
@@ -22,14 +34,16 @@
 
         so, to use this you could do:
             from pydmc.utils.plotting import get_colors
             my_colors = get_colors('tab10')
             ax = plt.scatter(x, y, color=my_colors['blue'])
     """
     colors = get_color_palettes()[palette]
+    colors["black"] = (0, 0, 0)
+    colors["white"] = (1, 1, 1)
     return colors
 
 
 def set_rc_params():
     """
     Args:
 
@@ -57,7 +71,29 @@
         "ytick.right": True,
         "axes.edgecolor": "black",
         "figure.figsize": [6, 4],
     }
     for p in params:
         mpl.rcParams[p] = params[p]
     return params
+
+
+def get_label(cmpd, els):
+    """
+    Args:
+        cmpd (str) - chemical formula
+        els (list) - ordered list of elements (str) as you want them to appear in label
+
+    Returns:
+        neatly formatted chemical formula label
+    """
+    label = r"$"
+    for el in els:
+        amt = CompTools(cmpd).stoich(el)
+        if amt == 0:
+            continue
+        label += el
+        if amt == 1:
+            continue
+        label += "_{%s}" % amt
+    label += "$"
+    return label
```

### Comparing `pydmclab-1.0.0/pydmclab.egg-info/PKG-INFO` & `pydmclab-1.0.1/pydmclab.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydmclab
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package to facilitate DFT calculations and analysis
 Home-page: https://github.umn.edu/bartel-group/pydmclab
 Author: Chris Bartel
 Author-email: cbartel@umn.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pydmclab-1.0.0/pydmclab.egg-info/SOURCES.txt` & `pydmclab-1.0.1/pydmclab.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -11,59 +11,64 @@
 pydmclab/core/README.md
 pydmclab/core/__init__.py
 pydmclab/core/comp.py
 pydmclab/core/energies.py
 pydmclab/core/hulls.py
 pydmclab/core/mag.py
 pydmclab/core/query.py
+pydmclab/core/reactions.py
 pydmclab/core/struc.py
 pydmclab/data/.DS_Store
 pydmclab/data/README.md
 pydmclab/data/__init__.py
 pydmclab/data/configs.py
 pydmclab/data/features.py
 pydmclab/data/plotting_configs.py
 pydmclab/data/thermochem.py
 pydmclab/data/data/221220_dmc-mus.json
 pydmclab/data/data/230122_dmc-mus.json
+pydmclab/data/data/230614_dmc-mus.json
 pydmclab/data/data/_batch_vasp_analysis_configs.yaml
 pydmclab/data/data/_launch_configs.yaml
 pydmclab/data/data/_partition_configs.yaml
 pydmclab/data/data/_slurm_configs.yaml
 pydmclab/data/data/_sub_configs.yaml
 pydmclab/data/data/_vasp_configs.yaml
 pydmclab/data/data/atomic_masses.json
 pydmclab/data/data/bartel2019_npj_reference-energies.csv
 pydmclab/data/data/colors.json
 pydmclab/data/data/elemental_gibbs_energies_T.json
+pydmclab/data/data/gas_thermo_data_nist.json
 pydmclab/data/data/mus_from_bartel2019_npj.json
 pydmclab/data/data/mus_from_dmc_no_corrections.json
 pydmclab/data/data/mus_from_mp_no_corrections.json
 pydmclab/data/data/ssub.dat
 pydmclab/data/data/ssub.json
 pydmclab/demos/demo_comp.py
+pydmclab/demos/demo_energies.py
 pydmclab/demos/demo_hulls.py
 pydmclab/demos/demo_launcher_template.py
+pydmclab/demos/demo_mag.py
+pydmclab/demos/demo_plot_dos.py
 pydmclab/demos/demo_query.py
 pydmclab/demos/demo_struc.py
-pydmclab/demos/demo_vasp_template.py
-pydmclab/demos/demo_vasp_test-mp-chemsys.py
-pydmclab/demos/demo_vasp_test-template.py
-pydmclab/demos/demo_vasp_test-transform-strucs.py
-pydmclab/demos/demo_vasp_test-typical-dmc.py
-pydmclab/demos/tmp.png
 pydmclab/dev/Untitled-2.py
 pydmclab/dev/__init__.py
 pydmclab/dev/echem.py
 pydmclab/dev/entries.py
 pydmclab/dev/grand.py
-pydmclab/dev/reactions.py
+pydmclab/dev/mixing_pmg.py
+pydmclab/dev/query_new_mp_api.py
 pydmclab/hpc/README.md
 pydmclab/hpc/__init__.py
 pydmclab/hpc/analyze.py
+pydmclab/hpc/helpers.py
 pydmclab/hpc/launch.py
 pydmclab/hpc/submit.py
 pydmclab/hpc/vasp.py
+pydmclab/plotting/__init__.py
+pydmclab/plotting/dos.py
+pydmclab/plotting/pd.py
+pydmclab/plotting/utils.py
 pydmclab/utils/README.md
 pydmclab/utils/__init__.py
-pydmclab/utils/handy.py
-pydmclab/utils/plotting.py
+pydmclab/utils/handy.py
```

### Comparing `pydmclab-1.0.0/setup.py` & `pydmclab-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 NAME = "pydmclab"
 DESCRIPTION = "Package to facilitate DFT calculations and analysis"
 URL = "https://github.umn.edu/bartel-group/pydmclab"
 EMAIL = "cbartel@umn.edu"
 AUTHOR = "Chris Bartel"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 
 REQUIRED = ["numpy", "pymatgen"]
 EXTRAS = {}
 here = os.path.abspath(os.path.dirname(__file__))
 try:
     with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
         long_description = "\n" + f.read()
```

