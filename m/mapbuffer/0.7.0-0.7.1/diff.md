# Comparing `tmp/mapbuffer-0.7.0.tar.gz` & `tmp/mapbuffer-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapbuffer-0.7.0.tar", last modified: Mon Mar 27 22:22:03 2023, max compression
+gzip compressed data, was "mapbuffer-0.7.1.tar", last modified: Tue Jun 27 07:58:49 2023, max compression
```

## Comparing `mapbuffer-0.7.0.tar` & `mapbuffer-0.7.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-03-27 22:22:03.615981 mapbuffer-0.7.0/
--rw-r--r--   0 wms        (501) staff       (20)       64 2021-01-11 02:44:57.000000 mapbuffer-0.7.0/.dockerignore
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-03-27 22:22:03.608580 mapbuffer-0.7.0/.github/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-03-27 22:22:03.613166 mapbuffer-0.7.0/.github/workflows/
--rw-r--r--   0 wms        (501) staff       (20)      914 2023-03-27 22:14:15.000000 mapbuffer-0.7.0/.github/workflows/build_wheel.yml
--rw-r--r--   0 wms        (501) staff       (20)       52 2023-03-27 22:22:02.000000 mapbuffer-0.7.0/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)     3056 2023-03-27 22:22:02.000000 mapbuffer-0.7.0/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)     1538 2021-01-11 02:44:57.000000 mapbuffer-0.7.0/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)     6021 2023-03-27 22:22:03.616130 mapbuffer-0.7.0/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     5094 2023-03-16 15:55:02.000000 mapbuffer-0.7.0/README.md
--rw-r--r--   0 wms        (501) staff       (20)     1425 2023-03-27 22:13:34.000000 mapbuffer-0.7.0/appveyor.yml
--rw-r--r--   0 wms        (501) staff       (20)     4809 2023-03-27 20:40:53.000000 mapbuffer-0.7.0/automated_test.py
--rwxr-xr-x   0 wms        (501) staff       (20)      721 2021-01-11 02:44:57.000000 mapbuffer-0.7.0/build_linux.sh
--rw-r--r--   0 wms        (501) staff       (20)     2492 2022-09-16 23:17:07.000000 mapbuffer-0.7.0/compare_searches.c
--rw-r--r--   0 wms        (501) staff       (20)      805 2021-01-11 02:44:57.000000 mapbuffer-0.7.0/manylinux1.Dockerfile
--rw-r--r--   0 wms        (501) staff       (20)     1416 2021-01-11 02:44:57.000000 mapbuffer-0.7.0/manylinux2010.Dockerfile
--rw-r--r--   0 wms        (501) staff       (20)     1771 2021-01-11 02:44:57.000000 mapbuffer-0.7.0/manylinux2014.Dockerfile
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-03-27 22:22:03.614392 mapbuffer-0.7.0/mapbuffer/
--rw-r--r--   0 wms        (501) staff       (20)      885 2023-03-15 22:19:05.000000 mapbuffer-0.7.0/mapbuffer/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     5815 2023-03-15 22:19:05.000000 mapbuffer-0.7.0/mapbuffer/compression.py
--rw-r--r--   0 wms        (501) staff       (20)      376 2021-01-11 02:44:57.000000 mapbuffer-0.7.0/mapbuffer/exceptions.py
--rw-r--r--   0 wms        (501) staff       (20)     5014 2023-03-27 21:27:10.000000 mapbuffer-0.7.0/mapbuffer/intmap.py
--rw-r--r--   0 wms        (501) staff       (20)     2414 2023-03-27 21:30:18.000000 mapbuffer-0.7.0/mapbuffer/lib.py
--rw-r--r--   0 wms        (501) staff       (20)     9550 2023-03-27 21:37:07.000000 mapbuffer-0.7.0/mapbuffer/mapbuffer.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-03-27 22:22:03.615794 mapbuffer-0.7.0/mapbuffer.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)     6021 2023-03-27 22:22:02.000000 mapbuffer-0.7.0/mapbuffer.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      688 2023-03-27 22:22:03.000000 mapbuffer-0.7.0/mapbuffer.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-03-27 22:22:02.000000 mapbuffer-0.7.0/mapbuffer.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2021-01-20 01:43:04.000000 mapbuffer-0.7.0/mapbuffer.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2023-03-27 22:22:02.000000 mapbuffer-0.7.0/mapbuffer.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)       50 2023-03-27 22:22:02.000000 mapbuffer-0.7.0/mapbuffer.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)       25 2023-03-27 22:22:02.000000 mapbuffer-0.7.0/mapbuffer.egg-info/top_level.txt
--rw-r--r--   0 wms        (501) staff       (20)     3598 2023-03-27 22:12:26.000000 mapbuffer-0.7.0/mapbufferaccel.c
--rw-r--r--   0 wms        (501) staff       (20)     1099 2023-03-27 21:30:18.000000 mapbuffer-0.7.0/perf.py
--rw-r--r--   0 wms        (501) staff       (20)       49 2022-09-16 23:21:34.000000 mapbuffer-0.7.0/requirements.txt
--rw-r--r--   0 wms        (501) staff       (20)        6 2021-01-11 02:44:57.000000 mapbuffer-0.7.0/requirements_dev.txt
--rw-r--r--   0 wms        (501) staff       (20)      910 2023-03-27 22:22:03.616855 mapbuffer-0.7.0/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)      607 2023-03-27 19:52:03.000000 mapbuffer-0.7.0/setup.py
--rw-r--r--   0 wms        (501) staff       (20)   177052 2021-01-11 02:44:57.000000 mapbuffer-0.7.0/ten_percent_select.png
--rw-r--r--   0 wms        (501) staff       (20)      241 2023-03-15 23:09:16.000000 mapbuffer-0.7.0/tox.ini
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-27 07:58:49.516602 mapbuffer-0.7.1/
+-rw-r--r--   0 wms        (501) staff       (20)       64 2021-01-11 02:44:57.000000 mapbuffer-0.7.1/.dockerignore
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-27 07:58:49.505144 mapbuffer-0.7.1/.github/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-27 07:58:49.512029 mapbuffer-0.7.1/.github/workflows/
+-rw-r--r--   0 wms        (501) staff       (20)      927 2023-06-27 07:57:38.000000 mapbuffer-0.7.1/.github/workflows/build_wheel.yml
+-rw-r--r--   0 wms        (501) staff       (20)       52 2023-06-27 07:58:48.000000 mapbuffer-0.7.1/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)     3142 2023-06-27 07:58:48.000000 mapbuffer-0.7.1/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)     1538 2021-01-11 02:44:57.000000 mapbuffer-0.7.1/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)     6021 2023-06-27 07:58:49.516759 mapbuffer-0.7.1/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     5094 2023-03-16 15:55:02.000000 mapbuffer-0.7.1/README.md
+-rw-r--r--   0 wms        (501) staff       (20)     1425 2023-03-27 22:13:34.000000 mapbuffer-0.7.1/appveyor.yml
+-rw-r--r--   0 wms        (501) staff       (20)     4809 2023-03-27 20:40:53.000000 mapbuffer-0.7.1/automated_test.py
+-rwxr-xr-x   0 wms        (501) staff       (20)      721 2021-01-11 02:44:57.000000 mapbuffer-0.7.1/build_linux.sh
+-rw-r--r--   0 wms        (501) staff       (20)     2492 2022-09-16 23:17:07.000000 mapbuffer-0.7.1/compare_searches.c
+-rw-r--r--   0 wms        (501) staff       (20)      805 2021-01-11 02:44:57.000000 mapbuffer-0.7.1/manylinux1.Dockerfile
+-rw-r--r--   0 wms        (501) staff       (20)     1416 2021-01-11 02:44:57.000000 mapbuffer-0.7.1/manylinux2010.Dockerfile
+-rw-r--r--   0 wms        (501) staff       (20)     1771 2021-01-11 02:44:57.000000 mapbuffer-0.7.1/manylinux2014.Dockerfile
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-27 07:58:49.514676 mapbuffer-0.7.1/mapbuffer/
+-rw-r--r--   0 wms        (501) staff       (20)      885 2023-03-15 22:19:05.000000 mapbuffer-0.7.1/mapbuffer/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     5815 2023-03-15 22:19:05.000000 mapbuffer-0.7.1/mapbuffer/compression.py
+-rw-r--r--   0 wms        (501) staff       (20)      376 2021-01-11 02:44:57.000000 mapbuffer-0.7.1/mapbuffer/exceptions.py
+-rw-r--r--   0 wms        (501) staff       (20)     5014 2023-03-27 21:27:10.000000 mapbuffer-0.7.1/mapbuffer/intmap.py
+-rw-r--r--   0 wms        (501) staff       (20)     2414 2023-03-27 21:30:18.000000 mapbuffer-0.7.1/mapbuffer/lib.py
+-rw-r--r--   0 wms        (501) staff       (20)     9550 2023-06-27 01:32:25.000000 mapbuffer-0.7.1/mapbuffer/mapbuffer.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-27 07:58:49.516395 mapbuffer-0.7.1/mapbuffer.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)     6021 2023-06-27 07:58:48.000000 mapbuffer-0.7.1/mapbuffer.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      688 2023-06-27 07:58:49.000000 mapbuffer-0.7.1/mapbuffer.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-27 07:58:48.000000 mapbuffer-0.7.1/mapbuffer.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2021-01-20 01:43:04.000000 mapbuffer-0.7.1/mapbuffer.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2023-06-27 07:58:48.000000 mapbuffer-0.7.1/mapbuffer.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)       50 2023-06-27 07:58:48.000000 mapbuffer-0.7.1/mapbuffer.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)       25 2023-06-27 07:58:48.000000 mapbuffer-0.7.1/mapbuffer.egg-info/top_level.txt
+-rw-r--r--   0 wms        (501) staff       (20)     3633 2023-06-27 01:32:36.000000 mapbuffer-0.7.1/mapbufferaccel.c
+-rw-r--r--   0 wms        (501) staff       (20)     1099 2023-03-27 21:30:18.000000 mapbuffer-0.7.1/perf.py
+-rw-r--r--   0 wms        (501) staff       (20)       49 2022-09-16 23:21:34.000000 mapbuffer-0.7.1/requirements.txt
+-rw-r--r--   0 wms        (501) staff       (20)        6 2021-01-11 02:44:57.000000 mapbuffer-0.7.1/requirements_dev.txt
+-rw-r--r--   0 wms        (501) staff       (20)      910 2023-06-27 07:58:49.517548 mapbuffer-0.7.1/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)      607 2023-03-27 19:52:03.000000 mapbuffer-0.7.1/setup.py
+-rw-r--r--   0 wms        (501) staff       (20)   177052 2021-01-11 02:44:57.000000 mapbuffer-0.7.1/ten_percent_select.png
+-rw-r--r--   0 wms        (501) staff       (20)      241 2023-03-15 23:09:16.000000 mapbuffer-0.7.1/tox.ini
```

### Comparing `mapbuffer-0.7.0/.github/workflows/build_wheel.yml` & `mapbuffer-0.7.1/.github/workflows/build_wheel.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 name: Build Wheels
 
 on:  
   push:
     tags:
       - '*'
 env:
-  CIBW_SKIP: cp27-* cp33-* cp34-* cp35-* cp36* pp27* pp36* pp37*
+  CIBW_SKIP: cp27-* cp33-* cp34-* cp35-* cp36* pp27* pp36* pp37* *-musllinux*
 
 jobs:
   build_wheels:
     name: Build wheels on ${{matrix.arch}} for ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
```

### Comparing `mapbuffer-0.7.0/ChangeLog` & `mapbuffer-0.7.1/ChangeLog`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+0.7.1
+-----
+
+* build: skip musllinux
+* fix: memory leak in eytzinger\_binary\_search
+
 0.7.0
 -----
 
 * build: update cibuildwheel
 * build: add py311 to appveyor
 * fix: compile warnings
 * perf: faster, more efficient eytzinger sort for mapbuffer
```

### Comparing `mapbuffer-0.7.0/LICENSE` & `mapbuffer-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mapbuffer-0.7.0/PKG-INFO` & `mapbuffer-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapbuffer
-Version: 0.7.0
+Version: 0.7.1
 Summary: Serializable map of integers to bytes with near zero parsing.
 Home-page: https://github.com/seung-lab/mapbuffer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: BSD License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `mapbuffer-0.7.0/README.md` & `mapbuffer-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `mapbuffer-0.7.0/appveyor.yml` & `mapbuffer-0.7.1/appveyor.yml`

 * *Files identical despite different names*

### Comparing `mapbuffer-0.7.0/automated_test.py` & `mapbuffer-0.7.1/automated_test.py`

 * *Files identical despite different names*

### Comparing `mapbuffer-0.7.0/build_linux.sh` & `mapbuffer-0.7.1/build_linux.sh`

 * *Files identical despite different names*

### Comparing `mapbuffer-0.7.0/compare_searches.c` & `mapbuffer-0.7.1/compare_searches.c`

 * *Files identical despite different names*

### Comparing `mapbuffer-0.7.0/manylinux1.Dockerfile` & `mapbuffer-0.7.1/manylinux1.Dockerfile`

 * *Files identical despite different names*

### Comparing `mapbuffer-0.7.0/manylinux2010.Dockerfile` & `mapbuffer-0.7.1/manylinux2010.Dockerfile`

 * *Files identical despite different names*

### Comparing `mapbuffer-0.7.0/manylinux2014.Dockerfile` & `mapbuffer-0.7.1/manylinux2014.Dockerfile`

 * *Files identical despite different names*

### Comparing `mapbuffer-0.7.0/mapbuffer/__init__.py` & `mapbuffer-0.7.1/mapbuffer/__init__.py`

 * *Files identical despite different names*

### Comparing `mapbuffer-0.7.0/mapbuffer/compression.py` & `mapbuffer-0.7.1/mapbuffer/compression.py`

 * *Files identical despite different names*

### Comparing `mapbuffer-0.7.0/mapbuffer/intmap.py` & `mapbuffer-0.7.1/mapbuffer/intmap.py`

 * *Files identical despite different names*

### Comparing `mapbuffer-0.7.0/mapbuffer/lib.py` & `mapbuffer-0.7.1/mapbuffer/lib.py`

 * *Files identical despite different names*

### Comparing `mapbuffer-0.7.0/mapbuffer/mapbuffer.py` & `mapbuffer-0.7.1/mapbuffer/mapbuffer.py`

 * *Files identical despite different names*

### Comparing `mapbuffer-0.7.0/mapbuffer.egg-info/PKG-INFO` & `mapbuffer-0.7.1/mapbuffer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapbuffer
-Version: 0.7.0
+Version: 0.7.1
 Summary: Serializable map of integers to bytes with near zero parsing.
 Home-page: https://github.com/seung-lab/mapbuffer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: BSD License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `mapbuffer-0.7.0/mapbuffer.egg-info/SOURCES.txt` & `mapbuffer-0.7.1/mapbuffer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapbuffer-0.7.0/mapbufferaccel.c` & `mapbuffer-0.7.1/mapbufferaccel.c`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,16 @@
     
     // num bytes / 8 = uint64, then divide by two because 
     // index is [label, pos, label, pos]
     size_t N = (size_t)index.len / 2 / 8;
     uint64_t* bytes = (uint64_t*)index.buf;
 
     int64_t res = c_eytzinger_binary_search((uint64_t)label, bytes, N);
+    PyBuffer_Release(&index);
+    
     return Py_BuildValue("L", res); // L = long long
 }
 
 static PyMethodDef mapbufferaccel_methods[] = {
     {"eytzinger_binary_search", (PyCFunction)eytzinger_binary_search, METH_VARARGS, "Binary search on Eytzinger sorted mapbuffer index. Arguments: uint64_t label, uint64* index"},
     {"eytzinger_sort_indices", (PyCFunction)eytzinger_sort_indices, METH_VARARGS, "Return the Eytzinger layout as a uint32 numpy array for a given sorted array of length N. Arguments: int length"},
     {NULL, NULL, 0, NULL}
```

### Comparing `mapbuffer-0.7.0/perf.py` & `mapbuffer-0.7.1/perf.py`

 * *Files identical despite different names*

### Comparing `mapbuffer-0.7.0/setup.cfg` & `mapbuffer-0.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mapbuffer-0.7.0/setup.py` & `mapbuffer-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `mapbuffer-0.7.0/ten_percent_select.png` & `mapbuffer-0.7.1/ten_percent_select.png`

 * *Files identical despite different names*

