# Comparing `tmp/prophecy-build-tool-1.1.2.tar.gz` & `tmp/prophecy-build-tool-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prophecy-build-tool/prophecy-build-tool/dist/.tmp-ykce7y69/prophecy-build-tool-1.1.2.tar", last modified: Fri May 19 07:27:35 2023, max compression
+gzip compressed data, was "/home/runner/work/prophecy-build-tool/prophecy-build-tool/dist/.tmp-2mqlfswu/prophecy-build-tool-1.1.3.tar", last modified: Tue Jun 27 07:26:51 2023, max compression
```

## Comparing `prophecy-build-tool-1.1.2.tar` & `prophecy-build-tool-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 07:22:56.000000 prophecy-build-tool-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-19 07:22:56.000000 prophecy-build-tool-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-19 07:22:56.000000 prophecy-build-tool-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-19 07:22:56.000000 prophecy-build-tool-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/src/pbt/
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-19 07:22:56.000000 prophecy-build-tool-1.1.2/src/pbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-19 07:22:56.000000 prophecy-build-tool-1.1.2/src/pbt/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    38325 2023-05-19 07:22:56.000000 prophecy-build-tool-1.1.2/src/pbt/prophecy_build_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/src/prophecy_build_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/src/prophecy_build_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/src/prophecy_build_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/src/prophecy_build_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/src/prophecy_build_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/src/prophecy_build_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/src/prophecy_build_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 07:27:35.000000 prophecy-build-tool-1.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-19 07:22:56.000000 prophecy-build-tool-1.1.2/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-19 07:22:56.000000 prophecy-build-tool-1.1.2/test/test_deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 07:21:52.000000 prophecy-build-tool-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-06-27 07:21:52.000000 prophecy-build-tool-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-27 07:21:52.000000 prophecy-build-tool-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-27 07:21:52.000000 prophecy-build-tool-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/src/pbt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-27 07:21:52.000000 prophecy-build-tool-1.1.3/src/pbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-27 07:21:52.000000 prophecy-build-tool-1.1.3/src/pbt/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39198 2023-06-27 07:21:52.000000 prophecy-build-tool-1.1.3/src/pbt/prophecy_build_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/src/prophecy_build_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/src/prophecy_build_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/src/prophecy_build_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/src/prophecy_build_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/src/prophecy_build_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/src/prophecy_build_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/src/prophecy_build_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-27 07:21:52.000000 prophecy-build-tool-1.1.3/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-06-27 07:21:52.000000 prophecy-build-tool-1.1.3/test/test_deploy.py
```

### Comparing `prophecy-build-tool-1.1.2/LICENSE` & `prophecy-build-tool-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.2/PKG-INFO` & `prophecy-build-tool-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophecy-build-tool
-Version: 1.1.2
+Version: 1.1.3
 Summary: Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the Prophecy IDE.
 Home-page: https://github.com/SimpleDataLabsInc/prophecy-build-tool
 Author: Prophecy
 Author-email: maciej@prophecy.io
 Project-URL: Bug Tracker, https://github.com/SimpleDataLabsInc/prophecy-build-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prophecy-build-tool-1.1.2/README.md` & `prophecy-build-tool-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.2/setup.py` & `prophecy-build-tool-1.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as _in:
     long_description = _in.read()
 
 setuptools.setup(
     name="prophecy-build-tool",
-    version="1.1.2",
+    version="1.1.3",
     author="Prophecy",
     author_email="maciej@prophecy.io",
     description="Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the "
     "Prophecy IDE.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SimpleDataLabsInc/prophecy-build-tool",
```

### Comparing `prophecy-build-tool-1.1.2/src/pbt/__init__.py` & `prophecy-build-tool-1.1.3/src/pbt/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,17 +31,24 @@
 
 @cli.command()
 @click.option(
     "--path",
     help="Path to the directory containing the pbt_project.yml file",
     required=True,
 )
-def validate(path):
+@click.option(
+    "--treat-warnings-as-errors",
+    help="Specifies whether to treat warnings as errors.",
+    is_flag=True,
+    required=False,
+    default=False
+)
+def validate(path, treat_warnings_as_errors):
     pbt = ProphecyBuildTool(path)
-    pbt.validate()
+    pbt.validate(treat_warnings_as_errors)
 
 
 @cli.command()
 @click.option(
     "--path",
     help="Path to the directory containing the pbt_project.yml file",
     required=True,
```

### Comparing `prophecy-build-tool-1.1.2/src/pbt/process.py` & `prophecy-build-tool-1.1.3/src/pbt/process.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.2/src/pbt/prophecy_build_tool.py` & `prophecy-build-tool-1.1.3/src/pbt/prophecy_build_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,32 +129,45 @@
             == 0
         ):
             return "python", "pip"
         else:
             print("ERROR: python not found")
             sys.exit(1)
 
-    def validate(self):
+    def validate(self, treat_warnings_as_errors: bool):
         pipelines = self.pipelines
         print("\n[bold blue]Validating %s pipelines [/bold blue]" % len(pipelines))
         overall_validate_status = True
         for pipeline_i, (path_pipeline, pipeline) in enumerate(pipelines.items()):
             print("\n  Validating pipeline %s [%s/%s]" % (path_pipeline, pipeline_i + 1, len(pipelines)))
 
             workflow_json_path_pipeline_absolute = os.path.join(
                 os.path.join(self.path_root, path_pipeline),
                 "code",
                 ".prophecy",
                 "workflow.latest.json",
             )
             if os.path.exists(workflow_json_path_pipeline_absolute):
                 workflow = json.load(open(workflow_json_path_pipeline_absolute, "r"))
+                num_errors = 0
+                num_warnings = 0
                 if "diagnostics" in workflow:
-                    print(f"\n[bold red]Pipeline is Broken: {pipeline['name']}[/bold red]")
-                    overall_validate_status = False
+                    diagnostics = workflow["diagnostics"]
+                    for diagnostic in diagnostics:
+                        if diagnostic.get('severity') == 1:
+                            print(f"\n[red]\[error] {pipeline['name']}: {diagnostic.get('message')}[/red]")
+                            num_errors += 1
+                        elif diagnostic.get('severity') == 2:
+                            print(
+                                f"\n[yellow]\[warn] {pipeline['name']}: {diagnostic.get('message')}[/yellow]")
+                            num_warnings += 1
+                    print(f"\n{pipeline['name']} has {num_errors} errors and {num_warnings} warnings.")
+                    if num_errors > 0 or (treat_warnings_as_errors and num_warnings > 0):
+                        print(f"\n[bold red]Pipeline is Broken: {pipeline['name']}[/bold red]")
+                        overall_validate_status = False
                 else:
                     print(f"\n[bold blue] Pipeline is validated: {pipeline['name']}[/bold blue]")
             else:
                 print(f"\n[bold red] Empty Pipeline Found: {pipeline['name']}![/bold red]")
                 overall_validate_status = False
 
         if not overall_validate_status:
```

### Comparing `prophecy-build-tool-1.1.2/src/prophecy_build_tool.egg-info/PKG-INFO` & `prophecy-build-tool-1.1.3/src/prophecy_build_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophecy-build-tool
-Version: 1.1.2
+Version: 1.1.3
 Summary: Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the Prophecy IDE.
 Home-page: https://github.com/SimpleDataLabsInc/prophecy-build-tool
 Author: Prophecy
 Author-email: maciej@prophecy.io
 Project-URL: Bug Tracker, https://github.com/SimpleDataLabsInc/prophecy-build-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prophecy-build-tool-1.1.2/test/test_build.py` & `prophecy-build-tool-1.1.3/test/test_build.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.2/test/test_deploy.py` & `prophecy-build-tool-1.1.3/test/test_deploy.py`

 * *Files identical despite different names*

