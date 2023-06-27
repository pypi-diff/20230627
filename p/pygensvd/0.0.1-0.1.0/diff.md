# Comparing `tmp/pygensvd-0.0.1.tar.gz` & `tmp/pygensvd-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygensvd-0.0.1.tar", last modified: Tue Jun 27 00:02:06 2023, max compression
+gzip compressed data, was "pygensvd-0.1.0.tar", last modified: Tue Jun 27 02:31:05 2023, max compression
```

## Comparing `pygensvd-0.0.1.tar` & `pygensvd-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 vanandrew  (1000) vanandrew  (1000)        0 2023-06-27 00:02:06.510629 pygensvd-0.0.1/
--rw-r--r--   0 vanandrew  (1000) vanandrew  (1000)     1975 2023-06-26 21:02:40.000000 pygensvd-0.0.1/CMakeLists.txt
--rw-r--r--   0 vanandrew  (1000) vanandrew  (1000)     1203 2023-06-17 23:21:24.000000 pygensvd-0.0.1/FindLAPACKE.cmake
--rw-r--r--   0 vanandrew  (1000) vanandrew  (1000)      732 2023-06-12 22:48:07.000000 pygensvd-0.0.1/LICENSE.txt
--rw-r--r--   0 vanandrew  (1000) vanandrew  (1000)       74 2023-06-26 23:33:50.000000 pygensvd-0.0.1/MANIFEST.in
--rw-r--r--   0 vanandrew  (1000) vanandrew  (1000)     4441 2023-06-27 00:02:06.510629 pygensvd-0.0.1/PKG-INFO
--rw-r--r--   0 vanandrew  (1000) vanandrew  (1000)     3980 2023-06-26 21:02:40.000000 pygensvd-0.0.1/README.md
-drwxr-xr-x   0 vanandrew  (1000) vanandrew  (1000)        0 2023-06-27 00:02:06.510629 pygensvd-0.0.1/pygensvd/
--rw-r--r--   0 vanandrew  (1000) vanandrew  (1000)     5188 2023-06-17 23:21:24.000000 pygensvd-0.0.1/pygensvd/__init__.py
-drwxr-xr-x   0 vanandrew  (1000) vanandrew  (1000)        0 2023-06-27 00:02:06.510629 pygensvd-0.0.1/pygensvd.egg-info/
--rw-r--r--   0 vanandrew  (1000) vanandrew  (1000)     4441 2023-06-27 00:02:06.000000 pygensvd-0.0.1/pygensvd.egg-info/PKG-INFO
--rw-r--r--   0 vanandrew  (1000) vanandrew  (1000)      301 2023-06-27 00:02:06.000000 pygensvd-0.0.1/pygensvd.egg-info/SOURCES.txt
--rw-r--r--   0 vanandrew  (1000) vanandrew  (1000)        1 2023-06-27 00:02:06.000000 pygensvd-0.0.1/pygensvd.egg-info/dependency_links.txt
--rw-r--r--   0 vanandrew  (1000) vanandrew  (1000)       25 2023-06-27 00:02:06.000000 pygensvd-0.0.1/pygensvd.egg-info/requires.txt
--rw-r--r--   0 vanandrew  (1000) vanandrew  (1000)        9 2023-06-27 00:02:06.000000 pygensvd-0.0.1/pygensvd.egg-info/top_level.txt
--rw-r--r--   0 vanandrew  (1000) vanandrew  (1000)     1028 2023-06-26 23:53:01.000000 pygensvd-0.0.1/pyproject.toml
--rw-r--r--   0 vanandrew  (1000) vanandrew  (1000)       38 2023-06-27 00:02:06.510629 pygensvd-0.0.1/setup.cfg
--rw-r--r--   0 vanandrew  (1000) vanandrew  (1000)      373 2023-06-12 23:54:52.000000 pygensvd-0.0.1/setup.py
-drwxr-xr-x   0 vanandrew  (1000) vanandrew  (1000)        0 2023-06-27 00:02:06.510629 pygensvd-0.0.1/src/
--rw-r--r--   0 vanandrew  (1000) vanandrew  (1000)     6142 2023-06-13 01:55:06.000000 pygensvd-0.0.1/src/_gsvd.c
-drwxr-xr-x   0 vanandrew  (1000) vanandrew  (1000)        0 2023-06-27 00:02:06.510629 pygensvd-0.0.1/tests/
--rw-r--r--   0 vanandrew  (1000) vanandrew  (1000)     6303 2023-06-17 23:21:24.000000 pygensvd-0.0.1/tests/test_gsvd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 02:31:05.238640 pygensvd-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-06-27 02:30:49.000000 pygensvd-0.1.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1203 2023-06-27 02:30:49.000000 pygensvd-0.1.0/FindLAPACKE.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)      732 2023-06-27 02:30:49.000000 pygensvd-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-06-27 02:30:49.000000 pygensvd-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4441 2023-06-27 02:31:05.238640 pygensvd-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3980 2023-06-27 02:30:49.000000 pygensvd-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 02:31:05.234640 pygensvd-0.1.0/pygensvd/
+-rw-r--r--   0 runner    (1001) docker     (122)     5188 2023-06-27 02:30:49.000000 pygensvd-0.1.0/pygensvd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 02:31:05.238640 pygensvd-0.1.0/pygensvd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4441 2023-06-27 02:31:05.000000 pygensvd-0.1.0/pygensvd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      301 2023-06-27 02:31:05.000000 pygensvd-0.1.0/pygensvd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 02:31:05.000000 pygensvd-0.1.0/pygensvd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-27 02:31:05.000000 pygensvd-0.1.0/pygensvd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-27 02:31:05.000000 pygensvd-0.1.0/pygensvd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-06-27 02:30:49.000000 pygensvd-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-27 02:31:05.238640 pygensvd-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-06-27 02:30:49.000000 pygensvd-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 02:31:05.238640 pygensvd-0.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     6142 2023-06-27 02:30:49.000000 pygensvd-0.1.0/src/_gsvd.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 02:31:05.238640 pygensvd-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     6303 2023-06-27 02:30:49.000000 pygensvd-0.1.0/tests/test_gsvd.py
```

### Comparing `pygensvd-0.0.1/CMakeLists.txt` & `pygensvd-0.1.0/CMakeLists.txt`

 * *Files 17% similar despite different names*

```diff
@@ -5,89 +5,65 @@
 set(CMAKE_C_STANDARD 17)
 
 # set project name and languages
 project(omni LANGUAGES C)
 
 # find python 3.10 > 3.7
 exec_program(${PYTHON_EXECUTABLE} ARGS "-c \"import sys; print('.'.join(map(str, sys.version_info[:2])))\"" OUTPUT_VARIABLE PYTHON_VERSION)
-find_package(Python ${PYTHON_VERSION} EXACT REQUIRED NumPy)
+find_package(Python ${PYTHON_VERSION} EXACT REQUIRED OPTIONAL_COMPONENTS NumPy)
+
+# if we couldn't find numpy with FindPython then try using the numpy module instead
+if(NOT Python_NumPy_FOUND)
+    message(STATUS "Could not find NumPy with FindPython, trying to find it with the numpy module instead.")
+    exec_program(${PYTHON_EXECUTABLE} ARGS "-c \"import numpy; print(numpy.get_include())\"" OUTPUT_VARIABLE Python_NumPy_INCLUDE_DIRS)
+    message(STATUS "Found NumPy include directory: ${Python_NumPy_INCLUDE_DIRS}")
+endif()
 
 # find LAPACK and BLAS (Use static linkage)
 set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} ${PROJECT_SOURCE_DIR})
 
-# if we didn't find MKL
-# then search for OpenBLAS
+# search for openblas first
 set(BLA_VENDOR OpenBLAS)
 find_package(BLAS)
 
 if(BLAS_FOUND)
     find_package(LAPACK REQUIRED)
     find_package(LAPACKE REQUIRED)
 endif()
 
 # then search for everything else
+# NO GUARANTEE THAT THIS WILL WORK!
 if(NOT BLAS_FOUND)
     find_package(BLAS REQUIRED)
     find_package(LAPACK REQUIRED)
     find_package(LAPACKE REQUIRED)
 endif()
 
 # add pygensvd library
 Python_add_library(
     _gsvd
     MODULE
     WITH_SOABI
     src/_gsvd.c
 )
-target_link_libraries(
-    _gsvd
-    PRIVATE
-    Python::NumPy
-)
-
-# check if this is an mkl library
-# THIS IS CURRENTLY NOT WORKING
-if(BLAS_LIBRARIES MATCHES "(mkl)")
-    if(NOT DEFINED ENV{MKLROOT})
-        message(
-            FATAL_ERROR
-            "CMake detected MKL for a BLAS/LAPACK backend, but MKLROOT is undefined! \
-            Check that your MKL environment is setup correctly."
-        )
-    endif()
-
-    set(MKLROOT $ENV{MKLROOT})
-    set(MKL_INCLUDE_DIRECTORY ${MKLROOT}/include)
-    target_compile_definitions(
-        _gsvd
-        PRIVATE
-        USE_MKL
-    )
-    target_include_directories(
-        _gsvd
-        PRIVATE
-        ${MKL_INCLUDE_DIRECTORY}
-    )
-else()
-    target_compile_definitions(
-        _gsvd
-        PRIVATE
-        USE_LAPACK
-    )
-endif()
-
 target_include_directories(
     _gsvd
     PRIVATE
     ${LAPACKE_INCLUDE_DIRS}
+    ${Python_NumPy_INCLUDE_DIRS}
 )
 target_link_libraries(
     _gsvd
     PRIVATE
     ${LAPACKE_LIBRARIES}
 )
+target_compile_definitions(
+    _gsvd
+    PRIVATE
+    USE_LAPACK
+)
 
 # install library
 install(
     TARGETS _gsvd
     LIBRARY DESTINATION lib
 )
```

### Comparing `pygensvd-0.0.1/FindLAPACKE.cmake` & `pygensvd-0.1.0/FindLAPACKE.cmake`

 * *Files identical despite different names*

### Comparing `pygensvd-0.0.1/LICENSE.txt` & `pygensvd-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygensvd-0.0.1/PKG-INFO` & `pygensvd-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygensvd
-Version: 0.0.1
+Version: 0.1.0
 Summary: Python and NumPy extension module implementing the generalized signular value decomposition (GSVD).
 Author-email: Andrew Van <vanandrew@wustl.edu>
 License: GNU License
 Project-URL: github, https://github.com/vanandrew/pygensvd
 Keywords: GSVD
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `pygensvd-0.0.1/README.md` & `pygensvd-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pygensvd-0.0.1/pygensvd/__init__.py` & `pygensvd-0.1.0/pygensvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pygensvd-0.0.1/pygensvd.egg-info/PKG-INFO` & `pygensvd-0.1.0/pygensvd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygensvd
-Version: 0.0.1
+Version: 0.1.0
 Summary: Python and NumPy extension module implementing the generalized signular value decomposition (GSVD).
 Author-email: Andrew Van <vanandrew@wustl.edu>
 License: GNU License
 Project-URL: github, https://github.com/vanandrew/pygensvd
 Keywords: GSVD
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `pygensvd-0.0.1/pyproject.toml` & `pygensvd-0.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,42 +2,47 @@
 name = "pygensvd"
 description = "Python and NumPy extension module implementing the generalized signular value decomposition (GSVD)."
 readme = "README.md"
 requires-python = ">=3.7"
 license = { text = "GNU License" }
 authors = [{ name = "Andrew Van", email = "vanandrew@wustl.edu" }]
 keywords = ["GSVD"]
-classifiers = [
-  "Programming Language :: Python :: 3",
-]
+classifiers = ["Programming Language :: Python :: 3"]
 urls = { github = "https://github.com/vanandrew/pygensvd" }
-version = "0.0.1"
-dependencies = [
-    "numpy >= 1.1"
-]
+version = "0.1.0"
+dependencies = ["numpy >= 1.1"]
 
 [build-system]
 requires = ["setuptools", "wheel", "cmake", "cmake-setuptools-ext", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project.optional-dependencies]
-dev = [
-    "pytest"
-]
+dev = ["pytest"]
 
 [tool.black]
 line-length = 120
-target-version = ['py37', 'py38', 'py39', 'py310']
+target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 
 [tool.cibuildwheel]
 archs = ['x86_64']
 build = [
-    "cp37-manylinux*",
-    "cp38-manylinux*",
-    "cp39-manylinux*",
-    "cp310-manylinux*",
-    "cp311-manylinux*",
+  "cp37-manylinux*",
+  "cp38-manylinux*",
+  "cp39-manylinux*",
+  "cp310-manylinux*",
+  "cp311-manylinux*",
+  "cp37-macosx*",
+  "cp38-macosx*",
+  "cp39-macosx*",
+  "cp310-macosx*",
+  "cp311-macosx*",
 ]
 build-frontend = "build"
+before-test = ["python -m pip install pytest"]
+test-command = ["python -m pytest {project}/tests"]
 
 [tool.cibuildwheel.linux]
-before-all = ["yum -y install openblas-devel"]
+before-all = ["yum -y install openblas-devel lapack-devel"]
+
+[tool.cibuildwheel.macos]
+before-all = ["brew install openblas"]
+environment = { CMAKE_ARGS = "-DCMAKE_PREFIX_PATH=/usr/local/opt/openblas" }
```

### Comparing `pygensvd-0.0.1/src/_gsvd.c` & `pygensvd-0.1.0/src/_gsvd.c`

 * *Files identical despite different names*

### Comparing `pygensvd-0.0.1/tests/test_gsvd.py` & `pygensvd-0.1.0/tests/test_gsvd.py`

 * *Files identical despite different names*

