# Comparing `tmp/zos-utilities-0.5.3.tar.gz` & `tmp/zos-utilities-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/zos-utilities/zos-utilities/dist/tmp01fq48dl/zos-utilities-0.5.3.tar", last modified: Mon Jun 13 15:54:20 2022, max compression
+gzip compressed data, was "/Users/kdm/src/zos-utilities/dist/.tmp-fv8g1cyq/zos-utilities-0.6.0.tar", last modified: Tue Jun 27 14:12:41 2023, max compression
```

## Comparing `zos-utilities-0.5.3.tar` & `zos-utilities-0.6.0.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-13 15:54:20.000000 zos-utilities-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (116)      159 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3528 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (116)      698 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (116)      575 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      262 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2484 2022-06-13 15:54:20.000000 zos-utilities-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      974 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-13 15:54:20.000000 zos-utilities-0.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (116)      614 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)       28 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (116)     4870 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)       33 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (116)       28 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (116)      309 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1158 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (116)      775 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (116)       27 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (116)       81 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (116)      432 2022-06-13 15:54:20.000000 zos-utilities-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1872 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-13 15:54:20.000000 zos-utilities-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-13 15:54:20.000000 zos-utilities-0.5.3/src/zos_utilities/
--rw-r--r--   0 runner    (1001) docker     (116)      134 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/src/zos_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      590 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/src/zos_utilities/cpc.py
--rw-r--r--   0 runner    (1001) docker     (116)      596 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/src/zos_utilities/julian_to_datetime.py
--rw-r--r--   0 runner    (1001) docker     (116)      380 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/src/zos_utilities/logical_cpu.py
--rw-r--r--   0 runner    (1001) docker     (116)    10484 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/src/zos_utilities/lpar.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-13 15:54:20.000000 zos-utilities-0.5.3/src/zos_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2484 2022-06-13 15:54:19.000000 zos-utilities-0.5.3/src/zos_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      701 2022-06-13 15:54:20.000000 zos-utilities-0.5.3/src/zos_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-06-13 15:54:19.000000 zos-utilities-0.5.3/src/zos_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-06-13 15:54:17.000000 zos-utilities-0.5.3/src/zos_utilities.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       14 2022-06-13 15:54:20.000000 zos-utilities-0.5.3/src/zos_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-13 15:54:20.000000 zos-utilities-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (116)      122 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/tests/test_cpc.py
--rw-r--r--   0 runner    (1001) docker     (116)      837 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/tests/test_julian_to_datetime.py
--rw-r--r--   0 runner    (1001) docker     (116)    15191 2022-06-13 15:54:07.000000 zos-utilities-0.5.3/tests/test_lpar_parse_core_status.py
+drwxr-xr-x   0 kdm        (501) staff       (20)        0 2023-06-27 14:12:41.000000 zos-utilities-0.6.0/
+-rw-r--r--   0 kdm        (501) staff       (20)      159 2022-04-15 03:06:15.000000 zos-utilities-0.6.0/AUTHORS.rst
+-rw-r--r--   0 kdm        (501) staff       (20)     3528 2022-04-20 15:26:05.000000 zos-utilities-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 kdm        (501) staff       (20)      844 2023-06-26 18:55:13.000000 zos-utilities-0.6.0/HISTORY.rst
+-rw-r--r--   0 kdm        (501) staff       (20)      575 2022-04-20 15:48:03.000000 zos-utilities-0.6.0/LICENSE
+-rw-r--r--   0 kdm        (501) staff       (20)      262 2022-04-20 15:44:21.000000 zos-utilities-0.6.0/MANIFEST.in
+-rw-r--r--   0 kdm        (501) staff       (20)     2854 2023-06-27 14:12:41.000000 zos-utilities-0.6.0/PKG-INFO
+-rw-r--r--   0 kdm        (501) staff       (20)     1147 2023-06-26 19:44:38.000000 zos-utilities-0.6.0/README.rst
+drwxr-xr-x   0 kdm        (501) staff       (20)        0 2023-06-27 14:12:41.000000 zos-utilities-0.6.0/docs/
+-rw-r--r--   0 kdm        (501) staff       (20)      614 2022-04-20 15:53:26.000000 zos-utilities-0.6.0/docs/Makefile
+-rw-r--r--   0 kdm        (501) staff       (20)       28 2022-03-04 19:04:14.000000 zos-utilities-0.6.0/docs/authors.rst
+-rwxr-xr-x   0 kdm        (501) staff       (20)     4870 2022-04-20 15:41:19.000000 zos-utilities-0.6.0/docs/conf.py
+-rw-r--r--   0 kdm        (501) staff       (20)       33 2022-03-04 19:04:14.000000 zos-utilities-0.6.0/docs/contributing.rst
+-rw-r--r--   0 kdm        (501) staff       (20)       28 2022-03-04 19:04:14.000000 zos-utilities-0.6.0/docs/history.rst
+-rw-r--r--   0 kdm        (501) staff       (20)      309 2022-04-20 15:54:16.000000 zos-utilities-0.6.0/docs/index.rst
+-rw-r--r--   0 kdm        (501) staff       (20)     1158 2022-04-20 15:55:10.000000 zos-utilities-0.6.0/docs/installation.rst
+-rw-r--r--   0 kdm        (501) staff       (20)      775 2022-04-20 17:30:26.000000 zos-utilities-0.6.0/docs/make.bat
+-rw-r--r--   0 kdm        (501) staff       (20)       27 2022-03-04 19:04:14.000000 zos-utilities-0.6.0/docs/readme.rst
+-rw-r--r--   0 kdm        (501) staff       (20)       81 2022-04-20 17:28:43.000000 zos-utilities-0.6.0/docs/usage.rst
+-rw-r--r--   0 kdm        (501) staff       (20)      432 2023-06-27 14:12:41.000000 zos-utilities-0.6.0/setup.cfg
+-rw-r--r--   0 kdm        (501) staff       (20)     1922 2023-06-26 19:58:58.000000 zos-utilities-0.6.0/setup.py
+drwxr-xr-x   0 kdm        (501) staff       (20)        0 2023-06-27 14:12:41.000000 zos-utilities-0.6.0/src/
+drwxr-xr-x   0 kdm        (501) staff       (20)        0 2023-06-27 14:12:41.000000 zos-utilities-0.6.0/src/zos_utilities/
+-rw-r--r--   0 kdm        (501) staff       (20)      134 2023-06-26 19:58:58.000000 zos-utilities-0.6.0/src/zos_utilities/__init__.py
+-rw-r--r--   0 kdm        (501) staff       (20)      590 2022-05-02 15:57:13.000000 zos-utilities-0.6.0/src/zos_utilities/cpc.py
+-rw-r--r--   0 kdm        (501) staff       (20)      160 2023-06-26 19:55:32.000000 zos-utilities-0.6.0/src/zos_utilities/dasd_volume.py
+-rw-r--r--   0 kdm        (501) staff       (20)      244 2023-06-26 19:55:32.000000 zos-utilities-0.6.0/src/zos_utilities/data_set.py
+-rw-r--r--   0 kdm        (501) staff       (20)      596 2022-04-20 17:34:17.000000 zos-utilities-0.6.0/src/zos_utilities/julian_to_datetime.py
+-rw-r--r--   0 kdm        (501) staff       (20)      374 2023-06-26 19:55:32.000000 zos-utilities-0.6.0/src/zos_utilities/logical_cpu.py
+-rw-r--r--   0 kdm        (501) staff       (20)    11934 2023-06-26 19:55:32.000000 zos-utilities-0.6.0/src/zos_utilities/lpar.py
+drwxr-xr-x   0 kdm        (501) staff       (20)        0 2023-06-27 14:12:41.000000 zos-utilities-0.6.0/src/zos_utilities.egg-info/
+-rw-r--r--   0 kdm        (501) staff       (20)     2854 2023-06-27 14:12:41.000000 zos-utilities-0.6.0/src/zos_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 kdm        (501) staff       (20)      793 2023-06-27 14:12:41.000000 zos-utilities-0.6.0/src/zos_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 kdm        (501) staff       (20)        1 2023-06-27 14:12:41.000000 zos-utilities-0.6.0/src/zos_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 kdm        (501) staff       (20)        1 2022-04-20 17:32:57.000000 zos-utilities-0.6.0/src/zos_utilities.egg-info/not-zip-safe
+-rw-r--r--   0 kdm        (501) staff       (20)       14 2023-06-27 14:12:41.000000 zos-utilities-0.6.0/src/zos_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 kdm        (501) staff       (20)        0 2023-06-27 14:12:41.000000 zos-utilities-0.6.0/tests/
+-rw-r--r--   0 kdm        (501) staff       (20)      122 2022-05-02 20:03:25.000000 zos-utilities-0.6.0/tests/test_cpc.py
+-rw-r--r--   0 kdm        (501) staff       (20)      837 2022-04-14 20:54:04.000000 zos-utilities-0.6.0/tests/test_julian_to_datetime.py
+-rw-r--r--   0 kdm        (501) staff       (20)     6764 2023-06-26 19:56:17.000000 zos-utilities-0.6.0/tests/test_lpar_parse_asm.py
+-rw-r--r--   0 kdm        (501) staff       (20)    15189 2023-06-26 19:55:32.000000 zos-utilities-0.6.0/tests/test_lpar_parse_core_status.py
```

### Comparing `zos-utilities-0.5.3/CONTRIBUTING.rst` & `zos-utilities-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `zos-utilities-0.5.3/HISTORY.rst` & `zos-utilities-0.6.0/HISTORY.rst`

 * *Files 25% similar despite different names*

```diff
@@ -20,7 +20,15 @@
 ----------------------
 * Add some additional cpc and lpar fields
 * Automate build and publishing to Pypi
 
 0.5.0 (2022-05-25)
 ----------------------
 * Strip out leading spaces from inputs (because sometimes they're getting passed in that way)
+
+0.5.3 (2022-06-13)
+----------------------
+* Bugfixes
+
+0.6.0 (2023-06-25)
+----------------------
+* Add initial support for IEE200I (D ASM output)
```

### Comparing `zos-utilities-0.5.3/LICENSE` & `zos-utilities-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zos-utilities-0.5.3/PKG-INFO` & `zos-utilities-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zos-utilities
-Version: 0.5.3
+Version: 0.6.0
 Summary: Library for performing various utility functions for z/OS
 Home-page: https://github.com/Tam-Lin/zos-utilities
 Author: Kevin McKenzie
 Author-email: kmckenzi@us.ibm.com
 License: Apache Software License 2.0
 Keywords: zos-utilities
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =============
 zos-utilities
 =============
@@ -33,14 +34,18 @@
         :target: https://github.com/Tam-Lin/zos-utilities/actions/workflows/build_and_test.yml
         :alt: Build and Test Status
 
 .. image:: https://readthedocs.org/projects/zos-utilities/badge/?version=latest
         :target: https://zos-utilities.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
+.. image:: https://img.shields.io/pypi/pyversions/zos-utilities.svg
+        :target: https://img.shields.io/pypi/pyversions/zos-utilities.svg
+        :alt: Python versions
+
 
 Library for performing various utility functions needed for z/OS libraries. I have a couple of libraries that do
 various things for/with z/OS, and they all need to convert from the z/OS Julian Date to datetime, so I thought I might
 as well put it into a library.  I'm also starting to build a representation of z/OS and IBM Z from an infrastructure
 perspective.
 
 
@@ -66,7 +71,15 @@
 ----------------------
 * Add some additional cpc and lpar fields
 * Automate build and publishing to Pypi
 
 0.5.0 (2022-05-25)
 ----------------------
 * Strip out leading spaces from inputs (because sometimes they're getting passed in that way)
+
+0.5.3 (2022-06-13)
+----------------------
+* Bugfixes
+
+0.6.0 (2023-06-25)
+----------------------
+* Add initial support for IEE200I (D ASM output)
```

### Comparing `zos-utilities-0.5.3/README.rst` & `zos-utilities-0.6.0/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -11,12 +11,16 @@
         :target: https://github.com/Tam-Lin/zos-utilities/actions/workflows/build_and_test.yml
         :alt: Build and Test Status
 
 .. image:: https://readthedocs.org/projects/zos-utilities/badge/?version=latest
         :target: https://zos-utilities.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
+.. image:: https://img.shields.io/pypi/pyversions/zos-utilities.svg
+        :target: https://img.shields.io/pypi/pyversions/zos-utilities.svg
+        :alt: Python versions
+
 
 Library for performing various utility functions needed for z/OS libraries. I have a couple of libraries that do
 various things for/with z/OS, and they all need to convert from the z/OS Julian Date to datetime, so I thought I might
 as well put it into a library.  I'm also starting to build a representation of z/OS and IBM Z from an infrastructure
 perspective.
```

### Comparing `zos-utilities-0.5.3/docs/Makefile` & `zos-utilities-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zos-utilities-0.5.3/docs/conf.py` & `zos-utilities-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zos-utilities-0.5.3/docs/installation.rst` & `zos-utilities-0.6.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `zos-utilities-0.5.3/docs/make.bat` & `zos-utilities-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zos-utilities-0.5.3/setup.py` & `zos-utilities-0.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     description="Library for performing various utility functions for z/OS",
     entry_points={
     },
     install_requires=requirements,
     license="Apache Software License 2.0",
     long_description=readme + '\n\n' + history,
@@ -59,10 +60,10 @@
     name='zos-utilities',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Tam-Lin/zos-utilities',
-    version='0.5.3',
+    version='0.6.0',
     zip_safe=False,
 )
```

### Comparing `zos-utilities-0.5.3/src/zos_utilities/cpc.py` & `zos-utilities-0.6.0/src/zos_utilities/cpc.py`

 * *Files identical despite different names*

### Comparing `zos-utilities-0.5.3/src/zos_utilities/julian_to_datetime.py` & `zos-utilities-0.6.0/src/zos_utilities/julian_to_datetime.py`

 * *Files identical despite different names*

### Comparing `zos-utilities-0.5.3/src/zos_utilities/lpar.py` & `zos-utilities-0.6.0/src/zos_utilities/lpar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import re
 import logging
 
 from collections import OrderedDict
 import dataclasses
 from datetime import datetime
 
-from zos_utilities.logical_cpu import Logical_CPU
+from .logical_cpu import Logical_CPU
+from .data_set import DataSet
+from .dasd_volume import DasdVolume
 
 
 @dataclasses.dataclass
 class LPAR:
     """
     Represents an IBM z/OS LPAR
     """
@@ -93,14 +95,19 @@
 
     storage: int = None
 
     initial_central_storage: int = None
     current_central_storage: int = None
     maximum_central_storage: int = None
 
+    plpa_data_set: DataSet = None
+    common_data_set: DataSet = None
+    local_data_set: dataclasses.field(default_factory=list()) = None
+    scm = None
+
     def parse_d_m_core(self, iee174i_message):
         """
         Takes the output of the response to 'D M=CORE' and builds a representation of the
         system logical processor state at that time
 
         :param core_status_message: The output of the message you want parsed
         :return: Updates the internal state information of the lpar
@@ -305,10 +312,45 @@
         if iee174i_message[linenum].lstrip().startswith("MIF ID  = "):
             self.mif_id = iee174i_message[linenum].lstrip()[10:].rstrip()
         else:
             error = ("line didn't start with MIF ID = ;  got %s" % iee174i_message[linenum])
             logger.error(error)
             raise LPARException(error)
 
+    def parse_d_asm(self, iee200i_message):
+
+        logger = logging.getLogger(__name__)
+
+        if iee200i_message[0].split()[0] != "IEE200I":
+            message = str("Incorrect message passed in; expected IEE200I, got %s" %
+                          iee200i_message[0].split()[0])
+            logger.error(message)
+            raise LPARException(message)
+
+        for linenum, line in enumerate(iee200i_message[2:], start=2):
+
+            split_line = line.split()
+            storage_type = split_line[0]
+
+            if storage_type in ("PLPA", "COMMON", "LOCAL"):
+
+                dev = split_line[4]
+                dataset_name = split_line[5]
+
+                dataset = DataSet(name=dataset_name, location=DasdVolume(unit_address=dev))
+
+                if storage_type == "PLPA":
+                    self.plpa_data_set = dataset
+                elif storage_type == "COMMON":
+                    self.common_data_set = dataset
+                elif storage_type == "LOCAL":
+                    try:
+                        self.local_data_set.append(dataset)
+                    except AttributeError:
+                        self.local_data_set = [dataset]
+
+            if storage_type == "SCM":
+                self.scm = True
+
 
 class LPARException(Exception):
     pass
```

### Comparing `zos-utilities-0.5.3/src/zos_utilities.egg-info/PKG-INFO` & `zos-utilities-0.6.0/src/zos_utilities.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zos-utilities
-Version: 0.5.3
+Version: 0.6.0
 Summary: Library for performing various utility functions for z/OS
 Home-page: https://github.com/Tam-Lin/zos-utilities
 Author: Kevin McKenzie
 Author-email: kmckenzi@us.ibm.com
 License: Apache Software License 2.0
 Keywords: zos-utilities
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =============
 zos-utilities
 =============
@@ -33,14 +34,18 @@
         :target: https://github.com/Tam-Lin/zos-utilities/actions/workflows/build_and_test.yml
         :alt: Build and Test Status
 
 .. image:: https://readthedocs.org/projects/zos-utilities/badge/?version=latest
         :target: https://zos-utilities.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
+.. image:: https://img.shields.io/pypi/pyversions/zos-utilities.svg
+        :target: https://img.shields.io/pypi/pyversions/zos-utilities.svg
+        :alt: Python versions
+
 
 Library for performing various utility functions needed for z/OS libraries. I have a couple of libraries that do
 various things for/with z/OS, and they all need to convert from the z/OS Julian Date to datetime, so I thought I might
 as well put it into a library.  I'm also starting to build a representation of z/OS and IBM Z from an infrastructure
 perspective.
 
 
@@ -66,7 +71,15 @@
 ----------------------
 * Add some additional cpc and lpar fields
 * Automate build and publishing to Pypi
 
 0.5.0 (2022-05-25)
 ----------------------
 * Strip out leading spaces from inputs (because sometimes they're getting passed in that way)
+
+0.5.3 (2022-06-13)
+----------------------
+* Bugfixes
+
+0.6.0 (2023-06-25)
+----------------------
+* Add initial support for IEE200I (D ASM output)
```

### Comparing `zos-utilities-0.5.3/src/zos_utilities.egg-info/SOURCES.txt` & `zos-utilities-0.6.0/src/zos_utilities.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,21 @@
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 src/zos_utilities/__init__.py
 src/zos_utilities/cpc.py
+src/zos_utilities/dasd_volume.py
+src/zos_utilities/data_set.py
 src/zos_utilities/julian_to_datetime.py
 src/zos_utilities/logical_cpu.py
 src/zos_utilities/lpar.py
 src/zos_utilities.egg-info/PKG-INFO
 src/zos_utilities.egg-info/SOURCES.txt
 src/zos_utilities.egg-info/dependency_links.txt
 src/zos_utilities.egg-info/not-zip-safe
 src/zos_utilities.egg-info/top_level.txt
 tests/test_cpc.py
 tests/test_julian_to_datetime.py
+tests/test_lpar_parse_asm.py
 tests/test_lpar_parse_core_status.py
```

### Comparing `zos-utilities-0.5.3/tests/test_julian_to_datetime.py` & `zos-utilities-0.6.0/tests/test_julian_to_datetime.py`

 * *Files identical despite different names*

### Comparing `zos-utilities-0.5.3/tests/test_lpar_parse_core_status.py` & `zos-utilities-0.6.0/tests/test_lpar_parse_core_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,14 @@
         assert test_lpar.cpc_id == "00"
         assert test_lpar.cpc_name == "T256"
         assert test_lpar.lpar_name == "S5E"
         assert test_lpar.lpar_id == "21"
         assert test_lpar.css_id == "2"
         assert test_lpar.mif_id == "1"
 
-
     def test_lpar_parse_d_m_core_procview_cpu_with_leading_spaces(self, good_input_procview_cpu):
         test_lpar = lpar.LPAR()
 
         leading_spaces_input = ['  {} '.format(x) for x in good_input_procview_cpu]
 
         test_lpar.parse_d_m_core(leading_spaces_input)
 
@@ -193,15 +192,14 @@
         assert test_lpar.cpc_id == "00"
         assert test_lpar.cpc_name == "T256"
         assert test_lpar.lpar_name == "S5E"
         assert test_lpar.lpar_id == "21"
         assert test_lpar.css_id == "2"
         assert test_lpar.mif_id == "1"
 
-
     def test_lpar_parse_d_m_core_procview_core(self, good_input_procview_core):
         test_lpar = lpar.LPAR()
         test_lpar.parse_d_m_core(good_input_procview_core)
 
         assert test_lpar.hiperdispatch is True
         assert test_lpar.mt_mode == 2
         assert test_lpar.cp_mt_mode == 1
```

