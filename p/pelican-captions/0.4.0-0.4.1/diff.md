# Comparing `tmp/pelican-captions-0.4.0.tar.gz` & `tmp/pelican_captions-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican-captions-0.4.0.tar", max compression
+gzip compressed data, was "pelican_captions-0.4.1.tar", max compression
```

## Comparing `pelican-captions-0.4.0.tar` & `pelican_captions-0.4.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    32387 2021-10-18 11:17:28.015143 pelican-captions-0.4.0/LICENSE
--rw-r--r--   0        0        0     1377 2022-04-08 10:38:26.851452 pelican-captions-0.4.0/README.md
--rw-r--r--   0        0        0       45 2021-10-28 13:11:38.565142 pelican-captions-0.4.0/pelican/plugins/captions/__init__.py
--rw-r--r--   0        0        0     5514 2021-10-28 13:11:38.565142 pelican-captions-0.4.0/pelican/plugins/captions/captions.py
--rw-r--r--   0        0        0       27 2021-10-18 11:17:28.016143 pelican-captions-0.4.0/pelican/plugins/captions/test_captions.py
--rw-r--r--   0        0        0     1986 2022-04-08 11:05:03.968077 pelican-captions-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2268 2022-04-08 11:05:10.013050 pelican-captions-0.4.0/setup.py
--rw-r--r--   0        0        0     2718 2022-04-08 11:05:10.013312 pelican-captions-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    32387 2021-10-18 11:17:28.015143 pelican_captions-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1377 2022-04-08 10:38:26.851452 pelican_captions-0.4.1/README.md
+-rw-r--r--   0        0        0       45 2021-10-28 13:11:38.565142 pelican_captions-0.4.1/pelican/plugins/captions/__init__.py
+-rw-r--r--   0        0        0     5514 2021-10-28 13:11:38.565142 pelican_captions-0.4.1/pelican/plugins/captions/captions.py
+-rw-r--r--   0        0        0       27 2021-10-18 11:17:28.016143 pelican_captions-0.4.1/pelican/plugins/captions/test_captions.py
+-rw-r--r--   0        0        0     1983 2023-06-27 10:49:14.863588 pelican_captions-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2770 1970-01-01 00:00:00.000000 pelican_captions-0.4.1/PKG-INFO
```

### Comparing `pelican-captions-0.4.0/LICENSE` & `pelican_captions-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican-captions-0.4.0/README.md` & `pelican_captions-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pelican-captions-0.4.0/pelican/plugins/captions/captions.py` & `pelican_captions-0.4.1/pelican/plugins/captions/captions.py`

 * *Files identical despite different names*

### Comparing `pelican-captions-0.4.0/pyproject.toml` & `pelican_captions-0.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 documentation = "https://docs.getpelican.com"
 keywords = ["pelican", "plugin"]
 license = "AGPL-3.0"
 name = "pelican-captions"
 packages = [{include = "pelican"}]
 readme = "README.md"
 repository = "https://github.com/f-koehler/pelican-captions"
-version = "0.4.0"
+version = "0.4.1"
 
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
   "Framework :: Pelican",
   "Framework :: Pelican :: Plugins",
   "Intended Audience :: End Users/Desktop",
@@ -29,25 +29,25 @@
 beautifulsoup4 = "^4.9.3"
 markdown = {version = "^3.2.2", optional = true}
 pelican = "^4.5"
 python = ">=3.10,<4.0"
 
 [tool.poetry.dev-dependencies]
 Werkzeug = "^2.0"
-black = {version = "^22.1", allow-prereleases = true}
-flake8 = "^4.0"
+black = {version = "^23.1", allow-prereleases = true}
+flake8 = "^6.0"
 flake8-black = "^0.3.2"
-invoke = "^1.3"
+invoke = "^2.0"
 isort = "^5.4"
 livereload = "^2.6"
 markdown = "^3.2.2"
-mypy = "^0.942"
-pre-commit = "^2.12.1"
+mypy = "^1.0"
+pre-commit = "^3.0.0"
 pytest = "^7.0"
-pytest-cov = "^3.0"
+pytest-cov = "^4.0"
 pytest-pythonpath = "^0.7.3"
 pytest-sugar = "^0.9.4"
 types-beautifulsoup4 = "^4.9.0"
 
 [tool.poetry.extras]
 markdown = ["markdown"]
```

### Comparing `pelican-captions-0.4.0/PKG-INFO` & `pelican_captions-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelican-captions
-Version: 0.4.0
+Version: 0.4.1
 Summary: Add captions and labels to figures, tables and code blocks.
 Home-page: https://github.com/f-koehler/pelican-captions
 License: AGPL-3.0
 Keywords: pelican,plugin
 Author: Fabian Köhler
 Author-email: fabian.koehler@protonmail.ch
 Requires-Python: >=3.10,<4.0
@@ -13,19 +13,20 @@
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
-Requires-Dist: markdown (>=3.2.2,<4.0.0); extra == "markdown"
+Requires-Dist: markdown (>=3.2.2,<4.0.0) ; extra == "markdown"
 Requires-Dist: pelican (>=4.5,<5.0)
 Project-URL: Documentation, https://docs.getpelican.com
 Project-URL: Funding, https://donate.getpelican.com/
 Project-URL: Issue Tracker, https://github.com/f-koehler/pelican-captions/issues
 Project-URL: Repository, https://github.com/f-koehler/pelican-captions
 Description-Content-Type: text/markdown
```

