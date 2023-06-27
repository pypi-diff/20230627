# Comparing `tmp/PyThat-0.1.6.tar.gz` & `tmp/PyThat-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyThat-0.1.6.tar", last modified: Tue Jun 20 20:55:02 2023, max compression
+gzip compressed data, was "PyThat-0.1.7.tar", last modified: Tue Jun 27 16:27:20 2023, max compression
```

## Comparing `PyThat-0.1.6.tar` & `PyThat-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:55:02.080178 PyThat-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-20 20:54:48.000000 PyThat-0.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-20 20:55:02.080178 PyThat-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-20 20:54:48.000000 PyThat-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 20:54:48.000000 PyThat-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-20 20:55:02.080178 PyThat-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:55:02.080178 PyThat-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:55:02.080178 PyThat-0.1.6/src/PyThat/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-20 20:54:48.000000 PyThat-0.1.6/src/PyThat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31259 2023-06-20 20:54:48.000000 PyThat-0.1.6/src/PyThat/h5to_nc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:55:02.080178 PyThat-0.1.6/src/PyThat/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-20 20:54:48.000000 PyThat-0.1.6/src/PyThat/helpers/BLS.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 20:54:48.000000 PyThat-0.1.6/src/PyThat/helpers/FMR.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-20 20:54:48.000000 PyThat-0.1.6/src/PyThat/helpers/ROI.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 20:54:48.000000 PyThat-0.1.6/src/PyThat/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-20 20:54:48.000000 PyThat-0.1.6/src/PyThat/helpers/dB.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:55:02.080178 PyThat-0.1.6/src/PyThat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-20 20:55:02.000000 PyThat-0.1.6/src/PyThat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-20 20:55:02.000000 PyThat-0.1.6/src/PyThat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 20:55:02.000000 PyThat-0.1.6/src/PyThat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-20 20:55:02.000000 PyThat-0.1.6/src/PyThat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 20:55:02.000000 PyThat-0.1.6/src/PyThat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:27:20.772143 PyThat-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-27 16:27:07.000000 PyThat-0.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-27 16:27:20.772143 PyThat-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-27 16:27:07.000000 PyThat-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 16:27:07.000000 PyThat-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-27 16:27:20.772143 PyThat-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:27:20.764143 PyThat-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:27:20.768143 PyThat-0.1.7/src/PyThat/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-27 16:27:07.000000 PyThat-0.1.7/src/PyThat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31259 2023-06-27 16:27:07.000000 PyThat-0.1.7/src/PyThat/h5to_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:27:20.772143 PyThat-0.1.7/src/PyThat/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-27 16:27:07.000000 PyThat-0.1.7/src/PyThat/helpers/BLS.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:27:07.000000 PyThat-0.1.7/src/PyThat/helpers/FMR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-27 16:27:07.000000 PyThat-0.1.7/src/PyThat/helpers/ROI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:27:07.000000 PyThat-0.1.7/src/PyThat/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-27 16:27:07.000000 PyThat-0.1.7/src/PyThat/helpers/dB.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:27:20.768143 PyThat-0.1.7/src/PyThat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-27 16:27:20.000000 PyThat-0.1.7/src/PyThat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-27 16:27:20.000000 PyThat-0.1.7/src/PyThat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 16:27:20.000000 PyThat-0.1.7/src/PyThat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-27 16:27:20.000000 PyThat-0.1.7/src/PyThat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 16:27:20.000000 PyThat-0.1.7/src/PyThat.egg-info/top_level.txt
```

### Comparing `PyThat-0.1.6/LICENSE.txt` & `PyThat-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyThat-0.1.6/PKG-INFO` & `PyThat-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyThat
-Version: 0.1.6
+Version: 0.1.7
 Summary: Read Thatec h5 formatting and convert it to netcdf files and xarray objects.
 Home-page: https://github.com/mrschweizer/PyThat
 Author: Matthias Schweizer
 Author-email: mareschweizer@gmail.com
 Project-URL: Bug Tracker, https://github.com/mrschweizer/PyThat/issues
 Project-URL: Documentation, https://pythat.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyThat-0.1.6/README.md` & `PyThat-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `PyThat-0.1.6/setup.cfg` & `PyThat-0.1.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = PyThat
-version = 0.1.6
+version = 0.1.7
 author = Matthias Schweizer
 author_email = mareschweizer@gmail.com
 description = Read Thatec h5 formatting and convert it to netcdf files and xarray objects.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mrschweizer/PyThat
 project_urls =
```

### Comparing `PyThat-0.1.6/src/PyThat/h5to_nc.py` & `PyThat-0.1.7/src/PyThat/h5to_nc.py`

 * *Files identical despite different names*

### Comparing `PyThat-0.1.6/src/PyThat/helpers/BLS.py` & `PyThat-0.1.7/src/PyThat/helpers/BLS.py`

 * *Files identical despite different names*

### Comparing `PyThat-0.1.6/src/PyThat/helpers/ROI.py` & `PyThat-0.1.7/src/PyThat/helpers/ROI.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             slices_one_dimension = [el.sum(key) for el in slices_one_dimension]
         x = xr.concat(slices_one_dimension, key)
         x = x.assign_coords({key: [str(x) for x in coord_range_edges]})
     return x
 
 
 xr.DataArray.slice_accumulate = slice_accumulate
-xr.DataSet.slice_accumulate = slice_accumulate
+xr.Dataset.slice_accumulate = slice_accumulate
 
 
 if __name__ == '__main__':
     import matplotlib.pyplot as plt
     a = np.linspace(-5, 5, 11)
     b = np.linspace(-7, 7, 15)
     A, B = np.meshgrid(a, b, indexing='ij')
```

### Comparing `PyThat-0.1.6/src/PyThat.egg-info/PKG-INFO` & `PyThat-0.1.7/src/PyThat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyThat
-Version: 0.1.6
+Version: 0.1.7
 Summary: Read Thatec h5 formatting and convert it to netcdf files and xarray objects.
 Home-page: https://github.com/mrschweizer/PyThat
 Author: Matthias Schweizer
 Author-email: mareschweizer@gmail.com
 Project-URL: Bug Tracker, https://github.com/mrschweizer/PyThat/issues
 Project-URL: Documentation, https://pythat.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
```

