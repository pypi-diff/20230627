# Comparing `tmp/hgboost-1.1.3.tar.gz` & `tmp/hgboost-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgboost-1.1.3.tar", last modified: Wed Oct  5 08:01:15 2022, max compression
+gzip compressed data, was "hgboost-1.1.4.tar", last modified: Tue Jun 27 20:16:32 2023, max compression
```

## Comparing `hgboost-1.1.3.tar` & `hgboost-1.1.4.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-10-05 08:01:15.325763 hgboost-1.1.3/
--rw-rw-rw-   0        0        0     1120 2021-01-17 22:40:22.000000 hgboost-1.1.3/LICENSE
--rw-rw-rw-   0        0        0       54 2021-01-17 22:40:22.000000 hgboost-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0    10263 2022-10-05 08:01:15.325763 hgboost-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     9640 2022-09-18 18:46:34.000000 hgboost-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2022-10-05 08:01:15.311369 hgboost-1.1.3/hgboost/
--rw-rw-rw-   0        0        0     3565 2022-10-05 07:52:43.000000 hgboost-1.1.3/hgboost/__init__.py
--rw-rw-rw-   0        0        0    10418 2022-10-05 07:44:50.000000 hgboost-1.1.3/hgboost/examples.py
--rw-rw-rw-   0        0        0    90149 2022-10-05 07:51:10.000000 hgboost-1.1.3/hgboost/hgboost.py
--rw-rw-rw-   0        0        0     4008 2019-11-07 18:23:02.000000 hgboost-1.1.3/hgboost/shapplot.py
-drwxrwxrwx   0        0        0        0 2022-10-05 08:01:15.324301 hgboost-1.1.3/hgboost/utils/
--rw-rw-rw-   0        0        0        0 2021-01-17 22:40:22.000000 hgboost-1.1.3/hgboost/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-05 08:01:15.324301 hgboost-1.1.3/hgboost.egg-info/
--rw-rw-rw-   0        0        0    10263 2022-10-05 08:01:15.000000 hgboost-1.1.3/hgboost.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2022-10-05 08:01:15.000000 hgboost-1.1.3/hgboost.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-05 08:01:15.000000 hgboost-1.1.3/hgboost.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2022-10-05 08:01:15.000000 hgboost-1.1.3/hgboost.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-10-05 08:01:15.000000 hgboost-1.1.3/hgboost.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-05 08:01:15.325763 hgboost-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1579 2022-03-11 12:59:18.000000 hgboost-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 20:16:32.890830 hgboost-1.1.4/
+-rw-rw-rw-   0        0        0     1120 2021-01-17 22:40:22.000000 hgboost-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0       54 2021-01-17 22:40:22.000000 hgboost-1.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    10263 2023-06-27 20:16:32.888840 hgboost-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9640 2022-09-18 18:46:34.000000 hgboost-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 20:16:32.803068 hgboost-1.1.4/hgboost/
+-rw-rw-rw-   0        0        0     3583 2023-06-27 18:04:10.000000 hgboost-1.1.4/hgboost/__init__.py
+-rw-rw-rw-   0        0        0    10803 2023-06-27 18:04:48.000000 hgboost-1.1.4/hgboost/examples.py
+-rw-rw-rw-   0        0        0    92757 2023-06-27 17:42:46.000000 hgboost-1.1.4/hgboost/hgboost.py
+-rw-rw-rw-   0        0        0     4008 2019-11-07 18:23:02.000000 hgboost-1.1.4/hgboost/shapplot.py
+drwxrwxrwx   0        0        0        0 2023-06-27 20:16:32.869855 hgboost-1.1.4/hgboost/utils/
+-rw-rw-rw-   0        0        0        0 2021-01-17 22:40:22.000000 hgboost-1.1.4/hgboost/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 20:16:32.863043 hgboost-1.1.4/hgboost.egg-info/
+-rw-rw-rw-   0        0        0    10263 2023-06-27 20:16:32.000000 hgboost-1.1.4/hgboost.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-06-27 20:16:32.000000 hgboost-1.1.4/hgboost.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 20:16:32.000000 hgboost-1.1.4/hgboost.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2023-06-27 20:16:32.000000 hgboost-1.1.4/hgboost.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-27 20:16:32.000000 hgboost-1.1.4/hgboost.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 20:16:32.891296 hgboost-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1584 2023-06-27 17:40:46.000000 hgboost-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 20:16:32.885807 hgboost-1.1.4/tests/
+-rw-rw-rw-   0        0        0    12561 2022-10-05 07:59:00.000000 hgboost-1.1.4/tests/test_hgboost.py
```

### Comparing `hgboost-1.1.3/LICENSE` & `hgboost-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hgboost-1.1.3/PKG-INFO` & `hgboost-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hgboost
-Version: 1.1.3
+Version: 1.1.4
 Summary: hgboost is a python package for hyperparameter optimization for xgboost, catboost and lightboost for both classification and regression tasks.
 Home-page: https://erdogant.github.io/hgboost
-Download-URL: https://github.com/erdogant/hgboost/archive/1.1.3.tar.gz
+Download-URL: https://github.com/erdogant/hgboost/archive/1.1.4.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `hgboost-1.1.3/README.md` & `hgboost-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `hgboost-1.1.3/hgboost/__init__.py` & `hgboost-1.1.4/hgboost/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
+from datazets import get as import_example
 from hgboost.hgboost import hgboost
 
 from hgboost.hgboost import (
     import_example,
     )
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.1.3'
+__version__ = '1.1.4'
 
 # module level doc-string
 __doc__ = """
 hgboost - Hyperoptimized Gradient Boosting
 =====================================================================
 
-Description
------------
 HGBoost stands for Hyperoptimized Gradient Boosting and is a Python package for hyperparameter optimization
 for XGBoost, LightBoost, and CatBoost. It will carefully split the dataset into a train, test, and independent
 validation set. Within the train-test set, there is the inner loop for optimizing the hyperparameters using
 Bayesian optimization (with hyperopt) and, the outer loop to score how well the top performing models can
 generalize based on k-fold cross validation. As such, it will make the best attempt to select the most robust
 model with the best performance.
 The hgboost approach contains the following parts:
```

### Comparing `hgboost-1.1.3/hgboost/examples.py` & `hgboost-1.1.4/hgboost/examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,38 @@
 
 # %%
 # import numpy as np
 # from hgboost import hgboost
 # print(dir(hgboost))
 # print(hgboost.__version__)
 
+# %%
+from hgboost import hgboost
+hgb = hgboost()
+df = hgb.import_example(data='ds_salaries')
+
+y = df['salary_in_usd'].values
+df.drop(['salary_in_usd', 'salary_currency', 'salary'], axis=1, inplace=True)
+X = hgb.preprocessing(df, verbose=4)
+
+import numpy as np
+I = ~np.isnan(y)
+X = X.loc[I, :]
+y = y[I]
+
+results  = hgb.xgboost_reg(X, y, eval_metric='mae')      # XGBoost
+
+
 # %% HYPEROPTIMIZED REGRESSION-XGBOOST
 import numpy as np
 from hgboost import hgboost
 
 hgb_xgb = hgboost(max_eval=25, cv=5, test_size=0.2, val_size=0.2, top_cv_evals=10, random_state=42, verbose=3)
-# hgb_cat = hgboost(max_eval=250, cv=5, test_size=0.2, val_size=0.2, top_cv_evals=10, random_state=42, verbose=3)
-# hgb_light = hgboost(max_eval=250, cv=5, test_size=0.2, val_size=0.2, top_cv_evals=10, random_state=42, verbose=3)
+hgb_cat = hgboost(max_eval=250, cv=5, test_size=0.2, val_size=0.2, top_cv_evals=10, random_state=42, verbose=3)
+hgb_light = hgboost(max_eval=250, cv=5, test_size=0.2, val_size=0.2, top_cv_evals=10, random_state=42, verbose=3)
 
 # Import data
 df = hgb_xgb.import_example()
 y = df['Age'].values
 df.drop(['Age', 'PassengerId', 'Name'], axis=1, inplace=True)
 
 # Preprocessing
```

### Comparing `hgboost-1.1.3/hgboost/hgboost.py` & `hgboost-1.1.4/hgboost/hgboost.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 warnings.filterwarnings("ignore")
 
 import classeval as cle
 from df2onehot import df2onehot
 import treeplot as tree
 import colourmap
 import pypickle
+import datazets as dz
 
 import os
 import numpy as np
 import pandas as pd
 import wget
 
 from sklearn.metrics import mean_squared_error, cohen_kappa_score, mean_absolute_error, log_loss, roc_auc_score, f1_score
@@ -795,15 +796,15 @@
             for param in model_params:
                 try:
                     if 'ctb' in self.method:
                         df_params[param].iloc[i] = trial['result']['model'].get_all_params().get(param)
                     else:
                         df_params[param].iloc[i] = getattr(trial['result']['model'], param)
                 except:
-                    if self.verbose>=3: print('[hgboost]> Skip [%s]' %(param))
+                    if self.verbose>=4: print('[hgboost]> Skip [%s]' %(param))
                     gather_params_legacy = True
 
         # The trials.vals stores the index for some parameters instead of the real values.
         if gather_params_legacy:
             df_params = pd.DataFrame(trials.vals)
         df_scoring = pd.DataFrame(trials.results)
         df = pd.concat([df_params, df_scoring], axis=1)
@@ -978,38 +979,39 @@
             Processed data.
 
         """
         if verbose is None: verbose = self.verbose
         X = df2onehot(df, y_min=y_min, hot_only=hot_only, perc_min_num=perc_min_num, excl_background=excl_background, verbose=verbose)
         return X['onehot']
 
-    def import_example(self, data='titanic', url=None, sep=',', verbose=3):
+    def import_example(self, data='titanic', url=None, sep=','):
         """Import example dataset from github source.
 
         Description
         -----------
         Import one of the few datasets from github source or specify your own download url link.
 
         Parameters
         ----------
         data : str
             Name of datasets: 'sprinkler', 'titanic', 'student', 'fifa', 'cancer', 'waterpump', 'retail'
         url : str
             url link to to dataset.
-        verbose : int, (default : 3)
-            Print progress to screen.
-            0: None, 1: ERROR, 2: WARN, 3: INFO, 4: DEBUG, 5: TRACE
 
         Returns
         -------
         pd.DataFrame()
             Dataset containing mixed features.
 
+        References
+        ----------
+            * https://github.com/erdogant/datazets
+
         """
-        return import_example(data=data, url=url, sep=sep, verbose=verbose)
+        return dz.get(data=data, url=url, sep=sep)
 
     def treeplot(self, num_trees=None, plottype='horizontal', figsize=(20, 25), return_ax=False, verbose=3):
         """Tree plot.
 
         Parameters
         ----------
         num_trees : int, default None
@@ -1446,14 +1448,34 @@
         filepath : str, (default: 'hgboost_model.pkl')
             Pathname to store pickle files.
         overwrite : bool, (default=False)
             Overwite file if exists.
         verbose : int, optional
             Show message. A higher number gives more informatie. The default is 3.
 
+        Examples
+        --------
+        >>> # Initialize libraries
+        >>> from hgboost import hgboost
+        >>> import pandas as pd
+        >>> from sklearn import datasets
+        >>>
+        >>> # Load example dataset
+        >>> iris = datasets.load_iris()
+        >>> X = pd.DataFrame(iris.data, columns=iris['feature_names'])
+        >>> y = iris.target
+        >>>
+        >>> # Train model using user-defined parameters
+        >>> hgb = hgboost(max_eval=10, threshold=0.5, cv=5, test_size=0.2, val_size=0.2, top_cv_evals=10, random_state=42)
+        >>> results = hgb.xgboost(X, y, method="xgb_clf_multi")
+        >>>
+        >>> # Save
+        >>> hgb.save(filepath='hgboost_model.pkl', overwrite=True)
+        >>>
+
         Returns
         -------
         bool : [True, False]
             Status whether the file is saved.
 
         """
         if (filepath is None) or (filepath==''):
@@ -1477,31 +1499,71 @@
         storedata['cv'] = self.cv
         storedata['random_state'] = self.random_state
         storedata['n_jobs'] = self.n_jobs
         storedata['verbose'] = self.verbose
         storedata['is_unbalance'] = self.is_unbalance
         # Save
         status = pypickle.save(filepath, storedata, overwrite=overwrite, verbose=verbose)
-        if verbose>=3: print('[hgboost] >Saving.. %s' %(status))
+        if status:
+            if verbose>=3: print('[hgboost] >Save model results.')
+            if verbose>=3: print('[hgboost] >Save user-defined parameters.')
+            if verbose>=3: print('[hgboost] >Save trained model.')
+            if verbose>=3: print('[hgboost] >Save succesful!')
+        else:
+            if verbose>=3: print('[hgboost] >Could not save. Tip: "hgb.save(overwrite=True)"')
         # return
         return status
 
     def load(self, filepath='hgboost_model.pkl', verbose=3):
         """Load learned model.
 
+        Description
+        -----------
+        The load function will restore the trained model and results.
+        In a fresh (new) start, you need to re-initialize the hgboost model first.
+        By loading the model, the user defined parameters are also restored.
+
         Parameters
         ----------
         filepath : str
             Pathname to stored pickle files.
         verbose : int, optional
             Show message. A higher number gives more information. The default is 3.
 
+        Examples
+        --------
+        >>> # Initialize libraries
+        >>> from hgboost import hgboost
+        >>> import pandas as pd
+        >>> from sklearn import datasets
+        >>>
+        >>> # Load example dataset
+        >>> iris = datasets.load_iris()
+        >>> X = pd.DataFrame(iris.data, columns=iris['feature_names'])
+        >>> y = iris.target
+        >>>
+        >>> # Train model using user-defined parameters
+        >>> hgb = hgboost(max_eval=10, threshold=0.5, cv=5, test_size=0.2, val_size=0.2, top_cv_evals=10, random_state=42)
+        >>> results = hgb.xgboost(X, y, method="xgb_clf_multi")
+        >>>
+        >>> # Save
+        >>> hgb.save(filepath='hgboost_model.pkl', overwrite=True)
+        >>>
+        >>> # Load
+        >>> from hgboost import hgboost
+        >>> hgb = hgboost()
+        >>> results = hgb.load(filepath='hgboost_model.pkl')
+        >>>
+        >>> # Make predictions again with:
+        >>> y_pred, y_proba = hgb.predict(X)
+
         Returns
         -------
-        Object.
+        * dictionary containing model results.
+        * Object with trained model.
 
         """
         if (filepath is None) or (filepath==''):
             filepath = 'hgboost_model.pkl'
         if filepath[-4:]!='.pkl':
             filepath = filepath + '.pkl'
         # Load
@@ -1521,15 +1583,17 @@
             self.test_size = storedata['test_size']
             self.val_size = storedata['val_size']
             self.cv = storedata['cv']
             self.is_unbalance = storedata['is_unbalance']
             self.random_state = storedata['random_state']
             self.n_jobs = storedata['n_jobs']
             self.verbose = storedata['verbose']
-
+            if verbose>=3: print('[hgboost] >Restore model results.')
+            if verbose>=3: print('[hgboost] >Restore user-defined parameters.')
+            if verbose>=3: print('[hgboost] >Restore trained model.')
             if verbose>=3: print('[hgboost] >Loading succesful!')
             # Return results
             return self.results
         else:
             if verbose>=2: print('[hgboost] >WARNING: Could not load data.')
```

### Comparing `hgboost-1.1.3/hgboost/shapplot.py` & `hgboost-1.1.4/hgboost/shapplot.py`

 * *Files identical despite different names*

### Comparing `hgboost-1.1.3/hgboost.egg-info/PKG-INFO` & `hgboost-1.1.4/hgboost.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hgboost
-Version: 1.1.3
+Version: 1.1.4
 Summary: hgboost is a python package for hyperparameter optimization for xgboost, catboost and lightboost for both classification and regression tasks.
 Home-page: https://erdogant.github.io/hgboost
-Download-URL: https://github.com/erdogant/hgboost/archive/1.1.3.tar.gz
+Download-URL: https://github.com/erdogant/hgboost/archive/1.1.4.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `hgboost-1.1.3/setup.py` & `hgboost-1.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 # Setup ------------
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
-     install_requires=['pypickle', 'wget','matplotlib','numpy','pandas','tqdm','hyperopt','lightgbm','catboost','xgboost','classeval','treeplot','df2onehot','colourmap','seaborn'],
+     install_requires=['datazets', 'pypickle', 'matplotlib','numpy','pandas','tqdm','hyperopt','lightgbm','catboost','xgboost','classeval','treeplot','df2onehot','colourmap','seaborn'],
      python_requires='>=3',
      name='hgboost',
      version=new_version,
      author="Erdogan Taskesen",
      author_email="erdogant@gmail.com",
      description="hgboost is a python package for hyperparameter optimization for xgboost, catboost and lightboost for both classification and regression tasks.",
      long_description=long_description,
```

