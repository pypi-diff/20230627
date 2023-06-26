# Comparing `tmp/flook-0.1.5.tar.gz` & `tmp/flook-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flook-0.1.5.tar", last modified: Mon Jun 26 00:43:09 2023, max compression
+gzip compressed data, was "flook-0.2.0.tar", last modified: Mon Jun 26 23:14:12 2023, max compression
```

## Comparing `flook-0.1.5.tar` & `flook-0.2.0.tar`

### file list

```diff
@@ -1,68 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.628960 flook-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.624959 flook-0.1.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-26 00:42:41.000000 flook-0.1.5/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 00:42:41.000000 flook-0.1.5/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.624959 flook-0.1.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-26 00:42:41.000000 flook-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-26 00:42:41.000000 flook-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.624959 flook-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-26 00:42:41.000000 flook-0.1.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-26 00:42:41.000000 flook-0.1.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-26 00:42:41.000000 flook-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 00:42:41.000000 flook-0.1.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 00:42:41.000000 flook-0.1.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-26 00:42:41.000000 flook-0.1.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-26 00:42:41.000000 flook-0.1.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-26 00:42:41.000000 flook-0.1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-26 00:42:41.000000 flook-0.1.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-26 00:43:09.628960 flook-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-26 00:42:41.000000 flook-0.1.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.624959 flook-0.1.5/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 00:42:41.000000 flook-0.1.5/cache/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 00:42:41.000000 flook-0.1.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.620959 flook-0.1.5/recipe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.624959 flook-0.1.5/recipe/nginx/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-26 00:42:41.000000 flook-0.1.5/recipe/nginx/motd.j2
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-26 00:42:41.000000 flook-0.1.5/recipe/nginx/recipe.yml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 00:42:41.000000 flook-0.1.5/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-26 00:43:09.628960 flook-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-26 00:42:41.000000 flook-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.620959 flook-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.624959 flook-0.1.5/src/flook/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.628960 flook-0.1.5/src/flook/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/command/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/command/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/command/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.628960 flook-0.1.5/src/flook/exception/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.628960 flook-0.1.5/src/flook/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/model/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/model/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/model/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.628960 flook-0.1.5/src/flook/module/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/module/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/module/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/module/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/module/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/module/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/module/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/module/playbook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.624959 flook-0.1.5/src/flook.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-26 00:43:09.000000 flook-0.1.5/src/flook.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-26 00:43:09.000000 flook-0.1.5/src/flook.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 00:43:09.000000 flook-0.1.5/src/flook.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 00:43:09.000000 flook-0.1.5/src/flook.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 00:43:09.000000 flook-0.1.5/src/flook.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-26 00:43:09.000000 flook-0.1.5/src/flook.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 00:43:09.000000 flook-0.1.5/src/flook.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.628960 flook-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 00:42:41.000000 flook-0.1.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.628960 flook-0.1.5/tests/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 00:42:41.000000 flook-0.1.5/tests/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-26 00:42:41.000000 flook-0.1.5/tests/module/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-26 00:42:41.000000 flook-0.1.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:14:12.933485 flook-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:14:12.929485 flook-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-26 23:13:50.000000 flook-0.2.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 23:13:50.000000 flook-0.2.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:14:12.929485 flook-0.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-26 23:13:50.000000 flook-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-26 23:13:50.000000 flook-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:14:12.929485 flook-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-26 23:13:50.000000 flook-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-26 23:13:50.000000 flook-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-26 23:13:50.000000 flook-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 23:13:50.000000 flook-0.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 23:13:50.000000 flook-0.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-26 23:13:50.000000 flook-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-26 23:13:50.000000 flook-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-26 23:13:50.000000 flook-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-26 23:13:50.000000 flook-0.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-26 23:14:12.933485 flook-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-26 23:13:50.000000 flook-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:14:12.929485 flook-0.2.0/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 23:13:50.000000 flook-0.2.0/cache/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 23:13:50.000000 flook-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:14:12.925485 flook-0.2.0/recipe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:14:12.929485 flook-0.2.0/recipe/nginx/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-26 23:13:50.000000 flook-0.2.0/recipe/nginx/motd.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-26 23:13:50.000000 flook-0.2.0/recipe/nginx/recipe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 23:13:50.000000 flook-0.2.0/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-26 23:14:12.933485 flook-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-26 23:13:50.000000 flook-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:14:12.925485 flook-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:14:12.929485 flook-0.2.0/src/flook/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-26 23:13:50.000000 flook-0.2.0/src/flook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-26 23:13:50.000000 flook-0.2.0/src/flook/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:14:12.929485 flook-0.2.0/src/flook/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 23:13:50.000000 flook-0.2.0/src/flook/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-26 23:13:50.000000 flook-0.2.0/src/flook/command/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-26 23:13:50.000000 flook-0.2.0/src/flook/command/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-26 23:13:50.000000 flook-0.2.0/src/flook/command/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:14:12.929485 flook-0.2.0/src/flook/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 23:13:50.000000 flook-0.2.0/src/flook/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:14:12.929485 flook-0.2.0/src/flook/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 23:13:50.000000 flook-0.2.0/src/flook/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-26 23:13:50.000000 flook-0.2.0/src/flook/model/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-26 23:13:50.000000 flook-0.2.0/src/flook/model/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-26 23:13:50.000000 flook-0.2.0/src/flook/model/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:14:12.929485 flook-0.2.0/src/flook/module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 23:13:50.000000 flook-0.2.0/src/flook/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-26 23:13:50.000000 flook-0.2.0/src/flook/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-26 23:13:50.000000 flook-0.2.0/src/flook/module/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-26 23:13:50.000000 flook-0.2.0/src/flook/module/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-26 23:13:50.000000 flook-0.2.0/src/flook/module/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-26 23:13:50.000000 flook-0.2.0/src/flook/module/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-26 23:13:50.000000 flook-0.2.0/src/flook/module/playbook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:14:12.929485 flook-0.2.0/src/flook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-26 23:14:12.000000 flook-0.2.0/src/flook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-26 23:14:12.000000 flook-0.2.0/src/flook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 23:14:12.000000 flook-0.2.0/src/flook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 23:14:12.000000 flook-0.2.0/src/flook.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 23:14:12.000000 flook-0.2.0/src/flook.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-26 23:14:12.000000 flook-0.2.0/src/flook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 23:14:12.000000 flook-0.2.0/src/flook.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:14:12.933485 flook-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 23:13:50.000000 flook-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:14:12.933485 flook-0.2.0/tests/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 23:13:50.000000 flook-0.2.0/tests/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-26 23:13:50.000000 flook-0.2.0/tests/module/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-26 23:13:50.000000 flook-0.2.0/tox.ini
```

### Comparing `flook-0.1.5/.github/workflows/release.yml` & `flook-0.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/.gitignore` & `flook-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/CODE_OF_CONDUCT.md` & `flook-0.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/CONTRIBUTING.rst` & `flook-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/LICENSE.txt` & `flook-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/Makefile` & `flook-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/PKG-INFO` & `flook-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flook
-Version: 0.1.5
+Version: 0.2.0
 Summary: A Lightweight and Flexible Ansible Command Line Tool.
 Home-page: https://github.com/norwik/flook/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/norwik/flook/
 Project-URL: Source, https://github.com/norwik/flook/
@@ -58,7 +58,28 @@
 
 
 4. Init the config file and the database
 
 .. code-block::
 
     $ flook config init
+
+
+5. Add recipe
+
+.. code-block::
+
+    $ flook recipe add clivern/nginx -p recipe/nginx
+
+
+6. Add a host
+
+.. code-block::
+
+    $ flook host add example.com -i 127.0.0.1 -p 22 -u root -s /Users/root/.ssh/id_rsa.pem
+
+
+7. Run a recipe towards a host
+
+.. code-block::
+
+    $ flook recipe run clivern/nginx -h example.com
```

### Comparing `flook-0.1.5/README.rst` & `flook-0.2.0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -38,7 +38,28 @@
 
 
 4. Init the config file and the database
 
 .. code-block::
 
     $ flook config init
+
+
+5. Add recipe
+
+.. code-block::
+
+    $ flook recipe add clivern/nginx -p recipe/nginx
+
+
+6. Add a host
+
+.. code-block::
+
+    $ flook host add example.com -i 127.0.0.1 -p 22 -u root -s /Users/root/.ssh/id_rsa.pem
+
+
+7. Run a recipe towards a host
+
+.. code-block::
+
+    $ flook recipe run clivern/nginx -h example.com
```

### Comparing `flook-0.1.5/recipe/nginx/recipe.yml` & `flook-0.2.0/recipe/nginx/recipe.yml`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/setup.cfg` & `flook-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	click<=8.1.3
 	ansible-runner<=2.3.3
-	Jinja2<=3.1.2
+	yaspin<=2.3.0
 	prettytable<=3.8.0
 	PyYAML<=6.0
 	importlib-metadata; python_version<"3.8"
 
 [options.packages.find]
 where = src
 exclude =
```

### Comparing `flook-0.1.5/setup.py` & `flook-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/src/flook/__init__.py` & `flook-0.2.0/src/flook/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/src/flook/cli.py` & `flook-0.2.0/src/flook/cli.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/src/flook/command/__init__.py` & `flook-0.2.0/src/flook/command/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/src/flook/command/configs.py` & `flook-0.2.0/src/flook/command/configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,18 @@
         self.logger = Logger().get_logger(__name__)
 
     def init(self):
         """Init Configs"""
         if self._home == "":
             raise click.ClickException("User home path is not defined")
 
-        base = {"database": {"type": "file", "path": "{}/flook.db".format(self._home)}}
+        base = {
+            "database": {"type": "file", "path": "{}/flook.db".format(self._home)},
+            "cache": {"path": "/tmp"},
+        }
 
         self.database.connect("{}/flook.db".format(self._home))
         self.database.migrate()
 
         self.file_system.write_file(
             "{}/{}".format(self._home, Configs.FILE), yaml.dump(base)
         )
```

### Comparing `flook-0.1.5/src/flook/command/hosts.py` & `flook-0.2.0/src/flook/command/hosts.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/src/flook/command/recipes.py` & `flook-0.2.0/src/flook/command/recipes.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,21 +19,24 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import uuid
 import click
 import yaml
+from yaspin import yaspin
 
 from flook.model.recipe import Recipe
 from flook.module.logger import Logger
 from flook.module.database import Database
 from flook.module.output import Output
 from flook.module.config import Config
 from flook.module.file_system import FileSystem
+from flook.module.playbook import Playbook
+from flook.module.ansible import Ansible
 
 
 class Recipes:
     """Recipes Class"""
 
     def __init__(self):
         self.output = Output()
@@ -167,9 +170,20 @@
                 if tag not in item.tags or found == item.id:
                     continue
                 hosts.append(item)
 
         if len(hosts) == 0:
             raise click.ClickException(f"No hosts matching!")
 
-        print(hosts)
-        print(recipe)
+        with yaspin(text="Running recipe..", color="cyan") as sp:
+            pb_id = str(uuid.uuid4())
+            pb = Playbook(
+                pb_id, self._configs["cache"]["path"].rstrip("/"), hosts, recipe
+            )
+            pb.build()
+            result = pb.run()
+            pb.cleanup()
+
+            if result:
+                sp.write("Recipe finished successfully!")
+            else:
+                sp.write("Oops! recipe failed.")
```

### Comparing `flook-0.1.5/src/flook/exception/__init__.py` & `flook-0.2.0/src/flook/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/src/flook/model/__init__.py` & `flook-0.2.0/src/flook/model/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/src/flook/model/host.py` & `flook-0.2.0/src/flook/model/host.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/src/flook/model/recipe.py` & `flook-0.2.0/src/flook/model/recipe.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/src/flook/model/task.py` & `flook-0.2.0/src/flook/model/task.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/src/flook/module/__init__.py` & `flook-0.2.0/src/flook/module/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/src/flook/module/ansible.py` & `flook-0.2.0/src/flook/module/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,47 +16,30 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import ansible_runner
+import os
+import yaml
 
-from flook.module.logger import Logger
-from flook.module.file_system import FileSystem
 
+class Config:
+    """Config Class"""
 
-class Ansible:
-    """Ansible Module"""
+    FILE = ".flook.yml"
 
     def __init__(self):
-        self.file_system = FileSystem()
-        self.logger = Logger().get_logger(__name__)
+        self.configs = {}
+        self._home = os.getenv("HOME", "")
 
-    def run(self, data_dir, playbook, inventory):
-        """
-        Run Ansible Playbook
-        """
-        out = ansible_runner.run(
-            private_data_dir=data_dir,
-            playbook=playbook,
-            inventory=inventory,
-            quiet=True,
-        )
-
-        if out.status.lower() == "failed":
-            return False
-
-        elif out.status.lower() == "successful":
-            return True
-
-        return False
-
-    def cleanup(self, path):
-        """
-        Cleanup Plan Directory
-        """
-        try:
-            self.file_system.delete_directory(path)
-        except Exception:
-            pass
+    def load(self):
+        """Load Configs"""
+        with open("{}/{}".format(self._home, Config.FILE)) as f:
+            self.configs = yaml.load(f, Loader=yaml.FullLoader)
+
+        return self.configs
+
+    def get_configs(self):
+        """Get Configs"""
+        return self.configs
```

### Comparing `flook-0.1.5/src/flook/module/config.py` & `flook-0.2.0/tests/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,31 +15,7 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-
-import os
-import yaml
-
-
-class Config:
-    """Config Class"""
-
-    FILE = ".flook.yml"
-
-    def __init__(self):
-        self.configs = {}
-        self._home = os.getenv("HOME", "")
-
-    def load(self):
-        """Load Configs"""
-        with open("{}/{}".format(self._home, Config.FILE)) as f:
-            self.configs = yaml.load(f, Loader=yaml.FullLoader)
-
-        return self.configs
-
-    def get_configs(self):
-        """Get Configs"""
-        return self.configs
```

### Comparing `flook-0.1.5/src/flook/module/database.py` & `flook-0.2.0/src/flook/module/database.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/src/flook/module/file_system.py` & `flook-0.2.0/src/flook/module/file_system.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/src/flook/module/logger.py` & `flook-0.2.0/src/flook/module/logger.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/src/flook/module/output.py` & `flook-0.2.0/src/flook/module/output.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.5/src/flook/module/playbook.py` & `flook-0.2.0/tests/module/test_logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,27 +16,18 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+import logging
+import pytest
+from flook.module.logger import Logger
 
-# @TODO this class should create a dir & create all the required
-# files for ansible to run against the host.
-class Playbook:
-    """Playbook Class"""
 
-    def __init__(self):
-        pass
+def test_logger():
+    """Logger Tests"""
+    logger = Logger()
+    result = logger.get_logger()
 
-    def set_cache_dir(self, cache_dir):
-        pass
-
-    def set_hosts(self, hosts):
-        pass
-
-    def set_recipe(self, recipe):
-        pass
-
-    def build(self):
-        pass
+    assert isinstance(result, logging.Logger) == True
```

### Comparing `flook-0.1.5/src/flook.egg-info/PKG-INFO` & `flook-0.2.0/src/flook.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flook
-Version: 0.1.5
+Version: 0.2.0
 Summary: A Lightweight and Flexible Ansible Command Line Tool.
 Home-page: https://github.com/norwik/flook/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/norwik/flook/
 Project-URL: Source, https://github.com/norwik/flook/
@@ -58,7 +58,28 @@
 
 
 4. Init the config file and the database
 
 .. code-block::
 
     $ flook config init
+
+
+5. Add recipe
+
+.. code-block::
+
+    $ flook recipe add clivern/nginx -p recipe/nginx
+
+
+6. Add a host
+
+.. code-block::
+
+    $ flook host add example.com -i 127.0.0.1 -p 22 -u root -s /Users/root/.ssh/id_rsa.pem
+
+
+7. Run a recipe towards a host
+
+.. code-block::
+
+    $ flook recipe run clivern/nginx -h example.com
```

### Comparing `flook-0.1.5/src/flook.egg-info/SOURCES.txt` & `flook-0.2.0/src/flook.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 src/flook/command/recipes.py
 src/flook/exception/__init__.py
 src/flook/model/__init__.py
 src/flook/model/host.py
 src/flook/model/recipe.py
 src/flook/model/task.py
 src/flook/module/__init__.py
-src/flook/module/ansible.py
 src/flook/module/config.py
 src/flook/module/database.py
 src/flook/module/file_system.py
 src/flook/module/logger.py
 src/flook/module/output.py
 src/flook/module/playbook.py
 tests/__init__.py
```

### Comparing `flook-0.1.5/tox.ini` & `flook-0.2.0/tox.ini`

 * *Files identical despite different names*

