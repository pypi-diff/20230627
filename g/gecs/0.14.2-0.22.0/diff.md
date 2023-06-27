# Comparing `tmp/gecs-0.14.2.tar.gz` & `tmp/gecs-0.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gecs-0.14.2.tar", max compression
+gzip compressed data, was "gecs-0.22.0.tar", max compression
```

## Comparing `gecs-0.14.2.tar` & `gecs-0.22.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1060 2023-04-06 09:38:20.465352 gecs-0.14.2/LICENSE
--rw-r--r--   0        0        0        0 2023-04-06 08:53:47.610205 gecs-0.14.2/README.md
--rw-r--r--   0        0        0      697 2023-06-19 09:20:16.050681 gecs-0.14.2/pyproject.toml
--rw-r--r--   0        0        0    43737 2023-06-19 09:19:34.711173 gecs-0.14.2/src/gecs/gec.py
--rw-r--r--   0        0        0     2112 2023-06-18 16:26:28.103885 gecs-0.14.2/src/gecs/utils/gaussian_process_visualisation.py
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 gecs-0.14.2/setup.py
--rw-r--r--   0        0        0      964 1970-01-01 00:00:00.000000 gecs-0.14.2/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-06 09:38:20.465352 gecs-0.22.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-06 08:53:47.610205 gecs-0.22.0/README.md
+-rw-r--r--   0        0        0      697 2023-06-26 18:40:00.063336 gecs-0.22.0/pyproject.toml
+-rw-r--r--   0        0        0    42972 2023-06-27 16:27:27.188690 gecs-0.22.0/src/gecs/gec.py
+-rw-r--r--   0        0        0     2112 2023-06-19 14:54:28.150721 gecs-0.22.0/src/gecs/utils/gaussian_process_visualisation.py
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 gecs-0.22.0/setup.py
+-rw-r--r--   0        0        0      964 1970-01-01 00:00:00.000000 gecs-0.22.0/PKG-INFO
```

### Comparing `gecs-0.14.2/LICENSE` & `gecs-0.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gecs-0.14.2/pyproject.toml` & `gecs-0.22.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gecs"
-version = "0.14.2"
+version = "0.22.0"
 authors = ["Leon Luithlen <leontimnaluithlen@gmail.com>"]
 description = "LightGBM Classifier with integrated bayesian hyperparameter optimization"
 keywords = ["lightgbm", "classification", "machine learning", "hyperparameter optimization", "classifier"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/0xideas/sequifier"
 repository = "https://github.com/0xideas/sequifier"
```

### Comparing `gecs-0.14.2/src/gecs/gec.py` & `gecs-0.22.0/src/gecs/gec.py`

 * *Files 3% similar despite different names*

```diff
@@ -198,45 +198,63 @@
         self._class_map = None
         self._n_features = None
         self._n_features_in = None
         self._classes = None
         self._n_classes = None
         self.set_params(**kwargs)
 
+        self._init_kwargs = {
+            k: v for k, v in kwargs.items()
+            if k not in ["bagging_freq", "bagging_fraction"]
+        }
+
+        non_optimized_init_args = [
+            "max_depth",
+            "subsample_for_bin",
+            "objective",
+            "class_weight",
+            "min_split_gain", 
+            "subsample",
+            "subsample_freq",
+            "random_state",
+            "n_jobs",
+            "silent",
+            "importance_type"
+        ]
+        self._init_args = {
+            arg: getattr(self, arg) for arg in non_optimized_init_args
+        }
+
         self.gec_hyperparameters = {
             "l": 1.0,
             "l_bagging": 0.1,
             "hyperparams_acquisition_percentile": 0.7,
             "bagging_acquisition_percentile": 0.7,
             "bandit_greediness": 1.0,
             "n_random_exploration": 10,
             "n_sample": 1000,
             "n_sample_initial": 10000,
             "best_share": 0.2,
             "hyperparameters": [
                 "learning_rate",
                 "n_estimators",
                 "num_leaves",
-                "max_bin",
-                "lambda_l1",
-                "lambda_l2",
-                "min_data_in_leaf",
-                "feature_fraction",
+                "reg_alpha",
+                "reg_lambda",
+                "min_child_samples",
+                "min_child_weight",
+                "colsample_bytree", #feature_fraction
             ],
-            "randomize": True,
-            "estimators_leaves": {
-                "n_exploitation": 5,
-                "share_exploitation": 0.1,
-                "exploration_max_n_estimators": 100,
-                "exploration_max_num_leaves": 100
-            }
+            "randomize": True
         }
-        self._set_hyperparameter_attributes()
+        self._set_gec_attributes()
+        self._set_gec_fields()
+
 
-    def _set_hyperparameter_attributes(self):
+    def _set_gec_attributes(self):
         self.categorical_hyperparameters = [
             ("boosting", ["gbdt", "dart", "rf"]),
             ("bagging", ["yes_bagging", "no_bagging"]),
         ]
 
         self._categorical_hyperparameter_names, _ = zip(
             *self.categorical_hyperparameters
@@ -257,23 +275,32 @@
                 np.arange(100, 200, 20),
                 np.arange(200, 500, 50),
                 np.arange(500, 100, 100),
                 np.arange(1000, 10001, 1000),
             ]
         )
         self._real_hyperparameters_all = [
-            ("learning_rate", (np.logspace(0.001, 2.5, 100)) / 1000),
+            ("learning_rate", (np.concatenate([np.arange(0.001, 0.5, 0.003), np.arange(0.5, 0.95, 0.02)])**2)),
             ("num_leaves",  np.array(list(range(1, 100))+list(range(100, 1000, 5)))),
             ("n_estimators", ten_to_ten_thousand),
-            ("max_bin", ten_to_ten_thousand[:-9]),
-            ("lambda_l1", (np.logspace(0.00, 1, 100) - 1) / 9),
-            ("lambda_l2", (np.logspace(0.00, 1, 100) - 1) / 9),
-            ("min_data_in_leaf", np.arange(2, 50, 1)),
-            ("feature_fraction",np.arange(0.1, 1.01, 0.01))
+            ("reg_alpha", (np.concatenate([np.arange(0.0, 0.5, 0.01), np.arange(0.5, 1.00, 0.02)])**2)),
+            ("reg_lambda", (np.concatenate([np.arange(0.0, 0.5, 0.01), np.arange(0.5, 1.00, 0.02)])**2)),
+            ("min_child_weight", list( np.concatenate([np.arange(0.0, 0.1, 0.001), np.arange(0.1, 0.5, 0.05)])**2)),
+            ("min_child_samples", np.arange(2, 50, 1)),
+            ("colsample_bytree",np.arange(0.1, 1.00, 0.01))
         ]
+
+        self.fixed_params = {
+            hyperparameter: getattr(self, hyperparameter)
+            for hyperparameter, _ in self._real_hyperparameters_all
+            if hyperparameter not in self.gec_hyperparameters["hyperparameters"]
+        }
+
+
+
         self._real_hyperparameters = [
             (hp_name, range_)
             for hp_name, range_ in self._real_hyperparameters_all
             if hp_name in self.gec_hyperparameters["hyperparameters"]
         ]
         self._real_hyperparameters_linear = [
             (name, np.arange(-1, 1, 2 / len(values)).astype(np.float16))
@@ -301,33 +328,39 @@
             *self._real_hyperparameters_linear
         )
 
         self._real_hypermarameter_types = [
             np.array(s).dtype for _, s in self._real_hyperparameters
         ]
 
+    def _set_gec_fields(self):
         self.kernel = RBF(self.gec_hyperparameters["l"])
         self.hyperparameter_scores = {
             c: {"inputs": [], "output": [], "means": [], "sigmas": []}
             for c in ["all-models"]
         }
         self.kernel_bagging = RBF(self.gec_hyperparameters["l_bagging"])
+
         self.bagging_scores = {
             c: {"inputs": [], "output": [], "means": [], "sigmas": []}
             for c in ["all-models"]
         }
         self._bagging_combinations = list(
             itertools.product(
                 *[
                     list(range(1, 11, 1)),
                     np.arange(0.5, 1.0, 0.01),
                 ]
             )
         )
 
+        self._rescale_bagging_combination = lambda freq, frac: (((freq/5)-1), ((frac*4)-3))
+        self._invert_rescaled_bagging_combination =  lambda freq, frac: (((freq+1)*5), ((frac+3)/4))
+        self._bagging_combinations_rescaled = [self._rescale_bagging_combination(freq, frac) for freq, frac in self._bagging_combinations]
+
         self.best_score = None
         self.best_params_ = None
         self.n_iterations = 0
 
         # parameters for bandit
         self.rewards = {
             c: {"a": 1, "b": 1} for c in self._categorical_hyperparameter_combinations
@@ -465,15 +498,15 @@
             "selected_arms": self.selected_arms,
             "hyperparameter_scores": hyperparameter_scores,
             "bagging_scores": bagging_scores,
             "best_params_": self.best_params_,
             "best_score": self.best_score,
             "best_params_gec": self.best_params_gec,
             "best_scores_gec": self.best_scores_gec,
-            "gec_iter": self.gec_iter,
+            "gec_iter": self.gec_iter
         }
         return representation
 
 
     def _validate_parameter_maps(self):
         real_to_linear_to_real = [
             self._real_hyperparameters_map[hp][self._real_hyperparameters_map_reverse[hp][v]] == v
@@ -497,17 +530,18 @@
                 dictionary with values for "l", "l_bagging",
                 "acquisition_percentile" and "bandit_greediness"
         """
         assert np.all(
             np.array([hp in self.gec_hyperparameters for hp in gec_hyperparameters.keys()])
         )
         self.gec_hyperparameters.update(gec_hyperparameters)
-        self._set_hyperparameter_attributes()
+        self._set_gec_attributes()
+
 
-    def fit(self, X, y, n_iter=100, n_estimators=100, num_leaves=32):
+    def fit(self, X, y, n_iter=100, fixed_hyperparameters=["n_estimators", "num_leaves"]):
         """Fit GEC on data
 
         Parameters
         ----------
             X : np.ndarray
                 Input feature matrix
             y : np.ndarray
@@ -516,21 +550,16 @@
                 number of bayesian optimisation iterations
 
         Returns
         -------
             self: GEC
         """
 
-        assert n_estimators <= 10000, "only up to 10000 estimators are allowed"
-        assert num_leaves <=1000, "only up to 1000 leaves are allowed"
-    
-        self.gec_num_leaves = num_leaves
-        self.gec_n_estimators = n_estimators
-
-        self.adjustment_factor = 1 / len(np.unique(y))  # get mean closer to 0
+        filtered_hyperparameters = list(set(self.gec_hyperparameters["hyperparameters"]).difference(set(fixed_hyperparameters)))
+        self.set_gec_hyperparameters({"hyperparameters": filtered_hyperparameters })
 
         self.best_scores_gec = {}
         self.best_params_gec = {}
         (
             self.best_params_gec["search"],
             self.best_scores_gec["search"],
         ) = self._optimise_hyperparameters(
@@ -567,30 +596,14 @@
     def _calculate_cv_score(self, X, y, params):
         clf = LGBMClassifier(**params)
         with open(os.devnull, "w") as f, contextlib.redirect_stdout(f):
             score = np.mean(cross_val_score(clf, X, y, cv=5))
         return score
 
 
-    def _set_n_estimators_and_num_leaves(self, arguments, i, n_iter):
-        last_n_iterations = (i+self.gec_hyperparameters["estimators_leaves"]["n_exploitation"]) >= n_iter
-        last_share_iterations = (i/n_iter) >= (1- self.gec_hyperparameters["estimators_leaves"]["share_exploitation"])
-        n_estimators_not_optimised = "n_estimators" not in self.gec_hyperparameters["hyperparameters"]
-        if last_n_iterations or last_share_iterations or n_estimators_not_optimised:
-            arguments["n_estimators"] = self.gec_n_estimators
-        else:
-            arguments["n_estimators"] = min(arguments["n_estimators"], self.gec_hyperparameters["estimators_leaves"]["exploration_max_n_estimators"])
-            
-        num_leaves_not_optimised = "num_leaves" not in self.gec_hyperparameters["hyperparameters"]
-        if last_n_iterations or last_share_iterations or num_leaves_not_optimised:
-            arguments["num_leaves"] = self.gec_num_leaves
-        else:
-            arguments["num_leaves"] = min(arguments["num_leaves"], self.gec_hyperparameters["estimators_leaves"]["exploration_max_num_leaves"])
-        return(arguments)
-
     def _optimise_hyperparameters(
         self,
         n_iter,
         X,
         Y,
         best_score,
         best_params,
@@ -690,26 +703,22 @@
                         for m, s in zip(mean, sigma)
                     ]
                 )
 
                 best_predicted_combination = combinations[np.argmax(predicted_rewards)]
                 selected_combination = best_predicted_combination
                 arguments = self._build_arguments(
-                    selected_arm.split("-"), best_predicted_combination
+                    selected_arm.split("-"), selected_combination
                 )
 
                 if "yes_bagging" in selected_arm:
                     if len(self.bagging_scores["all-models"]["inputs"]) > 0:
-                        self.gaussian_bagging.fit(
-                            np.array(self.bagging_scores["all-models"]["inputs"]),
-                            np.array(self.bagging_scores["all-models"]["output"])
-                            - self.adjustment_factor,
-                        )
+                        self._fit_gaussian_bagging()
                     mean_bagging, sigma_bagging = self.gaussian_bagging.predict(
-                        self._bagging_combinations, return_std=True
+                        self._bagging_combinations_rescaled, return_std=True
                     )
 
                     predicted_rewards_bagging = np.array(
                         [
                             scipy.stats.norm.ppf(
                                 self.gec_hyperparameters[
                                     "bagging_acquisition_percentile"
@@ -728,16 +737,14 @@
                         arguments["bagging_freq"],
                         arguments["bagging_fraction"],
                     ) = best_predicted_combination_bagging
 
             del arguments["bagging"]
             arguments["verbosity"] = -1
 
-            arguments = self._set_n_estimators_and_num_leaves(arguments, i, n_iter)
-
             try:
                 score = self._calculate_cv_score(X, Y, arguments)
                 if np.isnan(score):
                     score = 0
 
                 if best_score is None or score > best_score:
                     best_score = score
@@ -749,15 +756,15 @@
                 )
                 self.hyperparameter_scores["all-models"]["output"].append(score)
                 self.hyperparameter_scores["all-models"]["means"].append(mean)
                 self.hyperparameter_scores["all-models"]["sigmas"].append(sigma)
 
                 if "bagging_freq" in arguments:
                     self.bagging_scores["all-models"]["inputs"].append(
-                        [float(f) for f in selected_combination_bagging]
+                        list(self._rescale_bagging_combination(*selected_combination_bagging))
                     )
                     self.bagging_scores["all-models"]["output"].append(score)
                     self.bagging_scores["all-models"]["means"].append(mean_bagging)
                     self.bagging_scores["all-models"]["sigmas"].append(sigma_bagging)
 
                 if self.best_score is not None:
                     score_delta = score - self.best_score
@@ -776,17 +783,14 @@
                 else:
                     self.best_score = score
                     self.best_params_ = arguments
 
             except Exception as e:
                 warnings.warn(f"These arguments led to an Error: {arguments}: {e}")
 
-
-        best_params["n_estimators"] = self.gec_n_estimators
-        best_params["num_leaves"] = self.gec_num_leaves
         best_score = self._calculate_cv_score(X, Y, best_params)
 
         return (best_params, best_score)
 
     def _build_arguments(self, categorical_combination, real_combination_linear):
         best_predicted_combination_converted = [
             self._real_hyperparameters_map[name][value]
@@ -807,30 +811,36 @@
         arguments = dict(
             zip(
                 self._categorical_hyperparameter_names
                 + self._real_hyperparameter_names,
                 hyperparameter_values,
             )
         )
-        return arguments
+        return {**arguments, **self.fixed_params,  **self._init_args, **self._init_kwargs}
 
     def _fit_best_params(self, X, y):
 
         gec = GEC(**{**self.best_params_, "random_state": 101})
 
         for k, v in gec.__dict__.items():
             if k not in self.__dict__ or self.__dict__[k] is None:
                 self.__dict__[k] = v
 
         super().fit(X, y)
 
     def _fit_gaussian(self):
         self.gaussian.fit(
             np.array(self.hyperparameter_scores["all-models"]["inputs"]),
-            np.array(self.hyperparameter_scores["all-models"]["output"]) - self.adjustment_factor,
+            np.array(self.hyperparameter_scores["all-models"]["output"]) - np.mean(self.hyperparameter_scores["all-models"]["output"]),
+        )
+
+    def _fit_gaussian_bagging(self):
+        self.gaussian_bagging.fit(
+            np.array(self.bagging_scores["all-models"]["inputs"]),
+            np.array(self.bagging_scores["all-models"]["output"]) - np.mean(self.bagging_scores["all-models"]["output"]),
         )
 
     def _get_best_arm(self):
         mean_reward = np.array(
             [
                 reward["a"]/ ( reward["a"] + reward["b"])
                 for _, reward in self.rewards.items()
@@ -853,17 +863,14 @@
 
         best_combination, _ = self._find_best_parameters_iter(initial_combinations)
 
         best_params = self._find_best_parameters_from_initial_parameters(
             best_arm, best_combination, step_sizes
         )
 
-        best_params["n_estimators"] = self.gec_n_estimators
-        best_params["num_leaves"] = self.gec_num_leaves
-
         return best_params
 
     def _find_best_parameters_from_search(self, params):
         self._fit_gaussian()
 
         if "bagging_freq" in params:
             del params["bagging_freq"]
@@ -879,17 +886,14 @@
             for name in self._real_hyperparameter_names
         ]
         best_params = self._find_best_parameters_from_initial_parameters(
             best_arm,
             best_params_linear_values,
             step_sizes=[4, 2, 1],
         )
-
-        best_params["n_estimators"] = self.gec_n_estimators
-        best_params["num_leaves"] = self.gec_num_leaves
         
         return best_params
 
     def _find_best_parameters_iter(self, combinations):
 
         mean = self.gaussian.predict(combinations)
         best_score = np.max(mean)
@@ -921,24 +925,16 @@
 
 
         arguments = self._build_arguments(
             best_arm.split("-"), best_combination
         )
 
         if "yes_bagging" in best_arm:
-            bagging_scores = np.array(self.bagging_scores["all-models"]["inputs"])
-            bagging_scores[:, 0] = bagging_scores[:, 0] / 10
-            self.gaussian_bagging.fit(
-                bagging_scores,
-                np.array(self.bagging_scores["all-models"]["output"])
-                - self.adjustment_factor,
-            )
-            bagging_combinations = np.array(self._bagging_combinations)
-            bagging_combinations[:, 0] = bagging_combinations[:, 0] / 10
-            mean_bagging = self.gaussian_bagging.predict(bagging_combinations)
+            self._fit_gaussian_bagging()
+            mean_bagging = self.gaussian_bagging.predict(self._bagging_combinations_rescaled)
             best_predicted_combination_bagging = self._bagging_combinations[
                 np.argmax(mean_bagging)
             ]
 
             (
                 arguments["bagging_freq"],
                 arguments["bagging_fraction"],
@@ -1058,29 +1054,30 @@
             correlation,
             label="corr(preds mean, preds variance)",
         )
         ax.legend(loc="lower right")
 
     def _plot_linear_scaled_parameter_samples(self, cat, ax, x):
         inputs_ = np.array(self.hyperparameter_scores[cat]["inputs"])
-        assert (len(self._real_hyperparameter_names) == inputs_.shape[1])
+        assert (
+            (len(self._real_hyperparameter_names) == inputs_.shape[1]), 
+            f"{len(self._real_hyperparameter_names)}!={inputs_.shape[1]}"
+        )
         for i in range(inputs_.shape[1]):
             ax.plot(x, inputs_[:, i], label=self._real_hyperparameter_names[i])
 
     def _plot_boosting_parameter_surface(
         self,
         cat,
         plot_bounds=True,
     ):
-        bagging_scores = np.array(self.bagging_scores[cat]["inputs"])
-        bagging_scores[:, 0] = bagging_scores[:, 0] / 10
-        self.gaussian_bagging.fit(bagging_scores, self.bagging_scores[cat]["output"])
+        self._fit_gaussian_bagging()
 
-        X_range = np.arange(1, 11, 1) / 10
-        Y_range = np.arange(0.05, 1.0, 0.05)
+        X_range = np.array(self._bagging_combinations_rescaled)[0,:]
+        Y_range = np.array(self._bagging_combinations_rescaled)[1,:]
         Z_range = np.arange(-0.5, 1.5, 0.1)
 
         fig, ax = plt.subplots(subplot_kw={"projection": "3d"}, figsize=(12, 12))
 
         # Make data.
         X = np.arange(
             np.min(X_range), np.max(X_range), (np.max(X_range) - np.min(X_range)) / 100
```

### Comparing `gecs-0.14.2/src/gecs/utils/gaussian_process_visualisation.py` & `gecs-0.22.0/src/gecs/utils/gaussian_process_visualisation.py`

 * *Files identical despite different names*

### Comparing `gecs-0.14.2/setup.py` & `gecs-0.22.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'scikit-learn==1.2.2',
  'scipy==1.10.1',
  'tqdm==4.65.0',
  'typer==0.9.0']
 
 setup_kwargs = {
     'name': 'gecs',
-    'version': '0.14.2',
+    'version': '0.22.0',
     'description': 'LightGBM Classifier with integrated bayesian hyperparameter optimization',
     'long_description': '',
     'author': 'Leon Luithlen',
     'author_email': 'leontimnaluithlen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/0xideas/sequifier',
```

### Comparing `gecs-0.14.2/PKG-INFO` & `gecs-0.22.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gecs
-Version: 0.14.2
+Version: 0.22.0
 Summary: LightGBM Classifier with integrated bayesian hyperparameter optimization
 Home-page: https://github.com/0xideas/sequifier
 License: MIT
 Keywords: lightgbm,classification,machine learning,hyperparameter optimization,classifier
 Author: Leon Luithlen
 Author-email: leontimnaluithlen@gmail.com
 Requires-Python: >=3.10.0,<3.11.0
```

