# Comparing `tmp/pepotron-0.9.0.tar.gz` & `tmp/pepotron-1.0.0.tar.gz`

## Comparing `pepotron-0.9.0.tar` & `pepotron-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 pepotron-0.9.0/.coveragerc
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pepotron-0.9.0/.editorconfig
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pepotron-0.9.0/.flake8
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 pepotron-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pepotron-0.9.0/RELEASING.md
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 pepotron-0.9.0/tox.ini
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 pepotron-0.9.0/.github/labels.yml
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 pepotron-0.9.0/.github/release-drafter.yml
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pepotron-0.9.0/.github/renovate.json
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 pepotron-0.9.0/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 pepotron-0.9.0/.github/workflows/labels.yml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pepotron-0.9.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pepotron-0.9.0/.github/workflows/release-drafter.yml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pepotron-0.9.0/.github/workflows/require-pr-label.yml
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pepotron-0.9.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 pepotron-0.9.0/src/pepotron/__init__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pepotron-0.9.0/src/pepotron/__main__.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pepotron-0.9.0/src/pepotron/_cache.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 pepotron-0.9.0/src/pepotron/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pepotron-0.9.0/src/pepotron/scripts/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pepotron-0.9.0/src/pepotron/scripts/run_command.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pepotron-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 pepotron-0.9.0/tests/test_cache.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 pepotron-0.9.0/tests/test_pepotron.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pepotron-0.9.0/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pepotron-0.9.0/LICENSE.txt
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 pepotron-0.9.0/README.md
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 pepotron-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 pepotron-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 pepotron-1.0.0/.coveragerc
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pepotron-1.0.0/.editorconfig
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pepotron-1.0.0/.flake8
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 pepotron-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pepotron-1.0.0/RELEASING.md
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 pepotron-1.0.0/tox.ini
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 pepotron-1.0.0/.github/labels.yml
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 pepotron-1.0.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pepotron-1.0.0/.github/renovate.json
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 pepotron-1.0.0/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 pepotron-1.0.0/.github/workflows/labels.yml
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pepotron-1.0.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pepotron-1.0.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pepotron-1.0.0/.github/workflows/require-pr-label.yml
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pepotron-1.0.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 pepotron-1.0.0/src/pepotron/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pepotron-1.0.0/src/pepotron/__main__.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 pepotron-1.0.0/src/pepotron/_cache.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 pepotron-1.0.0/src/pepotron/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pepotron-1.0.0/src/pepotron/scripts/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pepotron-1.0.0/src/pepotron/scripts/run_command.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pepotron-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 pepotron-1.0.0/tests/test_cache.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 pepotron-1.0.0/tests/test_pepotron.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pepotron-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pepotron-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 pepotron-1.0.0/README.md
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 pepotron-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 pepotron-1.0.0/PKG-INFO
```

### Comparing `pepotron-0.9.0/.pre-commit-config.yaml` & `pepotron-1.0.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.4.0
     hooks:
       - id: pyupgrade
-        args: [--py37-plus]
+        args: [--py38-plus]
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/PyCQA/isort
@@ -37,37 +37,37 @@
       - id: check-json
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.3.0
     hooks:
       - id: mypy
         args: [--strict, --pretty, --show-error-codes]
         additional_dependencies:
           [httpx, platformdirs, pytest, types-freezegun, types-python-slugify]
 
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.9.2
+    rev: 0.10.0
     hooks:
       - id: pyproject-fmt
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.12.2
+    rev: v0.13
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/tox-dev/tox-ini-fmt
     rev: 1.3.0
     hooks:
       - id: tox-ini-fmt
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.6
+    rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
         args: [--prose-wrap=always, --print-width=88]
 
 ci:
   autoupdate_schedule: quarterly
```

### Comparing `pepotron-0.9.0/RELEASING.md` & `pepotron-1.0.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `pepotron-0.9.0/.github/labels.yml` & `pepotron-1.0.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `pepotron-0.9.0/.github/release-drafter.yml` & `pepotron-1.0.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pepotron-0.9.0/.github/workflows/deploy.yml` & `pepotron-1.0.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `pepotron-0.9.0/.github/workflows/release-drafter.yml` & `pepotron-1.0.0/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pepotron-0.9.0/.github/workflows/test.yml` & `pepotron-1.0.0/.github/workflows/test.yml`

 * *Files 11% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["pypy3.9", "3.7", "3.8", "3.9", "3.10", "3.11", "3.12-dev"]
+        python-version: ["pypy3.10", "3.8", "3.9", "3.10", "3.11", "3.12"]
         os: [windows-latest, macos-latest, ubuntu-latest]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
+          allow-prereleases: true
           cache: pip
           cache-dependency-path: pyproject.toml
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -U wheel
```

### Comparing `pepotron-0.9.0/src/pepotron/__init__.py` & `pepotron-1.0.0/src/pepotron/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 """
 CLI to open PEPs in your browser
 """
 from __future__ import annotations
 
+import importlib.metadata
 import logging
 import warnings
 from pathlib import Path
 
 from pepotron import _cache
 
-try:
-    # Python 3.8+
-    import importlib.metadata as importlib_metadata
-except ImportError:
-    # Python 3.7
-    import importlib_metadata  # type: ignore
-
-__version__ = importlib_metadata.version(__name__)
+__version__ = importlib.metadata.version(__name__)
 
 BASE_URL = "https://peps.python.org"
 JSON_PATH = "/api/peps.json"
 USER_AGENT = f"pepotron/{__version__}"
 
 TOPICS = ("governance", "packaging", "release", "typing")
 VERSION_TO_PEP = {
@@ -42,14 +36,15 @@
     "3.6": 494,
     "3.7": 537,
     "3.8": 569,
     "3.9": 596,
     "3.10": 619,
     "3.11": 664,
     "3.12": 693,
+    "3.13": 719,
 }
 
 
 def _download_peps_json() -> Path:
     json_url = BASE_URL + JSON_PATH
     cache_file = _cache.filename(json_url)
     logging.info(f"Cache file: {cache_file}")
```

### Comparing `pepotron-0.9.0/src/pepotron/_cache.py` & `pepotron-1.0.0/src/pepotron/_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 CACHE_DIR = Path(user_cache_dir("pepotron"))
 
 
 def filename(url: str) -> Path:
     """yyyy-mm-dd-url-slug.json"""
     from slugify import slugify
 
-    today = dt.datetime.utcnow().strftime("%Y-%m-%d")
+    today = dt.datetime.now(dt.timezone.utc).strftime("%Y-%m-%d")
     slug = slugify(url)
     return CACHE_DIR / f"{today}-{slug}.json"
 
 
 def load(cache_file: Path) -> PepData:
     """Load data from cache_file"""
     if not cache_file.exists():
@@ -59,11 +59,11 @@
     except OSError:
         pass
 
 
 def clear(clear_all: bool = False) -> None:
     """Delete all or old cache files"""
     cache_files = CACHE_DIR.glob("**/*.json")
-    today = dt.datetime.utcnow().strftime("%Y-%m-%d")
+    today = dt.datetime.now(dt.timezone.utc).strftime("%Y-%m-%d")
     for cache_file in cache_files:
         if clear_all or not cache_file.name.startswith(today):
             cache_file.unlink()
```

### Comparing `pepotron-0.9.0/src/pepotron/cli.py` & `pepotron-1.0.0/src/pepotron/cli.py`

 * *Files identical despite different names*

### Comparing `pepotron-0.9.0/src/pepotron/scripts/run_command.py` & `pepotron-1.0.0/src/pepotron/scripts/run_command.py`

 * *Files identical despite different names*

### Comparing `pepotron-0.9.0/tests/test_cache.py` & `pepotron-1.0.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `pepotron-0.9.0/tests/test_pepotron.py` & `pepotron-1.0.0/tests/test_pepotron.py`

 * *Files identical despite different names*

### Comparing `pepotron-0.9.0/.gitignore` & `pepotron-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pepotron-0.9.0/LICENSE.txt` & `pepotron-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pepotron-0.9.0/README.md` & `pepotron-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pepotron-0.9.0/pyproject.toml` & `pepotron-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -12,38 +12,36 @@
 keywords = [
   "bpo",
   "cli",
   "pep",
 ]
 license = {text = "MIT"}
 authors = [{name = "Hugo van Kemenade"}]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
-    "Development Status :: 4 - Beta",
-    "Intended Audience :: Developers",
-    "Intended Audience :: End Users/Desktop",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-    "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: Implementation :: PyPy",
+  "Development Status :: 5 - Production/Stable",
+  "Intended Audience :: Developers",
+  "Intended Audience :: End Users/Desktop",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: Implementation :: CPython",
+  "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
   "httpx>=0.22",
-  'importlib-metadata; python_version < "3.8"',
   "platformdirs",
   "python-slugify",
   "thefuzz",
 ]
 [project.optional-dependencies]
 tests = [
   "freezegun",
```

### Comparing `pepotron-0.9.0/PKG-INFO` & `pepotron-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: pepotron
-Version: 0.9.0
+Version: 1.0.0
 Summary: CLI to open PEPs in your browser
 Project-URL: Changelog, https://github.com/hugovk/pepotron/releases
 Project-URL: Homepage, https://github.com/hugovk/pepotron
 Project-URL: Source, https://github.com/hugovk/pepotron
 Author: Hugo van Kemenade
 License: MIT
 License-File: LICENSE.txt
 Keywords: bpo,cli,pep
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: httpx>=0.22
-Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: platformdirs
 Requires-Dist: python-slugify
 Requires-Dist: thefuzz
 Provides-Extra: tests
 Requires-Dist: freezegun; extra == 'tests'
 Requires-Dist: pytest; extra == 'tests'
 Requires-Dist: pytest-cov; extra == 'tests'
```

