# Comparing `tmp/django-gesha-0.1a4.tar.gz` & `tmp/django-gesha-0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-gesha-0.1a4.tar", last modified: Thu Jun 22 22:42:57 2023, max compression
+gzip compressed data, was "django-gesha-0.1a5.tar", last modified: Mon Jun 26 22:51:29 2023, max compression
```

## Comparing `django-gesha-0.1a4.tar` & `django-gesha-0.1a5.tar`

### file list

```diff
@@ -1,99 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.847611 django-gesha-0.1a4/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-22 22:42:47.000000 django-gesha-0.1a4/.eslintrc.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.835611 django-gesha-0.1a4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.839611 django-gesha-0.1a4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-22 22:42:47.000000 django-gesha-0.1a4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-22 22:42:47.000000 django-gesha-0.1a4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-22 22:42:47.000000 django-gesha-0.1a4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-22 22:42:47.000000 django-gesha-0.1a4/.mocharc.json
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-22 22:42:47.000000 django-gesha-0.1a4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-22 22:42:47.000000 django-gesha-0.1a4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-22 22:42:47.000000 django-gesha-0.1a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-22 22:42:57.847611 django-gesha-0.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-22 22:42:47.000000 django-gesha-0.1a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.839611 django-gesha-0.1a4/django_gesha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-22 22:42:57.000000 django-gesha-0.1a4/django_gesha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-22 22:42:57.000000 django-gesha-0.1a4/django_gesha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 22:42:57.000000 django-gesha-0.1a4/django_gesha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-22 22:42:57.000000 django-gesha-0.1a4/django_gesha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 22:42:57.000000 django-gesha-0.1a4/django_gesha.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/assets/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/settings.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/stylesheets/extra.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-06-22 22:42:47.000000 django-gesha-0.1a4/docs/user_guide.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/gesha/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.835611 django-gesha-0.1a4/gesha/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.835611 django-gesha-0.1a4/gesha/static/gesha/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.835611 django-gesha-0.1a4/gesha/static/gesha/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/gesha/static/gesha/dist/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/static/gesha/dist/js/django-gesha.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/gesha/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/templatetags/gesha.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gesha/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-22 22:42:47.000000 django-gesha-0.1a4/gulpfile.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/js_dist/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_dist/context.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_dist/converters.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_dist/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_dist/urls.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/js_src/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_src/context.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_src/converters.ts
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_src/main.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_src/urls.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/js_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_tests/context.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_tests/converters.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_tests/helpers.ts
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_tests/main.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_tests/test.html
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-22 22:42:47.000000 django-gesha-0.1a4/js_tests/urls.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-22 22:42:47.000000 django-gesha-0.1a4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)   349273 2023-06-22 22:42:47.000000 django-gesha-0.1a4/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-22 22:42:47.000000 django-gesha-0.1a4/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-22 22:42:47.000000 django-gesha-0.1a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 22:42:57.847611 django-gesha-0.1a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/test_project/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/test_project/fake/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.843611 django-gesha-0.1a4/test_project/fake/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.847611 django-gesha-0.1a4/test_project/fake/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/management/commands/printtestpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.847611 django-gesha-0.1a4/test_project/fake/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/templates/test.html
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/fake/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-06-22 22:42:47.000000 django-gesha-0.1a4/test_project/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:57.847611 django-gesha-0.1a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tests/test_package_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tests/test_package_versions_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tests/test_project_views_generate_correct_HTML.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-22 22:42:47.000000 django-gesha-0.1a4/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.087257 django-gesha-0.1a5/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-26 22:51:19.000000 django-gesha-0.1a5/.eslintrc.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.075257 django-gesha-0.1a5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.079257 django-gesha-0.1a5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-26 22:51:19.000000 django-gesha-0.1a5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-26 22:51:19.000000 django-gesha-0.1a5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-26 22:51:19.000000 django-gesha-0.1a5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 22:51:19.000000 django-gesha-0.1a5/.mocharc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-26 22:51:19.000000 django-gesha-0.1a5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 22:51:19.000000 django-gesha-0.1a5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-26 22:51:19.000000 django-gesha-0.1a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-26 22:51:29.087257 django-gesha-0.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-26 22:51:19.000000 django-gesha-0.1a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.079257 django-gesha-0.1a5/django_gesha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-26 22:51:29.000000 django-gesha-0.1a5/django_gesha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-26 22:51:29.000000 django-gesha-0.1a5/django_gesha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 22:51:29.000000 django-gesha-0.1a5/django_gesha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-26 22:51:29.000000 django-gesha-0.1a5/django_gesha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 22:51:29.000000 django-gesha-0.1a5/django_gesha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.083257 django-gesha-0.1a5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.083257 django-gesha-0.1a5/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-26 22:51:19.000000 django-gesha-0.1a5/docs/assets/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-26 22:51:19.000000 django-gesha-0.1a5/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:19.000000 django-gesha-0.1a5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-06-26 22:51:19.000000 django-gesha-0.1a5/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-26 22:51:19.000000 django-gesha-0.1a5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-26 22:51:19.000000 django-gesha-0.1a5/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-26 22:51:19.000000 django-gesha-0.1a5/docs/settings.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.083257 django-gesha-0.1a5/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-26 22:51:19.000000 django-gesha-0.1a5/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-26 22:51:19.000000 django-gesha-0.1a5/docs/stylesheets/extra.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-06-26 22:51:19.000000 django-gesha-0.1a5/docs/user_guide.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.083257 django-gesha-0.1a5/gesha/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-26 22:51:19.000000 django-gesha-0.1a5/gesha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-26 22:51:19.000000 django-gesha-0.1a5/gesha/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-26 22:51:19.000000 django-gesha-0.1a5/gesha/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:19.000000 django-gesha-0.1a5/gesha/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.079257 django-gesha-0.1a5/gesha/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.079257 django-gesha-0.1a5/gesha/static/gesha/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.079257 django-gesha-0.1a5/gesha/static/gesha/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.083257 django-gesha-0.1a5/gesha/static/gesha/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-06-26 22:51:19.000000 django-gesha-0.1a5/gesha/static/gesha/dist/js/django-gesha.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-06-26 22:51:19.000000 django-gesha-0.1a5/gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.083257 django-gesha-0.1a5/gesha/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:19.000000 django-gesha-0.1a5/gesha/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-26 22:51:19.000000 django-gesha-0.1a5/gesha/templatetags/gesha.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-26 22:51:19.000000 django-gesha-0.1a5/gesha/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-26 22:51:19.000000 django-gesha-0.1a5/gesha/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-26 22:51:19.000000 django-gesha-0.1a5/gesha/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-26 22:51:19.000000 django-gesha-0.1a5/gulpfile.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.083257 django-gesha-0.1a5/js_dist/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-26 22:51:19.000000 django-gesha-0.1a5/js_dist/context.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-26 22:51:19.000000 django-gesha-0.1a5/js_dist/converters.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-26 22:51:19.000000 django-gesha-0.1a5/js_dist/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-26 22:51:19.000000 django-gesha-0.1a5/js_dist/urls.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.083257 django-gesha-0.1a5/js_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-26 22:51:19.000000 django-gesha-0.1a5/js_src/context.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-26 22:51:19.000000 django-gesha-0.1a5/js_src/converters.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-26 22:51:19.000000 django-gesha-0.1a5/js_src/main.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-26 22:51:19.000000 django-gesha-0.1a5/js_src/urls.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.083257 django-gesha-0.1a5/js_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-26 22:51:19.000000 django-gesha-0.1a5/js_tests/context.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-26 22:51:19.000000 django-gesha-0.1a5/js_tests/converters.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-26 22:51:19.000000 django-gesha-0.1a5/js_tests/helpers.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-26 22:51:19.000000 django-gesha-0.1a5/js_tests/main.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-26 22:51:19.000000 django-gesha-0.1a5/js_tests/test.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-26 22:51:19.000000 django-gesha-0.1a5/js_tests/urls.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-26 22:51:19.000000 django-gesha-0.1a5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   349273 2023-06-26 22:51:19.000000 django-gesha-0.1a5/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-26 22:51:19.000000 django-gesha-0.1a5/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-26 22:51:19.000000 django-gesha-0.1a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 22:51:29.087257 django-gesha-0.1a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.083257 django-gesha-0.1a5/test_project/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.087257 django-gesha-0.1a5/test_project/fake/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:19.000000 django-gesha-0.1a5/test_project/fake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-26 22:51:19.000000 django-gesha-0.1a5/test_project/fake/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-26 22:51:19.000000 django-gesha-0.1a5/test_project/fake/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.087257 django-gesha-0.1a5/test_project/fake/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:19.000000 django-gesha-0.1a5/test_project/fake/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.087257 django-gesha-0.1a5/test_project/fake/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:19.000000 django-gesha-0.1a5/test_project/fake/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-26 22:51:19.000000 django-gesha-0.1a5/test_project/fake/management/commands/printtestpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-26 22:51:19.000000 django-gesha-0.1a5/test_project/fake/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.087257 django-gesha-0.1a5/test_project/fake/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-26 22:51:19.000000 django-gesha-0.1a5/test_project/fake/templates/test.html
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-26 22:51:19.000000 django-gesha-0.1a5/test_project/fake/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-26 22:51:19.000000 django-gesha-0.1a5/test_project/fake/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-26 22:51:19.000000 django-gesha-0.1a5/test_project/fake/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-06-26 22:51:19.000000 django-gesha-0.1a5/test_project/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:29.087257 django-gesha-0.1a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:51:19.000000 django-gesha-0.1a5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-26 22:51:19.000000 django-gesha-0.1a5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-26 22:51:19.000000 django-gesha-0.1a5/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-26 22:51:19.000000 django-gesha-0.1a5/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-26 22:51:19.000000 django-gesha-0.1a5/tests/test_package_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-26 22:51:19.000000 django-gesha-0.1a5/tests/test_package_versions_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-26 22:51:19.000000 django-gesha-0.1a5/tests/test_project_views_generate_correct_HTML.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-06-26 22:51:19.000000 django-gesha-0.1a5/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-26 22:51:19.000000 django-gesha-0.1a5/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 22:51:19.000000 django-gesha-0.1a5/tsconfig.json
```

### Comparing `django-gesha-0.1a4/.github/workflows/python-publish.yml` & `django-gesha-0.1a5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/.github/workflows/test.yml` & `django-gesha-0.1a5/.github/workflows/test.yml`

 * *Files 26% similar despite different names*

```diff
@@ -20,14 +20,21 @@
           python-version: ${{ matrix.python }}
       - name: Install tox
         run: |
           python -m pip install --upgrade pip
           pip install tox
       - name: Run tests
         run: tox -m ${{ matrix.python }}
+      - name: Upload coverage report
+        run: |
+          curl -X POST \
+          -H "Authorization: Bearer ${{ secrets.COV_ELYAS_TOKEN }}" \
+          -F file=@coverage.json \
+          https://cov.ely.as/github/${{ github.repository }}/${{ github.ref_name }}/
+        if: ${{ github.ref_name == 'main' }}
 
   test_js:
     name: JavaScript tests
 
     strategy:
       matrix:
         node-version: [16.x]
```

### Comparing `django-gesha-0.1a4/LICENSE` & `django-gesha-0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/PKG-INFO` & `django-gesha-0.1a5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gesha
-Version: 0.1a4
+Version: 0.1a5
 Summary: JavaScript utilities for Django projects.
 Author-email: elyas <elyas@ely.as>
 License: MIT
 Project-URL: Documentation, https://django-gesha.readthedocs.io/en/latest/
 Project-URL: Issue Tracker, https://github.com/ely-as/django-gesha/issues
 Project-URL: Source, https://github.com/ely-as/django-gesha
 Keywords: django,javascript,typescript
@@ -32,14 +32,15 @@
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
 # django-gesha
 
 [![Test](https://github.com/ely-as/django-gesha/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/ely-as/django-gesha/actions/workflows/test.yml)
+[![Coverage](https://cov.ely.as/github/ely-as/django-gesha/main/badge.svg)](https://cov.ely.as/github/ely-as/django-gesha/main/latest/)
 [![Version](https://img.shields.io/pypi/v/django-gesha)](https://pypi.org/project/django-gesha/)
 ![Python](https://img.shields.io/pypi/pyversions/django-gesha)
 ![Django](https://img.shields.io/pypi/djversions/django-gesha)
 
 
 [**Documentation**](https://django-gesha.readthedocs.io/en/latest/)
 **&nbsp;•&nbsp;**
```

### Comparing `django-gesha-0.1a4/README.md` & `django-gesha-0.1a5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # django-gesha
 
 [![Test](https://github.com/ely-as/django-gesha/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/ely-as/django-gesha/actions/workflows/test.yml)
+[![Coverage](https://cov.ely.as/github/ely-as/django-gesha/main/badge.svg)](https://cov.ely.as/github/ely-as/django-gesha/main/latest/)
 [![Version](https://img.shields.io/pypi/v/django-gesha)](https://pypi.org/project/django-gesha/)
 ![Python](https://img.shields.io/pypi/pyversions/django-gesha)
 ![Django](https://img.shields.io/pypi/djversions/django-gesha)
 
 
 [**Documentation**](https://django-gesha.readthedocs.io/en/latest/)
 **&nbsp;•&nbsp;**
```

### Comparing `django-gesha-0.1a4/django_gesha.egg-info/PKG-INFO` & `django-gesha-0.1a5/django_gesha.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gesha
-Version: 0.1a4
+Version: 0.1a5
 Summary: JavaScript utilities for Django projects.
 Author-email: elyas <elyas@ely.as>
 License: MIT
 Project-URL: Documentation, https://django-gesha.readthedocs.io/en/latest/
 Project-URL: Issue Tracker, https://github.com/ely-as/django-gesha/issues
 Project-URL: Source, https://github.com/ely-as/django-gesha
 Keywords: django,javascript,typescript
@@ -32,14 +32,15 @@
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
 # django-gesha
 
 [![Test](https://github.com/ely-as/django-gesha/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/ely-as/django-gesha/actions/workflows/test.yml)
+[![Coverage](https://cov.ely.as/github/ely-as/django-gesha/main/badge.svg)](https://cov.ely.as/github/ely-as/django-gesha/main/latest/)
 [![Version](https://img.shields.io/pypi/v/django-gesha)](https://pypi.org/project/django-gesha/)
 ![Python](https://img.shields.io/pypi/pyversions/django-gesha)
 ![Django](https://img.shields.io/pypi/djversions/django-gesha)
 
 
 [**Documentation**](https://django-gesha.readthedocs.io/en/latest/)
 **&nbsp;•&nbsp;**
```

### Comparing `django-gesha-0.1a4/django_gesha.egg-info/SOURCES.txt` & `django-gesha-0.1a5/django_gesha.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 docs/assets/favicon.svg
 docs/assets/logo.svg
 docs/stylesheets/extra.css
 docs/stylesheets/extra.min.css
 gesha/__init__.py
 gesha/conf.py
 gesha/mixins.py
+gesha/py.typed
 gesha/types.py
 gesha/urls.py
 gesha/views.py
 gesha/static/gesha/dist/js/django-gesha.bundle.min.js
 gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map
 gesha/templatetags/__init__.py
 gesha/templatetags/gesha.py
```

### Comparing `django-gesha-0.1a4/docs/assets/favicon.svg` & `django-gesha-0.1a5/docs/assets/favicon.svg`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/docs/assets/logo.svg` & `django-gesha-0.1a5/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/docs/contributing.md` & `django-gesha-0.1a5/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/docs/index.md` & `django-gesha-0.1a5/docs/index.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # django-gesha
 
 [![Test](https://github.com/ely-as/django-gesha/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/ely-as/django-gesha/actions/workflows/test.yml)
+[![Coverage](https://cov.ely.as/github/ely-as/django-gesha/main/badge.svg)](https://cov.ely.as/github/ely-as/django-gesha/main/latest/)
 [![Version](https://img.shields.io/pypi/v/django-gesha)](https://pypi.org/project/django-gesha/)
 ![Python](https://img.shields.io/pypi/pyversions/django-gesha)
 ![Django](https://img.shields.io/pypi/djversions/django-gesha)
 
 ---
 
 JavaScript utilities for [Django](https://www.djangoproject.com/) projects.
```

### Comparing `django-gesha-0.1a4/docs/installation.md` & `django-gesha-0.1a5/docs/installation.md`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/docs/settings.md` & `django-gesha-0.1a5/docs/settings.md`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/docs/stylesheets/extra.css` & `django-gesha-0.1a5/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/docs/user_guide.md` & `django-gesha-0.1a5/docs/user_guide.md`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/gesha/mixins.py` & `django-gesha-0.1a5/gesha/mixins.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/gesha/static/gesha/dist/js/django-gesha.bundle.min.js` & `django-gesha-0.1a5/gesha/static/gesha/dist/js/django-gesha.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map` & `django-gesha-0.1a5/gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/gesha/templatetags/gesha.py` & `django-gesha-0.1a5/gesha/templatetags/gesha.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/gesha/types.py` & `django-gesha-0.1a5/gesha/types.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/gesha/urls.py` & `django-gesha-0.1a5/gesha/urls.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/gulpfile.js` & `django-gesha-0.1a5/gulpfile.js`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/js_dist/converters.d.ts` & `django-gesha-0.1a5/js_dist/converters.d.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/js_dist/urls.d.ts` & `django-gesha-0.1a5/js_dist/urls.d.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/js_src/context.ts` & `django-gesha-0.1a5/js_src/context.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/js_src/converters.ts` & `django-gesha-0.1a5/js_src/converters.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/js_src/main.ts` & `django-gesha-0.1a5/js_src/main.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/js_src/urls.ts` & `django-gesha-0.1a5/js_src/urls.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/js_tests/converters.spec.ts` & `django-gesha-0.1a5/js_tests/converters.spec.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/js_tests/helpers.ts` & `django-gesha-0.1a5/js_tests/helpers.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/js_tests/test.html` & `django-gesha-0.1a5/js_tests/test.html`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/js_tests/urls.spec.ts` & `django-gesha-0.1a5/js_tests/urls.spec.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/mkdocs.yml` & `django-gesha-0.1a5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/package-lock.json` & `django-gesha-0.1a5/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8999924150485438%*

 * *Differences: {"'packages'": "{'': {'version': '0.1.0-alpha5'}}", "'version'": "'0.1.0-alpha5'"}*

```diff
@@ -26,15 +26,15 @@
                 "typescript": "^5.0.4",
                 "vinyl-buffer": "^1.0.1",
                 "vinyl-source-stream": "^2.0.0",
                 "watchify": "^4.0.0"
             },
             "license": "MIT",
             "name": "django-gesha",
-            "version": "0.1.0-alpha4"
+            "version": "0.1.0-alpha5"
         },
         "node_modules/@cspotcode/source-map-support": {
             "dependencies": {
                 "@jridgewell/trace-mapping": "0.3.9"
             },
             "dev": true,
             "engines": {
@@ -9499,9 +9499,9 @@
             },
             "integrity": "sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==",
             "resolved": "https://registry.npmjs.org/yocto-queue/-/yocto-queue-0.1.0.tgz",
             "version": "0.1.0"
         }
     },
     "requires": true,
-    "version": "0.1.0-alpha4"
+    "version": "0.1.0-alpha5"
 }
```

### Comparing `django-gesha-0.1a4/package.json` & `django-gesha-0.1a5/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.0-alpha5'"}*

```diff
@@ -41,9 +41,9 @@
         "url": "git+https://github.com/ely-as/django-gesha.git"
     },
     "scripts": {
         "lint": "eslint ./js_*/**/*.ts",
         "test": "mocha"
     },
     "types": "./js_dist/main.d.ts",
-    "version": "0.1.0-alpha4"
+    "version": "0.1.0-alpha5"
 }
```

### Comparing `django-gesha-0.1a4/pyproject.toml` & `django-gesha-0.1a5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -46,34 +46,40 @@
 version = {attr = "gesha.__version__"}
 readme = {file = ["README.md"], content-type = "text/markdown"}
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["gesha"]
 
+[tool.setuptools.package-data]
+gesha = ["py.typed"]
+
 [project.optional-dependencies]
 doc = [
     "mkdocs",
     "mkdocs-material",
 ]
 test = [
     "black",
     "beautifulsoup4",
     "lxml",
     "mypy",
-    "pytest>=7",      # >=7 required for pythonpath option
-    "pytest-cov",
+    "pytest>=7",        # >=7 required for pythonpath option
+    "pytest-cov>=4.1",  # >=4.1 required for JSON reports
     "pytest-django",
     "ruff",
     "types-beautifulsoup4",
     "uvicorn",
 ]
 
 [tool.coverage.run]
-omit = ["test_project/*"]
+omit = [
+    "test_project/*",
+    "tests/*",
+]
 
 [tool.mypy]
 warn_unused_configs = true
 files = [
     "gesha/**/*.py",
     "tests/**/*.py",
 ]
```

### Comparing `django-gesha-0.1a4/test_project/fake/management/commands/printtestpage.py` & `django-gesha-0.1a5/test_project/fake/management/commands/printtestpage.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/test_project/fake/settings.py` & `django-gesha-0.1a5/test_project/fake/settings.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/test_project/fake/urls.py` & `django-gesha-0.1a5/test_project/fake/urls.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/test_project/fake/views.py` & `django-gesha-0.1a5/test_project/fake/views.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/test_project/manage.py` & `django-gesha-0.1a5/test_project/manage.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/tests/conftest.py` & `django-gesha-0.1a5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/tests/test_package_versions_align.py` & `django-gesha-0.1a5/tests/test_package_versions_align.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/tests/test_project_views_generate_correct_HTML.py` & `django-gesha-0.1a5/tests/test_project_views_generate_correct_HTML.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/tests/test_urls.py` & `django-gesha-0.1a5/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a4/tox.ini` & `django-gesha-0.1a5/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -31,8 +31,8 @@
     py311-django41: Django>=4.1.3
 commands =
     format: black {tox_root}
     format: ruff check --fix-only {tox_root}
     static: black {tox_root} --check --diff
     static: ruff check {tox_root}
     static: mypy
-    test: pytest --cov={tox_root} --cov-report=term --cov-report=xml
+    test: pytest --cov={tox_root} --cov-report=term --cov-report=json
```

