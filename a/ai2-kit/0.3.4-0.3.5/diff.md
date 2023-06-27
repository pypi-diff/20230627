# Comparing `tmp/ai2_kit-0.3.4.tar.gz` & `tmp/ai2_kit-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai2_kit-0.3.4.tar", max compression
+gzip compressed data, was "ai2_kit-0.3.5.tar", max compression
```

## Comparing `ai2_kit-0.3.4.tar` & `ai2_kit-0.3.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.3.4/LICENSE
--rw-r--r--   0        0        0     1312 2023-06-21 07:23:29.824581 ai2_kit-0.3.4/README.md
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.4/ai2_kit/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 03:47:09.348444 ai2_kit-0.3.4/ai2_kit/algorithm/__init__.py
--rw-r--r--   0        0        0    12100 2023-06-13 03:47:09.348444 ai2_kit-0.3.4/ai2_kit/algorithm/proton_transfer.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.4/ai2_kit/core/__init__.py
--rw-r--r--   0        0        0     1884 2023-03-22 04:23:44.538179 ai2_kit-0.3.4/ai2_kit/core/artifact.py
--rw-r--r--   0        0        0     5465 2023-06-21 07:23:29.824581 ai2_kit-0.3.4/ai2_kit/core/checkpoint.py
--rw-r--r--   0        0        0      169 2023-06-21 03:36:08.888345 ai2_kit-0.3.4/ai2_kit/core/cmd.py
--rw-r--r--   0        0        0     5766 2023-02-06 09:01:27.000000 ai2_kit-0.3.4/ai2_kit/core/connector.py
--rw-r--r--   0        0        0     7995 2023-06-21 07:23:29.824581 ai2_kit-0.3.4/ai2_kit/core/executor.py
--rw-r--r--   0        0        0      365 2023-06-21 07:23:29.824581 ai2_kit-0.3.4/ai2_kit/core/future.py
--rw-r--r--   0        0        0     1852 2023-06-21 07:23:29.824581 ai2_kit-0.3.4/ai2_kit/core/job.py
--rw-r--r--   0        0        0      298 2023-06-20 08:43:41.238220 ai2_kit-0.3.4/ai2_kit/core/log.py
--rw-r--r--   0        0        0     9449 2023-06-21 07:23:29.824581 ai2_kit-0.3.4/ai2_kit/core/queue_system.py
--rw-r--r--   0        0        0     2315 2023-03-22 04:23:44.538179 ai2_kit-0.3.4/ai2_kit/core/resource_manager.py
--rw-r--r--   0        0        0     2358 2023-06-19 08:54:25.567391 ai2_kit-0.3.4/ai2_kit/core/script.py
--rw-r--r--   0        0        0     2911 2023-06-21 07:23:29.824581 ai2_kit-0.3.4/ai2_kit/core/util.py
--rw-r--r--   0        0        0        0 2023-06-13 03:47:09.348444 ai2_kit-0.3.4/ai2_kit/dflow/__init__.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.4/ai2_kit/domain/__init__.py
--rw-r--r--   0        0        0     1580 2023-06-20 08:43:41.238220 ai2_kit-0.3.4/ai2_kit/domain/cll.py
--rw-r--r--   0        0        0      341 2023-02-27 08:58:57.520622 ai2_kit-0.3.4/ai2_kit/domain/constant.py
--rw-r--r--   0        0        0     7773 2023-06-21 07:23:29.824581 ai2_kit-0.3.4/ai2_kit/domain/cp2k.py
--rw-r--r--   0        0        0     4129 2023-06-20 08:43:41.238220 ai2_kit-0.3.4/ai2_kit/domain/data_helper.py
--rw-r--r--   0        0        0     6679 2023-06-21 07:23:29.824581 ai2_kit-0.3.4/ai2_kit/domain/deepmd.py
--rw-r--r--   0        0        0    15549 2023-06-21 07:23:29.824581 ai2_kit-0.3.4/ai2_kit/domain/lammps.py
--rw-r--r--   0        0        0     3039 2023-06-20 08:43:41.238220 ai2_kit-0.3.4/ai2_kit/domain/selector.py
--rw-r--r--   0        0        0      183 2023-03-22 04:23:44.538179 ai2_kit-0.3.4/ai2_kit/domain/updater.py
--rw-r--r--   0        0        0     1588 2023-06-21 07:23:29.824581 ai2_kit-0.3.4/ai2_kit/main.py
--rw-r--r--   0        0        0        0 2023-06-20 08:43:41.238220 ai2_kit-0.3.4/ai2_kit/tool/__init__.py
--rw-r--r--   0        0        0      676 2023-06-21 07:23:29.824581 ai2_kit-0.3.4/ai2_kit/tool/ase.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.4/ai2_kit/workflow/__init__.py
--rw-r--r--   0        0        0     7840 2023-06-21 07:23:29.824581 ai2_kit-0.3.4/ai2_kit/workflow/cll_mlp.py
--rw-r--r--   0        0        0     9076 2023-06-21 07:23:29.824581 ai2_kit-0.3.4/ai2_kit/workflow/fep_mlp.py
--rw-r--r--   0        0        0      843 2023-06-21 07:23:47.352913 ai2_kit-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2339 1970-01-01 00:00:00.000000 ai2_kit-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1627 2023-06-27 03:30:12.011023 ai2_kit-0.3.5/README.md
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.5/ai2_kit/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-25 01:09:08.600393 ai2_kit-0.3.5/ai2_kit/algorithm/__init__.py
+-rw-r--r--   0        0        0    12100 2023-06-25 01:09:08.600393 ai2_kit-0.3.5/ai2_kit/algorithm/proton_transfer.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.5/ai2_kit/core/__init__.py
+-rw-r--r--   0        0        0     1854 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/core/artifact.py
+-rw-r--r--   0        0        0     5465 2023-06-25 01:09:08.600393 ai2_kit-0.3.5/ai2_kit/core/checkpoint.py
+-rw-r--r--   0        0        0      169 2023-06-25 01:09:08.600393 ai2_kit-0.3.5/ai2_kit/core/cmd.py
+-rw-r--r--   0        0        0     5766 2023-02-06 09:01:27.000000 ai2_kit-0.3.5/ai2_kit/core/connector.py
+-rw-r--r--   0        0        0     7939 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/core/executor.py
+-rw-r--r--   0        0        0      365 2023-06-25 01:09:08.600393 ai2_kit-0.3.5/ai2_kit/core/future.py
+-rw-r--r--   0        0        0     1852 2023-06-25 01:09:08.600393 ai2_kit-0.3.5/ai2_kit/core/job.py
+-rw-r--r--   0        0        0      298 2023-06-25 01:09:08.610393 ai2_kit-0.3.5/ai2_kit/core/log.py
+-rw-r--r--   0        0        0     9449 2023-06-25 01:09:08.610393 ai2_kit-0.3.5/ai2_kit/core/queue_system.py
+-rw-r--r--   0        0        0     2572 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/core/resource_manager.py
+-rw-r--r--   0        0        0     2358 2023-06-19 08:54:25.567391 ai2_kit-0.3.5/ai2_kit/core/script.py
+-rw-r--r--   0        0        0     3604 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/core/util.py
+-rw-r--r--   0        0        0        0 2023-06-25 01:09:08.610393 ai2_kit-0.3.5/ai2_kit/dflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.5/ai2_kit/domain/__init__.py
+-rw-r--r--   0        0        0     1734 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/domain/cll.py
+-rw-r--r--   0        0        0      341 2023-02-27 08:58:57.520622 ai2_kit-0.3.5/ai2_kit/domain/constant.py
+-rw-r--r--   0        0        0     8210 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/domain/cp2k.py
+-rw-r--r--   0        0        0     4356 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/domain/data_helper.py
+-rw-r--r--   0        0        0     6679 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/domain/deepmd.py
+-rw-r--r--   0        0        0    16845 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/domain/lammps.py
+-rw-r--r--   0        0        0     3039 2023-06-26 06:22:57.018618 ai2_kit-0.3.5/ai2_kit/domain/selector.py
+-rw-r--r--   0        0        0      183 2023-03-22 04:23:44.538179 ai2_kit-0.3.5/ai2_kit/domain/updater.py
+-rw-r--r--   0        0        0     1588 2023-06-25 01:09:08.610393 ai2_kit-0.3.5/ai2_kit/main.py
+-rw-r--r--   0        0        0        0 2023-06-25 01:09:08.610393 ai2_kit-0.3.5/ai2_kit/tool/__init__.py
+-rw-r--r--   0        0        0      676 2023-06-25 01:09:08.610393 ai2_kit-0.3.5/ai2_kit/tool/ase.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.5/ai2_kit/workflow/__init__.py
+-rw-r--r--   0        0        0     8161 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/workflow/cll_mlp.py
+-rw-r--r--   0        0        0     9117 2023-06-27 03:26:30.711049 ai2_kit-0.3.5/ai2_kit/workflow/fep_mlp.py
+-rw-r--r--   0        0        0      843 2023-06-27 03:28:50.521034 ai2_kit-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 ai2_kit-0.3.5/PKG-INFO
```

### Comparing `ai2_kit-0.3.4/LICENSE` & `ai2_kit-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.4/ai2_kit/algorithm/proton_transfer.py` & `ai2_kit-0.3.5/ai2_kit/algorithm/proton_transfer.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.4/ai2_kit/core/artifact.py` & `ai2_kit-0.3.5/ai2_kit/core/artifact.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,53 +8,53 @@
     class ArtifactDict(TypedDict):
         """
         A dict representation of Artifact.
         Use this when you need to run a remote function call as pydantic model is not pickleable.
 
         referrer is not included in this dict as it is not pickleable.
         """
-        executor: Optional[str]
         url: str
+        attrs: dict
+        executor: Optional[str]
         format: Optional[str]
         includes: Optional[str]
-        attrs: dict
+        key: Optional[str]
     return ArtifactDict
 ArtifactDict = __ArtifactDict()
 
 
 class Artifact(BaseModel):
+
+    key: Optional[str]
     executor: Optional[str]
     url: str
     format: Optional[str]
     includes: Optional[str]
     attrs: dict = dict()
-    referrer: Optional['Artifact']
 
     @classmethod
     def of(cls,
            url: str,
+           key: Optional[str] = None,
            executor: Optional[str] = None,
            includes: Optional[str] = None,
            attrs: Optional[dict] = None,
-           format: Optional[str] = None,
-           referrer: Optional['Artifact'] = None):
+           format: Optional[str] = None,):
         """Create an Artifact instance. Use this instead of __init__ to avoid type error of pydantic"""
-        return cls(
-            url=url,
-            executor=executor,
-            format=format,
-            includes=includes,
-            attrs=dict() if attrs is None else copy.deepcopy(attrs),  # deepcopy to reduce chance of mistake
-            referrer=referrer,
-        )
+        return cls(url=url,
+                   executor=executor,
+                   format=format,
+                   includes=includes,
+                   attrs=dict() if attrs is None else copy.deepcopy(attrs),  # deepcopy to reduce chance of mistake
+                   key=key)
 
     def to_dict(self) -> ArtifactDict:
         """Convert to a dict representation.
         Use this when you need to run a remote function call as pydantic model is not pickleable."""
-        return self.dict(exclude={'referrer',})  # type: ignore
+        return self.dict() # type: ignore
 
     def join(self, *paths, **kwargs):
         url = os.path.join(self.url, *paths)
-        return Artifact.of(url=url, executor=self.executor, referrer=self, **kwargs)
+        return Artifact.of(url=url, executor=self.executor, **kwargs)
 
 
 ArtifactMap = Mapping[str, Artifact]
```

### Comparing `ai2_kit-0.3.4/ai2_kit/core/checkpoint.py` & `ai2_kit-0.3.5/ai2_kit/core/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.4/ai2_kit/core/connector.py` & `ai2_kit-0.3.5/ai2_kit/core/connector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.4/ai2_kit/core/executor.py` & `ai2_kit-0.3.5/ai2_kit/core/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,12 +222,11 @@
 
 
 def fn_to_script(fn: Callable, delimiter='@'):
     dumped_fn = base64.b64encode(bz2.compress(cloudpickle.dumps(fn, protocol=cloudpickle.DEFAULT_PROTOCOL), 5))
     script = [
         f'''import base64,bz2,sys,cloudpickle as cp''',
         f'''r=cp.loads(bz2.decompress(base64.b64decode({repr(dumped_fn)})))()''',
-        f'''sys.stdout.flush()''',  # avoid overlapping
         f'''print({repr(delimiter)}+base64.b64encode(bz2.compress(cp.dumps(r, protocol=cp.DEFAULT_PROTOCOL),5)).decode('ascii'))''',
         f'''sys.stdout.flush()''',  # ensure all output is printed
     ]
     return ';'.join(script)
```

### Comparing `ai2_kit-0.3.4/ai2_kit/core/job.py` & `ai2_kit-0.3.5/ai2_kit/core/job.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.4/ai2_kit/core/queue_system.py` & `ai2_kit-0.3.5/ai2_kit/core/queue_system.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.4/ai2_kit/core/resource_manager.py` & `ai2_kit-0.3.5/ai2_kit/core/resource_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,19 +16,26 @@
     def __init__(self,
                  executor_configs: ExecutorMap,
                  artifacts: ArtifactMap,
                  default_executor: str,
                  ) -> None:
 
         self._executor_configs = executor_configs
-        self._artifacts = artifacts
         self._default_executor_name = default_executor
         self._executors: Dict[str, Executor] = dict()
+        # runtime check to ensure quick failure
+        self.default_executor
 
-        self.default_executor  # runtime check!
+        # fill in default values
+        for key, artifact in artifacts.items():
+            if artifact.executor is None:
+                artifact.executor = self.default_executor.name
+            if artifact.key is None:
+                artifact.key = key
+        self._artifacts = artifacts
 
     def get_executor(self, name: Optional[str] = None) -> Executor:
         if name is None:
             name = self._default_executor_name
 
         config = self._executor_configs.get(name)
         if config is None:
@@ -56,14 +63,13 @@
         paths = self.default_executor.resolve_artifact(artifact)
 
         return [Artifact.of(
             url=path,
             format=artifact.format,
             includes=None,  # has been consumed
             attrs=copy.deepcopy(artifact.attrs),
-            referrer=artifact,
             executor=self.default_executor.name,
         ) for path in paths]
 
     def resolve_artifacts(self, artifacts: Sequence[ArtifactOrKey]) -> List[Artifact]:
         # flat map
         return [x for a in artifacts for x in self.resolve_artifact(a)]
```

### Comparing `ai2_kit-0.3.4/ai2_kit/core/script.py` & `ai2_kit-0.3.5/ai2_kit/core/script.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.4/ai2_kit/domain/cll.py` & `ai2_kit-0.3.5/ai2_kit/domain/cll.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import abstractmethod, ABC
-from ai2_kit.core.artifact import Artifact
+from ai2_kit.core.artifact import Artifact, ArtifactMap
 from ai2_kit.core.future import IFuture
 from ai2_kit.core.resource_manager import ResourceManager
 from typing import List, Callable, Any
 from dataclasses import dataclass
 
 @dataclass
 class BaseCllContext:
@@ -63,7 +63,12 @@
         ...
 
     @abstractmethod
     def get_passing_rate(self) -> float:
         ...
 
 CllSelectorTaskType = Callable[[Any, BaseCllContext], IFuture[ICllSelectorOutput]]
+
+
+def init_artifacts(artifacts: ArtifactMap):
+    for key, artifact in artifacts.items():
+        artifact.attrs.setdefault('ancestor', key)
```

### Comparing `ai2_kit-0.3.4/ai2_kit/domain/cp2k.py` & `ai2_kit-0.3.5/ai2_kit/domain/cp2k.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from ai2_kit.core.artifact import Artifact
+from ai2_kit.core.artifact import Artifact, ArtifactDict
 from ai2_kit.core.script import BashScript, BashStep, BashTemplate
 from ai2_kit.core.job import gather_jobs
 from ai2_kit.core.util import merge_dict, parse_cp2k_input, dict_nested_get, dict_nested_set, split_list
 from ai2_kit.core.log import get_logger
 
-from typing import List, Union
+from typing import List, Union, Tuple
 from pydantic import BaseModel
 from dataclasses import dataclass
 
 import copy
 import os
 
 from .data_helper import LammpsOutputHelper, XyzHelper, Cp2kOutputHelper, ase_atoms_to_cp2k_input_data
@@ -107,88 +107,94 @@
         else:
             raise ValueError(f'unsupported format {system_file.url}: {system_file.format}')
 
     # create task dirs and prepare input files
     cp2k_task_dirs = []
     if lammps_dump_files or xyz_files:
         cp2k_task_dirs = executor.run_python_fn(make_cp2k_task_dirs)(
-            lammps_dump_files=[a.url for a in lammps_dump_files],
-            xyz_files=[a.url for a in xyz_files],
+            lammps_dump_files=[a.to_dict() for a in lammps_dump_files],
+            xyz_files=[a.to_dict() for a in xyz_files],
             type_map=input.type_map,
             base_dir=tasks_dir,
             input_template=input_template,
             limit=input.config.limit,
         )
     else:
         logger.warn('no available candidates, skip')
         return GenericCp2kOutput(cp2k_outputs=[])
 
     # build commands
     steps = []
     for cp2k_task_dir in cp2k_task_dirs:
         steps.append(BashStep(
-            cwd=cp2k_task_dir,
+            cwd=cp2k_task_dir['url'],
             cmd=[ctx.config.cp2k_cmd, '-i input.inp 1>> output 2>> output'],
             checkpoint='cp2k',
         ))
 
     # submit tasks and wait for completion
     jobs = []
     for i, steps_group in enumerate(split_list(steps, ctx.config.concurrency)):
         if not steps_group:
             continue
         script = BashScript(
             template=ctx.config.script_template,
             steps=steps_group,
         )
         job = executor.submit(script.render(), cwd=tasks_dir,
-                              checkpoint_key=f'submit-job/cp2k/{i}@{tasks_dir}')
+                              checkpoint_key=f'submit-job/cp2k/{i}:{tasks_dir}')
         jobs.append(job)
     jobs = await gather_jobs(jobs, max_tries=2)
 
     cp2k_outputs = [Artifact.of(
-        url=url,
+        url=a['url'],
         format=Cp2kOutputHelper.format,
         executor=executor.name,
-        attrs=dict(),  # TODO: success from input
-    ) for url in cp2k_task_dirs]
+        attrs=a['attrs'],
+    ) for a in cp2k_task_dirs]
 
     return GenericCp2kOutput(cp2k_outputs=cp2k_outputs)
 
 
 def __make_cp2k_task_dirs():
-    def make_cp2k_task_dirs(lammps_dump_files: List[str],
-                            xyz_files: List[str],
+    def make_cp2k_task_dirs(lammps_dump_files: List[ArtifactDict],
+                            xyz_files: List[ArtifactDict],
                             type_map: List[str],
                             input_template: dict,
                             base_dir: str,
                             limit: int = 0,
                             input_file_name: str = 'input.inp',
-                            ) -> List[str]:
+                            ) -> List[ArtifactDict]:
         """Generate CP2K input files from LAMMPS dump files or XYZ files."""
         from cp2k_input_tools import DEFAULT_CP2K_INPUT_XML
         from cp2k_input_tools.generator import CP2KInputGenerator
 
         import ase.io
         from ase import Atoms
 
         cp2k_generator = CP2KInputGenerator(DEFAULT_CP2K_INPUT_XML)
         task_dirs = []
-        atoms_list: List[Atoms] = []
+        atoms_list: List[Tuple[ArtifactDict, Atoms]] = []
 
         # read atoms
         for dump_file in lammps_dump_files:
-            atoms_list += ase.io.read(dump_file, ':', format='lammps-dump-text', order=False, specorder=type_map)  # type: ignore
+            atoms_list += [
+                (dump_file, atoms)
+                for atoms in ase.io.read(dump_file['url'], ':', format='lammps-dump-text', order=False, specorder=type_map)
+            ]  # type: ignore
         for xyz_file in xyz_files:
-            atoms_list += ase.io.read(xyz_file, ':', format='extxyz')  # type: ignore
+            atoms_list += [
+                (xyz_file, atoms)
+                for atoms in ase.io.read(xyz_file['url'], ':', format='extxyz')
+            ]  # type: ignore
 
         if limit > 0:
             atoms_list = atoms_list[:limit]
 
-        for i, atoms in enumerate(atoms_list):
+        for i, (file, atoms) in enumerate(atoms_list):
             # create task dir
             task_dir = os.path.join(base_dir, f'{str(i).zfill(6)}')
             os.makedirs(task_dir, exist_ok=True)
 
             # create input file
             input_data = copy.deepcopy(input_template)
             coords, cell = ase_atoms_to_cp2k_input_data(atoms)
@@ -205,12 +211,19 @@
                         }
                     }
                 }
             })
             input_text = '\n'.join(cp2k_generator.line_iter(input_data))
             with open(os.path.join(task_dir, input_file_name), 'w') as f:
                 f.write(input_text)
-            task_dirs.append(task_dir)
+
+            # inherit attrs from input file
+            # TODO: inherit only ancestor key should be enough
+            task_dirs.append({
+                'url': task_dir,
+                'attrs': file['attrs'],
+            })
+
         return task_dirs
 
     return make_cp2k_task_dirs
 make_cp2k_task_dirs = __make_cp2k_task_dirs()
```

### Comparing `ai2_kit-0.3.4/ai2_kit/domain/data_helper.py` & `ai2_kit-0.3.5/ai2_kit/domain/data_helper.py`

 * *Files 13% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 class DeepmdModelHelper(DataHelper):
     format = 'deepmd/model'
 
 class Cp2kOutputHelper(DataHelper):
     format = 'cp2k-output-dir'
 
 
+
 def __ase_atoms_to_cp2k_input_data():
     """workaround for cloudpickle issue"""
     def ase_atoms_to_cp2k_input_data(atoms: Atoms) -> Tuple[List[str], List[List[float]]]:
         """
         Convert ASE Atoms to CP2K input format
         """
         coords = [atom.symbol + ' ' + ' '.join(str(x) for x in atom.position) for atom in atoms] # type: ignore
@@ -72,23 +73,27 @@
 
 def __convert_to_deepmd_npy():
     """workaround for cloudpickle issue"""
     def covert_to_deepmd_npy(cp2k_outputs: List[ArtifactDict], base_dir: str, type_map: List[str]):
         import dpdata
         from itertools import groupby
 
-        atoms_list: List[Atoms] = []
+        atoms_list: List[Tuple[ArtifactDict, Atoms]] = []
         for cp2k_output in cp2k_outputs:
             dp_system = dpdata.LabeledSystem(os.path.join(cp2k_output['url'], 'output'), fmt='cp2k/output', type_map=type_map)
-            atoms_list.extend(dp_system.to_ase_structure())  # type: ignore
+            atoms_list += [
+                (cp2k_output, atoms)
+                for atoms in dp_system.to_ase_structure()  # type: ignore
+            ]
 
         output_dirs = []
-        for i, (symbols, atoms_group) in enumerate(groupby(atoms_list, key=lambda x: str(x.symbols))):
-            output_dir = os.path.join(base_dir, f'{i:03d}')
-            atoms_group = list(atoms_group)
+        # group dataset by ancestor key
+        for i, (key, atoms_group) in enumerate(groupby(atoms_list, key=lambda x: x[0]['attrs']['ancestor'])):
+            output_dir = os.path.join(base_dir, key.replace('/', '_'))
+            atoms_group = list(item[1] for item in atoms_group)
             if not atoms_group:
                 continue
             dp_system = dpdata.LabeledSystem(atoms_group[0], fmt='ase/structure')
             for atoms in atoms_group[1:]:
                 dp_system += dpdata.LabeledSystem(atoms, fmt='ase/structure')
             dp_system.to_deepmd_npy(output_dir, set_size=len(dp_system))  # type: ignore
             # TODO: return ArtifactDict
@@ -100,18 +105,19 @@
 
 
 def __convert_to_lammps_input_data():
     """workaround for cloudpickle issue"""
     def convert_to_lammps_input_data(poscar_files: List[ArtifactDict], base_dir: str, type_map: List[str]):
         import dpdata
         import os
-
         lammps_data_files = []
         for i, poscar_file in enumerate(poscar_files):
             output_file = os.path.join(base_dir, f'{i:06d}.lammps.data')
             dpdata.System(poscar_file['url'], fmt='vasp/poscar', type_map=type_map).to_lammps_lmp(output_file)  # type: ignore
-            lammps_data_files.append(output_file)
-        # TODO: return ArtifactDict
+            lammps_data_files.append({
+                'url': output_file,
+                'attrs': poscar_file['attrs'],
+            })
         return lammps_data_files
 
     return convert_to_lammps_input_data
 convert_to_lammps_input_data = __convert_to_lammps_input_data()
```

### Comparing `ai2_kit-0.3.4/ai2_kit/domain/deepmd.py` & `ai2_kit-0.3.5/ai2_kit/domain/deepmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
                 BashStep(cmd=dp_train_cmd, checkpoint='dp-train'),  # type: ignore
                 BashStep(cmd=dp_freeze_cmd),  # type: ignore
             ] # type: ignore
         )
         output_dirs.append(task_dir)
 
         # submit job
-        job = executor.submit(dp_train_script.render(), cwd=task_dir, checkpoint_key=f'submit-job/dp-train/{i}@{task_dir}')
+        job = executor.submit(dp_train_script.render(), cwd=task_dir, checkpoint_key=f'submit-job/dp-train/{i}:{task_dir}')
         jobs.append(job)
 
     await gather_jobs(jobs, max_tries=2)
 
     return GenericDeepmdOutput(
         input=input,
         outputs=[Artifact.of(
```

### Comparing `ai2_kit-0.3.4/ai2_kit/domain/lammps.py` & `ai2_kit-0.3.5/ai2_kit/domain/lammps.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ai2_kit.core.script import BashTemplate, BashStep, BashScript
-from ai2_kit.core.artifact import Artifact
+from ai2_kit.core.artifact import Artifact, ArtifactDict
 from ai2_kit.core.log import get_logger
 from ai2_kit.core.job import gather_jobs
-from ai2_kit.core.util import split_list
+from ai2_kit.core.util import split_list, dict_nested_get
 
-from typing import List, Literal, Optional, Union, Mapping, Sequence
+from typing import List, Literal, Optional, Union, Mapping, Sequence, Any
 from pydantic import BaseModel
 from dataclasses import dataclass
 from string import Template
 from allpairspy import AllPairs
 import os
 import itertools
 import random
@@ -22,24 +22,23 @@
     LAMMPS_TRAJ_DIR,
     LAMMPS_TRAJ_SUFFIX,
 )
 from .data_helper import LammpsOutputHelper, PoscarHelper, convert_to_lammps_input_data
 
 logger = get_logger(__name__)
 
-Scalar = Union[str, int, float, bool]
 
 class ExploreVariants(BaseModel):
     temp: List[float]
     """Temperatures variants."""
 
     pres: List[float]
     """Pressures variants."""
 
-    others: Mapping[str, Sequence[Scalar]] = dict()
+    others: Mapping[str, Sequence[Any]] = dict()
     """
     Other variants to be combined with.
     The key is the name of the variant, and the value is the list of values.
     For example, if you want to combine the variant 'LAMBDA' with values [0.0, 0.5, 1.0],
     you can set the others field to {'LAMBDA': [0.0, 0.5, 1.0]}.
     And in LAMMPS input template, you can use the variable ${LAMBDA} and v_LAMBDA to access the value.
     """
@@ -57,14 +56,17 @@
     the full combination will be used.
     It is strongly recommended to use n_wise when the full combination is too large.
     """
 
     system_files: List[str]
     """Artifacts of initial system data."""
 
+    plumed_config: Optional[str]
+    """Plumed config file content."""
+
     no_pbc: bool = False
     tau_t: float = 0.1
     tau_p: float = 0.5
     timestep: float = 0.0005
     sample_freq: int
     nsteps: int
     ensemble: Literal['nvt', 'nvt-i', 'nvt-a', 'nvt-iso', 'nvt-aniso', 'npt', 'npt-t', 'npt-tri', 'nve']
@@ -146,26 +148,26 @@
 
     for system_file in systems:
         if PoscarHelper.is_match(system_file):
             poscar_files.append(system_file)
         else:
             raise ValueError(f'unsupported system file type: {system_file}')
 
-    input_data_files: List[str] = executor.run_python_fn(convert_to_lammps_input_data)(
+    input_data_files: List[ArtifactDict] = executor.run_python_fn(convert_to_lammps_input_data)(
         poscar_files=[a.to_dict() for a in poscar_files],
         base_dir=input_data_dir,
         type_map=input.type_map,
     )
 
     combination_fields: List[str] = [
         'data_file',
         'temp',
         'pres'
     ]
-    combination_values: Sequence[Sequence[Scalar]] = [
+    combination_values: Sequence[Sequence[Any]] = [
         input_data_files,
         input.config.explore_vars.temp,
         input.config.explore_vars.pres,
     ]
 
     for k, v in input.config.explore_vars.others.items():
         combination_fields.append(k)
@@ -174,21 +176,22 @@
     if 1 < input.config.n_wise <= len(combination_fields):
         logger.info('using %d-wise combination', input.config.n_wise)
         combinations = AllPairs(combination_values, n=input.config.n_wise)
     else:
         logger.info('using full combination')
         combinations = itertools.product(*combination_values)
 
-    lammps_task_dirs = []
+    lammps_task_dirs: List[ArtifactDict] = []
     lammps_input_file_name = 'lammps.input'
 
     for i, combination in enumerate(combinations):
-        data_file, temp, pres = combination[:3]
+        data_file: ArtifactDict = combination[0]
+        temp, pres = combination[1:3]
         others_dict = dict(zip(combination_fields[3:], combination[3:]))
-        lammps_task_dir = os.path.join(tasks_dir, str(i).zfill(6))
+        lammps_task_dir = os.path.join(tasks_dir, f'{i:06d}')
         executor.mkdir(os.path.join(lammps_task_dir, LAMMPS_TRAJ_DIR))  # create dump directory for lammps or else will get error
 
         if input.md_options:
             force_field_section = make_md_force_field_section(
                 models=[a.url for a in input.md_options.models],
             )
         elif input.fep_options:
@@ -200,82 +203,90 @@
             others_dict['minus'] = -1
             force_field_section = make_fep_force_field_section(
                 neu_models=[a.url for a in input.fep_options.neu_models],
                 red_models=[a.url for a in input.fep_options.red_models],
             )
         else:
             raise ValueError('one and only one of md_options or fep_options must be set')
-        template = input.config.input_template or  DEFAULT_LAMMPS_INPUT_TEMPLATE
 
-        input_text = make_lammps_input(data_file=data_file,
-                          nsteps=input.config.nsteps,
-                          timestep=input.config.timestep,
-                          trj_freq=input.config.sample_freq,
-                          temp=temp,
-                          pres=pres,
-                          tau_t=input.config.tau_t,
-                          tau_p=input.config.tau_p,
-                          ensemble=input.config.ensemble,
-                          mass_map=input.mass_map,
-                          others_dict=others_dict,
-
-                          force_field_section=force_field_section,
-
-                          template=template,
-                          post_variables_section=input.config.post_variables_section,
-                          post_init_section=input.config.post_init_section,
-                          post_read_data_section=input.config.post_read_data_section,
-                          post_force_field_section=input.config.post_force_field_section,
-                          post_md_section=input.config.post_md_section,
-                          post_run_section=input.config.post_run_section,
-
-                          no_pbc=False,
-                          rand_start=1_000_000,
-                          )
+        plumed_file = None
+        # plumed_config could be overrided by the attrs of data_file
+        plumed_config = dict_nested_get(data_file, ['attrs', 'lammps', 'plumed_config'],
+                                        input.config.plumed_config)
+
+        if plumed_config and isinstance(plumed_config, str):
+            plumed_file = 'plumed.input'
+            plumed_file_path = os.path.join(lammps_task_dir, plumed_file)
+            logger.info(f'found plumed config, generate {plumed_file_path}')
+            executor.dump_text(plumed_config, plumed_file_path)
+
+        template = input.config.input_template or  DEFAULT_LAMMPS_INPUT_TEMPLATE
 
+        input_text = make_lammps_input(data_file=data_file['url'],
+                                       nsteps=input.config.nsteps,
+                                       timestep=input.config.timestep,
+                                       trj_freq=input.config.sample_freq,
+                                       temp=temp,
+                                       pres=pres,
+                                       tau_t=input.config.tau_t,
+                                       tau_p=input.config.tau_p,
+                                       ensemble=input.config.ensemble,
+                                       mass_map=input.mass_map,
+                                       others_dict=others_dict,
+
+                                       force_field_section=force_field_section,
+
+                                       template=template,
+                                       post_variables_section=input.config.post_variables_section,
+                                       post_init_section=input.config.post_init_section,
+                                       post_read_data_section=input.config.post_read_data_section,
+                                       post_force_field_section=input.config.post_force_field_section,
+                                       post_md_section=input.config.post_md_section,
+                                       post_run_section=input.config.post_run_section,
+                                       plumed_file=plumed_file,
+                                       no_pbc=False,
+                                       rand_start=1_000_000,
+                                       )
         input_file_path = os.path.join(lammps_task_dir, lammps_input_file_name)
+        logger.info(f'generate lammps config {input_file_path}')
+
         executor.dump_text(input_text, input_file_path)
-        lammps_task_dirs.append(lammps_task_dir)
+        lammps_task_dirs.append({'url': lammps_task_dir, 'attrs': data_file['attrs']})  # type: ignore
 
     # build scripts and submit
     lammps_cmd = ctx.config.lammps_cmd
     base_cmd = f'{lammps_cmd} -i {lammps_input_file_name}'
     cmd = f'''if [ -f md.restart.* ]; then {base_cmd} -v restart 1; else {base_cmd} -v restart 0; fi'''
 
     # generate steps
     steps = []
     for lammps_task_dir in lammps_task_dirs:
-        steps.append(BashStep(
-            cwd=lammps_task_dir,
-            cmd=cmd,
-            checkpoint='lammps',
-        ))
+        steps.append(BashStep(cwd=lammps_task_dir['url'], cmd=cmd, checkpoint='lammps'))
 
-    # submit jobs
+    # submit jobs by the number of concurrency
     jobs = []
     for i, steps_group in enumerate(split_list(steps, ctx.config.concurrency)):
         if not steps_group:
             continue
         script = BashScript(
             template=ctx.config.script_template,
             steps=steps_group,
         )
         job = executor.submit(script.render(), cwd=tasks_dir,
-                              checkpoint_key=f'submit-job/lammps/{i}@{tasks_dir}')
+                              checkpoint_key=f'submit-job/lammps/{i}:{tasks_dir}')
         jobs.append(job)
 
     await gather_jobs(jobs, max_tries=2)
 
     outputs = [
         Artifact.of(
-            url=task_dir,
+            url=task_dir['url'],
             executor=executor.name,
             format=LammpsOutputHelper.format,
-            attrs=dict(
-            ),  # TODO: inherit from input file
+            attrs=task_dir['attrs'],
         ) for task_dir in lammps_task_dirs]  # type: ignore
 
     return GenericLammpsOutput(model_devi_outputs=outputs)
 
 
 def make_md_force_field_section(models: List[str]):
     deepmd_args = ""
@@ -309,26 +320,26 @@
                       trj_freq: int,
                       temp: float,
                       pres: float,
                       tau_t: float,
                       tau_p: float,
                       ensemble: str,
                       mass_map: List[float],
-                      others_dict: Mapping[str, Scalar],
+                      others_dict: Mapping[str, Any],
 
                       template: str,
                       post_variables_section: str,
                       post_init_section: str,
                       post_read_data_section: str,
                       post_force_field_section: str,
                       post_md_section: str,
                       post_run_section: str,
 
                       force_field_section: List[str],
-
+                      plumed_file: Optional[str] = None,
                       no_pbc=False,
                       rand_start=1_000_000,
                       ):
 
     # FIXME: I am not sure if it is a good idea to fix it automatically
     # maybe we should consider raise an error here
     if not ensemble.startswith('npt'):
@@ -374,14 +385,17 @@
     elif ensemble in ('nvt',):
         md_section.append('fix 1 all nvt temp ${TEMP} ${TEMP} ${TAU_T}')
     elif ensemble in ('nve',):
         md_section.append('fix 1 all nve')
     else:
         raise ValueError('unknown ensemble: ' + ensemble)
 
+    if plumed_file:
+        md_section.append(f'fix dpgen_plm all plumed plumedfile {plumed_file} outfile plumed.out')
+
     if no_pbc:
         md_section.extend([
             'velocity all zero linear',
             'fix      fm all momentum 1 linear 1 1 1',
         ])
 
     md_section.extend([
```

### Comparing `ai2_kit-0.3.4/ai2_kit/domain/selector.py` & `ai2_kit-0.3.5/ai2_kit/domain/selector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.4/ai2_kit/main.py` & `ai2_kit-0.3.5/ai2_kit/main.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.4/ai2_kit/tool/ase.py` & `ai2_kit-0.3.5/ai2_kit/tool/ase.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.4/ai2_kit/workflow/cll_mlp.py` & `ai2_kit-0.3.5/ai2_kit/workflow/cll_mlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ai2_kit.core.executor import BaseExecutorConfig
 from ai2_kit.core.artifact import ArtifactMap
 from ai2_kit.core.log import get_logger
 from ai2_kit.core.util import load_yaml_files, merge_dict
 from ai2_kit.core.resource_manager import ResourceManager
-from ai2_kit.core.checkpoint import set_checkpoint_file
+from ai2_kit.core.checkpoint import set_checkpoint_file, apply_checkpoint
 from ai2_kit.domain import (
     deepmd,
     lammps,
     selector,
     cp2k,
     constant as const,
     updater,
@@ -92,14 +92,15 @@
     config = CllWorkflowConfig.parse_obj(config_data)
 
     if executor not in config.executors:
         raise ValueError(f'executor {executor} is not found')
     if path_prefix is None:
         raise ValueError('path_prefix should not be empty')
 
+    cll.init_artifacts(config.artifacts)
     resource_manager = ResourceManager(
         executor_configs=config.executors,
         artifacts=config.artifacts,
         default_executor=executor,
     )
     return asyncio.run(cll_mlp_training_workflow(config, resource_manager, executor, path_prefix))
 
@@ -128,29 +129,31 @@
 
         # shortcut for type_map and mass_map
         type_map = workflow_config.general.type_map
         mass_map = workflow_config.general.mass_map
 
         # decide path prefix for each iteration
         iter_path_prefix = os.path.join(path_prefix, f'iters-{i:03d}')
+        # prefix of checkpoint
+        cp_prefix = f'iters-{i:03d}'
 
         # label
         if workflow_config.label.cp2k:
             cp2k_input = cp2k.GenericCp2kInput(
                 config=workflow_config.label.cp2k,
                 type_map=type_map,
                 system_files=[] if selector_output is None else selector_output.get_model_devi_dataset(),
                 initiated=i > 0,
             )
             cpk2_context = cp2k.GenericCp2kContext(
                 config=context_config.label.cp2k,
                 path_prefix=os.path.join(iter_path_prefix, 'label-cp2k'),
                 resource_manager=resource_manager,
             )
-            label_output = await cp2k.generic_cp2k(cp2k_input, cpk2_context)
+            label_output = await apply_checkpoint(f'{cp_prefix}/label-cp2k')(cp2k.generic_cp2k)(cp2k_input, cpk2_context)
         else:
             raise ValueError('No label method is specified')
 
         # train
         if workflow_config.train.deepmd:
             deepmd_input = deepmd.GenericDeepmdInput(
                 config=workflow_config.train.deepmd,
@@ -160,15 +163,15 @@
                 initiated=i > 0,
             )
             deepmd_context = deepmd.GenericDeepmdContext(
                 path_prefix=os.path.join(iter_path_prefix, 'train-deepmd'),
                 config=context_config.train.deepmd,
                 resource_manager=resource_manager,
             )
-            train_output = await deepmd.generic_deepmd(deepmd_input, deepmd_context)
+            train_output = await apply_checkpoint(f'{cp_prefix}/train-deepmd')(deepmd.generic_deepmd)(deepmd_input, deepmd_context)
         else:
             raise ValueError('No train method is specified')
 
         # explore
         if workflow_config.explore.lammps:
             md_options = lammps.GenericLammpsInput.MdOptions(
                 models=train_output.get_mlp_models(),
@@ -180,30 +183,30 @@
                 md_options=md_options,
             )
             lammps_context = lammps.GenericLammpsContext(
                 path_prefix=os.path.join(iter_path_prefix, 'explore-lammps'),
                 config=context_config.explore.lammps,
                 resource_manager=resource_manager,
             )
-            explore_output = await lammps.generic_lammps(lammps_input, lammps_context)
+            explore_output = await apply_checkpoint(f'{cp_prefix}/explore-lammps')(lammps.generic_lammps)(lammps_input, lammps_context)
         else:
             raise ValueError('No explore method is specified')
 
         # select
         if workflow_config.select.by_threshold:
             selector_input = selector.ThresholdSelectorInput(
                 config=workflow_config.select.by_threshold,
                 model_devi_data=explore_output.get_model_devi_dataset(),
                 model_devi_out_filename=const.MODEL_DEVI_OUT,
             )
             selector_context = selector.ThresholdSelectorContext(
                 path_prefix=os.path.join(iter_path_prefix, 'selector-threshold'),
                 resource_manager=resource_manager,
             )
-            selector_output = await selector.threshold_selector(selector_input, selector_context)
+            selector_output = await apply_checkpoint(f'{cp_prefix}/selector-threshold')(selector.threshold_selector)(selector_input, selector_context)
         else:
             raise ValueError('No select method is specified')
 
         # Update
         update_config = workflow_config.update.walkthrough
 
         # nothing to update because the table is empty
```

### Comparing `ai2_kit-0.3.4/ai2_kit/workflow/fep_mlp.py` & `ai2_kit-0.3.5/ai2_kit/workflow/fep_mlp.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     config = FepWorkflowConfig.parse_obj(config_data)
 
     if executor not in config.executors:
         raise ValueError(f'executor {executor} is not found')
     if path_prefix is None:
         raise ValueError('path_prefix should not be empty')
 
+    cll.init_artifacts(config.artifacts)
     resource_manager = ResourceManager(
         executor_configs=config.executors,
         artifacts=config.artifacts,
         default_executor=executor,
     )
     return asyncio.run(cll_mlp_training_workflow(config, resource_manager, executor, path_prefix))
```

### Comparing `ai2_kit-0.3.4/pyproject.toml` & `ai2_kit-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai2-kit"
-version = "0.3.4"
+version = "0.3.5"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ai2_kit"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `ai2_kit-0.3.4/PKG-INFO` & `ai2_kit-0.3.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai2-kit
-Version: 0.3.4
+Version: 0.3.5
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -24,14 +24,17 @@
 Requires-Dist: pymatgen (>=2023.2.22,<2024.0.0)
 Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
 Requires-Dist: shortuuid (>=1.0.11,<2.0.0)
 Description-Content-Type: text/markdown
 
 # ai<sup>2</sup>-kit
 
+[![PyPI version](https://badge.fury.io/py/ai2-kit.svg)](https://badge.fury.io/py/ai2-kit)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ai2-kit)](https://pypi.org/project/ai2-kit/)
+
 A toolkit featured ***a**rtificial **i**ntelligence × **a**b **i**nitio* for computational chemistry research.
 
 *Please be advised that `ai2-kit` is still under heavy development and you should expect things to change often. We encourage people to play and explore with `ai2-kit`, and stay tuned with us for more features to come.*
 
 
 ## Feature Highlights
 * Collection of tools to facilitate the development of automated workflows for computational chemistry research.
@@ -52,23 +55,22 @@
 
 ```bash
 pip install poetry
 poetry install
 
 ./ai2-kit --help
 ```
+Note that instead of running global `ai2-kit` command, you should run `./ai2-kit` to run the command from source.
 
 ## Manuals
 
 ### Domain Specific Tools
 * [Proton Transfer Analysis Toolkit](doc/manual/proton-transfer.md)
 * [CLL MLP Training Workflow](doc/manual/cll-workflow.md)
 * [FEP MLP Training Workflow](doc/manual/fep-workflow.md)
 
 ### Build-in Functionalities
 * [Checkpoint Mechanism](doc/manual/checkpoint.md)
 * [ASE Toolkit](doc/manual/ase.md)
+* [FAQ](doc/manual/faq.md)
 
-## Tutorials
-
-## Notebooks
```

