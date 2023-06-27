# Comparing `tmp/refyre-0.0.1.4.tar.gz` & `tmp/refyre-0.0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refyre-0.0.1.4.tar", max compression
+gzip compressed data, was "refyre-0.0.1.5.tar", max compression
```

## Comparing `refyre-0.0.1.4.tar` & `refyre-0.0.1.5.tar`

### file list

```diff
@@ -1,34 +1,37 @@
--rw-r--r--   0        0        0    10009 2023-06-21 07:52:11.161686 refyre-0.0.1.4/README.md
--rw-r--r--   0        0        0      922 2023-06-21 07:52:11.161686 refyre-0.0.1.4/pyproject.toml
--rw-r--r--   0        0        0    23166 2023-06-21 07:52:11.161686 refyre-0.0.1.4/refyre/Refyre.py
--rw-r--r--   0        0        0      135 2023-06-21 07:52:11.161686 refyre-0.0.1.4/refyre/__init__.py
--rw-r--r--   0        0        0     1056 2023-06-21 07:52:11.161686 refyre-0.0.1.4/refyre/cli.py
--rw-r--r--   0        0        0     3427 2023-06-21 07:52:11.161686 refyre-0.0.1.4/refyre/cluster/Broadcast.py
--rw-r--r--   0        0        0    18513 2023-06-21 07:52:11.161686 refyre-0.0.1.4/refyre/cluster/Cluster.py
--rw-r--r--   0        0        0      718 2023-06-21 07:52:11.161686 refyre-0.0.1.4/refyre/cluster/FileClusterIterator.py
--rw-r--r--   0        0        0      164 2023-06-21 07:52:11.161686 refyre-0.0.1.4/refyre/cluster/__init__.py
--rw-r--r--   0        0        0     3637 2023-06-21 07:52:11.161686 refyre-0.0.1.4/refyre/cluster/cogs/VariableAction.py
--rw-r--r--   0        0        0     2767 2023-06-21 07:52:11.161686 refyre-0.0.1.4/refyre/cluster/cogs/VariableParser.py
--rw-r--r--   0        0        0       23 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/config/__init__.py
--rw-r--r--   0        0        0      355 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/config/log.py
--rw-r--r--   0        0        0      499 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/core/AliasManager.py
--rw-r--r--   0        0        0      375 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/core/CodeManager.py
--rw-r--r--   0        0        0     3882 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/core/RecipePreprocessor.py
--rw-r--r--   0        0        0      126 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/core/__init__.py
--rw-r--r--   0        0        0     1658 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/datastack/DataStack.py
--rw-r--r--   0        0        0       34 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/datastack/__init__.py
--rw-r--r--   0        0        0      802 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/graph/FileGraph.py
--rw-r--r--   0        0        0     2051 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/graph/FileGraphNode.py
--rw-r--r--   0        0        0       73 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/graph/__init__.py
--rw-r--r--   0        0        0     2262 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/reader/ExpressionGenerator.py
--rw-r--r--   0        0        0     6066 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/reader/Lexer.py
--rw-r--r--   0        0        0     3287 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/reader/Parser.py
--rw-r--r--   0        0        0     2662 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/reader/PatternGenerator.py
--rw-r--r--   0        0        0      221 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/reader/__init__.py
--rw-r--r--   0        0        0      799 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/reader/cogs/LexerToken.py
--rw-r--r--   0        0        0      618 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/reader/cogs/lexer_utils.py
--rw-r--r--   0        0        0      153 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/utils/__init__.py
--rw-r--r--   0        0        0      667 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/utils/clone.py
--rw-r--r--   0        0        0      453 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/utils/optional_imports.py
--rw-r--r--   0        0        0      903 2023-06-21 07:52:11.165686 refyre-0.0.1.4/refyre/utils/regex.py
--rw-r--r--   0        0        0    10868 1970-01-01 00:00:00.000000 refyre-0.0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    10130 2023-06-27 17:47:06.677770 refyre-0.0.1.5/README.md
+-rw-r--r--   0        0        0      922 2023-06-27 17:47:06.677770 refyre-0.0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    23589 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/Refyre.py
+-rw-r--r--   0        0        0      135 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/__init__.py
+-rw-r--r--   0        0        0     1056 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/cli.py
+-rw-r--r--   0        0        0     3731 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/cluster/Association.py
+-rw-r--r--   0        0        0     3825 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/cluster/Broadcast.py
+-rw-r--r--   0        0        0     2281 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/cluster/Cache.py
+-rw-r--r--   0        0        0    20495 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/cluster/Cluster.py
+-rw-r--r--   0        0        0      718 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/cluster/ClusterIterator.py
+-rw-r--r--   0        0        0      237 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/cluster/__init__.py
+-rw-r--r--   0        0        0     3714 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/cluster/cogs/VariableAction.py
+-rw-r--r--   0        0        0     2767 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/cluster/cogs/VariableParser.py
+-rw-r--r--   0        0        0       23 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/config/__init__.py
+-rw-r--r--   0        0        0      355 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/config/log.py
+-rw-r--r--   0        0        0      499 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/core/AliasManager.py
+-rw-r--r--   0        0        0      375 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/core/CodeManager.py
+-rw-r--r--   0        0        0     3882 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/core/RecipePreprocessor.py
+-rw-r--r--   0        0        0      126 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/core/__init__.py
+-rw-r--r--   0        0        0     1597 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/datastack/DataStack.py
+-rw-r--r--   0        0        0      347 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/datastack/TorchStack.py
+-rw-r--r--   0        0        0       34 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/datastack/__init__.py
+-rw-r--r--   0        0        0      802 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/graph/FileGraph.py
+-rw-r--r--   0        0        0     2051 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/graph/FileGraphNode.py
+-rw-r--r--   0        0        0       73 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/graph/__init__.py
+-rw-r--r--   0        0        0     2375 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/reader/ExpressionGenerator.py
+-rw-r--r--   0        0        0     6066 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/reader/Lexer.py
+-rw-r--r--   0        0        0     3287 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/reader/Parser.py
+-rw-r--r--   0        0        0     3492 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/reader/PatternGenerator.py
+-rw-r--r--   0        0        0      221 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/reader/__init__.py
+-rw-r--r--   0        0        0      799 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/reader/cogs/LexerToken.py
+-rw-r--r--   0        0        0      618 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/reader/cogs/lexer_utils.py
+-rw-r--r--   0        0        0      153 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/utils/__init__.py
+-rw-r--r--   0        0        0      667 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/utils/clone.py
+-rw-r--r--   0        0        0      453 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/utils/optional_imports.py
+-rw-r--r--   0        0        0      903 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/utils/regex.py
+-rw-r--r--   0        0        0    10989 1970-01-01 00:00:00.000000 refyre-0.0.1.5/PKG-INFO
```

### Comparing `refyre-0.0.1.4/README.md` & `refyre-0.0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Refyre: Filesystem dominance is all you need
+[![PyPI Version](https://img.shields.io/pypi/v/refyre.svg)](https://pypi.python.org/pypi/refyre)
 ___ 
 
 Refyre is an AI-fused Python package that provides two high level features:
 - Easy large scale filesystem manipulations
 - Efficient, code-less directory structuring and restructuring
 
 Enhance your favorite Python packages such as Pandas, NumPy, Spark, and other data manipulation tools to quickly structure scattered data.
@@ -34,15 +35,15 @@
         d2.txt
         ...
 
 You seek to analyze the a files and the c files
 '''
 [dir="a"|name="a_var"]
 [dir="b"]
-    [dir="c"|pattern="gc?.txt"|name="c_var"] #Glob patterns start with 'g', regex with 'r', no need for just normal pattern matching
+    [dir="c"|pattern="g!c?.txt"|name="c_var"] #Glob patterns start with 'g!', regex with 'r!', no need for just normal pattern matching
 ```
 
 Have refyre analyze the directory with the following:
 ```python
 #Main analysis line
 ref = Refyre(input_specs = ['sample_input_spec.txt'])
 
@@ -116,16 +117,16 @@
 Specs, as shown above are a Pythonic way for you to feed information to refyre. Each [] represents a *cluster*, which usually has a dir attribute specified. Attributes are seperated using the '|' seperator. 
 
 As shown above, Pythonic comments can be used in a similar fashion to Python. Back to the various attributes:
 
 - **dir**: Specifies the directory the cluster is targeting. *Usually, the clusters are relative paths*.
     - You can specify the three pattern types to target multiple directories
 - **pattern**: Allows you to target specific files by specifying a template pattern. Currently, glob, regex, and "generator expressions" are supported.
-  - For glob patterns, add a 'g' before the pattern; ex: `g*.txt`
-  - For regex patterns, add an 'r' before the pattern ex: `r.txt`
+  - For glob patterns, add a 'g!' before the pattern; ex: `g!*.txt`
+  - For regex patterns, add an 'r!' before the pattern ex: `r!.txt`
   - Generator expressions a simplified pattern matching, that's more humanly controllable
     - Just one template matching --> `$` matches to a number
     - refyre supports generator expressions the most out of the three
 
 - **name**: The workhorse of specs. Arguably the **meat** of the spec. Assigns all the values to a variable specified by **name**. *Only single variable / cluster are supported*
     - You can achieve 'appending' by specifying a `+` before the name
 - **flags**: A grab bag of various tricks you can use. You can specify as many as you want, and they work together to bring out cool cluster behaviours
@@ -212,18 +213,17 @@
 from refyre.datastack import PandasStack
 from PIL import Image
 import pandas as pd
 
 ref = Refyre(input_specs = ['specs/in.txt'])
 
 #We will do some pandas visualizations on the input data
-stack = PandasStack([ref["images"]])
+stack = PandasStack(AssociationCluster(input_vars = [ref["images"]]))
 
-def processor(tup):
-    fp = tup[0]
+def processor(fp):
     print('processing', fp)
     im = Image.open(fp).convert('RGB')
     width, height = im.size 
 
     ar, ag, ab = 0.0, 0.0, 0.0
     for i in range(width):
         for j in range(height):
@@ -232,8 +232,8 @@
         
     ar, ag, ab = ar / (width * height), ag / (width * height), ab / (width * height)
     return (fp.name, width, height, ar, ag, ab)
 
 df = stack.create_dataframe(['image_name', 'image_width', 'image_height', 'average_red', 'average_green', 'average_blue'], processor)
 ```
 
-As you can see, the majority of the work here comes from building a *processor* method to convert each row of variables into a DataFrame row.
+As you can see, the majority of the work here comes from building a *processor* method to convert each row of variables into a DataFrame row.
```

### Comparing `refyre-0.0.1.4/pyproject.toml` & `refyre-0.0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "refyre"
-version = "0.0.1.4"
+version = "0.0.1.5"
 description = "Filesystem dominance is all you need."
 authors = ["Ansh <teamnebulaco@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/flockfysh/refyre"
 license = "MIT"
 keywords = ["files", "manipulation", "data science", ]
 packages = [
```

### Comparing `refyre-0.0.1.4/refyre/Refyre.py` & `refyre-0.0.1.5/refyre/Refyre.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,19 +102,19 @@
             This method enables a single cluster to target multiple directories
         '''
         if not node:
             return [None]
 
         new_path = Path(node.directory) if node.is_root_dir() else Path(path) / node.directory
 
-        assert Path(path).exists(), f"Error, the path {path} doesn't exist"
+        #assert Path(path).exists(), f"Error, the path {path} doesn't exist"
         logger.debug(f'new path: {new_path} {node.directory} {node.pattern}')
         
         if (Path(path).is_file()) or (not new_path.exists() and not PatternGenerator.is_valid_regex(node.directory)):
-            logger.debug('invalid in general')
+            logger.debug(f'invalid in general {Path(path)} {new_path} {not new_path.exists() and not PatternGenerator.is_valid_regex(node.directory)}')
             return [None]
         
 
         #Handle limits 
         has_limit, lower, upper = False, 0, 1000000000
         if node.limit != '':
             has_limit = True
@@ -203,15 +203,15 @@
 
                     ret.append(new_node)
 
             
             #Before we go to children, let's handle any imports we must
             import_fgraph = None
             if node.imports != '' and Path(node.imports).exists():
-                import_fgraph = self.__construct(node.imports, expand_path = new_path)
+                _, import_fgraph = self.__construct(node.imports, expand_path = new_path)
                 import_fgraph.is_root = False
 
             #Now, attempt to check for all the node children of the original node
             #We will insert each of the current node's children into the new matched nodes, and recurse on them
             logger.debug(f'ret {ret}')
 
             for i, pattern_node in enumerate(ret):
@@ -350,14 +350,15 @@
             By default, this method performs an in-place generation of the file spec. In other words, no directories will be deleted, and it'll try to create 
             any folders that are missing.
 
             However, if you want the directory structure in the area to look exactly as mentioned in the output spec (no other dirs), you can specify the flag *c 
             using the flags attribute.
         '''
         #Updating the path
+        logger.debug(f'in output')
         new_path = Path(node.directory) if node.is_root_dir() else Path(path) / node.directory
 
         logger.debug(f'mode {node.mode}')
         self.__create_output(node, new_path, mode if node.mode == '' else node.mode)
         new_path = new_path.as_posix()
 
         for child in node.children:
@@ -387,16 +388,18 @@
 
         I expect this method to blow up as this codebase grows (it's an options methods, and you never can have enough options!), 
         so once this goes over 100 lines, we'll move
         it into the fgraph directory.
         '''
 
         if mode == "normal":
-            name, v = VariableAction(node.name, node, path, self.variables, self.out_temp_var_dict,  True, False, mode = mode)
-            logger.debug(f'updated vals {name} {v}')
+            for v_name in node.name.split(','):
+                logger.debug(f'NAME {v_name}')
+                name, v = VariableAction(v_name, node, path, self.variables, self.out_temp_var_dict,  True, False, mode = mode)
+                logger.debug(f'updated vals {name} {v}')
 
     def __create_output(self, node, path, mode):
         '''
         Parses all the options in the "names" attribute.
 
         I expect this method to blow up as this codebase grows (it's an options methods, and you never can have enough options!), 
         so once this goes over 100 lines, we'll move
@@ -404,19 +407,23 @@
 
         mode = "copy" - During output generation, the files are copied over from their original directories 
         mode = "cut"  - During output generation, the files are cut over from their original directories
 
         '''
 
         #First of all, let's do the work we need to do 
+        logger.debug(f'Creating, {path}')
         path.mkdir(parents = True, exist_ok = True)        
+        logger.debug(path.exists())
 
         if node.name != "":
-            name, v = VariableAction(node.name, node, path, self.variables, self.out_temp_var_dict , False, True, mode = mode)
-            logger.debug(f'updated vals {name} {v}')
+            for v_name in node.name.split(','):
+                logger.debug(f'NAME {v_name}')
+                name, v = VariableAction(v_name, node, path, self.variables, self.out_temp_var_dict , False, True, mode = mode)
+                logger.debug(f'updated vals {name} {v}')
 
             
     def __post_generate(self, node, path = "", mode = "copy", flags = ""):
         '''
         Performs any post generation cleanup. For example, it handles the *d flag, which deletes anything
         irrelevant. We do this here to give a chance for any variable data to have been used / moved elsewhere.
         '''
@@ -575,15 +582,15 @@
 
             for p in self.variables[var_name]:
                 pths[var_name].append(p.as_posix())
             
         save_pth = Path(save_dir) / "refyre_state.json"
         with open(save_pth.as_posix(), 'w') as f:
             json.dump(pths, f, indent = 4)
-    
+     
     def load(load_filename):
 
         with open(load_filename, 'r') as f:
             pths = json.load(f)
 
             variables = {}
```

### Comparing `refyre-0.0.1.4/refyre/cli.py` & `refyre-0.0.1.5/refyre/cli.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.4/refyre/cluster/Broadcast.py` & `refyre-0.0.1.5/refyre/cluster/Broadcast.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
         fdct[k] = set()
     
     fdct[k].add(v)
 
 class Broadcaster:
 
     files_dict = {}
+    ignore_list = []
 
     def __init__(self, *a, **kw):
         self.conf_args = a 
         self.conf_kw   = kw
     
     @classmethod
     def clear(cls):
@@ -28,27 +29,41 @@
     @classmethod
     def release(cls, cluster_id):
         logger.debug(f'released {cluster_id}')
         for k in cls.files_dict:
             logger.debug(f'{k}, {cluster_id}, {cls.files_dict[k]}')
             cls.files_dict[k].discard(cluster_id)
 
+        if cluster_id in cls.ignore_list:
+            cls.ignore_list.remove(cluster_id)
+
+    @classmethod
+    def unlink(cls, cluster_id):
+        if cluster_id not in cls.ignore_list:
+            cls.ignore_list.append(cluster_id)
+        
 
     def __call__(self, func):
         
         def wrapper(instance, *args, **kwargs):
             '''
                 change_arr: List[Tuple(Str, Str)]
                     - Lists the Str that the path started out as, and what it became. 
                     - If second tuple None, it implies a path was deleted
 
             '''
-            instance.values = [v for v in list(dict.fromkeys(instance.values)) if v.exists() ]
+
+            if instance.id not in self.ignore_list:
+                instance.values = [v for v in list(dict.fromkeys(instance.values)) if v.exists() ]
+
             change_arr, out = func(instance, *args, **kwargs)
 
+            if instance.id in self.ignore_list:
+                return out
+
 
             logger.debug(f"CHANGE {change_arr}")
             logger.debug(out)
 
             clusters = instance.all_clusters()
 
             logger.debug(self.files_dict)
@@ -88,8 +103,8 @@
             Broadcaster.files_dict = self.files_dict
 
             instance.values = [v for v in list(dict.fromkeys(instance.values)) if v.exists() ]
             logger.debug(f"RETURNED {instance.values} {self.files_dict} {Broadcaster.files_dict}")
 
             return out
             
-        return wrapper
+        return wrapper
```

### Comparing `refyre-0.0.1.4/refyre/cluster/Cluster.py` & `refyre-0.0.1.5/refyre/cluster/Cluster.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from refyre.reader import PatternGenerator
 import re
 
 #Copying / Deleting
 import shutil
 
 #Iteration
-from .FileClusterIterator import FileClusterIterator
+from .ClusterIterator import FileClusterIterator
 from .Broadcast import Broadcaster
+from .Cache import AutoCache
 
 #Copy
 import copy
 
 #Zip
 import zipfile
 
@@ -67,24 +68,28 @@
         #ID the variable
         self.id = FileCluster.GLOBAL_COUNTER
         FileCluster.GLOBAL_COUNTER += 1
 
         #Track the cluster without affecting garbage collection
         self.weak_ref = weakref.ref(self)
         FileCluster.clusters[self.id] = self.weak_ref
+
+        #Setup a cache dir
+        self.cache_dir = '.refyre_cache'
     
         #If the user didn't send the values as Pathlib objects already
         if not as_pathlib: 
             self.values += [ Path(pth) for pth in values ]
         else:
             self.values += values
 
         self.values = sorted(self.values)
         #Track variable on broadcaster
         Broadcaster.add(self.id, self.values)
+
     def all_clusters(self):
         return FileCluster.clusters
 
     def __del__(self):
         logger.debug(f'deleting {self.id}')
         if self.id in FileCluster.clusters:
             FileCluster.clusters.pop(self.id)
@@ -469,20 +474,89 @@
         """
         The function returns a deep clone of the current object.
         :return: A deep clone of the current object is being returned.
         """
 
         return self.__deepcopy__()
 
+    def decompress(self, complete = False):
+        """
+        Takes any folders within the values, and replaces them with all the items in the folder
+
+        If complete is set to True, then it will recursively empty all files 
+        """
+        nvals = []
+        for pth in self.values:
+            if pth.is_dir():
+                nvals.extend([*pth.iterdir()] if not complete else [*pth.rglob('**/*')])
+            elif pth.is_file():
+                nvals.append(pth)
+        
+        return FileCluster(values = nvals, as_pathlib = True)
+            
+    def cache(self):
+        """
+        Saves all the files to cache
+        """
+
+        ca = AutoCache(self.cache_dir)
+        return ca.cache(self)
+    
+    def decache(self):
+        ca = AutoCache(self.cache_dir)
+        return ca.decache(self)
+    
+    def cached(self):
+        """
+        Returns all the FileCluster files in the cluster that are currently cached
+        """
+        nvals = []
+        ca = AutoCache(self.cache_dir)
+
+        for v in self.values:
+            if ca.contains(str(v)):
+                nvals.append(v)
+            
+        return FileCluster(values = nvals, as_pathlib = True)
+    
+    def unlink(self):
+        """
+        Returns a FileCluster detached from the Broadcaster system
+        """
+
+        f = self.clone()
+        Broadcaster.unlink(f.id)
+        return f
+    
+    def relink(self):
+        """
+        Reconnect the FileCluster to the broadcaster
+        """
+        return self.clone()
+
     def filesize(self, format = "bytes"):
         """
         Returns the total file size, in bytes 
         """
         total_size = 0.0
 
         for pth in self.values:
             if pth.is_dir():
                 total_size += sum([p.stat().st_size for p in Path(pth).rglob('*')])
             elif pth.is_file():
                 total_size += pth.stat().st_size
 
-        return total_size
+        return total_size
+
+    def filecount(self):
+        """
+        Returns the total number of files over all folders
+        """
+        total_files = 0
+
+        for pth in self.values:
+            if pth.is_dir():
+                total_files += len([p.stat().st_size for p in Path(pth).rglob('*')])
+            elif pth.is_file():
+                total_files += 1
+        
+        return total_files
```

### Comparing `refyre-0.0.1.4/refyre/cluster/FileClusterIterator.py` & `refyre-0.0.1.5/refyre/cluster/ClusterIterator.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.4/refyre/cluster/cogs/VariableAction.py` & `refyre-0.0.1.5/refyre/cluster/cogs/VariableAction.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,31 +10,32 @@
     and provides an interface for the rest of the code to read & write 
     to variables
 
     Together, with the VariableParser, this class assembles "intent" that can 
     be used in specs.
     '''
 
-    def __new__(self, expression, node, path, variable_dict, out_variable_dict , is_read, is_write, mode = ""):
+    def __new__(self, var_name , node, path, variable_dict, out_variable_dict , is_read, is_write, mode = ""):
         '''
         Reads in all parameters, and returns the name of the updated 
         variable
 
         Ironically, the is_read and is_write are defined in opposite.
 
         is_read refers to whether we are trying to read a value into the variable (which really just means "write"), but
         I'm keeping the naming this way since we're mostly doing the writing in specs focused on reading
 
         Similarly, is_write is for output specs
         '''
 
+        logger.debug(mode)
         #Currently, this operator pattern supports only + and "" (appending and defining)
         options_pattern = r'^(\+)?(.*)$' 
 
-        match = re.match(options_pattern, node.name)
+        match = re.match(options_pattern, var_name)
         operator = match.group(1) or ""
         name = match.group(2)
 
         #If the operator is "", a read command is sought
         '''
         Each of these commands have dual meanings - 
 
@@ -70,14 +71,15 @@
                 out_variable_dict[name] = (p if name not in out_variable_dict else out_variable_dict[name] + p)
 
 
             return name, out_variable_dict[name] 
         
         if is_write:
 
+            logger.debug(f'{name} {variable_dict}')
             name, sliced, start, stop, step = VariableParser(name, variable_dict)
 
             #The refresher method will eliminate the invalid paths, so let's add back in the new paths at their original positions
             v = list(variable_dict[name].vals())
 
             if mode == "copy":
                 sliced = sliced.copy(path)
```

### Comparing `refyre-0.0.1.4/refyre/cluster/cogs/VariableParser.py` & `refyre-0.0.1.5/refyre/cluster/cogs/VariableParser.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.4/refyre/core/RecipePreprocessor.py` & `refyre-0.0.1.5/refyre/core/RecipePreprocessor.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.4/refyre/datastack/DataStack.py` & `refyre-0.0.1.5/refyre/datastack/DataStack.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,33 +5,32 @@
     import pandas as pd
     import matplotlib.pyplot as plt
 
 # The PandasStack class is a Python class that creates a Pandas dataframe from a list of variables
 # using a mapper function.
 class PandasStack:
 
-    def __init__(self, variables_array):
-        self.variables_array = variables_array
+    def __init__(self, association):
+        self.association = association 
     
     def create_dataframe(self, col_names, mapper_func):
         '''
             col_names: List[String] An array of the names of the columns of the dataframe
             mapper_func: A function that takes in input of a tuple (var1_output, var2_output, ...), and returns a tuple with values for each of the columns
                 - Note each tuple value should be the value for the corresponding columns (i.e the ith col_name should be associated with the ith tuple val)
         '''
 
-        vals = [ v.vals() for v in self.variables_array]
         out_dct = {}
 
         for n in col_names:
             out_dct[n] = []
 
-        for input_tuple in zip(*vals):
+        for input_tuple in self.association:
 
-            output_data = mapper_func(input_tuple)
+            output_data = mapper_func(*input_tuple)
             assert len(output_data) == len(col_names), "The data length and number of columns specified through the column names don't match up!"
 
             for i in range(len(col_names)):
                 out_dct[col_names[i]].append(output_data[i])
 
         return pd.DataFrame.from_dict(out_dct)
```

### Comparing `refyre-0.0.1.4/refyre/graph/FileGraph.py` & `refyre-0.0.1.5/refyre/graph/FileGraph.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.4/refyre/graph/FileGraphNode.py` & `refyre-0.0.1.5/refyre/graph/FileGraphNode.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.4/refyre/reader/ExpressionGenerator.py` & `refyre-0.0.1.5/refyre/reader/ExpressionGenerator.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,17 @@
     def generate_expression(string):
         # Replace '$' with '{}' to use it as a placeholder for string formatting
         lambda_function = lambda i: string.replace('$', str(i))
 
         return lambda_function
     
     def is_valid_genexp(expression):
-        pattern = r'^[a-zA-Z0-9\-_$]+$'
+        pattern = r'^[a-zA-Z0-9/\-_$]+$'
+        logger.debug(f'Pattern: {pattern}')
+        logger.debug(f'Ret: {bool(re.match(pattern, expression))}')
         return bool(re.match(pattern, expression))
     
     def is_null_generator(expression):
         '''
             By "null" generator, I just mean a genexp that 
             doesn't have any special characters, i.e. one that will stay the same
         '''
```

### Comparing `refyre-0.0.1.4/refyre/reader/Lexer.py` & `refyre-0.0.1.5/refyre/reader/Lexer.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.4/refyre/reader/Parser.py` & `refyre-0.0.1.5/refyre/reader/Parser.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.4/refyre/reader/PatternGenerator.py` & `refyre-0.0.1.5/refyre/reader/PatternGenerator.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,65 +14,83 @@
         matching does come in handy. 
 
         A glob string will come in the normal form. A regex string will start with an r before the actual pattern.
 
         ex: "a?.txt" is a glob pattern. "ra?.txt" is regex.
 
     '''
+    REGEX_STARTER = 'r!'
+    GLOB_STARTER = 'g!'
+
     def is_valid_regex(pattern_string):
         logger.debug(pattern_string)
-        if pattern_string.startswith('r'):
+        if pattern_string.startswith(PatternGenerator.REGEX_STARTER):
             try:
-                re.compile(pattern_string[1:])
+                re.compile(pattern_string[2:])
             except re.error as e:
                 logger.error(e)
                 return False
-        elif pattern_string.startswith('g'):
+        elif pattern_string.startswith(PatternGenerator.GLOB_STARTER):
             try:
-                re.compile(fnmatch.translate(pattern_string[1:]))
+                re.compile(fnmatch.translate(pattern_string[2:]))
             except re.error as e:
                 logger.error(e)
                 return False
         else:
             if not PatternGenerator.is_valid_genexp(pattern_string):
+                logger.debug('not a valid')
                 return False
         return True
 
     def is_valid_genexp(expression):
         return ExpressionGenerator.is_valid_genexp(expression)
     
     def convert_generator_expression(expression):
         return ExpressionGenerator.convert_generator_expression(expression)
 
     def get_pattern_type(pattern_string):
-        if pattern_string.startswith('r'):
+        if pattern_string.startswith(PatternGenerator.REGEX_STARTER):
             return "regex"
 
-        if pattern_string.startswith('g'):
+        if pattern_string.startswith(PatternGenerator.GLOB_STARTER):
             return "glob"
         
         #Handle generator expressions
         if not ExpressionGenerator.is_null_generator(pattern_string):
+            logger.debug('here, we think it is a expgen')
             return "generator_expression"
 
         #Else, the string is a normal string
         return "normal_string" 
 
-    def __new__(self, pattern_string):
+    def __new__(self, pattern_string, given_type = None):
         '''
             Takes in an input pattern string and returns the appropriate regex pattern.
 
         '''
-        if pattern_string.startswith('r'):
+        if given_type == 'regex' or given_type == 'r':
+            return pattern_string
+
+        if given_type == 'glob' or given_type == 'g':
+            return fnmatch.translate(pattern_string)
+
+        if given_type == 'expression_generator' or given_type == 'e':
+            return ExpressionGenerator.convert_generator_expression(pattern_string)
+        
+        if given_type == 'normal' or given_type == 'n':
+            return None 
+
+        #If the type isn't given, we'll have to infer it
+        if pattern_string.startswith(PatternGenerator.REGEX_STARTER):
             logger.debug('regex')
-            return pattern_string[1:]
+            return pattern_string[2:]
 
-        if pattern_string.startswith('g'):
+        if pattern_string.startswith(PatternGenerator.GLOB_STARTER):
             logger.debug('glob')
-            return fnmatch.translate(pattern_string[1:])
+            return fnmatch.translate(pattern_string[2:])
         
         #Handle generator expressions
         if not ExpressionGenerator.is_null_generator(pattern_string):
             return ExpressionGenerator.convert_generator_expression(pattern_string)
 
         #Else, the string is a normal string
         return pattern_string
```

### Comparing `refyre-0.0.1.4/refyre/reader/cogs/LexerToken.py` & `refyre-0.0.1.5/refyre/reader/cogs/LexerToken.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.4/refyre/reader/cogs/lexer_utils.py` & `refyre-0.0.1.5/refyre/reader/cogs/lexer_utils.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.4/refyre/utils/clone.py` & `refyre-0.0.1.5/refyre/utils/clone.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.4/refyre/utils/regex.py` & `refyre-0.0.1.5/refyre/utils/regex.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.4/PKG-INFO` & `refyre-0.0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refyre
-Version: 0.0.1.4
+Version: 0.0.1.5
 Summary: Filesystem dominance is all you need.
 Home-page: https://github.com/flockfysh/refyre
 License: MIT
 Keywords: files,manipulation,data science
 Author: Ansh
 Author-email: teamnebulaco@gmail.com
 Requires-Python: >=3.8
@@ -19,14 +19,15 @@
 Requires-Dist: pandas (>=2.0.0)
 Requires-Dist: requests (>=2.29.0)
 Requires-Dist: tqdm (>=4.64.0)
 Project-URL: Repository, https://github.com/flockfysh/refyre
 Description-Content-Type: text/markdown
 
 # Refyre: Filesystem dominance is all you need
+[![PyPI Version](https://img.shields.io/pypi/v/refyre.svg)](https://pypi.python.org/pypi/refyre)
 ___ 
 
 Refyre is an AI-fused Python package that provides two high level features:
 - Easy large scale filesystem manipulations
 - Efficient, code-less directory structuring and restructuring
 
 Enhance your favorite Python packages such as Pandas, NumPy, Spark, and other data manipulation tools to quickly structure scattered data.
@@ -58,15 +59,15 @@
         d2.txt
         ...
 
 You seek to analyze the a files and the c files
 '''
 [dir="a"|name="a_var"]
 [dir="b"]
-    [dir="c"|pattern="gc?.txt"|name="c_var"] #Glob patterns start with 'g', regex with 'r', no need for just normal pattern matching
+    [dir="c"|pattern="g!c?.txt"|name="c_var"] #Glob patterns start with 'g!', regex with 'r!', no need for just normal pattern matching
 ```
 
 Have refyre analyze the directory with the following:
 ```python
 #Main analysis line
 ref = Refyre(input_specs = ['sample_input_spec.txt'])
 
@@ -140,16 +141,16 @@
 Specs, as shown above are a Pythonic way for you to feed information to refyre. Each [] represents a *cluster*, which usually has a dir attribute specified. Attributes are seperated using the '|' seperator. 
 
 As shown above, Pythonic comments can be used in a similar fashion to Python. Back to the various attributes:
 
 - **dir**: Specifies the directory the cluster is targeting. *Usually, the clusters are relative paths*.
     - You can specify the three pattern types to target multiple directories
 - **pattern**: Allows you to target specific files by specifying a template pattern. Currently, glob, regex, and "generator expressions" are supported.
-  - For glob patterns, add a 'g' before the pattern; ex: `g*.txt`
-  - For regex patterns, add an 'r' before the pattern ex: `r.txt`
+  - For glob patterns, add a 'g!' before the pattern; ex: `g!*.txt`
+  - For regex patterns, add an 'r!' before the pattern ex: `r!.txt`
   - Generator expressions a simplified pattern matching, that's more humanly controllable
     - Just one template matching --> `$` matches to a number
     - refyre supports generator expressions the most out of the three
 
 - **name**: The workhorse of specs. Arguably the **meat** of the spec. Assigns all the values to a variable specified by **name**. *Only single variable / cluster are supported*
     - You can achieve 'appending' by specifying a `+` before the name
 - **flags**: A grab bag of various tricks you can use. You can specify as many as you want, and they work together to bring out cool cluster behaviours
@@ -236,18 +237,17 @@
 from refyre.datastack import PandasStack
 from PIL import Image
 import pandas as pd
 
 ref = Refyre(input_specs = ['specs/in.txt'])
 
 #We will do some pandas visualizations on the input data
-stack = PandasStack([ref["images"]])
+stack = PandasStack(AssociationCluster(input_vars = [ref["images"]]))
 
-def processor(tup):
-    fp = tup[0]
+def processor(fp):
     print('processing', fp)
     im = Image.open(fp).convert('RGB')
     width, height = im.size 
 
     ar, ag, ab = 0.0, 0.0, 0.0
     for i in range(width):
         for j in range(height):
@@ -257,7 +257,8 @@
     ar, ag, ab = ar / (width * height), ag / (width * height), ab / (width * height)
     return (fp.name, width, height, ar, ag, ab)
 
 df = stack.create_dataframe(['image_name', 'image_width', 'image_height', 'average_red', 'average_green', 'average_blue'], processor)
 ```
 
 As you can see, the majority of the work here comes from building a *processor* method to convert each row of variables into a DataFrame row.
+
```

