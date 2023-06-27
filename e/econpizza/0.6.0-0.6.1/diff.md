# Comparing `tmp/econpizza-0.6.0.tar.gz` & `tmp/econpizza-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econpizza-0.6.0.tar", last modified: Fri Jun 23 09:41:45 2023, max compression
+gzip compressed data, was "econpizza-0.6.1.tar", last modified: Tue Jun 27 10:05:07 2023, max compression
```

## Comparing `econpizza-0.6.0.tar` & `econpizza-0.6.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.324484 econpizza-0.6.0/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.301151 econpizza-0.6.0/.github/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.304484 econpizza-0.6.0/.github/workflows/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1316 2023-06-23 09:24:38.000000 econpizza-0.6.0/.github/workflows/continuous-integration.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      173 2023-03-17 19:22:56.000000 econpizza-0.6.0/.gitignore
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      287 2023-03-19 10:47:42.000000 econpizza-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      599 2023-03-22 13:14:47.000000 econpizza-0.6.0/.readthedocs.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-03-02 09:28:46.000000 econpizza-0.6.0/LICENSE
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3994 2023-06-23 09:41:45.324484 econpizza-0.6.0/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3516 2023-06-23 09:29:36.000000 econpizza-0.6.0/README.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.307818 econpizza-0.6.0/docs/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-03-02 09:28:46.000000 econpizza-0.6.0/docs/Makefile
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.301151 econpizza-0.6.0/docs/_static/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.307818 econpizza-0.6.0/docs/_static/css/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-03-02 09:28:46.000000 econpizza-0.6.0/docs/_static/css/custom.css
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1551 2023-05-02 19:15:35.000000 econpizza-0.6.0/docs/conf.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      331 2023-03-22 14:25:19.000000 econpizza-0.6.0/docs/content.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.307818 econpizza-0.6.0/docs/guide/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      564 2023-06-23 09:37:08.000000 econpizza-0.6.0/docs/guide/installation.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8245 2023-03-22 11:47:43.000000 econpizza-0.6.0/docs/guide/method.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2606 2023-05-07 18:36:01.000000 econpizza-0.6.0/docs/guide/solution.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2161 2023-05-07 18:29:06.000000 econpizza-0.6.0/docs/guide/steady_state.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    14328 2023-05-02 15:47:57.000000 econpizza-0.6.0/docs/guide/the_yaml.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2420 2023-05-27 12:18:06.000000 econpizza-0.6.0/docs/index.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    58150 2023-03-02 09:28:46.000000 econpizza-0.6.0/docs/lin_and_nlin.png
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      800 2023-03-02 09:28:46.000000 econpizza-0.6.0/docs/make.bat
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    22585 2023-03-02 09:28:46.000000 econpizza-0.6.0/docs/p_and_n.png
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       80 2023-03-30 19:10:44.000000 econpizza-0.6.0/docs/requirements.txt
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.311151 econpizza-0.6.0/docs/tutorial/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2954 2023-03-10 20:34:11.000000 econpizza-0.6.0/docs/tutorial/boehl_hommes.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   389791 2023-06-06 14:13:17.000000 econpizza-0.6.0/docs/tutorial/hank1.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   234012 2023-03-22 12:13:19.000000 econpizza-0.6.0/docs/tutorial/hank2.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    63713 2023-03-22 11:52:34.000000 econpizza-0.6.0/docs/tutorial/quickstart.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   407267 2023-03-22 12:01:00.000000 econpizza-0.6.0/docs/tutorial/rank.ipynb
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.311151 econpizza-0.6.0/econpizza/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3547 2023-03-28 11:53:45.000000 econpizza-0.6.0/econpizza/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       47 2023-06-23 09:40:38.000000 econpizza-0.6.0/econpizza/__version__.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.314484 econpizza-0.6.0/econpizza/examples/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      446 2023-03-25 22:11:17.000000 econpizza-0.6.0/econpizza/examples/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      770 2023-03-02 09:28:46.000000 econpizza-0.6.0/econpizza/examples/bh.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7086 2023-05-27 12:24:35.000000 econpizza-0.6.0/econpizza/examples/dsge.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4857 2023-03-25 10:04:56.000000 econpizza-0.6.0/econpizza/examples/ghls.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8709 2023-03-24 20:08:58.000000 econpizza-0.6.0/econpizza/examples/hank2.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5559 2023-03-14 23:49:18.000000 econpizza-0.6.0/econpizza/examples/hank2_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6656 2023-03-26 20:12:16.000000 econpizza-0.6.0/econpizza/examples/hank2_no_capital.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1652 2023-05-13 03:15:20.000000 econpizza-0.6.0/econpizza/examples/hank_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3716 2023-03-24 20:09:04.000000 econpizza-0.6.0/econpizza/examples/hank_labor.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3373 2023-03-15 14:58:36.000000 econpizza-0.6.0/econpizza/examples/hank_labor_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6137 2023-03-24 20:09:14.000000 econpizza-0.6.0/econpizza/examples/hank_with_comments.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1550 2023-04-11 07:59:18.000000 econpizza-0.6.0/econpizza/examples/nk.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5512 2023-03-02 09:28:46.000000 econpizza-0.6.0/econpizza/examples/tank.yml
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.317818 econpizza-0.6.0/econpizza/parser/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    12187 2023-05-13 03:38:34.000000 econpizza-0.6.0/econpizza/parser/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8145 2023-03-20 23:57:24.000000 econpizza-0.6.0/econpizza/parser/build_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4728 2023-04-21 09:07:56.000000 econpizza-0.6.0/econpizza/parser/checks.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3237 2023-03-18 14:35:53.000000 econpizza-0.6.0/econpizza/parser/het_agent_base_funcs.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4337 2023-05-12 08:16:06.000000 econpizza-0.6.0/econpizza/parser/write_dynamic_functions.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.317818 econpizza-0.6.0/econpizza/solvers/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6472 2023-03-10 20:34:11.000000 econpizza-0.6.0/econpizza/solvers/shooting.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2789 2023-03-18 09:32:31.000000 econpizza-0.6.0/econpizza/solvers/solve_linear.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4889 2023-03-10 20:34:11.000000 econpizza-0.6.0/econpizza/solvers/solve_linear_state_space.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6278 2023-05-16 14:17:55.000000 econpizza-0.6.0/econpizza/solvers/stacking.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8561 2023-05-05 14:50:38.000000 econpizza-0.6.0/econpizza/solvers/steady_state.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.321151 econpizza-0.6.0/econpizza/testing/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.321151 econpizza-0.6.0/econpizza/testing/cache/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1760 2023-03-14 23:53:28.000000 econpizza-0.6.0/econpizza/testing/cache/bh.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7064 2023-03-14 23:54:36.000000 econpizza-0.6.0/econpizza/testing/cache/hank_labor.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2984 2023-03-14 23:55:47.000000 econpizza-0.6.0/econpizza/testing/cache/hank_solid.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      429 2023-04-20 15:35:27.000000 econpizza-0.6.0/econpizza/testing/test_nb_hank1.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      429 2023-04-20 15:44:49.000000 econpizza-0.6.0/econpizza/testing/test_nb_hank2.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      421 2023-03-18 09:32:45.000000 econpizza-0.6.0/econpizza/testing/test_nb_quickstart.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      415 2023-03-18 09:32:45.000000 econpizza-0.6.0/econpizza/testing/test_nb_rank.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      414 2023-03-18 09:32:45.000000 econpizza-0.6.0/econpizza/testing/test_nb_under_the_hood.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1883 2023-05-10 08:08:46.000000 econpizza-0.6.0/econpizza/testing/test_rest.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      940 2023-03-10 20:34:11.000000 econpizza-0.6.0/econpizza/tools.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.324484 econpizza-0.6.0/econpizza/utilities/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3391 2023-03-18 14:36:19.000000 econpizza-0.6.0/econpizza/utilities/dists.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-04-27 11:18:13.000000 econpizza-0.6.0/econpizza/utilities/grids.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4769 2023-05-04 15:35:28.000000 econpizza-0.6.0/econpizza/utilities/interp.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4173 2023-03-30 22:34:43.000000 econpizza-0.6.0/econpizza/utilities/jacobian.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6395 2023-05-09 11:21:21.000000 econpizza-0.6.0/econpizza/utilities/newton.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.311151 econpizza-0.6.0/econpizza.egg-info/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3994 2023-06-23 09:41:45.000000 econpizza-0.6.0/econpizza.egg-info/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2060 2023-06-23 09:41:45.000000 econpizza-0.6.0/econpizza.egg-info/SOURCES.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-06-23 09:41:45.000000 econpizza-0.6.0/econpizza.egg-info/dependency_links.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       81 2023-06-23 09:41:45.000000 econpizza-0.6.0/econpizza.egg-info/requires.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       10 2023-06-23 09:41:45.000000 econpizza-0.6.0/econpizza.egg-info/top_level.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      163 2023-06-23 09:12:01.000000 econpizza-0.6.0/requirements.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-06-23 09:41:45.324484 econpizza-0.6.0/setup.cfg
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1334 2023-06-23 09:12:23.000000 econpizza-0.6.0/setup.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 10:05:07.714074 econpizza-0.6.1/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 10:05:07.684074 econpizza-0.6.1/.github/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 10:05:07.690740 econpizza-0.6.1/.github/workflows/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1316 2023-06-23 09:24:38.000000 econpizza-0.6.1/.github/workflows/continuous-integration.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      173 2023-03-17 19:22:56.000000 econpizza-0.6.1/.gitignore
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      287 2023-03-19 10:47:42.000000 econpizza-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      599 2023-03-22 13:14:47.000000 econpizza-0.6.1/.readthedocs.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-03-02 09:28:46.000000 econpizza-0.6.1/LICENSE
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3994 2023-06-27 10:05:07.714074 econpizza-0.6.1/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3516 2023-06-23 09:29:36.000000 econpizza-0.6.1/README.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 10:05:07.694074 econpizza-0.6.1/docs/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-03-02 09:28:46.000000 econpizza-0.6.1/docs/Makefile
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 10:05:07.684074 econpizza-0.6.1/docs/_static/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 10:05:07.694074 econpizza-0.6.1/docs/_static/css/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-03-02 09:28:46.000000 econpizza-0.6.1/docs/_static/css/custom.css
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1551 2023-05-02 19:15:35.000000 econpizza-0.6.1/docs/conf.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      331 2023-03-22 14:25:19.000000 econpizza-0.6.1/docs/content.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 10:05:07.697407 econpizza-0.6.1/docs/guide/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      563 2023-06-23 09:43:34.000000 econpizza-0.6.1/docs/guide/installation.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8245 2023-03-22 11:47:43.000000 econpizza-0.6.1/docs/guide/method.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2606 2023-05-07 18:36:01.000000 econpizza-0.6.1/docs/guide/solution.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2161 2023-05-07 18:29:06.000000 econpizza-0.6.1/docs/guide/steady_state.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    14328 2023-05-02 15:47:57.000000 econpizza-0.6.1/docs/guide/the_yaml.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2420 2023-05-27 12:18:06.000000 econpizza-0.6.1/docs/index.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    58150 2023-03-02 09:28:46.000000 econpizza-0.6.1/docs/lin_and_nlin.png
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      800 2023-03-02 09:28:46.000000 econpizza-0.6.1/docs/make.bat
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    22585 2023-03-02 09:28:46.000000 econpizza-0.6.1/docs/p_and_n.png
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       80 2023-03-30 19:10:44.000000 econpizza-0.6.1/docs/requirements.txt
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 10:05:07.700740 econpizza-0.6.1/docs/tutorial/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2954 2023-03-10 20:34:11.000000 econpizza-0.6.1/docs/tutorial/boehl_hommes.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   389791 2023-06-06 14:13:17.000000 econpizza-0.6.1/docs/tutorial/hank1.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   234012 2023-03-22 12:13:19.000000 econpizza-0.6.1/docs/tutorial/hank2.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    63713 2023-03-22 11:52:34.000000 econpizza-0.6.1/docs/tutorial/quickstart.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   407267 2023-03-22 12:01:00.000000 econpizza-0.6.1/docs/tutorial/rank.ipynb
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 10:05:07.700740 econpizza-0.6.1/econpizza/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3547 2023-03-28 11:53:45.000000 econpizza-0.6.1/econpizza/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       47 2023-06-27 10:04:53.000000 econpizza-0.6.1/econpizza/__version__.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 10:05:07.704074 econpizza-0.6.1/econpizza/examples/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      446 2023-03-25 22:11:17.000000 econpizza-0.6.1/econpizza/examples/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      770 2023-03-02 09:28:46.000000 econpizza-0.6.1/econpizza/examples/bh.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7086 2023-05-27 12:24:35.000000 econpizza-0.6.1/econpizza/examples/dsge.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4857 2023-03-25 10:04:56.000000 econpizza-0.6.1/econpizza/examples/ghls.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8709 2023-03-24 20:08:58.000000 econpizza-0.6.1/econpizza/examples/hank2.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5559 2023-03-14 23:49:18.000000 econpizza-0.6.1/econpizza/examples/hank2_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6656 2023-03-26 20:12:16.000000 econpizza-0.6.1/econpizza/examples/hank2_no_capital.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1652 2023-05-13 03:15:20.000000 econpizza-0.6.1/econpizza/examples/hank_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3777 2023-06-27 10:04:44.000000 econpizza-0.6.1/econpizza/examples/hank_labor.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3373 2023-03-15 14:58:36.000000 econpizza-0.6.1/econpizza/examples/hank_labor_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6233 2023-06-27 10:04:44.000000 econpizza-0.6.1/econpizza/examples/hank_with_comments.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1550 2023-04-11 07:59:18.000000 econpizza-0.6.1/econpizza/examples/nk.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5512 2023-03-02 09:28:46.000000 econpizza-0.6.1/econpizza/examples/tank.yml
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 10:05:07.707407 econpizza-0.6.1/econpizza/parser/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    12187 2023-05-13 03:38:34.000000 econpizza-0.6.1/econpizza/parser/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8145 2023-03-20 23:57:24.000000 econpizza-0.6.1/econpizza/parser/build_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4728 2023-04-21 09:07:56.000000 econpizza-0.6.1/econpizza/parser/checks.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3237 2023-03-18 14:35:53.000000 econpizza-0.6.1/econpizza/parser/het_agent_base_funcs.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4337 2023-05-12 08:16:06.000000 econpizza-0.6.1/econpizza/parser/write_dynamic_functions.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 10:05:07.707407 econpizza-0.6.1/econpizza/solvers/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6472 2023-03-10 20:34:11.000000 econpizza-0.6.1/econpizza/solvers/shooting.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2789 2023-03-18 09:32:31.000000 econpizza-0.6.1/econpizza/solvers/solve_linear.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4889 2023-03-10 20:34:11.000000 econpizza-0.6.1/econpizza/solvers/solve_linear_state_space.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6278 2023-05-16 14:17:55.000000 econpizza-0.6.1/econpizza/solvers/stacking.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8561 2023-05-05 14:50:38.000000 econpizza-0.6.1/econpizza/solvers/steady_state.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 10:05:07.710740 econpizza-0.6.1/econpizza/testing/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 10:05:07.710740 econpizza-0.6.1/econpizza/testing/cache/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1760 2023-03-14 23:53:28.000000 econpizza-0.6.1/econpizza/testing/cache/bh.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7472 2023-06-27 10:04:44.000000 econpizza-0.6.1/econpizza/testing/cache/hank_labor.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3152 2023-06-27 10:04:44.000000 econpizza-0.6.1/econpizza/testing/cache/hank_solid.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      429 2023-04-20 15:35:27.000000 econpizza-0.6.1/econpizza/testing/test_nb_hank1.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      429 2023-04-20 15:44:49.000000 econpizza-0.6.1/econpizza/testing/test_nb_hank2.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      421 2023-03-18 09:32:45.000000 econpizza-0.6.1/econpizza/testing/test_nb_quickstart.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      415 2023-03-18 09:32:45.000000 econpizza-0.6.1/econpizza/testing/test_nb_rank.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      414 2023-03-18 09:32:45.000000 econpizza-0.6.1/econpizza/testing/test_nb_under_the_hood.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1883 2023-05-10 08:08:46.000000 econpizza-0.6.1/econpizza/testing/test_rest.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      940 2023-03-10 20:34:11.000000 econpizza-0.6.1/econpizza/tools.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 10:05:07.714074 econpizza-0.6.1/econpizza/utilities/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3391 2023-03-18 14:36:19.000000 econpizza-0.6.1/econpizza/utilities/dists.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-04-27 11:18:13.000000 econpizza-0.6.1/econpizza/utilities/grids.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4769 2023-05-04 15:35:28.000000 econpizza-0.6.1/econpizza/utilities/interp.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4173 2023-03-30 22:34:43.000000 econpizza-0.6.1/econpizza/utilities/jacobian.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6395 2023-05-09 11:21:21.000000 econpizza-0.6.1/econpizza/utilities/newton.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-27 10:05:07.700740 econpizza-0.6.1/econpizza.egg-info/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3994 2023-06-27 10:05:07.000000 econpizza-0.6.1/econpizza.egg-info/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2060 2023-06-27 10:05:07.000000 econpizza-0.6.1/econpizza.egg-info/SOURCES.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-06-27 10:05:07.000000 econpizza-0.6.1/econpizza.egg-info/dependency_links.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       81 2023-06-27 10:05:07.000000 econpizza-0.6.1/econpizza.egg-info/requires.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       10 2023-06-27 10:05:07.000000 econpizza-0.6.1/econpizza.egg-info/top_level.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      163 2023-06-27 10:04:44.000000 econpizza-0.6.1/requirements.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-06-27 10:05:07.714074 econpizza-0.6.1/setup.cfg
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1334 2023-06-27 10:04:44.000000 econpizza-0.6.1/setup.py
```

### Comparing `econpizza-0.6.0/.github/workflows/continuous-integration.yml` & `econpizza-0.6.1/.github/workflows/continuous-integration.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/.readthedocs.yaml` & `econpizza-0.6.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/LICENSE` & `econpizza-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/PKG-INFO` & `econpizza-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econpizza
-Version: 0.6.0
+Version: 0.6.1
 Summary: Solve nonlinear perfect foresight models with heterogeneous agents
 Home-page: https://github.com/gboehl/econpizza
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `econpizza-0.6.0/README.rst` & `econpizza-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/docs/Makefile` & `econpizza-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/docs/conf.py` & `econpizza-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/docs/guide/installation.rst` & `econpizza-0.6.1/docs/guide/installation.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Installation
 ============
 
-The package is under active development. Stable releases can be installed from the official Python repositories, which are updated frequently. 
+The package is under active development. Stable releases can be installed from the official Python repositories, which are updated frequently.
 
 Installing the `repository version <https://pypi.org/project/econpizza/>`_ from PyPi is as simple as typing
 
 .. code-block:: bash
 
    pip install econpizza
```

### Comparing `econpizza-0.6.0/docs/guide/method.ipynb` & `econpizza-0.6.1/docs/guide/method.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/docs/guide/solution.rst` & `econpizza-0.6.1/docs/guide/solution.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/docs/guide/steady_state.rst` & `econpizza-0.6.1/docs/guide/steady_state.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/docs/guide/the_yaml.rst` & `econpizza-0.6.1/docs/guide/the_yaml.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/docs/index.rst` & `econpizza-0.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/docs/lin_and_nlin.png` & `econpizza-0.6.1/docs/lin_and_nlin.png`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/docs/make.bat` & `econpizza-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/docs/p_and_n.png` & `econpizza-0.6.1/docs/p_and_n.png`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/docs/tutorial/boehl_hommes.rst` & `econpizza-0.6.1/docs/tutorial/boehl_hommes.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/docs/tutorial/hank1.ipynb` & `econpizza-0.6.1/docs/tutorial/hank1.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/docs/tutorial/hank2.ipynb` & `econpizza-0.6.1/docs/tutorial/hank2.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/docs/tutorial/quickstart.ipynb` & `econpizza-0.6.1/docs/tutorial/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/docs/tutorial/rank.ipynb` & `econpizza-0.6.1/docs/tutorial/rank.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/__init__.py` & `econpizza-0.6.1/econpizza/__init__.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/examples/bh.yml` & `econpizza-0.6.1/econpizza/examples/bh.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/examples/dsge.yml` & `econpizza-0.6.1/econpizza/examples/dsge.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/examples/ghls.yml` & `econpizza-0.6.1/econpizza/examples/ghls.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/examples/hank2.yml` & `econpizza-0.6.1/econpizza/examples/hank2.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/examples/hank2_functions.py` & `econpizza-0.6.1/econpizza/examples/hank2_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/examples/hank2_no_capital.yml` & `econpizza-0.6.1/econpizza/examples/hank2_no_capital.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/examples/hank_functions.py` & `econpizza-0.6.1/econpizza/examples/hank_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/examples/hank_labor.yml` & `econpizza-0.6.1/econpizza/examples/hank_labor.yml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 description: 'A small example HANK model with endogenous labor supply'
 functions_file: 'hank_labor_functions.py'
 # NOTE: the file hank_with_comments.yaml contains a detailed explanation of the objects defined here
 
 definitions: |
     from jax.numpy import log, maximum
     from econpizza.tools import percentile, jax_print
-variables: [ div, y, y_prod, w, pi, R, Rn, Rr, Rstar, tax, z, beta, C, N, B, Top10C, Top10A ]
+variables: [ div, mc, y, y_prod, w, pi, R, Rn, Rr, Rstar, tax, z, beta, C, N, B, Top10C, Top10A ]
 parameters: [ sigma_c, sigma_l, theta, psi, phi_pi, phi_y, rho, rho_beta, rho_r, rho_z, chi ]
 shocks: [ e_beta, e_rstar, e_z ]
 
 distributions:
   dist:
     skills: # dim0
       type: exogenous_rouwenhorst
@@ -51,15 +51,16 @@
     ~ Top10C = top10c
     ~ Top10A = top10a
 
     # firms
     ~ N = y_prod/z # production function
     ~ div = - w*N + (1 - psi*(pi/piSS - 1)**2/2)*y_prod # dividends
     ~ y = (1 - psi*(pi/piSS - 1)**2/2)*y_prod # "effective" output
-    ~ psi*(pi/piSS - 1)*pi/piSS = (1-theta) + theta*w/z + psi*piPrime/R*(piPrime/piSS - 1)*piPrime/piSS*y_prodPrime/y_prod # NKPC
+    ~ psi*(pi/piSS - 1)*pi/piSS = (1-theta) + theta*mc + psi*piPrime/R*(piPrime/piSS - 1)*piPrime/piSS*y_prodPrime/y_prod # NKPC
+    ~ mc = w/z # marginal costs
 
     # government
     ~ Rr = RLag/pi # real rate ex-post
     ~ Rn = (Rstar*((pi/piSS)**phi_pi)*((y/yLag)**phi_y))**(1-rho)*RnLag**rho # MP rule on shadow nominal rate
     ~ R = maximum(1, Rn) # ZLB
     ~ tax = (Rr-1)*B # balanced budget
 
@@ -88,15 +89,16 @@
 
         # steady state
         y: 1.0 # effective output
         N: 1. # labor supply
         z: 1. # technology
         pi: 1.0 # inflation
         B: 5.6 # bond supply
-        w: (theta-1)/theta # wages
+        mc: (theta-1)/theta # marginal costs
+        w: mc*z
         div: 1 - w*N # dividends
         Rstar: 1.002 # steady stat target rate
 
     init_guesses:
         beta: 0.98 # discount factor
         chi: 0.8 # utility weight on disutility of labor
         tax: 0.028
```

### Comparing `econpizza-0.6.0/econpizza/examples/hank_labor_functions.py` & `econpizza-0.6.1/econpizza/examples/hank_labor_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/examples/hank_with_comments.yml` & `econpizza-0.6.1/econpizza/examples/hank_with_comments.yml`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # the following definitions are available during all three stages:
 definitions: |
     from jax.numpy import log, maximum
     # jax_print can be used for debugging
     from econpizza.tools import percentile, jax_print
 
 # these lists define the relevant models objects
-variables: [ div, y, y_prod, w, pi, R, Rn, Rr, Rstar, tax, z, beta, C, n, B, Top10C, Top10A ]
+variables: [ div, mc, y, y_prod, w, pi, R, Rn, Rr, Rstar, tax, z, beta, C, n, B, Top10C, Top10A ]
 parameters: [ sigma_c, sigma_l, theta, psi, phi_pi, phi_y, rho, rho_beta, rho_r, rho_z ]
 shocks: [ e_beta, e_rstar, e_z ]
 
 # this defines all distribution objects (so far, only one distribution is supported)
 distributions:
   # the name of the first distribution
   dist:
@@ -85,15 +85,16 @@
     ~ Top10C = top10c
     ~ Top10A = top10a
 
     # firms
     ~ n = y_prod/z # production function
     ~ div = -w*n + (1 - psi*(pi/piSS - 1)**2/2)*y_prod # dividends
     ~ y = (1 - psi*(pi/piSS - 1)**2/2)*y_prod # "effective" output
-    ~ psi*(pi/piSS - 1)*pi/piSS = (1-theta) + theta*w + psi*piPrime/R*(piPrime/piSS - 1)*piPrime/piSS*y_prodPrime/y_prod # NKPC
+    ~ psi*(pi/piSS - 1)*pi/piSS = (1-theta) + theta*mc + psi*piPrime/R*(piPrime/piSS - 1)*piPrime/piSS*y_prodPrime/y_prod # NKPC
+    ~ mc = w/z # marginal costs
 
     # government
     ~ tax = (Rr-1)*BLag # balanced budget
     ~ Rr = RLag/pi # real ex-post bond return
     ~ Rn = (Rstar*((pi/piSS)**phi_pi)*((y/yLag)**phi_y))**(1-rho)*RnLag**rho # MP rule on shadow nominal rate
     ~ R = maximum(1, Rn) # ZLB
 
@@ -125,18 +126,19 @@
         y: 1.0 # effective output
         y_prod: 1.0 # output
         C: 1.0 # consumption
         pi: 1.0 # inflation
         beta: 0.98 # discount factor
         B: 5.6 # bond supply
         # definitions can be recursive: theta is defined above
-        w: (theta-1)/theta # wages
+        mc: (theta-1)/theta # marginal costs
+        w: (mc*y)**(sigma_l/(1+sigma_l)) # wages
         n: w**(1/sigma_l) # labor supply
-        div: 1 - w*n # dividends
         z: y/n # technology
+        div: 1 - w*n # dividends
 
     init_guesses:
         Rstar: 1.002 # steady state target rage
         Rr: Rstar # steady state real rage
         Rn: Rstar # steady state notional rage
         R: Rstar # steady state nominal rage
         tax: 0.028
```

### Comparing `econpizza-0.6.0/econpizza/examples/nk.yml` & `econpizza-0.6.1/econpizza/examples/nk.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/examples/tank.yml` & `econpizza-0.6.1/econpizza/examples/tank.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/parser/__init__.py` & `econpizza-0.6.1/econpizza/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/parser/build_functions.py` & `econpizza-0.6.1/econpizza/parser/build_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/parser/checks.py` & `econpizza-0.6.1/econpizza/parser/checks.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/parser/het_agent_base_funcs.py` & `econpizza-0.6.1/econpizza/parser/het_agent_base_funcs.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/parser/write_dynamic_functions.py` & `econpizza-0.6.1/econpizza/parser/write_dynamic_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/solvers/shooting.py` & `econpizza-0.6.1/econpizza/solvers/shooting.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/solvers/solve_linear.py` & `econpizza-0.6.1/econpizza/solvers/solve_linear.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/solvers/solve_linear_state_space.py` & `econpizza-0.6.1/econpizza/solvers/solve_linear_state_space.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/solvers/stacking.py` & `econpizza-0.6.1/econpizza/solvers/stacking.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/solvers/steady_state.py` & `econpizza-0.6.1/econpizza/solvers/steady_state.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/testing/cache/bh.npy` & `econpizza-0.6.1/econpizza/testing/cache/bh.npy`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/testing/cache/hank_labor.npy` & `econpizza-0.6.1/econpizza/testing/cache/hank_labor.npy`

 * *Files 13% similar despite different names*

```diff
@@ -1,442 +1,467 @@
 00000000: 934e 554d 5059 0100 7600 7b27 6465 7363  .NUMPY..v.{'desc
 00000010: 7227 3a20 273c 6638 272c 2027 666f 7274  r': '<f8', 'fort
 00000020: 7261 6e5f 6f72 6465 7227 3a20 4661 6c73  ran_order': Fals
 00000030: 652c 2027 7368 6170 6527 3a20 2835 312c  e, 'shape': (51,
-00000040: 2031 3729 2c20 7d20 2020 2020 2020 2020   17), }         
+00000040: 2031 3829 2c20 7d20 2020 2020 2020 2020   18), }         
 00000050: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000060: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000070: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-00000080: 6666 6666 6666 1640 2788 a40b 6c86 ef3f  ffffff.@'...l..?
-00000090: 4ba2 4100 0000 f03f 5455 5555 5555 c53f  K.A....?TUUUUU.?
-000000a0: 0000 0000 0000 f03f 0000 0000 0000 f03f  .......?.......?
-000000b0: 2287 e926 3108 f03f 9586 e926 3108 f03f  "..&1..?...&1..?
-000000c0: ae87 e926 3108 f03f d578 e926 3108 f03f  ...&1..?.x.&1..?
-000000d0: 2074 b3ae 06f0 863f 11d1 5dbe b6b8 db3f   t.....?..]....?
-000000e0: 8ffd a762 6746 c43f abaa aaaa aaaa ea3f  ...bgF.?.......?
-000000f0: 0000 0000 0000 f03f 0000 0000 0000 f03f  .......?.......?
-00000100: 0000 0000 0000 f03f 8922 a566 6666 1640  .......?.".fff.@
-00000110: f0fe dc0d e0ae ef3f 3b5f d1ec d97e ee3f  .......?;_...~.?
-00000120: 5dc9 4ccb 8b5f cf3f c389 cce9 9858 ef3f  ].L.._.?.....X.?
-00000130: d53a 78a4 393d ef3f 20c8 faff ffff ef3f  .:x.9=.? ......?
-00000140: 4eee 03e7 7ecd ef3f 3023 2a9d 266c f03f  N...~..?0#*.&l.?
-00000150: d578 e926 3108 f03f 612a fb4d 28ed c23f  .x.&1..?a*.M(..?
-00000160: d446 9cb5 6d18 dc3f a3ed ae37 a0ab c43f  .F..m..?...7...?
-00000170: 1b82 1d26 f01f e73f 3b5f d1ec d97e ee3f  ...&...?;_...~.?
-00000180: c389 cce9 9858 ef3f 0000 0000 0000 f03f  .....X.?.......?
-00000190: 7e24 a566 6666 1640 8336 231f d2aa ef3f  ~$.fff.@.6#....?
-000001a0: 66c7 62cb 60f8 ee3f 1754 7a04 cfcc cd3f  f.b.`..?.Tz....?
-000001b0: 942f 51af a265 ef3f c6cc 3e77 2476 ef3f  ./Q..e.?..>w$v.?
-000001c0: d94c f8ff ffff ef3f 68b6 680e ecb3 ef3f  .L.....?h.h....?
-000001d0: 4589 5acc 1b46 f03f d578 e926 3108 f03f  E.Z..F.?.x.&1..?
-000001e0: 0961 8eb9 ba89 b83f 4090 3aaf e050 dc3f  .a.....?@.:..P.?
-000001f0: ef3d 1775 d88c c43f 3a6f 915c d0f8 e73f  .=.u...?:o.\...?
-00000200: 66c7 62cb 60f8 ee3f 942f 51af a265 ef3f  f.b.`..?./Q..e.?
-00000210: 0000 0000 0000 f03f d425 a566 6666 1640  .......?.%.fff.@
-00000220: 219b 0c6d 2ca7 ef3f 1c1c 5b34 f04c ef3f  !..m,..?..[4.L.?
-00000230: 036f e14c c410 cc3f a8a5 57d1 3380 ef3f  .o.L...?..W.3..?
-00000240: 7fbf 99aa b9a1 ef3f 2538 f7ff ffff ef3f  .......?%8.....?
-00000250: a733 e18e daab ef3f 3fa5 7aa7 af2f f03f  .3.....??.z../.?
-00000260: d578 e926 3108 f03f 2531 82d1 adb0 b03f  .x.&1..?%1.....?
-00000270: b96d 255c 4973 dc3f b9b5 6906 9278 c43f  .m%\Is.?..i..x.?
-00000280: bd30 cc3f 44ab e83f 1c1c 5b34 f04c ef3f  .0.?D..?..[4.L.?
-00000290: a8a5 57d1 3380 ef3f 0000 0000 0000 f03f  ..W.3..?.......?
-000002a0: 9326 a566 6666 1640 a907 8475 e4a3 ef3f  .&.fff.@...u...?
-000002b0: a1cb b522 228a ef3f 0c07 0e53 354c ca3f  ...""..?...S5L.?
-000002c0: 19cf 3f81 55a0 ef3f 4693 9750 15c2 ef3f  ..?.U..?F..P...?
-000002d0: 6e2c f7ff ffff ef3f 818f 73c4 9dae ef3f  n,.....?..s....?
-000002e0: decc 33b3 311f f03f d578 e926 3108 f03f  ..3.1..?.x.&1..?
-000002f0: db94 4c71 fdd5 a53f 8f2a 27c1 9c84 dc3f  ..Lq...?.*'....?
-00000300: ae82 bd45 d868 c43f ca8c 541a 9942 e93f  ...E.h.?..T..B.?
-00000310: a1cb b522 228a ef3f 19cf 3f81 55a0 ef3f  ...""..?..?.U..?
-00000320: 0000 0000 0000 f03f f726 a566 6666 1640  .......?.&.fff.@
-00000330: 6de1 94c7 f0a0 ef3f e5a3 2e84 ddb4 ef3f  m......?.......?
-00000340: 7675 19c8 b5c4 c83f fc87 1b2e c9bd ef3f  vu.....?.......?
-00000350: 0b70 e3a6 d2d8 ef3f 0ece f7ff ffff ef3f  .p.....?.......?
-00000360: bac8 90db 3fb7 ef3f ea0d 6fc5 ae13 f03f  ....?..?..o....?
-00000370: d578 e926 3108 f03f 0114 c79b 478e 9b3f  .x.&1..?....G..?
-00000380: d0e0 6ed1 c589 dc3f 3584 07e8 395d c43f  ..n....?5...9].?
-00000390: 3e7e 8b84 e9b8 e93f e5a3 2e84 ddb4 ef3f  >~.....?.......?
-000003a0: fc87 1b2e c9bd ef3f 0000 0000 0000 f03f  .......?.......?
-000003b0: 1927 a566 6666 1640 9dea 51e7 489e ef3f  .'.fff.@..Q.H..?
-000003c0: 492d d7f2 dad1 ef3f af54 78d9 3994 c73f  I-.....?.Tx.9..?
-000003d0: 0d27 69f4 32d5 ef3f 1e75 2873 0ce8 ef3f  .'i.2..?.u(s...?
-000003e0: 51cd f8ff ffff ef3f 065e 780e 6fc2 ef3f  Q......?.^x.o..?
-000003f0: eb42 cec3 020c f03f d578 e926 3108 f03f  .B.....?.x.&1..?
-00000400: 2fcb 8cba abd0 903f 200f cd49 d086 dc3f  /......? ..I...?
-00000410: a7af 8be0 ee54 c43f ffca be06 a80f ea3f  .....T.?.......?
-00000420: 492d d7f2 dad1 ef3f 0d27 69f4 32d5 ef3f  I-.....?.'i.2..?
-00000430: 0000 0000 0000 f03f 0a27 a566 6666 1640  .......?.'.fff.@
-00000440: 20d3 b134 e59b ef3f 10f0 08ab 0ce5 ef3f   ..4...?.......?
-00000450: 03af 7da6 53b8 c63f 79b6 33b9 3ae6 ef3f  ..}.S..?y.3.:..?
-00000460: 454f 4881 c9f1 ef3f 12ef f9ff ffff ef3f  EOH....?.......?
-00000470: a9be c9ec 1ace ef3f 5f96 c568 1e07 f03f  .......?_..h...?
-00000480: d578 e926 3108 f03f b246 43f6 beee 833f  .x.&1..?.FC....?
-00000490: d5eb 4fda c47e dc3f cd6b efdf 234f c43f  ..O..~.?.k..#O.?
-000004a0: ef2a 8f5d 254c ea3f 10f0 08ab 0ce5 ef3f  .*.]%L.?.......?
-000004b0: 79b6 33b9 3ae6 ef3f 0000 0000 0000 f03f  y.3.:..?.......?
-000004c0: da26 a566 6666 1640 d465 0ed5 be99 ef3f  .&.fff.@.e.....?
-000004d0: 5756 3616 81f1 ef3f c236 64c0 8721 c63f  WV6....?.6d..!.?
-000004e0: 2f80 e2e2 e7f1 ef3f 3357 20e3 b6f7 ef3f  /......?3W ....?
-000004f0: 510d fbff ffff ef3f 73e4 5152 17d9 ef3f  Q......?s.QR...?
-00000500: 5eb5 4ea1 2504 f03f d578 e926 3108 f03f  ^.N.%..?.x.&1..?
-00000510: 7bb7 38ec 2039 773f 1393 328e c573 dc3f  {.8. 9w?..2..s.?
-00000520: fa33 43f5 2e4b c43f a69b 772c c674 ea3f  .3C..K.?..w,.t.?
-00000530: 5756 3616 81f1 ef3f 2f80 e2e2 e7f1 ef3f  WV6....?/......?
-00000540: 0000 0000 0000 f03f 9426 a566 6666 1640  .......?.&.fff.@
-00000550: 3fea fc9e cf97 ef3f 52f8 8c81 67f9 ef3f  ?......?R...g..?
-00000560: cef7 8a83 5ebe c53f 002f a7a4 8bf9 ef3f  ....^..?./.....?
-00000570: 5e5d d4fa 16fb ef3f 4912 fcff ffff ef3f  ^].....?I......?
-00000580: 2c7e ac1f cfe2 ef3f 4f35 13e3 7402 f03f  ,~.....?O5..t..?
-00000590: d578 e926 3108 f03f 33e9 6ed7 8883 6b3f  .x.&1..?3.n...k?
-000005a0: 1a33 738b 4067 dc3f f970 5ab8 8448 c43f  .3s.@g.?.pZ..H.?
-000005b0: 5734 964b 2b8f ea3f 52f8 8c81 67f9 ef3f  W4.K+..?R...g..?
-000005c0: 002f a7a4 8bf9 ef3f 0000 0000 0000 f03f  ./.....?.......?
-000005d0: 4726 a566 6666 1640 0cce 3e08 1296 ef3f  G&.fff.@..>....?
-000005e0: 7a04 f220 42fe ef3f 1dc4 8525 d17f c53f  z.. B..?...%...?
-000005f0: 47c8 1962 51fe ef3f e7c8 b488 cffc ef3f  G..bQ..?.......?
-00000600: d2f3 fcff ffff ef3f ee70 88cb 0beb ef3f  .......?.p.....?
-00000610: cb95 5764 9801 f03f d578 e926 3108 f03f  ..Wd...?.x.&1..?
-00000620: 81bd bf6e fddd 613f 08c1 7bab 215a dc3f  ...n..a?..{.!Z.?
-00000630: 8e08 b409 b746 c43f 94ee f31c b49f ea3f  .....F.?.......?
-00000640: 7a04 f220 42fe ef3f 47c8 1962 51fe ef3f  z.. B..?G..bQ..?
-00000650: 0000 0000 0000 f03f f525 a566 6666 1640  .......?.%.fff.@
-00000660: 9513 9115 8194 ef3f c0a9 d9d5 8900 f03f  .......?.......?
-00000670: 50ed d6e1 8b5a c53f 1c47 6f89 8e00 f03f  P....Z.?.Go....?
-00000680: 054e a316 7ffd ef3f 33af fdff ffff ef3f  .N.....?3......?
-00000690: ebbd fd70 cef1 ef3f 8d07 c18d 4001 f03f  ...p...?....@..?
-000006a0: d578 e926 3108 f03f bc43 914a 670c 5c3f  .x.&1..?.C.Jg.\?
-000006b0: 6bb0 944f fa4c dc3f 4cbb 7d13 8045 c43f  k..O.L.?L.}..E.?
-000006c0: fd7f cc2d 83a9 ea3f c0a9 d9d5 8900 f03f  ...-...?.......?
-000006d0: 1c47 6f89 8e00 f03f 0000 0000 0000 f03f  .Go....?.......?
-000006e0: a925 a566 6666 1640 5081 274c 1893 ef3f  .%.fff.@P.'L...?
-000006f0: 20af bcb9 4301 f03f d401 1ba1 8b46 c53f   ...C..?.....F.?
-00000700: 1bf8 6329 4801 f03f ab5c 2e7e 91fd ef3f  ..c)H..?.\.~...?
-00000710: f045 feff ffff ef3f 2636 3584 36f7 ef3f  .E.....?&65.6..?
-00000720: b961 9058 3701 f03f d578 e926 3108 f03f  .a.X7..?.x.&1..?
-00000730: 0171 0c3c 263e 5b3f e81f 3e5e 1e40 dc3f  .q.<&>[?..>^.@.?
-00000740: 9da9 5e73 b244 c43f d0d9 b147 c1ae ea3f  ..^s.D.?...G...?
-00000750: 20af bcb9 4301 f03f 1bf8 6329 4801 f03f   ...C..?..c)H..?
-00000760: 0000 0000 0000 f03f 5d25 a566 6666 1640  .......?]%.fff.@
-00000770: e141 a6a4 d391 ef3f c84d 0aa6 8501 f03f  .A.....?.M.....?
-00000780: d7f8 ae30 803e c53f dc0b e411 8b01 f03f  ...0.>.?.......?
-00000790: 5b27 4fdb 4ffd ef3f 9ebb feff ffff ef3f  ['O.O..?.......?
-000007a0: f56f 2cf4 71fb ef3f d111 412f 5801 f03f  .o,.q..?..A/X..?
-000007b0: d578 e926 3108 f03f 5cd5 4918 bc1d 5e3f  .x.&1..?\.I...^?
-000007c0: ddd5 7557 b833 dc3f d1d4 a142 2e44 c43f  ..uW.3.?...B.D.?
-000007d0: f602 3734 d8b0 ea3f c84d 0aa6 8501 f03f  ..74...?.M.....?
-000007e0: dc0b e411 8b01 f03f 0000 0000 0000 f03f  .......?.......?
-000007f0: 1825 a566 6666 1640 dca8 717f af90 ef3f  .%.fff.@..q....?
-00000800: 1c23 de65 7101 f03f 405b dec1 183f c53f  .#.eq..?@[...?.?
-00000810: da22 c77e 7801 f03f bbf1 9fa1 ecfc ef3f  .".~x..?.......?
-00000820: 8b14 ffff ffff ef3f 6c90 66e3 b3fe ef3f  .......?l.f....?
-00000830: cabd 09d5 8901 f03f d578 e926 3108 f03f  .......?.x.&1..?
-00000840: 48e2 7da0 eb3a 613f a1aa e05b d727 dc3f  H.}..:a?...[.'.?
-00000850: 1d61 4fb2 d643 c43f 8a11 5090 a8b0 ea3f  .aO..C.?..P....?
-00000860: 1c23 de65 7101 f03f da22 c77e 7801 f03f  .#.eq..?.".~x..?
-00000870: 0000 0000 0000 f03f d424 a566 6666 1640  .......?.$.fff.@
-00000880: 493c 309a a88f ef3f d2b0 03e5 1901 f03f  I<0....?.......?
-00000890: 0372 18ff 7a46 c53f 55da d1d5 2201 f03f  .r..zF.?U..."..?
-000008a0: 4444 d93d 8cfc ef3f b38b 7ad3 9700 f03f  DD.=...?..z....?
-000008b0: b38b 7ad3 9700 f03f cca0 c310 ba01 f03f  ..z....?.......?
-000008c0: d578 e926 3108 f03f e7ab d828 2257 633f  .x.&1..?...("Wc?
-000008d0: a654 9990 781c dc3f e9c9 d84c 9c43 c43f  .T..x..?...L.C.?
-000008e0: af40 7707 b0ae ea3f d2b0 03e5 1901 f03f  .@w....?.......?
-000008f0: 55da d1d5 2201 f03f 0000 0000 0000 f03f  U..."..?.......?
-00000900: 9c24 a566 6666 1640 8b0a 5f06 bc8e ef3f  .$.fff.@.._....?
-00000910: 2735 a021 8800 f03f 77e5 ee76 e653 c53f  '5.!...?w..v.S.?
-00000920: c0e0 9f6f 9200 f03f 9faf 1827 4bfc ef3f  ...o...?...'K..?
-00000930: 993c 9c43 8b01 f03f 993c 9c43 8b01 f03f  .<.C...?.<.C...?
-00000940: 80d6 7f88 7202 f03f d578 e926 3108 f03f  ....r..?.x.&1..?
-00000950: 84f8 7bfe 2b69 6b3f 4595 5ee9 2412 dc3f  ..{.+ik?E.^.$..?
-00000960: 87ee 84ad d043 c43f fb82 db91 22ab ea3f  .....C.?...."..?
-00000970: 2735 a021 8800 f03f c0e0 9f6f 9200 f03f  '5.!...?...o...?
-00000980: 0000 0000 0000 f03f 6f24 a566 6666 1640  .......?o$.fff.@
-00000990: 71c8 db20 e78d ef3f bbf8 f476 0e00 f03f  q.. ...?...v...?
-000009a0: adbb d21c 2e5f c53f 61aa 9cf3 1800 f03f  ....._.?a......?
-000009b0: dfb4 46be 42fc ef3f 2721 3846 4d02 f03f  ..F.B..?'!8FM..?
-000009c0: 2721 3846 4d02 f03f f1ad a24a 6a03 f03f  '!8FM..?...Jj..?
-000009d0: d578 e926 3108 f03f 35a1 035c 0820 733f  .x.&1..?5..\. s?
-000009e0: 7752 553f 1409 dc3f e09b df08 3944 c43f  wRU?...?....9D.?
-000009f0: 4ca3 9ad4 27a8 ea3f bbf8 f476 0e00 f03f  L...'..?...v...?
-00000a00: 61aa 9cf3 1800 f03f 0000 0000 0000 f03f  a......?.......?
-00000a10: 4824 a566 6666 1640 5d42 4b8a 278d ef3f  H$.fff.@]BK.'..?
-00000a20: eb4b 4aae abff ef3f e739 85eb 2164 c53f  .KJ....?.9..!d.?
-00000a30: 78a2 18f8 beff ef3f 1672 11fd 69fc ef3f  x......?.r..i..?
-00000a40: 274d 18b4 ef02 f03f 274d 18b4 ef02 f03f  'M.....?'M.....?
-00000a50: 287c 35bd 1804 f03f d578 e926 3108 f03f  (|5....?.x.&1..?
-00000a60: ba86 f75e f0f0 763f 6db8 09c7 f500 dc3f  ...^..v?m......?
-00000a70: 11d4 5832 7944 c43f 01b4 e75c d9a6 ea3f  ..X2yD.?...\...?
-00000a80: eb4b 4aae abff ef3f 78a2 18f8 beff ef3f  .KJ....?x......?
-00000a90: 0000 0000 0000 f03f 2924 a566 6666 1640  .......?)$.fff.@
-00000aa0: e261 4520 7b8c ef3f 2fc5 9a35 7cff ef3f  .aE {..?/..5|..?
-00000ab0: 5263 17af e665 c53f 87d8 760d 8dff ef3f  Rc...e.?..v....?
-00000ac0: f90e c122 a6fc ef3f 1533 585b 7b03 f03f  ..."...?.3X[{..?
-00000ad0: 1533 585b 7b03 f03f 2282 671e 9d04 f03f  .3X[{..?".g....?
-00000ae0: d578 e926 3108 f03f 5a84 87dd 43d6 793f  .x.&1..?Z...C.y?
-00000af0: 7641 9da8 9ef9 db3f 4609 7570 a544 c43f  vA.....?F.up.D.?
-00000b00: eb80 8f44 62a6 ea3f 2fc5 9a35 7cff ef3f  ...Db..?/..5|..?
-00000b10: 87d8 760d 8dff ef3f 0000 0000 0000 f03f  ..v....?.......?
-00000b20: 0a24 a566 6666 1640 7f72 32f7 df8b ef3f  .$.fff.@.r2....?
-00000b30: 0cd4 a90f 6eff ef3f 34da 5376 1166 c53f  ....n..?4.Sv.f.?
-00000b40: 1f51 af5a 7cff ef3f e377 39bd e9fc ef3f  .Q.Z|..?.w9....?
-00000b50: 8ed5 a694 f503 f03f 8ed5 a694 f503 f03f  .......?.......?
-00000b60: 0915 e2f8 0605 f03f d578 e926 3108 f03f  .......?.x.&1..?
-00000b70: 34a3 c458 0b27 7c3f cf17 389f f4f2 db3f  4..X.'|?..8....?
-00000b80: bceb 3a18 c744 c43f 1144 b754 57a6 ea3f  ..:..D.?.D.TW..?
-00000b90: 0cd4 a90f 6eff ef3f 1f51 af5a 7cff ef3f  ....n..?.Q.Z|..?
-00000ba0: 0000 0000 0000 f03f f223 a566 6666 1640  .......?.#.fff.@
-00000bb0: 9374 c754 548b ef3f a722 7355 70ff ef3f  .t.TT..?."sUp..?
-00000bc0: 0d68 b715 7565 c53f effd 3743 7cff ef3f  .h..ue.?..7C|..?
-00000bd0: c9b6 3d0d 2efd ef3f a6b7 bfcb 6104 f03f  ..=....?....a..?
-00000be0: a6b7 bfcb 6104 f03f e7d3 3507 5f05 f03f  ....a..?..5._..?
-00000bf0: d578 e926 3108 f03f 90e4 f660 2814 7e3f  .x.&1..?...`(.~?
-00000c00: bdf7 e65a e6ec db3f 3593 8ed0 e244 c43f  ...Z...?5....D.?
-00000c10: a63d ddc6 80a6 ea3f a722 7355 70ff ef3f  .=.....?."sUp..?
-00000c20: effd 3743 7cff ef3f 0000 0000 0000 f03f  ..7C|..?.......?
-00000c30: db23 a566 6666 1640 0b36 11ab d68a ef3f  .#.fff.@.6.....?
-00000c40: 9026 0f70 7aff ef3f f3b0 ee92 7c64 c53f  .&.pz..?....|d.?
-00000c50: 470a e04a 84ff ef3f 5941 3acf 6ffd ef3f  G..J...?YA:.o..?
-00000c60: d6e8 3455 c204 f03f d6e8 3455 c204 f03f  ..4U...?..4U...?
-00000c70: de4b 4f58 aa05 f03f d578 e926 3108 f03f  .KOX...?.x.&1..?
-00000c80: 03ea 3489 eeb9 7f3f 40a8 4834 67e7 db3f  ..4....?@.H4g..?
-00000c90: 4f8c 12d0 fa44 c43f 4c43 2853 c2a6 ea3f  O....D.?LC(S...?
-00000ca0: 9026 0f70 7aff ef3f 470a e04a 84ff ef3f  .&.pz..?G..J...?
-00000cb0: 0000 0000 0000 f03f ca23 a566 6666 1640  .......?.#.fff.@
-00000cc0: bd9b ff93 658a ef3f 9e79 8be6 87ff ef3f  ....e..?.y.....?
-00000cd0: 049f a099 5f63 c53f 3e72 39fd 8fff ef3f  ...._c.?>r9....?
-00000ce0: c353 5083 adfd ef3f 4017 47df 1805 f03f  .SP....?@.G....?
-00000cf0: 4017 47df 1805 f03f 0eaf 9001 ec05 f03f  @.G....?.......?
-00000d00: d578 e926 3108 f03f c265 e52e d194 803f  .x.&1..?.e.....?
-00000d10: 98be 96c3 6ce2 db3f 9bb5 c625 1045 c43f  ....l..?...%.E.?
-00000d20: 58a9 214b 0da7 ea3f 9e79 8be6 87ff ef3f  X.!K...?.y.....?
-00000d30: 3e72 39fd 8fff ef3f 0000 0000 0000 f03f  >r9....?.......?
-00000d40: b823 a566 6666 1640 6c0a 64cd ff89 ef3f  .#.fff.@l.d....?
-00000d50: e93b 6b50 96ff ef3f 9ac3 881b 3c62 c53f  .;kP...?....<b.?
-00000d60: 310b a9ec 9cff ef3f 928b dc93 e6fd ef3f  1......?.......?
-00000d70: c998 0ab1 6605 f03f c998 0ab1 6605 f03f  ....f..?....f..?
-00000d80: 890f 9bfc 2506 f03f d578 e926 3108 f03f  ....%..?.x.&1..?
-00000d90: 93b6 5bb2 2937 813f 65c4 a08d eddd db3f  ..[.)7.?e......?
-00000da0: ccaa 6369 2345 c43f 97af 62cf 59a7 ea3f  ..ci#E.?..b.Y..?
-00000db0: e93b 6b50 96ff ef3f 310b a9ec 9cff ef3f  .;kP...?1......?
-00000dc0: 0000 0000 0000 f03f aa23 a566 6666 1640  .......?.#.fff.@
-00000dd0: f938 5735 a489 ef3f ac88 0564 a4ff ef3f  .8W5...?...d...?
-00000de0: 14fe c40d 2261 c53f bb14 c1c6 a9ff ef3f  ...."a.?.......?
-00000df0: 34b8 ade8 1afe ef3f a0f6 70cf ac05 f03f  4......?..p....?
-00000e00: a0f6 70cf ac05 f03f 6690 f69c 5906 f03f  ..p....?f...Y..?
-00000e10: d578 e926 3108 f03f eab7 5f7f b7c7 813f  .x.&1..?.._....?
-00000e20: af06 305c e0d9 db3f 56d9 9600 3545 c43f  ..0\...?V...5E.?
-00000e30: 033e cbb2 a3a7 ea3f ac88 0564 a4ff ef3f  .>.....?...d...?
-00000e40: bb14 c1c6 a9ff ef3f 0000 0000 0000 f03f  .......?.......?
-00000e50: 9a23 a566 6666 1640 0feb fbc6 5189 ef3f  .#.fff.@....Q..?
-00000e60: f70c c67d b1ff ef3f 12b4 f143 1960 c53f  ...}...?...C.`.?
-00000e70: 68aa 5fde b5ff ef3f 72c2 03ac 4afe ef3f  h._....?r...J..?
-00000e80: eb95 4513 ec05 f03f eb95 4513 ec05 f03f  ..E....?..E....?
-00000e90: 550e afd2 8706 f03f d578 e926 3108 f03f  U......?.x.&1..?
-00000ea0: a023 28b7 1a49 823f a58f 2b02 3cd6 db3f  .#(..I.?..+.<..?
-00000eb0: 60e4 5c33 4545 c43f 44fb 16ed e8a7 ea3f  `.\3EE.?D......?
-00000ec0: f70c c67d b1ff ef3f 68aa 5fde b5ff ef3f  ...}...?h._....?
-00000ed0: 0000 0000 0000 f03f 9023 a566 6666 1640  .......?.#.fff.@
-00000ee0: 2628 9597 0789 ef3f c40a 045a bdff ef3f  &(.....?...Z...?
-00000ef0: 6399 93da 245f c53f 8eb5 d8e6 c0ff ef3f  c...$_.?.......?
-00000f00: dd2a 5d28 76fe ef3f 8986 2436 2506 f03f  .*](v..?..$6%..?
-00000f10: 8986 2436 2506 f03f 56ca 7551 b106 f03f  ..$6%..?V.uQ...?
-00000f20: d578 e926 3108 f03f 3cd2 377d 4abd 823f  .x.&1..?<.7}J..?
-00000f30: e3c8 5960 f7d2 db3f 8aab ff34 5445 c43f  ..Y`...?...4TE.?
-00000f40: 5760 63b3 28a8 ea3f c40a 045a bdff ef3f  W`c.(..?...Z...?
-00000f50: 8eb5 d8e6 c0ff ef3f 0000 0000 0000 f03f  .......?.......?
-00000f60: 8423 a566 6666 1640 777a e7d3 c488 ef3f  .#.fff.@wz.....?
-00000f70: 5313 0dea c7ff ef3f 7d00 0152 455e c53f  S......?}..RE^.?
-00000f80: 43c5 86c9 caff ef3f 173a b5b4 9dfe ef3f  C......?.:.....?
-00000f90: 8326 28da 5806 f03f 8326 28da 5806 f03f  .&(.X..?.&(.X..?
-00000fa0: 919d 80a7 d606 f03f d578 e926 3108 f03f  .......?.x.&1..?
-00000fb0: 6dd0 ee01 d525 833f 7e09 118a 09d0 db3f  m....%.?~......?
-00000fc0: fe93 062a 6245 c43f 04cb d1e9 62a8 ea3f  ...*bE.?....b..?
-00000fd0: 5313 0dea c7ff ef3f 43c5 86c9 caff ef3f  S......?C......?
-00000fe0: 0000 0000 0000 f03f 7a23 a566 6666 1640  .......?z#.fff.@
-00000ff0: 119f ddbd 8888 ef3f 31d8 7f39 d1ff ef3f  .......?1..9...?
-00001000: 1120 ffde 795d c53f eda1 448b d3ff ef3f  . ..y].?..D....?
-00001010: a1cd a2a9 c1fe ef3f c965 958e 8706 f03f  .......?.e.....?
-00001020: c965 958e 8706 f03f 60f5 ac4a f806 f03f  .e.....?`..J...?
-00001030: d578 e926 3108 f03f 42b5 e54a 0484 833f  .x.&1..?B..J...?
-00001040: 85e8 baf0 69cd db3f 6b87 682d 6f45 c43f  ....i..?k.h-oE.?
-00001050: df04 d0ca 97a8 ea3f 31d8 7f39 d1ff ef3f  .......?1..9...?
-00001060: eda1 448b d3ff ef3f 0000 0000 0000 f03f  ..D....?.......?
-00001070: 7223 a566 6666 1640 acd6 69aa 5288 ef3f  r#.fff.@..i.R..?
-00001080: 8abf 3160 d9ff ef3f a1e8 c61d c15c c53f  ..1`...?.....\.?
-00001090: 5577 413e dbff ef3f eee8 fe5b e2fe ef3f  UwA>...?...[...?
-000010a0: 2968 ebd2 b106 f03f 2968 ebd2 b106 f03f  )h.....?)h.....?
-000010b0: 42c5 db9f 1607 f03f d578 e926 3108 f03f  B......?.x.&1..?
-000010c0: 0783 f9cd f2d8 833f 7a51 8688 10cb db3f  .......?zQ.....?
-000010d0: 0446 c153 7b45 c43f f764 09b8 c7a8 ea3f  .F.S{E.?.d.....?
-000010e0: 8abf 3160 d9ff ef3f 5577 413e dbff ef3f  ..1`...?UwA>...?
-000010f0: 0000 0000 0000 f03f 6a23 a566 6666 1640  .......?j#.fff.@
-00001100: bfb8 9dff 2188 ef3f fc8b 2a7a e0ff ef3f  ....!..?..*z...?
-00001110: 7034 6178 195c c53f f0bb d9f9 e1ff ef3f  p4ax.\.?.......?
-00001120: fb4a 791a 00ff ef3f e818 0919 d806 f03f  .Jy....?.......?
-00001130: e818 0919 d806 f03f 8dc8 38ff 3107 f03f  .......?..8.1..?
-00001140: d578 e926 3108 f03f e492 036c 9725 843f  .x.&1..?...l.%.?
-00001150: 85e1 a4e1 f5c8 db3f ad68 1bae 8645 c43f  .......?.h...E.?
-00001160: 65bb 951f f3a8 ea3f fc8b 2a7a e0ff ef3f  e......?..*z...?
-00001170: f0bb d9f9 e1ff ef3f 0000 0000 0000 f03f  .......?.......?
-00001180: 6423 a566 6666 1640 b609 f332 f687 ef3f  d#.fff.@...2...?
-00001190: ff3f b4a3 e6ff ef3f 6500 2159 815b c53f  .?.....?e.!Y.[.?
-000011a0: 598c 80d6 e7ff ef3f 93f4 d72c 1bff ef3f  Y......?...,...?
-000011b0: a574 d2c6 fa06 f03f a574 d2c6 fa06 f03f  .t.....?.t.....?
-000011c0: 8792 c1b6 4a07 f03f d578 e926 3108 f03f  ....J..?.x.&1..?
-000011d0: 2044 a084 cc6a 843f 7b4c f835 13c7 db3f   D...j.?{L.5...?
-000011e0: 563c c14b 9145 c43f 5cac d26e 1aa9 ea3f  V<.K.E.?\..n...?
-000011f0: ff3f b4a3 e6ff ef3f 598c 80d6 e7ff ef3f  .?.....?Y......?
-00001200: 0000 0000 0000 f03f 5e23 a566 6666 1640  .......?^#.fff.@
-00001210: 0ea4 c0c7 ce87 ef3f af2c 8ff7 ebff ef3f  .......?.,.....?
-00001220: ebfe b841 f75a c53f 4bc4 cfeb ecff ef3f  ...A.Z.?K......?
-00001230: 437b 07d4 33ff ef3f 3293 8937 1a07 f03f  C{..3..?2..7...?
-00001240: 3293 8937 1a07 f03f 8586 e30b 6107 f03f  2..7...?....a..?
-00001250: d578 e926 3108 f03f 551f 4c7d 54a9 843f  .x.&1..?U.L}T..?
-00001260: 4984 e06c 62c5 db3f ad56 443b 9b45 c43f  I..lb..?.VD;.E.?
-00001270: baba 6f0c 3ea9 ea3f af2c 8ff7 ebff ef3f  ..o.>..?.,.....?
-00001280: 4bc4 cfeb ecff ef3f 0000 0000 0000 f03f  K......?.......?
-00001290: 5823 a566 6666 1640 7804 d74d ab87 ef3f  X#.fff.@x..M...?
-000012a0: 6a4d 4a8e f0ff ef3f 7bee 8ed3 795a c53f  jMJ....?{...yZ.?
-000012b0: f91b c14f f1ff ef3f ad61 894a 4aff ef3f  ...O...?.a.JJ..?
-000012c0: 163e f6bc 3607 f03f 163e f6bc 3607 f03f  .>..6..?.>..6..?
-000012d0: 004c 9e3c 7507 f03f d578 e926 3108 f03f  .L.<u..?.x.&1..?
-000012e0: a6e2 a8ee dce1 843f 86eb 4917 dec3 db3f  .......?..I....?
-000012f0: 6a9f ec8a a445 c43f 8fc4 5756 5ea9 ea3f  j....E.?..WV^..?
-00001300: 6a4d 4a8e f0ff ef3f f91b c14f f1ff ef3f  jMJ....?...O...?
-00001310: 0000 0000 0000 f03f 5323 a566 6666 1640  .......?S#.fff.@
-00001320: 007c 4060 8b87 ef3f d49d f77d f4ff ef3f  .|@`...?...}...?
-00001330: fc5a 6dd3 075a c53f a549 4816 f5ff ef3f  .Zm..Z.?.IH....?
-00001340: 30e6 02c5 5eff ef3f 1ad4 68a0 5007 f03f  0...^..?..h.P..?
-00001350: 1ad4 68a0 5007 f03f 1e6a 6480 8707 f03f  ..h.P..?.jd....?
-00001360: d578 e926 3108 f03f 922c 6419 0115 853f  .x.&1..?.,d....?
-00001370: 1bfe 1566 81c2 db3f 6eeb e848 ad45 c43f  ...f...?n..H.E.?
-00001380: a906 cea0 7ba9 ea3f d49d f77d f4ff ef3f  ....{..?...}...?
-00001390: a549 4816 f5ff ef3f 0000 0000 0000 f03f  .IH....?.......?
-000013a0: 4f23 a566 6666 1640 a372 21a4 6e87 ef3f  O#.fff.@.r!.n..?
-000013b0: 89ca 30da f7ff ef3f 167c 0a29 a059 c53f  ..0....?.|.).Y.?
-000013c0: f204 4251 f8ff ef3f f14d d972 71ff ef3f  ..BQ...?.M.rq..?
-000013d0: e8b7 a123 6807 f03f e8b7 a123 6807 f03f  ...#h..?...#h..?
-000013e0: 5453 d008 9807 f03f d578 e926 3108 f03f  TS.....?.x.&1..?
-000013f0: 2edf 24e1 4b43 853f 7fc7 d31c 48c1 db3f  ..$.KC.?....H..?
-00001400: ccac 4083 b545 c43f 0c73 9f36 96a9 ea3f  ..@..E.?.s.6...?
-00001410: 89ca 30da f7ff ef3f f204 4251 f8ff ef3f  ..0....?..BQ...?
-00001420: 0000 0000 0000 f03f 4923 a566 6666 1640  .......?I#.fff.@
-00001430: 6f81 b5c7 5487 ef3f a902 52b4 faff ef3f  o...T..?..R....?
-00001440: 49f7 bcdb 4159 c53f 631b 9d10 fbff ef3f  I...AY.?c......?
-00001450: 6d93 ca7e 82ff ef3f 03f8 a181 7d07 f03f  m..~...?....}..?
-00001460: 03f8 a181 7d07 f03f 02b5 3f02 a707 f03f  ....}..?..?....?
-00001470: d578 e926 3108 f03f 6709 6a7f 396d 853f  .x.&1..?g.j.9m.?
-00001480: 5e12 8a82 2ec0 db3f 58a0 9e47 bd45 c43f  ^......?X..G.E.?
-00001490: 6944 0e5a aea9 ea3f a902 52b4 faff ef3f  iD.Z...?..R....?
-000014a0: 631b 9d10 fbff ef3f 0000 0000 0000 f03f  c......?.......?
-000014b0: 4623 a566 6666 1640 6d7e 6681 3d87 ef3f  F#.fff.@m~f.=..?
-000014c0: 3681 a11b fdff ef3f 0181 4b10 ec58 c53f  6......?..K..X.?
-000014d0: 648d 7362 fdff ef3f 1cf3 760f 92ff ef3f  d.sb...?..v....?
-000014e0: a6ba 66ef 9007 f03f a6ba 66ef 9007 f03f  ..f....?..f....?
-000014f0: 3383 5f94 b407 f03f d578 e926 3108 f03f  3._....?.x.&1..?
-00001500: 7fc9 ab0b 3993 853f 5a5b 0452 31bf db3f  ....9..?Z[.R1..?
-00001510: 18f4 2aa3 c445 c43f 7bd6 7045 c4a9 ea3f  ..*..E.?{.pE...?
-00001520: 3681 a11b fdff ef3f 648d 7362 fdff ef3f  6......?d.sb...?
-00001530: 0000 0000 0000 f03f 4523 a566 6666 1640  .......?E#.fff.@
-00001540: 9bdf fa8e 2887 ef3f 0827 bf1d ffff ef3f  ....(..?.'.....?
-00001550: 4335 da02 9e58 c53f ce67 6e53 ffff ef3f  C5...X.?.gnS...?
-00001560: f33e e047 a0ff ef3f dc0c 939c a207 f03f  .>.G...?.......?
-00001570: dc0c 939c a207 f03f d8d8 a7e2 c007 f03f  .......?.......?
-00001580: d578 e926 3108 f03f 5d90 35d6 adb5 853f  .x.&1..?].5....?
-00001590: 61e1 b5aa 4dbe db3f 9ab1 3aa2 cb45 c43f  a...M..?..:..E.?
-000015a0: 14d4 d22c d8a9 ea3f 0827 bf1d ffff ef3f  ...,...?.'.....?
-000015b0: ce67 6e53 ffff ef3f 0000 0000 0000 f03f  .gnS...?.......?
-000015c0: 4023 a566 6666 1640 311d d9b4 1587 ef3f  @#.fff.@1......?
-000015d0: 5174 9663 0000 f03f 51dc 87ff 5658 c53f  Qt.c...?Q...VX.?
-000015e0: dd57 a277 0000 f03f 37df ce47 adff ef3f  .W.w...?7..G...?
-000015f0: 072c 07b4 b207 f03f 072c 07b4 b207 f03f  .,.....?.,.....?
-00001600: 615f d30c cc07 f03f d578 e926 3108 f03f  a_.....?.x.&1..?
-00001610: 7e67 7bb6 f0d4 853f 71f0 e902 81bd db3f  ~g{....?q......?
-00001620: 0aa0 f64f d245 c43f 82a8 ec3f eaa9 ea3f  ...O.E.?...?...?
-00001630: 5174 9663 0000 f03f dd57 a277 0000 f03f  Qt.c...?.W.w...?
-00001640: 0000 0000 0000 f03f 3d23 a566 6666 1640  .......?=#.fff.@
-00001650: f3f7 5dbd 0487 ef3f ab5b c011 0100 f03f  ..]....?.[.....?
-00001660: 358a b55f 1658 c53f bfca 7220 0100 f03f  5.._.X.?..r ...?
-00001670: 2421 172c b9ff ef3f 741c 635c c107 f03f  $!.,...?t.c\...?
-00001680: 741c 635c c107 f03f 4d08 542f d607 f03f  t.c\...?M.T/...?
-00001690: d578 e926 3108 f03f a84b ee51 51f1 853f  .x.&1..?.K.QQ..?
-000016a0: c8ea 991b c9bc db3f d786 45b6 d845 c43f  .......?..E..E.?
-000016b0: cb67 e0aa faa9 ea3f ab5b c011 0100 f03f  .g.....?.[.....?
-000016c0: bfca 7220 0100 f03f 0000 0000 0000 f03f  ..r ...?.......?
-000016d0: 3b23 a566 6666 1640 8fbe 4378 f586 ef3f  ;#.fff.@..Cx...?
-000016e0: 718d bd9e 0100 f03f 81b8 da88 db57 c53f  q......?.....W.?
-000016f0: 2359 44a9 0100 f03f 3f89 d20e c4ff ef3f  #YD....??......?
-00001700: 067b 77b8 ce07 f03f 067b 77b8 ce07 f03f  .{w....?.{w....?
-00001710: 480d b963 df07 f03f d578 e926 3108 f03f  H..c...?.x.&1..?
-00001720: 391f 9639 170b 863f 5ded f7f5 23bc db3f  9..9...?]...#..?
-00001730: bad4 d1dd de45 c43f dee6 8d96 09aa ea3f  .....E.?.......?
-00001740: 718d bd9e 0100 f03f 2359 44a9 0100 f03f  q......?#YD....?
-00001750: 0000 0000 0000 f03f 3923 a566 6666 1640  .......?9#.fff.@
-00001760: b5dd 18ba e786 ef3f 448f c70f 0200 f03f  .......?D......?
-00001770: 078d fee4 a557 c53f 1558 1817 0200 f03f  .....W.?.X.....?
-00001780: 6ec2 9307 ceff ef3f c7b0 a8e7 da07 f03f  n......?.......?
-00001790: c7b0 a8e7 da07 f03f 35d8 05c1 e707 f03f  .......?5......?
-000017a0: d578 e926 3108 f03f 2b2d 68dd 8222 863f  .x.&1..?+-h..".?
-000017b0: d885 9dca 8fbb db3f da0a cecd e445 c43f  .......?.....E.?
-000017c0: bb82 8f2a 17aa ea3f 448f c70f 0200 f03f  ...*...?D......?
-000017d0: 1558 1817 0200 f03f 0000 0000 0000 f03f  .X.....?.......?
-000017e0: 3723 a566 6666 1640 8d32 c45b db86 ef3f  7#.fff.@.2.[...?
-000017f0: a5de 2c6a 0200 f03f 4ebd 27dc 7457 c53f  ..,j...?N.'.tW.?
-00001800: f632 0f6f 0200 f03f 5898 7a2b d7ff ef3f  .2.o...?X.z+...?
-00001810: bd26 4106 e607 f03f bd26 4106 e607 f03f  .&A....?.&A....?
-00001820: 7f4a 0b5c ef07 f03f d578 e926 3108 f03f  .J.\...?.x.&1..?
-00001830: 0c04 4286 ce37 863f 9574 3d02 0bbb db3f  ..B..7.?.t=....?
-00001840: e798 d08b ea45 c43f fab0 f58e 23aa ea3f  .....E.?....#..?
-00001850: a5de 2c6a 0200 f03f f632 0f6f 0200 f03f  ..,j...?.2.o...?
-00001860: 0000 0000 0000 f03f 3523 a566 6666 1640  .......?5#.fff.@
-00001870: 98be 153a d086 ef3f c524 28b3 0200 f03f  ...:...?.$(....?
-00001880: 3518 e8d8 4757 c53f a6d3 3db6 0200 f03f  5...GW.?..=....?
-00001890: 430b 2c8d dfff ef3f 78d5 af2d f007 f03f  C.,....?x..-...?
-000018a0: 78d5 af2d f007 f03f f5fa bd47 f607 f03f  x..-...?...G...?
-000018b0: d578 e926 3108 f03f c585 6347 2f4b 863f  .x.&1..?..cG/K.?
-000018c0: 8ce2 982f 94ba db3f bc66 3e1c f045 c43f  .../...?.f>..E.?
-000018d0: da86 19eb 2eaa ea3f c524 28b3 0200 f03f  .......?.$(....?
-000018e0: a6d3 3db6 0200 f03f 0000 0000 0000 f03f  ..=....?.......?
-000018f0: 3423 a566 6666 1640 517f 6235 c686 ef3f  4#.fff.@Q.b5...?
-00001900: d2a2 94ef 0200 f03f 0b7e 6650 1e57 c53f  .......?.~fP.W.?
-00001910: 9b83 60f1 0200 f03f ce20 dd3c e7ff ef3f  ..`....?. .<...?
-00001920: bd3f bb74 f907 f03f bd3f bb74 f907 f03f  .?.t...?.?.t...?
-00001930: 0769 6f95 fc07 f03f d578 e926 3108 f03f  .io....?.x.&1..?
-00001940: 31ea 979e d55c 863f 02e5 680a 2aba db3f  1....\.?..h.*..?
-00001950: b67a e282 f545 c43f 9ba0 8363 39aa ea3f  .z...E.?...c9..?
-00001960: d2a2 94ef 0200 f03f 9b83 60f1 0200 f03f  .......?..`....?
-00001970: 0000 0000 0000 f03f 3123 a566 6666 1640  .......?1#.fff.@
-00001980: fb4b 2a31 bd86 ef3f 4668 0f24 0300 f03f  .K*1...?Fh.$...?
-00001990: 5b01 12be f756 c53f 6dd2 fa24 0300 f03f  [....V.?m..$...?
-000019a0: 8942 7f48 eeff ef3f bd14 b3ef 0108 f03f  .B.H...?.......?
-000019b0: bd14 b3ef 0108 f03f 24c9 ea54 0208 f03f  .......?$..T...?
-000019c0: d578 e926 3108 f03f 3267 d8c4 ed6c 863f  .x.&1..?2g...l.?
-000019d0: f4ba 0a6b cbb9 db3f 2d9e eec2 fa45 c43f  ...k...?-....E.?
-000019e0: 1ea1 0c1b 43aa ea3f 4668 0f24 0300 f03f  ....C..?Fh.$...?
-000019f0: 6dd2 fa24 0300 f03f 0000 0000 0000 f03f  m..$...?.......?
-00001a00: 3023 a566 6666 1640 9cb8 c613 b586 ef3f  0#.fff.@.......?
-00001a10: 8018 bb54 0300 f03f 2e2e c0a8 d356 c53f  ...T...?.....V.?
-00001a20: 994a 1a55 0300 f03f 638a dabb f4ff ef3f  .J.U...?c......?
-00001a30: eaf9 99b0 0908 f03f eaf9 99b0 0908 f03f  .......?.......?
-00001a40: 2384 9994 0708 f03f d578 e926 3108 f03f  #......?.x.&1..?
-00001a50: 56bf 7d14 a07b 863f 85bf c846 77b9 db3f  V.}..{.?...Fw..?
-00001a60: 1d05 6ddf ff45 c43f 5856 8331 4caa ea3f  ..m..E.?XV.1L..?
-00001a70: 8018 bb54 0300 f03f 994a 1a55 0300 f03f  ...T...?.J.U...?
-00001a80: 0000 0000 0000 f03f 2d23 a566 6666 1640  .......?-#.fff.@
-00001a90: c016 22c6 ad86 ef3f 3b22 fd83 0300 f03f  .."....?;".....?
-00001aa0: 7d76 66d5 b156 c53f 47c7 1284 0300 f03f  }vf..V.?G......?
-00001ab0: 55b2 bda0 faff ef3f 06eb 48c7 1008 f03f  U......?..H....?
-00001ac0: 06eb 48c7 1008 f03f 6e05 9561 0c08 f03f  ..H....?n..a...?
-00001ad0: d578 e926 3108 f03f ce1f 1b3b 1189 863f  .x.&1..?...;...?
-00001ae0: 7679 55ac 2cb9 db3f 7229 f0dc 0446 c43f  vyU.,..?r)...F.?
-00001af0: fe3d 94b6 54aa ea3f 3b22 fd83 0300 f03f  .=..T..?;".....?
-00001b00: 47c7 1284 0300 f03f 0000 0000 0000 f03f  G......?.......?
-00001b10: 6666 6666 6666 1640 2788 a40b 6c86 ef3f  ffffff.@'...l..?
-00001b20: 4ba2 4100 0000 f03f 5455 5555 5555 c53f  K.A....?TUUUUU.?
-00001b30: 0000 0000 0000 f03f 0000 0000 0000 f03f  .......?.......?
-00001b40: 2287 e926 3108 f03f 9586 e926 3108 f03f  "..&1..?...&1..?
-00001b50: ae87 e926 3108 f03f d578 e926 3108 f03f  ...&1..?.x.&1..?
-00001b60: 2074 b3ae 06f0 863f 11d1 5dbe b6b8 db3f   t.....?..]....?
-00001b70: 8ffd a762 6746 c43f abaa aaaa aaaa ea3f  ...bgF.?.......?
-00001b80: 0000 0000 0000 f03f 0000 0000 0000 f03f  .......?.......?
-00001b90: 0000 0000 0000 f03f                      .......?
+00000080: 6666 6666 6666 1640 2188 a40b 6c86 ef3f  ffffff.@!...l..?
+00000090: 4ca2 4100 0000 f03f 5455 5555 5555 c53f  L.A....?TUUUUU.?
+000000a0: abaa aaaa aaaa ea3f 0000 0000 0000 f03f  .......?.......?
+000000b0: 0000 0000 0000 f03f 2587 e926 3108 f03f  .......?%..&1..?
+000000c0: 9886 e926 3108 f03f b187 e926 3108 f03f  ...&1..?...&1..?
+000000d0: d578 e926 3108 f03f e37c b3ae 06f0 863f  .x.&1..?.|.....?
+000000e0: f2d0 5dbe b6b8 db3f 8afd a762 6746 c43f  ..]....?...bgF.?
+000000f0: abaa aaaa aaaa ea3f 0000 0000 0000 f03f  .......?.......?
+00000100: 0000 0000 0000 f03f 0000 0000 0000 f03f  .......?.......?
+00000110: 8722 a566 6666 1640 eafe dc0d e0ae ef3f  .".fff.@.......?
+00000120: 3a63 d1ec d97e ee3f 43c2 4ccb 8b5f cf3f  :c...~.?C.L.._.?
+00000130: 3c88 1d26 f01f e73f 7289 cce9 9858 ef3f  <..&...?r....X.?
+00000140: c33c 78a4 393d ef3f 21c8 faff ffff ef3f  .<x.9=.?!......?
+00000150: feee 03e7 7ecd ef3f 2f22 2a9d 266c f03f  ....~..?/"*.&l.?
+00000160: d578 e926 3108 f03f 81fd fa4d 28ed c23f  .x.&1..?...M(..?
+00000170: c445 9cb5 6d18 dc3f 42ec ae37 a0ab c43f  .E..m..?B..7...?
+00000180: 3c88 1d26 f01f e73f 3a63 d1ec d97e ee3f  <..&...?:c...~.?
+00000190: 7289 cce9 9858 ef3f 0000 0000 0000 f03f  r....X.?.......?
+000001a0: 7a24 a566 6666 1640 7d36 231f d2aa ef3f  z$.fff.@}6#....?
+000001b0: 76ca 62cb 60f8 ee3f f146 7a04 cfcc cd3f  v.b.`..?.Fz....?
+000001c0: 4175 915c d0f8 e73f 2a30 51af a265 ef3f  Au.\...?*0Q..e.?
+000001d0: 58ce 3e77 2476 ef3f da4c f8ff ffff ef3f  X.>w$v.?.L.....?
+000001e0: 68b7 680e ecb3 ef3f 7588 5acc 1b46 f03f  h.h....?u.Z..F.?
+000001f0: d578 e926 3108 f03f 3918 8eb9 ba89 b83f  .x.&1..?9......?
+00000200: 868e 3aaf e050 dc3f b23c 1775 d88c c43f  ..:..P.?.<.u...?
+00000210: 4175 915c d0f8 e73f 76ca 62cb 60f8 ee3f  Au.\...?v.b.`..?
+00000220: 2a30 51af a265 ef3f 0000 0000 0000 f03f  *0Q..e.?.......?
+00000230: d425 a566 6666 1640 1b9b 0c6d 2ca7 ef3f  .%.fff.@...m,..?
+00000240: 551e 5b34 f04c ef3f 5260 e14c c410 cc3f  U.[4.L.?R`.L...?
+00000250: 0036 cc3f 44ab e83f 97a6 57d1 3380 ef3f  .6.?D..?..W.3..?
+00000260: b1c0 99aa b9a1 ef3f 2638 f7ff ffff ef3f  .......?&8.....?
+00000270: ca34 e18e daab ef3f a3a4 7aa7 af2f f03f  .4.....?..z../.?
+00000280: d578 e926 3108 f03f 7ffa 81d1 adb0 b03f  .x.&1..?.......?
+00000290: 616b 255c 4973 dc3f bdb4 6906 9278 c43f  ak%\Is.?..i..x.?
+000002a0: 0036 cc3f 44ab e83f 551e 5b34 f04c ef3f  .6.?D..?U.[4.L.?
+000002b0: 97a6 57d1 3380 ef3f 0000 0000 0000 f03f  ..W.3..?.......?
+000002c0: 9126 a566 6666 1640 a207 8475 e4a3 ef3f  .&.fff.@...u...?
+000002d0: 31cd b522 228a ef3f 68f9 0d53 354c ca3f  1..""..?h..S5L.?
+000002e0: 0f91 541a 9942 e93f 0cd0 3f81 55a0 ef3f  ..T..B.?..?.U..?
+000002f0: 2394 9750 15c2 ef3f 6e2c f7ff ffff ef3f  #..P...?n,.....?
+00000300: a990 73c4 9dae ef3f 6ecc 33b3 311f f03f  ..s....?n.3.1..?
+00000310: d578 e926 3108 f03f 4b46 4c71 fdd5 a53f  .x.&1..?KFLq...?
+00000320: de27 27c1 9c84 dc3f d681 bd45 d868 c43f  .''....?...E.h.?
+00000330: 0f91 541a 9942 e93f 31cd b522 228a ef3f  ..T..B.?1..""..?
+00000340: 0cd0 3f81 55a0 ef3f 0000 0000 0000 f03f  ..?.U..?.......?
+00000350: f526 a566 6666 1640 67e1 94c7 f0a0 ef3f  .&.fff.@g......?
+00000360: f2a4 2e84 ddb4 ef3f 7a6a 19c8 b5c4 c83f  .......?zj.....?
+00000370: 7081 8b84 e9b8 e93f c588 1b2e c9bd ef3f  p......?.......?
+00000380: a270 e3a6 d2d8 ef3f 0ece f7ff ffff ef3f  .p.....?.......?
+00000390: d2c9 90db 3fb7 ef3f 9e0d 6fc5 ae13 f03f  ....?..?..o....?
+000003a0: d578 e926 3108 f03f 7daa c69b 478e 9b3f  .x.&1..?}...G..?
+000003b0: e3dd 6ed1 c589 dc3f 9583 07e8 395d c43f  ..n....?....9].?
+000003c0: 7081 8b84 e9b8 e93f f2a4 2e84 ddb4 ef3f  p......?.......?
+000003d0: c588 1b2e c9bd ef3f 0000 0000 0000 f03f  .......?.......?
+000003e0: 1727 a566 6666 1640 97ea 51e7 489e ef3f  .'.fff.@..Q.H..?
+000003f0: fc2d d7f2 dad1 ef3f 6f4c 78d9 3994 c73f  .-.....?oLx.9..?
+00000400: 4acd be06 a80f ea3f a427 69f4 32d5 ef3f  J......?.'i.2..?
+00000410: 8275 2873 0ce8 ef3f 51cd f8ff ffff ef3f  .u(s...?Q......?
+00000420: 025f 780e 6fc2 ef3f ba42 cec3 020c f03f  ._x.o..?.B.....?
+00000430: d578 e926 3108 f03f 0086 8cba abd0 903f  .x.&1..?.......?
+00000440: 2e0c cd49 d086 dc3f 15af 8be0 ee54 c43f  ...I...?.....T.?
+00000450: 4acd be06 a80f ea3f fc2d d7f2 dad1 ef3f  J......?.-.....?
+00000460: a427 69f4 32d5 ef3f 0000 0000 0000 f03f  .'i.2..?.......?
+00000470: 0827 a566 6666 1640 1ad3 b134 e59b ef3f  .'.fff.@...4...?
+00000480: 80f0 08ab 0ce5 ef3f 38a9 7da6 53b8 c63f  .......?8.}.S..?
+00000490: 802c 8f5d 254c ea3f dfb6 33b9 3ae6 ef3f  .,.]%L.?..3.:..?
+000004a0: 834f 4881 c9f1 ef3f 13ef f9ff ffff ef3f  .OH....?.......?
+000004b0: 84bf c9ec 1ace ef3f 4096 c568 1e07 f03f  .......?@..h...?
+000004c0: d578 e926 3108 f03f 33f0 42f6 beee 833f  .x.&1..?3.B....?
+000004d0: dbe8 4fda c47e dc3f 556b efdf 234f c43f  ..O..~.?Uk..#O.?
+000004e0: 802c 8f5d 254c ea3f 80f0 08ab 0ce5 ef3f  .,.]%L.?.......?
+000004f0: dfb6 33b9 3ae6 ef3f 0000 0000 0000 f03f  ..3.:..?.......?
+00000500: d826 a566 6666 1640 ce65 0ed5 be99 ef3f  .&.fff.@.e.....?
+00000510: 9b56 3616 81f1 ef3f dc32 64c0 8721 c63f  .V6....?.2d..!.?
+00000520: b09c 772c c674 ea3f 6f80 e2e2 e7f1 ef3f  ..w,.t.?o......?
+00000530: 5857 20e3 b6f7 ef3f 520d fbff ffff ef3f  XW ....?R......?
+00000540: 2de5 5152 17d9 ef3f 4cb5 4ea1 2504 f03f  -.QR...?L.N.%..?
+00000550: d578 e926 3108 f03f 3b4e 38ec 2039 773f  .x.&1..?;N8. 9w?
+00000560: 2390 328e c573 dc3f a733 43f5 2e4b c43f  #.2..s.?.3C..K.?
+00000570: b09c 772c c674 ea3f 9b56 3616 81f1 ef3f  ..w,.t.?.V6....?
+00000580: 6f80 e2e2 e7f1 ef3f 0000 0000 0000 f03f  o......?.......?
+00000590: 9426 a566 6666 1640 38ea fc9e cf97 ef3f  .&.fff.@8......?
+000005a0: 7af8 8c81 67f9 ef3f 2ef5 8a83 5ebe c53f  z...g..?....^..?
+000005b0: 0735 964b 2b8f ea3f 282f a7a4 8bf9 ef3f  .5.K+..?(/.....?
+000005c0: 725d d4fa 16fb ef3f 4912 fcff ffff ef3f  r].....?I......?
+000005d0: c97e ac1f cfe2 ef3f 4535 13e3 7402 f03f  .~.....?E5..t..?
+000005e0: d578 e926 3108 f03f 377f 6ed7 8883 6b3f  .x.&1..?7.n...k?
+000005f0: 4030 738b 4067 dc3f a870 5ab8 8448 c43f  @0s.@g.?.pZ..H.?
+00000600: 0735 964b 2b8f ea3f 7af8 8c81 67f9 ef3f  .5.K+..?z...g..?
+00000610: 282f a7a4 8bf9 ef3f 0000 0000 0000 f03f  (/.....?.......?
+00000620: 4526 a566 6666 1640 05ce 3e08 1296 ef3f  E&.fff.@..>....?
+00000630: 8b04 f220 42fe ef3f abc2 8525 d17f c53f  ... B..?...%...?
+00000640: f3ee f31c b49f ea3f 58c8 1962 51fe ef3f  .......?X..bQ..?
+00000650: f0c8 b488 cffc ef3f d2f3 fcff ffff ef3f  .......?.......?
+00000660: 6d71 88cb 0beb ef3f c795 5764 9801 f03f  mq.....?..Wd...?
+00000670: d578 e926 3108 f03f 9f8b bf6e fddd 613f  .x.&1..?...n..a?
+00000680: 48be 7bab 215a dc3f 4208 b409 b746 c43f  H.{.!Z.?B....F.?
+00000690: f3ee f31c b49f ea3f 8b04 f220 42fe ef3f  .......?... B..?
+000006a0: 58c8 1962 51fe ef3f 0000 0000 0000 f03f  X..bQ..?.......?
+000006b0: f725 a566 6666 1640 8d13 9115 8194 ef3f  .%.fff.@.......?
+000006c0: c3a9 d9d5 8900 f03f 6cec d6e1 8b5a c53f  .......?l....Z.?
+000006d0: 3780 cc2d 83a9 ea3f 1e47 6f89 8e00 f03f  7..-...?.Go....?
+000006e0: 084e a316 7ffd ef3f 33af fdff ffff ef3f  .N.....?3......?
+000006f0: 52be fd70 cef1 ef3f 8b07 c18d 4001 f03f  R..p...?....@..?
+00000700: d578 e926 3108 f03f 2423 914a 670c 5c3f  .x.&1..?$#.Jg.\?
+00000710: cfad 944f fa4c dc3f 06bb 7d13 8045 c43f  ...O.L.?..}..E.?
+00000720: 3780 cc2d 83a9 ea3f c3a9 d9d5 8900 f03f  7..-...?.......?
+00000730: 1e47 6f89 8e00 f03f 0000 0000 0000 f03f  .Go....?.......?
+00000740: a725 a566 6666 1640 4881 274c 1893 ef3f  .%.fff.@H.'L...?
+00000750: 1daf bcb9 4301 f03f 8e01 1ba1 8b46 c53f  ....C..?.....F.?
+00000760: e0d9 b147 c1ae ea3f 18f8 6329 4801 f03f  ...G...?..c)H..?
+00000770: aa5c 2e7e 91fd ef3f f045 feff ffff ef3f  .\.~...?.E.....?
+00000780: 7a36 3584 36f7 ef3f b961 9058 3701 f03f  z65.6..?.a.X7..?
+00000790: d578 e926 3108 f03f 5278 0c3c 263e 5b3f  .x.&1..?Rx.<&>[?
+000007a0: 551d 3e5e 1e40 dc3f 4ea9 5e73 b244 c43f  U.>^.@.?N.^s.D.?
+000007b0: e0d9 b147 c1ae ea3f 1daf bcb9 4301 f03f  ...G...?....C..?
+000007c0: 18f8 6329 4801 f03f 0000 0000 0000 f03f  ..c)H..?.......?
+000007d0: 5b25 a566 6666 1640 d941 a6a4 d391 ef3f  [%.fff.@.A.....?
+000007e0: c24d 0aa6 8501 f03f e2f8 ae30 803e c53f  .M.....?...0.>.?
+000007f0: f202 3734 d8b0 ea3f d70b e411 8b01 f03f  ..74...?.......?
+00000800: 5a27 4fdb 4ffd ef3f 9ebb feff ffff ef3f  Z'O.O..?.......?
+00000810: 3670 2cf4 71fb ef3f d111 412f 5801 f03f  6p,.q..?..A/X..?
+00000820: d578 e926 3108 f03f d1db 4918 bc1d 5e3f  .x.&1..?..I...^?
+00000830: 68d3 7557 b833 dc3f 9dd4 a142 2e44 c43f  h.uW.3.?...B.D.?
+00000840: f202 3734 d8b0 ea3f c24d 0aa6 8501 f03f  ..74...?.M.....?
+00000850: d70b e411 8b01 f03f 0000 0000 0000 f03f  .......?.......?
+00000860: 1525 a566 6666 1640 d5a8 717f af90 ef3f  .%.fff.@..q....?
+00000870: 1223 de65 7101 f03f cd5b dec1 183f c53f  .#.eq..?.[...?.?
+00000880: 6411 5090 a8b0 ea3f cf22 c77e 7801 f03f  d.P....?.".~x..?
+00000890: baf1 9fa1 ecfc ef3f 8b14 ffff ffff ef3f  .......?.......?
+000008a0: 9e90 66e3 b3fe ef3f cbbd 09d5 8901 f03f  ..f....?.......?
+000008b0: d578 e926 3108 f03f 5ee9 7da0 eb3a 613f  .x.&1..?^.}..:a?
+000008c0: 4ba8 e05b d727 dc3f de60 4fb2 d643 c43f  K..[.'.?.`O..C.?
+000008d0: 6411 5090 a8b0 ea3f 1223 de65 7101 f03f  d.P....?.#.eq..?
+000008e0: cf22 c77e 7801 f03f 0000 0000 0000 f03f  .".~x..?.......?
+000008f0: d324 a566 6666 1640 413c 309a a88f ef3f  .$.fff.@A<0....?
+00000900: c4b0 03e5 1901 f03f e672 18ff 7a46 c53f  .......?.r..zF.?
+00000910: 7240 7707 b0ae ea3f 47da d1d5 2201 f03f  r@w....?G..."..?
+00000920: 4544 d93d 8cfc ef3f c88b 7ad3 9700 f03f  ED.=...?..z....?
+00000930: c88b 7ad3 9700 f03f cca0 c310 ba01 f03f  ..z....?.......?
+00000940: d578 e926 3108 f03f 1bab d828 2257 633f  .x.&1..?...("Wc?
+00000950: 6e52 9990 781c dc3f b7c9 d84c 9c43 c43f  nR..x..?...L.C.?
+00000960: 7240 7707 b0ae ea3f c4b0 03e5 1901 f03f  r@w....?.......?
+00000970: 47da d1d5 2201 f03f 0000 0000 0000 f03f  G..."..?.......?
+00000980: 9b24 a566 6666 1640 830a 5f06 bc8e ef3f  .$.fff.@.._....?
+00000990: 1635 a021 8800 f03f b3e6 ee76 e653 c53f  .5.!...?...v.S.?
+000009a0: a782 db91 22ab ea3f afe0 9f6f 9200 f03f  ...."..?...o...?
+000009b0: a4af 1827 4bfc ef3f aa3c 9c43 8b01 f03f  ...'K..?.<.C...?
+000009c0: aa3c 9c43 8b01 f03f 92d6 7f88 7202 f03f  .<.C...?....r..?
+000009d0: d578 e926 3108 f03f 14c0 7cfe 2b69 6b3f  .x.&1..?..|.+ik?
+000009e0: 2e93 5ee9 2412 dc3f 6eee 84ad d043 c43f  ..^.$..?n....C.?
+000009f0: a782 db91 22ab ea3f 1635 a021 8800 f03f  ...."..?.5.!...?
+00000a00: afe0 9f6f 9200 f03f 0000 0000 0000 f03f  ...o...?.......?
+00000a10: 6c24 a566 6666 1640 6ac8 db20 e78d ef3f  l$.fff.@j.. ...?
+00000a20: b0f8 f476 0e00 f03f 5fbc d21c 2e5f c53f  ...v...?_...._.?
+00000a30: 1ca3 9ad4 27a8 ea3f 56aa 9cf3 1800 f03f  ....'..?V......?
+00000a40: eab4 46be 42fc ef3f 3721 3846 4d02 f03f  ..F.B..?7!8FM..?
+00000a50: 3721 3846 4d02 f03f fdad a24a 6a03 f03f  7!8FM..?...Jj..?
+00000a60: d578 e926 3108 f03f 91e5 035c 0820 733f  .x.&1..?...\. s?
+00000a70: 8d50 553f 1409 dc3f c39b df08 3944 c43f  .PU?...?....9D.?
+00000a80: 1ca3 9ad4 27a8 ea3f b0f8 f476 0e00 f03f  ....'..?...v...?
+00000a90: 56aa 9cf3 1800 f03f 0000 0000 0000 f03f  V......?.......?
+00000aa0: 4624 a566 6666 1640 5542 4b8a 278d ef3f  F$.fff.@UBK.'..?
+00000ab0: db4b 4aae abff ef3f 633a 85eb 2164 c53f  .KJ....?c:..!d.?
+00000ac0: e0b3 e75c d9a6 ea3f 67a2 18f8 beff ef3f  ...\...?g......?
+00000ad0: 2372 11fd 69fc ef3f 374d 18b4 ef02 f03f  #r..i..?7M.....?
+00000ae0: 374d 18b4 ef02 f03f 317c 35bd 1804 f03f  7M.....?1|5....?
+00000af0: d578 e926 3108 f03f cab9 f75e f0f0 763f  .x.&1..?...^..v?
+00000b00: a2b6 09c7 f500 dc3f f0d3 5832 7944 c43f  .......?..X2yD.?
+00000b10: e0b3 e75c d9a6 ea3f db4b 4aae abff ef3f  ...\...?.KJ....?
+00000b20: 67a2 18f8 beff ef3f 0000 0000 0000 f03f  g......?.......?
+00000b30: 2624 a566 6666 1640 db61 4520 7b8c ef3f  &$.fff.@.aE {..?
+00000b40: 20c5 9a35 7cff ef3f a963 17af e665 c53f   ..5|..?.c...e.?
+00000b50: d380 8f44 62a6 ea3f 79d8 760d 8dff ef3f  ...Db..?y.v....?
+00000b60: 090f c122 a6fc ef3f 2533 585b 7b03 f03f  ..."...?%3X[{..?
+00000b70: 2533 585b 7b03 f03f 2a82 671e 9d04 f03f  %3X[{..?*.g....?
+00000b80: d578 e926 3108 f03f 87b1 87dd 43d6 793f  .x.&1..?....C.y?
+00000b90: d13f 9da8 9ef9 db3f 3509 7570 a544 c43f  .?.....?5.up.D.?
+00000ba0: d380 8f44 62a6 ea3f 20c5 9a35 7cff ef3f  ...Db..? ..5|..?
+00000bb0: 79d8 760d 8dff ef3f 0000 0000 0000 f03f  y.v....?.......?
+00000bc0: 0824 a566 6666 1640 7972 32f7 df8b ef3f  .$.fff.@yr2....?
+00000bd0: fdd3 a90f 6eff ef3f 77da 5376 1166 c53f  ....n..?w.Sv.f.?
+00000be0: ff43 b754 57a6 ea3f 1051 af5a 7cff ef3f  .C.TW..?.Q.Z|..?
+00000bf0: f477 39bd e9fc ef3f 9ed5 a694 f503 f03f  .w9....?.......?
+00000c00: 9ed5 a694 f503 f03f 0f15 e2f8 0605 f03f  .......?.......?
+00000c10: d578 e926 3108 f03f 07ca c458 0b27 7c3f  .x.&1..?...X.'|?
+00000c20: 3416 389f f4f2 db3f a0eb 3a18 c744 c43f  4.8....?..:..D.?
+00000c30: ff43 b754 57a6 ea3f fdd3 a90f 6eff ef3f  .C.TW..?....n..?
+00000c40: 1051 af5a 7cff ef3f 0000 0000 0000 f03f  .Q.Z|..?.......?
+00000c50: f023 a566 6666 1640 8e74 c754 548b ef3f  .#.fff.@.t.TT..?
+00000c60: 9e22 7355 70ff ef3f 1868 b715 7565 c53f  ."sUp..?.h..ue.?
+00000c70: a23d ddc6 80a6 ea3f e6fd 3743 7cff ef3f  .=.....?..7C|..?
+00000c80: dbb6 3d0d 2efd ef3f b5b7 bfcb 6104 f03f  ..=....?....a..?
+00000c90: b5b7 bfcb 6104 f03f edd3 3507 5f05 f03f  ....a..?..5._..?
+00000ca0: d578 e926 3108 f03f 5207 f760 2814 7e3f  .x.&1..?R..`(.~?
+00000cb0: 48f6 e65a e6ec db3f 2193 8ed0 e244 c43f  H..Z...?!....D.?
+00000cc0: a23d ddc6 80a6 ea3f 9e22 7355 70ff ef3f  .=.....?."sUp..?
+00000cd0: e6fd 3743 7cff ef3f 0000 0000 0000 f03f  ..7C|..?.......?
+00000ce0: db23 a566 6666 1640 0536 11ab d68a ef3f  .#.fff.@.6.....?
+00000cf0: 8626 0f70 7aff ef3f 15b1 ee92 7c64 c53f  .&.pz..?....|d.?
+00000d00: 4243 2853 c2a6 ea3f 3d0a e04a 84ff ef3f  BC(S...?=..J...?
+00000d10: 6b41 3acf 6ffd ef3f e5e8 3455 c204 f03f  kA:.o..?..4U...?
+00000d20: e5e8 3455 c204 f03f e44b 4f58 aa05 f03f  ..4U...?.KOX...?
+00000d30: d578 e926 3108 f03f 0a0a 3589 eeb9 7f3f  .x.&1..?..5....?
+00000d40: cfa6 4834 67e7 db3f 3b8c 12d0 fa44 c43f  ..H4g..?;....D.?
+00000d50: 4243 2853 c2a6 ea3f 8626 0f70 7aff ef3f  BC(S...?.&.pz..?
+00000d60: 3d0a e04a 84ff ef3f 0000 0000 0000 f03f  =..J...?.......?
+00000d70: c823 a566 6666 1640 b89b ff93 658a ef3f  .#.fff.@....e..?
+00000d80: 9379 8be6 87ff ef3f 1e9f a099 5f63 c53f  .y.....?...._c.?
+00000d90: 50a9 214b 0da7 ea3f 3472 39fd 8fff ef3f  P.!K...?4r9....?
+00000da0: d753 5083 adfd ef3f 4e17 47df 1805 f03f  .SP....?N.G....?
+00000db0: 4e17 47df 1805 f03f 14af 9001 ec05 f03f  N.G....?.......?
+00000dc0: d578 e926 3108 f03f 9f76 e52e d194 803f  .x.&1..?.v.....?
+00000dd0: 42bd 96c3 6ce2 db3f 90b5 c625 1045 c43f  B...l..?...%.E.?
+00000de0: 50a9 214b 0da7 ea3f 9379 8be6 87ff ef3f  P.!K...?.y.....?
+00000df0: 3472 39fd 8fff ef3f 0000 0000 0000 f03f  4r9....?.......?
+00000e00: b523 a566 6666 1640 670a 64cd ff89 ef3f  .#.fff.@g.d....?
+00000e10: e33b 6b50 96ff ef3f 9dc3 881b 3c62 c53f  .;kP...?....<b.?
+00000e20: 94af 62cf 59a7 ea3f 2a0b a9ec 9cff ef3f  ..b.Y..?*......?
+00000e30: a68b dc93 e6fd ef3f d798 0ab1 6605 f03f  .......?....f..?
+00000e40: d798 0ab1 6605 f03f 8d0f 9bfc 2506 f03f  ....f..?....%..?
+00000e50: d578 e926 3108 f03f 92c3 5bb2 2937 813f  .x.&1..?..[.)7.?
+00000e60: 2fc3 a08d eddd db3f b8aa 6369 2345 c43f  /......?..ci#E.?
+00000e70: 94af 62cf 59a7 ea3f e33b 6b50 96ff ef3f  ..b.Y..?.;kP...?
+00000e80: 2a0b a9ec 9cff ef3f 0000 0000 0000 f03f  *......?.......?
+00000e90: a523 a566 6666 1640 f438 5735 a489 ef3f  .#.fff.@.8W5...?
+00000ea0: a788 0564 a4ff ef3f 0cfe c40d 2261 c53f  ...d...?...."a.?
+00000eb0: 053e cbb2 a3a7 ea3f b514 c1c6 a9ff ef3f  .>.....?.......?
+00000ec0: 48b8 ade8 1afe ef3f aff6 70cf ac05 f03f  H......?..p....?
+00000ed0: aff6 70cf ac05 f03f 6b90 f69c 5906 f03f  ..p....?k...Y..?
+00000ee0: d578 e926 3108 f03f c7c3 5f7f b7c7 813f  .x.&1..?.._....?
+00000ef0: 8c05 305c e0d9 db3f 41d9 9600 3545 c43f  ..0\...?A...5E.?
+00000f00: 053e cbb2 a3a7 ea3f a788 0564 a4ff ef3f  .>.....?...d...?
+00000f10: b514 c1c6 a9ff ef3f 0000 0000 0000 f03f  .......?.......?
+00000f20: 9723 a566 6666 1640 0beb fbc6 5189 ef3f  .#.fff.@....Q..?
+00000f30: f20c c67d b1ff ef3f 13b4 f143 1960 c53f  ...}...?...C.`.?
+00000f40: 44fb 16ed e8a7 ea3f 62aa 5fde b5ff ef3f  D......?b._....?
+00000f50: 86c2 03ac 4afe ef3f f995 4513 ec05 f03f  ....J..?..E....?
+00000f60: f995 4513 ec05 f03f 5a0e afd2 8706 f03f  ..E....?Z......?
+00000f70: d578 e926 3108 f03f b531 28b7 1a49 823f  .x.&1..?.1(..I.?
+00000f80: 908e 2b02 3cd6 db3f 4ce4 5c33 4545 c43f  ..+.<..?L.\3EE.?
+00000f90: 44fb 16ed e8a7 ea3f f20c c67d b1ff ef3f  D......?...}...?
+00000fa0: 62aa 5fde b5ff ef3f 0000 0000 0000 f03f  b._....?.......?
+00000fb0: 8b23 a566 6666 1640 2228 9597 0789 ef3f  .#.fff.@"(.....?
+00000fc0: c30a 045a bdff ef3f 4799 93da 245f c53f  ...Z...?G...$_.?
+00000fd0: 5e60 63b3 28a8 ea3f 8bb5 d8e6 c0ff ef3f  ^`c.(..?.......?
+00000fe0: f12a 5d28 76fe ef3f 9786 2436 2506 f03f  .*](v..?..$6%..?
+00000ff0: 9786 2436 2506 f03f 5aca 7551 b106 f03f  ..$6%..?Z.uQ...?
+00001000: d578 e926 3108 f03f 14df 377d 4abd 823f  .x.&1..?..7}J..?
+00001010: d1c7 5960 f7d2 db3f 72ab ff34 5445 c43f  ..Y`...?r..4TE.?
+00001020: 5e60 63b3 28a8 ea3f c30a 045a bdff ef3f  ^`c.(..?...Z...?
+00001030: 8bb5 d8e6 c0ff ef3f 0000 0000 0000 f03f  .......?.......?
+00001040: 8023 a566 6666 1640 727a e7d3 c488 ef3f  .#.fff.@rz.....?
+00001050: 5113 0dea c7ff ef3f 4400 0152 455e c53f  Q......?D..RE^.?
+00001060: 13cb d1e9 62a8 ea3f 40c5 86c9 caff ef3f  ....b..?@......?
+00001070: 2a3a b5b4 9dfe ef3f 9126 28da 5806 f03f  *:.....?.&(.X..?
+00001080: 9126 28da 5806 f03f 969d 80a7 d606 f03f  .&(.X..?.......?
+00001090: d578 e926 3108 f03f d1dd ee01 d525 833f  .x.&1..?.....%.?
+000010a0: 9308 118a 09d0 db3f f793 062a 6245 c43f  .......?...*bE.?
+000010b0: 13cb d1e9 62a8 ea3f 5113 0dea c7ff ef3f  ....b..?Q......?
+000010c0: 40c5 86c9 caff ef3f 0000 0000 0000 f03f  @......?.......?
+000010d0: 7523 a566 6666 1640 0b9f ddbd 8888 ef3f  u#.fff.@.......?
+000010e0: 2ed8 7f39 d1ff ef3f f21f ffde 795d c53f  ...9...?....y].?
+000010f0: e604 d0ca 97a8 ea3f eaa1 448b d3ff ef3f  .......?..D....?
+00001100: b4cd a2a9 c1fe ef3f d865 958e 8706 f03f  .......?.e.....?
+00001110: d865 958e 8706 f03f 65f5 ac4a f806 f03f  .e.....?e..J...?
+00001120: d578 e926 3108 f03f 62c2 e54a 0484 833f  .x.&1..?b..J...?
+00001130: 97e7 baf0 69cd db3f 5f87 682d 6f45 c43f  ....i..?_.h-oE.?
+00001140: e604 d0ca 97a8 ea3f 2ed8 7f39 d1ff ef3f  .......?...9...?
+00001150: eaa1 448b d3ff ef3f 0000 0000 0000 f03f  ..D....?.......?
+00001160: 6e23 a566 6666 1640 a4d6 69aa 5288 ef3f  n#.fff.@..i.R..?
+00001170: 89bf 3160 d9ff ef3f 56e8 c61d c15c c53f  ..1`...?V....\.?
+00001180: 0a65 09b8 c7a8 ea3f 5477 413e dbff ef3f  .e.....?TwA>...?
+00001190: 01e9 fe5b e2fe ef3f 3868 ebd2 b106 f03f  ...[...?8h.....?
+000011a0: 3868 ebd2 b106 f03f 47c5 db9f 1607 f03f  8h.....?G......?
+000011b0: d578 e926 3108 f03f 5c91 f9cd f2d8 833f  .x.&1..?\......?
+000011c0: a650 8688 10cb db3f e945 c153 7b45 c43f  .P.....?.E.S{E.?
+000011d0: 0a65 09b8 c7a8 ea3f 89bf 3160 d9ff ef3f  .e.....?..1`...?
+000011e0: 5477 413e dbff ef3f 0000 0000 0000 f03f  TwA>...?.......?
+000011f0: 6723 a566 6666 1640 b7b8 9dff 2188 ef3f  g#.fff.@....!..?
+00001200: fe8b 2a7a e0ff ef3f 2334 6178 195c c53f  ..*z...?#4ax.\.?
+00001210: 79bb 951f f3a8 ea3f f2bb d9f9 e1ff ef3f  y......?.......?
+00001220: 0d4b 791a 00ff ef3f f618 0919 d806 f03f  .Ky....?.......?
+00001230: f618 0919 d806 f03f 94c8 38ff 3107 f03f  .......?..8.1..?
+00001240: d578 e926 3108 f03f 81a4 036c 9725 843f  .x.&1..?...l.%.?
+00001250: b4e0 a4e1 f5c8 db3f 9368 1bae 8645 c43f  .......?.h...E.?
+00001260: 79bb 951f f3a8 ea3f fe8b 2a7a e0ff ef3f  y......?..*z...?
+00001270: f2bb d9f9 e1ff ef3f 0000 0000 0000 f03f  .......?.......?
+00001280: 5f23 a566 6666 1640 ad09 f332 f687 ef3f  _#.fff.@...2...?
+00001290: fa3f b4a3 e6ff ef3f 5200 2159 815b c53f  .?.....?R.!Y.[.?
+000012a0: 60ac d26e 1aa9 ea3f 558c 80d6 e7ff ef3f  `..n...?U......?
+000012b0: a2f4 d72c 1bff ef3f b274 d2c6 fa06 f03f  ...,...?.t.....?
+000012c0: b274 d2c6 fa06 f03f 8e92 c1b6 4a07 f03f  .t.....?....J..?
+000012d0: d578 e926 3108 f03f e555 a084 cc6a 843f  .x.&1..?.U...j.?
+000012e0: c54b f835 13c7 db3f 483c c14b 9145 c43f  .K.5...?H<.K.E.?
+000012f0: 60ac d26e 1aa9 ea3f fa3f b4a3 e6ff ef3f  `..n...?.?.....?
+00001300: 558c 80d6 e7ff ef3f 0000 0000 0000 f03f  U......?.......?
+00001310: 5823 a566 6666 1640 07a4 c0c7 ce87 ef3f  X#.fff.@.......?
+00001320: ae2c 8ff7 ebff ef3f b8fe b841 f75a c53f  .,.....?...A.Z.?
+00001330: c7ba 6f0c 3ea9 ea3f 4ac4 cfeb ecff ef3f  ..o.>..?J......?
+00001340: 537b 07d4 33ff ef3f 3e93 8937 1a07 f03f  S{..3..?>..7...?
+00001350: 3e93 8937 1a07 f03f 8b86 e30b 6107 f03f  >..7...?....a..?
+00001360: d578 e926 3108 f03f 9c30 4c7d 54a9 843f  .x.&1..?.0L}T..?
+00001370: 9283 e06c 62c5 db3f 9f56 443b 9b45 c43f  ...lb..?.VD;.E.?
+00001380: c7ba 6f0c 3ea9 ea3f ae2c 8ff7 ebff ef3f  ..o.>..?.,.....?
+00001390: 4ac4 cfeb ecff ef3f 0000 0000 0000 f03f  J......?.......?
+000013a0: 5323 a566 6666 1640 7004 d74d ab87 ef3f  S#.fff.@p..M...?
+000013b0: 674d 4a8e f0ff ef3f 49ee 8ed3 795a c53f  gMJ....?I...yZ.?
+000013c0: 9bc4 5756 5ea9 ea3f f61b c14f f1ff ef3f  ..WV^..?...O...?
+000013d0: bc61 894a 4aff ef3f 223e f6bc 3607 f03f  .a.JJ..?">..6..?
+000013e0: 223e f6bc 3607 f03f 054c 9e3c 7507 f03f  ">..6..?.L.<u..?
+000013f0: d578 e926 3108 f03f c0ef a8ee dce1 843f  .x.&1..?.......?
+00001400: e6ea 4917 dec3 db3f 599f ec8a a445 c43f  ..I....?Y....E.?
+00001410: 9bc4 5756 5ea9 ea3f 674d 4a8e f0ff ef3f  ..WV^..?gMJ....?
+00001420: f61b c14f f1ff ef3f 0000 0000 0000 f03f  ...O...?.......?
+00001430: 4c23 a566 6666 1640 f87b 4060 8b87 ef3f  L#.fff.@.{@`...?
+00001440: d39d f77d f4ff ef3f bc5a 6dd3 075a c53f  ...}...?.Zm..Z.?
+00001450: ba06 cea0 7ba9 ea3f a449 4816 f5ff ef3f  ....{..?.IH....?
+00001460: 3ee6 02c5 5eff ef3f 26d4 68a0 5007 f03f  >...^..?&.h.P..?
+00001470: 26d4 68a0 5007 f03f 226a 6480 8707 f03f  &.h.P..?"jd....?
+00001480: d578 e926 3108 f03f f238 6419 0115 853f  .x.&1..?.8d....?
+00001490: 76fd 1566 81c2 db3f 63eb e848 ad45 c43f  v..f...?c..H.E.?
+000014a0: ba06 cea0 7ba9 ea3f d39d f77d f4ff ef3f  ....{..?...}...?
+000014b0: a449 4816 f5ff ef3f 0000 0000 0000 f03f  .IH....?.......?
+000014c0: 4823 a566 6666 1640 9c72 21a4 6e87 ef3f  H#.fff.@.r!.n..?
+000014d0: 87ca 30da f7ff ef3f e97b 0a29 a059 c53f  ..0....?.{.).Y.?
+000014e0: 1773 9f36 96a9 ea3f f004 4251 f8ff ef3f  .s.6...?..BQ...?
+000014f0: fe4d d972 71ff ef3f f4b7 a123 6807 f03f  .M.rq..?...#h..?
+00001500: f4b7 a123 6807 f03f 5953 d008 9807 f03f  ...#h..?YS.....?
+00001510: d578 e926 3108 f03f 4bee 24e1 4b43 853f  .x.&1..?K.$.KC.?
+00001520: e4c6 d31c 48c1 db3f c5ac 4083 b545 c43f  ....H..?..@..E.?
+00001530: 1773 9f36 96a9 ea3f 87ca 30da f7ff ef3f  .s.6...?..0....?
+00001540: f004 4251 f8ff ef3f 0000 0000 0000 f03f  ..BQ...?.......?
+00001550: 4423 a566 6666 1640 6781 b5c7 5487 ef3f  D#.fff.@g...T..?
+00001560: ac02 52b4 faff ef3f f3f6 bcdb 4159 c53f  ..R....?....AY.?
+00001570: 8044 0e5a aea9 ea3f 671b 9d10 fbff ef3f  .D.Z...?g......?
+00001580: 7993 ca7e 82ff ef3f 0df8 a181 7d07 f03f  y..~...?....}..?
+00001590: 0df8 a181 7d07 f03f 08b5 3f02 a707 f03f  ....}..?..?....?
+000015a0: d578 e926 3108 f03f 8719 6a7f 396d 853f  .x.&1..?..j.9m.?
+000015b0: cb11 8a82 2ec0 db3f 4ea0 9e47 bd45 c43f  .......?N..G.E.?
+000015c0: 8044 0e5a aea9 ea3f ac02 52b4 faff ef3f  .D.Z...?..R....?
+000015d0: 671b 9d10 fbff ef3f 0000 0000 0000 f03f  g......?.......?
+000015e0: 4023 a566 6666 1640 657e 6681 3d87 ef3f  @#.fff.@e~f.=..?
+000015f0: 3881 a11b fdff ef3f a080 4b10 ec58 c53f  8......?..K..X.?
+00001600: 93d6 7045 c4a9 ea3f 658d 7362 fdff ef3f  ..pE...?e.sb...?
+00001610: 27f3 760f 92ff ef3f afba 66ef 9007 f03f  '.v....?..f....?
+00001620: afba 66ef 9007 f03f 3983 5f94 b407 f03f  ..f....?9._....?
+00001630: d578 e926 3108 f03f 70d8 ab0b 3993 853f  .x.&1..?p...9..?
+00001640: e25a 0452 31bf db3f 04f4 2aa3 c445 c43f  .Z.R1..?..*..E.?
+00001650: 93d6 7045 c4a9 ea3f 3881 a11b fdff ef3f  ..pE...?8......?
+00001660: 658d 7362 fdff ef3f 0000 0000 0000 f03f  e.sb...?.......?
+00001670: 3c23 a566 6666 1640 93df fa8e 2887 ef3f  <#.fff.@....(..?
+00001680: 0b27 bf1d ffff ef3f dd34 da02 9e58 c53f  .'.....?.4...X.?
+00001690: 2dd4 d22c d8a9 ea3f d167 6e53 ffff ef3f  -..,...?.gnS...?
+000016a0: fd3e e047 a0ff ef3f e50c 939c a207 f03f  .>.G...?.......?
+000016b0: e50c 939c a207 f03f dcd8 a7e2 c007 f03f  .......?.......?
+000016c0: d578 e926 3108 f03f c59c 35d6 adb5 853f  .x.&1..?..5....?
+000016d0: eee0 b5aa 4dbe db3f 87b1 3aa2 cb45 c43f  ....M..?..:..E.?
+000016e0: 2dd4 d22c d8a9 ea3f 0b27 bf1d ffff ef3f  -..,...?.'.....?
+000016f0: d167 6e53 ffff ef3f 0000 0000 0000 f03f  .gnS...?.......?
+00001700: 3b23 a566 6666 1640 281d d9b4 1587 ef3f  ;#.fff.@(......?
+00001710: 5174 9663 0000 f03f 09dc 87ff 5658 c53f  Qt.c...?....VX.?
+00001720: 94a8 ec3f eaa9 ea3f dd57 a277 0000 f03f  ...?...?.W.w...?
+00001730: 3fdf ce47 adff ef3f 102c 07b4 b207 f03f  ?..G...?.,.....?
+00001740: 102c 07b4 b207 f03f 655f d30c cc07 f03f  .,.....?e_.....?
+00001750: d578 e926 3108 f03f 6874 7bb6 f0d4 853f  .x.&1..?ht{....?
+00001760: fdef e902 81bd db3f 03a0 f64f d245 c43f  .......?...O.E.?
+00001770: 94a8 ec3f eaa9 ea3f 5174 9663 0000 f03f  ...?...?Qt.c...?
+00001780: dd57 a277 0000 f03f 0000 0000 0000 f03f  .W.w...?.......?
+00001790: 3723 a566 6666 1640 eaf7 5dbd 0487 ef3f  7#.fff.@..]....?
+000017a0: ac5b c011 0100 f03f ed89 b55f 1658 c53f  .[.....?..._.X.?
+000017b0: dd67 e0aa faa9 ea3f c0ca 7220 0100 f03f  .g.....?..r ...?
+000017c0: 2b21 172c b9ff ef3f 7c1c 635c c107 f03f  +!.,...?|.c\...?
+000017d0: 7c1c 635c c107 f03f 5208 542f d607 f03f  |.c\...?R.T/...?
+000017e0: d578 e926 3108 f03f e25a ee51 51f1 853f  .x.&1..?.Z.QQ..?
+000017f0: 57ea 991b c9bc db3f c686 45b6 d845 c43f  W......?..E..E.?
+00001800: dd67 e0aa faa9 ea3f ac5b c011 0100 f03f  .g.....?.[.....?
+00001810: c0ca 7220 0100 f03f 0000 0000 0000 f03f  ..r ...?.......?
+00001820: 3423 a566 6666 1640 86be 4378 f586 ef3f  4#.fff.@..Cx...?
+00001830: 718d bd9e 0100 f03f 50b8 da88 db57 c53f  q......?P....W.?
+00001840: ebe6 8d96 09aa ea3f 2359 44a9 0100 f03f  .......?#YD....?
+00001850: 4489 d20e c4ff ef3f 0d7b 77b8 ce07 f03f  D......?.{w....?
+00001860: 0d7b 77b8 ce07 f03f 4d0d b963 df07 f03f  .{w....?M..c...?
+00001870: d578 e926 3108 f03f 152e 9639 170b 863f  .x.&1..?...9...?
+00001880: 00ed f7f5 23bc db3f b4d4 d1dd de45 c43f  ....#..?.....E.?
+00001890: ebe6 8d96 09aa ea3f 718d bd9e 0100 f03f  .......?q......?
+000018a0: 2359 44a9 0100 f03f 0000 0000 0000 f03f  #YD....?.......?
+000018b0: 3123 a566 6666 1640 acdd 18ba e786 ef3f  1#.fff.@.......?
+000018c0: 458f c70f 0200 f03f cd8c fee4 a557 c53f  E......?.....W.?
+000018d0: c982 8f2a 17aa ea3f 1558 1817 0200 f03f  ...*...?.X.....?
+000018e0: 73c2 9307 ceff ef3f ccb0 a8e7 da07 f03f  s......?.......?
+000018f0: ccb0 a8e7 da07 f03f 39d8 05c1 e707 f03f  .......?9......?
+00001900: d578 e926 3108 f03f 3639 68dd 8222 863f  .x.&1..?69h..".?
+00001910: 7a85 9dca 8fbb db3f cc0a cecd e445 c43f  z......?.....E.?
+00001920: c982 8f2a 17aa ea3f 458f c70f 0200 f03f  ...*...?E......?
+00001930: 1558 1817 0200 f03f 0000 0000 0000 f03f  .X.....?.......?
+00001940: 3023 a566 6666 1640 8432 c45b db86 ef3f  0#.fff.@.2.[...?
+00001950: a6de 2c6a 0200 f03f 13bd 27dc 7457 c53f  ..,j...?..'.tW.?
+00001960: 09b1 f58e 23aa ea3f f732 0f6f 0200 f03f  ....#..?.2.o...?
+00001970: 5c98 7a2b d7ff ef3f c226 4106 e607 f03f  \.z+...?.&A....?
+00001980: c226 4106 e607 f03f 824a 0b5c ef07 f03f  .&A....?.J.\...?
+00001990: d578 e926 3108 f03f e60d 4286 ce37 863f  .x.&1..?..B..7.?
+000019a0: 3b74 3d02 0bbb db3f db98 d08b ea45 c43f  ;t=....?.....E.?
+000019b0: 09b1 f58e 23aa ea3f a6de 2c6a 0200 f03f  ....#..?..,j...?
+000019c0: f732 0f6f 0200 f03f 0000 0000 0000 f03f  .2.o...?.......?
+000019d0: 2e23 a566 6666 1640 8fbe 153a d086 ef3f  .#.fff.@...:...?
+000019e0: c624 28b3 0200 f03f e217 e8d8 4757 c53f  .$(....?....GW.?
+000019f0: ef86 19eb 2eaa ea3f a7d3 3db6 0200 f03f  .......?..=....?
+00001a00: 460b 2c8d dfff ef3f 7dd5 af2d f007 f03f  F.,....?}..-...?
+00001a10: 7dd5 af2d f007 f03f fafa bd47 f607 f03f  }..-...?...G...?
+00001a20: d578 e926 3108 f03f f292 6347 2f4b 863f  .x.&1..?..cG/K.?
+00001a30: 32e2 982f 94ba db3f c166 3e1c f045 c43f  2../...?.f>..E.?
+00001a40: ef86 19eb 2eaa ea3f c624 28b3 0200 f03f  .......?.$(....?
+00001a50: a7d3 3db6 0200 f03f 0000 0000 0000 f03f  ..=....?.......?
+00001a60: 2923 a566 6666 1640 477f 6235 c686 ef3f  )#.fff.@G.b5...?
+00001a70: d2a2 94ef 0200 f03f e27d 6650 1e57 c53f  .......?.}fP.W.?
+00001a80: a5a0 8363 39aa ea3f 9a83 60f1 0200 f03f  ...c9..?..`....?
+00001a90: d020 dd3c e7ff ef3f c13f bb74 f907 f03f  . .<...?.?.t...?
+00001aa0: c13f bb74 f907 f03f 0c69 6f95 fc07 f03f  .?.t...?.io....?
+00001ab0: d578 e926 3108 f03f 3ff7 979e d55c 863f  .x.&1..??....\.?
+00001ac0: b9e4 680a 2aba db3f b37a e282 f545 c43f  ..h.*..?.z...E.?
+00001ad0: a5a0 8363 39aa ea3f d2a2 94ef 0200 f03f  ...c9..?.......?
+00001ae0: 9a83 60f1 0200 f03f 0000 0000 0000 f03f  ..`....?.......?
+00001af0: 2a23 a566 6666 1640 f24b 2a31 bd86 ef3f  *#.fff.@.K*1...?
+00001b00: 4668 0f24 0300 f03f 3801 12be f756 c53f  Fh.$...?8....V.?
+00001b10: 26a1 0c1b 43aa ea3f 6dd2 fa24 0300 f03f  &...C..?m..$...?
+00001b20: 8a42 7f48 eeff ef3f c114 b3ef 0108 f03f  .B.H...?.......?
+00001b30: c114 b3ef 0108 f03f 28c9 ea54 0208 f03f  .......?(..T...?
+00001b40: d578 e926 3108 f03f ef71 d8c4 ed6c 863f  .x.&1..?.q...l.?
+00001b50: b9ba 0a6b cbb9 db3f 169e eec2 fa45 c43f  ...k...?.....E.?
+00001b60: 26a1 0c1b 43aa ea3f 4668 0f24 0300 f03f  &...C..?Fh.$...?
+00001b70: 6dd2 fa24 0300 f03f 0000 0000 0000 f03f  m..$...?.......?
+00001b80: 2823 a566 6666 1640 93b8 c613 b586 ef3f  (#.fff.@.......?
+00001b90: 8018 bb54 0300 f03f 152e c0a8 d356 c53f  ...T...?.....V.?
+00001ba0: 5d56 8331 4caa ea3f 984a 1a55 0300 f03f  ]V.1L..?.J.U...?
+00001bb0: 638a dabb f4ff ef3f eef9 99b0 0908 f03f  c......?.......?
+00001bc0: eef9 99b0 0908 f03f 2684 9994 0708 f03f  .......?&......?
+00001bd0: d578 e926 3108 f03f 87c9 7d14 a07b 863f  .x.&1..?..}..{.?
+00001be0: 39bf c846 77b9 db3f 1605 6ddf ff45 c43f  9..Fw..?..m..E.?
+00001bf0: 5d56 8331 4caa ea3f 8018 bb54 0300 f03f  ]V.1L..?...T...?
+00001c00: 984a 1a55 0300 f03f 0000 0000 0000 f03f  .J.U...?.......?
+00001c10: 2623 a566 6666 1640 b816 22c6 ad86 ef3f  &#.fff.@.."....?
+00001c20: 3b22 fd83 0300 f03f 6976 66d5 b156 c53f  ;".....?ivf..V.?
+00001c30: 033e 94b6 54aa ea3f 47c7 1284 0300 f03f  .>..T..?G......?
+00001c40: 55b2 bda0 faff ef3f 08eb 48c7 1008 f03f  U......?..H....?
+00001c50: 08eb 48c7 1008 f03f 7205 9561 0c08 f03f  ..H....?r..a...?
+00001c60: d578 e926 3108 f03f 532a 1b3b 1189 863f  .x.&1..?S*.;...?
+00001c70: 4679 55ac 2cb9 db3f 6f29 f0dc 0446 c43f  FyU.,..?o)...F.?
+00001c80: 033e 94b6 54aa ea3f 3b22 fd83 0300 f03f  .>..T..?;".....?
+00001c90: 47c7 1284 0300 f03f 0000 0000 0000 f03f  G......?.......?
+00001ca0: 6666 6666 6666 1640 2188 a40b 6c86 ef3f  ffffff.@!...l..?
+00001cb0: 4ca2 4100 0000 f03f 5455 5555 5555 c53f  L.A....?TUUUUU.?
+00001cc0: abaa aaaa aaaa ea3f 0000 0000 0000 f03f  .......?.......?
+00001cd0: 0000 0000 0000 f03f 2587 e926 3108 f03f  .......?%..&1..?
+00001ce0: 9886 e926 3108 f03f b187 e926 3108 f03f  ...&1..?...&1..?
+00001cf0: d578 e926 3108 f03f e37c b3ae 06f0 863f  .x.&1..?.|.....?
+00001d00: f2d0 5dbe b6b8 db3f 8afd a762 6746 c43f  ..]....?...bgF.?
+00001d10: abaa aaaa aaaa ea3f 0000 0000 0000 f03f  .......?.......?
+00001d20: 0000 0000 0000 f03f 0000 0000 0000 f03f  .......?.......?
```

### Comparing `econpizza-0.6.0/econpizza/testing/test_rest.py` & `econpizza-0.6.1/econpizza/testing/test_rest.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/tools.py` & `econpizza-0.6.1/econpizza/tools.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/utilities/dists.py` & `econpizza-0.6.1/econpizza/utilities/dists.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/utilities/grids.py` & `econpizza-0.6.1/econpizza/utilities/grids.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/utilities/interp.py` & `econpizza-0.6.1/econpizza/utilities/interp.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/utilities/jacobian.py` & `econpizza-0.6.1/econpizza/utilities/jacobian.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza/utilities/newton.py` & `econpizza-0.6.1/econpizza/utilities/newton.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/econpizza.egg-info/PKG-INFO` & `econpizza-0.6.1/econpizza.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econpizza
-Version: 0.6.0
+Version: 0.6.1
 Summary: Solve nonlinear perfect foresight models with heterogeneous agents
 Home-page: https://github.com/gboehl/econpizza
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `econpizza-0.6.0/econpizza.egg-info/SOURCES.txt` & `econpizza-0.6.1/econpizza.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `econpizza-0.6.0/setup.py` & `econpizza-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,12 +32,12 @@
     package_data={"econpizza": ["examples/*"]},
     extras_require={
         'linear': ['grgrlib>=0.1.22'],
     },
     install_requires=[
         "jax>=0.4.13",
         "jaxlib>=0.4.13",
-        "grgrjax>=0.4.3",
+        "grgrjax>=0.4.4",
         "pyyaml",
         "scipy",
     ],
 )
```

