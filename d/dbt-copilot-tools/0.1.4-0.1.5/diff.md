# Comparing `tmp/dbt_copilot_tools-0.1.4.tar.gz` & `tmp/dbt_copilot_tools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_copilot_tools-0.1.4.tar", max compression
+gzip compressed data, was "dbt_copilot_tools-0.1.5.tar", max compression
```

## Comparing `dbt_copilot_tools-0.1.4.tar` & `dbt_copilot_tools-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1090 2023-06-16 11:05:25.987520 dbt_copilot_tools-0.1.4/LICENSE
--rw-r--r--   0        0        0    20712 2023-06-22 15:45:06.988416 dbt_copilot_tools-0.1.4/commands/COMMANDS.md
--rw-r--r--   0        0        0     1679 2023-06-22 15:42:02.772921 dbt_copilot_tools-0.1.4/commands/README.md
--rw-r--r--   0        0        0        0 2023-06-02 08:46:48.576039 dbt_copilot_tools-0.1.4/commands/__init__.py
--rwxr-xr-x   0        0        0     9980 2023-06-22 13:57:32.008663 dbt_copilot_tools-0.1.4/commands/bootstrap_cli.py
--rwxr-xr-x   0        0        0     2560 2023-06-20 14:07:55.205282 dbt_copilot_tools-0.1.4/commands/check_cloudformation.py
--rwxr-xr-x   0        0        0    13488 2023-06-20 09:47:08.337250 dbt_copilot_tools-0.1.4/commands/codebuild_cli.py
--rwxr-xr-x   0        0        0     8582 2023-06-15 16:41:34.056908 dbt_copilot_tools-0.1.4/commands/copilot_cli.py
--rwxr-xr-x   0        0        0    20699 2023-06-20 09:47:08.337507 dbt_copilot_tools-0.1.4/commands/dns_cli.py
--rw-r--r--   0        0        0     5902 2023-06-16 11:05:25.989196 dbt_copilot_tools-0.1.4/commands/utils.py
--rwxr-xr-x   0        0        0      880 2023-06-22 14:38:58.585299 dbt_copilot_tools-0.1.4/copilot_helper.py
--rw-r--r--   0        0        0     1169 2023-06-22 15:46:26.732715 dbt_copilot_tools-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 dbt_copilot_tools-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-16 11:05:25.987520 dbt_copilot_tools-0.1.5/LICENSE
+-rw-r--r--   0        0        0    13596 2023-06-27 16:14:10.422589 dbt_copilot_tools-0.1.5/commands/COMMANDS.md
+-rw-r--r--   0        0        0     1737 2023-06-27 16:14:10.422751 dbt_copilot_tools-0.1.5/commands/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 08:46:48.576039 dbt_copilot_tools-0.1.5/commands/__init__.py
+-rwxr-xr-x   0        0        0    10214 2023-06-27 16:01:04.635244 dbt_copilot_tools-0.1.5/commands/bootstrap_cli.py
+-rwxr-xr-x   0        0        0     2560 2023-06-20 14:07:55.205282 dbt_copilot_tools-0.1.5/commands/check_cloudformation.py
+-rwxr-xr-x   0        0        0    13488 2023-06-20 09:47:08.337250 dbt_copilot_tools-0.1.5/commands/codebuild_cli.py
+-rwxr-xr-x   0        0        0     8582 2023-06-15 16:41:34.056908 dbt_copilot_tools-0.1.5/commands/copilot_cli.py
+-rwxr-xr-x   0        0        0    20842 2023-06-27 16:01:14.828248 dbt_copilot_tools-0.1.5/commands/dns_cli.py
+-rw-r--r--   0        0        0     5994 2023-06-27 16:14:10.423077 dbt_copilot_tools-0.1.5/commands/utils.py
+-rw-r--r--   0        0        0     5695 2023-06-27 16:01:14.828564 dbt_copilot_tools-0.1.5/commands/waf_cli.py
+-rwxr-xr-x   0        0        0      970 2023-06-27 16:14:10.423415 dbt_copilot_tools-0.1.5/copilot_helper.py
+-rw-r--r--   0        0        0     1188 2023-06-27 16:14:10.423762 dbt_copilot_tools-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2750 1970-01-01 00:00:00.000000 dbt_copilot_tools-0.1.5/PKG-INFO
```

### Comparing `dbt_copilot_tools-0.1.4/LICENSE` & `dbt_copilot_tools-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.4/commands/README.md` & `dbt_copilot_tools-0.1.5/commands/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -45,8 +45,8 @@
 
 Commands:
   instructions     Show migration instructions.
   make-config      Generate copilot boilerplate code.
   migrate-secrets  Migrate secrets from your gov paas application to...
 ```
 
-See the [Commands Reference](./COMMANDS.md) for a list of all available subcommands.
+See the [Commands Reference](https://github.com/uktrade/copilot-tools/blob/main/commands/COMMANDS.md) for a list of all available subcommands.
```

### Comparing `dbt_copilot_tools-0.1.4/commands/bootstrap_cli.py` & `dbt_copilot_tools-0.1.5/commands/bootstrap_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 
 import click
 import yaml
 from cloudfoundry_client.client import CloudFoundryClient
 from schema import Optional
 from schema import Schema
 
-from .utils import SSM_PATH
-from .utils import camel_case
-from .utils import get_ssm_secret_names
-from .utils import mkdir
-from .utils import mkfile
-from .utils import set_ssm_param
-from .utils import setup_templates
+from commands.utils import SSM_PATH
+from commands.utils import camel_case
+from commands.utils import check_aws_conn
+from commands.utils import get_ssm_secret_names
+from commands.utils import mkdir
+from commands.utils import mkfile
+from commands.utils import set_ssm_param
+from commands.utils import setup_templates
 
 config_schema = Schema(
     {
         "app": str,
         "environments": {str: {Optional("certificate_arns"): [str]}},
         "services": [
             {
@@ -171,29 +172,31 @@
         "\nGitHub documentation: "
         "https://github.com/uktrade/platform-documentation/blob/main/gov-pass-to-copiltot-migration",
     )
 
 
 @bootstrap.command()
 @click.argument("config-file", type=click.Path(exists=True))
+@click.option("--project-profile", required=True, help="aws account profile name")
 @click.option("--env", help="Migrate secrets from a specific environment")
 @click.option("--svc", help="Migrate secrets from a specific service")
 @click.option("--overwrite", is_flag=True, show_default=True, default=False, help="Overwrite existing secrets?")
 @click.option("--dry-run", is_flag=True, show_default=True, default=False, help="dry run")
-def migrate_secrets(config_file, env, svc, overwrite, dry_run):
+def migrate_secrets(config_file, project_profile, env, svc, overwrite, dry_run):
     """
     Migrate secrets from your gov paas application to AWS/copilot.
 
     You need to be authenticated via cf cli and the AWS cli to use this commmand.
 
     If you're using AWS profiles, use the AWS_PROFILE env var to indicate the which profile to use, e.g.:
 
     AWS_PROFILE=myaccount copilot-bootstrap.py ...
     """
 
+    check_aws_conn(project_profile)
     # TODO: optional SSM or secret manager
 
     cf_client = CloudFoundryClient.build_from_cf_config()
     config = load_and_validate_config(config_file)
 
     if env and env not in config["environments"].keys():
         raise click.ClickException(f"{env} is not an environment in {config_file}")
```

### Comparing `dbt_copilot_tools-0.1.4/commands/check_cloudformation.py` & `dbt_copilot_tools-0.1.5/commands/check_cloudformation.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.4/commands/codebuild_cli.py` & `dbt_copilot_tools-0.1.5/commands/codebuild_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.4/commands/copilot_cli.py` & `dbt_copilot_tools-0.1.5/commands/copilot_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.4/commands/dns_cli.py` & `dbt_copilot_tools-0.1.5/commands/dns_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,18 +173,18 @@
                     },
                 ],
             },
         )
 
     check_response(response)
     click.echo(
-        click.style(f"{records['Name']}, Type: {records['Type']}", fg="white", bold=True) +
-        click.style("Added.", fg="magenta")
-        )
-    return response['ChangeInfo']['Status']
+        click.style(f"{records['Name']}, Type: {records['Type']}", fg="white", bold=True)
+        + click.style("Added.", fg="magenta"),
+    )
+    return response["ChangeInfo"]["Status"]
 
 
 def check_for_records(client, parent_id, subdom, subdom_id):
     records_to_add = []
     response = client.list_resource_record_sets(
         HostedZoneId=parent_id,
     )
@@ -282,15 +282,17 @@
     # Check if base domain is valid
     if base_domain[-1] != ".":
         base_domain = base_domain + "."
 
     if base_domain not in hosted_zones:
         click.secho(
             f"The base domain: {base_domain} does not exist in your AWS domain account \
-                {response['HostedZones']}", fg='red')
+                {response['HostedZones']}",
+            fg="red",
+        )
         exit()
 
     base_len = len(base_domain.split(".")) - 1
     parts = domain.split(".")
 
     for _ in range(len(parts) - 1):
         subdom = ".".join(parts) + "."
@@ -313,78 +315,15 @@
 
     # add records to hosted zone to validate certificate
     cert_arn = create_cert(acm_client, domain_client, domain, base_len)
 
     return cert_arn
 
 
-@click.group()
-def domain():
-    pass
-
-
-@domain.command()
-@click.option("--path", help="path of copilot folder", required=True)
-@click.option("--domain-profile", help="aws account profile name for R53 domains account", required=True)
-@click.option("--project-profile", help="aws account profile name for certificates account", required=True)
-@click.option("--base-domain", help="root domain", required=True)
-def check_domain(path, domain_profile, project_profile, base_domain):
-    """Scans to see if Domain exists."""
-
-    domain_session = check_aws_conn(domain_profile)
-    project_session = check_aws_conn(project_profile)
-
-    if not os.path.exists(path):
-        click.secho("Please check path, manifest file not found", fg="red")
-        exit()
-
-    if path.split(".")[-1] == "yml" or path.split(".")[-1] == "yaml":
-        click.secho("Please do not include the filename in the path", fg="red")
-        exit()
-
-    cert_list = {}
-    for root, dirs, files in os.walk(path):
-        for file in files:
-            if file == "manifest.yml" or file == "manifest.yaml":
-                # Need to check that the manifest file is correctly configured.
-                with open(os.path.join(root, file), "r") as fd:
-                    conf = yaml.safe_load(fd)
-                    if "environments" in conf:
-                        click.echo(
-                            click.style("Checking file: ", fg="cyan")
-                            + click.style(os.path.join(root, file), fg="white"),
-                        )
-                        click.secho("Domains listed in manifest file", fg="cyan", underline=True)
-
-                        for env, domain in conf["environments"].items():
-                            click.secho("Environment: " + env + "\t=> Domain: " + domain["http"]["alias"], fg="yellow")
-                            cert_arn = check_r53(domain_session, project_session, domain["http"]["alias"], base_domain)
-                            cert_list.update({domain["http"]["alias"]: cert_arn})
-    if cert_list:
-        click.secho("\nHere are your Cert ARNs:", fg="cyan")
-        for domain, cert in cert_list.items():
-            click.secho(f"Domain: {domain}\t => Cert ARN: {cert}", fg="white", bold=True)
-    else:
-        click.secho("No domains found, please check the manifest file", fg="red")
-
-
-@domain.command()
-@click.option("--app", help="Application Name", required=True)
-@click.option("--domain-profile", help="aws account profile name for R53 domains account", required=True)
-@click.option("--project-profile", help="aws account profile name for application account", required=True)
-@click.option("--svc", help="Service Name", required=True)
-@click.option("--env", help="Environment", required=True)
-def assign_domain(app, domain_profile, project_profile, svc, env):
-    """Check R53 domain is pointing to the correct ECS Load Blanacer."""
-    domain_session = check_aws_conn(domain_profile)
-    project_session = check_aws_conn(project_profile)
-
-    ensure_cwd_is_repo_root()
-
-    # Find the Load Balancer name.
+def lb_domain(project_session, app, svc, env):
     proj_client = project_session.client("ecs")
 
     response = proj_client.list_clusters()
     check_response(response)
     no_items = True
     for cluster_arn in response["clusterArns"]:
         cluster_name = cluster_arn.split("/")[1]
@@ -393,15 +332,15 @@
         cluster_env = cluster_name_items[1]
         if cluster_app == app and cluster_env == env:
             no_items = False
             break
 
     if no_items:
         click.echo(
-            click.style(f"There are no clusters matching ", fg="red")
+            click.style("There are no clusters matching ", fg="red")
             + click.style(f"{app}", fg="white", bold=True)
             + click.style("in this aws account", fg="red"),
         )
         exit()
 
     response = proj_client.list_services(cluster=cluster_name)
     check_response(response)
@@ -439,31 +378,100 @@
                 "loadBalancers"
             ][0]["targetGroupArn"],
         ],
     )["TargetGroups"][0]["LoadBalancerArns"][0]
 
     response = elb_client.describe_load_balancers(LoadBalancerArns=[elb_arn])
     check_response(response)
-    elb_name = response["LoadBalancers"][0]["DNSName"]
 
     # Find the domain name
     with open(f"./copilot/{svc}/manifest.yml", "r") as fd:
         conf = yaml.safe_load(fd)
         if "environments" in conf:
             for domain in conf["environments"].items():
                 if domain[0] == env:
                     domain_name = domain[1]["http"]["alias"]
 
-        click.echo(
-            click.style("The Domain: ", fg="yellow")
-            + click.style(f"{domain_name}\n", fg="white", bold=True)
-            + click.style("has been assigned the Load Balancer: ", fg="yellow")
-            + click.style(f"{elb_name}\n", fg="white", bold=True)
-            + click.style("Checking to see if this is in R53", fg="yellow"),
-        )
+    return domain_name, response
+
+
+@click.group()
+def domain():
+    pass
+
+
+@domain.command()
+@click.option("--path", help="path of copilot folder", required=True)
+@click.option("--domain-profile", help="aws account profile name for R53 domains account", required=True)
+@click.option("--project-profile", help="aws account profile name for certificates account", required=True)
+@click.option("--base-domain", help="root domain", required=True)
+def check_domain(path, domain_profile, project_profile, base_domain):
+    """Scans to see if Domain exists."""
+
+    domain_session = check_aws_conn(domain_profile)
+    project_session = check_aws_conn(project_profile)
+
+    if not os.path.exists(path):
+        click.secho("Please check path, manifest file not found", fg="red")
+        exit()
+
+    if path.split(".")[-1] == "yml" or path.split(".")[-1] == "yaml":
+        click.secho("Please do not include the filename in the path", fg="red")
+        exit()
+
+    cert_list = {}
+    for root, dirs, files in os.walk(path):
+        for file in files:
+            if file == "manifest.yml" or file == "manifest.yaml":
+                # Need to check that the manifest file is correctly configured.
+                with open(os.path.join(root, file), "r") as fd:
+                    conf = yaml.safe_load(fd)
+                    if "environments" in conf:
+                        click.echo(
+                            click.style("Checking file: ", fg="cyan")
+                            + click.style(os.path.join(root, file), fg="white"),
+                        )
+                        click.secho("Domains listed in manifest file", fg="cyan", underline=True)
+
+                        for env, domain in conf["environments"].items():
+                            click.secho("Environment: " + env + "\t=> Domain: " + domain["http"]["alias"], fg="yellow")
+                            cert_arn = check_r53(domain_session, project_session, domain["http"]["alias"], base_domain)
+                            cert_list.update({domain["http"]["alias"]: cert_arn})
+    if cert_list:
+        click.secho("\nHere are your Cert ARNs:", fg="cyan")
+        for domain, cert in cert_list.items():
+            click.secho(f"Domain: {domain}\t => Cert ARN: {cert}", fg="white", bold=True)
+    else:
+        click.secho("No domains found, please check the manifest file", fg="red")
+
+
+@domain.command()
+@click.option("--app", help="Application Name", required=True)
+@click.option("--domain-profile", help="aws account profile name for R53 domains account", required=True)
+@click.option("--project-profile", help="aws account profile name for application account", required=True)
+@click.option("--svc", help="Service Name", required=True)
+@click.option("--env", help="Environment", required=True)
+def assign_domain(app, domain_profile, project_profile, svc, env):
+    """Check R53 domain is pointing to the correct ECS Load Blanacer."""
+    domain_session = check_aws_conn(domain_profile)
+    project_session = check_aws_conn(project_profile)
+
+    ensure_cwd_is_repo_root()
+
+    # Find the Load Balancer name.
+    domain_name, response = lb_domain(project_session, app, svc, env)
+    elb_name = response["LoadBalancers"][0]["DNSName"]
+
+    click.echo(
+        click.style("The Domain: ", fg="yellow")
+        + click.style(f"{domain_name}\n", fg="white", bold=True)
+        + click.style("has been assigned the Load Balancer: ", fg="yellow")
+        + click.style(f"{elb_name}\n", fg="white", bold=True)
+        + click.style("Checking to see if this is in R53", fg="yellow"),
+    )
 
     domain_client = domain_session.client("route53")
     response = domain_client.list_hosted_zones_by_name()
     check_response(response)
 
     # Scan R53 Zone for matching domains and update records if needed.
     hosted_zones = {}
```

### Comparing `dbt_copilot_tools-0.1.4/commands/utils.py` & `dbt_copilot_tools-0.1.5/commands/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         Value=param_value,
         Type="SecureString",
         Overwrite=overwrite,
         Tags=[
             {"Key": "copilot-application", "Value": app},
             {"Key": "copilot-environment", "Value": env},
         ],
-        Tier='Intelligent-Tiering',
+        Tier="Intelligent-Tiering",
     )
 
     if overwrite and exists:
         # Tags can't be updated when overwriting
         del args["Tags"]
 
     client.put_parameter(**args)
@@ -86,15 +86,15 @@
 
     return sorted(secret_names)
 
 
 def setup_templates():
     template_path = Path(__file__).parent.parent / Path("templates")
     templateLoader = jinja2.FileSystemLoader(searchpath=template_path)
-    templateEnv = jinja2.Environment(loader=templateLoader)
+    templateEnv = jinja2.Environment(loader=templateLoader, keep_trailing_newline=True)
 
     templates = {
         "instructions": templateEnv.get_template("instructions.txt"),
         "storage-instructions": templateEnv.get_template("storage-instructions.txt"),
         "svc": {
             "public-manifest": templateEnv.get_template("svc/manifest-public.yml"),
             "backend-manifest": templateEnv.get_template("svc/manifest-backend.yml"),
@@ -106,21 +106,22 @@
             "rds-postgres": templateEnv.get_template("addons/env/rds-postgres.yml"),
             "aurora-postgres": templateEnv.get_template("addons/env/aurora-postgres.yml"),
             "redis": templateEnv.get_template("addons/env/redis-cluster.yml"),
             "s3": templateEnv.get_template("addons/env/s3.yml"),
             "waf": templateEnv.get_template("addons/env/waf.yml"),
             "parameters": templateEnv.get_template("addons/env/addons.parameters.yml"),
         },
+        "docs": templateEnv.get_template("COMMANDS.md.jinja"),
     }
 
     return templates
 
 
 def ensure_cwd_is_repo_root():
-    """Exit if we're not in the root of the repo"""
+    """Exit if we're not in the root of the repo."""
 
     if not Path("./copilot").exists() or not Path("./copilot").is_dir():
         click.secho(
             "Cannot find copilot directory. Run this command in the root of the deployment repository.",
             bg="red",
         )
         exit(1)
```

### Comparing `dbt_copilot_tools-0.1.4/copilot_helper.py` & `dbt_copilot_tools-0.1.5/copilot_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from commands.bootstrap_cli import bootstrap as bootstrap_commands
 from commands.check_cloudformation import \
     check_cloudformation as check_cloudformation_command
 from commands.codebuild_cli import codebuild as codebuild_commands
 from commands.copilot_cli import copilot as copilot_commands
 from commands.dns_cli import domain as domain_commands
+from commands.waf_cli import waf as waf_commands
 
 
 @click.group()
 @click.version_option(
     version=version("dbt-copilot-tools"),
     message=f"dbt-copilot-tools %(version)s",
 )
@@ -22,10 +23,11 @@
 
 
 copilot_helper.add_command(bootstrap_commands)
 copilot_helper.add_command(check_cloudformation_command)
 copilot_helper.add_command(copilot_commands)
 copilot_helper.add_command(codebuild_commands)
 copilot_helper.add_command(domain_commands)
+copilot_helper.add_command(waf_commands)
 
 if __name__ == "__main__":
     copilot_helper()
```

### Comparing `dbt_copilot_tools-0.1.4/pyproject.toml` & `dbt_copilot_tools-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 119
 
 [tool.poetry]
 name = "dbt-copilot-tools"
-version = "0.1.4"
+version = "0.1.5"
 description = "Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot."
 authors = ["Department for Business and Trade Platform Team <sre-team@digital.trade.gov.uk>"]
 license = "MIT"
 readme = "commands/README.md"
 packages = [
     { include = "commands" },
     { include = "copilot_helper.py" }
@@ -19,19 +19,20 @@
 [tool.poetry.dependencies]
 Jinja2 = "3.1.2"
 PyYAML = "6.0"
 boto3 = "1.26.31"
 boto3-stubs = "1.26.148"
 botocore = "1.29.31"
 click = "8.1.3"
-cloudfoundry-client = "1.34.1"
+cloudfoundry-client = "1.35.0"
 jsonschema = "4.17.3"
 mypy-boto3-codebuild = "1.26.0.post1"
 python = "^3.9"
 schema = "0.7.5"
+cfn-flip = "1.3.0"
 
 [tool.poetry.group.dev.dependencies]
 cfn-lint = "^0.77.7"
 moto = "^4.1.11"
 pyfakefs = "^5.2.2"
 pytest = "^7.3.1"
 pytest-env = "^0.8.1"
```

### Comparing `dbt_copilot_tools-0.1.4/PKG-INFO` & `dbt_copilot_tools-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-copilot-tools
-Version: 0.1.4
+Version: 0.1.5
 Summary: Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot.
 License: MIT
 Author: Department for Business and Trade Platform Team
 Author-email: sre-team@digital.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,16 +12,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (==3.1.2)
 Requires-Dist: PyYAML (==6.0)
 Requires-Dist: boto3 (==1.26.31)
 Requires-Dist: boto3-stubs (==1.26.148)
 Requires-Dist: botocore (==1.29.31)
+Requires-Dist: cfn-flip (==1.3.0)
 Requires-Dist: click (==8.1.3)
-Requires-Dist: cloudfoundry-client (==1.34.1)
+Requires-Dist: cloudfoundry-client (==1.35.0)
 Requires-Dist: jsonschema (==4.17.3)
 Requires-Dist: mypy-boto3-codebuild (==1.26.0.post1)
 Requires-Dist: schema (==0.7.5)
 Description-Content-Type: text/markdown
 
 # DBT Copilot Tools
 
@@ -70,9 +71,9 @@
 
 Commands:
   instructions     Show migration instructions.
   make-config      Generate copilot boilerplate code.
   migrate-secrets  Migrate secrets from your gov paas application to...
 ```
 
-See the [Commands Reference](./COMMANDS.md) for a list of all available subcommands.
+See the [Commands Reference](https://github.com/uktrade/copilot-tools/blob/main/commands/COMMANDS.md) for a list of all available subcommands.
```

