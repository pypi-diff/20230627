# Comparing `tmp/deezer_oauth_cli-0.4.0.tar.gz` & `tmp/deezer_oauth_cli-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deezer_oauth_cli-0.4.0.tar", max compression
+gzip compressed data, was "deezer_oauth_cli-1.0.0.tar", max compression
```

## Comparing `deezer_oauth_cli-0.4.0.tar` & `deezer_oauth_cli-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1068 2022-11-20 19:19:08.964916 deezer_oauth_cli-0.4.0/LICENSE
--rw-r--r--   0        0        0     5314 2022-11-20 19:19:08.964916 deezer_oauth_cli-0.4.0/README.md
--rw-r--r--   0        0        0     2157 2022-11-20 19:19:09.744913 deezer_oauth_cli-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       22 2022-11-20 19:19:09.700913 deezer_oauth_cli-0.4.0/src/deezer_oauth/__init__.py
--rw-r--r--   0        0        0     1821 2022-11-20 19:19:08.968916 deezer_oauth_cli-0.4.0/src/deezer_oauth/client.py
--rw-r--r--   0        0        0      115 2022-11-20 19:19:08.968916 deezer_oauth_cli-0.4.0/src/deezer_oauth/constants.py
--rw-r--r--   0        0        0     1003 2022-11-20 19:19:08.968916 deezer_oauth_cli-0.4.0/src/deezer_oauth/files.py
--rw-r--r--   0        0        0     1043 2022-11-20 19:19:08.968916 deezer_oauth_cli-0.4.0/src/deezer_oauth/main.py
--rw-r--r--   0        0        0        0 2022-11-20 19:19:08.968916 deezer_oauth_cli-0.4.0/src/deezer_oauth/py.typed
--rw-r--r--   0        0        0     3238 2022-11-20 19:19:08.968916 deezer_oauth_cli-0.4.0/src/deezer_oauth/server.py
--rw-r--r--   0        0        0     6322 1970-01-01 00:00:00.000000 deezer_oauth_cli-0.4.0/setup.py
--rw-r--r--   0        0        0     6682 1970-01-01 00:00:00.000000 deezer_oauth_cli-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-27 11:38:19.540667 deezer_oauth_cli-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5350 2023-06-27 11:38:19.540667 deezer_oauth_cli-1.0.0/README.md
+-rw-r--r--   0        0        0     2253 2023-06-27 11:38:20.592685 deezer_oauth_cli-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-27 11:38:20.564685 deezer_oauth_cli-1.0.0/src/deezer_oauth/__init__.py
+-rw-r--r--   0        0        0     1833 2023-06-27 11:38:19.540667 deezer_oauth_cli-1.0.0/src/deezer_oauth/client.py
+-rw-r--r--   0        0        0      115 2023-06-27 11:38:19.540667 deezer_oauth_cli-1.0.0/src/deezer_oauth/constants.py
+-rw-r--r--   0        0        0     1003 2023-06-27 11:38:19.544667 deezer_oauth_cli-1.0.0/src/deezer_oauth/files.py
+-rw-r--r--   0        0        0     1043 2023-06-27 11:38:19.544667 deezer_oauth_cli-1.0.0/src/deezer_oauth/main.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:38:19.544667 deezer_oauth_cli-1.0.0/src/deezer_oauth/py.typed
+-rw-r--r--   0        0        0     3238 2023-06-27 11:38:19.544667 deezer_oauth_cli-1.0.0/src/deezer_oauth/server.py
+-rw-r--r--   0        0        0     6781 1970-01-01 00:00:00.000000 deezer_oauth_cli-1.0.0/PKG-INFO
```

### Comparing `deezer_oauth_cli-0.4.0/LICENSE` & `deezer_oauth_cli-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-0.4.0/README.md` & `deezer_oauth_cli-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Deezer OAuth CLI
 
 <p align="center">
-  <a href="https://github.com/browniebroke/deezer-oauth-cli/actions?query=workflow%3ACI">
-    <img src="https://img.shields.io/github/workflow/status/browniebroke/deezer-oauth-cli/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >
+  <a href="https://github.com/browniebroke/deezer-oauth-cli/actions/workflows/ci.yml?query=branch%3Amain">
+    <img src="https://img.shields.io/github/actions/workflow/status/browniebroke/deezer-oauth-cli/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >
   </a>
   <a href="https://codecov.io/gh/browniebroke/deezer-oauth-cli">
     <img src="https://img.shields.io/codecov/c/github/browniebroke/deezer-oauth-cli.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
   </a>
 </p>
 <p align="center">
   <a href="https://python-poetry.org/">
```

### Comparing `deezer_oauth_cli-0.4.0/pyproject.toml` & `deezer_oauth_cli-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deezer-oauth-cli"
-version = "0.4.0"
+version = "1.0.0"
 description = "A small CLI to quickly obtain an API token for Deezer API."
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/browniebroke/deezer-oauth-cli"
 documentation = "https://github.com/browniebroke/deezer-oauth-cli/blob/main/README.md"
 classifiers = [
@@ -17,30 +17,32 @@
 packages = [
     { include = "deezer_oauth", from = "src" },
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/browniebroke/deezer-oauth-cli/issues"
 "Changelog" = "https://github.com/browniebroke/deezer-oauth-cli/blob/main/CHANGELOG.md"
+"Twitter" = "https://twitter.com/_BrunoAlla"
+"Mastodon" = "https://fosstodon.org/@browniebroke"
 
 [tool.poetry.scripts]
 deezer-oauth = "deezer_oauth.main:app"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 requests = "^2.27"
 rich = ">=10"
-typer = {extras = ["all"], version = "^0.7.0"}
+typer = {extras = ["all"], version = "^0.9.0"}
 
 [tool.poetry.group.dev.dependencies]
 pyfakefs = "^5.0"
 pytest = "^7.0"
 pytest-cov = "^4.0"
 pytest-mock = "^3.6"
-responses = "^0.22.0"
+responses = "^0.23.0"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/deezer_oauth/__init__.py:__version__"
 build_command = "pip install poetry && poetry build"
```

### Comparing `deezer_oauth_cli-0.4.0/src/deezer_oauth/client.py` & `deezer_oauth_cli-1.0.0/src/deezer_oauth/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,12 +45,12 @@
             {
                 "app_id": self.app_id,
                 "secret": self.app_secret,
                 "code": code,
             }
         )
         url = f"{self.base_url}/oauth/access_token.php?{query}"
-        response = requests.get(url)
+        response = requests.get(url, timeout=10)
         content = response.content.decode()
         # The body looks like this: 'access_token=blah&expires=1234'
         # -> parse this as querystring and convert to a dictionary
         return dict(parse_qsl(content))
```

### Comparing `deezer_oauth_cli-0.4.0/src/deezer_oauth/files.py` & `deezer_oauth_cli-1.0.0/src/deezer_oauth/files.py`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-0.4.0/src/deezer_oauth/main.py` & `deezer_oauth_cli-1.0.0/src/deezer_oauth/main.py`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-0.4.0/src/deezer_oauth/server.py` & `deezer_oauth_cli-1.0.0/src/deezer_oauth/server.py`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-0.4.0/setup.py` & `deezer_oauth_cli-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,121 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: deezer-oauth-cli
+Version: 1.0.0
+Summary: A small CLI to quickly obtain an API token for Deezer API.
+Home-page: https://github.com/browniebroke/deezer-oauth-cli
+License: MIT
+Author: Bruno Alla
+Author-email: alla.brunoo@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: requests (>=2.27,<3.0)
+Requires-Dist: rich (>=10)
+Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Project-URL: Bug Tracker, https://github.com/browniebroke/deezer-oauth-cli/issues
+Project-URL: Changelog, https://github.com/browniebroke/deezer-oauth-cli/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://github.com/browniebroke/deezer-oauth-cli/blob/main/README.md
+Project-URL: Mastodon, https://fosstodon.org/@browniebroke
+Project-URL: Repository, https://github.com/browniebroke/deezer-oauth-cli
+Project-URL: Twitter, https://twitter.com/_BrunoAlla
+Description-Content-Type: text/markdown
+
+# Deezer OAuth CLI
+
+<p align="center">
+  <a href="https://github.com/browniebroke/deezer-oauth-cli/actions/workflows/ci.yml?query=branch%3Amain">
+    <img src="https://img.shields.io/github/actions/workflow/status/browniebroke/deezer-oauth-cli/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >
+  </a>
+  <a href="https://codecov.io/gh/browniebroke/deezer-oauth-cli">
+    <img src="https://img.shields.io/codecov/c/github/browniebroke/deezer-oauth-cli.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
+  </a>
+</p>
+<p align="center">
+  <a href="https://python-poetry.org/">
+    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">
+  </a>
+  <a href="https://github.com/ambv/black">
+    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">
+  </a>
+  <a href="https://github.com/pre-commit/pre-commit">
+    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">
+  </a>
+</p>
+<p align="center">
+  <a href="https://pypi.org/project/deezer-oauth-cli/">
+    <img src="https://img.shields.io/pypi/v/deezer-oauth-cli.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
+  </a>
+  <img src="https://img.shields.io/pypi/pyversions/deezer-oauth-cli.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
+  <img src="https://img.shields.io/pypi/l/deezer-oauth-cli.svg?style=flat-square" alt="License">
+</p>
+
+A small CLI to quickly obtain an API token for the Deezer API.
+
+Obtaining API token to develop API applications can be complicated and sometimes feel like a chicken and egg situation: it's hard to play with the API without a token, but it can be difficult to get a token without an application to do the OAuth flow.
+
+Given the app ID and secret, this tool lets you quickly get an API token.
+
+## Installation
+
+Install this via pip (or your favourite package manager):
+
+`pip install deezer-oauth-cli`
+
+## Usage
+
+Before starting to use this tool, you first need to declare your Deezer app in [their developer portal](https://developers.deezer.com). Create a new app with the following Redirect URL: `http://localhost:8080/oauth/return`.
+
+Once created, Deezer will generate an application ID and secret key for you, that's the 2 parameters that you need to run this tool:
+
+```shell
+$ deezer-oauth APP_ID APP_SECRET
+```
+
+This will:
+
+- Spin up a webserver in the background running at `http://localhost:8080`.
+- Open your browser to grant authorisation access to your Deezer account.
+- Redirect to a page showing the API token & expiry.
+- Write the token to a `.env` file.
+
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- prettier-ignore-start -->
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center"><a href="https://browniebroke.com/"><img src="https://avatars.githubusercontent.com/u/861044?v=4?s=80" width="80px;" alt="Bruno Alla"/><br /><sub><b>Bruno Alla</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-oauth-cli/commits?author=browniebroke" title="Code">💻</a> <a href="#ideas-browniebroke" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/browniebroke/deezer-oauth-cli/commits?author=browniebroke" title="Documentation">📖</a></td>
+      <td align="center"><a href="https://github.com/prndrbr"><img src="https://avatars.githubusercontent.com/u/96344856?v=4?s=80" width="80px;" alt="Pierre"/><br /><sub><b>Pierre</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-oauth-cli/commits?author=prndrbr" title="Code">💻</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+<!-- prettier-ignore-end -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
+## Credits
+
+This package was created with
+[Cookiecutter](https://github.com/audreyr/cookiecutter) and the
+[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)
+project template.
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['deezer_oauth']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['requests>=2.27,<3.0', 'rich>=10', 'typer[all]>=0.7.0,<0.8.0']
-
-entry_points = \
-{'console_scripts': ['deezer-oauth = deezer_oauth.main:app']}
-
-setup_kwargs = {
-    'name': 'deezer-oauth-cli',
-    'version': '0.4.0',
-    'description': 'A small CLI to quickly obtain an API token for Deezer API.',
-    'long_description': '# Deezer OAuth CLI\n\n<p align="center">\n  <a href="https://github.com/browniebroke/deezer-oauth-cli/actions?query=workflow%3ACI">\n    <img src="https://img.shields.io/github/workflow/status/browniebroke/deezer-oauth-cli/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://codecov.io/gh/browniebroke/deezer-oauth-cli">\n    <img src="https://img.shields.io/codecov/c/github/browniebroke/deezer-oauth-cli.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/deezer-oauth-cli/">\n    <img src="https://img.shields.io/pypi/v/deezer-oauth-cli.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/deezer-oauth-cli.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/deezer-oauth-cli.svg?style=flat-square" alt="License">\n</p>\n\nA small CLI to quickly obtain an API token for the Deezer API.\n\nObtaining API token to develop API applications can be complicated and sometimes feel like a chicken and egg situation: it\'s hard to play with the API without a token, but it can be difficult to get a token without an application to do the OAuth flow.\n\nGiven the app ID and secret, this tool lets you quickly get an API token.\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install deezer-oauth-cli`\n\n## Usage\n\nBefore starting to use this tool, you first need to declare your Deezer app in [their developer portal](https://developers.deezer.com). Create a new app with the following Redirect URL: `http://localhost:8080/oauth/return`.\n\nOnce created, Deezer will generate an application ID and secret key for you, that\'s the 2 parameters that you need to run this tool:\n\n```shell\n$ deezer-oauth APP_ID APP_SECRET\n```\n\nThis will:\n\n- Spin up a webserver in the background running at `http://localhost:8080`.\n- Open your browser to grant authorisation access to your Deezer account.\n- Redirect to a page showing the API token & expiry.\n- Write the token to a `.env` file.\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tbody>\n    <tr>\n      <td align="center"><a href="https://browniebroke.com/"><img src="https://avatars.githubusercontent.com/u/861044?v=4?s=80" width="80px;" alt="Bruno Alla"/><br /><sub><b>Bruno Alla</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-oauth-cli/commits?author=browniebroke" title="Code">💻</a> <a href="#ideas-browniebroke" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/browniebroke/deezer-oauth-cli/commits?author=browniebroke" title="Documentation">📖</a></td>\n      <td align="center"><a href="https://github.com/prndrbr"><img src="https://avatars.githubusercontent.com/u/96344856?v=4?s=80" width="80px;" alt="Pierre"/><br /><sub><b>Pierre</b></sub></a><br /><a href="https://github.com/browniebroke/deezer-oauth-cli/commits?author=prndrbr" title="Code">💻</a></td>\n    </tr>\n  </tbody>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject template.\n',
-    'author': 'Bruno Alla',
-    'author_email': 'alla.brunoo@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/browniebroke/deezer-oauth-cli',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,44 +1,48 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['deezer_oauth'] package_data = \ {'': ['*']}
-install_requires = \ ['requests>=2.27,<3.0', 'rich>=10', 'typer
-[all]>=0.7.0,<0.8.0'] entry_points = \ {'console_scripts': ['deezer-oauth =
-deezer_oauth.main:app']} setup_kwargs = { 'name': 'deezer-oauth-cli',
-'version': '0.4.0', 'description': 'A small CLI to quickly obtain an API token
-for Deezer API.', 'long_description': '# Deezer OAuth CLI\n\n
-            \n \n_[CI_Status]\n\n \n_[Test_coverage_percentage]\n\n
-\n
-             \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
-\n
-      \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
-\n\nA small CLI to quickly obtain an API token for the Deezer API.\n\nObtaining
-API token to develop API applications can be complicated and sometimes feel
-like a chicken and egg situation: it\'s hard to play with the API without a
-token, but it can be difficult to get a token without an application to do the
-OAuth flow.\n\nGiven the app ID and secret, this tool lets you quickly get an
-API token.\n\n## Installation\n\nInstall this via pip (or your favourite
-package manager):\n\n`pip install deezer-oauth-cli`\n\n## Usage\n\nBefore
-starting to use this tool, you first need to declare your Deezer app in [their
-developer portal](https://developers.deezer.com). Create a new app with the
-following Redirect URL: `http://localhost:8080/oauth/return`.\n\nOnce created,
-Deezer will generate an application ID and secret key for you, that\'s the 2
-parameters that you need to run this tool:\n\n```shell\n$ deezer-oauth APP_ID
-APP_SECRET\n```\n\nThis will:\n\n- Spin up a webserver in the background
-running at `http://localhost:8080`.\n- Open your browser to grant authorisation
-access to your Deezer account.\n- Redirect to a page showing the API token &
-expiry.\n- Write the token to a `.env` file.\n\n## Contributors â¨\n\nThanks
-goes to these wonderful people ([emoji key](https://allcontributors.org/docs/
-en/emoji-key)):\n\n\n\n\n\n
+Metadata-Version: 2.1 Name: deezer-oauth-cli Version: 1.0.0 Summary: A small
+CLI to quickly obtain an API token for Deezer API. Home-page: https://
+github.com/browniebroke/deezer-oauth-cli License: MIT Author: Bruno Alla
+Author-email: alla.brunoo@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
+Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
+:: English Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Software Development :: Libraries Requires-
+Dist: requests (>=2.27,<3.0) Requires-Dist: rich (>=10) Requires-Dist: typer
+[all] (>=0.9.0,<0.10.0) Project-URL: Bug Tracker, https://github.com/
+browniebroke/deezer-oauth-cli/issues Project-URL: Changelog, https://
+github.com/browniebroke/deezer-oauth-cli/blob/main/CHANGELOG.md Project-URL:
+Documentation, https://github.com/browniebroke/deezer-oauth-cli/blob/main/
+README.md Project-URL: Mastodon, https://fosstodon.org/@browniebroke Project-
+URL: Repository, https://github.com/browniebroke/deezer-oauth-cli Project-URL:
+Twitter, https://twitter.com/_BrunoAlla Description-Content-Type: text/markdown
+# Deezer OAuth CLI
+                    [CI_Status] [Test_coverage_percentage]
+                         [Poetry] [black] [pre-commit]
+             [PyPI_Version] [Supported Python versions] [License]
+A small CLI to quickly obtain an API token for the Deezer API. Obtaining API
+token to develop API applications can be complicated and sometimes feel like a
+chicken and egg situation: it's hard to play with the API without a token, but
+it can be difficult to get a token without an application to do the OAuth flow.
+Given the app ID and secret, this tool lets you quickly get an API token. ##
+Installation Install this via pip (or your favourite package manager): `pip
+install deezer-oauth-cli` ## Usage Before starting to use this tool, you first
+need to declare your Deezer app in [their developer portal](https://
+developers.deezer.com). Create a new app with the following Redirect URL:
+`http://localhost:8080/oauth/return`. Once created, Deezer will generate an
+application ID and secret key for you, that's the 2 parameters that you need to
+run this tool: ```shell $ deezer-oauth APP_ID APP_SECRET ``` This will: - Spin
+up a webserver in the background running at `http://localhost:8080`. - Open
+your browser to grant authorisation access to your Deezer account. - Redirect
+to a page showing the API token & expiry. - Write the token to a `.env` file.
+## Contributors â¨ Thanks goes to these wonderful people ([emoji key](https://
+allcontributors.org/docs/en/emoji-key)):
        [Bruno_Alla]        [Pierre]
         Bruno_Alla          Pierre
       ð» ð¤ ð�  ð»
-\n\n\n\n\n\n\n\nThis project follows the [all-contributors](https://github.com/
-all-contributors/all-contributors) specification. Contributions of any kind
-welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https:/
-/github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-
-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject
-template.\n', 'author': 'Bruno Alla', 'author_email': 'alla.brunoo@gmail.com',
-'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://github.com/
-browniebroke/deezer-oauth-cli', 'package_dir': package_dir, 'packages':
-packages, 'package_data': package_data, 'install_requires': install_requires,
-'entry_points': entry_points, 'python_requires': '>=3.7,<4.0', } setup
-(**setup_kwargs)
+    This project follows the [all-contributors](https://github.com/all-
+contributors/all-contributors) specification. Contributions of any kind
+welcome! ## Credits This package was created with [Cookiecutter](https://
+github.com/audreyr/cookiecutter) and the [browniebroke/cookiecutter-pypackage]
+(https://github.com/browniebroke/cookiecutter-pypackage) project template.
```

