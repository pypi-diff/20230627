# Comparing `tmp/causica-0.3.2.tar.gz` & `tmp/causica-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causica-0.3.2.tar", max compression
+gzip compressed data, was "causica-0.3.3.tar", max compression
```

## Comparing `causica-0.3.2.tar` & `causica-0.3.3.tar`

### file list

```diff
@@ -1,70 +1,67 @@
--rw-r--r--   0        0        0     1141 2023-04-28 16:47:19.490397 causica-0.3.2/LICENSE
--rw-r--r--   0        0        0     7092 2023-04-28 16:47:19.490397 causica-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-04-28 16:47:19.500397 causica-0.3.2/examples/__init__.py
--rw-r--r--   0        0        0    76973 2023-04-28 16:47:19.500397 causica-0.3.2/examples/csuite_example.ipynb
--rw-r--r--   0        0        0   530941 2023-04-28 16:47:19.500397 causica-0.3.2/examples/multi_investment_sales_attribution.ipynb
--rw-r--r--   0        0        0      790 2023-04-28 17:58:20.964181 causica-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-28 16:47:19.500397 causica-0.3.2/src/causica/__init__.py
--rw-r--r--   0        0        0      153 2023-04-28 16:47:19.500397 causica-0.3.2/src/causica/config/lightning/default_data.yaml
--rw-r--r--   0        0        0     1227 2023-04-28 16:47:19.500397 causica-0.3.2/src/causica/config/lightning/default_gaussian.yaml
--rw-r--r--   0        0        0     1225 2023-04-28 16:47:19.500397 causica-0.3.2/src/causica/config/lightning/default_spline.yaml
--rw-r--r--   0        0        0        0 2023-04-28 16:47:19.500397 causica-0.3.2/src/causica/datasets/__init__.py
--rw-r--r--   0        0        0    12768 2023-04-28 16:47:19.500397 causica-0.3.2/src/causica/datasets/causica_dataset_format.py
--rw-r--r--   0        0        0     2642 2023-04-28 16:47:19.500397 causica-0.3.2/src/causica/datasets/interventional_data.py
--rw-r--r--   0        0        0     1230 2023-04-28 16:47:19.500397 causica-0.3.2/src/causica/datasets/loaded_expert_graph_container.py
--rw-r--r--   0        0        0     2454 2023-04-28 16:47:19.500397 causica-0.3.2/src/causica/datasets/standardizer.py
--rw-r--r--   0        0        0     1959 2023-04-28 16:47:19.500397 causica-0.3.2/src/causica/datasets/tensordict_utils.py
--rw-r--r--   0        0        0      307 2023-04-28 16:47:19.500397 causica-0.3.2/src/causica/datasets/variable_types.py
--rw-r--r--   0        0        0      891 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/distributions/__init__.py
--rw-r--r--   0        0        0      613 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/distributions/adjacency/__init__.py
--rw-r--r--   0        0        0     3600 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/distributions/adjacency/adjacency_distributions.py
--rw-r--r--   0        0        0     8583 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/distributions/adjacency/constrained_adjacency_distributions.py
--rw-r--r--   0        0        0     3401 2023-04-28 17:58:20.964181 causica-0.3.2/src/causica/distributions/adjacency/directed_acyclic.py
--rw-r--r--   0        0        0     8118 2023-04-28 17:58:20.964181 causica-0.3.2/src/causica/distributions/adjacency/enco.py
--rw-r--r--   0        0        0     3952 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/distributions/adjacency/gibbs_dag_prior.py
--rw-r--r--   0        0        0     4897 2023-04-28 17:58:20.964181 causica-0.3.2/src/causica/distributions/adjacency/three_way.py
--rw-r--r--   0        0        0      773 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/distributions/distribution_module.py
--rw-r--r--   0        0        0      649 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/distributions/gumbel_binary.py
--rw-r--r--   0        0        0      595 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/distributions/noise/__init__.py
--rw-r--r--   0        0        0     3612 2023-04-28 17:58:20.964181 causica-0.3.2/src/causica/distributions/noise/bernoulli.py
--rw-r--r--   0        0        0     3222 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/distributions/noise/categorical.py
--rw-r--r--   0        0        0     7593 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/distributions/noise/joint.py
--rw-r--r--   0        0        0     3389 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/distributions/noise/noise.py
--rw-r--r--   0        0        0      112 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/distributions/noise/spline/__init__.py
--rw-r--r--   0        0        0     6539 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/distributions/noise/spline/bayesiains_nsf_rqs.py
--rw-r--r--   0        0        0     4340 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/distributions/noise/spline/rational_quadratic_transform.py
--rw-r--r--   0        0        0     8024 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/distributions/noise/spline/spline.py
--rw-r--r--   0        0        0     1736 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/distributions/noise/univariate_normal.py
--rw-r--r--   0        0        0     4058 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/distributions/sem_distribution.py
--rw-r--r--   0        0        0     3063 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/distributions/transforms.py
--rw-r--r--   0        0        0      516 2023-04-28 16:47:19.500397 causica-0.3.2/src/causica/fsspec_helpers.py
--rw-r--r--   0        0        0      310 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/functional_relationships/__init__.py
--rw-r--r--   0        0        0     4574 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/functional_relationships/do_functional_relationships.py
--rw-r--r--   0        0        0     2330 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/functional_relationships/functional_relationships.py
--rw-r--r--   0        0        0     9442 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/functional_relationships/icgnn.py
--rw-r--r--   0        0        0     2949 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/functional_relationships/linear_functional_relationships.py
--rw-r--r--   0        0        0        0 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/graph/__init__.py
--rw-r--r--   0        0        0      375 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/graph/dag_constraint.py
--rw-r--r--   0        0        0     2711 2023-04-28 16:47:19.510397 causica-0.3.2/src/causica/graph/evaluation_metrics.py
--rw-r--r--   0        0        0        0 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/lightning/__init__.py
--rw-r--r--   0        0        0     3437 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/lightning/callbacks.py
--rw-r--r--   0        0        0      718 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/lightning/cli.py
--rw-r--r--   0        0        0        0 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/lightning/data_modules/__init__.py
--rw-r--r--   0        0        0     3052 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/lightning/data_modules/basic_data_module.py
--rw-r--r--   0        0        0     1143 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/lightning/data_modules/deci_data_module.py
--rw-r--r--   0        0        0     7778 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/lightning/data_modules/variable_spec_data.py
--rw-r--r--   0        0        0      776 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/lightning/main.py
--rw-r--r--   0        0        0        0 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/lightning/modules/__init__.py
--rw-r--r--   0        0        0    12424 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/lightning/modules/deci_module.py
--rw-r--r--   0        0        0     2096 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/lightning/modules/variable_spec_module.py
--rw-r--r--   0        0        0     1289 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/mlflow_helpers.py
--rw-r--r--   0        0        0        0 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/sem/__init__.py
--rw-r--r--   0        0        0     3711 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/sem/distribution_parameters_sem.py
--rw-r--r--   0        0        0     6175 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/sem/structural_equation_model.py
--rw-r--r--   0        0        0        0 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/training/__init__.py
--rw-r--r--   0        0        0    10903 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/training/auglag.py
--rw-r--r--   0        0        0     5286 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/training/evaluation.py
--rw-r--r--   0        0        0     8958 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/training/per_variable_metrics.py
--rw-r--r--   0        0        0     1169 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/training/training_callbacks.py
--rw-r--r--   0        0        0     1725 2023-04-28 16:47:19.520397 causica-0.3.2/src/causica/triangular_transformations.py
--rw-r--r--   0        0        0     7912 1970-01-01 00:00:00.000000 causica-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1141 2023-06-26 14:58:36.920302 causica-0.3.3/LICENSE
+-rw-r--r--   0        0        0     7092 2023-06-26 14:58:36.920302 causica-0.3.3/README.md
+-rw-r--r--   0        0        0      746 2023-06-27 09:25:26.129804 causica-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/__init__.py
+-rw-r--r--   0        0        0      172 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/config/lightning/default_data.yaml
+-rw-r--r--   0        0        0     1222 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/config/lightning/default_gaussian.yaml
+-rw-r--r--   0        0        0     1220 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/config/lightning/default_spline.yaml
+-rw-r--r--   0        0        0        0 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/datasets/__init__.py
+-rw-r--r--   0        0        0    13602 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/datasets/causica_dataset_format.py
+-rw-r--r--   0        0        0     2642 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/datasets/interventional_data.py
+-rw-r--r--   0        0        0     1230 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/datasets/loaded_expert_graph_container.py
+-rw-r--r--   0        0        0     2454 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/datasets/standardizer.py
+-rw-r--r--   0        0        0     1959 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/datasets/tensordict_utils.py
+-rw-r--r--   0        0        0      307 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/datasets/variable_types.py
+-rw-r--r--   0        0        0      801 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/distributions/__init__.py
+-rw-r--r--   0        0        0      613 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/adjacency/__init__.py
+-rw-r--r--   0        0        0     3600 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/adjacency/adjacency_distributions.py
+-rw-r--r--   0        0        0     8635 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/distributions/adjacency/constrained_adjacency_distributions.py
+-rw-r--r--   0        0        0     3442 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/distributions/adjacency/directed_acyclic.py
+-rw-r--r--   0        0        0     8118 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/adjacency/enco.py
+-rw-r--r--   0        0        0     4125 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/distributions/adjacency/gibbs_dag_prior.py
+-rw-r--r--   0        0        0     4897 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/adjacency/three_way.py
+-rw-r--r--   0        0        0      773 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/distribution_module.py
+-rw-r--r--   0        0        0      649 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/gumbel_binary.py
+-rw-r--r--   0        0        0      595 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/noise/__init__.py
+-rw-r--r--   0        0        0     3631 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/distributions/noise/bernoulli.py
+-rw-r--r--   0        0        0     3222 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/noise/categorical.py
+-rw-r--r--   0        0        0     7593 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/noise/joint.py
+-rw-r--r--   0        0        0     3389 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/noise/noise.py
+-rw-r--r--   0        0        0      112 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/noise/spline/__init__.py
+-rw-r--r--   0        0        0     6474 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/distributions/noise/spline/bayesiains_nsf_rqs.py
+-rw-r--r--   0        0        0     4340 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/noise/spline/rational_quadratic_transform.py
+-rw-r--r--   0        0        0     8024 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/noise/spline/spline.py
+-rw-r--r--   0        0        0     1736 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/distributions/noise/univariate_normal.py
+-rw-r--r--   0        0        0     5651 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/distributions/transforms.py
+-rw-r--r--   0        0        0      516 2023-06-26 14:58:36.920302 causica-0.3.3/src/causica/fsspec_helpers.py
+-rw-r--r--   0        0        0      264 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/functional_relationships/__init__.py
+-rw-r--r--   0        0        0     4591 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/functional_relationships/do_functional_relationships.py
+-rw-r--r--   0        0        0     1559 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/functional_relationships/functional_relationships.py
+-rw-r--r--   0        0        0     9076 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/functional_relationships/icgnn.py
+-rw-r--r--   0        0        0     2649 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/functional_relationships/linear_functional_relationships.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/graph/__init__.py
+-rw-r--r--   0        0        0      375 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/graph/dag_constraint.py
+-rw-r--r--   0        0        0     2711 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/graph/evaluation_metrics.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/lightning/__init__.py
+-rw-r--r--   0        0        0     3954 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/lightning/callbacks.py
+-rw-r--r--   0        0        0      748 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/lightning/cli.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/lightning/data_modules/__init__.py
+-rw-r--r--   0        0        0     3052 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/lightning/data_modules/basic_data_module.py
+-rw-r--r--   0        0        0     1143 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/lightning/data_modules/deci_data_module.py
+-rw-r--r--   0        0        0     7778 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/lightning/data_modules/variable_spec_data.py
+-rw-r--r--   0        0        0     2098 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/lightning/loggers.py
+-rw-r--r--   0        0        0      776 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/lightning/main.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/lightning/modules/__init__.py
+-rw-r--r--   0        0        0    12157 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/lightning/modules/deci_module.py
+-rw-r--r--   0        0        0     2088 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/lightning/modules/variable_spec_module.py
+-rw-r--r--   0        0        0     1289 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/mlflow_helpers.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/sem/__init__.py
+-rw-r--r--   0        0        0     3711 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/sem/distribution_parameters_sem.py
+-rw-r--r--   0        0        0     4058 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/sem/sem_distribution.py
+-rw-r--r--   0        0        0     6277 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/sem/structural_equation_model.py
+-rw-r--r--   0        0        0        0 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/training/__init__.py
+-rw-r--r--   0        0        0    11827 2023-06-27 09:25:26.129804 causica-0.3.3/src/causica/training/auglag.py
+-rw-r--r--   0        0        0     5286 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/training/evaluation.py
+-rw-r--r--   0        0        0     8958 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/training/per_variable_metrics.py
+-rw-r--r--   0        0        0     1725 2023-06-26 14:58:36.930302 causica-0.3.3/src/causica/triangular_transformations.py
+-rw-r--r--   0        0        0     7905 1970-01-01 00:00:00.000000 causica-0.3.3/PKG-INFO
```

### Comparing `causica-0.3.2/LICENSE` & `causica-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/README.md` & `causica-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/pyproject.toml` & `causica-0.3.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 [tool.poetry]
 name = "causica"
-version = "0.3.2"
+version = "0.3.3"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
-    { include = "causica", from = "src" },
-    { include = "examples", from = "." },
+    { include = "causica", from = "src" }
 ]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "~3.10"
 azureml-mlflow = "^1.46.0"
 mlflow = "^2.0.0"
@@ -18,15 +17,15 @@
 pandas = "^1.4.2"
 tensorboard = "^2.9.0"
 pytorch-lightning = {version = "^1.9.0", extras= ["extra"]}
 jsonargparse = "<4.21.0"  # 4.21.0 breaks lightning cli
 dataclasses-json = "^0.5.7"
 types-PyYAML = "^6.0.12.2"
 tensordict = "^0.1.0"
-torch = "^2.0.0"
+torch = "2.0.0"
 numba = "^0.56.0"  # needed to make the build work
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 
 [build-system]
```

### Comparing `causica-0.3.2/src/causica/config/lightning/default_gaussian.yaml` & `causica-0.3.3/src/causica/config/lightning/default_gaussian.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 seed_everything: 234
 model:
-  class_path: causica.lightning.deci_module.DECIModule
+  class_path: causica.lightning.modules.deci_module.DECIModule
   init_args:
     noise_dist: "GAUSSIAN"
     embedding_size: 32
     out_dim_g: 32
     norm_layer: true
     res_connection: true
     init_alpha: 0.0
@@ -35,13 +35,13 @@
 trainer:
   max_epochs: 2000
 best_checkpoint_callback:
   dirpath: "./outputs"
   filename: "best_model"
   save_top_k: 1
   mode: "max"
-  monitor: "average_batch_log_prob"
-  every_n_train_steps: 1
+  monitor: "batch_log_prob"
+  every_n_epochs: 1
 last_checkpoint_callback:
   save_last: true
   filename: "last_model"
   save_top_k: 0  # only the last checkpoint is saved
```

### Comparing `causica-0.3.2/src/causica/config/lightning/default_spline.yaml` & `causica-0.3.3/src/causica/config/lightning/default_spline.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 seed_everything: 234
 model:
-  class_path: causica.lightning.deci_module.DECIModule
+  class_path: causica.lightning.modules.deci_module.DECIModule
   init_args:
     noise_dist: "SPLINE"
     embedding_size: 32
     out_dim_g: 32
     norm_layer: true
     res_connection: true
     init_alpha: 0.0
@@ -35,13 +35,13 @@
 trainer:
   max_epochs: 2000
 best_checkpoint_callback:
   dirpath: "./outputs"
   filename: "best_model"
   save_top_k: 1
   mode: "max"
-  monitor: "average_batch_log_prob"
-  every_n_train_steps: 1
+  monitor: "batch_log_prob"
+  every_n_epochs: 1
 last_checkpoint_callback:
   save_last: true
   filename: "last_model"
   save_top_k: 0  # only the last checkpoint is saved
```

### Comparing `causica-0.3.2/src/causica/datasets/causica_dataset_format.py` & `causica-0.3.3/src/causica/datasets/causica_dataset_format.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         The downloaded data (the type depends on the data requested)
     """
 
     path_name = os.path.join(root_path, data_enum.value)
 
     fsspec_open = partial(fsspec.open, mode="r", encoding="utf-8", **storage_options)
 
-    logger.debug(f"Loading {data_enum} from {path_name} with storage options {storage_options}")
+    logger.debug("Loading %s from %s with storage options %s", data_enum, path_name, storage_options)
 
     if data_enum == DataEnum.TRUE_ADJACENCY:
         with fsspec_open(path_name) as f:
             return torch.tensor(np.loadtxt(f, dtype=int, delimiter=","))
 
     if data_enum == DataEnum.VARIABLES_JSON:
         if variables_metadata is not None:
@@ -85,27 +85,28 @@
         with fsspec_open(path_name) as f:
             return convert_variable_types_to_enum(json.load(f))
 
     if variables_metadata is None:
         variables_metadata = load_data(root_path, data_enum=DataEnum.VARIABLES_JSON)
 
     with fsspec_open(path_name) as f:
-        if data_enum in {DataEnum.TRAIN, DataEnum.TEST}:
-            arr = np.loadtxt(f, delimiter=",")
-            categorical_sizes = _get_categorical_sizes(variables_list=variables_metadata["variables"])
-            return convert_one_hot(
-                tensordict_from_variables_metadata(arr, variables_metadata["variables"]),
-                one_hot_sizes=categorical_sizes,
-            )
-        elif data_enum == DataEnum.INTERVENTIONS:
-            return _load_interventions(json_object=json.load(f), metadata=variables_metadata)
-        elif data_enum == DataEnum.COUNTERFACTUALS:
-            return _load_counterfactuals(json_object=json.load(f), metadata=variables_metadata)
-        else:
-            raise RuntimeError("Unrecognized data type")
+        match data_enum:
+            case (DataEnum.TRAIN | DataEnum.TEST):
+                arr = np.loadtxt(f, delimiter=",")
+                categorical_sizes = _get_categorical_sizes(variables_list=variables_metadata["variables"])
+                return convert_one_hot(
+                    tensordict_from_variables_metadata(arr, variables_metadata["variables"]),
+                    one_hot_sizes=categorical_sizes,
+                )
+            case DataEnum.INTERVENTIONS:
+                return _load_interventions(json_object=json.load(f), metadata=variables_metadata)
+            case DataEnum.COUNTERFACTUALS:
+                return _load_counterfactuals(json_object=json.load(f), metadata=variables_metadata)
+
+        raise RuntimeError("Unrecognized data type")
 
 
 def _load_interventions(json_object: dict[str, Any], metadata: dict[str, Any]) -> list[InterventionWithEffects]:
     """
     Load the Interventional Datasets as a list of interventions/counterfactuals.
 
     Args:
@@ -303,7 +304,26 @@
     """
     return torch.cat(tuple(tensor_dict.values()), dim=-1)
 
 
 def _intersect_dicts_left(dict_1: dict, dict_2: dict) -> dict:
     """Select the keys that are in both dictionaries, with values from the first."""
     return {key: dict_1[key] for key in dict_1.keys() & dict_2.keys()}
+
+
+def get_group_names(variables_dict: dict[str, Any]) -> list[str]:
+    """Get the names of the groups in the variables dict."""
+    return list(dict.fromkeys([var["group_name"] for var in variables_dict["variables"]]))
+
+
+def get_group_idxs(variables_dict: dict[str, Any]) -> list[list[int]]:
+    """Get the indices of the nodes/groups in each group."""
+    group_names = get_group_names(variables_dict)
+    return [
+        [idx for idx, var in enumerate(variables_dict["variables"]) if var["group_name"] == group_name]
+        for group_name in group_names
+    ]
+
+
+def get_name_to_idx(variables_dict: dict[str, Any]) -> dict[str, int]:
+    """Get a dictionary mapping node/group names to their index in the variables dict."""
+    return {var["name"]: idx for idx, var in enumerate(variables_dict["variables"])}
```

### Comparing `causica-0.3.2/src/causica/datasets/interventional_data.py` & `causica-0.3.3/src/causica/datasets/interventional_data.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/datasets/loaded_expert_graph_container.py` & `causica-0.3.3/src/causica/datasets/loaded_expert_graph_container.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/datasets/standardizer.py` & `causica-0.3.3/src/causica/datasets/standardizer.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/datasets/tensordict_utils.py` & `causica-0.3.3/src/causica/datasets/tensordict_utils.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/distributions/__init__.py` & `causica-0.3.3/src/causica/distributions/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,8 +24,7 @@
     SplineNoise,
     SplineNoiseModule,
     UnivariateNormalNoise,
     UnivariateNormalNoiseModule,
     create_noise_modules,
     create_spline_dist_params,
 )
-from causica.distributions.sem_distribution import SEMDistribution, SEMDistributionModule
```

### Comparing `causica-0.3.2/src/causica/distributions/adjacency/__init__.py` & `causica-0.3.3/src/causica/distributions/adjacency/__init__.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/distributions/adjacency/adjacency_distributions.py` & `causica-0.3.3/src/causica/distributions/adjacency/adjacency_distributions.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/distributions/adjacency/constrained_adjacency_distributions.py` & `causica-0.3.3/src/causica/distributions/adjacency/constrained_adjacency_distributions.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,16 +125,18 @@
         interpretation.
     """
     assert graph_constraint_matrix.ndim == 2, "Constraint matrix must be 2D."
     assert graph_constraint_matrix.shape[0] == graph_constraint_matrix.shape[1], "Constraint matrix must be square."
     # Mask self-edges
     mask = ~torch.eye(graph_constraint_matrix.shape[0], dtype=torch.bool, device=graph_constraint_matrix.device)
 
-    positive_constraints = mask * torch.nan_to_num(graph_constraint_matrix, nan=0).to(dtype=torch.bool)
-    negative_constraints = torch.nan_to_num(graph_constraint_matrix, nan=1).to(dtype=torch.bool)
+    positive_constraints = mask * torch.nan_to_num(graph_constraint_matrix, nan=0).to(
+        dtype=torch.bool, non_blocking=True
+    )
+    negative_constraints = torch.nan_to_num(graph_constraint_matrix, nan=1).to(dtype=torch.bool, non_blocking=True)
     return positive_constraints, negative_constraints
 
 
 def _create_distribution(
     dist_class: Type[AdjacencyDistribution], *args, graph_constraint_matrix: torch.Tensor, **kwargs
 ) -> ConstrainedAdjacencyDistribution:
     """Utility function for generating a constrained adjacency distribution with a base distribution.
```

### Comparing `causica-0.3.2/src/causica/distributions/adjacency/directed_acyclic.py` & `causica-0.3.3/src/causica/distributions/adjacency/directed_acyclic.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,17 @@
         # generate the lower triangle shape [..., n, n]
         low_tri = fill_triangular(self.bern_dist.sample(sample_shape=sample_shape))
 
         # generate a random permutation matrix
         aranges = np.tile(np.arange(self.num_nodes), sample_shape + self.probs.shape + (1,))  # shape [..., n]
         np_perms = torch.tensor(self.np_rng.permuted(aranges, axis=-1))  # a batch of rearranged [0, 1, 2... n]
         # one hot the last dimension to create a tensor of shape [..., n, n]
-        perms = torch.nn.functional.one_hot(np_perms, num_classes=self.num_nodes).to(dtype=low_tri.dtype)
+        perms = torch.nn.functional.one_hot(np_perms, num_classes=self.num_nodes).to(
+            dtype=low_tri.dtype, non_blocking=True
+        )
 
         return torch.einsum("...ij,...jk,...lk->...il", perms, low_tri, perms)
 
     def entropy(self) -> torch.Tensor:
         raise NotImplementedError
 
     @property
```

### Comparing `causica-0.3.2/src/causica/distributions/adjacency/enco.py` & `causica-0.3.3/src/causica/distributions/adjacency/enco.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/distributions/adjacency/gibbs_dag_prior.py` & `causica-0.3.3/src/causica/distributions/adjacency/gibbs_dag_prior.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,18 @@
             confidence: A value in the interval (0, 1] indicating the confidence of the existence of the edge
             scale: Scaling factor for expert graph loss
         """
         super().__init__()
 
         self.dag = torch.nn.Parameter(dag, requires_grad=False)
         self.mask = torch.nn.Parameter(mask, requires_grad=False)
-        self.confidence = confidence
-        self.scale = scale
+        self.confidence: torch.Tensor
+        self.scale: torch.Tensor
+        self.register_buffer("confidence", torch.tensor(confidence, dtype=torch.float))
+        self.register_buffer("scale", torch.tensor(scale, dtype=torch.float))
 
 
 class GibbsDAGPrior(td.Distribution):
     """
     Represents a prior distribution over adjacency matrices.
 
     The prior distribution consists of two terms:
```

### Comparing `causica-0.3.2/src/causica/distributions/adjacency/three_way.py` & `causica-0.3.3/src/causica/distributions/adjacency/three_way.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/distributions/distribution_module.py` & `causica-0.3.3/src/causica/distributions/distribution_module.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/distributions/gumbel_binary.py` & `causica-0.3.3/src/causica/distributions/gumbel_binary.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/distributions/noise/__init__.py` & `causica-0.3.3/src/causica/distributions/noise/__init__.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/distributions/noise/bernoulli.py` & `causica-0.3.3/src/causica/distributions/noise/bernoulli.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     @property
     def mode(self):
         """
         Override the default `mode` method to prevent it returning nan's.
 
         We favour sparseness, so if logit == 0, set the mode to be zero.
         """
-        return (self.logits > 0).to(self.logits)
+        return (self.logits > 0).to(self.logits, non_blocking=True)
 
 
 class BernoulliNoiseModule(NoiseModule[IndependentNoise[BernoulliNoise]]):
     """Represents a BernoulliNoise distribution with learnable logits."""
 
     def __init__(self, dim: int):
         """
```

### Comparing `causica-0.3.2/src/causica/distributions/noise/categorical.py` & `causica-0.3.3/src/causica/distributions/noise/categorical.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/distributions/noise/joint.py` & `causica-0.3.3/src/causica/distributions/noise/joint.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/distributions/noise/noise.py` & `causica-0.3.3/src/causica/distributions/noise/noise.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/distributions/noise/spline/bayesiains_nsf_rqs.py` & `causica-0.3.3/src/causica/distributions/noise/spline/bayesiains_nsf_rqs.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,25 +157,25 @@
             input_derivatives_plus_one * root.pow(2)
             + 2 * input_delta * theta_one_minus_theta
             + input_derivatives * (1 - root).pow(2)
         )
         logabsdet = torch.log(derivative_numerator) - 2 * torch.log(denominator)
 
         return outputs, -logabsdet
-    else:
-        theta = (inputs - input_cumwidths) / input_bin_widths
-        theta_one_minus_theta = theta * (1 - theta)
 
-        numerator = input_heights * (input_delta * theta.pow(2) + input_derivatives * theta_one_minus_theta)
-        denominator = input_delta + (
-            (input_derivatives + input_derivatives_plus_one - 2 * input_delta) * theta_one_minus_theta
-        )
-        outputs = input_cumheights + numerator / denominator
+    theta = (inputs - input_cumwidths) / input_bin_widths
+    theta_one_minus_theta = theta * (1 - theta)
 
-        derivative_numerator = input_delta.pow(2) * (
-            input_derivatives_plus_one * theta.pow(2)
-            + 2 * input_delta * theta_one_minus_theta
-            + input_derivatives * (1 - theta).pow(2)
-        )
-        logabsdet = torch.log(derivative_numerator) - 2 * torch.log(denominator)
+    numerator = input_heights * (input_delta * theta.pow(2) + input_derivatives * theta_one_minus_theta)
+    denominator = input_delta + (
+        (input_derivatives + input_derivatives_plus_one - 2 * input_delta) * theta_one_minus_theta
+    )
+    outputs = input_cumheights + numerator / denominator
+
+    derivative_numerator = input_delta.pow(2) * (
+        input_derivatives_plus_one * theta.pow(2)
+        + 2 * input_delta * theta_one_minus_theta
+        + input_derivatives * (1 - theta).pow(2)
+    )
+    logabsdet = torch.log(derivative_numerator) - 2 * torch.log(denominator)
 
-        return outputs, logabsdet
+    return outputs, logabsdet
```

### Comparing `causica-0.3.2/src/causica/distributions/noise/spline/rational_quadratic_transform.py` & `causica-0.3.3/src/causica/distributions/noise/spline/rational_quadratic_transform.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/distributions/noise/spline/spline.py` & `causica-0.3.3/src/causica/distributions/noise/spline/spline.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/distributions/noise/univariate_normal.py` & `causica-0.3.3/src/causica/distributions/noise/univariate_normal.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/distributions/sem_distribution.py` & `causica-0.3.3/src/causica/sem/sem_distribution.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/fsspec_helpers.py` & `causica-0.3.3/src/causica/fsspec_helpers.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/functional_relationships/do_functional_relationships.py` & `causica-0.3.3/src/causica/functional_relationships/do_functional_relationships.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,35 +14,36 @@
         Args:
             func: The unintervened functional relationships
             do: the nodes on which to intervene
             submatrix: the submatrix that the unintervened nodes represent in the larger graph
         """
         assert all(val.ndim == 1 for val in do.values()), "Intervention is only supported for 1 vector per variable"
 
-        new_variables = {key: value for key, value in func.variables.items() if key not in do.keys()}
-        super().__init__(new_variables)
+        new_shapes = {key: shape for key, shape in func.shapes.items() if key not in do.keys()}
+        super().__init__(new_shapes)
 
         self.func = func
         self.do = do  # dict of key to vectors
         self.submatrix = submatrix
 
         self.do_nodes_mask = torch.tensor(
-            [(name in self.do.keys()) for name in self.func.variables.keys()], dtype=torch.bool
+            [(name in self.do.keys()) for name in self.func.shapes.keys()], dtype=torch.bool
         )
 
     def pad_intervened_graphs(self, graphs: torch.Tensor) -> torch.Tensor:
         """
         Pad the intervened graph with the unintervened nodes.
 
         Args:
             graphs: Weighted adjacency matrix, size batch_size_g + (do_func_n, do_func_n)
         Returns:
             A tensor of shape batch_shape_g + (func_n, func_n)
         """
-        target_shape = graphs.shape[:-2] + (self.func.num_nodes, self.func.num_nodes)
+        num_nodes = self.func.tensor_to_td.num_keys
+        target_shape = graphs.shape[:-2] + (num_nodes, num_nodes)
 
         output_graphs = torch.zeros(target_shape, dtype=graphs.dtype, device=graphs.device)
         assign_submatrix(output_graphs, graphs, ~self.do_nodes_mask, ~self.do_nodes_mask)
         assign_submatrix(output_graphs, self.submatrix, self.do_nodes_mask, ~self.do_nodes_mask)
         return output_graphs
 
     def forward(self, samples: TensorDict, graphs: torch.Tensor) -> TensorDict:
@@ -89,15 +90,15 @@
     Args:
         interventions: the nodes and their intervention values
         func: the functional relationship of the unintervened SEM
         graph: the unintervened graph shape: [..., num_nodes, num_nodes]
     Return:
         A tuple with the intervened functional relationship and the intervened graph
     """
-    node_names = list(func.variables.keys())
+    node_names = list(func.shapes.keys())
     do_nodes_mask = torch.zeros(len(node_names), dtype=torch.bool)
     for i, name in enumerate(node_names):
         if name in interventions.keys():
             do_nodes_mask[i] = 1
 
     do_graph = graph[..., ~do_nodes_mask, :][..., :, ~do_nodes_mask]
     submatrix = graph[..., do_nodes_mask, :][..., :, ~do_nodes_mask]
```

### Comparing `causica-0.3.2/src/causica/functional_relationships/functional_relationships.py` & `causica-0.3.3/src/causica/functional_relationships/linear_functional_relationships.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,62 @@
-import abc
-from typing import Any
-
 import torch
 from tensordict import TensorDict
 
+from causica.functional_relationships.functional_relationships import FunctionalRelationships
 
-class FunctionalRelationships(abc.ABC, torch.nn.Module):
-    def __init__(self, variables: dict[str, torch.Size]) -> None:
-        """_summary_
 
+class LinearFunctionalRelationships(FunctionalRelationships):
+    """
+    A simple linear functional relationship.
+    """
+
+    def __init__(
+        self,
+        shapes: dict[str, torch.Size],
+        initial_linear_coefficient_matrix: torch.Tensor,
+        trainable: bool = False,
+    ) -> None:
+        """
         Args:
-            variables: Dict of node shapes (how many dimensions a variable has)
+            shapes: Dict of node shapes (how many dimensions a variable has)
                 Order corresponds to the order in graph(s).
+            initial_linear_coefficient_matrix: the linear coefficients [output_shape, output_shape]
+            trainable: whether the coefficient matrix should be learnable
         """
-        super().__init__()
-        self.num_nodes = len(variables)
-        self.variables = variables
-        self.output_shape = sum(variable.numel() for variable in variables.values())
-
-        self.variable_masks = {}
-        last_idx = 0
-        for name, shape in variables.items():
-            mask = torch.zeros(self.output_shape, dtype=torch.bool)
-            mask[last_idx : last_idx + shape.numel()] = True
-
-            self.variable_masks[name] = mask
-            last_idx += shape.numel()
-
-    def set_extra_state(self, state: dict[str, Any]):
-        self.num_nodes = state.pop("num_nodes")
-        self.variables = state.pop("variables")
-        self.output_shape = state.pop("output_shape")
-
-    def get_extra_state(self) -> dict[str, Any]:
-        return {
-            "num_nodes": self.num_nodes,
-            "variables": self.variables,
-            "output_shape": self.output_shape,
-        }
+        super().__init__(shapes=shapes)
 
-    @abc.abstractmethod
-    def forward(self, samples: TensorDict, graphs: torch.Tensor) -> TensorDict:
-        """Calculates the predictions of the children from parents.
+        shape = self.tensor_to_td.output_shape
+        assert initial_linear_coefficient_matrix.shape == (shape, shape)
+        self.linear_coefficients = torch.nn.Parameter(initial_linear_coefficient_matrix, requires_grad=trainable)
 
+    def forward(self, samples: TensorDict, graphs: torch.Tensor) -> TensorDict:
+        """
         Args:
-            samples: dictionary of variable samples of shape sample_shape + [node shape]
-            graphs: tensor of shape batch_shape + [nodes, nodes]
-
+            samples: Batched inputs, size batch_size_x + (processed_dim_all).
+            graphs: Weighted adjacency matrix, size batch_size_g + (n, n)
         Returns:
-            Dictionary of torch.Tensors of shape sample_shape + batch_shape + [node shape]
+            A Dict of tensors of shape batch_shape_x + batch_shape_g + (processed_dim_all)
         """
+        return self.tensor_to_td(self.linear_map(self.tensor_to_td.inv(samples), graphs))
 
+    def linear_map(self, samples: torch.Tensor, graph: torch.Tensor) -> torch.Tensor:
+        """
+        Applies the linear function to a concatenated tensor of samples.
+
+        Args:
+            samples: tensor of shape batch_shape_x + [n_cols]
+            graph: tensor of shape batch_shape_g + [n_nodes, n_nodes]
+        Returns:
+            tensor of shape batch_shape_x + batch_shape_g + [n_cols]
+        """
+        batch_shape_x = samples.shape[:-1]
+        batch_shape_g = graph.shape[:-2]
 
-def sample_dict_to_tensor(sample_dict: TensorDict, variable_masks: dict[str, torch.Tensor]) -> torch.Tensor:
-    """Converts a sample dictionary to a tensor."""
-    return torch.cat([sample_dict[name] for name in variable_masks.keys()], dim=-1)
+        masked_graph = torch.einsum("ji,...jk,kl->...il", self.stacked_key_masks, graph, self.stacked_key_masks)
 
+        graph_broad = masked_graph.expand(*(batch_shape_x + tuple([-1] * len(graph.shape))))
+        target_shape = batch_shape_x + batch_shape_g + samples.shape[-1:]
+        view_shape = batch_shape_x + (1,) * len(batch_shape_g) + samples.shape[-1:]
+        # Shape batch_shape_x + batch_shape_g + (num_nodes, out_dim_g)
+        samples_broad = samples.view(view_shape).expand(target_shape)
 
-def tensor_to_sample_dict(sample_tensor: torch.Tensor, variable_masks: dict[str, torch.Tensor]) -> TensorDict:
-    """Converts a tensor to a sample dictionary."""
-    return TensorDict(
-        {name: sample_tensor[..., mask] for name, mask in variable_masks.items()}, batch_size=sample_tensor.shape[:-1]
-    )
+        return torch.einsum("...i,...ij->...j", samples_broad, graph_broad * self.linear_coefficients)
```

### Comparing `causica-0.3.2/src/causica/functional_relationships/icgnn.py` & `causica-0.3.3/src/causica/functional_relationships/icgnn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,39 @@
 from typing import Optional, Type
 
 import torch
 from tensordict import TensorDict
 from torch import nn
 
-from causica.functional_relationships.functional_relationships import (
-    FunctionalRelationships,
-    sample_dict_to_tensor,
-    tensor_to_sample_dict,
-)
+from causica.functional_relationships.functional_relationships import FunctionalRelationships
 
 
 class ICGNN(FunctionalRelationships):
     """
     This is a `FunctionalRelationsips` that implements the ICGNN.
 
     Details can be found here: https://openreview.net/forum?id=S2pNPZM-w-f
 
     This wraps the `FGNNI` in a `TensorDict` interface.
     """
 
     def __init__(
         self,
-        variables: dict[str, torch.Size],
+        shapes: dict[str, torch.Size],
         embedding_size: Optional[int] = None,
         out_dim_g: Optional[int] = None,
         norm_layer: Optional[Type[nn.LayerNorm]] = None,
         res_connection: bool = False,
     ) -> None:
-        super().__init__(variables)
+        super().__init__(shapes=shapes)
 
-        # this needs to be a parameter so it is registered to the module
-        self.stacked_variable_masks = torch.nn.Parameter(
-            torch.stack(list(self.variable_masks.values())).float(), requires_grad=False
-        )
-
-        self.nn = FGNNI(self.stacked_variable_masks, embedding_size, out_dim_g, norm_layer, res_connection)
+        self.nn = FGNNI(self.stacked_key_masks, embedding_size, out_dim_g, norm_layer, res_connection)
 
     def forward(self, samples: TensorDict, graphs: torch.Tensor) -> TensorDict:
-        return tensor_to_sample_dict(
-            self.nn(sample_dict_to_tensor(samples, self.variable_masks), graphs), self.variable_masks
-        )
+        return self.tensor_to_td(self.nn(self.tensor_to_td.inv(samples), graphs))
 
 
 class FGNNI(nn.Module):
     """
     Defines the function f for the SEM. For each variable x_i we use
     f_i(x) = f(e_i, sum_{k in pa(i)} g(e_k, x_k)), where e_i is a learned embedding
     for node i.
```

### Comparing `causica-0.3.2/src/causica/graph/evaluation_metrics.py` & `causica-0.3.3/src/causica/graph/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/lightning/cli.py` & `causica-0.3.3/src/causica/lightning/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from pytorch_lightning.callbacks import ModelCheckpoint
 from pytorch_lightning.cli import LightningCLI
 
 
 class LightningCLIWithDefaults(LightningCLI):
     default_logger = {
-        "class_path": "pytorch_lightning.loggers.MLFlowLogger",
-        "init_args": {"run_id": os.environ.get("AZUREML_RUN_ID", None)},
+        "class_path": "causica.lightning.loggers.BufferingMlFlowLogger",
+        "init_args": {"run_id": os.environ.get("AZUREML_RUN_ID", None), "buffer_size": 2000},
     }
 
     def add_arguments_to_parser(self, parser):
         parser.add_lightning_class_args(ModelCheckpoint, "best_checkpoint_callback")
         parser.add_lightning_class_args(ModelCheckpoint, "last_checkpoint_callback")
         parser.link_arguments("best_checkpoint_callback.dirpath", "last_checkpoint_callback.dirpath")
```

### Comparing `causica-0.3.2/src/causica/lightning/data_modules/basic_data_module.py` & `causica-0.3.3/src/causica/lightning/data_modules/basic_data_module.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/lightning/data_modules/deci_data_module.py` & `causica-0.3.3/src/causica/lightning/data_modules/deci_data_module.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/lightning/data_modules/variable_spec_data.py` & `causica-0.3.3/src/causica/lightning/data_modules/variable_spec_data.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/lightning/main.py` & `causica-0.3.3/src/causica/lightning/main.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/lightning/modules/deci_module.py` & `causica-0.3.3/src/causica/lightning/modules/deci_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,35 +14,34 @@
     AdjacencyDistribution,
     ConstrainedAdjacency,
     DistributionModule,
     ENCOAdjacencyDistributionModule,
     ExpertGraphContainer,
     GibbsDAGPrior,
     JointNoiseModule,
-    SEMDistributionModule,
     create_noise_modules,
 )
 from causica.distributions.noise.joint import ContinuousNoiseDist
 from causica.fsspec_helpers import get_storage_options_for_path
 from causica.functional_relationships import ICGNN
 from causica.graph.dag_constraint import calculate_dagness
 from causica.graph.evaluation_metrics import adjacency_f1, orientation_f1
 from causica.lightning.callbacks import AuglagLRCallback
 from causica.lightning.data_modules.deci_data_module import DECIDataModule
 from causica.lightning.modules.variable_spec_module import VariableSpecModule
+from causica.sem.sem_distribution import SEMDistributionModule
 from causica.sem.structural_equation_model import SEM
 from causica.training.auglag import AugLagLossCalculator, AugLagLR, AugLagLRConfig
 from causica.training.evaluation import (
     eval_ate_rmse,
     eval_intervention_likelihoods,
     eval_ite_rmse,
     list_logsumexp,
     list_mean,
 )
-from causica.training.training_callbacks import AverageMetricTracker
 
 logging.basicConfig(level=logging.INFO)
 
 NUM_GRAPH_SAMPLES = 100
 NUM_ATE_ITE_SEMS = 10
 
 
@@ -128,15 +127,15 @@
                 self.variable_types = datamodule.variable_types
             if self.variable_names is None:
                 self.variable_names = datamodule.column_names
 
     def setup(self, stage: Optional[str] = None):
         if self.is_setup:
             return  # Already setup
-        elif stage not in {TrainerFn.TESTING, TrainerFn.FITTING}:
+        if stage not in {TrainerFn.TESTING, TrainerFn.FITTING}:
             raise ValueError(f"Model can only be setup during the {TrainerFn.FITTING} and {TrainerFn.TESTING} stages.")
 
         self.infer_missing_state_from_dataset()
         assert self.dataset_name is not None
         assert self.num_samples is not None
         assert self.variable_group_shapes is not None
         assert self.variable_types is not None
@@ -146,15 +145,15 @@
         num_nodes = len(self.variable_group_shapes)
 
         adjacency_dist: DistributionModule[AdjacencyDistribution] = ENCOAdjacencyDistributionModule(num_nodes)
         if self.constraint_matrix is not None:
             adjacency_dist = ConstrainedAdjacency(adjacency_dist, self.constraint_matrix)
 
         icgnn = ICGNN(
-            variables=self.variable_group_shapes,
+            shapes=self.variable_group_shapes,
             embedding_size=self.embedding_size,
             out_dim_g=self.out_dim_g,
             norm_layer=None if self.norm_layer is False else torch.nn.LayerNorm,
             res_connection=self.res_connection,
         )
         noise_submodules = create_noise_modules(self.variable_group_shapes, self.variable_types, self.noise_dist)
         noise_module = JointNoiseModule(noise_submodules)
@@ -163,38 +162,34 @@
             init_alpha=self.init_alpha, init_rho=self.init_rho
         )
         self.prior: GibbsDAGPrior = GibbsDAGPrior(
             num_nodes=num_nodes,
             sparsity_lambda=self.prior_sparsity_lambda,
             expert_graph_container=self.expert_graph_container,
         )
-        # TODO: Set a more reasonable averaging period
-        self.average_batch_log_prob_tracker: AverageMetricTracker = AverageMetricTracker(averaging_period=10)
         self.is_setup = True
 
     def training_step(self, *args, **kwargs) -> STEP_OUTPUT:
         _ = kwargs
         batch, *_ = args
-        batch = batch.apply(lambda t: t.to(torch.float32))
+        batch = batch.apply(lambda t: t.to(torch.float32, non_blocking=True))
 
         sem_distribution = self.sem_module()
         sem, *_ = sem_distribution.relaxed_sample(torch.Size([]), temperature=self.gumbel_temp)  # soft sample
 
         batch_log_prob = sem.log_prob(batch).mean()
         sem_distribution_entropy = sem_distribution.entropy()
         prior_term = self.prior.log_prob(sem.graph)
         objective = (-sem_distribution_entropy - prior_term) / self.num_samples - batch_log_prob
         constraint = calculate_dagness(sem.graph)
-        self.average_batch_log_prob_tracker.step(batch_log_prob.item())
         step_output = {
             "loss": self.auglag_loss(objective, constraint / self.num_samples),
             "batch_log_prob": batch_log_prob,
             "constraint": constraint,
             "num_edges": (sem.graph > 0.0).count_nonzero(),
-            "average_batch_log_prob": self.average_batch_log_prob_tracker.average,
             "vardist_entropy": sem_distribution_entropy,
             "prior_term": prior_term,
         }
         self.log_dict({"alpha": self.auglag_loss.alpha, "rho": self.auglag_loss.rho, **step_output}, prog_bar=True)
         return step_output
 
     def configure_optimizers(self):
@@ -214,19 +209,20 @@
         for module in self.parameters(recurse=False):
             assert module in check_modules, f"Module {module} not in module list"
 
         return torch.optim.Adam(parameter_list)
 
     def configure_callbacks(self) -> Union[Sequence[pl.Callback], pl.Callback]:
         """Create a callback for the auglag callback."""
-        return [AuglagLRCallback(AugLagLR(config=self.auglag_config))]
+        lr_scheduler = AugLagLR(config=self.auglag_config)
+        return [AuglagLRCallback(lr_scheduler, log_auglag=True)]
 
     def test_step_observational(self, batch: TensorDict, *args, **kwargs):
         """Evaluate the log prob of the model on the test set using multiple graph samples."""
-        batch = batch.apply(lambda t: t.to(torch.float32))
+        batch = batch.apply(lambda t: t.to(torch.float32, non_blocking=True))
         sems = self.sem_module().sample(torch.Size([NUM_GRAPH_SAMPLES]))
         dataset_size = self.trainer.datamodule.dataset_test.batch_size  # type: ignore
         assert len(dataset_size) == 1, "Only one batch size is supported"
         # estimate log prob for each sample using graph samples and report the mean over graphs
         log_prob_test = list_logsumexp([sem.log_prob(batch) for sem in sems]) - np.log(NUM_GRAPH_SAMPLES)
         self.log(
             "eval/test_LL",
```

### Comparing `causica-0.3.2/src/causica/lightning/modules/variable_spec_module.py` & `causica-0.3.3/src/causica/lightning/modules/variable_spec_module.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,22 +26,23 @@
         Test data
         Graph data
         Intervention data
         Counterfactual data
 
         See the superclass for *args and **kwargs conventions.
         """
-        if dataloader_idx == 0:
-            return self.test_step_observational(batch, batch_idx)
-        elif dataloader_idx == 1:
-            return self.test_step_graph(batch, batch_idx)
-        elif dataloader_idx == 2:
-            return self.test_step_interventions(batch, batch_idx)
-        elif dataloader_idx == 3:
-            return self.test_step_counterfactuals(batch, batch_idx)
+        match dataloader_idx:
+            case 0:
+                return self.test_step_observational(batch, batch_idx)
+            case 1:
+                return self.test_step_graph(batch, batch_idx)
+            case 2:
+                return self.test_step_interventions(batch, batch_idx)
+            case 3:
+                return self.test_step_counterfactuals(batch, batch_idx)
 
     @abc.abstractmethod
     def test_step_observational(self, batch: TensorDict, *args, **kwargs):
         """Test step method for the test data."""
 
     @abc.abstractmethod
     def test_step_graph(self, true_adj_matrix: torch.Tensor, *args, **kwargs):
```

### Comparing `causica-0.3.2/src/causica/mlflow_helpers.py` & `causica-0.3.3/src/causica/mlflow_helpers.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/sem/distribution_parameters_sem.py` & `causica-0.3.3/src/causica/sem/distribution_parameters_sem.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/sem/structural_equation_model.py` & `causica-0.3.3/src/causica/sem/structural_equation_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 
 import torch
 import torch.distributions as dist
 from tensordict import TensorDict
 
 
 class SEM(dist.Distribution, abc.ABC):
+    """A structural equation model (SEM).
+
+    An SEM defines the causal relationships amongst a given set of nodes. This class provides methods to sample data
+    from the observational and interventional distributions of the SEM.
+    """
+
     arg_constraints: dict = {}
 
     def __init__(
         self,
         graph: torch.Tensor,
         node_names: Sequence[str],
         event_shape: torch.Size = torch.Size(),
@@ -133,16 +139,14 @@
     Args:
         factual_data: Factual data to abduct the noise from.
         intervention: Specification of intervention.
 
     Returns:
        TensorDict: Dictionary holding the counterfactual values for all samples.
     """
-    # TODO: do we want to average over multiple "sample_to_noise" values for the discrete variables
-    # where this is not a 1:1 mapping?
     return sem.do(interventions=intervention).noise_to_sample(sem.sample_to_noise(factual_data))
 
 
 def ate(
     sem: SEM,
     intervention_a: TensorDict,
     intervention_b: TensorDict,
```

### Comparing `causica-0.3.2/src/causica/training/auglag.py` & `causica-0.3.3/src/causica/training/auglag.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from collections import deque
 from dataclasses import dataclass, field
-from typing import Union
+from typing import Optional, Union
 
-import numpy as np
 import torch
 from dataclasses_json import dataclass_json
 from torch.optim import Optimizer
 
 
-class AugLagLossCalculator:
+class AugLagLossCalculator(torch.nn.Module):
     def __init__(self, init_alpha: float, init_rho: float):
-        self.alpha = init_alpha
-        self.rho = init_rho
+        super().__init__()
+        self.alpha: torch.Tensor
+        self.rho: torch.Tensor
+        self.register_buffer("alpha", torch.tensor(init_alpha, dtype=torch.float))
+        self.register_buffer("rho", torch.tensor(init_rho, dtype=torch.float))
 
-    def __call__(self, objective: torch.Tensor, constraint: torch.Tensor) -> torch.Tensor:
+    def forward(self, objective: torch.Tensor, constraint: torch.Tensor) -> torch.Tensor:
         return objective + self.alpha * constraint + self.rho * constraint * constraint / 2
 
 
 @dataclass_json
 @dataclass(frozen=True)
 class AugLagLRConfig:
     """
@@ -71,34 +73,29 @@
             config: An `AugLagLRConfig` object containing the configuration parameters.
         """
         self.config = config
 
         self.outer_opt_counter = 0
         self.outer_below_penalty_tol = 0
         self.outer_max_rho = 0
-        self._prev_lagrangian_penalty = np.inf
-        self._cur_lagrangian_penalty = np.inf
+        self._prev_lagrangian_penalty = torch.tensor(torch.inf)
+        self._cur_lagrangian_penalty = torch.tensor(torch.inf)
 
-        self.best_loss = np.inf
-        self.last_lr_update_step = 0
-        self.num_lr_updates = 0
-        self.last_best_step = 0
-        self.loss_tracker: deque = deque([], maxlen=config.aggregation_period)
-        self.step_counter = 0
-        self.epoch_counter = 0
+        self.loss_tracker: deque[torch.Tensor] = deque([], maxlen=config.aggregation_period)
+        self._init_new_inner_optimisation()
 
-    def _init_new_inner_optimisation(self):
+    def _init_new_inner_optimisation(self) -> None:
         """Init the hyperparameters for a new inner loop optimization."""
-        self.best_loss = np.inf
+        self.best_loss = torch.tensor(torch.inf)
         self.last_lr_update_step = 0
         self.num_lr_updates = 0
         self.last_best_step = 0
         self.loss_tracker.clear()
+        self.loss_tracker_sum: Optional[torch.Tensor] = None
         self.step_counter = 0
-        self.epoch_counter = 0
 
     def _is_inner_converged(self) -> bool:
         """Check if the inner optimization loop has converged, based on maximum number of inner steps, number of lr updates.
 
         Returns:
             bool: Return True if converged, else False.
         """
@@ -152,15 +149,15 @@
             for opt in optimizer:
                 for param_group in opt.param_groups:
                     param_group["lr"] *= self.config.lr_factor
         else:
             for param_group in optimizer.param_groups:
                 param_group["lr"] *= self.config.lr_factor
 
-    def _reset_lr(self, optimizer: Union[Optimizer, list[Optimizer]]):
+    def reset_lr(self, optimizer: Union[Optimizer, list[Optimizer]]):
         """Reset the learning rate of individual param groups from lr init dictionary.
 
         Args:
             optimizer: Optimizer(s) corresponding to all param groups.
         """
         self.last_lr_update_step = self.step_counter
 
@@ -175,36 +172,37 @@
 
     def _update_lagrangian_params(self, loss: AugLagLossCalculator):
         """Update the lagrangian parameters (of the auglag routine) based on the dag constraint values observed.
 
         Args:
             loss: loss with lagrangian attributes rho and alpha to be updated.
         """
-        if self._cur_dag_penalty < self.config.penalty_tolerance:
+        if self._cur_lagrangian_penalty < self.config.penalty_tolerance:
             self.outer_below_penalty_tol += 1
         else:
             self.outer_below_penalty_tol = 0
 
         if loss.rho > self.config.safety_rho:
             self.outer_max_rho += 1
 
-        if self._cur_dag_penalty > self._prev_lagrangian_penalty * self.config.penalty_progress_rate:
+        if self._cur_lagrangian_penalty > self._prev_lagrangian_penalty * self.config.penalty_progress_rate:
             print(f"Updating rho, dag penalty prev: {self._prev_lagrangian_penalty: .10f}")
             loss.rho *= 10.0
         else:
-            self._prev_lagrangian_penalty = self._cur_dag_penalty
-            loss.alpha += loss.rho * self._cur_dag_penalty
-            if self._cur_dag_penalty == 0.0:
+            self._prev_lagrangian_penalty = self._cur_lagrangian_penalty
+            loss.alpha += loss.rho * self._cur_lagrangian_penalty
+            if self._cur_lagrangian_penalty == 0.0:
                 loss.alpha *= 5
             print(f"Updating alpha to: {loss.alpha}")
         if loss.rho >= self.config.safety_rho:
             loss.alpha *= 5
 
-        loss.rho = min([loss.rho, self.config.safety_rho])
-        loss.alpha = min([loss.alpha, self.config.safety_alpha])
+        # Update parameters and make sure to maintain the dtype and device
+        loss.alpha = torch.min(loss.alpha, torch.full_like(loss.alpha, self.config.safety_alpha))
+        loss.rho = torch.min(loss.rho, torch.full_like(loss.rho, self.config.safety_rho))
 
     def _is_auglag_converged(self, optimizer: Union[Optimizer, list[Optimizer]], loss: AugLagLossCalculator) -> bool:
         """Checks if the inner and outer loops have converged. If inner loop is converged,
         it initilaizes the optimisation parameters for a new inner loop. If both are converged, it returns True.
 
         Args:
             optimizer: Optimizer(s) corresponding to different parameter groups on which auglag is being performed.
@@ -212,49 +210,63 @@
 
         Returns:
             bool: Returns True if both inner and outer have converged, else False
         """
         if self._is_inner_converged():
             if self._is_outer_converged():
                 return True
-            else:
-                self._update_lagrangian_params(loss)
-                self.outer_opt_counter += 1
-                self._init_new_inner_optimisation()
-                self._reset_lr(optimizer)
+
+            self._update_lagrangian_params(loss)
+            self.outer_opt_counter += 1
+            self._init_new_inner_optimisation()
+            self.reset_lr(optimizer)
         elif self._enough_steps_since_last_lr_update() and self._enough_steps_since_best_model():
             self._update_lr(optimizer)
 
         return False
 
+    def _update_loss_tracker(self, loss_value: torch.Tensor):
+        """Update the loss tracker with the current loss value.
+
+        Args:
+            loss_value: The current loss value.
+        """
+        if self.loss_tracker_sum is None:
+            self.loss_tracker_sum = torch.zeros_like(loss_value)
+
+        if len(self.loss_tracker) == self.loss_tracker.maxlen:
+            self.loss_tracker_sum -= self.loss_tracker.popleft()
+        self.loss_tracker.append(loss_value)
+        self.loss_tracker_sum += loss_value
+
     def _check_best_loss(self):
         """Update the best loss based on the average loss over an aggregation period."""
-        if len(self.loss_tracker) == self.config.aggregation_period:
-            avg_loss = np.mean(self.loss_tracker)
+        if len(self.loss_tracker) == self.loss_tracker.maxlen and self.loss_tracker_sum is not None:
+            avg_loss = self.loss_tracker_sum / self.loss_tracker.maxlen
             if avg_loss < self.best_loss:
                 self.best_loss = avg_loss
                 self.last_best_step = self.step_counter
 
     def step(
         self,
         optimizer: Union[Optimizer, list[Optimizer]],
         loss: AugLagLossCalculator,
-        loss_value: float,
-        lagrangian_penalty: float,
+        loss_value: torch.Tensor,
+        lagrangian_penalty: torch.Tensor,
     ) -> bool:
         """The main update method to take one auglag inner step.
 
         Args:
             optimizer: Optimizer(s) corresponding to different param groups.
             loss: auglag loss with lagrangian parameters
             loss_value: the actual value of the elbo for the current update step.
             lagrangian_penalty: Dag penalty for the current update step.
 
         Returns:
             bool: if the auglag has converged (False) or not (True)
         """
-        assert lagrangian_penalty >= 0, "auglag penalty must be non-negative"
-        self.loss_tracker.append(loss_value)
-        self._cur_dag_penalty = lagrangian_penalty
+        assert torch.all(lagrangian_penalty >= 0), "auglag penalty must be non-negative"
+        self._update_loss_tracker(loss_value.detach())
+        self._cur_lagrangian_penalty = lagrangian_penalty.detach()
         self.step_counter += 1
         self._check_best_loss()
         return self._is_auglag_converged(optimizer=optimizer, loss=loss)
```

### Comparing `causica-0.3.2/src/causica/training/evaluation.py` & `causica-0.3.3/src/causica/training/evaluation.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/training/per_variable_metrics.py` & `causica-0.3.3/src/causica/training/per_variable_metrics.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/src/causica/triangular_transformations.py` & `causica-0.3.3/src/causica/triangular_transformations.py`

 * *Files identical despite different names*

### Comparing `causica-0.3.2/PKG-INFO` & `causica-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causica
-Version: 0.3.2
+Version: 0.3.3
 Summary: 
 License: MIT
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: azureml-mlflow (>=1.46.0,<2.0.0)
@@ -13,15 +13,15 @@
 Requires-Dist: mlflow (>=2.0.0,<3.0.0)
 Requires-Dist: numba (>=0.56.0,<0.57.0)
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0)
 Requires-Dist: pytorch-lightning[extra] (>=1.9.0,<2.0.0)
 Requires-Dist: tensorboard (>=2.9.0,<3.0.0)
 Requires-Dist: tensordict (>=0.1.0,<0.2.0)
-Requires-Dist: torch (>=2.0.0,<3.0.0)
+Requires-Dist: torch (==2.0.0)
 Requires-Dist: types-PyYAML (>=6.0.12.2,<7.0.0.0)
 Description-Content-Type: text/markdown
 
 [![Causica CI Build](https://github.com/microsoft/causica/actions/workflows/ci-build.yml/badge.svg)](https://github.com/microsoft/causica/actions/workflows/ci-build.yml)
 
 # Causica
```

