# Comparing `tmp/pdm-autoexport-0.1.1.tar.gz` & `tmp/pdm_autoexport-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-autoexport-0.1.1.tar", last modified: Wed Jul 27 10:17:26 2022, max compression
+gzip compressed data, was "pdm_autoexport-0.2.0.tar", last modified: Tue Jun 27 03:27:05 2023, max compression
```

## Comparing `pdm-autoexport-0.1.1.tar` & `pdm_autoexport-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-07-27 10:17:12.437215 pdm-autoexport-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-07-27 10:17:12.437215 pdm-autoexport-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-07-27 10:17:12.437215 pdm-autoexport-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-07-27 10:17:12.437215 pdm-autoexport-0.1.1/src/pdm_autoexport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1959 2022-07-27 10:17:12.437215 pdm-autoexport-0.1.1/src/pdm_autoexport/hook.py
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-07-27 10:17:12.437215 pdm-autoexport-0.1.1/tests/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-07-27 10:17:12.437215 pdm-autoexport-0.1.1/tests/test_autoexport.py
--rw-------   0 runner    (1001) docker     (121)     2245 2022-07-27 10:17:26.445732 pdm-autoexport-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-27 03:26:50.357078 pdm_autoexport-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1521 2023-06-27 03:26:50.357078 pdm_autoexport-0.2.0/README.md
+-rw-r--r--   0        0        0     1044 2023-06-27 03:27:05.782246 pdm_autoexport-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      273 2023-06-27 03:26:50.357078 pdm_autoexport-0.2.0/src/pdm_autoexport/__init__.py
+-rw-r--r--   0        0        0     1962 2023-06-27 03:26:50.357078 pdm_autoexport-0.2.0/src/pdm_autoexport/hook.py
+-rw-r--r--   0        0        0      330 2023-06-27 03:26:50.357078 pdm_autoexport-0.2.0/tests/pyproject.toml
+-rw-r--r--   0        0        0     1280 2023-06-27 03:26:50.357078 pdm_autoexport-0.2.0/tests/test_autoexport.py
+-rw-r--r--   0        0        0     2244 1970-01-01 00:00:00.000000 pdm_autoexport-0.2.0/PKG-INFO
```

### Comparing `pdm-autoexport-0.1.1/LICENSE` & `pdm_autoexport-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-autoexport-0.1.1/README.md` & `pdm_autoexport-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pdm-autoexport-0.1.1/pyproject.toml` & `pdm_autoexport-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
 ]
-version = "0.1.1"
+version = "0.2.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/frostming/pdm-autoexport"
 Changelog = "https://github.com/frostming/pdm-autoexport/releases"
@@ -39,10 +39,10 @@
 test = [
     "pytest>=7.1.2",
     "pdm>=1.0.0",
 ]
 
 [build-system]
 requires = [
-    "pdm-pep517>=0.12.0",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
```

### Comparing `pdm-autoexport-0.1.1/src/pdm_autoexport/hook.py` & `pdm_autoexport-0.2.0/src/pdm_autoexport/hook.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 class ExportConfig:
     filename: str
     format: str = "requirements"
     groups: Iterable[str] = ("default",)
     without_hashes: bool = False
 
     def __post_init__(self):
-        if self.format not in ("requirements", "setuppy"):
+        if self.format not in ("requirements",):
             raise ValueError(
-                f"Unsupported format: {self.format}, must be requirements or setuppy"
+                f"Unsupported format: {self.format}, now only requirements is supported"
             )
         if not self.groups:
             raise ValueError("No groups specified")
 
 
 def export_config(project: Project) -> Iterable[ExportConfig]:
     """
     Load the auto-export config.
     """
-    tool_settings = project.tool_settings
+    tool_settings = project.pyproject.settings
     return (
         ExportConfig(
             filename=item["filename"],
             format=item.get("format", "requirements"),
             groups=item.get("groups", ["default"]),
             without_hashes=item.get("without-hashes", False),
         )
@@ -43,15 +43,15 @@
 def run_auto_export(project: Project, dry_run: bool, **kwargs: Any) -> None:
     """
     Run the auto-export hook.
     """
     if dry_run:
         return
     core = project.core
-    dev_groups = set(project.tool_settings.get("dev-dependencies", []))
+    dev_groups = set(project.pyproject.settings.get("dev-dependencies", []))
     for config in export_config(project):
         group_args = ["--no-default"]
         if dev_groups.isdisjoint(config.groups):
             group_args.append("--prod")
         for group in config.groups:
             group_args.extend(["--group", group])
         hash_args = ["--without-hashes"] if config.without_hashes else []
```

### Comparing `pdm-autoexport-0.1.1/tests/test_autoexport.py` & `pdm_autoexport-0.2.0/tests/test_autoexport.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 def test_pdm_autoexport(tmp_project: Project):
     tmp_project.core.main(["lock", "-v"], obj=tmp_project)
     requirements_txt = tmp_project.root.joinpath("requirements.txt").read_text()
     requirements_test_txt = tmp_project.root.joinpath(
         "requirements-test.txt"
     ).read_text()
-    setup_py = tmp_project.root.joinpath("setup.py").read_text()
     assert any(line.startswith("requests==") for line in requirements_txt.splitlines())
     assert any(line.startswith("urllib3==") for line in requirements_txt.splitlines())
     assert any(
         line.strip().startswith("--hash=") for line in requirements_txt.splitlines()
     )
     assert not any(
         line.startswith("requests==") for line in requirements_test_txt.splitlines()
@@ -33,8 +32,7 @@
     assert any(
         line.startswith("pytest==") for line in requirements_test_txt.splitlines()
     )
     assert not any(
         line.strip().startswith("--hash=")
         for line in requirements_test_txt.splitlines()
     )
-    assert any(line.strip().startswith("'requests'") for line in setup_py.splitlines())
```

### Comparing `pdm-autoexport-0.1.1/PKG-INFO` & `pdm_autoexport-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pdm-autoexport
-Version: 0.1.1
+Version: 0.2.0
 Summary: A PDM plugin to sync the exported files with the project file
+Keywords: pdm plugin
+Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
-Keywords: pdm,plugin
-Author-email: Frost Ming <mianghong@gmail.com>
-Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Project-URL: Changelog, https://github.com/frostming/pdm-autoexport/releases
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
 Project-URL: Homepage, https://github.com/frostming/pdm-autoexport
+Project-URL: Changelog, https://github.com/frostming/pdm-autoexport/releases
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # pdm-autoexport
 
 ![Github Actions](https://github.com/frostming/pdm-autoexport/workflows/Tests/badge.svg)
 [![PyPI](https://img.shields.io/pypi/v/pdm-autoexport?logo=python&logoColor=%23cccccc)](https://pypi.org/project/pdm-autoexport)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
@@ -59,8 +59,7 @@
 The configuration is an array of table `[[tool.pdm.autoexport]]` where each item may contain the following keys:
 
 - `filename` (required): The path to the exported file.
 - `groups` (optional, default: `["default"]`): The groups of optional dependencies or dev dependency groups of PDM to sync with.
 - `format` (optional, default: `"requirements"`): The format of the exported file, same as the `--format` option to the `pdm export` command.
   Only `requirements` and `setuppy` are supported.
 - `without-hashes` (optional, default: `false`): Whether to remove the hashes from the exported file. Only applicable to `requirements` format.
-
```

