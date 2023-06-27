# Comparing `tmp/zyme-0.1.1.tar.gz` & `tmp/zyme-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyme-0.1.1.tar", last modified: Fri Jul 22 09:45:56 2022, max compression
+gzip compressed data, was "zyme-0.1.5.tar", last modified: Tue Jun 27 12:16:48 2023, max compression
```

## Comparing `zyme-0.1.1.tar` & `zyme-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxrwxrwx   0        0        0        0 2022-07-22 09:45:56.960652 zyme-0.1.1/
--rw-rw-rw-   0        0        0      163 2022-07-22 09:32:20.000000 zyme-0.1.1/AUTHORS.md
--rw-rw-rw-   0        0        0      227 2022-07-22 09:45:46.000000 zyme-0.1.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1074 2022-07-22 09:16:21.000000 zyme-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      194 2022-07-22 09:16:21.000000 zyme-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7506 2022-07-22 09:45:56.961654 zyme-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     6381 2022-07-22 09:32:26.000000 zyme-0.1.1/README.md
--rw-rw-rw-   0        0        0     2169 2022-07-22 09:16:21.000000 zyme-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0     1579 2022-07-22 09:45:56.962656 zyme-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      108 2022-07-22 09:16:21.000000 zyme-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-22 09:45:56.912654 zyme-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2022-07-22 09:45:56.950656 zyme-0.1.1/src/zyme/
--rw-rw-rw-   0        0        0     1702 2022-07-22 09:45:46.000000 zyme-0.1.1/src/zyme/__init__.py
--rw-rw-rw-   0        0        0      156 2022-07-22 09:32:20.000000 zyme-0.1.1/src/zyme/config.ini
--rw-rw-rw-   0        0        0      219 2022-07-22 09:32:26.000000 zyme-0.1.1/src/zyme/config.json
--rw-rw-rw-   0        0        0      166 2022-07-22 09:32:20.000000 zyme-0.1.1/src/zyme/config.toml
--rw-rw-rw-   0        0        0      149 2022-07-22 09:32:26.000000 zyme-0.1.1/src/zyme/config.yaml
--rw-rw-rw-   0        0        0     2601 2022-07-22 09:32:23.000000 zyme-0.1.1/src/zyme/zyme.py
--rw-rw-rw-   0        0        0      604 2022-07-22 09:16:22.000000 zyme-0.1.1/src/zyme/zyme_cli.py
-drwxrwxrwx   0        0        0        0 2022-07-22 09:45:56.959654 zyme-0.1.1/src/zyme.egg-info/
--rw-rw-rw-   0        0        0     7506 2022-07-22 09:45:56.000000 zyme-0.1.1/src/zyme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      423 2022-07-22 09:45:56.000000 zyme-0.1.1/src/zyme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-22 09:45:56.000000 zyme-0.1.1/src/zyme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2022-07-22 09:45:56.000000 zyme-0.1.1/src/zyme.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2022-07-22 09:45:56.000000 zyme-0.1.1/src/zyme.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-07-22 09:45:56.000000 zyme-0.1.1/src/zyme.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 12:16:48.042149 zyme-0.1.5/
+-rw-rw-rw-   0        0        0      161 2023-06-27 12:06:31.000000 zyme-0.1.5/AUTHORS.md
+-rw-rw-rw-   0        0        0      104 2023-06-27 12:01:28.000000 zyme-0.1.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-06-27 12:01:28.000000 zyme-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-06-27 12:01:28.000000 zyme-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     8539 2023-06-27 12:16:48.042149 zyme-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7021 2023-06-27 12:06:31.000000 zyme-0.1.5/README.md
+-rw-rw-rw-   0        0        0     2174 2023-06-27 12:01:28.000000 zyme-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0     2058 2023-06-27 12:16:48.050197 zyme-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      117 2023-06-27 12:01:28.000000 zyme-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:16:47.930524 zyme-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-27 12:16:47.991434 zyme-0.1.5/src/zyme/
+-rw-rw-rw-   0        0        0     2342 2023-06-27 12:06:27.000000 zyme-0.1.5/src/zyme/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:16:48.031992 zyme-0.1.5/src/zyme/resources/
+-rw-rw-rw-   0        0        0        0 2023-06-27 12:01:29.000000 zyme-0.1.5/src/zyme/resources/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-06-27 12:06:24.000000 zyme-0.1.5/src/zyme/resources/config.ini
+-rw-rw-rw-   0        0        0      219 2023-06-27 12:06:31.000000 zyme-0.1.5/src/zyme/resources/config.json
+-rw-rw-rw-   0        0        0      166 2023-06-27 12:06:24.000000 zyme-0.1.5/src/zyme/resources/config.toml
+-rw-rw-rw-   0        0        0      149 2023-06-27 12:06:31.000000 zyme-0.1.5/src/zyme/resources/config.yaml
+-rw-rw-rw-   0        0        0        0 2023-06-27 12:01:29.000000 zyme-0.1.5/src/zyme/resources/resource.db
+-rw-rw-rw-   0        0        0       60 2023-06-27 12:01:29.000000 zyme-0.1.5/src/zyme/resources/resource.pickle
+-rw-rw-rw-   0        0        0    14636 2023-06-27 12:01:29.000000 zyme-0.1.5/src/zyme/resources/resource.png
+-rw-rw-rw-   0        0        0     2706 2023-06-27 12:08:36.000000 zyme-0.1.5/src/zyme/zyme.py
+-rw-rw-rw-   0        0        0      619 2023-06-27 12:01:29.000000 zyme-0.1.5/src/zyme/zyme_cli.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:16:48.011773 zyme-0.1.5/src/zyme.egg-info/
+-rw-rw-rw-   0        0        0     8539 2023-06-27 12:16:47.000000 zyme-0.1.5/src/zyme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      634 2023-06-27 12:16:47.000000 zyme-0.1.5/src/zyme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 12:16:47.000000 zyme-0.1.5/src/zyme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-27 12:16:47.000000 zyme-0.1.5/src/zyme.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-06-27 12:16:47.000000 zyme-0.1.5/src/zyme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-27 12:16:47.000000 zyme-0.1.5/src/zyme.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 12:16:48.042149 zyme-0.1.5/tests/
+-rw-rw-rw-   0        0        0      935 2023-06-27 12:01:29.000000 zyme-0.1.5/tests/test_zyme.py
+-rw-rw-rw-   0        0        0     1152 2023-06-27 12:01:29.000000 zyme-0.1.5/tests/test_zyme_cli.py
```

### Comparing `zyme-0.1.1/LICENSE` & `zyme-0.1.5/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022, Stephen R A King
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
+Copyright (c) 2023, Stephen R A King
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

### Comparing `zyme-0.1.1/PKG-INFO` & `zyme-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,161 +1,184 @@
 Metadata-Version: 2.1
 Name: zyme
-Version: 0.1.1
+Version: 0.1.5
 Summary: placeholder
 Home-page: https://github.com/Stephen-RA-King/zyme
 Download-URL: https://github.com/Stephen-RA-King/zyme/archive/refs/heads/main.zip
 Author: Stephen R A King
-Author-email: stephen.ra.king@gmail.com
+Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
-Maintainer-email: stephen.ra.king@gmail.com
+Maintainer-email: sking.github@gmail.com
 License: MIT
+Project-URL: Bug Tracker, https://github.com/Stephen-RA-King/zyme/issues
+Project-URL: CI, https://github.com/Stephen-RA-King/zyme/actions
+Project-URL: Documentation, https://zyme.readthedocs.io/en/latest/
+Project-URL: Release Notes, https://github.com/Stephen-RA-King/zyme/releases
+Project-URL: Source Code, https://github.com/Stephen-RA-King/zyme/
 Keywords: utility
 Platform: Any
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: AUTHORS.md
 
 # zyme
 
 > Short blurb about what your product does.
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
-[![Format][format-image]][pypi-url]
-[![Requirements][requirements-status-image]][requirements-status-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
-[![CodeFactor][codefactor-image]][codefactor-url]
-[![Codeclimate][codeclimate-image]][codeclimate-url]
-[![Lgtm alerts][lgtm-alerts-image]][lgtm-alerts-url]
-[![Lgtm quality][lgtm-quality-image]][lgtm-quality-url]
 [![CodeQl][codeql-image]][codeql-url]
-[![readthedocs][readthedocs-image]][readthedocs-url]
+[![Docker][docker-image]][docker-url]
 [![pre-commit][pre-commit-image]][pre-commit-url]
 [![pre-commit.ci status][pre-commit.ci-image]][pre-commit.ci-url]
+[![readthedocs][readthedocs-image]][readthedocs-url]
+[![CodeFactor][codefactor-image]][codefactor-url]
+[![Codeclimate][codeclimate-image]][codeclimate-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
 [![Checked with mypy][mypy-image]][mypy-url]
 [![security: bandit][bandit-image]][bandit-url]
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
 [![license][license-image]][license-url]
+[![Pydough][pydough-image]][pydough-url]
+[![OpenSSFScorecard][openssf-image]][openssf-url]
 
 One to two paragraph statement about your product and what it does.
 
-![](assets/header.png)
+![](assets/header_dough.png)
 
 ## Installation
 
+---
+
 OS X & Linux:
 
 ```sh
 pip3 install zyme
 ```
 
 Windows:
 
 ```sh
 pip install zyme
 ```
 
 ## Usage example
 
+---
+
 A few motivating and useful examples of how your product can be used. Spice this up with code blocks and potentially more screenshots.
 
 _For more examples and usage, please refer to the [Wiki][wiki]._
 
 ## Development setup
 
+---
+
 Describe how to install all development dependencies and how to run an automated test-suite of some kind. Potentially do this for multiple platforms.
 
 ```sh
 pip install --editable zyme
 ```
 
 ## Documentation
 
-### - [**Read the Docs**](https://zyme.readthedocs.io/en/latest/)
+---
 
-### - [**Wiki**](https://github.com/Stephen-RA-King/zyme/wiki)
+[**Read the Docs**](https://zyme.readthedocs.io/en/latest/)
+
+-   [**Example Usage**](https://zyme.readthedocs.io/en/latest/example.html)
+-   [**Credits**](https://zyme.readthedocs.io/en/latest/example.html)
+-   [**Changelog**](https://zyme.readthedocs.io/en/latest/changelog.html)
+-   [**API Reference**](https://zyme.readthedocs.io/en/latest/autoapi/index.html)
+
+[**Wiki**](https://github.com/Stephen-RA-King/zyme/wiki)
 
 ## Meta
 
-[![](assets/linkedin.png)](https://linkedin.com/in/stephen-k-3a4644210)
+---
+
+[![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
-[![](assets/pypi.png)](https://pypi.org/project/zyme/)
+[![](assets/pypi.png)](https://pypi.org/project/zyme)
+[![Docker](assets/docker.png)](https://hub.docker.com/r/sraking/zyme)
 [![](assets/www.png)](https://www.justpython.tech)
-[![](assets/email.png)](mailto:stephen.ra.king@gmail.com)
-[![](assets/cv.png)](https://www.justpython.tech/cv)
+[![](assets/email.png)](mailto:sking.github@gmail.com)
+[![](assets/github.png)](https://github.com/Stephen-RA-King/zyme)
 
-Stephen R A King : stephen.ra.king@gmail.com
+Author: Stephen R A King ([sking.github@gmail.com](mailto:sking.github@gmail.com))
 
-Distributed under the MIT license. See [license](license-url) for more information.
+Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-[https://github.com/Stephen-RA-King/zyme](https://github.com/Stephen-RA-King/zyme)
+Created with Cookiecutter template: [![pydough][pydough-image]][pydough-url] version 1.3.3
 
-Created with Cookiecutter template: [**cc_template**][cc_template-url] version 1.1.1
+Digital object identifier: [![DOI](https://zenodo.org/badge/xxxxxxxxx.svg)](https://zenodo.org/badge/latestdoi/xxxxxxxxx)
 
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
-[cc_template-url]: https://github.com/Stephen-RA-King/cc_template
 [codeclimate-image]: https://api.codeclimate.com/v1/badges/7fc352185512a1dab75d/maintainability
 [codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/zyme/maintainability
 [codecov-image]: https://codecov.io/gh/Stephen-RA-King/zyme/branch/main/graph/badge.svg
 [codecov-url]: https://app.codecov.io/gh/Stephen-RA-King/zyme
 [codefactor-image]: https://www.codefactor.io/repository/github/Stephen-RA-King/zyme/badge
 [codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/zyme
-[codeql-image]: https://github.com/Stephen-RA-King/zyme/actions/workflows/codeql-analysis.yml/badge.svg
-[codeql-url]: https://github.com/Stephen-RA-King/zyme/actions/workflows/codeql-analysis.yml
+[codeql-image]: https://github.com/Stephen-RA-King/zyme/actions/workflows/github-code-scanning/codeql/badge.svg
+[codeql-url]: https://github.com/Stephen-RA-King/zyme/actions/workflows/github-code-scanning/codeql
 [commitizen-image]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
 [commitizen-url]: http://commitizen.github.io/cz-cli/
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square
 [conventional-commits-url]: https://conventionalcommits.org
 [deepsource-image]: https://static.deepsource.io/deepsource-badge-light-mini.svg
 [deepsource-url]: https://deepsource.io/gh/Stephen-RA-King/zyme/?ref=repository-badge
+[docker-image]: https://github.com/Stephen-RA-King/zyme/actions/workflows/docker-image.yml/badge.svg
+[docker-url]: https://github.com/Stephen-RA-King/zyme/actions/workflows/docker-image.yml
 [downloads-image]: https://static.pepy.tech/personalized-badge/zyme?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
 [downloads-url]: https://pepy.tech/project/zyme
 [format-image]: https://img.shields.io/pypi/format/zyme
 [isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
 [isort-url]: https://github.com/pycqa/isort/
 [lgtm-alerts-image]: https://img.shields.io/lgtm/alerts/g/Stephen-RA-King/zyme.svg?logo=lgtm&logoWidth=18
 [lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/zyme/alerts/
 [lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/zyme.svg?logo=lgtm&logoWidth=18
 [lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/zyme/context:python
 [license-image]: https://img.shields.io/pypi/l/zyme
-[license-url]: https://github.com/Stephen-RA-King/zyme/blob/main/license
+[license-url]: https://github.com/Stephen-RA-King/zyme/blob/main/LICENSE
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
+[openssf-image]: https://api.securityscorecards.dev/projects/github.com/Stephen-RA-King/zyme/badge
+[openssf-url]: https://api.securityscorecards.dev/projects/github.com/Stephen-RA-King/zyme
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
-[pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/gitwatch/main.svg
-[pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/gitwatch/main
+[pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/zyme/main.svg
+[pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/zyme/main
+[pydough-image]: https://img.shields.io/badge/pydough-2023-orange
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [pypi-url]: https://pypi.org/project/zyme/
 [pypi-image]: https://img.shields.io/pypi/v/zyme.svg
 [python-version-image]: https://img.shields.io/pypi/pyversions/zyme
 [readthedocs-image]: https://readthedocs.org/projects/zyme/badge/?version=latest
 [readthedocs-url]: https://zyme.readthedocs.io/en/latest/?badge=latest
-[requirements-status-image]: https://requires.io/github/Stephen-RA-King/zyme/requirements.svg?branch=main
-[requirements-status-url]: https://requires.io/github/Stephen-RA-King/zyme/requirements/?branch=main
 [status-image]: https://img.shields.io/pypi/status/zyme.svg
 [tests-image]: https://github.com/Stephen-RA-King/zyme/actions/workflows/tests.yml/badge.svg
 [tests-url]: https://github.com/Stephen-RA-King/zyme/actions/workflows/tests.yml
 [wiki]: https://github.com/Stephen-RA-King/zyme/wiki
```

### Comparing `zyme-0.1.1/README.md` & `zyme-0.1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,132 +2,150 @@
 
 > Short blurb about what your product does.
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
-[![Format][format-image]][pypi-url]
-[![Requirements][requirements-status-image]][requirements-status-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
-[![CodeFactor][codefactor-image]][codefactor-url]
-[![Codeclimate][codeclimate-image]][codeclimate-url]
-[![Lgtm alerts][lgtm-alerts-image]][lgtm-alerts-url]
-[![Lgtm quality][lgtm-quality-image]][lgtm-quality-url]
 [![CodeQl][codeql-image]][codeql-url]
-[![readthedocs][readthedocs-image]][readthedocs-url]
+[![Docker][docker-image]][docker-url]
 [![pre-commit][pre-commit-image]][pre-commit-url]
 [![pre-commit.ci status][pre-commit.ci-image]][pre-commit.ci-url]
+[![readthedocs][readthedocs-image]][readthedocs-url]
+[![CodeFactor][codefactor-image]][codefactor-url]
+[![Codeclimate][codeclimate-image]][codeclimate-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
 [![Checked with mypy][mypy-image]][mypy-url]
 [![security: bandit][bandit-image]][bandit-url]
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
 [![license][license-image]][license-url]
+[![Pydough][pydough-image]][pydough-url]
+[![OpenSSFScorecard][openssf-image]][openssf-url]
 
 One to two paragraph statement about your product and what it does.
 
-![](assets/header.png)
+![](assets/header_dough.png)
 
 ## Installation
 
+---
+
 OS X & Linux:
 
 ```sh
 pip3 install zyme
 ```
 
 Windows:
 
 ```sh
 pip install zyme
 ```
 
 ## Usage example
 
+---
+
 A few motivating and useful examples of how your product can be used. Spice this up with code blocks and potentially more screenshots.
 
 _For more examples and usage, please refer to the [Wiki][wiki]._
 
 ## Development setup
 
+---
+
 Describe how to install all development dependencies and how to run an automated test-suite of some kind. Potentially do this for multiple platforms.
 
 ```sh
 pip install --editable zyme
 ```
 
 ## Documentation
 
-### - [**Read the Docs**](https://zyme.readthedocs.io/en/latest/)
+---
 
-### - [**Wiki**](https://github.com/Stephen-RA-King/zyme/wiki)
+[**Read the Docs**](https://zyme.readthedocs.io/en/latest/)
+
+-   [**Example Usage**](https://zyme.readthedocs.io/en/latest/example.html)
+-   [**Credits**](https://zyme.readthedocs.io/en/latest/example.html)
+-   [**Changelog**](https://zyme.readthedocs.io/en/latest/changelog.html)
+-   [**API Reference**](https://zyme.readthedocs.io/en/latest/autoapi/index.html)
+
+[**Wiki**](https://github.com/Stephen-RA-King/zyme/wiki)
 
 ## Meta
 
-[![](assets/linkedin.png)](https://linkedin.com/in/stephen-k-3a4644210)
+---
+
+[![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
-[![](assets/pypi.png)](https://pypi.org/project/zyme/)
+[![](assets/pypi.png)](https://pypi.org/project/zyme)
+[![Docker](assets/docker.png)](https://hub.docker.com/r/sraking/zyme)
 [![](assets/www.png)](https://www.justpython.tech)
-[![](assets/email.png)](mailto:stephen.ra.king@gmail.com)
-[![](assets/cv.png)](https://www.justpython.tech/cv)
+[![](assets/email.png)](mailto:sking.github@gmail.com)
+[![](assets/github.png)](https://github.com/Stephen-RA-King/zyme)
 
-Stephen R A King : stephen.ra.king@gmail.com
+Author: Stephen R A King ([sking.github@gmail.com](mailto:sking.github@gmail.com))
 
-Distributed under the MIT license. See [license](license-url) for more information.
+Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-[https://github.com/Stephen-RA-King/zyme](https://github.com/Stephen-RA-King/zyme)
+Created with Cookiecutter template: [![pydough][pydough-image]][pydough-url] version 1.3.3
 
-Created with Cookiecutter template: [**cc_template**][cc_template-url] version 1.1.1
+Digital object identifier: [![DOI](https://zenodo.org/badge/xxxxxxxxx.svg)](https://zenodo.org/badge/latestdoi/xxxxxxxxx)
 
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
-[cc_template-url]: https://github.com/Stephen-RA-King/cc_template
 [codeclimate-image]: https://api.codeclimate.com/v1/badges/7fc352185512a1dab75d/maintainability
 [codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/zyme/maintainability
 [codecov-image]: https://codecov.io/gh/Stephen-RA-King/zyme/branch/main/graph/badge.svg
 [codecov-url]: https://app.codecov.io/gh/Stephen-RA-King/zyme
 [codefactor-image]: https://www.codefactor.io/repository/github/Stephen-RA-King/zyme/badge
 [codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/zyme
-[codeql-image]: https://github.com/Stephen-RA-King/zyme/actions/workflows/codeql-analysis.yml/badge.svg
-[codeql-url]: https://github.com/Stephen-RA-King/zyme/actions/workflows/codeql-analysis.yml
+[codeql-image]: https://github.com/Stephen-RA-King/zyme/actions/workflows/github-code-scanning/codeql/badge.svg
+[codeql-url]: https://github.com/Stephen-RA-King/zyme/actions/workflows/github-code-scanning/codeql
 [commitizen-image]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
 [commitizen-url]: http://commitizen.github.io/cz-cli/
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square
 [conventional-commits-url]: https://conventionalcommits.org
 [deepsource-image]: https://static.deepsource.io/deepsource-badge-light-mini.svg
 [deepsource-url]: https://deepsource.io/gh/Stephen-RA-King/zyme/?ref=repository-badge
+[docker-image]: https://github.com/Stephen-RA-King/zyme/actions/workflows/docker-image.yml/badge.svg
+[docker-url]: https://github.com/Stephen-RA-King/zyme/actions/workflows/docker-image.yml
 [downloads-image]: https://static.pepy.tech/personalized-badge/zyme?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
 [downloads-url]: https://pepy.tech/project/zyme
 [format-image]: https://img.shields.io/pypi/format/zyme
 [isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
 [isort-url]: https://github.com/pycqa/isort/
 [lgtm-alerts-image]: https://img.shields.io/lgtm/alerts/g/Stephen-RA-King/zyme.svg?logo=lgtm&logoWidth=18
 [lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/zyme/alerts/
 [lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/zyme.svg?logo=lgtm&logoWidth=18
 [lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/zyme/context:python
 [license-image]: https://img.shields.io/pypi/l/zyme
-[license-url]: https://github.com/Stephen-RA-King/zyme/blob/main/license
+[license-url]: https://github.com/Stephen-RA-King/zyme/blob/main/LICENSE
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
+[openssf-image]: https://api.securityscorecards.dev/projects/github.com/Stephen-RA-King/zyme/badge
+[openssf-url]: https://api.securityscorecards.dev/projects/github.com/Stephen-RA-King/zyme
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
-[pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/gitwatch/main.svg
-[pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/gitwatch/main
+[pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/zyme/main.svg
+[pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/zyme/main
+[pydough-image]: https://img.shields.io/badge/pydough-2023-orange
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [pypi-url]: https://pypi.org/project/zyme/
 [pypi-image]: https://img.shields.io/pypi/v/zyme.svg
 [python-version-image]: https://img.shields.io/pypi/pyversions/zyme
 [readthedocs-image]: https://readthedocs.org/projects/zyme/badge/?version=latest
 [readthedocs-url]: https://zyme.readthedocs.io/en/latest/?badge=latest
-[requirements-status-image]: https://requires.io/github/Stephen-RA-King/zyme/requirements.svg?branch=main
-[requirements-status-url]: https://requires.io/github/Stephen-RA-King/zyme/requirements/?branch=main
 [status-image]: https://img.shields.io/pypi/status/zyme.svg
 [tests-image]: https://github.com/Stephen-RA-King/zyme/actions/workflows/tests.yml/badge.svg
 [tests-url]: https://github.com/Stephen-RA-King/zyme/actions/workflows/tests.yml
 [wiki]: https://github.com/Stephen-RA-King/zyme/wiki
```

### Comparing `zyme-0.1.1/pyproject.toml` & `zyme-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,21 +5,25 @@
 ]
 build-backend = "setuptools.build_meta"
 
 [tool]
 [tool.black]
 line-length = 88
 
-[tool.pytest.ini_options]
-# https://docs.pytest.org/en/6.2.x/reference.html?highlight=minversion#configuration-options
-minversion = "6.0"
-testpaths = [
-    "tests",
+[tool.cruft]
+skip = [
+    "tests/",
+    "src/",
+    "*/header.png",
+    ".pypirc",
+    "CHANGELOG.md",
+    "setup.cfg"
 ]
 
+
 [tool.isort]
 import_heading_stdlib = "Core Library modules"
 import_heading_thirdparty = "Third party modules"
 import_heading_firstparty = "First party modules"
 import_heading_localfolder = "Local modules"
 include_trailing_comma = true
 indent = '    '
@@ -48,19 +52,29 @@
 warn_unused_ignores = true
 strict_optional = true
 warn_redundant_casts = true
 warn_unused_configs = true
 disallow_untyped_calls = false
 disallow_incomplete_defs = true
 follow_imports = "skip"
-html_report = "mypy-report"
+html_report = "reports/mypy"
+cache_dir = 'cache/.mypy_cache'
 mypy_path = "typeshed/pyi:typeshed/imports"
+exclude = [
+    '^tests/[\w]*.py$',
+    '^tools/[\w]*.py$',
+    '^docs/[\w]*.py$',
+    '^tasks.py$'
+]
 
 [tool.semantic_release]
-version_variable = "src/zyme/__init__.py:__version__"
+version_variable = [
+    "src/zyme/__init__.py:__version__",
+    "docs/conf.py:version",
+]
 branch = "main"
 changelog_file = "CHANGELOG.md"
 build_command = "python -m build"
 dist_path = "dist/"
 upload_to_pypi = true
 upload_to_repository = true
 remove_dist = true
@@ -77,16 +91,7 @@
 [tool.flakeheaven.plugins]
 pyflakes = ["+*", "-F401"]
 "flake8-*" = ["+*"]
 mccabe = ["+*"]
 pep8-naming = ["+*"]
 pycodestyle = ["+*"]
 pylint = ["+F*", "+E*", "-E0611", "-E1101", "-E0401", "-E1102", "-E1123"]
-
-[tool.coverage.run]
-branch = true
-parallel = true
-
-[tool.coverage.report]
-show_missing = true
-precision = 2
-skip_empty = true
```

### Comparing `zyme-0.1.1/setup.cfg` & `zyme-0.1.5/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,129 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 207a 796d 650d 0a76 6572 7369 6f6e   = zyme..version
 00000020: 203d 2061 7474 723a 207a 796d 652e 5f5f   = attr: zyme.__
 00000030: 7665 7273 696f 6e5f 5f0d 0a61 7574 686f  version__..autho
 00000040: 7220 3d20 5374 6570 6865 6e20 5220 4120  r = Stephen R A 
 00000050: 4b69 6e67 0d0a 6175 7468 6f72 5f65 6d61  King..author_ema
-00000060: 696c 203d 2073 7465 7068 656e 2e72 612e  il = stephen.ra.
-00000070: 6b69 6e67 4067 6d61 696c 2e63 6f6d 0d0a  king@gmail.com..
-00000080: 6d61 696e 7461 696e 6572 203d 2053 7465  maintainer = Ste
-00000090: 7068 656e 2052 2041 204b 696e 670d 0a6d  phen R A King..m
-000000a0: 6169 6e74 6169 6e65 725f 656d 6169 6c20  aintainer_email 
-000000b0: 3d20 7374 6570 6865 6e2e 7261 2e6b 696e  = stephen.ra.kin
-000000c0: 6740 676d 6169 6c2e 636f 6d0d 0a64 6573  g@gmail.com..des
-000000d0: 6372 6970 7469 6f6e 203d 2070 6c61 6365  cription = place
-000000e0: 686f 6c64 6572 0d0a 6c6f 6e67 5f64 6573  holder..long_des
-000000f0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
-00000100: 2052 4541 444d 452e 6d64 0d0a 6c6f 6e67   README.md..long
-00000110: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
-00000120: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
-00000130: 2f6d 6172 6b64 6f77 6e0d 0a6b 6579 776f  /markdown..keywo
-00000140: 7264 7320 3d20 7574 696c 6974 792c 0d0a  rds = utility,..
-00000150: 706c 6174 666f 726d 7320 3d20 416e 790d  platforms = Any.
-00000160: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
-00000170: 6974 6875 622e 636f 6d2f 5374 6570 6865  ithub.com/Stephe
-00000180: 6e2d 5241 2d4b 696e 672f 7a79 6d65 0d0a  n-RA-King/zyme..
-00000190: 646f 776e 6c6f 6164 5f75 726c 203d 2068  download_url = h
-000001a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000001b0: 6d2f 5374 6570 6865 6e2d 5241 2d4b 696e  m/Stephen-RA-Kin
-000001c0: 672f 7a79 6d65 2f61 7263 6869 7665 2f72  g/zyme/archive/r
-000001d0: 6566 732f 6865 6164 732f 6d61 696e 2e7a  efs/heads/main.z
-000001e0: 6970 0d0a 6c69 6365 6e73 6520 3d20 4d49  ip..license = MI
-000001f0: 540d 0a63 6c61 7373 6966 6965 7273 203d  T..classifiers =
-00000200: 200d 0a09 4465 7665 6c6f 706d 656e 7420   ...Development 
-00000210: 5374 6174 7573 203a 3a20 3120 2d20 506c  Status :: 1 - Pl
-00000220: 616e 6e69 6e67 0d0a 0945 6e76 6972 6f6e  anning...Environ
-00000230: 6d65 6e74 203a 3a20 436f 6e73 6f6c 650d  ment :: Console.
-00000240: 0a09 496e 7465 6e64 6564 2041 7564 6965  ..Intended Audie
-00000250: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
-00000260: 730d 0a09 4f70 6572 6174 696e 6720 5379  s...Operating Sy
-00000270: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-00000280: 656e 6465 6e74 0d0a 094e 6174 7572 616c  endent...Natural
-00000290: 204c 616e 6775 6167 6520 3a3a 2045 6e67   Language :: Eng
-000002a0: 6c69 7368 0d0a 0950 726f 6772 616d 6d69  lish...Programmi
-000002b0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000002c0: 7974 686f 6e20 3a3a 2033 0d0a 0950 726f  ython :: 3...Pro
-000002d0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000002e0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000002f0: 203a 3a20 4f6e 6c79 0d0a 0950 726f 6772   :: Only...Progr
-00000300: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000310: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
-00000320: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000330: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000340: 6e20 3a3a 2033 2e39 0d0a 0950 726f 6772  n :: 3.9...Progr
-00000350: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000360: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-00000370: 300d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  0....[options]..
-00000380: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
-00000390: 093d 7372 630d 0a70 6163 6b61 6765 7320  .=src..packages 
-000003a0: 3d20 6669 6e64 3a0d 0a70 726f 6a65 6374  = find:..project
-000003b0: 5f75 726c 7320 3d20 0d0a 696e 636c 7564  _urls = ..includ
-000003c0: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
-000003d0: 2054 7275 650d 0a70 7974 686f 6e5f 7265   True..python_re
-000003e0: 7175 6972 6573 203d 203e 3d33 2e38 0d0a  quires = >=3.8..
-000003f0: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-00000400: 203d 200d 0a09 636c 6963 6b0d 0a09 7079   = ...click...py
-00000410: 7961 6d6c 0d0a 0974 6f6d 6c0d 0a0d 0a5b  yaml...toml....[
-00000420: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
-00000430: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
-00000440: 7372 630d 0a0d 0a5b 6f70 7469 6f6e 732e  src....[options.
-00000450: 7061 636b 6167 655f 6461 7461 5d0d 0a7a  package_data]..z
-00000460: 796d 6520 3d20 0d0a 0963 6f6e 6669 672e  yme = ...config.
-00000470: 6a73 6f6e 0d0a 0963 6f6e 6669 672e 696e  json...config.in
-00000480: 690d 0a09 636f 6e66 6967 2e74 6f6d 6c0d  i...config.toml.
-00000490: 0a09 636f 6e66 6967 2e79 616d 6c0d 0a0d  ..config.yaml...
-000004a0: 0a5b 6f70 7469 6f6e 732e 656e 7472 795f  .[options.entry_
-000004b0: 706f 696e 7473 5d0d 0a63 6f6e 736f 6c65  points]..console
-000004c0: 5f73 6372 6970 7473 203d 200d 0a09 7a79  _scripts = ...zy
-000004d0: 6d65 203d 207a 796d 652e 7a79 6d65 3a63  me = zyme.zyme:c
-000004e0: 6c69 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a  li....[flake8]..
-000004f0: 646f 6373 7472 696e 672d 636f 6e76 656e  docstring-conven
-00000500: 7469 6f6e 203d 206e 756d 7079 0d0a 6d61  tion = numpy..ma
-00000510: 782d 636f 6d70 6c65 7869 7479 203d 2031  x-complexity = 1
-00000520: 380d 0a6d 6178 2d6c 696e 652d 6c65 6e67  8..max-line-leng
-00000530: 7468 203d 2038 380d 0a73 656c 6563 7420  th = 88..select 
-00000540: 3d20 422c 2042 392c 2043 2c20 442c 2045  = B, B9, C, D, E
-00000550: 2c20 462c 204e 2c20 570d 0a65 7863 6c75  , F, N, W..exclu
-00000560: 6465 203d 2074 6573 7473 2f2a 2c2e 746f  de = tests/*,.to
-00000570: 782f 2a2c 2e6e 6f78 2f2a 2c64 6f63 732f  x/*,.nox/*,docs/
-00000580: 2a2c 2e67 6974 2f2a 2c2e 6769 7468 7562  *,.git/*,.github
-00000590: 2f2a 0d0a 6967 6e6f 7265 203d 200d 0a09  /*..ignore = ...
-000005a0: 4532 3033 2c0d 0a09 5735 3033 2c0d 0a70  E203,...W503,..p
-000005b0: 6572 2d66 696c 652d 6967 6e6f 7265 7320  er-file-ignores 
-000005c0: 3d20 0d0a 095f 5f69 6e69 745f 5f2e 7079  = ...__init__.py
-000005d0: 3a46 3430 310d 0a09 7061 7468 6d61 6769  :F401...pathmagi
-000005e0: 632e 7079 3a46 3430 310d 0a09 7465 7374  c.py:F401...test
-000005f0: 5f7a 796d 652e 7079 3a46 3430 310d 0a0d  _zyme.py:F401...
-00000600: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000610: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000620: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000060: 696c 203d 2073 6b69 6e67 2e67 6974 6875  il = sking.githu
+00000070: 6240 676d 6169 6c2e 636f 6d0d 0a6d 6169  b@gmail.com..mai
+00000080: 6e74 6169 6e65 7220 3d20 5374 6570 6865  ntainer = Stephe
+00000090: 6e20 5220 4120 4b69 6e67 0d0a 6d61 696e  n R A King..main
+000000a0: 7461 696e 6572 5f65 6d61 696c 203d 2073  tainer_email = s
+000000b0: 6b69 6e67 2e67 6974 6875 6240 676d 6169  king.github@gmai
+000000c0: 6c2e 636f 6d0d 0a64 6573 6372 6970 7469  l.com..descripti
+000000d0: 6f6e 203d 2070 6c61 6365 686f 6c64 6572  on = placeholder
+000000e0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+000000f0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
+00000100: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
+00000110: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
+00000120: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
+00000130: 6f77 6e0d 0a6b 6579 776f 7264 7320 3d20  own..keywords = 
+00000140: 7574 696c 6974 792c 0d0a 706c 6174 666f  utility,..platfo
+00000150: 726d 7320 3d20 416e 790d 0a75 726c 203d  rms = Any..url =
+00000160: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000170: 636f 6d2f 5374 6570 6865 6e2d 5241 2d4b  com/Stephen-RA-K
+00000180: 696e 672f 7a79 6d65 0d0a 646f 776e 6c6f  ing/zyme..downlo
+00000190: 6164 5f75 726c 203d 2068 7474 7073 3a2f  ad_url = https:/
+000001a0: 2f67 6974 6875 622e 636f 6d2f 5374 6570  /github.com/Step
+000001b0: 6865 6e2d 5241 2d4b 696e 672f 7a79 6d65  hen-RA-King/zyme
+000001c0: 2f61 7263 6869 7665 2f72 6566 732f 6865  /archive/refs/he
+000001d0: 6164 732f 6d61 696e 2e7a 6970 0d0a 6c69  ads/main.zip..li
+000001e0: 6365 6e73 6520 3d20 4d49 540d 0a6c 6963  cense = MIT..lic
+000001f0: 656e 7365 5f66 696c 6573 203d 204c 4943  ense_files = LIC
+00000200: 454e 5345 0d0a 7072 6f6a 6563 745f 7572  ENSE..project_ur
+00000210: 6c73 203d 200d 0a09 4275 6720 5472 6163  ls = ...Bug Trac
+00000220: 6b65 7220 3d20 6874 7470 733a 2f2f 6769  ker = https://gi
+00000230: 7468 7562 2e63 6f6d 2f53 7465 7068 656e  thub.com/Stephen
+00000240: 2d52 412d 4b69 6e67 2f7a 796d 652f 6973  -RA-King/zyme/is
+00000250: 7375 6573 0d0a 0943 4920 3d20 6874 7470  sues...CI = http
+00000260: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
+00000270: 7465 7068 656e 2d52 412d 4b69 6e67 2f7a  tephen-RA-King/z
+00000280: 796d 652f 6163 7469 6f6e 730d 0a09 446f  yme/actions...Do
+00000290: 6375 6d65 6e74 6174 696f 6e20 3d20 6874  cumentation = ht
+000002a0: 7470 733a 2f2f 7a79 6d65 2e72 6561 6474  tps://zyme.readt
+000002b0: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+000002c0: 6573 742f 0d0a 0952 656c 6561 7365 204e  est/...Release N
+000002d0: 6f74 6573 203d 2068 7474 7073 3a2f 2f67  otes = https://g
+000002e0: 6974 6875 622e 636f 6d2f 5374 6570 6865  ithub.com/Stephe
+000002f0: 6e2d 5241 2d4b 696e 672f 7a79 6d65 2f72  n-RA-King/zyme/r
+00000300: 656c 6561 7365 730d 0a09 536f 7572 6365  eleases...Source
+00000310: 2043 6f64 6520 3d20 6874 7470 733a 2f2f   Code = https://
+00000320: 6769 7468 7562 2e63 6f6d 2f53 7465 7068  github.com/Steph
+00000330: 656e 2d52 412d 4b69 6e67 2f7a 796d 652f  en-RA-King/zyme/
+00000340: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
+00000350: 0d0a 0944 6576 656c 6f70 6d65 6e74 2053  ...Development S
+00000360: 7461 7475 7320 3a3a 2031 202d 2050 6c61  tatus :: 1 - Pla
+00000370: 6e6e 696e 670d 0a09 456e 7669 726f 6e6d  nning...Environm
+00000380: 656e 7420 3a3a 2043 6f6e 736f 6c65 0d0a  ent :: Console..
+00000390: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
+000003a0: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
+000003b0: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
+000003c0: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+000003d0: 6e64 656e 740d 0a09 4e61 7475 7261 6c20  ndent...Natural 
+000003e0: 4c61 6e67 7561 6765 203a 3a20 456e 676c  Language :: Engl
+000003f0: 6973 680d 0a09 5072 6f67 7261 6d6d 696e  ish...Programmin
+00000400: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000410: 7468 6f6e 203a 3a20 330d 0a09 5072 6f67  thon :: 3...Prog
+00000420: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000430: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
+00000440: 3a3a 204f 6e6c 790d 0a09 5072 6f67 7261  :: Only...Progra
+00000450: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000460: 3a20 5079 7468 6f6e 203a 3a20 332e 390d  : Python :: 3.9.
+00000470: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000480: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000490: 203a 3a20 332e 3130 0d0a 0950 726f 6772   :: 3.10...Progr
+000004a0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000004b0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+000004c0: 310d 0a09 5072 6f67 7261 6d6d 696e 6720  1...Programming 
+000004d0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000004e0: 6f6e 203a 3a20 332e 3132 0d0a 0d0a 5b6f  on :: 3.12....[o
+000004f0: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
+00000500: 5f64 6972 203d 200d 0a09 3d73 7263 0d0a  _dir = ...=src..
+00000510: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+00000520: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
+00000530: 655f 6461 7461 203d 2054 7275 650d 0a70  e_data = True..p
+00000540: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+00000550: 203e 3d33 2e39 0d0a 696e 7374 616c 6c5f   >=3.9..install_
+00000560: 7265 7175 6972 6573 203d 200d 0a09 7079  requires = ...py
+00000570: 7961 6d6c 0d0a 0974 6f6d 6c0d 0a09 5069  yaml...toml...Pi
+00000580: 6c6c 6f77 0d0a 0d0a 5b6f 7074 696f 6e73  llow....[options
+00000590: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
+000005a0: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
+000005b0: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+000005c0: 5f64 6174 615d 0d0a 7a79 6d65 203d 200d  _data]..zyme = .
+000005d0: 0a09 7265 736f 7572 6365 732f 636f 6e66  ..resources/conf
+000005e0: 6967 2e6a 736f 6e0d 0a09 7265 736f 7572  ig.json...resour
+000005f0: 6365 732f 636f 6e66 6967 2e69 6e69 0d0a  ces/config.ini..
+00000600: 0972 6573 6f75 7263 6573 2f63 6f6e 6669  .resources/confi
+00000610: 672e 746f 6d6c 0d0a 0972 6573 6f75 7263  g.toml...resourc
+00000620: 6573 2f63 6f6e 6669 672e 7961 6d6c 0d0a  es/config.yaml..
+00000630: 0972 6573 6f75 7263 6573 2f72 6573 6f75  .resources/resou
+00000640: 7263 652e 7069 636b 6c65 0d0a 0972 6573  rce.pickle...res
+00000650: 6f75 7263 6573 2f72 6573 6f75 7263 652e  ources/resource.
+00000660: 706e 670d 0a09 7265 736f 7572 6365 732f  png...resources/
+00000670: 7265 736f 7572 6365 2e64 620d 0a0d 0a5b  resource.db....[
+00000680: 6f70 7469 6f6e 732e 656e 7472 795f 706f  options.entry_po
+00000690: 696e 7473 5d0d 0a63 6f6e 736f 6c65 5f73  ints]..console_s
+000006a0: 6372 6970 7473 203d 200d 0a09 7a79 6d65  cripts = ...zyme
+000006b0: 203d 207a 796d 652e 7a79 6d65 3a6d 6169   = zyme.zyme:mai
+000006c0: 6e0d 0a0d 0a5b 666c 616b 6538 5d0d 0a64  n....[flake8]..d
+000006d0: 6f63 7374 7269 6e67 2d63 6f6e 7665 6e74  ocstring-convent
+000006e0: 696f 6e20 3d20 6e75 6d70 790d 0a6d 6178  ion = numpy..max
+000006f0: 2d63 6f6d 706c 6578 6974 7920 3d20 3138  -complexity = 18
+00000700: 0d0a 6d61 782d 6c69 6e65 2d6c 656e 6774  ..max-line-lengt
+00000710: 6820 3d20 3838 0d0a 7365 6c65 6374 203d  h = 88..select =
+00000720: 2042 2c20 4239 2c20 432c 2044 2c20 452c   B, B9, C, D, E,
+00000730: 2046 2c20 4e2c 2057 0d0a 6578 636c 7564   F, N, W..exclud
+00000740: 6520 3d20 7465 7374 732f 2a2c 2e74 6f78  e = tests/*,.tox
+00000750: 2f2a 2c2e 6e6f 782f 2a2c 646f 6373 2f2a  /*,.nox/*,docs/*
+00000760: 2c2e 6769 742f 2a2c 2e67 6974 6875 622f  ,.git/*,.github/
+00000770: 2a0d 0a69 676e 6f72 6520 3d20 0d0a 0945  *..ignore = ...E
+00000780: 3230 332c 0d0a 0957 3530 332c 0d0a 7065  203,...W503,..pe
+00000790: 722d 6669 6c65 2d69 676e 6f72 6573 203d  r-file-ignores =
+000007a0: 200d 0a09 5f5f 696e 6974 5f5f 2e70 793a   ...__init__.py:
+000007b0: 4634 3031 0d0a 0970 6174 686d 6167 6963  F401...pathmagic
+000007c0: 2e70 793a 4634 3031 0d0a 0974 6573 745f  .py:F401...test_
+000007d0: 7a79 6d65 2e70 793a 4634 3031 0d0a 0d0a  zyme.py:F401....
+000007e0: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+000007f0: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+00000800: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

### Comparing `zyme-0.1.1/src/zyme/zyme.py` & `zyme-0.1.5/src/zyme/zyme.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,101 +1,115 @@
-#!/usr/bin/env python3
-"""Example script to demonstrate layout and testing."""
-# Core Library modules
-import sys
-from typing import Any
-
-# Local modules
-from . import ini_config, json_config, logger, toml_config, yaml_config
-
-
-def get_config() -> tuple:
-
-    """Return a configuration parameter from one of the configuration files.
-
-    Returns
-    -------
-    tuple
-        length of the tuple along with the debug setting from each config file
-    """
-    configs = [ini_config, json_config, toml_config, yaml_config]
-    config_result = []
-    config_len = len(configs)
-
-    for config in configs:
-        config_result.append(bool(config["APP"]["DEBUG"]))
-    return config_len, config_result
-
-
-def handle_exception(exc_type, exc_value, exc_traceback):  # type: ignore
-    if issubclass(exc_type, KeyboardInterrupt):
-        sys.__excepthook__(exc_type, exc_value, exc_traceback)
-        return
-    logger.error("Uncaught exception", exc_info=(exc_type, exc_value, exc_traceback))
-
-
-sys.excepthook = handle_exception
-
-
-def fizzbuzz(number_range: int) -> list:
-
-    """Demonstrate one solution to the FizzBuzz problem.
-
-    Return integers 1 to N, but print “Fizz” if an integer is divisible by 3,
-    “Buzz” if an integer is divisible by 5, and “FizzBuzz” if an integer is
-    divisible by both 3 and 5
-
-    Parameters
-    ----------
-    number_range : int
-        The maximum number that will be used
-
-    Returns
-    -------
-    list
-        The result will be returned as a list
-
-    Examples
-    --------
-    >>> fizzbuzz(20)
-    """
-    result: list[Any] = []
-    for num in range(1, number_range):
-        if num % 15 == 0:
-            result.append("FizzBuzz")
-        elif num % 5 == 0:
-            result.append("Buzz")
-        elif num % 3 == 0:
-            result.append("Fizz")
-        else:
-            result.append(num)
-    logger.debug(f"fizzbuzz result: {result}")
-    return result
-
-
-def fibonacci(number_range: int) -> list:
-
-    """series of numbers in which each number is the sum of the two that precede it.
-
-    Parameters
-    ----------
-    number_range : int
-        The maximum number that will be used
-
-    Returns
-    -------
-    list
-        The result will be returned as a list
-
-    Examples
-    --------
-    >>> fibonacci(20)
-    """
-
-    result: list = []
-    a, b = 1, 1
-    while True:
-        if a >= number_range:
-            logger.debug(f"fibonacci result: {result}")
-            return result
-        result.append(a)
-        a, b = b, (a + b)
+#!/usr/bin/env python3
+"""Example script to demonstrate layout and testing."""
+# Core Library modules
+import sys
+from typing import Any
+
+# Local modules
+from . import (
+    ini_config,
+    json_config,
+    logger,
+    pickle_content,
+    toml_config,
+    yaml_config,
+)
+
+
+def get_config() -> tuple:
+    """Return a configuration parameter from one of the configuration files.
+
+    Returns
+    -------
+    tuple
+        length of the tuple along with the debug setting from each config file.
+    """
+    configs = [ini_config, json_config, toml_config, yaml_config]
+    config_result = []
+    config_len = len(configs)
+
+    for config in configs:
+        config_result.append(bool(config["APP"]["DEBUG"]))
+    return config_len, config_result
+
+
+def handle_exception(exc_type, exc_value, exc_traceback):  # type: ignore
+    if issubclass(exc_type, KeyboardInterrupt):
+        sys.__excepthook__(exc_type, exc_value, exc_traceback)
+        return
+    logger.error("Uncaught exception", exc_info=(exc_type, exc_value, exc_traceback))
+
+
+sys.excepthook = handle_exception
+
+
+def fizzbuzz(number_range: int) -> list:
+    """Demonstrate one solution to the FizzBuzz problem.
+
+    Return integers 1 to N, but print “Fizz” if an integer is divisible by 3,
+    “Buzz” if an integer is divisible by 5, and “FizzBuzz” if an integer is
+    divisible by both 3 and 5
+
+    Parameters
+    ----------
+    number_range : int
+        The maximum number that will be used
+
+    Returns
+    -------
+    list
+        The result will be returned as a list
+
+    Examples
+    --------
+    >>> fizzbuzz(20)
+    """
+    result: list[Any] = []
+    for num in range(1, number_range):
+        if num % 15 == 0:
+            result.append("FizzBuzz")
+        elif num % 5 == 0:
+            result.append("Buzz")
+        elif num % 3 == 0:
+            result.append("Fizz")
+        else:
+            result.append(num)
+    logger.debug(f"fizzbuzz result: {result}")
+    return result
+
+
+def fibonacci(number_range: int) -> list:
+    """series of numbers in which each number is the sum of the two that precede it.
+
+    Parameters
+    ----------
+    number_range : int
+        The maximum number that will be used
+
+    Returns
+    -------
+    list
+        The result will be returned as a list
+
+    Examples
+    --------
+    >>> fibonacci(20)
+    """
+
+    result: list = []
+    a, b = 1, 1
+    while True:
+        if a >= number_range:
+            logger.debug(f"fibonacci result: {result}")
+            return result
+        result.append(a)
+        a, b = b, (a + b)
+
+
+def main():  # type: ignore
+    print(pickle_content)
+    print(fizzbuzz(20))
+    print(fibonacci(20))
+
+
+if __name__ == "__main__":
+    raise SystemExit(main())
```

### Comparing `zyme-0.1.1/src/zyme/zyme_cli.py` & `zyme-0.1.5/src/zyme/zyme_cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 
 @info.command(help="Display Author Name")
 @click.option("-verbose", "--verbose", is_flag=True, help="set the verbosity")
 def author(verbose: str) -> None:
     """Returns details about the Author."""
     click.echo("Author name: Stephen R A King")
     if verbose:
-        click.echo("Author eMail: stephen.ra.king@gmail.com")
+        click.echo("Author eMail: sking.github@gmail.com")
 
 
 if __name__ == "__main__":
-    info()
+    raise SystemExit(info())
```

### Comparing `zyme-0.1.1/src/zyme.egg-info/PKG-INFO` & `zyme-0.1.5/src/zyme.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,161 +1,184 @@
 Metadata-Version: 2.1
 Name: zyme
-Version: 0.1.1
+Version: 0.1.5
 Summary: placeholder
 Home-page: https://github.com/Stephen-RA-King/zyme
 Download-URL: https://github.com/Stephen-RA-King/zyme/archive/refs/heads/main.zip
 Author: Stephen R A King
-Author-email: stephen.ra.king@gmail.com
+Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
-Maintainer-email: stephen.ra.king@gmail.com
+Maintainer-email: sking.github@gmail.com
 License: MIT
+Project-URL: Bug Tracker, https://github.com/Stephen-RA-King/zyme/issues
+Project-URL: CI, https://github.com/Stephen-RA-King/zyme/actions
+Project-URL: Documentation, https://zyme.readthedocs.io/en/latest/
+Project-URL: Release Notes, https://github.com/Stephen-RA-King/zyme/releases
+Project-URL: Source Code, https://github.com/Stephen-RA-King/zyme/
 Keywords: utility
 Platform: Any
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: AUTHORS.md
 
 # zyme
 
 > Short blurb about what your product does.
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
-[![Format][format-image]][pypi-url]
-[![Requirements][requirements-status-image]][requirements-status-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
-[![CodeFactor][codefactor-image]][codefactor-url]
-[![Codeclimate][codeclimate-image]][codeclimate-url]
-[![Lgtm alerts][lgtm-alerts-image]][lgtm-alerts-url]
-[![Lgtm quality][lgtm-quality-image]][lgtm-quality-url]
 [![CodeQl][codeql-image]][codeql-url]
-[![readthedocs][readthedocs-image]][readthedocs-url]
+[![Docker][docker-image]][docker-url]
 [![pre-commit][pre-commit-image]][pre-commit-url]
 [![pre-commit.ci status][pre-commit.ci-image]][pre-commit.ci-url]
+[![readthedocs][readthedocs-image]][readthedocs-url]
+[![CodeFactor][codefactor-image]][codefactor-url]
+[![Codeclimate][codeclimate-image]][codeclimate-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
 [![Checked with mypy][mypy-image]][mypy-url]
 [![security: bandit][bandit-image]][bandit-url]
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
 [![license][license-image]][license-url]
+[![Pydough][pydough-image]][pydough-url]
+[![OpenSSFScorecard][openssf-image]][openssf-url]
 
 One to two paragraph statement about your product and what it does.
 
-![](assets/header.png)
+![](assets/header_dough.png)
 
 ## Installation
 
+---
+
 OS X & Linux:
 
 ```sh
 pip3 install zyme
 ```
 
 Windows:
 
 ```sh
 pip install zyme
 ```
 
 ## Usage example
 
+---
+
 A few motivating and useful examples of how your product can be used. Spice this up with code blocks and potentially more screenshots.
 
 _For more examples and usage, please refer to the [Wiki][wiki]._
 
 ## Development setup
 
+---
+
 Describe how to install all development dependencies and how to run an automated test-suite of some kind. Potentially do this for multiple platforms.
 
 ```sh
 pip install --editable zyme
 ```
 
 ## Documentation
 
-### - [**Read the Docs**](https://zyme.readthedocs.io/en/latest/)
+---
 
-### - [**Wiki**](https://github.com/Stephen-RA-King/zyme/wiki)
+[**Read the Docs**](https://zyme.readthedocs.io/en/latest/)
+
+-   [**Example Usage**](https://zyme.readthedocs.io/en/latest/example.html)
+-   [**Credits**](https://zyme.readthedocs.io/en/latest/example.html)
+-   [**Changelog**](https://zyme.readthedocs.io/en/latest/changelog.html)
+-   [**API Reference**](https://zyme.readthedocs.io/en/latest/autoapi/index.html)
+
+[**Wiki**](https://github.com/Stephen-RA-King/zyme/wiki)
 
 ## Meta
 
-[![](assets/linkedin.png)](https://linkedin.com/in/stephen-k-3a4644210)
+---
+
+[![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
-[![](assets/pypi.png)](https://pypi.org/project/zyme/)
+[![](assets/pypi.png)](https://pypi.org/project/zyme)
+[![Docker](assets/docker.png)](https://hub.docker.com/r/sraking/zyme)
 [![](assets/www.png)](https://www.justpython.tech)
-[![](assets/email.png)](mailto:stephen.ra.king@gmail.com)
-[![](assets/cv.png)](https://www.justpython.tech/cv)
+[![](assets/email.png)](mailto:sking.github@gmail.com)
+[![](assets/github.png)](https://github.com/Stephen-RA-King/zyme)
 
-Stephen R A King : stephen.ra.king@gmail.com
+Author: Stephen R A King ([sking.github@gmail.com](mailto:sking.github@gmail.com))
 
-Distributed under the MIT license. See [license](license-url) for more information.
+Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-[https://github.com/Stephen-RA-King/zyme](https://github.com/Stephen-RA-King/zyme)
+Created with Cookiecutter template: [![pydough][pydough-image]][pydough-url] version 1.3.3
 
-Created with Cookiecutter template: [**cc_template**][cc_template-url] version 1.1.1
+Digital object identifier: [![DOI](https://zenodo.org/badge/xxxxxxxxx.svg)](https://zenodo.org/badge/latestdoi/xxxxxxxxx)
 
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
-[cc_template-url]: https://github.com/Stephen-RA-King/cc_template
 [codeclimate-image]: https://api.codeclimate.com/v1/badges/7fc352185512a1dab75d/maintainability
 [codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/zyme/maintainability
 [codecov-image]: https://codecov.io/gh/Stephen-RA-King/zyme/branch/main/graph/badge.svg
 [codecov-url]: https://app.codecov.io/gh/Stephen-RA-King/zyme
 [codefactor-image]: https://www.codefactor.io/repository/github/Stephen-RA-King/zyme/badge
 [codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/zyme
-[codeql-image]: https://github.com/Stephen-RA-King/zyme/actions/workflows/codeql-analysis.yml/badge.svg
-[codeql-url]: https://github.com/Stephen-RA-King/zyme/actions/workflows/codeql-analysis.yml
+[codeql-image]: https://github.com/Stephen-RA-King/zyme/actions/workflows/github-code-scanning/codeql/badge.svg
+[codeql-url]: https://github.com/Stephen-RA-King/zyme/actions/workflows/github-code-scanning/codeql
 [commitizen-image]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
 [commitizen-url]: http://commitizen.github.io/cz-cli/
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square
 [conventional-commits-url]: https://conventionalcommits.org
 [deepsource-image]: https://static.deepsource.io/deepsource-badge-light-mini.svg
 [deepsource-url]: https://deepsource.io/gh/Stephen-RA-King/zyme/?ref=repository-badge
+[docker-image]: https://github.com/Stephen-RA-King/zyme/actions/workflows/docker-image.yml/badge.svg
+[docker-url]: https://github.com/Stephen-RA-King/zyme/actions/workflows/docker-image.yml
 [downloads-image]: https://static.pepy.tech/personalized-badge/zyme?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
 [downloads-url]: https://pepy.tech/project/zyme
 [format-image]: https://img.shields.io/pypi/format/zyme
 [isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
 [isort-url]: https://github.com/pycqa/isort/
 [lgtm-alerts-image]: https://img.shields.io/lgtm/alerts/g/Stephen-RA-King/zyme.svg?logo=lgtm&logoWidth=18
 [lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/zyme/alerts/
 [lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/zyme.svg?logo=lgtm&logoWidth=18
 [lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/zyme/context:python
 [license-image]: https://img.shields.io/pypi/l/zyme
-[license-url]: https://github.com/Stephen-RA-King/zyme/blob/main/license
+[license-url]: https://github.com/Stephen-RA-King/zyme/blob/main/LICENSE
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
+[openssf-image]: https://api.securityscorecards.dev/projects/github.com/Stephen-RA-King/zyme/badge
+[openssf-url]: https://api.securityscorecards.dev/projects/github.com/Stephen-RA-King/zyme
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
-[pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/gitwatch/main.svg
-[pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/gitwatch/main
+[pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/zyme/main.svg
+[pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/zyme/main
+[pydough-image]: https://img.shields.io/badge/pydough-2023-orange
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [pypi-url]: https://pypi.org/project/zyme/
 [pypi-image]: https://img.shields.io/pypi/v/zyme.svg
 [python-version-image]: https://img.shields.io/pypi/pyversions/zyme
 [readthedocs-image]: https://readthedocs.org/projects/zyme/badge/?version=latest
 [readthedocs-url]: https://zyme.readthedocs.io/en/latest/?badge=latest
-[requirements-status-image]: https://requires.io/github/Stephen-RA-King/zyme/requirements.svg?branch=main
-[requirements-status-url]: https://requires.io/github/Stephen-RA-King/zyme/requirements/?branch=main
 [status-image]: https://img.shields.io/pypi/status/zyme.svg
 [tests-image]: https://github.com/Stephen-RA-King/zyme/actions/workflows/tests.yml/badge.svg
 [tests-url]: https://github.com/Stephen-RA-King/zyme/actions/workflows/tests.yml
 [wiki]: https://github.com/Stephen-RA-King/zyme/wiki
```

