# Comparing `tmp/wop-2.5.1.tar.gz` & `tmp/wop-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\rlafage\workspace\WhatsOpt-CLI\dist\.tmp-kffn7p5p\wop-2.5.1.tar", last modified: Mon Jun  5 19:32:20 2023, max compression
+gzip compressed data, was "D:\rlafage\workspace\WhatsOpt-CLI\dist\.tmp-oewp0oft\wop-2.5.2.tar", last modified: Tue Jun 27 13:05:59 2023, max compression
```

## Comparing `wop-2.5.1.tar` & `wop-2.5.2.tar`

### file list

```diff
@@ -1,37 +1,93 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 19:32:20.069787 wop-2.5.1/
--rw-rw-rw-   0        0        0    11558 2019-10-20 20:51:42.000000 wop-2.5.1/LICENSE
--rw-rw-rw-   0        0        0      851 2023-06-05 19:32:20.069787 wop-2.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1786 2021-05-16 20:10:24.000000 wop-2.5.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-05 19:32:20.069787 wop-2.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1481 2023-04-14 19:05:22.000000 wop-2.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 19:32:20.005787 wop-2.5.1/tests/
--rw-rw-rw-   0        0        0      517 2023-03-20 14:35:21.000000 wop-2.5.1/tests/test_convert_utils.py
--rw-rw-rw-   0        0        0      476 2022-06-10 09:28:53.000000 wop-2.5.1/tests/test_mooptimization.py
--rw-rw-rw-   0        0        0     2170 2023-03-20 14:35:21.000000 wop-2.5.1/tests/test_push_command.py
--rw-rw-rw-   0        0        0     2960 2023-03-20 14:35:21.000000 wop-2.5.1/tests/test_push_utils.py
--rw-rw-rw-   0        0        0     3452 2023-03-20 14:35:21.000000 wop-2.5.1/tests/test_upload_utils.py
--rw-rw-rw-   0        0        0     3872 2023-03-20 14:35:21.000000 wop-2.5.1/tests/test_utils.py
--rw-rw-rw-   0        0        0      350 2022-02-21 15:06:38.000000 wop-2.5.1/tests/test_whatsopt_client.py
--rw-rw-rw-   0        0        0     2108 2023-03-20 14:35:21.000000 wop-2.5.1/tests/test_wop.py
-drwxrwxrwx   0        0        0        0 2023-06-05 19:32:20.045788 wop-2.5.1/whatsopt/
--rw-rw-rw-   0        0        0       23 2023-06-05 19:22:39.000000 wop-2.5.1/whatsopt/__init__.py
--rw-rw-rw-   0        0        0     1493 2021-10-07 14:47:53.000000 wop-2.5.1/whatsopt/convert_utils.py
--rw-rw-rw-   0        0        0      502 2022-06-02 07:27:07.000000 wop-2.5.1/whatsopt/logging.py
--rw-rw-rw-   0        0        0     3186 2022-06-10 09:28:53.000000 wop-2.5.1/whatsopt/mooptimization.py
--rw-rw-rw-   0        0        0    11578 2023-03-20 14:35:21.000000 wop-2.5.1/whatsopt/optimization.py
--rw-rw-rw-   0        0        0      422 2023-06-05 19:01:08.000000 wop-2.5.1/whatsopt/publish_utils.py
--rw-rw-rw-   0        0        0    15185 2023-03-20 14:35:21.000000 wop-2.5.1/whatsopt/push_command.py
--rw-rw-rw-   0        0        0     5644 2023-03-19 12:20:40.000000 wop-2.5.1/whatsopt/push_utils.py
--rw-rw-rw-   0        0        0     1483 2021-06-21 11:38:00.000000 wop-2.5.1/whatsopt/show_utils.py
--rw-rw-rw-   0        0        0     7448 2022-06-29 16:15:18.000000 wop-2.5.1/whatsopt/upload_utils.py
--rw-rw-rw-   0        0        0     6025 2023-05-15 12:58:25.000000 wop-2.5.1/whatsopt/utils.py
--rw-rw-rw-   0        0        0    40617 2023-06-01 14:22:21.000000 wop-2.5.1/whatsopt/whatsopt_client.py
--rw-rw-rw-   0        0        0    13395 2023-06-05 19:01:08.000000 wop-2.5.1/whatsopt/wop.py
-drwxrwxrwx   0        0        0        0 2023-06-05 19:32:20.065788 wop-2.5.1/wop.egg-info/
--rw-rw-rw-   0        0        0      851 2023-06-05 19:32:19.000000 wop-2.5.1/wop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      719 2023-06-05 19:32:19.000000 wop-2.5.1/wop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 19:32:19.000000 wop-2.5.1/wop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-05 19:32:19.000000 wop-2.5.1/wop.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      131 2023-06-05 19:32:19.000000 wop-2.5.1/wop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 19:32:19.000000 wop-2.5.1/wop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2019-12-02 13:07:07.000000 wop-2.5.1/wop.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.395113 wop-2.5.2/
+drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.194065 wop-2.5.2/.github/
+drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.215066 wop-2.5.2/.github/workflows/
+-rw-rw-rw-   0        0        0      729 2023-06-27 09:24:47.000000 wop-2.5.2/.github/workflows/publish.yml
+-rw-rw-rw-   0        0        0      926 2023-06-27 09:48:35.000000 wop-2.5.2/.github/workflows/tests.yml
+-rw-rw-rw-   0        0        0     1395 2022-08-17 14:04:44.000000 wop-2.5.2/.gitignore
+-rw-rw-rw-   0        0        0     9757 2023-06-27 09:01:10.000000 wop-2.5.2/CHANGELOG
+-rw-rw-rw-   0        0        0    11558 2019-10-20 20:51:42.000000 wop-2.5.2/LICENSE
+-rw-rw-rw-   0        0        0     2786 2023-06-27 13:05:59.394115 wop-2.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1786 2021-05-16 20:10:24.000000 wop-2.5.2/README.md
+-rw-rw-rw-   0        0        0     1538 2023-06-27 13:05:42.000000 wop-2.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 13:05:59.395113 wop-2.5.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.231068 wop-2.5.2/tests/
+drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.291598 wop-2.5.2/tests/data/
+-rw-rw-rw-   0        0        0     1004 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/disc1.py
+-rw-rw-rw-   0        0        0      650 2022-01-28 17:02:42.000000 wop-2.5.2/tests/data/disc1_base.py
+-rw-rw-rw-   0        0        0      114 2021-05-16 16:24:08.000000 wop-2.5.2/tests/data/disc1_problem.py
+-rw-rw-rw-   0        0        0      758 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/fonctions_base.py
+-rw-rw-rw-   0        0        0      334 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/mda_init.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.320129 wop-2.5.2/tests/data/multipoint_beam/
+-rw-rw-rw-   0        0        0       78 2020-06-08 09:44:01.000000 wop-2.5.2/tests/data/multipoint_beam/__init__.py
+-rw-rw-rw-   0        0        0      918 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/i_comp.py
+-rw-rw-rw-   0        0        0      603 2022-01-28 17:02:42.000000 wop-2.5.2/tests/data/multipoint_beam/i_comp_base.py
+-rw-rw-rw-   0        0        0      933 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/interp.py
+-rw-rw-rw-   0        0        0      619 2022-01-28 17:02:42.000000 wop-2.5.2/tests/data/multipoint_beam/interp_base.py
+-rw-rw-rw-   0        0        0     1111 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/local_stiffness_matrix_comp.py
+-rw-rw-rw-   0        0        0      671 2022-01-28 17:02:42.000000 wop-2.5.2/tests/data/multipoint_beam/local_stiffness_matrix_comp_base.py
+-rw-rw-rw-   0        0        0     1656 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/multipoint_beam_group.py
+-rw-rw-rw-   0        0        0     4093 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/multipoint_beam_group_base.py
+-rw-rw-rw-   0        0        0     1070 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/obj_sum.py
+-rw-rw-rw-   0        0        0      683 2022-01-28 17:02:42.000000 wop-2.5.2/tests/data/multipoint_beam/obj_sum_base.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.327112 wop-2.5.2/tests/data/multipoint_beam/parallel/
+-rw-rw-rw-   0        0        0       78 2020-06-08 09:44:01.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/__init__.py
+-rw-rw-rw-   0        0        0     1692 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/parallel.py
+-rw-rw-rw-   0        0        0     2296 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/parallel_base.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.346114 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/
+-rw-rw-rw-   0        0        0       78 2020-06-08 09:44:01.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/__init__.py
+-rw-rw-rw-   0        0        0     1406 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/compliance_comp.py
+-rw-rw-rw-   0        0        0      765 2022-01-28 17:02:42.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/compliance_comp_base.py
+-rw-rw-rw-   0        0        0     1391 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/displacements_comp.py
+-rw-rw-rw-   0        0        0      760 2022-01-28 17:02:42.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/displacements_comp_base.py
+-rw-rw-rw-   0        0        0     1107 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/states_comp.py
+-rw-rw-rw-   0        0        0    11260 2022-01-28 17:02:42.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/states_comp_base.py
+-rw-rw-rw-   0        0        0     1645 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/sub0.py
+-rw-rw-rw-   0        0        0     2677 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/parallel/sub0/sub0_base.py
+-rw-rw-rw-   0        0        0      446 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/run_analysis.py
+-rw-rw-rw-   0        0        0      381 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/run_parameters_init.py
+-rw-rw-rw-   0        0        0      971 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/multipoint_beam/volume_comp.py
+-rw-rw-rw-   0        0        0      622 2022-01-28 17:02:42.000000 wop-2.5.2/tests/data/multipoint_beam/volume_comp_base.py
+-rw-rw-rw-   0        0        0    21993 2020-09-09 21:57:34.000000 wop-2.5.2/tests/data/multipoint_beam_group_d0.json
+-rw-rw-rw-   0        0        0    10911 2020-09-09 21:57:28.000000 wop-2.5.2/tests/data/multipoint_beam_group_d1.json
+-rw-rw-rw-   0        0        0    17820 2020-09-09 21:57:31.000000 wop-2.5.2/tests/data/multipoint_beam_group_d2.json
+-rw-rw-rw-   0        0        0      222 2023-03-20 14:35:21.000000 wop-2.5.2/tests/data/run_mda.py
+-rw-rw-rw-   0        0        0      161 2020-03-10 17:19:07.000000 wop-2.5.2/tests/data/sellar.py
+-rw-rw-rw-   0        0        0     3224 2020-03-10 17:19:07.000000 wop-2.5.2/tests/data/test_doe.csv
+-rw-rw-rw-   0        0        0   161472 2021-07-21 12:19:20.000000 wop-2.5.2/tests/data/test_doe.hdf5
+-rw-rw-rw-   0        0        0    98304 2020-06-08 09:44:01.000000 wop-2.5.2/tests/data/test_doe.sqlite
+-rw-rw-rw-   0        0        0    98304 2020-06-08 09:44:01.000000 wop-2.5.2/tests/data/test_parallel_doe.sqlite_0
+-rw-rw-rw-   0        0        0    98304 2020-06-08 09:44:01.000000 wop-2.5.2/tests/data/test_parallel_doe.sqlite_1
+-rw-rw-rw-   0        0        0    98304 2020-06-08 09:44:01.000000 wop-2.5.2/tests/data/test_parallel_doe.sqlite_2
+-rw-rw-rw-   0        0        0     3779 2020-06-08 09:44:01.000000 wop-2.5.2/tests/data/test_push_cut_flatten.json
+-rw-rw-rw-   0        0        0      222 2022-02-21 15:06:38.000000 wop-2.5.2/tests/data/wop_format_v1
+-rw-rw-rw-   0        0        0      254 2022-02-21 15:06:38.000000 wop-2.5.2/tests/data/wop_format_v2
+-rw-rw-rw-   0        0        0      394 2022-02-21 15:06:38.000000 wop-2.5.2/tests/data/wop_ref
+-rw-rw-rw-   0        0        0      517 2023-03-20 14:35:21.000000 wop-2.5.2/tests/test_convert_utils.py
+-rw-rw-rw-   0        0        0      476 2022-06-10 09:28:53.000000 wop-2.5.2/tests/test_mooptimization.py
+-rw-rw-rw-   0        0        0     2170 2023-03-20 14:35:21.000000 wop-2.5.2/tests/test_push_command.py
+-rw-rw-rw-   0        0        0     2960 2023-03-20 14:35:21.000000 wop-2.5.2/tests/test_push_utils.py
+-rw-rw-rw-   0        0        0     3452 2023-03-20 14:35:21.000000 wop-2.5.2/tests/test_upload_utils.py
+-rw-rw-rw-   0        0        0     3872 2023-03-20 14:35:21.000000 wop-2.5.2/tests/test_utils.py
+-rw-rw-rw-   0        0        0      350 2022-02-21 15:06:38.000000 wop-2.5.2/tests/test_whatsopt_client.py
+-rw-rw-rw-   0        0        0     2108 2023-03-20 14:35:21.000000 wop-2.5.2/tests/test_wop.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.376113 wop-2.5.2/whatsopt/
+-rw-rw-rw-   0        0        0       23 2023-06-27 09:48:35.000000 wop-2.5.2/whatsopt/__init__.py
+-rw-rw-rw-   0        0        0     1493 2021-10-07 14:47:53.000000 wop-2.5.2/whatsopt/convert_utils.py
+-rw-rw-rw-   0        0        0      502 2022-06-02 07:27:07.000000 wop-2.5.2/whatsopt/logging.py
+-rw-rw-rw-   0        0        0     3186 2022-06-10 09:28:53.000000 wop-2.5.2/whatsopt/mooptimization.py
+-rw-rw-rw-   0        0        0    11578 2023-03-20 14:35:21.000000 wop-2.5.2/whatsopt/optimization.py
+-rw-rw-rw-   0        0        0      422 2023-06-05 19:01:08.000000 wop-2.5.2/whatsopt/publish_utils.py
+-rw-rw-rw-   0        0        0    15185 2023-03-20 14:35:21.000000 wop-2.5.2/whatsopt/push_command.py
+-rw-rw-rw-   0        0        0     5644 2023-03-19 12:20:40.000000 wop-2.5.2/whatsopt/push_utils.py
+-rw-rw-rw-   0        0        0     1483 2021-06-21 11:38:00.000000 wop-2.5.2/whatsopt/show_utils.py
+-rw-rw-rw-   0        0        0     7448 2022-06-29 16:15:18.000000 wop-2.5.2/whatsopt/upload_utils.py
+-rw-rw-rw-   0        0        0     6025 2023-05-15 12:58:25.000000 wop-2.5.2/whatsopt/utils.py
+-rw-rw-rw-   0        0        0    40787 2023-06-27 09:01:10.000000 wop-2.5.2/whatsopt/whatsopt_client.py
+-rw-rw-rw-   0        0        0    13395 2023-06-05 19:01:08.000000 wop-2.5.2/whatsopt/wop.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:05:59.392113 wop-2.5.2/wop.egg-info/
+-rw-rw-rw-   0        0        0     2786 2023-06-27 13:05:58.000000 wop-2.5.2/wop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2738 2023-06-27 13:05:59.000000 wop-2.5.2/wop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 13:05:58.000000 wop-2.5.2/wop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-27 13:05:58.000000 wop-2.5.2/wop.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      146 2023-06-27 13:05:58.000000 wop-2.5.2/wop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-27 13:05:58.000000 wop-2.5.2/wop.egg-info/top_level.txt
```

### Comparing `wop-2.5.1/LICENSE` & `wop-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wop-2.5.1/README.md` & `wop-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `wop-2.5.1/setup.py` & `wop-2.5.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,60 @@
-"""
-Author: Remi Lafage <remi.lafage@onera.fr>
+[build-system]
+requires = ["setuptools", "setuptools-scm"]
+build-backend = "setuptools.build_meta"
 
-This package is distributed under Apache 2 license.
-"""
+[tools.setuptools-scm]
 
-from setuptools import setup
-from whatsopt import __version__
+[tool.setuptools]
+packages = ["whatsopt"]
 
-CLASSIFIERS = """
-Development Status :: 5 - Production/Stable
-Intended Audience :: Science/Research
-Intended Audience :: Developers
-License :: OSI Approved :: Apache Software License
-Programming Language :: Python :: 3
-Topic :: Software Development
-Topic :: Scientific/Engineering
-Operating System :: Microsoft :: Windows
-Operating System :: Unix
-Operating System :: MacOS
-"""
-
-metadata = dict(
-    name="wop",
-    version=__version__,
-    description="WhatsOpt web application command line client",
-    author="Rémi Lafage",
-    author_email="remi.lafage@onera.fr",
-    license="Apache License, Version 2.0",
-    classifiers=[_f for _f in CLASSIFIERS.split("\n") if _f],
-    packages=["whatsopt"],
-    install_requires=[
-        "build",
-        "click>=6.7",
-        "openmdao>=3.4.0",
-        "openmdao_extensions>=1.2.0",
-        "packaging",
-        "pkginfo",
-        "requests",
-        "tabulate>=0.8.2",
-        "tomli",
-        "tomli-w",
-        "xdsmjs>=1.0.0",
-    ],
-    python_requires=">=3.7",
-    entry_points="""
-        [console_scripts]
-        wop=whatsopt.wop:wop
-    """,
-    zip_safe=True,
-    url="https://github.com/OneraHub/WhatsOpt-CLI",
-    download_url="https://github.com/OneraHub/WhatsOpt-CLI/releases",
-)
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
 
-setup(**metadata)
```

### Comparing `wop-2.5.1/tests/test_convert_utils.py` & `wop-2.5.2/tests/test_convert_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.1/tests/test_push_command.py` & `wop-2.5.2/tests/test_push_command.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.1/tests/test_push_utils.py` & `wop-2.5.2/tests/test_push_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.1/tests/test_upload_utils.py` & `wop-2.5.2/tests/test_upload_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.1/tests/test_utils.py` & `wop-2.5.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.1/tests/test_wop.py` & `wop-2.5.2/tests/test_wop.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.1/whatsopt/convert_utils.py` & `wop-2.5.2/whatsopt/convert_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.1/whatsopt/mooptimization.py` & `wop-2.5.2/whatsopt/mooptimization.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.1/whatsopt/optimization.py` & `wop-2.5.2/whatsopt/optimization.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.1/whatsopt/push_command.py` & `wop-2.5.2/whatsopt/push_command.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.1/whatsopt/push_utils.py` & `wop-2.5.2/whatsopt/push_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.1/whatsopt/show_utils.py` & `wop-2.5.2/whatsopt/show_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.1/whatsopt/upload_utils.py` & `wop-2.5.2/whatsopt/upload_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.1/whatsopt/utils.py` & `wop-2.5.2/whatsopt/utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.5.1/whatsopt/whatsopt_client.py` & `wop-2.5.2/whatsopt/whatsopt_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -948,16 +948,17 @@
                     fd.write(chunk)
                 name = fd.name
             zipf = zipfile.ZipFile(name, "r")
             tempdir = tempfile.mkdtemp(suffix="wop", dir=tempfile.tempdir)
             zipf.extractall(tempdir)
             filenames = zipf.namelist()
             if not filenames:
-                warn(f"No package found for Analysis #{source_id}")
-                log("Nothing to do")
+                warn(
+                    f"Fetching but no package found for analysis #{source_id}, nothing to do"
+                )
                 return
             zipf.close()
 
             file_to_move = {}
             for f in filenames:
                 file_to = f
                 file_to_move[file_to] = True
@@ -975,22 +976,25 @@
                         file_to_move[file_to] = False
                 else:
                     log(f"Fetch {file_to}")
             if not options.get("--dry-run"):
                 move_files(file_to_move, tempdir)
                 info(f"Analysis #{source_id} disciplines fetched")
         else:
-            error(f"Error while fetching disciplines of Analysis #{source_id}")
+            error(f"Error while fetching disciplines of analysis #{source_id}")
             error(resp.json().get("message"))
 
     def merge(self, source_id, options={}):
         if not is_package_mode():
             error("Package mode is required!")
             exit(-1)
         current_id = get_analysis_id()
+        if int(source_id) == current_id:
+            warn(f"Merging analysis #{current_id} in itself, nothing to do")
+            return
         url = self.endpoint(f"/api/v1/analyses/{current_id}")
         params = {
             "analysis": {
                 "import": {"analysis": source_id},
             },
             "requested_at": str(datetime.now()),
         }
@@ -1001,26 +1005,26 @@
             log(f"Analysis #{source_id} #{resp.json()} is selected to be merged")
         else:
             resp = self.session.put(url, headers=self.headers, json=params)
         if resp.ok:
             if not options.get("--dry-run"):
                 info(f"Analysis #{source_id} merged")
         elif resp.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-            error(f"Error while merging Analysis #{source_id}.")
+            error(f"Error while merging analysis #{source_id}.")
             error(
                 f"    Check analyses, maybe they are not compatible (same variable produced by different disciplines)"
             )
         elif resp.status_code == HTTPStatus.FORBIDDEN:
-            error(f"Error while merging Analysis #{source_id}.")
+            error(f"Error while merging analysis #{source_id}.")
             error(
                 f"    You are not authorized to update the current analysis: either you do not own it or"
                 f" current analysis is already packaged or operated"
             )
         else:
-            error(f"Error while merging Analysis #{source_id}")
+            error(f"Error while merging analysis #{source_id}")
             resp.raise_for_status()
 
     def pull_source_mda(self, source_id, options={}):
         self.merge(source_id, options)
         self.fetch(source_id, options)
         self._update_mda_base(options.get("--dry-run"))
```

### Comparing `wop-2.5.1/whatsopt/wop.py` & `wop-2.5.2/whatsopt/wop.py`

 * *Files identical despite different names*

