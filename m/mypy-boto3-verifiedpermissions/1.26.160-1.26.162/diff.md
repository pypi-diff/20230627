# Comparing `tmp/mypy-boto3-verifiedpermissions-1.26.160.tar.gz` & `tmp/mypy-boto3-verifiedpermissions-1.26.162.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-verifiedpermissions-1.26.160.tar", last modified: Fri Jun 23 19:32:44 2023, max compression
+gzip compressed data, was "mypy-boto3-verifiedpermissions-1.26.162.tar", last modified: Tue Jun 27 21:23:12 2023, max compression
```

## Comparing `mypy-boto3-verifiedpermissions-1.26.160.tar` & `mypy-boto3-verifiedpermissions-1.26.162.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:32:44.307970 mypy-boto3-verifiedpermissions-1.26.160/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-23 19:32:33.000000 mypy-boto3-verifiedpermissions-1.26.160/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16877 2023-06-23 19:32:44.307970 mypy-boto3-verifiedpermissions-1.26.160/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15340 2023-06-23 19:32:33.000000 mypy-boto3-verifiedpermissions-1.26.160/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:32:44.307970 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-23 19:32:33.000000 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-23 19:32:33.000000 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-23 19:32:33.000000 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21090 2023-06-23 19:32:33.000000 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21055 2023-06-23 19:32:33.000000 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-06-23 19:32:34.000000 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8922 2023-06-23 19:32:34.000000 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-06-23 19:32:33.000000 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-23 19:32:33.000000 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 19:32:33.000000 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31198 2023-06-23 19:32:35.000000 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31147 2023-06-23 19:32:34.000000 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-23 19:32:33.000000 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:32:44.307970 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16877 2023-06-23 19:32:44.000000 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-23 19:32:44.000000 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:32:44.000000 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:32:44.000000 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 19:32:44.000000 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 19:32:44.000000 mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 19:32:44.307970 mypy-boto3-verifiedpermissions-1.26.160/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-23 19:32:33.000000 mypy-boto3-verifiedpermissions-1.26.160/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:23:12.978128 mypy-boto3-verifiedpermissions-1.26.162/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-27 21:22:57.000000 mypy-boto3-verifiedpermissions-1.26.162/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16877 2023-06-27 21:23:12.978128 mypy-boto3-verifiedpermissions-1.26.162/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15340 2023-06-27 21:22:57.000000 mypy-boto3-verifiedpermissions-1.26.162/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:23:12.978128 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-27 21:22:57.000000 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-27 21:22:57.000000 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-27 21:22:57.000000 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21090 2023-06-27 21:22:57.000000 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21055 2023-06-27 21:22:57.000000 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-06-27 21:22:57.000000 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-27 21:22:57.000000 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-06-27 21:22:57.000000 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-27 21:22:57.000000 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:22:57.000000 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31198 2023-06-27 21:22:58.000000 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31147 2023-06-27 21:22:58.000000 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-27 21:22:57.000000 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:23:12.978128 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16877 2023-06-27 21:23:12.000000 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-27 21:23:12.000000 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:23:12.000000 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:23:12.000000 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-27 21:23:12.000000 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-27 21:23:12.000000 mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 21:23:12.982128 mypy-boto3-verifiedpermissions-1.26.162/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-27 21:22:57.000000 mypy-boto3-verifiedpermissions-1.26.162/setup.py
```

### Comparing `mypy-boto3-verifiedpermissions-1.26.160/LICENSE` & `mypy-boto3-verifiedpermissions-1.26.162/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.26.160/PKG-INFO` & `mypy-boto3-verifiedpermissions-1.26.162/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-verifiedpermissions
-Version: 1.26.160
-Summary: Type annotations for boto3.VerifiedPermissions 1.26.160 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.162
+Summary: Type annotations for boto3.VerifiedPermissions 1.26.162 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-verifiedpermissions?color=blue)](https://pypistats.org/packages/mypy-boto3-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VerifiedPermissions 1.26.160](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[boto3.VerifiedPermissions 1.26.162](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-verifiedpermissions-1.26.160/README.md` & `mypy-boto3-verifiedpermissions-1.26.162/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-verifiedpermissions?color=blue)](https://pypistats.org/packages/mypy-boto3-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VerifiedPermissions 1.26.160](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[boto3.VerifiedPermissions 1.26.162](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/__init__.py` & `mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/__init__.pyi` & `mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/__main__.py` & `mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.VerifiedPermissions 1.26.160\nVersion:        "
-        " 1.26.160\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.VerifiedPermissions 1.26.162\nVersion:        "
+        " 1.26.162\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.160")
+    print("1.26.162")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/client.py` & `mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/client.pyi` & `mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/literals.py` & `mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DecisionType",
     "ListIdentitySourcesPaginatorName",
     "ListPoliciesPaginatorName",
     "ListPolicyStoresPaginatorName",
     "ListPolicyTemplatesPaginatorName",
     "OpenIdIssuerType",
@@ -31,15 +30,14 @@
     "VerifiedPermissionsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DecisionType = Literal["ALLOW", "DENY"]
 ListIdentitySourcesPaginatorName = Literal["list_identity_sources"]
 ListPoliciesPaginatorName = Literal["list_policies"]
 ListPolicyStoresPaginatorName = Literal["list_policy_stores"]
 ListPolicyTemplatesPaginatorName = Literal["list_policy_templates"]
 OpenIdIssuerType = Literal["COGNITO"]
 PolicyTypeType = Literal["STATIC", "TEMPLATE_LINKED"]
@@ -56,14 +54,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
```

### Comparing `mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/literals.pyi` & `mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DecisionType",
     "ListIdentitySourcesPaginatorName",
     "ListPoliciesPaginatorName",
     "ListPolicyStoresPaginatorName",
     "ListPolicyTemplatesPaginatorName",
     "OpenIdIssuerType",
@@ -30,14 +31,15 @@
     "VerifiedPermissionsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DecisionType = Literal["ALLOW", "DENY"]
 ListIdentitySourcesPaginatorName = Literal["list_identity_sources"]
 ListPoliciesPaginatorName = Literal["list_policies"]
 ListPolicyStoresPaginatorName = Literal["list_policy_stores"]
 ListPolicyTemplatesPaginatorName = Literal["list_policy_templates"]
 OpenIdIssuerType = Literal["COGNITO"]
 PolicyTypeType = Literal["STATIC", "TEMPLATE_LINKED"]
@@ -54,14 +56,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
```

### Comparing `mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/paginator.py` & `mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/paginator.pyi` & `mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/type_defs.py` & `mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions/type_defs.pyi` & `mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO` & `mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-verifiedpermissions
-Version: 1.26.160
-Summary: Type annotations for boto3.VerifiedPermissions 1.26.160 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.162
+Summary: Type annotations for boto3.VerifiedPermissions 1.26.162 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-verifiedpermissions?color=blue)](https://pypistats.org/packages/mypy-boto3-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VerifiedPermissions 1.26.160](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[boto3.VerifiedPermissions 1.26.162](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-verifiedpermissions-1.26.160/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt` & `mypy-boto3-verifiedpermissions-1.26.162/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.26.160/setup.py` & `mypy-boto3-verifiedpermissions-1.26.162/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-verifiedpermissions",
-    version="1.26.160",
+    version="1.26.162",
     packages=["mypy_boto3_verifiedpermissions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.VerifiedPermissions 1.26.160 service generated with"
+        "Type annotations for boto3.VerifiedPermissions 1.26.162 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

