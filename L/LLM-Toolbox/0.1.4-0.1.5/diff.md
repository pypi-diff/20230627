# Comparing `tmp/LLM-Toolbox-0.1.4.tar.gz` & `tmp/LLM-Toolbox-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LLM-Toolbox-0.1.4.tar", last modified: Tue Jun 27 04:14:12 2023, max compression
+gzip compressed data, was "LLM-Toolbox-0.1.5.tar", last modified: Tue Jun 27 10:23:46 2023, max compression
```

## Comparing `LLM-Toolbox-0.1.4.tar` & `LLM-Toolbox-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 04:14:12.340797 LLM-Toolbox-0.1.4/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 08:04:31.000000 LLM-Toolbox-0.1.4/LICENSE
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 04:14:12.340797 LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17827 2023-06-27 04:14:12.000000 LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      875 2023-06-27 04:14:12.000000 LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-27 04:14:12.000000 LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      674 2023-06-27 04:14:12.000000 LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       88 2023-06-27 04:14:12.000000 LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-27 04:14:12.000000 LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/top_level.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17827 2023-06-27 04:14:12.340797 LLM-Toolbox-0.1.4/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17289 2023-06-27 03:44:49.000000 LLM-Toolbox-0.1.4/README.md
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 04:14:12.340797 LLM-Toolbox-0.1.4/llm_toolbox/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.1.4/llm_toolbox/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    12595 2023-06-26 23:19:47.000000 LLM-Toolbox-0.1.4/llm_toolbox/cli.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 04:14:12.340797 LLM-Toolbox-0.1.4/llm_toolbox/tools/
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 04:14:12.340797 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      367 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/cheermeup.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      593 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/codereview.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      853 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/commitgen.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1372 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/critique.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      269 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/define.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      331 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/explain.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      747 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/lessonize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      532 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/pathlearner.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      422 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/proofread.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      452 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/study.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      411 2023-06-27 04:12:58.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/summarize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      817 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/teachlib.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      247 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/thesaurus.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      363 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/translate.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-27 04:14:12.340797 LLM-Toolbox-0.1.4/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2915 2023-06-27 04:13:39.000000 LLM-Toolbox-0.1.4/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 10:23:46.730680 LLM-Toolbox-0.1.5/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 08:04:31.000000 LLM-Toolbox-0.1.5/LICENSE
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 10:23:46.730680 LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17827 2023-06-27 10:23:46.000000 LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      913 2023-06-27 10:23:46.000000 LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-27 10:23:46.000000 LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      702 2023-06-27 10:23:46.000000 LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       96 2023-06-27 10:23:46.000000 LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-27 10:23:46.000000 LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/top_level.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17827 2023-06-27 10:23:46.730680 LLM-Toolbox-0.1.5/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17289 2023-06-27 04:18:20.000000 LLM-Toolbox-0.1.5/README.md
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 10:23:46.730680 LLM-Toolbox-0.1.5/llm_toolbox/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.1.5/llm_toolbox/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    15872 2023-06-27 10:19:56.000000 LLM-Toolbox-0.1.5/llm_toolbox/cli.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 10:23:46.730680 LLM-Toolbox-0.1.5/llm_toolbox/tools/
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 10:23:46.730680 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      367 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/cheermeup.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      593 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/codereview.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      853 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/commitgen.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1372 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/critique.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      269 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/define.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      331 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/explain.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      747 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/lessonize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      818 2023-06-27 10:12:29.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/life.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      532 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/pathlearner.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      422 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/proofread.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      452 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/study.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      411 2023-06-27 04:12:58.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/summarize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      817 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/teachlib.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      247 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/thesaurus.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      363 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/translate.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-27 10:23:46.730680 LLM-Toolbox-0.1.5/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2173 2023-06-27 10:20:58.000000 LLM-Toolbox-0.1.5/setup.py
```

### Comparing `LLM-Toolbox-0.1.4/LICENSE` & `LLM-Toolbox-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/PKG-INFO` & `LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLM-Toolbox
-Version: 0.1.4
+Version: 0.1.5
 Summary: A versatile collection of CLI tools leveraging large language models
 Home-page: https://github.com/sderev/llm-toolbox
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/llm-toolbox
 Project-URL: Issues, http://github.com/sderev/llm-toolbox/issues
 Project-URL: Changelog, https://github.com/sderev/llm-toolbox/releases
@@ -328,15 +328,15 @@
 
 ___
 
 ### [Summarize](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize)
 
 The [`summarize`](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize) tool provides succinct summaries of a web page, lengthy texts, or the content of given files. It's perfect for extracting key points and crucial information from vast amounts of data, saving users time and effort.
 
-![wikipedia](https://github.com/sderev/llm-toolbox/assets/24412384/655e34aa-07d9-4f3c-97e9-36fd319126ce)
+![wikipedia](https://github.com/sderev/llm-toolbox/assets/24412384/0c1988af-d11b-40c0-bf8a-de651315beb3)
 
 ___
 
 ### [Teachlib](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib)
 
 The [`teachlib`](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib) tool is designed to provide comprehensive lessons on various libraries. By simplifying complex aspects and focusing on the core functionalities, this tool helps users to understand and effectively utilize different libraries.
```

### Comparing `LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/SOURCES.txt` & `LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 llm_toolbox/tools/templates/cheermeup.yaml
 llm_toolbox/tools/templates/codereview.yaml
 llm_toolbox/tools/templates/commitgen.yaml
 llm_toolbox/tools/templates/critique.yaml
 llm_toolbox/tools/templates/define.yaml
 llm_toolbox/tools/templates/explain.yaml
 llm_toolbox/tools/templates/lessonize.yaml
+llm_toolbox/tools/templates/life.yaml
 llm_toolbox/tools/templates/pathlearner.yaml
 llm_toolbox/tools/templates/proofread.yaml
 llm_toolbox/tools/templates/study.yaml
 llm_toolbox/tools/templates/summarize.yaml
 llm_toolbox/tools/templates/teachlib.yaml
 llm_toolbox/tools/templates/thesaurus.yaml
 llm_toolbox/tools/templates/translate.yaml
```

### Comparing `LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/entry_points.txt` & `LLM-Toolbox-0.1.5/LLM_Toolbox.egg-info/entry_points.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 cheermeup = llm_toolbox.cli:cheermeup
 codereview = llm_toolbox.cli:codereview
 commitgen = llm_toolbox.cli:commitgen
 critique = llm_toolbox.cli:critique
 define = llm_toolbox.cli:define
 explain = llm_toolbox.cli:explain
 lessonize = llm_toolbox.cli:lessonize
+life = llm_toolbox.cli:life
 llm-toolbox = llm_toolbox.cli:cli
 lmt = lmt_cli.cli:lmt
 pathlearner = llm_toolbox.cli:pathlearner
 proofread = llm_toolbox.cli:proofread
 shellgenius = shellgenius.cli:shellgenius
 study = llm_toolbox.cli:study
 summarize = llm_toolbox.cli:summarize
```

### Comparing `LLM-Toolbox-0.1.4/PKG-INFO` & `LLM-Toolbox-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLM-Toolbox
-Version: 0.1.4
+Version: 0.1.5
 Summary: A versatile collection of CLI tools leveraging large language models
 Home-page: https://github.com/sderev/llm-toolbox
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/llm-toolbox
 Project-URL: Issues, http://github.com/sderev/llm-toolbox/issues
 Project-URL: Changelog, https://github.com/sderev/llm-toolbox/releases
@@ -328,15 +328,15 @@
 
 ___
 
 ### [Summarize](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize)
 
 The [`summarize`](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize) tool provides succinct summaries of a web page, lengthy texts, or the content of given files. It's perfect for extracting key points and crucial information from vast amounts of data, saving users time and effort.
 
-![wikipedia](https://github.com/sderev/llm-toolbox/assets/24412384/655e34aa-07d9-4f3c-97e9-36fd319126ce)
+![wikipedia](https://github.com/sderev/llm-toolbox/assets/24412384/0c1988af-d11b-40c0-bf8a-de651315beb3)
 
 ___
 
 ### [Teachlib](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib)
 
 The [`teachlib`](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib) tool is designed to provide comprehensive lessons on various libraries. By simplifying complex aspects and focusing on the core functionalities, this tool helps users to understand and effectively utilize different libraries.
```

### Comparing `LLM-Toolbox-0.1.4/README.md` & `LLM-Toolbox-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -314,15 +314,15 @@
 
 ___
 
 ### [Summarize](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize)
 
 The [`summarize`](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize) tool provides succinct summaries of a web page, lengthy texts, or the content of given files. It's perfect for extracting key points and crucial information from vast amounts of data, saving users time and effort.
 
-![wikipedia](https://github.com/sderev/llm-toolbox/assets/24412384/655e34aa-07d9-4f3c-97e9-36fd319126ce)
+![wikipedia](https://github.com/sderev/llm-toolbox/assets/24412384/0c1988af-d11b-40c0-bf8a-de651315beb3)
 
 ___
 
 ### [Teachlib](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib)
 
 The [`teachlib`](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib) tool is designed to provide comprehensive lessons on various libraries. By simplifying complex aspects and focusing on the core functionalities, this tool helps users to understand and effectively utilize different libraries.
```

### Comparing `LLM-Toolbox-0.1.4/llm_toolbox/cli.py` & `LLM-Toolbox-0.1.5/llm_toolbox/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,69 @@
+import json
 import os
 import re
 import requests
+import shutil
 import subprocess
 import sys
 import tempfile
+from datetime import datetime
 from functools import wraps
 from pathlib import Path
 
 import click
 import validators
 from strip_tags.lib import strip_tags
 
 from lmt_cli.lib import *
 from lmt_cli.cli import VALID_MODELS
 
 
+def install_templates():
+    """
+    Installs the templates in the user's home directory.
+    """
+    dest_path = Path.home() / ".config/lmt/templates"
+    dest_path.mkdir(parents=True, exist_ok=True)
+
+    config_file = Path.home() / ".config/lmt/config.json"
+    config_file.touch(exist_ok=True)
+
+    # Load existing config if it exists, else start with empty dictionary
+    with config_file.open("r") as f:
+        try:
+            config = json.load(f)
+        except json.JSONDecodeError:
+            click.echo(f"{click.style('Installing templates...', fg='yellow')}")
+            config = {}
+
+    src_path = Path(__file__).parent / "tools/templates"
+    for file in src_path.glob("*.yaml"):
+        destination = dest_path / file.name
+
+        # Only copy file if it does not exist
+        if not destination.exists():
+            shutil.copy2(file, dest_path)
+
+            # Update the config file with the copied template
+            template_name = file.stem
+            config[template_name] = str(dest_path / file.name)
+            click.echo(
+                f"{click.style(f'Installed `{template_name}` template.', fg='green')}"
+            )
+
+    # Write the updated config back to the file
+    with config_file.open("w") as f:
+        json.dump(config, f, indent=4)
+    print()
+
+
+install_templates()
+
+
 def validate_model_name(ctx, param, value):
     """
     Validates the model name parameter.
     """
     model_name = value.lower()
     if model_name in VALID_MODELS:
         return VALID_MODELS[model_name]
@@ -45,14 +90,15 @@
     pass
 
 
 def common_options(f):
     """
     Common options for all commands.
     """
+
     @wraps(f)
     @click.option("--emoji", is_flag=True, help="Add emotions and emojis.")
     @click.option(
         "-m",
         "--model",
         default="gpt-3.5-turbo",
         help="The model to use for the requests.",
@@ -240,20 +286,27 @@
         tokens=tokens,
         no_stream=no_stream,
         raw=raw,
         debug=debug,
     )
 
     # Get only the content of the ChatGPT request
-    commit_message = commit_message[0].strip()
+    try:
+        commit_message = commit_message[0].strip()
+    except IndexError as error:
+        click.echo(f"{click.style('Error occurred: {error}', fg='red')}", err=True)
+        return
+    except TypeError:
+        click.echo("No commit message generated. Aborting commit.")
+        return
+
 
     # Clean `^M` characters
     commit_message = commit_message.replace("\r", "")
 
-    # click.echo(commit_message) #TODO: delete?
     click.echo("\n---\n")
 
     choice = click.prompt(
         "Do you want to use this commit message? (yes/edit/no)",
         type=str,
         default="edit",
     )
@@ -473,14 +526,68 @@
         tokens,
         no_stream,
         raw,
         debug,
     )
 
 
+@cli.command()
+@click.pass_context
+@common_options
+def life(ctx, model, emoji, temperature, tokens, no_stream, raw, debug):
+    """
+    Comment on the remaining lifespan of a person.
+    """
+    template_file = get_template_content("life")
+    user_info = template_file["user_info"]
+
+    if user_info["name"] is None:
+        user_name = click.prompt("What is your name?", type=str)
+    else:
+        user_name = user_info["name"]
+
+    if user_info["date_of_birth"] is None:
+        date_of_birth = click.prompt(
+            "What is your date of birth? (YYYY-MM-DD)", type=str
+        )
+    else:
+        date_of_birth = user_info["date_of_birth"]
+
+    life_expectancy = user_info["life_expectancy"]
+    system = template_file["system"]
+
+    # Update the template file
+    template_file["user_info"]["name"] = user_name
+    template_file["user_info"]["date_of_birth"] = date_of_birth
+    template_path = TEMPLATES_DIR / "life.yaml"
+    with open(template_path, "w") as outfile:
+        yaml.dump(template_file, outfile, default_flow_style=False)
+
+    date_of_birth = datetime.strptime(user_info["date_of_birth"], "%Y-%m-%d")
+    remaining_days = life_expectancy - (datetime.now() - date_of_birth).days
+    percentage = f"{(remaining_days / life_expectancy) * 100:.2f}"
+
+    system = f"{system}".format(
+        user_name=user_name, remaining_days=remaining_days, percentage=percentage
+    )
+
+    prepare_and_generate_response(
+        system=system,
+        template="",  # No template for this command
+        model=model,
+        emoji=True,
+        prompt_input="",
+        temperature=temperature,
+        tokens=tokens,
+        no_stream=no_stream,
+        raw=raw,
+        debug=debug,
+    )
+
+
 def process_command(
     ctx,
     template: str,
     model: str,
     emoji: bool,
     prompt_input: str,
     temperature: float,
```

### Comparing `LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/codereview.yaml` & `LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/codereview.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/commitgen.yaml` & `LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/commitgen.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/critique.yaml` & `LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/critique.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/lessonize.yaml` & `LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/lessonize.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/pathlearner.yaml` & `LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/pathlearner.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/teachlib.yaml` & `LLM-Toolbox-0.1.5/llm_toolbox/tools/templates/teachlib.yaml`

 * *Files identical despite different names*

