# Comparing `tmp/aws-ssm-tools-1.5.1.tar.gz` & `tmp/aws-ssm-tools-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aws-ssm-tools-1.5.1.tar", last modified: Tue Feb 21 04:59:09 2023, max compression
+gzip compressed data, was "dist/aws-ssm-tools-1.6.0.tar", last modified: Tue Jun 27 02:20:11 2023, max compression
```

## Comparing `aws-ssm-tools-1.5.1.tar` & `aws-ssm-tools-1.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/aws_ssm_tools.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15752 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/aws_ssm_tools.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      471 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/aws_ssm_tools.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/aws_ssm_tools.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      271 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/aws_ssm_tools.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       41 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/aws_ssm_tools.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/aws_ssm_tools.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/ssm_tools/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/ssm_tools/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5725 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/ssm_tools/common.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5046 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/ssm_tools/ec2_instance_connect.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     3793 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/ssm_tools/ecs_session_cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12541 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/ssm_tools/resolver.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     5656 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/ssm_tools/ssm_session_cli.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     6636 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/ssm_tools/ssm_ssh_cli.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    13438 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/ssm_tools/ssm_tunnel_cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1604 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/ssm_tools/talker.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11856 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3388 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15752 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-02-21 04:59:09.000000 aws-ssm-tools-1.5.1/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 02:20:11.000000 aws-ssm-tools-1.6.0/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 02:20:11.000000 aws-ssm-tools-1.6.0/aws_ssm_tools.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15752 2023-06-27 02:20:11.000000 aws-ssm-tools-1.6.0/aws_ssm_tools.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      471 2023-06-27 02:20:11.000000 aws-ssm-tools-1.6.0/aws_ssm_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-27 02:20:11.000000 aws-ssm-tools-1.6.0/aws_ssm_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      271 2023-06-27 02:20:11.000000 aws-ssm-tools-1.6.0/aws_ssm_tools.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       41 2023-06-27 02:20:11.000000 aws-ssm-tools-1.6.0/aws_ssm_tools.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-06-27 02:20:11.000000 aws-ssm-tools-1.6.0/aws_ssm_tools.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 02:20:11.000000 aws-ssm-tools-1.6.0/ssm_tools/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2023-06-27 02:20:10.000000 aws-ssm-tools-1.6.0/ssm_tools/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6583 2023-06-27 02:20:10.000000 aws-ssm-tools-1.6.0/ssm_tools/common.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5046 2023-06-27 02:20:10.000000 aws-ssm-tools-1.6.0/ssm_tools/ec2_instance_connect.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     3793 2023-06-27 02:20:10.000000 aws-ssm-tools-1.6.0/ssm_tools/ecs_session_cli.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12541 2023-06-27 02:20:10.000000 aws-ssm-tools-1.6.0/ssm_tools/resolver.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     5656 2023-06-27 02:20:10.000000 aws-ssm-tools-1.6.0/ssm_tools/ssm_session_cli.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     7296 2023-06-27 02:20:10.000000 aws-ssm-tools-1.6.0/ssm_tools/ssm_ssh_cli.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    13438 2023-06-27 02:20:10.000000 aws-ssm-tools-1.6.0/ssm_tools/ssm_tunnel_cli.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1604 2023-06-27 02:20:10.000000 aws-ssm-tools-1.6.0/ssm_tools/talker.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11856 2023-06-27 02:20:10.000000 aws-ssm-tools-1.6.0/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3388 2023-06-27 02:20:10.000000 aws-ssm-tools-1.6.0/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15752 2023-06-27 02:20:11.000000 aws-ssm-tools-1.6.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-27 02:20:11.000000 aws-ssm-tools-1.6.0/setup.cfg
```

### Comparing `aws-ssm-tools-1.5.1/aws_ssm_tools.egg-info/PKG-INFO` & `aws-ssm-tools-1.6.0/aws_ssm_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ssm-tools
-Version: 1.5.1
+Version: 1.6.0
 Summary: Tools for AWS Systems Manager: ec2-session ecs-session ec2-ssh ssm-tunnel ssm-session ssm-ssh
 Home-page: https://github.com/mludvig/aws-ssm-tools
 Author: Michael Ludvig
 Author-email: mludvig@logix.net.nz
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/mludvig/aws-ssm-tools/issues
 Project-URL: Documentation, https://github.com/mludvig/aws-ssm-tools/blob/master/README.md
```

### Comparing `aws-ssm-tools-1.5.1/ssm_tools/common.py` & `aws-ssm-tools-1.6.0/ssm_tools/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,19 +143,46 @@
         result = subprocess.run([session_manager_plugin, "--version"], stdout=subprocess.PIPE, check=False)
         plugin_version = result.stdout.decode("ascii").strip()
         logger.debug(f"{session_manager_plugin} version {plugin_version}")
 
         if packaging.version.parse(plugin_version) >= packaging.version.parse(version_required):
             return True
 
-        logger.error(f"ERROR: session-manager-plugin version {plugin_version} is installed, {version_required} is required")
+        logger.error(f"session-manager-plugin version {plugin_version} is installed, {version_required} is required")
     except FileNotFoundError:
-        logger.error(f"ERROR: {session_manager_plugin} not installed")
+        logger.error(f"{session_manager_plugin} not installed")
 
-    logger.error("ERROR: Check out https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html for instructions")
+    logger.error("Check out https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html for instructions")
+
+    return False
+
+
+# ---------------------------------------------------------
+
+
+__all__.append("verify_awscli_version")
+
+
+def verify_awscli_version(version_required: str, logger: logging.Logger) -> bool:
+    """
+    Verify that the aws-cli is installed and is of a required version or newer.
+    """
+    aws_cli = "aws"
+
+    try:
+        result = subprocess.run([aws_cli, "--version"], stdout=subprocess.PIPE, check=False)
+        plugin_version = result.stdout.decode("ascii").strip().split(" ")[0].split("/")[1]
+        logger.debug(f"AWS-CLI version {plugin_version}")
+
+        if packaging.version.parse(plugin_version) >= packaging.version.parse(version_required):
+            return True
+
+        logger.error(f"AWS-CLI version {plugin_version} is installed, {version_required} is required")
+    except FileNotFoundError:
+        logger.error("AWS-CLI is not installed")
 
     return False
 
 
 # ---------------------------------------------------------
 
 __all__.append("AWSSessionBase")
```

### Comparing `aws-ssm-tools-1.5.1/ssm_tools/ec2_instance_connect.py` & `aws-ssm-tools-1.6.0/ssm_tools/ec2_instance_connect.py`

 * *Files identical despite different names*

### Comparing `aws-ssm-tools-1.5.1/ssm_tools/ecs_session_cli.py` & `aws-ssm-tools-1.6.0/ssm_tools/ecs_session_cli.py`

 * *Files identical despite different names*

### Comparing `aws-ssm-tools-1.5.1/ssm_tools/resolver.py` & `aws-ssm-tools-1.6.0/ssm_tools/resolver.py`

 * *Files identical despite different names*

### Comparing `aws-ssm-tools-1.5.1/ssm_tools/ssm_session_cli.py` & `aws-ssm-tools-1.6.0/ssm_tools/ssm_session_cli.py`

 * *Files identical despite different names*

### Comparing `aws-ssm-tools-1.5.1/ssm_tools/ssm_ssh_cli.py` & `aws-ssm-tools-1.6.0/ssm_tools/ssm_ssh_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import logging
 import argparse
 
 from typing import Tuple, List
 
 import botocore.exceptions
 
-from .common import add_general_parameters, show_version, configure_logging, verify_plugin_version
+from .common import add_general_parameters, show_version, configure_logging, verify_plugin_version, verify_awscli_version
 from .resolver import InstanceResolver
 from .ec2_instance_connect import EC2InstanceConnectHelper
 
 logger = logging.getLogger("ssm-tools.ec2-ssh")
 
 
 def parse_args(argv: list) -> Tuple[argparse.Namespace, List[str]]:
@@ -38,14 +38,15 @@
 
     group_instance = parser.add_argument_group("Instance Selection")
     group_instance.add_argument("--list", dest="list", action="store_true", help="List instances available for SSM Session")
 
     group_ec2ic = parser.add_argument_group("EC2 Instance Connect")
     group_ec2ic.add_argument("--send-key", dest="send_key", action="store_true", default=True, help="Send the SSH key to instance metadata using EC2 Instance Connect (default and deprecated - use --no-send-key instead)")
     group_ec2ic.add_argument("--no-send-key", dest="send_key", action="store_false", help="Send the SSH key to instance metadata using EC2 Instance Connect")
+    group_ec2ic.add_argument("--use-endpoint", dest="use_endpoint", action="store_true", default=False, help="Connect using 'EC2 Instance Connect Endpoint'")
 
     parser.description = "Open SSH connection through Session Manager"
     parser.epilog = f"""
 IMPORTANT: instances must be registered in AWS Systems Manager (SSM)
 before you can start a shell session! Instances not registered in SSM
 will not be recognised by {parser.prog} nor show up in --list output.
 
@@ -64,21 +65,29 @@
     # Require exactly one of INSTANCE or --list
     if bool(extra_args) + bool(args.list) != 1:
         parser.error("Specify either --list or SSH Options including instance name")
 
     return args, extra_args
 
 
-def start_ssh_session(ssh_args: list, profile: str = None, region: str = None) -> None:
+def start_ssh_session(ssh_args: list, profile: str, region: str, use_endpoint: bool) -> None:
     aws_args = ""
     if profile:
         aws_args += f"--profile {profile} "
     if region:
         aws_args += f"--region {region} "
-    proxy_option = ["-o", f"ProxyCommand=aws {aws_args} ssm start-session --target %h --document-name AWS-StartSSHSession --parameters portNumber=%p"]
+    if use_endpoint:
+        min_awscli_version = "2.12.0"
+        if not verify_awscli_version(min_awscli_version, logger):
+            logger.error(f"AWS CLI v{min_awscli_version} or newer is required for --use-endpoint, falling back to SSM Session Manager")
+            use_endpoint = False
+    if use_endpoint:
+        proxy_option = ["-o", f"ProxyCommand=aws {aws_args} ec2-instance-connect open-tunnel --instance-id %h"]
+    else:
+        proxy_option = ["-o", f"ProxyCommand=aws {aws_args} ssm start-session --target %h --document-name AWS-StartSSHSession --parameters portNumber=%p"]
     command = ["ssh"] + proxy_option + ssh_args
     logger.debug("Running: %s", command)
     os.execvp(command[0], command)
 
 
 def main() -> int:
     ## Deprecate old script name
@@ -175,15 +184,15 @@
             logger.warning("Could not resolve Instance ID for '%s'", instance)
             logger.warning("Perhaps the '%s' is not registered in SSM?", instance)
             sys.exit(1)
 
         if args.send_key:
             EC2InstanceConnectHelper(args).send_ssh_key(instance_id, login_name, key_file_name)
 
-        start_ssh_session(ssh_args=ssh_args, profile=args.profile, region=args.region)
+        start_ssh_session(ssh_args=ssh_args, profile=args.profile, region=args.region, use_endpoint=args.use_endpoint)
 
     except (botocore.exceptions.BotoCoreError, botocore.exceptions.ClientError) as e:
         logger.error(e)
         sys.exit(1)
 
     return 0
```

### Comparing `aws-ssm-tools-1.5.1/ssm_tools/ssm_tunnel_cli.py` & `aws-ssm-tools-1.6.0/ssm_tools/ssm_tunnel_cli.py`

 * *Files identical despite different names*

### Comparing `aws-ssm-tools-1.5.1/ssm_tools/talker.py` & `aws-ssm-tools-1.6.0/ssm_tools/talker.py`

 * *Files identical despite different names*

### Comparing `aws-ssm-tools-1.5.1/README.md` & `aws-ssm-tools-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-ssm-tools-1.5.1/setup.py` & `aws-ssm-tools-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `aws-ssm-tools-1.5.1/PKG-INFO` & `aws-ssm-tools-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ssm-tools
-Version: 1.5.1
+Version: 1.6.0
 Summary: Tools for AWS Systems Manager: ec2-session ecs-session ec2-ssh ssm-tunnel ssm-session ssm-ssh
 Home-page: https://github.com/mludvig/aws-ssm-tools
 Author: Michael Ludvig
 Author-email: mludvig@logix.net.nz
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/mludvig/aws-ssm-tools/issues
 Project-URL: Documentation, https://github.com/mludvig/aws-ssm-tools/blob/master/README.md
```

