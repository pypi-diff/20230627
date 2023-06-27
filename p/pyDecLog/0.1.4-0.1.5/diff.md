# Comparing `tmp/pyDecLog-0.1.4.tar.gz` & `tmp/pyDecLog-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDecLog-0.1.4.tar", last modified: Mon Jun 26 20:55:51 2023, max compression
+gzip compressed data, was "pyDecLog-0.1.5.tar", last modified: Tue Jun 27 10:19:34 2023, max compression
```

## Comparing `pyDecLog-0.1.4.tar` & `pyDecLog-0.1.5.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-26 20:55:51.267738 pyDecLog-0.1.4/
--rw-r--r--   0 gm_main    (501) staff       (20)      119 2023-06-26 19:28:02.000000 pyDecLog-0.1.4/.flake8
--rw-r--r--   0 gm_main    (501) staff       (20)     3191 2023-06-26 19:28:02.000000 pyDecLog-0.1.4/.gitignore
--rw-r--r--   0 gm_main    (501) staff       (20)      362 2023-06-26 20:31:42.000000 pyDecLog-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 gm_main    (501) staff       (20)     1077 2023-06-26 19:28:02.000000 pyDecLog-0.1.4/LICENSE
--rw-r--r--   0 gm_main    (501) staff       (20)     5453 2023-06-26 20:55:51.267206 pyDecLog-0.1.4/PKG-INFO
--rw-r--r--   0 gm_main    (501) staff       (20)    17907 2023-06-26 19:28:02.000000 pyDecLog-0.1.4/PyDecLog.py
--rw-r--r--   0 gm_main    (501) staff       (20)     5156 2023-06-26 20:45:11.000000 pyDecLog-0.1.4/README.md
--rw-r--r--   0 gm_main    (501) staff       (20)       23 2023-06-26 19:28:02.000000 pyDecLog-0.1.4/__init__.py
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-26 20:55:51.249250 pyDecLog-0.1.4/examples/
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-26 20:55:51.253873 pyDecLog-0.1.4/examples/@arguments/
--rw-r--r--   0 gm_main    (501) staff       (20)    10002 2023-06-26 20:19:01.000000 pyDecLog-0.1.4/examples/@arguments/@arguments.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-26 20:55:51.254309 pyDecLog-0.1.4/examples/@description/
--rw-r--r--   0 gm_main    (501) staff       (20)     3403 2023-06-26 20:19:53.000000 pyDecLog-0.1.4/examples/@description/@description.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-26 20:55:51.254647 pyDecLog-0.1.4/examples/@memory/
--rw-r--r--   0 gm_main    (501) staff       (20)    13004 2023-06-26 20:20:17.000000 pyDecLog-0.1.4/examples/@memory/@memory.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-26 20:55:51.255072 pyDecLog-0.1.4/examples/@message/
--rw-r--r--   0 gm_main    (501) staff       (20)    11406 2023-06-26 20:21:08.000000 pyDecLog-0.1.4/examples/@message/@message.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-26 20:55:51.255482 pyDecLog-0.1.4/examples/@profile_locals/
--rw-r--r--   0 gm_main    (501) staff       (20)     5066 2023-06-26 20:21:38.000000 pyDecLog-0.1.4/examples/@profile_locals/@profile_locals.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-26 20:55:51.255840 pyDecLog-0.1.4/examples/@signature/
--rw-r--r--   0 gm_main    (501) staff       (20)     3712 2023-06-26 20:22:08.000000 pyDecLog-0.1.4/examples/@signature/@signature.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-26 20:55:51.256304 pyDecLog-0.1.4/examples/@timing/
--rw-r--r--   0 gm_main    (501) staff       (20)    11334 2023-06-26 20:22:40.000000 pyDecLog-0.1.4/examples/@timing/@timing.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-26 20:55:51.256940 pyDecLog-0.1.4/examples/@typing/
--rw-r--r--   0 gm_main    (501) staff       (20)     9210 2023-06-26 20:23:00.000000 pyDecLog-0.1.4/examples/@typing/@typing.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-26 20:55:51.257377 pyDecLog-0.1.4/examples/lprint/
--rw-r--r--   0 gm_main    (501) staff       (20)     7415 2023-06-26 20:23:20.000000 pyDecLog-0.1.4/examples/lprint/lprint.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-26 20:55:51.257871 pyDecLog-0.1.4/examples/multiple_decorators/
--rw-r--r--   0 gm_main    (501) staff       (20)     3992 2023-06-26 20:23:46.000000 pyDecLog-0.1.4/examples/multiple_decorators/multiple_decorators.ipynb
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-26 20:55:51.258292 pyDecLog-0.1.4/examples/workflow/
--rw-r--r--   0 gm_main    (501) staff       (20)      943 2023-06-26 20:24:17.000000 pyDecLog-0.1.4/examples/workflow/workflow.py
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-26 20:55:51.260275 pyDecLog-0.1.4/pyDecLog.egg-info/
--rw-r--r--   0 gm_main    (501) staff       (20)     5453 2023-06-26 20:55:51.000000 pyDecLog-0.1.4/pyDecLog.egg-info/PKG-INFO
--rw-r--r--   0 gm_main    (501) staff       (20)     1005 2023-06-26 20:55:51.000000 pyDecLog-0.1.4/pyDecLog.egg-info/SOURCES.txt
--rw-r--r--   0 gm_main    (501) staff       (20)        1 2023-06-26 20:55:51.000000 pyDecLog-0.1.4/pyDecLog.egg-info/dependency_links.txt
--rw-r--r--   0 gm_main    (501) staff       (20)       14 2023-06-26 20:55:51.000000 pyDecLog-0.1.4/pyDecLog.egg-info/requires.txt
--rw-r--r--   0 gm_main    (501) staff       (20)        9 2023-06-26 20:55:51.000000 pyDecLog-0.1.4/pyDecLog.egg-info/top_level.txt
--rw-r--r--   0 gm_main    (501) staff       (20)      174 2023-06-26 19:28:02.000000 pyDecLog-0.1.4/pyproject.toml
--rw-r--r--   0 gm_main    (501) staff       (20)       38 2023-06-26 20:55:51.267882 pyDecLog-0.1.4/setup.cfg
--rw-r--r--   0 gm_main    (501) staff       (20)      816 2023-06-26 20:55:23.000000 pyDecLog-0.1.4/setup.py
-drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-26 20:55:51.266411 pyDecLog-0.1.4/tests/
--rwxr-xr-x   0 gm_main    (501) staff       (20)       85 2023-06-26 19:28:02.000000 pyDecLog-0.1.4/tests/test_all.sh
--rw-r--r--   0 gm_main    (501) staff       (20)     4166 2023-06-26 20:36:47.000000 pyDecLog-0.1.4/tests/test_arguments.py
--rw-r--r--   0 gm_main    (501) staff       (20)     3694 2023-06-26 20:36:47.000000 pyDecLog-0.1.4/tests/test_description.py
--rw-r--r--   0 gm_main    (501) staff       (20)     4119 2023-06-26 20:38:54.000000 pyDecLog-0.1.4/tests/test_get_log_and_level.py
--rw-r--r--   0 gm_main    (501) staff       (20)     1265 2023-06-26 20:34:06.000000 pyDecLog-0.1.4/tests/test_get_memory.py
--rw-r--r--   0 gm_main    (501) staff       (20)      785 2023-06-26 20:36:47.000000 pyDecLog-0.1.4/tests/test_get_time.py
--rw-r--r--   0 gm_main    (501) staff       (20)     2346 2023-06-26 20:36:47.000000 pyDecLog-0.1.4/tests/test_lprint.py
--rw-r--r--   0 gm_main    (501) staff       (20)     4189 2023-06-26 20:33:35.000000 pyDecLog-0.1.4/tests/test_memory.py
--rw-r--r--   0 gm_main    (501) staff       (20)     3635 2023-06-26 20:33:32.000000 pyDecLog-0.1.4/tests/test_message.py
--rw-r--r--   0 gm_main    (501) staff       (20)      828 2023-06-26 20:36:47.000000 pyDecLog-0.1.4/tests/test_profile_locals.py
--rw-r--r--   0 gm_main    (501) staff       (20)     3395 2023-06-26 20:36:47.000000 pyDecLog-0.1.4/tests/test_signature.py
--rw-r--r--   0 gm_main    (501) staff       (20)     3816 2023-06-26 20:36:47.000000 pyDecLog-0.1.4/tests/test_timing.py
--rw-r--r--   0 gm_main    (501) staff       (20)     3680 2023-06-26 20:36:47.000000 pyDecLog-0.1.4/tests/test_typing.py
--rwxr-xr-x   0 gm_main    (501) staff       (20)      431 2023-06-26 19:28:02.000000 pyDecLog-0.1.4/update_github.sh
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 10:19:34.233868 pyDecLog-0.1.5/
+-rw-r--r--   0 gm_main    (501) staff       (20)      119 2023-06-26 19:28:02.000000 pyDecLog-0.1.5/.flake8
+-rw-r--r--   0 gm_main    (501) staff       (20)        0 2023-06-27 06:17:56.000000 pyDecLog-0.1.5/.gitattributes
+-rw-r--r--   0 gm_main    (501) staff       (20)     3191 2023-06-26 19:28:02.000000 pyDecLog-0.1.5/.gitignore
+-rw-r--r--   0 gm_main    (501) staff       (20)      362 2023-06-26 20:31:42.000000 pyDecLog-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 gm_main    (501) staff       (20)     1077 2023-06-26 19:28:02.000000 pyDecLog-0.1.5/LICENSE
+-rw-r--r--   0 gm_main    (501) staff       (20)     5850 2023-06-27 10:19:34.233183 pyDecLog-0.1.5/PKG-INFO
+-rw-r--r--   0 gm_main    (501) staff       (20)     5532 2023-06-27 09:55:26.000000 pyDecLog-0.1.5/README.md
+-rw-r--r--   0 gm_main    (501) staff       (20)       23 2023-06-26 19:28:02.000000 pyDecLog-0.1.5/__init__.py
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 10:19:34.205907 pyDecLog-0.1.5/examples/
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 10:19:34.213285 pyDecLog-0.1.5/examples/@arguments/
+-rw-r--r--   0 gm_main    (501) staff       (20)    10002 2023-06-26 20:19:01.000000 pyDecLog-0.1.5/examples/@arguments/@arguments.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 10:19:34.214174 pyDecLog-0.1.5/examples/@description/
+-rw-r--r--   0 gm_main    (501) staff       (20)     3403 2023-06-26 20:19:53.000000 pyDecLog-0.1.5/examples/@description/@description.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 10:19:34.214858 pyDecLog-0.1.5/examples/@memory/
+-rw-r--r--   0 gm_main    (501) staff       (20)    13004 2023-06-26 20:20:17.000000 pyDecLog-0.1.5/examples/@memory/@memory.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 10:19:34.215702 pyDecLog-0.1.5/examples/@message/
+-rw-r--r--   0 gm_main    (501) staff       (20)    11406 2023-06-26 20:21:08.000000 pyDecLog-0.1.5/examples/@message/@message.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 10:19:34.216710 pyDecLog-0.1.5/examples/@profile_locals/
+-rw-r--r--   0 gm_main    (501) staff       (20)     5066 2023-06-26 20:21:38.000000 pyDecLog-0.1.5/examples/@profile_locals/@profile_locals.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 10:19:34.217638 pyDecLog-0.1.5/examples/@signature/
+-rw-r--r--   0 gm_main    (501) staff       (20)     3712 2023-06-26 20:22:08.000000 pyDecLog-0.1.5/examples/@signature/@signature.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 10:19:34.218555 pyDecLog-0.1.5/examples/@timing/
+-rw-r--r--   0 gm_main    (501) staff       (20)    11334 2023-06-26 20:22:40.000000 pyDecLog-0.1.5/examples/@timing/@timing.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 10:19:34.219291 pyDecLog-0.1.5/examples/@typing/
+-rw-r--r--   0 gm_main    (501) staff       (20)     9210 2023-06-26 20:23:00.000000 pyDecLog-0.1.5/examples/@typing/@typing.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 10:19:34.220060 pyDecLog-0.1.5/examples/lprint/
+-rw-r--r--   0 gm_main    (501) staff       (20)     8413 2023-06-27 08:21:32.000000 pyDecLog-0.1.5/examples/lprint/lprint.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 10:19:34.220767 pyDecLog-0.1.5/examples/multiple_decorators/
+-rw-r--r--   0 gm_main    (501) staff       (20)     3992 2023-06-26 20:23:46.000000 pyDecLog-0.1.5/examples/multiple_decorators/multiple_decorators.ipynb
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 10:19:34.221482 pyDecLog-0.1.5/examples/workflow/
+-rw-r--r--   0 gm_main    (501) staff       (20)      943 2023-06-26 20:24:17.000000 pyDecLog-0.1.5/examples/workflow/workflow.py
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 10:19:34.223860 pyDecLog-0.1.5/pyDecLog.egg-info/
+-rw-r--r--   0 gm_main    (501) staff       (20)     5850 2023-06-27 10:19:34.000000 pyDecLog-0.1.5/pyDecLog.egg-info/PKG-INFO
+-rw-r--r--   0 gm_main    (501) staff       (20)     1025 2023-06-27 10:19:34.000000 pyDecLog-0.1.5/pyDecLog.egg-info/SOURCES.txt
+-rw-r--r--   0 gm_main    (501) staff       (20)        1 2023-06-27 10:19:34.000000 pyDecLog-0.1.5/pyDecLog.egg-info/dependency_links.txt
+-rw-r--r--   0 gm_main    (501) staff       (20)       29 2023-06-27 10:19:34.000000 pyDecLog-0.1.5/pyDecLog.egg-info/requires.txt
+-rw-r--r--   0 gm_main    (501) staff       (20)        9 2023-06-27 10:19:34.000000 pyDecLog-0.1.5/pyDecLog.egg-info/top_level.txt
+-rw-r--r--   0 gm_main    (501) staff       (20)    17956 2023-06-27 07:08:23.000000 pyDecLog-0.1.5/pyDecLog.py
+-rw-r--r--   0 gm_main    (501) staff       (20)      174 2023-06-26 19:28:02.000000 pyDecLog-0.1.5/pyproject.toml
+-rw-r--r--   0 gm_main    (501) staff       (20)       28 2023-06-27 10:07:58.000000 pyDecLog-0.1.5/requirements.txt
+-rw-r--r--   0 gm_main    (501) staff       (20)       38 2023-06-27 10:19:34.234136 pyDecLog-0.1.5/setup.cfg
+-rw-r--r--   0 gm_main    (501) staff       (20)     1386 2023-06-27 10:19:32.000000 pyDecLog-0.1.5/setup.py
+drwxr-xr-x   0 gm_main    (501) staff       (20)        0 2023-06-27 10:19:34.232236 pyDecLog-0.1.5/tests/
+-rwxr-xr-x   0 gm_main    (501) staff       (20)       85 2023-06-26 19:28:02.000000 pyDecLog-0.1.5/tests/test_all.sh
+-rw-r--r--   0 gm_main    (501) staff       (20)     4166 2023-06-26 20:36:47.000000 pyDecLog-0.1.5/tests/test_arguments.py
+-rw-r--r--   0 gm_main    (501) staff       (20)     3694 2023-06-26 20:36:47.000000 pyDecLog-0.1.5/tests/test_description.py
+-rw-r--r--   0 gm_main    (501) staff       (20)     4119 2023-06-26 20:38:54.000000 pyDecLog-0.1.5/tests/test_get_log_and_level.py
+-rw-r--r--   0 gm_main    (501) staff       (20)     1265 2023-06-26 20:34:06.000000 pyDecLog-0.1.5/tests/test_get_memory.py
+-rw-r--r--   0 gm_main    (501) staff       (20)      785 2023-06-26 20:36:47.000000 pyDecLog-0.1.5/tests/test_get_time.py
+-rw-r--r--   0 gm_main    (501) staff       (20)     2346 2023-06-26 20:36:47.000000 pyDecLog-0.1.5/tests/test_lprint.py
+-rw-r--r--   0 gm_main    (501) staff       (20)     4189 2023-06-26 20:33:35.000000 pyDecLog-0.1.5/tests/test_memory.py
+-rw-r--r--   0 gm_main    (501) staff       (20)     3635 2023-06-26 20:33:32.000000 pyDecLog-0.1.5/tests/test_message.py
+-rw-r--r--   0 gm_main    (501) staff       (20)      828 2023-06-26 20:36:47.000000 pyDecLog-0.1.5/tests/test_profile_locals.py
+-rw-r--r--   0 gm_main    (501) staff       (20)     3395 2023-06-26 20:36:47.000000 pyDecLog-0.1.5/tests/test_signature.py
+-rw-r--r--   0 gm_main    (501) staff       (20)     3816 2023-06-26 20:36:47.000000 pyDecLog-0.1.5/tests/test_timing.py
+-rw-r--r--   0 gm_main    (501) staff       (20)     3680 2023-06-26 20:36:47.000000 pyDecLog-0.1.5/tests/test_typing.py
+-rwxr-xr-x   0 gm_main    (501) staff       (20)      431 2023-06-26 19:28:02.000000 pyDecLog-0.1.5/update_github.sh
```

### Comparing `pyDecLog-0.1.4/.gitignore` & `pyDecLog-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/LICENSE` & `pyDecLog-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/PKG-INFO` & `pyDecLog-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: pyDecLog
-Version: 0.1.4
-Summary: pyDecLog: a python package for logging via decorators 
+Version: 0.1.5
+Summary: pyDecLog: a Python module for logging via decorators
 Home-page: https://github.com/kyaiooiayk/pyDecLog
 Author: kyaiooiayk
 Author-email: kayaiooiayk@email.com
 License: MIT
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyDecLog
-pyDecLog: a simple and easy to use Python package for logging via decorators.
+
+[![PyPI Version](https://img.shields.io/pypi/v/pyDecLog.svg)](https://pypi.org/project/dython/)
+[![Python Version](https://img.shields.io/pypi/pyversions/pyDecLog.svg)](https://pypi.org/project/dython/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/pyDecLog)](https://pypistats.org/packages/pyDecLog)
+[![License](https://img.shields.io/pypi/l/pyDecLog)](https://github.com/kyaiooiayk/pyDecLog/blob/master/LICENSE)
+
+pyDecLog: a simple and easy to use Python module for logging via decorators.
 ***
 
 ## 🚀Quick start
 - Say we have the following workflow
 ```python
 from pyDecLog import arguments as arg
 from pyDecLog import signature as sign
@@ -77,17 +84,16 @@
 
 ## 🚀Useful for
 - Keep track of Python pipelines.
 - Log info about a function during development both on python script or jupyter notebook.
 ***
 
 ## ⚙️Installation
-- Create your own virtual environment and run `pip install -r requirements.txt`, then choose one of the following options:
-  - Option 1, via pip: `pip install pydeclog` 
-  - Option 2, from source: `pip install git+https://github.com/kayaiooiayk/pydeclog.git`
+- Create your own virtual environment and run `pip install -r requirements.txt`
+- Via pip: `pip install pyDecLog`   
 ***
 
 ## 🔗Dependencies
 - PyDevLog requires Python 3.5 or higher, and the following packages:
   - `pympler`
   - `numpy`
 ***
@@ -153,19 +159,20 @@
 - See the `examples` folder.
 ***
 
 ## 📚References
 - [Decorators with parameters?](https://stackoverflow.com/questions/5929107/decorators-with-parameters)
 - [How to expose persistent local variables? Part#1](https://code.activestate.com/recipes/577283-decorator-to-expose-local-variables-of-a-function-/)
 - [How to expose persistent local variables? Part#2](https://stackoverflow.com/questions/9186395/python-is-there-a-way-to-get-a-local-function-variable-from-within-a-decorator)
+- [How to time your code](https://stackoverflow.com/questions/17579357/time-time-vs-timeit-timeit)
 ***
 
 ## 📝Changelog
 - `0.1.4`  first release (26/06/23).
-- ***
+***
 
 ## 📝To-do
 - There is no planned development.
 ***
 
 ## 🪪License
 - MIT License
```

### Comparing `pyDecLog-0.1.4/PyDecLog.py` & `pyDecLog-0.1.5/pyDecLog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from functools import wraps, partial
 import logging
 import os
-import time
+from timeit import default_timer as timer
 from contextlib import redirect_stdout
 from io import StringIO
 import numpy as np
 import inspect
 from sys import getsizeof
 import sys
 from pympler.asizeof import asizeof
@@ -41,15 +41,14 @@
     logger_obj = get_logger(
         log_file_name=log_file_name,
         console_log_level=console_log_level,
         log_file_path=log_file_path,
     )
     return logger_obj
 
-
 def _get_time(t_start: float, t_end: float, unit: str):
     """Get elapsed time given the unit.
 
     Parameters
     ----------
     t_start : float
         kernel time at start of process.
@@ -110,24 +109,24 @@
     RunTimeWarning
         Raise if called with positional arguments.
     """
 
     def _decorator(func):
         @wraps(func)
         def wrapper(self, *args, **kwargs):
-            t1 = time.time()
+            time_start = timer()
             output = func(self, *args, **kwargs)
-            t2 = time.time()
+            time_end = timer()
 
             log_level = _get_log_level(
                 level, console_log_level, log_file_name, log_file_path
             )
 
             log_level(
-                f"{str(func.__name__)} was executed in: {str(_get_time(t1, t2, unit))} {unit}"
+                f"{str(func.__name__)} was executed in: {str(_get_time(time_start, time_end, unit))} {unit}"
             )
             return output
 
         return wrapper
 
     if callable(func_):
         return _decorator(func_)
```

### Comparing `pyDecLog-0.1.4/README.md` & `pyDecLog-0.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # pyDecLog
-pyDecLog: a simple and easy to use Python package for logging via decorators.
+
+[![PyPI Version](https://img.shields.io/pypi/v/pyDecLog.svg)](https://pypi.org/project/dython/)
+[![Python Version](https://img.shields.io/pypi/pyversions/pyDecLog.svg)](https://pypi.org/project/dython/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/pyDecLog)](https://pypistats.org/packages/pyDecLog)
+[![License](https://img.shields.io/pypi/l/pyDecLog)](https://github.com/kyaiooiayk/pyDecLog/blob/master/LICENSE)
+
+pyDecLog: a simple and easy to use Python module for logging via decorators.
 ***
 
 ## 🚀Quick start
 - Say we have the following workflow
 ```python
 from pyDecLog import arguments as arg
 from pyDecLog import signature as sign
@@ -66,17 +72,16 @@
 
 ## 🚀Useful for
 - Keep track of Python pipelines.
 - Log info about a function during development both on python script or jupyter notebook.
 ***
 
 ## ⚙️Installation
-- Create your own virtual environment and run `pip install -r requirements.txt`, then choose one of the following options:
-  - Option 1, via pip: `pip install pydeclog` 
-  - Option 2, from source: `pip install git+https://github.com/kayaiooiayk/pydeclog.git`
+- Create your own virtual environment and run `pip install -r requirements.txt`
+- Via pip: `pip install pyDecLog`   
 ***
 
 ## 🔗Dependencies
 - PyDevLog requires Python 3.5 or higher, and the following packages:
   - `pympler`
   - `numpy`
 ***
@@ -142,19 +147,20 @@
 - See the `examples` folder.
 ***
 
 ## 📚References
 - [Decorators with parameters?](https://stackoverflow.com/questions/5929107/decorators-with-parameters)
 - [How to expose persistent local variables? Part#1](https://code.activestate.com/recipes/577283-decorator-to-expose-local-variables-of-a-function-/)
 - [How to expose persistent local variables? Part#2](https://stackoverflow.com/questions/9186395/python-is-there-a-way-to-get-a-local-function-variable-from-within-a-decorator)
+- [How to time your code](https://stackoverflow.com/questions/17579357/time-time-vs-timeit-timeit)
 ***
 
 ## 📝Changelog
 - `0.1.4`  first release (26/06/23).
-- ***
+***
 
 ## 📝To-do
 - There is no planned development.
 ***
 
 ## 🪪License
 - MIT License
```

### Comparing `pyDecLog-0.1.4/examples/@arguments/@arguments.ipynb` & `pyDecLog-0.1.5/examples/@arguments/@arguments.ipynb`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/examples/@description/@description.ipynb` & `pyDecLog-0.1.5/examples/@description/@description.ipynb`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/examples/@memory/@memory.ipynb` & `pyDecLog-0.1.5/examples/@memory/@memory.ipynb`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/examples/@message/@message.ipynb` & `pyDecLog-0.1.5/examples/@message/@message.ipynb`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/examples/@profile_locals/@profile_locals.ipynb` & `pyDecLog-0.1.5/examples/@profile_locals/@profile_locals.ipynb`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/examples/@signature/@signature.ipynb` & `pyDecLog-0.1.5/examples/@signature/@signature.ipynb`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/examples/@timing/@timing.ipynb` & `pyDecLog-0.1.5/examples/@timing/@timing.ipynb`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/examples/@typing/@typing.ipynb` & `pyDecLog-0.1.5/examples/@typing/@typing.ipynb`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/examples/lprint/lprint.ipynb` & `pyDecLog-0.1.5/examples/lprint/lprint.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9715073529411764%*

 * *Differences: {"'cells'": "{0: {'metadata': {'ExecuteTime': {'end_time': '2023-06-27T08:20:07.739784Z', "*

 * *            "'start_time': '2023-06-27T08:20:07.648708Z'}}}, 1: {'metadata': {'ExecuteTime': "*

 * *            "{'end_time': '2023-06-27T08:20:07.863992Z', 'start_time': "*

 * *            "'2023-06-27T08:20:07.741557Z'}}, 'outputs': []}, 2: {'metadata': {'ExecuteTime': "*

 * *            "{'end_time': '2023-06-27T08:20:07.872199Z', 'start_time': "*

 * *            "'2023-06-27T08:20:07.868291Z'}}}, 3: {'metadata': {'ExecuteTime': {'en […]*

```diff
@@ -2,114 +2,106 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "9cb27718",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-06-26T20:23:18.370650Z",
-                    "start_time": "2023-06-26T20:23:18.275458Z"
+                    "end_time": "2023-06-27T08:20:07.739784Z",
+                    "start_time": "2023-06-27T08:20:07.648708Z"
                 }
             },
             "outputs": [],
             "source": [
                 "from pyDecLog import lprint"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "45c5909a",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-06-26T20:23:18.495096Z",
-                    "start_time": "2023-06-26T20:23:18.372218Z"
+                    "end_time": "2023-06-27T08:20:07.863992Z",
+                    "start_time": "2023-06-27T08:20:07.741557Z"
                 }
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "rm: LOG.log: No such file or directory\r\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "rm LOG.log"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "8384c3a8",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-06-26T20:23:18.503331Z",
-                    "start_time": "2023-06-26T20:23:18.498920Z"
+                    "end_time": "2023-06-27T08:20:07.872199Z",
+                    "start_time": "2023-06-27T08:20:07.868291Z"
                 }
             },
             "outputs": [],
             "source": [
                 "lprint(console_log_level=\"critical\").info(\"simple message\") "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "4769e6bc",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-06-26T20:23:18.508389Z",
-                    "start_time": "2023-06-26T20:23:18.505218Z"
+                    "end_time": "2023-06-27T08:20:07.877535Z",
+                    "start_time": "2023-06-27T08:20:07.874011Z"
                 }
             },
             "outputs": [],
             "source": [
                 "lprint(console_log_level=\"critical\").debug(\"simple message\") "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "dc49abfd",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-06-26T20:23:18.513512Z",
-                    "start_time": "2023-06-26T20:23:18.510266Z"
+                    "end_time": "2023-06-27T08:20:07.882597Z",
+                    "start_time": "2023-06-27T08:20:07.879448Z"
                 }
             },
             "outputs": [],
             "source": [
                 "lprint(console_log_level=\"critical\").warning(\"simple message\") "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "id": "574e4456",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-06-26T20:23:18.518705Z",
-                    "start_time": "2023-06-26T20:23:18.515432Z"
+                    "end_time": "2023-06-27T08:20:07.887116Z",
+                    "start_time": "2023-06-27T08:20:07.884154Z"
                 }
             },
             "outputs": [],
             "source": [
                 "lprint(console_log_level=\"critical\").error(\"simple message\") "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "id": "8fb665d2",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-06-26T20:23:18.524295Z",
-                    "start_time": "2023-06-26T20:23:18.520635Z"
+                    "end_time": "2023-06-27T08:20:07.892617Z",
+                    "start_time": "2023-06-27T08:20:07.888842Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
@@ -123,58 +115,58 @@
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "id": "406e0cf9",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-06-26T20:23:18.651519Z",
-                    "start_time": "2023-06-26T20:23:18.526144Z"
+                    "end_time": "2023-06-27T08:20:08.018051Z",
+                    "start_time": "2023-06-27T08:20:07.894519Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "2023/06/26 | 21:23:18 | INFO simple message\r\n",
-                        "2023/06/26 | 21:23:18 | DEBUG simple message\r\n",
-                        "2023/06/26 | 21:23:18 | WARNING simple message\r\n",
-                        "2023/06/26 | 21:23:18 | ERROR simple message\r\n",
-                        "2023/06/26 | 21:23:18 | CRITICAL simple CRITICAL message\r\n"
+                        "2023/06/27 | 09:20:07 | INFO simple message\r\n",
+                        "2023/06/27 | 09:20:07 | DEBUG simple message\r\n",
+                        "2023/06/27 | 09:20:07 | WARNING simple message\r\n",
+                        "2023/06/27 | 09:20:07 | ERROR simple message\r\n",
+                        "2023/06/27 | 09:20:07 | CRITICAL simple CRITICAL message\r\n"
                     ]
                 }
             ],
             "source": [
                 "cat LOG.log"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "id": "8f069c4c",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-06-26T20:23:18.783230Z",
-                    "start_time": "2023-06-26T20:23:18.656762Z"
+                    "end_time": "2023-06-27T08:20:08.151067Z",
+                    "start_time": "2023-06-27T08:20:08.023489Z"
                 }
             },
             "outputs": [],
             "source": [
                 "rm LOG.log"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "id": "56a6761b",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-06-26T20:23:18.792233Z",
-                    "start_time": "2023-06-26T20:23:18.785994Z"
+                    "end_time": "2023-06-27T08:20:08.161165Z",
+                    "start_time": "2023-06-27T08:20:08.153609Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
@@ -201,82 +193,124 @@
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "id": "b85bfd41",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-06-26T20:23:18.919396Z",
-                    "start_time": "2023-06-26T20:23:18.794006Z"
+                    "end_time": "2023-06-27T08:20:08.292458Z",
+                    "start_time": "2023-06-27T08:20:08.163599Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "2023/06/26 | 21:23:18 | INFO Results 1 is: 3\r\n",
-                        "2023/06/26 | 21:23:18 | DEBUG Results 2 is: 3\r\n",
-                        "2023/06/26 | 21:23:18 | WARNING Results 3 is: 3\r\n",
-                        "2023/06/26 | 21:23:18 | ERROR Results 4 is: 3\r\n",
-                        "2023/06/26 | 21:23:18 | CRITICAL Results 5 is: 3\r\n"
+                        "2023/06/27 | 09:20:08 | INFO Results 1 is: 3\r\n",
+                        "2023/06/27 | 09:20:08 | DEBUG Results 2 is: 3\r\n",
+                        "2023/06/27 | 09:20:08 | WARNING Results 3 is: 3\r\n",
+                        "2023/06/27 | 09:20:08 | ERROR Results 4 is: 3\r\n",
+                        "2023/06/27 | 09:20:08 | CRITICAL Results 5 is: 3\r\n"
                     ]
                 }
             ],
             "source": [
                 "cat LOG.log"
             ]
         },
         {
+            "cell_type": "markdown",
+            "id": "45223a88",
+            "metadata": {},
+            "source": [
+                "# `try` and `except` behaviour\n",
+                "<hr style=\"border:2px solid black\"> </hr>"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "ece4a456",
+            "metadata": {},
+            "source": [
+                "- Logging an exception in python with an error can be done in the `logging.exception()` method.\n",
+                "- This function logs a message with level `ERROR` on this logger. "
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": 12,
-            "id": "e6849545",
+            "id": "bb2c6349",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-06-26T20:23:18.924494Z",
-                    "start_time": "2023-06-26T20:23:18.921759Z"
+                    "end_time": "2023-06-27T08:20:08.425251Z",
+                    "start_time": "2023-06-27T08:20:08.295718Z"
                 }
             },
             "outputs": [],
             "source": [
-                "from time import time"
+                "rm LOG.log"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
-            "id": "8a6da5cd",
+            "id": "4c06ea42",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-06-26T20:23:18.936977Z",
-                    "start_time": "2023-06-26T20:23:18.926443Z"
+                    "end_time": "2023-06-27T08:20:08.433921Z",
+                    "start_time": "2023-06-27T08:20:08.428526Z"
                 }
             },
             "outputs": [
                 {
-                    "data": {
-                        "text/plain": [
-                            "3.409385681152344e-05"
-                        ]
-                    },
-                    "execution_count": 13,
-                    "metadata": {},
-                    "output_type": "execute_result"
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "Error occurred while printing pyDecLog\n"
+                    ]
+                }
+            ],
+            "source": [
+                "from pyDecLog import lprint\n",
+                "\n",
+                "try:\n",
+                "    printf(\"GeeksforGeeks\")\n",
+                "except Exception as Argument:\n",
+                "    # Equivalent to logging.exception(\"Error occurred while printing pyDecLog\")    \n",
+                "    lprint(console_log_level=\"error\").error(\"Error occurred while printing pyDecLog\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 14,
+            "id": "01442a6c",
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2023-06-27T08:20:08.562108Z",
+                    "start_time": "2023-06-27T08:20:08.435722Z"
+                }
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "2023/06/27 | 09:20:08 | ERROR Error occurred while printing pyDecLog\r\n"
+                    ]
                 }
             ],
             "source": [
-                "a = time()\n",
-                "b = time()\n",
-                "b-a"
+                "cat LOG.log"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "bb2c6349",
+            "id": "7ecbab2c",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `pyDecLog-0.1.4/examples/multiple_decorators/multiple_decorators.ipynb` & `pyDecLog-0.1.5/examples/multiple_decorators/multiple_decorators.ipynb`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/examples/workflow/workflow.py` & `pyDecLog-0.1.5/examples/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/pyDecLog.egg-info/PKG-INFO` & `pyDecLog-0.1.5/pyDecLog.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: pyDecLog
-Version: 0.1.4
-Summary: pyDecLog: a python package for logging via decorators 
+Version: 0.1.5
+Summary: pyDecLog: a Python module for logging via decorators
 Home-page: https://github.com/kyaiooiayk/pyDecLog
 Author: kyaiooiayk
 Author-email: kayaiooiayk@email.com
 License: MIT
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyDecLog
-pyDecLog: a simple and easy to use Python package for logging via decorators.
+
+[![PyPI Version](https://img.shields.io/pypi/v/pyDecLog.svg)](https://pypi.org/project/dython/)
+[![Python Version](https://img.shields.io/pypi/pyversions/pyDecLog.svg)](https://pypi.org/project/dython/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/pyDecLog)](https://pypistats.org/packages/pyDecLog)
+[![License](https://img.shields.io/pypi/l/pyDecLog)](https://github.com/kyaiooiayk/pyDecLog/blob/master/LICENSE)
+
+pyDecLog: a simple and easy to use Python module for logging via decorators.
 ***
 
 ## 🚀Quick start
 - Say we have the following workflow
 ```python
 from pyDecLog import arguments as arg
 from pyDecLog import signature as sign
@@ -77,17 +84,16 @@
 
 ## 🚀Useful for
 - Keep track of Python pipelines.
 - Log info about a function during development both on python script or jupyter notebook.
 ***
 
 ## ⚙️Installation
-- Create your own virtual environment and run `pip install -r requirements.txt`, then choose one of the following options:
-  - Option 1, via pip: `pip install pydeclog` 
-  - Option 2, from source: `pip install git+https://github.com/kayaiooiayk/pydeclog.git`
+- Create your own virtual environment and run `pip install -r requirements.txt`
+- Via pip: `pip install pyDecLog`   
 ***
 
 ## 🔗Dependencies
 - PyDevLog requires Python 3.5 or higher, and the following packages:
   - `pympler`
   - `numpy`
 ***
@@ -153,19 +159,20 @@
 - See the `examples` folder.
 ***
 
 ## 📚References
 - [Decorators with parameters?](https://stackoverflow.com/questions/5929107/decorators-with-parameters)
 - [How to expose persistent local variables? Part#1](https://code.activestate.com/recipes/577283-decorator-to-expose-local-variables-of-a-function-/)
 - [How to expose persistent local variables? Part#2](https://stackoverflow.com/questions/9186395/python-is-there-a-way-to-get-a-local-function-variable-from-within-a-decorator)
+- [How to time your code](https://stackoverflow.com/questions/17579357/time-time-vs-timeit-timeit)
 ***
 
 ## 📝Changelog
 - `0.1.4`  first release (26/06/23).
-- ***
+***
 
 ## 📝To-do
 - There is no planned development.
 ***
 
 ## 🪪License
 - MIT License
```

### Comparing `pyDecLog-0.1.4/pyDecLog.egg-info/SOURCES.txt` & `pyDecLog-0.1.5/pyDecLog.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 .flake8
+.gitattributes
 .gitignore
 .pre-commit-config.yaml
 LICENSE
-PyDecLog.py
 README.md
 __init__.py
 pyDecLog.py
 pyproject.toml
+requirements.txt
 setup.py
 update_github.sh
 examples/@arguments/@arguments.ipynb
 examples/@description/@description.ipynb
 examples/@memory/@memory.ipynb
 examples/@message/@message.ipynb
 examples/@profile_locals/@profile_locals.ipynb
```

### Comparing `pyDecLog-0.1.4/tests/test_arguments.py` & `pyDecLog-0.1.5/tests/test_arguments.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/tests/test_description.py` & `pyDecLog-0.1.5/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/tests/test_get_log_and_level.py` & `pyDecLog-0.1.5/tests/test_get_log_and_level.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/tests/test_get_memory.py` & `pyDecLog-0.1.5/tests/test_get_memory.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/tests/test_get_time.py` & `pyDecLog-0.1.5/tests/test_get_time.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/tests/test_lprint.py` & `pyDecLog-0.1.5/tests/test_lprint.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/tests/test_memory.py` & `pyDecLog-0.1.5/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/tests/test_message.py` & `pyDecLog-0.1.5/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/tests/test_profile_locals.py` & `pyDecLog-0.1.5/tests/test_profile_locals.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/tests/test_signature.py` & `pyDecLog-0.1.5/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/tests/test_timing.py` & `pyDecLog-0.1.5/tests/test_timing.py`

 * *Files identical despite different names*

### Comparing `pyDecLog-0.1.4/tests/test_typing.py` & `pyDecLog-0.1.5/tests/test_typing.py`

 * *Files identical despite different names*

