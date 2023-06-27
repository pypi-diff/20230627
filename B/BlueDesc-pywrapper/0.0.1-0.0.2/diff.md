# Comparing `tmp/BlueDesc_pywrapper-0.0.1.tar.gz` & `tmp/BlueDesc_pywrapper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlueDesc_pywrapper-0.0.1.tar", last modified: Mon Jun 26 22:16:12 2023, max compression
+gzip compressed data, was "BlueDesc_pywrapper-0.0.2.tar", last modified: Tue Jun 27 13:50:35 2023, max compression
```

## Comparing `BlueDesc_pywrapper-0.0.1.tar` & `BlueDesc_pywrapper-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 22:16:12.824229 BlueDesc_pywrapper-0.0.1/
--rw-rw-rw-   0        0        0     1100 2023-06-03 10:58:27.000000 BlueDesc_pywrapper-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2724 2023-06-26 22:16:12.824229 BlueDesc_pywrapper-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1791 2023-06-26 22:13:06.000000 BlueDesc_pywrapper-0.0.1/README.md
--rw-rw-rw-   0        0        0     1323 2023-06-26 22:16:12.826230 BlueDesc_pywrapper-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      123 2023-06-03 10:58:27.000000 BlueDesc_pywrapper-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 22:16:12.799217 BlueDesc_pywrapper-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-26 22:16:12.807216 BlueDesc_pywrapper-0.0.1/src/BlueDesc_pywrapper/
--rw-rw-rw-   0        0        0      142 2023-06-26 22:10:49.000000 BlueDesc_pywrapper-0.0.1/src/BlueDesc_pywrapper/__init__.py
--rw-rw-rw-   0        0        0     7717 2023-06-26 22:13:06.000000 BlueDesc_pywrapper-0.0.1/src/BlueDesc_pywrapper/bluedesc_pywrapper.py
--rw-rw-rw-   0        0        0     3040 2023-06-26 22:05:20.000000 BlueDesc_pywrapper-0.0.1/src/BlueDesc_pywrapper/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-26 22:16:12.823240 BlueDesc_pywrapper-0.0.1/src/BlueDesc_pywrapper.egg-info/
--rw-rw-rw-   0        0        0     2724 2023-06-26 22:16:12.000000 BlueDesc_pywrapper-0.0.1/src/BlueDesc_pywrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-06-26 22:16:12.000000 BlueDesc_pywrapper-0.0.1/src/BlueDesc_pywrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 22:16:12.000000 BlueDesc_pywrapper-0.0.1/src/BlueDesc_pywrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      172 2023-06-26 22:16:12.000000 BlueDesc_pywrapper-0.0.1/src/BlueDesc_pywrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-26 22:16:12.000000 BlueDesc_pywrapper-0.0.1/src/BlueDesc_pywrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 13:50:35.318803 BlueDesc_pywrapper-0.0.2/
+-rw-rw-rw-   0        0        0     1100 2023-06-27 11:18:36.000000 BlueDesc_pywrapper-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3015 2023-06-27 13:50:35.319819 BlueDesc_pywrapper-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2082 2023-06-27 13:48:39.000000 BlueDesc_pywrapper-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1323 2023-06-27 13:50:35.332129 BlueDesc_pywrapper-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      123 2023-06-27 11:18:36.000000 BlueDesc_pywrapper-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:50:35.273000 BlueDesc_pywrapper-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-27 13:50:35.286550 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper/
+-rw-rw-rw-   0        0        0      142 2023-06-27 13:49:37.000000 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper/__init__.py
+-rw-rw-rw-   0        0        0     8450 2023-06-27 13:46:44.000000 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper/bluedesc_pywrapper.py
+-rw-rw-rw-   0        0        0     3040 2023-06-27 11:18:36.000000 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:50:35.317291 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper.egg-info/
+-rw-rw-rw-   0        0        0     3015 2023-06-27 13:50:35.000000 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-06-27 13:50:35.000000 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 13:50:35.000000 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      172 2023-06-27 13:50:35.000000 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-27 13:50:35.000000 BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper.egg-info/top_level.txt
```

### Comparing `BlueDesc_pywrapper-0.0.1/LICENSE` & `BlueDesc_pywrapper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BlueDesc_pywrapper-0.0.1/PKG-INFO` & `BlueDesc_pywrapper-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlueDesc_pywrapper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper for BlueDesc molecular descriptors
 Home-page: https://github.com/OlivierBeq/bluedesc_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: BlueDesc,molecular descriptors,cheminformatics,toxicoinformatics,QSAR
@@ -58,18 +58,23 @@
 for mol in mols:
     _ = AllChem.EmbedMolecule(mol)
 
 bluedesc = BlueDesc()
 print(bluedesc.calculate(mols))
 ```
 
-The above calculates 174 molecular descriptors (33 1D, 85 2D and 56 3D).
-:warning: Molecules are required to have conformers for descriptors to be calculated. 
+The above calculates 174 molecular descriptors (33 1D, 85 2D and 56 3D).<br/>
+:warning: Molecules are required to have conformers for descriptors to be calculated.<br/>
+:warning: BlueDesc skips molecules it cannot parse internally, a warning is given when that is the case.
+The following command is recommended, should this occur, to prevent the unalignment of input and output indices.
 
+```python
+bluedesc.calculate(mols, chunksize=1, njobs=-1)
 ```
+
 ## Documentation
 
 ```python
 def calculate(mols, show_banner=True, njobs=1, chunksize=1000):
 ```
 
 Default method to calculate BlueDesc fingerprints.
```

### Comparing `BlueDesc_pywrapper-0.0.1/README.md` & `BlueDesc_pywrapper-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -36,18 +36,23 @@
 for mol in mols:
     _ = AllChem.EmbedMolecule(mol)
 
 bluedesc = BlueDesc()
 print(bluedesc.calculate(mols))
 ```
 
-The above calculates 174 molecular descriptors (33 1D, 85 2D and 56 3D).
-:warning: Molecules are required to have conformers for descriptors to be calculated. 
+The above calculates 174 molecular descriptors (33 1D, 85 2D and 56 3D).<br/>
+:warning: Molecules are required to have conformers for descriptors to be calculated.<br/>
+:warning: BlueDesc skips molecules it cannot parse internally, a warning is given when that is the case.
+The following command is recommended, should this occur, to prevent the unalignment of input and output indices.
 
+```python
+bluedesc.calculate(mols, chunksize=1, njobs=-1)
 ```
+
 ## Documentation
 
 ```python
 def calculate(mols, show_banner=True, njobs=1, chunksize=1000):
 ```
 
 Default method to calculate BlueDesc fingerprints.
```

### Comparing `BlueDesc_pywrapper-0.0.1/setup.cfg` & `BlueDesc_pywrapper-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `BlueDesc_pywrapper-0.0.1/src/BlueDesc_pywrapper/bluedesc_pywrapper.py` & `BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper/bluedesc_pywrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # -*- coding: utf-8
 
 """Python wrapper for BlueDesc descriptors"""
 
 from __future__ import annotations
 
-import os
+import json
+import more_itertools
 import multiprocessing
-import warnings
+import numpy as np
+import os
+import pandas as pd
 import subprocess
+import warnings
 from copy import deepcopy
 from typing import Iterable, List, Optional
 
-import more_itertools
-import numpy as np
-import pandas as pd
+from BlueDesc import BLUEDESC_EXEC_PATH
 from bounded_pool_executor import BoundedProcessPoolExecutor
 from rdkit import Chem
 from rdkit.rdBase import BlockLogs
 from scipy.io import arff
-from BlueDesc import BLUEDESC_EXEC_PATH
 
 from .utils import install_java, mktempfile, needsHs
 
 
 class BlueDesc:
     """Wrapper to obtain molecular descriptor from BlueDesc."""
 
@@ -44,14 +45,16 @@
         :param show_banner: If True, show notice on fingerprint usage
         :param njobs: number of concurrent processes
         :param chunksize: number of molecules to be processed by a process; ignored if njobs is 1
         :return: a pandas DataFrame containing all BlueDesc descriptor values
         """
         if show_banner:
             self._show_banner()
+        if njobs < 0:
+            njobs = os.cpu_count() - njobs + 1
         # Parallelize should need be
         if njobs > 1:
             with BoundedProcessPoolExecutor(max_workers=njobs) as worker:
                 futures = [worker.submit(self._multiproc_calculate, list(chunk))
                            for chunk in more_itertools.batched(mols, chunksize)
                            ]
             return pd.concat([future.result()
@@ -85,14 +88,15 @@
         """
         # 1) Ensure JRE is accessible
         with self.lock:
             self._java_path = install_java()
         # 2) Create temp SD v2k file
         self._tmp_sd = mktempfile('molecules_v3k.sd')
         self._skipped = []
+        self.n = 0
         try:
             block = BlockLogs()
             writer = Chem.SDWriter(self._tmp_sd)
             # Ensure V2000 as CDK cannot properly process v3000
             writer.SetForceV3000(True)
             for i, mol in enumerate(mols):
                 if mol is not None and isinstance(mol, Chem.Mol):
@@ -104,25 +108,26 @@
                     # Are molecules 3D
                     confs = list(mol.GetConformers())
                     if not (len(confs) > 0 and confs[-1].Is3D()):
                         raise ValueError('Cannot calculate the 3D descriptors of a conformer-less molecule')
                     writer.write(mol)
                 else:
                     self._skipped.append(i)
+                self.n += 1
             writer.close()
             del block
         except ValueError as e:
             # Free resources and raise error
             writer.close()
             del block
             os.remove(self._tmp_sd)
             raise e from None
         # 3) Create command
         java_path = install_java()
-        command = f"{java_path} -jar {self._jarfile} -f {self._tmp_sd} -l \'?\'" #  -Djava.awt.headless=true
+        command = f"{java_path} -jar {self._jarfile} -f {self._tmp_sd} -l \'?\'"
         return command
 
     def _cleanup(self) -> None:
         """Cleanup resources used for calculation."""
         # Remove temporary files
         os.remove(self._tmp_sd)
         os.remove(self._out)
@@ -132,23 +137,33 @@
         """Run the BlueDesc command.
 
         :param command: The command to be run.
         """
         process = subprocess.run(command.split(), stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
         if process.returncode == 0:
             self._out = f'{self._tmp_sd}.oddescriptors.arff'
-            values = arff.loadarff(self._out)
+            try:
+                values = arff.loadarff(self._out)
+                values = (pd.DataFrame(values[0])
+                          .drop("'?'", axis=1)
+                          .rename(columns=lambda x: x.replace('joelib2.feature.types.count.', ''))
+                          .rename(columns=lambda x: x.replace('joelib2.feature.types.', ''))
+                          )
+                if values.shape[0] != self.n:
+                    warnings.warn('Some molecules were skipped by BlueDesc')
+            except:
+                values = np.zeros((self.n, 174))
+                with open(os.path.abspath(os.path.join(__file__, os.pardir, 'desc_names.json'))) as fh:
+                    names = json.load(fh)
+                with open(os.path.abspath(os.path.join(__file__, os.pardir, 'dtypes.json'))) as fh:
+                    dtypes = json.load(fh)
+                values = pd.DataFrame(values, columns=names).astype(dtypes)
         else:
             self._cleanup()
             raise RuntimeError('BlueDesc did not succeed to run properly.')
-        values = (pd.DataFrame(values[0])
-                  .drop("'?'", axis=1)
-                  .rename(columns=lambda x: x.replace('joelib2.feature.types.count.', ''))
-                  .rename(columns=lambda x: x.replace('joelib2.feature.types.', ''))
-                  )
         return values
 
     def _calculate(self, mols: List[Chem.Mol]) -> pd.DataFrame:
         """Calculate BlueDesc molecular descriptors on one process.
 
         :param mols: RDKit molecules for which BlueDesc descriptors should be calculated.
         :return: a pandas DataFrame containing BlueDesc descriptor values
```

### Comparing `BlueDesc_pywrapper-0.0.1/src/BlueDesc_pywrapper/utils.py` & `BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper/utils.py`

 * *Files identical despite different names*

### Comparing `BlueDesc_pywrapper-0.0.1/src/BlueDesc_pywrapper.egg-info/PKG-INFO` & `BlueDesc_pywrapper-0.0.2/src/BlueDesc_pywrapper.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlueDesc-pywrapper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper for BlueDesc molecular descriptors
 Home-page: https://github.com/OlivierBeq/bluedesc_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: BlueDesc,molecular descriptors,cheminformatics,toxicoinformatics,QSAR
@@ -58,18 +58,23 @@
 for mol in mols:
     _ = AllChem.EmbedMolecule(mol)
 
 bluedesc = BlueDesc()
 print(bluedesc.calculate(mols))
 ```
 
-The above calculates 174 molecular descriptors (33 1D, 85 2D and 56 3D).
-:warning: Molecules are required to have conformers for descriptors to be calculated. 
+The above calculates 174 molecular descriptors (33 1D, 85 2D and 56 3D).<br/>
+:warning: Molecules are required to have conformers for descriptors to be calculated.<br/>
+:warning: BlueDesc skips molecules it cannot parse internally, a warning is given when that is the case.
+The following command is recommended, should this occur, to prevent the unalignment of input and output indices.
 
+```python
+bluedesc.calculate(mols, chunksize=1, njobs=-1)
 ```
+
 ## Documentation
 
 ```python
 def calculate(mols, show_banner=True, njobs=1, chunksize=1000):
 ```
 
 Default method to calculate BlueDesc fingerprints.
```

