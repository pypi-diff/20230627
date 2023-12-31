# Comparing `tmp/netlify_builds-0.3.3.tar.gz` & `tmp/netlify_builds-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netlify_builds-0.3.3.tar", max compression
+gzip compressed data, was "netlify_builds-1.0.0.tar", max compression
```

## Comparing `netlify_builds-0.3.3.tar` & `netlify_builds-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-03-27 19:28:50.392563 netlify_builds-0.3.3/LICENSE
--rw-r--r--   0        0        0     6020 2023-03-27 19:28:50.392563 netlify_builds-0.3.3/README.md
--rw-r--r--   0        0        0     1660 2023-03-27 19:28:51.084579 netlify_builds-0.3.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-27 19:28:51.068579 netlify_builds-0.3.3/src/netlify_builds/__init__.py
--rw-r--r--   0        0        0     3118 2023-03-27 19:28:50.392563 netlify_builds-0.3.3/src/netlify_builds/cli.py
--rw-r--r--   0        0        0     7393 1970-01-01 00:00:00.000000 netlify_builds-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-27 11:43:22.769859 netlify_builds-1.0.0/LICENSE
+-rw-r--r--   0        0        0     6020 2023-06-27 11:43:22.769859 netlify_builds-1.0.0/README.md
+-rw-r--r--   0        0        0     1662 2023-06-27 11:43:23.593864 netlify_builds-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-27 11:43:23.577864 netlify_builds-1.0.0/src/netlify_builds/__init__.py
+-rw-r--r--   0        0        0     3118 2023-06-27 11:43:22.773859 netlify_builds-1.0.0/src/netlify_builds/cli.py
+-rw-r--r--   0        0        0     7347 1970-01-01 00:00:00.000000 netlify_builds-1.0.0/PKG-INFO
```

### Comparing `netlify_builds-0.3.3/LICENSE` & `netlify_builds-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netlify_builds-0.3.3/README.md` & `netlify_builds-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `netlify_builds-0.3.3/pyproject.toml` & `netlify_builds-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netlify-builds"
-version = "0.3.3"
+version = "1.0.0"
 description = "A command line utility to check build usage across multiple Netlify accounts"
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/browniebroke/netlify-builds"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
@@ -23,16 +23,16 @@
 "Twitter" = "https://twitter.com/_BrunoAlla"
 "Mastodon" = "https://fosstodon.org/@browniebroke"
 
 [tool.poetry.scripts]
 netlify-builds = "netlify_builds.cli:main"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-httpx = "^0.23"
+python = "^3.8"
+httpx = "^0.24.0"
 python-dateutil = "^2.8"
 rich = ">=10"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.0"
```

### Comparing `netlify_builds-0.3.3/src/netlify_builds/cli.py` & `netlify_builds-1.0.0/src/netlify_builds/cli.py`

 * *Files identical despite different names*

### Comparing `netlify_builds-0.3.3/PKG-INFO` & `netlify_builds-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: netlify-builds
-Version: 0.3.3
+Version: 1.0.0
 Summary: A command line utility to check build usage across multiple Netlify accounts
 Home-page: https://github.com/browniebroke/netlify-builds
 License: MIT
 Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: httpx (>=0.23,<0.24)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: python-dateutil (>=2.8,<3.0)
 Requires-Dist: rich (>=10)
 Project-URL: Bug Tracker, https://github.com/browniebroke/netlify-builds/issues
 Project-URL: Changelog, https://netlify-builds.readthedocs.io/changelog.html
 Project-URL: Mastodon, https://fosstodon.org/@browniebroke
 Project-URL: Repository, https://github.com/browniebroke/netlify-builds
 Project-URL: Twitter, https://twitter.com/_BrunoAlla
```

#### html2text {}

```diff
@@ -1,26 +1,25 @@
-Metadata-Version: 2.1 Name: netlify-builds Version: 0.3.3 Summary: A command
+Metadata-Version: 2.1 Name: netlify-builds Version: 1.0.0 Summary: A command
 line utility to check build usage across multiple Netlify accounts Home-page:
 https://github.com/browniebroke/netlify-builds License: MIT Author: Bruno Alla
-Author-email: alla.brunoo@gmail.com Requires-Python: >=3.7,<4.0 Classifier:
+Author-email: alla.brunoo@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Topic :: Software Development :: Libraries Requires-Dist: httpx (>=0.23,<0.24)
-Requires-Dist: python-dateutil (>=2.8,<3.0) Requires-Dist: rich (>=10) Project-
-URL: Bug Tracker, https://github.com/browniebroke/netlify-builds/issues
-Project-URL: Changelog, https://netlify-builds.readthedocs.io/changelog.html
-Project-URL: Mastodon, https://fosstodon.org/@browniebroke Project-URL:
-Repository, https://github.com/browniebroke/netlify-builds Project-URL:
-Twitter, https://twitter.com/_BrunoAlla Description-Content-Type: text/markdown
-# Netlify Builds
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Software Development :: Libraries Requires-
+Dist: httpx (>=0.24.0,<0.25.0) Requires-Dist: python-dateutil (>=2.8,<3.0)
+Requires-Dist: rich (>=10) Project-URL: Bug Tracker, https://github.com/
+browniebroke/netlify-builds/issues Project-URL: Changelog, https://netlify-
+builds.readthedocs.io/changelog.html Project-URL: Mastodon, https://
+fosstodon.org/@browniebroke Project-URL: Repository, https://github.com/
+browniebroke/netlify-builds Project-URL: Twitter, https://twitter.com/
+_BrunoAlla Description-Content-Type: text/markdown # Netlify Builds
          [CI_Status] [Test_coverage_percentage] [pre-commit.ci_status]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 A command line utility to check build usage across multiple Netlify accounts ##
 Installation Recommended to install this via [pipx]: `pipx install netlify-
 builds` ## Setup Create a `.netlify-builds.json` in your home directory with
 the following shape: ```json { "team-name-1": "access-token-1", "team-name-2":
```

