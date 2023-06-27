# Comparing `tmp/flask-marshmallow-openapi-0.2.0.tar.gz` & `tmp/flask-marshmallow-openapi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-marshmallow-openapi-0.2.0.tar", last modified: Mon Jun 26 06:32:58 2023, max compression
+gzip compressed data, was "flask-marshmallow-openapi-0.3.0.tar", last modified: Tue Jun 27 07:17:47 2023, max compression
```

## Comparing `flask-marshmallow-openapi-0.2.0.tar` & `flask-marshmallow-openapi-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:58.045611 flask-marshmallow-openapi-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-26 06:32:58.045611 flask-marshmallow-openapi-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 06:32:58.045611 flask-marshmallow-openapi-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:58.037611 flask-marshmallow-openapi-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:58.037611 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:58.037611 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/redoc_favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:58.045611 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
--rw-r--r--   0 runner    (1001) docker     (123)  1045708 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   368781 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
--rw-r--r--   0 runner    (1001) docker     (123)  1045498 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   322863 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
--rw-r--r--   0 runner    (1001) docker     (123)   145206 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)   256702 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:58.045611 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/templates/re_doc.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:58.037611 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-26 06:32:58.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-26 06:32:58.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 06:32:58.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 06:32:57.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-26 06:32:58.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-26 06:32:58.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:47.906424 flask-marshmallow-openapi-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-06-27 07:17:47.906424 flask-marshmallow-openapi-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:17:47.906424 flask-marshmallow-openapi-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:47.898424 flask-marshmallow-openapi-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:47.898424 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:47.898424 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/decorators/decorate_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/decorators/decorate_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/decorators/decorate_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/decorators/decorate_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/decorators/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/flask_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/schemas_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/securities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:47.902423 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/redoc_favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:47.906424 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1045708 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   368781 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1045498 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   322863 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
+-rw-r--r--   0 runner    (1001) docker     (123)   145206 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)   256702 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:47.906424 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/templates/re_doc.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-27 07:17:37.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:17:47.898424 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-06-27 07:17:47.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-27 07:17:47.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:17:47.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:17:47.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-27 07:17:47.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 07:17:47.000000 flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi.egg-info/top_level.txt
```

### Comparing `flask-marshmallow-openapi-0.2.0/.gitignore` & `flask-marshmallow-openapi-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.2.0/LICENSE` & `flask-marshmallow-openapi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.2.0/MANIFEST.in` & `flask-marshmallow-openapi-0.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.2.0/pyproject.toml` & `flask-marshmallow-openapi-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=65", "wheel"]
+requires = ["setuptools >= 65", "wheel"]
 
 
 [project]
 name = "flask-marshmallow-openapi"
-version = "0.2.0"
+version = "0.3.0"
 description = "Flask + marshmallow + OpenAPI"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
@@ -18,37 +18,39 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
 keywords = ["OpenAPI SwaggerUI ReDoc"]
 license = { text = "MIT" }
 authors = [{ name = "Tomislav Adamic", email = "tomislav.adamic@gmail.com" }]
 dependencies = [
-    "wrapt",
-    "pyyaml",
+    "apispec[yaml,marshmallow]",
     "flask >= 2.3.0",
+    "inflection",
     "marshmallow >= 3.18.0",
-    "apispec[yaml,marshmallow]",
+    "pyyaml",
+    "requests",
+    "wrapt",
+    "openapi-pydantic-models >= 0.2.0",
 ]
 
 
 [project.urls]
 Source = "https://github.com/tadams42/flask-marshmallow-openapi"
 
 
 [project.optional-dependencies]
 # For dev machines
 dev = [
-    "ipython>=8.6.0",
     "black >= 22.1.0",
     "bump2version >= 1.0.1",
     "check-manifest >= 0.47",
+    "flask-shell-ipython >= 0.5.1",
+    "ipython >= 8.6.0",
     "isort >= 5.10.1",
     "pip-tools >= 6.5.1",
-    "flask-shell-ipython>=0.5.1",
-    "inflection",
 ]
 # For dev machines and CI generating docs
 docs = [
     "furo",
     "myst-parser",
     "sphinx > 5.2.0",
     "sphinx_rtd_theme",
@@ -57,17 +59,17 @@
 # For dev machines and CI running tests
 tests = [
     "coverage",
     "factory-boy >= 3.2.1",
     "faker >= 12.3.0",
     "lorem >= 0.1.1",
     "pytest >= 7.0.1",
-    "pytest-spec >= 3.2.0",
     "pytest-profiling >= 1.7.0",
-    "pytest-random-order>=1.0.4",
+    "pytest-random-order >= 1.0.4",
+    "pytest-spec >= 3.2.0",
 ]
 
 
 [tool.setuptools]
 zip-safe = false
 platforms = ["any"]
 include-package-data = true
```

### Comparing `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/helpers.py` & `flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/schemas_registry.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,88 +1,95 @@
 import importlib
 import inspect
-from typing import Optional, Set, Tuple, Type, Union
+from typing import Type
 
-import marshmallow
+import marshmallow as ma
 
+_KNOWN_SCHEMAS: dict[str, Type[ma.Schema]] = dict()
 
-def schema_ref(schema: Union[str, Type[marshmallow.Schema]]) -> str:
-    return f"#/components/schemas/{schema_name(schema)}"
 
+class SchemasRegistry:
+    @classmethod
+    def schema_ref(cls, schema: str | Type[ma.Schema]) -> str:
+        return f"#/components/schemas/{cls.schema_name(schema)}"
 
-def schema_name(schema: Union[str, Type[marshmallow.Schema]]) -> Optional[str]:
-    if schema:
+    @classmethod
+    def schema_name(cls, schema: str | Type[ma.Schema]) -> str:
         return (schema if isinstance(schema, str) else schema.__name__).replace(
             "Schema", ""
         )
-    else:
-        return None
 
+    @classmethod
+    def all_schemas(cls) -> dict[str, Type[ma.Schema]]:
+        return _KNOWN_SCHEMAS
 
-_KNOWN_SCHEMAS: Set[Tuple[str, Type[marshmallow.Schema]]] = set()
-
-
-def all_schemas() -> Set[Tuple[str, Type[marshmallow.Schema]]]:
-    return _KNOWN_SCHEMAS
-
-
-def main_schema_cls(
-    other_schema: Union[str, marshmallow.Schema]
-) -> Type[marshmallow.Schema]:
-    """
-    Given ie. class FooCreateSchema or name "FooCreateSchema", returns class FooSchema.
-    """
-    try:
-        other_schema = other_schema.__name__
-    except AttributeError:
-        pass
-
-    other_schema = other_schema.replace("Create", "").replace("Update", "")
-
-    retv = next((_[1] for _ in all_schemas() if _[1].__name__ == other_schema), None)
-
-    if not retv:
-        raise RuntimeError(f"Couldn't find main schema for {other_schema}!")
-
-    return retv
+    @classmethod
+    def main_schema_cls(
+        cls, other_schema: str | ma.Schema | Type[ma.Schema]
+    ) -> Type[ma.Schema]:
+        """
+        Given ie. class FooCreateSchema or name "FooCreateSchema", returns class
+        FooSchema.
+        """
+        name = None
+        if isinstance(other_schema, ma.Schema):
+            name = other_schema.__class__.__name__
+        elif isinstance(other_schema, str):
+            name = other_schema
+        else:
+            try:
+                name = other_schema.__name__
+            except AttributeError:
+                pass
+
+        if not name:
+            raise TypeError(f"Couldn't find schema name for {other_schema}!")
+
+        name = name.replace("Create", "").replace("Update", "")
+        retv = _KNOWN_SCHEMAS.get(name, None)
+        if not retv:
+            raise RuntimeError(f"Couldn't find main schema for {other_schema}!")
+
+        return retv
+
+    @classmethod
+    def find_all_schemas(cls, app_package_name: str) -> dict[str, Type[ma.Schema]]:
+        global _KNOWN_SCHEMAS
+
+        if _KNOWN_SCHEMAS:
+            return _KNOWN_SCHEMAS
+
+        modules = [
+            _[1]
+            for _ in inspect.getmembers(
+                importlib.import_module(".", app_package_name), inspect.ismodule
+            )
+        ]
 
+        clss = {
+            _[1]
+            for _ in inspect.getmembers(
+                importlib.import_module(".", app_package_name), inspect.isclass
+            )
+        }
 
-def find_all_schemas(
-    app_package_name: str,
-) -> Set[Tuple[str, Type[marshmallow.Schema]]]:
-    global _KNOWN_SCHEMAS
+        for klass in {
+            _
+            for module_ in modules
+            for name, _ in inspect.getmembers(module_, inspect.isclass)
+        }.union(clss):
+            if (
+                issubclass(klass, ma.Schema)
+                and klass.__name__ != "Schema"
+                and klass.__name__ != "JsonApiSchema"
+            ):
+                _KNOWN_SCHEMAS[cls.schema_name(klass)] = klass
 
-    if _KNOWN_SCHEMAS:
         return _KNOWN_SCHEMAS
 
-    modules = [
-        _[1]
-        for _ in inspect.getmembers(
-            importlib.import_module(".", app_package_name), inspect.ismodule
-        )
-    ]
-
-    clss = {
-        _[1]
-        for _ in inspect.getmembers(
-            importlib.import_module(".", app_package_name), inspect.isclass
-        )
-    }
-
-    for klass in {
-        _
-        for module_ in modules
-        for name, _ in inspect.getmembers(module_, inspect.isclass)
-    }.union(clss):
-        if (
-            issubclass(klass, marshmallow.Schema)
-            and klass.__name__ != "Schema"
-            and klass.__name__ != "JsonApiSchema"
-        ):
-            _KNOWN_SCHEMAS.add(
-                (
-                    schema_name(klass),
-                    klass,
-                )
-            )
 
-    return _KNOWN_SCHEMAS
+def main_schema_cls(other_schema: str | ma.Schema) -> Type[ma.Schema]:
+    """
+    Given ie. class FooCreateSchema or name "FooCreateSchema", returns class
+    FooSchema.
+    """
+    return SchemasRegistry.main_schema_cls(other_schema)
```

### Comparing `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/middleware.py` & `flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from __future__ import annotations
-
 import json
 import os
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Callable, Optional
+from typing import Callable
 
 import apispec
 import flask
 import requests
 from apispec.exceptions import DuplicateComponentNameError
 from apispec.ext.marshmallow import MarshmallowPlugin
 
-from . import decorators, helpers
+from .flask_paths import FlaskPathsManager
+from .schemas_registry import SchemasRegistry
 from .static_collector import StaticResourcesCollector
 
 _MINIMAL_SPEC = {"title": "Some API", "openapi_version": "3.0.2", "version": "v1"}
 
 
 @dataclass
 class OpenAPISettings:
@@ -108,65 +107,66 @@
     +--------------------------+--------+------------------------------------------------+
     | open_api.changelog       | GET    | /{self.mounted_at}/docs/changelog              |
     +--------------------------+--------+------------------------------------------------+
     | open_api.static          | GET    | /{self.mounted_at}/docs/static/<path:filename> |
     +--------------------------+--------+------------------------------------------------+
     """
 
-    def __init__(self, config: OpenAPISettings, app: Optional[flask.Flask] = None):
+    def __init__(self, config: OpenAPISettings, app: flask.Flask | None = None):
         self._apispec = None
         self.blueprint = flask.Blueprint(
             name="open_api",
             import_name=__name__,
             url_prefix="/docs",
             template_folder="./templates",
             static_folder="./static",
         )
         self.config = config
         if app:
             self.init_app(app)
 
     def init_app(self, app: flask.Flask):
-        self._add_own_endpoints(app)
+        self._add_own_endpoints()
 
         full_url_prefix = (
             Path(self.config.mounted_at or "/") / f"./{self.blueprint.url_prefix}"
         )
 
         with app.test_request_context():
-            helpers.find_all_schemas(self.config.app_package_name)
+            SchemasRegistry.find_all_schemas(self.config.app_package_name)
 
             initial_swagger_json: dict = _MINIMAL_SPEC
             if self.config.swagger_json_template_loader:
                 if self.config.swagger_json_template_loader_kwargs:
                     initial_swagger_json = self.config.swagger_json_template_loader(
                         **self.config.swagger_json_template_loader_kwargs
                     )
                 else:
                     initial_swagger_json = self.config.swagger_json_template_loader()
 
             self._apispec = apispec.APISpec(
                 plugins=[MarshmallowPlugin()], **(initial_swagger_json)
             )
-            for name, klass in helpers.all_schemas():
+            for name, klass in SchemasRegistry.all_schemas().items():
                 # apispec automatically registers all nested schema so we must prevent
                 # registering them ourselves because of DuplicateSchemaError
                 x_tags = getattr(klass.opts, "x_tags", None)
 
                 try:
                     if x_tags:
                         self._apispec.components.schema(
                             name, component={"x-tags": x_tags}, schema=klass
                         )
                     else:
                         self._apispec.components.schema(name, schema=klass)
                 except DuplicateComponentNameError:
                     pass
 
-            self._collect_endpoints_docs(app)
+            for path, operations in FlaskPathsManager(app).collect_endpoints_docs():
+                self._apispec.path(path=path, operations=operations.dict())
 
         app.register_blueprint(self.blueprint, url_prefix=str(full_url_prefix))
 
         if not hasattr(app, "extensions"):
             app.extensions = {}
         # app.extensions["open_api"] = self
 
@@ -200,25 +200,25 @@
         if oauth_config:
             fields["oauth_config_json"] = json.dumps(oauth_config)
 
         fields["api_name"] = self.config.api_name
 
         return fields
 
-    def _add_own_endpoints(self, app):
+    def _add_own_endpoints(self):
         # How this stuff works?
         #
         # On development machines, these endpoints will be handled by supplied lambdas.
         # This is inefficient and slow, but it always serves latest data for "static"
         # content (ie. "swagger.json", "CHANGELOG.md") without the need to reload
         # development server.
         #
-        # On deployed machines, we put reverse proxy in front of Flask app.
-        # We configure reverse proxy to rewrite request some URLs and point then onto
-        # static files that are generated once, during deployment.
+        # On deployed machines, we put reverse proxy in front of Flask app. We configure
+        # reverse proxy to rewrite request static URLs and point them onto static files
+        # that are generated once, during deployment.
         #
         # For example, request `GET /v1/docs/re_doc` will:
         #
         #   - on development machine will hit one of lambdas below
         #   - on deployed server, we will have generated `/foo/bar/static/re_doc.html`
         #     and configured reverse proxy to rewrite original request into
         #     `GET /static/re_doc.html`.
@@ -285,25 +285,7 @@
     @property
     def _to_dict(self):
         return self._apispec.to_dict()
 
     @property
     def _to_yaml(self):
         return self._apispec.to_yaml()
-
-    def _should_document_enpdpoint(self, name: str):
-        # Reduce spam in docs
-        return (
-            "_relationships_" not in name
-            and ".docs." not in name
-            and "static" not in name
-        )
-
-    def _collect_endpoints_docs(self, app):
-        for rule in app.url_map.iter_rules():
-            if self._should_document_enpdpoint(rule.endpoint):
-                open_api_path = decorators.path_for(app, rule)
-                if open_api_path:
-                    self._apispec.path(
-                        path=open_api_path["path"],
-                        operations=open_api_path["operations"],
-                    )
```

### Comparing `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/redoc_favicon.png` & `flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/redoc_favicon.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png` & `flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png` & `flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/index.html` & `flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/index.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html` & `flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js` & `flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js` & `flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js` & `flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js` & `flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js` & `flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css` & `flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js` & `flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static_collector.py` & `flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/static_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import hashlib
 import json
 import os
 import shutil
 from pathlib import Path
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING
 
 import flask
 from flask import current_app
 
 if TYPE_CHECKING:
-    from .open_api import OpenAPI
+    from .middleware import OpenAPI
 
 # TODO: This shouldn't be needed once we can fully rely on importlib.resources
 _SELF_PATH = Path(os.path.abspath(os.path.dirname(__file__)))
 
 
 class StaticResourcesCollector:
     def __init__(self, open_api: OpenAPI, destination_dir: str | Path):
@@ -92,15 +92,15 @@
 
     def _copy_src_static_folder(self):
         # TODO: "../static/" should really be handled by importlib.resources but that
         # doesn't support extracting directories from package, only individual files.
         shutil.copytree(_SELF_PATH / "static", self.docs_static, dirs_exist_ok=True)
 
 
-def _file_checksum(file_path: Union[str, Path], hashlib_callable):
+def _file_checksum(file_path: str | Path, hashlib_callable):
     """Given path of the file and hash function, calculates file digest"""
     if os.path.isfile(file_path) and callable(hashlib_callable):
         hash_obj = hashlib_callable()
         with open(file_path, "rb") as f:
             for chunk in iter(lambda: f.read(4096), b""):
                 hash_obj.update(chunk)
         return hash_obj.hexdigest()
```

### Comparing `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/templates/changelog.html.jinja2` & `flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/templates/changelog.html.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/templates/re_doc.jinja2` & `flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/templates/re_doc.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2` & `flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi.egg-info/SOURCES.txt` & `flask-marshmallow-openapi-0.3.0/src/flask_marshmallow_openapi.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 .bumpversion.cfg
 .gitignore
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/flask_marshmallow_openapi/__init__.py
-src/flask_marshmallow_openapi/decorators.py
-src/flask_marshmallow_openapi/helpers.py
+src/flask_marshmallow_openapi/flask_paths.py
 src/flask_marshmallow_openapi/middleware.py
-src/flask_marshmallow_openapi/models.py
+src/flask_marshmallow_openapi/schemas_registry.py
+src/flask_marshmallow_openapi/securities.py
 src/flask_marshmallow_openapi/static_collector.py
 src/flask_marshmallow_openapi.egg-info/PKG-INFO
 src/flask_marshmallow_openapi.egg-info/SOURCES.txt
 src/flask_marshmallow_openapi.egg-info/dependency_links.txt
 src/flask_marshmallow_openapi.egg-info/not-zip-safe
 src/flask_marshmallow_openapi.egg-info/requires.txt
 src/flask_marshmallow_openapi.egg-info/top_level.txt
+src/flask_marshmallow_openapi/decorators/__init__.py
+src/flask_marshmallow_openapi/decorators/decorate_delete.py
+src/flask_marshmallow_openapi/decorators/decorate_get.py
+src/flask_marshmallow_openapi/decorators/decorate_patch.py
+src/flask_marshmallow_openapi/decorators/decorate_post.py
+src/flask_marshmallow_openapi/decorators/helpers.py
 src/flask_marshmallow_openapi/static/redoc_favicon.png
 src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
 src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
 src/flask_marshmallow_openapi/static/swagger_ui/index.css
 src/flask_marshmallow_openapi/static/swagger_ui/index.html
 src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
 src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
```

