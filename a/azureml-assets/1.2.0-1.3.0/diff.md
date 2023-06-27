# Comparing `tmp/azureml-assets-1.2.0.tar.gz` & `tmp/azureml-assets-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azureml-assets-1.2.0.tar", last modified: Fri Jun 23 15:38:33 2023, max compression
+gzip compressed data, was "azureml-assets-1.3.0.tar", last modified: Tue Jun 27 16:59:41 2023, max compression
```

## Comparing `azureml-assets-1.2.0.tar` & `azureml-assets-1.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:38:33.393058 azureml-assets-1.2.0/
--rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-06-23 15:38:33.393058 azureml-assets-1.2.0/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:38:33.385058 azureml-assets-1.2.0/azureml/
--rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:38:33.389058 azureml-assets-1.2.0/azureml/assets/
--rw-r--r--   0 vsts      (1001) docker     (123)      764 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4119 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/asset_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    36392 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6521 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/copy_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8518 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/deployment_config.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:38:33.389058 azureml-assets-1.2.0/azureml/assets/environment/
--rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/environment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15375 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/environment/build.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6897 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/environment/pin_image_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5124 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/environment/pin_package_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/environment/pin_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4436 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/extract_tagged_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:38:33.389058 azureml-assets-1.2.0/azureml/assets/model/
--rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1187 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/model/mlflow_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3408 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/model/utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2869 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/tag_released_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11282 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/update_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5934 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/update_spec.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:38:33.393058 azureml-assets-1.2.0/azureml/assets/util/
--rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6906 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/util/logger.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/util/template.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15565 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/util/util.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16581 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/azureml/assets/validate_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:38:33.393058 azureml-assets-1.2.0/azureml_assets.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-06-23 15:38:33.000000 azureml-assets-1.2.0/azureml_assets.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      979 2023-06-23 15:38:33.000000 azureml-assets-1.2.0/azureml_assets.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-23 15:38:33.000000 azureml-assets-1.2.0/azureml_assets.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-06-23 15:38:33.000000 azureml-assets-1.2.0/azureml_assets.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-06-23 15:38:33.000000 azureml-assets-1.2.0/azureml_assets.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-23 15:38:33.393058 azureml-assets-1.2.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1275 2023-06-23 15:37:54.000000 azureml-assets-1.2.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 16:59:41.791803 azureml-assets-1.3.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-06-27 16:59:41.791803 azureml-assets-1.3.0/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 16:59:41.787803 azureml-assets-1.3.0/azureml/
+-rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 16:59:41.787803 azureml-assets-1.3.0/azureml/assets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      764 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4119 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/asset_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    36392 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7115 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/copy_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8518 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/deployment_config.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 16:59:41.787803 azureml-assets-1.3.0/azureml/assets/environment/
+-rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/environment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15375 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/environment/build.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6897 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/environment/pin_image_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5124 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/environment/pin_package_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/environment/pin_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4436 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/extract_tagged_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 16:59:41.791803 azureml-assets-1.3.0/azureml/assets/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1187 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/model/mlflow_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3408 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/model/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2869 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/tag_released_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11282 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/update_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5934 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/update_spec.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 16:59:41.791803 azureml-assets-1.3.0/azureml/assets/util/
+-rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6906 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/util/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/util/template.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15565 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/util/util.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16581 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/azureml/assets/validate_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 16:59:41.791803 azureml-assets-1.3.0/azureml_assets.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-06-27 16:59:41.000000 azureml-assets-1.3.0/azureml_assets.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      979 2023-06-27 16:59:41.000000 azureml-assets-1.3.0/azureml_assets.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-27 16:59:41.000000 azureml-assets-1.3.0/azureml_assets.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-06-27 16:59:41.000000 azureml-assets-1.3.0/azureml_assets.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-06-27 16:59:41.000000 azureml-assets-1.3.0/azureml_assets.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-27 16:59:41.791803 azureml-assets-1.3.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1275 2023-06-27 16:59:01.000000 azureml-assets-1.3.0/setup.py
```

### Comparing `azureml-assets-1.2.0/PKG-INFO` & `azureml-assets-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureml-assets
-Version: 1.2.0
+Version: 1.3.0
 Summary: Utilities for publishing assets to Azure Machine Learning system registries.
 Author: Microsoft Corp
 License: MIT
 Project-URL: Source, https://github.com/Azure/azureml-assets/
 Project-URL: Changelog, https://github.com/Azure/azureml-assets/blob/main/scripts/azureml-assets/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `azureml-assets-1.2.0/azureml/assets/__init__.py` & `azureml-assets-1.3.0/azureml/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/azureml/assets/asset_utils.py` & `azureml-assets-1.3.0/azureml/assets/asset_utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/azureml/assets/config.py` & `azureml-assets-1.3.0/azureml/assets/config.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/azureml/assets/copy_assets.py` & `azureml-assets-1.3.0/azureml/assets/copy_assets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 
 """Copy assets from directory to another."""
 
 import argparse
 import re
+from collections import Counter
 from pathlib import Path
+from string import Template
 from typing import List
 from urllib.error import HTTPError
 
 import azureml.assets as assets
 import azureml.assets.util as util
 from azureml.assets.util import logger
 from azureml.assets.config import AssetType
 
 COPIED_COUNT = "copied_count"
+COPIED_TYPE_COUNT = Template("copied_${type}_count")
 
 
 def copy_asset(asset_config: assets.AssetConfig,
                output_directory_root: Path,
                release_directory_root: Path = None,
                use_version_dir: bool = False,
                check_previous_release: bool = False) -> str:
@@ -81,30 +84,34 @@
         release_directory_root (Path, optional): Release directory location. Defaults to None.
         use_version_dirs (bool, optional): Use version directories for output. Defaults to False.
         pattern (re.Pattern, optional): Regex pattern for assets to copy. Defaults to None.
     """
     # Find assets under release dir
     asset_count = 0
     copied_count = 0
+    copied_type_counter = Counter()
     for asset_config in util.find_assets(input_dirs, asset_config_filename, pattern=pattern):
         asset_count += 1
 
         # Copy asset if tag doesn't exist or release_directory_root isn't specified
         version = copy_asset(asset_config=asset_config,
                              output_directory_root=output_directory_root,
                              release_directory_root=release_directory_root,
                              use_version_dir=use_version_dirs,
                              check_previous_release=check_previous_release)
         if version:
             logger.print(f"Copied {asset_config.type.value} {asset_config.name} version {version}")
             copied_count += 1
+            copied_type_counter[asset_config.type] += 1
     logger.print(f"{copied_count} of {asset_count} asset(s) copied")
 
     # Set variables
     logger.set_output(COPIED_COUNT, copied_count)
+    for type, count in copied_type_counter.items():
+        logger.set_output(COPIED_TYPE_COUNT.substitute(type=type.value), count)
 
 
 if __name__ == '__main__':
     # Handle command-line args
     parser = argparse.ArgumentParser()
     parser.add_argument("-i", "--input-dirs", required=True,
                         help="Comma-separated list of directories containing assets")
@@ -115,18 +122,22 @@
     parser.add_argument("-r", "--release-directory", type=Path,
                         help="Directory to which the release branch has been cloned. "
                         "If provided, only asset versions without a release tag will be copied.")
     parser.add_argument("-v", "--use-version-dirs", action="store_true",
                         help="Use version directories when storing assets in output directory")
     parser.add_argument("-t", "--pattern", type=re.compile,
                         help="Regex pattern to select assets to copy, in the format <type>/<name>/<version>")
-    parser.add_argument("-p", "--check_previous_release", action="store_true",
-                        help="Checks if previous release exists")
+    parser.add_argument("-p", "--check-previous-release", action="store_true",
+                        help="Check if previous release exists (environments only)")
     args = parser.parse_args()
 
+    # Ensure --release-directory is specified if --check-previous-release is
+    if args.check_previous_release and args.release_directory is None:
+        parser.error("--check-previous-release requires --release-directory")
+
     # Convert comma-separated values to lists
     input_dirs = [Path(d) for d in args.input_dirs.split(",")]
 
     # Copy assets
     copy_assets(input_dirs=input_dirs,
                 output_directory_root=args.output_directory,
                 asset_config_filename=args.asset_config_filename,
```

### Comparing `azureml-assets-1.2.0/azureml/assets/deployment_config.py` & `azureml-assets-1.3.0/azureml/assets/deployment_config.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/azureml/assets/environment/build.py` & `azureml-assets-1.3.0/azureml/assets/environment/build.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/azureml/assets/environment/pin_image_versions.py` & `azureml-assets-1.3.0/azureml/assets/environment/pin_image_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/azureml/assets/environment/pin_package_versions.py` & `azureml-assets-1.3.0/azureml/assets/environment/pin_package_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/azureml/assets/environment/pin_versions.py` & `azureml-assets-1.3.0/azureml/assets/environment/pin_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/azureml/assets/extract_tagged_assets.py` & `azureml-assets-1.3.0/azureml/assets/extract_tagged_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/azureml/assets/model/mlflow_utils.py` & `azureml-assets-1.3.0/azureml/assets/model/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/azureml/assets/model/utils.py` & `azureml-assets-1.3.0/azureml/assets/model/utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/azureml/assets/tag_released_assets.py` & `azureml-assets-1.3.0/azureml/assets/tag_released_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/azureml/assets/update_assets.py` & `azureml-assets-1.3.0/azureml/assets/update_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/azureml/assets/update_spec.py` & `azureml-assets-1.3.0/azureml/assets/update_spec.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/azureml/assets/util/__init__.py` & `azureml-assets-1.3.0/azureml/assets/util/__init__.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/azureml/assets/util/logger.py` & `azureml-assets-1.3.0/azureml/assets/util/logger.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/azureml/assets/util/template.py` & `azureml-assets-1.3.0/azureml/assets/util/template.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/azureml/assets/util/util.py` & `azureml-assets-1.3.0/azureml/assets/util/util.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/azureml/assets/validate_assets.py` & `azureml-assets-1.3.0/azureml/assets/validate_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/azureml_assets.egg-info/PKG-INFO` & `azureml-assets-1.3.0/azureml_assets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureml-assets
-Version: 1.2.0
+Version: 1.3.0
 Summary: Utilities for publishing assets to Azure Machine Learning system registries.
 Author: Microsoft Corp
 License: MIT
 Project-URL: Source, https://github.com/Azure/azureml-assets/
 Project-URL: Changelog, https://github.com/Azure/azureml-assets/blob/main/scripts/azureml-assets/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `azureml-assets-1.2.0/azureml_assets.egg-info/SOURCES.txt` & `azureml-assets-1.3.0/azureml_assets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.2.0/setup.py` & `azureml-assets-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """Set up azureml-assets package."""
 
 from setuptools import setup, find_packages
 
 setup(
    name="azureml-assets",
-   version="1.2.0",
+   version="1.3.0",
    description="Utilities for publishing assets to Azure Machine Learning system registries.",
    author="Microsoft Corp",
    packages=find_packages(),
    install_requires=[
       "GitPython>=3.1",
       "ruamel.yaml==0.17.21",
       "pip>=21",
```

