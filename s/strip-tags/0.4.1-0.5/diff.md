# Comparing `tmp/strip-tags-0.4.1.tar.gz` & `tmp/strip-tags-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strip-tags-0.4.1.tar", last modified: Sun Jun 18 08:39:13 2023, max compression
+gzip compressed data, was "strip-tags-0.5.tar", last modified: Tue Jun 27 20:28:52 2023, max compression
```

## Comparing `strip-tags-0.4.1.tar` & `strip-tags-0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:39:13.579093 strip-tags-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 08:38:56.000000 strip-tags-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-18 08:39:13.579093 strip-tags-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-06-18 08:38:56.000000 strip-tags-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 08:39:13.579093 strip-tags-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-18 08:38:56.000000 strip-tags-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:39:13.579093 strip-tags-0.4.1/strip_tags/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-18 08:38:56.000000 strip-tags-0.4.1/strip_tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 08:38:56.000000 strip-tags-0.4.1/strip_tags/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-18 08:38:56.000000 strip-tags-0.4.1/strip_tags/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-18 08:38:56.000000 strip-tags-0.4.1/strip_tags/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:39:13.579093 strip-tags-0.4.1/strip_tags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-18 08:39:13.000000 strip-tags-0.4.1/strip_tags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-18 08:39:13.000000 strip-tags-0.4.1/strip_tags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 08:39:13.000000 strip-tags-0.4.1/strip_tags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-18 08:39:13.000000 strip-tags-0.4.1/strip_tags.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 08:39:13.000000 strip-tags-0.4.1/strip_tags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 08:39:13.000000 strip-tags-0.4.1/strip_tags.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:39:13.579093 strip-tags-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-06-18 08:38:56.000000 strip-tags-0.4.1/tests/test_strip_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:28:52.656208 strip-tags-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 20:28:35.000000 strip-tags-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-06-27 20:28:52.656208 strip-tags-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-27 20:28:35.000000 strip-tags-0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 20:28:52.656208 strip-tags-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-27 20:28:35.000000 strip-tags-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:28:52.656208 strip-tags-0.5/strip_tags/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-27 20:28:35.000000 strip-tags-0.5/strip_tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-27 20:28:35.000000 strip-tags-0.5/strip_tags/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-27 20:28:35.000000 strip-tags-0.5/strip_tags/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-06-27 20:28:35.000000 strip-tags-0.5/strip_tags/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:28:52.656208 strip-tags-0.5/strip_tags.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-06-27 20:28:52.000000 strip-tags-0.5/strip_tags.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-27 20:28:52.000000 strip-tags-0.5/strip_tags.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 20:28:52.000000 strip-tags-0.5/strip_tags.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-27 20:28:52.000000 strip-tags-0.5/strip_tags.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-27 20:28:52.000000 strip-tags-0.5/strip_tags.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-27 20:28:52.000000 strip-tags-0.5/strip_tags.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:28:52.656208 strip-tags-0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-27 20:28:35.000000 strip-tags-0.5/tests/test_strip_tags.py
```

### Comparing `strip-tags-0.4.1/LICENSE` & `strip-tags-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `strip-tags-0.4.1/PKG-INFO` & `strip-tags-0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strip-tags
-Version: 0.4.1
+Version: 0.5
 Summary: Strip tags from HTML, optionally from areas identified by CSS selectors
 Home-page: https://github.com/simonw/strip-tags
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/strip-tags/issues
 Project-URL: CI, https://github.com/simonw/strip-tags/actions
 Project-URL: Changelog, https://github.com/simonw/strip-tags/releases
@@ -48,14 +48,18 @@
 ```bash
 cat input.html | strip-tags '.content' '.sidebar' > output.txt
 ```
 To return just the first element on the page that matches one of the selectors, use `--first`:
 ```bash
 cat input.html | strip-tags .content --first > output.txt
 ```
+To remove content contained by specific selectors - e.g. the `<nav>` section of a page, use `-r` or `--remove`:
+```bash
+cat input.html | strip-tags -r nav > output.txt
+```
 To minify whitespace - reducing multiple space and tab characters to a single space, and multiple newlines and spaces to a maximum of two newlines - add `-m` or `--minify`:
 ```bash
 cat input.html | strip-tags -m > output.txt
 ```
 You can also run this command using `python -m` like this:
 ```bash
 python -m strip_tags --help
@@ -66,14 +70,15 @@
 
 The `-t/--keep-tag` option can be passed multiple times to specify tags that should be kept.
 
 This example looks at the `<header>` section of https://datasette.io/ and keeps the tags around the list items and `<h1>` elements:
 
 ```
 curl -s https://datasette.io/ | strip-tags header -t h1 -t li
+```
 ```html
 <li>Uses</li>
 <li>Documentation Docs</li>
 <li>Tutorials</li>
 <li>Examples</li>
 <li>Plugins</li>
 <li>Tools</li>
@@ -87,34 +92,61 @@
 
 The `href` attribute on links, the `alt` attribute on images and the `name` and `value` attributes on `meta` tags are kept as well.
 
 You can also specify a bundle of tags. For example, `strip-tags -t hs` will keep the tag markup for all levels of headings.
 
 The following bundles can be used:
 
+<!-- [[[cog
+import cog
+from strip_tags.lib import BUNDLES
+lines = []
+for name, tags in BUNDLES.items():
+    lines.append("- `-t {}`: {}".format(name, ", ".join("`<{}>`".format(tag) for tag in tags)))
+cog.out("\n".join(lines))
+]]] -->
 - `-t hs`: `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`
 - `-t metadata`: `<title>`, `<meta>`
-- `-t structure`: `<header>`, `<section>`, `<main>`, `<aside>`, `<footer>`, `<article>`, `<nav>`
-
+- `-t structure`: `<header>`, `<nav>`, `<main>`, `<article>`, `<section>`, `<aside>`, `<footer>`
+- `-t tables`: `<table>`, `<tr>`, `<td>`, `<th>`, `<thead>`, `<tbody>`, `<tfoot>`, `<caption>`, `<colgroup>`, `<col>`
+- `-t lists`: `<ul>`, `<ol>`, `<li>`, `<dl>`, `<dd>`, `<dt>`
+<!-- [[[end]]] -->
 
 ## As a Python library
 
 You can use `strip-tags` from Python code too. The function signature looks like this:
 
+<!-- [[[cog
+import ast
+module = ast.parse(open("strip_tags/lib.py").read())
+strip_tags = [
+    fn for fn in module.body
+    if getattr(fn, 'name', None) == 'strip_tags'
+][0]
+code = ast.unparse(strip_tags)
+defline = code.split("\n")[0]
+code = (
+    ',\n    '.join(defline.split(', ')).replace(") ->", "\n) ->").replace("strip_tags(", "strip_tags(\n    ")
+)
+cog.out("```python\n{}\n```".format(code))
+]]] -->
 ```python
 def strip_tags(
     input: str,
-    selectors: Optional[Iterable[str]] = None,
+    selectors: Optional[Iterable[str]]=None,
     *,
-    minify: bool = False,
-    first: bool = False,
-    keep_tags: Optional[Iterable[str]] = None,
-    all_attrs: bool = False,
+    removes: Optional[Iterable[str]]=None,
+    minify: bool=False,
+    first: bool=False,
+    keep_tags: Optional[Iterable[str]]=None,
+    all_attrs: bool=False
 ) -> str:
 ```
+<!-- [[[end]]] -->
+
 Here's an example:
 ```python
 from strip_tags import strip_tags
 
 html = """
 <div>
 <h1>This has tags</h1>
@@ -129,14 +161,53 @@
 Output:
 ```
 <h1>This has tags</h1>
 
 And whitespace too
 ```
 
+## strip-tags --help
+
+<!-- [[[cog
+import cog
+from strip_tags import cli
+from click.testing import CliRunner
+runner = CliRunner()
+result = runner.invoke(cli.cli, ["--help"])
+help = result.output.replace("Usage: cli", "Usage: strip-tags")
+cog.out(
+    "```\n{}\n```".format(help)
+)
+]]] -->
+```
+Usage: strip-tags [OPTIONS] [SELECTORS]...
+
+  Strip tags from HTML, optionally from areas identified by CSS selectors
+
+  Example usage:
+
+      cat input.html | strip-tags > output.txt
+
+  To run against just specific areas identified by CSS selectors:
+
+      cat input.html | strip-tags .entry .footer > output.txt
+
+Options:
+  --version             Show the version and exit.
+  -r, --remove TEXT     Remove content in these selectors
+  -i, --input FILENAME  Input file
+  -m, --minify          Minify whitespace
+  -t, --keep-tag TEXT   Keep these <tags>
+  --all-attrs           Include all attributes on kept tags
+  --first               First element matching the selectors
+  --help                Show this message and exit.
+
+```
+<!-- [[[end]]] -->
+
 ## Development
 
 To contribute to this tool, first checkout the code. Then create a new virtual environment:
 ```bash
 cd strip-tags
 python -m venv venv
 source venv/bin/activate
```

### Comparing `strip-tags-0.4.1/setup.py` & `strip-tags-0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.4.1"
+VERSION = "0.5"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -28,10 +28,10 @@
     version=VERSION,
     packages=["strip_tags"],
     entry_points="""
         [console_scripts]
         strip-tags=strip_tags.cli:cli
     """,
     install_requires=["click", "beautifulsoup4", "html5lib"],
-    extras_require={"test": ["pytest", "pytest-icdiff"]},
+    extras_require={"test": ["pytest", "PyYAML", "cogapp"]},
     python_requires=">=3.7",
 )
```

### Comparing `strip-tags-0.4.1/strip_tags/cli.py` & `strip-tags-0.5/strip_tags/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,33 +2,41 @@
 
 from strip_tags import strip_tags
 
 
 @click.command()
 @click.version_option()
 @click.argument("selectors", nargs=-1)
-@click.option("-i", "--input", type=click.File("r"), default="-")
+@click.option(
+    "removes",
+    "-r",
+    "--remove",
+    multiple=True,
+    help="Remove content in these selectors",
+)
+@click.option("-i", "--input", type=click.File("r"), default="-", help="Input file")
 @click.option("-m", "--minify", is_flag=True, help="Minify whitespace")
 @click.option("keep_tags", "-t", "--keep-tag", multiple=True, help="Keep these <tags>")
 @click.option("--all-attrs", is_flag=True, help="Include all attributes on kept tags")
 @click.option("--first", is_flag=True, help="First element matching the selectors")
-def cli(selectors, input, minify, keep_tags, all_attrs, first):
+def cli(selectors, removes, input, minify, keep_tags, all_attrs, first):
     """
     Strip tags from HTML, optionally from areas identified by CSS selectors
 
     Example usage:
 
         cat input.html | strip-tags > output.txt
 
     To run against just specific areas identified by CSS selectors:
 
         cat input.html | strip-tags .entry .footer > output.txt
     """
     final = strip_tags(
         input,
         selectors,
+        removes=removes,
         minify=minify,
         first=first,
         keep_tags=keep_tags,
         all_attrs=all_attrs,
     )
     click.echo(final)
```

### Comparing `strip-tags-0.4.1/strip_tags/lib.py` & `strip-tags-0.5/strip_tags/lib.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import Iterable, Optional
 
-from bs4 import BeautifulSoup, NavigableString
+from bs4 import BeautifulSoup, Comment, NavigableString
 
 # Elements that should be followed by a newline, derived from
 # https://www.w3.org/TR/2011/WD-html5-20110405/rendering.html#display-types
 NEWLINE_ELEMENTS = (
     # display: block; default in the spec
     "address",
     "article",
@@ -89,38 +89,57 @@
     "track",
     "wbr",
 }
 
 BUNDLES = {
     "hs": ("h1", "h2", "h3", "h4", "h5", "h6"),
     "metadata": ("title", "meta"),
-    "structure": {"header", "nav", "main", "article", "section", "aside", "footer"},
+    "structure": ("header", "nav", "main", "article", "section", "aside", "footer"),
+    "tables": (
+        "table",
+        "tr",
+        "td",
+        "th",
+        "thead",
+        "tbody",
+        "tfoot",
+        "caption",
+        "colgroup",
+        "col",
+    ),
+    "lists": ("ul", "ol", "li", "dl", "dd", "dt"),
 }
 
 ATTRS_TO_KEEP = {
     "a": {"href"},
     "img": {"alt"},
     "meta": {"name", "value"},
 }
 
 
 def strip_tags(
     input: str,
     selectors: Optional[Iterable[str]] = None,
     *,
+    removes: Optional[Iterable[str]] = None,
     minify: bool = False,
     first: bool = False,
     keep_tags: Optional[Iterable[str]] = None,
     all_attrs: bool = False,
 ) -> str:
     soup = BeautifulSoup(input, "html5lib", multi_valued_attributes=False)
     if not selectors:
         selectors = ["body"]
     output = []
 
+    if removes:
+        for remove in removes:
+            for tag in soup.select(remove):
+                tag.decompose()
+
     keep_tags = keep_tags or []
 
     if keep_tags:
         # Expand any bundles
         expanded_keep_tags = []
         for tag in keep_tags:
             if tag in BUNDLES:
@@ -158,14 +177,16 @@
             break
 
     return "".join(output).strip()
 
 
 def process_node(node, minify, keep_tags, all_attrs=False):
     # Recursively process a tag or NavigableString
+    if isinstance(node, Comment):
+        return ""
     if isinstance(node, NavigableString):
         if minify:
             minified = _whitespace_re.sub(repl, node)
             if minified == "\n":
                 minified = " "
             return minified
         else:
```

### Comparing `strip-tags-0.4.1/strip_tags.egg-info/PKG-INFO` & `strip-tags-0.5/strip_tags.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strip-tags
-Version: 0.4.1
+Version: 0.5
 Summary: Strip tags from HTML, optionally from areas identified by CSS selectors
 Home-page: https://github.com/simonw/strip-tags
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/strip-tags/issues
 Project-URL: CI, https://github.com/simonw/strip-tags/actions
 Project-URL: Changelog, https://github.com/simonw/strip-tags/releases
@@ -48,14 +48,18 @@
 ```bash
 cat input.html | strip-tags '.content' '.sidebar' > output.txt
 ```
 To return just the first element on the page that matches one of the selectors, use `--first`:
 ```bash
 cat input.html | strip-tags .content --first > output.txt
 ```
+To remove content contained by specific selectors - e.g. the `<nav>` section of a page, use `-r` or `--remove`:
+```bash
+cat input.html | strip-tags -r nav > output.txt
+```
 To minify whitespace - reducing multiple space and tab characters to a single space, and multiple newlines and spaces to a maximum of two newlines - add `-m` or `--minify`:
 ```bash
 cat input.html | strip-tags -m > output.txt
 ```
 You can also run this command using `python -m` like this:
 ```bash
 python -m strip_tags --help
@@ -66,14 +70,15 @@
 
 The `-t/--keep-tag` option can be passed multiple times to specify tags that should be kept.
 
 This example looks at the `<header>` section of https://datasette.io/ and keeps the tags around the list items and `<h1>` elements:
 
 ```
 curl -s https://datasette.io/ | strip-tags header -t h1 -t li
+```
 ```html
 <li>Uses</li>
 <li>Documentation Docs</li>
 <li>Tutorials</li>
 <li>Examples</li>
 <li>Plugins</li>
 <li>Tools</li>
@@ -87,34 +92,61 @@
 
 The `href` attribute on links, the `alt` attribute on images and the `name` and `value` attributes on `meta` tags are kept as well.
 
 You can also specify a bundle of tags. For example, `strip-tags -t hs` will keep the tag markup for all levels of headings.
 
 The following bundles can be used:
 
+<!-- [[[cog
+import cog
+from strip_tags.lib import BUNDLES
+lines = []
+for name, tags in BUNDLES.items():
+    lines.append("- `-t {}`: {}".format(name, ", ".join("`<{}>`".format(tag) for tag in tags)))
+cog.out("\n".join(lines))
+]]] -->
 - `-t hs`: `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`
 - `-t metadata`: `<title>`, `<meta>`
-- `-t structure`: `<header>`, `<section>`, `<main>`, `<aside>`, `<footer>`, `<article>`, `<nav>`
-
+- `-t structure`: `<header>`, `<nav>`, `<main>`, `<article>`, `<section>`, `<aside>`, `<footer>`
+- `-t tables`: `<table>`, `<tr>`, `<td>`, `<th>`, `<thead>`, `<tbody>`, `<tfoot>`, `<caption>`, `<colgroup>`, `<col>`
+- `-t lists`: `<ul>`, `<ol>`, `<li>`, `<dl>`, `<dd>`, `<dt>`
+<!-- [[[end]]] -->
 
 ## As a Python library
 
 You can use `strip-tags` from Python code too. The function signature looks like this:
 
+<!-- [[[cog
+import ast
+module = ast.parse(open("strip_tags/lib.py").read())
+strip_tags = [
+    fn for fn in module.body
+    if getattr(fn, 'name', None) == 'strip_tags'
+][0]
+code = ast.unparse(strip_tags)
+defline = code.split("\n")[0]
+code = (
+    ',\n    '.join(defline.split(', ')).replace(") ->", "\n) ->").replace("strip_tags(", "strip_tags(\n    ")
+)
+cog.out("```python\n{}\n```".format(code))
+]]] -->
 ```python
 def strip_tags(
     input: str,
-    selectors: Optional[Iterable[str]] = None,
+    selectors: Optional[Iterable[str]]=None,
     *,
-    minify: bool = False,
-    first: bool = False,
-    keep_tags: Optional[Iterable[str]] = None,
-    all_attrs: bool = False,
+    removes: Optional[Iterable[str]]=None,
+    minify: bool=False,
+    first: bool=False,
+    keep_tags: Optional[Iterable[str]]=None,
+    all_attrs: bool=False
 ) -> str:
 ```
+<!-- [[[end]]] -->
+
 Here's an example:
 ```python
 from strip_tags import strip_tags
 
 html = """
 <div>
 <h1>This has tags</h1>
@@ -129,14 +161,53 @@
 Output:
 ```
 <h1>This has tags</h1>
 
 And whitespace too
 ```
 
+## strip-tags --help
+
+<!-- [[[cog
+import cog
+from strip_tags import cli
+from click.testing import CliRunner
+runner = CliRunner()
+result = runner.invoke(cli.cli, ["--help"])
+help = result.output.replace("Usage: cli", "Usage: strip-tags")
+cog.out(
+    "```\n{}\n```".format(help)
+)
+]]] -->
+```
+Usage: strip-tags [OPTIONS] [SELECTORS]...
+
+  Strip tags from HTML, optionally from areas identified by CSS selectors
+
+  Example usage:
+
+      cat input.html | strip-tags > output.txt
+
+  To run against just specific areas identified by CSS selectors:
+
+      cat input.html | strip-tags .entry .footer > output.txt
+
+Options:
+  --version             Show the version and exit.
+  -r, --remove TEXT     Remove content in these selectors
+  -i, --input FILENAME  Input file
+  -m, --minify          Minify whitespace
+  -t, --keep-tag TEXT   Keep these <tags>
+  --all-attrs           Include all attributes on kept tags
+  --first               First element matching the selectors
+  --help                Show this message and exit.
+
+```
+<!-- [[[end]]] -->
+
 ## Development
 
 To contribute to this tool, first checkout the code. Then create a new virtual environment:
 ```bash
 cd strip-tags
 python -m venv venv
 source venv/bin/activate
```

