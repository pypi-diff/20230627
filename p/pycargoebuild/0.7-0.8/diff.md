# Comparing `tmp/pycargoebuild-0.7.tar.gz` & `tmp/pycargoebuild-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycargoebuild-0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pycargoebuild-0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pycargoebuild-0.7.tar` & `pycargoebuild-0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1081 2022-11-09 09:31:36.847189 pycargoebuild-0.7/LICENSE
--rw-r--r--   0        0        0     2304 2022-12-11 16:55:26.062005 pycargoebuild-0.7/README.rst
--rw-r--r--   0        0        0       80 2023-06-18 14:57:52.100741 pycargoebuild-0.7/pycargoebuild/__init__.py
--rw-r--r--   0        0        0     8525 2023-06-18 14:25:48.715463 pycargoebuild-0.7/pycargoebuild/__main__.py
--rw-r--r--   0        0        0     3253 2023-06-18 14:37:33.218459 pycargoebuild-0.7/pycargoebuild/cargo.py
--rw-r--r--   0        0        0     6899 2023-06-18 14:43:47.326364 pycargoebuild-0.7/pycargoebuild/ebuild.py
--rw-r--r--   0        0        0     2272 2023-02-06 04:03:59.321434 pycargoebuild-0.7/pycargoebuild/fetch.py
--rw-r--r--   0        0        0     4645 2022-11-25 16:23:06.667384 pycargoebuild-0.7/pycargoebuild/format.py
--rw-r--r--   0        0        0     3541 2022-11-22 19:20:48.996065 pycargoebuild-0.7/pycargoebuild/license.py
--rw-r--r--   0        0        0     1126 2022-11-13 11:10:20.163896 pycargoebuild-0.7/pyproject.toml
--rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 pycargoebuild-0.7/PKG-INFO
+-rw-r--r--   0        0        0     1081 2022-11-09 09:31:36.847189 pycargoebuild-0.8/LICENSE
+-rw-r--r--   0        0        0     2304 2022-12-11 16:55:26.062005 pycargoebuild-0.8/README.rst
+-rw-r--r--   0        0        0       80 2023-06-27 14:55:13.160950 pycargoebuild-0.8/pycargoebuild/__init__.py
+-rw-r--r--   0        0        0     8537 2023-06-27 14:22:16.094695 pycargoebuild-0.8/pycargoebuild/__main__.py
+-rw-r--r--   0        0        0     6157 2023-06-27 13:32:53.404842 pycargoebuild-0.8/pycargoebuild/cargo.py
+-rw-r--r--   0        0        0     8866 2023-06-27 14:54:19.329899 pycargoebuild-0.8/pycargoebuild/ebuild.py
+-rw-r--r--   0        0        0     2572 2023-06-26 17:49:46.447413 pycargoebuild-0.8/pycargoebuild/fetch.py
+-rw-r--r--   0        0        0     4645 2022-11-25 16:23:06.667384 pycargoebuild-0.8/pycargoebuild/format.py
+-rw-r--r--   0        0        0     3541 2022-11-22 19:20:48.996065 pycargoebuild-0.8/pycargoebuild/license.py
+-rw-r--r--   0        0        0     1126 2023-06-27 14:09:19.035713 pycargoebuild-0.8/pyproject.toml
+-rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 pycargoebuild-0.8/PKG-INFO
```

### Comparing `pycargoebuild-0.7/LICENSE` & `pycargoebuild-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pycargoebuild-0.7/README.rst` & `pycargoebuild-0.8/README.rst`

 * *Files identical despite different names*

### Comparing `pycargoebuild-0.7/pycargoebuild/__main__.py` & `pycargoebuild-0.8/pycargoebuild/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,16 +158,16 @@
     if args.input is not None:
         ebuild = update_ebuild(args.input.read(),
                                pkg_meta,
                                crates,
                                distdir=args.distdir,
                                crate_license=not args.no_license)
         logging.warning(
-            "The in-place mode updates CRATES and crate LICENSE+= variables "
-            "only, other metadata is left unchanged")
+            "The in-place mode updates CRATES, GIT_CRATES and crate "
+            "LICENSE+= variables only, other metadata is left unchanged")
     else:
         ebuild = get_ebuild(pkg_meta,
                             crates,
                             distdir=args.distdir,
                             crate_license=not args.no_license)
 
     try:
```

### Comparing `pycargoebuild-0.7/pycargoebuild/ebuild.py` & `pycargoebuild-0.8/pycargoebuild/ebuild.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 import datetime
 import logging
 import re
+import shlex
 import tarfile
 import typing
 import urllib.parse
 
 from functools import partial
 from pathlib import Path
 
 import license_expression
 
 from pycargoebuild import __version__
-from pycargoebuild.cargo import Crate, PackageMetadata, get_package_metadata
+from pycargoebuild.cargo import (Crate,
+                                 FileCrate,
+                                 GitCrate,
+                                 PackageMetadata,
+                                 get_package_metadata,
+                                 )
 from pycargoebuild.format import format_license_var
 from pycargoebuild.license import spdx_to_ebuild
 
 
 EBUILD_TEMPLATE_START = """\
 # Copyright {year} Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 # Autogenerated by pycargoebuild {prog_version}
 
 EAPI=8
 
-CRATES="{crates}"
+CRATES="{crates}"{opt_git_crates}
 
 inherit cargo
 
 DESCRIPTION="{description}"
 HOMEPAGE="{homepage}"
 SRC_URI="
 \t${{CARGO_CRATE_URIS}}
@@ -51,66 +57,89 @@
 def get_CRATES(crates: typing.Iterable[Crate]) -> str:
     """
     Return the value of CRATES for the given crate list
     """
     if not crates:
         return ""
     return ("\n" +
-            "\n".join(sorted(f"\t{c.crate_entry}" for c in crates)) +
+            "\n".join(sorted(f"\t{c.crate_entry}"
+                             for c in crates
+                             if isinstance(c, FileCrate))) +
             "\n")
 
 
+def get_GIT_CRATES(crates: typing.Iterable[Crate],
+                   distdir: Path,
+                   ) -> str:
+    """
+    Return the complete GIT_CRATES assignment for the given crate list
+    """
+
+    values = "\n".join(
+        sorted(f"\t[{c.name}]={shlex.quote(c.get_git_crate_entry(distdir))}"
+               for c in crates if isinstance(c, GitCrate)))
+    if values:
+        return f"\n\ndeclare -A GIT_CRATES=(\n{values}\n)"
+    return ""
+
+
 def get_package_LICENSE(pkg_meta: PackageMetadata) -> str:
     """
     Get the value of package's LICENSE string
     """
 
     spdx = license_expression.get_spdx_licensing()
     if pkg_meta.license is not None:
         parsed_pkg_license = spdx.parse(pkg_meta.license,
                                         strict=True)
         return format_license_var(spdx_to_ebuild(parsed_pkg_license),
                                   prefix='LICENSE="')
     return ""
 
 
-def get_license_from_crate(path: Path) -> typing.Optional[str]:
+def get_license_from_crate(crate: Crate,
+                           distdir: Path,
+                           ) -> typing.Optional[str]:
     """
     Read the metadata from specified crate and return its license string
     """
 
-    assert path.name.endswith(".crate")
-    with tarfile.open(path, "r:gz") as crate:
-        tarf = crate.extractfile(f"{path.name[:-6]}/Cargo.toml")
+    filename = crate.filename
+    with tarfile.open(distdir / filename, "r:gz") as crate_tar:
+        tarf = crate_tar.extractfile(
+            str(crate.get_package_directory(distdir) / "Cargo.toml"))
         if tarf is None:
-            raise RuntimeError(f"Cargo.toml not found in {path}")
+            raise RuntimeError(f"Cargo.toml not found in {filename}")
         with tarf:
             # tarfile.ExFileObject() is IO[bytes] while tomli/tomllib
             # expects BinaryIO -- but it actually is compatible
             # https://github.com/hukkin/tomli/issues/214
             crate_metadata = get_package_metadata(tarf)  # type: ignore
             if crate_metadata.license_file is not None:
                 logging.warning(
-                    f"Crate {path.name} uses license-file="
+                    f"Crate {filename} uses license-file="
                     f"{crate_metadata.license_file!r}, please inspect "
                     "the license manually and add it *separately* from crate "
                     "licenses")
             elif crate_metadata.license is None:
                 raise RuntimeError(
-                    f"Crate {path.name} does not specify a license!")
+                    f"Crate {filename} does not specify a license!")
             return crate_metadata.license
 
 
-def get_crate_LICENSE(crate_files: typing.Iterable[Path]) -> str:
+def get_crate_LICENSE(crates: typing.Iterable[Crate],
+                      distdir: Path,
+                      ) -> str:
     """
     Get the value of LICENSE string for crates
     """
 
     spdx = license_expression.get_spdx_licensing()
-    crate_licenses = set(map(get_license_from_crate, crate_files))
+    crate_licenses = set(get_license_from_crate(crate, distdir)
+                         for crate in crates)
     crate_licenses.discard(None)
 
     # combine crate licenses and simplify the result
     combined_license = " AND ".join(f"( {x} )" for x in crate_licenses)
     parsed_license = spdx.parse(combined_license, strict=True)
     if parsed_license is None:
         return ""
@@ -154,35 +183,43 @@
     """
 
     template = EBUILD_TEMPLATE_START
     if crate_license:
         template += EBUILD_TEMPLATE_CRATE_LICENSE
     template += EBUILD_TEMPLATE_END
 
-    crate_files = [distdir / crate.filename for crate in crates]
     return template.format(
         crates=get_CRATES(crates),
-        crate_licenses=get_crate_LICENSE(crate_files),
+        crate_licenses=get_crate_LICENSE(crates, distdir),
         description=bash_dquote_escape(collapse_whitespace(
             pkg_meta.description or "")),
         homepage=url_dquote_escape(pkg_meta.homepage or ""),
+        opt_git_crates=get_GIT_CRATES(crates, distdir),
         pkg_license=get_package_LICENSE(pkg_meta),
         prog_version=__version__,
         year=datetime.date.today().year)
 
 
 CRATES_RE = re.compile(
     r"^(?P<start>CRATES=(?P<delim>['\"])).*?(?P=delim)$",
     re.DOTALL | re.MULTILINE)
 
+GIT_CRATES_RE = re.compile(
+    r"(?P<ws>\n\n?)declare -A GIT_CRATES=[(].*?[)]$",
+    re.DOTALL | re.MULTILINE)
+
 CRATE_LICENSE_RE = re.compile(
     r"^(?P<start># Dependent crate licenses\n"
     r"LICENSE[+]=(?P<delim>['\"])).*?(?P=delim)$",
     re.DOTALL | re.MULTILINE)
 
+GIT_CRATES_APPEND_RE = re.compile(
+    r"^(?P<start>CRATES=(?P<delim2>['\"]).*?(?P=delim2))(?P<delim>)$",
+    re.DOTALL | re.MULTILINE)
+
 
 class CountingSubst:
     def __init__(self, repl: typing.Callable[[], str]
                  ) -> None:
         self.count = 0
         self.repl = repl
 
@@ -192,30 +229,50 @@
 
     def assert_count(self, desc: str, expected: int) -> None:
         if self.count != expected:
             raise RuntimeError(
                 f"{desc} matched {self.count} times, {expected} expected")
 
 
+class GitCratesSubst(CountingSubst):
+    def __call__(self, match: re.Match) -> str:
+        self.count += 1
+        if repl := self.repl().lstrip():
+            return match.group("ws") + repl
+        return ""
+
+
 def update_ebuild(ebuild: str,
                   pkg_meta: PackageMetadata,
                   crates: typing.Iterable[Crate],
                   distdir: Path,
                   *,
                   crate_license: bool = True,
                   ) -> str:
     """
-    Update the CRATES and LICENSE in an existing ebuild
+    Update the CRATES, GIT_CRATES and LICENSE in an existing ebuild
     """
 
-    crate_files = [distdir / crate.filename for crate in crates]
     crates_repl = CountingSubst(partial(get_CRATES, crates))
-    crate_license_repl = CountingSubst(partial(get_crate_LICENSE, crate_files))
-
-    ebuild = CRATE_LICENSE_RE.sub(crate_license_repl,
-                                  CRATES_RE.sub(crates_repl, ebuild))
+    git_crates_repl = GitCratesSubst(partial(get_GIT_CRATES, crates, distdir))
+    crate_license_repl = (
+        CountingSubst(partial(get_crate_LICENSE, crates, distdir)))
+
+    for regex, repl in ((CRATES_RE, crates_repl),
+                        (GIT_CRATES_RE, git_crates_repl),
+                        (CRATE_LICENSE_RE, crate_license_repl)):
+        ebuild = regex.sub(repl, ebuild)
 
     crates_repl.assert_count("CRATES=", 1)
     crate_license_repl.assert_count(
         "Crate LICENSE+= (with marker comment)", 1 if crate_license else 0)
 
+    if git_crates_repl.count == 0:
+        if git_crates := git_crates_repl.repl():
+            git_crates_append = CountingSubst(lambda: git_crates)
+            ebuild = GIT_CRATES_APPEND_RE.sub(git_crates_append, ebuild)
+            git_crates_append.assert_count(
+                "CRATES= (while appending GIT_CRATES=)", 1)
+    else:
+        git_crates_repl.assert_count("GIT_CRATES=", 1)
+
     return ebuild
```

### Comparing `pycargoebuild-0.7/pycargoebuild/fetch.py` & `pycargoebuild-0.8/pycargoebuild/fetch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 import hashlib
 import subprocess
 import sys
+import tempfile
 import typing
 
 from pathlib import Path
 
-from pycargoebuild.cargo import Crate
+from pycargoebuild.cargo import Crate, FileCrate
 
 
 def fetch_crates_using_aria2(crates: typing.Iterable[Crate], *, distdir: Path
                              ) -> None:
     """
     Fetch specified crates into distdir using aria2c(1)
     """
 
     distdir.mkdir(parents=True, exist_ok=True)
-    crate_urls = [crate.crates_io_url
-                  for crate in crates
-                  if not (distdir / crate.filename).exists()]
-    if crate_urls:
+    with tempfile.NamedTemporaryFile("w+") as file_list_f:
+        for crate in crates:
+            if not (distdir / crate.filename).exists():
+                file_list_f.write(
+                    f"{crate.download_url}\n\tout={crate.filename}\n")
+
+        if file_list_f.tell() == 0:
+            # no crates to fetch
+            return
+
+        file_list_f.flush()
+
         subprocess.check_call(
-            ["aria2c", "-Z", "-d", str(distdir)] + crate_urls,
+            ["aria2c", "-d", str(distdir), "-i", file_list_f.name],
             stdout=sys.stderr)
 
 
 def fetch_files_using_wget(files: typing.Iterable[typing.Tuple[str, Path]]
                            ) -> None:
     """
     Fetch specified URLs to the specified filenames using wget(1)
@@ -41,15 +50,15 @@
                             ) -> None:
     """
     Fetch specified crates into distdir using wget(1)
     """
 
     distdir.mkdir(parents=True, exist_ok=True)
     fetch_files_using_wget(
-        (crate.crates_io_url, distdir / crate.filename) for crate in crates)
+        (crate.download_url, distdir / crate.filename) for crate in crates)
 
 
 def verify_files(files: typing.Iterable[typing.Tuple[Path, str]]) -> None:
     """
     Verify checksums of specified files
     """
 
@@ -70,9 +79,10 @@
 
 
 def verify_crates(crates: typing.Iterable[Crate], *, distdir: Path) -> None:
     """
     Verify checksums of crates fetched into distdir
     """
 
-    verify_files(
-        (distdir / crate.filename, crate.checksum) for crate in crates)
+    verify_files((distdir / crate.filename, crate.checksum)
+                 for crate in crates
+                 if isinstance(crate, FileCrate))
```

### Comparing `pycargoebuild-0.7/pycargoebuild/format.py` & `pycargoebuild-0.8/pycargoebuild/format.py`

 * *Files identical despite different names*

### Comparing `pycargoebuild-0.7/pycargoebuild/license.py` & `pycargoebuild-0.8/pycargoebuild/license.py`

 * *Files identical despite different names*

### Comparing `pycargoebuild-0.7/pyproject.toml` & `pycargoebuild-0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "pycargoebuild"
 authors = [{name = "Michał Górny", email = "mgorny@gentoo.org"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 readme = "README.rst"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 dependencies = [
     "license_expression",
     "tomli >= 1.2.3; python_version < '3.11'",
 ]
 
 [project.optional-dependencies]
 pretty-log = ["rich"]
```

### Comparing `pycargoebuild-0.7/PKG-INFO` & `pycargoebuild-0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pycargoebuild
-Version: 0.7
+Version: 0.8
 Summary: A generator for Rust/Cargo ebuilds written in Python
 Author-email: Michał Górny <mgorny@gentoo.org>
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: license_expression
 Requires-Dist: tomli >= 1.2.3; python_version < '3.11'
 Requires-Dist: rich ; extra == "pretty-log"
 Requires-Dist: pytest ; extra == "test"
 Project-URL: Homepage, https://github.com/projg2/pycargoebuild/
```

