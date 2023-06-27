# Comparing `tmp/alhazen-py-0.0.2.tar.gz` & `tmp/alhazen-py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alhazen-py-0.0.2.tar", last modified: Mon Mar 20 14:31:23 2023, max compression
+gzip compressed data, was "alhazen-py-0.0.3.tar", last modified: Tue Jun 27 06:23:09 2023, max compression
```

## Comparing `alhazen-py-0.0.2.tar` & `alhazen-py-0.0.3.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-03-20 14:31:23.691621 alhazen-py-0.0.2/
--rw-r--r--   0 martineberlein   (501) staff       (20)     1072 2023-02-10 18:59:52.000000 alhazen-py-0.0.2/LICENSE
--rw-r--r--   0 martineberlein   (501) staff       (20)     5792 2023-03-20 14:31:23.691753 alhazen-py-0.0.2/PKG-INFO
--rw-r--r--   0 martineberlein   (501) staff       (20)     5083 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/README.md
--rw-r--r--   0 martineberlein   (501) staff       (20)     1017 2023-03-20 14:31:23.692666 alhazen-py-0.0.2/setup.cfg
--rw-r--r--   0 martineberlein   (501) staff       (20)       38 2023-01-16 15:33:54.000000 alhazen-py-0.0.2/setup.py
-drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-03-20 14:31:23.685984 alhazen-py-0.0.2/src/
-drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-03-20 14:31:23.687970 alhazen-py-0.0.2/src/alhazen/
--rw-r--r--   0 martineberlein   (501) staff       (20)       36 2023-02-13 08:28:25.000000 alhazen-py-0.0.2/src/alhazen/__init__.py
--rw-r--r--   0 martineberlein   (501) staff       (20)     4895 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/src/alhazen/alhazen.py
--rw-r--r--   0 martineberlein   (501) staff       (20)     4195 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/src/alhazen/feature_collector.py
--rw-r--r--   0 martineberlein   (501) staff       (20)    10020 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/src/alhazen/features.py
--rw-r--r--   0 martineberlein   (501) staff       (20)    12011 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/src/alhazen/generator.py
--rw-r--r--   0 martineberlein   (501) staff       (20)      967 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/src/alhazen/grammar_transformation.py
--rw-r--r--   0 martineberlein   (501) staff       (20)      571 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/src/alhazen/helper.py
--rw-r--r--   0 martineberlein   (501) staff       (20)     1840 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/src/alhazen/input.py
--rw-r--r--   0 martineberlein   (501) staff       (20)     5043 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/src/alhazen/input_specifications.py
--rw-r--r--   0 martineberlein   (501) staff       (20)     6519 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/src/alhazen/learner.py
--rw-r--r--   0 martineberlein   (501) staff       (20)      158 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/src/alhazen/oracle.py
--rw-r--r--   0 martineberlein   (501) staff       (20)     5752 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/src/alhazen/performance_evaluator.py
-drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-03-20 14:31:23.688493 alhazen-py-0.0.2/src/alhazen/requirementExtractionDT/
--rw-r--r--   0 martineberlein   (501) staff       (20)        0 2022-08-29 08:49:57.000000 alhazen-py-0.0.2/src/alhazen/requirementExtractionDT/__init__.py
--rw-r--r--   0 martineberlein   (501) staff       (20)     3654 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/src/alhazen/requirementExtractionDT/features.py
--rw-r--r--   0 martineberlein   (501) staff       (20)     5014 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/src/alhazen/requirementExtractionDT/requirements.py
--rw-r--r--   0 martineberlein   (501) staff       (20)     9035 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/src/alhazen/requirementExtractionDT/treetools.py
-drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-03-20 14:31:23.688934 alhazen-py-0.0.2/src/alhazen_formalizations/
--rw-r--r--   0 martineberlein   (501) staff       (20)        0 2023-02-13 08:28:25.000000 alhazen-py-0.0.2/src/alhazen_formalizations/__init__.py
--rw-r--r--   0 martineberlein   (501) staff       (20)     1655 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/src/alhazen_formalizations/calculator.py
--rw-r--r--   0 martineberlein   (501) staff       (20)     1302 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/src/alhazen_formalizations/heartbeat.py
-drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-03-20 14:31:23.689644 alhazen-py-0.0.2/src/alhazen_py.egg-info/
--rw-r--r--   0 martineberlein   (501) staff       (20)     5792 2023-03-20 14:31:23.000000 alhazen-py-0.0.2/src/alhazen_py.egg-info/PKG-INFO
--rw-r--r--   0 martineberlein   (501) staff       (20)     1046 2023-03-20 14:31:23.000000 alhazen-py-0.0.2/src/alhazen_py.egg-info/SOURCES.txt
--rw-r--r--   0 martineberlein   (501) staff       (20)        1 2023-03-20 14:31:23.000000 alhazen-py-0.0.2/src/alhazen_py.egg-info/dependency_links.txt
--rw-r--r--   0 martineberlein   (501) staff       (20)      179 2023-03-20 14:31:23.000000 alhazen-py-0.0.2/src/alhazen_py.egg-info/requires.txt
--rw-r--r--   0 martineberlein   (501) staff       (20)       31 2023-03-20 14:31:23.000000 alhazen-py-0.0.2/src/alhazen_py.egg-info/top_level.txt
-drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-03-20 14:31:23.691471 alhazen-py-0.0.2/tests/
--rw-r--r--   0 martineberlein   (501) staff       (20)     1178 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/tests/test_alhazen.py
--rw-r--r--   0 martineberlein   (501) staff       (20)    16858 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/tests/test_features.py
--rw-r--r--   0 martineberlein   (501) staff       (20)     3074 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/tests/test_generator.py
--rw-r--r--   0 martineberlein   (501) staff       (20)     3229 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/tests/test_learner.py
--rw-r--r--   0 martineberlein   (501) staff       (20)     8470 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/tests/test_requirements.py
--rw-r--r--   0 martineberlein   (501) staff       (20)     2109 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/tests/test_test_inputs.py
--rw-r--r--   0 martineberlein   (501) staff       (20)      922 2023-03-20 14:30:48.000000 alhazen-py-0.0.2/tests/test_transform_grammar.py
+drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-06-27 06:23:09.967346 alhazen-py-0.0.3/
+-rw-r--r--   0 martineberlein   (501) staff       (20)     1072 2023-02-10 19:03:43.000000 alhazen-py-0.0.3/LICENSE
+-rw-r--r--   0 martineberlein   (501) staff       (20)     5816 2023-06-27 06:23:09.967420 alhazen-py-0.0.3/PKG-INFO
+-rw-r--r--   0 martineberlein   (501) staff       (20)     5083 2023-03-04 09:34:15.000000 alhazen-py-0.0.3/README.md
+-rw-r--r--   0 martineberlein   (501) staff       (20)     1063 2023-06-27 06:23:09.967729 alhazen-py-0.0.3/setup.cfg
+-rw-r--r--   0 martineberlein   (501) staff       (20)       38 2023-02-10 19:03:43.000000 alhazen-py-0.0.3/setup.py
+drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-06-27 06:23:09.961554 alhazen-py-0.0.3/src/
+drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-06-27 06:23:09.963924 alhazen-py-0.0.3/src/alhazen/
+-rw-r--r--   0 martineberlein   (501) staff       (20)     5000 2023-06-08 12:20:49.000000 alhazen-py-0.0.3/src/alhazen/Alhazen.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)       36 2023-02-12 16:56:51.000000 alhazen-py-0.0.3/src/alhazen/__init__.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     4222 2023-05-23 09:00:15.000000 alhazen-py-0.0.3/src/alhazen/feature_collector.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)    10020 2023-02-23 13:05:34.000000 alhazen-py-0.0.3/src/alhazen/features.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)    12011 2023-02-27 11:50:59.000000 alhazen-py-0.0.3/src/alhazen/generator.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)      967 2023-02-17 07:55:27.000000 alhazen-py-0.0.3/src/alhazen/grammar_transformation.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)      677 2023-03-27 17:11:34.000000 alhazen-py-0.0.3/src/alhazen/helper.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     2014 2023-05-22 20:44:40.000000 alhazen-py-0.0.3/src/alhazen/input.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     5043 2023-02-23 15:40:04.000000 alhazen-py-0.0.3/src/alhazen/input_specifications.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     6519 2023-02-25 17:26:51.000000 alhazen-py-0.0.3/src/alhazen/learner.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)      209 2023-04-21 09:12:02.000000 alhazen-py-0.0.3/src/alhazen/oracle.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     5752 2023-03-04 11:01:34.000000 alhazen-py-0.0.3/src/alhazen/performance_evaluator.py
+drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-06-27 06:23:09.964425 alhazen-py-0.0.3/src/alhazen/requirementExtractionDT/
+-rw-r--r--   0 martineberlein   (501) staff       (20)        0 2023-02-10 19:03:43.000000 alhazen-py-0.0.3/src/alhazen/requirementExtractionDT/__init__.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     3654 2023-02-21 15:08:29.000000 alhazen-py-0.0.3/src/alhazen/requirementExtractionDT/features.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     5014 2023-02-23 12:59:34.000000 alhazen-py-0.0.3/src/alhazen/requirementExtractionDT/requirements.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     9035 2023-02-23 13:05:34.000000 alhazen-py-0.0.3/src/alhazen/requirementExtractionDT/treetools.py
+drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-06-27 06:23:09.964762 alhazen-py-0.0.3/src/alhazen_formalizations/
+-rw-r--r--   0 martineberlein   (501) staff       (20)        0 2023-02-10 19:41:46.000000 alhazen-py-0.0.3/src/alhazen_formalizations/__init__.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     1655 2023-02-27 11:31:04.000000 alhazen-py-0.0.3/src/alhazen_formalizations/calculator.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     1302 2023-03-04 10:48:33.000000 alhazen-py-0.0.3/src/alhazen_formalizations/heartbeat.py
+drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-06-27 06:23:09.965438 alhazen-py-0.0.3/src/alhazen_py.egg-info/
+-rw-r--r--   0 martineberlein   (501) staff       (20)     5816 2023-06-27 06:23:09.000000 alhazen-py-0.0.3/src/alhazen_py.egg-info/PKG-INFO
+-rw-r--r--   0 martineberlein   (501) staff       (20)     1110 2023-06-27 06:23:09.000000 alhazen-py-0.0.3/src/alhazen_py.egg-info/SOURCES.txt
+-rw-r--r--   0 martineberlein   (501) staff       (20)        1 2023-06-27 06:23:09.000000 alhazen-py-0.0.3/src/alhazen_py.egg-info/dependency_links.txt
+-rw-r--r--   0 martineberlein   (501) staff       (20)       45 2023-06-27 06:23:09.000000 alhazen-py-0.0.3/src/alhazen_py.egg-info/entry_points.txt
+-rw-r--r--   0 martineberlein   (501) staff       (20)      132 2023-06-27 06:23:09.000000 alhazen-py-0.0.3/src/alhazen_py.egg-info/requires.txt
+-rw-r--r--   0 martineberlein   (501) staff       (20)       31 2023-06-27 06:23:09.000000 alhazen-py-0.0.3/src/alhazen_py.egg-info/top_level.txt
+drwxr-xr-x   0 martineberlein   (501) staff       (20)        0 2023-06-27 06:23:09.966949 alhazen-py-0.0.3/tests/
+-rw-r--r--   0 martineberlein   (501) staff       (20)     1178 2023-02-23 13:06:48.000000 alhazen-py-0.0.3/tests/test_alhazen.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)    16858 2023-02-21 15:08:29.000000 alhazen-py-0.0.3/tests/test_features.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     3074 2023-02-27 11:46:35.000000 alhazen-py-0.0.3/tests/test_generator.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     3229 2023-02-23 12:45:07.000000 alhazen-py-0.0.3/tests/test_learner.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     8470 2023-02-21 15:08:29.000000 alhazen-py-0.0.3/tests/test_requirements.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)     2109 2023-02-21 15:08:29.000000 alhazen-py-0.0.3/tests/test_test_inputs.py
+-rw-r--r--   0 martineberlein   (501) staff       (20)      922 2023-02-17 07:56:02.000000 alhazen-py-0.0.3/tests/test_transform_grammar.py
```

### Comparing `alhazen-py-0.0.2/LICENSE` & `alhazen-py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alhazen-py-0.0.2/PKG-INFO` & `alhazen-py-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: alhazen-py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python version of the debugging tool Alhazen
 Home-page: https://github.com/martineberlein/alhazen-py
 Author: Martin Eberlein
 Author-email: martin.eberlein@hu-berlin.de
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/martineberlein/alhazen-py/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [![Tests](https://github.com/martineberlein/alhazen-py/actions/workflows/test_alhazen.yml/badge.svg)](https://github.com/martineberlein/alhazen-py/actions/workflows/test_alhazen.yml)
 &nbsp;
```

### Comparing `alhazen-py-0.0.2/README.md` & `alhazen-py-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alhazen-py-0.0.2/setup.cfg` & `alhazen-py-0.0.3/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = alhazen-py
-version = 0.0.2
+version = 0.0.3
 description = Python version of the debugging tool Alhazen
 author = Martin Eberlein
 author_email = martin.eberlein@hu-berlin.de
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/martineberlein/alhazen-py
 project_urls = 
@@ -15,33 +15,37 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3.10
 	Operating System :: OS Independent
 	Topic :: Scientific/Engineering
 	Topic :: Software Development :: Testing
 
 [options]
+python_requires = >=3.10
 install_requires = 
-	fuzzingbook~=1.1
-	isla-solver~=1.10
-	islearn>=0.2.10
-	shap>=0.41
+	fuzzingbook>=1.1
+	isla-solver
+	islearn
 	lightgbm>=3.3.2
 	z3-solver>=4.10.2.0
-	pandas~=1.4.4
-	numpy~=1.23.2
-	scikit-learn~=1.1.2
+	pandas
+	numpy
+	scikit-learn
 packages = find:
 package_dir = =src
 
 [options.extras_require]
 dev = 
 	pytest>=7.2.0
 	twine
 	black
 
 [options.packages.find]
 where = ./src
 
+[options.entry_points]
+console_scripts = 
+	alhazen=alhazen.cli:main
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `alhazen-py-0.0.2/src/alhazen/alhazen.py` & `alhazen-py-0.0.3/src/alhazen/Alhazen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 import logging
 import sys
 from typing import List, Callable, Set, Union
 from pandas import DataFrame, concat
 
 from fuzzingbook.Grammars import Grammar, is_valid_grammar
 from fuzzingbook.Parser import EarleyParser
@@ -10,14 +9,15 @@
 
 from alhazen.input import Input
 from alhazen.learner import Learner, DecisionTreeLearner
 from alhazen.generator import SimpleGenerator, Generator
 from alhazen.oracle import OracleResult
 from alhazen.features import FeatureWrapper, STANDARD_FEATURES
 from alhazen.feature_collector import Collector
+from alhazen.helper import show_tree
 
 GENERATOR_TIMEOUT = 10  # timeout in seconds
 MAX_ITERATION = 20
 
 
 class Alhazen:
     def __init__(
@@ -137,7 +137,10 @@
 
     def _generate_inputs(self, input_specifications) -> Set[Input]:
         inputs = set()
         for specification in input_specifications:
             inputs.add(self._generator.generate(input_specification=specification))
 
         return inputs
+
+    def show_model(self):
+        return show_tree(self._models[-1], self._all_features)
```

### Comparing `alhazen-py-0.0.2/src/alhazen/feature_collector.py` & `alhazen-py-0.0.3/src/alhazen/feature_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,24 +16,24 @@
             features = STANDARD_FEATURES
         else:
             for feature in features:
                 assert isinstance(feature, FeatureWrapper)
 
         self._grammar: Grammar = grammar
         self._features: Set[FeatureWrapper] = features
-        self.all_features = self.get_all_features()
+        self.all_features: List[Feature] = self.get_all_features()
 
-    def get_all_features(self):
+    def get_all_features(self) -> List[Feature]:
         assert len(self._features) != 0
 
         features = []
         for feature_class in self._features:
-            features = features + feature_class.extract_from_grammar(
+            features.extend(feature_class.extract_from_grammar(
                 grammar=self._grammar
-            )
+            ))
         assert len(features) != 0, "Could not extract any features."
         return features
 
     def collect_features_from_list(self, test_inputs: Set[Input]) -> pandas.DataFrame:
         data = []
         for inp in test_inputs:
             data.append(self.collect_features(inp))
```

### Comparing `alhazen-py-0.0.2/src/alhazen/features.py` & `alhazen-py-0.0.3/src/alhazen/features.py`

 * *Files identical despite different names*

### Comparing `alhazen-py-0.0.2/src/alhazen/generator.py` & `alhazen-py-0.0.3/src/alhazen/generator.py`

 * *Files identical despite different names*

### Comparing `alhazen-py-0.0.2/src/alhazen/grammar_transformation.py` & `alhazen-py-0.0.3/src/alhazen/grammar_transformation.py`

 * *Files identical despite different names*

### Comparing `alhazen-py-0.0.2/src/alhazen/input.py` & `alhazen-py-0.0.3/src/alhazen/input.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,15 +36,20 @@
     def features(self, features_: Dict):
         self.__features = features_
 
     def __str__(self) -> str:
         return str(self.__tree)
 
     def __hash__(self):
-        return hash(self.__tree)
+        return hash(self.__tree.structural_hash())
+
+    def __eq__(self, other):
+        if not isinstance(other, DerivationTree):
+            return False
+        return self.__hash__() == other.__hash__()
 
     def __iter__(self) -> Generator[DerivationTree | OracleResult | None, None, None]:
         """
         Allows tuple unpacking: tree, oracle = input
 
         :return: An iterator of two elements: The derivation tree and the execution oracle.
         """
```

### Comparing `alhazen-py-0.0.2/src/alhazen/input_specifications.py` & `alhazen-py-0.0.3/src/alhazen/input_specifications.py`

 * *Files identical despite different names*

### Comparing `alhazen-py-0.0.2/src/alhazen/learner.py` & `alhazen-py-0.0.3/src/alhazen/learner.py`

 * *Files identical despite different names*

### Comparing `alhazen-py-0.0.2/src/alhazen/performance_evaluator.py` & `alhazen-py-0.0.3/src/alhazen/performance_evaluator.py`

 * *Files identical despite different names*

### Comparing `alhazen-py-0.0.2/src/alhazen/requirementExtractionDT/features.py` & `alhazen-py-0.0.3/src/alhazen/requirementExtractionDT/features.py`

 * *Files identical despite different names*

### Comparing `alhazen-py-0.0.2/src/alhazen/requirementExtractionDT/requirements.py` & `alhazen-py-0.0.3/src/alhazen/requirementExtractionDT/requirements.py`

 * *Files identical despite different names*

### Comparing `alhazen-py-0.0.2/src/alhazen/requirementExtractionDT/treetools.py` & `alhazen-py-0.0.3/src/alhazen/requirementExtractionDT/treetools.py`

 * *Files identical despite different names*

### Comparing `alhazen-py-0.0.2/src/alhazen_formalizations/calculator.py` & `alhazen-py-0.0.3/src/alhazen_formalizations/calculator.py`

 * *Files identical despite different names*

### Comparing `alhazen-py-0.0.2/src/alhazen_formalizations/heartbeat.py` & `alhazen-py-0.0.3/src/alhazen_formalizations/heartbeat.py`

 * *Files identical despite different names*

### Comparing `alhazen-py-0.0.2/src/alhazen_py.egg-info/PKG-INFO` & `alhazen-py-0.0.3/src/alhazen_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: alhazen-py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python version of the debugging tool Alhazen
 Home-page: https://github.com/martineberlein/alhazen-py
 Author: Martin Eberlein
 Author-email: martin.eberlein@hu-berlin.de
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/martineberlein/alhazen-py/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [![Tests](https://github.com/martineberlein/alhazen-py/actions/workflows/test_alhazen.yml/badge.svg)](https://github.com/martineberlein/alhazen-py/actions/workflows/test_alhazen.yml)
 &nbsp;
```

### Comparing `alhazen-py-0.0.2/src/alhazen_py.egg-info/SOURCES.txt` & `alhazen-py-0.0.3/src/alhazen_py.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
+src/alhazen/Alhazen.py
 src/alhazen/__init__.py
 src/alhazen/alhazen.py
 src/alhazen/feature_collector.py
 src/alhazen/features.py
 src/alhazen/generator.py
 src/alhazen/grammar_transformation.py
 src/alhazen/helper.py
@@ -20,14 +21,15 @@
 src/alhazen/requirementExtractionDT/treetools.py
 src/alhazen_formalizations/__init__.py
 src/alhazen_formalizations/calculator.py
 src/alhazen_formalizations/heartbeat.py
 src/alhazen_py.egg-info/PKG-INFO
 src/alhazen_py.egg-info/SOURCES.txt
 src/alhazen_py.egg-info/dependency_links.txt
+src/alhazen_py.egg-info/entry_points.txt
 src/alhazen_py.egg-info/requires.txt
 src/alhazen_py.egg-info/top_level.txt
 tests/test_alhazen.py
 tests/test_features.py
 tests/test_generator.py
 tests/test_learner.py
 tests/test_requirements.py
```

### Comparing `alhazen-py-0.0.2/tests/test_alhazen.py` & `alhazen-py-0.0.3/tests/test_alhazen.py`

 * *Files identical despite different names*

### Comparing `alhazen-py-0.0.2/tests/test_features.py` & `alhazen-py-0.0.3/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `alhazen-py-0.0.2/tests/test_generator.py` & `alhazen-py-0.0.3/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `alhazen-py-0.0.2/tests/test_learner.py` & `alhazen-py-0.0.3/tests/test_learner.py`

 * *Files identical despite different names*

### Comparing `alhazen-py-0.0.2/tests/test_requirements.py` & `alhazen-py-0.0.3/tests/test_requirements.py`

 * *Files identical despite different names*

### Comparing `alhazen-py-0.0.2/tests/test_test_inputs.py` & `alhazen-py-0.0.3/tests/test_test_inputs.py`

 * *Files identical despite different names*

### Comparing `alhazen-py-0.0.2/tests/test_transform_grammar.py` & `alhazen-py-0.0.3/tests/test_transform_grammar.py`

 * *Files identical despite different names*

