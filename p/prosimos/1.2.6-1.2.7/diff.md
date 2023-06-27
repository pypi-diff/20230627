# Comparing `tmp/prosimos-1.2.6.tar.gz` & `tmp/prosimos-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosimos-1.2.6.tar", max compression
+gzip compressed data, was "prosimos-1.2.7.tar", max compression
```

## Comparing `prosimos-1.2.6.tar` & `prosimos-1.2.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    15559 2023-06-15 18:05:44.750312 prosimos-1.2.6/README.md
--rw-r--r--   0        0        0        0 2023-06-15 18:05:44.766312 prosimos-1.2.6/bpdfr_discovery/__init__.py
--rw-r--r--   0        0        0     3478 2023-06-15 18:05:44.766312 prosimos-1.2.6/bpdfr_discovery/emd_metric.py
--rw-r--r--   0        0        0      489 2023-06-15 18:05:44.766312 prosimos-1.2.6/bpdfr_discovery/exceptions.py
--rw-r--r--   0        0        0     7248 2023-06-15 18:05:44.766312 prosimos-1.2.6/bpdfr_discovery/inter_arrival_cases_discovery.py
--rw-r--r--   0        0        0     5615 2023-06-15 18:05:44.766312 prosimos-1.2.6/bpdfr_discovery/log_comparison_metrics.py
--rw-r--r--   0        0        0    44127 2023-06-15 18:05:44.766312 prosimos-1.2.6/bpdfr_discovery/log_parser.py
--rw-r--r--   0        0        0        0 2023-06-15 18:05:44.766312 prosimos-1.2.6/cli/__init__.py
--rw-r--r--   0        0        0     3539 2023-06-15 18:05:44.766312 prosimos-1.2.6/cli/diff_res_bpsim.py
--rw-r--r--   0        0        0        0 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/__init__.py
--rw-r--r--   0        0        0    44604 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/batch_processing.py
--rw-r--r--   0        0        0     4401 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/batch_processing_parser.py
--rw-r--r--   0        0        0     2409 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/case_attributes.py
--rw-r--r--   0        0        0    48417 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/control_flow_manager.py
--rw-r--r--   0        0        0      623 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/exceptions.py
--rw-r--r--   0        0        0     7340 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/execution_info.py
--rw-r--r--   0        0        0     1109 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/file_manager.py
--rw-r--r--   0        0        0      555 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/histogram_distribution.py
--rw-r--r--   0        0        0     3147 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/prioritisation.py
--rw-r--r--   0        0        0     1345 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/prioritisation_parser.py
--rw-r--r--   0        0        0     3009 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/prioritisation_rules.py
--rw-r--r--   0        0        0     6974 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/probability_distributions.py
--rw-r--r--   0        0        0      467 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/resource_profile.py
--rw-r--r--   0        0        0    29277 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/simulation_engine.py
--rw-r--r--   0        0        0    21739 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/simulation_properties_parser.py
--rw-r--r--   0        0        0     6298 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/simulation_queues_ds.py
--rw-r--r--   0        0        0     6584 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/simulation_setup.py
--rw-r--r--   0        0        0    15565 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/simulation_stats.py
--rw-r--r--   0        0        0    14171 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/simulation_stats_calculator.py
--rw-r--r--   0        0        0     1730 2023-06-15 18:05:44.870312 prosimos-1.2.6/prosimos/weekday_helper.py
--rw-r--r--   0        0        0      668 2023-06-15 18:05:44.870312 prosimos-1.2.6/pyproject.toml
--rw-r--r--   0        0        0    16305 1970-01-01 00:00:00.000000 prosimos-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0    15559 2023-06-27 12:32:18.241897 prosimos-1.2.7/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 12:32:18.257897 prosimos-1.2.7/bpdfr_discovery/__init__.py
+-rw-r--r--   0        0        0     3478 2023-06-27 12:32:18.257897 prosimos-1.2.7/bpdfr_discovery/emd_metric.py
+-rw-r--r--   0        0        0      489 2023-06-27 12:32:18.257897 prosimos-1.2.7/bpdfr_discovery/exceptions.py
+-rw-r--r--   0        0        0     7248 2023-06-27 12:32:18.257897 prosimos-1.2.7/bpdfr_discovery/inter_arrival_cases_discovery.py
+-rw-r--r--   0        0        0     5615 2023-06-27 12:32:18.257897 prosimos-1.2.7/bpdfr_discovery/log_comparison_metrics.py
+-rw-r--r--   0        0        0    44127 2023-06-27 12:32:18.257897 prosimos-1.2.7/bpdfr_discovery/log_parser.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:32:18.257897 prosimos-1.2.7/cli/__init__.py
+-rw-r--r--   0        0        0     3539 2023-06-27 12:32:18.257897 prosimos-1.2.7/cli/diff_res_bpsim.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/__init__.py
+-rw-r--r--   0        0        0    44604 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/batch_processing.py
+-rw-r--r--   0        0        0     4401 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/batch_processing_parser.py
+-rw-r--r--   0        0        0     2409 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/case_attributes.py
+-rw-r--r--   0        0        0    48417 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/control_flow_manager.py
+-rw-r--r--   0        0        0      623 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/exceptions.py
+-rw-r--r--   0        0        0     7340 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/execution_info.py
+-rw-r--r--   0        0        0     1109 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/file_manager.py
+-rw-r--r--   0        0        0      555 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/histogram_distribution.py
+-rw-r--r--   0        0        0     3147 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/prioritisation.py
+-rw-r--r--   0        0        0     1345 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/prioritisation_parser.py
+-rw-r--r--   0        0        0     3009 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/prioritisation_rules.py
+-rw-r--r--   0        0        0     7010 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/probability_distributions.py
+-rw-r--r--   0        0        0      467 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/resource_profile.py
+-rw-r--r--   0        0        0    29277 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/simulation_engine.py
+-rw-r--r--   0        0        0    21739 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/simulation_properties_parser.py
+-rw-r--r--   0        0        0     6298 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/simulation_queues_ds.py
+-rw-r--r--   0        0        0     6584 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/simulation_setup.py
+-rw-r--r--   0        0        0    15565 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/simulation_stats.py
+-rw-r--r--   0        0        0    14171 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/simulation_stats_calculator.py
+-rw-r--r--   0        0        0     1730 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/weekday_helper.py
+-rw-r--r--   0        0        0      669 2023-06-27 12:32:18.361896 prosimos-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0    16306 1970-01-01 00:00:00.000000 prosimos-1.2.7/PKG-INFO
```

### Comparing `prosimos-1.2.6/README.md` & `prosimos-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/bpdfr_discovery/emd_metric.py` & `prosimos-1.2.7/bpdfr_discovery/emd_metric.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/bpdfr_discovery/inter_arrival_cases_discovery.py` & `prosimos-1.2.7/bpdfr_discovery/inter_arrival_cases_discovery.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/bpdfr_discovery/log_comparison_metrics.py` & `prosimos-1.2.7/bpdfr_discovery/log_comparison_metrics.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/bpdfr_discovery/log_parser.py` & `prosimos-1.2.7/bpdfr_discovery/log_parser.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/cli/diff_res_bpsim.py` & `prosimos-1.2.7/cli/diff_res_bpsim.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/prosimos/batch_processing.py` & `prosimos-1.2.7/prosimos/batch_processing.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/prosimos/batch_processing_parser.py` & `prosimos-1.2.7/prosimos/batch_processing_parser.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/prosimos/case_attributes.py` & `prosimos-1.2.7/prosimos/case_attributes.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/prosimos/control_flow_manager.py` & `prosimos-1.2.7/prosimos/control_flow_manager.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/prosimos/exceptions.py` & `prosimos-1.2.7/prosimos/exceptions.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/prosimos/execution_info.py` & `prosimos-1.2.7/prosimos/execution_info.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/prosimos/file_manager.py` & `prosimos-1.2.7/prosimos/file_manager.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/prosimos/histogram_distribution.py` & `prosimos-1.2.7/prosimos/histogram_distribution.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/prosimos/prioritisation.py` & `prosimos-1.2.7/prosimos/prioritisation.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/prosimos/prioritisation_parser.py` & `prosimos-1.2.7/prosimos/prioritisation_parser.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/prosimos/prioritisation_rules.py` & `prosimos-1.2.7/prosimos/prioritisation_rules.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/prosimos/probability_distributions.py` & `prosimos-1.2.7/prosimos/probability_distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,34 +33,34 @@
     x = (x + np.roll(x, -1))[:-1] / 2.0
 
     distributions = [
         st.norm, st.expon, st.exponnorm, st.gamma, st.triang, st.uniform, st.lognorm
     ]
 
     # Discrete distributions
-    disc_distributions = [
-        st.bernoulli, st.betabinom, st.binom, st.boltzmann, st.planck, st.poisson, st.geom, st.nbinom, st.hypergeom,
-        st.nchypergeom_fisher, st.nchypergeom_wallenius, st.nhypergeom, st.zipf, st.zipfian, st.logser, st.randint,
-        st.dlaplace, st.yulesimon, st.norm, st.expon, st.exponnorm, st.gamma, st.triang, st.lognorm, st.uniform
-    ]
+    # disc_distributions = [
+    #     st.bernoulli, st.betabinom, st.binom, st.boltzmann, st.planck, st.poisson, st.geom, st.nbinom, st.hypergeom,
+    #     st.nchypergeom_fisher, st.nchypergeom_wallenius, st.nhypergeom, st.zipf, st.zipfian, st.logser, st.randint,
+    #     st.dlaplace, st.yulesimon, st.norm, st.expon, st.exponnorm, st.gamma, st.triang, st.lognorm, st.uniform
+    # ]
 
     # Distributions to check
-    all_distributions = [
-        st.alpha, st.anglit, st.arcsine, st.beta, st.betaprime, st.bradford, st.burr, st.cauchy, st.chi, st.chi2,
-        st.cosine, st.dgamma, st.dweibull, st.erlang, st.expon, st.exponnorm, st.exponweib, st.exponpow, st.f,
-        st.fatiguelife, st.fisk, st.foldcauchy, st.foldnorm, st.genlogistic, st.genpareto,
-        st.gennorm, st.gausshyper, st.gamma, st.gengamma, st.genhalflogistic, st.gilbrat, st.gompertz,
-        st.gumbel_r, st.gumbel_l, st.halfcauchy, st.halflogistic, st.halfnorm, st.halfgennorm, st.hypsecant,
-        st.invgamma, st.invgauss, st.invweibull, st.johnsonsb, st.johnsonsu, st.ksone, st.kstwobign, st.laplace,
-        st.levy, st.levy_l, st.logistic, st.loggamma, st.loglaplace, st.lognorm, st.lomax, st.maxwell, st.mielke,
-        st.nakagami, st.ncx2, st.ncf, st.nct, st.norm, st.pareto, st.pearson3, st.powerlaw, st.powerlognorm,
-        st.powernorm, st.rdist, st.reciprocal, st.rayleigh, st.rice, st.semicircular, st.t, st.triang, st.truncexpon,
-        st.truncnorm, st.tukeylambda, st.uniform, st.vonmises, st.vonmises_line, st.wald, st.weibull_min,
-        st.weibull_max, st.wrapcauchy
-    ]
+    # all_distributions = [
+    #     st.alpha, st.anglit, st.arcsine, st.beta, st.betaprime, st.bradford, st.burr, st.cauchy, st.chi, st.chi2,
+    #     st.cosine, st.dgamma, st.dweibull, st.erlang, st.expon, st.exponnorm, st.exponweib, st.exponpow, st.f,
+    #     st.fatiguelife, st.fisk, st.foldcauchy, st.foldnorm, st.genlogistic, st.genpareto,
+    #     st.gennorm, st.gausshyper, st.gamma, st.gengamma, st.genhalflogistic, st.gilbrat, st.gompertz,
+    #     st.gumbel_r, st.gumbel_l, st.halfcauchy, st.halflogistic, st.halfnorm, st.halfgennorm, st.hypsecant,
+    #     st.invgamma, st.invgauss, st.invweibull, st.johnsonsb, st.johnsonsu, st.ksone, st.kstwobign, st.laplace,
+    #     st.levy, st.levy_l, st.logistic, st.loggamma, st.loglaplace, st.lognorm, st.lomax, st.maxwell, st.mielke,
+    #     st.nakagami, st.ncx2, st.ncf, st.nct, st.norm, st.pareto, st.pearson3, st.powerlaw, st.powerlognorm,
+    #     st.powernorm, st.rdist, st.reciprocal, st.rayleigh, st.rice, st.semicircular, st.t, st.triang, st.truncexpon,
+    #     st.truncnorm, st.tukeylambda, st.uniform, st.vonmises, st.vonmises_line, st.wald, st.weibull_min,
+    #     st.weibull_max, st.wrapcauchy
+    # ]
 
     # Best holders
     best_distribution = st.norm
     best_params = (0.0, 1.0)
     best_sse = np.inf
 
     # Estimate distribution parameters from data
```

### Comparing `prosimos-1.2.6/prosimos/simulation_engine.py` & `prosimos-1.2.7/prosimos/simulation_engine.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/prosimos/simulation_properties_parser.py` & `prosimos-1.2.7/prosimos/simulation_properties_parser.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/prosimos/simulation_queues_ds.py` & `prosimos-1.2.7/prosimos/simulation_queues_ds.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/prosimos/simulation_setup.py` & `prosimos-1.2.7/prosimos/simulation_setup.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/prosimos/simulation_stats.py` & `prosimos-1.2.7/prosimos/simulation_stats.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/prosimos/simulation_stats_calculator.py` & `prosimos-1.2.7/prosimos/simulation_stats_calculator.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/prosimos/weekday_helper.py` & `prosimos-1.2.7/prosimos/weekday_helper.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.6/pyproject.toml` & `prosimos-1.2.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prosimos"
-version = "1.2.6"
+version = "1.2.7"
 description = ""
 authors = ["Iryna Halenok, Orlenys López Pintado"]
 readme = "README.md"
 packages = [
     {include = "cli"},
     {include = "prosimos"},
     {include = "bpdfr_discovery"}
@@ -15,15 +15,15 @@
 click = "^8.1.3"
 numpy = "^1.24.3"
 pandas = "^2.0.1"
 python-dateutil = "^2.8.2"
 pytz = "^2023.3"
 scipy = "^1.10.1"
 pm4py = "^2.7.4"
-pix-framework = "^0.9.0"
+pix-framework = "^0.10.0"
 pylint = "^2.17.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 
 [tool.poetry.scripts]
 prosimos = "cli.diff_res_bpsim:cli"
```

### Comparing `prosimos-1.2.6/PKG-INFO` & `prosimos-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: prosimos
-Version: 1.2.6
+Version: 1.2.7
 Summary: 
 Author: Iryna Halenok, Orlenys López Pintado
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
-Requires-Dist: pix-framework (>=0.9.0,<0.10.0)
+Requires-Dist: pix-framework (>=0.10.0,<0.11.0)
 Requires-Dist: pm4py (>=2.7.4,<3.0.0)
 Requires-Dist: pylint (>=2.17.4,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Description-Content-Type: text/markdown
```

