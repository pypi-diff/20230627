# Comparing `tmp/simplesecurity-2022.tar.gz` & `tmp/simplesecurity-2023.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplesecurity-2022.tar", max compression
+gzip compressed data, was "simplesecurity-2023.tar", max compression
```

## Comparing `simplesecurity-2022.tar` & `simplesecurity-2023.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1100 2021-10-02 13:08:48.870092 simplesecurity-2022/LICENSE.md
--rw-r--r--   0        0        0     2211 2022-04-09 19:44:56.357123 simplesecurity-2022/pyproject.toml
--rw-r--r--   0        0        0     9318 2022-04-09 19:43:27.664767 simplesecurity-2022/README.md
--rw-r--r--   0        0        0     4906 2022-04-09 19:43:28.029555 simplesecurity-2022/simplesecurity/__init__.py
--rw-r--r--   0        0        0      116 2022-04-09 19:43:28.030553 simplesecurity-2022/simplesecurity/__main__.py
--rw-r--r--   0        0        0     2712 2022-04-09 19:43:28.022512 simplesecurity-2022/simplesecurity/filter.py
--rw-r--r--   0        0        0     8869 2022-04-09 19:43:28.024545 simplesecurity-2022/simplesecurity/formatter.py
--rw-r--r--   0        0        0      953 2022-04-09 19:43:28.025566 simplesecurity-2022/simplesecurity/level.py
--rw-r--r--   0        0        0     8658 2022-04-09 19:44:49.350292 simplesecurity-2022/simplesecurity/plugins.py
--rw-r--r--   0        0        0   163920 2022-04-09 19:23:16.490242 simplesecurity-2022/simplesecurity/semgrep_sec.yaml
--rw-r--r--   0        0        0      715 2022-04-09 19:43:28.028558 simplesecurity-2022/simplesecurity/types.py
--rw-r--r--   0        0        0    10340 2022-04-09 19:45:13.608602 simplesecurity-2022/setup.py
--rw-r--r--   0        0        0    10705 2022-04-09 19:45:13.613226 simplesecurity-2022/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-01-01 17:54:43.116685 simplesecurity-2023/LICENSE.md
+-rw-r--r--   0        0        0     2306 2023-06-27 15:32:54.330605 simplesecurity-2023/pyproject.toml
+-rw-r--r--   0        0        0     9796 2023-06-25 23:48:18.625949 simplesecurity-2023/README.md
+-rw-r--r--   0        0        0     4773 2023-06-27 15:26:17.541858 simplesecurity-2023/simplesecurity/__init__.py
+-rw-r--r--   0        0        0      116 2023-06-27 15:24:47.445979 simplesecurity-2023/simplesecurity/__main__.py
+-rw-r--r--   0        0        0     1041 2023-06-27 15:24:47.440980 simplesecurity-2023/simplesecurity/excluded.py
+-rw-r--r--   0        0        0     2712 2023-06-27 15:24:47.440980 simplesecurity-2023/simplesecurity/filter.py
+-rw-r--r--   0        0        0     8869 2023-06-27 15:24:47.441979 simplesecurity-2023/simplesecurity/formatter.py
+-rw-r--r--   0        0        0      953 2023-06-27 15:24:47.442979 simplesecurity-2023/simplesecurity/level.py
+-rw-r--r--   0        0        0     9748 2023-06-27 15:24:47.443980 simplesecurity-2023/simplesecurity/plugins.py
+-rw-r--r--   0        0        0   160087 2023-01-01 17:54:43.133800 simplesecurity-2023/simplesecurity/semgrep_sec.yaml
+-rw-r--r--   0        0        0      715 2023-06-27 15:24:47.443980 simplesecurity-2023/simplesecurity/types.py
+-rw-r--r--   0        0        0    11158 1970-01-01 00:00:00.000000 simplesecurity-2023/setup.py
+-rw-r--r--   0        0        0    11541 1970-01-01 00:00:00.000000 simplesecurity-2023/PKG-INFO
```

### Comparing `simplesecurity-2022/LICENSE.md` & `simplesecurity-2023/LICENSE.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-The MIT License (MIT)
-
-Copyright (c) 2020 FredHappyface
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2020 FredHappyface
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `simplesecurity-2022/pyproject.toml` & `simplesecurity-2023/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simplesecurity"
-version = "2022"
+version = "2023"
 license = "mit"
 description = "Combine multiple popular python security tools and generate reports or output into different formats"
 authors = ["FredHappyface"]
 classifiers = [
 	"Environment :: Console",
 	"Environment :: MacOS X",
 	"Environment :: Win32 (MS Windows)",
@@ -12,36 +12,48 @@
 	"Intended Audience :: Developers",
 	"Intended Audience :: Education",
 	"Natural Language :: English",
 	"Operating System :: OS Independent",
 	"Programming Language :: Python :: Implementation :: CPython",
 	"Topic :: Security",
 	"Topic :: Software Development :: Libraries :: Python Modules",
-	"Topic :: Utilities"
+	"Topic :: Utilities",
 ]
 homepage = "https://github.com/FHPythonUtils/SimpleSecurity"
 repository = "https://github.com/FHPythonUtils/SimpleSecurity"
 documentation = "https://github.com/FHPythonUtils/SimpleSecurity/blob/master/README.md"
 readme = "README.md"
 
 [tool.poetry.scripts]
 simplesecurity = 'simplesecurity:cli'
 
 [tool.poetry.dependencies]
 python = "^3.7"
-poetry = { version = "<2,>=1.1.10", optional = true }
-bandit = { version = "<2,>=1.7.0", optional = true }
-safety = { version = "<2,>=1.10.3", optional = true }
-dodgy = { version = "<2,>=0.2.1", optional = true }
-dlint = { version = "<2,>=0.11.0", optional = true }
-semgrep = { version = "<2,>=0.67.0", optional = true }
+poetry = {version = "<2,>=1.5.1", optional = true}
+bandit = {version = "<2,>=1.7.5", optional = true}
+safety = {version = "<3,>=2.3.5", optional = true}
+dodgy = {version = "<2,>=0.2.1", optional = true}
+dlint = {version = "<2,>=0.14.1", optional = true}
+semgrep = {version = "<2,>=1.29.0", optional = true}
 
 [tool.poetry.extras]
 full = ["poetry", "bandit", "safety", "dodgy", "dlint", "semgrep"]
 
+[tool.black]
+line-length = 100
+target-version = ["py38"]
+
+[tool.isort]
+profile = "black"
+indent = "Tab"
+
+[tool.pydocstyle]
+convention = "google"
+ignore = "D205,D415"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pylint.basic]
 argument-naming-style = "camelCase"
 attr-naming-style = "camelCase"
@@ -49,28 +61,26 @@
 method-naming-style = "camelCase"
 variable-naming-style = "camelCase"
 
 [tool.pylint.format]
 indent-string = "\t"
 
 [tool.pylint.master]
-ignore-patterns = "test_.*?py"
+ignore-paths = ["tests"]
 
 [tool.pylint.messages_control]
 enable = ["F", "E", "W", "R", "C"]
-disable = [
-	"pointless-string-statement",
-	"superfluous-parens",
-	"bad-continuation"
-]
-
-[tool.black]
-line-length = 100
-target-version = ["py37"]
+disable = ["pointless-string-statement", "superfluous-parens"]
 
-[tool.isort]
-profile = "black"
-indent = "Tab"
-
-[tool.pydocstyle]
-convention = "google"
-ignore = "D205,D415"
+[tool.tox]
+legacy_tox_ini = """
+[tox]
+env_list =
+	py311
+	py310
+	py39
+	py38
+
+[testenv]
+deps = pytest
+commands = pytest tests
+"""
```

### Comparing `simplesecurity-2022/README.md` & `simplesecurity-2023/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,303 +1,335 @@
-[![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../)
-[![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../)
-[![Issues](https://img.shields.io/github/issues/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../issues)
-[![License](https://img.shields.io/github/license/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](/LICENSE.md)
-[![Commit activity](https://img.shields.io/github/commit-activity/m/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../commits/master)
-[![Last commit](https://img.shields.io/github/last-commit/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../commits/master)
-[![PyPI Downloads](https://img.shields.io/pypi/dm/simplesecurity.svg?style=for-the-badge)](https://pypistats.org/packages/simplesecurity)
-[![PyPI Total Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=total%20downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fsimplesecurity)](https://pepy.tech/project/simplesecurity)
-[![PyPI Version](https://img.shields.io/pypi/v/simplesecurity.svg?style=for-the-badge)](https://pypi.org/project/simplesecurity)
-
-<!-- omit in toc -->
-# SimpleSecurity
-
-<img src="readme-assets/icons/name.png" alt="Project Icon" width="750">
-
-Combine multiple popular python security tools and generate reports or output
-into different formats
-
-Plugins (these require the plugin executable in the system path. e.g. bandit
-requires bandit to be in the system path...)
-
-- bandit
-- safety
-- dodgy
-- dlint
-- semgrep
-
-Formats
-
-- ansi (for terminal)
-- json
-- markdown
-- csv
-- sarif
-
-## Example Use
-
-See below for the output if you run `simplesecurity` in this directory
-
-<img src="readme-assets/screenshots/sec.svg" width="500px">
-
-### Help
-
-```txt
-usage: __main__.py [-h] [--format FORMAT] [--plugin PLUGIN] [--file FILE] [--level LEVEL] [--confidence CONFIDENCE]
-                   [--no-colour] [--high-contrast] [--fast] [--zero]
-
-Combine multiple popular python security tools...
-
-and generate reports or output into different formats.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --format FORMAT, -f FORMAT
-                        Output format. One of ansi, json, markdown, csv. default=ansi
-  --plugin PLUGIN, -p PLUGIN
-                        Plugin to use. One of bandit, safety, dodgy, dlint, semgrep, all, default=all
-  --file FILE, -o FILE  Filename to write to (omit for stdout)
-  --level LEVEL, -l LEVEL
-                        Minimum level/ severity to show
-  --confidence CONFIDENCE, -c CONFIDENCE
-                        Minimum confidence to show
-  --no-colour, -z       No ANSI colours
-  --high-contrast, -Z   High contrast colours
-  --fast, --skip        Skip long running jobs. Will omit plugins with long run time (applies to -p all only)
-  --zero, -0            Return non zero exit code if any security vulnerabilities are found
-```
-
-You can also import this into your own project and use any of the functions
-in the DOCS
-
-<!-- omit in toc -->
-## Table of Contents
-
-- [Example Use](#example-use)
-	- [Help](#help)
-- [Developer Notes](#developer-notes)
-	- [Generate semgrep_sec.yaml](#generate-semgrep_secyaml)
-- [Documentation](#documentation)
-- [Install With PIP](#install-with-pip)
-- [Language information](#language-information)
-	- [Built for](#built-for)
-- [Install Python on Windows](#install-python-on-windows)
-	- [Chocolatey](#chocolatey)
-	- [Windows - Python.org](#windows---pythonorg)
-- [Install Python on Linux](#install-python-on-linux)
-	- [Apt](#apt)
-	- [Dnf](#dnf)
-- [Install Python on MacOS](#install-python-on-macos)
-	- [Homebrew](#homebrew)
-	- [MacOS - Python.org](#macos---pythonorg)
-- [How to run](#how-to-run)
-	- [Windows](#windows)
-	- [Linux/ MacOS](#linux-macos)
-- [Download Project](#download-project)
-	- [Clone](#clone)
-		- [Using The Command Line](#using-the-command-line)
-		- [Using GitHub Desktop](#using-github-desktop)
-	- [Download Zip File](#download-zip-file)
-- [Community Files](#community-files)
-	- [Licence](#licence)
-	- [Changelog](#changelog)
-	- [Code of Conduct](#code-of-conduct)
-	- [Contributing](#contributing)
-	- [Security](#security)
-	- [Support](#support)
-	- [Rationale](#rationale)
-
-## Developer Notes
-
-### Generate semgrep_sec.yaml
-
-1. Clone https://github.com/returntocorp/semgrep-rules
-2. cd to `semgrep-rules/python`
-3. do
-
-   ```bash
-   cat **/security/**/*.yaml >> semgrep_sec.yaml
-   cat **/security/*.yaml >> semgrep_sec.yaml
-   ```
-
-4. Find and replace `rules:` with `` apart from the first instance
-5. Reformat with `ctrl+shift+i`
-6. replace simplesecurity/semgrep_sec.yaml with the new one
-
-## Documentation
-
-A high-level overview of how the documentation is organized organized will help you know
-where to look for certain things:
-
-<!--
-- [Tutorials](/documentation/tutorials) take you by the hand through a series of steps to get
-  started using the software. Start here if you’re new.
--->
-- The [Technical Reference](/documentation/reference) documents APIs and other aspects of the
-  machinery. This documentation describes how to use the classes and functions at a lower level
-  and assume that you have a good high-level understanding of the software.
-<!--
-- The [Help](/documentation/help) guide provides a starting point and outlines common issues that you
-  may have.
--->
-
-## Install With PIP
-
-**"Slim" Build:** Install bandit, dlint, dodgy, poetry, and safety with pipx
-
-```python
-pip install simplesecurity
-```
-
-**Otherwise:**
-
-```python
-pip install simplesecurity[full]
-```
-
-Head to https://pypi.org/project/SimpleSecurity/ for more info
-
-## Language information
-
-### Built for
-
-This program has been written for Python versions 3.7 - 3.10 and has been tested with both 3.7 and
-3.10
-
-## Install Python on Windows
-
-### Chocolatey
-
-```powershell
-choco install python
-```
-
-### Windows - Python.org
-
-To install Python, go to https://www.python.org/downloads/windows/ and download the latest
-version.
-
-## Install Python on Linux
-
-### Apt
-
-```bash
-sudo apt install python3.x
-```
-
-### Dnf
-
-```bash
-sudo dnf install python3.x
-```
-
-## Install Python on MacOS
-
-### Homebrew
-
-```bash
-brew install python@3.x
-```
-
-### MacOS - Python.org
-
-To install Python, go to https://www.python.org/downloads/macos/ and download the latest
-version.
-
-## How to run
-
-### Windows
-
-- Module
-	`py -3.x -m [module]` or `[module]` (if module installs a script)
-
-- File
-	`py -3.x [file]` or `./[file]`
-
-### Linux/ MacOS
-
-- Module
-	`python3.x -m [module]` or `[module]` (if module installs a script)
-
-- File
-	`python3.x [file]` or `./[file]`
-
-## Download Project
-
-### Clone
-
-#### Using The Command Line
-
-1. Press the Clone or download button in the top right
-2. Copy the URL (link)
-3. Open the command line and change directory to where you wish to
-clone to
-4. Type 'git clone' followed by URL in step 2
-
-	```bash
-	git clone https://github.com/FHPythonUtils/SimpleSecurity
-	```
-
-More information can be found at
-https://help.github.com/en/articles/cloning-a-repository
-
-#### Using GitHub Desktop
-
-1. Press the Clone or download button in the top right
-2. Click open in desktop
-3. Choose the path for where you want and click Clone
-
-More information can be found at
-https://help.github.com/en/desktop/contributing-to-projects/cloning-a-repository-from-github-to-github-desktop
-
-### Download Zip File
-
-1. Download this GitHub repository
-2. Extract the zip archive
-3. Copy/ move to the desired location
-
-## Community Files
-
-### Licence
-
-MIT License
-Copyright (c) FredHappyface
-(See the [LICENSE](/LICENSE.md) for more information.)
-
-### Changelog
-
-See the [Changelog](/CHANGELOG.md) for more information.
-
-### Code of Conduct
-
-Online communities include people from many backgrounds. The *Project*
-contributors are committed to providing a friendly, safe and welcoming
-environment for all. Please see the
-[Code of Conduct](https://github.com/FHPythonUtils/.github/blob/master/CODE_OF_CONDUCT.md)
- for more information.
-
-### Contributing
-
-Contributions are welcome, please see the
-[Contributing Guidelines](https://github.com/FHPythonUtils/.github/blob/master/CONTRIBUTING.md)
-for more information.
-
-### Security
-
-Thank you for improving the security of the project, please see the
-[Security Policy](https://github.com/FHPythonUtils/.github/blob/master/SECURITY.md)
-for more information.
-
-### Support
-
-Thank you for using this project, I hope it is of use to you. Please be aware that
-those involved with the project often do so for fun along with other commitments
-(such as work, family, etc). Please see the
-[Support Policy](https://github.com/FHPythonUtils/.github/blob/master/SUPPORT.md)
-for more information.
-
-### Rationale
-
-The rationale acts as a guide to various processes regarding projects such as
-the versioning scheme and the programming styles used. Please see the
-[Rationale](https://github.com/FHPythonUtils/.github/blob/master/RATIONALE.md)
-for more information.
+[![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../)
+[![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../)
+[![Issues](https://img.shields.io/github/issues/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../issues)
+[![License](https://img.shields.io/github/license/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](/LICENSE.md)
+[![Commit activity](https://img.shields.io/github/commit-activity/m/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../commits/master)
+[![Last commit](https://img.shields.io/github/last-commit/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../commits/master)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/simplesecurity.svg?style=for-the-badge)](https://pypistats.org/packages/simplesecurity)
+[![PyPI Total Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=total%20downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fsimplesecurity)](https://pepy.tech/project/simplesecurity)
+[![PyPI Version](https://img.shields.io/pypi/v/simplesecurity.svg?style=for-the-badge)](https://pypi.org/project/simplesecurity)
+
+<!-- omit in toc -->
+# SimpleSecurity
+
+<img src="readme-assets/icons/name.png" alt="Project Icon" width="750">
+
+Combine multiple popular python security tools and generate reports or output
+into different formats
+
+Plugins (these require the plugin executable in the system path. e.g. bandit
+requires bandit to be in the system path...)
+
+- bandit
+- safety
+- dodgy
+- dlint
+- semgrep
+
+Formats
+
+- ansi (for terminal)
+- json
+- markdown
+- csv
+- sarif
+
+## Example Use
+
+See below for the output if you run `simplesecurity` in this directory
+
+<img src="readme-assets/screenshots/sec.svg" width="500px">
+
+### Help
+
+```txt
+usage: __main__.py [-h] [--format FORMAT] [--plugin PLUGIN] [--file FILE] [--level LEVEL] [--confidence CONFIDENCE]
+                   [--no-colour] [--high-contrast] [--fast] [--zero]
+
+Combine multiple popular python security tools...
+
+and generate reports or output into different formats.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --format FORMAT, -f FORMAT
+                        Output format. One of ansi, json, markdown, csv. default=ansi
+  --plugin PLUGIN, -p PLUGIN
+                        Plugin to use. One of bandit, safety, dodgy, dlint, semgrep, all, default=all
+  --file FILE, -o FILE  Filename to write to (omit for stdout)
+  --level LEVEL, -l LEVEL
+                        Minimum level/ severity to show
+  --confidence CONFIDENCE, -c CONFIDENCE
+                        Minimum confidence to show
+  --no-colour, -z       No ANSI colours
+  --high-contrast, -Z   High contrast colours
+  --fast, --skip        Skip long running jobs. Will omit plugins with long run time (applies to -p all only)
+  --zero, -0            Return non zero exit code if any security vulnerabilities are found
+```
+
+You can also import this into your own project and use any of the functions
+in the DOCS
+
+<!-- omit in toc -->
+## Table of Contents
+
+- [Example Use](#example-use)
+	- [Help](#help)
+- [Developer Notes](#developer-notes)
+	- [Generate semgrep\_sec.yaml](#generate-semgrep_secyaml)
+- [Documentation](#documentation)
+- [Install With PIP](#install-with-pip)
+- [Language information](#language-information)
+	- [Built for](#built-for)
+- [Install Python on Windows](#install-python-on-windows)
+	- [Chocolatey](#chocolatey)
+	- [Windows - Python.org](#windows---pythonorg)
+- [Install Python on Linux](#install-python-on-linux)
+	- [Apt](#apt)
+	- [Dnf](#dnf)
+- [Install Python on MacOS](#install-python-on-macos)
+	- [Homebrew](#homebrew)
+	- [MacOS - Python.org](#macos---pythonorg)
+- [How to run](#how-to-run)
+	- [Windows](#windows)
+	- [Linux/ MacOS](#linux-macos)
+- [Building](#building)
+- [Testing](#testing)
+- [Download Project](#download-project)
+	- [Clone](#clone)
+		- [Using The Command Line](#using-the-command-line)
+		- [Using GitHub Desktop](#using-github-desktop)
+	- [Download Zip File](#download-zip-file)
+- [Community Files](#community-files)
+	- [Licence](#licence)
+	- [Changelog](#changelog)
+	- [Code of Conduct](#code-of-conduct)
+	- [Contributing](#contributing)
+	- [Security](#security)
+	- [Support](#support)
+	- [Rationale](#rationale)
+
+## Developer Notes
+
+### Generate semgrep_sec.yaml
+
+1. Clone https://github.com/returntocorp/semgrep-rules
+2. cd to `semgrep-rules/python`
+3. do
+
+   ```bash
+   cat **/security/**/*.yaml >> semgrep_sec.yaml
+   cat **/security/*.yaml >> semgrep_sec.yaml
+   ```
+
+4. Find and replace `rules:` with `` apart from the first instance
+5. Reformat with `ctrl+shift+i`
+6. replace simplesecurity/semgrep_sec.yaml with the new one
+
+## Documentation
+
+A high-level overview of how the documentation is organized organized will help you know
+where to look for certain things:
+
+<!--
+- [Tutorials](/documentation/tutorials) take you by the hand through a series of steps to get
+  started using the software. Start here if you’re new.
+-->
+- The [Technical Reference](/documentation/reference) documents APIs and other aspects of the
+  machinery. This documentation describes how to use the classes and functions at a lower level
+  and assume that you have a good high-level understanding of the software.
+<!--
+- The [Help](/documentation/help) guide provides a starting point and outlines common issues that you
+  may have.
+-->
+
+## Install With PIP
+
+**"Slim" Build:** Install bandit, dlint, dodgy, poetry, and safety with pipx
+
+```python
+pip install simplesecurity
+```
+
+**Otherwise:**
+
+```python
+pip install simplesecurity[full]
+```
+
+Head to https://pypi.org/project/SimpleSecurity/ for more info
+
+## Language information
+
+### Built for
+
+This program has been written for Python versions 3.8 - 3.11 and has been tested with both 3.8 and
+3.11
+
+## Install Python on Windows
+
+### Chocolatey
+
+```powershell
+choco install python
+```
+
+### Windows - Python.org
+
+To install Python, go to https://www.python.org/downloads/windows/ and download the latest
+version.
+
+## Install Python on Linux
+
+### Apt
+
+```bash
+sudo apt install python3.x
+```
+
+### Dnf
+
+```bash
+sudo dnf install python3.x
+```
+
+## Install Python on MacOS
+
+### Homebrew
+
+```bash
+brew install python@3.x
+```
+
+### MacOS - Python.org
+
+To install Python, go to https://www.python.org/downloads/macos/ and download the latest
+version.
+
+## How to run
+
+### Windows
+
+- Module
+	`py -3.x -m [module]` or `[module]` (if module installs a script)
+
+- File
+	`py -3.x [file]` or `./[file]`
+
+### Linux/ MacOS
+
+- Module
+	`python3.x -m [module]` or `[module]` (if module installs a script)
+
+- File
+	`python3.x [file]` or `./[file]`
+
+## Building
+
+This project uses https://github.com/FHPythonUtils/FHMake to automate most of the building. This
+command generates the documentation, updates the requirements.txt and builds the library artefacts
+
+Note the functionality provided by fhmake can be approximated by the following
+
+```sh
+handsdown  --cleanup -o documentation/reference
+poetry export -f requirements.txt --output requirements.txt
+poetry export -f requirements.txt --with dev --output requirements_optional.txt
+poetry build
+```
+
+`fhmake audit` can be run to perform additional checks
+
+## Testing
+
+For testing with the version of python used by poetry use
+
+```sh
+poetry run pytest
+```
+
+Alternatively use `tox` to run tests over python 3.8 - 3.11
+
+```sh
+tox
+```
+
+## Download Project
+
+### Clone
+
+#### Using The Command Line
+
+1. Press the Clone or download button in the top right
+2. Copy the URL (link)
+3. Open the command line and change directory to where you wish to
+clone to
+4. Type 'git clone' followed by URL in step 2
+
+	```bash
+	git clone https://github.com/FHPythonUtils/SimpleSecurity
+	```
+
+More information can be found at
+https://help.github.com/en/articles/cloning-a-repository
+
+#### Using GitHub Desktop
+
+1. Press the Clone or download button in the top right
+2. Click open in desktop
+3. Choose the path for where you want and click Clone
+
+More information can be found at
+https://help.github.com/en/desktop/contributing-to-projects/cloning-a-repository-from-github-to-github-desktop
+
+### Download Zip File
+
+1. Download this GitHub repository
+2. Extract the zip archive
+3. Copy/ move to the desired location
+
+## Community Files
+
+### Licence
+
+MIT License
+Copyright (c) FredHappyface
+(See the [LICENSE](/LICENSE.md) for more information.)
+
+### Changelog
+
+See the [Changelog](/CHANGELOG.md) for more information.
+
+### Code of Conduct
+
+Online communities include people from many backgrounds. The *Project*
+contributors are committed to providing a friendly, safe and welcoming
+environment for all. Please see the
+[Code of Conduct](https://github.com/FHPythonUtils/.github/blob/master/CODE_OF_CONDUCT.md)
+ for more information.
+
+### Contributing
+
+Contributions are welcome, please see the
+[Contributing Guidelines](https://github.com/FHPythonUtils/.github/blob/master/CONTRIBUTING.md)
+for more information.
+
+### Security
+
+Thank you for improving the security of the project, please see the
+[Security Policy](https://github.com/FHPythonUtils/.github/blob/master/SECURITY.md)
+for more information.
+
+### Support
+
+Thank you for using this project, I hope it is of use to you. Please be aware that
+those involved with the project often do so for fun along with other commitments
+(such as work, family, etc). Please see the
+[Support Policy](https://github.com/FHPythonUtils/.github/blob/master/SUPPORT.md)
+for more information.
+
+### Rationale
+
+The rationale acts as a guide to various processes regarding projects such as
+the versioning scheme and the programming styles used. Please see the
+[Rationale](https://github.com/FHPythonUtils/.github/blob/master/RATIONALE.md)
+for more information.
```

### Comparing `simplesecurity-2022/simplesecurity/__init__.py` & `simplesecurity-2023/simplesecurity/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,79 +20,144 @@
 - sarif
 """
 from __future__ import annotations
 
 import argparse
 from sys import exit as sysexit
 from sys import stdout
-from typing import Any
+from typing import Any, Callable, TextIO
 
 from simplesecurity import filter as secfilter
 from simplesecurity import formatter, plugins
-from simplesecurity.types import Finding
 
 stdout.reconfigure(encoding="utf-8")  # type:ignore
 FORMAT_HELP = "Output format. One of ansi, json, markdown, csv. default=ansi"
 PLUGIN_HELP = "Plugin to use. One of bandit, safety, dodgy, dlint, semgrep, all, default=all"
 
 
-def runAllPlugins(
-	pluginMap: dict[str, Any], severity: int, confidence: int, fast: bool
-) -> list[Finding]:
-	"""Run each plugin. Optimise as much as we can.
-
-	Args:
-		pluginMap (dict[str, Any]): the plugin map
-		severity (int): the minimum severity to report on
-		confidence (int): the minimum confidence to report on
-		fast (bool): runAllPlugins with optimisations
-
-	Returns:
-		list[Finding]: list of findings
-	"""
-	findings: list[Finding] = []
-	for plugin in pluginMap:
-		# Do optimisations
+def _processFile(file: str | None) -> TextIO:
+	return (
+		stdout
+		if file is None
+		else open(file, "w", encoding="utf-8")  # pylint: disable=consider-using-with
+	)
+
+
+def _processColour(noColour: bool, highContrast: bool) -> int:
+	colourMode = 1
+	if noColour:
+		colourMode = 0
+	if highContrast:
+		colourMode = 2
+	return colourMode
+
+
+def _processFormat(formatin: str | None) -> Callable:
+	formatMap = {
+		"json": formatter.json,
+		"markdown": formatter.markdown,
+		"csv": formatter.csv,
+		"ansi": formatter.ansi,
+		"sarif": formatter.sarif,
+	}
+	if formatin is None:
+		formatt = formatter.ansi
+	elif formatin in formatMap:
+		formatt = formatMap[formatin]
+	else:
+		print(FORMAT_HELP)
+		sysexit(1)
+	return formatt
+
+
+def _processPlugin(args) -> list[Callable]:
+	pluginMap: dict[str, Any] = {
+		"bandit": {
+			"func": plugins.bandit,
+			"max_severity": 3,
+			"max_confidence": 3,
+			"fast": True,
+		},
+		"safety": {
+			"func": plugins.safety,
+			"max_severity": 2,
+			"max_confidence": 3,
+			"fast": True,
+		},
+		"dodgy": {
+			"func": plugins.dodgy,
+			"max_severity": 2,
+			"max_confidence": 2,
+			"fast": True,
+		},
+		"dlint": {
+			"func": plugins.dlint,
+			"max_severity": 3,
+			"max_confidence": 2,
+			"fast": True,
+		},
+		"semgrep": {
+			"func": plugins.semgrep,
+			"max_severity": 3,
+			"max_confidence": 3,
+			"fast": False,
+		},
+	}
+
+	plugin = args.plugin
+
+	filtered = {
+		k: v["func"]
+		for k, v in pluginMap.items()
 		if (
-			pluginMap[plugin]["max_severity"] >= severity
-			and pluginMap[plugin]["max_confidence"] >= confidence
-			and (not fast or pluginMap[plugin]["fast"])
-		):
-			try:
-				findings.extend(pluginMap[plugin]["func"]())
-			except RuntimeError as error:
-				print(error)
-	return findings
+			v["max_severity"] >= args.level
+			and v["max_confidence"] >= args.confidence
+			and (not args.fast or v["fast"])
+		)
+	}
+
+	if plugin in (None, "all"):
+		return [v for _, v in filtered.items()]
+	if plugin in filtered:
+		return [filtered[plugin]]
+
+	print(PLUGIN_HELP)
+	sysexit(2)
 
 
 def cli():
 	"""Cli entry point."""
 	parser = argparse.ArgumentParser(
 		description=__doc__, formatter_class=argparse.RawTextHelpFormatter
 	)
 	parser.add_argument(
+		"--scan-dir",
+		"-s",
+		help="Pass a path to the scan directory (optional)",
+	)
+	parser.add_argument(
 		"--format",
 		"-f",
 		help=FORMAT_HELP,
 	)
 	parser.add_argument(
 		"--plugin",
 		"-p",
 		help=PLUGIN_HELP,
 	)
 	parser.add_argument(
 		"--file",
 		"-o",
 		help="Filename to write to (omit for stdout)",
 	)
-	# Let's use a low severity and medium confidence by default
+	# Let's use a low level and medium confidence by default
 	parser.add_argument(
 		"--level",
 		"-l",
-		help="Minimum level/ severity to show",
+		help="Minimum severity/ level to show",
 		type=int,
 		default=1,
 	)
 	parser.add_argument(
 		"--confidence",
 		"-c",
 		help="Minimum confidence to show",
@@ -120,93 +185,39 @@
 	parser.add_argument(
 		"--zero",
 		"-0",
 		action="store_true",
 		help="Return non zero exit code if any security vulnerabilities are found",
 	)
 	args = parser.parse_args()
-	# File
-	filename = (
-		stdout
-		if args.file is None
-		else open(args.file, "w", encoding="utf-8")  # pylint: disable=consider-using-with
-	)
-	# Colour Mode
-	colourMode = 1
-	if args.no_colour:
-		colourMode = 0
-	if args.high_contrast:
-		colourMode = 2
-	# Format
-	formatMap = {
-		"json": formatter.json,
-		"markdown": formatter.markdown,
-		"csv": formatter.csv,
-		"ansi": formatter.ansi,
-		"sarif": formatter.sarif,
-	}
-	if args.format is None:
-		formatt = formatter.ansi
-	elif args.format in formatMap:
-		formatt = formatMap[args.format]
-	else:
-		print(FORMAT_HELP)
-		sysexit(1)
 
-	# Plugin
-	pluginMap: dict[str, Any] = {
-		"bandit": {
-			"func": plugins.bandit,
-			"max_severity": 3,
-			"max_confidence": 3,
-			"fast": True,
-		},
-		"safety": {
-			"func": plugins.safety,
-			"max_severity": 2,
-			"max_confidence": 3,
-			"fast": True,
-		},
-		"dodgy": {
-			"func": plugins.dodgy,
-			"max_severity": 2,
-			"max_confidence": 2,
-			"fast": True,
-		},
-		"dlint": {
-			"func": plugins.dlint,
-			"max_severity": 2,
-			"max_confidence": 2,
-			"fast": True,
-		},
-		"semgrep": {
-			"func": plugins.semgrep,
-			"max_severity": 3,
-			"max_confidence": 3,
-			"fast": False,
-		},
-	}
+	scanDir = args.scan_dir or "."
+	filename = _processFile(args.file)
+	colourMode = _processColour(args.no_colour, args.high_contrast)
+	formatt = _processFormat(args.format)
+
+	filteredPlugins = _processPlugin(args)
+
+	findings = []
+	for plugin in filteredPlugins:
+		finding = []
+		try:
+			finding = plugin(scanDir=scanDir)
+		except BaseException as e:
+			print(f"! SimpleSecurity encountered an error: {e}")
+		findings.extend(finding)
+
+	filteredFindings = secfilter.filterSeverityAndConfidence(
+		secfilter.deduplicate(findings), args.level, args.confidence
+	)
+
+	print(
+		formatt(
+			filteredFindings,
+			colourMode=colourMode,
+		),
+		file=filename,
+	)
 
-	if args.plugin is None or args.plugin == "all" or args.plugin in pluginMap:
-		findings = []
-		if args.plugin is None or args.plugin == "all":
-			findings = runAllPlugins(pluginMap, args.level, args.confidence, args.fast)
-		elif (
-			pluginMap[args.plugin]["max_severity"] >= args.level
-			and pluginMap[args.plugin]["max_confidence"] >= args.confidence
-		):
-			findings = pluginMap[args.plugin]["func"]()
-		print(
-			formatt(
-				secfilter.filterSeverityAndConfidence(
-					secfilter.deduplicate(findings), args.level, args.confidence
-				),
-				colourMode=colourMode,
-			),
-			file=filename,
-		)
-	else:
-		print(PLUGIN_HELP)
-		sysexit(2)
-	if len(findings) > 0 and args.zero:
+	if len(filteredFindings) > 0 and args.zero:
 		sysexit(1)
 	sysexit(0)
```

### Comparing `simplesecurity-2022/simplesecurity/filter.py` & `simplesecurity-2023/simplesecurity/filter.py`

 * *Files identical despite different names*

### Comparing `simplesecurity-2022/simplesecurity/formatter.py` & `simplesecurity-2023/simplesecurity/formatter.py`

 * *Files identical despite different names*

### Comparing `simplesecurity-2022/simplesecurity/level.py` & `simplesecurity-2023/simplesecurity/level.py`

 * *Files identical despite different names*

### Comparing `simplesecurity-2022/simplesecurity/plugins.py` & `simplesecurity-2023/simplesecurity/plugins.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,30 +26,20 @@
 import platform
 import subprocess
 from json import loads
 from os import remove
 from pathlib import Path
 from typing import Any
 
+from simplesecurity.excluded import EXCLUDED
 from simplesecurity.level import Level
 from simplesecurity.types import Finding, Line
 
 THISDIR = str(Path(__file__).resolve().parent)
 
-EXCLUDED = [
-	"./.env",
-	"./tests",
-	"./.venv",
-	"./env/",
-	"./venv/",
-	"./ENV/",
-	"./env.bak/",
-	"./venv.bak/",
-]
-
 
 def _doSysExec(command: str, errorAsOut: bool = True) -> tuple[int, str]:
 	"""Execute a command and check for errors.
 
 	Args:
 			command (str): commands as a string
 			errorAsOut (bool, optional): redirect errors to stdout
@@ -93,17 +83,20 @@
 				lineContent = next(fileContents).rstrip().replace("\t", "    ")
 			except StopIteration:
 				break
 			content.append({"selected": line == desiredLine, "line": line, "content": lineContent})
 	return content
 
 
-def bandit() -> list[Finding]:
+def bandit(scanDir=".") -> list[Finding]:
 	"""Generate list of findings using bandit. requires bandit on the system path.
 
+	Params:
+		scanDir(str): select a scan directory (useful for cicd etc)
+
 	Raises:
 		RuntimeError: if bandit is not on the system path, then throw this
 		error
 
 	Returns:
 		list[Finding]: our findings dictionary
 	"""
@@ -112,17 +105,19 @@
 	findings = []
 	levelMap = {
 		"LOW": Level.LOW,
 		"MEDIUM": Level.MED,
 		"HIGH": Level.HIGH,
 		"UNDEFINED": Level.UNKNOWN,
 	}
-	results = loads(_doSysExec(f"bandit -lirq -x {','.join(EXCLUDED)} -f json .", False)[1])[
-		"results"
-	]
+	results = loads(
+		_doSysExec(
+			f"bandit -lirq -x {','.join([f'./{x}' for x in EXCLUDED])} -f json {scanDir}", False
+		)[1]
+	)["results"]
 	for result in results:
 		file = result["filename"].replace("\\", "/")
 		findings.append(
 			{
 				"id": result["test_id"],
 				"title": f"{result['test_id']}: {result['test_name']}",
 				"description": result["issue_text"],
@@ -138,15 +133,15 @@
 			}
 		)
 	return findings
 
 
 def _doSafetyProcessing(results: dict[str, Any]) -> list[Finding]:
 	findings = []
-	for result in results:
+	for result in results["vulnerabilities"]:
 		findings.append(
 			{
 				"id": result[4],
 				"title": f"{result[4]}: {result[0]}",
 				"description": result[3],
 				"file": "Project Requirements",
 				"evidence": [
@@ -161,33 +156,37 @@
 				"line": "Unknown",
 				"_other": {"id": result[4], "affected": result[1]},
 			}
 		)
 	return findings
 
 
-def _doPureSafety():
+def _doPureSafety() -> dict[str, Any]:
 	safe = _doSysExec("safety check -r requirements.txt --json")[1]
 	if safe.startswith("Warning:"):
 		safe = _doSysExec("safety check --json")[1]
 		if safe.startswith("Warning:"):
 			raise RuntimeError("some error occurred: " + safe)
 	return loads(safe)
 
 
-def safety() -> list[Finding]:
-	"""Generate list of findings using safety.
+def safety(scanDir=".") -> list[Finding]:
+	"""Generate list of findings using _tool_. requires _tool_ on the system path.
+
+	Params:
+		scanDir(str): select a scan directory (useful for cicd etc)
 
 	Raises:
 		RuntimeError: if safety is not on the system path, then throw this
 		error
 
 	Returns:
 		list[Finding]: our findings dictionary
 	"""
+	_ = scanDir
 	if _doSysExec("safety --help")[0] != 0:
 		raise RuntimeError("safety is not on the system path")
 	pShow = _doSysExec("poetry show")
 	if not pShow[0]:
 		lines = pShow[1].splitlines(False)
 		data = []
 		for line in lines:
@@ -205,28 +204,32 @@
 		remove("reqs.txt")
 	else:
 		# Use plain old safety (this will miss optional dependencies)
 		results = _doPureSafety()
 	return _doSafetyProcessing(results)
 
 
-def dodgy() -> list[Finding]:
-	"""Generate list of findings using dodgy. Requires dodgy on the system path.
+def dodgy(scanDir=".") -> list[Finding]:
+	"""Generate list of findings using _tool_. requires _tool_ on the system path.
+
+	Params:
+		scanDir(str): select a scan directory (useful for cicd etc)
 
 	Raises:
 		RuntimeError: if dodgy is not on the system path, then throw this
 		error
 
 	Returns:
 		list[Finding]: our findings dictionary
 	"""
 	if _doSysExec("dodgy -h")[0] != 0:
 		raise RuntimeError("dodgy is not on the system path")
 	findings = []
-	results = loads(_doSysExec(f"dodgy -i {' '.join(EXCLUDED)}")[1])["warnings"]
+	rawResults = _doSysExec(f"dodgy {scanDir} -i {' '.join(EXCLUDED)}")[1]
+	results = loads(rawResults)["warnings"]
 	for result in results:
 		file = "./" + result["path"].replace("\\", "/")
 		findings.append(
 			{
 				"id": result["code"],
 				"title": result["message"],
 				"description": result["message"],
@@ -237,53 +240,70 @@
 				"line": result["line"],
 				"_other": {},
 			}
 		)
 	return findings
 
 
-def dlint() -> list[Finding]:
-	"""Generate list of findings using dlint. Requires flake8 and dlint on the system path.
+def dlint(scanDir=".") -> list[Finding]:
+	"""Generate list of findings using _tool_. requires _tool_ on the system path.
+
+	Params:
+		scanDir(str): select a scan directory (useful for cicd etc)
 
 	Raises:
 		RuntimeError: if flake8 is not on the system path, then throw this
 		error
 
 	Returns:
 		list[Finding]: our findings dictionary
 	"""
 	if _doSysExec("flake8 -h")[0] != 0:
 		raise RuntimeError("flake8 is not on the system path")
 	findings = []
 	results = _doSysExec(
-		f"flake8 --select=DUO --exclude {','.join(EXCLUDED)} --format='%(path)s"
-		"::%(row)d::%(col)d::%(code)s::%(text)s' ."
+		f"flake8 --select=DUO --exclude {','.join(EXCLUDED)} --format=codeclimate {scanDir}"
 	)[1].splitlines(False)
-	for line in results:
-		if line[0] == "'":
-			line = line[1:-1]
-		result = line.split("::")
-		file = result[0].replace("\\", "/")
-		findings.append(
-			{
-				"id": result[3],
-				"title": f"{result[3]}: {result[4]}",
-				"description": result[4],
-				"file": file,
-				"evidence": extractEvidence(int(result[1]), file),
-				"severity": Level.MED,
-				"confidence": Level.MED,
-				"line": int(result[1]),
-				"_other": {"col": result[2]},
-			}
-		)
+
+	jsonResults = loads("".join(results)) if len(results) > 0 else {}
+	levelMap = {
+		"info": Level.LOW,
+		"minor": Level.MED,
+		"major": Level.MED,
+		"critical": Level.HIGH,
+		"blocker": Level.HIGH,
+	}
+	for filePath, scanResults in jsonResults.items():
+		for scanResult in scanResults:
+			findings.append(
+				{
+					"id": scanResult["check_name"],
+					"title": f"{scanResult['check_name']}: " f"{scanResult['description']}",
+					"description": f"{scanResult['check_name']}: " f"{scanResult['description']}",
+					"file": filePath,
+					"evidence": extractEvidence(
+						scanResult["location"]["positions"]["begin"]["line"],
+						filePath,
+					),
+					"severity": levelMap[scanResult["severity"]],
+					"confidence": Level.MED,
+					"line": scanResult["location"]["positions"]["begin"]["line"],
+					"_other": {
+						"col": scanResult["location"]["positions"]["begin"]["column"],
+						"start": scanResult["location"]["positions"]["begin"]["line"],
+						"end": scanResult["location"]["positions"]["end"]["line"],
+						"fingerprint": scanResult["fingerprint"],
+					},
+				}
+			)
+
 	return findings
 
 
-def semgrep() -> list[Finding]:
+def semgrep(scanDir=".") -> list[Finding]:
 	"""Generate list of findings using for semgrep. Requires semgrep on the
 	system path (wsl in windows).
 
 	Raises:
 		RuntimeError: if semgrep is not on the system path, then throw this
 		error
 
@@ -294,21 +314,22 @@
 	if platform.system() == "Windows":
 		raise RuntimeError("semgrep is not supported on windows")
 	if _doSysExec("semgrep --help")[0] != 0:
 		raise RuntimeError("semgrep is not on the system path")
 	sgExclude = ["--exclude {x}" for x in EXCLUDED]
 	results = loads(
 		_doSysExec(
-			f"semgrep -f {THISDIR}/semgrep_sec.yaml {' '.join(sgExclude)} "
+			f"semgrep -f {THISDIR}/semgrep_sec.yaml {scanDir} {' '.join(sgExclude)} "
 			"-q --json --no-rewrite-rule-ids"
 		)[1].strip()
 	)["results"]
 	levelMap = {"INFO": Level.LOW, "WARNING": Level.MED, "ERROR": Level.HIGH}
 	for result in results:
-		file = "./" + result["path"].replace("\\", "/")
+		filePath = result["Target"].replace("\\", "/")
+		file = f"{scanDir}/{filePath}"
 		findings.append(
 			{
 				"id": result["check_id"],
 				"title": result["check_id"].split(".")[-1],
 				"description": result["extra"]["message"].strip(),
 				"file": file,
 				"evidence": extractEvidence(result["start"]["line"], file),
```

### Comparing `simplesecurity-2022/simplesecurity/semgrep_sec.yaml` & `simplesecurity-2023/simplesecurity/semgrep_sec.yaml`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,3833 +1,3833 @@
-rules:
-  - id: formatted-string-bashoperator
-    patterns:
-      - pattern-either:
-          - pattern: |
-              airflow.operators.bash_operator.BashOperator(..., bash_command="..." + $CONCAT, ...)
-          - pattern: |
-              airflow.operators.bash_operator.BashOperator(..., bash_command="...".format(...), ...)
-          - pattern: |
-              airflow.operators.bash_operator.BashOperator(..., bash_command=f"...", ...)
-          - pattern: |
-              airflow.operators.bash_operator.BashOperator(..., bash_command="..." % $PARAMS, ...)
-          - pattern: |
-              $CMD = "..." % $PARAMS
-              ...
-              airflow.operators.bash_operator.BashOperator(..., bash_command=$CMD, ...)
-          - pattern: |
-              $CMD = $STR.format(...)
-              ...
-              airflow.operators.bash_operator.BashOperator(..., bash_command=$CMD, ...)
-          - pattern: |
-              $CMD = f"..."
-              ...
-              airflow.operators.bash_operator.BashOperator(..., bash_command=$CMD, ...)
-          - pattern: |
-              $CMD = "..." + $CONCAT
-              ...
-              airflow.operators.bash_operator.BashOperator(..., bash_command=$CMD, ...)
-          - pattern: |
-              $CMD = "..."
-              ...
-              $CMD += $CONCAT
-              ...
-              airflow.operators.bash_operator.BashOperator(..., bash_command=$CMD, ...)
-    message: |
-      Found a formatted string in BashOperator: $CMD.
-      This could be vulnerable to injection.
-      Be extra sure your variables are not controllable by external sources.
-    metadata:
-      cwe: "CWE-78: Improper Neutralization of Special Elements used in an OS Command ('OS Command Injection')"
-      owasp: "A1: Injection"
-    languages:
-      - python
-    severity: WARNING
-
-  - id: avoid-insecure-deserialization
-    metadata:
-      owasp: "A8: Insecure Deserialization"
-      cwe: "CWE-502: Deserialization of Untrusted Data"
-      references: https://docs.python.org/3/library/pickle.html
-    message:
-      Avoid using insecure deserialization library, backed by `pickle`, `_pickle`, `cpickle`, `dill`, `shelve`, or `yaml`,
-      which are known to lead to remote code execution vulnerabilities.
-    languages:
-      - python
-    severity: ERROR
-    patterns:
-      - pattern-inside: |
-          def $X(..., request, ...):
-            ...
-      - pattern-either:
-          - pattern: |
-              $VAR = <... request.$Y.get(...) ...>
-              ...
-              pickle.$FUNC(<... $VAR ...>)
-          - pattern: pickle.$FUNC(<... request.$Y.get(...) ...>)
-          - pattern: |
-              $VAR = <... request.$Y.get(...) ...>
-              ...
-              _pickle.$FUNC(<... $VAR ...>)
-          - pattern: _pickle.$FUNC(<... request.$Y.get(...) ...>)
-          - pattern: |
-              $VAR = <... request.$Y.get(...) ...>
-              ...
-              cPickle.$FUNC(<... $VAR ...>)
-          - pattern: cPickle.$FUNC(<... request.$Y.get(...) ...>)
-          - pattern: |
-              $VAR = <... request.$Y.get(...) ...>
-              ...
-              dill.$FUNC(<... $VAR ...>)
-          - pattern: dill.$FUNC(<... request.$Y.get(...) ...>)
-          - pattern: |
-              $VAR = <... request.$Y.get(...) ...>
-              ...
-              shelve.$FUNC(<... $VAR ...>)
-          - pattern: shelve.$FUNC(<... request.$Y.get(...) ...>)
-          - pattern: |
-              $VAR = <... request.$Y.get(...) ...>
-              ...
-              yaml.$FUNC(<... $VAR ...>)
-          - pattern: yaml.$FUNC(<... request.$Y.get(...) ...>)
-
-  - id: avoid-mark-safe
-    patterns:
-      - pattern-not-inside: django.utils.html.format_html(...)
-      - pattern-not: django.utils.safestring.mark_safe("...")
-      - pattern: django.utils.safestring.mark_safe(...)
-    message: |
-      'mark_safe()' is used to mark a string as "safe" for HTML output.
-      This disables escaping and could therefore subject the content to
-      XSS attacks. Use 'django.utils.html.format_html()' to build HTML
-      for rendering instead.
-    metadata:
-      cwe: "CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')"
-      owasp: "A7: Cross-Site Scripting (XSS)"
-      references:
-        - https://docs.djangoproject.com/en/3.0/ref/utils/#django.utils.safestring.mark_safe
-        - https://docs.djangoproject.com/en/3.0/ref/utils/#django.utils.html.format_html
-    languages: [python]
-    severity: WARNING
-
-  - id: no-csrf-exempt
-    pattern: |
-      @django.views.decorators.csrf.csrf_exempt
-      def $R(...):
-        ...
-    message: There is rarely a good reason to use @csrf_exempt as is used for `$R`.
-    metadata:
-      cwe: "CWE-352: Cross-Site Request Forgery (CSRF)"
-      owasp: "A6: Security Misconfiguration"
-    languages: [python]
-    severity: WARNING
-
-  - id: custom-expression-as-sql
-    languages:
-      - python
-    message:
-      Detected a Custom Expression ''$EXPRESSION'' calling ''as_sql(...).'' Ensure no user input enters this function
-      because it is susceptible to SQL injection. See https://docs.djangoproject.com/en/3.0/ref/models/expressions/#django.db.models.Func.as_sql
-      for more information.
-    metadata:
-      cwe: "CWE-89: Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection')"
-      owasp: "A1: Injection"
-      references:
-        - https://docs.djangoproject.com/en/3.0/ref/models/expressions/#django.db.models.Func.as_sql
-        - https://blog.r2c.dev/2020/preventing-sql-injection-a-django-authors-perspective/
-    pattern: $EXPRESSION.as_sql(...)
-    severity: WARNING
-
-  - id: extends-custom-expression
-    languages:
-      - python
-    message: |
-      Found extension of custom expression: $CLASS. Extending expressions
-      in this way could inadvertently expose a SQL injection vulnerability.
-      See https://docs.djangoproject.com/en/3.0/ref/models/expressions/#avoiding-sql-injection
-      for more information.
-    metadata:
-      cwe: "CWE-89: Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection')"
-      owasp: "A1: Injection"
-      references:
-        - https://docs.djangoproject.com/en/3.0/ref/models/expressions/#avoiding-sql-injection
-        - https://blog.r2c.dev/2020/preventing-sql-injection-a-django-authors-perspective/
-    patterns:
-      - pattern-either:
-          - pattern: |
-              class $CLASS(..., django.db.models.Func, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.expressions.Func, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.Expression, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.expressions.Expression, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.Value, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.expressions.Value, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.DurationValue, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.expressions.DurationValue, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.RawSQL, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.expressions.RawSQL, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.Star, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.expressions.Star, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.Random, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.expressions.Random, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.Col, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.expressions.Col, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.Ref, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.expressions.Ref, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.ExpressionList, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.expressions.ExpressionList, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.ExpressionWrapper, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.expressions.ExpressionWrapper, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.When, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.expressions.When, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.Case, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.expressions.Case, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.Subquery, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.expressions.Subquery, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.Exists, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.expressions.Exists, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.Window, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.expressions.Window, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.WindowFrame, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.expressions.WindowFrame, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.RowRange, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.expressions.RowRange, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.ValueRange, ...):
-                  ...
-          - pattern: |
-              class $CLASS(..., django.db.models.expressions.ValueRange, ...):
-                  ...
-    severity: WARNING
-
-  - id: avoid-query-set-extra
-    patterns:
-      - pattern-either:
-          - pattern: $X.objects.$FUNC(...).extra(...)
-          - pattern: $X.objects.$FUNC(...).$FILTER(...).extra(...)
-          - pattern: $X.objects.$FUNC(...).$FILTER(...).$UPDATE(...).extra(...)
-    message: This is a last resort. You should be careful when using QuerySet.extra due to SQLi https://docs.djangoproject.com/en/3.0/ref/models/querysets/#django.db.models.query.QuerySet.extra
-    metadata:
-      cwe: "CWE-89: Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection')"
-      owasp: "A1: Injection"
-      references:
-        - https://docs.djangoproject.com/en/3.0/ref/models/querysets/#django.db.models.query.QuerySet.extra
-        - https://blog.r2c.dev/2020/preventing-sql-injection-a-django-authors-perspective/
-    languages: [python]
-    severity: ERROR
-
-  - id: avoid-raw-sql
-    patterns:
-      - pattern-either:
-          - pattern: $MODEL.objects.raw($QUERY, ...)
-          - pattern: django.db.models.expressions.RawSQL(...)
-    message: You should be very careful whenever you write raw SQL. Consider using Django ORM before raw SQL. See https://docs.djangoproject.com/en/3.0/topics/db/sql/#passing-parameters-into-raw
-    metadata:
-      cwe: "CWE-89: Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection')"
-      owasp: "A1: Injection"
-      references:
-        - https://docs.djangoproject.com/en/3.0/ref/models/expressions/#raw-sql-expressions
-        - https://blog.r2c.dev/2020/preventing-sql-injection-a-django-authors-perspective/
-    languages: [python]
-    severity: ERROR
-
-  - id: django-secure-set-cookie
-    patterns:
-      - pattern-either:
-          - pattern-inside: |
-              import django.http.HttpResponse
-              ...
-          - pattern-inside: |
-              import django.shortcuts.render
-              ...
-            # Exclude vendored i18n code
-      - pattern-not-inside: |
-          LANGUAGE_QUERY_PARAMETER = 'language'
-          ...
-          def set_language(request):
-              ...
-          # Exclude vendored contrib/messages/storage/cookie.py
-      - pattern-not-inside: |
-          class CookieStorage(django.contrib.messages.storage.base.BaseStorage):
-              ...
-          # Exclude cookies handled by vendored middleware
-      - pattern-not: response.set_cookie(django.conf.settings.SESSION_COOKIE_NAME, ...)
-      - pattern-not: response.set_cookie(django.conf.settings.CSRF_COOKIE_NAME, ...)
-      - pattern-not: response.set_cookie(django.conf.settings.LANGUAGE_COOKIE_NAME, ...)
-      - pattern-not: response.set_cookie(rest_framework_jwt.settings.api_settings.JWT_AUTH_COOKIE, ...)
-      - pattern-not: response.set_cookie(..., secure=$A, httponly=$B, samesite=$C, ...)
-      - pattern-not: response.set_cookie(..., **$A)
-      - pattern: response.set_cookie(...)
-    message: |
-      Django cookies should be handled securely by setting secure=True, httponly=True, and samesite='Lax' in
-      response.set_cookie(...). If your situation calls for different settings, explicitly disable the setting.
-      If you want to send the cookie over http, set secure=False.  If you want to let client-side JavaScript
-      read the cookie, set httponly=False. If you want to attach cookies to requests for external sites,
-      set samesite=None.
-    metadata:
-      cwe: "CWE-614: Sensitive Cookie in HTTPS Session Without 'Secure' Attribute"
-      owasp: "A3: Sensitive Data Exposure"
-      references:
-        - https://docs.djangoproject.com/en/3.0/ref/request-response/#django.http.HttpResponse.set_cookie
-        - https://blog.r2c.dev/2020/bento-check-keeping-cookies-safe-in-flask/
-        - https://bento.dev/checks/flask/secure-set-cookie/
-    languages: [python]
-    severity: WARNING
-
-  - id: unvalidated-password
-    patterns:
-      - pattern-not-inside: |
-          if <... django.contrib.auth.password_validation.validate_password(...) ...>:
-              ...
-      - pattern-not-inside: |
-          django.contrib.auth.password_validation.validate_password(...)
-          ...
-      - pattern-not-inside: |
-          try:
-            ...
-            django.contrib.auth.password_validation.validate_password(...)
-            ...
-          except $EX:
-            ...
-          ...
-      - pattern-not-inside: |
-          try:
-            ...
-            django.contrib.auth.password_validation.validate_password(...)
-            ...
-          except $EX as $E:
-            ...
-          ...
-      - pattern-not: UserModel().set_password($X)
-      - pattern: $MODEL.set_password($X)
-    fix: |
-      if django.contrib.auth.password_validation.validate_password($X, user=$MODEL):
-          $MODEL.set_password($X)
-    message: |
-      The password on '$MODEL' is being set without validating the password.
-      Call django.contrib.auth.password_validation.validate_password() with
-      validation functions before setting the password. See
-      https://docs.djangoproject.com/en/3.0/topics/auth/passwords/
-      for more information.
-    metadata:
-      cwe: "CWE-521: Weak Password Requirements"
-      owasp: "A2: Broken Authentication"
-      references:
-        - https://docs.djangoproject.com/en/3.0/topics/auth/passwords/#module-django.contrib.auth.password_validation
-    languages: [python]
-    severity: WARNING
-
-  - id: mass-assignment
-    languages: [python]
-    severity: WARNING
-    message: |
-      Mass assignment detected. This can result in assignment to
-      model fields that are unintended and can be exploited by
-      an attacker. Instead of using '**request.$W', assign each field you
-      want to edit individually to prevent mass assignment. You can read
-      more about mass assignment at
-      https://cheatsheetseries.owasp.org/cheatsheets/Mass_Assignment_Cheat_Sheet.html.
-    metadata:
-      cwe: "CWE-915: Improperly Controlled Modification of Dynamically-Determined Object Attributes"
-      owasp: "A1: Injection"
-      owaspapi: "API6: Mass Assignment"
-      references:
-        - https://cheatsheetseries.owasp.org/cheatsheets/Mass_Assignment_Cheat_Sheet.html
-    patterns:
-      - pattern-either:
-          - pattern: $MODEL.objects.create(**request.$W)
-          - pattern: |
-              $OBJ.update(**request.$W)
-              ...
-              $OBJ.save()
-
-  - id: open-redirect
-    message: |
-      Data from request ($DATA) is passed to redirect(). This is an open redirect and could be exploited.
-      Ensure you are redirecting to safe URLs by using django.utils.http.is_safe_url().
-      See https://cwe.mitre.org/data/definitions/601.html for more information.
-    metadata:
-      cwe: "CWE-601: URL Redirection to Untrusted Site ('Open Redirect')"
-      owasp: "A1: Injection"
-      references:
-        - https://www.djm.org.uk/posts/djangos-little-protections-word-redirect-dangers/
-        - https://github.com/django/django/blob/d1b7bd030b1db111e1a3505b1fc029ab964382cc/django/utils/http.py#L231
-    languages: [python]
-    severity: WARNING
-    patterns:
-      - pattern-inside: |
-          def $FUNC(...):
-            ...
-      - pattern-not-inside: |
-          def $FUNC(...):
-            ...
-            django.utils.http.is_safe_url(...)
-            ...
-      - pattern-not-inside: |
-          def $FUNC(...):
-            ...
-            if <... django.utils.http.is_safe_url(...) ...>:
-              ...
-      - pattern-either:
-          - pattern: django.shortcuts.redirect(..., request.$W.get(...), ...)
-          - pattern: django.shortcuts.redirect(..., $S.format(..., request.$W.get(...), ...), ...)
-          - pattern: django.shortcuts.redirect(..., $S % request.$W.get(...), ...)
-          - pattern: django.shortcuts.redirect(..., f"...{request.$W.get(...)}...", ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.shortcuts.redirect(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = $DATA
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.shortcuts.redirect(..., $STR.format(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = $STR.format(..., $DATA, ...)
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.shortcuts.redirect(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.shortcuts.redirect(..., f"...{$DATA}...", ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.shortcuts.redirect(..., $STR + $DATA, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = $STR + $DATA
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: $A = django.shortcuts.redirect(..., request.$W.get(...), ...)
-          - pattern: $A = django.shortcuts.redirect(..., $S.format(..., request.$W.get(...), ...), ...)
-          - pattern: $A = django.shortcuts.redirect(..., $S % request.$W.get(...), ...)
-          - pattern: $A = django.shortcuts.redirect(..., f"...{request.$W.get(...)}...", ...)
-          - pattern: return django.shortcuts.redirect(..., request.$W.get(...), ...)
-          - pattern: return django.shortcuts.redirect(..., $S.format(..., request.$W.get(...), ...), ...)
-          - pattern: return django.shortcuts.redirect(..., $S % request.$W.get(...), ...)
-          - pattern: return django.shortcuts.redirect(..., f"...{request.$W.get(...)}...", ...)
-          - pattern: django.shortcuts.redirect(..., request.$W(...), ...)
-          - pattern: django.shortcuts.redirect(..., $S.format(..., request.$W(...), ...), ...)
-          - pattern: django.shortcuts.redirect(..., $S % request.$W(...), ...)
-          - pattern: django.shortcuts.redirect(..., f"...{request.$W(...)}...", ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.shortcuts.redirect(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = $DATA
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.shortcuts.redirect(..., $STR.format(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = $STR.format(..., $DATA, ...)
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.shortcuts.redirect(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.shortcuts.redirect(..., f"...{$DATA}...", ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.shortcuts.redirect(..., $STR + $DATA, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = $STR + $DATA
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: $A = django.shortcuts.redirect(..., request.$W(...), ...)
-          - pattern: $A = django.shortcuts.redirect(..., $S.format(..., request.$W(...), ...), ...)
-          - pattern: $A = django.shortcuts.redirect(..., $S % request.$W(...), ...)
-          - pattern: $A = django.shortcuts.redirect(..., f"...{request.$W(...)}...", ...)
-          - pattern: return django.shortcuts.redirect(..., request.$W(...), ...)
-          - pattern: return django.shortcuts.redirect(..., $S.format(..., request.$W(...), ...), ...)
-          - pattern: return django.shortcuts.redirect(..., $S % request.$W(...), ...)
-          - pattern: return django.shortcuts.redirect(..., f"...{request.$W(...)}...", ...)
-          - pattern: django.shortcuts.redirect(..., request.$W[...], ...)
-          - pattern: django.shortcuts.redirect(..., $S.format(..., request.$W[...], ...), ...)
-          - pattern: django.shortcuts.redirect(..., $S % request.$W[...], ...)
-          - pattern: django.shortcuts.redirect(..., f"...{request.$W[...]}...", ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.shortcuts.redirect(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = $DATA
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.shortcuts.redirect(..., $STR.format(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = $STR.format(..., $DATA, ...)
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.shortcuts.redirect(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.shortcuts.redirect(..., f"...{$DATA}...", ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.shortcuts.redirect(..., $STR + $DATA, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = $STR + $DATA
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: $A = django.shortcuts.redirect(..., request.$W[...], ...)
-          - pattern: $A = django.shortcuts.redirect(..., $S.format(..., request.$W[...], ...), ...)
-          - pattern: $A = django.shortcuts.redirect(..., $S % request.$W[...], ...)
-          - pattern: $A = django.shortcuts.redirect(..., f"...{request.$W[...]}...", ...)
-          - pattern: return django.shortcuts.redirect(..., request.$W[...], ...)
-          - pattern: return django.shortcuts.redirect(..., $S.format(..., request.$W[...], ...), ...)
-          - pattern: return django.shortcuts.redirect(..., $S % request.$W[...], ...)
-          - pattern: return django.shortcuts.redirect(..., f"...{request.$W[...]}...", ...)
-          - pattern: django.shortcuts.redirect(..., request.$W, ...)
-          - pattern: django.shortcuts.redirect(..., $S.format(..., request.$W, ...), ...)
-          - pattern: django.shortcuts.redirect(..., $S % request.$W, ...)
-          - pattern: django.shortcuts.redirect(..., f"...{request.$W}...", ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.shortcuts.redirect(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $DATA
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.shortcuts.redirect(..., $STR.format(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $STR.format(..., $DATA, ...)
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.shortcuts.redirect(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.shortcuts.redirect(..., f"...{$DATA}...", ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.shortcuts.redirect(..., $STR + $DATA, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $STR + $DATA
-              ...
-              django.shortcuts.redirect(..., $INTERM, ...)
-          - pattern: $A = django.shortcuts.redirect(..., request.$W, ...)
-          - pattern: $A = django.shortcuts.redirect(..., $S.format(..., request.$W, ...), ...)
-          - pattern: $A = django.shortcuts.redirect(..., $S % request.$W, ...)
-          - pattern: $A = django.shortcuts.redirect(..., f"...{request.$W}...", ...)
-          - pattern: return django.shortcuts.redirect(..., request.$W, ...)
-          - pattern: return django.shortcuts.redirect(..., $S.format(..., request.$W, ...), ...)
-          - pattern: return django.shortcuts.redirect(..., $S % request.$W, ...)
-          - pattern: return django.shortcuts.redirect(..., f"...{request.$W}...", ...)
-          - pattern: django.http.HttpResponseRedirect(..., request.$W.get(...), ...)
-          - pattern: django.http.HttpResponseRedirect(..., $S.format(..., request.$W.get(...), ...), ...)
-          - pattern: django.http.HttpResponseRedirect(..., $S % request.$W.get(...), ...)
-          - pattern: django.http.HttpResponseRedirect(..., f"...{request.$W.get(...)}...", ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.http.HttpResponseRedirect(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = $DATA
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.http.HttpResponseRedirect(..., $STR.format(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = $STR.format(..., $DATA, ...)
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.http.HttpResponseRedirect(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.http.HttpResponseRedirect(..., f"...{$DATA}...", ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.http.HttpResponseRedirect(..., $STR + $DATA, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = $STR + $DATA
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: $A = django.http.HttpResponseRedirect(..., request.$W.get(...), ...)
-          - pattern: $A = django.http.HttpResponseRedirect(..., $S.format(..., request.$W.get(...), ...), ...)
-          - pattern: $A = django.http.HttpResponseRedirect(..., $S % request.$W.get(...), ...)
-          - pattern: $A = django.http.HttpResponseRedirect(..., f"...{request.$W.get(...)}...", ...)
-          - pattern: return django.http.HttpResponseRedirect(..., request.$W.get(...), ...)
-          - pattern: return django.http.HttpResponseRedirect(..., $S.format(..., request.$W.get(...), ...), ...)
-          - pattern: return django.http.HttpResponseRedirect(..., $S % request.$W.get(...), ...)
-          - pattern: return django.http.HttpResponseRedirect(..., f"...{request.$W.get(...)}...", ...)
-          - pattern: django.http.HttpResponseRedirect(..., request.$W(...), ...)
-          - pattern: django.http.HttpResponseRedirect(..., $S.format(..., request.$W(...), ...), ...)
-          - pattern: django.http.HttpResponseRedirect(..., $S % request.$W(...), ...)
-          - pattern: django.http.HttpResponseRedirect(..., f"...{request.$W(...)}...", ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.http.HttpResponseRedirect(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = $DATA
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.http.HttpResponseRedirect(..., $STR.format(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = $STR.format(..., $DATA, ...)
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.http.HttpResponseRedirect(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.http.HttpResponseRedirect(..., f"...{$DATA}...", ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.http.HttpResponseRedirect(..., $STR + $DATA, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = $STR + $DATA
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: $A = django.http.HttpResponseRedirect(..., request.$W(...), ...)
-          - pattern: $A = django.http.HttpResponseRedirect(..., $S.format(..., request.$W(...), ...), ...)
-          - pattern: $A = django.http.HttpResponseRedirect(..., $S % request.$W(...), ...)
-          - pattern: $A = django.http.HttpResponseRedirect(..., f"...{request.$W(...)}...", ...)
-          - pattern: return django.http.HttpResponseRedirect(..., request.$W(...), ...)
-          - pattern: return django.http.HttpResponseRedirect(..., $S.format(..., request.$W(...), ...), ...)
-          - pattern: return django.http.HttpResponseRedirect(..., $S % request.$W(...), ...)
-          - pattern: return django.http.HttpResponseRedirect(..., f"...{request.$W(...)}...", ...)
-          - pattern: django.http.HttpResponseRedirect(..., request.$W[...], ...)
-          - pattern: django.http.HttpResponseRedirect(..., $S.format(..., request.$W[...], ...), ...)
-          - pattern: django.http.HttpResponseRedirect(..., $S % request.$W[...], ...)
-          - pattern: django.http.HttpResponseRedirect(..., f"...{request.$W[...]}...", ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.http.HttpResponseRedirect(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = $DATA
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.http.HttpResponseRedirect(..., $STR.format(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = $STR.format(..., $DATA, ...)
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.http.HttpResponseRedirect(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.http.HttpResponseRedirect(..., f"...{$DATA}...", ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.http.HttpResponseRedirect(..., $STR + $DATA, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = $STR + $DATA
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: $A = django.http.HttpResponseRedirect(..., request.$W[...], ...)
-          - pattern: $A = django.http.HttpResponseRedirect(..., $S.format(..., request.$W[...], ...), ...)
-          - pattern: $A = django.http.HttpResponseRedirect(..., $S % request.$W[...], ...)
-          - pattern: $A = django.http.HttpResponseRedirect(..., f"...{request.$W[...]}...", ...)
-          - pattern: return django.http.HttpResponseRedirect(..., request.$W[...], ...)
-          - pattern: return django.http.HttpResponseRedirect(..., $S.format(..., request.$W[...], ...), ...)
-          - pattern: return django.http.HttpResponseRedirect(..., $S % request.$W[...], ...)
-          - pattern: return django.http.HttpResponseRedirect(..., f"...{request.$W[...]}...", ...)
-          - pattern: django.http.HttpResponseRedirect(..., request.$W, ...)
-          - pattern: django.http.HttpResponseRedirect(..., $S.format(..., request.$W, ...), ...)
-          - pattern: django.http.HttpResponseRedirect(..., $S % request.$W, ...)
-          - pattern: django.http.HttpResponseRedirect(..., f"...{request.$W}...", ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.http.HttpResponseRedirect(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $DATA
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.http.HttpResponseRedirect(..., $STR.format(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $STR.format(..., $DATA, ...)
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.http.HttpResponseRedirect(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.http.HttpResponseRedirect(..., f"...{$DATA}...", ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.http.HttpResponseRedirect(..., $STR + $DATA, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $STR + $DATA
-              ...
-              django.http.HttpResponseRedirect(..., $INTERM, ...)
-          - pattern: $A = django.http.HttpResponseRedirect(..., request.$W, ...)
-          - pattern: $A = django.http.HttpResponseRedirect(..., $S.format(..., request.$W, ...), ...)
-          - pattern: $A = django.http.HttpResponseRedirect(..., $S % request.$W, ...)
-          - pattern: $A = django.http.HttpResponseRedirect(..., f"...{request.$W}...", ...)
-          - pattern: return django.http.HttpResponseRedirect(..., request.$W, ...)
-          - pattern: return django.http.HttpResponseRedirect(..., $S.format(..., request.$W, ...), ...)
-          - pattern: return django.http.HttpResponseRedirect(..., $S % request.$W, ...)
-          - pattern: return django.http.HttpResponseRedirect(..., f"...{request.$W}...", ...)
-      - metavariable-regex:
-          metavariable: $W
-          regex: (?!get_full_path)
-
-  - id: reflected-data-httpresponse
-    message:
-      Found request data reflected into HttpResponse. This could be vulnerable to XSS. Ensure the request data is properly
-      escaped or sanitzed.
-    metadata:
-      cwe: "CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')"
-      owasp: "A7: Cross-Site Scripting (XSS)"
-      references:
-        - https://django-book.readthedocs.io/en/latest/chapter20.html#cross-site-scripting-xss
-    languages: [python]
-    severity: WARNING
-    patterns:
-      - pattern-inside: |
-          def $FUNC(...):
-            ...
-      - pattern-either:
-          - pattern: django.http.HttpResponse(..., $S.format(..., request.$W.get(...), ...), ...)
-          - pattern: django.http.HttpResponse(..., $S % request.$W.get(...), ...)
-          - pattern: django.http.HttpResponse(..., f"...{request.$W.get(...)}...", ...)
-          - pattern: django.http.HttpResponse(..., request.$W.get(...), ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.http.HttpResponse(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = $DATA
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.http.HttpResponse(..., $STR.format(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = $STR.format(..., $DATA, ...)
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.http.HttpResponse(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.http.HttpResponse(..., f"...{$DATA}...", ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.http.HttpResponse(..., $STR + $DATA, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = $STR + $DATA
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: $A = django.http.HttpResponse(..., request.$W.get(...), ...)
-          - pattern: return django.http.HttpResponse(..., request.$W.get(...), ...)
-          - pattern: django.http.HttpResponse(..., $S.format(..., request.$W(...), ...), ...)
-          - pattern: django.http.HttpResponse(..., $S % request.$W(...), ...)
-          - pattern: django.http.HttpResponse(..., f"...{request.$W(...)}...", ...)
-          - pattern: django.http.HttpResponse(..., request.$W(...), ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.http.HttpResponse(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = $DATA
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.http.HttpResponse(..., $STR.format(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = $STR.format(..., $DATA, ...)
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.http.HttpResponse(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.http.HttpResponse(..., f"...{$DATA}...", ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.http.HttpResponse(..., $STR + $DATA, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = $STR + $DATA
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: $A = django.http.HttpResponse(..., request.$W(...), ...)
-          - pattern: return django.http.HttpResponse(..., request.$W(...), ...)
-          - pattern: django.http.HttpResponse(..., $S.format(..., request.$W[...], ...), ...)
-          - pattern: django.http.HttpResponse(..., $S % request.$W[...], ...)
-          - pattern: django.http.HttpResponse(..., f"...{request.$W[...]}...", ...)
-          - pattern: django.http.HttpResponse(..., request.$W[...], ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.http.HttpResponse(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = $DATA
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.http.HttpResponse(..., $STR.format(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = $STR.format(..., $DATA, ...)
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.http.HttpResponse(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.http.HttpResponse(..., f"...{$DATA}...", ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.http.HttpResponse(..., $STR + $DATA, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = $STR + $DATA
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: $A = django.http.HttpResponse(..., request.$W[...], ...)
-          - pattern: return django.http.HttpResponse(..., request.$W[...], ...)
-          - pattern: django.http.HttpResponse(..., $S.format(..., request.$W, ...), ...)
-          - pattern: django.http.HttpResponse(..., $S % request.$W, ...)
-          - pattern: django.http.HttpResponse(..., f"...{request.$W}...", ...)
-          - pattern: django.http.HttpResponse(..., request.$W, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.http.HttpResponse(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $DATA
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.http.HttpResponse(..., $STR.format(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $STR.format(..., $DATA, ...)
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.http.HttpResponse(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.http.HttpResponse(..., f"...{$DATA}...", ...)
-          - pattern: $A = django.http.HttpResponse(..., request.$W, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $STR + $DATA
-              ...
-              $A = django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: return django.http.HttpResponse(..., request.$W, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.http.HttpResponse(..., $STR + $DATA, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $STR + $DATA
-              ...
-              django.http.HttpResponse(..., $INTERM, ...)
-
-  - id: reflected-data-httpresponsebadrequest
-    message:
-      Found request data reflected into HttpResponseBadRequest. This could be vulnerable to XSS. Ensure the request data
-      is properly escaped or sanitzed.
-    metadata:
-      cwe: "CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')"
-      owasp: "A7: Cross-Site Scripting (XSS)"
-      references:
-        - https://django-book.readthedocs.io/en/latest/chapter20.html#cross-site-scripting-xss
-    languages: [python]
-    severity: WARNING
-    patterns:
-      - pattern-inside: |
-          def $FUNC(...):
-            ...
-      - pattern-either:
-          - pattern: django.http.HttpResponseBadRequest(..., $S.format(..., request.$W.get(...), ...), ...)
-          - pattern: django.http.HttpResponseBadRequest(..., $S % request.$W.get(...), ...)
-          - pattern: django.http.HttpResponseBadRequest(..., f"...{request.$W.get(...)}...", ...)
-          - pattern: django.http.HttpResponseBadRequest(..., request.$W.get(...), ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.http.HttpResponseBadRequest(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = $DATA
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.http.HttpResponseBadRequest(..., $STR.format(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = $STR.format(..., $DATA, ...)
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.http.HttpResponseBadRequest(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.http.HttpResponseBadRequest(..., f"...{$DATA}...", ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.http.HttpResponseBadRequest(..., $STR + $DATA, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = $STR + $DATA
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: $A = django.http.HttpResponseBadRequest(..., request.$W.get(...), ...)
-          - pattern: return django.http.HttpResponseBadRequest(..., request.$W.get(...), ...)
-          - pattern: django.http.HttpResponseBadRequest(..., $S.format(..., request.$W(...), ...), ...)
-          - pattern: django.http.HttpResponseBadRequest(..., $S % request.$W(...), ...)
-          - pattern: django.http.HttpResponseBadRequest(..., f"...{request.$W(...)}...", ...)
-          - pattern: django.http.HttpResponseBadRequest(..., request.$W(...), ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.http.HttpResponseBadRequest(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = $DATA
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.http.HttpResponseBadRequest(..., $STR.format(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = $STR.format(..., $DATA, ...)
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.http.HttpResponseBadRequest(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.http.HttpResponseBadRequest(..., f"...{$DATA}...", ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.http.HttpResponseBadRequest(..., $STR + $DATA, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = $STR + $DATA
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: $A = django.http.HttpResponseBadRequest(..., request.$W(...), ...)
-          - pattern: return django.http.HttpResponseBadRequest(..., request.$W(...), ...)
-          - pattern: django.http.HttpResponseBadRequest(..., $S.format(..., request.$W[...], ...), ...)
-          - pattern: django.http.HttpResponseBadRequest(..., $S % request.$W[...], ...)
-          - pattern: django.http.HttpResponseBadRequest(..., f"...{request.$W[...]}...", ...)
-          - pattern: django.http.HttpResponseBadRequest(..., request.$W[...], ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.http.HttpResponseBadRequest(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = $DATA
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.http.HttpResponseBadRequest(..., $STR.format(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = $STR.format(..., $DATA, ...)
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.http.HttpResponseBadRequest(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.http.HttpResponseBadRequest(..., f"...{$DATA}...", ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.http.HttpResponseBadRequest(..., $STR + $DATA, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = $STR + $DATA
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: $A = django.http.HttpResponseBadRequest(..., request.$W[...], ...)
-          - pattern: return django.http.HttpResponseBadRequest(..., request.$W[...], ...)
-          - pattern: django.http.HttpResponseBadRequest(..., $S.format(..., request.$W, ...), ...)
-          - pattern: django.http.HttpResponseBadRequest(..., $S % request.$W, ...)
-          - pattern: django.http.HttpResponseBadRequest(..., f"...{request.$W}...", ...)
-          - pattern: django.http.HttpResponseBadRequest(..., request.$W, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.http.HttpResponseBadRequest(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $DATA
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.http.HttpResponseBadRequest(..., $STR.format(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $STR.format(..., $DATA, ...)
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.http.HttpResponseBadRequest(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.http.HttpResponseBadRequest(..., f"...{$DATA}...", ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.http.HttpResponseBadRequest(..., $STR + $DATA, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $STR + $DATA
-              ...
-              django.http.HttpResponseBadRequest(..., $INTERM, ...)
-          - pattern: $A = django.http.HttpResponseBadRequest(..., request.$W, ...)
-          - pattern: return django.http.HttpResponseBadRequest(..., request.$W, ...)
-
-  - id: request-data-fileresponse
-    message:
-      Found request data opening a file into FileResponse. This is dangerous because an attacker could specify an arbitrary
-      file to read, leaking data. Be sure to validate or sanitize the filename before using it in FileResponse.
-    metadata:
-      cwe: "CWE-22: Improper Limitation of a Pathname to a Restricted Directory ('Path Traversal')"
-      owasp: "A1: Injection"
-      references:
-        - https://django-book.readthedocs.io/en/latest/chapter20.html#cross-site-scripting-xss
-    languages: [python]
-    severity: WARNING
-    patterns:
-      - pattern-inside: |
-          def $FUNC(...):
-            ...
-      - pattern-either:
-          - pattern: django.http.FileResponse(..., request.$W.get(...), ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              django.http.FileResponse(..., open($DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = open($DATA, ...)
-              ...
-              django.http.FileResponse(..., $INTERM, ...)
-          - pattern: $A = django.http.FileResponse(..., request.$W.get(...), ...)
-          - pattern: return django.http.FileResponse(..., request.$W.get(...), ...)
-          - pattern: django.http.FileResponse(..., request.$W(...), ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              django.http.FileResponse(..., open($DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = open($DATA, ...)
-              ...
-              django.http.FileResponse(..., $INTERM, ...)
-          - pattern: $A = django.http.FileResponse(..., request.$W(...), ...)
-          - pattern: return django.http.FileResponse(..., request.$W(...), ...)
-          - pattern: django.http.FileResponse(..., request.$W[...], ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              django.http.FileResponse(..., open($DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = open($DATA, ...)
-              ...
-              django.http.FileResponse(..., $INTERM, ...)
-          - pattern: $A = django.http.FileResponse(..., request.$W[...], ...)
-          - pattern: return django.http.FileResponse(..., request.$W[...], ...)
-          - pattern: django.http.FileResponse(..., request.$W, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              django.http.FileResponse(..., open($DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = open($DATA, ...)
-              ...
-              django.http.FileResponse(..., $INTERM, ...)
-          - pattern: $A = django.http.FileResponse(..., request.$W, ...)
-          - pattern: return django.http.FileResponse(..., request.$W, ...)
-
-  - id: request-data-write
-    message: |
-      Found request data in '.write(...)'. This could be dangerous if a malicious
-      actor is able to control data into sensitive files. For example, a malicious
-      actor could force rolling of critical log files, or cause a denial-of-service
-      by using up available disk space. Ensure content is validated.
-    metadata:
-      cwe: "CWE-93: Improper Neutralization of CRLF Sequences ('CRLF Injection')"
-      owasp: "A1: Injection"
-    languages: [python]
-    severity: WARNING
-    patterns:
-      - pattern-either:
-          - pattern: $F.write(..., request.$W.get(...), ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $F.write(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = $DATA
-              ...
-              $F.write(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $F.write(..., $B.$C(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = $B.$C(..., $DATA, ...)
-              ...
-              $F.write(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $F.write(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              $F.write(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $F.write(..., f"...{$DATA}...", ...)
-          - pattern: |
-              $DATA = request.$W.get(...)
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              $F.write(..., $INTERM, ...)
-          - pattern: $A = $F.write(..., request.$W.get(...), ...)
-          - pattern: return $F.write(..., request.$W.get(...), ...)
-          - pattern: $F.write(..., request.$W(...), ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $F.write(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = $DATA
-              ...
-              $F.write(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $F.write(..., $B.$C(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = $B.$C(..., $DATA, ...)
-              ...
-              $F.write(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $F.write(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              $F.write(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $F.write(..., f"...{$DATA}...", ...)
-          - pattern: |
-              $DATA = request.$W(...)
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              $F.write(..., $INTERM, ...)
-          - pattern: $A = $F.write(..., request.$W(...), ...)
-          - pattern: return $F.write(..., request.$W(...), ...)
-          - pattern: $F.write(..., request.$W[...], ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $F.write(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = $DATA
-              ...
-              $F.write(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $F.write(..., $B.$C(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = $B.$C(..., $DATA, ...)
-              ...
-              $F.write(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $F.write(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              $F.write(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $F.write(..., f"...{$DATA}...", ...)
-          - pattern: |
-              $DATA = request.$W[...]
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              $F.write(..., $INTERM, ...)
-          - pattern: $A = $F.write(..., request.$W[...], ...)
-          - pattern: return $F.write(..., request.$W[...], ...)
-          - pattern: $F.write(..., request.$W, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $F.write(..., $DATA, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $DATA
-              ...
-              $F.write(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $F.write(..., $B.$C(..., $DATA, ...), ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $B.$C(..., $DATA, ...)
-              ...
-              $F.write(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $F.write(..., $STR % $DATA, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = $STR % $DATA
-              ...
-              $F.write(..., $INTERM, ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $F.write(..., f"...{$DATA}...", ...)
-          - pattern: |
-              $DATA = request.$W
-              ...
-              $INTERM = f"...{$DATA}..."
-              ...
-              $F.write(..., $INTERM, ...)
-          - pattern: $A = $F.write(..., request.$W, ...)
-          - pattern: return $F.write(..., request.$W, ...)
-
-  - id: password-empty-string
-    message: |
-      '$VAR' is the empty string and is being used to set the password on '$MODEL'.
-      If you meant to set an unusable password, set the password to None or call
-      'set_unusable_password()'.
-    metadata:
-      cwe: "CWE-521: Weak Password Requirements"
-      owasp: "A2: Broken Authentication"
-      references:
-        - https://docs.djangoproject.com/en/3.0/ref/contrib/auth/#django.contrib.auth.models.User.set_password
-    patterns:
-      - pattern-either:
-          - pattern: |
-              $MODEL.set_password($EMPTY)
-              ...
-              $MODEL.save()
-          - pattern: |
-              $VAR = $EMPTY
-              ...
-              $MODEL.set_password($VAR)
-              ...
-              $MODEL.save()
-      - metavariable-regex:
-          metavariable: $EMPTY
-          regex: (\'\'|\"\")
-    languages: [python]
-    severity: ERROR
-
-  - id: use-none-for-password-default
-    message: |
-      '$VAR' is using the empty string as its default and is being used to set
-      the password on '$MODEL'. If you meant to set an unusable password, set
-      the default value to 'None' or call 'set_unusable_password()'.
-    metadata:
-      cwe: "CWE-521: Weak Password Requirements"
-      owasp: "A2: Broken Authentication"
-      references:
-        - https://docs.djangoproject.com/en/3.0/ref/contrib/auth/#django.contrib.auth.models.User.set_password
-    patterns:
-      - pattern-either:
-          - pattern: |
-              $VAR = request.$W.get($X, "")
-              ...
-              $MODEL.set_password($VAR)
-              ...
-              $MODEL.save(...)
-          - pattern: |
-              def $F(..., $VAR="", ...):
-                ...
-                $MODEL.set_password($VAR)
-    fix-regex:
-      regex: (def.*|request.*)(""|'')
-      replacement: \1None
-    languages: [python]
-    severity: ERROR
-
-  - id: docker-arbitrary-container-run
-    patterns:
-      - pattern-either:
-          - pattern-inside: |
-              $CLIENT = docker.from_env()
-              ...
-          - pattern-inside: |
-              $CLIENT = docker.DockerClient(...)
-              ...
-      - pattern-either:
-          - pattern: |
-              $CLIENT.containers.run(...)
-          - pattern: |
-              $CLIENT.containers.create(...)
-      - pattern-not: |
-          $CLIENT.containers.run("...",...)
-      - pattern-not: |
-          $CLIENT.containers.create("...",...)
-    message: |
-      If unverified user data can reach the `run` or `create` method it can result in runing arbitrary container.
-    languages:
-      - python
-    severity: WARNING
-  # Flask check3: Flask application app.run best practices https://flask.palletsprojects.com/en/1.1.x/api/?highlight=run#flask.Flask.run
-
-  # . Rules for app.run() parameters
-  - id: avoid_app_run_with_bad_host
-    patterns:
-      - pattern-either:
-          - pattern: app.run(..., host="0.0.0.0", ...)
-          - pattern: app.run(..., "0.0.0.0", ...)
-    message: Running flask app with host 0.0.0.0 could expose the server publicly.
-    metadata:
-      cwe: "CWE-668: Exposure of Resource to Wrong Sphere"
-      owasp: "A6: Security Misconfiguration"
-    languages: [python]
-    severity: WARNING
-  # Flask check3: Flask application app.run best practices https://flask.palletsprojects.com/en/1.1.x/api/?highlight=run#flask.Flask.run
-
-  - id: avoid_using_app_run_directly
-    patterns:
-      - pattern-not-inside: |
-          if __name__ == '__main__':
-            ...
-      - pattern-not-inside: |
-          def $X(...):
-            ...
-      - pattern: app.run(...)
-    message: top-level app.run(...) is ignored by flask. Consider putting app.run(...) behind a guard, like inside a function
-    metadata:
-      cwe: "CWE-668: Exposure of Resource to Wrong Sphere"
-      owasp: "A6: Security Misconfiguration"
-    languages: [python]
-    severity: WARNING
-
-  - id: debug-enabled
-    patterns:
-      - pattern-inside: |
-          import flask
-          ...
-      - pattern: $APP.run(..., debug=True, ...)
-    message: |
-      Detected Flask app with debug=True. Do not deploy to production with this flag enabled
-      as it will leak sensitive information. Instead, consider using Flask configuration
-      variables or setting 'debug' using system environment variables.
-    metadata:
-      cwe: "CWE-489: Active Debug Code"
-      owasp: "A6: Security Misconfiguration"
-      references:
-        - https://labs.detectify.com/2015/10/02/how-patreon-got-hacked-publicly-exposed-werkzeug-debugger/
-    severity: WARNING
-    languages:
-      - python
-
-  - id: directly-returned-format-string
-    message: |
-      Detected Flask route directly returning a formatted string. This
-      is subject to cross-site scripting if user input can reach the string.
-      Consider using the template engine instead and rendering pages with
-      'render_template()'.
-    metadata:
-      cwe: "CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')"
-      owasp: "A7: Cross-site Scripting (XSS)"
-    languages:
-      - python
-    severity: WARNING
-    patterns:
-      - pattern-inside: |
-          @$APP.route(...)
-          def $FUNC(...):
-            ...
-      - pattern-not-inside: return "..."
-      - pattern-either:
-          - pattern: return "...".format(...)
-          - pattern: return "..." % ...
-          - pattern: return "..." + ...
-          - pattern: return ... + "..."
-          - pattern: return f"...{...}..."
-          - patterns:
-              - pattern: return $X
-              - pattern-either:
-                  - pattern-inside: |
-                      $X = "...".format(...)
-                      ...
-                  - pattern-inside: |
-                      $X = "..." % ...
-                      ...
-                  - pattern-inside: |
-                      $X = "..." + ...
-                      ...
-                  - pattern-inside: |
-                      $X = ... + "..."
-                      ...
-                  - pattern-inside: |
-                      $X = f"...{...}..."
-                      ...
-  # Flask check3: Avoid hardcoded config rules
-
-  - id: avoid_hardcoded_config_TESTING
-    pattern-either:
-      - pattern: $M.config['TESTING'] = True
-      - pattern: $M.config['TESTING'] = False
-      - pattern: $M.update(TESTING=True, ...)
-      - pattern: $M.update(TESTING=False, ...)
-    message: Hardcoded variable `TESTING` detected. Use environment variables or config files instead
-    metadata:
-      cwe: "CWE-489: Active Debug Code"
-      owasp: "A6: Security Misconfiguration"
-      references:
-        - https://bento.dev/checks/flask/avoid-hardcoded-config/
-        - https://flask.palletsprojects.com/en/1.1.x/config/?highlight=configuration#builtin-configuration-values
-        - https://flask.palletsprojects.com/en/1.1.x/config/?highlight=configuration#environment-and-debug-features
-    languages: [python]
-    severity: WARNING
-  - id: avoid_hardcoded_config_SECRET_KEY
-    pattern-either:
-      - pattern: $M.update(SECRET_KEY="=~/.*/")
-      - pattern: $M.config['SECRET_KEY'] = "=~/.*/"
-    message: Hardcoded variable `SECRET_KEY` detected. Use environment variables or config files instead
-    metadata:
-      cwe: "CWE-798: Use of Hard-coded Credentials"
-      owasp: "A2: Broken Authentication"
-      references:
-        - https://bento.dev/checks/flask/avoid-hardcoded-config/
-        - https://flask.palletsprojects.com/en/1.1.x/config/?highlight=configuration#builtin-configuration-values
-        - https://flask.palletsprojects.com/en/1.1.x/config/?highlight=configuration#environment-and-debug-features
-    languages: [python]
-    severity: ERROR
-  - id: avoid_hardcoded_config_ENV
-    pattern-either:
-      - pattern: $M.update(ENV="=~/^development|production$/")
-      - pattern: $M.config['ENV'] = "=~/^development|production$/"
-    message: Hardcoded variable `ENV` detected. Set this by using FLASK_ENV environment variable
-    metadata:
-      cwe: "CWE-489: Active Debug Code"
-      owasp: "A6: Security Misconfiguration"
-      references:
-        - https://bento.dev/checks/flask/avoid-hardcoded-config/
-        - https://flask.palletsprojects.com/en/1.1.x/config/?highlight=configuration#builtin-configuration-values
-        - https://flask.palletsprojects.com/en/1.1.x/config/?highlight=configuration#environment-and-debug-features
-    languages: [python]
-    severity: WARNING
-  - id: avoid_hardcoded_config_DEBUG
-    pattern-either:
-      - pattern: $M.update(DEBUG=True)
-      - pattern: $M.update(DEBUG=False)
-      - pattern: $M.config['DEBUG'] = True
-      - pattern: $M.config['DEBUG'] = False
-    message: Hardcoded variable `DEBUG` detected. Set this by using FLASK_DEBUG environment variable
-    metadata:
-      cwe: "CWE-489: Active Debug Code"
-      owasp: "A6: Security Misconfiguration"
-      references:
-        - https://bento.dev/checks/flask/avoid-hardcoded-config/
-        - https://flask.palletsprojects.com/en/1.1.x/config/?highlight=configuration#builtin-configuration-values
-        - https://flask.palletsprojects.com/en/1.1.x/config/?highlight=configuration#environment-and-debug-features
-    languages: [python]
-    severity: WARNING
-
-  - id: render-template-string
-    pattern: flask.render_template_string(...)
-    metadata:
-      cwe: "CWE-96: Improper Neutralization of Directives in Statically Saved Code ('Static Code Injection')"
-      owasp: "A1: Injection"
-      references:
-        - https://nvisium.com/blog/2016/03/09/exploring-ssti-in-flask-jinja2.html
-    message:
-      Found a template created with string formatting. This is susceptible to server-side template injection and cross-site
-      scripting attacks.
-    languages: [python]
-    severity: WARNING
-
-  - id: secure-set-cookie
-    patterns:
-      - pattern-either:
-          - pattern-inside: |
-              $RESP = flask.make_response(...)
-              ...
-          - pattern-inside: |
-              $RESP = flask.Response(...)
-              ...
-      - pattern-not: $RESPONSE.set_cookie(..., secure=$A, httponly=$B, samesite=$C, ...)
-      - pattern-not: $RESPONSE.set_cookie(..., **$A)
-      - pattern: $RESPONSE.set_cookie(...)
-    message: |
-      Flask cookies should be handled securely by setting secure=True, httponly=True, and samesite='Lax' in
-      response.set_cookie(...). If your situation calls for different settings, explicitly disable the setting.
-      If you want to send the cookie over http, set secure=False.  If you want to let client-side JavaScript
-      read the cookie, set httponly=False. If you want to attach cookies to requests for external sites,
-      set samesite=None.
-    metadata:
-      cwe: "CWE-614: Sensitive Cookie in HTTPS Session Without 'Secure' Attribute"
-      owasp: "A3: Sensitive Data Exposure"
-      references:
-        - https://blog.r2c.dev/2020/bento-check-keeping-cookies-safe-in-flask/
-        - https://bento.dev/checks/flask/secure-set-cookie/
-        - https://flask.palletsprojects.com/en/1.1.x/security/#set-cookie-options
-    languages: [python]
-    severity: WARNING
-
-  - id: flask-wtf-csrf-disabled
-    patterns:
-      - pattern: |
-          $APP.config['WTF_CSRF_ENABLED'] = False
-    message: |
-      `$APP.config['WTF_CSRF_ENABLED'] = False` is probably not what you want in production because it disables https://flask-wtf.readthedocs.io/en/stable/csrf.html CSRF protection
-    metadata:
-      cwe: "CWE-352: Cross-Site Request Forgery (CSRF)"
-      owasp: "A6: Security Misconfiguration"
-      references:
-        - https://flask-wtf.readthedocs.io/en/stable/csrf.html
-    severity: WARNING
-    languages:
-      - python
-
-  - id: os-system-injection
-    languages:
-      - python
-    severity: ERROR
-    message: >-
-      User data detected in os.system. This could be vulnerable to a command injection and should be avoided. If this
-      must be done, use the 'subprocess' module instead and pass the arguments as a list.
-    metadata:
-      cwe: "CWE-78: Improper Neutralization of Special Elements used in an OS Command ('OS Command Injection')"
-      owasp: "A1: Injection"
-      references:
-        - https://owasp.org/www-community/attacks/Command_Injection
-    patterns:
-      - pattern-either:
-          - patterns:
-              - pattern-inside: |
-                  @$APP.route($ROUTE, ...)
-                  def $FUNC(..., $ROUTEVAR, ...):
-                    ...
-              - pattern-either:
-                  - pattern: os.system(..., <... $ROUTEVAR ...>, ...)
-                  - pattern: |
-                      $INTERM = <... $ROUTEVAR ...>
-                      ...
-                      os.system(..., <... $INTERM ...>, ...)
-          - patterns:
-              - pattern-either:
-                  - pattern: os.system(..., <... flask.request.$W.get(...) ...>, ...)
-                  - pattern: os.system(..., <... flask.request.$W[...] ...>, ...)
-                  - pattern: os.system(..., <... flask.request.$W(...) ...>, ...)
-                  - pattern: os.system(..., <... flask.request.$W ...>, ...)
-          - patterns:
-              - pattern-either:
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W.get(...) ...>
-                          ...
-                          os.system(<... $INTERM ...>)
-                      - pattern: os.system(...)
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W[...] ...>
-                          ...
-                          os.system(<... $INTERM ...>)
-                      - pattern: os.system(...)
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W(...) ...>
-                          ...
-                          os.system(<... $INTERM ...>)
-                      - pattern: os.system(...)
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W ...>
-                          ...
-                          os.system(<... $INTERM ...>)
-                      - pattern: os.system(...)
-
-  - id: path-traversal-open
-    languages:
-      - python
-    severity: ERROR
-    message: >-
-      Found request data in a call to 'open'. Ensure the request data is validated or sanitized, otherwise it could result
-      in path traversal attacks.
-    metadata:
-      cwe: "CWE-22: Improper Limitation of a Pathname to a Restricted Directory ('Path Traversal')"
-      owasp: "A1: Injection"
-      references:
-        - https://owasp.org/www-community/attacks/Path_Traversal
-    patterns:
-      - pattern-either:
-          - patterns:
-              - pattern-inside: |
-                  @$APP.route($ROUTE, ...)
-                  def $FUNC(..., $ROUTEVAR, ...):
-                    ...
-              - pattern-either:
-                  - pattern: open(..., <... $ROUTEVAR ...>, ...)
-                  - pattern: |
-                      $INTERM = <... $ROUTEVAR ...>
-                      ...
-                      open(..., <... $INTERM ...>, ...)
-          - patterns:
-              - pattern-either:
-                  - pattern: open(..., <... flask.request.$W.get(...) ...>, ...)
-                  - pattern: open(..., <... flask.request.$W[...] ...>, ...)
-                  - pattern: open(..., <... flask.request.$W(...) ...>, ...)
-                  - pattern: open(..., <... flask.request.$W ...>, ...)
-          - patterns:
-              - pattern-either:
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W.get(...) ...>
-                          ...
-                          open(<... $INTERM ...>, ...)
-                      - pattern: open(...)
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W[...] ...>
-                          ...
-                          open(<... $INTERM ...>, ...)
-                      - pattern: open(...)
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W(...) ...>
-                          ...
-                          open(<... $INTERM ...>, ...)
-                      - pattern: open(...)
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W ...>
-                          ...
-                          open(<... $INTERM ...>, ...)
-                      - pattern: open(...)
-          - patterns:
-              - pattern-either:
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W.get(...) ...>
-                          ...
-                          with open(<... $INTERM ...>, ...) as $F:
-                            ...
-                      - pattern: open(...)
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W[...] ...>
-                          ...
-                          with open(<... $INTERM ...>, ...) as $F:
-                            ...
-                      - pattern: open(...)
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W(...) ...>
-                          ...
-                          with open(<... $INTERM ...>, ...) as $F:
-                            ...
-                      - pattern: open(...)
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W ...>
-                          ...
-                          with open(<... $INTERM ...>, ...) as $F:
-                            ...
-                      - pattern: open(...)
-
-  - id: ssrf-requests
-    languages:
-      - python
-    severity: ERROR
-    message:
-      Data from request object is passed to a new server-side request. This could lead to a server-side request forgery
-      (SSRF). To mitigate, ensure that schemes and hosts are validated against a whitelist, do not forward the response to the
-      user, and ensure proper authentication and transport-layer security in the proxied request.
-    metadata:
-      cwe: "CWE-918: Server-Side Request Forgery (SSRF)"
-      owasp: "A1: Injection"
-      references:
-        - https://owasp.org/www-community/attacks/Server_Side_Request_Forgery
-    patterns:
-      - pattern-either:
-          - patterns:
-              - pattern-inside: |
-                  @$APP.route($ROUTE, ...)
-                  def $ROUTE_FUNC(..., $ROUTEVAR, ...):
-                    ...
-              - pattern-either:
-                  - pattern: requests.$FUNC(..., <... $ROUTEVAR ...>, ...)
-                  - pattern: |
-                      $INTERM = <... $ROUTEVAR ...>
-                      ...
-                      requests.$FUNC(..., <... $INTERM ...>, ...)
-          - patterns:
-              - pattern-either:
-                  - pattern: requests.$FUNC(..., <... flask.request.$W.get(...) ...>, ...)
-                  - pattern: requests.$FUNC(..., <... flask.request.$W[...] ...>, ...)
-                  - pattern: requests.$FUNC(..., <... flask.request.$W(...) ...>, ...)
-                  - pattern: requests.$FUNC(..., <... flask.request.$W ...>, ...)
-          - patterns:
-              - pattern-either:
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W.get(...) ...>
-                          ...
-                          requests.$FUNC(<... $INTERM ...>, ...)
-                      - pattern: requests.$FUNC(...)
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W[...] ...>
-                          ...
-                          requests.$FUNC(<... $INTERM ...>, ...)
-                      - pattern: requests.$FUNC(...)
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W(...) ...>
-                          ...
-                          requests.$FUNC(<... $INTERM ...>, ...)
-                      - pattern: requests.$FUNC(...)
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W ...>
-                          ...
-                          requests.$FUNC(<... $INTERM ...>, ...)
-                      - pattern: requests.$FUNC(...)
-
-  - id: eval-injection
-    languages:
-      - python
-    severity: ERROR
-    message: Detected user data flowing into eval. This is code injection and should be avoided.
-    metadata:
-      cwe: "CWE-95: Improper Neutralization of Directives in Dynamically Evaluated Code ('Eval Injection')"
-      owasp: "A1: Injection"
-      references:
-        - https://nedbatchelder.com/blog/201206/eval_really_is_dangerous.html
-    patterns:
-      - pattern-either:
-          - patterns:
-              - pattern-inside: |
-                  @$APP.route($ROUTE, ...)
-                  def $FUNC(..., $ROUTEVAR, ...):
-                    ...
-              - pattern-either:
-                  - pattern: eval(..., <... $ROUTEVAR ...>, ...)
-                  - pattern: |
-                      $INTERM = <... $ROUTEVAR ...>
-                      ...
-                      eval(..., <... $INTERM ...>, ...)
-          - patterns:
-              - pattern-either:
-                  - pattern: eval(..., <... flask.request.$W.get(...) ...>, ...)
-                  - pattern: eval(..., <... flask.request.$W[...] ...>, ...)
-                  - pattern: eval(..., <... flask.request.$W(...) ...>, ...)
-                  - pattern: eval(..., <... flask.request.$W ...>, ...)
-          - patterns:
-              - pattern-either:
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W.get(...) ...>
-                          ...
-                          eval(..., <... $INTERM ...>, ...)
-                      - pattern: eval(...)
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W[...] ...>
-                          ...
-                          eval(..., <... $INTERM ...>, ...)
-                      - pattern: eval(...)
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W(...) ...>
-                          ...
-                          eval(..., <... $INTERM ...>, ...)
-                      - pattern: eval(...)
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W ...>
-                          ...
-                          eval(..., <... $INTERM ...>, ...)
-                      - pattern: eval(...)
-
-  - id: exec-injection
-    languages:
-      - python
-    severity: ERROR
-    message: Detected user data flowing into exec. This is code injection and should be avoided.
-    metadata:
-      cwe: "CWE-95: Improper Neutralization of Directives in Dynamically Evaluated Code ('Eval Injection')"
-      owasp: "A1: Injection"
-      references:
-        - https://nedbatchelder.com/blog/201206/exec_really_is_dangerous.html
-    patterns:
-      - pattern-either:
-          - patterns:
-              - pattern-inside: |
-                  @$APP.route($ROUTE, ...)
-                  def $FUNC(..., $ROUTEVAR, ...):
-                    ...
-              - pattern-either:
-                  - pattern: exec(..., <... $ROUTEVAR ...>, ...)
-                  - pattern: |
-                      $INTERM = <... $ROUTEVAR ...>
-                      ...
-                      exec(..., <... $INTERM ...>, ...)
-          - patterns:
-              - pattern-either:
-                  - pattern: exec(..., <... flask.request.$W.get(...) ...>, ...)
-                  - pattern: exec(..., <... flask.request.$W[...] ...>, ...)
-                  - pattern: exec(..., <... flask.request.$W(...) ...>, ...)
-                  - pattern: exec(..., <... flask.request.$W ...>, ...)
-          - patterns:
-              - pattern-either:
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W.get(...) ...>
-                          ...
-                          exec(..., <... $INTERM ...>, ...)
-                      - pattern: exec(...)
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W[...] ...>
-                          ...
-                          exec(..., <... $INTERM ...>, ...)
-                      - pattern: exec(...)
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W(...) ...>
-                          ...
-                          exec(..., <... $INTERM ...>, ...)
-                      - pattern: exec(...)
-                  - patterns:
-                      - pattern-inside: |
-                          $INTERM = <... flask.request.$W ...>
-                          ...
-                          exec(..., <... $INTERM ...>, ...)
-                      - pattern: exec(...)
-
-  - id: autoescape-disabled
-    patterns:
-      - pattern-not: jinja2.Environment(..., autoescape=True, ...)
-      - pattern-not: jinja2.Environment(..., autoescape=jinja2.select_autoescape(...), ...)
-      - pattern: jinja2.Environment(...)
-    fix-regex:
-      regex: (.*)\)
-      replacement: \1, autoescape=True)
-    message: >-
-      Detected a Jinja2 environment without autoescaping. Jinja2 does not autoescape by default.
-      This is dangerous if you are rendering to a browser because this allows for cross-site
-      scripting (XSS) attacks. If you are in a web context, enable autoescaping by setting
-      'autoescape=True.' You may also consider using 'jinja2.select_autoescape()' to only enable
-      automatic escaping for certain file extensions.
-    metadata:
-      cwe: "CWE-116: Improper Encoding or Escaping of Output"
-      owasp: "A6: Security Misconfiguration"
-      references:
-        - https://jinja.palletsprojects.com/en/2.11.x/api/#basics
-    languages: [python]
-    severity: WARNING
-
-  - id: jwt-python-exposed-data
-    message: |
-      The object is passed strictly to jwt.encode(...)
-      Make sure that sensitive information is not exposed through JWT token payload.
-    severity: WARNING
-    metadata:
-      owasp: A3:2017-Sensitive Data Exposure
-      cwe: "CWE-522: Insufficiently Protected Credentials"
-      source-rule-url: https://r2c.dev/blog/2020/hardcoded-secrets-unverified-tokens-and-other-common-jwt-mistakes/
-    languages: [python]
-    patterns:
-      - pattern-inside: |
-          def $FUNC(...,$INPUT,...):
-            ...
-      - pattern: |-
-          jwt.encode($INPUT,...)
-
-  - id: multiprocessing-recv
-    languages:
-      - python
-    message:
-      "The Connection.recv() method automatically unpickles the data it receives, which can be a security risk unless
-      you can trust the process which sent the message. Therefore, unless the connection object was produced using Pipe() you
-      should only use the recv() and send() methods after performing some sort of authentication. See more dettails: https://docs.python.org/3/library/multiprocessing.html?highlight=security#multiprocessing.connection.Connection"
-    metadata:
-      cwe: "CWE-502: Deserialization of Untrusted Data"
-      owasp: "A8: Insecure Deserialization"
-      references:
-        - https://docs.python.org/3/library/multiprocessing.html?highlight=security#multiprocessing.connection.Connection
-    pattern-either:
-      - pattern: multiprocessing.connection.Connection.recv(...)
-      - pattern: multiprocessing.connection.Client.recv(...)
-      - pattern: |
-          $C = multiprocessing.connection.Client(...)
-          ...
-          $C.recv(...)
-    severity: WARNING
-
-  - id: dangerous-spawn-process
-    patterns:
-      - pattern-either:
-          - patterns:
-              - pattern-not: os.$W("...", ...)
-              - pattern-either:
-                  - pattern: os.execl(...)
-                  - pattern: os.execle(...)
-                  - pattern: os.execlp(...)
-                  - pattern: os.execlpe(...)
-                  - pattern: os.execv(...)
-                  - pattern: os.execve(...)
-                  - pattern: os.execvp(...)
-                  - pattern: os.execvpe(...)
-                  - pattern: os.startfile(...)
-          - patterns:
-              - pattern-not: os.$W($MODE, "...", ...)
-              - pattern-either:
-                  - pattern: os.spawnl(...)
-                  - pattern: os.spawnle(...)
-                  - pattern: os.spawnlp(...)
-                  - pattern: os.spawnlpe(...)
-                  - pattern: os.spawnv(...)
-                  - pattern: os.spawnve(...)
-                  - pattern: os.spawnvp(...)
-                  - pattern: os.spawnvpe(...)
-    message: |
-      Found dynamic content when spawning a process. This is dangerous if external
-      data can reach this function call because it allows a malicious actor to
-      execute commands. Ensure no external data reaches here.
-    metadata:
-      cwe: "CWE-78: Improper Neutralization of Special Elements used in an OS Command ('OS Command Injection')"
-      owasp: "A1: Injection"
-    languages: [python]
-    severity: WARNING
-
-  - id: dangerous-subprocess-use
-    patterns:
-      - pattern-not: subprocess.$FUNC("...", ...)
-      - pattern-not: subprocess.$FUNC([...], ...)
-      - pattern-not: subprocess.CalledProcessError(...)
-      - pattern-not: subprocess.SubprocessError(...)
-      - pattern: subprocess.$FUNC(...)
-    message: |
-      Detected subprocess function '$FUNC' without a static string. If this data can be
-      controlled by a malicious actor, it may be an instance of command injection.
-      Audit the use of this call to ensure it is not controllable by an external resource.
-      You may consider using 'shlex.escape()'.
-    metadata:
-      owasp: "A1: Injection"
-      cwe: "CWE-78: Improper Neutralization of Special Elements used in an OS Command ('OS Command Injection')"
-      references:
-        - https://stackoverflow.com/questions/3172470/actual-meaning-of-shell-true-in-subprocess
-        - https://docs.python.org/3/library/subprocess.html
-        - https://docs.python.org/3/library/shlex.html
-    languages: [python]
-    severity: WARNING
-
-  - id: dangerous-system-call
-    patterns:
-      - pattern-not: os.$W("...", ...)
-      - pattern-either:
-          - pattern: os.system(...)
-          - pattern: os.popen(...)
-          - pattern: os.popen2(...)
-          - pattern: os.popen3(...)
-          - pattern: os.popen4(...)
-    message: >-
-      Found dynamic content used in a system call. This is dangerous if external
-      data can reach this function call because it allows a malicious actor to
-      execute commands. Use the 'subprocess' module instead, which is easier
-      to use without accidentally exposing a command injection vulnerability.
-    metadata:
-      cwe: "CWE-78: Improper Neutralization of Special Elements used in an OS Command ('OS Command Injection')"
-      owasp: "A1: Injection"
-    languages: [python]
-    severity: WARNING
-
-  - id: dynamic-urllib-use-detected
-    patterns:
-      - pattern-not: urllib.$W("...")
-      - pattern-not: urllib.request.$W("...")
-      - pattern-not: $OPENER.$W("...")
-      - pattern-either:
-          - patterns:
-              - pattern-either:
-                  - pattern: urllib.urlopen(...)
-                  - pattern: urllib.request.urlopen(...)
-                  - pattern: urllib.urlretrieve(...)
-                  - pattern: urllib.request.urlretrieve(...)
-          - patterns:
-              - pattern-either:
-                  - pattern-inside: |
-                      $OPENER = urllib.URLopener(...)
-                      ...
-                  - pattern-inside: |
-                      $OPENER = urllib.request.URLopener(...)
-                      ...
-                  - pattern-inside: |
-                      $OPENER = urllib.FancyURLopener(...)
-                      ...
-                  - pattern-inside: |
-                      $OPENER = urllib.request.FancyURLopener(...)
-                      ...
-              - pattern-either:
-                  - pattern: $OPENER.open(...)
-                  - pattern: $OPENER.retrieve(...)
-    message: >-
-      Detected a dynamic value being used with urllib. urllib supports 'file://' schemes,
-      so a dynamic value controlled by a malicious actor may allow them to read arbitrary files.
-      Audit uses of urllib calls to ensure user data cannot control the URLs, or consider
-      using the 'requests' library instead.
-    metadata:
-      cwe: "CWE-939: Improper Authorization in Handler for Custom URL Scheme"
-      owasp: "A1: Injection"
-      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/blacklists/calls.py#L163
-      bandit-code: B310
-    languages: [python]
-    severity: WARNING
-
-  - id: eval-detected
-    patterns:
-      - pattern-not: eval("...")
-      - pattern: eval(...)
-    message: |
-      Detected the use of eval(). eval() can be dangerous if used to evaluate
-      dynamic content. If this content can be input from outside the program, this
-      may be a code injection vulnerability. Ensure evaluated content is not definable
-      by external sources.
-    metadata:
-      cwe: "CWE-95: Improper Neutralization of Directives in Dynamically Evaluated Code ('Eval Injection')"
-      owasp: "A1: Injection"
-    languages: [python]
-    severity: WARNING
-
-  - id: exec-detected
-    patterns:
-      - pattern-not: exec("...")
-      - pattern: exec(...)
-    message: |
-      Detected the use of exec(). exec() can be dangerous if used to evaluate
-      dynamic content. If this content can be input from outside the program, this
-      may be a code injection vulnerability. Ensure evaluated content is not definable
-      by external sources.
-    metadata:
-      cwe: "CWE-95: Improper Neutralization of Directives in Dynamically Evaluated Code ('Eval Injection')"
-      owasp: "A1: Injection"
-    languages: [python]
-    severity: WARNING
-
-  - id: formatted-sql-query
-    patterns:
-      - pattern-either:
-          - pattern: $DB.execute("..." % ...)
-          - pattern: $DB.execute("...".format(...))
-          - pattern: $DB.execute(f"...")
-          - patterns:
-              - pattern-either:
-                  - pattern-inside: |
-                      $SQL = "..." % ...
-                      ...
-                  - pattern-inside: |
-                      $SQL = "...".format(...)
-                      ...
-                  - pattern-inside: |
-                      $SQL = f"...{$X}..."
-                      ...
-              - pattern: $DB.execute($SQL)
-    message: |
-      Detected possible formatted SQL query. Use parameterized queries instead.
-    metadata:
-      owasp: "A1: Injection"
-      cwe: "CWE-89: Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection')"
-      references:
-        - https://stackoverflow.com/questions/775296/mysql-parameterized-queries
-    severity: WARNING
-    languages:
-      - python
-
-  - id: ftplib
-    pattern: ftplib.$ANYTHING(...)
-    message: |
-      FTP does not encrypt communications by default. This can lead to sensitive
-      data being exposed. Ensure use of FTP here does not expose sensitive data.
-    metadata:
-      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L265
-      cwe: "CWE-319: Cleartext Transmission of Sensitive Information"
-      owasp: "A3: Sensitive Data Exposure"
-      bandit-code: B321
-      references:
-        - https://docs.python.org/3/library/telnetlib.html
-    severity: WARNING
-    languages:
-      - python
-
-  - id: hardcoded-password-default-argument
-    patterns:
-      - pattern: |
-          def $FUNC(..., password="...", ...):
-            ...
-    message: |
-      Hardcoded password is used as a default argument to '$FUNC'. This could be dangerous if
-      a real password is not supplied.
-    languages: [python]
-    severity: WARNING
-
-  - id: httpsconnection-detected
-    patterns:
-      - pattern-either:
-          - pattern: httplib.HTTPSConnection(...)
-          - pattern: http.client.HTTPSConnection(...)
-          - pattern: six.moves.http_client.HTTPSConnection(...)
-    message: |
-      The HTTPSConnection API has changed frequently with minor releases of Python.
-      Ensure you are using the API for your version of Python securely.
-      For example, Python 3 versions prior to 3.4.3 will not verify SSL certificates by default.
-      See https://docs.python.org/3/library/http.client.html#http.client.HTTPSConnection
-      for more information.
-    metadata:
-      owasp: "A6: Security Misconfiguration"
-      cwe: "CWE-295: Improper Certificate Validation"
-      references:
-        - https://docs.python.org/3/library/http.client.html#http.client.HTTPSConnection
-    severity: WARNING
-    languages:
-      - python
-
-  - id: insecure-file-permissions
-    patterns:
-      - pattern-either:
-          - pattern: os.chmod($FILENAME, $MODE, ...)
-          - pattern: os.lchmod($FILENAME, $MODE)
-          - pattern: os.fchmod($FD, $MODE)
-      - pattern-where-python: |-
-          import stat
-
-          def stat_to_bits(mode):
-            bits = 0
-            for flag in mode.split('|'):
-              try:
-                bits |= {k: v for k, v in stat.__dict__.items() if type(v) == int}[flag.strip().replace("stat.", "")]
-              except: # ignore things that aren't in stat module
-                continue
-            return bits
-
-          def numeric_to_bits(mode):
-            # Try combos of ints: 0o777, 511, 0x1ff
-            bits = 0
-            for num in mode.split("|"):
-              num = num.strip()
-              try:
-                tidbit = int(num)
-              except:
-                try:
-                  tidbit = int(num, 8)
-                except:
-                  try:
-                    tidbit = int(num, 16)
-                  except:
-                    try:
-                      tidbit = int(num, 2)
-                    except:
-                      tidbit = 0
-              bits |= tidbit
-            return bits
-
-          perms = vars['$MODE']
-          try:
-            if "stat" in perms:
-              mode = stat_to_bits(perms)
-            else:
-              mode = numeric_to_bits(perms)
-          except:
-            mode = 0 # can't resolve. ignore this.
-
-          filemode = stat.filemode(mode)
-          alert = False
-          if 'w' in filemode[-3:] or 'x' in filemode[-3:]:
-            alert = True
-          elif 'x' in filemode[-6:-3]:
-            alert = True
-          alert
-    message: |
-      Insecure file permissions detected.
-    languages: [python]
-    severity: WARNING
-
-  - id: mako-templates-detected
-    pattern: mako.template.Template(...)
-    message: |
-      Mako templates do not provide a global HTML escaping mechanism.
-      This means you must escape all sensitive data in your templates
-      using '| u' for URL escaping or '| h' for HTML escaping.
-      If you are using Mako to serve web content, consider using
-      a system such as Jinja2 which enables global escaping.
-    metadata:
-      cwe: "CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')"
-      owasp: "A7: Cross-Site Scripting (XSS)"
-      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/mako_templates.py
-      references:
-        - https://docs.makotemplates.org/en/latest/syntax.html#expression-escaping
-        - https://jinja.palletsprojects.com/en/2.11.x/intro/#
-    languages: [python]
-    severity: INFO
-
-  - id: marshal-usage
-    languages:
-      - python
-    message: |
-      The marshal module is not intended to be secure against erroneous or maliciously constructed data.
-      Never unmarshal data received from an untrusted or unauthenticated source.
-      See more details: https://docs.python.org/3/library/marshal.html?highlight=security
-    metadata:
-      cwe: "CWE-502: Deserialization of Untrusted Data"
-      owasp: "A8: Insecure Deserialization"
-      references:
-        - https://docs.python.org/3/library/marshal.html?highlight=security
-    pattern-either:
-      - pattern: marshal.dump(...)
-      - pattern: marshal.dumps(...)
-      - pattern: marshal.load(...)
-      - pattern: marshal.loads(...)
-    severity: WARNING
-
-  - id: paramiko-implicit-trust-host-key
-    patterns:
-      - pattern-inside: |
-          $CLIENT = paramiko.client.SSHClient(...)
-          ...
-          $CLIENT.set_missing_host_key_policy(...)
-      - pattern-either:
-          - pattern: paramiko.client.AutoAddPolicy
-          - pattern: paramiko.client.WarningPolicy
-    message: |
-      Detected a paramiko host key policy that implicitly trusts a server's
-      host key. Host keys should be verified to ensure the connection
-      is not to a malicious server. Use RejectPolicy or a custom subclass
-      instead.
-    metadata:
-      cwe: "CWE-322: Key Exchange without Entity Authentication"
-      owasp: "A3: Sensitive Data Exposure"
-      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/ssh_no_host_key_verification.py
-      references:
-        - http://docs.paramiko.org/en/stable/api/client.html#paramiko.client.AutoAddPolicy
-    languages: [python]
-    severity: WARNING
-
-  - id: ssl-wrap-socket-is-deprecated
-    pattern: ssl.wrap_socket(...)
-    message: |
-      'ssl.wrap_socket()' is deprecated. This function creates an insecure socket
-      without server name indication or hostname matching. Instead, create an SSL
-      context using 'ssl.SSLContext()' and use that to wrap a socket.
-    metadata:
-      cwe: "CWE-326: Inadequate Encryption Strength"
-      owasp: "A3: Sensitive Data Exposure"
-      references:
-        - https://docs.python.org/3/library/ssl.html#ssl.wrap_socket
-        - https://docs.python.org/3/library/ssl.html#ssl.SSLContext.wrap_socket
-    languages: [python]
-    severity: WARNING
-
-  - id: subprocess-shell-true
-    pattern: subprocess.$FUNC(..., shell=True, ...)
-    message: |
-      Found 'subprocess' function '$FUNC' with 'shell=True'. This is dangerous because this call will spawn
-      the command using a shell process. Doing so propagates current shell settings and variables, which
-      makes it much easier for a malicious actor to execute commands. Use 'shell=False' instead.
-    fix-regex:
-      regex: (shell\s*=\s*)True
-      replacement: \1False
-    metadata:
-      owasp: "A1: Injection"
-      cwe: "CWE-78: Improper Neutralization of Special Elements used in an OS Command ('OS Command Injection')"
-      references:
-        - https://stackoverflow.com/questions/3172470/actual-meaning-of-shell-true-in-subprocess
-        - https://docs.python.org/3/library/subprocess.html
-    languages: [python]
-    severity: ERROR
-
-  - id: system-wildcard-detected
-    patterns:
-      - pattern-either:
-          - pattern-inside: os.system("...")
-          - pattern-inside: os.popen("...")
-          - pattern-inside: os.popen2("...")
-          - pattern-inside: os.popen3("...")
-          - pattern-inside: os.popen4("...")
-          - pattern-inside: subprocess.$W(..., shell=True, ...)
-      - pattern-regex: (tar|chmod|chown|rsync)(.*?)\*
-    message: |
-      Detected use of the wildcard character in a system call that spawns a shell.
-      This subjects the wildcard to normal shell expansion, which can have unintended consequences
-      if there exist any non-standard file names. Consider a file named '-e sh script.sh' -- this
-      will execute a script when 'rsync' is called. See
-      https://www.defensecode.com/public/DefenseCode_Unix_WildCards_Gone_Wild.txt
-      for more information.
-    metadata:
-      cwe: "CWE-155: Improper Neutralization of Wildcards or Matching Symbols"
-      owasp: "A1: Injection"
-      source-url-open: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/injection_wildcard.py
-      references:
-        - https://www.defensecode.com/public/DefenseCode_Unix_WildCards_Gone_Wild.txt
-    languages: [python]
-    severity: WARNING
-
-  - id: telnetlib
-    pattern: telnetlib.$ANYTHING(...)
-    message: |
-      Telnet does not encrypt communications. Use SSH instead.
-    metadata:
-      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L208
-      cwe: "CWE-319: Cleartext Transmission of Sensitive Information"
-      owasp: "A3: Sensitive Data Exposure"
-      bandit-code: B312
-      references:
-        - https://docs.python.org/3/library/telnetlib.html
-    severity: WARNING
-    languages:
-      - python
-
-  - id: weak-ssl-version
-    patterns:
-      - pattern-either:
-          - pattern: ssl.PROTOCOL_SSLv2
-          - pattern: ssl.PROTOCOL_SSLv3
-          - pattern: ssl.PROTOCOL_TLSv1
-          - pattern: ssl.PROTOCOL_TLSv1_1
-          - pattern: pyOpenSSL.SSL.SSLv2_METHOD
-          - pattern: pyOpenSSL.SSL.SSLv23_METHOD
-          - pattern: pyOpenSSL.SSL.SSLv3_METHOD
-          - pattern: pyOpenSSL.SSL.TLSv1_METHOD
-          - pattern: pyOpenSSL.SSL.TLSv1_1_METHOD
-    message: |
-      An insecure SSL version was detected. TLS versions 1.0, 1.1, and all SSL versions
-      are considered weak encryption and are deprecated.
-      Use 'ssl.PROTOCOL_TLSv1_2' or higher.
-    metadata:
-      cwe: "CWE-326: Inadequate Encryption Strength"
-      owasp: "A3: Sensitive Data Exposure"
-      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/insecure_ssl_tls.py#L30
-      references:
-        - https://tools.ietf.org/html/rfc7568
-        - https://tools.ietf.org/id/draft-ietf-tls-oldversions-deprecate-02.html
-        - https://docs.python.org/3/library/ssl.html#ssl.PROTOCOL_TLSv1_2
-    languages: [python]
-    severity: WARNING
-
-  - id: avoid-pyyaml-load
-    metadata:
-      owasp: "A8: Insecure Deserialization"
-      cwe: "CWE-502: Deserialization of Untrusted Data"
-      references:
-        - https://github.com/yaml/pyyaml/wiki/PyYAML-yaml.load(input)-Deprecation
-        - https://nvd.nist.gov/vuln/detail/CVE-2017-18342
-    languages:
-      - python
-    message: |
-      Avoid using `load()`. `PyYAML.load` can create arbitrary Python
-      objects. A malicious actor could exploit this to run arbitrary
-      code. Use `safe_load()` instead.
-    fix: yaml.safe_load($FOO)
-    severity: ERROR
-    patterns:
-      - pattern-inside: |
-          import yaml
-          ...
-          yaml.load($FOO)
-      - pattern: yaml.load($FOO)
-
-  - id: avoid-unsafe-ruamel
-    metadata:
-      owasp: "A8: Insecure Deserialization"
-      cwe: "CWE-502: Deserialization of Untrusted Data"
-      references:
-        - https://yaml.readthedocs.io/en/latest/basicuse.html?highlight=typ
-    languages:
-      - python
-    message: |
-      Avoid using unsafe `ruamel.yaml.YAML()`. `ruamel.yaml.YAML` can
-      create arbitrary Python objects. A malicious actor could exploit
-      this to run arbitrary code. Use `YAML(typ='rt')` or
-      `YAML(typ='safe')` instead.
-    severity: ERROR
-    pattern-either:
-      - pattern: ruamel.yaml.YAML(..., typ='unsafe', ...)
-      - pattern: ruamel.yaml.YAML(..., typ='base', ...)
-
-  - id: avoid-pickle
-    metadata:
-      owasp: "A8: Insecure Deserialization"
-      cwe: "CWE-502: Deserialization of Untrusted Data"
-      references:
-        - https://docs.python.org/3/library/pickle.html
-        - https://davidhamann.de/2020/04/05/exploiting-python-pickle/
-    languages:
-      - python
-    message: |
-      Avoid using `pickle`, which is known to lead to code execution vulnerabilities.
-      When unpickling, the serialized data could be manipulated to run arbitrary code.
-      Instead, consider serializing the relevant data as JSON or a similar text-based
-      serialization format.
-    severity: WARNING
-    pattern-either:
-      - pattern: pickle.$FUNC(...)
-      - pattern: _pickle.$FUNC(...)
-  - id: avoid-cPickle
-    metadata:
-      owasp: "A8: Insecure Deserialization"
-      cwe: "CWE-502: Deserialization of Untrusted Data"
-      references:
-        - https://docs.python.org/3/library/pickle.html
-    languages:
-      - python
-    message: |
-      Avoid using `cPickle`, which is known to lead to code execution vulnerabilities.
-      When unpickling, the serialized data could be manipulated to run arbitrary code.
-      Instead, consider serializing the relevant data as JSON or a similar text-based
-      serialization format.
-    severity: WARNING
-    pattern: cPickle.$FUNC(...)
-  - id: avoid-dill
-    metadata:
-      owasp: "A8: Insecure Deserialization"
-      cwe: "CWE-502: Deserialization of Untrusted Data"
-      references:
-        - https://docs.python.org/3/library/pickle.html
-    languages:
-      - python
-    message: |
-      Avoid using `dill`, which uses `pickle`, which is known to lead to code execution vulnerabilities.
-      When unpickling, the serialized data could be manipulated to run arbitrary code.
-      Instead, consider serializing the relevant data as JSON or a similar text-based
-      serialization format.
-    severity: WARNING
-    pattern-either:
-      - pattern: dill.$FUNC(...)
-  - id: avoid-shelve
-    metadata:
-      owasp: "A8: Insecure Deserialization"
-      cwe: "CWE-502: Deserialization of Untrusted Data"
-      references:
-        - https://docs.python.org/3/library/pickle.html
-    languages:
-      - python
-    message: |
-      Avoid using `shelve`, which uses `pickle`, which is known to lead to code execution vulnerabilities.
-      When unpickling, the serialized data could be manipulated to run arbitrary code.
-      Instead, consider serializing the relevant data as JSON or a similar text-based
-      serialization format.
-    severity: WARNING
-    pattern-either:
-      - pattern: shelve.$FUNC(...)
-
-  - id: hardcoded-token
-    message: |
-      Hardcoded AWS access token detected. Use environment variables
-      to access tokens (e.g., os.environ.get(...)) or use non version-controlled
-      configuration files.
-    metadata:
-      cwe: "CWE-798: Use of Hard-coded Credentials"
-      owasp: "A2: Broken Authentication"
-      source-rule-url: https://pypi.org/project/flake8-boto3/
-      references:
-        - https://bento.dev/checks/boto3/hardcoded-access-token/
-        - https://aws.amazon.com/blogs/security/what-to-do-if-you-inadvertently-expose-an-aws-access-key/
-    patterns:
-      - pattern-either:
-          - pattern: $W(..., aws_secret_access_key="=~/^[A-Za-z0-9/+=]+$/", ...)
-          - pattern: $W(..., aws_access_key_id="=~/^AKI/", ...)
-          - pattern: $W(..., aws_session_token="...", ...)
-    languages: [python]
-    severity: WARNING
-
-  - id: insecure-cipher-algorithm-rc4
-    pattern: cryptography.hazmat.primitives.ciphers.algorithms.ARC4(...)
-    message: |
-      Detected RC4 cipher algorithm which is considered insecure. The algorithm has many
-      known vulnerabilities. Use AES instead.
-    metadata:
-      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L94
-      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
-      owasp: "A3: Sensitive Data Exposure"
-      bandit-code: B304
-      references:
-        - https://crypto.stackexchange.com/questions/853/google-is-using-rc4-but-isnt-rc4-considered-unsafe
-        - https://sweet32.info/
-    severity: WARNING
-    languages:
-      - python
-  - id: insecure-cipher-algorithm-blowfish
-    pattern: cryptography.hazmat.primitives.ciphers.algorithms.Blowfish(...)
-    message: |
-      Detected Blowfish cipher algorithm which is considered insecure. The algorithm has many
-      known vulnerabilities. Use AES instead.
-    metadata:
-      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L96
-      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
-      owasp: "A3: Sensitive Data Exposure"
-      bandit-code: B304
-      references:
-        - https://sweet32.info/
-    severity: WARNING
-    languages:
-      - python
-  - id: insecure-cipher-algorithm-idea
-    pattern: cryptography.hazmat.primitives.ciphers.algorithms.IDEA(...)
-    message: |
-      Detected IDEA cipher algorithm which is considered insecure. The algorithm is
-      considered weak and has been deprecated. Use AES instead.
-    metadata:
-      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L98
-      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
-      owasp: "A3: Sensitive Data Exposure"
-      bandit-code: B304
-      references:
-        - https://tools.ietf.org/html/rfc5469
-    severity: WARNING
-    languages:
-      - python
-
-  - id: insecure-cipher-mode-ecb
-    pattern: cryptography.hazmat.primitives.ciphers.modes.ECB(...)
-    message: |
-      Detected ECB cipher mode which is considered insecure. The algorithm can
-      potentially leak information about the plaintext. Use CBC mode instead.
-    metadata:
-      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L101
-      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
-      owasp: "A3: Sensitive Data Exposure"
-      bandit-code: B305
-      references:
-        - https://crypto.stackexchange.com/questions/20941/why-shouldnt-i-use-ecb-encryption
-    severity: WARNING
-    languages:
-      - python
-
-  - id: insecure-hash-algorithm-md5
-    pattern: cryptography.hazmat.primitives.hashes.MD5(...)
-    message: |
-      Detected MD5 hash algorithm which is considered insecure. MD5 is not
-      collision resistant and is therefore not suitable as a cryptographic
-      signature. Use SHA256 or SHA3 instead.
-    metadata:
-      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L59
-      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
-      owasp: "A3: Sensitive Data Exposure"
-      bandit-code: B303
-      references:
-        - https://tools.ietf.org/html/rfc6151
-        - https://crypto.stackexchange.com/questions/44151/how-does-the-flame-malware-take-advantage-of-md5-collision
-        - https://pycryptodome.readthedocs.io/en/latest/src/hash/sha3_256.html
-    severity: WARNING
-    languages:
-      - python
-  - id: insecure-hash-algorithm-sha1
-    pattern: cryptography.hazmat.primitives.hashes.SHA1(...)
-    message: |
-      Detected SHA1 hash algorithm which is considered insecure. SHA1 is not
-      collision resistant and is therefore not suitable as a cryptographic
-      signature. Use SHA256 or SHA3 instead.
-    metadata:
-      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L59
-      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
-      owasp: "A3: Sensitive Data Exposure"
-      bandit-code: B303
-      references:
-        - https://www.schneier.com/blog/archives/2012/10/when_will_we_se.html
-        - https://www.trendmicro.com/vinfo/us/security/news/vulnerabilities-and-exploits/sha-1-collision-signals-the-end-of-the-algorithm-s-viability
-        - http://2012.sharcs.org/slides/stevens.pdf
-        - https://pycryptodome.readthedocs.io/en/latest/src/hash/sha3_256.html
-    severity: WARNING
-    languages:
-      - python
-
-  - id: insufficient-dsa-key-size
-    patterns:
-      - pattern-either:
-          - pattern: cryptography.hazmat.primitives.asymmetric.dsa.generate_private_key(..., key_size=$SIZE, ...)
-          - pattern: cryptography.hazmat.primitives.asymmetric.dsa.generate_private_key($SIZE, ...)
-      - metavariable-comparison:
-          metavariable: $SIZE
-          comparison: $SIZE < 2048
-    message: |
-      Detected an insufficient key size for DSA. NIST recommends
-      a key size of 2048 or higher.
-    metadata:
-      cwe: "CWE-326: Inadequate Encryption Strength"
-      owasp: "A3: Sensitive Data Exposure"
-      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/weak_cryptographic_key.py
-      references:
-        - https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-57Pt3r1.pdf
-    languages: [python]
-    severity: WARNING
-
-  - id: insufficient-ec-key-size
-    patterns:
-      - pattern-inside: cryptography.hazmat.primitives.asymmetric.ec.generate_private_key(...)
-      - pattern-either:
-          - pattern: cryptography.hazmat.primitives.asymmetric.ec.SECP192R1
-          - pattern: cryptography.hazmat.primitives.asymmetric.ec.SECT163K1
-          - pattern: cryptography.hazmat.primitives.asymmetric.ec.SECT163R2
-    message: |
-      Detected an insufficient curve size for EC. NIST recommends
-      a key size of 224 or higher. For example, use 'ec.SECP256R1'.
-    metadata:
-      cwe: "CWE-326: Inadequate Encryption Strength"
-      owasp: "A3: Sensitive Data Exposure"
-      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/weak_cryptographic_key.py
-      references:
-        - https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-57Pt3r1.pdf
-        - https://cryptography.io/en/latest/hazmat/primitives/asymmetric/ec/#elliptic-curves
-    languages: [python]
-    severity: WARNING
-
-  - id: insufficient-rsa-key-size
-    patterns:
-      - pattern-either:
-          - pattern: cryptography.hazmat.primitives.asymmetric.rsa.generate_private_key(..., key_size=$SIZE, ...)
-          - pattern: cryptography.hazmat.primitives.asymmetric.rsa.generate_private_key($EXP, $SIZE, ...)
-      - metavariable-comparison:
-          metavariable: $SIZE
-          comparison: $SIZE < 2048
-    message: |
-      Detected an insufficient key size for RSA. NIST recommends
-      a key size of 2048 or higher.
-    metadata:
-      cwe: "CWE-326: Inadequate Encryption Strength"
-      owasp: "A3: Sensitive Data Exposure"
-      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/weak_cryptographic_key.py
-      references:
-        - https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-57Pt3r1.pdf
-    languages: [python]
-    severity: WARNING
-
-  - id: dangerous-template-string
-    patterns:
-      - pattern-either:
-          - pattern: |
-              $V = "...".format(...)
-              ...
-              flask.render_template_string($V, ...)
-          - pattern: |
-              $V = "...".format(...)
-              ...
-              return flask.render_template_string($V, ...), $MORE
-          - pattern: |
-              $V = "..." % $S
-              ...
-              flask.render_template_string($V, ...)
-          - pattern: |
-              $V = "..." % $S
-              ...
-              return flask.render_template_string($V, ...), $MORE
-          - pattern: |
-              $V = "..."
-              ...
-              $V += $O
-              ...
-              flask.render_template_string($V, ...)
-          - pattern: |
-              $V = "..."
-              ...
-              $V += $O
-              ...
-              return flask.render_template_string($V, ...), $MORE
-          - pattern: |
-              $V = f"...{$X}..."
-              ...
-              flask.render_template_string($V, ...)
-          - pattern: |
-              $V = f"...{$X}..."
-              ...
-              return flask.render_template_string($V, ...), $CODE
-    message: |
-      Found a template created with string formatting.
-      This is susceptible to server-side template injection
-      and cross-site scripting attacks.
-    metadata:
-      cwe: "CWE-96: Improper Neutralization of Directives in Statically Saved Code ('Static Code Injection')"
-      owasp: "A1: Injection"
-      references:
-        - https://nvisium.com/blog/2016/03/09/exploring-ssti-in-flask-jinja2.html
-        - https://pequalsnp-team.github.io/cheatsheet/flask-jinja2-ssti
-    languages: [python]
-    severity: ERROR
-
-  - id: insecure-deserialization
-    metadata:
-      owasp: "A8: Insecure Deserialization"
-      cwe: "CWE-502: Deserialization of Untrusted Data"
-      references:
-        - https://docs.python.org/3/library/pickle.html
-    message: |
-      Detected the use of an insecure deserizliation library in a Flask route. These libraries
-      are prone to code execution vulnerabilities. Ensure user data does not enter this function.
-      To fix this, try to avoid serializing whole objects. Consider instead using a serializer
-      such as JSON.
-    languages:
-      - python
-    severity: ERROR
-    patterns:
-      - pattern-inside: |
-          @app.route(...)
-          def $X(...):
-            ...
-      - pattern-not: $MODULE.$FUNC("...")
-      - pattern-not: $MODULE.$FUNC(open("...", ...))
-      - pattern-either:
-          - pattern: pickle.$FUNC(...)
-          - pattern: _pickle.$FUNC(...)
-          - pattern: cPickle.$FUNC(...)
-          - pattern: dill.$FUNC(...)
-          - pattern: shelve.$FUNC(...)
-          - pattern: yaml.load(...)
-
-  - id: open-redirect
-    patterns:
-      - pattern-inside: |
-          @$APP.route(...)
-          def $X():
-            ...
-      - pattern-not-inside: |
-          ...
-          if <... werkzeug.urls.url_parse($V) ...>:
-            ...
-      - pattern-either:
-          - pattern: flask.redirect(<... flask.request.$W.get(...) ...>, ...)
-          - pattern: flask.redirect(<... flask.request.$W[...] ...>, ...)
-          - pattern: flask.redirect(<... flask.request.$W(...) ...>, ...)
-          - pattern: flask.redirect(<... flask.request.$W ...>, ...)
-          - pattern: |
-              $V = flask.request.$W.get(...)
-              ...
-              flask.redirect(<... $V ...>, ...)
-          - pattern: |
-              $V = flask.request.$W[...]
-              ...
-              flask.redirect(<... $V ...>, ...)
-          - pattern: |
-              $V = flask.request.$W(...)
-              ...
-              flask.redirect(<... $V ...>, ...)
-          - pattern: |
-              $V = flask.request.$W
-              ...
-              flask.redirect(<... $V ...>, ...)
-    message: |
-      Data from request is passed to redirect().
-      This is an open redirect and could be exploited.
-      Consider using 'url_for()' to generate links to known locations.
-      If you must use a URL to unknown pages, consider using 'urlparse()'
-      or similar and checking if the 'netloc' property is the same as
-      your site's host name. See the references for more information.
-    metadata:
-      cwe: "CWE-601: URL Redirection to Untrusted Site ('Open Redirect')"
-      owasp: "A1: Injection"
-      references:
-        - https://flask-login.readthedocs.io/en/latest/#login-example
-        - https://cheatsheetseries.owasp.org/cheatsheets/Unvalidated_Redirects_and_Forwards_Cheat_Sheet.html#dangerous-url-redirect-example-1
-        - https://docs.python.org/3/library/urllib.parse.html#url-parsing
-    languages: [python]
-    severity: ERROR
-  # For Flask app to serve file securely, it should use `send_from_directory` method
-  # The other methods like `send_file` or `send_static_file` are not recommended per
-  # https://stackoverflow.com/questions/20646822/how-to-serve-static-files-in-flask
-
-  - id: avoid_send_file_without_path_sanitization
-    patterns:
-      - pattern-inside: |
-          @app.route(...)
-          def $X(filename):
-            ...
-      - pattern-either:
-          - pattern: flask.send_file(filename, ...)
-    message:
-      Looks like `filename` could flow to `flask.send_file()` function. Make sure to properly sanitize filename or use
-      `flask.send_from_directory`
-    metadata:
-      cwe: "CWE-73: External Control of File Name or Path"
-      owasp: "A1: Injection"
-    languages: [python]
-    severity: WARNING
-
-  - id: unescaped-template-extension
-    message: |
-      Flask does not automatically escape Jinja templates unless they have
-      .html, .htm, .xml, or .xhtml extensions. This could lead to XSS attacks.
-      Use .html, .htm, .xml, or .xhtml for your template extensions.
-      See https://flask.palletsprojects.com/en/1.1.x/templating/#jinja-setup
-      for more information.
-    metadata:
-      cwe: "CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')"
-      owasp: "A7: Cross-Site Scripting (XSS)"
-      source-rule-url: https://pypi.org/project/flake8-flask/
-      references:
-        - https://flask.palletsprojects.com/en/1.1.x/templating/#jinja-setup
-        - https://blog.r2c.dev/2020/bento-check-unescaped-template-extensions-in-flask/
-        - https://bento.dev/checks/flask/unescaped-file-extension/
-    patterns:
-      - pattern-not: flask.render_template("=~/.+\.html$/", ...)
-      - pattern-not: flask.render_template("=~/.+\.xml$/", ...)
-      - pattern-not: flask.render_template("=~/.+\.htm$/", ...)
-      - pattern-not: flask.render_template("=~/.+\.xhtml$/", ...)
-      - pattern-not: flask.render_template($X + "=~/\.html$/", ...)
-      - pattern-not: flask.render_template($X + "=~/\.xml$/", ...)
-      - pattern-not: flask.render_template($X + "=~/\.htm$/", ...)
-      - pattern-not: flask.render_template($X + "=~/\.xhtml$/", ...)
-      - pattern-not: flask.render_template("=~/.+\.html$/" % $X, ...)
-      - pattern-not: flask.render_template("=~/.+\.xml$/" % $X, ...)
-      - pattern-not: flask.render_template("=~/.+\.htm$/" % $X, ...)
-      - pattern-not: flask.render_template("=~/.+\.xhtml$/" % $X, ...)
-      - pattern-not: flask.render_template("=~/.+\.html$/".format(...), ...)
-      - pattern-not: flask.render_template("=~/.+\.xml$/".format(...), ...)
-      - pattern-not: flask.render_template("=~/.+\.htm$/".format(...), ...)
-      - pattern-not: flask.render_template("=~/.+\.xhtml$/".format(...), ...)
-      - pattern-not: flask.render_template($TEMPLATE)
-      - pattern-either:
-          - pattern: flask.render_template("...", ...)
-          - pattern: flask.render_template($X + "...", ...)
-          - pattern: flask.render_template("..." % $Y, ...)
-          - pattern: flask.render_template("...".format(...), ...)
-    languages: [python]
-    severity: WARNING
-
-  - id: response-contains-unsanitized-input
-    patterns:
-      - pattern-either:
-          - pattern: |
-              $X = flask.request.args.get(...)
-              ...
-              flask.make_response("...".format($X))
-          - pattern: |
-              $X = flask.request.args.get(...)
-              ...
-              flask.make_response(f"...{$X}...")
-          - pattern: |
-              $X = flask.request.args.get(...)
-              ...
-              flask.make_response(f"...{$X}")
-          - pattern: |
-              $X = flask.request.args.get(...)
-              ...
-              flask.make_response(f"{$X}...")
-    message: |
-      Flask response reflects unsanitized user input. This could lead to a
-      cross-site scripting vulnerability (https://owasp.org/www-community/attacks/xss/)
-      in which an attacker causes arbitrary code to be executed in the user's browser.
-      To prevent, please sanitize the user input, e.g. by rendering the response
-      in a Jinja2 template (see considerations in https://flask.palletsprojects.com/en/1.0.x/security/).
-    metadata:
-      cwe: "CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')"
-      owasp: "A7: Cross-Site Scripting (XSS)"
-      references:
-        - https://flask.palletsprojects.com/en/1.0.x/security/
-        - https://owasp.org/www-community/attacks/xss/
-    languages: [python]
-    severity: WARNING
-
-  - id: jwt-python-exposed-credentials
-    languages:
-      - python
-    metadata:
-      cwe: "CWE-522: Insufficiently Protected Credentials"
-      owasp: "A2: Broken Authentication"
-      source-rule-url: https://r2c.dev/blog/2020/hardcoded-secrets-unverified-tokens-and-other-common-jwt-mistakes/
-      references:
-        - https://cwe.mitre.org/data/definitions/522.html
-    message: |
-      Password is exposed through JWT token payload. This is not encrypted and
-      the password could be compromised. Do not store passwords in JWT tokens.
-    pattern-either:
-      - pattern: |
-          jwt.encode({...,"password":$P,...},...)
-      - pattern: |
-          $PAYLOAD = {...,"password":$P,...}
-          ...
-          jwt.encode($PAYLOAD,...)
-    severity: ERROR
-
-  - id: jwt-python-hardcoded-secret
-    message: |
-      Hardcoded JWT secret or private key is used.
-      This is a Insufficiently Protected Credentials weakness: https://cwe.mitre.org/data/definitions/522.html
-      Consider using an appropriate security mechanism to protect the credentials (e.g. keeping secrets in environment variables)
-    metadata:
-      cwe: "CWE-522: Insufficiently Protected Credentials"
-      owasp: "A2: Broken Authentication"
-      source-rule-url: https://r2c.dev/blog/2020/hardcoded-secrets-unverified-tokens-and-other-common-jwt-mistakes/
-    pattern-either:
-      - pattern: |
-          jwt.encode($X, "...", ...)
-      - pattern: |
-          $SECRET = "..."
-          ...
-          jwt.encode($X, $SECRET, ...)
-    languages: [python]
-    severity: ERROR
-
-  - id: jwt-python-none-alg
-    message: |
-      Detected use of the 'none' algorithm in a JWT token.
-      The 'none' algorithm assumes the integrity of the token has already
-      been verified. This would allow a malicious actor to forge a JWT token
-      that will automatically be verified. Do not explicitly use the 'none'
-      algorithm. Instead, use an algorithm such as 'HS256'.
-    metadata:
-      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
-      owasp: "A2: Broken Authentication"
-      source-rule-url: https://r2c.dev/blog/2020/hardcoded-secrets-unverified-tokens-and-other-common-jwt-mistakes/
-    languages: [python]
-    severity: ERROR
-    pattern-either:
-      - pattern: |
-          jwt.encode(...,algorithm="none",...)
-      - pattern: |-
-          jwt.decode(...,algorithms=[...,"none",...],...)
-
-  - id: unverified-jwt-decode
-    pattern: |
-      jwt.decode(..., verify=False, ...)
-    message: |
-      Detected JWT token decoded with 'verify=False'. This bypasses any integrity
-      checks for the token which means the token could be tampered with by
-      malicious actors. Ensure that the JWT token is verified.
-    metadata:
-      owasp: "A5: Broken Authentication"
-      cwe: "CWE-287: Improper Authentication"
-      references:
-        - https://github.com/we45/Vulnerable-Flask-App/blob/752ee16087c0bfb79073f68802d907569a1f0df7/app/app.py#L96
-    fix-regex:
-      regex: (verify\s*=\s*)False
-      replacement: \1True
-    severity: ERROR
-    languages:
-      - python
-
-  - id: insecure-hash-algorithm-md5
-    pattern: hashlib.md5(...)
-    message: |
-      Detected MD5 hash algorithm which is considered insecure. MD5 is not
-      collision resistant and is therefore not suitable as a cryptographic
-      signature. Use SHA256 or SHA3 instead.
-    metadata:
-      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L59
-      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
-      owasp: "A3: Sensitive Data Exposure"
-      bandit-code: B303
-      references:
-        - https://tools.ietf.org/html/rfc6151
-        - https://crypto.stackexchange.com/questions/44151/how-does-the-flame-malware-take-advantage-of-md5-collision
-        - https://pycryptodome.readthedocs.io/en/latest/src/hash/sha3_256.html
-    severity: WARNING
-    languages:
-      - python
-  - id: insecure-hash-algorithm-sha1
-    pattern: hashlib.sha1(...)
-    message: |
-      Detected SHA1 hash algorithm which is considered insecure. SHA1 is not
-      collision resistant and is therefore not suitable as a cryptographic
-      signature. Use SHA256 or SHA3 instead.
-    metadata:
-      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L59
-      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
-      owasp: "A3: Sensitive Data Exposure"
-      bandit-code: B303
-      references:
-        - https://www.schneier.com/blog/archives/2012/10/when_will_we_se.html
-        - https://www.trendmicro.com/vinfo/us/security/news/vulnerabilities-and-exploits/sha-1-collision-signals-the-end-of-the-algorithm-s-viability
-        - http://2012.sharcs.org/slides/stevens.pdf
-        - https://pycryptodome.readthedocs.io/en/latest/src/hash/sha3_256.html
-    severity: WARNING
-    languages:
-      - python
-
-  - id: insecure-hash-function
-    patterns:
-      - pattern-either:
-          - pattern: hashlib.new("=~/[M|m][D|d][4|5]/", ...)
-          - pattern: hashlib.new(..., name="=~/[M|m][D|d][4|5]/", ...)
-    message: |
-      Detected use of an insecure MD4 or MD5 hash function.
-      These functions have known vulnerabilities and are considered deprecated.
-      Consider using 'SHA256' or a similar function instead.
-    metadata:
-      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
-      owasp: "A3: Sensitive Data Exposure"
-      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/hashlib_new_insecure_functions.py
-      references:
-        - https://tools.ietf.org/html/rfc6151
-        - https://crypto.stackexchange.com/questions/44151/how-does-the-flame-malware-take-advantage-of-md5-collision
-        - https://pycryptodome.readthedocs.io/en/latest/src/hash/sha3_256.html
-    languages: [python]
-    severity: WARNING
-
-  - id: unquoted-csv-writer
-    patterns:
-      - pattern-not: csv.writer(..., quoting=csv.QUOTE_ALL, ...)
-      - pattern: csv.writer(...)
-    message: Found an unquoted CSV writer. This is susceptible to injection. Use 'quoting=csv.QUOTE_ALL'.
-    metadata:
-      cwe: "CWE-1236: Improper Neutralization of Formula Elements in a CSV File"
-      owasp: "A1: Injection"
-      references:
-        - https://affinity-it-security.com/how-to-prevent-csv-injection/
-    fix-regex:
-      regex: (.*)\)
-      replacement: \1, quoting=csv.QUOTE_ALL)
-    languages: [python]
-    severity: ERROR
-
-  - id: unverified-ssl-context
-    pattern: ssl._create_unverified_context(...)
-    message: |
-      Unverified SSL context detected. This will permit insecure connections without verifying
-      SSL certificates. Use 'ssl.create_default_context()' instead.
-    metadata:
-      owasp: "A6: Security Misconfiguration"
-      cwe: "CWE-295: Improper Certificate Validation"
-      references:
-        - https://docs.python.org/3/library/ssl.html#ssl-security
-        - https://docs.python.org/3/library/http.client.html#http.client.HTTPSConnection
-    severity: ERROR
-    languages:
-      - python
-
-  - id: use-defused-xml
-    pattern-either:
-      - pattern: import xml
-    fix-regex:
-      regex: xml
-      replacement: defusedxml
-    metadata:
-      owasp: "A4: XML External Entities (XXE)"
-      cwe: "CWE-611: Improper Restriction of XML External Entity Reference"
-      references:
-        - https://docs.python.org/3/library/xml.html
-        - https://github.com/tiran/defusedxml
-    message: |
-      Found use of the native Python XML libraries, which is vulnerable to XML external entity (XXE)
-      attacks. The Python documentation recommends the 'defusedxml' library instead. Use 'defusedxml'.
-      See https://github.com/tiran/defusedxml for more information.
-    languages: [python]
-    severity: ERROR
-
-  - id: use-defused-xmlrpc
-    pattern-either:
-      - pattern: import xmlrpclib
-      - pattern: import SimpleXMLRPCServer
-      # Python 3
-      - pattern: import xmlrpc
-    message: |
-      Detected use of xmlrpc. xmlrpc is not inherently safe from vulnerabilities.
-      Use defusedxml.xmlrpc instead.
-    metadata:
-      cwe: "CWE-776: Improper Restriction of Recursive Entity References in DTDs ('XML Entity Expansion')"
-      owasp: "A4: XML External Entities (XXE)"
-      source-rule-url: https://github.com/PyCQA/bandit/blob/07f84cb5f5e7c1055e6feaa0fe93afa471de0ac3/bandit/blacklists/imports.py#L160
-      references:
-        - https://pypi.org/project/defusedxml/
-        - https://docs.python.org/3/library/xml.html#xml-vulnerabilities
-    severity: ERROR
-    languages:
-      - python
-
-  - id: insecure-cipher-algorithm-rc2
-    patterns:
-      - pattern-either:
-          - pattern: Cryptodome.Cipher.ARC2.new(...)
-          - pattern: Crypto.Cipher.ARC2.new
-    message: |
-      Detected RC2 cipher algorithm which is considered insecure. The algorithm has known vulnerabilities and is difficult to use securely. Use AES instead.
-    metadata:
-      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L84
-      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
-      owasp: "A3: Sensitive Data Exposure"
-      bandit-code: B304
-      references:
-        - https://security.stackexchange.com/questions/93924/is-rc2-cbc-at-all-secure
-        - https://sweet32.info/
-    severity: WARNING
-    languages:
-      - python
-  - id: insecure-cipher-algorithm-rc4
-    patterns:
-      - pattern-either:
-          - pattern: Cryptodome.Cipher.ARC4.new(...)
-          - pattern: Crypto.Cipher.ARC4.new(...)
-    message: |
-      Detected RC4 cipher algorithm which is considered insecure. The algorithm has many
-      known vulnerabilities. Use AES instead.
-    metadata:
-      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L84
-      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
-      owasp: "A3: Sensitive Data Exposure"
-      bandit-code: B304
-      references:
-        - https://crypto.stackexchange.com/questions/853/google-is-using-rc4-but-isnt-rc4-considered-unsafe
-        - https://sweet32.info/
-    severity: WARNING
-    languages:
-      - python
-  - id: insecure-cipher-algorithm-blowfish
-    patterns:
-      - pattern-either:
-          - pattern: Cryptodome.Cipher.Blowfish.new(...)
-          - pattern: Crypto.Cipher.Blowfish.new(...)
-    message: |
-      Detected Blowfish cipher algorithm which is considered insecure. The algorithm has many
-      known vulnerabilities. Use AES instead.
-    metadata:
-      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L84
-      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
-      owasp: "A3: Sensitive Data Exposure"
-      bandit-code: B304
-      references:
-        - https://sweet32.info/
-    severity: WARNING
-    languages:
-      - python
-  - id: insecure-cipher-algorithm-des
-    patterns:
-      - pattern-either:
-          - pattern: Cryptodome.Cipher.DES.new(...)
-          - pattern: Crypto.Cipher.DES.new(...)
-    message: |
-      Detected DES cipher algorithm which is considered insecure. The algorithm is
-      considered weak and has been deprecated. Use AES instead.
-    metadata:
-      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L84
-      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
-      owasp: "A3: Sensitive Data Exposure"
-      bandit-code: B304
-      references:
-        - https://tools.ietf.org/html/rfc5469
-    severity: WARNING
-    languages:
-      - python
-  - id: insecure-cipher-algorithm-xor
-    patterns:
-      - pattern-either:
-          - pattern: Cryptodome.Cipher.XOR.new(...)
-          - pattern: Crypto.Cipher.XOR.new(...)
-    message: |
-      Detected XOR cipher algorithm which is considered insecure. This algorithm
-      is not cryptographically secure and can be reversed easily. Use AES instead.
-    metadata:
-      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L84
-      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
-      owasp: "A3: Sensitive Data Exposure"
-      bandit-code: B304
-      references:
-        - https://stackoverflow.com/questions/1135186/whats-wrong-with-xor-encryption
-    severity: WARNING
-    languages:
-      - python
-
-  - id: insecure-hash-algorithm-md2
-    patterns:
-      - pattern-either:
-          - pattern: Crypto.Hash.MD2.new(...)
-          - pattern: Cryptodome.Hash.MD2.new (...)
-    message: |
-      Detected MD2 hash algorithm which is considered insecure. This algorithm
-      has many known vulnerabilities and has been deprecated. Use SHA256 or SHA3 instead.
-    metadata:
-      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L59
-      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
-      owasp: "A3: Sensitive Data Exposure"
-      references:
-        - https://tools.ietf.org/html/rfc6149
-        - https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2009-2409
-        - https://pycryptodome.readthedocs.io/en/latest/src/hash/sha3_256.html
-    severity: WARNING
-    languages:
-      - python
-  - id: insecure-hash-algorithm-md4
-    patterns:
-      - pattern-either:
-          - pattern: Crypto.Hash.MD4.new(...)
-          - pattern: Cryptodome.Hash.MD4.new (...)
-    message: |
-      Detected MD4 hash algorithm which is considered insecure. This algorithm
-      has many known vulnerabilities and has been deprecated. Use SHA256 or SHA3 instead.
-    metadata:
-      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L59
-      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
-      owasp: "A3: Sensitive Data Exposure"
-      references:
-        - https://tools.ietf.org/html/rfc6150
-        - https://pycryptodome.readthedocs.io/en/latest/src/hash/sha3_256.html
-    severity: WARNING
-    languages:
-      - python
-  - id: insecure-hash-algorithm-md5
-    patterns:
-      - pattern-either:
-          - pattern: Crypto.Hash.MD5.new(...)
-          - pattern: Cryptodome.Hash.MD5.new (...)
-    message: |
-      Detected MD5 hash algorithm which is considered insecure. MD5 is not
-      collision resistant and is therefore not suitable as a cryptographic
-      signature. Use SHA256 or SHA3 instead.
-    metadata:
-      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L59
-      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
-      owasp: "A3: Sensitive Data Exposure"
-      references:
-        - https://tools.ietf.org/html/rfc6151
-        - https://crypto.stackexchange.com/questions/44151/how-does-the-flame-malware-take-advantage-of-md5-collision
-        - https://pycryptodome.readthedocs.io/en/latest/src/hash/sha3_256.html
-    severity: WARNING
-    languages:
-      - python
-  - id: insecure-hash-algorithm-sha1
-    patterns:
-      - pattern-either:
-          - pattern: Crypto.Hash.SHA.new(...)
-          - pattern: Cryptodome.Hash.SHA.new (...)
-    message: |
-      Detected SHA1 hash algorithm which is considered insecure. SHA1 is not
-      collision resistant and is therefore not suitable as a cryptographic
-      signature. Use SHA256 or SHA3 instead.
-    metadata:
-      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L59
-      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
-      owasp: "A3: Sensitive Data Exposure"
-      references:
-        - https://www.schneier.com/blog/archives/2012/10/when_will_we_se.html
-        - https://www.trendmicro.com/vinfo/us/security/news/vulnerabilities-and-exploits/sha-1-collision-signals-the-end-of-the-algorithm-s-viability
-        - http://2012.sharcs.org/slides/stevens.pdf
-        - https://pycryptodome.readthedocs.io/en/latest/src/hash/sha3_256.html
-    severity: WARNING
-    languages:
-      - python
-
-  - id: insufficient-dsa-key-size
-    patterns:
-      - pattern-either:
-          - pattern: Crypto.PublicKey.DSA.generate(..., bits=$SIZE, ...)
-          - pattern: Crypto.PublicKey.DSA.generate($SIZE, ...)
-          - pattern: Cryptodome.PublicKey.DSA.generate(..., bits=$SIZE, ...)
-          - pattern: Cryptodome.PublicKey.DSA.generate($SIZE, ...)
-      - metavariable-comparison:
-          metavariable: $SIZE
-          comparison: $SIZE < 2048
-    message: |
-      Detected an insufficient key size for DSA. NIST recommends
-      a key size of 2048 or higher.
-    metadata:
-      cwe: "CWE-326: Inadequate Encryption Strength"
-      owasp: "A3: Sensitive Data Exposure"
-      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/weak_cryptographic_key.py
-      references:
-        - https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-57Pt3r1.pdf
-    languages: [python]
-    severity: WARNING
-
-  - id: insufficient-rsa-key-size
-    patterns:
-      - pattern-either:
-          - pattern: Crypto.PublicKey.RSA.generate(..., bits=$SIZE, ...)
-          - pattern: Crypto.PublicKey.RSA.generate($SIZE, ...)
-          - pattern: Cryptodome.PublicKey.RSA.generate(..., bits=$SIZE, ...)
-          - pattern: Cryptodome.PublicKey.RSA.generate($SIZE, ...)
-      - metavariable-comparison:
-          metavariable: $SIZE
-          comparison: $SIZE < 2048
-    message: |
-      Detected an insufficient key size for RSA. NIST recommends
-      a key size of 2048 or higher.
-    metadata:
-      cwe: "CWE-326: Inadequate Encryption Strength"
-      owasp: "A3: Sensitive Data Exposure"
-      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/weak_cryptographic_key.py
-      references:
-        - https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-57Pt3r1.pdf
-    languages: [python]
-    severity: WARNING
-
-  - id: disabled-cert-validation
-    patterns:
-      - pattern-either:
-          - pattern: requests.put(..., verify=False, ...)
-          - pattern: requests.patch(..., verify=False, ...)
-          - pattern: requests.delete(..., verify=False, ...)
-          - pattern: requests.head(..., verify=False, ...)
-          - pattern: requests.options(..., verify=False, ...)
-          - pattern: requests.request(..., verify=False, ...)
-          - pattern: requests.get(..., verify=False, ...)
-          - pattern: requests.post(..., verify=False, ...)
-    message: |
-      Certificate verification has been explicitly disabled. This
-      permits insecure connections to insecure servers. Re-enable
-      certification validation.
-    metadata:
-      cwe: "CWE-295: Improper Certificate Validation"
-      owasp: "A3: Sensitive Data Exposure"
-      references:
-        - https://stackoverflow.com/questions/41740361/is-it-safe-to-disable-ssl-certificate-verification-in-pythonss-requests-lib
-    languages: [python]
-    severity: ERROR
-
-  - id: no-auth-over-http
-    patterns:
-      - pattern-either:
-          - pattern: requests.$W("=~/http:\/\/.*/", ..., auth=$X, ...)
-          - pattern: |
-              $URL = "=~/http:\/\/.../"
-              ...
-              requests.$W($URL, ..., auth=$X, ...)
-    fix-regex:
-      regex: http:\/\/
-      replacement: https://
-      count: 1
-    message: |
-      Authentication detected over HTTP. HTTP does not provide any
-      encryption or protection for these authentication credentials.
-      This may expose these credentials to unauthhorized parties.
-      Use 'https://' instead.
-    metadata:
-      cwe: "CWE-523: Unprotected Transport of Credentials"
-      owasp: "A2: Broken Authentication"
-      source-rule-url: https://pypi.org/project/flake8-flask/
-      references:
-        - https://blog.r2c.dev/2020/bento-check-no-auth-over-http/
-        - https://bento.dev/checks/requests/no-auth-over-http/
-    languages: [python]
-    severity: ERROR
-
-  - id: string-concat
-    languages: [python]
-    severity: WARNING
-    message: |
-      Detected string concatenation or formatting in a call to a command via 'sh'.
-      This could be a command injection vulnerability if the data is user-controlled.
-      Instead, use a list and append the argument.
-    metadata:
-      cwe: "CWE-78: Improper Neutralization of Special Elements used in an OS Command ('OS Command Injection')"
-      owasp: "A1: Injection"
-    pattern-either:
-      - pattern: sh.$BIN($X + $Y)
-      - pattern: sh.$BIN($X.format(...))
-      - pattern: sh.$BIN(f"...{...}...")
-
-  - id: sqlalchemy-sql-injection
-    patterns:
-      - pattern-either:
-          - pattern: |
-              def $FUNC(...,$VAR,...):
-                ...
-                $SESSION.query(...).$SQLFUNC("...".$FORMATFUNC(...,$VAR,...))
-          - pattern: |
-              def $FUNC(...,$VAR,...):
-                ...
-                $SESSION.query.join(...).$SQLFUNC("...".$FORMATFUNC(...,$VAR,...))
-          - pattern: |
-              def $FUNC(...,$VAR,...):
-                ...
-                $SESSION.query.$SQLFUNC("...".$FORMATFUNC(...,$VAR,...))
-          - pattern: |
-              def $FUNC(...,$VAR,...):
-                ...
-                query.$SQLFUNC("...".$FORMATFUNC(...,$VAR,...))
-      - metavariable-regex:
-          metavariable: $SQLFUNC
-          regex: (group_by|order_by|distinct|having|filter)
-      - metavariable-regex:
-          metavariable: $FORMATFUNC
-          regex: (?!bindparams)
-    message: |
-      Distinct, Having, Group_by, Order_by, and Filter in SQLAlchemy can cause sql injections
-      if the developer inputs raw SQL into the before-mentioned clauses.
-      This pattern captures relevant cases in which the developer inputs raw SQL into the distinct, having, group_by, order_by or filter clauses and
-      injects user-input into the raw SQL with any function besides "bindparams". Use bindParams to securely bind user-input
-      to SQL statements.
-    fix-regex:
-      regex: format
-      replacement: bindparams
-    languages:
-      - python
-    severity: WARNING
+rules:
+  - id: formatted-string-bashoperator
+    patterns:
+      - pattern-either:
+          - pattern: |
+              airflow.operators.bash_operator.BashOperator(..., bash_command="..." + $CONCAT, ...)
+          - pattern: |
+              airflow.operators.bash_operator.BashOperator(..., bash_command="...".format(...), ...)
+          - pattern: |
+              airflow.operators.bash_operator.BashOperator(..., bash_command=f"...", ...)
+          - pattern: |
+              airflow.operators.bash_operator.BashOperator(..., bash_command="..." % $PARAMS, ...)
+          - pattern: |
+              $CMD = "..." % $PARAMS
+              ...
+              airflow.operators.bash_operator.BashOperator(..., bash_command=$CMD, ...)
+          - pattern: |
+              $CMD = $STR.format(...)
+              ...
+              airflow.operators.bash_operator.BashOperator(..., bash_command=$CMD, ...)
+          - pattern: |
+              $CMD = f"..."
+              ...
+              airflow.operators.bash_operator.BashOperator(..., bash_command=$CMD, ...)
+          - pattern: |
+              $CMD = "..." + $CONCAT
+              ...
+              airflow.operators.bash_operator.BashOperator(..., bash_command=$CMD, ...)
+          - pattern: |
+              $CMD = "..."
+              ...
+              $CMD += $CONCAT
+              ...
+              airflow.operators.bash_operator.BashOperator(..., bash_command=$CMD, ...)
+    message: |
+      Found a formatted string in BashOperator: $CMD.
+      This could be vulnerable to injection.
+      Be extra sure your variables are not controllable by external sources.
+    metadata:
+      cwe: "CWE-78: Improper Neutralization of Special Elements used in an OS Command ('OS Command Injection')"
+      owasp: "A1: Injection"
+    languages:
+      - python
+    severity: WARNING
+
+  - id: avoid-insecure-deserialization
+    metadata:
+      owasp: "A8: Insecure Deserialization"
+      cwe: "CWE-502: Deserialization of Untrusted Data"
+      references: https://docs.python.org/3/library/pickle.html
+    message:
+      Avoid using insecure deserialization library, backed by `pickle`, `_pickle`, `cpickle`, `dill`, `shelve`, or `yaml`,
+      which are known to lead to remote code execution vulnerabilities.
+    languages:
+      - python
+    severity: ERROR
+    patterns:
+      - pattern-inside: |
+          def $X(..., request, ...):
+            ...
+      - pattern-either:
+          - pattern: |
+              $VAR = <... request.$Y.get(...) ...>
+              ...
+              pickle.$FUNC(<... $VAR ...>)
+          - pattern: pickle.$FUNC(<... request.$Y.get(...) ...>)
+          - pattern: |
+              $VAR = <... request.$Y.get(...) ...>
+              ...
+              _pickle.$FUNC(<... $VAR ...>)
+          - pattern: _pickle.$FUNC(<... request.$Y.get(...) ...>)
+          - pattern: |
+              $VAR = <... request.$Y.get(...) ...>
+              ...
+              cPickle.$FUNC(<... $VAR ...>)
+          - pattern: cPickle.$FUNC(<... request.$Y.get(...) ...>)
+          - pattern: |
+              $VAR = <... request.$Y.get(...) ...>
+              ...
+              dill.$FUNC(<... $VAR ...>)
+          - pattern: dill.$FUNC(<... request.$Y.get(...) ...>)
+          - pattern: |
+              $VAR = <... request.$Y.get(...) ...>
+              ...
+              shelve.$FUNC(<... $VAR ...>)
+          - pattern: shelve.$FUNC(<... request.$Y.get(...) ...>)
+          - pattern: |
+              $VAR = <... request.$Y.get(...) ...>
+              ...
+              yaml.$FUNC(<... $VAR ...>)
+          - pattern: yaml.$FUNC(<... request.$Y.get(...) ...>)
+
+  - id: avoid-mark-safe
+    patterns:
+      - pattern-not-inside: django.utils.html.format_html(...)
+      - pattern-not: django.utils.safestring.mark_safe("...")
+      - pattern: django.utils.safestring.mark_safe(...)
+    message: |
+      'mark_safe()' is used to mark a string as "safe" for HTML output.
+      This disables escaping and could therefore subject the content to
+      XSS attacks. Use 'django.utils.html.format_html()' to build HTML
+      for rendering instead.
+    metadata:
+      cwe: "CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')"
+      owasp: "A7: Cross-Site Scripting (XSS)"
+      references:
+        - https://docs.djangoproject.com/en/3.0/ref/utils/#django.utils.safestring.mark_safe
+        - https://docs.djangoproject.com/en/3.0/ref/utils/#django.utils.html.format_html
+    languages: [python]
+    severity: WARNING
+
+  - id: no-csrf-exempt
+    pattern: |
+      @django.views.decorators.csrf.csrf_exempt
+      def $R(...):
+        ...
+    message: There is rarely a good reason to use @csrf_exempt as is used for `$R`.
+    metadata:
+      cwe: "CWE-352: Cross-Site Request Forgery (CSRF)"
+      owasp: "A6: Security Misconfiguration"
+    languages: [python]
+    severity: WARNING
+
+  - id: custom-expression-as-sql
+    languages:
+      - python
+    message:
+      Detected a Custom Expression ''$EXPRESSION'' calling ''as_sql(...).'' Ensure no user input enters this function
+      because it is susceptible to SQL injection. See https://docs.djangoproject.com/en/3.0/ref/models/expressions/#django.db.models.Func.as_sql
+      for more information.
+    metadata:
+      cwe: "CWE-89: Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection')"
+      owasp: "A1: Injection"
+      references:
+        - https://docs.djangoproject.com/en/3.0/ref/models/expressions/#django.db.models.Func.as_sql
+        - https://blog.r2c.dev/2020/preventing-sql-injection-a-django-authors-perspective/
+    pattern: $EXPRESSION.as_sql(...)
+    severity: WARNING
+
+  - id: extends-custom-expression
+    languages:
+      - python
+    message: |
+      Found extension of custom expression: $CLASS. Extending expressions
+      in this way could inadvertently expose a SQL injection vulnerability.
+      See https://docs.djangoproject.com/en/3.0/ref/models/expressions/#avoiding-sql-injection
+      for more information.
+    metadata:
+      cwe: "CWE-89: Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection')"
+      owasp: "A1: Injection"
+      references:
+        - https://docs.djangoproject.com/en/3.0/ref/models/expressions/#avoiding-sql-injection
+        - https://blog.r2c.dev/2020/preventing-sql-injection-a-django-authors-perspective/
+    patterns:
+      - pattern-either:
+          - pattern: |
+              class $CLASS(..., django.db.models.Func, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.expressions.Func, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.Expression, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.expressions.Expression, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.Value, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.expressions.Value, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.DurationValue, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.expressions.DurationValue, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.RawSQL, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.expressions.RawSQL, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.Star, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.expressions.Star, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.Random, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.expressions.Random, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.Col, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.expressions.Col, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.Ref, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.expressions.Ref, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.ExpressionList, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.expressions.ExpressionList, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.ExpressionWrapper, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.expressions.ExpressionWrapper, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.When, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.expressions.When, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.Case, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.expressions.Case, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.Subquery, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.expressions.Subquery, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.Exists, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.expressions.Exists, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.Window, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.expressions.Window, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.WindowFrame, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.expressions.WindowFrame, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.RowRange, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.expressions.RowRange, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.ValueRange, ...):
+                  ...
+          - pattern: |
+              class $CLASS(..., django.db.models.expressions.ValueRange, ...):
+                  ...
+    severity: WARNING
+
+  - id: avoid-query-set-extra
+    patterns:
+      - pattern-either:
+          - pattern: $X.objects.$FUNC(...).extra(...)
+          - pattern: $X.objects.$FUNC(...).$FILTER(...).extra(...)
+          - pattern: $X.objects.$FUNC(...).$FILTER(...).$UPDATE(...).extra(...)
+    message: This is a last resort. You should be careful when using QuerySet.extra due to SQLi https://docs.djangoproject.com/en/3.0/ref/models/querysets/#django.db.models.query.QuerySet.extra
+    metadata:
+      cwe: "CWE-89: Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection')"
+      owasp: "A1: Injection"
+      references:
+        - https://docs.djangoproject.com/en/3.0/ref/models/querysets/#django.db.models.query.QuerySet.extra
+        - https://blog.r2c.dev/2020/preventing-sql-injection-a-django-authors-perspective/
+    languages: [python]
+    severity: ERROR
+
+  - id: avoid-raw-sql
+    patterns:
+      - pattern-either:
+          - pattern: $MODEL.objects.raw($QUERY, ...)
+          - pattern: django.db.models.expressions.RawSQL(...)
+    message: You should be very careful whenever you write raw SQL. Consider using Django ORM before raw SQL. See https://docs.djangoproject.com/en/3.0/topics/db/sql/#passing-parameters-into-raw
+    metadata:
+      cwe: "CWE-89: Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection')"
+      owasp: "A1: Injection"
+      references:
+        - https://docs.djangoproject.com/en/3.0/ref/models/expressions/#raw-sql-expressions
+        - https://blog.r2c.dev/2020/preventing-sql-injection-a-django-authors-perspective/
+    languages: [python]
+    severity: ERROR
+
+  - id: django-secure-set-cookie
+    patterns:
+      - pattern-either:
+          - pattern-inside: |
+              import django.http.HttpResponse
+              ...
+          - pattern-inside: |
+              import django.shortcuts.render
+              ...
+            # Exclude vendored i18n code
+      - pattern-not-inside: |
+          LANGUAGE_QUERY_PARAMETER = 'language'
+          ...
+          def set_language(request):
+              ...
+          # Exclude vendored contrib/messages/storage/cookie.py
+      - pattern-not-inside: |
+          class CookieStorage(django.contrib.messages.storage.base.BaseStorage):
+              ...
+          # Exclude cookies handled by vendored middleware
+      - pattern-not: response.set_cookie(django.conf.settings.SESSION_COOKIE_NAME, ...)
+      - pattern-not: response.set_cookie(django.conf.settings.CSRF_COOKIE_NAME, ...)
+      - pattern-not: response.set_cookie(django.conf.settings.LANGUAGE_COOKIE_NAME, ...)
+      - pattern-not: response.set_cookie(rest_framework_jwt.settings.api_settings.JWT_AUTH_COOKIE, ...)
+      - pattern-not: response.set_cookie(..., secure=$A, httponly=$B, samesite=$C, ...)
+      - pattern-not: response.set_cookie(..., **$A)
+      - pattern: response.set_cookie(...)
+    message: |
+      Django cookies should be handled securely by setting secure=True, httponly=True, and samesite='Lax' in
+      response.set_cookie(...). If your situation calls for different settings, explicitly disable the setting.
+      If you want to send the cookie over http, set secure=False.  If you want to let client-side JavaScript
+      read the cookie, set httponly=False. If you want to attach cookies to requests for external sites,
+      set samesite=None.
+    metadata:
+      cwe: "CWE-614: Sensitive Cookie in HTTPS Session Without 'Secure' Attribute"
+      owasp: "A3: Sensitive Data Exposure"
+      references:
+        - https://docs.djangoproject.com/en/3.0/ref/request-response/#django.http.HttpResponse.set_cookie
+        - https://blog.r2c.dev/2020/bento-check-keeping-cookies-safe-in-flask/
+        - https://bento.dev/checks/flask/secure-set-cookie/
+    languages: [python]
+    severity: WARNING
+
+  - id: unvalidated-password
+    patterns:
+      - pattern-not-inside: |
+          if <... django.contrib.auth.password_validation.validate_password(...) ...>:
+              ...
+      - pattern-not-inside: |
+          django.contrib.auth.password_validation.validate_password(...)
+          ...
+      - pattern-not-inside: |
+          try:
+            ...
+            django.contrib.auth.password_validation.validate_password(...)
+            ...
+          except $EX:
+            ...
+          ...
+      - pattern-not-inside: |
+          try:
+            ...
+            django.contrib.auth.password_validation.validate_password(...)
+            ...
+          except $EX as $E:
+            ...
+          ...
+      - pattern-not: UserModel().set_password($X)
+      - pattern: $MODEL.set_password($X)
+    fix: |
+      if django.contrib.auth.password_validation.validate_password($X, user=$MODEL):
+          $MODEL.set_password($X)
+    message: |
+      The password on '$MODEL' is being set without validating the password.
+      Call django.contrib.auth.password_validation.validate_password() with
+      validation functions before setting the password. See
+      https://docs.djangoproject.com/en/3.0/topics/auth/passwords/
+      for more information.
+    metadata:
+      cwe: "CWE-521: Weak Password Requirements"
+      owasp: "A2: Broken Authentication"
+      references:
+        - https://docs.djangoproject.com/en/3.0/topics/auth/passwords/#module-django.contrib.auth.password_validation
+    languages: [python]
+    severity: WARNING
+
+  - id: mass-assignment
+    languages: [python]
+    severity: WARNING
+    message: |
+      Mass assignment detected. This can result in assignment to
+      model fields that are unintended and can be exploited by
+      an attacker. Instead of using '**request.$W', assign each field you
+      want to edit individually to prevent mass assignment. You can read
+      more about mass assignment at
+      https://cheatsheetseries.owasp.org/cheatsheets/Mass_Assignment_Cheat_Sheet.html.
+    metadata:
+      cwe: "CWE-915: Improperly Controlled Modification of Dynamically-Determined Object Attributes"
+      owasp: "A1: Injection"
+      owaspapi: "API6: Mass Assignment"
+      references:
+        - https://cheatsheetseries.owasp.org/cheatsheets/Mass_Assignment_Cheat_Sheet.html
+    patterns:
+      - pattern-either:
+          - pattern: $MODEL.objects.create(**request.$W)
+          - pattern: |
+              $OBJ.update(**request.$W)
+              ...
+              $OBJ.save()
+
+  - id: open-redirect
+    message: |
+      Data from request ($DATA) is passed to redirect(). This is an open redirect and could be exploited.
+      Ensure you are redirecting to safe URLs by using django.utils.http.is_safe_url().
+      See https://cwe.mitre.org/data/definitions/601.html for more information.
+    metadata:
+      cwe: "CWE-601: URL Redirection to Untrusted Site ('Open Redirect')"
+      owasp: "A1: Injection"
+      references:
+        - https://www.djm.org.uk/posts/djangos-little-protections-word-redirect-dangers/
+        - https://github.com/django/django/blob/d1b7bd030b1db111e1a3505b1fc029ab964382cc/django/utils/http.py#L231
+    languages: [python]
+    severity: WARNING
+    patterns:
+      - pattern-inside: |
+          def $FUNC(...):
+            ...
+      - pattern-not-inside: |
+          def $FUNC(...):
+            ...
+            django.utils.http.is_safe_url(...)
+            ...
+      - pattern-not-inside: |
+          def $FUNC(...):
+            ...
+            if <... django.utils.http.is_safe_url(...) ...>:
+              ...
+      - pattern-either:
+          - pattern: django.shortcuts.redirect(..., request.$W.get(...), ...)
+          - pattern: django.shortcuts.redirect(..., $S.format(..., request.$W.get(...), ...), ...)
+          - pattern: django.shortcuts.redirect(..., $S % request.$W.get(...), ...)
+          - pattern: django.shortcuts.redirect(..., f"...{request.$W.get(...)}...", ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.shortcuts.redirect(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = $DATA
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.shortcuts.redirect(..., $STR.format(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = $STR.format(..., $DATA, ...)
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.shortcuts.redirect(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.shortcuts.redirect(..., f"...{$DATA}...", ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.shortcuts.redirect(..., $STR + $DATA, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = $STR + $DATA
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: $A = django.shortcuts.redirect(..., request.$W.get(...), ...)
+          - pattern: $A = django.shortcuts.redirect(..., $S.format(..., request.$W.get(...), ...), ...)
+          - pattern: $A = django.shortcuts.redirect(..., $S % request.$W.get(...), ...)
+          - pattern: $A = django.shortcuts.redirect(..., f"...{request.$W.get(...)}...", ...)
+          - pattern: return django.shortcuts.redirect(..., request.$W.get(...), ...)
+          - pattern: return django.shortcuts.redirect(..., $S.format(..., request.$W.get(...), ...), ...)
+          - pattern: return django.shortcuts.redirect(..., $S % request.$W.get(...), ...)
+          - pattern: return django.shortcuts.redirect(..., f"...{request.$W.get(...)}...", ...)
+          - pattern: django.shortcuts.redirect(..., request.$W(...), ...)
+          - pattern: django.shortcuts.redirect(..., $S.format(..., request.$W(...), ...), ...)
+          - pattern: django.shortcuts.redirect(..., $S % request.$W(...), ...)
+          - pattern: django.shortcuts.redirect(..., f"...{request.$W(...)}...", ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.shortcuts.redirect(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = $DATA
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.shortcuts.redirect(..., $STR.format(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = $STR.format(..., $DATA, ...)
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.shortcuts.redirect(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.shortcuts.redirect(..., f"...{$DATA}...", ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.shortcuts.redirect(..., $STR + $DATA, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = $STR + $DATA
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: $A = django.shortcuts.redirect(..., request.$W(...), ...)
+          - pattern: $A = django.shortcuts.redirect(..., $S.format(..., request.$W(...), ...), ...)
+          - pattern: $A = django.shortcuts.redirect(..., $S % request.$W(...), ...)
+          - pattern: $A = django.shortcuts.redirect(..., f"...{request.$W(...)}...", ...)
+          - pattern: return django.shortcuts.redirect(..., request.$W(...), ...)
+          - pattern: return django.shortcuts.redirect(..., $S.format(..., request.$W(...), ...), ...)
+          - pattern: return django.shortcuts.redirect(..., $S % request.$W(...), ...)
+          - pattern: return django.shortcuts.redirect(..., f"...{request.$W(...)}...", ...)
+          - pattern: django.shortcuts.redirect(..., request.$W[...], ...)
+          - pattern: django.shortcuts.redirect(..., $S.format(..., request.$W[...], ...), ...)
+          - pattern: django.shortcuts.redirect(..., $S % request.$W[...], ...)
+          - pattern: django.shortcuts.redirect(..., f"...{request.$W[...]}...", ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.shortcuts.redirect(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = $DATA
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.shortcuts.redirect(..., $STR.format(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = $STR.format(..., $DATA, ...)
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.shortcuts.redirect(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.shortcuts.redirect(..., f"...{$DATA}...", ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.shortcuts.redirect(..., $STR + $DATA, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = $STR + $DATA
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: $A = django.shortcuts.redirect(..., request.$W[...], ...)
+          - pattern: $A = django.shortcuts.redirect(..., $S.format(..., request.$W[...], ...), ...)
+          - pattern: $A = django.shortcuts.redirect(..., $S % request.$W[...], ...)
+          - pattern: $A = django.shortcuts.redirect(..., f"...{request.$W[...]}...", ...)
+          - pattern: return django.shortcuts.redirect(..., request.$W[...], ...)
+          - pattern: return django.shortcuts.redirect(..., $S.format(..., request.$W[...], ...), ...)
+          - pattern: return django.shortcuts.redirect(..., $S % request.$W[...], ...)
+          - pattern: return django.shortcuts.redirect(..., f"...{request.$W[...]}...", ...)
+          - pattern: django.shortcuts.redirect(..., request.$W, ...)
+          - pattern: django.shortcuts.redirect(..., $S.format(..., request.$W, ...), ...)
+          - pattern: django.shortcuts.redirect(..., $S % request.$W, ...)
+          - pattern: django.shortcuts.redirect(..., f"...{request.$W}...", ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.shortcuts.redirect(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $DATA
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.shortcuts.redirect(..., $STR.format(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $STR.format(..., $DATA, ...)
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.shortcuts.redirect(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.shortcuts.redirect(..., f"...{$DATA}...", ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.shortcuts.redirect(..., $STR + $DATA, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $STR + $DATA
+              ...
+              django.shortcuts.redirect(..., $INTERM, ...)
+          - pattern: $A = django.shortcuts.redirect(..., request.$W, ...)
+          - pattern: $A = django.shortcuts.redirect(..., $S.format(..., request.$W, ...), ...)
+          - pattern: $A = django.shortcuts.redirect(..., $S % request.$W, ...)
+          - pattern: $A = django.shortcuts.redirect(..., f"...{request.$W}...", ...)
+          - pattern: return django.shortcuts.redirect(..., request.$W, ...)
+          - pattern: return django.shortcuts.redirect(..., $S.format(..., request.$W, ...), ...)
+          - pattern: return django.shortcuts.redirect(..., $S % request.$W, ...)
+          - pattern: return django.shortcuts.redirect(..., f"...{request.$W}...", ...)
+          - pattern: django.http.HttpResponseRedirect(..., request.$W.get(...), ...)
+          - pattern: django.http.HttpResponseRedirect(..., $S.format(..., request.$W.get(...), ...), ...)
+          - pattern: django.http.HttpResponseRedirect(..., $S % request.$W.get(...), ...)
+          - pattern: django.http.HttpResponseRedirect(..., f"...{request.$W.get(...)}...", ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.http.HttpResponseRedirect(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = $DATA
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.http.HttpResponseRedirect(..., $STR.format(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = $STR.format(..., $DATA, ...)
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.http.HttpResponseRedirect(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.http.HttpResponseRedirect(..., f"...{$DATA}...", ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.http.HttpResponseRedirect(..., $STR + $DATA, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = $STR + $DATA
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: $A = django.http.HttpResponseRedirect(..., request.$W.get(...), ...)
+          - pattern: $A = django.http.HttpResponseRedirect(..., $S.format(..., request.$W.get(...), ...), ...)
+          - pattern: $A = django.http.HttpResponseRedirect(..., $S % request.$W.get(...), ...)
+          - pattern: $A = django.http.HttpResponseRedirect(..., f"...{request.$W.get(...)}...", ...)
+          - pattern: return django.http.HttpResponseRedirect(..., request.$W.get(...), ...)
+          - pattern: return django.http.HttpResponseRedirect(..., $S.format(..., request.$W.get(...), ...), ...)
+          - pattern: return django.http.HttpResponseRedirect(..., $S % request.$W.get(...), ...)
+          - pattern: return django.http.HttpResponseRedirect(..., f"...{request.$W.get(...)}...", ...)
+          - pattern: django.http.HttpResponseRedirect(..., request.$W(...), ...)
+          - pattern: django.http.HttpResponseRedirect(..., $S.format(..., request.$W(...), ...), ...)
+          - pattern: django.http.HttpResponseRedirect(..., $S % request.$W(...), ...)
+          - pattern: django.http.HttpResponseRedirect(..., f"...{request.$W(...)}...", ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.http.HttpResponseRedirect(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = $DATA
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.http.HttpResponseRedirect(..., $STR.format(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = $STR.format(..., $DATA, ...)
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.http.HttpResponseRedirect(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.http.HttpResponseRedirect(..., f"...{$DATA}...", ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.http.HttpResponseRedirect(..., $STR + $DATA, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = $STR + $DATA
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: $A = django.http.HttpResponseRedirect(..., request.$W(...), ...)
+          - pattern: $A = django.http.HttpResponseRedirect(..., $S.format(..., request.$W(...), ...), ...)
+          - pattern: $A = django.http.HttpResponseRedirect(..., $S % request.$W(...), ...)
+          - pattern: $A = django.http.HttpResponseRedirect(..., f"...{request.$W(...)}...", ...)
+          - pattern: return django.http.HttpResponseRedirect(..., request.$W(...), ...)
+          - pattern: return django.http.HttpResponseRedirect(..., $S.format(..., request.$W(...), ...), ...)
+          - pattern: return django.http.HttpResponseRedirect(..., $S % request.$W(...), ...)
+          - pattern: return django.http.HttpResponseRedirect(..., f"...{request.$W(...)}...", ...)
+          - pattern: django.http.HttpResponseRedirect(..., request.$W[...], ...)
+          - pattern: django.http.HttpResponseRedirect(..., $S.format(..., request.$W[...], ...), ...)
+          - pattern: django.http.HttpResponseRedirect(..., $S % request.$W[...], ...)
+          - pattern: django.http.HttpResponseRedirect(..., f"...{request.$W[...]}...", ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.http.HttpResponseRedirect(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = $DATA
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.http.HttpResponseRedirect(..., $STR.format(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = $STR.format(..., $DATA, ...)
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.http.HttpResponseRedirect(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.http.HttpResponseRedirect(..., f"...{$DATA}...", ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.http.HttpResponseRedirect(..., $STR + $DATA, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = $STR + $DATA
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: $A = django.http.HttpResponseRedirect(..., request.$W[...], ...)
+          - pattern: $A = django.http.HttpResponseRedirect(..., $S.format(..., request.$W[...], ...), ...)
+          - pattern: $A = django.http.HttpResponseRedirect(..., $S % request.$W[...], ...)
+          - pattern: $A = django.http.HttpResponseRedirect(..., f"...{request.$W[...]}...", ...)
+          - pattern: return django.http.HttpResponseRedirect(..., request.$W[...], ...)
+          - pattern: return django.http.HttpResponseRedirect(..., $S.format(..., request.$W[...], ...), ...)
+          - pattern: return django.http.HttpResponseRedirect(..., $S % request.$W[...], ...)
+          - pattern: return django.http.HttpResponseRedirect(..., f"...{request.$W[...]}...", ...)
+          - pattern: django.http.HttpResponseRedirect(..., request.$W, ...)
+          - pattern: django.http.HttpResponseRedirect(..., $S.format(..., request.$W, ...), ...)
+          - pattern: django.http.HttpResponseRedirect(..., $S % request.$W, ...)
+          - pattern: django.http.HttpResponseRedirect(..., f"...{request.$W}...", ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.http.HttpResponseRedirect(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $DATA
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.http.HttpResponseRedirect(..., $STR.format(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $STR.format(..., $DATA, ...)
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.http.HttpResponseRedirect(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.http.HttpResponseRedirect(..., f"...{$DATA}...", ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.http.HttpResponseRedirect(..., $STR + $DATA, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $STR + $DATA
+              ...
+              django.http.HttpResponseRedirect(..., $INTERM, ...)
+          - pattern: $A = django.http.HttpResponseRedirect(..., request.$W, ...)
+          - pattern: $A = django.http.HttpResponseRedirect(..., $S.format(..., request.$W, ...), ...)
+          - pattern: $A = django.http.HttpResponseRedirect(..., $S % request.$W, ...)
+          - pattern: $A = django.http.HttpResponseRedirect(..., f"...{request.$W}...", ...)
+          - pattern: return django.http.HttpResponseRedirect(..., request.$W, ...)
+          - pattern: return django.http.HttpResponseRedirect(..., $S.format(..., request.$W, ...), ...)
+          - pattern: return django.http.HttpResponseRedirect(..., $S % request.$W, ...)
+          - pattern: return django.http.HttpResponseRedirect(..., f"...{request.$W}...", ...)
+      - metavariable-regex:
+          metavariable: $W
+          regex: (?!get_full_path)
+
+  - id: reflected-data-httpresponse
+    message:
+      Found request data reflected into HttpResponse. This could be vulnerable to XSS. Ensure the request data is properly
+      escaped or sanitzed.
+    metadata:
+      cwe: "CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')"
+      owasp: "A7: Cross-Site Scripting (XSS)"
+      references:
+        - https://django-book.readthedocs.io/en/latest/chapter20.html#cross-site-scripting-xss
+    languages: [python]
+    severity: WARNING
+    patterns:
+      - pattern-inside: |
+          def $FUNC(...):
+            ...
+      - pattern-either:
+          - pattern: django.http.HttpResponse(..., $S.format(..., request.$W.get(...), ...), ...)
+          - pattern: django.http.HttpResponse(..., $S % request.$W.get(...), ...)
+          - pattern: django.http.HttpResponse(..., f"...{request.$W.get(...)}...", ...)
+          - pattern: django.http.HttpResponse(..., request.$W.get(...), ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.http.HttpResponse(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = $DATA
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.http.HttpResponse(..., $STR.format(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = $STR.format(..., $DATA, ...)
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.http.HttpResponse(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.http.HttpResponse(..., f"...{$DATA}...", ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.http.HttpResponse(..., $STR + $DATA, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = $STR + $DATA
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: $A = django.http.HttpResponse(..., request.$W.get(...), ...)
+          - pattern: return django.http.HttpResponse(..., request.$W.get(...), ...)
+          - pattern: django.http.HttpResponse(..., $S.format(..., request.$W(...), ...), ...)
+          - pattern: django.http.HttpResponse(..., $S % request.$W(...), ...)
+          - pattern: django.http.HttpResponse(..., f"...{request.$W(...)}...", ...)
+          - pattern: django.http.HttpResponse(..., request.$W(...), ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.http.HttpResponse(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = $DATA
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.http.HttpResponse(..., $STR.format(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = $STR.format(..., $DATA, ...)
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.http.HttpResponse(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.http.HttpResponse(..., f"...{$DATA}...", ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.http.HttpResponse(..., $STR + $DATA, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = $STR + $DATA
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: $A = django.http.HttpResponse(..., request.$W(...), ...)
+          - pattern: return django.http.HttpResponse(..., request.$W(...), ...)
+          - pattern: django.http.HttpResponse(..., $S.format(..., request.$W[...], ...), ...)
+          - pattern: django.http.HttpResponse(..., $S % request.$W[...], ...)
+          - pattern: django.http.HttpResponse(..., f"...{request.$W[...]}...", ...)
+          - pattern: django.http.HttpResponse(..., request.$W[...], ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.http.HttpResponse(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = $DATA
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.http.HttpResponse(..., $STR.format(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = $STR.format(..., $DATA, ...)
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.http.HttpResponse(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.http.HttpResponse(..., f"...{$DATA}...", ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.http.HttpResponse(..., $STR + $DATA, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = $STR + $DATA
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: $A = django.http.HttpResponse(..., request.$W[...], ...)
+          - pattern: return django.http.HttpResponse(..., request.$W[...], ...)
+          - pattern: django.http.HttpResponse(..., $S.format(..., request.$W, ...), ...)
+          - pattern: django.http.HttpResponse(..., $S % request.$W, ...)
+          - pattern: django.http.HttpResponse(..., f"...{request.$W}...", ...)
+          - pattern: django.http.HttpResponse(..., request.$W, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.http.HttpResponse(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $DATA
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.http.HttpResponse(..., $STR.format(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $STR.format(..., $DATA, ...)
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.http.HttpResponse(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.http.HttpResponse(..., f"...{$DATA}...", ...)
+          - pattern: $A = django.http.HttpResponse(..., request.$W, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $STR + $DATA
+              ...
+              $A = django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: return django.http.HttpResponse(..., request.$W, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.http.HttpResponse(..., $STR + $DATA, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $STR + $DATA
+              ...
+              django.http.HttpResponse(..., $INTERM, ...)
+
+  - id: reflected-data-httpresponsebadrequest
+    message:
+      Found request data reflected into HttpResponseBadRequest. This could be vulnerable to XSS. Ensure the request data
+      is properly escaped or sanitzed.
+    metadata:
+      cwe: "CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')"
+      owasp: "A7: Cross-Site Scripting (XSS)"
+      references:
+        - https://django-book.readthedocs.io/en/latest/chapter20.html#cross-site-scripting-xss
+    languages: [python]
+    severity: WARNING
+    patterns:
+      - pattern-inside: |
+          def $FUNC(...):
+            ...
+      - pattern-either:
+          - pattern: django.http.HttpResponseBadRequest(..., $S.format(..., request.$W.get(...), ...), ...)
+          - pattern: django.http.HttpResponseBadRequest(..., $S % request.$W.get(...), ...)
+          - pattern: django.http.HttpResponseBadRequest(..., f"...{request.$W.get(...)}...", ...)
+          - pattern: django.http.HttpResponseBadRequest(..., request.$W.get(...), ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.http.HttpResponseBadRequest(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = $DATA
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.http.HttpResponseBadRequest(..., $STR.format(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = $STR.format(..., $DATA, ...)
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.http.HttpResponseBadRequest(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.http.HttpResponseBadRequest(..., f"...{$DATA}...", ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.http.HttpResponseBadRequest(..., $STR + $DATA, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = $STR + $DATA
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: $A = django.http.HttpResponseBadRequest(..., request.$W.get(...), ...)
+          - pattern: return django.http.HttpResponseBadRequest(..., request.$W.get(...), ...)
+          - pattern: django.http.HttpResponseBadRequest(..., $S.format(..., request.$W(...), ...), ...)
+          - pattern: django.http.HttpResponseBadRequest(..., $S % request.$W(...), ...)
+          - pattern: django.http.HttpResponseBadRequest(..., f"...{request.$W(...)}...", ...)
+          - pattern: django.http.HttpResponseBadRequest(..., request.$W(...), ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.http.HttpResponseBadRequest(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = $DATA
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.http.HttpResponseBadRequest(..., $STR.format(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = $STR.format(..., $DATA, ...)
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.http.HttpResponseBadRequest(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.http.HttpResponseBadRequest(..., f"...{$DATA}...", ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.http.HttpResponseBadRequest(..., $STR + $DATA, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = $STR + $DATA
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: $A = django.http.HttpResponseBadRequest(..., request.$W(...), ...)
+          - pattern: return django.http.HttpResponseBadRequest(..., request.$W(...), ...)
+          - pattern: django.http.HttpResponseBadRequest(..., $S.format(..., request.$W[...], ...), ...)
+          - pattern: django.http.HttpResponseBadRequest(..., $S % request.$W[...], ...)
+          - pattern: django.http.HttpResponseBadRequest(..., f"...{request.$W[...]}...", ...)
+          - pattern: django.http.HttpResponseBadRequest(..., request.$W[...], ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.http.HttpResponseBadRequest(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = $DATA
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.http.HttpResponseBadRequest(..., $STR.format(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = $STR.format(..., $DATA, ...)
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.http.HttpResponseBadRequest(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.http.HttpResponseBadRequest(..., f"...{$DATA}...", ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.http.HttpResponseBadRequest(..., $STR + $DATA, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = $STR + $DATA
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: $A = django.http.HttpResponseBadRequest(..., request.$W[...], ...)
+          - pattern: return django.http.HttpResponseBadRequest(..., request.$W[...], ...)
+          - pattern: django.http.HttpResponseBadRequest(..., $S.format(..., request.$W, ...), ...)
+          - pattern: django.http.HttpResponseBadRequest(..., $S % request.$W, ...)
+          - pattern: django.http.HttpResponseBadRequest(..., f"...{request.$W}...", ...)
+          - pattern: django.http.HttpResponseBadRequest(..., request.$W, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.http.HttpResponseBadRequest(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $DATA
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.http.HttpResponseBadRequest(..., $STR.format(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $STR.format(..., $DATA, ...)
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.http.HttpResponseBadRequest(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.http.HttpResponseBadRequest(..., f"...{$DATA}...", ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.http.HttpResponseBadRequest(..., $STR + $DATA, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $STR + $DATA
+              ...
+              django.http.HttpResponseBadRequest(..., $INTERM, ...)
+          - pattern: $A = django.http.HttpResponseBadRequest(..., request.$W, ...)
+          - pattern: return django.http.HttpResponseBadRequest(..., request.$W, ...)
+
+  - id: request-data-fileresponse
+    message:
+      Found request data opening a file into FileResponse. This is dangerous because an attacker could specify an arbitrary
+      file to read, leaking data. Be sure to validate or sanitize the filename before using it in FileResponse.
+    metadata:
+      cwe: "CWE-22: Improper Limitation of a Pathname to a Restricted Directory ('Path Traversal')"
+      owasp: "A1: Injection"
+      references:
+        - https://django-book.readthedocs.io/en/latest/chapter20.html#cross-site-scripting-xss
+    languages: [python]
+    severity: WARNING
+    patterns:
+      - pattern-inside: |
+          def $FUNC(...):
+            ...
+      - pattern-either:
+          - pattern: django.http.FileResponse(..., request.$W.get(...), ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              django.http.FileResponse(..., open($DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = open($DATA, ...)
+              ...
+              django.http.FileResponse(..., $INTERM, ...)
+          - pattern: $A = django.http.FileResponse(..., request.$W.get(...), ...)
+          - pattern: return django.http.FileResponse(..., request.$W.get(...), ...)
+          - pattern: django.http.FileResponse(..., request.$W(...), ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              django.http.FileResponse(..., open($DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = open($DATA, ...)
+              ...
+              django.http.FileResponse(..., $INTERM, ...)
+          - pattern: $A = django.http.FileResponse(..., request.$W(...), ...)
+          - pattern: return django.http.FileResponse(..., request.$W(...), ...)
+          - pattern: django.http.FileResponse(..., request.$W[...], ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              django.http.FileResponse(..., open($DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = open($DATA, ...)
+              ...
+              django.http.FileResponse(..., $INTERM, ...)
+          - pattern: $A = django.http.FileResponse(..., request.$W[...], ...)
+          - pattern: return django.http.FileResponse(..., request.$W[...], ...)
+          - pattern: django.http.FileResponse(..., request.$W, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              django.http.FileResponse(..., open($DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = open($DATA, ...)
+              ...
+              django.http.FileResponse(..., $INTERM, ...)
+          - pattern: $A = django.http.FileResponse(..., request.$W, ...)
+          - pattern: return django.http.FileResponse(..., request.$W, ...)
+
+  - id: request-data-write
+    message: |
+      Found request data in '.write(...)'. This could be dangerous if a malicious
+      actor is able to control data into sensitive files. For example, a malicious
+      actor could force rolling of critical log files, or cause a denial-of-service
+      by using up available disk space. Ensure content is validated.
+    metadata:
+      cwe: "CWE-93: Improper Neutralization of CRLF Sequences ('CRLF Injection')"
+      owasp: "A1: Injection"
+    languages: [python]
+    severity: WARNING
+    patterns:
+      - pattern-either:
+          - pattern: $F.write(..., request.$W.get(...), ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $F.write(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = $DATA
+              ...
+              $F.write(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $F.write(..., $B.$C(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = $B.$C(..., $DATA, ...)
+              ...
+              $F.write(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $F.write(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              $F.write(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $F.write(..., f"...{$DATA}...", ...)
+          - pattern: |
+              $DATA = request.$W.get(...)
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              $F.write(..., $INTERM, ...)
+          - pattern: $A = $F.write(..., request.$W.get(...), ...)
+          - pattern: return $F.write(..., request.$W.get(...), ...)
+          - pattern: $F.write(..., request.$W(...), ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $F.write(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = $DATA
+              ...
+              $F.write(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $F.write(..., $B.$C(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = $B.$C(..., $DATA, ...)
+              ...
+              $F.write(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $F.write(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              $F.write(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $F.write(..., f"...{$DATA}...", ...)
+          - pattern: |
+              $DATA = request.$W(...)
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              $F.write(..., $INTERM, ...)
+          - pattern: $A = $F.write(..., request.$W(...), ...)
+          - pattern: return $F.write(..., request.$W(...), ...)
+          - pattern: $F.write(..., request.$W[...], ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $F.write(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = $DATA
+              ...
+              $F.write(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $F.write(..., $B.$C(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = $B.$C(..., $DATA, ...)
+              ...
+              $F.write(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $F.write(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              $F.write(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $F.write(..., f"...{$DATA}...", ...)
+          - pattern: |
+              $DATA = request.$W[...]
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              $F.write(..., $INTERM, ...)
+          - pattern: $A = $F.write(..., request.$W[...], ...)
+          - pattern: return $F.write(..., request.$W[...], ...)
+          - pattern: $F.write(..., request.$W, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $F.write(..., $DATA, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $DATA
+              ...
+              $F.write(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $F.write(..., $B.$C(..., $DATA, ...), ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $B.$C(..., $DATA, ...)
+              ...
+              $F.write(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $F.write(..., $STR % $DATA, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = $STR % $DATA
+              ...
+              $F.write(..., $INTERM, ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $F.write(..., f"...{$DATA}...", ...)
+          - pattern: |
+              $DATA = request.$W
+              ...
+              $INTERM = f"...{$DATA}..."
+              ...
+              $F.write(..., $INTERM, ...)
+          - pattern: $A = $F.write(..., request.$W, ...)
+          - pattern: return $F.write(..., request.$W, ...)
+
+  - id: password-empty-string
+    message: |
+      '$VAR' is the empty string and is being used to set the password on '$MODEL'.
+      If you meant to set an unusable password, set the password to None or call
+      'set_unusable_password()'.
+    metadata:
+      cwe: "CWE-521: Weak Password Requirements"
+      owasp: "A2: Broken Authentication"
+      references:
+        - https://docs.djangoproject.com/en/3.0/ref/contrib/auth/#django.contrib.auth.models.User.set_password
+    patterns:
+      - pattern-either:
+          - pattern: |
+              $MODEL.set_password($EMPTY)
+              ...
+              $MODEL.save()
+          - pattern: |
+              $VAR = $EMPTY
+              ...
+              $MODEL.set_password($VAR)
+              ...
+              $MODEL.save()
+      - metavariable-regex:
+          metavariable: $EMPTY
+          regex: (\'\'|\"\")
+    languages: [python]
+    severity: ERROR
+
+  - id: use-none-for-password-default
+    message: |
+      '$VAR' is using the empty string as its default and is being used to set
+      the password on '$MODEL'. If you meant to set an unusable password, set
+      the default value to 'None' or call 'set_unusable_password()'.
+    metadata:
+      cwe: "CWE-521: Weak Password Requirements"
+      owasp: "A2: Broken Authentication"
+      references:
+        - https://docs.djangoproject.com/en/3.0/ref/contrib/auth/#django.contrib.auth.models.User.set_password
+    patterns:
+      - pattern-either:
+          - pattern: |
+              $VAR = request.$W.get($X, "")
+              ...
+              $MODEL.set_password($VAR)
+              ...
+              $MODEL.save(...)
+          - pattern: |
+              def $F(..., $VAR="", ...):
+                ...
+                $MODEL.set_password($VAR)
+    fix-regex:
+      regex: (def.*|request.*)(""|'')
+      replacement: \1None
+    languages: [python]
+    severity: ERROR
+
+  - id: docker-arbitrary-container-run
+    patterns:
+      - pattern-either:
+          - pattern-inside: |
+              $CLIENT = docker.from_env()
+              ...
+          - pattern-inside: |
+              $CLIENT = docker.DockerClient(...)
+              ...
+      - pattern-either:
+          - pattern: |
+              $CLIENT.containers.run(...)
+          - pattern: |
+              $CLIENT.containers.create(...)
+      - pattern-not: |
+          $CLIENT.containers.run("...",...)
+      - pattern-not: |
+          $CLIENT.containers.create("...",...)
+    message: |
+      If unverified user data can reach the `run` or `create` method it can result in runing arbitrary container.
+    languages:
+      - python
+    severity: WARNING
+  # Flask check3: Flask application app.run best practices https://flask.palletsprojects.com/en/1.1.x/api/?highlight=run#flask.Flask.run
+
+  # . Rules for app.run() parameters
+  - id: avoid_app_run_with_bad_host
+    patterns:
+      - pattern-either:
+          - pattern: app.run(..., host="0.0.0.0", ...)
+          - pattern: app.run(..., "0.0.0.0", ...)
+    message: Running flask app with host 0.0.0.0 could expose the server publicly.
+    metadata:
+      cwe: "CWE-668: Exposure of Resource to Wrong Sphere"
+      owasp: "A6: Security Misconfiguration"
+    languages: [python]
+    severity: WARNING
+  # Flask check3: Flask application app.run best practices https://flask.palletsprojects.com/en/1.1.x/api/?highlight=run#flask.Flask.run
+
+  - id: avoid_using_app_run_directly
+    patterns:
+      - pattern-not-inside: |
+          if __name__ == '__main__':
+            ...
+      - pattern-not-inside: |
+          def $X(...):
+            ...
+      - pattern: app.run(...)
+    message: top-level app.run(...) is ignored by flask. Consider putting app.run(...) behind a guard, like inside a function
+    metadata:
+      cwe: "CWE-668: Exposure of Resource to Wrong Sphere"
+      owasp: "A6: Security Misconfiguration"
+    languages: [python]
+    severity: WARNING
+
+  - id: debug-enabled
+    patterns:
+      - pattern-inside: |
+          import flask
+          ...
+      - pattern: $APP.run(..., debug=True, ...)
+    message: |
+      Detected Flask app with debug=True. Do not deploy to production with this flag enabled
+      as it will leak sensitive information. Instead, consider using Flask configuration
+      variables or setting 'debug' using system environment variables.
+    metadata:
+      cwe: "CWE-489: Active Debug Code"
+      owasp: "A6: Security Misconfiguration"
+      references:
+        - https://labs.detectify.com/2015/10/02/how-patreon-got-hacked-publicly-exposed-werkzeug-debugger/
+    severity: WARNING
+    languages:
+      - python
+
+  - id: directly-returned-format-string
+    message: |
+      Detected Flask route directly returning a formatted string. This
+      is subject to cross-site scripting if user input can reach the string.
+      Consider using the template engine instead and rendering pages with
+      'render_template()'.
+    metadata:
+      cwe: "CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')"
+      owasp: "A7: Cross-site Scripting (XSS)"
+    languages:
+      - python
+    severity: WARNING
+    patterns:
+      - pattern-inside: |
+          @$APP.route(...)
+          def $FUNC(...):
+            ...
+      - pattern-not-inside: return "..."
+      - pattern-either:
+          - pattern: return "...".format(...)
+          - pattern: return "..." % ...
+          - pattern: return "..." + ...
+          - pattern: return ... + "..."
+          - pattern: return f"...{...}..."
+          - patterns:
+              - pattern: return $X
+              - pattern-either:
+                  - pattern-inside: |
+                      $X = "...".format(...)
+                      ...
+                  - pattern-inside: |
+                      $X = "..." % ...
+                      ...
+                  - pattern-inside: |
+                      $X = "..." + ...
+                      ...
+                  - pattern-inside: |
+                      $X = ... + "..."
+                      ...
+                  - pattern-inside: |
+                      $X = f"...{...}..."
+                      ...
+  # Flask check3: Avoid hardcoded config rules
+
+  - id: avoid_hardcoded_config_TESTING
+    pattern-either:
+      - pattern: $M.config['TESTING'] = True
+      - pattern: $M.config['TESTING'] = False
+      - pattern: $M.update(TESTING=True, ...)
+      - pattern: $M.update(TESTING=False, ...)
+    message: Hardcoded variable `TESTING` detected. Use environment variables or config files instead
+    metadata:
+      cwe: "CWE-489: Active Debug Code"
+      owasp: "A6: Security Misconfiguration"
+      references:
+        - https://bento.dev/checks/flask/avoid-hardcoded-config/
+        - https://flask.palletsprojects.com/en/1.1.x/config/?highlight=configuration#builtin-configuration-values
+        - https://flask.palletsprojects.com/en/1.1.x/config/?highlight=configuration#environment-and-debug-features
+    languages: [python]
+    severity: WARNING
+  - id: avoid_hardcoded_config_SECRET_KEY
+    pattern-either:
+      - pattern: $M.update(SECRET_KEY="=~/.*/")
+      - pattern: $M.config['SECRET_KEY'] = "=~/.*/"
+    message: Hardcoded variable `SECRET_KEY` detected. Use environment variables or config files instead
+    metadata:
+      cwe: "CWE-798: Use of Hard-coded Credentials"
+      owasp: "A2: Broken Authentication"
+      references:
+        - https://bento.dev/checks/flask/avoid-hardcoded-config/
+        - https://flask.palletsprojects.com/en/1.1.x/config/?highlight=configuration#builtin-configuration-values
+        - https://flask.palletsprojects.com/en/1.1.x/config/?highlight=configuration#environment-and-debug-features
+    languages: [python]
+    severity: ERROR
+  - id: avoid_hardcoded_config_ENV
+    pattern-either:
+      - pattern: $M.update(ENV="=~/^development|production$/")
+      - pattern: $M.config['ENV'] = "=~/^development|production$/"
+    message: Hardcoded variable `ENV` detected. Set this by using FLASK_ENV environment variable
+    metadata:
+      cwe: "CWE-489: Active Debug Code"
+      owasp: "A6: Security Misconfiguration"
+      references:
+        - https://bento.dev/checks/flask/avoid-hardcoded-config/
+        - https://flask.palletsprojects.com/en/1.1.x/config/?highlight=configuration#builtin-configuration-values
+        - https://flask.palletsprojects.com/en/1.1.x/config/?highlight=configuration#environment-and-debug-features
+    languages: [python]
+    severity: WARNING
+  - id: avoid_hardcoded_config_DEBUG
+    pattern-either:
+      - pattern: $M.update(DEBUG=True)
+      - pattern: $M.update(DEBUG=False)
+      - pattern: $M.config['DEBUG'] = True
+      - pattern: $M.config['DEBUG'] = False
+    message: Hardcoded variable `DEBUG` detected. Set this by using FLASK_DEBUG environment variable
+    metadata:
+      cwe: "CWE-489: Active Debug Code"
+      owasp: "A6: Security Misconfiguration"
+      references:
+        - https://bento.dev/checks/flask/avoid-hardcoded-config/
+        - https://flask.palletsprojects.com/en/1.1.x/config/?highlight=configuration#builtin-configuration-values
+        - https://flask.palletsprojects.com/en/1.1.x/config/?highlight=configuration#environment-and-debug-features
+    languages: [python]
+    severity: WARNING
+
+  - id: render-template-string
+    pattern: flask.render_template_string(...)
+    metadata:
+      cwe: "CWE-96: Improper Neutralization of Directives in Statically Saved Code ('Static Code Injection')"
+      owasp: "A1: Injection"
+      references:
+        - https://nvisium.com/blog/2016/03/09/exploring-ssti-in-flask-jinja2.html
+    message:
+      Found a template created with string formatting. This is susceptible to server-side template injection and cross-site
+      scripting attacks.
+    languages: [python]
+    severity: WARNING
+
+  - id: secure-set-cookie
+    patterns:
+      - pattern-either:
+          - pattern-inside: |
+              $RESP = flask.make_response(...)
+              ...
+          - pattern-inside: |
+              $RESP = flask.Response(...)
+              ...
+      - pattern-not: $RESPONSE.set_cookie(..., secure=$A, httponly=$B, samesite=$C, ...)
+      - pattern-not: $RESPONSE.set_cookie(..., **$A)
+      - pattern: $RESPONSE.set_cookie(...)
+    message: |
+      Flask cookies should be handled securely by setting secure=True, httponly=True, and samesite='Lax' in
+      response.set_cookie(...). If your situation calls for different settings, explicitly disable the setting.
+      If you want to send the cookie over http, set secure=False.  If you want to let client-side JavaScript
+      read the cookie, set httponly=False. If you want to attach cookies to requests for external sites,
+      set samesite=None.
+    metadata:
+      cwe: "CWE-614: Sensitive Cookie in HTTPS Session Without 'Secure' Attribute"
+      owasp: "A3: Sensitive Data Exposure"
+      references:
+        - https://blog.r2c.dev/2020/bento-check-keeping-cookies-safe-in-flask/
+        - https://bento.dev/checks/flask/secure-set-cookie/
+        - https://flask.palletsprojects.com/en/1.1.x/security/#set-cookie-options
+    languages: [python]
+    severity: WARNING
+
+  - id: flask-wtf-csrf-disabled
+    patterns:
+      - pattern: |
+          $APP.config['WTF_CSRF_ENABLED'] = False
+    message: |
+      `$APP.config['WTF_CSRF_ENABLED'] = False` is probably not what you want in production because it disables https://flask-wtf.readthedocs.io/en/stable/csrf.html CSRF protection
+    metadata:
+      cwe: "CWE-352: Cross-Site Request Forgery (CSRF)"
+      owasp: "A6: Security Misconfiguration"
+      references:
+        - https://flask-wtf.readthedocs.io/en/stable/csrf.html
+    severity: WARNING
+    languages:
+      - python
+
+  - id: os-system-injection
+    languages:
+      - python
+    severity: ERROR
+    message: >-
+      User data detected in os.system. This could be vulnerable to a command injection and should be avoided. If this
+      must be done, use the 'subprocess' module instead and pass the arguments as a list.
+    metadata:
+      cwe: "CWE-78: Improper Neutralization of Special Elements used in an OS Command ('OS Command Injection')"
+      owasp: "A1: Injection"
+      references:
+        - https://owasp.org/www-community/attacks/Command_Injection
+    patterns:
+      - pattern-either:
+          - patterns:
+              - pattern-inside: |
+                  @$APP.route($ROUTE, ...)
+                  def $FUNC(..., $ROUTEVAR, ...):
+                    ...
+              - pattern-either:
+                  - pattern: os.system(..., <... $ROUTEVAR ...>, ...)
+                  - pattern: |
+                      $INTERM = <... $ROUTEVAR ...>
+                      ...
+                      os.system(..., <... $INTERM ...>, ...)
+          - patterns:
+              - pattern-either:
+                  - pattern: os.system(..., <... flask.request.$W.get(...) ...>, ...)
+                  - pattern: os.system(..., <... flask.request.$W[...] ...>, ...)
+                  - pattern: os.system(..., <... flask.request.$W(...) ...>, ...)
+                  - pattern: os.system(..., <... flask.request.$W ...>, ...)
+          - patterns:
+              - pattern-either:
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W.get(...) ...>
+                          ...
+                          os.system(<... $INTERM ...>)
+                      - pattern: os.system(...)
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W[...] ...>
+                          ...
+                          os.system(<... $INTERM ...>)
+                      - pattern: os.system(...)
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W(...) ...>
+                          ...
+                          os.system(<... $INTERM ...>)
+                      - pattern: os.system(...)
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W ...>
+                          ...
+                          os.system(<... $INTERM ...>)
+                      - pattern: os.system(...)
+
+  - id: path-traversal-open
+    languages:
+      - python
+    severity: ERROR
+    message: >-
+      Found request data in a call to 'open'. Ensure the request data is validated or sanitized, otherwise it could result
+      in path traversal attacks.
+    metadata:
+      cwe: "CWE-22: Improper Limitation of a Pathname to a Restricted Directory ('Path Traversal')"
+      owasp: "A1: Injection"
+      references:
+        - https://owasp.org/www-community/attacks/Path_Traversal
+    patterns:
+      - pattern-either:
+          - patterns:
+              - pattern-inside: |
+                  @$APP.route($ROUTE, ...)
+                  def $FUNC(..., $ROUTEVAR, ...):
+                    ...
+              - pattern-either:
+                  - pattern: open(..., <... $ROUTEVAR ...>, ...)
+                  - pattern: |
+                      $INTERM = <... $ROUTEVAR ...>
+                      ...
+                      open(..., <... $INTERM ...>, ...)
+          - patterns:
+              - pattern-either:
+                  - pattern: open(..., <... flask.request.$W.get(...) ...>, ...)
+                  - pattern: open(..., <... flask.request.$W[...] ...>, ...)
+                  - pattern: open(..., <... flask.request.$W(...) ...>, ...)
+                  - pattern: open(..., <... flask.request.$W ...>, ...)
+          - patterns:
+              - pattern-either:
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W.get(...) ...>
+                          ...
+                          open(<... $INTERM ...>, ...)
+                      - pattern: open(...)
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W[...] ...>
+                          ...
+                          open(<... $INTERM ...>, ...)
+                      - pattern: open(...)
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W(...) ...>
+                          ...
+                          open(<... $INTERM ...>, ...)
+                      - pattern: open(...)
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W ...>
+                          ...
+                          open(<... $INTERM ...>, ...)
+                      - pattern: open(...)
+          - patterns:
+              - pattern-either:
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W.get(...) ...>
+                          ...
+                          with open(<... $INTERM ...>, ...) as $F:
+                            ...
+                      - pattern: open(...)
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W[...] ...>
+                          ...
+                          with open(<... $INTERM ...>, ...) as $F:
+                            ...
+                      - pattern: open(...)
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W(...) ...>
+                          ...
+                          with open(<... $INTERM ...>, ...) as $F:
+                            ...
+                      - pattern: open(...)
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W ...>
+                          ...
+                          with open(<... $INTERM ...>, ...) as $F:
+                            ...
+                      - pattern: open(...)
+
+  - id: ssrf-requests
+    languages:
+      - python
+    severity: ERROR
+    message:
+      Data from request object is passed to a new server-side request. This could lead to a server-side request forgery
+      (SSRF). To mitigate, ensure that schemes and hosts are validated against a whitelist, do not forward the response to the
+      user, and ensure proper authentication and transport-layer security in the proxied request.
+    metadata:
+      cwe: "CWE-918: Server-Side Request Forgery (SSRF)"
+      owasp: "A1: Injection"
+      references:
+        - https://owasp.org/www-community/attacks/Server_Side_Request_Forgery
+    patterns:
+      - pattern-either:
+          - patterns:
+              - pattern-inside: |
+                  @$APP.route($ROUTE, ...)
+                  def $ROUTE_FUNC(..., $ROUTEVAR, ...):
+                    ...
+              - pattern-either:
+                  - pattern: requests.$FUNC(..., <... $ROUTEVAR ...>, ...)
+                  - pattern: |
+                      $INTERM = <... $ROUTEVAR ...>
+                      ...
+                      requests.$FUNC(..., <... $INTERM ...>, ...)
+          - patterns:
+              - pattern-either:
+                  - pattern: requests.$FUNC(..., <... flask.request.$W.get(...) ...>, ...)
+                  - pattern: requests.$FUNC(..., <... flask.request.$W[...] ...>, ...)
+                  - pattern: requests.$FUNC(..., <... flask.request.$W(...) ...>, ...)
+                  - pattern: requests.$FUNC(..., <... flask.request.$W ...>, ...)
+          - patterns:
+              - pattern-either:
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W.get(...) ...>
+                          ...
+                          requests.$FUNC(<... $INTERM ...>, ...)
+                      - pattern: requests.$FUNC(...)
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W[...] ...>
+                          ...
+                          requests.$FUNC(<... $INTERM ...>, ...)
+                      - pattern: requests.$FUNC(...)
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W(...) ...>
+                          ...
+                          requests.$FUNC(<... $INTERM ...>, ...)
+                      - pattern: requests.$FUNC(...)
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W ...>
+                          ...
+                          requests.$FUNC(<... $INTERM ...>, ...)
+                      - pattern: requests.$FUNC(...)
+
+  - id: eval-injection
+    languages:
+      - python
+    severity: ERROR
+    message: Detected user data flowing into eval. This is code injection and should be avoided.
+    metadata:
+      cwe: "CWE-95: Improper Neutralization of Directives in Dynamically Evaluated Code ('Eval Injection')"
+      owasp: "A1: Injection"
+      references:
+        - https://nedbatchelder.com/blog/201206/eval_really_is_dangerous.html
+    patterns:
+      - pattern-either:
+          - patterns:
+              - pattern-inside: |
+                  @$APP.route($ROUTE, ...)
+                  def $FUNC(..., $ROUTEVAR, ...):
+                    ...
+              - pattern-either:
+                  - pattern: eval(..., <... $ROUTEVAR ...>, ...)
+                  - pattern: |
+                      $INTERM = <... $ROUTEVAR ...>
+                      ...
+                      eval(..., <... $INTERM ...>, ...)
+          - patterns:
+              - pattern-either:
+                  - pattern: eval(..., <... flask.request.$W.get(...) ...>, ...)
+                  - pattern: eval(..., <... flask.request.$W[...] ...>, ...)
+                  - pattern: eval(..., <... flask.request.$W(...) ...>, ...)
+                  - pattern: eval(..., <... flask.request.$W ...>, ...)
+          - patterns:
+              - pattern-either:
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W.get(...) ...>
+                          ...
+                          eval(..., <... $INTERM ...>, ...)
+                      - pattern: eval(...)
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W[...] ...>
+                          ...
+                          eval(..., <... $INTERM ...>, ...)
+                      - pattern: eval(...)
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W(...) ...>
+                          ...
+                          eval(..., <... $INTERM ...>, ...)
+                      - pattern: eval(...)
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W ...>
+                          ...
+                          eval(..., <... $INTERM ...>, ...)
+                      - pattern: eval(...)
+
+  - id: exec-injection
+    languages:
+      - python
+    severity: ERROR
+    message: Detected user data flowing into exec. This is code injection and should be avoided.
+    metadata:
+      cwe: "CWE-95: Improper Neutralization of Directives in Dynamically Evaluated Code ('Eval Injection')"
+      owasp: "A1: Injection"
+      references:
+        - https://nedbatchelder.com/blog/201206/exec_really_is_dangerous.html
+    patterns:
+      - pattern-either:
+          - patterns:
+              - pattern-inside: |
+                  @$APP.route($ROUTE, ...)
+                  def $FUNC(..., $ROUTEVAR, ...):
+                    ...
+              - pattern-either:
+                  - pattern: exec(..., <... $ROUTEVAR ...>, ...)
+                  - pattern: |
+                      $INTERM = <... $ROUTEVAR ...>
+                      ...
+                      exec(..., <... $INTERM ...>, ...)
+          - patterns:
+              - pattern-either:
+                  - pattern: exec(..., <... flask.request.$W.get(...) ...>, ...)
+                  - pattern: exec(..., <... flask.request.$W[...] ...>, ...)
+                  - pattern: exec(..., <... flask.request.$W(...) ...>, ...)
+                  - pattern: exec(..., <... flask.request.$W ...>, ...)
+          - patterns:
+              - pattern-either:
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W.get(...) ...>
+                          ...
+                          exec(..., <... $INTERM ...>, ...)
+                      - pattern: exec(...)
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W[...] ...>
+                          ...
+                          exec(..., <... $INTERM ...>, ...)
+                      - pattern: exec(...)
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W(...) ...>
+                          ...
+                          exec(..., <... $INTERM ...>, ...)
+                      - pattern: exec(...)
+                  - patterns:
+                      - pattern-inside: |
+                          $INTERM = <... flask.request.$W ...>
+                          ...
+                          exec(..., <... $INTERM ...>, ...)
+                      - pattern: exec(...)
+
+  - id: autoescape-disabled
+    patterns:
+      - pattern-not: jinja2.Environment(..., autoescape=True, ...)
+      - pattern-not: jinja2.Environment(..., autoescape=jinja2.select_autoescape(...), ...)
+      - pattern: jinja2.Environment(...)
+    fix-regex:
+      regex: (.*)\)
+      replacement: \1, autoescape=True)
+    message: >-
+      Detected a Jinja2 environment without autoescaping. Jinja2 does not autoescape by default.
+      This is dangerous if you are rendering to a browser because this allows for cross-site
+      scripting (XSS) attacks. If you are in a web context, enable autoescaping by setting
+      'autoescape=True.' You may also consider using 'jinja2.select_autoescape()' to only enable
+      automatic escaping for certain file extensions.
+    metadata:
+      cwe: "CWE-116: Improper Encoding or Escaping of Output"
+      owasp: "A6: Security Misconfiguration"
+      references:
+        - https://jinja.palletsprojects.com/en/2.11.x/api/#basics
+    languages: [python]
+    severity: WARNING
+
+  - id: jwt-python-exposed-data
+    message: |
+      The object is passed strictly to jwt.encode(...)
+      Make sure that sensitive information is not exposed through JWT token payload.
+    severity: WARNING
+    metadata:
+      owasp: A3:2017-Sensitive Data Exposure
+      cwe: "CWE-522: Insufficiently Protected Credentials"
+      source-rule-url: https://r2c.dev/blog/2020/hardcoded-secrets-unverified-tokens-and-other-common-jwt-mistakes/
+    languages: [python]
+    patterns:
+      - pattern-inside: |
+          def $FUNC(...,$INPUT,...):
+            ...
+      - pattern: |-
+          jwt.encode($INPUT,...)
+
+  - id: multiprocessing-recv
+    languages:
+      - python
+    message:
+      "The Connection.recv() method automatically unpickles the data it receives, which can be a security risk unless
+      you can trust the process which sent the message. Therefore, unless the connection object was produced using Pipe() you
+      should only use the recv() and send() methods after performing some sort of authentication. See more dettails: https://docs.python.org/3/library/multiprocessing.html?highlight=security#multiprocessing.connection.Connection"
+    metadata:
+      cwe: "CWE-502: Deserialization of Untrusted Data"
+      owasp: "A8: Insecure Deserialization"
+      references:
+        - https://docs.python.org/3/library/multiprocessing.html?highlight=security#multiprocessing.connection.Connection
+    pattern-either:
+      - pattern: multiprocessing.connection.Connection.recv(...)
+      - pattern: multiprocessing.connection.Client.recv(...)
+      - pattern: |
+          $C = multiprocessing.connection.Client(...)
+          ...
+          $C.recv(...)
+    severity: WARNING
+
+  - id: dangerous-spawn-process
+    patterns:
+      - pattern-either:
+          - patterns:
+              - pattern-not: os.$W("...", ...)
+              - pattern-either:
+                  - pattern: os.execl(...)
+                  - pattern: os.execle(...)
+                  - pattern: os.execlp(...)
+                  - pattern: os.execlpe(...)
+                  - pattern: os.execv(...)
+                  - pattern: os.execve(...)
+                  - pattern: os.execvp(...)
+                  - pattern: os.execvpe(...)
+                  - pattern: os.startfile(...)
+          - patterns:
+              - pattern-not: os.$W($MODE, "...", ...)
+              - pattern-either:
+                  - pattern: os.spawnl(...)
+                  - pattern: os.spawnle(...)
+                  - pattern: os.spawnlp(...)
+                  - pattern: os.spawnlpe(...)
+                  - pattern: os.spawnv(...)
+                  - pattern: os.spawnve(...)
+                  - pattern: os.spawnvp(...)
+                  - pattern: os.spawnvpe(...)
+    message: |
+      Found dynamic content when spawning a process. This is dangerous if external
+      data can reach this function call because it allows a malicious actor to
+      execute commands. Ensure no external data reaches here.
+    metadata:
+      cwe: "CWE-78: Improper Neutralization of Special Elements used in an OS Command ('OS Command Injection')"
+      owasp: "A1: Injection"
+    languages: [python]
+    severity: WARNING
+
+  - id: dangerous-subprocess-use
+    patterns:
+      - pattern-not: subprocess.$FUNC("...", ...)
+      - pattern-not: subprocess.$FUNC([...], ...)
+      - pattern-not: subprocess.CalledProcessError(...)
+      - pattern-not: subprocess.SubprocessError(...)
+      - pattern: subprocess.$FUNC(...)
+    message: |
+      Detected subprocess function '$FUNC' without a static string. If this data can be
+      controlled by a malicious actor, it may be an instance of command injection.
+      Audit the use of this call to ensure it is not controllable by an external resource.
+      You may consider using 'shlex.escape()'.
+    metadata:
+      owasp: "A1: Injection"
+      cwe: "CWE-78: Improper Neutralization of Special Elements used in an OS Command ('OS Command Injection')"
+      references:
+        - https://stackoverflow.com/questions/3172470/actual-meaning-of-shell-true-in-subprocess
+        - https://docs.python.org/3/library/subprocess.html
+        - https://docs.python.org/3/library/shlex.html
+    languages: [python]
+    severity: WARNING
+
+  - id: dangerous-system-call
+    patterns:
+      - pattern-not: os.$W("...", ...)
+      - pattern-either:
+          - pattern: os.system(...)
+          - pattern: os.popen(...)
+          - pattern: os.popen2(...)
+          - pattern: os.popen3(...)
+          - pattern: os.popen4(...)
+    message: >-
+      Found dynamic content used in a system call. This is dangerous if external
+      data can reach this function call because it allows a malicious actor to
+      execute commands. Use the 'subprocess' module instead, which is easier
+      to use without accidentally exposing a command injection vulnerability.
+    metadata:
+      cwe: "CWE-78: Improper Neutralization of Special Elements used in an OS Command ('OS Command Injection')"
+      owasp: "A1: Injection"
+    languages: [python]
+    severity: WARNING
+
+  - id: dynamic-urllib-use-detected
+    patterns:
+      - pattern-not: urllib.$W("...")
+      - pattern-not: urllib.request.$W("...")
+      - pattern-not: $OPENER.$W("...")
+      - pattern-either:
+          - patterns:
+              - pattern-either:
+                  - pattern: urllib.urlopen(...)
+                  - pattern: urllib.request.urlopen(...)
+                  - pattern: urllib.urlretrieve(...)
+                  - pattern: urllib.request.urlretrieve(...)
+          - patterns:
+              - pattern-either:
+                  - pattern-inside: |
+                      $OPENER = urllib.URLopener(...)
+                      ...
+                  - pattern-inside: |
+                      $OPENER = urllib.request.URLopener(...)
+                      ...
+                  - pattern-inside: |
+                      $OPENER = urllib.FancyURLopener(...)
+                      ...
+                  - pattern-inside: |
+                      $OPENER = urllib.request.FancyURLopener(...)
+                      ...
+              - pattern-either:
+                  - pattern: $OPENER.open(...)
+                  - pattern: $OPENER.retrieve(...)
+    message: >-
+      Detected a dynamic value being used with urllib. urllib supports 'file://' schemes,
+      so a dynamic value controlled by a malicious actor may allow them to read arbitrary files.
+      Audit uses of urllib calls to ensure user data cannot control the URLs, or consider
+      using the 'requests' library instead.
+    metadata:
+      cwe: "CWE-939: Improper Authorization in Handler for Custom URL Scheme"
+      owasp: "A1: Injection"
+      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/blacklists/calls.py#L163
+      bandit-code: B310
+    languages: [python]
+    severity: WARNING
+
+  - id: eval-detected
+    patterns:
+      - pattern-not: eval("...")
+      - pattern: eval(...)
+    message: |
+      Detected the use of eval(). eval() can be dangerous if used to evaluate
+      dynamic content. If this content can be input from outside the program, this
+      may be a code injection vulnerability. Ensure evaluated content is not definable
+      by external sources.
+    metadata:
+      cwe: "CWE-95: Improper Neutralization of Directives in Dynamically Evaluated Code ('Eval Injection')"
+      owasp: "A1: Injection"
+    languages: [python]
+    severity: WARNING
+
+  - id: exec-detected
+    patterns:
+      - pattern-not: exec("...")
+      - pattern: exec(...)
+    message: |
+      Detected the use of exec(). exec() can be dangerous if used to evaluate
+      dynamic content. If this content can be input from outside the program, this
+      may be a code injection vulnerability. Ensure evaluated content is not definable
+      by external sources.
+    metadata:
+      cwe: "CWE-95: Improper Neutralization of Directives in Dynamically Evaluated Code ('Eval Injection')"
+      owasp: "A1: Injection"
+    languages: [python]
+    severity: WARNING
+
+  - id: formatted-sql-query
+    patterns:
+      - pattern-either:
+          - pattern: $DB.execute("..." % ...)
+          - pattern: $DB.execute("...".format(...))
+          - pattern: $DB.execute(f"...")
+          - patterns:
+              - pattern-either:
+                  - pattern-inside: |
+                      $SQL = "..." % ...
+                      ...
+                  - pattern-inside: |
+                      $SQL = "...".format(...)
+                      ...
+                  - pattern-inside: |
+                      $SQL = f"...{$X}..."
+                      ...
+              - pattern: $DB.execute($SQL)
+    message: |
+      Detected possible formatted SQL query. Use parameterized queries instead.
+    metadata:
+      owasp: "A1: Injection"
+      cwe: "CWE-89: Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection')"
+      references:
+        - https://stackoverflow.com/questions/775296/mysql-parameterized-queries
+    severity: WARNING
+    languages:
+      - python
+
+  - id: ftplib
+    pattern: ftplib.$ANYTHING(...)
+    message: |
+      FTP does not encrypt communications by default. This can lead to sensitive
+      data being exposed. Ensure use of FTP here does not expose sensitive data.
+    metadata:
+      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L265
+      cwe: "CWE-319: Cleartext Transmission of Sensitive Information"
+      owasp: "A3: Sensitive Data Exposure"
+      bandit-code: B321
+      references:
+        - https://docs.python.org/3/library/telnetlib.html
+    severity: WARNING
+    languages:
+      - python
+
+  - id: hardcoded-password-default-argument
+    patterns:
+      - pattern: |
+          def $FUNC(..., password="...", ...):
+            ...
+    message: |
+      Hardcoded password is used as a default argument to '$FUNC'. This could be dangerous if
+      a real password is not supplied.
+    languages: [python]
+    severity: WARNING
+
+  - id: httpsconnection-detected
+    patterns:
+      - pattern-either:
+          - pattern: httplib.HTTPSConnection(...)
+          - pattern: http.client.HTTPSConnection(...)
+          - pattern: six.moves.http_client.HTTPSConnection(...)
+    message: |
+      The HTTPSConnection API has changed frequently with minor releases of Python.
+      Ensure you are using the API for your version of Python securely.
+      For example, Python 3 versions prior to 3.4.3 will not verify SSL certificates by default.
+      See https://docs.python.org/3/library/http.client.html#http.client.HTTPSConnection
+      for more information.
+    metadata:
+      owasp: "A6: Security Misconfiguration"
+      cwe: "CWE-295: Improper Certificate Validation"
+      references:
+        - https://docs.python.org/3/library/http.client.html#http.client.HTTPSConnection
+    severity: WARNING
+    languages:
+      - python
+
+  - id: insecure-file-permissions
+    patterns:
+      - pattern-either:
+          - pattern: os.chmod($FILENAME, $MODE, ...)
+          - pattern: os.lchmod($FILENAME, $MODE)
+          - pattern: os.fchmod($FD, $MODE)
+      - pattern-where-python: |-
+          import stat
+
+          def stat_to_bits(mode):
+            bits = 0
+            for flag in mode.split('|'):
+              try:
+                bits |= {k: v for k, v in stat.__dict__.items() if type(v) == int}[flag.strip().replace("stat.", "")]
+              except: # ignore things that aren't in stat module
+                continue
+            return bits
+
+          def numeric_to_bits(mode):
+            # Try combos of ints: 0o777, 511, 0x1ff
+            bits = 0
+            for num in mode.split("|"):
+              num = num.strip()
+              try:
+                tidbit = int(num)
+              except:
+                try:
+                  tidbit = int(num, 8)
+                except:
+                  try:
+                    tidbit = int(num, 16)
+                  except:
+                    try:
+                      tidbit = int(num, 2)
+                    except:
+                      tidbit = 0
+              bits |= tidbit
+            return bits
+
+          perms = vars['$MODE']
+          try:
+            if "stat" in perms:
+              mode = stat_to_bits(perms)
+            else:
+              mode = numeric_to_bits(perms)
+          except:
+            mode = 0 # can't resolve. ignore this.
+
+          filemode = stat.filemode(mode)
+          alert = False
+          if 'w' in filemode[-3:] or 'x' in filemode[-3:]:
+            alert = True
+          elif 'x' in filemode[-6:-3]:
+            alert = True
+          alert
+    message: |
+      Insecure file permissions detected.
+    languages: [python]
+    severity: WARNING
+
+  - id: mako-templates-detected
+    pattern: mako.template.Template(...)
+    message: |
+      Mako templates do not provide a global HTML escaping mechanism.
+      This means you must escape all sensitive data in your templates
+      using '| u' for URL escaping or '| h' for HTML escaping.
+      If you are using Mako to serve web content, consider using
+      a system such as Jinja2 which enables global escaping.
+    metadata:
+      cwe: "CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')"
+      owasp: "A7: Cross-Site Scripting (XSS)"
+      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/mako_templates.py
+      references:
+        - https://docs.makotemplates.org/en/latest/syntax.html#expression-escaping
+        - https://jinja.palletsprojects.com/en/2.11.x/intro/#
+    languages: [python]
+    severity: INFO
+
+  - id: marshal-usage
+    languages:
+      - python
+    message: |
+      The marshal module is not intended to be secure against erroneous or maliciously constructed data.
+      Never unmarshal data received from an untrusted or unauthenticated source.
+      See more details: https://docs.python.org/3/library/marshal.html?highlight=security
+    metadata:
+      cwe: "CWE-502: Deserialization of Untrusted Data"
+      owasp: "A8: Insecure Deserialization"
+      references:
+        - https://docs.python.org/3/library/marshal.html?highlight=security
+    pattern-either:
+      - pattern: marshal.dump(...)
+      - pattern: marshal.dumps(...)
+      - pattern: marshal.load(...)
+      - pattern: marshal.loads(...)
+    severity: WARNING
+
+  - id: paramiko-implicit-trust-host-key
+    patterns:
+      - pattern-inside: |
+          $CLIENT = paramiko.client.SSHClient(...)
+          ...
+          $CLIENT.set_missing_host_key_policy(...)
+      - pattern-either:
+          - pattern: paramiko.client.AutoAddPolicy
+          - pattern: paramiko.client.WarningPolicy
+    message: |
+      Detected a paramiko host key policy that implicitly trusts a server's
+      host key. Host keys should be verified to ensure the connection
+      is not to a malicious server. Use RejectPolicy or a custom subclass
+      instead.
+    metadata:
+      cwe: "CWE-322: Key Exchange without Entity Authentication"
+      owasp: "A3: Sensitive Data Exposure"
+      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/ssh_no_host_key_verification.py
+      references:
+        - http://docs.paramiko.org/en/stable/api/client.html#paramiko.client.AutoAddPolicy
+    languages: [python]
+    severity: WARNING
+
+  - id: ssl-wrap-socket-is-deprecated
+    pattern: ssl.wrap_socket(...)
+    message: |
+      'ssl.wrap_socket()' is deprecated. This function creates an insecure socket
+      without server name indication or hostname matching. Instead, create an SSL
+      context using 'ssl.SSLContext()' and use that to wrap a socket.
+    metadata:
+      cwe: "CWE-326: Inadequate Encryption Strength"
+      owasp: "A3: Sensitive Data Exposure"
+      references:
+        - https://docs.python.org/3/library/ssl.html#ssl.wrap_socket
+        - https://docs.python.org/3/library/ssl.html#ssl.SSLContext.wrap_socket
+    languages: [python]
+    severity: WARNING
+
+  - id: subprocess-shell-true
+    pattern: subprocess.$FUNC(..., shell=True, ...)
+    message: |
+      Found 'subprocess' function '$FUNC' with 'shell=True'. This is dangerous because this call will spawn
+      the command using a shell process. Doing so propagates current shell settings and variables, which
+      makes it much easier for a malicious actor to execute commands. Use 'shell=False' instead.
+    fix-regex:
+      regex: (shell\s*=\s*)True
+      replacement: \1False
+    metadata:
+      owasp: "A1: Injection"
+      cwe: "CWE-78: Improper Neutralization of Special Elements used in an OS Command ('OS Command Injection')"
+      references:
+        - https://stackoverflow.com/questions/3172470/actual-meaning-of-shell-true-in-subprocess
+        - https://docs.python.org/3/library/subprocess.html
+    languages: [python]
+    severity: ERROR
+
+  - id: system-wildcard-detected
+    patterns:
+      - pattern-either:
+          - pattern-inside: os.system("...")
+          - pattern-inside: os.popen("...")
+          - pattern-inside: os.popen2("...")
+          - pattern-inside: os.popen3("...")
+          - pattern-inside: os.popen4("...")
+          - pattern-inside: subprocess.$W(..., shell=True, ...)
+      - pattern-regex: (tar|chmod|chown|rsync)(.*?)\*
+    message: |
+      Detected use of the wildcard character in a system call that spawns a shell.
+      This subjects the wildcard to normal shell expansion, which can have unintended consequences
+      if there exist any non-standard file names. Consider a file named '-e sh script.sh' -- this
+      will execute a script when 'rsync' is called. See
+      https://www.defensecode.com/public/DefenseCode_Unix_WildCards_Gone_Wild.txt
+      for more information.
+    metadata:
+      cwe: "CWE-155: Improper Neutralization of Wildcards or Matching Symbols"
+      owasp: "A1: Injection"
+      source-url-open: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/injection_wildcard.py
+      references:
+        - https://www.defensecode.com/public/DefenseCode_Unix_WildCards_Gone_Wild.txt
+    languages: [python]
+    severity: WARNING
+
+  - id: telnetlib
+    pattern: telnetlib.$ANYTHING(...)
+    message: |
+      Telnet does not encrypt communications. Use SSH instead.
+    metadata:
+      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L208
+      cwe: "CWE-319: Cleartext Transmission of Sensitive Information"
+      owasp: "A3: Sensitive Data Exposure"
+      bandit-code: B312
+      references:
+        - https://docs.python.org/3/library/telnetlib.html
+    severity: WARNING
+    languages:
+      - python
+
+  - id: weak-ssl-version
+    patterns:
+      - pattern-either:
+          - pattern: ssl.PROTOCOL_SSLv2
+          - pattern: ssl.PROTOCOL_SSLv3
+          - pattern: ssl.PROTOCOL_TLSv1
+          - pattern: ssl.PROTOCOL_TLSv1_1
+          - pattern: pyOpenSSL.SSL.SSLv2_METHOD
+          - pattern: pyOpenSSL.SSL.SSLv23_METHOD
+          - pattern: pyOpenSSL.SSL.SSLv3_METHOD
+          - pattern: pyOpenSSL.SSL.TLSv1_METHOD
+          - pattern: pyOpenSSL.SSL.TLSv1_1_METHOD
+    message: |
+      An insecure SSL version was detected. TLS versions 1.0, 1.1, and all SSL versions
+      are considered weak encryption and are deprecated.
+      Use 'ssl.PROTOCOL_TLSv1_2' or higher.
+    metadata:
+      cwe: "CWE-326: Inadequate Encryption Strength"
+      owasp: "A3: Sensitive Data Exposure"
+      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/insecure_ssl_tls.py#L30
+      references:
+        - https://tools.ietf.org/html/rfc7568
+        - https://tools.ietf.org/id/draft-ietf-tls-oldversions-deprecate-02.html
+        - https://docs.python.org/3/library/ssl.html#ssl.PROTOCOL_TLSv1_2
+    languages: [python]
+    severity: WARNING
+
+  - id: avoid-pyyaml-load
+    metadata:
+      owasp: "A8: Insecure Deserialization"
+      cwe: "CWE-502: Deserialization of Untrusted Data"
+      references:
+        - https://github.com/yaml/pyyaml/wiki/PyYAML-yaml.load(input)-Deprecation
+        - https://nvd.nist.gov/vuln/detail/CVE-2017-18342
+    languages:
+      - python
+    message: |
+      Avoid using `load()`. `PyYAML.load` can create arbitrary Python
+      objects. A malicious actor could exploit this to run arbitrary
+      code. Use `safe_load()` instead.
+    fix: yaml.safe_load($FOO)
+    severity: ERROR
+    patterns:
+      - pattern-inside: |
+          import yaml
+          ...
+          yaml.load($FOO)
+      - pattern: yaml.load($FOO)
+
+  - id: avoid-unsafe-ruamel
+    metadata:
+      owasp: "A8: Insecure Deserialization"
+      cwe: "CWE-502: Deserialization of Untrusted Data"
+      references:
+        - https://yaml.readthedocs.io/en/latest/basicuse.html?highlight=typ
+    languages:
+      - python
+    message: |
+      Avoid using unsafe `ruamel.yaml.YAML()`. `ruamel.yaml.YAML` can
+      create arbitrary Python objects. A malicious actor could exploit
+      this to run arbitrary code. Use `YAML(typ='rt')` or
+      `YAML(typ='safe')` instead.
+    severity: ERROR
+    pattern-either:
+      - pattern: ruamel.yaml.YAML(..., typ='unsafe', ...)
+      - pattern: ruamel.yaml.YAML(..., typ='base', ...)
+
+  - id: avoid-pickle
+    metadata:
+      owasp: "A8: Insecure Deserialization"
+      cwe: "CWE-502: Deserialization of Untrusted Data"
+      references:
+        - https://docs.python.org/3/library/pickle.html
+        - https://davidhamann.de/2020/04/05/exploiting-python-pickle/
+    languages:
+      - python
+    message: |
+      Avoid using `pickle`, which is known to lead to code execution vulnerabilities.
+      When unpickling, the serialized data could be manipulated to run arbitrary code.
+      Instead, consider serializing the relevant data as JSON or a similar text-based
+      serialization format.
+    severity: WARNING
+    pattern-either:
+      - pattern: pickle.$FUNC(...)
+      - pattern: _pickle.$FUNC(...)
+  - id: avoid-cPickle
+    metadata:
+      owasp: "A8: Insecure Deserialization"
+      cwe: "CWE-502: Deserialization of Untrusted Data"
+      references:
+        - https://docs.python.org/3/library/pickle.html
+    languages:
+      - python
+    message: |
+      Avoid using `cPickle`, which is known to lead to code execution vulnerabilities.
+      When unpickling, the serialized data could be manipulated to run arbitrary code.
+      Instead, consider serializing the relevant data as JSON or a similar text-based
+      serialization format.
+    severity: WARNING
+    pattern: cPickle.$FUNC(...)
+  - id: avoid-dill
+    metadata:
+      owasp: "A8: Insecure Deserialization"
+      cwe: "CWE-502: Deserialization of Untrusted Data"
+      references:
+        - https://docs.python.org/3/library/pickle.html
+    languages:
+      - python
+    message: |
+      Avoid using `dill`, which uses `pickle`, which is known to lead to code execution vulnerabilities.
+      When unpickling, the serialized data could be manipulated to run arbitrary code.
+      Instead, consider serializing the relevant data as JSON or a similar text-based
+      serialization format.
+    severity: WARNING
+    pattern-either:
+      - pattern: dill.$FUNC(...)
+  - id: avoid-shelve
+    metadata:
+      owasp: "A8: Insecure Deserialization"
+      cwe: "CWE-502: Deserialization of Untrusted Data"
+      references:
+        - https://docs.python.org/3/library/pickle.html
+    languages:
+      - python
+    message: |
+      Avoid using `shelve`, which uses `pickle`, which is known to lead to code execution vulnerabilities.
+      When unpickling, the serialized data could be manipulated to run arbitrary code.
+      Instead, consider serializing the relevant data as JSON or a similar text-based
+      serialization format.
+    severity: WARNING
+    pattern-either:
+      - pattern: shelve.$FUNC(...)
+
+  - id: hardcoded-token
+    message: |
+      Hardcoded AWS access token detected. Use environment variables
+      to access tokens (e.g., os.environ.get(...)) or use non version-controlled
+      configuration files.
+    metadata:
+      cwe: "CWE-798: Use of Hard-coded Credentials"
+      owasp: "A2: Broken Authentication"
+      source-rule-url: https://pypi.org/project/flake8-boto3/
+      references:
+        - https://bento.dev/checks/boto3/hardcoded-access-token/
+        - https://aws.amazon.com/blogs/security/what-to-do-if-you-inadvertently-expose-an-aws-access-key/
+    patterns:
+      - pattern-either:
+          - pattern: $W(..., aws_secret_access_key="=~/^[A-Za-z0-9/+=]+$/", ...)
+          - pattern: $W(..., aws_access_key_id="=~/^AKI/", ...)
+          - pattern: $W(..., aws_session_token="...", ...)
+    languages: [python]
+    severity: WARNING
+
+  - id: insecure-cipher-algorithm-rc4
+    pattern: cryptography.hazmat.primitives.ciphers.algorithms.ARC4(...)
+    message: |
+      Detected RC4 cipher algorithm which is considered insecure. The algorithm has many
+      known vulnerabilities. Use AES instead.
+    metadata:
+      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L94
+      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
+      owasp: "A3: Sensitive Data Exposure"
+      bandit-code: B304
+      references:
+        - https://crypto.stackexchange.com/questions/853/google-is-using-rc4-but-isnt-rc4-considered-unsafe
+        - https://sweet32.info/
+    severity: WARNING
+    languages:
+      - python
+  - id: insecure-cipher-algorithm-blowfish
+    pattern: cryptography.hazmat.primitives.ciphers.algorithms.Blowfish(...)
+    message: |
+      Detected Blowfish cipher algorithm which is considered insecure. The algorithm has many
+      known vulnerabilities. Use AES instead.
+    metadata:
+      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L96
+      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
+      owasp: "A3: Sensitive Data Exposure"
+      bandit-code: B304
+      references:
+        - https://sweet32.info/
+    severity: WARNING
+    languages:
+      - python
+  - id: insecure-cipher-algorithm-idea
+    pattern: cryptography.hazmat.primitives.ciphers.algorithms.IDEA(...)
+    message: |
+      Detected IDEA cipher algorithm which is considered insecure. The algorithm is
+      considered weak and has been deprecated. Use AES instead.
+    metadata:
+      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L98
+      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
+      owasp: "A3: Sensitive Data Exposure"
+      bandit-code: B304
+      references:
+        - https://tools.ietf.org/html/rfc5469
+    severity: WARNING
+    languages:
+      - python
+
+  - id: insecure-cipher-mode-ecb
+    pattern: cryptography.hazmat.primitives.ciphers.modes.ECB(...)
+    message: |
+      Detected ECB cipher mode which is considered insecure. The algorithm can
+      potentially leak information about the plaintext. Use CBC mode instead.
+    metadata:
+      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L101
+      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
+      owasp: "A3: Sensitive Data Exposure"
+      bandit-code: B305
+      references:
+        - https://crypto.stackexchange.com/questions/20941/why-shouldnt-i-use-ecb-encryption
+    severity: WARNING
+    languages:
+      - python
+
+  - id: insecure-hash-algorithm-md5
+    pattern: cryptography.hazmat.primitives.hashes.MD5(...)
+    message: |
+      Detected MD5 hash algorithm which is considered insecure. MD5 is not
+      collision resistant and is therefore not suitable as a cryptographic
+      signature. Use SHA256 or SHA3 instead.
+    metadata:
+      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L59
+      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
+      owasp: "A3: Sensitive Data Exposure"
+      bandit-code: B303
+      references:
+        - https://tools.ietf.org/html/rfc6151
+        - https://crypto.stackexchange.com/questions/44151/how-does-the-flame-malware-take-advantage-of-md5-collision
+        - https://pycryptodome.readthedocs.io/en/latest/src/hash/sha3_256.html
+    severity: WARNING
+    languages:
+      - python
+  - id: insecure-hash-algorithm-sha1
+    pattern: cryptography.hazmat.primitives.hashes.SHA1(...)
+    message: |
+      Detected SHA1 hash algorithm which is considered insecure. SHA1 is not
+      collision resistant and is therefore not suitable as a cryptographic
+      signature. Use SHA256 or SHA3 instead.
+    metadata:
+      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L59
+      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
+      owasp: "A3: Sensitive Data Exposure"
+      bandit-code: B303
+      references:
+        - https://www.schneier.com/blog/archives/2012/10/when_will_we_se.html
+        - https://www.trendmicro.com/vinfo/us/security/news/vulnerabilities-and-exploits/sha-1-collision-signals-the-end-of-the-algorithm-s-viability
+        - http://2012.sharcs.org/slides/stevens.pdf
+        - https://pycryptodome.readthedocs.io/en/latest/src/hash/sha3_256.html
+    severity: WARNING
+    languages:
+      - python
+
+  - id: insufficient-dsa-key-size
+    patterns:
+      - pattern-either:
+          - pattern: cryptography.hazmat.primitives.asymmetric.dsa.generate_private_key(..., key_size=$SIZE, ...)
+          - pattern: cryptography.hazmat.primitives.asymmetric.dsa.generate_private_key($SIZE, ...)
+      - metavariable-comparison:
+          metavariable: $SIZE
+          comparison: $SIZE < 2048
+    message: |
+      Detected an insufficient key size for DSA. NIST recommends
+      a key size of 2048 or higher.
+    metadata:
+      cwe: "CWE-326: Inadequate Encryption Strength"
+      owasp: "A3: Sensitive Data Exposure"
+      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/weak_cryptographic_key.py
+      references:
+        - https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-57Pt3r1.pdf
+    languages: [python]
+    severity: WARNING
+
+  - id: insufficient-ec-key-size
+    patterns:
+      - pattern-inside: cryptography.hazmat.primitives.asymmetric.ec.generate_private_key(...)
+      - pattern-either:
+          - pattern: cryptography.hazmat.primitives.asymmetric.ec.SECP192R1
+          - pattern: cryptography.hazmat.primitives.asymmetric.ec.SECT163K1
+          - pattern: cryptography.hazmat.primitives.asymmetric.ec.SECT163R2
+    message: |
+      Detected an insufficient curve size for EC. NIST recommends
+      a key size of 224 or higher. For example, use 'ec.SECP256R1'.
+    metadata:
+      cwe: "CWE-326: Inadequate Encryption Strength"
+      owasp: "A3: Sensitive Data Exposure"
+      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/weak_cryptographic_key.py
+      references:
+        - https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-57Pt3r1.pdf
+        - https://cryptography.io/en/latest/hazmat/primitives/asymmetric/ec/#elliptic-curves
+    languages: [python]
+    severity: WARNING
+
+  - id: insufficient-rsa-key-size
+    patterns:
+      - pattern-either:
+          - pattern: cryptography.hazmat.primitives.asymmetric.rsa.generate_private_key(..., key_size=$SIZE, ...)
+          - pattern: cryptography.hazmat.primitives.asymmetric.rsa.generate_private_key($EXP, $SIZE, ...)
+      - metavariable-comparison:
+          metavariable: $SIZE
+          comparison: $SIZE < 2048
+    message: |
+      Detected an insufficient key size for RSA. NIST recommends
+      a key size of 2048 or higher.
+    metadata:
+      cwe: "CWE-326: Inadequate Encryption Strength"
+      owasp: "A3: Sensitive Data Exposure"
+      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/weak_cryptographic_key.py
+      references:
+        - https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-57Pt3r1.pdf
+    languages: [python]
+    severity: WARNING
+
+  - id: dangerous-template-string
+    patterns:
+      - pattern-either:
+          - pattern: |
+              $V = "...".format(...)
+              ...
+              flask.render_template_string($V, ...)
+          - pattern: |
+              $V = "...".format(...)
+              ...
+              return flask.render_template_string($V, ...), $MORE
+          - pattern: |
+              $V = "..." % $S
+              ...
+              flask.render_template_string($V, ...)
+          - pattern: |
+              $V = "..." % $S
+              ...
+              return flask.render_template_string($V, ...), $MORE
+          - pattern: |
+              $V = "..."
+              ...
+              $V += $O
+              ...
+              flask.render_template_string($V, ...)
+          - pattern: |
+              $V = "..."
+              ...
+              $V += $O
+              ...
+              return flask.render_template_string($V, ...), $MORE
+          - pattern: |
+              $V = f"...{$X}..."
+              ...
+              flask.render_template_string($V, ...)
+          - pattern: |
+              $V = f"...{$X}..."
+              ...
+              return flask.render_template_string($V, ...), $CODE
+    message: |
+      Found a template created with string formatting.
+      This is susceptible to server-side template injection
+      and cross-site scripting attacks.
+    metadata:
+      cwe: "CWE-96: Improper Neutralization of Directives in Statically Saved Code ('Static Code Injection')"
+      owasp: "A1: Injection"
+      references:
+        - https://nvisium.com/blog/2016/03/09/exploring-ssti-in-flask-jinja2.html
+        - https://pequalsnp-team.github.io/cheatsheet/flask-jinja2-ssti
+    languages: [python]
+    severity: ERROR
+
+  - id: insecure-deserialization
+    metadata:
+      owasp: "A8: Insecure Deserialization"
+      cwe: "CWE-502: Deserialization of Untrusted Data"
+      references:
+        - https://docs.python.org/3/library/pickle.html
+    message: |
+      Detected the use of an insecure deserizliation library in a Flask route. These libraries
+      are prone to code execution vulnerabilities. Ensure user data does not enter this function.
+      To fix this, try to avoid serializing whole objects. Consider instead using a serializer
+      such as JSON.
+    languages:
+      - python
+    severity: ERROR
+    patterns:
+      - pattern-inside: |
+          @app.route(...)
+          def $X(...):
+            ...
+      - pattern-not: $MODULE.$FUNC("...")
+      - pattern-not: $MODULE.$FUNC(open("...", ...))
+      - pattern-either:
+          - pattern: pickle.$FUNC(...)
+          - pattern: _pickle.$FUNC(...)
+          - pattern: cPickle.$FUNC(...)
+          - pattern: dill.$FUNC(...)
+          - pattern: shelve.$FUNC(...)
+          - pattern: yaml.load(...)
+
+  - id: open-redirect
+    patterns:
+      - pattern-inside: |
+          @$APP.route(...)
+          def $X():
+            ...
+      - pattern-not-inside: |
+          ...
+          if <... werkzeug.urls.url_parse($V) ...>:
+            ...
+      - pattern-either:
+          - pattern: flask.redirect(<... flask.request.$W.get(...) ...>, ...)
+          - pattern: flask.redirect(<... flask.request.$W[...] ...>, ...)
+          - pattern: flask.redirect(<... flask.request.$W(...) ...>, ...)
+          - pattern: flask.redirect(<... flask.request.$W ...>, ...)
+          - pattern: |
+              $V = flask.request.$W.get(...)
+              ...
+              flask.redirect(<... $V ...>, ...)
+          - pattern: |
+              $V = flask.request.$W[...]
+              ...
+              flask.redirect(<... $V ...>, ...)
+          - pattern: |
+              $V = flask.request.$W(...)
+              ...
+              flask.redirect(<... $V ...>, ...)
+          - pattern: |
+              $V = flask.request.$W
+              ...
+              flask.redirect(<... $V ...>, ...)
+    message: |
+      Data from request is passed to redirect().
+      This is an open redirect and could be exploited.
+      Consider using 'url_for()' to generate links to known locations.
+      If you must use a URL to unknown pages, consider using 'urlparse()'
+      or similar and checking if the 'netloc' property is the same as
+      your site's host name. See the references for more information.
+    metadata:
+      cwe: "CWE-601: URL Redirection to Untrusted Site ('Open Redirect')"
+      owasp: "A1: Injection"
+      references:
+        - https://flask-login.readthedocs.io/en/latest/#login-example
+        - https://cheatsheetseries.owasp.org/cheatsheets/Unvalidated_Redirects_and_Forwards_Cheat_Sheet.html#dangerous-url-redirect-example-1
+        - https://docs.python.org/3/library/urllib.parse.html#url-parsing
+    languages: [python]
+    severity: ERROR
+  # For Flask app to serve file securely, it should use `send_from_directory` method
+  # The other methods like `send_file` or `send_static_file` are not recommended per
+  # https://stackoverflow.com/questions/20646822/how-to-serve-static-files-in-flask
+
+  - id: avoid_send_file_without_path_sanitization
+    patterns:
+      - pattern-inside: |
+          @app.route(...)
+          def $X(filename):
+            ...
+      - pattern-either:
+          - pattern: flask.send_file(filename, ...)
+    message:
+      Looks like `filename` could flow to `flask.send_file()` function. Make sure to properly sanitize filename or use
+      `flask.send_from_directory`
+    metadata:
+      cwe: "CWE-73: External Control of File Name or Path"
+      owasp: "A1: Injection"
+    languages: [python]
+    severity: WARNING
+
+  - id: unescaped-template-extension
+    message: |
+      Flask does not automatically escape Jinja templates unless they have
+      .html, .htm, .xml, or .xhtml extensions. This could lead to XSS attacks.
+      Use .html, .htm, .xml, or .xhtml for your template extensions.
+      See https://flask.palletsprojects.com/en/1.1.x/templating/#jinja-setup
+      for more information.
+    metadata:
+      cwe: "CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')"
+      owasp: "A7: Cross-Site Scripting (XSS)"
+      source-rule-url: https://pypi.org/project/flake8-flask/
+      references:
+        - https://flask.palletsprojects.com/en/1.1.x/templating/#jinja-setup
+        - https://blog.r2c.dev/2020/bento-check-unescaped-template-extensions-in-flask/
+        - https://bento.dev/checks/flask/unescaped-file-extension/
+    patterns:
+      - pattern-not: flask.render_template("=~/.+\.html$/", ...)
+      - pattern-not: flask.render_template("=~/.+\.xml$/", ...)
+      - pattern-not: flask.render_template("=~/.+\.htm$/", ...)
+      - pattern-not: flask.render_template("=~/.+\.xhtml$/", ...)
+      - pattern-not: flask.render_template($X + "=~/\.html$/", ...)
+      - pattern-not: flask.render_template($X + "=~/\.xml$/", ...)
+      - pattern-not: flask.render_template($X + "=~/\.htm$/", ...)
+      - pattern-not: flask.render_template($X + "=~/\.xhtml$/", ...)
+      - pattern-not: flask.render_template("=~/.+\.html$/" % $X, ...)
+      - pattern-not: flask.render_template("=~/.+\.xml$/" % $X, ...)
+      - pattern-not: flask.render_template("=~/.+\.htm$/" % $X, ...)
+      - pattern-not: flask.render_template("=~/.+\.xhtml$/" % $X, ...)
+      - pattern-not: flask.render_template("=~/.+\.html$/".format(...), ...)
+      - pattern-not: flask.render_template("=~/.+\.xml$/".format(...), ...)
+      - pattern-not: flask.render_template("=~/.+\.htm$/".format(...), ...)
+      - pattern-not: flask.render_template("=~/.+\.xhtml$/".format(...), ...)
+      - pattern-not: flask.render_template($TEMPLATE)
+      - pattern-either:
+          - pattern: flask.render_template("...", ...)
+          - pattern: flask.render_template($X + "...", ...)
+          - pattern: flask.render_template("..." % $Y, ...)
+          - pattern: flask.render_template("...".format(...), ...)
+    languages: [python]
+    severity: WARNING
+
+  - id: response-contains-unsanitized-input
+    patterns:
+      - pattern-either:
+          - pattern: |
+              $X = flask.request.args.get(...)
+              ...
+              flask.make_response("...".format($X))
+          - pattern: |
+              $X = flask.request.args.get(...)
+              ...
+              flask.make_response(f"...{$X}...")
+          - pattern: |
+              $X = flask.request.args.get(...)
+              ...
+              flask.make_response(f"...{$X}")
+          - pattern: |
+              $X = flask.request.args.get(...)
+              ...
+              flask.make_response(f"{$X}...")
+    message: |
+      Flask response reflects unsanitized user input. This could lead to a
+      cross-site scripting vulnerability (https://owasp.org/www-community/attacks/xss/)
+      in which an attacker causes arbitrary code to be executed in the user's browser.
+      To prevent, please sanitize the user input, e.g. by rendering the response
+      in a Jinja2 template (see considerations in https://flask.palletsprojects.com/en/1.0.x/security/).
+    metadata:
+      cwe: "CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')"
+      owasp: "A7: Cross-Site Scripting (XSS)"
+      references:
+        - https://flask.palletsprojects.com/en/1.0.x/security/
+        - https://owasp.org/www-community/attacks/xss/
+    languages: [python]
+    severity: WARNING
+
+  - id: jwt-python-exposed-credentials
+    languages:
+      - python
+    metadata:
+      cwe: "CWE-522: Insufficiently Protected Credentials"
+      owasp: "A2: Broken Authentication"
+      source-rule-url: https://r2c.dev/blog/2020/hardcoded-secrets-unverified-tokens-and-other-common-jwt-mistakes/
+      references:
+        - https://cwe.mitre.org/data/definitions/522.html
+    message: |
+      Password is exposed through JWT token payload. This is not encrypted and
+      the password could be compromised. Do not store passwords in JWT tokens.
+    pattern-either:
+      - pattern: |
+          jwt.encode({...,"password":$P,...},...)
+      - pattern: |
+          $PAYLOAD = {...,"password":$P,...}
+          ...
+          jwt.encode($PAYLOAD,...)
+    severity: ERROR
+
+  - id: jwt-python-hardcoded-secret
+    message: |
+      Hardcoded JWT secret or private key is used.
+      This is a Insufficiently Protected Credentials weakness: https://cwe.mitre.org/data/definitions/522.html
+      Consider using an appropriate security mechanism to protect the credentials (e.g. keeping secrets in environment variables)
+    metadata:
+      cwe: "CWE-522: Insufficiently Protected Credentials"
+      owasp: "A2: Broken Authentication"
+      source-rule-url: https://r2c.dev/blog/2020/hardcoded-secrets-unverified-tokens-and-other-common-jwt-mistakes/
+    pattern-either:
+      - pattern: |
+          jwt.encode($X, "...", ...)
+      - pattern: |
+          $SECRET = "..."
+          ...
+          jwt.encode($X, $SECRET, ...)
+    languages: [python]
+    severity: ERROR
+
+  - id: jwt-python-none-alg
+    message: |
+      Detected use of the 'none' algorithm in a JWT token.
+      The 'none' algorithm assumes the integrity of the token has already
+      been verified. This would allow a malicious actor to forge a JWT token
+      that will automatically be verified. Do not explicitly use the 'none'
+      algorithm. Instead, use an algorithm such as 'HS256'.
+    metadata:
+      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
+      owasp: "A2: Broken Authentication"
+      source-rule-url: https://r2c.dev/blog/2020/hardcoded-secrets-unverified-tokens-and-other-common-jwt-mistakes/
+    languages: [python]
+    severity: ERROR
+    pattern-either:
+      - pattern: |
+          jwt.encode(...,algorithm="none",...)
+      - pattern: |-
+          jwt.decode(...,algorithms=[...,"none",...],...)
+
+  - id: unverified-jwt-decode
+    pattern: |
+      jwt.decode(..., verify=False, ...)
+    message: |
+      Detected JWT token decoded with 'verify=False'. This bypasses any integrity
+      checks for the token which means the token could be tampered with by
+      malicious actors. Ensure that the JWT token is verified.
+    metadata:
+      owasp: "A5: Broken Authentication"
+      cwe: "CWE-287: Improper Authentication"
+      references:
+        - https://github.com/we45/Vulnerable-Flask-App/blob/752ee16087c0bfb79073f68802d907569a1f0df7/app/app.py#L96
+    fix-regex:
+      regex: (verify\s*=\s*)False
+      replacement: \1True
+    severity: ERROR
+    languages:
+      - python
+
+  - id: insecure-hash-algorithm-md5
+    pattern: hashlib.md5(...)
+    message: |
+      Detected MD5 hash algorithm which is considered insecure. MD5 is not
+      collision resistant and is therefore not suitable as a cryptographic
+      signature. Use SHA256 or SHA3 instead.
+    metadata:
+      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L59
+      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
+      owasp: "A3: Sensitive Data Exposure"
+      bandit-code: B303
+      references:
+        - https://tools.ietf.org/html/rfc6151
+        - https://crypto.stackexchange.com/questions/44151/how-does-the-flame-malware-take-advantage-of-md5-collision
+        - https://pycryptodome.readthedocs.io/en/latest/src/hash/sha3_256.html
+    severity: WARNING
+    languages:
+      - python
+  - id: insecure-hash-algorithm-sha1
+    pattern: hashlib.sha1(...)
+    message: |
+      Detected SHA1 hash algorithm which is considered insecure. SHA1 is not
+      collision resistant and is therefore not suitable as a cryptographic
+      signature. Use SHA256 or SHA3 instead.
+    metadata:
+      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L59
+      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
+      owasp: "A3: Sensitive Data Exposure"
+      bandit-code: B303
+      references:
+        - https://www.schneier.com/blog/archives/2012/10/when_will_we_se.html
+        - https://www.trendmicro.com/vinfo/us/security/news/vulnerabilities-and-exploits/sha-1-collision-signals-the-end-of-the-algorithm-s-viability
+        - http://2012.sharcs.org/slides/stevens.pdf
+        - https://pycryptodome.readthedocs.io/en/latest/src/hash/sha3_256.html
+    severity: WARNING
+    languages:
+      - python
+
+  - id: insecure-hash-function
+    patterns:
+      - pattern-either:
+          - pattern: hashlib.new("=~/[M|m][D|d][4|5]/", ...)
+          - pattern: hashlib.new(..., name="=~/[M|m][D|d][4|5]/", ...)
+    message: |
+      Detected use of an insecure MD4 or MD5 hash function.
+      These functions have known vulnerabilities and are considered deprecated.
+      Consider using 'SHA256' or a similar function instead.
+    metadata:
+      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
+      owasp: "A3: Sensitive Data Exposure"
+      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/hashlib_new_insecure_functions.py
+      references:
+        - https://tools.ietf.org/html/rfc6151
+        - https://crypto.stackexchange.com/questions/44151/how-does-the-flame-malware-take-advantage-of-md5-collision
+        - https://pycryptodome.readthedocs.io/en/latest/src/hash/sha3_256.html
+    languages: [python]
+    severity: WARNING
+
+  - id: unquoted-csv-writer
+    patterns:
+      - pattern-not: csv.writer(..., quoting=csv.QUOTE_ALL, ...)
+      - pattern: csv.writer(...)
+    message: Found an unquoted CSV writer. This is susceptible to injection. Use 'quoting=csv.QUOTE_ALL'.
+    metadata:
+      cwe: "CWE-1236: Improper Neutralization of Formula Elements in a CSV File"
+      owasp: "A1: Injection"
+      references:
+        - https://affinity-it-security.com/how-to-prevent-csv-injection/
+    fix-regex:
+      regex: (.*)\)
+      replacement: \1, quoting=csv.QUOTE_ALL)
+    languages: [python]
+    severity: ERROR
+
+  - id: unverified-ssl-context
+    pattern: ssl._create_unverified_context(...)
+    message: |
+      Unverified SSL context detected. This will permit insecure connections without verifying
+      SSL certificates. Use 'ssl.create_default_context()' instead.
+    metadata:
+      owasp: "A6: Security Misconfiguration"
+      cwe: "CWE-295: Improper Certificate Validation"
+      references:
+        - https://docs.python.org/3/library/ssl.html#ssl-security
+        - https://docs.python.org/3/library/http.client.html#http.client.HTTPSConnection
+    severity: ERROR
+    languages:
+      - python
+
+  - id: use-defused-xml
+    pattern-either:
+      - pattern: import xml
+    fix-regex:
+      regex: xml
+      replacement: defusedxml
+    metadata:
+      owasp: "A4: XML External Entities (XXE)"
+      cwe: "CWE-611: Improper Restriction of XML External Entity Reference"
+      references:
+        - https://docs.python.org/3/library/xml.html
+        - https://github.com/tiran/defusedxml
+    message: |
+      Found use of the native Python XML libraries, which is vulnerable to XML external entity (XXE)
+      attacks. The Python documentation recommends the 'defusedxml' library instead. Use 'defusedxml'.
+      See https://github.com/tiran/defusedxml for more information.
+    languages: [python]
+    severity: ERROR
+
+  - id: use-defused-xmlrpc
+    pattern-either:
+      - pattern: import xmlrpclib
+      - pattern: import SimpleXMLRPCServer
+      # Python 3
+      - pattern: import xmlrpc
+    message: |
+      Detected use of xmlrpc. xmlrpc is not inherently safe from vulnerabilities.
+      Use defusedxml.xmlrpc instead.
+    metadata:
+      cwe: "CWE-776: Improper Restriction of Recursive Entity References in DTDs ('XML Entity Expansion')"
+      owasp: "A4: XML External Entities (XXE)"
+      source-rule-url: https://github.com/PyCQA/bandit/blob/07f84cb5f5e7c1055e6feaa0fe93afa471de0ac3/bandit/blacklists/imports.py#L160
+      references:
+        - https://pypi.org/project/defusedxml/
+        - https://docs.python.org/3/library/xml.html#xml-vulnerabilities
+    severity: ERROR
+    languages:
+      - python
+
+  - id: insecure-cipher-algorithm-rc2
+    patterns:
+      - pattern-either:
+          - pattern: Cryptodome.Cipher.ARC2.new(...)
+          - pattern: Crypto.Cipher.ARC2.new
+    message: |
+      Detected RC2 cipher algorithm which is considered insecure. The algorithm has known vulnerabilities and is difficult to use securely. Use AES instead.
+    metadata:
+      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L84
+      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
+      owasp: "A3: Sensitive Data Exposure"
+      bandit-code: B304
+      references:
+        - https://security.stackexchange.com/questions/93924/is-rc2-cbc-at-all-secure
+        - https://sweet32.info/
+    severity: WARNING
+    languages:
+      - python
+  - id: insecure-cipher-algorithm-rc4
+    patterns:
+      - pattern-either:
+          - pattern: Cryptodome.Cipher.ARC4.new(...)
+          - pattern: Crypto.Cipher.ARC4.new(...)
+    message: |
+      Detected RC4 cipher algorithm which is considered insecure. The algorithm has many
+      known vulnerabilities. Use AES instead.
+    metadata:
+      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L84
+      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
+      owasp: "A3: Sensitive Data Exposure"
+      bandit-code: B304
+      references:
+        - https://crypto.stackexchange.com/questions/853/google-is-using-rc4-but-isnt-rc4-considered-unsafe
+        - https://sweet32.info/
+    severity: WARNING
+    languages:
+      - python
+  - id: insecure-cipher-algorithm-blowfish
+    patterns:
+      - pattern-either:
+          - pattern: Cryptodome.Cipher.Blowfish.new(...)
+          - pattern: Crypto.Cipher.Blowfish.new(...)
+    message: |
+      Detected Blowfish cipher algorithm which is considered insecure. The algorithm has many
+      known vulnerabilities. Use AES instead.
+    metadata:
+      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L84
+      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
+      owasp: "A3: Sensitive Data Exposure"
+      bandit-code: B304
+      references:
+        - https://sweet32.info/
+    severity: WARNING
+    languages:
+      - python
+  - id: insecure-cipher-algorithm-des
+    patterns:
+      - pattern-either:
+          - pattern: Cryptodome.Cipher.DES.new(...)
+          - pattern: Crypto.Cipher.DES.new(...)
+    message: |
+      Detected DES cipher algorithm which is considered insecure. The algorithm is
+      considered weak and has been deprecated. Use AES instead.
+    metadata:
+      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L84
+      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
+      owasp: "A3: Sensitive Data Exposure"
+      bandit-code: B304
+      references:
+        - https://tools.ietf.org/html/rfc5469
+    severity: WARNING
+    languages:
+      - python
+  - id: insecure-cipher-algorithm-xor
+    patterns:
+      - pattern-either:
+          - pattern: Cryptodome.Cipher.XOR.new(...)
+          - pattern: Crypto.Cipher.XOR.new(...)
+    message: |
+      Detected XOR cipher algorithm which is considered insecure. This algorithm
+      is not cryptographically secure and can be reversed easily. Use AES instead.
+    metadata:
+      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L84
+      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
+      owasp: "A3: Sensitive Data Exposure"
+      bandit-code: B304
+      references:
+        - https://stackoverflow.com/questions/1135186/whats-wrong-with-xor-encryption
+    severity: WARNING
+    languages:
+      - python
+
+  - id: insecure-hash-algorithm-md2
+    patterns:
+      - pattern-either:
+          - pattern: Crypto.Hash.MD2.new(...)
+          - pattern: Cryptodome.Hash.MD2.new (...)
+    message: |
+      Detected MD2 hash algorithm which is considered insecure. This algorithm
+      has many known vulnerabilities and has been deprecated. Use SHA256 or SHA3 instead.
+    metadata:
+      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L59
+      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
+      owasp: "A3: Sensitive Data Exposure"
+      references:
+        - https://tools.ietf.org/html/rfc6149
+        - https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2009-2409
+        - https://pycryptodome.readthedocs.io/en/latest/src/hash/sha3_256.html
+    severity: WARNING
+    languages:
+      - python
+  - id: insecure-hash-algorithm-md4
+    patterns:
+      - pattern-either:
+          - pattern: Crypto.Hash.MD4.new(...)
+          - pattern: Cryptodome.Hash.MD4.new (...)
+    message: |
+      Detected MD4 hash algorithm which is considered insecure. This algorithm
+      has many known vulnerabilities and has been deprecated. Use SHA256 or SHA3 instead.
+    metadata:
+      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L59
+      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
+      owasp: "A3: Sensitive Data Exposure"
+      references:
+        - https://tools.ietf.org/html/rfc6150
+        - https://pycryptodome.readthedocs.io/en/latest/src/hash/sha3_256.html
+    severity: WARNING
+    languages:
+      - python
+  - id: insecure-hash-algorithm-md5
+    patterns:
+      - pattern-either:
+          - pattern: Crypto.Hash.MD5.new(...)
+          - pattern: Cryptodome.Hash.MD5.new (...)
+    message: |
+      Detected MD5 hash algorithm which is considered insecure. MD5 is not
+      collision resistant and is therefore not suitable as a cryptographic
+      signature. Use SHA256 or SHA3 instead.
+    metadata:
+      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L59
+      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
+      owasp: "A3: Sensitive Data Exposure"
+      references:
+        - https://tools.ietf.org/html/rfc6151
+        - https://crypto.stackexchange.com/questions/44151/how-does-the-flame-malware-take-advantage-of-md5-collision
+        - https://pycryptodome.readthedocs.io/en/latest/src/hash/sha3_256.html
+    severity: WARNING
+    languages:
+      - python
+  - id: insecure-hash-algorithm-sha1
+    patterns:
+      - pattern-either:
+          - pattern: Crypto.Hash.SHA.new(...)
+          - pattern: Cryptodome.Hash.SHA.new (...)
+    message: |
+      Detected SHA1 hash algorithm which is considered insecure. SHA1 is not
+      collision resistant and is therefore not suitable as a cryptographic
+      signature. Use SHA256 or SHA3 instead.
+    metadata:
+      source-rule-url: https://github.com/PyCQA/bandit/blob/d5f8fa0d89d7b11442fc6ec80ca42953974354c8/bandit/blacklists/calls.py#L59
+      cwe: "CWE-327: Use of a Broken or Risky Cryptographic Algorithm"
+      owasp: "A3: Sensitive Data Exposure"
+      references:
+        - https://www.schneier.com/blog/archives/2012/10/when_will_we_se.html
+        - https://www.trendmicro.com/vinfo/us/security/news/vulnerabilities-and-exploits/sha-1-collision-signals-the-end-of-the-algorithm-s-viability
+        - http://2012.sharcs.org/slides/stevens.pdf
+        - https://pycryptodome.readthedocs.io/en/latest/src/hash/sha3_256.html
+    severity: WARNING
+    languages:
+      - python
+
+  - id: insufficient-dsa-key-size
+    patterns:
+      - pattern-either:
+          - pattern: Crypto.PublicKey.DSA.generate(..., bits=$SIZE, ...)
+          - pattern: Crypto.PublicKey.DSA.generate($SIZE, ...)
+          - pattern: Cryptodome.PublicKey.DSA.generate(..., bits=$SIZE, ...)
+          - pattern: Cryptodome.PublicKey.DSA.generate($SIZE, ...)
+      - metavariable-comparison:
+          metavariable: $SIZE
+          comparison: $SIZE < 2048
+    message: |
+      Detected an insufficient key size for DSA. NIST recommends
+      a key size of 2048 or higher.
+    metadata:
+      cwe: "CWE-326: Inadequate Encryption Strength"
+      owasp: "A3: Sensitive Data Exposure"
+      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/weak_cryptographic_key.py
+      references:
+        - https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-57Pt3r1.pdf
+    languages: [python]
+    severity: WARNING
+
+  - id: insufficient-rsa-key-size
+    patterns:
+      - pattern-either:
+          - pattern: Crypto.PublicKey.RSA.generate(..., bits=$SIZE, ...)
+          - pattern: Crypto.PublicKey.RSA.generate($SIZE, ...)
+          - pattern: Cryptodome.PublicKey.RSA.generate(..., bits=$SIZE, ...)
+          - pattern: Cryptodome.PublicKey.RSA.generate($SIZE, ...)
+      - metavariable-comparison:
+          metavariable: $SIZE
+          comparison: $SIZE < 2048
+    message: |
+      Detected an insufficient key size for RSA. NIST recommends
+      a key size of 2048 or higher.
+    metadata:
+      cwe: "CWE-326: Inadequate Encryption Strength"
+      owasp: "A3: Sensitive Data Exposure"
+      source-rule-url: https://github.com/PyCQA/bandit/blob/b1411bfb43795d3ffd268bef17a839dee954c2b1/bandit/plugins/weak_cryptographic_key.py
+      references:
+        - https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-57Pt3r1.pdf
+    languages: [python]
+    severity: WARNING
+
+  - id: disabled-cert-validation
+    patterns:
+      - pattern-either:
+          - pattern: requests.put(..., verify=False, ...)
+          - pattern: requests.patch(..., verify=False, ...)
+          - pattern: requests.delete(..., verify=False, ...)
+          - pattern: requests.head(..., verify=False, ...)
+          - pattern: requests.options(..., verify=False, ...)
+          - pattern: requests.request(..., verify=False, ...)
+          - pattern: requests.get(..., verify=False, ...)
+          - pattern: requests.post(..., verify=False, ...)
+    message: |
+      Certificate verification has been explicitly disabled. This
+      permits insecure connections to insecure servers. Re-enable
+      certification validation.
+    metadata:
+      cwe: "CWE-295: Improper Certificate Validation"
+      owasp: "A3: Sensitive Data Exposure"
+      references:
+        - https://stackoverflow.com/questions/41740361/is-it-safe-to-disable-ssl-certificate-verification-in-pythonss-requests-lib
+    languages: [python]
+    severity: ERROR
+
+  - id: no-auth-over-http
+    patterns:
+      - pattern-either:
+          - pattern: requests.$W("=~/http:\/\/.*/", ..., auth=$X, ...)
+          - pattern: |
+              $URL = "=~/http:\/\/.../"
+              ...
+              requests.$W($URL, ..., auth=$X, ...)
+    fix-regex:
+      regex: http:\/\/
+      replacement: https://
+      count: 1
+    message: |
+      Authentication detected over HTTP. HTTP does not provide any
+      encryption or protection for these authentication credentials.
+      This may expose these credentials to unauthhorized parties.
+      Use 'https://' instead.
+    metadata:
+      cwe: "CWE-523: Unprotected Transport of Credentials"
+      owasp: "A2: Broken Authentication"
+      source-rule-url: https://pypi.org/project/flake8-flask/
+      references:
+        - https://blog.r2c.dev/2020/bento-check-no-auth-over-http/
+        - https://bento.dev/checks/requests/no-auth-over-http/
+    languages: [python]
+    severity: ERROR
+
+  - id: string-concat
+    languages: [python]
+    severity: WARNING
+    message: |
+      Detected string concatenation or formatting in a call to a command via 'sh'.
+      This could be a command injection vulnerability if the data is user-controlled.
+      Instead, use a list and append the argument.
+    metadata:
+      cwe: "CWE-78: Improper Neutralization of Special Elements used in an OS Command ('OS Command Injection')"
+      owasp: "A1: Injection"
+    pattern-either:
+      - pattern: sh.$BIN($X + $Y)
+      - pattern: sh.$BIN($X.format(...))
+      - pattern: sh.$BIN(f"...{...}...")
+
+  - id: sqlalchemy-sql-injection
+    patterns:
+      - pattern-either:
+          - pattern: |
+              def $FUNC(...,$VAR,...):
+                ...
+                $SESSION.query(...).$SQLFUNC("...".$FORMATFUNC(...,$VAR,...))
+          - pattern: |
+              def $FUNC(...,$VAR,...):
+                ...
+                $SESSION.query.join(...).$SQLFUNC("...".$FORMATFUNC(...,$VAR,...))
+          - pattern: |
+              def $FUNC(...,$VAR,...):
+                ...
+                $SESSION.query.$SQLFUNC("...".$FORMATFUNC(...,$VAR,...))
+          - pattern: |
+              def $FUNC(...,$VAR,...):
+                ...
+                query.$SQLFUNC("...".$FORMATFUNC(...,$VAR,...))
+      - metavariable-regex:
+          metavariable: $SQLFUNC
+          regex: (group_by|order_by|distinct|having|filter)
+      - metavariable-regex:
+          metavariable: $FORMATFUNC
+          regex: (?!bindparams)
+    message: |
+      Distinct, Having, Group_by, Order_by, and Filter in SQLAlchemy can cause sql injections
+      if the developer inputs raw SQL into the before-mentioned clauses.
+      This pattern captures relevant cases in which the developer inputs raw SQL into the distinct, having, group_by, order_by or filter clauses and
+      injects user-input into the raw SQL with any function besides "bindparams". Use bindParams to securely bind user-input
+      to SQL statements.
+    fix-regex:
+      regex: format
+      replacement: bindparams
+    languages:
+      - python
+    severity: WARNING
```

### Comparing `simplesecurity-2022/simplesecurity/types.py` & `simplesecurity-2023/simplesecurity/types.py`

 * *Files identical despite different names*

### Comparing `simplesecurity-2022/setup.py` & `simplesecurity-2023/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 packages = \
 ['simplesecurity']
 
 package_data = \
 {'': ['*']}
 
 extras_require = \
-{'full': ['poetry>=1.1.10,<2',
-          'bandit>=1.7.0,<2',
-          'safety>=1.10.3,<2',
+{'full': ['poetry>=1.5.1,<2',
+          'bandit>=1.7.5,<2',
+          'safety>=2.3.5,<3',
           'dodgy>=0.2.1,<2',
-          'dlint>=0.11.0,<2',
-          'semgrep>=0.67.0,<2']}
+          'dlint>=0.14.1,<2',
+          'semgrep>=1.29.0,<2']}
 
 entry_points = \
 {'console_scripts': ['simplesecurity = simplesecurity:cli']}
 
 setup_kwargs = {
     'name': 'simplesecurity',
-    'version': '2022',
+    'version': '2023',
     'description': 'Combine multiple popular python security tools and generate reports or output into different formats',
-    'long_description': '[![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../)\n[![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../)\n[![Issues](https://img.shields.io/github/issues/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../issues)\n[![License](https://img.shields.io/github/license/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](/LICENSE.md)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../commits/master)\n[![Last commit](https://img.shields.io/github/last-commit/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../commits/master)\n[![PyPI Downloads](https://img.shields.io/pypi/dm/simplesecurity.svg?style=for-the-badge)](https://pypistats.org/packages/simplesecurity)\n[![PyPI Total Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=total%20downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fsimplesecurity)](https://pepy.tech/project/simplesecurity)\n[![PyPI Version](https://img.shields.io/pypi/v/simplesecurity.svg?style=for-the-badge)](https://pypi.org/project/simplesecurity)\n\n<!-- omit in toc -->\n# SimpleSecurity\n\n<img src="readme-assets/icons/name.png" alt="Project Icon" width="750">\n\nCombine multiple popular python security tools and generate reports or output\ninto different formats\n\nPlugins (these require the plugin executable in the system path. e.g. bandit\nrequires bandit to be in the system path...)\n\n- bandit\n- safety\n- dodgy\n- dlint\n- semgrep\n\nFormats\n\n- ansi (for terminal)\n- json\n- markdown\n- csv\n- sarif\n\n## Example Use\n\nSee below for the output if you run `simplesecurity` in this directory\n\n<img src="readme-assets/screenshots/sec.svg" width="500px">\n\n### Help\n\n```txt\nusage: __main__.py [-h] [--format FORMAT] [--plugin PLUGIN] [--file FILE] [--level LEVEL] [--confidence CONFIDENCE]\n                   [--no-colour] [--high-contrast] [--fast] [--zero]\n\nCombine multiple popular python security tools...\n\nand generate reports or output into different formats.\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --format FORMAT, -f FORMAT\n                        Output format. One of ansi, json, markdown, csv. default=ansi\n  --plugin PLUGIN, -p PLUGIN\n                        Plugin to use. One of bandit, safety, dodgy, dlint, semgrep, all, default=all\n  --file FILE, -o FILE  Filename to write to (omit for stdout)\n  --level LEVEL, -l LEVEL\n                        Minimum level/ severity to show\n  --confidence CONFIDENCE, -c CONFIDENCE\n                        Minimum confidence to show\n  --no-colour, -z       No ANSI colours\n  --high-contrast, -Z   High contrast colours\n  --fast, --skip        Skip long running jobs. Will omit plugins with long run time (applies to -p all only)\n  --zero, -0            Return non zero exit code if any security vulnerabilities are found\n```\n\nYou can also import this into your own project and use any of the functions\nin the DOCS\n\n<!-- omit in toc -->\n## Table of Contents\n\n- [Example Use](#example-use)\n\t- [Help](#help)\n- [Developer Notes](#developer-notes)\n\t- [Generate semgrep_sec.yaml](#generate-semgrep_secyaml)\n- [Documentation](#documentation)\n- [Install With PIP](#install-with-pip)\n- [Language information](#language-information)\n\t- [Built for](#built-for)\n- [Install Python on Windows](#install-python-on-windows)\n\t- [Chocolatey](#chocolatey)\n\t- [Windows - Python.org](#windows---pythonorg)\n- [Install Python on Linux](#install-python-on-linux)\n\t- [Apt](#apt)\n\t- [Dnf](#dnf)\n- [Install Python on MacOS](#install-python-on-macos)\n\t- [Homebrew](#homebrew)\n\t- [MacOS - Python.org](#macos---pythonorg)\n- [How to run](#how-to-run)\n\t- [Windows](#windows)\n\t- [Linux/ MacOS](#linux-macos)\n- [Download Project](#download-project)\n\t- [Clone](#clone)\n\t\t- [Using The Command Line](#using-the-command-line)\n\t\t- [Using GitHub Desktop](#using-github-desktop)\n\t- [Download Zip File](#download-zip-file)\n- [Community Files](#community-files)\n\t- [Licence](#licence)\n\t- [Changelog](#changelog)\n\t- [Code of Conduct](#code-of-conduct)\n\t- [Contributing](#contributing)\n\t- [Security](#security)\n\t- [Support](#support)\n\t- [Rationale](#rationale)\n\n## Developer Notes\n\n### Generate semgrep_sec.yaml\n\n1. Clone https://github.com/returntocorp/semgrep-rules\n2. cd to `semgrep-rules/python`\n3. do\n\n   ```bash\n   cat **/security/**/*.yaml >> semgrep_sec.yaml\n   cat **/security/*.yaml >> semgrep_sec.yaml\n   ```\n\n4. Find and replace `rules:` with `` apart from the first instance\n5. Reformat with `ctrl+shift+i`\n6. replace simplesecurity/semgrep_sec.yaml with the new one\n\n## Documentation\n\nA high-level overview of how the documentation is organized organized will help you know\nwhere to look for certain things:\n\n<!--\n- [Tutorials](/documentation/tutorials) take you by the hand through a series of steps to get\n  started using the software. Start here if you’re new.\n-->\n- The [Technical Reference](/documentation/reference) documents APIs and other aspects of the\n  machinery. This documentation describes how to use the classes and functions at a lower level\n  and assume that you have a good high-level understanding of the software.\n<!--\n- The [Help](/documentation/help) guide provides a starting point and outlines common issues that you\n  may have.\n-->\n\n## Install With PIP\n\n**"Slim" Build:** Install bandit, dlint, dodgy, poetry, and safety with pipx\n\n```python\npip install simplesecurity\n```\n\n**Otherwise:**\n\n```python\npip install simplesecurity[full]\n```\n\nHead to https://pypi.org/project/SimpleSecurity/ for more info\n\n## Language information\n\n### Built for\n\nThis program has been written for Python versions 3.7 - 3.10 and has been tested with both 3.7 and\n3.10\n\n## Install Python on Windows\n\n### Chocolatey\n\n```powershell\nchoco install python\n```\n\n### Windows - Python.org\n\nTo install Python, go to https://www.python.org/downloads/windows/ and download the latest\nversion.\n\n## Install Python on Linux\n\n### Apt\n\n```bash\nsudo apt install python3.x\n```\n\n### Dnf\n\n```bash\nsudo dnf install python3.x\n```\n\n## Install Python on MacOS\n\n### Homebrew\n\n```bash\nbrew install python@3.x\n```\n\n### MacOS - Python.org\n\nTo install Python, go to https://www.python.org/downloads/macos/ and download the latest\nversion.\n\n## How to run\n\n### Windows\n\n- Module\n\t`py -3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`py -3.x [file]` or `./[file]`\n\n### Linux/ MacOS\n\n- Module\n\t`python3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`python3.x [file]` or `./[file]`\n\n## Download Project\n\n### Clone\n\n#### Using The Command Line\n\n1. Press the Clone or download button in the top right\n2. Copy the URL (link)\n3. Open the command line and change directory to where you wish to\nclone to\n4. Type \'git clone\' followed by URL in step 2\n\n\t```bash\n\tgit clone https://github.com/FHPythonUtils/SimpleSecurity\n\t```\n\nMore information can be found at\nhttps://help.github.com/en/articles/cloning-a-repository\n\n#### Using GitHub Desktop\n\n1. Press the Clone or download button in the top right\n2. Click open in desktop\n3. Choose the path for where you want and click Clone\n\nMore information can be found at\nhttps://help.github.com/en/desktop/contributing-to-projects/cloning-a-repository-from-github-to-github-desktop\n\n### Download Zip File\n\n1. Download this GitHub repository\n2. Extract the zip archive\n3. Copy/ move to the desired location\n\n## Community Files\n\n### Licence\n\nMIT License\nCopyright (c) FredHappyface\n(See the [LICENSE](/LICENSE.md) for more information.)\n\n### Changelog\n\nSee the [Changelog](/CHANGELOG.md) for more information.\n\n### Code of Conduct\n\nOnline communities include people from many backgrounds. The *Project*\ncontributors are committed to providing a friendly, safe and welcoming\nenvironment for all. Please see the\n[Code of Conduct](https://github.com/FHPythonUtils/.github/blob/master/CODE_OF_CONDUCT.md)\n for more information.\n\n### Contributing\n\nContributions are welcome, please see the\n[Contributing Guidelines](https://github.com/FHPythonUtils/.github/blob/master/CONTRIBUTING.md)\nfor more information.\n\n### Security\n\nThank you for improving the security of the project, please see the\n[Security Policy](https://github.com/FHPythonUtils/.github/blob/master/SECURITY.md)\nfor more information.\n\n### Support\n\nThank you for using this project, I hope it is of use to you. Please be aware that\nthose involved with the project often do so for fun along with other commitments\n(such as work, family, etc). Please see the\n[Support Policy](https://github.com/FHPythonUtils/.github/blob/master/SUPPORT.md)\nfor more information.\n\n### Rationale\n\nThe rationale acts as a guide to various processes regarding projects such as\nthe versioning scheme and the programming styles used. Please see the\n[Rationale](https://github.com/FHPythonUtils/.github/blob/master/RATIONALE.md)\nfor more information.\n',
+    'long_description': '[![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../)\n[![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../)\n[![Issues](https://img.shields.io/github/issues/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../issues)\n[![License](https://img.shields.io/github/license/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](/LICENSE.md)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../commits/master)\n[![Last commit](https://img.shields.io/github/last-commit/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../commits/master)\n[![PyPI Downloads](https://img.shields.io/pypi/dm/simplesecurity.svg?style=for-the-badge)](https://pypistats.org/packages/simplesecurity)\n[![PyPI Total Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=total%20downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fsimplesecurity)](https://pepy.tech/project/simplesecurity)\n[![PyPI Version](https://img.shields.io/pypi/v/simplesecurity.svg?style=for-the-badge)](https://pypi.org/project/simplesecurity)\n\n<!-- omit in toc -->\n# SimpleSecurity\n\n<img src="readme-assets/icons/name.png" alt="Project Icon" width="750">\n\nCombine multiple popular python security tools and generate reports or output\ninto different formats\n\nPlugins (these require the plugin executable in the system path. e.g. bandit\nrequires bandit to be in the system path...)\n\n- bandit\n- safety\n- dodgy\n- dlint\n- semgrep\n\nFormats\n\n- ansi (for terminal)\n- json\n- markdown\n- csv\n- sarif\n\n## Example Use\n\nSee below for the output if you run `simplesecurity` in this directory\n\n<img src="readme-assets/screenshots/sec.svg" width="500px">\n\n### Help\n\n```txt\nusage: __main__.py [-h] [--format FORMAT] [--plugin PLUGIN] [--file FILE] [--level LEVEL] [--confidence CONFIDENCE]\n                   [--no-colour] [--high-contrast] [--fast] [--zero]\n\nCombine multiple popular python security tools...\n\nand generate reports or output into different formats.\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --format FORMAT, -f FORMAT\n                        Output format. One of ansi, json, markdown, csv. default=ansi\n  --plugin PLUGIN, -p PLUGIN\n                        Plugin to use. One of bandit, safety, dodgy, dlint, semgrep, all, default=all\n  --file FILE, -o FILE  Filename to write to (omit for stdout)\n  --level LEVEL, -l LEVEL\n                        Minimum level/ severity to show\n  --confidence CONFIDENCE, -c CONFIDENCE\n                        Minimum confidence to show\n  --no-colour, -z       No ANSI colours\n  --high-contrast, -Z   High contrast colours\n  --fast, --skip        Skip long running jobs. Will omit plugins with long run time (applies to -p all only)\n  --zero, -0            Return non zero exit code if any security vulnerabilities are found\n```\n\nYou can also import this into your own project and use any of the functions\nin the DOCS\n\n<!-- omit in toc -->\n## Table of Contents\n\n- [Example Use](#example-use)\n\t- [Help](#help)\n- [Developer Notes](#developer-notes)\n\t- [Generate semgrep\\_sec.yaml](#generate-semgrep_secyaml)\n- [Documentation](#documentation)\n- [Install With PIP](#install-with-pip)\n- [Language information](#language-information)\n\t- [Built for](#built-for)\n- [Install Python on Windows](#install-python-on-windows)\n\t- [Chocolatey](#chocolatey)\n\t- [Windows - Python.org](#windows---pythonorg)\n- [Install Python on Linux](#install-python-on-linux)\n\t- [Apt](#apt)\n\t- [Dnf](#dnf)\n- [Install Python on MacOS](#install-python-on-macos)\n\t- [Homebrew](#homebrew)\n\t- [MacOS - Python.org](#macos---pythonorg)\n- [How to run](#how-to-run)\n\t- [Windows](#windows)\n\t- [Linux/ MacOS](#linux-macos)\n- [Building](#building)\n- [Testing](#testing)\n- [Download Project](#download-project)\n\t- [Clone](#clone)\n\t\t- [Using The Command Line](#using-the-command-line)\n\t\t- [Using GitHub Desktop](#using-github-desktop)\n\t- [Download Zip File](#download-zip-file)\n- [Community Files](#community-files)\n\t- [Licence](#licence)\n\t- [Changelog](#changelog)\n\t- [Code of Conduct](#code-of-conduct)\n\t- [Contributing](#contributing)\n\t- [Security](#security)\n\t- [Support](#support)\n\t- [Rationale](#rationale)\n\n## Developer Notes\n\n### Generate semgrep_sec.yaml\n\n1. Clone https://github.com/returntocorp/semgrep-rules\n2. cd to `semgrep-rules/python`\n3. do\n\n   ```bash\n   cat **/security/**/*.yaml >> semgrep_sec.yaml\n   cat **/security/*.yaml >> semgrep_sec.yaml\n   ```\n\n4. Find and replace `rules:` with `` apart from the first instance\n5. Reformat with `ctrl+shift+i`\n6. replace simplesecurity/semgrep_sec.yaml with the new one\n\n## Documentation\n\nA high-level overview of how the documentation is organized organized will help you know\nwhere to look for certain things:\n\n<!--\n- [Tutorials](/documentation/tutorials) take you by the hand through a series of steps to get\n  started using the software. Start here if you’re new.\n-->\n- The [Technical Reference](/documentation/reference) documents APIs and other aspects of the\n  machinery. This documentation describes how to use the classes and functions at a lower level\n  and assume that you have a good high-level understanding of the software.\n<!--\n- The [Help](/documentation/help) guide provides a starting point and outlines common issues that you\n  may have.\n-->\n\n## Install With PIP\n\n**"Slim" Build:** Install bandit, dlint, dodgy, poetry, and safety with pipx\n\n```python\npip install simplesecurity\n```\n\n**Otherwise:**\n\n```python\npip install simplesecurity[full]\n```\n\nHead to https://pypi.org/project/SimpleSecurity/ for more info\n\n## Language information\n\n### Built for\n\nThis program has been written for Python versions 3.8 - 3.11 and has been tested with both 3.8 and\n3.11\n\n## Install Python on Windows\n\n### Chocolatey\n\n```powershell\nchoco install python\n```\n\n### Windows - Python.org\n\nTo install Python, go to https://www.python.org/downloads/windows/ and download the latest\nversion.\n\n## Install Python on Linux\n\n### Apt\n\n```bash\nsudo apt install python3.x\n```\n\n### Dnf\n\n```bash\nsudo dnf install python3.x\n```\n\n## Install Python on MacOS\n\n### Homebrew\n\n```bash\nbrew install python@3.x\n```\n\n### MacOS - Python.org\n\nTo install Python, go to https://www.python.org/downloads/macos/ and download the latest\nversion.\n\n## How to run\n\n### Windows\n\n- Module\n\t`py -3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`py -3.x [file]` or `./[file]`\n\n### Linux/ MacOS\n\n- Module\n\t`python3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`python3.x [file]` or `./[file]`\n\n## Building\n\nThis project uses https://github.com/FHPythonUtils/FHMake to automate most of the building. This\ncommand generates the documentation, updates the requirements.txt and builds the library artefacts\n\nNote the functionality provided by fhmake can be approximated by the following\n\n```sh\nhandsdown  --cleanup -o documentation/reference\npoetry export -f requirements.txt --output requirements.txt\npoetry export -f requirements.txt --with dev --output requirements_optional.txt\npoetry build\n```\n\n`fhmake audit` can be run to perform additional checks\n\n## Testing\n\nFor testing with the version of python used by poetry use\n\n```sh\npoetry run pytest\n```\n\nAlternatively use `tox` to run tests over python 3.8 - 3.11\n\n```sh\ntox\n```\n\n## Download Project\n\n### Clone\n\n#### Using The Command Line\n\n1. Press the Clone or download button in the top right\n2. Copy the URL (link)\n3. Open the command line and change directory to where you wish to\nclone to\n4. Type \'git clone\' followed by URL in step 2\n\n\t```bash\n\tgit clone https://github.com/FHPythonUtils/SimpleSecurity\n\t```\n\nMore information can be found at\nhttps://help.github.com/en/articles/cloning-a-repository\n\n#### Using GitHub Desktop\n\n1. Press the Clone or download button in the top right\n2. Click open in desktop\n3. Choose the path for where you want and click Clone\n\nMore information can be found at\nhttps://help.github.com/en/desktop/contributing-to-projects/cloning-a-repository-from-github-to-github-desktop\n\n### Download Zip File\n\n1. Download this GitHub repository\n2. Extract the zip archive\n3. Copy/ move to the desired location\n\n## Community Files\n\n### Licence\n\nMIT License\nCopyright (c) FredHappyface\n(See the [LICENSE](/LICENSE.md) for more information.)\n\n### Changelog\n\nSee the [Changelog](/CHANGELOG.md) for more information.\n\n### Code of Conduct\n\nOnline communities include people from many backgrounds. The *Project*\ncontributors are committed to providing a friendly, safe and welcoming\nenvironment for all. Please see the\n[Code of Conduct](https://github.com/FHPythonUtils/.github/blob/master/CODE_OF_CONDUCT.md)\n for more information.\n\n### Contributing\n\nContributions are welcome, please see the\n[Contributing Guidelines](https://github.com/FHPythonUtils/.github/blob/master/CONTRIBUTING.md)\nfor more information.\n\n### Security\n\nThank you for improving the security of the project, please see the\n[Security Policy](https://github.com/FHPythonUtils/.github/blob/master/SECURITY.md)\nfor more information.\n\n### Support\n\nThank you for using this project, I hope it is of use to you. Please be aware that\nthose involved with the project often do so for fun along with other commitments\n(such as work, family, etc). Please see the\n[Support Policy](https://github.com/FHPythonUtils/.github/blob/master/SUPPORT.md)\nfor more information.\n\n### Rationale\n\nThe rationale acts as a guide to various processes regarding projects such as\nthe versioning scheme and the programming styles used. Please see the\n[Rationale](https://github.com/FHPythonUtils/.github/blob/master/RATIONALE.md)\nfor more information.\n',
     'author': 'FredHappyface',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
+    'author_email': 'None',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/FHPythonUtils/SimpleSecurity',
     'packages': packages,
     'package_data': package_data,
     'extras_require': extras_require,
     'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `simplesecurity-2022/PKG-INFO` & `simplesecurity-2023/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplesecurity
-Version: 2022
+Version: 2023
 Summary: Combine multiple popular python security tools and generate reports or output into different formats
 Home-page: https://github.com/FHPythonUtils/SimpleSecurity
 License: MIT
 Author: FredHappyface
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -12,29 +12,30 @@
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Provides-Extra: full
-Requires-Dist: bandit (>=1.7.0,<2); extra == "full"
-Requires-Dist: dlint (>=0.11.0,<2); extra == "full"
-Requires-Dist: dodgy (>=0.2.1,<2); extra == "full"
-Requires-Dist: poetry (>=1.1.10,<2); extra == "full"
-Requires-Dist: safety (>=1.10.3,<2); extra == "full"
-Requires-Dist: semgrep (>=0.67.0,<2); extra == "full"
+Requires-Dist: bandit (>=1.7.5,<2) ; extra == "full"
+Requires-Dist: dlint (>=0.14.1,<2) ; extra == "full"
+Requires-Dist: dodgy (>=0.2.1,<2) ; extra == "full"
+Requires-Dist: poetry (>=1.5.1,<2) ; extra == "full"
+Requires-Dist: safety (>=2.3.5,<3) ; extra == "full"
+Requires-Dist: semgrep (>=1.29.0,<2) ; extra == "full"
 Project-URL: Documentation, https://github.com/FHPythonUtils/SimpleSecurity/blob/master/README.md
 Project-URL: Repository, https://github.com/FHPythonUtils/SimpleSecurity
 Description-Content-Type: text/markdown
 
 [![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../)
 [![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../)
 [![Issues](https://img.shields.io/github/issues/FHPythonUtils/SimpleSecurity.svg?style=for-the-badge)](../../issues)
@@ -108,15 +109,15 @@
 
 <!-- omit in toc -->
 ## Table of Contents
 
 - [Example Use](#example-use)
 	- [Help](#help)
 - [Developer Notes](#developer-notes)
-	- [Generate semgrep_sec.yaml](#generate-semgrep_secyaml)
+	- [Generate semgrep\_sec.yaml](#generate-semgrep_secyaml)
 - [Documentation](#documentation)
 - [Install With PIP](#install-with-pip)
 - [Language information](#language-information)
 	- [Built for](#built-for)
 - [Install Python on Windows](#install-python-on-windows)
 	- [Chocolatey](#chocolatey)
 	- [Windows - Python.org](#windows---pythonorg)
@@ -125,14 +126,16 @@
 	- [Dnf](#dnf)
 - [Install Python on MacOS](#install-python-on-macos)
 	- [Homebrew](#homebrew)
 	- [MacOS - Python.org](#macos---pythonorg)
 - [How to run](#how-to-run)
 	- [Windows](#windows)
 	- [Linux/ MacOS](#linux-macos)
+- [Building](#building)
+- [Testing](#testing)
 - [Download Project](#download-project)
 	- [Clone](#clone)
 		- [Using The Command Line](#using-the-command-line)
 		- [Using GitHub Desktop](#using-github-desktop)
 	- [Download Zip File](#download-zip-file)
 - [Community Files](#community-files)
 	- [Licence](#licence)
@@ -193,16 +196,16 @@
 
 Head to https://pypi.org/project/SimpleSecurity/ for more info
 
 ## Language information
 
 ### Built for
 
-This program has been written for Python versions 3.7 - 3.10 and has been tested with both 3.7 and
-3.10
+This program has been written for Python versions 3.8 - 3.11 and has been tested with both 3.8 and
+3.11
 
 ## Install Python on Windows
 
 ### Chocolatey
 
 ```powershell
 choco install python
@@ -254,14 +257,44 @@
 
 - Module
 	`python3.x -m [module]` or `[module]` (if module installs a script)
 
 - File
 	`python3.x [file]` or `./[file]`
 
+## Building
+
+This project uses https://github.com/FHPythonUtils/FHMake to automate most of the building. This
+command generates the documentation, updates the requirements.txt and builds the library artefacts
+
+Note the functionality provided by fhmake can be approximated by the following
+
+```sh
+handsdown  --cleanup -o documentation/reference
+poetry export -f requirements.txt --output requirements.txt
+poetry export -f requirements.txt --with dev --output requirements_optional.txt
+poetry build
+```
+
+`fhmake audit` can be run to perform additional checks
+
+## Testing
+
+For testing with the version of python used by poetry use
+
+```sh
+poetry run pytest
+```
+
+Alternatively use `tox` to run tests over python 3.8 - 3.11
+
+```sh
+tox
+```
+
 ## Download Project
 
 ### Clone
 
 #### Using The Command Line
 
 1. Press the Clone or download button in the top right
```

