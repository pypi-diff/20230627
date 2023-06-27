# Comparing `tmp/rubrical-0.2.1.tar.gz` & `tmp/rubrical-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubrical-0.2.1.tar", max compression
+gzip compressed data, was "rubrical-0.2.2.tar", max compression
```

## Comparing `rubrical-0.2.1.tar` & `rubrical-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    15976 2023-04-24 08:57:50.944846 rubrical-0.2.1/LICENSE
--rw-r--r--   0        0        0     2782 2023-04-24 08:57:50.944846 rubrical-0.2.1/README.md
--rw-r--r--   0        0        0     1865 2023-04-24 08:58:13.497104 rubrical-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/__init__.py
--rw-r--r--   0        0        0      784 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/comparisons/__init__.py
--rw-r--r--   0        0        0     2255 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/comparisons/semversion.py
--rw-r--r--   0        0        0      519 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/comparisons/string.py
--rw-r--r--   0        0        0      295 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/comparisons/utils.py
--rw-r--r--   0        0        0      568 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/enum.py
--rw-r--r--   0        0        0     2623 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/main.py
--rw-r--r--   0        0        0        0 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/package_managers/__init__.py
--rw-r--r--   0        0        0     2519 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/package_managers/base_package_manager.py
--rw-r--r--   0        0        0     1242 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/package_managers/go.py
--rw-r--r--   0        0        0     1479 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/package_managers/jsonnet.py
--rw-r--r--   0        0        0     4102 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/package_managers/nodejs.py
--rw-r--r--   0        0        0     1933 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/package_managers/python.py
--rw-r--r--   0        0        0      271 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/package_managers/utilities/git.py
--rw-r--r--   0        0        0     2352 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/reporters/gh.py
--rw-r--r--   0        0        0     1476 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/reporters/terminal.py
--rw-r--r--   0        0        0     4265 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/rubrical.py
--rw-r--r--   0        0        0      467 2023-04-24 08:57:50.948844 rubrical-0.2.1/rubrical/schemas/configuration.py
--rw-r--r--   0        0        0      251 2023-04-24 08:57:50.948844 rubrical-0.2.1/rubrical/schemas/package.py
--rw-r--r--   0        0        0      235 2023-04-24 08:57:50.948844 rubrical-0.2.1/rubrical/schemas/results.py
--rw-r--r--   0        0        0      633 2023-04-24 08:57:50.948844 rubrical-0.2.1/rubrical/utilities/console.py
--rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 rubrical-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    15976 2023-06-27 15:14:04.314099 rubrical-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2782 2023-06-27 15:14:04.314099 rubrical-0.2.2/README.md
+-rw-r--r--   0        0        0     1843 2023-06-27 15:14:24.855625 rubrical-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 15:14:04.314099 rubrical-0.2.2/rubrical/__init__.py
+-rw-r--r--   0        0        0      784 2023-06-27 15:14:04.314099 rubrical-0.2.2/rubrical/comparisons/__init__.py
+-rw-r--r--   0        0        0     2255 2023-06-27 15:14:04.314099 rubrical-0.2.2/rubrical/comparisons/semversion.py
+-rw-r--r--   0        0        0      519 2023-06-27 15:14:04.314099 rubrical-0.2.2/rubrical/comparisons/string.py
+-rw-r--r--   0        0        0      295 2023-06-27 15:14:04.314099 rubrical-0.2.2/rubrical/comparisons/utils.py
+-rw-r--r--   0        0        0      568 2023-06-27 15:14:04.314099 rubrical-0.2.2/rubrical/enum.py
+-rw-r--r--   0        0        0     2623 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/main.py
+-rw-r--r--   0        0        0        0 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/package_managers/__init__.py
+-rw-r--r--   0        0        0     2519 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/package_managers/base_package_manager.py
+-rw-r--r--   0        0        0     1242 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/package_managers/go.py
+-rw-r--r--   0        0        0     1504 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/package_managers/jsonnet.py
+-rw-r--r--   0        0        0     4102 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/package_managers/nodejs.py
+-rw-r--r--   0        0        0     1933 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/package_managers/python.py
+-rw-r--r--   0        0        0      271 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/package_managers/utilities/git.py
+-rw-r--r--   0        0        0     2352 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/reporters/gh.py
+-rw-r--r--   0        0        0     1476 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/reporters/terminal.py
+-rw-r--r--   0        0        0     4265 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/rubrical.py
+-rw-r--r--   0        0        0      467 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/schemas/configuration.py
+-rw-r--r--   0        0        0      251 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/schemas/package.py
+-rw-r--r--   0        0        0      235 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/schemas/results.py
+-rw-r--r--   0        0        0      633 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/utilities/console.py
+-rw-r--r--   0        0        0     3753 1970-01-01 00:00:00.000000 rubrical-0.2.2/PKG-INFO
```

### Comparing `rubrical-0.2.1/LICENSE` & `rubrical-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.1/README.md` & `rubrical-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.1/pyproject.toml` & `rubrical-0.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 [tool.isort]
 profile = "black"
 
 [tool.setuptools_scm]
 
 [tool.poetry]
 name = "rubrical"
-version = "0.2.1"
+version = "0.2.2"
 description = "A CLI to encourage (😅) people to update their dependencies!"
 authors = ["Ivan Lee <ivanklee86@gmail.com>"]
 license = "MPL-2.0"
 homepage = "https://github.com/ivanklee86/rubrical"
 repository = "https://github.com/ivanklee86/rubrical"
 readme = "README.md"
 classifiers=[
@@ -43,19 +43,19 @@
 ]
 
 [tool.poetry.scripts]
 rubrical = "rubrical.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-typer = {extras = ["all"], version = "^0.7.0"}
+typer = {extras = ["all"], version = "^0.9.0"}
 pydantic = "^1.10.4"
 semver = "^3.0.0"
 pygithub = "^1.58.0"
-python-benedict = {extras = ["all"], version = "^0.30.0"}
+python-benedict = {extras = ["all"], version = "^0.31.0"}
 pyyaml = "^6.0"
 requirements-parser = "^0.5.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.0.0"
 mypy = "^1.0"
 pytest = "^7.2.0"
@@ -65,17 +65,16 @@
 pytest-html = "^3.2.0"
 pytest-mock = "^3.10.0"
 pytest-xdist = "^3.0.2"
 setuptools-scm = "^7.0.5"
 twine = "^4.0.2"
 pre-commit = "^3.0.0"
 isort = "^5.10.1"
-ruff = "^0.0.262"
+ruff = "^0.0.275"
 python-dotenv = "^1.0.0"
-typer-cli = "^0.0.13"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [build-system]
```

### Comparing `rubrical-0.2.1/rubrical/comparisons/__init__.py` & `rubrical-0.2.2/rubrical/comparisons/__init__.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.1/rubrical/comparisons/semversion.py` & `rubrical-0.2.2/rubrical/comparisons/semversion.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.1/rubrical/comparisons/string.py` & `rubrical-0.2.2/rubrical/comparisons/string.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.1/rubrical/enum.py` & `rubrical-0.2.2/rubrical/enum.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.1/rubrical/main.py` & `rubrical-0.2.2/rubrical/main.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.1/rubrical/package_managers/base_package_manager.py` & `rubrical-0.2.2/rubrical/package_managers/base_package_manager.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.1/rubrical/package_managers/go.py` & `rubrical-0.2.2/rubrical/package_managers/go.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.1/rubrical/package_managers/jsonnet.py` & `rubrical-0.2.2/rubrical/package_managers/jsonnet.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import json
-from typing import List
+from typing import List, Optional
 
 from pydantic import BaseModel
 
 from rubrical.enum import DependencySpecifications, SupportedPackageManagers
 from rubrical.package_managers.base_package_manager import BasePackageManager
 from rubrical.package_managers.utilities import git
 from rubrical.schemas.package import Package
 
 
 class JsonnetDependencySourceGit(BaseModel):
     remote: str
-    subdir: str
+    subdir: Optional[str] = ""
 
 
 class JsonnetDependencySource(BaseModel):
     git: JsonnetDependencySourceGit
 
 
 class JsonnetDependency(BaseModel):
```

### Comparing `rubrical-0.2.1/rubrical/package_managers/nodejs.py` & `rubrical-0.2.2/rubrical/package_managers/nodejs.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.1/rubrical/package_managers/python.py` & `rubrical-0.2.2/rubrical/package_managers/python.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.1/rubrical/reporters/gh.py` & `rubrical-0.2.2/rubrical/reporters/gh.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.1/rubrical/reporters/terminal.py` & `rubrical-0.2.2/rubrical/reporters/terminal.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.1/rubrical/rubrical.py` & `rubrical-0.2.2/rubrical/rubrical.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.1/rubrical/utilities/console.py` & `rubrical-0.2.2/rubrical/utilities/console.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.1/PKG-INFO` & `rubrical-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: rubrical
-Version: 0.2.1
+Version: 0.2.2
 Summary: A CLI to encourage (😅) people to update their dependencies!
 Home-page: https://github.com/ivanklee86/rubrical
 License: MPL-2.0
 Author: Ivan Lee
 Author-email: ivanklee86@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Requires-Dist: pygithub (>=1.58.0,<2.0.0)
-Requires-Dist: python-benedict[all] (>=0.30.0,<0.31.0)
+Requires-Dist: python-benedict[all] (>=0.31.0,<0.32.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requirements-parser (>=0.5.0,<0.6.0)
 Requires-Dist: semver (>=3.0.0,<4.0.0)
-Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/ivanklee86/rubrical
 Description-Content-Type: text/markdown
 
 # rubrical
 
 [![CI](https://github.com/ivanklee86/rubrical/actions/workflows/ci.yaml/badge.svg)](https://github.com/ivanklee86/rubrical/actions/workflows/ci.yaml) [![codecov](https://codecov.io/gh/ivanklee86/rubrical/branch/main/graph/badge.svg?token=9WJM4LBDEX)](https://codecov.io/gh/ivanklee86/rubrical) [![PyPI version](https://badge.fury.io/py/rubrical.svg)](https://badge.fury.io/py/rubrical)
```

