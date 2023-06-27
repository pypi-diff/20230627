# Comparing `tmp/mypy-boto3-ssm-1.26.77.tar.gz` & `tmp/mypy-boto3-ssm-1.26.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-1.26.77.tar", last modified: Wed Feb 22 20:34:22 2023, max compression
+gzip compressed data, was "mypy-boto3-ssm-1.26.97.tar", last modified: Wed Mar 22 19:32:31 2023, max compression
```

## Comparing `mypy-boto3-ssm-1.26.77.tar` & `mypy-boto3-ssm-1.26.97.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.530112 mypy-boto3-ssm-1.26.77/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-22 20:34:05.000000 mypy-boto3-ssm-1.26.77/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46048 2023-02-22 20:34:22.530112 mypy-boto3-ssm-1.26.77/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    44577 2023-02-22 20:34:05.000000 mypy-boto3-ssm-1.26.77/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.530112 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/
--rw-r--r--   0 runner    (1001) docker     (123)    12702 2023-02-22 20:34:05.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-02-22 20:34:05.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-02-22 20:34:05.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   131290 2023-02-22 20:34:06.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   131097 2023-02-22 20:34:06.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27825 2023-02-22 20:34:07.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-02-22 20:34:07.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    59186 2023-02-22 20:34:07.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    59137 2023-02-22 20:34:07.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:05.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   204155 2023-02-22 20:34:12.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   203927 2023-02-22 20:34:10.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-22 20:34:05.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-02-22 20:34:07.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-02-22 20:34:07.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.530112 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46048 2023-02-22 20:34:22.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-02-22 20:34:22.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 20:34:22.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 20:34:22.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-22 20:34:22.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-22 20:34:22.000000 mypy-boto3-ssm-1.26.77/mypy_boto3_ssm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 20:34:22.530112 mypy-boto3-ssm-1.26.77/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-02-22 20:34:05.000000 mypy-boto3-ssm-1.26.77/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.357775 mypy-boto3-ssm-1.26.97/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-22 19:32:15.000000 mypy-boto3-ssm-1.26.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    46048 2023-03-22 19:32:31.349775 mypy-boto3-ssm-1.26.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    44577 2023-03-22 19:32:15.000000 mypy-boto3-ssm-1.26.97/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.345775 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)    12702 2023-03-22 19:32:15.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-03-22 19:32:15.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-22 19:32:15.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131290 2023-03-22 19:32:16.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131097 2023-03-22 19:32:15.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27891 2023-03-22 19:32:17.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-03-22 19:32:17.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    59186 2023-03-22 19:32:17.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59137 2023-03-22 19:32:16.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:15.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   204155 2023-03-22 19:32:22.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   203927 2023-03-22 19:32:19.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-22 19:32:15.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-03-22 19:32:17.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-22 19:32:17.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.349775 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46048 2023-03-22 19:32:31.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-22 19:32:31.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 19:32:31.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 19:32:31.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-22 19:32:31.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-22 19:32:31.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 19:32:31.357775 mypy-boto3-ssm-1.26.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-03-22 19:32:15.000000 mypy-boto3-ssm-1.26.97/setup.py
```

### Comparing `mypy-boto3-ssm-1.26.77/LICENSE` & `mypy-boto3-ssm-1.26.97/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.26.77/PKG-INFO` & `mypy-boto3-ssm-1.26.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm
-Version: 1.26.77
-Summary: Type annotations for boto3.SSM 1.26.77 service generated with mypy-boto3-builder 7.12.4
+Version: 1.26.97
+Summary: Type annotations for boto3.SSM 1.26.97 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSM 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[boto3.SSM 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ssm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ssm-1.26.77/README.md` & `mypy-boto3-ssm-1.26.97/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSM 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[boto3.SSM 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ssm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/__init__.py` & `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/__init__.pyi` & `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/__main__.py` & `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSM 1.26.77\nVersion:         1.26.77\nBuilder version:"
-        " 7.12.4\nDocs:           "
+        "Type annotations for boto3.SSM 1.26.97\nVersion:         1.26.97\nBuilder version:"
+        " 7.13.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.77")
+    print("1.26.97")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/client.py` & `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/client.pyi` & `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/literals.py` & `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,17 +358,19 @@
 ]
 MaintenanceWindowResourceTypeType = Literal["INSTANCE", "RESOURCE_GROUP"]
 MaintenanceWindowTaskCutoffBehaviorType = Literal["CANCEL_TASK", "CONTINUE_TASK"]
 MaintenanceWindowTaskTypeType = Literal["AUTOMATION", "LAMBDA", "RUN_COMMAND", "STEP_FUNCTIONS"]
 NotificationEventType = Literal["All", "Cancelled", "Failed", "InProgress", "Success", "TimedOut"]
 NotificationTypeType = Literal["Command", "Invocation"]
 OperatingSystemType = Literal[
+    "ALMA_LINUX",
     "AMAZON_LINUX",
     "AMAZON_LINUX_2",
     "AMAZON_LINUX_2022",
+    "AMAZON_LINUX_2023",
     "CENTOS",
     "DEBIAN",
     "MACOS",
     "ORACLE_LINUX",
     "RASPBIAN",
     "REDHAT_ENTERPRISE_LINUX",
     "ROCKY_LINUX",
@@ -661,14 +663,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
```

### Comparing `mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/literals.pyi` & `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -356,17 +356,19 @@
 ]
 MaintenanceWindowResourceTypeType = Literal["INSTANCE", "RESOURCE_GROUP"]
 MaintenanceWindowTaskCutoffBehaviorType = Literal["CANCEL_TASK", "CONTINUE_TASK"]
 MaintenanceWindowTaskTypeType = Literal["AUTOMATION", "LAMBDA", "RUN_COMMAND", "STEP_FUNCTIONS"]
 NotificationEventType = Literal["All", "Cancelled", "Failed", "InProgress", "Success", "TimedOut"]
 NotificationTypeType = Literal["Command", "Invocation"]
 OperatingSystemType = Literal[
+    "ALMA_LINUX",
     "AMAZON_LINUX",
     "AMAZON_LINUX_2",
     "AMAZON_LINUX_2022",
+    "AMAZON_LINUX_2023",
     "CENTOS",
     "DEBIAN",
     "MACOS",
     "ORACLE_LINUX",
     "RASPBIAN",
     "REDHAT_ENTERPRISE_LINUX",
     "ROCKY_LINUX",
@@ -659,14 +661,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
```

### Comparing `mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/paginator.py` & `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/paginator.pyi` & `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/type_defs.py` & `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/type_defs.pyi` & `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/waiter.py` & `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.26.77/mypy_boto3_ssm/waiter.pyi` & `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.26.77/mypy_boto3_ssm.egg-info/PKG-INFO` & `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm
-Version: 1.26.77
-Summary: Type annotations for boto3.SSM 1.26.77 service generated with mypy-boto3-builder 7.12.4
+Version: 1.26.97
+Summary: Type annotations for boto3.SSM 1.26.97 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSM 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[boto3.SSM 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ssm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ssm-1.26.77/mypy_boto3_ssm.egg-info/SOURCES.txt` & `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.26.77/setup.py` & `mypy-boto3-ssm-1.26.97/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-ssm",
-    version="1.26.77",
+    version="1.26.97",
     packages=["mypy_boto3_ssm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSM 1.26.77 service generated with mypy-boto3-builder 7.12.4"
+        "Type annotations for boto3.SSM 1.26.97 service generated with mypy-boto3-builder 7.13.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

