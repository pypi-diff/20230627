# Comparing `tmp/pelican-math-svg-0.8.2.tar.gz` & `tmp/pelican-math-svg-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican-math-svg-0.8.2.tar", max compression
+gzip compressed data, was "pelican-math-svg-0.9.0.tar", max compression
```

## Comparing `pelican-math-svg-0.8.2.tar` & `pelican-math-svg-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    32387 2021-10-15 12:28:39.139592 pelican-math-svg-0.8.2/LICENSE
--rw-r--r--   0        0        0     8074 2021-10-15 12:28:39.139592 pelican-math-svg-0.8.2/README.md
--rw-r--r--   0        0        0       45 2021-10-15 12:28:39.139592 pelican-math-svg-0.8.2/pelican/plugins/math_svg/__init__.py
--rw-r--r--   0        0        0     3380 2021-10-15 12:28:39.139592 pelican-math-svg-0.8.2/pelican/plugins/math_svg/database.py
--rw-r--r--   0        0        0      770 2021-10-15 12:28:39.139592 pelican-math-svg-0.8.2/pelican/plugins/math_svg/extension.py
--rw-r--r--   0        0        0     1858 2021-10-15 12:28:39.139592 pelican-math-svg-0.8.2/pelican/plugins/math_svg/main.py
--rw-r--r--   0        0        0     2012 2021-10-15 12:28:39.139592 pelican-math-svg-0.8.2/pelican/plugins/math_svg/markdown_extension.py
--rw-r--r--   0        0        0      429 2021-10-15 12:28:39.139592 pelican-math-svg-0.8.2/pelican/plugins/math_svg/math_svg.py
--rw-r--r--   0        0        0       75 2021-10-15 12:28:39.139592 pelican-math-svg-0.8.2/pelican/plugins/math_svg/math_svg_test.py
--rw-r--r--   0        0        0     5882 2021-10-15 12:28:39.139592 pelican-math-svg-0.8.2/pelican/plugins/math_svg/render.py
--rw-r--r--   0        0        0     3366 2021-10-15 12:28:39.139592 pelican-math-svg-0.8.2/pelican/plugins/math_svg/settings.py
--rw-r--r--   0        0        0      226 2021-10-15 12:28:39.139592 pelican-math-svg-0.8.2/pelican/plugins/math_svg/svgo.js
--rw-r--r--   0        0        0     2153 2021-10-15 12:28:55.675856 pelican-math-svg-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     9212 2021-10-15 12:28:56.703849 pelican-math-svg-0.8.2/setup.py
--rw-r--r--   0        0        0     9609 2021-10-15 12:28:56.704847 pelican-math-svg-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0    32387 2021-10-18 11:17:28.087143 pelican-math-svg-0.9.0/LICENSE
+-rw-r--r--   0        0        0     8074 2021-10-18 11:29:29.697185 pelican-math-svg-0.9.0/README.md
+-rw-r--r--   0        0        0       45 2021-10-18 11:29:29.698185 pelican-math-svg-0.9.0/pelican/plugins/math_svg/__init__.py
+-rw-r--r--   0        0        0     3380 2021-10-18 11:29:29.699185 pelican-math-svg-0.9.0/pelican/plugins/math_svg/database.py
+-rw-r--r--   0        0        0      805 2021-10-18 11:42:08.898229 pelican-math-svg-0.9.0/pelican/plugins/math_svg/extension.py
+-rw-r--r--   0        0        0     1858 2021-10-18 11:29:29.699185 pelican-math-svg-0.9.0/pelican/plugins/math_svg/main.py
+-rw-r--r--   0        0        0     2012 2021-10-18 11:29:29.699185 pelican-math-svg-0.9.0/pelican/plugins/math_svg/markdown_extension.py
+-rw-r--r--   0        0        0      429 2021-10-18 11:29:29.699185 pelican-math-svg-0.9.0/pelican/plugins/math_svg/math_svg.py
+-rw-r--r--   0        0        0       75 2021-10-18 11:29:29.699185 pelican-math-svg-0.9.0/pelican/plugins/math_svg/math_svg_test.py
+-rw-r--r--   0        0        0     5882 2021-10-18 11:29:29.700185 pelican-math-svg-0.9.0/pelican/plugins/math_svg/render.py
+-rw-r--r--   0        0        0     3366 2021-10-18 11:29:29.700185 pelican-math-svg-0.9.0/pelican/plugins/math_svg/settings.py
+-rw-r--r--   0        0        0      226 2021-10-18 11:17:28.088143 pelican-math-svg-0.9.0/pelican/plugins/math_svg/svgo.js
+-rw-r--r--   0        0        0     2130 2022-04-08 10:52:20.938097 pelican-math-svg-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     9213 2022-04-08 10:54:28.719267 pelican-math-svg-0.9.0/setup.py
+-rw-r--r--   0        0        0     9460 2022-04-08 10:54:28.720207 pelican-math-svg-0.9.0/PKG-INFO
```

### Comparing `pelican-math-svg-0.8.2/LICENSE` & `pelican-math-svg-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican-math-svg-0.8.2/README.md` & `pelican-math-svg-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pelican-math-svg-0.8.2/pelican/plugins/math_svg/database.py` & `pelican-math-svg-0.9.0/pelican/plugins/math_svg/database.py`

 * *Files identical despite different names*

### Comparing `pelican-math-svg-0.8.2/pelican/plugins/math_svg/extension.py` & `pelican-math-svg-0.9.0/pelican/plugins/math_svg/extension.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class PelicanMathExtension(markdown.Extension):
     def __init__(self, settings: PelicanMathSettings):
         super().__init__()
 
         self.settings = settings
 
     def extendMarkdown(self, md: markdown.core.Markdown):
+        md.registerExtension(self)
         md.inlinePatterns.register(
             InlineMathProcessor(
                 r"(?<!\\|\$)\$((?:[^$]|\\\$)+)(?<!\\)\$(?!\$)",
                 self.settings,
                 md,
             ),
             "inline_math",
```

### Comparing `pelican-math-svg-0.8.2/pelican/plugins/math_svg/main.py` & `pelican-math-svg-0.9.0/pelican/plugins/math_svg/main.py`

 * *Files identical despite different names*

### Comparing `pelican-math-svg-0.8.2/pelican/plugins/math_svg/markdown_extension.py` & `pelican-math-svg-0.9.0/pelican/plugins/math_svg/markdown_extension.py`

 * *Files identical despite different names*

### Comparing `pelican-math-svg-0.8.2/pelican/plugins/math_svg/render.py` & `pelican-math-svg-0.9.0/pelican/plugins/math_svg/render.py`

 * *Files identical despite different names*

### Comparing `pelican-math-svg-0.8.2/pelican/plugins/math_svg/settings.py` & `pelican-math-svg-0.9.0/pelican/plugins/math_svg/settings.py`

 * *Files identical despite different names*

### Comparing `pelican-math-svg-0.8.2/pyproject.toml` & `pelican-math-svg-0.9.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 [tool.poetry]
-name = "pelican-math-svg"
-version = "0.8.2"
-description = "Render math expressions to svg and embed them."
 authors = ["Fabian Köhler <fabian.koehler@protonmail.ch>"]
+description = "Render math expressions to svg and embed them."
+documentation = "https://docs.getpelican.com"
+keywords = ["pelican", "plugin"]
 license = "AGLP-3.0"
+name = "pelican-math-svg"
+packages = [{include = "pelican"}]
 readme = "README.md"
-keywords = ["pelican", "plugin"]
 repository = "https://github.com/f-koehler/pelican-math-svg"
-documentation = "https://docs.getpelican.com"
-packages = [{ include = "pelican" }]
+version = "0.9.0"
 
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Environment :: Console",
-    "Framework :: Pelican",
-    "Framework :: Pelican :: Plugins",
-    "Intended Audience :: End Users/Desktop",
-    "Operating System :: OS Independent",
-    "Topic :: Internet :: WWW/HTTP",
-    "Topic :: Software Development :: Libraries :: Python Modules",
+  "Development Status :: 5 - Production/Stable",
+  "Environment :: Console",
+  "Framework :: Pelican",
+  "Framework :: Pelican :: Plugins",
+  "Intended Audience :: End Users/Desktop",
+  "Operating System :: OS Independent",
+  "Topic :: Internet :: WWW/HTTP",
+  "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.urls]
 "Funding" = "https://donate.getpelican.com/"
 "Issue Tracker" = "https://github.com/f-koehler/pelican-math-svg/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
-pelican = "^4.5"
-markdown = { version = "^3.2.2", optional = true }
 lxml = "^4.6.3"
+markdown = {version = "^3.2.2", optional = true}
+pelican = "^4.5"
+python = ">=3.10,<4.0"
 setuptools = "^57.1.0"
 typer = "^0.4.0"
 
 [tool.poetry.dev-dependencies]
-black = { version = "^21.6b0", allow-prereleases = true }
+Werkzeug = "^2.0"
+bandit = "^1.6.2"
+black = {version = "^22.1", allow-prereleases = true}
 flake8 = "^4.0"
-flake8-black = "^0.2.1"
+flake8-black = "^0.3.2"
 invoke = "^1.3"
 isort = "^5.4"
+jedi = "^0.18.0"
 livereload = "^2.6"
 markdown = "^3.2.2"
-pytest = "^6.0"
+mypy = "^0.942"
+pre-commit = "^2.11.1"
+pylint = "^2.6.0"
+pytest = "^7.0"
 pytest-cov = "^3.0"
 pytest-pythonpath = "^0.7.3"
 pytest-sugar = "^0.9.4"
-Werkzeug = "^2.0"
-bandit = "^1.6.2"
-mypy = "^0.910"
-pylint = "^2.6.0"
-jedi = "^0.18.0"
-pre-commit = "^2.11.1"
 types-Markdown = "^3.3.0"
 
 [tool.poetry.scripts]
 pelican-math-svg = "pelican.plugins.math_svg.main:app"
 
 [tool.poetry.extras]
 markdown = ["markdown"]
 
 [tool.autopub]
-project-name = "math-svg"
-git-username = "f-koehler"
 git-email = "fabian.koehler@protonmail.ch"
+git-username = "f-koehler"
+project-name = "math-svg"
 
 [tool.isort]
 # Maintain compatibility with Black
-profile = "black"
 multi_line_output = 3
+profile = "black"
 
 # Sort imports within their section independent of the import type
 force_sort_within_sections = true
 
 # Designate "pelican" as separate import section
 known_pelican = "pelican"
 sections = "FUTURE,STDLIB,THIRDPARTY,PELICAN,FIRSTPARTY,LOCALFOLDER"
 
 [build-system]
-requires = ["poetry>=1.0.0"]
 build-backend = "poetry.masonry.api"
+requires = ["poetry>=1.0.0"]
```

### Comparing `pelican-math-svg-0.8.2/setup.py` & `pelican-math-svg-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 {'markdown': ['markdown>=3.2.2,<4.0.0']}
 
 entry_points = \
 {'console_scripts': ['pelican-math-svg = pelican.plugins.math_svg.main:app']}
 
 setup_kwargs = {
     'name': 'pelican-math-svg',
-    'version': '0.8.2',
+    'version': '0.9.0',
     'description': 'Render math expressions to svg and embed them.',
     'long_description': '# math-svg: A Plugin for Pelican\n\n[![Build Status](https://img.shields.io/github/workflow/status/f-koehler/pelican-math-svg/build)](https://github.com/f-koehler/pelican-math-svg/actions)\n[![PyPI Version](https://img.shields.io/pypi/v/pelican-math-svg)](https://pypi.org/project/pelican-math-svg/)\n![License](https://img.shields.io/pypi/l/pelican-math-svg?color=blue)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/f-koehler/pelican-math-svg/main.svg)](https://results.pre-commit.ci/latest/github/f-koehler/pelican-math-svg/main)\n\nRender math expressions to svg and embed them.\n\n## Installation\n\nThis plugin can be installed via:\n\n```shell\npython -m pip install pelican-math-svg\n```\n\nAfterwards, add the plugin to the `PLUGINS` list in your `pelicanconf.py` file, e.g.:\n\n```python\nPLUGINS = [\n    "math_svg",\n]\n```\n\n## Multi-Core Rendering\n\nTo use multi-core rendering of equations (highly recommended, especially when many equations have to be rendered) change the `html` target in the `Makefile` of your pelican site to a three step process:\n\n```makefile\nhtml:\n    PELICAN_MATH_SVG_DRY=True "$(PELICAN)" "$(INPUTDIR)" -o "$(OUTPUTDIR)" -s "$(CONFFILE)" $(PELICANOPTS)\n    pelican-math-svg render -j $(shell nproc)\n    "$(PELICAN)" "$(INPUTDIR)" -o "$(OUTPUTDIR)" -s "$(CONFFILE)" $(PELICANOPTS)\n```\n\nThe first commands will execute `math-svg` in dry-mode and only populate the equation database without actually rendering anything.\nThe second command will render all missing equations in parallel.\nThe number of threads is specified by the `-j` flag, in this example all CPU cores are used.\nReplace `$(shell nproc)` with a number to use a fixed number of cores.\nThe last command is the usual pelican command and produces the output files again, know including the rendered equations.\n\n## Requirements\n\n-   required LaTeX tools (all included in TeX Live and possibly other LaTeX distributions):\n    -   `lualatex` (or another LaTeX compiler if changed in the settings, [see below](#configuration))\n    -   `pdfcrop`\n    -   `dvisvgm`\n-   `scour` (optional)\n-   `svgo` (optional)\n\n## Usage\n\nIn Markdown you can use `$x$` for inline math and\n\n```\n$$\n  \\int x^2\n$$\n```\n\nfor display math.\n\nIt is required to set the stroke color using the `strokeonly` class (this class name can be changed, see [configuration options below](#configuration)), otherwise lines would be rendered white:\n\n```css\nsvg path.strokeonly {\n    color: #000;\n}\n```\n\nTo change the fill color for equations as well, thus essential changing the default color for math, specify the following additionally:\n\n```css\nspan.math svg path,\ndiv.math svg path {\n    fill: #000;\n}\n```\n\n## Configuration\n\nIn your `pelicanconf.py` you can use the following options to tweak the behavior of the plugin:\n\n| Setting                         | Description                                                                                                                 | Default Value                                                                                                                                       |\n| ------------------------------- | --------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |\n| `MATH_SVG["titles"]             | Whether to generate `<title>` tags containing the raw LaTeX code (recommended for accessibility).                           | `True`                                                                                                                                              |\n| `MATH_SVG["scale_inline"]`      | scaling factor for inline math                                                                                              | `1.0`                                                                                                                                               |\n| `MATH_SVG["scale_display"]`     | scaling factor for display math                                                                                             | `1.0`                                                                                                                                               |\n| `MATH_SVG["strokeonly_class]`   | CSS class for SVG paths that have no filling and a black stroke color, useful when changing the color of rendered equations | `strokeonly`                                                                                                                                        |\n| `MATH_SVG["latex"]["args"]`     | CLI arguments of the invoked LaTeX compiler                                                                                 | `"--interaction=errorstopmode", "--halt-on-error"`                                                                                                  |\n| `MATH_SVG["latex"]["preamble"]` | preamble of the generated LaTeX document                                                                                    | `[r"\\documentclass[preview,border={2pt 0pt}]{standalone}",r"\\usepackage{amsmath}",r"\\usepackage{amssymb}",]`                                        |\n| `MATH_SVG["latex"]["program"]`  | LaTeX compiler to use                                                                                                       | `lualatex`                                                                                                                                          |\n| `MATH_SVG["pdfcrop"]["args"]`   | CLI arguments for `pdfcrop`                                                                                                 | `--hires`                                                                                                                                           |\n| `MATH_SVG["dvisvgm"]["args"]`   | CLI arguments for `dvisvgm`                                                                                                 | `["--pdf", "--optimize=all", "--no-fonts", "--exact-bbox"]`                                                                                         |\n| `MATH_SVG["scour"]["args"]`     | CLI arguments for `scour`                                                                                                   | `["--strip-xml-prolog", "--remove-descriptions", "--remove-metadata", "--enable-comment-stripping", "--strip-xml-space", "--enable-id-stripping",]` |\n| `MATH_SVG["scour"]["enabled"]`  | whether to use `scour` to optimize SVG output                                                                               | `True` if `scour` is in `$PATH`, `False` otherwise                                                                                                  |\n| `MATH_SVG["svgo"]["args"]`      | CLI arguments for `svgo`                                                                                                    | `["--multipass", "--precision", "5"]`                                                                                                               |\n| `MATH_SVG["svgo"]["enabled"]`   | whether to use `svgo` to optimize SVG output                                                                                | `True` if `svgo` is in `$PATH`, `False` otherwise                                                                                                   |\n\n## Contributing\n\nContributions are welcome and much appreciated. Every little bit helps. You can contribute by improving the documentation, adding missing features, and fixing bugs. You can also help out by reviewing and commenting on [existing issues][].\n\nTo start contributing to this plugin, review the [Contributing to Pelican][] documentation, beginning with the **Contributing Code** section.\n\n[existing issues]: https://github.com/f-koehler/pelican-math-svg/issues\n[contributing to pelican]: https://docs.getpelican.com/en/latest/contribute.html\n\n## License\n\nThis project is licensed under the GPLv3 license.\n',
     'author': 'Fabian Köhler',
     'author_email': 'fabian.koehler@protonmail.ch',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/f-koehler/pelican-math-svg',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pelican-math-svg-0.8.2/PKG-INFO` & `pelican-math-svg-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Metadata-Version: 2.1
 Name: pelican-math-svg
-Version: 0.8.2
+Version: 0.9.0
 Summary: Render math expressions to svg and embed them.
 Home-page: https://github.com/f-koehler/pelican-math-svg
 License: AGLP-3.0
 Keywords: pelican,plugin
 Author: Fabian Köhler
 Author-email: fabian.koehler@protonmail.ch
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Pelican
 Classifier: Framework :: Pelican :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: markdown
 Requires-Dist: lxml (>=4.6.3,<5.0.0)
 Requires-Dist: markdown (>=3.2.2,<4.0.0); extra == "markdown"
 Requires-Dist: pelican (>=4.5,<5.0)
 Requires-Dist: setuptools (>=57.1.0,<58.0.0)
```

