# Comparing `tmp/starlette_csrf-2.0.0.tar.gz` & `tmp/starlette_csrf-3.0.0.tar.gz`

## Comparing `starlette_csrf-2.0.0.tar` & `starlette_csrf-3.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 starlette_csrf-2.0.0/.editorconfig
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 starlette_csrf-2.0.0/.github/FUNDING.yml
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 starlette_csrf-2.0.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 starlette_csrf-2.0.0/starlette_csrf/__init__.py
--rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 starlette_csrf-2.0.0/starlette_csrf/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_csrf-2.0.0/starlette_csrf/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_csrf-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 starlette_csrf-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 starlette_csrf-2.0.0/tests/test_middleware.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 starlette_csrf-2.0.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 starlette_csrf-2.0.0/LICENSE
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 starlette_csrf-2.0.0/README.md
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 starlette_csrf-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 starlette_csrf-2.0.0/PKG-INFO
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 starlette_csrf-2.0.0/setup.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 starlette_csrf-3.0.0/.editorconfig
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 starlette_csrf-3.0.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 starlette_csrf-3.0.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 starlette_csrf-3.0.0/starlette_csrf/__init__.py
+-rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 starlette_csrf-3.0.0/starlette_csrf/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_csrf-3.0.0/starlette_csrf/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_csrf-3.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 starlette_csrf-3.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 starlette_csrf-3.0.0/tests/test_middleware.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 starlette_csrf-3.0.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 starlette_csrf-3.0.0/LICENSE
+-rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 starlette_csrf-3.0.0/README.md
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 starlette_csrf-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5944 2020-02-02 00:00:00.000000 starlette_csrf-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 starlette_csrf-3.0.0/setup.py
```

### Comparing `starlette_csrf-2.0.0/.github/workflows/build.yml` & `starlette_csrf-3.0.0/.github/workflows/build.yml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 jobs:
   test:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python_version: [3.7, 3.8, 3.9, '3.10', '3.11']
+        python_version: [3.8, 3.9, '3.10', '3.11']
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python_version }}
@@ -39,15 +39,15 @@
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

### Comparing `starlette_csrf-2.0.0/starlette_csrf/middleware.py` & `starlette_csrf-3.0.0/starlette_csrf/middleware.py`

 * *Files identical despite different names*

### Comparing `starlette_csrf-2.0.0/tests/test_middleware.py` & `starlette_csrf-3.0.0/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `starlette_csrf-2.0.0/.gitignore` & `starlette_csrf-3.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `starlette_csrf-2.0.0/LICENSE` & `starlette_csrf-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette_csrf-2.0.0/README.md` & `starlette_csrf-3.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 ```bash
 hatch run test
 ```
 
 ### Format the code
 
-Execute the following command to apply `isort` and `black` formatting:
+Execute the following command to apply linting and check typing:
 
 ```bash
 hatch run lint
 ```
 
 ## License
```

### Comparing `starlette_csrf-2.0.0/pyproject.toml` & `starlette_csrf-3.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -57,23 +57,22 @@
 readme = "README.md"
 dynamic = ["version"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Development Status :: 5 - Production/Stable",
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
     "itsdangerous >=2.0.1,<3.0.0",
     "starlette >=0.14.2"
 ]
 
 [project.urls]
 Documentation = "https://github.com/frankie567/starlette-csrf"
```

### Comparing `starlette_csrf-2.0.0/PKG-INFO` & `starlette_csrf-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: starlette-csrf
-Version: 2.0.0
+Version: 3.0.0
 Summary: Starlette middleware implementing Double Submit Cookie technique to mitigate CSRF
 Project-URL: Documentation, https://github.com/frankie567/starlette-csrf
 Project-URL: Source, https://github.com/frankie567/starlette-csrf
 Author-email: François Voron <fvoron@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
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
 Requires-Dist: itsdangerous<3.0.0,>=2.0.1
 Requires-Dist: starlette>=0.14.2
 Description-Content-Type: text/markdown
 
 # Starlette CSRF Middleware
 
 Starlette middleware implementing Double Submit Cookie technique to mitigate CSRF.
@@ -121,15 +120,15 @@
 
 ```bash
 hatch run test
 ```
 
 ### Format the code
 
-Execute the following command to apply `isort` and `black` formatting:
+Execute the following command to apply linting and check typing:
 
 ```bash
 hatch run lint
 ```
 
 ## License
```

### Comparing `starlette_csrf-2.0.0/setup.py` & `starlette_csrf-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='starlette-csrf',
-    version='2.0.0',
+    version='3.0.0',
     description='Starlette middleware implementing Double Submit Cookie technique to mitigate CSRF',
-    long_description='# Starlette CSRF Middleware\n\nStarlette middleware implementing Double Submit Cookie technique to mitigate CSRF.\n\n[![build](https://github.com/frankie567/starlette-csrf/workflows/Build/badge.svg)](https://github.com/frankie567/starlette-csrf/actions)\n[![codecov](https://codecov.io/gh/frankie567/starlette-csrf/branch/main/graph/badge.svg?token=fL49kIvrj6)](https://codecov.io/gh/frankie567/starlette-csrf)\n[![PyPI version](https://badge.fury.io/py/starlette-csrf.svg)](https://badge.fury.io/py/starlette-csrf)\n[![Downloads](https://pepy.tech/badge/starlette-csrf)](https://pepy.tech/project/starlette-csrf)\n\n<p align="center">\n<a href="https://github.com/sponsors/frankie567"><img src="https://md-buttons.francoisvoron.com/button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50"></a>\n</p>\n\n## How it works?\n\n1. The user makes a first request with a method considered safe (by default `GET`, `HEAD`, `OPTIONS`, `TRACE`).\n2. It receives in response a cookie (named by default `csrftoken`) which contains a secret value.\n3. When the user wants to make an unsafe request, the server expects them to send the same secret value in a header (named by default `x-csrftoken`).\n4. The middleware will then compare the secret value provided in the cookie and the header.\n   * If they match, the request is processed.\n   * Otherwise, a `403 Forbidden` error response is given.\n\nThis mechanism is necessary if you rely on cookie authentication in a browser. You can have more information about CSRF and Double Submit Cookie in the [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html).\n\n## Installation\n\n```bash\npip install starlette-csrf\n```\n\n## Usage with Starlette\n\n```py\nfrom starlette.applications import Starlette\nfrom starlette.middleware import Middleware\nfrom starlette_csrf import CSRFMiddleware\n\nroutes = ...\n\nmiddleware = [\n    Middleware(CSRFMiddleware, secret="__CHANGE_ME__")\n]\n\napp = Starlette(routes=routes, middleware=middleware)\n```\n\n## Usage with FastAPI\n\n```py\nfrom fastapi import FastAPI\nfrom starlette_csrf import CSRFMiddleware\n\napp = FastAPI()\n\napp.add_middleware(CSRFMiddleware, secret="__CHANGE_ME__")\n```\n\n## Arguments\n\n* `secret` (`str`): Secret to sign the CSRF token value. **Be sure to choose a strong passphrase and keep it SECRET**.\n* `required_urls` (`Optional[List[re.Pattern]]` - `None`): List of URL regexes that the CSRF check should **always** be enforced, no matter the method or the cookies present.\n* `exempt_urls` (`Optional[List[re.Pattern]]` - `None`): List of URL regexes that the CSRF check should be skipped on. Useful if you have any APIs that you know do not need CSRF protection.\n* `sensitive_cookies` (`Set[str]` - `None`): Set of cookie names that should trigger the CSRF check if they are present in the request. Useful if you have other authentication methods that don\'t rely on cookies and don\'t need CSRF enforcement. If this parameter is `None`, the default, CSRF is **always** enforced.\n* `safe_methods` (`Set[str]` - `{"GET", "HEAD", "OPTIONS", "TRACE"}`): HTTP methods considered safe which don\'t need CSRF protection.\n* `cookie_name` (`str` - `csrftoken`): Name of the cookie.\n* `cookie_path` `str` - `/`): Cookie path.\n* `cookie_domain` (`Optional[str]` - `None`): Cookie domain. If your frontend and API lives in different sub-domains, be sure to set this argument with your root domain to allow your frontend sub-domain to read the cookie on the JavaScript side.\n* `cookie_secure` (`bool` - `False`): Whether to only send the cookie to the server via SSL request.\n* `cookie_samesite` (`str` - `lax`): Samesite strategy of the cookie.\n* `header_name` (`str` - `x-csrftoken`): Name of the header where you should set the CSRF token.\n\n## Customize error response\n\nBy default, a plain text response with the status code 403 is returned when the CSRF verification is failing. You can customize it by overloading the middleware class and implementing the `_get_error_response` method. It accepts in argument the original `Request` object and expects a `Response`. For example:\n\n```py\nfrom starlette.requests import Request\nfrom starlette.responses import JSONResponse, Response\nfrom starlette_csrf import CSRFMiddleware\n\nclass CustomResponseCSRFMiddleware(CSRFMiddleware):\n    def _get_error_response(self, request: Request) -> Response:\n        return JSONResponse(\n            content={"code": "CSRF_ERROR"}, status_code=403\n        )\n```\n\n## Development\n\n### Setup environment\n\nWe use [Hatch](https://hatch.pypa.io/latest/install/) to manage the development environment and production build. Ensure it\'s installed on your system.\n\n### Run unit tests\n\nYou can run all the tests with:\n\n```bash\nhatch run test\n```\n\n### Format the code\n\nExecute the following command to apply `isort` and `black` formatting:\n\n```bash\nhatch run lint\n```\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n',
+    long_description='# Starlette CSRF Middleware\n\nStarlette middleware implementing Double Submit Cookie technique to mitigate CSRF.\n\n[![build](https://github.com/frankie567/starlette-csrf/workflows/Build/badge.svg)](https://github.com/frankie567/starlette-csrf/actions)\n[![codecov](https://codecov.io/gh/frankie567/starlette-csrf/branch/main/graph/badge.svg?token=fL49kIvrj6)](https://codecov.io/gh/frankie567/starlette-csrf)\n[![PyPI version](https://badge.fury.io/py/starlette-csrf.svg)](https://badge.fury.io/py/starlette-csrf)\n[![Downloads](https://pepy.tech/badge/starlette-csrf)](https://pepy.tech/project/starlette-csrf)\n\n<p align="center">\n<a href="https://github.com/sponsors/frankie567"><img src="https://md-buttons.francoisvoron.com/button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50"></a>\n</p>\n\n## How it works?\n\n1. The user makes a first request with a method considered safe (by default `GET`, `HEAD`, `OPTIONS`, `TRACE`).\n2. It receives in response a cookie (named by default `csrftoken`) which contains a secret value.\n3. When the user wants to make an unsafe request, the server expects them to send the same secret value in a header (named by default `x-csrftoken`).\n4. The middleware will then compare the secret value provided in the cookie and the header.\n   * If they match, the request is processed.\n   * Otherwise, a `403 Forbidden` error response is given.\n\nThis mechanism is necessary if you rely on cookie authentication in a browser. You can have more information about CSRF and Double Submit Cookie in the [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html).\n\n## Installation\n\n```bash\npip install starlette-csrf\n```\n\n## Usage with Starlette\n\n```py\nfrom starlette.applications import Starlette\nfrom starlette.middleware import Middleware\nfrom starlette_csrf import CSRFMiddleware\n\nroutes = ...\n\nmiddleware = [\n    Middleware(CSRFMiddleware, secret="__CHANGE_ME__")\n]\n\napp = Starlette(routes=routes, middleware=middleware)\n```\n\n## Usage with FastAPI\n\n```py\nfrom fastapi import FastAPI\nfrom starlette_csrf import CSRFMiddleware\n\napp = FastAPI()\n\napp.add_middleware(CSRFMiddleware, secret="__CHANGE_ME__")\n```\n\n## Arguments\n\n* `secret` (`str`): Secret to sign the CSRF token value. **Be sure to choose a strong passphrase and keep it SECRET**.\n* `required_urls` (`Optional[List[re.Pattern]]` - `None`): List of URL regexes that the CSRF check should **always** be enforced, no matter the method or the cookies present.\n* `exempt_urls` (`Optional[List[re.Pattern]]` - `None`): List of URL regexes that the CSRF check should be skipped on. Useful if you have any APIs that you know do not need CSRF protection.\n* `sensitive_cookies` (`Set[str]` - `None`): Set of cookie names that should trigger the CSRF check if they are present in the request. Useful if you have other authentication methods that don\'t rely on cookies and don\'t need CSRF enforcement. If this parameter is `None`, the default, CSRF is **always** enforced.\n* `safe_methods` (`Set[str]` - `{"GET", "HEAD", "OPTIONS", "TRACE"}`): HTTP methods considered safe which don\'t need CSRF protection.\n* `cookie_name` (`str` - `csrftoken`): Name of the cookie.\n* `cookie_path` `str` - `/`): Cookie path.\n* `cookie_domain` (`Optional[str]` - `None`): Cookie domain. If your frontend and API lives in different sub-domains, be sure to set this argument with your root domain to allow your frontend sub-domain to read the cookie on the JavaScript side.\n* `cookie_secure` (`bool` - `False`): Whether to only send the cookie to the server via SSL request.\n* `cookie_samesite` (`str` - `lax`): Samesite strategy of the cookie.\n* `header_name` (`str` - `x-csrftoken`): Name of the header where you should set the CSRF token.\n\n## Customize error response\n\nBy default, a plain text response with the status code 403 is returned when the CSRF verification is failing. You can customize it by overloading the middleware class and implementing the `_get_error_response` method. It accepts in argument the original `Request` object and expects a `Response`. For example:\n\n```py\nfrom starlette.requests import Request\nfrom starlette.responses import JSONResponse, Response\nfrom starlette_csrf import CSRFMiddleware\n\nclass CustomResponseCSRFMiddleware(CSRFMiddleware):\n    def _get_error_response(self, request: Request) -> Response:\n        return JSONResponse(\n            content={"code": "CSRF_ERROR"}, status_code=403\n        )\n```\n\n## Development\n\n### Setup environment\n\nWe use [Hatch](https://hatch.pypa.io/latest/install/) to manage the development environment and production build. Ensure it\'s installed on your system.\n\n### Run unit tests\n\nYou can run all the tests with:\n\n```bash\nhatch run test\n```\n\n### Format the code\n\nExecute the following command to apply linting and check typing:\n\n```bash\nhatch run lint\n```\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n',
     author_email='François Voron <fvoron@gmail.com>',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Framework :: AsyncIO',
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
 # -*- coding: utf-8 -*- from setuptools import setup setup( name='starlette-
-csrf', version='2.0.0', description='Starlette middleware implementing Double
+csrf', version='3.0.0', description='Starlette middleware implementing Double
 Submit Cookie technique to mitigate CSRF', long_description='# Starlette CSRF
 Middleware\n\nStarlette middleware implementing Double Submit Cookie technique
 to mitigate CSRF.\n\n[![build](https://github.com/frankie567/starlette-csrf/
 workflows/Build/badge.svg)](https://github.com/frankie567/starlette-csrf/
 actions)\n[![codecov](https://codecov.io/gh/frankie567/starlette-csrf/branch/
 main/graph/badge.svg?token=fL49kIvrj6)](https://codecov.io/gh/frankie567/
 starlette-csrf)\n[![PyPI version](https://badge.fury.io/py/starlette-csrf.svg)]
@@ -61,18 +61,18 @@
 CSRFMiddleware\n\nclass CustomResponseCSRFMiddleware(CSRFMiddleware):\n def
 _get_error_response(self, request: Request) -> Response:\n return JSONResponse
 (\n content={"code": "CSRF_ERROR"}, status_code=403\n )\n```\n\n##
 Development\n\n### Setup environment\n\nWe use [Hatch](https://hatch.pypa.io/
 latest/install/) to manage the development environment and production build.
 Ensure it\'s installed on your system.\n\n### Run unit tests\n\nYou can run all
 the tests with:\n\n```bash\nhatch run test\n```\n\n### Format the
-code\n\nExecute the following command to apply `isort` and `black` formatting:
+code\n\nExecute the following command to apply linting and check typing:
 \n\n```bash\nhatch run lint\n```\n\n## License\n\nThis project is licensed
 under the terms of the MIT license.\n', author_email='FranÃ§ois Voron
 gmail.com>', classifiers=[ 'Development Status :: 5 - Production/Stable',
 'Framework :: AsyncIO', 'Intended Audience :: Developers', 'License :: OSI
 Approved :: MIT License', 'Programming Language :: Python :: 3 :: Only',
-'Programming Language :: Python :: 3.7', 'Programming Language :: Python ::
-3.8', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python
-:: 3.10', 'Programming Language :: Python :: 3.11', 'Topic :: Internet :: WWW/
-HTTP :: Session', ], install_requires=[ 'itsdangerous<3.0.0,>=2.0.1',
-'starlette>=0.14.2', ], packages=[ 'starlette_csrf', 'tests', ], )
+'Programming Language :: Python :: 3.8', 'Programming Language :: Python ::
+3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python
+:: 3.11', 'Topic :: Internet :: WWW/HTTP :: Session', ], install_requires=
+[ 'itsdangerous<3.0.0,>=2.0.1', 'starlette>=0.14.2', ], packages=
+[ 'starlette_csrf', 'tests', ], )
```

