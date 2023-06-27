# Comparing `tmp/catpandoc-2022.1.tar.gz` & `tmp/catpandoc-2022.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catpandoc-2022.1.tar", max compression
+gzip compressed data, was "catpandoc-2022.2.tar", max compression
```

## Comparing `catpandoc-2022.1.tar` & `catpandoc-2022.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2021-11-14 20:47:24.380773 catpandoc-2022.1/catpandoc/__init__.py
--rw-r--r--   0        0        0      128 2021-11-14 20:47:24.380773 catpandoc-2022.1/catpandoc/__main__.py
--rw-r--r--   0        0        0     1542 2022-01-23 22:37:10.920074 catpandoc-2022.1/catpandoc/application.py
--rw-r--r--   0        0        0     1089 2021-11-11 20:20:38.724491 catpandoc-2022.1/LICENSE.md
--rw-r--r--   0        0        0     1707 2022-01-23 22:37:29.923945 catpandoc-2022.1/pyproject.toml
--rw-r--r--   0        0        0     8517 2022-01-23 22:32:07.127654 catpandoc-2022.1/README.md
--rw-r--r--   0        0        0     9345 2022-01-23 22:37:33.130414 catpandoc-2022.1/setup.py
--rw-r--r--   0        0        0     9455 2022-01-23 22:37:33.130414 catpandoc-2022.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-27 20:30:50.658611 catpandoc-2022.2/catpandoc/__init__.py
+-rw-r--r--   0        0        0      128 2023-06-27 20:30:50.658611 catpandoc-2022.2/catpandoc/__main__.py
+-rw-r--r--   0        0        0     1576 2023-06-27 20:30:50.658611 catpandoc-2022.2/catpandoc/application.py
+-rw-r--r--   0        0        0     1068 2023-01-01 17:52:45.067218 catpandoc-2022.2/LICENSE.md
+-rw-r--r--   0        0        0     1979 2023-06-27 20:31:02.399832 catpandoc-2022.2/pyproject.toml
+-rw-r--r--   0        0        0     9389 2023-01-08 16:54:13.270095 catpandoc-2022.2/README.md
+-rw-r--r--   0        0        0    10591 1970-01-01 00:00:00.000000 catpandoc-2022.2/setup.py
+-rw-r--r--   0        0        0    10716 1970-01-01 00:00:00.000000 catpandoc-2022.2/PKG-INFO
```

### Comparing `catpandoc-2022.1/catpandoc/application.py` & `catpandoc-2022.2/catpandoc/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 import argparse
 
 import pypandoc
 from rich.console import Console
 from rich.markdown import Markdown
 
 
-def pandoc2ansi(file: str, width: int) -> str:
+def pandoc2ansi(file: str, width: int = 79) -> str:
 	console = Console(width=width)
 	markdown = Markdown(pypandoc.convert_file(file, "md"))
 	with console.capture() as capture:
 		console.print(markdown)
 	return capture.get()
 
 
-def pandoc2plain(file: str, width: int) -> str:
+def pandoc2plain(file: str, width: int = 79) -> str:
 	console = Console(color_system=None, width=width)
 	markdown = Markdown(pypandoc.convert_file(file, "md"))
 	with console.capture() as capture:
 		console.print(markdown)
 	return capture.get()
 
 
@@ -35,17 +35,19 @@
 
 	# Open file and convert to JSON
 	try:
 		pypandoc.convert_text("#test", "json", format="md")  # type: ignore
 	except OSError:
 		pypandoc.download_pandoc()  # type: ignore
 
+	width = args.width or 79
+
 	# Print to console
 	functions = pandoc2ansi, pandoc2plain
-	print(functions[args.to_plain](args.file, args.width))
+	print(functions[args.to_plain](args.file, width))
 
 
 def cli() -> None:
 	"""Parse args from the command line"""
 	parser = argparse.ArgumentParser(description="Print md")
 	parser.add_argument("file", help="file to render")
 	parser.add_argument("--width", help="terminal width", action="store", type=int)
```

### Comparing `catpandoc-2022.1/pyproject.toml` & `catpandoc-2022.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "catpandoc"
-version = "2022.1"
+version = "2022.2"
 license = "mit"
 description = "Cat multiple document files to the terminal"
 authors = ["FredHappyface"]
 classifiers = [
 	"Environment :: Console",
 	"Development Status :: 5 - Production/Stable",
 	"Intended Audience :: Developers",
@@ -22,46 +22,65 @@
 readme = "README.md"
 
 [tool.poetry.scripts]
 catpandoc = 'catpandoc.application:cli'
 
 [tool.poetry.dependencies]
 python = "^3.7"
-pypandoc = "<2,>=1.7.2"
-rich = "<12,>=11.0.0"
+pypandoc = "<2,>=1.11"
+rich = "<14,>=13.4.2"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.0"
+tox = "^4.6.3"
+coverage = "^7.2.7"
+
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
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.pylint.basic]
 argument-naming-style = "camelCase"
 attr-naming-style = "camelCase"
 function-naming-style = "camelCase"
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
 
-[tool.pydocstyle]
-convention = "google"
-ignore = "D205,D415"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.tox]
+legacy_tox_ini = """
+[tox]
+isolated_build = True
+env_list =
+	py311
+	py310
+	py39
+	py38
+
+[testenv]
+allowlist_externals = poetry
+commands =
+  poetry install -v
+  poetry run pytest
+"""
```

### Comparing `catpandoc-2022.1/setup.py` & `catpandoc-2022.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 packages = \
 ['catpandoc']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pypandoc>=1.7.2,<2', 'rich>=11.0.0,<12']
+['pypandoc>=1.11,<2', 'rich>=13.4.2,<14']
 
 entry_points = \
 {'console_scripts': ['catpandoc = catpandoc.application:cli']}
 
 setup_kwargs = {
     'name': 'catpandoc',
-    'version': '2022.1',
+    'version': '2022.2',
     'description': 'Cat multiple document files to the terminal',
-    'long_description': '[![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/CatPandoc.svg?style=for-the-badge)](../../)\n[![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/CatPandoc.svg?style=for-the-badge)](../../)\n[![Issues](https://img.shields.io/github/issues/FHPythonUtils/CatPandoc.svg?style=for-the-badge)](../../issues)\n[![License](https://img.shields.io/github/license/FHPythonUtils/CatPandoc.svg?style=for-the-badge)](/LICENSE.md)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/FHPythonUtils/CatPandoc.svg?style=for-the-badge)](../../commits/master)\n[![Last commit](https://img.shields.io/github/last-commit/FHPythonUtils/CatPandoc.svg?style=for-the-badge)](../../commits/master)\n[![PyPI Downloads](https://img.shields.io/pypi/dm/catpandoc.svg?style=for-the-badge)](https://pypistats.org/packages/catpandoc)\n[![PyPI Total Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=total%20downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fcatpandoc)](https://pepy.tech/project/catpandoc)\n[![PyPI Version](https://img.shields.io/pypi/v/catpandoc.svg?style=for-the-badge)](https://pypi.org/project/catpandoc)\n\n<!-- omit in toc -->\n# CatPandoc\n\n<img src="readme-assets/icons/name.png" alt="Project Icon" width="750">\n\nCat multiple documents to the terminal. The continuation of CatMD\n\n- [Features](#features)\n\t- [Document Compatability](#document-compatability)\n\t- [Terminal \'rendering\'](#terminal-rendering)\n- [Roadmap](#roadmap)\n- [Use](#use)\n\t- [CLI](#cli)\n\t- [Import](#import)\n- [Documentation](#documentation)\n- [Install With PIP](#install-with-pip)\n- [Language information](#language-information)\n\t- [Built for](#built-for)\n- [Install Python on Windows](#install-python-on-windows)\n\t- [Chocolatey](#chocolatey)\n\t- [Windows - Python.org](#windows---pythonorg)\n- [Install Python on Linux](#install-python-on-linux)\n\t- [Apt](#apt)\n\t- [Dnf](#dnf)\n- [Install Python on MacOS](#install-python-on-macos)\n\t- [Homebrew](#homebrew)\n\t- [MacOS - Python.org](#macos---pythonorg)\n- [How to run](#how-to-run)\n\t- [Windows](#windows)\n\t- [Linux/ MacOS](#linux-macos)\n- [Download Project](#download-project)\n\t- [Clone](#clone)\n\t\t- [Using The Command Line](#using-the-command-line)\n\t\t- [Using GitHub Desktop](#using-github-desktop)\n\t- [Download Zip File](#download-zip-file)\n- [Community Files](#community-files)\n\t- [Licence](#licence)\n\t- [Changelog](#changelog)\n\t- [Code of Conduct](#code-of-conduct)\n\t- [Contributing](#contributing)\n\t- [Security](#security)\n\t- [Support](#support)\n\t- [Rationale](#rationale)\n- [Screenshots](#screenshots)\n\t- [Desktop](#desktop)\n\n## Features\n\n### Document Compatability\n\nLightweight markup formats\n\n- Markdown (including CommonMark and GitHub-flavored Markdown)\n- reStructuredText\n- Emacs Org-Mode\n- Emacs Muse\n- Textile\n- txt2tags\n\nHTML formats\n\n- (X)HTML 4\n- HTML5\n\nEbooks\n\n- EPUB version 2 or 3\n- FictionBook2\n\nDocumentation formats\n\n- Haddock markup\n\nRoff formats\n\n- roff man\n\nTeX formats\n\n- LaTeX\n\nXML formats\n\n- DocBook version 4 or 5\n- JATS\n\nOutline formats\n\n- OPML\n\nData formats\n\n- CSV tables\n\nWord processor formats\n\n- Microsoft Word docx\n- OpenOffice/LibreOffice ODT\n\nInteractive notebook formats\n\n- Jupyter notebook (ipynb)\n\nWiki markup formats\n\n- MediaWiki markup\n- DokuWiki markup\n- TikiWiki markup\n- TWiki markup\n- Jira wiki markup\n\n### Terminal \'rendering\'\n\nHighlights the following:\n\n- Headers 1-6\n- Unordered and ordered lists\n- Block quotes\n- Bold, Italic, Strikethrough, inline code\n- Line Break (br)\n\nRenders the following\n\n- Tables\n\nHighlights code blocks\n\n- Uses pygments for code syntax highlighting\n\n## Roadmap\n\nFor completed components, see the changelog (link below)\n\n|Feature|Description|Status|\n|---|---|---|\n|pandoc2pysimplegui.py|Generate PySimpleGUI widgets|-|\n\n## Use\n\n### CLI\n\n```bash\nusage: application.py [-h] [--width WIDTH] [--theme THEME] file\n```\n\n### Import\n\nTake a look at test/catcomplex.py for an example of how to use catpandoc in your own\nproject. Or take a look at the example below\n\n```python\nimport json\nimport pypandoc\nfrom catpandoc import pandoc2ansi, processpandoc\n\noutput = json.loads(pypandoc.convert_file("cheatsheet.md", \'json\'))\nfor block in output["blocks"]:\n\tpandoc = pandoc2ansi.Pandoc2Ansi(130, 5, (4, 0, 0))\n\tprocesspandoc.processBlock(block, pandoc)\n\tprint(pandoc.genOutput())\n```\n\n## Documentation\n\nSee the [Docs](/DOCS/) for more information.\n\n## Install With PIP\n\n```python\npip install catpandoc\n```\n\nHead to https://pypi.org/project/catpandoc/ for more info\n\n## Language information\n\n### Built for\n\nThis program has been written for Python versions 3.7 - 3.10 and has been tested with both 3.7 and\n3.10\n\n## Install Python on Windows\n\n### Chocolatey\n\n```powershell\nchoco install python\n```\n\n### Windows - Python.org\n\nTo install Python, go to https://www.python.org/downloads/windows/ and download the latest\nversion.\n\n## Install Python on Linux\n\n### Apt\n\n```bash\nsudo apt install python3.x\n```\n\n### Dnf\n\n```bash\nsudo dnf install python3.x\n```\n\n## Install Python on MacOS\n\n### Homebrew\n\n```bash\nbrew install python@3.x\n```\n\n### MacOS - Python.org\n\nTo install Python, go to https://www.python.org/downloads/macos/ and download the latest\nversion.\n\n## How to run\n\n### Windows\n\n- Module\n\t`py -3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`py -3.x [file]` or `./[file]`\n\n### Linux/ MacOS\n\n- Module\n\t`python3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`python3.x [file]` or `./[file]`\n\n## Download Project\n\n### Clone\n\n#### Using The Command Line\n\n1. Press the Clone or download button in the top right\n2. Copy the URL (link)\n3. Open the command line and change directory to where you wish to\nclone to\n4. Type \'git clone\' followed by URL in step 2\n\n```bash\ngit clone https://github.com/FHPythonUtils/CatPandoc\n```\n\nMore information can be found at\nhttps://help.github.com/en/articles/cloning-a-repository\n\n#### Using GitHub Desktop\n\n1. Press the Clone or download button in the top right\n2. Click open in desktop\n3. Choose the path for where you want and click Clone\n\nMore information can be found at\nhttps://help.github.com/en/desktop/contributing-to-projects/cloning-a-repository-from-github-to-github-desktop\n\n### Download Zip File\n\n1. Download this GitHub repository\n2. Extract the zip archive\n3. Copy/ move to the desired location\n\n## Community Files\n\n### Licence\n\nMIT License\nCopyright (c) FredHappyface\n(See the [LICENSE](/LICENSE.md) for more information.)\n\n### Changelog\n\nSee the [Changelog](/CHANGELOG.md) for more information.\n\n### Code of Conduct\n\nOnline communities include people from many backgrounds. The *Project*\ncontributors are committed to providing a friendly, safe and welcoming\nenvironment for all. Please see the\n[Code of Conduct](https://github.com/FHPythonUtils/.github/blob/master/CODE_OF_CONDUCT.md)\n for more information.\n\n### Contributing\n\nContributions are welcome, please see the\n[Contributing Guidelines](https://github.com/FHPythonUtils/.github/blob/master/CONTRIBUTING.md)\nfor more information.\n\n### Security\n\nThank you for improving the security of the project, please see the\n[Security Policy](https://github.com/FHPythonUtils/.github/blob/master/SECURITY.md)\nfor more information.\n\n### Support\n\nThank you for using this project, I hope it is of use to you. Please be aware that\nthose involved with the project often do so for fun along with other commitments\n(such as work, family, etc). Please see the\n[Support Policy](https://github.com/FHPythonUtils/.github/blob/master/SUPPORT.md)\nfor more information.\n\n### Rationale\n\nThe rationale acts as a guide to various processes regarding projects such as\nthe versioning scheme and the programming styles used. Please see the\n[Rationale](https://github.com/FHPythonUtils/.github/blob/master/RATIONALE.md)\nfor more information.\n\n## Screenshots\n\n### Desktop\n\n<div>\n<img src="readme-assets/screenshots/desktop/screenshot-0.png" alt="Screenshot 1" width="600">\n<img src="readme-assets/screenshots/desktop/screenshot-1.png" alt="Screenshot 2" width="600">\n<img src="readme-assets/screenshots/desktop/screenshot-2.png" alt="Screenshot 3" width="600">\n</div>\n',
+    'long_description': '[![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/CatPandoc.svg?style=for-the-badge)](../../)\n[![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/CatPandoc.svg?style=for-the-badge)](../../)\n[![Issues](https://img.shields.io/github/issues/FHPythonUtils/CatPandoc.svg?style=for-the-badge)](../../issues)\n[![License](https://img.shields.io/github/license/FHPythonUtils/CatPandoc.svg?style=for-the-badge)](/LICENSE.md)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/FHPythonUtils/CatPandoc.svg?style=for-the-badge)](../../commits/master)\n[![Last commit](https://img.shields.io/github/last-commit/FHPythonUtils/CatPandoc.svg?style=for-the-badge)](../../commits/master)\n[![PyPI Downloads](https://img.shields.io/pypi/dm/catpandoc.svg?style=for-the-badge)](https://pypistats.org/packages/catpandoc)\n[![PyPI Total Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=total%20downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fcatpandoc)](https://pepy.tech/project/catpandoc)\n[![PyPI Version](https://img.shields.io/pypi/v/catpandoc.svg?style=for-the-badge)](https://pypi.org/project/catpandoc)\n\n<!-- omit in toc -->\n# CatPandoc\n\n<img src="readme-assets/icons/name.png" alt="Project Icon" width="750">\n\nCat multiple documents to the terminal. The continuation of CatMD\n\n- [Features](#features)\n\t- [Document Compatability](#document-compatability)\n\t- [Terminal \'rendering\'](#terminal-rendering)\n- [Roadmap](#roadmap)\n- [Use](#use)\n\t- [CLI](#cli)\n\t- [Import](#import)\n- [Documentation](#documentation)\n- [Install With PIP](#install-with-pip)\n- [Language information](#language-information)\n\t- [Built for](#built-for)\n- [Install Python on Windows](#install-python-on-windows)\n\t- [Chocolatey](#chocolatey)\n\t- [Windows - Python.org](#windows---pythonorg)\n- [Install Python on Linux](#install-python-on-linux)\n\t- [Apt](#apt)\n\t- [Dnf](#dnf)\n- [Install Python on MacOS](#install-python-on-macos)\n\t- [Homebrew](#homebrew)\n\t- [MacOS - Python.org](#macos---pythonorg)\n- [How to run](#how-to-run)\n\t- [Windows](#windows)\n\t- [Linux/ MacOS](#linux-macos)\n- [Building](#building)\n- [Download Project](#download-project)\n\t- [Clone](#clone)\n\t\t- [Using The Command Line](#using-the-command-line)\n\t\t- [Using GitHub Desktop](#using-github-desktop)\n\t- [Download Zip File](#download-zip-file)\n- [Community Files](#community-files)\n\t- [Licence](#licence)\n\t- [Changelog](#changelog)\n\t- [Code of Conduct](#code-of-conduct)\n\t- [Contributing](#contributing)\n\t- [Security](#security)\n\t- [Support](#support)\n\t- [Rationale](#rationale)\n- [Screenshots](#screenshots)\n\t- [Desktop](#desktop)\n\n## Features\n\n### Document Compatability\n\nLightweight markup formats\n\n- Markdown (including CommonMark and GitHub-flavored Markdown)\n- reStructuredText\n- Emacs Org-Mode\n- Emacs Muse\n- Textile\n- txt2tags\n\nHTML formats\n\n- (X)HTML 4\n- HTML5\n\nEbooks\n\n- EPUB version 2 or 3\n- FictionBook2\n\nDocumentation formats\n\n- Haddock markup\n\nRoff formats\n\n- roff man\n\nTeX formats\n\n- LaTeX\n\nXML formats\n\n- DocBook version 4 or 5\n- JATS\n\nOutline formats\n\n- OPML\n\nData formats\n\n- CSV tables\n\nWord processor formats\n\n- Microsoft Word docx\n- OpenOffice/LibreOffice ODT\n\nInteractive notebook formats\n\n- Jupyter notebook (ipynb)\n\nWiki markup formats\n\n- MediaWiki markup\n- DokuWiki markup\n- TikiWiki markup\n- TWiki markup\n- Jira wiki markup\n\n### Terminal \'rendering\'\n\nHighlights the following:\n\n- Headers 1-6\n- Unordered and ordered lists\n- Block quotes\n- Bold, Italic, Strikethrough, inline code\n- Line Break (br)\n\nRenders the following\n\n- Tables\n\nHighlights code blocks\n\n- Uses pygments for code syntax highlighting\n\n## Roadmap\n\nFor completed components, see the changelog (link below)\n\n|Feature|Description|Status|\n|---|---|---|\n|pandoc2pysimplegui.py|Generate PySimpleGUI widgets|-|\n\n## Use\n\n### CLI\n\n```bash\nusage: application.py [-h] [--width WIDTH] [--theme THEME] file\n```\n\n### Import\n\nTake a look at test/catcomplex.py for an example of how to use catpandoc in your own\nproject. Or take a look at the example below\n\n```python\nimport json\nimport pypandoc\nfrom catpandoc import pandoc2ansi, processpandoc\n\noutput = json.loads(pypandoc.convert_file("cheatsheet.md", \'json\'))\nfor block in output["blocks"]:\n\tpandoc = pandoc2ansi.Pandoc2Ansi(130, 5, (4, 0, 0))\n\tprocesspandoc.processBlock(block, pandoc)\n\tprint(pandoc.genOutput())\n```\n\n## Documentation\n\nA high-level overview of how the documentation is organized organized will help you know\nwhere to look for certain things:\n\n<!--\n- [Tutorials](/documentation/tutorials) take you by the hand through a series of steps to get\n  started using the software. Start here if you’re new.\n-->\n- The [Technical Reference](/documentation/reference) documents APIs and other aspects of the\n  machinery. This documentation describes how to use the classes and functions at a lower level\n  and assume that you have a good high-level understanding of the software.\n<!--\n- The [Help](/documentation/help) guide provides a starting point and outlines common issues that you\n  may have.\n-->\n\n## Install With PIP\n\n```python\npip install catpandoc\n```\n\nHead to https://pypi.org/project/catpandoc/ for more info\n\n## Language information\n\n### Built for\n\nThis program has been written for Python versions 3.8 - 3.11 and has been tested with both 3.8 and\n3.11\n\n## Install Python on Windows\n\n### Chocolatey\n\n```powershell\nchoco install python\n```\n\n### Windows - Python.org\n\nTo install Python, go to https://www.python.org/downloads/windows/ and download the latest\nversion.\n\n## Install Python on Linux\n\n### Apt\n\n```bash\nsudo apt install python3.x\n```\n\n### Dnf\n\n```bash\nsudo dnf install python3.x\n```\n\n## Install Python on MacOS\n\n### Homebrew\n\n```bash\nbrew install python@3.x\n```\n\n### MacOS - Python.org\n\nTo install Python, go to https://www.python.org/downloads/macos/ and download the latest\nversion.\n\n## How to run\n\n### Windows\n\n- Module\n\t`py -3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`py -3.x [file]` or `./[file]`\n\n### Linux/ MacOS\n\n- Module\n\t`python3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`python3.x [file]` or `./[file]`\n\n## Building\n\nThis project uses https://github.com/FHPythonUtils/FHMake to automate most of the building. This\ncommand generates the documentation, updates the requirements.txt and builds the library artefacts\n\nNote the functionality provided by fhmake can be approximated by the following\n\n```sh\nhandsdown  --cleanup -o documentation/reference\npoetry export -f requirements.txt --output requirements.txt\npoetry export -f requirements.txt --with dev --output requirements_optional.txt\npoetry build\n```\n\n`fhmake audit` can be run to perform additional checks\n\n## Download Project\n\n### Clone\n\n#### Using The Command Line\n\n1. Press the Clone or download button in the top right\n2. Copy the URL (link)\n3. Open the command line and change directory to where you wish to\nclone to\n4. Type \'git clone\' followed by URL in step 2\n\n```bash\ngit clone https://github.com/FHPythonUtils/CatPandoc\n```\n\nMore information can be found at\nhttps://help.github.com/en/articles/cloning-a-repository\n\n#### Using GitHub Desktop\n\n1. Press the Clone or download button in the top right\n2. Click open in desktop\n3. Choose the path for where you want and click Clone\n\nMore information can be found at\nhttps://help.github.com/en/desktop/contributing-to-projects/cloning-a-repository-from-github-to-github-desktop\n\n### Download Zip File\n\n1. Download this GitHub repository\n2. Extract the zip archive\n3. Copy/ move to the desired location\n\n## Community Files\n\n### Licence\n\nMIT License\nCopyright (c) FredHappyface\n(See the [LICENSE](/LICENSE.md) for more information.)\n\n### Changelog\n\nSee the [Changelog](/CHANGELOG.md) for more information.\n\n### Code of Conduct\n\nOnline communities include people from many backgrounds. The *Project*\ncontributors are committed to providing a friendly, safe and welcoming\nenvironment for all. Please see the\n[Code of Conduct](https://github.com/FHPythonUtils/.github/blob/master/CODE_OF_CONDUCT.md)\n for more information.\n\n### Contributing\n\nContributions are welcome, please see the\n[Contributing Guidelines](https://github.com/FHPythonUtils/.github/blob/master/CONTRIBUTING.md)\nfor more information.\n\n### Security\n\nThank you for improving the security of the project, please see the\n[Security Policy](https://github.com/FHPythonUtils/.github/blob/master/SECURITY.md)\nfor more information.\n\n### Support\n\nThank you for using this project, I hope it is of use to you. Please be aware that\nthose involved with the project often do so for fun along with other commitments\n(such as work, family, etc). Please see the\n[Support Policy](https://github.com/FHPythonUtils/.github/blob/master/SUPPORT.md)\nfor more information.\n\n### Rationale\n\nThe rationale acts as a guide to various processes regarding projects such as\nthe versioning scheme and the programming styles used. Please see the\n[Rationale](https://github.com/FHPythonUtils/.github/blob/master/RATIONALE.md)\nfor more information.\n\n## Screenshots\n\n### Desktop\n\n<div>\n<img src="readme-assets/screenshots/desktop/screenshot-0.png" alt="Screenshot 1" width="600">\n<img src="readme-assets/screenshots/desktop/screenshot-1.png" alt="Screenshot 2" width="600">\n<img src="readme-assets/screenshots/desktop/screenshot-2.png" alt="Screenshot 3" width="600">\n</div>\n',
     'author': 'FredHappyface',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
+    'author_email': 'None',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/FHPythonUtils/CatPandoc',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `catpandoc-2022.1/PKG-INFO` & `catpandoc-2022.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: catpandoc
-Version: 2022.1
+Version: 2022.2
 Summary: Cat multiple document files to the terminal
 Home-page: https://github.com/FHPythonUtils/CatPandoc
 License: MIT
 Author: FredHappyface
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
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
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
-Requires-Dist: pypandoc (>=1.7.2,<2)
-Requires-Dist: rich (>=11.0.0,<12)
+Requires-Dist: pypandoc (>=1.11,<2)
+Requires-Dist: rich (>=13.4.2,<14)
 Project-URL: Documentation, https://github.com/FHPythonUtils/CatPandoc/blob/master/README.md
 Project-URL: Repository, https://github.com/FHPythonUtils/CatPandoc
 Description-Content-Type: text/markdown
 
 [![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/CatPandoc.svg?style=for-the-badge)](../../)
 [![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/CatPandoc.svg?style=for-the-badge)](../../)
 [![Issues](https://img.shields.io/github/issues/FHPythonUtils/CatPandoc.svg?style=for-the-badge)](../../issues)
@@ -64,14 +65,15 @@
 	- [Dnf](#dnf)
 - [Install Python on MacOS](#install-python-on-macos)
 	- [Homebrew](#homebrew)
 	- [MacOS - Python.org](#macos---pythonorg)
 - [How to run](#how-to-run)
 	- [Windows](#windows)
 	- [Linux/ MacOS](#linux-macos)
+- [Building](#building)
 - [Download Project](#download-project)
 	- [Clone](#clone)
 		- [Using The Command Line](#using-the-command-line)
 		- [Using GitHub Desktop](#using-github-desktop)
 	- [Download Zip File](#download-zip-file)
 - [Community Files](#community-files)
 	- [Licence](#licence)
@@ -198,30 +200,43 @@
 	pandoc = pandoc2ansi.Pandoc2Ansi(130, 5, (4, 0, 0))
 	processpandoc.processBlock(block, pandoc)
 	print(pandoc.genOutput())
 ```
 
 ## Documentation
 
-See the [Docs](/DOCS/) for more information.
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
 
 ## Install With PIP
 
 ```python
 pip install catpandoc
 ```
 
 Head to https://pypi.org/project/catpandoc/ for more info
 
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
@@ -273,14 +288,30 @@
 
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
 ## Download Project
 
 ### Clone
 
 #### Using The Command Line
 
 1. Press the Clone or download button in the top right
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

