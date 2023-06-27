# Comparing `tmp/magic_run_cmd-1.0.0.tar.gz` & `tmp/magic_run_cmd-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magic_run_cmd-1.0.0.tar", max compression
+gzip compressed data, was "magic_run_cmd-1.1.0.tar", max compression
```

## Comparing `magic_run_cmd-1.0.0.tar` & `magic_run_cmd-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-03-04 00:22:21.207563 magic_run_cmd-1.0.0/LICENSE
--rw-r--r--   0        0        0     1222 2023-03-04 00:51:23.777139 magic_run_cmd-1.0.0/README.md
--rw-r--r--   0        0        0      526 2023-03-04 00:54:23.797093 magic_run_cmd-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-04 00:22:21.207563 magic_run_cmd-1.0.0/run_cmd/__init__.py
--rw-r--r--   0        0        0     1382 2023-03-04 00:36:09.047361 magic_run_cmd-1.0.0/run_cmd/run_cmd.py
--rw-r--r--   0        0        0     1886 1970-01-01 00:00:00.000000 magic_run_cmd-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-27 01:34:45.831316 magic_run_cmd-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1410 2023-06-27 02:04:51.235576 magic_run_cmd-1.1.0/README.md
+-rw-r--r--   0        0        0      593 2023-06-27 02:15:46.960211 magic_run_cmd-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 01:34:45.831946 magic_run_cmd-1.1.0/run_cmd/__init__.py
+-rw-r--r--   0        0        0     1892 2023-06-27 02:13:00.809926 magic_run_cmd-1.1.0/run_cmd/run_cmd.py
+-rw-r--r--   0        0        0     2141 1970-01-01 00:00:00.000000 magic_run_cmd-1.1.0/PKG-INFO
```

### Comparing `magic_run_cmd-1.0.0/LICENSE` & `magic_run_cmd-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `magic_run_cmd-1.0.0/README.md` & `magic_run_cmd-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 ```
 poetry add run-cmd
 ```
 
 This will install this code and all of its dependencies.
 
-Usage:
+# Usage:
 
 To use this code, you can simply import the run_cmd function:
 
 ```python
 from run_cmd.run_cmd import run_cmd
 
 print(run_cmd('ls'))
@@ -41,8 +41,21 @@
 
 If an error thrown it caught, and logged before, erroring out.
 
 You can also specify whether you want the output to be returned as a list or a string:
 
 run_cmd('ls', split=True)
 
-This will output the result as a list, with each element being one line of output.
+This will output the result as a list, with each element being one line of output.
+
+# Script
+
+
+
+```python
+        script = Scripts()
+        script.cmds = """
+                        ls
+                        echo "an"
+                       """
+        script()
+```
```

### Comparing `magic_run_cmd-1.0.0/pyproject.toml` & `magic_run_cmd-1.1.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "magic-run-cmd"
-version = "1.0.0"
-description = "A simple interface to run a bash command from python. It wraps Popen, so  it's easier to run the command"
+version = "1.1.0"
+description = "A simple interface to run a bash command from python. It wraps Popen, so  it's easier to run the command. You can use Script object to write pretty bash scripts in python."
 authors = ["daniel davee <daniel.v.davee@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "run_cmd"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `magic_run_cmd-1.0.0/run_cmd/run_cmd.py` & `magic_run_cmd-1.1.0/run_cmd/run_cmd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,35 @@
 from typing import List
+from dataclasses import dataclass
 from subprocess import Popen, PIPE as l
 from pysimplelog import Logger
 from inspect import getframeinfo, currentframe
 
 logger = Logger(__name__)
 logger.set_log_file_basename('run_cmd')
 logger.set_minimum_level(logger.logLevels['info'])
 
+@dataclass
+class Script():
+    
+    '''
+        Allows you write bash scripts in python code.
+        script = Scripts()
+        script.cmds = """
+                        ls
+                        echo "an"
+                       """
+        script()
+    '''
+    cmds:str = ''
+    
+    def __call__(self):
+        commmand_list: List[str] = self.cmds.split('\n')
+        commmand_list = [cmd.strip() for cmd in commmand_list if cmd]
+        return map(run_cmd,commmand_list)
 
 def run_cmd(cmd:str, split:bool=False) -> List[str] or str:
     """
     A simple wrapper for Popon to run shell commands from python
     
     Args:
         cmd str: The comanda you want to run
```

### Comparing `magic_run_cmd-1.0.0/PKG-INFO` & `magic_run_cmd-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: magic-run-cmd
-Version: 1.0.0
-Summary: A simple interface to run a bash command from python. It wraps Popen, so  it's easier to run the command
+Version: 1.1.0
+Summary: A simple interface to run a bash command from python. It wraps Popen, so  it's easier to run the command. You can use Script object to write pretty bash scripts in python.
 License: Apache 2.0
 Author: daniel davee
 Author-email: daniel.v.davee@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -36,15 +36,15 @@
 
 ```
 poetry add run-cmd
 ```
 
 This will install this code and all of its dependencies.
 
-Usage:
+# Usage:
 
 To use this code, you can simply import the run_cmd function:
 
 ```python
 from run_cmd.run_cmd import run_cmd
 
 print(run_cmd('ls'))
@@ -59,7 +59,21 @@
 If an error thrown it caught, and logged before, erroring out.
 
 You can also specify whether you want the output to be returned as a list or a string:
 
 run_cmd('ls', split=True)
 
 This will output the result as a list, with each element being one line of output.
+
+# Script
+
+
+
+```python
+        script = Scripts()
+        script.cmds = """
+                        ls
+                        echo "an"
+                       """
+        script()
+```
+
```

