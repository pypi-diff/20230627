# Comparing `tmp/selenium_testing_library-2023.5.tar.gz` & `tmp/selenium_testing_library-2023.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_testing_library-2023.5.tar", max compression
+gzip compressed data, was "selenium_testing_library-2023.6.tar", max compression
```

## Comparing `selenium_testing_library-2023.5.tar` & `selenium_testing_library-2023.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2021-06-06 09:30:53.872504 selenium_testing_library-2023.5/LICENSE.md
--rw-r--r--   0        0        0     9946 2023-06-26 15:30:47.718558 selenium_testing_library-2023.5/README.md
--rw-r--r--   0        0        0     1886 2023-06-26 15:30:47.719242 selenium_testing_library-2023.5/pyproject.toml
--rw-r--r--   0        0        0       60 2023-06-26 15:16:59.346228 selenium_testing_library-2023.5/selenium_testing_library/__init__.py
--rw-r--r--   0        0        0     7525 2023-02-17 17:32:49.420064 selenium_testing_library-2023.5/selenium_testing_library/locators.py
--rw-r--r--   0        0        0   220550 2023-05-18 15:28:50.991379 selenium_testing_library-2023.5/selenium_testing_library/main.js
--rw-r--r--   0        0        0        0 2021-06-05 14:50:48.385384 selenium_testing_library-2023.5/selenium_testing_library/py.typed
--rw-r--r--   0        0        0    34005 2023-02-17 17:51:00.247649 selenium_testing_library-2023.5/selenium_testing_library/screen.py
--rw-r--r--   0        0        0    10921 1970-01-01 00:00:00.000000 selenium_testing_library-2023.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2021-06-06 09:30:53.872504 selenium_testing_library-2023.6/LICENSE.md
+-rw-r--r--   0        0        0     9941 2023-06-27 13:27:00.617253 selenium_testing_library-2023.6/README.md
+-rw-r--r--   0        0        0     1856 2023-06-27 13:30:57.071298 selenium_testing_library-2023.6/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-06-27 13:30:57.071734 selenium_testing_library-2023.6/selenium_testing_library/__init__.py
+-rw-r--r--   0        0        0     7525 2023-02-17 17:32:49.420064 selenium_testing_library-2023.6/selenium_testing_library/locators.py
+-rw-r--r--   0        0        0   220550 2023-05-18 15:28:50.991379 selenium_testing_library-2023.6/selenium_testing_library/main.js
+-rw-r--r--   0        0        0        0 2021-06-05 14:50:48.385384 selenium_testing_library-2023.6/selenium_testing_library/py.typed
+-rw-r--r--   0        0        0    34017 2023-06-27 13:27:00.618716 selenium_testing_library-2023.6/selenium_testing_library/screen.py
+-rw-r--r--   0        0        0    10782 1970-01-01 00:00:00.000000 selenium_testing_library-2023.6/PKG-INFO
```

### Comparing `selenium_testing_library-2023.5/LICENSE.md` & `selenium_testing_library-2023.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_testing_library-2023.5/README.md` & `selenium_testing_library-2023.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![PyPI version](https://badge.fury.io/py/selenium-testing-library.svg)](https://badge.fury.io/py/selenium-testing-library)
 [![test](https://github.com/anze3db/selenium-testing-library/actions/workflows/main.yml/badge.svg)](https://github.com/anze3db/selenium-testing-library/actions/workflows/main.yml) [![codecov](https://codecov.io/gh/anze3db/selenium-testing-library/branch/main/graph/badge.svg?token=L1M7HO3DL7)](https://codecov.io/gh/anze3db/selenium-testing-library)
 
 Selenium Testing Library (STL) is a Python library implementing [Testing-Library](https://testing-library.com/) in Selenium.
 
 ## Dependencies
 
-- Python 3.7, 3.8, 3.9, 3.10, 3.11, 3.12-dev
+- Python 3.8, 3.9, 3.10, 3.11, 3.12-dev
 - [`selenium`](https://pypi.org/project/selenium/) >= 3.0.0, [`typing-extensions`](https://pypi.org/project/typing-extensions/) >= 4.0.0
 ## Installation
 
 ```
 pip install selenium-testing-library
 ```
```

### Comparing `selenium_testing_library-2023.5/pyproject.toml` & `selenium_testing_library-2023.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [tool.poetry]
 name = "selenium-testing-library"
-version = "2023.5"
+version = "2023.6"
 description = "A Python Selenium library inspired by the Testing Library"
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/anze3db/selenium-testing-library"
 authors = ["Anže Pečar <anze@pecar.me>"]
 include = [
     "selenium_testing_library/main.js"
 ]
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/anze3db/selenium-testing-library/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 selenium = ">3.0.0"
-typing_extensions = ">=4.0.0"
-ruff = "^0.0.247"
 
 [tool.poetry.dev-dependencies]
+ruff = "^0.0.247"
 pytest = "*"
 black = "*"
 pytest-cov = "*"
 pytest-watch = "*"
 mypy = "*"
 isort = "*"
 tox = "*"
@@ -41,15 +40,15 @@
 addopts = "--selenium-headless --cov=selenium_testing_library --cov-report html --cov-report xml --verbose --durations=10"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "2023.5"
+current_version = "2023.6"
 version_pattern = "YYYY.INC1"
 commit_message = "Bump version from {old_version} to {new_version} 🚀"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
@@ -61,19 +60,19 @@
     '__version__ = "{version}"'
 ]
 "tests/test_selenium_testing_library.py" = [
     'assert __version__ == "{version}"'
 ]
 
 [tool.mypy]
-python_version = "3.7"
+python_version = "3.8"
 warn_unused_configs = true
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
 select = [
     # Pyflakes
     "F",
     # Pycodestyle
     "E",
     "W",
     # isort
```

### Comparing `selenium_testing_library-2023.5/selenium_testing_library/locators.py` & `selenium_testing_library-2023.6/selenium_testing_library/locators.py`

 * *Files identical despite different names*

### Comparing `selenium_testing_library-2023.5/selenium_testing_library/main.js` & `selenium_testing_library-2023.6/selenium_testing_library/main.js`

 * *Files identical despite different names*

### Comparing `selenium_testing_library-2023.5/selenium_testing_library/screen.py` & `selenium_testing_library-2023.6/selenium_testing_library/screen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 from pathlib import Path
-from typing import Any, Callable, Generic, List, Optional, TypeVar, Union, cast
+from typing import (
+    Any,
+    Callable,
+    Generic,
+    List,
+    Optional,
+    Protocol,
+    TypeVar,
+    Union,
+    cast,
+)
 
 from selenium.common.exceptions import (
     NoSuchElementException,
     TimeoutException,
     WebDriverException,
 )
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions
 from selenium.webdriver.support.ui import WebDriverWait
-from typing_extensions import Protocol
 
 from . import locators
 
 testing_library = (Path(__file__).parent / Path("main.js")).read_text()
 
 Locator = locators.LocatorType
```

### Comparing `selenium_testing_library-2023.5/PKG-INFO` & `selenium_testing_library-2023.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 Metadata-Version: 2.1
 Name: selenium-testing-library
-Version: 2023.5
+Version: 2023.6
 Summary: A Python Selenium library inspired by the Testing Library
 Home-page: https://github.com/anze3db/selenium-testing-library
 License: MIT
 Author: Anže Pečar
 Author-email: anze@pecar.me
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: ruff (>=0.0.247,<0.0.248)
 Requires-Dist: selenium (>3.0.0)
-Requires-Dist: typing_extensions (>=4.0.0)
 Project-URL: Changelog, https://github.com/anze3db/selenium-testing-library/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/anze3db/selenium-testing-library
 Description-Content-Type: text/markdown
 
 # Selenium Testing Library
 
 [![PyPI version](https://badge.fury.io/py/selenium-testing-library.svg)](https://badge.fury.io/py/selenium-testing-library)
 [![test](https://github.com/anze3db/selenium-testing-library/actions/workflows/main.yml/badge.svg)](https://github.com/anze3db/selenium-testing-library/actions/workflows/main.yml) [![codecov](https://codecov.io/gh/anze3db/selenium-testing-library/branch/main/graph/badge.svg?token=L1M7HO3DL7)](https://codecov.io/gh/anze3db/selenium-testing-library)
 
 Selenium Testing Library (STL) is a Python library implementing [Testing-Library](https://testing-library.com/) in Selenium.
 
 ## Dependencies
 
-- Python 3.7, 3.8, 3.9, 3.10, 3.11, 3.12-dev
+- Python 3.8, 3.9, 3.10, 3.11, 3.12-dev
 - [`selenium`](https://pypi.org/project/selenium/) >= 3.0.0, [`typing-extensions`](https://pypi.org/project/typing-extensions/) >= 4.0.0
 ## Installation
 
 ```
 pip install selenium-testing-library
 ```
```

