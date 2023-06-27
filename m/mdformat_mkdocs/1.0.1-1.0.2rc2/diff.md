# Comparing `tmp/mdformat_mkdocs-1.0.1.tar.gz` & `tmp/mdformat_mkdocs-1.0.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdformat_mkdocs-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mdformat_mkdocs-1.0.2rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mdformat_mkdocs-1.0.1.tar` & `mdformat_mkdocs-1.0.2rc2.tar`

### file list

```diff
@@ -1,12 +1,19 @@
--rw-r--r--   0        0        0     1819 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/.gitignore
--rw-r--r--   0        0        0     1729 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      296 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/.pre-commit-test.yaml
--rw-r--r--   0        0        0       33 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/.tool-versions
--rw-r--r--   0        0        0      921 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1073 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/LICENSE
--rw-r--r--   0        0        0     2589 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/README.md
--rw-r--r--   0        0        0      134 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/mdformat_mkdocs/__init__.py
--rw-r--r--   0        0        0     2764 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/mdformat_mkdocs/plugin.py
--rw-r--r--   0        0        0     1639 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      789 2023-06-05 22:05:28.405867 mdformat_mkdocs-1.0.1/tox.ini
--rw-r--r--   0        0        0     4018 1970-01-01 00:00:00.000000 mdformat_mkdocs-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1819 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/.gitignore
+-rw-r--r--   0        0        0     1756 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      573 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/.pre-commit-test.yaml
+-rw-r--r--   0        0        0       33 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/.tool-versions
+-rw-r--r--   0        0        0      979 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1073 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/LICENSE
+-rw-r--r--   0        0        0     3095 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/README.md
+-rw-r--r--   0        0        0      175 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/mdformat_mkdocs/__init__.py
+-rw-r--r--   0        0        0     3613 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/mdformat_mkdocs/plugin.py
+-rw-r--r--   0        0        0      402 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/mkdocs-demo/README.md
+-rw-r--r--   0        0        0      672 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/mkdocs-demo/docs/README.md
+-rw-r--r--   0        0        0    78687 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/mkdocs-demo/mkdcs-demo-screenshot.png
+-rw-r--r--   0        0        0       42 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/mkdocs-demo/mkdocs.yml
+-rw-r--r--   0        0        0        0 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/mkdocs-demo/mkdocs_demo/__init__.py
+-rw-r--r--   0        0        0    24503 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/mkdocs-demo/poetry.lock
+-rw-r--r--   0        0        0      372 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/mkdocs-demo/pyproject.toml
+-rw-r--r--   0        0        0     1639 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/pyproject.toml
+-rw-r--r--   0        0        0      789 2023-06-27 12:30:14.064278 mdformat_mkdocs-1.0.2rc2/tox.ini
+-rw-r--r--   0        0        0     4527 1970-01-01 00:00:00.000000 mdformat_mkdocs-1.0.2rc2/PKG-INFO
```

### Comparing `mdformat_mkdocs-1.0.1/.gitignore` & `mdformat_mkdocs-1.0.2rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.1/.pre-commit-config.yaml` & `mdformat_mkdocs-1.0.2rc2/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -48,15 +48,15 @@
           - flake8-comprehensions>=3.4.0
         args: [--ignore=E501]
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
       - id: mdformat
         additional_dependencies: ['mdformat-mkdocs[recommended]']
-        exclude: tests/.+\.md
+        exclude: tests/.+\.md|mkdocs-demo/docs/README.md
         args: [--wrap=no]
   - repo: https://github.com/lyz-code/yamlfix/
     rev: 1.9.0
     hooks:
       - id: yamlfix
         types_or: []
         types: [file, yaml]
```

### Comparing `mdformat_mkdocs-1.0.1/CONTRIBUTING.md` & `mdformat_mkdocs-1.0.2rc2/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -46,10 +46,10 @@
 Either use flit directly:
 
 ```bash
 pip install flit
 flit publish
 ```
 
-or trigger the GitHub Action job, by creating a release with a tag equal to the version, e.g. `v0.0.1`.
+or trigger the GitHub Action job, by creating a release with a tag equal to the version, e.g. `v0.0.1` and updating the version in `mdformat_mkdocs/__init__.py`.
 
 Note, this requires generating an API key on PyPi and adding it to the repository `Settings/Secrets`, under the name `PYPI_KEY`.
```

### Comparing `mdformat_mkdocs-1.0.1/LICENSE` & `mdformat_mkdocs-1.0.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.1/README.md` & `mdformat_mkdocs-1.0.2rc2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![Build Status][ci-badge]][ci-link] [![PyPI version][pypi-badge]][pypi-link]
 
 <!-- [![codecov.io][cov-badge]][cov-link]
 [cov-badge]: https://codecov.io/gh/executablebooks/mdformat-mkdocs/branch/main/graph/badge.svg
 [cov-link]: https://codecov.io/gh/executablebooks/mdformat-mkdocs
  -->
 
-An [mdformat](https://github.com/executablebooks/mdformat) plugin for mkdocs.
+An [mdformat](https://github.com/executablebooks/mdformat) plugin for [mkdocs](https://github.com/mkdocs/mkdocs).
 
 ## Usage
 
 Add this package wherever you use `mdformat` and the plugin will be auto-recognized. No additional configuration necessary. See [additional information on `mdformat` plugins here](https://mdformat.readthedocs.io/en/stable/users/plugins.html)
 
 Tip: this package specifies an "extra" (`recommended`) for plugins that work well with mkdocs:
 
@@ -52,14 +52,28 @@
 ## Caveats
 
 - All indents are converted to 4-spaces
 - This plugin converts all bulleted items to dashes (`-`) and numerals to `1.`
 
 See the example test files, [./tests/pre-commit-test.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/pre-commit-test.md) and [./tests/fixtures.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/fixtures.md)
 
+## Configuration
+
+`mdformat-mkdocs` adds the CLI argument `--align-semantic-breaks-in-numbered-lists` to optionally align line breaks in numbered lists to 3-spaces. If not specified, the default of 4-indents is followed universally.
+
+```txt
+# with: mdformat
+1. Semantic line feed where the following line is
+    three spaces deep
+
+# vs. with: mdformat --align-semantic-breaks-in-numbered-lists
+1. Semantic line feed where the following line is
+   three spaces deep
+```
+
 ## Contributing
 
 See [CONTRIBUTING.md](https://github.com/KyleKing/mdformat-mkdocs/blob/main/CONTRIBUTING.md)
 
 [ci-badge]: https://github.com/kyleking/mdformat-mkdocs/workflows/CI/badge.svg?branch=main
 [ci-link]: https://github.com/kyleking/mdformat-mkdocs/actions?query=workflow%3ACI+branch%3Amain+event%3Apush
 [pypi-badge]: https://img.shields.io/pypi/v/mdformat-mkdocs.svg
```

### Comparing `mdformat_mkdocs-1.0.1/mdformat_mkdocs/plugin.py` & `mdformat_mkdocs-1.0.2rc2/mdformat_mkdocs/plugin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,37 @@
+import argparse
 import re
 from typing import Dict, Mapping
 
 from markdown_it import MarkdownIt
 from mdformat.renderer import RenderContext, RenderTreeNode
 from mdformat.renderer.typing import Postprocess, Render
 
 _MKDOCS_INDENT_COUNT = 4
 """Use 4-spaces for mkdocs."""
 
+_ALIGN_SEMANTIC_BREAKS_IN_NUMBERED_LISTS = False
+"""use 3-space on subsequent lines in semantic lists."""
+
+
+def add_cli_options(parser: argparse.ArgumentParser) -> None:
+    """Add options to the mdformat CLI, to be stored in `mdit.options["mdformat"]`."""
+    parser.add_argument(
+        "--align-semantic-breaks-in-numbered-lists",
+        action="store_true",
+        help="If specified, align semantic indents in numbered lists to the text",
+    )
+
 
 def update_mdit(mdit: MarkdownIt) -> None:
     """No changes to markdown parsing are necessary."""
-    ...
+    global _ALIGN_SEMANTIC_BREAKS_IN_NUMBERED_LISTS
+    _ALIGN_SEMANTIC_BREAKS_IN_NUMBERED_LISTS = mdit.options["mdformat"].get(
+        "align_semantic_breaks_in_numbered_lists", False
+    )
 
 
 _RE_INDENT = re.compile(r"(?P<indent>\s*)(?P<content>[^\s]?.*)")
 """Match `indent` and `content` against line`."""
 
 _RE_LIST_ITEM = re.compile(r"(?P<bullet>[\-\*\d\.]+)\s+(?P<item>.+)")
 """Match `bullet` and `item` against `content`."""
@@ -26,21 +42,23 @@
     eol = "\n"
     indent = " " * _MKDOCS_INDENT_COUNT
 
     rendered = ""
     last_indent = ""
     indent_counter = 0
     indent_lookup: Dict[str, int] = {}
+    is_numbered = False
     for line in text.split(eol):
         match = _RE_INDENT.match(line)
         assert match is not None  # for pylint
         list_match = _RE_LIST_ITEM.match(match["content"])
         new_line = line
         if list_match:
-            new_bullet = "-" if list_match["bullet"] in {"-", "*"} else "1."
+            is_numbered = list_match["bullet"] not in {"-", "*"}
+            new_bullet = "1." if is_numbered else "-"
             new_line = f'{new_bullet} {list_match["item"]}'
 
         this_indent = match["indent"]
         if this_indent:
             indent_diff = len(this_indent) - len(last_indent)
             if indent_diff == 0:
                 ...
@@ -51,14 +69,16 @@
                 indent_counter = indent_lookup[this_indent]
             else:
                 raise NotImplementedError(f"Error in indentation of: `{line}`")
         else:
             indent_counter = 0
         last_indent = this_indent
         new_indent = indent * indent_counter
+        if _ALIGN_SEMANTIC_BREAKS_IN_NUMBERED_LISTS and not list_match and is_numbered:
+            new_indent = new_indent[:-1]
         rendered += f"{new_indent}{new_line.strip()}{eol}"
     return rendered.rstrip()
 
 
 # A mapping from `RenderTreeNode.type` to a `Render` function that can
 # render the given `RenderTreeNode` type. These override the default
 # `Render` funcs defined in `mdformat.renderer.DEFAULT_RENDERERS`.
```

### Comparing `mdformat_mkdocs-1.0.1/pyproject.toml` & `mdformat_mkdocs-1.0.2rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.1/tox.ini` & `mdformat_mkdocs-1.0.2rc2/tox.ini`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.1/PKG-INFO` & `mdformat_mkdocs-1.0.2rc2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdformat_mkdocs
-Version: 1.0.1
+Version: 1.0.2rc2
 Summary: An mdformat plugin for mkdocs.
 Keywords: mdformat,markdown,markdown-it
 Author-email: Kyle King <dev.act.kyle@gmail.com>
 Requires-Python: >=3.7.2
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -36,15 +36,15 @@
 [![Build Status][ci-badge]][ci-link] [![PyPI version][pypi-badge]][pypi-link]
 
 <!-- [![codecov.io][cov-badge]][cov-link]
 [cov-badge]: https://codecov.io/gh/executablebooks/mdformat-mkdocs/branch/main/graph/badge.svg
 [cov-link]: https://codecov.io/gh/executablebooks/mdformat-mkdocs
  -->
 
-An [mdformat](https://github.com/executablebooks/mdformat) plugin for mkdocs.
+An [mdformat](https://github.com/executablebooks/mdformat) plugin for [mkdocs](https://github.com/mkdocs/mkdocs).
 
 ## Usage
 
 Add this package wherever you use `mdformat` and the plugin will be auto-recognized. No additional configuration necessary. See [additional information on `mdformat` plugins here](https://mdformat.readthedocs.io/en/stable/users/plugins.html)
 
 Tip: this package specifies an "extra" (`recommended`) for plugins that work well with mkdocs:
 
@@ -85,14 +85,28 @@
 ## Caveats
 
 - All indents are converted to 4-spaces
 - This plugin converts all bulleted items to dashes (`-`) and numerals to `1.`
 
 See the example test files, [./tests/pre-commit-test.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/pre-commit-test.md) and [./tests/fixtures.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/fixtures.md)
 
+## Configuration
+
+`mdformat-mkdocs` adds the CLI argument `--align-semantic-breaks-in-numbered-lists` to optionally align line breaks in numbered lists to 3-spaces. If not specified, the default of 4-indents is followed universally.
+
+```txt
+# with: mdformat
+1. Semantic line feed where the following line is
+    three spaces deep
+
+# vs. with: mdformat --align-semantic-breaks-in-numbered-lists
+1. Semantic line feed where the following line is
+   three spaces deep
+```
+
 ## Contributing
 
 See [CONTRIBUTING.md](https://github.com/KyleKing/mdformat-mkdocs/blob/main/CONTRIBUTING.md)
 
 [ci-badge]: https://github.com/kyleking/mdformat-mkdocs/workflows/CI/badge.svg?branch=main
 [ci-link]: https://github.com/kyleking/mdformat-mkdocs/actions?query=workflow%3ACI+branch%3Amain+event%3Apush
 [pypi-badge]: https://img.shields.io/pypi/v/mdformat-mkdocs.svg
```

