# Comparing `tmp/parse_stages-0.1.4.tar.gz` & `tmp/parse_stages-0.1.5.tar.gz`

## Comparing `parse_stages-0.1.4.tar` & `parse_stages-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 parse_stages-0.1.4/.editorconfig
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 parse_stages-0.1.4/.readthedocs.yaml
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 parse_stages-0.1.4/mkdocs.yml
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 parse_stages-0.1.4/setup.cfg
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 parse_stages-0.1.4/tox.ini
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 parse_stages-0.1.4/LICENSES/BSD-2-Clause.txt
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 parse_stages-0.1.4/config/ruff-all/pyproject.toml
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 parse_stages-0.1.4/config/ruff-base/pyproject.toml
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 parse_stages-0.1.4/config/ruff-most/pyproject.toml
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 parse_stages-0.1.4/docs/api.md
--rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 parse_stages-0.1.4/docs/changes.md
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 parse_stages-0.1.4/docs/index.md
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 parse_stages-0.1.4/docs/language.md
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 parse_stages-0.1.4/nix/mkdocs.nix
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 parse_stages-0.1.4/nix/python-pytest.nix
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 parse_stages-0.1.4/nix/reformat.sh
--rwxr-xr-x   0        0        0      735 2020-02-02 00:00:00.000000 parse_stages-0.1.4/nix/run-pytest.sh
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 parse_stages-0.1.4/requirements/docs.txt
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 parse_stages-0.1.4/requirements/install.txt
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 parse_stages-0.1.4/requirements/test.txt
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 parse_stages-0.1.4/src/parse_stages/__init__.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 parse_stages-0.1.4/src/parse_stages/defs.py
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 parse_stages-0.1.4/src/parse_stages/expr.py
--rw-r--r--   0        0        0     5239 2020-02-02 00:00:00.000000 parse_stages-0.1.4/src/parse_stages/p_pyp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parse_stages-0.1.4/src/parse_stages/py.typed
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 parse_stages-0.1.4/unit_tests/__init__.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 parse_stages-0.1.4/unit_tests/test_eval.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 parse_stages-0.1.4/unit_tests/test_parse.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 parse_stages-0.1.4/.gitignore
--rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 parse_stages-0.1.4/README.md
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 parse_stages-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 parse_stages-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 parse_stages-0.1.5/.editorconfig
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 parse_stages-0.1.5/.readthedocs.yaml
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 parse_stages-0.1.5/mkdocs.yml
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 parse_stages-0.1.5/tox.ini
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 parse_stages-0.1.5/LICENSES/BSD-2-Clause.txt
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 parse_stages-0.1.5/config/ruff-all/pyproject.toml
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 parse_stages-0.1.5/config/ruff-base/pyproject.toml
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 parse_stages-0.1.5/config/ruff-most/pyproject.toml
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 parse_stages-0.1.5/docs/api.md
+-rw-r--r--   0        0        0     7470 2020-02-02 00:00:00.000000 parse_stages-0.1.5/docs/changes.md
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 parse_stages-0.1.5/docs/index.md
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 parse_stages-0.1.5/docs/language.md
+-rwxr-xr-x   0        0        0      495 2020-02-02 00:00:00.000000 parse_stages-0.1.5/nix/cleanpy.sh
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 parse_stages-0.1.5/nix/mkdocs.nix
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 parse_stages-0.1.5/nix/python-pytest.nix
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 parse_stages-0.1.5/nix/python-tox.nix
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 parse_stages-0.1.5/nix/reformat.sh
+-rwxr-xr-x   0        0        0      436 2020-02-02 00:00:00.000000 parse_stages-0.1.5/nix/run-pytest.sh
+-rwxr-xr-x   0        0        0      433 2020-02-02 00:00:00.000000 parse_stages-0.1.5/nix/run-tox.sh
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 parse_stages-0.1.5/requirements/docs.txt
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 parse_stages-0.1.5/requirements/install.txt
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 parse_stages-0.1.5/requirements/test.txt
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 parse_stages-0.1.5/src/parse_stages/__init__.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 parse_stages-0.1.5/src/parse_stages/defs.py
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 parse_stages-0.1.5/src/parse_stages/expr.py
+-rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 parse_stages-0.1.5/src/parse_stages/p_pyp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parse_stages-0.1.5/src/parse_stages/py.typed
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 parse_stages-0.1.5/unit_tests/__init__.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 parse_stages-0.1.5/unit_tests/test_eval.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 parse_stages-0.1.5/unit_tests/test_parse.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 parse_stages-0.1.5/.gitignore
+-rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 parse_stages-0.1.5/README.md
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 parse_stages-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 parse_stages-0.1.5/PKG-INFO
```

### Comparing `parse_stages-0.1.4/.editorconfig` & `parse_stages-0.1.5/.editorconfig`

 * *Files identical despite different names*

### Comparing `parse_stages-0.1.4/mkdocs.yml` & `parse_stages-0.1.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `parse_stages-0.1.4/LICENSES/BSD-2-Clause.txt` & `parse_stages-0.1.5/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `parse_stages-0.1.4/config/ruff-base/pyproject.toml` & `parse_stages-0.1.5/config/ruff-base/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 target-version = "py38"
 line-length = 100
 select = []
 ignore = [
   # We know what "self" is... I hope
   "ANN101",
 
+  # We leave most of the formatting to the `black` tool
+  "COM812",
+
   # No blank lines before the class docstring, TYVM
   "D203",
 
   # The multi-line docstring summary starts on the same line
   "D213",
 
   # The Tagged and TaggedFrozen classes need to be typedload-compatible
@@ -20,7 +23,11 @@
 ]
 
 [tool.ruff.isort]
 force-single-line = true
 known-first-party = ["parse_stages"]
 lines-after-imports = 2
 single-line-exclusions = ["typing"]
+
+[tool.ruff.per-file-ignores]
+# This is a test suite
+"unit_tests/**.py" = ["S101"]
```

### Comparing `parse_stages-0.1.4/config/ruff-most/pyproject.toml` & `parse_stages-0.1.5/config/ruff-most/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,64 @@
 # SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
 # SPDX-License-Identifier: BSD-2-Clause
 
 [tool.ruff]
 extend = "../ruff-base/pyproject.toml"
-# These are all the Ruff 0.0.265 linters.
+# These are all the Ruff 0.0.275 linters.
 select = [
   "A",
+  "AIR",
   "ANN",
   "ARG",
+  "ASYNC",
   "B",
   "BLE",
   "C4",
   "C90",
   "COM",
+  "CPY",
   "D",
   "DJ",
   "DTZ",
   "E",
   "EM",
   "ERA",
   "EXE",
   "F",
+  "FA",
   "FBT",
+  "FIX",
   "FLY",
   "G",
   "I",
   "ICN",
   "INP",
   "INT",
   "ISC",
   "N",
   "NPY",
   "PD",
+  "PERF",
   "PGH",
   "PIE",
   "PL",
   "PT",
   "PTH",
   "PYI",
   "Q",
   "RET",
   "RSE",
   "RUF",
   "S",
   "SIM",
   "SLF",
+  "SLOT",
   "T10",
   "T20",
   "TCH",
+  "TD",
   "TID",
   "TRY",
   "UP",
   "W",
   "YTT",
 ]
```

### Comparing `parse_stages-0.1.4/docs/api.md` & `parse_stages-0.1.5/docs/api.md`

 * *Files identical despite different names*

### Comparing `parse_stages-0.1.4/docs/changes.md` & `parse_stages-0.1.5/docs/changes.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,19 +3,66 @@
 SPDX-License-Identifier: BSD-2-Clause
 -->
 
 # Changelog
 
 All notable changes to the parse-stages project will be documented in this file.
 
-The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
+The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.5] - 2023-06-27
+
+### Fixes
+
+- Build infrastructure:
+    - relax the `hatch-requirements-txt` to >= 0.3, which is the version in
+      Debian testing/unstable
+    - specify a lower requirement for `hatchling` as >= 1.8, which is
+      the version in Ubuntu 22.10 (kinetic)
+    - specify an upper requirement for `hatchling`
+- Main source:
+    - do not disable all Flake8 / Ruff checks for three files!
+    - fix some formatting nits in the newly-checked source files
+- Test suite:
+    - drop the `pyupgrade` environment from Tox's default envlist;
+      there is (by design) no way to run it in a no-op, report-only mode
+    - do not pass the `python_version` option to `mypy`, let it check
+      the code with regard to the currently-running Python interpreter
+
+### Additions
+
+- Build infrastructure:
+    - specify the project license
+    - add some more PyPI trove classifiers
+- Test suite:
+    - introduce the `PY_MINVER_MIN` and `PY_MINVER_MAX` environment variables for
+      the `nix/run-pytest.sh` helper tool so that e.g. the current flakiness of
+      Python 3.12 in nixpkgs-unstable can be skipped
+    - add a Nix expression and the `nix/run-tox.sh` helper tool to run
+      all the Tox tests using a different Python version
+    - also include the `reuse` Tox environment in the ones run at the `@check`
+      stage using the `tox-stages` tool
+
+### Other changes
+
+- Main source:
+    - replace assertions in the parsing code with `if` statements that
+      raise our own exceptions
+- Documentation:
+    - refer to version 1.1.0 of the "Keep a Changelog" format specification
+    - use `mkdocstrings` 0.22, no changes
+- Test suite:
+    - drop the `flake8` / `pep8`, `pylint`, and `pydocstyle`
+      Tox test environments, Ruff handles most of these checks now
+    - use Ruff 0.0.275, activate all the new check areas, just in case
+    - use mypy 1.x, no changes
+
 ## [0.1.4] - 2023-05-13
 
 ### Additions
 
 - Documentation:
     - add a [ReadTheDocs mirror](https://parse-stages.readthedocs.io/)
 - Main source:
@@ -136,13 +183,14 @@
 
 ## [0.1.0] - 2023-01-25
 
 ### Started
 
 - First public release.
 
-[Unreleased]: https://gitlab.com/ppentchev/parse-stages/-/compare/release%2F0.1.4...main
+[Unreleased]: https://gitlab.com/ppentchev/parse-stages/-/compare/release%2F0.1.5...main
+[0.1.5]: https://gitlab.com/ppentchev/parse-stages/-/compare/release%2F0.1.4...release%2F0.1.5
 [0.1.4]: https://gitlab.com/ppentchev/parse-stages/-/compare/release%2F0.1.3...release%2F0.1.4
 [0.1.3]: https://gitlab.com/ppentchev/parse-stages/-/compare/release%2F0.1.2...release%2F0.1.3
 [0.1.2]: https://gitlab.com/ppentchev/parse-stages/-/compare/release%2F0.1.1...release%2F0.1.2
 [0.1.1]: https://gitlab.com/ppentchev/parse-stages/-/compare/release%2F0.1.0...release%2F0.1.1
 [0.1.0]: https://gitlab.com/ppentchev/parse-stages/-/tags/release%2F0.1.0
```

### Comparing `parse_stages-0.1.4/docs/index.md` & `parse_stages-0.1.5/docs/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 [nox]: https://nox.thea.codes/en/stable/ "The nox flexible automation tool"
 
 ## Installation
 
 A program that uses the `parse-stages` library should specify it in
 its list of requirements, e.g. using [PEP508][pep508] syntax:
 
-    parse-stages >= 0.1.4, < 0.2
+    parse-stages >= 0.1.5, < 0.2
 
 [pep508]: https://peps.python.org/pep-0508/ "PEP 508 – Dependency specification for Python Software Packages"
 
 ## Parsing a stage specification
 
 The `parse_spec()` function parses a string specification into
 a [BoolExpr][parse_stages.BoolExpr] object that may later be used to
```

### Comparing `parse_stages-0.1.4/docs/language.md` & `parse_stages-0.1.5/docs/language.md`

 * *Files identical despite different names*

### Comparing `parse_stages-0.1.4/nix/mkdocs.nix` & `parse_stages-0.1.5/nix/mkdocs.nix`

 * *Files identical despite different names*

### Comparing `parse_stages-0.1.4/src/parse_stages/__init__.py` & `parse_stages-0.1.5/src/parse_stages/__init__.py`

 * *Files identical despite different names*

### Comparing `parse_stages-0.1.4/src/parse_stages/expr.py` & `parse_stages-0.1.5/src/parse_stages/expr.py`

 * *Files identical despite different names*

### Comparing `parse_stages-0.1.4/src/parse_stages/p_pyp.py` & `parse_stages-0.1.5/src/parse_stages/p_pyp.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,54 @@
 # SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
 # SPDX-License-Identifier: BSD-2-Clause
 """Parse an expression using the `pyparsing` library."""
 
-# Let's make sure that the parsed tokens are exactly as we expect them to be
-# flake8: noqa: S101
-
 from __future__ import annotations
 
+import dataclasses
+import typing
+
 import pyparsing as pyp
 
 from . import expr
 
 
+if typing.TYPE_CHECKING:
+    from typing import Any
+
+
+@dataclasses.dataclass
+class Error(Exception):
+    """A base class for parse-related errors."""
+
+
+@dataclasses.dataclass
+class ParseResultError(Error):
+    """The pyparsing module returned an unexpected series of tokens."""
+
+    tokens: pyp.ParseResults
+    """The unexpected sequence of tokens."""
+
+    def __str__(self) -> str:
+        """Provide a human-readable representation of the error."""
+        return f"Unexpected sequence of parse tokens: {self.tokens!r}"
+
+
+@dataclasses.dataclass
+class ParseError(Error):
+    """Our pyparsing handlers returned an unexpected object."""
+
+    res: Any
+    """The unexpected object returned."""
+
+    def __str__(self) -> str:
+        """Provide a human-readable representation of the error."""
+        return f"Unexpected parsed object: {self.res!r}"
+
+
 EMPTY_SET_SPECS = ["", "0", "none"]
 """The list of exact strings that `parse_stage_ids()` will return an empty list for."""
 
 
 _p_ws = pyp.White()[...]
 
 _p_tag = pyp.Char("@").suppress() + pyp.Word(pyp.alphanums + "_-")
@@ -37,101 +70,112 @@
 
 _p_spec = _p_ws.suppress() + _p_or_expr
 
 
 @_p_tag.set_parse_action
 def _parse_tag(tokens: pyp.ParseResults) -> expr.TagExpr:
     """Parse a tag name."""
-    assert len(tokens) == 1 and isinstance(tokens[0], str), repr(tokens)
+    if len(tokens) != 1 or not isinstance(tokens[0], str):
+        raise ParseResultError(tokens)
     return expr.TagExpr(tag=tokens[0])
 
 
 @_p_keyword.set_parse_action
 def _parse_keyword(tokens: pyp.ParseResults) -> expr.KeywordExpr:
     """Parse a keyword."""
-    assert len(tokens) == 1 and isinstance(tokens[0], str), repr(tokens)
+    if len(tokens) != 1 or not isinstance(tokens[0], str):
+        raise ParseResultError(tokens)
     return expr.KeywordExpr(keyword=tokens[0])
 
 
 @_p_atom.set_parse_action
 def _parse_atom(tokens: pyp.ParseResults) -> expr.BoolExpr:
     """Parse an atom (a tag or a keyword)."""
-    assert len(tokens) == 1 and isinstance(tokens[0], (expr.TagExpr, expr.KeywordExpr))
+    if len(tokens) != 1 or not isinstance(tokens[0], (expr.TagExpr, expr.KeywordExpr)):
+        raise ParseResultError(tokens)
     return tokens[0]
 
 
 @_p_not_atom.set_parse_action  # type: ignore[misc]
 def _parse_not_atom(tokens: pyp.ParseResults) -> expr.NotExpr:
     """Parse a "not @tag" or "not keyword" element."""
-    assert len(tokens) == 1 and isinstance(tokens[0], expr.BoolExpr)
+    if len(tokens) != 1 or not isinstance(tokens[0], expr.BoolExpr):
+        raise ParseResultError(tokens)
     return expr.NotExpr(child=tokens[0])
 
 
 @_p_and_expr.set_parse_action  # type: ignore[misc]
 def _parse_and_expr(tokens: pyp.ParseResults) -> expr.BoolExpr:
     """Parse a "atom [and atom...]" subexpression."""
     children: list[expr.BoolExpr] = tokens.as_list()
-    assert children and all(isinstance(item, expr.BoolExpr) for item in children)
+    if not children or any(not isinstance(item, expr.BoolExpr) for item in children):
+        raise ParseResultError(tokens)
     if len(children) == 1:
         return children[0]
 
     return expr.AndExpr(children=children)
 
 
 @_p_or_expr.set_parse_action  # type: ignore[misc]
 def _parse_or_expr(tokens: pyp.ParseResults) -> expr.BoolExpr:
     """Parse a "subexpr [or subexpr...]" subexpression."""
     children: list[expr.BoolExpr] = tokens.as_list()
-    assert children and all(isinstance(item, expr.BoolExpr) for item in children)
+    if not children or any(not isinstance(item, expr.BoolExpr) for item in children):
+        raise ParseResultError(tokens)
     if len(children) == 1:
         return children[0]
 
     return expr.OrExpr(children=children)
 
 
 _p_complete = _p_spec.leave_whitespace()
 
 
 def parse_spec(spec: str) -> expr.BoolExpr:
     """Parse an expression using the `pyparsing` library."""
     res = _p_complete.parse_string(spec, parse_all=True).as_list()
-    assert len(res) == 1 and isinstance(res[0], expr.BoolExpr), repr(res)
+    if len(res) != 1 or not isinstance(res[0], expr.BoolExpr):
+        raise ParseError(res)
     return res[0]
 
 
 _p_stage_id = pyp.Word(pyp.srange("[1-9]"), pyp.srange("[0-9]"))
 
 _p_stage_range = _p_stage_id + pyp.Opt(pyp.Literal("-").suppress() + _p_stage_id)
 
 _p_stage_ids = _p_stage_range + (pyp.Literal(",").suppress() + _p_stage_range)[...]
 
 
 @_p_stage_id.set_parse_action
 def _parse_stage_id(tokens: pyp.ParseResults) -> int:
     """Parse a single stage ID, return it as a zero-based index."""
-    assert len(tokens) == 1 and isinstance(tokens[0], str), repr(tokens)
+    if len(tokens) != 1 or not isinstance(tokens[0], str):
+        raise ParseResultError(tokens)
     res = int(tokens[0]) - 1
-    assert res >= 0, repr((tokens, res))
+    if res < 0:
+        raise ParseResultError(tokens)
     return res
 
 
 @_p_stage_range.set_parse_action
 def _parse_stage_range(tokens: pyp.ParseResults) -> list[int]:
     """Parse a range of stage IDs (possibly only containing a single one)."""
     if len(tokens) == 1:
-        assert isinstance(tokens[0], int), repr(tokens)
+        if not isinstance(tokens[0], int):
+            raise ParseResultError(tokens)
         return [tokens[0]]
 
     # The magic value will go away once we can use Python 3.10 structural matching
-    assert (
-        len(tokens) == 2  # pylint: disable=magic-value-comparison
-        and isinstance(tokens[0], int)
-        and isinstance(tokens[1], int)
-        and tokens[0] < tokens[1]
-    ), repr(tokens)
+    if (
+        len(tokens) != 2  # noqa: PLR2004
+        or not isinstance(tokens[0], int)
+        or not isinstance(tokens[1], int)
+        or tokens[0] >= tokens[1]
+    ):
+        raise ParseResultError(tokens)
     return list(range(tokens[0], tokens[1] + 1))
 
 
 _p_stage_ids_complete = _p_stage_ids.leave_whitespace()
 
 
 def parse_stage_ids(spec: str, *, empty_set_specs: list[str] | None = None) -> list[int]:
@@ -146,9 +190,10 @@
     """
     if empty_set_specs is None:
         empty_set_specs = EMPTY_SET_SPECS
     if spec in empty_set_specs:
         return []
 
     res: list[int] = _p_stage_ids_complete.parse_string(spec, parse_all=True).as_list()
-    assert all(isinstance(item, int) and item >= 0 for item in res), repr(res)
+    if any(not isinstance(item, int) and item >= 0 for item in res):
+        raise ParseError(res)
     return res
```

### Comparing `parse_stages-0.1.4/unit_tests/test_eval.py` & `parse_stages-0.1.5/unit_tests/test_eval.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 # SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
 # SPDX-License-Identifier: BSD-2-Clause
 """Test the evaluation of some simple expressions."""
 
-# This is a test suite, right?
-# flake8: noqa: S101
-
 from __future__ import annotations
 
 import dataclasses
-
 from typing import NamedTuple
 
 import pytest
 
 import parse_stages as pst
```

### Comparing `parse_stages-0.1.4/unit_tests/test_parse.py` & `parse_stages-0.1.5/unit_tests/test_parse.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 # SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
 # SPDX-License-Identifier: BSD-2-Clause
 """Test some basic parsing functionality."""
 
-# This is a test suite, right?
-# flake8: noqa: S101
-
 from __future__ import annotations
 
 from typing import NamedTuple
 
 import pytest
 
 import parse_stages as pst
```

### Comparing `parse_stages-0.1.4/README.md` & `parse_stages-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `parse_stages-0.1.4/PKG-INFO` & `parse_stages-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,36 @@
 Metadata-Version: 2.1
 Name: parse_stages
-Version: 0.1.4
+Version: 0.1.5
 Summary: Parse an expression for selecting stages and tags
 Project-URL: Homepage, https://devel.ringlet.net/devel/parse-stages/
 Project-URL: Changes, https://devel.ringlet.net/devel/parse-stages/changes/
 Project-URL: Issue Tracker, https://gitlab.com/ppentchev/parse-stages/-/issues
 Project-URL: Source Code, https://gitlab.com/ppentchev/parse-stages
 Author-email: Peter Pentchev <roam@ringlet.net>
+License: BSD-2-Clause
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: DFSG approved
+Classifier: License :: Freely Distributable
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Testing :: Unit
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: pyparsing<4,>=3
 Description-Content-Type: text/markdown
 
 <!--
 SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
 SPDX-License-Identifier: BSD-2-Clause
```

