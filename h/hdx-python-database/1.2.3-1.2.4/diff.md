# Comparing `tmp/hdx-python-database-1.2.3.tar.gz` & `tmp/hdx_python_database-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdx-python-database-1.2.3.tar", last modified: Sun Mar  5 22:16:18 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `hdx-python-database-1.2.3.tar` & `hdx_python_database-1.2.4.tar`

### file list

```diff
@@ -1,41 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:16:18.149290 hdx-python-database-1.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:16:18.145290 hdx-python-database-1.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:16:18.149290 hdx-python-database-1.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/.github/workflows/run-python-tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/.readthedocs.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-05 22:16:18.149290 hdx-python-database-1.2.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1112 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:16:18.149290 hdx-python-database-1.2.3/doc/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4060 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/doc/main.md
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1416 2023-03-05 22:16:18.149290 hdx-python-database-1.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:16:18.145290 hdx-python-database-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:16:18.145290 hdx-python-database-1.2.3/src/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:16:18.149290 hdx-python-database-1.2.3/src/hdx/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/src/hdx/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-05 22:16:18.000000 hdx-python-database-1.2.3/src/hdx/database/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/src/hdx/database/dburi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/src/hdx/database/no_timezone.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/src/hdx/database/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/src/hdx/database/with_timezone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:16:18.149290 hdx-python-database-1.2.3/src/hdx_python_database.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-05 22:16:18.000000 hdx-python-database-1.2.3/src/hdx_python_database.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-05 22:16:18.000000 hdx-python-database-1.2.3/src/hdx_python_database.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 22:16:18.000000 hdx-python-database-1.2.3/src/hdx_python_database.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-05 22:16:18.000000 hdx-python-database-1.2.3/src/hdx_python_database.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-05 22:16:18.000000 hdx-python-database-1.2.3/src/hdx_python_database.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 22:16:16.000000 hdx-python-database-1.2.3/src/hdx_python_database.egg-info/zip-safe
--rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:16:18.145290 hdx-python-database-1.2.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:16:18.145290 hdx-python-database-1.2.3/tests/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:16:18.149290 hdx-python-database-1.2.3/tests/hdx/database/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/tests/hdx/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/tests/hdx/database/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/tests/hdx/database/dbtestdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/tests/hdx/database/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/tests/hdx/database/test_dburi.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-05 22:16:03.000000 hdx-python-database-1.2.3/tests/hdx/database/test_postgresql.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     1520 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/.config/black.toml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/.config/coveragerc
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/.config/pytest.ini
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/documentation/.readthedocs.yaml
+-rwxr-xr-x   0        0        0     4060 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/documentation/main.md
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/documentation/pydoc-markdown.yaml
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/src/hdx/database/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/src/hdx/database/_version.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/src/hdx/database/dburi.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/src/hdx/database/no_timezone.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/src/hdx/database/postgresql.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/src/hdx/database/with_timezone.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/tests/hdx/database/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/tests/hdx/database/conftest.py
+-rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/tests/hdx/database/dbtestdate.py
+-rwxr-xr-x   0        0        0     3720 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/tests/hdx/database/test_database.py
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/tests/hdx/database/test_dburi.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/tests/hdx/database/test_postgresql.py
+-rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/LICENSE
+-rwxr-xr-x   0        0        0     1126 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/README.md
+-rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/PKG-INFO
```

### Comparing `hdx-python-database-1.2.3/.github/workflows/publish.yml` & `hdx_python_database-1.2.4/.github/workflows/publish.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -6,25 +6,28 @@
 
 jobs:
   publish:
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v3
-    - name: Get history and tags for SCM versioning to work
+    - name: Get history and tags for versioning to work
       run: |
         git fetch --prune --unshallow
         git fetch --depth=1 origin +refs/tags/*:refs/tags/*
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install --upgrade tox-gh-actions
-    - name: Publish with tox and twine
+        pip install --upgrade hatch
+    - name: Build with hatch
+      run: |
+        hatch build
+    - name: Publish with hatch
       env:
-        TWINE_USERNAME: ${{ secrets.TWINE_USERNAME }}
-        TWINE_PASSWORD: ${{ secrets.TWINE_PASSWORD }}
+        HATCH_INDEX_USER: ${{secrets.HATCH_INDEX_USER}}
+        HATCH_INDEX_AUTH: ${{secrets.HATCH_INDEX_AUTH}}
       run: |
-        tox -e publish
+        hatch publish
```

### Comparing `hdx-python-database-1.2.3/.github/workflows/run-python-tests.yml` & `hdx_python_database-1.2.4/.github/workflows/run-python-tests.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -20,20 +20,27 @@
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install --upgrade tox-gh-actions
-    - name: Test with tox/pytest
+        pip install --upgrade hatch
+    - name: Test with hatch/pytest
       run: |
-        tox
+        hatch run test:test
+    - name: Check styling
+      if: always()
+      run: |
+        hatch run lint:style
     - name: Publish Unit Test Results
       uses: EnricoMi/publish-unit-test-result-action@v2
       if: always()
       with:
         github_token: ${{ secrets.GITHUB_TOKEN }}
-        junit_files: .tox/*.xml
-    - name: Upload Coverage Results
-      uses: codecov/codecov-action@v3
-      if: success()
+        junit_files: test-results.xml
+    - name: Publish in Coveralls
+      uses: coverallsapp/github-action@v2
+      with:
+        github-token: ${{ secrets.GITHUB_TOKEN }}
+        flag-name: tests
+        format: lcov
```

### Comparing `hdx-python-database-1.2.3/.gitignore` & `hdx_python_database-1.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx-python-database-1.2.3/LICENSE` & `hdx_python_database-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx-python-database-1.2.3/PKG-INFO` & `hdx_python_database-1.2.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 Metadata-Version: 2.1
 Name: hdx-python-database
-Version: 1.2.3
+Version: 1.2.4
 Summary: HDX Python database utilities
-Home-page: https://github.com/OCHA-DAP/hdx-python-database
-Author: Michael Rans
-Author-email: rans@email.com
+Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-database
+Author-email: Michael Rans <rans@email.com>
 License: MIT
+License-File: LICENSE
 Keywords: HDX,database,postgresql
-Platform: any
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8
+Requires-Dist: sqlalchemy>=2
+Requires-Dist: sshtunnel
+Provides-Extra: dev
+Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: postgresql
-License-File: LICENSE
+Requires-Dist: psycopg[binary]; extra == 'postgresql'
+Provides-Extra: test
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Description-Content-Type: text/markdown
 
-[![Build Status](https://github.com/OCHA-DAP/hdx-python-database/actions/workflows/run-python-tests.yml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-database/actions/workflows/run-python-tests.yml)
-[![Coverage Status](https://codecov.io/gh/OCHA-DAP/hdx-python-database/branch/main/graph/badge.svg?token=JpWZc5js4y)](https://codecov.io/gh/OCHA-DAP/hdx-python-database)
+[![Build Status](https://github.com/OCHA-DAP/hdx-python-database/actions/workflows/run-python-tests.yaml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-database/actions/workflows/run-python-tests.yaml)
+[![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-database/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-database?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 The HDX Python Database Library provides utilities for connecting to databases in a standard way including
 through an ssh tunnel if needed. It is built on top of SQLAlchemy and simplifies its setup. 
 
 For more information, please read the [documentation](https://hdx-python-database.readthedocs.io/en/latest/).
 
 This library is part of the [Humanitarian Data Exchange](https://data.humdata.org/) (HDX) project. If you have 
-humanitarian related data, please upload your datasets to HDX.
+humanitarian related data, please upload your datasets to HDX.
```

### Comparing `hdx-python-database-1.2.3/README.md` & `hdx_python_database-1.2.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-[![Build Status](https://github.com/OCHA-DAP/hdx-python-database/actions/workflows/run-python-tests.yml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-database/actions/workflows/run-python-tests.yml)
-[![Coverage Status](https://codecov.io/gh/OCHA-DAP/hdx-python-database/branch/main/graph/badge.svg?token=JpWZc5js4y)](https://codecov.io/gh/OCHA-DAP/hdx-python-database)
+[![Build Status](https://github.com/OCHA-DAP/hdx-python-database/actions/workflows/run-python-tests.yaml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-database/actions/workflows/run-python-tests.yaml)
+[![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-database/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-database?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 The HDX Python Database Library provides utilities for connecting to databases in a standard way including
 through an ssh tunnel if needed. It is built on top of SQLAlchemy and simplifies its setup. 
 
 For more information, please read the [documentation](https://hdx-python-database.readthedocs.io/en/latest/).
```

### Comparing `hdx-python-database-1.2.3/doc/main.md` & `hdx_python_database-1.2.4/documentation/main.md`

 * *Files identical despite different names*

### Comparing `hdx-python-database-1.2.3/src/hdx/database/__init__.py` & `hdx_python_database-1.2.4/src/hdx/database/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from ._version import version as __version__  # noqa: F401
-
 """Database utilities"""
 import logging
 from typing import Any, Optional, Type, Union
 
 from sqlalchemy import create_engine
 from sqlalchemy.orm import DeclarativeBase, Session, sessionmaker
 from sqlalchemy.pool import NullPool
 from sshtunnel import SSHTunnelForwarder
 
+from ._version import version as __version__  # noqa: F401
 from .dburi import get_connection_uri
 from .no_timezone import Base as NoTZBase
 from .postgresql import wait_for_postgresql
 from .with_timezone import Base
 
 logger = logging.getLogger(__name__)
```

### Comparing `hdx-python-database-1.2.3/src/hdx/database/dburi.py` & `hdx_python_database-1.2.4/src/hdx/database/dburi.py`

 * *Files identical despite different names*

### Comparing `hdx-python-database-1.2.3/src/hdx/database/no_timezone.py` & `hdx_python_database-1.2.4/src/hdx/database/no_timezone.py`

 * *Files identical despite different names*

### Comparing `hdx-python-database-1.2.3/src/hdx/database/postgresql.py` & `hdx_python_database-1.2.4/src/hdx/database/postgresql.py`

 * *Files identical despite different names*

### Comparing `hdx-python-database-1.2.3/tests/hdx/database/dbtestdate.py` & `hdx_python_database-1.2.4/tests/hdx/database/dbtestdate.py`

 * *Files identical despite different names*

### Comparing `hdx-python-database-1.2.3/tests/hdx/database/test_database.py` & `hdx_python_database-1.2.4/tests/hdx/database/test_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 from datetime import datetime, timezone
 from os.path import join
 
 import pytest
 from sqlalchemy import select
 from sshtunnel import SSHTunnelForwarder
 
+from .dbtestdate import DBTestDate
 from hdx.database import Base, Database
 from hdx.database.no_timezone import Base as NoTZBase
 
-from .dbtestdate import DBTestDate
-
 
 class TestDatabase:
     started = False
     stopped = False
     table_base = NoTZBase
     dbpath = join("tests", "test_database.db")
     params_pg = {
```

### Comparing `hdx-python-database-1.2.3/tests/hdx/database/test_dburi.py` & `hdx_python_database-1.2.4/tests/hdx/database/test_dburi.py`

 * *Files identical despite different names*

