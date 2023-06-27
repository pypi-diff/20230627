# Comparing `tmp/gitease-0.0.5.tar.gz` & `tmp/gitease-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitease-0.0.5.tar", last modified: Mon Jun 19 18:15:56 2023, max compression
+gzip compressed data, was "gitease-0.0.6.tar", last modified: Tue Jun 27 12:57:16 2023, max compression
```

## Comparing `gitease-0.0.5.tar` & `gitease-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,39 @@
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-19 18:15:56.403934 gitease-0.0.5/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       79 2023-06-07 11:21:02.000000 gitease-0.0.5/.gitattributes
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4118 2023-06-12 19:42:29.000000 gitease-0.0.5/.gitignore
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     3063 2023-06-19 18:15:56.403598 gitease-0.0.5/PKG-INFO
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1809 2023-06-15 11:21:54.000000 gitease-0.0.5/README.md
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-19 18:15:56.400347 gitease-0.0.5/gitease/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        2 2023-06-14 15:01:01.000000 gitease-0.0.5/gitease/__init__.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4628 2023-06-13 12:41:22.000000 gitease-0.0.5/gitease/automations.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     5385 2023-06-15 11:21:54.000000 gitease-0.0.5/gitease/cli.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     3697 2023-06-15 11:21:54.000000 gitease-0.0.5/gitease/git_helper.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     3140 2023-06-19 18:15:11.000000 gitease-0.0.5/gitease/llm_helper.py
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-19 18:15:56.402796 gitease-0.0.5/gitease/prompts/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      947 2023-06-13 08:49:13.000000 gitease-0.0.5/gitease/prompts/prompt_template.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      823 2023-06-13 08:49:13.000000 gitease-0.0.5/gitease/prompts/refine_template.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      157 2023-06-15 11:21:54.000000 gitease-0.0.5/gitease/prompts/undo_template.txt
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-19 18:15:56.401630 gitease-0.0.5/gitease.egg-info/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     3063 2023-06-19 18:15:52.000000 gitease-0.0.5/gitease.egg-info/PKG-INFO
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      481 2023-06-19 18:15:56.000000 gitease-0.0.5/gitease.egg-info/SOURCES.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        1 2023-06-19 18:15:52.000000 gitease-0.0.5/gitease.egg-info/dependency_links.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       39 2023-06-19 18:15:52.000000 gitease-0.0.5/gitease.egg-info/entry_points.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       94 2023-06-19 18:15:52.000000 gitease-0.0.5/gitease.egg-info/requires.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        8 2023-06-19 18:15:52.000000 gitease-0.0.5/gitease.egg-info/top_level.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1555 2023-06-19 18:15:11.000000 gitease-0.0.5/pyproject.toml
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       64 2023-06-12 19:37:45.000000 gitease-0.0.5/requirements.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       38 2023-06-19 18:15:56.404015 gitease-0.0.5/setup.cfg
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-19 18:15:56.403092 gitease-0.0.5/tests/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        0 2023-06-07 11:21:27.000000 gitease-0.0.5/tests/__init__.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-27 12:57:16.285625 gitease-0.0.6/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       79 2023-06-07 11:21:02.000000 gitease-0.0.6/.gitattributes
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4161 2023-06-19 19:56:47.000000 gitease-0.0.6/.gitignore
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     1068 2023-06-19 20:28:50.000000 gitease-0.0.6/LICENSE
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4564 2023-06-27 12:57:16.285250 gitease-0.0.6/PKG-INFO
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     3287 2023-06-27 12:55:55.000000 gitease-0.0.6/README.md
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-27 12:57:16.279565 gitease-0.0.6/docs/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      634 2023-06-19 19:56:47.000000 gitease-0.0.6/docs/Makefile
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     1134 2023-06-27 12:55:55.000000 gitease-0.0.6/docs/conf.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-27 12:57:16.279940 gitease-0.0.6/docs/images/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)   174135 2023-06-19 20:35:34.000000 gitease-0.0.6/docs/images/logo.png
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     2152 2023-06-27 10:53:24.000000 gitease-0.0.6/docs/index.rst
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      800 2023-06-19 19:56:47.000000 gitease-0.0.6/docs/make.bat
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-27 12:57:16.281206 gitease-0.0.6/docs/markdowns/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      260 2023-06-19 19:56:47.000000 gitease-0.0.6/docs/markdowns/quickstart.md
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     9780 2023-06-27 12:55:55.000000 gitease-0.0.6/docs/markdowns/usage.md
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       60 2023-06-19 19:56:47.000000 gitease-0.0.6/docs/requirements.txt
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-27 12:57:16.282638 gitease-0.0.6/gitease/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        2 2023-06-14 15:01:01.000000 gitease-0.0.6/gitease/__init__.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4628 2023-06-27 10:53:24.000000 gitease-0.0.6/gitease/automations.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     6250 2023-06-27 12:55:55.000000 gitease-0.0.6/gitease/cli.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4765 2023-06-27 12:55:55.000000 gitease-0.0.6/gitease/git_helper.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     3140 2023-06-19 18:15:11.000000 gitease-0.0.6/gitease/llm_helper.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-27 12:57:16.284688 gitease-0.0.6/gitease/prompts/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      947 2023-06-13 08:49:13.000000 gitease-0.0.6/gitease/prompts/prompt_template.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      823 2023-06-13 08:49:13.000000 gitease-0.0.6/gitease/prompts/refine_template.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      157 2023-06-15 11:21:54.000000 gitease-0.0.6/gitease/prompts/undo_template.txt
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-27 12:57:16.283988 gitease-0.0.6/gitease.egg-info/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4564 2023-06-27 12:57:12.000000 gitease-0.0.6/gitease.egg-info/PKG-INFO
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      641 2023-06-27 12:57:16.000000 gitease-0.0.6/gitease.egg-info/SOURCES.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        1 2023-06-27 12:57:12.000000 gitease-0.0.6/gitease.egg-info/dependency_links.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       39 2023-06-27 12:57:12.000000 gitease-0.0.6/gitease.egg-info/entry_points.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       94 2023-06-27 12:57:12.000000 gitease-0.0.6/gitease.egg-info/requires.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        8 2023-06-27 12:57:12.000000 gitease-0.0.6/gitease.egg-info/top_level.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     1555 2023-06-27 12:55:55.000000 gitease-0.0.6/pyproject.toml
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       64 2023-06-12 19:37:45.000000 gitease-0.0.6/requirements.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       38 2023-06-27 12:57:16.285698 gitease-0.0.6/setup.cfg
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-27 12:57:16.284879 gitease-0.0.6/tests/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        0 2023-06-07 11:21:27.000000 gitease-0.0.6/tests/__init__.py
```

### Comparing `gitease-0.0.5/.gitignore` & `gitease-0.0.6/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -259,8 +259,11 @@
 __pycache__/**
 **/__pycache__/**
 # Including strong name files can present a security risk
 # (https://github.com/github/gitignore/pull/2483#issue-259490424)
 /gitllm.egg-info/
 **.egg-info/**
 **/**/**.pyc
-dist/*
+dist/*
+docs/_build/*
+docs/_static
+docs/_templates
```

### Comparing `gitease-0.0.5/gitease/automations.py` & `gitease-0.0.6/gitease/automations.py`

 * *Files identical despite different names*

### Comparing `gitease-0.0.5/gitease/cli.py` & `gitease-0.0.6/gitease/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typer
 import os
-import subprocess
-from typing import List
+
+from typing import List, Union
 from rich.style import Style
 from rich.console import Console
 from rich.prompt import Prompt
 from typing_extensions import Annotated
 from gitease.git_helper import GitHelper
 from gitease.llm_helper import LanguageModel
 
@@ -22,14 +22,18 @@
 y_annotation = Annotated[bool, typer.Option("--yes", "-y", help="If True - Skips confirmation message")]
 
 
 def _join_files(files):
     return '\n'.join(files)
 
 
+def is_valid(values: Union[List[str], str, None]):
+    return values is not None and values != "" and len(values) > 0 and values[0] != ""
+
+
 def get_user_message(diff):
     if not diff:
         return None
     console.print("\nHere is the diff:\n", style=Style(color="red", blink=True, bold=True))
     diffs = diff.split("diff --git")
     for change in diffs:
         console.print("diff --git" + change, style=Style())
@@ -42,61 +46,81 @@
     console.print(f"\nYour commit message is:\n{message}\n")
     console.print("To confirm, press Enter.", style=Style(color="green"))
     console.print("Otherwise, write your own message:", style=Style(color="yellow"))
     console.print("Press CTRL+C to cancel", style=Style(color="red"))
     return Prompt.ask("Response")
 
 
+def get_message(helper: GitHelper, quiet: bool, y: bool):
+    message = None
+    diff = helper.get_diff(staged=True)
+    if diff:
+        try:
+            if OPENAI_API_KEY:
+                message = LanguageModel(verbose=not quiet).summarize(diff).lstrip()
+                # message = message + f"\n{_join_files(add)}"
+                if not y:
+                    response = confirm_message(message)
+                    if response and len(response) > 0:  # new user commit message
+                        message = response
+            else:
+                message = get_user_message(diff)
+        except KeyboardInterrupt:
+            console.print("Cancelled", style=Style(color="red", blink=True, bold=True))
+            message = None
+    return message
+
+
+def get_stage(helper: GitHelper, stage_at_end: List[str] = None):
+    staged_at_start = None
+    if is_valid(stage_at_end):  # ignore files that are not requested to be added
+        staged_at_start = helper.get_staged()
+        helper.unstage(staged_at_start)
+    else:
+        stage_at_end = helper.get_changes()
+
+    if is_valid(stage_at_end):  # might not have changes
+        helper.stage(stage_at_end)
+    return staged_at_start, stage_at_end
+
+
 @cli.command()
 def save(add: add_annotation = None,
          message: message_annotation = None,
          quiet: quiet_annotation = False,
          y: y_annotation = False):
     """
     Add and commit files to git.
     """
     helper = GitHelper(verbose=not quiet)
-    if not add:
-        add = helper._get_changes()
-    if add:
-        helper.repo.index.add(add)
-    else:
+    staged_at_start, staged_at_end = get_stage(helper, add)
+    if not is_valid(staged_at_end):
         console.print("No changes files to add", style=Style(color="red", blink=True, bold=True))
 
-    if message is None:
-        diff = helper.get_diff(staged=True)
-        if not diff:
-            console.print("No message provided, skipping commit", style=Style(color="red", blink=True, bold=True))
-            return
-        response = None
-        if OPENAI_API_KEY:
-            message = LanguageModel(verbose=not quiet).summarize(diff).lstrip()
-            message = message + f"\n{_join_files(add)}"
-            if not y:
-                response = confirm_message(message)
-            if response and len(response) > 0:  # new user commit message
-                message = response
-        else:
-            message = get_user_message(diff)
+    if not is_valid(message):
+        message = get_message(helper, quiet, y)
 
-    if message:
-        helper.repo.index.commit(message)
+    if is_valid(message):
+        helper.commit(message)
         console.print(f"Committed with message: {message}")
-    else:
-        console.print("No message provided, skipping commit", style=Style(color="red", blink=True, bold=True))
+    if is_valid(staged_at_start):  # cleanup
+        helper.unstage(add)
+        helper.stage(staged_at_start)
 
 
 @cli.command()
 def share(add: add_annotation = None,
           message: message_annotation = None,
           quiet: quiet_annotation = False,
           y: y_annotation = False):
     """Share to remote: add, commit and push to git"""
     save(add=add, message=message, quiet=quiet, y=y)
-    GitHelper().push()
+    GitHelper(verbose=not quiet).push()
+    console.print("Pushed changes to the cloud", style=Style(color="green", blink=True, bold=True))
+
 
 
 @cli.command()
 def load():
     """Pull recent updates from git"""
     GitHelper().pull()
```

### Comparing `gitease-0.0.5/gitease/git_helper.py` & `gitease-0.0.6/gitease/git_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import contextlib
 import re
+import subprocess
 from typing import List
 from pathlib import Path
 from gitease.llm_helper import LanguageModel
 import git
 import os
 import openai.error
 
@@ -54,15 +55,46 @@
     def pull(self):
         """
         Pulls the repository from the remote.
          :return: The Git pull output.
         """
         return self.repo.git.pull()
 
-    def _get_changes(self):
+    def get_staged(self):
+        """
+        Returns the staged files.
+         :return: The staged files.
+        """
+        return self.repo.git.diff('--staged', '--name-only').split('\n')
+
+    def stage(self, files: List[str] = None):
+        """
+        Stages the files.
+         :param files: The files to stage.
+        """
+        if not files:
+            return False
+        self.repo.index.add(files)
+        return True
+
+    def unstage(self, files: List[str] = None):
+        """
+        Unstages the files.
+         :param files: The files to unstage.
+        """
+        if not files:
+            return False
+        self.repo.git.restore(files, "--staged")
+        return True
+
+    def commit(self, message: str):
+        self.repo.index.commit(message)
+        return True
+
+    def get_changes(self):
         """
         Returns a list of changed files in the repository.
         :return: The list of changed files.
         """
 
         files = []
         status = self.get_status()
@@ -76,15 +108,15 @@
         """
         Adds and commits changes to the repository.
          :param files: The list of files to add and commit. If None, all changes will be added and committed.
          :param message: The commit message.
         :return: True if changes were added and committed, False otherwise.
         """
         if not files:
-            new_files, changed_files = self._get_changes()
+            new_files, changed_files = self.get_changes()
             files = new_files + changed_files
         if not files:
             print("No changes found")
             return False
 
         if message is None:
             message = self.summarize_diff(staged=True)
@@ -108,7 +140,14 @@
                 f"OPENAI_API_KEY not set - please set it in your environment variables or provide a commit message manually.")
         with contextlib.suppress(openai.error.InvalidRequestError):
             return LanguageModel(verbose=self.verbose).summarize(self.get_diff(staged=staged))
         return "Diff too long to summarize."
 
     def reflog(self):
         return self.repo.git.reflog('show')
+
+    def restore(self, files: List[str] = None):
+        if not files:
+            return False
+        command = f"(cd {self.repo.working_tree_dir} && git restore --staged {' '.join(files)})"
+        subprocess.run(command, shell=True)
+        return True
```

### Comparing `gitease-0.0.5/gitease/llm_helper.py` & `gitease-0.0.6/gitease/llm_helper.py`

 * *Files identical despite different names*

### Comparing `gitease-0.0.5/gitease/prompts/prompt_template.txt` & `gitease-0.0.6/gitease/prompts/prompt_template.txt`

 * *Files identical despite different names*

### Comparing `gitease-0.0.5/gitease/prompts/refine_template.txt` & `gitease-0.0.6/gitease/prompts/refine_template.txt`

 * *Files identical despite different names*

### Comparing `gitease-0.0.5/pyproject.toml` & `gitease-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gitease"
-version = "0.0.5"
+version = "0.0.6"
 description = "A tool to simplfy git operations"
 readme = "README.md"
 keywords = [
     "ai",
     "llm",
     "openai",
     "developer-tools",
```

