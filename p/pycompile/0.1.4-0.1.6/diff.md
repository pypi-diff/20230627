# Comparing `tmp/pycompile-0.1.4.tar.gz` & `tmp/pycompile-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompile-0.1.4.tar", max compression
+gzip compressed data, was "pycompile-0.1.6.tar", max compression
```

## Comparing `pycompile-0.1.4.tar` & `pycompile-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1074 2023-06-24 11:24:13.499420 pycompile-0.1.4/LICENSE
--rw-r--r--   0        0        0     2368 2023-06-24 11:24:13.499420 pycompile-0.1.4/README.md
--rw-r--r--   0        0        0     1233 2023-06-24 11:24:13.499420 pycompile-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      307 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/__init__.py
--rw-r--r--   0        0        0     3684 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/benchmark.py
--rw-r--r--   0        0        0     3039 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/cli.py
--rw-r--r--   0        0        0     2641 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/compiler_handler.py
--rw-r--r--   0        0        0        0 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/examples/__init__.py
--rw-r--r--   0        0        0      192 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/examples/fib.py
--rw-r--r--   0        0        0      254 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/examples/harmonic.py
--rw-r--r--   0        0        0      176 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/examples/sum.py
--rw-r--r--   0        0        0      144 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/examples/sum_of_sqaures.py
--rw-r--r--   0        0        0       99 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/examples/test_fib.py
--rw-r--r--   0        0        0      131 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/examples/test_harmonic_mean.py
--rw-r--r--   0        0        0       95 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/examples/test_sum.py
--rw-r--r--   0        0        0      131 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/examples/test_sum_of_sqaures.py
--rw-r--r--   0        0        0     4062 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/file_handler.py
--rw-r--r--   0        0        0     1194 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/helpers.py
--rw-r--r--   0        0        0     1341 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/logging_setup.py
--rw-r--r--   0        0        0     3209 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/wrappers.py
--rw-r--r--   0        0        0     3053 1970-01-01 00:00:00.000000 pycompile-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-27 15:15:48.888388 pycompile-0.1.6/LICENSE
+-rw-r--r--   0        0        0     9925 2023-06-27 15:15:48.892389 pycompile-0.1.6/README.md
+-rw-r--r--   0        0        0     1565 2023-06-27 15:15:48.900389 pycompile-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      307 2023-06-27 15:15:48.900389 pycompile-0.1.6/src/__init__.py
+-rw-r--r--   0        0        0     7131 2023-06-27 15:15:48.900389 pycompile-0.1.6/src/benchmark.py
+-rw-r--r--   0        0        0        0 2023-06-27 15:15:48.900389 pycompile-0.1.6/src/cli/__init__.py
+-rw-r--r--   0        0        0     2489 2023-06-27 15:15:48.900389 pycompile-0.1.6/src/cli/benchmark_cmd.py
+-rw-r--r--   0        0        0     2352 2023-06-27 15:15:48.900389 pycompile-0.1.6/src/cli/compile_cmd.py
+-rw-r--r--   0        0        0     1666 2023-06-27 15:15:48.900389 pycompile-0.1.6/src/cli/dry_run_cmd.py
+-rw-r--r--   0        0        0      693 2023-06-27 15:15:48.900389 pycompile-0.1.6/src/cli/entrypoint.py
+-rw-r--r--   0        0        0     2682 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/compiler_handler.py
+-rw-r--r--   0        0        0        0 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/examples/__init__.py
+-rw-r--r--   0        0        0      243 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/examples/examples_benchmark.py
+-rw-r--r--   0        0        0      145 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/examples/fib.py
+-rw-r--r--   0        0        0      128 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/examples/harmonic.py
+-rw-r--r--   0        0        0      441 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/examples/sum.py
+-rw-r--r--   0        0        0       97 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/examples/test_examples.py
+-rw-r--r--   0        0        0     4531 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/file_handler.py
+-rw-r--r--   0        0        0     2989 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/helpers.py
+-rw-r--r--   0        0        0     1341 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/logging_setup.py
+-rw-r--r--   0        0        0     3209 2023-06-27 15:15:48.904389 pycompile-0.1.6/src/wrappers.py
+-rw-r--r--   0        0        0    10660 1970-01-01 00:00:00.000000 pycompile-0.1.6/PKG-INFO
```

### Comparing `pycompile-0.1.4/LICENSE` & `pycompile-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.4/pyproject.toml` & `pycompile-0.1.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycompile"
-version = "0.1.4"
+version = "0.1.6"
 description = "A CLI tool for compiling python"
 authors = ["iplitharas <johnplitharas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "src" }
 ]
@@ -12,42 +12,54 @@
 [tool.poetry.dependencies]
 python = ">3.8"                       # MIT
 click = "^8.1.3"                      # BSD-3-Clause
 tqdm = "^4.64.1"                      # MIT
 cython = "^0.29.33"                   # Apache
 nuitka = "^1.4.8"                     # Apache 2.0
 pytest-benchmark = "^4.0.0"           # BSD-2-Clause
+memory-profiler = "^0.61.0"           # BSD
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"                    # MIT
 black = "^23.1.0"                    # MIT
 pylint = "^2.16.2"                   # GPL v2
 isort = "^5.12.0"                    # MIT
 pytest-cov = "^4.0.0"                # MIT
 pre-commit = "^3.1.0"                # MIT
 ipython = "^8.10.0"                  # BSD-3-Clause
+mypy = "^1.4.1"                      # MIT
+types-tqdm = "^4.65.0.1"             # Apache 2.0
+sphinx = "^7.0.1"                    # BSD
+furo = "^2023.5.20"                  # MIT
+myst-parser = "^2.0.0"               # MIT
 
 [build-system]
 requires = [ "setuptools", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-pycompile = "src.cli:main"
+pycompile = "src.cli.entrypoint:main"
 
 
 [tool.black]
 line-length = 80
-target-version = ["py38", "py39"]
+target-version = ["py310"]
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 line_length = 80
 skip = [".gitignore", ".dockerignore" ,".env"]
 
 
+[tool.mypy]
+python_version = "3.10"
+strict_optional = true
+
+
+
```

### Comparing `pycompile-0.1.4/src/cli.py` & `pycompile-0.1.6/src/cli/compile_cmd.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 """
-CLI entrypoint.
+Compile command
 """
 import logging
-import sys
 from pathlib import Path
 
 import click
 
 from src import (
     CompilerHandler,
     CythonWrapper,
     FileHandler,
     NuitkaWrapper,
     setup_logging,
 )
-from src.benchmark import Benchmark
-from src.helpers import Colors
 
 logger = logging.getLogger(__name__)
 
 
-@click.command()
+@click.command(name="compile")
 @click.option(
     "-i",
     "--input-path",
-    required=False,
+    required=True,
     type=click.Path(exists=True),
     help="Specify the file/folder input path, "
     "by default it will exclude any `test` and `__init__.py` files",
 )
 @click.option(
     "-ex",
     "--exclude-glob-paths",
     required=False,
     multiple=True,
     type=str,
-    default=FileHandler(".").exclude_patterns,
+    default=FileHandler("..").exclude_patterns,  # type: ignore[arg-type]
     help="glob files patterns of the files to be excluded, example: **/ignore_this_module.py",
 )
 @click.option("-v", "--verbose", count=True, help="verbose level")
 @click.option(
     "-e",
     "--engine",
     default="cython",
@@ -66,57 +63,32 @@
     "-ce",
     "--clean-executables",
     "clean_executables",
     flag_value=True,
     default=False,
     help="Clean final executables (.so) files",
 )
-@click.option(
-    "-b",
-    "--benchmark",
-    required=False,
-    flag_value=True,
-    default=False,
-    help="Benchmark the examples.",
-)
-def main(  # pylint: disable=too-many-arguments
+def compile_cmd(  # pylint: disable=R0913
     input_path: Path,
     exclude_glob_paths: list[str],
     verbose,
     engine: str,
     clean_source: bool,
     keep_builds: bool,
     clean_executables: bool,
-    benchmark: bool,
 ):
-    r"""
-                                          _ _
-    _ __  _   _  ___ ___  _ __ ___  _ __ (_) | ___
-   | '_ \| | | |/ __/ _ \| '_ ` _ \| '_ \| | |/ _ \
-   | |_) | |_| | (_| (_) | | | | | | |_) | | |  __/
-   | .__/ \__, |\___\___/|_| |_| |_| .__/|_|_|\___|
-   |_|    |___/                    |_|
-   """
+    """
+    Compile the python files using `cython` or `nuitka`.
+    """
     setup_logging(verbose)
-    if benchmark:
-        bench = Benchmark()
-        bench.start()
-        sys.exit(0)
-
-    if not input_path:
-        logger.error(
-            "%s Input path is missing, exiting...%s", Colors.FAIL, Colors.RESET
-        )
-        sys.exit(1)
 
     dir_files = FileHandler(
         input_path=input_path,
         additional_exclude_patterns=exclude_glob_paths,
     ).start()
-
     if dir_files:
         compiler = (
             CythonWrapper() if engine.lower() == "cython" else NuitkaWrapper()
         )
         compiler_handler = CompilerHandler(
             files=dir_files,
             compiler=compiler,
```

### Comparing `pycompile-0.1.4/src/compiler_handler.py` & `pycompile-0.1.6/src/compiler_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,24 +16,49 @@
     """
      CompilerHandler is responsible for compiling all the `.py` files using
     `Cython` or `Nuitka`
     """
 
     def __init__(
         self,
-        files: dict[str : list[Path]],
+        files: dict[str, list[Path]],
         compiler: CompilerWrapper,
         clean_source: bool = False,
         keep_builds: bool = True,
     ):
         self.files = files
         self.compiler = compiler
         self.clean_source = clean_source
         self.keep_builds = keep_builds
 
+    @staticmethod
+    def _clean_source_files(files: list[Path]) -> None:
+        """
+        Cleans the `source` files.
+        """
+        deleted = [file.unlink() for file in files]  # type: ignore[func-returns-value]
+        logger.warning(
+            "%sFlag `--clean-source` is on, deleted " f"#{len(deleted)}" "%s",
+            Colors.CYAN,
+            Colors.RESET,
+        )
+
+    def _clean_build_files(self, files: list[Path]) -> None:
+        """
+        Cleans the temporary `build` files.
+        """
+        for file in files:
+            self.compiler.cleanup(file_path=file)
+        logger.warning(
+            "%s Flag `-keep-builds` is off, all temp build files are deleted.."
+            "%s",
+            Colors.CYAN,
+            Colors.RESET,
+        )
+
     def clean_executables(self) -> None:
         """
         Cleans all the `.so` files.
         """
         for directory, _ in self.files.items():
             for executable in Path(directory).glob(pattern="*.so"):
                 executable.unlink(missing_ok=True)
@@ -47,42 +72,17 @@
         for directory, dir_files in tqdm(
             self.files.items(),
             total=total_iterations,
             ascii=True,
             desc=f"{Colors.CYAN}Compiling using: `{self.compiler}`{Colors.RESET}",
             dynamic_ncols=True,
         ):
-            with change_dir(directory):
+            with change_dir(Path(directory)):
                 try:
                     run_sub_process(
                         files=dir_files, compile_cmd=self.compiler.cmd
                     )
                 finally:
                     if not self.keep_builds:
                         self._clean_build_files(files=dir_files)
                     if self.clean_source:
                         self._clean_source_files(files=dir_files)
-
-    @staticmethod
-    def _clean_source_files(files: list[Path]) -> None:
-        """
-        Cleans the `source` files.
-        """
-        deleted = [file.unlink() for file in files]
-        logger.warning(
-            "%sFlag `--clean-source` is on, deleted " f"#{len(deleted)}" "%s",
-            Colors.CYAN,
-            Colors.RESET,
-        )
-
-    def _clean_build_files(self, files: list[Path]) -> None:
-        """
-        Cleans the temporary `build` files.
-        """
-        for file in files:
-            self.compiler.cleanup(file_path=file)
-        logger.warning(
-            "%s Flag `-keep-builds` is off, all temp build files are deleted.."
-            "%s",
-            Colors.CYAN,
-            Colors.RESET,
-        )
```

### Comparing `pycompile-0.1.4/src/file_handler.py` & `pycompile-0.1.6/src/file_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
                          that fall under the current directory.
                  `*` :   On Unix, will match everything except slashes.
                          On Windows, it will avoid matching backslashes as well as slashes.
 """
 import logging
 from collections import defaultdict
 from pathlib import Path
-from typing import Generator
+from typing import Generator, Optional
 
 from src.helpers import Colors
 
 logger = logging.getLogger(__name__)
 
 
 class FileHandler:
@@ -21,16 +21,16 @@
     FileHandler is responsible for finding all the `.py` files  given
     any `input_path`.
     example usage: FileHandler("./my_module).start()
     """
 
     def __init__(
         self,
-        input_path: Path | str,
-        additional_exclude_patterns: list[str] = None,
+        input_path: Path,
+        additional_exclude_patterns: Optional[list[str]] = None,
     ):
         """
         By default, all the `test` files and any `__init__` files are excluded
         :param `input_path`: Should be a valid file/directory path.
         :param `additional_exclude_patterns`: Any optional additional glob patterns.
         """
         self.input_path = input_path
@@ -63,21 +63,22 @@
             "**/test**",
             "**/__init__.py",
         ]
 
         if additional_exclude_patterns:
             self._exclude_patterns.extend(additional_exclude_patterns)
 
-    def start(self) -> dict[str : list[Path]]:
+    def start(self) -> dict[str, list[Path]]:
         """
-        For the given `input path` collect all valid `.py` files.
+        For the given `input path` collect all valid `.py` files based on
+        the `exclude_patterns`
         :return: a dictionary for valid files within each directory.
         """
 
-        files = defaultdict(list[Path])
+        files = defaultdict(list[Path])  # type: ignore[var-annotated]
         excluded_files = list(self._filter_files())
         logger.debug(
             "%sExcluded files: %s%s",
             Colors.CYAN,
             Colors.RESET,
             [
                 excluded_file.name
@@ -88,15 +89,15 @@
 
         for file in self._collect_files():
             if file not in excluded_files:
                 files[str(file.resolve().parent)].append(file.resolve())
 
         return files
 
-    def _filter_files(self) -> Generator[Path, None, None]:
+    def _filter_files(self) -> Generator[Optional[Path], None, None]:
         """
         Collects all files to be excluded for the given `input path`
         using the `exclude_patterns` glob patterns.
         """
         if not self.input_path.is_dir():
             yield None
         yield from (
@@ -116,14 +117,27 @@
         else:
             for sub_dir in self.input_path.iterdir():
                 if sub_dir.is_dir():
                     yield from sub_dir.rglob(pattern="**/*.py")
 
             yield from self.input_path.glob(pattern="*.py")
 
+    def collect_with_pattern(self, pattern: str):
+        """
+        Collects all python files from the `input_path` where they mach
+        the `pattern`
+
+        """
+        if not self.input_path.is_dir():
+            yield self.input_path
+        else:
+            yield from (
+                file for file in self._collect_files() if file.match(pattern)
+            )
+
     def __str__(self) -> str:
         return (
             f"FileHandler\n"
             f"Input path: {self.input_path}\n"
             f"Exclude glob patters: {self.exclude_patterns}\n"
         )
```

### Comparing `pycompile-0.1.4/src/logging_setup.py` & `pycompile-0.1.6/src/logging_setup.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.4/src/wrappers.py` & `pycompile-0.1.6/src/wrappers.py`

 * *Files identical despite different names*

