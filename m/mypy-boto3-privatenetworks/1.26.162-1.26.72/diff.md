# Comparing `tmp/mypy-boto3-privatenetworks-1.26.162.tar.gz` & `tmp/mypy-boto3-privatenetworks-1.26.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-privatenetworks-1.26.162.tar", last modified: Tue Jun 27 21:23:10 2023, max compression
+gzip compressed data, was "mypy-boto3-privatenetworks-1.26.72.tar", last modified: Wed Feb 15 22:27:56 2023, max compression
```

## Comparing `mypy-boto3-privatenetworks-1.26.162.tar` & `mypy-boto3-privatenetworks-1.26.72.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:23:10.490103 mypy-boto3-privatenetworks-1.26.162/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-27 21:22:17.000000 mypy-boto3-privatenetworks-1.26.162/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16786 2023-06-27 21:23:10.490103 mypy-boto3-privatenetworks-1.26.162/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-06-27 21:22:17.000000 mypy-boto3-privatenetworks-1.26.162/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:23:10.490103 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-27 21:22:17.000000 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-27 21:22:17.000000 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-27 21:22:18.000000 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21342 2023-06-27 21:22:18.000000 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-06-27 21:22:18.000000 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-06-27 21:22:18.000000 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-06-27 21:22:18.000000 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-06-27 21:22:18.000000 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-06-27 21:22:18.000000 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:22:18.000000 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28954 2023-06-27 21:22:19.000000 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28901 2023-06-27 21:22:18.000000 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-27 21:22:17.000000 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:23:10.490103 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16786 2023-06-27 21:23:10.000000 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-27 21:23:10.000000 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:23:10.000000 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:23:10.000000 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-27 21:23:10.000000 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-27 21:23:10.000000 mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 21:23:10.494103 mypy-boto3-privatenetworks-1.26.162/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-27 21:22:17.000000 mypy-boto3-privatenetworks-1.26.162/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.854127 mypy-boto3-privatenetworks-1.26.72/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-02-15 22:27:56.854127 mypy-boto3-privatenetworks-1.26.72/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15149 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.854127 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21049 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21011 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27299 2023-02-15 22:27:26.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27250 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.854127 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-02-15 22:27:56.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-02-15 22:27:56.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:27:56.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:27:56.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-15 22:27:56.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-15 22:27:56.000000 mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 22:27:56.854127 mypy-boto3-privatenetworks-1.26.72/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-02-15 22:27:25.000000 mypy-boto3-privatenetworks-1.26.72/setup.py
```

### Comparing `mypy-boto3-privatenetworks-1.26.162/LICENSE` & `mypy-boto3-privatenetworks-1.26.72/LICENSE`

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

### Comparing `mypy-boto3-privatenetworks-1.26.162/PKG-INFO` & `mypy-boto3-privatenetworks-1.26.72/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-privatenetworks
-Version: 1.26.162
-Summary: Type annotations for boto3.Private5G 1.26.162 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.72
+Summary: Type annotations for boto3.Private5G 1.26.72 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-privatenetworks"></a>
 
 # mypy-boto3-privatenetworks
 
 [![PyPI - mypy-boto3-privatenetworks](https://img.shields.io/pypi/v/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-privatenetworks?color=blue)](https://pypistats.org/packages/mypy-boto3-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Private5G 1.26.162](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[boto3.Private5G 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-privatenetworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,15 +312,14 @@
 
 `mypy_boto3_privatenetworks.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_privatenetworks.literals import (
     AcknowledgmentStatusType,
-    CommitmentLengthType,
     DeviceIdentifierFilterKeysType,
     DeviceIdentifierStatusType,
     ElevationReferenceType,
     ElevationUnitType,
     HealthStatusType,
     ListDeviceIdentifiersPaginatorName,
     ListNetworkResourcesPaginatorName,
@@ -358,15 +357,14 @@
 ```python
 from mypy_boto3_privatenetworks.type_defs import (
     AcknowledgeOrderReceiptRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ActivateDeviceIdentifierRequestRequestTypeDef,
     DeviceIdentifierTypeDef,
     AddressTypeDef,
-    CommitmentConfigurationTypeDef,
     PositionTypeDef,
     CreateNetworkRequestRequestTypeDef,
     NetworkTypeDef,
     DeactivateDeviceIdentifierRequestRequestTypeDef,
     DeleteNetworkRequestRequestTypeDef,
     DeleteNetworkSiteRequestRequestTypeDef,
     GetDeviceIdentifierRequestRequestTypeDef,
@@ -388,40 +386,38 @@
     UpdateNetworkSiteRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PingResponseTypeDef,
     ActivateDeviceIdentifierResponseTypeDef,
     DeactivateDeviceIdentifierResponseTypeDef,
     GetDeviceIdentifierResponseTypeDef,
     ListDeviceIdentifiersResponseTypeDef,
-    ReturnInformationTypeDef,
     ActivateNetworkSiteRequestRequestTypeDef,
-    CommitmentInformationTypeDef,
-    OrderedResourceDefinitionTypeDef,
+    ReturnInformationTypeDef,
     StartNetworkResourceUpdateRequestRequestTypeDef,
     ConfigureAccessPointRequestRequestTypeDef,
     CreateNetworkResponseTypeDef,
     DeleteNetworkResponseTypeDef,
     GetNetworkResponseTypeDef,
     ListNetworksResponseTypeDef,
     ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
     ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
     ListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
     ListNetworksRequestListNetworksPaginateTypeDef,
     ListOrdersRequestListOrdersPaginateTypeDef,
     NetworkResourceDefinitionTypeDef,
-    NetworkResourceTypeDef,
     OrderTypeDef,
+    NetworkResourceTypeDef,
     SitePlanTypeDef,
+    AcknowledgeOrderReceiptResponseTypeDef,
+    GetOrderResponseTypeDef,
+    ListOrdersResponseTypeDef,
     ConfigureAccessPointResponseTypeDef,
     GetNetworkResourceResponseTypeDef,
     ListNetworkResourcesResponseTypeDef,
     StartNetworkResourceUpdateResponseTypeDef,
-    AcknowledgeOrderReceiptResponseTypeDef,
-    GetOrderResponseTypeDef,
-    ListOrdersResponseTypeDef,
     CreateNetworkSiteRequestRequestTypeDef,
     NetworkSiteTypeDef,
     UpdateNetworkSitePlanRequestRequestTypeDef,
     ActivateNetworkSiteResponseTypeDef,
     CreateNetworkSiteResponseTypeDef,
     DeleteNetworkSiteResponseTypeDef,
     GetNetworkSiteResponseTypeDef,
@@ -437,42 +433,42 @@
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

### Comparing `mypy-boto3-privatenetworks-1.26.162/README.md` & `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-privatenetworks
+Version: 1.26.72
+Summary: Type annotations for boto3.Private5G 1.26.72 service generated with mypy-boto3-builder 7.12.3
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 privatenetworks type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-privatenetworks"></a>
 
 # mypy-boto3-privatenetworks
 
 [![PyPI - mypy-boto3-privatenetworks](https://img.shields.io/pypi/v/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-privatenetworks?color=blue)](https://pypistats.org/packages/mypy-boto3-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Private5G 1.26.162](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[boto3.Private5G 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-privatenetworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -280,15 +312,14 @@
 
 `mypy_boto3_privatenetworks.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_privatenetworks.literals import (
     AcknowledgmentStatusType,
-    CommitmentLengthType,
     DeviceIdentifierFilterKeysType,
     DeviceIdentifierStatusType,
     ElevationReferenceType,
     ElevationUnitType,
     HealthStatusType,
     ListDeviceIdentifiersPaginatorName,
     ListNetworkResourcesPaginatorName,
@@ -326,15 +357,14 @@
 ```python
 from mypy_boto3_privatenetworks.type_defs import (
     AcknowledgeOrderReceiptRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ActivateDeviceIdentifierRequestRequestTypeDef,
     DeviceIdentifierTypeDef,
     AddressTypeDef,
-    CommitmentConfigurationTypeDef,
     PositionTypeDef,
     CreateNetworkRequestRequestTypeDef,
     NetworkTypeDef,
     DeactivateDeviceIdentifierRequestRequestTypeDef,
     DeleteNetworkRequestRequestTypeDef,
     DeleteNetworkSiteRequestRequestTypeDef,
     GetDeviceIdentifierRequestRequestTypeDef,
@@ -356,40 +386,38 @@
     UpdateNetworkSiteRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PingResponseTypeDef,
     ActivateDeviceIdentifierResponseTypeDef,
     DeactivateDeviceIdentifierResponseTypeDef,
     GetDeviceIdentifierResponseTypeDef,
     ListDeviceIdentifiersResponseTypeDef,
-    ReturnInformationTypeDef,
     ActivateNetworkSiteRequestRequestTypeDef,
-    CommitmentInformationTypeDef,
-    OrderedResourceDefinitionTypeDef,
+    ReturnInformationTypeDef,
     StartNetworkResourceUpdateRequestRequestTypeDef,
     ConfigureAccessPointRequestRequestTypeDef,
     CreateNetworkResponseTypeDef,
     DeleteNetworkResponseTypeDef,
     GetNetworkResponseTypeDef,
     ListNetworksResponseTypeDef,
     ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
     ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
     ListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
     ListNetworksRequestListNetworksPaginateTypeDef,
     ListOrdersRequestListOrdersPaginateTypeDef,
     NetworkResourceDefinitionTypeDef,
-    NetworkResourceTypeDef,
     OrderTypeDef,
+    NetworkResourceTypeDef,
     SitePlanTypeDef,
+    AcknowledgeOrderReceiptResponseTypeDef,
+    GetOrderResponseTypeDef,
+    ListOrdersResponseTypeDef,
     ConfigureAccessPointResponseTypeDef,
     GetNetworkResourceResponseTypeDef,
     ListNetworkResourcesResponseTypeDef,
     StartNetworkResourceUpdateResponseTypeDef,
-    AcknowledgeOrderReceiptResponseTypeDef,
-    GetOrderResponseTypeDef,
-    ListOrdersResponseTypeDef,
     CreateNetworkSiteRequestRequestTypeDef,
     NetworkSiteTypeDef,
     UpdateNetworkSitePlanRequestRequestTypeDef,
     ActivateNetworkSiteResponseTypeDef,
     CreateNetworkSiteResponseTypeDef,
     DeleteNetworkSiteResponseTypeDef,
     GetNetworkSiteResponseTypeDef,
@@ -405,42 +433,42 @@
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

### Comparing `mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/__init__.py` & `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/__init__.pyi` & `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/__main__.py` & `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Private5G 1.26.162\nVersion:         1.26.162\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Private5G 1.26.72\nVersion:         1.26.72\nBuilder version:"
+        " 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.162")
+    print("1.26.72")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/client.py` & `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     ListOrdersPaginator,
 )
 from .type_defs import (
     AcknowledgeOrderReceiptResponseTypeDef,
     ActivateDeviceIdentifierResponseTypeDef,
     ActivateNetworkSiteResponseTypeDef,
     AddressTypeDef,
-    CommitmentConfigurationTypeDef,
     ConfigureAccessPointResponseTypeDef,
     CreateNetworkResponseTypeDef,
     CreateNetworkSiteResponseTypeDef,
     DeactivateDeviceIdentifierResponseTypeDef,
     DeleteNetworkResponseTypeDef,
     DeleteNetworkSiteResponseTypeDef,
     GetDeviceIdentifierResponseTypeDef,
@@ -120,20 +119,15 @@
         Activates the specified device identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.activate_device_identifier)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#activate_device_identifier)
         """
 
     def activate_network_site(
-        self,
-        *,
-        networkSiteArn: str,
-        shippingAddress: AddressTypeDef,
-        clientToken: str = ...,
-        commitmentConfiguration: CommitmentConfigurationTypeDef = ...
+        self, *, networkSiteArn: str, shippingAddress: AddressTypeDef, clientToken: str = ...
     ) -> ActivateNetworkSiteResponseTypeDef:
         """
         Activates the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.activate_network_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#activate_network_site)
         """
@@ -382,21 +376,19 @@
         """
 
     def start_network_resource_update(
         self,
         *,
         networkResourceArn: str,
         updateType: UpdateTypeType,
-        commitmentConfiguration: CommitmentConfigurationTypeDef = ...,
         returnReason: str = ...,
         shippingAddress: AddressTypeDef = ...
     ) -> StartNetworkResourceUpdateResponseTypeDef:
         """
-        Use this action to do the following tasks: * Update the duration and renewal
-        status of the commitment period for a radio unit.
+        Starts an update of the specified network resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.start_network_resource_update)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#start_network_resource_update)
         """
 
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
```

### Comparing `mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/client.pyi` & `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     ListOrdersPaginator,
 )
 from .type_defs import (
     AcknowledgeOrderReceiptResponseTypeDef,
     ActivateDeviceIdentifierResponseTypeDef,
     ActivateNetworkSiteResponseTypeDef,
     AddressTypeDef,
-    CommitmentConfigurationTypeDef,
     ConfigureAccessPointResponseTypeDef,
     CreateNetworkResponseTypeDef,
     CreateNetworkSiteResponseTypeDef,
     DeactivateDeviceIdentifierResponseTypeDef,
     DeleteNetworkResponseTypeDef,
     DeleteNetworkSiteResponseTypeDef,
     GetDeviceIdentifierResponseTypeDef,
@@ -113,20 +112,15 @@
         """
         Activates the specified device identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.activate_device_identifier)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#activate_device_identifier)
         """
     def activate_network_site(
-        self,
-        *,
-        networkSiteArn: str,
-        shippingAddress: AddressTypeDef,
-        clientToken: str = ...,
-        commitmentConfiguration: CommitmentConfigurationTypeDef = ...
+        self, *, networkSiteArn: str, shippingAddress: AddressTypeDef, clientToken: str = ...
     ) -> ActivateNetworkSiteResponseTypeDef:
         """
         Activates the specified network site.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.activate_network_site)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#activate_network_site)
         """
@@ -353,21 +347,19 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#ping)
         """
     def start_network_resource_update(
         self,
         *,
         networkResourceArn: str,
         updateType: UpdateTypeType,
-        commitmentConfiguration: CommitmentConfigurationTypeDef = ...,
         returnReason: str = ...,
         shippingAddress: AddressTypeDef = ...
     ) -> StartNetworkResourceUpdateResponseTypeDef:
         """
-        Use this action to do the following tasks: * Update the duration and renewal
-        status of the commitment period for a radio unit.
+        Starts an update of the specified network resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client.start_network_resource_update)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/client/#start_network_resource_update)
         """
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds tags to the specified resource.
```

### Comparing `mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/literals.py` & `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "AcknowledgmentStatusType",
-    "CommitmentLengthType",
     "DeviceIdentifierFilterKeysType",
     "DeviceIdentifierStatusType",
     "ElevationReferenceType",
     "ElevationUnitType",
     "HealthStatusType",
     "ListDeviceIdentifiersPaginatorName",
     "ListNetworkResourcesPaginatorName",
@@ -46,15 +45,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
 
 AcknowledgmentStatusType = Literal["ACKNOWLEDGED", "ACKNOWLEDGING", "UNACKNOWLEDGED"]
-CommitmentLengthType = Literal["ONE_YEAR", "SIXTY_DAYS", "THREE_YEARS"]
 DeviceIdentifierFilterKeysType = Literal["ORDER", "STATUS", "TRAFFIC_GROUP"]
 DeviceIdentifierStatusType = Literal["ACTIVE", "INACTIVE"]
 ElevationReferenceType = Literal["AGL", "AMSL"]
 ElevationUnitType = Literal["FEET"]
 HealthStatusType = Literal["HEALTHY", "INITIAL", "UNHEALTHY"]
 ListDeviceIdentifiersPaginatorName = Literal["list_device_identifiers"]
 ListNetworkResourcesPaginatorName = Literal["list_network_resources"]
@@ -76,15 +74,15 @@
     "SHIPPED",
 ]
 NetworkResourceTypeType = Literal["RADIO_UNIT"]
 NetworkSiteFilterKeysType = Literal["STATUS"]
 NetworkSiteStatusType = Literal["AVAILABLE", "CREATED", "DELETED", "DEPROVISIONING", "PROVISIONING"]
 NetworkStatusType = Literal["AVAILABLE", "CREATED", "DELETED", "DEPROVISIONING", "PROVISIONING"]
 OrderFilterKeysType = Literal["NETWORK_SITE", "STATUS"]
-UpdateTypeType = Literal["COMMITMENT", "REPLACE", "RETURN"]
+UpdateTypeType = Literal["REPLACE", "RETURN"]
 Private5GServiceName = Literal["privatenetworks"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -93,15 +91,14 @@
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
@@ -141,15 +138,14 @@
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
@@ -228,15 +224,14 @@
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
@@ -247,15 +242,14 @@
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
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -291,15 +285,14 @@
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
@@ -318,19 +311,16 @@
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
@@ -410,21 +400,18 @@
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

### Comparing `mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/literals.pyi` & `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AcknowledgmentStatusType",
-    "CommitmentLengthType",
     "DeviceIdentifierFilterKeysType",
     "DeviceIdentifierStatusType",
     "ElevationReferenceType",
     "ElevationUnitType",
     "HealthStatusType",
     "ListDeviceIdentifiersPaginatorName",
     "ListNetworkResourcesPaginatorName",
@@ -44,15 +43,14 @@
     "Private5GServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
 AcknowledgmentStatusType = Literal["ACKNOWLEDGED", "ACKNOWLEDGING", "UNACKNOWLEDGED"]
-CommitmentLengthType = Literal["ONE_YEAR", "SIXTY_DAYS", "THREE_YEARS"]
 DeviceIdentifierFilterKeysType = Literal["ORDER", "STATUS", "TRAFFIC_GROUP"]
 DeviceIdentifierStatusType = Literal["ACTIVE", "INACTIVE"]
 ElevationReferenceType = Literal["AGL", "AMSL"]
 ElevationUnitType = Literal["FEET"]
 HealthStatusType = Literal["HEALTHY", "INITIAL", "UNHEALTHY"]
 ListDeviceIdentifiersPaginatorName = Literal["list_device_identifiers"]
 ListNetworkResourcesPaginatorName = Literal["list_network_resources"]
@@ -74,15 +72,15 @@
     "SHIPPED",
 ]
 NetworkResourceTypeType = Literal["RADIO_UNIT"]
 NetworkSiteFilterKeysType = Literal["STATUS"]
 NetworkSiteStatusType = Literal["AVAILABLE", "CREATED", "DELETED", "DEPROVISIONING", "PROVISIONING"]
 NetworkStatusType = Literal["AVAILABLE", "CREATED", "DELETED", "DEPROVISIONING", "PROVISIONING"]
 OrderFilterKeysType = Literal["NETWORK_SITE", "STATUS"]
-UpdateTypeType = Literal["COMMITMENT", "REPLACE", "RETURN"]
+UpdateTypeType = Literal["REPLACE", "RETURN"]
 Private5GServiceName = Literal["privatenetworks"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -91,15 +89,14 @@
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
@@ -139,15 +136,14 @@
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
@@ -226,15 +222,14 @@
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
@@ -245,15 +240,14 @@
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
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -289,15 +283,14 @@
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
@@ -316,19 +309,16 @@
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
@@ -408,21 +398,18 @@
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

### Comparing `mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/paginator.py` & `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/paginator.pyi` & `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/type_defs.py` & `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AcknowledgmentStatusType,
-    CommitmentLengthType,
     DeviceIdentifierFilterKeysType,
     DeviceIdentifierStatusType,
     ElevationReferenceType,
     HealthStatusType,
     NetworkResourceDefinitionTypeType,
     NetworkResourceFilterKeysType,
     NetworkResourceStatusType,
@@ -43,15 +42,14 @@
 
 __all__ = (
     "AcknowledgeOrderReceiptRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ActivateDeviceIdentifierRequestRequestTypeDef",
     "DeviceIdentifierTypeDef",
     "AddressTypeDef",
-    "CommitmentConfigurationTypeDef",
     "PositionTypeDef",
     "CreateNetworkRequestRequestTypeDef",
     "NetworkTypeDef",
     "DeactivateDeviceIdentifierRequestRequestTypeDef",
     "DeleteNetworkRequestRequestTypeDef",
     "DeleteNetworkSiteRequestRequestTypeDef",
     "GetDeviceIdentifierRequestRequestTypeDef",
@@ -73,40 +71,38 @@
     "UpdateNetworkSiteRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PingResponseTypeDef",
     "ActivateDeviceIdentifierResponseTypeDef",
     "DeactivateDeviceIdentifierResponseTypeDef",
     "GetDeviceIdentifierResponseTypeDef",
     "ListDeviceIdentifiersResponseTypeDef",
-    "ReturnInformationTypeDef",
     "ActivateNetworkSiteRequestRequestTypeDef",
-    "CommitmentInformationTypeDef",
-    "OrderedResourceDefinitionTypeDef",
+    "ReturnInformationTypeDef",
     "StartNetworkResourceUpdateRequestRequestTypeDef",
     "ConfigureAccessPointRequestRequestTypeDef",
     "CreateNetworkResponseTypeDef",
     "DeleteNetworkResponseTypeDef",
     "GetNetworkResponseTypeDef",
     "ListNetworksResponseTypeDef",
     "ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
     "ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
     "ListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
     "ListNetworksRequestListNetworksPaginateTypeDef",
     "ListOrdersRequestListOrdersPaginateTypeDef",
     "NetworkResourceDefinitionTypeDef",
-    "NetworkResourceTypeDef",
     "OrderTypeDef",
+    "NetworkResourceTypeDef",
     "SitePlanTypeDef",
+    "AcknowledgeOrderReceiptResponseTypeDef",
+    "GetOrderResponseTypeDef",
+    "ListOrdersResponseTypeDef",
     "ConfigureAccessPointResponseTypeDef",
     "GetNetworkResourceResponseTypeDef",
     "ListNetworkResourcesResponseTypeDef",
     "StartNetworkResourceUpdateResponseTypeDef",
-    "AcknowledgeOrderReceiptResponseTypeDef",
-    "GetOrderResponseTypeDef",
-    "ListOrdersResponseTypeDef",
     "CreateNetworkSiteRequestRequestTypeDef",
     "NetworkSiteTypeDef",
     "UpdateNetworkSitePlanRequestRequestTypeDef",
     "ActivateNetworkSiteResponseTypeDef",
     "CreateNetworkSiteResponseTypeDef",
     "DeleteNetworkSiteResponseTypeDef",
     "GetNetworkSiteResponseTypeDef",
@@ -181,35 +177,26 @@
         "street1": str,
     },
 )
 _OptionalAddressTypeDef = TypedDict(
     "_OptionalAddressTypeDef",
     {
         "company": str,
-        "emailAddress": str,
         "phoneNumber": str,
         "street2": str,
         "street3": str,
     },
     total=False,
 )
 
 
 class AddressTypeDef(_RequiredAddressTypeDef, _OptionalAddressTypeDef):
     pass
 
 
-CommitmentConfigurationTypeDef = TypedDict(
-    "CommitmentConfigurationTypeDef",
-    {
-        "automaticRenewal": bool,
-        "commitmentLength": CommitmentLengthType,
-    },
-)
-
 PositionTypeDef = TypedDict(
     "PositionTypeDef",
     {
         "elevation": float,
         "elevationReference": ElevationReferenceType,
         "elevationUnit": Literal["FEET"],
         "latitude": float,
@@ -596,104 +583,58 @@
     {
         "deviceIdentifiers": List[DeviceIdentifierTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReturnInformationTypeDef = TypedDict(
-    "ReturnInformationTypeDef",
-    {
-        "replacementOrderArn": str,
-        "returnReason": str,
-        "shippingAddress": AddressTypeDef,
-        "shippingLabel": str,
-    },
-    total=False,
-)
-
 _RequiredActivateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_RequiredActivateNetworkSiteRequestRequestTypeDef",
     {
         "networkSiteArn": str,
         "shippingAddress": AddressTypeDef,
     },
 )
 _OptionalActivateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_OptionalActivateNetworkSiteRequestRequestTypeDef",
     {
         "clientToken": str,
-        "commitmentConfiguration": CommitmentConfigurationTypeDef,
     },
     total=False,
 )
 
 
 class ActivateNetworkSiteRequestRequestTypeDef(
     _RequiredActivateNetworkSiteRequestRequestTypeDef,
     _OptionalActivateNetworkSiteRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredCommitmentInformationTypeDef = TypedDict(
-    "_RequiredCommitmentInformationTypeDef",
-    {
-        "commitmentConfiguration": CommitmentConfigurationTypeDef,
-    },
-)
-_OptionalCommitmentInformationTypeDef = TypedDict(
-    "_OptionalCommitmentInformationTypeDef",
-    {
-        "expiresOn": datetime,
-        "startAt": datetime,
-    },
-    total=False,
-)
-
-
-class CommitmentInformationTypeDef(
-    _RequiredCommitmentInformationTypeDef, _OptionalCommitmentInformationTypeDef
-):
-    pass
-
-
-_RequiredOrderedResourceDefinitionTypeDef = TypedDict(
-    "_RequiredOrderedResourceDefinitionTypeDef",
-    {
-        "count": int,
-        "type": NetworkResourceDefinitionTypeType,
-    },
-)
-_OptionalOrderedResourceDefinitionTypeDef = TypedDict(
-    "_OptionalOrderedResourceDefinitionTypeDef",
+ReturnInformationTypeDef = TypedDict(
+    "ReturnInformationTypeDef",
     {
-        "commitmentConfiguration": CommitmentConfigurationTypeDef,
+        "replacementOrderArn": str,
+        "returnReason": str,
+        "shippingAddress": AddressTypeDef,
+        "shippingLabel": str,
     },
     total=False,
 )
 
-
-class OrderedResourceDefinitionTypeDef(
-    _RequiredOrderedResourceDefinitionTypeDef, _OptionalOrderedResourceDefinitionTypeDef
-):
-    pass
-
-
 _RequiredStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
     "_RequiredStartNetworkResourceUpdateRequestRequestTypeDef",
     {
         "networkResourceArn": str,
         "updateType": UpdateTypeType,
     },
 )
 _OptionalStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
     "_OptionalStartNetworkResourceUpdateRequestRequestTypeDef",
     {
-        "commitmentConfiguration": CommitmentConfigurationTypeDef,
         "returnReason": str,
         "shippingAddress": AddressTypeDef,
     },
     total=False,
 )
 
 
@@ -884,19 +825,32 @@
 
 class NetworkResourceDefinitionTypeDef(
     _RequiredNetworkResourceDefinitionTypeDef, _OptionalNetworkResourceDefinitionTypeDef
 ):
     pass
 
 
+OrderTypeDef = TypedDict(
+    "OrderTypeDef",
+    {
+        "acknowledgmentStatus": AcknowledgmentStatusType,
+        "createdAt": datetime,
+        "networkArn": str,
+        "networkSiteArn": str,
+        "orderArn": str,
+        "shippingAddress": AddressTypeDef,
+        "trackingInformation": List[TrackingInformationTypeDef],
+    },
+    total=False,
+)
+
 NetworkResourceTypeDef = TypedDict(
     "NetworkResourceTypeDef",
     {
         "attributes": List[NameValuePairTypeDef],
-        "commitmentInformation": CommitmentInformationTypeDef,
         "createdAt": datetime,
         "description": str,
         "health": HealthStatusType,
         "model": str,
         "networkArn": str,
         "networkResourceArn": str,
         "networkSiteArn": str,
@@ -908,94 +862,79 @@
         "statusReason": str,
         "type": Literal["RADIO_UNIT"],
         "vendor": str,
     },
     total=False,
 )
 
-OrderTypeDef = TypedDict(
-    "OrderTypeDef",
-    {
-        "acknowledgmentStatus": AcknowledgmentStatusType,
-        "createdAt": datetime,
-        "networkArn": str,
-        "networkSiteArn": str,
-        "orderArn": str,
-        "orderedResources": List[OrderedResourceDefinitionTypeDef],
-        "shippingAddress": AddressTypeDef,
-        "trackingInformation": List[TrackingInformationTypeDef],
-    },
-    total=False,
-)
-
 SitePlanTypeDef = TypedDict(
     "SitePlanTypeDef",
     {
         "options": List[NameValuePairTypeDef],
         "resourceDefinitions": List[NetworkResourceDefinitionTypeDef],
     },
     total=False,
 )
 
-ConfigureAccessPointResponseTypeDef = TypedDict(
-    "ConfigureAccessPointResponseTypeDef",
+AcknowledgeOrderReceiptResponseTypeDef = TypedDict(
+    "AcknowledgeOrderReceiptResponseTypeDef",
     {
-        "accessPoint": NetworkResourceTypeDef,
+        "order": OrderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetNetworkResourceResponseTypeDef = TypedDict(
-    "GetNetworkResourceResponseTypeDef",
+GetOrderResponseTypeDef = TypedDict(
+    "GetOrderResponseTypeDef",
     {
-        "networkResource": NetworkResourceTypeDef,
+        "order": OrderTypeDef,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListNetworkResourcesResponseTypeDef = TypedDict(
-    "ListNetworkResourcesResponseTypeDef",
+ListOrdersResponseTypeDef = TypedDict(
+    "ListOrdersResponseTypeDef",
     {
-        "networkResources": List[NetworkResourceTypeDef],
         "nextToken": str,
+        "orders": List[OrderTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartNetworkResourceUpdateResponseTypeDef = TypedDict(
-    "StartNetworkResourceUpdateResponseTypeDef",
+ConfigureAccessPointResponseTypeDef = TypedDict(
+    "ConfigureAccessPointResponseTypeDef",
     {
-        "networkResource": NetworkResourceTypeDef,
+        "accessPoint": NetworkResourceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AcknowledgeOrderReceiptResponseTypeDef = TypedDict(
-    "AcknowledgeOrderReceiptResponseTypeDef",
+GetNetworkResourceResponseTypeDef = TypedDict(
+    "GetNetworkResourceResponseTypeDef",
     {
-        "order": OrderTypeDef,
+        "networkResource": NetworkResourceTypeDef,
+        "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetOrderResponseTypeDef = TypedDict(
-    "GetOrderResponseTypeDef",
+ListNetworkResourcesResponseTypeDef = TypedDict(
+    "ListNetworkResourcesResponseTypeDef",
     {
-        "order": OrderTypeDef,
-        "tags": Dict[str, str],
+        "networkResources": List[NetworkResourceTypeDef],
+        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListOrdersResponseTypeDef = TypedDict(
-    "ListOrdersResponseTypeDef",
+StartNetworkResourceUpdateResponseTypeDef = TypedDict(
+    "StartNetworkResourceUpdateResponseTypeDef",
     {
-        "nextToken": str,
-        "orders": List[OrderTypeDef],
+        "networkResource": NetworkResourceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNetworkSiteRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks/type_defs.pyi` & `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AcknowledgmentStatusType,
-    CommitmentLengthType,
     DeviceIdentifierFilterKeysType,
     DeviceIdentifierStatusType,
     ElevationReferenceType,
     HealthStatusType,
     NetworkResourceDefinitionTypeType,
     NetworkResourceFilterKeysType,
     NetworkResourceStatusType,
@@ -42,15 +41,14 @@
 
 __all__ = (
     "AcknowledgeOrderReceiptRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ActivateDeviceIdentifierRequestRequestTypeDef",
     "DeviceIdentifierTypeDef",
     "AddressTypeDef",
-    "CommitmentConfigurationTypeDef",
     "PositionTypeDef",
     "CreateNetworkRequestRequestTypeDef",
     "NetworkTypeDef",
     "DeactivateDeviceIdentifierRequestRequestTypeDef",
     "DeleteNetworkRequestRequestTypeDef",
     "DeleteNetworkSiteRequestRequestTypeDef",
     "GetDeviceIdentifierRequestRequestTypeDef",
@@ -72,40 +70,38 @@
     "UpdateNetworkSiteRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PingResponseTypeDef",
     "ActivateDeviceIdentifierResponseTypeDef",
     "DeactivateDeviceIdentifierResponseTypeDef",
     "GetDeviceIdentifierResponseTypeDef",
     "ListDeviceIdentifiersResponseTypeDef",
-    "ReturnInformationTypeDef",
     "ActivateNetworkSiteRequestRequestTypeDef",
-    "CommitmentInformationTypeDef",
-    "OrderedResourceDefinitionTypeDef",
+    "ReturnInformationTypeDef",
     "StartNetworkResourceUpdateRequestRequestTypeDef",
     "ConfigureAccessPointRequestRequestTypeDef",
     "CreateNetworkResponseTypeDef",
     "DeleteNetworkResponseTypeDef",
     "GetNetworkResponseTypeDef",
     "ListNetworksResponseTypeDef",
     "ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
     "ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
     "ListNetworkSitesRequestListNetworkSitesPaginateTypeDef",
     "ListNetworksRequestListNetworksPaginateTypeDef",
     "ListOrdersRequestListOrdersPaginateTypeDef",
     "NetworkResourceDefinitionTypeDef",
-    "NetworkResourceTypeDef",
     "OrderTypeDef",
+    "NetworkResourceTypeDef",
     "SitePlanTypeDef",
+    "AcknowledgeOrderReceiptResponseTypeDef",
+    "GetOrderResponseTypeDef",
+    "ListOrdersResponseTypeDef",
     "ConfigureAccessPointResponseTypeDef",
     "GetNetworkResourceResponseTypeDef",
     "ListNetworkResourcesResponseTypeDef",
     "StartNetworkResourceUpdateResponseTypeDef",
-    "AcknowledgeOrderReceiptResponseTypeDef",
-    "GetOrderResponseTypeDef",
-    "ListOrdersResponseTypeDef",
     "CreateNetworkSiteRequestRequestTypeDef",
     "NetworkSiteTypeDef",
     "UpdateNetworkSitePlanRequestRequestTypeDef",
     "ActivateNetworkSiteResponseTypeDef",
     "CreateNetworkSiteResponseTypeDef",
     "DeleteNetworkSiteResponseTypeDef",
     "GetNetworkSiteResponseTypeDef",
@@ -178,33 +174,24 @@
         "street1": str,
     },
 )
 _OptionalAddressTypeDef = TypedDict(
     "_OptionalAddressTypeDef",
     {
         "company": str,
-        "emailAddress": str,
         "phoneNumber": str,
         "street2": str,
         "street3": str,
     },
     total=False,
 )
 
 class AddressTypeDef(_RequiredAddressTypeDef, _OptionalAddressTypeDef):
     pass
 
-CommitmentConfigurationTypeDef = TypedDict(
-    "CommitmentConfigurationTypeDef",
-    {
-        "automaticRenewal": bool,
-        "commitmentLength": CommitmentLengthType,
-    },
-)
-
 PositionTypeDef = TypedDict(
     "PositionTypeDef",
     {
         "elevation": float,
         "elevationReference": ElevationReferenceType,
         "elevationUnit": Literal["FEET"],
         "latitude": float,
@@ -569,98 +556,56 @@
     {
         "deviceIdentifiers": List[DeviceIdentifierTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReturnInformationTypeDef = TypedDict(
-    "ReturnInformationTypeDef",
-    {
-        "replacementOrderArn": str,
-        "returnReason": str,
-        "shippingAddress": AddressTypeDef,
-        "shippingLabel": str,
-    },
-    total=False,
-)
-
 _RequiredActivateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_RequiredActivateNetworkSiteRequestRequestTypeDef",
     {
         "networkSiteArn": str,
         "shippingAddress": AddressTypeDef,
     },
 )
 _OptionalActivateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_OptionalActivateNetworkSiteRequestRequestTypeDef",
     {
         "clientToken": str,
-        "commitmentConfiguration": CommitmentConfigurationTypeDef,
     },
     total=False,
 )
 
 class ActivateNetworkSiteRequestRequestTypeDef(
     _RequiredActivateNetworkSiteRequestRequestTypeDef,
     _OptionalActivateNetworkSiteRequestRequestTypeDef,
 ):
     pass
 
-_RequiredCommitmentInformationTypeDef = TypedDict(
-    "_RequiredCommitmentInformationTypeDef",
-    {
-        "commitmentConfiguration": CommitmentConfigurationTypeDef,
-    },
-)
-_OptionalCommitmentInformationTypeDef = TypedDict(
-    "_OptionalCommitmentInformationTypeDef",
-    {
-        "expiresOn": datetime,
-        "startAt": datetime,
-    },
-    total=False,
-)
-
-class CommitmentInformationTypeDef(
-    _RequiredCommitmentInformationTypeDef, _OptionalCommitmentInformationTypeDef
-):
-    pass
-
-_RequiredOrderedResourceDefinitionTypeDef = TypedDict(
-    "_RequiredOrderedResourceDefinitionTypeDef",
-    {
-        "count": int,
-        "type": NetworkResourceDefinitionTypeType,
-    },
-)
-_OptionalOrderedResourceDefinitionTypeDef = TypedDict(
-    "_OptionalOrderedResourceDefinitionTypeDef",
+ReturnInformationTypeDef = TypedDict(
+    "ReturnInformationTypeDef",
     {
-        "commitmentConfiguration": CommitmentConfigurationTypeDef,
+        "replacementOrderArn": str,
+        "returnReason": str,
+        "shippingAddress": AddressTypeDef,
+        "shippingLabel": str,
     },
     total=False,
 )
 
-class OrderedResourceDefinitionTypeDef(
-    _RequiredOrderedResourceDefinitionTypeDef, _OptionalOrderedResourceDefinitionTypeDef
-):
-    pass
-
 _RequiredStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
     "_RequiredStartNetworkResourceUpdateRequestRequestTypeDef",
     {
         "networkResourceArn": str,
         "updateType": UpdateTypeType,
     },
 )
 _OptionalStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
     "_OptionalStartNetworkResourceUpdateRequestRequestTypeDef",
     {
-        "commitmentConfiguration": CommitmentConfigurationTypeDef,
         "returnReason": str,
         "shippingAddress": AddressTypeDef,
     },
     total=False,
 )
 
 class StartNetworkResourceUpdateRequestRequestTypeDef(
@@ -837,19 +782,32 @@
 )
 
 class NetworkResourceDefinitionTypeDef(
     _RequiredNetworkResourceDefinitionTypeDef, _OptionalNetworkResourceDefinitionTypeDef
 ):
     pass
 
+OrderTypeDef = TypedDict(
+    "OrderTypeDef",
+    {
+        "acknowledgmentStatus": AcknowledgmentStatusType,
+        "createdAt": datetime,
+        "networkArn": str,
+        "networkSiteArn": str,
+        "orderArn": str,
+        "shippingAddress": AddressTypeDef,
+        "trackingInformation": List[TrackingInformationTypeDef],
+    },
+    total=False,
+)
+
 NetworkResourceTypeDef = TypedDict(
     "NetworkResourceTypeDef",
     {
         "attributes": List[NameValuePairTypeDef],
-        "commitmentInformation": CommitmentInformationTypeDef,
         "createdAt": datetime,
         "description": str,
         "health": HealthStatusType,
         "model": str,
         "networkArn": str,
         "networkResourceArn": str,
         "networkSiteArn": str,
@@ -861,94 +819,79 @@
         "statusReason": str,
         "type": Literal["RADIO_UNIT"],
         "vendor": str,
     },
     total=False,
 )
 
-OrderTypeDef = TypedDict(
-    "OrderTypeDef",
-    {
-        "acknowledgmentStatus": AcknowledgmentStatusType,
-        "createdAt": datetime,
-        "networkArn": str,
-        "networkSiteArn": str,
-        "orderArn": str,
-        "orderedResources": List[OrderedResourceDefinitionTypeDef],
-        "shippingAddress": AddressTypeDef,
-        "trackingInformation": List[TrackingInformationTypeDef],
-    },
-    total=False,
-)
-
 SitePlanTypeDef = TypedDict(
     "SitePlanTypeDef",
     {
         "options": List[NameValuePairTypeDef],
         "resourceDefinitions": List[NetworkResourceDefinitionTypeDef],
     },
     total=False,
 )
 
-ConfigureAccessPointResponseTypeDef = TypedDict(
-    "ConfigureAccessPointResponseTypeDef",
+AcknowledgeOrderReceiptResponseTypeDef = TypedDict(
+    "AcknowledgeOrderReceiptResponseTypeDef",
     {
-        "accessPoint": NetworkResourceTypeDef,
+        "order": OrderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetNetworkResourceResponseTypeDef = TypedDict(
-    "GetNetworkResourceResponseTypeDef",
+GetOrderResponseTypeDef = TypedDict(
+    "GetOrderResponseTypeDef",
     {
-        "networkResource": NetworkResourceTypeDef,
+        "order": OrderTypeDef,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListNetworkResourcesResponseTypeDef = TypedDict(
-    "ListNetworkResourcesResponseTypeDef",
+ListOrdersResponseTypeDef = TypedDict(
+    "ListOrdersResponseTypeDef",
     {
-        "networkResources": List[NetworkResourceTypeDef],
         "nextToken": str,
+        "orders": List[OrderTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartNetworkResourceUpdateResponseTypeDef = TypedDict(
-    "StartNetworkResourceUpdateResponseTypeDef",
+ConfigureAccessPointResponseTypeDef = TypedDict(
+    "ConfigureAccessPointResponseTypeDef",
     {
-        "networkResource": NetworkResourceTypeDef,
+        "accessPoint": NetworkResourceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AcknowledgeOrderReceiptResponseTypeDef = TypedDict(
-    "AcknowledgeOrderReceiptResponseTypeDef",
+GetNetworkResourceResponseTypeDef = TypedDict(
+    "GetNetworkResourceResponseTypeDef",
     {
-        "order": OrderTypeDef,
+        "networkResource": NetworkResourceTypeDef,
+        "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetOrderResponseTypeDef = TypedDict(
-    "GetOrderResponseTypeDef",
+ListNetworkResourcesResponseTypeDef = TypedDict(
+    "ListNetworkResourcesResponseTypeDef",
     {
-        "order": OrderTypeDef,
-        "tags": Dict[str, str],
+        "networkResources": List[NetworkResourceTypeDef],
+        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListOrdersResponseTypeDef = TypedDict(
-    "ListOrdersResponseTypeDef",
+StartNetworkResourceUpdateResponseTypeDef = TypedDict(
+    "StartNetworkResourceUpdateResponseTypeDef",
     {
-        "nextToken": str,
-        "orders": List[OrderTypeDef],
+        "networkResource": NetworkResourceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNetworkSiteRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks.egg-info/PKG-INFO` & `mypy-boto3-privatenetworks-1.26.72/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-privatenetworks
-Version: 1.26.162
-Summary: Type annotations for boto3.Private5G 1.26.162 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 privatenetworks type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-privatenetworks"></a>
 
 # mypy-boto3-privatenetworks
 
 [![PyPI - mypy-boto3-privatenetworks](https://img.shields.io/pypi/v/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-privatenetworks?color=blue)](https://pypistats.org/packages/mypy-boto3-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Private5G 1.26.162](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[boto3.Private5G 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-privatenetworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,15 +280,14 @@
 
 `mypy_boto3_privatenetworks.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_privatenetworks.literals import (
     AcknowledgmentStatusType,
-    CommitmentLengthType,
     DeviceIdentifierFilterKeysType,
     DeviceIdentifierStatusType,
     ElevationReferenceType,
     ElevationUnitType,
     HealthStatusType,
     ListDeviceIdentifiersPaginatorName,
     ListNetworkResourcesPaginatorName,
@@ -358,15 +325,14 @@
 ```python
 from mypy_boto3_privatenetworks.type_defs import (
     AcknowledgeOrderReceiptRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ActivateDeviceIdentifierRequestRequestTypeDef,
     DeviceIdentifierTypeDef,
     AddressTypeDef,
-    CommitmentConfigurationTypeDef,
     PositionTypeDef,
     CreateNetworkRequestRequestTypeDef,
     NetworkTypeDef,
     DeactivateDeviceIdentifierRequestRequestTypeDef,
     DeleteNetworkRequestRequestTypeDef,
     DeleteNetworkSiteRequestRequestTypeDef,
     GetDeviceIdentifierRequestRequestTypeDef,
@@ -388,40 +354,38 @@
     UpdateNetworkSiteRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PingResponseTypeDef,
     ActivateDeviceIdentifierResponseTypeDef,
     DeactivateDeviceIdentifierResponseTypeDef,
     GetDeviceIdentifierResponseTypeDef,
     ListDeviceIdentifiersResponseTypeDef,
-    ReturnInformationTypeDef,
     ActivateNetworkSiteRequestRequestTypeDef,
-    CommitmentInformationTypeDef,
-    OrderedResourceDefinitionTypeDef,
+    ReturnInformationTypeDef,
     StartNetworkResourceUpdateRequestRequestTypeDef,
     ConfigureAccessPointRequestRequestTypeDef,
     CreateNetworkResponseTypeDef,
     DeleteNetworkResponseTypeDef,
     GetNetworkResponseTypeDef,
     ListNetworksResponseTypeDef,
     ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
     ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
     ListNetworkSitesRequestListNetworkSitesPaginateTypeDef,
     ListNetworksRequestListNetworksPaginateTypeDef,
     ListOrdersRequestListOrdersPaginateTypeDef,
     NetworkResourceDefinitionTypeDef,
-    NetworkResourceTypeDef,
     OrderTypeDef,
+    NetworkResourceTypeDef,
     SitePlanTypeDef,
+    AcknowledgeOrderReceiptResponseTypeDef,
+    GetOrderResponseTypeDef,
+    ListOrdersResponseTypeDef,
     ConfigureAccessPointResponseTypeDef,
     GetNetworkResourceResponseTypeDef,
     ListNetworkResourcesResponseTypeDef,
     StartNetworkResourceUpdateResponseTypeDef,
-    AcknowledgeOrderReceiptResponseTypeDef,
-    GetOrderResponseTypeDef,
-    ListOrdersResponseTypeDef,
     CreateNetworkSiteRequestRequestTypeDef,
     NetworkSiteTypeDef,
     UpdateNetworkSitePlanRequestRequestTypeDef,
     ActivateNetworkSiteResponseTypeDef,
     CreateNetworkSiteResponseTypeDef,
     DeleteNetworkSiteResponseTypeDef,
     GetNetworkSiteResponseTypeDef,
@@ -437,42 +401,42 @@
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

### Comparing `mypy-boto3-privatenetworks-1.26.162/mypy_boto3_privatenetworks.egg-info/SOURCES.txt` & `mypy-boto3-privatenetworks-1.26.72/mypy_boto3_privatenetworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.26.162/setup.py` & `mypy-boto3-privatenetworks-1.26.72/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-privatenetworks.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-privatenetworks",
-    version="1.26.162",
+    version="1.26.72",
     packages=["mypy_boto3_privatenetworks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Private5G 1.26.162 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Private5G 1.26.72 service generated with mypy-boto3-builder"
+        " 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/",
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

