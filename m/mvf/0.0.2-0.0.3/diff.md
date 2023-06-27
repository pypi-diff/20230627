# Comparing `tmp/mvf-0.0.2.tar.gz` & `tmp/mvf-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvf-0.0.2.tar", last modified: Fri Jun 23 15:47:38 2023, max compression
+gzip compressed data, was "mvf-0.0.3.tar", last modified: Tue Jun 27 14:42:50 2023, max compression
```

## Comparing `mvf-0.0.2.tar` & `mvf-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:47:38.876420 mvf-0.0.2/
--rw-rw-rw-   0 root         (0) root         (0)      798 2023-06-23 15:47:35.000000 mvf-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2871 2023-06-23 15:47:38.875420 mvf-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2301 2023-06-23 15:47:35.000000 mvf-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:47:38.875420 mvf-0.0.2/mvf.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2871 2023-06-23 15:47:38.000000 mvf-0.0.2/mvf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      198 2023-06-23 15:47:38.000000 mvf-0.0.2/mvf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 15:47:38.000000 mvf-0.0.2/mvf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-06-23 15:47:38.000000 mvf-0.0.2/mvf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 15:47:38.000000 mvf-0.0.2/mvf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 15:47:38.876420 mvf-0.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1378 2023-06-23 15:47:35.000000 mvf-0.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:47:38.875420 mvf-0.0.2/test/
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-23 15:47:35.000000 mvf-0.0.2/test/test_python_testing_framework.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.808687 mvf-0.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-06-27 14:42:47.000000 mvf-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3135 2023-06-27 14:42:50.808687 mvf-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2565 2023-06-27 14:42:47.000000 mvf-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.801687 mvf-0.0.3/mvf/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.803687 mvf-0.0.3/mvf/cli/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1543 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/cli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.803687 mvf-0.0.3/mvf/dag/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/dag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7144 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/dag/builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.804687 mvf-0.0.3/mvf/process/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1384 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/process/fit_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1611 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/process/predict_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1702 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/process/split_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      771 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/process/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/process/validate_model_r.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.804687 mvf-0.0.3/mvf/test/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.804687 mvf-0.0.3/mvf/test/integration/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.806687 mvf-0.0.3/mvf/test/integration/config/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2878 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/config/fit_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1208 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/config/mvf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/config/predict_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/config/preprocess_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1956 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/config/split_data.py
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/config/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/config/validate_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.807687 mvf-0.0.3/mvf/test/integration/process/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/process/fit_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/process/predict_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/process/preprocess_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2977 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/process/split_data.py
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/process/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/process/validate_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.802687 mvf-0.0.3/mvf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3135 2023-06-27 14:42:50.000000 mvf-0.0.3/mvf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-06-27 14:42:50.000000 mvf-0.0.3/mvf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 14:42:50.000000 mvf-0.0.3/mvf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-06-27 14:42:50.000000 mvf-0.0.3/mvf.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       99 2023-06-27 14:42:50.000000 mvf-0.0.3/mvf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-27 14:42:50.000000 mvf-0.0.3/mvf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 14:42:50.808687 mvf-0.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2023-06-27 14:42:47.000000 mvf-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.808687 mvf-0.0.3/test/
+-rw-rw-rw-   0 root         (0) root         (0)     5868 2023-06-27 14:42:47.000000 mvf-0.0.3/test/test_build_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-27 14:42:47.000000 mvf-0.0.3/test/test_python_testing_framework.py
```

### Comparing `mvf-0.0.2/LICENSE` & `mvf-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mvf-0.0.2/PKG-INFO` & `mvf-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvf
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package implementing a supervised learning model validation framework.
 Home-page: UNKNOWN
 Author: Tom Kim
 Author-email: tom.kim@certus-tech.com
 License: UNKNOWN
 Keywords: python,R,machine learning,validation,framework
 Platform: UNKNOWN
@@ -13,21 +13,25 @@
 Classifier: License :: Free For Educational Use
 Classifier: Operating System :: Unix
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-description here...
+MVF stands for model validation framework. MVF is a pluggable ML/statistical modelling framework that allows for the easy comparison of models implemented in Python and R. Write simple wrapper classes for your models and compare their performance on a particular dataset.
 
-## Getting Started
+## Getting started
 
 For full documentation of the project and instructions on how to get started, visit the [documentation site](https://tomkimcta.gitlab.io/model-validation-framework).
 
-## Project Administration
+## Main features
+
+
+
+## For developers
 
 ### Dependencies
 
 R dependencies are managed using `renv`. Spin up a Python Virtual Environment
 
 Python dependencies are specified by `requirements.txt`. This file is generated from `requirements.in` by running `python3 -m piptools compile`.
```

### Comparing `mvf-0.0.2/README.md` & `mvf-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-description here...
+MVF stands for model validation framework. MVF is a pluggable ML/statistical modelling framework that allows for the easy comparison of models implemented in Python and R. Write simple wrapper classes for your models and compare their performance on a particular dataset.
 
-## Getting Started
+## Getting started
 
 For full documentation of the project and instructions on how to get started, visit the [documentation site](https://tomkimcta.gitlab.io/model-validation-framework).
 
-## Project Administration
+## Main features
+
+
+
+## For developers
 
 ### Dependencies
 
 R dependencies are managed using `renv`. Spin up a Python Virtual Environment
 
 Python dependencies are specified by `requirements.txt`. This file is generated from `requirements.in` by running `python3 -m piptools compile`.
```

### Comparing `mvf-0.0.2/mvf.egg-info/PKG-INFO` & `mvf-0.0.3/mvf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvf
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package implementing a supervised learning model validation framework.
 Home-page: UNKNOWN
 Author: Tom Kim
 Author-email: tom.kim@certus-tech.com
 License: UNKNOWN
 Keywords: python,R,machine learning,validation,framework
 Platform: UNKNOWN
@@ -13,21 +13,25 @@
 Classifier: License :: Free For Educational Use
 Classifier: Operating System :: Unix
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-description here...
+MVF stands for model validation framework. MVF is a pluggable ML/statistical modelling framework that allows for the easy comparison of models implemented in Python and R. Write simple wrapper classes for your models and compare their performance on a particular dataset.
 
-## Getting Started
+## Getting started
 
 For full documentation of the project and instructions on how to get started, visit the [documentation site](https://tomkimcta.gitlab.io/model-validation-framework).
 
-## Project Administration
+## Main features
+
+
+
+## For developers
 
 ### Dependencies
 
 R dependencies are managed using `renv`. Spin up a Python Virtual Environment
 
 Python dependencies are specified by `requirements.txt`. This file is generated from `requirements.in` by running `python3 -m piptools compile`.
```

### Comparing `mvf-0.0.2/setup.py` & `mvf-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,22 +23,27 @@
     long_description=_get_long_description(),
     long_description_content_type='text/markdown',
     packages=find_packages(
         exclude=[
             'test*',
             'documentation*',
             'examples*',
-        ]
+        ],
     ),
+    # package_dir={
+    #     '': 'mvf'
+    # },
     install_requires=[
+        'click',
         'feather-format',
         'pandas',
         'ploomber',
         'rpy2',
         'rpy2-r6',
+        'schema',
         'scikit-learn',
     ],
     extras_require={
         'dev': [
             'coverage',
             'pytest',
             'twine',
@@ -54,8 +59,13 @@
     classifiers=[
         'Programming Language :: Python :: 3.9',
         'Framework :: Jupyter',
         'License :: Free For Educational Use',
         'Operating System :: Unix',
     ],
     python_requires='>=3.9',
+    entry_points={
+        'console_scripts': [
+            'mvf=mvf.cli.cli:cmd_router'
+        ]
+    },
 )
```

