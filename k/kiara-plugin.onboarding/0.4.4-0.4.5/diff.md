# Comparing `tmp/kiara_plugin.onboarding-0.4.4.tar.gz` & `tmp/kiara_plugin.onboarding-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.onboarding-0.4.4.tar", last modified: Wed May 24 13:48:03 2023, max compression
+gzip compressed data, was "kiara_plugin.onboarding-0.4.5.tar", last modified: Tue Jun 27 10:09:28 2023, max compression
```

## Comparing `kiara_plugin.onboarding-0.4.4.tar` & `kiara_plugin.onboarding-0.4.5.tar`

### file list

```diff
@@ -1,84 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.049426 kiara_plugin.onboarding-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.025426 kiara_plugin.onboarding-0.4.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.037426 kiara_plugin.onboarding-0.4.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.037426 kiara_plugin.onboarding-0.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-24 13:48:03.049426 kiara_plugin.onboarding-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.025426 kiara_plugin.onboarding-0.4.4/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.037426 kiara_plugin.onboarding-0.4.4/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/ci/conda/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.037426 kiara_plugin.onboarding-0.4.4/ci/conda/kiara_plugin.onboarding/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/ci/conda/kiara_plugin.onboarding/meta.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.037426 kiara_plugin.onboarding-0.4.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.037426 kiara_plugin.onboarding-0.4.4/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.025426 kiara_plugin.onboarding-0.4.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.041426 kiara_plugin.onboarding-0.4.4/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.041426 kiara_plugin.onboarding-0.4.4/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/examples/data/journals/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.025426 kiara_plugin.onboarding-0.4.4/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.041426 kiara_plugin.onboarding-0.4.4/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-24 13:48:03.053426 kiara_plugin.onboarding-0.4.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1396 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.029426 kiara_plugin.onboarding-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.029426 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.045426 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.045426 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.045426 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/files/
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/files/import_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/zenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.049426 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.049426 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.049426 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/utils/download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.045426 kiara_plugin.onboarding-0.4.4/src/kiara_plugin.onboarding.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-24 13:48:02.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin.onboarding.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-24 13:48:03.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin.onboarding.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:48:02.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin.onboarding.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-24 13:48:02.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin.onboarding.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:47:16.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin.onboarding.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-24 13:48:02.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin.onboarding.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 13:48:02.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin.onboarding.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.049426 kiara_plugin.onboarding-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      236 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.600107 kiara_plugin.onboarding-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.588106 kiara_plugin.onboarding-0.4.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.592106 kiara_plugin.onboarding-0.4.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.592106 kiara_plugin.onboarding-0.4.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.github/workflows/build-linux.yaml.rej
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-27 10:09:28.600107 kiara_plugin.onboarding-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.588106 kiara_plugin.onboarding-0.4.5/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.592106 kiara_plugin.onboarding-0.4.5/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/ci/conda/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.592106 kiara_plugin.onboarding-0.4.5/ci/conda/kiara_plugin.onboarding/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/ci/conda/kiara_plugin.onboarding/meta.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.588106 kiara_plugin.onboarding-0.4.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/examples/jobs/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/examples/pipelines/example_pipeline_onboarding.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.588106 kiara_plugin.onboarding-0.4.5/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-27 10:09:28.600107 kiara_plugin.onboarding-0.4.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1396 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.588106 kiara_plugin.onboarding-0.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.588106 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/data_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    17482 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/files/import_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/zenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.600107 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/utils/download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.596106 kiara_plugin.onboarding-0.4.5/src/kiara_plugin.onboarding.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-27 10:09:28.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin.onboarding.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-27 10:09:28.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin.onboarding.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:09:28.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin.onboarding.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-27 10:09:28.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin.onboarding.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:08:54.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin.onboarding.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-27 10:09:28.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin.onboarding.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 10:09:28.000000 kiara_plugin.onboarding-0.4.5/src/kiara_plugin.onboarding.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.600107 kiara_plugin.onboarding-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:28.600107 kiara_plugin.onboarding-0.4.5/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/tests/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      236 2023-06-27 10:08:41.000000 kiara_plugin.onboarding-0.4.5/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.onboarding-0.4.4/.cruft.json` & `kiara_plugin.onboarding-0.4.5/.cruft.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'f30a92644095dd13556ab071b97d20008badaed3'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "a49ee6e0061fd08f5758143b229c8816f60bc0d0",
+    "commit": "f30a92644095dd13556ab071b97d20008badaed3",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/DHARPA-Project/kiara_plugin.develop.git",
             "anaconda_user": "dharpa",
             "email": "markus@frkl.io",
             "full_name": "Markus Binsteiner",
             "github_user": "DHARPA-Project",
```

### Comparing `kiara_plugin.onboarding-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.onboarding-0.4.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.4/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.onboarding-0.4.5/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.4/.github/workflows/build-darwin.yaml` & `kiara_plugin.onboarding-0.4.5/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.4/.github/workflows/build-linux.yaml` & `kiara_plugin.onboarding-0.4.5/.github/workflows/build-linux.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     steps:
       - name: "Set up Python ${{ matrix.python_version }}"
         uses: actions/setup-python@v4
         with:
           python-version: "${{ matrix.python_version }}"
       - uses: actions/checkout@v3
       - name: install kiara_plugin.onboarding
-        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ .[all,dev_testing]
+        run: pip install -U .[all,dev_testing]
       - name: display installed kiara and module package versions
         run: pip list | grep kiara
       - name: Test with pytest
         run: make test
 
 # Uncomment this if you have coveralls.io setup with this repo
 #  coverage:
@@ -128,25 +128,25 @@
     needs:
       - test-linux
       - mypy-linux
       - linting-linux
     env:
         GEMFURY_PUSH_TOKEN: ${{ secrets.GEMFURY_PUSH_TOKEN }}
     steps:
-      - name: Set up Python 3.9
+      - name: Set up Python 3.11
         uses: actions/setup-python@v4
         with:
-          python-version: "3.9"
+          python-version: "3.11"
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: install pip
         run: pip install pip==21.2.4 setuptools==57.4.0
       - name: install kiara
-        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ -e .[all]
+        run: pip install -U -e .[all]
       - name: install 'build' package
         run: pip install -U build
       - name: create packages
         run: python -m build
       - name: upload source package
         run: curl -F package=@$(ls dist/kiara*.tar.gz) https://${GEMFURY_PUSH_TOKEN}@dharpa.fury.land:443/pypi/
       - name: upload wheel
```

### Comparing `kiara_plugin.onboarding-0.4.4/.github/workflows/build-windows.yaml` & `kiara_plugin.onboarding-0.4.5/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.4/.gitignore` & `kiara_plugin.onboarding-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.4/.pre-commit-config.yaml` & `kiara_plugin.onboarding-0.4.5/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     files: "^src/"
     pass_filenames: true
     args: ["--config-file", "setup.cfg", "--ignore-missing-imports", "--explicit-package-bases"]
     additional_dependencies: [pydantic>=1.8.0, rich>=10.0.0, ruamel.yaml, anyio>=3.0.0, pyzmq>=22.0.3, bidict, sqlalchemy-stubs, types-python-slugify, types-setuptools, types-python-dateutil, dag_cbor, multiformats, textual, regex, types-pytz, types-orjson]
 
 - repo: https://github.com/charliermarsh/ruff-pre-commit
   # Ruff version.
-  rev: 'v0.0.243'
+  rev: 'v0.0.272'
   hooks:
     - id: ruff
 
 - repo: https://github.com/Kludex/no-optional
   rev: 0.4.0
   hooks:
     - id: no_optional
```

### Comparing `kiara_plugin.onboarding-0.4.4/LICENSE` & `kiara_plugin.onboarding-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.4/Makefile` & `kiara_plugin.onboarding-0.4.5/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.4/PKG-INFO` & `kiara_plugin.onboarding-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.onboarding
-Version: 0.4.4
+Version: 0.4.5
 Summary: kiara modules for data onboarding.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.onboarding
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.onboarding
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.onboarding
 Keywords: kiara
```

### Comparing `kiara_plugin.onboarding-0.4.4/README.md` & `kiara_plugin.onboarding-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.4/ci/conda/kiara_plugin.onboarding/meta.yaml.template` & `kiara_plugin.onboarding-0.4.5/ci/conda/kiara_plugin.onboarding/meta.yaml.template`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.4/docs/development.md` & `kiara_plugin.onboarding-0.4.5/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.4/docs/index.md` & `kiara_plugin.onboarding-0.4.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.4/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.onboarding-0.4.5/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.4/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.onboarding-0.4.5/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.4/mkdocs.yml` & `kiara_plugin.onboarding-0.4.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.4/pyproject.toml` & `kiara_plugin.onboarding-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,19 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 dependencies = [
-    "kiara_plugin.core_types>=0.4.16",
+    "kiara>=0.4.44",
+    "kiara_plugin.core_types>=0.4.20",
     "httpx>=0.23.0",
-    "patool",
-    "pyzenodo3>=1.0.2"
+    "pyzenodo3>=1.0.2",
+    "PyGithub>=1.58.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev_documentation = [
     "kiara[dev_documentation]"
 ]
```

### Comparing `kiara_plugin.onboarding-0.4.4/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.onboarding-0.4.5/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.4/scripts/documentation/gen_info_pages.py` & `kiara_plugin.onboarding-0.4.5/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.4/scripts/documentation/gen_module_doc.py` & `kiara_plugin.onboarding-0.4.5/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.4/setup.cfg` & `kiara_plugin.onboarding-0.4.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 	tests
 
 [aliases]
 build = bdist_wheel
 release = build upload
 
 [bdist_wheel]
-universal = 1
+universal = 0
 
 [devpi:upload]
 no-vcs = 1
 formats = sdist, bdist_wheel
 
 [tool:pytest]
 addopts =
```

### Comparing `kiara_plugin.onboarding-0.4.4/setup.py` & `kiara_plugin.onboarding-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/__init__.py` & `kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/files/__init__.py` & `kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/files/import_file.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,176 +1,180 @@
 # -*- coding: utf-8 -*-
-import atexit
-import os
-import shutil
-import tempfile
-from typing import Any, Dict, Union
-
-from pydantic import Field
-
-from kiara.api import KiaraModule, KiaraModuleConfig, ValueMap, ValueMapSchema
-from kiara.exceptions import KiaraProcessingException
-from kiara.models.filesystem import FileBundle
-from kiara_plugin.onboarding.utils.download import download_file
-
-
-class DownloadFileConfig(KiaraModuleConfig):
-    download_metadata: bool = Field(
-        description="Whether to return the download metadata as well.",
-        default=True,
-    )
-
-
-class DownloadFileModule(KiaraModule):
-    """Download a single file from a remote location.
-
-    The result of this operation is a single value of type 'file' (basically an array of raw bytes), which can then be used in other modules to
-    create more meaningful data structures.
-    """
-
-    _module_type_name = "download.file"
-    _config_cls = DownloadFileConfig
-
-    def create_inputs_schema(self) -> ValueMapSchema:
-
-        result: Dict[str, Dict[str, Any]] = {
-            "url": {"type": "string", "doc": "The url of the file to download."},
-            "file_name": {
-                "type": "string",
-                "doc": "The file name to use for the downloaded file.",
-                "optional": True,
-            },
-        }
-        return result
-
-    def create_outputs_schema(
-        self,
-    ) -> ValueMapSchema:
-
-        result: Dict[str, Dict[str, Any]] = {
-            "file": {
-                "type": "file",
-                "doc": "The downloaded file.",
-            }
-        }
-
-        if self.get_config_value("download_metadata"):
-            result["download_metadata"] = {
-                "type": "dict",
-                "doc": "Metadata about the download.",
-            }
-        return result
-
-    def process(self, inputs: ValueMap, outputs: ValueMap):
-
-        url = inputs.get_value_data("url")
-        file_name = inputs.get_value_data("file_name")
-
-        result_file, metadata = download_file(url=url, file_name=file_name)
-
-        outputs.set_value("download_metadata", metadata)
-        outputs.set_value("file", result_file)
-
-
-class DownloadFileBundleModule(KiaraModule):
-    _module_type_name = "download.file_bundle"
-    _config_cls = DownloadFileConfig
-
-    def create_inputs_schema(self) -> ValueMapSchema:
-
-        result: Dict[str, Dict[str, Any]] = {
-            "url": {
-                "type": "string",
-                "doc": "The url of an archive/zip file to download.",
-            },
-            "sub_path": {
-                "type": "string",
-                "doc": "A relative path to select only a sub-folder from the archive.",
-                "optional": True,
-            },
-        }
-
-        return result
-
-    def create_outputs_schema(
-        self,
-    ) -> ValueMapSchema:
-
-        result: Dict[str, Dict[str, Any]] = {
-            "file_bundle": {
-                "type": "file_bundle",
-                "doc": "The downloaded file bundle.",
-            }
-        }
-
-        if self.get_config_value("download_metadata"):
-            result["download_metadata"] = {
-                "type": "dict",
-                "doc": "Metadata about the download.",
-            }
-        return result
-
-    def process(self, inputs: ValueMap, outputs: ValueMap):
-
-        from datetime import datetime
-        from urllib.parse import urlparse
-
-        import httpx
-        import pytz
-
-        url = inputs.get_value_data("url")
-        suffix = None
-        try:
-            parsed_url = urlparse(url)
-            _, suffix = os.path.splitext(parsed_url.path)
-        except Exception:
-            pass
-        if not suffix:
-            suffix = ""
-
-        sub_path: Union[None, str] = inputs.get_value_data("sub_path")
-        tmp_file = tempfile.NamedTemporaryFile(delete=False, suffix=suffix)
-        atexit.register(tmp_file.close)
-
-        history = []
-        datetime.utcnow().replace(tzinfo=pytz.utc)
-        with open(tmp_file.name, "wb") as f:
-            with httpx.stream("GET", url, follow_redirects=True) as r:
-                history.append(dict(r.headers))
-                for h in r.history:
-                    history.append(dict(h.headers))
-                for data in r.iter_bytes():
-                    f.write(data)
-
-        out_dir = tempfile.mkdtemp()
-
-        def del_out_dir():
-            shutil.rmtree(out_dir, ignore_errors=True)
-
-        atexit.register(del_out_dir)
-
-        error = None
-        try:
-            shutil.unpack_archive(tmp_file.name, out_dir)
-        except Exception:
-            # try patool, maybe we're lucky
-            try:
-                import patoolib
-
-                patoolib.extract_archive(tmp_file.name, outdir=out_dir)
-            except Exception as e:
-                error = e
-
-        if error is not None:
-            raise KiaraProcessingException(f"Could not extract archive: {error}.")
-
-        path = out_dir
-        if sub_path:
-            path = os.path.join(out_dir, sub_path)
-        bundle = FileBundle.import_folder(path)
-
-        metadata = {
-            "response_headers": history,
-            "request_time": datetime.utcnow().replace(tzinfo=pytz.utc).isoformat(),
-        }
-        outputs.set_value("download_metadata", metadata)
-        outputs.set_value("file_bundle", bundle)
+# import atexit
+# import os
+# import shutil
+# import tempfile
+# from typing import Any, Dict, Union
+#
+# from pydantic import Field
+#
+# from kiara.api import KiaraModule, KiaraModuleConfig, ValueMap, ValueMapSchema
+# from kiara.exceptions import KiaraProcessingException
+# from kiara.models.filesystem import FileBundle
+# from kiara_plugin.onboarding.utils.download import download_file
+#
+#
+# class ImportFileConfig(KiaraModuleConfig):
+#
+#     import_metadata: bool = Field(
+#         description="Whether to return the import metadata as well.",
+#         default=True,
+#     )
+#     source_location: Union[str, None] = Field(
+#         description="The location of the source file.", default=None
+#     )
+#
+#
+# class DownloadFileConfig(KiaraModuleConfig):
+#     attach_metadata: bool = Field(
+#         description="Whether to attach the download metadata to the result file.",
+#         default=True,
+#     )
+#
+#
+# class DownloadFileModule(KiaraModule):
+#     """Download a single file from a remote location.
+#
+#     The result of this operation is a single value of type 'file' (basically an array of raw bytes), which can then be used in other modules to
+#     create more meaningful data structures.
+#     """
+#
+#     _module_type_name = "download.file"
+#     _config_cls = DownloadFileConfig
+#
+#     def create_inputs_schema(self) -> ValueMapSchema:
+#
+#         result: Dict[str, Dict[str, Any]] = {
+#             "url": {"type": "string", "doc": "The url of the file to download."},
+#             "file_name": {
+#                 "type": "string",
+#                 "doc": "The file name to use for the downloaded file.",
+#                 "optional": True,
+#             },
+#         }
+#         return result
+#
+#     def create_outputs_schema(
+#         self,
+#     ) -> ValueMapSchema:
+#
+#         result: Dict[str, Dict[str, Any]] = {
+#             "file": {
+#                 "type": "file",
+#                 "doc": "The downloaded file.",
+#             }
+#         }
+#
+#         return result
+#
+#     def process(self, inputs: ValueMap, outputs: ValueMap):
+#
+#         url = inputs.get_value_data("url")
+#         file_name = inputs.get_value_data("file_name")
+#
+#         result_file = download_file(
+#             url=url,
+#             file_name=file_name,
+#             attach_metadata=self.get_config_value("attach_metadata"),
+#         )
+#
+#         outputs.set_value("file", result_file)
+#
+#
+# class DownloadFileBundleModule(KiaraModule):
+#     _module_type_name = "download.file_bundle"
+#     _config_cls = DownloadFileConfig
+#
+#     def create_inputs_schema(self) -> ValueMapSchema:
+#
+#         result: Dict[str, Dict[str, Any]] = {
+#             "url": {
+#                 "type": "string",
+#                 "doc": "The url of an archive/zip file to download.",
+#             },
+#             "sub_path": {
+#                 "type": "string",
+#                 "doc": "A relative path to select only a sub-folder from the archive.",
+#                 "optional": True,
+#             },
+#         }
+#
+#         return result
+#
+#     def create_outputs_schema(
+#         self,
+#     ) -> ValueMapSchema:
+#
+#         result: Dict[str, Dict[str, Any]] = {
+#             "file_bundle": {
+#                 "type": "file_bundle",
+#                 "doc": "The downloaded file bundle.",
+#             }
+#         }
+#
+#         return result
+#
+#     def process(self, inputs: ValueMap, outputs: ValueMap):
+#
+#         from datetime import datetime
+#         from urllib.parse import urlparse
+#
+#         import httpx
+#         import pytz
+#
+#         url = inputs.get_value_data("url")
+#         suffix = None
+#         try:
+#             parsed_url = urlparse(url)
+#             _, suffix = os.path.splitext(parsed_url.path)
+#         except Exception:
+#             pass
+#         if not suffix:
+#             suffix = ""
+#
+#         sub_path: Union[None, str] = inputs.get_value_data("sub_path")
+#         tmp_file = tempfile.NamedTemporaryFile(delete=False, suffix=suffix)
+#         atexit.register(tmp_file.close)
+#
+#         history = []
+#         datetime.utcnow().replace(tzinfo=pytz.utc)
+#         with open(tmp_file.name, "wb") as f:
+#             with httpx.stream("GET", url, follow_redirects=True) as r:
+#                 history.append(dict(r.headers))
+#                 for h in r.history:
+#                     history.append(dict(h.headers))
+#                 for data in r.iter_bytes():
+#                     f.write(data)
+#
+#         out_dir = tempfile.mkdtemp()
+#
+#         def del_out_dir():
+#             shutil.rmtree(out_dir, ignore_errors=True)
+#
+#         atexit.register(del_out_dir)
+#
+#         error = None
+#         try:
+#             shutil.unpack_archive(tmp_file.name, out_dir)
+#         except Exception:
+#             # try patool, maybe we're lucky
+#             try:
+#                 import patoolib
+#
+#                 patoolib.extract_archive(tmp_file.name, outdir=out_dir)
+#             except Exception as e:
+#                 error = e
+#
+#         if error is not None:
+#             raise KiaraProcessingException(f"Could not extract archive: {error}.")
+#
+#         path = out_dir
+#         if sub_path:
+#             path = os.path.join(out_dir, sub_path)
+#         bundle = FileBundle.import_folder(path)
+#
+#         metadata = {
+#             "response_headers": history,
+#             "request_time": datetime.utcnow().replace(tzinfo=pytz.utc).isoformat(),
+#         }
+#         outputs.set_value("download_metadata", metadata)
+#         outputs.set_value("file_bundle", bundle)
```

### Comparing `kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py` & `kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,55 @@
 # -*- coding: utf-8 -*-
-from typing import Any, Dict
 
-from pydantic import Field
 
-from kiara.api import KiaraModule, KiaraModuleConfig, ValueMap, ValueMapSchema
-
-
-class ImportFileBundleConfig(KiaraModuleConfig):
-
-    import_metadata: bool = Field(
-        description="Whether to return the import metadata as well.",
-        default=True,
-    )
-
-
-class ImportFileBundleModule(KiaraModule):
-    """A generic module to import a file bundle from any local or remote location."""
-
-    _module_type_name = "import.file_bundle"
-    _config_cls = ImportFileBundleConfig
-
-    def create_inputs_schema(
-        self,
-    ) -> ValueMapSchema:
-
-        result: Dict[str, Dict[str, Any]] = {
-            "uri": {
-                "type": "string",
-                "doc": "The uri (url/path/...) of the file to import.",
-            }
-        }
-        if self.get_config_value("import_metadata"):
-            result["import_metadata"] = {
-                "type": "dict",
-                "doc": "Metadata you want to attach to the file bundle.",
-                "optional": True,
-            }
-
-        return result
-
-    def create_outputs_schema(
-        self,
-    ) -> ValueMapSchema:
-
-        result = {
-            "file_bundle": {
-                "type": "file_bundle",
-                "doc": "The imported file bundle.",
-            }
-        }
-        if self.get_config_value("import_metadata"):
-            result["import_metadata"] = {
-                "type": "dict",
-                "doc": "Metadata about the import and file bundle.",
-            }
-        return result
-
-    def process(self, inputs: ValueMap, outputs: ValueMap) -> None:
-        pass
+# class ImportFileBundleConfig(KiaraModuleConfig):
+#
+#     import_metadata: bool = Field(
+#         description="Whether to return the import metadata as well.",
+#         default=True,
+#     )
+#
+#
+# class ImportFileBundleModule(KiaraModule):
+#     """A generic module to import a file bundle from any local or remote location."""
+#
+#     _module_type_name = "import.file_bundle"
+#     _config_cls = ImportFileBundleConfig
+#
+#     def create_inputs_schema(
+#         self,
+#     ) -> ValueMapSchema:
+#
+#         result: Dict[str, Dict[str, Any]] = {
+#             "uri": {
+#                 "type": "string",
+#                 "doc": "The uri (url/path/...) of the file to import.",
+#             }
+#         }
+#         if self.get_config_value("import_metadata"):
+#             result["import_metadata"] = {
+#                 "type": "dict",
+#                 "doc": "Metadata you want to attach to the file bundle.",
+#                 "optional": True,
+#             }
+#
+#         return result
+#
+#     def create_outputs_schema(
+#         self,
+#     ) -> ValueMapSchema:
+#
+#         result = {
+#             "file_bundle": {
+#                 "type": "file_bundle",
+#                 "doc": "The imported file bundle.",
+#             }
+#         }
+#         if self.get_config_value("import_metadata"):
+#             result["import_metadata"] = {
+#                 "type": "dict",
+#                 "doc": "Metadata about the import and file bundle.",
+#             }
+#         return result
+#
+#     def process(self, inputs: ValueMap, outputs: ValueMap) -> None:
+#         pass
```

### Comparing `kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/zenodo.py` & `kiara_plugin.onboarding-0.4.5/src/kiara_plugin/onboarding/modules/zenodo.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any, Mapping
 
 import orjson
 from pydantic import Field
 
 from kiara.api import KiaraModule, KiaraModuleConfig, ValueMap, ValueMapSchema
 from kiara.exceptions import KiaraProcessingException
-from kiara.models.filesystem import FileBundle
+from kiara.models.filesystem import KiaraFileBundle
 
 
 class ZenodoDownloadConfig(KiaraModuleConfig):
 
     metadata_filename: str = Field(
         description="The filename for the zenodo metadata.", default="metadata.json"
     )
@@ -87,20 +87,20 @@
         include_metadata = inputs.get_value_data("include_metadata")
 
         doi = inputs.get_value_data("doi")
         zen = pyzenodo3.Zenodo()
 
         record = zen.find_record_by_doi(doi)
 
-        path = FileBundle.create_tmp_dir()
+        path = KiaraFileBundle.create_tmp_dir()
         shutil.rmtree(path, ignore_errors=True)
         path.mkdir()
         for file_data in record.data["files"]:
             self.download_file(file_data, path)
 
         if include_metadata:
             metadata_filename = self.get_config_value("metadata_filename")
             metadata_file = path / metadata_filename
             metadata_file.write_bytes(orjson.dumps(record.data))
 
-        bundle = FileBundle.import_folder(path.as_posix())
+        bundle = KiaraFileBundle.import_folder(path.as_posix())
         outputs.set_value("file_bundle", bundle)
```

### Comparing `kiara_plugin.onboarding-0.4.4/src/kiara_plugin.onboarding.egg-info/PKG-INFO` & `kiara_plugin.onboarding-0.4.5/src/kiara_plugin.onboarding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.onboarding
-Version: 0.4.4
+Version: 0.4.5
 Summary: kiara modules for data onboarding.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.onboarding
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.onboarding
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.onboarding
 Keywords: kiara
```

