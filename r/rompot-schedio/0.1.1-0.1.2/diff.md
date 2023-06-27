# Comparing `tmp/rompot_schedio-0.1.1.tar.gz` & `tmp/rompot_schedio-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rompot_schedio-0.1.1.tar", max compression
+gzip compressed data, was "rompot_schedio-0.1.2.tar", max compression
```

## Comparing `rompot_schedio-0.1.1.tar` & `rompot_schedio-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,49 @@
--rw-r--r--   0        0        0     1071 2023-04-26 18:59:19.955041 rompot_schedio-0.1.1/LICENSE
--rw-r--r--   0        0        0     3718 2023-04-26 18:59:19.955041 rompot_schedio-0.1.1/README.md
--rw-r--r--   0        0        0     2863 2023-04-26 18:59:48.464746 rompot_schedio-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      175 2023-04-26 18:59:19.959041 rompot_schedio-0.1.1/src/schedio/__cli__.py
--rw-r--r--   0        0        0      888 2023-04-26 18:59:19.959041 rompot_schedio-0.1.1/src/schedio/__init__.py
--rw-r--r--   0        0        0       22 2023-04-26 18:59:48.408743 rompot_schedio-0.1.1/src/schedio/_version.py
--rw-r--r--   0        0        0        0 2023-04-26 18:59:19.959041 rompot_schedio-0.1.1/src/schedio/conf/__init__.py
--rw-r--r--   0        0        0      236 2023-04-26 18:59:48.408743 rompot_schedio-0.1.1/src/schedio/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-26 18:59:19.959041 rompot_schedio-0.1.1/src/schedio/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-26 18:59:19.959041 rompot_schedio-0.1.1/src/schedio/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-26 18:59:19.959041 rompot_schedio-0.1.1/src/schedio/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-26 18:59:19.959041 rompot_schedio-0.1.1/src/schedio/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-26 18:59:19.959041 rompot_schedio-0.1.1/src/schedio/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-26 18:59:19.959041 rompot_schedio-0.1.1/src/schedio/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-26 18:59:19.959041 rompot_schedio-0.1.1/src/schedio/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-26 18:59:19.959041 rompot_schedio-0.1.1/src/schedio/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-26 18:59:19.959041 rompot_schedio-0.1.1/src/schedio/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-26 18:59:19.959041 rompot_schedio-0.1.1/src/schedio/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-26 18:59:19.959041 rompot_schedio-0.1.1/src/schedio/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-26 18:59:19.959041 rompot_schedio-0.1.1/src/schedio/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-26 18:59:19.959041 rompot_schedio-0.1.1/src/schedio/conf/project/__init__.yaml
--rw-r--r--   0        0        0       83 2023-04-26 18:59:19.959041 rompot_schedio-0.1.1/src/schedio/conf/task/__init__.yaml
--rw-r--r--   0        0        0      211 2023-04-26 18:59:19.959041 rompot_schedio-0.1.1/src/schedio/project.toml
--rw-r--r--   0        0        0        0 2023-04-26 18:59:19.959041 rompot_schedio-0.1.1/src/schedio/py.typed
--rw-r--r--   0        0        0     4379 1970-01-01 00:00:00.000000 rompot_schedio-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-27 12:42:10.208041 rompot_schedio-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2174 2023-06-27 12:42:10.208041 rompot_schedio-0.1.2/README.md
+-rw-r--r--   0        0        0     2963 2023-06-27 12:42:34.264232 rompot_schedio-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/__cli__.py
+-rw-r--r--   0        0        0      379 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-27 12:42:34.212232 rompot_schedio-0.1.2/src/schedio/_version.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/__init__.py
+-rw-r--r--   0        0        0      238 2023-06-27 12:42:34.212232 rompot_schedio-0.1.2/src/schedio/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      435 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      155 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      320 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/config.yaml
+-rw-r--r--   0        0        0      569 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      709 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      291 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      217 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      921 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/mode/debug.yaml
+-rw-r--r--   0        0        0       61 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       96 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/path/__default__.yaml
+-rw-r--r--   0        0        0     1719 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      412 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/path/__task__.yaml
+-rw-r--r--   0        0        0       76 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       72 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       74 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0      119 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      237 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      242 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0       92 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0       19 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/pipeline/__test__.yaml
+-rw-r--r--   0        0        0      742 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      168 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/project/__test__.yaml
+-rw-r--r--   0        0        0       36 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      176 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      319 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      311 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/task/__test__.yaml
+-rw-r--r--   0        0        0       97 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0       97 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/conf/workflow/__test__.yaml
+-rw-r--r--   0        0        0      211 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/project.toml
+-rw-r--r--   0        0        0        0 2023-06-27 12:42:10.212041 rompot_schedio-0.1.2/src/schedio/py.typed
+-rw-r--r--   0        0        0     2874 1970-01-01 00:00:00.000000 rompot_schedio-0.1.2/PKG-INFO
```

### Comparing `rompot_schedio-0.1.1/LICENSE` & `rompot_schedio-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rompot_schedio-0.1.1/README.md` & `rompot_schedio-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,66 @@
-# Rompot Schedio: A Python Library for Robotic Drawings
+Metadata-Version: 2.1
+Name: rompot-schedio
+Version: 0.1.2
+Summary: A Python Library for Robotic Drawings
+Home-page: https://rompot-schedio.entelecheia.ai
+License: MIT
+Author: Young Joon Lee
+Author-email: entelecheia@hotmail.com
+Requires-Python: >=3.8.1,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: hyfi (>=0.15.0,<0.16.0)
+Project-URL: Repository, https://github.com/entelecheia/rompot-schedio
+Description-Content-Type: text/markdown
+
+# Rompot Schedio
 
 [![pypi-image]][pypi-url]
-[![license-image]][license-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
+[![license-image]][license-url]
+[![codecov][codecov-image]][codecov-url]
 [![jupyter-book-image]][docs-url]
 
 <!-- Links: -->
-
+[codecov-image]: https://codecov.io/gh/entelecheia/rompot-schedio/branch/main/graph/badge.svg?token=MWRAQQYOS7
+[codecov-url]: https://codecov.io/gh/entelecheia/rompot-schedio
 [pypi-image]: https://img.shields.io/pypi/v/rompot-schedio
 [license-image]: https://img.shields.io/github/license/entelecheia/rompot-schedio
 [license-url]: https://github.com/entelecheia/rompot-schedio/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/rompot-schedio?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/rompot-schedio
 [release-url]: https://github.com/entelecheia/rompot-schedio/releases
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
+
 [repo-url]: https://github.com/entelecheia/rompot-schedio
 [pypi-url]: https://pypi.org/project/rompot-schedio
 [docs-url]: https://rompot-schedio.entelecheia.ai
 [changelog]: https://github.com/entelecheia/rompot-schedio/blob/main/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/rompot-schedio/blob/main/CONTRIBUTING.md
-
 <!-- Links: -->
 
+A Python Library for Robotic Drawings
+
 - Documentation: [https://rompot-schedio.entelecheia.ai][docs-url]
 - GitHub: [https://github.com/entelecheia/rompot-schedio][repo-url]
 - PyPI: [https://pypi.org/project/rompot-schedio][pypi-url]
 
 Rompot-Schedio is an innovative and versatile Python library designed to facilitate the creation, manipulation, and control of robotic drawings. The name Rompot-Schedio combines the Greek words ρομπότ (robot) and σχέδιο (drawing), embodying the library's mission to empower users to design, simulate, and execute robotic drawing projects with ease and precision.
 
-## Features
-
-Rompot-Schedio offers a wide array of features tailored to cater to both enthusiasts and professionals in the fields of robotics, art, and engineering:
-
-- **Intuitive API**: The library provides a user-friendly API, allowing users to easily design, simulate, and control robotic drawing systems with minimal lines of code.
-- **Cross-platform compatibility**: Rompot-Schedio is designed to work with various robotic platforms, including industrial manipulators, mobile robots, and custom-built drawing machines, ensuring adaptability and flexibility for different projects and requirements.
-- **Advanced drawing tools**: The library includes a collection of advanced drawing tools and algorithms, enabling users to create intricate patterns, geometric shapes, and artistic designs with precision and accuracy.
-- **Simulations and visualizations**: Rompot-Schedio offers built-in simulation and visualization capabilities, allowing users to test their designs and control strategies in a virtual environment before deploying them to physical robots.
-- **Path planning and optimization**: The library includes powerful path planning and optimization algorithms, ensuring efficient and smooth drawing trajectories, while minimizing errors and artifacts in the final output.
-- **Customizability**: Users can create custom drawing tools, robotic platforms, and control strategies, offering complete control over every aspect of their robotic drawing projects.
-
-## Installation
-
-You can install Rompot-Schedio using pip:
-
-```bash
-pip install rompot-schedio
-```
-
-## Getting Started
-
-To get started with Rompot-Schedio, check out the [official documentation][docs-url] and the [GitHub repository][repo-url] for examples, tutorials, and more information.
-
 ## Changelog
 
 See the [CHANGELOG] for more information.
 
 ## Contributing
 
 Contributions are welcome! Please see the [contributing guidelines] for more information.
 
 ## License
 
 This project is released under the [MIT License][license-url].
+
```

### Comparing `rompot_schedio-0.1.1/pyproject.toml` & `rompot_schedio-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 [tool.poetry]
 name = "rompot-schedio"
-version = "0.1.1"
+version = "0.1.2"
 description = "A Python Library for Robotic Drawings"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://rompot-schedio.entelecheia.ai"
 repository = "https://github.com/entelecheia/rompot-schedio"
 readme = "README.md"
 packages = [{ include = "schedio", from = "src" }]
 
 [tool.poetry.scripts]
 schedio = 'schedio.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.2.20"
+click = "^8.1.3"
+hyfi = "^0.15.0"
+
+[tool.poetry.group.dev]
+optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 flake8-pyproject = "^1.2.2"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 
+[tool.poe]
+include = [".tasks.toml", ".tasks-extra.toml"]
+
 [tool.black]
 exclude = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
 
 [tool.isort]
 profile = "black"
 skip = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
 
@@ -70,15 +77,14 @@
 addopts = "-p no:cacheprovider" # deactivating pytest caching.
 
 [tool.coverage.report]
 exclude_lines = ['if __name__ == "__main__":']
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.1"
 tag_format = "v$version"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/schedio/_version.py:__version__"
 version_pattern = 'src/schedio/conf/about/__init__.yaml:version: "{version}"'
@@ -87,13 +93,14 @@
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
-build_command = "poetry build --no-cache"
 hvcs = "github" # hosting version control system, gitlab is also supported
+build_command = "poetry build --no-cache"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
```

### Comparing `rompot_schedio-0.1.1/src/schedio/conf/hydra/help/help.yaml` & `rompot_schedio-0.1.2/src/schedio/conf/hydra/help/help.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 # Configuration generated with overrides:
 #   $CONFIG : Generated config
 #
 template: |-
   ${hydra.help.header} 
   
-  author: ${about.author}
+  authors: ${about.authors}
   description: ${about.description}
 
   ${hydra.help.app_name} Command Line Interface for Hydra
 
   == Configuration groups ==
 
   Compose your configuration from those groups (task=task_name)
```

### Comparing `rompot_schedio-0.1.1/src/schedio/conf/path/__default__.yaml` & `rompot_schedio-0.1.2/src/schedio/conf/path/__default__.yaml`

 * *Files identical despite different names*

