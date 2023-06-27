# Comparing `tmp/mloptimizer-0.5.9.tar.gz` & `tmp/mloptimizer-0.5.9.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mloptimizer-0.5.9.tar", last modified: Sun Jun 25 10:12:25 2023, max compression
+gzip compressed data, was "mloptimizer-0.5.9.20.tar", last modified: Tue Jun 27 15:56:57 2023, max compression
```

## Comparing `mloptimizer-0.5.9.tar` & `mloptimizer-0.5.9.20.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:12:25.448268 mloptimizer-0.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-25 10:12:25.448268 mloptimizer-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:12:25.444268 mloptimizer-0.5.9/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1954444 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/data/data_sample.csv
--rw-r--r--   0 runner    (1001) docker     (123)   694332 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/data/data_sample_test.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1260187 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/data/data_sample_train.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:12:25.448268 mloptimizer-0.5.9/mloptimizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/alg_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    41176 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/genoptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/model_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:12:25.448268 mloptimizer-0.5.9/mloptimizer/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/test/test_TreeOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/test/test_XGBClassifierOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/test/test_alg_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/test/test_genoptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/mloptimizer/test/test_param.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:12:25.448268 mloptimizer-0.5.9/mloptimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-25 10:12:25.000000 mloptimizer-0.5.9/mloptimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-25 10:12:25.000000 mloptimizer-0.5.9/mloptimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 10:12:25.000000 mloptimizer-0.5.9/mloptimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-25 10:12:25.000000 mloptimizer-0.5.9/mloptimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 10:12:25.000000 mloptimizer-0.5.9/mloptimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 10:12:25.448268 mloptimizer-0.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-06-25 10:12:12.000000 mloptimizer-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:56:57.049287 mloptimizer-0.5.9.20/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-27 15:56:57.049287 mloptimizer-0.5.9.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:56:57.045287 mloptimizer-0.5.9.20/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1954444 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/data/data_sample.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   694332 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/data/data_sample_test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1260187 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/data/data_sample_train.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:56:57.045287 mloptimizer-0.5.9.20/mloptimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/mloptimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/mloptimizer/alg_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41454 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/mloptimizer/genoptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/mloptimizer/miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/mloptimizer/model_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/mloptimizer/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:56:57.049287 mloptimizer-0.5.9.20/mloptimizer/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/mloptimizer/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/mloptimizer/test/test_TreeOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/mloptimizer/test/test_XGBClassifierOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/mloptimizer/test/test_alg_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/mloptimizer/test/test_genoptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/mloptimizer/test/test_param.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:56:57.049287 mloptimizer-0.5.9.20/mloptimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-27 15:56:57.000000 mloptimizer-0.5.9.20/mloptimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-27 15:56:57.000000 mloptimizer-0.5.9.20/mloptimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 15:56:57.000000 mloptimizer-0.5.9.20/mloptimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-27 15:56:57.000000 mloptimizer-0.5.9.20/mloptimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 15:56:57.000000 mloptimizer-0.5.9.20/mloptimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 15:56:57.049287 mloptimizer-0.5.9.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-06-27 15:56:45.000000 mloptimizer-0.5.9.20/setup.py
```

### Comparing `mloptimizer-0.5.9/LICENSE` & `mloptimizer-0.5.9.20/LICENSE`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.9/PKG-INFO` & `mloptimizer-0.5.9.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mloptimizer
-Version: 0.5.9
+Version: 0.5.9.20
 Summary: mloptimizer is a Python library for optimizing hyperparameters of machine learning algorithms using genetic algorithms.
 Home-page: https://github.com/Caparrini/mloptimizer
 Author: Antonio Caparrini
 Author-email: acaparri@ucm.es
 Project-URL: Source, https://github.com/Caparrini/mloptimizer
 Keywords: xgboost,genetic,deap
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mloptimizer-0.5.9/README.md` & `mloptimizer-0.5.9.20/README.md`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.9/data/data_sample.csv` & `mloptimizer-0.5.9.20/data/data_sample.csv`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.9/data/data_sample_test.csv` & `mloptimizer-0.5.9.20/data/data_sample_test.csv`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.9/data/data_sample_train.csv` & `mloptimizer-0.5.9.20/data/data_sample_train.csv`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.9/mloptimizer/alg_wrapper.py` & `mloptimizer-0.5.9.20/mloptimizer/alg_wrapper.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.9/mloptimizer/genoptimizer.py` & `mloptimizer-0.5.9.20/mloptimizer/genoptimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from sklearn.neural_network import MLPClassifier
 from sklearn.svm import SVC
 from sklearn.tree import DecisionTreeClassifier
 
 from mloptimizer import miscellaneous
 from mloptimizer.alg_wrapper import CustomXGBClassifier, generate_model
 from mloptimizer.model_evaluation import kfold_stratified_score
-from mloptimizer.plots import plot_search_space, plot_logbook
+from mloptimizer.plots import plot_search_space, plot_logbook, plotly_logbook, plotly_search_space
 
 
 class Param(object):
     """
     Object to store param info, type and range of values
     """
 
@@ -398,21 +398,23 @@
         # self.file_out.write("Best accuracy: "+str(best_score[0])+"\n")
         # self.file_out.write("Best classifier(without parameter formating(DECIMALS)): "+str(self.get_clf(hof[0])))
         self._write_population_file()
         self._write_logbook_file()
         # self.plot_logbook(logbook=logbook)
         param_names = list(self.get_params().keys())
         param_names.append("fitness")
-        df = self.population_2_df()[param_names]
-        g = plot_search_space(df)
-        g.savefig(os.path.join(self.graphics_path, "search_space.png"))
+        population_df = self.population_2_df()
+        df = population_df[param_names]
+        g = plotly_search_space(df)
+        g.write_html(os.path.join(self.graphics_path, "search_space.html"))
         plt.close()
 
-        g2 = plot_logbook(self.logbook)
-        g2.savefig(os.path.join(self.graphics_path, "logbook.png"))
+        g2 = plotly_logbook(self.logbook, population_df)
+        #g2.savefig(os.path.join(self.graphics_path, "logbook.png"))
+        g2.write_html(os.path.join(self.graphics_path, "logbook.html"))
         plt.close()
 
         return self.get_clf(hof[0])
 
     def custom_ea_simple(self, population, toolbox, logbook,
                          cxpb, mutpb, start_gen=0, ngen=4, checkpoint_path=None, stats=None,
                          halloffame=None, verbose=__debug__, checkpoint_flag=True):
@@ -484,14 +486,15 @@
         # Begin the generational process
 
         for gen in range(start_gen, ngen + 1):
             progress_gen_path = os.path.join(self.progress_path, "Generation_{}.csv".format(gen))
             progress_gen_file = open(progress_gen_path, "w")
             header_progress_gen_file = "i;total;Individual;fitness\n"
             progress_gen_file.write(header_progress_gen_file)
+            progress_gen_file.close()
             self.optimization_logger.info("Generation: {}".format(gen))
             # Vary the pool of individuals
             population = varAnd(population, toolbox, cxpb, mutpb)
 
             # Evaluate the individuals with an invalid fitness
             invalid_ind = [ind for ind in population if not ind.fitness.valid]
             fitnesses = toolbox.map(toolbox.evaluate, invalid_ind)
@@ -501,19 +504,21 @@
                 self.optimization_logger.info(
                     "Fitting individual (informational purpose): gen {} - ind {} of {}".format(
                         gen, c, evaluations_pending
                     )
                 )
                 ind.fitness.values = fit
                 ind_formatted = self.individual2dict(ind)
+                progress_gen_file = open(progress_gen_path, "a")
                 progress_gen_file.write(
                     "{};{};{};{}\n".format(c,
                                            evaluations_pending,
                                            ind_formatted, fit)
                 )
+                progress_gen_file.close()
                 c = c + 1
 
             halloffame.update(population)
 
             record = stats.compile(population) if stats else {}
 
             logbook.record(gen=gen, nevals=len(invalid_ind), **record)
@@ -539,15 +544,14 @@
                 cp = dict(population=population, generation=gen, halloffame=halloffame,
                           logbook=logbook, rndstate=random.getstate())
 
                 cp_file = os.path.join(checkpoint_path, "cp_gen_{}.pkl".format(gen))
                 joblib.dump(cp, cp_file)
             self._write_population_file()
             self._write_logbook_file()
-            progress_gen_file.close()
 
         return population, logbook, halloffame
 
 
 class TreeOptimizer(BaseOptimizer, ABC):
     """
     Concrete optimizer for sklearn classifier -> sklearn.tree.DecisionTreeClassifier
```

### Comparing `mloptimizer-0.5.9/mloptimizer/miscellaneous.py` & `mloptimizer-0.5.9.20/mloptimizer/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.9/mloptimizer/model_evaluation.py` & `mloptimizer-0.5.9.20/mloptimizer/model_evaluation.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.9/mloptimizer/test/test_TreeOptimizer.py` & `mloptimizer-0.5.9.20/mloptimizer/test/test_TreeOptimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 def test_create_tree_optimizer(default_tree_optimizer):
     assert os.path.isdir(default_tree_optimizer.get_folder()) and os.path.exists(default_tree_optimizer.get_log_file())
     shutil.rmtree(default_tree_optimizer.get_folder())
 
 
 def test_create_custom_fixed_params_tree_optimizer(custom_fixed_params_tree_optimizer):
-    custom_fixed_params_tree_optimizer.optimize_clf(8, 10)
+    custom_fixed_params_tree_optimizer.optimize_clf(50, 30)
 
 
 def test_create_tree_optimizer2(default_tree_optimizer2):
     assert os.path.isdir(default_tree_optimizer2.get_folder()) and os.path.exists(
         default_tree_optimizer2.get_log_file())
     shutil.rmtree(default_tree_optimizer2.get_folder())
```

### Comparing `mloptimizer-0.5.9/mloptimizer/test/test_XGBClassifierOptimizer.py` & `mloptimizer-0.5.9.20/mloptimizer/test/test_XGBClassifierOptimizer.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.9/mloptimizer/test/test_alg_wrapper.py` & `mloptimizer-0.5.9.20/mloptimizer/test/test_alg_wrapper.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.9/mloptimizer/test/test_genoptimizer.py` & `mloptimizer-0.5.9.20/mloptimizer/test/test_genoptimizer.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.9/mloptimizer/test/test_param.py` & `mloptimizer-0.5.9.20/mloptimizer/test/test_param.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.9/mloptimizer.egg-info/PKG-INFO` & `mloptimizer-0.5.9.20/mloptimizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mloptimizer
-Version: 0.5.9
+Version: 0.5.9.20
 Summary: mloptimizer is a Python library for optimizing hyperparameters of machine learning algorithms using genetic algorithms.
 Home-page: https://github.com/Caparrini/mloptimizer
 Author: Antonio Caparrini
 Author-email: acaparri@ucm.es
 Project-URL: Source, https://github.com/Caparrini/mloptimizer
 Keywords: xgboost,genetic,deap
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mloptimizer-0.5.9/mloptimizer.egg-info/SOURCES.txt` & `mloptimizer-0.5.9.20/mloptimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.9/setup.py` & `mloptimizer-0.5.9.20/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     name="mloptimizer",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.5.9",  # Required
+    version="0.5.9.20",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="mloptimizer is a Python library "
                 "for optimizing hyperparameters of machine learning algorithms using genetic algorithms.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
@@ -122,15 +122,16 @@
         "pytz>=2022.7.1",
         "scikit-learn>=1.2.1",
         "scipy>=1.10.0",
         "seaborn==0.12.2",
         "six>=1.15.0",
         "tensorflow>=2.12.0",
         "xgboost>=1.7.3",
-        "matplotlib~=3.7.1"
+        #"matplotlib~=3.7.1",
+        "plotly>=5.15.0",
     ],  # Optional
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
```

