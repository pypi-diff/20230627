# Comparing `tmp/pyopenrivercam-0.5.0.tar.gz` & `tmp/pyopenrivercam-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopenrivercam-0.5.0.tar", last modified: Thu May 25 18:22:10 2023, max compression
+gzip compressed data, was "pyopenrivercam-0.5.1.tar", last modified: Tue Jun 27 19:09:34 2023, max compression
```

## Comparing `pyopenrivercam-0.5.0.tar` & `pyopenrivercam-0.5.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:22:10.792118 pyopenrivercam-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-05-25 18:22:10.792118 pyopenrivercam-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:22:10.788118 pyopenrivercam-0.5.0/pyopenrivercam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-05-25 18:22:10.000000 pyopenrivercam-0.5.0/pyopenrivercam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-25 18:22:10.000000 pyopenrivercam-0.5.0/pyopenrivercam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 18:22:10.000000 pyopenrivercam-0.5.0/pyopenrivercam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 18:22:10.000000 pyopenrivercam-0.5.0/pyopenrivercam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 18:22:10.000000 pyopenrivercam-0.5.0/pyopenrivercam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-25 18:22:10.000000 pyopenrivercam-0.5.0/pyopenrivercam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 18:22:10.000000 pyopenrivercam-0.5.0/pyopenrivercam.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:22:10.788118 pyopenrivercam-0.5.0/pyorc/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:22:10.792118 pyopenrivercam-0.5.0/pyorc/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40309 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/api/cameraconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    20874 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/api/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)    14887 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/api/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/api/orcbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    25778 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/api/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/api/transect.py
--rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/api/velocimetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    17689 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/api/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:22:10.792118 pyopenrivercam-0.5.0/pyorc/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20829 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/cli/cli_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/cli/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/cli/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    29408 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/cv.py
--rw-r--r--   0 runner    (1001) docker     (123)    21279 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/piv_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:22:10.792118 pyopenrivercam-0.5.0/pyorc/service/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/service/camera_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/pyorc/service/velocimetry.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 18:22:10.792118 pyopenrivercam-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:22:10.792118 pyopenrivercam-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/tests/test_cameraconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/tests/test_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/tests/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/tests/test_transect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/tests/test_velocimetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-25 18:21:55.000000 pyopenrivercam-0.5.0/tests/test_video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:09:34.530757 pyopenrivercam-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-06-27 19:09:34.530757 pyopenrivercam-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:09:34.522757 pyopenrivercam-0.5.1/pyopenrivercam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-06-27 19:09:34.000000 pyopenrivercam-0.5.1/pyopenrivercam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-27 19:09:34.000000 pyopenrivercam-0.5.1/pyopenrivercam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:09:34.000000 pyopenrivercam-0.5.1/pyopenrivercam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 19:09:34.000000 pyopenrivercam-0.5.1/pyopenrivercam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:09:34.000000 pyopenrivercam-0.5.1/pyopenrivercam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-27 19:09:34.000000 pyopenrivercam-0.5.1/pyopenrivercam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 19:09:34.000000 pyopenrivercam-0.5.1/pyopenrivercam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:09:34.522757 pyopenrivercam-0.5.1/pyorc/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:09:34.526757 pyopenrivercam-0.5.1/pyorc/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40309 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/api/cameraconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20872 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/api/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14887 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/api/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/api/orcbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26193 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/api/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/api/transect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/api/velocimetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17689 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/api/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:09:34.526757 pyopenrivercam-0.5.1/pyorc/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/cli/cli_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/cli/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/cli/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29408 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21279 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/piv_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:09:34.530757 pyopenrivercam-0.5.1/pyorc/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/service/camera_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/pyorc/service/velocimetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 19:09:34.530757 pyopenrivercam-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:09:34.530757 pyopenrivercam-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/tests/test_cameraconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/tests/test_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/tests/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/tests/test_transect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/tests/test_velocimetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-27 19:09:22.000000 pyopenrivercam-0.5.1/tests/test_video.py
```

### Comparing `pyopenrivercam-0.5.0/LICENSE` & `pyopenrivercam-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/PKG-INFO` & `pyopenrivercam-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopenrivercam
-Version: 0.5.0
+Version: 0.5.1
 Summary: pyopenrivercam (pyorc) is a front and backend to control river camera observation locations
 Home-page: https://github.com/localdevices/pyorc
 Author: Hessel Winsemius
 Author-email: winsemius@rainbowsensing.com
 License: AGPLv3
 Keywords: hydrology,hydrometry,river-flow,pyorc
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyopenrivercam-0.5.0/README.md` & `pyopenrivercam-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/pyopenrivercam.egg-info/PKG-INFO` & `pyopenrivercam-0.5.1/pyopenrivercam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopenrivercam
-Version: 0.5.0
+Version: 0.5.1
 Summary: pyopenrivercam (pyorc) is a front and backend to control river camera observation locations
 Home-page: https://github.com/localdevices/pyorc
 Author: Hessel Winsemius
 Author-email: winsemius@rainbowsensing.com
 License: AGPLv3
 Keywords: hydrology,hydrometry,river-flow,pyorc
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyopenrivercam-0.5.0/pyopenrivercam.egg-info/SOURCES.txt` & `pyopenrivercam-0.5.1/pyopenrivercam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/pyorc/api/cameraconfig.py` & `pyopenrivercam-0.5.1/pyorc/api/cameraconfig.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/pyorc/api/frames.py` & `pyopenrivercam-0.5.1/pyorc/api/frames.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,16 +58,16 @@
         # set an overlap if not provided in kwargs
         if not("overlap" in kwargs):
             kwargs["overlap"] = int(round(camera_config.window_size) / 2)
         # first get rid of coordinates that need to be recalculated
         coords_drop = list(set(self._obj.coords) - set(self._obj.dims))
         obj = self._obj.drop_vars(coords_drop)
         # get frames and shifted frames in time
-        frames1 = obj.shift(time=1)[1:].chunk({"time": 10})
-        frames2 = obj[1:].chunk({"time": 10})
+        frames1 = obj.shift(time=1)[1:].chunk({"time": 1})
+        frames2 = obj[1:].chunk({"time": 1})
 
         # get the cols and rows coordinates of the expected results
         cols, rows = piv_process.get_piv_size(
             image_size=frames1[0].shape,
             search_area_size=kwargs["search_area_size"],
             overlap=kwargs["overlap"]
         )
```

### Comparing `pyopenrivercam-0.5.0/pyorc/api/mask.py` & `pyopenrivercam-0.5.1/pyorc/api/mask.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/pyorc/api/orcbase.py` & `pyopenrivercam-0.5.1/pyorc/api/orcbase.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/pyorc/api/plot.py` & `pyopenrivercam-0.5.1/pyorc/api/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,19 @@
         Returns
         -------
         p : matplotlib mappable
             mappable of wrapped matplotlib function
 
         """
         # in case persistent transform is in kwargs_line, remove this
+        if mode == "geographical":
+            try:
+                import cartopy
+            except:
+                raise ImportError("Cartopy not found, please install with 'mamba install -c conda-forge cartopy")
         if "transform" in kwargs_line:
             del kwargs_line["transform"]
         ax = _prepare_axes(ax=ax, mode=mode)
         # update ax
 
         if len(ref._obj["v_x"].shape) > 2:
             raise OverflowError(
@@ -181,14 +186,15 @@
                 ],
                 crs=ccrs.PlateCarree()
             )
         return primitive
     return get_plot_method
 
 
+
 def _frames_plot(ref, ax=None, mode="local", *args, **kwargs):
     """Creates QuadMesh plot from a RGB or grayscale frame on a new or existing (if ax is not None) axes
     
     Wraps :py:func:`matplotlib:matplotlib.collections.QuadMesh`.
 
     Parameters
     ----------
@@ -203,14 +209,19 @@
 
     Returns
     -------
     p : matplotlib.collections.QuadMesh
 
     """
     # prepare axes
+    if mode == "geographical":
+        try:
+            import cartopy
+        except:
+            raise ImportError("Cartopy not found, please install with 'mamba install -c conda-forge cartopy")
     if "time" in ref._obj.coords:
         if ref._obj.time.size > 1:
             raise AttributeError(f'Object contains dimension "time" with length {len(ref._obj.time)}. Reduce dataset by selecting one time step or taking a median, mean or other statistic.')
     ax = _prepare_axes(ax=ax, mode=mode)
     f = ax.figure  # handle to figure
     if mode == "local":
         x = "x"
```

### Comparing `pyopenrivercam-0.5.0/pyorc/api/transect.py` & `pyopenrivercam-0.5.1/pyorc/api/transect.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,14 +182,16 @@
             f'fill_method must be "zeros", "log_fit", "log_interp", or "interpolate", instead "{fill_method}" given'
         ds = self._obj
         x = ds["xcoords"].values
         y = ds["ycoords"].values
         z = ds["zcoords"].values
         # add filled surface velocities with a logarithmic profile curve fit
         depth = self.camera_config.get_depth(z, self.h_a)
+        # make velocities zero where depth is zero
+        ds["v_eff_nofill"][:, depth<=0] = 0.
         if fill_method == "zeros":
             ds["v_eff"] = ds["v_eff_nofill"].fillna(0.)
         elif fill_method == "log_fit":
             dist_shore = self.camera_config.get_dist_shore(x, y, z, self.h_a)
             ds["v_eff"] = helpers.velocity_log_fit(ds["v_eff_nofill"], depth, dist_shore, dim="quantile")
         elif fill_method == "log_interp":
             dist_wall = self.camera_config.get_dist_wall(x, y, z, self.h_a)
```

### Comparing `pyopenrivercam-0.5.0/pyorc/api/velocimetry.py` & `pyopenrivercam-0.5.1/pyorc/api/velocimetry.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/pyorc/api/video.py` & `pyopenrivercam-0.5.1/pyorc/api/video.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/pyorc/cli/cli_elements.py` & `pyopenrivercam-0.5.1/pyorc/cli/cli_elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
-import cartopy.crs as ccrs
-import cartopy.io.img_tiles as cimgt
+try:
+    import cartopy.crs as ccrs
+    import cartopy.io.img_tiles as cimgt
+    use_cartopy = True
+except:
+    use_cartopy = False
+
 import logging
 
+
 import click
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib import patheffects
 from matplotlib.backend_bases import MouseButton
 from matplotlib.widgets import Button
 from matplotlib.patches import Polygon
@@ -24,27 +30,28 @@
     "downstream-right",
     "upstream-right"
 ]
 class BaseSelect:
     def __init__(self, img, dst=None, crs=None, buffer=0.0002, zoom_level=19, logger=logging):
         self.logger = logger
         self.height, self.width = img.shape[0:2]
-        self.crs = crs
+        if use_cartopy:
+            self.crs = crs
+        else:
+            self.crs = None
         fig = plt.figure(figsize=(16, 9), frameon=False, facecolor="black")
         fig.subplots_adjust(left=0, bottom=0, right=1, top=1, wspace=None, hspace=None)
         ax_geo = None
-        # extent = [4.5, 4.51, 51.2, 51.21]
         if dst is not None:
-            # fig = plt.figure(figsize=(12, 7))
             xmin = np.array(dst)[:, 0].min()
             xmax = np.array(dst)[:, 0].max()
             ymin = np.array(dst)[:, 1].min()
             ymax = np.array(dst)[:, 1].max()
             extent = [xmin - buffer, xmax + buffer, ymin - buffer, ymax + buffer]
-            if crs is not None:
+            if self.crs is not None:
                 tiler = getattr(cimgt, "GoogleTiles")(style="satellite")
                 ax_geo = fig.add_axes([0., 0., 1, 1], projection=tiler.crs)
                 ax_geo.set_extent(extent, crs=ccrs.PlateCarree())
                 ax_geo.add_image(tiler, zoom_level, zorder=1)
             else:
                 ax_geo = fig.add_axes([0., 0., 1, 1])
                 ax_geo.set_aspect("equal")
@@ -71,15 +78,15 @@
             zorder=4,
             path_effects=[
                 patheffects.Stroke(linewidth=3, foreground="w"),
                 patheffects.Normal(),
             ],
         )
         if dst is not None:
-            if crs is not None:
+            if self.crs is not None:
                 kwargs["transform"] = ccrs.PlateCarree()
                 transform = ccrs.PlateCarree()._as_mpl_transform(ax_geo)
                 kwargs_text["xycoords"] = transform
             self.p_geo = ax_geo.plot(
                 *list(zip(*dst))[0:2], "o",
                 **kwargs
             )
@@ -272,23 +279,23 @@
         self.p, = self.ax.plot([], [], "o", markersize=10, color="c", markeredgecolor="w", zorder=3)
         kwargs = dict(
             markersize=10,
             color="c",
             markeredgecolor="w",
             zorder=3,
         )
-        if hasattr(self.camera_config, "crs"):
+        if hasattr(self.camera_config, "crs") and use_cartopy:
             kwargs["transform"] = ccrs.PlateCarree()
         self.p_geo, = self.ax_geo.plot(
             [], [], "o",
             **kwargs
         )
         # plot an empty polygon
         pol = Polygon(np.zeros((0, 2)), edgecolor="w", alpha=0.5, linewidth=2)
-        if hasattr(self.camera_config, "crs"):
+        if hasattr(self.camera_config, "crs") and use_cartopy:
             pol_geo = Polygon(np.zeros((0, 2)), edgecolor="w", alpha=0.5, linewidth=2, transform=ccrs.PlateCarree(),
                               zorder=3)
         else:
             pol_geo = Polygon(np.zeros((0, 2)), edgecolor="w", alpha=0.5, linewidth=2, zorder=3)
         self.p_bbox_geo = self.ax_geo.add_patch(pol_geo)
         self.p_bbox = self.ax.add_patch(pol)
         xloc = self.ax.get_xlim()[0] + 50
@@ -328,15 +335,15 @@
             self.pts_t.append(pt)
             # check if all points are complete
             if len(self.src) == self.required_clicks:
                 try:
                     self.camera_config.set_bbox_from_corners(self.src)
                     bbox_cam = list(zip(*self.camera_config.get_bbox(camera=True, redistort=True).exterior.xy))
                     bbox_geo = list(zip(*self.camera_config.get_bbox().exterior.xy))
-                    if hasattr(self.camera_config, "crs"):
+                    if hasattr(self.camera_config, "crs") and use_cartopy:
                         bbox_geo = helpers.xyz_transform(
                             bbox_geo,
                             crs_from=self.camera_config.crs,
                             crs_to=4326
                         )
                     self.p_bbox.set_xy(bbox_cam)
                     self.p_bbox_geo.set_xy(bbox_geo)
@@ -364,15 +371,15 @@
         kwargs = dict(
             color="c",
             markeredgecolor="w",
             zorder=4,
             markersize=10,
             label="Selected control points"
         )
-        if crs is not None:
+        if crs is not None and use_cartopy:
             kwargs["transform"] = ccrs.PlateCarree()
         self.p_geo_selected, = self.ax_geo.plot(
             [], [], "o",
             **kwargs
         )
         if len(dst) >= 4:
             # plot an empty set of crosses for the fitted gcp row columns after optimization of perspective
@@ -395,15 +402,15 @@
             size=12,
             path_effects=path_effects
         )
         self.ax_geo.legend()
         self.ax.legend()
         self.lens_position = lens_position
         # add dst coords in the intended CRS
-        if crs is not None:
+        if crs is not None and use_cartopy:
             self.dst_crs = helpers.xyz_transform(self.dst, 4326, crs)
         else:
             self.dst_crs = self.dst
         self.required_clicks = len(self.dst)
         self.camera_matrix = None
         self.dist_coeffs = None
```

### Comparing `pyopenrivercam-0.5.0/pyorc/cli/cli_utils.py` & `pyopenrivercam-0.5.1/pyorc/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/pyorc/cli/log.py` & `pyopenrivercam-0.5.1/pyorc/cli/log.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/pyorc/cli/main.py` & `pyopenrivercam-0.5.1/pyorc/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 @click.option(
     '--debug/--no-debug',
     default=False,
     envvar='REPO_DEBUG'
 )
 @click.pass_context
 def cli(ctx, info, license, debug):  # , quiet, verbose):
-    """Command line interface for hydromt models."""
+    """Command line interface for pyOpenRiverCam."""
     if ctx.obj is None:
         ctx.obj = {}
 
     # ctx.obj["log_level"] = max(10, 30 - 10 * (verbose - quiet))
     # logging.basicConfig(stream=sys.stderr, level=ctx.obj["log_level"])
 
 
@@ -337,8 +337,8 @@
     )
     # process video following the settings
     processor.process()
     pass
 
 if __name__ == "__main__":
 #if getattr(sys, 'frozen', False):
-    cli(sys.argv[1:])
+    cli(sys.argv[1:])
```

### Comparing `pyopenrivercam-0.5.0/pyorc/const.py` & `pyopenrivercam-0.5.1/pyorc/const.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/pyorc/cv.py` & `pyopenrivercam-0.5.1/pyorc/cv.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/pyorc/helpers.py` & `pyopenrivercam-0.5.1/pyorc/helpers.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/pyorc/piv_process.py` & `pyopenrivercam-0.5.1/pyorc/piv_process.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/pyorc/service/camera_config.py` & `pyopenrivercam-0.5.1/pyorc/service/camera_config.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/pyorc/service/velocimetry.py` & `pyopenrivercam-0.5.1/pyorc/service/velocimetry.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/setup.py` & `pyopenrivercam-0.5.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="pyopenrivercam",
     description="pyopenrivercam (pyorc) is a front and backend to control river camera observation locations",
-    version="0.5.0",
+    version="0.5.1",
     long_description=readme + "\n\n",
     long_description_content_type="text/markdown",
     url="https://github.com/localdevices/pyorc",
     author="Hessel Winsemius",
     author_email="winsemius@rainbowsensing.com",
     packages=find_packages(),
     package_dir={"pyorc": "pyorc"},
@@ -24,14 +24,15 @@
     python_requires=">=3.9",
     install_requires=[
         "click",
         "cython; platform_machine == 'armv7l'",
         "dask",
         "descartes",
         "geojson",
+        "geopandas",
         "matplotlib",
         "netCDF4",
         "numpy",
         "opencv-python",
         "openpiv",
         "packaging; platform_machine == 'armv7l'",
         "pip",
```

### Comparing `pyopenrivercam-0.5.0/tests/conftest.py` & `pyopenrivercam-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/tests/test_cameraconfig.py` & `pyopenrivercam-0.5.1/tests/test_cameraconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import os
 import pyorc
 import pytest
 
-from cartopy.mpl.geoaxes import GeoAxesSubplot
+# from cartopy.mpl.geoaxes import GeoAxesSubplot
 from pyorc import helpers, cv
 
 from shapely.geometry import Polygon
 from rasterio import Affine
 import shapely
 
 def test_str(cam_config):
@@ -147,28 +147,28 @@
     assert(cam_config2.resolution == cam_config.resolution)
 
 
 @pytest.mark.parametrize(
     "camera",
     [
         True,
-        False
+#        False
     ]
 )
 def test_plot(cam_config, vid, camera):
     import matplotlib
     ax = cam_config.plot(camera=camera)
     if camera:
         assert(
             isinstance(ax, matplotlib.axes.Axes)
         )
-    else:
-        assert(
-            isinstance(ax, GeoAxesSubplot)
-        )
+    #else:
+        #assert(
+            #isinstance(ax, GeoAxesSubplot)
+        #)
 
 
 def test_cv_undistort_points(cam_config):
     # let's fake a distortion
     cam_config.dist_coeffs[0][0] = -3e-3
     src = cam_config.gcps["src"]
     mtx = cam_config.camera_matrix
```

### Comparing `pyopenrivercam-0.5.0/tests/test_cli.py` & `pyopenrivercam-0.5.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/tests/test_frames.py` & `pyopenrivercam-0.5.1/tests/test_frames.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,24 @@
 
 @pytest.mark.parametrize(
     "idx",
     [0, -1]
 )
 def test_plot_proj(frames_proj, idx):
     frames_proj[idx].frames.plot()
-    frames_proj[idx].frames.plot(mode="geographical")
+    plt.show(block=False)
     plt.close("all")
+    try:
+        import cartopy
+        frames_proj[idx].frames.plot(mode="geographical")
+        plt.show(block=False)
+        plt.close("all")
+    except:
+        print("Cartopy is missing, skipping cartopy dependent test")
+
 
 
 @pytest.mark.parametrize(
     "window_size, result",
     [
         # (5, [np.nan, np.nan, np.nan, 0.06877007]),
         (10, [0.13262428, 0.1469308 , 0.24223496, 0.14565821]),
@@ -112,8 +120,8 @@
         pytest.lazy_fixture("frames_grayscale"),
         pytest.lazy_fixture("frames_rgb_stabilize"),
         pytest.lazy_fixture("frames_proj"),
     ]
 )
 def test_to_video(frames, ani_mp4):
     # only store the first 3 frames
-    frames[0:3].frames.to_video(ani_mp4)
+    frames[0:3].frames.to_video(ani_mp4)
```

### Comparing `pyopenrivercam-0.5.0/tests/test_mask.py` & `pyopenrivercam-0.5.1/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/tests/test_transect.py` & `pyopenrivercam-0.5.1/tests/test_transect.py`

 * *Files identical despite different names*

### Comparing `pyopenrivercam-0.5.0/tests/test_velocimetry.py` & `pyopenrivercam-0.5.1/tests/test_velocimetry.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,14 +36,21 @@
         "pcolormesh",
         "scatter",
         "streamplot",
     ]
 )
 def test_plot(piv, mode, method):
     plot = True
+    if mode == "geographical":
+        try:
+            import cartopy
+        except:
+            print("Cartopy is missing, skipping cartopy dependent test")
+            plot = False
     if method == "streamplot":
         if mode != "local":
             # skipping the test, because streamplot only works local
             plot = False
     if plot:
         piv.mean(dim="time", keep_attrs=True).velocimetry.plot(method=method, mode=mode)
+        plt.show(block=False)
     plt.close("all")
```

### Comparing `pyopenrivercam-0.5.0/tests/test_video.py` & `pyopenrivercam-0.5.1/tests/test_video.py`

 * *Files identical despite different names*

