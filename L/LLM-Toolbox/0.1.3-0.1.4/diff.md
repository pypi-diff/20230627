# Comparing `tmp/LLM-Toolbox-0.1.3.tar.gz` & `tmp/LLM-Toolbox-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LLM-Toolbox-0.1.3.tar", last modified: Tue Jun 27 03:31:51 2023, max compression
+gzip compressed data, was "LLM-Toolbox-0.1.4.tar", last modified: Tue Jun 27 04:14:12 2023, max compression
```

## Comparing `LLM-Toolbox-0.1.3.tar` & `LLM-Toolbox-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 03:31:51.350803 LLM-Toolbox-0.1.3/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 08:04:31.000000 LLM-Toolbox-0.1.3/LICENSE
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 03:31:51.350803 LLM-Toolbox-0.1.3/LLM_Toolbox.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17821 2023-06-27 03:31:51.000000 LLM-Toolbox-0.1.3/LLM_Toolbox.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      875 2023-06-27 03:31:51.000000 LLM-Toolbox-0.1.3/LLM_Toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-27 03:31:51.000000 LLM-Toolbox-0.1.3/LLM_Toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      674 2023-06-27 03:31:51.000000 LLM-Toolbox-0.1.3/LLM_Toolbox.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       88 2023-06-27 03:31:51.000000 LLM-Toolbox-0.1.3/LLM_Toolbox.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-27 03:31:51.000000 LLM-Toolbox-0.1.3/LLM_Toolbox.egg-info/top_level.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17821 2023-06-27 03:31:51.350803 LLM-Toolbox-0.1.3/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17283 2023-06-27 02:43:22.000000 LLM-Toolbox-0.1.3/README.md
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 03:31:51.350803 LLM-Toolbox-0.1.3/llm_toolbox/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.1.3/llm_toolbox/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    12595 2023-06-26 23:19:47.000000 LLM-Toolbox-0.1.3/llm_toolbox/cli.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 03:31:51.350803 LLM-Toolbox-0.1.3/llm_toolbox/tools/
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 03:31:51.350803 LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      367 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/cheermeup.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      593 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/codereview.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      853 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/commitgen.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1372 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/critique.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      269 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/define.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      331 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/explain.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      747 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/lessonize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      532 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/pathlearner.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      422 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/proofread.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      452 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/study.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      424 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/summarize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      817 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/teachlib.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      247 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/thesaurus.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      363 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/translate.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-27 03:31:51.350803 LLM-Toolbox-0.1.3/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2915 2023-06-27 03:29:25.000000 LLM-Toolbox-0.1.3/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 04:14:12.340797 LLM-Toolbox-0.1.4/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 08:04:31.000000 LLM-Toolbox-0.1.4/LICENSE
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 04:14:12.340797 LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17827 2023-06-27 04:14:12.000000 LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      875 2023-06-27 04:14:12.000000 LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-27 04:14:12.000000 LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      674 2023-06-27 04:14:12.000000 LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       88 2023-06-27 04:14:12.000000 LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-27 04:14:12.000000 LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/top_level.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17827 2023-06-27 04:14:12.340797 LLM-Toolbox-0.1.4/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    17289 2023-06-27 03:44:49.000000 LLM-Toolbox-0.1.4/README.md
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 04:14:12.340797 LLM-Toolbox-0.1.4/llm_toolbox/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.1.4/llm_toolbox/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    12595 2023-06-26 23:19:47.000000 LLM-Toolbox-0.1.4/llm_toolbox/cli.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 04:14:12.340797 LLM-Toolbox-0.1.4/llm_toolbox/tools/
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 04:14:12.340797 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      367 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/cheermeup.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      593 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/codereview.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      853 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/commitgen.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1372 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/critique.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      269 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/define.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      331 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/explain.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      747 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/lessonize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      532 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/pathlearner.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      422 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/proofread.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      452 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/study.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      411 2023-06-27 04:12:58.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/summarize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      817 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/teachlib.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      247 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/thesaurus.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      363 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/translate.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-27 04:14:12.340797 LLM-Toolbox-0.1.4/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2915 2023-06-27 04:13:39.000000 LLM-Toolbox-0.1.4/setup.py
```

### Comparing `LLM-Toolbox-0.1.3/LICENSE` & `LLM-Toolbox-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.3/LLM_Toolbox.egg-info/PKG-INFO` & `LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLM-Toolbox
-Version: 0.1.3
+Version: 0.1.4
 Summary: A versatile collection of CLI tools leveraging large language models
 Home-page: https://github.com/sderev/llm-toolbox
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/llm-toolbox
 Project-URL: Issues, http://github.com/sderev/llm-toolbox/issues
 Project-URL: Changelog, https://github.com/sderev/llm-toolbox/releases
@@ -200,15 +200,15 @@
 
 Instructions on how to use each of the tools are included in the individual directories under [tools/](https://github.com/sderev/llm-toolbox/tree/main/tools). This is also where I give some tricks and tips on their usage 💡👀💭.
 
 Note that LMT is the main tool in the LLM-Toolbox. All of its options apply to (almost) all of the other tools. For instance, you change the model to GPT-4 with `-m 4` or add emojis with `--emoji`. Refer to the [LMT's documentation](https://github.com/sderev/lmt) for more information. 
 
 * **Reading from `stdin`**: Almost all of the tools can read from `stdin`. For instance: `cat my_text.md | summarize`.
 
-* **Output Redirection**: You can use output redirections with the tools. For instance: `cat my_text.md | critique > critique_of_my_text.md`
+* **Output Redirection**: You can use output redirections with the tools. For instance: `cat my_text.md | critique --raw > critique_of_my_text.md`
 
 Here's a brief overview of the tools:
 
 ### [LMT](https://github.com/sderev/lmt)
 
 [LMT](https://github.com/sderev/lmt) empowers you to interact directly with ChatGPT from the comfort of your terminal. One of the core features of `lmt` is its ability to facilitate the creation of custom templates, enabling you to design your personalized toolbox of CLI applications. You can easily install its standalone version from [the project's repository](https://github.com/sderev/lmt).
```

### Comparing `LLM-Toolbox-0.1.3/LLM_Toolbox.egg-info/SOURCES.txt` & `LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.3/LLM_Toolbox.egg-info/entry_points.txt` & `LLM-Toolbox-0.1.4/LLM_Toolbox.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.3/PKG-INFO` & `LLM-Toolbox-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLM-Toolbox
-Version: 0.1.3
+Version: 0.1.4
 Summary: A versatile collection of CLI tools leveraging large language models
 Home-page: https://github.com/sderev/llm-toolbox
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/llm-toolbox
 Project-URL: Issues, http://github.com/sderev/llm-toolbox/issues
 Project-URL: Changelog, https://github.com/sderev/llm-toolbox/releases
@@ -200,15 +200,15 @@
 
 Instructions on how to use each of the tools are included in the individual directories under [tools/](https://github.com/sderev/llm-toolbox/tree/main/tools). This is also where I give some tricks and tips on their usage 💡👀💭.
 
 Note that LMT is the main tool in the LLM-Toolbox. All of its options apply to (almost) all of the other tools. For instance, you change the model to GPT-4 with `-m 4` or add emojis with `--emoji`. Refer to the [LMT's documentation](https://github.com/sderev/lmt) for more information. 
 
 * **Reading from `stdin`**: Almost all of the tools can read from `stdin`. For instance: `cat my_text.md | summarize`.
 
-* **Output Redirection**: You can use output redirections with the tools. For instance: `cat my_text.md | critique > critique_of_my_text.md`
+* **Output Redirection**: You can use output redirections with the tools. For instance: `cat my_text.md | critique --raw > critique_of_my_text.md`
 
 Here's a brief overview of the tools:
 
 ### [LMT](https://github.com/sderev/lmt)
 
 [LMT](https://github.com/sderev/lmt) empowers you to interact directly with ChatGPT from the comfort of your terminal. One of the core features of `lmt` is its ability to facilitate the creation of custom templates, enabling you to design your personalized toolbox of CLI applications. You can easily install its standalone version from [the project's repository](https://github.com/sderev/lmt).
```

### Comparing `LLM-Toolbox-0.1.3/README.md` & `LLM-Toolbox-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 
 Instructions on how to use each of the tools are included in the individual directories under [tools/](https://github.com/sderev/llm-toolbox/tree/main/tools). This is also where I give some tricks and tips on their usage 💡👀💭.
 
 Note that LMT is the main tool in the LLM-Toolbox. All of its options apply to (almost) all of the other tools. For instance, you change the model to GPT-4 with `-m 4` or add emojis with `--emoji`. Refer to the [LMT's documentation](https://github.com/sderev/lmt) for more information. 
 
 * **Reading from `stdin`**: Almost all of the tools can read from `stdin`. For instance: `cat my_text.md | summarize`.
 
-* **Output Redirection**: You can use output redirections with the tools. For instance: `cat my_text.md | critique > critique_of_my_text.md`
+* **Output Redirection**: You can use output redirections with the tools. For instance: `cat my_text.md | critique --raw > critique_of_my_text.md`
 
 Here's a brief overview of the tools:
 
 ### [LMT](https://github.com/sderev/lmt)
 
 [LMT](https://github.com/sderev/lmt) empowers you to interact directly with ChatGPT from the comfort of your terminal. One of the core features of `lmt` is its ability to facilitate the creation of custom templates, enabling you to design your personalized toolbox of CLI applications. You can easily install its standalone version from [the project's repository](https://github.com/sderev/lmt).
```

### Comparing `LLM-Toolbox-0.1.3/llm_toolbox/cli.py` & `LLM-Toolbox-0.1.4/llm_toolbox/cli.py`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/codereview.yaml` & `LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/codereview.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/commitgen.yaml` & `LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/commitgen.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/critique.yaml` & `LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/critique.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/lessonize.yaml` & `LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/lessonize.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/pathlearner.yaml` & `LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/pathlearner.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.3/llm_toolbox/tools/templates/teachlib.yaml` & `LLM-Toolbox-0.1.4/llm_toolbox/tools/templates/teachlib.yaml`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.1.3/setup.py` & `LLM-Toolbox-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 from pathlib import Path
 import shutil
 
-VERSION = "0.1.3"
+VERSION = "0.1.4"
 
 
 class PostDevelopCommand(develop):
     """Post-installation for development mode."""
 
     def run(self):
         develop.run(self)
```

