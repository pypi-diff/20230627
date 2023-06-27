# Comparing `tmp/mypy-boto3-macie2-1.26.78.tar.gz` & `tmp/mypy-boto3-macie2-1.26.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-macie2-1.26.78.tar", last modified: Thu Feb 23 20:34:57 2023, max compression
+gzip compressed data, was "mypy-boto3-macie2-1.26.84.tar", last modified: Fri Mar  3 20:27:52 2023, max compression
```

## Comparing `mypy-boto3-macie2-1.26.78.tar` & `mypy-boto3-macie2-1.26.84.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.312421 mypy-boto3-macie2-1.26.78/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-23 20:34:39.000000 mypy-boto3-macie2-1.26.78/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28636 2023-02-23 20:34:57.312421 mypy-boto3-macie2-1.26.78/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27153 2023-02-23 20:34:39.000000 mypy-boto3-macie2-1.26.78/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.312421 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-02-23 20:34:39.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-02-23 20:34:39.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-02-23 20:34:39.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59831 2023-02-23 20:34:39.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    59728 2023-02-23 20:34:39.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17105 2023-02-23 20:34:40.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-02-23 20:34:40.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19513 2023-02-23 20:34:39.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19495 2023-02-23 20:34:39.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:39.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    88759 2023-02-23 20:34:42.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    88704 2023-02-23 20:34:41.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-23 20:34:39.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-02-23 20:34:39.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-02-23 20:34:39.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.312421 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28636 2023-02-23 20:34:57.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-02-23 20:34:57.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:57.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:57.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-23 20:34:57.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-23 20:34:57.000000 mypy-boto3-macie2-1.26.78/mypy_boto3_macie2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 20:34:57.312421 mypy-boto3-macie2-1.26.78/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-02-23 20:34:39.000000 mypy-boto3-macie2-1.26.78/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:27:52.670264 mypy-boto3-macie2-1.26.84/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-03 20:27:21.000000 mypy-boto3-macie2-1.26.84/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28636 2023-03-03 20:27:52.670264 mypy-boto3-macie2-1.26.84/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27153 2023-03-03 20:27:21.000000 mypy-boto3-macie2-1.26.84/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:27:52.666264 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-03-03 20:27:21.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-03-03 20:27:21.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-03 20:27:21.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59831 2023-03-03 20:27:21.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59728 2023-03-03 20:27:21.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17128 2023-03-03 20:27:23.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-03-03 20:27:22.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19513 2023-03-03 20:27:22.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19495 2023-03-03 20:27:22.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 20:27:21.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    88759 2023-03-03 20:27:24.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88704 2023-03-03 20:27:23.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-03 20:27:21.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-03 20:27:22.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-03-03 20:27:22.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:27:52.670264 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28636 2023-03-03 20:27:52.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-03 20:27:52.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 20:27:52.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 20:27:52.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-03 20:27:52.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-03 20:27:52.000000 mypy-boto3-macie2-1.26.84/mypy_boto3_macie2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 20:27:52.670264 mypy-boto3-macie2-1.26.84/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-03-03 20:27:21.000000 mypy-boto3-macie2-1.26.84/setup.py
```

### Comparing `mypy-boto3-macie2-1.26.78/LICENSE` & `mypy-boto3-macie2-1.26.84/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.26.78/PKG-INFO` & `mypy-boto3-macie2-1.26.84/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-macie2
-Version: 1.26.78
-Summary: Type annotations for boto3.Macie2 1.26.78 service generated with mypy-boto3-builder 7.12.4
+Version: 1.26.84
+Summary: Type annotations for boto3.Macie2 1.26.84 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie2.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie2)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-macie2?color=blue)](https://pypistats.org/packages/mypy-boto3-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie2 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
+[boto3.Macie2 1.26.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-macie2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-macie2-1.26.78/README.md` & `mypy-boto3-macie2-1.26.84/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie2.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie2)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-macie2?color=blue)](https://pypistats.org/packages/mypy-boto3-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie2 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
+[boto3.Macie2 1.26.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-macie2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/__init__.py` & `mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/__init__.pyi` & `mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/__main__.py` & `mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Macie2 1.26.78\nVersion:         1.26.78\nBuilder version:"
-        " 7.12.4\nDocs:           "
+        "Type annotations for boto3.Macie2 1.26.84\nVersion:         1.26.84\nBuilder version:"
+        " 7.12.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.78")
+    print("1.26.84")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/client.py` & `mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/client.pyi` & `mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/literals.py` & `mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,14 +389,15 @@
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

### Comparing `mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/literals.pyi` & `mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -387,14 +387,15 @@
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

### Comparing `mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/paginator.py` & `mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/paginator.pyi` & `mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/type_defs.py` & `mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/type_defs.pyi` & `mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/waiter.py` & `mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.26.78/mypy_boto3_macie2/waiter.pyi` & `mypy-boto3-macie2-1.26.84/mypy_boto3_macie2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.26.78/mypy_boto3_macie2.egg-info/PKG-INFO` & `mypy-boto3-macie2-1.26.84/mypy_boto3_macie2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-macie2
-Version: 1.26.78
-Summary: Type annotations for boto3.Macie2 1.26.78 service generated with mypy-boto3-builder 7.12.4
+Version: 1.26.84
+Summary: Type annotations for boto3.Macie2 1.26.84 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie2.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie2)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-macie2?color=blue)](https://pypistats.org/packages/mypy-boto3-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie2 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
+[boto3.Macie2 1.26.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-macie2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-macie2-1.26.78/mypy_boto3_macie2.egg-info/SOURCES.txt` & `mypy-boto3-macie2-1.26.84/mypy_boto3_macie2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.26.78/setup.py` & `mypy-boto3-macie2-1.26.84/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-macie2",
-    version="1.26.78",
+    version="1.26.84",
     packages=["mypy_boto3_macie2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Macie2 1.26.78 service generated with mypy-boto3-builder 7.12.4"
+        "Type annotations for boto3.Macie2 1.26.84 service generated with mypy-boto3-builder 7.12.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

