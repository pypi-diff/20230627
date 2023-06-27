# Comparing `tmp/pelican-references-0.3.0.tar.gz` & `tmp/pelican_references-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican-references-0.3.0.tar", max compression
+gzip compressed data, was "pelican_references-0.3.1.tar", max compression
```

## Comparing `pelican-references-0.3.0.tar` & `pelican_references-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1368 2021-10-28 13:12:23.625145 pelican-references-0.3.0/README.md
--rw-r--r--   0        0        0       47 2021-10-28 13:12:23.626145 pelican-references-0.3.0/pelican/plugins/references/__init__.py
--rw-r--r--   0        0        0        0 2021-10-18 11:17:28.158143 pelican-references-0.3.0/pelican/plugins/references/labels/__init__.py
--rw-r--r--   0        0        0     1074 2021-10-28 13:12:23.626145 pelican-references-0.3.0/pelican/plugins/references/labels/number_brackets.py
--rw-r--r--   0        0        0     6698 2021-10-28 13:12:23.626145 pelican-references-0.3.0/pelican/plugins/references/references.py
--rw-r--r--   0        0        0      595 2021-10-18 11:17:28.159143 pelican-references-0.3.0/pelican/plugins/references/settings.py
--rw-r--r--   0        0        0       27 2021-10-18 11:17:28.159143 pelican-references-0.3.0/pelican/plugins/references/test_references.py
--rw-r--r--   0        0        0     2156 2022-04-08 10:51:04.454765 pelican-references-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2536 2022-04-08 10:55:15.363830 pelican-references-0.3.0/setup.py
--rw-r--r--   0        0        0     2769 2022-04-08 10:55:15.364102 pelican-references-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1368 2021-10-28 13:12:23.625145 pelican_references-0.3.1/README.md
+-rw-r--r--   0        0        0       47 2021-10-28 13:12:23.626145 pelican_references-0.3.1/pelican/plugins/references/__init__.py
+-rw-r--r--   0        0        0        0 2021-10-18 11:17:28.158143 pelican_references-0.3.1/pelican/plugins/references/labels/__init__.py
+-rw-r--r--   0        0        0     1074 2021-10-28 13:12:23.626145 pelican_references-0.3.1/pelican/plugins/references/labels/number_brackets.py
+-rw-r--r--   0        0        0     6698 2021-10-28 13:12:23.626145 pelican_references-0.3.1/pelican/plugins/references/references.py
+-rw-r--r--   0        0        0      595 2021-10-18 11:17:28.159143 pelican_references-0.3.1/pelican/plugins/references/settings.py
+-rw-r--r--   0        0        0       27 2021-10-18 11:17:28.159143 pelican_references-0.3.1/pelican/plugins/references/test_references.py
+-rw-r--r--   0        0        0     2153 2023-06-27 10:49:28.090256 pelican_references-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2777 1970-01-01 00:00:00.000000 pelican_references-0.3.1/PKG-INFO
```

### Comparing `pelican-references-0.3.0/README.md` & `pelican_references-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pelican-references-0.3.0/pelican/plugins/references/labels/number_brackets.py` & `pelican_references-0.3.1/pelican/plugins/references/labels/number_brackets.py`

 * *Files identical despite different names*

### Comparing `pelican-references-0.3.0/pelican/plugins/references/references.py` & `pelican_references-0.3.1/pelican/plugins/references/references.py`

 * *Files identical despite different names*

### Comparing `pelican-references-0.3.0/pelican/plugins/references/settings.py` & `pelican_references-0.3.1/pelican/plugins/references/settings.py`

 * *Files identical despite different names*

### Comparing `pelican-references-0.3.0/pyproject.toml` & `pelican_references-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 documentation = "https://docs.getpelican.com"
 keywords = ["pelican", "plugin"]
 license = "AGPL-3.0"
 name = "pelican-references"
 packages = [{include = "pelican"}]
 readme = "README.md"
 repository = "https://github.com/f-koehler/pelican-references"
-version = "0.3.0"
+version = "0.3.1"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Console",
   "Framework :: Pelican",
   "Framework :: Pelican :: Plugins",
   "Intended Audience :: End Users/Desktop",
@@ -25,30 +25,30 @@
 "Funding" = "https://donate.getpelican.com/"
 "Issue Tracker" = "https://github.com/f-koehler/pelican-references/issues"
 
 [tool.poetry.dependencies]
 beautifulsoup4 = "^4.9.3"
 markdown = {version = ">=3.2", optional = true}
 pelican = ">=4.5"
-pre-commit = "^2.13.0"
 pybtex = "^0.24.0"
 python = ">=3.10,<4.0"
 
 [tool.poetry.dev-dependencies]
+pre-commit = "^3.0.0"
 Werkzeug = "^2.0"
-black = {version = "^22.1", allow-prereleases = true}
-flake8 = "^4.0"
+black = {version = "^23.1", allow-prereleases = true}
+flake8 = "^6.0"
 flake8-black = "^0.3"
-invoke = "^1.3"
+invoke = "^2.0"
 isort = "^5.4"
 livereload = "^2.6"
 markdown = "^3.2"
-mypy = "^0.942"
+mypy = "^1.0"
 pytest = "^7.0"
-pytest-cov = "^3.0"
+pytest-cov = "^4.0"
 pytest-pythonpath = "^0.7"
 pytest-sugar = "^0.9"
 types-beautifulsoup4 = "^4.9.0"
 
 [tool.poetry.extras]
 markdown = ["markdown"]
```

### Comparing `pelican-references-0.3.0/PKG-INFO` & `pelican_references-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelican-references
-Version: 0.3.0
+Version: 0.3.1
 Summary: Generate bibliographies from BibTeX files
 Home-page: https://github.com/f-koehler/pelican-references
 License: AGPL-3.0
 Keywords: pelican,plugin
 Author: Fabian Köhler
 Author-email: fabian.koehler@protonmail.ch
 Requires-Python: >=3.10,<4.0
@@ -13,21 +13,21 @@
 Classifier: Framework :: Pelican
 Classifier: Framework :: Pelican :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: markdown
 Requires-Dist: beautifulsoup4 (>=4.9.3,<5.0.0)
-Requires-Dist: markdown (>=3.2); extra == "markdown"
+Requires-Dist: markdown (>=3.2) ; extra == "markdown"
 Requires-Dist: pelican (>=4.5)
-Requires-Dist: pre-commit (>=2.13.0,<3.0.0)
 Requires-Dist: pybtex (>=0.24.0,<0.25.0)
 Project-URL: Documentation, https://docs.getpelican.com
 Project-URL: Funding, https://donate.getpelican.com/
 Project-URL: Issue Tracker, https://github.com/f-koehler/pelican-references/issues
 Project-URL: Repository, https://github.com/f-koehler/pelican-references
 Description-Content-Type: text/markdown
```

