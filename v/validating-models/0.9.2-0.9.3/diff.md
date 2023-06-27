# Comparing `tmp/validating_models-0.9.2.tar.gz` & `tmp/validating_models-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validating_models-0.9.2.tar", last modified: Mon Mar 13 16:52:05 2023, max compression
+gzip compressed data, was "validating_models-0.9.3.tar", last modified: Tue Jun 27 11:53:42 2023, max compression
```

## Comparing `validating_models-0.9.2.tar` & `validating_models-0.9.3.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:52:05.141615 validating_models-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-03-13 16:51:53.000000 validating_models-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-13 16:51:53.000000 validating_models-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-03-13 16:52:05.137615 validating_models-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-13 16:51:53.000000 validating_models-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 16:52:05.141615 validating_models-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-13 16:51:53.000000 validating_models-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:52:05.133614 validating_models-0.9.2/validating_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    48441 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    43214 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/drawing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23815 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/frequency_distribution_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:52:05.137615 validating_models-0.9.2/validating_models/groupings/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/groupings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/groupings/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/groupings/decision_trees.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/groupings/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/groupings/random_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:52:05.137615 validating_models-0.9.2/validating_models/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/models/decision_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/models/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/shacl_validation_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:52:05.137615 validating_models-0.9.2/validating_models/visualizations/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/visualizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/visualizations/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    29318 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/visualizations/decision_trees.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/visualizations/ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/visualizations/graphviz_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-03-13 16:51:53.000000 validating_models-0.9.2/validating_models/visualizations/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:52:05.133614 validating_models-0.9.2/validating_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-03-13 16:52:05.000000 validating_models-0.9.2/validating_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-03-13 16:52:05.000000 validating_models-0.9.2/validating_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 16:52:05.000000 validating_models-0.9.2/validating_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-13 16:52:05.000000 validating_models-0.9.2/validating_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-13 16:52:05.000000 validating_models-0.9.2/validating_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:53:42.163456 validating_models-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-27 11:53:25.000000 validating_models-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 11:53:25.000000 validating_models-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-27 11:53:42.163456 validating_models-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-27 11:53:25.000000 validating_models-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 11:53:42.163456 validating_models-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-27 11:53:25.000000 validating_models-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:53:42.155456 validating_models-0.9.3/validating_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48649 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43216 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/drawing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23815 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/frequency_distribution_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:53:42.159456 validating_models-0.9.3/validating_models/groupings/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/groupings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/groupings/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/groupings/decision_trees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/groupings/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/groupings/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:53:42.159456 validating_models-0.9.3/validating_models/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/models/decision_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/models/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/shacl_validation_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:53:42.163456 validating_models-0.9.3/validating_models/visualizations/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/visualizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/visualizations/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29424 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/visualizations/decision_trees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/visualizations/ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/visualizations/graphviz_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/visualizations/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:53:42.155456 validating_models-0.9.3/validating_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-27 11:53:42.000000 validating_models-0.9.3/validating_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-27 11:53:42.000000 validating_models-0.9.3/validating_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:53:42.000000 validating_models-0.9.3/validating_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-27 11:53:42.000000 validating_models-0.9.3/validating_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 11:53:42.000000 validating_models-0.9.3/validating_models.egg-info/top_level.txt
```

### Comparing `validating_models-0.9.2/LICENSE` & `validating_models-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.2/PKG-INFO` & `validating_models-0.9.3/validating_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: validating_models
-Version: 0.9.2
+Name: validating-models
+Version: 0.9.3
 Summary: Supporting Explainable AI on Semantic Constraint Validation
 Home-page: https://github.com/JulianLoewe/Validating_Models
-Download-URL: https://github.com/JulianLoewe/Validating_Models/archive/refs/tags/v0.9.2.tar.gz
+Download-URL: https://github.com/JulianLoewe/Validating_Models/archive/refs/tags/v0.9.3.tar.gz
 Author: Julian Gercke
 License: GNU/GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `validating_models-0.9.2/README.md` & `validating_models-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.2/setup.py` & `validating_models-0.9.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 import setuptools
 
-VERSION = '0.9.2'
+VERSION = '0.9.3'
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='validating_models',
     version=VERSION,
@@ -16,15 +16,15 @@
     author='Julian Gercke',
     url='https://github.com/JulianLoewe/Validating_Models',
     download_url='https://github.com/JulianLoewe/Validating_Models/archive/refs/tags/v' + VERSION + '.tar.gz',
     packages=setuptools.find_packages(),
     install_requires=[
         'shaclapi>=0.9.0',
         'cairosvg>=2.5.2',
-        'dtreeviz',
+        'dtreeviz>=2.0.0',
         'matplotlib',
         'numpy',
         'openml',
         'pandas',
         'Pillow',
         'rdflib>=6.1.0',
         'requests',
```

### Comparing `validating_models-0.9.2/validating_models/checker.py` & `validating_models-0.9.3/validating_models/checker.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.2/validating_models/colors.py` & `validating_models-0.9.3/validating_models/colors.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.2/validating_models/constraint.py` & `validating_models-0.9.3/validating_models/constraint.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.2/validating_models/dataset.py` & `validating_models-0.9.3/validating_models/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from functools import lru_cache
 import itertools
 import json
 from pathlib import Path
 
 from .constraint import Constraint, InvertedPredictionConstraint, InvertedShaclSchemaConstraint, PredictionConstraint, ShaclSchemaConstraint
 from .shacl_validation_engine import Communicator,ReducedTravshaclCommunicator
+from .logger import get_logger
 
 import pandas as pd
 import numpy as np
 from sklearn.utils import Bunch
 import re
 
 from typing import Union, List, Mapping
@@ -18,14 +19,16 @@
 from rdflib.plugins import sparql
 
 from validating_models.stats import get_decorator, get_hyperparameter_value, new_entry
 
 time_join = get_decorator('join')
 time_shacl_schema_validation = get_decorator('shacl_schema_validation')
 
+logger = get_logger('validating_models.dataset')
+
 MAX_INSTANCES_IN_FILTER = 200
 DATATYPE_TO_PANDAS_TYPE = {
     'http://www.w3.org/2001/XMLSchema#int': 'numeric',
     'http://www.w3.org/2001/XMLSchema#boolean': 'bool'
 }
 
 TYPE_TO_PANDAS_TYPE = {
@@ -305,15 +308,15 @@
 
         self.seed_query = seed_query
         self.feature_names = list(self.df.columns)
         if self.target_name in self.feature_names:
             self.feature_names.remove(self.target_name)
         if self.seed_var in self.feature_names:
             self.feature_names.remove(self.seed_var)
-        print('Number of unique nodes: ' + str(len(self.get_sample_to_node_mapping().unique())))
+        logger.info('Number of unique nodes: ' + str(len(self.get_sample_to_node_mapping().unique())))
 
     @staticmethod
     def from_knowledge_graph(endpoint, validation_engine: Communicator, data_query: str, target_name: str, seed_var:str = 'x', seed_query: str = None, ground_truth: pd.DataFrame = None, raw_data_query_results_to_df_hook=None, **args):
         """To create the dataset, while generating the task_example_to_node mapping, the dataset has to be retrieved from an endpoint by querying. 
         This is the method, which has to be used if one doesn't has the task_example_to_node mapping locally available.
 
         Parameters
@@ -378,15 +381,15 @@
                     if 'datatype' in value:
                         if value['datatype'] in DATATYPE_TO_PANDAS_TYPE:
                             found_type = DATATYPE_TO_PANDAS_TYPE[value['datatype']]
                     if 'type' in value:
                         if value['type'] in TYPE_TO_PANDAS_TYPE:
                             found_type = TYPE_TO_PANDAS_TYPE[value['type']]
                     if found_type != None:
-                        print(column, found_type)
+                        logger.debug(column + ': ' + found_type)
                         if found_type == 'numeric':
                             df[column] = pd.to_numeric(
                                 df[column], errors='ignore')
                         elif found_type == 'category':
                             categories = list(df[column].unique().astype(str))
                             df[column] = df[column].astype(
                                 pd.CategoricalDtype(categories=categories))
@@ -407,15 +410,15 @@
     def _generate_random_shacl_schema_validation_results(self, constraint):
         p = np.random.random_sample(size=(3,))
         p = p/p.sum()
         random_val_results = np.random.choice(np.array([True, False, None]), size=(len(self.unique_seed_nodes),),p = list(p))
         return {constraint.target_shape: {node: random_val_results[i] for i,node in enumerate(self.unique_seed_nodes) if random_val_results[i] != None}}
 
     def _calculate_shacl_schema_validation_result(self, constraint: Constraint):
-        print(f"Validating SHACL shape schema {constraint.shape_schema_dir} of single constraint with target {constraint.target_shape}")
+        logger.info(f"Validating SHACL shape schema {constraint.shape_schema_dir} of single constraint with target {constraint.target_shape}")
         if self.random_schema_validation:
             val_results = self._generate_random_shacl_schema_validation_results(constraint)
         else:
             val_results = self.communicator.request(
                 self.seed_query, constraint.shape_schema_dir, [constraint.target_shape], self.seed_var)
         
         self.shacl_validation_results[constraint.shacl_identifier] = pd.DataFrame.from_dict(val_results[constraint.target_shape], orient='index', columns=[constraint.shacl_identifier], dtype=bool) 
@@ -477,45 +480,45 @@
                         nodes_to_exclude = set(sample_to_node_mapping[indices_to_exclude].values.unique()).union(dataset.unneeded_seed_nodes)
                         nodes_to_include = dataset.unique_seed_nodes.difference(nodes_to_exclude)                        
                         num_nodes_to_exclude = len(nodes_to_exclude)
                         num_nodes_to_include = len(nodes_to_include)
 
                         if num_nodes_to_exclude < num_nodes_to_include:
                             if num_nodes_to_exclude <= MAX_INSTANCES_IN_FILTER:
-                                print('Adding FILTER clause to reduce the number of results.')
+                                logger.debug('Adding FILTER clause to reduce the number of results.')
                                 filter_clause_per_target_shape[target_shape] = f'FILTER (?{self.seed_var} NOT IN ({",".join([f"<{node}>" for node in nodes_to_exclude])}))'
                             else:
-                                print(f'Skip adding filter clause to {target_shape} because of to many instances ({num_nodes_to_exclude}) to exclude.')
+                                logger.debug(f'Skip adding filter clause to {target_shape} because of to many instances ({num_nodes_to_exclude}) to exclude.')
                                 continue
                         else:
                             if num_nodes_to_include <= MAX_INSTANCES_IN_FILTER:
-                                print('Adding FILTER clause to reduce the number of results.')
+                                logger.debug('Adding FILTER clause to reduce the number of results.')
                                 filter_clause_per_target_shape[target_shape] = f'FILTER (?{self.seed_var} IN ({",".join([f"<{node}>" for node in nodes_to_include])}))'
                             else:
-                                print(f'Skip adding filter clause to {target_shape} because of to many instances ({num_nodes_to_include}) to include.')
+                                logger.debug(f'Skip adding filter clause to {target_shape} because of to many instances ({num_nodes_to_include}) to include.')
                                 continue  
 
                 else:
-                    print('Skip adding filter clause because no checker instance is provided.')
+                    logger.debug('Skip adding filter clause because no checker instance is provided.')
 
-                print(f"Validating {shape_schema_dir} for targets {target_shapes}")
+                logger.info(f"Validating {shape_schema_dir} for targets {target_shapes}")
                 if filter_clause_per_target_shape:
                     try:
                         val_results = self.communicator.request(self.seed_query, shape_schema_dir, target_shapes, self.seed_var, filter_clause_per_target_shape)
                     except:
-                        print('Falling back to not use additional FILTER clauses.')
+                        logger.warning('Falling back to not use additional FILTER clauses.')
                         
                 else:
                     val_results = self.communicator.request(self.seed_query, shape_schema_dir, target_shapes, self.seed_var)
 
                 for target_shape in target_shapes:
                     shacl_identifier = Constraint.get_shacl_identifier(shape_schema_dir, target_shape)
                     self.shacl_validation_results[shacl_identifier] = pd.DataFrame.from_dict(val_results[target_shape], orient='index', columns=[shacl_identifier], dtype=bool) 
 
-                    print("Number of validated targets: " + str(self.shacl_validation_results[shacl_identifier].sum()))
+                    logger.info("Number of validated targets: " + str(self.shacl_validation_results[shacl_identifier].sum()))
         else:
             new_entry('n_unique_nodes',len(self.unique_seed_nodes))
             for constraint in constraints:
                 if constraint.shacl_identifier not in self.shacl_validation_results:
                     self._calculate_shacl_schema_validation_result(constraint)
     
     def get_shacl_schema_validation_results(self, constraints: List[Constraint], indices= None, rename_columns=False, replace_non_applicable_nans=False, checker = None):
@@ -583,45 +586,45 @@
                     result[constraint.shacl_identifier] = result[constraint.shacl_identifier].replace({np.nan: True})
         if rename_columns:
             result = result.rename(columns={constraint.shacl_identifier:constraint.name for constraint in constraints})
         return result
     
     @time_join
     def _index_join_pandas(self, identifiers, class_to_identifier): # left outer join
-        print('Directly joining with the sample to node mapping!')
+        logger.info('Directly joining with the sample to node mapping!')
         for identifier in identifiers:
-            print(f"Joining {identifier}")
+            logger.debug(f"Joining {identifier}")
             self.sample_to_node_mapping = self.sample_to_node_mapping.join(self.shacl_validation_results[identifier], on=self.seed_var)
         return self.sample_to_node_mapping
     
     @time_join
     def _outer_join_pandas(self, identifiers, class_to_identifier):
-        print('Using the outer join')
+        logger.info('Using the outer join')
         if isinstance(identifiers, list) and len(identifiers) == 1:
             identifiers = identifiers.pop()
             return self.sample_to_node_mapping.join(self.shacl_validation_results[identifiers], on=self.seed_var)
         elif isinstance(identifiers, str):
             return self.sample_to_node_mapping.join(self.shacl_validation_results[identifiers], on=self.seed_var)
         else:
             if get_hyperparameter_value('optimize_intermediate_results'):
-                print('Ordering by cardinality')
+                logger.info('Ordering by cardinality')
                 if 'NONE' in class_to_identifier:
                     remaining_identifiers = sorted(list(class_to_identifier['NONE']), key = lambda x: len(self.shacl_validation_results[x]))
                 else:
                     remaining_identifiers = []
                 class_to_identifier = {classe: list(identif) for classe, identif in class_to_identifier.items() if classe != 'NONE'}
                 ordered_classes = sorted(list(class_to_identifier.keys()), key = lambda x: len(self.shacl_validation_results[class_to_identifier[x][0]]))
                 identifiers = list(itertools.chain.from_iterable([class_to_identifier[classe] for classe in ordered_classes])) + remaining_identifiers
             
             #print([(identifier, len(self.shacl_validation_results[identifier])) for identifier in identifiers])
 
             first_key = identifiers.pop() # shacl results are joined first with full outer join and afterwards joined with the mapping with a left outer join
             
             if get_hyperparameter_value('not_pandas_optimized'):
-                print('Using not pandas optimized join')
+                logger.debug('Using not pandas optimized join')
                 result = self.shacl_validation_results[first_key]
                 for key in identifiers:
                     result = result.join(self.shacl_validation_results[key], how='outer')
                     
                 return self.sample_to_node_mapping.join(result, on=self.seed_var)
             
             return self.sample_to_node_mapping.join(self.shacl_validation_results[first_key].join([self.shacl_validation_results[key] for key in identifiers], how='outer'), on=self.seed_var)
@@ -690,16 +693,16 @@
         self.feature_names = list(self.df.columns)
         if self.target_name in self.feature_names:
             self.feature_names.remove(self.target_name)
         if self.seed_var in self.feature_names:
             self.feature_names.remove(self.seed_var)
         self.unique_seed_nodes = set(self.get_sample_to_node_mapping().unique())
         self.unneeded_seed_nodes = self.base.unique_seed_nodes - self.unique_seed_nodes
-        print(f'Identified {len(self.unique_seed_nodes)} unique seed nodes!')
-        print(f'In comparison to the BaseDataset this makes a total of {len(self.unneeded_seed_nodes)} unneeded seed nodes!')
+        logger.info(f'Identified {len(self.unique_seed_nodes)} unique seed nodes!')
+        logger.info(f'In comparison to the BaseDataset this makes a total of {len(self.unneeded_seed_nodes)} unneeded seed nodes!')
     
     @staticmethod
     def from_unchanged_index(processed_df: pd.DataFrame, base: BaseDataset, target_name: str = None, categorical_mapping=None):
         """Creates the ProcessedDataset from a Dataframe with the index structure kept intact. For the datasets, this means that a given index refers to the semantically indentical samples (which therefor refer to the same seed node in the knowledge graph).
         E.g. :math:`\\forall i ((\\text{processed\_df}[i] \\rightarrow seednode_1) \land (\\text{base.df}[i] \\rightarrow seednode_2)) \implies seednode_1 = seednode_2`
```

### Comparing `validating_models-0.9.2/validating_models/drawing_utils.py` & `validating_models-0.9.3/validating_models/drawing_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
                  proxy_artists=None,
                  fontname='DejaVu Sans',
                  fontsize=14,
                  graph_colors=None,
                  data_std=None) -> None:
         self._data = data
         if isinstance(data_std, list):
-            print('std given')
+            # print('std given')
             self._data_std = data_std
         else:
             self._data_std = [np.zeros_like(self._data[0]) for i in range(len(self._data))]
         self._num_groups = self._data[0].shape[0]
         self._num_bars_per_group = self._data[0].shape[1]
         super().__init__(figure_size, ax, proxy_artists, fontname, fontsize, graph_colors)
```

### Comparing `validating_models-0.9.2/validating_models/frequency_distribution_table.py` & `validating_models-0.9.3/validating_models/frequency_distribution_table.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.2/validating_models/groupings/classification.py` & `validating_models-0.9.3/validating_models/groupings/classification.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.2/validating_models/groupings/decision_trees.py` & `validating_models-0.9.3/validating_models/groupings/decision_trees.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.2/validating_models/groupings/general.py` & `validating_models-0.9.3/validating_models/groupings/general.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.2/validating_models/groupings/random_forest.py` & `validating_models-0.9.3/validating_models/groupings/random_forest.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.2/validating_models/models/decision_tree.py` & `validating_models-0.9.3/validating_models/models/decision_tree.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from dtreeviz.models.shadow_decision_tree import ShadowDecTree, ShadowDecTreeNode
 from validating_models.stats import get_decorator, get_hyperparameter_value, new_entry
+from validating_models.logger import get_logger
 
+logger = get_logger('validating_models.models.decision_tree')
 time_node_samples = get_decorator('node_samples')
 
 def get_shadow_tree_from_checker(model, checker, tree_index=None) -> ShadowDecTree:
     dataset = checker.dataset
     return ShadowDecTree.get_shadow_tree(model, x_data=dataset.x_data(), y_data=dataset.y_data(), feature_names=dataset.feature_names, target_name=dataset.target_name, class_names=dataset.class_names, tree_index=tree_index)
 
 
@@ -25,23 +27,23 @@
         return get_node_samples(tree)[node.id]
 
 
 @time_node_samples
 def get_node_samples(tree: ShadowDecTree):
     result = None
     if tree.node_to_samples is not None:
-        print('Reusing Node_samples!')
+        logger.info('Reusing Node_samples!')
         result = tree.node_to_samples
     else:
         if get_hyperparameter_value('node_to_samples_non_optimized'):
-            print('Using non optimized node_samples on purpose!')
+            logger.info('Using non optimized node_samples on purpose!')
             result = tree.get_node_samples()
         else:
             try:
-                print('Calculating node samples!')
+                logger.info('Calculating node samples!')
                 dec_paths = tree.tree_model.decision_path(tree.x_data)
                 dec_paths = dec_paths.tocsc()
 
                 n_nodes = dec_paths.shape[1]
                 node_to_samples = {}
                 for node_id in range(n_nodes):
                     node_to_samples[node_id] = list(dec_paths[:,node_id].nonzero()[0])
```

### Comparing `validating_models-0.9.2/validating_models/models/random_forest.py` & `validating_models-0.9.3/validating_models/models/random_forest.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.2/validating_models/shacl_validation_engine.py` & `validating_models-0.9.3/validating_models/shacl_validation_engine.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.2/validating_models/stats.py` & `validating_models-0.9.3/validating_models/stats.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.2/validating_models/visualizations/classification.py` & `validating_models-0.9.3/validating_models/visualizations/classification.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.2/validating_models/visualizations/decision_trees.py` & `validating_models-0.9.3/validating_models/visualizations/decision_trees.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,24 +10,27 @@
 from ..constraint import TRUTH_LABELS, Constraint
 from ..drawing_utils import Function, Scatter, extract_labels_handles, new_draw_legend
 from ..colors import VAL_COLORS, adjust_colors
 
 from ..groupings.general import group_by_complete_dataset
 from ..groupings.decision_trees import group_by_decision_tree_leaves, group_by_decision_tree_nodes, group_by_node_split_feature
 from .regression import get_feature_target_for_indices_plot
+from ..logger import get_logger
 from ..models.decision_tree import get_shadow_tree_from_checker, get_node_samples, get_single_node_samples
 from dtreeviz.models.shadow_decision_tree import ShadowDecTreeNode
 from ..visualizations.graphviz_helper import DTreeVizConv
 from dtreeviz.utils import myround
 from tqdm import tqdm
 import multiprocessing as mp
 from pebble import ProcessPool
 
 from validating_models.stats import get_process_stats_initalizer_args, process_stats_initializer
 
+logger = get_logger('validating_models.visualizations.ensembles')
+
 ##################################################################
 # Plots based on constraint validation counts:                   #
 # Regression                                                     #
 ##################################################################
 
 def get_kde_plot(node: ShadowDecTreeNode,
                  checker: Checker,
@@ -532,15 +535,15 @@
 
     if use_node_predictions:
         checker_per_prediction = {}
         for y in np.unique(checker.dataset.y_data()):
             checker_per_prediction[y] = ConstantModelChecker(y, checker.dataset, use_gt=checker._use_gt)
             checker_per_prediction[y].validate(constraints)
 
-    print(f'Using {mp.cpu_count() if visualize_in_parallel else 1} worker(s)!')
+    logger.debug(f'Using {mp.cpu_count() if visualize_in_parallel else 1} worker(s)!')
     with ProcessPool(max_workers=mp.cpu_count(),context=mp.get_context('spawn'), initializer=process_stats_initializer, initargs=get_process_stats_initalizer_args()) as pool:
         for i, node in enumerate(tqdm(nodes_to_plot)):
             if use_node_predictions:
                 handles_or_args = generate_node_plot(node, visualize_in_parallel, shadow_tree, checker_per_prediction[node.shadow_tree.get_prediction(node.id)], constraints, non_applicable_counts, depth_range_to_display, coverage, use_node_predictions, label_fontsize, leaf_grouping_function, node_samples, tmp, os.getpid())
             else:
                 handles_or_args = generate_node_plot(node, visualize_in_parallel, shadow_tree, checker, constraints, non_applicable_counts, depth_range_to_display, coverage, use_node_predictions, label_fontsize, leaf_grouping_function, node_samples, tmp, os.getpid())
             tasks_left.append(handles_or_args)
```

### Comparing `validating_models-0.9.2/validating_models/visualizations/ensembles.py` & `validating_models-0.9.3/validating_models/visualizations/ensembles.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,368 +26,374 @@
 00000190: 6f72 730a 6672 6f6d 202e 2e63 6f6e 7374  ors.from ..const
 000001a0: 7261 696e 7420 696d 706f 7274 2043 6f6e  raint import Con
 000001b0: 7374 7261 696e 740a 696d 706f 7274 206e  straint.import n
 000001c0: 756d 7079 2061 7320 6e70 0a66 726f 6d20  umpy as np.from 
 000001d0: 2e2e 6772 6f75 7069 6e67 732e 636c 6173  ..groupings.clas
 000001e0: 7369 6669 6361 7469 6f6e 2069 6d70 6f72  sification impor
 000001f0: 7420 6772 6f75 705f 6279 5f67 745f 636c  t group_by_gt_cl
-00000200: 6173 730a 6672 6f6d 202e 2e6d 6f64 656c  ass.from ..model
-00000210: 732e 7261 6e64 6f6d 5f66 6f72 6573 7420  s.random_forest 
-00000220: 696d 706f 7274 2067 6574 5f73 6861 646f  import get_shado
-00000230: 775f 666f 7265 7374 5f66 726f 6d5f 6368  w_forest_from_ch
-00000240: 6563 6b65 720a 6672 6f6d 202e 2e6d 6f64  ecker.from ..mod
-00000250: 656c 732e 6465 6369 7369 6f6e 5f74 7265  els.decision_tre
-00000260: 6520 696d 706f 7274 2067 6574 5f73 6861  e import get_sha
-00000270: 646f 775f 7472 6565 5f66 726f 6d5f 6368  dow_tree_from_ch
-00000280: 6563 6b65 720a 6672 6f6d 202e 2e67 726f  ecker.from ..gro
-00000290: 7570 696e 6773 2e67 656e 6572 616c 2069  upings.general i
-000002a0: 6d70 6f72 7420 6772 6f75 705f 6279 5f63  mport group_by_c
-000002b0: 6f6d 706c 6574 655f 6461 7461 7365 740a  omplete_dataset.
-000002c0: 6672 6f6d 202e 2e64 7261 7769 6e67 5f75  from ..drawing_u
-000002d0: 7469 6c73 2069 6d70 6f72 7420 6472 6177  tils import draw
-000002e0: 5f6c 6567 656e 640a 6672 6f6d 202e 2e66  _legend.from ..f
-000002f0: 7265 7175 656e 6379 5f64 6973 7472 6962  requency_distrib
-00000300: 7574 696f 6e5f 7461 626c 6520 696d 706f  ution_table impo
-00000310: 7274 2046 7265 7175 656e 6379 4469 7374  rt FrequencyDist
-00000320: 7269 6275 7469 6f6e 5461 626c 650a 6672  ributionTable.fr
-00000330: 6f6d 202e 2e76 6973 7561 6c69 7a61 7469  om ..visualizati
-00000340: 6f6e 7320 696d 706f 7274 2067 7261 7068  ons import graph
-00000350: 7669 7a5f 6865 6c70 6572 200a 6672 6f6d  viz_helper .from
-00000360: 202e 2e76 6973 7561 6c69 7a61 7469 6f6e   ..visualization
-00000370: 7320 696d 706f 7274 2064 6563 6973 696f  s import decisio
-00000380: 6e5f 7472 6565 730a 6672 6f6d 2074 7164  n_trees.from tqd
-00000390: 6d20 696d 706f 7274 2074 7164 6d0a 6672  m import tqdm.fr
-000003a0: 6f6d 202e 2e6d 6f64 656c 732e 6465 6369  om ..models.deci
-000003b0: 7369 6f6e 5f74 7265 6520 696d 706f 7274  sion_tree import
-000003c0: 2067 6574 5f73 696e 676c 655f 6e6f 6465   get_single_node
-000003d0: 5f73 616d 706c 6573 0a0a 6465 6620 6e6f  _samples..def no
-000003e0: 6465 5f6e 616d 6528 6929 3a0a 2020 2020  de_name(i):.    
-000003f0: 7265 7475 726e 2066 2765 7374 696d 6174  return f'estimat
-00000400: 6f72 7b69 7d27 0a0a 6465 6620 6669 785f  or{i}'..def fix_
-00000410: 7376 675f 6669 6c65 2870 6174 6829 3a0a  svg_file(path):.
-00000420: 2020 2020 6d69 7373 696e 675f 6865 6164      missing_head
-00000430: 6572 203d 2027 3c3f 786d 6c20 7665 7273  er = '<?xml vers
-00000440: 696f 6e3d 2231 2e30 2220 656e 636f 6469  ion="1.0" encodi
-00000450: 6e67 3d22 7574 662d 3822 2073 7461 6e64  ng="utf-8" stand
-00000460: 616c 6f6e 653d 226e 6f22 3f3e 5c6e 3c21  alone="no"?>\n<!
-00000470: 444f 4354 5950 4520 7376 6720 5055 424c  DOCTYPE svg PUBL
-00000480: 4943 2022 2d2f 2f57 3343 2f2f 4454 4420  IC "-//W3C//DTD 
-00000490: 5356 4720 312e 312f 2f45 4e22 2022 6874  SVG 1.1//EN" "ht
-000004a0: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
-000004b0: 4772 6170 6869 6373 2f53 5647 2f31 2e31  Graphics/SVG/1.1
-000004c0: 2f44 5444 2f73 7667 3131 2e64 7464 223e  /DTD/svg11.dtd">
-000004d0: 5c6e 270a 2020 2020 7769 7468 206f 7065  \n'.    with ope
-000004e0: 6e28 7061 7468 2c20 2772 2729 2061 7320  n(path, 'r') as 
-000004f0: 6f72 6967 696e 616c 3a0a 2020 2020 2020  original:.      
-00000500: 2020 7376 675f 636f 6e74 656e 7420 3d20    svg_content = 
-00000510: 6f72 6967 696e 616c 2e72 6561 6428 290a  original.read().
-00000520: 2020 2020 0a20 2020 2077 6974 6820 6f70      .    with op
-00000530: 656e 2870 6174 682c 2027 7727 2920 6173  en(path, 'w') as
-00000540: 206e 6577 3a0a 2020 2020 2020 2020 6e65   new:.        ne
-00000550: 772e 7772 6974 6528 6d69 7373 696e 675f  w.write(missing_
-00000560: 6865 6164 6572 290a 2020 2020 2020 2020  header).        
-00000570: 6e65 772e 7772 6974 6528 7376 675f 636f  new.write(svg_co
-00000580: 6e74 656e 7429 0a0a 6465 6620 6772 6f75  ntent)..def grou
-00000590: 705f 7265 7375 6c74 735f 6279 5f63 6c75  p_results_by_clu
-000005a0: 7374 6572 696e 6728 5829 3a0a 2020 2020  stering(X):.    
-000005b0: 6672 6f6d 2073 6b6c 6561 726e 2e63 6c75  from sklearn.clu
-000005c0: 7374 6572 2069 6d70 6f72 7420 4b4d 6561  ster import KMea
-000005d0: 6e73 0a20 2020 2066 726f 6d20 736b 6c65  ns.    from skle
-000005e0: 6172 6e2e 6d65 7472 6963 7320 696d 706f  arn.metrics impo
-000005f0: 7274 2073 696c 686f 7565 7474 655f 7363  rt silhouette_sc
-00000600: 6f72 650a 2020 2020 7363 6f72 6573 203d  ore.    scores =
-00000610: 205b 5d0a 2020 2020 616c 6c5f 6c61 6265   [].    all_labe
-00000620: 6c73 203d 205b 5d0a 2020 2020 756e 6971  ls = [].    uniq
-00000630: 7565 5f73 616d 706c 6573 203d 206e 702e  ue_samples = np.
-00000640: 756e 6971 7565 2858 2c61 7869 733d 3029  unique(X,axis=0)
-00000650: 0a20 2020 2069 6620 756e 6971 7565 5f73  .    if unique_s
-00000660: 616d 706c 6573 2e73 6861 7065 5b30 5d20  amples.shape[0] 
-00000670: 3e3d 2032 3a0a 2020 2020 2020 2020 666f  >= 2:.        fo
-00000680: 7220 6920 696e 2074 7164 6d28 7261 6e67  r i in tqdm(rang
-00000690: 6528 322c 756e 6971 7565 5f73 616d 706c  e(2,unique_sampl
-000006a0: 6573 2e73 6861 7065 5b30 5d20 2b20 3129  es.shape[0] + 1)
-000006b0: 2c64 6573 633d 2747 7269 6420 5365 6172  ,desc='Grid Sear
-000006c0: 6368 2066 6f72 2062 6573 7420 636c 7573  ch for best clus
-000006d0: 7465 7269 6e67 2729 3a0a 2020 2020 2020  tering'):.      
-000006e0: 2020 2020 2020 6c61 6265 6c73 203d 204b        labels = K
-000006f0: 4d65 616e 7328 6e5f 636c 7573 7465 7273  Means(n_clusters
-00000700: 3d69 292e 6669 745f 7072 6564 6963 7428  =i).fit_predict(
-00000710: 5829 0a20 2020 2020 2020 2020 2020 2074  X).            t
-00000720: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00000730: 2020 2020 7363 6f72 6573 2e61 7070 656e      scores.appen
-00000740: 6428 7369 6c68 6f75 6574 7465 5f73 636f  d(silhouette_sco
-00000750: 7265 2858 2c20 6c61 6265 6c73 2929 0a20  re(X, labels)). 
-00000760: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00000770: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-00000780: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-00000790: 2020 2020 2020 2020 616c 6c5f 6c61 6265          all_labe
-000007a0: 6c73 2e61 7070 656e 6428 6c61 6265 6c73  ls.append(labels
-000007b0: 290a 2020 2020 2020 2020 6265 7374 5f69  ).        best_i
-000007c0: 6478 203d 206e 702e 6172 676d 6178 286e  dx = np.argmax(n
-000007d0: 702e 6172 7261 7928 7363 6f72 6573 2929  p.array(scores))
-000007e0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-000007f0: 4265 7374 2053 696c 686f 7565 7474 6520  Best Silhouette 
-00000800: 5363 6f72 653a 2022 202b 2073 7472 286e  Score: " + str(n
-00000810: 702e 6d61 7828 6e70 2e61 7272 6179 2873  p.max(np.array(s
-00000820: 636f 7265 7329 2929 290a 2020 2020 656c  cores)))).    el
-00000830: 7365 3a0a 2020 2020 2020 2020 7265 7475  se:.        retu
-00000840: 726e 206e 702e 7a65 726f 7328 2858 2e73  rn np.zeros((X.s
-00000850: 6861 7065 5b30 5d2c 2929 2c20 310a 2020  hape[0],)), 1.  
-00000860: 2020 7265 7475 726e 2061 6c6c 5f6c 6162    return all_lab
-00000870: 656c 735b 6265 7374 5f69 6478 5d2c 2062  els[best_idx], b
-00000880: 6573 745f 6964 7820 2b20 3220 0a0a 0a64  est_idx + 2 ...d
-00000890: 6566 2072 616e 646f 6d5f 666f 7265 7374  ef random_forest
-000008a0: 5f76 697a 286d 6f64 656c 2c0a 2020 2020  _viz(model,.    
-000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008c0: 6368 6563 6b65 723a 2043 6865 636b 6572  checker: Checker
-000008d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000008e0: 2020 2020 2020 636f 6e73 7472 6169 6e74        constraint
-000008f0: 733a 204c 6973 745b 436f 6e73 7472 6169  s: List[Constrai
-00000900: 6e74 5d2c 0a20 2020 2020 2020 2020 2020  nt],.           
-00000910: 2020 2020 2020 2020 2067 726f 7570 5f66           group_f
-00000920: 756e 6374 696f 6e73 203d 2067 726f 7570  unctions = group
-00000930: 5f62 795f 6774 5f63 6c61 7373 2c0a 2020  _by_gt_class,.  
+00000200: 6173 730a 6672 6f6d 202e 2e6c 6f67 6765  ass.from ..logge
+00000210: 7220 696d 706f 7274 2067 6574 5f6c 6f67  r import get_log
+00000220: 6765 720a 6672 6f6d 202e 2e6d 6f64 656c  ger.from ..model
+00000230: 732e 7261 6e64 6f6d 5f66 6f72 6573 7420  s.random_forest 
+00000240: 696d 706f 7274 2067 6574 5f73 6861 646f  import get_shado
+00000250: 775f 666f 7265 7374 5f66 726f 6d5f 6368  w_forest_from_ch
+00000260: 6563 6b65 720a 6672 6f6d 202e 2e6d 6f64  ecker.from ..mod
+00000270: 656c 732e 6465 6369 7369 6f6e 5f74 7265  els.decision_tre
+00000280: 6520 696d 706f 7274 2067 6574 5f73 6861  e import get_sha
+00000290: 646f 775f 7472 6565 5f66 726f 6d5f 6368  dow_tree_from_ch
+000002a0: 6563 6b65 720a 6672 6f6d 202e 2e67 726f  ecker.from ..gro
+000002b0: 7570 696e 6773 2e67 656e 6572 616c 2069  upings.general i
+000002c0: 6d70 6f72 7420 6772 6f75 705f 6279 5f63  mport group_by_c
+000002d0: 6f6d 706c 6574 655f 6461 7461 7365 740a  omplete_dataset.
+000002e0: 6672 6f6d 202e 2e64 7261 7769 6e67 5f75  from ..drawing_u
+000002f0: 7469 6c73 2069 6d70 6f72 7420 6472 6177  tils import draw
+00000300: 5f6c 6567 656e 640a 6672 6f6d 202e 2e66  _legend.from ..f
+00000310: 7265 7175 656e 6379 5f64 6973 7472 6962  requency_distrib
+00000320: 7574 696f 6e5f 7461 626c 6520 696d 706f  ution_table impo
+00000330: 7274 2046 7265 7175 656e 6379 4469 7374  rt FrequencyDist
+00000340: 7269 6275 7469 6f6e 5461 626c 650a 6672  ributionTable.fr
+00000350: 6f6d 202e 2e76 6973 7561 6c69 7a61 7469  om ..visualizati
+00000360: 6f6e 7320 696d 706f 7274 2067 7261 7068  ons import graph
+00000370: 7669 7a5f 6865 6c70 6572 200a 6672 6f6d  viz_helper .from
+00000380: 202e 2e76 6973 7561 6c69 7a61 7469 6f6e   ..visualization
+00000390: 7320 696d 706f 7274 2064 6563 6973 696f  s import decisio
+000003a0: 6e5f 7472 6565 730a 6672 6f6d 2074 7164  n_trees.from tqd
+000003b0: 6d20 696d 706f 7274 2074 7164 6d0a 6672  m import tqdm.fr
+000003c0: 6f6d 202e 2e6d 6f64 656c 732e 6465 6369  om ..models.deci
+000003d0: 7369 6f6e 5f74 7265 6520 696d 706f 7274  sion_tree import
+000003e0: 2067 6574 5f73 696e 676c 655f 6e6f 6465   get_single_node
+000003f0: 5f73 616d 706c 6573 0a0a 6c6f 6767 6572  _samples..logger
+00000400: 203d 2067 6574 5f6c 6f67 6765 7228 2776   = get_logger('v
+00000410: 616c 6964 6174 696e 675f 6d6f 6465 6c73  alidating_models
+00000420: 2e76 6973 7561 6c69 7a61 7469 6f6e 732e  .visualizations.
+00000430: 656e 7365 6d62 6c65 7327 290a 0a64 6566  ensembles')..def
+00000440: 206e 6f64 655f 6e61 6d65 2869 293a 0a20   node_name(i):. 
+00000450: 2020 2072 6574 7572 6e20 6627 6573 7469     return f'esti
+00000460: 6d61 746f 727b 697d 270a 0a64 6566 2066  mator{i}'..def f
+00000470: 6978 5f73 7667 5f66 696c 6528 7061 7468  ix_svg_file(path
+00000480: 293a 0a20 2020 206d 6973 7369 6e67 5f68  ):.    missing_h
+00000490: 6561 6465 7220 3d20 273c 3f78 6d6c 2076  eader = '<?xml v
+000004a0: 6572 7369 6f6e 3d22 312e 3022 2065 6e63  ersion="1.0" enc
+000004b0: 6f64 696e 673d 2275 7466 2d38 2220 7374  oding="utf-8" st
+000004c0: 616e 6461 6c6f 6e65 3d22 6e6f 223f 3e5c  andalone="no"?>\
+000004d0: 6e3c 2144 4f43 5459 5045 2073 7667 2050  n<!DOCTYPE svg P
+000004e0: 5542 4c49 4320 222d 2f2f 5733 432f 2f44  UBLIC "-//W3C//D
+000004f0: 5444 2053 5647 2031 2e31 2f2f 454e 2220  TD SVG 1.1//EN" 
+00000500: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
+00000510: 7267 2f47 7261 7068 6963 732f 5356 472f  rg/Graphics/SVG/
+00000520: 312e 312f 4454 442f 7376 6731 312e 6474  1.1/DTD/svg11.dt
+00000530: 6422 3e5c 6e27 0a20 2020 2077 6974 6820  d">\n'.    with 
+00000540: 6f70 656e 2870 6174 682c 2027 7227 2920  open(path, 'r') 
+00000550: 6173 206f 7269 6769 6e61 6c3a 0a20 2020  as original:.   
+00000560: 2020 2020 2073 7667 5f63 6f6e 7465 6e74       svg_content
+00000570: 203d 206f 7269 6769 6e61 6c2e 7265 6164   = original.read
+00000580: 2829 0a20 2020 200a 2020 2020 7769 7468  ().    .    with
+00000590: 206f 7065 6e28 7061 7468 2c20 2777 2729   open(path, 'w')
+000005a0: 2061 7320 6e65 773a 0a20 2020 2020 2020   as new:.       
+000005b0: 206e 6577 2e77 7269 7465 286d 6973 7369   new.write(missi
+000005c0: 6e67 5f68 6561 6465 7229 0a20 2020 2020  ng_header).     
+000005d0: 2020 206e 6577 2e77 7269 7465 2873 7667     new.write(svg
+000005e0: 5f63 6f6e 7465 6e74 290a 0a64 6566 2067  _content)..def g
+000005f0: 726f 7570 5f72 6573 756c 7473 5f62 795f  roup_results_by_
+00000600: 636c 7573 7465 7269 6e67 2858 293a 0a20  clustering(X):. 
+00000610: 2020 2066 726f 6d20 736b 6c65 6172 6e2e     from sklearn.
+00000620: 636c 7573 7465 7220 696d 706f 7274 204b  cluster import K
+00000630: 4d65 616e 730a 2020 2020 6672 6f6d 2073  Means.    from s
+00000640: 6b6c 6561 726e 2e6d 6574 7269 6373 2069  klearn.metrics i
+00000650: 6d70 6f72 7420 7369 6c68 6f75 6574 7465  mport silhouette
+00000660: 5f73 636f 7265 0a20 2020 2073 636f 7265  _score.    score
+00000670: 7320 3d20 5b5d 0a20 2020 2061 6c6c 5f6c  s = [].    all_l
+00000680: 6162 656c 7320 3d20 5b5d 0a20 2020 2075  abels = [].    u
+00000690: 6e69 7175 655f 7361 6d70 6c65 7320 3d20  nique_samples = 
+000006a0: 6e70 2e75 6e69 7175 6528 582c 6178 6973  np.unique(X,axis
+000006b0: 3d30 290a 2020 2020 6966 2075 6e69 7175  =0).    if uniqu
+000006c0: 655f 7361 6d70 6c65 732e 7368 6170 655b  e_samples.shape[
+000006d0: 305d 203e 3d20 323a 0a20 2020 2020 2020  0] >= 2:.       
+000006e0: 2066 6f72 2069 2069 6e20 7471 646d 2872   for i in tqdm(r
+000006f0: 616e 6765 2832 2c75 6e69 7175 655f 7361  ange(2,unique_sa
+00000700: 6d70 6c65 732e 7368 6170 655b 305d 202b  mples.shape[0] +
+00000710: 2031 292c 6465 7363 3d27 4772 6964 2053   1),desc='Grid S
+00000720: 6561 7263 6820 666f 7220 6265 7374 2063  earch for best c
+00000730: 6c75 7374 6572 696e 6727 293a 0a20 2020  lustering'):.   
+00000740: 2020 2020 2020 2020 206c 6162 656c 7320           labels 
+00000750: 3d20 4b4d 6561 6e73 286e 5f63 6c75 7374  = KMeans(n_clust
+00000760: 6572 733d 6929 2e66 6974 5f70 7265 6469  ers=i).fit_predi
+00000770: 6374 2858 290a 2020 2020 2020 2020 2020  ct(X).          
+00000780: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00000790: 2020 2020 2020 2073 636f 7265 732e 6170         scores.ap
+000007a0: 7065 6e64 2873 696c 686f 7565 7474 655f  pend(silhouette_
+000007b0: 7363 6f72 6528 582c 206c 6162 656c 7329  score(X, labels)
+000007c0: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
+000007d0: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
+000007e0: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+000007f0: 2020 2020 2020 2020 2020 2061 6c6c 5f6c             all_l
+00000800: 6162 656c 732e 6170 7065 6e64 286c 6162  abels.append(lab
+00000810: 656c 7329 0a20 2020 2020 2020 2062 6573  els).        bes
+00000820: 745f 6964 7820 3d20 6e70 2e61 7267 6d61  t_idx = np.argma
+00000830: 7828 6e70 2e61 7272 6179 2873 636f 7265  x(np.array(score
+00000840: 7329 290a 2020 2020 2020 2020 6c6f 6767  s)).        logg
+00000850: 6572 2e64 6562 7567 2822 4265 7374 2053  er.debug("Best S
+00000860: 696c 686f 7565 7474 6520 5363 6f72 653a  ilhouette Score:
+00000870: 2022 202b 2073 7472 286e 702e 6d61 7828   " + str(np.max(
+00000880: 6e70 2e61 7272 6179 2873 636f 7265 7329  np.array(scores)
+00000890: 2929 290a 2020 2020 656c 7365 3a0a 2020  ))).    else:.  
+000008a0: 2020 2020 2020 7265 7475 726e 206e 702e        return np.
+000008b0: 7a65 726f 7328 2858 2e73 6861 7065 5b30  zeros((X.shape[0
+000008c0: 5d2c 2929 2c20 310a 2020 2020 7265 7475  ],)), 1.    retu
+000008d0: 726e 2061 6c6c 5f6c 6162 656c 735b 6265  rn all_labels[be
+000008e0: 7374 5f69 6478 5d2c 2062 6573 745f 6964  st_idx], best_id
+000008f0: 7820 2b20 3220 0a0a 0a64 6566 2072 616e  x + 2 ...def ran
+00000900: 646f 6d5f 666f 7265 7374 5f76 697a 286d  dom_forest_viz(m
+00000910: 6f64 656c 2c0a 2020 2020 2020 2020 2020  odel,.          
+00000920: 2020 2020 2020 2020 2020 6368 6563 6b65            checke
+00000930: 723a 2043 6865 636b 6572 2c0a 2020 2020  r: Checker,.    
 00000940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000950: 2020 636f 7665 7261 6765 3a20 626f 6f6c    coverage: bool
-00000960: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
-00000970: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00000980: 6e5f 6170 706c 6963 6162 6c65 5f63 6f75  n_applicable_cou
-00000990: 6e74 733d 4661 6c73 652c 0a20 2020 2020  nts=False,.     
-000009a0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000009b0: 6572 666f 726d 5f63 6c75 7374 6572 696e  erform_clusterin
-000009c0: 673d 4661 6c73 652c 0a20 2020 2020 2020  g=False,.       
-000009d0: 2020 2020 2020 2020 2020 2020 206f 6e6c               onl
-000009e0: 795f 7573 655f 7472 6169 6e5f 696e 7374  y_use_train_inst
-000009f0: 616e 6365 733d 4661 6c73 652c 0a20 2020  ances=False,.   
-00000a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a10: 2058 203d 204e 6f6e 652c 0a20 2020 2020   X = None,.     
-00000a20: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00000a30: 6f6c 6f72 7320 3d20 4e6f 6e65 293a 0a20  olors = None):. 
-00000a40: 2020 2063 6f6c 6f72 7320 3d20 6164 6a75     colors = adju
-00000a50: 7374 5f63 6f6c 6f72 7328 636f 6c6f 7273  st_colors(colors
-00000a60: 290a 0a20 2020 2073 6861 646f 775f 666f  )..    shadow_fo
-00000a70: 7265 7374 203d 2067 6574 5f73 6861 646f  rest = get_shado
-00000a80: 775f 666f 7265 7374 5f66 726f 6d5f 6368  w_forest_from_ch
-00000a90: 6563 6b65 7228 6d6f 6465 6c2c 2063 6865  ecker(model, che
-00000aa0: 636b 6572 290a 2020 2020 6e5f 6573 7469  cker).    n_esti
-00000ab0: 6d61 746f 7273 203d 206c 656e 2873 6861  mators = len(sha
-00000ac0: 646f 775f 666f 7265 7374 2e65 7374 696d  dow_forest.estim
-00000ad0: 6174 6f72 7329 0a20 2020 206e 6f64 6573  ators).    nodes
-00000ae0: 203d 205b 5d0a 2020 2020 6664 7473 203d   = [].    fdts =
-00000af0: 205b 5d0a 2020 2020 706c 6f74 7320 3d20   [].    plots = 
-00000b00: 5b5d 0a0a 2020 2020 6966 2069 7369 6e73  []..    if isins
-00000b10: 7461 6e63 6528 582c 6e70 2e6e 6461 7272  tance(X,np.ndarr
-00000b20: 6179 293a 0a20 2020 2020 2020 2079 5f70  ay):.        y_p
-00000b30: 7265 645f 666f 7265 7374 203d 2073 6861  red_forest = sha
-00000b40: 646f 775f 666f 7265 7374 2e70 7265 6469  dow_forest.predi
-00000b50: 6374 2858 2e72 6573 6861 7065 2828 312c  ct(X.reshape((1,
-00000b60: 2d31 2929 295b 305d 0a20 2020 2020 2020  -1)))[0].       
-00000b70: 2079 5f70 7265 6473 5f74 7265 6520 3d20   y_preds_tree = 
-00000b80: 5b5d 0a20 2020 2065 6c73 653a 0a20 2020  [].    else:.   
-00000b90: 2020 2020 2079 5f70 7265 645f 666f 7265       y_pred_fore
-00000ba0: 7374 203d 206e 702e 696e 660a 0a20 2020  st = np.inf..   
-00000bb0: 2066 6f72 2069 2069 6e20 7471 646d 2872   for i in tqdm(r
-00000bc0: 616e 6765 286e 5f65 7374 696d 6174 6f72  ange(n_estimator
-00000bd0: 7329 2c20 6465 7363 3d27 4576 616c 7561  s), desc='Evalua
-00000be0: 7469 6e67 2044 6563 6973 696f 6e20 5472  ting Decision Tr
-00000bf0: 6565 7327 293a 200a 2020 2020 2020 2020  ees'): .        
-00000c00: 6573 7469 6d61 746f 725f 6368 6563 6b65  estimator_checke
-00000c10: 7220 3d20 4368 6563 6b65 7228 7368 6164  r = Checker(shad
-00000c20: 6f77 5f66 6f72 6573 742e 6573 7469 6d61  ow_forest.estima
-00000c30: 746f 7273 5b69 5d2e 7072 6564 6963 742c  tors[i].predict,
-00000c40: 2063 6865 636b 6572 2e64 6174 6173 6574   checker.dataset
-00000c50: 2c20 7573 655f 6774 3d63 6865 636b 6572  , use_gt=checker
-00000c60: 2e5f 7573 655f 6774 290a 2020 2020 2020  ._use_gt).      
-00000c70: 2020 7368 6164 6f77 5f74 7265 6520 3d20    shadow_tree = 
-00000c80: 6765 745f 7368 6164 6f77 5f74 7265 655f  get_shadow_tree_
-00000c90: 6672 6f6d 5f63 6865 636b 6572 2873 6861  from_checker(sha
-00000ca0: 646f 775f 666f 7265 7374 2e65 7374 696d  dow_forest.estim
-00000cb0: 6174 6f72 735b 695d 2c20 6573 7469 6d61  ators[i], estima
-00000cc0: 746f 725f 6368 6563 6b65 7229 0a0a 2020  tor_checker)..  
-00000cd0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00000ce0: 6e63 6528 582c 6e70 2e6e 6461 7272 6179  nce(X,np.ndarray
-00000cf0: 293a 0a20 2020 2020 2020 2020 2020 2079  ):.            y
-00000d00: 5f70 7265 6473 5f74 7265 652e 6170 7065  _preds_tree.appe
-00000d10: 6e64 2873 6861 646f 775f 666f 7265 7374  nd(shadow_forest
-00000d20: 2e65 7374 696d 6174 6f72 735b 695d 2e70  .estimators[i].p
-00000d30: 7265 6469 6374 2858 2e72 6573 6861 7065  redict(X.reshape
-00000d40: 2828 312c 2d31 2929 295b 305d 290a 2020  ((1,-1)))[0]).  
-00000d50: 2020 2020 2020 2020 2020 6e6f 6465 203d            node =
-00000d60: 2073 6861 646f 775f 7472 6565 2e70 7265   shadow_tree.pre
-00000d70: 6469 6374 5f70 6174 6828 5829 5b2d 315d  dict_path(X)[-1]
-00000d80: 0a20 2020 2020 2020 2020 2020 2065 7374  .            est
-00000d90: 696d 6174 6f72 5f63 6865 636b 6572 203d  imator_checker =
-00000da0: 2044 6563 6973 696f 6e4e 6f64 6543 6865   DecisionNodeChe
-00000db0: 636b 6572 280a 2020 2020 2020 2020 2020  cker(.          
-00000dc0: 2020 2020 2020 6e6f 6465 2c20 6368 6563        node, chec
-00000dd0: 6b65 722e 6461 7461 7365 742c 2075 7365  ker.dataset, use
-00000de0: 5f67 743d 6368 6563 6b65 722e 5f75 7365  _gt=checker._use
-00000df0: 5f67 7429 0a20 2020 2020 2020 2065 6c73  _gt).        els
-00000e00: 653a 0a20 2020 2020 2020 2020 2020 206e  e:.            n
-00000e10: 6f64 6520 3d20 7368 6164 6f77 5f74 7265  ode = shadow_tre
-00000e20: 652e 726f 6f74 0a20 2020 2020 2020 200a  e.root.        .
-00000e30: 2020 2020 2020 2020 6966 206f 6e6c 795f          if only_
-00000e40: 7573 655f 7472 6169 6e5f 696e 7374 616e  use_train_instan
-00000e50: 6365 733a 0a20 2020 2020 2020 2020 2020  ces:.           
-00000e60: 2073 616d 706c 6573 203d 2073 6574 2867   samples = set(g
-00000e70: 6574 5f73 696e 676c 655f 6e6f 6465 5f73  et_single_node_s
-00000e80: 616d 706c 6573 286e 6f64 652c 6f6e 6c79  amples(node,only
-00000e90: 5f63 616c 6375 6c61 7465 5f73 696e 676c  _calculate_singl
-00000ea0: 655f 6e6f 6465 3d54 7275 6529 292e 696e  e_node=True)).in
-00000eb0: 7465 7273 6563 7469 6f6e 2873 6574 2873  tersection(set(s
-00000ec0: 6861 646f 775f 666f 7265 7374 2e67 6574  hadow_forest.get
-00000ed0: 5f62 6f6f 7473 7472 6170 5f69 6e64 6963  _bootstrap_indic
-00000ee0: 6573 2869 2929 290a 2020 2020 2020 2020  es(i))).        
-00000ef0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00000f00: 2020 7361 6d70 6c65 7320 3d20 6765 745f    samples = get_
-00000f10: 7369 6e67 6c65 5f6e 6f64 655f 7361 6d70  single_node_samp
-00000f20: 6c65 7328 6e6f 6465 2c20 6f6e 6c79 5f63  les(node, only_c
-00000f30: 616c 6375 6c61 7465 5f73 696e 676c 655f  alculate_single_
-00000f40: 6e6f 6465 3d54 7275 6529 0a0a 2020 2020  node=True)..    
-00000f50: 2020 2020 6664 7420 3d20 4672 6571 7565      fdt = Freque
-00000f60: 6e63 7944 6973 7472 6962 7574 696f 6e54  ncyDistributionT
-00000f70: 6162 6c65 2865 7374 696d 6174 6f72 5f63  able(estimator_c
-00000f80: 6865 636b 6572 2c63 6f6e 7374 7261 696e  hecker,constrain
-00000f90: 7473 2c20 6c69 7374 2873 616d 706c 6573  ts, list(samples
-00000fa0: 292c 2067 726f 7570 5f66 756e 6374 696f  ), group_functio
-00000fb0: 6e73 2c20 636f 7665 7261 6765 3d63 6f76  ns, coverage=cov
-00000fc0: 6572 6167 652c 206e 6f6e 5f61 7070 6c69  erage, non_appli
-00000fd0: 6361 626c 655f 636f 756e 7473 3d6e 6f6e  cable_counts=non
-00000fe0: 5f61 7070 6c69 6361 626c 655f 636f 756e  _applicable_coun
-00000ff0: 7473 290a 2020 2020 2020 2020 6664 7473  ts).        fdts
-00001000: 2e61 7070 656e 6428 6664 7429 0a20 2020  .append(fdt).   
-00001010: 200a 2020 2020 6966 2070 6572 666f 726d   .    if perform
-00001020: 5f63 6c75 7374 6572 696e 673a 0a20 2020  _clustering:.   
-00001030: 2020 2020 206c 6162 656c 732c 206e 5f63       labels, n_c
-00001040: 6c75 7374 6572 7320 3d20 6772 6f75 705f  lusters = group_
-00001050: 7265 7375 6c74 735f 6279 5f63 6c75 7374  results_by_clust
-00001060: 6572 696e 6728 6e70 2e73 7461 636b 286c  ering(np.stack(l
-00001070: 6973 7428 6d61 7028 6c61 6d62 6461 2066  ist(map(lambda f
-00001080: 6474 3a20 6664 742e 6664 742e 7661 6c75  dt: fdt.fdt.valu
-00001090: 6573 2e66 6c61 7474 656e 2829 2c20 6664  es.flatten(), fd
-000010a0: 7473 2929 2929 0a20 2020 2020 2020 2067  ts)))).        g
-000010b0: 726f 7570 5f66 6474 5f69 6478 203d 207b  roup_fdt_idx = {
-000010c0: 7d0a 2020 2020 2020 2020 666f 7220 6920  }.        for i 
-000010d0: 696e 2072 616e 6765 286e 5f63 6c75 7374  in range(n_clust
-000010e0: 6572 7329 3a0a 2020 2020 2020 2020 2020  ers):.          
-000010f0: 2020 6772 6f75 705f 6664 745f 6964 785b    group_fdt_idx[
-00001100: 695d 203d 206c 6973 7428 6e70 2e77 6865  i] = list(np.whe
-00001110: 7265 286c 6162 656c 7320 3d3d 2069 295b  re(labels == i)[
-00001120: 305d 290a 2020 2020 656c 7365 3a0a 2020  0]).    else:.  
-00001130: 2020 2020 2020 6772 6f75 705f 6664 745f        group_fdt_
-00001140: 6964 7820 3d20 7b69 3a5b 695d 2066 6f72  idx = {i:[i] for
-00001150: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-00001160: 6664 7473 2929 7d0a 0a20 2020 2066 6f72  fdts))}..    for
-00001170: 2069 2069 6e20 7471 646d 2872 616e 6765   i in tqdm(range
-00001180: 286c 656e 2867 726f 7570 5f66 6474 5f69  (len(group_fdt_i
-00001190: 6478 2e6b 6579 7328 2929 292c 2064 6573  dx.keys())), des
-000011a0: 633d 2756 6973 7561 6c69 7a69 6e67 2052  c='Visualizing R
-000011b0: 6573 756c 7473 2729 3a0a 2020 2020 2020  esults'):.      
-000011c0: 2020 6966 206c 656e 2867 726f 7570 5f66    if len(group_f
-000011d0: 6474 5f69 6478 5b69 5d29 203e 2030 3a0a  dt_idx[i]) > 0:.
-000011e0: 2020 2020 2020 2020 2020 2020 706c 6f74              plot
-000011f0: 203d 2066 6474 735b 6772 6f75 705f 6664   = fdts[group_fd
-00001200: 745f 6964 785b 695d 5b30 5d5d 2e76 6973  t_idx[i][0]].vis
-00001210: 7561 6c69 7a65 2827 4454 2027 202b 2027  ualize('DT ' + '
-00001220: 2c27 2e6a 6f69 6e28 5b73 7472 286a 2920  ,'.join([str(j) 
-00001230: 666f 7220 6a20 696e 2067 726f 7570 5f66  for j in group_f
-00001240: 6474 5f69 6478 5b69 5d5d 2929 0a20 2020  dt_idx[i]])).   
-00001250: 2020 2020 2020 2020 2070 6c6f 7473 2e61           plots.a
-00001260: 7070 656e 6428 706c 6f74 290a 2020 2020  ppend(plot).    
-00001270: 2020 2020 2020 2020 7669 7a5f 7061 7468          viz_path
-00001280: 203d 2067 7261 7068 7669 7a5f 6865 6c70   = graphviz_help
-00001290: 6572 2e67 6574 5f69 6d61 6765 5f70 6174  er.get_image_pat
-000012a0: 6828 6e6f 6465 5f6e 616d 6528 6929 290a  h(node_name(i)).
-000012b0: 2020 2020 2020 2020 2020 2020 706c 6f74              plot
-000012c0: 2e73 6176 6528 7669 7a5f 7061 7468 290a  .save(viz_path).
-000012d0: 2020 2020 2020 2020 2020 2020 636c 7573              clus
-000012e0: 7465 725f 7072 6564 203d 2043 6f75 6e74  ter_pred = Count
-000012f0: 6572 285b 795f 7072 6564 735f 7472 6565  er([y_preds_tree
-00001300: 5b6a 5d20 666f 7220 6a20 696e 2067 726f  [j] for j in gro
-00001310: 7570 5f66 6474 5f69 6478 5b69 5d5d 292e  up_fdt_idx[i]]).
-00001320: 6d6f 7374 5f63 6f6d 6d6f 6e28 3129 5b30  most_common(1)[0
-00001330: 5d5b 305d 0a20 2020 2020 2020 2020 2020  ][0].           
-00001340: 2068 6967 686c 6967 6874 203d 2063 6c75   highlight = clu
-00001350: 7374 6572 5f70 7265 6420 3d3d 2079 5f70  ster_pred == y_p
-00001360: 7265 645f 666f 7265 7374 2069 6620 6973  red_forest if is
-00001370: 696e 7374 616e 6365 2858 2c6e 702e 6e64  instance(X,np.nd
-00001380: 6172 7261 7929 2065 6c73 6520 4661 6c73  array) else Fals
-00001390: 650a 2020 2020 2020 2020 2020 2020 6e6f  e.            no
-000013a0: 6465 732e 6170 7065 6e64 2867 7261 7068  des.append(graph
-000013b0: 7669 7a5f 6865 6c70 6572 2e6e 6f64 655f  viz_helper.node_
-000013c0: 7374 6d74 286e 6f64 655f 6e61 6d65 2869  stmt(node_name(i
-000013d0: 292c 6772 6170 6876 697a 5f68 656c 7065  ),graphviz_helpe
-000013e0: 722e 6874 6d6c 5f69 6d61 6765 2827 272c  r.html_image('',
-000013f0: 7669 7a5f 7061 7468 292c 6869 6768 6c69  viz_path),highli
-00001400: 6768 7420 2c63 6f6c 6f72 7329 290a 0a20  ght ,colors)).. 
-00001410: 2020 206c 6567 656e 6420 3d20 6472 6177     legend = draw
-00001420: 5f6c 6567 656e 6428 706c 6f74 7329 0a20  _legend(plots). 
-00001430: 2020 206c 6567 656e 645f 7061 7468 203d     legend_path =
-00001440: 2067 7261 7068 7669 7a5f 6865 6c70 6572   graphviz_helper
-00001450: 2e67 6574 5f69 6d61 6765 5f70 6174 6828  .get_image_path(
-00001460: 276c 6567 656e 6427 290a 2020 2020 6c65  'legend').    le
-00001470: 6765 6e64 2e73 6176 6528 6c65 6765 6e64  gend.save(legend
-00001480: 5f70 6174 6829 0a0a 2020 2020 7265 7475  _path)..    retu
-00001490: 726e 2067 7261 7068 7669 7a5f 6865 6c70  rn graphviz_help
-000014a0: 6572 2e67 7269 645f 6c61 796f 7574 2827  er.grid_layout('
-000014b0: 5261 6e64 6f6d 2046 6f72 6573 7427 2c20  Random Forest', 
-000014c0: 6e6f 6465 732c 5b5d 2c6c 6567 656e 645f  nodes,[],legend_
-000014d0: 7061 7468 2c20 636f 6c6f 7273 2c20 6f72  path, colors, or
-000014e0: 6965 6e74 6174 696f 6e3d 2754 4427 290a  ientation='TD').
-000014f0: 0a64 6566 2063 6f6d 7061 7265 5f64 6563  .def compare_dec
-00001500: 6973 696f 6e5f 7472 6565 7328 6d6f 6465  ision_trees(mode
-00001510: 6c2c 2063 6865 636b 6572 3a20 4368 6563  l, checker: Chec
-00001520: 6b65 722c 2063 6f6e 7374 7261 696e 7473  ker, constraints
-00001530: 3a20 4c69 7374 5b43 6f6e 7374 7261 696e  : List[Constrain
-00001540: 745d 2c20 7472 6565 5f69 6e64 697a 6573  t], tree_indizes
-00001550: 3a20 6c69 7374 2c20 636f 6c6f 7273 3d4e  : list, colors=N
-00001560: 6f6e 652c 202a 2a61 7267 7329 3a0a 2020  one, **args):.  
-00001570: 2020 636f 6c6f 7273 203d 2061 646a 7573    colors = adjus
-00001580: 745f 636f 6c6f 7273 2863 6f6c 6f72 7329  t_colors(colors)
-00001590: 0a20 2020 2073 6861 646f 775f 666f 7265  .    shadow_fore
-000015a0: 7374 203d 2067 6574 5f73 6861 646f 775f  st = get_shadow_
-000015b0: 666f 7265 7374 5f66 726f 6d5f 6368 6563  forest_from_chec
-000015c0: 6b65 7228 6d6f 6465 6c2c 2063 6865 636b  ker(model, check
-000015d0: 6572 290a 2020 2020 6e6f 6465 7320 3d20  er).    nodes = 
-000015e0: 5b5d 0a20 2020 2066 6f72 2069 2069 6e20  [].    for i in 
-000015f0: 7471 646d 2874 7265 655f 696e 6469 7a65  tqdm(tree_indize
-00001600: 732c 2064 6573 633d 2745 7661 6c75 6174  s, desc='Evaluat
-00001610: 696e 6720 436f 6e73 7472 6169 6e74 7320  ing Constraints 
-00001620: 616e 6420 5669 7375 616c 697a 696e 6720  and Visualizing 
-00001630: 4465 6369 7369 6f6e 2054 7265 6573 2729  Decision Trees')
-00001640: 3a0a 2020 2020 2020 2020 7368 6164 6f77  :.        shadow
-00001650: 5f74 7265 6520 3d20 6765 745f 7368 6164  _tree = get_shad
-00001660: 6f77 5f74 7265 655f 6672 6f6d 5f63 6865  ow_tree_from_che
-00001670: 636b 6572 2873 6861 646f 775f 666f 7265  cker(shadow_fore
-00001680: 7374 2e65 7374 696d 6174 6f72 735b 695d  st.estimators[i]
-00001690: 2c20 6368 6563 6b65 7229 0a20 2020 2020  , checker).     
-000016a0: 2020 2076 697a 203d 2064 6563 6973 696f     viz = decisio
-000016b0: 6e5f 7472 6565 732e 6474 7265 6576 697a  n_trees.dtreeviz
-000016c0: 2873 6861 646f 775f 7472 6565 2c20 6368  (shadow_tree, ch
-000016d0: 6563 6b65 722c 2063 6f6e 7374 7261 696e  ecker, constrain
-000016e0: 7473 2c69 6e64 6963 6573 3d73 6861 646f  ts,indices=shado
-000016f0: 775f 666f 7265 7374 2e67 6574 5f62 6f6f  w_forest.get_boo
-00001700: 7473 7472 6170 5f69 6e64 6963 6573 2869  tstrap_indices(i
-00001710: 292c 202a 2a61 7267 7329 0a20 2020 2020  ), **args).     
-00001720: 2020 2076 697a 5f70 6174 6820 3d20 6772     viz_path = gr
-00001730: 6170 6876 697a 5f68 656c 7065 722e 6765  aphviz_helper.ge
-00001740: 745f 696d 6167 655f 7061 7468 286e 6f64  t_image_path(nod
-00001750: 655f 6e61 6d65 2869 2929 0a20 2020 2020  e_name(i)).     
-00001760: 2020 2076 697a 2e73 6176 6528 7669 7a5f     viz.save(viz_
-00001770: 7061 7468 290a 2020 2020 2020 2020 6e6f  path).        no
-00001780: 6465 732e 6170 7065 6e64 2867 7261 7068  des.append(graph
-00001790: 7669 7a5f 6865 6c70 6572 2e6e 6f64 655f  viz_helper.node_
-000017a0: 7374 6d74 286e 6f64 655f 6e61 6d65 2869  stmt(node_name(i
-000017b0: 292c 6772 6170 6876 697a 5f68 656c 7065  ),graphviz_helpe
-000017c0: 722e 6874 6d6c 5f69 6d61 6765 2827 4454  r.html_image('DT
-000017d0: 2027 202b 2073 7472 2869 292c 7669 7a5f   ' + str(i),viz_
-000017e0: 7061 7468 292c 4661 6c73 652c 636f 6c6f  path),False,colo
-000017f0: 7273 2929 0a20 2020 2072 6574 7572 6e20  rs)).    return 
-00001800: 6772 6170 6876 697a 5f68 656c 7065 722e  graphviz_helper.
-00001810: 6772 6964 5f6c 6179 6f75 7428 2753 656c  grid_layout('Sel
-00001820: 6563 7465 6420 4573 7469 6d61 746f 7273  ected Estimators
-00001830: 272c 206e 6f64 6573 2c5b 5d2c 4e6f 6e65  ', nodes,[],None
-00001840: 2c63 6f6c 6f72 732c 7369 7a65 3d28 312c  ,colors,size=(1,
-00001850: 6c65 6e28 7472 6565 5f69 6e64 697a 6573  len(tree_indizes
-00001860: 2929 2c20 6f72 6965 6e74 6174 696f 6e3d  )), orientation=
-00001870: 2754 4427 290a 0a0a 0a0a 2020 2020 0a20  'TD').....    . 
-00001880: 2020 200a 0a                                ..
+00000950: 636f 6e73 7472 6169 6e74 733a 204c 6973  constraints: Lis
+00000960: 745b 436f 6e73 7472 6169 6e74 5d2c 0a20  t[Constraint],. 
+00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000980: 2020 2067 726f 7570 5f66 756e 6374 696f     group_functio
+00000990: 6e73 203d 2067 726f 7570 5f62 795f 6774  ns = group_by_gt
+000009a0: 5f63 6c61 7373 2c0a 2020 2020 2020 2020  _class,.        
+000009b0: 2020 2020 2020 2020 2020 2020 636f 7665              cove
+000009c0: 7261 6765 3a20 626f 6f6c 203d 2046 616c  rage: bool = Fal
+000009d0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+000009e0: 2020 2020 2020 2020 6e6f 6e5f 6170 706c          non_appl
+000009f0: 6963 6162 6c65 5f63 6f75 6e74 733d 4661  icable_counts=Fa
+00000a00: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+00000a10: 2020 2020 2020 2020 2070 6572 666f 726d           perform
+00000a20: 5f63 6c75 7374 6572 696e 673d 4661 6c73  _clustering=Fals
+00000a30: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00000a40: 2020 2020 2020 206f 6e6c 795f 7573 655f         only_use_
+00000a50: 7472 6169 6e5f 696e 7374 616e 6365 733d  train_instances=
+00000a60: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
+00000a70: 2020 2020 2020 2020 2020 2058 203d 204e             X = N
+00000a80: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00000a90: 2020 2020 2020 2020 2063 6f6c 6f72 7320           colors 
+00000aa0: 3d20 4e6f 6e65 293a 0a20 2020 2063 6f6c  = None):.    col
+00000ab0: 6f72 7320 3d20 6164 6a75 7374 5f63 6f6c  ors = adjust_col
+00000ac0: 6f72 7328 636f 6c6f 7273 290a 0a20 2020  ors(colors)..   
+00000ad0: 2073 6861 646f 775f 666f 7265 7374 203d   shadow_forest =
+00000ae0: 2067 6574 5f73 6861 646f 775f 666f 7265   get_shadow_fore
+00000af0: 7374 5f66 726f 6d5f 6368 6563 6b65 7228  st_from_checker(
+00000b00: 6d6f 6465 6c2c 2063 6865 636b 6572 290a  model, checker).
+00000b10: 2020 2020 6e5f 6573 7469 6d61 746f 7273      n_estimators
+00000b20: 203d 206c 656e 2873 6861 646f 775f 666f   = len(shadow_fo
+00000b30: 7265 7374 2e65 7374 696d 6174 6f72 7329  rest.estimators)
+00000b40: 0a20 2020 206e 6f64 6573 203d 205b 5d0a  .    nodes = [].
+00000b50: 2020 2020 6664 7473 203d 205b 5d0a 2020      fdts = [].  
+00000b60: 2020 706c 6f74 7320 3d20 5b5d 0a0a 2020    plots = []..  
+00000b70: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00000b80: 582c 6e70 2e6e 6461 7272 6179 293a 0a20  X,np.ndarray):. 
+00000b90: 2020 2020 2020 2079 5f70 7265 645f 666f         y_pred_fo
+00000ba0: 7265 7374 203d 2073 6861 646f 775f 666f  rest = shadow_fo
+00000bb0: 7265 7374 2e70 7265 6469 6374 2858 2e72  rest.predict(X.r
+00000bc0: 6573 6861 7065 2828 312c 2d31 2929 295b  eshape((1,-1)))[
+00000bd0: 305d 0a20 2020 2020 2020 2079 5f70 7265  0].        y_pre
+00000be0: 6473 5f74 7265 6520 3d20 5b5d 0a20 2020  ds_tree = [].   
+00000bf0: 2065 6c73 653a 0a20 2020 2020 2020 2079   else:.        y
+00000c00: 5f70 7265 645f 666f 7265 7374 203d 206e  _pred_forest = n
+00000c10: 702e 696e 660a 0a20 2020 2066 6f72 2069  p.inf..    for i
+00000c20: 2069 6e20 7471 646d 2872 616e 6765 286e   in tqdm(range(n
+00000c30: 5f65 7374 696d 6174 6f72 7329 2c20 6465  _estimators), de
+00000c40: 7363 3d27 4576 616c 7561 7469 6e67 2044  sc='Evaluating D
+00000c50: 6563 6973 696f 6e20 5472 6565 7327 293a  ecision Trees'):
+00000c60: 200a 2020 2020 2020 2020 6573 7469 6d61   .        estima
+00000c70: 746f 725f 6368 6563 6b65 7220 3d20 4368  tor_checker = Ch
+00000c80: 6563 6b65 7228 7368 6164 6f77 5f66 6f72  ecker(shadow_for
+00000c90: 6573 742e 6573 7469 6d61 746f 7273 5b69  est.estimators[i
+00000ca0: 5d2e 7072 6564 6963 742c 2063 6865 636b  ].predict, check
+00000cb0: 6572 2e64 6174 6173 6574 2c20 7573 655f  er.dataset, use_
+00000cc0: 6774 3d63 6865 636b 6572 2e5f 7573 655f  gt=checker._use_
+00000cd0: 6774 290a 2020 2020 2020 2020 7368 6164  gt).        shad
+00000ce0: 6f77 5f74 7265 6520 3d20 6765 745f 7368  ow_tree = get_sh
+00000cf0: 6164 6f77 5f74 7265 655f 6672 6f6d 5f63  adow_tree_from_c
+00000d00: 6865 636b 6572 2873 6861 646f 775f 666f  hecker(shadow_fo
+00000d10: 7265 7374 2e65 7374 696d 6174 6f72 735b  rest.estimators[
+00000d20: 695d 2c20 6573 7469 6d61 746f 725f 6368  i], estimator_ch
+00000d30: 6563 6b65 7229 0a0a 2020 2020 2020 2020  ecker)..        
+00000d40: 6966 2069 7369 6e73 7461 6e63 6528 582c  if isinstance(X,
+00000d50: 6e70 2e6e 6461 7272 6179 293a 0a20 2020  np.ndarray):.   
+00000d60: 2020 2020 2020 2020 2079 5f70 7265 6473           y_preds
+00000d70: 5f74 7265 652e 6170 7065 6e64 2873 6861  _tree.append(sha
+00000d80: 646f 775f 666f 7265 7374 2e65 7374 696d  dow_forest.estim
+00000d90: 6174 6f72 735b 695d 2e70 7265 6469 6374  ators[i].predict
+00000da0: 2858 2e72 6573 6861 7065 2828 312c 2d31  (X.reshape((1,-1
+00000db0: 2929 295b 305d 290a 2020 2020 2020 2020  )))[0]).        
+00000dc0: 2020 2020 6e6f 6465 203d 2073 6861 646f      node = shado
+00000dd0: 775f 7472 6565 2e70 7265 6469 6374 5f70  w_tree.predict_p
+00000de0: 6174 6828 5829 5b2d 315d 0a20 2020 2020  ath(X)[-1].     
+00000df0: 2020 2020 2020 2065 7374 696d 6174 6f72         estimator
+00000e00: 5f63 6865 636b 6572 203d 2044 6563 6973  _checker = Decis
+00000e10: 696f 6e4e 6f64 6543 6865 636b 6572 280a  ionNodeChecker(.
+00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e30: 6e6f 6465 2c20 6368 6563 6b65 722e 6461  node, checker.da
+00000e40: 7461 7365 742c 2075 7365 5f67 743d 6368  taset, use_gt=ch
+00000e50: 6563 6b65 722e 5f75 7365 5f67 7429 0a20  ecker._use_gt). 
+00000e60: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00000e70: 2020 2020 2020 2020 206e 6f64 6520 3d20           node = 
+00000e80: 7368 6164 6f77 5f74 7265 652e 726f 6f74  shadow_tree.root
+00000e90: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000ea0: 2020 6966 206f 6e6c 795f 7573 655f 7472    if only_use_tr
+00000eb0: 6169 6e5f 696e 7374 616e 6365 733a 0a20  ain_instances:. 
+00000ec0: 2020 2020 2020 2020 2020 2073 616d 706c             sampl
+00000ed0: 6573 203d 2073 6574 2867 6574 5f73 696e  es = set(get_sin
+00000ee0: 676c 655f 6e6f 6465 5f73 616d 706c 6573  gle_node_samples
+00000ef0: 286e 6f64 652c 6f6e 6c79 5f63 616c 6375  (node,only_calcu
+00000f00: 6c61 7465 5f73 696e 676c 655f 6e6f 6465  late_single_node
+00000f10: 3d54 7275 6529 292e 696e 7465 7273 6563  =True)).intersec
+00000f20: 7469 6f6e 2873 6574 2873 6861 646f 775f  tion(set(shadow_
+00000f30: 666f 7265 7374 2e67 6574 5f62 6f6f 7473  forest.get_boots
+00000f40: 7472 6170 5f69 6e64 6963 6573 2869 2929  trap_indices(i))
+00000f50: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00000f60: 2020 2020 2020 2020 2020 2020 7361 6d70              samp
+00000f70: 6c65 7320 3d20 6765 745f 7369 6e67 6c65  les = get_single
+00000f80: 5f6e 6f64 655f 7361 6d70 6c65 7328 6e6f  _node_samples(no
+00000f90: 6465 2c20 6f6e 6c79 5f63 616c 6375 6c61  de, only_calcula
+00000fa0: 7465 5f73 696e 676c 655f 6e6f 6465 3d54  te_single_node=T
+00000fb0: 7275 6529 0a0a 2020 2020 2020 2020 6664  rue)..        fd
+00000fc0: 7420 3d20 4672 6571 7565 6e63 7944 6973  t = FrequencyDis
+00000fd0: 7472 6962 7574 696f 6e54 6162 6c65 2865  tributionTable(e
+00000fe0: 7374 696d 6174 6f72 5f63 6865 636b 6572  stimator_checker
+00000ff0: 2c63 6f6e 7374 7261 696e 7473 2c20 6c69  ,constraints, li
+00001000: 7374 2873 616d 706c 6573 292c 2067 726f  st(samples), gro
+00001010: 7570 5f66 756e 6374 696f 6e73 2c20 636f  up_functions, co
+00001020: 7665 7261 6765 3d63 6f76 6572 6167 652c  verage=coverage,
+00001030: 206e 6f6e 5f61 7070 6c69 6361 626c 655f   non_applicable_
+00001040: 636f 756e 7473 3d6e 6f6e 5f61 7070 6c69  counts=non_appli
+00001050: 6361 626c 655f 636f 756e 7473 290a 2020  cable_counts).  
+00001060: 2020 2020 2020 6664 7473 2e61 7070 656e        fdts.appen
+00001070: 6428 6664 7429 0a20 2020 200a 2020 2020  d(fdt).    .    
+00001080: 6966 2070 6572 666f 726d 5f63 6c75 7374  if perform_clust
+00001090: 6572 696e 673a 0a20 2020 2020 2020 206c  ering:.        l
+000010a0: 6162 656c 732c 206e 5f63 6c75 7374 6572  abels, n_cluster
+000010b0: 7320 3d20 6772 6f75 705f 7265 7375 6c74  s = group_result
+000010c0: 735f 6279 5f63 6c75 7374 6572 696e 6728  s_by_clustering(
+000010d0: 6e70 2e73 7461 636b 286c 6973 7428 6d61  np.stack(list(ma
+000010e0: 7028 6c61 6d62 6461 2066 6474 3a20 6664  p(lambda fdt: fd
+000010f0: 742e 6664 742e 7661 6c75 6573 2e66 6c61  t.fdt.values.fla
+00001100: 7474 656e 2829 2c20 6664 7473 2929 2929  tten(), fdts))))
+00001110: 0a20 2020 2020 2020 2067 726f 7570 5f66  .        group_f
+00001120: 6474 5f69 6478 203d 207b 7d0a 2020 2020  dt_idx = {}.    
+00001130: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00001140: 6765 286e 5f63 6c75 7374 6572 7329 3a0a  ge(n_clusters):.
+00001150: 2020 2020 2020 2020 2020 2020 6772 6f75              grou
+00001160: 705f 6664 745f 6964 785b 695d 203d 206c  p_fdt_idx[i] = l
+00001170: 6973 7428 6e70 2e77 6865 7265 286c 6162  ist(np.where(lab
+00001180: 656c 7320 3d3d 2069 295b 305d 290a 2020  els == i)[0]).  
+00001190: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000011a0: 6772 6f75 705f 6664 745f 6964 7820 3d20  group_fdt_idx = 
+000011b0: 7b69 3a5b 695d 2066 6f72 2069 2069 6e20  {i:[i] for i in 
+000011c0: 7261 6e67 6528 6c65 6e28 6664 7473 2929  range(len(fdts))
+000011d0: 7d0a 0a20 2020 2066 6f72 2069 2069 6e20  }..    for i in 
+000011e0: 7471 646d 2872 616e 6765 286c 656e 2867  tqdm(range(len(g
+000011f0: 726f 7570 5f66 6474 5f69 6478 2e6b 6579  roup_fdt_idx.key
+00001200: 7328 2929 292c 2064 6573 633d 2756 6973  s())), desc='Vis
+00001210: 7561 6c69 7a69 6e67 2052 6573 756c 7473  ualizing Results
+00001220: 2729 3a0a 2020 2020 2020 2020 6966 206c  '):.        if l
+00001230: 656e 2867 726f 7570 5f66 6474 5f69 6478  en(group_fdt_idx
+00001240: 5b69 5d29 203e 2030 3a0a 2020 2020 2020  [i]) > 0:.      
+00001250: 2020 2020 2020 706c 6f74 203d 2066 6474        plot = fdt
+00001260: 735b 6772 6f75 705f 6664 745f 6964 785b  s[group_fdt_idx[
+00001270: 695d 5b30 5d5d 2e76 6973 7561 6c69 7a65  i][0]].visualize
+00001280: 2827 4454 2027 202b 2027 2c27 2e6a 6f69  ('DT ' + ','.joi
+00001290: 6e28 5b73 7472 286a 2920 666f 7220 6a20  n([str(j) for j 
+000012a0: 696e 2067 726f 7570 5f66 6474 5f69 6478  in group_fdt_idx
+000012b0: 5b69 5d5d 2929 0a20 2020 2020 2020 2020  [i]])).         
+000012c0: 2020 2070 6c6f 7473 2e61 7070 656e 6428     plots.append(
+000012d0: 706c 6f74 290a 2020 2020 2020 2020 2020  plot).          
+000012e0: 2020 7669 7a5f 7061 7468 203d 2067 7261    viz_path = gra
+000012f0: 7068 7669 7a5f 6865 6c70 6572 2e67 6574  phviz_helper.get
+00001300: 5f69 6d61 6765 5f70 6174 6828 6e6f 6465  _image_path(node
+00001310: 5f6e 616d 6528 6929 290a 2020 2020 2020  _name(i)).      
+00001320: 2020 2020 2020 706c 6f74 2e73 6176 6528        plot.save(
+00001330: 7669 7a5f 7061 7468 290a 2020 2020 2020  viz_path).      
+00001340: 2020 2020 2020 636c 7573 7465 725f 7072        cluster_pr
+00001350: 6564 203d 2043 6f75 6e74 6572 285b 795f  ed = Counter([y_
+00001360: 7072 6564 735f 7472 6565 5b6a 5d20 666f  preds_tree[j] fo
+00001370: 7220 6a20 696e 2067 726f 7570 5f66 6474  r j in group_fdt
+00001380: 5f69 6478 5b69 5d5d 292e 6d6f 7374 5f63  _idx[i]]).most_c
+00001390: 6f6d 6d6f 6e28 3129 5b30 5d5b 305d 0a20  ommon(1)[0][0]. 
+000013a0: 2020 2020 2020 2020 2020 2068 6967 686c             highl
+000013b0: 6967 6874 203d 2063 6c75 7374 6572 5f70  ight = cluster_p
+000013c0: 7265 6420 3d3d 2079 5f70 7265 645f 666f  red == y_pred_fo
+000013d0: 7265 7374 2069 6620 6973 696e 7374 616e  rest if isinstan
+000013e0: 6365 2858 2c6e 702e 6e64 6172 7261 7929  ce(X,np.ndarray)
+000013f0: 2065 6c73 6520 4661 6c73 650a 2020 2020   else False.    
+00001400: 2020 2020 2020 2020 6e6f 6465 732e 6170          nodes.ap
+00001410: 7065 6e64 2867 7261 7068 7669 7a5f 6865  pend(graphviz_he
+00001420: 6c70 6572 2e6e 6f64 655f 7374 6d74 286e  lper.node_stmt(n
+00001430: 6f64 655f 6e61 6d65 2869 292c 6772 6170  ode_name(i),grap
+00001440: 6876 697a 5f68 656c 7065 722e 6874 6d6c  hviz_helper.html
+00001450: 5f69 6d61 6765 2827 272c 7669 7a5f 7061  _image('',viz_pa
+00001460: 7468 292c 6869 6768 6c69 6768 7420 2c63  th),highlight ,c
+00001470: 6f6c 6f72 7329 290a 0a20 2020 206c 6567  olors))..    leg
+00001480: 656e 6420 3d20 6472 6177 5f6c 6567 656e  end = draw_legen
+00001490: 6428 706c 6f74 7329 0a20 2020 206c 6567  d(plots).    leg
+000014a0: 656e 645f 7061 7468 203d 2067 7261 7068  end_path = graph
+000014b0: 7669 7a5f 6865 6c70 6572 2e67 6574 5f69  viz_helper.get_i
+000014c0: 6d61 6765 5f70 6174 6828 276c 6567 656e  mage_path('legen
+000014d0: 6427 290a 2020 2020 6c65 6765 6e64 2e73  d').    legend.s
+000014e0: 6176 6528 6c65 6765 6e64 5f70 6174 6829  ave(legend_path)
+000014f0: 0a0a 2020 2020 7265 7475 726e 2067 7261  ..    return gra
+00001500: 7068 7669 7a5f 6865 6c70 6572 2e67 7269  phviz_helper.gri
+00001510: 645f 6c61 796f 7574 2827 5261 6e64 6f6d  d_layout('Random
+00001520: 2046 6f72 6573 7427 2c20 6e6f 6465 732c   Forest', nodes,
+00001530: 5b5d 2c6c 6567 656e 645f 7061 7468 2c20  [],legend_path, 
+00001540: 636f 6c6f 7273 2c20 6f72 6965 6e74 6174  colors, orientat
+00001550: 696f 6e3d 2754 4427 290a 0a64 6566 2063  ion='TD')..def c
+00001560: 6f6d 7061 7265 5f64 6563 6973 696f 6e5f  ompare_decision_
+00001570: 7472 6565 7328 6d6f 6465 6c2c 2063 6865  trees(model, che
+00001580: 636b 6572 3a20 4368 6563 6b65 722c 2063  cker: Checker, c
+00001590: 6f6e 7374 7261 696e 7473 3a20 4c69 7374  onstraints: List
+000015a0: 5b43 6f6e 7374 7261 696e 745d 2c20 7472  [Constraint], tr
+000015b0: 6565 5f69 6e64 697a 6573 3a20 6c69 7374  ee_indizes: list
+000015c0: 2c20 636f 6c6f 7273 3d4e 6f6e 652c 202a  , colors=None, *
+000015d0: 2a61 7267 7329 3a0a 2020 2020 636f 6c6f  *args):.    colo
+000015e0: 7273 203d 2061 646a 7573 745f 636f 6c6f  rs = adjust_colo
+000015f0: 7273 2863 6f6c 6f72 7329 0a20 2020 2073  rs(colors).    s
+00001600: 6861 646f 775f 666f 7265 7374 203d 2067  hadow_forest = g
+00001610: 6574 5f73 6861 646f 775f 666f 7265 7374  et_shadow_forest
+00001620: 5f66 726f 6d5f 6368 6563 6b65 7228 6d6f  _from_checker(mo
+00001630: 6465 6c2c 2063 6865 636b 6572 290a 2020  del, checker).  
+00001640: 2020 6e6f 6465 7320 3d20 5b5d 0a20 2020    nodes = [].   
+00001650: 2066 6f72 2069 2069 6e20 7471 646d 2874   for i in tqdm(t
+00001660: 7265 655f 696e 6469 7a65 732c 2064 6573  ree_indizes, des
+00001670: 633d 2745 7661 6c75 6174 696e 6720 436f  c='Evaluating Co
+00001680: 6e73 7472 6169 6e74 7320 616e 6420 5669  nstraints and Vi
+00001690: 7375 616c 697a 696e 6720 4465 6369 7369  sualizing Decisi
+000016a0: 6f6e 2054 7265 6573 2729 3a0a 2020 2020  on Trees'):.    
+000016b0: 2020 2020 7368 6164 6f77 5f74 7265 6520      shadow_tree 
+000016c0: 3d20 6765 745f 7368 6164 6f77 5f74 7265  = get_shadow_tre
+000016d0: 655f 6672 6f6d 5f63 6865 636b 6572 2873  e_from_checker(s
+000016e0: 6861 646f 775f 666f 7265 7374 2e65 7374  hadow_forest.est
+000016f0: 696d 6174 6f72 735b 695d 2c20 6368 6563  imators[i], chec
+00001700: 6b65 7229 0a20 2020 2020 2020 2076 697a  ker).        viz
+00001710: 203d 2064 6563 6973 696f 6e5f 7472 6565   = decision_tree
+00001720: 732e 6474 7265 6576 697a 2873 6861 646f  s.dtreeviz(shado
+00001730: 775f 7472 6565 2c20 6368 6563 6b65 722c  w_tree, checker,
+00001740: 2063 6f6e 7374 7261 696e 7473 2c69 6e64   constraints,ind
+00001750: 6963 6573 3d73 6861 646f 775f 666f 7265  ices=shadow_fore
+00001760: 7374 2e67 6574 5f62 6f6f 7473 7472 6170  st.get_bootstrap
+00001770: 5f69 6e64 6963 6573 2869 292c 202a 2a61  _indices(i), **a
+00001780: 7267 7329 0a20 2020 2020 2020 2076 697a  rgs).        viz
+00001790: 5f70 6174 6820 3d20 6772 6170 6876 697a  _path = graphviz
+000017a0: 5f68 656c 7065 722e 6765 745f 696d 6167  _helper.get_imag
+000017b0: 655f 7061 7468 286e 6f64 655f 6e61 6d65  e_path(node_name
+000017c0: 2869 2929 0a20 2020 2020 2020 2076 697a  (i)).        viz
+000017d0: 2e73 6176 6528 7669 7a5f 7061 7468 290a  .save(viz_path).
+000017e0: 2020 2020 2020 2020 6e6f 6465 732e 6170          nodes.ap
+000017f0: 7065 6e64 2867 7261 7068 7669 7a5f 6865  pend(graphviz_he
+00001800: 6c70 6572 2e6e 6f64 655f 7374 6d74 286e  lper.node_stmt(n
+00001810: 6f64 655f 6e61 6d65 2869 292c 6772 6170  ode_name(i),grap
+00001820: 6876 697a 5f68 656c 7065 722e 6874 6d6c  hviz_helper.html
+00001830: 5f69 6d61 6765 2827 4454 2027 202b 2073  _image('DT ' + s
+00001840: 7472 2869 292c 7669 7a5f 7061 7468 292c  tr(i),viz_path),
+00001850: 4661 6c73 652c 636f 6c6f 7273 2929 0a20  False,colors)). 
+00001860: 2020 2072 6574 7572 6e20 6772 6170 6876     return graphv
+00001870: 697a 5f68 656c 7065 722e 6772 6964 5f6c  iz_helper.grid_l
+00001880: 6179 6f75 7428 2753 656c 6563 7465 6420  ayout('Selected 
+00001890: 4573 7469 6d61 746f 7273 272c 206e 6f64  Estimators', nod
+000018a0: 6573 2c5b 5d2c 4e6f 6e65 2c63 6f6c 6f72  es,[],None,color
+000018b0: 732c 7369 7a65 3d28 312c 6c65 6e28 7472  s,size=(1,len(tr
+000018c0: 6565 5f69 6e64 697a 6573 2929 2c20 6f72  ee_indizes)), or
+000018d0: 6965 6e74 6174 696f 6e3d 2754 4427 290a  ientation='TD').
+000018e0: 0a0a 0a0a 2020 2020 0a20 2020 200a 0a    ....    .    ..
```

### Comparing `validating_models-0.9.2/validating_models/visualizations/graphviz_helper.py` & `validating_models-0.9.3/validating_models/visualizations/graphviz_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,365 +1,365 @@
 00000000: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
 00000010: 6e70 0a66 726f 6d20 6474 7265 6576 697a  np.from dtreeviz
 00000020: 2e74 7265 6573 2069 6d70 6f72 7420 4454  .trees import DT
-00000030: 7265 6556 697a 0a69 6d70 6f72 7420 7465  reeViz.import te
-00000040: 6d70 6669 6c65 0a69 6d70 6f72 7420 6f73  mpfile.import os
-00000050: 0a66 726f 6d20 7661 6c69 6461 7469 6e67  .from validating
-00000060: 5f6d 6f64 656c 732e 7374 6174 7320 696d  _models.stats im
-00000070: 706f 7274 2067 6574 5f64 6563 6f72 6174  port get_decorat
-00000080: 6f72 0a0a 7469 6d65 5f70 6963 7475 7265  or..time_picture
-00000090: 5f63 6f70 6f73 6974 696f 6e20 3d20 6765  _coposition = ge
-000000a0: 745f 6465 636f 7261 746f 7228 2770 6963  t_decorator('pic
-000000b0: 7475 7265 5f63 6f6d 706f 7369 7469 6f6e  ture_composition
-000000c0: 2729 0a0a 746d 7020 3d20 7465 6d70 6669  ')..tmp = tempfi
-000000d0: 6c65 2e67 6574 7465 6d70 6469 7228 290a  le.gettempdir().
-000000e0: 0a63 6c61 7373 2044 5472 6565 5669 7a43  .class DTreeVizC
-000000f0: 6f6e 7628 4454 7265 6556 697a 293a 0a20  onv(DTreeViz):. 
-00000100: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00000110: 7365 6c66 2c20 646f 742c 2073 6361 6c65  self, dot, scale
-00000120: 3d31 2e30 293a 0a20 2020 2020 2020 2073  =1.0):.        s
-00000130: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
-00000140: 646f 742c 2073 6361 6c65 290a 2020 2020  dot, scale).    
-00000150: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-00000160: 6f64 0a20 2020 2064 6566 2066 726f 6d5f  od.    def from_
-00000170: 4454 7265 6556 697a 2864 7472 6565 7669  DTreeViz(dtreevi
-00000180: 7a29 3a0a 2020 2020 2020 2020 7265 7475  z):.        retu
-00000190: 726e 2044 5472 6565 5669 7a43 6f6e 7628  rn DTreeVizConv(
-000001a0: 6474 7265 6576 697a 2e64 6f74 2c20 6474  dtreeviz.dot, dt
-000001b0: 7265 6576 697a 2e73 6361 6c65 290a 0a20  reeviz.scale).. 
-000001c0: 2020 2040 7469 6d65 5f70 6963 7475 7265     @time_picture
-000001d0: 5f63 6f70 6f73 6974 696f 6e0a 2020 2020  _coposition.    
-000001e0: 6465 6620 7361 7665 2873 656c 662c 2066  def save(self, f
-000001f0: 696c 656e 616d 652c 2074 7261 6e73 7061  ilename, transpa
-00000200: 7265 6e74 203d 2054 7275 652c 2064 7069  rent = True, dpi
-00000210: 3d31 3030 3029 3a0a 0a20 2020 2020 2020  =1000):..       
-00000220: 2064 6f74 5f69 6478 203d 2066 696c 656e   dot_idx = filen
-00000230: 616d 652e 7269 6e64 6578 2827 2e27 290a  ame.rindex('.').
-00000240: 2020 2020 2020 2020 7376 675f 6669 6c65          svg_file
-00000250: 203d 2066 696c 656e 616d 655b 3a64 6f74   = filename[:dot
-00000260: 5f69 6478 5d20 2b20 272e 7376 6727 0a20  _idx] + '.svg'. 
-00000270: 2020 2020 2020 2073 7570 6572 2829 2e73         super().s
-00000280: 6176 6528 7376 675f 6669 6c65 290a 2020  ave(svg_file).  
-00000290: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-000002a0: 2041 6464 206d 6973 7369 6e67 2068 6561   Add missing hea
-000002b0: 6465 720a 2020 2020 2020 2020 6d69 7373  der.        miss
-000002c0: 696e 675f 6865 6164 6572 203d 2027 3c3f  ing_header = '<?
-000002d0: 786d 6c20 7665 7273 696f 6e3d 2231 2e30  xml version="1.0
-000002e0: 2220 656e 636f 6469 6e67 3d22 7574 662d  " encoding="utf-
-000002f0: 3822 2073 7461 6e64 616c 6f6e 653d 226e  8" standalone="n
-00000300: 6f22 3f3e 5c6e 3c21 444f 4354 5950 4520  o"?>\n<!DOCTYPE 
-00000310: 7376 6720 5055 424c 4943 2022 2d2f 2f57  svg PUBLIC "-//W
-00000320: 3343 2f2f 4454 4420 5356 4720 312e 312f  3C//DTD SVG 1.1/
-00000330: 2f45 4e22 2022 6874 7470 3a2f 2f77 7777  /EN" "http://www
-00000340: 2e77 332e 6f72 672f 4772 6170 6869 6373  .w3.org/Graphics
-00000350: 2f53 5647 2f31 2e31 2f44 5444 2f73 7667  /SVG/1.1/DTD/svg
-00000360: 3131 2e64 7464 223e 5c6e 270a 2020 2020  11.dtd">\n'.    
-00000370: 2020 2020 7769 7468 206f 7065 6e28 7376      with open(sv
-00000380: 675f 6669 6c65 2c20 2772 2729 2061 7320  g_file, 'r') as 
-00000390: 6f72 6967 696e 616c 3a0a 2020 2020 2020  original:.      
-000003a0: 2020 2020 2020 7376 675f 636f 6e74 656e        svg_conten
-000003b0: 7420 3d20 6f72 6967 696e 616c 2e72 6561  t = original.rea
-000003c0: 6428 290a 2020 2020 2020 2020 0a20 2020  d().        .   
-000003d0: 2020 2020 2069 6620 6669 6c65 6e61 6d65       if filename
-000003e0: 2e65 6e64 7377 6974 6828 272e 7376 6727  .endswith('.svg'
-000003f0: 293a 0a20 2020 2020 2020 2020 2020 2077  ):.            w
-00000400: 6974 6820 6f70 656e 2866 696c 656e 616d  ith open(filenam
-00000410: 652c 2027 7727 2920 6173 206e 6577 3a0a  e, 'w') as new:.
-00000420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000430: 6e65 772e 7772 6974 6528 6d69 7373 696e  new.write(missin
-00000440: 675f 6865 6164 6572 290a 2020 2020 2020  g_header).      
-00000450: 2020 2020 2020 2020 2020 6e65 772e 7772            new.wr
-00000460: 6974 6528 7376 675f 636f 6e74 656e 7429  ite(svg_content)
-00000470: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00000480: 2020 2020 2020 2020 2020 2069 6d70 6f72             impor
-00000490: 7420 6361 6972 6f73 7667 0a20 2020 2020  t cairosvg.     
-000004a0: 2020 2020 2020 2069 6d70 6f72 7420 696f         import io
-000004b0: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
-000004c0: 6d20 5049 4c20 696d 706f 7274 2049 6d61  m PIL import Ima
-000004d0: 6765 0a20 2020 2020 2020 2020 2020 206f  ge.            o
-000004e0: 7574 7075 745f 706e 6720 3d20 696f 2e42  utput_png = io.B
-000004f0: 7974 6573 494f 2829 0a20 2020 2020 2020  ytesIO().       
-00000500: 2020 2020 2063 6169 726f 7376 672e 7376       cairosvg.sv
-00000510: 6732 706e 6728 6279 7465 7374 7269 6e67  g2png(bytestring
-00000520: 3d73 7667 5f63 6f6e 7465 6e74 2c20 7772  =svg_content, wr
-00000530: 6974 655f 746f 3d6f 7574 7075 745f 706e  ite_to=output_pn
-00000540: 672c 2073 6361 6c65 3d64 7069 2f31 3030  g, scale=dpi/100
-00000550: 290a 2020 2020 2020 2020 2020 2020 696d  ).            im
-00000560: 203d 2049 6d61 6765 2e6f 7065 6e28 6f75   = Image.open(ou
-00000570: 7470 7574 5f70 6e67 290a 2020 2020 2020  tput_png).      
-00000580: 2020 2020 2020 6f75 7470 7574 5f70 6e67        output_png
-00000590: 2e63 6c6f 7365 2829 0a0a 2020 2020 2020  .close()..      
-000005a0: 2020 2020 2020 6966 2074 7261 6e73 7061        if transpa
-000005b0: 7265 6e74 3a0a 2020 2020 2020 2020 2020  rent:.          
-000005c0: 2020 2020 2020 696d 203d 2069 6d2e 636f        im = im.co
-000005d0: 6e76 6572 7428 2752 4742 4127 290a 2020  nvert('RGBA').  
-000005e0: 2020 2020 2020 2020 2020 2020 2020 6461                da
-000005f0: 7461 203d 206e 702e 6172 7261 7928 696d  ta = np.array(im
-00000600: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00000610: 2020 2370 7269 6e74 2864 6174 612e 7368    #print(data.sh
-00000620: 6170 6529 0a20 2020 2020 2020 2020 2020  ape).           
-00000630: 2020 2020 2072 6762 203d 2064 6174 615b       rgb = data[
-00000640: 3a2c 3a2c 3a33 5d0a 2020 2020 2020 2020  :,:,:3].        
-00000650: 2020 2020 2020 2020 7768 6974 6520 3d20          white = 
-00000660: 5b32 3535 2c32 3535 2c32 3535 5d0a 2020  [255,255,255].  
-00000670: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00000680: 616e 7370 6172 656e 7420 3d20 5b32 3535  ansparent = [255
-00000690: 2c32 3535 2c32 3535 2c30 5d0a 2020 2020  ,255,255,0].    
-000006a0: 2020 2020 2020 2020 2020 2020 6d61 736b              mask
-000006b0: 203d 206e 702e 616c 6c28 7267 6220 3d3d   = np.all(rgb ==
-000006c0: 2077 6869 7465 2c20 6178 6973 203d 202d   white, axis = -
-000006d0: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
-000006e0: 2020 2023 7072 696e 7428 6e70 2e73 756d     #print(np.sum
-000006f0: 286d 6173 6b29 290a 2020 2020 2020 2020  (mask)).        
-00000700: 2020 2020 2020 2020 6461 7461 5b6d 6173          data[mas
-00000710: 6b5d 203d 2074 7261 6e73 7061 7265 6e74  k] = transparent
-00000720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000730: 2069 6d20 3d20 496d 6167 652e 6672 6f6d   im = Image.from
-00000740: 6172 7261 7928 6461 7461 290a 0a20 2020  array(data)..   
-00000750: 2020 2020 2020 2020 2069 6d2e 7361 7665           im.save
-00000760: 2866 696c 656e 616d 6529 0a0a 0a0a 6465  (filename)....de
-00000770: 6620 6874 6d6c 5f6c 6162 656c 286c 6162  f html_label(lab
-00000780: 656c 2c20 636f 6c6f 722c 2073 697a 6529  el, color, size)
-00000790: 3a0a 2020 2020 2727 2752 6574 7572 6e73  :.    '''Returns
-000007a0: 2074 6865 2068 746d 6c20 7265 7072 6573   the html repres
-000007b0: 656e 7461 7469 6f6e 2074 6f20 7368 6f77  entation to show
-000007c0: 2061 206c 6162 656c 2069 6e20 6120 6874   a label in a ht
-000007d0: 6d6c 2074 6162 6c65 2e0a 2020 2020 2727  ml table..    ''
-000007e0: 270a 2020 2020 7265 7475 726e 2066 273c  '.    return f'<
-000007f0: 666f 6e74 2066 6163 653d 2248 656c 7665  font face="Helve
-00000800: 7469 6361 2220 636f 6c6f 723d 227b 636f  tica" color="{co
-00000810: 6c6f 727d 2220 706f 696e 742d 7369 7a65  lor}" point-size
-00000820: 3d22 7b73 697a 657d 223e 3c69 3e7b 6c61  ="{size}"><i>{la
-00000830: 6265 6c7d 3c2f 693e 3c2f 666f 6e74 3e27  bel}</i></font>'
-00000840: 0a0a 6465 6620 6874 6d6c 5f69 6d61 6765  ..def html_image
-00000850: 2868 746d 6c5f 6c61 6265 6c2c 2069 6d67  (html_label, img
-00000860: 5f70 6174 6829 3a0a 2020 2020 2727 2752  _path):.    '''R
-00000870: 6574 7572 6e73 2074 6865 2068 746d 6c20  eturns the html 
-00000880: 7265 7072 6573 656e 7461 7469 6f6e 2074  representation t
-00000890: 6f20 7368 6f77 2074 6865 206c 6162 656c  o show the label
-000008a0: 2061 626f 7665 2074 6865 2067 6976 656e   above the given
-000008b0: 2069 6d61 6765 2e0a 2020 2020 2727 270a   image..    '''.
-000008c0: 2020 2020 6874 6d6c 5f6c 6162 656c 5f72      html_label_r
-000008d0: 6f77 203d 2066 273c 7472 3e3c 7464 2043  ow = f'<tr><td C
-000008e0: 454c 4c50 4144 4449 4e47 3d22 3022 2043  ELLPADDING="0" C
-000008f0: 454c 4c53 5041 4349 4e47 3d22 3022 3e7b  ELLSPACING="0">{
-00000900: 6874 6d6c 5f6c 6162 656c 7d3c 2f74 643e  html_label}</td>
-00000910: 3c2f 7472 3e27 0a20 2020 2072 6574 7572  </tr>'.    retur
-00000920: 6e20 6622 2222 3c74 6162 6c65 2062 6f72  n f"""<table bor
-00000930: 6465 723d 2230 2220 4345 4c4c 424f 5244  der="0" CELLBORD
-00000940: 4552 3d22 3022 3e0a 2020 2020 2020 2020  ER="0">.        
-00000950: 7b68 746d 6c5f 6c61 6265 6c5f 726f 777d  {html_label_row}
-00000960: 0a20 2020 2020 2020 203c 7472 3e0a 2020  .        <tr>.  
-00000970: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
-00000980: 643e 3c69 6d67 2073 7263 3d22 7b69 6d67  d><img src="{img
-00000990: 5f70 6174 687d 222f 3e3c 2f74 643e 0a20  _path}"/></td>. 
-000009a0: 2020 2020 2020 203c 2f74 723e 0a20 2020         </tr>.   
-000009b0: 2020 2020 203c 2f74 6162 6c65 3e22 2222       </table>"""
-000009c0: 0a0a 6465 6620 6874 6d6c 5f6e 6f64 655f  ..def html_node_
-000009d0: 6c61 6265 6c28 6e6f 6465 2c20 636f 6c6f  label(node, colo
-000009e0: 722c 2073 697a 6529 3a0a 2020 2020 7265  r, size):.    re
-000009f0: 7475 726e 2068 746d 6c5f 6c61 6265 6c28  turn html_label(
-00000a00: 6622 4e6f 6465 207b 6e6f 6465 2e69 647d  f"Node {node.id}
-00000a10: 222c 636f 6c6f 722c 2073 697a 6529 0a0a  ",color, size)..
-00000a20: 6465 6620 6e6f 6465 5f73 746d 7428 6e6f  def node_stmt(no
-00000a30: 6465 5f6e 616d 652c 2068 746d 6c5f 636f  de_name, html_co
-00000a40: 6e74 656e 742c 2068 6967 686c 6967 6874  ntent, highlight
-00000a50: 3a62 6f6f 6c2c 2063 6f6c 6f72 7329 3a0a  :bool, colors):.
-00000a60: 2020 2020 6966 2068 6967 686c 6967 6874      if highlight
-00000a70: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00000a80: 2066 277b 6e6f 6465 5f6e 616d 657d 205b   f'{node_name} [
-00000a90: 6d61 7267 696e 3d22 3022 2073 6861 7065  margin="0" shape
-00000aa0: 3d62 6f78 2070 656e 7769 6474 683d 222e  =box penwidth=".
-00000ab0: 3522 2063 6f6c 6f72 3d22 7b63 6f6c 6f72  5" color="{color
-00000ac0: 735b 2268 6967 686c 6967 6874 225d 7d22  s["highlight"]}"
-00000ad0: 2073 7479 6c65 3d22 6461 7368 6564 2220   style="dashed" 
-00000ae0: 6c61 6265 6c3d 3c7b 6874 6d6c 5f63 6f6e  label=<{html_con
-00000af0: 7465 6e74 7d3e 5d27 200a 2020 2020 656c  tent}>]' .    el
-00000b00: 7365 3a20 0a20 2020 2020 2020 2072 6574  se: .        ret
-00000b10: 7572 6e20 6627 7b6e 6f64 655f 6e61 6d65  urn f'{node_name
-00000b20: 7d20 5b6d 6172 6769 6e3d 2230 2220 7368  } [margin="0" sh
-00000b30: 6170 653d 626f 7820 7065 6e77 6964 7468  ape=box penwidth
-00000b40: 3d22 3022 2063 6f6c 6f72 3d22 7b63 6f6c  ="0" color="{col
-00000b50: 6f72 735b 2274 6578 7422 5d7d 2220 6c61  ors["text"]}" la
-00000b60: 6265 6c3d 3c7b 6874 6d6c 5f63 6f6e 7465  bel=<{html_conte
-00000b70: 6e74 7d3e 5d27 0a0a 6465 6620 636c 7573  nt}>]'..def clus
-00000b80: 7465 725f 6e6f 6465 7328 636c 7573 7465  ter_nodes(cluste
-00000b90: 725f 6e61 6d65 2c20 6c61 6265 6c2c 206e  r_name, label, n
-00000ba0: 6f64 6573 293a 0a20 2020 206e 6577 6c69  odes):.    newli
-00000bb0: 6e65 203d 2022 5c6e 5c74 220a 2020 2020  ne = "\n\t".    
-00000bc0: 7265 7475 726e 2066 2727 2773 7562 6772  return f'''subgr
-00000bd0: 6170 6820 636c 7573 7465 725f 7b63 6c75  aph cluster_{clu
-00000be0: 7374 6572 5f6e 616d 657d 207b 7b0a 2020  ster_name} {{.  
-00000bf0: 2020 2020 2020 636f 6c6f 723d 6c69 6768        color=ligh
-00000c00: 7467 7265 793b 0a20 2020 2020 2020 206c  tgrey;.        l
-00000c10: 6162 656c 3d22 7b6c 6162 656c 7d22 3b0a  abel="{label}";.
-00000c20: 2020 2020 2020 2020 7b6e 6577 6c69 6e65          {newline
-00000c30: 2e6a 6f69 6e28 6e6f 6465 7329 7d0a 2020  .join(nodes)}.  
-00000c40: 2020 7d7d 0a20 2020 2027 2727 0a0a 6465    }}.    '''..de
-00000c50: 6620 636c 6173 735f 6c65 6765 6e64 5f67  f class_legend_g
-00000c60: 7228 7061 7468 293a 0a20 2020 2069 6620  r(path):.    if 
-00000c70: 7061 7468 2021 3d20 4e6f 6e65 3a0a 2020  path != None:.  
-00000c80: 2020 2020 2020 7265 7475 726e 2066 2727        return f''
-00000c90: 2773 7562 6772 6170 6820 636c 7573 7465  'subgraph cluste
-00000ca0: 725f 6c65 6765 6e64 207b 7b0a 2020 2020  r_legend {{.    
-00000cb0: 2020 2020 2020 2020 2020 2020 7374 796c              styl
-00000cc0: 653d 696e 7669 733b 0a20 2020 2020 2020  e=invis;.       
-00000cd0: 2020 2020 2020 2020 206c 6567 656e 6420           legend 
-00000ce0: 5b70 656e 7769 6474 683d 2230 2220 6d61  [penwidth="0" ma
-00000cf0: 7267 696e 3d22 3022 2073 6861 7065 3d62  rgin="0" shape=b
-00000d00: 6f78 206d 6172 6769 6e3d 2230 2e30 3322  ox margin="0.03"
-00000d10: 2077 6964 7468 3d2e 312c 2068 6569 6768   width=.1, heigh
-00000d20: 743d 2e31 206c 6162 656c 3d3c 0a20 2020  t=.1 label=<.   
-00000d30: 2020 2020 2020 2020 2020 2020 207b 6874               {ht
-00000d40: 6d6c 5f69 6d61 6765 2827 272c 2070 6174  ml_image('', pat
-00000d50: 6829 7d0a 2020 2020 2020 2020 2020 2020  h)}.            
-00000d60: 2020 2020 3e5d 0a20 2020 2020 2020 2020      >].         
-00000d70: 2020 207d 7d0a 2020 2020 2020 2020 2020     }}.          
-00000d80: 2020 2727 270a 2020 2020 656c 7365 3a0a    '''.    else:.
-00000d90: 2020 2020 2020 2020 7265 7475 726e 2027          return '
-00000da0: 270a 0a64 6566 2067 6574 5f69 6d61 6765  '..def get_image
-00000db0: 5f70 6174 6828 6964 656e 7469 6669 6572  _path(identifier
-00000dc0: 3a20 7374 7229 3a0a 2020 2020 7265 7475  : str):.    retu
-00000dd0: 726e 206f 732e 7061 7468 2e6a 6f69 6e28  rn os.path.join(
-00000de0: 746d 702c 6622 7b74 6d70 7d2f 7b69 6465  tmp,f"{tmp}/{ide
-00000df0: 6e74 6966 6965 727d 5f7b 6f73 2e67 6574  ntifier}_{os.get
-00000e00: 7069 6428 297d 2e73 7667 2229 0a0a 6465  pid()}.svg")..de
-00000e10: 6620 6772 6964 5f6c 6179 6f75 7428 7469  f grid_layout(ti
-00000e20: 746c 652c 206e 6f64 6573 2c20 6564 6765  tle, nodes, edge
-00000e30: 732c 206c 6567 656e 642c 2063 6f6c 6f72  s, legend, color
-00000e40: 732c 2073 697a 653d 4e6f 6e65 2c20 666f  s, size=None, fo
-00000e50: 6e74 6e61 6d65 3d27 4865 6c76 6574 6963  ntname='Helvetic
-00000e60: 6127 2c20 7363 616c 653d 312e 302c 206f  a', scale=1.0, o
-00000e70: 7269 656e 7461 7469 6f6e 203d 2027 4c52  rientation = 'LR
-00000e80: 2729 3a20 2320 4c52 206f 7220 5444 0a20  '): # LR or TD. 
-00000e90: 2020 206e 6f64 655f 6e61 6d65 7320 3d20     node_names = 
-00000ea0: 5b6e 6f64 652e 7370 6c69 7428 2220 222c  [node.split(" ",
-00000eb0: 3129 5b30 5d20 6966 206e 6f64 652e 7370  1)[0] if node.sp
-00000ec0: 6c69 7428 2220 222c 3129 5b30 5d20 213d  lit(" ",1)[0] !=
-00000ed0: 2027 7375 6267 7261 7068 2720 656c 7365   'subgraph' else
-00000ee0: 206e 6f64 652e 7370 6c69 7428 2220 222c   node.split(" ",
-00000ef0: 3229 5b31 5d20 666f 7220 6e6f 6465 2069  2)[1] for node i
-00000f00: 6e20 6e6f 6465 735d 0a20 2020 2069 6620  n nodes].    if 
-00000f10: 7369 7a65 203d 3d20 4e6f 6e65 3a0a 2020  size == None:.  
-00000f20: 2020 2020 2020 6772 6964 5f73 697a 6520        grid_size 
-00000f30: 3d20 696e 7428 6e70 2e63 6569 6c28 6e70  = int(np.ceil(np
-00000f40: 2e73 7172 7428 6c65 6e28 6e6f 6465 5f6e  .sqrt(len(node_n
-00000f50: 616d 6573 2929 2929 0a20 2020 2020 2020  ames)))).       
-00000f60: 2073 697a 6520 3d20 2867 7269 645f 7369   size = (grid_si
-00000f70: 7a65 2c67 7269 645f 7369 7a65 290a 0a20  ze,grid_size).. 
-00000f80: 2020 2073 697a 6520 3d20 6c69 7374 2873     size = list(s
-00000f90: 697a 6529 0a20 2020 206e 756d 5f6e 6f64  ize).    num_nod
-00000fa0: 6573 203d 2073 697a 655b 305d 202a 2073  es = size[0] * s
-00000fb0: 697a 655b 315d 0a0a 2020 2020 6269 675f  ize[1]..    big_
-00000fc0: 696e 6465 7820 3d20 3020 6966 2073 697a  index = 0 if siz
-00000fd0: 655b 305d 203e 2073 697a 655b 315d 2065  e[0] > size[1] e
-00000fe0: 6c73 6520 310a 0a20 2020 2077 6869 6c65  lse 1..    while
-00000ff0: 206e 756d 5f6e 6f64 6573 203e 3d20 6c65   num_nodes >= le
-00001000: 6e28 6e6f 6465 7329 202b 2073 697a 655b  n(nodes) + size[
-00001010: 6269 675f 696e 6465 785d 3a0a 2020 2020  big_index]:.    
-00001020: 2020 2020 7369 7a65 5b62 6967 5f69 6e64      size[big_ind
-00001030: 6578 5d20 3d20 7369 7a65 5b62 6967 5f69  ex] = size[big_i
-00001040: 6e64 6578 5d20 2d20 310a 2020 2020 2020  ndex] - 1.      
-00001050: 2020 6e75 6d5f 6e6f 6465 7320 3d20 7369    num_nodes = si
-00001060: 7a65 5b30 5d20 2a20 7369 7a65 5b31 5d0a  ze[0] * size[1].
-00001070: 2020 2020 0a20 2020 2077 6869 6c65 206e      .    while n
-00001080: 756d 5f6e 6f64 6573 203e 3d20 6c65 6e28  um_nodes >= len(
-00001090: 6e6f 6465 7329 202b 2073 697a 655b 2862  nodes) + size[(b
-000010a0: 6967 5f69 6e64 6578 202b 2031 2920 2520  ig_index + 1) % 
-000010b0: 325d 3a0a 2020 2020 2020 2020 7369 7a65  2]:.        size
-000010c0: 5b28 6269 675f 696e 6465 7820 2b20 3129  [(big_index + 1)
-000010d0: 2025 2032 5d20 3d20 7369 7a65 5b28 6269   % 2] = size[(bi
-000010e0: 675f 696e 6465 7820 2b20 3129 2025 2032  g_index + 1) % 2
-000010f0: 5d20 2d20 310a 2020 2020 2020 2020 6e75  ] - 1.        nu
-00001100: 6d5f 6e6f 6465 7320 3d20 7369 7a65 5b30  m_nodes = size[0
-00001110: 5d20 2a20 7369 7a65 5b31 5d0a 0a20 2020  ] * size[1]..   
-00001120: 2023 2046 696c 6c20 6772 6964 2077 6974   # Fill grid wit
-00001130: 6820 7370 6163 6568 6f6c 6465 7220 6e6f  h spaceholder no
-00001140: 6465 730a 2020 2020 6e75 6d5f 7370 6163  des.    num_spac
-00001150: 6568 6f6c 6465 7273 203d 2030 0a20 2020  eholders = 0.   
-00001160: 2077 6869 6c65 206c 656e 286e 6f64 6573   while len(nodes
-00001170: 2920 3c20 6e75 6d5f 6e6f 6465 733a 0a20  ) < num_nodes:. 
-00001180: 2020 2020 2020 206e 756d 5f73 7061 6365         num_space
-00001190: 686f 6c64 6572 7320 2b3d 2031 0a20 2020  holders += 1.   
-000011a0: 2020 2020 206e 6f64 6573 2e61 7070 656e       nodes.appen
-000011b0: 6428 6e6f 6465 5f73 746d 7428 6627 7370  d(node_stmt(f'sp
-000011c0: 6163 6568 6f6c 6465 727b 6e75 6d5f 7370  aceholder{num_sp
-000011d0: 6163 6568 6f6c 6465 7273 7d27 2c20 2727  aceholders}', ''
-000011e0: 2c20 4661 6c73 652c 2063 6f6c 6f72 7329  , False, colors)
-000011f0: 290a 2020 2020 2020 2020 6e6f 6465 5f6e  ).        node_n
-00001200: 616d 6573 2e61 7070 656e 6428 6627 7370  ames.append(f'sp
-00001210: 6163 6568 6f6c 6465 727b 6e75 6d5f 7370  aceholder{num_sp
-00001220: 6163 6568 6f6c 6465 7273 7d27 290a 0a20  aceholders}').. 
-00001230: 2020 206e 6f64 655f 6e61 6d65 7320 3d20     node_names = 
-00001240: 6e70 2e61 7272 6179 286e 6f64 655f 6e61  np.array(node_na
-00001250: 6d65 7329 2e72 6573 6861 7065 2828 7369  mes).reshape((si
-00001260: 7a65 5b30 5d2c 7369 7a65 5b31 5d29 290a  ze[0],size[1])).
-00001270: 2020 2020 2320 4372 6561 7465 2067 7269      # Create gri
-00001280: 6420 7374 7275 6374 7572 650a 2020 2020  d structure.    
-00001290: 6772 6964 5f65 6467 6573 203d 205b 5d0a  grid_edges = [].
-000012a0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-000012b0: 6765 2873 697a 655b 305d 293a 200a 2020  ge(size[0]): .  
-000012c0: 2020 2020 2020 2320 486f 7269 7a6f 6e74        # Horizont
-000012d0: 616c 2043 6f6e 6e65 6374 696f 6e73 0a20  al Connections. 
-000012e0: 2020 2020 2020 2076 6563 203d 206e 6f64         vec = nod
-000012f0: 655f 6e61 6d65 735b 692c 3a5d 0a20 2020  e_names[i,:].   
-00001300: 2020 2020 2076 6563 203d 206c 6973 7428       vec = list(
-00001310: 7665 632e 7265 7368 6170 6528 2d31 2c29  vec.reshape(-1,)
-00001320: 290a 2020 2020 2020 2020 6966 206c 656e  ).        if len
-00001330: 2876 6563 2920 3e20 313a 0a20 2020 2020  (vec) > 1:.     
-00001340: 2020 2020 2020 2067 7269 645f 6564 6765         grid_edge
-00001350: 732e 6170 7065 6e64 2827 7261 6e6b 3d73  s.append('rank=s
-00001360: 616d 6520 7b27 202b 2027 202d 2d20 272e  ame {' + ' -- '.
-00001370: 6a6f 696e 2876 6563 2920 2b20 277d 2729  join(vec) + '}')
-00001380: 0a20 2020 200a 2020 2020 666f 7220 6a20  .    .    for j 
-00001390: 696e 2072 616e 6765 2873 697a 655b 315d  in range(size[1]
-000013a0: 293a 0a20 2020 2020 2020 2023 2056 6572  ):.        # Ver
-000013b0: 7469 6361 6c20 436f 6e6e 6563 7469 6f6e  tical Connection
-000013c0: 730a 2020 2020 2020 2020 7665 6320 3d20  s.        vec = 
-000013d0: 6e6f 6465 5f6e 616d 6573 5b3a 2c6a 5d0a  node_names[:,j].
-000013e0: 2020 2020 2020 2020 7665 6320 3d20 6c69          vec = li
-000013f0: 7374 2876 6563 2e72 6573 6861 7065 282d  st(vec.reshape(-
-00001400: 312c 2929 0a20 2020 2020 2020 2069 6620  1,)).        if 
-00001410: 6c65 6e28 7665 6329 203e 2031 3a0a 2020  len(vec) > 1:.  
-00001420: 2020 2020 2020 2020 2020 6772 6964 5f65            grid_e
-00001430: 6467 6573 2e61 7070 656e 6428 2720 2d2d  dges.append(' --
-00001440: 2027 2e6a 6f69 6e28 7665 6329 290a 2020   '.join(vec)).  
-00001450: 2020 2020 2020 0a20 2020 2020 2020 2069        .        i
-00001460: 6620 6f72 6965 6e74 6174 696f 6e20 3d3d  f orientation ==
-00001470: 2027 4c52 2720 616e 6420 6a20 3d3d 2030   'LR' and j == 0
-00001480: 2061 6e64 206c 6567 656e 6420 213d 204e   and legend != N
-00001490: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000014a0: 2067 7269 645f 6564 6765 732e 6170 7065   grid_edges.appe
-000014b0: 6e64 2827 202d 2d20 6c65 6765 6e64 2729  nd(' -- legend')
-000014c0: 0a0a 0a20 2020 206e 6577 6c69 6e65 203d  ...    newline =
-000014d0: 2022 5c6e 5c74 220a 2020 2020 646f 7420   "\n\t".    dot 
-000014e0: 3d20 6627 2727 0a20 2020 2067 7261 7068  = f'''.    graph
-000014f0: 2047 207b 7b0a 2020 2020 2020 2020 7370   G {{.        sp
-00001500: 6c69 6e65 733d 6c69 6e65 3b0a 2020 2020  lines=line;.    
-00001510: 2020 2020 666f 6e74 6e61 6d65 3d22 7b66      fontname="{f
-00001520: 6f6e 746e 616d 657d 220a 2020 2020 2020  ontname}".      
-00001530: 2020 6e6f 6465 205b 666f 6e74 6e61 6d65    node [fontname
-00001540: 3d22 7b66 6f6e 746e 616d 657d 225d 0a20  ="{fontname}"]. 
-00001550: 2020 2020 2020 2065 6467 6520 5b66 6f6e         edge [fon
-00001560: 746e 616d 653d 227b 666f 6e74 6e61 6d65  tname="{fontname
-00001570: 7d22 5d0a 2020 2020 2020 2020 6c61 796f  }"].        layo
-00001580: 7574 3d64 6f74 0a20 2020 2020 2020 206c  ut=dot.        l
-00001590: 6162 656c 3d22 7b74 6974 6c65 7d22 0a20  abel="{title}". 
-000015a0: 2020 2020 2020 206c 6162 656c 6c6f 633d         labelloc=
-000015b0: 2274 220a 2020 2020 2020 2020 7261 6e6b  "t".        rank
-000015c0: 6469 723d 227b 6f72 6965 6e74 6174 696f  dir="{orientatio
-000015d0: 6e7d 220a 0a20 2020 2020 2020 207b 6e65  n}"..        {ne
-000015e0: 776c 696e 652e 6a6f 696e 286e 6f64 6573  wline.join(nodes
-000015f0: 297d 0a0a 2020 2020 2020 2020 7b6e 6577  )}..        {new
-00001600: 6c69 6e65 2e6a 6f69 6e28 6564 6765 7329  line.join(edges)
-00001610: 7d0a 0a20 2020 2020 2020 2065 6467 6520  }..        edge 
-00001620: 5b73 7479 6c65 3d69 6e76 6973 5d0a 0a20  [style=invis].. 
-00001630: 2020 2020 2020 207b 6e65 776c 696e 652e         {newline.
-00001640: 6a6f 696e 2867 7269 645f 6564 6765 7329  join(grid_edges)
-00001650: 7d0a 2020 2020 2020 2020 7b63 6c61 7373  }.        {class
-00001660: 5f6c 6567 656e 645f 6772 286c 6567 656e  _legend_gr(legen
-00001670: 6429 2069 6620 6c65 6765 6e64 2021 3d20  d) if legend != 
-00001680: 4e6f 6e65 2065 6c73 6520 2727 7d0a 0a20  None else ''}.. 
-00001690: 2020 207d 7d0a 2020 2020 2727 270a 2020     }}.    '''.  
-000016a0: 2020 7265 7475 726e 2044 5472 6565 5669    return DTreeVi
-000016b0: 7a43 6f6e 7628 646f 742c 2073 6361 6c65  zConv(dot, scale
-000016c0: 29                                       )
+00000030: 7265 6556 697a 4150 490a 696d 706f 7274  reeVizAPI.import
+00000040: 2074 656d 7066 696c 650a 696d 706f 7274   tempfile.import
+00000050: 206f 730a 6672 6f6d 2076 616c 6964 6174   os.from validat
+00000060: 696e 675f 6d6f 6465 6c73 2e73 7461 7473  ing_models.stats
+00000070: 2069 6d70 6f72 7420 6765 745f 6465 636f   import get_deco
+00000080: 7261 746f 720a 0a74 696d 655f 7069 6374  rator..time_pict
+00000090: 7572 655f 636f 706f 7369 7469 6f6e 203d  ure_coposition =
+000000a0: 2067 6574 5f64 6563 6f72 6174 6f72 2827   get_decorator('
+000000b0: 7069 6374 7572 655f 636f 6d70 6f73 6974  picture_composit
+000000c0: 696f 6e27 290a 0a74 6d70 203d 2074 656d  ion')..tmp = tem
+000000d0: 7066 696c 652e 6765 7474 656d 7064 6972  pfile.gettempdir
+000000e0: 2829 0a0a 636c 6173 7320 4454 7265 6556  ()..class DTreeV
+000000f0: 697a 436f 6e76 2844 5472 6565 5669 7a41  izConv(DTreeVizA
+00000100: 5049 293a 0a20 2020 2064 6566 205f 5f69  PI):.    def __i
+00000110: 6e69 745f 5f28 7365 6c66 2c20 646f 742c  nit__(self, dot,
+00000120: 2073 6361 6c65 3d31 2e30 293a 0a20 2020   scale=1.0):.   
+00000130: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
+00000140: 6e69 745f 5f28 646f 742c 2073 6361 6c65  nit__(dot, scale
+00000150: 290a 2020 2020 0a20 2020 2040 7374 6174  ).    .    @stat
+00000160: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
+00000170: 2066 726f 6d5f 4454 7265 6556 697a 2864   from_DTreeViz(d
+00000180: 7472 6565 7669 7a29 3a0a 2020 2020 2020  treeviz):.      
+00000190: 2020 7265 7475 726e 2044 5472 6565 5669    return DTreeVi
+000001a0: 7a43 6f6e 7628 6474 7265 6576 697a 2e64  zConv(dtreeviz.d
+000001b0: 6f74 2c20 6474 7265 6576 697a 2e73 6361  ot, dtreeviz.sca
+000001c0: 6c65 290a 0a20 2020 2040 7469 6d65 5f70  le)..    @time_p
+000001d0: 6963 7475 7265 5f63 6f70 6f73 6974 696f  icture_copositio
+000001e0: 6e0a 2020 2020 6465 6620 7361 7665 2873  n.    def save(s
+000001f0: 656c 662c 2066 696c 656e 616d 652c 2074  elf, filename, t
+00000200: 7261 6e73 7061 7265 6e74 203d 2054 7275  ransparent = Tru
+00000210: 652c 2064 7069 3d31 3030 3029 3a0a 0a20  e, dpi=1000):.. 
+00000220: 2020 2020 2020 2064 6f74 5f69 6478 203d         dot_idx =
+00000230: 2066 696c 656e 616d 652e 7269 6e64 6578   filename.rindex
+00000240: 2827 2e27 290a 2020 2020 2020 2020 7376  ('.').        sv
+00000250: 675f 6669 6c65 203d 2066 696c 656e 616d  g_file = filenam
+00000260: 655b 3a64 6f74 5f69 6478 5d20 2b20 272e  e[:dot_idx] + '.
+00000270: 7376 6727 0a20 2020 2020 2020 2073 7570  svg'.        sup
+00000280: 6572 2829 2e73 6176 6528 7376 675f 6669  er().save(svg_fi
+00000290: 6c65 290a 2020 2020 2020 2020 0a20 2020  le).        .   
+000002a0: 2020 2020 2023 2041 6464 206d 6973 7369       # Add missi
+000002b0: 6e67 2068 6561 6465 720a 2020 2020 2020  ng header.      
+000002c0: 2020 6d69 7373 696e 675f 6865 6164 6572    missing_header
+000002d0: 203d 2027 3c3f 786d 6c20 7665 7273 696f   = '<?xml versio
+000002e0: 6e3d 2231 2e30 2220 656e 636f 6469 6e67  n="1.0" encoding
+000002f0: 3d22 7574 662d 3822 2073 7461 6e64 616c  ="utf-8" standal
+00000300: 6f6e 653d 226e 6f22 3f3e 5c6e 3c21 444f  one="no"?>\n<!DO
+00000310: 4354 5950 4520 7376 6720 5055 424c 4943  CTYPE svg PUBLIC
+00000320: 2022 2d2f 2f57 3343 2f2f 4454 4420 5356   "-//W3C//DTD SV
+00000330: 4720 312e 312f 2f45 4e22 2022 6874 7470  G 1.1//EN" "http
+00000340: 3a2f 2f77 7777 2e77 332e 6f72 672f 4772  ://www.w3.org/Gr
+00000350: 6170 6869 6373 2f53 5647 2f31 2e31 2f44  aphics/SVG/1.1/D
+00000360: 5444 2f73 7667 3131 2e64 7464 223e 5c6e  TD/svg11.dtd">\n
+00000370: 270a 2020 2020 2020 2020 7769 7468 206f  '.        with o
+00000380: 7065 6e28 7376 675f 6669 6c65 2c20 2772  pen(svg_file, 'r
+00000390: 2729 2061 7320 6f72 6967 696e 616c 3a0a  ') as original:.
+000003a0: 2020 2020 2020 2020 2020 2020 7376 675f              svg_
+000003b0: 636f 6e74 656e 7420 3d20 6f72 6967 696e  content = origin
+000003c0: 616c 2e72 6561 6428 290a 2020 2020 2020  al.read().      
+000003d0: 2020 0a20 2020 2020 2020 2069 6620 6669    .        if fi
+000003e0: 6c65 6e61 6d65 2e65 6e64 7377 6974 6828  lename.endswith(
+000003f0: 272e 7376 6727 293a 0a20 2020 2020 2020  '.svg'):.       
+00000400: 2020 2020 2077 6974 6820 6f70 656e 2866       with open(f
+00000410: 696c 656e 616d 652c 2027 7727 2920 6173  ilename, 'w') as
+00000420: 206e 6577 3a0a 2020 2020 2020 2020 2020   new:.          
+00000430: 2020 2020 2020 6e65 772e 7772 6974 6528        new.write(
+00000440: 6d69 7373 696e 675f 6865 6164 6572 290a  missing_header).
+00000450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000460: 6e65 772e 7772 6974 6528 7376 675f 636f  new.write(svg_co
+00000470: 6e74 656e 7429 0a20 2020 2020 2020 2065  ntent).        e
+00000480: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00000490: 2069 6d70 6f72 7420 6361 6972 6f73 7667   import cairosvg
+000004a0: 0a20 2020 2020 2020 2020 2020 2069 6d70  .            imp
+000004b0: 6f72 7420 696f 0a20 2020 2020 2020 2020  ort io.         
+000004c0: 2020 2066 726f 6d20 5049 4c20 696d 706f     from PIL impo
+000004d0: 7274 2049 6d61 6765 0a20 2020 2020 2020  rt Image.       
+000004e0: 2020 2020 206f 7574 7075 745f 706e 6720       output_png 
+000004f0: 3d20 696f 2e42 7974 6573 494f 2829 0a20  = io.BytesIO(). 
+00000500: 2020 2020 2020 2020 2020 2063 6169 726f             cairo
+00000510: 7376 672e 7376 6732 706e 6728 6279 7465  svg.svg2png(byte
+00000520: 7374 7269 6e67 3d73 7667 5f63 6f6e 7465  string=svg_conte
+00000530: 6e74 2c20 7772 6974 655f 746f 3d6f 7574  nt, write_to=out
+00000540: 7075 745f 706e 672c 2073 6361 6c65 3d64  put_png, scale=d
+00000550: 7069 2f31 3030 290a 2020 2020 2020 2020  pi/100).        
+00000560: 2020 2020 696d 203d 2049 6d61 6765 2e6f      im = Image.o
+00000570: 7065 6e28 6f75 7470 7574 5f70 6e67 290a  pen(output_png).
+00000580: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+00000590: 7574 5f70 6e67 2e63 6c6f 7365 2829 0a0a  ut_png.close()..
+000005a0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+000005b0: 7261 6e73 7061 7265 6e74 3a0a 2020 2020  ransparent:.    
+000005c0: 2020 2020 2020 2020 2020 2020 696d 203d              im =
+000005d0: 2069 6d2e 636f 6e76 6572 7428 2752 4742   im.convert('RGB
+000005e0: 4127 290a 2020 2020 2020 2020 2020 2020  A').            
+000005f0: 2020 2020 6461 7461 203d 206e 702e 6172      data = np.ar
+00000600: 7261 7928 696d 290a 2020 2020 2020 2020  ray(im).        
+00000610: 2020 2020 2020 2020 2370 7269 6e74 2864          #print(d
+00000620: 6174 612e 7368 6170 6529 0a20 2020 2020  ata.shape).     
+00000630: 2020 2020 2020 2020 2020 2072 6762 203d             rgb =
+00000640: 2064 6174 615b 3a2c 3a2c 3a33 5d0a 2020   data[:,:,:3].  
+00000650: 2020 2020 2020 2020 2020 2020 2020 7768                wh
+00000660: 6974 6520 3d20 5b32 3535 2c32 3535 2c32  ite = [255,255,2
+00000670: 3535 5d0a 2020 2020 2020 2020 2020 2020  55].            
+00000680: 2020 2020 7472 616e 7370 6172 656e 7420      transparent 
+00000690: 3d20 5b32 3535 2c32 3535 2c32 3535 2c30  = [255,255,255,0
+000006a0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000006b0: 2020 6d61 736b 203d 206e 702e 616c 6c28    mask = np.all(
+000006c0: 7267 6220 3d3d 2077 6869 7465 2c20 6178  rgb == white, ax
+000006d0: 6973 203d 202d 3129 0a20 2020 2020 2020  is = -1).       
+000006e0: 2020 2020 2020 2020 2023 7072 696e 7428           #print(
+000006f0: 6e70 2e73 756d 286d 6173 6b29 290a 2020  np.sum(mask)).  
+00000700: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00000710: 7461 5b6d 6173 6b5d 203d 2074 7261 6e73  ta[mask] = trans
+00000720: 7061 7265 6e74 0a20 2020 2020 2020 2020  parent.         
+00000730: 2020 2020 2020 2069 6d20 3d20 496d 6167         im = Imag
+00000740: 652e 6672 6f6d 6172 7261 7928 6461 7461  e.fromarray(data
+00000750: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00000760: 6d2e 7361 7665 2866 696c 656e 616d 6529  m.save(filename)
+00000770: 0a0a 0a0a 6465 6620 6874 6d6c 5f6c 6162  ....def html_lab
+00000780: 656c 286c 6162 656c 2c20 636f 6c6f 722c  el(label, color,
+00000790: 2073 697a 6529 3a0a 2020 2020 2727 2752   size):.    '''R
+000007a0: 6574 7572 6e73 2074 6865 2068 746d 6c20  eturns the html 
+000007b0: 7265 7072 6573 656e 7461 7469 6f6e 2074  representation t
+000007c0: 6f20 7368 6f77 2061 206c 6162 656c 2069  o show a label i
+000007d0: 6e20 6120 6874 6d6c 2074 6162 6c65 2e0a  n a html table..
+000007e0: 2020 2020 2727 270a 2020 2020 7265 7475      '''.    retu
+000007f0: 726e 2066 273c 666f 6e74 2066 6163 653d  rn f'<font face=
+00000800: 2248 656c 7665 7469 6361 2220 636f 6c6f  "Helvetica" colo
+00000810: 723d 227b 636f 6c6f 727d 2220 706f 696e  r="{color}" poin
+00000820: 742d 7369 7a65 3d22 7b73 697a 657d 223e  t-size="{size}">
+00000830: 3c69 3e7b 6c61 6265 6c7d 3c2f 693e 3c2f  <i>{label}</i></
+00000840: 666f 6e74 3e27 0a0a 6465 6620 6874 6d6c  font>'..def html
+00000850: 5f69 6d61 6765 2868 746d 6c5f 6c61 6265  _image(html_labe
+00000860: 6c2c 2069 6d67 5f70 6174 6829 3a0a 2020  l, img_path):.  
+00000870: 2020 2727 2752 6574 7572 6e73 2074 6865    '''Returns the
+00000880: 2068 746d 6c20 7265 7072 6573 656e 7461   html representa
+00000890: 7469 6f6e 2074 6f20 7368 6f77 2074 6865  tion to show the
+000008a0: 206c 6162 656c 2061 626f 7665 2074 6865   label above the
+000008b0: 2067 6976 656e 2069 6d61 6765 2e0a 2020   given image..  
+000008c0: 2020 2727 270a 2020 2020 6874 6d6c 5f6c    '''.    html_l
+000008d0: 6162 656c 5f72 6f77 203d 2066 273c 7472  abel_row = f'<tr
+000008e0: 3e3c 7464 2043 454c 4c50 4144 4449 4e47  ><td CELLPADDING
+000008f0: 3d22 3022 2043 454c 4c53 5041 4349 4e47  ="0" CELLSPACING
+00000900: 3d22 3022 3e7b 6874 6d6c 5f6c 6162 656c  ="0">{html_label
+00000910: 7d3c 2f74 643e 3c2f 7472 3e27 0a20 2020  }</td></tr>'.   
+00000920: 2072 6574 7572 6e20 6622 2222 3c74 6162   return f"""<tab
+00000930: 6c65 2062 6f72 6465 723d 2230 2220 4345  le border="0" CE
+00000940: 4c4c 424f 5244 4552 3d22 3022 3e0a 2020  LLBORDER="0">.  
+00000950: 2020 2020 2020 7b68 746d 6c5f 6c61 6265        {html_labe
+00000960: 6c5f 726f 777d 0a20 2020 2020 2020 203c  l_row}.        <
+00000970: 7472 3e0a 2020 2020 2020 2020 2020 2020  tr>.            
+00000980: 2020 2020 3c74 643e 3c69 6d67 2073 7263      <td><img src
+00000990: 3d22 7b69 6d67 5f70 6174 687d 222f 3e3c  ="{img_path}"/><
+000009a0: 2f74 643e 0a20 2020 2020 2020 203c 2f74  /td>.        </t
+000009b0: 723e 0a20 2020 2020 2020 203c 2f74 6162  r>.        </tab
+000009c0: 6c65 3e22 2222 0a0a 6465 6620 6874 6d6c  le>"""..def html
+000009d0: 5f6e 6f64 655f 6c61 6265 6c28 6e6f 6465  _node_label(node
+000009e0: 2c20 636f 6c6f 722c 2073 697a 6529 3a0a  , color, size):.
+000009f0: 2020 2020 7265 7475 726e 2068 746d 6c5f      return html_
+00000a00: 6c61 6265 6c28 6622 4e6f 6465 207b 6e6f  label(f"Node {no
+00000a10: 6465 2e69 647d 222c 636f 6c6f 722c 2073  de.id}",color, s
+00000a20: 697a 6529 0a0a 6465 6620 6e6f 6465 5f73  ize)..def node_s
+00000a30: 746d 7428 6e6f 6465 5f6e 616d 652c 2068  tmt(node_name, h
+00000a40: 746d 6c5f 636f 6e74 656e 742c 2068 6967  tml_content, hig
+00000a50: 686c 6967 6874 3a62 6f6f 6c2c 2063 6f6c  hlight:bool, col
+00000a60: 6f72 7329 3a0a 2020 2020 6966 2068 6967  ors):.    if hig
+00000a70: 686c 6967 6874 3a0a 2020 2020 2020 2020  hlight:.        
+00000a80: 7265 7475 726e 2066 277b 6e6f 6465 5f6e  return f'{node_n
+00000a90: 616d 657d 205b 6d61 7267 696e 3d22 3022  ame} [margin="0"
+00000aa0: 2073 6861 7065 3d62 6f78 2070 656e 7769   shape=box penwi
+00000ab0: 6474 683d 222e 3522 2063 6f6c 6f72 3d22  dth=".5" color="
+00000ac0: 7b63 6f6c 6f72 735b 2268 6967 686c 6967  {colors["highlig
+00000ad0: 6874 225d 7d22 2073 7479 6c65 3d22 6461  ht"]}" style="da
+00000ae0: 7368 6564 2220 6c61 6265 6c3d 3c7b 6874  shed" label=<{ht
+00000af0: 6d6c 5f63 6f6e 7465 6e74 7d3e 5d27 200a  ml_content}>]' .
+00000b00: 2020 2020 656c 7365 3a20 0a20 2020 2020      else: .     
+00000b10: 2020 2072 6574 7572 6e20 6627 7b6e 6f64     return f'{nod
+00000b20: 655f 6e61 6d65 7d20 5b6d 6172 6769 6e3d  e_name} [margin=
+00000b30: 2230 2220 7368 6170 653d 626f 7820 7065  "0" shape=box pe
+00000b40: 6e77 6964 7468 3d22 3022 2063 6f6c 6f72  nwidth="0" color
+00000b50: 3d22 7b63 6f6c 6f72 735b 2274 6578 7422  ="{colors["text"
+00000b60: 5d7d 2220 6c61 6265 6c3d 3c7b 6874 6d6c  ]}" label=<{html
+00000b70: 5f63 6f6e 7465 6e74 7d3e 5d27 0a0a 6465  _content}>]'..de
+00000b80: 6620 636c 7573 7465 725f 6e6f 6465 7328  f cluster_nodes(
+00000b90: 636c 7573 7465 725f 6e61 6d65 2c20 6c61  cluster_name, la
+00000ba0: 6265 6c2c 206e 6f64 6573 293a 0a20 2020  bel, nodes):.   
+00000bb0: 206e 6577 6c69 6e65 203d 2022 5c6e 5c74   newline = "\n\t
+00000bc0: 220a 2020 2020 7265 7475 726e 2066 2727  ".    return f''
+00000bd0: 2773 7562 6772 6170 6820 636c 7573 7465  'subgraph cluste
+00000be0: 725f 7b63 6c75 7374 6572 5f6e 616d 657d  r_{cluster_name}
+00000bf0: 207b 7b0a 2020 2020 2020 2020 636f 6c6f   {{.        colo
+00000c00: 723d 6c69 6768 7467 7265 793b 0a20 2020  r=lightgrey;.   
+00000c10: 2020 2020 206c 6162 656c 3d22 7b6c 6162       label="{lab
+00000c20: 656c 7d22 3b0a 2020 2020 2020 2020 7b6e  el}";.        {n
+00000c30: 6577 6c69 6e65 2e6a 6f69 6e28 6e6f 6465  ewline.join(node
+00000c40: 7329 7d0a 2020 2020 7d7d 0a20 2020 2027  s)}.    }}.    '
+00000c50: 2727 0a0a 6465 6620 636c 6173 735f 6c65  ''..def class_le
+00000c60: 6765 6e64 5f67 7228 7061 7468 293a 0a20  gend_gr(path):. 
+00000c70: 2020 2069 6620 7061 7468 2021 3d20 4e6f     if path != No
+00000c80: 6e65 3a0a 2020 2020 2020 2020 7265 7475  ne:.        retu
+00000c90: 726e 2066 2727 2773 7562 6772 6170 6820  rn f'''subgraph 
+00000ca0: 636c 7573 7465 725f 6c65 6765 6e64 207b  cluster_legend {
+00000cb0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000cc0: 2020 7374 796c 653d 696e 7669 733b 0a20    style=invis;. 
+00000cd0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00000ce0: 6567 656e 6420 5b70 656e 7769 6474 683d  egend [penwidth=
+00000cf0: 2230 2220 6d61 7267 696e 3d22 3022 2073  "0" margin="0" s
+00000d00: 6861 7065 3d62 6f78 206d 6172 6769 6e3d  hape=box margin=
+00000d10: 2230 2e30 3322 2077 6964 7468 3d2e 312c  "0.03" width=.1,
+00000d20: 2068 6569 6768 743d 2e31 206c 6162 656c   height=.1 label
+00000d30: 3d3c 0a20 2020 2020 2020 2020 2020 2020  =<.             
+00000d40: 2020 207b 6874 6d6c 5f69 6d61 6765 2827     {html_image('
+00000d50: 272c 2070 6174 6829 7d0a 2020 2020 2020  ', path)}.      
+00000d60: 2020 2020 2020 2020 2020 3e5d 0a20 2020            >].   
+00000d70: 2020 2020 2020 2020 207d 7d0a 2020 2020           }}.    
+00000d80: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00000d90: 656c 7365 3a0a 2020 2020 2020 2020 7265  else:.        re
+00000da0: 7475 726e 2027 270a 0a64 6566 2067 6574  turn ''..def get
+00000db0: 5f69 6d61 6765 5f70 6174 6828 6964 656e  _image_path(iden
+00000dc0: 7469 6669 6572 3a20 7374 7229 3a0a 2020  tifier: str):.  
+00000dd0: 2020 7265 7475 726e 206f 732e 7061 7468    return os.path
+00000de0: 2e6a 6f69 6e28 746d 702c 6622 7b74 6d70  .join(tmp,f"{tmp
+00000df0: 7d2f 7b69 6465 6e74 6966 6965 727d 5f7b  }/{identifier}_{
+00000e00: 6f73 2e67 6574 7069 6428 297d 2e73 7667  os.getpid()}.svg
+00000e10: 2229 0a0a 6465 6620 6772 6964 5f6c 6179  ")..def grid_lay
+00000e20: 6f75 7428 7469 746c 652c 206e 6f64 6573  out(title, nodes
+00000e30: 2c20 6564 6765 732c 206c 6567 656e 642c  , edges, legend,
+00000e40: 2063 6f6c 6f72 732c 2073 697a 653d 4e6f   colors, size=No
+00000e50: 6e65 2c20 666f 6e74 6e61 6d65 3d27 4865  ne, fontname='He
+00000e60: 6c76 6574 6963 6127 2c20 7363 616c 653d  lvetica', scale=
+00000e70: 312e 302c 206f 7269 656e 7461 7469 6f6e  1.0, orientation
+00000e80: 203d 2027 4c52 2729 3a20 2320 4c52 206f   = 'LR'): # LR o
+00000e90: 7220 5444 0a20 2020 206e 6f64 655f 6e61  r TD.    node_na
+00000ea0: 6d65 7320 3d20 5b6e 6f64 652e 7370 6c69  mes = [node.spli
+00000eb0: 7428 2220 222c 3129 5b30 5d20 6966 206e  t(" ",1)[0] if n
+00000ec0: 6f64 652e 7370 6c69 7428 2220 222c 3129  ode.split(" ",1)
+00000ed0: 5b30 5d20 213d 2027 7375 6267 7261 7068  [0] != 'subgraph
+00000ee0: 2720 656c 7365 206e 6f64 652e 7370 6c69  ' else node.spli
+00000ef0: 7428 2220 222c 3229 5b31 5d20 666f 7220  t(" ",2)[1] for 
+00000f00: 6e6f 6465 2069 6e20 6e6f 6465 735d 0a20  node in nodes]. 
+00000f10: 2020 2069 6620 7369 7a65 203d 3d20 4e6f     if size == No
+00000f20: 6e65 3a0a 2020 2020 2020 2020 6772 6964  ne:.        grid
+00000f30: 5f73 697a 6520 3d20 696e 7428 6e70 2e63  _size = int(np.c
+00000f40: 6569 6c28 6e70 2e73 7172 7428 6c65 6e28  eil(np.sqrt(len(
+00000f50: 6e6f 6465 5f6e 616d 6573 2929 2929 0a20  node_names)))). 
+00000f60: 2020 2020 2020 2073 697a 6520 3d20 2867         size = (g
+00000f70: 7269 645f 7369 7a65 2c67 7269 645f 7369  rid_size,grid_si
+00000f80: 7a65 290a 0a20 2020 2073 697a 6520 3d20  ze)..    size = 
+00000f90: 6c69 7374 2873 697a 6529 0a20 2020 206e  list(size).    n
+00000fa0: 756d 5f6e 6f64 6573 203d 2073 697a 655b  um_nodes = size[
+00000fb0: 305d 202a 2073 697a 655b 315d 0a0a 2020  0] * size[1]..  
+00000fc0: 2020 6269 675f 696e 6465 7820 3d20 3020    big_index = 0 
+00000fd0: 6966 2073 697a 655b 305d 203e 2073 697a  if size[0] > siz
+00000fe0: 655b 315d 2065 6c73 6520 310a 0a20 2020  e[1] else 1..   
+00000ff0: 2077 6869 6c65 206e 756d 5f6e 6f64 6573   while num_nodes
+00001000: 203e 3d20 6c65 6e28 6e6f 6465 7329 202b   >= len(nodes) +
+00001010: 2073 697a 655b 6269 675f 696e 6465 785d   size[big_index]
+00001020: 3a0a 2020 2020 2020 2020 7369 7a65 5b62  :.        size[b
+00001030: 6967 5f69 6e64 6578 5d20 3d20 7369 7a65  ig_index] = size
+00001040: 5b62 6967 5f69 6e64 6578 5d20 2d20 310a  [big_index] - 1.
+00001050: 2020 2020 2020 2020 6e75 6d5f 6e6f 6465          num_node
+00001060: 7320 3d20 7369 7a65 5b30 5d20 2a20 7369  s = size[0] * si
+00001070: 7a65 5b31 5d0a 2020 2020 0a20 2020 2077  ze[1].    .    w
+00001080: 6869 6c65 206e 756d 5f6e 6f64 6573 203e  hile num_nodes >
+00001090: 3d20 6c65 6e28 6e6f 6465 7329 202b 2073  = len(nodes) + s
+000010a0: 697a 655b 2862 6967 5f69 6e64 6578 202b  ize[(big_index +
+000010b0: 2031 2920 2520 325d 3a0a 2020 2020 2020   1) % 2]:.      
+000010c0: 2020 7369 7a65 5b28 6269 675f 696e 6465    size[(big_inde
+000010d0: 7820 2b20 3129 2025 2032 5d20 3d20 7369  x + 1) % 2] = si
+000010e0: 7a65 5b28 6269 675f 696e 6465 7820 2b20  ze[(big_index + 
+000010f0: 3129 2025 2032 5d20 2d20 310a 2020 2020  1) % 2] - 1.    
+00001100: 2020 2020 6e75 6d5f 6e6f 6465 7320 3d20      num_nodes = 
+00001110: 7369 7a65 5b30 5d20 2a20 7369 7a65 5b31  size[0] * size[1
+00001120: 5d0a 0a20 2020 2023 2046 696c 6c20 6772  ]..    # Fill gr
+00001130: 6964 2077 6974 6820 7370 6163 6568 6f6c  id with spacehol
+00001140: 6465 7220 6e6f 6465 730a 2020 2020 6e75  der nodes.    nu
+00001150: 6d5f 7370 6163 6568 6f6c 6465 7273 203d  m_spaceholders =
+00001160: 2030 0a20 2020 2077 6869 6c65 206c 656e   0.    while len
+00001170: 286e 6f64 6573 2920 3c20 6e75 6d5f 6e6f  (nodes) < num_no
+00001180: 6465 733a 0a20 2020 2020 2020 206e 756d  des:.        num
+00001190: 5f73 7061 6365 686f 6c64 6572 7320 2b3d  _spaceholders +=
+000011a0: 2031 0a20 2020 2020 2020 206e 6f64 6573   1.        nodes
+000011b0: 2e61 7070 656e 6428 6e6f 6465 5f73 746d  .append(node_stm
+000011c0: 7428 6627 7370 6163 6568 6f6c 6465 727b  t(f'spaceholder{
+000011d0: 6e75 6d5f 7370 6163 6568 6f6c 6465 7273  num_spaceholders
+000011e0: 7d27 2c20 2727 2c20 4661 6c73 652c 2063  }', '', False, c
+000011f0: 6f6c 6f72 7329 290a 2020 2020 2020 2020  olors)).        
+00001200: 6e6f 6465 5f6e 616d 6573 2e61 7070 656e  node_names.appen
+00001210: 6428 6627 7370 6163 6568 6f6c 6465 727b  d(f'spaceholder{
+00001220: 6e75 6d5f 7370 6163 6568 6f6c 6465 7273  num_spaceholders
+00001230: 7d27 290a 0a20 2020 206e 6f64 655f 6e61  }')..    node_na
+00001240: 6d65 7320 3d20 6e70 2e61 7272 6179 286e  mes = np.array(n
+00001250: 6f64 655f 6e61 6d65 7329 2e72 6573 6861  ode_names).resha
+00001260: 7065 2828 7369 7a65 5b30 5d2c 7369 7a65  pe((size[0],size
+00001270: 5b31 5d29 290a 2020 2020 2320 4372 6561  [1])).    # Crea
+00001280: 7465 2067 7269 6420 7374 7275 6374 7572  te grid structur
+00001290: 650a 2020 2020 6772 6964 5f65 6467 6573  e.    grid_edges
+000012a0: 203d 205b 5d0a 2020 2020 666f 7220 6920   = [].    for i 
+000012b0: 696e 2072 616e 6765 2873 697a 655b 305d  in range(size[0]
+000012c0: 293a 200a 2020 2020 2020 2020 2320 486f  ): .        # Ho
+000012d0: 7269 7a6f 6e74 616c 2043 6f6e 6e65 6374  rizontal Connect
+000012e0: 696f 6e73 0a20 2020 2020 2020 2076 6563  ions.        vec
+000012f0: 203d 206e 6f64 655f 6e61 6d65 735b 692c   = node_names[i,
+00001300: 3a5d 0a20 2020 2020 2020 2076 6563 203d  :].        vec =
+00001310: 206c 6973 7428 7665 632e 7265 7368 6170   list(vec.reshap
+00001320: 6528 2d31 2c29 290a 2020 2020 2020 2020  e(-1,)).        
+00001330: 6966 206c 656e 2876 6563 2920 3e20 313a  if len(vec) > 1:
+00001340: 0a20 2020 2020 2020 2020 2020 2067 7269  .            gri
+00001350: 645f 6564 6765 732e 6170 7065 6e64 2827  d_edges.append('
+00001360: 7261 6e6b 3d73 616d 6520 7b27 202b 2027  rank=same {' + '
+00001370: 202d 2d20 272e 6a6f 696e 2876 6563 2920   -- '.join(vec) 
+00001380: 2b20 277d 2729 0a20 2020 200a 2020 2020  + '}').    .    
+00001390: 666f 7220 6a20 696e 2072 616e 6765 2873  for j in range(s
+000013a0: 697a 655b 315d 293a 0a20 2020 2020 2020  ize[1]):.       
+000013b0: 2023 2056 6572 7469 6361 6c20 436f 6e6e   # Vertical Conn
+000013c0: 6563 7469 6f6e 730a 2020 2020 2020 2020  ections.        
+000013d0: 7665 6320 3d20 6e6f 6465 5f6e 616d 6573  vec = node_names
+000013e0: 5b3a 2c6a 5d0a 2020 2020 2020 2020 7665  [:,j].        ve
+000013f0: 6320 3d20 6c69 7374 2876 6563 2e72 6573  c = list(vec.res
+00001400: 6861 7065 282d 312c 2929 0a20 2020 2020  hape(-1,)).     
+00001410: 2020 2069 6620 6c65 6e28 7665 6329 203e     if len(vec) >
+00001420: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+00001430: 6772 6964 5f65 6467 6573 2e61 7070 656e  grid_edges.appen
+00001440: 6428 2720 2d2d 2027 2e6a 6f69 6e28 7665  d(' -- '.join(ve
+00001450: 6329 290a 2020 2020 2020 2020 0a20 2020  c)).        .   
+00001460: 2020 2020 2069 6620 6f72 6965 6e74 6174       if orientat
+00001470: 696f 6e20 3d3d 2027 4c52 2720 616e 6420  ion == 'LR' and 
+00001480: 6a20 3d3d 2030 2061 6e64 206c 6567 656e  j == 0 and legen
+00001490: 6420 213d 204e 6f6e 653a 0a20 2020 2020  d != None:.     
+000014a0: 2020 2020 2020 2067 7269 645f 6564 6765         grid_edge
+000014b0: 732e 6170 7065 6e64 2827 202d 2d20 6c65  s.append(' -- le
+000014c0: 6765 6e64 2729 0a0a 0a20 2020 206e 6577  gend')...    new
+000014d0: 6c69 6e65 203d 2022 5c6e 5c74 220a 2020  line = "\n\t".  
+000014e0: 2020 646f 7420 3d20 6627 2727 0a20 2020    dot = f'''.   
+000014f0: 2067 7261 7068 2047 207b 7b0a 2020 2020   graph G {{.    
+00001500: 2020 2020 7370 6c69 6e65 733d 6c69 6e65      splines=line
+00001510: 3b0a 2020 2020 2020 2020 666f 6e74 6e61  ;.        fontna
+00001520: 6d65 3d22 7b66 6f6e 746e 616d 657d 220a  me="{fontname}".
+00001530: 2020 2020 2020 2020 6e6f 6465 205b 666f          node [fo
+00001540: 6e74 6e61 6d65 3d22 7b66 6f6e 746e 616d  ntname="{fontnam
+00001550: 657d 225d 0a20 2020 2020 2020 2065 6467  e}"].        edg
+00001560: 6520 5b66 6f6e 746e 616d 653d 227b 666f  e [fontname="{fo
+00001570: 6e74 6e61 6d65 7d22 5d0a 2020 2020 2020  ntname}"].      
+00001580: 2020 6c61 796f 7574 3d64 6f74 0a20 2020    layout=dot.   
+00001590: 2020 2020 206c 6162 656c 3d22 7b74 6974       label="{tit
+000015a0: 6c65 7d22 0a20 2020 2020 2020 206c 6162  le}".        lab
+000015b0: 656c 6c6f 633d 2274 220a 2020 2020 2020  elloc="t".      
+000015c0: 2020 7261 6e6b 6469 723d 227b 6f72 6965    rankdir="{orie
+000015d0: 6e74 6174 696f 6e7d 220a 0a20 2020 2020  ntation}"..     
+000015e0: 2020 207b 6e65 776c 696e 652e 6a6f 696e     {newline.join
+000015f0: 286e 6f64 6573 297d 0a0a 2020 2020 2020  (nodes)}..      
+00001600: 2020 7b6e 6577 6c69 6e65 2e6a 6f69 6e28    {newline.join(
+00001610: 6564 6765 7329 7d0a 0a20 2020 2020 2020  edges)}..       
+00001620: 2065 6467 6520 5b73 7479 6c65 3d69 6e76   edge [style=inv
+00001630: 6973 5d0a 0a20 2020 2020 2020 207b 6e65  is]..        {ne
+00001640: 776c 696e 652e 6a6f 696e 2867 7269 645f  wline.join(grid_
+00001650: 6564 6765 7329 7d0a 2020 2020 2020 2020  edges)}.        
+00001660: 7b63 6c61 7373 5f6c 6567 656e 645f 6772  {class_legend_gr
+00001670: 286c 6567 656e 6429 2069 6620 6c65 6765  (legend) if lege
+00001680: 6e64 2021 3d20 4e6f 6e65 2065 6c73 6520  nd != None else 
+00001690: 2727 7d0a 0a20 2020 207d 7d0a 2020 2020  ''}..    }}.    
+000016a0: 2727 270a 2020 2020 7265 7475 726e 2044  '''.    return D
+000016b0: 5472 6565 5669 7a43 6f6e 7628 646f 742c  TreeVizConv(dot,
+000016c0: 2073 6361 6c65 29                         scale)
```

### Comparing `validating_models-0.9.2/validating_models/visualizations/regression.py` & `validating_models-0.9.3/validating_models/visualizations/regression.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.2/validating_models.egg-info/PKG-INFO` & `validating_models-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: validating-models
-Version: 0.9.2
+Name: validating_models
+Version: 0.9.3
 Summary: Supporting Explainable AI on Semantic Constraint Validation
 Home-page: https://github.com/JulianLoewe/Validating_Models
-Download-URL: https://github.com/JulianLoewe/Validating_Models/archive/refs/tags/v0.9.2.tar.gz
+Download-URL: https://github.com/JulianLoewe/Validating_Models/archive/refs/tags/v0.9.3.tar.gz
 Author: Julian Gercke
 License: GNU/GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `validating_models-0.9.2/validating_models.egg-info/SOURCES.txt` & `validating_models-0.9.3/validating_models.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 validating_models/__init__.py
 validating_models/checker.py
 validating_models/colors.py
 validating_models/constraint.py
 validating_models/dataset.py
 validating_models/drawing_utils.py
 validating_models/frequency_distribution_table.py
+validating_models/logger.py
 validating_models/shacl_validation_engine.py
 validating_models/stats.py
 validating_models.egg-info/PKG-INFO
 validating_models.egg-info/SOURCES.txt
 validating_models.egg-info/dependency_links.txt
 validating_models.egg-info/requires.txt
 validating_models.egg-info/top_level.txt
```

