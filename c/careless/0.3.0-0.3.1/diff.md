# Comparing `tmp/careless-0.3.0.tar.gz` & `tmp/careless-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "careless-0.3.0.tar", last modified: Tue May 23 21:55:50 2023, max compression
+gzip compressed data, was "careless-0.3.1.tar", last modified: Tue Jun 27 21:50:16 2023, max compression
```

## Comparing `careless-0.3.0.tar` & `careless-0.3.1.tar`

### file list

```diff
@@ -1,85 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.126896 careless-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-23 21:55:39.000000 careless-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-23 21:55:39.000000 careless-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-23 21:55:50.126896 careless-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-23 21:55:39.000000 careless-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.110895 careless-0.3.0/careless/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 21:55:39.000000 careless-0.3.0/careless/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-23 21:55:39.000000 careless-0.3.0/careless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.114896 careless-0.3.0/careless/args/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/crossvalidation.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/filtration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/interpretation.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/required.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/tf_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.118896 careless-0.3.0/careless/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:39.000000 careless-0.3.0/careless/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-23 21:55:39.000000 careless-0.3.0/careless/callbacks/progress_bar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4879 2023-05-23 21:55:39.000000 careless-0.3.0/careless/careless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.118896 careless-0.3.0/careless/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:39.000000 careless-0.3.0/careless/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-23 21:55:39.000000 careless-0.3.0/careless/io/asu.py
--rw-r--r--   0 runner    (1001) docker     (123)    22392 2023-05-23 21:55:39.000000 careless-0.3.0/careless/io/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16476 2023-05-23 21:55:39.000000 careless-0.3.0/careless/io/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-23 21:55:39.000000 careless-0.3.0/careless/io/xds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.118896 careless-0.3.0/careless/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.118896 careless-0.3.0/careless/models/likelihoods/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/likelihoods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/likelihoods/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/likelihoods/laue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/likelihoods/mono.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.122896 careless-0.3.0/careless/models/merging/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/merging/surrogate_posteriors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/merging/variational.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.122896 careless-0.3.0/careless/models/priors/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/priors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/priors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/priors/empirical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/priors/wilson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.122896 careless-0.3.0/careless/models/scaling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/scaling/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/scaling/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/scaling/nn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4389 2023-05-23 21:55:39.000000 careless-0.3.0/careless/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.126896 careless-0.3.0/careless/stats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:39.000000 careless-0.3.0/careless/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-23 21:55:39.000000 careless-0.3.0/careless/stats/ccanom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-23 21:55:39.000000 careless-0.3.0/careless/stats/cchalf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-23 21:55:39.000000 careless-0.3.0/careless/stats/ccpred.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-23 21:55:39.000000 careless-0.3.0/careless/stats/completeness.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-23 21:55:39.000000 careless-0.3.0/careless/stats/rsplit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.126896 careless-0.3.0/careless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:39.000000 careless-0.3.0/careless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-23 21:55:39.000000 careless-0.3.0/careless/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-05-23 21:55:39.000000 careless-0.3.0/careless/utils/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-23 21:55:39.000000 careless-0.3.0/careless/utils/laue.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-23 21:55:39.000000 careless-0.3.0/careless/utils/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-23 21:55:39.000000 careless-0.3.0/careless/utils/shame.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.114896 careless-0.3.0/careless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-23 21:55:50.000000 careless-0.3.0/careless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-23 21:55:50.000000 careless-0.3.0/careless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:55:50.000000 careless-0.3.0/careless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-23 21:55:50.000000 careless-0.3.0/careless.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-23 21:55:50.000000 careless-0.3.0/careless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 21:55:50.000000 careless-0.3.0/careless.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.126896 careless-0.3.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3872 2023-05-23 21:55:39.000000 careless-0.3.0/scripts/make_difference_map
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-05-23 21:55:39.000000 careless-0.3.0/scripts/stream2mtz
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-23 21:55:50.130896 careless-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-23 21:55:39.000000 careless-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.126896 careless-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:39.000000 careless-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-23 21:55:39.000000 careless-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-05-23 21:55:39.000000 careless-0.3.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.425697 careless-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-27 21:50:03.000000 careless-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 21:50:03.000000 careless-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-27 21:50:16.425697 careless-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-06-27 21:50:03.000000 careless-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.417697 careless-0.3.1/careless/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 21:50:03.000000 careless-0.3.1/careless/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-27 21:50:03.000000 careless-0.3.1/careless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.421697 careless-0.3.1/careless/args/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/crossvalidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/filtration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/interpretation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/required.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-27 21:50:03.000000 careless-0.3.1/careless/args/tf_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.421697 careless-0.3.1/careless/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:03.000000 careless-0.3.1/careless/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-27 21:50:03.000000 careless-0.3.1/careless/callbacks/progress_bar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4879 2023-06-27 21:50:03.000000 careless-0.3.1/careless/careless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.421697 careless-0.3.1/careless/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:03.000000 careless-0.3.1/careless/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-27 21:50:03.000000 careless-0.3.1/careless/io/asu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-06-27 21:50:03.000000 careless-0.3.1/careless/io/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16811 2023-06-27 21:50:03.000000 careless-0.3.1/careless/io/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-27 21:50:03.000000 careless-0.3.1/careless/io/xds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.421697 careless-0.3.1/careless/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.421697 careless-0.3.1/careless/models/likelihoods/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/likelihoods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/likelihoods/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/likelihoods/laue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/likelihoods/mono.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.421697 careless-0.3.1/careless/models/merging/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/merging/surrogate_posteriors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/merging/variational.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.421697 careless-0.3.1/careless/models/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/priors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/priors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/priors/empirical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/priors/wilson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.421697 careless-0.3.1/careless/models/scaling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/scaling/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/scaling/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-27 21:50:03.000000 careless-0.3.1/careless/models/scaling/nn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4389 2023-06-27 21:50:03.000000 careless-0.3.1/careless/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.421697 careless-0.3.1/careless/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:03.000000 careless-0.3.1/careless/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-27 21:50:03.000000 careless-0.3.1/careless/stats/ccanom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-27 21:50:03.000000 careless-0.3.1/careless/stats/cchalf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-27 21:50:03.000000 careless-0.3.1/careless/stats/ccpred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-27 21:50:03.000000 careless-0.3.1/careless/stats/completeness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-27 21:50:03.000000 careless-0.3.1/careless/stats/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-06-27 21:50:03.000000 careless-0.3.1/careless/stats/prior_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-27 21:50:03.000000 careless-0.3.1/careless/stats/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-27 21:50:03.000000 careless-0.3.1/careless/stats/rsplit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.425697 careless-0.3.1/careless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:03.000000 careless-0.3.1/careless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-27 21:50:03.000000 careless-0.3.1/careless/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-06-27 21:50:03.000000 careless-0.3.1/careless/utils/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-27 21:50:03.000000 careless-0.3.1/careless/utils/laue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-27 21:50:03.000000 careless-0.3.1/careless/utils/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-27 21:50:03.000000 careless-0.3.1/careless/utils/shame.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.417697 careless-0.3.1/careless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-27 21:50:16.000000 careless-0.3.1/careless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-27 21:50:16.000000 careless-0.3.1/careless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:50:16.000000 careless-0.3.1/careless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-27 21:50:16.000000 careless-0.3.1/careless.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-27 21:50:16.000000 careless-0.3.1/careless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 21:50:16.000000 careless-0.3.1/careless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.425697 careless-0.3.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3872 2023-06-27 21:50:03.000000 careless-0.3.1/scripts/make_difference_map
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-06-27 21:50:03.000000 careless-0.3.1/scripts/stream2mtz
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-27 21:50:16.425697 careless-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-27 21:50:03.000000 careless-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:16.425697 careless-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:50:03.000000 careless-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-27 21:50:03.000000 careless-0.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-06-27 21:50:03.000000 careless-0.3.1/tests/test_cli.py
```

### Comparing `careless-0.3.0/LICENSE` & `careless-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/PKG-INFO` & `careless-0.3.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: careless
-Version: 0.3.0
+Version: 0.3.1
 Summary: Merging crystallography data without much physics.
 Home-page: https://github.com/rs-station/careless
 Author: Kevin M. Dalton
 Author-email: kmdalton@fas.harvard.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rs-station/careless/issues
 Project-URL: Source Code, https://github.com/rs-station/careless
```

### Comparing `careless-0.3.0/README.md` & `careless-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/args/common.py` & `careless-0.3.1/careless/args/common.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/args/crossvalidation.py` & `careless-0.3.1/careless/args/crossvalidation.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/args/filtration.py` & `careless-0.3.1/careless/args/filtration.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/args/interpretation.py` & `careless-0.3.1/careless/args/interpretation.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,23 @@
     (("--intensity-key", ),  {
         "help":"What key to use for reflection intensities. "
                "If no key is given, careless will use the first key with the intensity dtype.",
         "type":str, 
         "default" : None,
     }),
 
+    (("--uncertainty-key", ),  {
+        "help":"What key to use for reflection error estimates. "
+               "If no key is given, careless will first check for a key beginning with 'SIG' or 'Sig' "
+               "which matches the intensity key (e.g. Iobs -> SigIobs). "
+               "Failing that, careless will ust first key with the StdDev dtype.",
+        "type":str, 
+        "default" : None,
+    }),
+
     (("--anomalous",), { 
         "help":f"If this flag is supplied, Friedel mates will be kept separate.", 
         "action":'store_true', 
         "default":False,
     }),
 
     (("--separate-files",), {
```

### Comparing `careless-0.3.0/careless/args/optimizer.py` & `careless-0.3.1/careless/args/optimizer.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/args/poly.py` & `careless-0.3.1/careless/args/poly.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/args/positional_encoding.py` & `careless-0.3.1/careless/args/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/args/prior.py` & `careless-0.3.1/careless/args/prior.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/args/required.py` & `careless-0.3.1/careless/args/required.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/args/scaling.py` & `careless-0.3.1/careless/args/scaling.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/args/tf_options.py` & `careless-0.3.1/careless/args/tf_options.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/callbacks/progress_bar.py` & `careless-0.3.1/careless/callbacks/progress_bar.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/careless.py` & `careless-0.3.1/careless/careless.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/io/asu.py` & `careless-0.3.1/careless/io/asu.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,31 +143,37 @@
             (n x 3) array of miller indices 
         """
         data = self.refl_id_lookup_table.loc[refl_id.flatten()]
         H = data.get_hkls()
         asu_id = data['asu_id'].to_numpy('int')
         return asu_id[:,None], H
 
-    def to_refl_id(self, asu_id, H):
+    def to_refl_id(self, asu_id, H, allow_missing=False):
         """
         Parameters
         ----------
         asu_id : np.array
             (n x 1) array of asu ids 
         H : np.array
             (n x 3) array of miller indices 
+        allow_missing : bool (optional)
+            Replace missing reflections with -1 rather than throwing an error
 
         Returns
         -------
         refl_id : np.array
             (n x 1) array of integer reflection ids to convert to miller indices
         """
         idx = np.concatenate((asu_id, H), axis=1).astype('int')
         idx = pd.MultiIndex.from_arrays(idx.T, names = ['asu_id', 'H', 'K', 'L'])
-        return self.asu_and_miller_lookup_table.loc[idx, 'id'].to_numpy('int')
+        if allow_missing:
+            refl_ids = pd.DataFrame(index=idx).join(self.asu_and_miller_lookup_table.id)
+            refl_ids = refl_ids.fillna(-1).to_numpy("int").flatten()
+            return refl_ids
+        return self.asu_and_miller_lookup_table.loc[idx, 'id'].to_numpy('int').flatten()
 
     def __getitem__(self, i):
         return self.reciprocal_asus[i]
 
     def __len__(self):
         return len(self.reciprocal_asus)
```

### Comparing `careless-0.3.0/careless/io/formatter.py` & `careless-0.3.1/careless/io/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,15 +207,15 @@
                 raise ValueError(
                     "Multiple values provided for --spacegroups=, but the number of provided values does not match the number of reflection files. "
                     "Either provide a single spacegroup or one per reflection file as a comma-separated list. " 
                 )
 
         return cls(
             parser.intensity_key,
-            None, #<-- uncertainty key has to match {SIG,Sig}intensity_key
+            parser.uncertainty_key,
             parser.image_key,
             parser.metadata_keys.split(','),
             parser.separate_files,
             parser.anomalous,
             dmin,
             parser.isigi_cutoff,
             pe_keys,
@@ -284,19 +284,17 @@
         # Try to guess the uncertainty key
         uncertainty_key = self.uncertainty_key
         if uncertainty_key is None:
             for prefix in ['Sig', 'SIG']:
                 for k in ds:
                     if k == prefix + intensity_key:
                         uncertainty_key = k
-        # TODO: this is a temporary fix for an older version of the crystfel parser
-        # please remove this upon the next rs release (2021-09-10)
         if uncertainty_key is None:
-            if 'sigmaI' in ds:
-                uncertainty_key = 'sigmaI'
+            uncertainty_key = get_first_key_of_dtype(ds, 'Q')
+
 
         if uncertainty_key is None:
             raise ValueError(
                 f"No matching uncertainty key found for intensity key {intensity_key}"
                  "please manually specify the uncertainty key. "
             )
 
@@ -333,24 +331,26 @@
             metadata = standardize_metadata(metadata)
 
         if self.positional_encoding_keys is not None:
             to_encode = data[self.positional_encoding_keys].to_numpy('float32')
             encoded  = positional_encoding(to_encode, self.ecoding_bit_depth)
             metadata = np.concatenate((metadata, encoded), axis=1)
 
+        file_id = data['file_id'].to_numpy('int64')
         refl_id = rac.to_refl_id(
             data['asu_id'].to_numpy('int64')[:,None],
             data.get_hkls(),
             )
 
         iobs    = data['intensity'].to_numpy('float32')[:,None]
         sigiobs = data['uncertainty'].to_numpy('float32')[:,None]
 
         inputs = {
             'refl_id'   : refl_id[:,None],
+            'file_id'   : file_id[:,None],
             'image_id'  : data['image_id'].to_numpy('int64')[:,None],
             'metadata'  : metadata,
             'intensities'   : iobs,
             'uncertainties' : sigiobs,
         }
 
         return self.pack_inputs(inputs), rac
@@ -439,15 +439,15 @@
                     "Multiple values provided for --spacegroups=, but the number of provided values does not match the number of reflection files. "
                     "Either provide a single spacegroup or one per reflection file as a comma-separated list. " 
                 )
 
         return cls(
             parser.wavelength_key,
             parser.intensity_key,
-            None, #<-- uncertainty key has to match {SIG,Sig}intensity_key
+            parser.uncertainty_key,
             parser.image_key,
             parser.metadata_keys.split(','),
             parser.separate_files,
             parser.anomalous,
             lmin,
             lmax,
             parser.dmin,
@@ -532,19 +532,16 @@
         # Try to guess the uncertainty key
         uncertainty_key = self.uncertainty_key
         if uncertainty_key is None:
             for prefix in ['Sig', 'SIG']:
                 for k in ds:
                     if k == prefix + intensity_key:
                         uncertainty_key = k
-        # TODO: this is a temporary fix for an older version of the crystfel parser
-        # please remove this upon the next rs release (2021-09-10)
         if uncertainty_key is None:
-            if 'sigmaI' in ds:
-                uncertainty_key = 'sigmaI'
+            uncertainty_key = get_first_key_of_dtype(ds, 'Q')
 
         if uncertainty_key is None:
             raise ValueError(
                 f"No matching uncertainty key found for intensity key {intensity_key}"
                  "please manually specify the uncertainty key. "
             )
 
@@ -585,26 +582,28 @@
             metadata = standardize_metadata(metadata)
 
         if self.positional_encoding_keys is not None:
             to_encode = data[self.positional_encoding_keys].to_numpy('float32')
             encoded  = positional_encoding(to_encode, self.ecoding_bit_depth)
             metadata = np.concatenate((metadata, encoded), axis=1)
 
+        file_id = data['file_id'].to_numpy('int64')
         refl_id = rac.to_refl_id(
             data['asu_id'].to_numpy('int64')[:,None],
             data.get_hkls(),
             )
 
         iobs  = data[['harmonic_id',   'intensity']].groupby('harmonic_id').first().to_numpy('float32')
         sigma = data[['harmonic_id', 'uncertainty']].groupby('harmonic_id').first().to_numpy('float32')
         iobs  = np.pad( iobs, [[0, len(refl_id) - len( iobs)], [0, 0]], constant_values=1.)
         sigma = np.pad(sigma, [[0, len(refl_id) - len(sigma)], [0, 0]], constant_values=1.)
 
         inputs = {
             'refl_id'   : refl_id[:,None],
+            'file_id'   : file_id[:,None],
             'image_id'  : data['image_id'].to_numpy('int64')[:,None],
             'metadata'  : metadata,
             'intensities'   : iobs,
             'uncertainties'   : sigma,
             'wavelength' : data[self.wavelength_key].to_numpy('float32')[:,None],
             'harmonic_id' : data['harmonic_id'].to_numpy('int64')[:,None],
         }
```

### Comparing `careless-0.3.0/careless/io/manager.py` & `careless-0.3.1/careless/io/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,18 +34,23 @@
     def from_mtz_files(cls, filenames, formatter):
         return cls.from_datasets((rs.read_mtz(i) for i in filenames), formatter)
 
     @classmethod
     def from_stream_files(cls, filenames, formatter):
         return cls.from_datasets((rs.read_crystfel(i) for i in filenames), formatter)
 
+    @staticmethod
+    def wilson_sigma(b, dHKL):
+        sigma = np.exp(-0.25 * b * np.reciprocal(dHKL*dHKL))
+        return sigma
+
     def get_wilson_sigma(self, b=None):
         if b is None:
             return 1.
-        sigma = np.exp(-0.25 * b * self.asu_collection.dHKL**-2.)
+        sigma = self.wilson_sigma(b, self.asu_collection.dHKL)
         return sigma
 
     def get_wilson_prior(self, b=None, k=1.):
         """ Construct a wilson prior with an optional temperature factor, b, appropriate for self.asu_collection. """
         if b is None:
             sigma = 1.
         elif isinstance(b, float):
@@ -101,28 +106,31 @@
 
         refl_id = BaseModel.get_refl_id(inputs)
         iobs = BaseModel.get_intensities(inputs).flatten()
         sig_iobs = BaseModel.get_uncertainties(inputs).flatten()
         asu_id,H = self.asu_collection.to_asu_id_and_miller_index(refl_id)
         #ipred = model(inputs)
         ipred,sigipred = model.prediction_mean_stddev(inputs)
+        scale,sigscale = model.prediction_mean_stddev(inputs)
 
         h,k,l = H.T
         results = ()
         for i,asu in enumerate(self.asu_collection):
             idx = asu_id == i
             idx = idx.flatten()
             output = rs.DataSet({
                 'H' : h[idx],
                 'K' : k[idx],
                 'L' : l[idx],
                 'Iobs' : iobs[idx],
                 'SigIobs' : sig_iobs[idx],
                 'Ipred' : ipred[idx],
                 'SigIpred' : sigipred[idx],
+                'Scale' : scale[idx],
+                'SigScale' : sigscale[idx],
                 }, 
                 cell=asu.cell, 
                 spacegroup=asu.spacegroup,
                 merged=False,
             ).infer_mtz_dtypes().set_index(['H', 'K', 'L'])
             results += (output, )
         return results
@@ -171,14 +179,15 @@
                 params[k] = numpify(v).flatten() * np.ones(len(F), dtype='float32')
         asu_id,H = self.asu_collection.to_asu_id_and_miller_index(np.arange(len(F)))
         h,k,l = H.T
         refl_id = BaseModel.get_refl_id(inputs)
         N = np.bincount(refl_id.flatten(), minlength=len(F)).astype('float32')
         results = ()
         for i,asu in enumerate(self.asu_collection):
+            multiplicity = asu.multiplicity.astype('float32')
             idx = asu_id == i
             idx = idx.flatten()
             output = rs.DataSet({
                 'H' : h[idx],
                 'K' : k[idx],
                 'L' : l[idx],
                 'F' : F[idx],
```

### Comparing `careless-0.3.0/careless/io/xds.py` & `careless-0.3.1/careless/io/xds.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/models/base.py` & `careless-0.3.1/careless/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,20 @@
         harmonic_id
     } static methods to parse your inputs. This ensures it is easy to
     change the data format in the future.
     """
     input_index = {
         'refl_id'       : 0,
         'image_id'      : 1,
-        'metadata'      : 2,
-        'intensities'   : 3,
-        'uncertainties' : 4,
-        'wavelength'    : 5,
-        'harmonic_id'   : 6,
+        'file_id'       : 2,
+        'metadata'      : 3,
+        'intensities'   : 4,
+        'uncertainties' : 5,
+        'wavelength'    : 6,
+        'harmonic_id'   : 7,
     }
 
     def call(self, inputs):
         raise NotImplementedError(
             "All Scaler classes must implement a call method which accepts inputs "
             "defined by this class.                                               "
         )
@@ -81,14 +82,19 @@
 
     @staticmethod
     def get_refl_id(inputs):
         """ Given a collection of inputs extract just the reflection_id """
         return BaseModel.get_input_by_name(inputs, 'refl_id')
 
     @staticmethod
+    def get_file_id(inputs):
+        """ Given a collection of inputs extract just the file_id """
+        return BaseModel.get_input_by_name(inputs, 'file_id')
+
+    @staticmethod
     def get_image_id(inputs):
         """ Given a collection of inputs extract just the image_id """
         return BaseModel.get_input_by_name(inputs, 'image_id')
 
     @staticmethod
     def get_metadata(inputs):
         """ Given a collection of inputs extract just the metadata """
```

### Comparing `careless-0.3.0/careless/models/likelihoods/laue.py` & `careless-0.3.1/careless/models/likelihoods/laue.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/models/likelihoods/mono.py` & `careless-0.3.1/careless/models/likelihoods/mono.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/models/merging/surrogate_posteriors.py` & `careless-0.3.1/careless/models/merging/surrogate_posteriors.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/models/merging/variational.py` & `careless-0.3.1/careless/models/merging/variational.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,14 +40,47 @@
         self.likelihood = likelihood
         self.scaling_model = scaling_model
         self.mc_sample_size = mc_sample_size
         self.kl_weight = kl_weight
         self.scale_kl_weight = scale_kl_weight
         self.scale_prior = scale_prior
 
+    def scale_mean_sttdev(self, inputs):
+        """
+        Compute the moments of the posterior of reflection observation scale factors. 
+
+        Parameters
+        ----------
+        inputs : data
+            inputs is a data structure like [refl_id, image_id, metadata, intensity, uncertainty]. 
+            This can be a tf.DataSet, or a group of tensors. 
+
+        Returns
+        -------
+        mean : np.array
+            A numpy array containing the mean value of the scale predicted by the model for each input. 
+        stddev : np.array
+            A numpy array containing the standard deviation of the scale predicted by the model for each input. 
+            This is a reasonable estimate of the uncertainty of the model about each input.
+        """
+        refl_id = self.get_refl_id(inputs)
+
+        scale_dist = self.scaling_model(inputs)
+        mean = scale_dist.mean().numpy()
+        stddev = scale_dist.stddev().numpy()
+
+        # We need to convolve the predictions if this is laue data
+        from careless.models.likelihoods.laue import LaueBase
+        if isinstance(self.likelihood, LaueBase):
+            likelihood = self.likelihood(inputs)
+            mean = likelihood.convolve(mean)
+            stddev = np.sqrt(likelihood.convolve(stddev * stddev))
+
+        return mean, stddev
+
     def prediction_mean_stddev(self, inputs):
         """
         Parameters
         ----------
         inputs : data
             inputs is a data structure like [refl_id, image_id, metadata, intensity, uncertainty]. 
             This can be a tf.DataSet, or a group of tensors.
```

### Comparing `careless-0.3.0/careless/models/priors/empirical.py` & `careless-0.3.1/careless/models/priors/empirical.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/models/priors/wilson.py` & `careless-0.3.1/careless/models/priors/wilson.py`

 * *Files 8% similar despite different names*

```diff
@@ -113,34 +113,39 @@
                 root.append(np.ones(len(child_asu.lookup_table), dtype='bool'))
             else:
                 root.append(np.zeros(len(child_asu.lookup_table), dtype='bool'))
                 parent_asu = asu_collection.reciprocal_asus[parent]
                 h = child_asu.Hall
                 h,_ = rs.utils.hkl_to_asu(h, parent_asu.spacegroup)
                 pid = parent*np.ones((len(h), 1), dtype='int32')
-                reflids.append(asu_collection.to_refl_id(pid, h))
+                reflids.append(asu_collection.to_refl_id(pid, h, allow_missing=True))
 
         self.centric = asu_collection.centric
         self.multiplicity = asu_collection.multiplicity
 
         self.sigma = sigma
         self.reflids = np.concatenate(reflids)
+        self.absent = tf.convert_to_tensor(self.reflids == -1)
         self.r = np.concatenate(r)
         self.root = np.concatenate(root)
         self.wilson_prior = WilsonPrior(asu_collection.centric, asu_collection.multiplicity, sigma)
 
     def mean(self):
         return self.wilson_prior.mean()
 
     def stddev(self):
         return self.wilson_prior.stddev()
 
     def log_prob(self, z):
         z_parent = tf.gather(z, self.reflids, axis=-1)
-        loc = z_parent * self.r
+        loc = tf.where(
+            self.absent, 
+            0.,
+            z_parent * self.r
+        )
         r2 = tf.square(self.r)
         scale = tf.where(
             self.centric,
             tf.math.sqrt(self.multiplicity * self.sigma * (1. - r2)),
             tf.math.sqrt(0.5*self.multiplicity * self.sigma * (1. - r2)),
         )
```

### Comparing `careless-0.3.0/careless/models/scaling/image.py` & `careless-0.3.1/careless/models/scaling/image.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/models/scaling/nn.py` & `careless-0.3.1/careless/models/scaling/nn.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/parser.py` & `careless-0.3.1/careless/parser.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/stats/ccanom.py` & `careless-0.3.1/careless/stats/ccanom.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 """
 import argparse
 import matplotlib.pyplot as plt
 import reciprocalspaceship as rs
 import seaborn as sns
 
 
-class ArgumentParser(argparse.ArgumentParser):
+from careless.stats.parser import BaseParser
+class ArgumentParser(BaseParser):
     def __init__(self):
         super().__init__(
-            formatter_class=argparse.RawTextHelpFormatter, 
             description=__doc__
         )
 
         # Required arguments
         self.add_argument(
             "mtz",
             nargs="+",
@@ -23,32 +23,26 @@
 
         # Optional arguments
         self.add_argument(
             "-m",
             "--method",
             default="spearman",
             choices=["spearman", "pearson"],
-            help=("Method for computing correlation coefficient (spearman or pearson)"),
+            help="Method for computing correlation coefficient (spearman or pearson)",
         )
 
         self.add_argument(
             "-b",
             "--bins",
             default=10,
             type=int,
-            help=("Number of resolution bins to use, the default is 10."),
+            help="Number of resolution bins to use, the default is 10.",
         )
 
-        self.add_argument(
-            "-o",
-            "--output",
-            type=str,
-            default=None,
-            help=("Optionally save CCanom values to this file in csv format."),
-        )
+
 
 
 
 def make_halves_ccanom(mtz, bins=10):
     """Construct half-datasets for computing CCanom"""
 
     half1 = mtz.loc[mtz.half == 0].copy()
@@ -88,15 +82,15 @@
 
     if return_labels:
         return result, labels
     else:
         return result
 
 
-def run_analysis(args, show=True):
+def run_analysis(args):
     results = []
     labels = None
     for m in args.mtz:
         result = analyze_ccanom_mtz(m, method=args.method, bins=args.bins)
         if result is None:
             continue
         else:
@@ -110,24 +104,29 @@
     results.drop(columns=[("DF1", "DF2")], inplace=True)
 
     for k in ('bin', 'repeat'):
         results[k] = results[k].to_numpy('int32')
 
     if args.output is not None:
         results.to_csv(args.output)
+    else:
+        print(results.to_string())
 
     sns.lineplot(
         data=results, x="bin", y="CCanom", hue="filename", palette="Dark2"
     )
     plt.xticks(range(args.bins), labels, rotation=45, ha="right", rotation_mode="anchor")
     plt.ylabel(r"$\mathrm{CC_{anom}}$ " + f"({args.method})")
     plt.xlabel("Resolution ($\mathrm{\AA}$)")
     plt.grid(which='both', axis='both', ls='dashdot')
     plt.tight_layout()
-    if show:
-        print(results.to_string())
+
+    if args.image is not None:
+        plt.savefig(args.image)
+
+    if args.show:
         plt.show()
 
 def main():
     parser = ArgumentParser().parse_args()
-    run_analysis(parser, True)
+    run_analysis(parser)
```

### Comparing `careless-0.3.0/careless/stats/cchalf.py` & `careless-0.3.1/careless/stats/cchalf.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 """
 import argparse
 import matplotlib.pyplot as plt
 import reciprocalspaceship as rs
 import seaborn as sns
 
 
-class ArgumentParser(argparse.ArgumentParser):
+from careless.stats.parser import BaseParser
+class ArgumentParser(BaseParser):
     def __init__(self):
         super().__init__(
-            formatter_class=argparse.RawTextHelpFormatter, 
             description=__doc__
         )
 
         # Required arguments
         self.add_argument(
             "mtz",
             nargs="+",
@@ -33,23 +33,14 @@
             "-b",
             "--bins",
             default=10,
             type=int,
             help=("Number of resolution bins to use, the default is 10."),
         )
 
-        self.add_argument(
-            "-o",
-            "--output",
-            type=str,
-            default=None,
-            help=("Optionally save CChalf values to this file in csv format."),
-        )
-
-
 def make_halves_cchalf(mtz, bins=10):
     """Construct half-datasets for computing CChalf"""
 
     half1 = mtz.loc[mtz.half == 0].copy()
     half2 = mtz.loc[mtz.half == 1].copy()
 
     # Support anomalous
@@ -83,15 +74,15 @@
 
     if return_labels:
         return result, labels
     else:
         return result
 
 
-def run_analysis(args, show=True):
+def run_analysis(args):
     results = []
     labels = None
     for m in args.mtz:
         result = analyze_cchalf_mtz(m, bins=args.bins, method=args.method)
         if result is None:
             continue
         else:
@@ -106,25 +97,30 @@
 
 
     for k in ('bin', 'repeat'):
         results[k] = results[k].to_numpy('int32')
 
     if args.output is not None:
         results.to_csv(args.output)
+    else:
+        print(results.to_string())
     
     sns.lineplot(
         data=results, x="bin", y="CChalf", hue="filename", palette="viridis"
     )
     plt.xticks(range(args.bins), labels, rotation=45, ha="right", rotation_mode="anchor")
     plt.ylabel(r"$\mathrm{CC_{1/2}}$ " + f"({args.method})")
     plt.xlabel("Resolution ($\mathrm{\AA}$)")
     plt.grid(which='both', axis='both', ls='dashdot')
     plt.tight_layout()
-    if show:
-        print(results.to_string())
+
+    if args.image is not None:
+        plt.savefig(args.image)
+
+    if args.show:
         plt.show()
 
 
 def main():
     parser = ArgumentParser().parse_args()
-    run_analysis(parser, True)
+    run_analysis(parser)
```

### Comparing `careless-0.3.0/careless/stats/ccpred.py` & `careless-0.3.1/careless/stats/ccpred.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 import reciprocalspaceship as rs
 import gemmi
 
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 
-class ArgumentParser(argparse.ArgumentParser):
+from careless.stats.parser import BaseParser
+class ArgumentParser(BaseParser):
     def __init__(self):
         super().__init__(
-            formatter_class=argparse.RawTextHelpFormatter, 
             description=__doc__
         )
 
         # Required arguments
         self.add_argument(
             "mtzs",
             nargs="+",
@@ -44,28 +44,14 @@
 
         self.add_argument(
             '--overall',
             action="store_true",
             help="Pool all prediction mtz files into a single calculation rather than treating each file individually.",
         )
 
-        self.add_argument(
-            "-o",
-            "--output",
-            type=str,
-            default=None,
-            help="Optionally save CCpred values to this file in csv format.",
-        )
-
-        self.add_argument(
-            "--plot",
-            action="store_true",
-            help="Make a plot of the results with seaborn and display it using matplotlib.",
-        )
-
 
 def compute_ccpred(
     dataset, overall=False, bins=10, return_labels=True, method="spearman"
 ):
     """Compute CCpred from cross-validation"""
 
     if overall:
@@ -117,14 +103,16 @@
     results.drop(columns=[("Iobs", "Ipred")], inplace=True)
 
     results['bin'] = results['bin'].to_numpy('int32')
     results['test'] = np.array(['Train', 'Test'])[results['test']]
 
     if args.output is not None:
         results.to_csv(args.output)
+    else:
+        print(results.to_string())
 
     plot_kwargs = {
         'data' : results,
         'x' : 'bin',
         'y' : 'CCpred',
         'style' : 'test',
     }
@@ -139,15 +127,18 @@
 
     plt.xticks(range(args.bins), labels, rotation=45, ha="right", rotation_mode="anchor")
     plt.ylabel(r"$\mathrm{CC_{pred}}$ " + f"({args.method})")
     plt.legend(loc="center left", bbox_to_anchor=(1, 0.5))
     plt.xlabel("Resolution ($\mathrm{\AA}$)")
     plt.grid(which='both', axis='both', ls='dashdot')
     plt.tight_layout()
-    print(results.to_string())
-    if args.plot:
+
+    if args.image is not None:
+        plt.savefig(args.image)
+
+    if args.show:
         plt.show()
 
 def main():
     parser = ArgumentParser().parse_args()
     run_analysis(parser)
```

### Comparing `careless-0.3.0/careless/stats/completeness.py` & `careless-0.3.1/careless/stats/completeness.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 """
 import argparse
 import matplotlib.pyplot as plt
 import reciprocalspaceship as rs
 import seaborn as sns
 import numpy as np
 
-
-class ArgumentParser(argparse.ArgumentParser):
+from careless.stats.parser import BaseParser
+class ArgumentParser(BaseParser):
     def __init__(self):
         super().__init__(
-            formatter_class=argparse.RawTextHelpFormatter, 
             description=__doc__
         )
 
         # Required arguments
         self.add_argument(
             "mtz",
             help="MTZ containing merged data from careless",
@@ -25,28 +24,22 @@
             "-b",
             "--bins",
             default=10,
             type=int,
             help=("Number of resolution bins to use, the default is 10."),
         )
 
-        self.add_argument(
-            "-o",
-            "--output",
-            type=str,
-            default=None,
-            help=("Optionally save completeness values to this file in csv format."),
-        )
-
-def run_analysis(args, show=True):
+def run_analysis(args):
     ds = rs.read_mtz(args.mtz)
     results = rs.stats.compute_completeness(ds, bins=args.bins)
 
     if args.output is not None:
         results.to_csv(args.output)
+    else:
+        print(results.to_string())
 
     #Move overall to the beginning
     results = results.iloc[np.roll(np.arange(len(results)), 1)]
 
     ax = sns.lineplot(
         data=results.reset_index().melt('index'),
         x='index',
@@ -56,16 +49,18 @@
     )
     plt.xticks(rotation=45, rotation_mode='anchor', ha='right')
     plt.legend(title="")
     plt.ylabel(r"Completeness")
     plt.xlabel("Resolution ($\mathrm{\AA}$)")
     plt.grid(which='both', axis='both', ls='dashdot')
     plt.tight_layout()
-    if show:
-        print(results.to_string())
-        plt.show()
 
+    if args.image is not None:
+        plt.savefig(args.image)
+
+    if args.show:
+        plt.show()
 
 def main():
     parser = ArgumentParser().parse_args()
-    run_analysis(parser, True)
+    run_analysis(parser)
```

### Comparing `careless-0.3.0/careless/stats/rsplit.py` & `careless-0.3.1/careless/stats/rsplit.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import matplotlib.pyplot as plt
 import reciprocalspaceship as rs
 import seaborn as sns
 from scipy.optimize import minimize
 import numpy as np
 
 
-class ArgumentParser(argparse.ArgumentParser):
+from careless.stats.parser import BaseParser
+class ArgumentParser(BaseParser):
     def __init__(self):
         super().__init__(
-            formatter_class=argparse.RawTextHelpFormatter, 
             description=__doc__
         )
 
         # Required arguments
         self.add_argument(
             "mtz",
             nargs="+",
@@ -33,22 +33,14 @@
 
         self.add_argument(
             "--use-intensities",
             action="store_true",
             help=("Optionally use intensities instead of structure factors to facilitate comparisons with other softwares."),
         )
 
-        self.add_argument(
-            "-o",
-            "--output",
-            type=str,
-            default=None,
-            help=("Optionally save Rsplit values to this file in csv format."),
-        )
-
 
 def make_halves_cchalf(mtz, bins=10):
     """Construct half-datasets for computing Rsplit"""
 
     half1 = mtz.loc[mtz.half == 0].copy()
     half2 = mtz.loc[mtz.half == 1].copy()
 
@@ -94,15 +86,15 @@
 
     if return_labels:
         return result, labels
     else:
         return result
 
 
-def run_analysis(args, show=True):
+def run_analysis(args):
     results = []
     labels = None
 
     if args.use_intensities:
         keys = ("I1", "I2")
     else:
         keys = ("F1", "F2")
@@ -123,25 +115,30 @@
 
 
     for k in ('bin', 'repeat'):
         results[k] = results[k].to_numpy('int32')
 
     if args.output is not None:
         results.to_csv(args.output)
+    else:
+        print(results.to_string())
     
     sns.lineplot(
         data=results, x="bin", y="Rsplit", hue="filename", palette="Dark2"
     )
     plt.xticks(range(args.bins), labels, rotation=45, ha="right", rotation_mode="anchor")
     plt.ylabel(r"$\mathrm{R_{split}}$ ")
     plt.xlabel("Resolution ($\mathrm{\AA}$)")
     plt.grid(which='both', axis='both', ls='dashdot')
     plt.tight_layout()
-    if show:
-        print(results.to_string())
+
+    if args.image is not None:
+        plt.savefig(args.image)
+
+    if args.show:
         plt.show()
 
 
 def main():
     parser = ArgumentParser().parse_args()
-    run_analysis(parser, True)
+    run_analysis(parser)
```

### Comparing `careless-0.3.0/careless/utils/distributions.py` & `careless-0.3.1/careless/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/utils/laue.py` & `careless-0.3.1/careless/utils/laue.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless/utils/positional_encoding.py` & `careless-0.3.1/careless/utils/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/careless.egg-info/PKG-INFO` & `careless-0.3.1/careless.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: careless
-Version: 0.3.0
+Version: 0.3.1
 Summary: Merging crystallography data without much physics.
 Home-page: https://github.com/rs-station/careless
 Author: Kevin M. Dalton
 Author-email: kmdalton@fas.harvard.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rs-station/careless/issues
 Project-URL: Source Code, https://github.com/rs-station/careless
```

### Comparing `careless-0.3.0/careless.egg-info/SOURCES.txt` & `careless-0.3.1/careless.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,17 @@
 careless/models/scaling/image.py
 careless/models/scaling/nn.py
 careless/stats/__init__.py
 careless/stats/ccanom.py
 careless/stats/cchalf.py
 careless/stats/ccpred.py
 careless/stats/completeness.py
+careless/stats/parser.py
+careless/stats/prior_b.py
+careless/stats/rescale.py
 careless/stats/rsplit.py
 careless/utils/__init__.py
 careless/utils/device.py
 careless/utils/distributions.py
 careless/utils/laue.py
 careless/utils/positional_encoding.py
 careless/utils/shame.py
```

### Comparing `careless-0.3.0/scripts/make_difference_map` & `careless-0.3.1/scripts/make_difference_map`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/scripts/stream2mtz` & `careless-0.3.1/scripts/stream2mtz`

 * *Files identical despite different names*

### Comparing `careless-0.3.0/setup.py` & `careless-0.3.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     ],
     entry_points={
         "console_scripts": [
             "careless=careless.careless:main",
             "careless.ccanom=careless.stats.ccanom:main",
             "careless.cchalf=careless.stats.cchalf:main",
             "careless.ccpred=careless.stats.ccpred:main",
+            "careless.bfactor=careless.stats.prior_b:main",
+            "careless.apply_bfactor=careless.stats.rescale:main",
             "careless.completeness=careless.stats.completeness:main",
             "careless.rsplit=careless.stats.rsplit:main",
             "careless.xds2mtz=careless.io.xds:main",
         ]
     },
     setup_requires=["pytest-runner"],
     tests_require=["pytest", "pytest-cov", "pytest-xdist>=3"],
```

### Comparing `careless-0.3.0/tests/conftest.py` & `careless-0.3.1/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,17 +108,19 @@
         pad = len(refl_id) - len(intensities)
         intensities   = np.pad(intensities, [[0,pad],[0,0]])
         uncertainties = np.pad(uncertainties, [[0,pad],[0,0]], constant_values = 1./np.sqrt(np.pi * 2))
 
         self.data = ds
         self.reciprocal_asu = rasu
         self.reciprocal_asu_collection = rasu_collection
+        file_id = np.zeros_like(refl_id)
         self.inputs = [
             refl_id,
             image_id,
+            file_id,
             metadata,
             intensities,
             uncertainties,
             wavelength,
             harmonic_id
         ]
 
@@ -163,17 +165,19 @@
         ]].to_numpy('float32')
         intensities   = ds.I.to_numpy('float32')[:,None]
         uncertainties = ds.SigI.to_numpy('float32')[:,None]
 
         self.data = ds
         self.reciprocal_asu = rasu
         self.reciprocal_asu_collection = rasu_collection
+        file_id = np.zeros_like(refl_id)
         self.inputs = [
             refl_id,
             image_id,
+            file_id,
             metadata,
             intensities,
             uncertainties,
         ]
 
 mono_test_data = MonoTestData('data/pyp_off.mtz')
```

### Comparing `careless-0.3.0/tests/test_cli.py` & `careless-0.3.1/tests/test_cli.py`

 * *Files identical despite different names*

