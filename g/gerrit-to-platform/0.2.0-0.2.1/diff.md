# Comparing `tmp/gerrit-to-platform-0.2.0.tar.gz` & `tmp/gerrit-to-platform-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerrit-to-platform-0.2.0.tar", last modified: Thu Jun 15 18:00:54 2023, max compression
+gzip compressed data, was "gerrit-to-platform-0.2.1.tar", last modified: Tue Jun 27 21:00:17 2023, max compression
```

## Comparing `gerrit-to-platform-0.2.0.tar` & `gerrit-to-platform-0.2.1.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.253065 gerrit-to-platform-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.225065 gerrit-to-platform-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.237065 gerrit-to-platform-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.github/workflows/gerrit-verify.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.gitreview
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-06-15 18:00:54.253065 gerrit-to-platform-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.241065 gerrit-to-platform-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.241065 gerrit-to-platform-0.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/conf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/onboard.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/docs/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/license-header.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.225065 gerrit-to-platform-0.2.0/releasenotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.241065 gerrit-to-platform-0.2.0/releasenotes/notes/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/releasenotes/notes/initial_release-eb04a5f0690afc15.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/releasenotes/notes/only-file-names-f0e5c44c8f62bca4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/releasenotes/notes/required_workflows-859326ccaa55da24.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 18:00:54.253065 gerrit-to-platform-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.225065 gerrit-to-platform-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.245065 gerrit-to-platform-0.2.0/src/gerrit_to_platform/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform/change_merged.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform/comment_added.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform/patchset_created.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.245065 gerrit-to-platform-0.2.0/src/gerrit_to_platform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-06-15 18:00:54.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-15 18:00:54.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 18:00:54.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-15 18:00:54.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 18:00:54.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 18:00:54.000000 gerrit-to-platform-0.2.0/src/gerrit_to_platform.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.249065 gerrit-to-platform-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:00:54.249065 gerrit-to-platform-0.2.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/github_workflow_empty_list.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/github_workflow_empty_list_get_workflows_return.json
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/github_workflow_list.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/github_workflow_list_filter_workflows_return.json
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/github_workflow_list_filter_workflows_return_merge.json
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/github_workflow_list_get_workflows_return.json
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/github_workflow_list_required_filter_workflows_return.json
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/limited_replication_remotes_return_github.json
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/limited_replication_remotes_return_gitlab.json
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/replication.config
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/replication_remotes_return.json
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/fixtures/testconfig.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/test_change_merged.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/test_comment_added.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tests/test_patchset_created.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-15 18:00:42.000000 gerrit-to-platform-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:00:17.877076 gerrit-to-platform-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:00:17.857075 gerrit-to-platform-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:00:17.865075 gerrit-to-platform-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/.github/workflows/gerrit-verify.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/.gitreview
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-06-27 21:00:17.877076 gerrit-to-platform-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:00:17.869076 gerrit-to-platform-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:00:17.869076 gerrit-to-platform-0.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/docs/conf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/docs/onboard.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/docs/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/license-header.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:00:17.857075 gerrit-to-platform-0.2.1/releasenotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:00:17.869076 gerrit-to-platform-0.2.1/releasenotes/notes/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/releasenotes/notes/fix_required_branch_ref-5895658b99c9721b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/releasenotes/notes/initial_release-eb04a5f0690afc15.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/releasenotes/notes/only-file-names-f0e5c44c8f62bca4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/releasenotes/notes/required_workflows-859326ccaa55da24.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 21:00:17.877076 gerrit-to-platform-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:00:17.857075 gerrit-to-platform-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:00:17.873076 gerrit-to-platform-0.2.1/src/gerrit_to_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/src/gerrit_to_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/src/gerrit_to_platform/change_merged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/src/gerrit_to_platform/comment_added.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/src/gerrit_to_platform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/src/gerrit_to_platform/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/src/gerrit_to_platform/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/src/gerrit_to_platform/patchset_created.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:00:17.873076 gerrit-to-platform-0.2.1/src/gerrit_to_platform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-06-27 21:00:17.000000 gerrit-to-platform-0.2.1/src/gerrit_to_platform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-27 21:00:17.000000 gerrit-to-platform-0.2.1/src/gerrit_to_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:00:17.000000 gerrit-to-platform-0.2.1/src/gerrit_to_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-27 21:00:17.000000 gerrit-to-platform-0.2.1/src/gerrit_to_platform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-27 21:00:17.000000 gerrit-to-platform-0.2.1/src/gerrit_to_platform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-27 21:00:17.000000 gerrit-to-platform-0.2.1/src/gerrit_to_platform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:00:17.873076 gerrit-to-platform-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:00:17.877076 gerrit-to-platform-0.2.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tests/fixtures/github_workflow_empty_list.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tests/fixtures/github_workflow_empty_list_get_workflows_return.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tests/fixtures/github_workflow_list.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tests/fixtures/github_workflow_list_filter_workflows_return.json
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tests/fixtures/github_workflow_list_filter_workflows_return_merge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tests/fixtures/github_workflow_list_get_workflows_return.json
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tests/fixtures/github_workflow_list_required_filter_workflows_return.json
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tests/fixtures/limited_replication_remotes_return_github.json
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tests/fixtures/limited_replication_remotes_return_gitlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tests/fixtures/replication.config
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tests/fixtures/replication_remotes_return.json
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tests/fixtures/testconfig.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tests/test_change_merged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tests/test_comment_added.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tests/test_patchset_created.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-27 21:00:03.000000 gerrit-to-platform-0.2.1/tox.ini
```

### Comparing `gerrit-to-platform-0.2.0/.coveragerc` & `gerrit-to-platform-0.2.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/.github/workflows/codeql.yaml` & `gerrit-to-platform-0.2.1/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/.github/workflows/gerrit-verify.yaml` & `gerrit-to-platform-0.2.1/.github/workflows/gerrit-verify.yaml`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/.github/workflows/release.yaml` & `gerrit-to-platform-0.2.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/.gitignore` & `gerrit-to-platform-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/.gitlint` & `gerrit-to-platform-0.2.1/.gitlint`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/.pre-commit-config.yaml` & `gerrit-to-platform-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/.readthedocs.yml` & `gerrit-to-platform-0.2.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/CONTRIBUTING.rst` & `gerrit-to-platform-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/LICENSE.txt` & `gerrit-to-platform-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/PKG-INFO` & `gerrit-to-platform-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerrit-to-platform
-Version: 0.2.0
+Version: 0.2.1
 Summary: Gerrit to GitHub / GitLab
 Author-email: Andrew Grimberg <agrimberg@linuxfoundation.org>
 Maintainer-email: Andrew Grimberg <agrimberg@linuxfoundation.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `gerrit-to-platform-0.2.0/README.rst` & `gerrit-to-platform-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/docs/Makefile` & `gerrit-to-platform-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/docs/_static/logo.png` & `gerrit-to-platform-0.2.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/docs/conf.py` & `gerrit-to-platform-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/docs/index.rst` & `gerrit-to-platform-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/docs/onboard.rst` & `gerrit-to-platform-0.2.1/docs/onboard.rst`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/docs/troubleshooting.rst` & `gerrit-to-platform-0.2.1/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/pyproject.toml` & `gerrit-to-platform-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/src/gerrit_to_platform/__init__.py` & `gerrit-to-platform-0.2.1/src/gerrit_to_platform/__init__.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/src/gerrit_to_platform/change_merged.py` & `gerrit-to-platform-0.2.1/src/gerrit_to_platform/change_merged.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/src/gerrit_to_platform/comment_added.py` & `gerrit-to-platform-0.2.1/src/gerrit_to_platform/comment_added.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/src/gerrit_to_platform/config.py` & `gerrit-to-platform-0.2.1/src/gerrit_to_platform/config.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/src/gerrit_to_platform/github.py` & `gerrit-to-platform-0.2.1/src/gerrit_to_platform/github.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/src/gerrit_to_platform/helpers.py` & `gerrit-to-platform-0.2.1/src/gerrit_to_platform/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
                         + f"{inputs['GERRIT_PATCHSET_NUMBER']} against "
                         + f"{platform.value}:{owner}/{repo}"
                     )
                     dispatcher(
                         owner,
                         magic_repo,
                         workflow["id"],
-                        f"refs/heads/{inputs['GERRIT_BRANCH']}",
+                        "refs/heads/main",
                         inputs,
                     )
 
 
 def get_change_id(change: str) -> str:
     """
     Get the Gerrit change_id from an hook event.
```

### Comparing `gerrit-to-platform-0.2.0/src/gerrit_to_platform/patchset_created.py` & `gerrit-to-platform-0.2.1/src/gerrit_to_platform/patchset_created.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/src/gerrit_to_platform.egg-info/PKG-INFO` & `gerrit-to-platform-0.2.1/src/gerrit_to_platform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerrit-to-platform
-Version: 0.2.0
+Version: 0.2.1
 Summary: Gerrit to GitHub / GitLab
 Author-email: Andrew Grimberg <agrimberg@linuxfoundation.org>
 Maintainer-email: Andrew Grimberg <agrimberg@linuxfoundation.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `gerrit-to-platform-0.2.0/src/gerrit_to_platform.egg-info/SOURCES.txt` & `gerrit-to-platform-0.2.1/src/gerrit_to_platform.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 docs/license.rst
 docs/onboard.rst
 docs/readme.rst
 docs/requirements.txt
 docs/troubleshooting.rst
 docs/_static/.gitignore
 docs/_static/logo.png
+releasenotes/notes/fix_required_branch_ref-5895658b99c9721b.yaml
 releasenotes/notes/initial_release-eb04a5f0690afc15.yaml
 releasenotes/notes/only-file-names-f0e5c44c8f62bca4.yaml
 releasenotes/notes/required_workflows-859326ccaa55da24.yaml
 src/gerrit_to_platform/__init__.py
 src/gerrit_to_platform/change_merged.py
 src/gerrit_to_platform/comment_added.py
 src/gerrit_to_platform/config.py
```

### Comparing `gerrit-to-platform-0.2.0/tests/conftest.py` & `gerrit-to-platform-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/tests/fixtures/github_workflow_list.json` & `gerrit-to-platform-0.2.1/tests/fixtures/github_workflow_list.json`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/tests/fixtures/github_workflow_list_get_workflows_return.json` & `gerrit-to-platform-0.2.1/tests/fixtures/github_workflow_list_get_workflows_return.json`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/tests/fixtures/replication.config` & `gerrit-to-platform-0.2.1/tests/fixtures/replication.config`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/tests/test_change_merged.py` & `gerrit-to-platform-0.2.1/tests/test_change_merged.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/tests/test_comment_added.py` & `gerrit-to-platform-0.2.1/tests/test_comment_added.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/tests/test_config.py` & `gerrit-to-platform-0.2.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/tests/test_github.py` & `gerrit-to-platform-0.2.1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/tests/test_helpers.py` & `gerrit-to-platform-0.2.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/tests/test_patchset_created.py` & `gerrit-to-platform-0.2.1/tests/test_patchset_created.py`

 * *Files identical despite different names*

### Comparing `gerrit-to-platform-0.2.0/tox.ini` & `gerrit-to-platform-0.2.1/tox.ini`

 * *Files identical despite different names*

