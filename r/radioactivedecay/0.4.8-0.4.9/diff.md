# Comparing `tmp/radioactivedecay-0.4.8.tar.gz` & `tmp/radioactivedecay-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/radioactivedecay-0.4.8.tar", last modified: Wed Dec 15 10:03:26 2021, max compression
+gzip compressed data, was "dist/radioactivedecay-0.4.9.tar", last modified: Mon Feb  7 05:40:50 2022, max compression
```

## Comparing `radioactivedecay-0.4.8.tar` & `radioactivedecay-0.4.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 10:03:26.000000 radioactivedecay-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11336 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     5245 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     4657 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      704 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/LICENSE.AMDC
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/LICENSE.ICRP-07
--rw-r--r--   0 runner    (1001) docker     (121)      216 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14484 2021-12-15 10:03:26.000000 radioactivedecay-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10693 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       97 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 10:03:26.000000 radioactivedecay-0.4.8/radioactivedecay/
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22392 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/converters.py
--rw-r--r--   0 runner    (1001) docker     (121)    24852 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/decaydata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 10:03:26.000000 radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34304 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/atomic_masses_sympy_1.8.pickle
--rw-r--r--   0 runner    (1001) docker     (121)    53168 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/atomic_masses_sympy_1.9.pickle
--rw-r--r--   0 runner    (1001) docker     (121)    38046 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/c_inv_scipy.npz
--rw-r--r--   0 runner    (1001) docker     (121)   251346 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/c_inv_sympy_1.8.pickle
--rw-r--r--   0 runner    (1001) docker     (121)   237571 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/c_inv_sympy_1.9.pickle
--rw-r--r--   0 runner    (1001) docker     (121)    45592 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/c_scipy.npz
--rw-r--r--   0 runner    (1001) docker     (121)   269334 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/c_sympy_1.8.pickle
--rw-r--r--   0 runner    (1001) docker     (121)   248266 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/c_sympy_1.9.pickle
--rw-r--r--   0 runner    (1001) docker     (121)    32275 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/decay_consts_sympy_1.8.pickle
--rw-r--r--   0 runner    (1001) docker     (121)    43678 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/decay_consts_sympy_1.9.pickle
--rw-r--r--   0 runner    (1001) docker     (121)    65531 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/decay_data.npz
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/year_conversion_sympy_1.8.pickle
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/year_conversion_sympy_1.9.pickle
--rw-r--r--   0 runner    (1001) docker     (121)    53288 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/inventory.py
--rw-r--r--   0 runner    (1001) docker     (121)    13728 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/nuclide.py
--rw-r--r--   0 runner    (1001) docker     (121)     5467 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/plots.py
--rw-r--r--   0 runner    (1001) docker     (121)    10983 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/radioactivedecay/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 10:03:26.000000 radioactivedecay-0.4.8/radioactivedecay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14484 2021-12-15 10:03:25.000000 radioactivedecay-0.4.8/radioactivedecay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1695 2021-12-15 10:03:26.000000 radioactivedecay-0.4.8/radioactivedecay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-15 10:03:25.000000 radioactivedecay-0.4.8/radioactivedecay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2021-12-15 10:03:25.000000 radioactivedecay-0.4.8/radioactivedecay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-15 10:03:25.000000 radioactivedecay-0.4.8/radioactivedecay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1888 2021-12-15 10:03:26.000000 radioactivedecay-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 10:03:26.000000 radioactivedecay-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    36932 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (121)    24361 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/tests/test_decaydata.py
--rw-r--r--   0 runner    (1001) docker     (121)    32173 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/tests/test_inventory.py
--rw-r--r--   0 runner    (1001) docker     (121)     5090 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/tests/test_nuclide.py
--rw-r--r--   0 runner    (1001) docker     (121)     2727 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (121)     9160 2021-12-15 10:03:13.000000 radioactivedecay-0.4.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 05:40:50.000000 radioactivedecay-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    12186 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     5245 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     4657 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/LICENSE.AMDC
+-rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/LICENSE.ICRP-07
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    14511 2022-02-07 05:40:50.000000 radioactivedecay-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10712 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 05:40:50.000000 radioactivedecay-0.4.9/radioactivedecay/
+-rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15729 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/converters.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27562 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/decaydata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 05:40:50.000000 radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34304 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/atomic_masses_sympy_1.8.pickle
+-rw-r--r--   0 runner    (1001) docker     (121)    53168 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/atomic_masses_sympy_1.9.pickle
+-rw-r--r--   0 runner    (1001) docker     (121)    38046 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/c_inv_scipy.npz
+-rw-r--r--   0 runner    (1001) docker     (121)   251346 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/c_inv_sympy_1.8.pickle
+-rw-r--r--   0 runner    (1001) docker     (121)   237571 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/c_inv_sympy_1.9.pickle
+-rw-r--r--   0 runner    (1001) docker     (121)    45592 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/c_scipy.npz
+-rw-r--r--   0 runner    (1001) docker     (121)   269334 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/c_sympy_1.8.pickle
+-rw-r--r--   0 runner    (1001) docker     (121)   248266 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/c_sympy_1.9.pickle
+-rw-r--r--   0 runner    (1001) docker     (121)    32275 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/decay_consts_sympy_1.8.pickle
+-rw-r--r--   0 runner    (1001) docker     (121)    43678 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/decay_consts_sympy_1.9.pickle
+-rw-r--r--   0 runner    (1001) docker     (121)    65531 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/decay_data.npz
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/year_conversion_sympy_1.8.pickle
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/year_conversion_sympy_1.9.pickle
+-rw-r--r--   0 runner    (1001) docker     (121)    57263 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15231 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/nuclide.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5498 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/plots.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10978 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/radioactivedecay/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 05:40:50.000000 radioactivedecay-0.4.9/radioactivedecay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    14511 2022-02-07 05:40:50.000000 radioactivedecay-0.4.9/radioactivedecay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1695 2022-02-07 05:40:50.000000 radioactivedecay-0.4.9/radioactivedecay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 05:40:50.000000 radioactivedecay-0.4.9/radioactivedecay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-02-07 05:40:50.000000 radioactivedecay-0.4.9/radioactivedecay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-02-07 05:40:50.000000 radioactivedecay-0.4.9/radioactivedecay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-02-07 05:40:50.000000 radioactivedecay-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 05:40:50.000000 radioactivedecay-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36704 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24496 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/tests/test_decaydata.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31620 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/tests/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5273 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/tests/test_nuclide.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2727 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9160 2022-02-07 05:40:37.000000 radioactivedecay-0.4.9/tests/test_utils.py
```

### Comparing `radioactivedecay-0.4.8/CHANGELOG.md` & `radioactivedecay-0.4.9/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # Changelog
 
+## [0.4.9] - 2022-02-07
+- Code refactoring: reduce coupling between modules by refactoring Converter, Nuclide & Inventory
+classes to not store duplicate data, but to receive data when needed via their API calls. DecayData objects
+no longer store Converter objects. Continuing to reduce pylint/mypy errors/warnings, however will
+need to wait to bump requirement to Python 3.7+ to improve type hinting of NumPy/SciPy arrays
+(requires NumPy 1.20+, holding off for now to maintain Python 3.6 support) (#64, #66).
+- Improve API documentation table of contents & README fix (#66).
+- Better unit tests for DecayData class and error handling is instance does not contain SymPy data
+(#66).
+- Move dataset creation and comparison notebooks to separate repos within the radioactivedecay org
+on GitHub (#63).
+- Tweak GitHub Issue & PR markdown templates (#62).
+
 ## [0.4.8] - 2021-12-13
 - Fix some code bugs and make other improvements to the ReadMe and the Docs (#57, #58 & #59).
 - Reduce number of mypy errors, use Python f-strings everywhere (#60).
 - Fix the URL for the codecov badge in the ReadMe (#56 & #60).
 - Introduce GitHub Actions for CI/CD. Add Issue & Pull Request templates (#61).
 
 ## [0.4.7] - 2021-11-08
```

### Comparing `radioactivedecay-0.4.8/CODE_OF_CONDUCT.md` & `radioactivedecay-0.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `radioactivedecay-0.4.8/CONTRIBUTING.md` & `radioactivedecay-0.4.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `radioactivedecay-0.4.8/LICENSE` & `radioactivedecay-0.4.9/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2020-2021 Japan Atomic Energy Agency
+Copyright (c) 2020-2022 Japan Atomic Energy Agency
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `radioactivedecay-0.4.8/LICENSE.AMDC` & `radioactivedecay-0.4.9/LICENSE.AMDC`

 * *Files identical despite different names*

### Comparing `radioactivedecay-0.4.8/LICENSE.ICRP-07` & `radioactivedecay-0.4.9/LICENSE.ICRP-07`

 * *Files identical despite different names*

### Comparing `radioactivedecay-0.4.8/PKG-INFO` & `radioactivedecay-0.4.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radioactivedecay
-Version: 0.4.8
+Version: 0.4.9
 Summary: A Python package for radioactive decay modelling that supports 1252 radionuclides, decay chains, branching, and metastable states.
 Home-page: https://github.com/radioactivedecay/radioactivedecay
 Author: Alex Malins, Thom Lemoine, & contributors
 Author-email: github@alexmalinsREMOVETHIS.com
 License: MIT, ICRP-07, AMDC
 Project-URL: Bug Tracker, https://github.com/radioactivedecay/radioactivedecay/issues
 Project-URL: Discussions, https://github.com/radioactivedecay/radioactivedecay/discussions
@@ -32,15 +32,15 @@
         The code solves the radioactive decay differential equations analytically using
         NumPy and SciPy linear algebra routines. There is also a high numerical
         precision calculation mode employing SymPy routines. This gives more accurate
         results for decay chains containing radionuclides with orders of magnitude
         differences between the half-lives.
         
         This is free-to-use open source software. It was created for engineers,
-        technicians and researchers who work with and study radioactivity, and for
+        technicians and researchers who work with radioactivity, and for
         educational use.
         
         - **Full Documentation**: 
         [https://radioactivedecay.github.io/](https://radioactivedecay.github.io/)
         
         
         ## Installation
@@ -134,15 +134,17 @@
         ```pycon
         >>> Mo99_t0.plot(20, 'd', yunits='Bq')
         ```
         
         <img src="https://raw.githubusercontent.com/radioactivedecay/radioactivedecay/main/docs/source/images/Mo-99_decay.png" alt="Mo-99 decay graph" width="450"/>
         
         The graph shows the decay of Mo-99 over 20 days, leading to the ingrowth of
-        Tc-99m and a trace quantity of Tc-99. Graphs are drawn using Matplotlib.
+        Tc-99m and a trace quantity of Tc-99. The activity of Ru-99 is strictly zero as
+        it is the stable nuclide at the end of the decay chain. Graphs are drawn using
+        Matplotlib.
         
         
         ### Fetching decay data
         
         The ``Nuclide`` class can be used to fetch decay information for
         individual radionuclides, e.g. for Rn-222:
         
@@ -243,25 +245,24 @@
         
         By default ``radioactivedecay`` uses decay data from
         [ICRP Publication 107
         (2008)](https://journals.sagepub.com/doi/pdf/10.1177/ANIB_38_3) and atomic mass
         data from the [Atomic Mass Data Center](https://www-nds.iaea.org/amdc/)
         (AMDC - AME2020 and Nubase2020 evaluations).
         
-        The [notebooks
-        directory](https://github.com/radioactivedecay/radioactivedecay/tree/main/notebooks)
-        in the GitHub repository contains Jupyter Notebooks for creating the decay
-        datasets that are read in by ``radioactivedecay``, e.g.
-        [ICRP
-        107](https://github.com/radioactivedecay/radioactivedecay/tree/main/notebooks/icrp107_dataset/icrp107_dataset.ipynb).
-        It also contains some comparisons against decay calculations made with
-        [PyNE](https://github.com/radioactivedecay/radioactivedecay/tree/main/notebooks/comparisons/pyne/rd_pyne_truncated_compare.ipynb)
-        and
-        [Radiological
-        Toolbox](https://github.com/radioactivedecay/radioactivedecay/tree/main/notebooks/comparisons/radiological_toolbox/radiological_toolbox_compare.ipynb).
+        The [datasets repo](https://github.com/radioactivedecay/datasets) contains
+        Jupyter Notebooks for creating decay datasets that can be used by
+        ``radioactivedecay``, e.g. [ICRP
+        107](https://github.com/radioactivedecay/datasets/blob/main/icrp107_ame2020_nubase2020/icrp107_dataset.ipynb).
+        
+        The [comparisons repo](https://github.com/radioactivedecay/comparisons)
+        contains some checks of ``radioactivedecay`` against
+        [PyNE](https://github.com/radioactivedecay/comparisons/blob/main/pyne/rd_pyne_truncated_compare.ipynb)
+        and [Radiological
+        Toolbox](https://github.com/radioactivedecay/comparisons/blob/main/radiological_toolbox/radiological_toolbox_compare.ipynb).
         
         
         ## Tests
         
         From the base directory run:
         
         ```console
```

### Comparing `radioactivedecay-0.4.8/README.md` & `radioactivedecay-0.4.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 The code solves the radioactive decay differential equations analytically using
 NumPy and SciPy linear algebra routines. There is also a high numerical
 precision calculation mode employing SymPy routines. This gives more accurate
 results for decay chains containing radionuclides with orders of magnitude
 differences between the half-lives.
 
 This is free-to-use open source software. It was created for engineers,
-technicians and researchers who work with and study radioactivity, and for
+technicians and researchers who work with radioactivity, and for
 educational use.
 
 - **Full Documentation**: 
 [https://radioactivedecay.github.io/](https://radioactivedecay.github.io/)
 
 
 ## Installation
@@ -122,15 +122,17 @@
 ```pycon
 >>> Mo99_t0.plot(20, 'd', yunits='Bq')
 ```
 
 <img src="https://raw.githubusercontent.com/radioactivedecay/radioactivedecay/main/docs/source/images/Mo-99_decay.png" alt="Mo-99 decay graph" width="450"/>
 
 The graph shows the decay of Mo-99 over 20 days, leading to the ingrowth of
-Tc-99m and a trace quantity of Tc-99. Graphs are drawn using Matplotlib.
+Tc-99m and a trace quantity of Tc-99. The activity of Ru-99 is strictly zero as
+it is the stable nuclide at the end of the decay chain. Graphs are drawn using
+Matplotlib.
 
 
 ### Fetching decay data
 
 The ``Nuclide`` class can be used to fetch decay information for
 individual radionuclides, e.g. for Rn-222:
 
@@ -231,25 +233,24 @@
 
 By default ``radioactivedecay`` uses decay data from
 [ICRP Publication 107
 (2008)](https://journals.sagepub.com/doi/pdf/10.1177/ANIB_38_3) and atomic mass
 data from the [Atomic Mass Data Center](https://www-nds.iaea.org/amdc/)
 (AMDC - AME2020 and Nubase2020 evaluations).
 
-The [notebooks
-directory](https://github.com/radioactivedecay/radioactivedecay/tree/main/notebooks)
-in the GitHub repository contains Jupyter Notebooks for creating the decay
-datasets that are read in by ``radioactivedecay``, e.g.
-[ICRP
-107](https://github.com/radioactivedecay/radioactivedecay/tree/main/notebooks/icrp107_dataset/icrp107_dataset.ipynb).
-It also contains some comparisons against decay calculations made with
-[PyNE](https://github.com/radioactivedecay/radioactivedecay/tree/main/notebooks/comparisons/pyne/rd_pyne_truncated_compare.ipynb)
-and
-[Radiological
-Toolbox](https://github.com/radioactivedecay/radioactivedecay/tree/main/notebooks/comparisons/radiological_toolbox/radiological_toolbox_compare.ipynb).
+The [datasets repo](https://github.com/radioactivedecay/datasets) contains
+Jupyter Notebooks for creating decay datasets that can be used by
+``radioactivedecay``, e.g. [ICRP
+107](https://github.com/radioactivedecay/datasets/blob/main/icrp107_ame2020_nubase2020/icrp107_dataset.ipynb).
+
+The [comparisons repo](https://github.com/radioactivedecay/comparisons)
+contains some checks of ``radioactivedecay`` against
+[PyNE](https://github.com/radioactivedecay/comparisons/blob/main/pyne/rd_pyne_truncated_compare.ipynb)
+and [Radiological
+Toolbox](https://github.com/radioactivedecay/comparisons/blob/main/radiological_toolbox/radiological_toolbox_compare.ipynb).
 
 
 ## Tests
 
 From the base directory run:
 
 ```console
```

### Comparing `radioactivedecay-0.4.8/radioactivedecay/__init__.py` & `radioactivedecay-0.4.9/radioactivedecay/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 The code solves the radioactive decay differential equations analytically using
 NumPy and SciPy linear algebra routines. There is also a high numerical
 precision calculation mode employing SymPy routines. This gives more accurate
 results for decay chains containing radionuclides with orders of magnitude
 differences between the half-lives.
 
 This is free-to-use open source software. It was created for engineers,
-technicians and researchers who work with and study radioactivity, and for
+technicians and researchers who work with radioactivity, and for
 educational use.
 
 The docstring code examples assume the ``radioactivedecay`` package has been
-imported as:
+imported as ``rd``:
 
 .. highlight:: python
 .. code-block:: python
 
     >>> import radioactivedecay as rd
 
 """
 
-__version__ = "0.4.8"
+__version__ = "0.4.9"
 
 from radioactivedecay.decaydata import DecayData, DEFAULTDATA
 from radioactivedecay.inventory import Inventory, InventoryHP
 from radioactivedecay.nuclide import Nuclide
```

### Comparing `radioactivedecay-0.4.8/radioactivedecay/decaydata.py` & `radioactivedecay-0.4.9/radioactivedecay/decaydata.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 """
-The decaydata module defines the ``DecayData``, ``DecayMatrices`` and ``DecayMatricesSympy``
-classes. ``DecayMatrices`` and ``DecayMatricesSympy`` instances store data used for decay
+The decaydata module defines the ``DecayData``, ``DecayMatricesScipy`` and ``DecayMatricesSympy``
+classes. ``DecayMatricesScipy`` and ``DecayMatricesSympy`` instances store data used for decay
 calculations and other inventory transformations (using double-precision floating point and SymPy
-arbitrary precision numbers, respectively). ``DecayData`` instances store ``DecayMatrices``,
+arbitrary precision numbers, respectively). ``DecayData`` instances store ``DecayMatricesScipy``,
 ``DecayMatricesSympy`` and unit converter objects, along with other decay data for reporting to
 users (this data is not used for calculations).
 
 The docstring code examples assume that ``radioactivedecay`` has been imported
-as `rd`:
+as ``rd``:
 
 .. highlight:: python
 .. code-block:: python
 
     >>> import radioactivedecay as rd
 
 Constants
 ---------
 DEFAULTDATA : DecayData
     Default radioactive decay dataset used by ``radioactivedecay``. This is currently ICRP-107 for
     decay data and AME2020 and Nubase2020 for atomic mass data.
 """
 
+from abc import ABC, abstractmethod
 from pathlib import Path
 import pickle
 from typing import Any, ContextManager, Optional, Union
 import numpy as np
 from scipy import sparse
 import sympy
 from sympy import Matrix
 from sympy.matrices import SparseMatrix
-from radioactivedecay.converters import (
-    UnitConverterFloat,
-    UnitConverterSympy,
-    QuantityConverter,
-    QuantityConverterSympy,
-)
+from sympy.core.expr import Expr
+from radioactivedecay.converters import UnitConverterFloat
 from radioactivedecay.utils import parse_nuclide
 
+
+# importlib.resources is new in Python version 3.7
+# this block adds support using a backport for Python <3.7
+# the except block and dependency can be removed once min required Python version is 3.7
 try:
     from importlib import resources
 except ImportError:
     import importlib_resources as resources  # type:ignore
 
 
 def _csr_matrix_equal(matrix_a: sparse.csr_matrix, matrix_b: sparse.csr_matrix) -> bool:
     """
-    Checks whether two SciPy Compressed Sparse Row (CSR) matrices are equal (i.e. they have the
-    same elements and all elements are equal).
+    Utility function checking whether two SciPy Compressed Sparse Row (CSR) matrices are equal
+    (i.e. they have the same elements and all elements are equal).
 
     Parameters
     ----------
     matrix_a : scipy.sparse.csr.csr_matrix
         First SciPy CSR matrix.
     matrix_b : scipy.sparse.csr.csr_matrix
         Second SciPy CSR matrix.
@@ -64,133 +65,202 @@
     return (
         np.array_equal(matrix_a.indptr, matrix_b.indptr)
         and np.array_equal(matrix_a.indices, matrix_b.indices)
         and np.array_equal(matrix_a.data, matrix_b.data)
     )
 
 
-class DecayMatrices:
+class DecayMatrices(ABC):
     """
-    Instances of DecayMatrices store vectors with fundamental decay/atomic data and matrices used
-    for decay calculations.
+    Template class for for SciPy (float) or SymPy DecayMatrices classes. Instances of these classes
+    store vectors and matrices of data used for decay calculations.
 
     Parameters
     ----------
-    atomic_masses : numpy.ndarray
+    atomic_masses : numpy.ndarray or sympy.matrices.dense.MutableSparseMatrix
         Column vector of the atomic masses (in g/mol).
-    decay_consts : numpy.ndarray
+    decay_consts : numpy.ndarray or sympy.matrices.dense.MutableSparseMatrix
         Column vector of the decay constants (in s\\ :sup:`-1`).
-    matrix_c : scipy.sparse.csr.csr_matrix
+    matrix_c : scipy.sparse.csr.csr_matrix or sympy.matrices.dense.MutableSparseMatrix
         A pre-calculated sparse lower traingular matrix used in decay calculations.
-    matrix_c_inv : scipy.sparse.csr.csr_matrix
+    matrix_c_inv : scipy.sparse.csr.csr_matrix or sympy.matrices.dense.MutableSparseMatrix
         The inverse of matrix_c, also used in decay calculations.
 
     Attributes
     ----------
-    atomic_masses : numpy.ndarray
+    atomic_masses : numpy.ndarray or sympy.matrices.dense.MutableSparseMatrix
         Column vector of the atomic masses (in g/mol).
-    decay_consts : numpy.ndarray
+    decay_consts : numpy.ndarray or sympy.matrices.dense.MutableSparseMatrix
         Column vector of the decay constants (in s\\ :sup:`-1`).
-    ln2: float
+    ln2: float or sympy.log
         Constant natural logarithm of 2.
-    matrix_c : scipy.sparse.csr.csr_matrix
+    matrix_c : scipy.sparse.csr.csr_matrix or sympy.matrices.dense.MutableSparseMatrix
         A precalculated sparse lower triangular matrix used in decay calculations.
-    matrix_c_inv : scipy.sparse.csr.csr_matrix
+    matrix_c_inv : scipy.sparse.csr.csr_matrix or sympy.matrices.dense.MutableSparseMatrix
         The inverse of matrix_c, also used in decay calculations.
-    matrix_e : scipy.sparse.csr.csr_matrix
+    matrix_e : scipy.sparse.csr.csr_matrix or sympy.matrices.dense.MutableSparseMatrix
         The matrix exponential that is used in radioactive decay calculations. It is a diagonal
         matrix that is pre-allocted for performance reasons.
-    vector_n0 : numpy.ndarray
+    vector_n0 : numpy.ndarray or sympy.matrices.dense.MutableDenseMatrix
         Column vector for the number of atoms of each nuclide. It is pre-allocted here to improve
         the performance of decay calculations.
 
     """
 
     def __init__(
         self,
-        atomic_masses: np.ndarray,
-        decay_consts: np.ndarray,
-        matrix_c: sparse.csr_matrix,
-        matrix_c_inv: sparse.csr_matrix,
+        atomic_masses: Union[np.ndarray, Matrix],
+        decay_consts: Union[np.ndarray, Matrix],
+        matrix_c: Union[sparse.csr_matrix, Matrix],
+        matrix_c_inv: Union[sparse.csr_matrix, Matrix],
     ) -> None:
         self.atomic_masses = atomic_masses
         self.decay_consts = decay_consts
         self.ln2 = self._setup_ln2()
         self.matrix_c = matrix_c
         self.matrix_c_inv = matrix_c_inv
         self.matrix_e = self._setup_matrix_e(matrix_c.shape[0])
         self.vector_n0 = self._setup_vector_n0(matrix_c.shape[0])
 
     @staticmethod
+    @abstractmethod
     def _setup_ln2() -> float:
         """
-        Returns NumPy ln2.
+        Set up natural log of 2 (ln(2)).
+        """
+
+    @staticmethod
+    @abstractmethod
+    def _setup_matrix_e(size: int) -> Union[sparse.csr_matrix, Matrix]:
+        """
+        Set up sparse matrix_e (created here rather than at decay calculation time
+        for performance reasons).
+        """
+
+    @staticmethod
+    @abstractmethod
+    def _setup_vector_n0(size: int) -> Union[np.ndarray, Matrix]:
+        """
+        Set up vector_n0 (created here rather than at decay calculation time for performance
+        reasons).
+        """
+
+    @abstractmethod
+    def __eq__(self, other: object) -> bool:
+        """
+        Check whether two ``DecayMatrices`` instances are equal with ``==`` operator.
+        """
+
+    def __ne__(self, other: object) -> bool:
+        """
+        Check whether two ``DecayMatrices`` instances are not equal with ``!=`` operator.
+        """
+
+        if not isinstance(other, self.__class__):
+            return NotImplemented
+        return not self.__eq__(other)
+
+
+class DecayMatricesScipy(DecayMatrices):
+    """
+    Version of DecayMatrices with data for SciPy double-precision floating point decay
+    calculations.
+
+    Parameters
+    ----------
+    atomic_masses : numpy.ndarray
+        Column vector of the atomic masses (in g/mol).
+    decay_consts : numpy.ndarray
+        Column vector of the decay constants (in s\\ :sup:`-1`).
+    matrix_c : scipy.sparse.csr.csr_matrix
+        A pre-calculated sparse lower traingular matrix used in decay calculations.
+    matrix_c_inv : scipy.sparse.csr.csr_matrix
+        The inverse of matrix_c, also used in decay calculations.
+
+    Attributes
+    ----------
+    atomic_masses : numpy.ndarray
+        Column vector of the atomic masses (in g/mol).
+    decay_consts : numpy.ndarray
+        Column vector of the decay constants (in s\\ :sup:`-1`).
+    ln2: float
+        Constant natural logarithm of 2.
+    matrix_c : scipy.sparse.csr.csr_matrix
+        A precalculated sparse lower triangular matrix used in decay calculations.
+    matrix_c_inv : scipy.sparse.csr.csr_matrix
+        The inverse of matrix_c, also used in decay calculations.
+    matrix_e : scipy.sparse.csr.csr_matrix
+        The matrix exponential that is used in radioactive decay calculations. It is a diagonal
+        matrix that is pre-allocted for performance reasons.
+    vector_n0 : numpy.ndarray
+        Column vector for the number of atoms of each nuclide. It is pre-allocted here to improve
+        the performance of decay calculations.
+
+    """
+
+    @staticmethod
+    def _setup_ln2() -> float:
+        """
+        Set up natural log of 2 (ln(2)).
         """
 
         log2: float = np.log(2)
         return log2
 
     @staticmethod
     def _setup_matrix_e(size: int) -> sparse.csr_matrix:
         """
-        Returns SciPy CSR sparse matrix template for matrix_e.
+        Set up sparse matrix_e (created here rather than at decay calculation time
+        for performance reasons).
         """
 
         return sparse.csr_matrix(
             (
                 np.zeros(size),
                 (np.arange(size), np.arange(size)),
             )
         )
 
     @staticmethod
     def _setup_vector_n0(size: int) -> np.ndarray:
         """
-        Returns NumPy array template for vector_n0.
+        Set up vector_n0 (created here rather than at decay calculation time for performance
+        reasons).
         """
 
         return np.zeros([size], dtype=np.float64)
 
     def __eq__(self, other: object) -> bool:
         """
-        Check whether two ``DecayMatrices`` instances are equal with ``==`` operator.
+        Check whether two ``DecayMatricesScipy`` instances are equal with ``==`` operator.
         """
 
-        if not isinstance(other, DecayMatrices):
+        if not isinstance(other, self.__class__):
             return NotImplemented
         return (
             np.array_equal(self.atomic_masses, other.atomic_masses)
             and np.array_equal(self.decay_consts, other.decay_consts)
             and self.ln2 == other.ln2
             and _csr_matrix_equal(self.matrix_c, other.matrix_c)
             and _csr_matrix_equal(self.matrix_c_inv, other.matrix_c_inv)
             and _csr_matrix_equal(self.matrix_e, other.matrix_e)
             and np.array_equal(self.vector_n0, other.vector_n0)
         )
 
-    def __ne__(self, other: object) -> bool:
-        """
-        Check whether two ``DecayMatrices`` instances are not equal with ``!=`` operator.
-        """
-
-        if not isinstance(other, DecayMatrices):
-            return NotImplemented
-        return not self.__eq__(other)
-
     def __repr__(self) -> str:
 
         return (
-            "DecayMatrices: data stored in SciPy/NumPy objects for double precision "
+            "DecayMatricesScipy: data stored in SciPy/NumPy objects for double precision "
             "calculations."
         )
 
 
 class DecayMatricesSympy(DecayMatrices):
     """
-    Version of DecayMatrices using SymPy arbitrary precision operations.
+    Version of DecayMatrices with data for SymPy arbitrary precision decay calculations.
 
     Parameters
     ----------
     atomic_masses : sympy.matrices.dense.MutableDenseMatrix
         Column vector of the atomic masses (in g/mol).
     decay_consts : sympy.matrices.dense.MutableDenseMatrix
         Column vector of the decay constants (in s\\ :sup:`-1`).
@@ -268,120 +338,121 @@
             "calculations."
         )
 
 
 class DecayData:
     """
     Instances of DecayData store a complete radioactive decay dataset. It stores data for decay
-    calculations, inventory transformations and unit conversions using DecayMatrices,
-    UnitConverterFloat, QuantityConverter, DecayMatricesSympy, UnitConverterSympy and
-    QuantityConverterSympy objects. Other decay data which are reported to users but not used in
-    calculations are stored in other instance attributes.
+    calculations and inventory transformations using DecayMatrices attributes. Other decay data
+    which are reported to users but not used incalculations are stored in other instance
+    attributes.
 
     Parameters
     ----------
     dataset_name : str
         Name of the decay dataset.
     bfs : numpy.ndarray
         NumPy array of lists with branching fraction data.
+    float_year_conv : float
+        Number of days in one year for float time unit conversions.
     hldata : numpy.ndarray
         List of tuples containing half-life floats, time unit strings and readable format half-life
         strings.
     modes : numpy.ndarray
         NumPy array of lists with decay mode data.
     nuclides : numpy.ndarray
         NumPy array of nuclides in the dataset (string format is 'H-3', etc.).
     progeny : numpy.ndarray
         NumPy array of lists with direct progeny data.
-    scipy_data : DecayMatrices
+    scipy_data : DecayMatricesScipy
         Dataset of double precision decay matrices (SciPy/NumPy objects).
-    float_unit_converter : UnitConverterFloat
-        Convert between units of a single quantity using floating point operations.
     sympy_data : None or DecayMatricesSympy
         Dataset of arbitrary-precision decay matrices (SymPy objects). Or None if SymPy
         functionality is not used. Default is None.
-    sympy_unit_converter : None or UnitConverterSympy
-        Convert between units of a single quantity using SymPy arbitrary precision operations.
-        Default is None.
+    sympy_year_conv : None or Expr
+        Number of days in one year for SymPy time unit conversions.
 
     Attributes
     ----------
     bfs : numpy.ndarray
         NumPy array of lists with branching fraction data.
     dataset_name : str
         Name of the decay dataset.
-    float_quantity_converter : QuantityConverter
-        Convert between quantities using floating point operations.
-    float_unit_converter : UnitConverterFloat
-        Convert between units of a single quantity using floating point operations.
+    float_year_conv : float
+        Number of days in one year for float time unit conversions.
     hldata : numpy.ndarray
         List of tuples containing half-life floats, time unit strings and readable format half-life
         strings.
     modes : numpy.ndarray
         NumPy array of lists with decay mode data.
     nuclides : numpy.ndarray
         NumPy array of nuclides in the dataset (string format is 'H-3', etc.).
     nuclide_dict : dict
         Dictionary containing nuclide strings as keys and positions in the matrices as values.
     progeny : numpy.ndarray
         NumPy array of lists with direct progeny data.
-    scipy_data : DecayMatrices
+    _scipy_data : DecayMatricesScipy
         Dataset of double precision decay matrices (SciPy/NumPy objects).
-    sympy_data : None or DecayMatricesSympy
-        Dataset of arbitrary-precision decay matrices (SymPy objects). Or None if this functionality
-        is not used.
-    sympy_quantity_converter : None or QuantityConverterSympy
-        Convert between quantities using SymPy arbitrary precision operations.
-    sympy_unit_converter : None or UnitConverterSympy
-        Convert between units of a single quantity using SymPy arbitrary precision operations.
+    _sympy_year_conv : None or Expr
+        Number of days in one year for SymPy time unit conversions.
 
     """
 
     def __init__(
         self,
         dataset_name: str,
         bfs: np.ndarray,
+        float_year_conv: float,
         hldata: np.ndarray,
         modes: np.ndarray,
         nuclides: np.ndarray,
         progeny: np.ndarray,
-        scipy_data: DecayMatrices,
-        float_unit_converter: UnitConverterFloat,
+        scipy_data: DecayMatricesScipy,
         sympy_data: Optional[DecayMatricesSympy] = None,
-        sympy_unit_converter: Optional[UnitConverterSympy] = None,
+        sympy_year_conv: Optional[Expr] = None,
     ) -> None:
 
         self.dataset_name = dataset_name
         self.bfs = bfs
-        self.float_unit_converter = float_unit_converter
+        self.float_year_conv = float_year_conv
         self.hldata = hldata
         self.modes = modes
         self.nuclides = nuclides
         self.nuclide_dict = dict(zip(self.nuclides, list(range(0, self.nuclides.size))))
         self.progeny = progeny
         self.scipy_data = scipy_data
 
-        self.float_quantity_converter = QuantityConverter(
-            self.nuclide_dict,
-            self.scipy_data.atomic_masses,
-            self.scipy_data.decay_consts,
-        )
-
-        self.sympy_data: Optional[DecayMatricesSympy] = None
-        self.sympy_unit_converter: Optional[UnitConverterSympy] = None
-        self.sympy_quantity_converter: Optional[QuantityConverterSympy] = None
-
-        if sympy_data and sympy_unit_converter:
-            self.sympy_data = sympy_data
-            self.sympy_unit_converter = sympy_unit_converter
-            self.sympy_quantity_converter = QuantityConverterSympy(
-                self.nuclide_dict,
-                self.sympy_data.atomic_masses,
-                self.sympy_data.decay_consts,
-            )
+        self._sympy_data: Optional[DecayMatricesSympy] = None
+        self._sympy_year_conv: Optional[Expr] = None
+
+        if sympy_data and sympy_year_conv:
+            self._sympy_data = sympy_data
+            self._sympy_year_conv = sympy_year_conv
+
+    @property
+    def sympy_data(self) -> DecayMatricesSympy:
+        """
+        Property to return DecayMatricesSympy instance if it exists, or raise an error if the
+        dataset does not contain SymPy data.
+        """
+
+        if self._sympy_data is None:
+            raise ValueError(f"{self.dataset_name} does not contain SymPy data.")
+        return self._sympy_data
+
+    @property
+    def sympy_year_conv(self) -> Expr:
+        """
+        Property to return SymPy number of days in one year if it exists, or raise an error if the
+        dataset does not contain SymPy data.
+        """
+
+        if self._sympy_year_conv is None:
+            raise ValueError(f"{self.dataset_name} does not contain SymPy data.")
+        return self._sympy_year_conv
 
     def half_life(self, nuclide: str, units: str = "s") -> Union[float, str]:
         """
         Returns the half-life of the nuclide as a float in your chosen units, or as
         a human-readable string with appropriate units.
 
         Parameters
@@ -421,18 +492,19 @@
 
         if units == "readable":
             return readable_str
 
         return (
             half_life
             if unit == units
-            else self.float_unit_converter.time_unit_conv(
+            else UnitConverterFloat.time_unit_conv(
                 half_life,
                 units_from=unit,
                 units_to=units,
+                year_conv=self.float_year_conv,
             )
         )
 
     def branching_fraction(self, parent: str, progeny: str) -> float:
         """
         Returns the branching fraction for parent to progeny (if it exists).
 
@@ -502,39 +574,39 @@
         Check whether two ``DecayData`` instances are equal with ``==`` operator.
         """
 
         if not isinstance(other, DecayData):
             return NotImplemented
         return (
             self.dataset_name == other.dataset_name
-            and self.float_unit_converter == other.float_unit_converter
+            and self.float_year_conv == other.float_year_conv
             and np.array_equal(self.hldata, other.hldata)
             and np.array_equal(self.nuclides, other.nuclides)
             and self.nuclide_dict == other.nuclide_dict
             and np.array_equal(self.progeny, other.progeny)
             and np.array_equal(self.bfs, other.bfs)
             and np.array_equal(self.modes, other.modes)
             and self.scipy_data == other.scipy_data
-            and self.sympy_data == other.sympy_data
-            and self.sympy_unit_converter == other.sympy_unit_converter
+            and self._sympy_data == other._sympy_data
+            and self._sympy_year_conv == other._sympy_year_conv
         )
 
     def __ne__(self, other: object) -> bool:
         """
         Check whether two ``DecayData`` instances are not equal with ``!=`` operator.
         """
 
         if not isinstance(other, DecayData):
             return NotImplemented
         return not self.__eq__(other)
 
     def __repr__(self) -> str:
         return (
             f"Decay dataset: {self.dataset_name}, contains SymPy data: "
-            f"{self.sympy_data is not None}"
+            f"{self._sympy_data is not None}"
         )
 
 
 def _get_package_filepath(subpackage_dir: str, filename: str) -> ContextManager[Path]:
     """
     Returns the path to a file which is bundled as a sub-package within the
     ``radioactivedecay`` package.
@@ -665,32 +737,35 @@
     """
 
     data = np.load(
         _get_filepath(dataset_name, dir_path, "decay_data.npz"),
         allow_pickle=True,
     )
 
-    float_unit_converter = UnitConverterFloat(data["year_conv"])
-    decay_consts = np.array(
+    decay_consts: np.ndarray = np.array(
         [
             np.log(2)
-            / float_unit_converter.time_unit_conv(hl[0], units_from=hl[1], units_to="s")
+            / UnitConverterFloat.time_unit_conv(
+                hl[0], units_from=hl[1], units_to="s", year_conv=data["year_conv"]
+            )
             for hl in data["hldata"]
         ]
     )
 
     matrix_c = sparse.load_npz(_get_filepath(dataset_name, dir_path, "c_scipy.npz"))
     matrix_c_inv = sparse.load_npz(
         _get_filepath(dataset_name, dir_path, "c_inv_scipy.npz")
     )
 
-    scipy_data = DecayMatrices(data["masses"], decay_consts, matrix_c, matrix_c_inv)
+    scipy_data = DecayMatricesScipy(
+        data["masses"], decay_consts, matrix_c, matrix_c_inv
+    )
 
     sympy_data = None
-    sympy_unit_converter = None
+    sympy_year_conv = None
     if load_sympy:
         sympy_pickle_version = "1.9" if sympy.__version__ >= "1.9" else "1.8"
 
         atomic_masses = _load_pickle_file(
             dataset_name, dir_path, f"atomic_masses_sympy_{sympy_pickle_version}.pickle"
         )
         decay_consts = _load_pickle_file(
@@ -698,32 +773,31 @@
         )
         matrix_c = _load_pickle_file(
             dataset_name, dir_path, f"c_sympy_{sympy_pickle_version}.pickle"
         )
         matrix_c_inv = _load_pickle_file(
             dataset_name, dir_path, f"c_inv_sympy_{sympy_pickle_version}.pickle"
         )
-        year_conv_sympy = _load_pickle_file(
+        sympy_year_conv = _load_pickle_file(
             dataset_name,
             dir_path,
             f"year_conversion_sympy_{sympy_pickle_version}.pickle",
         )
         sympy_data = DecayMatricesSympy(
             atomic_masses, decay_consts, matrix_c, matrix_c_inv
         )
-        sympy_unit_converter = UnitConverterSympy(year_conv_sympy)
 
     return DecayData(
         dataset_name,
         data["bfs"],
+        data["year_conv"],
         data["hldata"],
         data["modes"],
         data["nuclides"],
         data["progeny"],
         scipy_data,
-        float_unit_converter,
         sympy_data,
-        sympy_unit_converter,
+        sympy_year_conv,
     )
 
 
 DEFAULTDATA = load_dataset("icrp107_ame2020_nubase2020", load_sympy=True)
```

### Comparing `radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/atomic_masses_sympy_1.8.pickle` & `radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/atomic_masses_sympy_1.8.pickle`

 * *Files identical despite different names*

### Comparing `radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/atomic_masses_sympy_1.9.pickle` & `radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/atomic_masses_sympy_1.9.pickle`

 * *Files identical despite different names*

### Comparing `radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/c_inv_scipy.npz` & `radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/c_inv_scipy.npz`

 * *Files identical despite different names*

### Comparing `radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/c_inv_sympy_1.8.pickle` & `radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/c_inv_sympy_1.8.pickle`

 * *Files identical despite different names*

### Comparing `radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/c_inv_sympy_1.9.pickle` & `radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/c_inv_sympy_1.9.pickle`

 * *Files identical despite different names*

### Comparing `radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/c_scipy.npz` & `radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/c_scipy.npz`

 * *Files identical despite different names*

### Comparing `radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/c_sympy_1.8.pickle` & `radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/c_sympy_1.8.pickle`

 * *Files identical despite different names*

### Comparing `radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/c_sympy_1.9.pickle` & `radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/c_sympy_1.9.pickle`

 * *Files identical despite different names*

### Comparing `radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/decay_consts_sympy_1.8.pickle` & `radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/decay_consts_sympy_1.8.pickle`

 * *Files identical despite different names*

### Comparing `radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/decay_consts_sympy_1.9.pickle` & `radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/decay_consts_sympy_1.9.pickle`

 * *Files identical despite different names*

### Comparing `radioactivedecay-0.4.8/radioactivedecay/icrp107_ame2020_nubase2020/decay_data.npz` & `radioactivedecay-0.4.9/radioactivedecay/icrp107_ame2020_nubase2020/decay_data.npz`

 * *Files identical despite different names*

### Comparing `radioactivedecay-0.4.8/radioactivedecay/inventory.py` & `radioactivedecay-0.4.9/radioactivedecay/inventory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,74 +1,85 @@
 """
-The inventory module defines the ``Inventory`` class. An ``Inventory`` instance contains one or
-more nuclides each with an associated amount (number of atoms). The decay of the nuclide(s) in an
-``Inventory`` can be calculated by using the ``decay()`` method (normal double-precision
-floating-point operations). The corresponding ``InventoryHP`` class performs decay calculations
-with SymPy high numerical precision operations. A ``DecayData`` dataset is associated with
-``Inventory`` and ``InventoryHP`` instances (default is rd.DEFAULTDATA).
+The inventory module defines the ``Inventory`` and ``InventoryHP`` classes. Instances of these
+classes contain one or more nuclides each with an associated amount (number of atoms). The decay
+of the nuclide(s) can be calculated by using the ``decay()`` method. The ``Inventory`` class
+performs calculations using double-precision floats. The ``InventoryHP`` class performs
+calculations using SymPy high numerical precision operations. A ``DecayData`` dataset is associated
+with ``Inventory`` and ``InventoryHP`` instances (default is rd.DEFAULTDATA).
 
 The docstring code examples assume that ``radioactivedecay`` has been imported
-as `rd`:
+as ``rd``:
 
 .. highlight:: python
 .. code-block:: python
 
     >>> import radioactivedecay as rd
 
 """
 
-from functools import singledispatch, update_wrapper
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from abc import ABC, abstractmethod
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
 import matplotlib
 import numpy as np
 from scipy import sparse
 from sympy import exp, Integer, Matrix, nsimplify
 from sympy.core.expr import Expr
 from radioactivedecay.converters import (
     QuantityConverter,
+    QuantityConverterFloat,
     QuantityConverterSympy,
+    UnitConverter,
     UnitConverterFloat,
     UnitConverterSympy,
 )
 from radioactivedecay.decaydata import (
     DecayData,
     DecayMatrices,
+    DecayMatricesScipy,
     DecayMatricesSympy,
     DEFAULTDATA,
 )
-from radioactivedecay.plots import _decay_graph
+from radioactivedecay.plots import decay_graph
 from radioactivedecay.nuclide import Nuclide
 from radioactivedecay.utils import (
     parse_nuclide,
     add_dictionaries,
     sort_dictionary_alphabetically,
     sort_list_according_to_dataset,
 )
 
+# functools.singledispatchmethod is new in Python version 3.8
+# this block adds support manually for Python <3.8
+# the except block can be removed once min required Python version is 3.8
+try:
+    from functools import singledispatchmethod
+except ImportError:
+    from functools import singledispatch, update_wrapper
+
+    def singledispatchmethod(func: Callable[..., Any]):  # type:ignore
+        """Adds singledispatch support for instance methods of a class."""
+
+        dispatcher = singledispatch(func)
+
+        def wrapper(*args, **kwargs):  # type:ignore
+            return dispatcher.dispatch(args[1].__class__)(*args, **kwargs)
+
+        wrapper.register = dispatcher.register
+        update_wrapper(wrapper, func)
+        return wrapper
 
-# pylint: disable=too-many-arguments, too-many-lines, too-many-locals
-
-
-def _method_dispatch(func: Callable[..., Any]):
-    """Adds singledispatch support for class methods."""
-
-    dispatcher = singledispatch(func)
-
-    def wrapper(*args, **kwargs):
-        return dispatcher.dispatch(args[1].__class__)(*args, **kwargs)
 
-    wrapper.register = dispatcher.register
-    update_wrapper(wrapper, func)
-    return wrapper
+# pylint: disable=too-many-arguments, too-many-lines, too-many-locals
 
 
-class Inventory:
+class AbstractInventory(ABC):
     """
-    ``Inventory`` instances store nuclides and associated quantities (numbers of atoms) in the
-    contents dictionary. Each instance is associated with a decay dataset.
+    Template class for float (SciPy) or SymPy Inventory classes. Each AbstractInventory instance
+    stores nuclides and associated quantities (numbers of atoms) in the contents dictionary. A
+    decay dataset is associated with each instance.
 
     Parameters
     ----------
     contents : dict
         Dictionary containing nuclide strings/canonical ids or Nuclide instances as keys and
         quantities (activities, number of atoms, masses or moles) as values.
     units : str, optional
@@ -85,56 +96,40 @@
     ----------
     contents : dict
         Dictionary containing nuclide strings as keys and number of atoms of each nuclide as
         values. Nuclides are sorted alphabetically in this dictionary.
     decay_data : DecayData
         Decay dataset.
     decay_matrices : DecayMatrices
-        Float/SciPy version of the DecayMatrices associated with the decay dataset.
-    quantity_converter : QuantityConverter
-        Float/SciPy version of a convertor between different quantities.
-    unit_converter : UnitConverterFloat
-        Float version of a convertor for within different units.
-
-    Examples
-    --------
-    >>> rd.Inventory({'Tc-99m': 2.3, 'I-123': 5.8}, 'Bq')
-    Inventory activities (Bq): {'I-123': 2.3, 'Tc-99m': 5.8}, decay dataset: icrp107_ame2020_nubase2020
-    >>> H3 = rd.Nuclide('H-3')
-    >>> rd.Inventory({H3: 3.0}, 'g')
-    Inventory activities (Bq): {'H-3': 1067957043281807.0}, decay dataset: icrp107_ame2020_nubase2020
-    >>> rd.Inventory({270570000: 7.2, 922380000: 21.1}, 'Ci')
-    Inventory activities (Bq): {'Co-57': 266400000000.0, 'U-238': 780700000000.0001}, decay dataset: icrp107_ame2020_nubase2020
+        SciPy or SymPy version of a DecayMatrices instance associated with the decay dataset.
 
     """
 
     def __init__(
         self,
-        contents: Dict[Union[str, int, Nuclide], float],
+        contents: Dict[Union[str, int, Nuclide], Union[float, Expr]],
         units: str = "Bq",
         check: bool = True,
         decay_data: DecayData = DEFAULTDATA,
     ) -> None:
 
         self.decay_data = decay_data
         self.decay_matrices = self._get_decay_matrices()
-        self.quantity_converter = self._get_quantity_converter()
-        self.unit_converter = self._get_unit_converter()
 
         if check is True:
-            contents_with_parsed_keys: Dict[str, float] = self._parse_nuclides(
+            contents_with_parsed_keys: Dict[
+                str, Union[float, Expr]
+            ] = self._parse_nuclides(
                 contents, self.decay_data.nuclides, self.decay_data.dataset_name
             )
             self._check_values(contents_with_parsed_keys)
         else:
             contents_with_parsed_keys = contents
         contents_sorted = sort_dictionary_alphabetically(contents_with_parsed_keys)
-        self.contents = self._convert_to_number(
-            contents_sorted, units, self.quantity_converter, self.unit_converter
-        )
+        self.contents = self._convert_to_number(contents_sorted, units)
 
     @staticmethod
     def _parse_nuclides(
         contents: Dict[Union[str, int, Nuclide], Union[float, Expr]],
         nuclides: np.ndarray,
         dataset_name: str,
     ) -> Dict[str, Union[float, Expr]]:
@@ -158,51 +153,57 @@
 
         for nuc, inp in contents.items():
             if isinstance(inp, (float, int, Expr)):
                 if inp >= 0:
                     continue
             raise ValueError(f"{inp} is not a valid quantity of nuclide {nuc}.")
 
+    def _get_atomic_mass(self, nuc: str) -> Union[float, Expr]:
+        """Returns the appropriate atomic mass."""
+
+        return self.decay_matrices.atomic_masses[self.decay_data.nuclide_dict[nuc]]
+
+    def _get_decay_const(self, nuc: str) -> Union[float, Expr]:
+        """Returns the appropriate atomic mass."""
+
+        return self.decay_matrices.decay_consts[self.decay_data.nuclide_dict[nuc]]
+
+    @abstractmethod
     def _get_decay_matrices(self) -> DecayMatrices:
         """Returns the appropriate DecayMatrices instance."""
 
-        return self.decay_data.scipy_data
-
-    def _get_quantity_converter(self) -> QuantityConverter:
+    @staticmethod
+    @abstractmethod
+    def _get_quantity_converter() -> Type[QuantityConverter]:
         """Returns the appropriate QuantityConverter instance."""
 
-        return self.decay_data.float_quantity_converter
-
-    def _get_unit_converter(self) -> UnitConverterFloat:
+    @abstractmethod
+    def _get_unit_converter(self) -> Type[UnitConverter]:
         """Returns the appropriate UnitConverter instance."""
 
-        return self.decay_data.float_unit_converter
+    @abstractmethod
+    def _get_year_conv(self) -> Union[float, Expr]:
+        """Returns the appropriate number of days in a year."""
 
-    @staticmethod
     def _convert_to_number(
+        self,
         contents: Dict[str, Union[float, Expr]],
         units: str,
-        quantity_converter: QuantityConverter,
-        unit_converter: UnitConverterFloat,
     ) -> Dict[str, Union[float, Expr]]:
         """
         Converts an inventory dictionary where the values are masses, moles or activities to one
         where the values are number of atoms.
 
         Parameters
         ----------
         contents : dict
             Dictionary containing nuclide strings or Nuclide objects as keys, and masses,
             moles, or activities as values.
         units : str
             Units of the values in the input dictionary.
-        quantity_conveter : QuantityConverter
-            Convertor between quantities.
-        unit_conveter : UnitConverterFloat
-            Convertor between units of a single quantity.
 
         Returns
         -------
         dict
             Inventory dictionary where the values are the number of atoms of the nuclide.
 
         Raises
@@ -210,33 +211,34 @@
         ValueError
             If the units supplied are invalid.
 
         """
 
         if units == "num":
             contents_as_numbers = contents
-        elif units in unit_converter.activity_units:
+        elif units in self._get_unit_converter().activity_units:
             contents_as_numbers = {
-                nuc: quantity_converter.activity_to_number(
-                    nuc, unit_converter.activity_unit_conv(act, units, "Bq")
+                nuc: self._get_quantity_converter().activity_to_number(
+                    self._get_unit_converter().activity_unit_conv(act, units, "Bq"),
+                    self._get_decay_const(nuc),
                 )
                 for nuc, act in contents.items()
             }
-        elif units in unit_converter.moles_units:
+        elif units in self._get_unit_converter().moles_units:
             contents_as_numbers = {
-                nuc: quantity_converter.moles_to_number(
-                    unit_converter.moles_unit_conv(mol, units, "mol")
+                nuc: self._get_quantity_converter().moles_to_number(
+                    self._get_unit_converter().moles_unit_conv(mol, units, "mol")
                 )
                 for nuc, mol in contents.items()
             }
-        elif units in unit_converter.mass_units:
+        elif units in self._get_unit_converter().mass_units:
             contents_as_numbers = {
-                nuc: quantity_converter.mass_to_number(
-                    nuc,
-                    unit_converter.mass_unit_conv(mass, units, "g"),
+                nuc: self._get_quantity_converter().mass_to_number(
+                    self._get_unit_converter().mass_unit_conv(mass, units, "g"),
+                    self._get_atomic_mass(nuc),
                 )
                 for nuc, mass in contents.items()
             }
         else:
             raise ValueError(units + " is not a supported unit.")
 
         return contents_as_numbers
@@ -282,16 +284,18 @@
         --------
         >>> rd.Inventory({'Tc-99m': 2300, 'I-123': 5800}, 'Bq').activities('kBq')
         {'I-123': 5.8, 'Tc-99m': 2.3}
 
         """
 
         activities = {
-            nuc: self.unit_converter.activity_unit_conv(
-                self.quantity_converter.number_to_activity(nuc, num),
+            nuc: self._get_unit_converter().activity_unit_conv(
+                self._get_quantity_converter().number_to_activity(
+                    num, self._get_decay_const(nuc)
+                ),
                 "Bq",
                 units,
             )
             for nuc, num in self.contents.items()
         }
 
         return activities
@@ -310,16 +314,18 @@
         --------
         >>> rd.Inventory({'Tc-99m': 2.3, 'I-123': 5.8}, 'Bq').masses('pg')
         {'I-123': 8.158243973887584e-05, 'Tc-99m': 1.1800869622748502e-05}
 
         """
 
         masses = {
-            nuc: self.unit_converter.mass_unit_conv(
-                self.quantity_converter.number_to_mass(nuc, num),
+            nuc: self._get_unit_converter().mass_unit_conv(
+                self._get_quantity_converter().number_to_mass(
+                    num, self._get_atomic_mass(nuc)
+                ),
                 "g",
                 units,
             )
             for nuc, num in self.contents.items()
         }
 
         return masses
@@ -339,16 +345,16 @@
         --------
         >>> rd.Inventory({'Tc-99m': 2.3, 'I-123': 5.8}, 'Bq').moles()
         {'I-123': 6.637813617983513e-19, 'Tc-99m': 1.1931350531142702e-19}
 
         """
 
         moles = {
-            nuc: self.unit_converter.moles_unit_conv(
-                self.quantity_converter.number_to_moles(num), "mol", units
+            nuc: self._get_unit_converter().moles_unit_conv(
+                self._get_quantity_converter().number_to_moles(num), "mol", units
             )
             for nuc, num in self.contents.items()
         }
 
         return moles
 
     def activity_fractions(self) -> Dict[str, float]:
@@ -470,73 +476,73 @@
         {'C-14': 2.0, 'H-3': 0.0}
 
         """
 
         other = Inventory(sub_contents, units, True, self.decay_data)
         self.contents = (self - other).contents
 
-    def __add__(self, other: "Inventory") -> "Inventory":
+    def __add__(self, other: "AbstractInventory") -> "AbstractInventory":
         """Defines + operator to add two Inventory objects together."""
 
         if self.decay_data != other.decay_data:
             raise ValueError(
                 "Decay datasets do not match. "
                 + self.decay_data.dataset_name
                 + " and "
                 + other.decay_data.dataset_name
             )
         new_contents = add_dictionaries(self.contents, other.contents)
-        return Inventory(new_contents, "num", False, self.decay_data)
+        return self.__class__(new_contents, "num", False, self.decay_data)
 
-    def __sub__(self, other: "Inventory") -> "Inventory":
+    def __sub__(self, other: "AbstractInventory") -> "AbstractInventory":
         """Defines - operator to subtract one inventory object from another."""
 
         if self.decay_data != other.decay_data:
             raise ValueError(
                 "Decay datasets do not match. "
                 + self.decay_data.dataset_name
                 + " and "
                 + other.decay_data.dataset_name
             )
         sub_contents = other.contents.copy()
         sub_contents.update(
             (nuclide, number * -1.0) for nuclide, number in sub_contents.items()
         )
         new_contents = add_dictionaries(self.contents, sub_contents)
-        return Inventory(new_contents, "num", False, self.decay_data)
+        return self.__class__(new_contents, "num", False, self.decay_data)
 
-    def __mul__(self, const: Union[float, Expr]) -> "Inventory":
+    def __mul__(self, const: Union[float, Expr]) -> "AbstractInventory":
         """
         Defines * operator to multiply all quantities of nuclides in an inventory by a constant.
         """
 
         new_contents = self.contents.copy()
         for nuclide, number in new_contents.items():
             new_contents[nuclide] = number * const
 
-        return Inventory(new_contents, "num", False, self.decay_data)
+        return self.__class__(new_contents, "num", False, self.decay_data)
 
-    def __rmul__(self, const: Union[float, Expr]) -> "Inventory":
+    def __rmul__(self, const: Union[float, Expr]) -> "AbstractInventory":
         """
         Defines * operator to multiply all quantities of nuclides in an Inventory by a constant.
         """
 
         return self.__mul__(const)
 
-    def __truediv__(self, const: Union[float, Expr]) -> "Inventory":
+    def __truediv__(self, const: Union[float, Expr]) -> "AbstractInventory":
         """
         Defines / operator to divide all quantities of nuclides in an inventory by a constant.
         """
         new_contents = self.contents.copy()
         for nuclide, number in new_contents.items():
             new_contents[nuclide] = number / const
 
-        return Inventory(new_contents, "num", False, self.decay_data)
+        return self.__class__(new_contents, "num", False, self.decay_data)
 
-    @_method_dispatch
+    @singledispatchmethod
     def remove(
         self, delete: Union[str, int, Nuclide, List[Union[str, int, Nuclide]]]
     ) -> None:
         """
         Removes nuclide(s) from the inventory.
 
         Parameters
@@ -573,78 +579,80 @@
         new_contents = self.contents.copy()
         if delete not in new_contents:
             raise ValueError(delete + " does not exist in this inventory.")
         new_contents.pop(delete)
 
         self.contents = new_contents
 
-    @remove.register(int)  # type: ignore[no-redef]
+    @remove.register(int)
     def _(
         self, delete: int
     ) -> Callable[[Dict[str, float], str, bool, DecayData], None]:
         """Remove nuclide string from this inventory."""
 
-        delete = parse_nuclide(
+        delete_str = parse_nuclide(
             delete, self.decay_data.nuclides, self.decay_data.dataset_name
         )
         new_contents = self.contents.copy()
-        if delete not in new_contents:
-            raise ValueError(delete + " does not exist in this inventory.")
-        new_contents.pop(delete)
+        if delete_str not in new_contents:
+            raise ValueError(delete_str + " does not exist in this inventory.")
+        new_contents.pop(delete_str)
 
         self.contents = new_contents
 
-    @remove.register(Nuclide)  # type: ignore[no-redef]
+    @remove.register(Nuclide)
     def _(
         self, delete: Nuclide
     ) -> Callable[[Dict[str, float], str, bool, DecayData], None]:
         """Remove Nuclide object from this inventory."""
 
-        delete = parse_nuclide(
+        delete_str = parse_nuclide(
             delete.nuclide, self.decay_data.nuclides, self.decay_data.dataset_name
         )
         new_contents = self.contents.copy()
-        if delete not in new_contents:
-            raise ValueError(delete + " does not exist in this inventory.")
-        new_contents.pop(delete)
+        if delete_str not in new_contents:
+            raise ValueError(delete_str + " does not exist in this inventory.")
+        new_contents.pop(delete_str)
 
         self.contents = new_contents
 
-    @remove.register(list)  # type: ignore[no-redef]
+    @remove.register(list)
     def _(
         self, delete: List[Union[str, int, Nuclide]]
     ) -> Callable[[Dict[str, float], str, bool, DecayData], None]:
         """Remove list of nuclide(s) from this inventory."""
 
-        delete = [
+        delete_list = [
             parse_nuclide(
                 nuc.nuclide, self.decay_data.nuclides, self.decay_data.dataset_name
             )
             if isinstance(nuc, Nuclide)
             else parse_nuclide(
                 nuc, self.decay_data.nuclides, self.decay_data.dataset_name
             )
             for nuc in delete
         ]
         new_contents = self.contents.copy()
-        for nuc in delete:
+        for nuc in delete_list:
             if nuc not in new_contents:
                 raise ValueError(nuc + " does not exist in this inventory.")
             new_contents.pop(nuc)
 
         self.contents = new_contents
 
     def _convert_decay_time(
         self, decay_time: Union[float, Expr], units: str
     ) -> Union[float, Expr]:
         """
         Converts a decay time period into seconds.
         """
 
-        return self.unit_converter.time_unit_conv(decay_time, units, "s")
+        return self._get_unit_converter().time_unit_conv(
+            decay_time, units, "s", self._get_year_conv()
+        )
 
     def _setup_decay_calc(
         self,
     ) -> Tuple[Union[np.ndarray, Matrix], List[int], Union[sparse.csr_matrix, Matrix]]:
         """
         Setup variables for a decay calculation.
         """
@@ -674,106 +682,31 @@
             self.decay_matrices.matrix_c
             @ matrix_e
             @ self.decay_matrices.matrix_c_inv
             @ vector_n0
         )
         return vector_nt
 
-    def decay(self, decay_time: float, units: str = "s") -> "Inventory":
+    @abstractmethod
+    def decay(self, decay_time: float, units: str = "s") -> "AbstractInventory":
         """
         Returns a new inventory calculated from the radioactive decay of the current inventory for
         decay_time.
-
-        Parameters
-        ----------
-        decay_time : float
-            Decay time.
-        units : str, optional
-            Units of decay_time (default is seconds). Options are 'ns', 'us', 'ms', 's', 'm', 'h',
-            'd', 'y', 'ky', 'My', 'Gy', 'Ty', 'Py', and some of the common spelling variations of
-            these time units.
-
-        Returns
-        -------
-        Inventory
-            New Inventory after the radioactive decay.
-
-        Examples
-        --------
-        >>> inv_t0 = rd.Inventory({'H-3': 1.0}, 'Bq')
-        >>> inv_t1 = inv_t0.decay(12.32, 'y')
-        >>> inv_t1.activities()
-        {'H-3': 0.5, 'He-3': 0.0}
-
         """
 
-        decay_time = self._convert_decay_time(decay_time, units)
-        vector_n0, indices, matrix_e = self._setup_decay_calc()
-
-        matrix_e.data[indices] = np.exp(
-            -decay_time * self.decay_matrices.decay_consts[indices]
-        )
-
-        vector_nt = self._perform_decay_calc(vector_n0, matrix_e)
-        new_contents = dict(zip(self.decay_data.nuclides[indices], vector_nt[indices]))
-
-        return Inventory(new_contents, "num", False, self.decay_data)
-
+    @abstractmethod
     def cumulative_decays(
         self, decay_time: float, units: str = "s"
     ) -> Dict[str, float]:
         """
         Calculates the total number of decays of each nuclide in the inventory between t=0 and
         t=decay_time. Note no results are reported for stable nuclides, as cumulative decays is
         zero.
-
-        Parameters
-        ----------
-        decay_time : float
-            Decay time (calculates total number of decays over this period).
-        units : str, optional
-            Units of decay_time (default is seconds). Options are 'ns', 'us', 'ms', 's', 'm', 'h',
-            'd', 'y', 'ky', 'My', 'Gy', 'Ty', 'Py', and some of the common spelling variations of
-            these time units.
-
-        Returns
-        -------
-        dict
-            Dictionary containing nuclide strings as keys and total number of decays of each
-            nuclide as values (floats).
-
-        Examples
-        --------
-        >>> inv_t0 = rd.Inventory({'Sr-90': 10.0}, 'num')
-        >>> inv_t0.cumulative_decays(1.0, 'My')
-        {'Sr-90': 10.0, 'Y-90': 10.000000000000002}
-
         """
 
-        decay_time = self._convert_decay_time(decay_time, units)
-        vector_n0, indices, matrix_e = self._setup_decay_calc()
-
-        indices = [
-            idx for idx in indices if self.decay_matrices.decay_consts[idx] > 0.0
-        ]
-        for idx in indices:
-            matrix_e[idx, idx] = (
-                1.0 - np.exp((-decay_time * self.decay_matrices.decay_consts[idx]))
-            ) / self.decay_matrices.decay_consts[idx]
-
-        cumulative_decays = self._perform_decay_calc(vector_n0, matrix_e)
-        result_dict = {
-            self.decay_data.nuclides[idx]: float(
-                self.decay_matrices.decay_consts[idx] * cumulative_decays[idx]
-            )
-            for idx in indices
-        }
-
-        return result_dict
-
     def half_lives(self, units: str = "s") -> Dict[str, Union[float, str]]:
         """
         Returns dictionary of half-lives of the nuclides in the inventory in your chosen time
         units, or as a human-readable string with appropriate units.
 
         Parameters
         ----------
@@ -864,15 +797,15 @@
 
         """
 
         return {
             nuc: Nuclide(nuc, self.decay_data).decay_modes() for nuc in self.contents
         }
 
-    def plot(
+    def plot(  # type: ignore
         self,
         xmax: float,
         xunits: str = "s",
         xmin: float = 0.0,
         xscale: str = "linear",
         yscale: str = "linear",
         ymin: float = 0.0,
@@ -972,27 +905,27 @@
                 parse_nuclide(
                     rad, self.decay_data.nuclides, self.decay_data.dataset_name
                 )
                 for rad in display
             ]
 
         ydata = np.zeros(shape=(npoints, len(display)))
-        if yunits in self.unit_converter.activity_units:
+        if yunits in self._get_unit_converter().activity_units:
             for idx in range(0, npoints):
                 decayed_contents = self.decay(time_points[idx], xunits).activities(
                     yunits
                 )
                 ydata[idx] = [decayed_contents[rad] for rad in display]
                 ylabel = f"Activity ({yunits})"
-        elif yunits in self.unit_converter.moles_units:
+        elif yunits in self._get_unit_converter().moles_units:
             for idx in range(0, npoints):
                 decayed_contents = self.decay(time_points[idx], xunits).moles(yunits)
                 ydata[idx] = [decayed_contents[rad] for rad in display]
                 ylabel = f"Number of moles ({yunits})"
-        elif yunits in self.unit_converter.mass_units:
+        elif yunits in self._get_unit_converter().mass_units:
             for idx in range(0, npoints):
                 decayed_contents = self.decay(time_points[idx], xunits).masses(yunits)
                 ydata[idx] = [decayed_contents[rad] for rad in display]
                 ylabel = f"Mass ({yunits})"
         elif yunits == "num":
             for idx in range(0, npoints):
                 decayed_contents = self.decay(time_points[idx], xunits).numbers()
@@ -1018,15 +951,15 @@
         else:
             raise ValueError(f"{yunits} is not a supported y-axes unit.")
 
         if yscale == "log" and ymin == 0.0:
             ymin = 0.1
         ylimits = [ymin, ymax] if ymax else [ymin, 1.05 * ydata.max()]
 
-        fig, axes = _decay_graph(
+        fig, axes = decay_graph(
             time_points=time_points,
             ydata=ydata.T,
             nuclides=display,
             xunits=xunits,
             ylabel=ylabel,
             xscale=xscale,
             yscale=yscale,
@@ -1040,73 +973,234 @@
         return fig, axes
 
     def __eq__(self, other: object) -> bool:
         """
         Check whether two instances are equal with ``==`` operator.
         """
 
-        if not isinstance(other, Inventory):
+        if not isinstance(other, AbstractInventory):
             return NotImplemented
         return self.contents == other.contents and self.decay_data == other.decay_data
 
     def __ne__(self, other: object) -> bool:
         """
         Check whether two instances are not equal with ``!=`` operator.
         """
 
-        if not isinstance(other, Inventory):
+        if not isinstance(other, AbstractInventory):
             return NotImplemented
         return not self.__eq__(other)
 
+
+class Inventory(AbstractInventory):
+    # pylint: disable=line-too-long
+    """
+    ``Inventory`` instances store nuclides and associated quantities (numbers of atoms) in the
+    contents dictionary. A decay dataset is associated with each instance.
+
+    Parameters
+    ----------
+    contents : dict
+        Dictionary containing nuclide strings/canonical ids or Nuclide instances as keys and
+        quantities (activities, number of atoms, masses or moles) as values.
+    units : str, optional
+        Units of the contents dictionary values. Specify either 'num' for number of atoms, or an
+        activity, mass or moles unit. e.g. 'Bq', 'kBq', 'Ci', 'g', 'kg', 'mol', 'kmol'. Default is
+        'Bq'.
+    check : bool, optional
+        Check for the validity of the contents dictionary (nuclides are in the decay dataset,
+        and quantities provided are physical, etc.). Default is True.
+    decay_data : DecayData, optional
+        Decay dataset (default is the ICRP-107 dataset).
+
+    Attributes
+    ----------
+    contents : dict
+        Dictionary containing nuclide strings as keys and number of atoms of each nuclide as
+        values. Nuclides are sorted alphabetically in this dictionary.
+    decay_data : DecayData
+        Decay dataset.
+    decay_matrices : DecayMatricesScipy
+        Float/SciPy version of the DecayMatrices associated with the decay dataset.
+
+    Examples
+    --------
+    >>> rd.Inventory({'Tc-99m': 2.3, 'I-123': 5.8}, 'Bq')
+    Inventory activities (Bq): {'I-123': 2.3, 'Tc-99m': 5.8}, decay dataset: icrp107_ame2020_nubase2020
+    >>> H3 = rd.Nuclide('H-3')
+    >>> rd.Inventory({H3: 3.0}, 'g')
+    Inventory activities (Bq): {'H-3': 1067957043281807.0}, decay dataset: icrp107_ame2020_nubase2020
+    >>> rd.Inventory({270570000: 7.2, 922380000: 21.1}, 'Ci')
+    Inventory activities (Bq): {'Co-57': 266400000000.0, 'U-238': 780700000000.0001}, decay dataset: icrp107_ame2020_nubase2020
+
+    """
+    # pylint: enable=line-too-long
+
+    def _get_decay_matrices(self) -> DecayMatricesScipy:
+        """Returns the appropriate DecayMatrices instance."""
+
+        return self.decay_data.scipy_data
+
+    @staticmethod
+    def _get_quantity_converter() -> Type[QuantityConverter]:
+        """
+        Returns the appropriate QuantityConverter instance.
+        """
+
+        return QuantityConverterFloat
+
+    def _get_unit_converter(self) -> Type[UnitConverter]:
+        """
+        Returns the appropriate UnitConverter instance.
+        """
+
+        return UnitConverterFloat
+
+    def _get_year_conv(self) -> float:
+        """Returns the appropriate number of days in a year."""
+
+        return self.decay_data.float_year_conv
+
+    def decay(self, decay_time: float, units: str = "s") -> "Inventory":
+        """
+        Returns a new inventory calculated from the radioactive decay of the current inventory for
+        decay_time.
+
+        Parameters
+        ----------
+        decay_time : float
+            Decay time.
+        units : str, optional
+            Units of decay_time (default is seconds). Options are 'ns', 'us', 'ms', 's', 'm', 'h',
+            'd', 'y', 'ky', 'My', 'Gy', 'Ty', 'Py', and some of the common spelling variations of
+            these time units.
+
+        Returns
+        -------
+        Inventory
+            New Inventory after the radioactive decay.
+
+        Examples
+        --------
+        >>> inv_t0 = rd.Inventory({'H-3': 1.0}, 'Bq')
+        >>> inv_t1 = inv_t0.decay(12.32, 'y')
+        >>> inv_t1.activities()
+        {'H-3': 0.5, 'He-3': 0.0}
+
+        """
+
+        decay_time = self._convert_decay_time(decay_time, units)
+        vector_n0, indices, matrix_e = self._setup_decay_calc()
+
+        matrix_e.data[indices] = np.exp(
+            -decay_time * self.decay_matrices.decay_consts[indices]
+        )
+
+        vector_nt = self._perform_decay_calc(vector_n0, matrix_e)
+        new_contents = dict(zip(self.decay_data.nuclides[indices], vector_nt[indices]))
+
+        return self.__class__(new_contents, "num", False, self.decay_data)
+
+    def cumulative_decays(
+        self, decay_time: float, units: str = "s"
+    ) -> Dict[str, float]:
+        """
+        Calculates the total number of decays of each nuclide in the inventory between t=0 and
+        t=decay_time. Note no results are reported for stable nuclides, as cumulative decays is
+        zero.
+
+        Parameters
+        ----------
+        decay_time : float
+            Decay time (calculates total number of decays over this period).
+        units : str, optional
+            Units of decay_time (default is seconds). Options are 'ns', 'us', 'ms', 's', 'm', 'h',
+            'd', 'y', 'ky', 'My', 'Gy', 'Ty', 'Py', and some of the common spelling variations of
+            these time units.
+
+        Returns
+        -------
+        dict
+            Dictionary containing nuclide strings as keys and total number of decays of each
+            nuclide as values (floats).
+
+        Examples
+        --------
+        >>> inv_t0 = rd.Inventory({'Sr-90': 10.0}, 'num')
+        >>> inv_t0.cumulative_decays(1.0, 'My')
+        {'Sr-90': 10.0, 'Y-90': 10.000000000000002}
+
+        """
+
+        decay_time = self._convert_decay_time(decay_time, units)
+        vector_n0, indices, matrix_e = self._setup_decay_calc()
+
+        indices = [
+            idx for idx in indices if self.decay_matrices.decay_consts[idx] > 0.0
+        ]
+        for idx in indices:
+            matrix_e[idx, idx] = (
+                1.0 - np.exp((-decay_time * self.decay_matrices.decay_consts[idx]))
+            ) / self.decay_matrices.decay_consts[idx]
+
+        cumulative_decays = self._perform_decay_calc(vector_n0, matrix_e)
+        result_dict = {
+            self.decay_data.nuclides[idx]: float(
+                self.decay_matrices.decay_consts[idx] * cumulative_decays[idx]
+            )
+            for idx in indices
+        }
+
+        return result_dict
+
     def __repr__(self) -> str:
         return (
             f"Inventory activities (Bq): {self.activities()}, "
             + f"decay dataset: {self.decay_data.dataset_name}"
         )
 
 
-class InventoryHP(Inventory):
+class InventoryHP(AbstractInventory):
     """
     ``InventoryHP`` instances store a dictionary of nuclides and associated numbers of atoms, and a
     ``DecayData`` instance of radioactive decay data. Uses SymPy high precision arithmetic for all
     calculations.
 
     Parameters
     ----------
     contents : dict
         Dictionary containing nuclide strings/canonical ids or Nuclide
         objects as keys and quantities as values.
     units : str, optional
         Units of the values in the contents dictionary e.g. 'Bq', 'kBq', 'Ci', 'g', 'mol',
         'num'... (default is 'Bq').
     check : bool, optional
-        Check for the validity of contents (default is True).
+        Check for the validity of contents and that the supplied decay dataset contains SymPy data
+        (default is True).
     data : DecayData, optional
         Decay dataset (default is the ICRP-107 dataset).
     sympy_contents : dict, optional
         Version of the contents dictionary with SymPy expressions as values. Setting this requires
         that data (the decay dataset) contains SymPy data. ``radioactivedecay`` will create
         sympy_contents automatically from contents if None is supplied.
 
     Attributes
     ----------
     contents : dict
         Dictionary containing nuclide strings as keys and number of atoms of each nuclide as
         values. Nuclides are sorted alphabetically in this dictionary.
     data : DecayData
         Decay dataset.
-    decay_matrices : DecayMatrices
+    decay_matrices : DecayMatricesSympy
        SymPy DecayMatrices instance associated with the decay dataset.
     sig_fig: int
         Number of significant figures for high precision decay calculations and plots. Deafult is
         320.
-    quantity_converter : QuantityConverterSympy
-        Float/SciPy version of a convertor between different quantities.
     unit_converter : UnitConverterSympy
-        Float version of a convertor for within different units.
+        SymPy version of a convertor for within different units.
 
     Examples
     --------
     >>> rd.InventoryHP({'Tc-99m': 2.3, 'I-123': 5.8}, 'Bq')
     InventoryHP activities: {'I-123': 2.3, 'Tc-99m': 5.8}, decay dataset: icrp107
     >>> H3 = rd.Nuclide('H-3')
     >>> rd.InventoryHP({H3: 3.0} 'Bq')
@@ -1121,49 +1215,53 @@
         contents: Dict[Union[str, int, Nuclide], float],
         units: str = "Bq",
         check: bool = True,
         decay_data: DecayData = DEFAULTDATA,
     ) -> None:
 
         if check is True:
+            try:
+                assert decay_data.sympy_data
+                assert decay_data.sympy_year_conv
+            except ValueError:
+                raise ValueError(
+                    f"Decay dataset supplied to {self.__class__.__name__} constructor does not "
+                    "contain SymPy data."
+                ) from None
             contents = {nuc: nsimplify(val) for nuc, val in contents.items()}
+
         self.sig_fig = 320
         super().__init__(contents, units, check, decay_data)
 
     def _get_decay_matrices(self) -> DecayMatricesSympy:
         """
         Returns the appropriate DecayMatrices instance.
         """
 
-        if self.decay_data.sympy_data is None:
-            raise ValueError(
-                f"{self.decay_data.dataset_name} does not contain DecayMatricesSymPy instance."
-            )
         return self.decay_data.sympy_data
 
-    def _get_quantity_converter(self) -> QuantityConverterSympy:
+    @staticmethod
+    def _get_quantity_converter() -> Type[QuantityConverter]:
         """
         Returns the appropriate QuantityConverter instance.
         """
-        if self.decay_data.sympy_quantity_converter is None:
-            raise ValueError(
-                f"{self.decay_data.dataset_name} does not contain QuantityConverterSympy instance."
-            )
-        return self.decay_data.sympy_quantity_converter
 
-    def _get_unit_converter(self) -> UnitConverterSympy:
+        return QuantityConverterSympy
+
+    def _get_unit_converter(self) -> Type[UnitConverter]:
         """
         Returns the appropriate UnitConverter instance.
         """
 
-        if self.decay_data.sympy_unit_converter is None:
-            raise ValueError(
-                f"{self.decay_data.dataset_name} does not contain UnitConverterSympy instance."
-            )
-        return self.decay_data.sympy_unit_converter
+        return UnitConverterSympy
+
+    def _get_year_conv(self) -> Expr:
+        """Returns the appropriate number of days in a year."""
+
+        return self.decay_data.sympy_year_conv
 
     def numbers(self) -> Dict[str, float]:
         """
         Returns a dictionary containing the number of atoms of each nuclide (as floats) within this
         InventoryHP instance.
 
         Examples
@@ -1187,16 +1285,18 @@
             Activity units for output, e.g. 'Bq', 'kBq', 'mBq', 'Ci', 'dpm'...
             Deafult is 'Bq'.
 
         """
 
         activities = {
             nuc: float(
-                self.unit_converter.activity_unit_conv(
-                    self.quantity_converter.number_to_activity(nuc, num),
+                self._get_unit_converter().activity_unit_conv(
+                    self._get_quantity_converter().number_to_activity(
+                        num, self._get_decay_const(nuc)
+                    ),
                     "Bq",
                     units,
                 )
             )
             for nuc, num in self.contents.items()
         }
 
@@ -1213,16 +1313,18 @@
             Mass units for output, e.g. 'Bq', 'g', 'kg', 'mg', 'ton'...
             Deafult is 'g'.
 
         """
 
         masses = {
             nuc: float(
-                self.unit_converter.mass_unit_conv(
-                    self.quantity_converter.number_to_mass(nuc, num),
+                self._get_unit_converter().mass_unit_conv(
+                    self._get_quantity_converter().number_to_mass(
+                        num, self._get_atomic_mass(nuc)
+                    ),
                     "g",
                     units,
                 )
             )
             for nuc, num in self.contents.items()
         }
 
@@ -1239,16 +1341,16 @@
             Moles units, e.g. 'mmol', 'mol', 'kmol'...
             Deafult is 'mol'.
 
         """
 
         moles = {
             nuc: float(
-                self.unit_converter.moles_unit_conv(
-                    self.quantity_converter.number_to_moles(num), "mol", units
+                self._get_unit_converter().moles_unit_conv(
+                    self._get_quantity_converter().number_to_moles(num), "mol", units
                 )
             )
             for nuc, num in self.contents.items()
         }
 
         return moles
 
@@ -1311,15 +1413,15 @@
             )
 
         vector_nt = self._perform_decay_calc(vector_n0, matrix_e)
         new_contents = {
             self.decay_data.nuclides[idx]: vector_nt[idx] for idx in indices
         }
 
-        return InventoryHP(new_contents, "num", False, self.decay_data)
+        return self.__class__(new_contents, "num", False, self.decay_data)
 
     def cumulative_decays(
         self, decay_time: float, units: str = "s"
     ) -> Dict[str, float]:
         """
         Calculates the total number of decays of each nuclide in the inventory between t=0 and
         t=decay_time. Uses SymPy high precision calculations. Note no results are reported for
@@ -1381,15 +1483,19 @@
                 self.decay_matrices.decay_consts[idx] * cumulative_decays[idx]
             )
             for idx in indices
         }
 
         return result_dict
 
-    def plot(
+    # Redefines one default parameter of the plot function (npoints) for performance reasons.
+    # Note rewriting all the parameters like this violates the Don't Repeat Yourself principle, but
+    # currently no better solution while still maintaining auto-complete functionality for
+    # the method signature with some editors.
+    def plot(  # type: ignore
         self,
         xmax: float,
         xunits: str = "s",
         xmin: float = 0.0,
         xscale: str = "linear",
         yscale: str = "linear",
         ymin: float = 0.0,
@@ -1400,15 +1506,15 @@
         npoints: int = 51,
         fig: Optional[matplotlib.figure.Figure] = None,
         axes: Optional[matplotlib.axes.Axes] = None,
         **kwargs,
     ) -> Tuple[matplotlib.figure.Figure, matplotlib.axes.Axes]:
         """
         Plots a decay graph using high precision decay calculations. Only difference from normal
-        precision decay plot (``Inventory.plot()``) is default npoints=51
+        precision decay plot (``Inventory.plot()``) is default npoints=51.
 
         Parameters
         ----------
         xmax : float
             Maximum decay time on x-axis.
         xunits : str, optional
             Units for decay times (default is 's', i.e. seconds). Options are 'ps', 'ns', 'us',
```

### Comparing `radioactivedecay-0.4.8/radioactivedecay/nuclide.py` & `radioactivedecay-0.4.9/radioactivedecay/nuclide.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 extracting atomic number and mass information, as well as a clean name string.
 Furthermore, additional methods provide an access point for mass data of
 nuclides, and the decay data of radionuclides, if present in a specified
 dataset. The default decay dataset used if none is supplied to the constructor
 is rd.DEFAULTDATA.
 
 The docstring code examples assume that ``radioactivedecay`` has been imported
-as `rd`:
+as ``rd``:
 
 .. highlight:: python
 .. code-block:: python
 
     >>> import radioactivedecay as rd
 
 """
@@ -35,113 +35,160 @@
 class Nuclide:
     """
     ``Nuclide`` instances serve as name and atomic number/mass parsing
     objects for any nuclide or element.
 
     Parameters
     ----------
-    input_nuclide : str or int
-        Input value for instantiation. Can be nuclide string in name
-        format (with or without hyphen), or canonical id (zzzaaassss).
+    nuclide : str or int
+        Specify the nuclide with either a name string (e.g. 'H-3', 'H3' or '3H') or a canonical id
+        (zzzaaassss format).
     decay_data : DecayData, optional
         Decay dataset (default is the ICRP-107 dataset).
 
     Attributes
     ----------
     nuclide: str
         Nuclide name string.
-    Z : int
-        Atomic number.
-    A : int
-        Atomic mass number.
-    id : int
-        Canonical nuclide id, in zzzaaassss form. Ground state is 0000,
-        first excited state ("m") is 0001, second ("n") is 0002, etc.
     decay_data : DecayData
         Decay dataset.
-    atomic_mass : float
-        Atomic weight of the nuclide, in g/mol.
-    prog : list
-        List of direct progeny of this nuclide.
-    bfs : list
-        List of branching fractions to direct progeny of this nuclide.
-    modes : list
-        List of modes to direct progeny of this nuclide.
 
     Examples
     --------
     >>> rd.Nuclide('K-40')
-    Nuclide: K-40
+    Nuclide: K-40, decay dataset: icrp107_ame2020_nubase2020
     >>> rd.Nuclide('K40')
-    Nuclide: K-40
+    Nuclide: K-40, decay dataset: icrp107_ame2020_nubase2020
     >>> rd.Nuclide(190400000)
-    Nuclide: K-40
+    Nuclide: K-40, decay dataset: icrp107_ame2020_nubase2020
     >>> rd.Nuclide(280560001)
-    Nuclide: Ni-56m
+    Nuclide: Ni-56m, decay dataset: icrp107_ame2020_nubase2020
 
     """
 
     def __init__(
-        self, input_nuclide: Union[str, int], decay_data: DecayData = DEFAULTDATA
+        self, nuclide: Union[str, int], decay_data: DecayData = DEFAULTDATA
     ) -> None:
         self.decay_data = decay_data
-        self.parse_name(input_nuclide)
-        idx = decay_data.nuclide_dict[self.nuclide]
-        self.atomic_mass = decay_data.scipy_data.atomic_masses[idx]
-        self.prog: List[str] = decay_data.progeny[idx]
-        self.bfs: List[float] = decay_data.bfs[idx]
-        self.modes: List[str] = decay_data.modes[idx]
+        self.nuclide = parse_nuclide(
+            nuclide, self.decay_data.nuclides, self.decay_data.dataset_name
+        )
 
-    def parse_name(self, input_nuclide: Union[str, int]) -> None:
+    @property
+    def Z(self) -> int:
         """
-        Parse input and set atomic data attributes.
+        Returns the atomic number of the nuclide.
+
+        Returns
+        -------
+        int
+            Atomic number of the nuclide.
+
+        Examples
+        --------
+        >>> H3 = rd.Nuclide('H-3')
+        >>> H3.Z
+        1
+
         """
 
-        self.nuclide = parse_nuclide(
-            input_nuclide, self.decay_data.nuclides, self.decay_data.dataset_name
-        )
-        self.Z = elem_to_Z(self.nuclide.split("-")[0])
-        self.A = int(self.nuclide.split("-")[1].strip("mn"))
-        self.state = self.nuclide.split("-")[1].strip("0123456789")
-        self.id = build_id(self.Z, self.A, self.state)
+        return elem_to_Z(self.nuclide.split("-")[0])
 
-    def __repr__(self) -> str:
-        rep = (
-            "Nuclide: "
-            + self.nuclide
-            + ", decay dataset: "
-            + self.decay_data.dataset_name
-        )
+    @property
+    def A(self) -> int:
+        """
+        Returns the mass number of the nuclide.
 
-        return rep
+        Returns
+        -------
+        int
+            Mass number of the nuclide.
+
+        Examples
+        --------
+        >>> H3 = rd.Nuclide('H-3')
+        >>> H3.A
+        3
 
-    def __eq__(self, other: object) -> bool:
         """
-        Check whether two ``Nuclide`` instances are equal with ``==`` operator.
+
+        return int(self.nuclide.split("-")[1].strip("mn"))
+
+    @property
+    def state(self) -> str:
         """
+        Returns the metastable state character, i.e. '' for ground state, 'm' for first metastable
+        state, 'n' for second metastable state, etc..
 
-        if not isinstance(other, Nuclide):
-            return NotImplemented
-        return self.nuclide == other.nuclide and self.decay_data == other.decay_data
+        Returns
+        -------
+        str
+            Metastable state character.
+
+        Examples
+        --------
+        >>> H3 = rd.Nuclide('H-3')
+        >>> H3.state
+        ''
+        >>> Ba137m = rd.Nuclide('Ba-137m')
+        >>> Ba137m.state
+        'm'
 
-    def __ne__(self, other: object) -> bool:
         """
-        Check whether two ``Nuclide`` instances are not equal with ``!=`` operator.
+
+        return self.nuclide.split("-")[1].strip("0123456789")
+
+    @property
+    def id(self) -> int:
         """
+        Returns the canonical nuclide id, in zzzaaassss form. Ground state is 0000, first excited
+        state ("m") is 0001, second ("n") is 0002, etc.
 
-        if not isinstance(other, Nuclide):
-            return NotImplemented
-        return not self.__eq__(other)
+        Returns
+        -------
+        int
+            Canonical id of the nuclide.
+
+        Examples
+        --------
+        >>> H3 = rd.Nuclide('H-3')
+        >>> H3.id
+        10030000
+        >>> Ba137m = rd.Nuclide('Ba-137m')
+        >>> Ba137m.id
+        561370001
 
-    def __hash__(self) -> int:
         """
-        Hash function for ``Nuclide`` instances.
+
+        return build_id(self.Z, self.A, self.state)
+
+    @property
+    def atomic_mass(self) -> float:
         """
+        Returns the atomic mass of the nuclide, in g/mol.
 
-        return hash((self.nuclide, self.decay_data.dataset_name))
+        Returns
+        -------
+        float
+            Atomic mass of the nuclide in g/mol.
+
+        Examples
+        --------
+        >>> H3 = rd.Nuclide('H-3')
+        >>> H3.atomic_mass
+        3.01604928132
+        >>> Ba137m = rd.Nuclide('Ba-137m')
+        >>> Ba137m.atomic_mass
+        136.9065375271172
+
+        """
+
+        return self.decay_data.scipy_data.atomic_masses[
+            self.decay_data.nuclide_dict[self.nuclide]
+        ]
 
     def half_life(self, units: str = "s") -> Union[float, str]:
         """
         Returns the half-life of a nuclide as a float in your chosen
         units, or as a human-readable string with appropriate units.
 
         Parameters
@@ -159,41 +206,42 @@
             Half-life of the nuclide.
 
         Examples
         --------
         >>> K40 = rd.Nuclide('K-40')
         >>> K40.half_life('y')
         1251000000.0
+        >>> K40.half_life('readable')
+        '1.251 By'
         >>> Fe56 = rd.Nuclide('Fe-56')
         >>> Fe56.half_life('readable')
         'stable'
 
         """
 
         return self.decay_data.half_life(self.nuclide, units)
 
     def progeny(self) -> List[str]:
         """
-        Returns the direct progeny of a radionuclide.
+        Returns list of the direct progeny of the nuclide.
 
         Returns
         -------
         list
-            List of the direct progeny of the radionuclide, ordered by
-            decreasing branching fraction.
+            List of the direct progeny of the nuclide, ordered by decreasing branching fraction.
 
         Examples
         --------
         >>> K40 = rd.Nuclide('K-40')
         >>> K40.progeny()
         ['Ca-40', 'Ar-40']
 
         """
 
-        return self.prog
+        return self.decay_data.progeny[self.decay_data.nuclide_dict[self.nuclide]]
 
     def branching_fractions(self) -> List[float]:
         """
         Returns the branching fractions to the direct progeny of a
         radionuclide.
 
         Returns
@@ -205,15 +253,15 @@
         --------
         >>> K40 = rd.Nuclide('K-40')
         >>> K40.branching_fractions()
         [0.8914, 0.1086]
 
         """
 
-        return self.bfs
+        return self.decay_data.bfs[self.decay_data.nuclide_dict[self.nuclide]]
 
     def decay_modes(self) -> List[str]:
         """
         Returns the decay modes for a radionuclide, as defined in the
         decay dataset. Note: the decay mode strings returned are not
         lists of all the different radiation types emitted during the
         parent to progeny decay processes. They are the labels defined
@@ -229,15 +277,15 @@
         --------
         >>> K40 = rd.Nuclide('K-40')
         >>> K40.decay_modes()
         ['\u03b2-', '\u03b2+ & EC']
 
         """
 
-        return self.modes
+        return self.decay_data.modes[self.decay_data.nuclide_dict[self.nuclide]]
 
     def plot(
         self,
         label_pos: float = 0.5,
         fig: Optional[matplotlib.figure.Figure] = None,
         axes: Optional[matplotlib.axes.Axes] = None,
         kwargs_draw: Optional[Dict[str, Any]] = None,
@@ -329,14 +377,49 @@
         )
 
         axes.set_xlim(-0.3, max_xpos + 0.3)
         axes.set_ylim(-max_generation - 0.3, 0.3)
 
         return fig, axes
 
+    def __repr__(self) -> str:
+        rep = (
+            "Nuclide: "
+            + self.nuclide
+            + ", decay dataset: "
+            + self.decay_data.dataset_name
+        )
+
+        return rep
+
+    def __eq__(self, other: object) -> bool:
+        """
+        Check whether two ``Nuclide`` instances are equal with ``==`` operator.
+        """
+
+        if not isinstance(other, Nuclide):
+            return NotImplemented
+        return self.nuclide == other.nuclide and self.decay_data == other.decay_data
+
+    def __ne__(self, other: object) -> bool:
+        """
+        Check whether two ``Nuclide`` instances are not equal with ``!=`` operator.
+        """
+
+        if not isinstance(other, Nuclide):
+            return NotImplemented
+        return not self.__eq__(other)
+
+    def __hash__(self) -> int:
+        """
+        Hash function for ``Nuclide`` instances.
+        """
+
+        return hash((self.nuclide, self.decay_data.dataset_name))
+
 
 def _build_decay_digraph(
     parent: Nuclide,
     digraph: nx.classes.digraph.DiGraph,
 ) -> nx.classes.digraph.DiGraph:
     """
     Build a networkx DiGraph for the decay chain of this nuclide.
```

### Comparing `radioactivedecay-0.4.8/radioactivedecay/plots.py` & `radioactivedecay-0.4.9/radioactivedecay/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     }
 
     for unformatted, formatted in mode_conversion.items():
         mode = mode.replace(unformatted, formatted)
     return mode
 
 
-def _check_fig_axes(
+def _check_fig_axes(  # type: ignore
     fig_in: Optional[matplotlib.figure.Figure],
     axes_in: Optional[matplotlib.axes.Axes],
     **kwargs,
 ) -> Tuple[matplotlib.figure.Figure, matplotlib.axes.Axes]:
     """
     Checks to see if user supplies Matplotlib Figure and/or Axes objects. Creates them where
     necessary.
@@ -120,15 +120,15 @@
     else:
         fig = fig_in
         axes = axes_in
 
     return fig, axes
 
 
-def _decay_graph(
+def decay_graph(  # type: ignore
     time_points: np.ndarray,
     ydata: np.ndarray,
     nuclides: List[str],
     xunits: str,
     ylabel: str,
     xscale: str,
     yscale: str,
```

### Comparing `radioactivedecay-0.4.8/radioactivedecay/utils.py` & `radioactivedecay-0.4.9/radioactivedecay/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The utils module contains functions to parse nuclide strings and manipulate lists and dictionaries.
 
 The docstring code examples assume that ``radioactivedecay`` has been imported
-as `rd`:
+as ``rd``:
 
 .. highlight:: python
 .. code-block:: python
 
     >>> import radioactivedecay as rd
 
 """
@@ -258,15 +258,15 @@
     >>> rd.utils.build_nuclide_string(26, 56)
     'Fe-56'
     >>> rd.utils.build_nuclide_string(28, 56, 'm')
     'Fe-56m'
 
     """
 
-    if Z not in Z_DICT.keys():
+    if Z not in Z_DICT:
         raise ValueError(str(Z) + " is not a valid atomic number")
 
     return_string = f"{Z_DICT[Z]}-{A}{meta_state}"
 
     return return_string
```

### Comparing `radioactivedecay-0.4.8/radioactivedecay.egg-info/PKG-INFO` & `radioactivedecay-0.4.9/radioactivedecay.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radioactivedecay
-Version: 0.4.8
+Version: 0.4.9
 Summary: A Python package for radioactive decay modelling that supports 1252 radionuclides, decay chains, branching, and metastable states.
 Home-page: https://github.com/radioactivedecay/radioactivedecay
 Author: Alex Malins, Thom Lemoine, & contributors
 Author-email: github@alexmalinsREMOVETHIS.com
 License: MIT, ICRP-07, AMDC
 Project-URL: Bug Tracker, https://github.com/radioactivedecay/radioactivedecay/issues
 Project-URL: Discussions, https://github.com/radioactivedecay/radioactivedecay/discussions
@@ -32,15 +32,15 @@
         The code solves the radioactive decay differential equations analytically using
         NumPy and SciPy linear algebra routines. There is also a high numerical
         precision calculation mode employing SymPy routines. This gives more accurate
         results for decay chains containing radionuclides with orders of magnitude
         differences between the half-lives.
         
         This is free-to-use open source software. It was created for engineers,
-        technicians and researchers who work with and study radioactivity, and for
+        technicians and researchers who work with radioactivity, and for
         educational use.
         
         - **Full Documentation**: 
         [https://radioactivedecay.github.io/](https://radioactivedecay.github.io/)
         
         
         ## Installation
@@ -134,15 +134,17 @@
         ```pycon
         >>> Mo99_t0.plot(20, 'd', yunits='Bq')
         ```
         
         <img src="https://raw.githubusercontent.com/radioactivedecay/radioactivedecay/main/docs/source/images/Mo-99_decay.png" alt="Mo-99 decay graph" width="450"/>
         
         The graph shows the decay of Mo-99 over 20 days, leading to the ingrowth of
-        Tc-99m and a trace quantity of Tc-99. Graphs are drawn using Matplotlib.
+        Tc-99m and a trace quantity of Tc-99. The activity of Ru-99 is strictly zero as
+        it is the stable nuclide at the end of the decay chain. Graphs are drawn using
+        Matplotlib.
         
         
         ### Fetching decay data
         
         The ``Nuclide`` class can be used to fetch decay information for
         individual radionuclides, e.g. for Rn-222:
         
@@ -243,25 +245,24 @@
         
         By default ``radioactivedecay`` uses decay data from
         [ICRP Publication 107
         (2008)](https://journals.sagepub.com/doi/pdf/10.1177/ANIB_38_3) and atomic mass
         data from the [Atomic Mass Data Center](https://www-nds.iaea.org/amdc/)
         (AMDC - AME2020 and Nubase2020 evaluations).
         
-        The [notebooks
-        directory](https://github.com/radioactivedecay/radioactivedecay/tree/main/notebooks)
-        in the GitHub repository contains Jupyter Notebooks for creating the decay
-        datasets that are read in by ``radioactivedecay``, e.g.
-        [ICRP
-        107](https://github.com/radioactivedecay/radioactivedecay/tree/main/notebooks/icrp107_dataset/icrp107_dataset.ipynb).
-        It also contains some comparisons against decay calculations made with
-        [PyNE](https://github.com/radioactivedecay/radioactivedecay/tree/main/notebooks/comparisons/pyne/rd_pyne_truncated_compare.ipynb)
-        and
-        [Radiological
-        Toolbox](https://github.com/radioactivedecay/radioactivedecay/tree/main/notebooks/comparisons/radiological_toolbox/radiological_toolbox_compare.ipynb).
+        The [datasets repo](https://github.com/radioactivedecay/datasets) contains
+        Jupyter Notebooks for creating decay datasets that can be used by
+        ``radioactivedecay``, e.g. [ICRP
+        107](https://github.com/radioactivedecay/datasets/blob/main/icrp107_ame2020_nubase2020/icrp107_dataset.ipynb).
+        
+        The [comparisons repo](https://github.com/radioactivedecay/comparisons)
+        contains some checks of ``radioactivedecay`` against
+        [PyNE](https://github.com/radioactivedecay/comparisons/blob/main/pyne/rd_pyne_truncated_compare.ipynb)
+        and [Radiological
+        Toolbox](https://github.com/radioactivedecay/comparisons/blob/main/radiological_toolbox/radiological_toolbox_compare.ipynb).
         
         
         ## Tests
         
         From the base directory run:
         
         ```console
```

### Comparing `radioactivedecay-0.4.8/radioactivedecay.egg-info/SOURCES.txt` & `radioactivedecay-0.4.9/radioactivedecay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radioactivedecay-0.4.8/setup.cfg` & `radioactivedecay-0.4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `radioactivedecay-0.4.8/tests/test_decaydata.py` & `radioactivedecay-0.4.9/tests/test_decaydata.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import unittest
 import numpy as np
 from scipy import sparse
 from sympy import Integer, log, Matrix
 from sympy.matrices import SparseMatrix
-from radioactivedecay import converters, decaydata, icrp107_ame2020_nubase2020
+from radioactivedecay import decaydata, icrp107_ame2020_nubase2020
 
 
 class TestFunctions(unittest.TestCase):
     """
     Unit tests for the decaydata.py functions.
     """
 
@@ -25,104 +25,105 @@
         matrix_a = sparse.csr_matrix(([1.0], ([0], [0])), shape=(2, 2))
         matrix_b = sparse.csr_matrix(([1.0], ([0], [0])), shape=(2, 2))
         matrix_c = sparse.csr_matrix(([1.0], ([1], [0])), shape=(2, 2))
         self.assertEqual(decaydata._csr_matrix_equal(matrix_a, matrix_b), True)
         self.assertEqual(decaydata._csr_matrix_equal(matrix_a, matrix_c), False)
 
 
-class TestDecayMatrices(unittest.TestCase):
+class TestDecayMatricesScipy(unittest.TestCase):
     """
-    Unit tests for the decaydata.py DecayMatrices class.
+    Unit tests for the decaydata.py DecayMatricesScipy class.
     """
 
     def test_instantiation(self) -> None:
         """
-        Test instantiation of DecayMatrices objects.
+        Test instantiation of DecayMatricesScipy objects.
         """
 
         atomic_masses = np.array([0.0] * 2)
         decay_consts = np.array([0.0] * 2)
         matrix_c = sparse.csr_matrix(([1.0], ([0], [0])), shape=(2, 2))
         matrix_c_inv = sparse.csr_matrix(([1.0], ([1], [1])), shape=(2, 2))
-        decay_mats = decaydata.DecayMatrices(
+        decay_mats = decaydata.DecayMatricesScipy(
             atomic_masses, decay_consts, matrix_c, matrix_c_inv
         )
         self.assertEqual(decay_mats.atomic_masses[0], 0.0)
         self.assertEqual(decay_mats.atomic_masses[1], 0.0)
         self.assertEqual(decay_mats.decay_consts[0], 0.0)
         self.assertEqual(decay_mats.decay_consts[1], 0.0)
         self.assertEqual(decay_mats.ln2, np.log(2))
         self.assertEqual(decay_mats.matrix_c[0, 0], 1.0)
         self.assertEqual(decay_mats.matrix_c_inv[1, 1], 1.0)
         self.assertEqual(decay_mats.matrix_e[0, 0], 0.0)
         self.assertEqual(decay_mats.matrix_e[1, 1], 0.0)
         self.assertEqual(decay_mats.vector_n0[0], 0.0)
         self.assertEqual(decay_mats.vector_n0[1], 0.0)
 
-    def test_decaymatrices___eq__(self) -> None:
+    def test___eq__(self) -> None:
         """
-        Test DecayMatrices equality.
+        Test DecayMatricesScipy equality.
         """
 
         atomic_masses = np.array([0.0] * 2)
         decay_consts = np.array([0.0] * 2)
         matrix_c = sparse.csr_matrix(([1.0], ([0], [0])), shape=(2, 2))
         matrix_c_inv = sparse.csr_matrix(([1.0], ([0], [0])), shape=(2, 2))
-        decay_mats_a = decaydata.DecayMatrices(
+        decay_mats_a = decaydata.DecayMatricesScipy(
             atomic_masses, decay_consts, matrix_c, matrix_c_inv
         )
         atomic_masses = np.array([0.0] * 2)
         decay_consts = np.array([0.0] * 2)
         matrix_c = sparse.csr_matrix(([1.0], ([0], [0])), shape=(2, 2))
         matrix_c_inv = sparse.csr_matrix(([1.0], ([0], [0])), shape=(2, 2))
-        decay_mats_b = decaydata.DecayMatrices(
+        decay_mats_b = decaydata.DecayMatricesScipy(
             atomic_masses, decay_consts, matrix_c, matrix_c_inv
         )
         self.assertEqual(decay_mats_a, decay_mats_b)
 
         self.assertFalse(decay_mats_a == "random object")
 
-    def test_decaymatrices___ne__(self) -> None:
+    def test___ne__(self) -> None:
         """
-        Test DecayMatrices inequal.
+        Test DecayMatricesScipy inequal.
         """
 
         atomic_masses = np.array([0.0] * 2)
         decay_consts = np.array([0.0] * 2)
         matrix_c = sparse.csr_matrix(([1.0], ([0], [0])), shape=(2, 2))
         matrix_c_inv = sparse.csr_matrix(([1.0], ([0], [0])), shape=(2, 2))
-        decay_mats_a = decaydata.DecayMatrices(
+        decay_mats_a = decaydata.DecayMatricesScipy(
             atomic_masses, decay_consts, matrix_c, matrix_c_inv
         )
         atomic_masses = np.array([0.0] * 2)
         decay_consts = np.array([0.0] * 2)
         matrix_c = sparse.csr_matrix(([1.0], ([0], [0])), shape=(2, 2))
         matrix_c_inv = sparse.csr_matrix(([2.0], ([0], [0])), shape=(2, 2))
-        decay_mats_b = decaydata.DecayMatrices(
+        decay_mats_b = decaydata.DecayMatricesScipy(
             atomic_masses, decay_consts, matrix_c, matrix_c_inv
         )
         self.assertNotEqual(decay_mats_a, decay_mats_b)
 
         self.assertTrue(decay_mats_a != "random object")
 
-    def test_decaymatrices___repr__(self) -> None:
+    def test___repr__(self) -> None:
         """
-        Test DecayMatrices __repr__ strings.
+        Test DecayMatricesScipy __repr__ strings.
         """
 
         atomic_masses = np.array([0.0] * 2)
         decay_consts = np.array([0.0] * 2)
         matrix_c = sparse.csr_matrix(([1.0], ([0], [0])), shape=(2, 2))
         matrix_c_inv = sparse.csr_matrix(([1.0], ([1], [1])), shape=(2, 2))
-        decay_mats = decaydata.DecayMatrices(
+        decay_mats = decaydata.DecayMatricesScipy(
             atomic_masses, decay_consts, matrix_c, matrix_c_inv
         )
         self.assertEqual(
             decay_mats.__repr__(),
-            "DecayMatrices: data stored in SciPy/NumPy objects for double precision calculations.",
+            "DecayMatricesScipy: data stored in SciPy/NumPy objects for double precision "
+            "calculations.",
         )
 
 
 class TestDecayMatricesSympy(unittest.TestCase):
     """
     Unit tests for the decaydata.py DecayMatricesSympy class.
     """
@@ -240,33 +241,33 @@
         dataset_name = "test_dataset"
 
         bfs = np.array([[1.0], []], dtype=object)
         hldata = np.array([[2.0, "h", "2.0 h"], [np.inf, "s", "stable"]], dtype=object)
         modes = np.array([["\u03b2+"], []], dtype=object)
         nuclides = np.array(["A-2", "B-1"])
         progeny = np.array([["B-1"], []], dtype=object)
-        float_unit_converter = converters.UnitConverterFloat(365.2422)
+        float_year_conv = 365.2422
 
         atomic_masses = np.array([0.0] * 2)
         decay_consts = np.array([0.0] * 2)
         matrix_c = sparse.csr_matrix(([1.0], ([0], [0])), shape=(2, 2))
         matrix_c_inv = sparse.csr_matrix(([1.0], ([1], [1])), shape=(2, 2))
-        decay_mats = decaydata.DecayMatrices(
+        decay_mats = decaydata.DecayMatricesScipy(
             atomic_masses, decay_consts, matrix_c, matrix_c_inv
         )
 
         dataset = decaydata.DecayData(
             dataset_name,
             bfs,
+            float_year_conv,
             hldata,
             modes,
             nuclides,
             progeny,
             decay_mats,
-            float_unit_converter,
         )
 
         self.assertEqual(dataset.dataset_name, "test_dataset")
         self.assertEqual(dataset.hldata[0][0], 2.0)
         self.assertEqual(dataset.hldata[0][1], "h")
         self.assertEqual(dataset.hldata[0][2], "2.0 h")
         self.assertEqual(dataset.hldata[-1][0], np.inf)
@@ -278,50 +279,45 @@
         self.assertEqual(dataset.nuclide_dict["B-1"], 1)
         self.assertEqual(dataset.progeny[0][0], "B-1")
         self.assertEqual(dataset.bfs[0][0], 1.0)
         self.assertEqual(dataset.modes[0][0], "\u03b2+")
         self.assertEqual(dataset.progeny[-1], [])
         self.assertEqual(dataset.bfs[-1], [])
         self.assertEqual(dataset.modes[-1], [])
-        self.assertEqual(
-            dataset.float_unit_converter, converters.UnitConverterFloat(365.2422)
-        )
-        self.assertIsNotNone(dataset.float_quantity_converter)
-        self.assertIsNone(dataset.sympy_data)
-        self.assertIsNone(dataset.sympy_unit_converter)
-        self.assertIsNone(dataset.sympy_quantity_converter)
+        self.assertEqual(dataset.float_year_conv, 365.2422)
+        with self.assertRaises(ValueError):
+            assert dataset.sympy_data
+        with self.assertRaises(ValueError):
+            assert dataset.sympy_year_conv
 
         atomic_masses_sympy = Matrix.zeros(2, 1)
         decay_consts_sympy = Matrix.zeros(2, 1)
         matrix_c_sympy = SparseMatrix.zeros(2, 2)
         matrix_c_sympy[0, 0] = Integer(2)
         matrix_c_inv_sympy = SparseMatrix.zeros(2, 2)
         matrix_c_inv_sympy[1, 1] = Integer(3)
         decay_mats_sympy = decaydata.DecayMatricesSympy(
             atomic_masses_sympy, decay_consts_sympy, matrix_c_sympy, matrix_c_inv_sympy
         )
-        sympy_unit_converter = converters.UnitConverterSympy(
-            Integer(3652422) / Integer(1000)
-        )
+        sympy_year_conv = Integer(3652422) / Integer(10000)
 
         dataset = decaydata.DecayData(
             dataset_name,
             bfs,
+            float_year_conv,
             hldata,
             modes,
             nuclides,
             progeny,
             decay_mats,
-            float_unit_converter,
             decay_mats_sympy,
-            sympy_unit_converter,
+            sympy_year_conv,
         )
         self.assertIsNotNone(dataset.sympy_data)
-        self.assertIsNotNone(dataset.sympy_unit_converter)
-        self.assertIsNotNone(dataset.sympy_quantity_converter)
+        self.assertIsNotNone(dataset.sympy_year_conv)
 
     def test_half_life(self) -> None:
         """
         Test DecayData half_life() method.
         """
 
         data = decaydata.load_dataset("icrp107_ame2020_nubase2020")
@@ -438,15 +434,18 @@
         self.assertEqual(data.scipy_data.matrix_c.shape, (1498, 1498))
         self.assertEqual(data.scipy_data.matrix_c[0, 0], 1.0)
         self.assertEqual(data.scipy_data.matrix_c_inv.shape, (1498, 1498))
         self.assertEqual(data.scipy_data.matrix_c_inv[0, 0], 1.0)
         self.assertEqual(data.scipy_data.matrix_e.shape, (1498, 1498))
         self.assertEqual(data.scipy_data.matrix_e[0, 0], 0.0)
         self.assertEqual(data.scipy_data.vector_n0[0], 0.0)
-        self.assertEqual(data.sympy_data, None)
+        with self.assertRaises(ValueError):
+            assert data.sympy_data
+        with self.assertRaises(ValueError):
+            assert data.sympy_year_conv
 
         # check instantiation with supplied dataset path
         data = decaydata.load_dataset(
             "icrp107_ame2020_nubase2020_2",
             icrp107_ame2020_nubase2020.__path__[0],
             load_sympy=False,
         )
@@ -477,15 +476,18 @@
         self.assertEqual(data.scipy_data.matrix_c.shape, (1498, 1498))
         self.assertEqual(data.scipy_data.matrix_c[0, 0], 1.0)
         self.assertEqual(data.scipy_data.matrix_c_inv.shape, (1498, 1498))
         self.assertEqual(data.scipy_data.matrix_c_inv[0, 0], 1.0)
         self.assertEqual(data.scipy_data.matrix_e.shape, (1498, 1498))
         self.assertEqual(data.scipy_data.matrix_e[0, 0], 0.0)
         self.assertEqual(data.scipy_data.vector_n0[0], 0.0)
-        self.assertEqual(data.sympy_data, None)
+        with self.assertRaises(ValueError):
+            assert data.sympy_data
+        with self.assertRaises(ValueError):
+            assert data.sympy_year_conv
 
         # check instantiation from sub-package with SymPy data
         data = decaydata.load_dataset("icrp107_ame2020_nubase2020", load_sympy=True)
         self.assertEqual(data.dataset_name, "icrp107_ame2020_nubase2020")
         self.assertEqual(data.hldata[0][0], 100.5)
         self.assertEqual(data.hldata[0][1], "d")
         self.assertEqual(data.hldata[0][2], "100.5 d")
@@ -524,14 +526,15 @@
         self.assertEqual(data.sympy_data.matrix_c.shape, (1498, 1498))
         self.assertEqual(data.sympy_data.matrix_c[0, 0], Integer(1))
         self.assertEqual(data.sympy_data.matrix_c_inv.shape, (1498, 1498))
         self.assertEqual(data.sympy_data.matrix_c_inv[0, 0], Integer(1))
         self.assertEqual(data.sympy_data.matrix_e.shape, (1498, 1498))
         self.assertEqual(data.sympy_data.matrix_e[0, 0], Integer(0))
         self.assertEqual(data.sympy_data.vector_n0[0], Integer(0))
+        self.assertEqual(data.sympy_year_conv, Integer(3652422) / Integer(10000))
 
         # check instantiation with supplied dataset path with SymPy data
         data = decaydata.load_dataset(
             "icrp107_ame2020_nubase2020_2",
             icrp107_ame2020_nubase2020.__path__[0],
             load_sympy=True,
         )
@@ -574,11 +577,12 @@
         self.assertEqual(data.sympy_data.matrix_c.shape, (1498, 1498))
         self.assertEqual(data.sympy_data.matrix_c[0, 0], Integer(1))
         self.assertEqual(data.sympy_data.matrix_c_inv.shape, (1498, 1498))
         self.assertEqual(data.sympy_data.matrix_c_inv[0, 0], Integer(1))
         self.assertEqual(data.sympy_data.matrix_e.shape, (1498, 1498))
         self.assertEqual(data.sympy_data.matrix_e[0, 0], Integer(0))
         self.assertEqual(data.sympy_data.vector_n0[0], Integer(0))
+        self.assertEqual(data.sympy_year_conv, Integer(3652422) / Integer(10000))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `radioactivedecay-0.4.8/tests/test_inventory.py` & `radioactivedecay-0.4.9/tests/test_inventory.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,14 @@
         """
 
         # check basic instantiation
         inv = Inventory({"H3": 1}, "num", True)
         self.assertEqual(inv.contents, {"H-3": 1})
         self.assertEqual(inv.decay_data, DEFAULTDATA)
         self.assertEqual(inv.decay_matrices, DEFAULTDATA.scipy_data)
-        self.assertEqual(inv.quantity_converter, DEFAULTDATA.float_quantity_converter)
-        self.assertEqual(inv.unit_converter, DEFAULTDATA.float_unit_converter)
 
         # check instantiation using Nuclide instance
         tritium = Nuclide("H3")
         inv = Inventory({tritium: 1.0}, "num", True)
         self.assertEqual(inv.contents, {"H-3": 1})
 
         # check that check=False turns off nuclide string convertion and quantity check
@@ -93,40 +91,39 @@
             Inventory._check_values({"H-3": "1"})
 
     def test__convert_to_number(self) -> None:
         """
         Test that the contents dictionary values (amounts of each nuclide) are physical.
         """
 
-        qconv = DEFAULTDATA.float_quantity_converter
-        uconv = DEFAULTDATA.float_unit_converter
+        inv = Inventory({"H3": 1}, "num", True)
         self.assertEqual(
-            Inventory._convert_to_number({"H-3": 1.0}, "num", qconv, uconv),
+            inv._convert_to_number({"H-3": 1.0}, "num"),
             {"H-3": 1.0},
         )
         self.assertEqual(
-            Inventory._convert_to_number({"H-3": 1.0}, "Bq", qconv, uconv),
+            inv._convert_to_number({"H-3": 1.0}, "Bq"),
             {"H-3": 560892895.7794082},
         )
         self.assertEqual(
-            Inventory._convert_to_number({"H-3": 1.0}, "mBq", qconv, uconv),
+            inv._convert_to_number({"H-3": 1.0}, "mBq"),
             {"H-3": 560892.8957794083},
         )
         self.assertEqual(
-            Inventory._convert_to_number({"H-3": 1.0}, "mol", qconv, uconv),
+            inv._convert_to_number({"H-3": 1.0}, "mol"),
             {"H-3": 6.02214076e23},
         )
         self.assertEqual(
-            Inventory._convert_to_number({"He-3": 1.0}, "kg", qconv, uconv),
+            inv._convert_to_number({"He-3": 1.0}, "kg"),
             {"He-3": 1.9967116089131648e26},
         )
 
         # check catch of incorrect units
         with self.assertRaises(ValueError):
-            Inventory._convert_to_number({"H-3": 1.0}, "xyz", qconv, uconv)
+            inv._convert_to_number({"H-3": 1.0}, "xyz")
 
     def test_nuclides(self) -> None:
         """
         Test Inventory.nuclides property.
         """
 
         inv = Inventory({"H-3": 1.0})
@@ -667,25 +664,22 @@
 
         inv = InventoryHP({"H3": 1}, "Bq", True)
         self.assertEqual(
             inv.contents, {"H-3": Integer(242988330816) / (Integer(625) * log(2))}
         )
         self.assertEqual(inv.decay_data, DEFAULTDATA)
         self.assertEqual(inv.decay_matrices, DEFAULTDATA.sympy_data)
-        self.assertEqual(inv.quantity_converter, DEFAULTDATA.sympy_quantity_converter)
-        self.assertEqual(inv.unit_converter, DEFAULTDATA.sympy_unit_converter)
 
         temp_data = copy.deepcopy(DEFAULTDATA)
-        temp_data.sympy_unit_converter = None
-        with self.assertRaises(ValueError):
-            InventoryHP({"H3": 1}, "Bq", True, temp_data)
-        temp_data.sympy_quantity_converter = None
+        backup_year_conv = temp_data._sympy_year_conv
+        temp_data._sympy_year_conv = None
         with self.assertRaises(ValueError):
             InventoryHP({"H3": 1}, "Bq", True, temp_data)
-        temp_data.sympy_data = None
+        temp_data._sympy_year_conv = backup_year_conv
+        temp_data._sympy_data = None
         with self.assertRaises(ValueError):
             InventoryHP({"H3": 1}, "Bq", True, temp_data)
 
     def test_numbers(self) -> None:
         """
         Test InventoryHP.numbers() method.
         """
```

### Comparing `radioactivedecay-0.4.8/tests/test_nuclide.py` & `radioactivedecay-0.4.9/tests/test_nuclide.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,101 +12,116 @@
     Unit tests for the nuclide.py Nuclide class.
     """
 
     def test_nuclide_instantiation(self) -> None:
         """
         Test instantiation of Nuclide objects.
         """
+        decay_data = load_dataset("icrp107_ame2020_nubase2020", load_sympy=True)
 
         nuc = Nuclide("Rn-222")
         self.assertEqual(nuc.nuclide, "Rn-222")
-        self.assertEqual(nuc.prog, ["Po-218"])
-        self.assertEqual(nuc.bfs, [1.0])
-        self.assertEqual(nuc.modes, ["\u03b1"])
+        self.assertEqual(nuc.decay_data, decay_data)
 
         nuc = Nuclide("222Rn")
         self.assertEqual(nuc.nuclide, "Rn-222")
-        self.assertEqual(nuc.prog, ["Po-218"])
-        self.assertEqual(nuc.bfs, [1.0])
-        self.assertEqual(nuc.modes, ["\u03b1"])
 
         nuc = Nuclide(611450000)
         self.assertEqual(nuc.nuclide, "Pm-145")
-        self.assertEqual(nuc.prog, ["Nd-145", "Pr-141"])
-        self.assertEqual(nuc.bfs, [1.0, 2.8e-09])
-        self.assertEqual(nuc.modes, ["EC", "\u03b1"])
 
     def test_nuclide_Z(self) -> None:
         """
-        Test Nuclide Z attribute.
+        Test Nuclide Z property.
         """
 
         nuc = Nuclide("H-3")
         self.assertEqual(nuc.Z, 1)
 
     def test_nuclide_A(self) -> None:
         """
-        Test Nuclide A attribute.
+        Test Nuclide A property.
         """
 
         nuc = Nuclide("H-3")
         self.assertEqual(nuc.A, 3)
 
+    def test_nuclide_state(self) -> None:
+        """
+        Test Nuclide state property.
+        """
+
+        nuc = Nuclide("H-3")
+        self.assertEqual(nuc.state, "")
+
+        nuc = Nuclide("Ba-137m")
+        self.assertEqual(nuc.state, "m")
+
+        nuc = Nuclide("Ir-192n")
+        self.assertEqual(nuc.state, "n")
+
     def test_nuclide_id(self) -> None:
         """
-        Test Nuclide id attribute.
+        Test Nuclide id property.
         """
 
         nuc = Nuclide("H-3")
         self.assertEqual(nuc.id, 10030000)
 
         nuc = Nuclide("I-118m")
         self.assertEqual(nuc.id, 531180001)
 
         nuc = Nuclide(190400000)
         self.assertEqual(nuc.id, 190400000)
 
-    def test_radionuclide_half_life(self) -> None:
+    def test_nuclide_atomic_mass(self) -> None:
+        """
+        Test Nuclide atomic_mass property.
+        """
+
+        nuc = Nuclide("H-3")
+        self.assertEqual(nuc.atomic_mass, 3.01604928132)
+
+    def test_nuclide_half_life(self) -> None:
         """
         Test Nuclide half_life() method.
         """
 
         nuc = Nuclide("H-3")
         self.assertEqual(nuc.half_life(), 388781329.30560005)
         self.assertEqual(nuc.half_life("y"), 12.32)
         self.assertEqual(nuc.half_life("readable"), "12.32 y")
 
-    def test_radionuclide_progeny(self) -> None:
+    def test_nuclide_progeny(self) -> None:
         """
-        Test Nuclide half_life() method.
+        Test Nuclide progeny() method.
         """
 
         nuc = Nuclide("K-40")
         self.assertEqual(nuc.progeny()[0], "Ca-40")
         self.assertEqual(nuc.progeny()[1], "Ar-40")
 
-    def test_radionuclide_branching_fractions(self) -> None:
+    def test_nuclide_branching_fractions(self) -> None:
         """
         Test Nuclide branching_fractions() method.
         """
 
         nuc = Nuclide("K-40")
         self.assertEqual(nuc.branching_fractions()[0], 0.8914)
         self.assertEqual(nuc.branching_fractions()[1], 0.1086)
 
-    def test_radionuclide_decay_modes(self) -> None:
+    def test_nuclide_decay_modes(self) -> None:
         """
         Test Nuclide decay_modes() method.
         """
 
         nuc = Nuclide("K-40")
         self.assertEqual(nuc.decay_modes()[0], "\u03b2-")
         self.assertEqual(nuc.decay_modes()[1], "\u03b2+ & EC")
 
-    def test_radionuclide_plot(self) -> None:
+    def test_nuclide_plot(self) -> None:
         """
         Test Nuclide plot() method.
 
         Only testing auto-generation of limits so far.
         """
 
         nuc = Nuclide("H-3")
@@ -125,15 +140,15 @@
         self.assertEqual(axes.get_ylim(), (-19.3, 0.3))
 
         nuc = Nuclide("Cu-64")
         _, axes = nuc.plot()
         self.assertEqual(axes.get_xlim(), (-0.3, 1.3))
         self.assertEqual(axes.get_ylim(), (-1.3, 0.3))
 
-    def test_radionuclide___repr__(self) -> None:
+    def test_nuclide___repr__(self) -> None:
         """
         Test Nuclide __repr__ strings.
         """
 
         nuc = Nuclide("H-3")
         self.assertEqual(
             nuc.__repr__(),
@@ -153,26 +168,26 @@
 
         decay_data = load_dataset("icrp107_ame2020_nubase2020", load_sympy=True)
         nuc2 = Nuclide("K-40", decay_data)
         self.assertEqual(nuc1, nuc2)
 
         self.assertFalse(nuc1 == "random object")
 
-    def test_radionuclide___ne__(self) -> None:
+    def test_nuclide___ne__(self) -> None:
         """
         Test Nuclide inequality.
         """
 
         nuc1 = Nuclide("K-40")
         nuc2 = Nuclide("H-3")
         self.assertNotEqual(nuc1, nuc2)
 
         self.assertTrue(nuc1 != "random object")
 
-    def test_radionuclide___hash__(self) -> None:
+    def test_nuclide___hash__(self) -> None:
         """
         Test Nuclide hash function.
         """
 
         nuc = Nuclide("K-40")
         decay_data = load_dataset("icrp107_ame2020_nubase2020", load_sympy=True)
         self.assertEqual(hash(nuc), hash(("K-40", decay_data.dataset_name)))
```

### Comparing `radioactivedecay-0.4.8/tests/test_plots.py` & `radioactivedecay-0.4.9/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `radioactivedecay-0.4.8/tests/test_utils.py` & `radioactivedecay-0.4.9/tests/test_utils.py`

 * *Files identical despite different names*

