# Comparing `tmp/sitk-cli-0.4.0.tar.gz` & `tmp/sitk-cli-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitk-cli-0.4.0.tar", last modified: Wed Nov 23 08:28:01 2022, max compression
+gzip compressed data, was "sitk-cli-0.5.0.tar", last modified: Tue Jun 27 08:00:04 2023, max compression
```

## Comparing `sitk-cli-0.4.0.tar` & `sitk-cli-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 lloyd      (501) staff       (20)        0 2022-11-23 08:28:01.055988 sitk-cli-0.4.0/
--rw-r--r--   0 lloyd      (501) staff       (20)     1067 2022-07-02 08:52:02.000000 sitk-cli-0.4.0/LICENSE
--rw-r--r--   0 lloyd      (501) staff       (20)     1645 2022-11-23 08:28:01.056104 sitk-cli-0.4.0/PKG-INFO
--rw-r--r--   0 lloyd      (501) staff       (20)     1263 2022-11-23 08:26:42.000000 sitk-cli-0.4.0/README.md
--rw-r--r--   0 lloyd      (501) staff       (20)       82 2022-07-02 08:54:22.000000 sitk-cli-0.4.0/pyproject.toml
--rw-r--r--   0 lloyd      (501) staff       (20)      811 2022-11-23 08:28:01.056737 sitk-cli-0.4.0/setup.cfg
--rw-r--r--   0 lloyd      (501) staff       (20)       83 2022-07-03 15:27:45.000000 sitk-cli-0.4.0/setup.py
-drwxr-xr-x   0 lloyd      (501) staff       (20)        0 2022-11-23 08:28:01.050912 sitk-cli-0.4.0/src/
-drwxr-xr-x   0 lloyd      (501) staff       (20)        0 2022-11-23 08:28:01.053842 sitk-cli-0.4.0/src/sitk_cli/
--rw-r--r--   0 lloyd      (501) staff       (20)       88 2022-07-03 15:48:44.000000 sitk-cli-0.4.0/src/sitk_cli/__init__.py
--rw-r--r--   0 lloyd      (501) staff       (20)     2997 2022-11-23 08:26:42.000000 sitk-cli-0.4.0/src/sitk_cli/lib.py
-drwxr-xr-x   0 lloyd      (501) staff       (20)        0 2022-11-23 08:28:01.055729 sitk-cli-0.4.0/src/sitk_cli.egg-info/
--rw-r--r--   0 lloyd      (501) staff       (20)     1645 2022-11-23 08:28:01.000000 sitk-cli-0.4.0/src/sitk_cli.egg-info/PKG-INFO
--rw-r--r--   0 lloyd      (501) staff       (20)      275 2022-11-23 08:28:01.000000 sitk-cli-0.4.0/src/sitk_cli.egg-info/SOURCES.txt
--rw-r--r--   0 lloyd      (501) staff       (20)        1 2022-11-23 08:28:01.000000 sitk-cli-0.4.0/src/sitk_cli.egg-info/dependency_links.txt
--rw-r--r--   0 lloyd      (501) staff       (20)       43 2022-11-23 08:28:01.000000 sitk-cli-0.4.0/src/sitk_cli.egg-info/requires.txt
--rw-r--r--   0 lloyd      (501) staff       (20)        9 2022-11-23 08:28:01.000000 sitk-cli-0.4.0/src/sitk_cli.egg-info/top_level.txt
+drwxr-xr-x   0 lloyd      (501) staff       (20)        0 2023-06-27 08:00:04.075555 sitk-cli-0.5.0/
+-rw-r--r--   0 lloyd      (501) staff       (20)     1067 2023-06-27 06:39:35.000000 sitk-cli-0.5.0/LICENSE
+-rw-r--r--   0 lloyd      (501) staff       (20)     1960 2023-06-27 08:00:04.075612 sitk-cli-0.5.0/PKG-INFO
+-rw-r--r--   0 lloyd      (501) staff       (20)     1578 2023-06-27 06:39:35.000000 sitk-cli-0.5.0/README.md
+-rw-r--r--   0 lloyd      (501) staff       (20)       82 2023-06-27 06:39:35.000000 sitk-cli-0.5.0/pyproject.toml
+-rw-r--r--   0 lloyd      (501) staff       (20)      837 2023-06-27 08:00:04.075879 sitk-cli-0.5.0/setup.cfg
+-rw-r--r--   0 lloyd      (501) staff       (20)       83 2023-06-27 06:39:35.000000 sitk-cli-0.5.0/setup.py
+drwxr-xr-x   0 lloyd      (501) staff       (20)        0 2023-06-27 08:00:04.073365 sitk-cli-0.5.0/src/
+drwxr-xr-x   0 lloyd      (501) staff       (20)        0 2023-06-27 08:00:04.074479 sitk-cli-0.5.0/src/sitk_cli/
+-rw-r--r--   0 lloyd      (501) staff       (20)       88 2023-06-27 06:39:35.000000 sitk-cli-0.5.0/src/sitk_cli/__init__.py
+-rw-r--r--   0 lloyd      (501) staff       (20)     3250 2023-06-27 07:40:35.000000 sitk-cli-0.5.0/src/sitk_cli/lib.py
+drwxr-xr-x   0 lloyd      (501) staff       (20)        0 2023-06-27 08:00:04.075144 sitk-cli-0.5.0/src/sitk_cli.egg-info/
+-rw-r--r--   0 lloyd      (501) staff       (20)     1960 2023-06-27 08:00:04.000000 sitk-cli-0.5.0/src/sitk_cli.egg-info/PKG-INFO
+-rw-r--r--   0 lloyd      (501) staff       (20)      325 2023-06-27 08:00:04.000000 sitk-cli-0.5.0/src/sitk_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 lloyd      (501) staff       (20)        1 2023-06-27 08:00:04.000000 sitk-cli-0.5.0/src/sitk_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 lloyd      (501) staff       (20)       43 2023-06-27 08:00:04.000000 sitk-cli-0.5.0/src/sitk_cli.egg-info/requires.txt
+-rw-r--r--   0 lloyd      (501) staff       (20)        9 2023-06-27 08:00:04.000000 sitk-cli-0.5.0/src/sitk_cli.egg-info/top_level.txt
+drwxr-xr-x   0 lloyd      (501) staff       (20)        0 2023-06-27 08:00:04.075436 sitk-cli-0.5.0/tests/
+-rw-r--r--   0 lloyd      (501) staff       (20)     1961 2023-06-27 06:39:35.000000 sitk-cli-0.5.0/tests/test_make_cli.py
+-rw-r--r--   0 lloyd      (501) staff       (20)      697 2023-06-27 06:39:35.000000 sitk-cli-0.5.0/tests/test_register_cli.py
```

### Comparing `sitk-cli-0.4.0/LICENSE` & `sitk-cli-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sitk-cli-0.4.0/setup.cfg` & `sitk-cli-0.5.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [metadata]
 name = sitk-cli
-version = 0.4.0
+version = 0.5.0
+requires-python = ">=3.8"
 url = https://github.com/dyollb/sitk-cli
 description = Wrap SimpleITK functions as command lines
 long_description = file: README.md
 license = MIT License
 project_urls = 
 	Bug Tracker=https://github.com/dyollb/sitk-cli/issues
 	Source Code=https://github.com/dyollb/sitk-cli
```

### Comparing `sitk-cli-0.4.0/src/sitk_cli/lib.py` & `sitk-cli-0.5.0/src/sitk_cli/lib.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 from inspect import Parameter, isclass, signature
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Union, get_args, get_origin
 
 import SimpleITK as sitk
 import typer
 from makefun import wraps
 
 
 def make_cli(func, output_arg_name="output"):
     """Make command line interface from function with sitk.Image args"""
     image_args = []
     transform_args = []
 
     def _translate_param(p: Parameter):
         annotation, default = p.annotation, p.default
-        if isclass(p.annotation) and issubclass(
-            p.annotation, (sitk.Image, sitk.Transform)
-        ):
-            if issubclass(p.annotation, sitk.Image):
+
+        # handle Optional[A] and Union[A, None]
+        origin = get_origin(annotation)
+        args = get_args(annotation)
+        if origin is Union and args and not isinstance(args[0], type(None)):
+            annotation = get_args(annotation)[0]
+
+        if isclass(annotation) and issubclass(annotation, (sitk.Image, sitk.Transform)):
+            if issubclass(annotation, sitk.Image):
                 image_args.append(p.name)
             else:
                 transform_args.append(p.name)
             annotation = Path
             default = typer.Option(None) if p.default is None else typer.Option(...)
         elif p.default == Parameter.empty:
             default = typer.Option(...)
```

