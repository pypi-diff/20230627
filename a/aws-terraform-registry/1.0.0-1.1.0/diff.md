# Comparing `tmp/aws_terraform_registry-1.0.0.tar.gz` & `tmp/aws_terraform_registry-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_terraform_registry-1.0.0.tar", max compression
+gzip compressed data, was "aws_terraform_registry-1.1.0.tar", max compression
```

## Comparing `aws_terraform_registry-1.0.0.tar` & `aws_terraform_registry-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1100 2023-06-23 22:26:45.910980 aws_terraform_registry-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     6885 2023-06-23 22:26:45.910980 aws_terraform_registry-1.0.0/README.md
--rw-r--r--   0        0        0      396 2023-06-23 22:26:45.914980 aws_terraform_registry-1.0.0/aws_terraform_registry/__init__.py
--rw-r--r--   0        0        0       30 2023-06-23 22:26:45.914980 aws_terraform_registry-1.0.0/aws_terraform_registry/__main__.py
--rw-r--r--   0        0        0     4570 2023-06-23 22:26:45.914980 aws_terraform_registry-1.0.0/aws_terraform_registry/cli.py
--rw-r--r--   0        0        0      376 2023-06-23 22:26:45.914980 aws_terraform_registry-1.0.0/aws_terraform_registry/common/__init__.py
--rw-r--r--   0        0        0     1434 2023-06-23 22:26:45.914980 aws_terraform_registry-1.0.0/aws_terraform_registry/common/logger.py
--rw-r--r--   0        0        0     9388 2023-06-23 22:26:45.914980 aws_terraform_registry-1.0.0/aws_terraform_registry/common/matrix.py
--rw-r--r--   0        0        0     1405 2023-06-23 22:26:45.914980 aws_terraform_registry-1.0.0/aws_terraform_registry/common/model.py
--rw-r--r--   0        0        0     1045 2023-06-23 22:26:45.914980 aws_terraform_registry-1.0.0/aws_terraform_registry/common/publish.py
--rw-r--r--   0        0        0     3179 2023-06-23 22:26:45.914980 aws_terraform_registry-1.0.0/aws_terraform_registry/common/release.py
--rw-r--r--   0        0        0     1894 2023-06-23 22:26:45.914980 aws_terraform_registry-1.0.0/aws_terraform_registry/common/token.py
--rw-r--r--   0        0        0     2494 2023-06-23 22:26:45.914980 aws_terraform_registry-1.0.0/aws_terraform_registry/config.py
--rw-r--r--   0        0        0     3464 2023-06-23 22:26:45.914980 aws_terraform_registry-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     8226 1970-01-01 00:00:00.000000 aws_terraform_registry-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-06-26 22:10:26.469411 aws_terraform_registry-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0     7674 2023-06-26 22:10:26.469411 aws_terraform_registry-1.1.0/README.md
+-rw-r--r--   0        0        0      396 2023-06-26 22:10:26.469411 aws_terraform_registry-1.1.0/aws_terraform_registry/__init__.py
+-rw-r--r--   0        0        0       30 2023-06-26 22:10:26.469411 aws_terraform_registry-1.1.0/aws_terraform_registry/__main__.py
+-rw-r--r--   0        0        0     5400 2023-06-26 22:10:26.469411 aws_terraform_registry-1.1.0/aws_terraform_registry/cli.py
+-rw-r--r--   0        0        0      418 2023-06-26 22:10:26.469411 aws_terraform_registry-1.1.0/aws_terraform_registry/common/__init__.py
+-rw-r--r--   0        0        0     1434 2023-06-26 22:10:26.469411 aws_terraform_registry-1.1.0/aws_terraform_registry/common/logger.py
+-rw-r--r--   0        0        0     9388 2023-06-26 22:10:26.469411 aws_terraform_registry-1.1.0/aws_terraform_registry/common/matrix.py
+-rw-r--r--   0        0        0     1674 2023-06-26 22:10:26.469411 aws_terraform_registry-1.1.0/aws_terraform_registry/common/model.py
+-rw-r--r--   0        0        0     2730 2023-06-26 22:10:26.469411 aws_terraform_registry-1.1.0/aws_terraform_registry/common/publish.py
+-rw-r--r--   0        0        0     3614 2023-06-26 22:10:26.469411 aws_terraform_registry-1.1.0/aws_terraform_registry/common/release.py
+-rw-r--r--   0        0        0     1894 2023-06-26 22:10:26.469411 aws_terraform_registry-1.1.0/aws_terraform_registry/common/token.py
+-rw-r--r--   0        0        0     2653 2023-06-26 22:10:26.469411 aws_terraform_registry-1.1.0/aws_terraform_registry/config.py
+-rw-r--r--   0        0        0     3464 2023-06-26 22:10:26.473410 aws_terraform_registry-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9015 1970-01-01 00:00:00.000000 aws_terraform_registry-1.1.0/PKG-INFO
```

### Comparing `aws_terraform_registry-1.0.0/LICENSE.md` & `aws_terraform_registry-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aws_terraform_registry-1.0.0/README.md` & `aws_terraform_registry-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 ## Installation
 
 Install this library directly into an activated virtual environment:
 
 ```text
-$ python3 -m pip install terraform-aws-tf-registry-cli
+$ python3 -m pip install terraform-aws-tf-registry
 ```
 
 ## Configuration
 
 We have to provide few informations to this client :
 
 
@@ -87,22 +87,23 @@
 ```bash
 > tfr
 usage: tfr [-h] {config,generate-token,generate-terraformrc,publish,release} ...
 
 Manage terraform registry
 
 positional arguments:
-  {config,generate-token,generate-terraformrc,publish,release}
+  {config,generate-token,generate-terraformrc,release,unpublish,publish}
                         commands
     config              Show configuration parameters
     generate-token      Generate an access token
     generate-terraformrc
                         Generate terraformrc configuration file
-    publish             Publish a terraform module from custom source.
     release             Release a terraform module from custom source.
+    publish             Publish a terraform module from custom source.
+    unpublish           Unpublish a terraform module (Keep archive on s3).
 
 optional arguments:
   -h, --help            show this help message and exit
   ```
 
 ### Configuration
 
@@ -171,23 +172,42 @@
 
 > `publish`: register the source module as is in the aws private terraform regstry. You could have access issue if this url is not public.
 
 > `release`: 
 >
 >    - store the source into the dedicated bucket of aws private terraform regstry. The access is managed within registry.
 >    - archive (targ.gz) if the source is a folder
->    - download the source if it's an http utl
+>    - download the source if it's an http url
+>    - As your module will be stored within registry bucket, terraform client will use s3 signed url
 
-We use `release` from our ci/cd pipeline and `publish` when we have to do something like 'quick and dirty' ... (It never happen, I swear !)
+We use `release` from our ci/cd pipeline and `publish` only when we have to do something like 'quick and dirty' ... (It never happen, I swear !)
 
+### Release command
 
-### Publish command
+```bash
+usage: tfr release [-h] [-namespace NAMESPACE] -name NAME -system SYSTEM -version VERSION -source SOURCE
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -namespace NAMESPACE, --namespace NAMESPACE
+                        module namespace
+  -name NAME, --name NAME
+                        module name
+  -system SYSTEM, --system SYSTEM
+                        module system (aws, ...)
+  -version VERSION, --version VERSION
+                        module version
+  -source SOURCE, --source SOURCE
+                        module source
+```
+
+### Unpublish command
 
 ```bash
-usage: tfr publish [-h] [-namespace NAMESPACE] -name NAME -system SYSTEM -version VERSION -source SOURCE
+usage: tfr unpublish [-h] [-namespace NAMESPACE] -name NAME -system SYSTEM -version VERSION -source SOURCE
 
 optional arguments:
   -h, --help            show this help message and exit
   -namespace NAMESPACE, --namespace NAMESPACE
                         module namespace
   -name NAME, --name NAME
                         module name
@@ -195,18 +215,19 @@
                         module system (aws, ...)
   -version VERSION, --version VERSION
                         module version
   -source SOURCE, --source SOURCE
                         module source
 ```
 
-### Release command
+
+### Publish command
 
 ```bash
-usage: tfr release [-h] [-namespace NAMESPACE] -name NAME -system SYSTEM -version VERSION -source SOURCE
+usage: tfr publish [-h] [-namespace NAMESPACE] -name NAME -system SYSTEM -version VERSION -source SOURCE
 
 optional arguments:
   -h, --help            show this help message and exit
   -namespace NAMESPACE, --namespace NAMESPACE
                         module namespace
   -name NAME, --name NAME
                         module name
@@ -215,7 +236,8 @@
   -version VERSION, --version VERSION
                         module version
   -source SOURCE, --source SOURCE
                         module source
 ```
 
 
+
```

### Comparing `aws_terraform_registry-1.0.0/aws_terraform_registry/cli.py` & `aws_terraform_registry-1.1.0/aws_terraform_registry/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .common import (
     TerraformModuleIdentifier,
     generate_terraformrc,
     generate_token,
     init_root_logger,
     publish_module,
     release_module,
+    unpublish_module,
 )
 from .config import ApplicationConfig
 
 __all__ = ["main"]
 
 
 def main():
@@ -33,15 +34,22 @@
 
 
 def build_parser(config: ApplicationConfig):
     """Build arguments parser."""
     parser = argparse.ArgumentParser(prog="tfr", description="Manage terraform registry")
     subparsers = parser.add_subparsers(help='commands')
 
-    for item in [_define_config, _define_generate, _define_terraformrc, _define_publish, _define_release]:
+    for item in [
+        _define_config,
+        _define_generate,
+        _define_terraformrc,
+        _define_release,
+        _define_publish,
+        _define_unpublish,
+    ]:
         item(subparsers, config)
 
     return parser
 
 
 # mypy: disable-error-code="attr-defined"
 def _define_config(subparsers, config: ApplicationConfig):
@@ -102,14 +110,30 @@
             ),
             version=args.version,
             source=args.source,
         )
     )
 
 
+def _define_unpublish(subparsers, config: ApplicationConfig):
+    parser = subparsers.add_parser('unpublish', help='Unpublish a terraform module (Keep archive on s3).')
+    _add_common_terraform_module_identifier_args(parser=parser)
+    parser.set_defaults(
+        func=lambda args: unpublish_module(
+            config=config,
+            terraform_module=TerraformModuleIdentifier(
+                namespace=args.namespace if args.namespace else config.default_namespace,
+                name=args.name,
+                system=args.system,
+            ),
+            version=args.version,
+        )
+    )
+
+
 def _define_release(subparsers, config: ApplicationConfig):
     parser = subparsers.add_parser('release', help='Release a terraform module from custom source.')
     _add_common_terraform_module_args(parser=parser)
     parser.set_defaults(
         func=lambda args: release_module(
             config=config,
             terraform_module=TerraformModuleIdentifier(
@@ -130,17 +154,21 @@
         action="store",
         type=int,
         help="#weeks of validity (52 per default)",
         default=52,
     )
 
 
-def _add_common_terraform_module_args(parser):
+def _add_common_terraform_module_identifier_args(parser):
     parser.add_argument(
         "-namespace", "--namespace", action="store", type=str, help="module namespace", required=False, default=None
     )
     parser.add_argument("-name", "--name", action="store", type=str, help="module name", required=True)
     parser.add_argument(
         "-system", "--system", action="store", type=str, help="module system (aws, azure, ...)", required=True
     )
     parser.add_argument("-version", "--version", action="store", type=str, help="module version", required=True)
+
+
+def _add_common_terraform_module_args(parser):
+    _add_common_terraform_module_identifier_args(parser=parser)
     parser.add_argument("-source", "--source", action="store", type=str, help="module source", required=True)
```

### Comparing `aws_terraform_registry-1.0.0/aws_terraform_registry/common/logger.py` & `aws_terraform_registry-1.1.0/aws_terraform_registry/common/logger.py`

 * *Files identical despite different names*

### Comparing `aws_terraform_registry-1.0.0/aws_terraform_registry/common/matrix.py` & `aws_terraform_registry-1.1.0/aws_terraform_registry/common/matrix.py`

 * *Files identical despite different names*

### Comparing `aws_terraform_registry-1.0.0/aws_terraform_registry/common/model.py` & `aws_terraform_registry-1.1.0/aws_terraform_registry/common/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 from dataclasses import dataclass
 
 from boto3 import client
 
-__all__ = ['TerraformModuleIdentifier']
+__all__ = ['TerraformModuleIdentifier', 'BUCKET_FILE_NAME']
+
+BUCKET_FILE_NAME = "archive.tar.gz"
 
 
 @dataclass()
 class TerraformModuleIdentifier:
     """Define a Terraform Module Identifier.
 
     Attributes:
@@ -25,24 +27,28 @@
 
     @property
     def module_id(self) -> str:
         return f"{self.namespace}/{self.name}/{self.system}".lower()
 
     def get_bucket_key(self, version: str) -> str:
         """Return bucket key."""
-        return f"{self.module_id}/{version}/archive.tar.gz"
+        return f"{self.module_id}/{version}/{BUCKET_FILE_NAME}"
 
     def get_publish_url(self, bucket_name: str, version: str) -> str:
         """Return s3 url."""
 
         region = _find_caller_region()
         bucket_sub_name = f"s3-{region}" if region != "us-east-1" else "s3"
         return "/".join(
             [f"s3::https://{bucket_name}.{bucket_sub_name}.amazonaws.com", self.get_bucket_key(version=version)]
         )
 
+    def get_blob_url(self, repository_url: str, version: str) -> str:
+        """Return registry url with blob api."""
+        return "/".join([repository_url, "blob", self.get_bucket_key(version=version)])
+
 
 def _find_caller_region() -> str:
     try:
         return client('s3').meta.region_name
     except RuntimeError:
         return os.environ.get('AWS_REGION', "eu-west-1")
```

### Comparing `aws_terraform_registry-1.0.0/aws_terraform_registry/common/publish.py` & `aws_terraform_registry-1.1.0/aws_terraform_registry/common/publish.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from boto3 import client
 
 from ..config import ApplicationConfig
 from .model import TerraformModuleIdentifier
 
 logger = getLogger()
 
-__all__ = ["publish_module"]
+__all__ = ["publish_module", "exists"]
 
 # mypy: disable-error-code="arg-type"
 def publish_module(
     config: ApplicationConfig, terraform_module: TerraformModuleIdentifier, version: str, source: str
 ) -> str:
     """Publish terraform module.
 
@@ -20,19 +20,67 @@
         config (ApplicationConfig): application configuration
         terraform_module (TerraformModuleIdentifier): module identifier
         version (str): version to publish
         source (str): module source
 
     Returns:
         str: source
+
+    Raises:
+        (RuntimeError): if specified version and module is ever published.
     """
     config.validate()
+
+    if exists(config=config, terraform_module=terraform_module, version=version):
+        msg = f"Version {version} for module {terraform_module.module_id} ever exist"
+        logger.error(msg)
+        raise RuntimeError(msg)
+
     client('dynamodb').put_item(
         TableName=config.dynamodb_table_name,
         Item={
             "Id": {"S": terraform_module.module_id},
             "Version": {"S": version},
             "Source": {"S": source},
         },
     )
     logger.info(f"Published module {terraform_module.module_id}, Version {version}, Source {source}")
     return source
+
+
+# mypy: disable-error-code="arg-type"
+def unpublish_module(config: ApplicationConfig, terraform_module: TerraformModuleIdentifier, version: str):
+    """UnPublish terraform module.
+
+    Args:
+
+        config (ApplicationConfig): application configuration
+        terraform_module (TerraformModuleIdentifier): module identifier
+        version (str): version to publish
+
+
+    Raises:
+        (RuntimeError): if specified version and module did not exists.
+    """
+    config.validate()
+
+    if not exists(config=config, terraform_module=terraform_module, version=version):
+        msg = f"Version {version} for module {terraform_module.module_id} did not exist"
+        logger.error(msg)
+        raise RuntimeError(msg)
+
+    client('dynamodb').delete_item(
+        TableName=config.dynamodb_table_name,
+        Key={
+            "Id": {"S": terraform_module.module_id},
+            "Version": {"S": version},
+        },
+    )
+    logger.info(f"Unpublished module {terraform_module.module_id}, Version {version}")
+
+
+def exists(config: ApplicationConfig, terraform_module: TerraformModuleIdentifier, version: str) -> bool:
+    dynamodb_client = client("dynamodb")
+    response = dynamodb_client.get_item(
+        TableName=config.dynamodb_table_name, Key={'Id': {'S': terraform_module.module_id}, 'Version': {'S': version}}
+    )
+    return 'Item' in response
```

### Comparing `aws_terraform_registry-1.0.0/aws_terraform_registry/common/release.py` & `aws_terraform_registry-1.1.0/aws_terraform_registry/common/release.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import urllib.request
 from logging import getLogger
 from pathlib import Path
 
 from boto3 import client
 
 from ..config import ApplicationConfig
-from .model import TerraformModuleIdentifier
-from .publish import publish_module
+from .model import BUCKET_FILE_NAME, TerraformModuleIdentifier
+from .publish import exists, publish_module
 
 logger = getLogger()
 
 
 __all__ = ['release_module', 'send_s3_from_file', 'send_s3_from_dir', 'send_s3_from_url']
 
 # mypy: disable-error-code="arg-type"
@@ -31,20 +31,25 @@
 
         config (ApplicationConfig): application configuration
         terraform_module (TerraformModuleIdentifier): module identifier
         version (str): version to publish
         source (str): module source
 
     Raise:
-        (RuntimeError): if source did not exists
+        (RuntimeError): if source did not exists or if specified version and module is ever published.
     """
     config.validate()
     # remove the v
     version = version if not version.lower().startswith("v") else version[1:]
 
+    if exists(config=config, terraform_module=terraform_module, version=version):
+        msg = f"Version {version} for module {terraform_module.module_id} ever exist"
+        logger.error(msg)
+        raise RuntimeError(msg)
+
     s3_key = terraform_module.get_bucket_key(version=version)
     logger.debug(f"Put module archive to {s3_key}")
 
     if source.lower().startswith("http"):
         send_s3_from_url(config=config, source_url=source, s3_key=s3_key)
     else:
         _source = Path(source)
@@ -52,39 +57,41 @@
             raise RuntimeError(f"Source {source} did not exists ")
         if _source.is_file():
             send_s3_from_file(config=config, archive_file=_source, s3_key=s3_key)
 
         send_s3_from_dir(config=config, archive_dir=_source, s3_key=s3_key)
 
     publish_url = terraform_module.get_publish_url(bucket_name=config.bucket_name, version=version)
+    # experimental API
+    # publish_url = terraform_module.get_blob_url(repository_url=config.repository_url, version=version)
     logger.debug(f"url: {publish_url}")
     publish_module(config=config, terraform_module=terraform_module, version=version, source=publish_url)
 
     return publish_url
 
 
 def send_s3_from_file(config: ApplicationConfig, archive_file: str, s3_key: str):
     s3 = client('s3')
     with open(archive_file, "rb") as object_data:
         s3.put_object(Bucket=config.bucket_name, Key=s3_key, Body=object_data)
 
 
 def send_s3_from_dir(config: ApplicationConfig, archive_dir: str, s3_key: str):
-    archive_file = Path.cwd() / "archive.tar.gz"
+    archive_file = Path.cwd() / BUCKET_FILE_NAME
     try:
         with tarfile.open(archive_file, "w:gz") as tar:
             tar.add(archive_dir, arcname=".", filter=lambda a: a if not a.name.startswith("./.") else None)
         send_s3_from_file(config=config, archive_file=archive_file, s3_key=s3_key)
     finally:
         archive_file.unlink()
 
 
 def send_s3_from_url(config: ApplicationConfig, source_url: str, s3_key: str):
     opener = urllib.request.build_opener()
-    archive_file = Path.cwd() / "archive.tar.gz"
+    archive_file = Path.cwd() / BUCKET_FILE_NAME
     try:
         with open(archive_file, "wb") as archive:
             with opener.open(source_url) as object_data:
                 archive.write(object_data.read())
         send_s3_from_file(config=config, archive_file=archive_file, s3_key=s3_key)
     finally:
         archive_file.unlink()
```

### Comparing `aws_terraform_registry-1.0.0/aws_terraform_registry/common/token.py` & `aws_terraform_registry-1.1.0/aws_terraform_registry/common/token.py`

 * *Files identical despite different names*

### Comparing `aws_terraform_registry-1.0.0/aws_terraform_registry/config.py` & `aws_terraform_registry-1.1.0/aws_terraform_registry/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,14 +40,18 @@
         """Finalize configuration.
 
         Feed attributs from TFR_xxxx env variable if exists.
         """
         # Feed from env var
         load_env(self, prefix='tfr')
 
+        # remove ending '/'
+        if self.repository_url and self.repository_url.endswith('/'):
+            self.repository_url = self.repository_url[0:-2]
+
     def validate(self):
         """Validate each attributs.
 
         Raise:
             (RuntimeError): if an attribut is empty
 
         """
```

### Comparing `aws_terraform_registry-1.0.0/pyproject.toml` & `aws_terraform_registry-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws_terraform_registry"
-version = "1.0.0"
+version = "1.1.0"
 description = "Python client tool for aws private terraform registry."
 license = "MIT"
 authors = ["Jerome Guibert <jguibert@gmail.com>"]
 readme = "README.md"
 homepage = "https://pypi.org/project/terraform-aws-tf-registry-cli"
 documentation = "https://geronimo-iia.github.io/terraform-aws-tf-registry-cli/"
 repository = "https://github.com/geronimo-iia/terraform-aws-tf-registry-cli"
```

### Comparing `aws_terraform_registry-1.0.0/PKG-INFO` & `aws_terraform_registry-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-terraform-registry
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python client tool for aws private terraform registry.
 Home-page: https://pypi.org/project/terraform-aws-tf-registry-cli
 License: MIT
 Author: Jerome Guibert
 Author-email: jguibert@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,15 +58,15 @@
 
 
 ## Installation
 
 Install this library directly into an activated virtual environment:
 
 ```text
-$ python3 -m pip install terraform-aws-tf-registry-cli
+$ python3 -m pip install terraform-aws-tf-registry
 ```
 
 ## Configuration
 
 We have to provide few informations to this client :
 
 
@@ -118,22 +118,23 @@
 ```bash
 > tfr
 usage: tfr [-h] {config,generate-token,generate-terraformrc,publish,release} ...
 
 Manage terraform registry
 
 positional arguments:
-  {config,generate-token,generate-terraformrc,publish,release}
+  {config,generate-token,generate-terraformrc,release,unpublish,publish}
                         commands
     config              Show configuration parameters
     generate-token      Generate an access token
     generate-terraformrc
                         Generate terraformrc configuration file
-    publish             Publish a terraform module from custom source.
     release             Release a terraform module from custom source.
+    publish             Publish a terraform module from custom source.
+    unpublish           Unpublish a terraform module (Keep archive on s3).
 
 optional arguments:
   -h, --help            show this help message and exit
   ```
 
 ### Configuration
 
@@ -202,23 +203,42 @@
 
 > `publish`: register the source module as is in the aws private terraform regstry. You could have access issue if this url is not public.
 
 > `release`: 
 >
 >    - store the source into the dedicated bucket of aws private terraform regstry. The access is managed within registry.
 >    - archive (targ.gz) if the source is a folder
->    - download the source if it's an http utl
+>    - download the source if it's an http url
+>    - As your module will be stored within registry bucket, terraform client will use s3 signed url
 
-We use `release` from our ci/cd pipeline and `publish` when we have to do something like 'quick and dirty' ... (It never happen, I swear !)
+We use `release` from our ci/cd pipeline and `publish` only when we have to do something like 'quick and dirty' ... (It never happen, I swear !)
 
+### Release command
 
-### Publish command
+```bash
+usage: tfr release [-h] [-namespace NAMESPACE] -name NAME -system SYSTEM -version VERSION -source SOURCE
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -namespace NAMESPACE, --namespace NAMESPACE
+                        module namespace
+  -name NAME, --name NAME
+                        module name
+  -system SYSTEM, --system SYSTEM
+                        module system (aws, ...)
+  -version VERSION, --version VERSION
+                        module version
+  -source SOURCE, --source SOURCE
+                        module source
+```
+
+### Unpublish command
 
 ```bash
-usage: tfr publish [-h] [-namespace NAMESPACE] -name NAME -system SYSTEM -version VERSION -source SOURCE
+usage: tfr unpublish [-h] [-namespace NAMESPACE] -name NAME -system SYSTEM -version VERSION -source SOURCE
 
 optional arguments:
   -h, --help            show this help message and exit
   -namespace NAMESPACE, --namespace NAMESPACE
                         module namespace
   -name NAME, --name NAME
                         module name
@@ -226,18 +246,19 @@
                         module system (aws, ...)
   -version VERSION, --version VERSION
                         module version
   -source SOURCE, --source SOURCE
                         module source
 ```
 
-### Release command
+
+### Publish command
 
 ```bash
-usage: tfr release [-h] [-namespace NAMESPACE] -name NAME -system SYSTEM -version VERSION -source SOURCE
+usage: tfr publish [-h] [-namespace NAMESPACE] -name NAME -system SYSTEM -version VERSION -source SOURCE
 
 optional arguments:
   -h, --help            show this help message and exit
   -namespace NAMESPACE, --namespace NAMESPACE
                         module namespace
   -name NAME, --name NAME
                         module name
@@ -247,7 +268,8 @@
                         module version
   -source SOURCE, --source SOURCE
                         module source
 ```
 
 
 
+
```

