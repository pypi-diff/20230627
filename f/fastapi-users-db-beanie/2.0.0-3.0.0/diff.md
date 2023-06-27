# Comparing `tmp/fastapi_users_db_beanie-2.0.0.tar.gz` & `tmp/fastapi_users_db_beanie-3.0.0.tar.gz`

## Comparing `fastapi_users_db_beanie-2.0.0.tar` & `fastapi_users_db_beanie-3.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/.editorconfig
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/test_build.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/.github/stale.yml
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/fastapi_users_db_beanie/__init__.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/fastapi_users_db_beanie/access_token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/fastapi_users_db_beanie/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/tests/test_access_token.py
--rw-r--r--   0        0        0     7978 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/tests/test_fastapi_users_db_beanie.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/LICENSE
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/README.md
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/PKG-INFO
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-2.0.0/setup.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/.editorconfig
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/test_build.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/.github/stale.yml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/fastapi_users_db_beanie/__init__.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/fastapi_users_db_beanie/access_token.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/fastapi_users_db_beanie/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/tests/test_access_token.py
+-rw-r--r--   0        0        0     7978 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/tests/test_fastapi_users_db_beanie.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/README.md
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 fastapi_users_db_beanie-3.0.0/setup.py
```

### Comparing `fastapi_users_db_beanie-2.0.0/.github/stale.yml` & `fastapi_users_db_beanie-3.0.0/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_beanie-2.0.0/.github/ISSUE_TEMPLATE/bug_report.md` & `fastapi_users_db_beanie-3.0.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_beanie-2.0.0/.github/workflows/build.yml` & `fastapi_users_db_beanie-3.0.0/.github/workflows/build.yml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 jobs:
 
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python_version: [3.7, 3.8, 3.9, '3.10', '3.11']
+        python_version: [3.8, 3.9, '3.10', '3.11']
 
     services:
       mongo:
         image: mongo
         ports:
           - 27017:27017
 
@@ -50,15 +50,15 @@
     if: startsWith(github.ref, 'refs/tags/')
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: 3.7
+        python-version: 3.8
     - name: Install dependencies
       shell: bash
       run: |
         python -m pip install --upgrade pip
         pip install hatch
     - name: Build and publish on PyPI
       env:
```

### Comparing `fastapi_users_db_beanie-2.0.0/fastapi_users_db_beanie/__init__.py` & `fastapi_users_db_beanie-3.0.0/fastapi_users_db_beanie/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from fastapi_users.db.base import BaseUserDatabase
 from fastapi_users.exceptions import InvalidID
 from fastapi_users.models import ID, OAP
 from pydantic import BaseModel, Field
 from pymongo import IndexModel
 from pymongo.collation import Collation
 
-__version__ = "2.0.0"
+__version__ = "3.0.0"
 
 
 class BeanieBaseUser(BaseModel):
     email: str
     hashed_password: str
     is_active: bool = True
     is_superuser: bool = False
```

### Comparing `fastapi_users_db_beanie-2.0.0/fastapi_users_db_beanie/access_token.py` & `fastapi_users_db_beanie-3.0.0/fastapi_users_db_beanie/access_token.py`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_beanie-2.0.0/tests/conftest.py` & `fastapi_users_db_beanie-3.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_beanie-2.0.0/tests/test_access_token.py` & `fastapi_users_db_beanie-3.0.0/tests/test_access_token.py`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_beanie-2.0.0/tests/test_fastapi_users_db_beanie.py` & `fastapi_users_db_beanie-3.0.0/tests/test_fastapi_users_db_beanie.py`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_beanie-2.0.0/.gitignore` & `fastapi_users_db_beanie-3.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_beanie-2.0.0/LICENSE` & `fastapi_users_db_beanie-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_beanie-2.0.0/README.md` & `fastapi_users_db_beanie-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_users_db_beanie-2.0.0/pyproject.toml` & `fastapi_users_db_beanie-3.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -66,23 +66,22 @@
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
     "fastapi-users >= 10.0.1",
     "beanie >=1.11.0,<2.0.0",
 ]
 
 [project.urls]
 Documentation = "https://fastapi-users.github.io/fastapi-users"
```

### Comparing `fastapi_users_db_beanie-2.0.0/PKG-INFO` & `fastapi_users_db_beanie-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: fastapi-users-db-beanie
-Version: 2.0.0
+Version: 3.0.0
 Summary: FastAPI Users database adapter for Beanie
 Project-URL: Documentation, https://fastapi-users.github.io/fastapi-users
 Project-URL: Source, https://github.com/fastapi-users/fastapi-users-db-beanie
 Author-email: François Voron <fvoron@gmail.com>, Schwannden Kuo <schwannden@gmail.com>
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
 Requires-Dist: beanie<2.0.0,>=1.11.0
 Requires-Dist: fastapi-users>=10.0.1
 Description-Content-Type: text/markdown
 
 # FastAPI Users - Database adapter for Beanie
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: fastapi-users-db-beanie Version: 2.0.0 Summary:
+Metadata-Version: 2.1 Name: fastapi-users-db-beanie Version: 3.0.0 Summary:
 FastAPI Users database adapter for Beanie Project-URL: Documentation, https://
 fastapi-users.github.io/fastapi-users Project-URL: Source, https://github.com/
 fastapi-users/fastapi-users-db-beanie Author-email: FranÃ§ois Voron
 gmail.com>, Schwannden Kuo
 gmail.com> License-File: LICENSE Classifier: Development Status :: 5 -
 Production/Stable Classifier: Framework :: AsyncIO Classifier: Framework ::
 FastAPI Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Internet :: WWW/HTTP :: Session
-Requires-Python: >=3.7 Requires-Dist: beanie<2.0.0,>=1.11.0 Requires-Dist:
-fastapi-users>=10.0.1 Description-Content-Type: text/markdown # FastAPI Users -
-Database adapter for Beanie
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Internet :: WWW/HTTP :: Session Requires-Python: >=3.8 Requires-Dist:
+beanie<2.0.0,>=1.11.0 Requires-Dist: fastapi-users>=10.0.1 Description-Content-
+Type: text/markdown # FastAPI Users - Database adapter for Beanie
                                 [FastAPI Users]
           Ready-to-use and customizable users management for FastAPI
 [![build](https://github.com/fastapi-users/fastapi-users-db-beanie/workflows/
 Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/actions) [!
 [codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-beanie/branch/
 master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users-db-
 beanie) [![PyPI version](https://badge.fury.io/py/fastapi-users-db-beanie.svg)]
```

### Comparing `fastapi_users_db_beanie-2.0.0/setup.py` & `fastapi_users_db_beanie-3.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='fastapi-users-db-beanie',
-    version='2.0.0',
+    version='3.0.0',
     description='FastAPI Users database adapter for Beanie',
     long_description='# FastAPI Users - Database adapter for Beanie\n\n<p align="center">\n  <img src="https://raw.githubusercontent.com/frankie567/fastapi-users/master/logo.svg?sanitize=true" alt="FastAPI Users">\n</p>\n\n<p align="center">\n    <em>Ready-to-use and customizable users management for FastAPI</em>\n</p>\n\n[![build](https://github.com/fastapi-users/fastapi-users-db-beanie/workflows/Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/actions)\n[![codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-beanie/branch/master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users-db-beanie)\n[![PyPI version](https://badge.fury.io/py/fastapi-users-db-beanie.svg)](https://badge.fury.io/py/fastapi-users-db-beanie)\n[![Downloads](https://pepy.tech/badge/fastapi-users-db-beanie)](https://pepy.tech/project/fastapi-users-db-beanie)\n<p align="center">\n<a href="https://github.com/sponsors/frankie567"><img src="https://md-buttons.francoisvoron.com/button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50"></a>\n</p>\n\n---\n\n**Documentation**: <a href="https://fastapi-users.github.io/fastapi-users/" target="_blank">https://fastapi-users.github.io/fastapi-users/</a>\n\n**Source Code**: <a href="https://github.com/fastapi-users/fastapi-users" target="_blank">https://github.com/fastapi-users/fastapi-users</a>\n\n---\n\nAdd quickly a registration and authentication system to your [FastAPI](https://fastapi.tiangolo.com/) project. **FastAPI Users** is designed to be as customizable and adaptable as possible.\n\n**Sub-package for Beanie support in FastAPI Users.**\n\n## Development\n\n### Setup environment\n\nWe use [Hatch](https://hatch.pypa.io/latest/install/) to manage the development environment and production build. Ensure it\'s installed on your system.\n\n### Run unit tests\n\nYou can run all the tests with:\n\n```bash\nhatch run test\n```\n\n### Format the code\n\nExecute the following command to apply `isort` and `black` formatting:\n\n```bash\nhatch run lint\n```\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n',
     author_email='François Voron <fvoron@gmail.com>, Schwannden Kuo <schwannden@gmail.com>',
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
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*- from setuptools import setup setup( name='fastapi-
-users-db-beanie', version='2.0.0', description='FastAPI Users database adapter
+users-db-beanie', version='3.0.0', description='FastAPI Users database adapter
 for Beanie', long_description='# FastAPI Users - Database adapter for
 Beanie\n\n
                              \n [FastAPI Users]\n
 \n\n
         \n Ready-to-use and customizable users management for FastAPI\n
 \n\n[![build](https://github.com/fastapi-users/fastapi-users-db-beanie/
 workflows/Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/
@@ -27,13 +27,12 @@
 Format the code\n\nExecute the following command to apply `isort` and `black`
 formatting:\n\n```bash\nhatch run lint\n```\n\n## License\n\nThis project is
 licensed under the terms of the MIT license.\n', author_email='FranÃ§ois Voron
 gmail.com>, Schwannden Kuo
 gmail.com>', classifiers=[ 'Development Status :: 5 - Production/Stable',
 'Framework :: AsyncIO', 'Framework :: FastAPI', 'Intended Audience ::
 Developers', 'License :: OSI Approved :: MIT License', 'Programming Language ::
-Python :: 3 :: Only', 'Programming Language :: Python :: 3.7', 'Programming
-Language :: Python :: 3.8', 'Programming Language :: Python :: 3.9',
-'Programming Language :: Python :: 3.10', 'Programming Language :: Python ::
-3.11', 'Topic :: Internet :: WWW/HTTP :: Session', ], install_requires=
-[ 'beanie<2.0.0,>=1.11.0', 'fastapi-users>=10.0.1', ], packages=
-[ 'fastapi_users_db_beanie', 'tests', ], )
+Python :: 3 :: Only', 'Programming Language :: Python :: 3.8', 'Programming
+Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10',
+'Programming Language :: Python :: 3.11', 'Topic :: Internet :: WWW/HTTP ::
+Session', ], install_requires=[ 'beanie<2.0.0,>=1.11.0', 'fastapi-
+users>=10.0.1', ], packages=[ 'fastapi_users_db_beanie', 'tests', ], )
```

