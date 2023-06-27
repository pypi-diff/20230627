# Comparing `tmp/gpflow-2.8.0.tar.gz` & `tmp/gpflow-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gpflow-2.8.0.tar", last modified: Thu May  4 08:51:21 2023, max compression
+gzip compressed data, was "dist/gpflow-2.8.1.tar", last modified: Tue Jun 27 14:04:20 2023, max compression
```

## Comparing `gpflow-2.8.0.tar` & `gpflow-2.8.1.tar`

### file list

```diff
@@ -1,262 +1,262 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-05-04 08:51:07.000000 gpflow-2.8.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2023-05-04 08:51:07.000000 gpflow-2.8.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12653 2023-05-04 08:51:21.000000 gpflow-2.8.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11316 2023-05-04 08:51:07.000000 gpflow-2.8.0/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21377 2023-05-04 08:51:07.000000 gpflow-2.8.0/RELEASE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-05-04 08:51:07.000000 gpflow-2.8.0/VERSION
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/benchmark/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9767 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/benchmark_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3524 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/benchmarks.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10736 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/dataset_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4590 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/datasets.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8301 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6597 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/metadata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1652 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/metric_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3286 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/metrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3137 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/model_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2921 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/models.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/paths.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6093 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/plot.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2792 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/plotter_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4478 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/plotters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2438 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/run.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3496 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/sharding.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4781 2023-05-04 08:51:07.000000 gpflow-2.8.0/benchmark/tag.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/doc/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/doc/sphinx/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      398 2023-05-04 08:51:07.000000 gpflow-2.8.0/doc/sphinx/benchmarks.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2023-05-04 08:51:07.000000 gpflow-2.8.0/doc/sphinx/bibliography.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3109 2023-05-04 08:51:07.000000 gpflow-2.8.0/doc/sphinx/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1473 2023-05-04 08:51:07.000000 gpflow-2.8.0/doc/sphinx/getting_started.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7585 2023-05-04 08:51:07.000000 gpflow-2.8.0/doc/sphinx/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2468 2023-05-04 08:51:07.000000 gpflow-2.8.0/doc/sphinx/installation.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4444 2023-05-04 08:51:07.000000 gpflow-2.8.0/doc/sphinx/user_guide.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1745 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13183 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1772 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/ci_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/conditionals/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      445 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/conditionals/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5399 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/conditionals/conditionals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1293 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/conditionals/dispatch.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/conditionals/multioutput/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      110 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/conditionals/multioutput/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11061 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/conditionals/multioutput/conditionals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3007 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/conditionals/multioutput/sample_conditionals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3281 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/conditionals/sample_conditionals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6231 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/conditionals/uncertain_conditionals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23736 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/conditionals/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12677 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/config/__config__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      618 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/config/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/covariances/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/covariances/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      695 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/covariances/dispatch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2665 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/covariances/kufs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2370 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/covariances/kuus.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/covariances/multioutput/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/covariances/multioutput/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6858 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/covariances/multioutput/kufs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4048 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/covariances/multioutput/kuus.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/expectations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      454 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5380 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/cross_kernels.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      813 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/dispatch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5479 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/expectations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5954 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/linears.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6170 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/mean_functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7115 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/misc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4450 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/products.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6814 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/quadratures.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10043 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/squared_exponentials.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4972 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/expectations/sums.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/experimental/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      879 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/experimental/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1551 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/experimental/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10582 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/functions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/inducing_variables/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      785 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/inducing_variables/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      708 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/inducing_variables/inducing_patch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3690 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/inducing_variables/inducing_variables.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/inducing_variables/multioutput/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/inducing_variables/multioutput/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7262 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/inducing_variables/multioutput/inducing_variables.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/kernels/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2532 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10659 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5135 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/categorical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6817 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/changepoints.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6351 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/convolutional.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3844 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/linears.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11102 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/misc.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/kernels/multioutput/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/multioutput/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15660 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/multioutput/kernels.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4042 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/periodic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2823 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/statics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11179 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kernels/stationaries.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5901 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/kullback_leiblers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/likelihoods/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3720 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/likelihoods/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24692 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/likelihoods/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      869 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/likelihoods/misc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9162 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/likelihoods/multiclass.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4782 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/likelihoods/multilatent.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11574 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/likelihoods/scalar_continuous.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7553 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/likelihoods/scalar_discrete.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      948 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/likelihoods/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4530 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/logdensities.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/mean_functions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1909 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14250 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/cglb.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11614 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/gplvm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4451 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/gpmc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7000 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/gpr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13688 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4718 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/sgpmc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22082 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/sgpr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10487 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/svgp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5794 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/training_mixins.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3692 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15454 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/models/vgp.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/monitor/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      915 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/monitor/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5300 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/monitor/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8983 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/monitor/tensorboard.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      839 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/mypy_flags.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/optimizers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      269 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/optimizers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5294 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/optimizers/mcmc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18062 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/optimizers/natgrad.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9750 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/optimizers/scipy.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    40522 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/posteriors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3005 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/probability_distributions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/py.typed
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/quadrature/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      360 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/quadrature/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4887 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/quadrature/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9494 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/quadrature/deprecated.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5590 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/quadrature/gauss_hermite.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1784 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/type_flags.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow/utilities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1217 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/utilities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2169 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/utilities/bijectors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3724 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/utilities/misc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1547 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/utilities/model_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3325 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/utilities/multipledispatch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5626 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/utilities/ops.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1736 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/utilities/parameter_or_function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13979 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/utilities/traversal.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      177 2023-05-04 08:51:07.000000 gpflow-2.8.0/gpflow/versions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12653 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7281 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      354 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2023-05-04 08:51:21.000000 gpflow-2.8.0/gpflow.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-04 08:51:21.000000 gpflow-2.8.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2592 2023-05-04 08:51:07.000000 gpflow-2.8.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/conditionals/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/conditionals/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7895 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/conditionals/test_broadcasted_conditionals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6959 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/conditionals/test_conditionals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32563 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/conditionals/test_multioutput.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10722 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/conditionals/test_uncertain_conditional.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4537 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/conditionals/test_util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/config/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6991 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/config/test_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1278 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/conftest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/covariances/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/covariances/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4244 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/covariances/test_base_covariances.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4968 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/covariances/test_multioutput.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/expectations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/expectations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12096 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/expectations/test_expectations.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/experimental/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/experimental/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      954 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/experimental/test_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/kernels/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/kernels/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3473 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/kernels/reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9302 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/kernels/test_broadcasting.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      475 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/kernels/test_changepoints.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7805 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/kernels/test_coregion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23223 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/kernels/test_kernels.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2071 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/kernels/test_positive_semidefinite.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1940 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/kernels/test_scaled_euclid_dist.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/likelihoods/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/likelihoods/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7752 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/likelihoods/test_function_params.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1688 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/likelihoods/test_heteroskedastic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5586 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/likelihoods/test_heteroskedastic_constant_variance.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11288 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/likelihoods/test_likelihoods.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8112 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/likelihoods/test_multiclass.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7141 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/likelihoods/test_switched_likelihood.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6499 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_cglb.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3806 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_gplvm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2220 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_gpr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2496 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_gpr_posterior.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1814 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_mcmc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3160 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_methods.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7970 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_model_predict.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2662 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_sgpr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4189 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_sgpr_posterior.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6777 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_svgp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3056 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_svgp_posterior.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1042 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_training_mixins.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8714 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_variational.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1991 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_vgp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2997 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/models/test_vgp_posterior.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/optimizers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/optimizers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7811 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/optimizers/test_mcmc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6341 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/optimizers/test_natural_gradient.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7186 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/optimizers/test_scipy.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/posteriors/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/posteriors/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2280 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/posteriors/conftest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13721 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/posteriors/test_bo_integration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27405 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/posteriors/test_posteriors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3877 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_all.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9354 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4993 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_base_prior.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4057 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_base_training.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13060 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4391 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_inducing_variables.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5127 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_initial_value.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9171 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_kullback_leiblers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4339 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_logdensities.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9554 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/test_monitor.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/gpflow/utilities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2224 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_bijectors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3094 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_deepcopy.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2740 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_misc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2785 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_model_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3422 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_multipledispatch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2251 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_ops.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3234 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_parameter_or_function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_set_trainable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1845 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_training_loop.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21264 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_traversal.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1226 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/gpflow/utilities/test_utilities.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:21.000000 gpflow-2.8.0/tests/integration/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/integration/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2481 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/integration/test_benchmark.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1441 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/integration/test_docs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5442 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/integration/test_dynamic_shapes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3329 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/integration/test_linear_noise.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11174 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/integration/test_method_equivalence.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1393 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/integration/test_model_serialization.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3020 2023-05-04 08:51:07.000000 gpflow-2.8.0/tests/integration/test_notebooks.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-06-27 14:04:08.000000 gpflow-2.8.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2023-06-27 14:04:08.000000 gpflow-2.8.1/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12653 2023-06-27 14:04:20.000000 gpflow-2.8.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11316 2023-06-27 14:04:08.000000 gpflow-2.8.1/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21625 2023-06-27 14:04:08.000000 gpflow-2.8.1/RELEASE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-06-27 14:04:08.000000 gpflow-2.8.1/VERSION
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/benchmark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:08.000000 gpflow-2.8.1/benchmark/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9767 2023-06-27 14:04:08.000000 gpflow-2.8.1/benchmark/benchmark_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3524 2023-06-27 14:04:08.000000 gpflow-2.8.1/benchmark/benchmarks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10736 2023-06-27 14:04:08.000000 gpflow-2.8.1/benchmark/dataset_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4590 2023-06-27 14:04:08.000000 gpflow-2.8.1/benchmark/datasets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8301 2023-06-27 14:04:08.000000 gpflow-2.8.1/benchmark/grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6597 2023-06-27 14:04:08.000000 gpflow-2.8.1/benchmark/metadata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1652 2023-06-27 14:04:08.000000 gpflow-2.8.1/benchmark/metric_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3286 2023-06-27 14:04:08.000000 gpflow-2.8.1/benchmark/metrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3137 2023-06-27 14:04:08.000000 gpflow-2.8.1/benchmark/model_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2921 2023-06-27 14:04:08.000000 gpflow-2.8.1/benchmark/models.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2023-06-27 14:04:08.000000 gpflow-2.8.1/benchmark/paths.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6093 2023-06-27 14:04:08.000000 gpflow-2.8.1/benchmark/plot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2792 2023-06-27 14:04:08.000000 gpflow-2.8.1/benchmark/plotter_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4478 2023-06-27 14:04:08.000000 gpflow-2.8.1/benchmark/plotters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2438 2023-06-27 14:04:08.000000 gpflow-2.8.1/benchmark/registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2023-06-27 14:04:08.000000 gpflow-2.8.1/benchmark/run.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3496 2023-06-27 14:04:08.000000 gpflow-2.8.1/benchmark/sharding.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4781 2023-06-27 14:04:08.000000 gpflow-2.8.1/benchmark/tag.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/doc/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/doc/sphinx/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      398 2023-06-27 14:04:08.000000 gpflow-2.8.1/doc/sphinx/benchmarks.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2023-06-27 14:04:08.000000 gpflow-2.8.1/doc/sphinx/bibliography.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3109 2023-06-27 14:04:08.000000 gpflow-2.8.1/doc/sphinx/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1473 2023-06-27 14:04:08.000000 gpflow-2.8.1/doc/sphinx/getting_started.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7585 2023-06-27 14:04:08.000000 gpflow-2.8.1/doc/sphinx/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2700 2023-06-27 14:04:08.000000 gpflow-2.8.1/doc/sphinx/installation.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4444 2023-06-27 14:04:08.000000 gpflow-2.8.1/doc/sphinx/user_guide.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1745 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13183 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1772 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/ci_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow/conditionals/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      445 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/conditionals/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5399 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/conditionals/conditionals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1293 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/conditionals/dispatch.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow/conditionals/multioutput/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      110 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/conditionals/multioutput/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11061 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/conditionals/multioutput/conditionals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3007 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/conditionals/multioutput/sample_conditionals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3281 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/conditionals/sample_conditionals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6231 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/conditionals/uncertain_conditionals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23736 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/conditionals/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow/config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12677 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/config/__config__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      618 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/config/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow/covariances/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/covariances/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      695 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/covariances/dispatch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2665 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/covariances/kufs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2370 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/covariances/kuus.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow/covariances/multioutput/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/covariances/multioutput/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6858 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/covariances/multioutput/kufs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4048 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/covariances/multioutput/kuus.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow/expectations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      454 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/expectations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5380 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/expectations/cross_kernels.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      813 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/expectations/dispatch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5479 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/expectations/expectations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5954 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/expectations/linears.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6170 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/expectations/mean_functions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7115 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/expectations/misc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4450 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/expectations/products.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6814 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/expectations/quadratures.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10043 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/expectations/squared_exponentials.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4972 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/expectations/sums.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow/experimental/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      879 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/experimental/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1551 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/experimental/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10582 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/functions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow/inducing_variables/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      785 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/inducing_variables/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      708 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/inducing_variables/inducing_patch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3690 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/inducing_variables/inducing_variables.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow/inducing_variables/multioutput/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/inducing_variables/multioutput/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7262 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/inducing_variables/multioutput/inducing_variables.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow/kernels/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2532 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/kernels/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10659 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/kernels/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5135 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/kernels/categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6817 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/kernels/changepoints.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6351 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/kernels/convolutional.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3844 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/kernels/linears.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11102 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/kernels/misc.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow/kernels/multioutput/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/kernels/multioutput/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15660 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/kernels/multioutput/kernels.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4042 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/kernels/periodic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2823 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/kernels/statics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11179 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/kernels/stationaries.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5901 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/kullback_leiblers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow/likelihoods/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3720 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/likelihoods/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24692 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/likelihoods/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      869 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/likelihoods/misc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9162 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/likelihoods/multiclass.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4782 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/likelihoods/multilatent.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11574 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/likelihoods/scalar_continuous.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7553 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/likelihoods/scalar_discrete.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      948 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/likelihoods/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4530 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/logdensities.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/mean_functions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1909 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14250 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/models/cglb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11614 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/models/gplvm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4451 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/models/gpmc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7000 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/models/gpr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13688 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/models/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4718 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/models/sgpmc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22082 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/models/sgpr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10487 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/models/svgp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5794 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/models/training_mixins.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3692 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/models/util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15454 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/models/vgp.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow/monitor/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      915 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/monitor/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5300 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/monitor/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8983 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/monitor/tensorboard.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      839 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/mypy_flags.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow/optimizers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      269 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/optimizers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5294 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/optimizers/mcmc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18184 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/optimizers/natgrad.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9750 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/optimizers/scipy.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    40522 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/posteriors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3005 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/probability_distributions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/py.typed
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow/quadrature/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      360 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/quadrature/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4887 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/quadrature/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9494 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/quadrature/deprecated.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5590 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/quadrature/gauss_hermite.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1784 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/type_flags.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow/utilities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1217 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/utilities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2169 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/utilities/bijectors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3724 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/utilities/misc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1547 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/utilities/model_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3325 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/utilities/multipledispatch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5626 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/utilities/ops.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1736 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/utilities/parameter_or_function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13979 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/utilities/traversal.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      177 2023-06-27 14:04:08.000000 gpflow-2.8.1/gpflow/versions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12653 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7281 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      354 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2023-06-27 14:04:20.000000 gpflow-2.8.1/gpflow.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-27 14:04:20.000000 gpflow-2.8.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2592 2023-06-27 14:04:08.000000 gpflow-2.8.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/tests/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/tests/gpflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/tests/gpflow/conditionals/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/conditionals/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7895 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/conditionals/test_broadcasted_conditionals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6959 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/conditionals/test_conditionals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32563 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/conditionals/test_multioutput.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10722 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/conditionals/test_uncertain_conditional.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4537 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/conditionals/test_util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/tests/gpflow/config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/config/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6991 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/config/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1278 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/tests/gpflow/covariances/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/covariances/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4244 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/covariances/test_base_covariances.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4968 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/covariances/test_multioutput.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/tests/gpflow/expectations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/expectations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12096 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/expectations/test_expectations.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/tests/gpflow/experimental/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/experimental/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      954 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/experimental/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/tests/gpflow/kernels/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/kernels/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3473 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/kernels/reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9302 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/kernels/test_broadcasting.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      475 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/kernels/test_changepoints.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7805 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/kernels/test_coregion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23223 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/kernels/test_kernels.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2071 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/kernels/test_positive_semidefinite.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1940 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/kernels/test_scaled_euclid_dist.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/tests/gpflow/likelihoods/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/likelihoods/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7752 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/likelihoods/test_function_params.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1688 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/likelihoods/test_heteroskedastic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5586 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/likelihoods/test_heteroskedastic_constant_variance.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11288 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/likelihoods/test_likelihoods.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8112 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/likelihoods/test_multiclass.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7141 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/likelihoods/test_switched_likelihood.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/tests/gpflow/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6499 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/models/test_cglb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3806 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/models/test_gplvm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2220 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/models/test_gpr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2496 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/models/test_gpr_posterior.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1814 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/models/test_mcmc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3160 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/models/test_methods.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7970 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/models/test_model_predict.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2662 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/models/test_sgpr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4189 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/models/test_sgpr_posterior.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6777 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/models/test_svgp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3056 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/models/test_svgp_posterior.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1042 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/models/test_training_mixins.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8714 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/models/test_variational.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1991 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/models/test_vgp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2997 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/models/test_vgp_posterior.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/tests/gpflow/optimizers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/optimizers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7811 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/optimizers/test_mcmc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6341 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/optimizers/test_natural_gradient.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7186 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/optimizers/test_scipy.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/tests/gpflow/posteriors/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/posteriors/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2280 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/posteriors/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13721 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/posteriors/test_bo_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27405 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/posteriors/test_posteriors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3877 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/test_all.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9354 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/test_base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4993 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/test_base_prior.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4057 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/test_base_training.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13060 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/test_functions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4391 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/test_inducing_variables.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5127 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/test_initial_value.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9171 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/test_kullback_leiblers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4339 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/test_logdensities.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9554 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/test_monitor.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/tests/gpflow/utilities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/utilities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2224 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/utilities/test_bijectors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3094 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/utilities/test_deepcopy.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2740 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/utilities/test_misc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2785 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/utilities/test_model_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3422 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/utilities/test_multipledispatch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2251 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/utilities/test_ops.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3234 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/utilities/test_parameter_or_function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/utilities/test_set_trainable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1845 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/utilities/test_training_loop.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21264 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/utilities/test_traversal.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1226 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/gpflow/utilities/test_utilities.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:20.000000 gpflow-2.8.1/tests/integration/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/integration/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2481 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/integration/test_benchmark.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1441 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/integration/test_docs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5442 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/integration/test_dynamic_shapes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3329 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/integration/test_linear_noise.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11174 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/integration/test_method_equivalence.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1393 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/integration/test_model_serialization.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3020 2023-06-27 14:04:08.000000 gpflow-2.8.1/tests/integration/test_notebooks.py
```

### Comparing `gpflow-2.8.0/LICENSE` & `gpflow-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/PKG-INFO` & `gpflow-2.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpflow
-Version: 2.8.0
+Version: 2.8.1
 Summary: Gaussian process methods in TensorFlow
 Home-page: https://www.gpflow.org
 Author: James Hensman, Alex Matthews
 Author-email: james.hensman@gmail.com
 License: Apache License 2.0
 Project-URL: Source on GitHub, https://github.com/GPflow/GPflow
 Project-URL: Documentation, https://gpflow.github.io/GPflow/
```

### Comparing `gpflow-2.8.0/README.md` & `gpflow-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/RELEASE.md` & `gpflow-2.8.1/RELEASE.md`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,29 @@
 ## Thanks to our Contributors
 
 This release contains contributions from:
 
 <INSERT>, <NAME>, <HERE>, <USING>, <GITHUB>, <HANDLE>
 
 
+# Release 2.8.1
+
+A small fix to ensure support for (and testing with) TensorFlow 2.12.
+
+## Bug Fixes and Other Changes
+
+* Support and test with TensorFlow 2.12
+
+## Thanks to our Contributors
+
+This release contains contributions from:
+
+uri-granta
+
+
 # Release 2.8.0
 
 The main focus of this release is to provide users control over arguments for `tf.function`
 compilation inside the Scipy minimize wrapper. It also adds support for a new categorical kernel.
 
 ## Major Features and Improvements
```

### Comparing `gpflow-2.8.0/benchmark/benchmark_api.py` & `gpflow-2.8.1/benchmark/benchmark_api.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/benchmark/benchmarks.py` & `gpflow-2.8.1/benchmark/benchmarks.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/benchmark/dataset_api.py` & `gpflow-2.8.1/benchmark/dataset_api.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/benchmark/datasets.py` & `gpflow-2.8.1/benchmark/datasets.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/benchmark/grouping.py` & `gpflow-2.8.1/benchmark/grouping.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/benchmark/metadata.py` & `gpflow-2.8.1/benchmark/metadata.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/benchmark/metric_api.py` & `gpflow-2.8.1/benchmark/metric_api.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/benchmark/metrics.py` & `gpflow-2.8.1/benchmark/metrics.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/benchmark/model_api.py` & `gpflow-2.8.1/benchmark/model_api.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/benchmark/models.py` & `gpflow-2.8.1/benchmark/models.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/benchmark/paths.py` & `gpflow-2.8.1/benchmark/paths.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/benchmark/plot.py` & `gpflow-2.8.1/benchmark/plot.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/benchmark/plotter_api.py` & `gpflow-2.8.1/benchmark/plotter_api.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/benchmark/plotters.py` & `gpflow-2.8.1/benchmark/plotters.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/benchmark/registry.py` & `gpflow-2.8.1/benchmark/registry.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/benchmark/run.py` & `gpflow-2.8.1/benchmark/run.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/benchmark/sharding.py` & `gpflow-2.8.1/benchmark/sharding.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/benchmark/tag.py` & `gpflow-2.8.1/benchmark/tag.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/doc/sphinx/conf.py` & `gpflow-2.8.1/doc/sphinx/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "GPflow"
 copyright = "2023, The GPflow Contributors"
 author = "The GPflow Contributors"
 
 # The full version, including alpha/beta/rc tags
-release = "2.8.0"
+release = "2.8.1"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `gpflow-2.8.0/doc/sphinx/getting_started.rst` & `gpflow-2.8.1/doc/sphinx/getting_started.rst`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/doc/sphinx/index.rst` & `gpflow-2.8.1/doc/sphinx/index.rst`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/doc/sphinx/installation.rst` & `gpflow-2.8.1/doc/sphinx/installation.rst`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 +---------------------+---------------------------------+
 | 2.8.*               | 0.16.*                          |
 +---------------------+---------------------------------+
 | 2.9.*               | 0.17.*                          |
 +---------------------+---------------------------------+
 | 2.10.*              | 0.18.*                          |
 +---------------------+---------------------------------+
+| 2.11.*              | 0.19.*                          |
++---------------------+---------------------------------+
+| 2.12.*              | 0.20.*                          |
++---------------------+---------------------------------+
 
 Second, a word of warning about new Mac computers. On new Mac machines you will need to install
 ``tensorflow-macos`` instead of the regular ``tensorflow``.
 
 Pre-built installation
 ----------------------
```

### Comparing `gpflow-2.8.0/doc/sphinx/user_guide.rst` & `gpflow-2.8.1/doc/sphinx/user_guide.rst`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/__init__.py` & `gpflow-2.8.1/gpflow/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/base.py` & `gpflow-2.8.1/gpflow/base.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/ci_utils.py` & `gpflow-2.8.1/gpflow/ci_utils.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/conditionals/conditionals.py` & `gpflow-2.8.1/gpflow/conditionals/conditionals.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/conditionals/dispatch.py` & `gpflow-2.8.1/gpflow/conditionals/dispatch.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/conditionals/multioutput/conditionals.py` & `gpflow-2.8.1/gpflow/conditionals/multioutput/conditionals.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/conditionals/multioutput/sample_conditionals.py` & `gpflow-2.8.1/gpflow/conditionals/multioutput/sample_conditionals.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/conditionals/sample_conditionals.py` & `gpflow-2.8.1/gpflow/conditionals/sample_conditionals.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/conditionals/uncertain_conditionals.py` & `gpflow-2.8.1/gpflow/conditionals/uncertain_conditionals.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/conditionals/util.py` & `gpflow-2.8.1/gpflow/conditionals/util.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/config/__config__.py` & `gpflow-2.8.1/gpflow/config/__config__.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/config/__init__.py` & `gpflow-2.8.1/gpflow/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/covariances/dispatch.py` & `gpflow-2.8.1/gpflow/covariances/dispatch.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/covariances/kufs.py` & `gpflow-2.8.1/gpflow/covariances/kufs.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/covariances/kuus.py` & `gpflow-2.8.1/gpflow/covariances/kuus.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/covariances/multioutput/kufs.py` & `gpflow-2.8.1/gpflow/covariances/multioutput/kufs.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/covariances/multioutput/kuus.py` & `gpflow-2.8.1/gpflow/covariances/multioutput/kuus.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/expectations/cross_kernels.py` & `gpflow-2.8.1/gpflow/expectations/cross_kernels.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/expectations/dispatch.py` & `gpflow-2.8.1/gpflow/expectations/dispatch.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/expectations/expectations.py` & `gpflow-2.8.1/gpflow/expectations/expectations.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/expectations/linears.py` & `gpflow-2.8.1/gpflow/expectations/linears.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/expectations/mean_functions.py` & `gpflow-2.8.1/gpflow/expectations/mean_functions.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/expectations/misc.py` & `gpflow-2.8.1/gpflow/expectations/misc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/expectations/products.py` & `gpflow-2.8.1/gpflow/expectations/products.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/expectations/quadratures.py` & `gpflow-2.8.1/gpflow/expectations/quadratures.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/expectations/squared_exponentials.py` & `gpflow-2.8.1/gpflow/expectations/squared_exponentials.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/expectations/sums.py` & `gpflow-2.8.1/gpflow/expectations/sums.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/experimental/__init__.py` & `gpflow-2.8.1/gpflow/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/experimental/utils.py` & `gpflow-2.8.1/gpflow/experimental/utils.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/functions.py` & `gpflow-2.8.1/gpflow/functions.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/inducing_variables/__init__.py` & `gpflow-2.8.1/gpflow/inducing_variables/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/inducing_variables/inducing_patch.py` & `gpflow-2.8.1/gpflow/inducing_variables/inducing_patch.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/inducing_variables/inducing_variables.py` & `gpflow-2.8.1/gpflow/inducing_variables/inducing_variables.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/inducing_variables/multioutput/__init__.py` & `gpflow-2.8.1/gpflow/inducing_variables/multioutput/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/inducing_variables/multioutput/inducing_variables.py` & `gpflow-2.8.1/gpflow/inducing_variables/multioutput/inducing_variables.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/kernels/__init__.py` & `gpflow-2.8.1/gpflow/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/kernels/base.py` & `gpflow-2.8.1/gpflow/kernels/base.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/kernels/categorical.py` & `gpflow-2.8.1/gpflow/kernels/categorical.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/kernels/changepoints.py` & `gpflow-2.8.1/gpflow/kernels/changepoints.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/kernels/convolutional.py` & `gpflow-2.8.1/gpflow/kernels/convolutional.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/kernels/linears.py` & `gpflow-2.8.1/gpflow/kernels/linears.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/kernels/misc.py` & `gpflow-2.8.1/gpflow/kernels/misc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/kernels/multioutput/kernels.py` & `gpflow-2.8.1/gpflow/kernels/multioutput/kernels.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/kernels/periodic.py` & `gpflow-2.8.1/gpflow/kernels/periodic.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/kernels/statics.py` & `gpflow-2.8.1/gpflow/kernels/statics.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/kernels/stationaries.py` & `gpflow-2.8.1/gpflow/kernels/stationaries.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/kullback_leiblers.py` & `gpflow-2.8.1/gpflow/kullback_leiblers.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/likelihoods/__init__.py` & `gpflow-2.8.1/gpflow/likelihoods/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/likelihoods/base.py` & `gpflow-2.8.1/gpflow/likelihoods/base.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/likelihoods/misc.py` & `gpflow-2.8.1/gpflow/likelihoods/misc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/likelihoods/multiclass.py` & `gpflow-2.8.1/gpflow/likelihoods/multiclass.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/likelihoods/multilatent.py` & `gpflow-2.8.1/gpflow/likelihoods/multilatent.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/likelihoods/scalar_continuous.py` & `gpflow-2.8.1/gpflow/likelihoods/scalar_continuous.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/likelihoods/scalar_discrete.py` & `gpflow-2.8.1/gpflow/likelihoods/scalar_discrete.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/likelihoods/utils.py` & `gpflow-2.8.1/gpflow/likelihoods/utils.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/logdensities.py` & `gpflow-2.8.1/gpflow/logdensities.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/mean_functions.py` & `gpflow-2.8.1/gpflow/mean_functions.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/models/__init__.py` & `gpflow-2.8.1/gpflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/models/cglb.py` & `gpflow-2.8.1/gpflow/models/cglb.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/models/gplvm.py` & `gpflow-2.8.1/gpflow/models/gplvm.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/models/gpmc.py` & `gpflow-2.8.1/gpflow/models/gpmc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/models/gpr.py` & `gpflow-2.8.1/gpflow/models/gpr.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/models/model.py` & `gpflow-2.8.1/gpflow/models/model.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/models/sgpmc.py` & `gpflow-2.8.1/gpflow/models/sgpmc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/models/sgpr.py` & `gpflow-2.8.1/gpflow/models/sgpr.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/models/svgp.py` & `gpflow-2.8.1/gpflow/models/svgp.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/models/training_mixins.py` & `gpflow-2.8.1/gpflow/models/training_mixins.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/models/util.py` & `gpflow-2.8.1/gpflow/models/util.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/models/vgp.py` & `gpflow-2.8.1/gpflow/models/vgp.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/monitor/__init__.py` & `gpflow-2.8.1/gpflow/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/monitor/base.py` & `gpflow-2.8.1/gpflow/monitor/base.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/monitor/tensorboard.py` & `gpflow-2.8.1/gpflow/monitor/tensorboard.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/mypy_flags.py` & `gpflow-2.8.1/gpflow/mypy_flags.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/optimizers/mcmc.py` & `gpflow-2.8.1/gpflow/optimizers/mcmc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/optimizers/natgrad.py` & `gpflow-2.8.1/gpflow/optimizers/natgrad.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,14 +197,16 @@
         """
         :param gamma: natgrad step length
         :param xi_transform: default ξ transform (can be overridden in the call to minimize())
             The XiNat default choice works well in general.
         """
         name = self.__class__.__name__ if name is None else name
         super().__init__(name)
+        # explicitly store name (as TF <2.12 stores it differently from TF 2.12+)
+        self.natgrad_name = name
         self.gamma = gamma
         self.xi_transform = xi_transform
 
     @check_shapes(
         "var_list[all][0]: [N, D]",
         "var_list[all][1]: [D, N, N]",
     )
@@ -259,15 +261,15 @@
         with tf.GradientTape(watch_accessed_variables=False) as tape:
             tape.watch(q_mu_vars + q_sqrt_vars)
             loss = loss_fn()
 
         q_mu_grads, q_sqrt_grads = tape.gradient(loss, [q_mu_vars, q_sqrt_vars])
         # NOTE that these are the gradients in *unconstrained* space
 
-        with tf.name_scope(f"{self._name}/natural_gradient_steps"):
+        with tf.name_scope(f"{self.natgrad_name}/natural_gradient_steps"):
             for q_mu_grad, q_sqrt_grad, q_mu, q_sqrt, xi_transform in zip(
                 q_mu_grads, q_sqrt_grads, q_mus, q_sqrts, xis
             ):
                 self._natgrad_apply_gradients(q_mu_grad, q_sqrt_grad, q_mu, q_sqrt, xi_transform)
 
     @check_shapes(
         "q_mu_grad: [N, D]",
```

### Comparing `gpflow-2.8.0/gpflow/optimizers/scipy.py` & `gpflow-2.8.1/gpflow/optimizers/scipy.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/posteriors.py` & `gpflow-2.8.1/gpflow/posteriors.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/probability_distributions.py` & `gpflow-2.8.1/gpflow/probability_distributions.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/quadrature/base.py` & `gpflow-2.8.1/gpflow/quadrature/base.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/quadrature/deprecated.py` & `gpflow-2.8.1/gpflow/quadrature/deprecated.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/quadrature/gauss_hermite.py` & `gpflow-2.8.1/gpflow/quadrature/gauss_hermite.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/type_flags.py` & `gpflow-2.8.1/gpflow/type_flags.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/utilities/__init__.py` & `gpflow-2.8.1/gpflow/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/utilities/bijectors.py` & `gpflow-2.8.1/gpflow/utilities/bijectors.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/utilities/misc.py` & `gpflow-2.8.1/gpflow/utilities/misc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/utilities/model_utils.py` & `gpflow-2.8.1/gpflow/utilities/model_utils.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/utilities/multipledispatch.py` & `gpflow-2.8.1/gpflow/utilities/multipledispatch.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/utilities/ops.py` & `gpflow-2.8.1/gpflow/utilities/ops.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/utilities/parameter_or_function.py` & `gpflow-2.8.1/gpflow/utilities/parameter_or_function.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow/utilities/traversal.py` & `gpflow-2.8.1/gpflow/utilities/traversal.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/gpflow.egg-info/PKG-INFO` & `gpflow-2.8.1/gpflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpflow
-Version: 2.8.0
+Version: 2.8.1
 Summary: Gaussian process methods in TensorFlow
 Home-page: https://www.gpflow.org
 Author: James Hensman, Alex Matthews
 Author-email: james.hensman@gmail.com
 License: Apache License 2.0
 Project-URL: Source on GitHub, https://github.com/GPflow/GPflow
 Project-URL: Documentation, https://gpflow.github.io/GPflow/
```

### Comparing `gpflow-2.8.0/gpflow.egg-info/SOURCES.txt` & `gpflow-2.8.1/gpflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/setup.py` & `gpflow-2.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/conditionals/test_broadcasted_conditionals.py` & `gpflow-2.8.1/tests/gpflow/conditionals/test_broadcasted_conditionals.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/conditionals/test_conditionals.py` & `gpflow-2.8.1/tests/gpflow/conditionals/test_conditionals.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/conditionals/test_multioutput.py` & `gpflow-2.8.1/tests/gpflow/conditionals/test_multioutput.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/conditionals/test_uncertain_conditional.py` & `gpflow-2.8.1/tests/gpflow/conditionals/test_uncertain_conditional.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/conditionals/test_util.py` & `gpflow-2.8.1/tests/gpflow/conditionals/test_util.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/config/test_config.py` & `gpflow-2.8.1/tests/gpflow/config/test_config.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/conftest.py` & `gpflow-2.8.1/tests/gpflow/conftest.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/covariances/test_base_covariances.py` & `gpflow-2.8.1/tests/gpflow/covariances/test_base_covariances.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/covariances/test_multioutput.py` & `gpflow-2.8.1/tests/gpflow/covariances/test_multioutput.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/expectations/test_expectations.py` & `gpflow-2.8.1/tests/gpflow/expectations/test_expectations.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/experimental/test_utils.py` & `gpflow-2.8.1/tests/gpflow/experimental/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/kernels/reference.py` & `gpflow-2.8.1/tests/gpflow/kernels/reference.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/kernels/test_broadcasting.py` & `gpflow-2.8.1/tests/gpflow/kernels/test_broadcasting.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/kernels/test_coregion.py` & `gpflow-2.8.1/tests/gpflow/kernels/test_coregion.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/kernels/test_kernels.py` & `gpflow-2.8.1/tests/gpflow/kernels/test_kernels.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/kernels/test_positive_semidefinite.py` & `gpflow-2.8.1/tests/gpflow/kernels/test_positive_semidefinite.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/kernels/test_scaled_euclid_dist.py` & `gpflow-2.8.1/tests/gpflow/kernels/test_scaled_euclid_dist.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/likelihoods/test_function_params.py` & `gpflow-2.8.1/tests/gpflow/likelihoods/test_function_params.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/likelihoods/test_heteroskedastic.py` & `gpflow-2.8.1/tests/gpflow/likelihoods/test_heteroskedastic.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/likelihoods/test_heteroskedastic_constant_variance.py` & `gpflow-2.8.1/tests/gpflow/likelihoods/test_heteroskedastic_constant_variance.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/likelihoods/test_likelihoods.py` & `gpflow-2.8.1/tests/gpflow/likelihoods/test_likelihoods.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/likelihoods/test_multiclass.py` & `gpflow-2.8.1/tests/gpflow/likelihoods/test_multiclass.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/likelihoods/test_switched_likelihood.py` & `gpflow-2.8.1/tests/gpflow/likelihoods/test_switched_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/models/test_cglb.py` & `gpflow-2.8.1/tests/gpflow/models/test_cglb.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/models/test_gplvm.py` & `gpflow-2.8.1/tests/gpflow/models/test_gplvm.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/models/test_gpr.py` & `gpflow-2.8.1/tests/gpflow/models/test_gpr.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/models/test_gpr_posterior.py` & `gpflow-2.8.1/tests/gpflow/models/test_gpr_posterior.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/models/test_mcmc.py` & `gpflow-2.8.1/tests/gpflow/models/test_mcmc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/models/test_methods.py` & `gpflow-2.8.1/tests/gpflow/models/test_methods.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/models/test_model_predict.py` & `gpflow-2.8.1/tests/gpflow/models/test_model_predict.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/models/test_sgpr.py` & `gpflow-2.8.1/tests/gpflow/models/test_sgpr.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/models/test_sgpr_posterior.py` & `gpflow-2.8.1/tests/gpflow/models/test_sgpr_posterior.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/models/test_svgp.py` & `gpflow-2.8.1/tests/gpflow/models/test_svgp.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/models/test_svgp_posterior.py` & `gpflow-2.8.1/tests/gpflow/models/test_svgp_posterior.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/models/test_training_mixins.py` & `gpflow-2.8.1/tests/gpflow/models/test_training_mixins.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/models/test_variational.py` & `gpflow-2.8.1/tests/gpflow/models/test_variational.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/models/test_vgp.py` & `gpflow-2.8.1/tests/gpflow/models/test_vgp.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/models/test_vgp_posterior.py` & `gpflow-2.8.1/tests/gpflow/models/test_vgp_posterior.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/optimizers/test_mcmc.py` & `gpflow-2.8.1/tests/gpflow/optimizers/test_mcmc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/optimizers/test_natural_gradient.py` & `gpflow-2.8.1/tests/gpflow/optimizers/test_natural_gradient.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/optimizers/test_scipy.py` & `gpflow-2.8.1/tests/gpflow/optimizers/test_scipy.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/posteriors/conftest.py` & `gpflow-2.8.1/tests/gpflow/posteriors/conftest.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/posteriors/test_bo_integration.py` & `gpflow-2.8.1/tests/gpflow/posteriors/test_bo_integration.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/posteriors/test_posteriors.py` & `gpflow-2.8.1/tests/gpflow/posteriors/test_posteriors.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/test_all.py` & `gpflow-2.8.1/tests/gpflow/test_all.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/test_base.py` & `gpflow-2.8.1/tests/gpflow/test_base.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/test_base_prior.py` & `gpflow-2.8.1/tests/gpflow/test_base_prior.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/test_base_training.py` & `gpflow-2.8.1/tests/gpflow/test_base_training.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/test_functions.py` & `gpflow-2.8.1/tests/gpflow/test_functions.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/test_inducing_variables.py` & `gpflow-2.8.1/tests/gpflow/test_inducing_variables.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/test_initial_value.py` & `gpflow-2.8.1/tests/gpflow/test_initial_value.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/test_kullback_leiblers.py` & `gpflow-2.8.1/tests/gpflow/test_kullback_leiblers.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/test_logdensities.py` & `gpflow-2.8.1/tests/gpflow/test_logdensities.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/test_monitor.py` & `gpflow-2.8.1/tests/gpflow/test_monitor.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/utilities/test_bijectors.py` & `gpflow-2.8.1/tests/gpflow/utilities/test_bijectors.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/utilities/test_deepcopy.py` & `gpflow-2.8.1/tests/gpflow/utilities/test_deepcopy.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/utilities/test_misc.py` & `gpflow-2.8.1/tests/gpflow/utilities/test_misc.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/utilities/test_model_utils.py` & `gpflow-2.8.1/tests/gpflow/utilities/test_model_utils.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/utilities/test_multipledispatch.py` & `gpflow-2.8.1/tests/gpflow/utilities/test_multipledispatch.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/utilities/test_ops.py` & `gpflow-2.8.1/tests/gpflow/utilities/test_ops.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/utilities/test_parameter_or_function.py` & `gpflow-2.8.1/tests/gpflow/utilities/test_parameter_or_function.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/utilities/test_set_trainable.py` & `gpflow-2.8.1/tests/gpflow/utilities/test_set_trainable.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/utilities/test_training_loop.py` & `gpflow-2.8.1/tests/gpflow/utilities/test_training_loop.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/utilities/test_traversal.py` & `gpflow-2.8.1/tests/gpflow/utilities/test_traversal.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/gpflow/utilities/test_utilities.py` & `gpflow-2.8.1/tests/gpflow/utilities/test_utilities.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/integration/test_benchmark.py` & `gpflow-2.8.1/tests/integration/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/integration/test_docs.py` & `gpflow-2.8.1/tests/integration/test_docs.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/integration/test_dynamic_shapes.py` & `gpflow-2.8.1/tests/integration/test_dynamic_shapes.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/integration/test_linear_noise.py` & `gpflow-2.8.1/tests/integration/test_linear_noise.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/integration/test_method_equivalence.py` & `gpflow-2.8.1/tests/integration/test_method_equivalence.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/integration/test_model_serialization.py` & `gpflow-2.8.1/tests/integration/test_model_serialization.py`

 * *Files identical despite different names*

### Comparing `gpflow-2.8.0/tests/integration/test_notebooks.py` & `gpflow-2.8.1/tests/integration/test_notebooks.py`

 * *Files identical despite different names*

