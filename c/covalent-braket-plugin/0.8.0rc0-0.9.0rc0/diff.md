# Comparing `tmp/covalent-braket-plugin-0.8.0rc0.tar.gz` & `tmp/covalent-braket-plugin-0.9.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covalent-braket-plugin-0.8.0rc0.tar", last modified: Tue Oct 25 19:45:01 2022, max compression
+gzip compressed data, was "covalent-braket-plugin-0.9.0rc0.tar", last modified: Thu Oct 27 12:58:34 2022, max compression
```

## Comparing `covalent-braket-plugin-0.8.0rc0.tar` & `covalent-braket-plugin-0.9.0rc0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 19:45:01.113726 covalent-braket-plugin-0.8.0rc0/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-10-25 19:44:49.000000 covalent-braket-plugin-0.8.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-25 19:44:49.000000 covalent-braket-plugin-0.8.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6960 2022-10-25 19:45:01.113726 covalent-braket-plugin-0.8.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4623 2022-10-25 19:44:49.000000 covalent-braket-plugin-0.8.0rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-25 19:44:49.000000 covalent-braket-plugin-0.8.0rc0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 19:45:01.109726 covalent-braket-plugin-0.8.0rc0/covalent_braket_plugin/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-25 19:44:49.000000 covalent-braket-plugin-0.8.0rc0/covalent_braket_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12913 2022-10-25 19:44:49.000000 covalent-braket-plugin-0.8.0rc0/covalent_braket_plugin/braket.py
--rw-r--r--   0 runner    (1001) docker     (121)      930 2022-10-25 19:44:49.000000 covalent-braket-plugin-0.8.0rc0/covalent_braket_plugin/exec.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 19:45:01.113726 covalent-braket-plugin-0.8.0rc0/covalent_braket_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6960 2022-10-25 19:45:00.000000 covalent-braket-plugin-0.8.0rc0/covalent_braket_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-10-25 19:45:01.000000 covalent-braket-plugin-0.8.0rc0/covalent_braket_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 19:45:00.000000 covalent-braket-plugin-0.8.0rc0/covalent_braket_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-10-25 19:45:00.000000 covalent-braket-plugin-0.8.0rc0/covalent_braket_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-10-25 19:45:00.000000 covalent-braket-plugin-0.8.0rc0/covalent_braket_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-25 19:45:00.000000 covalent-braket-plugin-0.8.0rc0/covalent_braket_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-10-25 19:44:49.000000 covalent-braket-plugin-0.8.0rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-10-25 19:44:49.000000 covalent-braket-plugin-0.8.0rc0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-25 19:45:01.113726 covalent-braket-plugin-0.8.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3051 2022-10-25 19:44:49.000000 covalent-braket-plugin-0.8.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 19:45:01.113726 covalent-braket-plugin-0.8.0rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-25 19:44:49.000000 covalent-braket-plugin-0.8.0rc0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 19:45:01.113726 covalent-braket-plugin-0.8.0rc0/tests/covalent_braket_plugin_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-25 19:44:49.000000 covalent-braket-plugin-0.8.0rc0/tests/covalent_braket_plugin_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7603 2022-10-25 19:44:49.000000 covalent-braket-plugin-0.8.0rc0/tests/covalent_braket_plugin_tests/braket_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1706 2022-10-25 19:44:49.000000 covalent-braket-plugin-0.8.0rc0/tests/covalent_braket_plugin_tests/exec_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2022-10-25 19:44:49.000000 covalent-braket-plugin-0.8.0rc0/tests/functional_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 12:58:34.635651 covalent-braket-plugin-0.9.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-10-27 12:58:21.000000 covalent-braket-plugin-0.9.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-27 12:58:21.000000 covalent-braket-plugin-0.9.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7181 2022-10-27 12:58:34.635651 covalent-braket-plugin-0.9.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4844 2022-10-27 12:58:21.000000 covalent-braket-plugin-0.9.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-27 12:58:21.000000 covalent-braket-plugin-0.9.0rc0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 12:58:34.631651 covalent-braket-plugin-0.9.0rc0/covalent_braket_plugin/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 12:58:21.000000 covalent-braket-plugin-0.9.0rc0/covalent_braket_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12913 2022-10-27 12:58:21.000000 covalent-braket-plugin-0.9.0rc0/covalent_braket_plugin/braket.py
+-rw-r--r--   0 runner    (1001) docker     (121)      930 2022-10-27 12:58:21.000000 covalent-braket-plugin-0.9.0rc0/covalent_braket_plugin/exec.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 12:58:34.635651 covalent-braket-plugin-0.9.0rc0/covalent_braket_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7181 2022-10-27 12:58:34.000000 covalent-braket-plugin-0.9.0rc0/covalent_braket_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      643 2022-10-27 12:58:34.000000 covalent-braket-plugin-0.9.0rc0/covalent_braket_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 12:58:34.000000 covalent-braket-plugin-0.9.0rc0/covalent_braket_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-10-27 12:58:34.000000 covalent-braket-plugin-0.9.0rc0/covalent_braket_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-10-27 12:58:34.000000 covalent-braket-plugin-0.9.0rc0/covalent_braket_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-27 12:58:34.000000 covalent-braket-plugin-0.9.0rc0/covalent_braket_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-10-27 12:58:21.000000 covalent-braket-plugin-0.9.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-10-27 12:58:21.000000 covalent-braket-plugin-0.9.0rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-27 12:58:34.635651 covalent-braket-plugin-0.9.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3051 2022-10-27 12:58:21.000000 covalent-braket-plugin-0.9.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 12:58:34.635651 covalent-braket-plugin-0.9.0rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 12:58:21.000000 covalent-braket-plugin-0.9.0rc0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 12:58:34.635651 covalent-braket-plugin-0.9.0rc0/tests/covalent_braket_plugin_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 12:58:21.000000 covalent-braket-plugin-0.9.0rc0/tests/covalent_braket_plugin_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7603 2022-10-27 12:58:21.000000 covalent-braket-plugin-0.9.0rc0/tests/covalent_braket_plugin_tests/braket_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1706 2022-10-27 12:58:21.000000 covalent-braket-plugin-0.9.0rc0/tests/covalent_braket_plugin_tests/exec_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1460 2022-10-27 12:58:21.000000 covalent-braket-plugin-0.9.0rc0/tests/functional_test.py
```

### Comparing `covalent-braket-plugin-0.8.0rc0/LICENSE` & `covalent-braket-plugin-0.9.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `covalent-braket-plugin-0.8.0rc0/PKG-INFO` & `covalent-braket-plugin-0.9.0rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: covalent-braket-plugin
-Version: 0.8.0rc0
+Version: 0.9.0rc0
 Summary: Covalent Braket Plugin
 Home-page: https://github.com/AgnostiqHQ/covalent-braket-plugin
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: GNU Affero GPL v3.0
-Download-URL: https://github.com/AgnostiqHQ/covalent-braket-plugin/archive/v0.8.0.tar.gz
+Download-URL: https://github.com/AgnostiqHQ/covalent-braket-plugin/archive/v0.9.0.tar.gz
 Description: &nbsp;
         
         <div align="center">
         
         <img src="https://raw.githubusercontent.com/AgnostiqHQ/covalent-braket-plugin/main/assets/aws_braket_readme_banner.jpg" width=150%>
         
         [![covalent](https://img.shields.io/badge/covalent-0.177.0-purple)](https://github.com/AgnostiqHQ/covalent)
@@ -41,22 +41,22 @@
         from covalent_braket_plugin.braket import BraketExecutor
         import os
         
         # AWS resources to pass to the executor
         credentials_file = "~/.aws/credentials"
         profile = "default"
         s3_bucket_name = "braket_s3_bucket"
-        ecr_repo_name = "braket_ecr_repo"
+        ecr_image_uri = "111223344.dkr.ecr.us-east-1.amazonaws.com/amazon-braket-ecr-repo:latest"
         iam_role_name = "covalent-braket-iam-role"
         
         ex = BraketExecutor(
-            credentials=credentials_file,
             profile=profile,
+            credentials=credentials_file,
             s3_bucket_name=s3_bucket_name,
-            ecr_repo_name=ecr_repo_name,
+            ecr_image_uri=ecr_image_uri,
             braket_job_execution_role_name=iam_role_name,
             quantum_device="arn:aws:braket:::device/quantum-simulator/amazon/sv1",
             classical_device="ml.m5.large",
             storage=30,
             time_limit=300,
         )
         
@@ -109,15 +109,15 @@
         
         See the
         [RTD](https://covalent.readthedocs.io/en/latest/api/executors/awsbraket.html)
         for how to configure this executor.
         
         ## Required Cloud Resources
         
-        In order to run your workflows with covalent there are a few notable resources that need to be provisioned first.
+        In order to run your workflows with covalent there are a few notable resources that need to be provisioned first. Particularly an S3 bucket must be created, an IAM role with the `AmazonBraketFullAccess` policy, and a private ECR repo with an uploaded image for the tasks to use.
         
         For more information regarding which cloud resources need to be provisioned visit our read the docs [RTD](https://covalent.readthedocs.io/en/latest/api/executors/awsbraket.html) guide for this plugin.
         
         ## Release Notes
         
         Release notes are available in the [Changelog](https://github.com/AgnostiqHQ/covalent-braket-plugin/blob/main/CHANGELOG.md).
```

### Comparing `covalent-braket-plugin-0.8.0rc0/README.md` & `covalent-braket-plugin-0.9.0rc0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -31,22 +31,22 @@
 from covalent_braket_plugin.braket import BraketExecutor
 import os
 
 # AWS resources to pass to the executor
 credentials_file = "~/.aws/credentials"
 profile = "default"
 s3_bucket_name = "braket_s3_bucket"
-ecr_repo_name = "braket_ecr_repo"
+ecr_image_uri = "111223344.dkr.ecr.us-east-1.amazonaws.com/amazon-braket-ecr-repo:latest"
 iam_role_name = "covalent-braket-iam-role"
 
 ex = BraketExecutor(
-    credentials=credentials_file,
     profile=profile,
+    credentials=credentials_file,
     s3_bucket_name=s3_bucket_name,
-    ecr_repo_name=ecr_repo_name,
+    ecr_image_uri=ecr_image_uri,
     braket_job_execution_role_name=iam_role_name,
     quantum_device="arn:aws:braket:::device/quantum-simulator/amazon/sv1",
     classical_device="ml.m5.large",
     storage=30,
     time_limit=300,
 )
 
@@ -99,15 +99,15 @@
 
 See the
 [RTD](https://covalent.readthedocs.io/en/latest/api/executors/awsbraket.html)
 for how to configure this executor.
 
 ## Required Cloud Resources
 
-In order to run your workflows with covalent there are a few notable resources that need to be provisioned first.
+In order to run your workflows with covalent there are a few notable resources that need to be provisioned first. Particularly an S3 bucket must be created, an IAM role with the `AmazonBraketFullAccess` policy, and a private ECR repo with an uploaded image for the tasks to use.
 
 For more information regarding which cloud resources need to be provisioned visit our read the docs [RTD](https://covalent.readthedocs.io/en/latest/api/executors/awsbraket.html) guide for this plugin.
 
 ## Release Notes
 
 Release notes are available in the [Changelog](https://github.com/AgnostiqHQ/covalent-braket-plugin/blob/main/CHANGELOG.md).
```

### Comparing `covalent-braket-plugin-0.8.0rc0/covalent_braket_plugin/braket.py` & `covalent-braket-plugin-0.9.0rc0/covalent_braket_plugin/braket.py`

 * *Files identical despite different names*

### Comparing `covalent-braket-plugin-0.8.0rc0/covalent_braket_plugin/exec.py` & `covalent-braket-plugin-0.9.0rc0/covalent_braket_plugin/exec.py`

 * *Files identical despite different names*

### Comparing `covalent-braket-plugin-0.8.0rc0/covalent_braket_plugin.egg-info/PKG-INFO` & `covalent-braket-plugin-0.9.0rc0/covalent_braket_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: covalent-braket-plugin
-Version: 0.8.0rc0
+Version: 0.9.0rc0
 Summary: Covalent Braket Plugin
 Home-page: https://github.com/AgnostiqHQ/covalent-braket-plugin
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: GNU Affero GPL v3.0
-Download-URL: https://github.com/AgnostiqHQ/covalent-braket-plugin/archive/v0.8.0.tar.gz
+Download-URL: https://github.com/AgnostiqHQ/covalent-braket-plugin/archive/v0.9.0.tar.gz
 Description: &nbsp;
         
         <div align="center">
         
         <img src="https://raw.githubusercontent.com/AgnostiqHQ/covalent-braket-plugin/main/assets/aws_braket_readme_banner.jpg" width=150%>
         
         [![covalent](https://img.shields.io/badge/covalent-0.177.0-purple)](https://github.com/AgnostiqHQ/covalent)
@@ -41,22 +41,22 @@
         from covalent_braket_plugin.braket import BraketExecutor
         import os
         
         # AWS resources to pass to the executor
         credentials_file = "~/.aws/credentials"
         profile = "default"
         s3_bucket_name = "braket_s3_bucket"
-        ecr_repo_name = "braket_ecr_repo"
+        ecr_image_uri = "111223344.dkr.ecr.us-east-1.amazonaws.com/amazon-braket-ecr-repo:latest"
         iam_role_name = "covalent-braket-iam-role"
         
         ex = BraketExecutor(
-            credentials=credentials_file,
             profile=profile,
+            credentials=credentials_file,
             s3_bucket_name=s3_bucket_name,
-            ecr_repo_name=ecr_repo_name,
+            ecr_image_uri=ecr_image_uri,
             braket_job_execution_role_name=iam_role_name,
             quantum_device="arn:aws:braket:::device/quantum-simulator/amazon/sv1",
             classical_device="ml.m5.large",
             storage=30,
             time_limit=300,
         )
         
@@ -109,15 +109,15 @@
         
         See the
         [RTD](https://covalent.readthedocs.io/en/latest/api/executors/awsbraket.html)
         for how to configure this executor.
         
         ## Required Cloud Resources
         
-        In order to run your workflows with covalent there are a few notable resources that need to be provisioned first.
+        In order to run your workflows with covalent there are a few notable resources that need to be provisioned first. Particularly an S3 bucket must be created, an IAM role with the `AmazonBraketFullAccess` policy, and a private ECR repo with an uploaded image for the tasks to use.
         
         For more information regarding which cloud resources need to be provisioned visit our read the docs [RTD](https://covalent.readthedocs.io/en/latest/api/executors/awsbraket.html) guide for this plugin.
         
         ## Release Notes
         
         Release notes are available in the [Changelog](https://github.com/AgnostiqHQ/covalent-braket-plugin/blob/main/CHANGELOG.md).
```

### Comparing `covalent-braket-plugin-0.8.0rc0/covalent_braket_plugin.egg-info/SOURCES.txt` & `covalent-braket-plugin-0.9.0rc0/covalent_braket_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `covalent-braket-plugin-0.8.0rc0/pyproject.toml` & `covalent-braket-plugin-0.9.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `covalent-braket-plugin-0.8.0rc0/setup.py` & `covalent-braket-plugin-0.9.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `covalent-braket-plugin-0.8.0rc0/tests/covalent_braket_plugin_tests/braket_test.py` & `covalent-braket-plugin-0.9.0rc0/tests/covalent_braket_plugin_tests/braket_test.py`

 * *Files identical despite different names*

### Comparing `covalent-braket-plugin-0.8.0rc0/tests/covalent_braket_plugin_tests/exec_test.py` & `covalent-braket-plugin-0.9.0rc0/tests/covalent_braket_plugin_tests/exec_test.py`

 * *Files identical despite different names*

### Comparing `covalent-braket-plugin-0.8.0rc0/tests/functional_test.py` & `covalent-braket-plugin-0.9.0rc0/tests/functional_test.py`

 * *Files identical despite different names*

