# Comparing `tmp/browniebroke_utils-0.1.0.tar.gz` & `tmp/browniebroke_utils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browniebroke_utils-0.1.0.tar", max compression
+gzip compressed data, was "browniebroke_utils-1.0.0.tar", max compression
```

## Comparing `browniebroke_utils-0.1.0.tar` & `browniebroke_utils-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1068 2022-11-18 20:29:13.459728 browniebroke_utils-0.1.0/LICENSE
--rw-r--r--   0        0        0     4483 2022-11-20 13:51:17.343748 browniebroke_utils-0.1.0/README.md
--rw-r--r--   0        0        0     2098 2022-11-20 13:53:59.325847 browniebroke_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2022-11-20 13:53:59.326265 browniebroke_utils-0.1.0/src/browniebroke_utils/__init__.py
--rw-r--r--   0        0        0        0 2022-11-18 20:29:13.596270 browniebroke_utils-0.1.0/src/browniebroke_utils/py.typed
--rw-r--r--   0        0        0     1106 2022-11-20 13:51:17.345011 browniebroke_utils-0.1.0/src/browniebroke_utils/setup_prettier.py
--rw-r--r--   0        0        0      343 2022-11-20 13:51:17.345438 browniebroke_utils-0.1.0/src/browniebroke_utils/setup_pywatchers.py
--rw-r--r--   0        0        0      264 2022-11-20 13:51:17.346176 browniebroke_utils-0.1.0/src/browniebroke_utils/templates/prettier/prettier.xml
--rw-r--r--   0        0        0      449 2022-11-20 13:51:17.346511 browniebroke_utils-0.1.0/src/browniebroke_utils/templates/prettier/to_add.xml
--rw-r--r--   0        0        0     2731 2022-11-20 13:51:17.346996 browniebroke_utils-0.1.0/src/browniebroke_utils/templates/pywatchers/watchers.xml
--rw-r--r--   0        0        0     5634 1970-01-01 00:00:00.000000 browniebroke_utils-0.1.0/setup.py
--rw-r--r--   0        0        0     5673 1970-01-01 00:00:00.000000 browniebroke_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-27 11:45:42.997304 browniebroke_utils-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4519 2023-06-27 11:45:42.997304 browniebroke_utils-1.0.0/README.md
+-rw-r--r--   0        0        0     2194 2023-06-27 11:45:44.197297 browniebroke_utils-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-27 11:45:44.145297 browniebroke_utils-1.0.0/src/browniebroke_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:45:42.997304 browniebroke_utils-1.0.0/src/browniebroke_utils/py.typed
+-rw-r--r--   0        0        0     1106 2023-06-27 11:45:42.997304 browniebroke_utils-1.0.0/src/browniebroke_utils/setup_prettier.py
+-rw-r--r--   0        0        0      343 2023-06-27 11:45:42.997304 browniebroke_utils-1.0.0/src/browniebroke_utils/setup_pywatchers.py
+-rw-r--r--   0        0        0      264 2023-06-27 11:45:42.997304 browniebroke_utils-1.0.0/src/browniebroke_utils/templates/prettier/prettier.xml
+-rw-r--r--   0        0        0      449 2023-06-27 11:45:42.997304 browniebroke_utils-1.0.0/src/browniebroke_utils/templates/prettier/to_add.xml
+-rw-r--r--   0        0        0     2731 2023-06-27 11:45:42.997304 browniebroke_utils-1.0.0/src/browniebroke_utils/templates/pywatchers/watchers.xml
+-rw-r--r--   0        0        0     5771 1970-01-01 00:00:00.000000 browniebroke_utils-1.0.0/PKG-INFO
```

### Comparing `browniebroke_utils-0.1.0/LICENSE` & `browniebroke_utils-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `browniebroke_utils-0.1.0/README.md` & `browniebroke_utils-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Browniebroke Utils
 
 <p align="center">
-  <a href="https://github.com/browniebroke/browniebroke-utils/actions?query=workflow%3ACI">
-    <img src="https://img.shields.io/github/workflow/status/browniebroke/browniebroke-utils/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >
+  <a href="https://github.com/browniebroke/browniebroke-utils/actions/workflows/ci.yml?query=branch%3Amain">
+    <img src="https://img.shields.io/github/actions/workflow/status/browniebroke/browniebroke-utils/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >
   </a>
   <a href="https://codecov.io/gh/browniebroke/browniebroke-utils">
     <img src="https://img.shields.io/codecov/c/github/browniebroke/browniebroke-utils.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
   </a>
 </p>
 <p align="center">
   <a href="https://python-poetry.org/">
```

### Comparing `browniebroke_utils-0.1.0/pyproject.toml` & `browniebroke_utils-1.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "browniebroke-utils"
-version = "0.1.0"
+version = "1.0.0"
 description = "A collections of small scripts."
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/browniebroke/browniebroke-utils"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
@@ -16,22 +16,24 @@
 packages = [
     { include = "browniebroke_utils", from = "src" },
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/browniebroke/browniebroke-utils/issues"
 "Changelog" = "https://github.com/browniebroke/browniebroke-utils/blob/main/CHANGELOG.md"
+"Twitter" = "https://twitter.com/_BrunoAlla"
+"Mastodon" = "https://fosstodon.org/@browniebroke"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 xmltodict = "^0.13.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
-pytest-cov = "^3.0"
+pytest-cov = "^4.0"
 pyfakefs = "^5.0.0"
 
 [tool.poetry.scripts]
 pych-prettier = "browniebroke_utils.setup_prettier:main"
 pych-pywatchers = "browniebroke_utils.setup_pywatchers:main"
 
 [tool.semantic_release]
```

### Comparing `browniebroke_utils-0.1.0/src/browniebroke_utils/setup_prettier.py` & `browniebroke_utils-1.0.0/src/browniebroke_utils/setup_prettier.py`

 * *Files identical despite different names*

### Comparing `browniebroke_utils-0.1.0/src/browniebroke_utils/templates/pywatchers/watchers.xml` & `browniebroke_utils-1.0.0/src/browniebroke_utils/templates/pywatchers/watchers.xml`

 * *Files identical despite different names*

### Comparing `browniebroke_utils-0.1.0/setup.py` & `browniebroke_utils-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,114 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: browniebroke-utils
+Version: 1.0.0
+Summary: A collections of small scripts.
+Home-page: https://github.com/browniebroke/browniebroke-utils
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
+Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
+Project-URL: Bug Tracker, https://github.com/browniebroke/browniebroke-utils/issues
+Project-URL: Changelog, https://github.com/browniebroke/browniebroke-utils/blob/main/CHANGELOG.md
+Project-URL: Mastodon, https://fosstodon.org/@browniebroke
+Project-URL: Repository, https://github.com/browniebroke/browniebroke-utils
+Project-URL: Twitter, https://twitter.com/_BrunoAlla
+Description-Content-Type: text/markdown
+
+# Browniebroke Utils
+
+<p align="center">
+  <a href="https://github.com/browniebroke/browniebroke-utils/actions/workflows/ci.yml?query=branch%3Amain">
+    <img src="https://img.shields.io/github/actions/workflow/status/browniebroke/browniebroke-utils/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >
+  </a>
+  <a href="https://codecov.io/gh/browniebroke/browniebroke-utils">
+    <img src="https://img.shields.io/codecov/c/github/browniebroke/browniebroke-utils.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
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
+  <a href="https://pypi.org/project/browniebroke-utils/">
+    <img src="https://img.shields.io/pypi/v/browniebroke-utils.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
+  </a>
+  <img src="https://img.shields.io/pypi/pyversions/browniebroke-utils.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
+  <img src="https://img.shields.io/pypi/l/browniebroke-utils.svg?style=flat-square" alt="License">
+</p>
+
+A collections of small scripts.
+
+## Installation
+
+Install this via pip (or your favourite package manager):
+
+`pip install browniebroke-utils`
+
+## Usage
+
+This tool provides a few random scripts I use in my day to day work.
+
+### `pych-prettier`
+
+Configure [Prettier](https://prettier.io/) as file watcher in the current PyCharm project. This is done by editing the appropriate files in the `.idea` folder.
+
+### `pych-pywatchers`
+
+Setup a few Python-related linting tools as file watchers in the current PyCharm project:
+
+- Black
+- isort
+- pyupgrade
+
+This is done by editing the appropriate files in the `.idea` folder.
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
+      <td align="center" valign="top" width="14.28%"><a href="https://browniebroke.com/"><img src="https://avatars.githubusercontent.com/u/861044?v=4?s=80" width="80px;" alt="Bruno Alla"/><br /><sub><b>Bruno Alla</b></sub></a><br /><a href="https://github.com/browniebroke/browniebroke-utils/commits?author=browniebroke" title="Code">💻</a> <a href="#ideas-browniebroke" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/browniebroke/browniebroke-utils/commits?author=browniebroke" title="Documentation">📖</a></td>
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
+[Copier](https://copier.readthedocs.io/) and the
+[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-template)
+project template.
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['browniebroke_utils']
-
-package_data = \
-{'': ['*'],
- 'browniebroke_utils': ['templates/prettier/*', 'templates/pywatchers/*']}
-
-install_requires = \
-['xmltodict>=0.13.0,<0.14.0']
-
-entry_points = \
-{'console_scripts': ['pych-prettier = browniebroke_utils.setup_prettier:main',
-                     'pych-pywatchers = '
-                     'browniebroke_utils.setup_pywatchers:main']}
-
-setup_kwargs = {
-    'name': 'browniebroke-utils',
-    'version': '0.1.0',
-    'description': 'A collections of small scripts.',
-    'long_description': '# Browniebroke Utils\n\n<p align="center">\n  <a href="https://github.com/browniebroke/browniebroke-utils/actions?query=workflow%3ACI">\n    <img src="https://img.shields.io/github/workflow/status/browniebroke/browniebroke-utils/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://codecov.io/gh/browniebroke/browniebroke-utils">\n    <img src="https://img.shields.io/codecov/c/github/browniebroke/browniebroke-utils.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/browniebroke-utils/">\n    <img src="https://img.shields.io/pypi/v/browniebroke-utils.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/browniebroke-utils.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/browniebroke-utils.svg?style=flat-square" alt="License">\n</p>\n\nA collections of small scripts.\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install browniebroke-utils`\n\n## Usage\n\nThis tool provides a few random scripts I use in my day to day work.\n\n### `pych-prettier`\n\nConfigure [Prettier](https://prettier.io/) as file watcher in the current PyCharm project. This is done by editing the appropriate files in the `.idea` folder.\n\n### `pych-pywatchers`\n\nSetup a few Python-related linting tools as file watchers in the current PyCharm project:\n\n- Black\n- isort\n- pyupgrade\n\nThis is done by editing the appropriate files in the `.idea` folder.\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tbody>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="https://browniebroke.com/"><img src="https://avatars.githubusercontent.com/u/861044?v=4?s=80" width="80px;" alt="Bruno Alla"/><br /><sub><b>Bruno Alla</b></sub></a><br /><a href="https://github.com/browniebroke/browniebroke-utils/commits?author=browniebroke" title="Code">💻</a> <a href="#ideas-browniebroke" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/browniebroke/browniebroke-utils/commits?author=browniebroke" title="Documentation">📖</a></td>\n    </tr>\n  </tbody>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Copier](https://copier.readthedocs.io/) and the\n[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-template)\nproject template.\n',
-    'author': 'Bruno Alla',
-    'author_email': 'alla.brunoo@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/browniebroke/browniebroke-utils',
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
@@ -1,38 +1,39 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['browniebroke_utils'] package_data = \ {'': ['*'],
-'browniebroke_utils': ['templates/prettier/*', 'templates/pywatchers/*']}
-install_requires = \ ['xmltodict>=0.13.0,<0.14.0'] entry_points = \
-{'console_scripts': ['pych-prettier = browniebroke_utils.setup_prettier:main',
-'pych-pywatchers = ' 'browniebroke_utils.setup_pywatchers:main']} setup_kwargs
-= { 'name': 'browniebroke-utils', 'version': '0.1.0', 'description': 'A
-collections of small scripts.', 'long_description': '# Browniebroke Utils\n\n
-            \n \n_[CI_Status]\n\n \n_[Test_coverage_percentage]\n\n
-\n
-             \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
-\n
-      \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
-\n\nA collections of small scripts.\n\n## Installation\n\nInstall this via pip
-(or your favourite package manager):\n\n`pip install browniebroke-utils`\n\n##
-Usage\n\nThis tool provides a few random scripts I use in my day to day
-work.\n\n### `pych-prettier`\n\nConfigure [Prettier](https://prettier.io/) as
-file watcher in the current PyCharm project. This is done by editing the
-appropriate files in the `.idea` folder.\n\n### `pych-pywatchers`\n\nSetup a
-few Python-related linting tools as file watchers in the current PyCharm
-project:\n\n- Black\n- isort\n- pyupgrade\n\nThis is done by editing the
-appropriate files in the `.idea` folder.\n\n## Contributors â¨\n\nThanks goes
-to these wonderful people ([emoji key](https://allcontributors.org/docs/en/
-emoji-key)):\n\n\n\n\n\n
+Metadata-Version: 2.1 Name: browniebroke-utils Version: 1.0.0 Summary: A
+collections of small scripts. Home-page: https://github.com/browniebroke/
+browniebroke-utils License: MIT Author: Bruno Alla Author-email:
+alla.brunoo@gmail.com Requires-Python: >=3.8,<4.0 Classifier: Development
+Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
+License :: OSI Approved :: MIT License Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Software Development :: Libraries Requires-Dist: xmltodict
+(>=0.13.0,<0.14.0) Project-URL: Bug Tracker, https://github.com/browniebroke/
+browniebroke-utils/issues Project-URL: Changelog, https://github.com/
+browniebroke/browniebroke-utils/blob/main/CHANGELOG.md Project-URL: Mastodon,
+https://fosstodon.org/@browniebroke Project-URL: Repository, https://
+github.com/browniebroke/browniebroke-utils Project-URL: Twitter, https://
+twitter.com/_BrunoAlla Description-Content-Type: text/markdown # Browniebroke
+Utils
+                    [CI_Status] [Test_coverage_percentage]
+                         [Poetry] [black] [pre-commit]
+             [PyPI_Version] [Supported Python versions] [License]
+A collections of small scripts. ## Installation Install this via pip (or your
+favourite package manager): `pip install browniebroke-utils` ## Usage This tool
+provides a few random scripts I use in my day to day work. ### `pych-prettier`
+Configure [Prettier](https://prettier.io/) as file watcher in the current
+PyCharm project. This is done by editing the appropriate files in the `.idea`
+folder. ### `pych-pywatchers` Setup a few Python-related linting tools as file
+watchers in the current PyCharm project: - Black - isort - pyupgrade This is
+done by editing the appropriate files in the `.idea` folder. ## Contributors
+â¨ Thanks goes to these wonderful people ([emoji key](https://
+allcontributors.org/docs/en/emoji-key)):
        [Bruno_Alla]
         Bruno_Alla
       ð» ð¤ ð
-\n\n\n\n\n\n\n\nThis project follows the [all-contributors](https://github.com/
-all-contributors/all-contributors) specification. Contributions of any kind
-welcome!\n\n## Credits\n\nThis package was created with\n[Copier](https://
-copier.readthedocs.io/) and the\n[browniebroke/pypackage-template](https://
-github.com/browniebroke/pypackage-template)\nproject template.\n', 'author':
-'Bruno Alla', 'author_email': 'alla.brunoo@gmail.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://github.com/browniebroke/
-browniebroke-utils', 'package_dir': package_dir, 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'entry_points': entry_points, 'python_requires': '>=3.7,<4.0', } setup
-(**setup_kwargs)
+    This project follows the [all-contributors](https://github.com/all-
+contributors/all-contributors) specification. Contributions of any kind
+welcome! ## Credits This package was created with [Copier](https://
+copier.readthedocs.io/) and the [browniebroke/pypackage-template](https://
+github.com/browniebroke/pypackage-template) project template.
```

