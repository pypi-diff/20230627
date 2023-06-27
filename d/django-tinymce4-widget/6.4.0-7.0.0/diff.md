# Comparing `tmp/django-tinymce4-widget-6.4.0.tar.gz` & `tmp/django_tinymce4_widget-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tinymce4-widget-6.4.0.tar", max compression
+gzip compressed data, was "django_tinymce4_widget-7.0.0.tar", max compression
```

## Comparing `django-tinymce4-widget-6.4.0.tar` & `django_tinymce4_widget-7.0.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1199 2022-08-24 10:20:43.260896 django-tinymce4-widget-6.4.0/LICENSE.txt
--rw-r--r--   0        0        0     4469 2022-08-24 10:20:43.260896 django-tinymce4-widget-6.4.0/README.md
--rw-r--r--   0        0        0     2496 2022-08-24 10:20:44.112906 django-tinymce4-widget-6.4.0/pyproject.toml
--rw-r--r--   0        0        0      367 2022-08-24 10:20:44.064905 django-tinymce4-widget-6.4.0/src/tinymce/__init__.py
--rw-r--r--   0        0        0       89 2022-08-24 10:20:43.264896 django-tinymce4-widget-6.4.0/src/tinymce/apps.py
--rw-r--r--   0        0        0      990 2022-08-24 10:20:43.264896 django-tinymce4-widget-6.4.0/src/tinymce/models.py
--rw-r--r--   0        0        0     1511 2022-08-24 10:20:43.264896 django-tinymce4-widget-6.4.0/src/tinymce/settings.py
--rw-r--r--   0        0        0      465 2022-08-24 10:20:43.264896 django-tinymce4-widget-6.4.0/src/tinymce/templates/tinymce/spellchecker.js
--rw-r--r--   0        0        0      165 2022-08-24 10:20:43.264896 django-tinymce4-widget-6.4.0/src/tinymce/templates/tinymce/tinymce4.css
--rw-r--r--   0        0        0      165 2022-08-24 10:20:43.264896 django-tinymce4-widget-6.4.0/src/tinymce/templates/tinymce/tinymce_init.js
--rw-r--r--   0        0        0      197 2022-08-24 10:20:43.264896 django-tinymce4-widget-6.4.0/src/tinymce/urls.py
--rw-r--r--   0        0        0     2349 2022-08-24 10:20:43.264896 django-tinymce4-widget-6.4.0/src/tinymce/views.py
--rw-r--r--   0        0        0     5392 2022-08-24 10:20:43.264896 django-tinymce4-widget-6.4.0/src/tinymce/widgets.py
--rw-r--r--   0        0        0     5614 2022-08-24 10:20:52.807052 django-tinymce4-widget-6.4.0/setup.py
--rw-r--r--   0        0        0     6472 2022-08-24 10:20:52.807431 django-tinymce4-widget-6.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1199 2023-06-27 14:03:04.930237 django_tinymce4_widget-7.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     4510 2023-06-27 14:03:04.930237 django_tinymce4_widget-7.0.0/README.md
+-rw-r--r--   0        0        0     2335 2023-06-27 14:03:06.158247 django_tinymce4_widget-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0      367 2023-06-27 14:03:06.118247 django_tinymce4_widget-7.0.0/src/tinymce/__init__.py
+-rw-r--r--   0        0        0       89 2023-06-27 14:03:04.934237 django_tinymce4_widget-7.0.0/src/tinymce/apps.py
+-rw-r--r--   0        0        0      990 2023-06-27 14:03:04.934237 django_tinymce4_widget-7.0.0/src/tinymce/models.py
+-rw-r--r--   0        0        0     1511 2023-06-27 14:03:04.934237 django_tinymce4_widget-7.0.0/src/tinymce/settings.py
+-rw-r--r--   0        0        0      465 2023-06-27 14:03:04.934237 django_tinymce4_widget-7.0.0/src/tinymce/templates/tinymce/spellchecker.js
+-rw-r--r--   0        0        0      165 2023-06-27 14:03:04.934237 django_tinymce4_widget-7.0.0/src/tinymce/templates/tinymce/tinymce4.css
+-rw-r--r--   0        0        0      165 2023-06-27 14:03:04.934237 django_tinymce4_widget-7.0.0/src/tinymce/templates/tinymce/tinymce_init.js
+-rw-r--r--   0        0        0      197 2023-06-27 14:03:04.934237 django_tinymce4_widget-7.0.0/src/tinymce/urls.py
+-rw-r--r--   0        0        0     2349 2023-06-27 14:03:04.934237 django_tinymce4_widget-7.0.0/src/tinymce/views.py
+-rw-r--r--   0        0        0     5392 2023-06-27 14:03:04.934237 django_tinymce4_widget-7.0.0/src/tinymce/widgets.py
+-rw-r--r--   0        0        0     6239 1970-01-01 00:00:00.000000 django_tinymce4_widget-7.0.0/PKG-INFO
```

### Comparing `django-tinymce4-widget-6.4.0/LICENSE.txt` & `django_tinymce4_widget-7.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-tinymce4-widget-6.4.0/README.md` & `django_tinymce4_widget-7.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # django-tinymce4-widget
 
 <p align="center">
-  <a href="https://github.com/browniebroke/django-tinymce4-widget/actions?query=workflow%3ACI">
-    <img alt="CI Status" src="https://img.shields.io/github/workflow/status/browniebroke/django-tinymce4-widget/CI?label=CI&logo=github&style=flat-square">
+  <a href="https://github.com/browniebroke/django-tinymce4-widget/actions/workflows/ci.yml?query=branch%3Amain">
+    <img alt="CI Status" src="https://img.shields.io/github/actions/workflow/status/browniebroke/django-tinymce4-widget/ci.yml?branch=main&label=CI&logo=github&style=flat-square">
   </a>
   <a href="https://django-tinymce4-widget.readthedocs.io">
     <img src="https://img.shields.io/readthedocs/django-tinymce4-widget.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">
   </a>
   <a href="https://codecov.io/gh/browniebroke/django-tinymce4-widget">
     <img src="https://img.shields.io/codecov/c/github/browniebroke/django-tinymce4-widget.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage">
   </a>
@@ -37,16 +37,16 @@
 
 This version **does not** include any static files, it's using the TinyMCE from the CDN by default.
 
 **Warning**: TinyMCE 4 is incompatible with TinyMCE 3. Read [TinyMCE](https://www.tinymce.com/) docs for more information about how to configure TimyMCE 4 editor widget.
 
 ## Compatibility
 
-- **Python**: 3.7-3.10
-- **Django**: 2.2-4.1
+- **Python**: 3.8-3.11
+- **Django**: 3.2-4.2
 
 ## Quick Start
 
 Install `django-tinymce4-widget`:
 
     $ pip install django-tinymce4-widget
```

### Comparing `django-tinymce4-widget-6.4.0/pyproject.toml` & `django_tinymce4_widget-7.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,64 +1,60 @@
 [tool.poetry]
 name = "django-tinymce4-widget"
-version = "6.4.0"
+version = "7.0.0"
 description = "A Django application that provides a TinyMCE 4 editor widget without any static files"
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["django", "wysiwyg", "widget", "tinymce"]
 repository = "https://github.com/browniebroke/django-tinymce4-widget"
 documentation = "https://django-tinymce4-widget.readthedocs.io"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Framework :: Django",
-    "Framework :: Django :: 2.2",
-    "Framework :: Django :: 3.0",
-    "Framework :: Django :: 3.1",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Text Editors",
     "Topic :: Text Processing",
     "Topic :: Text Processing :: Markup",
     "Topic :: Text Processing :: Markup :: HTML",
 ]
 packages = [
     { include = "tinymce", from = "src" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-Django = ">=2.2,<4.2"
+python = "^3.8"
+Django = ">=3.2,<5.0"
 pyenchant = { version = "^3.1", optional = true }
 
-# Docs deps
-Sphinx = { version = "^5.0", optional = true }
-sphinx-rtd-theme = { version = "^1.0", optional = true }
-myst-parser = { version = "^0.18.0", optional = true }
-
 [tool.poetry.extras]
-docs = [
-    "myst-parser",
-    "sphinx",
-    "sphinx-rtd-theme",
-]
 spellcheck = ["pyenchant"]
 
 [tool.poetry.dev-dependencies]
-coverage = { version = "^6.0", extras = ["toml"] }
+coverage = { version = "^7.0", extras = ["toml"] }
 pytest = "^7.0"
 pytest-django = "^4.5"
-pytest-cov = "^3.0"
+pytest-cov = "^4.0"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+myst-parser = ">=2.0"
+sphinx = ">=6.0"
+sphinx-rtd-theme = ">=1.0"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/tinymce/__init__.py:__version__"
 build_command = "pip install poetry && poetry build"
```

### Comparing `django-tinymce4-widget-6.4.0/src/tinymce/models.py` & `django_tinymce4_widget-7.0.0/src/tinymce/models.py`

 * *Files identical despite different names*

### Comparing `django-tinymce4-widget-6.4.0/src/tinymce/settings.py` & `django_tinymce4_widget-7.0.0/src/tinymce/settings.py`

 * *Files identical despite different names*

### Comparing `django-tinymce4-widget-6.4.0/src/tinymce/views.py` & `django_tinymce4_widget-7.0.0/src/tinymce/views.py`

 * *Files identical despite different names*

### Comparing `django-tinymce4-widget-6.4.0/src/tinymce/widgets.py` & `django_tinymce4_widget-7.0.0/src/tinymce/widgets.py`

 * *Files identical despite different names*

### Comparing `django-tinymce4-widget-6.4.0/PKG-INFO` & `django_tinymce4_widget-7.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,51 @@
 Metadata-Version: 2.1
 Name: django-tinymce4-widget
-Version: 6.4.0
+Version: 7.0.0
 Summary: A Django application that provides a TinyMCE 4 editor widget without any static files
 Home-page: https://github.com/browniebroke/django-tinymce4-widget
 License: MIT
 Keywords: django,wysiwyg,widget,tinymce
 Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Editors
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Text Processing :: Markup :: HTML
-Provides-Extra: docs
 Provides-Extra: spellcheck
-Requires-Dist: Django (>=2.2,<4.2)
-Requires-Dist: Sphinx (>=5.0,<6.0); extra == "docs"
-Requires-Dist: myst-parser (>=0.18.0,<0.19.0); extra == "docs"
-Requires-Dist: pyenchant (>=3.1,<4.0); extra == "spellcheck"
-Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0); extra == "docs"
+Requires-Dist: Django (>=3.2,<5.0)
+Requires-Dist: pyenchant (>=3.1,<4.0) ; extra == "spellcheck"
 Project-URL: Documentation, https://django-tinymce4-widget.readthedocs.io
 Project-URL: Repository, https://github.com/browniebroke/django-tinymce4-widget
 Description-Content-Type: text/markdown
 
 # django-tinymce4-widget
 
 <p align="center">
-  <a href="https://github.com/browniebroke/django-tinymce4-widget/actions?query=workflow%3ACI">
-    <img alt="CI Status" src="https://img.shields.io/github/workflow/status/browniebroke/django-tinymce4-widget/CI?label=CI&logo=github&style=flat-square">
+  <a href="https://github.com/browniebroke/django-tinymce4-widget/actions/workflows/ci.yml?query=branch%3Amain">
+    <img alt="CI Status" src="https://img.shields.io/github/actions/workflow/status/browniebroke/django-tinymce4-widget/ci.yml?branch=main&label=CI&logo=github&style=flat-square">
   </a>
   <a href="https://django-tinymce4-widget.readthedocs.io">
     <img src="https://img.shields.io/readthedocs/django-tinymce4-widget.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">
   </a>
   <a href="https://codecov.io/gh/browniebroke/django-tinymce4-widget">
     <img src="https://img.shields.io/codecov/c/github/browniebroke/django-tinymce4-widget.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage">
   </a>
@@ -82,16 +76,16 @@
 
 This version **does not** include any static files, it's using the TinyMCE from the CDN by default.
 
 **Warning**: TinyMCE 4 is incompatible with TinyMCE 3. Read [TinyMCE](https://www.tinymce.com/) docs for more information about how to configure TimyMCE 4 editor widget.
 
 ## Compatibility
 
-- **Python**: 3.7-3.10
-- **Django**: 2.2-4.1
+- **Python**: 3.8-3.11
+- **Django**: 3.2-4.2
 
 ## Quick Start
 
 Install `django-tinymce4-widget`:
 
     $ pip install django-tinymce4-widget
```

