# Comparing `tmp/redhat_qe_cloud_tools-1.0.6.tar.gz` & `tmp/redhat_qe_cloud_tools-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redhat_qe_cloud_tools-1.0.6.tar", max compression
+gzip compressed data, was "redhat_qe_cloud_tools-1.0.7.tar", max compression
```

## Comparing `redhat_qe_cloud_tools-1.0.6.tar` & `redhat_qe_cloud_tools-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-06-11 14:32:12.058322 redhat_qe_cloud_tools-1.0.6/LICENSE
--rw-r--r--   0        0        0      852 2023-06-11 14:32:12.058322 redhat_qe_cloud_tools-1.0.6/README.md
--rw-r--r--   0        0        0        0 2023-06-11 14:32:12.058322 redhat_qe_cloud_tools-1.0.6/clouds/__init__.py
--rw-r--r--   0        0        0      787 2023-06-11 14:32:12.058322 redhat_qe_cloud_tools-1.0.6/clouds/aws/README.md
--rw-r--r--   0        0        0        0 2023-06-11 14:32:12.058322 redhat_qe_cloud_tools-1.0.6/clouds/aws/__init__.py
--rw-r--r--   0        0        0     4066 2023-06-11 14:32:12.059322 redhat_qe_cloud_tools-1.0.6/clouds/aws/aws_utils.py
--rw-r--r--   0        0        0     4317 2023-06-11 14:32:12.059322 redhat_qe_cloud_tools-1.0.6/clouds/aws/delete_s3_velero_bucket.py
--rw-r--r--   0        0        0      455 2023-06-11 14:32:12.059322 redhat_qe_cloud_tools-1.0.6/clouds/aws/roles/README.md
--rw-r--r--   0        0        0        0 2023-06-11 14:32:12.059322 redhat_qe_cloud_tools-1.0.6/clouds/aws/roles/__init__.py
--rw-r--r--   0        0        0     1193 2023-06-11 14:32:12.059322 redhat_qe_cloud_tools-1.0.6/clouds/aws/roles/roles.py
--rw-r--r--   0        0        0      554 2023-06-11 14:32:12.059322 redhat_qe_cloud_tools-1.0.6/clouds/aws/session_clients.py
--rw-r--r--   0        0        0     7789 2023-06-11 14:32:12.059322 redhat_qe_cloud_tools-1.0.6/clouds/aws/utilities/delete_aws_resources.py
--rw-r--r--   0        0        0      815 2023-06-11 14:32:12.060322 redhat_qe_cloud_tools-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 redhat_qe_cloud_tools-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/LICENSE
+-rw-r--r--   0        0        0      852 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/clouds/__init__.py
+-rw-r--r--   0        0        0      787 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/clouds/aws/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/clouds/aws/__init__.py
+-rw-r--r--   0        0        0     4478 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/clouds/aws/aws_utils.py
+-rw-r--r--   0        0        0     4317 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/clouds/aws/delete_s3_velero_bucket.py
+-rw-r--r--   0        0        0      455 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/clouds/aws/roles/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/clouds/aws/roles/__init__.py
+-rw-r--r--   0        0        0     1193 2023-06-27 10:39:32.776041 redhat_qe_cloud_tools-1.0.7/clouds/aws/roles/roles.py
+-rw-r--r--   0        0        0      554 2023-06-27 10:39:32.777041 redhat_qe_cloud_tools-1.0.7/clouds/aws/session_clients.py
+-rw-r--r--   0        0        0     7805 2023-06-27 10:39:32.777041 redhat_qe_cloud_tools-1.0.7/clouds/aws/utilities/delete_aws_resources.py
+-rw-r--r--   0        0        0      815 2023-06-27 10:39:32.777041 redhat_qe_cloud_tools-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 redhat_qe_cloud_tools-1.0.7/PKG-INFO
```

### Comparing `redhat_qe_cloud_tools-1.0.6/LICENSE` & `redhat_qe_cloud_tools-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.6/README.md` & `redhat_qe_cloud_tools-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.6/clouds/aws/README.md` & `redhat_qe_cloud_tools-1.0.7/clouds/aws/README.md`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.6/clouds/aws/aws_utils.py` & `redhat_qe_cloud_tools-1.0.7/clouds/aws/aws_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,34 @@
 import os
 from configparser import ConfigParser, NoOptionError, NoSectionError
 from http import HTTPStatus
 
 from simple_logger.logger import get_logger
 
 LOGGER = get_logger(name=__name__)
+AWS_CONFIG_FILE = os.environ.get("AWS_CONFIG_FILE", os.path.expanduser("~/.aws/config"))
+AWS_CREDENTIALS_FILE = os.environ.get(
+    "AWS_CONFIG_FILE", os.path.expanduser("~/.aws/credentials")
+)
 
 
 class AWSConfigurationError(Exception):
     pass
 
 
-def verify_existing_config_in_env_vars_or_file(vars_list, file_path, section="default"):
+def set_and_verify_existing_config_in_env_vars_or_file(
+    vars_list, file_path, section="default"
+):
     """
     Verify vars are either set as environment variables or in a config file.
 
+    When var exists as OS environment then continue.
+    When vars exists in config file, set them as OS environment.
+    If none of the above raise.
+
     Args:
         vars_list (list): A list of variable names
         file_path (str): Absolute path to config file
         section (str): Section name in config file
 
     Raises:
         AWSConfigurationError: raises on missing configuration
@@ -27,44 +37,47 @@
     missing_vars = []
     parser = ConfigParser()
     parser.read(file_path)
     aws_region_str = "region"
     for var in vars_list:
         if os.getenv(var.upper()):
             continue
+
         LOGGER.info(
             f"Variable {var} is not set as environment variables, checking in config file."
         )
         try:
-            var = var.lower()
+            var_in_file = var.lower()
             # `AWS_REGION` environment variable is set as `region` in the config file
-            if aws_region_str in var:
-                var = aws_region_str
-            parser.get(section, var)
+            if aws_region_str in var_in_file:
+                var_in_file = aws_region_str
+
+            os.environ[var.upper()] = parser.get(section, var_in_file)
         except (NoSectionError, NoOptionError):
             missing_vars.append(var)
+
     if missing_vars:
         LOGGER.error(
             f"Missing configuration: {','.join(missing_vars)}. "
             f"Values should be set in environment variables or in {file_path}"
         )
         raise AWSConfigurationError()
 
 
-def verify_aws_credentials():
-    verify_existing_config_in_env_vars_or_file(
+def set_and_verify_aws_credentials():
+    set_and_verify_existing_config_in_env_vars_or_file(
         vars_list=["AWS_ACCESS_KEY_ID", "AWS_SECRET_ACCESS_KEY"],
-        file_path=os.path.expanduser("~/.aws/credentials"),
+        file_path=AWS_CREDENTIALS_FILE,
     )
 
 
-def verify_aws_config():
-    verify_existing_config_in_env_vars_or_file(
+def set_and_verify_aws_config():
+    set_and_verify_existing_config_in_env_vars_or_file(
         vars_list=["AWS_REGION"],
-        file_path=os.path.expanduser("~/.aws/config"),
+        file_path=AWS_CONFIG_FILE,
     )
 
 
 def delete_all_objects_from_s3_folder(bucket_name: str, boto_client) -> None:
     """
     Deletes all files in a folder of an S3 bucket
```

### Comparing `redhat_qe_cloud_tools-1.0.6/clouds/aws/delete_s3_velero_bucket.py` & `redhat_qe_cloud_tools-1.0.7/clouds/aws/delete_s3_velero_bucket.py`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.6/clouds/aws/roles/roles.py` & `redhat_qe_cloud_tools-1.0.7/clouds/aws/roles/roles.py`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.6/clouds/aws/session_clients.py` & `redhat_qe_cloud_tools-1.0.7/clouds/aws/session_clients.py`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.6/clouds/aws/utilities/delete_aws_resources.py` & `redhat_qe_cloud_tools-1.0.7/clouds/aws/utilities/delete_aws_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import click
 from ocp_utilities.utils import run_command
 from simple_logger.logger import get_logger
 
 from clouds.aws.aws_utils import (
     delete_all_objects_from_s3_folder,
     delete_bucket,
-    verify_aws_credentials,
+    set_and_verify_aws_credentials,
 )
 from clouds.aws.session_clients import ec2_client, iam_client, rds_client, s3_client
 
 LOGGER = get_logger(name="delete-aws-resources", filename="delete_aws_resources.log")
 MAX_ITEMS = 1000
 
 
@@ -164,15 +164,15 @@
 
     if not shutil.which("cloud-nuke"):
         click.echo(
             "cloud-nuke is not installed; install from https://github.com/gruntwork-io/cloud-nuke"
         )
         raise click.Abort()
 
-    verify_aws_credentials()
+    set_and_verify_aws_credentials()
 
     rerun_cleanup_list = clean_aws_resources(aws_regions=_aws_regions)
     while rerun_cleanup_list:
         rerun_cleanup_list = clean_aws_resources(aws_regions=rerun_cleanup_list)
 
 
 def clean_aws_resources(aws_regions):
```

### Comparing `redhat_qe_cloud_tools-1.0.6/pyproject.toml` & `redhat_qe_cloud_tools-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [tool.isort]
 line_length = 88
 profile = "black"
 
 [tool.poetry]
 name = "redhat-qe-cloud-tools"
-version = "1.0.6"
+version = "1.0.7"
 description = "Python utilities to manage cloud services, such as AWS."
 authors = ["Meni Yakove", "Ruth Netser"]
 readme = "README.md"
 repository = "https://github.com/RedHatQE/cloud-tools"
 packages = [{include = "clouds"}]
 
 [tool.poetry.dependencies]
```

### Comparing `redhat_qe_cloud_tools-1.0.6/PKG-INFO` & `redhat_qe_cloud_tools-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redhat-qe-cloud-tools
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python utilities to manage cloud services, such as AWS.
 Home-page: https://github.com/RedHatQE/cloud-tools
 Author: Meni Yakove
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

