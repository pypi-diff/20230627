# Comparing `tmp/validating_models-0.9.3.tar.gz` & `tmp/validating_models-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validating_models-0.9.3.tar", last modified: Tue Jun 27 11:53:42 2023, max compression
+gzip compressed data, was "validating_models-0.9.4.tar", last modified: Tue Jun 27 12:27:05 2023, max compression
```

## Comparing `validating_models-0.9.3.tar` & `validating_models-0.9.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:53:42.163456 validating_models-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-27 11:53:25.000000 validating_models-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 11:53:25.000000 validating_models-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-27 11:53:42.163456 validating_models-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-27 11:53:25.000000 validating_models-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 11:53:42.163456 validating_models-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-27 11:53:25.000000 validating_models-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:53:42.155456 validating_models-0.9.3/validating_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    48649 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    43216 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/drawing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23815 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/frequency_distribution_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:53:42.159456 validating_models-0.9.3/validating_models/groupings/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/groupings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/groupings/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/groupings/decision_trees.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/groupings/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/groupings/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:53:42.159456 validating_models-0.9.3/validating_models/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/models/decision_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/models/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/shacl_validation_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:53:42.163456 validating_models-0.9.3/validating_models/visualizations/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/visualizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/visualizations/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    29424 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/visualizations/decision_trees.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/visualizations/ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/visualizations/graphviz_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-27 11:53:25.000000 validating_models-0.9.3/validating_models/visualizations/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:53:42.155456 validating_models-0.9.3/validating_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-27 11:53:42.000000 validating_models-0.9.3/validating_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-27 11:53:42.000000 validating_models-0.9.3/validating_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:53:42.000000 validating_models-0.9.3/validating_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-27 11:53:42.000000 validating_models-0.9.3/validating_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 11:53:42.000000 validating_models-0.9.3/validating_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:27:05.644250 validating_models-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-27 12:26:54.000000 validating_models-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 12:26:54.000000 validating_models-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-27 12:27:05.644250 validating_models-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-27 12:26:54.000000 validating_models-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 12:27:05.644250 validating_models-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-27 12:26:54.000000 validating_models-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:27:05.640250 validating_models-0.9.4/validating_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48649 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43216 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/drawing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23815 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/frequency_distribution_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:27:05.644250 validating_models-0.9.4/validating_models/groupings/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/groupings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/groupings/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/groupings/decision_trees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/groupings/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/groupings/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:27:05.644250 validating_models-0.9.4/validating_models/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/models/decision_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/models/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/shacl_validation_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:27:05.644250 validating_models-0.9.4/validating_models/visualizations/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/visualizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/visualizations/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29424 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/visualizations/decision_trees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/visualizations/ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/visualizations/graphviz_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-27 12:26:54.000000 validating_models-0.9.4/validating_models/visualizations/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:27:05.644250 validating_models-0.9.4/validating_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-27 12:27:05.000000 validating_models-0.9.4/validating_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-27 12:27:05.000000 validating_models-0.9.4/validating_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:27:05.000000 validating_models-0.9.4/validating_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-27 12:27:05.000000 validating_models-0.9.4/validating_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 12:27:05.000000 validating_models-0.9.4/validating_models.egg-info/top_level.txt
```

### Comparing `validating_models-0.9.3/LICENSE` & `validating_models-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/PKG-INFO` & `validating_models-0.9.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: validating_models
-Version: 0.9.3
+Version: 0.9.4
 Summary: Supporting Explainable AI on Semantic Constraint Validation
 Home-page: https://github.com/JulianLoewe/Validating_Models
-Download-URL: https://github.com/JulianLoewe/Validating_Models/archive/refs/tags/v0.9.3.tar.gz
+Download-URL: https://github.com/JulianLoewe/Validating_Models/archive/refs/tags/v0.9.4.tar.gz
 Author: Julian Gercke
 License: GNU/GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `validating_models-0.9.3/README.md` & `validating_models-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/setup.py` & `validating_models-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 import setuptools
 
-VERSION = '0.9.3'
+VERSION = '0.9.4'
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='validating_models',
     version=VERSION,
```

### Comparing `validating_models-0.9.3/validating_models/checker.py` & `validating_models-0.9.4/validating_models/checker.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/validating_models/colors.py` & `validating_models-0.9.4/validating_models/colors.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/validating_models/constraint.py` & `validating_models-0.9.4/validating_models/constraint.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/validating_models/dataset.py` & `validating_models-0.9.4/validating_models/dataset.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/validating_models/drawing_utils.py` & `validating_models-0.9.4/validating_models/drawing_utils.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/validating_models/frequency_distribution_table.py` & `validating_models-0.9.4/validating_models/frequency_distribution_table.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/validating_models/groupings/classification.py` & `validating_models-0.9.4/validating_models/groupings/classification.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/validating_models/groupings/decision_trees.py` & `validating_models-0.9.4/validating_models/groupings/decision_trees.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/validating_models/groupings/general.py` & `validating_models-0.9.4/validating_models/groupings/general.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/validating_models/groupings/random_forest.py` & `validating_models-0.9.4/validating_models/groupings/random_forest.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/validating_models/models/decision_tree.py` & `validating_models-0.9.4/validating_models/models/decision_tree.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from validating_models.logger import get_logger
 
 logger = get_logger('validating_models.models.decision_tree')
 time_node_samples = get_decorator('node_samples')
 
 def get_shadow_tree_from_checker(model, checker, tree_index=None) -> ShadowDecTree:
     dataset = checker.dataset
-    return ShadowDecTree.get_shadow_tree(model, x_data=dataset.x_data(), y_data=dataset.y_data(), feature_names=dataset.feature_names, target_name=dataset.target_name, class_names=dataset.class_names, tree_index=tree_index)
+    return ShadowDecTree.get_shadow_tree(model, X_train=dataset.x_data(), y_train=dataset.y_data(), feature_names=dataset.feature_names, target_name=dataset.target_name, class_names=dataset.class_names, tree_index=tree_index)
 
 
 def _get_single_node_samples(node: ShadowDecTreeNode):
     '''
     Fast methode to get the samples of a single node.
     '''
     model = node.shadow_tree.tree_model
-    x_data = node.shadow_tree.x_data
+    x_data = node.shadow_tree.X_train
     paths = model.decision_path(x_data)
     return list(paths[:,node.id].nonzero()[0])
 
 def get_single_node_samples(node: ShadowDecTreeNode, only_calculate_single_node=False):
     if only_calculate_single_node:
         return _get_single_node_samples(node)
     else:
@@ -36,23 +36,22 @@
     else:
         if get_hyperparameter_value('node_to_samples_non_optimized'):
             logger.info('Using non optimized node_samples on purpose!')
             result = tree.get_node_samples()
         else:
             try:
                 logger.info('Calculating node samples!')
-                dec_paths = tree.tree_model.decision_path(tree.x_data)
+                dec_paths = tree.tree_model.decision_path(tree.X_train)
                 dec_paths = dec_paths.tocsc()
 
                 n_nodes = dec_paths.shape[1]
                 node_to_samples = {}
                 for node_id in range(n_nodes):
                     node_to_samples[node_id] = list(dec_paths[:,node_id].nonzero()[0])
                 tree.node_to_samples = node_to_samples
                 result = tree.node_to_samples
             except:
                 result = tree.get_node_samples()
     new_entry('n_dnodes',len(result))
     new_entry('n_leaves',len(tree.leaves))
     new_entry('n_splitnodes',len(tree.internal))
     return result
-
```

### Comparing `validating_models-0.9.3/validating_models/models/random_forest.py` & `validating_models-0.9.4/validating_models/models/random_forest.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/validating_models/shacl_validation_engine.py` & `validating_models-0.9.4/validating_models/shacl_validation_engine.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/validating_models/stats.py` & `validating_models-0.9.4/validating_models/stats.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/validating_models/visualizations/classification.py` & `validating_models-0.9.4/validating_models/visualizations/classification.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/validating_models/visualizations/decision_trees.py` & `validating_models-0.9.4/validating_models/visualizations/decision_trees.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/validating_models/visualizations/ensembles.py` & `validating_models-0.9.4/validating_models/visualizations/ensembles.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/validating_models/visualizations/graphviz_helper.py` & `validating_models-0.9.4/validating_models/visualizations/graphviz_helper.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/validating_models/visualizations/regression.py` & `validating_models-0.9.4/validating_models/visualizations/regression.py`

 * *Files identical despite different names*

### Comparing `validating_models-0.9.3/validating_models.egg-info/PKG-INFO` & `validating_models-0.9.4/validating_models.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: validating-models
-Version: 0.9.3
+Version: 0.9.4
 Summary: Supporting Explainable AI on Semantic Constraint Validation
 Home-page: https://github.com/JulianLoewe/Validating_Models
-Download-URL: https://github.com/JulianLoewe/Validating_Models/archive/refs/tags/v0.9.3.tar.gz
+Download-URL: https://github.com/JulianLoewe/Validating_Models/archive/refs/tags/v0.9.4.tar.gz
 Author: Julian Gercke
 License: GNU/GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `validating_models-0.9.3/validating_models.egg-info/SOURCES.txt` & `validating_models-0.9.4/validating_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

