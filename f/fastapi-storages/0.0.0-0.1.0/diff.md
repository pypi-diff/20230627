# Comparing `tmp/fastapi-storages-0.0.0.tar.gz` & `tmp/fastapi_storages-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-storages-0.0.0.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `fastapi-storages-0.0.0.tar` & `fastapi_storages-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0     1067 2022-05-31 17:23:51.535806 fastapi-storages-0.0.0/LICENSE
--rw-r--r--   0        0        0     3030 2022-06-17 08:26:28.591384 fastapi-storages-0.0.0/README.md
--rw-r--r--   0        0        0       24 2022-05-31 17:23:51.616259 fastapi-storages-0.0.0/fastapi_storages/__init__.py
--rw-r--r--   0        0        0        0 2022-06-16 11:38:19.425074 fastapi-storages-0.0.0/fastapi_storages/filesystem.py
--rw-r--r--   0        0        0       24 2022-06-17 08:27:19.344665 fastapi-storages-0.0.0/fastapi_storages/protocols.py
--rw-r--r--   0        0        0        0 2022-05-31 17:23:51.618382 fastapi-storages-0.0.0/fastapi_storages/py.typed
--rw-r--r--   0        0        0     2206 2022-06-16 10:10:52.769778 fastapi-storages-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     3769 2022-06-17 08:28:29.463781 fastapi-storages-0.0.0/setup.py
--rw-r--r--   0        0        0     4190 2022-06-17 08:28:29.464166 fastapi-storages-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/fastapi_storages/__init__.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/fastapi_storages/base.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/fastapi_storages/exceptions.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/fastapi_storages/filesystem.py
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/fastapi_storages/s3.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/fastapi_storages/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/fastapi_storages/integrations/__init__.py
+-rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/fastapi_storages/integrations/sqlalchemy.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/README.md
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/PKG-INFO
```

### Comparing `fastapi-storages-0.0.0/LICENSE` & `fastapi_storages-0.1.0/LICENSE.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,9 @@
 MIT License
 
-Copyright © 2022 Tobi DEGNON
+Copyright (c) 2023-present Amin Alaee <me@aminalaee.dev>
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fastapi-storages-0.0.0/README.md` & `fastapi_storages-0.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,88 +1,91 @@
-# Fastapi Storages
+<p align="center">
+<a href="https://github.com/aminalaee/fastapi-storages">
+    <img width="500px" src="https://raw.githubusercontent.com/aminalaee/fastapi-storages/main/docs/assets/images/banner.png" alt"FastAPI_Storages">
+</a>
+</p>
+
+<p align="center">
+<a href="https://github.com/aminalaee/fastapi-storages/actions">
+    <img src="https://github.com/aminalaee/fastapi-storages/workflows/Tests/badge.svg" alt="Build Status">
+</a>
+<a href="https://github.com/aminalaee/fastapi-storages/actions">
+    <img src="https://github.com/aminalaee/fastapi-storages/workflows/Publish/badge.svg" alt="Publish Status">
+</a>
+<a href="https://codecov.io/gh/aminalaee/fastapi-storages">
+    <img src="https://codecov.io/gh/aminalaee/fastapi-storages/branch/main/graph/badge.svg" alt="Coverage">
+</a>
+<a href="https://pypi.org/project/fastapi-storages/">
+    <img src="https://badge.fury.io/py/fastapi-storages.svg" alt="Package version">
+</a>
+<a href="https://pypi.org/project/fastapi-storages" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/fastapi-storages.svg?color=%2334D058" alt="Supported Python versions">
+</a>
+</p>
+
+---
+
+# FastAPI Storages
+
+A collection of backend storages and ORM extensions to simplify file management in FastAPI and Starlette projects.
+
+Similar to `django-storages` project, but aiming to work with a wider range of database ORMs and backends.
 
-Collection of backend storages and orm extensions to simplify file management in fastapi projects. This project
-is inspired by the [django-storages](https://github.com/jschneier/django-storages) packages. If you have  suggestion for a storage backend that is not 
-yet supported, please [open an issue](https://github.com/Tobi-De/fastapi-storages/issues/new) and will discuss it.
+---
 
-[![PyPI](https://img.shields.io/pypi/v/fastapi-storages.svg)][pypi_]
-[![Status](https://img.shields.io/pypi/status/fastapi-storages.svg)][status]
-[![Python Version](https://img.shields.io/pypi/pyversions/fastapi-storages)][python version]
-[![License](https://img.shields.io/pypi/l/fastapi-storages)][license]
+**Documentation**: [https://aminalaee.dev/fastapi-storages](https://aminalaee.dev/fastapi-storages)
 
-[![Read the documentation at https://fastapi-storages.readthedocs.io/](https://img.shields.io/readthedocs/fastapi-storages/latest.svg?label=Read%20the%20Docs)][read the docs]
-[![Tests](https://github.com/Tobi-De/fastapi-storages/workflows/Tests/badge.svg)][tests]
-[![Codecov](https://codecov.io/gh/Tobi-De/fastapi-storages/branch/main/graph/badge.svg)][codecov]
+**Source Code**: [https://github.com/aminalaee/fastapi-storages](https://github.com/aminalaee/fastapi-storages)
 
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
-[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
-
-[pypi_]: https://pypi.org/project/fastapi-storages/
-[status]: https://pypi.org/project/fastapi-storages/
-[python version]: https://pypi.org/project/fastapi-storages
-[read the docs]: https://fastapi-storages.readthedocs.io/
-[tests]: https://github.com/Tobi-De/fastapi-storages/actions?workflow=Tests
-[codecov]: https://app.codecov.io/gh/Tobi-De/fastapi-storages
-[pre-commit]: https://github.com/pre-commit/pre-commit
-[black]: https://github.com/psf/black
-
-
-## Features
-
-### Media storage backend
-
-- [ ] Local
-- [ ] Amazon ses
-- [ ] Google cloud
-- [ ] Deta
-
-### Database extensions
-
-- [ ] Tortoise ORM
-- [ ] RedisOM
-- [ ] Beanie
-- [ ] SQLModel
+---
 
 ## Installation
 
-You can install _Fastapi Storages_ via [pip] from [PyPI]:
-
 ```console
-$ pip install fastapi-storages
+pip install fastapi-storages
+pip install 'fastapi-storages[full]'
 ```
 
-## Quickstart
+## Supported integrations
 
-```python
+- `SQLAlchemy`
+- `SQLModel`
+- `SQLAdmin`
 
-```
+## Supported storage backends
 
-## Contributing
+- `FileSystemStorage`
+- `S3Storage`
 
-Contributions are very welcome.
-To learn more, see the [Contributor Guide].
+## Example
 
-## License
+```python
+from fastapi import FastAPI, UploadFile
+from sqlalchemy import Column, Integer, create_engine
+from sqlalchemy.orm import Session, declarative_base
+from fastapi_storages import FileSystemStorage
+from fastapi_storages.integrations.sqlalchemy import FileType
 
-Distributed under the terms of the [MIT license][license],
-_Fastapi Storages_ is free and open source software.
+app = FastAPI()
+Base = declarative_base()
+engine = create_engine("sqlite:///test.db")
 
-## Issues
 
-If you encounter any problems,
-please [file an issue] along with a detailed description.
+class Example(Base):
+    __tablename__ = "example"
 
-## Credits
+    id = Column(Integer, primary_key=True)
+    file = Column(FileType(storage=FileSystemStorage(path="/tmp")))
 
-This project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.
 
-[@cjolowicz]: https://github.com/cjolowicz
-[pypi]: https://pypi.org/
-[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
-[file an issue]: https://github.com/Tobi-De/fastapi-storages/issues
-[pip]: https://pip.pypa.io/
+# Create database and table
+Base.metadata.create_all(engine)
 
-<!-- github-only -->
 
-[license]: https://github.com/Tobi-De/fastapi-storages/blob/main/LICENSE
-[contributor guide]: https://github.com/Tobi-De/fastapi-storages/blob/main/CONTRIBUTING.md
-[command-line reference]: https://fastapi-storages.readthedocs.io/en/latest/usage.html
+@app.post("/upload/")
+def create_upload_file(file: UploadFile):
+    example = Example(file=file)
+    with Session(engine) as session:
+        session.add(example)
+        session.commit()
+        return {"filename": example.file.name}
+```
```

### Comparing `fastapi-storages-0.0.0/setup.py` & `fastapi_storages-0.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,121 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['fastapi_storages']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['fastapi>=0.78.0']
-
-setup_kwargs = {
-    'name': 'fastapi-storages',
-    'version': '0.0.0',
-    'description': 'Fastapi Storages',
-    'long_description': "# Fastapi Storages\n\nCollection of backend storages and orm extensions to simplify file management in fastapi projects. This project\nis inspired by the [django-storages](https://github.com/jschneier/django-storages) packages. If you have  suggestion for a storage backend that is not \nyet supported, please [open an issue](https://github.com/Tobi-De/fastapi-storages/issues/new) and will discuss it.\n\n[![PyPI](https://img.shields.io/pypi/v/fastapi-storages.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/fastapi-storages.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/fastapi-storages)][python version]\n[![License](https://img.shields.io/pypi/l/fastapi-storages)][license]\n\n[![Read the documentation at https://fastapi-storages.readthedocs.io/](https://img.shields.io/readthedocs/fastapi-storages/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/Tobi-De/fastapi-storages/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/Tobi-De/fastapi-storages/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/fastapi-storages/\n[status]: https://pypi.org/project/fastapi-storages/\n[python version]: https://pypi.org/project/fastapi-storages\n[read the docs]: https://fastapi-storages.readthedocs.io/\n[tests]: https://github.com/Tobi-De/fastapi-storages/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/Tobi-De/fastapi-storages\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n\n## Features\n\n### Media storage backend\n\n- [ ] Local\n- [ ] Amazon ses\n- [ ] Google cloud\n- [ ] Deta\n\n### Database extensions\n\n- [ ] Tortoise ORM\n- [ ] RedisOM\n- [ ] Beanie\n- [ ] SQLModel\n\n## Installation\n\nYou can install _Fastapi Storages_ via [pip] from [PyPI]:\n\n```console\n$ pip install fastapi-storages\n```\n\n## Quickstart\n\n```python\n\n```\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Fastapi Storages_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/Tobi-De/fastapi-storages/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/Tobi-De/fastapi-storages/blob/main/LICENSE\n[contributor guide]: https://github.com/Tobi-De/fastapi-storages/blob/main/CONTRIBUTING.md\n[command-line reference]: https://fastapi-storages.readthedocs.io/en/latest/usage.html\n",
-    'author': 'Tobi DEGNON',
-    'author_email': 'tobidegnon@proton.me',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/Tobi-De/fastapi-storages',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: fastapi-storages
+Version: 0.1.0
+Summary: FastAPI Storages
+Project-URL: Documentation, https://github.com/aminalaee/fastapi-storages#readme
+Project-URL: Issues, https://github.com/aminalaee/fastapi-storages/issues
+Project-URL: Source, https://github.com/aminalaee/fastapi-storages
+Author-email: Amin Alaee <me@aminalaee.dev>
+License-Expression: MIT
+License-File: LICENSE.txt
+Keywords: django,orm,sqlalchemy
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Database
+Classifier: Topic :: Database :: Database Engines/Servers
+Classifier: Topic :: Internet
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Requires-Dist: boto3~=1.25
+Provides-Extra: full
+Requires-Dist: pillow~=9.4; extra == 'full'
+Requires-Dist: sqlalchemy>=1.4; extra == 'full'
+Description-Content-Type: text/markdown
+
+<p align="center">
+<a href="https://github.com/aminalaee/fastapi-storages">
+    <img width="500px" src="https://raw.githubusercontent.com/aminalaee/fastapi-storages/main/docs/assets/images/banner.png" alt"FastAPI_Storages">
+</a>
+</p>
+
+<p align="center">
+<a href="https://github.com/aminalaee/fastapi-storages/actions">
+    <img src="https://github.com/aminalaee/fastapi-storages/workflows/Tests/badge.svg" alt="Build Status">
+</a>
+<a href="https://github.com/aminalaee/fastapi-storages/actions">
+    <img src="https://github.com/aminalaee/fastapi-storages/workflows/Publish/badge.svg" alt="Publish Status">
+</a>
+<a href="https://codecov.io/gh/aminalaee/fastapi-storages">
+    <img src="https://codecov.io/gh/aminalaee/fastapi-storages/branch/main/graph/badge.svg" alt="Coverage">
+</a>
+<a href="https://pypi.org/project/fastapi-storages/">
+    <img src="https://badge.fury.io/py/fastapi-storages.svg" alt="Package version">
+</a>
+<a href="https://pypi.org/project/fastapi-storages" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/fastapi-storages.svg?color=%2334D058" alt="Supported Python versions">
+</a>
+</p>
+
+---
+
+# FastAPI Storages
+
+A collection of backend storages and ORM extensions to simplify file management in FastAPI and Starlette projects.
+
+Similar to `django-storages` project, but aiming to work with a wider range of database ORMs and backends.
+
+---
+
+**Documentation**: [https://aminalaee.dev/fastapi-storages](https://aminalaee.dev/fastapi-storages)
+
+**Source Code**: [https://github.com/aminalaee/fastapi-storages](https://github.com/aminalaee/fastapi-storages)
+
+---
+
+## Installation
+
+```console
+pip install fastapi-storages
+pip install 'fastapi-storages[full]'
+```
+
+## Supported integrations
+
+- `SQLAlchemy`
+- `SQLModel`
+- `SQLAdmin`
+
+## Supported storage backends
+
+- `FileSystemStorage`
+- `S3Storage`
+
+## Example
+
+```python
+from fastapi import FastAPI, UploadFile
+from sqlalchemy import Column, Integer, create_engine
+from sqlalchemy.orm import Session, declarative_base
+from fastapi_storages import FileSystemStorage
+from fastapi_storages.integrations.sqlalchemy import FileType
+
+app = FastAPI()
+Base = declarative_base()
+engine = create_engine("sqlite:///test.db")
+
+
+class Example(Base):
+    __tablename__ = "example"
+
+    id = Column(Integer, primary_key=True)
+    file = Column(FileType(storage=FileSystemStorage(path="/tmp")))
+
+
+# Create database and table
+Base.metadata.create_all(engine)
+
+
+@app.post("/upload/")
+def create_upload_file(file: UploadFile):
+    example = Example(file=file)
+    with Session(engine) as session:
+        session.add(example)
+        session.commit()
+        return {"filename": example.file.name}
+```
```

