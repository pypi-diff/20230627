# Comparing `tmp/balcony-0.1.1.tar.gz` & `tmp/balcony-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balcony-0.1.1.tar", max compression
+gzip compressed data, was "balcony-0.1.2.tar", max compression
```

## Comparing `balcony-0.1.1.tar` & `balcony-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,43 @@
--rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.1.1/LICENSE
--rw-r--r--   0        0        0     1890 2023-06-22 10:24:32.348247 balcony-0.1.1/README.md
--rw-r--r--   0        0        0      933 2023-04-29 21:23:00.565222 balcony-0.1.1/balcony/__init__.py
--rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.1.1/balcony/__main__.py
--rw-r--r--   0        0        0     5622 2023-04-21 19:12:44.411429 balcony-0.1.1/balcony/aws.py
--rw-r--r--   0        0        0    11892 2023-04-21 17:50:16.401554 balcony-0.1.1/balcony/botocore_utils.py
--rw-r--r--   0        0        0    19026 2023-06-25 12:59:49.346224 balcony-0.1.1/balcony/cli.py
--rw-r--r--   0        0        0     3621 2023-06-18 17:53:12.079460 balcony-0.1.1/balcony/config.py
--rw-r--r--   0        0        0      488 2023-04-29 22:03:44.770391 balcony-0.1.1/balcony/custom_nodes/__init__.py
--rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.1.1/balcony/custom_nodes/codebuild.py
--rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.1.1/balcony/custom_nodes/ecs.py
--rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.1.1/balcony/custom_nodes/iam.py
--rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.1.1/balcony/custom_nodes/lambda_functions.py
--rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.1.1/balcony/custom_nodes/s3.py
--rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.1.1/balcony/custom_nodes/ses.py
--rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.1.1/balcony/custom_nodes/ssm.py
--rw-r--r--   0        0        0        0 2023-06-18 18:05:04.079497 balcony-0.1.1/balcony/custom_tf_import_configs/_example_import_conf.yaml
--rw-r--r--   0        0        0      647 2023-06-22 14:01:11.797785 balcony-0.1.1/balcony/custom_tf_import_configs/ec2.yaml
--rw-r--r--   0        0        0      336 2023-06-22 11:23:28.065064 balcony-0.1.1/balcony/custom_tf_import_configs/s3.yaml
--rw-r--r--   0        0        0     3149 2023-04-15 19:49:24.900287 balcony-0.1.1/balcony/custom_yamls/_example_service.yaml
--rw-r--r--   0        0        0      517 2023-04-06 12:50:36.974851 balcony-0.1.1/balcony/custom_yamls/ec2.yaml
--rw-r--r--   0        0        0        0 2023-04-05 13:32:52.449913 balcony-0.1.1/balcony/custom_yamls/ecs.yaml
--rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.1.1/balcony/custom_yamls/iam.yaml
--rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.1.1/balcony/custom_yamls/s3.yaml
--rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.1.1/balcony/errors.py
--rw-r--r--   0        0        0    48206 2023-06-19 13:08:46.777156 balcony-0.1.1/balcony/nodes.py
--rw-r--r--   0        0        0    17113 2023-05-01 12:20:53.387726 balcony-0.1.1/balcony/reader.py
--rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.1.1/balcony/registries.py
--rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.1.1/balcony/relations.py
--rw-r--r--   0        0        0     1407 2023-06-25 08:18:38.934823 balcony-0.1.1/balcony/terraform_import/README.md
--rw-r--r--   0        0        0        0 2023-06-18 17:41:34.879852 balcony-0.1.1/balcony/terraform_import/__init__.py
--rw-r--r--   0        0        0     6272 2023-06-25 12:23:39.913627 balcony-0.1.1/balcony/terraform_import/importer.py
--rw-r--r--   0        0        0     1262 2023-06-23 11:28:38.779925 balcony-0.1.1/balcony/terraform_import/models.py
--rw-r--r--   0        0        0     2276 2023-06-23 11:28:47.429086 balcony-0.1.1/balcony/terraform_import/parsers.py
--rw-r--r--   0        0        0     2980 2023-06-19 18:24:25.368221 balcony-0.1.1/balcony/test.py
--rw-r--r--   0        0        0     6108 2023-06-18 17:25:37.430772 balcony-0.1.1/balcony/utils.py
--rw-r--r--   0        0        0     2130 2023-06-18 18:03:08.298654 balcony-0.1.1/balcony/yaml_config.py
--rw-r--r--   0        0        0     2049 2023-06-18 17:05:58.939803 balcony-0.1.1/balcony/yaml_validators.py
--rw-r--r--   0        0        0      748 2023-06-25 14:35:22.458376 balcony-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 balcony-0.1.1/setup.py
--rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 balcony-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1890 2023-06-22 10:24:32.348247 balcony-0.1.2/README.md
+-rw-r--r--   0        0        0      933 2023-04-29 21:23:00.565222 balcony-0.1.2/balcony/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.1.2/balcony/__main__.py
+-rw-r--r--   0        0        0     5622 2023-04-21 19:12:44.411429 balcony-0.1.2/balcony/aws.py
+-rw-r--r--   0        0        0    15168 2023-06-26 21:21:12.986943 balcony-0.1.2/balcony/botocore_utils.py
+-rw-r--r--   0        0        0    20638 2023-06-26 21:56:38.194764 balcony-0.1.2/balcony/cli.py
+-rw-r--r--   0        0        0     3621 2023-06-18 17:53:12.079460 balcony-0.1.2/balcony/config.py
+-rw-r--r--   0        0        0      488 2023-04-29 22:03:44.770391 balcony-0.1.2/balcony/custom_nodes/__init__.py
+-rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.1.2/balcony/custom_nodes/codebuild.py
+-rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.1.2/balcony/custom_nodes/ecs.py
+-rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.1.2/balcony/custom_nodes/iam.py
+-rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.1.2/balcony/custom_nodes/lambda_functions.py
+-rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.1.2/balcony/custom_nodes/s3.py
+-rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.1.2/balcony/custom_nodes/ses.py
+-rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.1.2/balcony/custom_nodes/ssm.py
+-rw-r--r--   0        0        0        0 2023-06-18 18:05:04.079497 balcony-0.1.2/balcony/custom_tf_import_configs/_example_import_conf.yaml
+-rw-r--r--   0        0        0      894 2023-06-26 21:37:52.076889 balcony-0.1.2/balcony/custom_tf_import_configs/ec2.yaml
+-rw-r--r--   0        0        0      289 2023-06-26 21:48:48.327208 balcony-0.1.2/balcony/custom_tf_import_configs/iam.yaml
+-rw-r--r--   0        0        0      336 2023-06-22 11:23:28.065064 balcony-0.1.2/balcony/custom_tf_import_configs/s3.yaml
+-rw-r--r--   0        0        0     3149 2023-04-15 19:49:24.900287 balcony-0.1.2/balcony/custom_yamls/_example_service.yaml
+-rw-r--r--   0        0        0      517 2023-04-06 12:50:36.974851 balcony-0.1.2/balcony/custom_yamls/ec2.yaml
+-rw-r--r--   0        0        0        0 2023-04-05 13:32:52.449913 balcony-0.1.2/balcony/custom_yamls/ecs.yaml
+-rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.1.2/balcony/custom_yamls/iam.yaml
+-rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.1.2/balcony/custom_yamls/s3.yaml
+-rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.1.2/balcony/errors.py
+-rw-r--r--   0        0        0    48806 2023-06-26 21:17:28.989726 balcony-0.1.2/balcony/nodes.py
+-rw-r--r--   0        0        0    17113 2023-05-01 12:20:53.387726 balcony-0.1.2/balcony/reader.py
+-rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.1.2/balcony/registries.py
+-rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.1.2/balcony/relations.py
+-rw-r--r--   0        0        0     1407 2023-06-25 08:18:38.934823 balcony-0.1.2/balcony/terraform_import/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 17:41:34.879852 balcony-0.1.2/balcony/terraform_import/__init__.py
+-rw-r--r--   0        0        0    12861 2023-06-26 21:33:22.666107 balcony-0.1.2/balcony/terraform_import/helper.py
+-rw-r--r--   0        0        0     6278 2023-06-26 21:38:54.628133 balcony-0.1.2/balcony/terraform_import/importer.py
+-rw-r--r--   0        0        0     1262 2023-06-23 11:28:38.779925 balcony-0.1.2/balcony/terraform_import/models.py
+-rw-r--r--   0        0        0     2613 2023-06-26 20:32:49.881902 balcony-0.1.2/balcony/terraform_import/parsers.py
+-rw-r--r--   0        0        0     2980 2023-06-19 18:24:25.368221 balcony-0.1.2/balcony/test.py
+-rw-r--r--   0        0        0     6108 2023-06-18 17:25:37.430772 balcony-0.1.2/balcony/utils.py
+-rw-r--r--   0        0        0     2130 2023-06-26 15:42:20.730332 balcony-0.1.2/balcony/yaml_config.py
+-rw-r--r--   0        0        0     2049 2023-06-18 17:05:58.939803 balcony-0.1.2/balcony/yaml_validators.py
+-rw-r--r--   0        0        0      748 2023-06-26 23:57:40.315361 balcony-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 balcony-0.1.2/setup.py
+-rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 balcony-0.1.2/PKG-INFO
```

### Comparing `balcony-0.1.1/LICENSE` & `balcony-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/README.md` & `balcony-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/__init__.py` & `balcony-0.1.2/balcony/__init__.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/aws.py` & `balcony-0.1.2/balcony/aws.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/cli.py` & `balcony-0.1.2/balcony/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 import logging
 import boto3
 from pathlib import Path
 from terraform_import.importer import (
     generate_import_block_for_resource,
     get_importable_resources,
 )
+from terraform_import.helper import (
+    interactive_help,
+)
 from rich.padding import Padding
 
 console = get_rich_console()
 logger = get_logger(__name__)
 session = _create_boto_session()
 balcony_aws = BalconyAWS(session)
 app = typer.Typer(no_args_is_help=True, pretty_exceptions_enable=False)
@@ -264,15 +267,14 @@
 
     # warn user if pagination is not set
     if not follow_pagination:
         logger.debug(
             "[underline][yellow bold][WARNING][/] [bold][--paginate, -p][/] option [bold red]is NOT set[/]. You're likely to get incomplete data.[/]"
         )
     service_markup = f"[green]{service}[/]"
-    resource_node_markup = f"[green]{service}[/].[blue]{resource_node}[/]"
 
     if not service and not resource_node:
         # print out resource nodes of this service.
         _list_service_or_resource(service, resource_node, screen_pager=screen)
         console.print(
             Panel("[bold]Please pick one of the AWS Services", title="[red][bold]ERROR")
         )
@@ -437,16 +439,14 @@
         )
         console.print(rendered_service_resource_list)
         return  # list option is enabled, do not run the actual importing code.
 
     if (not service) or (not resource_node):
         screen = False
         _list_service_or_resource(service, resource_node, screen_pager=screen)
-
-        console.print(f"{service=} {resource_node=}")
         console.print(f"[red bold]Please pick a Service and Resource Node[/]")
         return
 
     import_blocks = generate_import_block_for_resource(
         balcony_aws,
         service,
         resource_node,
@@ -484,14 +484,65 @@
 
     else:
         console.print("\n".join(import_blocks))
 
     return import_blocks
 
 
+@app.command(
+    "terraform-wizard",
+    no_args_is_help=True,
+    help="Helps you generate the correct configuration for the terraform import command.",
+)
+def wizard_the_terraform_import_configurer(
+    service: Optional[str] = typer.Argument(
+        None,
+        show_default=False,
+        help="Name of the AWS Service (e.g. ec2, s3, rds)",
+        autocompletion=_complete_service_name,
+    ),
+    resource_node: Optional[str] = typer.Argument(
+        None,
+        show_default=False,
+        help="Name of the AWS Resource Node. (e.g. Instances, Buckets, DBInstances)",
+        autocompletion=_complete_resource_node_name,
+    ),
+    debug: bool = typer.Option(False, "--debug", "-d", help="Enable debug messages."),
+    list_contents: bool = typer.Option(
+        False,
+        "--list",
+        "-l",
+        help="Show documentation about the currently selected Service and ResourceNode. Does not make requests.",
+    ),
+    screen: bool = typer.Option(
+        False, "--screen", "-s", help="Open the data on a separate paginator on shell."
+    ),
+):
+    # set debug level if enabled
+    if debug:
+        set_log_level_at_runtime(logging.DEBUG)
+
+    if list_contents:
+        _list_service_or_resource(service, resource_node, screen_pager=screen)
+        raise typer.Exit()
+
+    if (not service) or (not resource_node):
+        _list_service_or_resource(service, resource_node, screen_pager=screen)
+
+        console.print(f"[red bold]Please pick a Service and Resource Node[/]")
+        return
+    
+    
+    # if we got here, we have both service and resource node
+    
+    # call a function 
+    interactive_help(balcony_aws, service, resource_node)
+    print
+
+
 @app.command("clear-cache", help="Clear relations json cache")
 def clear_cache_command(
     # service: Optional[str] = typer.Argument(None, show_default='all',
     # help='Name of the Service to clear relation caches of', autocompletion=_complete_service_name),
 ):
     logger.debug("Deleting relations cache for services:")
     deleted_service_caches = clear_relations_cache()
```

### Comparing `balcony-0.1.1/balcony/config.py` & `balcony-0.1.2/balcony/config.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/custom_nodes/codebuild.py` & `balcony-0.1.2/balcony/custom_nodes/codebuild.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/custom_nodes/ecs.py` & `balcony-0.1.2/balcony/custom_nodes/ecs.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/custom_nodes/iam.py` & `balcony-0.1.2/balcony/custom_nodes/iam.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/custom_nodes/lambda_functions.py` & `balcony-0.1.2/balcony/custom_nodes/lambda_functions.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/custom_nodes/s3.py` & `balcony-0.1.2/balcony/custom_nodes/s3.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/custom_nodes/ses.py` & `balcony-0.1.2/balcony/custom_nodes/ses.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/custom_nodes/ssm.py` & `balcony-0.1.2/balcony/custom_nodes/ssm.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/custom_tf_import_configs/ec2.yaml` & `balcony-0.1.2/balcony/custom_tf_import_configs/ec2.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -14,7 +14,14 @@
     resource_node: Volumes
     operation_name: DescribeVolumes
     to_resource_type: aws_ebs_volume
     jmespath_query: "[].Volumes[]"
     to_resource_name_jinja2_template: "{{ VolumeId }}"
     id_generator_jinja2_template: "{{ VolumeId }}"
  
+  - id_generator_jinja2_template: '{{ VpcId }}'
+    jmespath_query: '[].Vpcs[]'
+    operation_name: DescribeVpcs
+    resource_node: Vpcs
+    service: ec2
+    to_resource_name_jinja2_template: '{{ tag_Name or VpcId }}'
+    to_resource_type: aws_vpc
```

### Comparing `balcony-0.1.1/balcony/custom_yamls/_example_service.yaml` & `balcony-0.1.2/balcony/custom_yamls/_example_service.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/custom_yamls/ec2.yaml` & `balcony-0.1.2/balcony/custom_yamls/ec2.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/custom_yamls/iam.yaml` & `balcony-0.1.2/balcony/custom_yamls/iam.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/nodes.py` & `balcony-0.1.2/balcony/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     compare_two_camel_case_words,
     str_relations,
     is_word_in_a_list_of_words,
     inform_about_develeoping_custom_resource_nodes
 )
 from botocore_utils import (
     get_input_shape,
+    annotate_shape_and_its_members_with_target_path,
     get_max_results_value_from_shape,
     find_key_in_dict_keys,
     generate_rich_tree_from_shape,
     icompare_two_camel_case_words,
     ifind_key_in_dict_keys,
     READ_ONLY_VERBS,
     IDENTIFIER_NAMES,
@@ -488,27 +489,28 @@
 
         return api_parameters_list, None
 
     def print_operation(self, operation_name: str) -> None:
         operation_panel = self._rich_operation_details_panel(operation_name)
         console.print(operation_panel)
 
-    def _rich_operation_details_panel(self, operation_name: str) -> Panel:
+    def _rich_operation_details_panel(self, operation_name: str, remove_input_shape=False, remove_documentation=False) -> Panel:
 
         operation_model = self.get_operation_model(operation_name)
         input_shape = get_input_shape(operation_model)
         output_shape = operation_model.output_shape
         input_shape_name = 'No Input Shape Found'
         input_shape_tree = Text("No Input Shape Found")
         if input_shape:
-            input_shape_tree = generate_rich_tree_from_shape(input_shape)
+            input_shape_tree = generate_rich_tree_from_shape(input_shape, remove_documentation=remove_documentation)
             input_shape_name = input_shape.name
-        output_shape_tree = generate_rich_tree_from_shape(output_shape)
+        output_shape_tree = generate_rich_tree_from_shape(output_shape, remove_documentation=remove_documentation)
 
         operation_docs = cleanhtml(operation_model.documentation)
+        
         panel_group = Group(
             Padding(f"[bold underline]Documentation:[/] {operation_docs}", (1, 2)),
             Panel(
                 input_shape_tree,
                 title=f"Input: [yellow]{input_shape_name}",
                 title_align="left",
                 padding=(1, 1),
@@ -516,14 +518,25 @@
             Panel(
                 output_shape_tree,
                 title=f"Output: [yellow]{output_shape.name}",
                 title_align="left",
                 padding=(1, 1),
             ),
         )
+        
+        if remove_input_shape:
+            panel_group = Group(
+                Padding(f"[bold underline]Documentation:[/] {operation_docs}", (1, 2)),
+                Panel(
+                    output_shape_tree,
+                    title=f"Output: [yellow]{output_shape.name}",
+                    title_align="left",
+                    padding=(1, 1),
+                ),
+            )
 
         required_parameters = self.get_required_parameter_names_from_operation_name(
             operation_name
         )
         _title = f"[bold]Operation[/]: [magenta bold]{operation_name}[/]"
         if required_parameters:
             _title = f"{_title}   [white][Required: {', '.join(required_parameters)}]"
```

### Comparing `balcony-0.1.1/balcony/reader.py` & `balcony-0.1.2/balcony/reader.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/registries.py` & `balcony-0.1.2/balcony/registries.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/relations.py` & `balcony-0.1.2/balcony/relations.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/terraform_import/README.md` & `balcony-0.1.2/balcony/terraform_import/README.md`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/terraform_import/importer.py` & `balcony-0.1.2/balcony/terraform_import/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 logger = get_logger(__name__)
 
 
 def extract_resource_tags_as_kwargs(data: dict) -> dict:
     tags_as_kwargs = {}
     tag_list = data.get("Tags", [])
-    if not tag_list:
+    if not tag_list or not isinstance(tag_list, list):
         return tags_as_kwargs
 
     for tag in tag_list:
         key = tag.get("Key")
         value = tag.get("Value")
         tags_as_kwargs[f"tag_{key}"] = value
     return tags_as_kwargs
@@ -75,23 +75,20 @@
 
         logger.debug(f"{resource_name_list=}    {import_id_list=}")
         assert len(resource_name_list) == len(import_id_list)
         return list(zip(resource_name_list, import_id_list))
 
 
 def generate_terraform_import_block(to_resource_type, to_resource_name, import_id):
-    jinja_tmpl = textwrap.dedent(
-        """
+    jinja_tmpl = textwrap.dedent("""
     import {
         to = {{ to_resource_type }}.{{ to_resource_name }}
         id = "{{ import_id }}"
     }
-    
-    """
-    ).lstrip()
+    """)
 
     jinja_env = Environment()
     template = jinja_env.from_string(jinja_tmpl)
     rendered_output = template.render(
         to_resource_type=to_resource_type,
         import_id=import_id,
         to_resource_name=to_resource_name,
```

### Comparing `balcony-0.1.1/balcony/terraform_import/models.py` & `balcony-0.1.2/balcony/terraform_import/models.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/terraform_import/parsers.py` & `balcony-0.1.2/balcony/terraform_import/parsers.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,24 @@
 from typing import Union, Tuple
 import yaml
 from collections import defaultdict
 
 logger = get_logger(__name__)
 
 
+def parse_json_to_tf_import_config(
+    input_configuration_dict: str,
+) -> Union[bool, CustomTerraformImportConfigFile]:
+    try:
+        return CustomTerraformImportConfigFile(**input_configuration_dict)
+    except Exception as e:
+        logger.debug(f"Error while parsing user defined tf import config: {str(e)}")
+    return False
+
+
 def parse_yaml_file_to_tf_import_config(
     yaml_file_path: str,
 ) -> Tuple[CustomTerraformImportConfigFile, Union[Exception, None]]:
     """Parses given YAML file and returns a pydantic model: YamlService object
 
     Args:
         yaml_file_path (str): Filepath for the yaml file
```

### Comparing `balcony-0.1.1/balcony/test.py` & `balcony-0.1.2/balcony/test.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/utils.py` & `balcony-0.1.2/balcony/utils.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/yaml_config.py` & `balcony-0.1.2/balcony/yaml_config.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/balcony/yaml_validators.py` & `balcony-0.1.2/balcony/yaml_validators.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.1/pyproject.toml` & `balcony-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "balcony"
-version = "0.1.1"
+version = "0.1.2"
 description = "Read any resource in your AWS Account. You can generate terraform code for them, too."
 authors = ["Oguzhan Yilmaz <oguzhanylmz271@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.scripts]
 balcony = "balcony.cli:run_app"
```

### Comparing `balcony-0.1.1/setup.py` & `balcony-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['balcony = balcony.cli:run_app']}
 
 setup_kwargs = {
     'name': 'balcony',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Read any resource in your AWS Account. You can generate terraform code for them, too.',
     'long_description': '# balcony\n\n\n<div style="display: flex;">\n  <a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml/badge.svg" alt="Build and publish a Docker image to ghcr.io"></a>\n  <span style="width: 5px"></span>\n\n<a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment/badge.svg" alt="Build and Deploy Documentation website"></a>\n</div>\n\n\n\nbalcony dynamically parses AWS SDK(`boto3` library) and analyzes required parameters for each operation. \n\nBy **establishing relations between operations over required parameters**, it\'s **able to auto-fill** them by reading the related operation beforehand.\n\nBy simply entering their name, balcony enables developers to easily list their AWS resources.\n\n\n## Installation & Documentation \n\n**[https://oguzhan-yilmaz.github.io/balcony/](https://oguzhan-yilmaz.github.io/balcony/quickstart)**\n\nBalcony\'s documentation website contains quickstart guide, usage cookbook and more.\n\n\n\n\n\n## Features & GIFs\n> click to play the videos\n### List Resource Nodes of an AWS Service \n`balcony aws <service-name>` to see every Resource Node of a service.\n\n![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/resource-node-list.gif)\n\n\n### Reading a Resource Node \n`balcony aws <service-name> <resource-node>` to read operations of a Resource Node.\n\n![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/reading-a-resource-node.gif)\n\n\n### Documentation and Input & Output of Operations\nUse the `--list`, `-l` flag to print the given AWS API Operations documentation, input & output structure. \n \n\n![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/list-option.gif)\n',
     'author': 'Oguzhan Yilmaz',
     'author_email': 'oguzhanylmz271@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 ['*'], 'balcony': ['custom_tf_import_configs/*', 'custom_yamls/*']}
 install_requires = \ ['Jinja2>=3.1.2,<4.0.0', 'PyYAML>=6.0,<7.0',
 'boto3>=1.24.80,<2.0.0', 'inflect>=6.0.0,<7.0.0', 'jmespath>=1.0.1,<2.0.0',
 'mkdocs-autorefs>=0.4.1,<0.5.0', 'mkdocs-material>=8.5.7,<10.0.0',
 'mkdocstrings[python]>=0.21.2,<0.22.0', 'pydantic>=1.10.7,<2.0.0',
 'rich>=13.3.4,<14.0.0', 'typer>=0.7.0,<0.8.0'] entry_points = \
 {'console_scripts': ['balcony = balcony.cli:run_app']} setup_kwargs = { 'name':
-'balcony', 'version': '0.1.1', 'description': 'Read any resource in your AWS
+'balcony', 'version': '0.1.2', 'description': 'Read any resource in your AWS
 Account. You can generate terraform code for them, too.', 'long_description':
 '# balcony\n\n\n
 \n [Build_and_publish_a_Docker_image_to_ghcr.io]\n \n\n[Build_and_Deploy
 Documentation_website]\n
 \n\n\n\nbalcony dynamically parses AWS SDK(`boto3` library) and analyzes
 required parameters for each operation. \n\nBy **establishing relations between
 operations over required parameters**, it\'s **able to auto-fill** them by
```

### Comparing `balcony-0.1.1/PKG-INFO` & `balcony-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balcony
-Version: 0.1.1
+Version: 0.1.2
 Summary: Read any resource in your AWS Account. You can generate terraform code for them, too.
 License: GPL-3.0-or-later
 Author: Oguzhan Yilmaz
 Author-email: oguzhanylmz271@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: balcony Version: 0.1.1 Summary: Read any resource
+Metadata-Version: 2.1 Name: balcony Version: 0.1.2 Summary: Read any resource
 in your AWS Account. You can generate terraform code for them, too. License:
 GPL-3.0-or-later Author: Oguzhan Yilmaz Author-email: oguzhanylmz271@gmail.com
 Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Requires-Dist: Jinja2
```

