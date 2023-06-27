# Comparing `tmp/fastapi_users_db_sqlalchemy-5.0.0.tar.gz` & `tmp/fastapi_users_db_sqlalchemy-6.0.0.tar.gz`

## Comparing `fastapi_users_db_sqlalchemy-5.0.0.tar` & `fastapi_users_db_sqlalchemy-6.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/.editorconfig
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/Makefile
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/test_build.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/.github/stale.yml
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/fastapi_users_db_sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/fastapi_users_db_sqlalchemy/access_token.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/fastapi_users_db_sqlalchemy/generics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/fastapi_users_db_sqlalchemy/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/tests/__init__.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/tests/conftest.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/tests/test_access_token.py
--rw-r--r--   0        0        0     6760 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/tests/test_users.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/LICENSE
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/README.md
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/PKG-INFO
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-5.0.0/setup.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/.editorconfig
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/Makefile
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/test_build.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/.github/stale.yml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/fastapi_users_db_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/fastapi_users_db_sqlalchemy/access_token.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/fastapi_users_db_sqlalchemy/generics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/fastapi_users_db_sqlalchemy/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/tests/test_access_token.py
+-rw-r--r--   0        0        0     6760 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/tests/test_users.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/LICENSE
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/README.md
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 fastapi_users_db_sqlalchemy-6.0.0/setup.py
```

### Comparing `fastapi_users_db_sqlalchemy-5.0.0/.github/stale.yml` & `fastapi_users_db_sqlalchemy-6.0.0/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_sqlalchemy-5.0.0/.github/ISSUE_TEMPLATE/bug_report.md` & `fastapi_users_db_sqlalchemy-6.0.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_sqlalchemy-5.0.0/.github/workflows/build.yml` & `fastapi_users_db_sqlalchemy-6.0.0/.github/workflows/build.yml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
           MARIADB_DATABASE: fastapiusers
           MARIADB_USER: fastapiusers
           MARIADB_PASSWORD: fastapiuserspassword
 
     strategy:
       fail-fast: false
       matrix:
-        python_version: [3.7, 3.8, 3.9, '3.10', '3.11']
+        python_version: [3.8, 3.9, '3.10', '3.11']
         database_url:
           [
             "sqlite+aiosqlite:///./test-fastapiusers.db",
             "postgresql+asyncpg://fastapiusers:fastapiuserspassword@localhost:5432/fastapiusers",
             "mysql+aiomysql://root:fastapiuserspassword@localhost:3306/fastapiusers",
           ]
 
@@ -78,15 +78,15 @@
     if: startsWith(github.ref, 'refs/tags/')
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: 3.7
+          python-version: 3.8
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install hatch
       - name: Build and publish on PyPI
         env:
           HATCH_INDEX_USER: ${{ secrets.HATCH_INDEX_USER }}
```

### Comparing `fastapi_users_db_sqlalchemy-5.0.0/fastapi_users_db_sqlalchemy/__init__.py` & `fastapi_users_db_sqlalchemy-6.0.0/fastapi_users_db_sqlalchemy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from sqlalchemy import Boolean, ForeignKey, Integer, String, func, select
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.orm import Mapped, declared_attr, mapped_column
 from sqlalchemy.sql import Select
 
 from fastapi_users_db_sqlalchemy.generics import GUID
 
-__version__ = "5.0.0"
+__version__ = "6.0.0"
 
 UUID_ID = uuid.UUID
 
 
 class SQLAlchemyBaseUserTable(Generic[ID]):
     """Base SQLAlchemy users table definition."""
```

### Comparing `fastapi_users_db_sqlalchemy-5.0.0/fastapi_users_db_sqlalchemy/access_token.py` & `fastapi_users_db_sqlalchemy-6.0.0/fastapi_users_db_sqlalchemy/access_token.py`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_sqlalchemy-5.0.0/fastapi_users_db_sqlalchemy/generics.py` & `fastapi_users_db_sqlalchemy-6.0.0/fastapi_users_db_sqlalchemy/generics.py`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_sqlalchemy-5.0.0/tests/conftest.py` & `fastapi_users_db_sqlalchemy-6.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_sqlalchemy-5.0.0/tests/test_access_token.py` & `fastapi_users_db_sqlalchemy-6.0.0/tests/test_access_token.py`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_sqlalchemy-5.0.0/tests/test_users.py` & `fastapi_users_db_sqlalchemy-6.0.0/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_sqlalchemy-5.0.0/.gitignore` & `fastapi_users_db_sqlalchemy-6.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_sqlalchemy-5.0.0/LICENSE` & `fastapi_users_db_sqlalchemy-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_sqlalchemy-5.0.0/README.md` & `fastapi_users_db_sqlalchemy-6.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 </p>
 
 [![build](https://github.com/fastapi-users/fastapi-users-db-sqlalchemy/workflows/Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/actions)
 [![codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-sqlalchemy/branch/master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users-db-sqlalchemy)
 [![PyPI version](https://badge.fury.io/py/fastapi-users-db-sqlalchemy.svg)](https://badge.fury.io/py/fastapi-users-db-sqlalchemy)
 [![Downloads](https://pepy.tech/badge/fastapi-users-db-sqlalchemy)](https://pepy.tech/project/fastapi-users-db-sqlalchemy)
 <p align="center">
-<a href="https://github.com/sponsors/frankie567"><img src="https://md-btn.deta.dev/button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50"></a>
+<a href="https://github.com/sponsors/frankie567"><img src="https://md-buttons.francoisvoron.com/button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50"></a>
 </p>
 
 ---
 
 **Documentation**: <a href="https://fastapi-users.github.io/fastapi-users/" target="_blank">https://fastapi-users.github.io/fastapi-users/</a>
 
 **Source Code**: <a href="https://github.com/fastapi-users/fastapi-users" target="_blank">https://github.com/fastapi-users/fastapi-users</a>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 workflows/Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/
 actions) [![codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-
 sqlalchemy/branch/master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/
 fastapi-users-db-sqlalchemy) [![PyPI version](https://badge.fury.io/py/fastapi-
 users-db-sqlalchemy.svg)](https://badge.fury.io/py/fastapi-users-db-sqlalchemy)
 [![Downloads](https://pepy.tech/badge/fastapi-users-db-sqlalchemy)](https://
 pepy.tech/project/fastapi-users-db-sqlalchemy)
-                           [https://md-btn.deta.dev/
+                    [https://md-buttons.francoisvoron.com/
 button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50]
 --- **Documentation**: https://fastapi-users.github.io/fastapi-users/ **Source
 Code**: https://github.com/fastapi-users/fastapi-users --- Add quickly a
 registration and authentication system to your [FastAPI](https://
 fastapi.tiangolo.com/) project. **FastAPI Users** is designed to be as
 customizable and adaptable as possible. **Sub-package for SQLAlchemy ORM
 support in FastAPI Users.** ## Development ### Setup environment We use [Hatch]
```

### Comparing `fastapi_users_db_sqlalchemy-5.0.0/pyproject.toml` & `fastapi_users_db_sqlalchemy-6.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -67,23 +67,22 @@
 dynamic = ["version"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Development Status :: 5 - Production/Stable",
     "Framework :: FastAPI",
     "Framework :: AsyncIO",
     "Intended Audience :: Developers",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Internet :: WWW/HTTP :: Session",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "fastapi-users >= 10.0.0",
     "sqlalchemy[asyncio] >=2.0.0,<2.1.0",
 ]
 
 [project.urls]
 Documentation = "https://fastapi-users.github.io/fastapi-users"
```

### Comparing `fastapi_users_db_sqlalchemy-5.0.0/PKG-INFO` & `fastapi_users_db_sqlalchemy-6.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: fastapi-users-db-sqlalchemy
-Version: 5.0.0
+Version: 6.0.0
 Summary: FastAPI Users database adapter for SQLAlchemy
 Project-URL: Documentation, https://fastapi-users.github.io/fastapi-users
 Project-URL: Source, https://github.com/fastapi-users/fastapi-users-db-sqlalchemy
 Author-email: François Voron <fvoron@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: FastAPI
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: fastapi-users>=10.0.0
 Requires-Dist: sqlalchemy[asyncio]<2.1.0,>=2.0.0
 Description-Content-Type: text/markdown
 
 # FastAPI Users - Database adapter for SQLAlchemy ORM
 
 <p align="center">
@@ -34,15 +33,15 @@
 </p>
 
 [![build](https://github.com/fastapi-users/fastapi-users-db-sqlalchemy/workflows/Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/actions)
 [![codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-sqlalchemy/branch/master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users-db-sqlalchemy)
 [![PyPI version](https://badge.fury.io/py/fastapi-users-db-sqlalchemy.svg)](https://badge.fury.io/py/fastapi-users-db-sqlalchemy)
 [![Downloads](https://pepy.tech/badge/fastapi-users-db-sqlalchemy)](https://pepy.tech/project/fastapi-users-db-sqlalchemy)
 <p align="center">
-<a href="https://github.com/sponsors/frankie567"><img src="https://md-btn.deta.dev/button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50"></a>
+<a href="https://github.com/sponsors/frankie567"><img src="https://md-buttons.francoisvoron.com/button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50"></a>
 </p>
 
 ---
 
 **Documentation**: <a href="https://fastapi-users.github.io/fastapi-users/" target="_blank">https://fastapi-users.github.io/fastapi-users/</a>
 
 **Source Code**: <a href="https://github.com/fastapi-users/fastapi-users" target="_blank">https://github.com/fastapi-users/fastapi-users</a>
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: fastapi-users-db-sqlalchemy Version: 5.0.0 Summary:
+Metadata-Version: 2.1 Name: fastapi-users-db-sqlalchemy Version: 6.0.0 Summary:
 FastAPI Users database adapter for SQLAlchemy Project-URL: Documentation,
 https://fastapi-users.github.io/fastapi-users Project-URL: Source, https://
 github.com/fastapi-users/fastapi-users-db-sqlalchemy Author-email: FranÃ§ois
 Voron
 gmail.com> License-File: LICENSE Classifier: Development Status :: 5 -
 Production/Stable Classifier: Framework :: AsyncIO Classifier: Framework ::
 FastAPI Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Internet :: WWW/HTTP :: Session
-Requires-Python: >=3.7 Requires-Dist: fastapi-users>=10.0.0 Requires-Dist:
-sqlalchemy[asyncio]<2.1.0,>=2.0.0 Description-Content-Type: text/markdown #
-FastAPI Users - Database adapter for SQLAlchemy ORM
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Internet :: WWW/HTTP :: Session Requires-Python: >=3.8 Requires-Dist: fastapi-
+users>=10.0.0 Requires-Dist: sqlalchemy[asyncio]<2.1.0,>=2.0.0 Description-
+Content-Type: text/markdown # FastAPI Users - Database adapter for SQLAlchemy
+ORM
                                 [FastAPI Users]
           Ready-to-use and customizable users management for FastAPI
 [![build](https://github.com/fastapi-users/fastapi-users-db-sqlalchemy/
 workflows/Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/
 actions) [![codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-
 sqlalchemy/branch/master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/
 fastapi-users-db-sqlalchemy) [![PyPI version](https://badge.fury.io/py/fastapi-
 users-db-sqlalchemy.svg)](https://badge.fury.io/py/fastapi-users-db-sqlalchemy)
 [![Downloads](https://pepy.tech/badge/fastapi-users-db-sqlalchemy)](https://
 pepy.tech/project/fastapi-users-db-sqlalchemy)
-                           [https://md-btn.deta.dev/
+                    [https://md-buttons.francoisvoron.com/
 button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50]
 --- **Documentation**: https://fastapi-users.github.io/fastapi-users/ **Source
 Code**: https://github.com/fastapi-users/fastapi-users --- Add quickly a
 registration and authentication system to your [FastAPI](https://
 fastapi.tiangolo.com/) project. **FastAPI Users** is designed to be as
 customizable and adaptable as possible. **Sub-package for SQLAlchemy ORM
 support in FastAPI Users.** ## Development ### Setup environment We use [Hatch]
```

### Comparing `fastapi_users_db_sqlalchemy-5.0.0/setup.py` & `fastapi_users_db_sqlalchemy-6.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='fastapi-users-db-sqlalchemy',
-    version='5.0.0',
+    version='6.0.0',
     description='FastAPI Users database adapter for SQLAlchemy',
-    long_description='# FastAPI Users - Database adapter for SQLAlchemy ORM\n\n<p align="center">\n  <img src="https://raw.githubusercontent.com/frankie567/fastapi-users/master/logo.svg?sanitize=true" alt="FastAPI Users">\n</p>\n\n<p align="center">\n    <em>Ready-to-use and customizable users management for FastAPI</em>\n</p>\n\n[![build](https://github.com/fastapi-users/fastapi-users-db-sqlalchemy/workflows/Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/actions)\n[![codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-sqlalchemy/branch/master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users-db-sqlalchemy)\n[![PyPI version](https://badge.fury.io/py/fastapi-users-db-sqlalchemy.svg)](https://badge.fury.io/py/fastapi-users-db-sqlalchemy)\n[![Downloads](https://pepy.tech/badge/fastapi-users-db-sqlalchemy)](https://pepy.tech/project/fastapi-users-db-sqlalchemy)\n<p align="center">\n<a href="https://github.com/sponsors/frankie567"><img src="https://md-btn.deta.dev/button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50"></a>\n</p>\n\n---\n\n**Documentation**: <a href="https://fastapi-users.github.io/fastapi-users/" target="_blank">https://fastapi-users.github.io/fastapi-users/</a>\n\n**Source Code**: <a href="https://github.com/fastapi-users/fastapi-users" target="_blank">https://github.com/fastapi-users/fastapi-users</a>\n\n---\n\nAdd quickly a registration and authentication system to your [FastAPI](https://fastapi.tiangolo.com/) project. **FastAPI Users** is designed to be as customizable and adaptable as possible.\n\n**Sub-package for SQLAlchemy ORM support in FastAPI Users.**\n\n## Development\n\n### Setup environment\n\nWe use [Hatch](https://hatch.pypa.io/latest/install/) to manage the development environment and production build. Ensure it\'s installed on your system.\n\n### Run unit tests\n\nYou can run all the tests with:\n\n```bash\nhatch run test\n```\n\n### Format the code\n\nExecute the following command to apply `isort` and `black` formatting:\n\n```bash\nhatch run lint\n```\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n',
+    long_description='# FastAPI Users - Database adapter for SQLAlchemy ORM\n\n<p align="center">\n  <img src="https://raw.githubusercontent.com/frankie567/fastapi-users/master/logo.svg?sanitize=true" alt="FastAPI Users">\n</p>\n\n<p align="center">\n    <em>Ready-to-use and customizable users management for FastAPI</em>\n</p>\n\n[![build](https://github.com/fastapi-users/fastapi-users-db-sqlalchemy/workflows/Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/actions)\n[![codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-sqlalchemy/branch/master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users-db-sqlalchemy)\n[![PyPI version](https://badge.fury.io/py/fastapi-users-db-sqlalchemy.svg)](https://badge.fury.io/py/fastapi-users-db-sqlalchemy)\n[![Downloads](https://pepy.tech/badge/fastapi-users-db-sqlalchemy)](https://pepy.tech/project/fastapi-users-db-sqlalchemy)\n<p align="center">\n<a href="https://github.com/sponsors/frankie567"><img src="https://md-buttons.francoisvoron.com/button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50"></a>\n</p>\n\n---\n\n**Documentation**: <a href="https://fastapi-users.github.io/fastapi-users/" target="_blank">https://fastapi-users.github.io/fastapi-users/</a>\n\n**Source Code**: <a href="https://github.com/fastapi-users/fastapi-users" target="_blank">https://github.com/fastapi-users/fastapi-users</a>\n\n---\n\nAdd quickly a registration and authentication system to your [FastAPI](https://fastapi.tiangolo.com/) project. **FastAPI Users** is designed to be as customizable and adaptable as possible.\n\n**Sub-package for SQLAlchemy ORM support in FastAPI Users.**\n\n## Development\n\n### Setup environment\n\nWe use [Hatch](https://hatch.pypa.io/latest/install/) to manage the development environment and production build. Ensure it\'s installed on your system.\n\n### Run unit tests\n\nYou can run all the tests with:\n\n```bash\nhatch run test\n```\n\n### Format the code\n\nExecute the following command to apply `isort` and `black` formatting:\n\n```bash\nhatch run lint\n```\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n',
     author_email='François Voron <fvoron@gmail.com>',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Framework :: AsyncIO',
         'Framework :: FastAPI',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Internet :: WWW/HTTP :: Session',
     ],
     install_requires=[
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*- from setuptools import setup setup( name='fastapi-
-users-db-sqlalchemy', version='5.0.0', description='FastAPI Users database
+users-db-sqlalchemy', version='6.0.0', description='FastAPI Users database
 adapter for SQLAlchemy', long_description='# FastAPI Users - Database adapter
 for SQLAlchemy ORM\n\n
                              \n [FastAPI Users]\n
 \n\n
         \n Ready-to-use and customizable users management for FastAPI\n
 \n\n[![build](https://github.com/fastapi-users/fastapi-users-db-sqlalchemy/
 workflows/Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/
 actions)\n[![codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-
 sqlalchemy/branch/master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/
 fastapi-users-db-sqlalchemy)\n[![PyPI version](https://badge.fury.io/py/
 fastapi-users-db-sqlalchemy.svg)](https://badge.fury.io/py/fastapi-users-db-
 sqlalchemy)\n[![Downloads](https://pepy.tech/badge/fastapi-users-db-
 sqlalchemy)](https://pepy.tech/project/fastapi-users-db-sqlalchemy)\n
-                          \n[https://md-btn.deta.dev/
+                   \n[https://md-buttons.francoisvoron.com/
 button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50]\n
 \n\n---\n\n**Documentation**: https://fastapi-users.github.io/fastapi-users/
 \n\n**Source Code**: https://github.com/fastapi-users/fastapi-users\n\n---
 \n\nAdd quickly a registration and authentication system to your [FastAPI]
 (https://fastapi.tiangolo.com/) project. **FastAPI Users** is designed to be as
 customizable and adaptable as possible.\n\n**Sub-package for SQLAlchemy ORM
 support in FastAPI Users.**\n\n## Development\n\n### Setup environment\n\nWe
@@ -27,13 +27,13 @@
 test\n```\n\n### Format the code\n\nExecute the following command to apply
 `isort` and `black` formatting:\n\n```bash\nhatch run lint\n```\n\n##
 License\n\nThis project is licensed under the terms of the MIT license.\n',
 author_email='FranÃ§ois Voron
 gmail.com>', classifiers=[ 'Development Status :: 5 - Production/Stable',
 'Framework :: AsyncIO', 'Framework :: FastAPI', 'Intended Audience ::
 Developers', 'License :: OSI Approved :: MIT License', 'Programming Language ::
-Python :: 3 :: Only', 'Programming Language :: Python :: 3.7', 'Programming
-Language :: Python :: 3.8', 'Programming Language :: Python :: 3.9',
-'Programming Language :: Python :: 3.10', 'Programming Language :: Python ::
-3.11', 'Topic :: Internet :: WWW/HTTP :: Session', ], install_requires=
-[ 'fastapi-users>=10.0.0', 'sqlalchemy[asyncio]<2.1.0,>=2.0.0', ], packages=
-[ 'fastapi_users_db_sqlalchemy', 'tests', ], )
+Python :: 3 :: Only', 'Programming Language :: Python :: 3.8', 'Programming
+Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10',
+'Programming Language :: Python :: 3.11', 'Topic :: Internet :: WWW/HTTP ::
+Session', ], install_requires=[ 'fastapi-users>=10.0.0', 'sqlalchemy
+[asyncio]<2.1.0,>=2.0.0', ], packages=[ 'fastapi_users_db_sqlalchemy', 'tests',
+], )
```

