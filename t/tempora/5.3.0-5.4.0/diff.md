# Comparing `tmp/tempora-5.3.0.tar.gz` & `tmp/tempora-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempora-5.3.0.tar", last modified: Sat Jun 10 16:01:54 2023, max compression
+gzip compressed data, was "tempora-5.4.0.tar", last modified: Tue Jun 27 08:55:02 2023, max compression
```

## Comparing `tempora-5.3.0.tar` & `tempora-5.4.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:01:54.641063 tempora-5.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-10 16:01:34.000000 tempora-5.3.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-10 16:01:34.000000 tempora-5.3.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:01:54.637063 tempora-5.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-10 16:01:34.000000 tempora-5.3.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-10 16:01:34.000000 tempora-5.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:01:54.637063 tempora-5.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-10 16:01:34.000000 tempora-5.3.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-10 16:01:34.000000 tempora-5.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-10 16:01:34.000000 tempora-5.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-06-10 16:01:34.000000 tempora-5.3.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-10 16:01:34.000000 tempora-5.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-10 16:01:54.641063 tempora-5.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-10 16:01:34.000000 tempora-5.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-10 16:01:34.000000 tempora-5.3.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:01:54.637063 tempora-5.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-10 16:01:34.000000 tempora-5.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-10 16:01:34.000000 tempora-5.3.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-10 16:01:34.000000 tempora-5.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-10 16:01:34.000000 tempora-5.3.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-10 16:01:34.000000 tempora-5.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-10 16:01:34.000000 tempora-5.3.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-10 16:01:54.645063 tempora-5.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:01:54.641063 tempora-5.3.0/tempora/
--rw-r--r--   0 runner    (1001) docker     (123)    18208 2023-06-10 16:01:34.000000 tempora-5.3.0/tempora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-06-10 16:01:34.000000 tempora-5.3.0/tempora/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-06-10 16:01:34.000000 tempora-5.3.0/tempora/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-10 16:01:34.000000 tempora-5.3.0/tempora/utc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:01:54.641063 tempora-5.3.0/tempora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-10 16:01:54.000000 tempora-5.3.0/tempora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-10 16:01:54.000000 tempora-5.3.0/tempora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 16:01:54.000000 tempora-5.3.0/tempora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-10 16:01:54.000000 tempora-5.3.0/tempora.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-10 16:01:54.000000 tempora-5.3.0/tempora.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 16:01:54.000000 tempora-5.3.0/tempora.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:01:54.641063 tempora-5.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-06-10 16:01:34.000000 tempora-5.3.0/tests/test_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-10 16:01:34.000000 tempora-5.3.0/tests/test_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-10 16:01:34.000000 tempora-5.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:55:02.851325 tempora-5.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-27 08:54:43.000000 tempora-5.4.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-27 08:54:43.000000 tempora-5.4.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:55:02.843325 tempora-5.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 08:54:43.000000 tempora-5.4.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 08:54:43.000000 tempora-5.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:55:02.843325 tempora-5.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-27 08:54:43.000000 tempora-5.4.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-27 08:54:43.000000 tempora-5.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-27 08:54:43.000000 tempora-5.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-27 08:54:43.000000 tempora-5.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-27 08:54:43.000000 tempora-5.4.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-27 08:55:02.851325 tempora-5.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-27 08:54:43.000000 tempora-5.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-27 08:54:43.000000 tempora-5.4.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:55:02.843325 tempora-5.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-27 08:54:43.000000 tempora-5.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 08:54:43.000000 tempora-5.4.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-27 08:54:43.000000 tempora-5.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-27 08:54:43.000000 tempora-5.4.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-27 08:54:43.000000 tempora-5.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 08:54:43.000000 tempora-5.4.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-27 08:55:02.851325 tempora-5.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:55:02.847325 tempora-5.4.0/tempora/
+-rw-r--r--   0 runner    (1001) docker     (123)    18208 2023-06-27 08:54:43.000000 tempora-5.4.0/tempora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-06-27 08:54:43.000000 tempora-5.4.0/tempora/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-06-27 08:54:43.000000 tempora-5.4.0/tempora/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-27 08:54:43.000000 tempora-5.4.0/tempora/utc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:55:02.847325 tempora-5.4.0/tempora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-27 08:55:02.000000 tempora-5.4.0/tempora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-27 08:55:02.000000 tempora-5.4.0/tempora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 08:55:02.000000 tempora-5.4.0/tempora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 08:55:02.000000 tempora-5.4.0/tempora.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 08:55:02.000000 tempora-5.4.0/tempora.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 08:55:02.000000 tempora-5.4.0/tempora.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:55:02.851325 tempora-5.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-06-27 08:54:43.000000 tempora-5.4.0/tests/test_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-27 08:54:43.000000 tempora-5.4.0/tests/test_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 08:54:43.000000 tempora-5.4.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-27 08:54:43.000000 tempora-5.4.0/tox.ini
```

### Comparing `tempora-5.3.0/.github/workflows/main.yml` & `tempora-5.4.0/.github/workflows/main.yml`

 * *Files 4% similar despite different names*

```diff
@@ -38,57 +38,51 @@
 
 
 jobs:
   test:
     strategy:
       matrix:
         python:
-        - "3.7"
+        - "3.8"
         - "3.11"
         - "3.12"
-        # Workaround for actions/setup-python#508
-        dev:
-        - -dev
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
-        - python: "3.8"
-          platform: ubuntu-latest
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
         - python: pypy3.9
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
     continue-on-error: ${{ matrix.python == '3.12' }}
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
+          python-version: ${{ matrix.python }}
+          allow-prereleases: true
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Run tests
         run: tox
 
   docs:
     runs-on: ubuntu-latest
     env:
       TOXENV: docs
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
-        with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Run tests
         run: tox
 
   check:  # This job does nothing and is only used for the branch protection
```

### Comparing `tempora-5.3.0/CHANGES.rst` & `tempora-5.4.0/NEWS.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v5.4.0
+======
+
+Features
+--------
+
+- Require Python 3.8 or later.
+
+
 v5.3.0
 ======
 
 #24: Removed use of ``datetime.utc**`` functions
 deprecated in Python 3.12.
 
 v5.2.2
```

### Comparing `tempora-5.3.0/LICENSE` & `tempora-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tempora-5.3.0/PKG-INFO` & `tempora-5.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: tempora
-Version: 5.3.0
+Version: 5.4.0
 Summary: Objects and routines pertaining to date and time (tempora)
 Home-page: https://github.com/jaraco/tempora
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/tempora.svg
    :target: https://pypi.org/project/tempora
 
 .. image:: https://img.shields.io/pypi/pyversions/tempora.svg
 
 .. image:: https://github.com/jaraco/tempora/workflows/tests/badge.svg
    :target: https://github.com/jaraco/tempora/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/tempora/badge/?version=latest
    :target: https://tempora.readthedocs.io/en/latest/?badge=latest
```

### Comparing `tempora-5.3.0/README.rst` & `tempora-5.4.0/tempora.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,37 @@
+Metadata-Version: 2.1
+Name: tempora
+Version: 5.4.0
+Summary: Objects and routines pertaining to date and time (tempora)
+Home-page: https://github.com/jaraco/tempora
+Author: Jason R. Coombs
+Author-email: jaraco@jaraco.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8
+Provides-Extra: testing
+Provides-Extra: docs
+License-File: LICENSE
+
 .. image:: https://img.shields.io/pypi/v/tempora.svg
    :target: https://pypi.org/project/tempora
 
 .. image:: https://img.shields.io/pypi/pyversions/tempora.svg
 
 .. image:: https://github.com/jaraco/tempora/workflows/tests/badge.svg
    :target: https://github.com/jaraco/tempora/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/tempora/badge/?version=latest
    :target: https://tempora.readthedocs.io/en/latest/?badge=latest
```

### Comparing `tempora-5.3.0/docs/conf.py` & `tempora-5.4.0/docs/conf.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 master_doc = "index"
 html_theme = "furo"
 
 # Link dates and other references in the changelog
 extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
```

### Comparing `tempora-5.3.0/docs/index.rst` & `tempora-5.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tempora-5.3.0/pytest.ini` & `tempora-5.4.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `tempora-5.3.0/setup.cfg` & `tempora-5.4.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	pytz
 	jaraco.functools>=1.20
 
 [options.packages.find]
 exclude = 
 	build*
@@ -32,15 +32,15 @@
 	pytest >= 6
 	pytest-checkdocs >= 2.4
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
-	pytest-enabler >= 1.3
+	pytest-enabler >= 2.2
 	pytest-ruff
 	
 	backports.unittest_mock
 	pytest-freezer
 	types-pytz
 docs = 
 	sphinx >= 3.5
```

### Comparing `tempora-5.3.0/tempora/__init__.py` & `tempora-5.4.0/tempora/__init__.py`

 * *Files identical despite different names*

### Comparing `tempora-5.3.0/tempora/schedule.py` & `tempora-5.4.0/tempora/schedule.py`

 * *Files identical despite different names*

### Comparing `tempora-5.3.0/tempora/timing.py` & `tempora-5.4.0/tempora/timing.py`

 * *Files identical despite different names*

### Comparing `tempora-5.3.0/tempora/utc.py` & `tempora-5.4.0/tempora/utc.py`

 * *Files identical despite different names*

### Comparing `tempora-5.3.0/tempora.egg-info/SOURCES.txt` & `tempora-5.4.0/tempora.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 .coveragerc
 .editorconfig
 .pre-commit-config.yaml
 .readthedocs.yaml
-CHANGES.rst
 LICENSE
+NEWS.rst
 README.rst
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
+towncrier.toml
 tox.ini
 .github/FUNDING.yml
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
```

### Comparing `tempora-5.3.0/tests/test_schedule.py` & `tempora-5.4.0/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `tempora-5.3.0/tests/test_timing.py` & `tempora-5.4.0/tests/test_timing.py`

 * *Files identical despite different names*

### Comparing `tempora-5.3.0/tox.ini` & `tempora-5.4.0/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 [tox]
-envlist = python
-minversion = 3.2
-# https://github.com/jaraco/skeleton/issues/6
-tox_pip_extensions_ext_venv_update = true
 toxworkdir={env:TOX_WORK_DIR:.tox}
 
 
 [testenv]
 deps =
 setenv =
 	PYTHONWARNDEFAULTENCODING = 1
@@ -21,14 +17,24 @@
 	docs
 	testing
 changedir = docs
 commands =
 	python -m sphinx -W --keep-going . {toxinidir}/build/html
 	python -m sphinxlint
 
+[testenv:finalize]
+skip_install = True
+deps =
+	towncrier
+	jaraco.develop >= 7.23
+passenv = *
+commands =
+	python -m jaraco.develop.finalize
+
+
 [testenv:release]
 skip_install = True
 deps =
 	build
 	twine>=3
 	jaraco.develop>=7.1
 passenv =
```

