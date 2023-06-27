# Comparing `tmp/logiclearnertools-0.1.8.tar.gz` & `tmp/logiclearnertools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/nataliadittren/Desktop/workspace/logiclearnertools/dist/.tmp-8183y41f/logiclearnertools-0.1.8.tar", last modified: Wed Mar 29 19:12:32 2023, max compression
+gzip compressed data, was "/Users/nataliadittren/Desktop/workspace/logiclearnertools/dist/.tmp-440316am/logiclearnertools-0.1.9.tar", last modified: Tue Jun 27 21:35:57 2023, max compression
```

## Comparing `logiclearnertools-0.1.8.tar` & `logiclearnertools-0.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 nataliadittren   (502) staff       (20)        0 2023-03-29 19:12:32.681128 logiclearnertools-0.1.8/
--rw-r--r--   0 nataliadittren   (502) staff       (20)      291 2022-04-05 13:33:34.000000 logiclearnertools-0.1.8/AUTHORS.md
--rw-r--r--   0 nataliadittren   (502) staff       (20)    35149 2021-11-12 16:43:23.000000 logiclearnertools-0.1.8/LICENSE
--rw-r--r--   0 nataliadittren   (502) staff       (20)       49 2022-06-15 21:16:53.000000 logiclearnertools-0.1.8/MANIFEST.in
--rw-r--r--   0 nataliadittren   (502) staff       (20)      367 2023-03-29 19:12:32.680515 logiclearnertools-0.1.8/PKG-INFO
--rw-r--r--   0 nataliadittren   (502) staff       (20)       22 2021-11-12 16:44:34.000000 logiclearnertools-0.1.8/README.md
-drwxr-xr-x   0 nataliadittren   (502) staff       (20)        0 2023-03-29 19:12:32.655905 logiclearnertools-0.1.8/logiclearnertools.egg-info/
--rw-r--r--   0 nataliadittren   (502) staff       (20)      367 2023-03-29 19:12:32.000000 logiclearnertools-0.1.8/logiclearnertools.egg-info/PKG-INFO
--rw-r--r--   0 nataliadittren   (502) staff       (20)     1174 2023-03-29 19:12:32.000000 logiclearnertools-0.1.8/logiclearnertools.egg-info/SOURCES.txt
--rw-r--r--   0 nataliadittren   (502) staff       (20)        1 2023-03-29 19:12:32.000000 logiclearnertools-0.1.8/logiclearnertools.egg-info/dependency_links.txt
--rw-r--r--   0 nataliadittren   (502) staff       (20)       11 2023-03-29 19:12:32.000000 logiclearnertools-0.1.8/logiclearnertools.egg-info/top_level.txt
-drwxr-xr-x   0 nataliadittren   (502) staff       (20)        0 2023-03-29 19:12:32.664943 logiclearnertools-0.1.8/logictools/
-drwxr-xr-x   0 nataliadittren   (502) staff       (20)        0 2023-03-29 19:12:32.671394 logiclearnertools-0.1.8/logictools/AI/
--rw-r--r--   0 nataliadittren   (502) staff       (20)        0 2022-06-13 19:16:10.000000 logiclearnertools-0.1.8/logictools/AI/__init__.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)      614 2022-06-13 19:16:10.000000 logiclearnertools-0.1.8/logictools/AI/astar_heuristic_weights.txt
--rw-r--r--   0 nataliadittren   (502) staff       (20)     4868 2023-03-28 19:22:44.000000 logiclearnertools-0.1.8/logictools/AI/astar_heuristics.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)     4740 2023-03-28 19:22:44.000000 logiclearnertools-0.1.8/logictools/AI/astar_search.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)     3287 2023-03-28 19:22:44.000000 logiclearnertools-0.1.8/logictools/AI/evaluate_astar_heuristic.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)     7383 2023-03-28 19:22:44.000000 logiclearnertools-0.1.8/logictools/AI/genetic_algorithm.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)      519 2022-06-13 19:16:10.000000 logiclearnertools-0.1.8/logictools/AI/grammar.lark
-drwxr-xr-x   0 nataliadittren   (502) staff       (20)        0 2023-03-29 19:12:32.679388 logiclearnertools-0.1.8/logictools/AI/neural_heuristic/
--rw-r--r--   0 nataliadittren   (502) staff       (20)        0 2023-03-28 19:22:44.000000 logiclearnertools-0.1.8/logictools/AI/neural_heuristic/__init__.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)     3674 2023-03-28 19:22:44.000000 logiclearnertools-0.1.8/logictools/AI/neural_heuristic/dataset.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)     3656 2023-03-28 19:22:44.000000 logiclearnertools-0.1.8/logictools/AI/neural_heuristic/model.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)     2380 2023-03-28 19:22:44.000000 logiclearnertools-0.1.8/logictools/AI/neural_heuristic/neural_embedding_heuristic.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)     1792 2023-03-28 19:22:44.000000 logiclearnertools-0.1.8/logictools/AI/neural_heuristic/sample_train_model.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)     6602 2023-03-28 19:22:44.000000 logiclearnertools-0.1.8/logictools/AI/neural_heuristic/sim_net.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)     4861 2023-03-28 19:22:44.000000 logiclearnertools-0.1.8/logictools/AI/neural_heuristic/train.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)     2760 2023-03-28 19:22:44.000000 logiclearnertools-0.1.8/logictools/AI/neural_heuristic/training_data_generator.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)        0 2022-03-02 19:37:55.000000 logiclearnertools-0.1.8/logictools/__init__.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)    11668 2023-03-28 19:22:44.000000 logiclearnertools-0.1.8/logictools/expression_parser.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)     6681 2022-03-02 19:37:55.000000 logiclearnertools-0.1.8/logictools/legacy_questions.json
--rw-r--r--   0 nataliadittren   (502) staff       (20)    20663 2023-03-28 19:22:44.000000 logiclearnertools-0.1.8/logictools/logic_rule_transforms.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)     1994 2023-03-28 19:22:44.000000 logiclearnertools-0.1.8/logictools/next_step.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)     1948 2023-03-28 19:22:44.000000 logiclearnertools-0.1.8/logictools/question_generator.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)    16899 2022-04-26 04:31:37.000000 logiclearnertools-0.1.8/logictools/questions.json
--rw-r--r--   0 nataliadittren   (502) staff       (20)     7568 2023-03-28 19:22:44.000000 logiclearnertools-0.1.8/logictools/test_expressionparser.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)     9470 2023-03-28 19:22:44.000000 logiclearnertools-0.1.8/logictools/test_logicruletransforms.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)     1273 2023-03-28 19:22:44.000000 logiclearnertools-0.1.8/logictools/test_solutions.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)      809 2022-03-02 19:37:55.000000 logiclearnertools-0.1.8/logictools/validation_exception.py
--rw-r--r--   0 nataliadittren   (502) staff       (20)       38 2023-03-29 19:12:32.681357 logiclearnertools-0.1.8/setup.cfg
--rw-r--r--   0 nataliadittren   (502) staff       (20)     2110 2023-03-29 19:08:03.000000 logiclearnertools-0.1.8/setup.py
+drwxr-xr-x   0 nataliadittren   (502) staff       (20)        0 2023-06-27 21:35:57.521796 logiclearnertools-0.1.9/
+-rw-r--r--   0 nataliadittren   (502) staff       (20)      291 2022-04-05 13:33:34.000000 logiclearnertools-0.1.9/AUTHORS.md
+-rw-r--r--   0 nataliadittren   (502) staff       (20)    35149 2021-11-12 16:43:23.000000 logiclearnertools-0.1.9/LICENSE
+-rw-r--r--   0 nataliadittren   (502) staff       (20)       49 2022-06-15 21:16:53.000000 logiclearnertools-0.1.9/MANIFEST.in
+-rw-r--r--   0 nataliadittren   (502) staff       (20)      367 2023-06-27 21:35:57.521170 logiclearnertools-0.1.9/PKG-INFO
+-rw-r--r--   0 nataliadittren   (502) staff       (20)       22 2021-11-12 16:44:34.000000 logiclearnertools-0.1.9/README.md
+drwxr-xr-x   0 nataliadittren   (502) staff       (20)        0 2023-06-27 21:35:57.503077 logiclearnertools-0.1.9/logiclearnertools.egg-info/
+-rw-r--r--   0 nataliadittren   (502) staff       (20)      367 2023-06-27 21:35:57.000000 logiclearnertools-0.1.9/logiclearnertools.egg-info/PKG-INFO
+-rw-r--r--   0 nataliadittren   (502) staff       (20)     1174 2023-06-27 21:35:57.000000 logiclearnertools-0.1.9/logiclearnertools.egg-info/SOURCES.txt
+-rw-r--r--   0 nataliadittren   (502) staff       (20)        1 2023-06-27 21:35:57.000000 logiclearnertools-0.1.9/logiclearnertools.egg-info/dependency_links.txt
+-rw-r--r--   0 nataliadittren   (502) staff       (20)       11 2023-06-27 21:35:57.000000 logiclearnertools-0.1.9/logiclearnertools.egg-info/top_level.txt
+drwxr-xr-x   0 nataliadittren   (502) staff       (20)        0 2023-06-27 21:35:57.509547 logiclearnertools-0.1.9/logictools/
+drwxr-xr-x   0 nataliadittren   (502) staff       (20)        0 2023-06-27 21:35:57.514881 logiclearnertools-0.1.9/logictools/AI/
+-rw-r--r--   0 nataliadittren   (502) staff       (20)        0 2022-06-13 19:16:10.000000 logiclearnertools-0.1.9/logictools/AI/__init__.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)      614 2022-06-13 19:16:10.000000 logiclearnertools-0.1.9/logictools/AI/astar_heuristic_weights.txt
+-rw-r--r--   0 nataliadittren   (502) staff       (20)     4868 2023-03-28 19:22:44.000000 logiclearnertools-0.1.9/logictools/AI/astar_heuristics.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)     4740 2023-03-28 19:22:44.000000 logiclearnertools-0.1.9/logictools/AI/astar_search.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)     3287 2023-03-28 19:22:44.000000 logiclearnertools-0.1.9/logictools/AI/evaluate_astar_heuristic.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)     7383 2023-03-28 19:22:44.000000 logiclearnertools-0.1.9/logictools/AI/genetic_algorithm.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)      519 2022-06-13 19:16:10.000000 logiclearnertools-0.1.9/logictools/AI/grammar.lark
+drwxr-xr-x   0 nataliadittren   (502) staff       (20)        0 2023-06-27 21:35:57.520206 logiclearnertools-0.1.9/logictools/AI/neural_heuristic/
+-rw-r--r--   0 nataliadittren   (502) staff       (20)        0 2023-03-28 19:22:44.000000 logiclearnertools-0.1.9/logictools/AI/neural_heuristic/__init__.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)     3674 2023-03-28 19:22:44.000000 logiclearnertools-0.1.9/logictools/AI/neural_heuristic/dataset.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)     3656 2023-03-28 19:22:44.000000 logiclearnertools-0.1.9/logictools/AI/neural_heuristic/model.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)     2380 2023-03-28 19:22:44.000000 logiclearnertools-0.1.9/logictools/AI/neural_heuristic/neural_embedding_heuristic.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)     1792 2023-03-28 19:22:44.000000 logiclearnertools-0.1.9/logictools/AI/neural_heuristic/sample_train_model.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)     6602 2023-03-28 19:22:44.000000 logiclearnertools-0.1.9/logictools/AI/neural_heuristic/sim_net.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)     4861 2023-03-28 19:22:44.000000 logiclearnertools-0.1.9/logictools/AI/neural_heuristic/train.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)     2760 2023-03-28 19:22:44.000000 logiclearnertools-0.1.9/logictools/AI/neural_heuristic/training_data_generator.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)        0 2022-03-02 19:37:55.000000 logiclearnertools-0.1.9/logictools/__init__.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)    11668 2023-03-28 19:22:44.000000 logiclearnertools-0.1.9/logictools/expression_parser.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)     6681 2022-03-02 19:37:55.000000 logiclearnertools-0.1.9/logictools/legacy_questions.json
+-rw-r--r--   0 nataliadittren   (502) staff       (20)    20663 2023-03-28 19:22:44.000000 logiclearnertools-0.1.9/logictools/logic_rule_transforms.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)     1994 2023-03-28 19:22:44.000000 logiclearnertools-0.1.9/logictools/next_step.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)     1948 2023-03-28 19:22:44.000000 logiclearnertools-0.1.9/logictools/question_generator.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)    16899 2022-04-26 04:31:37.000000 logiclearnertools-0.1.9/logictools/questions.json
+-rw-r--r--   0 nataliadittren   (502) staff       (20)     7568 2023-03-28 19:22:44.000000 logiclearnertools-0.1.9/logictools/test_expressionparser.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)     9470 2023-03-28 19:22:44.000000 logiclearnertools-0.1.9/logictools/test_logicruletransforms.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)     1273 2023-03-28 19:22:44.000000 logiclearnertools-0.1.9/logictools/test_solutions.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)      809 2022-03-02 19:37:55.000000 logiclearnertools-0.1.9/logictools/validation_exception.py
+-rw-r--r--   0 nataliadittren   (502) staff       (20)       38 2023-06-27 21:35:57.522066 logiclearnertools-0.1.9/setup.cfg
+-rw-r--r--   0 nataliadittren   (502) staff       (20)     2110 2023-06-27 21:35:04.000000 logiclearnertools-0.1.9/setup.py
```

### Comparing `logiclearnertools-0.1.8/LICENSE` & `logiclearnertools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logiclearnertools.egg-info/SOURCES.txt` & `logiclearnertools-0.1.9/logiclearnertools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/AI/astar_heuristic_weights.txt` & `logiclearnertools-0.1.9/logictools/AI/astar_heuristic_weights.txt`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/AI/astar_heuristics.py` & `logiclearnertools-0.1.9/logictools/AI/astar_heuristics.py`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/AI/astar_search.py` & `logiclearnertools-0.1.9/logictools/AI/astar_search.py`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/AI/evaluate_astar_heuristic.py` & `logiclearnertools-0.1.9/logictools/AI/evaluate_astar_heuristic.py`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/AI/genetic_algorithm.py` & `logiclearnertools-0.1.9/logictools/AI/genetic_algorithm.py`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/AI/grammar.lark` & `logiclearnertools-0.1.9/logictools/AI/grammar.lark`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/AI/neural_heuristic/dataset.py` & `logiclearnertools-0.1.9/logictools/AI/neural_heuristic/dataset.py`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/AI/neural_heuristic/model.py` & `logiclearnertools-0.1.9/logictools/AI/neural_heuristic/model.py`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/AI/neural_heuristic/neural_embedding_heuristic.py` & `logiclearnertools-0.1.9/logictools/AI/neural_heuristic/neural_embedding_heuristic.py`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/AI/neural_heuristic/sample_train_model.py` & `logiclearnertools-0.1.9/logictools/AI/neural_heuristic/sample_train_model.py`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/AI/neural_heuristic/sim_net.py` & `logiclearnertools-0.1.9/logictools/AI/neural_heuristic/sim_net.py`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/AI/neural_heuristic/train.py` & `logiclearnertools-0.1.9/logictools/AI/neural_heuristic/train.py`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/AI/neural_heuristic/training_data_generator.py` & `logiclearnertools-0.1.9/logictools/AI/neural_heuristic/training_data_generator.py`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/expression_parser.py` & `logiclearnertools-0.1.9/logictools/expression_parser.py`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/legacy_questions.json` & `logiclearnertools-0.1.9/logictools/legacy_questions.json`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/logic_rule_transforms.py` & `logiclearnertools-0.1.9/logictools/logic_rule_transforms.py`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/next_step.py` & `logiclearnertools-0.1.9/logictools/next_step.py`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/question_generator.py` & `logiclearnertools-0.1.9/logictools/question_generator.py`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/questions.json` & `logiclearnertools-0.1.9/logictools/questions.json`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/test_expressionparser.py` & `logiclearnertools-0.1.9/logictools/test_expressionparser.py`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/test_logicruletransforms.py` & `logiclearnertools-0.1.9/logictools/test_logicruletransforms.py`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/test_solutions.py` & `logiclearnertools-0.1.9/logictools/test_solutions.py`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/logictools/validation_exception.py` & `logiclearnertools-0.1.9/logictools/validation_exception.py`

 * *Files identical despite different names*

### Comparing `logiclearnertools-0.1.8/setup.py` & `logiclearnertools-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from setuptools import setup
 
 setup(
     name="logiclearnertools",
-    version="0.1.8",
+    version="0.1.9",
     author="Natalia Dittren, Columbia University Computer Science Faculty and Students",
     author_email="natalia.d@columbia.edu",
     url="https://github.com/ccnmtl/logiclearnertools",
     description="Logic Learner library",
     long_description="Logic Learner library",
     install_requires=[],
     scripts=[],
```

