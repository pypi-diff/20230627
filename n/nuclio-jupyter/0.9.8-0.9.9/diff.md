# Comparing `tmp/nuclio-jupyter-0.9.8.tar.gz` & `tmp/nuclio-jupyter-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nuclio-jupyter-0.9.8.tar", last modified: Thu Feb  2 12:03:11 2023, max compression
+gzip compressed data, was "dist/nuclio-jupyter-0.9.9.tar", last modified: Thu Feb 23 13:31:31 2023, max compression
```

## Comparing `nuclio-jupyter-0.9.8.tar` & `nuclio-jupyter-0.9.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 alonm      (501) staff       (20)        0 2023-02-02 12:03:11.687512 nuclio-jupyter-0.9.8/
--rw-r--r--   0 alonm      (501) staff       (20)    11357 2021-02-23 15:54:13.000000 nuclio-jupyter-0.9.8/LICENSE.txt
--rw-r--r--   0 alonm      (501) staff       (20)      743 2021-02-23 15:54:13.000000 nuclio-jupyter-0.9.8/MANIFEST.in
--rw-r--r--   0 alonm      (501) staff       (20)     1402 2023-02-02 12:02:50.000000 nuclio-jupyter-0.9.8/Makefile
--rw-r--r--   0 alonm      (501) staff       (20)    28048 2023-02-02 12:03:11.687682 nuclio-jupyter-0.9.8/PKG-INFO
--rw-r--r--   0 alonm      (501) staff       (20)      600 2023-02-02 12:02:50.000000 nuclio-jupyter-0.9.8/Pipfile
--rw-r--r--   0 alonm      (501) staff       (20)    92126 2023-02-02 12:02:50.000000 nuclio-jupyter-0.9.8/Pipfile.lock
--rw-r--r--   0 alonm      (501) staff       (20)    27070 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.8/README.md
-drwxr-xr-x   0 alonm      (501) staff       (20)        0 2023-02-02 12:03:11.670935 nuclio-jupyter-0.9.8/nuclio/
--rw-r--r--   0 alonm      (501) staff       (20)     1105 2023-02-02 12:02:50.000000 nuclio-jupyter-0.9.8/nuclio/__init__.py
--rw-r--r--   0 alonm      (501) staff       (20)     1799 2021-02-23 15:54:13.000000 nuclio-jupyter-0.9.8/nuclio/__main__.py
--rw-r--r--   0 alonm      (501) staff       (20)    10295 2021-02-23 15:54:13.000000 nuclio-jupyter-0.9.8/nuclio/archive.py
--rw-r--r--   0 alonm      (501) staff       (20)     1728 2022-09-28 13:21:10.000000 nuclio-jupyter-0.9.8/nuclio/auth.py
--rw-r--r--   0 alonm      (501) staff       (20)     8419 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.8/nuclio/build.py
--rw-r--r--   0 alonm      (501) staff       (20)    11652 2023-02-02 12:02:50.000000 nuclio-jupyter-0.9.8/nuclio/config.py
--rw-r--r--   0 alonm      (501) staff       (20)    26775 2022-11-28 14:36:59.000000 nuclio-jupyter-0.9.8/nuclio/deploy.py
--rw-r--r--   0 alonm      (501) staff       (20)    17301 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.8/nuclio/export.py
--rw-r--r--   0 alonm      (501) staff       (20)    14513 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.8/nuclio/magic.py
--rw-r--r--   0 alonm      (501) staff       (20)     7476 2022-11-28 14:36:59.000000 nuclio-jupyter-0.9.8/nuclio/request.py
--rw-r--r--   0 alonm      (501) staff       (20)     8891 2022-11-06 08:55:43.000000 nuclio-jupyter-0.9.8/nuclio/triggers.py
--rw-r--r--   0 alonm      (501) staff       (20)     7071 2023-01-26 07:19:17.000000 nuclio-jupyter-0.9.8/nuclio/utils.py
-drwxr-xr-x   0 alonm      (501) staff       (20)        0 2023-02-02 12:03:11.674384 nuclio-jupyter-0.9.8/nuclio_jupyter.egg-info/
--rw-r--r--   0 alonm      (501) staff       (20)    28048 2023-02-02 12:03:11.000000 nuclio-jupyter-0.9.8/nuclio_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 alonm      (501) staff       (20)      990 2023-02-02 12:03:11.000000 nuclio-jupyter-0.9.8/nuclio_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 alonm      (501) staff       (20)        1 2023-02-02 12:03:11.000000 nuclio-jupyter-0.9.8/nuclio_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 alonm      (501) staff       (20)      109 2023-02-02 12:03:11.000000 nuclio-jupyter-0.9.8/nuclio_jupyter.egg-info/entry_points.txt
--rw-r--r--   0 alonm      (501) staff       (20)        1 2023-02-02 12:03:11.000000 nuclio-jupyter-0.9.8/nuclio_jupyter.egg-info/not-zip-safe
--rw-r--r--   0 alonm      (501) staff       (20)      130 2023-02-02 12:03:11.000000 nuclio-jupyter-0.9.8/nuclio_jupyter.egg-info/requires.txt
--rw-r--r--   0 alonm      (501) staff       (20)        7 2023-02-02 12:03:11.000000 nuclio-jupyter-0.9.8/nuclio_jupyter.egg-info/top_level.txt
--rw-r--r--   0 alonm      (501) staff       (20)      136 2023-02-02 12:03:11.688357 nuclio-jupyter-0.9.8/setup.cfg
--rw-r--r--   0 alonm      (501) staff       (20)     3817 2023-02-02 12:02:50.000000 nuclio-jupyter-0.9.8/setup.py
-drwxr-xr-x   0 alonm      (501) staff       (20)        0 2023-02-02 12:03:11.687204 nuclio-jupyter-0.9.8/tests/
--rw-r--r--   0 alonm      (501) staff       (20)     1589 2022-09-28 13:21:10.000000 nuclio-jupyter-0.9.8/tests/annotations_test_cases.yml
--rw-r--r--   0 alonm      (501) staff       (20)     2451 2022-09-28 13:21:10.000000 nuclio-jupyter-0.9.8/tests/cell_and_line_magic_test_cases.yml
--rw-r--r--   0 alonm      (501) staff       (20)     5945 2022-09-28 13:21:10.000000 nuclio-jupyter-0.9.8/tests/code_generation_test_cases.yml
--rw-r--r--   0 alonm      (501) staff       (20)     1242 2021-02-23 15:54:13.000000 nuclio-jupyter-0.9.8/tests/conftest.py
--rw-r--r--   0 alonm      (501) staff       (20)     1316 2021-02-23 15:54:13.000000 nuclio-jupyter-0.9.8/tests/convert_cases.yml
--rw-r--r--   0 alonm      (501) staff       (20)     6287 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.8/tests/deploy.json
--rw-r--r--   0 alonm      (501) staff       (20)       11 2021-02-23 15:54:13.000000 nuclio-jupyter-0.9.8/tests/env.txt
--rw-r--r--   0 alonm      (501) staff       (20)     4994 2021-02-23 15:54:13.000000 nuclio-jupyter-0.9.8/tests/handler.ipynb
--rw-r--r--   0 alonm      (501) staff       (20)      689 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.8/tests/handler.py
--rw-r--r--   0 alonm      (501) staff       (20)     1858 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.8/tests/tags-test.ipynb
--rw-r--r--   0 alonm      (501) staff       (20)     4402 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.8/tests/test_build.py
--rw-r--r--   0 alonm      (501) staff       (20)     3066 2022-11-06 08:55:43.000000 nuclio-jupyter-0.9.8/tests/test_config.py
--rw-r--r--   0 alonm      (501) staff       (20)     7080 2022-11-28 14:36:59.000000 nuclio-jupyter-0.9.8/tests/test_deploy.py
--rw-r--r--   0 alonm      (501) staff       (20)     8456 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.8/tests/test_export.py
--rw-r--r--   0 alonm      (501) staff       (20)     1614 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.8/tests/test_install.py
--rw-r--r--   0 alonm      (501) staff       (20)     1169 2021-02-23 15:54:13.000000 nuclio-jupyter-0.9.8/tests/test_magic.py
--rw-r--r--   0 alonm      (501) staff       (20)     1304 2022-11-28 14:36:59.000000 nuclio-jupyter-0.9.8/tests/test_request.py
--rw-r--r--   0 alonm      (501) staff       (20)     2036 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.8/tests/test_triggers.py
--rw-r--r--   0 alonm      (501) staff       (20)     1731 2023-02-02 12:02:50.000000 nuclio-jupyter-0.9.8/tests/test_utils.py
+drwxr-xr-x   0 alonm      (501) staff       (20)        0 2023-02-23 13:31:31.702720 nuclio-jupyter-0.9.9/
+-rw-r--r--   0 alonm      (501) staff       (20)    11357 2021-02-23 15:54:13.000000 nuclio-jupyter-0.9.9/LICENSE.txt
+-rw-r--r--   0 alonm      (501) staff       (20)      743 2021-02-23 15:54:13.000000 nuclio-jupyter-0.9.9/MANIFEST.in
+-rw-r--r--   0 alonm      (501) staff       (20)     1402 2023-02-02 12:02:50.000000 nuclio-jupyter-0.9.9/Makefile
+-rw-r--r--   0 alonm      (501) staff       (20)    28048 2023-02-23 13:31:31.702909 nuclio-jupyter-0.9.9/PKG-INFO
+-rw-r--r--   0 alonm      (501) staff       (20)      582 2023-02-23 13:30:59.000000 nuclio-jupyter-0.9.9/Pipfile
+-rw-r--r--   0 alonm      (501) staff       (20)    95589 2023-02-23 13:30:59.000000 nuclio-jupyter-0.9.9/Pipfile.lock
+-rw-r--r--   0 alonm      (501) staff       (20)    27070 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.9/README.md
+drwxr-xr-x   0 alonm      (501) staff       (20)        0 2023-02-23 13:31:31.690568 nuclio-jupyter-0.9.9/nuclio/
+-rw-r--r--   0 alonm      (501) staff       (20)     1105 2023-02-23 13:30:59.000000 nuclio-jupyter-0.9.9/nuclio/__init__.py
+-rw-r--r--   0 alonm      (501) staff       (20)     1799 2021-02-23 15:54:13.000000 nuclio-jupyter-0.9.9/nuclio/__main__.py
+-rw-r--r--   0 alonm      (501) staff       (20)    10295 2021-02-23 15:54:13.000000 nuclio-jupyter-0.9.9/nuclio/archive.py
+-rw-r--r--   0 alonm      (501) staff       (20)     1728 2022-09-28 13:21:10.000000 nuclio-jupyter-0.9.9/nuclio/auth.py
+-rw-r--r--   0 alonm      (501) staff       (20)     8419 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.9/nuclio/build.py
+-rw-r--r--   0 alonm      (501) staff       (20)    11652 2023-02-02 12:02:50.000000 nuclio-jupyter-0.9.9/nuclio/config.py
+-rw-r--r--   0 alonm      (501) staff       (20)    26775 2022-11-28 14:36:59.000000 nuclio-jupyter-0.9.9/nuclio/deploy.py
+-rw-r--r--   0 alonm      (501) staff       (20)    17301 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.9/nuclio/export.py
+-rw-r--r--   0 alonm      (501) staff       (20)    14513 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.9/nuclio/magic.py
+-rw-r--r--   0 alonm      (501) staff       (20)     7476 2022-11-28 14:36:59.000000 nuclio-jupyter-0.9.9/nuclio/request.py
+-rw-r--r--   0 alonm      (501) staff       (20)     8891 2022-11-06 08:55:43.000000 nuclio-jupyter-0.9.9/nuclio/triggers.py
+-rw-r--r--   0 alonm      (501) staff       (20)     7071 2023-01-26 07:19:17.000000 nuclio-jupyter-0.9.9/nuclio/utils.py
+drwxr-xr-x   0 alonm      (501) staff       (20)        0 2023-02-23 13:31:31.692961 nuclio-jupyter-0.9.9/nuclio_jupyter.egg-info/
+-rw-r--r--   0 alonm      (501) staff       (20)    28048 2023-02-23 13:31:31.000000 nuclio-jupyter-0.9.9/nuclio_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 alonm      (501) staff       (20)      990 2023-02-23 13:31:31.000000 nuclio-jupyter-0.9.9/nuclio_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 alonm      (501) staff       (20)        1 2023-02-23 13:31:31.000000 nuclio-jupyter-0.9.9/nuclio_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 alonm      (501) staff       (20)      109 2023-02-23 13:31:31.000000 nuclio-jupyter-0.9.9/nuclio_jupyter.egg-info/entry_points.txt
+-rw-r--r--   0 alonm      (501) staff       (20)        1 2023-02-02 12:03:11.000000 nuclio-jupyter-0.9.9/nuclio_jupyter.egg-info/not-zip-safe
+-rw-r--r--   0 alonm      (501) staff       (20)      198 2023-02-23 13:31:31.000000 nuclio-jupyter-0.9.9/nuclio_jupyter.egg-info/requires.txt
+-rw-r--r--   0 alonm      (501) staff       (20)        7 2023-02-23 13:31:31.000000 nuclio-jupyter-0.9.9/nuclio_jupyter.egg-info/top_level.txt
+-rw-r--r--   0 alonm      (501) staff       (20)      136 2023-02-23 13:31:31.703415 nuclio-jupyter-0.9.9/setup.cfg
+-rw-r--r--   0 alonm      (501) staff       (20)     3970 2023-02-23 13:30:59.000000 nuclio-jupyter-0.9.9/setup.py
+drwxr-xr-x   0 alonm      (501) staff       (20)        0 2023-02-23 13:31:31.702123 nuclio-jupyter-0.9.9/tests/
+-rw-r--r--   0 alonm      (501) staff       (20)     1589 2022-09-28 13:21:10.000000 nuclio-jupyter-0.9.9/tests/annotations_test_cases.yml
+-rw-r--r--   0 alonm      (501) staff       (20)     2451 2022-09-28 13:21:10.000000 nuclio-jupyter-0.9.9/tests/cell_and_line_magic_test_cases.yml
+-rw-r--r--   0 alonm      (501) staff       (20)     5945 2022-09-28 13:21:10.000000 nuclio-jupyter-0.9.9/tests/code_generation_test_cases.yml
+-rw-r--r--   0 alonm      (501) staff       (20)     1242 2021-02-23 15:54:13.000000 nuclio-jupyter-0.9.9/tests/conftest.py
+-rw-r--r--   0 alonm      (501) staff       (20)     1316 2021-02-23 15:54:13.000000 nuclio-jupyter-0.9.9/tests/convert_cases.yml
+-rw-r--r--   0 alonm      (501) staff       (20)     6287 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.9/tests/deploy.json
+-rw-r--r--   0 alonm      (501) staff       (20)       11 2021-02-23 15:54:13.000000 nuclio-jupyter-0.9.9/tests/env.txt
+-rw-r--r--   0 alonm      (501) staff       (20)     4994 2021-02-23 15:54:13.000000 nuclio-jupyter-0.9.9/tests/handler.ipynb
+-rw-r--r--   0 alonm      (501) staff       (20)      689 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.9/tests/handler.py
+-rw-r--r--   0 alonm      (501) staff       (20)     1858 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.9/tests/tags-test.ipynb
+-rw-r--r--   0 alonm      (501) staff       (20)     4402 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.9/tests/test_build.py
+-rw-r--r--   0 alonm      (501) staff       (20)     3066 2022-11-06 08:55:43.000000 nuclio-jupyter-0.9.9/tests/test_config.py
+-rw-r--r--   0 alonm      (501) staff       (20)     7080 2022-11-28 14:36:59.000000 nuclio-jupyter-0.9.9/tests/test_deploy.py
+-rw-r--r--   0 alonm      (501) staff       (20)     8456 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.9/tests/test_export.py
+-rw-r--r--   0 alonm      (501) staff       (20)     1614 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.9/tests/test_install.py
+-rw-r--r--   0 alonm      (501) staff       (20)     1169 2021-02-23 15:54:13.000000 nuclio-jupyter-0.9.9/tests/test_magic.py
+-rw-r--r--   0 alonm      (501) staff       (20)     1304 2022-11-28 14:36:59.000000 nuclio-jupyter-0.9.9/tests/test_request.py
+-rw-r--r--   0 alonm      (501) staff       (20)     2036 2022-09-28 13:20:51.000000 nuclio-jupyter-0.9.9/tests/test_triggers.py
+-rw-r--r--   0 alonm      (501) staff       (20)     1731 2023-02-02 12:02:50.000000 nuclio-jupyter-0.9.9/tests/test_utils.py
```

### Comparing `nuclio-jupyter-0.9.8/LICENSE.txt` & `nuclio-jupyter-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/MANIFEST.in` & `nuclio-jupyter-0.9.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/Makefile` & `nuclio-jupyter-0.9.9/Makefile`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/PKG-INFO` & `nuclio-jupyter-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclio-jupyter
-Version: 0.9.8
+Version: 0.9.9
 Summary: Convert Jupyter notebook to nuclio
 Home-page: https://github.com/nuclio/nuclio-jupyter
 Author: Miki Tebeka
 Author-email: miki@353solutions.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `nuclio-jupyter-0.9.8/Pipfile` & `nuclio-jupyter-0.9.9/Pipfile`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [[source]]
 url = "https://pypi.org/simple"
 verify_ssl = true
 name = "pypi"
 
 [packages]
-ipython = "~=7.0"
 nbconvert = ">=6.4.5"
 notebook = ">=6.4"
 # pyyaml 6.0 added backwards incompatible change https://github.com/yaml/pyyaml/issues/576
 pyyaml = ">=3.13, <6.0.0"
 requests = ">=2.20.1"
 # nbconvert is not compatible with tornado 6 (which is in alpha)
 #tornado = ">=5"
```

### Comparing `nuclio-jupyter-0.9.8/Pipfile.lock` & `nuclio-jupyter-0.9.9/Pipfile.lock`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9340916480862133%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'cb04a1b551f4bf64689256fa0422a8db5309623ee53e23438bf75a7ba006026f'}}",*

 * * "'default'": "{'boto3': {'hashes': "*

 * *              "['sha256:17f0d782487275cac12676a61b3f1a4900954cc454c842b8551ca47a3dcd59b4', "*

 * *              "'sha256:bf808f7433629650128ab577a9d4a0f4daf072d9f2f3a907b9d567a6952d9154'], "*

 * *              "'version': '==1.26.77'}, 'botocore': {'hashes': "*

 * *              "['sha256:9d94a02f2584b52c65fb3cb309fb1b29d6d0c36d69062722b0275c1c382c44c9', "*

 * *            […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "da11196ad9f7e66119d0d1419f0e87fa9c5ec090c91e040922e9bd2e148db356"
+            "sha256": "cb04a1b551f4bf64689256fa0422a8db5309623ee53e23438bf75a7ba006026f"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
@@ -61,14 +61,29 @@
                 "sha256:ed2937d286e2ad0cc79a7087d3c272832865f779430e0cc2b4f3718d3159b0cb",
                 "sha256:f1152ac548bd5b8bcecfb0b0371f082037e47128653df2e8ba6e914d384f3c3e",
                 "sha256:f9f8b450ed0547e3d473fdc8612083fd08dd2120d6ac8f73828df9b7d45bb351"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==21.2.0"
         },
+        "arrow": {
+            "hashes": [
+                "sha256:3934b30ca1b9f292376d9db15b19446088d12ec58629bc3f0da28fd55fb633a1",
+                "sha256:5a49ab92e3b7b71d96cd6bfcc4df14efefc9dfa96ea19045815914a6ab6b1fe2"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==1.2.3"
+        },
+        "asttokens": {
+            "hashes": [
+                "sha256:4622110b2a6f30b77e1473affaa97e711bc2f07d3f10848420ff1898edbe94f3",
+                "sha256:6b0ac9e93fb0335014d382b8fa9b3afa7df546984258005da0b9e7095b3deb1c"
+            ],
+            "version": "==2.2.1"
+        },
         "attrs": {
             "hashes": [
                 "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836",
                 "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==22.2.0"
@@ -94,27 +109,27 @@
                 "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==6.0.0"
         },
         "boto3": {
             "hashes": [
-                "sha256:5194c16e1f2371c25ee038e8291faf99117b4f2d272d70f48851ba47bcea44b4",
-                "sha256:78d75f6a08c33618d9ce37acca78e4f80e316a8ce3ac040c562f8054afe6451e"
+                "sha256:17f0d782487275cac12676a61b3f1a4900954cc454c842b8551ca47a3dcd59b4",
+                "sha256:bf808f7433629650128ab577a9d4a0f4daf072d9f2f3a907b9d567a6952d9154"
             ],
             "index": "pypi",
-            "version": "==1.26.61"
+            "version": "==1.26.77"
         },
         "botocore": {
             "hashes": [
-                "sha256:22ead51f900e3465d0e4e670d02d091e613c88be8b333c47bfda727f8988eef3",
-                "sha256:c7a7133d02c5e9a8fcc9e5a238bf15bde2d5369366553520332a88bc05b7358a"
+                "sha256:9d94a02f2584b52c65fb3cb309fb1b29d6d0c36d69062722b0275c1c382c44c9",
+                "sha256:d8aa7bffe2422de282b2d02945b7b45d5fecf00f67b65eebb0b1fa3de1abc6d0"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.61"
+            "version": "==1.29.77"
         },
         "certifi": {
             "hashes": [
                 "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
                 "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
             ],
             "markers": "python_version >= '3.6'",
@@ -278,14 +293,22 @@
                 "sha256:f6f45710b4459401609ebebdbcfb34515da4fc2aa886f95107f556ac69a9147e",
                 "sha256:f97e83fa6c25693c7a35de154681fcc257c1c41b38beb0304b9c4d2d9e164479",
                 "sha256:f9d0c5c045a3ca9bedfc35dca8526798eb91a07aa7a2c0fee134c6c6f321cbd7",
                 "sha256:ff6f3db31555657f3163b15a6b7c6938d08df7adbfc9dd13d9d19edad678f1e8"
             ],
             "version": "==3.0.1"
         },
+        "comm": {
+            "hashes": [
+                "sha256:3e2f5826578e683999b93716285b3b1f344f157bf75fa9ce0a797564e742f062",
+                "sha256:9f3abf3515112fa7c55a42a6a5ab358735c9dccc8b5910a9d8e3ef5998130666"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==0.1.2"
+        },
         "debugpy": {
             "hashes": [
                 "sha256:0ea1011e94416e90fb3598cc3ef5e08b0a4dd6ce6b9b33ccd436c1dffc8cd664",
                 "sha256:11a0f3a106f69901e4a9a5683ce943a7a5605696024134b522aa1bfda25b5fec",
                 "sha256:23363e6d2a04d726bbc1400bd4e9898d54419b36b2cdf7020e3e215e1dcd0f8e",
                 "sha256:23c29e40e39ad7d869d408ded414f6d46d82f8a93b5857ac3ac1e915893139ca",
                 "sha256:549ae0cb2d34fc09d1675f9b01942499751d174381b6082279cf19cdb3c47cbe",
@@ -318,76 +341,81 @@
             "hashes": [
                 "sha256:1bb3032db185915b62d7c6209c5a8792be6a32ab2fedacc84e01b52c51aa3e69",
                 "sha256:a352e7e428770286cc899e2542b6cdaedb2b4953ff269a210103ec58f6198a61"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==0.7.1"
         },
-        "entrypoints": {
+        "executing": {
             "hashes": [
-                "sha256:b706eddaa9218a19ebcd67b56818f05bb27589b1ca9e8d797b74affad4ccacd4",
-                "sha256:f174b5ff827504fd3cd97cc3f8649f3693f51538c7e4bdf3ef002c8429d42f9f"
+                "sha256:0314a69e37426e3608aada02473b4161d4caf5a4b244d1d0c48072b8fee7bacc",
+                "sha256:19da64c18d2d851112f09c287f8d3dbbdf725ab0e569077efb6cdcbd3497c107"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==0.4"
+            "version": "==1.2.0"
         },
         "fastjsonschema": {
             "hashes": [
                 "sha256:01e366f25d9047816fe3d288cbfc3e10541daf0af2044763f3d0ade42476da18",
                 "sha256:21f918e8d9a1a4ba9c22e09574ba72267a6762d47822db9add95f6454e51cc1c"
             ],
             "version": "==2.16.2"
         },
+        "fqdn": {
+            "hashes": [
+                "sha256:105ed3677e767fb5ca086a0c1f4bb66ebc3c100be518f0e0d755d9eae164d89f",
+                "sha256:3a179af3761e4df6eb2e026ff9e1a3033d3587bf980a0b1b2e1e5d08d7358014"
+            ],
+            "version": "==1.5.1"
+        },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==3.4"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:057e92c15bc8d9e8109738a48db0ccb31b4d9d5cfbee5a8670879a30be66304b",
-                "sha256:b7e52a1f8dec14a75ea73e0891f3060099ca1d8e6a462a4dff11c3e119ea1b31"
+                "sha256:7efb448ec9a5e313a57655d35aa54cd3e01b7e1fbcf72dce1bf06119420f5bad",
+                "sha256:e354bedeb60efa6affdcc8ae121b73544a7aa74156d047311948f6d711cd378d"
             ],
-            "index": "pypi",
-            "version": "==4.2.0"
-        },
-        "importlib-resources": {
-            "hashes": [
-                "sha256:7d543798b0beca10b6a01ac7cafda9f822c54db9e8376a6bf57e0cbd74d486b6",
-                "sha256:e4a96c8cc0339647ff9a5e0550d9f276fc5a01ffa276012b58ec108cfd7b8484"
-            ],
-            "markers": "python_version < '3.9'",
-            "version": "==5.10.2"
+            "markers": "python_version < '3.10'",
+            "version": "==6.0.0"
         },
         "ipykernel": {
             "hashes": [
-                "sha256:463f3d87a92e99969b1605cb7a5b4d7b36b7145a0e72d06e65918a6ddefbe630",
-                "sha256:67daf93e5b52456cd8eea87a8b59405d2bb80ae411864a1ea206c3631d8179af"
+                "sha256:430d00549b6aaf49bd0f5393150691edb1815afa62d457ee6b1a66b25cb17874",
+                "sha256:6e9213484e4ce1fb14267ee435e18f23cc3a0634e635b9fb4ed4677b84e0fdf8"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==6.16.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==6.21.2"
         },
         "ipython": {
             "hashes": [
-                "sha256:af3bdb46aa292bce5615b1b2ebc76c2080c5f77f54bda2ec72461317273e7cd6",
-                "sha256:c175d2440a1caff76116eb719d40538fbb316e214eda85c5515c303aacbfb23e"
+                "sha256:b13a1d6c1f5818bd388db53b7107d17454129a70de2b87481d555daede5eb49e",
+                "sha256:b38c31e8fc7eff642fc7c597061fff462537cf2314e3225a19c906b7b0d8a345"
             ],
             "index": "pypi",
-            "version": "==7.34.0"
+            "version": "==8.10.0"
         },
         "ipython-genutils": {
             "hashes": [
                 "sha256:72dd37233799e619666c9f639a9da83c34013a73e8bbc79a7a6348d93c61fab8",
                 "sha256:eb2e116e75ecef9d4d228fdc66af54269afa26ab4463042e33785b887c628ba8"
             ],
             "version": "==0.2.0"
         },
+        "isoduration": {
+            "hashes": [
+                "sha256:ac2f9015137935279eac671f94f89eb00584f940f5dc49462a0c4ee692ba1bd9",
+                "sha256:b2904c2a4228c3d44f409c8ae8e2370eb21a26f7ac2ec5446df141dde3452042"
+            ],
+            "version": "==20.11.0"
+        },
         "jedi": {
             "hashes": [
                 "sha256:203c1fd9d969ab8f2119ec0a3342e0b49910045abe6af0a3ae83a5764d54639e",
                 "sha256:bae794c30d07f6d910d32a7048af09b5a39ed740918da923c6b780790ebac612"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.18.2"
@@ -404,45 +432,71 @@
             "hashes": [
                 "sha256:02e2e4cc71b5bcab88332eebf907519190dd9e6e82107fa7f83b1003a6252980",
                 "sha256:90261b206d6defd58fdd5e85f478bf633a2901798906be2ad389150c5c60edbe"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.1"
         },
+        "jsonpointer": {
+            "hashes": [
+                "sha256:51801e558539b4e9cd268638c078c6c5746c9ac96bc38152d443400e4f3793e9",
+                "sha256:97cba51526c829282218feb99dab1b1e6bdf8efd1c43dc9d57be093c0d69c99a"
+            ],
+            "version": "==2.3"
+        },
         "jsonschema": {
+            "extras": [
+                "format-nongpl"
+            ],
             "hashes": [
                 "sha256:0f864437ab8b6076ba6707453ef8f98a6a0d512a80e93f8abdb676f737ecb60d",
                 "sha256:a870ad254da1a8ca84b6a2905cac29d265f805acc57af304784962a2aa6508f6"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.17.3"
         },
         "jupyter-client": {
             "hashes": [
-                "sha256:214668aaea208195f4c13d28eb272ba79f945fc0cf3f11c7092c20b2ca1980e7",
-                "sha256:52be28e04171f07aed8f20e1616a5a552ab9fee9cbbe6c1896ae170c3880d392"
+                "sha256:be48ac6bd659cbbddb7a674cf06b3b8afbf53f228253cf58bde604c03bd487b0",
+                "sha256:ed65498bea6d876ef9d8da3e0db3dd33c5d129f5b2645f56ae03993782966bd0"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==7.4.9"
+            "markers": "python_version >= '3.8'",
+            "version": "==8.0.3"
         },
         "jupyter-core": {
             "hashes": [
-                "sha256:87f39d7642412ae8a52291cc68e71ac01dfa2c735df2701f8108251d51b4f460",
-                "sha256:a54672c539333258495579f6964144924e0aa7b07f7069947bef76d7ea5cb4c1"
+                "sha256:1407cdb4c79ee467696c04b76633fc1884015fa109323365a6372c8e890cc83f",
+                "sha256:4bdc2928c37f6917130c667d8b8708f20aee539d8283c6be72aabd2a4b4c83b0"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==5.2.0"
+        },
+        "jupyter-events": {
+            "hashes": [
+                "sha256:57a2749f87ba387cd1bfd9b22a0875b889237dbf2edc2121ebb22bde47036c17",
+                "sha256:9a6e9995f75d1b7146b436ea24d696ce3a35bfa8bfe45e0c33c334c79464d0b3"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.12.0"
+            "version": "==0.6.3"
         },
         "jupyter-server": {
             "hashes": [
-                "sha256:a2caa759e2a29ece1aad013c58215fe951f38317b97de462b921834955fe3fca",
-                "sha256:d42e520af98af9fbb7f0fb0d069991054d88e4d2ee051eb7110aef35f3756cef"
+                "sha256:29d6657bfb160b0e39b9030d67f33f918a188f2eba28065314a933b327fef872",
+                "sha256:b15078954120886d580e19d1746e2b62a3dc7bd082cb4716115c25fcd7061b00"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==1.23.5"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.3.0"
+        },
+        "jupyter-server-terminals": {
+            "hashes": [
+                "sha256:57ab779797c25a7ba68e97bcfb5d7740f2b5e8a83b5e8102b10438041a7eac5d",
+                "sha256:75779164661cec02a8758a5311e18bb8eb70c4e86c6b699403100f1585a12a36"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==0.4.4"
         },
         "jupyterlab-pygments": {
             "hashes": [
                 "sha256:2405800db07c9f770863bcf8049a529c3dd4d3e28536638bd7c1c01d2748309f",
                 "sha256:7405d7fde60819d905a9fa8ce89e4cd830e318cdad22a0030f7a901da705585d"
             ],
             "markers": "python_version >= '3.7'",
@@ -510,26 +564,26 @@
                 "sha256:f887e5f10ba98e8d2b150ddcf4702c1e5f8b3a20005eb0f74bfdbd360ee6f304"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==0.1.6"
         },
         "mistune": {
             "hashes": [
-                "sha256:182cc5ee6f8ed1b807de6b7bb50155df7b66495412836b9a74c8fbdfc75fe36d",
-                "sha256:9ee0a66053e2267aba772c71e06891fa8f1af6d4b01d5e84e267b4570d4d9808"
+                "sha256:0246113cb2492db875c6be56974a7c893333bf26cd92891c85f63151cee09d34",
+                "sha256:bad7f5d431886fcbaf5f758118ecff70d31f75231b34024a1341120340a65ce8"
             ],
-            "version": "==2.0.4"
+            "version": "==2.0.5"
         },
         "nbclassic": {
             "hashes": [
-                "sha256:32c235e1f22f4048f3b877d354c198202898797cf9c2085856827598cead001b",
-                "sha256:8e8ffce7582bb7a4baf11fa86a3d88b184e8e7df78eed4ead69f15aa4fc0e323"
+                "sha256:40f11bbcc59e8956c3d5ef132dec8e5a853e893ecf831e791d54da0d8a50d79d",
+                "sha256:6403a996562dadefa7fee9c49e17b663b5fd508241de5df655b90011cf3342d9"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.5.1"
+            "version": "==0.5.2"
         },
         "nbclient": {
             "hashes": [
                 "sha256:884a3f4a8c4fc24bb9302f263e0af47d97f0d01fe11ba714171b320c8ac09547",
                 "sha256:d97ac6257de2794f5397609df754fcbca1a603e94e924eb9b99787c031ae2e7c"
             ],
             "markers": "python_version >= '3.7'",
@@ -610,37 +664,37 @@
         "pickleshare": {
             "hashes": [
                 "sha256:87683d47965c1da65cdacaf31c8441d12b8044cdec9aca500cd78fc2c683afca",
                 "sha256:9649af414d74d4df115d5d718f82acb59c9d418196b7b4290ed47a12ce62df56"
             ],
             "version": "==0.7.5"
         },
-        "pkgutil-resolve-name": {
+        "platformdirs": {
             "hashes": [
-                "sha256:357d6c9e6a755653cfd78893817c0853af365dd51ec97f3d358a819373bbd174",
-                "sha256:ca27cc078d25c5ad71a9de0a7a330146c4e014c2462d9af19c6b828280649c5e"
+                "sha256:8a1228abb1ef82d788f74139988b137e78692984ec7b08eaa6c65f1723af28f9",
+                "sha256:b1d5eb14f221506f50d6604a561f4c5786d9e80355219694a1b244bcd96f4567"
             ],
-            "markers": "python_version < '3.9'",
-            "version": "==1.3.10"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.0.0"
         },
         "prometheus-client": {
             "hashes": [
                 "sha256:0836af6eb2c8f4fed712b2f279f6c0a8bbab29f9f4aa15276b91c7cb0d1616ab",
                 "sha256:a03e35b359f14dd1630898543e2120addfdeacd1a6069c1367ae90fd93ad3f48"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.16.0"
         },
         "prompt-toolkit": {
             "hashes": [
-                "sha256:3e163f254bef5a03b146397d7c1963bd3e2812f0964bb9a24e6ec761fd28db63",
-                "sha256:aa64ad242a462c5ff0363a7b9cfe696c20d55d9fc60c11fd8e632d064804d305"
+                "sha256:6a2948ec427dfcc7c983027b1044b355db6aaa8be374f54ad2015471f7d81c5b",
+                "sha256:d5d73d4b5eb1a92ba884a88962b157f49b71e06c4348b417dd622b25cdd3800b"
             ],
-            "markers": "python_full_version >= '3.6.2'",
-            "version": "==3.0.36"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.0.37"
         },
         "psutil": {
             "hashes": [
                 "sha256:149555f59a69b33f056ba1c4eb22bb7bf24332ce631c44a319cec09f876aaeff",
                 "sha256:16653106f3b59386ffe10e0bad3bb6299e169d5327d3f187614b1cb8f24cf2e1",
                 "sha256:3d7f9739eb435d4b1338944abe23f49584bde5395f27487d2ee25ad9a8774a62",
                 "sha256:3ff89f9b835100a825b14c2808a106b6fdcc4b15483141482a12c725e7f78549",
@@ -662,14 +716,21 @@
             "hashes": [
                 "sha256:4b41f3967fce3af57cc7e94b888626c18bf37a083e3651ca8feeb66d492fef35",
                 "sha256:5c5d0a3b48ceee0b48485e0c26037c0acd7d29765ca3fbb5cb3831d347423220"
             ],
             "markers": "os_name != 'nt'",
             "version": "==0.7.0"
         },
+        "pure-eval": {
+            "hashes": [
+                "sha256:01eaab343580944bc56080ebe0a674b39ec44a945e6d09ba7db3cb8cec289350",
+                "sha256:2b45320af6dfaa1750f543d714b6d1c520a1688dec6fd24d339063ce0aaa9ac3"
+            ],
+            "version": "==0.2.2"
+        },
         "pycparser": {
             "hashes": [
                 "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
                 "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.21"
@@ -719,14 +780,22 @@
             "hashes": [
                 "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.8.2"
         },
+        "python-json-logger": {
+            "hashes": [
+                "sha256:23e7ec02d34237c5aa1e29a070193a4ea87583bb4e7f8fd06d3de8264c4b2e1c",
+                "sha256:f380b826a991ebbe3de4d897aeec42760035ac760345e57b812938dc8b35e2bd"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==2.0.7"
+        },
         "pyyaml": {
             "hashes": [
                 "sha256:08682f6b72c722394747bddaf0aa62277e02557c0fd1c42cb853016a38f8dedf",
                 "sha256:0f5f5786c0e09baddcd8b4b45f20a7b5d61a7e7e99846e3c799b05c7c53fa696",
                 "sha256:129def1b7c1bf22faffd67b8f3724645203b79d8f4cc81f674654d9902cb4393",
                 "sha256:294db365efa064d00b8d1ef65d8ea2c3426ac366c0c4368d930bf1c5fb497f77",
                 "sha256:3b2b1824fe7112845700f815ff6a489360226a5609b96ec2190a45e62a9fc922",
@@ -845,14 +914,30 @@
             "hashes": [
                 "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
                 "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
             ],
             "index": "pypi",
             "version": "==2.28.2"
         },
+        "rfc3339-validator": {
+            "hashes": [
+                "sha256:138a2abdf93304ad60530167e51d2dfb9549521a836871b88d7f4695d0022f6b",
+                "sha256:24f6ec1eda14ef823da9e36ec7113124b39c04d50a4d3d3a3c2859577e7791fa"
+            ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
+            "version": "==0.1.4"
+        },
+        "rfc3986-validator": {
+            "hashes": [
+                "sha256:2f235c432ef459970b4306369336b9d5dbdda31b510ca1e327636e01f528bfa9",
+                "sha256:3d44bde7921b3b9ec3ae4e3adca370438eccebc676456449b145d533b240d055"
+            ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
+            "version": "==0.1.1"
+        },
         "s3transfer": {
             "hashes": [
                 "sha256:06176b74f3a15f61f1b4f25a1fc29a4429040b7647133a463da8fa5bd28d5ecd",
                 "sha256:2ed07d3866f523cc561bf4a00fc5535827981b117dd7876f036b0c1aca42c947"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.6.0"
@@ -860,22 +945,14 @@
         "send2trash": {
             "hashes": [
                 "sha256:d2c24762fd3759860a0aff155e45871447ea58d2be6bdd39b5c8f966a0c99c2d",
                 "sha256:f20eaadfdb517eaca5ce077640cb261c7d2698385a6a0f072a4a5447fd49fa08"
             ],
             "version": "==1.8.0"
         },
-        "setuptools": {
-            "hashes": [
-                "sha256:883131c5b6efa70b9101c7ef30b2b7b780a4283d5fc1616383cdf22c83cbefe6",
-                "sha256:9d790961ba6219e9ff7d9557622d2fe136816a264dd01d5997cfc057d804853d"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==67.0.0"
-        },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
@@ -886,19 +963,26 @@
                 "sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.3.0"
         },
         "soupsieve": {
             "hashes": [
-                "sha256:3b2503d3c7084a42b1ebd08116e5f81aadfaea95863628c80a3b774a11b7c759",
-                "sha256:fc53893b3da2c33de295667a0e19f078c14bf86544af307354de5fcf12a3f30d"
+                "sha256:49e5368c2cda80ee7e84da9dbe3e110b70a4575f196efb74e51b94549d921955",
+                "sha256:e28dba9ca6c7c00173e34e4ba57448f0688bb681b7c5e8bf4971daafc093d69a"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.3.2.post1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.4"
+        },
+        "stack-data": {
+            "hashes": [
+                "sha256:32d2dd0376772d01b6cb9fc996f3c8b57a357089dec328ed4b6553d037eaf815",
+                "sha256:cbb2a53eb64e5785878201a97ed7c7b94883f48b87bfb0bbe8b623c74679e4a8"
+            ],
+            "version": "==0.6.2"
         },
         "terminado": {
             "hashes": [
                 "sha256:6ccbbcd3a4f8a25a5ec04991f39a0b8db52dfcd487ea0e578d977e6752380333",
                 "sha256:8650d44334eba354dd591129ca3124a6ba42c3d5b70df5051b6921d506fdaeae"
             ],
             "markers": "python_version >= '3.7'",
@@ -933,21 +1017,20 @@
             "hashes": [
                 "sha256:9e6ec080259b9a5940c797d58b613b5e31441c2257b87c2e795c5228ae80d2d8",
                 "sha256:f6cde21a9c68cf756af02035f72d5a723bf607e862e7be33ece505abf4a3bad9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==5.9.0"
         },
-        "typing-extensions": {
+        "uri-template": {
             "hashes": [
-                "sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa",
-                "sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e"
+                "sha256:934e4d09d108b70eb8a24410af8615294d09d279ce0e7cbcdaef1bd21f932b06",
+                "sha256:f1699c77b73b925cf4937eae31ab282a86dc885c333f2e942513f08f691fc7db"
             ],
-            "markers": "python_version < '3.8'",
-            "version": "==4.4.0"
+            "version": "==1.2.0"
         },
         "urllib3": {
             "hashes": [
                 "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
                 "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
@@ -956,36 +1039,43 @@
         "wcwidth": {
             "hashes": [
                 "sha256:795b138f6875577cd91bba52baf9e445cd5118fd32723b460e30a0af30ea230e",
                 "sha256:a5220780a404dbe3353789870978e472cfe477761f06ee55077256e509b156d0"
             ],
             "version": "==0.2.6"
         },
+        "webcolors": {
+            "hashes": [
+                "sha256:16d043d3a08fd6a1b1b7e3e9e62640d09790dce80d2bdd4792a175b35fe794a9",
+                "sha256:d98743d81d498a2d3eaf165196e65481f0d2ea85281463d856b1e51b09f62dce"
+            ],
+            "version": "==1.12"
+        },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
         },
         "websocket-client": {
             "hashes": [
-                "sha256:561ca949e5bbb5d33409a37235db55c279235c78ee407802f1d2314fff8a8536",
-                "sha256:fb5d81b95d350f3a54838ebcb4c68a5353bbd1412ae8f068b1e5280faeb13074"
+                "sha256:3f09e6d8230892547132177f575a4e3e73cfdf06526e20cc02aa1c3b47184d40",
+                "sha256:cdf5877568b7e83aa7cf2244ab56a3213de587bbe0ce9d8b9600fc77b455d89e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.5.0"
+            "version": "==1.5.1"
         },
         "zipp": {
             "hashes": [
-                "sha256:73efd63936398aac78fd92b6f4865190119d6c91b531532e798977ea8dd402eb",
-                "sha256:9eb0a4c5feab9b08871db0d672745b53450d7f26992fd1e4653aa43345e97b86"
+                "sha256:188834565033387710d046e3fe96acfc9b5e86cbca7f39ff69cf21a4128198b7",
+                "sha256:9e5421e176ef5ab4c0ad896624e87a7b2f07aca746c9b2aa305952800cb8eecb"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.12.0"
+            "version": "==3.14.0"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
                 "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
                 "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
@@ -1132,19 +1222,19 @@
                 "sha256:bcb67d800a4497e1b404c2dd44fca47d3b7a5e5433dbab67f96c1a685cdfdf23"
             ],
             "markers": "python_version < '3.11'",
             "version": "==1.1.0"
         },
         "flake8": {
             "hashes": [
-                "sha256:6fbe320aad8d6b95cec8b8e47bc933004678dc63095be98528b7bdd2a9f510db",
-                "sha256:7a1cf6b73744f5806ab95e526f6f0d8c01c66d7bbe349562d22dfca20610b248"
+                "sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7",
+                "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"
             ],
             "index": "pypi",
-            "version": "==5.0.4"
+            "version": "==6.0.0"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
@@ -1156,19 +1246,19 @@
                 "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:057e92c15bc8d9e8109738a48db0ccb31b4d9d5cfbee5a8670879a30be66304b",
-                "sha256:b7e52a1f8dec14a75ea73e0891f3060099ca1d8e6a462a4dff11c3e119ea1b31"
+                "sha256:7efb448ec9a5e313a57655d35aa54cd3e01b7e1fbcf72dce1bf06119420f5bad",
+                "sha256:e354bedeb60efa6affdcc8ae121b73544a7aa74156d047311948f6d711cd378d"
             ],
-            "index": "pypi",
-            "version": "==4.2.0"
+            "markers": "python_version < '3.10'",
+            "version": "==6.0.0"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
@@ -1188,27 +1278,27 @@
                 "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.2"
         },
         "keyring": {
             "hashes": [
-                "sha256:69732a15cb1433bdfbc3b980a8a36a04878a6cfd7cb99f497b573f31618001c0",
-                "sha256:69b01dd83c42f590250fe7a1f503fc229b14de83857314b1933a3ddbf595c4a5"
+                "sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd",
+                "sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.9.3"
+            "version": "==23.13.1"
         },
         "markdown-it-py": {
             "hashes": [
-                "sha256:93de681e5c021a432c63147656fe21790bc01231e0cd2da73626f1aa3ac0fe27",
-                "sha256:cf7e59fed14b5ae17c0006eff14a2d9a00ed5f3a846148153899a0224e2c07da"
+                "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30",
+                "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.1.0"
+            "version": "==2.2.0"
         },
         "markupsafe": {
             "hashes": [
                 "sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed",
                 "sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc",
                 "sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2",
                 "sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460",
@@ -1308,27 +1398,27 @@
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.0.0"
         },
         "pycodestyle": {
             "hashes": [
-                "sha256:2c9607871d58c76354b697b42f5d57e1ada7d261c261efac224b664affdc5785",
-                "sha256:d1735fc58b418fd7c5f658d28d943854f8a849b01a5d0a1e6f3f3fdd0166804b"
+                "sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053",
+                "sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2.9.1"
+            "version": "==2.10.0"
         },
         "pyflakes": {
             "hashes": [
-                "sha256:4579f67d887f804e67edb544428f264b7b24f435b263c4614f384135cea553d2",
-                "sha256:491feb020dca48ccc562a8c0cbe8df07ee13078df59813b83959cbdada312ea3"
+                "sha256:ec55bf7fe21fff7f1ad2f7da62363d749e2a470500eab1b555334b67aa1ef8cf",
+                "sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2.5.0"
+            "version": "==3.0.1"
         },
         "pygments": {
             "hashes": [
                 "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
                 "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
             ],
             "markers": "python_version >= '3.6'",
@@ -1422,19 +1512,19 @@
                 "sha256:8aa57747f3fc3e977684f0176a88e789be314a99f99b43b75d1e9cb5dc6db9e9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==13.3.1"
         },
         "setuptools": {
             "hashes": [
-                "sha256:883131c5b6efa70b9101c7ef30b2b7b780a4283d5fc1616383cdf22c83cbefe6",
-                "sha256:9d790961ba6219e9ff7d9557622d2fe136816a264dd01d5997cfc057d804853d"
+                "sha256:e5fd0a713141a4a105412233c63dc4e17ba0090c8e8334594ac790ec97792330",
+                "sha256:f106dee1b506dee5102cc3f3e9e68137bbad6d47b616be7991714b0c62204251"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==67.0.0"
+            "version": "==67.4.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -1453,35 +1543,35 @@
                 "sha256:6a11ea5dd0bdb197f9c2abc2e0ce73e01340464feaece525e64036546d24c851"
             ],
             "index": "pypi",
             "version": "==4.3.2"
         },
         "sphinxcontrib-applehelp": {
             "hashes": [
-                "sha256:806111e5e962be97c29ec4c1e7fe277bfd19e9652fb1a4392105b43e01af885a",
-                "sha256:a072735ec80e7675e3f432fcae8610ecf509c5f1869d17e2eecff44389cdbc58"
+                "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228",
+                "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"
             ],
-            "markers": "python_version >= '3.5'",
-            "version": "==1.0.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.0.4"
         },
         "sphinxcontrib-devhelp": {
             "hashes": [
                 "sha256:8165223f9a335cc1af7ffe1ed31d2871f325254c0423bc0c4c7cd1c1e4734a2e",
                 "sha256:ff7f1afa7b9642e7060379360a67e9c41e8f3121f2ce9164266f61b9f4b338e4"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.2"
         },
         "sphinxcontrib-htmlhelp": {
             "hashes": [
-                "sha256:d412243dfb797ae3ec2b59eca0e52dac12e75a241bf0e4eb861e450d06c6ed07",
-                "sha256:f5f8bb2d0d629f398bf47d0d69c07bc13b65f75a81ad9e2f71a63d4b7a2f6db2"
+                "sha256:0cbdd302815330058422b98a113195c9249825d681e18f11e8b1f78a2f11efff",
+                "sha256:c38cb46dccf316c79de6e5515e1770414b797162b23cd3d06e67020e1d2a6903"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.0.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.0.1"
         },
         "sphinxcontrib-jsmath": {
             "hashes": [
                 "sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178",
                 "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"
             ],
             "markers": "python_version >= '3.5'",
@@ -1515,22 +1605,14 @@
             "hashes": [
                 "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
                 "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
             "version": "==4.0.2"
         },
-        "typing-extensions": {
-            "hashes": [
-                "sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa",
-                "sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e"
-            ],
-            "markers": "python_version < '3.8'",
-            "version": "==4.4.0"
-        },
         "urllib3": {
             "hashes": [
                 "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
                 "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==1.26.14"
@@ -1548,15 +1630,15 @@
                 "sha256:b60533f3f5d530e971d6737ca6d58681ee434818fab630c83a734bb10c083ce8"
             ],
             "index": "pypi",
             "version": "==0.38.4"
         },
         "zipp": {
             "hashes": [
-                "sha256:73efd63936398aac78fd92b6f4865190119d6c91b531532e798977ea8dd402eb",
-                "sha256:9eb0a4c5feab9b08871db0d672745b53450d7f26992fd1e4653aa43345e97b86"
+                "sha256:188834565033387710d046e3fe96acfc9b5e86cbca7f39ff69cf21a4128198b7",
+                "sha256:9e5421e176ef5ab4c0ad896624e87a7b2f07aca746c9b2aa305952800cb8eecb"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.12.0"
+            "version": "==3.14.0"
         }
     }
 }
```

### Comparing `nuclio-jupyter-0.9.8/README.md` & `nuclio-jupyter-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/nuclio/__init__.py` & `nuclio-jupyter-0.9.9/nuclio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .request import Context, Event, inject_context as _inject_context  # noqa
 from . import magic  # noqa
 from .deploy import deploy_code, deploy_file, delete_func, deploy_model  # noqa
 from .config import Volume, ConfigSpec  # noqa
 from .build import build_file  # noqa
 from .triggers import HttpTrigger, CronTrigger, KafkaTrigger  # noqa
 
-__version__ = '0.9.8'
+__version__ = '0.9.9'
 
 _inject_context()
 del _inject_context
 
 
 # Allow %load_ext nuclio
 def load_ipython_extension(ipython):
```

### Comparing `nuclio-jupyter-0.9.8/nuclio/__main__.py` & `nuclio-jupyter-0.9.9/nuclio/__main__.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/nuclio/archive.py` & `nuclio-jupyter-0.9.9/nuclio/archive.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/nuclio/auth.py` & `nuclio-jupyter-0.9.9/nuclio/auth.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/nuclio/build.py` & `nuclio-jupyter-0.9.9/nuclio/build.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/nuclio/config.py` & `nuclio-jupyter-0.9.9/nuclio/config.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/nuclio/deploy.py` & `nuclio-jupyter-0.9.9/nuclio/deploy.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/nuclio/export.py` & `nuclio-jupyter-0.9.9/nuclio/export.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/nuclio/magic.py` & `nuclio-jupyter-0.9.9/nuclio/magic.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/nuclio/request.py` & `nuclio-jupyter-0.9.9/nuclio/request.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/nuclio/triggers.py` & `nuclio-jupyter-0.9.9/nuclio/triggers.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/nuclio/utils.py` & `nuclio-jupyter-0.9.9/nuclio/utils.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/nuclio_jupyter.egg-info/PKG-INFO` & `nuclio-jupyter-0.9.9/nuclio_jupyter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclio-jupyter
-Version: 0.9.8
+Version: 0.9.9
 Summary: Convert Jupyter notebook to nuclio
 Home-page: https://github.com/nuclio/nuclio-jupyter
 Author: Miki Tebeka
 Author-email: miki@353solutions.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `nuclio-jupyter-0.9.8/nuclio_jupyter.egg-info/SOURCES.txt` & `nuclio-jupyter-0.9.9/nuclio_jupyter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/setup.py` & `nuclio-jupyter-0.9.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,19 @@
                     yield '{}{}'.format(pkg, version.replace('"', ''))
 
 
 with open('README.md') as fp:
     long_desc = fp.read()
 
 install_requires = list(load_deps('packages'))
+ipython_requirements = [
+    'ipython~=7.0; python_version<"3.8"',
+    'ipython~=8.0; python_version>="3.8"',
+]
+install_requires += ipython_requirements
 tests_require = list(load_deps('dev-packages'))
 
 
 setup(
     name='nuclio-jupyter',
     version=version(),
     description='Convert Jupyter notebook to nuclio',
```

### Comparing `nuclio-jupyter-0.9.8/tests/annotations_test_cases.yml` & `nuclio-jupyter-0.9.9/tests/annotations_test_cases.yml`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/tests/cell_and_line_magic_test_cases.yml` & `nuclio-jupyter-0.9.9/tests/cell_and_line_magic_test_cases.yml`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/tests/code_generation_test_cases.yml` & `nuclio-jupyter-0.9.9/tests/code_generation_test_cases.yml`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/tests/conftest.py` & `nuclio-jupyter-0.9.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/tests/convert_cases.yml` & `nuclio-jupyter-0.9.9/tests/convert_cases.yml`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/tests/deploy.json` & `nuclio-jupyter-0.9.9/tests/deploy.json`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/tests/handler.ipynb` & `nuclio-jupyter-0.9.9/tests/handler.ipynb`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/tests/handler.py` & `nuclio-jupyter-0.9.9/tests/handler.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/tests/tags-test.ipynb` & `nuclio-jupyter-0.9.9/tests/tags-test.ipynb`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/tests/test_build.py` & `nuclio-jupyter-0.9.9/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/tests/test_config.py` & `nuclio-jupyter-0.9.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/tests/test_deploy.py` & `nuclio-jupyter-0.9.9/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/tests/test_export.py` & `nuclio-jupyter-0.9.9/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/tests/test_install.py` & `nuclio-jupyter-0.9.9/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/tests/test_magic.py` & `nuclio-jupyter-0.9.9/tests/test_magic.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/tests/test_request.py` & `nuclio-jupyter-0.9.9/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/tests/test_triggers.py` & `nuclio-jupyter-0.9.9/tests/test_triggers.py`

 * *Files identical despite different names*

### Comparing `nuclio-jupyter-0.9.8/tests/test_utils.py` & `nuclio-jupyter-0.9.9/tests/test_utils.py`

 * *Files identical despite different names*

