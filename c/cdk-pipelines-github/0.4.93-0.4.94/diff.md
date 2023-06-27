# Comparing `tmp/cdk-pipelines-github-0.4.93.tar.gz` & `tmp/cdk-pipelines-github-0.4.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-pipelines-github-0.4.93.tar", last modified: Mon Jun 26 00:19:58 2023, max compression
+gzip compressed data, was "cdk-pipelines-github-0.4.94.tar", last modified: Tue Jun 27 00:22:14 2023, max compression
```

## Comparing `cdk-pipelines-github-0.4.93.tar` & `cdk-pipelines-github-0.4.94.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:19:58.471791 cdk-pipelines-github-0.4.93/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-26 00:19:43.000000 cdk-pipelines-github-0.4.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 00:19:43.000000 cdk-pipelines-github-0.4.93/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-26 00:19:43.000000 cdk-pipelines-github-0.4.93/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    24130 2023-06-26 00:19:58.471791 cdk-pipelines-github-0.4.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-06-26 00:19:43.000000 cdk-pipelines-github-0.4.93/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 00:19:43.000000 cdk-pipelines-github-0.4.93/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 00:19:58.471791 cdk-pipelines-github-0.4.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-26 00:19:43.000000 cdk-pipelines-github-0.4.93/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:19:58.467791 cdk-pipelines-github-0.4.93/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:19:58.467791 cdk-pipelines-github-0.4.93/src/cdk_pipelines_github/
--rw-r--r--   0 runner    (1001) docker     (123)   312642 2023-06-26 00:19:43.000000 cdk-pipelines-github-0.4.93/src/cdk_pipelines_github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:19:58.471791 cdk-pipelines-github-0.4.93/src/cdk_pipelines_github/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-26 00:19:43.000000 cdk-pipelines-github-0.4.93/src/cdk_pipelines_github/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   322704 2023-06-26 00:19:43.000000 cdk-pipelines-github-0.4.93/src/cdk_pipelines_github/_jsii/cdk-pipelines-github@0.4.93.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 00:19:43.000000 cdk-pipelines-github-0.4.93/src/cdk_pipelines_github/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:19:58.471791 cdk-pipelines-github-0.4.93/src/cdk_pipelines_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24130 2023-06-26 00:19:58.000000 cdk-pipelines-github-0.4.93/src/cdk_pipelines_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-26 00:19:58.000000 cdk-pipelines-github-0.4.93/src/cdk_pipelines_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 00:19:58.000000 cdk-pipelines-github-0.4.93/src/cdk_pipelines_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 00:19:58.000000 cdk-pipelines-github-0.4.93/src/cdk_pipelines_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 00:19:58.000000 cdk-pipelines-github-0.4.93/src/cdk_pipelines_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:22:14.599695 cdk-pipelines-github-0.4.94/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-27 00:21:51.000000 cdk-pipelines-github-0.4.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 00:21:51.000000 cdk-pipelines-github-0.4.94/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 00:21:51.000000 cdk-pipelines-github-0.4.94/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    24130 2023-06-27 00:22:14.599695 cdk-pipelines-github-0.4.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-06-27 00:21:51.000000 cdk-pipelines-github-0.4.94/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-27 00:21:51.000000 cdk-pipelines-github-0.4.94/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 00:22:14.599695 cdk-pipelines-github-0.4.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-27 00:21:51.000000 cdk-pipelines-github-0.4.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:22:14.595695 cdk-pipelines-github-0.4.94/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:22:14.595695 cdk-pipelines-github-0.4.94/src/cdk_pipelines_github/
+-rw-r--r--   0 runner    (1001) docker     (123)   312642 2023-06-27 00:21:51.000000 cdk-pipelines-github-0.4.94/src/cdk_pipelines_github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:22:14.599695 cdk-pipelines-github-0.4.94/src/cdk_pipelines_github/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-27 00:21:51.000000 cdk-pipelines-github-0.4.94/src/cdk_pipelines_github/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   322705 2023-06-27 00:21:51.000000 cdk-pipelines-github-0.4.94/src/cdk_pipelines_github/_jsii/cdk-pipelines-github@0.4.94.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 00:21:51.000000 cdk-pipelines-github-0.4.94/src/cdk_pipelines_github/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:22:14.599695 cdk-pipelines-github-0.4.94/src/cdk_pipelines_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24130 2023-06-27 00:22:14.000000 cdk-pipelines-github-0.4.94/src/cdk_pipelines_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-27 00:22:14.000000 cdk-pipelines-github-0.4.94/src/cdk_pipelines_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 00:22:14.000000 cdk-pipelines-github-0.4.94/src/cdk_pipelines_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-27 00:22:14.000000 cdk-pipelines-github-0.4.94/src/cdk_pipelines_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 00:22:14.000000 cdk-pipelines-github-0.4.94/src/cdk_pipelines_github.egg-info/top_level.txt
```

### Comparing `cdk-pipelines-github-0.4.93/LICENSE` & `cdk-pipelines-github-0.4.94/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-pipelines-github-0.4.93/PKG-INFO` & `cdk-pipelines-github-0.4.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-pipelines-github
-Version: 0.4.93
+Version: 0.4.94
 Summary: GitHub Workflows support for CDK Pipelines
 Home-page: https://github.com/cdklabs/cdk-pipelines-github.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-pipelines-github.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-pipelines-github-0.4.93/README.md` & `cdk-pipelines-github-0.4.94/README.md`

 * *Files identical despite different names*

### Comparing `cdk-pipelines-github-0.4.93/setup.py` & `cdk-pipelines-github-0.4.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-pipelines-github",
-    "version": "0.4.93",
+    "version": "0.4.94",
     "description": "GitHub Workflows support for CDK Pipelines",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-pipelines-github.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_pipelines_github",
         "cdk_pipelines_github._jsii"
     ],
     "package_data": {
         "cdk_pipelines_github._jsii": [
-            "cdk-pipelines-github@0.4.93.jsii.tgz"
+            "cdk-pipelines-github@0.4.94.jsii.tgz"
         ],
         "cdk_pipelines_github": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-pipelines-github-0.4.93/src/cdk_pipelines_github/__init__.py` & `cdk-pipelines-github-0.4.94/src/cdk_pipelines_github/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-pipelines-github-0.4.93/src/cdk_pipelines_github.egg-info/PKG-INFO` & `cdk-pipelines-github-0.4.94/src/cdk_pipelines_github.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-pipelines-github
-Version: 0.4.93
+Version: 0.4.94
 Summary: GitHub Workflows support for CDK Pipelines
 Home-page: https://github.com/cdklabs/cdk-pipelines-github.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-pipelines-github.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

