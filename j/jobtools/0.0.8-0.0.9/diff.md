# Comparing `tmp/jobtools-0.0.8.tar.gz` & `tmp/jobtools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobtools-0.0.8.tar", last modified: Mon Feb 14 00:58:57 2022, max compression
+gzip compressed data, was "jobtools-0.0.9.tar", last modified: Tue Feb 22 15:30:13 2022, max compression
```

## Comparing `jobtools-0.0.8.tar` & `jobtools-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 00:58:57.305023 jobtools-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-02-14 00:58:44.000000 jobtools-0.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     5484 2022-02-14 00:58:57.305023 jobtools-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5025 2022-02-14 00:58:44.000000 jobtools-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-14 00:58:57.305023 jobtools-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-02-14 00:58:44.000000 jobtools-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 00:58:57.301022 jobtools-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 00:58:57.301022 jobtools-0.0.8/src/jobtools/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-02-14 00:58:44.000000 jobtools-0.0.8/src/jobtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      872 2022-02-14 00:58:44.000000 jobtools-0.0.8/src/jobtools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7700 2022-02-14 00:58:44.000000 jobtools-0.0.8/src/jobtools/arguments.py
--rw-r--r--   0 runner    (1001) docker     (121)     2051 2022-02-14 00:58:44.000000 jobtools-0.0.8/src/jobtools/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 00:58:57.305023 jobtools-0.0.8/src/jobtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5484 2022-02-14 00:58:57.000000 jobtools-0.0.8/src/jobtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-02-14 00:58:57.000000 jobtools-0.0.8/src/jobtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-14 00:58:57.000000 jobtools-0.0.8/src/jobtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-02-14 00:58:57.000000 jobtools-0.0.8/src/jobtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-02-14 00:58:57.000000 jobtools-0.0.8/src/jobtools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 00:58:57.301022 jobtools-0.0.8/src/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-02-14 00:58:44.000000 jobtools-0.0.8/src/scripts/jobtools
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-02-14 00:58:44.000000 jobtools-0.0.8/src/scripts/pyrunit
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 15:30:13.627427 jobtools-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-02-22 15:29:59.000000 jobtools-0.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)     5484 2022-02-22 15:30:13.627427 jobtools-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5025 2022-02-22 15:29:59.000000 jobtools-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-22 15:30:13.627427 jobtools-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      894 2022-02-22 15:29:59.000000 jobtools-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 15:30:13.623427 jobtools-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 15:30:13.623427 jobtools-0.0.9/src/jobtools/
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-02-22 15:29:59.000000 jobtools-0.0.9/src/jobtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      872 2022-02-22 15:29:59.000000 jobtools-0.0.9/src/jobtools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8733 2022-02-22 15:29:59.000000 jobtools-0.0.9/src/jobtools/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2051 2022-02-22 15:29:59.000000 jobtools-0.0.9/src/jobtools/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 15:30:13.627427 jobtools-0.0.9/src/jobtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5484 2022-02-22 15:30:13.000000 jobtools-0.0.9/src/jobtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2022-02-22 15:30:13.000000 jobtools-0.0.9/src/jobtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-22 15:30:13.000000 jobtools-0.0.9/src/jobtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-02-22 15:30:13.000000 jobtools-0.0.9/src/jobtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-02-22 15:30:13.000000 jobtools-0.0.9/src/jobtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 15:30:13.623427 jobtools-0.0.9/src/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-02-22 15:29:59.000000 jobtools-0.0.9/src/scripts/jobtools
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-02-22 15:29:59.000000 jobtools-0.0.9/src/scripts/pyrunit
```

### Comparing `jobtools-0.0.8/LICENSE.md` & `jobtools-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jobtools-0.0.8/PKG-INFO` & `jobtools-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobtools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Facilitates the use of Python from the command line
 Home-page: https://github.com/santiagxf/jobtools
 Author: Facundo Santiago
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jobtools-0.0.8/README.md` & `jobtools-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `jobtools-0.0.8/setup.py` & `jobtools-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jobtools",
-    version="0.0.8",
+    version="0.0.9",
     author="Facundo Santiago",
     description="Facilitates the use of Python from the command line",
     url = 'https://github.com/santiagxf/jobtools',
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `jobtools-0.0.8/src/jobtools/__main__.py` & `jobtools-0.0.9/src/jobtools/__main__.py`

 * *Files identical despite different names*

### Comparing `jobtools-0.0.8/src/jobtools/arguments.py` & `jobtools-0.0.9/src/jobtools/arguments.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,32 @@
 import json
 import yaml
 
 class StringEnum(Enum):
     def __str__(self):
         return str(self.value)
 
+def delimited2list(delimited: str, delimiter: str = ',') -> List[str]:
+    """
+    Parses a delimited list encoded as string to a list of string
+
+    Parameters
+    ----------
+    delimited : str
+        The argument containing string values delimited by comma.
+    delimiter: str
+        The delimiter
+
+    Returns
+    -------
+    List[str]
+        Parsed output
+    """
+    return [item.strip() for item in delimited.split(delimiter)]
+
 def file2namespace(config_file_path: str) -> SimpleNamespace:
     """
     Loads a `YAML` or `JSON` file containing representing configuration and parses
     it as a `SimpleNamespace` object.
 
     Parameters
     ----------
@@ -87,36 +105,46 @@
         parser.add_argument(extra_arg, type=str, )
 
     required_args_idxs = len(args_annotations) - len(fullargs.defaults if fullargs.defaults else [])
     for idx, (arg, arg_type) in enumerate(args_annotations.items()):
         is_required = idx < required_args_idxs
         assigned_parser = required_parser if is_required else parser
         argument_flag = f"--{arg.replace('_','-')}"
-
-        if issubclass(arg_type, SimpleNamespace):
-            if not is_required:
-                raise ValueError("An argument of type SimpleNamespace can't be optional.\
-                     Remove default values.")
-            assigned_parser.add_argument(argument_flag,
-                                dest=arg,
-                                type=file2namespace,
-                                required=is_required,
-                                help='indicated as a YAML or JSON file')
-        elif issubclass(arg_type, Enum):
-            assigned_parser.add_argument(argument_flag,
-                                dest=arg,
-                                type=arg_type,
-                                choices=list(arg_type),
-                                required=is_required)
+        if isinstance(arg_type, type):
+            if issubclass(arg_type, SimpleNamespace):
+                if not is_required:
+                    raise ValueError("An argument of type SimpleNamespace can't be optional.\
+                        Remove default values.")
+                assigned_parser.add_argument(argument_flag,
+                                    dest=arg,
+                                    type=file2namespace,
+                                    required=is_required,
+                                    help='indicated as a YAML or JSON file')
+            elif issubclass(arg_type, Enum):
+                assigned_parser.add_argument(argument_flag,
+                                    dest=arg,
+                                    type=arg_type,
+                                    choices=list(arg_type),
+                                    required=is_required)
+            else:
+                assigned_parser.add_argument(argument_flag,
+                                    dest=arg,
+                                    type=arg_type,
+                                    required=is_required,
+                                    help=f"of type {arg_type.__name__}")
         else:
-            assigned_parser.add_argument(argument_flag,
-                                dest=arg,
-                                type=arg_type,
-                                required=is_required,
-                                help=f"of type {arg_type.__name__}")
+            if arg_type._name == 'List':
+                assigned_parser.add_argument(argument_flag,
+                                    dest=arg,
+                                    type=delimited2list,
+                                    required=is_required,
+                                    help=f"indicated as a comma separted string")
+            else:
+                raise TypeError(f'Type {arg_type} is not supported in this version of jobtools')
+
 
     return parser
 
 def get_args_from_signature(method: Callable, extra_arguments: List[str] = []) -> Dict[str, Any]:
     """
     Automatically parses all the arguments to match an specific method. The method should
     implement type hinting in order for this to work. All arguments required by the method
```

### Comparing `jobtools-0.0.8/src/jobtools/runner.py` & `jobtools-0.0.9/src/jobtools/runner.py`

 * *Files identical despite different names*

### Comparing `jobtools-0.0.8/src/jobtools.egg-info/PKG-INFO` & `jobtools-0.0.9/src/jobtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobtools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Facilitates the use of Python from the command line
 Home-page: https://github.com/santiagxf/jobtools
 Author: Facundo Santiago
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

