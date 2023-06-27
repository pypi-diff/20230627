# Comparing `tmp/duty-0.9.0.tar.gz` & `tmp/duty-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duty-0.9.0.tar", last modified: Tue Mar  7 19:39:11 2023, max compression
+gzip compressed data, was "duty-1.0.0.tar", last modified: Tue Jun 27 21:46:18 2023, max compression
```

## Comparing `duty-0.9.0.tar` & `duty-1.0.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      754 2023-02-18 18:32:06.812496 duty-0.9.0/LICENSE
--rw-r--r--   0        0        0     1218 2023-02-18 18:32:07.099158 duty-0.9.0/README.md
--rw-r--r--   0        0        0     2338 2023-02-18 18:32:07.099158 duty-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      144 2023-02-18 18:32:07.099158 duty-0.9.0/src/duty/__init__.py
--rw-r--r--   0        0        0      333 2023-02-18 18:32:05.312520 duty-0.9.0/src/duty/__main__.py
--rw-r--r--   0        0        0     2285 2023-02-18 16:25:12.282914 duty-0.9.0/src/duty/callables/__init__.py
--rw-r--r--   0        0        0      367 2023-02-17 17:16:47.840819 duty-0.9.0/src/duty/callables/_io.py
--rw-r--r--   0        0        0     4699 2023-02-18 16:09:01.647898 duty-0.9.0/src/duty/callables/autoflake.py
--rw-r--r--   0        0        0     7148 2023-02-18 16:14:20.452821 duty-0.9.0/src/duty/callables/black.py
--rw-r--r--   0        0        0     3216 2023-03-07 19:38:39.771702 duty-0.9.0/src/duty/callables/blacken_docs.py
--rw-r--r--   0        0        0    23941 2023-02-18 16:19:55.114352 duty-0.9.0/src/duty/callables/coverage.py
--rw-r--r--   0        0        0     8608 2023-02-18 16:14:20.452821 duty-0.9.0/src/duty/callables/flake8.py
--rw-r--r--   0        0        0     5203 2023-03-03 14:18:24.951319 duty-0.9.0/src/duty/callables/interrogate.py
--rw-r--r--   0        0        0    26580 2023-02-18 16:14:20.456154 duty-0.9.0/src/duty/callables/isort.py
--rw-r--r--   0        0        0     7882 2023-02-18 16:14:20.456154 duty-0.9.0/src/duty/callables/mkdocs.py
--rw-r--r--   0        0        0    19925 2023-02-18 16:14:20.452821 duty-0.9.0/src/duty/callables/mypy.py
--rw-r--r--   0        0        0    18523 2023-02-18 16:14:20.452821 duty-0.9.0/src/duty/callables/pytest.py
--rw-r--r--   0        0        0    10053 2023-02-18 16:14:20.456154 duty-0.9.0/src/duty/callables/ruff.py
--rw-r--r--   0        0        0     2217 2023-02-18 15:32:33.711095 duty-0.9.0/src/duty/callables/safety.py
--rw-r--r--   0        0        0     7966 2023-02-18 18:32:07.099158 duty-0.9.0/src/duty/cli.py
--rw-r--r--   0        0        0     6512 2023-02-17 18:11:29.418617 duty-0.9.0/src/duty/collection.py
--rw-r--r--   0        0        0     2984 2023-02-17 18:11:30.915261 duty-0.9.0/src/duty/context.py
--rw-r--r--   0        0        0     3021 2023-02-17 18:10:17.209735 duty-0.9.0/src/duty/decorator.py
--rw-r--r--   0        0        0      358 2023-02-17 18:11:31.715248 duty-0.9.0/src/duty/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-18 18:32:04.939193 duty-0.9.0/src/duty/py.typed
--rw-r--r--   0        0        0     6288 2023-02-17 18:11:43.025072 duty-0.9.0/src/duty/validation.py
--rw-r--r--   0        0        0      157 2023-02-18 18:32:04.925860 duty-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0       47 2023-02-18 18:32:04.919193 duty-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0      130 2021-06-18 16:29:00.138929 duty-0.9.0/tests/fixtures/arguments.py
--rw-r--r--   0        0        0       55 2021-06-18 16:29:00.155592 duty-0.9.0/tests/fixtures/basic.py
--rw-r--r--   0        0        0      105 2021-06-18 16:29:00.155592 duty-0.9.0/tests/fixtures/booleans.py
--rw-r--r--   0        0        0       82 2021-06-18 16:29:00.172255 duty-0.9.0/tests/fixtures/code.py
--rw-r--r--   0        0        0      102 2021-06-18 16:29:00.172255 duty-0.9.0/tests/fixtures/list.py
--rw-r--r--   0        0        0      180 2021-06-18 16:29:00.182252 duty-0.9.0/tests/fixtures/multiple.py
--rw-r--r--   0        0        0      121 2021-06-18 16:29:00.182252 duty-0.9.0/tests/fixtures/precedence.py
--rw-r--r--   0        0        0      538 2021-07-19 11:03:47.419786 duty-0.9.0/tests/fixtures/validation.py
--rw-r--r--   0        0        0      335 2023-02-10 14:56:32.165244 duty-0.9.0/tests/fixtures/validation_38.py
--rw-r--r--   0        0        0     6115 2023-02-18 18:32:07.099158 duty-0.9.0/tests/test_cli.py
--rw-r--r--   0        0        0     1918 2023-02-18 16:46:57.019566 duty-0.9.0/tests/test_collection.py
--rw-r--r--   0        0        0     3181 2023-02-18 16:46:57.022899 duty-0.9.0/tests/test_context.py
--rw-r--r--   0        0        0      682 2023-02-18 16:46:57.019566 duty-0.9.0/tests/test_decorator.py
--rw-r--r--   0        0        0     3022 2023-02-18 16:46:57.036232 duty-0.9.0/tests/test_running.py
--rw-r--r--   0        0        0     5386 2023-02-18 16:46:57.019566 duty-0.9.0/tests/test_validation.py
--rw-r--r--   0        0        0     2576 1970-01-01 00:00:00.000000 duty-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-06-26 12:54:11.024581 duty-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1306 2023-06-26 12:54:13.211217 duty-1.0.0/README.md
+-rw-r--r--   0        0        0     2450 2023-06-27 21:46:18.844857 duty-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-06-26 12:54:13.204551 duty-1.0.0/src/duty/__init__.py
+-rw-r--r--   0        0        0      333 2023-06-26 12:54:10.861250 duty-1.0.0/src/duty/__main__.py
+-rw-r--r--   0        0        0     1661 2023-04-10 14:47:07.887091 duty-1.0.0/src/duty/callables/__init__.py
+-rw-r--r--   0        0        0      367 2023-04-13 14:11:08.482199 duty-1.0.0/src/duty/callables/_io.py
+-rw-r--r--   0        0        0     4699 2023-04-13 14:16:42.639974 duty-1.0.0/src/duty/callables/autoflake.py
+-rw-r--r--   0        0        0     7153 2023-04-10 14:49:36.264138 duty-1.0.0/src/duty/callables/black.py
+-rw-r--r--   0        0        0     3221 2023-04-10 14:49:09.981212 duty-1.0.0/src/duty/callables/blacken_docs.py
+-rw-r--r--   0        0        0    23843 2023-06-26 13:00:14.421342 duty-1.0.0/src/duty/callables/coverage.py
+-rw-r--r--   0        0        0     8476 2023-06-26 13:00:14.418009 duty-1.0.0/src/duty/callables/flake8.py
+-rw-r--r--   0        0        0     5060 2023-06-26 13:00:14.418009 duty-1.0.0/src/duty/callables/interrogate.py
+-rw-r--r--   0        0        0    26437 2023-06-26 13:00:14.424676 duty-1.0.0/src/duty/callables/isort.py
+-rw-r--r--   0        0        0     7902 2023-04-10 14:48:43.645095 duty-1.0.0/src/duty/callables/mkdocs.py
+-rw-r--r--   0        0        0    19783 2023-06-26 13:00:14.421342 duty-1.0.0/src/duty/callables/mypy.py
+-rw-r--r--   0        0        0    18380 2023-06-26 13:00:14.424676 duty-1.0.0/src/duty/callables/pytest.py
+-rw-r--r--   0        0        0    10092 2023-05-18 09:14:52.815394 duty-1.0.0/src/duty/callables/ruff.py
+-rw-r--r--   0        0        0     2067 2023-06-26 13:00:14.414676 duty-1.0.0/src/duty/callables/safety.py
+-rw-r--r--   0        0        0      843 2023-04-13 14:02:39.704234 duty-1.0.0/src/duty/callables/ssort.py
+-rw-r--r--   0        0        0     7927 2023-06-26 12:54:13.204551 duty-1.0.0/src/duty/cli.py
+-rw-r--r--   0        0        0     6589 2023-06-26 15:07:41.275411 duty-1.0.0/src/duty/collection.py
+-rw-r--r--   0        0        0     2984 2023-05-18 09:14:38.192258 duty-1.0.0/src/duty/context.py
+-rw-r--r--   0        0        0     3021 2023-02-17 18:10:17.209735 duty-1.0.0/src/duty/decorator.py
+-rw-r--r--   0        0        0      358 2023-02-17 18:11:31.715248 duty-1.0.0/src/duty/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-26 12:54:10.861250 duty-1.0.0/src/duty/py.typed
+-rw-r--r--   0        0        0     7240 2023-06-27 21:37:01.354297 duty-1.0.0/src/duty/validation.py
+-rw-r--r--   0        0        0      157 2023-06-26 12:54:10.841250 duty-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-26 12:54:10.837916 duty-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      130 2021-06-18 16:29:00.138929 duty-1.0.0/tests/fixtures/arguments.py
+-rw-r--r--   0        0        0       55 2021-06-18 16:29:00.155592 duty-1.0.0/tests/fixtures/basic.py
+-rw-r--r--   0        0        0      105 2021-06-18 16:29:00.155592 duty-1.0.0/tests/fixtures/booleans.py
+-rw-r--r--   0        0        0       82 2021-06-18 16:29:00.172255 duty-1.0.0/tests/fixtures/code.py
+-rw-r--r--   0        0        0      102 2021-06-18 16:29:00.172255 duty-1.0.0/tests/fixtures/list.py
+-rw-r--r--   0        0        0      180 2021-06-18 16:29:00.182252 duty-1.0.0/tests/fixtures/multiple.py
+-rw-r--r--   0        0        0      121 2021-06-18 16:29:00.182252 duty-1.0.0/tests/fixtures/precedence.py
+-rw-r--r--   0        0        0      875 2023-06-27 21:07:36.016860 duty-1.0.0/tests/fixtures/validation.py
+-rw-r--r--   0        0        0     6470 2023-06-26 12:54:13.204551 duty-1.0.0/tests/test_cli.py
+-rw-r--r--   0        0        0     2157 2023-04-13 14:33:11.976230 duty-1.0.0/tests/test_collection.py
+-rw-r--r--   0        0        0     3401 2023-04-13 14:33:56.073074 duty-1.0.0/tests/test_context.py
+-rw-r--r--   0        0        0      796 2023-04-13 14:32:18.229261 duty-1.0.0/tests/test_decorator.py
+-rw-r--r--   0        0        0     3264 2023-05-18 09:12:31.970572 duty-1.0.0/tests/test_running.py
+-rw-r--r--   0        0        0     4903 2023-06-27 21:42:16.266864 duty-1.0.0/tests/test_validation.py
+-rw-r--r--   0        0        0     2644 1970-01-01 00:00:00.000000 duty-1.0.0/PKG-INFO
```

### Comparing `duty-0.9.0/LICENSE` & `duty-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `duty-0.9.0/README.md` & `duty-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 With `pip`:
 ```bash
 pip install duty
 ```
 
 With [`pipx`](https://github.com/pipxproject/pipx):
 ```bash
-python3.7 -m pip install --user pipx
+python3.8 -m pip install --user pipx
 pipx install duty
 ```
 
 ## Quick start
 
 Create a `duties.py` file at the root of your repository.
 
@@ -41,7 +41,9 @@
 
 ```bash
 duty docs
 ```
 
 See the [Usage](https://pawamoy.github.io/duty/usage/)
 section in the documentation for more examples.
+
+Also see ["Why choosing duty over..."](https://pawamoy.github.io/duty/#why-duty-over).
```

### Comparing `duty-0.9.0/pyproject.toml` & `duty-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,100 +1,114 @@
 [build-system]
 requires = [
-    "pdm-pep517",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
 
 [project]
 name = "duty"
 description = "A simple task runner."
 authors = [
     { name = "Timothée Mazzucotelli", email = "pawamoy@pm.me" },
 ]
-license = "ISC"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = [
     "task-runner",
     "task",
     "runner",
     "cross-platform",
 ]
 dynamic = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Documentation",
     "Topic :: Software Development",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
-    "failprint>=0.10",
-    "cached-property>=1.5; python_version < '3.8'",
-    "typing-extensions>=4.5; python_version < '3.8'",
+    "failprint>=0.11",
 ]
-version = "0.9.0"
+version = "1.0.0"
+
+[project.license]
+text = "ISC"
 
 [project.urls]
 Homepage = "https://pawamoy.github.io/duty"
 Documentation = "https://pawamoy.github.io/duty"
 Changelog = "https://pawamoy.github.io/duty/changelog"
 Repository = "https://github.com/pawamoy/duty"
 Issues = "https://github.com/pawamoy/duty/issues"
 Discussions = "https://github.com/pawamoy/duty/discussions"
 Gitter = "https://gitter.im/duty/community"
 Funding = "https://github.com/sponsors/pawamoy"
 
 [project.scripts]
 duty = "duty.cli:main"
 
+[tool.pdm]
+plugins = [
+    "pdm-multirun",
+]
+
 [tool.pdm.version]
 source = "scm"
 
 [tool.pdm.build]
 package-dir = "src"
 editable-backend = "editables"
 
 [tool.pdm.dev-dependencies]
+ci-quality = [
+    "duty[docs,quality,typing,security]",
+]
+ci-tests = [
+    "duty[tests]",
+]
 docs = [
+    "black>=23.1",
+    "markdown-callouts>=0.2",
+    "markdown-exec>=0.5",
     "mkdocs>=1.3",
     "mkdocs-coverage>=0.2",
     "mkdocs-gen-files>=0.3",
+    "mkdocs-git-committers-plugin-2>=1.1",
     "mkdocs-literate-nav>=0.4",
     "mkdocs-material>=7.3",
-    "mkdocs-section-index>=0.3",
+    "mkdocs-minify-plugin>=0.6.4",
     "mkdocstrings[python]>=0.18",
-    "markdown-callouts>=0.2",
-    "markdown-exec>=0.5",
     "toml>=0.10",
 ]
 maintain = [
     "black>=23.1",
     "blacken-docs>=1.13",
     "git-changelog>=1.0",
+    "ssort>=0.10.0",
 ]
 quality = [
     "ruff>=0.0.246",
 ]
 tests = [
     "pytest>=6.2",
     "pytest-cov>=3.0",
     "pytest-randomly>=3.10",
     "pytest-xdist>=2.4",
 ]
 typing = [
     "mypy>=0.910",
     "types-markdown>=3.3",
+    "types-pyyaml>=6.0",
     "types-toml>=0.10",
 ]
 security = [
     "safety>=2",
 ]
```

### Comparing `duty-0.9.0/src/duty/callables/__init__.py` & `duty-1.0.0/src/duty/callables/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,35 +24,10 @@
         Slight customizations can be made to support `--flag` / `--no-flag` with single parameters.
     - Use only built-in types: don't make users import and use objects from your API.
         For example, accept a list of strings, not a list of `MyCustomClass` instances.
 """
 
 from __future__ import annotations
 
-from functools import wraps
-from typing import Callable
+from failprint.lazy import lazy
 
-from failprint.lazy import lazy as failprint_lazy
-
-
-def lazy(name: str | None = None) -> Callable:
-    """Transform a callable into a lazy callable.
-
-    Also assign the given name to the callable, for better display.
-
-    Parameters:
-        name: The name to assign to the callable.
-
-    Returns:
-        A lazy callable.
-    """
-
-    def decorator(func: Callable) -> Callable:
-        @wraps(func)
-        def inner(*args, **kwargs):  # noqa: ANN002,ANN003,ANN202
-            return func(*args, **kwargs)
-
-        if name:
-            inner.__name__ = name
-        return failprint_lazy(inner)
-
-    return decorator
+__all__ = ["lazy"]
```

### Comparing `duty-0.9.0/src/duty/callables/autoflake.py` & `duty-1.0.0/src/duty/callables/autoflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Callable for [autoflake](https://github.com/PyCQA/autoflake)."""
 
 from __future__ import annotations
 
-from duty.callables import _io, lazy
+from failprint.lazy import lazy
 
+from duty.callables import _io
 
-@lazy("autoflake")
+
+@lazy(name="autoflake")
 def run(
     *files: str,
     config: str | None = None,
     check: bool | None = None,
     check_diff: bool | None = None,
     imports: list[str] | None = None,
     remove_all_unused_imports: bool | None = None,
@@ -121,10 +123,10 @@
         cli_args.append("--in-place")
 
     if stdout:
         cli_args.append("--stdout")
 
     return autoflake(
         cli_args,
-        standard_out=_io._LazyStdout(),  # noqa: SLF001
-        standard_error=_io._LazyStderr(),  # noqa: SLF001
+        standard_out=_io._LazyStdout(),
+        standard_error=_io._LazyStderr(),
     )
```

### Comparing `duty-0.9.0/src/duty/callables/black.py` & `duty-1.0.0/src/duty/callables/black.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Callable for [Black](https://github.com/psf/black)."""
 
 from __future__ import annotations
 
-from duty.callables import lazy
+from failprint.lazy import lazy
 
 
-@lazy("black")
+@lazy(name="black")
 def run(
     *src: str,
     config: str | None = None,
     code: str | None = None,
     line_length: int | None = None,
     target_version: str | None = None,
     check: bool | None = None,
```

### Comparing `duty-0.9.0/src/duty/callables/blacken_docs.py` & `duty-1.0.0/src/duty/callables/blacken_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from __future__ import annotations
 
 import re
 from pathlib import Path
 from typing import Pattern, Sequence
 
-from duty.callables import lazy
+from failprint.lazy import lazy
 
 
-@lazy("blacken_docs")
+@lazy(name="blacken_docs")
 def run(
     *paths: str | Path,
     exts: Sequence[str] | None = None,
     exclude: Sequence[str | Pattern] | None = None,
     skip_errors: bool = False,
     rst_literal_blocks: bool = False,
     line_length: int | None = None,
```

### Comparing `duty-0.9.0/src/duty/callables/coverage.py` & `duty-1.0.0/src/duty/callables/coverage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 """Callable for [Coverage.py](https://github.com/nedbat/coveragepy)."""
 
 from __future__ import annotations
 
-import sys
+from typing import Literal
 
-from duty.callables import lazy
-
-# TODO: remove once support for Python 3.7 is dropped
-if sys.version_info < (3, 8):
-    from typing_extensions import Literal
-else:
-    from typing import Literal
+from failprint.lazy import lazy
 
 
 def _run(args: list[str]) -> None:
     from coverage.cmdline import main as coverage
 
     coverage(args)
 
 
-@lazy("coverage.annotate")
+@lazy(name="coverage.annotate")
 def annotate(
     *,
     rcfile: str | None = None,
     directory: str | None = None,
     data_file: str | None = None,
     ignore_errors: bool | None = None,
     include: list[str] | None = None,
@@ -74,15 +68,15 @@
     if rcfile:
         cli_args.append("--rcfile")
         cli_args.append(rcfile)
 
     _run(cli_args)
 
 
-@lazy("coverage.combine")
+@lazy(name="coverage.combine")
 def combine(
     *paths: str,
     rcfile: str | None = None,
     append: bool | None = None,
     data_file: str | None = None,
     keep: bool | None = None,
     quiet: bool | None = None,
@@ -128,15 +122,15 @@
     if rcfile:
         cli_args.append("--rcfile")
         cli_args.append(rcfile)
 
     _run(cli_args)
 
 
-@lazy("coverage.debug")
+@lazy(name="coverage.debug")
 def debug(
     topic: Literal["data", "sys", "config", "premain", "pybehave"],
     *,
     rcfile: str | None = None,
     debug_opts: list[str] | None = None,
 ) -> None:
     """Display information about the internals of coverage.py.
@@ -162,15 +156,15 @@
     if rcfile:
         cli_args.append("--rcfile")
         cli_args.append(rcfile)
 
     _run(cli_args)
 
 
-@lazy("coverage.erase")
+@lazy(name="coverage.erase")
 def erase(
     *,
     rcfile: str | None = None,
     data_file: str | None = None,
     debug_opts: list[str] | None = None,
 ) -> None:
     """Erase previously collected coverage data.
@@ -195,15 +189,15 @@
     if rcfile:
         cli_args.append("--rcfile")
         cli_args.append(rcfile)
 
     _run(cli_args)
 
 
-@lazy("coverage.html")
+@lazy(name="coverage.html")
 def html(
     *,
     rcfile: str | None = None,
     contexts: list[str] | None = None,
     directory: str | None = None,
     data_file: str | None = None,
     fail_under: int | None = None,
@@ -301,15 +295,15 @@
     if rcfile:
         cli_args.append("--rcfile")
         cli_args.append(rcfile)
 
     _run(cli_args)
 
 
-@lazy("coverage.json")
+@lazy(name="coverage.json")
 def json(
     *,
     rcfile: str | None = None,
     contexts: list[str] | None = None,
     data_file: str | None = None,
     fail_under: int | None = None,
     ignore_errors: bool | None = None,
@@ -385,15 +379,15 @@
     if rcfile:
         cli_args.append("--rcfile")
         cli_args.append(rcfile)
 
     _run(cli_args)
 
 
-@lazy("coverage.lcov")
+@lazy(name="coverage.lcov")
 def lcov(
     *,
     rcfile: str | None = None,
     data_file: str | None = None,
     fail_under: int | None = None,
     ignore_errors: bool | None = None,
     include: list[str] | None = None,
@@ -452,15 +446,15 @@
     if rcfile:
         cli_args.append("--rcfile")
         cli_args.append(rcfile)
 
     _run(cli_args)
 
 
-@lazy("coverage.report")
+@lazy(name="coverage.report")
 def report(
     *,
     rcfile: str | None = None,
     contexts: list[str] | None = None,
     data_file: str | None = None,
     fail_under: int | None = None,
     output_format: Literal["text", "markdown", "total"] | None = None,
@@ -549,15 +543,15 @@
     if rcfile:
         cli_args.append("--rcfile")
         cli_args.append(rcfile)
 
     _run(cli_args)
 
 
-@lazy("coverage.run")
+@lazy(name="coverage.run")
 def run(
     pyfile: str,
     *,
     rcfile: str | None = None,
     append: bool | None = None,
     branch: bool | None = None,
     concurrency: list[str] | None = None,
@@ -646,15 +640,15 @@
     if rcfile:
         cli_args.append("--rcfile")
         cli_args.append(rcfile)
 
     _run(cli_args)
 
 
-@lazy("coverage.xml")
+@lazy(name="coverage.xml")
 def xml(
     *,
     rcfile: str | None = None,
     data_file: str | None = None,
     fail_under: int | None = None,
     ignore_errors: bool | None = None,
     include: list[str] | None = None,
```

### Comparing `duty-0.9.0/src/duty/callables/flake8.py` & `duty-1.0.0/src/duty/callables/flake8.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 """Callable for [Flake8](https://github.com/PyCQA/flake8)."""
 
 from __future__ import annotations
 
 import sys
+from typing import Literal
 
-from duty.callables import lazy
+from failprint.lazy import lazy
 
-# TODO: remove once support for Python 3.7 is dropped
-if sys.version_info < (3, 8):
-    from typing_extensions import Literal
-else:
-    from typing import Literal
 
-
-@lazy("flake8")
+@lazy(name="flake8")
 def run(
     *paths: str,
     config: str | None = None,
     verbose: bool | None = None,
     output_file: str | None = None,
     append_config: str | None = None,
     isolated: bool | None = None,
```

### Comparing `duty-0.9.0/src/duty/callables/interrogate.py` & `duty-1.0.0/src/duty/callables/interrogate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 """Callable for [Interrogate](https://github.com/econchick/interrogate)."""
 
 from __future__ import annotations
 
-import sys
+from typing import Literal
 
-from duty.callables import lazy
-
-# TODO: remove once support for Python 3.7 is dropped
-if sys.version_info < (3, 8):
-    from typing_extensions import Literal
-else:
-    from typing import Literal
+from failprint.lazy import lazy
 
 _BADGE_STYLE = Literal["flat", "flat-square", "flat-square-modified", "for-the-badge", "plastic", "social"]
 
 
-@lazy("interrogate")
+@lazy(name="interrogate")
 def run(
     *src: str,
     verbose: int | None = None,
     quiet: bool | None = None,
     fail_under: float | None = None,
     exclude: str | None = None,
     ignore_init_method: bool | None = None,
```

### Comparing `duty-0.9.0/src/duty/callables/isort.py` & `duty-1.0.0/src/duty/callables/isort.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 """Callable for [isort](https://github.com/PyCQA/isort)."""
 
 from __future__ import annotations
 
-import sys
+from typing import Literal
 
-from duty.callables import lazy
-
-# TODO: remove once support for Python 3.7 is dropped
-if sys.version_info < (3, 8):
-    from typing_extensions import Literal
-else:
-    from typing import Literal
+from failprint.lazy import lazy
 
 Multiline = Literal[
     "GRID",
     "VERTICAL",
     "HANGING_INDENT",
     "VERTICAL_HANGING_INDENT",
     "VERTICAL_GRID",
@@ -36,15 +30,15 @@
     "8",
     "9",
     "10",
     "11",
 ]
 
 
-@lazy("isort")
+@lazy(name="isort")
 def run(
     *files: str,
     settings: str | None = None,
     verbose: bool | None = None,
     only_modified: bool | None = None,
     dedup_headings: bool | None = None,
     quiet: bool | None = None,
```

### Comparing `duty-0.9.0/src/duty/callables/mkdocs.py` & `duty-1.0.0/src/duty/callables/mkdocs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Callable for [MkDocs](https://github.com/mkdocs/mkdocs)."""
 
 from __future__ import annotations
 
-from duty.callables import lazy
+from failprint.lazy import lazy
 
 
 def run(*args: str, quiet: bool = False, verbose: bool = False) -> None:
     """Run `mkdocs`.
 
     Parameters:
         *args: CLI arguments.
@@ -22,15 +22,15 @@
 
     if verbose and "-v" not in cli_args:
         cli_args.append("--verbose")
 
     mkdocs(cli_args)
 
 
-@lazy("mkdocs.build")
+@lazy(name="mkdocs.build")
 def build(
     *,
     config_file: str | None = None,
     clean: bool | None = None,
     strict: bool | None = None,
     theme: str | None = None,
     directory_urls: bool | None = None,
@@ -76,15 +76,15 @@
     if site_dir:
         cli_args.append("--site_dir")
         cli_args.append(site_dir)
 
     run("build", *cli_args, quiet=quiet, verbose=verbose)
 
 
-@lazy("mkdocs.gh_deploy")
+@lazy(name="mkdocs.gh_deploy")
 def gh_deploy(
     *,
     config_file: str | None = None,
     clean: bool | None = None,
     message: str | None = None,
     remote_branch: str | None = None,
     remote_name: str | None = None,
@@ -169,27 +169,27 @@
     if site_dir:
         cli_args.append("--site_dir")
         cli_args.append(site_dir)
 
     run("gh-deploy", *cli_args, quiet=quiet, verbose=verbose)
 
 
-@lazy("mkdocs.new")
+@lazy(name="mkdocs.new")
 def new(project_directory: str, *, quiet: bool = False, verbose: bool = False) -> None:
     """Create a new MkDocs project.
 
     Parameters:
         project_directory: Where to create the project.
         quiet: Silence warnings.
         verbose: Enable verbose output.
     """
     run("new", project_directory, quiet=quiet, verbose=verbose)
 
 
-@lazy("mkdocs.serve")
+@lazy(name="mkdocs.serve")
 def serve(
     *,
     config_file: str | None = None,
     dev_addr: str | None = None,
     livereload: bool | None = None,
     dirtyreload: bool | None = None,
     watch_theme: bool | None = None,
```

### Comparing `duty-0.9.0/src/duty/callables/mypy.py` & `duty-1.0.0/src/duty/callables/mypy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 """Callable for [Mypy](https://github.com/python/mypy)."""
 
 from __future__ import annotations
 
-import sys
+from typing import Literal
 
-from duty.callables import lazy
-from duty.callables._io import _LazyStderr, _LazyStdout
+from failprint.lazy import lazy
 
-# TODO: remove once support for Python 3.7 is dropped
-if sys.version_info < (3, 8):
-    from typing_extensions import Literal
-else:
-    from typing import Literal
+from duty.callables._io import _LazyStderr, _LazyStdout
 
 
-@lazy("mypy")
+@lazy(name="mypy")
 def run(
     *paths: str,
     config_file: str | None = None,
     enable_incomplete_feature: bool | None = None,
     verbose: bool | None = None,
     warn_unused_configs: bool | None = None,
     no_namespace_packages: bool | None = None,
```

### Comparing `duty-0.9.0/src/duty/callables/pytest.py` & `duty-1.0.0/src/duty/callables/pytest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 """Callable for [pytest](https://github.com/pytest-dev/pytest)."""
 
 from __future__ import annotations
 
-import sys
+from typing import Literal
 
-from duty.callables import lazy
+from failprint.lazy import lazy
 
-# TODO: remove once support for Python 3.7 is dropped
-if sys.version_info < (3, 8):
-    from typing_extensions import Literal
-else:
-    from typing import Literal
 
-
-@lazy("pytest")
+@lazy(name="pytest")
 def run(
     *paths: str,
     config_file: str | None = None,
     select: str | None = None,
     select_markers: str | None = None,
     markers: bool | None = None,
     exitfirst: bool | None = None,
```

### Comparing `duty-0.9.0/src/duty/callables/ruff.py` & `duty-1.0.0/src/duty/callables/ruff.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 import os
 import subprocess
 import sys
 from functools import lru_cache
 
-from duty.callables import lazy
+from failprint.lazy import lazy
 
 
 @lru_cache(maxsize=None)
 def _find_ruff() -> str:
     from ruff.__main__ import find_ruff_bin
 
     try:
@@ -43,20 +43,20 @@
 
     if quiet:
         cli_args.append("--quiet")
 
     if silent:
         cli_args.append("--silent")
 
-    process = subprocess.run([_find_ruff(), *cli_args], capture_output=True, text=True)
+    process = subprocess.run([_find_ruff(), *cli_args], capture_output=True, text=True)  # noqa: S603
     print(process.stdout)  # noqa: T201
     return process.returncode
 
 
-@lazy("ruff.check")
+@lazy(name="ruff.check")
 def check(
     *files: str,
     config: str | None = None,
     fix: bool | None = None,
     show_source: bool | None = None,
     show_fixes: bool | None = None,
     diff: bool | None = None,
@@ -221,15 +221,15 @@
 
     if exit_non_zero_on_fix:
         cli_args.append("--exit-non-zero-on-fix")
 
     return _run("check", *cli_args, verbose=verbose, quiet=quiet, silent=silent)
 
 
-@lazy("ruff.rule")
+@lazy(name="ruff.rule")
 def rule(
     *,
     output_format: str | None = None,
     verbose: bool = False,
     quiet: bool = False,
     silent: bool = False,
 ) -> int:
@@ -246,15 +246,15 @@
     if output_format:
         cli_args.append("--format")
         cli_args.append(output_format)
 
     return _run("rule", *cli_args, verbose=verbose, quiet=quiet, silent=silent)
 
 
-@lazy("ruff.config")
+@lazy(name="ruff.config")
 def config(
     *,
     verbose: bool = False,
     quiet: bool = False,
     silent: bool = False,
 ) -> int:
     """List or describe the available configuration options.
@@ -263,15 +263,15 @@
         verbose: Enable verbose logging.
         quiet: Print lint violations, but nothing else.
         silent: Disable all logging (but still exit with status code "1" upon detecting lint violations).
     """
     return _run("config", verbose=verbose, quiet=quiet, silent=silent)
 
 
-@lazy("ruff.linter")
+@lazy(name="ruff.linter")
 def linter(
     *,
     output_format: str | None = None,
     verbose: bool = False,
     quiet: bool = False,
     silent: bool = False,
 ) -> int:
@@ -288,15 +288,15 @@
     if output_format:
         cli_args.append("--format")
         cli_args.append(output_format)
 
     return _run("linter", *cli_args, verbose=verbose, quiet=quiet, silent=silent)
 
 
-@lazy("ruff.clean")
+@lazy(name="ruff.clean")
 def clean(
     *,
     verbose: bool = False,
     quiet: bool = False,
     silent: bool = False,
 ) -> int:
     """Clear any caches in the current directory and any subdirectories.
```

### Comparing `duty-0.9.0/src/duty/callables/safety.py` & `duty-1.0.0/src/duty/callables/safety.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 """Callable for [Safety](https://github.com/pyupio/safety)."""
 
 from __future__ import annotations
 
 import importlib
 import sys
 from io import StringIO
-from typing import Sequence, cast
+from typing import Literal, Sequence, cast
 
-from duty.callables import lazy
+from failprint.lazy import lazy
 
-# TODO: remove once support for Python 3.7 is dropped
-if sys.version_info < (3, 8):
-    from typing_extensions import Literal
-else:
-    from typing import Literal
 
-
-@lazy("safety.check")
+@lazy(name="safety.check")
 def check(
     requirements: str | Sequence[str],
     *,
     ignore_vulns: dict[str, str] | None = None,
     formatter: Literal["json", "bare", "text"] = "text",
     full_report: bool = True,
 ) -> bool:
```

### Comparing `duty-0.9.0/src/duty/cli.py` & `duty-1.0.0/src/duty/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         metavar="DUTY",
         help="Show this help message and exit. Pass duties names to print their help.",
     )
 
     add_flags(parser, set_defaults=False)
     parser.add_argument("remainder", nargs=argparse.REMAINDER)
 
-    parser._optionals.title = "Global options"  # noqa: SLF001
+    parser._optionals.title = "Global options"
 
     return parser
 
 
 def split_args(args: list[str], names: list[str]) -> list[list[str]]:
     """Split command line arguments into duty commands.
 
@@ -258,15 +258,15 @@
     try:
         arg_lists = split_args(remainder, collection.names())
     except ValueError as error:
         print(error, file=sys.stderr)
         return 1
 
     if not arg_lists:
-        print("> Please choose at least one duty", file=sys.stderr)
+        print_help(parser, opts, collection)
         return 1
 
     global_opts = specified_options(opts, exclude={"duties_file", "list", "help", "remainder"})
     try:
         commands = parse_commands(arg_lists, global_opts, collection)
     except TypeError as error:
         print(f"> {error}", file=sys.stderr)
```

### Comparing `duty-0.9.0/src/duty/collection.py` & `duty-1.0.0/src/duty/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,117 +1,26 @@
 """Module containing all the logic."""
 from __future__ import annotations
 
 import inspect
+import sys
 from copy import deepcopy
 from importlib import util as importlib_util
-from typing import Any, Callable, List, Union
+from typing import Any, Callable, ClassVar, List, Union
 
 from duty.context import Context
 
 DutyListType = List[Union[str, Callable, "Duty"]]
 default_duties_file = "duties.py"
 
 
-class Collection:
-    """A collection of duties.
-
-    Attributes:
-        path: The path to the duties file.
-        duties: The list of duties.
-        aliases: A dictionary of aliases pointing to their respective duties.
-    """
-
-    def __init__(self, path: str = default_duties_file) -> None:
-        """Initialize the collection.
-
-        Parameters:
-            path: The path to the duties file.
-        """
-        self.path = path
-        self.duties: dict[str, Duty] = {}
-        self.aliases: dict[str, Duty] = {}
-
-    def clear(self) -> None:
-        """Clear the collection."""
-        self.duties.clear()
-        self.aliases.clear()
-
-    def names(self) -> list[str]:
-        """Return the list of duties names and aliases.
-
-        Returns:
-            The list of duties names and aliases.
-        """
-        return list(self.duties.keys()) + list(self.aliases.keys())
-
-    def get(self, name_or_alias: str) -> Duty:
-        """Get a duty by its name or alias.
-
-        Parameters:
-            name_or_alias: The name or alias of the duty.
-
-        Returns:
-            A duty.
-        """
-        try:
-            return self.duties[name_or_alias]
-        except KeyError:
-            return self.aliases[name_or_alias]
-
-    def format_help(self) -> str:
-        """Format a message listing the duties.
-
-        Returns:
-            A string listing the duties and their summary.
-        """
-        lines = []
-        # 20 makes the summary aligned with options description
-        longest_name = max(max(len(name) for name in self.duties), 20)
-        for name, duty in self.duties.items():
-            description = duty.description.split("\n")[0]
-            lines.append(f"{name:{longest_name}}  {description}")
-        return "\n".join(lines)
-
-    def load(self, path: str | None = None) -> None:
-        """Load duties from a Python file.
-
-        Parameters:
-            path: The path to the Python file to load.
-                Uses the collection's path by default.
-        """
-        path = path or self.path
-        spec = importlib_util.spec_from_file_location("duty.duties", path)
-        if spec:
-            duties = importlib_util.module_from_spec(spec)
-            spec.loader.exec_module(duties)  # type: ignore[union-attr]
-            declared_duties = inspect.getmembers(duties, lambda member: isinstance(member, Duty))
-            for _, duty in declared_duties:
-                self.add(duty)
-
-    def add(self, duty: Duty) -> None:
-        """Add a duty to the collection.
-
-        Parameters:
-            duty: The duty to add.
-        """
-        if duty.collection is not None:
-            # we must copy the duty to be able to add it
-            # in multiple collections
-            duty = deepcopy(duty)
-        duty.collection = self
-        self.duties[duty.name] = duty
-        for alias in duty.aliases:
-            self.aliases[alias] = duty
-
-
 class Duty:
     """The main duty class."""
 
-    default_options: dict[str, Any] = {}
+    default_options: ClassVar[dict[str, Any]] = {}
 
     def __init__(
         self,
         name: str,
         description: str,
         function: Callable,
         collection: Collection | None = None,
@@ -141,26 +50,14 @@
         self.options = opts or self.default_options
         self.options_override: dict = {}
 
         self.collection: Collection | None = None
         if collection:
             collection.add(self)
 
-    def __call__(self, context: Context, *args: Any, **kwargs: Any) -> None:
-        """Run the duty function.
-
-        Parameters:
-            context: The context to use.
-            args: Positional arguments passed to the function.
-            kwargs: Keyword arguments passed to the function.
-        """
-        self.run_duties(context, self.pre)
-        self.function(context, *args, **kwargs)
-        self.run_duties(context, self.post)
-
     @property
     def context(self) -> Context:
         """Return a new context instance.
 
         Returns:
             A new context instance.
         """
@@ -195,7 +92,112 @@
                 duty_item(context)
             elif isinstance(duty_item, str):
                 # Item is a reference to a duty.
                 if self.collection is None:
                     raise RuntimeError(f"Can't find duty by name without a collection ({duty_item})")
                 # Get the duty and run it.
                 self.collection.get(duty_item)(context)
+
+    def __call__(self, context: Context, *args: Any, **kwargs: Any) -> None:
+        """Run the duty function.
+
+        Parameters:
+            context: The context to use.
+            args: Positional arguments passed to the function.
+            kwargs: Keyword arguments passed to the function.
+        """
+        self.run_duties(context, self.pre)
+        self.function(context, *args, **kwargs)
+        self.run_duties(context, self.post)
+
+
+class Collection:
+    """A collection of duties.
+
+    Attributes:
+        path: The path to the duties file.
+        duties: The list of duties.
+        aliases: A dictionary of aliases pointing to their respective duties.
+    """
+
+    def __init__(self, path: str = default_duties_file) -> None:
+        """Initialize the collection.
+
+        Parameters:
+            path: The path to the duties file.
+        """
+        self.path = path
+        self.duties: dict[str, Duty] = {}
+        self.aliases: dict[str, Duty] = {}
+
+    def clear(self) -> None:
+        """Clear the collection."""
+        self.duties.clear()
+        self.aliases.clear()
+
+    def names(self) -> list[str]:
+        """Return the list of duties names and aliases.
+
+        Returns:
+            The list of duties names and aliases.
+        """
+        return list(self.duties.keys()) + list(self.aliases.keys())
+
+    def get(self, name_or_alias: str) -> Duty:
+        """Get a duty by its name or alias.
+
+        Parameters:
+            name_or_alias: The name or alias of the duty.
+
+        Returns:
+            A duty.
+        """
+        try:
+            return self.duties[name_or_alias]
+        except KeyError:
+            return self.aliases[name_or_alias]
+
+    def format_help(self) -> str:
+        """Format a message listing the duties.
+
+        Returns:
+            A string listing the duties and their summary.
+        """
+        lines = []
+        # 20 makes the summary aligned with options description
+        longest_name = max(*(len(name) for name in self.duties), 20)
+        for name, duty in self.duties.items():
+            description = duty.description.split("\n")[0]
+            lines.append(f"{name:{longest_name}}  {description}")
+        return "\n".join(lines)
+
+    def add(self, duty: Duty) -> None:
+        """Add a duty to the collection.
+
+        Parameters:
+            duty: The duty to add.
+        """
+        if duty.collection is not None:
+            # we must copy the duty to be able to add it
+            # in multiple collections
+            duty = deepcopy(duty)
+        duty.collection = self
+        self.duties[duty.name] = duty
+        for alias in duty.aliases:
+            self.aliases[alias] = duty
+
+    def load(self, path: str | None = None) -> None:
+        """Load duties from a Python file.
+
+        Parameters:
+            path: The path to the Python file to load.
+                Uses the collection's path by default.
+        """
+        path = path or self.path
+        spec = importlib_util.spec_from_file_location("duty.duties", path)
+        if spec:
+            duties = importlib_util.module_from_spec(spec)
+            sys.modules["duty.duties"] = duties
+            spec.loader.exec_module(duties)  # type: ignore[union-attr]
+            declared_duties = inspect.getmembers(duties, lambda member: isinstance(member, Duty))
+            for _, duty in declared_duties:
+                self.add(duty)
```

### Comparing `duty-0.9.0/src/duty/context.py` & `duty-1.0.0/src/duty/context.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,34 @@
             options_override: Options that override `run` and `@duty` options.
                 This argument is used to allow users to override options from the CLI or environment.
         """
         self._options = options
         self._option_stack: list[dict[str, Any]] = []
         self._options_override = options_override or {}
 
+    @contextmanager
+    def cd(self, directory: str) -> Iterator:
+        """Change working directory as a context manager.
+
+        Parameters:
+            directory: The directory to go into.
+
+        Yields:
+            Nothing.
+        """
+        if not directory:
+            yield
+            return
+        old_wd = os.getcwd()
+        os.chdir(directory)
+        try:
+            yield
+        finally:
+            os.chdir(old_wd)
+
     def run(self, cmd: CmdType, **options: Any) -> str:
         """Run a command in a subprocess or a Python callable.
 
         Parameters:
             cmd: A command or a Python callable.
             options: Options passed to `failprint` functions.
 
@@ -77,27 +97,7 @@
         """
         self._option_stack.append(self._options)
         self._options = {**self._options, **opts}
         try:
             yield
         finally:
             self._options = self._option_stack.pop()
-
-    @contextmanager
-    def cd(self, directory: str) -> Iterator:
-        """Change working directory as a context manager.
-
-        Parameters:
-            directory: The directory to go into.
-
-        Yields:
-            Nothing.
-        """
-        if not directory:
-            yield
-            return
-        old_wd = os.getcwd()
-        os.chdir(directory)
-        try:
-            yield
-        finally:
-            os.chdir(old_wd)
```

### Comparing `duty-0.9.0/src/duty/decorator.py` & `duty-1.0.0/src/duty/decorator.py`

 * *Files identical despite different names*

### Comparing `duty-0.9.0/src/duty/validation.py` & `duty-1.0.0/src/duty/validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,19 @@
 effectively checking all CLI arguments and failing early
 if they are incorrect.
 """
 
 from __future__ import annotations
 
 import sys
+import textwrap
+from functools import cached_property
 from inspect import Parameter, Signature, signature
 from typing import Any, Callable, Sequence
 
-# TODO: remove once support for Python 3.7 is dropped
-if sys.version_info < (3, 8):
-    from cached_property import cached_property
-else:
-    from functools import cached_property
-
 
 def to_bool(value: str) -> bool:
     """Convert a string to a boolean.
 
     Parameters:
         value: The string to convert.
 
@@ -49,33 +45,22 @@
     except Exception:  # noqa: BLE001
         return arg
 
 
 class ParamsCaster:
     """A helper class to cast parameters based on a function's signature annotations."""
 
-    def __init__(self, function: Callable) -> None:
+    def __init__(self, signature: Signature) -> None:
         """Initialize the object.
 
         Parameters:
-            function: The function to use to cast arguments.
+            signature: The signature to use to cast arguments.
         """
-        self.function = function
-        self.signature = signature(function)
-        self.params_dict = self.signature.parameters
-        self.params_list = list(self.params_dict.values())[1:]
-
-    @cached_property
-    def has_var_positional(self) -> bool:
-        """Tell if there is a variable positional parameter.
-
-        Returns:
-            True or False.
-        """
-        return self.var_positional_position >= 0
+        self.params_dict = signature.parameters
+        self.params_list = list(self.params_dict.values())
 
     @cached_property
     def var_positional_position(self) -> int:
         """Give the position of the variable positional parameter in the signature.
 
         Returns:
             The position of the variable positional parameter.
@@ -84,14 +69,23 @@
         for param in self.params_list:
             if param.kind is Parameter.VAR_POSITIONAL:
                 return pos
             pos += 1
         return -1
 
     @cached_property
+    def has_var_positional(self) -> bool:
+        """Tell if there is a variable positional parameter.
+
+        Returns:
+            True or False.
+        """
+        return self.var_positional_position >= 0
+
+    @cached_property
     def var_positional_annotation(self) -> Any:
         """Give the variable positional parameter (`*args`) annotation if any.
 
         Returns:
             The variable positional parameter annotation.
         """
         return self.params_list[self.var_positional_position].annotation
@@ -169,14 +163,62 @@
             The cast arguments.
         """
         positional = tuple(self.cast_posarg(pos, arg) for pos, arg in enumerate(args))
         keyword = {name: self.cast_kwarg(name, value) for name, value in kwargs.items()}
         return positional, keyword
 
 
+def _get_params_caster(func: Callable, *args: Any, **kwargs: Any) -> ParamsCaster:
+    duties_module = sys.modules[func.__module__]
+    exec_globals = dict(duties_module.__dict__)
+    eval_str = False
+    for name in list(exec_globals.keys()):
+        if exec_globals[name] is annotations:
+            eval_str = True
+            del exec_globals[name]
+    exec_globals["__context_above"] = {}
+
+    # Don't keep first parameter: context.
+    params = list(signature(func).parameters.values())[1:]
+    params_no_types = [Parameter(param.name, param.kind, default=param.default) for param in params]
+    code_sig = Signature(parameters=params_no_types)
+    if eval_str:
+        params_types = [
+            Parameter(
+                param.name,
+                param.kind,
+                default=param.default,
+                annotation=eval(  # noqa: PGH001
+                    param.annotation,
+                    exec_globals,
+                )
+                if param.annotation is not Parameter.empty
+                else type(param.default),
+            )
+            for param in params
+        ]
+    else:
+        params_types = params
+    cast_sig = Signature(parameters=params_types)
+
+    code = f"""
+        import inspect
+        def {func.__name__}{code_sig}: ...
+        __context_above['func'] = {func.__name__}
+    """
+
+    exec(textwrap.dedent(code), exec_globals)  # noqa: S102
+    func = exec_globals["__context_above"]["func"]
+
+    # Trigger TypeError early.
+    func(*args, **kwargs)
+
+    return ParamsCaster(cast_sig)
+
+
 def validate(
     func: Callable,
     *args: Any,
     **kwargs: Any,
 ) -> tuple[Sequence, dict[str, Any]]:
     """Validate positional and keyword arguments against a function.
 
@@ -191,18 +233,8 @@
         func: The function to copy.
         *args: The positional arguments.
         **kwargs: The keyword arguments.
 
     Returns:
         The casted arguments.
     """
-    name = func.__name__
-
-    # don't keep first parameter: context
-    params_list = list(signature(func).parameters.values())[1:]
-    params = [Parameter(param.name, param.kind, default=param.default) for param in params_list]
-    sig = Signature(parameters=params)
-    trixx: dict = {}
-    exec(f"def {name}{sig}: ...\ntrixx[0] = {name}")  # noqa: S102
-    trixx[0](*args, **kwargs)
-    caster = ParamsCaster(func)
-    return caster.cast(*args, **kwargs)
+    return _get_params_caster(func, *args, **kwargs).cast(*args, **kwargs)
```

### Comparing `duty-0.9.0/tests/fixtures/validation.py` & `duty-1.0.0/tests/fixtures/validation.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,7 +24,23 @@
 
 def varkw_param(ctx, a: int, **b: int):
     pass  # pragma: no cover
 
 
 def varkw_no_annotation(ctx, **a):
     pass  # pragma: no cover
+
+
+def posonly_marker(ctx, a: int, /, b: int):
+    pass  # pragma: no cover
+
+
+def kwonly_marker(ctx, a: int, *, b: int):
+    pass  # pragma: no cover
+
+
+def only_markers(ctx, a: int, /, b: int, *, c: int):
+    pass  # pragma: no cover
+
+
+def full(ctx, a: int, /, b: int, *c: int, d: int, e: int = 0, **f: int):
+    pass  # pragma: no cover
```

### Comparing `duty-0.9.0/tests/test_cli.py` & `duty-1.0.0/tests/test_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,97 +1,99 @@
 """Tests for the `cli` module."""
 
+from __future__ import annotations
+
 import pytest
 
 from duty import cli
 
 
-def test_no_duty(capsys):
+def test_no_duty(capsys: pytest.CaptureFixture) -> None:
     """Run no duties.
 
     Parameters:
         capsys: Pytest fixture to capture output.
     """
     assert cli.main([]) == 1
     captured = capsys.readouterr()
-    assert "choose at least one duty" in captured.err
+    assert "Available duties" in captured.out
 
 
-def test_show_help(capsys):
+def test_show_help(capsys: pytest.CaptureFixture) -> None:
     """Show help.
 
     Parameters:
         capsys: Pytest fixture to capture output.
     """
     assert cli.main(["-h"]) == 0
     captured = capsys.readouterr()
     assert "duty" in captured.out
 
 
-def test_show_help_for_given_duties(capsys):
+def test_show_help_for_given_duties(capsys: pytest.CaptureFixture) -> None:
     """Show help for given duties.
 
     Parameters:
         capsys: Pytest fixture to capture output.
     """
     assert cli.main(["-d", "tests/fixtures/basic.py", "-h", "hello"]) == 0
     captured = capsys.readouterr()
     assert "hello" in captured.out
 
 
-def test_show_help_unknown_duty(capsys):
+def test_show_help_unknown_duty(capsys: pytest.CaptureFixture) -> None:
     """Show help for an unknown duty.
 
     Parameters:
         capsys: Pytest fixture to capture output.
     """
     assert cli.main(["-d", "tests/fixtures/basic.py", "-h", "not-here"]) == 0
     captured = capsys.readouterr()
     assert "Unknown duty" in captured.out
 
 
-def test_select_duties():
+def test_select_duties() -> None:
     """Run a duty."""
     assert cli.main(["-d", "tests/fixtures/basic.py", "hello"]) == 0
 
 
-def test_unknown_duty():
+def test_unknown_duty() -> None:
     """Don't run an unknown duty."""
     assert cli.main(["-d", "tests/fixtures/basic.py", "byebye"]) == 1
 
 
-def test_incorrect_arguments():
+def test_incorrect_arguments() -> None:
     """Use incorrect arguments."""
     assert cli.main(["-d", "tests/fixtures/basic.py", "hello=1"]) == 1
 
 
 # we use 300 because it's slightly above the valid maximum 255
 @pytest.mark.parametrize("code", range(-100, 300, 7))
-def test_duty_failure(code):
+def test_duty_failure(code: int) -> None:
     """Check exit code.
 
     Parameters:
         code: Code to match.
     """
     assert cli.main(["-d", "tests/fixtures/code.py", "exit_with", f"code={code}"]) == code
 
 
-def test_multiple_duties(capsys):
+def test_multiple_duties(capsys: pytest.CaptureFixture) -> None:
     """Run multiple duties.
 
     Parameters:
         capsys: Pytest fixture to capture output.
     """
     assert cli.main(["-d", "tests/fixtures/multiple.py", "first_duty", "second_duty"]) == 0
     captured = capsys.readouterr()
     assert "first" in captured.out
     assert "second" in captured.out
 
 
-def test_duty_arguments(capsys):
+def test_duty_arguments(capsys: pytest.CaptureFixture) -> None:
     """Run duty with arguments.
 
     Parameters:
         capsys: Pytest fixture to capture output.
     """
     assert cli.main(["-d", "tests/fixtures/arguments.py", "say_hello", "cat=fabric"]) == 0
     captured = capsys.readouterr()
@@ -100,37 +102,37 @@
 
     assert cli.main(["-d", "tests/fixtures/arguments.py", "say_hello", "dog=paramiko", "cat=invoke"]) == 0
     captured = capsys.readouterr()
     assert "cat invoke" in captured.out
     assert "dog paramiko" in captured.out
 
 
-def test_list_duties(capsys):
+def test_list_duties(capsys: pytest.CaptureFixture) -> None:
     """List duties.
 
     Parameters:
         capsys: Pytest fixture to capture output.
     """
     assert cli.main(["-d", "tests/fixtures/list.py", "-l"]) == 0
     captured = capsys.readouterr()
     assert "Tong..." in captured.out
     assert "DEUM!" in captured.out
 
 
-def test_global_options():
+def test_global_options() -> None:
     """Test global options."""
     assert cli.main(["-d", "tests/fixtures/code.py", "-z", "exit_with", "1"]) == 0
 
 
-def test_global_and_local_options():
+def test_global_and_local_options() -> None:
     """Test global and local options."""
     assert cli.main(["-d", "tests/fixtures/code.py", "-z", "exit_with", "-Z", "1"]) == 1
 
 
-def test_options_precedence():
+def test_options_precedence() -> None:
     """Test options precedence."""
     # @duty(nofail=True) is overridden by ctx.run(nofail=False)
     assert cli.main(["-d", "tests/fixtures/precedence.py", "precedence"]) == 1
 
     # ctx.run(nofail=False) is overridden by local option -z
     assert cli.main(["-d", "tests/fixtures/precedence.py", "precedence", "-z"]) == 0
 
@@ -189,25 +191,25 @@
         ("zero=true", 0),
         ("zero=TRUE", 0),
         ("zero=anything else", 0),
         ("zero=-1", 0),
         ("zero=1", 0),
     ],
 )
-def test_cast_bool_parameter(param, expected):
+def test_cast_bool_parameter(param: str, expected: int) -> None:
     """Test parameters casting as boolean.
 
     Parameters:
         param: Pytest parametrization fixture.
         expected: Pytest parametrization fixture.
     """
     assert cli.main(["-d", "tests/fixtures/booleans.py", "boolean", param]) == expected
 
 
-def test_invalid_params(capsys):
+def test_invalid_params(capsys: pytest.CaptureFixture) -> None:
     """Check that invalid parameters are early and correctly detected.
 
     Parameters:
         capsys: Pytest fixture to capture output.
     """
     assert cli.main(["-d", "tests/fixtures/booleans.py", "boolean", "zore=off"]) == 1
     captured = capsys.readouterr()
```

### Comparing `duty-0.9.0/tests/test_collection.py` & `duty-1.0.0/tests/test_collection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 """Tests for the `collection` module."""
 
+from __future__ import annotations
+
 import pytest
 
 from duty.collection import Collection, Duty
 from duty.decorator import duty as decorate
 
 
-def none(*args, **kwargs):  # noqa: ARG001,D103
+def none(*args, **kwargs) -> None:  # noqa: ANN002, ANN003, ARG001, D103
     ...  # pragma: no cover
 
 
-def test_instantiate_duty():
+def test_instantiate_duty() -> None:
     """Instantiate a duty."""
     assert Duty("name", "description", none)
-    assert Duty("name", "description", none, pre=[0, 1], post=[2])
+    assert Duty("name", "description", none, pre=["0", "1"], post=["2"])
 
 
-def test_dont_get_duty():
+def test_dont_get_duty() -> None:
     """Don't find a duty."""
     collection = Collection()
     with pytest.raises(KeyError):
         collection.get("hello")
 
 
-def test_register_aliases():
+def test_register_aliases() -> None:
     """Register a duty and its aliases."""
-    duty = decorate(none, name="hello", aliases=["HELLO", "_hello_", ".hello."])
+    duty = decorate(none, name="hello", aliases=["HELLO", "_hello_", ".hello."])  # type: ignore[call-overload]
     collection = Collection()
     collection.add(duty)
     assert collection.get("hello")
     assert collection.get("HELLO")
     assert collection.get("_hello_")
     assert collection.get(".hello.")
 
 
-def test_replace_name_and_set_alias():
+def test_replace_name_and_set_alias() -> None:
     """Replace underscores by dashes in duties names."""
     collection = Collection()
-    collection.add(decorate(none, name="snake_case"))
+    collection.add(decorate(none, name="snake_case"))  # type: ignore[call-overload]
     assert collection.get("snake_case") is collection.get("snake-case")
 
 
-def test_clear_collection():
+def test_clear_collection() -> None:
     """Check that duties and their aliases are correctly cleared from a collection."""
     collection = Collection()
-    collection.add(decorate(none, name="duty_1"))
+    collection.add(decorate(none, name="duty_1"))  # type: ignore[call-overload]
     collection.clear()
     with pytest.raises(KeyError):
         collection.get("duty-1")
 
 
-def test_add_duty_to_multiple_collections():
+def test_add_duty_to_multiple_collections() -> None:
     """Check what happens when adding the same duty to multiple collections."""
     collection1 = Collection()
     collection2 = Collection()
 
-    duty = decorate(none, name="duty")
+    duty = decorate(none, name="duty")  # type: ignore[call-overload]
 
     collection1.add(duty)
     collection2.add(duty)
 
     duty1 = collection1.get("duty")
     duty2 = collection2.get("duty")
```

### Comparing `duty-0.9.0/tests/test_context.py` & `duty-1.0.0/tests/test_context.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 """Tests for the `context` module."""
 
+from __future__ import annotations
+
 from collections import namedtuple
 from pathlib import Path
 
 import pytest
 
 from duty import context
 from duty.exceptions import DutyFailure
 
 RunResult = namedtuple("RunResult", "code output")
 
 
-def test_allow_overrides(monkeypatch):
+def test_allow_overrides(monkeypatch: pytest.MonkeyPatch) -> None:
     """Test the `allow_overrides` option.
 
     Parameters:
         monkeypatch: A Pytest fixture to monkeypatch objects.
     """
     ctx = context.Context({"a": 1}, {"a": 2})
     records = []
-    monkeypatch.setattr(context, "failprint_run", lambda _, **opts: RunResult(records.append(opts), ""))
+    monkeypatch.setattr(context, "failprint_run", lambda _, **opts: RunResult(records.append(opts), ""))  # type: ignore[func-returns-value]
     ctx.run("")
     ctx.run("", allow_overrides=False)
     ctx.run("", allow_overrides=True)
     ctx.run("", allow_overrides=False, a=3)
     assert records[0]["a"] == 2
     assert records[1]["a"] == 1
     assert records[2]["a"] == 2
     assert records[3]["a"] == 3
 
 
-def test_options_context_manager(monkeypatch):
+def test_options_context_manager(monkeypatch: pytest.MonkeyPatch) -> None:
     """Test changing options using the context manager.
 
     Parameters:
         monkeypatch: A Pytest fixture to monkeypatch objects.
     """
     ctx = context.Context({"a": 1}, {"a": 2})
     records = []
-    monkeypatch.setattr(context, "failprint_run", lambda _, **opts: RunResult(records.append(opts), ""))
+    monkeypatch.setattr(context, "failprint_run", lambda _, **opts: RunResult(records.append(opts), ""))  # type: ignore[func-returns-value]
 
     with ctx.options(a=3):
         ctx.run("")  # should be overridden by 2
         with ctx.options(a=4, allow_overrides=False):
             ctx.run("")  # should be 4
             ctx.run("", allow_overrides=True)  # should be 2
         ctx.run("", allow_overrides=False)  # should be 3
 
     assert records[0]["a"] == 2
     assert records[1]["a"] == 4
     assert records[2]["a"] == 2
     assert records[3]["a"] == 3
 
 
-def test_workdir(monkeypatch):
+def test_workdir(monkeypatch: pytest.MonkeyPatch) -> None:
     """Test the `workdir` option.
 
     Parameters:
         monkeypatch: A Pytest fixture to monkeypatch objects.
     """
     ctx = context.Context({})
     monkeypatch.setattr(context, "failprint_run", lambda _: RunResult(len(Path.cwd().parts), ""))
@@ -67,15 +69,15 @@
     records.append(failure.value.code)
     with pytest.raises(DutyFailure) as failure:
         ctx.run("", workdir="..")
     records.append(failure.value.code)
     assert records[0] == records[1] + 1
 
 
-def test_workdir_as_context_manager(monkeypatch):
+def test_workdir_as_context_manager(monkeypatch: pytest.MonkeyPatch) -> None:
     """Test the `workdir` option as a context manager, and the `cd` context manager.
 
     Parameters:
         monkeypatch: A Pytest fixture to monkeypatch objects.
     """
     ctx = context.Context({})
     monkeypatch.setattr(context, "failprint_run", lambda _: RunResult(len(Path.cwd().parts), ""))
```

### Comparing `duty-0.9.0/tests/test_running.py` & `duty-1.0.0/tests/test_running.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 """Tests about running duties."""
 
+from __future__ import annotations
+
+from typing import NoReturn
 from unittest.mock import NonCallableMock
 
 import pytest
 
 from duty.collection import Collection, Duty
 from duty.decorator import duty as decorate
 from duty.exceptions import DutyFailure
 
 INTERRUPT_CODE = 130
 
 
-def test_run_duty():
+def test_run_duty() -> None:
     """Run a duty."""
-    duty = Duty("name", "description", lambda ctx: None)
-    assert duty.run() is None
-    assert duty(duty.context) is None
+    duty = Duty("name", "description", lambda ctx: 1)
+    assert duty.run() is None  # type: ignore[func-returns-value]
+    assert duty(duty.context) is None  # type: ignore[func-returns-value]
 
 
-def test_run_pre_post_duties_lambdas():
+def test_run_pre_post_duties_lambdas() -> None:
     """Run pre- and post- duties as lambdas."""
     pre_calls = []
     post_calls = []
 
     duty = Duty(
         "name",
         "description",
         lambda ctx: None,
-        pre=[lambda ctx: pre_calls.append(True)],  # noqa: FBT003
-        post=[lambda ctx: post_calls.append(True)],  # noqa: FBT003
+        pre=[lambda ctx: pre_calls.append(True)],
+        post=[lambda ctx: post_calls.append(True)],
     )
 
     duty.run()
 
     assert pre_calls[0] is True
     assert post_calls[0] is True
 
 
-def test_run_pre_post_duties_instances():
+def test_run_pre_post_duties_instances() -> None:
     """Run pre- and post- duties as duties."""
     pre_calls = []
     post_calls = []
 
-    pre_duty = Duty("pre", "", lambda ctx: pre_calls.append(True))  # noqa: FBT003
-    post_duty = Duty("post", "", lambda ctx: post_calls.append(True))  # noqa: FBT003
+    pre_duty = Duty("pre", "", lambda ctx: pre_calls.append(True))
+    post_duty = Duty("post", "", lambda ctx: post_calls.append(True))
 
     duty = Duty(
         name="name",
         description="description",
         function=lambda ctx: None,
         pre=[pre_duty],
         post=[post_duty],
@@ -55,57 +58,57 @@
 
     duty.run()
 
     assert pre_calls[0] is True
     assert post_calls[0] is True
 
 
-def test_run_pre_post_duties_refs():
+def test_run_pre_post_duties_refs() -> None:
     """Run pre- and post- duties as duties references."""
     pre_calls = []
     post_calls = []
 
     collection = Collection()
-    collection.add(decorate(lambda ctx: pre_calls.append(True), name="pre"))  # noqa: FBT003
-    collection.add(decorate(lambda ctx: post_calls.append(True), name="post"))  # noqa: FBT003
+    collection.add(decorate(lambda ctx: pre_calls.append(True), name="pre"))  # type: ignore[call-overload]
+    collection.add(decorate(lambda ctx: post_calls.append(True), name="post"))  # type: ignore[call-overload]
 
     duty = Duty("name", "description", lambda ctx: None, collection=collection, pre=["pre"], post=["post"])
     duty.run()
 
     assert pre_calls[0] is True
     assert post_calls[0] is True
 
 
-def test_dont_run_other_pre_post_duties():
+def test_dont_run_other_pre_post_duties() -> None:
     """Don't run other types of pre- and post- duties."""
     pre_duty = NonCallableMock()
     post_duty = NonCallableMock()
 
     duty = Duty("name", "description", lambda ctx: 0, pre=[pre_duty], post=[post_duty])
     duty.run()
 
     assert not pre_duty.called
     assert not post_duty.called
 
 
-def test_code_when_keyboard_interrupt():
+def test_code_when_keyboard_interrupt() -> None:
     """Return a code 130 on keyboard interruption."""
 
-    def interrupt():
+    def interrupt() -> NoReturn:
         raise KeyboardInterrupt
 
     with pytest.raises(DutyFailure) as excinfo:
         Duty("name", "description", lambda ctx: ctx.run(interrupt)).run()
     assert excinfo.value.code == INTERRUPT_CODE
 
 
-def test_dont_raise_duty_failure():
+def test_dont_raise_duty_failure() -> None:
     """Don't raise a duty failure on success."""
     duty = Duty("n", "d", lambda ctx: ctx.run(lambda: 0))
-    assert not duty.run()
+    assert not duty.run()  # type: ignore[func-returns-value]
 
 
-def test_cant_find_duty_without_collection():
+def test_cant_find_duty_without_collection() -> None:
     """Check that we can't find a duty with its name without a collection."""
-    duty = decorate(lambda ctx: None, name="duty1", post=["duty2"])
+    duty = decorate(lambda ctx: None, name="duty1", post=["duty2"])  # type: ignore[call-overload]
     with pytest.raises(RuntimeError):
         duty.run()
```

### Comparing `duty-0.9.0/PKG-INFO` & `duty-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: duty
-Version: 0.9.0
+Version: 1.0.0
 Summary: A simple task runner.
+Keywords: task-runner task runner cross-platform
+Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
-Keywords: task-runner,task,runner,cross-platform
-Author-email: Timothée Mazzucotelli <pawamoy@pm.me>
-Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
+Project-URL: Homepage, https://pawamoy.github.io/duty
+Project-URL: Documentation, https://pawamoy.github.io/duty
 Project-URL: Changelog, https://pawamoy.github.io/duty/changelog
+Project-URL: Repository, https://github.com/pawamoy/duty
+Project-URL: Issues, https://github.com/pawamoy/duty/issues
 Project-URL: Discussions, https://github.com/pawamoy/duty/discussions
-Project-URL: Documentation, https://pawamoy.github.io/duty
-Project-URL: Funding, https://github.com/sponsors/pawamoy
 Project-URL: Gitter, https://gitter.im/duty/community
-Project-URL: Homepage, https://pawamoy.github.io/duty
-Project-URL: Issues, https://github.com/pawamoy/duty/issues
-Project-URL: Repository, https://github.com/pawamoy/duty
+Project-URL: Funding, https://github.com/sponsors/pawamoy
+Requires-Python: >=3.8
+Requires-Dist: failprint>=0.11
 Description-Content-Type: text/markdown
 
 # duty
 
 [![ci](https://github.com/pawamoy/duty/workflows/ci/badge.svg)](https://github.com/pawamoy/duty/actions?query=workflow%3Aci)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://pawamoy.github.io/duty/)
 [![pypi version](https://img.shields.io/pypi/v/duty.svg)](https://pypi.org/project/duty/)
@@ -49,15 +49,15 @@
 With `pip`:
 ```bash
 pip install duty
 ```
 
 With [`pipx`](https://github.com/pipxproject/pipx):
 ```bash
-python3.7 -m pip install --user pipx
+python3.8 -m pip install --user pipx
 pipx install duty
 ```
 
 ## Quick start
 
 Create a `duties.py` file at the root of your repository.
 
@@ -74,7 +74,8 @@
 ```bash
 duty docs
 ```
 
 See the [Usage](https://pawamoy.github.io/duty/usage/)
 section in the documentation for more examples.
 
+Also see ["Why choosing duty over..."](https://pawamoy.github.io/duty/#why-duty-over).
```

