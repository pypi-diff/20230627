# Comparing `tmp/balcony-0.1.3.tar.gz` & `tmp/balcony-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balcony-0.1.3.tar", max compression
+gzip compressed data, was "balcony-0.1.4.tar", max compression
```

## Comparing `balcony-0.1.3.tar` & `balcony-0.1.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.1.3/LICENSE
--rw-r--r--   0        0        0     1890 2023-06-22 10:24:32.348247 balcony-0.1.3/README.md
--rw-r--r--   0        0        0      933 2023-04-29 21:23:00.565222 balcony-0.1.3/balcony/__init__.py
--rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.1.3/balcony/__main__.py
--rw-r--r--   0        0        0     5622 2023-04-21 19:12:44.411429 balcony-0.1.3/balcony/aws.py
--rw-r--r--   0        0        0    15169 2023-06-27 10:41:54.525900 balcony-0.1.3/balcony/botocore_utils.py
--rw-r--r--   0        0        0    21434 2023-06-27 13:09:07.624382 balcony-0.1.3/balcony/cli.py
--rw-r--r--   0        0        0     3723 2023-06-27 12:34:24.543878 balcony-0.1.3/balcony/config.py
--rw-r--r--   0        0        0      488 2023-04-29 22:03:44.770391 balcony-0.1.3/balcony/custom_nodes/__init__.py
--rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.1.3/balcony/custom_nodes/codebuild.py
--rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.1.3/balcony/custom_nodes/ecs.py
--rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.1.3/balcony/custom_nodes/iam.py
--rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.1.3/balcony/custom_nodes/lambda_functions.py
--rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.1.3/balcony/custom_nodes/s3.py
--rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.1.3/balcony/custom_nodes/ses.py
--rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.1.3/balcony/custom_nodes/ssm.py
--rw-r--r--   0        0        0        0 2023-06-18 18:05:04.079497 balcony-0.1.3/balcony/custom_tf_import_configs/_example_import_conf.yaml
--rw-r--r--   0        0        0      894 2023-06-26 21:37:52.076889 balcony-0.1.3/balcony/custom_tf_import_configs/ec2.yaml
--rw-r--r--   0        0        0      312 2023-06-27 00:04:18.331870 balcony-0.1.3/balcony/custom_tf_import_configs/ecs.yaml
--rw-r--r--   0        0        0     1079 2023-06-27 12:36:49.277772 balcony-0.1.3/balcony/custom_tf_import_configs/iam.yaml
--rw-r--r--   0        0        0      336 2023-06-22 11:23:28.065064 balcony-0.1.3/balcony/custom_tf_import_configs/s3.yaml
--rw-r--r--   0        0        0     3149 2023-04-15 19:49:24.900287 balcony-0.1.3/balcony/custom_yamls/_example_service.yaml
--rw-r--r--   0        0        0      517 2023-04-06 12:50:36.974851 balcony-0.1.3/balcony/custom_yamls/ec2.yaml
--rw-r--r--   0        0        0        0 2023-04-05 13:32:52.449913 balcony-0.1.3/balcony/custom_yamls/ecs.yaml
--rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.1.3/balcony/custom_yamls/iam.yaml
--rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.1.3/balcony/custom_yamls/s3.yaml
--rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.1.3/balcony/errors.py
--rw-r--r--   0        0        0    48806 2023-06-26 21:17:28.989726 balcony-0.1.3/balcony/nodes.py
--rw-r--r--   0        0        0    17448 2023-06-27 11:52:38.036399 balcony-0.1.3/balcony/reader.py
--rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.1.3/balcony/registries.py
--rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.1.3/balcony/relations.py
--rw-r--r--   0        0        0     1407 2023-06-25 08:18:38.934823 balcony-0.1.3/balcony/terraform_import/README.md
--rw-r--r--   0        0        0        0 2023-06-18 17:41:34.879852 balcony-0.1.3/balcony/terraform_import/__init__.py
--rw-r--r--   0        0        0     6929 2023-06-27 11:42:12.855449 balcony-0.1.3/balcony/terraform_import/importer.py
--rw-r--r--   0        0        0     1262 2023-06-23 11:28:38.779925 balcony-0.1.3/balcony/terraform_import/models.py
--rw-r--r--   0        0        0     2654 2023-06-27 11:55:46.303705 balcony-0.1.3/balcony/terraform_import/parsers.py
--rw-r--r--   0        0        0    16109 2023-06-27 11:32:20.666703 balcony-0.1.3/balcony/terraform_import/wizard.py
--rw-r--r--   0        0        0     2980 2023-06-19 18:24:25.368221 balcony-0.1.3/balcony/test.py
--rw-r--r--   0        0        0     6108 2023-06-27 10:22:17.365596 balcony-0.1.3/balcony/utils.py
--rw-r--r--   0        0        0     2171 2023-06-27 11:55:23.845723 balcony-0.1.3/balcony/yaml_config.py
--rw-r--r--   0        0        0     2049 2023-06-18 17:05:58.939803 balcony-0.1.3/balcony/yaml_validators.py
--rw-r--r--   0        0        0      748 2023-06-27 13:35:11.997682 balcony-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 balcony-0.1.3/setup.py
--rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 balcony-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1890 2023-06-22 10:24:32.348247 balcony-0.1.4/README.md
+-rw-r--r--   0        0        0      933 2023-04-29 21:23:00.565222 balcony-0.1.4/balcony/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.1.4/balcony/__main__.py
+-rw-r--r--   0        0        0     5622 2023-04-21 19:12:44.411429 balcony-0.1.4/balcony/aws.py
+-rw-r--r--   0        0        0    15169 2023-06-27 10:41:54.525900 balcony-0.1.4/balcony/botocore_utils.py
+-rw-r--r--   0        0        0    21434 2023-06-27 13:09:07.624382 balcony-0.1.4/balcony/cli.py
+-rw-r--r--   0        0        0     3723 2023-06-27 12:34:24.543878 balcony-0.1.4/balcony/config.py
+-rw-r--r--   0        0        0      488 2023-04-29 22:03:44.770391 balcony-0.1.4/balcony/custom_nodes/__init__.py
+-rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.1.4/balcony/custom_nodes/codebuild.py
+-rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.1.4/balcony/custom_nodes/ecs.py
+-rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.1.4/balcony/custom_nodes/iam.py
+-rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.1.4/balcony/custom_nodes/lambda_functions.py
+-rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.1.4/balcony/custom_nodes/s3.py
+-rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.1.4/balcony/custom_nodes/ses.py
+-rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.1.4/balcony/custom_nodes/ssm.py
+-rw-r--r--   0        0        0        0 2023-06-18 18:05:04.079497 balcony-0.1.4/balcony/custom_tf_import_configs/_example_import_conf.yaml
+-rw-r--r--   0        0        0      894 2023-06-26 21:37:52.076889 balcony-0.1.4/balcony/custom_tf_import_configs/ec2.yaml
+-rw-r--r--   0        0        0      312 2023-06-27 00:04:18.331870 balcony-0.1.4/balcony/custom_tf_import_configs/ecs.yaml
+-rw-r--r--   0        0        0     1079 2023-06-27 12:36:49.277772 balcony-0.1.4/balcony/custom_tf_import_configs/iam.yaml
+-rw-r--r--   0        0        0      336 2023-06-22 11:23:28.065064 balcony-0.1.4/balcony/custom_tf_import_configs/s3.yaml
+-rw-r--r--   0        0        0     3149 2023-04-15 19:49:24.900287 balcony-0.1.4/balcony/custom_yamls/_example_service.yaml
+-rw-r--r--   0        0        0      517 2023-04-06 12:50:36.974851 balcony-0.1.4/balcony/custom_yamls/ec2.yaml
+-rw-r--r--   0        0        0        0 2023-04-05 13:32:52.449913 balcony-0.1.4/balcony/custom_yamls/ecs.yaml
+-rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.1.4/balcony/custom_yamls/iam.yaml
+-rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.1.4/balcony/custom_yamls/s3.yaml
+-rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.1.4/balcony/errors.py
+-rw-r--r--   0        0        0    48806 2023-06-26 21:17:28.989726 balcony-0.1.4/balcony/nodes.py
+-rw-r--r--   0        0        0    17448 2023-06-27 11:52:38.036399 balcony-0.1.4/balcony/reader.py
+-rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.1.4/balcony/registries.py
+-rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.1.4/balcony/relations.py
+-rw-r--r--   0        0        0     1407 2023-06-25 08:18:38.934823 balcony-0.1.4/balcony/terraform_import/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 17:41:34.879852 balcony-0.1.4/balcony/terraform_import/__init__.py
+-rw-r--r--   0        0        0     6929 2023-06-27 11:42:12.855449 balcony-0.1.4/balcony/terraform_import/importer.py
+-rw-r--r--   0        0        0     1262 2023-06-23 11:28:38.779925 balcony-0.1.4/balcony/terraform_import/models.py
+-rw-r--r--   0        0        0     2654 2023-06-27 11:55:46.303705 balcony-0.1.4/balcony/terraform_import/parsers.py
+-rw-r--r--   0        0        0    16069 2023-06-27 13:47:03.229109 balcony-0.1.4/balcony/terraform_import/wizard.py
+-rw-r--r--   0        0        0     2980 2023-06-19 18:24:25.368221 balcony-0.1.4/balcony/test.py
+-rw-r--r--   0        0        0     6108 2023-06-27 10:22:17.365596 balcony-0.1.4/balcony/utils.py
+-rw-r--r--   0        0        0     2171 2023-06-27 11:55:23.845723 balcony-0.1.4/balcony/yaml_config.py
+-rw-r--r--   0        0        0     2049 2023-06-18 17:05:58.939803 balcony-0.1.4/balcony/yaml_validators.py
+-rw-r--r--   0        0        0      748 2023-06-27 13:48:56.118849 balcony-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 balcony-0.1.4/setup.py
+-rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 balcony-0.1.4/PKG-INFO
```

### Comparing `balcony-0.1.3/LICENSE` & `balcony-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/README.md` & `balcony-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/__init__.py` & `balcony-0.1.4/balcony/__init__.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/aws.py` & `balcony-0.1.4/balcony/aws.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/botocore_utils.py` & `balcony-0.1.4/balcony/botocore_utils.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/cli.py` & `balcony-0.1.4/balcony/cli.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/config.py` & `balcony-0.1.4/balcony/config.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/custom_nodes/codebuild.py` & `balcony-0.1.4/balcony/custom_nodes/codebuild.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/custom_nodes/ecs.py` & `balcony-0.1.4/balcony/custom_nodes/ecs.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/custom_nodes/iam.py` & `balcony-0.1.4/balcony/custom_nodes/iam.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/custom_nodes/lambda_functions.py` & `balcony-0.1.4/balcony/custom_nodes/lambda_functions.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/custom_nodes/s3.py` & `balcony-0.1.4/balcony/custom_nodes/s3.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/custom_nodes/ses.py` & `balcony-0.1.4/balcony/custom_nodes/ses.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/custom_nodes/ssm.py` & `balcony-0.1.4/balcony/custom_nodes/ssm.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/custom_tf_import_configs/ec2.yaml` & `balcony-0.1.4/balcony/custom_tf_import_configs/ec2.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/custom_tf_import_configs/iam.yaml` & `balcony-0.1.4/balcony/custom_tf_import_configs/iam.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/custom_yamls/_example_service.yaml` & `balcony-0.1.4/balcony/custom_yamls/_example_service.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/custom_yamls/ec2.yaml` & `balcony-0.1.4/balcony/custom_yamls/ec2.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/custom_yamls/iam.yaml` & `balcony-0.1.4/balcony/custom_yamls/iam.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/nodes.py` & `balcony-0.1.4/balcony/nodes.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/reader.py` & `balcony-0.1.4/balcony/reader.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/registries.py` & `balcony-0.1.4/balcony/registries.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/relations.py` & `balcony-0.1.4/balcony/relations.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/terraform_import/README.md` & `balcony-0.1.4/balcony/terraform_import/README.md`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/terraform_import/importer.py` & `balcony-0.1.4/balcony/terraform_import/importer.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/terraform_import/models.py` & `balcony-0.1.4/balcony/terraform_import/models.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/terraform_import/parsers.py` & `balcony-0.1.4/balcony/terraform_import/parsers.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/terraform_import/wizard.py` & `balcony-0.1.4/balcony/terraform_import/wizard.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,15 +304,14 @@
         )
         # wrap the input with {{ }}
         j2_tpl_resource_name = f"{{{{ {input_j2_tpl_resource_name} }}}}"
 
         # render the jinja2 template with the filtered data
         to_resource_name_list = []
         for filtered_datum in jmespath_filtered_data:
-            console.log(filtered_datum)
             _rendered_data_list = render_jinja2_template_with_data(
                 filtered_datum, j2_tpl_resource_name
             )
             to_resource_name_list.extend(_rendered_data_list)
 
         console.print(
             Panel(
```

### Comparing `balcony-0.1.3/balcony/test.py` & `balcony-0.1.4/balcony/test.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/utils.py` & `balcony-0.1.4/balcony/utils.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/yaml_config.py` & `balcony-0.1.4/balcony/yaml_config.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/balcony/yaml_validators.py` & `balcony-0.1.4/balcony/yaml_validators.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.3/setup.py` & `balcony-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['balcony = balcony.cli:run_app']}
 
 setup_kwargs = {
     'name': 'balcony',
-    'version': '0.1.3',
+    'version': '0.1.4',
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
-'balcony', 'version': '0.1.3', 'description': 'Read any resource in your AWS
+'balcony', 'version': '0.1.4', 'description': 'Read any resource in your AWS
 Account. You can generate terraform code for them, too.', 'long_description':
 '# balcony\n\n\n
 \n [Build_and_publish_a_Docker_image_to_ghcr.io]\n \n\n[Build_and_Deploy
 Documentation_website]\n
 \n\n\n\nbalcony dynamically parses AWS SDK(`boto3` library) and analyzes
 required parameters for each operation. \n\nBy **establishing relations between
 operations over required parameters**, it\'s **able to auto-fill** them by
```

### Comparing `balcony-0.1.3/PKG-INFO` & `balcony-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balcony
-Version: 0.1.3
+Version: 0.1.4
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
-Metadata-Version: 2.1 Name: balcony Version: 0.1.3 Summary: Read any resource
+Metadata-Version: 2.1 Name: balcony Version: 0.1.4 Summary: Read any resource
 in your AWS Account. You can generate terraform code for them, too. License:
 GPL-3.0-or-later Author: Oguzhan Yilmaz Author-email: oguzhanylmz271@gmail.com
 Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Requires-Dist: Jinja2
```

