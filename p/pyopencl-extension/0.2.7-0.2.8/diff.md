# Comparing `tmp/pyopencl-extension-0.2.7.tar.gz` & `tmp/pyopencl-extension-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopencl-extension-0.2.7.tar", last modified: Wed May 24 12:37:32 2023, max compression
+gzip compressed data, was "pyopencl-extension-0.2.8.tar", last modified: Tue Jun 27 14:43:58 2023, max compression
```

## Comparing `pyopencl-extension-0.2.7.tar` & `pyopencl-extension-0.2.8.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 12:37:32.342010 pyopencl-extension-0.2.7/
--rw-rw-rw-   0        0        0     1994 2021-02-20 16:14:08.000000 pyopencl-extension-0.2.7/.gitignore
--rw-rw-rw-   0        0        0     1084 2022-10-04 15:29:34.000000 pyopencl-extension-0.2.7/LICENSE
--rw-rw-rw-   0        0        0     3333 2023-05-24 12:37:32.342010 pyopencl-extension-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     2583 2022-10-04 15:29:34.000000 pyopencl-extension-0.2.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-24 12:37:32.279517 pyopencl-extension-0.2.7/examples/
--rw-rw-rw-   0        0        0        0 2021-02-04 18:19:20.000000 pyopencl-extension-0.2.7/examples/__init__.py
--rw-rw-rw-   0        0        0      515 2021-11-16 11:51:09.000000 pyopencl-extension-0.2.7/examples/minimal.py
-drwxrwxrwx   0        0        0        0 2023-05-24 12:37:32.279517 pyopencl-extension-0.2.7/pyopencl_extension/
--rw-rw-rw-   0        0        0     1292 2023-05-24 12:36:22.000000 pyopencl-extension-0.2.7/pyopencl_extension/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 12:37:32.295137 pyopencl-extension-0.2.7/pyopencl_extension/components/
--rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.7/pyopencl_extension/components/__init__.py
--rw-rw-rw-   0        0        0    13458 2023-01-16 12:36:15.000000 pyopencl-extension-0.2.7/pyopencl_extension/components/copy_array_region.py
--rw-rw-rw-   0        0        0    23764 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.7/pyopencl_extension/components/fft.py
--rw-rw-rw-   0        0        0       61 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.7/pyopencl_extension/components/pytest.ini
--rw-rw-rw-   0        0        0     4241 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.7/pyopencl_extension/components/sumalongaxis.py
--rw-rw-rw-   0        0        0     3893 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.7/pyopencl_extension/components/transpose.py
--rw-rw-rw-   0        0        0    40168 2023-03-23 11:16:57.000000 pyopencl-extension-0.2.7/pyopencl_extension/emulation.py
--rw-rw-rw-   0        0        0    42315 2023-03-02 10:19:10.000000 pyopencl-extension-0.2.7/pyopencl_extension/framework.py
-drwxrwxrwx   0        0        0        0 2023-05-24 12:37:32.310760 pyopencl-extension-0.2.7/pyopencl_extension/helpers/
--rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.7/pyopencl_extension/helpers/__init__.py
--rw-rw-rw-   0        0        0     1048 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.7/pyopencl_extension/helpers/general.py
--rw-rw-rw-   0        0        0      605 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.7/pyopencl_extension/helpers/setup_pyopencl.py
-drwxrwxrwx   0        0        0        0 2023-05-24 12:37:32.310760 pyopencl-extension-0.2.7/pyopencl_extension/modifications_pyopencl/
--rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.7/pyopencl_extension/modifications_pyopencl/__init__.py
--rw-rw-rw-   0        0        0     2737 2022-06-22 15:19:37.000000 pyopencl-extension-0.2.7/pyopencl_extension/modifications_pyopencl/array.py
--rw-rw-rw-   0        0        0     4862 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.7/pyopencl_extension/modifications_pyopencl/cltypes.py
--rw-rw-rw-   0        0        0     9483 2023-05-24 12:07:46.000000 pyopencl-extension-0.2.7/pyopencl_extension/modifications_pyopencl/command_queue.py
--rw-rw-rw-   0        0        0     1378 2022-02-18 12:09:00.000000 pyopencl-extension-0.2.7/pyopencl_extension/modifications_pyopencl/context.py
-drwxrwxrwx   0        0        0        0 2023-05-24 12:37:32.326393 pyopencl-extension-0.2.7/pyopencl_extension/types/
--rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.7/pyopencl_extension/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 12:37:32.326393 pyopencl-extension-0.2.7/pyopencl_extension/types/auto_gen/
--rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.7/pyopencl_extension/types/auto_gen/__init__.py
--rw-rw-rw-   0        0        0     3155 2023-02-12 21:05:55.000000 pyopencl-extension-0.2.7/pyopencl_extension/types/auto_gen/cl_types.py
--rw-rw-rw-   0        0        0     1399 2023-02-12 21:05:55.000000 pyopencl-extension-0.2.7/pyopencl_extension/types/auto_gen/cl_types_import.py
--rw-rw-rw-   0        0        0     3706 2023-02-12 21:05:53.000000 pyopencl-extension-0.2.7/pyopencl_extension/types/auto_gen/generate_files.py
--rw-rw-rw-   0        0        0     2014 2023-02-12 21:05:55.000000 pyopencl-extension-0.2.7/pyopencl_extension/types/auto_gen/types_for_emulation.py
--rw-rw-rw-   0        0        0     5159 2022-06-01 11:28:11.000000 pyopencl-extension-0.2.7/pyopencl_extension/types/funcs_for_emulation.py
--rw-rw-rw-   0        0        0    12075 2021-11-17 18:50:32.000000 pyopencl-extension-0.2.7/pyopencl_extension/types/type_handler.py
--rw-rw-rw-   0        0        0     7414 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.7/pyopencl_extension/types/utilities_np_cl.py
-drwxrwxrwx   0        0        0        0 2023-05-24 12:37:32.295137 pyopencl-extension-0.2.7/pyopencl_extension.egg-info/
--rw-rw-rw-   0        0        0     3333 2023-05-24 12:37:32.000000 pyopencl-extension-0.2.7/pyopencl_extension.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1750 2023-05-24 12:37:32.000000 pyopencl-extension-0.2.7/pyopencl_extension.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 12:37:32.000000 pyopencl-extension-0.2.7/pyopencl_extension.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-05-24 12:37:32.000000 pyopencl-extension-0.2.7/pyopencl_extension.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-24 12:37:32.000000 pyopencl-extension-0.2.7/pyopencl_extension.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 12:37:32.342010 pyopencl-extension-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     5529 2023-05-24 12:36:22.000000 pyopencl-extension-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 12:37:32.342010 pyopencl-extension-0.2.7/tests/
--rw-rw-rw-   0        0        0        0 2020-04-20 11:14:23.000000 pyopencl-extension-0.2.7/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2021-11-16 10:28:59.000000 pyopencl-extension-0.2.7/tests/conftest.py
--rw-rw-rw-   0        0        0       77 2022-07-25 11:40:17.000000 pyopencl-extension-0.2.7/tests/pytest.ini
-drwxrwxrwx   0        0        0        0 2023-05-24 12:37:32.342010 pyopencl-extension-0.2.7/tests/test_components/
--rw-rw-rw-   0        0        0        0 2021-02-04 17:45:00.000000 pyopencl-extension-0.2.7/tests/test_components/__init__.py
--rw-rw-rw-   0        0        0     2532 2021-11-16 11:30:31.000000 pyopencl-extension-0.2.7/tests/test_components/test_copy_array_region.py
--rw-rw-rw-   0        0        0     4597 2021-11-16 11:33:33.000000 pyopencl-extension-0.2.7/tests/test_components/test_fft.py
--rw-rw-rw-   0        0        0      807 2021-11-16 11:35:44.000000 pyopencl-extension-0.2.7/tests/test_components/test_sum.py
--rw-rw-rw-   0        0        0     1368 2021-11-16 11:36:28.000000 pyopencl-extension-0.2.7/tests/test_components/test_transpose.py
--rw-rw-rw-   0        0        0    21012 2023-03-23 11:16:32.000000 pyopencl-extension-0.2.7/tests/test_emulation.py
--rw-rw-rw-   0        0        0    13125 2023-05-24 12:36:43.000000 pyopencl-extension-0.2.7/tests/test_framework.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:43:58.232654 pyopencl-extension-0.2.8/
+-rw-rw-rw-   0        0        0     1994 2021-02-20 16:14:08.000000 pyopencl-extension-0.2.8/.gitignore
+-rw-rw-rw-   0        0        0     1084 2022-10-04 15:29:34.000000 pyopencl-extension-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0     3333 2023-06-27 14:43:58.226885 pyopencl-extension-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2583 2022-10-04 15:29:34.000000 pyopencl-extension-0.2.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-27 14:43:58.154755 pyopencl-extension-0.2.8/examples/
+-rw-rw-rw-   0        0        0        0 2021-02-04 18:19:20.000000 pyopencl-extension-0.2.8/examples/__init__.py
+-rw-rw-rw-   0        0        0      515 2021-11-16 11:51:09.000000 pyopencl-extension-0.2.8/examples/minimal.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:43:58.154755 pyopencl-extension-0.2.8/pyopencl_extension/
+-rw-rw-rw-   0        0        0     1292 2023-05-24 12:36:22.000000 pyopencl-extension-0.2.8/pyopencl_extension/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:43:58.170376 pyopencl-extension-0.2.8/pyopencl_extension/components/
+-rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.8/pyopencl_extension/components/__init__.py
+-rw-rw-rw-   0        0        0    13458 2023-01-16 12:36:15.000000 pyopencl-extension-0.2.8/pyopencl_extension/components/copy_array_region.py
+-rw-rw-rw-   0        0        0    23764 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.8/pyopencl_extension/components/fft.py
+-rw-rw-rw-   0        0        0       61 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.8/pyopencl_extension/components/pytest.ini
+-rw-rw-rw-   0        0        0     4241 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.8/pyopencl_extension/components/sumalongaxis.py
+-rw-rw-rw-   0        0        0     3893 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.8/pyopencl_extension/components/transpose.py
+-rw-rw-rw-   0        0        0    40452 2023-06-26 14:51:40.000000 pyopencl-extension-0.2.8/pyopencl_extension/emulation.py
+-rw-rw-rw-   0        0        0    42315 2023-03-02 10:19:10.000000 pyopencl-extension-0.2.8/pyopencl_extension/framework.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:43:58.185998 pyopencl-extension-0.2.8/pyopencl_extension/helpers/
+-rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.8/pyopencl_extension/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1048 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.8/pyopencl_extension/helpers/general.py
+-rw-rw-rw-   0        0        0      605 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.8/pyopencl_extension/helpers/setup_pyopencl.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:43:58.185998 pyopencl-extension-0.2.8/pyopencl_extension/modifications_pyopencl/
+-rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.8/pyopencl_extension/modifications_pyopencl/__init__.py
+-rw-rw-rw-   0        0        0     2737 2022-06-22 15:19:37.000000 pyopencl-extension-0.2.8/pyopencl_extension/modifications_pyopencl/array.py
+-rw-rw-rw-   0        0        0     4862 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.8/pyopencl_extension/modifications_pyopencl/cltypes.py
+-rw-rw-rw-   0        0        0     9483 2023-05-24 12:07:46.000000 pyopencl-extension-0.2.8/pyopencl_extension/modifications_pyopencl/command_queue.py
+-rw-rw-rw-   0        0        0     1378 2022-02-18 12:09:00.000000 pyopencl-extension-0.2.8/pyopencl_extension/modifications_pyopencl/context.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:43:58.201619 pyopencl-extension-0.2.8/pyopencl_extension/types/
+-rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.8/pyopencl_extension/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:43:58.201619 pyopencl-extension-0.2.8/pyopencl_extension/types/auto_gen/
+-rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.8/pyopencl_extension/types/auto_gen/__init__.py
+-rw-rw-rw-   0        0        0     3155 2023-02-12 21:05:55.000000 pyopencl-extension-0.2.8/pyopencl_extension/types/auto_gen/cl_types.py
+-rw-rw-rw-   0        0        0     1399 2023-02-12 21:05:55.000000 pyopencl-extension-0.2.8/pyopencl_extension/types/auto_gen/cl_types_import.py
+-rw-rw-rw-   0        0        0     3706 2023-02-12 21:05:53.000000 pyopencl-extension-0.2.8/pyopencl_extension/types/auto_gen/generate_files.py
+-rw-rw-rw-   0        0        0     2014 2023-02-12 21:05:55.000000 pyopencl-extension-0.2.8/pyopencl_extension/types/auto_gen/types_for_emulation.py
+-rw-rw-rw-   0        0        0     5188 2023-06-26 10:28:32.000000 pyopencl-extension-0.2.8/pyopencl_extension/types/funcs_for_emulation.py
+-rw-rw-rw-   0        0        0    12075 2021-11-17 18:50:32.000000 pyopencl-extension-0.2.8/pyopencl_extension/types/type_handler.py
+-rw-rw-rw-   0        0        0     7414 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.8/pyopencl_extension/types/utilities_np_cl.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:43:58.170376 pyopencl-extension-0.2.8/pyopencl_extension.egg-info/
+-rw-rw-rw-   0        0        0     3333 2023-06-27 14:43:57.000000 pyopencl-extension-0.2.8/pyopencl_extension.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1750 2023-06-27 14:43:58.000000 pyopencl-extension-0.2.8/pyopencl_extension.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 14:43:57.000000 pyopencl-extension-0.2.8/pyopencl_extension.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-06-27 14:43:57.000000 pyopencl-extension-0.2.8/pyopencl_extension.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-27 14:43:57.000000 pyopencl-extension-0.2.8/pyopencl_extension.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 14:43:58.233531 pyopencl-extension-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     5531 2023-06-27 14:42:49.000000 pyopencl-extension-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 14:43:58.217240 pyopencl-extension-0.2.8/tests/
+-rw-rw-rw-   0        0        0        0 2020-04-20 11:14:23.000000 pyopencl-extension-0.2.8/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-11-16 10:28:59.000000 pyopencl-extension-0.2.8/tests/conftest.py
+-rw-rw-rw-   0        0        0       77 2022-07-25 11:40:17.000000 pyopencl-extension-0.2.8/tests/pytest.ini
+drwxrwxrwx   0        0        0        0 2023-06-27 14:43:58.226885 pyopencl-extension-0.2.8/tests/test_components/
+-rw-rw-rw-   0        0        0        0 2021-02-04 17:45:00.000000 pyopencl-extension-0.2.8/tests/test_components/__init__.py
+-rw-rw-rw-   0        0        0     2532 2021-11-16 11:30:31.000000 pyopencl-extension-0.2.8/tests/test_components/test_copy_array_region.py
+-rw-rw-rw-   0        0        0     4597 2021-11-16 11:33:33.000000 pyopencl-extension-0.2.8/tests/test_components/test_fft.py
+-rw-rw-rw-   0        0        0      807 2021-11-16 11:35:44.000000 pyopencl-extension-0.2.8/tests/test_components/test_sum.py
+-rw-rw-rw-   0        0        0     1368 2021-11-16 11:36:28.000000 pyopencl-extension-0.2.8/tests/test_components/test_transpose.py
+-rw-rw-rw-   0        0        0    21816 2023-06-27 14:42:28.000000 pyopencl-extension-0.2.8/tests/test_emulation.py
+-rw-rw-rw-   0        0        0    13125 2023-05-24 12:36:43.000000 pyopencl-extension-0.2.8/tests/test_framework.py
```

### Comparing `pyopencl-extension-0.2.7/.gitignore` & `pyopencl-extension-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/LICENSE` & `pyopencl-extension-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/PKG-INFO` & `pyopencl-extension-0.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencl-extension
-Version: 0.2.7
+Version: 0.2.8
 Summary: This package extends PyOpenCl by providing an object-oriented kernel programming framework and debugging capabilities.
 Home-page: https://github.com/philipp-mohr/pyopencl-extension
 Author: P.Mohr
 Author-email: philipp.mohr@tuhh.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyopencl-extension-0.2.7/README.rst` & `pyopencl-extension-0.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/examples/minimal.py` & `pyopencl-extension-0.2.8/examples/minimal.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/__init__.py` & `pyopencl-extension-0.2.8/pyopencl_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/components/copy_array_region.py` & `pyopencl-extension-0.2.8/pyopencl_extension/components/copy_array_region.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/components/fft.py` & `pyopencl-extension-0.2.8/pyopencl_extension/components/fft.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/components/sumalongaxis.py` & `pyopencl-extension-0.2.8/pyopencl_extension/components/sumalongaxis.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/components/transpose.py` & `pyopencl-extension-0.2.8/pyopencl_extension/components/transpose.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/emulation.py` & `pyopencl-extension-0.2.8/pyopencl_extension/emulation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+import logging
 import os
 import re
 from collections import namedtuple
 from dataclasses import dataclass, field
 from pathlib import Path
 from textwrap import indent
 from typing import Tuple, List
@@ -205,256 +206,314 @@
     """
     args = ', '.join(['{}'.format(p.name) if not any(q in ['local', '__local'] for q in p.quals)
                       else f'{p.name}: {_unparse(p.type.type.type.names[0])}'
                       for p in node.args.params])
     return _unparse_header(args, node)
 
 
-def _unparse(node: Node) -> Container:
-    if isinstance(node, FuncDef):
-        # check if function is kernel
+def _deal_with_func_def_node(node):
+    # check if function is kernel
 
-        if len(node.decl.funcspec) > 0:
-            if node.decl.funcspec[0] == '__kernel':
-                header = _unparse_knl_header(node.decl.type)
-                header = f'@cl_kernel\n{header}'
-            else:
-                raise ValueError('Func spec not supported')
+    if len(node.decl.funcspec) > 0:
+        if node.decl.funcspec[0] == '__kernel':
+            header = _unparse_knl_header(node.decl.type)
+            header = f'@cl_kernel\n{header}'
         else:
-            header = _unparse(node.decl.type)
+            raise ValueError('Func spec not supported')
+    else:
+        header = _unparse(node.decl.type)
 
-        body = _unparse(node.body)
-        final_yield = ''
-        if len(node.decl.funcspec) > 0:
-            if node.decl.funcspec[0] == '__kernel':
-                final_yield = py_indent('yield  # required to model local memory behaviour correctly')
-        if final_yield == '':
-            function = '{}\n{}'.format(header, py_indent(body))
-        else:
-            function = '{}\n{}\n{}'.format(header, py_indent(body), final_yield)
-        res = function
-    elif isinstance(node, FuncDeclExt):
-        res = _unparse_func_header(node)
-    elif isinstance(node, TypeDecl):
-        res = node.declname
-    elif isinstance(node, FuncCall):
-        if isinstance(node.name, ID):
-            func_name = node.name.name
-            # todo: use funcs_for_cl_emulation.py for adding support for all cl functions
-            if func_name.startswith('convert_'):
-                """
-                alternative:
-                def convert(value, dtype='int32'):
-                    return np.dtype(dtype).type(value)
-                """
-                type_name = re.search(r'(convert_)([\w]+)', node.name.name).group(2)
-                res = '{}({})'.format(type_name, _unparse(node.args))
-            elif 'cos' == func_name:
-                res = 'np.cos({})'.format(_unparse(node.args))
-            elif 'sin' == func_name:
-                res = 'np.sin({})'.format(_unparse(node.args))
-            elif func_name in translation_cl_work_item_functions:
-                res = 'wi.{}[{}]'.format(translation_cl_work_item_functions[func_name], _unparse(node.args))
-            elif 'barrier' == func_name:
-                if isinstance((_ := node.args.exprs[0]), BinaryOp):
-                    barrier_name = f'{node.args.exprs[0].left.name}|{node.args.exprs[0].right.name}'
-                else:
-                    barrier_name = node.args.exprs[0].name
-                res = f'\nwi.scope = locals()  # saves reference to objects in scope for debugging other wi in wg \n' \
-                      f'yield  # yield models the behaviour of barrier({barrier_name})\n'
+    body = _unparse(node.body)
+    final_yield = ''
+    if len(node.decl.funcspec) > 0:
+        if node.decl.funcspec[0] == '__kernel':
+            final_yield = py_indent('yield  # required to model local memory behaviour correctly')
+    if final_yield == '':
+        function = '{}\n{}'.format(header, py_indent(body))
+    else:
+        function = '{}\n{}\n{}'.format(header, py_indent(body), final_yield)
+    return function
+
+
+def _deal_with_func_call(node: FuncCall):
+    if isinstance(node.name, ID):
+        func_name = node.name.name
+        # todo: use funcs_for_cl_emulation.py for adding support for all cl functions
+        if func_name.startswith('convert_'):
+            """
+            alternative:
+            def convert(value, dtype='int32'):
+                return np.dtype(dtype).type(value)
+            """
+            type_name = re.search(r'(convert_)([\w]+)', node.name.name).group(2)
+            res = '{}({})'.format(type_name, _unparse(node.args))
+        elif 'cos' == func_name:
+            res = 'np.cos({})'.format(_unparse(node.args))
+        elif 'sin' == func_name:
+            res = 'np.sin({})'.format(_unparse(node.args))
+        elif func_name in translation_cl_work_item_functions:
+            res = 'wi.{}[{}]'.format(translation_cl_work_item_functions[func_name], _unparse(node.args))
+        elif 'barrier' == func_name:
+            if isinstance((_ := node.args.exprs[0]), BinaryOp):
+                barrier_name = f'{node.args.exprs[0].left.name}|{node.args.exprs[0].right.name}'
             else:
-                if func_name in (_ := MacroWithArguments.names_py_macro):
-                    args = _unparse(node.args).split(', ')
-                    format_arg = ', '.join([f'{macro_arg}="{args[i]}"' for i, macro_arg in enumerate(_[func_name])])
-                    res = f'exec({func_name}.format({format_arg}))'
-                elif func_name in names_func_require_work_item:
-                    res = '{}({}, wi=wi)'.format(_unparse(node.name), _unparse(node.args))
-                    if func_name in names_func_has_barrier:
-                        res = f'(yield from {res})'
-                else:
-                    res = '{}({})'.format(_unparse(node.name), _unparse(node.args))
+                barrier_name = node.args.exprs[0].name
+            res = f'\nwi.scope = locals()  # saves reference to objects in scope for debugging other wi in wg \n' \
+                  f'yield  # yield models the behaviour of barrier({barrier_name})\n'
         else:
-            res = '{}({})'.format(_unparse(node.name), _unparse(node.args))
-    elif isinstance(node, ExprList):
-        res = ', '.join([_unparse(expr) for expr in node.exprs])
-    elif isinstance(node, Compound):  # e.g. body of a function or a for loop
-        # compound = [_unparse(block_item) for block_item in node.block_items]
-        # loop makes debugging easier. Set breakpoint in loop, then remove BP and step over to get to target line
-        compound = []
-        for block_item in node.block_items:
-            if isinstance(block_item, UnaryOp):  # number++; should translate to number +=1 and not numbernumber+=1
-                compound.append(_unparse(block_item).only_use_prefix_postfix())
+            if func_name in (_ := MacroWithArguments.names_py_macro):
+                args = _unparse(node.args).split(', ')
+                format_arg = ', '.join([f'{macro_arg}="{args[i]}"' for i, macro_arg in enumerate(_[func_name])])
+                res = f'exec({func_name}.format({format_arg}))'
+            elif func_name in names_func_require_work_item:
+                res = '{}({}, wi=wi)'.format(_unparse(node.name), _unparse(node.args))
+                if func_name in names_func_has_barrier:
+                    res = f'(yield from {res})'
             else:
-                compound.append(_unparse(block_item).wrap_code_with_prefix_postfix())
-        res = '\n'.join(compound)
-    elif isinstance(node, ArrayRef):
-        # if isinstance(node.subscript, UnaryOp):  # e.g. array[pos++] = 5; -> pos+=1; \n array[pos] = 5;
-        #     unary_op = _unparse(node.subscript)
-        #     res = '{}[{}]'.format(_unparse(node.name), node.subscript.expr.name)
-        # else:
-        array_index = _unparse(node.subscript)
-        res = Container('{}[{}]'.format(_unparse(node.name), array_index))
-        res.add_container_pre_post_fix(array_index)
-    elif isinstance(node, For):
-        # only for loop considered of style: for(int i=start; i<=stop; i++)
-        #                                 or for(int i>=stop; i>=0; i--)
-        detect_inconsistent_for_loop_header_variable(node)
-
-        var = node.init.decls[0].name
-        right = _unparse(node.cond.right)
-        left = _unparse(node.cond.left)
-        cond_op = node.cond.op
-        if right == var:  # e.g. 5>=i -> i<= 5
-            right = left
-            left = var
-            cond_op = {'!=': '!=',
-                       '<=': '>=',
-                       '>=': '<=',
-                       '>': '<',
-                       '<': '>'}[cond_op]
-        stop = right
-        op = node.next.op
-        stop = {'p++': {'!=': stop,
-                        '<': stop,
-                        '<=': stop + '+1'},
-                'p--': {'!=': stop,
-                        '>': stop,
-                        '>=': stop + '-1'}}[op][cond_op]
-        if op == 'p++':
-            step = 1
-        elif op == 'p--':
-            step = -1
-        else:
-            raise NotImplementedError()
-        loop_header = '{var} in range({start}, {stop}, {step})'.format(var=var,
-                                                                       start=_unparse(node.init.decls[0].init),
-                                                                       stop=stop,
-                                                                       step=step)
-        loop_body = _unparse(node.stmt)
-        res = 'for {}:\n{}'.format(loop_header, py_indent(loop_body))
-    elif isinstance(node, While):
-        res = 'while {}:\n{}'.format(_unparse(node.cond), py_indent(_unparse(node.stmt)))
-    elif isinstance(node, Break):
-        res = 'break'
-    elif isinstance(node, If):
-        if_true_cond = '{}'.format(_unparse(node.cond))
-        if_true_body = _unparse(node.iftrue)
-        if_true = 'if {}:\n{}'.format(if_true_cond, py_indent(if_true_body))
-        if node.iffalse is not None:
-            else_body = _unparse(node.iffalse)
-            else_ = 'else:\n{}'.format(py_indent(else_body))
-            res = '{}\n{}'.format(if_true, else_)
+                res = '{}({})'.format(_unparse(node.name), _unparse(node.args))
+    else:
+        res = '{}({})'.format(_unparse(node.name), _unparse(node.args))
+    return res
+
+
+def _deal_with_compound(node: Compound):
+    # compound = [_unparse(block_item) for block_item in node.block_items]
+    # loop makes debugging easier. Set breakpoint in loop, then remove BP and step over to get to target line
+    compound = []
+    for block_item in node.block_items:
+        if isinstance(block_item, UnaryOp):  # number++; should translate to number +=1 and not numbernumber+=1
+            compound.append(_unparse(block_item).only_use_prefix_postfix())
         else:
-            res = if_true
-    elif isinstance(node, Decl):
-        if len(node.quals) > 0 and node.quals[0] == 'private':  # private int indices_states_prior[ALPHABET_SIZE];
+            compound.append(_unparse(block_item).wrap_code_with_prefix_postfix())
+    res = '\n'.join(compound)
+    return res
+
+
+def _deal_with_arrayref(node: ArrayRef):
+    # if isinstance(node.subscript, UnaryOp):  # e.g. array[pos++] = 5; -> pos+=1; \n array[pos] = 5;
+    #     unary_op = _unparse(node.subscript)
+    #     res = '{}[{}]'.format(_unparse(node.name), node.subscript.expr.name)
+    # else:
+    array_index = _unparse(node.subscript)
+    res = Container('{}[{}]'.format(_unparse(node.name), array_index))
+    res.add_container_pre_post_fix(array_index)
+    return res
+
+
+def _deal_with_for(node: For):
+    # only for loop considered of style: for(int i=start; i<=stop; i++)
+    #                                 or for(int i>=stop; i>=0; i--)
+    detect_inconsistent_for_loop_header_variable(node)
+
+    var = node.init.decls[0].name
+    right = _unparse(node.cond.right)
+    left = _unparse(node.cond.left)
+    cond_op = node.cond.op
+    if right == var:  # e.g. 5>=i -> i<= 5
+        right = left
+        left = var
+        cond_op = {'!=': '!=',
+                   '<=': '>=',
+                   '>=': '<=',
+                   '>': '<',
+                   '<': '>'}[cond_op]
+    stop = right
+    op = node.next.op
+    stop = {'p++': {'!=': stop,
+                    '<': stop,
+                    '<=': stop + '+1'},
+            'p--': {'!=': stop,
+                    '>': stop,
+                    '>=': stop + '-1'}}[op][cond_op]
+    if op == 'p++':
+        step = 1
+    elif op == 'p--':
+        step = -1
+    else:
+        raise NotImplementedError()
+    loop_header = '{var} in range({start}, {stop}, {step})'.format(var=var,
+                                                                   start=_unparse(node.init.decls[0].init),
+                                                                   stop=stop,
+                                                                   step=step)
+    loop_body = _unparse(node.stmt)
+    res = 'for {}:\n{}'.format(loop_header, py_indent(loop_body))
+    return res
+
+
+def _deal_with_if(node: If):
+    if_true_cond = '{}'.format(_unparse(node.cond))
+    if_true_body = _unparse(node.iftrue)
+    if_true = 'if {}:\n{}'.format(if_true_cond, py_indent(if_true_body))
+    if node.iffalse is not None:
+        else_body = _unparse(node.iffalse)
+        else_ = 'else:\n{}'.format(py_indent(else_body))
+        res = '{}\n{}'.format(if_true, else_)
+    else:
+        res = if_true
+    return res
+
+
+def _deal_with_decl(node: Decl):
+    if len(node.quals) > 0 and node.quals[0] == 'private':  # private int indices_states_prior[ALPHABET_SIZE];
+        res = _unparse(node.type)
+    elif isinstance(node.type, ArrayDecl):
+        if node.init is None:  # real_t p_x[2];
             res = _unparse(node.type)
-        elif isinstance(node.type, ArrayDecl):
-            if node.init is None:  # real_t p_x[2];
-                res = _unparse(node.type)
-            elif isinstance(node.init, InitList):  # real_t p_x[2]={0.0};
-                # todo: if array /var is not inialized assign random values or give warning
-                array_decl = _unparse(node.type)
-                array_fill = [_unparse(item) for item in node.init.exprs]
-                # todo: deal with a[5]={1}->a=[1,0,0,0,0} node.type.dim.value == 1 and len(array_fill) == 1 and int(array_fill) != 0:
-                if len(array_fill) == 1 and array_fill[0] in ['0', '0.0']:
-                    res = '{}\n{}.fill({})'.format(array_decl, node.type.type.declname, array_fill[0])
-                else:
-                    raise ValueError('Currently array initializer with multiple or non zero values not supported')
-        elif node.init is None:
-            if isinstance(node.type, PtrDecl):  # e.g. float *x;
-                res = f'{node.name} = {node.type.type.type.names[0]}(0)'
-            else:  # e.g. float x;
-                res = f'{node.name} = {node.type.type.names[0]}(0)'
-        else:  # int gid1=get_global_id(0);
-            if isinstance(node.type, PtrDecl):
-                type_cl = node.type.type.type.names[0]
+        elif isinstance(node.init, InitList):  # real_t p_x[2]={0.0};
+            # todo: if array /var is not inialized assign random values or give warning
+            array_decl = _unparse(node.type)
+            array_fill = [_unparse(item) for item in node.init.exprs]
+            # todo: deal with a[5]={1}->a=[1,0,0,0,0} node.type.dim.value == 1 and len(array_fill) == 1 and int(array_fill) != 0:
+            if len(array_fill) == 1 and array_fill[0] in ['0', '0.0']:
+                res = '{}\n{}.fill({})'.format(array_decl, node.type.type.declname, array_fill[0])
             else:
-                type_cl = node.type.type.names[0]
-            res = '{} = {}({})'.format(node.name, type_cl, _unparse(node.init))
-    elif isinstance(node, ArrayDecl):
-        if len(node.type.quals) > 0 and node.type.quals[0] in ['local', '__local']:
-            res = "{name} = local_memory(wi, '{name}', lambda: init_array({dim}, {dtype}))".format(
-                name=_unparse(node.type),
-                dim=_unparse(node.dim),
-                dtype=node.type.type.names[0])
+                raise ValueError('Currently array initializer with multiple or non zero values not supported')
         else:
-            res = f'{_unparse(node.type)} = init_array({_unparse(node.dim)}, {node.type.type.names[0]})'
-    elif isinstance(node, Assignment):
-        left = _unparse(node.lvalue)
-        right = _unparse(node.rvalue)
-        if search(regex_real_imag_assignment, left):
-            groups = search(regex_real_imag_assignment, left).groups()
-            res = Container(f'set_{groups[5]}(ary={groups[0]}, idx={groups[2]}, value={right})')
+            raise ValueError('Not supported case')
+    elif node.init is None:
+        if isinstance(node.type, PtrDecl):  # e.g. float *x;
+            res = f'{node.name} = {node.type.type.type.names[0]}(0)'
+        else:  # e.g. float x;
+            res = f'{node.name} = {node.type.type.names[0]}(0)'
+    else:  # int gid1=get_global_id(0);
+        if isinstance(node.type, PtrDecl):
+            type_cl = node.type.type.type.names[0]
         else:
-            res = Container('{} {} {}'.format(left, _unparse(node.op), right))
-            res.add_container_pre_post_fix(left)
-            res.add_container_pre_post_fix(right)
-    elif isinstance(node, Constant):
-        res = node.value
-    elif isinstance(node, Return):
-        res = 'return ' + _unparse(node.expr)
-    elif isinstance(node, BinaryOp):
-        left = _unparse(node.left)
-        right = _unparse(node.right)
-        # todo: see test_pointer_arithmetics
-        # if isinstance(node.left, ID) and node.op in ['+']:
-        #     res = f'{node.left.name}[{node.op}:]'
-        # elif isinstance(node.right, ID) and node.op in ['+']:
-        #     res = f'{node.right.name}[{node.op}:]'
-        if node.op in ['%']:
-            res = Container(f'c_modulo({left},{right})')
-        else:
-            if node.op in ['&&']:  # && not supported in python
-                node_op = '&'
-            elif node.op in ['||']:
-                node_op = 'or'
-            else:
-                node_op = node.op
-            # following lines reduce unnecessary brackets like 1+2 is not translated to (1+2) in Python equivalent
-            if isinstance(node.right, BinaryOp):
-                right = Container(f'({right})', **right.__dict__)
-            if isinstance(node.left, BinaryOp):
-                left = Container(f'({left})', **left.__dict__)
-            res = Container('{} {} {}'.format(left, node_op, right))
+            type_cl = node.type.type.names[0]
+        res = '{} = {}({})'.format(node.name, type_cl, _unparse(node.init))
+    return res
+
+
+def _deal_with_array_decl(node: ArrayDecl):
+    if len(node.type.quals) > 0 and node.type.quals[0] in ['local', '__local']:
+        res = "{name} = local_memory(wi, '{name}', lambda: init_array({dim}, {dtype}))".format(
+            name=_unparse(node.type),
+            dim=_unparse(node.dim),
+            dtype=node.type.type.names[0])
+    else:
+        res = f'{_unparse(node.type)} = init_array({_unparse(node.dim)}, {node.type.type.names[0]})'
+    return res
+
+
+def _deal_with_assignment(node: Assignment):
+    left = _unparse(node.lvalue)
+    right = _unparse(node.rvalue)
+    if search(regex_real_imag_assignment, left):
+        groups = search(regex_real_imag_assignment, left).groups()
+        res = Container(f'set_{groups[5]}(ary={groups[0]}, idx={groups[2]}, value={right})')
+    else:
+        res = Container('{} {} {}'.format(left, _unparse(node.op), right))
         res.add_container_pre_post_fix(left)
         res.add_container_pre_post_fix(right)
-    elif isinstance(node, ID):
-        res = node.name
-    elif isinstance(node, IdentifierType):
-        res = ''
-    elif isinstance(node, str):
-        res = node
-    elif isinstance(node, Cast):
-        type_cl = node.to_type.type.type.names[0]
-        res = '{}({})'.format(type_cl, _unparse(node.expr))
-    elif isinstance(node, UnaryOp):
-        if node.op == 'p++':
-            res = Container(node.expr.name, code_unary_operator_postfix=['{} += 1'.format(_unparse(node.expr))])
-            # res = '{} += 1'.format(_unparse(node.expr))
-        elif node.op == 'p--':
-            res = Container(node.expr.name, code_unary_operator_postfix=['{} -= 1'.format(_unparse(node.expr))])
-        elif node.op == '++':
-            res = Container(node.expr.name, code_unary_operator_prefix=['{} += 1'.format(_unparse(node.expr))])
-        elif node.op == '--':
-            res = Container(node.expr.name, code_unary_operator_prefix=['{} -= 1'.format(_unparse(node.expr))])
-        elif node.op == '!':
-            res = f'not {_unparse(node.expr)}'
+    return res
+
+
+def _deal_with_binary_op(node: BinaryOp):
+    left = _unparse(node.left)
+    right = _unparse(node.right)
+    # todo: see test_pointer_arithmetics
+    # if isinstance(node.left, ID) and node.op in ['+']:
+    #     res = f'{node.left.name}[{node.op}:]'
+    # elif isinstance(node.right, ID) and node.op in ['+']:
+    #     res = f'{node.right.name}[{node.op}:]'
+    if node.op in ['%']:
+        res = Container(f'c_modulo({left},{right})')
+    else:
+        if node.op in ['&&']:  # && not supported in python
+            node_op = '&'
+        elif node.op in ['||']:
+            node_op = 'or'
         else:
-            res = '{}{}'.format(node.op, _unparse(node.expr))
-    elif isinstance(node, StructRef):
-        res = f'{_unparse(node.name)}.{_unparse(node.field)}'
-    elif isinstance(node, TernaryOp):
-        res = f'{_unparse(node.iftrue)} if {_unparse(node.cond)} else {_unparse(node.iffalse)}'
-    elif isinstance(node, EmptyStatement):
-        res = 'pass'
-    elif node is None:
-        res = ''
+            node_op = node.op
+        # following lines reduce unnecessary brackets like 1+2 is not translated to (1+2) in Python equivalent
+        if isinstance(node.right, BinaryOp):
+            right = Container(f'({right})', **right.__dict__)
+        if isinstance(node.left, BinaryOp):
+            left = Container(f'({left})', **left.__dict__)
+        res = Container('{} {} {}'.format(left, node_op, right))
+    res.add_container_pre_post_fix(left)
+    res.add_container_pre_post_fix(right)
+    return res
+
+
+def _deal_with_unary_op(node: UnaryOp):
+    if node.op == 'p++':
+        res = Container(node.expr.name, code_unary_operator_postfix=['{} += 1'.format(_unparse(node.expr))])
+        # res = '{} += 1'.format(_unparse(node.expr))
+    elif node.op == 'p--':
+        res = Container(node.expr.name, code_unary_operator_postfix=['{} -= 1'.format(_unparse(node.expr))])
+    elif node.op == '++':
+        res = Container(node.expr.name, code_unary_operator_prefix=['{} += 1'.format(_unparse(node.expr))])
+    elif node.op == '--':
+        res = Container(node.expr.name, code_unary_operator_prefix=['{} -= 1'.format(_unparse(node.expr))])
+    elif node.op == '!':
+        res = f'not {_unparse(node.expr)}'
     else:
-        raise ValueError('Node type not considered')
+        res = '{}{}'.format(node.op, _unparse(node.expr))
+    return res
+
+
+def _unparse(node: Node) -> Container:
+    match node:
+        case FuncDef():
+            res = _deal_with_func_def_node(node)
+        case FuncDeclExt():
+            res = _unparse_func_header(node)
+        case TypeDecl():
+            res = node.declname
+        case FuncCall():
+            res = _deal_with_func_call(node)
+        case ExprList():
+            res = ', '.join([_unparse(expr) for expr in node.exprs])
+        case Compound(): # e.g. body of a function or a for loop
+            res = _deal_with_compound(node)
+        case ArrayRef():
+            res = _deal_with_arrayref(node)
+        case For():
+            res = _deal_with_for(node)
+        case While():
+            res = 'while {}:\n{}'.format(_unparse(node.cond), py_indent(_unparse(node.stmt)))
+        case Break():
+            res = 'break'
+        case If():
+            res = _deal_with_if(node)
+        case Decl():
+            res = _deal_with_decl(node)
+        case ArrayDecl():
+            res = _deal_with_array_decl(node)
+        case Assignment():
+            res = _deal_with_assignment(node)
+        case Constant():
+            res = node.value
+        case Return():
+            res = 'return ' + _unparse(node.expr)
+        case BinaryOp():
+            res = _deal_with_binary_op(node)
+        case ID():
+            res = node.name
+        case IdentifierType():
+            res = ''
+        case str():
+            res = node
+        case Cast():
+            type_cl = node.to_type.type.type.names[0]
+            res = '{}({})'.format(type_cl, _unparse(node.expr))
+        case UnaryOp():
+            res = _deal_with_unary_op(node)
+        case StructRef():
+            res = f'{_unparse(node.name)}.{_unparse(node.field)}'
+        case TernaryOp():
+            res = f'{_unparse(node.iftrue)} if {_unparse(node.cond)} else {_unparse(node.iffalse)}'
+        case EmptyStatement():
+            res = 'pass'
+        case None:
+            res = ''
+        case _:
+            raise ValueError('Node type not considered')
+
     if not isinstance(res, Container):
         res = Container(res)
     return res
 
 
 def unparse_function_node(node: Node) -> str:
     return str(_unparse(node))
@@ -782,15 +841,16 @@
         ==gid0
     }
     """
     rgx = '#define[ ]+([\w]+)[ ]+(get_[\w\.\-e\(\)]+)[\s\n]'
     defines_to_be_replaced = re.findall(rgx, code_c)
     code_c = re.sub(rgx, '', code_c)
     for name, val in defines_to_be_replaced:
-        code_c = re.sub('([\[\(\s\+\*\/\-\=]|==)' + f'({name})' + '([\]\)\s\+\*\/\-\;]|==)', r'\1' + val + r'\3', code_c)
+        code_c = re.sub('([\[\(\s\+\*\/\-\=]|==)' + f'({name})' + '([\]\)\s\+\*\/\-\;]|==)', r'\1' + val + r'\3',
+                        code_c)
     return code_c
 
 
 def unparse_c_code_to_python(code_c: str) -> str:
     # todo prevents files: https://stackoverflow.com/questions/12644902/how-to-prevent-table-regeneration-in-ply
     # yacc.yacc(debug=False, write_tables=False)
     code_c = re.sub('#define[ ]+TP_ROOT[ ]+(cfloat|cdouble])[ ]*(\n)', '', code_c)  # removes TP_ROOT = cfloat
@@ -854,14 +914,15 @@
     #     preamble_buff_t = preamble_buff_t_complex64_np
     # elif 'cdouble_t' in code_c:
     #     preamble_buff_t = preamble_buff_t_complex128_np
     # else:
     #     preamble_buff_t = preamble_buff_t_real_np
     #
     # preamble_buff_t = '{}\n\n{}'.format(preamble_buff_t, preamble_cl_funcs_to_lambdas)
+    # logging.info(code_py)
     return code_py
 
 
 b_use_existing_file_for_emulation = False
 
 
 def use_existing_file_for_emulation(value: bool):
@@ -908,8 +969,8 @@
 
 def compute_tuple_idx(idx_lin, dimensions):
     n_dim = len(dimensions)
     idx_tuple = [0] * n_dim
     for _i in range(n_dim):
         i = n_dim - 1 - _i
         idx_lin, idx_tuple[i] = divmod(idx_lin, dimensions[i])
-    return tuple(idx_tuple)
+    return tuple(idx_tuple)
```

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/framework.py` & `pyopencl-extension-0.2.8/pyopencl_extension/framework.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/helpers/general.py` & `pyopencl-extension-0.2.8/pyopencl_extension/helpers/general.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/helpers/setup_pyopencl.py` & `pyopencl-extension-0.2.8/pyopencl_extension/helpers/setup_pyopencl.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/modifications_pyopencl/array.py` & `pyopencl-extension-0.2.8/pyopencl_extension/modifications_pyopencl/array.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/modifications_pyopencl/cltypes.py` & `pyopencl-extension-0.2.8/pyopencl_extension/modifications_pyopencl/cltypes.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/modifications_pyopencl/command_queue.py` & `pyopencl-extension-0.2.8/pyopencl_extension/modifications_pyopencl/command_queue.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/modifications_pyopencl/context.py` & `pyopencl-extension-0.2.8/pyopencl_extension/modifications_pyopencl/context.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/types/auto_gen/cl_types.py` & `pyopencl-extension-0.2.8/pyopencl_extension/types/auto_gen/cl_types.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/types/auto_gen/cl_types_import.py` & `pyopencl-extension-0.2.8/pyopencl_extension/types/auto_gen/cl_types_import.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/types/auto_gen/generate_files.py` & `pyopencl-extension-0.2.8/pyopencl_extension/types/auto_gen/generate_files.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/types/auto_gen/types_for_emulation.py` & `pyopencl-extension-0.2.8/pyopencl_extension/types/auto_gen/types_for_emulation.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/types/funcs_for_emulation.py` & `pyopencl-extension-0.2.8/pyopencl_extension/types/funcs_for_emulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
         else:
             res = self.memory[item + self.pos]
             return VecVal(res.copy())
 
 
 sign = lambda x: np.sign(x)
 fabs = lambda x: np.abs(x)
+ceil = lambda x: np.ceil(x)
 log2 = lambda x: np.log2(x)
 sqrt = lambda x: x ** 0.5
 exp = lambda x: np.exp(x)
 log = lambda x: np.log(x)
 pow = lambda x, y: x ** y
 barrier = lambda x: x
 CLK_GLOBAL_MEM_FENCE = None
```

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/types/type_handler.py` & `pyopencl-extension-0.2.8/pyopencl_extension/types/type_handler.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension/types/utilities_np_cl.py` & `pyopencl-extension-0.2.8/pyopencl_extension/types/utilities_np_cl.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension.egg-info/PKG-INFO` & `pyopencl-extension-0.2.8/pyopencl_extension.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencl-extension
-Version: 0.2.7
+Version: 0.2.8
 Summary: This package extends PyOpenCl by providing an object-oriented kernel programming framework and debugging capabilities.
 Home-page: https://github.com/philipp-mohr/pyopencl-extension
 Author: P.Mohr
 Author-email: philipp.mohr@tuhh.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyopencl-extension-0.2.7/pyopencl_extension.egg-info/SOURCES.txt` & `pyopencl-extension-0.2.8/pyopencl_extension.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/setup.py` & `pyopencl-extension-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 NAME = 'pyopencl-extension'
 DESCRIPTION = 'This package extends PyOpenCl by providing an object-oriented kernel programming framework and ' \
               'debugging capabilities.'
 URL = 'https://github.com/philipp-mohr/pyopencl-extension'
 EMAIL = 'philipp.mohr@tuhh.de'
 AUTHOR = 'P.Mohr'
 REQUIRES_PYTHON = '>=3.10.0'
-VERSION = '0.2.7'
+VERSION = '0.2.8'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'numpy', 'pyopencl', 'mako', 'pycparser', 'pycparserext', 'pyastyle'  # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
 EXTRAS = {
     'dev': [
         'pytest',
         'check-manifest',
         'twine',
-        'reikna',
+        # 'reikna',
         'wheel'
     ]  # 'fancy feature': ['django'],
 }
 
 # Use .whl from other sources than pip?
 DEPENDENCY_LINKS = []
```

### Comparing `pyopencl-extension-0.2.7/tests/test_components/test_copy_array_region.py` & `pyopencl-extension-0.2.8/tests/test_components/test_copy_array_region.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/tests/test_components/test_fft.py` & `pyopencl-extension-0.2.8/tests/test_components/test_fft.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/tests/test_components/test_sum.py` & `pyopencl-extension-0.2.8/tests/test_components/test_sum.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/tests/test_components/test_transpose.py` & `pyopencl-extension-0.2.8/tests/test_components/test_transpose.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.7/tests/test_emulation.py` & `pyopencl-extension-0.2.8/tests/test_emulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -552,7 +552,30 @@
                                                         ((1, 2), (2, 4), 6),
                                                         ((1,), (2,), 1)])
 def test_compute_tuple_from_idx_linear(idx_tuple, dimensions, idx_lin_ref):
     idx_lin = compute_linear_idx(idx_tuple, dimensions)
     assert idx_lin == idx_lin_ref
     idx_tuple2 = compute_tuple_idx(idx_lin, dimensions)
     assert idx_tuple == idx_tuple2
+
+
+def test_kernel_pointer_decl():
+    a = cl.zeros((10,), dtype=cl.int)
+    knl = cl.Kernel('my_knl', {'a': a},
+                    """
+                    global int* c_glob = a;
+                    private int ary[5];
+                    int* c;
+                    int* b=ary;
+                    c = b; // swap pointers
+                    c[1] = 5;
+                    a[1] = ary[1];
+                    c_glob[2] = 10;""",
+                    global_size=a.shape)
+    knl_py = knl.compile(emulate=True)
+    knl_py()
+    assert a.get()[1] == 5   # verify private pointer behavior
+    assert a.get()[2] == 10  # verify global pointer behavior global int* c_glob = a;
+    a2 = cl.zeros((10,), dtype=cl.int)
+    knl(a=a2)
+    assert a2.get()[1] == 5
+    assert a2.get()[2] == 10
```

### Comparing `pyopencl-extension-0.2.7/tests/test_framework.py` & `pyopencl-extension-0.2.8/tests/test_framework.py`

 * *Files identical despite different names*

