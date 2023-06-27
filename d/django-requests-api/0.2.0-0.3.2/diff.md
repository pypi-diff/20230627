# Comparing `tmp/django-requests-api-0.2.0.tar.gz` & `tmp/django-requests-api-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-requests-api-0.2.0.tar", last modified: Wed Jun 21 20:48:22 2023, max compression
+gzip compressed data, was "django-requests-api-0.3.2.tar", last modified: Tue Jun 27 08:30:35 2023, max compression
```

## Comparing `django-requests-api-0.2.0.tar` & `django-requests-api-0.3.2.tar`

### file list

```diff
@@ -1,49 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 20:48:22.465506 django-requests-api-0.2.0/
--rw-rw-rw-   0        0        0      423 2023-06-21 20:48:16.000000 django-requests-api-0.2.0/.bumpversion.cfg
--rw-rw-rw-   0        0        0     1189 2022-12-20 21:47:14.000000 django-requests-api-0.2.0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      100 2021-11-12 13:28:56.000000 django-requests-api-0.2.0/CHANGELOG.rst
--rw-rw-rw-   0        0        0      139 2023-06-20 06:42:54.000000 django-requests-api-0.2.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1135 2023-04-25 19:48:49.000000 django-requests-api-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      336 2023-02-22 09:22:06.000000 django-requests-api-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4304 2023-06-21 20:48:22.465506 django-requests-api-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2738 2023-06-21 20:46:00.000000 django-requests-api-0.2.0/README.md
--rw-rw-rw-   0        0        0     2014 2023-06-20 06:46:10.000000 django-requests-api-0.2.0/mkdocs.yml
--rw-rw-rw-   0        0        0     1644 2023-06-21 20:48:16.000000 django-requests-api-0.2.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-21 20:48:22.432323 django-requests-api-0.2.0/requirements/
--rw-rw-rw-   0        0        0       58 2021-11-12 16:17:16.000000 django-requests-api-0.2.0/requirements/docs.in
--rw-rw-rw-   0        0        0    15726 2022-03-17 16:23:55.000000 django-requests-api-0.2.0/requirements/docs.txt
--rw-rw-rw-   0        0        0     7125 2022-12-20 21:47:14.000000 django-requests-api-0.2.0/requirements/py310-django32.txt
--rw-rw-rw-   0        0        0     6920 2022-12-20 21:47:14.000000 django-requests-api-0.2.0/requirements/py310-django40.txt
--rw-rw-rw-   0        0        0     7125 2022-12-20 21:47:14.000000 django-requests-api-0.2.0/requirements/py311-django32.txt
--rw-rw-rw-   0        0        0     6920 2022-12-20 21:47:14.000000 django-requests-api-0.2.0/requirements/py311-django40.txt
--rw-rw-rw-   0        0        0     7629 2022-12-20 21:47:14.000000 django-requests-api-0.2.0/requirements/py37-django22.txt
--rw-rw-rw-   0        0        0     7861 2022-12-20 21:47:14.000000 django-requests-api-0.2.0/requirements/py37-django32.txt
--rw-rw-rw-   0        0        0     7778 2022-12-20 21:47:14.000000 django-requests-api-0.2.0/requirements/py38-django22.txt
--rw-rw-rw-   0        0        0     7984 2022-12-20 21:47:14.000000 django-requests-api-0.2.0/requirements/py38-django32.txt
--rw-rw-rw-   0        0        0     9406 2022-12-20 21:47:14.000000 django-requests-api-0.2.0/requirements/py38-django40.txt
--rw-rw-rw-   0        0        0     7360 2022-12-20 21:47:14.000000 django-requests-api-0.2.0/requirements/py39-django22.txt
--rw-rw-rw-   0        0        0     7566 2022-12-20 21:47:14.000000 django-requests-api-0.2.0/requirements/py39-django32.txt
--rw-rw-rw-   0        0        0     7361 2022-12-20 21:47:14.000000 django-requests-api-0.2.0/requirements/py39-django40.txt
--rw-rw-rw-   0        0        0       68 2023-06-20 06:48:13.000000 django-requests-api-0.2.0/requirements/requirements.in
--rw-rw-rw-   0        0        0     1608 2021-11-15 15:50:56.000000 django-requests-api-0.2.0/runtests.py
--rw-rw-rw-   0        0        0     1956 2023-06-21 20:48:22.472339 django-requests-api-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      110 2023-06-20 11:24:34.000000 django-requests-api-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 20:48:22.361075 django-requests-api-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-21 20:48:22.448915 django-requests-api-0.2.0/src/django_requests_api.egg-info/
--rw-rw-rw-   0        0        0     4304 2023-06-21 20:48:22.000000 django-requests-api-0.2.0/src/django_requests_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2023-06-21 20:48:22.000000 django-requests-api-0.2.0/src/django_requests_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 20:48:22.000000 django-requests-api-0.2.0/src/django_requests_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-20 11:25:12.000000 django-requests-api-0.2.0/src/django_requests_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       65 2023-06-21 20:48:22.000000 django-requests-api-0.2.0/src/django_requests_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-21 20:48:22.000000 django-requests-api-0.2.0/src/django_requests_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 20:48:22.454771 django-requests-api-0.2.0/src/requests_api/
--rw-rw-rw-   0        0        0      483 2023-06-21 20:48:16.000000 django-requests-api-0.2.0/src/requests_api/__init__.py
--rw-rw-rw-   0        0        0      192 2023-06-21 20:28:55.000000 django-requests-api-0.2.0/src/requests_api/apps.py
--rw-rw-rw-   0        0        0     2062 2023-06-20 06:50:10.000000 django-requests-api-0.2.0/src/requests_api/requests_api.py
-drwxrwxrwx   0        0        0        0 2023-06-21 20:48:22.463554 django-requests-api-0.2.0/tests/
--rw-rw-rw-   0        0        0        0 2020-04-19 11:28:18.000000 django-requests-api-0.2.0/tests/__init__.py
--rw-rw-rw-   0        0        0      398 2023-06-20 06:59:18.000000 django-requests-api-0.2.0/tests/settings.py
--rw-rw-rw-   0        0        0      435 2023-06-20 06:42:54.000000 django-requests-api-0.2.0/tests/test_iubenda.py
--rw-rw-rw-   0        0        0       50 2023-06-20 06:42:54.000000 django-requests-api-0.2.0/tests/urls.py
--rw-rw-rw-   0        0        0       43 2023-06-20 06:42:54.000000 django-requests-api-0.2.0/tests/views.py
--rw-rw-rw-   0        0        0      930 2023-02-04 22:09:32.000000 django-requests-api-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:30:35.966387 django-requests-api-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-27 08:30:35.966387 django-requests-api-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:30:35.966387 django-requests-api-0.3.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)    29679 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15448 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/requirements/py310-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/requirements/py310-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14826 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/requirements/py311-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/requirements/py311-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15880 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/requirements/py38-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/requirements/py38-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15880 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/requirements/py39-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15679 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/requirements/py39-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-27 08:30:35.966387 django-requests-api-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:30:35.962387 django-requests-api-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:30:35.966387 django-requests-api-0.3.2/src/django_requests_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-27 08:30:35.000000 django-requests-api-0.3.2/src/django_requests_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-27 08:30:35.000000 django-requests-api-0.3.2/src/django_requests_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 08:30:35.000000 django-requests-api-0.3.2/src/django_requests_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 08:30:35.000000 django-requests-api-0.3.2/src/django_requests_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 08:30:35.000000 django-requests-api-0.3.2/src/django_requests_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 08:30:35.000000 django-requests-api-0.3.2/src/django_requests_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:30:35.966387 django-requests-api-0.3.2/src/requests_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/src/requests_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/src/requests_api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/src/requests_api/requests_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:30:35.966387 django-requests-api-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/tests/test_requests_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-27 08:30:24.000000 django-requests-api-0.3.2/tox.ini
```

### Comparing `django-requests-api-0.2.0/LICENSE` & `django-requests-api-0.3.2/LICENSE`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2010-present DLRSP (https://dlrsp.org) and other contributors.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2010-present DLRSP (https://dlrsp.org) and other contributors.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `django-requests-api-0.2.0/PKG-INFO` & `django-requests-api-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,96 +1,95 @@
-Metadata-Version: 2.1
-Name: django-requests-api
-Version: 0.2.0
-Summary: Django application to provide simple and shared requests client.
-Home-page: https://github.com/DLRSP/django-requests-api
-Author: DLRSP
-Author-email: dlrsp.dev@gmail.com
-License: MIT License
-Keywords: django,requests,API,privacy,cookie
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-Provides-Extra: linting
-License-File: LICENSE
-
-# django-requests-api [![PyPi license](https://img.shields.io/pypi/l/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-
-[![PyPi status](https://img.shields.io/pypi/status/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-[![PyPi version](https://img.shields.io/pypi/v/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-[![PyPi python version](https://img.shields.io/pypi/pyversions/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-[![PyPi downloads](https://img.shields.io/pypi/dm/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-[![PyPi downloads](https://img.shields.io/pypi/dw/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-[![PyPi downloads](https://img.shields.io/pypi/dd/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-
-## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-requests-api.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-requests-api.svg)
-
-## Test [![codecov.io](https://codecov.io/github/DLRSP/django-requests-api/coverage.svg?branch=master)](https://codecov.io/github/DLRSP/django-requests-api?branch=master) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-requests-api/master.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-requests-api/master) [![gitthub.com](https://github.com/DLRSP/django-requests-api/actions/workflows/ci.yml/badge.svg)](https://github.com/DLRSP/django-requests-api/actions/workflows/ci.yml)
-
-## Check Demo Project
-* Browser the demo app on-line on [Heroku](https://django-requests-api.herokuapp.com/)
-* Check the demo repo on [GitHub](https://github.com/DLRSP/example/tree/django-requests-api)
-
-## Requirements
--   Python 3.7 to 3.10 supported.
--   Django 3.2 to 4.2 supported.
-
-## Setup
-1. Install from **pip**:
-```shell
-pip install django-requests-api
-```
-
-2. Modify `settings.py` by adding the app to `INSTALLED_APPS`:
-```python
-INSTALLED_APPS = (
-    # ...
-    "requests_api",
-    # ...
-)
-```
-
-## Usage
-
-```shell
-from requests_api import RequestsApi
-
-client = RequestsApi("https://api.publicapis.org")
-r = client.get("/entries")
-print(r.json())
-
-github = RequestsApi("https://api.github.com", headers={"Authorization": "token abcdef"})
-r = github.get("/user", headers={"Accept": "application/json"})
-print(r.text)
-```
-
-## Run Example Project
-
-```shell
-git clone --depth=50 --branch=django-requests-api https://github.com/DLRSP/example.git DLRSP/example
-cd DLRSP/example
-python manage.py runserver
-```
-
-Now browser the app @ http://127.0.0.1:8000
+Metadata-Version: 2.1
+Name: django-requests-api
+Version: 0.3.2
+Summary: Django application to provide simple and shared requests client.
+Home-page: https://github.com/DLRSP/django-requests-api
+Author: DLRSP
+Author-email: dlrsp.dev@gmail.com
+License: MIT License
+Keywords: django,requests,API,privacy,cookie
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+Provides-Extra: linting
+License-File: LICENSE
+
+# django-requests-api [![PyPi license](https://img.shields.io/pypi/l/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+
+[![PyPi status](https://img.shields.io/pypi/status/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+[![PyPi version](https://img.shields.io/pypi/v/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+[![PyPi python version](https://img.shields.io/pypi/pyversions/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+[![PyPi downloads](https://img.shields.io/pypi/dm/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+[![PyPi downloads](https://img.shields.io/pypi/dw/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+[![PyPi downloads](https://img.shields.io/pypi/dd/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+
+## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-requests-api.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-requests-api.svg)
+
+## Test [![codecov.io](https://codecov.io/github/DLRSP/django-requests-api/coverage.svg?branch=master)](https://codecov.io/github/DLRSP/django-requests-api?branch=master) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-requests-api/master.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-requests-api/master) [![gitthub.com](https://github.com/DLRSP/django-requests-api/actions/workflows/ci.yml/badge.svg)](https://github.com/DLRSP/django-requests-api/actions/workflows/ci.yml)
+
+## Check Demo Project
+* Browser the demo app on-line on [Heroku](https://django-requests-api.herokuapp.com/)
+* Check the demo repo on [GitHub](https://github.com/DLRSP/example/tree/django-requests-api)
+
+## Requirements
+-   Python 3.8+ supported.
+-   Django 3.2+ supported.
+
+## Setup
+1. Install from **pip**:
+```shell
+pip install django-requests-api
+```
+
+2. Modify `settings.py` by adding the app to `INSTALLED_APPS`:
+```python
+INSTALLED_APPS = (
+    # ...
+    "requests_api",
+    # ...
+)
+```
+
+## Usage
+
+```shell
+from requests_api import RequestsApi
+
+client = RequestsApi("https://api.publicapis.org")
+r = client.get("/entries")
+print(r.json())
+
+github = RequestsApi("https://api.github.com", headers={"Authorization": "token abcdef"})
+r = github.get("/user", headers={"Accept": "application/json"})
+print(r.text)
+```
+
+## Run Example Project
+
+```shell
+git clone --depth=50 --branch=django-requests-api https://github.com/DLRSP/example.git DLRSP/example
+cd DLRSP/example
+python manage.py runserver
+```
+
+Now browser the app @ http://127.0.0.1:8000
```

### Comparing `django-requests-api-0.2.0/README.md` & `django-requests-api-0.3.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-# django-requests-api [![PyPi license](https://img.shields.io/pypi/l/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-
-[![PyPi status](https://img.shields.io/pypi/status/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-[![PyPi version](https://img.shields.io/pypi/v/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-[![PyPi python version](https://img.shields.io/pypi/pyversions/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-[![PyPi downloads](https://img.shields.io/pypi/dm/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-[![PyPi downloads](https://img.shields.io/pypi/dw/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-[![PyPi downloads](https://img.shields.io/pypi/dd/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-
-## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-requests-api.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-requests-api.svg)
-
-## Test [![codecov.io](https://codecov.io/github/DLRSP/django-requests-api/coverage.svg?branch=master)](https://codecov.io/github/DLRSP/django-requests-api?branch=master) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-requests-api/master.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-requests-api/master) [![gitthub.com](https://github.com/DLRSP/django-requests-api/actions/workflows/ci.yml/badge.svg)](https://github.com/DLRSP/django-requests-api/actions/workflows/ci.yml)
-
-## Check Demo Project
-* Browser the demo app on-line on [Heroku](https://django-requests-api.herokuapp.com/)
-* Check the demo repo on [GitHub](https://github.com/DLRSP/example/tree/django-requests-api)
-
-## Requirements
--   Python 3.7 to 3.10 supported.
--   Django 3.2 to 4.2 supported.
-
-## Setup
-1. Install from **pip**:
-```shell
-pip install django-requests-api
-```
-
-2. Modify `settings.py` by adding the app to `INSTALLED_APPS`:
-```python
-INSTALLED_APPS = (
-    # ...
-    "requests_api",
-    # ...
-)
-```
-
-## Usage
-
-```shell
-from requests_api import RequestsApi
-
-client = RequestsApi("https://api.publicapis.org")
-r = client.get("/entries")
-print(r.json())
-
-github = RequestsApi("https://api.github.com", headers={"Authorization": "token abcdef"})
-r = github.get("/user", headers={"Accept": "application/json"})
-print(r.text)
-```
-
-## Run Example Project
-
-```shell
-git clone --depth=50 --branch=django-requests-api https://github.com/DLRSP/example.git DLRSP/example
-cd DLRSP/example
-python manage.py runserver
-```
-
-Now browser the app @ http://127.0.0.1:8000
+# django-requests-api [![PyPi license](https://img.shields.io/pypi/l/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+
+[![PyPi status](https://img.shields.io/pypi/status/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+[![PyPi version](https://img.shields.io/pypi/v/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+[![PyPi python version](https://img.shields.io/pypi/pyversions/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+[![PyPi downloads](https://img.shields.io/pypi/dm/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+[![PyPi downloads](https://img.shields.io/pypi/dw/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+[![PyPi downloads](https://img.shields.io/pypi/dd/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+
+## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-requests-api.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-requests-api.svg)
+
+## Test [![codecov.io](https://codecov.io/github/DLRSP/django-requests-api/coverage.svg?branch=master)](https://codecov.io/github/DLRSP/django-requests-api?branch=master) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-requests-api/master.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-requests-api/master) [![gitthub.com](https://github.com/DLRSP/django-requests-api/actions/workflows/ci.yml/badge.svg)](https://github.com/DLRSP/django-requests-api/actions/workflows/ci.yml)
+
+## Check Demo Project
+* Browser the demo app on-line on [Heroku](https://django-requests-api.herokuapp.com/)
+* Check the demo repo on [GitHub](https://github.com/DLRSP/example/tree/django-requests-api)
+
+## Requirements
+-   Python 3.8+ supported.
+-   Django 3.2+ supported.
+
+## Setup
+1. Install from **pip**:
+```shell
+pip install django-requests-api
+```
+
+2. Modify `settings.py` by adding the app to `INSTALLED_APPS`:
+```python
+INSTALLED_APPS = (
+    # ...
+    "requests_api",
+    # ...
+)
+```
+
+## Usage
+
+```shell
+from requests_api import RequestsApi
+
+client = RequestsApi("https://api.publicapis.org")
+r = client.get("/entries")
+print(r.json())
+
+github = RequestsApi("https://api.github.com", headers={"Authorization": "token abcdef"})
+r = github.get("/user", headers={"Accept": "application/json"})
+print(r.text)
+```
+
+## Run Example Project
+
+```shell
+git clone --depth=50 --branch=django-requests-api https://github.com/DLRSP/example.git DLRSP/example
+cd DLRSP/example
+python manage.py runserver
+```
+
+Now browser the app @ http://127.0.0.1:8000
```

### Comparing `django-requests-api-0.2.0/pyproject.toml` & `django-requests-api-0.3.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-[build-system]
-requires = ["setuptools >= 40.8.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[tool.black]
-target-version = ['py310']
-
-[tool.isort]
-profile = "black"
-
-[tool.mypy]
-check_untyped_defs = true
-disallow_any_generics = true
-disallow_incomplete_defs = true
-disallow_untyped_defs = true
-mypy_path = "src/"
-no_implicit_optional = true
-show_error_codes = true
-warn_unreachable = true
-warn_unused_ignores = true
-
-[[tool.mypy.overrides]]
-module = "tests.*"
-allow_untyped_defs = true
-
-[tool.pytest.ini_options]
-addopts = """\
-    --strict-config
-    --strict-markers
-    --ds=tests.settings
-    """
-django_find_project = false
-
-[tool.towncrier]
-package = "requests_api"
-package_dir = "src"
-filename = "CHANGELOG.rst"
-directory = "news/"
-version = "0.2.0"
-
-# For rendering properly for this project
-issue_format = "`#{issue} <https://github.com/DLRSP/django-requests-api/issues/{issue}>`_"
-# template = "tools/news/template.rst"
-
-# Grouping of entries, within our changelog
-type = [
-  { name = "Process",                   directory = "process", showcontent = true },
-  { name = "Deprecations and Removals", directory = "removal", showcontent = true },
-  { name = "Features",                  directory = "feature", showcontent = true },
-  { name = "Bug Fixes",                 directory = "bugfix",  showcontent = true },
-  { name = "Vendored Libraries",        directory = "vendor",  showcontent = true },
-  { name = "Improved Documentation",    directory = "doc",     showcontent = true },
-  { name = "Trivial Changes",           directory = "trivial", showcontent = false },
-]
+[build-system]
+requires = ["setuptools >= 40.8.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[tool.black]
+target-version = ['py310']
+
+[tool.isort]
+profile = "black"
+
+[tool.mypy]
+check_untyped_defs = true
+disallow_any_generics = true
+disallow_incomplete_defs = true
+disallow_untyped_defs = true
+mypy_path = "src/"
+no_implicit_optional = true
+show_error_codes = true
+warn_unreachable = true
+warn_unused_ignores = true
+
+[[tool.mypy.overrides]]
+module = "tests.*"
+allow_untyped_defs = true
+
+[tool.pytest.ini_options]
+addopts = """\
+    --strict-config
+    --strict-markers
+    --ds=tests.settings
+    """
+django_find_project = false
+
+[tool.towncrier]
+package = "requests_api"
+package_dir = "src"
+filename = "CHANGELOG.rst"
+directory = "news/"
+version = "0.3.2"
+
+# For rendering properly for this project
+issue_format = "`#{issue} <https://github.com/DLRSP/django-requests-api/issues/{issue}>`_"
+# template = "tools/news/template.rst"
+
+# Grouping of entries, within our changelog
+type = [
+  { name = "Process",                   directory = "process", showcontent = true },
+  { name = "Deprecations and Removals", directory = "removal", showcontent = true },
+  { name = "Features",                  directory = "feature", showcontent = true },
+  { name = "Bug Fixes",                 directory = "bugfix",  showcontent = true },
+  { name = "Vendored Libraries",        directory = "vendor",  showcontent = true },
+  { name = "Improved Documentation",    directory = "doc",     showcontent = true },
+  { name = "Trivial Changes",           directory = "trivial", showcontent = false },
+]
```

### Comparing `django-requests-api-0.2.0/requirements/docs.txt` & `django-requests-api-0.3.2/requirements/py38-django32.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,231 +1,224 @@
-#
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
-#
-#    pip-compile --allow-unsafe --generate-hashes --output-file=docs.txt docs.in
-#
-click==8.0.3 \
-    --hash=sha256:353f466495adaeb40b6b5f592f9f91cb22372351c84caeb068132442a4518ef3 \
-    --hash=sha256:410e932b050f5eed773c4cda94de75971c89cdb3155a72a0831139a79e5ecb5b
-    # via mkdocs
-ghp-import==2.0.2 \
-    --hash=sha256:5f8962b30b20652cdffa9c5a9812f7de6bcb56ec475acac579807719bf242c46 \
-    --hash=sha256:947b3771f11be850c852c64b561c600fdddf794bab363060854c1ee7ad05e071
-    # via mkdocs
-gitdb==4.0.9 \
-    --hash=sha256:8033ad4e853066ba6ca92050b9df2f89301b8fc8bf7e9324d412a63f8bf1a8fd \
-    --hash=sha256:bac2fd45c0a1c9cf619e63a90d62bdc63892ef92387424b855792a6cabe789aa
-    # via gitpython
-gitpython==3.1.24 \
-    --hash=sha256:dc0a7f2f697657acc8d7f89033e8b1ea94dd90356b2983bca89dc8d2ab3cc647 \
-    --hash=sha256:df83fdf5e684fef7c6ee2c02fc68a5ceb7e7e759d08b694088d0cacb4eba59e5
-    # via mkdocs-git-revision-date-plugin
-importlib-metadata==4.8.2 \
-    --hash=sha256:53ccfd5c134223e497627b9815d5030edf77d2ed573922f7a0b8f8bb81a1c100 \
-    --hash=sha256:75bdec14c397f528724c1bfd9709d660b33a4d2e77387a3358f20b848bb5e5fb
-    # via mkdocs
-jinja2==3.0.3 \
-    --hash=sha256:077ce6014f7b40d03b47d1f1ca4b0fc8328a692bd284016f806ed0eaca390ad8 \
-    --hash=sha256:611bb273cd68f3b993fabdc4064fc858c5b47a973cb5aa7999ec1ba405c87cd7
-    # via
-    #   mkdocs
-    #   mkdocs-git-revision-date-plugin
-    #   mkdocs-material
-markdown==3.3.4 \
-    --hash=sha256:31b5b491868dcc87d6c24b7e3d19a0d730d59d3e46f4eea6430a321bed387a49 \
-    --hash=sha256:96c3ba1261de2f7547b46a00ea8463832c921d3f9d6aba3f255a6f71386db20c
-    # via
-    #   mkdocs
-    #   mkdocs-material
-    #   pymdown-extensions
-markupsafe==2.0.1 \
-    --hash=sha256:01a9b8ea66f1658938f65b93a85ebe8bc016e6769611be228d797c9d998dd298 \
-    --hash=sha256:023cb26ec21ece8dc3907c0e8320058b2e0cb3c55cf9564da612bc325bed5e64 \
-    --hash=sha256:0446679737af14f45767963a1a9ef7620189912317d095f2d9ffa183a4d25d2b \
-    --hash=sha256:04635854b943835a6ea959e948d19dcd311762c5c0c6e1f0e16ee57022669194 \
-    --hash=sha256:0717a7390a68be14b8c793ba258e075c6f4ca819f15edfc2a3a027c823718567 \
-    --hash=sha256:0955295dd5eec6cb6cc2fe1698f4c6d84af2e92de33fbcac4111913cd100a6ff \
-    --hash=sha256:0d4b31cc67ab36e3392bbf3862cfbadac3db12bdd8b02a2731f509ed5b829724 \
-    --hash=sha256:10f82115e21dc0dfec9ab5c0223652f7197feb168c940f3ef61563fc2d6beb74 \
-    --hash=sha256:168cd0a3642de83558a5153c8bd34f175a9a6e7f6dc6384b9655d2697312a646 \
-    --hash=sha256:1d609f577dc6e1aa17d746f8bd3c31aa4d258f4070d61b2aa5c4166c1539de35 \
-    --hash=sha256:1f2ade76b9903f39aa442b4aadd2177decb66525062db244b35d71d0ee8599b6 \
-    --hash=sha256:20dca64a3ef2d6e4d5d615a3fd418ad3bde77a47ec8a23d984a12b5b4c74491a \
-    --hash=sha256:2a7d351cbd8cfeb19ca00de495e224dea7e7d919659c2841bbb7f420ad03e2d6 \
-    --hash=sha256:2d7d807855b419fc2ed3e631034685db6079889a1f01d5d9dac950f764da3dad \
-    --hash=sha256:2ef54abee730b502252bcdf31b10dacb0a416229b72c18b19e24a4509f273d26 \
-    --hash=sha256:36bc903cbb393720fad60fc28c10de6acf10dc6cc883f3e24ee4012371399a38 \
-    --hash=sha256:37205cac2a79194e3750b0af2a5720d95f786a55ce7df90c3af697bfa100eaac \
-    --hash=sha256:3c112550557578c26af18a1ccc9e090bfe03832ae994343cfdacd287db6a6ae7 \
-    --hash=sha256:3dd007d54ee88b46be476e293f48c85048603f5f516008bee124ddd891398ed6 \
-    --hash=sha256:4296f2b1ce8c86a6aea78613c34bb1a672ea0e3de9c6ba08a960efe0b0a09047 \
-    --hash=sha256:47ab1e7b91c098ab893b828deafa1203de86d0bc6ab587b160f78fe6c4011f75 \
-    --hash=sha256:49e3ceeabbfb9d66c3aef5af3a60cc43b85c33df25ce03d0031a608b0a8b2e3f \
-    --hash=sha256:4dc8f9fb58f7364b63fd9f85013b780ef83c11857ae79f2feda41e270468dd9b \
-    --hash=sha256:4efca8f86c54b22348a5467704e3fec767b2db12fc39c6d963168ab1d3fc9135 \
-    --hash=sha256:53edb4da6925ad13c07b6d26c2a852bd81e364f95301c66e930ab2aef5b5ddd8 \
-    --hash=sha256:5855f8438a7d1d458206a2466bf82b0f104a3724bf96a1c781ab731e4201731a \
-    --hash=sha256:594c67807fb16238b30c44bdf74f36c02cdf22d1c8cda91ef8a0ed8dabf5620a \
-    --hash=sha256:5b6d930f030f8ed98e3e6c98ffa0652bdb82601e7a016ec2ab5d7ff23baa78d1 \
-    --hash=sha256:5bb28c636d87e840583ee3adeb78172efc47c8b26127267f54a9c0ec251d41a9 \
-    --hash=sha256:60bf42e36abfaf9aff1f50f52644b336d4f0a3fd6d8a60ca0d054ac9f713a864 \
-    --hash=sha256:611d1ad9a4288cf3e3c16014564df047fe08410e628f89805e475368bd304914 \
-    --hash=sha256:6300b8454aa6930a24b9618fbb54b5a68135092bc666f7b06901f897fa5c2fee \
-    --hash=sha256:63f3268ba69ace99cab4e3e3b5840b03340efed0948ab8f78d2fd87ee5442a4f \
-    --hash=sha256:6557b31b5e2c9ddf0de32a691f2312a32f77cd7681d8af66c2692efdbef84c18 \
-    --hash=sha256:693ce3f9e70a6cf7d2fb9e6c9d8b204b6b39897a2c4a1aa65728d5ac97dcc1d8 \
-    --hash=sha256:6a7fae0dd14cf60ad5ff42baa2e95727c3d81ded453457771d02b7d2b3f9c0c2 \
-    --hash=sha256:6c4ca60fa24e85fe25b912b01e62cb969d69a23a5d5867682dd3e80b5b02581d \
-    --hash=sha256:6fcf051089389abe060c9cd7caa212c707e58153afa2c649f00346ce6d260f1b \
-    --hash=sha256:7d91275b0245b1da4d4cfa07e0faedd5b0812efc15b702576d103293e252af1b \
-    --hash=sha256:89c687013cb1cd489a0f0ac24febe8c7a666e6e221b783e53ac50ebf68e45d86 \
-    --hash=sha256:8d206346619592c6200148b01a2142798c989edcb9c896f9ac9722a99d4e77e6 \
-    --hash=sha256:905fec760bd2fa1388bb5b489ee8ee5f7291d692638ea5f67982d968366bef9f \
-    --hash=sha256:97383d78eb34da7e1fa37dd273c20ad4320929af65d156e35a5e2d89566d9dfb \
-    --hash=sha256:984d76483eb32f1bcb536dc27e4ad56bba4baa70be32fa87152832cdd9db0833 \
-    --hash=sha256:99df47edb6bda1249d3e80fdabb1dab8c08ef3975f69aed437cb69d0a5de1e28 \
-    --hash=sha256:9f02365d4e99430a12647f09b6cc8bab61a6564363f313126f775eb4f6ef798e \
-    --hash=sha256:a30e67a65b53ea0a5e62fe23682cfe22712e01f453b95233b25502f7c61cb415 \
-    --hash=sha256:ab3ef638ace319fa26553db0624c4699e31a28bb2a835c5faca8f8acf6a5a902 \
-    --hash=sha256:aca6377c0cb8a8253e493c6b451565ac77e98c2951c45f913e0b52facdcff83f \
-    --hash=sha256:add36cb2dbb8b736611303cd3bfcee00afd96471b09cda130da3581cbdc56a6d \
-    --hash=sha256:b2f4bf27480f5e5e8ce285a8c8fd176c0b03e93dcc6646477d4630e83440c6a9 \
-    --hash=sha256:b7f2d075102dc8c794cbde1947378051c4e5180d52d276987b8d28a3bd58c17d \
-    --hash=sha256:baa1a4e8f868845af802979fcdbf0bb11f94f1cb7ced4c4b8a351bb60d108145 \
-    --hash=sha256:be98f628055368795d818ebf93da628541e10b75b41c559fdf36d104c5787066 \
-    --hash=sha256:bf5d821ffabf0ef3533c39c518f3357b171a1651c1ff6827325e4489b0e46c3c \
-    --hash=sha256:c47adbc92fc1bb2b3274c4b3a43ae0e4573d9fbff4f54cd484555edbf030baf1 \
-    --hash=sha256:cdfba22ea2f0029c9261a4bd07e830a8da012291fbe44dc794e488b6c9bb353a \
-    --hash=sha256:d6c7ebd4e944c85e2c3421e612a7057a2f48d478d79e61800d81468a8d842207 \
-    --hash=sha256:d7f9850398e85aba693bb640262d3611788b1f29a79f0c93c565694658f4071f \
-    --hash=sha256:d8446c54dc28c01e5a2dbac5a25f071f6653e6e40f3a8818e8b45d790fe6ef53 \
-    --hash=sha256:deb993cacb280823246a026e3b2d81c493c53de6acfd5e6bfe31ab3402bb37dd \
-    --hash=sha256:e0f138900af21926a02425cf736db95be9f4af72ba1bb21453432a07f6082134 \
-    --hash=sha256:e9936f0b261d4df76ad22f8fee3ae83b60d7c3e871292cd42f40b81b70afae85 \
-    --hash=sha256:f0567c4dc99f264f49fe27da5f735f414c4e7e7dd850cfd8e69f0862d7c74ea9 \
-    --hash=sha256:f5653a225f31e113b152e56f154ccbe59eeb1c7487b39b9d9f9cdb58e6c79dc5 \
-    --hash=sha256:f826e31d18b516f653fe296d967d700fddad5901ae07c622bb3705955e1faa94 \
-    --hash=sha256:f8ba0e8349a38d3001fae7eadded3f6606f0da5d748ee53cc1dab1d6527b9509 \
-    --hash=sha256:f9081981fe268bd86831e5c75f7de206ef275defcb82bc70740ae6dc507aee51 \
-    --hash=sha256:fa130dd50c57d53368c9d59395cb5526eda596d3ffe36666cd81a44d56e48872
-    # via jinja2
-mergedeep==1.3.4 \
-    --hash=sha256:0096d52e9dad9939c3d975a774666af186eda617e6ca84df4c94dec30004f2a8 \
-    --hash=sha256:70775750742b25c0d8f36c55aed03d24c3384d17c951b3175d898bd778ef0307
-    # via mkdocs
-mkdocs==1.2.3 \
-    --hash=sha256:89f5a094764381cda656af4298727c9f53dc3e602983087e1fe96ea1df24f4c1 \
-    --hash=sha256:a1fa8c2d0c1305d7fc2b9d9f607c71778572a8b110fb26642aa00296c9e6d072
-    # via
-    #   -r requirements/docs.in
-    #   mkdocs-git-revision-date-plugin
-    #   mkdocs-material
-mkdocs-git-revision-date-plugin==0.3.2 \
-    --hash=sha256:2e67956cb01823dd2418e2833f3623dee8604cdf223bddd005fe36226a56f6ef
-    # via -r requirements/docs.in
-mkdocs-material==8.2.5 \
-    --hash=sha256:95283c6af633809f32ba688fcf9bce4604af320e188d3e26fcb40d0e5ab9b823 \
-    --hash=sha256:cdfb39edc77f5c2bbfca02b4fc3764de38b2093eff121aed37674204439901ce
-    # via -r requirements/docs.in
-mkdocs-material-extensions==1.0.3 \
-    --hash=sha256:a82b70e533ce060b2a5d9eb2bc2e1be201cf61f901f93704b4acf6e3d5983a44 \
-    --hash=sha256:bfd24dfdef7b41c312ede42648f9eb83476ea168ec163b613f9abd12bbfddba2
-    # via mkdocs-material
-packaging==21.2 \
-    --hash=sha256:096d689d78ca690e4cd8a89568ba06d07ca097e3306a4381635073ca91479966 \
-    --hash=sha256:14317396d1e8cdb122989b916fa2c7e9ca8e2be9e8060a6eff75b6b7b4d8a7e0
-    # via mkdocs
-pygments==2.10.0 \
-    --hash=sha256:b8e67fe6af78f492b3c4b3e2970c0624cbf08beb1e493b2c99b9fa1b67a20380 \
-    --hash=sha256:f398865f7eb6874156579fdf36bc840a03cab64d1cde9e93d68f46a425ec52c6
-    # via mkdocs-material
-pymdown-extensions==9.0 \
-    --hash=sha256:01e4bec7f4b16beaba0087a74496401cf11afd69e3a11fe95cb593e5c698ef40 \
-    --hash=sha256:430cc2fbb30cef2df70edac0b4f62614a6a4d2b06462e32da4ca96098b7c1dfb
-    # via mkdocs-material
-pyparsing==2.4.7 \
-    --hash=sha256:c203ec8783bf771a155b207279b9bccb8dea02d8f0c9e5f8ead507bc3246ecc1 \
-    --hash=sha256:ef9d7589ef3c200abe66653d3f1ab1033c3c419ae9b9bdb1240a85b024efc88b
-    # via packaging
-python-dateutil==2.8.2 \
-    --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
-    --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
-    # via ghp-import
-pyyaml==6.0 \
-    --hash=sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293 \
-    --hash=sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b \
-    --hash=sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57 \
-    --hash=sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b \
-    --hash=sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4 \
-    --hash=sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07 \
-    --hash=sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba \
-    --hash=sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9 \
-    --hash=sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287 \
-    --hash=sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513 \
-    --hash=sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0 \
-    --hash=sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0 \
-    --hash=sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92 \
-    --hash=sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f \
-    --hash=sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2 \
-    --hash=sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc \
-    --hash=sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c \
-    --hash=sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86 \
-    --hash=sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4 \
-    --hash=sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c \
-    --hash=sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34 \
-    --hash=sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b \
-    --hash=sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c \
-    --hash=sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb \
-    --hash=sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737 \
-    --hash=sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3 \
-    --hash=sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d \
-    --hash=sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53 \
-    --hash=sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78 \
-    --hash=sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803 \
-    --hash=sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a \
-    --hash=sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174 \
-    --hash=sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5
-    # via
-    #   mkdocs
-    #   pyyaml-env-tag
-pyyaml-env-tag==0.1 \
-    --hash=sha256:70092675bda14fdec33b31ba77e7543de9ddc88f2e5b99160396572d11525bdb \
-    --hash=sha256:af31106dec8a4d68c60207c1886031cbf839b68aa7abccdb19868200532c2069
-    # via mkdocs
-six==1.16.0 \
-    --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
-    --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
-    # via python-dateutil
-smmap==5.0.0 \
-    --hash=sha256:2aba19d6a040e78d8b09de5c57e96207b09ed71d8e55ce0959eeee6c8e190d94 \
-    --hash=sha256:c840e62059cd3be204b0c9c9f74be2c09d5648eddd4580d9314c3ecde0b30936
-    # via gitdb
-watchdog==2.1.6 \
-    --hash=sha256:25fb5240b195d17de949588628fdf93032ebf163524ef08933db0ea1f99bd685 \
-    --hash=sha256:3386b367e950a11b0568062b70cc026c6f645428a698d33d39e013aaeda4cc04 \
-    --hash=sha256:3becdb380d8916c873ad512f1701f8a92ce79ec6978ffde92919fd18d41da7fb \
-    --hash=sha256:4ae38bf8ba6f39d5b83f78661273216e7db5b00f08be7592062cb1fc8b8ba542 \
-    --hash=sha256:8047da932432aa32c515ec1447ea79ce578d0559362ca3605f8e9568f844e3c6 \
-    --hash=sha256:8f1c00aa35f504197561060ca4c21d3cc079ba29cf6dd2fe61024c70160c990b \
-    --hash=sha256:922a69fa533cb0c793b483becaaa0845f655151e7256ec73630a1b2e9ebcb660 \
-    --hash=sha256:9693f35162dc6208d10b10ddf0458cc09ad70c30ba689d9206e02cd836ce28a3 \
-    --hash=sha256:a0f1c7edf116a12f7245be06120b1852275f9506a7d90227648b250755a03923 \
-    --hash=sha256:a36e75df6c767cbf46f61a91c70b3ba71811dfa0aca4a324d9407a06a8b7a2e7 \
-    --hash=sha256:aba5c812f8ee8a3ff3be51887ca2d55fb8e268439ed44110d3846e4229eb0e8b \
-    --hash=sha256:ad6f1796e37db2223d2a3f302f586f74c72c630b48a9872c1e7ae8e92e0ab669 \
-    --hash=sha256:ae67501c95606072aafa865b6ed47343ac6484472a2f95490ba151f6347acfc2 \
-    --hash=sha256:b2fcf9402fde2672545b139694284dc3b665fd1be660d73eca6805197ef776a3 \
-    --hash=sha256:b52b88021b9541a60531142b0a451baca08d28b74a723d0c99b13c8c8d48d604 \
-    --hash=sha256:b7d336912853d7b77f9b2c24eeed6a5065d0a0cc0d3b6a5a45ad6d1d05fb8cd8 \
-    --hash=sha256:bd9ba4f332cf57b2c1f698be0728c020399ef3040577cde2939f2e045b39c1e5 \
-    --hash=sha256:be9be735f827820a06340dff2ddea1fb7234561fa5e6300a62fe7f54d40546a0 \
-    --hash=sha256:cca7741c0fcc765568350cb139e92b7f9f3c9a08c4f32591d18ab0a6ac9e71b6 \
-    --hash=sha256:d0d19fb2441947b58fbf91336638c2b9f4cc98e05e1045404d7a4cb7cddc7a65 \
-    --hash=sha256:e02794ac791662a5eafc6ffeaf9bcc149035a0e48eb0a9d40a8feb4622605a3d \
-    --hash=sha256:e0f30db709c939cabf64a6dc5babb276e6d823fd84464ab916f9b9ba5623ca15 \
-    --hash=sha256:e92c2d33858c8f560671b448205a268096e17870dcf60a9bb3ac7bfbafb7f5f9
-    # via mkdocs
-zipp==3.6.0 \
-    --hash=sha256:71c644c5369f4a6e07636f0aa966270449561fcea2e3d6747b8d23efaa9d7832 \
-    --hash=sha256:9fe5ea21568a0a70e50f273397638d39b03353731e6cbbb3fd8502a33fec40bc
-    # via importlib-metadata
+#
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
+#
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py38-django32.txt requirements/requirements.in
+#
+asgiref==3.7.2 \
+    --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
+    --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
+    # via django
+certifi==2023.5.7 \
+    --hash=sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7 \
+    --hash=sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716
+    # via requests
+charset-normalizer==3.1.0 \
+    --hash=sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6 \
+    --hash=sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1 \
+    --hash=sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e \
+    --hash=sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373 \
+    --hash=sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62 \
+    --hash=sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230 \
+    --hash=sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be \
+    --hash=sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c \
+    --hash=sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0 \
+    --hash=sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448 \
+    --hash=sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f \
+    --hash=sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649 \
+    --hash=sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d \
+    --hash=sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0 \
+    --hash=sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706 \
+    --hash=sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a \
+    --hash=sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59 \
+    --hash=sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23 \
+    --hash=sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5 \
+    --hash=sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb \
+    --hash=sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e \
+    --hash=sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e \
+    --hash=sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c \
+    --hash=sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28 \
+    --hash=sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d \
+    --hash=sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41 \
+    --hash=sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974 \
+    --hash=sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce \
+    --hash=sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f \
+    --hash=sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1 \
+    --hash=sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d \
+    --hash=sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8 \
+    --hash=sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017 \
+    --hash=sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31 \
+    --hash=sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7 \
+    --hash=sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8 \
+    --hash=sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e \
+    --hash=sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14 \
+    --hash=sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd \
+    --hash=sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d \
+    --hash=sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795 \
+    --hash=sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b \
+    --hash=sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b \
+    --hash=sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b \
+    --hash=sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203 \
+    --hash=sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f \
+    --hash=sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19 \
+    --hash=sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1 \
+    --hash=sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a \
+    --hash=sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac \
+    --hash=sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9 \
+    --hash=sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0 \
+    --hash=sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137 \
+    --hash=sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f \
+    --hash=sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6 \
+    --hash=sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5 \
+    --hash=sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909 \
+    --hash=sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f \
+    --hash=sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0 \
+    --hash=sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324 \
+    --hash=sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755 \
+    --hash=sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb \
+    --hash=sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854 \
+    --hash=sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c \
+    --hash=sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60 \
+    --hash=sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84 \
+    --hash=sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0 \
+    --hash=sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b \
+    --hash=sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1 \
+    --hash=sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531 \
+    --hash=sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1 \
+    --hash=sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11 \
+    --hash=sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326 \
+    --hash=sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df \
+    --hash=sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab
+    # via requests
+coverage==7.2.7 \
+    --hash=sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f \
+    --hash=sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2 \
+    --hash=sha256:0a5f9e1dbd7fbe30196578ca36f3fba75376fb99888c395c5880b355e2875f8a \
+    --hash=sha256:0e1f928eaf5469c11e886fe0885ad2bf1ec606434e79842a879277895a50942a \
+    --hash=sha256:171717c7cb6b453aebac9a2ef603699da237f341b38eebfee9be75d27dc38e01 \
+    --hash=sha256:1e9d683426464e4a252bf70c3498756055016f99ddaec3774bf368e76bbe02b6 \
+    --hash=sha256:201e7389591af40950a6480bd9edfa8ed04346ff80002cec1a66cac4549c1ad7 \
+    --hash=sha256:245167dd26180ab4c91d5e1496a30be4cd721a5cf2abf52974f965f10f11419f \
+    --hash=sha256:2aee274c46590717f38ae5e4650988d1af340fe06167546cc32fe2f58ed05b02 \
+    --hash=sha256:2e07b54284e381531c87f785f613b833569c14ecacdcb85d56b25c4622c16c3c \
+    --hash=sha256:31563e97dae5598556600466ad9beea39fb04e0229e61c12eaa206e0aa202063 \
+    --hash=sha256:33d6d3ea29d5b3a1a632b3c4e4f4ecae24ef170b0b9ee493883f2df10039959a \
+    --hash=sha256:3d376df58cc111dc8e21e3b6e24606b5bb5dee6024f46a5abca99124b2229ef5 \
+    --hash=sha256:419bfd2caae268623dd469eff96d510a920c90928b60f2073d79f8fe2bbc5959 \
+    --hash=sha256:48c19d2159d433ccc99e729ceae7d5293fbffa0bdb94952d3579983d1c8c9d97 \
+    --hash=sha256:49969a9f7ffa086d973d91cec8d2e31080436ef0fb4a359cae927e742abfaaa6 \
+    --hash=sha256:52edc1a60c0d34afa421c9c37078817b2e67a392cab17d97283b64c5833f427f \
+    --hash=sha256:537891ae8ce59ef63d0123f7ac9e2ae0fc8b72c7ccbe5296fec45fd68967b6c9 \
+    --hash=sha256:54b896376ab563bd38453cecb813c295cf347cf5906e8b41d340b0321a5433e5 \
+    --hash=sha256:58c2ccc2f00ecb51253cbe5d8d7122a34590fac9646a960d1430d5b15321d95f \
+    --hash=sha256:5b7540161790b2f28143191f5f8ec02fb132660ff175b7747b95dcb77ac26562 \
+    --hash=sha256:5baa06420f837184130752b7c5ea0808762083bf3487b5038d68b012e5937dbe \
+    --hash=sha256:5e330fc79bd7207e46c7d7fd2bb4af2963f5f635703925543a70b99574b0fea9 \
+    --hash=sha256:61b9a528fb348373c433e8966535074b802c7a5d7f23c4f421e6c6e2f1697a6f \
+    --hash=sha256:63426706118b7f5cf6bb6c895dc215d8a418d5952544042c8a2d9fe87fcf09cb \
+    --hash=sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb \
+    --hash=sha256:6f48351d66575f535669306aa7d6d6f71bc43372473b54a832222803eb956fd1 \
+    --hash=sha256:7ee7d9d4822c8acc74a5e26c50604dff824710bc8de424904c0982e25c39c6cb \
+    --hash=sha256:81c13a1fc7468c40f13420732805a4c38a105d89848b7c10af65a90beff25250 \
+    --hash=sha256:8d13c64ee2d33eccf7437961b6ea7ad8673e2be040b4f7fd4fd4d4d28d9ccb1e \
+    --hash=sha256:8de8bb0e5ad103888d65abef8bca41ab93721647590a3f740100cd65c3b00511 \
+    --hash=sha256:8fa03bce9bfbeeef9f3b160a8bed39a221d82308b4152b27d82d8daa7041fee5 \
+    --hash=sha256:924d94291ca674905fe9481f12294eb11f2d3d3fd1adb20314ba89e94f44ed59 \
+    --hash=sha256:975d70ab7e3c80a3fe86001d8751f6778905ec723f5b110aed1e450da9d4b7f2 \
+    --hash=sha256:976b9c42fb2a43ebf304fa7d4a310e5f16cc99992f33eced91ef6f908bd8f33d \
+    --hash=sha256:9e31cb64d7de6b6f09702bb27c02d1904b3aebfca610c12772452c4e6c21a0d3 \
+    --hash=sha256:a342242fe22407f3c17f4b499276a02b01e80f861f1682ad1d95b04018e0c0d4 \
+    --hash=sha256:a3d33a6b3eae87ceaefa91ffdc130b5e8536182cd6dfdbfc1aa56b46ff8c86de \
+    --hash=sha256:a895fcc7b15c3fc72beb43cdcbdf0ddb7d2ebc959edac9cef390b0d14f39f8a9 \
+    --hash=sha256:afb17f84d56068a7c29f5fa37bfd38d5aba69e3304af08ee94da8ed5b0865833 \
+    --hash=sha256:b1c546aca0ca4d028901d825015dc8e4d56aac4b541877690eb76490f1dc8ed0 \
+    --hash=sha256:b29019c76039dc3c0fd815c41392a044ce555d9bcdd38b0fb60fb4cd8e475ba9 \
+    --hash=sha256:b46517c02ccd08092f4fa99f24c3b83d8f92f739b4657b0f146246a0ca6a831d \
+    --hash=sha256:b7aa5f8a41217360e600da646004f878250a0d6738bcdc11a0a39928d7dc2050 \
+    --hash=sha256:b7b4c971f05e6ae490fef852c218b0e79d4e52f79ef0c8475566584a8fb3e01d \
+    --hash=sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6 \
+    --hash=sha256:cb017fd1b2603ef59e374ba2063f593abe0fc45f2ad9abdde5b4d83bd922a353 \
+    --hash=sha256:d22656368f0e6189e24722214ed8d66b8022db19d182927b9a248a2a8a2f67eb \
+    --hash=sha256:d2c2db7fd82e9b72937969bceac4d6ca89660db0a0967614ce2481e81a0b771e \
+    --hash=sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8 \
+    --hash=sha256:d62a5c7dad11015c66fbb9d881bc4caa5b12f16292f857842d9d1871595f4495 \
+    --hash=sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2 \
+    --hash=sha256:e84606b74eb7de6ff581a7915e2dab7a28a0517fbe1c9239eb227e1354064dcd \
+    --hash=sha256:eb393e5ebc85245347950143969b241d08b52b88a3dc39479822e073a1a8eb27 \
+    --hash=sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1 \
+    --hash=sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818 \
+    --hash=sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4 \
+    --hash=sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e \
+    --hash=sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850 \
+    --hash=sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3
+    # via -r requirements/requirements.in
+django==3.2.19 \
+    --hash=sha256:031365bae96814da19c10706218c44dff3b654cc4de20a98bd2d29b9bde469f0 \
+    --hash=sha256:21cc991466245d659ab79cb01204f9515690f8dae00e5eabde307f14d24d4d7d
+    # via -r requirements/requirements.in
+exceptiongroup==1.1.1 \
+    --hash=sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e \
+    --hash=sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785
+    # via pytest
+idna==3.4 \
+    --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
+    --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
+    # via requests
+importlib-metadata==6.7.0 \
+    --hash=sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4 \
+    --hash=sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5
+    # via pytest-randomly
+iniconfig==2.0.0 \
+    --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
+    --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
+    # via pytest
+packaging==23.1 \
+    --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
+    --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
+    # via pytest
+pluggy==1.2.0 \
+    --hash=sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849 \
+    --hash=sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3
+    # via pytest
+pytest==7.4.0 \
+    --hash=sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32 \
+    --hash=sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a
+    # via
+    #   -r requirements/requirements.in
+    #   pytest-django
+    #   pytest-randomly
+pytest-django==4.5.2 \
+    --hash=sha256:c60834861933773109334fe5a53e83d1ef4828f2203a1d6a0fa9972f4f75ab3e \
+    --hash=sha256:d9076f759bb7c36939dbdd5ae6633c18edfc2902d1a69fdbefd2426b970ce6c2
+    # via -r requirements/requirements.in
+pytest-randomly==3.12.0 \
+    --hash=sha256:d60c2db71ac319aee0fc6c4110a7597d611a8b94a5590918bfa8583f00caccb2 \
+    --hash=sha256:f4f2e803daf5d1ba036cc22bf4fe9dbbf99389ec56b00e5cba732fb5c1d07fdd
+    # via -r requirements/requirements.in
+pytz==2023.3 \
+    --hash=sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588 \
+    --hash=sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb
+    # via django
+requests==2.31.0 \
+    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
+    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
+    # via -r requirements/requirements.in
+sqlparse==0.4.4 \
+    --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
+    --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
+    # via django
+tomli==2.0.1 \
+    --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
+    --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
+    # via pytest
+typing-extensions==4.6.3 \
+    --hash=sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26 \
+    --hash=sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5
+    # via asgiref
+urllib3==2.0.3 \
+    --hash=sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1 \
+    --hash=sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825
+    # via requests
+zipp==3.15.0 \
+    --hash=sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b \
+    --hash=sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556
+    # via importlib-metadata
```

### Comparing `django-requests-api-0.2.0/runtests.py` & `django-requests-api-0.3.2/runtests.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import sys
-
-import pytest
-
-
-def split_class_and_function(string):
-    class_string, function_string = string.split(".", 1)
-    return f"{class_string} and {function_string}"
-
-
-def is_function(string):
-    # `True` if it looks like a test function is included in the string.
-    return string.startswith("test_") or ".test_" in string
-
-
-def is_class(string):
-    # `True` if first character is uppercase - assume it's a class name.
-    return string[0] == string[0].upper()
-
-
-if __name__ == "__main__":
-    if len(sys.argv) > 1:
-        pytest_args = sys.argv[1:]
-        first_arg = pytest_args[0]
-
-        try:
-            pytest_args.remove("--coverage")
-        except ValueError:
-            pass
-        else:
-            pytest_args = [
-                "--cov",
-                ".",
-                "--cov-report",
-                "xml",
-            ] + pytest_args
-
-        if first_arg.startswith("-"):
-            # `runtests.py [flags]`
-            pytest_args = ["tests"] + pytest_args
-        elif is_class(first_arg) and is_function(first_arg):
-            # `runtests.py TestCase.test_function [flags]`
-            expression = split_class_and_function(first_arg)
-            pytest_args = ["tests", "-k", expression] + pytest_args[1:]
-        elif is_class(first_arg) or is_function(first_arg):
-            # `runtests.py TestCase [flags]`
-            # `runtests.py test_function [flags]`
-            pytest_args = ["tests", "-k", pytest_args[0]] + pytest_args[1:]
-    else:
-        pytest_args = []
-
-    sys.exit(pytest.main(pytest_args))
+import sys
+
+import pytest
+
+
+def split_class_and_function(string):
+    class_string, function_string = string.split(".", 1)
+    return f"{class_string} and {function_string}"
+
+
+def is_function(string):
+    # `True` if it looks like a test function is included in the string.
+    return string.startswith("test_") or ".test_" in string
+
+
+def is_class(string):
+    # `True` if first character is uppercase - assume it's a class name.
+    return string[0] == string[0].upper()
+
+
+if __name__ == "__main__":
+    if len(sys.argv) > 1:
+        pytest_args = sys.argv[1:]
+        first_arg = pytest_args[0]
+
+        try:
+            pytest_args.remove("--coverage")
+        except ValueError:
+            pass
+        else:
+            pytest_args = [
+                "--cov",
+                ".",
+                "--cov-report",
+                "xml",
+            ] + pytest_args
+
+        if first_arg.startswith("-"):
+            # `runtests.py [flags]`
+            pytest_args = ["tests"] + pytest_args
+        elif is_class(first_arg) and is_function(first_arg):
+            # `runtests.py TestCase.test_function [flags]`
+            expression = split_class_and_function(first_arg)
+            pytest_args = ["tests", "-k", expression] + pytest_args[1:]
+        elif is_class(first_arg) or is_function(first_arg):
+            # `runtests.py TestCase [flags]`
+            # `runtests.py test_function [flags]`
+            pytest_args = ["tests", "-k", pytest_args[0]] + pytest_args[1:]
+    else:
+        pytest_args = []
+
+    sys.exit(pytest.main(pytest_args))
```

### Comparing `django-requests-api-0.2.0/setup.cfg` & `django-requests-api-0.3.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,115 @@
-00000000: 5b62 6469 7374 5f77 6865 656c 5d0d 0a75  [bdist_wheel]..u
-00000010: 6e69 7665 7273 616c 203d 2031 0d0a 0d0a  niversal = 1....
-00000020: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000030: 203d 2064 6a61 6e67 6f2d 7265 7175 6573   = django-reques
-00000040: 7473 2d61 7069 0d0a 7665 7273 696f 6e20  ts-api..version 
-00000050: 3d20 302e 322e 300d 0a75 726c 203d 2068  = 0.2.0..url = h
-00000060: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000070: 6d2f 444c 5253 502f 646a 616e 676f 2d72  m/DLRSP/django-r
-00000080: 6571 7565 7374 732d 6170 690d 0a61 7574  equests-api..aut
-00000090: 686f 7220 3d20 444c 5253 500d 0a61 7574  hor = DLRSP..aut
-000000a0: 686f 725f 656d 6169 6c20 3d20 646c 7273  hor_email = dlrs
-000000b0: 702e 6465 7640 676d 6169 6c2e 636f 6d0d  p.dev@gmail.com.
-000000c0: 0a64 6573 6372 6970 7469 6f6e 203d 2044  .description = D
-000000d0: 6a61 6e67 6f20 6170 706c 6963 6174 696f  jango applicatio
-000000e0: 6e20 746f 2070 726f 7669 6465 2073 696d  n to provide sim
-000000f0: 706c 6520 616e 6420 7368 6172 6564 2072  ple and shared r
-00000100: 6571 7565 7374 7320 636c 6965 6e74 2e0d  equests client..
-00000110: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-00000120: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
-00000130: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
-00000140: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
-00000150: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
-00000160: 776e 0d0a 6c69 6365 6e73 6520 3d20 4d49  wn..license = MI
-00000170: 5420 4c69 6365 6e73 650d 0a6c 6963 656e  T License..licen
-00000180: 7365 5f66 696c 6573 203d 204c 4943 454e  se_files = LICEN
-00000190: 5345 0d0a 6b65 7977 6f72 6473 203d 200d  SE..keywords = .
-000001a0: 0a09 646a 616e 676f 0d0a 0972 6571 7565  ..django...reque
-000001b0: 7374 730d 0a09 4150 490d 0a09 7072 6976  sts...API...priv
-000001c0: 6163 790d 0a09 636f 6f6b 6965 0d0a 636c  acy...cookie..cl
-000001d0: 6173 7369 6669 6572 7320 3d20 0d0a 0944  assifiers = ...D
-000001e0: 6576 656c 6f70 6d65 6e74 2053 7461 7475  evelopment Statu
-000001f0: 7320 3a3a 2034 202d 2042 6574 610d 0a09  s :: 4 - Beta...
-00000200: 456e 7669 726f 6e6d 656e 7420 3a3a 2057  Environment :: W
-00000210: 6562 2045 6e76 6972 6f6e 6d65 6e74 0d0a  eb Environment..
-00000220: 0946 7261 6d65 776f 726b 203a 3a20 446a  .Framework :: Dj
-00000230: 616e 676f 0d0a 0946 7261 6d65 776f 726b  ango...Framework
-00000240: 203a 3a20 446a 616e 676f 203a 3a20 332e   :: Django :: 3.
-00000250: 320d 0a09 4672 616d 6577 6f72 6b20 3a3a  2...Framework ::
-00000260: 2044 6a61 6e67 6f20 3a3a 2034 2e30 0d0a   Django :: 4.0..
-00000270: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
-00000280: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
-00000290: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
-000002a0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-000002b0: 5420 4c69 6365 6e73 650d 0a09 4f70 6572  T License...Oper
-000002c0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-000002d0: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
-000002e0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-000002f0: 6775 6167 6520 3a3a 2050 7974 686f 6e0d  guage :: Python.
-00000300: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000310: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000320: 203a 3a20 330d 0a09 5072 6f67 7261 6d6d   :: 3...Programm
-00000330: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000340: 5079 7468 6f6e 203a 3a20 3320 3a3a 204f  Python :: 3 :: O
-00000350: 6e6c 790d 0a09 5072 6f67 7261 6d6d 696e  nly...Programmin
-00000360: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000370: 7468 6f6e 203a 3a20 332e 370d 0a09 5072  thon :: 3.7...Pr
-00000380: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000390: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000003a0: 332e 380d 0a09 5072 6f67 7261 6d6d 696e  3.8...Programmin
-000003b0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000003c0: 7468 6f6e 203a 3a20 332e 390d 0a09 5072  thon :: 3.9...Pr
-000003d0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000003e0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000003f0: 332e 3130 0d0a 0950 726f 6772 616d 6d69  3.10...Programmi
-00000400: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000410: 7974 686f 6e20 3a3a 2033 2e31 310d 0a09  ython :: 3.11...
-00000420: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000430: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-00000440: 6e74 0d0a 0954 6f70 6963 203a 3a20 496e  nt...Topic :: In
-00000450: 7465 726e 6574 203a 3a20 5757 572f 4854  ternet :: WWW/HT
-00000460: 5450 0d0a 0954 6f70 6963 203a 3a20 496e  TP...Topic :: In
-00000470: 7465 726e 6574 203a 3a20 5757 572f 4854  ternet :: WWW/HT
-00000480: 5450 203a 3a20 4479 6e61 6d69 6320 436f  TP :: Dynamic Co
-00000490: 6e74 656e 740d 0a09 546f 7069 6320 3a3a  ntent...Topic ::
-000004a0: 2049 6e74 6572 6e65 7420 3a3a 2057 5757   Internet :: WWW
-000004b0: 2f48 5454 5020 3a3a 2057 5347 4920 3a3a  /HTTP :: WSGI ::
-000004c0: 2041 7070 6c69 6361 7469 6f6e 0d0a 0954   Application...T
-000004d0: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
-000004e0: 2044 6576 656c 6f70 6d65 6e74 203a 3a20   Development :: 
-000004f0: 4c69 6272 6172 6965 7320 3a3a 2041 7070  Libraries :: App
-00000500: 6c69 6361 7469 6f6e 2046 7261 6d65 776f  lication Framewo
-00000510: 726b 730d 0a09 546f 7069 6320 3a3a 2053  rks...Topic :: S
-00000520: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
-00000530: 656e 7420 3a3a 204c 6962 7261 7269 6573  ent :: Libraries
-00000540: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
-00000550: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
-00000560: 3d73 7263 0d0a 7365 7475 705f 7265 7175  =src..setup_requ
-00000570: 6972 6573 203d 2044 6a61 6e67 6f3e 3d32  ires = Django>=2
-00000580: 2e32 0d0a 696e 7374 616c 6c5f 7265 7175  .2..install_requ
-00000590: 6972 6573 203d 2044 6a61 6e67 6f3e 3d32  ires = Django>=2
-000005a0: 2e32 0d0a 7061 636b 6167 6573 203d 2066  .2..packages = f
-000005b0: 696e 643a 0d0a 696e 636c 7564 655f 7061  ind:..include_pa
-000005c0: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
-000005d0: 650d 0a70 7974 686f 6e5f 7265 7175 6972  e..python_requir
-000005e0: 6573 203d 203e 3d33 2e37 0d0a 7a69 705f  es = >=3.7..zip_
-000005f0: 7361 6665 203d 2046 616c 7365 0d0a 0d0a  safe = False....
-00000600: 5b6f 7074 696f 6e73 2e65 7874 7261 735f  [options.extras_
-00000610: 7265 7175 6972 655d 0d0a 7465 7374 696e  require]..testin
-00000620: 6720 3d20 0d0a 0963 6f76 6572 6167 650d  g = ...coverage.
-00000630: 0a09 636f 6465 636f 760d 0a6c 696e 7469  ..codecov..linti
-00000640: 6e67 203d 200d 0a09 666c 616b 6538 0d0a  ng = ...flake8..
-00000650: 0970 796c 696e 740d 0a0d 0a5b 6f70 7469  .pylint....[opti
-00000660: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
-00000670: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
-00000680: 0a0d 0a5b 636f 7665 7261 6765 3a72 756e  ...[coverage:run
-00000690: 5d0d 0a62 7261 6e63 6820 3d20 5472 7565  ]..branch = True
-000006a0: 0d0a 736f 7572 6365 203d 2072 6571 7565  ..source = reque
-000006b0: 7374 5f61 7069 0d0a 0d0a 5b63 6f76 6572  st_api....[cover
-000006c0: 6167 653a 7061 7468 735d 0d0a 736f 7572  age:paths]..sour
-000006d0: 6365 203d 200d 0a09 7372 630d 0a09 2e74  ce = ...src....t
-000006e0: 6f78 2f2a 2f73 6974 652d 7061 636b 6167  ox/*/site-packag
-000006f0: 6573 0d0a 0d0a 5b63 6f76 6572 6167 653a  es....[coverage:
-00000700: 7265 706f 7274 5d0d 0a73 686f 775f 6d69  report]..show_mi
-00000710: 7373 696e 6720 3d20 5472 7565 0d0a 0d0a  ssing = True....
-00000720: 5b66 6c61 6b65 385d 0d0a 6d61 782d 6c69  [flake8]..max-li
-00000730: 6e65 2d6c 656e 6774 6820 3d20 3830 0d0a  ne-length = 80..
-00000740: 7365 6c65 6374 203d 2045 2c46 2c57 2c42  select = E,F,W,B
-00000750: 2c42 3935 302c 432c 492c 5459 500d 0a69  ,B950,C,I,TYP..i
-00000760: 676e 6f72 6520 3d20 4532 3033 2c45 3530  gnore = E203,E50
-00000770: 312c 5735 3033 0d0a 0d0a 5b65 6767 5f69  1,W503....[egg_i
-00000780: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-00000790: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-000007a0: 0d0a 0d0a                                ....
+00000000: 5b62 6469 7374 5f77 6865 656c 5d0a 756e  [bdist_wheel].un
+00000010: 6976 6572 7361 6c20 3d20 310a 0a5b 6d65  iversal = 1..[me
+00000020: 7461 6461 7461 5d0a 6e61 6d65 203d 2064  tadata].name = d
+00000030: 6a61 6e67 6f2d 7265 7175 6573 7473 2d61  jango-requests-a
+00000040: 7069 0a76 6572 7369 6f6e 203d 2030 2e33  pi.version = 0.3
+00000050: 2e32 0a75 726c 203d 2068 7474 7073 3a2f  .2.url = https:/
+00000060: 2f67 6974 6875 622e 636f 6d2f 444c 5253  /github.com/DLRS
+00000070: 502f 646a 616e 676f 2d72 6571 7565 7374  P/django-request
+00000080: 732d 6170 690a 6175 7468 6f72 203d 2044  s-api.author = D
+00000090: 4c52 5350 0a61 7574 686f 725f 656d 6169  LRSP.author_emai
+000000a0: 6c20 3d20 646c 7273 702e 6465 7640 676d  l = dlrsp.dev@gm
+000000b0: 6169 6c2e 636f 6d0a 6465 7363 7269 7074  ail.com.descript
+000000c0: 696f 6e20 3d20 446a 616e 676f 2061 7070  ion = Django app
+000000d0: 6c69 6361 7469 6f6e 2074 6f20 7072 6f76  lication to prov
+000000e0: 6964 6520 7369 6d70 6c65 2061 6e64 2073  ide simple and s
+000000f0: 6861 7265 6420 7265 7175 6573 7473 2063  hared requests c
+00000100: 6c69 656e 742e 0a6c 6f6e 675f 6465 7363  lient..long_desc
+00000110: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
+00000120: 5245 4144 4d45 2e6d 640a 6c6f 6e67 5f64  README.md.long_d
+00000130: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
+00000140: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
+00000150: 6172 6b64 6f77 6e0a 6c69 6365 6e73 6520  arkdown.license 
+00000160: 3d20 4d49 5420 4c69 6365 6e73 650a 6c69  = MIT License.li
+00000170: 6365 6e73 655f 6669 6c65 7320 3d20 4c49  cense_files = LI
+00000180: 4345 4e53 450a 6b65 7977 6f72 6473 203d  CENSE.keywords =
+00000190: 200a 0964 6a61 6e67 6f0a 0972 6571 7565   ..django..reque
+000001a0: 7374 730a 0941 5049 0a09 7072 6976 6163  sts..API..privac
+000001b0: 790a 0963 6f6f 6b69 650a 636c 6173 7369  y..cookie.classi
+000001c0: 6669 6572 7320 3d20 0a09 4465 7665 6c6f  fiers = ..Develo
+000001d0: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
+000001e0: 3420 2d20 4265 7461 0a09 456e 7669 726f  4 - Beta..Enviro
+000001f0: 6e6d 656e 7420 3a3a 2057 6562 2045 6e76  nment :: Web Env
+00000200: 6972 6f6e 6d65 6e74 0a09 4672 616d 6577  ironment..Framew
+00000210: 6f72 6b20 3a3a 2044 6a61 6e67 6f0a 0946  ork :: Django..F
+00000220: 7261 6d65 776f 726b 203a 3a20 446a 616e  ramework :: Djan
+00000230: 676f 203a 3a20 332e 320a 0946 7261 6d65  go :: 3.2..Frame
+00000240: 776f 726b 203a 3a20 446a 616e 676f 203a  work :: Django :
+00000250: 3a20 342e 320a 0949 6e74 656e 6465 6420  : 4.2..Intended 
+00000260: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
+00000270: 6c6f 7065 7273 0a09 4c69 6365 6e73 6520  lopers..License 
+00000280: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00000290: 3a3a 204d 4954 204c 6963 656e 7365 0a09  :: MIT License..
+000002a0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+000002b0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+000002c0: 6e74 0a09 5072 6f67 7261 6d6d 696e 6720  nt..Programming 
+000002d0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002e0: 6f6e 0a09 5072 6f67 7261 6d6d 696e 6720  on..Programming 
+000002f0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000300: 6f6e 203a 3a20 330a 0950 726f 6772 616d  on :: 3..Program
+00000310: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000320: 2050 7974 686f 6e20 3a3a 2033 203a 3a20   Python :: 3 :: 
+00000330: 4f6e 6c79 0a09 5072 6f67 7261 6d6d 696e  Only..Programmin
+00000340: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000350: 7468 6f6e 203a 3a20 332e 380a 0950 726f  thon :: 3.8..Pro
+00000360: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000370: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000380: 2e39 0a09 5072 6f67 7261 6d6d 696e 6720  .9..Programming 
+00000390: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000003a0: 6f6e 203a 3a20 332e 3130 0a09 5072 6f67  on :: 3.10..Prog
+000003b0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000003c0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000003d0: 3131 0a09 4f70 6572 6174 696e 6720 5379  11..Operating Sy
+000003e0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+000003f0: 656e 6465 6e74 0a09 546f 7069 6320 3a3a  endent..Topic ::
+00000400: 2049 6e74 6572 6e65 7420 3a3a 2057 5757   Internet :: WWW
+00000410: 2f48 5454 500a 0954 6f70 6963 203a 3a20  /HTTP..Topic :: 
+00000420: 496e 7465 726e 6574 203a 3a20 5757 572f  Internet :: WWW/
+00000430: 4854 5450 203a 3a20 4479 6e61 6d69 6320  HTTP :: Dynamic 
+00000440: 436f 6e74 656e 740a 0954 6f70 6963 203a  Content..Topic :
+00000450: 3a20 496e 7465 726e 6574 203a 3a20 5757  : Internet :: WW
+00000460: 572f 4854 5450 203a 3a20 5753 4749 203a  W/HTTP :: WSGI :
+00000470: 3a20 4170 706c 6963 6174 696f 6e0a 0954  : Application..T
+00000480: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
+00000490: 2044 6576 656c 6f70 6d65 6e74 203a 3a20   Development :: 
+000004a0: 4c69 6272 6172 6965 7320 3a3a 2041 7070  Libraries :: App
+000004b0: 6c69 6361 7469 6f6e 2046 7261 6d65 776f  lication Framewo
+000004c0: 726b 730a 0954 6f70 6963 203a 3a20 536f  rks..Topic :: So
+000004d0: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
+000004e0: 6e74 203a 3a20 4c69 6272 6172 6965 730a  nt :: Libraries.
+000004f0: 0a5b 6f70 7469 6f6e 735d 0a70 6163 6b61  .[options].packa
+00000500: 6765 5f64 6972 203d 200a 093d 7372 630a  ge_dir = ..=src.
+00000510: 7365 7475 705f 7265 7175 6972 6573 203d  setup_requires =
+00000520: 2044 6a61 6e67 6f3e 3d33 2e32 0a69 6e73   Django>=3.2.ins
+00000530: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
+00000540: 446a 616e 676f 3e3d 332e 320a 7061 636b  Django>=3.2.pack
+00000550: 6167 6573 203d 2066 696e 643a 0a69 6e63  ages = find:.inc
+00000560: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
+00000570: 6120 3d20 5472 7565 0a70 7974 686f 6e5f  a = True.python_
+00000580: 7265 7175 6972 6573 203d 203e 3d33 2e38  requires = >=3.8
+00000590: 0a7a 6970 5f73 6166 6520 3d20 4661 6c73  .zip_safe = Fals
+000005a0: 650a 0a5b 6f70 7469 6f6e 732e 6578 7472  e..[options.extr
+000005b0: 6173 5f72 6571 7569 7265 5d0a 7465 7374  as_require].test
+000005c0: 696e 6720 3d20 0a09 636f 7665 7261 6765  ing = ..coverage
+000005d0: 0a09 636f 6465 636f 760a 6c69 6e74 696e  ..codecov.lintin
+000005e0: 6720 3d20 0a09 666c 616b 6538 0a09 7079  g = ..flake8..py
+000005f0: 6c69 6e74 0a0a 5b6f 7074 696f 6e73 2e70  lint..[options.p
+00000600: 6163 6b61 6765 732e 6669 6e64 5d0a 7768  ackages.find].wh
+00000610: 6572 6520 3d20 7372 630a 0a5b 636f 7665  ere = src..[cove
+00000620: 7261 6765 3a72 756e 5d0a 6272 616e 6368  rage:run].branch
+00000630: 203d 2054 7275 650a 736f 7572 6365 203d   = True.source =
+00000640: 2072 6571 7565 7374 735f 6170 690a 0a5b   requests_api..[
+00000650: 636f 7665 7261 6765 3a70 6174 6873 5d0a  coverage:paths].
+00000660: 736f 7572 6365 203d 200a 0973 7263 0a09  source = ..src..
+00000670: 2e74 6f78 2f2a 2f73 6974 652d 7061 636b  .tox/*/site-pack
+00000680: 6167 6573 0a0a 5b63 6f76 6572 6167 653a  ages..[coverage:
+00000690: 7265 706f 7274 5d0a 7368 6f77 5f6d 6973  report].show_mis
+000006a0: 7369 6e67 203d 2054 7275 650a 0a5b 666c  sing = True..[fl
+000006b0: 616b 6538 5d0a 6d61 782d 6c69 6e65 2d6c  ake8].max-line-l
+000006c0: 656e 6774 6820 3d20 3830 0a73 656c 6563  ength = 80.selec
+000006d0: 7420 3d20 452c 462c 572c 422c 4239 3530  t = E,F,W,B,B950
+000006e0: 2c43 2c49 2c54 5950 0a69 676e 6f72 6520  ,C,I,TYP.ignore 
+000006f0: 3d20 4532 3033 2c45 3530 312c 5735 3033  = E203,E501,W503
+00000700: 0a0a 5b65 6767 5f69 6e66 6f5d 0a74 6167  ..[egg_info].tag
+00000710: 5f62 7569 6c64 203d 200a 7461 675f 6461  _build = .tag_da
+00000720: 7465 203d 2030 0a0a                      te = 0..
```

### Comparing `django-requests-api-0.2.0/src/django_requests_api.egg-info/PKG-INFO` & `django-requests-api-0.3.2/src/django_requests_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,96 +1,95 @@
-Metadata-Version: 2.1
-Name: django-requests-api
-Version: 0.2.0
-Summary: Django application to provide simple and shared requests client.
-Home-page: https://github.com/DLRSP/django-requests-api
-Author: DLRSP
-Author-email: dlrsp.dev@gmail.com
-License: MIT License
-Keywords: django,requests,API,privacy,cookie
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-Provides-Extra: linting
-License-File: LICENSE
-
-# django-requests-api [![PyPi license](https://img.shields.io/pypi/l/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-
-[![PyPi status](https://img.shields.io/pypi/status/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-[![PyPi version](https://img.shields.io/pypi/v/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-[![PyPi python version](https://img.shields.io/pypi/pyversions/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-[![PyPi downloads](https://img.shields.io/pypi/dm/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-[![PyPi downloads](https://img.shields.io/pypi/dw/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-[![PyPi downloads](https://img.shields.io/pypi/dd/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
-
-## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-requests-api.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-requests-api.svg)
-
-## Test [![codecov.io](https://codecov.io/github/DLRSP/django-requests-api/coverage.svg?branch=master)](https://codecov.io/github/DLRSP/django-requests-api?branch=master) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-requests-api/master.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-requests-api/master) [![gitthub.com](https://github.com/DLRSP/django-requests-api/actions/workflows/ci.yml/badge.svg)](https://github.com/DLRSP/django-requests-api/actions/workflows/ci.yml)
-
-## Check Demo Project
-* Browser the demo app on-line on [Heroku](https://django-requests-api.herokuapp.com/)
-* Check the demo repo on [GitHub](https://github.com/DLRSP/example/tree/django-requests-api)
-
-## Requirements
--   Python 3.7 to 3.10 supported.
--   Django 3.2 to 4.2 supported.
-
-## Setup
-1. Install from **pip**:
-```shell
-pip install django-requests-api
-```
-
-2. Modify `settings.py` by adding the app to `INSTALLED_APPS`:
-```python
-INSTALLED_APPS = (
-    # ...
-    "requests_api",
-    # ...
-)
-```
-
-## Usage
-
-```shell
-from requests_api import RequestsApi
-
-client = RequestsApi("https://api.publicapis.org")
-r = client.get("/entries")
-print(r.json())
-
-github = RequestsApi("https://api.github.com", headers={"Authorization": "token abcdef"})
-r = github.get("/user", headers={"Accept": "application/json"})
-print(r.text)
-```
-
-## Run Example Project
-
-```shell
-git clone --depth=50 --branch=django-requests-api https://github.com/DLRSP/example.git DLRSP/example
-cd DLRSP/example
-python manage.py runserver
-```
-
-Now browser the app @ http://127.0.0.1:8000
+Metadata-Version: 2.1
+Name: django-requests-api
+Version: 0.3.2
+Summary: Django application to provide simple and shared requests client.
+Home-page: https://github.com/DLRSP/django-requests-api
+Author: DLRSP
+Author-email: dlrsp.dev@gmail.com
+License: MIT License
+Keywords: django,requests,API,privacy,cookie
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+Provides-Extra: linting
+License-File: LICENSE
+
+# django-requests-api [![PyPi license](https://img.shields.io/pypi/l/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+
+[![PyPi status](https://img.shields.io/pypi/status/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+[![PyPi version](https://img.shields.io/pypi/v/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+[![PyPi python version](https://img.shields.io/pypi/pyversions/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+[![PyPi downloads](https://img.shields.io/pypi/dm/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+[![PyPi downloads](https://img.shields.io/pypi/dw/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+[![PyPi downloads](https://img.shields.io/pypi/dd/django-requests-api.svg)](https://pypi.python.org/pypi/django-requests-api)
+
+## GitHub ![GitHub release](https://img.shields.io/github/tag/DLRSP/django-requests-api.svg) ![GitHub release](https://img.shields.io/github/release/DLRSP/django-requests-api.svg)
+
+## Test [![codecov.io](https://codecov.io/github/DLRSP/django-requests-api/coverage.svg?branch=master)](https://codecov.io/github/DLRSP/django-requests-api?branch=master) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DLRSP/django-requests-api/master.svg)](https://results.pre-commit.ci/latest/github/DLRSP/django-requests-api/master) [![gitthub.com](https://github.com/DLRSP/django-requests-api/actions/workflows/ci.yml/badge.svg)](https://github.com/DLRSP/django-requests-api/actions/workflows/ci.yml)
+
+## Check Demo Project
+* Browser the demo app on-line on [Heroku](https://django-requests-api.herokuapp.com/)
+* Check the demo repo on [GitHub](https://github.com/DLRSP/example/tree/django-requests-api)
+
+## Requirements
+-   Python 3.8+ supported.
+-   Django 3.2+ supported.
+
+## Setup
+1. Install from **pip**:
+```shell
+pip install django-requests-api
+```
+
+2. Modify `settings.py` by adding the app to `INSTALLED_APPS`:
+```python
+INSTALLED_APPS = (
+    # ...
+    "requests_api",
+    # ...
+)
+```
+
+## Usage
+
+```shell
+from requests_api import RequestsApi
+
+client = RequestsApi("https://api.publicapis.org")
+r = client.get("/entries")
+print(r.json())
+
+github = RequestsApi("https://api.github.com", headers={"Authorization": "token abcdef"})
+r = github.get("/user", headers={"Accept": "application/json"})
+print(r.text)
+```
+
+## Run Example Project
+
+```shell
+git clone --depth=50 --branch=django-requests-api https://github.com/DLRSP/example.git DLRSP/example
+cd DLRSP/example
+python manage.py runserver
+```
+
+Now browser the app @ http://127.0.0.1:8000
```

### Comparing `django-requests-api-0.2.0/src/django_requests_api.egg-info/SOURCES.txt` & `django-requests-api-0.3.2/src/django_requests_api.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -10,33 +10,29 @@
 runtests.py
 setup.cfg
 setup.py
 tox.ini
 requirements/docs.in
 requirements/docs.txt
 requirements/py310-django32.txt
-requirements/py310-django40.txt
+requirements/py310-django42.txt
 requirements/py311-django32.txt
-requirements/py311-django40.txt
-requirements/py37-django22.txt
-requirements/py37-django32.txt
-requirements/py38-django22.txt
+requirements/py311-django42.txt
 requirements/py38-django32.txt
-requirements/py38-django40.txt
-requirements/py39-django22.txt
+requirements/py38-django42.txt
 requirements/py39-django32.txt
-requirements/py39-django40.txt
+requirements/py39-django42.txt
 requirements/requirements.in
 src/django_requests_api.egg-info/PKG-INFO
 src/django_requests_api.egg-info/SOURCES.txt
 src/django_requests_api.egg-info/dependency_links.txt
 src/django_requests_api.egg-info/not-zip-safe
 src/django_requests_api.egg-info/requires.txt
 src/django_requests_api.egg-info/top_level.txt
 src/requests_api/__init__.py
 src/requests_api/apps.py
 src/requests_api/requests_api.py
 tests/__init__.py
 tests/settings.py
-tests/test_iubenda.py
+tests/test_requests_api.py
 tests/urls.py
 tests/views.py
```

### Comparing `django-requests-api-0.2.0/src/requests_api/requests_api.py` & `django-requests-api-0.3.2/src/requests_api/requests_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,55 @@
-from http.cookiejar import Cookie
-
-import requests
-from requests import Response
-
-
-class RequestsApi:
-    def __init__(self, base_url: str | bytes, **kwargs):
-        self.base_url = base_url
-        self.session = requests.Session()
-        for arg in kwargs:
-            if isinstance(kwargs[arg], dict):
-                kwargs[arg] = self.__deep_merge(getattr(self.session, arg), kwargs[arg])
-            setattr(self.session, arg, kwargs[arg])
-
-    def request(self, method: str | bytes, url: str | bytes, **kwargs) -> Response:
-        return self.session.request(method, self.base_url + url, **kwargs)
-
-    def head(self, url: str | bytes, **kwargs) -> Response:
-        return self.session.head(self.base_url + url, **kwargs)
-
-    def get(self, url: str | bytes, **kwargs) -> Response:
-        return self.session.get(self.base_url + url, **kwargs)
-
-    def post(self, url: str | bytes, **kwargs) -> Response:
-        return self.session.post(self.base_url + url, **kwargs)
-
-    def put(self, url: str | bytes, **kwargs) -> Response:
-        return self.session.put(self.base_url + url, **kwargs)
-
-    def patch(self, url: str | bytes, **kwargs) -> Response:
-        return self.session.patch(self.base_url + url, **kwargs)
-
-    def delete(self, url: str | bytes, **kwargs) -> Response:
-        return self.session.delete(self.base_url + url, **kwargs)
-
-    def create_cookie(self, **kwargs) -> Cookie:
-        return requests.cookies.create_cookie(**kwargs)
-
-    def set_cookie(self, cookie: Cookie) -> None:
-        return self.session.cookies.set_cookie(cookie)
-
-    def headers(self, header: dict) -> None:
-        return self.session.headers.update(header)
-
-    @staticmethod
-    def __deep_merge(source, destination):
-        for key, value in source.items():
-            if isinstance(value, dict):
-                node = destination.setdefault(key, {})
-                RequestsApi.__deep_merge(value, node)
-            else:
-                destination[key] = value
-        return destination
+from __future__ import annotations
+from http.cookiejar import Cookie
+
+import requests
+from requests import Response
+
+
+class RequestsApi:
+    def __init__(self, base_url: str | bytes, **kwargs):
+        self.base_url = base_url
+        self.session = requests.Session()
+        for arg in kwargs:
+            if isinstance(kwargs[arg], dict):
+                kwargs[arg] = self.__deep_merge(getattr(self.session, arg), kwargs[arg])
+            setattr(self.session, arg, kwargs[arg])
+
+    def request(self, method: str | bytes, url: str | bytes, **kwargs) -> Response:
+        return self.session.request(method, self.base_url + url, **kwargs)
+
+    def head(self, url: str | bytes, **kwargs) -> Response:
+        return self.session.head(self.base_url + url, **kwargs)
+
+    def get(self, url: str | bytes, **kwargs) -> Response:
+        return self.session.get(self.base_url + url, **kwargs)
+
+    def post(self, url: str | bytes, **kwargs) -> Response:
+        return self.session.post(self.base_url + url, **kwargs)
+
+    def put(self, url: str | bytes, **kwargs) -> Response:
+        return self.session.put(self.base_url + url, **kwargs)
+
+    def patch(self, url: str | bytes, **kwargs) -> Response:
+        return self.session.patch(self.base_url + url, **kwargs)
+
+    def delete(self, url: str | bytes, **kwargs) -> Response:
+        return self.session.delete(self.base_url + url, **kwargs)
+
+    def create_cookie(self, **kwargs) -> Cookie:
+        return requests.cookies.create_cookie(**kwargs)
+
+    def set_cookie(self, cookie: Cookie) -> None:
+        return self.session.cookies.set_cookie(cookie)
+
+    def headers(self, header: dict) -> None:
+        return self.session.headers.update(header)
+
+    @staticmethod
+    def __deep_merge(source, destination):
+        for key, value in source.items():
+            if isinstance(value, dict):
+                node = destination.setdefault(key, {})
+                RequestsApi.__deep_merge(value, node)
+            else:
+                destination[key] = value
+        return destination
```

### Comparing `django-requests-api-0.2.0/tox.ini` & `django-requests-api-0.3.2/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,51 @@
-00000000: 5b74 6f78 5d0d 0a69 736f 6c61 7465 645f  [tox]..isolated_
-00000010: 6275 696c 6420 3d20 5472 7565 0d0a 656e  build = True..en
-00000020: 766c 6973 7420 3d0d 0a20 2020 2070 7933  vlist =..    py3
-00000030: 372d 646a 616e 676f 7b33 327d 0d0a 2020  7-django{32}..  
-00000040: 2020 7079 3338 2d64 6a61 6e67 6f7b 3332    py38-django{32
-00000050: 2c34 307d 0d0a 2020 2020 7079 3339 2d64  ,40}..    py39-d
-00000060: 6a61 6e67 6f7b 3332 2c34 307d 0d0a 2020  jango{32,40}..  
-00000070: 2020 7079 3331 302d 646a 616e 676f 7b33    py310-django{3
-00000080: 322c 3430 7d0d 0a20 2020 2070 7933 3131  2,40}..    py311
-00000090: 2d64 6a61 6e67 6f7b 3332 2c34 307d 0d0a  -django{32,40}..
-000000a0: 0d0a 5b74 6573 7465 6e76 5d0d 0a63 6f6d  ..[testenv]..com
-000000b0: 6d61 6e64 7320 3d20 7079 7468 6f6e 202d  mands = python -
-000000c0: 5720 6572 726f 723a 3a44 6570 7265 6361  W error::Depreca
-000000d0: 7469 6f6e 5761 726e 696e 6720 2d57 2065  tionWarning -W e
-000000e0: 7272 6f72 3a3a 5065 6e64 696e 6744 6570  rror::PendingDep
-000000f0: 7265 6361 7469 6f6e 5761 726e 696e 6720  recationWarning 
-00000100: 2d6d 2063 6f76 6572 6167 6520 7275 6e20  -m coverage run 
-00000110: 2d2d 7061 7261 6c6c 656c 202d 6d20 7079  --parallel -m py
-00000120: 7465 7374 207b 706f 7361 7267 733a 7465  test {posargs:te
-00000130: 7374 737d 0d0a 0d0a 5b74 6573 7465 6e76  sts}....[testenv
-00000140: 3a70 7933 372d 646a 616e 676f 3332 5d0d  :py37-django32].
-00000150: 0a64 6570 7320 3d20 2d72 7265 7175 6972  .deps = -rrequir
-00000160: 656d 656e 7473 2f70 7933 372d 646a 616e  ements/py37-djan
-00000170: 676f 3332 2e74 7874 0d0a 0d0a 5b74 6573  go32.txt....[tes
-00000180: 7465 6e76 3a70 7933 382d 646a 616e 676f  tenv:py38-django
-00000190: 3332 5d0d 0a64 6570 7320 3d20 2d72 7265  32]..deps = -rre
-000001a0: 7175 6972 656d 656e 7473 2f70 7933 382d  quirements/py38-
-000001b0: 646a 616e 676f 3332 2e74 7874 0d0a 0d0a  django32.txt....
-000001c0: 5b74 6573 7465 6e76 3a70 7933 382d 646a  [testenv:py38-dj
-000001d0: 616e 676f 3430 5d0d 0a64 6570 7320 3d20  ango40]..deps = 
-000001e0: 2d72 7265 7175 6972 656d 656e 7473 2f70  -rrequirements/p
-000001f0: 7933 382d 646a 616e 676f 3430 2e74 7874  y38-django40.txt
-00000200: 0d0a 0d0a 5b74 6573 7465 6e76 3a70 7933  ....[testenv:py3
-00000210: 392d 646a 616e 676f 3332 5d0d 0a64 6570  9-django32]..dep
-00000220: 7320 3d20 2d72 7265 7175 6972 656d 656e  s = -rrequiremen
-00000230: 7473 2f70 7933 392d 646a 616e 676f 3332  ts/py39-django32
-00000240: 2e74 7874 0d0a 0d0a 5b74 6573 7465 6e76  .txt....[testenv
-00000250: 3a70 7933 392d 646a 616e 676f 3430 5d0d  :py39-django40].
-00000260: 0a64 6570 7320 3d20 2d72 7265 7175 6972  .deps = -rrequir
-00000270: 656d 656e 7473 2f70 7933 392d 646a 616e  ements/py39-djan
-00000280: 676f 3430 2e74 7874 0d0a 0d0a 5b74 6573  go40.txt....[tes
-00000290: 7465 6e76 3a70 7933 3130 2d64 6a61 6e67  tenv:py310-djang
-000002a0: 6f33 325d 0d0a 6465 7073 203d 202d 7272  o32]..deps = -rr
-000002b0: 6571 7569 7265 6d65 6e74 732f 7079 3331  equirements/py31
-000002c0: 302d 646a 616e 676f 3332 2e74 7874 0d0a  0-django32.txt..
-000002d0: 0d0a 5b74 6573 7465 6e76 3a70 7933 3130  ..[testenv:py310
-000002e0: 2d64 6a61 6e67 6f34 305d 0d0a 6465 7073  -django40]..deps
-000002f0: 203d 202d 7272 6571 7569 7265 6d65 6e74   = -rrequirement
-00000300: 732f 7079 3331 302d 646a 616e 676f 3430  s/py310-django40
-00000310: 2e74 7874 0d0a 0d0a 5b74 6573 7465 6e76  .txt....[testenv
-00000320: 3a70 7933 3131 2d64 6a61 6e67 6f33 325d  :py311-django32]
-00000330: 0d0a 6465 7073 203d 202d 7272 6571 7569  ..deps = -rrequi
-00000340: 7265 6d65 6e74 732f 7079 3331 312d 646a  rements/py311-dj
-00000350: 616e 676f 3332 2e74 7874 0d0a 0d0a 5b74  ango32.txt....[t
-00000360: 6573 7465 6e76 3a70 7933 3131 2d64 6a61  estenv:py311-dja
-00000370: 6e67 6f34 305d 0d0a 6465 7073 203d 202d  ngo40]..deps = -
-00000380: 7272 6571 7569 7265 6d65 6e74 732f 7079  rrequirements/py
-00000390: 3331 312d 646a 616e 676f 3430 2e74 7874  311-django40.txt
-000003a0: 0d0a                                     ..
+00000000: 5b74 6f78 5d0a 6973 6f6c 6174 6564 5f62  [tox].isolated_b
+00000010: 7569 6c64 203d 2054 7275 650a 656e 766c  uild = True.envl
+00000020: 6973 7420 3d0a 2020 2020 7079 3338 2d64  ist =.    py38-d
+00000030: 6a61 6e67 6f7b 3332 2c34 327d 0a20 2020  jango{32,42}.   
+00000040: 2070 7933 392d 646a 616e 676f 7b33 322c   py39-django{32,
+00000050: 3432 7d0a 2020 2020 7079 3331 302d 646a  42}.    py310-dj
+00000060: 616e 676f 7b33 322c 3432 7d0a 2020 2020  ango{32,42}.    
+00000070: 7079 3331 312d 646a 616e 676f 7b33 322c  py311-django{32,
+00000080: 3432 7d0a 0a5b 7465 7374 656e 765d 0a63  42}..[testenv].c
+00000090: 6f6d 6d61 6e64 7320 3d20 7079 7468 6f6e  ommands = python
+000000a0: 202d 5720 6572 726f 723a 3a44 6570 7265   -W error::Depre
+000000b0: 6361 7469 6f6e 5761 726e 696e 6720 2d57  cationWarning -W
+000000c0: 2065 7272 6f72 3a3a 5065 6e64 696e 6744   error::PendingD
+000000d0: 6570 7265 6361 7469 6f6e 5761 726e 696e  eprecationWarnin
+000000e0: 6720 2d6d 2063 6f76 6572 6167 6520 7275  g -m coverage ru
+000000f0: 6e20 2d2d 7061 7261 6c6c 656c 202d 6d20  n --parallel -m 
+00000100: 7079 7465 7374 207b 706f 7361 7267 733a  pytest {posargs:
+00000110: 7465 7374 737d 0a0a 5b74 6573 7465 6e76  tests}..[testenv
+00000120: 3a70 7933 382d 646a 616e 676f 3332 5d0a  :py38-django32].
+00000130: 6465 7073 203d 202d 7272 6571 7569 7265  deps = -rrequire
+00000140: 6d65 6e74 732f 7079 3338 2d64 6a61 6e67  ments/py38-djang
+00000150: 6f33 322e 7478 740a 0a5b 7465 7374 656e  o32.txt..[testen
+00000160: 763a 7079 3338 2d64 6a61 6e67 6f34 325d  v:py38-django42]
+00000170: 0a64 6570 7320 3d20 2d72 7265 7175 6972  .deps = -rrequir
+00000180: 656d 656e 7473 2f70 7933 382d 646a 616e  ements/py38-djan
+00000190: 676f 3432 2e74 7874 0a0a 5b74 6573 7465  go42.txt..[teste
+000001a0: 6e76 3a70 7933 392d 646a 616e 676f 3332  nv:py39-django32
+000001b0: 5d0a 6465 7073 203d 202d 7272 6571 7569  ].deps = -rrequi
+000001c0: 7265 6d65 6e74 732f 7079 3339 2d64 6a61  rements/py39-dja
+000001d0: 6e67 6f33 322e 7478 740a 0a5b 7465 7374  ngo32.txt..[test
+000001e0: 656e 763a 7079 3339 2d64 6a61 6e67 6f34  env:py39-django4
+000001f0: 325d 0a64 6570 7320 3d20 2d72 7265 7175  2].deps = -rrequ
+00000200: 6972 656d 656e 7473 2f70 7933 392d 646a  irements/py39-dj
+00000210: 616e 676f 3432 2e74 7874 0a0a 5b74 6573  ango42.txt..[tes
+00000220: 7465 6e76 3a70 7933 3130 2d64 6a61 6e67  tenv:py310-djang
+00000230: 6f33 325d 0a64 6570 7320 3d20 2d72 7265  o32].deps = -rre
+00000240: 7175 6972 656d 656e 7473 2f70 7933 3130  quirements/py310
+00000250: 2d64 6a61 6e67 6f33 322e 7478 740a 0a5b  -django32.txt..[
+00000260: 7465 7374 656e 763a 7079 3331 302d 646a  testenv:py310-dj
+00000270: 616e 676f 3432 5d0a 6465 7073 203d 202d  ango42].deps = -
+00000280: 7272 6571 7569 7265 6d65 6e74 732f 7079  rrequirements/py
+00000290: 3331 302d 646a 616e 676f 3432 2e74 7874  310-django42.txt
+000002a0: 0a0a 5b74 6573 7465 6e76 3a70 7933 3131  ..[testenv:py311
+000002b0: 2d64 6a61 6e67 6f33 325d 0a64 6570 7320  -django32].deps 
+000002c0: 3d20 2d72 7265 7175 6972 656d 656e 7473  = -rrequirements
+000002d0: 2f70 7933 3131 2d64 6a61 6e67 6f33 322e  /py311-django32.
+000002e0: 7478 740a 0a5b 7465 7374 656e 763a 7079  txt..[testenv:py
+000002f0: 3331 312d 646a 616e 676f 3432 5d0a 6465  311-django42].de
+00000300: 7073 203d 202d 7272 6571 7569 7265 6d65  ps = -rrequireme
+00000310: 6e74 732f 7079 3331 312d 646a 616e 676f  nts/py311-django
+00000320: 3432 2e74 7874 0a                        42.txt.
```

