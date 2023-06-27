# Comparing `tmp/ai2_kit-0.3.5.tar.gz` & `tmp/ai2_kit-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai2_kit-0.3.5.tar", max compression
+gzip compressed data, was "ai2_kit-0.3.6.tar", max compression
```

## Comparing `ai2_kit-0.3.5.tar` & `ai2_kit-0.3.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.3.5/LICENSE
--rw-r--r--   0        0        0     1627 2023-06-27 03:30:12.011023 ai2_kit-0.3.5/README.md
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.5/ai2_kit/__init__.py
--rw-r--r--   0        0        0        0 2023-06-25 01:09:08.600393 ai2_kit-0.3.5/ai2_kit/algorithm/__init__.py
--rw-r--r--   0        0        0    12100 2023-06-25 01:09:08.600393 ai2_kit-0.3.5/ai2_kit/algorithm/proton_transfer.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.5/ai2_kit/core/__init__.py
--rw-r--r--   0        0        0     1854 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/core/artifact.py
--rw-r--r--   0        0        0     5465 2023-06-25 01:09:08.600393 ai2_kit-0.3.5/ai2_kit/core/checkpoint.py
--rw-r--r--   0        0        0      169 2023-06-25 01:09:08.600393 ai2_kit-0.3.5/ai2_kit/core/cmd.py
--rw-r--r--   0        0        0     5766 2023-02-06 09:01:27.000000 ai2_kit-0.3.5/ai2_kit/core/connector.py
--rw-r--r--   0        0        0     7939 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/core/executor.py
--rw-r--r--   0        0        0      365 2023-06-25 01:09:08.600393 ai2_kit-0.3.5/ai2_kit/core/future.py
--rw-r--r--   0        0        0     1852 2023-06-25 01:09:08.600393 ai2_kit-0.3.5/ai2_kit/core/job.py
--rw-r--r--   0        0        0      298 2023-06-25 01:09:08.610393 ai2_kit-0.3.5/ai2_kit/core/log.py
--rw-r--r--   0        0        0     9449 2023-06-25 01:09:08.610393 ai2_kit-0.3.5/ai2_kit/core/queue_system.py
--rw-r--r--   0        0        0     2572 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/core/resource_manager.py
--rw-r--r--   0        0        0     2358 2023-06-19 08:54:25.567391 ai2_kit-0.3.5/ai2_kit/core/script.py
--rw-r--r--   0        0        0     3604 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/core/util.py
--rw-r--r--   0        0        0        0 2023-06-25 01:09:08.610393 ai2_kit-0.3.5/ai2_kit/dflow/__init__.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.5/ai2_kit/domain/__init__.py
--rw-r--r--   0        0        0     1734 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/domain/cll.py
--rw-r--r--   0        0        0      341 2023-02-27 08:58:57.520622 ai2_kit-0.3.5/ai2_kit/domain/constant.py
--rw-r--r--   0        0        0     8210 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/domain/cp2k.py
--rw-r--r--   0        0        0     4356 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/domain/data_helper.py
--rw-r--r--   0        0        0     6679 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/domain/deepmd.py
--rw-r--r--   0        0        0    16845 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/domain/lammps.py
--rw-r--r--   0        0        0     3039 2023-06-26 06:22:57.018618 ai2_kit-0.3.5/ai2_kit/domain/selector.py
--rw-r--r--   0        0        0      183 2023-03-22 04:23:44.538179 ai2_kit-0.3.5/ai2_kit/domain/updater.py
--rw-r--r--   0        0        0     1588 2023-06-25 01:09:08.610393 ai2_kit-0.3.5/ai2_kit/main.py
--rw-r--r--   0        0        0        0 2023-06-25 01:09:08.610393 ai2_kit-0.3.5/ai2_kit/tool/__init__.py
--rw-r--r--   0        0        0      676 2023-06-25 01:09:08.610393 ai2_kit-0.3.5/ai2_kit/tool/ase.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.5/ai2_kit/workflow/__init__.py
--rw-r--r--   0        0        0     8161 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/workflow/cll_mlp.py
--rw-r--r--   0        0        0     9117 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/workflow/fep_mlp.py
--rw-r--r--   0        0        0      843 2023-06-27 03:28:50.521034 ai2_kit-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 ai2_kit-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.3.6/LICENSE
+-rw-r--r--   0        0        0     1627 2023-06-27 03:30:12.011023 ai2_kit-0.3.6/README.md
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.6/ai2_kit/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-25 01:09:08.600393 ai2_kit-0.3.6/ai2_kit/algorithm/__init__.py
+-rw-r--r--   0        0        0    12100 2023-06-25 01:09:08.600393 ai2_kit-0.3.6/ai2_kit/algorithm/proton_transfer.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.6/ai2_kit/core/__init__.py
+-rw-r--r--   0        0        0     1854 2023-06-27 03:26:30.711049 ai2_kit-0.3.6/ai2_kit/core/artifact.py
+-rw-r--r--   0        0        0     5465 2023-06-25 01:09:08.600393 ai2_kit-0.3.6/ai2_kit/core/checkpoint.py
+-rw-r--r--   0        0        0      169 2023-06-25 01:09:08.600393 ai2_kit-0.3.6/ai2_kit/core/cmd.py
+-rw-r--r--   0        0        0     5766 2023-02-06 09:01:27.000000 ai2_kit-0.3.6/ai2_kit/core/connector.py
+-rw-r--r--   0        0        0     7939 2023-06-27 03:26:30.711049 ai2_kit-0.3.6/ai2_kit/core/executor.py
+-rw-r--r--   0        0        0      365 2023-06-25 01:09:08.600393 ai2_kit-0.3.6/ai2_kit/core/future.py
+-rw-r--r--   0        0        0     1852 2023-06-25 01:09:08.600393 ai2_kit-0.3.6/ai2_kit/core/job.py
+-rw-r--r--   0        0        0      298 2023-06-25 01:09:08.610393 ai2_kit-0.3.6/ai2_kit/core/log.py
+-rw-r--r--   0        0        0     9449 2023-06-25 01:09:08.610393 ai2_kit-0.3.6/ai2_kit/core/queue_system.py
+-rw-r--r--   0        0        0     2572 2023-06-27 03:26:30.711049 ai2_kit-0.3.6/ai2_kit/core/resource_manager.py
+-rw-r--r--   0        0        0     2358 2023-06-19 08:54:25.567391 ai2_kit-0.3.6/ai2_kit/core/script.py
+-rw-r--r--   0        0        0     4195 2023-06-27 09:15:51.228409 ai2_kit-0.3.6/ai2_kit/core/util.py
+-rw-r--r--   0        0        0        0 2023-06-25 01:09:08.610393 ai2_kit-0.3.6/ai2_kit/dflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.6/ai2_kit/domain/__init__.py
+-rw-r--r--   0        0        0     1734 2023-06-27 03:26:30.711049 ai2_kit-0.3.6/ai2_kit/domain/cll.py
+-rw-r--r--   0        0        0      341 2023-02-27 08:58:57.520622 ai2_kit-0.3.6/ai2_kit/domain/constant.py
+-rw-r--r--   0        0        0     8210 2023-06-27 03:26:30.711049 ai2_kit-0.3.6/ai2_kit/domain/cp2k.py
+-rw-r--r--   0        0        0     4356 2023-06-27 03:26:30.711049 ai2_kit-0.3.6/ai2_kit/domain/data_helper.py
+-rw-r--r--   0        0        0     6679 2023-06-27 03:26:30.711049 ai2_kit-0.3.6/ai2_kit/domain/deepmd.py
+-rw-r--r--   0        0        0    16845 2023-06-27 03:26:30.711049 ai2_kit-0.3.6/ai2_kit/domain/lammps.py
+-rw-r--r--   0        0        0     3039 2023-06-26 06:22:57.018618 ai2_kit-0.3.6/ai2_kit/domain/selector.py
+-rw-r--r--   0        0        0      183 2023-03-22 04:23:44.538179 ai2_kit-0.3.6/ai2_kit/domain/updater.py
+-rw-r--r--   0        0        0     1588 2023-06-25 01:09:08.610393 ai2_kit-0.3.6/ai2_kit/main.py
+-rw-r--r--   0        0        0        0 2023-06-25 01:09:08.610393 ai2_kit-0.3.6/ai2_kit/tool/__init__.py
+-rw-r--r--   0        0        0      676 2023-06-25 01:09:08.610393 ai2_kit-0.3.6/ai2_kit/tool/ase.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.6/ai2_kit/workflow/__init__.py
+-rw-r--r--   0        0        0     8161 2023-06-27 03:26:30.711049 ai2_kit-0.3.6/ai2_kit/workflow/cll_mlp.py
+-rw-r--r--   0        0        0     9117 2023-06-27 03:26:30.711049 ai2_kit-0.3.6/ai2_kit/workflow/fep_mlp.py
+-rw-r--r--   0        0        0      843 2023-06-27 09:16:09.938406 ai2_kit-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 ai2_kit-0.3.6/PKG-INFO
```

### Comparing `ai2_kit-0.3.5/LICENSE` & `ai2_kit-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/README.md` & `ai2_kit-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/ai2_kit/algorithm/proton_transfer.py` & `ai2_kit-0.3.6/ai2_kit/algorithm/proton_transfer.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/ai2_kit/core/artifact.py` & `ai2_kit-0.3.6/ai2_kit/core/artifact.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/ai2_kit/core/checkpoint.py` & `ai2_kit-0.3.6/ai2_kit/core/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/ai2_kit/core/connector.py` & `ai2_kit-0.3.6/ai2_kit/core/connector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/ai2_kit/core/executor.py` & `ai2_kit-0.3.6/ai2_kit/core/executor.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/ai2_kit/core/job.py` & `ai2_kit-0.3.6/ai2_kit/core/job.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/ai2_kit/core/queue_system.py` & `ai2_kit-0.3.6/ai2_kit/core/queue_system.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/ai2_kit/core/resource_manager.py` & `ai2_kit-0.3.6/ai2_kit/core/resource_manager.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/ai2_kit/core/script.py` & `ai2_kit-0.3.6/ai2_kit/core/script.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/ai2_kit/core/util.py` & `ai2_kit-0.3.6/ai2_kit/core/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 merge_dict = __merge_dict()
 
 
 # TODO: support http(s) url
 def load_yaml_file(path: Path):
     yaml = YAML(typ='safe')
     JoinTag.register(yaml)
+    ReadTag.register(yaml)
     return yaml.load(path)
 
 
 def load_yaml_files(*paths: Tuple[Path]):
     d = {}
     for path in paths:
         print('load yaml file: ', path)
@@ -62,14 +63,15 @@
 
 
 def s_uuid():
     """short uuid"""
     return shortuuid.uuid()
 
 
+# TODO: this should be moved out from core module
 def parse_cp2k_input(text: str):
     parser = CP2KInputParserSimplified(key_trafo=str.upper)
     return parser.parse(io.StringIO(text))
 
 
 def dict_nested_get(d: dict, keys: List[str], default=EMPTY):
     """get value from nested dict"""
@@ -130,9 +132,31 @@
 
     @classmethod
     def to_yaml(cls, dumper, data):
         # do nothing
         return dumper.represent_sequence(cls.yaml_tag, data)
 
     @classmethod
+    def register(cls, yaml: YAML):
+        yaml.register_class(cls)
+
+
+class ReadTag:
+    """a tag to read string from file"""
+
+    yaml_tag = u'!read'
+
+    @classmethod
+    def from_yaml(cls, constructor, node):
+        seq = constructor.construct_sequence(node)
+        path = os.path.join(*seq)
+        with open(path, 'r') as f:
+            return f.read()
+
+    @classmethod
+    def to_yaml(cls, dumper, data):
+        # do nothing
+        return dumper.represent_sequence(cls.yaml_tag, data)
+
+    @classmethod
     def register(cls, yaml: YAML):
         yaml.register_class(cls)
```

### Comparing `ai2_kit-0.3.5/ai2_kit/domain/cll.py` & `ai2_kit-0.3.6/ai2_kit/domain/cll.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/ai2_kit/domain/cp2k.py` & `ai2_kit-0.3.6/ai2_kit/domain/cp2k.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/ai2_kit/domain/data_helper.py` & `ai2_kit-0.3.6/ai2_kit/domain/data_helper.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/ai2_kit/domain/deepmd.py` & `ai2_kit-0.3.6/ai2_kit/domain/deepmd.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/ai2_kit/domain/lammps.py` & `ai2_kit-0.3.6/ai2_kit/domain/lammps.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/ai2_kit/domain/selector.py` & `ai2_kit-0.3.6/ai2_kit/domain/selector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/ai2_kit/main.py` & `ai2_kit-0.3.6/ai2_kit/main.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/ai2_kit/tool/ase.py` & `ai2_kit-0.3.6/ai2_kit/tool/ase.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/ai2_kit/workflow/cll_mlp.py` & `ai2_kit-0.3.6/ai2_kit/workflow/cll_mlp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/ai2_kit/workflow/fep_mlp.py` & `ai2_kit-0.3.6/ai2_kit/workflow/fep_mlp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.5/pyproject.toml` & `ai2_kit-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai2-kit"
-version = "0.3.5"
+version = "0.3.6"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ai2_kit"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `ai2_kit-0.3.5/PKG-INFO` & `ai2_kit-0.3.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai2-kit
-Version: 0.3.5
+Version: 0.3.6
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

