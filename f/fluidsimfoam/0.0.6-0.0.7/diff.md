# Comparing `tmp/fluidsimfoam-0.0.6.tar.gz` & `tmp/fluidsimfoam-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluidsimfoam-0.0.6.tar", max compression
+gzip compressed data, was "fluidsimfoam-0.0.7.tar", max compression
```

## Comparing `fluidsimfoam-0.0.6.tar` & `fluidsimfoam-0.0.7.tar`

### file list

```diff
@@ -1,76 +1,81 @@
--rw-r--r--   0        0        0     1521 2023-03-02 21:01:46.291446 fluidsimfoam-0.0.6/LICENSE
--rw-r--r--   0        0        0     7375 2023-06-04 19:44:44.715013 fluidsimfoam-0.0.6/README.md
--rw-r--r--   0        0        0     2342 2023-06-09 19:17:24.747107 fluidsimfoam-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2059 2023-05-25 19:17:46.752187 fluidsimfoam-0.0.6/src/fluidsimfoam/__init__.py
--rw-r--r--   0        0        0     3164 2023-06-02 09:21:38.899122 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__init__.py
--rw-r--r--   0        0        0     3428 2023-06-02 09:23:55.178145 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    16781 2023-06-02 07:08:26.447668 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/ast.cpython-310.pyc
--rw-r--r--   0        0        0     1980 2023-05-25 19:19:08.676600 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/constant_files.cpython-310.pyc
--rw-r--r--   0        0        0     3457 2023-06-01 08:42:32.898140 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/control_dict.cpython-310.pyc
--rw-r--r--   0        0        0     2743 2023-06-07 09:45:32.720354 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/decompose_par.cpython-310.pyc
--rw-r--r--   0        0        0     7155 2023-05-30 20:33:58.056468 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/fields.cpython-310.pyc
--rw-r--r--   0        0        0     1450 2023-06-02 09:25:06.533632 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/format.cpython-310.pyc
--rw-r--r--   0        0        0     5005 2023-05-22 18:59:45.385794 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/fv_options.cpython-310.pyc
--rw-r--r--   0        0        0     2441 2023-05-24 19:26:28.851965 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes.cpython-310.pyc
--rw-r--r--   0        0        0     1844 2023-05-05 07:20:02.628943 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes_helper.cpython-310.pyc
--rw-r--r--   0        0        0     5418 2023-05-23 07:52:07.543018 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/generators.cpython-310.pyc
--rw-r--r--   0        0        0    10473 2023-05-09 12:43:04.027476 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/parser.cpython-310.pyc
--rw-r--r--   0        0        0     1082 2023-05-03 21:01:43.908143 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/polymesh.cpython-310.pyc
--rw-r--r--   0        0        0      889 2023-05-24 19:26:28.847965 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/util.cpython-310.pyc
--rw-r--r--   0        0        0    16765 2023-06-02 07:07:00.868495 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/ast.py
--rw-r--r--   0        0        0     1080 2023-04-23 15:48:42.099657 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/LICENSE
--rw-r--r--   0        0        0    16070 2023-06-05 19:44:44.570045 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/__init__.py
--rw-r--r--   0        0        0    17560 2023-06-05 19:44:47.242342 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2999 2023-06-05 19:24:15.763776 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/edges.cpython-310.pyc
--rw-r--r--   0        0        0     3085 2023-05-05 07:26:24.622314 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/grading.cpython-310.pyc
--rw-r--r--   0        0        0     2124 2023-06-05 19:23:23.082283 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/edges.py
--rw-r--r--   0        0        0     3426 2023-04-24 20:58:16.942659 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/grading.py
--rw-r--r--   0        0        0     2058 2023-05-25 19:17:46.752187 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/constant_files.py
--rw-r--r--   0        0        0     2822 2023-05-31 20:11:47.954320 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/control_dict.py
--rw-r--r--   0        0        0     3238 2023-06-07 07:30:57.181605 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/decompose_par.py
--rw-r--r--   0        0        0     6673 2023-05-30 19:50:15.784136 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/fields.py
--rw-r--r--   0        0        0     1345 2023-06-02 09:25:03.501654 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/format.py
--rw-r--r--   0        0        0     6107 2023-05-22 18:56:58.335368 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/fv_options.py
--rw-r--r--   0        0        0     1987 2023-05-24 19:23:08.313065 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/fv_schemes.py
--rw-r--r--   0        0        0     5250 2023-05-23 07:52:05.747013 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/generators.py
--rw-r--r--   0        0        0     1916 2023-05-16 18:45:49.936442 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/grammar.lark
--rw-r--r--   0        0        0     2337 2023-05-16 18:45:49.940441 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/grammar_advanced.lark
--rw-r--r--   0        0        0     9522 2023-05-09 12:42:41.039310 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/parser.py
--rw-r--r--   0        0        0      973 2023-05-03 19:26:40.332634 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/polymesh.py
--rw-r--r--   0        0        0      766 2023-05-24 19:24:59.484896 fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/util.py
--rw-r--r--   0        0        0     1400 2023-05-09 20:05:14.235128 fluidsimfoam-0.0.6/src/fluidsimfoam/info.py
--rw-r--r--   0        0        0      124 2023-05-09 13:01:28.476575 fluidsimfoam-0.0.6/src/fluidsimfoam/init_fields.py
--rw-r--r--   0        0        0      747 2023-05-09 13:00:38.420124 fluidsimfoam-0.0.6/src/fluidsimfoam/log.py
--rw-r--r--   0        0        0      608 2023-05-11 19:44:39.696948 fluidsimfoam-0.0.6/src/fluidsimfoam/make.py
--rw-r--r--   0        0        0     1210 2023-05-22 18:56:58.335368 fluidsimfoam-0.0.6/src/fluidsimfoam/operators.py
--rw-r--r--   0        0        0      423 2023-05-25 19:38:04.703998 fluidsimfoam-0.0.6/src/fluidsimfoam/output/__init__.py
--rw-r--r--   0        0        0      544 2023-05-25 19:41:05.807251 fluidsimfoam-0.0.6/src/fluidsimfoam/output/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7746 2023-06-04 20:15:04.168667 fluidsimfoam-0.0.6/src/fluidsimfoam/output/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     1539 2023-05-25 19:19:08.700611 fluidsimfoam-0.0.6/src/fluidsimfoam/output/__pycache__/dataframe_from_paths.cpython-310.pyc
--rw-r--r--   0        0        0     3514 2023-06-07 09:45:34.666101 fluidsimfoam-0.0.6/src/fluidsimfoam/output/__pycache__/fields.cpython-310.pyc
--rw-r--r--   0        0        0     5445 2023-05-25 19:19:08.944725 fluidsimfoam-0.0.6/src/fluidsimfoam/output/__pycache__/log.cpython-310.pyc
--rw-r--r--   0        0        0    10233 2023-06-04 20:13:56.099256 fluidsimfoam-0.0.6/src/fluidsimfoam/output/base.py
--rw-r--r--   0        0        0     1080 2023-05-25 19:17:46.756188 fluidsimfoam-0.0.6/src/fluidsimfoam/output/dataframe_from_paths.py
--rw-r--r--   0        0        0     2998 2023-06-07 07:30:21.271923 fluidsimfoam-0.0.6/src/fluidsimfoam/output/fields.py
--rw-r--r--   0        0        0     6580 2023-05-25 19:17:46.756188 fluidsimfoam-0.0.6/src/fluidsimfoam/output/log.py
--rw-r--r--   0        0        0     2886 2023-05-22 18:56:58.339368 fluidsimfoam-0.0.6/src/fluidsimfoam/params.py
--rw-r--r--   0        0        0     1516 2023-05-30 19:50:11.700069 fluidsimfoam-0.0.6/src/fluidsimfoam/resources/LICENSE.template
--rw-r--r--   0        0        0      235 2023-05-30 19:50:11.700069 fluidsimfoam-0.0.6/src/fluidsimfoam/resources/README.md.template
--rw-r--r--   0        0        0      573 2023-05-09 13:02:35.270502 fluidsimfoam-0.0.6/src/fluidsimfoam/resources/__init__.py
--rw-r--r--   0        0        0      535 2023-05-30 19:50:11.700069 fluidsimfoam-0.0.6/src/fluidsimfoam/resources/__init__.py.template
--rw-r--r--   0        0        0      955 2023-05-09 13:02:39.537858 fluidsimfoam-0.0.6/src/fluidsimfoam/resources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      516 2023-06-01 20:14:27.398486 fluidsimfoam-0.0.6/src/fluidsimfoam/resources/output.py.template
--rw-r--r--   0        0        0      507 2023-06-01 09:02:52.471699 fluidsimfoam-0.0.6/src/fluidsimfoam/resources/pyproject.toml.template
--rw-r--r--   0        0        0       42 2023-05-30 19:50:11.700069 fluidsimfoam-0.0.6/src/fluidsimfoam/resources/tasks.py.template
--rw-r--r--   0        0        0      726 2023-06-02 09:41:43.285771 fluidsimfoam-0.0.6/src/fluidsimfoam/resources/test_generated_solver.py.template
--rw-r--r--   0        0        0     2765 2023-05-09 13:04:52.906067 fluidsimfoam-0.0.6/src/fluidsimfoam/solvers/__init__.py
--rw-r--r--   0        0        0     2620 2023-05-09 13:05:27.378825 fluidsimfoam-0.0.6/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2748 2023-05-24 19:26:28.699960 fluidsimfoam-0.0.6/src/fluidsimfoam/solvers/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     2915 2023-05-24 19:14:04.619885 fluidsimfoam-0.0.6/src/fluidsimfoam/solvers/base.py
--rw-r--r--   0        0        0     3298 2023-06-02 08:33:23.157994 fluidsimfoam-0.0.6/src/fluidsimfoam/tasks.py
--rw-r--r--   0        0        0     1716 2023-06-05 19:47:19.026905 fluidsimfoam-0.0.6/src/fluidsimfoam/testing.py
--rw-r--r--   0        0        0       77 2023-05-09 20:05:14.251128 fluidsimfoam-0.0.6/src/fluidsimfoam/util/__init__.py
--rw-r--r--   0        0        0      238 2023-05-09 20:27:04.597492 fluidsimfoam-0.0.6/src/fluidsimfoam/util/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5471 2023-06-02 09:35:15.850833 fluidsimfoam-0.0.6/src/fluidsimfoam/util/__pycache__/console.cpython-310.pyc
--rw-r--r--   0        0        0     6906 2023-06-02 09:35:05.306884 fluidsimfoam-0.0.6/src/fluidsimfoam/util/console.py
--rw-r--r--   0        0        0     8672 1970-01-01 00:00:00.000000 fluidsimfoam-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1521 2023-03-02 21:01:46.291446 fluidsimfoam-0.0.7/LICENSE
+-rw-r--r--   0        0        0     7375 2023-06-04 19:44:44.715013 fluidsimfoam-0.0.7/README.md
+-rw-r--r--   0        0        0     2583 2023-06-26 20:15:21.248924 fluidsimfoam-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2060 2023-06-22 12:49:10.680089 fluidsimfoam-0.0.7/src/fluidsimfoam/__init__.py
+-rw-r--r--   0        0        0     4068 2023-06-26 19:57:36.119413 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__init__.py
+-rw-r--r--   0        0        0     4204 2023-06-26 19:59:23.383917 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    16681 2023-06-19 14:07:08.903130 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/ast.cpython-310.pyc
+-rw-r--r--   0        0        0     1980 2023-05-25 19:19:08.676600 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/constant_files.cpython-310.pyc
+-rw-r--r--   0        0        0     3457 2023-06-01 08:42:32.898140 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/control_dict.cpython-310.pyc
+-rw-r--r--   0        0        0     3435 2023-06-21 22:24:18.919311 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/decompose_par.cpython-310.pyc
+-rw-r--r--   0        0        0     8504 2023-06-26 19:59:23.531955 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/fields.cpython-310.pyc
+-rw-r--r--   0        0        0     1496 2023-06-17 19:47:51.274014 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/format.cpython-310.pyc
+-rw-r--r--   0        0        0     5005 2023-05-22 18:59:45.385794 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/fv_options.cpython-310.pyc
+-rw-r--r--   0        0        0     2441 2023-05-24 19:26:28.851965 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes.cpython-310.pyc
+-rw-r--r--   0        0        0     1844 2023-05-05 07:20:02.628943 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes_helper.cpython-310.pyc
+-rw-r--r--   0        0        0     5380 2023-06-19 11:39:20.213779 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/generators.cpython-310.pyc
+-rw-r--r--   0        0        0    10369 2023-06-26 19:59:23.387918 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/parser.cpython-310.pyc
+-rw-r--r--   0        0        0     1082 2023-05-03 21:01:43.908143 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/polymesh.cpython-310.pyc
+-rw-r--r--   0        0        0      889 2023-05-24 19:26:28.847965 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/util.cpython-310.pyc
+-rw-r--r--   0        0        0    16822 2023-06-19 14:07:07.195184 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/ast.py
+-rw-r--r--   0        0        0     1080 2023-04-23 15:48:42.099657 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/blockmesh/LICENSE
+-rw-r--r--   0        0        0    16070 2023-06-05 19:44:44.570045 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/blockmesh/__init__.py
+-rw-r--r--   0        0        0    17560 2023-06-05 19:44:47.242342 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2999 2023-06-05 19:24:15.763776 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/edges.cpython-310.pyc
+-rw-r--r--   0        0        0     3085 2023-05-05 07:26:24.622314 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/grading.cpython-310.pyc
+-rw-r--r--   0        0        0     2124 2023-06-05 19:23:23.082283 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/blockmesh/edges.py
+-rw-r--r--   0        0        0     3426 2023-04-24 20:58:16.942659 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/blockmesh/grading.py
+-rw-r--r--   0        0        0     2058 2023-05-25 19:17:46.752187 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/constant_files.py
+-rw-r--r--   0        0        0     2822 2023-05-31 20:11:47.954320 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/control_dict.py
+-rw-r--r--   0        0        0     4209 2023-06-21 22:22:32.717960 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/decompose_par.py
+-rw-r--r--   0        0        0     8799 2023-06-26 19:57:36.119413 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/fields.py
+-rw-r--r--   0        0        0     1483 2023-06-17 19:27:38.753396 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/format.py
+-rw-r--r--   0        0        0     6107 2023-05-22 18:56:58.335368 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/fv_options.py
+-rw-r--r--   0        0        0     1987 2023-05-24 19:23:08.313065 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/fv_schemes.py
+-rw-r--r--   0        0        0     5295 2023-06-19 11:37:36.816521 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/generators.py
+-rw-r--r--   0        0        0     1808 2023-06-19 13:59:54.496884 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/grammar.lark
+-rw-r--r--   0        0        0     2282 2023-06-19 14:01:04.118684 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/grammar_advanced.lark
+-rw-r--r--   0        0        0     9222 2023-06-26 19:57:36.119413 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/parser.py
+-rw-r--r--   0        0        0      973 2023-05-03 19:26:40.332634 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/polymesh.py
+-rw-r--r--   0        0        0      766 2023-05-24 19:24:59.484896 fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/util.py
+-rw-r--r--   0        0        0     1400 2023-05-09 20:05:14.235128 fluidsimfoam-0.0.7/src/fluidsimfoam/info.py
+-rw-r--r--   0        0        0      124 2023-05-09 13:01:28.476575 fluidsimfoam-0.0.7/src/fluidsimfoam/init_fields.py
+-rw-r--r--   0        0        0       87 2023-06-21 22:22:32.721958 fluidsimfoam-0.0.7/src/fluidsimfoam/invoke/__init__.py
+-rw-r--r--   0        0        0      250 2023-06-22 12:49:14.475648 fluidsimfoam-0.0.7/src/fluidsimfoam/invoke/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3398 2023-06-22 13:13:03.091638 fluidsimfoam-0.0.7/src/fluidsimfoam/invoke/__pycache__/context.cpython-310.pyc
+-rw-r--r--   0        0        0     3650 2023-06-27 21:03:43.520533 fluidsimfoam-0.0.7/src/fluidsimfoam/invoke/__pycache__/tasks.cpython-310.pyc
+-rw-r--r--   0        0        0     3848 2023-06-22 13:12:59.971650 fluidsimfoam-0.0.7/src/fluidsimfoam/invoke/context.py
+-rw-r--r--   0        0        0     3680 2023-06-27 20:56:42.313334 fluidsimfoam-0.0.7/src/fluidsimfoam/invoke/tasks.py
+-rw-r--r--   0        0        0      747 2023-05-09 13:00:38.420124 fluidsimfoam-0.0.7/src/fluidsimfoam/log.py
+-rw-r--r--   0        0        0      608 2023-05-11 19:44:39.696948 fluidsimfoam-0.0.7/src/fluidsimfoam/make.py
+-rw-r--r--   0        0        0     1210 2023-05-22 18:56:58.335368 fluidsimfoam-0.0.7/src/fluidsimfoam/operators.py
+-rw-r--r--   0        0        0      423 2023-05-25 19:38:04.703998 fluidsimfoam-0.0.7/src/fluidsimfoam/output/__init__.py
+-rw-r--r--   0        0        0      544 2023-05-25 19:41:05.807251 fluidsimfoam-0.0.7/src/fluidsimfoam/output/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7935 2023-06-19 12:18:02.243530 fluidsimfoam-0.0.7/src/fluidsimfoam/output/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     1539 2023-05-25 19:19:08.700611 fluidsimfoam-0.0.7/src/fluidsimfoam/output/__pycache__/dataframe_from_paths.cpython-310.pyc
+-rw-r--r--   0        0        0    12368 2023-06-27 19:55:58.448800 fluidsimfoam-0.0.7/src/fluidsimfoam/output/__pycache__/fields.cpython-310.pyc
+-rw-r--r--   0        0        0     5445 2023-05-25 19:19:08.944725 fluidsimfoam-0.0.7/src/fluidsimfoam/output/__pycache__/log.cpython-310.pyc
+-rw-r--r--   0        0        0    10564 2023-06-19 12:17:59.879284 fluidsimfoam-0.0.7/src/fluidsimfoam/output/base.py
+-rw-r--r--   0        0        0     1080 2023-05-25 19:17:46.756188 fluidsimfoam-0.0.7/src/fluidsimfoam/output/dataframe_from_paths.py
+-rw-r--r--   0        0        0    14006 2023-06-27 19:49:18.892432 fluidsimfoam-0.0.7/src/fluidsimfoam/output/fields.py
+-rw-r--r--   0        0        0     6580 2023-05-25 19:17:46.756188 fluidsimfoam-0.0.7/src/fluidsimfoam/output/log.py
+-rw-r--r--   0        0        0     2886 2023-05-22 18:56:58.339368 fluidsimfoam-0.0.7/src/fluidsimfoam/params.py
+-rw-r--r--   0        0        0     1516 2023-05-30 19:50:11.700069 fluidsimfoam-0.0.7/src/fluidsimfoam/resources/LICENSE.template
+-rw-r--r--   0        0        0      235 2023-05-30 19:50:11.700069 fluidsimfoam-0.0.7/src/fluidsimfoam/resources/README.md.template
+-rw-r--r--   0        0        0      573 2023-05-09 13:02:35.270502 fluidsimfoam-0.0.7/src/fluidsimfoam/resources/__init__.py
+-rw-r--r--   0        0        0      535 2023-05-30 19:50:11.700069 fluidsimfoam-0.0.7/src/fluidsimfoam/resources/__init__.py.template
+-rw-r--r--   0        0        0      955 2023-05-09 13:02:39.537858 fluidsimfoam-0.0.7/src/fluidsimfoam/resources/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      559 2023-06-19 08:19:58.219408 fluidsimfoam-0.0.7/src/fluidsimfoam/resources/output.py.template
+-rw-r--r--   0        0        0      507 2023-06-01 09:02:52.471699 fluidsimfoam-0.0.7/src/fluidsimfoam/resources/pyproject.toml.template
+-rw-r--r--   0        0        0       49 2023-06-22 20:23:35.079865 fluidsimfoam-0.0.7/src/fluidsimfoam/resources/tasks.py.template
+-rw-r--r--   0        0        0      725 2023-06-21 22:22:32.721958 fluidsimfoam-0.0.7/src/fluidsimfoam/resources/test_generated_solver.py.template
+-rw-r--r--   0        0        0     2765 2023-05-09 13:04:52.906067 fluidsimfoam-0.0.7/src/fluidsimfoam/solvers/__init__.py
+-rw-r--r--   0        0        0     2620 2023-05-09 13:05:27.378825 fluidsimfoam-0.0.7/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2748 2023-05-24 19:26:28.699960 fluidsimfoam-0.0.7/src/fluidsimfoam/solvers/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     2915 2023-05-24 19:14:04.619885 fluidsimfoam-0.0.7/src/fluidsimfoam/solvers/base.py
+-rw-r--r--   0        0        0     1716 2023-06-05 19:47:19.026905 fluidsimfoam-0.0.7/src/fluidsimfoam/testing.py
+-rw-r--r--   0        0        0     1380 2023-06-21 22:22:32.721958 fluidsimfoam-0.0.7/src/fluidsimfoam/util/__init__.py
+-rw-r--r--   0        0        0     1374 2023-06-21 22:39:16.034118 fluidsimfoam-0.0.7/src/fluidsimfoam/util/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6570 2023-06-19 13:04:04.355454 fluidsimfoam-0.0.7/src/fluidsimfoam/util/__pycache__/console.cpython-310.pyc
+-rw-r--r--   0        0        0     8688 2023-06-19 13:02:15.131658 fluidsimfoam-0.0.7/src/fluidsimfoam/util/console.py
+-rw-r--r--   0        0        0     8759 1970-01-01 00:00:00.000000 fluidsimfoam-0.0.7/PKG-INFO
```

### Comparing `fluidsimfoam-0.0.6/LICENSE` & `fluidsimfoam-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/README.md` & `fluidsimfoam-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/pyproject.toml` & `fluidsimfoam-0.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fluidsimfoam"
-version = "0.0.6"
+version = "0.0.7"
 description = "Python framework for OpenFOAM"
 authors = ["pierre.augier <pierre.augier@univ-grenoble-alpes.fr>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -18,27 +18,30 @@
 rich = "^13.3.3"
 invoke = "^2.0.0"
 PySide6 = {version = "^6.5.1", optional = true, python = ">=3.9,<3.12"}
 jupyterlab = {version = "^3.6.3", optional = true}
 jupyterlab_myst = {version = "^1.1.3", optional = true}
 jupytext = {version = "^1.14.5", optional = true}
 mdformat-myst = {version = "^0.1.4", optional = true}
+pyvista = {version = "^0.39.1", optional = true}
 
 [tool.poetry.extras]
 qt = ["PySide6"]
 jupyter = ["jupyterlab", "jupyterlab_myst", "jupytext", "mdformat-myst"]
+pyvista = ["pyvista"]
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.1"
 fluidsimfoam-tgv = { path = "./doc/examples/fluidsimfoam-tgv/", develop = true }
 fluidsimfoam-cbox = { path = "./doc/examples/fluidsimfoam-cbox/", develop = true }
 fluidsimfoam-sed = { path = "./doc/examples/fluidsimfoam-sed/", develop = true }
 fluidsimfoam-cavity = { path = "./doc/examples/fluidsimfoam-cavity/", develop = true }
 fluidsimfoam-phill = { path = "./doc/examples/fluidsimfoam-phill/", develop = true }
 fluidsimfoam-dam = { path = "./doc/examples/fluidsimfoam-dam/", develop = true }
+fluidsimfoam-multi-region-snappy = { path = "./doc/examples/fluidsimfoam-multi-region-snappy/", develop = true }
 pytest-mock = "^3.10.0"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
@@ -47,14 +50,15 @@
 twine = "^4.0.2"
 
 [tool.poetry.group.doc.dependencies]
 myst-nb = "^0.17.1"
 sphinx-inline-tabs = "^2022.1.2b11"
 sphinx-copybutton = "^0.5.1"
 pydata-sphinx-theme = "^0.13.1"
+sphinx-togglebutton = "^0.3.2"
 
 [tool.poetry.scripts]
 fluidsimfoam-info = 'fluidsimfoam.util.console:print_versions'
 fluidsimfoam-ipy-load = 'fluidsimfoam.util.console:start_ipython_load_sim'
 fluidsimfoam-initiate-solver = "fluidsimfoam.util.console:initiate_solver"
 
 [build-system]
@@ -69,8 +73,9 @@
 
 [tool.coverage.report]
 exclude_lines = [
     "raise AssertionError",
     "raise NotImplementedError",
     "raise RuntimeError",
     "raise ValueError",
+    "except ImportError",
 ]
```

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/__init__.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,26 @@
    :toctree:
 
    foam_input_files
    solvers
    output
    util
    resources
+   invoke
 
 .. rubric:: Modules
 
 .. autosummary::
    :toctree:
 
    info
    make
    init_fields
    operators
    log
-   tasks
    testing
    params
 
 """
 import importlib.metadata
 import sys
```

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__init__.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     "ConstantFileHelper",
     "BlockMeshDictRectilinear",
     "FvOptionsHelper",
     "DimensionSet",
     "DecomposeParDictHelper",
     "format_code",
     "FoamFormatError",
+    "read_header",
+    "parse_header",
 ]
 
 
 def _as_py_name(name):
     return underscore(name).replace(".", "_")
 
 
@@ -110,14 +112,44 @@
 |   \\  /    A nd           | Website:  www.openfoam.com                      |
 |    \\/     M anipulation  |                                                 |
 \*---------------------------------------------------------------------------*/
 """
 
 DEFAULT_HEADER = DEFAULT_HEADER[1:-1]
 
+
+def read_header(path):
+    """Read the header ("FoamFile" entry) of an OpenFOAM file"""
+    lines_header = []
+    with open(path) as file:
+        # reach header
+        for line in file:
+            if line.startswith("FoamFile\n"):
+                lines_header.append(line)
+                break
+        for line in file:
+            lines_header.append(line)
+            if line.startswith("}"):
+                break
+        if not lines_header:
+            raise ValueError("No FoamFile entry found")
+        code_header = "".join(lines_header)
+        tree = parse(code_header)
+        return tree.value
+
+
+def parse_header(code: str):
+    """Parse the header ("FoamFile" entry) of an OpenFOAM file"""
+    code_header = (
+        "FoamFile" + code.split("FoamFile", 1)[1].split("\n}", 1)[0] + "\n}"
+    )
+    tree = parse(code_header)
+    return tree.value
+
+
 from .blockmesh import BlockMeshDict, BlockMeshDictRectilinear, Vertex
 from .constant_files import ConstantFileHelper
 from .control_dict import ControlDictHelper
 from .decompose_par import DecomposeParDictHelper
 from .fields import (
     VolScalarField,
     VolVectorField,
```

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/ast.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/ast.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  2 07:07:00 2023 UTC, .py size: 16765 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 1495 7964 7d41 0000  o.........yd}A..
+00000000: 6f0d 0d0a 0000 0000 0b61 9064 b641 0000  o........a.d.A..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 8e01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6401 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6407 6c0b 6d0c 5a0c 0100 6401 6402 6c0d  d.l.m.Z...d.d.l.
@@ -31,15 +31,15 @@
 000001e0: 414d 2069 6e70 7574 2066 696c 6573 e900  AM input files..
 000001f0: 0000 004e 2902 da03 4142 43da 0e61 6273  ...N)...ABC..abs
 00000200: 7472 6163 746d 6574 686f 6429 01da 0964  tractmethod)...d
 00000210: 6174 6163 6c61 7373 2901 da06 4e75 6d62  ataclass)...Numb
 00000220: 6572 2901 da06 6465 6465 6e74 2901 da08  er)...dedent)...
 00000230: 4f70 7469 6f6e 616c 2901 da0a 756e 6465  Optional)...unde
 00000240: 7273 636f 7265 2907 5a02 6b67 da01 6dda  rscore).Z.kg..m.
-00000250: 0173 da01 4b5a 046b 6d6f 6cda 0141 da02  .s..KZ.kmol..A..
+00000250: 0173 da01 4b5a 046b 6d6f 6cda 0141 5a02  .s..KZ.kmol..AZ.
 00000260: 6364 6301 0000 0000 0000 0000 0000 0009  cdc.............
 00000270: 0000 0008 0000 0043 0000 0073 d600 0000  .......C...s....
 00000280: 6401 6701 6402 1400 7d01 6403 7d02 7c00  d.g.d...}.d.}.|.
 00000290: 7269 7a0a 7400 a001 6404 7c00 a102 a002  riz.t...d.|.....
 000002a0: a100 7d03 5700 6e0f 0400 7403 7922 0100  ..}.W.n...t.y"..
 000002b0: 0100 0100 7c00 7d04 6405 7d00 6406 7d05  ....|.}.d.}.d.}.
 000002c0: 5900 6e19 7700 7c00 7c03 1900 7d05 7c05  Y.n.w.|.|...}.|.
@@ -55,53 +55,53 @@
 00000360: 0000 00e9 0100 0000 7a04 5b2f 2e5d da00  ........z.[/.]..
 00000370: da01 2e7a 022f 2efa 015e da01 31e9 ffff  ...z./...^..1...
 00000380: ffff 2908 da02 7265 da06 7365 6172 6368  ..)...re..search
 00000390: da05 7374 6172 74da 0e41 7474 7269 6275  ..start..Attribu
 000003a0: 7465 4572 726f 72da 0573 706c 6974 da03  teError..split..
 000003b0: 696e 74da 0773 796d 626f 6c73 da05 696e  int..symbols..in
 000003c0: 6465 7829 09da 0575 6e69 7473 da06 7265  dex)...units..re
-000003d0: 7375 6c74 da04 7369 676e 721c 0000 005a  sult..signr....Z
+000003d0: 7375 6c74 da04 7369 676e 721b 0000 005a  sult..signr....Z
 000003e0: 0875 6e69 745f 616c 6c5a 096e 6578 745f  .unit_allZ.next_
 000003f0: 6f70 6572 da09 756e 6974 5f6e 616d 655a  oper..unit_nameZ
 00000400: 0a75 6e69 745f 7661 6c75 655a 0a75 6e69  .unit_valueZ.uni
-00000410: 745f 696e 6465 78a9 0072 2100 0000 fa46  t_index..r!....F
+00000410: 745f 696e 6465 78a9 0072 2000 0000 fa46  t_index..r ....F
 00000420: 2f68 6f6d 652f 7069 6572 7265 2f44 6576  /home/pierre/Dev
 00000430: 2f66 6c75 6964 7369 6d66 6f61 6d2f 7372  /fluidsimfoam/sr
 00000440: 632f 666c 7569 6473 696d 666f 616d 2f66  c/fluidsimfoam/f
 00000450: 6f61 6d5f 696e 7075 745f 6669 6c65 732f  oam_input_files/
 00000460: 6173 742e 7079 da0e 7374 7232 666f 616d  ast.py..str2foam
 00000470: 5f75 6e69 7473 1000 0000 7330 0000 000a  _units....s0....
 00000480: 0104 0104 0102 0114 010c 0104 0104 0108  ................
 00000490: 0102 fd08 050c 010c 0110 0108 010e 010a  ................
 000004a0: 010a 0208 010a 010c 0110 0104 ec04 1572  ...............r
-000004b0: 2300 0000 6301 0000 0000 0000 0000 0000  #...c...........
+000004b0: 2200 0000 6301 0000 0000 0000 0000 0000  "...c...........
 000004c0: 0005 0000 0008 0000 0043 0000 0073 a800  .........C...s..
 000004d0: 0000 6700 7d01 7400 7401 7c00 8302 4400  ..g.}.t.t.|...D.
 000004e0: 5d2f 5c02 7d02 7d03 7c03 6401 6b02 7210  ]/\.}.}.|.d.k.r.
 000004f0: 7107 7c03 6401 6b04 7216 6402 6e01 6403  q.|.d.k.r.d.n.d.
 00000500: 7d04 7402 7c03 8301 6404 6b02 7228 7c01  }.t.|...d.k.r(|.
 00000510: a003 7c04 9b00 7c02 9b00 9d02 a101 0100  ..|...|.........
 00000520: 7107 7c01 a003 7c04 9b00 7c02 9b00 6405  q.|...|...|...d.
 00000530: 7402 7c03 8301 9b00 9d04 a101 0100 7107  t.|...........q.
 00000540: 6406 a004 7c01 a101 7d01 7c01 a005 6402  d...|...}.|...d.
 00000550: a101 7249 7c01 6404 6400 8502 1900 7d01  ..rI|.d.d.....}.
 00000560: 7c01 5300 7c01 a005 6403 a101 7252 6407  |.S.|...d...rRd.
 00000570: 7c01 1700 7d01 7c01 5300 2908 4e72 0100  |...}.|.S.).Nr..
-00000580: 0000 7211 0000 00fa 012f 720f 0000 0072  ..r....../r....r
-00000590: 1200 0000 7210 0000 0072 1300 0000 2906  ....r....r....).
-000005a0: da03 7a69 7072 1b00 0000 da03 6162 73da  ..zipr......abs.
+00000580: 0000 7210 0000 00fa 012f 720e 0000 0072  ..r....../r....r
+00000590: 1100 0000 720f 0000 0072 1200 0000 2906  ....r....r....).
+000005a0: da03 7a69 7072 1a00 0000 da03 6162 73da  ..zipr......abs.
 000005b0: 0661 7070 656e 64da 046a 6f69 6eda 0a73  .append..join..s
 000005c0: 7461 7274 7377 6974 6829 05da 0a66 6f61  tartswith)...foa
-000005d0: 6d5f 756e 6974 7372 1e00 0000 da06 7379  m_unitsr......sy
+000005d0: 6d5f 756e 6974 7372 1d00 0000 da06 7379  m_unitsr......sy
 000005e0: 6d62 6f6c da08 6578 706f 6e65 6e74 da08  mbol..exponent..
-000005f0: 6f70 6572 6174 6f72 7221 0000 0072 2100  operatorr!...r!.
-00000600: 0000 7222 0000 00da 0e66 6f61 6d5f 756e  ..r".....foam_un
+000005f0: 6f70 6572 6174 6f72 7220 0000 0072 2000  operatorr ...r .
+00000600: 0000 7221 0000 00da 0e66 6f61 6d5f 756e  ..r!.....foam_un
 00000610: 6974 7332 7374 722b 0000 0073 1e00 0000  its2str+...s....
 00000620: 0401 1201 0801 0201 1001 0c01 1401 1e02  ................
-00000630: 0a01 0a01 0c01 0403 0afe 0801 0401 722e  ..............r.
+00000630: 0a01 0a01 0c01 0403 0afe 0801 0401 722d  ..............r-
 00000640: 0000 00e9 1400 0000 6302 0000 0000 0000  ........c.......
 00000650: 0000 0000 0003 0000 0008 0000 0043 0000  .............C..
 00000660: 0073 4400 0000 7a10 7400 7c01 7401 6401  .sD...z.t.|.t.d.
 00000670: 6402 8400 7c00 a002 a100 4400 8301 8301  d...|.....D.....
 00000680: 8302 7d01 5700 6e0b 0400 7403 791b 0100  ..}.W.n...t.y...
 00000690: 0100 0100 6403 7d01 5900 6e01 7700 6404  ....d.}.Y.n.w.d.
 000006a0: 7d02 7c01 7c02 1700 5300 2905 4e63 0100  }.|.|...S.).Nc..
@@ -109,57 +109,57 @@
 000006c0: 0000 7300 0000 7332 0000 0081 007c 005d  ..s...s2.....|.]
 000006d0: 145c 027d 017d 027c 0264 0075 0172 0274  .\.}.}.|.d.u.r.t
 000006e0: 007c 0274 0174 0266 0283 0273 0274 037c  .|.t.t.f...s.t.|
 000006f0: 0183 0156 0001 0071 0264 0053 00a9 014e  ...V...q.d.S...N
 00000700: 2904 da0a 6973 696e 7374 616e 6365 da04  )...isinstance..
 00000710: 4469 6374 da04 4c69 7374 da03 6c65 6e29  Dict..List..len)
 00000720: 03da 022e 30da 036b 6579 da05 7661 6c75  ....0..key..valu
-00000730: 6572 2100 0000 7221 0000 0072 2200 0000  er!...r!...r"...
+00000730: 6572 2000 0000 7220 0000 0072 2100 0000  er ...r ...r!...
 00000740: da09 3c67 656e 6578 7072 3e41 0000 0073  ..<genexpr>A...s
 00000750: 1200 0000 0280 0400 0602 0601 02fd 0c03  ................
 00000760: 02fd 0601 0aff 7a2b 5f63 6f6d 7075 7465  ......z+_compute
 00000770: 5f73 7061 6365 735f 746f 5f61 6c69 676e  _spaces_to_align
 00000780: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
 00000790: 7072 3e72 0100 0000 e904 0000 0029 04da  pr>r.........)..
 000007a0: 036d 696e da03 6d61 78da 0569 7465 6d73  .min..max..items
 000007b0: da0a 5661 6c75 6545 7272 6f72 2903 da04  ..ValueError)...
 000007c0: 6461 7461 da0a 6d61 785f 6c65 6e67 7468  data..max_length
 000007d0: 5a0d 6465 6661 756c 745f 7370 6163 6572  Z.default_spacer
-000007e0: 2100 0000 7221 0000 0072 2200 0000 da18  !...r!...r".....
+000007e0: 2000 0000 7220 0000 0072 2100 0000 da18   ...r ...r!.....
 000007f0: 5f63 6f6d 7075 7465 5f73 7061 6365 735f  _compute_spaces_
 00000800: 746f 5f61 6c69 676e 3d00 0000 7318 0000  to_align=...s...
 00000810: 0002 0102 0102 0108 0106 0206 fe08 fe0c  ................
-00000820: 0808 0102 ff04 0308 0172 4000 0000 6300  .........r@...c.
+00000820: 0808 0102 ff04 0308 0172 3f00 0000 6300  .........r?...c.
 00000830: 0000 0000 0000 0000 0000 0000 0000 0002  ................
 00000840: 0000 0040 0000 0073 1400 0000 6500 5a01  ...@...s....e.Z.
 00000850: 6400 5a02 6401 6402 8400 5a03 6403 5300  d.Z.d.d...Z.d.S.
 00000860: 2904 da04 4e6f 6465 6302 0000 0000 0000  )...Nodec.......
 00000870: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
 00000880: 0073 2000 0000 7400 7c01 8301 7400 7c00  .s ...t.|...t.|.
 00000890: 8301 7500 720e 7c00 6a01 7c01 6a01 6b02  ..u.r.|.j.|.j.k.
 000008a0: 5300 6401 5300 2902 4e46 2902 da04 7479  S.d.S.).NF)...ty
 000008b0: 7065 da08 5f5f 6469 6374 5f5f 2902 da04  pe..__dict__)...
-000008c0: 7365 6c66 da05 6f74 6865 7272 2100 0000  self..otherr!...
-000008d0: 7221 0000 0072 2200 0000 da06 5f5f 6571  r!...r".....__eq
+000008c0: 7365 6c66 da05 6f74 6865 7272 2000 0000  self..otherr ...
+000008d0: 7220 0000 0072 2100 0000 da06 5f5f 6571  r ...r!.....__eq
 000008e0: 5f5f 4f00 0000 7306 0000 0010 010c 0104  __O...s.........
 000008f0: 017a 0b4e 6f64 652e 5f5f 6571 5f5f 4e29  .z.Node.__eq__N)
 00000900: 04da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
 00000910: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00000920: 616d 655f 5f72 4600 0000 7221 0000 0072  ame__rF...r!...r
-00000930: 2100 0000 7221 0000 0072 2200 0000 7241  !...r!...r"...rA
+00000920: 616d 655f 5f72 4500 0000 7220 0000 0072  ame__rE...r ...r
+00000930: 2000 0000 7220 0000 0072 2100 0000 7240   ...r ...r!...r@
 00000940: 0000 004e 0000 0073 0400 0000 0800 0c01  ...N...s........
-00000950: 7241 0000 0063 0000 0000 0000 0000 0000  rA...c..........
+00000950: 7240 0000 0063 0000 0000 0000 0000 0000  r@...c..........
 00000960: 0000 0000 0000 0800 0000 4000 0000 7350  ..........@...sP
 00000970: 0000 0065 005a 0164 005a 0209 0109 0209  ...e.Z.d.Z......
 00000980: 0164 0e64 0365 0364 0465 0465 0319 0064  .d.d.e.d.e.e...d
 00000990: 0565 0465 0319 0066 0664 0664 0784 055a  .e.e...f.d.d...Z
 000009a0: 0564 0864 0984 005a 0664 0f64 0a64 0b84  .d.d...Z.d.d.d..
 000009b0: 015a 0765 0864 0c64 0d84 0083 015a 0964  .Z.e.d.d.....Z.d
 000009c0: 0153 0029 10da 0e4e 6f64 654c 696b 6550  .S.)...NodeLikeP
-000009d0: 7944 6963 744e 4672 3e00 0000 da0a 6469  yDictNFr>.....di
+000009d0: 7944 6963 744e 4672 3d00 0000 da0a 6469  yDictNFr=.....di
 000009e0: 6d65 6e73 696f 6e73 da08 636f 6d6d 656e  mensions..commen
 000009f0: 7473 6305 0000 0000 0000 0000 0000 000b  tsc.............
 00000a00: 0000 0007 0000 0043 0000 0073 fa00 0000  .......C...s....
 00000a10: 7c02 6400 7500 7206 6900 7d02 7c04 6400  |.d.u.r.i.}.|.d.
 00000a20: 7500 720c 6900 7d04 7c01 a000 a100 4400  u.r.i.}.|.....D.
 00000a30: 5d6a 5c02 7d05 7d06 7401 7c06 7402 6400  ]j\.}.}.t.|.t.d.
 00000a40: 8301 7403 6602 8302 7224 7c00 a004 7c05  ..t.f...r$|...|.
@@ -171,32 +171,32 @@
 00000aa0: 7c06 7c07 a103 0100 7110 7401 7c06 740a  |.|.....q.t.|.t.
 00000ab0: 8302 7275 7c02 a007 7c05 6400 a102 7d08  ..ru|...|.d...}.
 00000ac0: 7c04 a007 7c05 6400 a102 7d09 740b 6900  |...|.d...}.t.i.
 00000ad0: 7c05 7c09 6402 8d03 7d0a 7c0a 6a0c 7c06  |.|.d...}.|.j.|.
 00000ae0: 7c08 7c03 7c09 6403 8d04 0100 7c00 a00d  |.|.|.d.....|...
 00000af0: 7c05 7c0a a102 0100 7110 740e 7402 7c06  |.|.....q.t.t.|.
 00000b00: 8301 8301 8201 6400 5300 2904 4e46 2902  ......d.S.).NF).
-00000b10: da04 6e61 6d65 724c 0000 0029 0372 4b00  ..namerL...).rK.
+00000b10: da04 6e61 6d65 724b 0000 0029 0372 4a00  ..namerK...).rJ.
 00000b20: 0000 da11 6465 6661 756c 745f 6469 6d65  ....default_dime
-00000b30: 6e73 696f 6e72 4c00 0000 290f 723c 0000  nsionrL...).r<..
-00000b40: 0072 3100 0000 7242 0000 00da 0373 7472  .r1...rB.....str
+00000b30: 6e73 696f 6e72 4b00 0000 290f 723b 0000  nsionrK...).r;..
+00000b40: 0072 3000 0000 7241 0000 00da 0373 7472  .r0...rA.....str
 00000b50: da09 7365 745f 6368 696c 6472 0500 0000  ..set_childr....
-00000b60: da04 6c69 7374 da03 6765 7472 3300 0000  ..list..getr3...
+00000b60: da04 6c69 7374 da03 6765 7472 3200 0000  ..list..getr2...
 00000b70: da09 7365 745f 7661 6c75 65da 0464 6963  ..set_value..dic
-00000b80: 7472 3200 0000 da14 696e 6974 5f66 726f  tr2.....init_fro
+00000b80: 7472 3100 0000 da14 696e 6974 5f66 726f  tr1.....init_fro
 00000b90: 6d5f 7079 5f6f 626a 6563 7473 da09 5f73  m_py_objects.._s
 00000ba0: 6574 5f69 7465 6dda 134e 6f74 496d 706c  et_item..NotImpl
-00000bb0: 656d 656e 7465 6445 7272 6f72 290b 7244  ementedError).rD
-00000bc0: 0000 0072 3e00 0000 724b 0000 0072 4e00  ...r>...rK...rN.
-00000bd0: 0000 724c 0000 0072 3600 0000 7237 0000  ..rL...r6...r7..
+00000bb0: 656d 656e 7465 6445 7272 6f72 290b 7243  ementedError).rC
+00000bc0: 0000 0072 3d00 0000 724a 0000 0072 4d00  ...r=...rJ...rM.
+00000bd0: 0000 724b 0000 0072 3500 0000 7236 0000  ..rK...r5...r6..
 00000be0: 00da 0964 696d 656e 7369 6f6e 5a0f 6469  ...dimensionZ.di
 00000bf0: 6d65 6e73 696f 6e73 5f64 6963 745a 0d63  mensions_dictZ.c
 00000c00: 6f6d 6d65 6e74 735f 6469 6374 da03 6f62  omments_dict..ob
-00000c10: 6a72 2100 0000 7221 0000 0072 2200 0000  jr!...r!...r"...
-00000c20: 7255 0000 0056 0000 0073 3600 0000 0807  rU...V...s6.....
+00000c10: 6a72 2000 0000 7220 0000 0072 2100 0000  jr ...r ...r!...
+00000c20: 7254 0000 0056 0000 0073 3600 0000 0807  rT...V...s6.....
 00000c30: 0401 0801 0401 1001 1201 0e01 0e01 0801  ................
 00000c40: 0e01 0c02 0a01 0801 1001 0a01 0c01 0c01  ................
 00000c50: 0e01 0401 0201 0201 0201 0201 06fc 0e06  ................
 00000c60: 0c02 04e9 7a23 4e6f 6465 4c69 6b65 5079  ....z#NodeLikePy
 00000c70: 4469 6374 2e69 6e69 745f 6672 6f6d 5f70  Dict.init_from_p
 00000c80: 795f 6f62 6a65 6374 7363 0300 0000 0000  y_objectsc......
 00000c90: 0000 0000 0000 0600 0000 0600 0000 4300  ..............C.
@@ -220,114 +220,114 @@
 00000db0: 0564 0e8d 037d 026e 0c74 007c 0274 1183  .d...}.n.t.|.t..
 00000dc0: 0272 8f6e 0674 1074 057c 0283 0183 0182  .r.n.t.t.|......
 00000dd0: 017c 00a0 127c 017c 02a1 0201 0064 0053  .|...|.|.....d.S
 00000de0: 0029 0f4e 7201 0000 0063 0100 0000 0000  .).Nr....c......
 00000df0: 0000 0000 0000 0200 0000 0400 0000 7300  ..............s.
 00000e00: 0000 f31a 0000 0081 007c 005d 087d 0174  .........|.].}.t
 00000e10: 007c 0174 0183 0256 0001 0071 0264 0053  .|.t...V...q.d.S
-00000e20: 0072 3000 0000 2902 7231 0000 0072 0500  .r0...).r1...r..
-00000e30: 0000 2902 7235 0000 00da 016e 7221 0000  ..).r5.....nr!..
-00000e40: 0072 2100 0000 7222 0000 0072 3800 0000  .r!...r"...r8...
+00000e20: 0072 2f00 0000 2902 7230 0000 0072 0500  .r/...).r0...r..
+00000e30: 0000 2902 7234 0000 00da 016e 7220 0000  ..).r4.....nr ..
+00000e40: 0072 2000 0000 7221 0000 0072 3700 0000  .r ...r!...r7...
 00000e50: 8000 0000 f304 0000 0002 8018 007a 2b4e  .............z+N
 00000e60: 6f64 654c 696b 6550 7944 6963 742e 7365  odeLikePyDict.se
 00000e70: 745f 6368 696c 642e 3c6c 6f63 616c 733e  t_child.<locals>
-00000e80: 2e3c 6765 6e65 7870 723e a901 724d 0000  .<genexpr>..rM..
-00000e90: 00e9 0200 0000 720f 0000 00e9 0900 0000  ......r.........
+00000e80: 2e3c 6765 6e65 7870 723e a901 724c 0000  .<genexpr>..rL..
+00000e90: 00e9 0200 0000 720e 0000 00e9 0900 0000  ......r.........
 00000ea0: da06 7465 6e73 6f72 e903 0000 005a 0676  ..tensor.....Z.v
 00000eb0: 6563 746f 7263 0100 0000 0000 0000 0000  ectorc..........
 00000ec0: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
 00000ed0: 0000 0067 007c 005d 067d 0174 007c 0183  ...g.|.].}.t.|..
-00000ee0: 0191 0271 0253 0072 2100 0000 2901 7233  ...q.S.r!...).r3
-00000ef0: 0000 0029 0272 3500 0000 da08 7365 7175  ...).r5.....sequ
-00000f00: 656e 6365 7221 0000 0072 2100 0000 7222  encer!...r!...r"
+00000ee0: 0191 0271 0253 0072 2000 0000 2901 7232  ...q.S.r ...).r2
+00000ef0: 0000 0029 0272 3400 0000 da08 7365 7175  ...).r4.....sequ
+00000f00: 656e 6365 7220 0000 0072 2000 0000 7221  encer ...r ...r!
 00000f10: 0000 00da 0a3c 6c69 7374 636f 6d70 3e96  .....<listcomp>.
 00000f20: 0000 0073 0200 0000 1400 7a2c 4e6f 6465  ...s......z,Node
 00000f30: 4c69 6b65 5079 4469 6374 2e73 6574 5f63  LikePyDict.set_c
 00000f40: 6869 6c64 2e3c 6c6f 6361 6c73 3e2e 3c6c  hild.<locals>.<l
 00000f50: 6973 7463 6f6d 703e da06 7363 616c 6172  istcomp>..scalar
-00000f60: 2902 724d 0000 00da 0564 7479 7065 2913  ).rM.....dtype).
-00000f70: 7231 0000 0072 5100 0000 da03 616c 6cda  r1...rQ.....all.
-00000f80: 026e 70da 0561 7272 6179 7242 0000 0072  .np..arrayrB...r
-00000f90: 4f00 0000 7205 0000 00da 0c44 696d 656e  O...r......Dimen
-00000fa0: 7369 6f6e 5365 7472 5400 0000 7232 0000  sionSetrT...r2..
-00000fb0: 0072 3300 0000 da07 6e64 6172 7261 79da  .r3.....ndarray.
+00000f60: 2902 724c 0000 00da 0564 7479 7065 2913  ).rL.....dtype).
+00000f70: 7230 0000 0072 5000 0000 da03 616c 6cda  r0...rP.....all.
+00000f80: 026e 70da 0561 7272 6179 7241 0000 0072  .np..arrayrA...r
+00000f90: 4e00 0000 7205 0000 00da 0c44 696d 656e  N...r......Dimen
+00000fa0: 7369 6f6e 5365 7472 5300 0000 7231 0000  sionSetrS...r1..
+00000fb0: 0072 3200 0000 da07 6e64 6172 7261 79da  .r2.....ndarray.
 00000fc0: 0573 6861 7065 da04 6e64 696d da06 746f  .shape..ndim..to
-00000fd0: 6c69 7374 7257 0000 0072 4100 0000 7256  listrW...rA...rV
-00000fe0: 0000 0029 0672 4400 0000 7236 0000 00da  ...).rD...r6....
-00000ff0: 0563 6869 6c64 726b 0000 0072 6c00 0000  .childrk...rl...
-00001000: 7265 0000 0072 2100 0000 7221 0000 0072  re...r!...r!...r
-00001010: 2200 0000 7250 0000 007a 0000 0073 4a00  "...rP...z...sJ.
+00000fd0: 6c69 7374 7256 0000 0072 4000 0000 7255  listrV...r@...rU
+00000fe0: 0000 0029 0672 4300 0000 7235 0000 00da  ...).rC...r5....
+00000ff0: 0563 6869 6c64 726a 0000 0072 6b00 0000  .childrj...rk...
+00001000: 7264 0000 0072 2000 0000 7220 0000 0072  rd...r ...r ...r
+00001010: 2100 0000 724f 0000 007a 0000 0073 4a00  !...rO...z...sJ.
 00001020: 0000 0802 02ff 0202 02fe 0c03 02fd 0604  ................
 00001030: 02fc 1405 02fb 0a07 1602 0201 0a01 0e01  ................
 00001040: 0a01 0e01 0c01 0601 0601 0801 0401 0801  ................
 00001050: 0c01 0601 0c01 0601 0402 1001 0801 0601  ................
 00001060: 0402 1001 0a01 0201 0c02 1001 7a18 4e6f  ............z.No
 00001070: 6465 4c69 6b65 5079 4469 6374 2e73 6574  deLikePyDict.set
 00001080: 5f63 6869 6c64 6304 0000 0000 0000 0000  _childc.........
 00001090: 0000 0004 0000 0005 0000 0043 0000 0073  ...........C...s
 000010a0: 3000 0000 7400 7c02 7401 8302 7309 7c03  0...t.|.t...s.|.
 000010b0: 6400 7501 7210 7402 7c02 7c01 7c03 6401  d.u.r.t.|.|.|.d.
 000010c0: 8d03 7d02 7c00 a003 7c01 7c02 a102 0100  ..}.|...|.|.....
-000010d0: 6400 5300 2902 4e29 0172 5800 0000 2904  d.S.).N).rX...).
-000010e0: 7231 0000 0072 0500 0000 da05 5661 6c75  r1...r......Valu
-000010f0: 6572 5600 0000 2904 7244 0000 0072 4d00  erV...).rD...rM.
-00001100: 0000 7237 0000 0072 5800 0000 7221 0000  ..r7...rX...r!..
-00001110: 0072 2100 0000 7222 0000 0072 5300 0000  .r!...r"...rS...
+000010d0: 6400 5300 2902 4e29 0172 5700 0000 2904  d.S.).N).rW...).
+000010e0: 7230 0000 0072 0500 0000 da05 5661 6c75  r0...r......Valu
+000010f0: 6572 5500 0000 2904 7243 0000 0072 4c00  erU...).rC...rL.
+00001100: 0000 7236 0000 0072 5700 0000 7220 0000  ..r6...rW...r ..
+00001110: 0072 2000 0000 7221 0000 0072 5200 0000  .r ...r!...rR...
 00001120: a200 0000 7306 0000 0012 010e 0110 017a  ....s..........z
 00001130: 184e 6f64 654c 696b 6550 7944 6963 742e  .NodeLikePyDict.
 00001140: 7365 745f 7661 6c75 6563 0300 0000 0000  set_valuec......
 00001150: 0000 0000 0000 0300 0000 0100 0000 4300  ..............C.
 00001160: 0000 7304 0000 0064 0153 0029 027a 0b53  ..s....d.S.).z.S
-00001170: 6574 2061 6e20 6974 656d 4e72 2100 0000  et an itemNr!...
-00001180: a903 7244 0000 0072 3600 0000 7237 0000  ..rD...r6...r7..
-00001190: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
-000011a0: 7256 0000 00a7 0000 0073 0200 0000 0400  rV.......s......
+00001170: 6574 2061 6e20 6974 656d 4e72 2000 0000  et an itemNr ...
+00001180: a903 7243 0000 0072 3500 0000 7236 0000  ..rC...r5...r6..
+00001190: 0072 2000 0000 7220 0000 0072 2100 0000  .r ...r ...r!...
+000011a0: 7255 0000 00a7 0000 0073 0200 0000 0400  rU.......s......
 000011b0: 7a18 4e6f 6465 4c69 6b65 5079 4469 6374  z.NodeLikePyDict
 000011c0: 2e5f 7365 745f 6974 656d 2903 4e46 4e72  ._set_item).NFNr
-000011d0: 3000 0000 290a 7247 0000 0072 4800 0000  0...).rG...rH...
-000011e0: 7249 0000 0072 5400 0000 7207 0000 0072  rI...rT...r....r
-000011f0: 5500 0000 7250 0000 0072 5300 0000 7203  U...rP...rS...r.
-00001200: 0000 0072 5600 0000 7221 0000 0072 2100  ...rV...r!...r!.
-00001210: 0000 7221 0000 0072 2200 0000 724a 0000  ..r!...r"...rJ..
+000011d0: 2f00 0000 290a 7246 0000 0072 4700 0000  /...).rF...rG...
+000011e0: 7248 0000 0072 5300 0000 7207 0000 0072  rH...rS...r....r
+000011f0: 5400 0000 724f 0000 0072 5200 0000 7203  T...rO...rR...r.
+00001200: 0000 0072 5500 0000 7220 0000 0072 2000  ...rU...r ...r .
+00001210: 0000 7220 0000 0072 2100 0000 7249 0000  ..r ...r!...rI..
 00001220: 0055 0000 0073 1e00 0000 0800 0204 0201  .U...s..........
 00001230: 0201 04fb 0202 02fe 0603 02fd 0605 0afb  ................
-00001240: 0824 0a28 0205 0e01 724a 0000 0063 0000  .$.(....rJ...c..
+00001240: 0824 0a28 0205 0e01 7249 0000 0063 0000  .$.(....rI...c..
 00001250: 0000 0000 0000 0000 0000 0000 0000 0300  ................
 00001260: 0000 4000 0000 7346 0000 0065 005a 0164  ..@...sF...e.Z.d
 00001270: 005a 0264 1064 0264 0384 015a 0364 0464  .Z.d.d.d...Z.d.d
 00001280: 0584 005a 0464 0664 0784 005a 0564 0864  ...Z.d.d...Z.d.d
 00001290: 0984 005a 0664 0a64 0b84 005a 0764 0c64  ...Z.d.d...Z.d.d
 000012a0: 0d84 005a 0864 0e64 0f84 005a 0964 0153  ...Z.d.d...Z.d.S
 000012b0: 0029 11da 0d46 6f61 6d49 6e70 7574 4669  .)...FoamInputFi
 000012c0: 6c65 4e63 0500 0000 0000 0000 0000 0000  leNc............
 000012d0: 0500 0000 0200 0000 4300 0000 732e 0000  ........C...s...
 000012e0: 007c 017c 005f 007c 0264 0075 0072 0969  .|.|._.|.d.u.r.i
 000012f0: 007d 027c 027c 005f 017c 037c 005f 027c  .}.|.|._.|.|._.|
 00001300: 047c 005f 0364 007c 005f 0464 0053 0072  .|._.d.|._.d.S.r
-00001310: 3000 0000 2905 da04 696e 666f da08 6368  0...)...info..ch
-00001320: 696c 6472 656e da06 6865 6164 6572 724c  ildren..headerrL
-00001330: 0000 00da 0470 6174 6829 0572 4400 0000  .....path).rD...
-00001340: 7272 0000 0072 7300 0000 7274 0000 0072  rr...rs...rt...r
-00001350: 4c00 0000 7221 0000 0072 2100 0000 7222  L...r!...r!...r"
+00001310: 2f00 0000 2905 da04 696e 666f da08 6368  /...)...info..ch
+00001320: 696c 6472 656e da06 6865 6164 6572 724b  ildren..headerrK
+00001330: 0000 00da 0470 6174 6829 0572 4300 0000  .....path).rC...
+00001340: 7271 0000 0072 7200 0000 7273 0000 0072  rq...rr...rs...r
+00001350: 4b00 0000 7220 0000 0072 2000 0000 7221  K...r ...r ...r!
 00001360: 0000 00da 085f 5f69 6e69 745f 5fad 0000  .....__init__...
 00001370: 0073 0e00 0000 0601 0801 0401 0601 0601  .s..............
 00001380: 0601 0a01 7a16 466f 616d 496e 7075 7446  ....z.FoamInputF
 00001390: 696c 652e 5f5f 696e 6974 5f5f 6301 0000  ile.__init__c...
 000013a0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
 000013b0: 0043 0000 0073 4200 0000 6401 6701 7d01  .C...sB...d.g.}.
 000013c0: 7c00 6a00 6400 7501 7212 7c01 a001 6402  |.j.d.u.r.|...d.
 000013d0: 7c00 6a00 9b00 6403 9d03 a101 0100 7c01  |.j...d.......|.
 000013e0: a001 6404 7c00 6a02 9b00 6405 9d03 a101  ..d.|.j...d.....
 000013f0: 0100 6406 a003 7c01 a101 5300 2907 4e7a  ..d...|...S.).Nz
 00001400: 0b49 6e70 7574 4669 6c65 280a 7a05 696e  .InputFile(.z.in
 00001410: 666f 3d7a 022c 0a7a 0963 6869 6c64 7265  fo=z.,.z.childre
-00001420: 6e3d 7a02 0a29 7210 0000 0029 0472 7200  n=z..)r....).rr.
-00001430: 0000 7227 0000 0072 7300 0000 7228 0000  ..r'...rs...r(..
-00001440: 0029 0272 4400 0000 da03 746d 7072 2100  .).rD.....tmpr!.
-00001450: 0000 7221 0000 0072 2200 0000 da08 5f5f  ..r!...r".....__
+00001420: 6e3d 7a02 0a29 720f 0000 0029 0472 7100  n=z..)r....).rq.
+00001430: 0000 7226 0000 0072 7200 0000 7227 0000  ..r&...rr...r'..
+00001440: 0029 0272 4300 0000 da03 746d 7072 2000  .).rC.....tmpr .
+00001450: 0000 7220 0000 0072 2100 0000 da08 5f5f  ..r ...r!.....__
 00001460: 7265 7072 5f5f b600 0000 730a 0000 0006  repr__....s.....
 00001470: 010a 0114 0114 010a 017a 1646 6f61 6d49  .........z.FoamI
 00001480: 6e70 7574 4669 6c65 2e5f 5f72 6570 725f  nputFile.__repr_
 00001490: 5f63 0100 0000 0000 0000 0000 0000 0b00  _c..............
 000014a0: 0000 0800 0000 4300 0000 73a2 0100 0067  ......C...s....g
 000014b0: 007d 017c 006a 0064 0075 0172 3664 0167  .}.|.j.d.u.r6d.g
 000014c0: 017d 027c 006a 00a0 01a1 0044 005d 195c  .}.|.j.....D.].\
@@ -353,697 +353,691 @@
 00001600: 0964 0717 007c 0717 007d 077c 01a0 037c  .d...|...}.|...|
 00001610: 07a1 0101 0071 4264 10a0 047c 01a1 017d  .....qBd...|...}
 00001620: 0a7c 006a 1064 0075 0172 c57c 006a 1064  .|.j.d.u.r.|.j.d
 00001630: 0717 007c 0a17 007d 0a7c 0a64 1119 0064  ...|...}.|.d...d
 00001640: 076b 0372 cf7c 0a64 0737 007d 0a7c 0a53  .k.r.|.d.7.}.|.S
 00001650: 0029 124e 7a0a 466f 616d 4669 6c65 0a7b  .).Nz.FoamFile.{
 00001660: e90c 0000 00fa 0120 fa04 2020 2020 fa01  ....... ..    ..
-00001670: 3bda 017d da01 0ae9 0e00 0000 2901 723f  ;..}........).r?
+00001670: 3bda 017d da01 0ae9 0e00 0000 2901 723e  ;..}........).r>
 00001680: 0000 00da 0464 756d 70da 1764 756d 705f  .....dump..dump_
 00001690: 7769 7468 6f75 745f 6173 7369 676e 6d65  without_assignme
-000016a0: 6e74 7210 0000 0072 5e00 0000 7a03 2f2f  ntr....r^...z.//
-000016b0: 207a 040a 2f2f 207a 020a 0a72 1400 0000   z..// z...r....
-000016c0: 2911 7272 0000 0072 3c00 0000 7234 0000  ).rr...r<...r4..
-000016d0: 0072 2700 0000 7228 0000 0072 4000 0000  .r'...r(...r@...
-000016e0: 7273 0000 00da 0768 6173 6174 7472 7280  rs.....hasattrr.
-000016f0: 0000 0072 3100 0000 7233 0000 0072 8100  ...r1...r3...r..
-00001700: 0000 723b 0000 0072 4c00 0000 724f 0000  ..r;...rL...rO..
-00001710: 00da 0772 6570 6c61 6365 7274 0000 0029  ...replacert...)
-00001720: 0b72 4400 0000 7277 0000 005a 0474 6d70  .rD...rw...Z.tmp
-00001730: 3172 3600 0000 da04 6e6f 6465 720a 0000  1r6.....noder...
+000016a0: 6e74 720f 0000 0072 5d00 0000 7a03 2f2f  ntr....r]...z.//
+000016b0: 207a 040a 2f2f 207a 020a 0a72 1300 0000   z..// z...r....
+000016c0: 2911 7271 0000 0072 3b00 0000 7233 0000  ).rq...r;...r3..
+000016d0: 0072 2600 0000 7227 0000 0072 3f00 0000  .r&...r'...r?...
+000016e0: 7272 0000 00da 0768 6173 6174 7472 727f  rr.....hasattrr.
+000016f0: 0000 0072 3000 0000 7232 0000 0072 8000  ...r0...r2...r..
+00001700: 0000 723a 0000 0072 4b00 0000 724e 0000  ..r:...rK...rN..
+00001710: 00da 0772 6570 6c61 6365 7273 0000 0029  ...replacers...)
+00001720: 0b72 4300 0000 7276 0000 005a 0474 6d70  .rC...rv...Z.tmp
+00001730: 3172 3500 0000 da04 6e6f 6465 720a 0000  1r5.....noder...
 00001740: 00da 0a6e 756d 5f73 7061 6365 73da 0963  ...num_spaces..c
 00001750: 6f64 655f 6e6f 6465 5a0b 6e6f 6465 5f64  ode_nodeZ.node_d
-00001760: 756d 7065 64da 0763 6f6d 6d65 6e74 721e  umped..commentr.
-00001770: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
-00001780: 0000 7280 0000 00bd 0000 0073 4800 0000  ..r........sH...
+00001760: 756d 7065 64da 0763 6f6d 6d65 6e74 721d  umped..commentr.
+00001770: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
+00001780: 0000 727f 0000 00bd 0000 0073 4800 0000  ..r........sH...
 00001790: 0401 0a01 0601 1201 1001 1c01 0a01 1001  ................
 000017a0: 0e02 1201 0a01 0801 1202 0801 0280 0801  ................
 000017b0: 0801 0a02 0a01 0402 0801 0601 1602 1201  ................
 000017c0: 1401 0a01 0a01 1001 0c01 0c01 0a01 0a01  ................
 000017d0: 0e01 0c01 0801 0401 7a12 466f 616d 496e  ........z.FoamIn
 000017e0: 7075 7446 696c 652e 6475 6d70 6301 0000  putFile.dumpc...
 000017f0: 0000 0000 0000 0000 0002 0000 0008 0000  ................
 00001800: 0043 0000 0073 5200 0000 7c00 6a00 6400  .C...sR...|.j.d.
 00001810: 7500 7209 7401 6401 8301 8201 7402 7c00  u.r.t.d.....t.|.
 00001820: 6a00 6402 8302 8f10 7d01 7c01 a003 7c00  j.d.....}.|...|.
 00001830: a004 a100 a101 0100 5700 6400 0400 0400  ........W.d.....
 00001840: 8303 0100 6400 5300 3100 7322 7701 0100  ....d.S.1.s"w...
 00001850: 0100 0100 5900 0100 6400 5300 2903 4e7a  ....Y...d.S.).Nz
 00001860: 1173 656c 662e 7061 7468 2069 7320 4e6f  .self.path is No
-00001870: 6e65 da01 7729 0572 7500 0000 723d 0000  ne..w).ru...r=..
-00001880: 00da 046f 7065 6eda 0577 7269 7465 7280  ...open..writer.
-00001890: 0000 0029 0272 4400 0000 da04 6669 6c65  ...).rD.....file
-000018a0: 7221 0000 0072 2100 0000 7222 0000 00da  r!...r!...r"....
+00001870: 6e65 da01 7729 0572 7400 0000 723c 0000  ne..w).rt...r<..
+00001880: 00da 046f 7065 6eda 0577 7269 7465 727f  ...open..writer.
+00001890: 0000 0029 0272 4300 0000 da04 6669 6c65  ...).rC.....file
+000018a0: 7220 0000 0072 2000 0000 7221 0000 00da  r ...r ...r!....
 000018b0: 096f 7665 7277 7269 7465 e700 0000 730a  .overwrite....s.
 000018c0: 0000 000a 0108 010e 0110 0122 ff7a 1746  ...........".z.F
 000018d0: 6f61 6d49 6e70 7574 4669 6c65 2e6f 7665  oamInputFile.ove
 000018e0: 7277 7269 7465 6303 0000 0000 0000 0000  rwritec.........
 000018f0: 0000 0003 0000 0003 0000 0043 0000 00f3  ...........C....
 00001900: 0e00 0000 7c02 7c00 6a00 7c01 3c00 6400  ....|.|.j.|.<.d.
-00001910: 5300 7230 0000 00a9 0172 7300 0000 7270  S.r0.....rs...rp
-00001920: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
-00001930: 0000 7256 0000 00ed 0000 00f3 0200 0000  ..rV............
+00001910: 5300 722f 0000 00a9 0172 7200 0000 726f  S.r/.....rr...ro
+00001920: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
+00001930: 0000 7255 0000 00ed 0000 00f3 0200 0000  ..rU............
 00001940: 0e01 7a17 466f 616d 496e 7075 7446 696c  ..z.FoamInputFil
 00001950: 652e 5f73 6574 5f69 7465 6d63 0300 0000  e._set_itemc....
 00001960: 0000 0000 0000 0000 0300 0000 0300 0000  ................
-00001970: 4300 0000 728d 0000 0072 3000 0000 728e  C...r....r0...r.
-00001980: 0000 0029 0372 4400 0000 7236 0000 00da  ...).rD...r6....
-00001990: 0469 7465 6d72 2100 0000 7221 0000 0072  .itemr!...r!...r
-000019a0: 2200 0000 da0b 5f5f 7365 7469 7465 6d5f  ".....__setitem_
-000019b0: 5ff0 0000 0072 8f00 0000 7a19 466f 616d  _....r....z.Foam
+00001970: 4300 0000 728c 0000 0072 2f00 0000 728d  C...r....r/...r.
+00001980: 0000 0029 0372 4300 0000 7235 0000 00da  ...).rC...r5....
+00001990: 0469 7465 6d72 2000 0000 7220 0000 0072  .itemr ...r ...r
+000019a0: 2100 0000 da0b 5f5f 7365 7469 7465 6d5f  !.....__setitem_
+000019b0: 5ff0 0000 0072 8e00 0000 7a19 466f 616d  _....r....z.Foam
 000019c0: 496e 7075 7446 696c 652e 5f5f 7365 7469  InputFile.__seti
 000019d0: 7465 6d5f 5f63 0200 0000 0000 0000 0000  tem__c..........
 000019e0: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
-000019f0: 0000 007c 006a 007c 0119 0053 0072 3000  ...|.j.|...S.r0.
-00001a00: 0000 728e 0000 0029 0272 4400 0000 7236  ..r....).rD...r6
-00001a10: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
+000019f0: 0000 007c 006a 007c 0119 0053 0072 2f00  ...|.j.|...S.r/.
+00001a00: 0000 728d 0000 0029 0272 4300 0000 7235  ..r....).rC...r5
+00001a10: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
 00001a20: 0000 da0b 5f5f 6765 7469 7465 6d5f 5ff3  ....__getitem__.
 00001a30: 0000 00f3 0200 0000 0a01 7a19 466f 616d  ..........z.Foam
 00001a40: 496e 7075 7446 696c 652e 5f5f 6765 7469  InputFile.__geti
-00001a50: 7465 6d5f 5fa9 034e 4e4e 290a 7247 0000  tem__..NNN).rG..
-00001a60: 0072 4800 0000 7249 0000 0072 7600 0000  .rH...rI...rv...
-00001a70: 7278 0000 0072 8000 0000 728c 0000 0072  rx...r....r....r
-00001a80: 5600 0000 7291 0000 0072 9200 0000 7221  V...r....r....r!
-00001a90: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
-00001aa0: 0000 7271 0000 00ac 0000 0073 1000 0000  ..rq.......s....
+00001a50: 7465 6d5f 5fa9 034e 4e4e 290a 7246 0000  tem__..NNN).rF..
+00001a60: 0072 4700 0000 7248 0000 0072 7500 0000  .rG...rH...ru...
+00001a70: 7277 0000 0072 7f00 0000 728b 0000 0072  rw...r....r....r
+00001a80: 5500 0000 7290 0000 0072 9100 0000 7220  U...r....r....r 
+00001a90: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
+00001aa0: 0000 7270 0000 00ac 0000 0073 1000 0000  ..rp.......s....
 00001ab0: 0800 0a01 0809 0807 082a 0806 0803 0c03  .........*......
-00001ac0: 7271 0000 0063 0000 0000 0000 0000 0000  rq...c..........
+00001ac0: 7270 0000 0063 0000 0000 0000 0000 0000  rp...c..........
 00001ad0: 0000 0000 0000 0300 0000 4000 0000 7328  ..........@...s(
 00001ae0: 0000 0065 005a 0164 005a 0255 0065 0365  ...e.Z.d.Z.U.e.e
 00001af0: 0464 013c 0065 0565 0464 023c 0064 0764  .d.<.e.e.d.<.d.d
 00001b00: 0464 0584 015a 0664 0653 0029 08da 0a41  .d...Z.d.S.)...A
-00001b10: 7373 6967 6e6d 656e 7472 4d00 0000 7237  ssignmentrM...r7
+00001b10: 7373 6967 6e6d 656e 7472 4c00 0000 7236  ssignmentrL...r6
 00001b20: 0000 0072 0100 0000 6302 0000 0000 0000  ...r....c.......
-00001b30: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
-00001b40: 0073 3400 0000 7400 7c00 6a01 6401 8302  .s4...t.|.j.d...
-00001b50: 720c 7c00 6a01 a002 7c01 a101 5300 7c01  r.|.j...|...S.|.
-00001b60: 6402 1400 7c00 6a03 9b00 6403 7c00 6a01  d...|.j...d.|.j.
-00001b70: 9b00 6404 9d04 1700 5300 a905 4e72 8000  ..d.....S...Nr..
-00001b80: 0000 727a 0000 00fa 0220 2072 7c00 0000  ..rz.....  r|...
-00001b90: 2904 7282 0000 0072 3700 0000 7280 0000  ).r....r7...r...
-00001ba0: 0072 4d00 0000 a902 7244 0000 00da 0669  .rM.....rD.....i
-00001bb0: 6e64 656e 7472 2100 0000 7221 0000 0072  ndentr!...r!...r
-00001bc0: 2200 0000 7280 0000 00fc 0000 0073 0600  "...r........s..
-00001bd0: 0000 0c01 0c01 1c02 7a0f 4173 7369 676e  ........z.Assign
-00001be0: 6d65 6e74 2e64 756d 704e a901 7201 0000  ment.dumpN..r...
-00001bf0: 0029 0772 4700 0000 7248 0000 0072 4900  .).rG...rH...rI.
-00001c00: 0000 724f 0000 00da 0f5f 5f61 6e6e 6f74  ..rO.....__annot
-00001c10: 6174 696f 6e73 5f5f da06 6f62 6a65 6374  ations__..object
-00001c20: 7280 0000 0072 2100 0000 7221 0000 0072  r....r!...r!...r
-00001c30: 2100 0000 7222 0000 0072 9500 0000 f700  !...r"...r......
-00001c40: 0000 7308 0000 000a 0008 0208 010e 0272  ..s............r
-00001c50: 9500 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00001c60: 0000 0000 0003 0000 0000 0000 0073 2600  .............s&.
-00001c70: 0000 6500 5a01 6400 5a02 8700 6601 6401  ..e.Z.d.Z...f.d.
-00001c80: 6402 8408 5a03 6406 6404 6405 8401 5a04  d...Z.d.d.d...Z.
-00001c90: 8700 0400 5a05 5300 2907 da12 5661 7269  ....Z.S.)...Vari
-00001ca0: 6162 6c65 4173 7369 676e 6d65 6e74 6301  ableAssignmentc.
-00001cb0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-00001cc0: 0000 0003 0000 0073 0e00 0000 7400 8300  .......s....t...
-00001cd0: a001 a100 7d01 7c01 5300 7230 0000 00a9  ....}.|.S.r0....
-00001ce0: 02da 0573 7570 6572 7278 0000 0029 0272  ...superrx...).r
-00001cf0: 4400 0000 720a 0000 00a9 01da 095f 5f63  D...r........__c
-00001d00: 6c61 7373 5f5f 7221 0000 0072 2200 0000  lass__r!...r"...
-00001d10: 7278 0000 0004 0100 0073 0400 0000 0a01  rx.......s......
-00001d20: 0401 7a1b 5661 7269 6162 6c65 4173 7369  ..z.VariableAssi
-00001d30: 676e 6d65 6e74 2e5f 5f72 6570 725f 5f72  gnment.__repr__r
-00001d40: 0100 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00001d50: 0002 0000 0006 0000 0043 0000 0073 4a00  .........C...sJ.
-00001d60: 0000 7400 7c00 6a01 6401 8302 7217 7c01  ..t.|.j.d...r.|.
-00001d70: 6402 1400 7c00 6a02 9b00 6403 7c00 6a01  d...|.j...d.|.j.
-00001d80: a003 7c01 a101 9b00 6404 9d04 1700 5300  ..|.....d.....S.
-00001d90: 7c01 6402 1400 7c00 6a02 9b00 6403 7c00  |.d...|.j...d.|.
-00001da0: 6a01 9b00 6404 9d04 1700 5300 7296 0000  j...d.....S.r...
-00001db0: 0029 0472 8200 0000 7237 0000 0072 4d00  .).r....r7...rM.
-00001dc0: 0000 7280 0000 0072 9800 0000 7221 0000  ..r....r....r!..
-00001dd0: 0072 2100 0000 7222 0000 0072 8000 0000  .r!...r"...r....
-00001de0: 0801 0000 7306 0000 000c 0122 011c 027a  ....s......"...z
-00001df0: 1756 6172 6961 626c 6541 7373 6967 6e6d  .VariableAssignm
-00001e00: 656e 742e 6475 6d70 729a 0000 0029 0672  ent.dumpr....).r
-00001e10: 4700 0000 7248 0000 0072 4900 0000 7278  G...rH...rI...rx
-00001e20: 0000 0072 8000 0000 da0d 5f5f 636c 6173  ...r......__clas
-00001e30: 7363 656c 6c5f 5f72 2100 0000 7221 0000  scell__r!...r!..
-00001e40: 0072 a000 0000 7222 0000 0072 9d00 0000  .r....r"...r....
-00001e50: 0301 0000 7306 0000 0008 000c 0112 0472  ....s..........r
-00001e60: 9d00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00001e70: 0000 0000 0003 0000 0040 0000 00f3 2800  .........@....(.
-00001e80: 0000 6500 5a01 6400 5a02 6409 6402 6403  ..e.Z.d.Z.d.d.d.
-00001e90: 8401 5a03 6404 6405 8400 5a04 640a 6407  ..Z.d.d...Z.d.d.
-00001ea0: 6408 8401 5a05 6401 5300 290b 726f 0000  d...Z.d.S.).ro..
-00001eb0: 004e 6304 0000 0000 0000 0000 0000 0004  .Nc.............
-00001ec0: 0000 0004 0000 0043 0000 0073 2c00 0000  .......C...s,...
-00001ed0: 7c01 7c00 5f00 7c02 7c00 5f01 7402 7c03  |.|._.|.|._.t.|.
-00001ee0: 7403 7404 6602 8302 7211 7405 7c03 8301  t.t.f...r.t.|...
-00001ef0: 7d03 7c03 7c00 5f06 6400 5300 7230 0000  }.|.|._.d.S.r0..
-00001f00: 0029 0772 3700 0000 724d 0000 0072 3100  .).r7...rM...r1.
-00001f10: 0000 7251 0000 00da 0574 7570 6c65 722e  ..rQ.....tupler.
-00001f20: 0000 0072 5800 0000 2904 7244 0000 0072  ...rX...).rD...r
-00001f30: 3700 0000 724d 0000 0072 5800 0000 7221  7...rM...rX...r!
-00001f40: 0000 0072 2100 0000 7222 0000 0072 7600  ...r!...r"...rv.
-00001f50: 0000 1101 0000 730a 0000 0006 0106 010e  ......s.........
-00001f60: 0108 010a 017a 0e56 616c 7565 2e5f 5f69  .....z.Value.__i
-00001f70: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
-00001f80: 0000 0100 0000 0700 0000 4300 0000 7394  ..........C...s.
-00001f90: 0000 007c 006a 0064 0075 0172 197c 006a  ...|.j.d.u.r.|.j
-00001fa0: 0164 0075 0172 1964 017c 006a 029b 0064  .d.u.r.d.|.j...d
-00001fb0: 027c 006a 019b 0064 037c 006a 009b 0064  .|.j...d.|.j...d
-00001fc0: 049d 0753 007c 006a 0064 0075 0072 2e7c  ...S.|.j.d.u.r.|
-00001fd0: 006a 0164 0075 0172 2e64 017c 006a 029b  .j.d.u.r.d.|.j..
-00001fe0: 0064 027c 006a 019b 0064 049d 0553 007c  .d.|.j...d...S.|
-00001ff0: 006a 0064 0075 0172 437c 006a 0164 0075  .j.d.u.rC|.j.d.u
-00002000: 0072 4364 017c 006a 029b 0064 057c 006a  .rCd.|.j...d.|.j
-00002010: 009b 0064 049d 0553 0064 017c 006a 029b  ...d...S.d.|.j..
-00002020: 0064 069d 0353 0029 074e 7a06 5661 6c75  .d...S.).Nz.Valu
-00002030: 6528 7a08 2c20 6e61 6d65 3d22 7a0e 222c  e(z., name="z.",
-00002040: 2064 696d 656e 7369 6f6e 3d22 7a02 2229   dimension="z.")
-00002050: 7a0d 2c20 6469 6d65 6e73 696f 6e3d 22fa  z., dimension=".
-00002060: 0129 2903 7258 0000 0072 4d00 0000 7237  .)).rX...rM...r7
-00002070: 0000 00a9 0172 4400 0000 7221 0000 0072  .....rD...r!...r
-00002080: 2100 0000 7222 0000 0072 7800 0000 1801  !...r"...rx.....
-00002090: 0000 730e 0000 0014 011e 0114 0116 0114  ..s.............
-000020a0: 0116 010e 027a 0e56 616c 7565 2e5f 5f72  .....z.Value.__r
-000020b0: 6570 725f 5f72 0100 0000 6302 0000 0000  epr__r....c.....
-000020c0: 0000 0000 0000 0005 0000 0005 0000 0043  ...............C
-000020d0: 0000 0073 ce00 0000 7c00 6a00 6400 7501  ...s....|.j.d.u.
-000020e0: 7214 7401 7c00 6a00 8301 7d02 6401 a002  r.t.|.j...}.d...
-000020f0: 6402 6403 8400 7c02 4400 8301 a101 7d03  d.d...|.D.....}.
-00002100: 7403 7c00 6a04 7405 8302 7226 7406 7c00  t.|.j.t...r&t.|.
-00002110: 6a04 6404 8302 7226 7c00 6a04 a007 a100  j.d...r&|.j.....
-00002120: 7d04 6e05 7408 7c00 6a04 8301 7d04 7c00  }.n.t.|.j...}.|.
-00002130: 6a00 6400 7501 7240 7c00 6a09 6400 7501  j.d.u.r@|.j.d.u.
-00002140: 7240 7c00 6a09 9b00 6405 7c03 9b00 6406  r@|.j...d.|...d.
-00002150: 7c04 9b00 9d05 5300 7c00 6a00 6400 7500  |.....S.|.j.d.u.
-00002160: 7252 7c00 6a09 6400 7501 7252 7c00 6a09  rR|.j.d.u.rR|.j.
-00002170: 9b00 6401 7c04 9b00 9d03 5300 7c00 6a00  ..d.|.....S.|.j.
-00002180: 6400 7501 7264 7c00 6a09 6400 7500 7264  d.u.rd|.j.d.u.rd
-00002190: 6407 7c03 9b00 6406 7c04 9b00 9d04 5300  d.|...d.|.....S.
-000021a0: 7c04 9b00 5300 2908 4e72 7a00 0000 6301  |...S.).Nrz...c.
-000021b0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-000021c0: 0000 0073 0000 00f3 1800 0000 8100 7c00  ...s..........|.
-000021d0: 5d07 7d01 7400 7c01 8301 5600 0100 7102  ].}.t.|...V...q.
-000021e0: 6400 5300 7230 0000 00a9 0172 4f00 0000  d.S.r0.....rO...
-000021f0: a902 7235 0000 00da 066e 756d 6265 7272  ..r5.....numberr
-00002200: 2100 0000 7221 0000 0072 2200 0000 7238  !...r!...r"...r8
-00002210: 0000 0025 0100 00f3 0400 0000 0280 1600  ...%............
-00002220: 7a30 5661 6c75 652e 6475 6d70 5f77 6974  z0Value.dump_wit
-00002230: 686f 7574 5f61 7373 6967 6e6d 656e 742e  hout_assignment.
-00002240: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
-00002250: 723e 7280 0000 007a 0220 5b7a 025d 20fa  r>r....z. [z.] .
-00002260: 015b 290a 7258 0000 0072 2300 0000 7228  .[).rX...r#...r(
-00002270: 0000 0072 3100 0000 7237 0000 0072 4100  ...r1...r7...rA.
-00002280: 0000 7282 0000 0072 8000 0000 724f 0000  ..r....r....rO..
-00002290: 0072 4d00 0000 2905 7244 0000 0072 9900  .rM...).rD...r..
-000022a0: 0000 5a0e 6469 6d65 6e73 696f 6e5f 6c69  ..Z.dimension_li
-000022b0: 7374 5a10 6469 6d65 6e73 696f 6e5f 6475  stZ.dimension_du
-000022c0: 6d70 6564 5a0c 7661 6c75 655f 6475 6d70  mpedZ.value_dump
-000022d0: 6564 7221 0000 0072 2100 0000 7222 0000  edr!...r!...r"..
-000022e0: 0072 8100 0000 2201 0000 731a 0000 000a  .r...."...s.....
-000022f0: 010a 0114 0118 020c 010a 0214 0216 0114  ................
-00002300: 0110 0114 0110 0106 027a 1d56 616c 7565  .........z.Value
-00002310: 2e64 756d 705f 7769 7468 6f75 745f 6173  .dump_without_as
-00002320: 7369 676e 6d65 6e74 2902 4e4e 729a 0000  signment).NNr...
-00002330: 0029 0672 4700 0000 7248 0000 0072 4900  .).rG...rH...rI.
-00002340: 0000 7276 0000 0072 7800 0000 7281 0000  ..rv...rx...r...
-00002350: 0072 2100 0000 7221 0000 0072 2100 0000  .r!...r!...r!...
-00002360: 7222 0000 0072 6f00 0000 0f01 0000 7308  r"...ro.......s.
-00002370: 0000 0008 000a 0208 070e 0a72 6f00 0000  ...........ro...
-00002380: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00002390: 0003 0000 0000 0000 0073 2e00 0000 6500  .........s....e.
-000023a0: 5a01 6400 5a02 8700 6601 6401 6402 8408  Z.d.Z...f.d.d...
-000023b0: 5a03 6403 6404 8400 5a04 6408 6406 6407  Z.d.d...Z.d.d.d.
-000023c0: 8401 5a05 8700 0400 5a06 5300 2909 7269  ..Z.....Z.S.).ri
-000023d0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-000023e0: 0200 0000 0300 0000 0300 0000 733c 0000  ............s<..
-000023f0: 0074 007c 0174 0183 0272 0974 027c 0183  .t.|.t...r.t.|..
-00002400: 017d 0174 0364 0164 0284 007c 0144 0083  .}.t.d.d...|.D..
-00002410: 0183 0173 1674 0464 0383 0182 0174 0583  ...s.t.d.....t..
-00002420: 00a0 067c 01a1 0101 0064 0053 0029 044e  ...|.....d.S.).N
-00002430: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00002440: 0004 0000 0073 0000 0072 5a00 0000 7230  .....s...rZ...r0
-00002450: 0000 0029 0272 3100 0000 721a 0000 0029  ...).r1...r....)
-00002460: 0272 3500 0000 da04 656c 656d 7221 0000  .r5.....elemr!..
-00002470: 0072 2100 0000 7222 0000 0072 3800 0000  .r!...r"...r8...
-00002480: 3a01 0000 725c 0000 007a 2844 696d 656e  :...r\...z(Dimen
-00002490: 7369 6f6e 5365 742e 5f5f 696e 6974 5f5f  sionSet.__init__
-000024a0: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
-000024b0: 7072 3e7a 1342 6164 207b 666f 616d 5f75  pr>z.Bad {foam_u
-000024c0: 6e69 7473 203d 207d 2907 7231 0000 0072  nits = }).r1...r
-000024d0: 4f00 0000 7223 0000 0072 6600 0000 723d  O...r#...rf...r=
-000024e0: 0000 0072 9f00 0000 7276 0000 0029 0272  ...r....rv...).r
-000024f0: 4400 0000 722a 0000 0072 a000 0000 7221  D...r*...r....r!
-00002500: 0000 0072 2200 0000 7276 0000 0037 0100  ...r"...rv...7..
-00002510: 0073 0a00 0000 0a01 0801 1201 0801 1001  .s..............
-00002520: 7a15 4469 6d65 6e73 696f 6e53 6574 2e5f  z.DimensionSet._
-00002530: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-00002540: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00002550: 7308 0000 0074 007c 0083 0153 0072 3000  s....t.|...S.r0.
-00002560: 0000 2901 722e 0000 0072 a600 0000 7221  ..).r....r....r!
-00002570: 0000 0072 2100 0000 7222 0000 0072 7800  ...r!...r"...rx.
-00002580: 0000 3e01 0000 f302 0000 0008 017a 1544  ..>..........z.D
-00002590: 696d 656e 7369 6f6e 5365 742e 5f5f 7265  imensionSet.__re
-000025a0: 7072 5f5f 7201 0000 0063 0200 0000 0000  pr__r....c......
-000025b0: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
-000025c0: 0000 731c 0000 0064 0164 02a0 0064 0364  ..s....d.d...d.d
-000025d0: 0484 007c 0044 0083 01a1 0117 0064 0517  ...|.D.......d..
-000025e0: 0053 0029 064e 72ac 0000 0072 7a00 0000  .S.).Nr....rz...
-000025f0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00002600: 0003 0000 0073 0000 0072 a700 0000 7230  .....s...r....r0
-00002610: 0000 0072 a800 0000 72a9 0000 0072 2100  ...r....r....r!.
-00002620: 0000 7221 0000 0072 2200 0000 7238 0000  ..r!...r"...r8..
-00002630: 0042 0100 0072 ab00 0000 7a37 4469 6d65  .B...r....z7Dime
-00002640: 6e73 696f 6e53 6574 2e64 756d 705f 7769  nsionSet.dump_wi
-00002650: 7468 6f75 745f 6173 7369 676e 6d65 6e74  thout_assignment
-00002660: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
-00002670: 7072 3efa 015d a901 7228 0000 0072 9800  pr>..]..r(...r..
-00002680: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
-00002690: 0072 8100 0000 4101 0000 f302 0000 001c  .r....A.........
-000026a0: 017a 2444 696d 656e 7369 6f6e 5365 742e  .z$DimensionSet.
-000026b0: 6475 6d70 5f77 6974 686f 7574 5f61 7373  dump_without_ass
-000026c0: 6967 6e6d 656e 7472 9a00 0000 2907 7247  ignmentr....).rG
-000026d0: 0000 0072 4800 0000 7249 0000 0072 7600  ...rH...rI...rv.
-000026e0: 0000 7278 0000 0072 8100 0000 72a2 0000  ..rx...r....r...
-000026f0: 0072 2100 0000 7221 0000 0072 a000 0000  .r!...r!...r....
-00002700: 7222 0000 0072 6900 0000 3601 0000 7308  r"...ri...6...s.
-00002710: 0000 0008 000c 0108 0712 0372 6900 0000  ...........ri...
-00002720: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00002730: 0004 0000 0000 0000 0073 4400 0000 6500  .........sD...e.
-00002740: 5a01 6400 5a02 640d 8700 6601 6402 6403  Z.d.Z.d...f.d.d.
-00002750: 8409 5a03 6404 6405 8400 5a04 8700 6601  ..Z.d.d...Z...f.
-00002760: 6406 6407 8408 5a05 640e 6409 640a 8401  d.d...Z.d.d.d...
-00002770: 5a06 640b 640c 8400 5a07 8700 0400 5a08  Z.d.d...Z.....Z.
-00002780: 5300 290f 7232 0000 004e 6305 0000 0000  S.).r2...Nc.....
-00002790: 0000 0000 0000 0005 0000 0004 0000 0003  ................
-000027a0: 0000 0073 2800 0000 7c02 7c00 5f00 7c03  ...s(...|.|._.|.
-000027b0: 7c00 5f01 7c04 7c00 5f02 7403 8300 6a04  |._.|.|._.t...j.
-000027c0: 6401 6900 7c01 a401 8e01 0100 6400 5300  d.i.|.......d.S.
-000027d0: 2902 4e72 2100 0000 2905 da05 5f6e 616d  ).Nr!...)..._nam
-000027e0: 65da 0a5f 6469 7265 6374 6976 6572 4c00  e.._directiverL.
-000027f0: 0000 729f 0000 0072 7600 0000 2905 7244  ..r....rv...).rD
-00002800: 0000 0072 3e00 0000 724d 0000 00da 0964  ...r>...rM.....d
-00002810: 6972 6563 7469 7665 724c 0000 0072 a000  irectiverL...r..
-00002820: 0000 7221 0000 0072 2200 0000 7276 0000  ..r!...r"...rv..
-00002830: 0046 0100 0073 0800 0000 0601 0601 0601  .F...s..........
-00002840: 1601 7a0d 4469 6374 2e5f 5f69 6e69 745f  ..z.Dict.__init_
-00002850: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
-00002860: 0000 0100 0000 4300 0000 f306 0000 007c  ......C........|
-00002870: 006a 0053 0072 3000 0000 a901 72b2 0000  .j.S.r0.....r...
-00002880: 0072 a600 0000 7221 0000 0072 2100 0000  .r....r!...r!...
-00002890: 7222 0000 00da 0867 6574 5f6e 616d 654c  r".....get_nameL
-000028a0: 0100 00f3 0200 0000 0601 7a0d 4469 6374  ..........z.Dict
-000028b0: 2e67 6574 5f6e 616d 6563 0100 0000 0000  .get_namec......
-000028c0: 0000 0000 0000 0100 0000 0200 0000 0300  ................
-000028d0: 0000 f30a 0000 0074 0083 00a0 01a1 0053  .......t.......S
-000028e0: 0072 3000 0000 729e 0000 0072 a600 0000  .r0...r....r....
-000028f0: 72a0 0000 0072 2100 0000 7222 0000 0072  r....r!...r"...r
-00002900: 7800 0000 4f01 0000 7293 0000 007a 0d44  x...O...r....z.D
-00002910: 6963 742e 5f5f 7265 7072 5f5f 7201 0000  ict.__repr__r...
-00002920: 0063 0200 0000 0000 0000 0000 0000 0b00  .c..............
-00002930: 0000 0900 0000 4300 0000 7372 0100 0067  ......C...sr...g
-00002940: 007d 027c 0164 0114 007d 037c 006a 0064  .}.|.d...}.|.j.d
-00002950: 0075 0172 287c 037c 006a 0017 007d 047c  .u.r(|.|.j...}.|
-00002960: 006a 0164 0075 0172 1c7c 0464 027c 006a  .j.d.u.r.|.d.|.j
-00002970: 0117 0037 007d 047c 02a0 027c 0464 037c  ...7.}.|...|.d.|
-00002980: 039b 009d 0217 0064 0417 00a1 0101 0074  .......d.......t
-00002990: 037c 0083 017d 057c 00a0 04a1 0044 005d  .|...}.|.....D.]
-000029a0: 6f5c 027d 067d 077c 006a 0564 0075 0172  o\.}.}.|.j.d.u.r
-000029b0: 537c 067c 006a 0576 0072 537c 006a 057c  S|.|.j.v.rS|.j.|
-000029c0: 0619 007d 0874 067c 0874 0783 0272 537c  ...}.t.|.t...rS|
-000029d0: 02a0 0264 057c 08a0 0864 0364 06a1 0217  ...d.|...d.d....
-000029e0: 00a1 0101 0074 097c 0764 0783 0272 637c  .....t.|.d...rc|
-000029f0: 02a0 027c 07a0 0a7c 0164 0817 00a1 01a1  ...|...|.d......
-00002a00: 0101 0071 307c 0764 0075 0072 727c 02a0  ...q0|.d.u.rr|..
-00002a10: 027c 0364 097c 069b 009d 0217 00a1 0101  .|.d.|..........
-00002a20: 0071 3074 097c 0764 0a83 0272 7c7c 07a0  .q0t.|.d...r||..
-00002a30: 0ba1 007d 096e 027c 077d 097c 0764 0b6b  ...}.n.|.}.|.d.k
-00002a40: 0272 8564 0b7d 0a6e 0b74 0c64 0c7c 0574  .r.d.}.n.t.d.|.t
-00002a50: 0d7c 0683 0118 0083 0264 0114 007d 0a7c  .|.......d...}.|
-00002a60: 02a0 027c 0364 097c 069b 007c 0a9b 007c  ...|.d.|...|...|
-00002a70: 099b 0064 0d9d 0517 00a1 0101 0071 307c  ...d.........q0|
-00002a80: 02a0 027c 0364 0e17 00a1 0101 0074 067c  ...|.d.......t.|
-00002a90: 0074 0e83 0272 b47c 0264 0f05 0019 0064  .t...r.|.d.....d
-00002aa0: 0d37 0003 003c 0064 03a0 0f7c 02a1 0153  .7...<.d...|...S
-00002ab0: 0029 104e 727a 0000 0072 9700 0000 727e  .).Nrz...r....r~
-00002ac0: 0000 00da 017b 7a07 2020 2020 2f2f 207a  .....{z.    // z
-00002ad0: 080a 2020 2020 2f2f 2072 8000 0000 7239  ..    // r....r9
-00002ae0: 0000 0072 7b00 0000 7281 0000 0072 1000  ...r{...r....r..
-00002af0: 0000 725e 0000 0072 7c00 0000 727d 0000  ..r^...r|...r}..
-00002b00: 0072 1400 0000 2910 72b2 0000 0072 b300  .r....).r....r..
-00002b10: 0000 7227 0000 0072 4000 0000 723c 0000  ..r'...r@...r<..
-00002b20: 0072 4c00 0000 7231 0000 0072 4f00 0000  .rL...r1...rO...
-00002b30: 7283 0000 0072 8200 0000 7280 0000 0072  r....r....r....r
-00002b40: 8100 0000 723b 0000 0072 3400 0000 da0a  ....r;...r4.....
-00002b50: 436f 6465 5374 7265 616d 7228 0000 0029  CodeStreamr(...)
-00002b60: 0b72 4400 0000 7299 0000 0072 7700 0000  .rD...r....rw...
-00002b70: da0b 696e 6465 6e74 6174 696f 6eda 046c  ..indentation..l
-00002b80: 696e 6572 8500 0000 7236 0000 0072 8400  iner....r6...r..
-00002b90: 0000 7287 0000 0072 8600 0000 720a 0000  ..r....r....r...
-00002ba0: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
-00002bb0: 7280 0000 0052 0100 0073 3800 0000 0401  r....R...s8.....
-00002bc0: 0801 0a01 0a01 0a01 0e01 1801 0802 1001  ................
-00002bd0: 1401 0a01 0a01 1601 0a02 1601 0801 1601  ................
-00002be0: 0a02 0a01 0402 0801 0601 1602 2001 0e01  ............ ...
-00002bf0: 0a03 1001 0a02 7a09 4469 6374 2e64 756d  ......z.Dict.dum
-00002c00: 7063 0300 0000 0000 0000 0000 0000 0300  pc..............
-00002c10: 0000 0300 0000 4300 0000 730c 0000 007c  ......C...s....|
-00002c20: 027c 007c 013c 0064 0053 0072 3000 0000  .|.|.<.d.S.r0...
-00002c30: 7221 0000 0072 7000 0000 7221 0000 0072  r!...rp...r!...r
-00002c40: 2100 0000 7222 0000 0072 5600 0000 7801  !...r"...rV...x.
-00002c50: 0000 7302 0000 000c 017a 0e44 6963 742e  ..s......z.Dict.
-00002c60: 5f73 6574 5f69 7465 6d72 9400 0000 729a  _set_itemr....r.
-00002c70: 0000 0029 0972 4700 0000 7248 0000 0072  ...).rG...rH...r
-00002c80: 4900 0000 7276 0000 0072 b700 0000 7278  I...rv...r....rx
-00002c90: 0000 0072 8000 0000 7256 0000 0072 a200  ...r....rV...r..
-00002ca0: 0000 7221 0000 0072 2100 0000 72a0 0000  ..r!...r!...r...
-00002cb0: 0072 2200 0000 7232 0000 0045 0100 0073  .r"...r2...E...s
-00002cc0: 0c00 0000 0800 0e01 0806 0c03 0a03 1026  ...............&
-00002cd0: 7232 0000 0063 0000 0000 0000 0000 0000  r2...c..........
-00002ce0: 0000 0000 0000 0400 0000 0000 0000 735a  ..............sZ
-00002cf0: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
-00002d00: 1287 0066 0164 0364 0484 095a 0464 0564  ...f.d.d...Z.d.d
-00002d10: 0684 005a 0564 0764 0884 005a 0687 0066  ...Z.d.d...Z...f
-00002d20: 0164 0964 0a84 085a 0764 0b64 0c84 005a  .d.d...Z.d.d...Z
-00002d30: 0864 1364 0e64 0f84 015a 0964 1364 1064  .d.d.d...Z.d.d.d
-00002d40: 1184 015a 0a87 0004 005a 0b53 0029 1472  ...Z.....Z.S.).r
-00002d50: 3300 0000 7a1b 5265 7072 6573 656e 7473  3...z.Represents
-00002d60: 2061 6e20 4f70 656e 466f 616d 206c 6973   an OpenFoam lis
-00002d70: 744e 6304 0000 0000 0000 0000 0000 0004  tNc.............
-00002d80: 0000 0003 0000 0003 0000 0073 1c00 0000  ...........s....
-00002d90: 7c02 7c00 5f00 7c03 7c00 5f01 7402 8300  |.|._.|.|._.t...
-00002da0: a003 7c01 a101 0100 6400 5300 7230 0000  ..|.....d.S.r0..
-00002db0: 0029 0472 b200 0000 da06 5f64 7479 7065  .).r......_dtype
-00002dc0: 729f 0000 0072 7600 0000 2904 7244 0000  r....rv...).rD..
-00002dd0: 00da 0869 7465 7261 626c 6572 4d00 0000  ...iterablerM...
-00002de0: 7265 0000 0072 a000 0000 7221 0000 0072  re...r....r!...r
-00002df0: 2200 0000 7276 0000 007f 0100 0073 0600  "...rv.......s..
-00002e00: 0000 0601 0601 1001 7a0d 4c69 7374 2e5f  ........z.List._
-00002e10: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-00002e20: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00002e30: 72b5 0000 0072 3000 0000 72b6 0000 0072  r....r0...r....r
-00002e40: a600 0000 7221 0000 0072 2100 0000 7222  ....r!...r!...r"
-00002e50: 0000 0072 b700 0000 8401 0000 72b8 0000  ...r........r...
-00002e60: 007a 0d4c 6973 742e 6765 745f 6e61 6d65  .z.List.get_name
-00002e70: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00002e80: 0003 0000 0043 0000 0073 4800 0000 7c00  .....C...sH...|.
-00002e90: 6a00 6400 7500 720a 7c01 7c00 5f00 6400  j.d.u.r.|.|._.d.
-00002ea0: 5300 7401 7c00 6a00 7402 8302 7221 7c00  S.t.|.j.t...r!|.
-00002eb0: 6a00 7c01 6b03 721f 7c01 6401 1700 7c00  j.|.k.r.|.d...|.
-00002ec0: 6a00 1700 7c00 5f00 6400 5300 6400 5300  j...|._.d.S.d.S.
-00002ed0: 7403 8300 8201 2902 4e72 7a00 0000 2904  t.....).Nrz...).
-00002ee0: 72b2 0000 0072 3100 0000 724f 0000 00da  r....r1...rO....
-00002ef0: 0c52 756e 7469 6d65 4572 726f 7229 0272  .RuntimeError).r
-00002f00: 4400 0000 724d 0000 0072 2100 0000 7221  D...rM...r!...r!
-00002f10: 0000 0072 2200 0000 da08 6164 645f 6e61  ...r".....add_na
-00002f20: 6d65 8701 0000 730e 0000 000a 010a 010c  me....s.........
-00002f30: 010a 0114 0104 ff06 037a 0d4c 6973 742e  .........z.List.
-00002f40: 6164 645f 6e61 6d65 6301 0000 0000 0000  add_namec.......
-00002f50: 0000 0000 0001 0000 0002 0000 0003 0000  ................
-00002f60: 0072 b900 0000 7230 0000 0072 9e00 0000  .r....r0...r....
-00002f70: 72a6 0000 0072 a000 0000 7221 0000 0072  r....r....r!...r
-00002f80: 2200 0000 7278 0000 0090 0100 0072 9300  "...rx.......r..
-00002f90: 0000 7a0d 4c69 7374 2e5f 5f72 6570 725f  ..z.List.__repr_
-00002fa0: 5f63 0200 0000 0000 0000 0000 0000 0200  _c..............
-00002fb0: 0000 0300 0000 0300 0000 7314 0000 0087  ..........s.....
-00002fc0: 0087 0166 0264 0164 0284 0888 0144 0083  ...f.d.d.....D..
-00002fd0: 0153 0029 034e 6301 0000 0000 0000 0000  .S.).Nc.........
-00002fe0: 0000 0002 0000 0006 0000 0013 0000 0073  ...............s
-00002ff0: 1800 0000 6700 7c00 5d08 7d01 8801 a000  ....g.|.].}.....
-00003000: 7c01 8800 a102 9102 7102 5300 7221 0000  |.......q.S.r!..
-00003010: 00a9 01da 0a5f 6475 6d70 5f69 7465 6d29  ....._dump_item)
-00003020: 0272 3500 0000 7290 0000 00a9 0272 9900  .r5...r......r..
-00003030: 0000 7244 0000 0072 2100 0000 7222 0000  ..rD...r!...r"..
-00003040: 0072 6300 0000 9401 0000 7302 0000 0018  .rc.......s.....
-00003050: 007a 2b4c 6973 742e 5f6d 616b 655f 6c69  .z+List._make_li
-00003060: 7374 5f73 7472 696e 6773 2e3c 6c6f 6361  st_strings.<loca
-00003070: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7221  ls>.<listcomp>r!
-00003080: 0000 0072 9800 0000 7221 0000 0072 c400  ...r....r!...r..
-00003090: 0000 7222 0000 00da 125f 6d61 6b65 5f6c  ..r"....._make_l
-000030a0: 6973 745f 7374 7269 6e67 7393 0100 0073  ist_strings....s
-000030b0: 0200 0000 1401 7a17 4c69 7374 2e5f 6d61  ......z.List._ma
-000030c0: 6b65 5f6c 6973 745f 7374 7269 6e67 7372  ke_list_stringsr
-000030d0: 0100 0000 6303 0000 0000 0000 0000 0000  ....c...........
-000030e0: 0003 0000 0004 0000 0043 0000 0073 3200  .........C...s2.
-000030f0: 0000 7400 7c01 7401 7402 6602 8302 7211  ..t.|.t.t.f...r.
-00003100: 7403 7c01 6401 8302 7211 7c01 a004 7c02  t.|.d...r.|...|.
-00003110: a101 5300 7c02 6402 1400 7405 7c01 8301  ..S.|.d...t.|...
-00003120: 1700 5300 2903 4e72 8000 0000 727a 0000  ..S.).Nr....rz..
-00003130: 0029 0672 3100 0000 7241 0000 0072 9500  .).r1...rA...r..
-00003140: 0000 7282 0000 0072 8000 0000 724f 0000  ..r....r....rO..
-00003150: 0029 0372 4400 0000 7290 0000 0072 9900  .).rD...r....r..
-00003160: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
-00003170: 0072 c300 0000 9601 0000 7306 0000 0018  .r........s.....
-00003180: 010a 0110 027a 0f4c 6973 742e 5f64 756d  .....z.List._dum
-00003190: 705f 6974 656d 6302 0000 0000 0000 0000  p_itemc.........
-000031a0: 0000 000b 0000 0008 0000 0003 0000 0073  ...............s
-000031b0: 7001 0000 6700 7d02 8800 6401 1400 7d03  p...g.}...d...}.
-000031c0: 8801 6a00 6400 7500 721f 7c02 a001 8801  ..j.d.u.r.|.....
-000031d0: 6a02 6402 6403 8d01 a101 0100 7c03 6404  j.d.d.......|.d.
-000031e0: 1700 6401 a003 7c02 a101 1700 6405 1700  ..d...|.....d...
-000031f0: 5300 8801 6a00 7d04 8801 6a04 6400 7501  S...j.}...j.d.u.
-00003200: 7236 7c04 6406 8801 6a04 9b00 6407 7c03  r6|.d...j...d.|.
-00003210: 9b00 7405 8801 8301 9b00 9d05 3700 7d04  ..t.........7.}.
-00003220: 7c02 a006 7c03 7c04 1700 6408 7c03 9b00  |...|.|...d.|...
-00003230: 9d02 1700 6404 1700 a101 0100 6409 640a  ....d.......d.d.
-00003240: 640b 9c02 7d05 8801 6a00 7c05 a007 a100  d...}...j.|.....
-00003250: 7601 725e 7c02 a006 6408 a003 8801 a002  v.r^|...d.......
-00003260: 8800 640c 1700 a101 a101 a101 0100 6e4e  ..d...........nN
-00003270: 8801 72ac 7c05 8801 6a00 1900 7d06 8801  ..r.|...j...}...
-00003280: 6402 1900 7c06 7601 726f 7408 8801 8301  d...|.v.rot.....
-00003290: 8201 8801 6402 1900 7d07 6700 7d08 6400  ....d...}.g.}.d.
-000032a0: 7d09 8801 4400 5d18 7d0a 7c0a 7c07 6b02  }...D.].}.|.|.k.
-000032b0: 728c 7c09 6400 7501 7288 7c08 a006 7c09  r.|.d.u.r.|...|.
-000032c0: a101 0100 7c0a 6701 7d09 7179 7c09 a006  ....|.g.}.qy|...
-000032d0: 7c0a a101 0100 7179 7c08 a006 7c09 a101  |.....qy|...|...
-000032e0: 0100 8701 6601 640d 640e 8408 7c08 4400  ....f.d.d...|.D.
-000032f0: 8301 7d08 7c02 a001 8700 6601 640f 6410  ..}.|.....f.d.d.
-00003300: 8408 7c08 4400 8301 a101 0100 7c02 a006  ..|.D.......|...
-00003310: 7c03 6411 1700 a101 0100 6408 a003 7c02  |.d.......d...|.
-00003320: a101 5300 2912 4e72 7a00 0000 7201 0000  ..S.).Nrz...r...
-00003330: 00a9 0172 9900 0000 fa01 2872 a500 0000  ...r......(r....
-00003340: 7a13 2020 206e 6f6e 756e 6966 6f72 6d20  z.   nonuniform 
-00003350: 4c69 7374 3c7a 023e 0a72 7e00 0000 2901  List<z.>.r~...).
-00003360: da03 6865 7829 055a 0673 706c 696e 65da  ..hex).Z.spline.
-00003370: 0361 7263 5a08 706f 6c79 4c69 6e65 5a07  .arcZ.polyLineZ.
-00003380: 4253 706c 696e 6572 bd00 0000 2902 da06  BSpliner....)...
-00003390: 626c 6f63 6b73 da05 6564 6765 7372 3900  blocks..edgesr9.
-000033a0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-000033b0: 0000 0007 0000 0013 0000 0073 2400 0000  ...........s$...
-000033c0: 6700 7c00 5d0e 7d01 6400 a000 8700 6601  g.|.].}.d.....f.
-000033d0: 6401 6402 8408 7c01 4400 8301 a101 9102  d.d...|.D.......
-000033e0: 7102 5300 2903 727a 0000 0063 0100 0000  q.S.).rz...c....
-000033f0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00003400: 3300 0000 731a 0000 0081 007c 005d 087d  3...s......|.].}
-00003410: 0188 00a0 007c 01a1 0156 0001 0071 0264  .....|...V...q.d
-00003420: 0053 0072 3000 0000 72c2 0000 0029 0272  .S.r0...r....).r
-00003430: 3500 0000 da05 5f69 7465 6d72 a600 0000  5....._itemr....
-00003440: 7221 0000 0072 2200 0000 7238 0000 00c1  r!...r"...r8....
-00003450: 0100 0072 5c00 0000 7a27 4c69 7374 2e64  ...r\...z'List.d
-00003460: 756d 702e 3c6c 6f63 616c 733e 2e3c 6c69  ump.<locals>.<li
-00003470: 7374 636f 6d70 3e2e 3c67 656e 6578 7072  stcomp>.<genexpr
-00003480: 3e72 b000 0000 2902 7235 0000 00da 0a69  >r....).r5.....i
-00003490: 7465 6d73 5f6c 696e 6572 a600 0000 7221  tems_liner....r!
-000034a0: 0000 0072 2200 0000 7263 0000 00c0 0100  ...r"...rc......
-000034b0: 0073 0800 0000 0600 0202 16ff 06ff 7a1d  .s............z.
-000034c0: 4c69 7374 2e64 756d 702e 3c6c 6f63 616c  List.dump.<local
-000034d0: 733e 2e3c 6c69 7374 636f 6d70 3e63 0100  s>.<listcomp>c..
-000034e0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-000034f0: 0000 3300 0000 7320 0000 0081 007c 005d  ..3...s .....|.]
-00003500: 0b7d 0188 0064 0017 0064 0114 007c 0117  .}...d...d...|..
-00003510: 0056 0001 0071 0264 0253 0029 0372 3900  .V...q.d.S.).r9.
-00003520: 0000 727a 0000 004e 7221 0000 0029 0272  ..rz...Nr!...).r
-00003530: 3500 0000 72bd 0000 0072 c600 0000 7221  5...r....r....r!
-00003540: 0000 0072 2200 0000 7238 0000 00c4 0100  ...r"...r8......
-00003550: 0073 0400 0000 0280 1e00 7a1c 4c69 7374  .s........z.List
-00003560: 2e64 756d 702e 3c6c 6f63 616c 733e 2e3c  .dump.<locals>.<
-00003570: 6765 6e65 7870 723e 7a02 293b 2909 72b2  genexpr>z.);).r.
-00003580: 0000 00da 0665 7874 656e 6472 c500 0000  .....extendr....
-00003590: 7228 0000 0072 be00 0000 7234 0000 0072  r(...r....r4...r
-000035a0: 2700 0000 da04 6b65 7973 723d 0000 0029  '.....keysr=...)
-000035b0: 0b72 4400 0000 7299 0000 0072 7700 0000  .rD...r....rw...
-000035c0: 72bc 0000 0072 7400 0000 5a0d 7370 6563  r....rt...Z.spec
-000035d0: 6961 6c5f 6b65 7973 735a 0c73 7065 6369  ial_keyssZ.speci
-000035e0: 616c 5f6b 6579 735a 0b73 7065 6369 616c  al_keysZ.special
-000035f0: 5f6b 6579 da05 6c69 6e65 7372 cd00 0000  _key..linesr....
-00003600: 7290 0000 0072 2100 0000 72c4 0000 0072  r....r!...r....r
-00003610: 2200 0000 7280 0000 009c 0100 0073 5000  "...r........sP.
-00003620: 0000 0401 0801 0a01 1201 1601 0602 0a01  ................
-00003630: 0201 0a01 0201 02ff 0601 04ff 04ff 1c05  ................
-00003640: 0202 0201 06fe 0e04 1c01 0401 0a01 0c01  ................
-00003650: 0801 0801 0401 0401 0801 0801 0801 0a01  ................
-00003660: 0801 0c02 0a01 0a01 0202 06fe 1804 0e01  ................
-00003670: 0a01 7a09 4c69 7374 2e64 756d 7072 9400  ..z.List.dumpr..
-00003680: 0000 729a 0000 0029 0c72 4700 0000 7248  ..r....).rG...rH
-00003690: 0000 0072 4900 0000 da07 5f5f 646f 635f  ...rI.....__doc_
-000036a0: 5f72 7600 0000 72b7 0000 0072 c100 0000  _rv...r....r....
-000036b0: 7278 0000 0072 c500 0000 72c3 0000 0072  rx...r....r....r
-000036c0: 8000 0000 72a2 0000 0072 2100 0000 7221  ....r....r!...r!
-000036d0: 0000 0072 a000 0000 7222 0000 0072 3300  ...r....r"...r3.
-000036e0: 0000 7c01 0000 7312 0000 0008 0004 010e  ..|...s.........
-000036f0: 0208 0508 030c 0908 030a 0312 0672 3300  .............r3.
-00003700: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00003710: 0000 0001 0000 0040 0000 0073 1000 0000  .......@...s....
-00003720: 6500 5a01 6400 5a02 6401 5a03 6402 5300  e.Z.d.Z.d.Z.d.S.
-00003730: 2903 72bb 0000 007a 2241 2064 6963 7469  ).r....z"A dicti
-00003740: 6f6e 6e61 7279 2074 6f20 7374 6f72 6520  onnary to store 
-00003750: 2363 6f64 6553 7472 6561 6d4e 2904 7247  #codeStreamN).rG
-00003760: 0000 0072 4800 0000 7249 0000 0072 d100  ...rH...rI...r..
-00003770: 0000 7221 0000 0072 2100 0000 7221 0000  ..r!...r!...r!..
-00003780: 0072 2200 0000 72bb 0000 00c9 0100 0073  .r"...r........s
-00003790: 0400 0000 0800 0801 72bb 0000 0063 0100  ........r....c..
-000037a0: 0000 0000 0000 0000 0000 0300 0000 0300  ................
-000037b0: 0000 0300 0000 7322 0000 0087 0066 0164  ......s".....f.d
-000037c0: 0164 0284 087d 0187 0066 0164 0364 0484  .d...}...f.d.d..
-000037d0: 087d 0274 007c 017c 0283 0253 0029 054e  .}.t.|.|...S.).N
-000037e0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000037f0: 0002 0000 0013 0000 0073 0a00 0000 7c00  .........s....|.
-00003800: 8800 1900 6a00 5300 7230 0000 00a9 01da  ....j.S.r0......
-00003810: 0463 6f64 6572 a600 0000 725d 0000 0072  .coder....r]...r
-00003820: 2100 0000 7222 0000 0072 5200 0000 ce01  !...r"...rR.....
-00003830: 0000 7293 0000 007a 185f 6d61 6b65 5f61  ..r....z._make_a
-00003840: 6c69 6173 2e3c 6c6f 6361 6c73 3e2e 6765  lias.<locals>.ge
-00003850: 7463 0200 0000 0000 0000 0000 0000 0200  tc..............
-00003860: 0000 0300 0000 1300 0000 730e 0000 007c  ..........s....|
-00003870: 017c 0088 0019 005f 0064 0053 0072 3000  .|....._.d.S.r0.
-00003880: 0000 72d2 0000 0029 02da 055f 7365 6c66  ..r....)..._self
-00003890: 7237 0000 0072 5d00 0000 7221 0000 0072  r7...r]...r!...r
-000038a0: 2200 0000 da03 7365 74d1 0100 0072 8f00  ".....set....r..
-000038b0: 0000 7a18 5f6d 616b 655f 616c 6961 732e  ..z._make_alias.
-000038c0: 3c6c 6f63 616c 733e 2e73 6574 2901 da08  <locals>.set)...
-000038d0: 7072 6f70 6572 7479 2903 724d 0000 0072  property).rM...r
-000038e0: 5200 0000 72d5 0000 0072 2100 0000 725d  R...r....r!...r]
-000038f0: 0000 0072 2200 0000 da0b 5f6d 616b 655f  ...r"....._make_
-00003900: 616c 6961 73cd 0100 0073 0600 0000 0c01  alias....s......
-00003910: 0c03 0a03 72d7 0000 0029 045a 0b63 6f64  ....r....).Z.cod
-00003920: 6549 6e63 6c75 6465 5a0b 636f 6465 4f70  eIncludeZ.codeOp
-00003930: 7469 6f6e 735a 0863 6f64 654c 6962 7372  tionsZ.codeLibsr
-00003940: d300 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00003950: 0000 0000 0003 0000 0040 0000 0072 a300  .........@...r..
-00003960: 0000 290b da04 436f 6465 4e63 0400 0000  ..)...CodeNc....
-00003970: 0000 0000 0000 0000 0400 0000 0200 0000  ................
-00003980: 4300 0000 731a 0000 007c 017c 005f 0074  C...s....|.|._.t
-00003990: 017c 0283 017c 005f 027c 037c 005f 0364  .|...|._.|.|._.d
-000039a0: 0053 0072 3000 0000 2904 724d 0000 0072  .S.r0...).rM...r
-000039b0: 0600 0000 72d3 0000 0072 b400 0000 2904  ....r....r....).
-000039c0: 7244 0000 0072 4d00 0000 72d3 0000 0072  rD...rM...r....r
-000039d0: b400 0000 7221 0000 0072 2100 0000 7222  ....r!...r!...r"
-000039e0: 0000 0072 7600 0000 dc01 0000 7306 0000  ...rv.......s...
-000039f0: 0006 010a 010a 017a 0d43 6f64 652e 5f5f  .......z.Code.__
-00003a00: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
-00003a10: 0000 0001 0000 0005 0000 0043 0000 0073  ...........C...s
-00003a20: 3e00 0000 7c00 6a00 6400 7500 7210 6401  >...|.j.d.u.r.d.
-00003a30: 7c00 6a01 6400 6402 8502 1900 9b00 6403  |.j.d.d.......d.
-00003a40: 9d03 5300 6401 7c00 6a01 6400 6402 8502  ..S.d.|.j.d.d...
-00003a50: 1900 9b00 6404 7c00 6a00 9b00 6405 9d05  ....d.|.j...d...
-00003a60: 5300 2906 4e7a 0643 6f64 6528 2272 2f00  S.).Nz.Code("r/.
-00003a70: 0000 7a07 5b2e 2e2e 5d22 297a 125b 2e2e  ..z.[...]")z.[..
-00003a80: 2e5d 222c 2064 6972 6563 7469 7665 3d72  .]", directive=r
-00003a90: a500 0000 2902 72b4 0000 0072 d300 0000  ....).r....r....
-00003aa0: 72a6 0000 0072 2100 0000 7221 0000 0072  r....r!...r!...r
-00003ab0: 2200 0000 7278 0000 00e1 0100 0073 0600  "...rx.......s..
-00003ac0: 0000 0a01 1601 1e01 7a0d 436f 6465 2e5f  ........z.Code._
-00003ad0: 5f72 6570 725f 5f72 0100 0000 6302 0000  _repr__r....c...
-00003ae0: 0000 0000 0000 0000 0007 0000 0005 0000  ................
-00003af0: 0043 0000 0073 8a00 0000 6700 7d02 7c01  .C...s....g.}.|.
-00003b00: 6401 1400 7d03 7c01 6402 1700 6401 1400  d...}.|.d...d...
-00003b10: 7d04 7c03 7c00 6a00 1700 7d05 7c00 6a01  }.|.|.j...}.|.j.
-00003b20: 6400 7501 721d 7c05 6401 7c00 6a01 1700  d.u.r.|.d.|.j...
-00003b30: 3700 7d05 7c02 a002 7c05 6403 7c03 9b00  7.}.|...|.d.|...
-00003b40: 9d02 1700 6404 1700 a101 0100 7c00 6a03  ....d.......|.j.
-00003b50: a004 6403 a101 4400 5d09 7d06 7c02 a002  ..d...D.].}.|...
-00003b60: 7c04 7c06 1700 a101 0100 712f 7c02 a002  |.|.......q/|...
-00003b70: 7c03 6405 1700 a101 0100 6403 a005 7c02  |.d.......d...|.
-00003b80: a101 5300 2906 4e72 7a00 0000 7239 0000  ..S.).Nrz...r9..
-00003b90: 0072 7e00 0000 7a02 237b 7a03 237d 3b29  .r~...z.#{z.#};)
-00003ba0: 0672 4d00 0000 72b4 0000 0072 2700 0000  .rM...r....r'...
-00003bb0: 72d3 0000 0072 1900 0000 7228 0000 0029  r....r....r(...)
-00003bc0: 0772 4400 0000 7299 0000 0072 7700 0000  .rD...r....rw...
-00003bd0: 72bc 0000 005a 0c69 6e64 656e 7461 7469  r....Z.indentati
-00003be0: 6f6e 3472 1700 0000 72bd 0000 0072 2100  on4r....r....r!.
-00003bf0: 0000 7221 0000 0072 2200 0000 7280 0000  ..r!...r"...r...
-00003c00: 00e6 0100 0073 1600 0000 0401 0801 0c01  .....s..........
-00003c10: 0a01 0a01 0e01 1801 1001 1001 0e01 0a01  ................
-00003c20: 7a09 436f 6465 2e64 756d 7072 3000 0000  z.Code.dumpr0...
-00003c30: 729a 0000 00a9 0672 4700 0000 7248 0000  r......rG...rH..
-00003c40: 0072 4900 0000 7276 0000 0072 7800 0000  .rI...rv...rx...
-00003c50: 7280 0000 0072 2100 0000 7221 0000 0072  r....r!...r!...r
-00003c60: 2100 0000 7222 0000 0072 d800 0000 db01  !...r"...r......
-00003c70: 0000 7308 0000 0008 000a 0108 050e 0572  ..s............r
-00003c80: d800 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00003c90: 0000 0000 0003 0000 0040 0000 0072 a300  .........@...r..
-00003ca0: 0000 290b da04 4e61 6d65 4e63 0300 0000  ..)...NameNc....
-00003cb0: 0000 0000 0000 0000 0300 0000 0200 0000  ................
-00003cc0: 4300 0000 f310 0000 007c 017c 005f 007c  C........|.|._.|
-00003cd0: 027c 005f 0164 0053 0072 3000 0000 2902  .|._.d.S.r0...).
-00003ce0: 724d 0000 0072 3700 0000 2903 7244 0000  rM...r7...).rD..
-00003cf0: 0072 4d00 0000 7237 0000 0072 2100 0000  .rM...r7...r!...
-00003d00: 7221 0000 0072 2200 0000 7276 0000 00f6  r!...r"...rv....
-00003d10: 0100 00f3 0400 0000 0601 0a01 7a0d 4e61  ............z.Na
-00003d20: 6d65 2e5f 5f69 6e69 745f 5f63 0100 0000  me.__init__c....
-00003d30: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00003d40: 4300 0000 730e 0000 0064 017c 006a 009b  C...s....d.|.j..
-00003d50: 0064 029d 0353 0029 034e 7a05 4e61 6d65  .d...S.).Nz.Name
-00003d60: 2872 a500 0000 725d 0000 0072 a600 0000  (r....r]...r....
-00003d70: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
-00003d80: 7800 0000 fa01 0000 728f 0000 007a 0d4e  x.......r....z.N
-00003d90: 616d 652e 5f5f 7265 7072 5f5f 7201 0000  ame.__repr__r...
-00003da0: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
-00003db0: 0000 0100 0000 4300 0000 7308 0000 007c  ......C...s....|
-00003dc0: 006a 009b 0053 0072 3000 0000 725d 0000  .j...S.r0...r]..
-00003dd0: 0072 9800 0000 7221 0000 0072 2100 0000  .r....r!...r!...
-00003de0: 7222 0000 0072 8000 0000 fd01 0000 72ae  r"...r........r.
-00003df0: 0000 007a 094e 616d 652e 6475 6d70 7230  ...z.Name.dumpr0
-00003e00: 0000 0072 9a00 0000 72d9 0000 0072 2100  ...r....r....r!.
-00003e10: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
-00003e20: 0072 da00 0000 f401 0000 7308 0000 0008  .r........s.....
-00003e30: 000a 0208 040e 0372 da00 0000 6300 0000  .......r....c...
-00003e40: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00003e50: 0040 0000 0073 2600 0000 6500 5a01 6400  .@...s&...e.Z.d.
-00003e60: 5a02 6401 6402 8400 5a03 6403 6404 8400  Z.d.d...Z.d.d...
-00003e70: 5a04 6409 6406 6407 8401 5a05 6408 5300  Z.d.d.d...Z.d.S.
-00003e80: 290a da09 4469 7265 6374 6976 6563 0300  )...Directivec..
-00003e90: 0000 0000 0000 0000 0000 0300 0000 0200  ................
-00003ea0: 0000 4300 0000 72db 0000 0072 3000 0000  ..C...r....r0...
-00003eb0: a902 72b4 0000 00da 0763 6f6e 7465 6e74  ..r......content
-00003ec0: 2903 7244 0000 0072 b400 0000 72df 0000  ).rD...r....r...
-00003ed0: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
-00003ee0: 7276 0000 0002 0200 0072 dc00 0000 7a12  rv.......r....z.
-00003ef0: 4469 7265 6374 6976 652e 5f5f 696e 6974  Directive.__init
-00003f00: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
-00003f10: 0000 0003 0000 0043 0000 0073 1200 0000  .......C...s....
-00003f20: 7c00 6a00 9b00 6401 7c00 6a01 9b00 9d03  |.j...d.|.j.....
-00003f30: 5300 2902 4e72 9700 0000 72de 0000 0072  S.).Nr....r....r
-00003f40: a600 0000 7221 0000 0072 2100 0000 7222  ....r!...r!...r"
-00003f50: 0000 0072 7800 0000 0602 0000 7302 0000  ...rx.......s...
-00003f60: 0012 017a 1244 6972 6563 7469 7665 2e5f  ...z.Directive._
-00003f70: 5f72 6570 725f 5f72 0100 0000 6302 0000  _repr__r....c...
-00003f80: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-00003f90: 0043 0000 0073 1c00 0000 7c01 6401 1400  .C...s....|.d...
-00003fa0: 7c00 6a00 9b00 6402 7c00 6a01 9b00 6403  |.j...d.|.j...d.
-00003fb0: 9d04 1700 5300 2904 4e72 7a00 0000 7297  ....S.).Nrz...r.
-00003fc0: 0000 0072 7c00 0000 72de 0000 0072 9800  ...r|...r....r..
-00003fd0: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
-00003fe0: 0072 8000 0000 0902 0000 72b1 0000 007a  .r........r....z
-00003ff0: 0e44 6972 6563 7469 7665 2e64 756d 704e  .Directive.dumpN
-00004000: 729a 0000 0072 d900 0000 7221 0000 0072  r....r....r!...r
-00004010: 2100 0000 7221 0000 0072 2200 0000 72dd  !...r!...r"...r.
-00004020: 0000 0001 0200 0073 0800 0000 0800 0801  .......s........
-00004030: 0804 0e03 72dd 0000 0029 0172 2f00 0000  ....r....).r/...
-00004040: 2927 72d1 0000 0072 1500 0000 da03 6162  )'r....r......ab
-00004050: 6372 0200 0000 7203 0000 00da 0b64 6174  cr....r......dat
-00004060: 6163 6c61 7373 6573 7204 0000 00da 076e  aclassesr......n
-00004070: 756d 6265 7273 7205 0000 00da 0874 6578  umbersr......tex
-00004080: 7477 7261 7072 0600 0000 da06 7479 7069  twrapr......typi
-00004090: 6e67 7207 0000 00da 056e 756d 7079 7267  ngr......numpyrg
-000040a0: 0000 00da 0a69 6e66 6c65 6374 696f 6e72  .....inflectionr
-000040b0: 0800 0000 721b 0000 0072 2300 0000 722e  ....r....r#...r.
-000040c0: 0000 0072 4000 0000 7241 0000 0072 4a00  ...r@...rA...rJ.
-000040d0: 0000 7271 0000 0072 9500 0000 729d 0000  ..rq...r....r...
-000040e0: 0072 6f00 0000 7251 0000 0072 6900 0000  .ro...rQ...ri...
-000040f0: 7254 0000 0072 3200 0000 7233 0000 0072  rT...r2...r3...r
-00004100: bb00 0000 72d7 0000 0072 b200 0000 da07  ....r....r......
-00004110: 7365 7461 7474 7272 d800 0000 72da 0000  setattrr....r...
-00004120: 0072 dd00 0000 7221 0000 0072 2100 0000  .r....r!...r!...
-00004130: 7221 0000 0072 2200 0000 da08 3c6d 6f64  r!...r".....<mod
-00004140: 756c 653e 0100 0000 7340 0000 0004 0008  ule>....s@......
-00004150: 0210 010c 010c 010c 010c 0108 020c 0108  ................
-00004160: 0208 0308 1b0a 120e 1110 0712 5702 4b10  ............W.K.
-00004170: 0110 0b02 0c12 0112 2614 0f12 3710 4d08  ........&...7.M.
-00004180: 0408 0a16 0110 0302 1912 0114 0c         .............
+00001b30: 0000 0000 0003 0000 0005 0000 0043 0000  .............C..
+00001b40: 0073 5000 0000 7400 7c00 6a01 6401 8302  .sP...t.|.j.d...
+00001b50: 720c 7c00 6a01 a002 7c01 a101 5300 7400  r.|.j...|...S.t.
+00001b60: 7c00 6a01 6402 8302 7218 7c00 6a01 a003  |.j.d...r.|.j...
+00001b70: a100 7d02 6e03 7c00 6a01 7d02 7c01 6403  ..}.n.|.j.}.|.d.
+00001b80: 1400 7c00 6a04 9b00 6404 7c02 9b00 6405  ..|.j...d.|...d.
+00001b90: 9d04 1700 5300 2906 4e72 7f00 0000 7280  ....S.).Nr....r.
+00001ba0: 0000 0072 7900 0000 fa02 2020 727b 0000  ...ry.....  r{..
+00001bb0: 0029 0572 8100 0000 7236 0000 0072 7f00  .).r....r6...r..
+00001bc0: 0000 7280 0000 0072 4c00 0000 a903 7243  ..r....rL.....rC
+00001bd0: 0000 00da 0669 6e64 656e 7472 3600 0000  .....indentr6...
+00001be0: 7220 0000 0072 2000 0000 7221 0000 0072  r ...r ...r!...r
+00001bf0: 7f00 0000 fc00 0000 730c 0000 000c 010c  ........s.......
+00001c00: 010c 010c 0106 021a 017a 0f41 7373 6967  .........z.Assig
+00001c10: 6e6d 656e 742e 6475 6d70 4ea9 0172 0100  nment.dumpN..r..
+00001c20: 0000 2907 7246 0000 0072 4700 0000 7248  ..).rF...rG...rH
+00001c30: 0000 0072 4e00 0000 da0f 5f5f 616e 6e6f  ...rN.....__anno
+00001c40: 7461 7469 6f6e 735f 5fda 066f 626a 6563  tations__..objec
+00001c50: 7472 7f00 0000 7220 0000 0072 2000 0000  tr....r ...r ...
+00001c60: 7220 0000 0072 2100 0000 7294 0000 00f7  r ...r!...r.....
+00001c70: 0000 0073 0800 0000 0a00 0802 0801 0e02  ...s............
+00001c80: 7294 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00001c90: 0000 0000 0000 0300 0000 0000 0000 7326  ..............s&
+00001ca0: 0000 0065 005a 0164 005a 0287 0066 0164  ...e.Z.d.Z...f.d
+00001cb0: 0164 0284 085a 0364 0664 0464 0584 015a  .d...Z.d.d.d...Z
+00001cc0: 0487 0004 005a 0553 0029 07da 1256 6172  .....Z.S.)...Var
+00001cd0: 6961 626c 6541 7373 6967 6e6d 656e 7463  iableAssignmentc
+00001ce0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001cf0: 0200 0000 0300 0000 730e 0000 0074 0083  ........s....t..
+00001d00: 00a0 01a1 007d 017c 0153 0072 2f00 0000  .....}.|.S.r/...
+00001d10: a902 da05 7375 7065 7272 7700 0000 2902  ....superrw...).
+00001d20: 7243 0000 0072 0a00 0000 a901 da09 5f5f  rC...r........__
+00001d30: 636c 6173 735f 5f72 2000 0000 7221 0000  class__r ...r!..
+00001d40: 0072 7700 0000 0701 0000 7304 0000 000a  .rw.......s.....
+00001d50: 0104 017a 1b56 6172 6961 626c 6541 7373  ...z.VariableAss
+00001d60: 6967 6e6d 656e 742e 5f5f 7265 7072 5f5f  ignment.__repr__
+00001d70: 7201 0000 0063 0200 0000 0000 0000 0000  r....c..........
+00001d80: 0000 0300 0000 0600 0000 4300 0000 7366  ..........C...sf
+00001d90: 0000 0074 007c 006a 0164 0183 0272 177c  ...t.|.j.d...r.|
+00001da0: 0164 0214 007c 006a 029b 0064 037c 006a  .d...|.j...d.|.j
+00001db0: 01a0 037c 01a1 019b 0064 049d 0417 0053  ...|.....d.....S
+00001dc0: 0074 007c 006a 0164 0583 0272 237c 006a  .t.|.j.d...r#|.j
+00001dd0: 01a0 04a1 007d 026e 037c 006a 017d 027c  .....}.n.|.j.}.|
+00001de0: 0164 0214 007c 006a 029b 0064 037c 029b  .d...|.j...d.|..
+00001df0: 0064 049d 0417 0053 0029 064e 727f 0000  .d.....S.).Nr...
+00001e00: 0072 7900 0000 7295 0000 0072 7b00 0000  .ry...r....r{...
+00001e10: 7280 0000 0029 0572 8100 0000 7236 0000  r....).r....r6..
+00001e20: 0072 4c00 0000 727f 0000 0072 8000 0000  .rL...r....r....
+00001e30: 7296 0000 0072 2000 0000 7220 0000 0072  r....r ...r ...r
+00001e40: 2100 0000 727f 0000 000b 0100 0073 0c00  !...r........s..
+00001e50: 0000 0c01 2201 0c01 0c01 0602 1a01 7a17  ....".........z.
+00001e60: 5661 7269 6162 6c65 4173 7369 676e 6d65  VariableAssignme
+00001e70: 6e74 2e64 756d 7072 9800 0000 2906 7246  nt.dumpr....).rF
+00001e80: 0000 0072 4700 0000 7248 0000 0072 7700  ...rG...rH...rw.
+00001e90: 0000 727f 0000 00da 0d5f 5f63 6c61 7373  ..r......__class
+00001ea0: 6365 6c6c 5f5f 7220 0000 0072 2000 0000  cell__r ...r ...
+00001eb0: 729e 0000 0072 2100 0000 729b 0000 0006  r....r!...r.....
+00001ec0: 0100 0073 0600 0000 0800 0c01 1204 729b  ...s..........r.
+00001ed0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00001ee0: 0000 0000 0300 0000 4000 0000 f328 0000  ........@....(..
+00001ef0: 0065 005a 0164 005a 0264 0964 0264 0384  .e.Z.d.Z.d.d.d..
+00001f00: 015a 0364 0464 0584 005a 0464 0a64 0764  .Z.d.d...Z.d.d.d
+00001f10: 0884 015a 0564 0153 0029 0b72 6e00 0000  ...Z.d.S.).rn...
+00001f20: 4e63 0400 0000 0000 0000 0000 0000 0400  Nc..............
+00001f30: 0000 0400 0000 4300 0000 732c 0000 007c  ......C...s,...|
+00001f40: 017c 005f 007c 027c 005f 0174 027c 0374  .|._.|.|._.t.|.t
+00001f50: 0374 0466 0283 0272 1174 057c 0383 017d  .t.f...r.t.|...}
+00001f60: 037c 037c 005f 0664 0053 0072 2f00 0000  .|.|._.d.S.r/...
+00001f70: 2907 7236 0000 0072 4c00 0000 7230 0000  ).r6...rL...r0..
+00001f80: 0072 5000 0000 da05 7475 706c 6572 2d00  .rP.....tupler-.
+00001f90: 0000 7257 0000 0029 0472 4300 0000 7236  ..rW...).rC...r6
+00001fa0: 0000 0072 4c00 0000 7257 0000 0072 2000  ...rL...rW...r .
+00001fb0: 0000 7220 0000 0072 2100 0000 7275 0000  ..r ...r!...ru..
+00001fc0: 0017 0100 0073 0a00 0000 0601 0601 0e01  .....s..........
+00001fd0: 0801 0a01 7a0e 5661 6c75 652e 5f5f 696e  ....z.Value.__in
+00001fe0: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
+00001ff0: 0001 0000 0007 0000 0043 0000 0073 9400  .........C...s..
+00002000: 0000 7c00 6a00 6400 7501 7219 7c00 6a01  ..|.j.d.u.r.|.j.
+00002010: 6400 7501 7219 6401 7c00 6a02 9b00 6402  d.u.r.d.|.j...d.
+00002020: 7c00 6a01 9b00 6403 7c00 6a00 9b00 6404  |.j...d.|.j...d.
+00002030: 9d07 5300 7c00 6a00 6400 7500 722e 7c00  ..S.|.j.d.u.r.|.
+00002040: 6a01 6400 7501 722e 6401 7c00 6a02 9b00  j.d.u.r.d.|.j...
+00002050: 6402 7c00 6a01 9b00 6404 9d05 5300 7c00  d.|.j...d...S.|.
+00002060: 6a00 6400 7501 7243 7c00 6a01 6400 7500  j.d.u.rC|.j.d.u.
+00002070: 7243 6401 7c00 6a02 9b00 6405 7c00 6a00  rCd.|.j...d.|.j.
+00002080: 9b00 6404 9d05 5300 6401 7c00 6a02 9b00  ..d...S.d.|.j...
+00002090: 6406 9d03 5300 2907 4e7a 0656 616c 7565  d...S.).Nz.Value
+000020a0: 287a 082c 206e 616d 653d 227a 0e22 2c20  (z., name="z.", 
+000020b0: 6469 6d65 6e73 696f 6e3d 227a 0222 297a  dimension="z.")z
+000020c0: 0d2c 2064 696d 656e 7369 6f6e 3d22 fa01  ., dimension="..
+000020d0: 2929 0372 5700 0000 724c 0000 0072 3600  )).rW...rL...r6.
+000020e0: 0000 a901 7243 0000 0072 2000 0000 7220  ....rC...r ...r 
+000020f0: 0000 0072 2100 0000 7277 0000 001e 0100  ...r!...rw......
+00002100: 0073 0e00 0000 1401 1e01 1401 1601 1401  .s..............
+00002110: 1601 0e02 7a0e 5661 6c75 652e 5f5f 7265  ....z.Value.__re
+00002120: 7072 5f5f 7201 0000 0063 0200 0000 0000  pr__r....c......
+00002130: 0000 0000 0000 0500 0000 0500 0000 4300  ..............C.
+00002140: 0000 73ce 0000 007c 006a 0064 0075 0172  ..s....|.j.d.u.r
+00002150: 1474 017c 006a 0083 017d 0264 01a0 0264  .t.|.j...}.d...d
+00002160: 0264 0384 007c 0244 0083 01a1 017d 0374  .d...|.D.....}.t
+00002170: 037c 006a 0474 0583 0272 2674 067c 006a  .|.j.t...r&t.|.j
+00002180: 0464 0483 0272 267c 006a 04a0 07a1 007d  .d...r&|.j.....}
+00002190: 046e 0574 087c 006a 0483 017d 047c 006a  .n.t.|.j...}.|.j
+000021a0: 0064 0075 0172 407c 006a 0964 0075 0172  .d.u.r@|.j.d.u.r
+000021b0: 407c 006a 099b 0064 057c 039b 0064 067c  @|.j...d.|...d.|
+000021c0: 049b 009d 0553 007c 006a 0064 0075 0072  .....S.|.j.d.u.r
+000021d0: 527c 006a 0964 0075 0172 527c 006a 099b  R|.j.d.u.rR|.j..
+000021e0: 0064 017c 049b 009d 0353 007c 006a 0064  .d.|.....S.|.j.d
+000021f0: 0075 0172 647c 006a 0964 0075 0072 6464  .u.rd|.j.d.u.rdd
+00002200: 077c 039b 0064 067c 049b 009d 0453 007c  .|...d.|.....S.|
+00002210: 049b 0053 0029 084e 7279 0000 0063 0100  ...S.).Nry...c..
+00002220: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00002230: 0000 7300 0000 f318 0000 0081 007c 005d  ..s..........|.]
+00002240: 077d 0174 007c 0183 0156 0001 0071 0264  .}.t.|...V...q.d
+00002250: 0053 0072 2f00 0000 a901 724e 0000 00a9  .S.r/.....rN....
+00002260: 0272 3400 0000 da06 6e75 6d62 6572 7220  .r4.....numberr 
+00002270: 0000 0072 2000 0000 7221 0000 0072 3700  ...r ...r!...r7.
+00002280: 0000 2b01 0000 f304 0000 0002 8016 007a  ..+............z
+00002290: 3056 616c 7565 2e64 756d 705f 7769 7468  0Value.dump_with
+000022a0: 6f75 745f 6173 7369 676e 6d65 6e74 2e3c  out_assignment.<
+000022b0: 6c6f 6361 6c73 3e2e 3c67 656e 6578 7072  locals>.<genexpr
+000022c0: 3e72 7f00 0000 7a02 205b 7a02 5d20 fa01  >r....z. [z.] ..
+000022d0: 5b29 0a72 5700 0000 7222 0000 0072 2700  [).rW...r"...r'.
+000022e0: 0000 7230 0000 0072 3600 0000 7240 0000  ..r0...r6...r@..
+000022f0: 0072 8100 0000 727f 0000 0072 4e00 0000  .r....r....rN...
+00002300: 724c 0000 0029 0572 4300 0000 7297 0000  rL...).rC...r...
+00002310: 005a 0e64 696d 656e 7369 6f6e 5f6c 6973  .Z.dimension_lis
+00002320: 745a 1064 696d 656e 7369 6f6e 5f64 756d  tZ.dimension_dum
+00002330: 7065 645a 0c76 616c 7565 5f64 756d 7065  pedZ.value_dumpe
+00002340: 6472 2000 0000 7220 0000 0072 2100 0000  dr ...r ...r!...
+00002350: 7280 0000 0028 0100 0073 1a00 0000 0a01  r....(...s......
+00002360: 0a01 1401 1802 0c01 0a02 1402 1601 1401  ................
+00002370: 1001 1401 1001 0602 7a1d 5661 6c75 652e  ........z.Value.
+00002380: 6475 6d70 5f77 6974 686f 7574 5f61 7373  dump_without_ass
+00002390: 6967 6e6d 656e 7429 024e 4e72 9800 0000  ignment).NNr....
+000023a0: 2906 7246 0000 0072 4700 0000 7248 0000  ).rF...rG...rH..
+000023b0: 0072 7500 0000 7277 0000 0072 8000 0000  .ru...rw...r....
+000023c0: 7220 0000 0072 2000 0000 7220 0000 0072  r ...r ...r ...r
+000023d0: 2100 0000 726e 0000 0015 0100 0073 0800  !...rn.......s..
+000023e0: 0000 0800 0a02 0807 0e0a 726e 0000 0063  ..........rn...c
+000023f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002400: 0300 0000 0000 0000 732e 0000 0065 005a  ........s....e.Z
+00002410: 0164 005a 0287 0066 0164 0164 0284 085a  .d.Z...f.d.d...Z
+00002420: 0364 0364 0484 005a 0464 0864 0664 0784  .d.d...Z.d.d.d..
+00002430: 015a 0587 0004 005a 0653 0029 0972 6800  .Z.....Z.S.).rh.
+00002440: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
+00002450: 0000 0003 0000 0003 0000 0073 3c00 0000  ...........s<...
+00002460: 7400 7c01 7401 8302 7209 7402 7c01 8301  t.|.t...r.t.|...
+00002470: 7d01 7403 6401 6402 8400 7c01 4400 8301  }.t.d.d...|.D...
+00002480: 8301 7316 7404 6403 8301 8201 7405 8300  ..s.t.d.....t...
+00002490: a006 7c01 a101 0100 6400 5300 2904 4e63  ..|.....d.S.).Nc
+000024a0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000024b0: 0400 0000 7300 0000 7259 0000 0072 2f00  ....s...rY...r/.
+000024c0: 0000 2902 7230 0000 0072 1900 0000 2902  ..).r0...r....).
+000024d0: 7234 0000 00da 0465 6c65 6d72 2000 0000  r4.....elemr ...
+000024e0: 7220 0000 0072 2100 0000 7237 0000 0040  r ...r!...r7...@
+000024f0: 0100 0072 5b00 0000 7a28 4469 6d65 6e73  ...r[...z(Dimens
+00002500: 696f 6e53 6574 2e5f 5f69 6e69 745f 5f2e  ionSet.__init__.
+00002510: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
+00002520: 723e 7a13 4261 6420 7b66 6f61 6d5f 756e  r>z.Bad {foam_un
+00002530: 6974 7320 3d20 7d29 0772 3000 0000 724e  its = }).r0...rN
+00002540: 0000 0072 2200 0000 7265 0000 0072 3c00  ...r"...re...r<.
+00002550: 0000 729d 0000 0072 7500 0000 2902 7243  ..r....ru...).rC
+00002560: 0000 0072 2900 0000 729e 0000 0072 2000  ...r)...r....r .
+00002570: 0000 7221 0000 0072 7500 0000 3d01 0000  ..r!...ru...=...
+00002580: 730a 0000 000a 0108 0112 0108 0110 017a  s..............z
+00002590: 1544 696d 656e 7369 6f6e 5365 742e 5f5f  .DimensionSet.__
+000025a0: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+000025b0: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
+000025c0: 0800 0000 7400 7c00 8301 5300 722f 0000  ....t.|...S.r/..
+000025d0: 0029 0172 2d00 0000 72a4 0000 0072 2000  .).r-...r....r .
+000025e0: 0000 7220 0000 0072 2100 0000 7277 0000  ..r ...r!...rw..
+000025f0: 0044 0100 00f3 0200 0000 0801 7a15 4469  .D..........z.Di
+00002600: 6d65 6e73 696f 6e53 6574 2e5f 5f72 6570  mensionSet.__rep
+00002610: 725f 5f72 0100 0000 6302 0000 0000 0000  r__r....c.......
+00002620: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
+00002630: 0073 1c00 0000 6401 6402 a000 6403 6404  .s....d.d...d.d.
+00002640: 8400 7c00 4400 8301 a101 1700 6405 1700  ..|.D.......d...
+00002650: 5300 2906 4e72 aa00 0000 7279 0000 0063  S.).Nr....ry...c
+00002660: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00002670: 0300 0000 7300 0000 72a5 0000 0072 2f00  ....s...r....r/.
+00002680: 0000 72a6 0000 0072 a700 0000 7220 0000  ..r....r....r ..
+00002690: 0072 2000 0000 7221 0000 0072 3700 0000  .r ...r!...r7...
+000026a0: 4801 0000 72a9 0000 007a 3744 696d 656e  H...r....z7Dimen
+000026b0: 7369 6f6e 5365 742e 6475 6d70 5f77 6974  sionSet.dump_wit
+000026c0: 686f 7574 5f61 7373 6967 6e6d 656e 742e  hout_assignment.
+000026d0: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
+000026e0: 723e fa01 5da9 0172 2700 0000 a902 7243  r>..]..r'.....rC
+000026f0: 0000 0072 9700 0000 7220 0000 0072 2000  ...r....r ...r .
+00002700: 0000 7221 0000 0072 8000 0000 4701 0000  ..r!...r....G...
+00002710: f302 0000 001c 017a 2444 696d 656e 7369  .......z$Dimensi
+00002720: 6f6e 5365 742e 6475 6d70 5f77 6974 686f  onSet.dump_witho
+00002730: 7574 5f61 7373 6967 6e6d 656e 7472 9800  ut_assignmentr..
+00002740: 0000 2907 7246 0000 0072 4700 0000 7248  ..).rF...rG...rH
+00002750: 0000 0072 7500 0000 7277 0000 0072 8000  ...ru...rw...r..
+00002760: 0000 72a0 0000 0072 2000 0000 7220 0000  ..r....r ...r ..
+00002770: 0072 9e00 0000 7221 0000 0072 6800 0000  .r....r!...rh...
+00002780: 3c01 0000 7308 0000 0008 000c 0108 0712  <...s...........
+00002790: 0372 6800 0000 6300 0000 0000 0000 0000  .rh...c.........
+000027a0: 0000 0000 0000 0004 0000 0000 0000 0073  ...............s
+000027b0: 4400 0000 6500 5a01 6400 5a02 640d 8700  D...e.Z.d.Z.d...
+000027c0: 6601 6402 6403 8409 5a03 6404 6405 8400  f.d.d...Z.d.d...
+000027d0: 5a04 8700 6601 6406 6407 8408 5a05 640e  Z...f.d.d...Z.d.
+000027e0: 6409 640a 8401 5a06 640b 640c 8400 5a07  d.d...Z.d.d...Z.
+000027f0: 8700 0400 5a08 5300 290f 7231 0000 004e  ....Z.S.).r1...N
+00002800: 6305 0000 0000 0000 0000 0000 0005 0000  c...............
+00002810: 0004 0000 0003 0000 0073 2800 0000 7c02  .........s(...|.
+00002820: 7c00 5f00 7c03 7c00 5f01 7c04 7c00 5f02  |._.|.|._.|.|._.
+00002830: 7403 8300 6a04 6401 6900 7c01 a401 8e01  t...j.d.i.|.....
+00002840: 0100 6400 5300 2902 4e72 2000 0000 2905  ..d.S.).Nr ...).
+00002850: da05 5f6e 616d 65da 0a5f 6469 7265 6374  .._name.._direct
+00002860: 6976 6572 4b00 0000 729d 0000 0072 7500  iverK...r....ru.
+00002870: 0000 2905 7243 0000 0072 3d00 0000 724c  ..).rC...r=...rL
+00002880: 0000 00da 0964 6972 6563 7469 7665 724b  .....directiverK
+00002890: 0000 0072 9e00 0000 7220 0000 0072 2100  ...r....r ...r!.
+000028a0: 0000 7275 0000 004c 0100 0073 0800 0000  ..ru...L...s....
+000028b0: 0601 0601 0601 1601 7a0d 4469 6374 2e5f  ........z.Dict._
+000028c0: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+000028d0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+000028e0: f306 0000 007c 006a 0053 0072 2f00 0000  .....|.j.S.r/...
+000028f0: a901 72b1 0000 0072 a400 0000 7220 0000  ..r....r....r ..
+00002900: 0072 2000 0000 7221 0000 00da 0867 6574  .r ...r!.....get
+00002910: 5f6e 616d 6552 0100 00f3 0200 0000 0601  _nameR..........
+00002920: 7a0d 4469 6374 2e67 6574 5f6e 616d 6563  z.Dict.get_namec
+00002930: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00002940: 0200 0000 0300 0000 f30a 0000 0074 0083  .............t..
+00002950: 00a0 01a1 0053 0072 2f00 0000 729c 0000  .....S.r/...r...
+00002960: 0072 a400 0000 729e 0000 0072 2000 0000  .r....r....r ...
+00002970: 7221 0000 0072 7700 0000 5501 0000 7292  r!...rw...U...r.
+00002980: 0000 007a 0d44 6963 742e 5f5f 7265 7072  ...z.Dict.__repr
+00002990: 5f5f 7201 0000 0063 0200 0000 0000 0000  __r....c........
+000029a0: 0000 0000 0b00 0000 0900 0000 4300 0000  ............C...
+000029b0: 737a 0100 0067 007d 027c 0164 0114 007d  sz...g.}.|.d...}
+000029c0: 037c 006a 0064 0075 0172 217c 037c 006a  .|.j.d.u.r!|.|.j
+000029d0: 0017 007d 047c 006a 0164 0075 0172 1c7c  ...}.|.j.d.u.r.|
+000029e0: 0464 027c 006a 0117 0037 007d 047c 0464  .d.|.j...7.}.|.d
+000029f0: 0337 007d 046e 0264 047d 047c 02a0 027c  .7.}.n.d.}.|...|
+00002a00: 047c 0317 0064 0517 00a1 0101 0074 037c  .|...d.......t.|
+00002a10: 0083 017d 057c 00a0 04a1 0044 005d 6f5c  ...}.|.....D.]o\
+00002a20: 027d 067d 077c 006a 0564 0075 0172 577c  .}.}.|.j.d.u.rW|
+00002a30: 067c 006a 0576 0072 577c 006a 057c 0619  .|.j.v.rW|.j.|..
+00002a40: 007d 0874 067c 0874 0783 0272 577c 02a0  .}.t.|.t...rW|..
+00002a50: 0264 067c 08a0 0864 0364 07a1 0217 00a1  .d.|...d.d......
+00002a60: 0101 0074 097c 0764 0883 0272 677c 02a0  ...t.|.d...rg|..
+00002a70: 027c 07a0 0a7c 0164 0917 00a1 01a1 0101  .|...|.d........
+00002a80: 0071 347c 0764 0075 0072 767c 02a0 027c  .q4|.d.u.rv|...|
+00002a90: 0364 0a7c 069b 009d 0217 00a1 0101 0071  .d.|...........q
+00002aa0: 3474 097c 0764 0b83 0272 807c 07a0 0ba1  4t.|.d...r.|....
+00002ab0: 007d 096e 027c 077d 097c 0764 046b 0272  .}.n.|.}.|.d.k.r
+00002ac0: 8964 047d 0a6e 0b74 0c64 0c7c 0574 0d7c  .d.}.n.t.d.|.t.|
+00002ad0: 0683 0118 0083 0264 0114 007d 0a7c 02a0  .......d...}.|..
+00002ae0: 027c 0364 0a7c 069b 007c 0a9b 007c 099b  .|.d.|...|...|..
+00002af0: 0064 0d9d 0517 00a1 0101 0071 347c 02a0  .d.........q4|..
+00002b00: 027c 0364 0e17 00a1 0101 0074 067c 0074  .|.d.......t.|.t
+00002b10: 0e83 0272 b87c 0264 0f05 0019 0064 0d37  ...r.|.d.....d.7
+00002b20: 0003 003c 0064 03a0 0f7c 02a1 0153 0029  ...<.d...|...S.)
+00002b30: 104e 7279 0000 0072 9500 0000 727d 0000  .Nry...r....r}..
+00002b40: 0072 0f00 0000 da01 7b7a 0720 2020 202f  .r......{z.    /
+00002b50: 2f20 7a08 0a20 2020 202f 2f20 727f 0000  / z..    // r...
+00002b60: 0072 3800 0000 727a 0000 0072 8000 0000  .r8...rz...r....
+00002b70: 725d 0000 0072 7b00 0000 727c 0000 0072  r]...r{...r|...r
+00002b80: 1300 0000 2910 72b1 0000 0072 b200 0000  ....).r....r....
+00002b90: 7226 0000 0072 3f00 0000 723b 0000 0072  r&...r?...r;...r
+00002ba0: 4b00 0000 7230 0000 0072 4e00 0000 7282  K...r0...rN...r.
+00002bb0: 0000 0072 8100 0000 727f 0000 0072 8000  ...r....r....r..
+00002bc0: 0000 723a 0000 0072 3300 0000 da0a 436f  ..r:...r3.....Co
+00002bd0: 6465 5374 7265 616d 7227 0000 0029 0b72  deStreamr'...).r
+00002be0: 4300 0000 7297 0000 0072 7600 0000 da0b  C...r....rv.....
+00002bf0: 696e 6465 6e74 6174 696f 6eda 0473 7461  indentation..sta
+00002c00: 7272 8400 0000 7235 0000 0072 8300 0000  rr....r5...r....
+00002c10: 7286 0000 0072 8500 0000 720a 0000 0072  r....r....r....r
+00002c20: 2000 0000 7220 0000 0072 2100 0000 727f   ...r ...r!...r.
+00002c30: 0000 0058 0100 0073 3c00 0000 0401 0801  ...X...s<.......
+00002c40: 0a01 0a01 0a01 0e01 0a01 0402 1201 0802  ................
+00002c50: 1001 1401 0a01 0a01 1601 0a02 1601 0801  ................
+00002c60: 1601 0a02 0a01 0402 0801 0601 1602 2001  .............. .
+00002c70: 0e01 0a03 1001 0a02 7a09 4469 6374 2e64  ........z.Dict.d
+00002c80: 756d 7063 0300 0000 0000 0000 0000 0000  umpc............
+00002c90: 0300 0000 0300 0000 4300 0000 730c 0000  ........C...s...
+00002ca0: 007c 027c 007c 013c 0064 0053 0072 2f00  .|.|.|.<.d.S.r/.
+00002cb0: 0000 7220 0000 0072 6f00 0000 7220 0000  ..r ...ro...r ..
+00002cc0: 0072 2000 0000 7221 0000 0072 5500 0000  .r ...r!...rU...
+00002cd0: 8101 0000 7302 0000 000c 017a 0e44 6963  ....s......z.Dic
+00002ce0: 742e 5f73 6574 5f69 7465 6d72 9300 0000  t._set_itemr....
+00002cf0: 7298 0000 0029 0972 4600 0000 7247 0000  r....).rF...rG..
+00002d00: 0072 4800 0000 7275 0000 0072 b600 0000  .rH...ru...r....
+00002d10: 7277 0000 0072 7f00 0000 7255 0000 0072  rw...r....rU...r
+00002d20: a000 0000 7220 0000 0072 2000 0000 729e  ....r ...r ...r.
+00002d30: 0000 0072 2100 0000 7231 0000 004b 0100  ...r!...r1...K..
+00002d40: 0073 0c00 0000 0800 0e01 0806 0c03 0a03  .s..............
+00002d50: 1029 7231 0000 0063 0000 0000 0000 0000  .)r1...c........
+00002d60: 0000 0000 0000 0000 0400 0000 0000 0000  ................
+00002d70: 7352 0000 0065 005a 0164 005a 0264 015a  sR...e.Z.d.Z.d.Z
+00002d80: 0364 1087 0066 0164 0364 0484 095a 0464  .d...f.d.d...Z.d
+00002d90: 0564 0684 005a 0587 0066 0164 0764 0884  .d...Z...f.d.d..
+00002da0: 085a 0664 0964 0a84 005a 0764 1164 0c64  .Z.d.d...Z.d.d.d
+00002db0: 0d84 015a 0864 1164 0e64 0f84 015a 0987  ...Z.d.d.d...Z..
+00002dc0: 0004 005a 0a53 0029 1272 3200 0000 7a1b  ...Z.S.).r2...z.
+00002dd0: 5265 7072 6573 656e 7473 2061 6e20 4f70  Represents an Op
+00002de0: 656e 466f 616d 206c 6973 744e 6304 0000  enFoam listNc...
+00002df0: 0000 0000 0000 0000 0004 0000 0003 0000  ................
+00002e00: 0003 0000 0073 1c00 0000 7c02 7c00 5f00  .....s....|.|._.
+00002e10: 7c03 7c00 5f01 7402 8300 a003 7c01 a101  |.|._.t.....|...
+00002e20: 0100 6400 5300 722f 0000 0029 0472 b100  ..d.S.r/...).r..
+00002e30: 0000 da06 5f64 7479 7065 729d 0000 0072  ...._dtyper....r
+00002e40: 7500 0000 2904 7243 0000 00da 0869 7465  u...).rC.....ite
+00002e50: 7261 626c 6572 4c00 0000 7264 0000 0072  rablerL...rd...r
+00002e60: 9e00 0000 7220 0000 0072 2100 0000 7275  ....r ...r!...ru
+00002e70: 0000 0088 0100 0073 0600 0000 0601 0601  .......s........
+00002e80: 1001 7a0d 4c69 7374 2e5f 5f69 6e69 745f  ..z.List.__init_
+00002e90: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+00002ea0: 0000 0100 0000 4300 0000 72b4 0000 0072  ......C...r....r
+00002eb0: 2f00 0000 72b5 0000 0072 a400 0000 7220  /...r....r....r 
+00002ec0: 0000 0072 2000 0000 7221 0000 0072 b600  ...r ...r!...r..
+00002ed0: 0000 8d01 0000 72b7 0000 007a 0d4c 6973  ......r....z.Lis
+00002ee0: 742e 6765 745f 6e61 6d65 6301 0000 0000  t.get_namec.....
+00002ef0: 0000 0000 0000 0001 0000 0002 0000 0003  ................
+00002f00: 0000 0072 b800 0000 722f 0000 0072 9c00  ...r....r/...r..
+00002f10: 0000 72a4 0000 0072 9e00 0000 7220 0000  ..r....r....r ..
+00002f20: 0072 2100 0000 7277 0000 0090 0100 0072  .r!...rw.......r
+00002f30: 9200 0000 7a0d 4c69 7374 2e5f 5f72 6570  ....z.List.__rep
+00002f40: 725f 5f63 0200 0000 0000 0000 0000 0000  r__c............
+00002f50: 0200 0000 0300 0000 0300 0000 7314 0000  ............s...
+00002f60: 0087 0087 0166 0264 0164 0284 0888 0144  .....f.d.d.....D
+00002f70: 0083 0153 0029 034e 6301 0000 0000 0000  ...S.).Nc.......
+00002f80: 0000 0000 0002 0000 0006 0000 0013 0000  ................
+00002f90: 0073 1800 0000 6700 7c00 5d08 7d01 8801  .s....g.|.].}...
+00002fa0: a000 7c01 8800 a102 9102 7102 5300 7220  ..|.......q.S.r 
+00002fb0: 0000 00a9 01da 0a5f 6475 6d70 5f69 7465  ......._dump_ite
+00002fc0: 6d29 0272 3400 0000 728f 0000 00a9 0272  m).r4...r......r
+00002fd0: 9700 0000 7243 0000 0072 2000 0000 7221  ....rC...r ...r!
+00002fe0: 0000 0072 6200 0000 9401 0000 7302 0000  ...rb.......s...
+00002ff0: 0018 007a 2b4c 6973 742e 5f6d 616b 655f  ...z+List._make_
+00003000: 6c69 7374 5f73 7472 696e 6773 2e3c 6c6f  list_strings.<lo
+00003010: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00003020: 7220 0000 0072 af00 0000 7220 0000 0072  r ...r....r ...r
+00003030: c100 0000 7221 0000 00da 125f 6d61 6b65  ....r!....._make
+00003040: 5f6c 6973 745f 7374 7269 6e67 7393 0100  _list_strings...
+00003050: 0073 0200 0000 1401 7a17 4c69 7374 2e5f  .s......z.List._
+00003060: 6d61 6b65 5f6c 6973 745f 7374 7269 6e67  make_list_string
+00003070: 7372 0100 0000 6303 0000 0000 0000 0000  sr....c.........
+00003080: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
+00003090: 3200 0000 7400 7c01 7401 7402 6602 8302  2...t.|.t.t.f...
+000030a0: 7211 7403 7c01 6401 8302 7211 7c01 a004  r.t.|.d...r.|...
+000030b0: 7c02 a101 5300 7c02 6402 1400 7405 7c01  |...S.|.d...t.|.
+000030c0: 8301 1700 5300 2903 4e72 7f00 0000 7279  ....S.).Nr....ry
+000030d0: 0000 0029 0672 3000 0000 7240 0000 0072  ...).r0...r@...r
+000030e0: 9400 0000 7281 0000 0072 7f00 0000 724e  ....r....r....rN
+000030f0: 0000 0029 0372 4300 0000 728f 0000 0072  ...).rC...r....r
+00003100: 9700 0000 7220 0000 0072 2000 0000 7221  ....r ...r ...r!
+00003110: 0000 0072 c000 0000 9601 0000 7306 0000  ...r........s...
+00003120: 0018 010a 0110 027a 0f4c 6973 742e 5f64  .......z.List._d
+00003130: 756d 705f 6974 656d 6302 0000 0000 0000  ump_itemc.......
+00003140: 0000 0000 000b 0000 0008 0000 0003 0000  ................
+00003150: 0073 7001 0000 6700 7d02 8800 6401 1400  .sp...g.}...d...
+00003160: 7d03 8801 6a00 6400 7500 721f 7c02 a001  }...j.d.u.r.|...
+00003170: 8801 6a02 6402 6403 8d01 a101 0100 7c03  ..j.d.d.......|.
+00003180: 6404 1700 6401 a003 7c02 a101 1700 6405  d...d...|.....d.
+00003190: 1700 5300 8801 6a00 7d04 8801 6a04 6400  ..S...j.}...j.d.
+000031a0: 7501 7236 7c04 6406 8801 6a04 9b00 6407  u.r6|.d...j...d.
+000031b0: 7c03 9b00 7405 8801 8301 9b00 9d05 3700  |...t.........7.
+000031c0: 7d04 7c02 a006 7c03 7c04 1700 6408 7c03  }.|...|.|...d.|.
+000031d0: 9b00 9d02 1700 6404 1700 a101 0100 6409  ......d.......d.
+000031e0: 640a 640b 9c02 7d05 8801 6a00 7c05 a007  d.d...}...j.|...
+000031f0: a100 7601 725e 7c02 a006 6408 a003 8801  ..v.r^|...d.....
+00003200: a002 8800 640c 1700 a101 a101 a101 0100  ....d...........
+00003210: 6e4e 8801 72ac 7c05 8801 6a00 1900 7d06  nN..r.|...j...}.
+00003220: 8801 6402 1900 7c06 7601 726f 7408 8801  ..d...|.v.rot...
+00003230: 8301 8201 8801 6402 1900 7d07 6700 7d08  ......d...}.g.}.
+00003240: 6400 7d09 8801 4400 5d18 7d0a 7c0a 7c07  d.}...D.].}.|.|.
+00003250: 6b02 728c 7c09 6400 7501 7288 7c08 a006  k.r.|.d.u.r.|...
+00003260: 7c09 a101 0100 7c0a 6701 7d09 7179 7c09  |.....|.g.}.qy|.
+00003270: a006 7c0a a101 0100 7179 7c08 a006 7c09  ..|.....qy|...|.
+00003280: a101 0100 8701 6601 640d 640e 8408 7c08  ......f.d.d...|.
+00003290: 4400 8301 7d08 7c02 a001 8700 6601 640f  D...}.|.....f.d.
+000032a0: 6410 8408 7c08 4400 8301 a101 0100 7c02  d...|.D.......|.
+000032b0: a006 7c03 6411 1700 a101 0100 6408 a003  ..|.d.......d...
+000032c0: 7c02 a101 5300 2912 4e72 7900 0000 7201  |...S.).Nry...r.
+000032d0: 0000 00a9 0172 9700 0000 fa01 2872 a300  .....r......(r..
+000032e0: 0000 7a13 2020 206e 6f6e 756e 6966 6f72  ..z.   nonunifor
+000032f0: 6d20 4c69 7374 3c7a 023e 0a72 7d00 0000  m List<z.>.r}...
+00003300: 2901 da03 6865 7829 055a 0673 706c 696e  )...hex).Z.splin
+00003310: 655a 0361 7263 5a08 706f 6c79 4c69 6e65  eZ.arcZ.polyLine
+00003320: 5a07 4253 706c 696e 65da 046c 696e 6529  Z.BSpline..line)
+00003330: 02da 0662 6c6f 636b 73da 0565 6467 6573  ...blocks..edges
+00003340: 7238 0000 0063 0100 0000 0000 0000 0000  r8...c..........
+00003350: 0000 0200 0000 0700 0000 1300 0000 7324  ..............s$
+00003360: 0000 0067 007c 005d 0e7d 0164 00a0 0087  ...g.|.].}.d....
+00003370: 0066 0164 0164 0284 087c 0144 0083 01a1  .f.d.d...|.D....
+00003380: 0191 0271 0253 0029 0372 7900 0000 6301  ...q.S.).ry...c.
+00003390: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+000033a0: 0000 0033 0000 0073 1a00 0000 8100 7c00  ...3...s......|.
+000033b0: 5d08 7d01 8800 a000 7c01 a101 5600 0100  ].}.....|...V...
+000033c0: 7102 6400 5300 722f 0000 0072 bf00 0000  q.d.S.r/...r....
+000033d0: 2902 7234 0000 00da 055f 6974 656d 72a4  ).r4....._itemr.
+000033e0: 0000 0072 2000 0000 7221 0000 0072 3700  ...r ...r!...r7.
+000033f0: 0000 c101 0000 725b 0000 007a 274c 6973  ......r[...z'Lis
+00003400: 742e 6475 6d70 2e3c 6c6f 6361 6c73 3e2e  t.dump.<locals>.
+00003410: 3c6c 6973 7463 6f6d 703e 2e3c 6765 6e65  <listcomp>.<gene
+00003420: 7870 723e 72ae 0000 0029 0272 3400 0000  xpr>r....).r4...
+00003430: da0a 6974 656d 735f 6c69 6e65 72a4 0000  ..items_liner...
+00003440: 0072 2000 0000 7221 0000 0072 6200 0000  .r ...r!...rb...
+00003450: c001 0000 7308 0000 0006 0002 0216 ff06  ....s...........
+00003460: ff7a 1d4c 6973 742e 6475 6d70 2e3c 6c6f  .z.List.dump.<lo
+00003470: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00003480: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00003490: 0003 0000 0033 0000 0073 2000 0000 8100  .....3...s .....
+000034a0: 7c00 5d0b 7d01 8800 6400 1700 6401 1400  |.].}...d...d...
+000034b0: 7c01 1700 5600 0100 7102 6402 5300 2903  |...V...q.d.S.).
+000034c0: 7238 0000 0072 7900 0000 4e72 2000 0000  r8...ry...Nr ...
+000034d0: 2902 7234 0000 0072 c600 0000 72c3 0000  ).r4...r....r...
+000034e0: 0072 2000 0000 7221 0000 0072 3700 0000  .r ...r!...r7...
+000034f0: c401 0000 7304 0000 0002 801e 007a 1c4c  ....s........z.L
+00003500: 6973 742e 6475 6d70 2e3c 6c6f 6361 6c73  ist.dump.<locals
+00003510: 3e2e 3c67 656e 6578 7072 3e7a 0229 3b29  >.<genexpr>z.);)
+00003520: 0972 b100 0000 da06 6578 7465 6e64 72c2  .r......extendr.
+00003530: 0000 0072 2700 0000 72bd 0000 0072 3300  ...r'...r....r3.
+00003540: 0000 7226 0000 00da 046b 6579 7372 3c00  ..r&.....keysr<.
+00003550: 0000 290b 7243 0000 0072 9700 0000 7276  ..).rC...r....rv
+00003560: 0000 0072 bb00 0000 7273 0000 005a 0d73  ...r....rs...Z.s
+00003570: 7065 6369 616c 5f6b 6579 7373 5a0c 7370  pecial_keyssZ.sp
+00003580: 6563 6961 6c5f 6b65 7973 5a0b 7370 6563  ecial_keysZ.spec
+00003590: 6961 6c5f 6b65 79da 056c 696e 6573 72ca  ial_key..linesr.
+000035a0: 0000 0072 8f00 0000 7220 0000 0072 c100  ...r....r ...r..
+000035b0: 0000 7221 0000 0072 7f00 0000 9c01 0000  ..r!...r........
+000035c0: 7350 0000 0004 0108 010a 0112 0116 0106  sP..............
+000035d0: 020a 0102 010a 0102 0102 ff06 0104 ff04  ................
+000035e0: ff1c 0502 0202 0106 fe0e 041c 0104 010a  ................
+000035f0: 010c 0108 0108 0104 0104 0108 0108 0108  ................
+00003600: 010a 0108 010c 020a 010a 0102 0206 fe18  ................
+00003610: 040e 010a 017a 094c 6973 742e 6475 6d70  .....z.List.dump
+00003620: 7293 0000 0072 9800 0000 290b 7246 0000  r....r....).rF..
+00003630: 0072 4700 0000 7248 0000 00da 075f 5f64  .rG...rH.....__d
+00003640: 6f63 5f5f 7275 0000 0072 b600 0000 7277  oc__ru...r....rw
+00003650: 0000 0072 c200 0000 72c0 0000 0072 7f00  ...r....r....r..
+00003660: 0000 72a0 0000 0072 2000 0000 7220 0000  ..r....r ...r ..
+00003670: 0072 9e00 0000 7221 0000 0072 3200 0000  .r....r!...r2...
+00003680: 8501 0000 7310 0000 0008 0004 010e 0208  ....s...........
+00003690: 050c 0308 030a 0312 0672 3200 0000 6300  .........r2...c.
+000036a0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+000036b0: 0000 0040 0000 0073 1000 0000 6500 5a01  ...@...s....e.Z.
+000036c0: 6400 5a02 6401 5a03 6402 5300 2903 72ba  d.Z.d.Z.d.S.).r.
+000036d0: 0000 007a 2241 2064 6963 7469 6f6e 6e61  ...z"A dictionna
+000036e0: 7279 2074 6f20 7374 6f72 6520 2363 6f64  ry to store #cod
+000036f0: 6553 7472 6561 6d4e 2904 7246 0000 0072  eStreamN).rF...r
+00003700: 4700 0000 7248 0000 0072 ce00 0000 7220  G...rH...r....r 
+00003710: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
+00003720: 0000 72ba 0000 00c9 0100 0073 0400 0000  ..r........s....
+00003730: 0800 0801 72ba 0000 0063 0100 0000 0000  ....r....c......
+00003740: 0000 0000 0000 0300 0000 0300 0000 0300  ................
+00003750: 0000 7322 0000 0087 0066 0164 0164 0284  ..s".....f.d.d..
+00003760: 087d 0187 0066 0164 0364 0484 087d 0274  .}...f.d.d...}.t
+00003770: 007c 017c 0283 0253 0029 054e 6301 0000  .|.|...S.).Nc...
+00003780: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00003790: 0013 0000 0073 0a00 0000 7c00 8800 1900  .....s....|.....
+000037a0: 6a00 5300 722f 0000 00a9 01da 0463 6f64  j.S.r/.......cod
+000037b0: 6572 a400 0000 725c 0000 0072 2000 0000  er....r\...r ...
+000037c0: 7221 0000 0072 5100 0000 ce01 0000 7292  r!...rQ.......r.
+000037d0: 0000 007a 185f 6d61 6b65 5f61 6c69 6173  ...z._make_alias
+000037e0: 2e3c 6c6f 6361 6c73 3e2e 6765 7463 0200  .<locals>.getc..
+000037f0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00003800: 0000 1300 0000 730e 0000 007c 017c 0088  ......s....|.|..
+00003810: 0019 005f 0064 0053 0072 2f00 0000 72cf  ..._.d.S.r/...r.
+00003820: 0000 0029 02da 055f 7365 6c66 7236 0000  ...)..._selfr6..
+00003830: 0072 5c00 0000 7220 0000 0072 2100 0000  .r\...r ...r!...
+00003840: da03 7365 74d1 0100 0072 8e00 0000 7a18  ..set....r....z.
+00003850: 5f6d 616b 655f 616c 6961 732e 3c6c 6f63  _make_alias.<loc
+00003860: 616c 733e 2e73 6574 2901 da08 7072 6f70  als>.set)...prop
+00003870: 6572 7479 2903 724c 0000 0072 5100 0000  erty).rL...rQ...
+00003880: 72d2 0000 0072 2000 0000 725c 0000 0072  r....r ...r\...r
+00003890: 2100 0000 da0b 5f6d 616b 655f 616c 6961  !....._make_alia
+000038a0: 73cd 0100 0073 0600 0000 0c01 0c03 0a03  s....s..........
+000038b0: 72d4 0000 0029 04da 0b63 6f64 6549 6e63  r....)...codeInc
+000038c0: 6c75 6465 5a0b 636f 6465 4f70 7469 6f6e  ludeZ.codeOption
+000038d0: 735a 0863 6f64 654c 6962 7372 d000 0000  sZ.codeLibsr....
+000038e0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000038f0: 0003 0000 0040 0000 0072 a100 0000 290b  .....@...r....).
+00003900: da04 436f 6465 4e63 0400 0000 0000 0000  ..CodeNc........
+00003910: 0000 0000 0400 0000 0200 0000 4300 0000  ............C...
+00003920: 731a 0000 007c 017c 005f 0074 017c 0283  s....|.|._.t.|..
+00003930: 017c 005f 027c 037c 005f 0364 0053 0072  .|._.|.|._.d.S.r
+00003940: 2f00 0000 2904 724c 0000 0072 0600 0000  /...).rL...r....
+00003950: 72d0 0000 0072 b300 0000 2904 7243 0000  r....r....).rC..
+00003960: 0072 4c00 0000 72d0 0000 0072 b300 0000  .rL...r....r....
+00003970: 7220 0000 0072 2000 0000 7221 0000 0072  r ...r ...r!...r
+00003980: 7500 0000 dc01 0000 7306 0000 0006 010a  u.......s.......
+00003990: 010a 017a 0d43 6f64 652e 5f5f 696e 6974  ...z.Code.__init
+000039a0: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
+000039b0: 0000 0005 0000 0043 0000 0073 3e00 0000  .......C...s>...
+000039c0: 7c00 6a00 6400 7500 7210 6401 7c00 6a01  |.j.d.u.r.d.|.j.
+000039d0: 6400 6402 8502 1900 9b00 6403 9d03 5300  d.d.......d...S.
+000039e0: 6401 7c00 6a01 6400 6402 8502 1900 9b00  d.|.j.d.d.......
+000039f0: 6404 7c00 6a00 9b00 6405 9d05 5300 2906  d.|.j...d...S.).
+00003a00: 4e7a 0643 6f64 6528 2272 2e00 0000 7a07  Nz.Code("r....z.
+00003a10: 5b2e 2e2e 5d22 297a 125b 2e2e 2e5d 222c  [...]")z.[...]",
+00003a20: 2064 6972 6563 7469 7665 3d72 a300 0000   directive=r....
+00003a30: 2902 72b3 0000 0072 d000 0000 72a4 0000  ).r....r....r...
+00003a40: 0072 2000 0000 7220 0000 0072 2100 0000  .r ...r ...r!...
+00003a50: 7277 0000 00e1 0100 0073 0600 0000 0a01  rw.......s......
+00003a60: 1601 1e01 7a0d 436f 6465 2e5f 5f72 6570  ....z.Code.__rep
+00003a70: 725f 5f72 0100 0000 6302 0000 0000 0000  r__r....c.......
+00003a80: 0000 0000 0007 0000 0005 0000 0043 0000  .............C..
+00003a90: 0073 8a00 0000 6700 7d02 7c01 6401 1400  .s....g.}.|.d...
+00003aa0: 7d03 7c01 6402 1700 6401 1400 7d04 7c03  }.|.d...d...}.|.
+00003ab0: 7c00 6a00 1700 7d05 7c00 6a01 6400 7501  |.j...}.|.j.d.u.
+00003ac0: 721d 7c05 6401 7c00 6a01 1700 3700 7d05  r.|.d.|.j...7.}.
+00003ad0: 7c02 a002 7c05 6403 7c03 9b00 9d02 1700  |...|.d.|.......
+00003ae0: 6404 1700 a101 0100 7c00 6a03 a004 6403  d.......|.j...d.
+00003af0: a101 4400 5d09 7d06 7c02 a002 7c04 7c06  ..D.].}.|...|.|.
+00003b00: 1700 a101 0100 712f 7c02 a002 7c03 6405  ......q/|...|.d.
+00003b10: 1700 a101 0100 6403 a005 7c02 a101 5300  ......d...|...S.
+00003b20: 2906 4e72 7900 0000 7238 0000 0072 7d00  ).Nry...r8...r}.
+00003b30: 0000 7a02 237b 7a03 237d 3b29 0672 4c00  ..z.#{z.#};).rL.
+00003b40: 0000 72b3 0000 0072 2600 0000 72d0 0000  ..r....r&...r...
+00003b50: 0072 1800 0000 7227 0000 0029 0772 4300  .r....r'...).rC.
+00003b60: 0000 7297 0000 0072 7600 0000 72bb 0000  ..r....rv...r...
+00003b70: 005a 0c69 6e64 656e 7461 7469 6f6e 3472  .Z.indentation4r
+00003b80: 1600 0000 72c6 0000 0072 2000 0000 7220  ....r....r ...r 
+00003b90: 0000 0072 2100 0000 727f 0000 00e6 0100  ...r!...r.......
+00003ba0: 0073 1600 0000 0401 0801 0c01 0a01 0a01  .s..............
+00003bb0: 0e01 1801 1001 1001 0e01 0a01 7a09 436f  ............z.Co
+00003bc0: 6465 2e64 756d 7072 2f00 0000 7298 0000  de.dumpr/...r...
+00003bd0: 00a9 0672 4600 0000 7247 0000 0072 4800  ...rF...rG...rH.
+00003be0: 0000 7275 0000 0072 7700 0000 727f 0000  ..ru...rw...r...
+00003bf0: 0072 2000 0000 7220 0000 0072 2000 0000  .r ...r ...r ...
+00003c00: 7221 0000 0072 d600 0000 db01 0000 7308  r!...r........s.
+00003c10: 0000 0008 000a 0108 050e 0572 d600 0000  ...........r....
+00003c20: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00003c30: 0003 0000 0040 0000 0072 a100 0000 290b  .....@...r....).
+00003c40: da04 4e61 6d65 4e63 0300 0000 0000 0000  ..NameNc........
+00003c50: 0000 0000 0300 0000 0200 0000 4300 0000  ............C...
+00003c60: f310 0000 007c 017c 005f 007c 027c 005f  .....|.|._.|.|._
+00003c70: 0164 0053 0072 2f00 0000 2902 724c 0000  .d.S.r/...).rL..
+00003c80: 0072 3600 0000 2903 7243 0000 0072 4c00  .r6...).rC...rL.
+00003c90: 0000 7236 0000 0072 2000 0000 7220 0000  ..r6...r ...r ..
+00003ca0: 0072 2100 0000 7275 0000 00f6 0100 00f3  .r!...ru........
+00003cb0: 0400 0000 0601 0a01 7a0d 4e61 6d65 2e5f  ........z.Name._
+00003cc0: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+00003cd0: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
+00003ce0: 730e 0000 0064 017c 006a 009b 0064 029d  s....d.|.j...d..
+00003cf0: 0353 0029 034e 7a05 4e61 6d65 2872 a300  .S.).Nz.Name(r..
+00003d00: 0000 725c 0000 0072 a400 0000 7220 0000  ..r\...r....r ..
+00003d10: 0072 2000 0000 7221 0000 0072 7700 0000  .r ...r!...rw...
+00003d20: fa01 0000 728e 0000 007a 0d4e 616d 652e  ....r....z.Name.
+00003d30: 5f5f 7265 7072 5f5f 7201 0000 0063 0200  __repr__r....c..
+00003d40: 0000 0000 0000 0000 0000 0200 0000 0100  ................
+00003d50: 0000 4300 0000 7308 0000 007c 006a 009b  ..C...s....|.j..
+00003d60: 0053 0072 2f00 0000 725c 0000 0072 af00  .S.r/...r\...r..
+00003d70: 0000 7220 0000 0072 2000 0000 7221 0000  ..r ...r ...r!..
+00003d80: 0072 7f00 0000 fd01 0000 72ac 0000 007a  .r........r....z
+00003d90: 094e 616d 652e 6475 6d70 722f 0000 0072  .Name.dumpr/...r
+00003da0: 9800 0000 72d7 0000 0072 2000 0000 7220  ....r....r ...r 
+00003db0: 0000 0072 2000 0000 7221 0000 0072 d800  ...r ...r!...r..
+00003dc0: 0000 f401 0000 7308 0000 0008 000a 0208  ......s.........
+00003dd0: 040e 0372 d800 0000 6300 0000 0000 0000  ...r....c.......
+00003de0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00003df0: 0073 2600 0000 6500 5a01 6400 5a02 6401  .s&...e.Z.d.Z.d.
+00003e00: 6402 8400 5a03 6403 6404 8400 5a04 6409  d...Z.d.d...Z.d.
+00003e10: 6406 6407 8401 5a05 6408 5300 290a da09  d.d...Z.d.S.)...
+00003e20: 4469 7265 6374 6976 6563 0300 0000 0000  Directivec......
+00003e30: 0000 0000 0000 0300 0000 0200 0000 4300  ..............C.
+00003e40: 0000 72d9 0000 0072 2f00 0000 a902 72b3  ..r....r/.....r.
+00003e50: 0000 00da 0763 6f6e 7465 6e74 2903 7243  .....content).rC
+00003e60: 0000 0072 b300 0000 72dd 0000 0072 2000  ...r....r....r .
+00003e70: 0000 7220 0000 0072 2100 0000 7275 0000  ..r ...r!...ru..
+00003e80: 0002 0200 0072 da00 0000 7a12 4469 7265  .....r....z.Dire
+00003e90: 6374 6976 652e 5f5f 696e 6974 5f5f 6301  ctive.__init__c.
+00003ea0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00003eb0: 0000 0043 0000 0073 1200 0000 7c00 6a00  ...C...s....|.j.
+00003ec0: 9b00 6401 7c00 6a01 9b00 9d03 5300 2902  ..d.|.j.....S.).
+00003ed0: 4e72 9500 0000 72dc 0000 0072 a400 0000  Nr....r....r....
+00003ee0: 7220 0000 0072 2000 0000 7221 0000 0072  r ...r ...r!...r
+00003ef0: 7700 0000 0602 0000 7302 0000 0012 017a  w.......s......z
+00003f00: 1244 6972 6563 7469 7665 2e5f 5f72 6570  .Directive.__rep
+00003f10: 725f 5f72 0100 0000 6302 0000 0000 0000  r__r....c.......
+00003f20: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
+00003f30: 0073 1c00 0000 7c01 6401 1400 7c00 6a00  .s....|.d...|.j.
+00003f40: 9b00 6402 7c00 6a01 9b00 6403 9d04 1700  ..d.|.j...d.....
+00003f50: 5300 2904 4e72 7900 0000 7295 0000 0072  S.).Nry...r....r
+00003f60: 7b00 0000 72dc 0000 0072 af00 0000 7220  {...r....r....r 
+00003f70: 0000 0072 2000 0000 7221 0000 0072 7f00  ...r ...r!...r..
+00003f80: 0000 0902 0000 72b0 0000 007a 0e44 6972  ......r....z.Dir
+00003f90: 6563 7469 7665 2e64 756d 704e 7298 0000  ective.dumpNr...
+00003fa0: 0072 d700 0000 7220 0000 0072 2000 0000  .r....r ...r ...
+00003fb0: 7220 0000 0072 2100 0000 72db 0000 0001  r ...r!...r.....
+00003fc0: 0200 0073 0800 0000 0800 0801 0804 0e03  ...s............
+00003fd0: 72db 0000 0029 0172 2e00 0000 2927 72ce  r....).r....)'r.
+00003fe0: 0000 0072 1400 0000 da03 6162 6372 0200  ...r......abcr..
+00003ff0: 0000 7203 0000 00da 0b64 6174 6163 6c61  ..r......datacla
+00004000: 7373 6573 7204 0000 00da 076e 756d 6265  ssesr......numbe
+00004010: 7273 7205 0000 00da 0874 6578 7477 7261  rsr......textwra
+00004020: 7072 0600 0000 da06 7479 7069 6e67 7207  pr......typingr.
+00004030: 0000 00da 056e 756d 7079 7266 0000 00da  .....numpyrf....
+00004040: 0a69 6e66 6c65 6374 696f 6e72 0800 0000  .inflectionr....
+00004050: 721a 0000 0072 2200 0000 722d 0000 0072  r....r"...r-...r
+00004060: 3f00 0000 7240 0000 0072 4900 0000 7270  ?...r@...rI...rp
+00004070: 0000 0072 9400 0000 729b 0000 0072 6e00  ...r....r....rn.
+00004080: 0000 7250 0000 0072 6800 0000 7253 0000  ..rP...rh...rS..
+00004090: 0072 3100 0000 7232 0000 0072 ba00 0000  .r1...r2...r....
+000040a0: 72d4 0000 0072 b100 0000 da07 7365 7461  r....r......seta
+000040b0: 7474 7272 d600 0000 72d8 0000 0072 db00  ttrr....r....r..
+000040c0: 0000 7220 0000 0072 2000 0000 7220 0000  ..r ...r ...r ..
+000040d0: 0072 2100 0000 da08 3c6d 6f64 756c 653e  .r!.....<module>
+000040e0: 0100 0000 7340 0000 0004 0008 0210 010c  ....s@..........
+000040f0: 010c 010c 010c 0108 020c 0108 0208 0308  ................
+00004100: 1b0a 120e 1110 0712 5702 4b10 0110 0e02  ........W.K.....
+00004110: 0f12 0112 2614 0f12 3a10 4408 0408 0a16  ....&...:.D.....
+00004120: 0110 0302 1912 0114 0c                   .........
```

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/constant_files.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/constant_files.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/control_dict.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/control_dict.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/decompose_par.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/decompose_par.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 07:30:57 2023 UTC, .py size: 3238 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,172 +1,215 @@
-00000000: 6f0d 0d0a 0000 0000 3132 8064 a60c 0000  o.......12.d....
+00000000: 6f0d 0d0a 0000 0000 2878 9364 7110 0000  o.......(x.dq...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
+00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
-00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6506  d.l.m.Z.m.Z...e.
-00000050: 6700 6404 a201 8301 5a07 6506 6700 6405  g.d.....Z.e.g.d.
-00000060: a201 8301 5a08 6406 6407 8400 5a09 4700  ....Z.d.d...Z.G.
-00000070: 6408 6409 8400 6409 6504 8303 5a0a 640a  d.d...d.e...Z.d.
-00000080: 5300 290b 7a27 4865 6c70 6572 2074 6f20  S.).z'Helper to 
-00000090: 6372 6561 7465 2064 6563 6f6d 706f 7365  create decompose
-000000a0: 5061 7244 6963 7420 6669 6c65 73e9 0000  ParDict files...
-000000b0: 0000 2901 da04 7072 6f64 2902 da0a 4669  ..)...prod)...Fi
-000000c0: 6c65 4865 6c70 6572 da0d 466f 616d 496e  leHelper..FoamIn
-000000d0: 7075 7446 696c 6529 03da 0673 696d 706c  putFile)...simpl
-000000e0: 65da 0673 636f 7463 68da 0c68 6965 7261  e..scotch..hiera
-000000f0: 7263 6869 6361 6c29 085a 066d 616e 7561  rchical).Z.manua
-00000100: 6c72 0500 0000 7207 0000 005a 056b 6168  lr....r....Z.kah
-00000110: 6970 5a05 6d65 7469 7372 0600 0000 5a0a  ipZ.metisr....Z.
-00000120: 7374 7275 6374 7572 6564 5a0a 6d75 6c74  structuredZ.mult
-00000130: 694c 6576 656c 6301 0000 0000 0000 0000  iLevelc.........
-00000140: 0000 0001 0000 0005 0000 0043 0000 0073  ...........C...s
-00000150: 3c00 0000 7c00 7400 7601 720e 7401 6401  <...|.t.v.r.t.d.
-00000160: 7c00 9b02 6402 7400 9b00 9d04 8301 8201  |...d.t.........
-00000170: 7c00 7402 7601 721c 7403 6401 7c00 9b02  |.t.v.r.t.d.|...
-00000180: 6403 7402 9b02 9d04 8301 8201 6400 5300  d.t.........d.S.
-00000190: 2904 4e7a 096d 6574 686f 6420 3d20 7a08  ).Nz.method = z.
-000001a0: 206e 6f74 2069 6e20 7a1c 206e 6f74 2069   not in z. not i
-000001b0: 6e20 7375 7070 6f72 7465 645f 6d65 7468  n supported_meth
-000001c0: 6f64 7320 3d20 2904 da07 6d65 7468 6f64  ods = )...method
-000001d0: 73da 0a56 616c 7565 4572 726f 72da 1173  s..ValueError..s
-000001e0: 7570 706f 7274 6564 5f6d 6574 686f 6473  upported_methods
-000001f0: da13 4e6f 7449 6d70 6c65 6d65 6e74 6564  ..NotImplemented
-00000200: 4572 726f 7229 01da 066d 6574 686f 64a9  Error)...method.
-00000210: 0072 0d00 0000 fa50 2f68 6f6d 652f 7069  .r.....P/home/pi
-00000220: 6572 7265 2f44 6576 2f66 6c75 6964 7369  erre/Dev/fluidsi
-00000230: 6d66 6f61 6d2f 7372 632f 666c 7569 6473  mfoam/src/fluids
-00000240: 696d 666f 616d 2f66 6f61 6d5f 696e 7075  imfoam/foam_inpu
-00000250: 745f 6669 6c65 732f 6465 636f 6d70 6f73  t_files/decompos
-00000260: 655f 7061 722e 7079 da0c 6368 6563 6b5f  e_par.py..check_
-00000270: 6d65 7468 6f64 1d00 0000 730a 0000 0008  method....s.....
-00000280: 0114 0108 0214 0104 ff72 0f00 0000 6300  .........r....c.
-00000290: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-000002a0: 0000 0040 0000 0073 2a00 0000 6500 5a01  ...@...s*...e.Z.
-000002b0: 6400 5a02 0901 0902 640a 6403 6404 8401  d.Z.....d.d.d...
-000002c0: 5a03 6405 6406 8400 5a04 6407 6408 8400  Z.d.d...Z.d.d...
-000002d0: 5a05 6409 5300 290b da16 4465 636f 6d70  Z.d.S.)...Decomp
-000002e0: 6f73 6550 6172 4469 6374 4865 6c70 6572  oseParDictHelper
-000002f0: e901 0000 0072 0600 0000 6303 0000 0000  .....r....c.....
-00000300: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
-00000310: 0000 0073 1800 0000 7c01 7c00 5f00 7401  ...s....|.|._.t.
-00000320: 7c02 8301 0100 7c02 7c00 5f02 6400 5300  |.....|.|._.d.S.
-00000330: 2901 4e29 03da 086e 7375 6264 6f6d 7372  ).N)...nsubdomsr
-00000340: 0f00 0000 720c 0000 0029 03da 0473 656c  ....r....)...sel
-00000350: 6672 1200 0000 720c 0000 0072 0d00 0000  fr....r....r....
-00000360: 720d 0000 0072 0e00 0000 da08 5f5f 696e  r....r......__in
-00000370: 6974 5f5f 2600 0000 7306 0000 0006 0508  it__&...s.......
-00000380: 010a 017a 1f44 6563 6f6d 706f 7365 5061  ...z.DecomposePa
-00000390: 7244 6963 7448 656c 7065 722e 5f5f 696e  rDictHelper.__in
-000003a0: 6974 5f5f 6302 0000 0000 0000 0000 0000  it__c...........
-000003b0: 0003 0000 0008 0000 0043 0000 0073 3400  .........C...s4.
-000003c0: 0000 7c01 6a00 6401 6402 7c00 6a01 6400  ..|.j.d.d.|.j.d.
-000003d0: 6403 6404 6405 9c05 6406 6407 8d03 7d02  d.d.d...d.d...}.
-000003e0: 7c02 6a00 6408 6409 6400 6901 640a 8d02  |.j.d.d.d.i.d...
-000003f0: 0100 6400 5300 290b 4eda 0870 6172 616c  ..d.S.).N..paral
-00000400: 6c65 6c72 1100 0000 da03 7879 7a67 fca9  lelr......xyzg..
-00000410: f1d2 4d62 503f 2905 7212 0000 0072 0c00  ..MbP?).r....r..
-00000420: 0000 da0c 6e73 7562 646f 6d73 5f78 797a  ....nsubdoms_xyz
-00000430: da05 6f72 6465 72da 0564 656c 7461 5a04  ..order..deltaZ.
-00000440: 544f 444f 2902 da07 6174 7472 6962 73da  TODO)...attribs.
-00000450: 0364 6f63 7206 0000 00da 0873 7472 6174  .docr......strat
-00000460: 6567 7929 0172 1a00 0000 2902 da0a 5f73  egy).r....)..._s
-00000470: 6574 5f63 6869 6c64 720c 0000 0029 0372  et_childr....).r
-00000480: 1300 0000 da06 7061 7261 6d73 da0a 7061  ......params..pa
-00000490: 725f 7061 7261 6d73 720d 0000 0072 0d00  r_paramsr....r..
-000004a0: 0000 720e 0000 00da 0f63 6f6d 706c 6574  ..r......complet
-000004b0: 655f 7061 7261 6d73 2f00 0000 7316 0000  e_params/...s...
-000004c0: 0004 0102 0102 0204 0102 0102 0102 0104  ................
-000004d0: fb02 0706 f716 0c7a 2644 6563 6f6d 706f  .......z&Decompo
-000004e0: 7365 5061 7244 6963 7448 656c 7065 722e  seParDictHelper.
-000004f0: 636f 6d70 6c65 7465 5f70 6172 616d 7363  complete_paramsc
-00000500: 0200 0000 0000 0000 0000 0000 0a00 0000  ................
-00000510: 0800 0000 4300 0000 733c 0100 007c 016a  ....C...s<...|.j
-00000520: 007d 027c 026a 017d 037c 0364 016b 0272  .}.|.j.}.|.d.k.r
-00000530: 0c64 0253 007c 026a 027d 0474 037c 0483  .d.S.|.j.}.t.|..
-00000540: 0101 0074 0464 0364 0464 0564 0664 0764  ...t.d.d.d.d.d.d
-00000550: 089c 0564 098d 017d 057c 037c 0464 0a9c  ...d...}.|.|.d..
-00000560: 027d 0664 0b7d 077c 0464 0c6b 0272 337c  .}.d.}.|.d.k.r3|
-00000570: 026a 057c 026a 067c 026a 0764 0d9c 037d  .j.|.j.|.j.d...}
-00000580: 086e 207c 0464 0e6b 0272 477c 026a 086a  .n |.d.k.rG|.j.j
-00000590: 0964 0075 0072 4064 007d 086e 1364 0f7c  .d.u.r@d.}.n.d.|
-000005a0: 026a 086a 0969 017d 086e 0c7c 0464 106b  .j.j.i.}.n.|.d.k
-000005b0: 0272 5164 117c 026a 0569 017d 086e 0274  .rQd.|.j.i.}.n.t
-000005c0: 0a82 017c 0864 0075 0172 977a 067c 0864  ...|.d.u.r.z.|.d
-000005d0: 1119 007d 0957 006e 0904 0074 0b79 6601  ...}.W.n...t.yf.
-000005e0: 0001 0001 0059 006e 2d77 007c 0964 0075  .....Y.n-w.|.d.u
-000005f0: 0072 6f74 0c64 1283 0182 0174 0d7c 0974  .rot.d.....t.|.t
-00000600: 0e83 0272 8364 1364 1484 007c 09a0 0fa1  ...r.d.d...|....
-00000610: 0064 0164 1585 0219 00a0 10a1 0044 0083  .d.d.........D..
-00000620: 017d 0974 117c 0983 017c 036b 0372 9374  .}.t.|...|.k.r.t
-00000630: 0c64 167c 099b 0264 177c 039b 029d 0483  .d.|...d.|......
-00000640: 0182 017c 087c 067c 073c 007c 05a0 127c  ...|.|.|.<.|...|
-00000650: 06a1 0101 007c 0553 0029 184e 7211 0000  .....|.S.).Nr...
-00000660: 0046 6700 0000 0000 0000 40da 0561 7363  .Fg.......@..asc
-00000670: 6969 da0a 6469 6374 696f 6e61 7279 7a08  ii..dictionaryz.
-00000680: 2273 7973 7465 6d22 da10 6465 636f 6d70  "system"..decomp
-00000690: 6f73 6550 6172 4469 6374 2905 da07 7665  oseParDict)...ve
-000006a0: 7273 696f 6eda 0666 6f72 6d61 74da 0563  rsion..format..c
-000006b0: 6c61 7373 da08 6c6f 6361 7469 6f6e da06  lass..location..
-000006c0: 6f62 6a65 6374 2901 da04 696e 666f 2902  object)...info).
-000006d0: 5a12 6e75 6d62 6572 4f66 5375 6264 6f6d  Z.numberOfSubdom
-000006e0: 6169 6e73 720c 0000 00da 0663 6f65 6666  ainsr......coeff
-000006f0: 7372 0500 0000 2903 da01 6e72 1800 0000  sr....)...nr....
-00000700: 7219 0000 0072 0600 0000 721c 0000 0072  r....r....r....r
-00000710: 0700 0000 722b 0000 007a 2470 6172 616d  ....r+...z$param
-00000720: 732e 7061 7261 6c6c 656c 2e6e 7375 6264  s.parallel.nsubd
-00000730: 6f6d 735f 7879 7a20 6973 204e 6f6e 6563  oms_xyz is Nonec
-00000740: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000750: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
-00000760: 005d 067d 0174 007c 0183 0191 0271 0253  .].}.t.|.....q.S
-00000770: 0072 0d00 0000 2901 da03 696e 7429 02da  .r....)...int)..
-00000780: 022e 30da 0477 6f72 6472 0d00 0000 720d  ..0..wordr....r.
-00000790: 0000 0072 0e00 0000 da0a 3c6c 6973 7463  ...r......<listc
-000007a0: 6f6d 703e 6f00 0000 7306 0000 0006 0008  omp>o...s.......
-000007b0: 0106 ff7a 3444 6563 6f6d 706f 7365 5061  ...z4DecomposePa
-000007c0: 7244 6963 7448 656c 7065 722e 6d61 6b65  rDictHelper.make
-000007d0: 5f74 7265 652e 3c6c 6f63 616c 733e 2e3c  _tree.<locals>.<
-000007e0: 6c69 7374 636f 6d70 3ee9 ffff ffff 7a34  listcomp>.....z4
-000007f0: 496e 636f 6e73 6973 7465 6e74 2070 6172  Inconsistent par
-00000800: 616c 6c65 6c20 7061 7261 6d65 7465 7273  allel parameters
-00000810: 3a20 7072 6f64 286e 7375 6264 6f6d 735f  : prod(nsubdoms_
-00000820: 7879 7a3d 7a0e 2920 213d 206e 7375 6264  xyz=z.) != nsubd
-00000830: 6f6d 733d 2913 7215 0000 0072 1200 0000  oms=).r....r....
-00000840: 720c 0000 0072 0f00 0000 7204 0000 0072  r....r....r....r
-00000850: 1700 0000 7218 0000 0072 1900 0000 7206  ....r....r....r.
-00000860: 0000 0072 1c00 0000 da0c 5275 6e74 696d  ...r......Runtim
-00000870: 6545 7272 6f72 da08 4b65 7945 7272 6f72  eError..KeyError
-00000880: 7209 0000 00da 0a69 7369 6e73 7461 6e63  r......isinstanc
-00000890: 65da 0373 7472 da05 7374 7269 70da 0573  e..str..strip..s
-000008a0: 706c 6974 7202 0000 00da 1469 6e69 745f  plitr......init_
-000008b0: 6672 6f6d 5f70 795f 6f62 6a65 6374 7329  from_py_objects)
-000008c0: 0a72 1300 0000 721e 0000 0072 1f00 0000  .r....r....r....
-000008d0: 7212 0000 0072 0c00 0000 da04 7472 6565  r....r......tree
-000008e0: da04 6461 7461 5a0f 6b65 795f 636f 6566  ..dataZ.key_coef
-000008f0: 6673 5f64 6963 7472 2a00 0000 7217 0000  fs_dictr*...r...
-00000900: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
-00000910: da09 6d61 6b65 5f74 7265 653e 0000 0073  ..make_tree>...s
-00000920: 6600 0000 0601 0602 0801 0401 0602 0801  f...............
-00000930: 0202 0202 0201 0201 0201 0201 04fb 06ff  ................
-00000940: 0a0a 0402 0801 0402 0401 0401 08fd 0805  ................
-00000950: 0c01 0601 0e02 0801 0c01 0402 0802 0201  ................
-00000960: 0c01 0c01 0401 02ff 0803 0801 0a02 0601  ................
-00000970: 1201 06ff 0c04 0201 0201 0201 04ff 0201  ................
-00000980: 04ff 04ff 0805 0a02 0402 7a20 4465 636f  ..........z Deco
-00000990: 6d70 6f73 6550 6172 4469 6374 4865 6c70  mposeParDictHelp
-000009a0: 6572 2e6d 616b 655f 7472 6565 4e29 0272  er.make_treeN).r
-000009b0: 1100 0000 7206 0000 0029 06da 085f 5f6e  ....r....)...__n
-000009c0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-000009d0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-000009e0: 1400 0000 7220 0000 0072 3a00 0000 720d  ....r ...r:...r.
-000009f0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000a00: 0000 7210 0000 0025 0000 0073 0c00 0000  ..r....%...s....
-00000a10: 0800 0203 0201 0afd 0809 0c0f 7210 0000  ............r...
-00000a20: 004e 290b da07 5f5f 646f 635f 5fda 046d  .N)...__doc__..m
-00000a30: 6174 6872 0200 0000 da1d 666c 7569 6473  athr......fluids
-00000a40: 696d 666f 616d 2e66 6f61 6d5f 696e 7075  imfoam.foam_inpu
-00000a50: 745f 6669 6c65 7372 0300 0000 7204 0000  t_filesr....r...
-00000a60: 00da 0373 6574 720a 0000 0072 0800 0000  ...setr....r....
-00000a70: 720f 0000 0072 1000 0000 720d 0000 0072  r....r....r....r
-00000a80: 0d00 0000 720d 0000 0072 0e00 0000 da08  ....r....r......
-00000a90: 3c6d 6f64 756c 653e 0100 0000 7316 0000  <module>....s...
-00000aa0: 0004 000c 0210 0202 0206 0104 ff02 0806  ................
-00000ab0: 0104 ff08 0e14 08                        .......
+00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
+00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
+00000060: 0100 650a 6700 6405 a201 8301 5a0b 650a  ..e.g.d.....Z.e.
+00000070: 6700 6406 a201 8301 5a0c 6407 6408 8400  g.d.....Z.d.d...
+00000080: 5a0d 4700 6409 640a 8400 640a 6506 8303  Z.G.d.d...d.e...
+00000090: 5a0e 640b 5300 290c 7a27 4865 6c70 6572  Z.d.S.).z'Helper
+000000a0: 2074 6f20 6372 6561 7465 2064 6563 6f6d   to create decom
+000000b0: 706f 7365 5061 7244 6963 7420 6669 6c65  poseParDict file
+000000c0: 73e9 0000 0000 2901 da08 6465 6570 636f  s.....)...deepco
+000000d0: 7079 2901 da04 7072 6f64 2904 da0a 4669  py)...prod)...Fi
+000000e0: 6c65 4865 6c70 6572 da0d 466f 616d 496e  leHelper..FoamIn
+000000f0: 7075 7446 696c 65da 155f 636f 6d70 6c65  putFile.._comple
+00000100: 7465 5f70 6172 616d 735f 6469 6374 da18  te_params_dict..
+00000110: 5f75 7064 6174 655f 6469 6374 5f77 6974  _update_dict_wit
+00000120: 685f 7061 7261 6d73 2903 da06 7369 6d70  h_params)...simp
+00000130: 6c65 da06 7363 6f74 6368 da0c 6869 6572  le..scotch..hier
+00000140: 6172 6368 6963 616c 2908 5a06 6d61 6e75  archical).Z.manu
+00000150: 616c 7208 0000 0072 0a00 0000 5a05 6b61  alr....r....Z.ka
+00000160: 6869 705a 056d 6574 6973 7209 0000 005a  hipZ.metisr....Z
+00000170: 0a73 7472 7563 7475 7265 645a 0a6d 756c  .structuredZ.mul
+00000180: 7469 4c65 7665 6c63 0100 0000 0000 0000  tiLevelc........
+00000190: 0000 0000 0100 0000 0500 0000 4300 0000  ............C...
+000001a0: 733c 0000 007c 0074 0076 0172 0e74 0164  s<...|.t.v.r.t.d
+000001b0: 017c 009b 0264 0274 009b 009d 0483 0182  .|...d.t........
+000001c0: 017c 0074 0276 0172 1c74 0364 017c 009b  .|.t.v.r.t.d.|..
+000001d0: 0264 0374 029b 029d 0483 0182 0164 0053  .d.t.........d.S
+000001e0: 0029 044e 7a09 6d65 7468 6f64 203d 207a  .).Nz.method = z
+000001f0: 0820 6e6f 7420 696e 207a 1c20 6e6f 7420  . not in z. not 
+00000200: 696e 2073 7570 706f 7274 6564 5f6d 6574  in supported_met
+00000210: 686f 6473 203d 2029 04da 076d 6574 686f  hods = )...metho
+00000220: 6473 da0a 5661 6c75 6545 7272 6f72 da11  ds..ValueError..
+00000230: 7375 7070 6f72 7465 645f 6d65 7468 6f64  supported_method
+00000240: 73da 134e 6f74 496d 706c 656d 656e 7465  s..NotImplemente
+00000250: 6445 7272 6f72 2901 da06 6d65 7468 6f64  dError)...method
+00000260: a900 7210 0000 00fa 502f 686f 6d65 2f70  ..r.....P/home/p
+00000270: 6965 7272 652f 4465 762f 666c 7569 6473  ierre/Dev/fluids
+00000280: 696d 666f 616d 2f73 7263 2f66 6c75 6964  imfoam/src/fluid
+00000290: 7369 6d66 6f61 6d2f 666f 616d 5f69 6e70  simfoam/foam_inp
+000002a0: 7574 5f66 696c 6573 2f64 6563 6f6d 706f  ut_files/decompo
+000002b0: 7365 5f70 6172 2e70 79da 0c63 6865 636b  se_par.py..check
+000002c0: 5f6d 6574 686f 6423 0000 0073 0a00 0000  _method#...s....
+000002d0: 0801 1401 0802 1401 04ff 7212 0000 0063  ..........r....c
+000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002f0: 0300 0000 4000 0000 733e 0000 0065 005a  ....@...s>...e.Z
+00000300: 0164 005a 0209 0109 0209 0364 0f64 0464  .d.Z.......d.d.d
+00000310: 0584 015a 0364 0664 0784 005a 0464 0864  ...Z.d.d...Z.d.d
+00000320: 0984 005a 0564 0a64 0b84 005a 0664 1064  ...Z.d.d...Z.d.d
+00000330: 0d64 0e84 015a 0764 0c53 0029 11da 1644  .d...Z.d.S.)...D
+00000340: 6563 6f6d 706f 7365 5061 7244 6963 7448  ecomposeParDictH
+00000350: 656c 7065 72e9 0100 0000 7209 0000 00da  elper.....r.....
+00000360: 0870 6172 616c 6c65 6c63 0400 0000 0000  .parallelc......
+00000370: 0000 0000 0000 0400 0000 0200 0000 4300  ..............C.
+00000380: 0000 7324 0000 007c 017c 005f 0074 017c  ..s$...|.|._.t.|
+00000390: 0283 0101 007c 027c 005f 027c 037c 005f  .....|.|._.|.|._
+000003a0: 0369 007c 005f 0464 0053 00a9 014e 2905  .i.|._.d.S...N).
+000003b0: da08 6e73 7562 646f 6d73 7212 0000 0072  ..nsubdomsr....r
+000003c0: 0f00 0000 da0d 6b65 795f 696e 5f70 6172  ......key_in_par
+000003d0: 616d 73da 0772 6567 696f 6e73 a904 da04  ams..regions....
+000003e0: 7365 6c66 7217 0000 0072 0f00 0000 7218  selfr....r....r.
+000003f0: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
+00000400: 0000 da08 5f5f 696e 6974 5f5f 2c00 0000  ....__init__,...
+00000410: 730a 0000 0006 0608 0106 0106 010a 017a  s..............z
+00000420: 1f44 6563 6f6d 706f 7365 5061 7244 6963  .DecomposeParDic
+00000430: 7448 656c 7065 722e 5f5f 696e 6974 5f5f  tHelper.__init__
+00000440: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+00000450: 0003 0000 0043 0000 0073 0e00 0000 7c02  .....C...s....|.
+00000460: 7c00 6a00 7c01 3c00 6400 5300 7216 0000  |.j.|.<.d.S.r...
+00000470: 0029 0172 1900 0000 2903 721b 0000 00da  .).r....).r.....
+00000480: 046e 616d 65da 0464 6174 6172 1000 0000  .name..datar....
+00000490: 7210 0000 0072 1100 0000 da0a 6164 645f  r....r......add_
+000004a0: 7265 6769 6f6e 3800 0000 7302 0000 000e  region8...s.....
+000004b0: 017a 2144 6563 6f6d 706f 7365 5061 7244  .z!DecomposeParD
+000004c0: 6963 7448 656c 7065 722e 6164 645f 7265  ictHelper.add_re
+000004d0: 6769 6f6e 6302 0000 0000 0000 0000 0000  gionc...........
+000004e0: 0003 0000 0008 0000 0043 0000 0073 5000  .........C...sP.
+000004f0: 0000 7c01 6a00 7c00 6a01 7c00 6a02 7c00  ..|.j.|.j.|.j.|.
+00000500: 6a03 6400 6401 6402 6403 9c05 6404 6405  j.d.d.d.d...d.d.
+00000510: 8d03 7d02 7c02 6a00 6406 6407 6400 6901  ..}.|.j.d.d.d.i.
+00000520: 6408 8d02 0100 7c00 6a04 7226 7405 7c02  d.....|.j.r&t.|.
+00000530: 6409 7c00 6a04 8303 0100 6400 5300 6400  d.|.j.....d.S.d.
+00000540: 5300 290a 4eda 0378 797a 67fc a9f1 d24d  S.).N..xyzg....M
+00000550: 6250 3f29 0572 1700 0000 720f 0000 00da  bP?).r....r.....
+00000560: 0c6e 7375 6264 6f6d 735f 7879 7ada 056f  .nsubdoms_xyz..o
+00000570: 7264 6572 da05 6465 6c74 61da 0454 4f44  rder..delta..TOD
+00000580: 4f29 02da 0761 7474 7269 6273 da03 646f  O)...attribs..do
+00000590: 6372 0900 0000 da08 7374 7261 7465 6779  cr......strategy
+000005a0: 2901 7225 0000 0072 1900 0000 2906 da0a  ).r%...r....)...
+000005b0: 5f73 6574 5f63 6869 6c64 7218 0000 0072  _set_childr....r
+000005c0: 1700 0000 720f 0000 0072 1900 0000 7206  ....r....r....r.
+000005d0: 0000 0029 0372 1b00 0000 da06 7061 7261  ...).r......para
+000005e0: 6d73 da0a 7061 725f 7061 7261 6d73 7210  ms..par_paramsr.
+000005f0: 0000 0072 1000 0000 7211 0000 00da 0f63  ...r....r......c
+00000600: 6f6d 706c 6574 655f 7061 7261 6d73 3b00  omplete_params;.
+00000610: 0000 731c 0000 0004 0104 0104 0204 0102  ..s.............
+00000620: 0102 0102 0104 fb02 0706 f712 0c06 0212  ................
+00000630: 0104 ff7a 2644 6563 6f6d 706f 7365 5061  ...z&DecomposePa
+00000640: 7244 6963 7448 656c 7065 722e 636f 6d70  rDictHelper.comp
+00000650: 6c65 7465 5f70 6172 616d 7363 0200 0000  lete_paramsc....
+00000660: 0000 0000 0000 0000 0b00 0000 0800 0000  ................
+00000670: 4300 0000 7376 0100 007c 017c 006a 0019  C...sv...|.|.j..
+00000680: 007d 027c 026a 017d 037c 0364 016b 0272  .}.|.j.}.|.d.k.r
+00000690: 0e64 0253 007c 026a 027d 0474 037c 0483  .d.S.|.j.}.t.|..
+000006a0: 0101 0074 0464 0364 0464 0564 0664 0764  ...t.d.d.d.d.d.d
+000006b0: 089c 0564 098d 017d 057c 037c 0464 0a9c  ...d...}.|.|.d..
+000006c0: 027d 0664 0b7d 077c 0464 0c6b 0272 357c  .}.d.}.|.d.k.r5|
+000006d0: 026a 057c 026a 067c 026a 0764 0d9c 037d  .j.|.j.|.j.d...}
+000006e0: 086e 207c 0464 0e6b 0272 497c 026a 086a  .n |.d.k.rI|.j.j
+000006f0: 0964 0075 0072 4264 007d 086e 1364 0f7c  .d.u.rBd.}.n.d.|
+00000700: 026a 086a 0969 017d 086e 0c7c 0464 106b  .j.j.i.}.n.|.d.k
+00000710: 0272 5364 117c 026a 0569 017d 086e 0274  .rSd.|.j.i.}.n.t
+00000720: 0a82 017c 0864 0075 0172 997a 067c 0864  ...|.d.u.r.z.|.d
+00000730: 1119 007d 0957 006e 0904 0074 0b79 6801  ...}.W.n...t.yh.
+00000740: 0001 0001 0059 006e 2d77 007c 0964 0075  .....Y.n-w.|.d.u
+00000750: 0072 7174 0c64 1283 0182 0174 0d7c 0974  .rqt.d.....t.|.t
+00000760: 0e83 0272 8564 1364 1484 007c 09a0 0fa1  ...r.d.d...|....
+00000770: 0064 0164 1585 0219 00a0 10a1 0044 0083  .d.d.........D..
+00000780: 017d 0974 117c 0983 017c 036b 0372 9574  .}.t.|...|.k.r.t
+00000790: 0c64 167c 099b 0264 177c 039b 029d 0483  .d.|...d.|......
+000007a0: 0182 017c 087c 067c 073c 007c 05a0 127c  ...|.|.|.<.|...|
+000007b0: 06a1 0101 007c 006a 1372 b974 147c 006a  .....|.j.r.t.|.j
+000007c0: 1383 017d 0a74 157c 0a7c 026a 1383 0201  ...}.t.|.|.j....
+000007d0: 007c 05a0 1664 1869 00a1 0201 007c 0564  .|...d.i.....|.d
+000007e0: 1819 00a0 127c 0aa1 0101 007c 0553 0029  .....|.....|.S.)
+000007f0: 194e 7214 0000 0046 6700 0000 0000 0000  .Nr....Fg.......
+00000800: 40da 0561 7363 6969 da0a 6469 6374 696f  @..ascii..dictio
+00000810: 6e61 7279 7a08 2273 7973 7465 6d22 5a10  naryz."system"Z.
+00000820: 6465 636f 6d70 6f73 6550 6172 4469 6374  decomposeParDict
+00000830: 2905 da07 7665 7273 696f 6eda 0666 6f72  )...version..for
+00000840: 6d61 74da 0563 6c61 7373 da08 6c6f 6361  mat..class..loca
+00000850: 7469 6f6e da06 6f62 6a65 6374 2901 da04  tion..object)...
+00000860: 696e 666f 2902 5a12 6e75 6d62 6572 4f66  info).Z.numberOf
+00000870: 5375 6264 6f6d 6169 6e73 720f 0000 00da  Subdomainsr.....
+00000880: 0663 6f65 6666 7372 0800 0000 2903 da01  .coeffsr....)...
+00000890: 6e72 2200 0000 7223 0000 0072 0900 0000  nr"...r#...r....
+000008a0: 7227 0000 0072 0a00 0000 7235 0000 007a  r'...r....r5...z
+000008b0: 2470 6172 616d 732e 7061 7261 6c6c 656c  $params.parallel
+000008c0: 2e6e 7375 6264 6f6d 735f 7879 7a20 6973  .nsubdoms_xyz is
+000008d0: 204e 6f6e 6563 0100 0000 0000 0000 0000   Nonec..........
+000008e0: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
+000008f0: 0000 0067 007c 005d 067d 0174 007c 0183  ...g.|.].}.t.|..
+00000900: 0191 0271 0253 0072 1000 0000 2901 da03  ...q.S.r....)...
+00000910: 696e 7429 02da 022e 30da 0477 6f72 6472  int)....0..wordr
+00000920: 1000 0000 7210 0000 0072 1100 0000 da0a  ....r....r......
+00000930: 3c6c 6973 7463 6f6d 703e 7e00 0000 7306  <listcomp>~...s.
+00000940: 0000 0006 0008 0106 ff7a 3444 6563 6f6d  .........z4Decom
+00000950: 706f 7365 5061 7244 6963 7448 656c 7065  poseParDictHelpe
+00000960: 722e 6d61 6b65 5f74 7265 652e 3c6c 6f63  r.make_tree.<loc
+00000970: 616c 733e 2e3c 6c69 7374 636f 6d70 3ee9  als>.<listcomp>.
+00000980: ffff ffff 7a34 496e 636f 6e73 6973 7465  ....z4Inconsiste
+00000990: 6e74 2070 6172 616c 6c65 6c20 7061 7261  nt parallel para
+000009a0: 6d65 7465 7273 3a20 7072 6f64 286e 7375  meters: prod(nsu
+000009b0: 6264 6f6d 735f 7879 7a3d 7a0e 2920 213d  bdoms_xyz=z.) !=
+000009c0: 206e 7375 6264 6f6d 733d 7219 0000 0029   nsubdoms=r....)
+000009d0: 1772 1800 0000 7217 0000 0072 0f00 0000  .r....r....r....
+000009e0: 7212 0000 0072 0500 0000 7221 0000 0072  r....r....r!...r
+000009f0: 2200 0000 7223 0000 0072 0900 0000 7227  "...r#...r....r'
+00000a00: 0000 00da 0c52 756e 7469 6d65 4572 726f  .....RuntimeErro
+00000a10: 72da 084b 6579 4572 726f 7272 0c00 0000  r..KeyErrorr....
+00000a20: da0a 6973 696e 7374 616e 6365 da03 7374  ..isinstance..st
+00000a30: 72da 0573 7472 6970 da05 7370 6c69 7472  r..strip..splitr
+00000a40: 0300 0000 da14 696e 6974 5f66 726f 6d5f  ......init_from_
+00000a50: 7079 5f6f 626a 6563 7473 7219 0000 0072  py_objectsr....r
+00000a60: 0200 0000 7207 0000 00da 0973 6574 5f63  ....r......set_c
+00000a70: 6869 6c64 290b 721b 0000 0072 2900 0000  hild).r....r)...
+00000a80: 722a 0000 0072 1700 0000 720f 0000 00da  r*...r....r.....
+00000a90: 0474 7265 6572 1e00 0000 5a0f 6b65 795f  .treer....Z.key_
+00000aa0: 636f 6566 6673 5f64 6963 7472 3400 0000  coeffs_dictr4...
+00000ab0: 7221 0000 0072 1900 0000 7210 0000 0072  r!...r....r....r
+00000ac0: 1000 0000 7211 0000 00da 096d 616b 655f  ....r......make_
+00000ad0: 7472 6565 4d00 0000 7370 0000 000a 0106  treeM...sp......
+00000ae0: 0208 0104 0106 0208 0102 0202 0202 0102  ................
+00000af0: 0102 0102 0104 fb06 ff0a 0a04 0208 0104  ................
+00000b00: 0204 0104 0108 fd08 050c 0106 010e 0208  ................
+00000b10: 010c 0104 0208 0202 010c 010c 0104 0102  ................
+00000b20: ff08 0308 010a 0206 0112 0106 ff0c 0402  ................
+00000b30: 0102 0102 0104 ff02 0104 ff04 ff08 050a  ................
+00000b40: 0206 020a 010c 010c 010e 0104 027a 2044  .............z D
+00000b50: 6563 6f6d 706f 7365 5061 7244 6963 7448  ecomposeParDictH
+00000b60: 656c 7065 722e 6d61 6b65 5f74 7265 654e  elper.make_treeN
+00000b70: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
+00000b80: 0004 0000 0043 0000 0073 3a00 0000 7c01  .....C...s:...|.
+00000b90: 6400 7500 7207 7c00 6a00 7d01 7c02 6400  d.u.r.|.j.}.|.d.
+00000ba0: 7500 720e 7c00 6a01 7d02 7c03 6400 7500  u.r.|.j.}.|.d.u.
+00000bb0: 7215 7c00 6a02 7d03 7403 7c00 8301 7c01  r.|.j.}.t.|...|.
+00000bc0: 7c02 7c03 8303 5300 7216 0000 0029 0472  |.|...S.r....).r
+00000bd0: 1700 0000 720f 0000 0072 1800 0000 da04  ....r....r......
+00000be0: 7479 7065 721a 0000 0072 1000 0000 7210  typer....r....r.
+00000bf0: 0000 0072 1100 0000 da03 6e65 7794 0000  ...r......new...
+00000c00: 0073 0e00 0000 0801 0601 0801 0601 0801  .s..............
+00000c10: 0601 1001 7a1a 4465 636f 6d70 6f73 6550  ....z.DecomposeP
+00000c20: 6172 4469 6374 4865 6c70 6572 2e6e 6577  arDictHelper.new
+00000c30: 2903 7214 0000 0072 0900 0000 7215 0000  ).r....r....r...
+00000c40: 0029 034e 4e4e 2908 da08 5f5f 6e61 6d65  .).NNN)...__name
+00000c50: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000c60: 5f5f 7175 616c 6e61 6d65 5f5f 721c 0000  __qualname__r...
+00000c70: 0072 1f00 0000 722b 0000 0072 4400 0000  .r....r+...rD...
+00000c80: 7246 0000 0072 1000 0000 7210 0000 0072  rF...r....r....r
+00000c90: 1000 0000 7211 0000 0072 1300 0000 2b00  ....r....r....+.
+00000ca0: 0000 7312 0000 0008 0002 0302 0102 010a  ..s.............
+00000cb0: fc08 0c08 0308 120e 4772 1300 0000 4e29  ........Gr....N)
+00000cc0: 0fda 075f 5f64 6f63 5f5f da04 636f 7079  ...__doc__..copy
+00000cd0: 7202 0000 00da 046d 6174 6872 0300 0000  r......mathr....
+00000ce0: da1d 666c 7569 6473 696d 666f 616d 2e66  ..fluidsimfoam.f
+00000cf0: 6f61 6d5f 696e 7075 745f 6669 6c65 7372  oam_input_filesr
+00000d00: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
+00000d10: 0000 00da 0373 6574 720d 0000 0072 0b00  .....setr....r..
+00000d20: 0000 7212 0000 0072 1300 0000 7210 0000  ..r....r....r...
+00000d30: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
+00000d40: da08 3c6d 6f64 756c 653e 0100 0000 7318  ..<module>....s.
+00000d50: 0000 0004 000c 020c 0118 0202 0706 0104  ................
+00000d60: ff02 0806 0104 ff08 0e14 08              ...........
```

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/format.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/format.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  2 09:25:03 2023 UTC, .py size: 1345 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6fb5 7964 4105 0000  o.......o.ydA...
+00000000: 6f0d 0d0a 0000 0000 2a09 8e64 cb05 0000  o.......*..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6405 6406 8400 5a07 4700  m.Z...d.d...Z.G.
 00000060: 6407 6408 8400 6408 6508 8303 5a09 640d  d.d...d.e...Z.d.
 00000070: 640b 640c 8401 5a0a 6402 5300 290e 7a1b  d.d...Z.d.S.).z.
@@ -44,48 +44,51 @@
 000002b0: 6d46 6f72 6d61 7445 7272 6f72 4e29 03da  mFormatErrorN)..
 000002c0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
 000002d0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
 000002e0: 655f 5f72 0e00 0000 720e 0000 0072 0e00  e__r....r....r..
 000002f0: 0000 720f 0000 0072 1100 0000 1700 0000  ..r....r........
 00000300: 7304 0000 0008 0004 0172 1100 0000 4654  s........r....FT
 00000310: 6303 0000 0000 0000 0000 0000 0007 0000  c...............
-00000320: 0008 0000 0043 0000 0073 8000 0000 7c01  .....C...s....|.
-00000330: 733a 7400 7c00 8301 7d03 7401 7c03 8301  s:t.|...}.t.|...
-00000340: 7d04 7c02 7238 7a06 7400 7c04 8301 7d05  }.|.r8z.t.|...}.
-00000350: 5700 6e10 0400 7402 6a03 6a04 7922 0100  W.n...t.j.j.y"..
-00000360: 0100 0100 7405 6401 7c00 9b00 9d02 8301  ....t.d.|.......
-00000370: 8201 7700 7401 7c05 8301 7d06 7c04 7c06  ..w.t.|...}.|.|.
-00000380: 6b03 7238 7406 6402 7407 7c04 7c06 8302  k.r8t.d.t.|.|...
-00000390: 1700 8301 0100 7405 6403 8301 8201 7c04  ......t.d.....|.
-000003a0: 5300 7408 7c00 8301 a001 a100 5300 2904  S.t.|.......S.).
-000003b0: 4e7a 204c 6172 6b45 7272 6f72 2077 6869  Nz LarkError whi
-000003c0: 6c65 2066 6f72 6d61 7474 696e 6720 636f  le formatting co
-000003d0: 6465 0a7a 274e 6f74 2061 626c 6520 746f  de.z'Not able to
-000003e0: 2063 6f72 7265 6374 6c79 2070 6172 7365   correctly parse
-000003f0: 2074 6869 7320 636f 6465 3a0a 7a25 4e6f   this code:.z%No
-00000400: 7420 6162 6c65 2074 6f20 636f 7272 6563  t able to correc
-00000410: 746c 7920 7061 7273 6520 7468 6973 2063  tly parse this c
-00000420: 6f64 6529 0972 0400 0000 7203 0000 00da  ode).r....r.....
-00000430: 046c 6172 6bda 0a65 7863 6570 7469 6f6e  .lark..exception
-00000440: 73da 094c 6172 6b45 7272 6f72 7211 0000  s..LarkErrorr...
-00000450: 00da 0570 7269 6e74 7210 0000 0072 0200  ...printr....r..
-00000460: 0000 2907 da04 636f 6465 5a08 6173 5f66  ..)...codeZ.as_f
-00000470: 6965 6c64 da05 6368 6563 6bda 0474 7265  ield..check..tre
-00000480: 65da 0672 6573 756c 745a 0574 7265 6531  e..resultZ.tree1
-00000490: 5a07 7265 7375 6c74 3172 0e00 0000 720e  Z.result1r....r.
-000004a0: 0000 0072 0f00 0000 da0b 666f 726d 6174  ...r......format
-000004b0: 5f63 6f64 651b 0000 0073 2600 0000 0401  _code....s&.....
-000004c0: 0801 0801 0401 0201 0c01 1001 0e01 02ff  ................
-000004d0: 0803 0802 0201 0201 0801 02ff 04ff 0804  ................
-000004e0: 0401 0c02 721d 0000 0029 0246 5429 0bda  ....r....).FT)..
-000004f0: 075f 5f64 6f63 5f5f 7215 0000 005a 2466  .__doc__r....Z$f
-00000500: 6c75 6964 7369 6d66 6f61 6d2e 666f 616d  luidsimfoam.foam
-00000510: 5f69 6e70 7574 5f66 696c 6573 2e66 6965  _input_files.fie
-00000520: 6c64 7372 0200 0000 5a24 666c 7569 6473  ldsr....Z$fluids
-00000530: 696d 666f 616d 2e66 6f61 6d5f 696e 7075  imfoam.foam_inpu
-00000540: 745f 6669 6c65 732e 7061 7273 6572 7203  t_files.parserr.
-00000550: 0000 0072 0400 0000 7210 0000 00da 0c52  ...r....r......R
-00000560: 756e 7469 6d65 4572 726f 7272 1100 0000  untimeErrorr....
-00000570: 721d 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
-00000580: 0e00 0000 720f 0000 00da 083c 6d6f 6475  ....r......<modu
-00000590: 6c65 3e01 0000 0073 0e00 0000 0400 0802  le>....s........
-000005a0: 0c02 1001 0803 100e 0e04                 ..........
+00000320: 0008 0000 0043 0000 0073 a600 0000 7c01  .....C...s....|.
+00000330: 734d 7a06 7400 7c00 8301 7d03 5700 6e10  sMz.t.|...}.W.n.
+00000340: 0400 7401 6a02 6a03 7918 0100 0100 0100  ..t.j.j.y.......
+00000350: 7404 6401 7c00 9b00 9d02 8301 8201 7700  t.d.|.........w.
+00000360: 7405 7c03 8301 7d04 7c02 724b 7a06 7400  t.|...}.|.rKz.t.
+00000370: 7c04 8301 7d05 5700 6e10 0400 7401 6a02  |...}.W.n...t.j.
+00000380: 6a03 7935 0100 0100 0100 7404 6401 7c00  j.y5......t.d.|.
+00000390: 9b00 9d02 8301 8201 7700 7405 7c05 8301  ........w.t.|...
+000003a0: 7d06 7c04 7c06 6b03 724b 7406 6402 7407  }.|.|.k.rKt.d.t.
+000003b0: 7c04 7c06 8302 1700 8301 0100 7404 6403  |.|.........t.d.
+000003c0: 8301 8201 7c04 5300 7408 7c00 8301 a005  ....|.S.t.|.....
+000003d0: a100 5300 2904 4e7a 204c 6172 6b45 7272  ..S.).Nz LarkErr
+000003e0: 6f72 2077 6869 6c65 2066 6f72 6d61 7474  or while formatt
+000003f0: 696e 6720 636f 6465 0a7a 274e 6f74 2061  ing code.z'Not a
+00000400: 626c 6520 746f 2063 6f72 7265 6374 6c79  ble to correctly
+00000410: 2070 6172 7365 2074 6869 7320 636f 6465   parse this code
+00000420: 3a0a 7a25 4e6f 7420 6162 6c65 2074 6f20  :.z%Not able to 
+00000430: 636f 7272 6563 746c 7920 7061 7273 6520  correctly parse 
+00000440: 7468 6973 2063 6f64 6529 0972 0400 0000  this code).r....
+00000450: da04 6c61 726b da0a 6578 6365 7074 696f  ..lark..exceptio
+00000460: 6e73 da09 4c61 726b 4572 726f 7272 1100  ns..LarkErrorr..
+00000470: 0000 7203 0000 00da 0570 7269 6e74 7210  ..r......printr.
+00000480: 0000 0072 0200 0000 2907 da04 636f 6465  ...r....)...code
+00000490: 5a08 6173 5f66 6965 6c64 da05 6368 6563  Z.as_field..chec
+000004a0: 6bda 0474 7265 65da 0672 6573 756c 745a  k..tree..resultZ
+000004b0: 0574 7265 6531 5a07 7265 7375 6c74 3172  .tree1Z.result1r
+000004c0: 0e00 0000 720e 0000 0072 0f00 0000 da0b  ....r....r......
+000004d0: 666f 726d 6174 5f63 6f64 651b 0000 0073  format_code....s
+000004e0: 2e00 0000 0401 0201 0c01 1001 0e01 02ff  ................
+000004f0: 0803 0401 0201 0c01 1001 0e01 02ff 0803  ................
+00000500: 0802 0201 0201 0801 02ff 04ff 0804 0401  ................
+00000510: 0c02 721d 0000 0029 0246 5429 0bda 075f  ..r....).FT)..._
+00000520: 5f64 6f63 5f5f 7215 0000 005a 2466 6c75  _doc__r....Z$flu
+00000530: 6964 7369 6d66 6f61 6d2e 666f 616d 5f69  idsimfoam.foam_i
+00000540: 6e70 7574 5f66 696c 6573 2e66 6965 6c64  nput_files.field
+00000550: 7372 0200 0000 5a24 666c 7569 6473 696d  sr....Z$fluidsim
+00000560: 666f 616d 2e66 6f61 6d5f 696e 7075 745f  foam.foam_input_
+00000570: 6669 6c65 732e 7061 7273 6572 7203 0000  files.parserr...
+00000580: 0072 0400 0000 7210 0000 00da 0c52 756e  .r....r......Run
+00000590: 7469 6d65 4572 726f 7272 1100 0000 721d  timeErrorr....r.
+000005a0: 0000 0072 0e00 0000 720e 0000 0072 0e00  ...r....r....r..
+000005b0: 0000 720f 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000005c0: 3e01 0000 0073 0e00 0000 0400 0802 0c02  >....s..........
+000005d0: 1001 0803 100e 0e04                      ........
```

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/fv_options.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/fv_options.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes_helper.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/fv_schemes_helper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/generators.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/generators.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May 23 07:52:05 2023 UTC, .py size: 5250 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a570 6c64 8214 0000  o........pld....
+00000000: 6f0d 0d0a 0000 0000 003e 9064 af14 0000  o........>.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 5a08 6401 6406 6c09 6d0a 5a0a 6d0b 5a0b  Z.d.d.l.m.Z.m.Z.
 00000070: 0100 6401 6407 6c0c 6d0d 5a0d 0100 6401  ..d.d.l.m.Z...d.
@@ -33,307 +33,305 @@
 00000200: 0000 0000 0000 0400 0000 0700 0000 4300  ..............C.
 00000210: 0000 7362 0000 007c 017c 005f 0074 0174  ..sb...|.|._.t.t
 00000220: 027c 016a 0383 0183 017d 0274 047c 026a  .|.j.....}.t.|.j
 00000230: 0583 01a0 06a1 006a 0764 011b 007c 005f  .......j.d...|._
 00000240: 0874 09a0 0a74 09a0 0b7c 026a 0c64 01a1  .t...t...|.j.d..
 00000250: 0274 09a0 0b64 0264 03a1 0267 02a1 017d  .t...d.d...g...}
 00000260: 0374 096a 0d7c 0374 096a 0e64 0464 058d  .t.j.|.t.j.d.d..
-00000270: 037c 005f 0f64 0053 0029 064e 5a09 7465  .|._.d.S.).NZ.te
+00000270: 037c 005f 0f64 0053 0029 064e da09 7465  .|._.d.S.).N..te
 00000280: 6d70 6c61 7465 73da 0c66 6c75 6964 7369  mplates..fluidsi
-00000290: 6d66 6f61 6d5a 0972 6573 6f75 7263 6573  mfoamZ.resources
+00000290: 6d66 6f61 6dda 0972 6573 6f75 7263 6573  mfoam..resources
 000002a0: 5429 03da 066c 6f61 6465 72da 0975 6e64  T)...loader..und
 000002b0: 6566 696e 6564 5a15 6b65 6570 5f74 7261  efinedZ.keep_tra
 000002c0: 696c 696e 675f 6e65 776c 696e 6529 10da  iling_newline)..
 000002d0: 066f 7574 7075 7472 0400 0000 da04 7479  .outputr......ty
 000002e0: 7065 da03 7369 6d72 0500 0000 da08 5f5f  pe..simr......__
 000002f0: 6669 6c65 5f5f da08 6162 736f 6c75 7465  file__..absolute
 00000300: da06 7061 7265 6e74 da0d 7465 6d70 6c61  ..parent..templa
 00000310: 7465 735f 6469 72da 066a 696e 6a61 325a  tes_dir..jinja2Z
 00000320: 0c43 686f 6963 654c 6f61 6465 725a 0d50  .ChoiceLoaderZ.P
 00000330: 6163 6b61 6765 4c6f 6164 6572 da0b 5f5f  ackageLoader..__
 00000340: 7061 636b 6167 655f 5f5a 0b45 6e76 6972  package__Z.Envir
 00000350: 6f6e 6d65 6e74 5a0f 5374 7269 6374 556e  onmentZ.StrictUn
 00000360: 6465 6669 6e65 64da 096a 696e 6a61 5f65  defined..jinja_e
-00000370: 6e76 2904 da04 7365 6c66 7210 0000 00da  nv)...selfr.....
-00000380: 036d 6f64 720e 0000 00a9 0072 1c00 0000  .modr......r....
+00000370: 6e76 2904 da04 7365 6c66 7212 0000 00da  nv)...selfr.....
+00000380: 036d 6f64 7210 0000 00a9 0072 1e00 0000  .modr......r....
 00000390: fa4d 2f68 6f6d 652f 7069 6572 7265 2f44  .M/home/pierre/D
 000003a0: 6576 2f66 6c75 6964 7369 6d66 6f61 6d2f  ev/fluidsimfoam/
 000003b0: 7372 632f 666c 7569 6473 696d 666f 616d  src/fluidsimfoam
 000003c0: 2f66 6f61 6d5f 696e 7075 745f 6669 6c65  /foam_input_file
 000003d0: 732f 6765 6e65 7261 746f 7273 2e70 79da  s/generators.py.
 000003e0: 085f 5f69 6e69 745f 5f11 0000 0073 1a00  .__init__....s..
 000003f0: 0000 0601 0e01 1601 0402 0c02 0a01 02fe  ................
 00000400: 04ff 0407 0201 0401 0201 0cfd 7a13 496e  ............z.In
 00000410: 7075 7446 696c 6573 2e5f 5f69 6e69 745f  putFiles.__init_
 00000420: 5f63 0200 0000 0000 0000 0000 0000 0200  _c..............
 00000430: 0000 0300 0000 4300 0000 730c 0000 007c  ......C...s....|
 00000440: 006a 00a0 017c 01a1 0153 00a9 014e 2902  .j...|...S...N).
-00000450: 7219 0000 00da 0c67 6574 5f74 656d 706c  r......get_templ
-00000460: 6174 6529 0272 1a00 0000 da0d 7465 6d70  ate).r......temp
-00000470: 6c61 7465 5f6e 616d 6572 1c00 0000 721c  late_namer....r.
-00000480: 0000 0072 1d00 0000 7220 0000 0023 0000  ...r....r ...#..
+00000450: 721b 0000 00da 0c67 6574 5f74 656d 706c  r......get_templ
+00000460: 6174 6529 0272 1c00 0000 da0d 7465 6d70  ate).r......temp
+00000470: 6c61 7465 5f6e 616d 6572 1e00 0000 721e  late_namer....r.
+00000480: 0000 0072 1f00 0000 7222 0000 0023 0000  ...r....r"...#..
 00000490: 0073 0200 0000 0c01 7a17 496e 7075 7446  .s......z.InputF
 000004a0: 696c 6573 2e67 6574 5f74 656d 706c 6174  iles.get_templat
 000004b0: 654e 2906 da08 5f5f 6e61 6d65 5f5f da0a  eN)...__name__..
 000004c0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
 000004d0: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-000004e0: 5f72 1e00 0000 7220 0000 0072 1c00 0000  _r....r ...r....
-000004f0: 721c 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
+000004e0: 5f72 2000 0000 7222 0000 0072 1e00 0000  _r ...r"...r....
+000004f0: 721e 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
 00000500: 0c00 0000 0e00 0000 7308 0000 0008 0004  ........s.......
 00000510: 0108 020c 1272 0c00 0000 6300 0000 0000  .....r....c.....
 00000520: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
 00000530: 0000 0073 4400 0000 6500 5a01 6400 5a02  ...sD...e.Z.d.Z.
 00000540: 5500 6503 6504 6401 3c00 6402 6403 8400  U.e.e.d.<.d.d...
 00000550: 5a05 640d 6405 6406 8401 5a06 6507 6407  Z.d.d.d...Z.e.d.
 00000560: 6408 8400 8301 5a08 6409 640a 8400 5a09  d.....Z.d.d...Z.
 00000570: 640b 640c 8400 5a0a 6404 5300 290e da10  d.d...Z.d.S.)...
 00000580: 4669 6c65 4765 6e65 7261 746f 7241 4243  FileGeneratorABC
 00000590: da08 7265 6c5f 7061 7468 6302 0000 0000  ..rel_pathc.....
 000005a0: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
 000005b0: 0000 0073 1200 0000 7c01 7c00 5f00 7c01  ...s....|.|._.|.
-000005c0: 6a01 7c00 5f01 6400 5300 721f 0000 0029  j.|._.d.S.r....)
-000005d0: 0272 1000 0000 da0b 696e 7075 745f 6669  .r......input_fi
-000005e0: 6c65 73a9 0272 1a00 0000 7210 0000 0072  les..r....r....r
-000005f0: 1c00 0000 721c 0000 0072 1d00 0000 721e  ....r....r....r.
+000005c0: 6a01 7c00 5f01 6400 5300 7221 0000 0029  j.|._.d.S.r!...)
+000005d0: 0272 1200 0000 da0b 696e 7075 745f 6669  .r......input_fi
+000005e0: 6c65 73a9 0272 1c00 0000 7212 0000 0072  les..r....r....r
+000005f0: 1e00 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
 00000600: 0000 002a 0000 0073 0400 0000 0601 0c01  ...*...s........
 00000610: 7a19 4669 6c65 4765 6e65 7261 746f 7241  z.FileGeneratorA
 00000620: 4243 2e5f 5f69 6e69 745f 5f4e 6302 0000  BC.__init__Nc...
-00000630: 0000 0000 0000 0000 0004 0000 0008 0000  ................
-00000640: 0043 0000 0073 6c00 0000 7c01 6401 7500  .C...sl...|.d.u.
+00000630: 0000 0000 0000 0000 0004 0000 0003 0000  ................
+00000640: 0043 0000 0073 5200 0000 7c01 6401 7500  .C...sR...|.d.u.
 00000650: 7209 7c00 6a00 6a01 6a02 7d01 7c00 a003  r.|.j.j.j.}.|...
 00000660: 7c01 a101 7d02 7c02 6402 7500 7214 6401  |...}.|.d.u.r.d.
-00000670: 5300 7404 7c00 6a00 6a05 7c00 6a06 1b00  S.t.|.j.j.|.j...
-00000680: 6403 8302 8f0e 7d03 7c03 a007 7c02 a101  d.....}.|...|...
-00000690: 0100 5700 6401 0400 0400 8303 0100 6401  ..W.d.........d.
-000006a0: 5300 3100 732f 7701 0100 0100 0100 5900  S.1.s/w.......Y.
-000006b0: 0100 6401 5300 2904 7a11 4765 6e65 7261  ..d.S.).z.Genera
-000006c0: 7465 2074 6865 2066 696c 654e 46da 0177  te the fileNF..w
-000006d0: 2908 7210 0000 0072 1200 0000 da06 7061  ).r....r......pa
-000006e0: 7261 6d73 da0d 6765 6e65 7261 7465 5f63  rams..generate_c
-000006f0: 6f64 65da 046f 7065 6eda 0870 6174 685f  ode..open..path_
-00000700: 7275 6e72 2700 0000 da05 7772 6974 6529  runr'.....write)
-00000710: 0472 1a00 0000 722b 0000 00da 0463 6f64  .r....r+.....cod
-00000720: 65da 0466 696c 6572 1c00 0000 721c 0000  e..filer....r...
-00000730: 0072 1d00 0000 da0d 6765 6e65 7261 7465  .r......generate
-00000740: 5f66 696c 652e 0000 0073 1000 0000 0802  _file....s......
-00000750: 0a01 0a02 0801 0401 1602 0c01 22ff 7a1e  ............".z.
-00000760: 4669 6c65 4765 6e65 7261 746f 7241 4243  FileGeneratorABC
-00000770: 2e67 656e 6572 6174 655f 6669 6c65 6301  .generate_filec.
-00000780: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00000790: 0000 0043 0000 0073 0400 0000 6401 5300  ...C...s....d.S.
-000007a0: 2902 7a1d 4765 6e65 7261 7465 2074 6865  ).z.Generate the
-000007b0: 2063 6f64 6520 6f66 2074 6865 2066 696c   code of the fil
-000007c0: 654e 721c 0000 00a9 0172 1a00 0000 721c  eNr......r....r.
-000007d0: 0000 0072 1c00 0000 721d 0000 0072 2c00  ...r....r....r,.
-000007e0: 0000 3a00 0000 7302 0000 0004 007a 1e46  ..:...s......z.F
-000007f0: 696c 6547 656e 6572 6174 6f72 4142 432e  ileGeneratorABC.
-00000800: 6765 6e65 7261 7465 5f63 6f64 6563 0100  generate_codec..
-00000810: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00000820: 0000 0300 0000 7342 0000 0088 006a 006a  ......sB.....j.j
-00000830: 0188 006a 021b 007d 0174 0387 0066 0164  ...j...}.t...f.d
-00000840: 0164 0284 0864 0344 0083 0183 0172 1d74  .d...d.D.....r.t
-00000850: 047c 01a0 05a1 0083 017d 027c 017c 025f  .|.......}.|.|._
-00000860: 067c 0253 0074 077c 0183 0153 0029 044e  .|.S.t.|...S.).N
-00000870: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000880: 0004 0000 0033 0000 0073 1c00 0000 8100  .....3...s......
-00000890: 7c00 5d09 7d01 8800 6a00 a001 7c01 a101  |.].}...j...|...
-000008a0: 5600 0100 7102 6400 5300 721f 0000 0029  V...q.d.S.r....)
-000008b0: 0272 2700 0000 da0a 7374 6172 7473 7769  .r'.....startswi
-000008c0: 7468 2902 da02 2e30 da05 7374 6172 7472  th)....0..startr
-000008d0: 3300 0000 721c 0000 0072 1d00 0000 da09  3...r....r......
-000008e0: 3c67 656e 6578 7072 3e40 0000 0073 0800  <genexpr>@...s..
-000008f0: 0000 0280 0400 0c01 0aff 7a28 4669 6c65  ..........z(File
-00000900: 4765 6e65 7261 746f 7241 4243 2e72 6561  GeneratorABC.rea
-00000910: 642e 3c6c 6f63 616c 733e 2e3c 6765 6e65  d.<locals>.<gene
-00000920: 7870 723e 2902 da06 7379 7374 656d da08  xpr>)...system..
-00000930: 636f 6e73 7461 6e74 2908 7210 0000 0072  constant).r....r
-00000940: 2e00 0000 7227 0000 00da 0361 6e79 720a  ....r'.....anyr.
-00000950: 0000 00da 0972 6561 645f 7465 7874 da04  .....read_text..
-00000960: 7061 7468 720b 0000 0029 0372 1a00 0000  pathr....).r....
-00000970: 723c 0000 00da 0474 7265 6572 1c00 0000  r<.....treer....
-00000980: 7233 0000 0072 1d00 0000 da04 7265 6164  r3...r......read
-00000990: 3e00 0000 7310 0000 000e 010c 0102 0108  >...s...........
-000009a0: ff0c 0306 0104 0108 027a 1546 696c 6547  .........z.FileG
-000009b0: 656e 6572 6174 6f72 4142 432e 7265 6164  eneratorABC.read
-000009c0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-000009d0: 0008 0000 0043 0000 0073 4800 0000 7400  .....C...sH...t.
-000009e0: 7c00 6a01 6a02 7c00 6a03 1b00 6401 8302  |.j.j.|.j...d...
-000009f0: 8f10 7d02 7c02 a004 7c01 a005 a100 a101  ..}.|...|.......
-00000a00: 0100 5700 6400 0400 0400 8303 0100 6400  ..W.d.........d.
-00000a10: 5300 3100 731d 7701 0100 0100 0100 5900  S.1.s.w.......Y.
-00000a20: 0100 6400 5300 2902 4e72 2a00 0000 2906  ..d.S.).Nr*...).
-00000a30: 722d 0000 0072 1000 0000 722e 0000 0072  r-...r....r....r
-00000a40: 2700 0000 722f 0000 00da 0464 756d 7029  '...r/.....dump)
-00000a50: 0372 1a00 0000 5a08 6475 6d70 6162 6c65  .r....Z.dumpable
-00000a60: 7231 0000 0072 1c00 0000 721c 0000 0072  r1...r....r....r
-00000a70: 1d00 0000 da09 6f76 6572 7772 6974 6549  ......overwriteI
-00000a80: 0000 0073 0600 0000 1601 1001 22ff 7a1a  ...s........".z.
-00000a90: 4669 6c65 4765 6e65 7261 746f 7241 4243  FileGeneratorABC
-00000aa0: 2e6f 7665 7277 7269 7465 721f 0000 0029  .overwriter....)
-00000ab0: 0b72 2200 0000 7223 0000 0072 2400 0000  .r"...r#...r$...
-00000ac0: da03 7374 72da 0f5f 5f61 6e6e 6f74 6174  ..str..__annotat
-00000ad0: 696f 6e73 5f5f 721e 0000 0072 3200 0000  ions__r....r2...
-00000ae0: 7203 0000 0072 2c00 0000 723e 0000 0072  r....r,...r>...r
-00000af0: 4000 0000 721c 0000 0072 1c00 0000 721c  @...r....r....r.
-00000b00: 0000 0072 1d00 0000 7226 0000 0027 0000  ...r....r&...'..
-00000b10: 0073 1000 0000 0a00 0801 0802 0a04 020c  .s..............
-00000b20: 0a01 0803 0c0b 7226 0000 0063 0000 0000  ......r&...c....
-00000b30: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000b40: 0000 0000 733c 0000 0065 005a 0164 005a  ....s<...e.Z.d.Z
-00000b50: 0255 0065 0365 0464 013c 0087 0066 0164  .U.e.e.d.<...f.d
-00000b60: 0264 0384 085a 0564 0964 0564 0684 015a  .d...Z.d.d.d...Z
-00000b70: 0665 0764 0764 0884 0083 015a 0887 0004  .e.d.d.....Z....
-00000b80: 005a 0953 0029 0ada 0d46 696c 6547 656e  .Z.S.)...FileGen
-00000b90: 6572 6174 6f72 7221 0000 0063 0200 0000  eratorr!...c....
-00000ba0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00000bb0: 0300 0000 7310 0000 0074 0083 00a0 017c  ....s....t.....|
-00000bc0: 01a1 0101 0064 0053 0072 1f00 0000 2902  .....d.S.r....).
-00000bd0: da05 7375 7065 7272 1e00 0000 7229 0000  ..superr....r)..
-00000be0: 00a9 01da 095f 5f63 6c61 7373 5f5f 721c  .....__class__r.
-00000bf0: 0000 0072 1d00 0000 721e 0000 0051 0000  ...r....r....Q..
-00000c00: 0073 0200 0000 1001 7a16 4669 6c65 4765  .s......z.FileGe
-00000c10: 6e65 7261 746f 722e 5f5f 696e 6974 5f5f  nerator.__init__
-00000c20: 4e63 0200 0000 0000 0000 0000 0000 0500  Nc..............
-00000c30: 0000 0800 0000 0300 0000 732c 0100 007c  ..........s,...|
-00000c40: 0164 0175 0072 097c 006a 006a 016a 027d  .d.u.r.|.j.j.j.}
-00000c50: 017a 0b74 037c 006a 0064 027c 006a 0417  .z.t.|.j.d.|.j..
-00000c60: 0083 027d 0257 006e 0b04 0074 0579 1f01  ...}.W.n...t.y..
-00000c70: 0001 0001 0064 017d 0259 006e 0177 007c  .....d.}.Y.n.w.|
-00000c80: 0264 0175 0072 667a 0b74 037c 006a 0064  .d.u.rfz.t.|.j.d
-00000c90: 037c 006a 0417 0083 0289 0057 006e 0b04  .|.j.......W.n..
-00000ca0: 0074 0579 3a01 0001 0001 0064 0189 0059  .t.y:......d...Y
-00000cb0: 006e 0177 0088 0064 0175 0072 5c7a 0b74  .n.w...d.u.r\z.t
-00000cc0: 037c 006a 0064 047c 006a 0417 0083 027d  .|.j.d.|.j.....}
-00000cd0: 0357 006e 0904 0074 0579 5301 0001 0001  .W.n...t.yS.....
-00000ce0: 0059 006e 0977 0074 067c 0374 0783 0272  .Y.n.w.t.|.t...r
-00000cf0: 5c7c 036a 0889 0088 0064 0175 0172 6687  \|.j.....d.u.rf.
-00000d00: 0066 0164 0564 0684 087d 027c 0264 0175  .f.d.d...}.|.d.u
-00000d10: 0072 777c 006a 09a0 0a7c 006a 0ba1 017d  .rw|.j...|.j...}
-00000d20: 047c 046a 0c7c 0164 078d 0153 007c 006a  .|.j.|.d...S.|.j
-00000d30: 096a 0d7c 006a 0b1b 00a0 0ea1 0072 9274  .j.|.j.......r.t
-00000d40: 0f64 087c 006a 109b 0064 097c 006a 096a  .d.|.j...d.|.j.j
-00000d50: 0d9b 0064 0a7c 006a 049b 0064 0b9d 0783  ...d.|.j...d....
-00000d60: 0182 017c 027c 0183 0153 0029 0c7a 9647  ...|.|...S.).z.G
-00000d70: 656e 6572 6174 6520 7468 6520 636f 6465  enerate the code
-00000d80: 206f 6620 7468 6520 6669 6c65 2066 726f   of the file fro
-00000d90: 6d20 2e2e 2e0a 0a20 2020 2020 2020 202d  m .....        -
-00000da0: 2061 206d 6574 686f 6420 6e61 6d65 6420   a method named 
-00000db0: 6c69 6b65 2060 7369 6d2e 6f75 7470 7574  like `sim.output
-00000dc0: 2e5f 6d61 6b65 5f63 6f64 655f 626c 6f63  ._make_code_bloc
-00000dd0: 6b5f 6d65 7368 5f64 6963 7460 2c0a 2020  k_mesh_dict`,.  
-00000de0: 2020 2020 2020 2d20 6f72 2061 204a 696e        - or a Jin
-00000df0: 6a61 2074 656d 706c 6174 652e 0a20 2020  ja template..   
-00000e00: 2020 2020 204e 5a0b 5f6d 616b 655f 636f       NZ._make_co
-00000e10: 6465 5f5a 0b5f 6d61 6b65 5f74 7265 655f  de_Z._make_tree_
-00000e20: da08 5f68 656c 7065 725f 6301 0000 0000  .._helper_c.....
-00000e30: 0000 0000 0000 0002 0000 0002 0000 0013  ................
-00000e40: 0000 0073 1c00 0000 8800 7c00 8301 7d01  ...s......|...}.
-00000e50: 7c01 6401 7500 720a 6401 5300 7c01 a000  |.d.u.r.d.S.|...
-00000e60: a100 5300 2902 4e46 2901 723f 0000 0029  ..S.).NF).r?...)
-00000e70: 025a 0770 6172 616d 735f 723d 0000 00a9  .Z.params_r=....
-00000e80: 01da 096d 616b 655f 7472 6565 721c 0000  ...make_treer...
-00000e90: 0072 1d00 0000 da09 6d61 6b65 5f63 6f64  .r......make_cod
-00000ea0: 6573 0000 0073 0800 0000 0801 0801 0401  es...s..........
-00000eb0: 0801 7a2e 4669 6c65 4765 6e65 7261 746f  ..z.FileGenerato
-00000ec0: 722e 6765 6e65 7261 7465 5f63 6f64 652e  r.generate_code.
-00000ed0: 3c6c 6f63 616c 733e 2e6d 616b 655f 636f  <locals>.make_co
-00000ee0: 6465 2901 722b 0000 007a 3b46 6c75 6964  de).r+...z;Fluid
-00000ef0: 7369 6d66 6f61 6d20 736f 6c76 6572 2069  simfoam solver i
-00000f00: 7373 7565 3a20 3220 636f 6e63 7572 7265  ssue: 2 concurre
-00000f10: 6e74 206d 6574 686f 6473 2074 6f20 7072  nt methods to pr
-00000f20: 6f64 7563 6520 7a10 3a0a 2d20 7465 6d70  oduce z.:.- temp
-00000f30: 6c61 7465 2069 6e20 7a1f 2c0a 2d20 6675  late in z.,.- fu
-00000f40: 6e63 7469 6f6e 206f 7574 7075 742e 5f6d  nction output._m
-00000f50: 616b 655f 636f 6465 5f7a 3d2e 0a52 656d  ake_code_z=..Rem
-00000f60: 6f76 6520 7468 6520 6669 6c65 206f 7220  ove the file or 
-00000f70: 7468 6520 6675 6e63 7469 6f6e 2028 6f72  the function (or
-00000f80: 206d 616b 6520 6974 2065 7175 616c 2074   make it equal t
-00000f90: 6f20 4e6f 6e65 292e 2911 7210 0000 0072  o None).).r....r
-00000fa0: 1200 0000 722b 0000 00da 0767 6574 6174  ....r+.....getat
-00000fb0: 7472 da05 5f6e 616d 65da 0e41 7474 7269  tr.._name..Attri
-00000fc0: 6275 7465 4572 726f 72da 0a69 7369 6e73  buteError..isins
-00000fd0: 7461 6e63 6572 0900 0000 7249 0000 0072  tancer....rI...r
-00000fe0: 2800 0000 7220 0000 0072 2100 0000 da06  (...r ...r!.....
-00000ff0: 7265 6e64 6572 7216 0000 00da 0665 7869  renderr......exi
-00001000: 7374 73da 0c52 756e 7469 6d65 4572 726f  sts..RuntimeErro
-00001010: 7272 2700 0000 2905 721a 0000 0072 2b00  rr'...).r....r+.
-00001020: 0000 724a 0000 00da 0668 656c 7065 72da  ..rJ.....helper.
-00001030: 0874 656d 706c 6174 6572 1c00 0000 7248  .templater....rH
-00001040: 0000 0072 1d00 0000 722c 0000 0054 0000  ...r....r,...T..
-00001050: 0073 4a00 0000 0806 0a01 0202 1601 0c01  .sJ.............
-00001060: 0801 02ff 0803 0201 1601 0c01 0801 02ff  ................
-00001070: 0803 0201 1601 0c01 0401 02ff 0a03 0601  ................
-00001080: 0802 0c02 0806 0e01 0c01 1202 0201 0201  ................
-00001090: 0401 04ff 0602 04fe 0403 06fd 04ff 0808  ................
-000010a0: 7a1b 4669 6c65 4765 6e65 7261 746f 722e  z.FileGenerator.
-000010b0: 6765 6e65 7261 7465 5f63 6f64 6563 0300  generate_codec..
-000010c0: 0000 0000 0000 0000 0000 0600 0000 0800  ................
-000010d0: 0000 4300 0000 739a 0000 0074 007c 026a  ..C...s....t.|.j
-000010e0: 016a 026a 037c 026a 016a 026a 0483 027d  .j.j.|.j.j.j...}
-000010f0: 037a 0a74 057c 0364 017c 006a 0617 0083  .z.t.|.d.|.j....
-00001100: 027d 0457 006e 0b04 0074 0779 2001 0001  .}.W.n...t.y ...
-00001110: 0001 0064 007d 0459 006e 0177 007c 0464  ...d.}.Y.n.w.|.d
-00001120: 0075 0072 417a 0a74 057c 0364 027c 006a  .u.rAz.t.|.d.|.j
-00001130: 0617 0083 027d 0557 006e 0904 0074 0779  .....}.W.n...t.y
-00001140: 3801 0001 0001 0059 006e 0977 0074 087c  8......Y.n.w.t.|
-00001150: 0574 0983 0272 417c 056a 0a7d 047c 0464  .t...rA|.j.}.|.d
-00001160: 0075 0172 4b7c 047c 0183 0101 0064 0053  .u.rK|.|.....d.S
-00001170: 0064 0053 0029 034e 5a11 5f63 6f6d 706c  .d.S.).NZ._compl
-00001180: 6574 655f 7061 7261 6d73 5f72 4700 0000  ete_params_rG...
-00001190: 290b 7208 0000 00da 0763 6c61 7373 6573  ).r......classes
-000011a0: da06 4f75 7470 7574 da0b 6d6f 6475 6c65  ..Output..module
-000011b0: 5f6e 616d 65da 0a63 6c61 7373 5f6e 616d  _name..class_nam
-000011c0: 6572 4b00 0000 724c 0000 0072 4d00 0000  erK...rL...rM...
-000011d0: 724e 0000 0072 0900 0000 da0f 636f 6d70  rN...r......comp
-000011e0: 6c65 7465 5f70 6172 616d 7329 06da 0363  lete_params)...c
-000011f0: 6c73 722b 0000 00da 0b69 6e66 6f5f 736f  lsr+.....info_so
-00001200: 6c76 6572 5a0a 6f75 7470 7574 5f63 6c73  lverZ.output_cls
-00001210: 7258 0000 0072 5200 0000 721c 0000 0072  rX...rR...r....r
-00001220: 1c00 0000 721d 0000 00da 1d5f 636f 6d70  ....r......_comp
-00001230: 6c65 7465 5f70 6172 616d 735f 7769 7468  lete_params_with
-00001240: 5f64 6566 6175 6c74 8800 0000 7328 0000  _default....s(..
-00001250: 0002 0208 0108 0104 fe02 0414 010c 0108  ................
-00001260: 0102 ff08 0302 0114 010c 0104 0102 ff0a  ................
-00001270: 0306 0108 020c 0104 ff7a 2b46 696c 6547  .........z+FileG
-00001280: 656e 6572 6174 6f72 2e5f 636f 6d70 6c65  enerator._comple
-00001290: 7465 5f70 6172 616d 735f 7769 7468 5f64  te_params_with_d
-000012a0: 6566 6175 6c74 721f 0000 0029 0a72 2200  efaultr....).r".
-000012b0: 0000 7223 0000 0072 2400 0000 7241 0000  ..r#...r$...rA..
-000012c0: 0072 4200 0000 721e 0000 0072 2c00 0000  .rB...r....r,...
-000012d0: da0b 636c 6173 736d 6574 686f 6472 5b00  ..classmethodr[.
-000012e0: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
-000012f0: 5f72 1c00 0000 721c 0000 0072 4500 0000  _r....r....rE...
-00001300: 721d 0000 0072 4300 0000 4e00 0000 730c  r....rC...N...s.
-00001310: 0000 000a 0008 010c 020a 0302 3412 0172  ............4..r
-00001320: 4300 0000 da01 3063 0200 0000 0000 0000  C.....0c........
-00001330: 0000 0000 0300 0000 0b00 0000 4300 0000  ............C...
-00001340: 7342 0000 0064 0174 007c 0083 019b 009d  sB...d.t.|......
-00001350: 027d 0274 017c 0274 0266 017c 017c 019b  .}.t.|.t.f.|.|..
-00001360: 0064 027c 009b 009d 037c 009b 0064 039d  .d.|.....|...d..
-00001370: 0274 037c 00a0 0464 0464 05a1 0283 0164  .t.|...d.d.....d
-00001380: 069c 0483 0353 0029 074e 7243 0000 00fa  .....S.).NrC....
-00001390: 012f 7a06 2e6a 696e 6a61 da01 2eda 015f  ./z..jinja....._
-000013a0: 2904 da08 6469 725f 6e61 6d65 7227 0000  )...dir_namer'..
-000013b0: 0072 2100 0000 724c 0000 0029 0572 0600  .r!...rL...).r..
-000013c0: 0000 7211 0000 0072 4300 0000 7207 0000  ..r....rC...r...
-000013d0: 00da 0772 6570 6c61 6365 2903 da09 6669  ...replace)...fi
-000013e0: 6c65 5f6e 616d 6572 6200 0000 da08 636c  le_namerb.....cl
-000013f0: 735f 6e61 6d65 721c 0000 0072 1c00 0000  s_namer....r....
-00001400: 721d 0000 00da 186e 6577 5f66 696c 655f  r......new_file_
-00001410: 6765 6e65 7261 746f 725f 636c 6173 73a0  generator_class.
-00001420: 0000 0073 1400 0000 0e01 0201 0201 0401  ...s............
-00001430: 0202 0c01 0801 0e01 04fc 04fd 7266 0000  ............rf..
-00001440: 0029 0172 5e00 0000 2916 7225 0000 00da  .).r^...).r%....
-00001450: 0361 6263 7202 0000 0072 0300 0000 da07  .abcr....r......
-00001460: 696e 7370 6563 7472 0400 0000 da07 7061  inspectr......pa
-00001470: 7468 6c69 6272 0500 0000 7217 0000 00da  thlibr....r.....
-00001480: 0a69 6e66 6c65 6374 696f 6e72 0600 0000  .inflectionr....
-00001490: 7207 0000 00da 0d66 6c75 6964 6479 6e2e  r......fluiddyn.
-000014a0: 7574 696c 7208 0000 00da 1d66 6c75 6964  utilr......fluid
-000014b0: 7369 6d66 6f61 6d2e 666f 616d 5f69 6e70  simfoam.foam_inp
-000014c0: 7574 5f66 696c 6573 7209 0000 0072 0a00  ut_filesr....r..
-000014d0: 0000 720b 0000 0072 0c00 0000 7226 0000  ..r....r....r&..
-000014e0: 0072 4300 0000 7266 0000 0072 1c00 0000  .rC...rf...r....
-000014f0: 721c 0000 0072 1c00 0000 721d 0000 00da  r....r....r.....
-00001500: 083c 6d6f 6475 6c65 3e01 0000 0073 1800  .<module>....s..
-00001510: 0000 0400 1002 0c01 0c01 0802 1001 0c02  ................
-00001520: 1401 0e03 1019 1027 0e52                 .......'.R
+00000670: 5300 7c00 6a00 6a04 7c00 6a05 1b00 7d03  S.|.j.j.|.j...}.
+00000680: 7c03 6a06 6a07 6403 6404 8d01 0100 7c03  |.j.j.d.d.....|.
+00000690: a008 7c02 a101 0100 6401 5300 2905 7a11  ..|.....d.S.).z.
+000006a0: 4765 6e65 7261 7465 2074 6865 2066 696c  Generate the fil
+000006b0: 654e 4654 2901 da08 6578 6973 745f 6f6b  eNFT)...exist_ok
+000006c0: 2909 7212 0000 0072 1400 0000 da06 7061  ).r....r......pa
+000006d0: 7261 6d73 da0d 6765 6e65 7261 7465 5f63  rams..generate_c
+000006e0: 6f64 65da 0870 6174 685f 7275 6e72 2900  ode..path_runr).
+000006f0: 0000 7217 0000 00da 056d 6b64 6972 da0a  ..r......mkdir..
+00000700: 7772 6974 655f 7465 7874 2904 721c 0000  write_text).r...
+00000710: 0072 2d00 0000 da04 636f 6465 da04 7061  .r-.....code..pa
+00000720: 7468 721e 0000 0072 1e00 0000 721f 0000  thr....r....r...
+00000730: 00da 0d67 656e 6572 6174 655f 6669 6c65  ...generate_file
+00000740: 2e00 0000 7310 0000 0008 020a 010a 0208  ....s...........
+00000750: 0104 010e 020e 010e 017a 1e46 696c 6547  .........z.FileG
+00000760: 656e 6572 6174 6f72 4142 432e 6765 6e65  eneratorABC.gene
+00000770: 7261 7465 5f66 696c 6563 0100 0000 0000  rate_filec......
+00000780: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+00000790: 0000 7304 0000 0064 0153 0029 027a 1d47  ..s....d.S.).z.G
+000007a0: 656e 6572 6174 6520 7468 6520 636f 6465  enerate the code
+000007b0: 206f 6620 7468 6520 6669 6c65 4e72 1e00   of the fileNr..
+000007c0: 0000 a901 721c 0000 0072 1e00 0000 721e  ....r....r....r.
+000007d0: 0000 0072 1f00 0000 722e 0000 003b 0000  ...r....r....;..
+000007e0: 0073 0200 0000 0400 7a1e 4669 6c65 4765  .s......z.FileGe
+000007f0: 6e65 7261 746f 7241 4243 2e67 656e 6572  neratorABC.gener
+00000800: 6174 655f 636f 6465 6301 0000 0000 0000  ate_codec.......
+00000810: 0000 0000 0003 0000 0004 0000 0003 0000  ................
+00000820: 0073 4200 0000 8800 6a00 6a01 8800 6a02  .sB.....j.j...j.
+00000830: 1b00 7d01 7403 8700 6601 6401 6402 8408  ..}.t...f.d.d...
+00000840: 6403 4400 8301 8301 721d 7404 7c01 a005  d.D.....r.t.|...
+00000850: a100 8301 7d02 7c01 7c02 5f06 7c02 5300  ....}.|.|._.|.S.
+00000860: 7407 7c01 8301 5300 2904 4e63 0100 0000  t.|...S.).Nc....
+00000870: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000880: 3300 0000 731c 0000 0081 007c 005d 097d  3...s......|.].}
+00000890: 0188 006a 00a0 017c 01a1 0156 0001 0071  ...j...|...V...q
+000008a0: 0264 0053 0072 2100 0000 2902 7229 0000  .d.S.r!...).r)..
+000008b0: 00da 0a73 7461 7274 7377 6974 6829 02da  ...startswith)..
+000008c0: 022e 30da 0573 7461 7274 7235 0000 0072  ..0..startr5...r
+000008d0: 1e00 0000 721f 0000 00da 093c 6765 6e65  ....r......<gene
+000008e0: 7870 723e 4100 0000 7308 0000 0002 8004  xpr>A...s.......
+000008f0: 000c 010a ff7a 2846 696c 6547 656e 6572  .....z(FileGener
+00000900: 6174 6f72 4142 432e 7265 6164 2e3c 6c6f  atorABC.read.<lo
+00000910: 6361 6c73 3e2e 3c67 656e 6578 7072 3e29  cals>.<genexpr>)
+00000920: 02da 0673 7973 7465 6dda 0863 6f6e 7374  ...system..const
+00000930: 616e 7429 0872 1200 0000 722f 0000 0072  ant).r....r/...r
+00000940: 2900 0000 da03 616e 7972 0a00 0000 da09  ).....anyr......
+00000950: 7265 6164 5f74 6578 7472 3300 0000 720b  read_textr3...r.
+00000960: 0000 0029 0372 1c00 0000 7233 0000 00da  ...).r....r3....
+00000970: 0474 7265 6572 1e00 0000 7235 0000 0072  .treer....r5...r
+00000980: 1f00 0000 da04 7265 6164 3f00 0000 7310  ......read?...s.
+00000990: 0000 000e 010c 0102 0108 ff0c 0306 0104  ................
+000009a0: 0108 027a 1546 696c 6547 656e 6572 6174  ...z.FileGenerat
+000009b0: 6f72 4142 432e 7265 6164 6302 0000 0000  orABC.readc.....
+000009c0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+000009d0: 0000 0073 1c00 0000 7c00 6a00 6a01 7c00  ...s....|.j.j.|.
+000009e0: 6a02 1b00 a003 7c01 a004 a100 a101 0100  j.....|.........
+000009f0: 6400 5300 7221 0000 0029 0572 1200 0000  d.S.r!...).r....
+00000a00: 722f 0000 0072 2900 0000 7231 0000 00da  r/...r)...r1....
+00000a10: 0464 756d 7029 0272 1c00 0000 5a08 6475  .dump).r....Z.du
+00000a20: 6d70 6162 6c65 721e 0000 0072 1e00 0000  mpabler....r....
+00000a30: 721f 0000 00da 096f 7665 7277 7269 7465  r......overwrite
+00000a40: 4a00 0000 7302 0000 001c 017a 1a46 696c  J...s......z.Fil
+00000a50: 6547 656e 6572 6174 6f72 4142 432e 6f76  eGeneratorABC.ov
+00000a60: 6572 7772 6974 6572 2100 0000 290b 7224  erwriter!...).r$
+00000a70: 0000 0072 2500 0000 7226 0000 00da 0373  ...r%...r&.....s
+00000a80: 7472 da0f 5f5f 616e 6e6f 7461 7469 6f6e  tr..__annotation
+00000a90: 735f 5f72 2000 0000 7234 0000 0072 0300  s__r ...r4...r..
+00000aa0: 0000 722e 0000 0072 3f00 0000 7241 0000  ..r....r?...rA..
+00000ab0: 0072 1e00 0000 721e 0000 0072 1e00 0000  .r....r....r....
+00000ac0: 721f 0000 0072 2800 0000 2700 0000 7310  r....r(...'...s.
+00000ad0: 0000 000a 0008 0108 020a 0402 0d0a 0108  ................
+00000ae0: 030c 0b72 2800 0000 6300 0000 0000 0000  ...r(...c.......
+00000af0: 0000 0000 0000 0000 0003 0000 0000 0000  ................
+00000b00: 0073 3c00 0000 6500 5a01 6400 5a02 5500  .s<...e.Z.d.Z.U.
+00000b10: 6503 6504 6401 3c00 8700 6601 6402 6403  e.e.d.<...f.d.d.
+00000b20: 8408 5a05 6409 6405 6406 8401 5a06 6507  ..Z.d.d.d...Z.e.
+00000b30: 6407 6408 8400 8301 5a08 8700 0400 5a09  d.d.....Z.....Z.
+00000b40: 5300 290a da0d 4669 6c65 4765 6e65 7261  S.)...FileGenera
+00000b50: 746f 7272 2300 0000 6302 0000 0000 0000  torr#...c.......
+00000b60: 0000 0000 0002 0000 0003 0000 0003 0000  ................
+00000b70: 0073 1000 0000 7400 8300 a001 7c01 a101  .s....t.....|...
+00000b80: 0100 6400 5300 7221 0000 0029 02da 0573  ..d.S.r!...)...s
+00000b90: 7570 6572 7220 0000 0072 2b00 0000 a901  uperr ...r+.....
+00000ba0: da09 5f5f 636c 6173 735f 5f72 1e00 0000  ..__class__r....
+00000bb0: 721f 0000 0072 2000 0000 5100 0000 7302  r....r ...Q...s.
+00000bc0: 0000 0010 017a 1646 696c 6547 656e 6572  .....z.FileGener
+00000bd0: 6174 6f72 2e5f 5f69 6e69 745f 5f4e 6302  ator.__init__Nc.
+00000be0: 0000 0000 0000 0000 0000 0005 0000 0008  ................
+00000bf0: 0000 0003 0000 0073 2c01 0000 7c01 6401  .......s,...|.d.
+00000c00: 7500 7209 7c00 6a00 6a01 6a02 7d01 7a0b  u.r.|.j.j.j.}.z.
+00000c10: 7403 7c00 6a00 6402 7c00 6a04 1700 8302  t.|.j.d.|.j.....
+00000c20: 7d02 5700 6e0b 0400 7405 791f 0100 0100  }.W.n...t.y.....
+00000c30: 0100 6401 7d02 5900 6e01 7700 7c02 6401  ..d.}.Y.n.w.|.d.
+00000c40: 7500 7266 7a0b 7403 7c00 6a00 6403 7c00  u.rfz.t.|.j.d.|.
+00000c50: 6a04 1700 8302 8900 5700 6e0b 0400 7405  j.......W.n...t.
+00000c60: 793a 0100 0100 0100 6401 8900 5900 6e01  y:......d...Y.n.
+00000c70: 7700 8800 6401 7500 725c 7a0b 7403 7c00  w...d.u.r\z.t.|.
+00000c80: 6a00 6404 7c00 6a04 1700 8302 7d03 5700  j.d.|.j.....}.W.
+00000c90: 6e09 0400 7405 7953 0100 0100 0100 5900  n...t.yS......Y.
+00000ca0: 6e09 7700 7406 7c03 7407 8302 725c 7c03  n.w.t.|.t...r\|.
+00000cb0: 6a08 8900 8800 6401 7501 7266 8700 6601  j.....d.u.rf..f.
+00000cc0: 6405 6406 8408 7d02 7c02 6401 7500 7277  d.d...}.|.d.u.rw
+00000cd0: 7c00 6a09 a00a 7c00 6a0b a101 7d04 7c04  |.j...|.j...}.|.
+00000ce0: 6a0c 7c01 6407 8d01 5300 7c00 6a09 6a0d  j.|.d...S.|.j.j.
+00000cf0: 7c00 6a0b 1b00 a00e a100 7292 740f 6408  |.j.......r.t.d.
+00000d00: 7c00 6a10 9b00 6409 7c00 6a09 6a0d 9b00  |.j...d.|.j.j...
+00000d10: 640a 7c00 6a04 9b00 640b 9d07 8301 8201  d.|.j...d.......
+00000d20: 7c02 7c01 8301 5300 290c 7a96 4765 6e65  |.|...S.).z.Gene
+00000d30: 7261 7465 2074 6865 2063 6f64 6520 6f66  rate the code of
+00000d40: 2074 6865 2066 696c 6520 6672 6f6d 202e   the file from .
+00000d50: 2e2e 0a0a 2020 2020 2020 2020 2d20 6120  ....        - a 
+00000d60: 6d65 7468 6f64 206e 616d 6564 206c 696b  method named lik
+00000d70: 6520 6073 696d 2e6f 7574 7075 742e 5f6d  e `sim.output._m
+00000d80: 616b 655f 636f 6465 5f62 6c6f 636b 5f6d  ake_code_block_m
+00000d90: 6573 685f 6469 6374 602c 0a20 2020 2020  esh_dict`,.     
+00000da0: 2020 202d 206f 7220 6120 4a69 6e6a 6120     - or a Jinja 
+00000db0: 7465 6d70 6c61 7465 2e0a 2020 2020 2020  template..      
+00000dc0: 2020 4e5a 0b5f 6d61 6b65 5f63 6f64 655f    NZ._make_code_
+00000dd0: 5a0b 5f6d 616b 655f 7472 6565 5fda 085f  Z._make_tree_.._
+00000de0: 6865 6c70 6572 5f63 0100 0000 0000 0000  helper_c........
+00000df0: 0000 0000 0200 0000 0200 0000 1300 0000  ................
+00000e00: 731c 0000 0088 007c 0083 017d 017c 0164  s......|...}.|.d
+00000e10: 0175 0072 0a64 0153 007c 01a0 00a1 0053  .u.r.d.S.|.....S
+00000e20: 0029 024e 4629 0172 4000 0000 2902 5a07  .).NF).r@...).Z.
+00000e30: 7061 7261 6d73 5f72 3e00 0000 a901 da09  params_r>.......
+00000e40: 6d61 6b65 5f74 7265 6572 1e00 0000 721f  make_treer....r.
+00000e50: 0000 00da 096d 616b 655f 636f 6465 7300  .....make_codes.
+00000e60: 0000 7308 0000 0008 0108 0104 0108 017a  ..s............z
+00000e70: 2e46 696c 6547 656e 6572 6174 6f72 2e67  .FileGenerator.g
+00000e80: 656e 6572 6174 655f 636f 6465 2e3c 6c6f  enerate_code.<lo
+00000e90: 6361 6c73 3e2e 6d61 6b65 5f63 6f64 6529  cals>.make_code)
+00000ea0: 0172 2d00 0000 7a3b 466c 7569 6473 696d  .r-...z;Fluidsim
+00000eb0: 666f 616d 2073 6f6c 7665 7220 6973 7375  foam solver issu
+00000ec0: 653a 2032 2063 6f6e 6375 7272 656e 7420  e: 2 concurrent 
+00000ed0: 6d65 7468 6f64 7320 746f 2070 726f 6475  methods to produ
+00000ee0: 6365 207a 103a 0a2d 2074 656d 706c 6174  ce z.:.- templat
+00000ef0: 6520 696e 207a 1f2c 0a2d 2066 756e 6374  e in z.,.- funct
+00000f00: 696f 6e20 6f75 7470 7574 2e5f 6d61 6b65  ion output._make
+00000f10: 5f63 6f64 655f 7a3d 2e0a 5265 6d6f 7665  _code_z=..Remove
+00000f20: 2074 6865 2066 696c 6520 6f72 2074 6865   the file or the
+00000f30: 2066 756e 6374 696f 6e20 286f 7220 6d61   function (or ma
+00000f40: 6b65 2069 7420 6571 7561 6c20 746f 204e  ke it equal to N
+00000f50: 6f6e 6529 2e29 1172 1200 0000 7214 0000  one).).r....r...
+00000f60: 0072 2d00 0000 da07 6765 7461 7474 72da  .r-.....getattr.
+00000f70: 055f 6e61 6d65 da0e 4174 7472 6962 7574  ._name..Attribut
+00000f80: 6545 7272 6f72 da0a 6973 696e 7374 616e  eError..isinstan
+00000f90: 6365 7209 0000 0072 4a00 0000 722a 0000  cer....rJ...r*..
+00000fa0: 0072 2200 0000 7223 0000 00da 0672 656e  .r"...r#.....ren
+00000fb0: 6465 7272 1800 0000 da06 6578 6973 7473  derr......exists
+00000fc0: da0c 5275 6e74 696d 6545 7272 6f72 7229  ..RuntimeErrorr)
+00000fd0: 0000 0029 0572 1c00 0000 722d 0000 0072  ...).r....r-...r
+00000fe0: 4b00 0000 da06 6865 6c70 6572 da08 7465  K.....helper..te
+00000ff0: 6d70 6c61 7465 721e 0000 0072 4900 0000  mplater....rI...
+00001000: 721f 0000 0072 2e00 0000 5400 0000 734a  r....r....T...sJ
+00001010: 0000 0008 060a 0102 0216 010c 0108 0102  ................
+00001020: ff08 0302 0116 010c 0108 0102 ff08 0302  ................
+00001030: 0116 010c 0104 0102 ff0a 0306 0108 020c  ................
+00001040: 0208 060e 010c 0112 0202 0102 0104 0104  ................
+00001050: ff06 0204 fe04 0306 fd04 ff08 087a 1b46  .............z.F
+00001060: 696c 6547 656e 6572 6174 6f72 2e67 656e  ileGenerator.gen
+00001070: 6572 6174 655f 636f 6465 6303 0000 0000  erate_codec.....
+00001080: 0000 0000 0000 0006 0000 0008 0000 0043  ...............C
+00001090: 0000 0073 9a00 0000 7400 7c02 6a01 6a02  ...s....t.|.j.j.
+000010a0: 6a03 7c02 6a01 6a02 6a04 8302 7d03 7a0a  j.|.j.j.j...}.z.
+000010b0: 7405 7c03 6401 7c00 6a06 1700 8302 7d04  t.|.d.|.j.....}.
+000010c0: 5700 6e0b 0400 7407 7920 0100 0100 0100  W.n...t.y ......
+000010d0: 6400 7d04 5900 6e01 7700 7c04 6400 7500  d.}.Y.n.w.|.d.u.
+000010e0: 7241 7a0a 7405 7c03 6402 7c00 6a06 1700  rAz.t.|.d.|.j...
+000010f0: 8302 7d05 5700 6e09 0400 7407 7938 0100  ..}.W.n...t.y8..
+00001100: 0100 0100 5900 6e09 7700 7408 7c05 7409  ....Y.n.w.t.|.t.
+00001110: 8302 7241 7c05 6a0a 7d04 7c04 6400 7501  ..rA|.j.}.|.d.u.
+00001120: 724b 7c04 7c01 8301 0100 6400 5300 6400  rK|.|.....d.S.d.
+00001130: 5300 2903 4e5a 115f 636f 6d70 6c65 7465  S.).NZ._complete
+00001140: 5f70 6172 616d 735f 7248 0000 0029 0b72  _params_rH...).r
+00001150: 0800 0000 da07 636c 6173 7365 73da 064f  ......classes..O
+00001160: 7574 7075 74da 0b6d 6f64 756c 655f 6e61  utput..module_na
+00001170: 6d65 da0a 636c 6173 735f 6e61 6d65 724c  me..class_namerL
+00001180: 0000 0072 4d00 0000 724e 0000 0072 4f00  ...rM...rN...rO.
+00001190: 0000 7209 0000 00da 0f63 6f6d 706c 6574  ..r......complet
+000011a0: 655f 7061 7261 6d73 2906 da03 636c 7372  e_params)...clsr
+000011b0: 2d00 0000 da0b 696e 666f 5f73 6f6c 7665  -.....info_solve
+000011c0: 725a 0a6f 7574 7075 745f 636c 7372 5900  rZ.output_clsrY.
+000011d0: 0000 7253 0000 0072 1e00 0000 721e 0000  ..rS...r....r...
+000011e0: 0072 1f00 0000 da1d 5f63 6f6d 706c 6574  .r......_complet
+000011f0: 655f 7061 7261 6d73 5f77 6974 685f 6465  e_params_with_de
+00001200: 6661 756c 7488 0000 0073 2800 0000 0202  fault....s(.....
+00001210: 0801 0801 04fe 0204 1401 0c01 0801 02ff  ................
+00001220: 0803 0201 1401 0c01 0401 02ff 0a03 0601  ................
+00001230: 0802 0c01 04ff 7a2b 4669 6c65 4765 6e65  ......z+FileGene
+00001240: 7261 746f 722e 5f63 6f6d 706c 6574 655f  rator._complete_
+00001250: 7061 7261 6d73 5f77 6974 685f 6465 6661  params_with_defa
+00001260: 756c 7472 2100 0000 290a 7224 0000 0072  ultr!...).r$...r
+00001270: 2500 0000 7226 0000 0072 4200 0000 7243  %...r&...rB...rC
+00001280: 0000 0072 2000 0000 722e 0000 00da 0b63  ...r ...r......c
+00001290: 6c61 7373 6d65 7468 6f64 725c 0000 00da  lassmethodr\....
+000012a0: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 721e  .__classcell__r.
+000012b0: 0000 0072 1e00 0000 7246 0000 0072 1f00  ...r....rF...r..
+000012c0: 0000 7244 0000 004e 0000 0073 0c00 0000  ..rD...N...s....
+000012d0: 0a00 0801 0c02 0a03 0234 1201 7244 0000  .........4..rD..
+000012e0: 00da 0130 6302 0000 0000 0000 0000 0000  ...0c...........
+000012f0: 0004 0000 000b 0000 0043 0000 0073 4e00  .........C...sN.
+00001300: 0000 6401 7400 7c00 8301 9b00 9d02 7d02  ..d.t.|.......}.
+00001310: 7c01 9b00 6402 7c00 9b00 9d03 7d03 7401  |...d.|.....}.t.
+00001320: 7c02 7402 6601 7c01 7c03 7c03 9b00 6403  |.t.f.|.|.|...d.
+00001330: 9d02 7403 7c00 a004 6404 6405 a102 a004  ..t.|...d.d.....
+00001340: 6402 6405 a102 8301 6406 9c04 8303 5300  d.d.....d.....S.
+00001350: 2907 4e72 4400 0000 fa01 2f7a 062e 6a69  ).NrD...../z..ji
+00001360: 6e6a 61da 012e da01 5f29 04da 0864 6972  nja....._)...dir
+00001370: 5f6e 616d 6572 2900 0000 7223 0000 0072  _namer)...r#...r
+00001380: 4d00 0000 2905 7206 0000 0072 1300 0000  M...).r....r....
+00001390: 7244 0000 0072 0700 0000 da07 7265 706c  rD...r......repl
+000013a0: 6163 6529 04da 0966 696c 655f 6e61 6d65  ace)...file_name
+000013b0: 7263 0000 00da 0863 6c73 5f6e 616d 65da  rc.....cls_name.
+000013c0: 0d72 656c 6174 6976 655f 7061 7468 721e  .relative_pathr.
+000013d0: 0000 0072 1e00 0000 721f 0000 00da 186e  ...r....r......n
+000013e0: 6577 5f66 696c 655f 6765 6e65 7261 746f  ew_file_generato
+000013f0: 725f 636c 6173 73a0 0000 0073 1600 0000  r_class....s....
+00001400: 0e01 0e01 0201 0201 0401 0202 0201 0801  ................
+00001410: 1601 04fc 04fd 7268 0000 0029 0172 5f00  ......rh...).r_.
+00001420: 0000 2916 7227 0000 00da 0361 6263 7202  ..).r'.....abcr.
+00001430: 0000 0072 0300 0000 da07 696e 7370 6563  ...r......inspec
+00001440: 7472 0400 0000 da07 7061 7468 6c69 6272  tr......pathlibr
+00001450: 0500 0000 7219 0000 00da 0a69 6e66 6c65  ....r......infle
+00001460: 6374 696f 6e72 0600 0000 7207 0000 00da  ctionr....r.....
+00001470: 0d66 6c75 6964 6479 6e2e 7574 696c 7208  .fluiddyn.utilr.
+00001480: 0000 00da 1d66 6c75 6964 7369 6d66 6f61  .....fluidsimfoa
+00001490: 6d2e 666f 616d 5f69 6e70 7574 5f66 696c  m.foam_input_fil
+000014a0: 6573 7209 0000 0072 0a00 0000 720b 0000  esr....r....r...
+000014b0: 0072 0c00 0000 7228 0000 0072 4400 0000  .r....r(...rD...
+000014c0: 7268 0000 0072 1e00 0000 721e 0000 0072  rh...r....r....r
+000014d0: 1e00 0000 721f 0000 00da 083c 6d6f 6475  ....r......<modu
+000014e0: 6c65 3e01 0000 0073 1800 0000 0400 1002  le>....s........
+000014f0: 0c01 0c01 0802 1001 0c02 1401 0e03 1019  ................
+00001500: 1027 0e52                                .'.R
```

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/parser.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May  9 12:42:41 2023 UTC, .py size: 9522 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c13f 5a64 3225 0000  o........?Zd2%..
+00000000: 6f0d 0d0a 0000 0000 b0ed 9964 0624 0000  o..........d.$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 0401 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6406 6407 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
@@ -54,602 +54,596 @@
 00000350: 652f 4465 762f 666c 7569 6473 696d 666f  e/Dev/fluidsimfo
 00000360: 616d 2f73 7263 2f66 6c75 6964 7369 6d66  am/src/fluidsimf
 00000370: 6f61 6d2f 666f 616d 5f69 6e70 7574 5f66  oam/foam_input_f
 00000380: 696c 6573 2f70 6172 7365 722e 7079 7219  iles/parser.pyr.
 00000390: 0000 0022 0000 0073 0a00 0000 0a00 0802  ..."...s........
 000003a0: 0c01 0c01 1001 7219 0000 004e 6302 0000  ......r....Nc...
 000003b0: 0000 0000 0000 0000 0003 0000 0008 0000  ................
-000003c0: 0043 0000 0073 7a00 0000 6401 a000 6402  .C...sz...d...d.
-000003d0: 6403 8400 7c00 a001 6401 a101 4400 8301  d...|...d...D...
-000003e0: a101 7d00 7c00 a002 6401 a101 7316 7c00  ..}.|...d...s.|.
-000003f0: 6401 3700 7d00 7c01 6400 7500 7230 7a07  d.7.}.|.d.u.r0z.
-00000400: 7403 a004 7c00 a101 7d02 5700 6e15 0400  t...|...}.W.n...
-00000410: 7405 792f 0100 0100 0100 7406 a004 7c00  t.y/......t...|.
-00000420: a101 7d02 5900 6e08 7700 7407 7c01 1900  ..}.Y.n.w.t.|...
-00000430: a004 7c00 a101 7d02 7408 8300 a009 7c02  ..|...}.t.....|.
-00000440: a101 5300 2904 4eda 010a 6301 0000 0000  ..S.).N...c.....
-00000450: 0000 0000 0000 0002 0000 0003 0000 0073  ...............s
-00000460: 0000 0073 1800 0000 8100 7c00 5d07 7d01  ...s......|.].}.
-00000470: 7c01 a000 a100 5600 0100 7102 6400 5300  |.....V...q.d.S.
-00000480: a901 4e29 01da 0672 7374 7269 7029 02da  ..N)...rstrip)..
-00000490: 022e 30da 046c 696e 6572 2400 0000 7224  ..0..liner$...r$
-000004a0: 0000 0072 2500 0000 da09 3c67 656e 6578  ...r%.....<genex
-000004b0: 7072 3e2b 0000 0073 0400 0000 0280 1600  pr>+...s........
-000004c0: 7a18 7061 7273 652e 3c6c 6f63 616c 733e  z.parse.<locals>
-000004d0: 2e3c 6765 6e65 7870 723e 290a da04 6a6f  .<genexpr>)...jo
-000004e0: 696e da05 7370 6c69 74da 0865 6e64 7377  in..split..endsw
-000004f0: 6974 68da 0b6c 6172 6b5f 7061 7273 6572  ith..lark_parser
-00000500: da05 7061 7273 6572 0700 0000 da14 6c61  ..parser......la
-00000510: 726b 5f70 6172 7365 725f 6164 7661 6e63  rk_parser_advanc
-00000520: 6564 da07 7061 7273 6572 73da 0f46 6f61  ed..parsers..Foa
-00000530: 6d54 7261 6e73 666f 726d 6572 da09 7472  mTransformer..tr
-00000540: 616e 7366 6f72 6d29 03da 0474 6578 74da  ansform)...text.
-00000550: 0767 7261 6d6d 6172 da04 7472 6565 7224  .grammar..treer$
-00000560: 0000 0072 2400 0000 7225 0000 0072 3000  ...r$...r%...r0.
-00000570: 0000 2a00 0000 7316 0000 001a 010a 0108  ..*...s.........
-00000580: 0108 0202 010e 010c 010e 0102 ff0e 030c  ................
-00000590: 0272 3000 0000 6301 0000 0000 0000 0000  .r0...c.........
-000005a0: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
-000005b0: 0800 0000 7c00 a000 a100 5300 7227 0000  ....|.....S.r'..
-000005c0: 0029 01da 0464 756d 7029 0172 3700 0000  .)...dump).r7...
-000005d0: 7224 0000 0072 2400 0000 7225 0000 0072  r$...r$...r%...r
-000005e0: 3800 0000 3a00 0000 f302 0000 0008 0172  8...:..........r
-000005f0: 3800 0000 6301 0000 0000 0000 0000 0000  8...c...........
-00000600: 0001 0000 0002 0000 0043 0000 0073 0e00  .........C...s..
-00000610: 0000 6401 6402 8400 7c00 4400 8301 5300  ..d.d...|.D...S.
-00000620: 2903 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
-00000630: 0200 0000 0400 0000 5300 0000 f318 0000  ........S.......
-00000640: 0067 007c 005d 087d 017c 0164 0075 0172  .g.|.].}.|.d.u.r
-00000650: 027c 0191 0271 0253 0072 2700 0000 7224  .|...q.S.r'...r$
-00000660: 0000 00a9 0272 2900 0000 da04 6974 656d  .....r).....item
-00000670: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
-00000680: 0a3c 6c69 7374 636f 6d70 3e3f 0000 00f3  .<listcomp>?....
-00000690: 0200 0000 1800 7a26 6669 6c74 6572 5f6e  ......z&filter_n
-000006a0: 6f5f 6e65 776c 696e 6573 2e3c 6c6f 6361  o_newlines.<loca
-000006b0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7224  ls>.<listcomp>r$
-000006c0: 0000 0029 01da 0569 7465 6d73 7224 0000  ...)...itemsr$..
-000006d0: 0072 2400 0000 7225 0000 00da 1266 696c  .r$...r%.....fil
-000006e0: 7465 725f 6e6f 5f6e 6577 6c69 6e65 733e  ter_no_newlines>
-000006f0: 0000 0073 0200 0000 0e01 7240 0000 0063  ...s......r@...c
-00000700: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000710: 0800 0000 4300 0000 732e 0000 0074 007c  ....C...s....t.|
-00000720: 0083 017d 007a 0574 017c 0083 0157 0053  ...}.z.t.|...W.S
-00000730: 0004 0074 0279 1601 0001 0001 0074 037c  ...t.y.......t.|
-00000740: 0083 0106 0059 0053 0077 0072 2700 0000  .....Y.S.w.r'...
-00000750: 2904 7221 0000 0072 2300 0000 da0a 5661  ).r!...r#.....Va
-00000760: 6c75 6545 7272 6f72 da05 666c 6f61 7429  lueError..float)
-00000770: 01da 066e 756d 6265 7272 2400 0000 7224  ...numberr$...r$
-00000780: 0000 0072 2500 0000 da12 5f63 6f6e 7665  ...r%....._conve
-00000790: 7274 5f74 6f5f 6e75 6d62 6572 4200 0000  rt_to_numberB...
-000007a0: 730c 0000 0008 0102 010a 010c 010c 0102  s...............
-000007b0: ff72 4400 0000 6300 0000 0000 0000 0000  .rD...c.........
-000007c0: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
-000007d0: c400 0000 6500 5a01 6400 5a02 6401 6402  ....e.Z.d.Z.d.d.
-000007e0: 8400 5a03 6403 6404 8400 5a04 6405 6406  ..Z.d.d...Z.d.d.
-000007f0: 8400 5a05 6407 6408 8400 5a06 6409 640a  ..Z.d.d...Z.d.d.
-00000800: 8400 5a07 640b 640c 8400 5a08 640d 640e  ..Z.d.d...Z.d.d.
-00000810: 8400 5a09 640f 6410 8400 5a0a 6411 6412  ..Z.d.d...Z.d.d.
-00000820: 8400 5a0b 6413 6414 8400 5a0c 6415 6416  ..Z.d.d...Z.d.d.
-00000830: 8400 5a0d 6417 6418 8400 5a0e 6419 641a  ..Z.d.d...Z.d.d.
-00000840: 8400 5a0f 641b 641c 8400 5a10 641d 641e  ..Z.d.d...Z.d.d.
-00000850: 8400 5a11 641f 6420 8400 5a12 6421 6422  ..Z.d.d ..Z.d!d"
-00000860: 8400 5a13 6423 6424 8400 5a14 6425 6426  ..Z.d#d$..Z.d%d&
-00000870: 8400 5a15 6427 6428 8400 5a16 6429 642a  ..Z.d'd(..Z.d)d*
-00000880: 8400 5a17 642b 642c 8400 5a18 642d 642e  ..Z.d+d,..Z.d-d.
-00000890: 8400 5a19 642f 5300 2930 7233 0000 0063  ..Z.d/S.)0r3...c
-000008a0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-000008b0: 0200 0000 4300 0000 7308 0000 0074 007c  ....C...s....t.|
-000008c0: 0183 0153 0072 2700 0000 2901 7244 0000  ...S.r'...).rD..
-000008d0: 00a9 02da 0473 656c 66da 0574 6f6b 656e  .....self..token
-000008e0: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
-000008f0: 0d53 4947 4e45 445f 4e55 4d42 4552 4b00  .SIGNED_NUMBERK.
-00000900: 0000 7239 0000 007a 1d46 6f61 6d54 7261  ..r9...z.FoamTra
-00000910: 6e73 666f 726d 6572 2e53 4947 4e45 445f  nsformer.SIGNED_
-00000920: 4e55 4d42 4552 6302 0000 0000 0000 0000  NUMBERc.........
-00000930: 0000 0002 0000 0001 0000 0043 0000 00f3  ...........C....
-00000940: 0600 0000 7c01 6a00 5300 7227 0000 00a9  ....|.j.S.r'....
-00000950: 0172 1400 0000 7245 0000 0072 2400 0000  .r....rE...r$...
-00000960: 7224 0000 0072 2500 0000 da05 434e 414d  r$...r%.....CNAM
-00000970: 454e 0000 00f3 0200 0000 0601 7a15 466f  EN..........z.Fo
-00000980: 616d 5472 616e 7366 6f72 6d65 722e 434e  amTransformer.CN
-00000990: 414d 4563 0200 0000 0000 0000 0000 0000  AMEc............
-000009a0: 0200 0000 0100 0000 4300 0000 7304 0000  ........C...s...
-000009b0: 0064 0053 0072 2700 0000 7224 0000 00a9  .d.S.r'...r$....
-000009c0: 0272 4600 0000 da05 6e6f 6465 7372 2400  .rF.....nodesr$.
-000009d0: 0000 7224 0000 0072 2500 0000 da07 4e45  ..r$...r%.....NE
-000009e0: 574c 494e 4551 0000 0073 0200 0000 0401  WLINEQ...s......
-000009f0: 7a17 466f 616d 5472 616e 7366 6f72 6d65  z.FoamTransforme
-00000a00: 722e 4e45 574c 494e 4563 0200 0000 0000  r.NEWLINEc......
-00000a10: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
-00000a20: 0000 7249 0000 0072 2700 0000 724a 0000  ..rI...r'...rJ..
-00000a30: 0072 4500 0000 7224 0000 0072 2400 0000  .rE...r$...r$...
-00000a40: 7225 0000 00da 0e45 5343 4150 4544 5f53  r%.....ESCAPED_S
-00000a50: 5452 494e 4754 0000 0072 4c00 0000 7a1e  TRINGT...rL...z.
-00000a60: 466f 616d 5472 616e 7366 6f72 6d65 722e  FoamTransformer.
-00000a70: 4553 4341 5045 445f 5354 5249 4e47 6302  ESCAPED_STRINGc.
-00000a80: 0000 0000 0000 0000 0000 0002 0000 0001  ................
-00000a90: 0000 0043 0000 0072 4900 0000 7227 0000  ...C...rI...r'..
-00000aa0: 0072 4a00 0000 7245 0000 0072 2400 0000  .rJ...rE...r$...
-00000ab0: 7224 0000 0072 2500 0000 da0b 444f 5542  r$...r%.....DOUB
-00000ac0: 4c45 5f4e 414d 4557 0000 0072 4c00 0000  LE_NAMEW...rL...
-00000ad0: 7a1b 466f 616d 5472 616e 7366 6f72 6d65  z.FoamTransforme
-00000ae0: 722e 444f 5542 4c45 5f4e 414d 4563 0200  r.DOUBLE_NAMEc..
-00000af0: 0000 0000 0000 0000 0000 0200 0000 0100  ................
-00000b00: 0000 4300 0000 7249 0000 0072 2700 0000  ..C...rI...r'...
-00000b10: 724a 0000 0072 4500 0000 7224 0000 0072  rJ...rE...r$...r
-00000b20: 2400 0000 7225 0000 00da 0b54 5249 504c  $...r%.....TRIPL
-00000b30: 455f 4e41 4d45 5a00 0000 724c 0000 007a  E_NAMEZ...rL...z
-00000b40: 1b46 6f61 6d54 7261 6e73 666f 726d 6572  .FoamTransformer
-00000b50: 2e54 5249 504c 455f 4e41 4d45 6302 0000  .TRIPLE_NAMEc...
-00000b60: 0000 0000 0000 0000 0002 0000 0001 0000  ................
-00000b70: 0043 0000 0072 4900 0000 7227 0000 0072  .C...rI...r'...r
-00000b80: 4a00 0000 7245 0000 0072 2400 0000 7224  J...rE...r$...r$
-00000b90: 0000 0072 2500 0000 da05 4551 4b45 595d  ...r%.....EQKEY]
-00000ba0: 0000 0072 4c00 0000 7a15 466f 616d 5472  ...rL...z.FoamTr
-00000bb0: 616e 7366 6f72 6d65 722e 4551 4b45 5963  ansformer.EQKEYc
-00000bc0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000bd0: 0100 0000 4300 0000 7249 0000 0072 2700  ....C...rI...r'.
-00000be0: 0000 724a 0000 0072 4500 0000 7224 0000  ..rJ...rE...r$..
-00000bf0: 0072 2400 0000 7225 0000 00da 054d 4143  .r$...r%.....MAC
-00000c00: 524f 6000 0000 724c 0000 007a 1546 6f61  RO`...rL...z.Foa
-00000c10: 6d54 7261 6e73 666f 726d 6572 2e4d 4143  mTransformer.MAC
-00000c20: 524f 6302 0000 0000 0000 0000 0000 0002  ROc.............
-00000c30: 0000 0003 0000 0043 0000 00f3 1200 0000  .......C........
-00000c40: 7400 6401 6402 8400 7c01 4400 8301 8301  t.d.d...|.D.....
-00000c50: 5300 2903 4e63 0100 0000 0000 0000 0000  S.).Nc..........
-00000c60: 0000 0200 0000 0500 0000 5300 0000 7324  ..........S...s$
-00000c70: 0000 0067 007c 005d 0e7d 0174 007c 0174  ...g.|.].}.t.|.t
-00000c80: 0183 0272 0e7c 016a 0264 006b 0273 027c  ...r.|.j.d.k.s.|
-00000c90: 0191 0271 0253 0029 0172 4f00 0000 a903  ...q.S.).rO.....
-00000ca0: da0a 6973 696e 7374 616e 6365 7205 0000  ..isinstancer...
-00000cb0: 00da 0474 7970 6572 3b00 0000 7224 0000  ...typer;...r$..
-00000cc0: 0072 2400 0000 7225 0000 0072 3d00 0000  .r$...r%...r=...
-00000cd0: 6500 0000 f310 0000 0006 0002 0208 0102  e...............
-00000ce0: fd08 0302 fd02 0106 ff7a 3146 6f61 6d54  .........z1FoamT
-00000cf0: 7261 6e73 666f 726d 6572 2e64 696d 656e  ransformer.dimen
-00000d00: 7369 6f6e 5f73 6574 2e3c 6c6f 6361 6c73  sion_set.<locals
-00000d10: 3e2e 3c6c 6973 7463 6f6d 703e 2901 720d  >.<listcomp>).r.
-00000d20: 0000 00a9 0272 4600 0000 723f 0000 0072  .....rF...r?...r
-00000d30: 2400 0000 7224 0000 0072 2500 0000 da0d  $...r$...r%.....
-00000d40: 6469 6d65 6e73 696f 6e5f 7365 7463 0000  dimension_setc..
-00000d50: 00f3 0a00 0000 0201 0601 0202 04fe 04ff  ................
-00000d60: 7a1d 466f 616d 5472 616e 7366 6f72 6d65  z.FoamTransforme
-00000d70: 722e 6469 6d65 6e73 696f 6e5f 7365 7463  r.dimension_setc
-00000d80: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000d90: 0300 0000 4300 0000 731c 0000 0074 007c  ....C...s....t.|
-00000da0: 0183 0164 016b 0372 0874 0182 0174 027c  ...d.k.r.t...t.|
-00000db0: 0164 0219 0083 0153 00a9 034e 7208 0000  .d.....S...Nr...
-00000dc0: 0072 0100 0000 2903 da03 6c65 6eda 0c52  .r....)...len..R
-00000dd0: 756e 7469 6d65 4572 726f 7272 2100 0000  untimeErrorr!...
-00000de0: 724d 0000 0072 2400 0000 7224 0000 0072  rM...r$...r$...r
-00000df0: 2500 0000 da09 6469 7265 6374 6976 656c  %.....directivel
-00000e00: 0000 0073 0600 0000 0c01 0401 0c01 7a19  ...s..........z.
-00000e10: 466f 616d 5472 616e 7366 6f72 6d65 722e  FoamTransformer.
-00000e20: 6469 7265 6374 6976 6563 0200 0000 0000  directivec......
-00000e30: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-00000e40: 0000 7255 0000 0029 034e 6301 0000 0000  ..rU...).Nc.....
-00000e50: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
-00000e60: 0000 0073 2c00 0000 6700 7c00 5d12 7d01  ...s,...g.|.].}.
-00000e70: 7400 7c01 7401 8302 720e 7c01 6a02 6400  t.|.t...r.|.j.d.
-00000e80: 6b02 7302 7c01 6401 7501 7202 7c01 9102  k.s.|.d.u.r.|...
-00000e90: 7102 5300 2902 724f 0000 004e 7256 0000  q.S.).rO...NrV..
-00000ea0: 0072 3b00 0000 7224 0000 0072 2400 0000  .r;...r$...r$...
-00000eb0: 7225 0000 0072 3d00 0000 7300 0000 7314  r%...r=...s...s.
-00000ec0: 0000 0006 0002 0208 0102 fd08 0302 fd06  ................
-00000ed0: 0402 fc02 0106 ff7a 2846 6f61 6d54 7261  .......z(FoamTra
-00000ee0: 6e73 666f 726d 6572 2e6c 6973 742e 3c6c  nsformer.list.<l
-00000ef0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00000f00: 3e29 0172 1000 0000 725a 0000 0072 2400  >).r....rZ...r$.
-00000f10: 0000 7224 0000 0072 2500 0000 da04 6c69  ..r$...r%.....li
-00000f20: 7374 7100 0000 725c 0000 007a 1446 6f61  stq...r\...z.Foa
-00000f30: 6d54 7261 6e73 666f 726d 6572 2e6c 6973  mTransformer.lis
-00000f40: 7463 0200 0000 0000 0000 0000 0000 0500  tc..............
-00000f50: 0000 0400 0000 4300 0000 7362 0000 007c  ......C...sb...|
-00000f60: 0164 0119 007d 027c 026a 0064 026b 0272  .d...}.|.j.d.k.r
-00000f70: 137c 026a 017d 037c 0164 0364 0085 0219  .|.j.}.|.d.d....
-00000f80: 007d 016e 0264 007d 037c 0144 005d 0f7d  .}.n.d.}.|.D.].}
-00000f90: 0474 027c 046a 0174 0383 0272 267c 046a  .t.|.j.t...r&|.j
-00000fa0: 01a0 047c 046a 00a1 0101 0071 1774 057c  ...|.j.....q.t.|
-00000fb0: 0364 0464 0584 007c 0144 0083 0183 0253  .d.d...|.D.....S
-00000fc0: 0029 064e 7201 0000 005a 0846 6f61 6d46  .).Nr....Z.FoamF
-00000fd0: 696c 6572 0800 0000 6301 0000 0000 0000  iler....c.......
-00000fe0: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
-00000ff0: 00f3 1600 0000 6900 7c00 5d07 7d01 7c01  ......i.|.].}.|.
-00001000: 6a00 7c01 6a01 9302 7102 5300 7224 0000  j.|.j...q.S.r$..
-00001010: 00a9 0272 1a00 0000 7214 0000 00a9 0272  ...r....r......r
-00001020: 2900 0000 da04 6e6f 6465 7224 0000 0072  ).....noder$...r
-00001030: 2400 0000 7225 0000 00da 0a3c 6469 6374  $...r%.....<dict
-00001040: 636f 6d70 3e87 0000 00f3 0200 0000 1600  comp>...........
-00001050: 7a28 466f 616d 5472 616e 7366 6f72 6d65  z(FoamTransforme
-00001060: 722e 6669 6c65 2e3c 6c6f 6361 6c73 3e2e  r.file.<locals>.
-00001070: 3c64 6963 7463 6f6d 703e 2906 721a 0000  <dictcomp>).r...
-00001080: 0072 1400 0000 7257 0000 0072 1000 0000  .r....rW...r....
-00001090: da08 6164 645f 6e61 6d65 720f 0000 0029  ..add_namer....)
-000010a0: 0572 4600 0000 724e 0000 005a 1066 6972  .rF...rN...Z.fir
-000010b0: 7374 5f61 7373 6967 6e6d 656e 74da 0969  st_assignment..i
-000010c0: 6e66 6f5f 6469 6374 7265 0000 0072 2400  nfo_dictre...r$.
-000010d0: 0000 7224 0000 0072 2500 0000 da04 6669  ..r$...r%.....fi
-000010e0: 6c65 7b00 0000 7314 0000 0008 010a 0106  le{...s.........
-000010f0: 010e 0104 0208 020c 010e 0102 8014 027a  ...............z
-00001100: 1446 6f61 6d54 7261 6e73 666f 726d 6572  .FoamTransformer
-00001110: 2e66 696c 6563 0200 0000 0000 0000 0000  .filec..........
-00001120: 0000 0800 0000 0800 0000 4300 0000 7312  ..........C...s.
-00001130: 0100 0064 0164 0284 007c 0144 0083 017d  ...d.d...|.D...}
-00001140: 0164 007d 0264 007d 037c 01a0 0064 03a1  .d.}.d.}.|...d..
-00001150: 017d 0474 017c 0183 0164 046b 0272 1b7c  .}.t.|...d.k.r.|
-00001160: 0164 0319 007d 056e 697a 0c64 0564 0284  .d...}.niz.d.d..
-00001170: 007c 0144 0083 01a0 0264 06a1 017d 0657  .|.D.....d...}.W
-00001180: 006e 0b04 0074 0379 3201 0001 0001 0064  .n...t.y2......d
-00001190: 007d 0259 006e 0677 007c 01a0 007c 06a1  .}.Y.n.w.|...|..
-000011a0: 017d 0264 007d 0374 0464 0764 0284 007c  .}.d.}.t.d.d...|
-000011b0: 0144 0083 0183 0172 4964 08a0 057c 01a1  .D.....rId...|..
-000011c0: 017d 076e 247c 01a0 0064 09a1 017d 0774  .}.n$|...d...}.t
-000011d0: 0464 0a64 0b84 007c 0144 0083 0183 0173  .d.d...|.D.....s
-000011e0: 5e64 0c64 0284 007c 0144 0083 017d 017c  ^d.d...|.D...}.|
-000011f0: 0172 6564 08a0 057c 01a1 017d 0374 067c  .red...|...}.t.|
-00001200: 0774 0783 0272 6d7c 037c 075f 087c 0364  .t...rm|.|._.|.d
-00001210: 0075 0072 757c 0264 0075 0073 7a74 067c  .u.ru|.d.u.szt.|
-00001220: 0774 0783 0272 7d7c 077d 056e 0774 097c  .t...r}|.}.n.t.|
-00001230: 077c 037c 0264 0d8d 037d 0574 0a7c 047c  .|.|.d...}.t.|.|
-00001240: 0583 0253 0029 0e4e 6301 0000 0000 0000  ...S.).Nc.......
-00001250: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
-00001260: 0072 3a00 0000 7227 0000 0072 2400 0000  .r:...r'...r$...
-00001270: 7264 0000 0072 2400 0000 7224 0000 0072  rd...r$...r$...r
-00001280: 2500 0000 723d 0000 008a 0000 0072 3e00  %...r=.......r>.
-00001290: 0000 7a32 466f 616d 5472 616e 7366 6f72  ..z2FoamTransfor
-000012a0: 6d65 722e 7661 725f 6173 7369 676e 6d65  mer.var_assignme
-000012b0: 6e74 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  nt.<locals>.<lis
-000012c0: 7463 6f6d 703e 7201 0000 0072 0800 0000  tcomp>r....r....
-000012d0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000012e0: 0005 0000 0053 0000 00f3 1600 0000 6700  .....S........g.
-000012f0: 7c00 5d07 7d01 7400 7c01 7401 8302 9102  |.].}.t.|.t.....
-00001300: 7102 5300 7224 0000 0029 0272 5700 0000  q.S.r$...).rW...
-00001310: 720d 0000 00a9 0272 2900 0000 da04 656c  r......r).....el
-00001320: 656d 7224 0000 0072 2400 0000 7225 0000  emr$...r$...r%..
-00001330: 0072 3d00 0000 9200 0000 7306 0000 0006  .r=.......s.....
-00001340: 000a 0106 ff54 6301 0000 0000 0000 0000  .....Tc.........
-00001350: 0000 0002 0000 0005 0000 0053 0000 0072  ...........S...r
-00001360: 6b00 0000 7224 0000 00a9 0272 5700 0000  k...r$.....rW...
-00001370: 7221 0000 0072 6c00 0000 7224 0000 0072  r!...rl...r$...r
-00001380: 2400 0000 7225 0000 0072 3d00 0000 9b00  $...r%...r=.....
-00001390: 0000 7267 0000 00da 0120 e9ff ffff ff63  ..rg..... .....c
-000013a0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000013b0: 0400 0000 7300 0000 731a 0000 0081 007c  ....s...s......|
-000013c0: 005d 087d 0174 007c 0174 0183 0256 0001  .].}.t.|.t...V..
-000013d0: 0071 0264 0053 0072 2700 0000 726e 0000  .q.d.S.r'...rn..
-000013e0: 0072 6400 0000 7224 0000 0072 2400 0000  .rd...r$...r$...
-000013f0: 7225 0000 0072 2b00 0000 9f00 0000 7304  r%...r+.......s.
-00001400: 0000 0002 8018 007a 3146 6f61 6d54 7261  .......z1FoamTra
-00001410: 6e73 666f 726d 6572 2e76 6172 5f61 7373  nsformer.var_ass
-00001420: 6967 6e6d 656e 742e 3c6c 6f63 616c 733e  ignment.<locals>
-00001430: 2e3c 6765 6e65 7870 723e 6301 0000 0000  .<genexpr>c.....
-00001440: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-00001450: 0000 0073 1400 0000 6700 7c00 5d06 7d01  ...s....g.|.].}.
-00001460: 7400 7c01 8301 9102 7102 5300 7224 0000  t.|.....q.S.r$..
-00001470: 0029 0172 2100 0000 7264 0000 0072 2400  .).r!...rd...r$.
-00001480: 0000 7224 0000 0072 2500 0000 723d 0000  ..r$...r%...r=..
-00001490: 00a0 0000 0073 0200 0000 1400 2902 721a  .....s......).r.
-000014a0: 0000 00da 0964 696d 656e 7369 6f6e 290b  .....dimension).
-000014b0: da03 706f 7072 5e00 0000 da05 696e 6465  ..popr^.....inde
-000014c0: 7872 4100 0000 da03 616c 6c72 2c00 0000  xrA.....allr,...
-000014d0: 7257 0000 0072 1000 0000 da05 5f6e 616d  rW...r......_nam
-000014e0: 6572 1200 0000 7213 0000 0029 0872 4600  er....r....).rF.
-000014f0: 0000 724e 0000 0072 5b00 0000 5a0d 6e61  ..rN...r[...Z.na
-00001500: 6d65 5f69 6e5f 7661 6c75 6572 1a00 0000  me_in_valuer....
-00001510: 7214 0000 005a 0f69 6e64 6578 5f64 696d  r....Z.index_dim
-00001520: 656e 7369 6f6e da0a 6c61 7374 5f76 616c  ension..last_val
-00001530: 7565 7224 0000 0072 2400 0000 7225 0000  uer$...r$...r%..
-00001540: 00da 0e76 6172 5f61 7373 6967 6e6d 656e  ...var_assignmen
-00001550: 7489 0000 0073 4400 0000 0e01 0401 0401  t....sD.........
-00001560: 0a01 0c01 0a01 0202 0601 0201 04ff 0602  ................
-00001570: 06fe 0c03 0801 02ff 0a03 0402 1201 0c01  ................
-00001580: 0a02 1201 0e01 0401 0a01 0a01 0601 1202  ................
-00001590: 0401 04ff 0603 0202 0601 06ff 0a03 7a1e  ..............z.
-000015a0: 466f 616d 5472 616e 7366 6f72 6d65 722e  FoamTransformer.
-000015b0: 7661 725f 6173 7369 676e 6d65 6e74 6302  var_assignmentc.
-000015c0: 0000 0000 0000 0000 0000 0008 0000 0007  ................
-000015d0: 0000 0043 0000 0073 1601 0000 7400 7c01  ...C...s....t.|.
-000015e0: 8301 7d01 6400 7d02 7401 7c01 8301 6401  ..}.d.}.t.|...d.
-000015f0: 6b02 721a 7c01 a002 6402 a101 7d03 7403  k.r.|...d...}.t.
-00001600: 7c03 7404 6900 7c03 6403 8d02 8302 5300  |.t.i.|.d.....S.
-00001610: 6700 7d04 7c01 4400 5d13 7d05 7405 7c05  g.}.|.D.].}.t.|.
-00001620: 7406 8302 7231 7c05 a007 6404 a101 7231  t...r1|...d...r1
-00001630: 7c01 a002 6401 a101 7d02 0100 6e01 711e  |...d...}...n.q.
-00001640: 7405 7c01 6402 1900 7408 8302 7246 6405  t.|.d...t...rFd.
-00001650: 6406 a009 7c01 a002 6402 a101 a101 1700  d...|...d.......
-00001660: 6407 1700 7d03 6e05 7c01 a002 6402 a101  d...}.n.|...d...
-00001670: 7d03 7c04 7256 7c03 6406 6406 a009 7c04  }.|.rV|.d.d...|.
-00001680: a101 1700 3700 7d03 6408 6409 8400 7c01  ....7.}.d.d...|.
-00001690: 4400 8301 7d06 7c06 4400 5d0f 7d05 7405  D...}.|.D.].}.t.
-000016a0: 7c05 6a0a 740b 8302 726e 7c05 6a0a a00c  |.j.t...rn|.j...
-000016b0: 7c05 6a0d a101 0100 715f 7c02 6400 7501  |.j.....q_|.d.u.
-000016c0: 727a 7c02 640a 6b02 727a 740e 7d07 6e02  rz|.d.k.rzt.}.n.
-000016d0: 7404 7d07 7403 7c03 7c07 640b 640c 8400  t.}.t.|.|.d.d...
-000016e0: 7c06 4400 8301 7c03 7c02 640d 8d03 8302  |.D...|.|.d.....
-000016f0: 5300 290e 4e72 0800 0000 7201 0000 0029  S.).Nr....r....)
-00001700: 02da 0464 6174 6172 1a00 0000 fa01 23fa  ...datar......#.
-00001710: 0128 726f 0000 00fa 0129 6301 0000 0000  .(ro.....)c.....
-00001720: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
-00001730: 0000 0073 2400 0000 6700 7c00 5d0e 7d01  ...s$...g.|.].}.
-00001740: 7400 7c01 6400 8302 7202 7400 7c01 6401  t.|.d...r.t.|.d.
-00001750: 8302 7202 7c01 9102 7102 5300 7263 0000  ..r.|...q.S.rc..
-00001760: 0029 01da 0768 6173 6174 7472 7264 0000  .)...hasattrrd..
-00001770: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
-00001780: 723d 0000 00c5 0000 0072 5900 0000 7a33  r=.......rY...z3
-00001790: 466f 616d 5472 616e 7366 6f72 6d65 722e  FoamTransformer.
-000017a0: 6469 6374 5f61 7373 6967 6e6d 656e 742e  dict_assignment.
-000017b0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-000017c0: 6d70 3e7a 0b23 636f 6465 5374 7265 616d  mp>z.#codeStream
-000017d0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000017e0: 0004 0000 0053 0000 0072 6200 0000 7224  .....S...rb...r$
-000017f0: 0000 0072 6300 0000 7264 0000 0072 2400  ...rc...rd...r$.
-00001800: 0000 7224 0000 0072 2500 0000 7266 0000  ..r$...r%...rf..
-00001810: 00d7 0000 0072 6700 0000 7a33 466f 616d  .....rg...z3Foam
-00001820: 5472 616e 7366 6f72 6d65 722e 6469 6374  Transformer.dict
-00001830: 5f61 7373 6967 6e6d 656e 742e 3c6c 6f63  _assignment.<loc
-00001840: 616c 733e 2e3c 6469 6374 636f 6d70 3e29  als>.<dictcomp>)
-00001850: 0372 7800 0000 721a 0000 0072 6000 0000  .rx...r....r`...
-00001860: 290f 7240 0000 0072 5e00 0000 7272 0000  ).r@...r^...rr..
-00001870: 0072 0900 0000 720c 0000 0072 5700 0000  .r....r....rW...
-00001880: 7221 0000 00da 0a73 7461 7274 7377 6974  r!.....startswit
-00001890: 6872 6100 0000 722c 0000 0072 1400 0000  hra...r,...r....
-000018a0: 7210 0000 0072 6800 0000 721a 0000 0072  r....rh...r....r
-000018b0: 0b00 0000 2908 7246 0000 0072 4e00 0000  ....).rF...rN...
-000018c0: 7260 0000 0072 1a00 0000 5a09 6e6f 6465  r`...r....Z.node
-000018d0: 735f 7374 7272 6500 0000 5a0c 6e6f 6465  s_strre...Z.node
-000018e0: 735f 6173 7369 676e da03 636c 7372 2400  s_assign..clsr$.
-000018f0: 0000 7224 0000 0072 2500 0000 da0f 6469  ..r$...r%.....di
-00001900: 6374 5f61 7373 6967 6e6d 656e 74b0 0000  ct_assignment...
-00001910: 0073 4400 0000 0801 0401 0c02 0a01 1201  .sD.............
-00001920: 0402 0801 1401 0a02 0401 0280 0e01 1a01  ................
-00001930: 0a02 0401 1201 0602 0202 06fe 0806 0c01  ................
-00001940: 0e01 0280 1002 0601 0402 0202 0201 0201  ................
-00001950: 0c01 0201 0201 04fd 04fe 7a1f 466f 616d  ..........z.Foam
-00001960: 5472 616e 7366 6f72 6d65 722e 6469 6374  Transformer.dict
-00001970: 5f61 7373 6967 6e6d 656e 7463 0200 0000  _assignmentc....
-00001980: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00001990: 4300 0000 732e 0000 0074 007c 0183 017d  C...s....t.|...}
-000019a0: 0174 017c 0183 0164 016b 0372 0e74 027c  .t.|...d.k.r.t.|
-000019b0: 0183 0182 0164 007d 0274 037c 027c 0164  .....d.}.t.|.|.d
-000019c0: 0219 0083 0253 0072 5d00 0000 2904 7240  .....S.r]...).r@
-000019d0: 0000 0072 5e00 0000 da13 4e6f 7449 6d70  ...r^.....NotImp
-000019e0: 6c65 6d65 6e74 6564 4572 726f 7272 0900  lementedErrorr..
-000019f0: 0000 a903 7246 0000 0072 4e00 0000 721a  ....rF...rN...r.
-00001a00: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
-00001a10: 0000 da0d 6973 6f6c 6174 6564 5f6c 6973  ....isolated_lis
-00001a20: 74dd 0000 0073 0a00 0000 0801 0c01 0801  t....s..........
-00001a30: 0401 0e01 7a1d 466f 616d 5472 616e 7366  ....z.FoamTransf
-00001a40: 6f72 6d65 722e 6973 6f6c 6174 6564 5f6c  ormer.isolated_l
-00001a50: 6973 7463 0200 0000 0000 0000 0000 0000  istc............
-00001a60: 0800 0000 0600 0000 4300 0000 73ac 0000  ........C...s...
-00001a70: 0074 007c 0183 017d 0164 007d 0274 017c  .t.|...}.d.}.t.|
-00001a80: 0183 0144 005d 185c 027d 037d 0474 027c  ...D.].\.}.}.t.|
-00001a90: 0474 0383 0272 227c 046a 0464 016b 0272  .t...r"|.j.d.k.r
-00001aa0: 2274 057c 0483 0164 0264 0385 0219 007d  "t.|...d.d.....}
-00001ab0: 0201 006e 0171 0a7c 0264 0075 0172 2c7c  ...n.q.|.d.u.r,|
-00001ac0: 01a0 067c 03a1 0101 0064 007d 0574 077c  ...|.....d.}.t.|
-00001ad0: 0183 0164 046b 0472 4074 027c 0164 0319  ...d.k.r@t.|.d..
-00001ae0: 0074 0883 0272 407c 01a0 0664 03a1 017d  .t...r@|...d...}
-00001af0: 057c 01a0 0664 05a1 017d 0664 007d 077c  .|...d...}.d.}.|
-00001b00: 0172 4e64 06a0 097c 01a1 017d 0774 0a7c  .rNd...|...}.t.|
-00001b10: 067c 077c 027c 0564 078d 0453 0029 084e  .|.|.|.d...S.).N
-00001b20: 5a09 4c49 5354 5f54 5950 45e9 0500 0000  Z.LIST_TYPE.....
-00001b30: 7270 0000 0072 0800 0000 7201 0000 0072  rp...r....r....r
-00001b40: 6f00 0000 2904 721a 0000 0072 1b00 0000  o...).r....r....
-00001b50: 721c 0000 0072 1d00 0000 290b 7240 0000  r....r....).r@..
-00001b60: 00da 0965 6e75 6d65 7261 7465 7257 0000  ...enumeraterW..
-00001b70: 0072 0500 0000 7258 0000 0072 2100 0000  .r....rX...r!...
-00001b80: 7272 0000 0072 5e00 0000 7223 0000 0072  rr...r^...r#...r
-00001b90: 2c00 0000 7219 0000 0029 0872 4600 0000  ,...r....).rF...
-00001ba0: 724e 0000 0072 1c00 0000 da05 696e 6f64  rN...r......inod
-00001bb0: 6572 6500 0000 721d 0000 0072 1a00 0000  ere...r....r....
-00001bc0: 721b 0000 0072 2400 0000 7224 0000 0072  r....r$...r$...r
-00001bd0: 2500 0000 da09 6c69 7374 5f69 6e66 6fe4  %.....list_info.
-00001be0: 0000 0073 2200 0000 0801 0402 1001 1401  ...s"...........
-00001bf0: 1001 0401 0280 0801 0a01 0402 1a01 0a01  ................
-00001c00: 0a02 0402 0401 0a01 1002 7a19 466f 616d  ..........z.Foam
-00001c10: 5472 616e 7366 6f72 6d65 722e 6c69 7374  Transformer.list
-00001c20: 5f69 6e66 6f63 0200 0000 0000 0000 0000  _infoc..........
-00001c30: 0000 0600 0000 0400 0000 4300 0000 73aa  ..........C...s.
-00001c40: 0000 0074 007c 0183 017d 017c 015c 027d  ...t.|...}.|.\.}
-00001c50: 027d 0374 017c 0274 0283 0273 0f4a 0082  .}.t.|.t...s.J..
-00001c60: 017c 026a 037d 047c 047d 057c 026a 0464  .|.j.}.|.}.|.j.d
-00001c70: 0075 0172 207c 0564 017c 026a 0417 0037  .u.r |.d.|.j...7
-00001c80: 007d 057c 026a 0564 0075 0172 2e7c 0564  .}.|.j.d.u.r.|.d
-00001c90: 027c 026a 059b 0064 039d 0337 007d 057c  .|.j...d...7.}.|
-00001ca0: 026a 0664 0075 0172 3b7c 0564 047c 026a  .j.d.u.r;|.d.|.j
-00001cb0: 069b 009d 0237 007d 0574 017c 0474 0783  .....7.}.t.|.t..
-00001cc0: 0272 4474 087c 0483 017d 0474 017c 0574  .rDt.|...}.t.|.t
-00001cd0: 0783 0272 4d74 087c 0583 017d 057c 057c  ...rMt.|...}.|.|
-00001ce0: 035f 0974 0a7c 047c 0383 0253 0029 054e  ._.t.|.|...S.).N
-00001cf0: 726f 0000 007a 060a 4c69 7374 3cda 013e  ro...z..List<..>
-00001d00: 7226 0000 0029 0b72 4000 0000 7257 0000  r&...).r@...rW..
-00001d10: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00001d20: 721c 0000 0072 1d00 0000 7223 0000 0072  r....r....r#...r
-00001d30: 2100 0000 7275 0000 0072 0900 0000 2906  !...ru...r....).
-00001d40: 7246 0000 0072 4e00 0000 7286 0000 00da  rF...rN...r.....
-00001d50: 0874 6865 5f6c 6973 7472 1a00 0000 5a0d  .the_listr....Z.
-00001d60: 6e61 6d65 5f69 6e74 6572 6e61 6c72 2400  name_internalr$.
-00001d70: 0000 7224 0000 0072 2500 0000 da0f 6c69  ..r$...r%.....li
-00001d80: 7374 5f61 7373 6967 6e6d 656e 74fb 0000  st_assignment...
-00001d90: 0073 2200 0000 0801 0802 0e01 0602 0401  .s".............
-00001da0: 0a02 0e01 0a02 1201 0a02 1001 0a02 0801  ................
-00001db0: 0a01 0801 0602 0a01 7a1f 466f 616d 5472  ........z.FoamTr
-00001dc0: 616e 7366 6f72 6d65 722e 6c69 7374 5f61  ansformer.list_a
-00001dd0: 7373 6967 6e6d 656e 7463 0200 0000 0000  ssignmentc......
-00001de0: 0000 0000 0000 0300 0000 0700 0000 4300  ..............C.
-00001df0: 0000 7370 0000 0064 0164 0284 007c 0144  ..sp...d.d...|.D
-00001e00: 0083 017d 017c 01a0 0064 03a1 017d 0274  ...}.|...d...}.t
-00001e10: 017c 0183 0164 046b 0272 2174 027c 0274  .|...d.k.r!t.|.t
-00001e20: 037c 0164 0519 007c 0164 0319 007c 0164  .|.d...|.d...|.d
-00001e30: 0619 0083 0383 0253 0074 017c 0183 0164  .......S.t.|...d
-00001e40: 076b 0272 3474 027c 0274 037c 0164 0519  .k.r4t.|.t.|.d..
-00001e50: 007c 0164 0619 0064 088d 0283 0253 0074  .|.d...d.....S.t
-00001e60: 047c 0183 0182 0129 094e 6301 0000 0000  .|.....).Nc.....
-00001e70: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-00001e80: 0000 0072 3a00 0000 7227 0000 0072 2400  ...r:...r'...r$.
-00001e90: 0000 7264 0000 0072 2400 0000 7224 0000  ..rd...r$...r$..
-00001ea0: 0072 2500 0000 723d 0000 0016 0100 0072  .r%...r=.......r
-00001eb0: 3e00 0000 7a38 466f 616d 5472 616e 7366  >...z8FoamTransf
-00001ec0: 6f72 6d65 722e 6469 6d65 6e73 696f 6e5f  ormer.dimension_
-00001ed0: 6173 7369 676e 6d65 6e74 2e3c 6c6f 6361  assignment.<loca
-00001ee0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7201  ls>.<listcomp>r.
-00001ef0: 0000 00e9 0300 0000 7270 0000 00e9 feff  ........rp......
-00001f00: ffff e902 0000 0029 0172 7100 0000 2905  .......).rq...).
-00001f10: 7272 0000 0072 5e00 0000 7209 0000 0072  rr...r^...r....r
-00001f20: 1200 0000 725f 0000 0072 8100 0000 7224  ....r_...r....r$
-00001f30: 0000 0072 2400 0000 7225 0000 00da 1464  ...r$...r%.....d
-00001f40: 696d 656e 7369 6f6e 5f61 7373 6967 6e6d  imension_assignm
-00001f50: 656e 7415 0100 0073 0e00 0000 0e01 0a01  ent....s........
-00001f60: 0c02 1e01 0c01 1a01 0802 7a24 466f 616d  ..........z$Foam
-00001f70: 5472 616e 7366 6f72 6d65 722e 6469 6d65  Transformer.dime
-00001f80: 6e73 696f 6e5f 6173 7369 676e 6d65 6e74  nsion_assignment
-00001f90: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-00001fa0: 0003 0000 0043 0000 0073 3600 0000 6401  .....C...s6...d.
-00001fb0: 6402 8400 7c01 4400 8301 7d01 7400 7c01  d...|.D...}.t.|.
-00001fc0: 8301 6403 6b03 7211 7401 7c01 8301 8201  ..d.k.r.t.|.....
-00001fd0: 7c01 a002 6404 a101 7d02 7403 7c02 6405  |...d...}.t.|.d.
-00001fe0: 8302 5300 2906 4e63 0100 0000 0000 0000  ..S.).Nc........
-00001ff0: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
-00002000: 723a 0000 0072 2700 0000 7224 0000 0072  r:...r'...r$...r
-00002010: 6400 0000 7224 0000 0072 2400 0000 7225  d...r$...r$...r%
-00002020: 0000 0072 3d00 0000 2101 0000 723e 0000  ...r=...!...r>..
-00002030: 007a 3446 6f61 6d54 7261 6e73 666f 726d  .z4FoamTransform
-00002040: 6572 2e6d 6163 726f 5f61 7373 6967 6e6d  er.macro_assignm
-00002050: 656e 742e 3c6c 6f63 616c 733e 2e3c 6c69  ent.<locals>.<li
-00002060: 7374 636f 6d70 3e72 0800 0000 7201 0000  stcomp>r....r...
-00002070: 00da 0029 0472 5e00 0000 7280 0000 0072  ...).r^...r....r
-00002080: 7200 0000 7209 0000 0072 8100 0000 7224  r...r....r....r$
-00002090: 0000 0072 2400 0000 7225 0000 00da 106d  ...r$...r%.....m
-000020a0: 6163 726f 5f61 7373 6967 6e6d 656e 7420  acro_assignment 
-000020b0: 0100 0073 0a00 0000 0e01 0c01 0801 0a01  ...s............
-000020c0: 0a01 7a20 466f 616d 5472 616e 7366 6f72  ..z FoamTransfor
-000020d0: 6d65 722e 6d61 6372 6f5f 6173 7369 676e  mer.macro_assign
-000020e0: 6d65 6e74 6302 0000 0000 0000 0000 0000  mentc...........
-000020f0: 0003 0000 0003 0000 0043 0000 0073 4e00  .........C...sN.
-00002100: 0000 6401 6402 8400 7c01 4400 8301 7d01  ..d.d...|.D...}.
-00002110: 7400 7c01 8301 6403 6b03 7211 7401 7c01  t.|...d.k.r.t.|.
-00002120: 8301 8201 7c01 6404 1900 7d02 7402 7c02  ....|.d...}.t.|.
-00002130: 6405 8302 721e 7c02 a003 a100 7d02 7c01  d...r.|.....}.|.
-00002140: 6406 1900 9b00 6407 7c02 9b00 9d03 5300  d.....d.|.....S.
-00002150: 2908 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
-00002160: 0200 0000 0400 0000 5300 0000 723a 0000  ........S...r:..
-00002170: 0072 2700 0000 7224 0000 0072 6400 0000  .r'...r$...rd...
-00002180: 7224 0000 0072 2400 0000 7225 0000 0072  r$...r$...r%...r
-00002190: 3d00 0000 2801 0000 723e 0000 007a 3046  =...(...r>...z0F
-000021a0: 6f61 6d54 7261 6e73 666f 726d 6572 2e65  oamTransformer.e
-000021b0: 7175 616c 5f61 7373 6967 6e2e 3c6c 6f63  qual_assign.<loc
-000021c0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
-000021d0: 8c00 0000 7208 0000 0072 3800 0000 7201  ....r....r8...r.
-000021e0: 0000 00da 013d 2904 725e 0000 0072 5f00  .....=).r^...r_.
-000021f0: 0000 727c 0000 0072 3800 0000 2903 7246  ..r|...r8...).rF
-00002200: 0000 0072 4e00 0000 7214 0000 0072 2400  ...rN...r....r$.
-00002210: 0000 7224 0000 0072 2500 0000 da0c 6571  ..r$...r%.....eq
-00002220: 7561 6c5f 6173 7369 676e 2701 0000 730e  ual_assign'...s.
-00002230: 0000 000e 010c 0108 0108 010a 0108 0112  ................
-00002240: 017a 1c46 6f61 6d54 7261 6e73 666f 726d  .z.FoamTransform
-00002250: 6572 2e65 7175 616c 5f61 7373 6967 6e63  er.equal_assignc
-00002260: 0200 0000 0000 0000 0000 0000 0700 0000  ................
-00002270: 0500 0000 4300 0000 736e 0000 0064 0164  ....C...sn...d.d
-00002280: 0284 007c 0144 0083 017d 0174 007c 0183  ...|.D...}.t.|..
-00002290: 0164 036b 0272 127c 015c 027d 027d 036e  .d.k.r.|.\.}.}.n
-000022a0: 177c 01a0 0164 04a1 017d 027c 01a0 0164  .|...d...}.|...d
-000022b0: 04a1 017d 0464 05a0 027c 01a1 017d 057c  ...}.d...|...}.|
-000022c0: 0464 067c 059b 0064 079d 0317 007d 037c  .d.|...d.....}.|
-000022d0: 0264 0817 007c 0317 007d 0674 037c 0674  .d...|...}.t.|.t
-000022e0: 047c 027c 0383 0283 0253 0029 094e 6301  .|.|.....S.).Nc.
-000022f0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00002300: 0000 0053 0000 0072 3a00 0000 7227 0000  ...S...r:...r'..
-00002310: 0072 2400 0000 7264 0000 0072 2400 0000  .r$...rd...r$...
-00002320: 7224 0000 0072 2500 0000 723d 0000 0031  r$...r%...r=...1
-00002330: 0100 0072 3e00 0000 7a38 466f 616d 5472  ...r>...z8FoamTr
-00002340: 616e 7366 6f72 6d65 722e 6469 7265 6374  ansformer.direct
-00002350: 6976 655f 6173 7369 676e 6d65 6e74 2e3c  ive_assignment.<
-00002360: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00002370: 703e 728c 0000 0072 0100 0000 7a02 2c20  p>r....r....z., 
-00002380: 727a 0000 0072 7b00 0000 726f 0000 0029  rz...r{...ro...)
-00002390: 0572 5e00 0000 7272 0000 0072 2c00 0000  .r^...rr...r,...
-000023a0: 7209 0000 0072 0e00 0000 2907 7246 0000  r....r....).rF..
-000023b0: 0072 4e00 0000 7260 0000 00da 0763 6f6e  .rN...r`.....con
-000023c0: 7465 6e74 da0d 6675 6e63 7469 6f6e 5f6e  tent..function_n
-000023d0: 616d 65da 0961 7267 756d 656e 7473 da03  ame..arguments..
-000023e0: 6b65 7972 2400 0000 7224 0000 0072 2500  keyr$...r$...r%.
-000023f0: 0000 da14 6469 7265 6374 6976 655f 6173  ....directive_as
-00002400: 7369 676e 6d65 6e74 3001 0000 7312 0000  signment0...s...
-00002410: 000e 010c 010a 010a 020a 010a 0110 010c  ................
-00002420: 0110 017a 2446 6f61 6d54 7261 6e73 666f  ...z$FoamTransfo
-00002430: 726d 6572 2e64 6972 6563 7469 7665 5f61  rmer.directive_a
-00002440: 7373 6967 6e6d 656e 7463 0200 0000 0000  ssignmentc......
-00002450: 0000 0000 0000 0500 0000 0700 0000 4300  ..............C.
-00002460: 0000 73ac 0000 0074 007c 0183 017d 0164  ..s....t.|...}.d
-00002470: 007d 0274 017c 0183 0164 016b 0272 117c  .}.t.|...d.k.r.|
-00002480: 015c 027d 037d 046e 1974 017c 0183 0164  .\.}.}.n.t.|...d
-00002490: 026b 0272 267c 015c 037d 037d 027d 047c  .k.r&|.\.}.}.}.|
-000024a0: 02a0 0264 03a1 0173 2574 037c 0183 0182  ...d...s%t.|....
-000024b0: 016e 0474 037c 0183 0182 0174 047c 0483  .n.t.|.....t.|..
-000024c0: 017d 047c 04a0 0264 04a1 0172 447c 04a0  .}.|...d...rD|..
-000024d0: 0564 0564 06a1 0264 0719 007d 047c 04a0  .d.d...d...}.|..
-000024e0: 0664 0564 06a1 0264 0819 007d 046e 087c  .d.d...d...}.n.|
-000024f0: 0464 0164 0985 0219 00a0 07a1 007d 0474  .d.d.........}.t
-00002500: 087c 0374 097c 037c 047c 0264 0a8d 0383  .|.t.|.|.|.d....
-00002510: 0253 0029 0b4e 728c 0000 0072 8a00 0000  .S.).Nr....r....
-00002520: 7279 0000 007a 0323 7b0a 7226 0000 0072  ry...z.#{.r&...r
-00002530: 0800 0000 7270 0000 0072 0100 0000 e9fd  ....rp...r......
-00002540: ffff ff29 0172 6000 0000 290a 7240 0000  ...).r`...).r@..
-00002550: 0072 5e00 0000 727d 0000 0072 8000 0000  .r^...r}...r....
-00002560: 7221 0000 0072 2d00 0000 da06 7273 706c  r!...r-.....rspl
-00002570: 6974 da05 7374 7269 7072 0900 0000 720a  it..stripr....r.
-00002580: 0000 0029 0572 4600 0000 724e 0000 0072  ...).rF...rN...r
-00002590: 6000 0000 721a 0000 00da 0463 6f64 6572  `...r......coder
-000025a0: 2400 0000 7224 0000 0072 2500 0000 da0f  $...r$...r%.....
-000025b0: 636f 6465 5f61 7373 6967 6e6d 656e 743c  code_assignment<
-000025c0: 0100 0073 2000 0000 0801 0401 0c01 0a01  ...s ...........
-000025d0: 0c01 0a01 0a01 0801 02ff 0803 0801 0a01  ................
-000025e0: 1001 1201 1002 1401 7a1f 466f 616d 5472  ........z.FoamTr
-000025f0: 616e 7366 6f72 6d65 722e 636f 6465 5f61  ansformer.code_a
-00002600: 7373 6967 6e6d 656e 7463 0200 0000 0000  ssignmentc......
-00002610: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-00002620: 0000 731a 0000 0074 007c 0183 017d 0174  ..s....t.|...}.t
-00002630: 017c 0164 0119 006a 0264 0217 0083 0153  .|.d...j.d.....S
-00002640: 0029 034e 7201 0000 0072 2600 0000 2903  .).Nr....r&...).
-00002650: 7240 0000 0072 1100 0000 7214 0000 0072  r@...r....r....r
-00002660: 4500 0000 7224 0000 0072 2400 0000 7225  E...r$...r$...r%
-00002670: 0000 00da 1273 7065 6369 616c 5f64 6972  .....special_dir
-00002680: 6563 7469 7665 734f 0100 0073 0400 0000  ectivesO...s....
-00002690: 0801 1201 7a22 466f 616d 5472 616e 7366  ....z"FoamTransf
-000026a0: 6f72 6d65 722e 7370 6563 6961 6c5f 6469  ormer.special_di
-000026b0: 7265 6374 6976 6573 4e29 1a72 1e00 0000  rectivesN).r....
-000026c0: 721f 0000 0072 2000 0000 7248 0000 0072  r....r ...rH...r
-000026d0: 4b00 0000 724f 0000 0072 5000 0000 7251  K...rO...rP...rQ
-000026e0: 0000 0072 5200 0000 7253 0000 0072 5400  ...rR...rS...rT.
-000026f0: 0000 725b 0000 0072 6000 0000 7261 0000  ..r[...r`...ra..
-00002700: 0072 6a00 0000 7277 0000 0072 7f00 0000  .rj...rw...r....
-00002710: 7282 0000 0072 8600 0000 7289 0000 0072  r....r....r....r
-00002720: 8d00 0000 728f 0000 0072 9100 0000 7296  ....r....r....r.
-00002730: 0000 0072 9b00 0000 729c 0000 0072 2400  ...r....r....r$.
-00002740: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
-00002750: 0072 3300 0000 4a00 0000 7330 0000 0008  .r3...J...s0....
-00002760: 0008 0108 0308 0308 0308 0308 0308 0308  ................
-00002770: 0308 0308 0908 0508 0a08 0e08 2708 2d08  ............'.-.
-00002780: 0708 1708 1a08 0b08 0708 0908 0c0c 1372  ...............r
-00002790: 3300 0000 7227 0000 0029 27da 075f 5f64  3...r'...)'..__d
-000027a0: 6f63 5f5f da0b 6461 7461 636c 6173 7365  oc__..dataclasse
-000027b0: 7372 0200 0000 da07 7061 7468 6c69 6272  sr......pathlibr
-000027c0: 0300 0000 5a04 6c61 726b 7204 0000 0072  ....Z.larkr....r
-000027d0: 0500 0000 7206 0000 005a 0f6c 6172 6b2e  ....r....Z.lark.
-000027e0: 6578 6365 7074 696f 6e73 7207 0000 00da  exceptionsr.....
-000027f0: 0361 7374 7209 0000 0072 0a00 0000 720b  .astr....r....r.
-00002800: 0000 0072 0c00 0000 720d 0000 0072 0e00  ...r....r....r..
-00002810: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00002820: 0072 1200 0000 7213 0000 00da 085f 5f66  .r....r......__f
-00002830: 696c 655f 5fda 0861 6273 6f6c 7574 65da  ile__..absolute.
-00002840: 0670 6172 656e 74da 0468 6572 65da 0972  .parent..here..r
-00002850: 6561 645f 7465 7874 7236 0000 005a 1067  ead_textr6...Z.g
-00002860: 7261 6d6d 6172 5f61 6476 616e 6365 6472  rammar_advancedr
-00002870: 2f00 0000 7231 0000 0072 3200 0000 7219  /...r1...r2...r.
-00002880: 0000 0072 3000 0000 7238 0000 0072 4000  ...r0...r8...r@.
-00002890: 0000 7244 0000 0072 3300 0000 7224 0000  ..rD...r3...r$..
-000028a0: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
-000028b0: da08 3c6d 6f64 756c 653e 0100 0000 7326  ..<module>....s&
-000028c0: 0000 0004 000c 020c 0114 020c 0134 020e  .............4..
-000028d0: 0e0c 020c 010e 020e 010a 0202 0310 010a  ................
-000028e0: 0708 1008 0408 0414 08                   .........
+000003c0: 0043 0000 0073 8c00 0000 7400 7c00 7401  .C...s....t.|.t.
+000003d0: 8302 7209 7c00 a002 a100 7d00 6401 a003  ..r.|.....}.d...
+000003e0: 6402 6403 8400 7c00 a004 6401 a101 4400  d.d...|...d...D.
+000003f0: 8301 a101 7d00 7c00 a005 6401 a101 731f  ....}.|...d...s.
+00000400: 7c00 6401 3700 7d00 7c01 6400 7500 7239  |.d.7.}.|.d.u.r9
+00000410: 7a07 7406 a007 7c00 a101 7d02 5700 6e15  z.t...|...}.W.n.
+00000420: 0400 7408 7938 0100 0100 0100 7409 a007  ..t.y8......t...
+00000430: 7c00 a101 7d02 5900 6e08 7700 740a 7c01  |...}.Y.n.w.t.|.
+00000440: 1900 a007 7c00 a101 7d02 740b 8300 a00c  ....|...}.t.....
+00000450: 7c02 a101 5300 2904 4eda 010a 6301 0000  |...S.).N...c...
+00000460: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00000470: 0073 0000 0073 1800 0000 8100 7c00 5d07  .s...s......|.].
+00000480: 7d01 7c01 a000 a100 5600 0100 7102 6400  }.|.....V...q.d.
+00000490: 5300 a901 4e29 01da 0672 7374 7269 7029  S...N)...rstrip)
+000004a0: 02da 022e 30da 046c 696e 6572 2400 0000  ....0..liner$...
+000004b0: 7224 0000 0072 2500 0000 da09 3c67 656e  r$...r%.....<gen
+000004c0: 6578 7072 3e2e 0000 0073 0400 0000 0280  expr>....s......
+000004d0: 1600 7a18 7061 7273 652e 3c6c 6f63 616c  ..z.parse.<local
+000004e0: 733e 2e3c 6765 6e65 7870 723e 290d da0a  s>.<genexpr>)...
+000004f0: 6973 696e 7374 616e 6365 da05 6279 7465  isinstance..byte
+00000500: 73da 0664 6563 6f64 65da 046a 6f69 6eda  s..decode..join.
+00000510: 0573 706c 6974 da08 656e 6473 7769 7468  .split..endswith
+00000520: da0b 6c61 726b 5f70 6172 7365 72da 0570  ..lark_parser..p
+00000530: 6172 7365 7207 0000 00da 146c 6172 6b5f  arser......lark_
+00000540: 7061 7273 6572 5f61 6476 616e 6365 64da  parser_advanced.
+00000550: 0770 6172 7365 7273 da0f 466f 616d 5472  .parsers..FoamTr
+00000560: 616e 7366 6f72 6d65 72da 0974 7261 6e73  ansformer..trans
+00000570: 666f 726d 2903 da04 7465 7874 da07 6772  form)...text..gr
+00000580: 616d 6d61 72da 0474 7265 6572 2400 0000  ammar..treer$...
+00000590: 7224 0000 0072 2500 0000 7233 0000 002a  r$...r%...r3...*
+000005a0: 0000 0073 1a00 0000 0a01 0801 1a02 0a01  ...s............
+000005b0: 0801 0802 0201 0e01 0c01 0e01 02ff 0e03  ................
+000005c0: 0c02 7233 0000 0063 0100 0000 0000 0000  ..r3...c........
+000005d0: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+000005e0: 7308 0000 007c 00a0 00a1 0053 0072 2700  s....|.....S.r'.
+000005f0: 0000 2901 da04 6475 6d70 2901 723a 0000  ..)...dump).r:..
+00000600: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
+00000610: 723b 0000 003d 0000 00f3 0200 0000 0801  r;...=..........
+00000620: 723b 0000 0063 0100 0000 0000 0000 0000  r;...c..........
+00000630: 0000 0100 0000 0200 0000 4300 0000 730e  ..........C...s.
+00000640: 0000 0064 0164 0284 007c 0044 0083 0153  ...d.d...|.D...S
+00000650: 0029 034e 6301 0000 0000 0000 0000 0000  .).Nc...........
+00000660: 0002 0000 0004 0000 0053 0000 00f3 1800  .........S......
+00000670: 0000 6700 7c00 5d08 7d01 7c01 6400 7501  ..g.|.].}.|.d.u.
+00000680: 7202 7c01 9102 7102 5300 7227 0000 0072  r.|...q.S.r'...r
+00000690: 2400 0000 a902 7229 0000 00da 0469 7465  $.....r).....ite
+000006a0: 6d72 2400 0000 7224 0000 0072 2500 0000  mr$...r$...r%...
+000006b0: da0a 3c6c 6973 7463 6f6d 703e 4200 0000  ..<listcomp>B...
+000006c0: f302 0000 0018 007a 2666 696c 7465 725f  .......z&filter_
+000006d0: 6e6f 5f6e 6577 6c69 6e65 732e 3c6c 6f63  no_newlines.<loc
+000006e0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
+000006f0: 2400 0000 2901 da05 6974 656d 7372 2400  $...)...itemsr$.
+00000700: 0000 7224 0000 0072 2500 0000 da12 6669  ..r$...r%.....fi
+00000710: 6c74 6572 5f6e 6f5f 6e65 776c 696e 6573  lter_no_newlines
+00000720: 4100 0000 7302 0000 000e 0172 4300 0000  A...s......rC...
+00000730: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000740: 0008 0000 0043 0000 0073 2e00 0000 7400  .....C...s....t.
+00000750: 7c00 8301 7d00 7a05 7401 7c00 8301 5700  |...}.z.t.|...W.
+00000760: 5300 0400 7402 7916 0100 0100 0100 7403  S...t.y.......t.
+00000770: 7c00 8301 0600 5900 5300 7700 7227 0000  |.....Y.S.w.r'..
+00000780: 0029 0472 2100 0000 7223 0000 00da 0a56  .).r!...r#.....V
+00000790: 616c 7565 4572 726f 72da 0566 6c6f 6174  alueError..float
+000007a0: 2901 da06 6e75 6d62 6572 7224 0000 0072  )...numberr$...r
+000007b0: 2400 0000 7225 0000 00da 125f 636f 6e76  $...r%....._conv
+000007c0: 6572 745f 746f 5f6e 756d 6265 7245 0000  ert_to_numberE..
+000007d0: 0073 0c00 0000 0801 0201 0a01 0c01 0c01  .s..............
+000007e0: 02ff 7247 0000 0063 0000 0000 0000 0000  ..rG...c........
+000007f0: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
+00000800: 73c4 0000 0065 005a 0164 005a 0264 0164  s....e.Z.d.Z.d.d
+00000810: 0284 005a 0364 0364 0484 005a 0464 0564  ...Z.d.d...Z.d.d
+00000820: 0684 005a 0564 0764 0884 005a 0664 0964  ...Z.d.d...Z.d.d
+00000830: 0a84 005a 0764 0b64 0c84 005a 0864 0d64  ...Z.d.d...Z.d.d
+00000840: 0e84 005a 0964 0f64 1084 005a 0a64 1164  ...Z.d.d...Z.d.d
+00000850: 1284 005a 0b64 1364 1484 005a 0c64 1564  ...Z.d.d...Z.d.d
+00000860: 1684 005a 0d64 1764 1884 005a 0e64 1964  ...Z.d.d...Z.d.d
+00000870: 1a84 005a 0f64 1b64 1c84 005a 1064 1d64  ...Z.d.d...Z.d.d
+00000880: 1e84 005a 1164 1f64 2084 005a 1264 2164  ...Z.d.d ..Z.d!d
+00000890: 2284 005a 1364 2364 2484 005a 1464 2564  "..Z.d#d$..Z.d%d
+000008a0: 2684 005a 1564 2764 2884 005a 1664 2964  &..Z.d'd(..Z.d)d
+000008b0: 2a84 005a 1764 2b64 2c84 005a 1864 2d64  *..Z.d+d,..Z.d-d
+000008c0: 2e84 005a 1964 2f53 0029 3072 3600 0000  ...Z.d/S.)0r6...
+000008d0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+000008e0: 0002 0000 0043 0000 0073 0800 0000 7400  .....C...s....t.
+000008f0: 7c01 8301 5300 7227 0000 0029 0172 4700  |...S.r'...).rG.
+00000900: 0000 a902 da04 7365 6c66 da05 746f 6b65  ......self..toke
+00000910: 6e72 2400 0000 7224 0000 0072 2500 0000  nr$...r$...r%...
+00000920: da0d 5349 474e 4544 5f4e 554d 4245 524e  ..SIGNED_NUMBERN
+00000930: 0000 0072 3c00 0000 7a1d 466f 616d 5472  ...r<...z.FoamTr
+00000940: 616e 7366 6f72 6d65 722e 5349 474e 4544  ansformer.SIGNED
+00000950: 5f4e 554d 4245 5263 0200 0000 0000 0000  _NUMBERc........
+00000960: 0000 0000 0200 0000 0100 0000 4300 0000  ............C...
+00000970: f306 0000 007c 016a 0053 0072 2700 0000  .....|.j.S.r'...
+00000980: a901 7214 0000 0072 4800 0000 7224 0000  ..r....rH...r$..
+00000990: 0072 2400 0000 7225 0000 00da 0543 4e41  .r$...r%.....CNA
+000009a0: 4d45 5100 0000 f302 0000 0006 017a 1546  MEQ..........z.F
+000009b0: 6f61 6d54 7261 6e73 666f 726d 6572 2e43  oamTransformer.C
+000009c0: 4e41 4d45 6302 0000 0000 0000 0000 0000  NAMEc...........
+000009d0: 0002 0000 0001 0000 0043 0000 0073 0400  .........C...s..
+000009e0: 0000 6400 5300 7227 0000 0072 2400 0000  ..d.S.r'...r$...
+000009f0: a902 7249 0000 00da 056e 6f64 6573 7224  ..rI.....nodesr$
+00000a00: 0000 0072 2400 0000 7225 0000 00da 074e  ...r$...r%.....N
+00000a10: 4557 4c49 4e45 5400 0000 7302 0000 0004  EWLINET...s.....
+00000a20: 017a 1746 6f61 6d54 7261 6e73 666f 726d  .z.FoamTransform
+00000a30: 6572 2e4e 4557 4c49 4e45 6302 0000 0000  er.NEWLINEc.....
+00000a40: 0000 0000 0000 0002 0000 0001 0000 0043  ...............C
+00000a50: 0000 0072 4c00 0000 7227 0000 0072 4d00  ...rL...r'...rM.
+00000a60: 0000 7248 0000 0072 2400 0000 7224 0000  ..rH...r$...r$..
+00000a70: 0072 2500 0000 da0e 4553 4341 5045 445f  .r%.....ESCAPED_
+00000a80: 5354 5249 4e47 5700 0000 724f 0000 007a  STRINGW...rO...z
+00000a90: 1e46 6f61 6d54 7261 6e73 666f 726d 6572  .FoamTransformer
+00000aa0: 2e45 5343 4150 4544 5f53 5452 494e 4763  .ESCAPED_STRINGc
+00000ab0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000ac0: 0100 0000 4300 0000 724c 0000 0072 2700  ....C...rL...r'.
+00000ad0: 0000 724d 0000 0072 4800 0000 7224 0000  ..rM...rH...r$..
+00000ae0: 0072 2400 0000 7225 0000 00da 0b44 4f55  .r$...r%.....DOU
+00000af0: 424c 455f 4e41 4d45 5a00 0000 724f 0000  BLE_NAMEZ...rO..
+00000b00: 007a 1b46 6f61 6d54 7261 6e73 666f 726d  .z.FoamTransform
+00000b10: 6572 2e44 4f55 424c 455f 4e41 4d45 6302  er.DOUBLE_NAMEc.
+00000b20: 0000 0000 0000 0000 0000 0002 0000 0001  ................
+00000b30: 0000 0043 0000 0072 4c00 0000 7227 0000  ...C...rL...r'..
+00000b40: 0072 4d00 0000 7248 0000 0072 2400 0000  .rM...rH...r$...
+00000b50: 7224 0000 0072 2500 0000 da0b 5452 4950  r$...r%.....TRIP
+00000b60: 4c45 5f4e 414d 455d 0000 0072 4f00 0000  LE_NAME]...rO...
+00000b70: 7a1b 466f 616d 5472 616e 7366 6f72 6d65  z.FoamTransforme
+00000b80: 722e 5452 4950 4c45 5f4e 414d 4563 0200  r.TRIPLE_NAMEc..
+00000b90: 0000 0000 0000 0000 0000 0200 0000 0100  ................
+00000ba0: 0000 4300 0000 724c 0000 0072 2700 0000  ..C...rL...r'...
+00000bb0: 724d 0000 0072 4800 0000 7224 0000 0072  rM...rH...r$...r
+00000bc0: 2400 0000 7225 0000 00da 0545 514b 4559  $...r%.....EQKEY
+00000bd0: 6000 0000 724f 0000 007a 1546 6f61 6d54  `...rO...z.FoamT
+00000be0: 7261 6e73 666f 726d 6572 2e45 514b 4559  ransformer.EQKEY
+00000bf0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000c00: 0001 0000 0043 0000 0072 4c00 0000 7227  .....C...rL...r'
+00000c10: 0000 0072 4d00 0000 7248 0000 0072 2400  ...rM...rH...r$.
+00000c20: 0000 7224 0000 0072 2500 0000 da05 4d41  ..r$...r%.....MA
+00000c30: 4352 4f63 0000 0072 4f00 0000 7a15 466f  CROc...rO...z.Fo
+00000c40: 616d 5472 616e 7366 6f72 6d65 722e 4d41  amTransformer.MA
+00000c50: 4352 4f63 0200 0000 0000 0000 0000 0000  CROc............
+00000c60: 0200 0000 0300 0000 4300 0000 f312 0000  ........C.......
+00000c70: 0074 0064 0164 0284 007c 0144 0083 0183  .t.d.d...|.D....
+00000c80: 0153 0029 034e 6301 0000 0000 0000 0000  .S.).Nc.........
+00000c90: 0000 0002 0000 0005 0000 0053 0000 0073  ...........S...s
+00000ca0: 2400 0000 6700 7c00 5d0e 7d01 7400 7c01  $...g.|.].}.t.|.
+00000cb0: 7401 8302 720e 7c01 6a02 6400 6b02 7302  t...r.|.j.d.k.s.
+00000cc0: 7c01 9102 7102 5300 2901 7252 0000 00a9  |...q.S.).rR....
+00000cd0: 0372 2c00 0000 7205 0000 00da 0474 7970  .r,...r......typ
+00000ce0: 6572 3e00 0000 7224 0000 0072 2400 0000  er>...r$...r$...
+00000cf0: 7225 0000 0072 4000 0000 6800 0000 f310  r%...r@...h.....
+00000d00: 0000 0006 0002 0208 0102 fd08 0302 fd02  ................
+00000d10: 0106 ff7a 3146 6f61 6d54 7261 6e73 666f  ...z1FoamTransfo
+00000d20: 726d 6572 2e64 696d 656e 7369 6f6e 5f73  rmer.dimension_s
+00000d30: 6574 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  et.<locals>.<lis
+00000d40: 7463 6f6d 703e 2901 720d 0000 00a9 0272  tcomp>).r......r
+00000d50: 4900 0000 7242 0000 0072 2400 0000 7224  I...rB...r$...r$
+00000d60: 0000 0072 2500 0000 da0d 6469 6d65 6e73  ...r%.....dimens
+00000d70: 696f 6e5f 7365 7466 0000 00f3 0a00 0000  ion_setf........
+00000d80: 0201 0601 0202 04fe 04ff 7a1d 466f 616d  ..........z.Foam
+00000d90: 5472 616e 7366 6f72 6d65 722e 6469 6d65  Transformer.dime
+00000da0: 6e73 696f 6e5f 7365 7463 0200 0000 0000  nsion_setc......
+00000db0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+00000dc0: 0000 731c 0000 0074 007c 0183 0164 016b  ..s....t.|...d.k
+00000dd0: 0372 0874 0182 0174 027c 0164 0219 0083  .r.t...t.|.d....
+00000de0: 0153 00a9 034e 7208 0000 0072 0100 0000  .S...Nr....r....
+00000df0: 2903 da03 6c65 6eda 0c52 756e 7469 6d65  )...len..Runtime
+00000e00: 4572 726f 7272 2100 0000 7250 0000 0072  Errorr!...rP...r
+00000e10: 2400 0000 7224 0000 0072 2500 0000 da09  $...r$...r%.....
+00000e20: 6469 7265 6374 6976 656f 0000 0073 0600  directiveo...s..
+00000e30: 0000 0c01 0401 0c01 7a19 466f 616d 5472  ........z.FoamTr
+00000e40: 616e 7366 6f72 6d65 722e 6469 7265 6374  ansformer.direct
+00000e50: 6976 6563 0200 0000 0000 0000 0000 0000  ivec............
+00000e60: 0200 0000 0300 0000 4300 0000 7258 0000  ........C...rX..
+00000e70: 0029 034e 6301 0000 0000 0000 0000 0000  .).Nc...........
+00000e80: 0002 0000 0005 0000 0053 0000 0073 2c00  .........S...s,.
+00000e90: 0000 6700 7c00 5d12 7d01 7400 7c01 7401  ..g.|.].}.t.|.t.
+00000ea0: 8302 720e 7c01 6a02 6400 6b02 7302 7c01  ..r.|.j.d.k.s.|.
+00000eb0: 6401 7501 7202 7c01 9102 7102 5300 2902  d.u.r.|...q.S.).
+00000ec0: 7252 0000 004e 7259 0000 0072 3e00 0000  rR...NrY...r>...
+00000ed0: 7224 0000 0072 2400 0000 7225 0000 0072  r$...r$...r%...r
+00000ee0: 4000 0000 7600 0000 7314 0000 0006 0002  @...v...s.......
+00000ef0: 0208 0102 fd08 0302 fd06 0402 fc02 0106  ................
+00000f00: ff7a 2846 6f61 6d54 7261 6e73 666f 726d  .z(FoamTransform
+00000f10: 6572 2e6c 6973 742e 3c6c 6f63 616c 733e  er.list.<locals>
+00000f20: 2e3c 6c69 7374 636f 6d70 3e29 0172 1000  .<listcomp>).r..
+00000f30: 0000 725c 0000 0072 2400 0000 7224 0000  ..r\...r$...r$..
+00000f40: 0072 2500 0000 da04 6c69 7374 7400 0000  .r%.....listt...
+00000f50: 725e 0000 007a 1446 6f61 6d54 7261 6e73  r^...z.FoamTrans
+00000f60: 666f 726d 6572 2e6c 6973 7463 0200 0000  former.listc....
+00000f70: 0000 0000 0000 0000 0400 0000 0400 0000  ................
+00000f80: 4300 0000 733e 0000 007c 0164 0119 007d  C...s>...|.d...}
+00000f90: 027c 026a 0064 026b 0272 137c 026a 017d  .|.j.d.k.r.|.j.}
+00000fa0: 037c 0164 0364 0085 0219 007d 016e 0264  .|.d.d.....}.n.d
+00000fb0: 007d 0374 027c 0364 0464 0584 007c 0144  .}.t.|.d.d...|.D
+00000fc0: 0083 0183 0253 0029 064e 7201 0000 00da  .....S.).Nr.....
+00000fd0: 0846 6f61 6d46 696c 6572 0800 0000 6301  .FoamFiler....c.
+00000fe0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000ff0: 0000 0053 0000 00f3 1600 0000 6900 7c00  ...S........i.|.
+00001000: 5d07 7d01 7c01 6a00 7c01 6a01 9302 7102  ].}.|.j.|.j...q.
+00001010: 5300 7224 0000 00a9 0272 1a00 0000 7214  S.r$.....r....r.
+00001020: 0000 00a9 0272 2900 0000 da04 6e6f 6465  .....r).....node
+00001030: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
+00001040: 0a3c 6469 6374 636f 6d70 3e85 0000 00f3  .<dictcomp>.....
+00001050: 0200 0000 1600 7a28 466f 616d 5472 616e  ......z(FoamTran
+00001060: 7366 6f72 6d65 722e 6669 6c65 2e3c 6c6f  sformer.file.<lo
+00001070: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
+00001080: 2903 721a 0000 0072 1400 0000 720f 0000  ).r....r....r...
+00001090: 0029 0472 4900 0000 7251 0000 005a 1066  .).rI...rQ...Z.f
+000010a0: 6972 7374 5f61 7373 6967 6e6d 656e 74da  irst_assignment.
+000010b0: 0969 6e66 6f5f 6469 6374 7224 0000 0072  .info_dictr$...r
+000010c0: 2400 0000 7225 0000 00da 0466 696c 657e  $...r%.....file~
+000010d0: 0000 0073 0c00 0000 0801 0a01 0601 0e01  ...s............
+000010e0: 0402 1401 7a14 466f 616d 5472 616e 7366  ....z.FoamTransf
+000010f0: 6f72 6d65 722e 6669 6c65 6302 0000 0000  ormer.filec.....
+00001100: 0000 0000 0000 0008 0000 0008 0000 0043  ...............C
+00001110: 0000 0073 1201 0000 6401 6402 8400 7c01  ...s....d.d...|.
+00001120: 4400 8301 7d01 6400 7d02 6400 7d03 7c01  D...}.d.}.d.}.|.
+00001130: a000 6403 a101 7d04 7401 7c01 8301 6404  ..d...}.t.|...d.
+00001140: 6b02 721b 7c01 6403 1900 7d05 6e69 7a0c  k.r.|.d...}.niz.
+00001150: 6405 6402 8400 7c01 4400 8301 a002 6406  d.d...|.D.....d.
+00001160: a101 7d06 5700 6e0b 0400 7403 7932 0100  ..}.W.n...t.y2..
+00001170: 0100 0100 6400 7d02 5900 6e06 7700 7c01  ....d.}.Y.n.w.|.
+00001180: a000 7c06 a101 7d02 6400 7d03 7404 6407  ..|...}.d.}.t.d.
+00001190: 6402 8400 7c01 4400 8301 8301 7249 6408  d...|.D.....rId.
+000011a0: a005 7c01 a101 7d07 6e24 7c01 a000 6409  ..|...}.n$|...d.
+000011b0: a101 7d07 7404 640a 640b 8400 7c01 4400  ..}.t.d.d...|.D.
+000011c0: 8301 8301 735e 640c 6402 8400 7c01 4400  ....s^d.d...|.D.
+000011d0: 8301 7d01 7c01 7265 6408 a005 7c01 a101  ..}.|.red...|...
+000011e0: 7d03 7406 7c07 7407 8302 726d 7c03 7c07  }.t.|.t...rm|.|.
+000011f0: 5f08 7c03 6400 7500 7275 7c02 6400 7500  _.|.d.u.ru|.d.u.
+00001200: 737a 7406 7c07 7407 8302 727d 7c07 7d05  szt.|.t...r}|.}.
+00001210: 6e07 7409 7c07 7c03 7c02 640d 8d03 7d05  n.t.|.|.|.d...}.
+00001220: 740a 7c04 7c05 8302 5300 290e 4e63 0100  t.|.|...S.).Nc..
+00001230: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00001240: 0000 5300 0000 723d 0000 0072 2700 0000  ..S...r=...r'...
+00001250: 7224 0000 0072 6700 0000 7224 0000 0072  r$...rg...r$...r
+00001260: 2400 0000 7225 0000 0072 4000 0000 8800  $...r%...r@.....
+00001270: 0000 7241 0000 007a 3246 6f61 6d54 7261  ..rA...z2FoamTra
+00001280: 6e73 666f 726d 6572 2e76 6172 5f61 7373  nsformer.var_ass
+00001290: 6967 6e6d 656e 742e 3c6c 6f63 616c 733e  ignment.<locals>
+000012a0: 2e3c 6c69 7374 636f 6d70 3e72 0100 0000  .<listcomp>r....
+000012b0: 7208 0000 0063 0100 0000 0000 0000 0000  r....c..........
+000012c0: 0000 0200 0000 0500 0000 5300 0000 f316  ..........S.....
+000012d0: 0000 0067 007c 005d 077d 0174 007c 0174  ...g.|.].}.t.|.t
+000012e0: 0183 0291 0271 0253 0072 2400 0000 2902  .....q.S.r$...).
+000012f0: 722c 0000 0072 0d00 0000 a902 7229 0000  r,...r......r)..
+00001300: 00da 0465 6c65 6d72 2400 0000 7224 0000  ...elemr$...r$..
+00001310: 0072 2500 0000 7240 0000 0090 0000 0073  .r%...r@.......s
+00001320: 0600 0000 0600 0a01 06ff 5463 0100 0000  ..........Tc....
+00001330: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+00001340: 5300 0000 726d 0000 0072 2400 0000 a902  S...rm...r$.....
+00001350: 722c 0000 0072 2100 0000 726e 0000 0072  r,...r!...rn...r
+00001360: 2400 0000 7224 0000 0072 2500 0000 7240  $...r$...r%...r@
+00001370: 0000 0099 0000 0072 6a00 0000 da01 20e9  .......rj..... .
+00001380: ffff ffff 6301 0000 0000 0000 0000 0000  ....c...........
+00001390: 0002 0000 0004 0000 0073 0000 0073 1a00  .........s...s..
+000013a0: 0000 8100 7c00 5d08 7d01 7400 7c01 7401  ....|.].}.t.|.t.
+000013b0: 8302 5600 0100 7102 6400 5300 7227 0000  ..V...q.d.S.r'..
+000013c0: 0072 7000 0000 7267 0000 0072 2400 0000  .rp...rg...r$...
+000013d0: 7224 0000 0072 2500 0000 722b 0000 009d  r$...r%...r+....
+000013e0: 0000 0073 0400 0000 0280 1800 7a31 466f  ...s........z1Fo
+000013f0: 616d 5472 616e 7366 6f72 6d65 722e 7661  amTransformer.va
+00001400: 725f 6173 7369 676e 6d65 6e74 2e3c 6c6f  r_assignment.<lo
+00001410: 6361 6c73 3e2e 3c67 656e 6578 7072 3e63  cals>.<genexpr>c
+00001420: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001430: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
+00001440: 005d 067d 0174 007c 0183 0191 0271 0253  .].}.t.|.....q.S
+00001450: 0072 2400 0000 2901 7221 0000 0072 6700  .r$...).r!...rg.
+00001460: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
+00001470: 0072 4000 0000 9e00 0000 7302 0000 0014  .r@.......s.....
+00001480: 0029 0272 1a00 0000 da09 6469 6d65 6e73  .).r......dimens
+00001490: 696f 6e29 0bda 0370 6f70 7260 0000 00da  ion)...popr`....
+000014a0: 0569 6e64 6578 7244 0000 00da 0361 6c6c  .indexrD.....all
+000014b0: 722f 0000 0072 2c00 0000 7210 0000 00da  r/...r,...r.....
+000014c0: 055f 6e61 6d65 7212 0000 0072 1300 0000  ._namer....r....
+000014d0: 2908 7249 0000 0072 5100 0000 725d 0000  ).rI...rQ...r]..
+000014e0: 005a 0d6e 616d 655f 696e 5f76 616c 7565  .Z.name_in_value
+000014f0: 721a 0000 0072 1400 0000 5a0f 696e 6465  r....r....Z.inde
+00001500: 785f 6469 6d65 6e73 696f 6eda 0a6c 6173  x_dimension..las
+00001510: 745f 7661 6c75 6572 2400 0000 7224 0000  t_valuer$...r$..
+00001520: 0072 2500 0000 da0e 7661 725f 6173 7369  .r%.....var_assi
+00001530: 676e 6d65 6e74 8700 0000 7344 0000 000e  gnment....sD....
+00001540: 0104 0104 010a 010c 010a 0102 0206 0102  ................
+00001550: 0104 ff06 0206 fe0c 0308 0102 ff0a 0304  ................
+00001560: 0212 010c 010a 0212 010e 0104 010a 010a  ................
+00001570: 0106 0112 0204 0104 ff06 0302 0206 0106  ................
+00001580: ff0a 037a 1e46 6f61 6d54 7261 6e73 666f  ...z.FoamTransfo
+00001590: 726d 6572 2e76 6172 5f61 7373 6967 6e6d  rmer.var_assignm
+000015a0: 656e 7463 0200 0000 0000 0000 0000 0000  entc............
+000015b0: 0300 0000 0300 0000 4300 0000 7322 0000  ........C...s"..
+000015c0: 0064 0164 0284 007c 0144 0083 017d 0274  .d.d...|.D...}.t
+000015d0: 0064 0364 0484 007c 0244 0083 0164 058d  .d.d...|.D...d..
+000015e0: 0153 0029 064e 6301 0000 0000 0000 0000  .S.).Nc.........
+000015f0: 0000 0002 0000 0005 0000 0053 0000 00f3  ...........S....
+00001600: 2400 0000 6700 7c00 5d0e 7d01 7400 7c01  $...g.|.].}.t.|.
+00001610: 6400 8302 7202 7400 7c01 6401 8302 7202  d...r.t.|.d...r.
+00001620: 7c01 9102 7102 5300 7266 0000 00a9 01da  |...q.S.rf......
+00001630: 0768 6173 6174 7472 7267 0000 0072 2400  .hasattrrg...r$.
+00001640: 0000 7224 0000 0072 2500 0000 7240 0000  ..r$...r%...r@..
+00001650: 00af 0000 0072 5b00 0000 7a30 466f 616d  .....r[...z0Foam
+00001660: 5472 616e 7366 6f72 6d65 722e 756e 6e61  Transformer.unna
+00001670: 6d65 645f 6469 6374 2e3c 6c6f 6361 6c73  med_dict.<locals
+00001680: 3e2e 3c6c 6973 7463 6f6d 703e 6301 0000  >.<listcomp>c...
+00001690: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+000016a0: 0053 0000 0072 6500 0000 7224 0000 0072  .S...re...r$...r
+000016b0: 6600 0000 7267 0000 0072 2400 0000 7224  f...rg...r$...r$
+000016c0: 0000 0072 2500 0000 7269 0000 00b5 0000  ...r%...ri......
+000016d0: 0072 6a00 0000 7a30 466f 616d 5472 616e  .rj...z0FoamTran
+000016e0: 7366 6f72 6d65 722e 756e 6e61 6d65 645f  sformer.unnamed_
+000016f0: 6469 6374 2e3c 6c6f 6361 6c73 3e2e 3c64  dict.<locals>.<d
+00001700: 6963 7463 6f6d 703e 2901 da04 6461 7461  ictcomp>)...data
+00001710: 2901 720c 0000 0029 0372 4900 0000 7251  ).r....).rI...rQ
+00001720: 0000 00da 0c6e 6f64 6573 5f61 7373 6967  .....nodes_assig
+00001730: 6e72 2400 0000 7224 0000 0072 2500 0000  nr$...r$...r%...
+00001740: da0c 756e 6e61 6d65 645f 6469 6374 ae00  ..unnamed_dict..
+00001750: 0000 730c 0000 0006 0102 0206 fe02 050c  ..s.............
+00001760: 0106 ff7a 1c46 6f61 6d54 7261 6e73 666f  ...z.FoamTransfo
+00001770: 726d 6572 2e75 6e6e 616d 6564 5f64 6963  rmer.unnamed_dic
+00001780: 7463 0200 0000 0000 0000 0000 0000 0800  tc..............
+00001790: 0000 0700 0000 4300 0000 73f2 0000 0074  ......C...s....t
+000017a0: 007c 0183 017d 0164 007d 0274 017c 0183  .|...}.d.}.t.|..
+000017b0: 0164 016b 0272 1a7c 01a0 0264 02a1 017d  .d.k.r.|...d...}
+000017c0: 0374 037c 0374 0469 007c 0364 038d 0283  .t.|.t.i.|.d....
+000017d0: 0253 0067 007d 047c 0144 005d 137d 0574  .S.g.}.|.D.].}.t
+000017e0: 057c 0574 0683 0272 317c 05a0 0764 04a1  .|.t...r1|...d..
+000017f0: 0172 317c 01a0 0264 01a1 017d 0201 006e  .r1|...d...}...n
+00001800: 0171 1e74 057c 0164 0219 0074 0883 0272  .q.t.|.d...t...r
+00001810: 4664 0564 06a0 097c 01a0 0264 02a1 01a1  Fd.d...|...d....
+00001820: 0117 0064 0717 007d 036e 057c 01a0 0264  ...d...}.n.|...d
+00001830: 02a1 017d 037c 0472 567c 0364 0664 06a0  ...}.|.rV|.d.d..
+00001840: 097c 04a1 0117 0037 007d 0364 0864 0984  .|.....7.}.d.d..
+00001850: 007c 0144 0083 017d 067c 0264 0075 0172  .|.D...}.|.d.u.r
+00001860: 687c 0264 0a6b 0272 6874 0a7d 076e 0274  h|.d.k.rht.}.n.t
+00001870: 047d 0774 037c 037c 0764 0b64 0c84 007c  .}.t.|.|.d.d...|
+00001880: 0644 0083 017c 037c 0264 0d8d 0383 0253  .D...|.|.d.....S
+00001890: 0029 0e4e 7208 0000 0072 0100 0000 2902  .).Nr....r....).
+000018a0: 727d 0000 0072 1a00 0000 fa01 23fa 0128  r}...r......#..(
+000018b0: 7271 0000 00fa 0129 6301 0000 0000 0000  rq.....)c.......
+000018c0: 0000 0000 0002 0000 0005 0000 0053 0000  .............S..
+000018d0: 0072 7a00 0000 7266 0000 0072 7b00 0000  .rz...rf...r{...
+000018e0: 7267 0000 0072 2400 0000 7224 0000 0072  rg...r$...r$...r
+000018f0: 2500 0000 7240 0000 00cd 0000 0072 5b00  %...r@.......r[.
+00001900: 0000 7a33 466f 616d 5472 616e 7366 6f72  ..z3FoamTransfor
+00001910: 6d65 722e 6469 6374 5f61 7373 6967 6e6d  mer.dict_assignm
+00001920: 656e 742e 3c6c 6f63 616c 733e 2e3c 6c69  ent.<locals>.<li
+00001930: 7374 636f 6d70 3e7a 0b23 636f 6465 5374  stcomp>z.#codeSt
+00001940: 7265 616d 6301 0000 0000 0000 0000 0000  reamc...........
+00001950: 0002 0000 0004 0000 0053 0000 0072 6500  .........S...re.
+00001960: 0000 7224 0000 0072 6600 0000 7267 0000  ..r$...rf...rg..
+00001970: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
+00001980: 7269 0000 00db 0000 0072 6a00 0000 7a33  ri.......rj...z3
+00001990: 466f 616d 5472 616e 7366 6f72 6d65 722e  FoamTransformer.
+000019a0: 6469 6374 5f61 7373 6967 6e6d 656e 742e  dict_assignment.
+000019b0: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
+000019c0: 6d70 3e29 0372 7d00 0000 721a 0000 0072  mp>).r}...r....r
+000019d0: 6200 0000 290b 7243 0000 0072 6000 0000  b...).rC...r`...
+000019e0: 7274 0000 0072 0900 0000 720c 0000 0072  rt...r....r....r
+000019f0: 2c00 0000 7221 0000 00da 0a73 7461 7274  ,...r!.....start
+00001a00: 7377 6974 6872 6300 0000 722f 0000 0072  swithrc...r/...r
+00001a10: 0b00 0000 2908 7249 0000 0072 5100 0000  ....).rI...rQ...
+00001a20: 7262 0000 0072 1a00 0000 5a09 6e6f 6465  rb...r....Z.node
+00001a30: 735f 7374 7272 6800 0000 727e 0000 00da  s_strrh...r~....
+00001a40: 0363 6c73 7224 0000 0072 2400 0000 7225  .clsr$...r$...r%
+00001a50: 0000 00da 0f64 6963 745f 6173 7369 676e  .....dict_assign
+00001a60: 6d65 6e74 b800 0000 733c 0000 0008 0104  ment....s<......
+00001a70: 010c 020a 0112 0104 0208 0114 010a 0204  ................
+00001a80: 0102 800e 011a 010a 0204 0112 0106 0202  ................
+00001a90: 0206 fe10 0606 0104 0202 0202 0102 010c  ................
+00001aa0: 0102 0102 0104 fd04 fe7a 1f46 6f61 6d54  .........z.FoamT
+00001ab0: 7261 6e73 666f 726d 6572 2e64 6963 745f  ransformer.dict_
+00001ac0: 6173 7369 676e 6d65 6e74 6302 0000 0000  assignmentc.....
+00001ad0: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+00001ae0: 0000 0073 2e00 0000 7400 7c01 8301 7d01  ...s....t.|...}.
+00001af0: 7401 7c01 8301 6401 6b03 720e 7402 7c01  t.|...d.k.r.t.|.
+00001b00: 8301 8201 6400 7d02 7403 7c02 7c01 6402  ....d.}.t.|.|.d.
+00001b10: 1900 8302 5300 725f 0000 0029 0472 4300  ....S.r_...).rC.
+00001b20: 0000 7260 0000 00da 134e 6f74 496d 706c  ..r`.....NotImpl
+00001b30: 656d 656e 7465 6445 7272 6f72 7209 0000  ementedErrorr...
+00001b40: 00a9 0372 4900 0000 7251 0000 0072 1a00  ...rI...rQ...r..
+00001b50: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
+00001b60: 00da 0d69 736f 6c61 7465 645f 6c69 7374  ...isolated_list
+00001b70: e100 0000 730a 0000 0008 010c 0108 0104  ....s...........
+00001b80: 010e 017a 1d46 6f61 6d54 7261 6e73 666f  ...z.FoamTransfo
+00001b90: 726d 6572 2e69 736f 6c61 7465 645f 6c69  rmer.isolated_li
+00001ba0: 7374 6302 0000 0000 0000 0000 0000 0008  stc.............
+00001bb0: 0000 0006 0000 0043 0000 0073 ac00 0000  .......C...s....
+00001bc0: 7400 7c01 8301 7d01 6400 7d02 7401 7c01  t.|...}.d.}.t.|.
+00001bd0: 8301 4400 5d18 5c02 7d03 7d04 7402 7c04  ..D.].\.}.}.t.|.
+00001be0: 7403 8302 7222 7c04 6a04 6401 6b02 7222  t...r"|.j.d.k.r"
+00001bf0: 7405 7c04 8301 6402 6403 8502 1900 7d02  t.|...d.d.....}.
+00001c00: 0100 6e01 710a 7c02 6400 7501 722c 7c01  ..n.q.|.d.u.r,|.
+00001c10: a006 7c03 a101 0100 6400 7d05 7407 7c01  ..|.....d.}.t.|.
+00001c20: 8301 6404 6b04 7240 7402 7c01 6403 1900  ..d.k.r@t.|.d...
+00001c30: 7408 8302 7240 7c01 a006 6403 a101 7d05  t...r@|...d...}.
+00001c40: 7c01 a006 6405 a101 7d06 6400 7d07 7c01  |...d...}.d.}.|.
+00001c50: 724e 6406 a009 7c01 a101 7d07 740a 7c06  rNd...|...}.t.|.
+00001c60: 7c07 7c02 7c05 6407 8d04 5300 2908 4e5a  |.|.|.d...S.).NZ
+00001c70: 094c 4953 545f 5459 5045 e905 0000 0072  .LIST_TYPE.....r
+00001c80: 7200 0000 7208 0000 0072 0100 0000 7271  r...r....r....rq
+00001c90: 0000 0029 0472 1a00 0000 721b 0000 0072  ...).r....r....r
+00001ca0: 1c00 0000 721d 0000 0029 0b72 4300 0000  ....r....).rC...
+00001cb0: da09 656e 756d 6572 6174 6572 2c00 0000  ..enumerater,...
+00001cc0: 7205 0000 0072 5a00 0000 7221 0000 0072  r....rZ...r!...r
+00001cd0: 7400 0000 7260 0000 0072 2300 0000 722f  t...r`...r#...r/
+00001ce0: 0000 0072 1900 0000 2908 7249 0000 0072  ...r....).rI...r
+00001cf0: 5100 0000 721c 0000 00da 0569 6e6f 6465  Q...r......inode
+00001d00: 7268 0000 0072 1d00 0000 721a 0000 0072  rh...r....r....r
+00001d10: 1b00 0000 7224 0000 0072 2400 0000 7225  ....r$...r$...r%
+00001d20: 0000 00da 096c 6973 745f 696e 666f e800  .....list_info..
+00001d30: 0000 7322 0000 0008 0104 0210 0114 0110  ..s"............
+00001d40: 0104 0102 8008 010a 0104 021a 010a 010a  ................
+00001d50: 0204 0204 010a 0110 027a 1946 6f61 6d54  .........z.FoamT
+00001d60: 7261 6e73 666f 726d 6572 2e6c 6973 745f  ransformer.list_
+00001d70: 696e 666f 6302 0000 0000 0000 0000 0000  infoc...........
+00001d80: 0006 0000 0004 0000 0043 0000 0073 aa00  .........C...s..
+00001d90: 0000 7400 7c01 8301 7d01 7c01 5c02 7d02  ..t.|...}.|.\.}.
+00001da0: 7d03 7401 7c02 7402 8302 730f 4a00 8201  }.t.|.t...s.J...
+00001db0: 7c02 6a03 7d04 7c04 7d05 7c02 6a04 6400  |.j.}.|.}.|.j.d.
+00001dc0: 7501 7220 7c05 6401 7c02 6a04 1700 3700  u.r |.d.|.j...7.
+00001dd0: 7d05 7c02 6a05 6400 7501 722e 7c05 6402  }.|.j.d.u.r.|.d.
+00001de0: 7c02 6a05 9b00 6403 9d03 3700 7d05 7c02  |.j...d...7.}.|.
+00001df0: 6a06 6400 7501 723b 7c05 6404 7c02 6a06  j.d.u.r;|.d.|.j.
+00001e00: 9b00 9d02 3700 7d05 7401 7c04 7407 8302  ....7.}.t.|.t...
+00001e10: 7244 7408 7c04 8301 7d04 7401 7c05 7407  rDt.|...}.t.|.t.
+00001e20: 8302 724d 7408 7c05 8301 7d05 7c05 7c03  ..rMt.|...}.|.|.
+00001e30: 5f09 740a 7c04 7c03 8302 5300 2905 4e72  _.t.|.|...S.).Nr
+00001e40: 7100 0000 7a06 0a4c 6973 743c da01 3e72  q...z..List<..>r
+00001e50: 2600 0000 290b 7243 0000 0072 2c00 0000  &...).rC...r,...
+00001e60: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
+00001e70: 1c00 0000 721d 0000 0072 2300 0000 7221  ....r....r#...r!
+00001e80: 0000 0072 7700 0000 7209 0000 0029 0672  ...rw...r....).r
+00001e90: 4900 0000 7251 0000 0072 8c00 0000 da08  I...rQ...r......
+00001ea0: 7468 655f 6c69 7374 721a 0000 005a 0d6e  the_listr....Z.n
+00001eb0: 616d 655f 696e 7465 726e 616c 7224 0000  ame_internalr$..
+00001ec0: 0072 2400 0000 7225 0000 00da 0f6c 6973  .r$...r%.....lis
+00001ed0: 745f 6173 7369 676e 6d65 6e74 ff00 0000  t_assignment....
+00001ee0: 7322 0000 0008 0108 020e 0106 0204 010a  s"..............
+00001ef0: 020e 010a 0212 010a 0210 010a 0208 010a  ................
+00001f00: 0108 0106 020a 017a 1f46 6f61 6d54 7261  .......z.FoamTra
+00001f10: 6e73 666f 726d 6572 2e6c 6973 745f 6173  nsformer.list_as
+00001f20: 7369 676e 6d65 6e74 6302 0000 0000 0000  signmentc.......
+00001f30: 0000 0000 0003 0000 0003 0000 0043 0000  .............C..
+00001f40: 0073 3600 0000 6401 6402 8400 7c01 4400  .s6...d.d...|.D.
+00001f50: 8301 7d01 7400 7c01 8301 6403 6b03 7211  ..}.t.|...d.k.r.
+00001f60: 7401 7c01 8301 8201 7c01 a002 6404 a101  t.|.....|...d...
+00001f70: 7d02 7403 7c02 6405 8302 5300 2906 4e63  }.t.|.d...S.).Nc
+00001f80: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001f90: 0400 0000 5300 0000 723d 0000 0072 2700  ....S...r=...r'.
+00001fa0: 0000 7224 0000 0072 6700 0000 7224 0000  ..r$...rg...r$..
+00001fb0: 0072 2400 0000 7225 0000 0072 4000 0000  .r$...r%...r@...
+00001fc0: 1a01 0000 7241 0000 007a 3446 6f61 6d54  ....rA...z4FoamT
+00001fd0: 7261 6e73 666f 726d 6572 2e6d 6163 726f  ransformer.macro
+00001fe0: 5f61 7373 6967 6e6d 656e 742e 3c6c 6f63  _assignment.<loc
+00001ff0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
+00002000: 0800 0000 7201 0000 00da 0029 0472 6000  ....r......).r`.
+00002010: 0000 7286 0000 0072 7400 0000 7209 0000  ..r....rt...r...
+00002020: 0072 8700 0000 7224 0000 0072 2400 0000  .r....r$...r$...
+00002030: 7225 0000 00da 106d 6163 726f 5f61 7373  r%.....macro_ass
+00002040: 6967 6e6d 656e 7419 0100 0073 0a00 0000  ignment....s....
+00002050: 0e01 0c01 0801 0a01 0a01 7a20 466f 616d  ..........z Foam
+00002060: 5472 616e 7366 6f72 6d65 722e 6d61 6372  Transformer.macr
+00002070: 6f5f 6173 7369 676e 6d65 6e74 6302 0000  o_assignmentc...
+00002080: 0000 0000 0000 0000 0003 0000 0003 0000  ................
+00002090: 0043 0000 0073 4e00 0000 6401 6402 8400  .C...sN...d.d...
+000020a0: 7c01 4400 8301 7d01 7400 7c01 8301 6403  |.D...}.t.|...d.
+000020b0: 6b03 7211 7401 7c01 8301 8201 7c01 6404  k.r.t.|.....|.d.
+000020c0: 1900 7d02 7402 7c02 6405 8302 721e 7c02  ..}.t.|.d...r.|.
+000020d0: a003 a100 7d02 7c01 6406 1900 9b00 6407  ....}.|.d.....d.
+000020e0: 7c02 9b00 9d03 5300 2908 4e63 0100 0000  |.....S.).Nc....
+000020f0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00002100: 5300 0000 723d 0000 0072 2700 0000 7224  S...r=...r'...r$
+00002110: 0000 0072 6700 0000 7224 0000 0072 2400  ...rg...r$...r$.
+00002120: 0000 7225 0000 0072 4000 0000 2101 0000  ..r%...r@...!...
+00002130: 7241 0000 007a 3046 6f61 6d54 7261 6e73  rA...z0FoamTrans
+00002140: 666f 726d 6572 2e65 7175 616c 5f61 7373  former.equal_ass
+00002150: 6967 6e2e 3c6c 6f63 616c 733e 2e3c 6c69  ign.<locals>.<li
+00002160: 7374 636f 6d70 3ee9 0200 0000 7208 0000  stcomp>.....r...
+00002170: 0072 3b00 0000 7201 0000 00da 013d 2904  .r;...r......=).
+00002180: 7260 0000 0072 6100 0000 727c 0000 0072  r`...ra...r|...r
+00002190: 3b00 0000 2903 7249 0000 0072 5100 0000  ;...).rI...rQ...
+000021a0: 7214 0000 0072 2400 0000 7224 0000 0072  r....r$...r$...r
+000021b0: 2500 0000 da0c 6571 7561 6c5f 6173 7369  %.....equal_assi
+000021c0: 676e 2001 0000 730e 0000 000e 010c 0108  gn ...s.........
+000021d0: 0108 010a 0108 0112 017a 1c46 6f61 6d54  .........z.FoamT
+000021e0: 7261 6e73 666f 726d 6572 2e65 7175 616c  ransformer.equal
+000021f0: 5f61 7373 6967 6e63 0200 0000 0000 0000  _assignc........
+00002200: 0000 0000 0700 0000 0500 0000 4300 0000  ............C...
+00002210: 736e 0000 0064 0164 0284 007c 0144 0083  sn...d.d...|.D..
+00002220: 017d 0174 007c 0183 0164 036b 0272 127c  .}.t.|...d.k.r.|
+00002230: 015c 027d 027d 036e 177c 01a0 0164 04a1  .\.}.}.n.|...d..
+00002240: 017d 027c 01a0 0164 04a1 017d 0464 05a0  .}.|...d...}.d..
+00002250: 027c 01a1 017d 057c 0464 067c 059b 0064  .|...}.|.d.|...d
+00002260: 079d 0317 007d 037c 0264 0817 007c 0317  .....}.|.d...|..
+00002270: 007d 0674 037c 0674 047c 027c 0383 0283  .}.t.|.t.|.|....
+00002280: 0253 0029 094e 6301 0000 0000 0000 0000  .S.).Nc.........
+00002290: 0000 0002 0000 0004 0000 0053 0000 0072  ...........S...r
+000022a0: 3d00 0000 7227 0000 0072 2400 0000 7267  =...r'...r$...rg
+000022b0: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
+000022c0: 0000 7240 0000 002a 0100 0072 4100 0000  ..r@...*...rA...
+000022d0: 7a38 466f 616d 5472 616e 7366 6f72 6d65  z8FoamTransforme
+000022e0: 722e 6469 7265 6374 6976 655f 6173 7369  r.directive_assi
+000022f0: 676e 6d65 6e74 2e3c 6c6f 6361 6c73 3e2e  gnment.<locals>.
+00002300: 3c6c 6973 7463 6f6d 703e 7292 0000 0072  <listcomp>r....r
+00002310: 0100 0000 7a02 2c20 7281 0000 0072 8200  ....z., r....r..
+00002320: 0000 7271 0000 0029 0572 6000 0000 7274  ..rq...).r`...rt
+00002330: 0000 0072 2f00 0000 7209 0000 0072 0e00  ...r/...r....r..
+00002340: 0000 2907 7249 0000 0072 5100 0000 7262  ..).rI...rQ...rb
+00002350: 0000 00da 0763 6f6e 7465 6e74 da0d 6675  .....content..fu
+00002360: 6e63 7469 6f6e 5f6e 616d 65da 0961 7267  nction_name..arg
+00002370: 756d 656e 7473 da03 6b65 7972 2400 0000  uments..keyr$...
+00002380: 7224 0000 0072 2500 0000 da14 6469 7265  r$...r%.....dire
+00002390: 6374 6976 655f 6173 7369 676e 6d65 6e74  ctive_assignment
+000023a0: 2901 0000 7312 0000 000e 010c 010a 010a  )...s...........
+000023b0: 020a 010a 0110 010c 0110 017a 2446 6f61  ...........z$Foa
+000023c0: 6d54 7261 6e73 666f 726d 6572 2e64 6972  mTransformer.dir
+000023d0: 6563 7469 7665 5f61 7373 6967 6e6d 656e  ective_assignmen
+000023e0: 7463 0200 0000 0000 0000 0000 0000 0500  tc..............
+000023f0: 0000 0700 0000 4300 0000 73ac 0000 0074  ......C...s....t
+00002400: 007c 0183 017d 0164 007d 0274 017c 0183  .|...}.d.}.t.|..
+00002410: 0164 016b 0272 117c 015c 027d 037d 046e  .d.k.r.|.\.}.}.n
+00002420: 1974 017c 0183 0164 026b 0272 267c 015c  .t.|...d.k.r&|.\
+00002430: 037d 037d 027d 047c 02a0 0264 03a1 0173  .}.}.}.|...d...s
+00002440: 2574 037c 0183 0182 016e 0474 037c 0183  %t.|.....n.t.|..
+00002450: 0182 0174 047c 0483 017d 047c 04a0 0264  ...t.|...}.|...d
+00002460: 04a1 0172 447c 04a0 0564 0564 06a1 0264  ...rD|...d.d...d
+00002470: 0719 007d 047c 04a0 0664 0564 06a1 0264  ...}.|...d.d...d
+00002480: 0819 007d 046e 087c 0464 0164 0985 0219  ...}.n.|.d.d....
+00002490: 00a0 07a1 007d 0474 087c 0374 097c 037c  .....}.t.|.t.|.|
+000024a0: 047c 0264 0a8d 0383 0253 0029 0b4e 7292  .|.d.....S.).Nr.
+000024b0: 0000 00e9 0300 0000 7280 0000 007a 0323  ........r....z.#
+000024c0: 7b0a 7226 0000 0072 0800 0000 7272 0000  {.r&...r....rr..
+000024d0: 0072 0100 0000 e9fd ffff ff29 0172 6200  .r.........).rb.
+000024e0: 0000 290a 7243 0000 0072 6000 0000 7283  ..).rC...r`...r.
+000024f0: 0000 0072 8600 0000 7221 0000 0072 3000  ...r....r!...r0.
+00002500: 0000 da06 7273 706c 6974 da05 7374 7269  ....rsplit..stri
+00002510: 7072 0900 0000 720a 0000 0029 0572 4900  pr....r....).rI.
+00002520: 0000 7251 0000 0072 6200 0000 721a 0000  ..rQ...rb...r...
+00002530: 00da 0463 6f64 6572 2400 0000 7224 0000  ...coder$...r$..
+00002540: 0072 2500 0000 da0f 636f 6465 5f61 7373  .r%.....code_ass
+00002550: 6967 6e6d 656e 7435 0100 0073 2000 0000  ignment5...s ...
+00002560: 0801 0401 0c01 0a01 0c01 0a01 0a01 0801  ................
+00002570: 02ff 0803 0801 0a01 1001 1201 1002 1401  ................
+00002580: 7a1f 466f 616d 5472 616e 7366 6f72 6d65  z.FoamTransforme
+00002590: 722e 636f 6465 5f61 7373 6967 6e6d 656e  r.code_assignmen
+000025a0: 7463 0200 0000 0000 0000 0000 0000 0200  tc..............
+000025b0: 0000 0300 0000 4300 0000 731a 0000 0074  ......C...s....t
+000025c0: 007c 0183 017d 0174 017c 0164 0119 006a  .|...}.t.|.d...j
+000025d0: 0264 0217 0083 0153 0029 034e 7201 0000  .d.....S.).Nr...
+000025e0: 0072 2600 0000 2903 7243 0000 0072 1100  .r&...).rC...r..
+000025f0: 0000 7214 0000 0072 4800 0000 7224 0000  ..r....rH...r$..
+00002600: 0072 2400 0000 7225 0000 00da 1273 7065  .r$...r%.....spe
+00002610: 6369 616c 5f64 6972 6563 7469 7665 7348  cial_directivesH
+00002620: 0100 0073 0400 0000 0801 1201 7a22 466f  ...s........z"Fo
+00002630: 616d 5472 616e 7366 6f72 6d65 722e 7370  amTransformer.sp
+00002640: 6563 6961 6c5f 6469 7265 6374 6976 6573  ecial_directives
+00002650: 4e29 1a72 1e00 0000 721f 0000 0072 2000  N).r....r....r .
+00002660: 0000 724b 0000 0072 4e00 0000 7252 0000  ..rK...rN...rR..
+00002670: 0072 5300 0000 7254 0000 0072 5500 0000  .rS...rT...rU...
+00002680: 7256 0000 0072 5700 0000 725d 0000 0072  rV...rW...r]...r
+00002690: 6200 0000 7263 0000 0072 6c00 0000 7279  b...rc...rl...ry
+000026a0: 0000 0072 7f00 0000 7285 0000 0072 8800  ...r....r....r..
+000026b0: 0000 728c 0000 0072 8f00 0000 7291 0000  ..r....r....r...
+000026c0: 0072 9400 0000 7299 0000 0072 9f00 0000  .r....r....r....
+000026d0: 72a0 0000 0072 2400 0000 7224 0000 0072  r....r$...r$...r
+000026e0: 2400 0000 7225 0000 0072 3600 0000 4d00  $...r%...r6...M.
+000026f0: 0000 7330 0000 0008 0008 0108 0308 0308  ..s0............
+00002700: 0308 0308 0308 0308 0308 0308 0908 0508  ................
+00002710: 0a08 0908 2708 0a08 2908 0708 1708 1a08  ....'...).......
+00002720: 0708 0908 0c0c 1372 3600 0000 7227 0000  .......r6...r'..
+00002730: 0029 27da 075f 5f64 6f63 5f5f da0b 6461  .)'..__doc__..da
+00002740: 7461 636c 6173 7365 7372 0200 0000 da07  taclassesr......
+00002750: 7061 7468 6c69 6272 0300 0000 5a04 6c61  pathlibr....Z.la
+00002760: 726b 7204 0000 0072 0500 0000 7206 0000  rkr....r....r...
+00002770: 005a 0f6c 6172 6b2e 6578 6365 7074 696f  .Z.lark.exceptio
+00002780: 6e73 7207 0000 00da 0361 7374 7209 0000  nsr......astr...
+00002790: 0072 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
+000027a0: 720d 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
+000027b0: 1000 0000 7211 0000 0072 1200 0000 7213  ....r....r....r.
+000027c0: 0000 00da 085f 5f66 696c 655f 5fda 0861  .....__file__..a
+000027d0: 6273 6f6c 7574 65da 0670 6172 656e 74da  bsolute..parent.
+000027e0: 0468 6572 65da 0972 6561 645f 7465 7874  .here..read_text
+000027f0: 7239 0000 005a 1067 7261 6d6d 6172 5f61  r9...Z.grammar_a
+00002800: 6476 616e 6365 6472 3200 0000 7234 0000  dvancedr2...r4..
+00002810: 0072 3500 0000 7219 0000 0072 3300 0000  .r5...r....r3...
+00002820: 723b 0000 0072 4300 0000 7247 0000 0072  r;...rC...rG...r
+00002830: 3600 0000 7224 0000 0072 2400 0000 7224  6...r$...r$...r$
+00002840: 0000 0072 2500 0000 da08 3c6d 6f64 756c  ...r%.....<modul
+00002850: 653e 0100 0000 7326 0000 0004 000c 020c  e>....s&........
+00002860: 0114 020c 0134 020e 0e0c 020c 010e 020e  .....4..........
+00002870: 010a 0202 0310 010a 0708 1308 0408 0414  ................
+00002880: 08                                       .
```

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/polymesh.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/polymesh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/__pycache__/util.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/__pycache__/util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/ast.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,28 +248,34 @@
 class Assignment:
     name: str
     value: object
 
     def dump(self, indent=0):
         if hasattr(self.value, "dump"):
             return self.value.dump(indent)
+        if hasattr(self.value, "dump_without_assignment"):
+            value = self.value.dump_without_assignment()
         else:
-            return indent * " " + f"{self.name}  {self.value};"
+            value = self.value
+        return indent * " " + f"{self.name}  {value};"
 
 
 class VariableAssignment(Assignment):
     def __repr__(self):
         s = super().__repr__()
         return s
 
     def dump(self, indent=0):
         if hasattr(self.value, "dump"):
             return indent * " " + f"{self.name}  {self.value.dump(indent)};"
+        if hasattr(self.value, "dump_without_assignment"):
+            value = self.value.dump_without_assignment()
         else:
-            return indent * " " + f"{self.name}  {self.value};"
+            value = self.value
+        return indent * " " + f"{self.name}  {value};"
 
 
 @dataclass
 class Value(Node):
     def __init__(self, value, name=None, dimension=None):
         self.value = value
         self.name = name
@@ -335,18 +341,21 @@
     def __repr__(self):
         return super().__repr__()
 
     def dump(self, indent=0):
         tmp = []
         indentation = indent * " "
         if self._name is not None:
-            line = indentation + self._name
+            star = indentation + self._name
             if self._directive is not None:
-                line += "  " + self._directive
-            tmp.append(line + f"\n{indentation}" + "{")
+                star += "  " + self._directive
+            star += "\n"
+        else:
+            star = ""
+        tmp.append(star + indentation + "{")
 
         num_spaces = _compute_spaces_to_align(self)
         for key, node in self.items():
             if self.comments is not None and key in self.comments:
                 comment = self.comments[key]
                 if isinstance(comment, str):
                     tmp.append("    // " + comment.replace("\n", "\n    // "))
@@ -384,23 +393,14 @@
         self._name = name
         self._dtype = dtype
         super().__init__(iterable)
 
     def get_name(self):
         return self._name
 
-    def add_name(self, name):
-        if self._name is None:
-            self._name = name
-        elif isinstance(self._name, str):
-            if self._name != name:
-                self._name = name + " " + self._name
-        else:
-            raise RuntimeError()
-
     def __repr__(self):
         return super().__repr__()
 
     def _make_list_strings(self, indent):
         return [self._dump_item(item, indent) for item in self]
 
     def _dump_item(self, item, indent=0):
```

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/LICENSE` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/blockmesh/LICENSE`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/__init__.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/blockmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/__init__.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/edges.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/edges.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/grading.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/blockmesh/__pycache__/grading.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/edges.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/blockmesh/edges.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/blockmesh/grading.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/blockmesh/grading.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/constant_files.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/constant_files.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/control_dict.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/control_dict.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/format.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/format.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,19 @@
 
 class FoamFormatError(RuntimeError):
     pass
 
 
 def format_code(code, as_field=False, check=True):
     if not as_field:
-        tree = parse(code)
+        try:
+            tree = parse(code)
+        except lark.exceptions.LarkError:
+            raise FoamFormatError(f"LarkError while formatting code\n{code}")
+
         result = dump(tree)
         if check:
             try:
                 tree1 = parse(result)
             except lark.exceptions.LarkError:
                 raise FoamFormatError(f"LarkError while formatting code\n{code}")
             else:
```

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/fv_options.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/fv_options.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/fv_schemes.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/fv_schemes.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/generators.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,17 @@
         if params is None:
             params = self.output.sim.params
 
         code = self.generate_code(params)
         if code is False:
             return
 
-        with open(self.output.path_run / self.rel_path, "w") as file:
-            file.write(code)
+        path = self.output.path_run / self.rel_path
+        path.parent.mkdir(exist_ok=True)
+        path.write_text(code)
 
     @abstractmethod
     def generate_code(self):
         """Generate the code of the file"""
 
     def read(self):
         path = self.output.path_run / self.rel_path
@@ -67,16 +68,15 @@
             tree = parse(path.read_text())
             tree.path = path
             return tree
         else:
             return read_field_file(path)
 
     def overwrite(self, dumpable):
-        with open(self.output.path_run / self.rel_path, "w") as file:
-            file.write(dumpable.dump())
+        (self.output.path_run / self.rel_path).write_text(dumpable.dump())
 
 
 class FileGenerator(FileGeneratorABC):
     template_name: str
 
     def __init__(self, output):
         super().__init__(output)
@@ -155,17 +155,18 @@
 
         if complete_params is not None:
             complete_params(params)
 
 
 def new_file_generator_class(file_name, dir_name="0"):
     cls_name = f"FileGenerator{camelize(file_name)}"
+    relative_path = f"{dir_name}/{file_name}"
     return type(
         cls_name,
         (FileGenerator,),
         {
             "dir_name": dir_name,
-            "rel_path": f"{dir_name}/{file_name}",
-            "template_name": f"{file_name}.jinja",
-            "_name": underscore(file_name.replace(".", "_")),
+            "rel_path": relative_path,
+            "template_name": f"{relative_path}.jinja",
+            "_name": underscore(file_name.replace(".", "_").replace("/", "_")),
         },
     )
```

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/grammar.lark` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/grammar.lark`

 * *Files 4% similar despite different names*

```diff
@@ -10,32 +10,31 @@
 _var_name : CNAME|ESCAPED_STRING|DOUBLE_NAME|EQKEY
 
 LIST_TYPE.2 : /List<[\w]+>/
 list_info : _list_name [CNAME] [NEWLINE LIST_TYPE] [NEWLINE SIGNED_NUMBER]
 
 directive: /#[a-zA-Z]+/ | /#[a-zA-Z]+{[^}]*}/
 dimension_set : "[" (SIGNED_NUMBER)+ "]"
-_dataentry : DOUBLE_NAME | CNAME | list | ESCAPED_STRING | MACRO | directive
+_dataentry : DOUBLE_NAME | CNAME | ESCAPED_STRING | MACRO | directive
     | SIGNED_NUMBER | dimension_set | EQKEY
 
-list : "(" (_dataentry|NEWLINE|dict_assignment)* ")"
+list : "(" (_dataentry|list|NEWLINE|dict_assignment)* ")"
 
 equal_assign: CNAME "=" (CNAME|SIGNED_NUMBER|list) | CNAME "=" NEWLINE list
 _in_funtion_call : CNAME|DOUBLE_NAME|equal_assign|_funtion_call
 _funtion_call : CNAME [NEWLINE] "(" [NEWLINE] (_in_funtion_call) ( "," [NEWLINE] (_in_funtion_call))* [NEWLINE] ")"
 
 directive_assignment: [NEWLINE] directive (_funtion_call|CNAME|EQKEY|ESCAPED_STRING) [";"] NEWLINE
 macro_assignment : [NEWLINE] MACRO ";" NEWLINE
-list_assignment : [NEWLINE] list_info NEWLINE list ";" NEWLINE
+list_assignment : [NEWLINE] list_info NEWLINE? list ";" NEWLINE
 var_assignment : [NEWLINE] _var_name [(_dataentry)+] ";" NEWLINE
 dict_assignment : [NEWLINE] _dict_name NEWLINE "{" [NEWLINE] [(_assignment)+] "}" [";"] NEWLINE
 code_assignment : [NEWLINE] CNAME NEWLINE /#{[\S\s]*?#};/ NEWLINE
-dimension_assignment : [NEWLINE] CNAME [CNAME] dimension_set _dataentry ";" NEWLINE
 _assignment : var_assignment | dict_assignment | list_assignment
-              | dimension_assignment | code_assignment | macro_assignment | directive_assignment
+              | code_assignment | macro_assignment | directive_assignment
 
 file : (_assignment)+
 
 CPP_COMMENT: /\/\/[^\n]*/ NEWLINE
 C_COMMENT: "/*" /(.|\n)*?/ "*/" NEWLINE
 
 %ignore /[\n\f\r]+/
```

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/grammar_advanced.lark` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/grammar_advanced.lark`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 EQKEY.2 : /[a-zA-Z]+\(\S+\)[a-zA-Z]*/
 
 MACRO : /[\-]?\$[^;^\s\n\)]+/ | /\$\{{[^;^\n]+/
 DOUBLE_NAME.1 : /[a-zA-Z][a-zA-Z\d]*[:\.-][:]?[a-zA-Z\d\._]+/
 TRIPLE_NAME.3 :  /[a-zA-Z][a-zA-Z\d]*[:\-][a-zA-Z\d\._]+[:\-][a-zA-Z\d\._]/
 
 _list_name: CNAME|ESCAPED_STRING|DOUBLE_NAME|MACRO|SIGNED_NUMBER|EQKEY|directive
-_dict_name: CNAME|ESCAPED_STRING|DOUBLE_NAME|EQKEY|TRIPLE_NAME|list
+_dict_name: CNAME|ESCAPED_STRING|DOUBLE_NAME|EQKEY|TRIPLE_NAME
 _var_name : CNAME|ESCAPED_STRING|DOUBLE_NAME|MACRO|EQKEY
 
 LIST_TYPE.2 : /List<[\w]+>/
-list_info : _list_name [CNAME] [NEWLINE] [LIST_TYPE] [NEWLINE SIGNED_NUMBER]
+list_info : _list_name CNAME? NEWLINE? LIST_TYPE? [NEWLINE? SIGNED_NUMBER]
 
 directive: /#[a-zA-Z]+/ | /#[a-zA-Z]+{[^}]*}/
 dimension_set : "[" (SIGNED_NUMBER)+ "]"
-_dataentry : DOUBLE_NAME | CNAME | list | ESCAPED_STRING | MACRO | directive
+_dataentry : DOUBLE_NAME | CNAME | ESCAPED_STRING | MACRO | directive
     | SIGNED_NUMBER | dimension_set | EQKEY
-list : "(" (_dataentry|NEWLINE|dict_assignment)* ")"
+list : "(" (_dataentry|NEWLINE|list|dict_assignment|unnamed_dict)* ")"
+unnamed_dict : "{" [NEWLINE] [(_assignment)+] "}"
 
 equal_assign: CNAME "=" (CNAME|SIGNED_NUMBER|list) | CNAME "=" NEWLINE list
 _in_funtion_call : CNAME|DOUBLE_NAME|equal_assign|_funtion_call
 _funtion_call : CNAME [NEWLINE] "(" [NEWLINE] (_in_funtion_call) ( "," [NEWLINE] (_in_funtion_call))* [NEWLINE] ")"
 
 isolated_list : [NEWLINE] list ";" [NEWLINE]
 _isolated_thing : isolated_list
@@ -29,17 +30,16 @@
 directive_assignment: [NEWLINE] directive (_funtion_call|CNAME|EQKEY|ESCAPED_STRING) [";"] [NEWLINE]
 macro_assignment : [NEWLINE] MACRO [";"] [NEWLINE]
 list_assignment : [NEWLINE] list_info [NEWLINE] list [NEWLINE] ";" [NEWLINE]
 var_assignment : [NEWLINE] _var_name [(_dataentry)+] ";" [NEWLINE]
 dict_assignment : [NEWLINE] _dict_name (CNAME)* [directive] [NEWLINE] "{" [NEWLINE] [(_assignment)+] "}" [";"] NEWLINE
 code_assignment : [NEWLINE] CNAME [directive] [NEWLINE] /#{[\S\s]*?#};/ NEWLINE
 special_directives : [NEWLINE] (/#if[\S\s]*#endif/|/#remove[\S\s]+[^;\n{]/) NEWLINE
-dimension_assignment : [NEWLINE] CNAME [CNAME] dimension_set _dataentry ";" [NEWLINE]
 _assignment : var_assignment | dict_assignment | list_assignment
-              | dimension_assignment | code_assignment | macro_assignment | directive_assignment
+              | code_assignment | macro_assignment | directive_assignment
               | special_directives
 
 file : (_assignment | _isolated_thing)+
 
 CPP_COMMENT: /\/\/[^\n]*/ [NEWLINE]
 C_COMMENT: "/*" /(.|\n)*?/ "*/" [NEWLINE]
```

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/parser.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,17 @@
     name: str
     info: str = None
     dtype: str = None
     size: int = None
 
 
 def parse(text, grammar=None):
+    if isinstance(text, bytes):
+        text = text.decode()
+
     text = "\n".join(line.rstrip() for line in text.split("\n"))
     if not text.endswith("\n"):
         text += "\n"
 
     if grammar is None:
         try:
             tree = lark_parser.parse(text)
@@ -123,19 +126,14 @@
     def file(self, nodes):
         first_assignment = nodes[0]
         if first_assignment.name == "FoamFile":
             info_dict = first_assignment.value
             nodes = nodes[1:]
         else:
             info_dict = None
-
-        for node in nodes:
-            if isinstance(node.value, List):
-                node.value.add_name(node.name)
-
         return FoamInputFile(info_dict, {node.name: node.value for node in nodes})
 
     def var_assignment(self, nodes):
         nodes = [node for node in nodes if node is not None]
         dimension_set = None
         name_in_value = None
         name = nodes.pop(0)
@@ -169,14 +167,24 @@
                 value = last_value
             else:
                 value = Value(
                     last_value, name=name_in_value, dimension=dimension_set
                 )
         return VariableAssignment(name, value)
 
+    def unnamed_dict(self, nodes):
+        nodes_assign = [
+            node
+            for node in nodes
+            if hasattr(node, "name") and hasattr(node, "value")
+        ]
+        return Dict(
+            data={node.name: node.value for node in nodes_assign},
+        )
+
     def dict_assignment(self, nodes):
         nodes = filter_no_newlines(nodes)
         directive = None
 
         if len(nodes) == 1:
             name = nodes.pop(0)
             return Assignment(name, Dict(data={}, name=name))
@@ -196,18 +204,14 @@
 
         nodes_assign = [
             node
             for node in nodes
             if hasattr(node, "name") and hasattr(node, "value")
         ]
 
-        for node in nodes_assign:
-            if isinstance(node.value, List):
-                node.value.add_name(node.name)
-
         if directive is not None and directive == "#codeStream":
             cls = CodeStream
         else:
             cls = Dict
 
         return Assignment(
             name,
@@ -270,25 +274,14 @@
             name = str(name)
         if isinstance(name_internal, int):
             name_internal = str(name_internal)
 
         the_list._name = name_internal
         return Assignment(name, the_list)
 
-    def dimension_assignment(self, nodes):
-        nodes = [node for node in nodes if node is not None]
-        name = nodes.pop(0)
-
-        if len(nodes) == 3:
-            return Assignment(name, Value(nodes[-1], nodes[0], nodes[-2]))
-        elif len(nodes) == 2:
-            return Assignment(name, Value(nodes[-1], dimension=nodes[-2]))
-        else:
-            raise RuntimeError(nodes)
-
     def macro_assignment(self, nodes):
         nodes = [node for node in nodes if node is not None]
         if len(nodes) != 1:
             raise NotImplementedError(nodes)
         name = nodes.pop(0)
         return Assignment(name, "")
```

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/polymesh.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/polymesh.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/foam_input_files/util.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/foam_input_files/util.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/info.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/info.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/log.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/log.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/make.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/make.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/operators.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/operators.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/output/__pycache__/__init__.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/output/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/output/__pycache__/base.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/output/__pycache__/base.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun  4 20:13:56 2023 UTC, .py size: 10233 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 84f0 7c64 f927 0000  o.........|d.'..
+00000000: 6f0d 0d0a 0000 0000 7747 9064 4429 0000  o.......wG.dD)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6401 6402 6c04 5a04 6401 6402 6c05  Z.d.d.l.Z.d.d.l.
 00000050: 5a05 6401 6402 6c06 5a06 6401 6403 6c07  Z.d.d.l.Z.d.d.l.
 00000060: 6d08 5a08 0100 6401 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6405 6c0b 6d0c 5a0c 0100 6401  ..d.d.l.m.Z...d.
@@ -28,458 +28,469 @@
 000001b0: 72da 1644 6563 6f6d 706f 7365 5061 7244  r..DecomposeParD
 000001c0: 6963 7448 656c 7065 7229 02da 0a49 6e70  ictHelper)...Inp
 000001d0: 7574 4669 6c65 73da 186e 6577 5f66 696c  utFiles..new_fil
 000001e0: 655f 6765 6e65 7261 746f 725f 636c 6173  e_generator_clas
 000001f0: 7329 01da 066c 6f67 6765 7229 01da 1267  s)...logger)...g
 00000200: 6574 5f73 6f6c 7665 725f 7061 636b 6167  et_solver_packag
 00000210: 6563 0200 0000 0000 0000 0000 0000 0800  ec..............
-00000220: 0000 0900 0000 4300 0000 7338 0100 007c  ......C...s8...|
+00000220: 0000 0900 0000 4300 0000 7346 0100 007c  ......C...sF...|
 00000230: 0064 0075 0072 0664 0053 0074 007c 0074  .d.u.r.d.S.t.|.t
 00000240: 0183 0272 0e7c 0067 017d 007c 0044 005d  ...r.|.g.}.|.D.]
-00000250: 897d 0274 017c 0283 017d 0264 017c 0276  .}.t.|...}.d.|.v
+00000250: 907d 0274 017c 0283 017d 0264 017c 0276  .}.t.|...}.d.|.v
 00000260: 0072 2c7c 02a0 0264 01a1 015c 027d 027d  .r,|...d...\.}.}
 00000270: 037c 017c 03a0 03a1 001b 007d 047c 02a0  .|.|.......}.|..
 00000280: 03a1 007d 026e 027c 017d 047c 02a0 0464  ...}.n.|.}.|...d
 00000290: 02a1 0172 547c 02a0 0564 02a1 017d 027c  ...rT|...d...}.|
 000002a0: 02a0 0264 03a1 015c 027d 057d 037c 03a0  ...d...\.}.}.|..
 000002b0: 0564 04a1 017d 0374 066a 07a0 087c 05a1  .d...}.t.j...|..
 000002c0: 017d 067c 06a0 097c 03a1 017d 0274 066a  .}.|...|...}.t.j
 000002d0: 076a 0a7d 076e 0c74 0b74 0c6a 0da0 0e7c  .j.}.n.t.t.j...|
 000002e0: 02a1 0183 01a0 0fa1 007d 0274 107d 077c  .........}.t.}.|
-000002f0: 077c 0283 018f 2d7d 027c 02a0 11a1 0072  .|....-}.|.....r
-00000300: 7074 12a0 137c 027c 04a1 0201 006e 1a7c  pt...|.|.....n.|
-00000310: 02a0 14a1 0072 7e74 12a0 157c 027c 047c  .....r~t...|.|.|
-00000320: 026a 161b 00a1 0201 006e 0c74 1764 057c  .j.......n.t.d.|
-00000330: 029b 0264 067c 02a0 18a1 009b 029d 0483  ...d.|..........
-00000340: 0182 0157 0064 0004 0004 0083 0301 006e  ...W.d.........n
-00000350: 0831 0073 9477 0101 0001 0001 0059 0001  .1.s.w.......Y..
-00000360: 0071 1064 0053 0029 074e 7a02 2d3e 7a0d  .q.d.S.).Nz.->z.
-00000370: 7061 636b 6167 652d 6461 7461 28fa 0129  package-data(..)
-00000380: fa01 2f7a 0b72 6573 6f75 7263 6520 3d20  ../z.resource = 
-00000390: 7a16 2c20 7265 736f 7572 6365 2e65 7869  z., resource.exi
-000003a0: 7374 7328 2920 3d20 2919 da0a 6973 696e  sts() = )...isin
-000003b0: 7374 616e 6365 da03 7374 72da 0573 706c  stance..str..spl
-000003c0: 6974 da05 7374 7269 70da 0a73 7461 7274  it..strip..start
-000003d0: 7377 6974 68da 0c72 656d 6f76 6570 7265  swith..removepre
-000003e0: 6669 78da 0969 6d70 6f72 746c 6962 da09  fix..importlib..
-000003f0: 7265 736f 7572 6365 73da 0566 696c 6573  resources..files
-00000400: da08 6a6f 696e 7061 7468 5a07 6173 5f66  ..joinpathZ.as_f
-00000410: 696c 6572 0300 0000 da02 6f73 da04 7061  iler......os..pa
-00000420: 7468 da0a 6578 7061 6e64 7661 7273 da0a  th..expandvars..
-00000430: 6578 7061 6e64 7573 6572 7202 0000 00da  expanduserr.....
-00000440: 0769 735f 6669 6c65 da06 7368 7574 696c  .is_file..shutil
-00000450: da04 636f 7079 da06 6973 5f64 6972 da08  ..copy..is_dir..
-00000460: 636f 7079 7472 6565 da04 6e61 6d65 da13  copytree..name..
-00000470: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
-00000480: 726f 72da 0665 7869 7374 7329 0872 1900  ror..exists).r..
-00000490: 0000 da08 7061 7468 5f72 756e da08 7265  ....path_run..re
-000004a0: 736f 7572 6365 da0d 7265 6c61 7469 7665  source..relative
-000004b0: 5f70 6174 68da 0b64 6573 7469 6e61 7469  _path..destinati
-000004c0: 6f6e da0c 7061 636b 6167 655f 6e61 6d65  on..package_name
-000004d0: 5a10 6d75 6c74 6970 6c65 7865 645f 7061  Z.multiplexed_pa
-000004e0: 7468 da0f 636f 6e74 6578 745f 6d61 6e61  th..context_mana
-000004f0: 6765 72a9 0072 2e00 0000 fa3d 2f68 6f6d  ger..r.....=/hom
-00000500: 652f 7069 6572 7265 2f44 6576 2f66 6c75  e/pierre/Dev/flu
-00000510: 6964 7369 6d66 6f61 6d2f 7372 632f 666c  idsimfoam/src/fl
-00000520: 7569 6473 696d 666f 616d 2f6f 7574 7075  uidsimfoam/outpu
-00000530: 742f 6261 7365 2e70 79da 0e63 6f70 795f  t/base.py..copy_
-00000540: 7265 736f 7572 6365 731e 0000 0073 4000  resources....s@.
-00000550: 0000 0801 0401 0a01 0601 0802 0801 0801  ................
-00000560: 0e01 0c01 0a01 0402 0a02 0a01 0e01 0a01  ................
-00000570: 0c01 0a01 0a01 1402 0401 0a02 0801 0e01  ................
-00000580: 0801 1401 0202 1201 04ff 0280 1cfa 0280  ................
-00000590: 04ec 7230 0000 0063 0000 0000 0000 0000  ..r0...c........
-000005a0: 0000 0000 0000 0000 0400 0000 0000 0000  ................
-000005b0: 73b4 0000 0065 005a 0164 005a 0264 0164  s....e.Z.d.Z.d.d
-000005c0: 0267 025a 0364 0364 0467 025a 0467 0064  .g.Z.d.d.g.Z.g.d
-000005d0: 05a2 015a 0565 0664 0464 0664 0769 0183  ...Z.e.d.d.d.i..
-000005e0: 025a 0765 0883 005a 0965 0a83 005a 0b65  .Z.e...Z.e...Z.e
-000005f0: 0c64 0864 0984 0083 015a 0d65 0c64 0a64  .d.d.....Z.e.d.d
-00000600: 0b84 0083 015a 0e65 0c64 0c64 0d84 0083  .....Z.e.d.d....
-00000610: 015a 0f65 0c64 0e64 0f84 0083 015a 1064  .Z.e.d.d.....Z.d
-00000620: 1d87 0066 0164 1164 1284 095a 1165 0c64  ...f.d.d...Z.e.d
-00000630: 1364 1484 0083 015a 1287 0066 0164 1564  .d.....Z...f.d.d
-00000640: 1684 085a 1364 1764 1884 005a 1465 0c64  ...Z.d.d...Z.e.d
-00000650: 1964 1a84 0083 015a 1564 1b64 1c84 005a  .d.....Z.d.d...Z
-00000660: 1687 0004 005a 1753 0029 1eda 064f 7574  .....Z.S.)...Out
-00000670: 7075 74da 0170 da01 55da 1374 7261 6e73  put..p..U..trans
-00000680: 706f 7274 5072 6f70 6572 7469 6573 da14  portProperties..
-00000690: 7475 7262 756c 656e 6365 5072 6f70 6572  turbulenceProper
-000006a0: 7469 6573 2904 da0b 636f 6e74 726f 6c44  ties)...controlD
-000006b0: 6963 74da 0966 7653 6368 656d 6573 da0a  ict..fvSchemes..
-000006c0: 6676 536f 6c75 7469 6f6e da10 6465 636f  fvSolution..deco
-000006d0: 6d70 6f73 6550 6172 4469 6374 5a0e 7369  mposeParDictZ.si
-000006e0: 6d75 6c61 7469 6f6e 5479 7065 5a07 6c61  mulationTypeZ.la
-000006f0: 6d69 6e61 7263 0200 0000 0000 0000 0000  minarc..........
-00000700: 0000 0300 0000 0300 0000 4300 0000 7328  ..........C...s(
-00000710: 0000 007c 016a 006a 01a0 0264 01a1 017d  ...|.j.j...d...}
-00000720: 027c 00a0 037c 02a1 0101 007c 016a 006a  .|...|.....|.j.j
-00000730: 01a0 04a1 0001 0064 0253 0029 037a 6643  .......d.S.).zfC
-00000740: 6f6d 706c 6574 6520 7468 6520 696e 666f  omplete the info
-00000750: 5f73 6f6c 7665 7220 696e 7374 616e 6365  _solver instance
-00000760: 2077 6974 6820 6368 696c 6420 636c 6173   with child clas
-00000770: 7320 6465 7461 696c 7320 286d 6f64 756c  s details (modul
-00000780: 650a 2020 2020 2020 2020 616e 6420 636c  e.        and cl
-00000790: 6173 7320 6e61 6d65 7329 2e0a 0a20 2020  ass names)...   
-000007a0: 2020 2020 20da 0763 6c61 7373 6573 4e29       ..classesN)
-000007b0: 0572 3a00 0000 7231 0000 00da 0a5f 7365  .r:...r1....._se
-000007c0: 745f 6368 696c 64da 185f 7365 745f 696e  t_child.._set_in
-000007d0: 666f 5f73 6f6c 7665 725f 636c 6173 7365  fo_solver_classe
-000007e0: 73da 1563 6f6d 706c 6574 655f 7769 7468  s..complete_with
-000007f0: 5f63 6c61 7373 6573 2903 da03 636c 73da  _classes)...cls.
-00000800: 0b69 6e66 6f5f 736f 6c76 6572 723a 0000  .info_solverr:..
-00000810: 0072 2e00 0000 722e 0000 0072 2f00 0000  .r....r....r/...
-00000820: da15 5f63 6f6d 706c 6574 655f 696e 666f  .._complete_info
-00000830: 5f73 6f6c 7665 7253 0000 0073 0600 0000  _solverS...s....
-00000840: 0e06 0a01 1002 7a1c 4f75 7470 7574 2e5f  ......z.Output._
-00000850: 636f 6d70 6c65 7465 5f69 6e66 6f5f 736f  complete_info_so
-00000860: 6c76 6572 6302 0000 0000 0000 0000 0000  lverc...........
-00000870: 0002 0000 0007 0000 0043 0000 0073 2c00  .........C...s,.
-00000880: 0000 7c01 a000 6401 7401 6402 6401 6403  ..|...d.t.d.d.d.
-00000890: 8d02 a102 0100 7c01 a000 6404 7401 6405  ......|...d.t.d.
-000008a0: 6404 6403 8d02 a102 0100 6406 5300 2907  d.d.......d.S.).
-000008b0: 7a2e 5365 7420 7468 6520 636c 6173 7365  z.Set the classe
-000008c0: 7320 666f 7220 696e 666f 5f73 6f6c 7665  s for info_solve
-000008d0: 722e 636c 6173 7365 732e 4f75 7470 7574  r.classes.Output
-000008e0: 5a03 4c6f 677a 1766 6c75 6964 7369 6d66  Z.Logz.fluidsimf
-000008f0: 6f61 6d2e 6f75 7470 7574 2e6c 6f67 2902  oam.output.log).
-00000900: da0b 6d6f 6475 6c65 5f6e 616d 65da 0a63  ..module_name..c
-00000910: 6c61 7373 5f6e 616d 655a 0646 6965 6c64  lass_nameZ.Field
-00000920: 737a 1a66 6c75 6964 7369 6d66 6f61 6d2e  sz.fluidsimfoam.
-00000930: 6f75 7470 7574 2e66 6965 6c64 734e 2902  output.fieldsN).
-00000940: 723b 0000 00da 0464 6963 7429 0272 3e00  r;.....dict).r>.
-00000950: 0000 723a 0000 0072 2e00 0000 722e 0000  ..r:...r....r...
-00000960: 0072 2f00 0000 723c 0000 005e 0000 0073  .r/...r<...^...s
-00000970: 1c00 0000 0403 0201 0201 0201 0201 04fe  ................
-00000980: 04fe 0408 0201 0201 0201 0201 04fe 08fe  ................
-00000990: 7a1f 4f75 7470 7574 2e5f 7365 745f 696e  z.Output._set_in
-000009a0: 666f 5f73 6f6c 7665 725f 636c 6173 7365  fo_solver_classe
-000009b0: 7363 0100 0000 0000 0000 0000 0000 0400  sc..............
-000009c0: 0000 0700 0000 4300 0000 7362 0000 0069  ......C...sb...i
-000009d0: 0004 007d 017c 005f 007c 006a 0144 005d  ...}.|._.|.j.D.]
-000009e0: 0c7d 0274 027c 0283 017c 017c 02a0 0364  .}.t.|...|.|...d
-000009f0: 0164 02a1 023c 0071 087c 006a 0444 005d  .d...<.q.|.j.D.]
-00000a00: 097d 0374 027c 0364 0383 027c 017c 033c  .}.t.|.d...|.|.<
-00000a10: 0071 187c 006a 0544 005d 097d 0374 027c  .q.|.j.D.].}.t.|
-00000a20: 0364 0483 027c 017c 033c 0071 2564 0053  .d...|.|.<.q%d.S
-00000a30: 0029 054e da01 2eda 015f da08 636f 6e73  .).N....._..cons
-00000a40: 7461 6e74 da06 7379 7374 656d 2906 da18  tant..system)...
-00000a50: 5f66 696c 655f 6765 6e65 7261 746f 7273  _file_generators
-00000a60: 5f63 6c61 7373 6573 da0e 6e61 6d65 5f76  _classes..name_v
-00000a70: 6172 6961 626c 6573 720d 0000 00da 0772  ariablesr......r
-00000a80: 6570 6c61 6365 da13 6e61 6d65 5f63 6f6e  eplace..name_con
-00000a90: 7374 616e 745f 6669 6c65 73da 116e 616d  stant_files..nam
-00000aa0: 655f 7379 7374 656d 5f66 696c 6573 2904  e_system_files).
-00000ab0: 723e 0000 0072 3a00 0000 5a0d 7661 7269  r>...r:...Z.vari
-00000ac0: 6162 6c65 5f6e 616d 65da 0966 696c 655f  able_name..file_
-00000ad0: 6e61 6d65 722e 0000 0072 2e00 0000 722f  namer....r....r/
-00000ae0: 0000 00da 1e5f 7365 7475 705f 6669 6c65  ....._setup_file
-00000af0: 5f67 656e 6572 6174 6f72 735f 636c 6173  _generators_clas
-00000b00: 7365 7371 0000 0073 1400 0000 0a02 0a01  sesq...s........
-00000b10: 0201 0201 12ff 0a04 1001 0a02 1001 04ff  ................
-00000b20: 7a25 4f75 7470 7574 2e5f 7365 7475 705f  z%Output._setup_
-00000b30: 6669 6c65 5f67 656e 6572 6174 6f72 735f  file_generators_
-00000b40: 636c 6173 7365 7363 0300 0000 0000 0000  classesc........
-00000b50: 0000 0000 0400 0000 0700 0000 4300 0000  ............C...
-00000b60: 7374 0000 007c 00a0 00a1 0001 0074 017c  st...|.......t.|
-00000b70: 017c 027c 006a 02a0 03a1 0083 0301 007c  .|.|.j.........|
-00000b80: 01a0 0474 0564 0164 0264 0364 048d 03a1  ...t.d.d.d.d....
-00000b90: 0101 007c 016a 0664 0564 0164 0664 079c  ...|.j.d.d.d.d..
-00000ba0: 0264 088d 0201 007c 016a 07a0 0874 09a0  .d.....|.j...t..
-00000bb0: 0a64 09a1 01a1 0101 007c 026a 0b6a 0ca0  .d.......|.j.j..
-00000bc0: 0da1 007d 0374 017c 017c 027c 03a0 03a1  ...}.t.|.|.|....
-00000bd0: 0083 0301 0064 0353 0029 0a7a 3e54 6869  .....d.S.).z>Thi
-00000be0: 7320 7374 6174 6963 206d 6574 686f 6420  s static method 
-00000bf0: 6973 2075 7365 6420 746f 2063 6f6d 706c  is used to compl
-00000c00: 6574 6520 7468 6520 2a70 6172 616d 732a  ete the *params*
-00000c10: 2063 6f6e 7461 696e 6572 2e54 da03 7275   container.T..ru
-00000c20: 6e4e 2903 da0f 4e45 575f 4449 525f 5245  nN)...NEW_DIR_RE
-00000c30: 5355 4c54 535a 1373 686f 7274 5f6e 616d  SULTSZ.short_nam
-00000c40: 655f 7479 7065 5f72 756e 7219 0000 00da  e_type_runr.....
-00000c50: 066f 7574 7075 74da 0029 02da 0b48 4153  .output..)...HAS
-00000c60: 5f54 4f5f 5341 5645 da0d 7375 625f 6469  _TO_SAVE..sub_di
-00000c70: 7265 6374 6f72 7929 01da 0761 7474 7269  rectory)...attri
-00000c80: 6273 612e 0100 000a 2020 2020 2d20 6060  bsa.....    - ``
-00000c90: 4841 535f 544f 5f53 4156 4560 603a 2062  HAS_TO_SAVE``: b
-00000ca0: 6f6f 6c20 2864 6566 6175 6c74 3a20 5472  ool (default: Tr
-00000cb0: 7565 2920 4966 2046 616c 7365 2c20 6e6f  ue) If False, no
-00000cc0: 7468 696e 6720 6e65 7720 6973 2073 6176  thing new is sav
-00000cd0: 6564 2069 6e0a 2020 2020 2020 7468 6520  ed in.      the 
-00000ce0: 6469 7265 6374 6f72 7920 6f66 2074 6865  directory of the
-00000cf0: 2073 696d 756c 6174 696f 6e2e 0a20 2020   simulation..   
-00000d00: 202d 2060 6073 7562 5f64 6972 6563 746f   - ``sub_directo
-00000d10: 7279 6060 3a20 7374 7220 2864 6566 6175  ry``: str (defau
-00000d20: 6c74 3a20 2222 2920 4120 6e61 6d65 206f  lt: "") A name o
-00000d30: 6620 6120 7375 622d 6469 7265 6374 6f72  f a sub-director
-00000d40: 7920 2872 656c 6174 6976 650a 2020 2020  y (relative.    
-00000d50: 2020 746f 2024 464c 5549 4444 594e 5f50    to $FLUIDDYN_P
-00000d60: 4154 485f 5343 5241 5443 4829 2077 6865  ATH_SCRATCH) whe
-00000d70: 7265 696e 2074 6865 2064 6972 6563 746f  rein the directo
-00000d80: 7279 206f 6620 7468 6520 7369 6d75 6c61  ry of the simula
-00000d90: 7469 6f6e 0a20 2020 2020 2028 6060 7061  tion.      (``pa
-00000da0: 7468 5f72 756e 6060 2920 6973 2073 6176  th_run``) is sav
-00000db0: 6564 2e0a 0a29 0e72 4e00 0000 7208 0000  ed...).rN...r...
-00000dc0: 0072 4800 0000 da06 7661 6c75 6573 da0c  .rH.....values..
-00000dd0: 5f73 6574 5f61 7474 7269 6273 7243 0000  _set_attribsrC..
-00000de0: 0072 3b00 0000 7251 0000 00da 085f 7365  .r;...rQ....._se
-00000df0: 745f 646f 63da 0874 6578 7477 7261 70da  t_doc..textwrap.
-00000e00: 0664 6564 656e 7472 3a00 0000 7231 0000  .dedentr:...r1..
-00000e10: 00da 0e69 6d70 6f72 745f 636c 6173 7365  ...import_classe
-00000e20: 7329 0472 3e00 0000 da06 7061 7261 6d73  s).r>.....params
-00000e30: 723f 0000 00da 0c64 6963 745f 636c 6173  r?.....dict_clas
-00000e40: 7365 7372 2e00 0000 722e 0000 0072 2f00  sesr....r....r/.
-00000e50: 0000 da1d 5f63 6f6d 706c 6574 655f 7061  ...._complete_pa
-00000e60: 7261 6d73 5f77 6974 685f 6465 6661 756c  rams_with_defaul
-00000e70: 747f 0000 0073 2200 0000 0804 0201 0c01  t....s".........
-00000e80: 04ff 0405 0c01 04ff 0403 0a01 06ff 0603  ................
-00000e90: 0401 0201 02ff 04ff 0c0d 1401 7a24 4f75  ............z$Ou
-00000ea0: 7470 7574 2e5f 636f 6d70 6c65 7465 5f70  tput._complete_p
-00000eb0: 6172 616d 735f 7769 7468 5f64 6566 6175  arams_with_defau
-00000ec0: 6c74 4e63 0300 0000 0000 0000 0000 0000  ltNc............
-00000ed0: 0b00 0000 0800 0000 0300 0000 733c 0200  ............s<..
-00000ee0: 007c 017c 005f 007a 087c 016a 016a 026a  .|.|._.z.|.j.j.j
-00000ef0: 037c 005f 0457 006e 0904 0074 0579 1401  .|._.W.n...t.y..
-00000f00: 0001 0001 0059 006e 0777 0074 067c 006a  .....Y.n.w.t.|.j
-00000f10: 0483 017c 005f 077c 00a0 08a1 007c 005f  ...|._.|.....|._
-00000f20: 097c 0172 2e7c 016a 0a6a 0b7c 005f 0a74  .|.r.|.j.j.|._.t
-00000f30: 0c83 00a0 0d7c 01a1 0101 006e 0f7c 0272  .....|.....n.|.r
-00000f40: 357c 026a 0b7c 005f 0a6e 0864 007c 005f  5|.j.|._.n.d.|._
-00000f50: 0a74 0ea0 0f64 01a1 0101 007c 0173 4164  .t...d.....|.sAd
-00000f60: 0053 0074 107c 006a 1183 017c 005f 1174  .S.t.|.j...|._.t
-00000f70: 127c 0083 017c 005f 137c 016a 016a 026a  .|...|._.|.j.j.j
-00000f80: 146a 15a0 16a1 007d 037c 03a0 17a1 0044  .j.....}.|.....D
-00000f90: 005d 265c 027d 047d 0574 187c 007c 0583  .]&\.}.}.t.|.|..
-00000fa0: 0272 6271 5874 197c 0483 017d 067c 006a  .rbqXt.|...}.|.j
-00000fb0: 0004 006a 1a64 02a0 1b64 037c 069b 0064  ...j.d...d.|...d
-00000fc0: 049d 037c 05a1 0237 0002 005f 1a74 1c7c  ...|...7..._.t.|
-00000fd0: 007c 067c 057c 0083 0183 0301 0071 5874  .|.|.|.......qXt
-00000fe0: 1d7c 0064 0583 0273 887c 00a0 1ea1 0001  .|.d...s.|......
-00000ff0: 0069 007d 077c 006a 1fa0 17a1 0044 005d  .i.}.|.j.....D.]
-00001000: 255c 027d 047d 0574 197c 0483 017d 067c  %\.}.}.t.|...}.|
-00001010: 056a 207c 0776 0172 a37c 0467 017c 077c  .j |.v.r.|.g.|.|
-00001020: 056a 203c 006e 087c 077c 056a 2019 00a0  .j <.n.|.|.j ...
-00001030: 217c 04a1 0101 0074 1c7c 006a 137c 067c  !|.....t.|.j.|.|
-00001040: 057c 0083 0183 0301 0071 8f7c 0772 dc7c  .|.......q.|.r.|
-00001050: 006a 0004 006a 1a64 0637 0002 005f 1a7c  .j...j.d.7..._.|
-00001060: 07a0 17a1 0044 005d 185c 027d 087d 097c  .....D.].\.}.}.|
-00001070: 006a 0004 006a 1a64 077c 0864 0817 0064  .j...j.d.|.d...d
-00001080: 099b 0464 0aa0 227c 09a1 019b 0064 0b9d  ...d.."|.....d..
-00001090: 0437 0002 005f 1a71 c374 236a 2464 0c6b  .7..._.q.t#j$d.k
-000010a0: 0272 e97c 006a 2572 e97c 006a 006a 0a6a  .r.|.j%r.|.j.j.j
-000010b0: 2673 eb64 0053 007c 006a 1164 0d1b 00a0  &s.d.S.|.j.d....
-000010c0: 27a1 0001 007c 006a 1164 0e1b 00a0 27a1  '....|.j.d....'.
-000010d0: 0001 007c 006a 1164 0f1b 00a0 27a1 0001  ...|.j.d....'...
-000010e0: 0074 287c 006a 1383 01a0 29a1 0044 005d  .t(|.j....)..D.]
-000010f0: 147d 0a74 1d7c 0a64 1083 0290 0172 1a7c  .}.t.|.d.....r.|
-00001100: 0a6a 2aa0 2b64 0da1 0190 0172 1a7c 0aa0  .j*.+d.....r.|..
-00001110: 2ca1 0001 0090 0171 0764 0053 0029 114e  ,......q.d.S.).N
-00001120: 7a45 496e 6974 6961 6c69 7a69 6e67 204f  zEInitializing O
-00001130: 7574 7075 7420 636c 6173 7320 7769 7468  utput class with
-00001140: 6f75 7420 7369 6d20 6f72 2070 6172 616d  out sim or param
-00001150: 7320 6d69 6768 7420 6c65 6164 2074 6f20  s might lead to 
-00001160: 6572 726f 7273 2e7a 097b 3a32 3873 7d7b  errors.z.{:28s}{
-00001170: 7d0a 7a0b 7369 6d2e 6f75 7470 7574 2e7a  }.z.sim.output.z
-00001180: 023a 2072 4800 0000 7a0d 696e 7075 745f  .: rH...z.input_
-00001190: 6669 6c65 733a 0a7a 0720 202d 2069 6e20  files:.z.  - in 
-000011a0: fa01 3a5a 0331 3273 da01 20da 010a 7201  ..:Z.12s.. ...r.
-000011b0: 0000 0072 4700 0000 da01 3072 4600 0000  ...rG.....0rF...
-000011c0: da0d 6765 6e65 7261 7465 5f66 696c 6529  ..generate_file)
-000011d0: 2dda 0373 696d da04 696e 666f da06 736f  -..sim..info..so
-000011e0: 6c76 6572 da0a 7368 6f72 745f 6e61 6d65  lver..short_name
-000011f0: da0b 6e61 6d65 5f73 6f6c 7665 72da 0e41  ..name_solver..A
-00001200: 7474 7269 6275 7465 4572 726f 7272 0f00  ttributeErrorr..
-00001210: 0000 da07 7061 636b 6167 65da 1767 6574  ....package..get
-00001220: 5f70 6174 685f 736f 6c76 6572 5f70 6163  _path_solver_pac
-00001230: 6b61 6765 5a13 7061 7468 5f73 6f6c 7665  kageZ.path_solve
-00001240: 725f 7061 636b 6167 6572 5c00 0000 7251  r_packager\...rQ
-00001250: 0000 00da 0573 7570 6572 da08 5f5f 696e  .....super..__in
-00001260: 6974 5f5f 720e 0000 00da 0777 6172 6e69  it__r......warni
-00001270: 6e67 7203 0000 0072 2800 0000 720c 0000  ngr....r(...r...
-00001280: 00da 0b69 6e70 7574 5f66 696c 6573 723a  ...input_filesr:
-00001290: 0000 0072 3100 0000 725b 0000 00da 0569  ...r1...r[.....i
-000012a0: 7465 6d73 7212 0000 0072 0400 0000 da11  temsr....r......
-000012b0: 5f6f 626a 6563 7473 5f74 6f5f 7072 696e  _objects_to_prin
-000012c0: 74da 0666 6f72 6d61 74da 0773 6574 6174  t..format..setat
-000012d0: 7472 da07 6861 7361 7474 7272 4e00 0000  tr..hasattrrN...
-000012e0: 7248 0000 00da 0864 6972 5f6e 616d 65da  rH.....dir_name.
-000012f0: 0661 7070 656e 64da 046a 6f69 6e72 0600  .append..joinr..
-00001300: 0000 da04 7261 6e6b da0c 5f68 6173 5f74  ....rank.._has_t
-00001310: 6f5f 7361 7665 7250 0000 00da 056d 6b64  o_saverP.....mkd
-00001320: 6972 da04 7661 7273 7256 0000 00da 0872  ir..varsrV.....r
-00001330: 656c 5f70 6174 6872 1600 0000 7263 0000  el_pathr....rc..
-00001340: 0029 0bda 0473 656c 6672 6400 0000 725c  .)...selfrd...r\
-00001350: 0000 0072 5d00 0000 da08 636c 735f 6e61  ...r].....cls_na
-00001360: 6d65 da05 436c 6173 73da 086f 626a 5f6e  me..Class..obj_n
-00001370: 616d 655a 1366 6f72 5f73 7472 5f69 6e70  ameZ.for_str_inp
-00001380: 7574 5f66 696c 6573 7275 0000 0072 6f00  ut_filesru...ro.
-00001390: 0000 da0e 6669 6c65 5f67 656e 6572 6174  ....file_generat
-000013a0: 6f72 a901 da09 5f5f 636c 6173 735f 5f72  or....__class__r
-000013b0: 2e00 0000 722f 0000 0072 6d00 0000 9f00  ....r/...rm.....
-000013c0: 0000 7380 0000 0006 0102 0110 010c 0104  ..s.............
-000013d0: 0102 ff0c 030a 0204 020a 020e 0104 010a  ................
-000013e0: 0206 0204 0102 0104 ff04 0404 010c 020a  ................
-000013f0: 0210 0210 010a 0102 0108 010c 010c 0108  ................
-00001400: ff12 030a 0208 0104 0112 0108 010a 020e  ................
-00001410: 0110 0214 0104 0210 0110 0108 011a 0108  ................
-00001420: ff08 0502 ff04 0202 fe08 0302 fd04 050e  ................
-00001430: 020e 010e 0112 0202 0104 0106 ff0a 0204  ................
-00001440: fe08 0304 8004 fc7a 0f4f 7574 7075 742e  .......z.Output.
-00001450: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
-00001460: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
-00001470: 0073 1200 0000 7400 7401 a002 7c00 a101  .s....t.t...|...
-00001480: 6a03 8301 6a04 5300 2901 7a28 4765 7420  j...j.S.).z(Get 
-00001490: 7468 6520 7061 7468 2074 6f77 6172 6473  the path towards
-000014a0: 2074 6865 2073 6f6c 7665 7220 7061 636b   the solver pack
-000014b0: 6167 652e 2905 7203 0000 00da 0769 6e73  age.).r......ins
-000014c0: 7065 6374 da09 6765 746d 6f64 756c 65da  pect..getmodule.
-000014d0: 085f 5f66 696c 655f 5fda 0670 6172 656e  .__file__..paren
-000014e0: 7429 0172 3e00 0000 722e 0000 0072 2e00  t).r>...r....r..
-000014f0: 0000 722f 0000 0072 6b00 0000 ec00 0000  ..r/...rk.......
-00001500: 7302 0000 0012 037a 1e4f 7574 7075 742e  s......z.Output.
-00001510: 6765 745f 7061 7468 5f73 6f6c 7665 725f  get_path_solver_
-00001520: 7061 636b 6167 6563 0100 0000 0000 0000  packagec........
-00001530: 0000 0000 0400 0000 0800 0000 0300 0000  ................
-00001540: 73d8 0000 0074 006a 0164 016b 0272 0d74  s....t.j.d.k.r.t
-00001550: 0264 027c 006a 039b 009d 0283 0101 0074  .d.|.j.........t
-00001560: 0483 008f 0d01 0074 0583 00a0 06a1 0001  .......t........
-00001570: 0057 0064 0304 0004 0083 0301 006e 0831  .W.d.........n.1
-00001580: 0073 2077 0101 0001 0001 0059 0001 0074  .s w.......Y...t
-00001590: 07a0 087c 006a 096a 0aa1 0101 0074 006a  ...|.j.j.....t.j
-000015a0: 0164 016b 0272 397c 006a 0b72 397c 006a  .d.k.r9|.j.r9|.j
-000015b0: 096a 0c6a 0d73 3b64 0353 0074 0e7c 006a  .j.j.s;d.S.t.|.j
-000015c0: 096a 0c6a 0f7c 006a 0383 0201 007c 00a0  .j.j.|.j.....|..
-000015d0: 10a1 0001 007c 006a 0364 041b 007d 017c  .....|.j.d...}.|
-000015e0: 016a 1164 0564 068d 0101 0064 0744 005d  .j.d.d.....d.D.]
-000015f0: 147d 027c 017c 021b 007d 037c 03a0 12a1  .}.|.|...}.|....
-00001600: 0072 6071 5574 13a0 147c 006a 037c 021b  .r`qUt...|.j.|..
-00001610: 007c 03a1 0201 0071 5564 0353 0029 087a  .|.....qUd.S.).z
-00001620: 214c 6f67 7320 696e 666f 206f 6e20 696e  !Logs info on in
-00001630: 7374 616e 7469 6174 6564 2063 6c61 7373  stantiated class
-00001640: 6573 7201 0000 007a 0a70 6174 685f 7275  esr....z.path_ru
-00001650: 6e3a 204e 7a0e 2e64 6174 615f 666c 7569  n: Nz..data_flui
-00001660: 6473 696d 5429 01da 0865 7869 7374 5f6f  dsimT)...exist_o
-00001670: 6b29 027a 0f69 6e66 6f5f 736f 6c76 6572  k).z.info_solver
-00001680: 2e78 6d6c 7a10 7061 7261 6d73 5f73 696d  .xmlz.params_sim
-00001690: 756c 2e78 6d6c 2915 7206 0000 0072 7800  ul.xml).r....rx.
-000016a0: 0000 da05 7072 696e 7472 2800 0000 7205  ....printr(...r.
-000016b0: 0000 0072 6c00 0000 da09 706f 7374 5f69  ...rl.....post_i
-000016c0: 6e69 7472 0e00 0000 7265 0000 0072 6400  nitr....re...rd.
-000016d0: 0000 7271 0000 0072 7900 0000 725c 0000  ..rq...ry...r\..
-000016e0: 0072 5000 0000 7230 0000 0072 1900 0000  .rP...r0...r....
-000016f0: da29 5f70 6f73 745f 696e 6974 5f63 7265  .)_post_init_cre
-00001700: 6174 655f 6164 6469 7469 6f6e 616c 5f73  ate_additional_s
-00001710: 6f75 7263 655f 6669 6c65 7372 7a00 0000  ource_filesrz...
-00001720: 7227 0000 0072 2100 0000 7222 0000 0029  r'...r!...r"...)
-00001730: 0472 7d00 0000 5a12 7061 7468 5f69 6e66  .r}...Z.path_inf
-00001740: 6f5f 666c 7569 6473 696d 724d 0000 005a  o_fluidsimrM...Z
-00001750: 0870 6174 685f 6e65 7772 8200 0000 722e  .path_newr....r.
-00001760: 0000 0072 2f00 0000 728a 0000 00f1 0000  ...r/...r.......
-00001770: 0073 2e00 0000 0a03 1001 0803 0c01 1cff  .s..............
-00001780: 0e03 0804 02ff 0402 02fe 0803 02fd 0405  ................
-00001790: 1202 0801 0a03 0c01 0801 0801 0801 0201  ................
-000017a0: 1401 04fc 7a10 4f75 7470 7574 2e70 6f73  ....z.Output.pos
-000017b0: 745f 696e 6974 6301 0000 0000 0000 0000  t_initc.........
-000017c0: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
-000017d0: 6c00 0000 7c00 6a00 6a01 6401 1b00 7d01  l...|.j.j.d...}.
-000017e0: 7c01 a002 a100 7313 7403 6402 7c00 6a00  |.....s.t.d.|.j.
-000017f0: 6a01 9b00 9d02 8301 8201 7404 a005 7c01  j.........t...|.
-00001800: 7c00 6a06 6a07 a102 0100 7408 7c00 6a00  |.j.j.....t.|.j.
-00001810: 8301 a009 a100 4400 5d11 7d02 740a 7c02  ......D.].}.t.|.
-00001820: 6403 8302 7233 7c02 6a0b a00c 6404 a101  d...r3|.j...d...
-00001830: 7333 7c02 a00d a100 0100 7122 6405 5300  s3|.......q"d.S.
-00001840: 2906 7a24 4372 6561 7465 2074 6865 2066  ).z$Create the f
-00001850: 696c 6573 2066 726f 6d20 7468 6569 7220  iles from their 
-00001860: 7465 6d70 6c61 7465 7a08 7461 736b 732e  templatez.tasks.
-00001870: 7079 7a29 7461 736b 732e 7079 206d 6973  pyz)tasks.py mis
-00001880: 7369 6e67 2069 6e20 736f 6c76 6572 2074  sing in solver t
-00001890: 656d 706c 6174 6573 5f64 6972 2072 6300  emplates_dir rc.
-000018a0: 0000 7247 0000 004e 290e 726f 0000 005a  ..rG...N).ro...Z
-000018b0: 0d74 656d 706c 6174 6573 5f64 6972 7227  .templates_dirr'
-000018c0: 0000 00da 0c52 756e 7469 6d65 4572 726f  .....RuntimeErro
-000018d0: 7272 2100 0000 7222 0000 0072 6400 0000  rr!...r"...rd...
-000018e0: 7228 0000 0072 7b00 0000 7256 0000 0072  r(...r{...rV...r
-000018f0: 7400 0000 727c 0000 0072 1600 0000 7263  t...r|...r....rc
-00001900: 0000 0029 0372 7d00 0000 5a0d 7061 7468  ...).r}...Z.path
-00001910: 5f74 6173 6b73 5f70 7972 8100 0000 722e  _tasks_pyr....r.
-00001920: 0000 0072 2e00 0000 722f 0000 0072 8b00  ...r....r/...r..
-00001930: 0000 1101 0000 7322 0000 000c 0208 0102  ......s"........
-00001940: 0102 0106 0104 ff04 ff10 0412 0202 0104  ................
-00001950: 0104 ff0a 0202 fe08 0402 8004 fb7a 304f  .............z0O
-00001960: 7574 7075 742e 5f70 6f73 745f 696e 6974  utput._post_init
-00001970: 5f63 7265 6174 655f 6164 6469 7469 6f6e  _create_addition
-00001980: 616c 5f73 6f75 7263 655f 6669 6c65 7363  al_source_filesc
-00001990: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-000019a0: 0800 0000 4300 0000 7328 0000 0064 0164  ....C...s(...d.d
-000019b0: 0164 0164 0264 0264 0264 0364 049c 077d  .d.d.d.d.d.d...}
-000019c0: 027c 016a 0064 057c 0264 0664 078d 0301  .|.j.d.|.d.d....
-000019d0: 0064 0053 0029 084e e928 0000 0067 0000  .d.S.).N.(...g..
-000019e0: 0000 0000 f03f e901 0000 0029 07da 026e  .....?.....)...n
-000019f0: 78da 026e 79da 026e 7ada 026c 78da 026c  x..ny..nz..lx..l
-00001a00: 79da 026c 7ada 0573 6361 6c65 da0f 626c  y..lz..scale..bl
-00001a10: 6f63 6b5f 6d65 7368 5f64 6963 74da 0454  ock_mesh_dict..T
-00001a20: 4f44 4f29 0272 5500 0000 da03 646f 6329  ODO).rU.....doc)
-00001a30: 0172 3b00 0000 2903 723e 0000 0072 5c00  .r;...).r>...r\.
-00001a40: 0000 da07 6465 6661 756c 7472 2e00 0000  ....defaultr....
-00001a50: 722e 0000 0072 2f00 0000 da20 5f63 6f6d  r....r/.... _com
-00001a60: 706c 6574 655f 7061 7261 6d73 5f62 6c6f  plete_params_blo
-00001a70: 636b 5f6d 6573 685f 6469 6374 2201 0000  ck_mesh_dict"...
-00001a80: 731a 0000 0002 0302 0102 0102 0102 0102  s...............
-00001a90: 0102 0106 f904 0a02 0102 0102 010a fd7a  ...............z
-00001aa0: 274f 7574 7075 742e 5f63 6f6d 706c 6574  'Output._complet
-00001ab0: 655f 7061 7261 6d73 5f62 6c6f 636b 5f6d  e_params_block_m
-00001ac0: 6573 685f 6469 6374 6303 0000 0000 0000  esh_dictc.......
-00001ad0: 0000 0000 0003 0000 0001 0000 0043 0000  .............C..
-00001ae0: 0073 0400 0000 6900 5300 2901 4e72 2e00  .s....i.S.).Nr..
-00001af0: 0000 2903 727d 0000 005a 0474 6d69 6e5a  ..).r}...Z.tminZ
-00001b00: 0474 6d61 7872 2e00 0000 722e 0000 0072  .tmaxr....r....r
-00001b10: 2f00 0000 da14 5f63 6f6d 7075 7465 5f6d  /....._compute_m
-00001b20: 6561 6e5f 7661 6c75 6573 3401 0000 7302  ean_values4...s.
-00001b30: 0000 0004 017a 1b4f 7574 7075 742e 5f63  .....z.Output._c
-00001b40: 6f6d 7075 7465 5f6d 6561 6e5f 7661 6c75  ompute_mean_valu
-00001b50: 6573 2902 4e4e 2918 da08 5f5f 6e61 6d65  es).NN)...__name
-00001b60: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00001b70: 5f5f 7175 616c 6e61 6d65 5f5f 7249 0000  __qualname__rI..
-00001b80: 0072 4b00 0000 724c 0000 0072 0900 0000  .rK...rL...r....
-00001b90: 5a1d 5f68 656c 7065 725f 7475 7262 756c  Z._helper_turbul
-00001ba0: 656e 6365 5f70 726f 7065 7274 6965 7372  ence_propertiesr
-00001bb0: 0b00 0000 5a1a 5f68 656c 7065 725f 6465  ....Z._helper_de
-00001bc0: 636f 6d70 6f73 655f 7061 725f 6469 6374  compose_par_dict
-00001bd0: 720a 0000 00da 145f 6865 6c70 6572 5f63  r......_helper_c
-00001be0: 6f6e 7472 6f6c 5f64 6963 74da 0b63 6c61  ontrol_dict..cla
-00001bf0: 7373 6d65 7468 6f64 7240 0000 0072 3c00  ssmethodr@...r<.
-00001c00: 0000 724e 0000 0072 5e00 0000 726d 0000  ..rN...r^...rm..
-00001c10: 0072 6b00 0000 728a 0000 0072 8b00 0000  .rk...r....r....
-00001c20: 729a 0000 0072 9b00 0000 da0d 5f5f 636c  r....r......__cl
-00001c30: 6173 7363 656c 6c5f 5f72 2e00 0000 722e  asscell__r....r.
-00001c40: 0000 0072 8200 0000 722f 0000 0072 3100  ...r....r/...r1.
-00001c50: 0000 4300 0000 7332 0000 0008 0008 0108  ..C...s2........
-00001c60: 0108 0102 0708 0104 ff06 0306 0102 020a  ................
-00001c70: 0102 0a0a 0102 120a 0102 0d0a 010e 1f02  ................
-00001c80: 4d0a 010c 0408 2002 110a 0110 1172 3100  M..... ......r1.
-00001c90: 0000 2922 da07 5f5f 646f 635f 5f5a 1369  ..)"..__doc__Z.i
-00001ca0: 6d70 6f72 746c 6962 2e72 6573 6f75 7263  mportlib.resourc
-00001cb0: 6573 7218 0000 0072 8400 0000 721c 0000  esr....r....r...
-00001cc0: 0072 2100 0000 7259 0000 00da 0a63 6f6e  .r!...rY.....con
-00001cd0: 7465 7874 6c69 6272 0200 0000 da07 7061  textlibr......pa
-00001ce0: 7468 6c69 6272 0300 0000 da0a 696e 666c  thlibr......infl
-00001cf0: 6563 7469 6f6e 7204 0000 005a 0b66 6c75  ectionr....Z.flu
-00001d00: 6964 6479 6e2e 696f 7205 0000 005a 0d66  iddyn.ior....Z.f
-00001d10: 6c75 6964 6479 6e2e 7574 696c 7206 0000  luiddyn.utilr...
-00001d20: 005a 1466 6c75 6964 7369 6d5f 636f 7265  .Z.fluidsim_core
-00001d30: 2e6f 7574 7075 7472 0700 0000 da14 666c  .outputr......fl
-00001d40: 7569 6473 696d 5f63 6f72 652e 7061 7261  uidsim_core.para
-00001d50: 6d73 7208 0000 00da 1d66 6c75 6964 7369  msr......fluidsi
-00001d60: 6d66 6f61 6d2e 666f 616d 5f69 6e70 7574  mfoam.foam_input
-00001d70: 5f66 696c 6573 7209 0000 0072 0a00 0000  _filesr....r....
-00001d80: 720b 0000 005a 2866 6c75 6964 7369 6d66  r....Z(fluidsimf
-00001d90: 6f61 6d2e 666f 616d 5f69 6e70 7574 5f66  oam.foam_input_f
-00001da0: 696c 6573 2e67 656e 6572 6174 6f72 7372  iles.generatorsr
-00001db0: 0c00 0000 720d 0000 005a 1066 6c75 6964  ....r....Z.fluid
-00001dc0: 7369 6d66 6f61 6d2e 6c6f 6772 0e00 0000  simfoam.logr....
-00001dd0: da14 666c 7569 6473 696d 666f 616d 2e73  ..fluidsimfoam.s
-00001de0: 6f6c 7665 7273 720f 0000 0072 3000 0000  olversr....r0...
-00001df0: 7231 0000 0072 2e00 0000 722e 0000 0072  r1...r....r....r
-00001e00: 2e00 0000 722f 0000 00da 083c 6d6f 6475  ....r/.....<modu
-00001e10: 6c65 3e01 0000 0073 2600 0000 0400 0802  le>....s&.......
-00001e20: 0801 0801 0801 0801 0c01 0c01 0c02 0c02  ................
-00001e30: 0c01 0c01 0c01 1401 1005 0c04 0c01 0803  ................
-00001e40: 1425                                     .%
+000002f0: 046a 116a 1264 0564 068d 0101 007c 077c  .j.j.d.d.....|.|
+00000300: 0283 018f 2d7d 027c 02a0 13a1 0072 7774  ....-}.|.....rwt
+00000310: 14a0 157c 027c 04a1 0201 006e 1a7c 02a0  ...|.|.....n.|..
+00000320: 16a1 0072 8574 14a0 177c 027c 047c 026a  ...r.t...|.|.|.j
+00000330: 181b 00a1 0201 006e 0c74 1964 077c 029b  .......n.t.d.|..
+00000340: 0264 087c 02a0 1aa1 009b 029d 0483 0182  .d.|............
+00000350: 0157 0064 0004 0004 0083 0301 006e 0831  .W.d.........n.1
+00000360: 0073 9b77 0101 0001 0001 0059 0001 0071  .s.w.......Y...q
+00000370: 1064 0053 0029 094e 7a02 2d3e 7a0d 7061  .d.S.).Nz.->z.pa
+00000380: 636b 6167 652d 6461 7461 28fa 0129 fa01  ckage-data(..)..
+00000390: 2f54 a901 da08 6578 6973 745f 6f6b 7a0b  /T....exist_okz.
+000003a0: 7265 736f 7572 6365 203d 207a 162c 2072  resource = z., r
+000003b0: 6573 6f75 7263 652e 6578 6973 7473 2829  esource.exists()
+000003c0: 203d 2029 1bda 0a69 7369 6e73 7461 6e63   = )...isinstanc
+000003d0: 65da 0373 7472 da05 7370 6c69 74da 0573  e..str..split..s
+000003e0: 7472 6970 da0a 7374 6172 7473 7769 7468  trip..startswith
+000003f0: da0c 7265 6d6f 7665 7072 6566 6978 da09  ..removeprefix..
+00000400: 696d 706f 7274 6c69 62da 0972 6573 6f75  importlib..resou
+00000410: 7263 6573 da05 6669 6c65 73da 086a 6f69  rces..files..joi
+00000420: 6e70 6174 685a 0761 735f 6669 6c65 7203  npathZ.as_filer.
+00000430: 0000 00da 026f 73da 0470 6174 68da 0a65  .....os..path..e
+00000440: 7870 616e 6476 6172 73da 0a65 7870 616e  xpandvars..expan
+00000450: 6475 7365 7272 0200 0000 da06 7061 7265  duserr......pare
+00000460: 6e74 da05 6d6b 6469 72da 0769 735f 6669  nt..mkdir..is_fi
+00000470: 6c65 da06 7368 7574 696c da04 636f 7079  le..shutil..copy
+00000480: da06 6973 5f64 6972 da08 636f 7079 7472  ..is_dir..copytr
+00000490: 6565 da04 6e61 6d65 da13 4e6f 7449 6d70  ee..name..NotImp
+000004a0: 6c65 6d65 6e74 6564 4572 726f 72da 0665  lementedError..e
+000004b0: 7869 7374 7329 0872 1b00 0000 da08 7061  xists).r......pa
+000004c0: 7468 5f72 756e da08 7265 736f 7572 6365  th_run..resource
+000004d0: da0d 7265 6c61 7469 7665 5f70 6174 68da  ..relative_path.
+000004e0: 0b64 6573 7469 6e61 7469 6f6e da0c 7061  .destination..pa
+000004f0: 636b 6167 655f 6e61 6d65 5a10 6d75 6c74  ckage_nameZ.mult
+00000500: 6970 6c65 7865 645f 7061 7468 da0f 636f  iplexed_path..co
+00000510: 6e74 6578 745f 6d61 6e61 6765 72a9 0072  ntext_manager..r
+00000520: 3200 0000 fa3d 2f68 6f6d 652f 7069 6572  2....=/home/pier
+00000530: 7265 2f44 6576 2f66 6c75 6964 7369 6d66  re/Dev/fluidsimf
+00000540: 6f61 6d2f 7372 632f 666c 7569 6473 696d  oam/src/fluidsim
+00000550: 666f 616d 2f6f 7574 7075 742f 6261 7365  foam/output/base
+00000560: 2e70 79da 0e63 6f70 795f 7265 736f 7572  .py..copy_resour
+00000570: 6365 731e 0000 0073 4200 0000 0801 0401  ces....sB.......
+00000580: 0a01 0601 0802 0801 0801 0e01 0c01 0a01  ................
+00000590: 0402 0a02 0a01 0e01 0a01 0c01 0a01 0a01  ................
+000005a0: 1402 0401 0e02 0a01 0801 0e01 0801 1401  ................
+000005b0: 0202 1201 04ff 0280 1cfa 0280 04eb 7234  ..............r4
+000005c0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000005d0: 0000 0000 0400 0000 0000 0000 73b4 0000  ............s...
+000005e0: 0065 005a 0164 005a 0264 0164 0267 025a  .e.Z.d.Z.d.d.g.Z
+000005f0: 0364 0364 0467 025a 0467 0064 05a2 015a  .d.d.g.Z.g.d...Z
+00000600: 0565 0664 0464 0664 0769 0183 025a 0765  .e.d.d.d.i...Z.e
+00000610: 0883 005a 0965 0a83 005a 0b65 0c64 0864  ...Z.e...Z.e.d.d
+00000620: 0984 0083 015a 0d65 0c64 0a64 0b84 0083  .....Z.e.d.d....
+00000630: 015a 0e65 0c64 0c64 0d84 0083 015a 0f65  .Z.e.d.d.....Z.e
+00000640: 0c64 0e64 0f84 0083 015a 1064 1d87 0066  .d.d.....Z.d...f
+00000650: 0164 1164 1284 095a 1165 0c64 1364 1484  .d.d...Z.e.d.d..
+00000660: 0083 015a 1287 0066 0164 1564 1684 085a  ...Z...f.d.d...Z
+00000670: 1364 1764 1884 005a 1465 0c64 1964 1a84  .d.d...Z.e.d.d..
+00000680: 0083 015a 1564 1b64 1c84 005a 1687 0004  ...Z.d.d...Z....
+00000690: 005a 1753 0029 1eda 064f 7574 7075 74da  .Z.S.)...Output.
+000006a0: 0170 da01 555a 1374 7261 6e73 706f 7274  .p..UZ.transport
+000006b0: 5072 6f70 6572 7469 6573 da14 7475 7262  Properties..turb
+000006c0: 756c 656e 6365 5072 6f70 6572 7469 6573  ulenceProperties
+000006d0: 2904 da0b 636f 6e74 726f 6c44 6963 74da  )...controlDict.
+000006e0: 0966 7653 6368 656d 6573 da0a 6676 536f  .fvSchemes..fvSo
+000006f0: 6c75 7469 6f6e da10 6465 636f 6d70 6f73  lution..decompos
+00000700: 6550 6172 4469 6374 5a0e 7369 6d75 6c61  eParDictZ.simula
+00000710: 7469 6f6e 5479 7065 5a07 6c61 6d69 6e61  tionTypeZ.lamina
+00000720: 7263 0200 0000 0000 0000 0000 0000 0300  rc..............
+00000730: 0000 0300 0000 4300 0000 7328 0000 007c  ......C...s(...|
+00000740: 016a 006a 01a0 0264 01a1 017d 027c 00a0  .j.j...d...}.|..
+00000750: 037c 02a1 0101 007c 016a 006a 01a0 04a1  .|.....|.j.j....
+00000760: 0001 0064 0253 0029 037a 6643 6f6d 706c  ...d.S.).zfCompl
+00000770: 6574 6520 7468 6520 696e 666f 5f73 6f6c  ete the info_sol
+00000780: 7665 7220 696e 7374 616e 6365 2077 6974  ver instance wit
+00000790: 6820 6368 696c 6420 636c 6173 7320 6465  h child class de
+000007a0: 7461 696c 7320 286d 6f64 756c 650a 2020  tails (module.  
+000007b0: 2020 2020 2020 616e 6420 636c 6173 7320        and class 
+000007c0: 6e61 6d65 7329 2e0a 0a20 2020 2020 2020  names)...       
+000007d0: 20da 0763 6c61 7373 6573 4e29 0572 3d00   ..classesN).r=.
+000007e0: 0000 7235 0000 00da 0a5f 7365 745f 6368  ..r5....._set_ch
+000007f0: 696c 64da 185f 7365 745f 696e 666f 5f73  ild.._set_info_s
+00000800: 6f6c 7665 725f 636c 6173 7365 73da 1563  olver_classes..c
+00000810: 6f6d 706c 6574 655f 7769 7468 5f63 6c61  omplete_with_cla
+00000820: 7373 6573 2903 da03 636c 73da 0b69 6e66  sses)...cls..inf
+00000830: 6f5f 736f 6c76 6572 723d 0000 0072 3200  o_solverr=...r2.
+00000840: 0000 7232 0000 0072 3300 0000 da15 5f63  ..r2...r3....._c
+00000850: 6f6d 706c 6574 655f 696e 666f 5f73 6f6c  omplete_info_sol
+00000860: 7665 7254 0000 0073 0600 0000 0e06 0a01  verT...s........
+00000870: 1002 7a1c 4f75 7470 7574 2e5f 636f 6d70  ..z.Output._comp
+00000880: 6c65 7465 5f69 6e66 6f5f 736f 6c76 6572  lete_info_solver
+00000890: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+000008a0: 0007 0000 0043 0000 0073 2c00 0000 7c01  .....C...s,...|.
+000008b0: a000 6401 7401 6402 6401 6403 8d02 a102  ..d.t.d.d.d.....
+000008c0: 0100 7c01 a000 6404 7401 6405 6404 6403  ..|...d.t.d.d.d.
+000008d0: 8d02 a102 0100 6406 5300 2907 7a2e 5365  ......d.S.).z.Se
+000008e0: 7420 7468 6520 636c 6173 7365 7320 666f  t the classes fo
+000008f0: 7220 696e 666f 5f73 6f6c 7665 722e 636c  r info_solver.cl
+00000900: 6173 7365 732e 4f75 7470 7574 5a03 4c6f  asses.OutputZ.Lo
+00000910: 677a 1766 6c75 6964 7369 6d66 6f61 6d2e  gz.fluidsimfoam.
+00000920: 6f75 7470 7574 2e6c 6f67 2902 da0b 6d6f  output.log)...mo
+00000930: 6475 6c65 5f6e 616d 65da 0a63 6c61 7373  dule_name..class
+00000940: 5f6e 616d 655a 0646 6965 6c64 737a 1a66  _nameZ.Fieldsz.f
+00000950: 6c75 6964 7369 6d66 6f61 6d2e 6f75 7470  luidsimfoam.outp
+00000960: 7574 2e66 6965 6c64 734e 2902 723e 0000  ut.fieldsN).r>..
+00000970: 00da 0464 6963 7429 0272 4100 0000 723d  ...dict).rA...r=
+00000980: 0000 0072 3200 0000 7232 0000 0072 3300  ...r2...r2...r3.
+00000990: 0000 723f 0000 005f 0000 0073 1c00 0000  ..r?..._...s....
+000009a0: 0403 0201 0201 0201 0201 04fe 04fe 0408  ................
+000009b0: 0201 0201 0201 0201 04fe 08fe 7a1f 4f75  ............z.Ou
+000009c0: 7470 7574 2e5f 7365 745f 696e 666f 5f73  tput._set_info_s
+000009d0: 6f6c 7665 725f 636c 6173 7365 7363 0100  olver_classesc..
+000009e0: 0000 0000 0000 0000 0000 0400 0000 0700  ................
+000009f0: 0000 4300 0000 7362 0000 0069 0004 007d  ..C...sb...i...}
+00000a00: 017c 005f 007c 006a 0144 005d 0c7d 0274  .|._.|.j.D.].}.t
+00000a10: 027c 0283 017c 017c 02a0 0364 0164 02a1  .|...|.|...d.d..
+00000a20: 023c 0071 087c 006a 0444 005d 097d 0374  .<.q.|.j.D.].}.t
+00000a30: 027c 0364 0383 027c 017c 033c 0071 187c  .|.d...|.|.<.q.|
+00000a40: 006a 0544 005d 097d 0374 027c 0364 0483  .j.D.].}.t.|.d..
+00000a50: 027c 017c 033c 0071 2564 0053 0029 054e  .|.|.<.q%d.S.).N
+00000a60: da01 2eda 015f da08 636f 6e73 7461 6e74  ....._..constant
+00000a70: da06 7379 7374 656d 2906 da18 5f66 696c  ..system)..._fil
+00000a80: 655f 6765 6e65 7261 746f 7273 5f63 6c61  e_generators_cla
+00000a90: 7373 6573 da0e 6e61 6d65 5f76 6172 6961  sses..name_varia
+00000aa0: 626c 6573 720d 0000 00da 0772 6570 6c61  blesr......repla
+00000ab0: 6365 da13 6e61 6d65 5f63 6f6e 7374 616e  ce..name_constan
+00000ac0: 745f 6669 6c65 73da 116e 616d 655f 7379  t_files..name_sy
+00000ad0: 7374 656d 5f66 696c 6573 2904 7241 0000  stem_files).rA..
+00000ae0: 0072 3d00 0000 5a0d 7661 7269 6162 6c65  .r=...Z.variable
+00000af0: 5f6e 616d 65da 0966 696c 655f 6e61 6d65  _name..file_name
+00000b00: 7232 0000 0072 3200 0000 7233 0000 00da  r2...r2...r3....
+00000b10: 1e5f 7365 7475 705f 6669 6c65 5f67 656e  ._setup_file_gen
+00000b20: 6572 6174 6f72 735f 636c 6173 7365 7372  erators_classesr
+00000b30: 0000 0073 1400 0000 0a02 0a01 0201 0201  ...s............
+00000b40: 12ff 0a04 1001 0a02 1001 04ff 7a25 4f75  ............z%Ou
+00000b50: 7470 7574 2e5f 7365 7475 705f 6669 6c65  tput._setup_file
+00000b60: 5f67 656e 6572 6174 6f72 735f 636c 6173  _generators_clas
+00000b70: 7365 7363 0300 0000 0000 0000 0000 0000  sesc............
+00000b80: 0400 0000 0700 0000 4300 0000 7374 0000  ........C...st..
+00000b90: 007c 00a0 00a1 0001 0074 017c 017c 027c  .|.......t.|.|.|
+00000ba0: 006a 02a0 03a1 0083 0301 007c 01a0 0474  .j.........|...t
+00000bb0: 0564 0164 0264 0364 048d 03a1 0101 007c  .d.d.d.d.......|
+00000bc0: 016a 0664 0564 0164 0664 079c 0264 088d  .j.d.d.d.d...d..
+00000bd0: 0201 007c 016a 07a0 0874 09a0 0a64 09a1  ...|.j...t...d..
+00000be0: 01a1 0101 007c 026a 0b6a 0ca0 0da1 007d  .....|.j.j.....}
+00000bf0: 0374 017c 017c 027c 03a0 03a1 0083 0301  .t.|.|.|........
+00000c00: 0064 0353 0029 0a7a 3e54 6869 7320 7374  .d.S.).z>This st
+00000c10: 6174 6963 206d 6574 686f 6420 6973 2075  atic method is u
+00000c20: 7365 6420 746f 2063 6f6d 706c 6574 6520  sed to complete 
+00000c30: 7468 6520 2a70 6172 616d 732a 2063 6f6e  the *params* con
+00000c40: 7461 696e 6572 2e54 da03 7275 6e4e 2903  tainer.T..runN).
+00000c50: da0f 4e45 575f 4449 525f 5245 5355 4c54  ..NEW_DIR_RESULT
+00000c60: 535a 1373 686f 7274 5f6e 616d 655f 7479  SZ.short_name_ty
+00000c70: 7065 5f72 756e 721b 0000 00da 066f 7574  pe_runr......out
+00000c80: 7075 74da 0029 02da 0b48 4153 5f54 4f5f  put..)...HAS_TO_
+00000c90: 5341 5645 da0d 7375 625f 6469 7265 6374  SAVE..sub_direct
+00000ca0: 6f72 7929 01da 0761 7474 7269 6273 612e  ory)...attribsa.
+00000cb0: 0100 000a 2020 2020 2d20 6060 4841 535f  ....    - ``HAS_
+00000cc0: 544f 5f53 4156 4560 603a 2062 6f6f 6c20  TO_SAVE``: bool 
+00000cd0: 2864 6566 6175 6c74 3a20 5472 7565 2920  (default: True) 
+00000ce0: 4966 2046 616c 7365 2c20 6e6f 7468 696e  If False, nothin
+00000cf0: 6720 6e65 7720 6973 2073 6176 6564 2069  g new is saved i
+00000d00: 6e0a 2020 2020 2020 7468 6520 6469 7265  n.      the dire
+00000d10: 6374 6f72 7920 6f66 2074 6865 2073 696d  ctory of the sim
+00000d20: 756c 6174 696f 6e2e 0a20 2020 202d 2060  ulation..    - `
+00000d30: 6073 7562 5f64 6972 6563 746f 7279 6060  `sub_directory``
+00000d40: 3a20 7374 7220 2864 6566 6175 6c74 3a20  : str (default: 
+00000d50: 2222 2920 4120 6e61 6d65 206f 6620 6120  "") A name of a 
+00000d60: 7375 622d 6469 7265 6374 6f72 7920 2872  sub-directory (r
+00000d70: 656c 6174 6976 650a 2020 2020 2020 746f  elative.      to
+00000d80: 2024 464c 5549 4444 594e 5f50 4154 485f   $FLUIDDYN_PATH_
+00000d90: 5343 5241 5443 4829 2077 6865 7265 696e  SCRATCH) wherein
+00000da0: 2074 6865 2064 6972 6563 746f 7279 206f   the directory o
+00000db0: 6620 7468 6520 7369 6d75 6c61 7469 6f6e  f the simulation
+00000dc0: 0a20 2020 2020 2028 6060 7061 7468 5f72  .      (``path_r
+00000dd0: 756e 6060 2920 6973 2073 6176 6564 2e0a  un``) is saved..
+00000de0: 0a29 0e72 5100 0000 7208 0000 0072 4b00  .).rQ...r....rK.
+00000df0: 0000 da06 7661 6c75 6573 da0c 5f73 6574  ....values.._set
+00000e00: 5f61 7474 7269 6273 7246 0000 0072 3e00  _attribsrF...r>.
+00000e10: 0000 7254 0000 00da 085f 7365 745f 646f  ..rT....._set_do
+00000e20: 63da 0874 6578 7477 7261 70da 0664 6564  c..textwrap..ded
+00000e30: 656e 7472 3d00 0000 7235 0000 00da 0e69  entr=...r5.....i
+00000e40: 6d70 6f72 745f 636c 6173 7365 7329 0472  mport_classes).r
+00000e50: 4100 0000 da06 7061 7261 6d73 7242 0000  A.....paramsrB..
+00000e60: 00da 0c64 6963 745f 636c 6173 7365 7372  ...dict_classesr
+00000e70: 3200 0000 7232 0000 0072 3300 0000 da1d  2...r2...r3.....
+00000e80: 5f63 6f6d 706c 6574 655f 7061 7261 6d73  _complete_params
+00000e90: 5f77 6974 685f 6465 6661 756c 7480 0000  _with_default...
+00000ea0: 0073 2200 0000 0804 0201 0c01 04ff 0405  .s".............
+00000eb0: 0c01 04ff 0403 0a01 06ff 0603 0401 0201  ................
+00000ec0: 02ff 04ff 0c0d 1401 7a24 4f75 7470 7574  ........z$Output
+00000ed0: 2e5f 636f 6d70 6c65 7465 5f70 6172 616d  ._complete_param
+00000ee0: 735f 7769 7468 5f64 6566 6175 6c74 4e63  s_with_defaultNc
+00000ef0: 0300 0000 0000 0000 0000 0000 0b00 0000  ................
+00000f00: 0800 0000 0300 0000 733c 0200 007c 017c  ........s<...|.|
+00000f10: 005f 007a 087c 016a 016a 026a 037c 005f  ._.z.|.j.j.j.|._
+00000f20: 0457 006e 0904 0074 0579 1401 0001 0001  .W.n...t.y......
+00000f30: 0059 006e 0777 0074 067c 006a 0483 017c  .Y.n.w.t.|.j...|
+00000f40: 005f 077c 00a0 08a1 007c 005f 097c 0172  ._.|.....|._.|.r
+00000f50: 2e7c 016a 0a6a 0b7c 005f 0a74 0c83 00a0  .|.j.j.|._.t....
+00000f60: 0d7c 01a1 0101 006e 0f7c 0272 357c 026a  .|.....n.|.r5|.j
+00000f70: 0b7c 005f 0a6e 0864 007c 005f 0a74 0ea0  .|._.n.d.|._.t..
+00000f80: 0f64 01a1 0101 007c 0173 4164 0053 0074  .d.....|.sAd.S.t
+00000f90: 107c 006a 1183 017c 005f 1174 127c 0083  .|.j...|._.t.|..
+00000fa0: 017c 005f 137c 016a 016a 026a 146a 15a0  .|._.|.j.j.j.j..
+00000fb0: 16a1 007d 037c 03a0 17a1 0044 005d 265c  ...}.|.....D.]&\
+00000fc0: 027d 047d 0574 187c 007c 0583 0272 6271  .}.}.t.|.|...rbq
+00000fd0: 5874 197c 0483 017d 067c 006a 0004 006a  Xt.|...}.|.j...j
+00000fe0: 1a64 02a0 1b64 037c 069b 0064 049d 037c  .d...d.|...d...|
+00000ff0: 05a1 0237 0002 005f 1a74 1c7c 007c 067c  ...7..._.t.|.|.|
+00001000: 057c 0083 0183 0301 0071 5874 1d7c 0064  .|.......qXt.|.d
+00001010: 0583 0273 887c 00a0 1ea1 0001 0069 007d  ...s.|.......i.}
+00001020: 077c 006a 1fa0 17a1 0044 005d 255c 027d  .|.j.....D.]%\.}
+00001030: 047d 0574 197c 0483 017d 067c 056a 207c  .}.t.|...}.|.j |
+00001040: 0776 0172 a37c 0467 017c 077c 056a 203c  .v.r.|.g.|.|.j <
+00001050: 006e 087c 077c 056a 2019 00a0 217c 04a1  .n.|.|.j ...!|..
+00001060: 0101 0074 1c7c 006a 137c 067c 057c 0083  ...t.|.j.|.|.|..
+00001070: 0183 0301 0071 8f7c 0772 dc7c 006a 0004  .....q.|.r.|.j..
+00001080: 006a 1a64 0637 0002 005f 1a7c 07a0 17a1  .j.d.7..._.|....
+00001090: 0044 005d 185c 027d 087d 097c 006a 0004  .D.].\.}.}.|.j..
+000010a0: 006a 1a64 077c 0864 0817 0064 099b 0464  .j.d.|.d...d...d
+000010b0: 0aa0 227c 09a1 019b 0064 0b9d 0437 0002  .."|.....d...7..
+000010c0: 005f 1a71 c374 236a 2464 0c6b 0272 e97c  ._.q.t#j$d.k.r.|
+000010d0: 006a 2572 e97c 006a 006a 0a6a 2673 eb64  .j%r.|.j.j.j&s.d
+000010e0: 0053 007c 006a 1164 0d1b 00a0 27a1 0001  .S.|.j.d....'...
+000010f0: 007c 006a 1164 0e1b 00a0 27a1 0001 007c  .|.j.d....'....|
+00001100: 006a 1164 0f1b 00a0 27a1 0001 0074 287c  .j.d....'....t(|
+00001110: 006a 1383 01a0 29a1 0044 005d 147d 0a74  .j....)..D.].}.t
+00001120: 1d7c 0a64 1083 0290 0172 1a7c 0a6a 2aa0  .|.d.....r.|.j*.
+00001130: 2b64 0da1 0190 0172 1a7c 0aa0 2ca1 0001  +d.....r.|..,...
+00001140: 0090 0171 0764 0053 0029 114e 7a45 496e  ...q.d.S.).NzEIn
+00001150: 6974 6961 6c69 7a69 6e67 204f 7574 7075  itializing Outpu
+00001160: 7420 636c 6173 7320 7769 7468 6f75 7420  t class without 
+00001170: 7369 6d20 6f72 2070 6172 616d 7320 6d69  sim or params mi
+00001180: 6768 7420 6c65 6164 2074 6f20 6572 726f  ght lead to erro
+00001190: 7273 2e7a 097b 3a32 3873 7d7b 7d0a 7a0b  rs.z.{:28s}{}.z.
+000011a0: 7369 6d2e 6f75 7470 7574 2e7a 023a 2072  sim.output.z.: r
+000011b0: 4b00 0000 7a0d 696e 7075 745f 6669 6c65  K...z.input_file
+000011c0: 733a 0a7a 0720 202d 2069 6e20 fa01 3a5a  s:.z.  - in ..:Z
+000011d0: 0331 3273 da01 20da 010a 7201 0000 0072  .12s.. ...r....r
+000011e0: 4a00 0000 da01 3072 4900 0000 da0d 6765  J.....0rI.....ge
+000011f0: 6e65 7261 7465 5f66 696c 6529 2dda 0373  nerate_file)-..s
+00001200: 696d da04 696e 666f da06 736f 6c76 6572  im..info..solver
+00001210: da0a 7368 6f72 745f 6e61 6d65 da0b 6e61  ..short_name..na
+00001220: 6d65 5f73 6f6c 7665 72da 0e41 7474 7269  me_solver..Attri
+00001230: 6275 7465 4572 726f 7272 0f00 0000 da07  buteErrorr......
+00001240: 7061 636b 6167 65da 1767 6574 5f70 6174  package..get_pat
+00001250: 685f 736f 6c76 6572 5f70 6163 6b61 6765  h_solver_package
+00001260: 5a13 7061 7468 5f73 6f6c 7665 725f 7061  Z.path_solver_pa
+00001270: 636b 6167 6572 5f00 0000 7254 0000 00da  ckager_...rT....
+00001280: 0573 7570 6572 da08 5f5f 696e 6974 5f5f  .super..__init__
+00001290: 720e 0000 00da 0777 6172 6e69 6e67 7203  r......warningr.
+000012a0: 0000 0072 2c00 0000 720c 0000 00da 0b69  ...r,...r......i
+000012b0: 6e70 7574 5f66 696c 6573 723d 0000 0072  nput_filesr=...r
+000012c0: 3500 0000 725e 0000 00da 0569 7465 6d73  5...r^.....items
+000012d0: 7214 0000 0072 0400 0000 da11 5f6f 626a  r....r......_obj
+000012e0: 6563 7473 5f74 6f5f 7072 696e 74da 0666  ects_to_print..f
+000012f0: 6f72 6d61 74da 0773 6574 6174 7472 da07  ormat..setattr..
+00001300: 6861 7361 7474 7272 5100 0000 724b 0000  hasattrrQ...rK..
+00001310: 00da 0864 6972 5f6e 616d 65da 0661 7070  ...dir_name..app
+00001320: 656e 64da 046a 6f69 6e72 0600 0000 da04  end..joinr......
+00001330: 7261 6e6b da0c 5f68 6173 5f74 6f5f 7361  rank.._has_to_sa
+00001340: 7665 7253 0000 0072 2300 0000 da04 7661  verS...r#.....va
+00001350: 7273 7259 0000 00da 0872 656c 5f70 6174  rsrY.....rel_pat
+00001360: 6872 1800 0000 7266 0000 0029 0bda 0473  hr....rf...)...s
+00001370: 656c 6672 6700 0000 725f 0000 0072 6000  elfrg...r_...r`.
+00001380: 0000 da08 636c 735f 6e61 6d65 da05 436c  ....cls_name..Cl
+00001390: 6173 73da 086f 626a 5f6e 616d 655a 1366  ass..obj_nameZ.f
+000013a0: 6f72 5f73 7472 5f69 6e70 7574 5f66 696c  or_str_input_fil
+000013b0: 6573 7278 0000 0072 7200 0000 da0e 6669  esrx...rr.....fi
+000013c0: 6c65 5f67 656e 6572 6174 6f72 a901 da09  le_generator....
+000013d0: 5f5f 636c 6173 735f 5f72 3200 0000 7233  __class__r2...r3
+000013e0: 0000 0072 7000 0000 a000 0000 7380 0000  ...rp.......s...
+000013f0: 0006 0102 0110 010c 0104 0102 ff0c 030a  ................
+00001400: 0204 020a 020e 0104 010a 0206 0204 0102  ................
+00001410: 0104 ff04 0404 010c 020a 0210 0210 010a  ................
+00001420: 0102 0108 010c 010c 0108 ff12 030a 0208  ................
+00001430: 0104 0112 0108 010a 020e 0110 0214 0104  ................
+00001440: 0210 0110 0108 011a 0108 ff08 0502 ff04  ................
+00001450: 0202 fe08 0302 fd04 050e 020e 010e 0112  ................
+00001460: 0202 0104 0106 ff0a 0204 fe08 0304 8004  ................
+00001470: fc7a 0f4f 7574 7075 742e 5f5f 696e 6974  .z.Output.__init
+00001480: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
+00001490: 0000 0004 0000 0043 0000 0073 1200 0000  .......C...s....
+000014a0: 7400 7401 a002 7c00 a101 6a03 8301 6a04  t.t...|...j...j.
+000014b0: 5300 2901 7a28 4765 7420 7468 6520 7061  S.).z(Get the pa
+000014c0: 7468 2074 6f77 6172 6473 2074 6865 2073  th towards the s
+000014d0: 6f6c 7665 7220 7061 636b 6167 652e 2905  olver package.).
+000014e0: 7203 0000 00da 0769 6e73 7065 6374 da09  r......inspect..
+000014f0: 6765 746d 6f64 756c 65da 085f 5f66 696c  getmodule..__fil
+00001500: 655f 5f72 2200 0000 2901 7241 0000 0072  e__r"...).rA...r
+00001510: 3200 0000 7232 0000 0072 3300 0000 726e  2...r2...r3...rn
+00001520: 0000 00ed 0000 0073 0200 0000 1203 7a1e  .......s......z.
+00001530: 4f75 7470 7574 2e67 6574 5f70 6174 685f  Output.get_path_
+00001540: 736f 6c76 6572 5f70 6163 6b61 6765 6301  solver_packagec.
+00001550: 0000 0000 0000 0000 0000 0004 0000 0008  ................
+00001560: 0000 0003 0000 0073 d800 0000 7400 6a01  .......s....t.j.
+00001570: 6401 6b02 720d 7402 6402 7c00 6a03 9b00  d.k.r.t.d.|.j...
+00001580: 9d02 8301 0100 7404 8300 8f0d 0100 7405  ......t.......t.
+00001590: 8300 a006 a100 0100 5700 6403 0400 0400  ........W.d.....
+000015a0: 8303 0100 6e08 3100 7320 7701 0100 0100  ....n.1.s w.....
+000015b0: 0100 5900 0100 7407 a008 7c00 6a09 6a0a  ..Y...t...|.j.j.
+000015c0: a101 0100 7400 6a01 6401 6b02 7239 7c00  ....t.j.d.k.r9|.
+000015d0: 6a0b 7239 7c00 6a09 6a0c 6a0d 733b 6403  j.r9|.j.j.j.s;d.
+000015e0: 5300 740e 7c00 6a09 6a0c 6a0f 7c00 6a03  S.t.|.j.j.j.|.j.
+000015f0: 8302 0100 7c00 a010 a100 0100 7c00 6a03  ....|.......|.j.
+00001600: 6404 1b00 7d01 7c01 6a11 6405 6406 8d01  d...}.|.j.d.d...
+00001610: 0100 6407 4400 5d14 7d02 7c01 7c02 1b00  ..d.D.].}.|.|...
+00001620: 7d03 7c03 a012 a100 7260 7155 7413 a014  }.|.....r`qUt...
+00001630: 7c00 6a03 7c02 1b00 7c03 a102 0100 7155  |.j.|...|.....qU
+00001640: 6403 5300 2908 7a21 4c6f 6773 2069 6e66  d.S.).z!Logs inf
+00001650: 6f20 6f6e 2069 6e73 7461 6e74 6961 7465  o on instantiate
+00001660: 6420 636c 6173 7365 7372 0100 0000 7a0a  d classesr....z.
+00001670: 7061 7468 5f72 756e 3a20 4e7a 0e2e 6461  path_run: Nz..da
+00001680: 7461 5f66 6c75 6964 7369 6d54 7212 0000  ta_fluidsimTr...
+00001690: 0029 027a 0f69 6e66 6f5f 736f 6c76 6572  .).z.info_solver
+000016a0: 2e78 6d6c 7a10 7061 7261 6d73 5f73 696d  .xmlz.params_sim
+000016b0: 756c 2e78 6d6c 2915 7206 0000 0072 7b00  ul.xml).r....r{.
+000016c0: 0000 da05 7072 696e 7472 2c00 0000 7205  ....printr,...r.
+000016d0: 0000 0072 6f00 0000 da09 706f 7374 5f69  ...ro.....post_i
+000016e0: 6e69 7472 0e00 0000 7268 0000 0072 6700  nitr....rh...rg.
+000016f0: 0000 7274 0000 0072 7c00 0000 725f 0000  ..rt...r|...r_..
+00001700: 0072 5300 0000 7234 0000 0072 1b00 0000  .rS...r4...r....
+00001710: da29 5f70 6f73 745f 696e 6974 5f63 7265  .)_post_init_cre
+00001720: 6174 655f 6164 6469 7469 6f6e 616c 5f73  ate_additional_s
+00001730: 6f75 7263 655f 6669 6c65 7372 2300 0000  ource_filesr#...
+00001740: 722b 0000 0072 2500 0000 7226 0000 0029  r+...r%...r&...)
+00001750: 0472 7f00 0000 5a12 7061 7468 5f69 6e66  .r....Z.path_inf
+00001760: 6f5f 666c 7569 6473 696d 7250 0000 005a  o_fluidsimrP...Z
+00001770: 0870 6174 685f 6e65 7772 8400 0000 7232  .path_newr....r2
+00001780: 0000 0072 3300 0000 728a 0000 00f2 0000  ...r3...r.......
+00001790: 0073 2e00 0000 0a03 1001 0803 0c01 1cff  .s..............
+000017a0: 0e03 0804 02ff 0402 02fe 0803 02fd 0405  ................
+000017b0: 1202 0801 0a03 0c01 0801 0801 0801 0201  ................
+000017c0: 1401 04fc 7a10 4f75 7470 7574 2e70 6f73  ....z.Output.pos
+000017d0: 745f 696e 6974 6301 0000 0000 0000 0000  t_initc.........
+000017e0: 0000 0006 0000 0004 0000 0043 0000 0073  ...........C...s
+000017f0: ae00 0000 7c00 6a00 6a01 6401 1b00 7d01  ....|.j.j.d...}.
+00001800: 7c01 a002 a100 7313 7403 6402 7c00 6a00  |.....s.t.d.|.j.
+00001810: 6a01 9b00 9d02 8301 8201 7404 a005 7c01  j.........t...|.
+00001820: 7c00 6a06 a102 0100 7407 7c00 6a00 8301  |.j.....t.|.j...
+00001830: a008 a100 4400 5d11 7d02 7409 7c02 6403  ....D.].}.t.|.d.
+00001840: 8302 7232 7c02 6a0a a00b 6404 a101 7332  ..r2|.j...d...s2
+00001850: 7c02 a00c a100 0100 7121 7409 7c00 6405  |.......q!t.|.d.
+00001860: 8302 7253 7c00 6a0d a00e a100 4400 5d17  ..rS|.j.....D.].
+00001870: 5c02 7d03 7d04 7c00 6a06 7c03 1b00 7d05  \.}.}.|.j.|...}.
+00001880: 7c05 6a0f 6a10 6406 6407 8d01 0100 7c05  |.j.j.d.d.....|.
+00001890: a011 7c04 a101 0100 713d 6408 5300 6408  ..|.....q=d.S.d.
+000018a0: 5300 2909 7a24 4372 6561 7465 2074 6865  S.).z$Create the
+000018b0: 2066 696c 6573 2066 726f 6d20 7468 6569   files from thei
+000018c0: 7220 7465 6d70 6c61 7465 7a08 7461 736b  r templatez.task
+000018d0: 732e 7079 7a29 7461 736b 732e 7079 206d  s.pyz)tasks.py m
+000018e0: 6973 7369 6e67 2069 6e20 736f 6c76 6572  issing in solver
+000018f0: 2074 656d 706c 6174 6573 5f64 6972 2072   templates_dir r
+00001900: 6600 0000 724a 0000 00da 1169 6e74 6572  f...rJ.....inter
+00001910: 6e61 6c5f 7379 6d6c 696e 6b73 5472 1200  nal_symlinksTr..
+00001920: 0000 4e29 1272 7200 0000 5a0d 7465 6d70  ..N).rr...Z.temp
+00001930: 6c61 7465 735f 6469 7272 2b00 0000 da0c  lates_dirr+.....
+00001940: 5275 6e74 696d 6545 7272 6f72 7225 0000  RuntimeErrorr%..
+00001950: 0072 2600 0000 722c 0000 0072 7d00 0000  .r&...r,...r}...
+00001960: 7259 0000 0072 7700 0000 727e 0000 0072  rY...rw...r~...r
+00001970: 1800 0000 7266 0000 0072 8c00 0000 7273  ....rf...r....rs
+00001980: 0000 0072 2200 0000 7223 0000 00da 0a73  ...r"...r#.....s
+00001990: 796d 6c69 6e6b 5f74 6f29 0672 7f00 0000  ymlink_to).r....
+000019a0: 5a0d 7061 7468 5f74 6173 6b73 5f70 7972  Z.path_tasks_pyr
+000019b0: 8300 0000 722e 0000 00da 0674 6172 6765  ....r......targe
+000019c0: 745a 0c70 6174 685f 7379 6d6c 696e 6b72  tZ.path_symlinkr
+000019d0: 3200 0000 7232 0000 0072 3300 0000 728b  2...r2...r3...r.
+000019e0: 0000 0012 0100 0073 2e00 0000 0c02 0801  .......s........
+000019f0: 0201 0201 0601 04ff 04ff 0e04 1202 0201  ................
+00001a00: 0401 04ff 0a02 02fe 0804 0280 0a02 1201  ................
+00001a10: 0a01 0e01 0c01 04fc 0401 7a30 4f75 7470  ..........z0Outp
+00001a20: 7574 2e5f 706f 7374 5f69 6e69 745f 6372  ut._post_init_cr
+00001a30: 6561 7465 5f61 6464 6974 696f 6e61 6c5f  eate_additional_
+00001a40: 736f 7572 6365 5f66 696c 6573 6302 0000  source_filesc...
+00001a50: 0000 0000 0000 0000 0003 0000 0008 0000  ................
+00001a60: 0043 0000 0073 2800 0000 6401 6401 6401  .C...s(...d.d.d.
+00001a70: 6402 6402 6402 6403 6404 9c07 7d02 7c01  d.d.d.d.d...}.|.
+00001a80: 6a00 6405 7c02 6406 6407 8d03 0100 6400  j.d.|.d.d.....d.
+00001a90: 5300 2908 4ee9 2800 0000 6700 0000 0000  S.).N.(...g.....
+00001aa0: 00f0 3fe9 0100 0000 2907 da02 6e78 da02  ..?.....)...nx..
+00001ab0: 6e79 da02 6e7a da02 6c78 da02 6c79 da02  ny..nz..lx..ly..
+00001ac0: 6c7a da05 7363 616c 655a 0f62 6c6f 636b  lz..scaleZ.block
+00001ad0: 5f6d 6573 685f 6469 6374 da04 544f 444f  _mesh_dict..TODO
+00001ae0: 2902 7258 0000 00da 0364 6f63 2901 723e  ).rX.....doc).r>
+00001af0: 0000 0029 0372 4100 0000 725f 0000 00da  ...).rA...r_....
+00001b00: 0764 6566 6175 6c74 7232 0000 0072 3200  .defaultr2...r2.
+00001b10: 0000 7233 0000 00da 205f 636f 6d70 6c65  ..r3.... _comple
+00001b20: 7465 5f70 6172 616d 735f 626c 6f63 6b5f  te_params_block_
+00001b30: 6d65 7368 5f64 6963 7429 0100 0073 1a00  mesh_dict)...s..
+00001b40: 0000 0203 0201 0201 0201 0201 0201 0201  ................
+00001b50: 06f9 040a 0201 0201 0201 0afd 7a27 4f75  ............z'Ou
+00001b60: 7470 7574 2e5f 636f 6d70 6c65 7465 5f70  tput._complete_p
+00001b70: 6172 616d 735f 626c 6f63 6b5f 6d65 7368  arams_block_mesh
+00001b80: 5f64 6963 7463 0300 0000 0000 0000 0000  _dictc..........
+00001b90: 0000 0300 0000 0100 0000 4300 0000 7304  ..........C...s.
+00001ba0: 0000 0069 0053 0029 014e 7232 0000 0029  ...i.S.).Nr2...)
+00001bb0: 0372 7f00 0000 5a04 746d 696e 5a04 746d  .r....Z.tminZ.tm
+00001bc0: 6178 7232 0000 0072 3200 0000 7233 0000  axr2...r2...r3..
+00001bd0: 00da 145f 636f 6d70 7574 655f 6d65 616e  ..._compute_mean
+00001be0: 5f76 616c 7565 733b 0100 0073 0200 0000  _values;...s....
+00001bf0: 0401 7a1b 4f75 7470 7574 2e5f 636f 6d70  ..z.Output._comp
+00001c00: 7574 655f 6d65 616e 5f76 616c 7565 7329  ute_mean_values)
+00001c10: 024e 4e29 18da 085f 5f6e 616d 655f 5fda  .NN)...__name__.
+00001c20: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00001c30: 7561 6c6e 616d 655f 5f72 4c00 0000 724e  ualname__rL...rN
+00001c40: 0000 0072 4f00 0000 7209 0000 00da 1d5f  ...rO...r......_
+00001c50: 6865 6c70 6572 5f74 7572 6275 6c65 6e63  helper_turbulenc
+00001c60: 655f 7072 6f70 6572 7469 6573 720b 0000  e_propertiesr...
+00001c70: 00da 1a5f 6865 6c70 6572 5f64 6563 6f6d  ..._helper_decom
+00001c80: 706f 7365 5f70 6172 5f64 6963 7472 0a00  pose_par_dictr..
+00001c90: 0000 da14 5f68 656c 7065 725f 636f 6e74  ...._helper_cont
+00001ca0: 726f 6c5f 6469 6374 da0b 636c 6173 736d  rol_dict..classm
+00001cb0: 6574 686f 6472 4300 0000 723f 0000 0072  ethodrC...r?...r
+00001cc0: 5100 0000 7261 0000 0072 7000 0000 726e  Q...ra...rp...rn
+00001cd0: 0000 0072 8a00 0000 728b 0000 0072 9c00  ...r....r....r..
+00001ce0: 0000 729d 0000 00da 0d5f 5f63 6c61 7373  ..r......__class
+00001cf0: 6365 6c6c 5f5f 7232 0000 0072 3200 0000  cell__r2...r2...
+00001d00: 7284 0000 0072 3300 0000 7235 0000 0044  r....r3...r5...D
+00001d10: 0000 0073 3200 0000 0800 0801 0801 0801  ...s2...........
+00001d20: 0207 0801 04ff 0603 0601 0202 0a01 020a  ................
+00001d30: 0a01 0212 0a01 020d 0a01 0e1f 024d 0a01  .............M..
+00001d40: 0c04 0820 0217 0a01 1011 7235 0000 0029  ... ......r5...)
+00001d50: 22da 075f 5f64 6f63 5f5f 5a13 696d 706f  "..__doc__Z.impo
+00001d60: 7274 6c69 622e 7265 736f 7572 6365 7372  rtlib.resourcesr
+00001d70: 1a00 0000 7286 0000 0072 1e00 0000 7225  ....r....r....r%
+00001d80: 0000 0072 5c00 0000 da0a 636f 6e74 6578  ...r\.....contex
+00001d90: 746c 6962 7202 0000 00da 0770 6174 686c  tlibr......pathl
+00001da0: 6962 7203 0000 00da 0a69 6e66 6c65 6374  ibr......inflect
+00001db0: 696f 6e72 0400 0000 5a0b 666c 7569 6464  ionr....Z.fluidd
+00001dc0: 796e 2e69 6f72 0500 0000 5a0d 666c 7569  yn.ior....Z.flui
+00001dd0: 6464 796e 2e75 7469 6c72 0600 0000 5a14  ddyn.utilr....Z.
+00001de0: 666c 7569 6473 696d 5f63 6f72 652e 6f75  fluidsim_core.ou
+00001df0: 7470 7574 7207 0000 00da 1466 6c75 6964  tputr......fluid
+00001e00: 7369 6d5f 636f 7265 2e70 6172 616d 7372  sim_core.paramsr
+00001e10: 0800 0000 da1d 666c 7569 6473 696d 666f  ......fluidsimfo
+00001e20: 616d 2e66 6f61 6d5f 696e 7075 745f 6669  am.foam_input_fi
+00001e30: 6c65 7372 0900 0000 720a 0000 0072 0b00  lesr....r....r..
+00001e40: 0000 5a28 666c 7569 6473 696d 666f 616d  ..Z(fluidsimfoam
+00001e50: 2e66 6f61 6d5f 696e 7075 745f 6669 6c65  .foam_input_file
+00001e60: 732e 6765 6e65 7261 746f 7273 720c 0000  s.generatorsr...
+00001e70: 0072 0d00 0000 5a10 666c 7569 6473 696d  .r....Z.fluidsim
+00001e80: 666f 616d 2e6c 6f67 720e 0000 00da 1466  foam.logr......f
+00001e90: 6c75 6964 7369 6d66 6f61 6d2e 736f 6c76  luidsimfoam.solv
+00001ea0: 6572 7372 0f00 0000 7234 0000 0072 3500  ersr....r4...r5.
+00001eb0: 0000 7232 0000 0072 3200 0000 7232 0000  ..r2...r2...r2..
+00001ec0: 0072 3300 0000 da08 3c6d 6f64 756c 653e  .r3.....<module>
+00001ed0: 0100 0000 7326 0000 0004 0008 0208 0108  ....s&..........
+00001ee0: 0108 0108 010c 010c 010c 020c 020c 010c  ................
+00001ef0: 010c 0114 0110 050c 040c 0108 0314 26    ..............&
```

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/output/__pycache__/dataframe_from_paths.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/output/__pycache__/dataframe_from_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/output/__pycache__/log.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/output/__pycache__/log.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/output/base.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/output/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,15 @@
             multiplexed_path = importlib.resources.files(package_name)
             resource = multiplexed_path.joinpath(relative_path)
             context_manager = importlib.resources.as_file
         else:
             resource = Path(os.path.expandvars(resource)).expanduser()
             context_manager = nullcontext
 
+        destination.parent.mkdir(exist_ok=True)
         with context_manager(resource) as resource:
             if resource.is_file():
                 shutil.copy(resource, destination)
             elif resource.is_dir():
                 shutil.copytree(resource, destination / resource.name)
             else:
                 raise NotImplementedError(
@@ -274,23 +275,29 @@
         """Create the files from their template"""
         path_tasks_py = self.input_files.templates_dir / "tasks.py"
         if not path_tasks_py.exists():
             raise RuntimeError(
                 "tasks.py missing in solver templates_dir "
                 f"{self.input_files.templates_dir}"
             )
-        shutil.copy(path_tasks_py, self.sim.path_run)
+        shutil.copy(path_tasks_py, self.path_run)
 
         for file_generator in vars(self.input_files).values():
             if hasattr(
                 file_generator, "generate_file"
             ) and not file_generator.rel_path.startswith("system"):
                 # system files are already generated
                 file_generator.generate_file()
 
+        if hasattr(self, "internal_symlinks"):
+            for relative_path, target in self.internal_symlinks.items():
+                path_symlink = self.path_run / relative_path
+                path_symlink.parent.mkdir(exist_ok=True)
+                path_symlink.symlink_to(target)
+
     @classmethod
     def _complete_params_block_mesh_dict(cls, params):
         default = {
             "nx": 40,
             "ny": 40,
             "nz": 40,
             "lx": 1.0,
```

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/output/dataframe_from_paths.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/output/dataframe_from_paths.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/output/log.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/output/log.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/params.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/params.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/resources/LICENSE.template` & `fluidsimfoam-0.0.7/src/fluidsimfoam/resources/LICENSE.template`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/resources/__init__.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/resources/__init__.py.template` & `fluidsimfoam-0.0.7/src/fluidsimfoam/resources/__init__.py.template`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/resources/__pycache__/__init__.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/resources/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/resources/test_generated_solver.py.template` & `fluidsimfoam-0.0.7/src/fluidsimfoam/resources/test_generated_solver.py.template`

 * *Files 2% similar despite different names*

```diff
@@ -14,11 +14,11 @@
     check_saved_case(here / "saved_cases/case0", sim.path_run)
 
 
 # @skipif_executable_not_available("interFoam")
 # def test_run():
 #     params = Simul.create_default_params()
 #     params.output.sub_directory = "tests_fluidsimfoam/$name_short"
-#     # change parameters to get a very short and small simulations
+#     # change parameters to get a very short and small simulation
 #     ...
 #     sim = Simul(params)
 #     sim.make.exec("run")
```

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/solvers/__init__.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/solvers/__pycache__/base.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/solvers/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/solvers/base.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/solvers/base.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/tasks.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/invoke/tasks.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,86 +1,118 @@
-"""Invoke tasks to be used from the ``tasks.py`` file in the solvers"""
+"""Invoke tasks to be used from the ``tasks.py`` file in the solvers
+
+.. autodata:: clean
+.. autodata:: block_mesh
+.. autodata:: surface_feature_extract
+.. autodata:: snappy_hex_mesh
+.. autodata:: polymesh
+.. autodata:: set_fields
+.. autodata:: decompose_par
+.. autodata:: run
+
+"""
 
 import re
 from pathlib import Path
 from subprocess import Popen
 from time import sleep, time
 
+import invoke.context
 from invoke import task
+from invoke.exceptions import Exit
 
-from fluiddyn.util import time_as_str
 from fluidsimfoam.foam_input_files import parse
 
+from .context import Context
+
+invoke.tasks.Context = Context
+
 
 @task
 def clean(context):
+    """clean with foamCleanTutorials"""
     context.run("foamCleanTutorials", warn=True)
+    for path in Path(".").glob(".data_fluidsim/*_called*"):
+        path.unlink()
 
 
 @task
 def block_mesh(context):
-    if (
-        Path("system/blockMeshDict").exists()
-        and not Path("constant/polyMesh").is_dir()
-    ):
-        context.run("blockMesh")
+    """Run ``blockMesh``"""
+    context.run_appl_once("blockMesh")
+
+
+@task
+def surface_feature_extract(context):
+    """Run ``surfaceFeatureExtract``"""
+    context.run_appl_once("surfaceFeatureExtract")
+
 
+PATH_DECOMPOSE_PAR_DICT_MESH = None
 
-@task(block_mesh)
+
+@task
+def snappy_hex_mesh(context):
+    """Run ``snappyHexMesh -overwrite``"""
+    context.run_appl_once(
+        "snappyHexMesh -overwrite",
+        parallel_if_needed=True,
+        path_decompose_par_dict=PATH_DECOMPOSE_PAR_DICT_MESH,
+    )
+
+
+@task(pre=[block_mesh, surface_feature_extract, snappy_hex_mesh])
 def polymesh(context):
     """Create the polymesh directory"""
 
 
 @task
 def set_fields(context, force=False):
-    if Path("system/setFieldsDict").exists():
-        path_setFields_called = Path(".data_fluidsim/setFields_called")
-        path_setFields_called.parent.mkdir(exist_ok=True)
-        if force or not path_setFields_called.exists():
-            path_setFields_called.touch()
-            context.run("setFields")
+    """Run ``setFields``"""
+    context.run_appl_once("setFields")
+
+
+@task
+def decompose_par(context):
+    """Run ``decomposePar``"""
+    context.run_appl_once("decomposePar")
 
 
-@task(polymesh, set_fields)
+@task(pre=[polymesh, set_fields, decompose_par])
 def run(context):
     """Main target to launch a simulation"""
     with open("system/controlDict") as file:
         ctr_dict = file.read()
     ctr_dict = parse(ctr_dict)
 
     application = ctr_dict.children["application"]
     end_time = ctr_dict["endTime"]
     start_time = ctr_dict["startTime"]
 
     path_run = Path.cwd()
 
-    path_decompose_par_dict = path_run / "system/decomposeParDict"
-    parallel = path_decompose_par_dict.exists()
-    if parallel:
-        context.run("decomposePar")
-        nsubdoms = None
-        with open(path_decompose_par_dict) as file:
-            for line in file:
-                if "numberOfSubdomains" in line:
-                    line = line.strip().removesuffix(";")
-                    nsubdoms = int(line.split()[-1])
-                    break
-        if nsubdoms is None:
-            raise RuntimeError(f"Bad decomposeParDict {path_decompose_par_dict}")
-        command = ["mpirun", "-np", str(nsubdoms), application, "-parallel"]
+    if context.parallel:
+        # Options '-n' and '-np' are synonymous, but msmpi only supports '-n'
+        command = [
+            context.mpi_command,
+            "-n",
+            str(context.nsubdoms),
+            application,
+            "-parallel",
+        ]
     else:
         command = application
 
-    path_log = path_run / f"log_{time_as_str()}.txt"
+    path_log = path_run / f"log_{context.time_as_str}.txt"
     print(f"Starting simulation in \n{path_run}")
     with open(path_log, "w") as file_log:
         file_log.write(f"{start_time = }\n{end_time = }\n")
         file_log.flush()
         print(f"{end_time = }")
-        pattern_time = re.compile(r"\nTime = ([\d]+\.[\d]+)")
+        pattern_time = re.compile(r"\nTime = ([\d]+\.?[\d]+)")
         t_start = time()
         process = Popen(command, stdout=file_log)
         t_last = time() - 10.0
         while process.poll() is None:
             sleep(0.2)
             t_now = time()
             if t_now - t_last > 2:
@@ -96,7 +128,9 @@
                         print(
                             f"eq_time: {time_simul:12.3f} "
                             f"({100 * time_simul/end_time:6.2f} %), "
                             f"clock_time: {t_now - t_start: 12.3f} s"
                         )
 
     print(f"Simulation done. path_run:\n{path_run}")
+    if process.returncode:
+        raise Exit(process.returncode)
```

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/testing.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/testing.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/util/__pycache__/console.cpython-310.pyc` & `fluidsimfoam-0.0.7/src/fluidsimfoam/util/__pycache__/console.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  2 09:35:05 2023 UTC, .py size: 6906 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,342 +1,411 @@
-00000000: 6f0d 0d0a 0000 0000 c9b7 7964 fa1a 0000  o.........yd....
+00000000: 6f0d 0d0a 0000 0000 d751 9064 f021 0000  o........Q.d.!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 c800 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 6401 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6401 6406 6c0b 6d0b 5a0b  m.Z...d.d.l.m.Z.
-00000080: 0100 6401 6407 6c0c 6d0d 5a0d 0100 6401  ..d.d.l.m.Z...d.
-00000090: 6408 6c0e 6d0f 5a0f 0100 6401 6409 6c10  d.l.m.Z...d.d.l.
-000000a0: 6d11 5a11 0100 6401 640a 6c12 6d13 5a14  m.Z...d.d.l.m.Z.
-000000b0: 0100 6401 640b 6c15 6d16 5a16 0100 6401  ..d.d.l.m.Z...d.
-000000c0: 640c 6c17 6d18 5a19 0100 6401 640d 6c1a  d.l.m.Z...d.d.l.
-000000d0: 6d1b 5a1b 0100 640e 640f 8400 5a1c 6506  m.Z...d.d...Z.e.
-000000e0: 6514 6410 6411 8d02 5a13 6412 6413 8400  e.d.d...Z.d.d...
-000000f0: 5a1d 6402 5300 2914 7a1a 436f 6e73 6f6c  Z.d.S.).z.Consol
-00000100: 6520 7363 7269 7074 2066 756e 6374 696f  e script functio
-00000110: 6e73 0a0a e900 0000 004e 2901 da07 7061  ns.......N)...pa
-00000120: 7274 6961 6c29 01da 0972 6573 6f75 7263  rtial)...resourc
-00000130: 6573 2901 da04 5061 7468 2901 da06 7070  es)...Path)...pp
-00000140: 7269 6e74 2901 da04 636f 7079 2901 da08  rint)...copy)...
-00000150: 5465 6d70 6c61 7465 2901 da08 6361 6d65  Template)...came
-00000160: 6c69 7a65 2901 da16 7374 6172 745f 6970  lize)...start_ip
-00000170: 7974 686f 6e5f 6c6f 6164 5f73 696d 2901  ython_load_sim).
-00000180: da10 7061 7468 5f64 6972 5f72 6573 756c  ..path_dir_resul
-00000190: 7473 2901 da0b 5f5f 7665 7273 696f 6e5f  ts)...__version_
-000001a0: 5f29 01da 1161 7661 696c 6162 6c65 5f73  _)...available_s
-000001b0: 6f6c 7665 7273 6300 0000 0000 0000 0000  olversc.........
-000001c0: 0000 0009 0000 0005 0000 0043 0000 0073  ...........C...s
-000001d0: 9a00 0000 6401 6400 6c00 7d00 6401 6400  ....d.d.l.}.d.d.
-000001e0: 6c01 7d01 6401 6400 6c02 7d02 6402 6403  l.}.d.d.l.}.d.d.
-000001f0: 6404 9c02 7d03 7c02 7c00 7c01 6703 7d04  d...}.|.|.|.g.}.
-00000200: 7c04 4400 5d08 7d05 7c05 6a03 7c03 7c05  |.D.].}.|.j.|.|.
-00000210: 6a04 3c00 7118 7c03 a005 a100 4400 5d10  j.<.q.|.....D.].
-00000220: 5c02 7d06 7d07 7406 7c06 a007 6405 a101  \.}.}.t.|...d...
-00000230: 9b00 6406 7c07 9b00 9d03 8301 0100 7125  ..d.|.........q%
-00000240: 7408 7409 6407 6408 8400 740a 8300 4400  t.t.d.d...t...D.
-00000250: 8301 8301 8301 7d08 7406 6409 640a a00b  ......}.t.d.d...
-00000260: 7c08 a101 1700 8301 0100 6400 5300 290b  |.........d.S.).
-00000270: 4e72 0100 0000 da07 5665 7273 696f 6efa  Nr......Version.
-00000280: 072d 2d2d 2d2d 2d2d 2902 5a07 5061 636b  .-------).Z.Pack
-00000290: 6167 6572 0e00 0000 e90f 0000 00fa 0120  ager........... 
-000002a0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000002b0: 0003 0000 0053 0000 00f3 1200 0000 6700  .....S........g.
-000002c0: 7c00 5d05 7d01 7c01 6a00 9102 7102 5300  |.].}.|.j...q.S.
-000002d0: a900 a901 da04 6e61 6d65 2902 da02 2e30  ......name)....0
-000002e0: 5a0b 656e 7472 795f 706f 696e 7472 1200  Z.entry_pointr..
-000002f0: 0000 7212 0000 00fa 3e2f 686f 6d65 2f70  ..r.....>/home/p
-00000300: 6965 7272 652f 4465 762f 666c 7569 6473  ierre/Dev/fluids
-00000310: 696d 666f 616d 2f73 7263 2f66 6c75 6964  imfoam/src/fluid
-00000320: 7369 6d66 6f61 6d2f 7574 696c 2f63 6f6e  simfoam/util/con
-00000330: 736f 6c65 2e70 79da 0a3c 6c69 7374 636f  sole.py..<listco
-00000340: 6d70 3e28 0000 00f3 0200 0000 1200 7a22  mp>(..........z"
-00000350: 7072 696e 745f 7665 7273 696f 6e73 2e3c  print_versions.<
-00000360: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00000370: 703e 7a14 0a49 6e73 7461 6c6c 6564 2073  p>z..Installed s
-00000380: 6f6c 7665 7273 3a20 7a02 2c20 290c da08  olvers: z., )...
-00000390: 666c 7569 6464 796e da0d 666c 7569 6473  fluiddyn..fluids
-000003a0: 696d 5f63 6f72 65da 0c66 6c75 6964 7369  im_core..fluidsi
-000003b0: 6d66 6f61 6d72 0b00 0000 da08 5f5f 6e61  mfoamr......__na
-000003c0: 6d65 5f5f da05 6974 656d 73da 0570 7269  me__..items..pri
-000003d0: 6e74 da05 6c6a 7573 74da 0673 6f72 7465  nt..ljust..sorte
-000003e0: 64da 0373 6574 720c 0000 00da 046a 6f69  d..setr......joi
-000003f0: 6e29 0972 1900 0000 721a 0000 0072 1b00  n).r....r....r..
-00000400: 0000 5a08 7665 7273 696f 6e73 5a08 7061  ..Z.versionsZ.pa
-00000410: 636b 6167 6573 da07 7061 636b 6167 655a  ckages..packageZ
-00000420: 0870 6b67 5f6e 616d 65da 0776 6572 7369  .pkg_name..versi
-00000430: 6f6e da05 6e61 6d65 7372 1200 0000 7212  on..namesr....r.
-00000440: 0000 0072 1600 0000 da0e 7072 696e 745f  ...r......print_
-00000450: 7665 7273 696f 6e73 1a00 0000 7316 0000  versions....s...
-00000460: 0008 0108 0108 010a 020a 0208 010e 0110  ................
-00000470: 021a 0118 0216 0172 2600 0000 7a1d 6672  .......r&...z.fr
-00000480: 6f6d 2066 6c75 6964 7369 6d66 6f61 6d20  om fluidsimfoam 
-00000490: 696d 706f 7274 206c 6f61 6429 015a 0b6c  import load).Z.l
-000004a0: 6f61 645f 696d 706f 7274 6300 0000 0000  oad_importc.....
-000004b0: 0000 0000 0000 001e 0000 000c 0000 0003  ................
-000004c0: 0000 0073 b404 0000 6401 6402 6c00 6d01  ...s....d.d.l.m.
-000004d0: 7d00 6d02 7d01 0100 7403 6a04 6403 6404  }.m.}...t.j.d.d.
-000004e0: 6405 8d02 7d02 7c02 a005 6406 a101 0100  d...}.|...d.....
-000004f0: 7c02 a005 6407 6408 a102 0100 7c02 a005  |...d.d.....|...
-00000500: 6409 640a a102 0100 7c02 6a05 640b 640c  d.d.....|.j.d.d.
-00000510: 640d 640e 8d03 0100 7c02 a005 640f 6410  d.d.....|...d.d.
-00000520: a102 0100 7c02 a006 a100 7d03 7407 7c03  ....|.....}.t.|.
-00000530: 8301 0100 7c03 6a08 6400 7500 7249 7c03  ....|.j.d.u.rI|.
-00000540: 6a09 6400 7500 7249 7407 6411 8301 0100  j.d.u.rIt.d.....
-00000550: 740a a00b 6412 a101 0100 7c03 6a09 6400  t...d.....|.j.d.
-00000560: 7501 7252 740c 6413 8301 8201 7c03 6a08  u.rRt.d.....|.j.
-00000570: 6400 7501 726c 740d 7c03 6a08 8301 8900  d.u.rlt.|.j.....
-00000580: 8800 a00e a100 736c 7407 8800 9b00 6414  ......slt.....d.
-00000590: 9d02 8301 0100 740a a00b 6412 a101 0100  ......t...d.....
-000005a0: 7c03 6a0f 6400 7501 7279 740d 7c03 6a0f  |.j.d.u.ryt.|.j.
-000005b0: 8301 a010 a100 7d04 6e02 7411 7d04 6415  ......}.n.t.}.d.
-000005c0: 7c03 6a12 9b00 9d02 7d05 7c03 6a12 a013  |.j.....}.|.j...
-000005d0: 6416 6417 a102 7d06 6418 7c06 9b00 9d02  d.d...}.d.|.....
-000005e0: 7d07 7c04 7c05 1b00 7d08 7c08 a00e a100  }.|.|...}.|.....
-000005f0: 72a1 7407 7c08 9b00 6419 9d02 8301 0100  r.t.|...d.......
-00000600: 740a a00b 6412 a101 0100 7407 641a 7c08  t...d.....t.d.|.
-00000610: 9b00 9d02 8301 0100 7c03 6a08 6400 7501  ........|.j.d.u.
-00000620: 72f0 7407 641b 8800 9b00 9d02 8301 0100  r.t.d...........
-00000630: 6900 7d09 6900 7d0a 641c 4400 5d14 7d0b  i.}.i.}.d.D.].}.
-00000640: 7414 8700 6601 641d 641e 8408 8800 a015  t...f.d.d.......
-00000650: 7c0b 641f 1700 a101 4400 8301 8301 7c09  |.d.....D.....|.
-00000660: 7c0b 3c00 71ba 7c09 a016 6420 a101 7d0c  |.<.q.|...d ..}.
-00000670: 7c0c 72da 7c0c 7c09 6421 3c00 7c09 a017  |.r.|.|.d!<.|...
-00000680: a100 4400 5d0d 7d0b 6422 6423 8400 7c09  ..D.].}.d"d#..|.
-00000690: 7c0b 1900 4400 8301 7c0a 7c0b 3c00 71de  |...D...|.|.<.q.
-000006a0: 7418 7c0a 8301 0100 7407 6424 7c08 9b00  t.|.....t.d$|...
-000006b0: 9d02 8301 0100 7c08 a019 a100 0100 741a  ......|.......t.
-000006c0: 741b 6a1c a01d a100 6a1e 8301 7c03 6a1f  t.j.....j...|.j.
-000006d0: 7c03 6a12 7c05 7c07 7420 7421 7c06 8301  |.j.|.|.t t!|...
-000006e0: 741a 7c0a 6421 1900 8301 741a 7c0a 6425  t.|.d!....t.|.d%
-000006f0: 1900 8301 741a 7c0a 6426 1900 8301 6427  ....t.|.d&....d'
-00000700: 9c0a 7d0d 6900 7d0e 6428 4400 5d0b 7d0f  ..}.i.}.d(D.].}.
-00000710: 7c0f 7d10 7c0f 6429 1700 7c0e 7c10 3c00  |.}.|.d)..|.|.<.
-00000720: 9001 7122 7c08 642a 7c07 9b00 9d02 1b00  ..q"|.d*|.......
-00000730: 7d11 642b 4400 5d0d 7d0f 7c11 7c0f 1b00  }.d+D.].}.|.|...
-00000740: 7d10 7c0f 6429 1700 7c0e 7c10 3c00 9001  }.|.d)..|.|.<...
-00000750: 7137 7c11 642c 1b00 7d12 7c12 6a19 642d  q7|.d,..}.|.j.d-
-00000760: 642e 8d01 0100 642f 7d0f 7c0f 6429 1700  d.....d/}.|.d)..
-00000770: 7c0e 7c12 7c0f 1b00 3c00 7c08 6430 1b00  |.|.|...<.|.d0..
-00000780: 7d13 7c13 a019 a100 0100 6431 7c0e 7c13  }.|.......d1|.|.
-00000790: 6432 7c06 9b00 6433 9d03 1b00 3c00 7c0e  d2|...d3....<.|.
-000007a0: a022 a100 4400 5d35 5c02 7d10 7d14 7423  ."..D.]5\.}.}.t#
-000007b0: a024 6434 a101 a025 7c14 a101 7d15 7423  .$d4...%|...}.t#
-000007c0: a026 7c15 a101 8f0c 7d16 7c16 a027 a100  .&|.....}.|..'..
-000007d0: 7d17 5700 6400 0400 0400 8303 0100 6e09  }.W.d.........n.
-000007e0: 3100 9001 7390 7701 0100 0100 0100 5900  1...s.w.......Y.
-000007f0: 0100 7428 7c17 8301 a029 7c0d a101 7d17  ..t(|....)|...}.
-00000800: 7c08 7c10 1b00 a02a 7c17 a101 0100 9001  |.|....*|.......
-00000810: 716f 7c13 6435 1b00 7d18 7c18 6a19 642d  qo|.d5..}.|.j.d-
-00000820: 642e 8d01 0100 7c09 a022 a100 4400 5d7c  d.....|.."..D.]|
-00000830: 5c02 7d0b 7d19 7c0b 6421 6b02 7d1a 7c18  \.}.}.|.d!k.}.|.
-00000840: 7c0b 1b00 7d1b 7c1b a019 a100 0100 7c19  |...}.|.......|.
-00000850: 4400 5d68 7d10 8800 7c10 1b00 a027 a100  D.]h}...|....'..
-00000860: 7d17 7a08 7c01 7c17 7c1a 6436 8d02 7d17  }.z.|.|.|.d6..}.
-00000870: 5700 6e11 0400 7c00 9001 79e6 0100 0100  W.n...|...y.....
-00000880: 0100 7407 6437 7c10 9b00 9d02 8301 0100  ..t.d7|.........
-00000890: 5900 6e01 7700 742b a02c 6438 6439 7c17  Y.n.w.t+.,d8d9|.
-000008a0: a103 a02d a100 6439 1700 7d17 643a 7c17  ...-..d9..}.d:|.
-000008b0: 7600 9002 7200 643b 7c17 a02d a100 1700  v...r.d;|..-....
-000008c0: 643c 1700 7d1c 6e02 7c17 7d1c 7c0b 6421  d<..}.n.|.}.|.d!
-000008d0: 6b02 9002 721b 742e 7c10 6a2f 8301 7d1d  k...r.t.|.j/..}.
-000008e0: 7c1d 6401 1900 6420 6b02 9002 721b 6421  |.d...d k...r.d!
-000008f0: 7c1d 6401 3c00 740d 7c1d 8e00 7d10 7c18  |.d.<.t.|...}.|.
-00000900: 7c10 1b00 a02a 7c17 a101 0100 7c12 7c10  |....*|.....|.|.
-00000910: 6a12 643d 1700 1b00 a02a 7c1c a101 0100  j.d=.....*|.....
-00000920: 9001 71c5 9001 71b3 7c03 6a08 6400 7501  ..q...q.|.j.d.u.
-00000930: 9002 724a 643e 4400 5d11 7d0f 8800 7c0f  ..rJd>D.].}...|.
-00000940: 1b00 7d16 7c16 a00e a100 9002 7248 7430  ..}.|.......rHt0
-00000950: 7c16 7c18 8302 0100 9002 7138 7407 643f  |.|.......q8t.d?
-00000960: 7c05 9b00 6440 7c08 9b00 6441 7c07 9b00  |...d@|...dA|...
-00000970: 6442 9d07 8301 0100 6400 5300 2943 4e72  dB......d.S.)CNr
-00000980: 0100 0000 2902 da0f 466f 616d 466f 726d  ....)...FoamForm
-00000990: 6174 4572 726f 72da 0b66 6f72 6d61 745f  atError..format_
-000009a0: 636f 6465 7a1c 666c 7569 6473 696d 666f  codez.fluidsimfo
-000009b0: 616d 2d69 6e69 7469 6174 652d 736f 6c76  am-initiate-solv
-000009c0: 6572 7a15 496e 6974 6961 7465 2061 206e  erz.Initiate a n
-000009d0: 6577 2073 6f6c 7665 7229 02da 0470 726f  ew solver)...pro
-000009e0: 67da 0b64 6573 6372 6970 7469 6f6e 7214  g..descriptionr.
-000009f0: 0000 007a 022d 637a 0b2d 2d66 726f 6d2d  ...z.-cz.--from-
-00000a00: 6361 7365 7a02 2d73 7a0d 2d2d 6672 6f6d  casez.-sz.--from
-00000a10: 2d73 6f6c 7665 727a 022d 617a 082d 2d61  -solverz.-az.--a
-00000a20: 7574 686f 727a 1746 6c75 6964 7369 6d66  uthorz.Fluidsimf
-00000a30: 6f61 6d20 6465 7665 6c6f 7065 7273 2901  oam developers).
-00000a40: da07 6465 6661 756c 747a 022d 647a 0d2d  ..defaultz.-dz.-
-00000a50: 2d64 6573 7469 6e61 7469 6f6e 7a38 596f  -destinationz8Yo
-00000a60: 7520 7368 6f75 6c64 2061 7420 6c65 6173  u should at leas
-00000a70: 7420 7072 6f76 6964 6520 6120 6361 7365  t provide a case
-00000a80: 2028 2d63 2920 6f72 2061 2073 6f6c 7665   (-c) or a solve
-00000a90: 7220 282d 7329 e901 0000 007a 2a53 6f72  r (-s).....z*Sor
-00000aa0: 7279 2c20 6f70 7469 6f6e 202d 7320 6973  ry, option -s is
-00000ab0: 206e 6f74 2079 6574 2069 6d70 6c65 6d65   not yet impleme
-00000ac0: 6e74 6564 2e2e 2e7a 1020 646f 6573 206e  nted...z. does n
-00000ad0: 6f74 2065 7869 7374 2e7a 0d66 6c75 6964  ot exist.z.fluid
-00000ae0: 7369 6d66 6f61 6d2d fa01 2dda 015f 5a0d  simfoam-..-.._Z.
-00000af0: 666c 7569 6473 696d 666f 616d 5f7a 1020  fluidsimfoam_z. 
-00000b00: 616c 7265 6164 7920 6578 6973 7473 2e7a  already exists.z
-00000b10: 1a4c 6574 2773 2069 6e69 7469 6174 6520  .Let's initiate 
-00000b20: 7468 6520 736f 6c76 6572 207a 0b55 7369  the solver z.Usi
-00000b30: 6e67 2063 6173 6520 2904 da06 7379 7374  ng case )...syst
-00000b40: 656d da08 636f 6e73 7461 6e74 da01 30fa  em..constant..0.
-00000b50: 0630 2e6f 7269 6763 0100 0000 0000 0000  .0.origc........
-00000b60: 0000 0000 0200 0000 0400 0000 3300 0000  ............3...
-00000b70: 7322 0000 0081 007c 005d 0c7d 017c 01a0  s".....|.].}.|..
-00000b80: 00a1 0072 027c 01a0 0188 00a1 0156 0001  ...r.|.......V..
-00000b90: 0071 0264 0053 0029 014e 2902 da07 6973  .q.d.S.).N)...is
-00000ba0: 5f66 696c 65da 0b72 656c 6174 6976 655f  _file..relative_
-00000bb0: 746f 2902 7215 0000 00da 0470 6174 68a9  to).r......path.
-00000bc0: 015a 0970 6174 685f 6361 7365 7212 0000  .Z.path_caser...
-00000bd0: 0072 1600 0000 da09 3c67 656e 6578 7072  .r......<genexpr
-00000be0: 3e68 0000 0073 0e00 0000 0280 0400 0202  >h...s..........
-00000bf0: 0602 02fc 0801 0aff 7a22 696e 6974 6961  ........z"initia
-00000c00: 7465 5f73 6f6c 7665 722e 3c6c 6f63 616c  te_solver.<local
-00000c10: 733e 2e3c 6765 6e65 7870 723e 7a02 2f2a  s>.<genexpr>z./*
-00000c20: 7232 0000 0072 3100 0000 6301 0000 0000  r2...r1...c.....
-00000c30: 0000 0000 0000 0002 0000 0003 0000 0053  ...............S
-00000c40: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
-00000c50: 0000 2902 7215 0000 00da 0170 7212 0000  ..).r......pr...
-00000c60: 0072 1200 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000c70: 7400 0000 7218 0000 007a 2369 6e69 7469  t...r....z#initi
-00000c80: 6174 655f 736f 6c76 6572 2e3c 6c6f 6361  ate_solver.<loca
-00000c90: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7a07  ls>.<listcomp>z.
-00000ca0: 4d61 6b69 6e67 2072 2f00 0000 7230 0000  Making r/...r0..
-00000cb0: 0029 0ada 0479 6561 72da 0661 7574 686f  .)...year..autho
-00000cc0: 725a 0a6e 616d 655f 7368 6f72 74da 0c6e  rZ.name_short..n
-00000cd0: 616d 655f 7072 6f6a 6563 74da 0c6e 616d  ame_project..nam
-00000ce0: 655f 7061 636b 6167 65da 1466 6c75 6964  e_package..fluid
-00000cf0: 7369 6d66 6f61 6d5f 7665 7273 696f 6e5a  simfoam_versionZ
-00000d00: 1073 7566 6669 785f 666f 725f 636c 6173  .suffix_for_clas
-00000d10: 735a 0e6e 616d 655f 7661 7269 6162 6c65  sZ.name_variable
-00000d20: 735a 116e 616d 655f 7379 7374 656d 5f66  sZ.name_system_f
-00000d30: 696c 6573 5a13 6e61 6d65 5f63 6f6e 7374  ilesZ.name_const
-00000d40: 616e 745f 6669 6c65 7329 03da 074c 4943  ant_files)...LIC
-00000d50: 454e 5345 7a09 5245 4144 4d45 2e6d 647a  ENSEz.README.mdz
-00000d60: 0e70 7970 726f 6a65 6374 2e74 6f6d 6c7a  .pyproject.tomlz
-00000d70: 092e 7465 6d70 6c61 7465 7a04 7372 632f  ..templatez.src/
-00000d80: 2903 7a0b 5f5f 696e 6974 5f5f 2e70 797a  ).z.__init__.pyz
-00000d90: 096f 7574 7075 742e 7079 fa08 7461 736b  .output.py..task
-00000da0: 732e 7079 da09 7465 6d70 6c61 7465 7354  s.py..templatesT
-00000db0: 2901 da07 7061 7265 6e74 7372 3f00 0000  )...parentsr?...
-00000dc0: da05 7465 7374 737a 2174 6573 745f 6765  ..testsz!test_ge
-00000dd0: 6e65 7261 7465 645f 736f 6c76 6572 2e70  nerated_solver.p
-00000de0: 792e 7465 6d70 6c61 7465 5a05 7465 7374  y.templateZ.test
-00000df0: 5f7a 032e 7079 7a16 666c 7569 6473 696d  _z..pyz.fluidsim
-00000e00: 666f 616d 2e72 6573 6f75 7263 6573 7a11  foam.resourcesz.
-00000e10: 7361 7665 645f 6361 7365 732f 6361 7365  saved_cases/case
-00000e20: 3029 01da 0861 735f 6669 656c 647a 184e  0)...as_fieldz.N
-00000e30: 6f74 2061 626c 6520 746f 2066 6f72 6d61  ot able to forma
-00000e40: 7420 6669 6c65 207a 055c 732b 5c6e da01  t file z.\s+\n..
-00000e50: 0a7a 027b 7b7a 097b 2520 7261 7720 257d  .z.{{z.{% raw %}
-00000e60: 7a0d 7b25 2065 6e64 7261 7720 257d 0a7a  z.{% endraw %}.z
-00000e70: 062e 6a69 6e6a 6129 025a 0841 6c6c 636c  ..jinja).Z.Allcl
-00000e80: 6561 6e5a 0641 6c6c 7275 6e7a 0d0a 0a4e  eanZ.Allrunz...N
-00000e90: 6577 2073 6f6c 7665 7220 7a5f 2063 7265  ew solver z_ cre
-00000ea0: 6174 6564 2120 596f 7520 6361 6e20 6e6f  ated! You can no
-00000eb0: 7720 696e 7374 616c 6c20 616e 6420 7465  w install and te
-00000ec0: 7374 2069 7420 746f 2063 6865 636b 2069  st it to check i
-00000ed0: 660a 6974 2072 6570 726f 6475 6365 7320  f.it reproduces 
-00000ee0: 796f 7572 2069 6e69 7469 616c 2063 6173  your initial cas
-00000ef0: 652e 0a0a 6060 600a 6364 207a 860a 7069  e...```.cd z..pi
-00000f00: 7020 696e 7374 616c 6c20 2d65 202e 0a70  p install -e ..p
-00000f10: 7974 6573 7420 7465 7374 7320 2d76 760a  ytest tests -vv.
-00000f20: 6060 600a 0a59 6f75 2063 616e 2074 6865  ```..You can the
-00000f30: 6e20 696d 7072 6f76 6520 796f 7572 2066  n improve your f
-00000f40: 6c75 6964 7369 6d66 6f61 6d20 736f 6c76  luidsimfoam solv
-00000f50: 6572 2062 7920 6d6f 6469 6679 696e 6720  er by modifying 
-00000f60: 6974 7320 6669 6c65 730a 2865 7370 6563  its files.(espec
-00000f70: 6961 6c6c 7920 7468 6520 6669 6c65 2073  ially the file s
-00000f80: 7263 2f7a 7e2f 6f75 7470 7574 2e70 7929  rc/z~/output.py)
-00000f90: 2e20 4578 616d 706c 6573 2063 616e 2062  . Examples can b
-00000fa0: 6520 666f 756e 6420 696e 0a68 7474 7073  e found in.https
-00000fb0: 3a2f 2f66 6f73 732e 6865 7074 6170 6f64  ://foss.heptapod
-00000fc0: 2e6e 6574 2f66 6c75 6964 6479 6e2f 666c  .net/fluiddyn/fl
-00000fd0: 7569 6473 696d 666f 616d 2f2d 2f74 7265  uidsimfoam/-/tre
-00000fe0: 652f 6272 616e 6368 2f64 6566 6175 6c74  e/branch/default
-00000ff0: 2f64 6f63 2f65 7861 6d70 6c65 730a 0a20  /doc/examples.. 
-00001000: 2020 2029 315a 1d66 6c75 6964 7369 6d66     )1Z.fluidsimf
-00001010: 6f61 6d2e 666f 616d 5f69 6e70 7574 5f66  oam.foam_input_f
-00001020: 696c 6573 7227 0000 0072 2800 0000 da08  ilesr'...r(.....
-00001030: 6172 6770 6172 7365 da0e 4172 6775 6d65  argparse..Argume
-00001040: 6e74 5061 7273 6572 da0c 6164 645f 6172  ntParser..add_ar
-00001050: 6775 6d65 6e74 da0a 7061 7273 655f 6172  gument..parse_ar
-00001060: 6773 721e 0000 005a 0966 726f 6d5f 6361  gsr....Z.from_ca
-00001070: 7365 5a0b 6672 6f6d 5f73 6f6c 7665 72da  seZ.from_solver.
-00001080: 0373 7973 da04 6578 6974 da13 4e6f 7449  .sys..exit..NotI
-00001090: 6d70 6c65 6d65 6e74 6564 4572 726f 7272  mplementedErrorr
-000010a0: 0400 0000 da06 6578 6973 7473 da0b 6465  ......exists..de
-000010b0: 7374 696e 6174 696f 6eda 0772 6573 6f6c  stination..resol
-000010c0: 7665 720a 0000 0072 1400 0000 da07 7265  ver....r......re
-000010d0: 706c 6163 6572 2000 0000 da04 676c 6f62  placer .....glob
-000010e0: da03 706f 70da 046b 6579 7372 0500 0000  ..pop..keysr....
-000010f0: da05 6d6b 6469 72da 0373 7472 da08 6461  ..mkdir..str..da
-00001100: 7465 7469 6d65 da04 6461 7465 da05 746f  tetime..date..to
-00001110: 6461 7972 3900 0000 723a 0000 0072 3d00  dayr9...r:...r=.
-00001120: 0000 7208 0000 0072 1d00 0000 7203 0000  ..r....r....r...
-00001130: 00da 0566 696c 6573 da08 6a6f 696e 7061  ...files..joinpa
-00001140: 7468 5a07 6173 5f66 696c 65da 0972 6561  thZ.as_file..rea
-00001150: 645f 7465 7874 7207 0000 00da 0a73 7562  d_textr......sub
-00001160: 7374 6974 7574 65da 0a77 7269 7465 5f74  stitute..write_t
-00001170: 6578 74da 0272 65da 0373 7562 da05 7374  ext..re..sub..st
-00001180: 7269 70da 046c 6973 74da 0570 6172 7473  rip..list..parts
-00001190: 7206 0000 0029 1e72 2700 0000 7228 0000  r....).r'...r(..
-000011a0: 00da 0670 6172 7365 72da 0461 7267 735a  ...parser..argsZ
-000011b0: 1070 6174 685f 6465 7374 696e 6174 696f  .path_destinatio
-000011c0: 6e72 3b00 0000 5a11 7375 6666 6978 5f66  nr;...Z.suffix_f
-000011d0: 6f72 5f6d 6f64 756c 6572 3c00 0000 5a0b  or_moduler<...Z.
-000011e0: 7061 7468 5f72 6573 756c 745a 0a70 6174  path_resultZ.pat
-000011f0: 685f 6669 6c65 735a 0a6e 616d 655f 6669  h_filesZ.name_fi
-00001200: 6c65 735a 086e 616d 655f 6469 725a 0a70  lesZ.name_dirZ.p
-00001210: 6174 6873 5f6f 7269 675a 0d73 7562 7374  aths_origZ.subst
-00001220: 6974 7574 696f 6e73 7240 0000 0072 1400  itutionsr@...r..
-00001230: 0000 5a0d 7265 6c61 7469 7665 5f70 6174  ..Z.relative_pat
-00001240: 685a 0c70 6174 685f 7061 636b 6167 655a  hZ.path_packageZ
-00001250: 0e70 6174 685f 7465 6d70 6c61 7465 735a  .path_templatesZ
-00001260: 0a70 6174 685f 7465 7374 73da 0874 656d  .path_tests..tem
-00001270: 706c 6174 655a 0c74 656d 706c 6174 655f  plateZ.template_
-00001280: 7265 7372 3500 0000 da04 636f 6465 5a0f  resr5.....codeZ.
-00001290: 7061 7468 5f73 6176 6564 5f63 6173 655a  path_saved_caseZ
-000012a0: 0e70 6174 685f 6669 6c65 735f 6469 7272  .path_files_dirr
-000012b0: 4300 0000 5a13 7061 7468 5f64 6972 5f73  C...Z.path_dir_s
-000012c0: 6176 6564 5f63 6173 655a 0d63 6f64 655f  aved_caseZ.code_
-000012d0: 7465 6d70 6c61 7465 7261 0000 0072 1200  templatera...r..
-000012e0: 0000 7236 0000 0072 1600 0000 da0f 696e  ..r6...r......in
-000012f0: 6974 6961 7465 5f73 6f6c 7665 7231 0000  itiate_solver1..
-00001300: 0073 0201 0000 1001 0402 0201 0201 06fe  .s..............
-00001310: 0a05 0c02 0c01 1001 0c01 0802 0802 1402  ................
-00001320: 0801 0a01 0a02 0801 0a02 0a01 0801 0e01  ................
-00001330: 0a01 0a02 1001 0402 0c02 0e01 0a01 0801  ................
-00001340: 0802 0e01 0a01 0e02 0a02 0e01 0402 0401  ................
-00001350: 0802 0c01 0c02 0efe 0a07 0401 0801 0c02  ................
-00001360: 1801 0802 0e02 0801 0e03 0401 0401 0201  ................
-00001370: 0201 0201 0601 0a01 0a01 0a01 06f6 040d  ................
-00001380: 0802 0401 1001 0e02 0801 0801 1001 0802  ................
-00001390: 0c01 0401 1001 0802 0801 0203 02fe 0e01  ................
-000013a0: 02ff 1004 0a01 0201 04ff 0c03 0a01 1eff  ................
-000013b0: 0e02 1201 0802 0c01 1002 0801 0801 0801  ................
-000013c0: 0802 0c01 0201 1001 0e01 1201 02ff 1604  ................
-000013d0: 0a02 1202 0402 0a02 0a01 0e01 0801 0801  ................
-000013e0: 0e02 0e01 0201 08ff 04e9 0c1b 0801 0801  ................
-000013f0: 0a01 0a01 0480 0202 0201 0202 04fe 0206  ................
-00001400: 04fa 020c 06f4 08ff 7266 0000 0029 1eda  ........rf...)..
-00001410: 075f 5f64 6f63 5f5f 7245 0000 0072 5500  .__doc__rE...rU.
-00001420: 0000 725d 0000 0072 4900 0000 da09 6675  ..r]...rI.....fu
-00001430: 6e63 746f 6f6c 7372 0200 0000 da09 696d  nctoolsr......im
-00001440: 706f 7274 6c69 6272 0300 0000 da07 7061  portlibr......pa
-00001450: 7468 6c69 6272 0400 0000 7205 0000 00da  thlibr....r.....
-00001460: 0673 6875 7469 6c72 0600 0000 da06 7374  .shutilr......st
-00001470: 7269 6e67 7207 0000 005a 0a69 6e66 6c65  ringr....Z.infle
-00001480: 6374 696f 6e72 0800 0000 5a16 666c 7569  ctionr....Z.flui
-00001490: 6473 696d 5f63 6f72 652e 6970 795f 6c6f  dsim_core.ipy_lo
-000014a0: 6164 7209 0000 005a 175f 7374 6172 745f  adr....Z._start_
-000014b0: 6970 7974 686f 6e5f 6c6f 6164 5f73 696d  ipython_load_sim
-000014c0: da13 666c 7569 6473 696d 5f63 6f72 652e  ..fluidsim_core.
-000014d0: 7061 7468 7372 0a00 0000 721b 0000 0072  pathsr....r....r
-000014e0: 0b00 0000 723d 0000 00da 1466 6c75 6964  ....r=.....fluid
-000014f0: 7369 6d66 6f61 6d2e 736f 6c76 6572 7372  simfoam.solversr
-00001500: 0c00 0000 7226 0000 0072 6600 0000 7212  ....r&...rf...r.
-00001510: 0000 0072 1200 0000 7212 0000 0072 1600  ...r....r....r..
-00001520: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00001530: 732a 0000 0004 0008 0408 0108 0108 010c  s*..............
-00001540: 010c 010c 010c 010c 010c 010c 020c 020c  ................
-00001550: 030c 010c 0108 0302 1204 0106 ff0c 05    ...............
+00000080: 0100 6401 6407 6c0c 6d0d 5a0d 6d0e 5a0e  ..d.d.l.m.Z.m.Z.
+00000090: 0100 6401 6408 6c0f 6d10 5a10 0100 6401  ..d.d.l.m.Z...d.
+000000a0: 6409 6c11 6d12 5a12 0100 6401 640a 6c13  d.l.m.Z...d.d.l.
+000000b0: 6d14 5a14 0100 6401 640b 6c15 6d16 5a17  m.Z...d.d.l.m.Z.
+000000c0: 0100 6401 640c 6c18 6d19 5a19 0100 6401  ..d.d.l.m.Z...d.
+000000d0: 640d 6c1a 6d1b 5a1c 0100 6401 640e 6c1d  d.l.m.Z...d.d.l.
+000000e0: 6d1e 5a1e 0100 640f 6410 8400 5a1f 6506  m.Z...d.d...Z.e.
+000000f0: 6517 6411 6412 8d02 5a16 6413 6414 8400  e.d.d...Z.d.d...
+00000100: 5a20 6402 5300 2915 7a1a 436f 6e73 6f6c  Z d.S.).z.Consol
+00000110: 6520 7363 7269 7074 2066 756e 6374 696f  e script functio
+00000120: 6e73 0a0a e900 0000 004e 2901 da07 7061  ns.......N)...pa
+00000130: 7274 6961 6c29 01da 0972 6573 6f75 7263  rtial)...resourc
+00000140: 6573 2901 da04 5061 7468 2901 da06 7070  es)...Path)...pp
+00000150: 7269 6e74 2902 da04 636f 7079 da05 7768  rint)...copy..wh
+00000160: 6963 6829 01da 0854 656d 706c 6174 6529  ich)...Template)
+00000170: 01da 0372 756e 2901 da08 6361 6d65 6c69  ...run)...cameli
+00000180: 7a65 2901 da16 7374 6172 745f 6970 7974  ze)...start_ipyt
+00000190: 686f 6e5f 6c6f 6164 5f73 696d 2901 da10  hon_load_sim)...
+000001a0: 7061 7468 5f64 6972 5f72 6573 756c 7473  path_dir_results
+000001b0: 2901 da0b 5f5f 7665 7273 696f 6e5f 5f29  )...__version__)
+000001c0: 01da 1161 7661 696c 6162 6c65 5f73 6f6c  ...available_sol
+000001d0: 7665 7273 6300 0000 0000 0000 0000 0000  versc...........
+000001e0: 0009 0000 0005 0000 0043 0000 0073 9a00  .........C...s..
+000001f0: 0000 6401 6400 6c00 7d00 6401 6400 6c01  ..d.d.l.}.d.d.l.
+00000200: 7d01 6401 6400 6c02 7d02 6402 6403 6404  }.d.d.l.}.d.d.d.
+00000210: 9c02 7d03 7c02 7c00 7c01 6703 7d04 7c04  ..}.|.|.|.g.}.|.
+00000220: 4400 5d08 7d05 7c05 6a03 7c03 7c05 6a04  D.].}.|.j.|.|.j.
+00000230: 3c00 7118 7c03 a005 a100 4400 5d10 5c02  <.q.|.....D.].\.
+00000240: 7d06 7d07 7406 7c06 a007 6405 a101 9b00  }.}.t.|...d.....
+00000250: 6406 7c07 9b00 9d03 8301 0100 7125 7408  d.|.........q%t.
+00000260: 7409 6407 6408 8400 740a 8300 4400 8301  t.d.d...t...D...
+00000270: 8301 8301 7d08 7406 6409 640a a00b 7c08  ....}.t.d.d...|.
+00000280: a101 1700 8301 0100 6400 5300 290b 4e72  ........d.S.).Nr
+00000290: 0100 0000 da07 5665 7273 696f 6efa 072d  ......Version..-
+000002a0: 2d2d 2d2d 2d2d 2902 5a07 5061 636b 6167  ------).Z.Packag
+000002b0: 6572 1000 0000 e90f 0000 00fa 0120 6301  er........... c.
+000002c0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+000002d0: 0000 0053 0000 0073 1200 0000 6700 7c00  ...S...s....g.|.
+000002e0: 5d05 7d01 7c01 6a00 9102 7102 5300 a900  ].}.|.j...q.S...
+000002f0: 2901 da04 6e61 6d65 2902 da02 2e30 5a0b  )...name)....0Z.
+00000300: 656e 7472 795f 706f 696e 7472 1300 0000  entry_pointr....
+00000310: 7213 0000 00fa 3e2f 686f 6d65 2f70 6965  r.....>/home/pie
+00000320: 7272 652f 4465 762f 666c 7569 6473 696d  rre/Dev/fluidsim
+00000330: 666f 616d 2f73 7263 2f66 6c75 6964 7369  foam/src/fluidsi
+00000340: 6d66 6f61 6d2f 7574 696c 2f63 6f6e 736f  mfoam/util/conso
+00000350: 6c65 2e70 79da 0a3c 6c69 7374 636f 6d70  le.py..<listcomp
+00000360: 3e29 0000 0073 0200 0000 1200 7a22 7072  >)...s......z"pr
+00000370: 696e 745f 7665 7273 696f 6e73 2e3c 6c6f  int_versions.<lo
+00000380: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00000390: 7a14 0a49 6e73 7461 6c6c 6564 2073 6f6c  z..Installed sol
+000003a0: 7665 7273 3a20 7a02 2c20 290c da08 666c  vers: z., )...fl
+000003b0: 7569 6464 796e da0d 666c 7569 6473 696d  uiddyn..fluidsim
+000003c0: 5f63 6f72 65da 0c66 6c75 6964 7369 6d66  _core..fluidsimf
+000003d0: 6f61 6d72 0d00 0000 da08 5f5f 6e61 6d65  oamr......__name
+000003e0: 5f5f da05 6974 656d 73da 0570 7269 6e74  __..items..print
+000003f0: da05 6c6a 7573 74da 0673 6f72 7465 64da  ..ljust..sorted.
+00000400: 0373 6574 720e 0000 00da 046a 6f69 6e29  .setr......join)
+00000410: 0972 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00000420: 5a08 7665 7273 696f 6e73 5a08 7061 636b  Z.versionsZ.pack
+00000430: 6167 6573 da07 7061 636b 6167 655a 0870  ages..packageZ.p
+00000440: 6b67 5f6e 616d 65da 0776 6572 7369 6f6e  kg_name..version
+00000450: da05 6e61 6d65 7372 1300 0000 7213 0000  ..namesr....r...
+00000460: 0072 1600 0000 da0e 7072 696e 745f 7665  .r......print_ve
+00000470: 7273 696f 6e73 1b00 0000 7316 0000 0008  rsions....s.....
+00000480: 0108 0108 010a 020a 0208 010e 0110 021a  ................
+00000490: 0118 0216 0172 2500 0000 7a1d 6672 6f6d  .....r%...z.from
+000004a0: 2066 6c75 6964 7369 6d66 6f61 6d20 696d   fluidsimfoam im
+000004b0: 706f 7274 206c 6f61 6429 015a 0b6c 6f61  port load).Z.loa
+000004c0: 645f 696d 706f 7274 6300 0000 0000 0000  d_importc.......
+000004d0: 0000 0000 0026 0000 000c 0000 0003 0000  .....&..........
+000004e0: 0073 fe05 0000 6401 6402 6c00 6d01 7d00  .s....d.d.l.m.}.
+000004f0: 6d02 7d01 0100 7403 6a04 6403 6404 6405  m.}...t.j.d.d.d.
+00000500: 8d02 7d02 7c02 a005 6406 a101 0100 7c02  ..}.|...d.....|.
+00000510: a005 6407 6408 a102 0100 7c02 a005 6409  ..d.d.....|...d.
+00000520: 640a a102 0100 7c02 6a05 640b 640c 640d  d.....|.j.d.d.d.
+00000530: 640e 8d03 0100 7c02 a005 640f 6410 a102  d.....|...d.d...
+00000540: 0100 7c02 a006 a100 7d03 7407 7c03 8301  ..|.....}.t.|...
+00000550: 0100 7c03 6a08 6400 7500 7249 7c03 6a09  ..|.j.d.u.rI|.j.
+00000560: 6400 7500 7249 7407 6411 8301 0100 740a  d.u.rIt.d.....t.
+00000570: a00b 6412 a101 0100 7c03 6a09 6400 7501  ..d.....|.j.d.u.
+00000580: 7252 740c 6413 8301 8201 7c03 6a08 6400  rRt.d.....|.j.d.
+00000590: 7501 726c 740d 7c03 6a08 8301 8900 8800  u.rlt.|.j.......
+000005a0: a00e a100 736c 7407 8800 9b00 6414 9d02  ....slt.....d...
+000005b0: 8301 0100 740a a00b 6412 a101 0100 7c03  ....t...d.....|.
+000005c0: 6a0f 6400 7501 7279 740d 7c03 6a0f 8301  j.d.u.ryt.|.j...
+000005d0: a010 a100 7d04 6e02 7411 7d04 6415 7c03  ....}.n.t.}.d.|.
+000005e0: 6a12 9b00 9d02 7d05 7c03 6a12 a013 6416  j.....}.|.j...d.
+000005f0: 6417 a102 7d06 6418 7c06 9b00 9d02 7d07  d...}.d.|.....}.
+00000600: 7c04 7c05 1b00 7d08 7c08 a00e a100 72a1  |.|...}.|.....r.
+00000610: 7407 7c08 9b00 6419 9d02 8301 0100 740a  t.|...d.......t.
+00000620: a00b 6412 a101 0100 7407 641a 7c08 9b00  ..d.....t.d.|...
+00000630: 9d02 8301 0100 7c03 6a08 6400 7501 9001  ......|.j.d.u...
+00000640: 724b 7407 641b 8800 9b00 9d02 8301 0100  rKt.d...........
+00000650: 6900 7d09 641c 4400 5d35 7d0a 7414 8800  i.}.d.D.]5}.t...
+00000660: a015 7c0a 641d 1700 a101 8301 7d0b 8700  ..|.d.......}...
+00000670: 6601 641e 641f 8408 7c0b 4400 8301 7c09  f.d.d...|.D...|.
+00000680: 7c0a 3c00 6420 641f 8400 7c0b 4400 8301  |.<.d d...|.D...
+00000690: 7d0c 7c0c 4400 5d15 7d0d 7c09 7c0a 1900  }.|.D.].}.|.|...
+000006a0: a016 7414 8700 6601 6421 6422 8408 7c0d  ..t...f.d!d"..|.
+000006b0: a015 6423 a101 4400 8301 8301 a101 0100  ..d#..D.........
+000006c0: 71d8 71b9 6900 7d0e 8800 a017 6423 a101  q.q.i.}.....d#..
+000006d0: 4400 5d22 7d0f 7c0f a018 a100 73fd 71f6  D.]"}.|.....s.q.
+000006e0: 7c0f a010 a100 7d10 8800 7c10 6a19 7601  |.....}...|.j.v.
+000006f0: 9001 720b 740c 6424 8301 8201 741a 7c0f  ..r.t.d$....t.|.
+00000700: a01b a100 8301 7c0e 741a 7c0f a01c 8800  ......|.t.|.....
+00000710: a101 8301 3c00 71f6 7c0e 9001 7224 7407  ....<.q.|...r$t.
+00000720: 6425 8301 0100 741d 7c0e 8301 0100 7c09  d%....t.|.....|.
+00000730: a01e 6426 a101 7d11 7c11 9001 7230 7c11  ..d&..}.|...r0|.
+00000740: 7c09 6427 3c00 6900 7d12 7c09 a01f a100  |.d'<.i.}.|.....
+00000750: 4400 5d10 7d0a 7414 6428 6422 8400 7c09  D.].}.t.d(d"..|.
+00000760: 7c0a 1900 4400 8301 8301 7c12 7c0a 3c00  |...D.....|.|.<.
+00000770: 9001 7136 741d 7c12 8301 0100 7407 6429  ..q6t.|.....t.d)
+00000780: 7c08 9b00 9d02 8301 0100 7c08 a020 a100  |.........|.. ..
+00000790: 0100 741a 7421 6a22 a023 a100 6a24 8301  ..t.t!j".#..j$..
+000007a0: 7c03 6a25 7c03 6a12 7c05 7c07 7426 7427  |.j%|.j.|.|.t&t'
+000007b0: 7c06 8301 741a 7c12 6427 1900 8301 741a  |...t.|.d'....t.
+000007c0: 7c12 642a 1900 8301 741a 7c12 642b 1900  |.d*....t.|.d+..
+000007d0: 8301 741a 7c0e 8301 642c 9c0b 7d13 6900  ..t.|...d,..}.i.
+000007e0: 7d14 642d 4400 5d0b 7d15 7c15 7d16 7c15  }.d-D.].}.|.}.|.
+000007f0: 642e 1700 7c14 7c16 3c00 9001 7180 7c08  d...|.|.<...q.|.
+00000800: 642f 7c07 9b00 9d02 1b00 7d17 6430 4400  d/|.......}.d0D.
+00000810: 5d0d 7d15 7c17 7c15 1b00 7d16 7c15 642e  ].}.|.|...}.|.d.
+00000820: 1700 7c14 7c16 3c00 9001 7195 7c17 6431  ..|.|.<...q.|.d1
+00000830: 1b00 7d18 7c18 6a20 6432 6433 8d01 0100  ..}.|.j d2d3....
+00000840: 7c18 6434 1b00 a028 a100 0100 6435 7d15  |.d4...(....d5}.
+00000850: 7c15 642e 1700 7c14 7c18 7c15 1b00 3c00  |.d...|.|.|...<.
+00000860: 7c08 6436 1b00 7d19 7c19 a020 a100 0100  |.d6..}.|.. ....
+00000870: 6437 7c14 7c19 6438 7c06 9b00 6439 9d03  d7|.|.d8|...d9..
+00000880: 1b00 3c00 7c14 a029 a100 4400 5d35 5c02  ..<.|..)..D.]5\.
+00000890: 7d16 7d1a 742a a02b 643a a101 a02c 7c1a  }.}.t*.+d:...,|.
+000008a0: a101 7d1b 742a a02d 7c1b a101 8f0c 7d0f  ..}.t*.-|.....}.
+000008b0: 7c0f a02e a100 7d1c 5700 6400 0400 0400  |.....}.W.d.....
+000008c0: 8303 0100 6e09 3100 9001 73f4 7701 0100  ....n.1...s.w...
+000008d0: 0100 0100 5900 0100 742f 7c1c 8301 a030  ....Y...t/|....0
+000008e0: 7c13 a101 7d1c 7c08 7c16 1b00 a031 7c1c  |...}.|.|....1|.
+000008f0: a101 0100 9001 71d3 7c19 643b 1b00 7d1d  ......q.|.d;..}.
+00000900: 7c1d 6a20 6432 6433 8d01 0100 7c09 a029  |.j d2d3....|..)
+00000910: a100 4400 5d93 5c02 7d0a 7d1e 7c0a 6427  ..D.].\.}.}.|.d'
+00000920: 6b02 7d1f 7c1d 7c0a 1b00 7d20 7c20 a020  k.}.|.|...} | . 
+00000930: a100 0100 7c1e 4400 5d7f 7d16 8800 7c16  ....|.D.].}...|.
+00000940: 1b00 a02e a100 7d1c 7a08 7c01 7c1c 7c1f  ......}.z.|.|.|.
+00000950: 643c 8d02 7d1c 5700 6e11 0400 7c00 9002  d<..}.W.n...|...
+00000960: 794a 0100 0100 0100 7407 643d 7c16 9b00  yJ......t.d=|...
+00000970: 9d02 8301 0100 5900 6e01 7700 7432 a033  ......Y.n.w.t2.3
+00000980: 643e 643f 7c1c a103 a034 a100 643f 1700  d>d?|....4..d?..
+00000990: 7d1c 6440 7c1c 7600 9002 7264 6441 7c1c  }.d@|.v...rddA|.
+000009a0: a034 a100 1700 6442 1700 7d21 6e02 7c1c  .4....dB..}!n.|.
+000009b0: 7d21 7c0a 6427 6b02 9002 727f 7435 7c16  }!|.d'k...r.t5|.
+000009c0: 6a36 8301 7d22 7c22 6401 1900 6426 6b02  j6..}"|"d...d&k.
+000009d0: 9002 727f 6427 7c22 6401 3c00 740d 7c22  ..r.d'|"d.<.t.|"
+000009e0: 8e00 7d16 7c1d 7c16 1b00 7d23 7c23 6a37  ..}.|.|...}#|#j7
+000009f0: 6a20 6432 6443 8d01 0100 7c23 a031 7c1c  j d2dC....|#.1|.
+00000a00: a101 0100 7c18 7c16 1b00 7d24 7c24 a038  ....|.|...}$|$.8
+00000a10: 7c24 6a12 6444 1700 a101 7d24 7c24 6a37  |$j.dD....}$|$j7
+00000a20: 6a20 6432 6443 8d01 0100 7c24 a031 7c21  j d2dC....|$.1|!
+00000a30: a101 0100 9002 7129 9002 7117 7c0e a029  ......q)..q.|..)
+00000a40: a100 4400 5d15 5c02 7d16 7d25 7c1d 7c16  ..D.].\.}.}%|.|.
+00000a50: 1b00 7d23 7c23 6a37 6a20 6432 6443 8d01  ..}#|#j7j d2dC..
+00000a60: 0100 7c23 a039 7c25 a101 0100 9002 71af  ..|#.9|%......q.
+00000a70: 7c03 6a08 6400 7501 9002 72de 8800 a015  |.j.d.u...r.....
+00000a80: 6445 a101 4400 5d0d 7d0f 7c0f a00e a100  dE..D.].}.|.....
+00000a90: 9002 72dc 743a 7c0f 7c1d 8302 0100 9002  ..r.t:|.|.......
+00000aa0: 71d0 743b 6446 8301 6400 7501 9002 72ef  q.t;dF..d.u...r.
+00000ab0: 743c 6446 6447 6448 741a 7c08 8301 6704  t<dFdGdHt.|...g.
+00000ac0: 8301 0100 7407 6449 7c05 9b00 644a 7c08  ....t.dI|...dJ|.
+00000ad0: 9b00 644b 7c07 9b00 644c 9d07 8301 0100  ..dK|...dL......
+00000ae0: 6400 5300 294d 4e72 0100 0000 2902 da0f  d.S.)MNr....)...
+00000af0: 466f 616d 466f 726d 6174 4572 726f 72da  FoamFormatError.
+00000b00: 0b66 6f72 6d61 745f 636f 6465 7a1c 666c  .format_codez.fl
+00000b10: 7569 6473 696d 666f 616d 2d69 6e69 7469  uidsimfoam-initi
+00000b20: 6174 652d 736f 6c76 6572 7a15 496e 6974  ate-solverz.Init
+00000b30: 6961 7465 2061 206e 6577 2073 6f6c 7665  iate a new solve
+00000b40: 7229 02da 0470 726f 67da 0b64 6573 6372  r)...prog..descr
+00000b50: 6970 7469 6f6e 7214 0000 007a 022d 637a  iptionr....z.-cz
+00000b60: 0b2d 2d66 726f 6d2d 6361 7365 7a02 2d73  .--from-casez.-s
+00000b70: 7a0d 2d2d 6672 6f6d 2d73 6f6c 7665 727a  z.--from-solverz
+00000b80: 022d 617a 082d 2d61 7574 686f 727a 1746  .-az.--authorz.F
+00000b90: 6c75 6964 7369 6d66 6f61 6d20 6465 7665  luidsimfoam deve
+00000ba0: 6c6f 7065 7273 2901 da07 6465 6661 756c  lopers)...defaul
+00000bb0: 747a 022d 647a 0d2d 2d64 6573 7469 6e61  tz.-dz.--destina
+00000bc0: 7469 6f6e 7a38 596f 7520 7368 6f75 6c64  tionz8You should
+00000bd0: 2061 7420 6c65 6173 7420 7072 6f76 6964   at least provid
+00000be0: 6520 6120 6361 7365 2028 2d63 2920 6f72  e a case (-c) or
+00000bf0: 2061 2073 6f6c 7665 7220 282d 7329 e901   a solver (-s)..
+00000c00: 0000 007a 2a53 6f72 7279 2c20 6f70 7469  ...z*Sorry, opti
+00000c10: 6f6e 202d 7320 6973 206e 6f74 2079 6574  on -s is not yet
+00000c20: 2069 6d70 6c65 6d65 6e74 6564 2e2e 2e7a   implemented...z
+00000c30: 1020 646f 6573 206e 6f74 2065 7869 7374  . does not exist
+00000c40: 2e7a 0d66 6c75 6964 7369 6d66 6f61 6d2d  .z.fluidsimfoam-
+00000c50: fa01 2dda 015f 5a0d 666c 7569 6473 696d  ..-.._Z.fluidsim
+00000c60: 666f 616d 5f7a 1020 616c 7265 6164 7920  foam_z. already 
+00000c70: 6578 6973 7473 2e7a 1a4c 6574 2773 2069  exists.z.Let's i
+00000c80: 6e69 7469 6174 6520 7468 6520 736f 6c76  nitiate the solv
+00000c90: 6572 207a 0b55 7369 6e67 2063 6173 6520  er z.Using case 
+00000ca0: 2904 da06 7379 7374 656d da08 636f 6e73  )...system..cons
+00000cb0: 7461 6e74 da01 30fa 0630 2e6f 7269 677a  tant..0..0.origz
+00000cc0: 022f 2a63 0100 0000 0000 0000 0000 0000  ./*c............
+00000cd0: 0200 0000 0500 0000 1300 0000 7326 0000  ............s&..
+00000ce0: 0067 007c 005d 0f7d 017c 01a0 00a1 0072  .g.|.].}.|.....r
+00000cf0: 027c 01a0 01a1 0073 027c 01a0 0288 00a1  .|.....s.|......
+00000d00: 0191 0271 0253 0072 1300 0000 a903 da07  ...q.S.r........
+00000d10: 6973 5f66 696c 65da 0a69 735f 7379 6d6c  is_file..is_syml
+00000d20: 696e 6bda 0b72 656c 6174 6976 655f 746f  ink..relative_to
+00000d30: a902 7215 0000 00da 0470 6174 68a9 015a  ..r......path..Z
+00000d40: 0970 6174 685f 6361 7365 7213 0000 0072  .path_caser....r
+00000d50: 1600 0000 7217 0000 0069 0000 0073 1000  ....r....i...s..
+00000d60: 0000 0600 0202 0601 02fd 0603 02fd 0801  ................
+00000d70: 06ff 7a23 696e 6974 6961 7465 5f73 6f6c  ..z#initiate_sol
+00000d80: 7665 722e 3c6c 6f63 616c 733e 2e3c 6c69  ver.<locals>.<li
+00000d90: 7374 636f 6d70 3e63 0100 0000 0000 0000  stcomp>c........
+00000da0: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
+00000db0: 7322 0000 0067 007c 005d 0d7d 017c 01a0  s"...g.|.].}.|..
+00000dc0: 00a1 0072 027c 016a 0164 006b 0372 027c  ...r.|.j.d.k.r.|
+00000dd0: 0191 0271 0253 0029 015a 0870 6f6c 794d  ...q.S.).Z.polyM
+00000de0: 6573 6829 02da 0669 735f 6469 7272 1400  esh)...is_dirr..
+00000df0: 0000 7236 0000 0072 1300 0000 7213 0000  ..r6...r....r...
+00000e00: 0072 1600 0000 7217 0000 006f 0000 0073  .r....r....o...s
+00000e10: 1000 0000 0600 0202 0601 02fd 0803 02fd  ................
+00000e20: 0201 06ff 6301 0000 0000 0000 0000 0000  ....c...........
+00000e30: 0002 0000 0004 0000 0033 0000 0073 2a00  .........3...s*.
+00000e40: 0000 8100 7c00 5d10 7d01 7c01 a000 a100  ....|.].}.|.....
+00000e50: 7202 7c01 a001 a100 7302 7c01 a002 8800  r.|.....s.|.....
+00000e60: a101 5600 0100 7102 6400 5300 2901 4e72  ..V...q.d.S.).Nr
+00000e70: 3200 0000 7236 0000 0072 3800 0000 7213  2...r6...r8...r.
+00000e80: 0000 0072 1600 0000 da09 3c67 656e 6578  ...r......<genex
+00000e90: 7072 3e77 0000 0073 1200 0000 0280 0400  pr>w...s........
+00000ea0: 0202 0601 02fd 0603 02fd 0801 0aff 7a22  ..............z"
+00000eb0: 696e 6974 6961 7465 5f73 6f6c 7665 722e  initiate_solver.
+00000ec0: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
+00000ed0: 723e da01 2a7a 2145 7874 6572 6e61 6c20  r>..*z!External 
+00000ee0: 7379 6d6c 696e 6b73 206e 6f74 2069 6d70  symlinks not imp
+00000ef0: 6c65 6d65 6e74 6564 7a12 696e 7465 726e  lementedz.intern
+00000f00: 616c 5f73 796d 6c69 6e6b 733a 7231 0000  al_symlinks:r1..
+00000f10: 0072 3000 0000 6301 0000 0000 0000 0000  .r0...c.........
+00000f20: 0000 0002 0000 0006 0000 0073 0000 0073  ...........s...s
+00000f30: 2600 0000 8100 7c00 5d0e 7d01 7400 7401  &.....|.].}.t.t.
+00000f40: 7c01 6a02 6400 6401 8502 1900 8e00 8301  |.j.d.d.........
+00000f50: 5600 0100 7102 6401 5300 2902 722b 0000  V...q.d.S.).r+..
+00000f60: 004e 2903 da03 7374 7272 0400 0000 da05  .N)...strr......
+00000f70: 7061 7274 7329 0272 1500 0000 da01 7072  parts).r......pr
+00000f80: 1300 0000 7213 0000 0072 1600 0000 723a  ....r....r....r:
+00000f90: 0000 0093 0000 0073 0800 0000 0280 0400  .......s........
+00000fa0: 1601 0aff 7a07 4d61 6b69 6e67 2072 2e00  ....z.Making r..
+00000fb0: 0000 722f 0000 0029 0bda 0479 6561 72da  ..r/...)...year.
+00000fc0: 0661 7574 686f 725a 0a6e 616d 655f 7368  .authorZ.name_sh
+00000fd0: 6f72 74da 0c6e 616d 655f 7072 6f6a 6563  ort..name_projec
+00000fe0: 74da 0c6e 616d 655f 7061 636b 6167 65da  t..name_package.
+00000ff0: 1466 6c75 6964 7369 6d66 6f61 6d5f 7665  .fluidsimfoam_ve
+00001000: 7273 696f 6e5a 1073 7566 6669 785f 666f  rsionZ.suffix_fo
+00001010: 725f 636c 6173 735a 0e6e 616d 655f 7661  r_classZ.name_va
+00001020: 7269 6162 6c65 735a 116e 616d 655f 7379  riablesZ.name_sy
+00001030: 7374 656d 5f66 696c 6573 5a13 6e61 6d65  stem_filesZ.name
+00001040: 5f63 6f6e 7374 616e 745f 6669 6c65 73da  _constant_files.
+00001050: 1169 6e74 6572 6e61 6c5f 7379 6d6c 696e  .internal_symlin
+00001060: 6b73 2903 da07 4c49 4345 4e53 457a 0952  ks)...LICENSEz.R
+00001070: 4541 444d 452e 6d64 7a0e 7079 7072 6f6a  EADME.mdz.pyproj
+00001080: 6563 742e 746f 6d6c 7a09 2e74 656d 706c  ect.tomlz..templ
+00001090: 6174 657a 0473 7263 2f29 02fa 0b5f 5f69  atez.src/)...__i
+000010a0: 6e69 745f 5f2e 7079 7a09 6f75 7470 7574  nit__.pyz.output
+000010b0: 2e70 79da 0974 656d 706c 6174 6573 5429  .py..templatesT)
+000010c0: 01da 0770 6172 656e 7473 7246 0000 007a  ...parentsrF...z
+000010d0: 0874 6173 6b73 2e70 79da 0574 6573 7473  .tasks.py..tests
+000010e0: 7a21 7465 7374 5f67 656e 6572 6174 6564  z!test_generated
+000010f0: 5f73 6f6c 7665 722e 7079 2e74 656d 706c  _solver.py.templ
+00001100: 6174 655a 0574 6573 745f 7a03 2e70 797a  ateZ.test_z..pyz
+00001110: 1666 6c75 6964 7369 6d66 6f61 6d2e 7265  .fluidsimfoam.re
+00001120: 736f 7572 6365 737a 1173 6176 6564 5f63  sourcesz.saved_c
+00001130: 6173 6573 2f63 6173 6530 2901 da08 6173  ases/case0)...as
+00001140: 5f66 6965 6c64 7a18 4e6f 7420 6162 6c65  _fieldz.Not able
+00001150: 2074 6f20 666f 726d 6174 2066 696c 6520   to format file 
+00001160: 7a0c 5b5e 5c53 5c6e 5c72 5d2b 5c6e da01  z.[^\S\n\r]+\n..
+00001170: 0a7a 027b 7b7a 097b 2520 7261 7720 257d  .z.{{z.{% raw %}
+00001180: 7a0d 7b25 2065 6e64 7261 7720 257d 0a29  z.{% endraw %}.)
+00001190: 01da 0865 7869 7374 5f6f 6b7a 062e 6a69  ...exist_okz..ji
+000011a0: 6e6a 617a 0441 6c6c 2a5a 0562 6c61 636b  njaz.All*Z.black
+000011b0: 7a02 2d6c 5a02 3832 7a0d 0a0a 4e65 7720  z.-lZ.82z...New 
+000011c0: 736f 6c76 6572 207a 5f20 6372 6561 7465  solver z_ create
+000011d0: 6421 2059 6f75 2063 616e 206e 6f77 2069  d! You can now i
+000011e0: 6e73 7461 6c6c 2061 6e64 2074 6573 7420  nstall and test 
+000011f0: 6974 2074 6f20 6368 6563 6b20 6966 0a69  it to check if.i
+00001200: 7420 7265 7072 6f64 7563 6573 2079 6f75  t reproduces you
+00001210: 7220 696e 6974 6961 6c20 6361 7365 2e0a  r initial case..
+00001220: 0a60 6060 0a63 6420 7a86 0a70 6970 2069  .```.cd z..pip i
+00001230: 6e73 7461 6c6c 202d 6520 2e0a 7079 7465  nstall -e ..pyte
+00001240: 7374 2074 6573 7473 202d 7676 0a60 6060  st tests -vv.```
+00001250: 0a0a 596f 7520 6361 6e20 7468 656e 2069  ..You can then i
+00001260: 6d70 726f 7665 2079 6f75 7220 666c 7569  mprove your flui
+00001270: 6473 696d 666f 616d 2073 6f6c 7665 7220  dsimfoam solver 
+00001280: 6279 206d 6f64 6966 7969 6e67 2069 7473  by modifying its
+00001290: 2066 696c 6573 0a28 6573 7065 6369 616c   files.(especial
+000012a0: 6c79 2074 6865 2066 696c 6520 7372 632f  ly the file src/
+000012b0: 7a7e 2f6f 7574 7075 742e 7079 292e 2045  z~/output.py). E
+000012c0: 7861 6d70 6c65 7320 6361 6e20 6265 2066  xamples can be f
+000012d0: 6f75 6e64 2069 6e0a 6874 7470 733a 2f2f  ound in.https://
+000012e0: 666f 7373 2e68 6570 7461 706f 642e 6e65  foss.heptapod.ne
+000012f0: 742f 666c 7569 6464 796e 2f66 6c75 6964  t/fluiddyn/fluid
+00001300: 7369 6d66 6f61 6d2f 2d2f 7472 6565 2f62  simfoam/-/tree/b
+00001310: 7261 6e63 682f 6465 6661 756c 742f 646f  ranch/default/do
+00001320: 632f 6578 616d 706c 6573 0a0a 2020 2020  c/examples..    
+00001330: 293d 5a1d 666c 7569 6473 696d 666f 616d  )=Z.fluidsimfoam
+00001340: 2e66 6f61 6d5f 696e 7075 745f 6669 6c65  .foam_input_file
+00001350: 7372 2600 0000 7227 0000 00da 0861 7267  sr&...r'.....arg
+00001360: 7061 7273 65da 0e41 7267 756d 656e 7450  parse..ArgumentP
+00001370: 6172 7365 72da 0c61 6464 5f61 7267 756d  arser..add_argum
+00001380: 656e 74da 0a70 6172 7365 5f61 7267 7372  ent..parse_argsr
+00001390: 1d00 0000 5a09 6672 6f6d 5f63 6173 655a  ....Z.from_caseZ
+000013a0: 0b66 726f 6d5f 736f 6c76 6572 da03 7379  .from_solver..sy
+000013b0: 73da 0465 7869 74da 134e 6f74 496d 706c  s..exit..NotImpl
+000013c0: 656d 656e 7465 6445 7272 6f72 7204 0000  ementedErrorr...
+000013d0: 00da 0665 7869 7374 73da 0b64 6573 7469  ...exists..desti
+000013e0: 6e61 7469 6f6e da07 7265 736f 6c76 6572  nation..resolver
+000013f0: 0c00 0000 7214 0000 00da 0772 6570 6c61  ....r......repla
+00001400: 6365 721f 0000 00da 0467 6c6f 62da 0665  cer......glob..e
+00001410: 7874 656e 64da 0572 676c 6f62 7234 0000  xtend..rglobr4..
+00001420: 0072 4800 0000 723c 0000 00da 0872 6561  .rH...r<.....rea
+00001430: 646c 696e 6b72 3500 0000 7205 0000 00da  dlinkr5...r.....
+00001440: 0370 6f70 da04 6b65 7973 da05 6d6b 6469  .pop..keys..mkdi
+00001450: 72da 0864 6174 6574 696d 65da 0464 6174  r..datetime..dat
+00001460: 65da 0574 6f64 6179 723f 0000 0072 4000  e..todayr?...r@.
+00001470: 0000 7243 0000 0072 0a00 0000 da05 746f  ..rC...r......to
+00001480: 7563 6872 1c00 0000 7203 0000 00da 0566  uchr....r......f
+00001490: 696c 6573 da08 6a6f 696e 7061 7468 5a07  iles..joinpathZ.
+000014a0: 6173 5f66 696c 65da 0972 6561 645f 7465  as_file..read_te
+000014b0: 7874 7208 0000 00da 0a73 7562 7374 6974  xtr......substit
+000014c0: 7574 65da 0a77 7269 7465 5f74 6578 74da  ute..write_text.
+000014d0: 0272 65da 0373 7562 da05 7374 7269 70da  .re..sub..strip.
+000014e0: 046c 6973 7472 3d00 0000 da06 7061 7265  .listr=.....pare
+000014f0: 6e74 da09 7769 7468 5f6e 616d 65da 0a73  nt..with_name..s
+00001500: 796d 6c69 6e6b 5f74 6f72 0600 0000 7207  ymlink_tor....r.
+00001510: 0000 0072 0900 0000 2926 7226 0000 0072  ...r....)&r&...r
+00001520: 2700 0000 da06 7061 7273 6572 da04 6172  '.....parser..ar
+00001530: 6773 5a10 7061 7468 5f64 6573 7469 6e61  gsZ.path_destina
+00001540: 7469 6f6e 7241 0000 005a 1173 7566 6669  tionrA...Z.suffi
+00001550: 785f 666f 725f 6d6f 6475 6c65 7242 0000  x_for_modulerB..
+00001560: 005a 0b70 6174 685f 7265 7375 6c74 5a0a  .Z.path_resultZ.
+00001570: 7061 7468 5f66 696c 6573 5a08 6e61 6d65  path_filesZ.name
+00001580: 5f64 6972 5a0c 7061 7468 735f 696e 5f64  _dirZ.paths_in_d
+00001590: 6972 5a0c 7061 7468 5f73 7562 6469 7273  irZ.path_subdirs
+000015a0: 5a0b 7061 7468 5f73 7562 6469 7272 4400  Z.path_subdirrD.
+000015b0: 0000 7237 0000 005a 0d70 6174 685f 7265  ..r7...Z.path_re
+000015c0: 736f 6c76 6564 5a0a 7061 7468 735f 6f72  solvedZ.paths_or
+000015d0: 6967 5a0a 6e61 6d65 5f66 696c 6573 5a0d  igZ.name_filesZ.
+000015e0: 7375 6273 7469 7475 7469 6f6e 7372 4700  substitutionsrG.
+000015f0: 0000 7214 0000 005a 0d72 656c 6174 6976  ..r....Z.relativ
+00001600: 655f 7061 7468 5a0c 7061 7468 5f70 6163  e_pathZ.path_pac
+00001610: 6b61 6765 5a0e 7061 7468 5f74 656d 706c  kageZ.path_templ
+00001620: 6174 6573 5a0a 7061 7468 5f74 6573 7473  atesZ.path_tests
+00001630: da08 7465 6d70 6c61 7465 5a0c 7465 6d70  ..templateZ.temp
+00001640: 6c61 7465 5f72 6573 da04 636f 6465 5a0f  late_res..codeZ.
+00001650: 7061 7468 5f73 6176 6564 5f63 6173 655a  path_saved_caseZ
+00001660: 0e70 6174 685f 6669 6c65 735f 6469 7272  .path_files_dirr
+00001670: 4a00 0000 5a13 7061 7468 5f64 6972 5f73  J...Z.path_dir_s
+00001680: 6176 6564 5f63 6173 655a 0d63 6f64 655f  aved_caseZ.code_
+00001690: 7465 6d70 6c61 7465 723d 0000 005a 1270  templater=...Z.p
+000016a0: 6174 685f 696e 5f73 6176 6564 5f63 6173  ath_in_saved_cas
+000016b0: 655a 0d70 6174 685f 7465 6d70 6c61 7465  eZ.path_template
+000016c0: da06 7461 7267 6574 7213 0000 0072 3800  ..targetr....r8.
+000016d0: 0000 7216 0000 00da 0f69 6e69 7469 6174  ..r......initiat
+000016e0: 655f 736f 6c76 6572 3200 0000 734a 0100  e_solver2...sJ..
+000016f0: 0010 0104 0202 0102 0106 fe0a 050c 020c  ................
+00001700: 0110 010c 0108 0208 0214 0208 010a 010a  ................
+00001710: 0208 010a 020a 0108 010e 010a 010a 0210  ................
+00001720: 0104 020c 020e 010a 0108 0108 020e 010a  ................
+00001730: 010e 020c 020e 0104 0208 0112 010a 0202  ................
+00001740: 020a fe06 0602 0206 fe08 0608 010c 0108  ................
+00001750: 0206 fe06 ff02 ff04 090e 0108 0102 0108  ................
+00001760: 010c 0108 0102 0106 0114 ff06 0408 0108  ................
+00001770: 010a 0206 0108 0104 020c 0108 0106 0110  ................
+00001780: ff08 040e 0208 010e 0304 0104 0102 0102  ................
+00001790: 0102 0106 010a 010a 010a 0106 0106 f504  ................
+000017a0: 0e08 0204 0110 010e 0208 0108 0110 0108  ................
+000017b0: 020c 010c 0104 0110 0108 0208 0102 0302  ................
+000017c0: fe0e 0102 ff10 040a 0102 0104 ff0c 030a  ................
+000017d0: 011e ff0e 0212 0108 020c 0110 0208 0108  ................
+000017e0: 0108 0108 020c 0102 0110 010e 0112 0102  ................
+000017f0: ff16 040a 0212 0204 020a 020a 010e 0108  ................
+00001800: 0108 0108 020e 010a 0108 0210 010e 010e  ................
+00001810: 0104 e310 2008 010e 010e 010c 020e 010a  .... ...........
+00001820: 010a 0104 800e 0214 0102 0202 0102 0204  ................
+00001830: fe02 0604 fa02 0c06 f408 ff72 7400 0000  ...........rt...
+00001840: 2921 da07 5f5f 646f 635f 5f72 4d00 0000  )!..__doc__rM...
+00001850: 725f 0000 0072 6800 0000 7251 0000 00da  r_...rh...rQ....
+00001860: 0966 756e 6374 6f6f 6c73 7202 0000 00da  .functoolsr.....
+00001870: 0969 6d70 6f72 746c 6962 7203 0000 00da  .importlibr.....
+00001880: 0770 6174 686c 6962 7204 0000 0072 0500  .pathlibr....r..
+00001890: 0000 da06 7368 7574 696c 7206 0000 0072  ....shutilr....r
+000018a0: 0700 0000 da06 7374 7269 6e67 7208 0000  ......stringr...
+000018b0: 00da 0a73 7562 7072 6f63 6573 7372 0900  ...subprocessr..
+000018c0: 0000 5a0a 696e 666c 6563 7469 6f6e 720a  ..Z.inflectionr.
+000018d0: 0000 005a 1666 6c75 6964 7369 6d5f 636f  ...Z.fluidsim_co
+000018e0: 7265 2e69 7079 5f6c 6f61 6472 0b00 0000  re.ipy_loadr....
+000018f0: 5a17 5f73 7461 7274 5f69 7079 7468 6f6e  Z._start_ipython
+00001900: 5f6c 6f61 645f 7369 6dda 1366 6c75 6964  _load_sim..fluid
+00001910: 7369 6d5f 636f 7265 2e70 6174 6873 720c  sim_core.pathsr.
+00001920: 0000 0072 1a00 0000 720d 0000 0072 4300  ...r....r....rC.
+00001930: 0000 da14 666c 7569 6473 696d 666f 616d  ....fluidsimfoam
+00001940: 2e73 6f6c 7665 7273 720e 0000 0072 2500  .solversr....r%.
+00001950: 0000 7274 0000 0072 1300 0000 7213 0000  ..rt...r....r...
+00001960: 0072 1300 0000 7216 0000 00da 083c 6d6f  .r....r......<mo
+00001970: 6475 6c65 3e01 0000 0073 2c00 0000 0400  dule>....s,.....
+00001980: 0804 0801 0801 0801 0c01 0c01 0c01 0c01  ................
+00001990: 1001 0c01 0c01 0c02 0c02 0c03 0c01 0c01  ................
+000019a0: 0803 0212 0401 06ff 0c05                 ..........
```

### Comparing `fluidsimfoam-0.0.6/src/fluidsimfoam/util/console.py` & `fluidsimfoam-0.0.7/src/fluidsimfoam/util/console.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 import datetime
 import re
 import sys
 from functools import partial
 from importlib import resources
 from pathlib import Path
 from pprint import pprint
-from shutil import copy
+from shutil import copy, which
 from string import Template
+from subprocess import run
 
 from inflection import camelize
 
 from fluidsim_core.ipy_load import (
     start_ipython_load_sim as _start_ipython_load_sim,
 )
 from fluidsim_core.paths import path_dir_results
@@ -94,30 +95,62 @@
 
     print(f"Let's initiate the solver {path_result}")
 
     if args.from_case is not None:
         print(f"Using case {path_case}")
 
         path_files = {}
-        name_files = {}
-
         for name_dir in ("system", "constant", "0", "0.orig"):
-            path_files[name_dir] = sorted(
+            paths_in_dir = sorted(path_case.glob(name_dir + "/*"))
+
+            path_files[name_dir] = [
                 path.relative_to(path_case)
-                for path in path_case.glob(name_dir + "/*")
-                # directories are not supported...
-                if path.is_file()
+                for path in paths_in_dir
+                if path.is_file() and not path.is_symlink()
+            ]
+
+            path_subdirs = [
+                path
+                for path in paths_in_dir
+                if path.is_dir() and path.name != "polyMesh"
+            ]
+
+            for path_subdir in path_subdirs:
+                path_files[name_dir].extend(
+                    sorted(
+                        path.relative_to(path_case)
+                        for path in path_subdir.glob("*")
+                        if path.is_file() and not path.is_symlink()
+                    )
+                )
+
+        internal_symlinks = {}
+        for path in path_case.rglob("*"):
+            if not path.is_symlink():
+                continue
+            path_resolved = path.resolve()
+            if path_case not in path_resolved.parents:
+                raise NotImplementedError("External symlinks not implemented")
+            internal_symlinks[str(path.relative_to(path_case))] = str(
+                path.readlink()
             )
 
+        if internal_symlinks:
+            print("internal_symlinks:")
+            pprint(internal_symlinks)
+
         paths_orig = path_files.pop("0.orig")
         if paths_orig:
             path_files["0"] = paths_orig
 
+        name_files = {}
         for name_dir in path_files.keys():
-            name_files[name_dir] = [p.name for p in path_files[name_dir]]
+            name_files[name_dir] = sorted(
+                str(Path(*p.parts[1:])) for p in path_files[name_dir]
+            )
 
         pprint(name_files)
 
     print(f"Making {path_result}")
     path_result.mkdir()
 
     substitutions = {
@@ -127,29 +160,31 @@
         "name_project": name_project,
         "name_package": name_package,
         "fluidsimfoam_version": fluidsimfoam_version,
         "suffix_for_class": camelize(suffix_for_module),
         "name_variables": str(name_files["0"]),
         "name_system_files": str(name_files["system"]),
         "name_constant_files": str(name_files["constant"]),
+        "internal_symlinks": str(internal_symlinks),
     }
 
     templates = {}
 
     for name in ["LICENSE", "README.md", "pyproject.toml"]:
         relative_path = name
         templates[relative_path] = name + ".template"
 
     path_package = path_result / f"src/{name_package}"
-    for name in ["__init__.py", "output.py", "tasks.py"]:
+    for name in ["__init__.py", "output.py"]:
         relative_path = path_package / name
         templates[relative_path] = name + ".template"
 
     path_templates = path_package / "templates"
     path_templates.mkdir(parents=True)
+    (path_templates / "__init__.py").touch()
     name = "tasks.py"
     templates[path_templates / name] = name + ".template"
 
     path_tests = path_result / "tests"
     path_tests.mkdir()
     templates[
         path_tests / f"test_{suffix_for_module}.py"
@@ -176,39 +211,51 @@
             code = (path_case / relative_path).read_text()
             try:
                 code = format_code(code, as_field=as_field)
             except FoamFormatError:
                 print(f"Not able to format file {relative_path}")
 
             # Trim trailing whitespaces
-            code = re.sub(r"\s+\n", "\n", code).strip() + "\n"
+            code = re.sub(r"[^\S\n\r]+\n", "\n", code).strip() + "\n"
 
             if "{{" in code:
                 # Escape jinja syntax
                 code_template = "{% raw %}" + code.strip() + "{% endraw %}\n"
             else:
                 code_template = code
 
             if name_dir == "0":
                 parts = list(relative_path.parts)
                 if parts[0] == "0.orig":
                     parts[0] = "0"
                     relative_path = Path(*parts)
 
-            (path_saved_case / relative_path).write_text(code)
-            (path_templates / (relative_path.name + ".jinja")).write_text(
-                code_template
-            )
+            path_in_saved_case = path_saved_case / relative_path
+            path_in_saved_case.parent.mkdir(exist_ok=True)
+            path_in_saved_case.write_text(code)
+
+            path_template = path_templates / relative_path
+            path_template = path_template.with_name(path_template.name + ".jinja")
+            path_template.parent.mkdir(exist_ok=True)
+            path_template.write_text(code_template)
+
+    # create the symlinks
+    for relative_path, target in internal_symlinks.items():
+        path_in_saved_case = path_saved_case / relative_path
+        path_in_saved_case.parent.mkdir(exist_ok=True)
+        path_in_saved_case.symlink_to(target)
 
     if args.from_case is not None:
-        for name in ("Allclean", "Allrun"):
-            path = path_case / name
+        for path in path_case.glob("All*"):
             if path.exists():
                 copy(path, path_saved_case)
 
+    if which("black") is not None:
+        run(["black", "-l", "82", str(path_result)])
+
     print(
         f"""
 
 New solver {name_project} created! You can now install and test it to check if
 it reproduces your initial case.
 
 ```
```

### Comparing `fluidsimfoam-0.0.6/PKG-INFO` & `fluidsimfoam-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: fluidsimfoam
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python framework for OpenFOAM
 License: BSD-3-Clause
 Author: pierre.augier
 Author-email: pierre.augier@univ-grenoble-alpes.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: jupyter
+Provides-Extra: pyvista
 Provides-Extra: qt
 Requires-Dist: PySide6 (>=6.5.1,<7.0.0) ; (python_version >= "3.9" and python_version < "3.12") and (extra == "qt")
 Requires-Dist: fluiddyn (>=0.5.2,<0.6.0)
 Requires-Dist: fluidsim-core (>=0.7.3,<0.8.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: invoke (>=2.0.0,<3.0.0)
 Requires-Dist: ipython (>=8.14.0,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jupyterlab (>=3.6.3,<4.0.0) ; extra == "jupyter"
 Requires-Dist: jupyterlab_myst (>=1.1.3,<2.0.0) ; extra == "jupyter"
 Requires-Dist: jupytext (>=1.14.5,<2.0.0) ; extra == "jupyter"
 Requires-Dist: lark (>=1.1.5,<2.0.0)
 Requires-Dist: mdformat-myst (>=0.1.4,<0.2.0) ; extra == "jupyter"
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pyvista (>=0.39.1,<0.40.0) ; extra == "pyvista"
 Requires-Dist: rich (>=13.3.3,<14.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # Fluidsimfoam
```

