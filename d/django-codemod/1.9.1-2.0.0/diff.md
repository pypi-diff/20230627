# Comparing `tmp/django-codemod-1.9.1.tar.gz` & `tmp/django_codemod-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-codemod-1.9.1.tar", max compression
+gzip compressed data, was "django_codemod-2.0.0.tar", max compression
```

## Comparing `django-codemod-1.9.1.tar` & `django_codemod-2.0.0.tar`

### file list

```diff
@@ -1,36 +1,63 @@
--rw-r--r--   0        0        0     1068 2022-03-11 09:08:35.777822 django-codemod-1.9.1/LICENSE
--rw-r--r--   0        0        0     9810 2022-03-11 09:08:35.777822 django-codemod-1.9.1/README.md
--rw-r--r--   0        0        0     2203 2022-03-11 09:08:36.473827 django-codemod-1.9.1/pyproject.toml
--rw-r--r--   0        0        0       22 2022-03-11 09:08:36.461827 django-codemod-1.9.1/src/django_codemod/__init__.py
--rw-r--r--   0        0        0     8612 2022-03-11 09:08:35.777822 django-codemod-1.9.1/src/django_codemod/cli.py
--rw-r--r--   0        0        0      710 2022-03-11 09:08:35.777822 django-codemod-1.9.1/src/django_codemod/commands.py
--rw-r--r--   0        0        0      448 2022-03-11 09:08:35.777822 django-codemod-1.9.1/src/django_codemod/constants.py
--rw-r--r--   0        0        0      116 2022-03-11 09:08:35.777822 django-codemod-1.9.1/src/django_codemod/feature_flags.py
--rw-r--r--   0        0        0     3640 2022-03-11 09:08:35.777822 django-codemod-1.9.1/src/django_codemod/path_utils.py
--rw-r--r--   0        0        0        0 2022-03-11 09:08:35.777822 django-codemod-1.9.1/src/django_codemod/utils/__init__.py
--rw-r--r--   0        0        0     1378 2022-03-11 09:08:35.777822 django-codemod-1.9.1/src/django_codemod/utils/calls.py
--rw-r--r--   0        0        0     3367 2022-03-11 09:08:35.777822 django-codemod-1.9.1/src/django_codemod/visitors/__init__.py
--rw-r--r--   0        0        0     5979 2022-03-11 09:08:35.777822 django-codemod-1.9.1/src/django_codemod/visitors/admin.py
--rw-r--r--   0        0        0    14945 2022-03-11 09:08:35.777822 django-codemod-1.9.1/src/django_codemod/visitors/base.py
--rw-r--r--   0        0        0      379 2022-03-11 09:08:35.777822 django-codemod-1.9.1/src/django_codemod/visitors/core.py
--rw-r--r--   0        0        0     1222 2022-03-11 09:08:35.781823 django-codemod-1.9.1/src/django_codemod/visitors/crypto.py
--rw-r--r--   0        0        0     1107 2022-03-11 09:08:35.781823 django-codemod-1.9.1/src/django_codemod/visitors/decorators.py
--rw-r--r--   0        0        0     1042 2022-03-11 09:08:35.781823 django-codemod-1.9.1/src/django_codemod/visitors/encoding.py
--rw-r--r--   0        0        0     1459 2022-03-11 09:08:35.781823 django-codemod-1.9.1/src/django_codemod/visitors/exceptions.py
--rw-r--r--   0        0        0      699 2022-03-11 09:08:35.781823 django-codemod-1.9.1/src/django_codemod/visitors/forms.py
--rw-r--r--   0        0        0      415 2022-03-11 09:08:35.781823 django-codemod-1.9.1/src/django_codemod/visitors/html.py
--rw-r--r--   0        0        0     3240 2022-03-11 09:08:35.781823 django-codemod-1.9.1/src/django_codemod/visitors/http.py
--rw-r--r--   0        0        0      413 2022-03-11 09:08:35.781823 django-codemod-1.9.1/src/django_codemod/visitors/lru_cache.py
--rw-r--r--   0        0        0     7917 2022-03-11 09:08:35.781823 django-codemod-1.9.1/src/django_codemod/visitors/models.py
--rw-r--r--   0        0        0      390 2022-03-11 09:08:35.781823 django-codemod-1.9.1/src/django_codemod/visitors/os_utils.py
--rw-r--r--   0        0        0      422 2022-03-11 09:08:35.781823 django-codemod-1.9.1/src/django_codemod/visitors/paginator.py
--rw-r--r--   0        0        0     1116 2022-03-11 09:08:35.781823 django-codemod-1.9.1/src/django_codemod/visitors/postgres_fields.py
--rw-r--r--   0        0        0      648 2022-03-11 09:08:35.781823 django-codemod-1.9.1/src/django_codemod/visitors/shortcuts.py
--rw-r--r--   0        0        0     3974 2022-03-11 09:08:35.781823 django-codemod-1.9.1/src/django_codemod/visitors/signals.py
--rw-r--r--   0        0        0     1339 2022-03-11 09:08:35.781823 django-codemod-1.9.1/src/django_codemod/visitors/template_context.py
--rw-r--r--   0        0        0     5774 2022-03-11 09:08:35.781823 django-codemod-1.9.1/src/django_codemod/visitors/template_tags.py
--rw-r--r--   0        0        0     1259 2022-03-11 09:08:35.781823 django-codemod-1.9.1/src/django_codemod/visitors/timezone.py
--rw-r--r--   0        0        0     1654 2022-03-11 09:08:35.781823 django-codemod-1.9.1/src/django_codemod/visitors/translations.py
--rw-r--r--   0        0        0     4170 2022-03-11 09:08:35.781823 django-codemod-1.9.1/src/django_codemod/visitors/urls.py
--rw-r--r--   0        0        0    11076 2022-03-11 09:08:45.616405 django-codemod-1.9.1/setup.py
--rw-r--r--   0        0        0    11365 2022-03-11 09:08:45.617512 django-codemod-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-27 12:18:53.930551 django_codemod-2.0.0/LICENSE
+-rw-r--r--   0        0        0     9809 2023-06-27 12:18:53.930551 django_codemod-2.0.0/README.md
+-rw-r--r--   0        0        0     2340 2023-06-27 12:18:55.098557 django_codemod-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-27 12:18:55.066557 django_codemod-2.0.0/src/django_codemod/__init__.py
+-rw-r--r--   0        0        0     8612 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/cli.py
+-rw-r--r--   0        0        0      710 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/commands.py
+-rw-r--r--   0        0        0      448 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/constants.py
+-rw-r--r--   0        0        0      116 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/feature_flags.py
+-rw-r--r--   0        0        0     3640 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/path_utils.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/utils/__init__.py
+-rw-r--r--   0        0        0     1378 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/utils/calls.py
+-rw-r--r--   0        0        0     3367 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/__init__.py
+-rw-r--r--   0        0        0     5978 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/admin.py
+-rw-r--r--   0        0        0    14945 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/base.py
+-rw-r--r--   0        0        0      379 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/core.py
+-rw-r--r--   0        0        0     1222 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/crypto.py
+-rw-r--r--   0        0        0     1107 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/decorators.py
+-rw-r--r--   0        0        0     1042 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/encoding.py
+-rw-r--r--   0        0        0     1459 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/exceptions.py
+-rw-r--r--   0        0        0      699 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/forms.py
+-rw-r--r--   0        0        0      415 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/html.py
+-rw-r--r--   0        0        0     3240 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/http.py
+-rw-r--r--   0        0        0      413 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/lru_cache.py
+-rw-r--r--   0        0        0     7917 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/models.py
+-rw-r--r--   0        0        0      390 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/os_utils.py
+-rw-r--r--   0        0        0      422 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/paginator.py
+-rw-r--r--   0        0        0     1116 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/postgres_fields.py
+-rw-r--r--   0        0        0      648 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/shortcuts.py
+-rw-r--r--   0        0        0     3974 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/signals.py
+-rw-r--r--   0        0        0     1339 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/template_context.py
+-rw-r--r--   0        0        0     5774 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/template_tags.py
+-rw-r--r--   0        0        0     1259 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/timezone.py
+-rw-r--r--   0        0        0     1654 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/translations.py
+-rw-r--r--   0        0        0     4170 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/urls.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     6320 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/test_cli.py
+-rwxr-xr-x   0        0        0      737 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/test_e2e.sh
+-rw-r--r--   0        0        0     6959 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/test_path_utils.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/__init__.py
+-rw-r--r--   0        0        0      484 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/base.py
+-rw-r--r--   0        0        0     7083 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_admin.py
+-rw-r--r--   0        0        0    14132 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_base.py
+-rw-r--r--   0        0        0      951 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_core.py
+-rw-r--r--   0        0        0     2264 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_crypto.py
+-rw-r--r--   0        0        0     1894 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_decorators.py
+-rw-r--r--   0        0        0     1704 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_encoding.py
+-rw-r--r--   0        0        0     2071 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_exceptions.py
+-rw-r--r--   0        0        0      954 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_forms.py
+-rw-r--r--   0        0        0      559 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_html.py
+-rw-r--r--   0        0        0     5449 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_http.py
+-rw-r--r--   0        0        0      531 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_lru_cache.py
+-rw-r--r--   0        0        0    11944 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_models.py
+-rw-r--r--   0        0        0      514 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_os_utils.py
+-rw-r--r--   0        0        0     1351 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_paginator.py
+-rw-r--r--   0        0        0     2560 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_postgres_fields.py
+-rw-r--r--   0        0        0      671 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_shortcuts.py
+-rw-r--r--   0        0        0     4162 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_signals.py
+-rw-r--r--   0        0        0     1957 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_template_context.py
+-rw-r--r--   0        0        0     4713 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_template_tags.py
+-rw-r--r--   0        0        0     2409 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_timezone.py
+-rw-r--r--   0        0        0     4501 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_translations.py
+-rw-r--r--   0        0        0     6971 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_urls.py
+-rw-r--r--   0        0        0    11280 1970-01-01 00:00:00.000000 django_codemod-2.0.0/PKG-INFO
```

### Comparing `django-codemod-1.9.1/LICENSE` & `django_codemod-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/README.md` & `django_codemod-2.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <p align="center">
   <img alt="Django Codemod" src="https://raw.githubusercontent.com/browniebroke/django-codemod/main/assets/djangocodemod-stroke.png">
 </p>
 
 <p align="center">
-  <a href="https://github.com/browniebroke/django-codemod/actions?query=workflow%3ACI">
-    <img alt="CI Status" src="https://img.shields.io/github/workflow/status/browniebroke/django-codemod/CI?label=CI&logo=github&style=flat-square">
+  <a href="https://github.com/browniebroke/django-codemod/actions/workflows/ci.yml?query=branch%3Amain">
+    <img alt="CI Status" src="https://img.shields.io/github/actions/workflow/status/browniebroke/django-codemod/ci.yml?branch=main&label=CI&logo=github&style=flat-square">
   </a>
   <a href="https://django-codemod.readthedocs.io">
     <img src="https://img.shields.io/readthedocs/django-codemod.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">
   </a>
   <a href="https://codecov.io/gh/browniebroke/django-codemod">
     <img src="https://img.shields.io/codecov/c/github/browniebroke/django-codemod.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
   </a>
@@ -61,15 +61,15 @@
 - This tool is best suited for Django sites, NOT for reusable Django applications. The project needs to target a single Django version, e.g. 3.1.x.
 - You do NOT need to install this tool as part of your project dependencies, it is a CLI tool, not a Django package to be installed in your site.
 
 ### Similar tools
 
 [django-upgrade](https://github.com/adamchainz/django-upgrade) is a similar tool written by Adam Johnson. It's a reimplementation taking a different approach based only on standard library module.
 
-django-codemod is based on [libCST](https://libcst.readthedocs.io/) (Concrete Syntax Tree), and it's a limiting factor in terms of supported Python versions as well as its speed. By using standard library modules, django-upgrade is a lot faster and is able to support the latest Python, however it requires Python 3.8+.
+django-codemod is based on [libCST](https://libcst.readthedocs.io/) (Concrete Syntax Tree) which is a limiting factor in terms of speed. By using standard library modules, django-upgrade is a lot faster and is able to support the latest Python, however it requires Python 3.8+.
 
 ## Contributors ✨
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
```

#### html2text {}

```diff
@@ -26,20 +26,19 @@
 for Django sites, NOT for reusable Django applications. The project needs to
 target a single Django version, e.g. 3.1.x. - You do NOT need to install this
 tool as part of your project dependencies, it is a CLI tool, not a Django
 package to be installed in your site. ### Similar tools [django-upgrade](https:
 //github.com/adamchainz/django-upgrade) is a similar tool written by Adam
 Johnson. It's a reimplementation taking a different approach based only on
 standard library module. django-codemod is based on [libCST](https://
-libcst.readthedocs.io/) (Concrete Syntax Tree), and it's a limiting factor in
-terms of supported Python versions as well as its speed. By using standard
-library modules, django-upgrade is a lot faster and is able to support the
-latest Python, however it requires Python 3.8+. ## Contributors â¨ Thanks goes
-to these wonderful people ([emoji key](https://allcontributors.org/docs/en/
-emoji-key)):
+libcst.readthedocs.io/) (Concrete Syntax Tree) which is a limiting factor in
+terms of speed. By using standard library modules, django-upgrade is a lot
+faster and is able to support the latest Python, however it requires Python
+3.8+. ## Contributors â¨ Thanks goes to these wonderful people ([emoji key]
+(https://allcontributors.org/docs/en/emoji-key)):
 
         Bruno_Alla                 Aarni_Koskela             Adam     Nikita    Chris     John_Vandenberg  Anjishnu
                                                            Johnson   Sobolev  VanderKolk
       ð» ð ð�       ð» ð¤ â                                    ð ð�  ð
                                                              ð  ð�   ð»
 
           Drew_Winstel                Dmytro_Litvinov         M.
```

### Comparing `django-codemod-1.9.1/pyproject.toml` & `django_codemod-2.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-codemod"
-version = "1.9.1"
+version = "2.0.0"
 description = "A command line tool to automatically fix Django deprecations."
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["django", "codemod", "libCST"]
 repository = "https://github.com/browniebroke/django-codemod"
 documentation = "https://django-codemod.readthedocs.io"
@@ -13,54 +13,47 @@
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
 ]
 packages = [
     { include = "django_codemod", from = "src" },
+    { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/browniebroke/django-codemod/issues"
 "Changelog" = "https://django-codemod.readthedocs.io/en/stable/changelog.html"
+"Twitter" = "https://twitter.com/_BrunoAlla"
+"Mastodon" = "https://fosstodon.org/@browniebroke"
 
 [tool.poetry.scripts]
 djcodemod = "django_codemod.cli:djcodemod"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 click = "<9"
-libcst = "==0.4.1"
+libcst = "==1.0.1"
 pathspec = ">=0.6,<1"
-rich = "<13"
+rich = ">=10"
 rich-click = ">=1.0"
 
-# Docs deps
-Sphinx = { version = "^4.0", optional = true }
-sphinx-rtd-theme = { version = "^1.0", optional = true }
-myst-parser = { version = "^0.17.0", optional = true }
-
-[tool.poetry.extras]
-docs = [
-    "myst-parser",
-    "sphinx",
-    "sphinx-rtd-theme",
-]
-
 [tool.poetry.dev-dependencies]
+parameterized = "^0.9.0"
 pytest = "^7.0"
-black = "^22.1"
-pytest-cov = "^3.0"
+pytest-cov = "^4.0"
 pytest-mock = "^3.3"
-tox = "^3.20"
-parameterized = "^0.8.0"
-flake8 = "^4.0"
-pyupgrade = "^2.31"
-isort = "^5.10"
-mypy = "^0.931"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+myst-parser = ">=0.16"
+sphinx = ">=4.0"
+sphinx-rtd-theme = ">=1.0"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/django_codemod/__init__.py:__version__"
 build_command = "pip install poetry && poetry build"
 
@@ -78,10 +71,21 @@
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "raise AssertionError",
     "raise NotImplementedError",
 ]
 
+[tool.mypy]
+# suppress errors about unsatisfied imports
+ignore_missing_imports = true
+
+no_implicit_optional = true
+
+# ensure all execution paths are returning
+warn_no_return = true
+
+show_error_codes = true
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django-codemod-1.9.1/src/django_codemod/cli.py` & `django_codemod-2.0.0/src/django_codemod/cli.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/commands.py` & `django_codemod-2.0.0/src/django_codemod/commands.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/path_utils.py` & `django_codemod-2.0.0/src/django_codemod/path_utils.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/utils/calls.py` & `django_codemod-2.0.0/src/django_codemod/utils/calls.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/visitors/__init__.py` & `django_codemod-2.0.0/src/django_codemod/visitors/__init__.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/visitors/admin.py` & `django_codemod-2.0.0/src/django_codemod/visitors/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,14 @@
                     base_cls_matcher.append(m.Arg(m.Name("StackedInline")))
         if m.matches(
             updated_node,
             m.ImportFrom(module=module_matcher(["django", "contrib"])),
         ):
             for imported_name in updated_node.names:
                 if m.matches(imported_name, m.ImportAlias(name=m.Name("admin"))):
-
                     base_cls_matcher.extend(
                         [
                             m.Arg(
                                 m.Attribute(
                                     value=m.Name("admin"), attr=m.Name("TabularInline")
                                 )
                             ),
```

### Comparing `django-codemod-1.9.1/src/django_codemod/visitors/base.py` & `django_codemod-2.0.0/src/django_codemod/visitors/base.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/visitors/crypto.py` & `django_codemod-2.0.0/src/django_codemod/visitors/crypto.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/visitors/decorators.py` & `django_codemod-2.0.0/src/django_codemod/visitors/decorators.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/visitors/encoding.py` & `django_codemod-2.0.0/src/django_codemod/visitors/encoding.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/visitors/exceptions.py` & `django_codemod-2.0.0/src/django_codemod/visitors/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/visitors/forms.py` & `django_codemod-2.0.0/src/django_codemod/visitors/forms.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/visitors/http.py` & `django_codemod-2.0.0/src/django_codemod/visitors/http.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/visitors/models.py` & `django_codemod-2.0.0/src/django_codemod/visitors/models.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/visitors/postgres_fields.py` & `django_codemod-2.0.0/src/django_codemod/visitors/postgres_fields.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/visitors/shortcuts.py` & `django_codemod-2.0.0/src/django_codemod/visitors/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/visitors/signals.py` & `django_codemod-2.0.0/src/django_codemod/visitors/signals.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/visitors/template_context.py` & `django_codemod-2.0.0/src/django_codemod/visitors/template_context.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/visitors/template_tags.py` & `django_codemod-2.0.0/src/django_codemod/visitors/template_tags.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/visitors/timezone.py` & `django_codemod-2.0.0/src/django_codemod/visitors/timezone.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/visitors/translations.py` & `django_codemod-2.0.0/src/django_codemod/visitors/translations.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/src/django_codemod/visitors/urls.py` & `django_codemod-2.0.0/src/django_codemod/visitors/urls.py`

 * *Files identical despite different names*

### Comparing `django-codemod-1.9.1/setup.py` & `django_codemod-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,141 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-codemod
+Version: 2.0.0
+Summary: A command line tool to automatically fix Django deprecations.
+Home-page: https://github.com/browniebroke/django-codemod
+License: MIT
+Keywords: django,codemod,libCST
+Author: Bruno Alla
+Author-email: alla.brunoo@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: click (<9)
+Requires-Dist: libcst (==1.0.1)
+Requires-Dist: pathspec (>=0.6,<1)
+Requires-Dist: rich (>=10)
+Requires-Dist: rich-click (>=1.0)
+Project-URL: Bug Tracker, https://github.com/browniebroke/django-codemod/issues
+Project-URL: Changelog, https://django-codemod.readthedocs.io/en/stable/changelog.html
+Project-URL: Documentation, https://django-codemod.readthedocs.io
+Project-URL: Mastodon, https://fosstodon.org/@browniebroke
+Project-URL: Repository, https://github.com/browniebroke/django-codemod
+Project-URL: Twitter, https://twitter.com/_BrunoAlla
+Description-Content-Type: text/markdown
+
+<p align="center">
+  <img alt="Django Codemod" src="https://raw.githubusercontent.com/browniebroke/django-codemod/main/assets/djangocodemod-stroke.png">
+</p>
+
+<p align="center">
+  <a href="https://github.com/browniebroke/django-codemod/actions/workflows/ci.yml?query=branch%3Amain">
+    <img alt="CI Status" src="https://img.shields.io/github/actions/workflow/status/browniebroke/django-codemod/ci.yml?branch=main&label=CI&logo=github&style=flat-square">
+  </a>
+  <a href="https://django-codemod.readthedocs.io">
+    <img src="https://img.shields.io/readthedocs/django-codemod.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">
+  </a>
+  <a href="https://codecov.io/gh/browniebroke/django-codemod">
+    <img src="https://img.shields.io/codecov/c/github/browniebroke/django-codemod.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
+  </a>
+  <a href="https://results.pre-commit.ci/latest/github/browniebroke/django-codemod/main">
+    <img src="https://results.pre-commit.ci/badge/github/browniebroke/django-codemod/main.svg" alt="pre-commit.ci status">
+  </a>
+</p>
+<p align="center">
+  <a href="https://python-poetry.org/">
+    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">
+  </a>
+  <a href="https://github.com/ambv/black">
+    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?amp;style=flat-square" alt="black">
+  </a>
+  <a href="https://github.com/pre-commit/pre-commit">
+    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">
+  </a>
+</p>
+<p align="center">
+  <a href="https://pypi.org/project/django-codemod/">
+    <img src="https://img.shields.io/pypi/v/django-codemod.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPi Status">
+  </a>
+  <img src="https://img.shields.io/pypi/pyversions/django-codemod.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="pyversions">
+  <img src="https://img.shields.io/pypi/l/django-codemod.svg?style=flat-square" alt="license">
+  <a href="https://github.com/browniebroke/django-codemod">
+    <img src="https://tokei.rs/b1/github/browniebroke/django-codemod/" alt="LoC">
+  </a>
+</p>
+
+A tool to help upgrade Django projects to newer version of the framework by automatically fixing deprecations.
+
+## The problem
+
+When maintaining a Django site, over time you'll find yourself to a point where you'll need to update to the next major version of Django. When Django APIs changes, functions move or are removed, changing usages in your project might add up to many changes. Often these changes are simple to do, but sometimes a simple "find and replace" is not possible.
+
+Take, for instance, the removal of the `url()` function from Django 4.0, to be replaced by `re_path()`. In simple cases, you might even want to switch to `path()`, which has a nicer API. A typical Django project easily has 100's or routes, so this simple decision becomes a much longer task when to be made for each of them.
+
+### This solution
+
+This project solves this problem by providing codemodders for simple changes like this. A codemodder re-writes your code from the old way to the new way.
+
+With the help of AST analysis, we're able to understand what modifications are applicable, remove imports as they become irrelevant, and add missing ones as they are needed.
+
+To continue the example, the tool will look at the route in the `url()` call, and decide whether the regular expression may be replaced by one of the built-in URL converters and use `path()` or stick to a regex and use `re_path()`.
+
+Interested? Check out [the documentation](https://django-codemod.readthedocs.io) for usage and the full list of codemodders.
+
+### What this tool is not
+
+- This tool is best suited for Django sites, NOT for reusable Django applications. The project needs to target a single Django version, e.g. 3.1.x.
+- You do NOT need to install this tool as part of your project dependencies, it is a CLI tool, not a Django package to be installed in your site.
+
+### Similar tools
+
+[django-upgrade](https://github.com/adamchainz/django-upgrade) is a similar tool written by Adam Johnson. It's a reimplementation taking a different approach based only on standard library module.
+
+django-codemod is based on [libCST](https://libcst.readthedocs.io/) (Concrete Syntax Tree) which is a limiting factor in terms of speed. By using standard library modules, django-upgrade is a lot faster and is able to support the latest Python, however it requires Python 3.8+.
+
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tr>
+    <td align="center"><a href="https://browniebroke.com"><img src="https://avatars1.githubusercontent.com/u/861044?v=4?s=80" width="80px;" alt=""/><br /><sub><b>Bruno Alla</b></sub></a><br /><a href="https://github.com/browniebroke/django-codemod/commits?author=browniebroke" title="Code">💻</a> <a href="https://github.com/browniebroke/django-codemod/commits?author=browniebroke" title="Documentation">📖</a> <a href="#ideas-browniebroke" title="Ideas, Planning, & Feedback">🤔</a></td>
+    <td align="center"><a href="https://akx.github.io/"><img src="https://avatars2.githubusercontent.com/u/58669?v=4?s=80" width="80px;" alt=""/><br /><sub><b>Aarni Koskela</b></sub></a><br /><a href="https://github.com/browniebroke/django-codemod/commits?author=akx" title="Code">💻</a> <a href="#ideas-akx" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/browniebroke/django-codemod/commits?author=akx" title="Tests">⚠️</a></td>
+    <td align="center"><a href="https://adamj.eu/"><img src="https://avatars2.githubusercontent.com/u/857609?v=4?s=80" width="80px;" alt=""/><br /><sub><b>Adam Johnson</b></sub></a><br /><a href="https://github.com/browniebroke/django-codemod/commits?author=adamchainz" title="Documentation">📖</a></td>
+    <td align="center"><a href="https://sobolevn.me"><img src="https://avatars1.githubusercontent.com/u/4660275?v=4?s=80" width="80px;" alt=""/><br /><sub><b>Nikita Sobolev</b></sub></a><br /><a href="https://github.com/browniebroke/django-codemod/commits?author=sobolevn" title="Documentation">📖</a></td>
+    <td align="center"><a href="http://www.zapier.com"><img src="https://avatars3.githubusercontent.com/u/21158438?v=4?s=80" width="80px;" alt=""/><br /><sub><b>Chris VanderKolk</b></sub></a><br /><a href="https://github.com/browniebroke/django-codemod/commits?author=cvanderkolk" title="Code">💻</a></td>
+    <td align="center"><a href="https://ghuser.io/jayvdb"><img src="https://avatars1.githubusercontent.com/u/15092?v=4?s=80" width="80px;" alt=""/><br /><sub><b>John Vandenberg</b></sub></a><br /><a href="https://github.com/browniebroke/django-codemod/issues?q=author%3Ajayvdb" title="Bug reports">🐛</a> <a href="https://github.com/browniebroke/django-codemod/commits?author=jayvdb" title="Code">💻</a></td>
+    <td align="center"><a href="https://iamshnoo.github.io/blog/"><img src="https://avatars1.githubusercontent.com/u/45921510?v=4?s=80" width="80px;" alt=""/><br /><sub><b>Anjishnu</b></sub></a><br /><a href="#infra-iamshnoo" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
+  </tr>
+  <tr>
+    <td align="center"><a href="https://github.com/drewbrew"><img src="https://avatars1.githubusercontent.com/u/7773256?v=4?s=80" width="80px;" alt=""/><br /><sub><b>Drew Winstel</b></sub></a><br /><a href="#ideas-drewbrew" title="Ideas, Planning, & Feedback">🤔</a></td>
+    <td align="center"><a href="https://DmytroLitvinov.com"><img src="https://avatars.githubusercontent.com/u/16066485?v=4?s=80" width="80px;" alt=""/><br /><sub><b>Dmytro Litvinov</b></sub></a><br /><a href="https://github.com/browniebroke/django-codemod/commits?author=DmytroLitvinov" title="Documentation">📖</a></td>
+    <td align="center"><a href="https://mzulqarnain1.github.io/"><img src="https://avatars.githubusercontent.com/u/23311265?v=4?s=80" width="80px;" alt=""/><br /><sub><b>M. Zulqarnain</b></sub></a><br /><a href="https://github.com/browniebroke/django-codemod/commits?author=mzulqarnain1" title="Documentation">📖</a></td>
+  </tr>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
+## Credits
+
+This package was created with
+[Cookiecutter](https://github.com/audreyr/cookiecutter) and the
+[audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
+project template.
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['django_codemod', 'django_codemod.utils', 'django_codemod.visitors']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click<9', 'libcst==0.4.1', 'pathspec>=0.6,<1', 'rich-click>=1.0', 'rich<13']
-
-extras_require = \
-{'docs': ['Sphinx>=4.0,<5.0',
-          'sphinx-rtd-theme>=1.0,<2.0',
-          'myst-parser>=0.17.0,<0.18.0']}
-
-entry_points = \
-{'console_scripts': ['djcodemod = django_codemod.cli:djcodemod']}
-
-setup_kwargs = {
-    'name': 'django-codemod',
-    'version': '1.9.1',
-    'description': 'A command line tool to automatically fix Django deprecations.',
-    'long_description': '<p align="center">\n  <img alt="Django Codemod" src="https://raw.githubusercontent.com/browniebroke/django-codemod/main/assets/djangocodemod-stroke.png">\n</p>\n\n<p align="center">\n  <a href="https://github.com/browniebroke/django-codemod/actions?query=workflow%3ACI">\n    <img alt="CI Status" src="https://img.shields.io/github/workflow/status/browniebroke/django-codemod/CI?label=CI&logo=github&style=flat-square">\n  </a>\n  <a href="https://django-codemod.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/django-codemod.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/browniebroke/django-codemod">\n    <img src="https://img.shields.io/codecov/c/github/browniebroke/django-codemod.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n  <a href="https://results.pre-commit.ci/latest/github/browniebroke/django-codemod/main">\n    <img src="https://results.pre-commit.ci/badge/github/browniebroke/django-codemod/main.svg" alt="pre-commit.ci status">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?amp;style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/django-codemod/">\n    <img src="https://img.shields.io/pypi/v/django-codemod.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPi Status">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/django-codemod.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="pyversions">\n  <img src="https://img.shields.io/pypi/l/django-codemod.svg?style=flat-square" alt="license">\n  <a href="https://github.com/browniebroke/django-codemod">\n    <img src="https://tokei.rs/b1/github/browniebroke/django-codemod/" alt="LoC">\n  </a>\n</p>\n\nA tool to help upgrade Django projects to newer version of the framework by automatically fixing deprecations.\n\n## The problem\n\nWhen maintaining a Django site, over time you\'ll find yourself to a point where you\'ll need to update to the next major version of Django. When Django APIs changes, functions move or are removed, changing usages in your project might add up to many changes. Often these changes are simple to do, but sometimes a simple "find and replace" is not possible.\n\nTake, for instance, the removal of the `url()` function from Django 4.0, to be replaced by `re_path()`. In simple cases, you might even want to switch to `path()`, which has a nicer API. A typical Django project easily has 100\'s or routes, so this simple decision becomes a much longer task when to be made for each of them.\n\n### This solution\n\nThis project solves this problem by providing codemodders for simple changes like this. A codemodder re-writes your code from the old way to the new way.\n\nWith the help of AST analysis, we\'re able to understand what modifications are applicable, remove imports as they become irrelevant, and add missing ones as they are needed.\n\nTo continue the example, the tool will look at the route in the `url()` call, and decide whether the regular expression may be replaced by one of the built-in URL converters and use `path()` or stick to a regex and use `re_path()`.\n\nInterested? Check out [the documentation](https://django-codemod.readthedocs.io) for usage and the full list of codemodders.\n\n### What this tool is not\n\n- This tool is best suited for Django sites, NOT for reusable Django applications. The project needs to target a single Django version, e.g. 3.1.x.\n- You do NOT need to install this tool as part of your project dependencies, it is a CLI tool, not a Django package to be installed in your site.\n\n### Similar tools\n\n[django-upgrade](https://github.com/adamchainz/django-upgrade) is a similar tool written by Adam Johnson. It\'s a reimplementation taking a different approach based only on standard library module.\n\ndjango-codemod is based on [libCST](https://libcst.readthedocs.io/) (Concrete Syntax Tree), and it\'s a limiting factor in terms of supported Python versions as well as its speed. By using standard library modules, django-upgrade is a lot faster and is able to support the latest Python, however it requires Python 3.8+.\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tr>\n    <td align="center"><a href="https://browniebroke.com"><img src="https://avatars1.githubusercontent.com/u/861044?v=4?s=80" width="80px;" alt=""/><br /><sub><b>Bruno Alla</b></sub></a><br /><a href="https://github.com/browniebroke/django-codemod/commits?author=browniebroke" title="Code">💻</a> <a href="https://github.com/browniebroke/django-codemod/commits?author=browniebroke" title="Documentation">📖</a> <a href="#ideas-browniebroke" title="Ideas, Planning, & Feedback">🤔</a></td>\n    <td align="center"><a href="https://akx.github.io/"><img src="https://avatars2.githubusercontent.com/u/58669?v=4?s=80" width="80px;" alt=""/><br /><sub><b>Aarni Koskela</b></sub></a><br /><a href="https://github.com/browniebroke/django-codemod/commits?author=akx" title="Code">💻</a> <a href="#ideas-akx" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/browniebroke/django-codemod/commits?author=akx" title="Tests">⚠️</a></td>\n    <td align="center"><a href="https://adamj.eu/"><img src="https://avatars2.githubusercontent.com/u/857609?v=4?s=80" width="80px;" alt=""/><br /><sub><b>Adam Johnson</b></sub></a><br /><a href="https://github.com/browniebroke/django-codemod/commits?author=adamchainz" title="Documentation">📖</a></td>\n    <td align="center"><a href="https://sobolevn.me"><img src="https://avatars1.githubusercontent.com/u/4660275?v=4?s=80" width="80px;" alt=""/><br /><sub><b>Nikita Sobolev</b></sub></a><br /><a href="https://github.com/browniebroke/django-codemod/commits?author=sobolevn" title="Documentation">📖</a></td>\n    <td align="center"><a href="http://www.zapier.com"><img src="https://avatars3.githubusercontent.com/u/21158438?v=4?s=80" width="80px;" alt=""/><br /><sub><b>Chris VanderKolk</b></sub></a><br /><a href="https://github.com/browniebroke/django-codemod/commits?author=cvanderkolk" title="Code">💻</a></td>\n    <td align="center"><a href="https://ghuser.io/jayvdb"><img src="https://avatars1.githubusercontent.com/u/15092?v=4?s=80" width="80px;" alt=""/><br /><sub><b>John Vandenberg</b></sub></a><br /><a href="https://github.com/browniebroke/django-codemod/issues?q=author%3Ajayvdb" title="Bug reports">🐛</a> <a href="https://github.com/browniebroke/django-codemod/commits?author=jayvdb" title="Code">💻</a></td>\n    <td align="center"><a href="https://iamshnoo.github.io/blog/"><img src="https://avatars1.githubusercontent.com/u/45921510?v=4?s=80" width="80px;" alt=""/><br /><sub><b>Anjishnu</b></sub></a><br /><a href="#infra-iamshnoo" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>\n  </tr>\n  <tr>\n    <td align="center"><a href="https://github.com/drewbrew"><img src="https://avatars1.githubusercontent.com/u/7773256?v=4?s=80" width="80px;" alt=""/><br /><sub><b>Drew Winstel</b></sub></a><br /><a href="#ideas-drewbrew" title="Ideas, Planning, & Feedback">🤔</a></td>\n    <td align="center"><a href="https://DmytroLitvinov.com"><img src="https://avatars.githubusercontent.com/u/16066485?v=4?s=80" width="80px;" alt=""/><br /><sub><b>Dmytro Litvinov</b></sub></a><br /><a href="https://github.com/browniebroke/django-codemod/commits?author=DmytroLitvinov" title="Documentation">📖</a></td>\n    <td align="center"><a href="https://mzulqarnain1.github.io/"><img src="https://avatars.githubusercontent.com/u/23311265?v=4?s=80" width="80px;" alt=""/><br /><sub><b>M. Zulqarnain</b></sub></a><br /><a href="https://github.com/browniebroke/django-codemod/commits?author=mzulqarnain1" title="Documentation">📖</a></td>\n  </tr>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)\nproject template.\n',
-    'author': 'Bruno Alla',
-    'author_email': 'alla.brunoo@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/browniebroke/django-codemod',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,72 +1,72 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['django_codemod', 'django_codemod.utils',
-'django_codemod.visitors'] package_data = \ {'': ['*']} install_requires = \
-['click<9', 'libcst==0.4.1', 'pathspec>=0.6,<1', 'rich-click>=1.0', 'rich<13']
-extras_require = \ {'docs': ['Sphinx>=4.0,<5.0', 'sphinx-rtd-theme>=1.0,<2.0',
-'myst-parser>=0.17.0,<0.18.0']} entry_points = \ {'console_scripts':
-['djcodemod = django_codemod.cli:djcodemod']} setup_kwargs = { 'name': 'django-
-codemod', 'version': '1.9.1', 'description': 'A command line tool to
-automatically fix Django deprecations.', 'long_description': '
-                             \n [Django Codemod]\n
-\n\n
-     \n \n_[CI_Status]\n\n \n_[Documentation_Status]\n\n \n_[Test_coverage
-                 percentage]\n\n \n_[pre-commit.ci_status]\n\n
-\n
-             \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
-\n
-        \n \n_[PyPi_Status]\n\n [pyversions]\n [license]\n \n_[LoC]\n\n
-\n\nA tool to help upgrade Django projects to newer version of the framework by
-automatically fixing deprecations.\n\n## The problem\n\nWhen maintaining a
-Django site, over time you\'ll find yourself to a point where you\'ll need to
-update to the next major version of Django. When Django APIs changes, functions
-move or are removed, changing usages in your project might add up to many
-changes. Often these changes are simple to do, but sometimes a simple "find and
-replace" is not possible.\n\nTake, for instance, the removal of the `url()`
-function from Django 4.0, to be replaced by `re_path()`. In simple cases, you
-might even want to switch to `path()`, which has a nicer API. A typical Django
-project easily has 100\'s or routes, so this simple decision becomes a much
-longer task when to be made for each of them.\n\n### This solution\n\nThis
-project solves this problem by providing codemodders for simple changes like
-this. A codemodder re-writes your code from the old way to the new way.\n\nWith
-the help of AST analysis, we\'re able to understand what modifications are
-applicable, remove imports as they become irrelevant, and add missing ones as
-they are needed.\n\nTo continue the example, the tool will look at the route in
-the `url()` call, and decide whether the regular expression may be replaced by
-one of the built-in URL converters and use `path()` or stick to a regex and use
-`re_path()`.\n\nInterested? Check out [the documentation](https://django-
-codemod.readthedocs.io) for usage and the full list of codemodders.\n\n### What
-this tool is not\n\n- This tool is best suited for Django sites, NOT for
-reusable Django applications. The project needs to target a single Django
-version, e.g. 3.1.x.\n- You do NOT need to install this tool as part of your
-project dependencies, it is a CLI tool, not a Django package to be installed in
-your site.\n\n### Similar tools\n\n[django-upgrade](https://github.com/
-adamchainz/django-upgrade) is a similar tool written by Adam Johnson. It\'s a
-reimplementation taking a different approach based only on standard library
-module.\n\ndjango-codemod is based on [libCST](https://libcst.readthedocs.io/)
-(Concrete Syntax Tree), and it\'s a limiting factor in terms of supported
-Python versions as well as its speed. By using standard library modules,
-django-upgrade is a lot faster and is able to support the latest Python,
-however it requires Python 3.8+.\n\n## Contributors â¨\n\nThanks goes to these
-wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
-\n\n\n\n\n
+Metadata-Version: 2.1 Name: django-codemod Version: 2.0.0 Summary: A command
+line tool to automatically fix Django deprecations. Home-page: https://
+github.com/browniebroke/django-codemod License: MIT Keywords:
+django,codemod,libCST Author: Bruno Alla Author-email: alla.brunoo@gmail.com
+Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
+Approved :: MIT License Classifier: Natural Language :: English Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Software Development :: Libraries Requires-Dist: click (<9) Requires-Dist:
+libcst (==1.0.1) Requires-Dist: pathspec (>=0.6,<1) Requires-Dist: rich (>=10)
+Requires-Dist: rich-click (>=1.0) Project-URL: Bug Tracker, https://github.com/
+browniebroke/django-codemod/issues Project-URL: Changelog, https://django-
+codemod.readthedocs.io/en/stable/changelog.html Project-URL: Documentation,
+https://django-codemod.readthedocs.io Project-URL: Mastodon, https://
+fosstodon.org/@browniebroke Project-URL: Repository, https://github.com/
+browniebroke/django-codemod Project-URL: Twitter, https://twitter.com/
+_BrunoAlla Description-Content-Type: text/markdown
+                               [Django Codemod]
+ [CI_Status] [Documentation_Status] [Test_coverage_percentage] [pre-commit.ci
+                                    status]
+                         [Poetry] [black] [pre-commit]
+                  [PyPi_Status] [pyversions] [license] [LoC]
+A tool to help upgrade Django projects to newer version of the framework by
+automatically fixing deprecations. ## The problem When maintaining a Django
+site, over time you'll find yourself to a point where you'll need to update to
+the next major version of Django. When Django APIs changes, functions move or
+are removed, changing usages in your project might add up to many changes.
+Often these changes are simple to do, but sometimes a simple "find and replace"
+is not possible. Take, for instance, the removal of the `url()` function from
+Django 4.0, to be replaced by `re_path()`. In simple cases, you might even want
+to switch to `path()`, which has a nicer API. A typical Django project easily
+has 100's or routes, so this simple decision becomes a much longer task when to
+be made for each of them. ### This solution This project solves this problem by
+providing codemodders for simple changes like this. A codemodder re-writes your
+code from the old way to the new way. With the help of AST analysis, we're able
+to understand what modifications are applicable, remove imports as they become
+irrelevant, and add missing ones as they are needed. To continue the example,
+the tool will look at the route in the `url()` call, and decide whether the
+regular expression may be replaced by one of the built-in URL converters and
+use `path()` or stick to a regex and use `re_path()`. Interested? Check out
+[the documentation](https://django-codemod.readthedocs.io) for usage and the
+full list of codemodders. ### What this tool is not - This tool is best suited
+for Django sites, NOT for reusable Django applications. The project needs to
+target a single Django version, e.g. 3.1.x. - You do NOT need to install this
+tool as part of your project dependencies, it is a CLI tool, not a Django
+package to be installed in your site. ### Similar tools [django-upgrade](https:
+//github.com/adamchainz/django-upgrade) is a similar tool written by Adam
+Johnson. It's a reimplementation taking a different approach based only on
+standard library module. django-codemod is based on [libCST](https://
+libcst.readthedocs.io/) (Concrete Syntax Tree) which is a limiting factor in
+terms of speed. By using standard library modules, django-upgrade is a lot
+faster and is able to support the latest Python, however it requires Python
+3.8+. ## Contributors â¨ Thanks goes to these wonderful people ([emoji key]
+(https://allcontributors.org/docs/en/emoji-key)):
 
         Bruno_Alla                 Aarni_Koskela             Adam     Nikita    Chris     John_Vandenberg  Anjishnu
                                                            Johnson   Sobolev  VanderKolk
       ð» ð ð�       ð» ð¤ â                                    ð ð�  ð
                                                              ð  ð�   ð»
 
           Drew_Winstel                Dmytro_Litvinov         M.
                                                           Zulqarnain
               ð¤                      ð
                                                              ð
-\n\n\n\n\n\n\nThis project follows the [all-contributors](https://github.com/
-all-contributors/all-contributors) specification. Contributions of any kind
-welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https:/
-/github.com/audreyr/cookiecutter) and the\n[audreyr/cookiecutter-pypackage]
-(https://github.com/audreyr/cookiecutter-pypackage)\nproject template.\n',
-'author': 'Bruno Alla', 'author_email': 'alla.brunoo@gmail.com', 'maintainer':
-None, 'maintainer_email': None, 'url': 'https://github.com/browniebroke/django-
-codemod', 'package_dir': package_dir, 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'extras_require':
-extras_require, 'entry_points': entry_points, 'python_requires': '>=3.7,<4.0',
-} setup(**setup_kwargs)
+   This project follows the [all-contributors](https://github.com/all-
+contributors/all-contributors) specification. Contributions of any kind
+welcome! ## Credits This package was created with [Cookiecutter](https://
+github.com/audreyr/cookiecutter) and the [audreyr/cookiecutter-pypackage]
+(https://github.com/audreyr/cookiecutter-pypackage) project template.
```

