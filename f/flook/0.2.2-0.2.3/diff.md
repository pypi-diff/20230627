# Comparing `tmp/flook-0.2.2.tar.gz` & `tmp/flook-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flook-0.2.2.tar", last modified: Tue Jun 27 12:24:25 2023, max compression
+gzip compressed data, was "flook-0.2.3.tar", last modified: Tue Jun 27 17:54:28 2023, max compression
```

## Comparing `flook-0.2.2.tar` & `flook-0.2.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:24:25.755612 flook-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:24:25.747612 flook-0.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-27 12:24:00.000000 flook-0.2.2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 12:24:00.000000 flook-0.2.2/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:24:25.747612 flook-0.2.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-27 12:24:00.000000 flook-0.2.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-27 12:24:00.000000 flook-0.2.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:24:25.747612 flook-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-27 12:24:00.000000 flook-0.2.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-27 12:24:00.000000 flook-0.2.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-27 12:24:00.000000 flook-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 12:24:00.000000 flook-0.2.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-27 12:24:00.000000 flook-0.2.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-27 12:24:00.000000 flook-0.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-27 12:24:00.000000 flook-0.2.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-27 12:24:00.000000 flook-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-27 12:24:00.000000 flook-0.2.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-27 12:24:25.755612 flook-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-27 12:24:00.000000 flook-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:24:25.747612 flook-0.2.2/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 12:24:00.000000 flook-0.2.2/cache/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-27 12:24:00.000000 flook-0.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:24:25.743612 flook-0.2.2/recipe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:24:25.747612 flook-0.2.2/recipe/motd/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-27 12:24:00.000000 flook-0.2.2/recipe/motd/motd.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-27 12:24:00.000000 flook-0.2.2/recipe/motd/recipe.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:24:25.747612 flook-0.2.2/recipe/nginx/
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-27 12:24:00.000000 flook-0.2.2/recipe/nginx/recipe.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:24:25.747612 flook-0.2.2/recipe/ping/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-27 12:24:00.000000 flook-0.2.2/recipe/ping/recipe.yml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 12:24:00.000000 flook-0.2.2/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-27 12:24:25.759612 flook-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-27 12:24:00.000000 flook-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:24:25.743612 flook-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:24:25.751612 flook-0.2.2/src/flook/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-27 12:24:00.000000 flook-0.2.2/src/flook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-27 12:24:00.000000 flook-0.2.2/src/flook/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:24:25.751612 flook-0.2.2/src/flook/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-27 12:24:00.000000 flook-0.2.2/src/flook/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-27 12:24:00.000000 flook-0.2.2/src/flook/command/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-27 12:24:00.000000 flook-0.2.2/src/flook/command/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-27 12:24:00.000000 flook-0.2.2/src/flook/command/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:24:25.751612 flook-0.2.2/src/flook/exception/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-27 12:24:00.000000 flook-0.2.2/src/flook/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:24:25.755612 flook-0.2.2/src/flook/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-27 12:24:00.000000 flook-0.2.2/src/flook/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-27 12:24:00.000000 flook-0.2.2/src/flook/model/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-27 12:24:00.000000 flook-0.2.2/src/flook/model/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-27 12:24:00.000000 flook-0.2.2/src/flook/model/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:24:25.755612 flook-0.2.2/src/flook/module/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-27 12:24:00.000000 flook-0.2.2/src/flook/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-27 12:24:00.000000 flook-0.2.2/src/flook/module/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-27 12:24:00.000000 flook-0.2.2/src/flook/module/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-27 12:24:00.000000 flook-0.2.2/src/flook/module/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-27 12:24:00.000000 flook-0.2.2/src/flook/module/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-27 12:24:00.000000 flook-0.2.2/src/flook/module/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-27 12:24:00.000000 flook-0.2.2/src/flook/module/playbook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:24:25.751612 flook-0.2.2/src/flook.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-27 12:24:25.000000 flook-0.2.2/src/flook.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-27 12:24:25.000000 flook-0.2.2/src/flook.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:24:25.000000 flook-0.2.2/src/flook.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 12:24:25.000000 flook-0.2.2/src/flook.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:24:25.000000 flook-0.2.2/src/flook.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-27 12:24:25.000000 flook-0.2.2/src/flook.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 12:24:25.000000 flook-0.2.2/src/flook.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:24:25.755612 flook-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-27 12:24:00.000000 flook-0.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:24:25.755612 flook-0.2.2/tests/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:24:00.000000 flook-0.2.2/tests/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-27 12:24:00.000000 flook-0.2.2/tests/module/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-27 12:24:00.000000 flook-0.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:54:28.802683 flook-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:54:28.798683 flook-0.2.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-27 17:54:07.000000 flook-0.2.3/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 17:54:07.000000 flook-0.2.3/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:54:28.798683 flook-0.2.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-27 17:54:07.000000 flook-0.2.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-27 17:54:07.000000 flook-0.2.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:54:28.798683 flook-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-27 17:54:07.000000 flook-0.2.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-27 17:54:07.000000 flook-0.2.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-27 17:54:07.000000 flook-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 17:54:07.000000 flook-0.2.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-27 17:54:07.000000 flook-0.2.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-27 17:54:07.000000 flook-0.2.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-27 17:54:07.000000 flook-0.2.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-27 17:54:07.000000 flook-0.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-27 17:54:07.000000 flook-0.2.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-27 17:54:28.802683 flook-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-27 17:54:07.000000 flook-0.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:54:28.798683 flook-0.2.3/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 17:54:07.000000 flook-0.2.3/cache/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-27 17:54:07.000000 flook-0.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:54:28.798683 flook-0.2.3/recipe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:54:28.798683 flook-0.2.3/recipe/motd/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-27 17:54:07.000000 flook-0.2.3/recipe/motd/motd.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-27 17:54:07.000000 flook-0.2.3/recipe/motd/recipe.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:54:28.798683 flook-0.2.3/recipe/nginx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-27 17:54:07.000000 flook-0.2.3/recipe/nginx/recipe.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:54:28.798683 flook-0.2.3/recipe/ping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-27 17:54:07.000000 flook-0.2.3/recipe/ping/recipe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 17:54:07.000000 flook-0.2.3/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-27 17:54:28.802683 flook-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-27 17:54:07.000000 flook-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:54:28.798683 flook-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:54:28.798683 flook-0.2.3/src/flook/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-27 17:54:07.000000 flook-0.2.3/src/flook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-06-27 17:54:07.000000 flook-0.2.3/src/flook/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:54:28.802683 flook-0.2.3/src/flook/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-27 17:54:07.000000 flook-0.2.3/src/flook/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-27 17:54:07.000000 flook-0.2.3/src/flook/command/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-27 17:54:07.000000 flook-0.2.3/src/flook/command/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-27 17:54:07.000000 flook-0.2.3/src/flook/command/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:54:28.802683 flook-0.2.3/src/flook/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-27 17:54:07.000000 flook-0.2.3/src/flook/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:54:28.802683 flook-0.2.3/src/flook/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-27 17:54:07.000000 flook-0.2.3/src/flook/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-27 17:54:07.000000 flook-0.2.3/src/flook/model/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-27 17:54:07.000000 flook-0.2.3/src/flook/model/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-27 17:54:07.000000 flook-0.2.3/src/flook/model/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:54:28.802683 flook-0.2.3/src/flook/module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-27 17:54:07.000000 flook-0.2.3/src/flook/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-27 17:54:07.000000 flook-0.2.3/src/flook/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-27 17:54:07.000000 flook-0.2.3/src/flook/module/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-27 17:54:07.000000 flook-0.2.3/src/flook/module/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-27 17:54:07.000000 flook-0.2.3/src/flook/module/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-27 17:54:07.000000 flook-0.2.3/src/flook/module/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-27 17:54:07.000000 flook-0.2.3/src/flook/module/playbook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:54:28.802683 flook-0.2.3/src/flook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-27 17:54:28.000000 flook-0.2.3/src/flook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-27 17:54:28.000000 flook-0.2.3/src/flook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:54:28.000000 flook-0.2.3/src/flook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 17:54:28.000000 flook-0.2.3/src/flook.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:54:28.000000 flook-0.2.3/src/flook.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-27 17:54:28.000000 flook-0.2.3/src/flook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 17:54:28.000000 flook-0.2.3/src/flook.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:54:28.802683 flook-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-27 17:54:07.000000 flook-0.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:54:28.802683 flook-0.2.3/tests/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:54:07.000000 flook-0.2.3/tests/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-27 17:54:07.000000 flook-0.2.3/tests/module/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-27 17:54:07.000000 flook-0.2.3/tox.ini
```

### Comparing `flook-0.2.2/.github/workflows/release.yml` & `flook-0.2.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/.gitignore` & `flook-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/CODE_OF_CONDUCT.md` & `flook-0.2.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/CONTRIBUTING.rst` & `flook-0.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/LICENSE.txt` & `flook-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/Makefile` & `flook-0.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/PKG-INFO` & `flook-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flook
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Lightweight and Flexible Ansible Command Line Tool.
 Home-page: https://github.com/norwik/flook/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/norwik/flook/
 Project-URL: Source, https://github.com/norwik/flook/
```

### Comparing `flook-0.2.2/README.rst` & `flook-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/recipe/motd/recipe.yml` & `flook-0.2.3/recipe/motd/recipe.yml`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/recipe/nginx/recipe.yml` & `flook-0.2.3/recipe/nginx/recipe.yml`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/recipe/ping/recipe.yml` & `flook-0.2.3/recipe/ping/recipe.yml`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/setup.cfg` & `flook-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/setup.py` & `flook-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/src/flook/__init__.py` & `flook-0.2.3/src/flook/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/src/flook/cli.py` & `flook-0.2.3/src/flook/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,29 +95,29 @@
     default="",
     help="The password to use to authenticate to the host",
 )
 @click.option(
     "-s",
     "--ssh_private_key_file",
     "ssh_private_key_file",
+    required=False,
     type=click.File(),
-    default="",
     help="Private key file used by ssh",
 )
 @click.option("-t", "--tags", "tags", type=click.STRING, default="", help="Host tags")
 def add(name, connection, ip, port, user, password, ssh_private_key_file, tags):
     host = Host(
         str(uuid.uuid4()),
         name,
         connection,
         ip,
         port,
         user,
         password,
-        ssh_private_key_file.read(),
+        ssh_private_key_file.read() if ssh_private_key_file is not None else "",
         tags.split(",") if "," in tags else [],
         None,
         None,
     )
 
     return Hosts().init().add(host)
```

### Comparing `flook-0.2.2/src/flook/command/__init__.py` & `flook-0.2.3/src/flook/command/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/src/flook/command/configs.py` & `flook-0.2.3/src/flook/command/configs.py`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/src/flook/command/hosts.py` & `flook-0.2.3/src/flook/command/hosts.py`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/src/flook/command/recipes.py` & `flook-0.2.3/src/flook/command/recipes.py`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/src/flook/exception/__init__.py` & `flook-0.2.3/src/flook/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/src/flook/model/__init__.py` & `flook-0.2.3/src/flook/model/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/src/flook/model/host.py` & `flook-0.2.3/src/flook/model/host.py`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/src/flook/model/recipe.py` & `flook-0.2.3/src/flook/model/recipe.py`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/src/flook/model/task.py` & `flook-0.2.3/src/flook/model/task.py`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/src/flook/module/__init__.py` & `flook-0.2.3/src/flook/module/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/src/flook/module/config.py` & `flook-0.2.3/src/flook/module/config.py`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/src/flook/module/database.py` & `flook-0.2.3/src/flook/module/database.py`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/src/flook/module/file_system.py` & `flook-0.2.3/src/flook/module/file_system.py`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/src/flook/module/logger.py` & `flook-0.2.3/src/flook/module/logger.py`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/src/flook/module/output.py` & `flook-0.2.3/src/flook/module/output.py`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/src/flook/module/playbook.py` & `flook-0.2.3/src/flook/module/playbook.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,22 @@
         """Build Playbook"""
         self._file_system.create_dirs("{}/{}".format(self._cache, self._id))
         self._file_system.create_dirs("{}/{}/cache".format(self._cache, self._id))
 
         hosts = "[remote]\n"
 
         for host in self._hosts:
-            if host.password != "":
+
+            if host.connection == "local":
+                hosts = (
+                    hosts
+                    + f"{host.ip} ansible_connection={host.connection} ansible_python_interpreter=python3"
+                )
+
+            elif host.password != "":
                 hosts = (
                     hosts
                     + f"{host.ip} ansible_port={host.port} ansible_connection={host.connection} ansible_user={host.user} ansible_password={host.password} ansible_python_interpreter=python3"
                 )
             else:
                 hosts = (
                     hosts
@@ -76,15 +83,14 @@
                         "{}/{}/{}".format(self._cache, self._id, key), item[key]
                     )
 
             del data["templates"]
 
         base = {
             "hosts": "remote",
-            "become": "yes",
         }
 
         base.update(data)
         playbook = [base]
         self._file_system.write_file(
             "{}/{}/playbook.yml".format(self._cache, self._id), yaml.dump(playbook)
         )
```

### Comparing `flook-0.2.2/src/flook.egg-info/PKG-INFO` & `flook-0.2.3/src/flook.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flook
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Lightweight and Flexible Ansible Command Line Tool.
 Home-page: https://github.com/norwik/flook/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/norwik/flook/
 Project-URL: Source, https://github.com/norwik/flook/
```

### Comparing `flook-0.2.2/src/flook.egg-info/SOURCES.txt` & `flook-0.2.3/src/flook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/tests/__init__.py` & `flook-0.2.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/tests/module/test_logger.py` & `flook-0.2.3/tests/module/test_logger.py`

 * *Files identical despite different names*

### Comparing `flook-0.2.2/tox.ini` & `flook-0.2.3/tox.ini`

 * *Files identical despite different names*

