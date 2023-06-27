# Comparing `tmp/pelican-syntax-highlighting-0.4.1.tar.gz` & `tmp/pelican_syntax_highlighting-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican-syntax-highlighting-0.4.1.tar", max compression
+gzip compressed data, was "pelican_syntax_highlighting-0.4.2.tar", max compression
```

## Comparing `pelican-syntax-highlighting-0.4.1.tar` & `pelican_syntax_highlighting-0.4.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1497 2022-09-28 13:56:51.877143 pelican-syntax-highlighting-0.4.1/README.md
--rw-r--r--   0        0        0       56 2022-09-28 13:56:51.877143 pelican-syntax-highlighting-0.4.1/pelican/plugins/syntax_highlighting/__init__.py
--rw-r--r--   0        0        0     2291 2022-09-28 13:56:51.877143 pelican-syntax-highlighting-0.4.1/pelican/plugins/syntax_highlighting/markdown_extension.py
--rw-r--r--   0        0        0      979 2022-09-28 13:56:51.877143 pelican-syntax-highlighting-0.4.1/pelican/plugins/syntax_highlighting/settings.py
--rw-r--r--   0        0        0      454 2022-09-28 13:56:51.877143 pelican-syntax-highlighting-0.4.1/pelican/plugins/syntax_highlighting/syntax_highlighting.py
--rw-r--r--   0        0        0       27 2022-09-28 13:56:51.877143 pelican-syntax-highlighting-0.4.1/pelican/plugins/syntax_highlighting/test_syntax_highlighting.py
--rw-r--r--   0        0        0     2013 2022-09-28 13:57:05.945977 pelican-syntax-highlighting-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2377 1970-01-01 00:00:00.000000 pelican-syntax-highlighting-0.4.1/setup.py
--rw-r--r--   0        0        0     2822 1970-01-01 00:00:00.000000 pelican-syntax-highlighting-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1497 2021-10-19 07:58:43.057440 pelican_syntax_highlighting-0.4.2/README.md
+-rw-r--r--   0        0        0       56 2021-10-18 11:30:00.745186 pelican_syntax_highlighting-0.4.2/pelican/plugins/syntax_highlighting/__init__.py
+-rw-r--r--   0        0        0     2291 2022-09-28 13:50:46.710592 pelican_syntax_highlighting-0.4.2/pelican/plugins/syntax_highlighting/markdown_extension.py
+-rw-r--r--   0        0        0      979 2022-04-08 10:07:27.634834 pelican_syntax_highlighting-0.4.2/pelican/plugins/syntax_highlighting/settings.py
+-rw-r--r--   0        0        0      454 2021-11-01 10:33:13.308534 pelican_syntax_highlighting-0.4.2/pelican/plugins/syntax_highlighting/syntax_highlighting.py
+-rw-r--r--   0        0        0       27 2021-10-18 11:18:55.775148 pelican_syntax_highlighting-0.4.2/pelican/plugins/syntax_highlighting/test_syntax_highlighting.py
+-rw-r--r--   0        0        0     2010 2023-06-27 10:49:34.546923 pelican_syntax_highlighting-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2874 1970-01-01 00:00:00.000000 pelican_syntax_highlighting-0.4.2/PKG-INFO
```

### Comparing `pelican-syntax-highlighting-0.4.1/README.md` & `pelican_syntax_highlighting-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pelican-syntax-highlighting-0.4.1/pelican/plugins/syntax_highlighting/markdown_extension.py` & `pelican_syntax_highlighting-0.4.2/pelican/plugins/syntax_highlighting/markdown_extension.py`

 * *Files identical despite different names*

### Comparing `pelican-syntax-highlighting-0.4.1/pelican/plugins/syntax_highlighting/settings.py` & `pelican_syntax_highlighting-0.4.2/pelican/plugins/syntax_highlighting/settings.py`

 * *Files identical despite different names*

### Comparing `pelican-syntax-highlighting-0.4.1/pyproject.toml` & `pelican_syntax_highlighting-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 documentation = "https://docs.getpelican.com"
 keywords = ["pelican", "plugin"]
 license = "AGPL-3.0"
 name = "pelican-syntax-highlighting"
 packages = [{include = "pelican"}]
 readme = "README.md"
 repository = "https://github.com/f-koehler/pelican-syntax-highlighting"
-version = "0.4.1"
+version = "0.4.2"
 
 classifiers = [
   "Development Status :: 1 - Planning",
   "Environment :: Console",
   "Framework :: Pelican",
   "Framework :: Pelican :: Plugins",
   "Intended Audience :: End Users/Desktop",
@@ -28,25 +28,25 @@
 [tool.poetry.dependencies]
 markdown = {version = ">=3.2", optional = true}
 pelican = ">=4.5"
 python = ">=3.10,<4.0"
 
 [tool.poetry.dev-dependencies]
 Werkzeug = "^2.0"
-black = {version = "^22.1", allow-prereleases = true}
-flake8 = "^5.0"
+black = {version = "^23.1", allow-prereleases = true}
+flake8 = "^6.0"
 flake8-black = "^0.3"
-invoke = "^1.3"
+invoke = "^2.0"
 isort = "^5.4"
 livereload = "^2.6"
 markdown = "^3.2"
-mypy = "^0.981"
-pre-commit = "^2.15.0"
+mypy = "^1.0"
+pre-commit = "^3.0.0"
 pytest = "^7.0"
-pytest-cov = "^3.0"
+pytest-cov = "^4.0"
 pytest-pythonpath = "^0.7"
 pytest-sugar = "^0.9"
 types-Markdown = "^3.3.6"
 
 [tool.poetry.extras]
 markdown = ["markdown"]
```

### Comparing `pelican-syntax-highlighting-0.4.1/setup.py` & `pelican_syntax_highlighting-0.4.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,63 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pelican-syntax-highlighting
+Version: 0.4.2
+Summary: Highlight syntax using Prism.js, Highlight.js or Pygments
+Home-page: https://github.com/f-koehler/pelican-syntax-highlighting
+License: AGPL-3.0
+Keywords: pelican,plugin
+Author: Fabian Köhler
+Author-email: fabian.koehler@protonmail.ch
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 1 - Planning
+Classifier: Environment :: Console
+Classifier: Framework :: Pelican
+Classifier: Framework :: Pelican :: Plugins
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: markdown
+Requires-Dist: markdown (>=3.2) ; extra == "markdown"
+Requires-Dist: pelican (>=4.5)
+Project-URL: Documentation, https://docs.getpelican.com
+Project-URL: Funding, https://donate.getpelican.com/
+Project-URL: Issue Tracker, https://github.com/f-koehler/pelican-syntax-highlighting/issues
+Project-URL: Repository, https://github.com/f-koehler/pelican-syntax-highlighting
+Description-Content-Type: text/markdown
+
+# Syntax Highlighting: A Plugin for Pelican
+
+[![Build Status](https://github.com/f-koehler/pelican-syntax-highlighting/actions/workflows/main.yml/badge.svg)](https://github.com/f-koehler/pelican-syntax-highlighting/actions/workflows/main.yml)
+[![PyPI Version](https://img.shields.io/pypi/v/pelican-syntax-highlighting)](https://pypi.org/project/pelican-syntax-highlighting/)
+![License](https://img.shields.io/pypi/l/pelican-syntax-highlighting?color=blue)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/f-koehler/pelican-syntax-highlighting/main.svg)](https://results.pre-commit.ci/latest/github/f-koehler/pelican-syntax-highlighting/main)
+
+Highlight syntax using Prism.js, Highlight.js or Pygments
+
+## Installation
+
+This plugin can be installed via:
+
+    python -m pip install pelican-syntax-highlighting
+
+## Usage
+
+<<Add plugin details here>>
+
+## Contributing
+
+Contributions are welcome and much appreciated. Every little bit helps. You can contribute by improving the documentation, adding missing features, and fixing bugs. You can also help out by reviewing and commenting on [existing issues][].
 
-packages = \
-['pelican', 'pelican.plugins.syntax_highlighting']
+To start contributing to this plugin, review the [Contributing to Pelican][] documentation, beginning with the **Contributing Code** section.
 
-package_data = \
-{'': ['*']}
+[existing issues]: https://github.com/f-koehler/pelican-syntax-highlighting/issues
+[contributing to pelican]: https://docs.getpelican.com/en/latest/contribute.html
 
-install_requires = \
-['pelican>=4.5']
-
-extras_require = \
-{'markdown': ['markdown>=3.2']}
-
-setup_kwargs = {
-    'name': 'pelican-syntax-highlighting',
-    'version': '0.4.1',
-    'description': 'Highlight syntax using Prism.js, Highlight.js or Pygments',
-    'long_description': '# Syntax Highlighting: A Plugin for Pelican\n\n[![Build Status](https://github.com/f-koehler/pelican-syntax-highlighting/actions/workflows/main.yml/badge.svg)](https://github.com/f-koehler/pelican-syntax-highlighting/actions/workflows/main.yml)\n[![PyPI Version](https://img.shields.io/pypi/v/pelican-syntax-highlighting)](https://pypi.org/project/pelican-syntax-highlighting/)\n![License](https://img.shields.io/pypi/l/pelican-syntax-highlighting?color=blue)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/f-koehler/pelican-syntax-highlighting/main.svg)](https://results.pre-commit.ci/latest/github/f-koehler/pelican-syntax-highlighting/main)\n\nHighlight syntax using Prism.js, Highlight.js or Pygments\n\n## Installation\n\nThis plugin can be installed via:\n\n    python -m pip install pelican-syntax-highlighting\n\n## Usage\n\n<<Add plugin details here>>\n\n## Contributing\n\nContributions are welcome and much appreciated. Every little bit helps. You can contribute by improving the documentation, adding missing features, and fixing bugs. You can also help out by reviewing and commenting on [existing issues][].\n\nTo start contributing to this plugin, review the [Contributing to Pelican][] documentation, beginning with the **Contributing Code** section.\n\n[existing issues]: https://github.com/f-koehler/pelican-syntax-highlighting/issues\n[contributing to pelican]: https://docs.getpelican.com/en/latest/contribute.html\n\n## License\n\nThis project is licensed under the AGPL-3.0 license.\n',
-    'author': 'Fabian Köhler',
-    'author_email': 'fabian.koehler@protonmail.ch',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/f-koehler/pelican-syntax-highlighting',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.10,<4.0',
-}
+## License
 
+This project is licensed under the AGPL-3.0 license.
 
-setup(**setup_kwargs)
```

