# Comparing `tmp/rushd-0.4.0.tar.gz` & `tmp/rushd-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rushd-0.4.0.tar", last modified: Fri Apr 21 13:22:50 2023, max compression
+gzip compressed data, was "rushd-0.4.1.tar", last modified: Tue Jun 27 16:28:16 2023, max compression
```

## Comparing `rushd-0.4.0.tar` & `rushd-0.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-04-21 13:22:50.693870 rushd-0.4.0/
--rw-r--r--   0 christopher  (1000) christopher  (1000)     1069 2022-08-30 19:04:22.000000 rushd-0.4.0/LICENSE
--rw-r--r--   0 christopher  (1000) christopher  (1000)     3824 2023-04-21 13:22:50.693870 rushd-0.4.0/PKG-INFO
--rw-r--r--   0 christopher  (1000) christopher  (1000)     2856 2023-04-21 13:20:40.000000 rushd-0.4.0/README.md
--rw-r--r--   0 christopher  (1000) christopher  (1000)      527 2023-02-02 22:08:57.000000 rushd-0.4.0/pyproject.toml
--rw-r--r--   0 christopher  (1000) christopher  (1000)       38 2023-04-21 13:22:50.693870 rushd-0.4.0/setup.cfg
--rw-r--r--   0 christopher  (1000) christopher  (1000)     1885 2023-04-21 13:13:34.000000 rushd-0.4.0/setup.py
-drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-04-21 13:22:50.683870 rushd-0.4.0/src/
-drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-04-21 13:22:50.687204 rushd-0.4.0/src/rushd/
--rw-r--r--   0 christopher  (1000) christopher  (1000)      651 2023-04-19 21:24:37.000000 rushd-0.4.0/src/rushd/__init__.py
--rw-r--r--   0 christopher  (1000) christopher  (1000)    15001 2023-04-19 19:55:19.000000 rushd-0.4.0/src/rushd/flow.py
--rw-r--r--   0 christopher  (1000) christopher  (1000)    11309 2023-02-02 21:36:26.000000 rushd-0.4.0/src/rushd/io.py
--rw-r--r--   0 christopher  (1000) christopher  (1000)     6509 2023-04-21 13:09:39.000000 rushd-0.4.0/src/rushd/plot.py
--rw-r--r--   0 christopher  (1000) christopher  (1000)     6281 2023-04-19 19:55:18.000000 rushd-0.4.0/src/rushd/well_mapper.py
-drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-04-21 13:22:50.687204 rushd-0.4.0/src/rushd.egg-info/
--rw-r--r--   0 christopher  (1000) christopher  (1000)     3824 2023-04-21 13:22:50.000000 rushd-0.4.0/src/rushd.egg-info/PKG-INFO
--rw-r--r--   0 christopher  (1000) christopher  (1000)      440 2023-04-21 13:22:50.000000 rushd-0.4.0/src/rushd.egg-info/SOURCES.txt
--rw-r--r--   0 christopher  (1000) christopher  (1000)        1 2023-04-21 13:22:50.000000 rushd-0.4.0/src/rushd.egg-info/dependency_links.txt
--rw-r--r--   0 christopher  (1000) christopher  (1000)      210 2023-04-21 13:22:50.000000 rushd-0.4.0/src/rushd.egg-info/requires.txt
--rw-r--r--   0 christopher  (1000) christopher  (1000)        6 2023-04-21 13:22:50.000000 rushd-0.4.0/src/rushd.egg-info/top_level.txt
-drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-04-21 13:22:50.690537 rushd-0.4.0/tests/
--rw-r--r--   0 christopher  (1000) christopher  (1000)    11898 2023-02-02 22:12:16.000000 rushd-0.4.0/tests/test_file_io.py
--rw-r--r--   0 christopher  (1000) christopher  (1000)     3607 2023-02-02 22:12:16.000000 rushd-0.4.0/tests/test_file_moi.py
--rw-r--r--   0 christopher  (1000) christopher  (1000)    18337 2023-03-24 17:26:34.000000 rushd-0.4.0/tests/test_flow.py
--rw-r--r--   0 christopher  (1000) christopher  (1000)      891 2023-02-02 22:12:16.000000 rushd-0.4.0/tests/test_pandas_cache.py
--rw-r--r--   0 christopher  (1000) christopher  (1000)     4469 2023-04-19 20:32:45.000000 rushd-0.4.0/tests/test_plot.py
--rw-r--r--   0 christopher  (1000) christopher  (1000)     3274 2023-02-02 22:12:16.000000 rushd-0.4.0/tests/test_well_mapper.py
+drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-06-27 16:28:16.027449 rushd-0.4.1/
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     1069 2022-08-30 19:04:22.000000 rushd-0.4.1/LICENSE
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     3950 2023-06-27 16:28:16.027449 rushd-0.4.1/PKG-INFO
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     2982 2023-06-27 16:26:42.000000 rushd-0.4.1/README.md
+-rw-r--r--   0 christopher  (1000) christopher  (1000)      527 2023-02-02 22:08:57.000000 rushd-0.4.1/pyproject.toml
+-rw-r--r--   0 christopher  (1000) christopher  (1000)       38 2023-06-27 16:28:16.027449 rushd-0.4.1/setup.cfg
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     1885 2023-06-27 16:26:11.000000 rushd-0.4.1/setup.py
+drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-06-27 16:28:16.020782 rushd-0.4.1/src/
+drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-06-27 16:28:16.024116 rushd-0.4.1/src/rushd/
+-rw-r--r--   0 christopher  (1000) christopher  (1000)      651 2023-04-19 21:24:37.000000 rushd-0.4.1/src/rushd/__init__.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)    15035 2023-06-08 19:55:56.000000 rushd-0.4.1/src/rushd/flow.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)    11323 2023-06-08 19:55:36.000000 rushd-0.4.1/src/rushd/io.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     6548 2023-06-08 19:54:47.000000 rushd-0.4.1/src/rushd/plot.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     6268 2023-06-08 19:55:12.000000 rushd-0.4.1/src/rushd/well_mapper.py
+drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-06-27 16:28:16.024116 rushd-0.4.1/src/rushd.egg-info/
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     3950 2023-06-27 16:28:16.000000 rushd-0.4.1/src/rushd.egg-info/PKG-INFO
+-rw-r--r--   0 christopher  (1000) christopher  (1000)      440 2023-06-27 16:28:16.000000 rushd-0.4.1/src/rushd.egg-info/SOURCES.txt
+-rw-r--r--   0 christopher  (1000) christopher  (1000)        1 2023-06-27 16:28:16.000000 rushd-0.4.1/src/rushd.egg-info/dependency_links.txt
+-rw-r--r--   0 christopher  (1000) christopher  (1000)      210 2023-06-27 16:28:16.000000 rushd-0.4.1/src/rushd.egg-info/requires.txt
+-rw-r--r--   0 christopher  (1000) christopher  (1000)        6 2023-06-27 16:28:16.000000 rushd-0.4.1/src/rushd.egg-info/top_level.txt
+drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-06-27 16:28:16.027449 rushd-0.4.1/tests/
+-rw-r--r--   0 christopher  (1000) christopher  (1000)    11898 2023-02-02 22:12:16.000000 rushd-0.4.1/tests/test_file_io.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     3607 2023-02-02 22:12:16.000000 rushd-0.4.1/tests/test_file_moi.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)    18337 2023-03-24 17:26:34.000000 rushd-0.4.1/tests/test_flow.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)      891 2023-02-02 22:12:16.000000 rushd-0.4.1/tests/test_pandas_cache.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     4845 2023-06-02 21:07:49.000000 rushd-0.4.1/tests/test_plot.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     3274 2023-02-02 22:12:16.000000 rushd-0.4.1/tests/test_well_mapper.py
```

### Comparing `rushd-0.4.0/LICENSE` & `rushd-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rushd-0.4.0/PKG-INFO` & `rushd-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rushd
-Version: 0.4.0
+Version: 0.4.1
 Summary: Package for maintaining robust, reproducible data management.
 Home-page: https://github.com/GallowayLabMIT/rushd
 Author: Christopher Johnstone, Kasey Love, Conrad Oakes
 Author-email: meson800@gmail.com
 Project-URL: Bug Tracker, https://github.com/GallowayLabMIT/rushd/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -68,14 +68,17 @@
 ```
 After this 'local install', you can use and import `rushd` freely without
 having to re-install after each update.
 
 ## Changelog
 See the [CHANGELOG](CHANGELOG.md) for detailed changes.
 ```
+## [0.4.1] - 2023-06-27
+### Modified
+- Updated the `rd.plot.plot_mapping` command to properly handle the single-numeric case.
 ## [0.4.0] - 2023-04-21
 ### Added
 - `rd.plot.plot_well_metadata` to make nice plots corresponding to well metadata specified as a YAML file.
 ```
 
 ## License
 This is licensed by the MIT license. Use freely!
```

### Comparing `rushd-0.4.0/README.md` & `rushd-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,17 @@
 ```
 After this 'local install', you can use and import `rushd` freely without
 having to re-install after each update.
 
 ## Changelog
 See the [CHANGELOG](CHANGELOG.md) for detailed changes.
 ```
+## [0.4.1] - 2023-06-27
+### Modified
+- Updated the `rd.plot.plot_mapping` command to properly handle the single-numeric case.
 ## [0.4.0] - 2023-04-21
 ### Added
 - `rd.plot.plot_well_metadata` to make nice plots corresponding to well metadata specified as a YAML file.
 ```
 
 ## License
 This is licensed by the MIT license. Use freely!
```

### Comparing `rushd-0.4.0/pyproject.toml` & `rushd-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rushd-0.4.0/setup.py` & `rushd-0.4.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rushd",
-    version="0.4.0",
+    version="0.4.1",
     author="Christopher Johnstone, Kasey Love, Conrad Oakes",
     author_email="meson800@gmail.com",
     description="Package for maintaining robust, reproducible data management.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/GallowayLabMIT/rushd",
     project_urls={
```

### Comparing `rushd-0.4.0/src/rushd/__init__.py` & `rushd-0.4.1/src/rushd/__init__.py`

 * *Files identical despite different names*

### Comparing `rushd-0.4.0/src/rushd/flow.py` & `rushd-0.4.1/src/rushd/flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
             if isinstance(v, dict):
                 warnings.warn(
                     f'Metadata column "{k}" is a YAML dictionary, not a list!'
                     " Make sure your entries under this key start with dashes."
                     " Passing a dictionary does not allow duplicate keys and"
                     " is sort-order-dependent.",
                     MetadataWarning,
+                    stacklevel=2,
                 )
     return {k: well_mapper.well_mapping(v) for k, v in metadata["metadata"].items()}
 
 
 def load_csv_with_metadata(
     data_path: Union[str, Path], yaml_path: Union[str, Path], filename_regex: Optional[str] = None
 ) -> pd.DataFrame:
```

### Comparing `rushd-0.4.0/src/rushd/io.py` & `rushd-0.4.1/src/rushd/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     rootdir = datadir_txt.parent
     datadir = Path(datadir_txt.read_text().strip("\n"))
     return (rootdir if rootdir.is_dir() else None, datadir if datadir.is_dir() else None)
 
 
 _rootdir, _datadir = _load_root_datadir(_locate_datadir_txt())
 if _datadir is None:
-    warnings.warn("Unable to locate datadir.txt", category=ImportWarning)
+    warnings.warn("Unable to locate datadir.txt", category=ImportWarning, stacklevel=2)
 
 
 def __getattr__(name: str) -> Path:
     """
     Set up module exports.
 
     rushd.io exports two attributes,
```

### Comparing `rushd-0.4.0/src/rushd/plot.py` & `rushd-0.4.1/src/rushd/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     """
     if fig is None:
         fig = plt.figure()
     ax = fig.subplots()  # type: ignore
 
     if plate_size is None:
         # Check if we have any wells beyond H or beyond 12
-        if any([k[0] > "H" or int(k[1:]) > 12 for k in mapping.keys()]):
+        if any(k[0] > "H" or int(k[1:]) > 12 for k in mapping.keys()):
             plate_size = (24, 16)
         else:
             plate_size = (12, 8)
 
     # Only use the two-digit mappings so they sort properly
     sorted_mapping_values = [
         t[1]
@@ -62,15 +62,15 @@
         )
     ]
     mapping_vals = sorted(set(sorted_mapping_values), key=lambda x: sorted_mapping_values.index(x))
     if style is None:
         # Autodetect mapping.
         # If it is all numbers, then we find the median. If all numbers are non-negative
         # and the median lies outside [.15, .85] percentile ranges, guess log scale.
-        if not all([isinstance(x, (int, float)) for x in mapping_vals]):
+        if not all(isinstance(x, (int, float)) for x in mapping_vals):
             style = "category"
         else:
             min_val = min(mapping_vals)
             max_val = max(mapping_vals)
 
             if min_val < 0 or max_val == min_val:
                 style = "linear"
@@ -88,15 +88,16 @@
         }
     elif style == "linear":
         mapping_vals = sorted(mapping_vals)
         min_val = min(mapping_vals)
         max_val = max(mapping_vals)
         base_cmap = plt.get_cmap("viridis")  # type: ignore
         mapping_colors = {
-            x: base_cmap((x - min_val) / (max_val - min_val) * 0.85) for x in mapping_vals
+            x: base_cmap((x - min_val) / (max_val - min_val) * 0.85 if min_val != max_val else 0.0)
+            for x in mapping_vals
         }
     elif style == "log":
         mapping_vals = sorted(mapping_vals)
         min_nonzero_val = min([x for x in mapping_vals if x > 0])
         max_val = max(mapping_vals)
         base_cmap = plt.get_cmap("viridis")  # type: ignore
         mapping_colors = {}
```

### Comparing `rushd-0.4.0/src/rushd/well_mapper.py` & `rushd-0.4.1/src/rushd/well_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,17 +122,17 @@
     # Save plate_spec into a list of a single dictionary if it isn't already
     # an iterable of dictionaries
     if isinstance(plate_spec, Dict):
         plate_spec = [plate_spec]
 
     # Char To Int mapping and Int To Char mapping
     cti_mapping = {v: k for k, v in enumerate(list("ABCDEFGHIJKLMNOP"))}
-    itc_mapping = {
-        k: v for k, v in enumerate(list("ABCDEFGHIJKLMNOP"))
-    }  # pylint: disable=unnecessary-comprehension
+    itc_mapping = dict(
+        enumerate(list("ABCDEFGHIJKLMNOP"))
+    )  # pylint: disable=unnecessary-comprehension
 
     output_mapping: Dict[str, Any] = {}
     for mapping_dict in plate_spec:
         for key, val in mapping_dict.items():
             if len(val) == 0:
                 raise ValueError("Empty mapping spec is not allowed!")
             # Remove all whitespace
```

### Comparing `rushd-0.4.0/src/rushd.egg-info/PKG-INFO` & `rushd-0.4.1/src/rushd.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rushd
-Version: 0.4.0
+Version: 0.4.1
 Summary: Package for maintaining robust, reproducible data management.
 Home-page: https://github.com/GallowayLabMIT/rushd
 Author: Christopher Johnstone, Kasey Love, Conrad Oakes
 Author-email: meson800@gmail.com
 Project-URL: Bug Tracker, https://github.com/GallowayLabMIT/rushd/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -68,14 +68,17 @@
 ```
 After this 'local install', you can use and import `rushd` freely without
 having to re-install after each update.
 
 ## Changelog
 See the [CHANGELOG](CHANGELOG.md) for detailed changes.
 ```
+## [0.4.1] - 2023-06-27
+### Modified
+- Updated the `rd.plot.plot_mapping` command to properly handle the single-numeric case.
 ## [0.4.0] - 2023-04-21
 ### Added
 - `rd.plot.plot_well_metadata` to make nice plots corresponding to well metadata specified as a YAML file.
 ```
 
 ## License
 This is licensed by the MIT license. Use freely!
```

### Comparing `rushd-0.4.0/tests/test_file_io.py` & `rushd-0.4.1/tests/test_file_io.py`

 * *Files identical despite different names*

### Comparing `rushd-0.4.0/tests/test_file_moi.py` & `rushd-0.4.1/tests/test_file_moi.py`

 * *Files identical despite different names*

### Comparing `rushd-0.4.0/tests/test_flow.py` & `rushd-0.4.1/tests/test_flow.py`

 * *Files identical despite different names*

### Comparing `rushd-0.4.0/tests/test_pandas_cache.py` & `rushd-0.4.1/tests/test_pandas_cache.py`

 * *Files identical despite different names*

### Comparing `rushd-0.4.0/tests/test_plot.py` & `rushd-0.4.1/tests/test_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,7 +119,16 @@
     Test that larger plates can be processed
     """
     with (tmp_path / "metadata.yaml").open("w") as meta_file:
         meta_file.write("metadata:\n  example:\n    - test: A1-G14")
     mapping = rushd.flow.load_well_metadata(tmp_path / "metadata.yaml")
     rushd.plot.plot_mapping(mapping["example"])
     plt.close()
+
+
+def test_single_entry_zero(tmp_path: Path):
+    """Tests that single entries where max=min do not crash the plotter"""
+    with (tmp_path / "metadata.yaml").open("w") as meta_file:
+        meta_file.write("metadata:\n  foo:\n    - 0: A1-H6")
+    mapping = rushd.flow.load_well_metadata(tmp_path / "metadata.yaml")
+    rushd.plot.plot_mapping(mapping["foo"])
+    plt.close()
```

### Comparing `rushd-0.4.0/tests/test_well_mapper.py` & `rushd-0.4.1/tests/test_well_mapper.py`

 * *Files identical despite different names*

