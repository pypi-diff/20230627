# Comparing `tmp/markdown_it_pyrs-0.1.0.tar.gz` & `tmp/markdown_it_pyrs-0.2.0.tar.gz`

## Comparing `markdown_it_pyrs-0.1.0.tar` & `markdown_it_pyrs-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0      455 1970-01-01 00:00:00.000000 markdown_it_pyrs-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123      722 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/.github/dependabot.yml
--rw-r--r--   0     1001      123     6016 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      696 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/.gitignore
--rw-r--r--   0     1001      123     1001 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0     1001      123    11357 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/LICENSE
--rw-r--r--   0     1001      123      554 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/NOTICE
--rw-r--r--   0     1001      123     9327 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/README.md
--rw-r--r--   0     1001      123     1452 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123      208 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/python/markdown_it_pyrs/__init__.py
--rw-r--r--   0     1001      123     2365 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/python/markdown_it_pyrs/cli.py
--rw-r--r--   0     1001      123     3594 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/python/markdown_it_pyrs/markdown_it_pyrs.pyi
--rw-r--r--   0     1001      123        0 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/python/markdown_it_pyrs/py.typed
--rw-r--r--   0     1001      123     8534 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123    16310 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/src/nodes.rs
--rw-r--r--   0     1001      123      693 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tests/bench_html.py
--rw-r--r--   0     1001      123      838 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tests/bench_tree.py
--rw-r--r--   0     1001      123     3412 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tests/fixtures/ast.md
--rw-r--r--   0     1001      123     8424 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tests/fixtures/commonmark_extras.md
--rw-r--r--   0     1001      123   150858 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tests/fixtures/commonmark_spec.json
--rw-r--r--   0     1001      123     8323 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tests/fixtures/footnote.md
--rw-r--r--   0     1001      123      791 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tests/fixtures/front_matter.md
--rw-r--r--   0     1001      123     3909 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tests/fixtures/linkify.md
--rw-r--r--   0     1001      123      817 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tests/fixtures/normalize.md
--rw-r--r--   0     1001      123     2639 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tests/fixtures/smartquotes.md
--rw-r--r--   0     1001      123      512 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tests/fixtures/sourcepos.md
--rw-r--r--   0     1001      123   202694 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tests/fixtures/spec.md
--rw-r--r--   0     1001      123     1562 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tests/fixtures/strikethrough.md
--rw-r--r--   0     1001      123    10687 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tests/fixtures/tables.md
--rw-r--r--   0     1001      123     3648 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tests/fixtures/tasklists.md
--rw-r--r--   0     1001      123     1108 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tests/fixtures/typographer.md
--rw-r--r--   0     1001      123     1988 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tests/test_api.py
--rw-r--r--   0     1001      123     2452 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tests/test_cli.py
--rw-r--r--   0     1001      123     3913 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tests/test_fixtures.py
--rw-r--r--   0     1001      123      701 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/tox.ini
--rw-r--r--   0     1001      123    24729 2023-06-22 17:42:36.000000 markdown_it_pyrs-0.1.0/Cargo.lock
--rw-r--r--   0        0        0    10528 1970-01-01 00:00:00.000000 markdown_it_pyrs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 markdown_it_pyrs-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123      722 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/.github/dependabot.yml
+-rw-r--r--   0     1001      123     6016 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      696 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/.gitignore
+-rw-r--r--   0     1001      123     1001 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123    11357 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/LICENSE
+-rw-r--r--   0     1001      123      554 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/NOTICE
+-rw-r--r--   0     1001      123     9563 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/README.md
+-rw-r--r--   0     1001      123     1452 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123      208 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/python/markdown_it_pyrs/__init__.py
+-rw-r--r--   0     1001      123     2365 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/python/markdown_it_pyrs/cli.py
+-rw-r--r--   0     1001      123     3614 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/python/markdown_it_pyrs/markdown_it_pyrs.pyi
+-rw-r--r--   0     1001      123        0 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/python/markdown_it_pyrs/py.typed
+-rw-r--r--   0     1001      123     8653 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123    16310 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/src/nodes.rs
+-rw-r--r--   0     1001      123      693 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/bench_html.py
+-rw-r--r--   0     1001      123      838 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/bench_tree.py
+-rw-r--r--   0     1001      123     3412 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/fixtures/ast.md
+-rw-r--r--   0     1001      123     6483 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/fixtures/autolink_ext.md
+-rw-r--r--   0     1001      123     8424 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/fixtures/commonmark_extras.md
+-rw-r--r--   0     1001      123   150858 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/fixtures/commonmark_spec.json
+-rw-r--r--   0     1001      123     8323 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/fixtures/footnote.md
+-rw-r--r--   0     1001      123      791 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/fixtures/front_matter.md
+-rw-r--r--   0     1001      123     3909 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/fixtures/linkify.md
+-rw-r--r--   0     1001      123      817 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/fixtures/normalize.md
+-rw-r--r--   0     1001      123     2639 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/fixtures/smartquotes.md
+-rw-r--r--   0     1001      123      512 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/fixtures/sourcepos.md
+-rw-r--r--   0     1001      123   202694 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/fixtures/spec.md
+-rw-r--r--   0     1001      123     1562 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/fixtures/strikethrough.md
+-rw-r--r--   0     1001      123    10687 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/fixtures/tables.md
+-rw-r--r--   0     1001      123     3648 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/fixtures/tasklists.md
+-rw-r--r--   0     1001      123     1108 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/fixtures/typographer.md
+-rw-r--r--   0     1001      123     1988 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/test_api.py
+-rw-r--r--   0     1001      123     2452 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/test_cli.py
+-rw-r--r--   0     1001      123     4146 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tests/test_fixtures.py
+-rw-r--r--   0     1001      123      701 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/tox.ini
+-rw-r--r--   0     1001      123    25466 2023-06-27 08:54:32.000000 markdown_it_pyrs-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0    10764 1970-01-01 00:00:00.000000 markdown_it_pyrs-0.2.0/PKG-INFO
```

### Comparing `markdown_it_pyrs-0.1.0/.github/dependabot.yml` & `markdown_it_pyrs-0.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/.github/workflows/CI.yml` & `markdown_it_pyrs-0.2.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/.gitignore` & `markdown_it_pyrs-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/.pre-commit-config.yaml` & `markdown_it_pyrs-0.2.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -27,20 +27,20 @@
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
     - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.272
+    rev: v0.0.275
     hooks:
     - id: ruff
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.3.0
+    rev: v1.4.1
     hooks:
     - id: mypy
       files: >
         (?x)^(
           .*\.pyi|
           tests/test_api\.py
         )$
```

### Comparing `markdown_it_pyrs-0.1.0/LICENSE` & `markdown_it_pyrs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/NOTICE` & `markdown_it_pyrs-0.2.0/NOTICE`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/README.md` & `markdown_it_pyrs-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # markdown-it-pyrs
 
+[![PyPI][pypi-badge]][pypi-link]
+
+[pypi-badge]: https://img.shields.io/pypi/v/markdown-it-pyrs.svg
+[pypi-link]: https://pypi.org/project/markdown-it-pyrs
+
 **Currently in Beta, feedback welcome!**
 
 A Python interface for [markdown-it.rs](https://github.com/rlidwka/markdown-it.rs) (and [plugins](https://github.com/chrisjsewell/markdown-it-plugins.rs)), using Rust for blazingly fast Markdown parsing ⚡️
 
 The goal of this project is to provide a fast, safe, extensible, and easy-to-use Markdown parser for Python.
 It is complimentary to [markdown-it-py](https://github.com/ExecutableBookProject/markdown-it-py), which is a pure Python implementation of markdown-it, and here we aim to follow as close as possible the API for that package.
 
@@ -138,26 +143,27 @@
 - `table`:
 
   ```markdown
   | foo | bar |
   | --- | --- |
   | baz | bim |
   ```
-- `linkify`: Automatically linkify URLs
 - `strikethrough`: `~~strikethrough~~`
 - `tasklist`: `- [x] tasklist item`
+- `autolink_ext`: Extended autolink detection with "bare URLs" like `https://example.com` and `www.example.com`
 
 Others:
 
 - `sourcepos`: Add source mapping to rendered HTML, looks like this: `<stuff data-sourcepos="1:1-2:3">`, i.e. `line:col-line:col`
 - `replacements`: Typographic replacements, like `--` to `—`
 - `smartquotes`: Smart quotes, like `"` to `“`
 - `front_matter`: YAML front matter
 - `footnote`: Pandoc-style footnotes (see <https://pandoc.org/MANUAL.html#footnotes>)
 - `heading_anchors`: Add heading anchors, with defaults like GitHub
+- `linkify`: Automatically linkify URLs with <https://crates.io/crates/linkify> (note currently this only matches URLs with a scheme, e.g. `https://example.com`)
 
 ## Development
 
 I'm quite new to Rust, so if you see something that could be improved, issues and PRs are welcome!
 
 [PyO3](https://pyo3.rs) and [Maturin](https://www.maturin.rs) are used to build the Python package, by wrapping [markdown-it.rs](https://github.com/rlidwka/markdown-it.rs) in a Python module.
 
@@ -176,15 +182,14 @@
 
 - Allow options for plugins:
   - heading anchors
   - tasklist checkboxes to be disabled
   - footnotes with options to turn on/off inline/collect/backrefs
 
 - The `gfm` (Github Flavoured Markdown) initialisation mode needs improving
-  - `linkify` is not strictly equivalent to <https://github.github.com/gfm/#autolinks-extension->, e.g. it does not currently autolink `www.example.com`
   - Add <https://github.github.com/gfm/#disallowed-raw-html-extension->
   - heading anchors, is not strictly in the spec, but should be noted
   - Add more testing
 
 Open issue upstream:
 
 - no `text_join` rule (to join adjacent `text` and `text_special` tokens)
```

### Comparing `markdown_it_pyrs-0.1.0/pyproject.toml` & `markdown_it_pyrs-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/python/markdown_it_pyrs/cli.py` & `markdown_it_pyrs-0.2.0/python/markdown_it_pyrs/cli.py`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/python/markdown_it_pyrs/markdown_it_pyrs.pyi` & `markdown_it_pyrs-0.2.0/python/markdown_it_pyrs/markdown_it_pyrs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
     "sourcepos",
     "strikethrough",
     "table",
     "front_matter",
     "tasklist",
     "footnote",
     "heading_anchors",
+    "autolink_ext",
 ]
 
 class MarkdownIt:
     """Markdown parser class."""
 
     def __init__(
         self, config: Literal["commonmark", "gfm", "zero"] = "commonmark"
```

### Comparing `markdown_it_pyrs-0.1.0/src/lib.rs` & `markdown_it_pyrs-0.2.0/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,17 @@
             }
             "footnote" => {
                 markdown_it_footnote::add(&mut self.parser);
             }
             "heading_anchors" => {
                 markdown_it_heading_anchors::add(&mut self.parser);
             }
+            "autolink_ext" => {
+                markdown_it_autolink::add(&mut self.parser);
+            }
             _ => {
                 return {
                     Err(pyo3::exceptions::PyValueError::new_err(format!(
                         "Unknown plugin: {}",
                         name
                     )))
                 }
@@ -129,15 +132,15 @@
             }
             "gfm" => {
                 let mut parser = markdown_it::MarkdownIt::new();
                 markdown_it::plugins::cmark::add(&mut parser);
                 markdown_it::plugins::html::add(&mut parser);
                 markdown_it::plugins::extra::tables::add(&mut parser);
                 markdown_it::plugins::extra::strikethrough::add(&mut parser);
-                markdown_it::plugins::extra::linkify::add(&mut parser);
+                markdown_it_autolink::add(&mut parser);
                 markdown_it_tasklist::add(&mut parser);
                 Ok(Self {
                     parser,
                     xhtml_out: true,
                 })
             }
             "zero" => Ok(Self {
@@ -184,14 +187,15 @@
             "sourcepos",
             "strikethrough",
             "table",
             "front_matter",
             "tasklist",
             "footnote",
             "heading_anchors",
+            "autolink_ext",
         ]
         .iter()
         .map(|s| s.to_string())
         .collect()
     }
 
     /// Enable a plugin
```

### Comparing `markdown_it_pyrs-0.1.0/src/nodes.rs` & `markdown_it_pyrs-0.2.0/src/nodes.rs`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/tests/bench_html.py` & `markdown_it_pyrs-0.2.0/tests/bench_html.py`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/tests/bench_tree.py` & `markdown_it_pyrs-0.2.0/tests/bench_tree.py`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/tests/fixtures/ast.md` & `markdown_it_pyrs-0.2.0/tests/fixtures/ast.md`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/tests/fixtures/commonmark_extras.md` & `markdown_it_pyrs-0.2.0/tests/fixtures/commonmark_extras.md`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/tests/fixtures/commonmark_spec.json` & `markdown_it_pyrs-0.2.0/tests/fixtures/commonmark_spec.json`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/tests/fixtures/footnote.md` & `markdown_it_pyrs-0.2.0/tests/fixtures/footnote.md`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/tests/fixtures/front_matter.md` & `markdown_it_pyrs-0.2.0/tests/fixtures/front_matter.md`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/tests/fixtures/linkify.md` & `markdown_it_pyrs-0.2.0/tests/fixtures/linkify.md`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/tests/fixtures/normalize.md` & `markdown_it_pyrs-0.2.0/tests/fixtures/normalize.md`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/tests/fixtures/smartquotes.md` & `markdown_it_pyrs-0.2.0/tests/fixtures/smartquotes.md`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/tests/fixtures/sourcepos.md` & `markdown_it_pyrs-0.2.0/tests/fixtures/sourcepos.md`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/tests/fixtures/spec.md` & `markdown_it_pyrs-0.2.0/tests/fixtures/spec.md`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/tests/fixtures/strikethrough.md` & `markdown_it_pyrs-0.2.0/tests/fixtures/strikethrough.md`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/tests/fixtures/tables.md` & `markdown_it_pyrs-0.2.0/tests/fixtures/tables.md`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/tests/fixtures/tasklists.md` & `markdown_it_pyrs-0.2.0/tests/fixtures/tasklists.md`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/tests/fixtures/typographer.md` & `markdown_it_pyrs-0.2.0/tests/fixtures/typographer.md`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/tests/test_api.py` & `markdown_it_pyrs-0.2.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/tests/test_cli.py` & `markdown_it_pyrs-0.2.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/tests/test_fixtures.py` & `markdown_it_pyrs-0.2.0/tests/test_fixtures.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,14 +94,20 @@
 
 @pytest.mark.param_file(FIXTURE_PATH.joinpath("footnote.md"))
 def test_footnote(file_params):
     md = MarkdownIt().enable("footnote")
     assert file_params.assert_expected(md.render(file_params.content), rstrip=True)
 
 
+@pytest.mark.param_file(FIXTURE_PATH.joinpath("autolink_ext.md"))
+def test_autolink_ext(file_params):
+    md = MarkdownIt().enable("autolink_ext")
+    assert file_params.assert_expected(md.render(file_params.content), rstrip=True)
+
+
 @pytest.mark.param_file(FIXTURE_PATH.joinpath("ast.md"))
 def test_ast(file_params):
     md = MarkdownIt().enable_many(
         [
             "front_matter",
             "strikethrough",
             "table",
```

### Comparing `markdown_it_pyrs-0.1.0/tox.ini` & `markdown_it_pyrs-0.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `markdown_it_pyrs-0.1.0/Cargo.lock` & `markdown_it_pyrs-0.2.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,24 @@
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
+name = "gfm-autolinks"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e759407cedde28f2324a4ce9e1b309a5730b328985c2f5482d87fd3a75535d55"
+dependencies = [
+ "once_cell",
+ "unicode_categories",
+]
+
+[[package]]
 name = "github-slugger"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "721820f4eab1c427d482e144b63288754d9872fb7f0d72d73ab101008ef43147"
 dependencies = [
  "once_cell",
  "regex",
@@ -229,17 +239,17 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "itertools"
-version = "0.10.5"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
+checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
 version = "1.0.6"
@@ -312,14 +322,24 @@
  "regex",
  "stacker",
  "syntect",
  "unicode-general-category",
 ]
 
 [[package]]
+name = "markdown-it-autolink"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6ea23e65f2a1cd149861f2cb8c0a50c8f1f47f35d0b0706100f50e39e7c0bc52"
+dependencies = [
+ "gfm-autolinks",
+ "markdown-it",
+]
+
+[[package]]
 name = "markdown-it-footnote"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2070379510522a1b5d9d44dafacb0bfc983b4bb5e197882fe51c8852986e9dfd"
 dependencies = [
  "markdown-it",
 ]
@@ -353,18 +373,19 @@
  "once_cell",
  "regex",
  "stacker",
 ]
 
 [[package]]
 name = "markdown_it_pyrs"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "itertools",
  "markdown-it",
+ "markdown-it-autolink",
  "markdown-it-footnote",
  "markdown-it-front-matter",
  "markdown-it-heading-anchors",
  "markdown-it-tasklist",
  "pyo3",
  "stacker",
 ]
@@ -818,14 +839,20 @@
 [[package]]
 name = "unicode-xid"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
 
 [[package]]
+name = "unicode_categories"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "39ec24b3121d976906ece63c9daad25b85969647682eee313cb5779fdd69e14e"
+
+[[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "utf8-width"
```

### Comparing `markdown_it_pyrs-0.1.0/PKG-INFO` & `markdown_it_pyrs-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown_it_pyrs
-Version: 0.1.0
+Version: 0.2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
@@ -22,14 +22,19 @@
 Author-email: Chris Sewell <chrisj_sewell@hotmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Homepage, https://github.com/chrisjsewell/markdown-it-pyrs
 
 # markdown-it-pyrs
 
+[![PyPI][pypi-badge]][pypi-link]
+
+[pypi-badge]: https://img.shields.io/pypi/v/markdown-it-pyrs.svg
+[pypi-link]: https://pypi.org/project/markdown-it-pyrs
+
 **Currently in Beta, feedback welcome!**
 
 A Python interface for [markdown-it.rs](https://github.com/rlidwka/markdown-it.rs) (and [plugins](https://github.com/chrisjsewell/markdown-it-plugins.rs)), using Rust for blazingly fast Markdown parsing ⚡️
 
 The goal of this project is to provide a fast, safe, extensible, and easy-to-use Markdown parser for Python.
 It is complimentary to [markdown-it-py](https://github.com/ExecutableBookProject/markdown-it-py), which is a pure Python implementation of markdown-it, and here we aim to follow as close as possible the API for that package.
 
@@ -164,26 +169,27 @@
 - `table`:
 
   ```markdown
   | foo | bar |
   | --- | --- |
   | baz | bim |
   ```
-- `linkify`: Automatically linkify URLs
 - `strikethrough`: `~~strikethrough~~`
 - `tasklist`: `- [x] tasklist item`
+- `autolink_ext`: Extended autolink detection with "bare URLs" like `https://example.com` and `www.example.com`
 
 Others:
 
 - `sourcepos`: Add source mapping to rendered HTML, looks like this: `<stuff data-sourcepos="1:1-2:3">`, i.e. `line:col-line:col`
 - `replacements`: Typographic replacements, like `--` to `—`
 - `smartquotes`: Smart quotes, like `"` to `“`
 - `front_matter`: YAML front matter
 - `footnote`: Pandoc-style footnotes (see <https://pandoc.org/MANUAL.html#footnotes>)
 - `heading_anchors`: Add heading anchors, with defaults like GitHub
+- `linkify`: Automatically linkify URLs with <https://crates.io/crates/linkify> (note currently this only matches URLs with a scheme, e.g. `https://example.com`)
 
 ## Development
 
 I'm quite new to Rust, so if you see something that could be improved, issues and PRs are welcome!
 
 [PyO3](https://pyo3.rs) and [Maturin](https://www.maturin.rs) are used to build the Python package, by wrapping [markdown-it.rs](https://github.com/rlidwka/markdown-it.rs) in a Python module.
 
@@ -202,15 +208,14 @@
 
 - Allow options for plugins:
   - heading anchors
   - tasklist checkboxes to be disabled
   - footnotes with options to turn on/off inline/collect/backrefs
 
 - The `gfm` (Github Flavoured Markdown) initialisation mode needs improving
-  - `linkify` is not strictly equivalent to <https://github.github.com/gfm/#autolinks-extension->, e.g. it does not currently autolink `www.example.com`
   - Add <https://github.github.com/gfm/#disallowed-raw-html-extension->
   - heading anchors, is not strictly in the spec, but should be noted
   - Add more testing
 
 Open issue upstream:
 
 - no `text_join` rule (to join adjacent `text` and `text_special` tokens)
```

