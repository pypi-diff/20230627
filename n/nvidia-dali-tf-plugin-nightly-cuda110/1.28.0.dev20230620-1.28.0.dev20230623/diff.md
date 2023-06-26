# Comparing `tmp/nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620.tar.gz` & `tmp/nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620.tar", last modified: Wed Jun 21 16:03:32 2023, max compression
+gzip compressed data, was "nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623.tar", last modified: Mon Jun 26 23:43:28 2023, max compression
```

## Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620.tar` & `nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-21 16:03:32.568578 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      469 2023-06-21 16:03:32.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 10:03:35.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       37 2023-06-21 16:03:32.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-06-21 16:03:32.568578 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      316 2023-06-21 16:03:32.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-21 16:03:32.567578 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-06-21 16:03:32.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      297 2023-06-21 16:03:32.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-21 16:03:32.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-21 16:03:32.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-21 16:03:32.568578 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 10:03:35.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-26 23:43:28.407073 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      469 2023-06-26 23:43:28.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 04:38:44.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       37 2023-06-26 23:43:28.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-06-26 23:43:28.407073 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      316 2023-06-26 23:43:28.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-26 23:43:28.407073 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-06-26 23:43:28.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      297 2023-06-26 23:43:28.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-26 23:43:28.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-26 23:43:28.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-26 23:43:28.407073 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 04:38:44.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623/setup.py
```

### Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620/LICENSE.md` & `nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620/PKG-INFO` & `nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-nightly-cuda110
-Version: 1.28.0.dev20230620
+Version: 1.28.0.dev20230623
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/PKG-INFO` & `nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-nightly-cuda110
-Version: 1.28.0.dev20230620
+Version: 1.28.0.dev20230623
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230620/setup.py` & `nvidia-dali-tf-plugin-nightly-cuda110-1.28.0.dev20230623/setup.py`

 * *Files identical despite different names*

