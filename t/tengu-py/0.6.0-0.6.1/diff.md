# Comparing `tmp/tengu_py-0.6.0.tar.gz` & `tmp/tengu_py-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tengu_py-0.6.0.tar", max compression
+gzip compressed data, was "tengu_py-0.6.1.tar", max compression
```

## Comparing `tengu_py-0.6.0.tar` & `tengu_py-0.6.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3783 2023-06-23 09:21:14.812532 tengu_py-0.6.0/README.md
--rw-r--r--   0        0        0     1567 2023-06-27 01:56:54.063497 tengu_py-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      175 2023-06-14 09:42:26.699305 tengu_py-0.6.0/tengu/__init__.py
--rw-r--r--   0        0        0    20427 2023-06-27 01:55:42.579287 tengu_py-0.6.0/tengu/api.py
--rw-r--r--   0        0        0     7311 2023-05-31 05:29:35.614982 tengu_py-0.6.0/tengu/calcq.py
--rw-r--r--   0        0        0     4434 2023-05-31 05:29:35.614982 tengu_py-0.6.0/tengu/data.py
--rw-r--r--   0        0        0     7366 2023-06-23 09:23:19.909586 tengu_py-0.6.0/tengu/local.py
--rw-r--r--   0        0        0     4665 1970-01-01 00:00:00.000000 tengu_py-0.6.0/setup.py
--rw-r--r--   0        0        0     4367 1970-01-01 00:00:00.000000 tengu_py-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     3783 2023-06-23 09:21:14.812532 tengu_py-0.6.1/README.md
+-rw-r--r--   0        0        0     1567 2023-06-27 03:25:26.545016 tengu_py-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-06-14 09:42:26.699305 tengu_py-0.6.1/tengu/__init__.py
+-rw-r--r--   0        0        0    20444 2023-06-27 03:24:05.180970 tengu_py-0.6.1/tengu/api.py
+-rw-r--r--   0        0        0     7311 2023-05-31 05:29:35.614982 tengu_py-0.6.1/tengu/calcq.py
+-rw-r--r--   0        0        0     4434 2023-05-31 05:29:35.614982 tengu_py-0.6.1/tengu/data.py
+-rw-r--r--   0        0        0     7366 2023-06-23 09:23:19.909586 tengu_py-0.6.1/tengu/local.py
+-rw-r--r--   0        0        0     4665 1970-01-01 00:00:00.000000 tengu_py-0.6.1/setup.py
+-rw-r--r--   0        0        0     4367 1970-01-01 00:00:00.000000 tengu_py-0.6.1/PKG-INFO
```

### Comparing `tengu_py-0.6.0/README.md` & `tengu_py-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `tengu_py-0.6.0/pyproject.toml` & `tengu_py-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 [tool.setuptools.packages]
 [tool.setuptools.packages.find]
 exclude = ["test", "tests"]
 where = [""]
 
 [tool.poetry]
 name = "tengu-py"
-version = "0.6.0"
+version = "0.6.1"
 description = "Python SDK for interacting with the QDX Tengu API and modules"
 authors = ["Ryan Swart <ryan@talosystems.com>"]
 readme = "README.md"
 packages = [{include = "tengu"}]
 
 [tool.poetry.scripts]
 # tengu = "tengu.__main__:main"
```

### Comparing `tengu_py-0.6.0/tengu/api.py` & `tengu_py-0.6.1/tengu/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
     "method": "MBE",
     "monomer_cutoff": 30,
     "monomer_mp2_cutoff": 30,
     "ngpus_per_node": 4,
     "reference_fragment": 293,
     "trimer_cutoff": 10,
     "trimer_mp2_cutoff": 10,
-    "lattice_energy_calc": True,
+    "lattice_energy_calc": "InteractivityEnergy",
 }
 
 scf_keywords = {
     "convergence_metric": "diis",
     "dynamic_screening_threshold_exp": 10,
     "ndiis": 8,
     "niter": 40,
```

### Comparing `tengu_py-0.6.0/tengu/calcq.py` & `tengu_py-0.6.1/tengu/calcq.py`

 * *Files identical despite different names*

### Comparing `tengu_py-0.6.0/tengu/data.py` & `tengu_py-0.6.1/tengu/data.py`

 * *Files identical despite different names*

### Comparing `tengu_py-0.6.0/tengu/local.py` & `tengu_py-0.6.1/tengu/local.py`

 * *Files identical despite different names*

### Comparing `tengu_py-0.6.0/setup.py` & `tengu_py-0.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['dataclasses-json>=0.5.7,<0.6.0',
  'datargs>=0.11.0,<0.12.0',
  'gql[requests]>=3.4.0,<4.0.0',
  'rdkit-pypi>=2022.9.5,<2023.0.0']
 
 setup_kwargs = {
     'name': 'tengu-py',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': 'Python SDK for interacting with the QDX Tengu API and modules',
     'long_description': '# Tengu-py: Python SDK for the QDX Tengu API\n\nThis package exposes a simple provider and CLI for the different tools exposed by the QDX Tengu GraphQL API.\n\n## Usage\n\n### As a library\n\n``` python\nimport json\nfrom pathlib import Path\n\nimport tengu\n\nTOKEN = "your qdx access token"\n\n# get our client to talk with the API\nclient = tengu.Provider(access_token=TOKEN)\n\n# get newest versions modules that can be run\nmodules = client.latest_modules()\n# or for all modules\nmodules = client.modules()\n\n# get input arguments that need to be provided for module\nprint(modules[0]["ins"])\n\n## running convert\n\n# path to protein pdb with correct charges and protonation\nprotein_pdb = Path("./examples/4w9f_prepared_protein.pdb")\n\n# get base64 encoded data\n\nfile_arg = provider.upload_arg(protein_pdb)\n\nres = client.run("github:talo/tengu-prelude/77e44748f1d1e20c463ef34cc40178d4f656ef0a#convert", [ \nArg(value = "PDB"), file_arg\n])\n\n// res contains "id" - the instance id; and "outs" - the ids of the return values \n\n// we can pass arguments by "id" reference or by value literal\n\nclient.run("github:talo/tengu-prelude/f8e2e55d9bd428aa7f2bbe3f87c24775fa592b10#pick_conformer", [ \nArg( id =  res["outs"][0]["id"] ), Arg( value = 1 ) }\n])\n\nclient.poll_module_instance(id) \n// status, progress, logs, outs - out values will be null until module_instance is done\n```\n\n## Local runner\n\nWe also provide a local executor, that will run modules locally, without making remote calls\n\nFirst, you must have nix installed and configured with an access token for qdx projects.\n\nThen you must install the tengu-runtime with `nix run github:talo/tengu#tengu-runtime -- install`\n\nFinally, you can run locally with\n\n``` python\nfrom tengu import LocalProvider\n\nclient = LocalProvider()\n\n## you should be able to use client.run / client.object / client.module_instance / client.poll_module instance as normal\n```\n\n## Sample QP Run\n\n``` python\nfrag_keywords = {\n    "dimer_cutoff": 25,\n    "dimer_mp2_cutoff": 25,\n    "fragmentation_level": 2,\n    "method": "MBE",\n    "monomer_cutoff": 30,\n    "monomer_mp2_cutoff": 30,\n    "ngpus_per_node": 4,\n    "reference_fragment": 293,\n    "trimer_cutoff": 10,\n    "trimer_mp2_cutoff": 10,\n    "lattice_energy_calc": True,\n}\n\nscf_keywords = {\n    "convergence_metric": "diis",\n    "dynamic_screening_threshold_exp": 10,\n    "ndiis": 8,\n    "niter": 40,\n    "scf_conv": 0.000001,\n}\n\ndefault_model = {"method": "RIMP2", "basis": "cc-pVDZ", "aux_basis": "cc-pVDZ-RIFIT", "frag_enabled": True}\n\nqp_instances = client.qp_run(\n    "github:talo/tengu-prelude/0986e4b23780d5e976e7938dc02a949185090fa1#qp_gen_inputs",\n    "github:talo/tengu-prelude/0986e4b23780d5e976e7938dc02a949185090fa1#hermes_energy",\n    "github:talo/tengu-prelude/0986e4b23780d5e976e7938dc02a949185090fa1#qp_collate",\n    provider.upload_arg(Path("some.pdb")),\n    provider.upload_arg(Path("some.gro")),\n    provider.upload_arg(Path("some.sdf")),\n    Arg(None, "sdf"),\n    Arg(None, "MOL"),\n    Arg(\n        None,\n        default_model,\n    ),\n    Arg(None, {"frag": frag_keywords, "scf": scf_keywords}),\n    Arg(\n        None,\n        [\n            ("GLY", 100), # map of amino acids of interest\n        ],\n    ),\n    "GADI",\n    {"walltime": 420},\n    autopoll = (10, 100) # optionally configure polling to wait on the final instance, \n                         # and clean up if any of the prior instances fails\n)\n\n# if you set autpoll, you will get the results of the qp_collate instance,\n# otherwise you will get an array with all the spawned instances, and have to poll manually\ncompleted_instance = client.poll_module_instance(qp_collate_instance[2]["id"]) \n\n# the result will be an object, so fetch from object store\nclient.object(completed_instance["outs"][0]["id"]) # will return the json qp results\n```\n',
     'author': 'Ryan Swart',
     'author_email': 'ryan@talosystems.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tengu_py-0.6.0/PKG-INFO` & `tengu_py-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tengu-py
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python SDK for interacting with the QDX Tengu API and modules
 Author: Ryan Swart
 Author-email: ryan@talosystems.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

