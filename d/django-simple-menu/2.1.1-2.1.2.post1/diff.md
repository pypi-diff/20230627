# Comparing `tmp/django-simple-menu-2.1.1.tar.gz` & `tmp/django_simple_menu-2.1.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-simple-menu-2.1.1.tar", last modified: Sat Mar 11 23:48:15 2023, max compression
+gzip compressed data, was "django_simple_menu-2.1.2.post1.tar", last modified: Tue Jun 27 21:53:09 2023, max compression
```

## Comparing `django-simple-menu-2.1.1.tar` & `django_simple_menu-2.1.2.post1.tar`

### file list

```diff
@@ -1,94 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.919009 django-simple-menu-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.907009 django-simple-menu-2.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.911009 django-simple-menu-2.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/CHANGES
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-03-11 23:48:15.919009 django-simple-menu-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/TODO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.911009 django-simple-menu-2.1.1/django_simple_menu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-03-11 23:48:15.000000 django-simple-menu-2.1.1/django_simple_menu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-03-11 23:48:15.000000 django-simple-menu-2.1.1/django_simple_menu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 23:48:15.000000 django-simple-menu-2.1.1/django_simple_menu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-11 23:48:15.000000 django-simple-menu-2.1.1/django_simple_menu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-11 23:48:15.000000 django-simple-menu-2.1.1/django_simple_menu.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.915009 django-simple-menu-2.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/docs/example.rst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.915009 django-simple-menu-2.1.1/example/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.915009 django-simple-menu-2.1.1/example/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/accounts/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/accounts/menus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.915009 django-simple-menu-2.1.1/example/accounts/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/accounts/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.907009 django-simple-menu-2.1.1/example/accounts/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.915009 django-simple-menu-2.1.1/example/accounts/templates/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/accounts/templates/accounts/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/accounts/templates/accounts/profile.html
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/accounts/templates/accounts/sign_in.html
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/accounts/templates/accounts/subpage.html
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/accounts/templates/accounts/super_only.html
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/accounts/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/accounts/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.915009 django-simple-menu-2.1.1/example/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/example/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/example/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/example/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/example/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.915009 django-simple-menu-2.1.1/example/screenshots/
--rw-r--r--   0 runner    (1001) docker     (123)    44365 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/screenshots/main_page.png
--rw-r--r--   0 runner    (1001) docker     (123)    29340 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/screenshots/secret_page.png
--rw-r--r--   0 runner    (1001) docker     (123)    47275 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/screenshots/subpage.png
--rw-r--r--   0 runner    (1001) docker     (123)    44804 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/screenshots/user_page.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.919009 django-simple-menu-2.1.1/example/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/templates/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/example/templates/submenu.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.919009 django-simple-menu-2.1.1/menu/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/menu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/menu/menu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.919009 django-simple-menu-2.1.1/menu/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/menu/templates/bootstrap-navbar-submenu.html
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/menu/templates/bootstrap-navbar.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.919009 django-simple-menu-2.1.1/menu/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/menu/templatetags/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-03-11 23:48:15.919009 django-simple-menu-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.919009 django-simple-menu-2.1.1/simple_menu/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/simple_menu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/simple_menu/menu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.907009 django-simple-menu-2.1.1/simple_menu/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.919009 django-simple-menu-2.1.1/simple_menu/templates/simple_menu/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/simple_menu/templates/simple_menu/bootstrap-navbar-submenu.html
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/simple_menu/templates/simple_menu/bootstrap-navbar.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.919009 django-simple-menu-2.1.1/simple_menu/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/simple_menu/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/simple_menu/templatetags/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/simple_menu/templatetags/simple_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/simple_menu/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:15.919009 django-simple-menu-2.1.1/simple_menu/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/simple_menu/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/simple_menu/tests/test_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-11 23:48:00.000000 django-simple-menu-2.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.097299 django_simple_menu-2.1.2.post1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.089300 django_simple_menu-2.1.2.post1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.089300 django_simple_menu-2.1.2.post1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-27 21:53:09.097299 django_simple_menu-2.1.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/TODO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.089300 django_simple_menu-2.1.2.post1/django_simple_menu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-27 21:53:09.000000 django_simple_menu-2.1.2.post1/django_simple_menu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-27 21:53:09.000000 django_simple_menu-2.1.2.post1/django_simple_menu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:53:09.000000 django_simple_menu-2.1.2.post1/django_simple_menu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-27 21:53:09.000000 django_simple_menu-2.1.2.post1/django_simple_menu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 21:53:09.000000 django_simple_menu-2.1.2.post1/django_simple_menu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.093299 django_simple_menu-2.1.2.post1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/docs/example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.093299 django_simple_menu-2.1.2.post1/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.093299 django_simple_menu-2.1.2.post1/example/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/accounts/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/accounts/menus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.093299 django_simple_menu-2.1.2.post1/example/accounts/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/accounts/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.089300 django_simple_menu-2.1.2.post1/example/accounts/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.093299 django_simple_menu-2.1.2.post1/example/accounts/templates/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/accounts/templates/accounts/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/accounts/templates/accounts/profile.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/accounts/templates/accounts/sign_in.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/accounts/templates/accounts/subpage.html
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/accounts/templates/accounts/super_only.html
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/accounts/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/accounts/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.093299 django_simple_menu-2.1.2.post1/example/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/example/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/example/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/example/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/example/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.093299 django_simple_menu-2.1.2.post1/example/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (123)    44365 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/screenshots/main_page.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29340 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/screenshots/secret_page.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47275 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/screenshots/subpage.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44804 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/screenshots/user_page.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.093299 django_simple_menu-2.1.2.post1/example/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/templates/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/example/templates/submenu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.093299 django_simple_menu-2.1.2.post1/menu/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/menu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/menu/menu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.097299 django_simple_menu-2.1.2.post1/menu/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/menu/templates/bootstrap-navbar-submenu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/menu/templates/bootstrap-navbar.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.097299 django_simple_menu-2.1.2.post1/menu/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/menu/templatetags/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-27 21:53:09.097299 django_simple_menu-2.1.2.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.097299 django_simple_menu-2.1.2.post1/simple_menu/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/simple_menu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/simple_menu/menu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.089300 django_simple_menu-2.1.2.post1/simple_menu/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.097299 django_simple_menu-2.1.2.post1/simple_menu/templates/simple_menu/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/simple_menu/templates/simple_menu/bootstrap-navbar-submenu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/simple_menu/templates/simple_menu/bootstrap-navbar.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.097299 django_simple_menu-2.1.2.post1/simple_menu/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/simple_menu/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/simple_menu/templatetags/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/simple_menu/templatetags/simple_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/simple_menu/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:53:09.097299 django_simple_menu-2.1.2.post1/simple_menu/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/simple_menu/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/simple_menu/tests/test_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-27 21:52:52.000000 django_simple_menu-2.1.2.post1/tox.ini
```

### Comparing `django-simple-menu-2.1.1/.github/workflows/release.yml` & `django_simple_menu-2.1.2.post1/.github/workflows/release.yml`

 * *Files 9% similar despite different names*

```diff
@@ -14,26 +14,26 @@
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: 3.8
+          python-version: 3.11
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
-          python -m pip install -U setuptools twine wheel
+          python -m pip install -U build setuptools setuptools-scm twine
 
       - name: Build package
         run: |
-          python setup.py --version
-          python setup.py sdist --format=gztar bdist_wheel
-          twine check dist/*
+          python -m setuptools_scm
+          python -m build
+          twine check --strict dist/*
 
       - name: Upload packages to Jazzband
         if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@master
         with:
           user: jazzband
           password: ${{ secrets.JAZZBAND_RELEASE_KEY }}
```

### Comparing `django-simple-menu-2.1.1/.github/workflows/test.yml` & `django_simple_menu-2.1.2.post1/.github/workflows/test.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,89 @@
 name: Test
 
-on: [push, pull_request]
+on:
+  push:
+    branches: [master]
+    tags: ["*"]
+  pull_request:
+    branches: [master]
+
+env:
+  FORCE_COLOR: "1"
 
 jobs:
   build:
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-20.04
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.6', '3.7', '3.8', '3.9', '3.10', '3.11']
-        django-version: ['3.2', '4.0', '4.1', 'main']
-        exclude:
+        # https://docs.djangoproject.com/faq/install/#what-python-version-can-i-use-with-django
+        include:
           - django-version: '3.2'
-            python-version: '3.11'
+            python-version: '3.6'
+          - django-version: '3.2'
+            python-version: '3.7'
+          - django-version: '3.2'
+            python-version: '3.8'
+          - django-version: '3.2'
+            python-version: '3.9'
+          - django-version: '3.2'
+            python-version: '3.10'
 
           - django-version: '4.0'
-            python-version: '3.6'
+            python-version: '3.8'
           - django-version: '4.0'
-            python-version: '3.7'
+            python-version: '3.9'
           - django-version: '4.0'
-            python-version: '3.11'
+            python-version: '3.10'
 
           - django-version: '4.1'
-            python-version: '3.6'
+            python-version: '3.8'
           - django-version: '4.1'
-            python-version: '3.7'
+            python-version: '3.9'
+          - django-version: '4.1'
+            python-version: '3.10'
+          - django-version: '4.1'
+            python-version: '3.11'
+
+          - django-version: '4.2'
+            python-version: '3.8'
+          - django-version: '4.2'
+            python-version: '3.9'
+          - django-version: '4.2'
+            python-version: '3.10'
+          - django-version: '4.2'
+            python-version: '3.11'
 
           - django-version: 'main'
-            python-version: '3.6'
-          - django-version: 'main'
-            python-version: '3.7'
+            python-version: '3.10'
           - django-version: 'main'
-            python-version: '3.8'
+            python-version: '3.11'
           - django-version: 'main'
-            python-version: '3.9'
+            python-version: '3.12'
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
-
-    - name: Get pip cache dir
-      id: pip-cache
-      run: |
-        echo "dir=$(pip cache dir)" >> $GITHUB_OUTPUT
-
-    - name: Cache
-      uses: actions/cache@v3
-      with:
-        path: ${{ steps.pip-cache.outputs.dir }}
-        key:
-          ${{ matrix.python-version }}-v1-${{ hashFiles('**/setup.cfg') }}-${{ hashFiles('**/tox.ini') }}
-        restore-keys: |
-          ${{ matrix.python-version }}-v1-
+        allow-prereleases: true
+        cache: pip
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install --upgrade tox tox-gh-actions
 
     - name: Tox tests
       run: |
-        tox -v run
+        tox -v
       env:
         DJANGO: ${{ matrix.django-version }}
 
     - name: Upload coverage
       uses: codecov/codecov-action@v3
       with:
         name: Python ${{ matrix.python-version }}
```

### Comparing `django-simple-menu-2.1.1/.pre-commit-config.yaml` & `django_simple_menu-2.1.2.post1/.pre-commit-config.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,43 @@
+ci:
+    autoupdate_schedule: monthly
+
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
-    -   id: check-yaml
     -   id: end-of-file-fixer
     -   id: trailing-whitespace
     -   id: mixed-line-ending
+    -   id: check-toml
+    -   id: check-yaml
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.7.0
     hooks:
     -   id: pyupgrade
         args: [--py36-plus]
 -   repo: https://github.com/adamchainz/django-upgrade
-    rev: 1.13.0
+    rev: 1.14.0
     hooks:
     -   id: django-upgrade
         args: [--target-version, "3.2"]
 -   repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
     -   id: python-check-blanket-noqa
     -   id: python-check-mock-methods
     -   id: python-no-eval
     -   id: python-no-log-warn
     -   id: rst-backticks
     -   id: rst-directive-colons
+-   repo: https://github.com/asottile/setup-cfg-fmt
+    rev: v2.3.0
+    hooks:
+    -   id: setup-cfg-fmt
+-   repo: https://github.com/tox-dev/pyproject-fmt
+    rev: "0.12.1"
+    hooks:
+    -   id: pyproject-fmt
+-   repo: https://github.com/tox-dev/tox-ini-fmt
+    rev: "1.2.0"
+    hooks:
+    -   id: tox-ini-fmt
```

### Comparing `django-simple-menu-2.1.1/CHANGES` & `django_simple_menu-2.1.2.post1/CHANGES`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 django-simple-menu changelog
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+Version 2.1.2 - Released June 27th, 2023
+ - Correctly parse a deeper menu structure (#63, #133)
+ - Improved DX and CI
+
 Version 2.1.1 - Released March 12th, 2023
  - Install `importlib_metadata` only on older Python versions
 
 Version 2.1.0 - Released November 27th, 2022
  - Allow MenuItem's url to be callable (#70, #71, #112)
 
 Version 2.0.4 - Released November 17th, 2022
```

### Comparing `django-simple-menu-2.1.1/CODE_OF_CONDUCT.md` & `django_simple_menu-2.1.2.post1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/LICENSE` & `django_simple_menu-2.1.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/PKG-INFO` & `django_simple_menu-2.1.2.post1/django_simple_menu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: django-simple-menu
-Version: 2.1.1
+Version: 2.1.2.post1
 Summary: Simple, yet powerful, code-based menus for Django applications
 Home-page: https://github.com/jazzband/django-simple-menu
 Author: Evan Borgstrom
 Author-email: evan@borgstrom.ca
-License: BSD 2-Clause "Simplified" License
+License: BSD-2-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: <4.0,>=3.6
+Description-Content-Type: text/x-rst
 License-File: LICENSE
-License-File: AUTHORS
 
 ===================================
 django-simple-menu |latest-version|
 ===================================
 
 |jazzband| |build-status| |coverage| |docs| |python-support| |django-support|
```

### Comparing `django-simple-menu-2.1.1/README.rst` & `django_simple_menu-2.1.2.post1/README.rst`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/django_simple_menu.egg-info/PKG-INFO` & `django_simple_menu-2.1.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
-Name: django-simple-menu
-Version: 2.1.1
+Name: django_simple_menu
+Version: 2.1.2.post1
 Summary: Simple, yet powerful, code-based menus for Django applications
 Home-page: https://github.com/jazzband/django-simple-menu
 Author: Evan Borgstrom
 Author-email: evan@borgstrom.ca
-License: BSD 2-Clause "Simplified" License
+License: BSD-2-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: <4.0,>=3.6
+Description-Content-Type: text/x-rst
 License-File: LICENSE
-License-File: AUTHORS
 
 ===================================
 django-simple-menu |latest-version|
 ===================================
 
 |jazzband| |build-status| |coverage| |docs| |python-support| |django-support|
```

### Comparing `django-simple-menu-2.1.1/django_simple_menu.egg-info/SOURCES.txt` & `django_simple_menu-2.1.2.post1/django_simple_menu.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-.coveragerc
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
 AUTHORS
 CHANGES
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.rst
 TODO
 pyproject.toml
 setup.cfg
-setup.py
 tox.ini
 .github/workflows/release.yml
 .github/workflows/test.yml
 django_simple_menu.egg-info/PKG-INFO
 django_simple_menu.egg-info/SOURCES.txt
 django_simple_menu.egg-info/dependency_links.txt
 django_simple_menu.egg-info/requires.txt
```

### Comparing `django-simple-menu-2.1.1/docs/Makefile` & `django_simple_menu-2.1.2.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/docs/conf.py` & `django_simple_menu-2.1.2.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/docs/configuration.rst` & `django_simple_menu-2.1.2.post1/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/docs/installation.rst` & `django_simple_menu-2.1.2.post1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/docs/usage.rst` & `django_simple_menu-2.1.2.post1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/example/README.rst` & `django_simple_menu-2.1.2.post1/example/README.rst`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/example/accounts/menus.py` & `django_simple_menu-2.1.2.post1/example/accounts/menus.py`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/example/accounts/templates/accounts/index.html` & `django_simple_menu-2.1.2.post1/example/accounts/templates/accounts/index.html`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/example/accounts/templates/accounts/profile.html` & `django_simple_menu-2.1.2.post1/example/accounts/templates/accounts/profile.html`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/example/accounts/templates/accounts/sign_in.html` & `django_simple_menu-2.1.2.post1/example/accounts/templates/accounts/sign_in.html`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/example/accounts/templates/accounts/subpage.html` & `django_simple_menu-2.1.2.post1/example/accounts/templates/accounts/subpage.html`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/example/accounts/templates/accounts/super_only.html` & `django_simple_menu-2.1.2.post1/example/accounts/templates/accounts/super_only.html`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/example/accounts/views.py` & `django_simple_menu-2.1.2.post1/example/accounts/views.py`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/example/example/settings.py` & `django_simple_menu-2.1.2.post1/example/example/settings.py`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/example/manage.py` & `django_simple_menu-2.1.2.post1/example/manage.py`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/example/screenshots/main_page.png` & `django_simple_menu-2.1.2.post1/example/screenshots/main_page.png`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/example/screenshots/secret_page.png` & `django_simple_menu-2.1.2.post1/example/screenshots/secret_page.png`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/example/screenshots/subpage.png` & `django_simple_menu-2.1.2.post1/example/screenshots/subpage.png`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/example/screenshots/user_page.png` & `django_simple_menu-2.1.2.post1/example/screenshots/user_page.png`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/example/templates/base.html` & `django_simple_menu-2.1.2.post1/example/templates/base.html`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/menu/templates/bootstrap-navbar-submenu.html` & `django_simple_menu-2.1.2.post1/menu/templates/bootstrap-navbar-submenu.html`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/menu/templates/bootstrap-navbar.html` & `django_simple_menu-2.1.2.post1/menu/templates/bootstrap-navbar.html`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/setup.cfg` & `django_simple_menu-2.1.2.post1/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 [metadata]
-name = django-simple-menu
+name = django_simple_menu
+description = Simple, yet powerful, code-based menus for Django applications
+long_description = file: README.rst
+long_description_content_type = text/x-rst
 url = https://github.com/jazzband/django-simple-menu
 author = Evan Borgstrom
 author_email = evan@borgstrom.ca
-description = Simple, yet powerful, code-based menus for Django applications
-long_description = file: README.rst
-license = BSD 2-Clause "Simplified" License
+license = BSD-2-Clause
+license_files = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Operating System :: OS Independent
-	Topic :: Software Development :: Libraries
-	Topic :: Software Development :: Libraries :: Python Modules
 	Programming Language :: Python
-	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
+	Topic :: Software Development :: Libraries
+	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 packages = 
 	simple_menu
 	menu
-include_package_data = True
-python_requires = >=3.6,<4.0
 install_requires = 
 	Django>=2.2
-	importlib_metadata; python_version < '3.8'
+	importlib-metadata;python_version < '3.8'
+python_requires = >=3.6,<4.0
+include_package_data = True
 setup_requires = 
-	setuptools_scm
+	setuptools-scm
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `django-simple-menu-2.1.1/simple_menu/menu.py` & `django_simple_menu-2.1.2.post1/simple_menu/menu.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,22 +120,28 @@
             for item in items
             if item.visible
         ]
 
         # determine if we should apply 'selected' to parents when one of their
         # children is the 'selected' menu
         if getattr(settings, 'MENU_SELECT_PARENTS', False):
-            def is_child_selected(item):
-                for child in item.children:
-                    if child.selected or is_child_selected(child):
-                        return True
+            def get_path_selected(item, parents):
+                if item.selected:
+                    return parents + [item]
+                else:
+                    for child in item.children:
+                        path_selected = get_path_selected(child, parents + [item])
+                        if path_selected:
+                            return path_selected
 
             for item in visible:
-                if is_child_selected(item):
-                    item.selected = True
+                path_selected = get_path_selected(item, [])
+                if path_selected:
+                    for item_selected in path_selected:
+                        item_selected.selected = True
 
         return visible
 
 
 class MenuItem:
     """
     MenuItem represents an item in a menu, possibly one that has a sub-menu (children).
```

### Comparing `django-simple-menu-2.1.1/simple_menu/templates/simple_menu/bootstrap-navbar-submenu.html` & `django_simple_menu-2.1.2.post1/simple_menu/templates/simple_menu/bootstrap-navbar-submenu.html`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/simple_menu/templates/simple_menu/bootstrap-navbar.html` & `django_simple_menu-2.1.2.post1/simple_menu/templates/simple_menu/bootstrap-navbar.html`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/simple_menu/templatetags/simple_menu.py` & `django_simple_menu-2.1.2.post1/simple_menu/templatetags/simple_menu.py`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/simple_menu/test_settings.py` & `django_simple_menu-2.1.2.post1/simple_menu/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-simple-menu-2.1.1/simple_menu/tests/test_menu.py` & `django_simple_menu-2.1.2.post1/simple_menu/tests/test_menu.py`

 * *Files identical despite different names*

