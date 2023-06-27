# Comparing `tmp/nonos-0.7.3.tar.gz` & `tmp/nonos-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/wafflarg/nonos/dist/.tmp-o0uadfk3/nonos-0.7.3.tar", last modified: Thu Mar  9 14:39:28 2023, max compression
+gzip compressed data, was "/home/wafflarg/nonos/dist/.tmp-q9slxm44/nonos-0.9.0.tar", last modified: Tue Jun 27 15:38:07 2023, max compression
```

## Comparing `nonos-0.7.3.tar` & `nonos-0.9.0.tar`

### file list

```diff
@@ -1,74 +1,73 @@
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-03-09 14:39:28.782822 nonos-0.7.3/
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-03-09 14:39:28.714822 nonos-0.7.3/.github/
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-03-09 14:39:28.714822 nonos-0.7.3/.github/workflows/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     2992 2023-03-09 13:44:29.000000 nonos-0.7.3/.github/workflows/ci.yml
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      749 2023-03-08 16:19:23.000000 nonos-0.7.3/.pre-commit-config.yaml
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    35149 2021-03-19 13:34:53.000000 nonos-0.7.3/LICENSE
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    10802 2023-03-09 14:39:28.782822 nonos-0.7.3/PKG-INFO
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    10228 2023-03-09 13:44:29.000000 nonos-0.7.3/README.md
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-03-09 14:39:28.718822 nonos-0.7.3/nonos/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       37 2023-02-02 16:13:06.000000 nonos-0.7.3/nonos/__init__.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       73 2021-12-17 15:56:12.000000 nonos-0.7.3/nonos/__main__.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       22 2023-03-09 13:44:29.000000 nonos-0.7.3/nonos/__version__.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     2362 2023-02-08 18:06:57.000000 nonos-0.7.3/nonos/_mpl_utils.py
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-03-09 14:39:28.718822 nonos-0.7.3/nonos/api/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      365 2023-03-09 13:44:29.000000 nonos-0.7.3/nonos/api/__init__.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    20614 2022-11-16 09:58:36.000000 nonos-0.7.3/nonos/api/_adapt_clm_vtk.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    60485 2023-03-08 16:19:23.000000 nonos-0.7.3/nonos/api/analysis.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    31352 2023-03-08 16:19:23.000000 nonos-0.7.3/nonos/api/from_simulation.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     7444 2023-03-09 13:44:29.000000 nonos-0.7.3/nonos/api/satellite.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      438 2022-11-21 14:54:36.000000 nonos-0.7.3/nonos/api/tools.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1392 2022-11-21 14:54:36.000000 nonos-0.7.3/nonos/config.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      111 2023-03-09 13:44:29.000000 nonos-0.7.3/nonos/default.mplstyle
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1031 2023-02-02 16:13:06.000000 nonos-0.7.3/nonos/logging.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1765 2021-12-17 15:56:12.000000 nonos-0.7.3/nonos/logo.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    17499 2023-03-08 16:19:23.000000 nonos-0.7.3/nonos/main.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     2335 2022-11-21 14:54:36.000000 nonos-0.7.3/nonos/parsing.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        0 2022-11-21 14:54:36.000000 nonos-0.7.3/nonos/py.typed
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     2004 2023-03-09 13:44:29.000000 nonos-0.7.3/nonos/styling.py
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-03-09 14:39:28.718822 nonos-0.7.3/nonos.egg-info/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    10802 2023-03-09 14:39:28.000000 nonos-0.7.3/nonos.egg-info/PKG-INFO
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1713 2023-03-09 14:39:28.000000 nonos-0.7.3/nonos.egg-info/SOURCES.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        1 2023-03-09 14:39:28.000000 nonos-0.7.3/nonos.egg-info/dependency_links.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       42 2023-03-09 14:39:28.000000 nonos-0.7.3/nonos.egg-info/entry_points.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      165 2023-03-09 14:39:28.000000 nonos-0.7.3/nonos.egg-info/requires.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        6 2023-03-09 14:39:28.000000 nonos-0.7.3/nonos.egg-info/top_level.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1858 2023-03-09 13:44:29.000000 nonos-0.7.3/pyproject.toml
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       38 2023-03-09 14:39:28.782822 nonos-0.7.3/setup.cfg
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-03-09 14:39:28.722822 nonos-0.7.3/tests/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      670 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/conftest.py
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-03-09 14:39:28.714822 nonos-0.7.3/tests/data/
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-03-09 14:39:28.726822 nonos-0.7.3/tests/data/fargo3d_planet2d/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     5525 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/data/fargo3d_planet2d/domain_x.dat
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     5523 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/data/fargo3d_planet2d/domain_y.dat
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       42 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/data/fargo3d_planet2d/domain_z.dat
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   524289 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/data/fargo3d_planet2d/gasdens0.dat
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   524288 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/data/fargo3d_planet2d/gasdens40.dat
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   524288 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/data/fargo3d_planet2d/gasvy40.dat
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      263 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/data/fargo3d_planet2d/myplanet.cfg
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     7886 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/data/fargo3d_planet2d/planet0.dat
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1014 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/data/fargo3d_planet2d/variables.par
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-03-09 14:39:28.730822 nonos-0.7.3/tests/data/idefix_newvtk_planet2d/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   298359 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/data/idefix_newvtk_planet2d/data.0000.vtk
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   298359 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/data/idefix_newvtk_planet2d/data.0023.vtk
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1007 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/data/idefix_newvtk_planet2d/idefix.ini
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     3717 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/data/idefix_newvtk_planet2d/planet0.dat
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-03-09 14:39:28.770822 nonos-0.7.3/tests/data/idefix_planet3d/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)  7490113 2021-03-30 18:17:30.000000 nonos-0.7.3/tests/data/idefix_planet3d/data.0000.vtk
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)  7490113 2021-03-30 18:22:00.000000 nonos-0.7.3/tests/data/idefix_planet3d/data.0043.vtk
--rwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)      213 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/data/idefix_planet3d/definitions.hpp
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      805 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/data/idefix_planet3d/idefix.ini
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    11155 2021-03-30 18:24:51.000000 nonos-0.7.3/tests/data/idefix_planet3d/planet0.dat
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-03-09 14:39:28.782822 nonos-0.7.3/tests/data/idefix_rwi/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)  1579289 2021-04-12 13:19:18.000000 nonos-0.7.3/tests/data/idefix_rwi/data.0000.vtk
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)  1579289 2021-04-12 13:19:18.000000 nonos-0.7.3/tests/data/idefix_rwi/data.0001.vtk
--rwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)      213 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/data/idefix_rwi/definitions.hpp
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      543 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/data/idefix_rwi/idefix.ini
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     3260 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/test_cli.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      261 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/test_errors.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1631 2023-02-02 16:13:07.000000 nonos-0.7.3/tests/test_image_comp.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1449 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/test_load_config.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      763 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/test_params_usage.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     3764 2022-11-21 14:54:36.000000 nonos-0.7.3/tests/test_parsing.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     5863 2023-03-08 16:19:23.000000 nonos-0.7.3/tests/test_plotting.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      604 2023-02-08 18:05:36.000000 nonos-0.7.3/tests/test_readme.py
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.902330 nonos-0.9.0/
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.882331 nonos-0.9.0/.github/
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.882331 nonos-0.9.0/.github/workflows/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     2992 2023-03-09 13:44:29.000000 nonos-0.9.0/.github/workflows/ci.yml
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      749 2023-05-31 10:33:03.000000 nonos-0.9.0/.pre-commit-config.yaml
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    35149 2021-03-19 13:34:53.000000 nonos-0.9.0/LICENSE
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    11036 2023-06-27 15:38:07.902330 nonos-0.9.0/PKG-INFO
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    10462 2023-06-13 13:00:11.000000 nonos-0.9.0/README.md
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.882331 nonos-0.9.0/nonos/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       37 2023-02-02 16:13:06.000000 nonos-0.9.0/nonos/__init__.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       73 2021-12-17 15:56:12.000000 nonos-0.9.0/nonos/__main__.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       22 2023-06-27 15:37:20.000000 nonos-0.9.0/nonos/__version__.py
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.886330 nonos-0.9.0/nonos/api/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      365 2023-03-09 13:44:29.000000 nonos-0.9.0/nonos/api/__init__.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    20614 2022-11-16 09:58:36.000000 nonos-0.9.0/nonos/api/_adapt_clm_vtk.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    61648 2023-06-27 07:49:11.000000 nonos-0.9.0/nonos/api/analysis.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    31352 2023-03-08 16:19:23.000000 nonos-0.9.0/nonos/api/from_simulation.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     7346 2023-06-27 08:45:04.000000 nonos-0.9.0/nonos/api/satellite.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      438 2022-11-21 14:54:36.000000 nonos-0.9.0/nonos/api/tools.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1392 2022-11-21 14:54:36.000000 nonos-0.9.0/nonos/config.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      111 2023-03-09 13:44:29.000000 nonos-0.9.0/nonos/default.mplstyle
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1031 2023-02-02 16:13:06.000000 nonos-0.9.0/nonos/logging.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1765 2021-12-17 15:56:12.000000 nonos-0.9.0/nonos/logo.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    17408 2023-06-27 08:45:04.000000 nonos-0.9.0/nonos/main.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     2335 2022-11-21 14:54:36.000000 nonos-0.9.0/nonos/parsing.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        0 2022-11-21 14:54:36.000000 nonos-0.9.0/nonos/py.typed
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     2004 2023-03-09 13:44:29.000000 nonos-0.9.0/nonos/styling.py
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.882331 nonos-0.9.0/nonos.egg-info/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    11036 2023-06-27 15:38:07.000000 nonos-0.9.0/nonos.egg-info/PKG-INFO
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1693 2023-06-27 15:38:07.000000 nonos-0.9.0/nonos.egg-info/SOURCES.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        1 2023-06-27 15:38:07.000000 nonos-0.9.0/nonos.egg-info/dependency_links.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       42 2023-06-27 15:38:07.000000 nonos-0.9.0/nonos.egg-info/entry_points.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      165 2023-06-27 15:38:07.000000 nonos-0.9.0/nonos.egg-info/requires.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        6 2023-06-27 15:38:07.000000 nonos-0.9.0/nonos.egg-info/top_level.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     2057 2023-06-27 08:45:04.000000 nonos-0.9.0/pyproject.toml
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       38 2023-06-27 15:38:07.902330 nonos-0.9.0/setup.cfg
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.886330 nonos-0.9.0/tests/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      686 2023-06-26 16:17:24.000000 nonos-0.9.0/tests/conftest.py
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.882331 nonos-0.9.0/tests/data/
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.886330 nonos-0.9.0/tests/data/fargo3d_planet2d/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     5525 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/fargo3d_planet2d/domain_x.dat
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     5523 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/fargo3d_planet2d/domain_y.dat
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       42 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/fargo3d_planet2d/domain_z.dat
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   524289 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/fargo3d_planet2d/gasdens0.dat
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   524288 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/fargo3d_planet2d/gasdens40.dat
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   524288 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/fargo3d_planet2d/gasvy40.dat
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      263 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/fargo3d_planet2d/myplanet.cfg
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     7886 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/fargo3d_planet2d/planet0.dat
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1014 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/fargo3d_planet2d/variables.par
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.886330 nonos-0.9.0/tests/data/idefix_newvtk_planet2d/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   298359 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/idefix_newvtk_planet2d/data.0000.vtk
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   298359 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/idefix_newvtk_planet2d/data.0023.vtk
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1007 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/idefix_newvtk_planet2d/idefix.ini
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     3717 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/idefix_newvtk_planet2d/planet0.dat
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.898331 nonos-0.9.0/tests/data/idefix_planet3d/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)  7490113 2021-03-30 18:17:30.000000 nonos-0.9.0/tests/data/idefix_planet3d/data.0000.vtk
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)  7490113 2021-03-30 18:22:00.000000 nonos-0.9.0/tests/data/idefix_planet3d/data.0043.vtk
+-rwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)      213 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/idefix_planet3d/definitions.hpp
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      805 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/idefix_planet3d/idefix.ini
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    11155 2021-03-30 18:24:51.000000 nonos-0.9.0/tests/data/idefix_planet3d/planet0.dat
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.898331 nonos-0.9.0/tests/data/idefix_rwi/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)  1579289 2021-04-12 13:19:18.000000 nonos-0.9.0/tests/data/idefix_rwi/data.0000.vtk
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)  1579289 2021-04-12 13:19:18.000000 nonos-0.9.0/tests/data/idefix_rwi/data.0001.vtk
+-rwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)      213 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/idefix_rwi/definitions.hpp
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      543 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/idefix_rwi/idefix.ini
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     3260 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/test_cli.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      253 2023-06-26 16:17:24.000000 nonos-0.9.0/tests/test_errors.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1631 2023-02-02 16:13:07.000000 nonos-0.9.0/tests/test_image_comp.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1449 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/test_load_config.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      763 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/test_params_usage.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     3541 2023-06-26 16:17:24.000000 nonos-0.9.0/tests/test_parsing.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     5791 2023-06-27 08:45:04.000000 nonos-0.9.0/tests/test_plotting.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      604 2023-02-08 18:05:36.000000 nonos-0.9.0/tests/test_readme.py
```

### Comparing `nonos-0.7.3/.github/workflows/ci.yml` & `nonos-0.9.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/.pre-commit-config.yaml` & `nonos-0.9.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -10,27 +10,27 @@
   - id: debug-statements
   - id: check-merge-conflict
   - id: trailing-whitespace
   - id: end-of-file-fixer
   - id: check-toml
 
 - repo: https://github.com/neutrinoceros/inifix.git
-  rev: v4.0.0
+  rev: v4.3.2
   hooks:
   - id: inifix-format
 
 - repo: https://github.com/psf/black
-  rev: 23.1.0
+  rev: 23.3.0
   hooks:
   - id: black
 
 - repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: v0.0.239
+  rev: v0.0.260
   hooks:
   - id: ruff
     args: [--fix]
 
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.6.0
+  rev: v2.8.0
   hooks:
   - id: pretty-format-yaml
     args: [--autofix, --indent, '2']
```

### Comparing `nonos-0.7.3/LICENSE` & `nonos-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/PKG-INFO` & `nonos-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonos
-Version: 0.7.3
+Version: 0.9.0
 Summary: A tool to analyze results from idefix/pluto simulations (for protoplanetary disks more specifically)
 Author: G. Wafflard-Fernandez, C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/volodia99/nonos
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -12,20 +12,23 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nonos
 [![PyPI](https://img.shields.io/pypi/v/nonos.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/nonos/)
 [![PyPI](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)](https://pypi.org/project/nonos/)
+[![Documentation Status](https://readthedocs.org/projects/nonos/badge/?version=latest)](https://nonos.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/volodia99/nonos/main.svg)](https://results.pre-commit.ci/badge/github/volodia99/nonos/main.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 nonos is a 2D visualization command line application for planet-disk numerical simulations, as well as a Python library. It works with vtk-formatted data from Pluto and Idefix, and dat-formatted data for Fargo-adsg and Fargo3D.
 
+For more, read [the documentation !](https://nonos.readthedocs.io/en/latest/?badge=latest)
+
 ##### Data Formats
 We list here the accepted formats for the data:
 Pluto and Idefix: data.\*\*\*\*.vtk
 Fargo-adsg: gasdens.dat, gasvy\*.dat, gasvx\*.dat
 Fargo3D: same as Fargo-adsg + gasvz\*.dat
 
 :construction: This project and documentation are under construction :construction:
```

### Comparing `nonos-0.7.3/README.md` & `nonos-0.9.0/nonos.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,34 @@
+Metadata-Version: 2.1
+Name: nonos
+Version: 0.9.0
+Summary: A tool to analyze results from idefix/pluto simulations (for protoplanetary disks more specifically)
+Author: G. Wafflard-Fernandez, C.M.T. Robert
+License: GPL-3.0
+Project-URL: Homepage, https://github.com/volodia99/nonos
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # nonos
 [![PyPI](https://img.shields.io/pypi/v/nonos.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/nonos/)
 [![PyPI](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)](https://pypi.org/project/nonos/)
+[![Documentation Status](https://readthedocs.org/projects/nonos/badge/?version=latest)](https://nonos.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/volodia99/nonos/main.svg)](https://results.pre-commit.ci/badge/github/volodia99/nonos/main.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 nonos is a 2D visualization command line application for planet-disk numerical simulations, as well as a Python library. It works with vtk-formatted data from Pluto and Idefix, and dat-formatted data for Fargo-adsg and Fargo3D.
 
+For more, read [the documentation !](https://nonos.readthedocs.io/en/latest/?badge=latest)
+
 ##### Data Formats
 We list here the accepted formats for the data:
 Pluto and Idefix: data.\*\*\*\*.vtk
 Fargo-adsg: gasdens.dat, gasvy\*.dat, gasvx\*.dat
 Fargo3D: same as Fargo-adsg + gasvz\*.dat
 
 :construction: This project and documentation are under construction :construction:
```

### Comparing `nonos-0.7.3/nonos/api/_adapt_clm_vtk.py` & `nonos-0.9.0/nonos/api/_adapt_clm_vtk.py`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/nonos/api/analysis.py` & `nonos-0.9.0/nonos/api/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import glob
 import os
+import warnings
 from pathlib import Path
 from typing import Any, Optional, Tuple
 
-import matplotlib.pyplot as plt
 import numpy as np
-from matplotlib.colors import SymLogNorm
-from mpl_toolkits.axes_grid1 import make_axes_locatable
+from matplotlib.ticker import SymmetricalLogLocator
 
-from nonos._mpl_utils import set_symlog_minor_ticks
 from nonos.api.from_simulation import Parameters
 from nonos.api.tools import find_around, find_nearest
 from nonos.logging import logger
 
 
 class Plotable:
     def __init__(self, dict_plotable: dict):
@@ -23,22 +21,27 @@
     def plot(
         self,
         fig,
         ax,
         *,
         log=False,
         cmap="inferno",
-        nbin=None,
         filename=None,
         fmt="png",
         dpi=500,
         title=None,
         unit_conversion=None,
+        nbin=None,  # deprecated
         **kwargs,
     ):
+        if nbin is not None:
+            warnings.warn(
+                "The nbin parameter has no effect and is deprecated",
+                stacklevel=2,
+            )
         data = self.data
         if unit_conversion is not None:
             data = data * unit_conversion
         if log:
             data = np.log10(data)
 
         if self.dimension == 2:
@@ -51,15 +54,15 @@
                 if "vmin" in kwargs:
                     norm.vmin = kwargs.pop("vmin")
                 if "vmax" in kwargs:
                     norm.vmax = kwargs.pop("vmax")
             else:
                 vmin = kwargs.pop("vmin") if "vmin" in kwargs else np.nanmin(data)
                 vmax = kwargs.pop("vmax") if "vmax" in kwargs else np.nanmax(data)
-                kw.update(dict(vmin=vmin, vmax=vmax))
+                kw.update({"vmin": vmin, "vmax": vmax})
 
             im = ax.pcolormesh(
                 self.avalue,
                 self.ovalue,
                 data,
                 cmap=cmap,
                 **kwargs,
@@ -69,23 +72,35 @@
                 xlim=(self.avalue.min(), self.avalue.max()),
                 ylim=(self.ovalue.min(), self.ovalue.max()),
             )
 
             ax.set_xlabel(self.akey)
             ax.set_ylabel(self.okey)
             if title is not None:
+                from mpl_toolkits.axes_grid1 import make_axes_locatable
+
                 divider = make_axes_locatable(ax)
                 cax = divider.append_axes("right", size="5%", pad=0.05)
                 cbar = fig.colorbar(
                     im, cax=cax, orientation="vertical"
                 )  # , format='%.0e')
                 cbar.set_label(title)
-                if isinstance(norm, SymLogNorm):
-                    # special cases logic layer, heavily inspired from yt
-                    set_symlog_minor_ticks(norm, cax)
+
+                cb_axis = cbar.ax.yaxis
+                if cb_axis.get_scale() == "symlog":
+                    # no minor tick is drawn in symlog norms by default
+                    # as of matplotlib 3.7.1, see
+                    # https://github.com/matplotlib/matplotlib/issues/25994
+                    trf = cb_axis.get_transform()
+                    cb_axis.set_major_locator(SymmetricalLogLocator(trf))
+                    if float(trf.base).is_integer():
+                        locator = SymmetricalLogLocator(
+                            trf, subs=np.arange(1, trf.base)
+                        )
+                        cb_axis.set_minor_locator(locator)
             else:
                 return im
         if self.dimension == 1:
             vmin = kwargs.pop("vmin") if "vmin" in kwargs else np.nanmin(data)
             vmax = kwargs.pop("vmax") if "vmax" in kwargs else np.nanmax(data)
             self.akey = self.dict_plotable["abscissa"]
             self.avalue = self.dict_plotable[self.akey]
@@ -99,15 +114,15 @@
             )
             ax.set_ylim(ymin=vmin)
             ax.set_ylim(ymax=vmax)
             ax.set_xlabel(self.akey)
             if title is not None:
                 ax.set_ylabel(title)
         if filename is not None:
-            plt.savefig(f"{filename}.{fmt}", bbox_inches="tight", dpi=dpi)
+            fig.savefig(f"{filename}.{fmt}", bbox_inches="tight", dpi=dpi)
 
 
 class Coordinates:
     """Coordinates class from x1, x2, x3"""
 
     def __init__(self, geometry: str, x1: np.ndarray, x2: np.ndarray, x3: np.ndarray):
         if x1.shape[0] == 1:
@@ -372,27 +387,27 @@
         ngeom: str,
         on: int,
         operation: str,
         *,
         inifile: str = "",
         code: str = "",
         directory="",
-        rotate_grid: bool = False,
+        rotate_grid: int = -1,
     ):
         self.field = field
         self.operation = operation
         self.native_geometry = ngeom
         self.data = data
         self.coords = coords
         self.on = on
 
         self.inifile = inifile
         self.code = code
         self.directory = directory
-        self.rotate_grid = rotate_grid
+        self._rotate_grid = rotate_grid
 
     @property
     def shape(self) -> Tuple[Any, ...]:
         """
         Returns
         =======
         shape : tuple
@@ -408,15 +423,19 @@
         dimension = len(wanted)
 
         if dimension == 1:
             meshgrid_conversion = self.coords._meshgrid_conversion(*wanted)
             # abscissa = meshgrid_conversion[wanted[0]]
             abscissa_value = list(meshgrid_conversion.values())[0]
             abscissa_key = list(meshgrid_conversion.keys())[0]
-            if planet_corotation is not None and "phi" in wanted:
+            if (
+                planet_corotation is not None
+                and "phi" in wanted
+                and self._rotate_grid != planet_corotation
+            ):
                 phip = self.find_phip(planet_number=planet_corotation)
                 phicoord = self.coords.phi - phip  # - np.pi
                 ipi = find_nearest(phicoord, 0)
                 if abs(0 - phicoord[ipi]) > abs(
                     np.ediff1d(find_around(phicoord, 0))[0]
                 ):
                     ipi = find_nearest(phicoord, 2 * np.pi)
@@ -449,15 +468,19 @@
             meshgrid_conversion = self.coords._meshgrid_conversion(*wanted)
             abscissa_value, ordinate_value = (
                 meshgrid_conversion[wanted[0]],
                 meshgrid_conversion[wanted[1]],
             )
             abscissa_key, ordinate_key = (wanted[0], wanted[1])
             native_from_wanted = self.coords.native_from_wanted(*wanted)[0]
-            if planet_corotation is not None and "phi" in native_from_wanted:
+            if (
+                planet_corotation is not None
+                and "phi" in native_from_wanted
+                and self._rotate_grid != planet_corotation
+            ):
                 phip = self.find_phip(planet_number=planet_corotation)
                 phicoord = self.coords.phi - phip  # - np.pi
                 # ipi = find_nearest(phicoord, np.pi)
                 # if (abs(np.pi-phicoord[ipi])>abs(np.ediff1d(find_around(phicoord, np.pi))[0])):
                 #     ipi = find_nearest(phicoord, -np.pi)
                 ipi = find_nearest(phicoord, 0)
                 if abs(0 - phicoord[ipi]) > abs(
@@ -472,14 +495,15 @@
                     self.data = np.roll(
                         self.data, -ipi - self.coords.phi.shape[0] // 2 + 1, axis=2
                     )
                 else:
                     raise NotImplementedError(
                         f"geometry flag '{self.native_geometry}' not implemented yet if planet_corotation"
                     )
+                self._rotate_grid = planet_corotation
             ordered = meshgrid_conversion["ordered"]
             # move the axis of reduction in the front in order to
             # perform the operation 3D(i,j,1) -> 2D(i,j) in a general way,
             # whatever the position of (i,j,1)
             # for that we must be careful to change the order ("ordered") if the data is reversed
             # in practice, this is tricky only if the "1" is in the middle:
             # 3D(i,1,k) -> 2D(i,k) is not a direct triedre anymore, we need to do 2D(i,k).T = 2D(k,i)
@@ -573,15 +597,15 @@
         )
         init.loadIniFile()
         init.loadPlanetFile(planet_number=planet_number)
         ind_on = find_nearest(init.tpl, init.vtk * self.on)
         return pow(init.qpl[ind_on] / 3.0, 1.0 / 3.0) * init.apl[ind_on]
 
     def find_phip(self, planet_number: int = 0):
-        if self.rotate_grid:
+        if self._rotate_grid == planet_number:
             return 0.0
         init = Parameters(
             inifile=self.inifile, code=self.code, directory=self.directory
         )
         init.loadIniFile()
         init.loadPlanetFile(planet_number=planet_number)
         ind_on = find_nearest(init.tpl, init.vtk * self.on)
@@ -649,15 +673,15 @@
             ret_coords,
             self.native_geometry,
             self.on,
             operation,
             inifile=self.inifile,
             code=self.code,
             directory=self.directory,
-            rotate_grid=self.rotate_grid,
+            rotate_grid=self._rotate_grid,
         )
 
     # def latitudinal_projection(self, theta=None):
     #     operation = self.operation + "_latitudinal_projection"
     #     imid = self.find_imid()
     #     if self.native_geometry == "polar":
     #         ret_coords = Coordinates(
@@ -745,15 +769,15 @@
     #         ret_coords,
     #         self.native_geometry,
     #         self.on,
     #         operation,
     #         inifile=self.inifile,
     #         code=self.code,
     #         directory=self.directory,
-    #         rotate_grid=self.rotate_grid,
+    #         rotate_grid=self._rotate_grid,
     #     )
 
     def vertical_projection(self, z=None):
         operation = self.operation + "_vertical_projection"
         imid = self.find_imid()
         if self.native_geometry == "cartesian":
             ret_coords = Coordinates(
@@ -806,15 +830,15 @@
             ret_coords,
             self.native_geometry,
             self.on,
             operation,
             inifile=self.inifile,
             code=self.code,
             directory=self.directory,
-            rotate_grid=self.rotate_grid,
+            rotate_grid=self._rotate_grid,
         )
 
     def vertical_at_midplane(self):
         # self.field = r"%s$_{\rm mid}$" % self.field
         operation = self.operation + "_vertical_at_midplane"
         imid = self.find_imid()
         if self.native_geometry == "cartesian":
@@ -852,15 +876,15 @@
             ret_coords,
             self.native_geometry,
             self.on,
             operation,
             inifile=self.inifile,
             code=self.code,
             directory=self.directory,
-            rotate_grid=self.rotate_grid,
+            rotate_grid=self._rotate_grid,
         )
 
     def latitudinal_at_theta(self, theta=None, name_operation=None):
         logger.info("latitudinal_at_theta TO BE TESTED")
         if theta is None:
             if self.native_geometry in ("cartesian", "polar", "spherical"):
                 theta = 0.0
@@ -933,15 +957,15 @@
             ret_coords,
             self.native_geometry,
             self.on,
             operation,
             inifile=self.inifile,
             code=self.code,
             directory=self.directory,
-            rotate_grid=self.rotate_grid,
+            rotate_grid=self._rotate_grid,
         )
 
     def vertical_at_z(self, z=None, name_operation=None):
         logger.info("vertical_at_z TO BE TESTED")
         # self.field = r"%s$_{\rm mid}$" % self.field
         if z is None:
             z = 0
@@ -1024,15 +1048,15 @@
             ret_coords,
             self.native_geometry,
             self.on,
             operation,
             inifile=self.inifile,
             code=self.code,
             directory=self.directory,
-            rotate_grid=self.rotate_grid,
+            rotate_grid=self._rotate_grid,
         )
 
     def azimuthal_at_phi(self, phi=None):
         if phi is None:
             phi = 0.0
         # self.field = r"%s ($\phi_P$)" % self.field
         operation = self.operation + f"_azimuthal_at_phi{phi}"
@@ -1064,15 +1088,15 @@
             ret_coords,
             self.native_geometry,
             self.on,
             operation,
             inifile=self.inifile,
             code=self.code,
             directory=self.directory,
-            rotate_grid=self.rotate_grid,
+            rotate_grid=self._rotate_grid,
         )
 
     def azimuthal_at_planet(self, planet_number: int = 0):
         operation = self.operation + "_azimuthal_at_planet"
         phip = self.find_phip(planet_number=planet_number)
         aziphip = self.azimuthal_at_phi(phi=phip)
         return GasField(
@@ -1081,15 +1105,15 @@
             aziphip.coords,
             self.native_geometry,
             self.on,
             operation,
             inifile=self.inifile,
             code=self.code,
             directory=self.directory,
-            rotate_grid=self.rotate_grid,
+            rotate_grid=self._rotate_grid,
         )
 
     def azimuthal_average(self):
         # self.field = r"$\langle$%s$\rangle$" % self.field
         operation = self.operation + "_azimuthal_average"
         iphi = self.find_iphi(phi=0)
         if self.native_geometry == "cartesian":
@@ -1122,15 +1146,15 @@
             ret_coords,
             self.native_geometry,
             self.on,
             operation,
             inifile=self.inifile,
             code=self.code,
             directory=self.directory,
-            rotate_grid=self.rotate_grid,
+            rotate_grid=self._rotate_grid,
         )
 
     def remove_planet_hill(self, planet_number: int = 0):
         # self.field = r"$\langle$%s$\rangle$" % self.field
         operation = self.operation + "_remove_planet_hill"
         phip = self.find_phip(planet_number=planet_number)
         rp = self.find_rp(planet_number=planet_number)
@@ -1187,15 +1211,15 @@
             ret_coords,
             self.native_geometry,
             self.on,
             operation,
             inifile=self.inifile,
             code=self.code,
             directory=self.directory,
-            rotate_grid=self.rotate_grid,
+            rotate_grid=self._rotate_grid,
         )
 
     def radial_at_r(self, distance=None):
         if distance is None:
             distance = 1.0
         operation = self.operation + f"_radial_at_r{distance}"
         ir1 = self.find_ir(distance=distance)
@@ -1226,15 +1250,15 @@
             ret_coords,
             self.native_geometry,
             self.on,
             operation,
             inifile=self.inifile,
             code=self.code,
             directory=self.directory,
-            rotate_grid=self.rotate_grid,
+            rotate_grid=self._rotate_grid,
         )
 
     def radial_average_interval(self, vmin=None, vmax=None):
         operation = self.operation + f"_radial_average_interval_{vmin}_{vmax}"
         irmin = self.find_ir(distance=vmin)
         irmax = self.find_ir(distance=vmax)
         ir = self.find_ir(distance=(vmax - vmin) / 2)
@@ -1273,15 +1297,15 @@
             ret_coords,
             self.native_geometry,
             self.on,
             operation,
             inifile=self.inifile,
             code=self.code,
             directory=self.directory,
-            rotate_grid=self.rotate_grid,
+            rotate_grid=self._rotate_grid,
         )
 
     def diff(self, on_2):
         ds_2 = GasDataSet(
             on_2,
             geometry=self.native_geometry,
             inifile=self.inifile,
@@ -1302,48 +1326,51 @@
             ret_coords,
             self.native_geometry,
             self.on,
             self.operation,
             inifile=self.inifile,
             code=self.code,
             directory=self.directory,
-            rotate_grid=self.rotate_grid,
+            rotate_grid=self._rotate_grid,
         )
 
     def rotate(self, planet_corotation: Optional[int] = None):
         operation = self.operation
         if self.shape.count(1) != 1:
             raise ValueError("data has to be 2D in order to rotate the data.")
-        if planet_corotation is not None:  # and self.coords.phi.shape[0]!=1:
+        if (
+            planet_corotation is not None and self._rotate_grid != planet_corotation
+        ):  # and self.coords.phi.shape[0]!=1:
             phip = self.find_phip(planet_number=planet_corotation)
             phicoord = self.coords.phi - phip  # - np.pi
             ipi = find_nearest(phicoord, 0)
             if abs(0 - phicoord[ipi]) > abs(np.ediff1d(find_around(phicoord, 0))[0]):
                 ipi = find_nearest(phicoord, 2 * np.pi)
             if self.native_geometry == "polar":
                 ret_data = np.roll(
-                    self.data, -ipi - self.coords.phi.shape[0] // 2, axis=1
+                    self.data, -ipi - self.coords.phi.shape[0] // 2 + 1, axis=1
                 )
                 ret_coords = Coordinates(
                     self.native_geometry, self.coords.R, self.coords.phi, self.coords.z
                 )
             elif self.native_geometry == "spherical":
                 ret_data = np.roll(
-                    self.data, -ipi - self.coords.phi.shape[0] // 2, axis=2
+                    self.data, -ipi - self.coords.phi.shape[0] // 2 + 1, axis=2
                 )
                 ret_coords = Coordinates(
                     self.native_geometry,
                     self.coords.r,
                     self.coords.theta,
                     self.coords.phi,
                 )
             else:
                 raise NotImplementedError(
                     f"geometry flag '{self.native_geometry}' not implemented yet if planet_corotation"
                 )
+            self._rotate_grid = planet_corotation
         else:
             ret_data = self.data
             if self.native_geometry == "polar":
                 ret_coords = Coordinates(
                     self.native_geometry, self.coords.R, self.coords.phi, self.coords.z
                 )
             elif self.native_geometry == "spherical":
@@ -1360,29 +1387,29 @@
             ret_coords,
             self.native_geometry,
             self.on,
             operation,
             inifile=self.inifile,
             code=self.code,
             directory=self.directory,
-            rotate_grid=True,
+            rotate_grid=self._rotate_grid,
         )
 
 
 class GasDataSet:
     """Idefix dataset class that contains everything in the .vtk file
 
-    Attributes
-    ==========
-    on : int corresponding to the output number.
-    dict: dictionary[str, array] that contains all the fields
-    coords : Coordinates of the data.
-        Edge of the cells.
-    coordsmed : Coordinates of the data.
-        Center of the cells.
+    Args:
+        on (int): output number
+        directory (str): directory of the .vtk
+        geometry (str): for retrocompatibility if old vtk format
+        inifile (str): name of the simulation's parameter file if no default files (combined with code)
+        code (str): name of the code ("idefix", "pluto", "fargo3d", "fargo-adsg")
+    Returns:
+        dataset
     """
 
     # def __init__(self, on:int, *, code:Optional[str]=None, directory:str=""):
     def __init__(
         self,
         on: int,
         *,
@@ -1473,15 +1500,15 @@
     data: np.ndarray,
     coords: Coordinates,
     on: int,
     operation: str,
     inifile: str = "",
     code: str = "",
     directory: str = "",
-    rotate_grid: bool = False,
+    rotate_grid: int = -1,
 ):
     ret_data = data
     ret_coords = coords
     geometry = coords.geometry
     return GasField(
         field,
         ret_data,
```

### Comparing `nonos-0.7.3/nonos/api/from_simulation.py` & `nonos-0.9.0/nonos/api/from_simulation.py`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/nonos/api/satellite.py` & `nonos-0.9.0/nonos/api/satellite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 import os
-import re
+import warnings
 from typing import Any, Dict, List, Optional, Tuple
 
 import numpy as np
 from lick.lick import lick_box
-from scipy.ndimage.filters import uniform_filter1d
 
 from nonos.api.analysis import GasField, Plotable, temporal
 from nonos.api.from_simulation import Parameters
 
 
 def file_analysis(filename, *, inifile="", code="", directory="", norb=None):
-    fullpath = os.path.join(directory, filename)
-    with open(fullpath) as f1:
-        data = f1.readlines()
-    y = [[v for v in re.split(r"[\t ]+", r)] for r in data]
-    columns = np.array(y, dtype="float64").T
+    from scipy.ndimage import uniform_filter1d
+
+    columns = np.loadtxt(os.path.join(directory, filename), dtype="float64").T
     if norb is not None:
         init = Parameters(inifile=inifile, code=code, directory=directory)
         init.loadIniFile()
-        if init.code == "idefix" and "analysis" in init.inifile["Output"].keys():
+        if init.code == "idefix" and "analysis" in init.inifile["Output"]:
             analysis = init.inifile["Output"]["analysis"]
             rpini = init.inifile["Planet"]["dpl"]
             Ntmean = round(norb * 2 * np.pi * pow(rpini, 1.5) / analysis)
             for i in range(1, len(columns) - 1):
                 columns[i] = uniform_filter1d(columns[i], Ntmean)
         else:
             raise NotImplementedError(
                 f"moving average on {norb} orbits is not implemented for the code {init.code}"
             )
     return columns
 
 
 def planet_analysis(planet_number, *, inifile="", code="", directory="", norb=None):
+    if norb is not None:
+        warnings.warn(
+            "The norb argument has no effect and is deprecated",
+            stacklevel=2,
+        )
     init = Parameters(inifile=inifile, code=code, directory=directory)
     init.loadIniFile()
     init.loadPlanetFile(planet_number=planet_number)
     return init
 
 
 def save_temporal(
@@ -160,15 +162,14 @@
         vmin: Optional[float] = None,
         vmax: Optional[float] = None,
         alpha: float = 0.45,
         log: bool = False,
         cmap=None,
         title: Optional[str] = None,
         density_streamlines: Optional[float] = None,
-        **kwargs,
     ):
         dict_background = {}
         dict_background["field"] = "background"
         dict_background["abscissa"] = "x"
         dict_background["ordinate"] = "y"
         dict_background[dict_background["field"]] = self.F
         dict_background[dict_background["abscissa"]] = self.X
@@ -225,28 +226,23 @@
         return im
 
 
 def compute(
     field: str,
     data: np.ndarray,
     ref: GasField,
-    *,
-    inifile: str = "",
-    code: str = "",
-    directory: str = "",
-    rotate_grid: bool = False,
 ):
     ret_data = data
     ret_coords = ref.coords
     geometry = ret_coords.geometry
     return GasField(
         field,
         ret_data,
         ret_coords,
         geometry,
         ref.on,
         operation=ref.operation,
-        inifile=inifile,
-        code=code,
-        directory=directory,
-        rotate_grid=rotate_grid,
+        inifile=ref.inifile,
+        code=ref.code,
+        directory=ref.directory,
+        rotate_grid=ref._rotate_grid,
     )
```

### Comparing `nonos-0.7.3/nonos/config.py` & `nonos-0.9.0/nonos/config.py`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/nonos/logging.py` & `nonos-0.9.0/nonos/logging.py`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/nonos/logo.txt` & `nonos-0.9.0/nonos/logo.txt`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/nonos/main.py` & `nonos-0.9.0/nonos/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 import re
 import sys
 import time
 from collections import ChainMap
 from multiprocessing import Pool
 from typing import Any, Dict, List, Optional
 
-import cblind as cb
+import cblind  # noqa
 import inifix
-import matplotlib.pyplot as plt
 import numpy as np
 from inifix.format import iniformat
 
 from nonos.__version__ import __version__
 from nonos.api import GasDataSet, Parameters
 from nonos.config import DEFAULTS
 from nonos.logging import (
@@ -63,23 +62,23 @@
     cmap,
     title,
     unit_conversion: int,
     datadir,
     show: bool,
     dpi: int,
     fmt: str,
-    pbar,
-    parallel,
     theta,
     z,
     phi,
     distance,
     *,
     log_level,
 ):
+    import matplotlib.pyplot as plt
+
     configure_logger(level=log_level)
     set_mpl_style(scaling=scaling)
 
     ds = GasDataSet(on, geometry=geometry, directory=datadir)
     dsop = ds[field]
     if diff:
         dsop = dsop.diff(0)
@@ -138,15 +137,15 @@
     elif dim == 2:
         dsop.map(plane[0], plane[1], planet_corotation=corotate).plot(
             fig,
             ax,
             log=log,
             vmin=vmin,
             vmax=vmax,
-            cmap=cb.cbmap(cmap, nbin=None),
+            cmap=cmap,
             title="$%s$" % title,
             unit_conversion=unit_conversion,
         )
         akey = dsop.map(plane[0], plane[1], planet_corotation=corotate).dict_plotable[
             "abscissa"
         ]
         okey = dsop.map(plane[0], plane[1], planet_corotation=corotate).dict_plotable[
@@ -549,15 +548,15 @@
         from rich.progress import track
 
         def mytrack(iterable, *args, **kwargs):
             return track(iterable, *args, **kwargs)
 
     else:
         # replace rich.progress.track with a no-op dummy
-        def mytrack(iterable, *args, **kwargs):
+        def mytrack(iterable, *args, **kwargs):  # noqa: ARG001
             return iterable
 
     # call of the process_field function, whether it be in parallel or not
     # TODO: reduce this to the bare minimum
     func = functools.partial(
         process_field,
         operations=operations,
@@ -574,16 +573,14 @@
         cmap=args["cmap"],
         title=title,
         unit_conversion=args["unit_conversion"],
         datadir=args["datadir"],
         show=show,
         dpi=args["dpi"],
         fmt=args["format"],
-        pbar=args["progressBar"],
-        parallel=args["ncpu"] > 1,
         theta=theta,
         z=z,
         phi=phi,
         distance=distance,
         log_level=level,
     )
```

### Comparing `nonos-0.7.3/nonos/parsing.py` & `nonos-0.9.0/nonos/parsing.py`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/nonos/styling.py` & `nonos-0.9.0/nonos/styling.py`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/nonos.egg-info/PKG-INFO` & `nonos-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,19 @@
-Metadata-Version: 2.1
-Name: nonos
-Version: 0.7.3
-Summary: A tool to analyze results from idefix/pluto simulations (for protoplanetary disks more specifically)
-Author: G. Wafflard-Fernandez, C.M.T. Robert
-License: GPL-3.0
-Project-URL: Homepage, https://github.com/volodia99/nonos
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Typing :: Typed
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # nonos
 [![PyPI](https://img.shields.io/pypi/v/nonos.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/nonos/)
 [![PyPI](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)](https://pypi.org/project/nonos/)
+[![Documentation Status](https://readthedocs.org/projects/nonos/badge/?version=latest)](https://nonos.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/volodia99/nonos/main.svg)](https://results.pre-commit.ci/badge/github/volodia99/nonos/main.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 nonos is a 2D visualization command line application for planet-disk numerical simulations, as well as a Python library. It works with vtk-formatted data from Pluto and Idefix, and dat-formatted data for Fargo-adsg and Fargo3D.
 
+For more, read [the documentation !](https://nonos.readthedocs.io/en/latest/?badge=latest)
+
 ##### Data Formats
 We list here the accepted formats for the data:
 Pluto and Idefix: data.\*\*\*\*.vtk
 Fargo-adsg: gasdens.dat, gasvy\*.dat, gasvx\*.dat
 Fargo3D: same as Fargo-adsg + gasvz\*.dat
 
 :construction: This project and documentation are under construction :construction:
```

### Comparing `nonos-0.7.3/nonos.egg-info/SOURCES.txt` & `nonos-0.9.0/nonos.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 LICENSE
 README.md
 pyproject.toml
 .github/workflows/ci.yml
 nonos/__init__.py
 nonos/__main__.py
 nonos/__version__.py
-nonos/_mpl_utils.py
 nonos/config.py
 nonos/default.mplstyle
 nonos/logging.py
 nonos/logo.txt
 nonos/main.py
 nonos/parsing.py
 nonos/py.typed
```

### Comparing `nonos-0.7.3/pyproject.toml` & `nonos-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 requires = [
     "setuptools>=61.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nonos"
-version = "0.7.3"
 description = "A tool to analyze results from idefix/pluto simulations (for protoplanetary disks more specifically)"
 authors = [
     { name = "G. Wafflard-Fernandez" },
     { name = "C.M.T. Robert" },
 ]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -18,24 +17,25 @@
     "Programming Language :: Python :: 3 :: Only",
     "Typing :: Typed",
 ]
 requires-python = ">=3.8"
 
 # keep in sync with constraints/minimal_dependencies.txt
 dependencies = [
-    "cblind>=2.2.2",
+    "cblind>=2.3.0",
     "inifix>=3.0.0",
     "lick>=0.2.0",
     "loguru>=0.5.3",
     "matplotlib>=3.5.0",
     "numpy>=1.18.5",
     "rich>=10.13.0",
     "scipy>=1.6.1",
     "importlib_resources>=1.3; python_version < '3.9'"
 ]
+dynamic = ["version"]
 
 [project.license]
 text = "GPL-3.0"
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
@@ -58,30 +58,38 @@
     "logo.txt",
     "default.mplstyle",
 ]
 
 [tool.setuptools.packages.find]
 namespaces = false
 
+[tool.setuptools.dynamic]
+version = {attr = "nonos.__version__.__version__"}
+
 [tool.ruff]
-target-version = "py38" # https://github.com/charliermarsh/ruff/issues/2039
 exclude = ["*__init__.py"]
 ignore = ["E501"]
 select = [
     "E",
     "F",
     "W",
-    "B",
-    "I",
-    "UP",
+    "ARG", # flake8-unused-arguments
+    "C4",  # flake8-comprehensions
+    "B",   # flake8-bugbear
+    "YTT", # flake8-2020
+    "I",   # isort
+    "UP",  # pyupgrade
 ]
 
 [tool.ruff.isort]
 combine-as-imports = true
 
+[tool.pytest.ini_options]
+filterwarnings = ["error"]
+
 [tool.mypy]
 python_version = "3.8"
 show_error_codes = true
 warn_unused_configs = true
 warn_unused_ignores = true
 warn_unreachable = true
 show_error_context = true
```

### Comparing `nonos-0.7.3/tests/conftest.py` & `nonos-0.9.0/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 import matplotlib
 import matplotlib.pyplot as plt
 import pytest
 
 
-def pytest_configure(config):
+def pytest_configure(config):  # noqa: ARG001
     matplotlib.use("Agg")
 
 
 @pytest.fixture()
 def test_data_dir():
     return Path(__file__).parent / "data"
```

### Comparing `nonos-0.7.3/tests/data/fargo3d_planet2d/domain_x.dat` & `nonos-0.9.0/tests/data/fargo3d_planet2d/domain_x.dat`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/data/fargo3d_planet2d/domain_y.dat` & `nonos-0.9.0/tests/data/fargo3d_planet2d/domain_y.dat`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/data/fargo3d_planet2d/gasdens0.dat` & `nonos-0.9.0/tests/data/fargo3d_planet2d/gasdens0.dat`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/data/fargo3d_planet2d/gasdens40.dat` & `nonos-0.9.0/tests/data/fargo3d_planet2d/gasdens40.dat`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/data/fargo3d_planet2d/gasvy40.dat` & `nonos-0.9.0/tests/data/fargo3d_planet2d/gasvy40.dat`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/data/fargo3d_planet2d/planet0.dat` & `nonos-0.9.0/tests/data/fargo3d_planet2d/planet0.dat`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/data/fargo3d_planet2d/variables.par` & `nonos-0.9.0/tests/data/fargo3d_planet2d/variables.par`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/data/idefix_newvtk_planet2d/data.0000.vtk` & `nonos-0.9.0/tests/data/idefix_newvtk_planet2d/data.0000.vtk`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/data/idefix_newvtk_planet2d/data.0023.vtk` & `nonos-0.9.0/tests/data/idefix_newvtk_planet2d/data.0023.vtk`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/data/idefix_newvtk_planet2d/idefix.ini` & `nonos-0.9.0/tests/data/idefix_newvtk_planet2d/idefix.ini`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/data/idefix_newvtk_planet2d/planet0.dat` & `nonos-0.9.0/tests/data/idefix_newvtk_planet2d/planet0.dat`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/data/idefix_planet3d/data.0000.vtk` & `nonos-0.9.0/tests/data/idefix_planet3d/data.0000.vtk`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/data/idefix_planet3d/data.0043.vtk` & `nonos-0.9.0/tests/data/idefix_planet3d/data.0043.vtk`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/data/idefix_planet3d/idefix.ini` & `nonos-0.9.0/tests/data/idefix_planet3d/idefix.ini`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/data/idefix_planet3d/planet0.dat` & `nonos-0.9.0/tests/data/idefix_planet3d/planet0.dat`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/data/idefix_rwi/data.0000.vtk` & `nonos-0.9.0/tests/data/idefix_rwi/data.0000.vtk`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/data/idefix_rwi/data.0001.vtk` & `nonos-0.9.0/tests/data/idefix_rwi/data.0001.vtk`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/data/idefix_rwi/idefix.ini` & `nonos-0.9.0/tests/data/idefix_rwi/idefix.ini`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/test_cli.py` & `nonos-0.9.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/test_image_comp.py` & `nonos-0.9.0/tests/test_image_comp.py`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/test_load_config.py` & `nonos-0.9.0/tests/test_load_config.py`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/test_params_usage.py` & `nonos-0.9.0/tests/test_params_usage.py`

 * *Files identical despite different names*

### Comparing `nonos-0.7.3/tests/test_parsing.py` & `nonos-0.9.0/tests/test_parsing.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,33 +48,28 @@
             "Can't parse a range from sequence [1, 2, 3, 4] with more than 3 values."
         ),
     ):
         parse_output_number_range([1, 2, 3, 4])
 
 
 @pytest.mark.parametrize(
-    "abscissa, ordinate, dim, received",
+    "dim, extent",
     [
-        (
-            np.linspace(0.2, 10, 100),
-            np.linspace(-0.4, 0.4, 100),
-            2,
-            ("0.4", "8", "0", "-0.2", "0.2"),
-        ),
-        (np.linspace(0.2, 10, 100), np.linspace(-0.4, 0.4, 100), 1, (0.4, 8, 0.2)),
+        (2, ("0.4", "8", "0", "-0.2", "0.2")),
+        (1, (0.4, 8, 0.2)),
     ],
 )
-def test_invalid_nargs_parse_range(abscissa, ordinate, dim, received):
+def test_invalid_nargs_parse_range(dim, extent):
     with pytest.raises(
         ValueError,
         match=re.escape(
-            f"Received sequence `extent` with incorrect size {len(received)}. Expected exactly {2*dim=} values."
+            f"Received sequence `extent` with incorrect size {len(extent)}. Expected exactly {2*dim=} values."
         ),
     ):
-        parse_range(received, dim=dim)
+        parse_range(extent, dim)
 
 
 @pytest.mark.parametrize(
     "received",
     [
         [1, 0],
         [1, 0, 1],
```

### Comparing `nonos-0.7.3/tests/test_plotting.py` & `nonos-0.9.0/tests/test_plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,24 +176,22 @@
     rhovx2_from_data = from_data(
         field="RHOVX2",
         data=rhovp * vx2vp,
         coords=rhovpfield.coords,
         on=rhovpfield.on,
         operation=rhovpfield.operation,
         directory=directory,
-        rotate_grid=rhovpfield.rotate_grid,
+        rotate_grid=rhovpfield._rotate_grid,
     )
 
     datane = ne.evaluate("rhovp*vx2vp")
     rhovx2_compute = compute(
         field="RHOVX2",
         data=datane,
         ref=rhovpfield,
-        directory=directory,
-        rotate_grid=rhovpfield.rotate_grid,
     )
 
     npt.assert_array_equal(rhovx2_from_data.data, rhovx2_compute.data)
 
 
 def test_pbar(simulation_dir, capsys):
     ret = main(["-pbar", "-dir", str(simulation_dir), "-geometry", "polar"])
```

### Comparing `nonos-0.7.3/tests/test_readme.py` & `nonos-0.9.0/tests/test_readme.py`

 * *Files identical despite different names*

