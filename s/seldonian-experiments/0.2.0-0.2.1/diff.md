# Comparing `tmp/seldonian_experiments-0.2.0.tar.gz` & `tmp/seldonian_experiments-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seldonian_experiments-0.2.0.tar", last modified: Fri May 26 15:37:18 2023, max compression
+gzip compressed data, was "seldonian_experiments-0.2.1.tar", last modified: Tue Jun 27 17:39:31 2023, max compression
```

## Comparing `seldonian_experiments-0.2.0.tar` & `seldonian_experiments-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-05-26 15:37:18.889847 seldonian_experiments-0.2.0/
--rw-r--r--   0 ahoag      (501) staff       (20)     1527 2022-04-25 15:36:26.000000 seldonian_experiments-0.2.0/LICENSE
--rw-r--r--   0 ahoag      (501) staff       (20)      816 2023-05-26 15:37:18.889677 seldonian_experiments-0.2.0/PKG-INFO
--rw-r--r--   0 ahoag      (501) staff       (20)      295 2022-11-11 21:28:20.000000 seldonian_experiments-0.2.0/README.md
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-05-26 15:37:18.883975 seldonian_experiments-0.2.0/examples/
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2023-03-09 21:51:03.000000 seldonian_experiments-0.2.0/examples/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4973 2023-03-27 18:38:58.000000 seldonian_experiments-0.2.0/examples/run_examples.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-05-26 15:37:18.887174 seldonian_experiments-0.2.0/experiments/
--rw-r--r--   0 ahoag      (501) staff       (20)       81 2023-03-09 00:38:52.000000 seldonian_experiments-0.2.0/experiments/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4062 2023-05-25 23:09:19.000000 seldonian_experiments-0.2.0/experiments/base_example.py
--rw-r--r--   0 ahoag      (501) staff       (20)    13564 2023-05-25 22:51:03.000000 seldonian_experiments-0.2.0/experiments/experiment_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)    44773 2023-05-25 23:07:24.000000 seldonian_experiments-0.2.0/experiments/experiments.py
--rw-r--r--   0 ahoag      (501) staff       (20)    39631 2023-05-25 22:09:58.000000 seldonian_experiments-0.2.0/experiments/generate_plots.py
--rw-r--r--   0 ahoag      (501) staff       (20)     3527 2023-05-25 22:54:38.000000 seldonian_experiments-0.2.0/experiments/headless_example.py
--rw-r--r--   0 ahoag      (501) staff       (20)    17446 2023-05-21 09:38:11.000000 seldonian_experiments-0.2.0/experiments/headless_experiments.py
--rw-r--r--   0 ahoag      (501) staff       (20)     8933 2023-04-25 19:01:34.000000 seldonian_experiments-0.2.0/experiments/headless_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2127 2023-05-08 15:32:53.000000 seldonian_experiments-0.2.0/experiments/perf_eval_funcs.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-05-26 15:37:18.888167 seldonian_experiments-0.2.0/seldonian_experiments.egg-info/
--rw-r--r--   0 ahoag      (501) staff       (20)      816 2023-05-26 15:37:18.000000 seldonian_experiments-0.2.0/seldonian_experiments.egg-info/PKG-INFO
--rw-r--r--   0 ahoag      (501) staff       (20)      680 2023-05-26 15:37:18.000000 seldonian_experiments-0.2.0/seldonian_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 ahoag      (501) staff       (20)        1 2023-05-26 15:37:18.000000 seldonian_experiments-0.2.0/seldonian_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 ahoag      (501) staff       (20)       17 2023-05-26 15:37:18.000000 seldonian_experiments-0.2.0/seldonian_experiments.egg-info/requires.txt
--rw-r--r--   0 ahoag      (501) staff       (20)       21 2023-05-26 15:37:18.000000 seldonian_experiments-0.2.0/seldonian_experiments.egg-info/top_level.txt
--rw-r--r--   0 ahoag      (501) staff       (20)       38 2023-05-26 15:37:18.889893 seldonian_experiments-0.2.0/setup.cfg
--rw-r--r--   0 ahoag      (501) staff       (20)      869 2023-05-26 15:37:03.000000 seldonian_experiments-0.2.0/setup.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-05-26 15:37:18.889320 seldonian_experiments-0.2.0/tests/
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-07-11 18:48:12.000000 seldonian_experiments-0.2.0/tests/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4257 2023-01-09 18:12:54.000000 seldonian_experiments-0.2.0/tests/conftest.py
--rw-r--r--   0 ahoag      (501) staff       (20)     9611 2023-05-26 14:48:12.000000 seldonian_experiments-0.2.0/tests/test_examples.py
--rw-r--r--   0 ahoag      (501) staff       (20)      848 2023-05-26 14:46:07.000000 seldonian_experiments-0.2.0/tests/test_experiments.py
--rw-r--r--   0 ahoag      (501) staff       (20)     9041 2023-05-22 23:02:27.000000 seldonian_experiments-0.2.0/tests/test_generate_plots.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-27 17:39:31.634804 seldonian_experiments-0.2.1/
+-rw-r--r--   0 ahoag      (501) staff       (20)     1527 2022-04-25 15:36:26.000000 seldonian_experiments-0.2.1/LICENSE
+-rw-r--r--   0 ahoag      (501) staff       (20)      816 2023-06-27 17:39:31.634636 seldonian_experiments-0.2.1/PKG-INFO
+-rw-r--r--   0 ahoag      (501) staff       (20)      295 2022-11-11 21:28:20.000000 seldonian_experiments-0.2.1/README.md
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-27 17:39:31.627881 seldonian_experiments-0.2.1/examples/
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2023-03-09 21:51:03.000000 seldonian_experiments-0.2.1/examples/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4973 2023-03-27 18:38:58.000000 seldonian_experiments-0.2.1/examples/run_examples.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-27 17:39:31.632115 seldonian_experiments-0.2.1/experiments/
+-rw-r--r--   0 ahoag      (501) staff       (20)       81 2023-03-09 00:38:52.000000 seldonian_experiments-0.2.1/experiments/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4062 2023-05-25 23:09:19.000000 seldonian_experiments-0.2.1/experiments/base_example.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    13506 2023-06-23 19:23:37.000000 seldonian_experiments-0.2.1/experiments/experiment_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    42671 2023-06-22 22:30:47.000000 seldonian_experiments-0.2.1/experiments/experiments.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    39631 2023-05-25 22:09:58.000000 seldonian_experiments-0.2.1/experiments/generate_plots.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     3527 2023-05-25 22:54:38.000000 seldonian_experiments-0.2.1/experiments/headless_example.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    17398 2023-06-22 22:33:01.000000 seldonian_experiments-0.2.1/experiments/headless_experiments.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     8933 2023-04-25 19:01:34.000000 seldonian_experiments-0.2.1/experiments/headless_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2127 2023-05-08 15:32:53.000000 seldonian_experiments-0.2.1/experiments/perf_eval_funcs.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-27 17:39:31.633050 seldonian_experiments-0.2.1/seldonian_experiments.egg-info/
+-rw-r--r--   0 ahoag      (501) staff       (20)      816 2023-06-27 17:39:31.000000 seldonian_experiments-0.2.1/seldonian_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 ahoag      (501) staff       (20)      680 2023-06-27 17:39:31.000000 seldonian_experiments-0.2.1/seldonian_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)        1 2023-06-27 17:39:31.000000 seldonian_experiments-0.2.1/seldonian_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)       17 2023-06-27 17:39:31.000000 seldonian_experiments-0.2.1/seldonian_experiments.egg-info/requires.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)       21 2023-06-27 17:39:31.000000 seldonian_experiments-0.2.1/seldonian_experiments.egg-info/top_level.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)       38 2023-06-27 17:39:31.634849 seldonian_experiments-0.2.1/setup.cfg
+-rw-r--r--   0 ahoag      (501) staff       (20)      869 2023-06-27 17:39:18.000000 seldonian_experiments-0.2.1/setup.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-27 17:39:31.634295 seldonian_experiments-0.2.1/tests/
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-07-11 18:48:12.000000 seldonian_experiments-0.2.1/tests/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4276 2023-06-27 16:43:15.000000 seldonian_experiments-0.2.1/tests/conftest.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     9611 2023-05-26 14:48:12.000000 seldonian_experiments-0.2.1/tests/test_examples.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      848 2023-05-26 14:46:07.000000 seldonian_experiments-0.2.1/tests/test_experiments.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     9041 2023-05-22 23:02:27.000000 seldonian_experiments-0.2.1/tests/test_generate_plots.py
```

### Comparing `seldonian_experiments-0.2.0/LICENSE` & `seldonian_experiments-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.0/PKG-INFO` & `seldonian_experiments-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seldonian_experiments
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library for running experiments with Seldonian algorithms
 Home-page: 
 Author: Austin Hoag
 Author-email: austinthomashoag@gmail.com
 Project-URL: Bug Tracker, https://github.com/seldonian-framework/Experiments/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `seldonian_experiments-0.2.0/examples/run_examples.py` & `seldonian_experiments-0.2.1/examples/run_examples.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.0/experiments/base_example.py` & `seldonian_experiments-0.2.1/experiments/base_example.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.0/experiments/experiment_utils.py` & `seldonian_experiments-0.2.1/experiments/experiment_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                 resamp_sensitive_attrs = []
 
             resampled_dataset = SupervisedDataSet(
                 features=resamp_features,
                 labels=resamp_labels,
                 sensitive_attrs=resamp_sensitive_attrs,
                 num_datapoints=num_datapoints,
-                meta_information=dataset.meta_information,
+                meta=dataset.meta,
             )
 
             with open(savename, "wb") as outfile:
                 pickle.dump(resampled_dataset, outfile)
             print(f"Saved {savename}")
 
 
@@ -161,15 +161,15 @@
         )
 
         dataset_for_exp = SupervisedDataSet(
             features=features,
             labels=labels,
             sensitive_attrs=sensitive_attrs,
             num_datapoints=n_points,
-            meta_information=trial_dataset.meta_information,
+            meta=trial_dataset.meta,
         )
 
         # Make a new spec object and update its dataset
         spec_for_exp = copy.deepcopy(spec)
         spec_for_exp.dataset = dataset_for_exp
 
     elif regime == "reinforcement_learning":
@@ -202,16 +202,15 @@
 
             # Take first n_episodes episodes
             episodes_for_exp = episodes_all[0:n_episodes_for_exp]
             assert len(episodes_for_exp) == n_episodes_for_exp
 
             dataset_for_exp = RLDataSet(
                 episodes=episodes_for_exp,
-                meta_information=spec.dataset.meta_information,
-                regime=regime,
+                meta=spec.dataset.meta,
             )
 
             # Make a new spec object from a copy of spec, where the
             # only thing that is different is the dataset
 
             spec_for_exp = copy.deepcopy(spec)
             spec_for_exp.dataset = dataset_for_exp
@@ -309,14 +308,16 @@
         and values are [batch_size,num_epochs]
     """
     data_sizes = (
         data_fracs * N_max
     )  # number of points used in candidate selection in each data frac
     n_batches = data_sizes / batch_size  # number of batches in each data frac
     n_batches = np.array([math.ceil(x) for x in n_batches])
+    print("n_batches:")
+    print(n_batches)
     n_epochs_arr = (
         niter / n_batches
     )  # number of epochs needed to get to niter iterations in each data frac
     n_epochs_arr = np.array([math.ceil(x) for x in n_epochs_arr])
     batch_epoch_dict = {
         data_fracs[ii]: [batch_size, n_epochs_arr[ii]] for ii in range(len(data_fracs))
     }
```

### Comparing `seldonian_experiments-0.2.0/experiments/experiments.py` & `seldonian_experiments-0.2.1/experiments/experiments.py`

 * *Files 3% similar despite different names*

```diff
@@ -295,64 +295,17 @@
                     **pred_kwargs,
                 )
             else:
                 y_pred = baseline_model.predict(
                     solution, 
                     X_test_baseline, 
                     **pred_kwargs)
-        except ValueError:
+        except (ValueError,IndexError):
             solution = "NSF"
 
-        # if self.model_name == "linear_regression":
-        #     baseline_model = LinearRegressionModel()
-        #     try:
-        #         solution = baseline_model.fit(features, labels)
-        #         y_pred = baseline_model.predict(solution, X_test_baseline)
-        #     except ValueError:
-        #         solution = "NSF"
-
-        # if self.model_name == "logistic_regression":
-        #     baseline_model = BinaryLogisticRegressionModel()
-        #     try:
-        #         solution = baseline_model.fit(features, labels)
-        #         # predict the probabilities not the class labels
-        #         y_pred = baseline_model.predict(solution, X_test_baseline)
-        #     except ValueError:
-        #         solution = "NSF"
-
-        # if self.model_name == "random_classifier":
-        #     # Returns the positive class with p=0.5 every time
-        #     baseline_model = RandomClassifierModel()
-        #     solution = None
-        #     y_pred = baseline_model.predict(solution, X_test_baseline)
-
-        # if self.model_name == "weighted_random_classifier":
-        #     # Returns the positive class with p=num_pos_class/num_neg_class every time
-        #     from .baselines.random_classifiers import WeightedRandomClassifierModel
-
-        #     baseline_model = WeightedRandomClassifierModel(0.4772833)
-        #     solution = None
-        #     y_pred = baseline_model.predict(solution, X_test_baseline)
-
-        # if self.model_name == "facial_recog_cnn":
-        #     from .baselines.facial_recog_cnn import PytorchFacialRecog
-
-        #     device = perf_eval_kwargs["device"]
-        #     baseline_model = PytorchFacialRecog(device=device)
-        #     batch_size, n_epochs = batch_epoch_dict[data_frac]
-        #     baseline_model.train(
-        #         features, labels, batch_size=batch_size, num_epochs=n_epochs
-        #     )
-        #     solution = baseline_model.get_model_params()
-        #     y_pred = batch_predictions(
-        #         baseline_model, solution, X_test_baseline, **perf_eval_kwargs
-        #     )
-
-        
-
         #########################################################
         """" Calculate performance and safety on ground truth """
         #########################################################
         # Handle whether solution was found
         solution_found = True
         if type(solution) == str and solution == "NSF":
             solution_found = False
@@ -732,15 +685,15 @@
                 constraint_eval_kwargs["dataset"] = spec_orig.dataset
 
             elif regime == "reinforcement_learning":
                 episodes_for_eval = constraint_eval_kwargs["episodes_for_eval"]
 
                 dataset_for_eval = RLDataSet(
                     episodes=episodes_for_eval,
-                    meta_information=spec_for_exp.dataset.meta_information,
+                    meta=spec_for_exp.dataset.meta,
                     regime=regime,
                 )
 
                 constraint_eval_kwargs["dataset"] = dataset_for_eval
 
             for parse_tree in spec_for_exp.parse_trees:
                 parse_tree.reset_base_node_dict(reset_data=True)
```

### Comparing `seldonian_experiments-0.2.0/experiments/generate_plots.py` & `seldonian_experiments-0.2.1/experiments/generate_plots.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.0/experiments/headless_example.py` & `seldonian_experiments-0.2.1/experiments/headless_example.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.0/experiments/headless_experiments.py` & `seldonian_experiments-0.2.1/experiments/headless_experiments.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,15 @@
             device=pretraining_device)
         
         dataset_for_experiment = SupervisedDataSet(
             features=latent_features,
             labels=labels,
             sensitive_attrs=sensitive_attrs,
             num_datapoints=n_points,
-            meta_information=resampled_dataset.meta_information,
+            meta=resampled_dataset.meta,
         )
 
         # Make a new spec object
         # and update the dataset
 
         spec_for_experiment = copy.deepcopy(spec)
         spec_for_experiment.dataset = dataset_for_experiment
@@ -394,15 +394,15 @@
                 # for this trial. a.k.a the latent features
                 X_test = constraint_eval_kwargs["X_test"]
                 dataset_for_eval = SupervisedDataSet(
                     features=X_test,
                     labels=orig_dataset.labels,
                     sensitive_attrs=orig_dataset.sensitive_attrs,
                     num_datapoints=orig_dataset.num_datapoints,
-                    meta_information=orig_dataset.meta_information)
+                    meta=orig_dataset.meta)
                 constraint_eval_kwargs["dataset"] = dataset_for_eval
 
             for parse_tree in spec_for_experiment.parse_trees:
                 parse_tree.reset_base_node_dict(reset_data=True)
                 parse_tree.evaluate_constraint(**constraint_eval_kwargs)
 
                 g = parse_tree.root.value
```

### Comparing `seldonian_experiments-0.2.0/experiments/headless_utils.py` & `seldonian_experiments-0.2.1/experiments/headless_utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.0/experiments/perf_eval_funcs.py` & `seldonian_experiments-0.2.1/experiments/perf_eval_funcs.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.0/seldonian_experiments.egg-info/PKG-INFO` & `seldonian_experiments-0.2.1/seldonian_experiments.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seldonian-experiments
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library for running experiments with Seldonian algorithms
 Home-page: 
 Author: Austin Hoag
 Author-email: austinthomashoag@gmail.com
 Project-URL: Bug Tracker, https://github.com/seldonian-framework/Experiments/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `seldonian_experiments-0.2.0/seldonian_experiments.egg-info/SOURCES.txt` & `seldonian_experiments-0.2.1/seldonian_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.0/setup.py` & `seldonian_experiments-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seldonian_experiments",
-    version="0.2.0",
+    version="0.2.1",
     author="Austin Hoag",
     author_email="austinthomashoag@gmail.com",
     description="Library for running experiments with Seldonian algorithms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="",
```

### Comparing `seldonian_experiments-0.2.0/tests/conftest.py` & `seldonian_experiments-0.2.1/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,36 +8,33 @@
 from seldonian.RL.Agents.Policies.Softmax import DiscreteSoftmax
 from seldonian.RL.Env_Description.Env_Description import Env_Description
 from seldonian.RL.Env_Description.Spaces import Discrete_Space
 from seldonian.models import objectives
 from seldonian.utils.io_utils import (load_json,
 	load_pickle)
 from seldonian.dataset import (DataSetLoader,RLDataSet,
-	load_supervised_metadata)
+	load_supervised_metadata, RLMetaData)
 from seldonian.parse_tree.parse_tree import (ParseTree,
 	make_parse_trees_from_constraints)
 from seldonian.spec import createSupervisedSpec,createRLSpec
 
 @pytest.fixture
 def gpa_regression_spec():
 	print("Setup gpa_regression_spec")
 	
 	def spec_maker(constraint_strs,deltas):
 
 		data_pth = 'static/datasets/supervised/GPA/gpa_regression_dataset_1000points.csv'
 		metadata_pth = 'static/datasets/supervised/GPA/metadata_regression.json'
 
-		(regime, sub_regime, all_col_names, feature_col_names,
-			label_col_names, sensitive_col_names) = load_supervised_metadata(
-				metadata_pth)
-					
+		meta = load_supervised_metadata(metadata_pth)			
 
 		# Load dataset from file
 		loader = DataSetLoader(
-			regime=regime)
+			regime=meta.regime)
 
 		dataset = loader.load_supervised_dataset(
 			filename=data_pth,
 			metadata_filename=metadata_pth,
 			file_type='csv')
 
 		spec = createSupervisedSpec(
@@ -118,16 +115,18 @@
 def gridworld_spec():
 	print("Setup gridworld_spec")
 	
 	def spec_maker(constraint_strs,deltas):
 
 		episodes_file = 'static/datasets/RL/gridworld/gridworld_100episodes.pkl'
 		episodes = load_pickle(episodes_file)
-		dataset = RLDataSet(episodes=episodes)
-
+		meta = RLMetaData(
+	        all_col_names=["episode_index", "O", "A", "R", "pi_b"]
+	    )
+		dataset = RLDataSet(episodes=episodes,meta=meta)
 		# Initialize policy
 		num_states = 9
 		observation_space = Discrete_Space(0, num_states-1)
 		action_space = Discrete_Space(0, 3)
 		env_description =  Env_Description(observation_space, action_space)
 		policy = DiscreteSoftmax(hyperparam_and_setting_dict={},
 			env_description=env_description)
```

### Comparing `seldonian_experiments-0.2.0/tests/test_examples.py` & `seldonian_experiments-0.2.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.0/tests/test_experiments.py` & `seldonian_experiments-0.2.1/tests/test_experiments.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.2.0/tests/test_generate_plots.py` & `seldonian_experiments-0.2.1/tests/test_generate_plots.py`

 * *Files identical despite different names*

