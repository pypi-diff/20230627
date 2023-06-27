# Comparing `tmp/ColGenEstimator-0.0.9.tar.gz` & `tmp/ColGenEstimator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ColGenEstimator-0.0.9.tar", last modified: Thu Aug 25 19:43:08 2022, max compression
+gzip compressed data, was "dist/ColGenEstimator-0.1.1.tar", last modified: Tue Jun 27 14:26:45 2023, max compression
```

## Comparing `ColGenEstimator-0.0.9.tar` & `ColGenEstimator-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 krunal     (501) staff       (20)        0 2022-08-25 19:43:08.386825 ColGenEstimator-0.0.9/
-drwxr-xr-x   0 krunal     (501) staff       (20)        0 2022-08-25 19:43:08.385372 ColGenEstimator-0.0.9/ColGenEstimator.egg-info/
--rw-r--r--   0 krunal     (501) staff       (20)     2805 2022-08-25 19:43:08.000000 ColGenEstimator-0.0.9/ColGenEstimator.egg-info/PKG-INFO
--rw-r--r--   0 krunal     (501) staff       (20)      617 2022-08-25 19:43:08.000000 ColGenEstimator-0.0.9/ColGenEstimator.egg-info/SOURCES.txt
--rw-r--r--   0 krunal     (501) staff       (20)        1 2022-08-25 19:43:08.000000 ColGenEstimator-0.0.9/ColGenEstimator.egg-info/dependency_links.txt
--rw-r--r--   0 krunal     (501) staff       (20)        1 2022-08-24 18:48:47.000000 ColGenEstimator-0.0.9/ColGenEstimator.egg-info/not-zip-safe
--rw-r--r--   0 krunal     (501) staff       (20)      136 2022-08-25 19:43:08.000000 ColGenEstimator-0.0.9/ColGenEstimator.egg-info/requires.txt
--rw-r--r--   0 krunal     (501) staff       (20)       18 2022-08-25 19:43:08.000000 ColGenEstimator-0.0.9/ColGenEstimator.egg-info/top_level.txt
--rw-r--r--   0 krunal     (501) staff       (20)       25 2021-12-14 15:40:21.000000 ColGenEstimator-0.0.9/MANIFEST.in
--rw-r--r--   0 krunal     (501) staff       (20)     2805 2022-08-25 19:43:08.386952 ColGenEstimator-0.0.9/PKG-INFO
--rw-r--r--   0 krunal     (501) staff       (20)     1539 2022-07-28 13:33:16.000000 ColGenEstimator-0.0.9/README.rst
-drwxr-xr-x   0 krunal     (501) staff       (20)        0 2022-08-25 19:43:08.386075 ColGenEstimator-0.0.9/col_gen_estimator/
--rw-r--r--   0 krunal     (501) staff       (20)     1003 2022-08-24 18:19:38.000000 ColGenEstimator-0.0.9/col_gen_estimator/__init__.py
--rw-r--r--   0 krunal     (501) staff       (20)    33574 2022-07-28 13:33:16.000000 ColGenEstimator-0.0.9/col_gen_estimator/_bdr_classifier.py
--rw-r--r--   0 krunal     (501) staff       (20)     7150 2022-08-18 19:38:00.000000 ColGenEstimator-0.0.9/col_gen_estimator/_col_gen_classifier.py
--rw-r--r--   0 krunal     (501) staff       (20)    23305 2022-08-25 19:41:54.000000 ColGenEstimator-0.0.9/col_gen_estimator/_dtree_classifier.py
--rw-r--r--   0 krunal     (501) staff       (20)       22 2022-08-25 19:42:01.000000 ColGenEstimator-0.0.9/col_gen_estimator/_version.py
-drwxr-xr-x   0 krunal     (501) staff       (20)        0 2022-08-25 19:43:08.386705 ColGenEstimator-0.0.9/col_gen_estimator/tests/
--rw-r--r--   0 krunal     (501) staff       (20)        0 2021-12-14 15:40:21.000000 ColGenEstimator-0.0.9/col_gen_estimator/tests/__init__.py
--rw-r--r--   0 krunal     (501) staff       (20)     7520 2022-07-28 13:33:16.000000 ColGenEstimator-0.0.9/col_gen_estimator/tests/test_bdrc.py
--rw-r--r--   0 krunal     (501) staff       (20)      488 2022-08-25 19:12:12.000000 ColGenEstimator-0.0.9/col_gen_estimator/tests/test_common.py
--rw-r--r--   0 krunal     (501) staff       (20)    10399 2022-08-25 19:07:59.000000 ColGenEstimator-0.0.9/col_gen_estimator/tests/test_dtree.py
--rw-r--r--   0 krunal     (501) staff       (20)       41 2022-07-28 13:33:16.000000 ColGenEstimator-0.0.9/requirements.txt
--rw-r--r--   0 krunal     (501) staff       (20)      148 2022-08-25 19:43:08.387334 ColGenEstimator-0.0.9/setup.cfg
--rw-r--r--   0 krunal     (501) staff       (20)     2051 2022-07-28 13:33:16.000000 ColGenEstimator-0.0.9/setup.py
+drwxr-xr-x   0 krunal     (501) staff       (20)        0 2023-06-27 14:26:45.000000 ColGenEstimator-0.1.1/
+drwxr-xr-x   0 krunal     (501) staff       (20)        0 2023-06-27 14:26:45.000000 ColGenEstimator-0.1.1/ColGenEstimator.egg-info/
+-rw-r--r--   0 krunal     (501) staff       (20)     3198 2023-06-27 14:26:45.000000 ColGenEstimator-0.1.1/ColGenEstimator.egg-info/PKG-INFO
+-rw-r--r--   0 krunal     (501) staff       (20)      667 2023-06-27 14:26:45.000000 ColGenEstimator-0.1.1/ColGenEstimator.egg-info/SOURCES.txt
+-rw-r--r--   0 krunal     (501) staff       (20)        1 2023-06-27 14:26:45.000000 ColGenEstimator-0.1.1/ColGenEstimator.egg-info/dependency_links.txt
+-rw-r--r--   0 krunal     (501) staff       (20)        1 2022-08-24 18:48:47.000000 ColGenEstimator-0.1.1/ColGenEstimator.egg-info/not-zip-safe
+-rw-r--r--   0 krunal     (501) staff       (20)      136 2023-06-27 14:26:45.000000 ColGenEstimator-0.1.1/ColGenEstimator.egg-info/requires.txt
+-rw-r--r--   0 krunal     (501) staff       (20)       27 2023-06-27 14:26:45.000000 ColGenEstimator-0.1.1/ColGenEstimator.egg-info/top_level.txt
+-rw-r--r--   0 krunal     (501) staff       (20)       25 2021-12-14 15:40:21.000000 ColGenEstimator-0.1.1/MANIFEST.in
+-rw-r--r--   0 krunal     (501) staff       (20)     3198 2023-06-27 14:26:45.000000 ColGenEstimator-0.1.1/PKG-INFO
+-rw-r--r--   0 krunal     (501) staff       (20)     1852 2023-06-27 13:50:05.000000 ColGenEstimator-0.1.1/README.rst
+drwxr-xr-x   0 krunal     (501) staff       (20)        0 2023-06-27 14:26:45.000000 ColGenEstimator-0.1.1/col_gen_estimator/
+-rw-r--r--   0 krunal     (501) staff       (20)     1099 2022-12-05 19:48:50.000000 ColGenEstimator-0.1.1/col_gen_estimator/__init__.py
+-rw-r--r--   0 krunal     (501) staff       (20)    33599 2022-09-19 18:26:15.000000 ColGenEstimator-0.1.1/col_gen_estimator/_bdr_classifier.py
+-rw-r--r--   0 krunal     (501) staff       (20)    11947 2023-03-18 10:58:40.000000 ColGenEstimator-0.1.1/col_gen_estimator/_col_gen_classifier.py
+-rw-r--r--   0 krunal     (501) staff       (20)   100933 2023-06-27 14:17:39.000000 ColGenEstimator-0.1.1/col_gen_estimator/_dtree_classifier.py
+-rw-r--r--   0 krunal     (501) staff       (20)       22 2023-06-27 14:19:54.000000 ColGenEstimator-0.1.1/col_gen_estimator/_version.py
+drwxr-xr-x   0 krunal     (501) staff       (20)        0 2023-06-27 14:26:45.000000 ColGenEstimator-0.1.1/col_gen_estimator/tests/
+-rw-r--r--   0 krunal     (501) staff       (20)        0 2021-12-14 15:40:21.000000 ColGenEstimator-0.1.1/col_gen_estimator/tests/__init__.py
+-rw-r--r--   0 krunal     (501) staff       (20)     7491 2023-01-27 20:15:50.000000 ColGenEstimator-0.1.1/col_gen_estimator/tests/test_bdrc.py
+-rw-r--r--   0 krunal     (501) staff       (20)      488 2022-08-25 19:12:12.000000 ColGenEstimator-0.1.1/col_gen_estimator/tests/test_common.py
+-rw-r--r--   0 krunal     (501) staff       (20)    12196 2023-06-22 13:19:59.000000 ColGenEstimator-0.1.1/col_gen_estimator/tests/test_dtree.py
+drwxr-xr-x   0 krunal     (501) staff       (20)        0 2023-06-27 14:26:45.000000 ColGenEstimator-0.1.1/examples/
+-rw-r--r--   0 krunal     (501) staff       (20)        0 2023-06-22 15:46:25.000000 ColGenEstimator-0.1.1/examples/__init__.py
+-rw-r--r--   0 krunal     (501) staff       (20)    27066 2023-06-27 13:43:04.000000 ColGenEstimator-0.1.1/examples/dtree_experiment.py
+-rw-r--r--   0 krunal     (501) staff       (20)       48 2023-06-22 16:54:54.000000 ColGenEstimator-0.1.1/requirements.txt
+-rw-r--r--   0 krunal     (501) staff       (20)      148 2023-06-27 14:26:45.000000 ColGenEstimator-0.1.1/setup.cfg
+-rw-r--r--   0 krunal     (501) staff       (20)     2051 2022-07-28 13:33:16.000000 ColGenEstimator-0.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ColGenEstimator-0.0.9/ColGenEstimator.egg-info/PKG-INFO` & `ColGenEstimator-0.1.1/ColGenEstimator.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColGenEstimator
-Version: 0.0.9
+Version: 0.1.1
 Summary: Classifiers using column generation
 Home-page: https://github.com/krooonal/col_gen_estimator
 Maintainer: K. Patel
 Maintainer-email: krunalkachadia@gmail.com
 License: new BSD
 Download-URL: https://github.com/krooonal/col_gen_estimator
 Description: .. -*- mode: rst -*-
@@ -31,18 +31,28 @@
         This project is built using the sklearn template. 
         
         It aids development of estimators that can be used in scikit-learn pipelines
         and (hyper)parameter search, while facilitating testing (including some API
         compliance), documentation, open source development, packaging, and continuous
         integration.
         
-        An example extension of a column generation based binary classifier (Boolean 
-        Decision Rule Generation by S. Dash et. al. 2018) is included. The developer 
-        needs to extend the master and subproblem classes and implement the required
-        methods. The coumn generation part is taken care of by the template fit method.
+        Following example extensions of a column generation based binary classifiers 
+        are included.
+        - Boolean Decision Rule Generation by S. Dash et. al. 2018 
+        - Decision Tree classifiers by Firat et. al. 2020 (modified)  
+        
+        The developer needs to extend the master and subproblem classes and implement 
+        the required methods. The coumn generation part is taken care of by the 
+        template fit method.
+        
+        The Decision Tree Classifier experiments can be launched from the example 
+        directory. See the README file in the examples directory for details.
+        
+        To reproduce the results submitted in the Decision tree paper, use the branch
+        'dtreedev'.
         
         *Thank you for cleanly contributing to the estimator template!*
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
```

### Comparing `ColGenEstimator-0.0.9/PKG-INFO` & `ColGenEstimator-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColGenEstimator
-Version: 0.0.9
+Version: 0.1.1
 Summary: Classifiers using column generation
 Home-page: https://github.com/krooonal/col_gen_estimator
 Maintainer: K. Patel
 Maintainer-email: krunalkachadia@gmail.com
 License: new BSD
 Download-URL: https://github.com/krooonal/col_gen_estimator
 Description: .. -*- mode: rst -*-
@@ -31,18 +31,28 @@
         This project is built using the sklearn template. 
         
         It aids development of estimators that can be used in scikit-learn pipelines
         and (hyper)parameter search, while facilitating testing (including some API
         compliance), documentation, open source development, packaging, and continuous
         integration.
         
-        An example extension of a column generation based binary classifier (Boolean 
-        Decision Rule Generation by S. Dash et. al. 2018) is included. The developer 
-        needs to extend the master and subproblem classes and implement the required
-        methods. The coumn generation part is taken care of by the template fit method.
+        Following example extensions of a column generation based binary classifiers 
+        are included.
+        - Boolean Decision Rule Generation by S. Dash et. al. 2018 
+        - Decision Tree classifiers by Firat et. al. 2020 (modified)  
+        
+        The developer needs to extend the master and subproblem classes and implement 
+        the required methods. The coumn generation part is taken care of by the 
+        template fit method.
+        
+        The Decision Tree Classifier experiments can be launched from the example 
+        directory. See the README file in the examples directory for details.
+        
+        To reproduce the results submitted in the Decision tree paper, use the branch
+        'dtreedev'.
         
         *Thank you for cleanly contributing to the estimator template!*
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
```

### Comparing `ColGenEstimator-0.0.9/README.rst` & `ColGenEstimator-0.1.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -22,13 +22,23 @@
 This project is built using the sklearn template. 
 
 It aids development of estimators that can be used in scikit-learn pipelines
 and (hyper)parameter search, while facilitating testing (including some API
 compliance), documentation, open source development, packaging, and continuous
 integration.
 
-An example extension of a column generation based binary classifier (Boolean 
-Decision Rule Generation by S. Dash et. al. 2018) is included. The developer 
-needs to extend the master and subproblem classes and implement the required
-methods. The coumn generation part is taken care of by the template fit method.
+Following example extensions of a column generation based binary classifiers 
+are included.
+- Boolean Decision Rule Generation by S. Dash et. al. 2018 
+- Decision Tree classifiers by Firat et. al. 2020 (modified)  
+
+The developer needs to extend the master and subproblem classes and implement 
+the required methods. The coumn generation part is taken care of by the 
+template fit method.
+
+The Decision Tree Classifier experiments can be launched from the example 
+directory. See the README file in the examples directory for details.
+
+To reproduce the results submitted in the Decision tree paper, use the branch
+'dtreedev'.
 
 *Thank you for cleanly contributing to the estimator template!*
```

### Comparing `ColGenEstimator-0.0.9/col_gen_estimator/_bdr_classifier.py` & `ColGenEstimator-0.1.1/col_gen_estimator/_bdr_classifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -647,21 +647,21 @@
     def __init__(self, max_iterations=-1,
                  C=10,
                  p=1,
                  rmp_solver_params="",
                  rmp_solver="glop",
                  master_ip_solver_params="",
                  subproblem_solver="cbc",
-                 subproblem_params=[""]):
+                 subproblem_params=[[""]]):
         super(BooleanDecisionRuleClassifier, self).__init__(
             max_iterations,
             master_problem=BDRMasterProblem(
                 C, p, rmp_solver),
-            subproblems=[BDRSubProblem(
-                C, subproblem_solver)],
+            subproblems=[[BDRSubProblem(
+                C, subproblem_solver)]],
             rmp_is_ip=True,
             rmp_solver_params=rmp_solver_params,
             master_ip_solver_params=master_ip_solver_params,
             subproblem_params=subproblem_params)
         # Not used after this but we have to store them for sklearn
         # compatibility.
         self.C = C
@@ -820,22 +820,22 @@
     def __init__(self, max_iterations=-1,
                  C=10,
                  p=1,
                  rmp_solver_params="",
                  rmp_solver="glop",
                  master_ip_solver_params="",
                  subproblem_solver="cbc",
-                 subproblem_params=["", ""]):
+                 subproblem_params=[[""], [""]]):
         super(BooleanDecisionRuleClassifier, self).__init__(
             max_iterations,
             master_problem=BDRMasterProblem(
                 C, p, rmp_solver),
-            subproblems=[BDRHeuristic(K=1),
-                         BDRSubProblem(
-                C, subproblem_solver)],
+            subproblems=[[BDRHeuristic(K=1)],
+                         [BDRSubProblem(
+                             C, subproblem_solver)]],
             rmp_is_ip=True,
             rmp_solver_params=rmp_solver_params,
             master_ip_solver_params=master_ip_solver_params,
             subproblem_params=subproblem_params)
         # Not used after this but we have to store them for sklearn
         # compatibility.
         self.C = C
```

### Comparing `ColGenEstimator-0.0.9/col_gen_estimator/_col_gen_classifier.py` & `ColGenEstimator-0.1.1/col_gen_estimator/_col_gen_classifier.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Base Column Genaration Classifier. One needs to extend this for implementing
 column generation based classifiers.
 """
 
+from time import time
+
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.utils.validation import check_X_y
 from sklearn.utils.multiclass import unique_labels
 from sklearn.preprocessing import LabelEncoder
 
 
 class BaseMasterProblem():
@@ -54,45 +56,86 @@
         Parameters
         ----------
         solver_params : string, default='',
             The solver parameters for solving the integer RMP.
         """
         pass
 
+    def rmp_objective_improved(self):
+        """ (Optional) Returns True if objective value of rmp is improved. 
+        This is used for computing the number of improving iterations.
+        """
+        return False
+
 
 class BaseSubproblem():
     """ Base class for subproblem. One needs to extend this for using with
     ColGenClassifier.
     """
 
     def generate_columns(self, X, y, dual_costs, params):
         """ Generates the new columns to be added to the RMP.
+        Parameters
+        ----------
+        X : ndarray, shape (n_samples, n_features)
+            The input.
+        y : ndarray, shape (n_samples,)
+            The labels.
+        dual_costs:
+            The dual costs and other information needed to update the
+            subproblem.
+        params:
+            The parameters for the subproblem. (TODO: Remove this.)
         """
         pass
 
+    def update_subproblem(self, X, y, dual_costs):
+        """ (Optional) Updates the subproblem model. This is useful when we add
+        more constraints to the master problem. The subproblem needs to be
+        updated to handle new dual cost information.
+        Parameters
+        ----------
+        X : ndarray, shape (n_samples, n_features)
+            The input.
+        y : ndarray, shape (n_samples,)
+            The labels.
+        dual_costs:
+            The dual costs and other information needed to update the
+            subproblem.
+        """
+        return
+
 
 class ColGenClassifier(ClassifierMixin, BaseEstimator):
     """ Base Column Genaration Classifier. One needs to extend this for
     implementing column generation based classifiers.
 
     Parameters
     ----------
     max_iterations : int, default=-1
         Maximum column generation iterations. Negative values removes the
-        iteration limit and the problem is solved till optimality.
+        iteration limit.
+    time_limit : int, default=-1
+        Time limit in seconds. Negative values removes the time limit.
     master_problem : Instance of BaseMasterProblem, default = BaseSubproblem()
-    subproblem : Instance of BaseSubproblem, default = BaseSubproblem()
+    subproblems : List of list of instances of BaseSubproblem according to
+        their levels. The subproblems are called in increasing values of their
+        levels. The list of subproblems at level i+1 is given by
+        subproblems[i+1]. The subproblems[i+1] are called only if the
+        subproblems[i] fail to generate any columns. Typically, the subproblem
+        heuristics are passed at lower levels and the exact methods are passed
+        at the higher levels. Default = [[BaseSubproblem()]]
     rmp_is_ip : boolean, default = False
         True if the master problem has integer variables.
     rmp_solver_params: string, default = "",
         Solver parameters for solving restricted master problem (rmp).
     master_ip_solver_params: string, default = "",
         Solver parameters for solving the integer master problem.
-    subproblem_params: list of string, default = [""],
-        Parameters for solving the subproblem.
+    subproblem_params: list of list of string, default = [""],
+        Parameters for solving the subproblems (as per their levels).
 
     Attributes
     ----------
     X_ : ndarray, shape (n_samples, n_features)
         The input passed during :meth:`fit`.
     y_ : ndarray, shape (n_samples,)
         The labels passed during :meth:`fit`.
@@ -105,28 +148,32 @@
         iteration.
     num_col_added_sp_: list of ints (size = number of subproblems)
         Count of number of columns added to the master problem by each
         subproblem.
     """
 
     def __init__(self, max_iterations=-1,
+                 time_limit=-1,
                  master_problem=BaseMasterProblem(),
-                 subproblems=[BaseSubproblem()],
+                 subproblems=[[BaseSubproblem()]],
                  rmp_is_ip=False,
                  rmp_solver_params="",
                  master_ip_solver_params="",
-                 subproblem_params=[""]):
+                 subproblem_params=[[""]]):
         self.max_iterations = max_iterations
+        self.time_limit = time_limit
         self.master_problem = master_problem
         self.subproblems = subproblems
         self.rmp_is_ip = rmp_is_ip
         self.rmp_solver_params = rmp_solver_params
         self.master_ip_solver_params = master_ip_solver_params
         self.subproblem_params = subproblem_params
         assert len(subproblems) == len(subproblem_params)
+        for level in range(len(subproblems)):
+            assert len(subproblems[level]) == len(subproblem_params[level])
 
     def fit(self, X, y):
         """Runs the column generation loop.
 
         Parameters
         ----------
         X : array-like, shape (n_samples, n_features)
@@ -135,16 +182,18 @@
             The target values. An array of int.
 
         Returns
         -------
         self : object
             Returns self.
         """
+        t_start = time()
         # Check that X and y have correct shape
         X, y = check_X_y(X, y)
+        has_time_limit = self.time_limit > 0
         # Store the classes seen during fit
         self.classes_ = unique_labels(y)
 
         self.X_ = X
         self.y_ = y
 
         # Convert the y into integer class lables.
@@ -156,46 +205,105 @@
             raise ValueError(
                 "Classifier can't train when only one class is present.")
 
         # Initiate the master and subproblems
         self.master_problem.generate_mp(X, self.processed_y_)
 
         self.performed_iter_ = 0
+        self.num_improving_iter_ = 0
         self.mp_optimal_ = False
-        self.num_col_added_sp_ = [0]*len(self.subproblems)
-
-        for iter in range(self.max_iterations):
-            self.performed_iter_ += 1
+        self.time_limit_reached_ = False
+        self.num_col_added_sp_ = []
+        self.time_spent_sp_ = []
+        self.time_add_col_ = 0.0
+        self.time_spent_master_ = 0.0
+        for level in range(len(self.subproblems)):
+            self.num_col_added_sp_.append([0]*len(self.subproblems[level]))
+            self.time_spent_sp_.append([0.0]*len(self.subproblems[level]))
+
+        self.iter_ = 0
+        while True:
+            if self.max_iterations > 0 and self.iter_ >= self.max_iterations:
+                break
+            self.iter_ += 1
+            print("Iteration number: ", self.iter_)
+            print("Time elapsed: ", time() - t_start)
+            master_time_start = time()
             dual_costs = self.master_problem.solve_rmp(self.rmp_solver_params)
+            self.time_spent_master_ += time() - master_time_start
+            if self.master_problem.rmp_objective_improved():
+                self.num_improving_iter_ += 1
+
+            # TODO:Remove this.
+            if hasattr(self.master_problem, 'reset_timer_'):
+                if self.master_problem.reset_timer_:
+                    t_start = time()
+                    self.master_problem.reset_timer_ = False
+                    print("Reset timer.")
 
             rmp_updated = False
-            sp_ind = 0
-            for sp_ind in range(len(self.subproblems)):
-                generated_columns = self.subproblems[sp_ind].generate_columns(
-                    X, self.processed_y_, dual_costs,
-                    self.subproblem_params[sp_ind])
+            # Update the subproblems
+            for sp_level in range(len(self.subproblems)):
+                for sp_ind in range(len(self.subproblems[sp_level])):
+                    sp_time_start = time()
+                    self.subproblems[sp_level][sp_ind] \
+                        .update_subproblem(
+                            X, self.processed_y_, dual_costs)
+                    sp_time_end = time()
+                    self.time_spent_sp_[
+                        sp_level][sp_ind] += sp_time_end - sp_time_start
 
+            for sp_level in range(len(self.subproblems)):
+                # TODO: do this in parallel.
                 rmp_updated = False
-                for column in generated_columns:
-                    col_added = self.master_problem.add_column(column)
-                    self.num_col_added_sp_[sp_ind] += 1 if col_added else 0
-                    rmp_updated = rmp_updated or col_added
+                for sp_ind in range(len(self.subproblems[sp_level])):
+                    self.time_elapsed_ = time() - t_start
+                    if has_time_limit and self.time_elapsed_ > self.time_limit:
+                        self.time_limit_reached_ = True
+                        break
+                    sp_time_start = time()
+                    generated_columns = self.subproblems[sp_level][sp_ind] \
+                        .generate_columns(
+                        X, self.processed_y_, dual_costs,
+                        self.subproblem_params[sp_level][sp_ind])
+                    sp_time_end = time()
+                    self.time_spent_sp_[
+                        sp_level][sp_ind] += sp_time_end - sp_time_start
+
+                    col_add_start = time()
+                    for column in generated_columns:
+                        col_added = self.master_problem.add_column(column)
+                        self.num_col_added_sp_[
+                            sp_level][sp_ind] += 1 if col_added else 0
+                        rmp_updated = rmp_updated or col_added
+                    self.time_add_col_ += time() - col_add_start
+                    if rmp_updated:
+                        break
+                self.time_elapsed_ = time() - t_start
+                if self.time_limit_reached_:
+                    print("Time limit reached!")
+                    break
                 if rmp_updated:
                     break
 
             if not rmp_updated:
                 print("RMP not updated. exiting the loop.")
-                self.mp_optimal_ = True
+                if not self.time_limit_reached_:
+                    self.mp_optimal_ = True
                 break
 
+        self.time_spent_master_ip_ = 0.0
         if self.rmp_is_ip:
+            master_ip_start_time = time()
             solved = self.master_problem.solve_ip(self.master_ip_solver_params)
+            self.time_spent_master_ip_ += time() - master_ip_start_time
             assert solved, "RMP integer program couldn't be solved."
 
         self.is_fitted_ = True
+        self.time_elapsed_ = time() - t_start
         # Return the classifier
         return self
 
     def predict(self, X):
         """ Predicts the class based on the solution of master problem. This
         method is abstract.
```

### Comparing `ColGenEstimator-0.0.9/col_gen_estimator/tests/test_bdrc.py` & `ColGenEstimator-0.1.1/col_gen_estimator/tests/test_bdrc.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,33 +35,33 @@
 def test_default_params():
     clf = BooleanDecisionRuleClassifier()
     assert clf.max_iterations == -1
     assert clf.C == 10
     assert clf.p == 1
     assert clf.rmp_solver_params == ""
     assert clf.master_ip_solver_params == ""
-    assert clf.subproblem_params == [""]
+    assert clf.subproblem_params == [[""]]
     assert clf.rmp_is_ip
 
 
 def test_fit_predict(data):
     clf = BooleanDecisionRuleClassifier(max_iterations=3, C=10, p=1)
     clf.fit(data[0], data[1])
     assert hasattr(clf, 'is_fitted_')
 
     assert hasattr(clf, 'classes_')
     assert hasattr(clf, 'X_')
     assert hasattr(clf, 'y_')
     assert hasattr(clf, 'mp_optimal_')
-    assert hasattr(clf, 'performed_iter_')
+    assert hasattr(clf, 'iter_')
     assert hasattr(clf, 'num_col_added_sp_')
 
     assert_equal(clf.mp_optimal_, True)
-    assert_equal(clf.performed_iter_, 2)
-    assert_equal(clf.num_col_added_sp_[0], 1)
+    assert_equal(clf.iter_, 2)
+    assert_equal(clf.num_col_added_sp_[0][0], 1)
 
     X = data[0]
     y_pred = clf.predict(X)
     assert y_pred.shape == (X.shape[0],)
     assert_array_equal(y_pred, data[1])
 
 
@@ -77,21 +77,21 @@
     clf.fit(data[0], data[1])
     assert hasattr(clf, 'is_fitted_')
 
     assert hasattr(clf, 'classes_')
     assert hasattr(clf, 'X_')
     assert hasattr(clf, 'y_')
     assert hasattr(clf, 'mp_optimal_')
-    assert hasattr(clf, 'performed_iter_')
+    assert hasattr(clf, 'iter_')
     assert hasattr(clf, 'num_col_added_sp_')
 
     assert_equal(clf.mp_optimal_, True)
-    assert_equal(clf.performed_iter_, 3)
-    assert_equal(clf.num_col_added_sp_[0], 2)
-    assert_equal(clf.num_col_added_sp_[1], 1)
+    assert_equal(clf.iter_, 3)
+    assert_equal(clf.num_col_added_sp_[0][0], 2)
+    assert_equal(clf.num_col_added_sp_[1][0], 1)
 
     X = data[0]
     y_pred = clf.predict(X)
     assert y_pred.shape == (X.shape[0],)
     assert_array_equal(y_pred, data[1])
```

### Comparing `ColGenEstimator-0.0.9/col_gen_estimator/tests/test_dtree.py` & `ColGenEstimator-0.1.1/col_gen_estimator/tests/test_dtree.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import pytest
 import numpy as np
+import random
 
 from numpy.testing import assert_array_equal
 from numpy.testing import assert_equal
-from numpy.testing import assert_raises
 
 from col_gen_estimator import DTreeMasterProblem
 from col_gen_estimator import DTreeSubProblem
+from col_gen_estimator import DTreeSubProblemHeuristic
 from col_gen_estimator import DTreeClassifier
 from col_gen_estimator import Split
 from col_gen_estimator import Node
 from col_gen_estimator import Leaf
 from col_gen_estimator import Path
 
 
@@ -33,27 +34,91 @@
     assert_array_equal(leaf.right_nodes, [2, 0])
 
 
 def test_path_set_leaf():
     path = Path()
     path.set_leaf(0, 2)
     assert_array_equal(path.node_ids, [1, 0])
-    assert(path.leaf_id, 0)
+    assert_equal(path.leaf_id, 0)
 
     path.set_leaf(1, 2)
     assert_array_equal(path.node_ids, [1, 0])
-    assert(path.leaf_id, 1)
+    assert_equal(path.leaf_id, 1)
 
     path.set_leaf(2, 2)
     assert_array_equal(path.node_ids, [2, 0])
-    assert(path.leaf_id, 2)
+    assert_equal(path.leaf_id, 2)
 
     path.set_leaf(3, 2)
     assert_array_equal(path.node_ids, [2, 0])
-    assert(path.leaf_id, 3)
+    assert_equal(path.leaf_id, 3)
+
+
+def test_path_is_same_as():
+    path = Path()
+    path.leaf_id = 0
+    path.node_ids = [1, 0]
+    path.splits = [2, 0]
+    path.cost = 1
+    path.target = 1
+    assert(path.is_same_as(path))
+
+    path2 = Path()
+    path2.leaf_id = 0
+    path2.node_ids = [0, 1]
+    path2.splits = [0, 2]
+    path2.cost = 1
+    path2.target = 1
+    assert(path.is_same_as(path2))
+    assert(path2.is_same_as(path))
+
+    # Different leaf
+    path2 = Path()
+    path2.leaf_id = 1
+    path2.node_ids = [0, 1]
+    path2.splits = [0, 2]
+    path2.cost = 1
+    path2.target = 1
+    assert(not path.is_same_as(path2))
+
+    # Different target
+    path2 = Path()
+    path2.leaf_id = 0
+    path2.node_ids = [0, 1]
+    path2.splits = [0, 2]
+    path2.cost = 1
+    path2.target = 0
+    assert(not path.is_same_as(path2))
+
+    # Different cost
+    path2 = Path()
+    path2.leaf_id = 0
+    path2.node_ids = [0, 1]
+    path2.splits = [0, 2]
+    path2.cost = 3
+    path2.target = 1
+    assert(not path.is_same_as(path2))
+
+    # Different node length
+    path2 = Path()
+    path2.leaf_id = 0
+    path2.node_ids = [0, 1, 2]
+    path2.splits = [0, 2, 3]
+    path2.cost = 1
+    path2.target = 1
+    assert(not path.is_same_as(path2))
+
+    # Different splits
+    path2 = Path()
+    path2.leaf_id = 0
+    path2.node_ids = [0, 1]
+    path2.splits = [2, 0]
+    path2.cost = 1
+    path2.target = 1
+    assert(not path.is_same_as(path2))
 
 
 @pytest.fixture
 def data():
     X = np.array([[1, 1, 1],
                   [1, 1, 0],
                   [1, 0, 1],
@@ -64,24 +129,30 @@
                   [0, 0, 0], ], np.int8)
     y = np.array([1, 1, 0, 0, 0, 1, 0, 1], np.int8)
 
     splitA = Split()
     splitA.id = 0
     splitA.feature = 0
     splitA.threshold = 0.5
+    splitA.left_rows = {4, 5, 6, 7}
+    splitA.right_rows = {0, 1, 2, 3}
 
     splitB = Split()
     splitB.id = 1
     splitB.feature = 1
     splitB.threshold = 0.5
+    splitB.left_rows = {2, 3, 6, 7}
+    splitB.right_rows = {0, 1, 4, 5}
 
     splitC = Split()
     splitC.id = 2
     splitC.feature = 2
     splitC.threshold = 0.5
+    splitC.left_rows = {1, 3, 5, 7}
+    splitC.right_rows = {0, 2, 4, 6}
 
     root_node = Node()
     root_node.id = 0
     root_node.candidate_splits = [0]
 
     left_node = Node()
     left_node.id = 1
@@ -156,224 +227,227 @@
     leaves = [leaf_0, leaf_1, leaf_2, leaf_3]
     splits = [splitA, splitB, splitC]
     targets = [0, 1]
 
     return (X, y, paths, nodes, leaves, splits, targets)
 
 
+def print_ns_duals(nodes, leaves, ns_duals):
+    for leaf in leaves:
+        for node in nodes:
+            if node.id not in leaf.left_nodes + leaf.right_nodes:
+                continue
+            for split_id in node.candidate_splits:
+                print("leaf={leaf}, node={node}, split={split},\
+                      dual={dual}".format(
+                    leaf=leaf.id, node=node.id, split=split_id,
+                    dual=ns_duals[leaf.id][node.id][split_id]))
+
+
+def initialize_ns_duals(nodes, leaves):
+    ns_duals = {}
+
+    for leaf_id in range(len(leaves)):
+        ns_duals[leaf_id] = {}
+        leaf_nodes = leaves[leaf_id].left_nodes + leaves[leaf_id].right_nodes
+        for node in nodes:
+            if node.id not in leaf_nodes:
+                continue
+            ns_duals[leaf_id][node.id] = {}
+            for split_id in node.candidate_splits:
+                ns_duals[leaf_id][node.id][split_id] = 0.0
+    return ns_duals
+
+
 def test_master_prob(data):
     X = data[0]
     y = data[1]
     paths = data[2]
     nodes = data[3]
     leaves = data[4]
     splits = data[5]
-    master_problem = DTreeMasterProblem(paths, leaves, nodes, splits)
+    master_problem = DTreeMasterProblem(
+        paths, leaves, nodes, splits, solver_type='glop')
     assert_equal(master_problem.generated_, False)
     master_problem.generate_mp(X, y)
     assert_equal(master_problem.generated_, True)
     duals = master_problem.solve_rmp()
-    assert(len(duals), 3)
+    assert_equal(len(duals), 5)
     leaf_duals = duals[0]
     row_duals = duals[1]
     ns_duals = duals[2]
-    assert_array_equal(leaf_duals, [1, 0, 2, 1])
-    assert_array_equal(row_duals, [0, -1, 0, 0, 0, 1, 0, 0])
-    assert_equal(ns_duals[1][1][2], 2)
-    assert_equal(ns_duals[3][2][1], 2)
+    assert_array_equal(leaf_duals, [2, 2, 1, 3])
+    assert_array_equal(row_duals, [0, 0, 0, 0, 0, 0, 0, 0])
+    print_ns_duals(nodes, leaves, ns_duals)
 
 
 def test_master_prob_add_col(data):
     X = data[0]
     y = data[1]
     paths = data[2][:7]
     nodes = data[3]
     leaves = data[4]
     splits = data[5]
-    master_problem = DTreeMasterProblem(paths, leaves, nodes, splits)
+    master_problem = DTreeMasterProblem(
+        paths, leaves, nodes, splits, solver_type='glop')
     assert_equal(master_problem.generated_, False)
     master_problem.generate_mp(X, y)
     assert_equal(master_problem.generated_, True)
     duals = master_problem.solve_rmp()
-    assert(len(duals), 3)
+    assert_equal(len(duals), 5)
     leaf_duals = duals[0]
     row_duals = duals[1]
     ns_duals = duals[2]
-    assert_array_equal(leaf_duals, [1, 0, 0, 0])
-    assert_array_equal(row_duals, [0, 0, 1, 0, 0, 1, 0, 0])
-    assert_equal(ns_duals[1][1][2], 2)
+    assert_array_equal(leaf_duals, [2, 2, 0, 2])
+    assert_array_equal(row_duals, [0, 0, 0, 0, 0, 0, 0, 0])
+    print_ns_duals(nodes, leaves, ns_duals)
 
-    for leaf in leaves:
-        for node in nodes:
-            if node.id not in leaf.left_nodes + leaf.right_nodes:
-                continue
-            for split_id in node.candidate_splits:
-                print("leaf={leaf}, node={node}, split={split},\
-                      dual={dual}".format(
-                    leaf=leaf.id, node=node.id, split=split_id,
-                    dual=ns_duals[leaf.id][node.id][split_id]))
     path_7 = data[2][-1]
     master_problem.add_column(path_7)
     duals = master_problem.solve_rmp()
-    assert(len(duals), 3)
+    assert_equal(len(duals), 5)
     leaf_duals = duals[0]
     row_duals = duals[1]
     ns_duals = duals[2]
-    assert_array_equal(leaf_duals, [1, 0, 2, 1])
-    assert_array_equal(row_duals, [0, -1, 0, 0, 0, 1, 0, 0])
-    assert_equal(ns_duals[1][1][2], 2)
-    assert_equal(ns_duals[3][2][1], 2)
+    assert_array_equal(leaf_duals, [2, 2, 1, 3])
+    assert_array_equal(row_duals, [0, 0, 0, 0, 0, 0, 0, 0])
+    print_ns_duals(nodes, leaves, ns_duals)
 
 
 def test_subproblem(data):
     X = data[0]
     y = data[1]
-    paths = data[2]
     nodes = data[3]
     leaves = data[4]
     splits = data[5]
     targets = data[6]
     subproblem = DTreeSubProblem(leaves[0], nodes, splits, targets, depth=2)
 
-    leaf_duals = [2, 3, 1, 2]
-    row_duals = [0, 1, 0, 0, 0, -1, 0, 0]
-    ns_duals = {}
+    leaf_duals, row_duals, ns_duals = get_incomplete_mp_duals(nodes, leaves)
 
-    ns_duals[0] = {}
-    zero_nodes = leaves[0].left_nodes + leaves[0].right_nodes
-    for node in nodes:
-        if node.id not in zero_nodes:
-            continue
-        ns_duals[0][node.id] = {}
-        for split_id in node.candidate_splits:
-            ns_duals[0][node.id][split_id] = 0.0
-    duals = (leaf_duals, row_duals, ns_duals)
+    duals = (leaf_duals, row_duals, ns_duals, [], [])
+    subproblem.update_subproblem(X, y, duals)
     new_paths = subproblem.generate_columns(X, y, duals)
-    assert_equal(len(new_paths), 1)
-    path = new_paths[0]
-    assert_equal(path.leaf_id, 0)
-    assert_array_equal(path.node_ids, [0, 1])
-    assert_array_equal(path.splits, [0, 2])
-    assert_equal(path.cost, 2)
-    assert_equal(path.target, 1)
+    assert_array_equal(new_paths, [])
 
 
 def test_subproblem2(data):
     X = data[0]
     y = data[1]
-    paths = data[2]
     nodes = data[3]
     leaves = data[4]
     splits = data[5]
     targets = data[6]
-    subproblem = DTreeSubProblem(leaves[0], nodes, splits, targets, depth=2)
+    subproblem = DTreeSubProblem(leaves[3], nodes, splits, targets, depth=2)
 
-    leaf_duals = [1, 0, 2, 1]
-    row_duals = [0, -1, 0, 0, 0, 1, 0, 0]
-    ns_duals = {}
+    leaf_duals, row_duals, ns_duals = get_incomplete_mp_duals(nodes, leaves)
 
-    ns_duals[0] = {}
-    zero_nodes = leaves[0].left_nodes + leaves[0].right_nodes
-    for node in nodes:
-        if node.id not in zero_nodes:
-            continue
-        ns_duals[0][node.id] = {}
-        for split_id in node.candidate_splits:
-            ns_duals[0][node.id][split_id] = 0.0
-    duals = (leaf_duals, row_duals, ns_duals)
+    duals = (leaf_duals, row_duals, ns_duals, [], [])
+    subproblem.update_subproblem(X, y, duals)
     new_paths = subproblem.generate_columns(X, y, duals)
-    assert_array_equal(new_paths, [])
+    assert_equal(len(new_paths), 1)
+    path = new_paths[0]
+    assert_equal(path.leaf_id, 3)
+    assert_array_equal(path.node_ids, [0, 2])
+    assert_array_equal(path.splits, [0, 1])
+    assert_equal(path.cost, 2)
+    assert_equal(path.target, 1)
 
 
-def test_subproblem3(data):
+def test_get_reduced_cost(data):
     X = data[0]
     y = data[1]
-    paths = data[2]
     nodes = data[3]
     leaves = data[4]
     splits = data[5]
     targets = data[6]
-    subproblem = DTreeSubProblem(leaves[2], nodes, splits, targets, depth=2)
+    subproblem_heuristic = DTreeSubProblemHeuristic(
+        leaves, nodes, splits, targets, depth=2)
 
-    leaf_duals = [1, 0, 0, 0]
-    row_duals = [0, 0, 1, 0, 0, 1, 0, 0]
-    ns_duals = {}
-    for node in nodes:
-        print(node.candidate_splits)
+    leaf_duals, row_duals, ns_duals = get_incomplete_mp_duals(nodes, leaves)
 
-    ns_duals[2] = {}
-    two_nodes = leaves[2].left_nodes + leaves[2].right_nodes
-    for node in nodes:
-        if node.id not in two_nodes:
-            continue
-        ns_duals[2][node.id] = {}
-        for split_id in node.candidate_splits:
-            ns_duals[2][node.id][split_id] = 0.0
-    ns_duals[2][0][0] = 1.0
-    duals = (leaf_duals, row_duals, ns_duals)
-    new_paths = subproblem.generate_columns(X, y, duals)
-    assert_array_equal(new_paths, [])
+    duals = (leaf_duals, row_duals, ns_duals, [], [])
+    path = Path()
+    path.leaf_id = 3
+    path.node_ids = [0, 2]
+    path.splits = [0, 1]
+    path.cost = 2
+    path.target = 1
+    row_satisfies_path_array = [False]*X.shape[0]
+    row_satisfies_path_array[0] = True
+    row_satisfies_path_array[1] = True
+    reduced_cost = subproblem_heuristic.get_reduced_cost(
+        X, y, duals, path, row_satisfies_path_array)
+    # reduced_cost = 2
+    assert(reduced_cost > 1e-6)
+
+
+def get_incomplete_mp_duals(nodes, leaves):
+    leaf_duals = [2, 0, 0, 0]
+    row_duals = [0, 0, 0, 0, 0, 0, 0, 0]
+    ns_duals = initialize_ns_duals(nodes, leaves)
+    ns_duals[0][1][1] = -1
+    ns_duals[1][1][1] = 1
+    ns_duals[1][1][2] = 2
+    ns_duals[2][0][0] = 1
+    ns_duals[2][2][1] = 1
+    ns_duals[3][0][0] = 1
+    ns_duals[3][2][1] = -1
+    return leaf_duals, row_duals, ns_duals
 
 
-def test_subproblem4(data):
+def test_subproblem_heuristic1(data):
     X = data[0]
     y = data[1]
-    paths = data[2]
     nodes = data[3]
     leaves = data[4]
     splits = data[5]
     targets = data[6]
-    subproblem = DTreeSubProblem(leaves[3], nodes, splits, targets, depth=2)
+    subproblem = DTreeSubProblemHeuristic(
+        leaves, nodes, splits, targets, depth=2)
 
-    leaf_duals = [1, 0, 0, 0]
-    row_duals = [0, 0, 1, 0, 0, 1, 0, 0]
-    ns_duals = {}
-    for node in nodes:
-        print(node.candidate_splits)
+    leaf_duals, row_duals, ns_duals = get_incomplete_mp_duals(nodes, leaves)
 
-    ns_duals[3] = {}
-    two_nodes = leaves[3].left_nodes + leaves[3].right_nodes
-    for node in nodes:
-        if node.id not in two_nodes:
-            continue
-        ns_duals[3][node.id] = {}
-        for split_id in node.candidate_splits:
-            ns_duals[3][node.id][split_id] = 0.0
-    duals = (leaf_duals, row_duals, ns_duals)
+    duals = (leaf_duals, row_duals, ns_duals, [], [])
+    random.seed(10)
     new_paths = subproblem.generate_columns(X, y, duals)
     assert_equal(len(new_paths), 1)
     path = new_paths[0]
     assert_equal(path.leaf_id, 3)
-    assert_array_equal(path.node_ids, [0, 2])
-    assert_array_equal(path.splits, [0, 1])
+    assert_array_equal(path.node_ids, [2, 0])
+    assert_array_equal(path.splits, [1, 0])
     assert_equal(path.cost, 2)
     assert_equal(path.target, 1)
 
 
 def test_fit_predict(data):
     X = data[0]
     y = data[1]
     paths = data[2][:7]
     nodes = data[3]
     leaves = data[4]
     splits = data[5]
     clf = DTreeClassifier(paths, leaves, nodes, splits,
-                          tree_depth=2, targets=[0, 1], max_iterations=3)
+                          tree_depth=2, targets=[0, 1], max_iterations=5,
+                          master_solver_type='glop')
     clf.fit(X, y)
     assert hasattr(clf, 'is_fitted_')
     assert hasattr(clf, 'classes_')
     assert hasattr(clf, 'X_')
     assert hasattr(clf, 'y_')
     assert hasattr(clf, 'mp_optimal_')
-    assert hasattr(clf, 'performed_iter_')
+    assert hasattr(clf, 'iter_')
     assert hasattr(clf, 'num_col_added_sp_')
 
     assert_equal(clf.mp_optimal_, True)
-    assert_equal(clf.performed_iter_, 2)
-    assert_equal(clf.num_col_added_sp_[0], 0)
-    assert_equal(clf.num_col_added_sp_[1], 0)
-    assert_equal(clf.num_col_added_sp_[2], 0)
-    assert_equal(clf.num_col_added_sp_[3], 1)
+    assert_equal(clf.iter_, 2)
+    total_cols_added = clf.num_col_added_sp_[
+        0][0] + sum(clf.num_col_added_sp_[1])
+    assert_equal(total_cols_added, 1)
+
+    assert_equal(clf.num_col_added_sp_[1][0], 0)
+    assert_equal(clf.num_col_added_sp_[1][1], 0)
+    assert_equal(clf.num_col_added_sp_[1][2], 0)
 
     y_pred = clf.predict(X)
     assert y_pred.shape == (X.shape[0],)
     assert_array_equal(y_pred, y)
```

### Comparing `ColGenEstimator-0.0.9/setup.py` & `ColGenEstimator-0.1.1/setup.py`

 * *Files identical despite different names*

