# Comparing `tmp/all_repos_envvar-0.3.0.tar.gz` & `tmp/all_repos_envvar-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "all_repos_envvar-0.3.0.tar", max compression
+gzip compressed data, was "all_repos_envvar-1.0.0.tar", max compression
```

## Comparing `all_repos_envvar-0.3.0.tar` & `all_repos_envvar-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1068 2022-11-20 15:11:57.473542 all_repos_envvar-0.3.0/LICENSE
--rw-r--r--   0        0        0     4746 2022-11-20 15:11:57.473542 all_repos_envvar-0.3.0/README.md
--rw-r--r--   0        0        0     1970 2022-11-20 15:11:58.313546 all_repos_envvar-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       22 2022-11-20 15:11:58.285546 all_repos_envvar-0.3.0/src/all_repos_envvar/__init__.py
--rw-r--r--   0        0        0      485 2022-11-20 15:11:57.473542 all_repos_envvar-0.3.0/src/all_repos_envvar/mixin.py
--rw-r--r--   0        0        0      167 2022-11-20 15:11:57.473542 all_repos_envvar-0.3.0/src/all_repos_envvar/push.py
--rw-r--r--   0        0        0        0 2022-11-20 15:11:57.473542 all_repos_envvar-0.3.0/src/all_repos_envvar/py.typed
--rw-r--r--   0        0        0      168 2022-11-20 15:11:57.473542 all_repos_envvar-0.3.0/src/all_repos_envvar/source.py
--rw-r--r--   0        0        0     5623 1970-01-01 00:00:00.000000 all_repos_envvar-0.3.0/setup.py
--rw-r--r--   0        0        0     6036 1970-01-01 00:00:00.000000 all_repos_envvar-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-27 11:39:30.286209 all_repos_envvar-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4782 2023-06-27 11:39:30.286209 all_repos_envvar-1.0.0/README.md
+-rw-r--r--   0        0        0     2072 2023-06-27 11:39:31.526219 all_repos_envvar-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-27 11:39:31.486219 all_repos_envvar-1.0.0/src/all_repos_envvar/__init__.py
+-rw-r--r--   0        0        0      485 2023-06-27 11:39:30.286209 all_repos_envvar-1.0.0/src/all_repos_envvar/mixin.py
+-rw-r--r--   0        0        0      167 2023-06-27 11:39:30.286209 all_repos_envvar-1.0.0/src/all_repos_envvar/push.py
+-rw-r--r--   0        0        0        0 2023-06-27 11:39:30.286209 all_repos_envvar-1.0.0/src/all_repos_envvar/py.typed
+-rw-r--r--   0        0        0      168 2023-06-27 11:39:30.286209 all_repos_envvar-1.0.0/src/all_repos_envvar/source.py
+-rw-r--r--   0        0        0     6134 1970-01-01 00:00:00.000000 all_repos_envvar-1.0.0/PKG-INFO
```

### Comparing `all_repos_envvar-0.3.0/LICENSE` & `all_repos_envvar-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `all_repos_envvar-0.3.0/README.md` & `all_repos_envvar-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # all-repos-envvar
 
 <p align="center">
-  <a href="https://github.com/browniebroke/all-repos-envvar/actions?query=workflow%3ACI">
-    <img src="https://img.shields.io/github/workflow/status/browniebroke/all-repos-envvar/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >
+  <a href="https://github.com/browniebroke/all-repos-envvar/actions/workflows/ci.yml?query=branch%3Amain">
+    <img src="https://img.shields.io/github/actions/workflow/status/browniebroke/all-repos-envvar/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >
   </a>
   <a href="https://codecov.io/gh/browniebroke/all-repos-envvar">
     <img src="https://img.shields.io/codecov/c/github/browniebroke/all-repos-envvar.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
   </a>
 </p>
 <p align="center">
   <a href="https://python-poetry.org/">
```

### Comparing `all_repos_envvar-0.3.0/pyproject.toml` & `all_repos_envvar-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "all-repos-envvar"
-version = "0.3.0"
+version = "1.0.0"
 description = "An all-repos extension to read values from environment variables."
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/browniebroke/all-repos-envvar"
 documentation = "https://all-repos-envvar.readthedocs.io"
 classifiers = [
@@ -17,21 +17,23 @@
 packages = [
     { include = "all_repos_envvar", from = "src" },
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/browniebroke/all-repos-envvar/issues"
 "Changelog" = "https://all-repos-envvar.readthedocs.io/changelog.html"
+"Twitter" = "https://twitter.com/_BrunoAlla"
+"Mastodon" = "https://fosstodon.org/@browniebroke"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 all-repos = ">=1"
 environs = "^9.4"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.0"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/all_repos_envvar/__init__.py:__version__"
```

### Comparing `all_repos_envvar-0.3.0/setup.py` & `all_repos_envvar-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,116 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: all-repos-envvar
+Version: 1.0.0
+Summary: An all-repos extension to read values from environment variables.
+Home-page: https://github.com/browniebroke/all-repos-envvar
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
+Requires-Dist: all-repos (>=1)
+Requires-Dist: environs (>=9.4,<10.0)
+Project-URL: Bug Tracker, https://github.com/browniebroke/all-repos-envvar/issues
+Project-URL: Changelog, https://all-repos-envvar.readthedocs.io/changelog.html
+Project-URL: Documentation, https://all-repos-envvar.readthedocs.io
+Project-URL: Mastodon, https://fosstodon.org/@browniebroke
+Project-URL: Repository, https://github.com/browniebroke/all-repos-envvar
+Project-URL: Twitter, https://twitter.com/_BrunoAlla
+Description-Content-Type: text/markdown
+
+# all-repos-envvar
+
+<p align="center">
+  <a href="https://github.com/browniebroke/all-repos-envvar/actions/workflows/ci.yml?query=branch%3Amain">
+    <img src="https://img.shields.io/github/actions/workflow/status/browniebroke/all-repos-envvar/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >
+  </a>
+  <a href="https://codecov.io/gh/browniebroke/all-repos-envvar">
+    <img src="https://img.shields.io/codecov/c/github/browniebroke/all-repos-envvar.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
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
+  <a href="https://pypi.org/project/all-repos-envvar/">
+    <img src="https://img.shields.io/pypi/v/all-repos-envvar.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
+  </a>
+  <img src="https://img.shields.io/pypi/pyversions/all-repos-envvar.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
+  <img src="https://img.shields.io/pypi/l/all-repos-envvar.svg?style=flat-square" alt="License">
+</p>
+
+An all-repos extension to read values from environment variables.
+
+## Installation
+
+Install this via pip (or your favourite package manager):
+
+`pip install all-repos-envvar`
+
+## Usage
+
+This library should be installed alongside `all-repos` so that it's findable at import time. It provides a custom `source` and `push` to get the GitHub API key from an environment variable `GITHUB_API_KEY` (reading from and `.env` file is also supported), allowing you to omit it from the config:
+
+```json
+{
+  "output_dir": "output",
+  "source": "all_repos_envvar.source",
+  "source_settings": {
+    "username": "browniebroke"
+  },
+  "push": "all_repos_envvar.push",
+  "push_settings": {
+    "username": "browniebroke"
+  }
+}
+```
 
-package_dir = \
-{'': 'src'}
+I wanted this feature, but it looks like it won't be implemented in the main repo, hence this little extension. The source module extends `all_repos.source.github` and the push module extends `all_repos.push.github_pull_request`
 
-packages = \
-['all_repos_envvar']
+## Contributors ✨
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['all-repos>=1', 'environs>=9.4,<10.0']
-
-setup_kwargs = {
-    'name': 'all-repos-envvar',
-    'version': '0.3.0',
-    'description': 'An all-repos extension to read values from environment variables.',
-    'long_description': '# all-repos-envvar\n\n<p align="center">\n  <a href="https://github.com/browniebroke/all-repos-envvar/actions?query=workflow%3ACI">\n    <img src="https://img.shields.io/github/workflow/status/browniebroke/all-repos-envvar/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://codecov.io/gh/browniebroke/all-repos-envvar">\n    <img src="https://img.shields.io/codecov/c/github/browniebroke/all-repos-envvar.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/all-repos-envvar/">\n    <img src="https://img.shields.io/pypi/v/all-repos-envvar.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/all-repos-envvar.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/all-repos-envvar.svg?style=flat-square" alt="License">\n</p>\n\nAn all-repos extension to read values from environment variables.\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install all-repos-envvar`\n\n## Usage\n\nThis library should be installed alongside `all-repos` so that it\'s findable at import time. It provides a custom `source` and `push` to get the GitHub API key from an environment variable `GITHUB_API_KEY` (reading from and `.env` file is also supported), allowing you to omit it from the config:\n\n```json\n{\n  "output_dir": "output",\n  "source": "all_repos_envvar.source",\n  "source_settings": {\n    "username": "browniebroke"\n  },\n  "push": "all_repos_envvar.push",\n  "push_settings": {\n    "username": "browniebroke"\n  }\n}\n```\n\nI wanted this feature, but it looks like it won\'t be implemented in the main repo, hence this little extension. The source module extends `all_repos.source.github` and the push module extends `all_repos.push.github_pull_request`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tr>\n    <td align="center"><a href="https://browniebroke.com/"><img src="https://avatars.githubusercontent.com/u/861044?v=4?s=80" width="80px;" alt=""/><br /><sub><b>Bruno Alla</b></sub></a><br /><a href="https://github.com/browniebroke/all-repos-envvar/commits?author=browniebroke" title="Code">💻</a> <a href="#ideas-browniebroke" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/browniebroke/all-repos-envvar/commits?author=browniebroke" title="Documentation">📖</a></td>\n  </tr>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject template.\n',
-    'author': 'Bruno Alla',
-    'author_email': 'alla.brunoo@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/browniebroke/all-repos-envvar',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- prettier-ignore-start -->
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tr>
+    <td align="center"><a href="https://browniebroke.com/"><img src="https://avatars.githubusercontent.com/u/861044?v=4?s=80" width="80px;" alt=""/><br /><sub><b>Bruno Alla</b></sub></a><br /><a href="https://github.com/browniebroke/all-repos-envvar/commits?author=browniebroke" title="Code">💻</a> <a href="#ideas-browniebroke" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/browniebroke/all-repos-envvar/commits?author=browniebroke" title="Documentation">📖</a></td>
+  </tr>
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
 
+This package was created with
+[Cookiecutter](https://github.com/audreyr/cookiecutter) and the
+[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)
+project template.
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,41 +1,45 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['all_repos_envvar'] package_data = \ {'': ['*']}
-install_requires = \ ['all-repos>=1', 'environs>=9.4,<10.0'] setup_kwargs =
-{ 'name': 'all-repos-envvar', 'version': '0.3.0', 'description': 'An all-repos
-extension to read values from environment variables.', 'long_description': '#
-all-repos-envvar\n\n
-            \n \n_[CI_Status]\n\n \n_[Test_coverage_percentage]\n\n
-\n
-             \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
-\n
-      \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
-\n\nAn all-repos extension to read values from environment variables.\n\n##
-Installation\n\nInstall this via pip (or your favourite package manager):
-\n\n`pip install all-repos-envvar`\n\n## Usage\n\nThis library should be
-installed alongside `all-repos` so that it\'s findable at import time. It
-provides a custom `source` and `push` to get the GitHub API key from an
-environment variable `GITHUB_API_KEY` (reading from and `.env` file is also
-supported), allowing you to omit it from the config:\n\n```json\n{\n
-"output_dir": "output",\n "source": "all_repos_envvar.source",\n
-"source_settings": {\n "username": "browniebroke"\n },\n "push":
-"all_repos_envvar.push",\n "push_settings": {\n "username": "browniebroke"\n
-}\n}\n```\n\nI wanted this feature, but it looks like it won\'t be implemented
-in the main repo, hence this little extension. The source module extends
+Metadata-Version: 2.1 Name: all-repos-envvar Version: 1.0.0 Summary: An all-
+repos extension to read values from environment variables. Home-page: https://
+github.com/browniebroke/all-repos-envvar License: MIT Author: Bruno Alla
+Author-email: alla.brunoo@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
+Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
+:: English Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Software Development :: Libraries Requires-
+Dist: all-repos (>=1) Requires-Dist: environs (>=9.4,<10.0) Project-URL: Bug
+Tracker, https://github.com/browniebroke/all-repos-envvar/issues Project-URL:
+Changelog, https://all-repos-envvar.readthedocs.io/changelog.html Project-URL:
+Documentation, https://all-repos-envvar.readthedocs.io Project-URL: Mastodon,
+https://fosstodon.org/@browniebroke Project-URL: Repository, https://
+github.com/browniebroke/all-repos-envvar Project-URL: Twitter, https://
+twitter.com/_BrunoAlla Description-Content-Type: text/markdown # all-repos-
+envvar
+                    [CI_Status] [Test_coverage_percentage]
+                         [Poetry] [black] [pre-commit]
+             [PyPI_Version] [Supported Python versions] [License]
+An all-repos extension to read values from environment variables. ##
+Installation Install this via pip (or your favourite package manager): `pip
+install all-repos-envvar` ## Usage This library should be installed alongside
+`all-repos` so that it's findable at import time. It provides a custom `source`
+and `push` to get the GitHub API key from an environment variable
+`GITHUB_API_KEY` (reading from and `.env` file is also supported), allowing you
+to omit it from the config: ```json { "output_dir": "output", "source":
+"all_repos_envvar.source", "source_settings": { "username": "browniebroke" },
+"push": "all_repos_envvar.push", "push_settings": { "username": "browniebroke"
+} } ``` I wanted this feature, but it looks like it won't be implemented in the
+main repo, hence this little extension. The source module extends
 `all_repos.source.github` and the push module extends
-`all_repos.push.github_pull_request`\n\n## Contributors â¨\n\nThanks goes to
-these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-
-key)):\n\n\n\n\n\n
+`all_repos.push.github_pull_request` ## Contributors â¨ Thanks goes to these
+wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
         Bruno_Alla
 
       ð» ð¤ ð
-\n\n\n\n\n\n\n\nThis project follows the [all-contributors](https://github.com/
-all-contributors/all-contributors) specification. Contributions of any kind
-welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https:/
-/github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-
-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject
-template.\n', 'author': 'Bruno Alla', 'author_email': 'alla.brunoo@gmail.com',
-'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://github.com/
-browniebroke/all-repos-envvar', 'package_dir': package_dir, 'packages':
-packages, 'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+    This project follows the [all-contributors](https://github.com/all-
+contributors/all-contributors) specification. Contributions of any kind
+welcome! ## Credits This package was created with [Cookiecutter](https://
+github.com/audreyr/cookiecutter) and the [browniebroke/cookiecutter-pypackage]
+(https://github.com/browniebroke/cookiecutter-pypackage) project template.
```

