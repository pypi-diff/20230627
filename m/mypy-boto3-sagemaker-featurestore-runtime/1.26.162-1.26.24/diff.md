# Comparing `tmp/mypy-boto3-sagemaker-featurestore-runtime-1.26.162.tar.gz` & `tmp/mypy-boto3-sagemaker-featurestore-runtime-1.26.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-featurestore-runtime-1.26.162.tar", last modified: Tue Jun 27 21:23:12 2023, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-featurestore-runtime-1.26.24.tar", last modified: Tue Dec  6 20:25:48 2022, max compression
```

## Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.26.162.tar` & `mypy-boto3-sagemaker-featurestore-runtime-1.26.24.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:23:12.866127 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-27 21:22:19.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-06-27 21:23:12.866127 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-06-27 21:22:19.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:23:12.858127 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-27 21:22:19.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-27 21:22:19.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-27 21:22:19.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-06-27 21:22:19.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-06-27 21:22:19.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-06-27 21:22:19.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-06-27 21:22:19.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:22:19.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-06-27 21:22:19.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-06-27 21:22:19.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-27 21:22:19.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:23:12.866127 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-06-27 21:23:12.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-27 21:23:12.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:23:12.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:23:12.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-27 21:23:12.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-27 21:23:12.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 21:23:12.866127 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-27 21:22:19.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.162/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:25:48.481958 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-12-06 20:25:38.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    13320 2022-12-06 20:25:48.477958 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11793 2022-12-06 20:25:38.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:25:48.473957 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2022-12-06 20:25:38.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2022-12-06 20:25:38.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2022-12-06 20:25:38.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6344 2022-12-06 20:25:38.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6334 2022-12-06 20:25:38.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     7326 2022-12-06 20:25:38.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7324 2022-12-06 20:25:38.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-06 20:25:38.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     4802 2022-12-06 20:25:39.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4793 2022-12-06 20:25:38.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2022-12-06 20:25:38.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:25:48.477958 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    13320 2022-12-06 20:25:48.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1006 2022-12-06 20:25:48.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-06 20:25:48.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-06 20:25:48.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2022-12-06 20:25:48.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2022-12-06 20:25:48.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-06 20:25:48.481958 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2197 2022-12-06 20:25:38.000000 mypy-boto3-sagemaker-featurestore-runtime-1.26.24/setup.py
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.26.162/LICENSE` & `mypy-boto3-sagemaker-featurestore-runtime-1.26.24/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.26.162/PKG-INFO` & `mypy-boto3-sagemaker-featurestore-runtime-1.26.24/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-featurestore-runtime
-Version: 1.26.162
-Summary: Type annotations for boto3.SageMakerFeatureStoreRuntime 1.26.162 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.24
+Summary: Type annotations for boto3.SageMakerFeatureStoreRuntime 1.26.24 service generated with mypy-boto3-builder 7.11.11
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,44 +18,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-sagemaker-featurestore-runtime"></a>
 
 # mypy-boto3-sagemaker-featurestore-runtime
 
 [![PyPI - mypy-boto3-sagemaker-featurestore-runtime](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-featurestore-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-featurestore-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerFeatureStoreRuntime 1.26.162](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
+[boto3.SageMakerFeatureStoreRuntime 1.26.24](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sagemaker-featurestore-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -277,25 +276,22 @@
 ### Literals
 
 `mypy_boto3_sagemaker_featurestore_runtime.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_sagemaker_featurestore_runtime.literals import (
-    DeletionModeType,
-    ExpirationTimeResponseType,
     TargetStoreType,
-    TtlDurationUnitType,
     SageMakerFeatureStoreRuntimeServiceName,
     ServiceName,
     ResourceServiceName,
 )
 
 
-def check_value(value: DeletionModeType) -> bool:
+def check_value(value: TargetStoreType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
@@ -307,15 +303,14 @@
 from mypy_boto3_sagemaker_featurestore_runtime.type_defs import (
     BatchGetRecordErrorTypeDef,
     BatchGetRecordIdentifierTypeDef,
     ResponseMetadataTypeDef,
     FeatureValueTypeDef,
     DeleteRecordRequestRequestTypeDef,
     GetRecordRequestRequestTypeDef,
-    TtlDurationTypeDef,
     BatchGetRecordRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     BatchGetRecordResultDetailTypeDef,
     GetRecordResponseTypeDef,
     PutRecordRequestRequestTypeDef,
     BatchGetRecordResponseTypeDef,
 )
@@ -328,42 +323,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.26.162/README.md` & `mypy-boto3-sagemaker-featurestore-runtime-1.26.24/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sagemaker-featurestore-runtime"></a>
 
 # mypy-boto3-sagemaker-featurestore-runtime
 
 [![PyPI - mypy-boto3-sagemaker-featurestore-runtime](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-featurestore-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-featurestore-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerFeatureStoreRuntime 1.26.162](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
+[boto3.SageMakerFeatureStoreRuntime 1.26.24](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sagemaker-featurestore-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -245,25 +245,22 @@
 ### Literals
 
 `mypy_boto3_sagemaker_featurestore_runtime.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_sagemaker_featurestore_runtime.literals import (
-    DeletionModeType,
-    ExpirationTimeResponseType,
     TargetStoreType,
-    TtlDurationUnitType,
     SageMakerFeatureStoreRuntimeServiceName,
     ServiceName,
     ResourceServiceName,
 )
 
 
-def check_value(value: DeletionModeType) -> bool:
+def check_value(value: TargetStoreType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
@@ -275,15 +272,14 @@
 from mypy_boto3_sagemaker_featurestore_runtime.type_defs import (
     BatchGetRecordErrorTypeDef,
     BatchGetRecordIdentifierTypeDef,
     ResponseMetadataTypeDef,
     FeatureValueTypeDef,
     DeleteRecordRequestRequestTypeDef,
     GetRecordRequestRequestTypeDef,
-    TtlDurationTypeDef,
     BatchGetRecordRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     BatchGetRecordResultDetailTypeDef,
     GetRecordResponseTypeDef,
     PutRecordRequestRequestTypeDef,
     BatchGetRecordResponseTypeDef,
 )
@@ -296,42 +292,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/__init__.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/__init__.pyi` & `mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/__main__.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SageMakerFeatureStoreRuntime 1.26.162\nVersion:        "
-        " 1.26.162\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.SageMakerFeatureStoreRuntime 1.26.24\nVersion:        "
+        " 1.26.24\nBuilder version: 7.11.11\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.162")
+    print("1.26.24")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/client.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,22 +13,21 @@
     client: SageMakerFeatureStoreRuntimeClient = session.client("sagemaker-featurestore-runtime")
     ```
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import DeletionModeType, ExpirationTimeResponseType, TargetStoreType
+from .literals import TargetStoreType
 from .type_defs import (
     BatchGetRecordIdentifierTypeDef,
     BatchGetRecordResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FeatureValueTypeDef,
     GetRecordResponseTypeDef,
-    TtlDurationTypeDef,
 )
 
 __all__ = ("SageMakerFeatureStoreRuntimeClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -61,21 +60,18 @@
         SageMakerFeatureStoreRuntimeClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/client/#exceptions)
         """
 
     def batch_get_record(
-        self,
-        *,
-        Identifiers: Sequence[BatchGetRecordIdentifierTypeDef],
-        ExpirationTimeResponse: ExpirationTimeResponseType = ...
+        self, *, Identifiers: Sequence[BatchGetRecordIdentifierTypeDef]
     ) -> BatchGetRecordResponseTypeDef:
         """
-        Retrieves a batch of `Records` from a `FeatureGroup`.
+        Retrieves a batch of `Records` from a `FeatureGroup` .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.batch_get_record)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/client/#batch_get_record)
         """
 
     def can_paginate(self, operation_name: str) -> bool:
         """
@@ -95,19 +91,18 @@
 
     def delete_record(
         self,
         *,
         FeatureGroupName: str,
         RecordIdentifierValueAsString: str,
         EventTime: str,
-        TargetStores: Sequence[TargetStoreType] = ...,
-        DeletionMode: DeletionModeType = ...
+        TargetStores: Sequence[TargetStoreType] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes a `Record` from a `FeatureGroup` in the `OnlineStore`.
+        Deletes a `Record` from a `FeatureGroup`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.delete_record)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/client/#delete_record)
         """
 
     def generate_presigned_url(
         self,
@@ -124,31 +119,29 @@
         """
 
     def get_record(
         self,
         *,
         FeatureGroupName: str,
         RecordIdentifierValueAsString: str,
-        FeatureNames: Sequence[str] = ...,
-        ExpirationTimeResponse: ExpirationTimeResponseType = ...
+        FeatureNames: Sequence[str] = ...
     ) -> GetRecordResponseTypeDef:
         """
         Use for `OnlineStore` serving from a `FeatureStore`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.get_record)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/client/#get_record)
         """
 
     def put_record(
         self,
         *,
         FeatureGroupName: str,
         Record: Sequence[FeatureValueTypeDef],
-        TargetStores: Sequence[TargetStoreType] = ...,
-        TtlDuration: TtlDurationTypeDef = ...
+        TargetStores: Sequence[TargetStoreType] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used for data ingestion into the `FeatureStore`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.put_record)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/client/#put_record)
         """
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/client.pyi` & `mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/client.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -13,22 +13,21 @@
     client: SageMakerFeatureStoreRuntimeClient = session.client("sagemaker-featurestore-runtime")
     ```
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import DeletionModeType, ExpirationTimeResponseType, TargetStoreType
+from .literals import TargetStoreType
 from .type_defs import (
     BatchGetRecordIdentifierTypeDef,
     BatchGetRecordResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FeatureValueTypeDef,
     GetRecordResponseTypeDef,
-    TtlDurationTypeDef,
 )
 
 __all__ = ("SageMakerFeatureStoreRuntimeClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -57,21 +56,18 @@
         """
         SageMakerFeatureStoreRuntimeClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/client/#exceptions)
         """
     def batch_get_record(
-        self,
-        *,
-        Identifiers: Sequence[BatchGetRecordIdentifierTypeDef],
-        ExpirationTimeResponse: ExpirationTimeResponseType = ...
+        self, *, Identifiers: Sequence[BatchGetRecordIdentifierTypeDef]
     ) -> BatchGetRecordResponseTypeDef:
         """
-        Retrieves a batch of `Records` from a `FeatureGroup`.
+        Retrieves a batch of `Records` from a `FeatureGroup` .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.batch_get_record)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/client/#batch_get_record)
         """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
@@ -88,19 +84,18 @@
         """
     def delete_record(
         self,
         *,
         FeatureGroupName: str,
         RecordIdentifierValueAsString: str,
         EventTime: str,
-        TargetStores: Sequence[TargetStoreType] = ...,
-        DeletionMode: DeletionModeType = ...
+        TargetStores: Sequence[TargetStoreType] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes a `Record` from a `FeatureGroup` in the `OnlineStore`.
+        Deletes a `Record` from a `FeatureGroup`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.delete_record)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/client/#delete_record)
         """
     def generate_presigned_url(
         self,
         ClientMethod: str,
@@ -115,30 +110,28 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/client/#generate_presigned_url)
         """
     def get_record(
         self,
         *,
         FeatureGroupName: str,
         RecordIdentifierValueAsString: str,
-        FeatureNames: Sequence[str] = ...,
-        ExpirationTimeResponse: ExpirationTimeResponseType = ...
+        FeatureNames: Sequence[str] = ...
     ) -> GetRecordResponseTypeDef:
         """
         Use for `OnlineStore` serving from a `FeatureStore`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.get_record)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/client/#get_record)
         """
     def put_record(
         self,
         *,
         FeatureGroupName: str,
         Record: Sequence[FeatureValueTypeDef],
-        TargetStores: Sequence[TargetStoreType] = ...,
-        TtlDuration: TtlDurationTypeDef = ...
+        TargetStores: Sequence[TargetStoreType] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used for data ingestion into the `FeatureStore`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.put_record)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/client/#put_record)
         """
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/literals.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,42 +2,36 @@
 Type annotations for sagemaker-featurestore-runtime service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_sagemaker_featurestore_runtime.literals import DeletionModeType
+    from mypy_boto3_sagemaker_featurestore_runtime.literals import TargetStoreType
 
-    data: DeletionModeType = "HardDelete"
+    data: TargetStoreType = "OfflineStore"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
-    "DeletionModeType",
-    "ExpirationTimeResponseType",
     "TargetStoreType",
-    "TtlDurationUnitType",
     "SageMakerFeatureStoreRuntimeServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
 
-DeletionModeType = Literal["HardDelete", "SoftDelete"]
-ExpirationTimeResponseType = Literal["Disabled", "Enabled"]
 TargetStoreType = Literal["OfflineStore", "OnlineStore"]
-TtlDurationUnitType = Literal["Days", "Hours", "Minutes", "Seconds", "Weeks"]
 SageMakerFeatureStoreRuntimeServiceName = Literal["sagemaker-featurestore-runtime"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -46,15 +40,14 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
-    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -75,34 +68,31 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
-    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -181,15 +171,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -200,38 +189,34 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -244,15 +229,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -271,19 +255,16 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
-    "payment-cryptography",
-    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -321,15 +302,14 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -363,21 +343,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
-    "verifiedpermissions",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/literals.pyi` & `mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,40 +2,34 @@
 Type annotations for sagemaker-featurestore-runtime service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_sagemaker_featurestore_runtime.literals import DeletionModeType
+    from mypy_boto3_sagemaker_featurestore_runtime.literals import TargetStoreType
 
-    data: DeletionModeType = "HardDelete"
+    data: TargetStoreType = "OfflineStore"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
-    "DeletionModeType",
-    "ExpirationTimeResponseType",
     "TargetStoreType",
-    "TtlDurationUnitType",
     "SageMakerFeatureStoreRuntimeServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
-DeletionModeType = Literal["HardDelete", "SoftDelete"]
-ExpirationTimeResponseType = Literal["Disabled", "Enabled"]
 TargetStoreType = Literal["OfflineStore", "OnlineStore"]
-TtlDurationUnitType = Literal["Days", "Hours", "Minutes", "Seconds", "Weeks"]
 SageMakerFeatureStoreRuntimeServiceName = Literal["sagemaker-featurestore-runtime"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -44,15 +38,14 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
-    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -73,34 +66,31 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
-    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -179,15 +169,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -198,38 +187,34 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -242,15 +227,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -269,19 +253,16 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
-    "payment-cryptography",
-    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -319,15 +300,14 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -361,21 +341,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
-    "verifiedpermissions",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime/type_defs.pyi` & `mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime/type_defs.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,34 +10,29 @@
 
     data: BatchGetRecordErrorTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
-from .literals import (
-    DeletionModeType,
-    ExpirationTimeResponseType,
-    TargetStoreType,
-    TtlDurationUnitType,
-)
+from .literals import TargetStoreType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BatchGetRecordErrorTypeDef",
     "BatchGetRecordIdentifierTypeDef",
     "ResponseMetadataTypeDef",
     "FeatureValueTypeDef",
     "DeleteRecordRequestRequestTypeDef",
     "GetRecordRequestRequestTypeDef",
-    "TtlDurationTypeDef",
     "BatchGetRecordRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "BatchGetRecordResultDetailTypeDef",
     "GetRecordResponseTypeDef",
     "PutRecordRequestRequestTypeDef",
     "BatchGetRecordResponseTypeDef",
 )
@@ -63,19 +58,21 @@
     "_OptionalBatchGetRecordIdentifierTypeDef",
     {
         "FeatureNames": Sequence[str],
     },
     total=False,
 )
 
+
 class BatchGetRecordIdentifierTypeDef(
     _RequiredBatchGetRecordIdentifierTypeDef, _OptionalBatchGetRecordIdentifierTypeDef
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -99,105 +96,74 @@
         "EventTime": str,
     },
 )
 _OptionalDeleteRecordRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteRecordRequestRequestTypeDef",
     {
         "TargetStores": Sequence[TargetStoreType],
-        "DeletionMode": DeletionModeType,
     },
     total=False,
 )
 
+
 class DeleteRecordRequestRequestTypeDef(
     _RequiredDeleteRecordRequestRequestTypeDef, _OptionalDeleteRecordRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetRecordRequestRequestTypeDef = TypedDict(
     "_RequiredGetRecordRequestRequestTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
     },
 )
 _OptionalGetRecordRequestRequestTypeDef = TypedDict(
     "_OptionalGetRecordRequestRequestTypeDef",
     {
         "FeatureNames": Sequence[str],
-        "ExpirationTimeResponse": ExpirationTimeResponseType,
     },
     total=False,
 )
 
+
 class GetRecordRequestRequestTypeDef(
     _RequiredGetRecordRequestRequestTypeDef, _OptionalGetRecordRequestRequestTypeDef
 ):
     pass
 
-TtlDurationTypeDef = TypedDict(
-    "TtlDurationTypeDef",
-    {
-        "Unit": TtlDurationUnitType,
-        "Value": int,
-    },
-)
 
-_RequiredBatchGetRecordRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGetRecordRequestRequestTypeDef",
+BatchGetRecordRequestRequestTypeDef = TypedDict(
+    "BatchGetRecordRequestRequestTypeDef",
     {
         "Identifiers": Sequence[BatchGetRecordIdentifierTypeDef],
     },
 )
-_OptionalBatchGetRecordRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGetRecordRequestRequestTypeDef",
-    {
-        "ExpirationTimeResponse": ExpirationTimeResponseType,
-    },
-    total=False,
-)
-
-class BatchGetRecordRequestRequestTypeDef(
-    _RequiredBatchGetRecordRequestRequestTypeDef, _OptionalBatchGetRecordRequestRequestTypeDef
-):
-    pass
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchGetRecordResultDetailTypeDef = TypedDict(
-    "_RequiredBatchGetRecordResultDetailTypeDef",
+BatchGetRecordResultDetailTypeDef = TypedDict(
+    "BatchGetRecordResultDetailTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
         "Record": List[FeatureValueTypeDef],
     },
 )
-_OptionalBatchGetRecordResultDetailTypeDef = TypedDict(
-    "_OptionalBatchGetRecordResultDetailTypeDef",
-    {
-        "ExpiresAt": str,
-    },
-    total=False,
-)
-
-class BatchGetRecordResultDetailTypeDef(
-    _RequiredBatchGetRecordResultDetailTypeDef, _OptionalBatchGetRecordResultDetailTypeDef
-):
-    pass
 
 GetRecordResponseTypeDef = TypedDict(
     "GetRecordResponseTypeDef",
     {
         "Record": List[FeatureValueTypeDef],
-        "ExpiresAt": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutRecordRequestRequestTypeDef = TypedDict(
     "_RequiredPutRecordRequestRequestTypeDef",
     {
@@ -205,24 +171,25 @@
         "Record": Sequence[FeatureValueTypeDef],
     },
 )
 _OptionalPutRecordRequestRequestTypeDef = TypedDict(
     "_OptionalPutRecordRequestRequestTypeDef",
     {
         "TargetStores": Sequence[TargetStoreType],
-        "TtlDuration": TtlDurationTypeDef,
     },
     total=False,
 )
 
+
 class PutRecordRequestRequestTypeDef(
     _RequiredPutRecordRequestRequestTypeDef, _OptionalPutRecordRequestRequestTypeDef
 ):
     pass
 
+
 BatchGetRecordResponseTypeDef = TypedDict(
     "BatchGetRecordResponseTypeDef",
     {
         "Records": List[BatchGetRecordResultDetailTypeDef],
         "Errors": List[BatchGetRecordErrorTypeDef],
         "UnprocessedIdentifiers": List[BatchGetRecordIdentifierTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-featurestore-runtime
-Version: 1.26.162
-Summary: Type annotations for boto3.SageMakerFeatureStoreRuntime 1.26.162 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.24
+Summary: Type annotations for boto3.SageMakerFeatureStoreRuntime 1.26.24 service generated with mypy-boto3-builder 7.11.11
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,44 +18,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-sagemaker-featurestore-runtime"></a>
 
 # mypy-boto3-sagemaker-featurestore-runtime
 
 [![PyPI - mypy-boto3-sagemaker-featurestore-runtime](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-featurestore-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-featurestore-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerFeatureStoreRuntime 1.26.162](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
+[boto3.SageMakerFeatureStoreRuntime 1.26.24](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sagemaker-featurestore-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -277,25 +276,22 @@
 ### Literals
 
 `mypy_boto3_sagemaker_featurestore_runtime.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_sagemaker_featurestore_runtime.literals import (
-    DeletionModeType,
-    ExpirationTimeResponseType,
     TargetStoreType,
-    TtlDurationUnitType,
     SageMakerFeatureStoreRuntimeServiceName,
     ServiceName,
     ResourceServiceName,
 )
 
 
-def check_value(value: DeletionModeType) -> bool:
+def check_value(value: TargetStoreType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
@@ -307,15 +303,14 @@
 from mypy_boto3_sagemaker_featurestore_runtime.type_defs import (
     BatchGetRecordErrorTypeDef,
     BatchGetRecordIdentifierTypeDef,
     ResponseMetadataTypeDef,
     FeatureValueTypeDef,
     DeleteRecordRequestRequestTypeDef,
     GetRecordRequestRequestTypeDef,
-    TtlDurationTypeDef,
     BatchGetRecordRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     BatchGetRecordResultDetailTypeDef,
     GetRecordResponseTypeDef,
     PutRecordRequestRequestTypeDef,
     BatchGetRecordResponseTypeDef,
 )
@@ -328,42 +323,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.26.162/mypy_boto3_sagemaker_featurestore_runtime.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-featurestore-runtime-1.26.24/mypy_boto3_sagemaker_featurestore_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.26.162/setup.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.26.24/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 """
 Setup script for mypy-boto3-sagemaker-featurestore-runtime.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-sagemaker-featurestore-runtime",
-    version="1.26.162",
+    version="1.26.24",
     packages=["mypy_boto3_sagemaker_featurestore_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SageMakerFeatureStoreRuntime 1.26.162 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SageMakerFeatureStoreRuntime 1.26.24 service generated with"
+        " mypy-boto3-builder 7.11.11"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords=(
         "boto3 sagemaker-featurestore-runtime type-annotations boto3-stubs mypy typeshed"
         " autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"mypy_boto3_sagemaker_featurestore_runtime": ["py.typed", "*.pyi"]},
+    package_data={
+        "": ["LICENSE"],
+        "mypy_boto3_sagemaker_featurestore_runtime": ["py.typed", "*.pyi"],
+    },
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

