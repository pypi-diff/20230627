# Comparing `tmp/python3-pip-skeleton-3.4.0.tar.gz` & `tmp/python3-pip-skeleton-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3-pip-skeleton-3.4.0.tar", last modified: Thu Apr 13 08:15:16 2023, max compression
+gzip compressed data, was "python3-pip-skeleton-3.5.0.tar", last modified: Tue Jun 27 10:01:34 2023, max compression
```

## Comparing `python3-pip-skeleton-3.4.0.tar` & `python3-pip-skeleton-3.5.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.550402 python3-pip-skeleton-3.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.542403 python3-pip-skeleton-3.4.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.542403 python3-pip-skeleton-3.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.538402 python3-pip-skeleton-3.4.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.542403 python3-pip-skeleton-3.4.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.542403 python3-pip-skeleton-3.4.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.542403 python3-pip-skeleton-3.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.542403 python3-pip-skeleton-3.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-04-13 08:15:16.550402 python3-pip-skeleton-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.542403 python3-pip-skeleton-3.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.542403 python3-pip-skeleton-3.4.0/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.542403 python3-pip-skeleton-3.4.0/docs/developer/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/explanations/skeleton.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.546403 python3-pip-skeleton-3.4.0/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.546403 python3-pip-skeleton-3.4.0/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.546403 python3-pip-skeleton-3.4.0/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.546403 python3-pip-skeleton-3.4.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/images/excalidraw-example.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/images/git_merge.png
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.546403 python3-pip-skeleton-3.4.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.546403 python3-pip-skeleton-3.4.0/docs/user/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.546403 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0003-docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0004-why-src.rst
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0005-pyproject-toml.rst
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0006-setuptools-scm.rst
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0007-dev-dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0008-use-tox.rst
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0009-sphinx-theme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0010-vscode-settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0011-requirements-txt.rst
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0012-containers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/explanations/why-use-skeleton.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.550402 python3-pip-skeleton-3.4.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/how-to/excalidraw.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/how-to/existing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/how-to/maintain-your-own-skeleton.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/how-to/pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/how-to/update.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.550402 python3-pip-skeleton-3.4.0/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.550402 python3-pip-skeleton-3.4.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/tutorials/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/docs/user/tutorials/new.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:15:16.550402 python3-pip-skeleton-3.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.538402 python3-pip-skeleton-3.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.550402 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 08:15:16.000000 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.550402 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-04-13 08:15:16.000000 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-13 08:15:16.000000 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:15:16.000000 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 08:15:16.000000 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-13 08:15:16.000000 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 08:15:16.000000 python3-pip-skeleton-3.4.0/src/python3_pip_skeleton.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:15:16.550402 python3-pip-skeleton-3.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10005 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/tests/test_adopt.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-13 08:15:02.000000 python3-pip-skeleton-3.4.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.335068 python3-pip-skeleton-3.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.319068 python3-pip-skeleton-3.5.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.323068 python3-pip-skeleton-3.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.315068 python3-pip-skeleton-3.5.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.323068 python3-pip-skeleton-3.5.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.323068 python3-pip-skeleton-3.5.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.323068 python3-pip-skeleton-3.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.323068 python3-pip-skeleton-3.5.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-06-27 10:01:34.335068 python3-pip-skeleton-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.323068 python3-pip-skeleton-3.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.323068 python3-pip-skeleton-3.5.0/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.323068 python3-pip-skeleton-3.5.0/docs/developer/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/developer/explanations/skeleton.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.327068 python3-pip-skeleton-3.5.0/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.327068 python3-pip-skeleton-3.5.0/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.327068 python3-pip-skeleton-3.5.0/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.327068 python3-pip-skeleton-3.5.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/images/excalidraw-example.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/images/git_merge.png
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.327068 python3-pip-skeleton-3.5.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.327068 python3-pip-skeleton-3.5.0/docs/user/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.331068 python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/0003-docs-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/0004-why-src.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/0005-pyproject-toml.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/0006-setuptools-scm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/0007-dev-dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/0008-use-tox.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/0009-sphinx-theme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/0010-vscode-settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/0011-requirements-txt.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/0012-containers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/explanations/decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/explanations/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/explanations/why-use-skeleton.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.331068 python3-pip-skeleton-3.5.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/how-to/excalidraw.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/how-to/existing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/how-to/maintain-your-own-skeleton.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/how-to/pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/how-to/update.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.331068 python3-pip-skeleton-3.5.0/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.331068 python3-pip-skeleton-3.5.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/tutorials/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/docs/user/tutorials/new.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 10:01:34.335068 python3-pip-skeleton-3.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.319068 python3-pip-skeleton-3.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.331068 python3-pip-skeleton-3.5.0/src/python3_pip_skeleton/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/src/python3_pip_skeleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/src/python3_pip_skeleton/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-27 10:01:34.000000 python3-pip-skeleton-3.5.0/src/python3_pip_skeleton/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.331068 python3-pip-skeleton-3.5.0/src/python3_pip_skeleton.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-06-27 10:01:34.000000 python3-pip-skeleton-3.5.0/src/python3_pip_skeleton.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-27 10:01:34.000000 python3-pip-skeleton-3.5.0/src/python3_pip_skeleton.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:01:34.000000 python3-pip-skeleton-3.5.0/src/python3_pip_skeleton.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-27 10:01:34.000000 python3-pip-skeleton-3.5.0/src/python3_pip_skeleton.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-27 10:01:34.000000 python3-pip-skeleton-3.5.0/src/python3_pip_skeleton.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 10:01:34.000000 python3-pip-skeleton-3.5.0/src/python3_pip_skeleton.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:01:34.335068 python3-pip-skeleton-3.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10005 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/tests/test_adopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-27 10:01:22.000000 python3-pip-skeleton-3.5.0/tests/test_cli.py
```

### Comparing `python3-pip-skeleton-3.4.0/.devcontainer/devcontainer.json` & `python3-pip-skeleton-3.5.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/.github/CONTRIBUTING.rst` & `python3-pip-skeleton-3.5.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/.github/actions/install_requirements/action.yml` & `python3-pip-skeleton-3.5.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/.github/dependabot.yml` & `python3-pip-skeleton-3.5.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/.github/pages/make_switcher.py` & `python3-pip-skeleton-3.5.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/.github/workflows/code.yml` & `python3-pip-skeleton-3.5.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/.github/workflows/docs.yml` & `python3-pip-skeleton-3.5.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/.github/workflows/docs_clean.yml` & `python3-pip-skeleton-3.5.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/.github/workflows/linkcheck.yml` & `python3-pip-skeleton-3.5.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/.gitignore` & `python3-pip-skeleton-3.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/.vscode/launch.json` & `python3-pip-skeleton-3.5.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/Dockerfile` & `python3-pip-skeleton-3.5.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/LICENSE` & `python3-pip-skeleton-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/PKG-INFO` & `python3-pip-skeleton-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-pip-skeleton
-Version: 3.4.0
+Version: 3.5.0
 Summary: One line description of your module
 Author-email: Firstname Lastname <email@address.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `python3-pip-skeleton-3.4.0/README.rst` & `python3-pip-skeleton-3.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/conf.py` & `python3-pip-skeleton-3.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/developer/explanations/skeleton.rst` & `python3-pip-skeleton-3.5.0/docs/developer/explanations/skeleton.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/developer/how-to/build-docs.rst` & `python3-pip-skeleton-3.5.0/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/developer/how-to/lint.rst` & `python3-pip-skeleton-3.5.0/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/developer/how-to/make-release.rst` & `python3-pip-skeleton-3.5.0/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/developer/how-to/pin-requirements.rst` & `python3-pip-skeleton-3.5.0/docs/developer/how-to/pin-requirements.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/developer/how-to/test-container.rst` & `python3-pip-skeleton-3.5.0/docs/developer/how-to/test-container.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/developer/how-to/update-tools.rst` & `python3-pip-skeleton-3.5.0/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/developer/index.rst` & `python3-pip-skeleton-3.5.0/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/developer/reference/standards.rst` & `python3-pip-skeleton-3.5.0/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/developer/tutorials/dev-install.rst` & `python3-pip-skeleton-3.5.0/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/images/dls-favicon.ico` & `python3-pip-skeleton-3.5.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/images/dls-logo.svg` & `python3-pip-skeleton-3.5.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/images/excalidraw-example.svg` & `python3-pip-skeleton-3.5.0/docs/images/excalidraw-example.svg`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/images/git_merge.png` & `python3-pip-skeleton-3.5.0/docs/images/git_merge.png`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/index.rst` & `python3-pip-skeleton-3.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0003-docs-structure.rst` & `python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/0003-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0004-why-src.rst` & `python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/0004-why-src.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0006-setuptools-scm.rst` & `python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/0006-setuptools-scm.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0007-dev-dependencies.rst` & `python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/0007-dev-dependencies.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0008-use-tox.rst` & `python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/0008-use-tox.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0010-vscode-settings.rst` & `python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/0010-vscode-settings.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0011-requirements-txt.rst` & `python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/0011-requirements-txt.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/user/explanations/decisions/0012-containers.rst` & `python3-pip-skeleton-3.5.0/docs/user/explanations/decisions/0012-containers.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/user/explanations/decisions.rst` & `python3-pip-skeleton-3.5.0/docs/user/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/user/explanations/structure.rst` & `python3-pip-skeleton-3.5.0/docs/user/explanations/structure.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/user/explanations/why-use-skeleton.rst` & `python3-pip-skeleton-3.5.0/docs/user/explanations/why-use-skeleton.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/user/how-to/excalidraw.rst` & `python3-pip-skeleton-3.5.0/docs/user/how-to/excalidraw.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/user/how-to/existing.rst` & `python3-pip-skeleton-3.5.0/docs/user/how-to/existing.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/user/how-to/maintain-your-own-skeleton.rst` & `python3-pip-skeleton-3.5.0/docs/user/how-to/maintain-your-own-skeleton.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/user/how-to/pypi.rst` & `python3-pip-skeleton-3.5.0/docs/user/how-to/pypi.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/user/how-to/update.rst` & `python3-pip-skeleton-3.5.0/docs/user/how-to/update.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/user/index.rst` & `python3-pip-skeleton-3.5.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/user/tutorials/installation.rst` & `python3-pip-skeleton-3.5.0/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/docs/user/tutorials/new.rst` & `python3-pip-skeleton-3.5.0/docs/user/tutorials/new.rst`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/pyproject.toml` & `python3-pip-skeleton-3.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/src/python3_pip_skeleton/__main__.py` & `python3-pip-skeleton-3.5.0/src/python3_pip_skeleton/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 import re
 import shutil
 from argparse import ArgumentParser
 from configparser import ConfigParser
 from pathlib import Path
 from subprocess import STDOUT, CalledProcessError, call, check_output
 from tempfile import TemporaryDirectory
-from typing import List
+from typing import Callable, Dict, List, Tuple
 
 import tomli
 
 from . import __version__
 
 __all__ = ["main"]
 
 # The url of the default skeleton module to pull from, a different skeleton
 # url can be passed in with --skeleton-git-url
 SKELETON_URL = "https://github.com/%s/python3-pip-skeleton"
 # The name of the merge branch that will be created
 MERGE_BRANCH = "skeleton-merge-branch"
 # Extensions to change
 CHANGE_SUFFIXES = [".py", ".rst", ".cfg", "", ".toml"]
-# Files not to change
-IGNORE_FILES = [
-    "test_boilerplate_removed.py",
-    "pin-requirements.rst",
-    "update-tools.rst",
-]
+# Files not to change where IGNORE_FILES[x] is a list of tuples where substitutions
+# will be ignored in that file in any substring between the two strings.
+# An empty list will ignore the whole file.
+IGNORE_FILES: Dict[str, List[Tuple[str, str]]] = {
+    "update-tools.rst": [],
+    "test_boilerplate_removed.py": [
+        ("import sys", "def test_module_summary"),
+        ("One line description of your", "features and why people should use it"),
+    ],
+    "pin-requirements.rst": [],
+    "0002-switched-to-pip-skeleton.rst:": [],
+    "README.rst": [
+        ("adopt this skeleton project see", "that describes what your module does")
+    ],
+}
 
 SKELETON_ROOT_COMMIT = "ededf00035e6ccfac78946213009c1ecd7c110a9"
 
 
 def git(*args, cwd=None) -> str:
     command = ["git"] + [str(x) for x in args]
     try:
@@ -50,14 +59,56 @@
     def __call__(self, *args) -> str:
         return git(*args, cwd=self.name)
 
     def __truediv__(self, other) -> Path:
         return Path(self.name) / other
 
 
+def find_ignore_sections(
+    file_name: str, file_text: str, ignore_sections: List[Tuple[str, str]]
+) -> List[re.Match]:
+    ignore_section_matches = []
+    for sub_strings in ignore_sections:
+        pre_sub_string, post_sub_string = sub_strings
+        regex = rf"(?s){pre_sub_string}(.*?){post_sub_string}"
+        # finditer so we can throw an error if the used ignore strings ignore
+        # more than once in the file
+        original_substrings = list(re.finditer(regex, file_text))
+        assert original_substrings, (
+            f"could not find substrings {pre_sub_string} or "
+            f"{post_sub_string} in {file_name}."
+        )
+        assert len(original_substrings) == 1, (
+            f"multiple substrings found between {pre_sub_string} and "
+            f"{post_sub_string} in {file_name}."
+        )
+        ignore_section_matches.append(original_substrings[0])
+
+    ignore_section_matches.sort(key=lambda x: x.start())
+    return ignore_section_matches
+
+
+def replace_text_ignoring_sections(
+    text: str,
+    ignore_section_matches: List[re.Match],
+    text_replacement_method: Callable,
+) -> str:
+    replacement_text = ""
+    next_start = 0
+    for ignore_section in ignore_section_matches:
+        replacement_text += text_replacement_method(
+            text[next_start : ignore_section.start()]
+        )
+        replacement_text += text[ignore_section.start() : ignore_section.end()]
+        next_start = ignore_section.end()
+
+    replacement_text += text_replacement_method(text[next_start : len(text)])
+    return replacement_text
+
+
 def merge_skeleton(
     path: Path,
     org: str,
     full_name: str,
     email: str,
     from_branch: str,
     skeleton_org: str,
@@ -102,14 +153,29 @@
             git_tmp("mv", "src/python3_pip_skeleton", f"src/{package}")
         # Change contents of all children known to git
         for relative_child in git_tmp("ls-files").splitlines():
             child = Path(git_tmp.name) / relative_child
             if child.suffix in CHANGE_SUFFIXES and child.name not in IGNORE_FILES:
                 text = replace_text(child.read_text())
                 child.write_text(text)
+            # Replace the file, ignoring text between specified substrings
+            elif (
+                child.suffix in CHANGE_SUFFIXES
+                and child.name in IGNORE_FILES
+                and IGNORE_FILES[child.name]
+            ):
+                original_text = child.read_text()
+                ignore_sections = find_ignore_sections(
+                    child.name, original_text, IGNORE_FILES[child.name]
+                )
+                child.write_text(
+                    replace_text_ignoring_sections(
+                        original_text, ignore_sections, replace_text
+                    )
+                )
 
         # Change instructions in the docs to reflect which pip skeleton is in use
         replace_in_file(
             Path(git_tmp.name) / "docs/developer/how-to/update-tools.rst",
             "DiamondLightSource",
             skeleton_org,
         )
```

### Comparing `python3-pip-skeleton-3.4.0/src/python3_pip_skeleton.egg-info/PKG-INFO` & `python3-pip-skeleton-3.5.0/src/python3_pip_skeleton.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-pip-skeleton
-Version: 3.4.0
+Version: 3.5.0
 Summary: One line description of your module
 Author-email: Firstname Lastname <email@address.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `python3-pip-skeleton-3.4.0/src/python3_pip_skeleton.egg-info/SOURCES.txt` & `python3-pip-skeleton-3.5.0/src/python3_pip_skeleton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python3-pip-skeleton-3.4.0/tests/test_adopt.py` & `python3-pip-skeleton-3.5.0/tests/test_adopt.py`

 * *Files identical despite different names*

