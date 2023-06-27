# Comparing `tmp/TravSHACL-1.3.0.tar.gz` & `tmp/TravSHACL-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TravSHACL-1.3.0.tar", last modified: Fri Feb 17 09:48:47 2023, max compression
+gzip compressed data, was "TravSHACL-1.3.1.tar", last modified: Tue Jun 27 14:38:17 2023, max compression
```

## Comparing `TravSHACL-1.3.0.tar` & `TravSHACL-1.3.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 09:48:47.750461 TravSHACL-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-02-17 09:48:47.750461 TravSHACL-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 09:48:47.742461 TravSHACL-1.3.0/TravSHACL/
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/TravSHACL.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 09:48:47.742461 TravSHACL-1.3.0/TravSHACL/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/constraints/Constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/constraints/MaxOnlyConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/constraints/MinMaxConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/constraints/MinOnlyConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/constraints/SPARQLConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 09:48:47.746461 TravSHACL-1.3.0/TravSHACL/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/core/GraphTraversal.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/core/RulePattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/core/Shape.py
--rw-r--r--   0 runner    (1001) docker     (123)    19766 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/core/ShapeParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/core/ShapeSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 09:48:47.746461 TravSHACL-1.3.0/TravSHACL/rule_based_validation/
--rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/rule_based_validation/InstancesRetrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)    33825 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/rule_based_validation/Validation.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/rule_based_validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 09:48:47.746461 TravSHACL-1.3.0/TravSHACL/sparql/
--rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/sparql/QueryGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/sparql/SPARQLEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/sparql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 09:48:47.750461 TravSHACL-1.3.0/TravSHACL/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/utils/ValidationStats.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/utils/VariableGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/TravSHACL/utils/fileManagement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 09:48:47.742461 TravSHACL-1.3.0/TravSHACL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-02-17 09:48:47.000000 TravSHACL-1.3.0/TravSHACL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-02-17 09:48:47.000000 TravSHACL-1.3.0/TravSHACL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 09:48:47.000000 TravSHACL-1.3.0/TravSHACL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-17 09:48:47.000000 TravSHACL-1.3.0/TravSHACL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-17 09:48:47.000000 TravSHACL-1.3.0/TravSHACL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-02-17 09:48:47.750461 TravSHACL-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 09:48:47.750461 TravSHACL-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-02-17 09:48:38.000000 TravSHACL-1.3.0/tests/test_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:38:17.278545 TravSHACL-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-06-27 14:38:17.278545 TravSHACL-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:38:17.270545 TravSHACL-1.3.1/TravSHACL/
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/TravSHACL.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:38:17.274545 TravSHACL-1.3.1/TravSHACL/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/constraints/Constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/constraints/MaxOnlyConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/constraints/MinMaxConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/constraints/MinOnlyConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/constraints/SPARQLConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:38:17.274545 TravSHACL-1.3.1/TravSHACL/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/core/GraphTraversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/core/RulePattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/core/Shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19766 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/core/ShapeParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/core/ShapeSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:38:17.274545 TravSHACL-1.3.1/TravSHACL/rule_based_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/rule_based_validation/InstancesRetrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33764 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/rule_based_validation/Validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/rule_based_validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:38:17.278545 TravSHACL-1.3.1/TravSHACL/sparql/
+-rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/sparql/QueryGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/sparql/SPARQLEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/sparql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:38:17.278545 TravSHACL-1.3.1/TravSHACL/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/utils/ValidationStats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/utils/VariableGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/TravSHACL/utils/fileManagement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:38:17.270545 TravSHACL-1.3.1/TravSHACL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-06-27 14:38:17.000000 TravSHACL-1.3.1/TravSHACL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-27 14:38:17.000000 TravSHACL-1.3.1/TravSHACL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:38:17.000000 TravSHACL-1.3.1/TravSHACL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-27 14:38:17.000000 TravSHACL-1.3.1/TravSHACL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 14:38:17.000000 TravSHACL-1.3.1/TravSHACL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-27 14:38:17.278545 TravSHACL-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:38:17.278545 TravSHACL-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-27 14:38:06.000000 TravSHACL-1.3.1/tests/test_cases.py
```

### Comparing `TravSHACL-1.3.0/LICENSE` & `TravSHACL-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/PKG-INFO` & `TravSHACL-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TravSHACL
-Version: 1.3.0
+Version: 1.3.1
 Summary: A SHACL validator capable of planning the traversal and execution of the validation of a shape schema to detect violations early.
 Home-page: https://github.com/SDM-TIB/Trav-SHACL
-Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.3.0.tar.gz
+Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.3.1.tar.gz
 Author: Mónica Figuera, Philipp D. Rohde
 Author-email: philipp.rohde@tib.eu
 License: GNU/GPLv3
 Classifier: Development Status :: 5 - Production/Stable 
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `TravSHACL-1.3.0/README.md` & `TravSHACL-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/TravSHACL/TravSHACL.py` & `TravSHACL-1.3.1/TravSHACL/TravSHACL.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/TravSHACL/constraints/Constraint.py` & `TravSHACL-1.3.1/TravSHACL/constraints/Constraint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/TravSHACL/constraints/MaxOnlyConstraint.py` & `TravSHACL-1.3.1/TravSHACL/constraints/MaxOnlyConstraint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/TravSHACL/constraints/MinMaxConstraint.py` & `TravSHACL-1.3.1/TravSHACL/constraints/MinMaxConstraint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/TravSHACL/constraints/MinOnlyConstraint.py` & `TravSHACL-1.3.1/TravSHACL/constraints/MinOnlyConstraint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/TravSHACL/constraints/SPARQLConstraint.py` & `TravSHACL-1.3.1/TravSHACL/constraints/SPARQLConstraint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/TravSHACL/core/GraphTraversal.py` & `TravSHACL-1.3.1/TravSHACL/core/GraphTraversal.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/TravSHACL/core/RulePattern.py` & `TravSHACL-1.3.1/TravSHACL/core/RulePattern.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/TravSHACL/core/Shape.py` & `TravSHACL-1.3.1/TravSHACL/core/Shape.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/TravSHACL/core/ShapeParser.py` & `TravSHACL-1.3.1/TravSHACL/core/ShapeParser.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/TravSHACL/core/ShapeSchema.py` & `TravSHACL-1.3.1/TravSHACL/core/ShapeSchema.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/TravSHACL/rule_based_validation/InstancesRetrieval.py` & `TravSHACL-1.3.1/TravSHACL/rule_based_validation/InstancesRetrieval.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/TravSHACL/rule_based_validation/Validation.py` & `TravSHACL-1.3.1/TravSHACL/rule_based_validation/Validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
         state.shapes_state[focus_shape.get_id()]['remaining_targets_count'] = len(initial_targets)
 
         start = time.time() * 1000.0
         self.validate(state, focus_shape)
         finish = time.time() * 1000.0
         elapsed = round(finish - start)
         self.stats.record_total_time(elapsed)
-        print('Total execution time: ', str(elapsed), ' ms')
         self.stats.record_total_rules(state.total_rule_number)
         self.stats.update_log('\n\nMaximal number or rules in memory: ' + str(self.stats.max_rules))
         self.stats.update_log('\nTotal number of rules: ' + str(state.total_rule_number))
         return self.validation_output(state.shapes_state)
 
     def validate(self, state, focus_shape):
         """
```

### Comparing `TravSHACL-1.3.0/TravSHACL/sparql/QueryGenerator.py` & `TravSHACL-1.3.1/TravSHACL/sparql/QueryGenerator.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/TravSHACL/sparql/SPARQLEndpoint.py` & `TravSHACL-1.3.1/TravSHACL/sparql/SPARQLEndpoint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/TravSHACL/utils/ValidationStats.py` & `TravSHACL-1.3.1/TravSHACL/utils/ValidationStats.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/TravSHACL/utils/VariableGenerator.py` & `TravSHACL-1.3.1/TravSHACL/utils/VariableGenerator.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/TravSHACL/utils/fileManagement.py` & `TravSHACL-1.3.1/TravSHACL/utils/fileManagement.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/TravSHACL.egg-info/PKG-INFO` & `TravSHACL-1.3.1/TravSHACL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TravSHACL
-Version: 1.3.0
+Version: 1.3.1
 Summary: A SHACL validator capable of planning the traversal and execution of the validation of a shape schema to detect violations early.
 Home-page: https://github.com/SDM-TIB/Trav-SHACL
-Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.3.0.tar.gz
+Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.3.1.tar.gz
 Author: Mónica Figuera, Philipp D. Rohde
 Author-email: philipp.rohde@tib.eu
 License: GNU/GPLv3
 Classifier: Development Status :: 5 - Production/Stable 
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `TravSHACL-1.3.0/TravSHACL.egg-info/SOURCES.txt` & `TravSHACL-1.3.1/TravSHACL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/setup.py` & `TravSHACL-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.3.0/tests/test_cases.py` & `TravSHACL-1.3.1/tests/test_cases.py`

 * *Files identical despite different names*

