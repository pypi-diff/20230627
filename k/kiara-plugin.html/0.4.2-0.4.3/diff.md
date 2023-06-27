# Comparing `tmp/kiara_plugin.html-0.4.2.tar.gz` & `tmp/kiara_plugin.html-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.html-0.4.2.tar", last modified: Wed Jun 21 10:03:58 2023, max compression
+gzip compressed data, was "kiara_plugin.html-0.4.3.tar", last modified: Tue Jun 27 10:09:45 2023, max compression
```

## Comparing `kiara_plugin.html-0.4.2.tar` & `kiara_plugin.html-0.4.3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.935572 kiara_plugin.html-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.923573 kiara_plugin.html-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.927573 kiara_plugin.html-0.4.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.927573 kiara_plugin.html-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-21 10:03:58.935572 kiara_plugin.html-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.923573 kiara_plugin.html-0.4.2/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.927573 kiara_plugin.html-0.4.2/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/ci/conda/conda-pkg-patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.927573 kiara_plugin.html-0.4.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33398 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/examples/jobs/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/examples/pipelines/example_pipeline_html.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.927573 kiara_plugin.html-0.4.2/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-21 10:03:58.935572 kiara_plugin.html-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.927573 kiara_plugin.html-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.927573 kiara_plugin.html-0.4.2/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/interfaces/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/interfaces/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/modules/core_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/modules/included_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/modules/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/renderers/lineage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.927573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/templates/lineage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/templates/lineage/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/templates/lineage/assets/json-fomatter.js
--rw-r--r--   0 runner    (1001) docker     (123)    31573 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/templates/lineage/assets/msgpack.js
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/templates/lineage/lineage.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.931573 kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-21 10:03:58.000000 kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-21 10:03:58.000000 kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:03:58.000000 kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-21 10:03:58.000000 kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:03:30.000000 kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-21 10:03:58.000000 kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 10:03:58.000000 kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.935572 kiara_plugin.html-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:58.935572 kiara_plugin.html-0.4.2/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      218 2023-06-21 10:03:22.000000 kiara_plugin.html-0.4.2/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.394141 kiara_plugin.html-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.382141 kiara_plugin.html-0.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.390141 kiara_plugin.html-0.4.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.390141 kiara_plugin.html-0.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-27 10:09:45.394141 kiara_plugin.html-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.382141 kiara_plugin.html-0.4.3/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.390141 kiara_plugin.html-0.4.3/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/ci/conda/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.390141 kiara_plugin.html-0.4.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.390141 kiara_plugin.html-0.4.3/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.382141 kiara_plugin.html-0.4.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.390141 kiara_plugin.html-0.4.3/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.390141 kiara_plugin.html-0.4.3/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33398 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.390141 kiara_plugin.html-0.4.3/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/examples/jobs/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.390141 kiara_plugin.html-0.4.3/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/examples/pipelines/example_pipeline_html.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.382141 kiara_plugin.html-0.4.3/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.390141 kiara_plugin.html-0.4.3/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-27 10:09:45.398141 kiara_plugin.html-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.386141 kiara_plugin.html-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.386141 kiara_plugin.html-0.4.3/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.394141 kiara_plugin.html-0.4.3/src/kiara_plugin/html/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/src/kiara_plugin/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/src/kiara_plugin/html/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/src/kiara_plugin/html/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.394141 kiara_plugin.html-0.4.3/src/kiara_plugin/html/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/src/kiara_plugin/html/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.394141 kiara_plugin.html-0.4.3/src/kiara_plugin/html/interfaces/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/src/kiara_plugin/html/interfaces/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.394141 kiara_plugin.html-0.4.3/src/kiara_plugin/html/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/src/kiara_plugin/html/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.394141 kiara_plugin.html-0.4.3/src/kiara_plugin/html/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/src/kiara_plugin/html/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/src/kiara_plugin/html/modules/core_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/src/kiara_plugin/html/modules/included_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/src/kiara_plugin/html/modules/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.394141 kiara_plugin.html-0.4.3/src/kiara_plugin/html/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/src/kiara_plugin/html/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/src/kiara_plugin/html/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/src/kiara_plugin/html/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.394141 kiara_plugin.html-0.4.3/src/kiara_plugin/html/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/src/kiara_plugin/html/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/src/kiara_plugin/html/renderers/lineage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.394141 kiara_plugin.html-0.4.3/src/kiara_plugin/html/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/src/kiara_plugin/html/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.386141 kiara_plugin.html-0.4.3/src/kiara_plugin/html/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.394141 kiara_plugin.html-0.4.3/src/kiara_plugin/html/resources/templates/lineage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.394141 kiara_plugin.html-0.4.3/src/kiara_plugin/html/resources/templates/lineage/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/src/kiara_plugin/html/resources/templates/lineage/assets/json-fomatter.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31573 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/src/kiara_plugin/html/resources/templates/lineage/assets/msgpack.js
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/src/kiara_plugin/html/resources/templates/lineage/lineage.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.390141 kiara_plugin.html-0.4.3/src/kiara_plugin.html.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-27 10:09:45.000000 kiara_plugin.html-0.4.3/src/kiara_plugin.html.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-27 10:09:45.000000 kiara_plugin.html-0.4.3/src/kiara_plugin.html.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:09:45.000000 kiara_plugin.html-0.4.3/src/kiara_plugin.html.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-27 10:09:45.000000 kiara_plugin.html-0.4.3/src/kiara_plugin.html.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:09:17.000000 kiara_plugin.html-0.4.3/src/kiara_plugin.html.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-27 10:09:45.000000 kiara_plugin.html-0.4.3/src/kiara_plugin.html.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 10:09:45.000000 kiara_plugin.html-0.4.3/src/kiara_plugin.html.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.394141 kiara_plugin.html-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:45.394141 kiara_plugin.html-0.4.3/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/tests/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      218 2023-06-27 10:09:06.000000 kiara_plugin.html-0.4.3/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.html-0.4.2/.cruft.json` & `kiara_plugin.html-0.4.3/.cruft.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.html-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.html-0.4.3/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/.github/workflows/build-darwin.yaml` & `kiara_plugin.html-0.4.3/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/.github/workflows/build-linux.yaml` & `kiara_plugin.html-0.4.3/.github/workflows/build-linux.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/.github/workflows/build-windows.yaml` & `kiara_plugin.html-0.4.3/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/.gitignore` & `kiara_plugin.html-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/.pre-commit-config.yaml` & `kiara_plugin.html-0.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/LICENSE` & `kiara_plugin.html-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/Makefile` & `kiara_plugin.html-0.4.3/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/PKG-INFO` & `kiara_plugin.html-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.html
-Version: 0.4.2
+Version: 0.4.3
 Summary: Kiara plugin for html-related tasks.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.html
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.html
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.html
 Keywords: kiara
```

### Comparing `kiara_plugin.html-0.4.2/README.md` & `kiara_plugin.html-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/docs/development.md` & `kiara_plugin.html-0.4.3/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/docs/index.md` & `kiara_plugin.html-0.4.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.html-0.4.3/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.html-0.4.3/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/examples/pipelines/example_pipeline_html.yaml` & `kiara_plugin.html-0.4.3/examples/pipelines/example_pipeline_html.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/mkdocs.yml` & `kiara_plugin.html-0.4.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/pyproject.toml` & `kiara_plugin.html-0.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 dependencies = [
-    "kiara>=0.4.41",
+    "kiara>=0.4.44",
     "kiara_plugin.core_types>=0.4.20",
     "hypercorn",
     "json2html>=1.3.0",
     "markdown>=3.2.1",
     "pymdown-extensions>=9.9",
     "airium>=0.2.3"
 ]
```

### Comparing `kiara_plugin.html-0.4.2/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.html-0.4.3/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/scripts/documentation/gen_info_pages.py` & `kiara_plugin.html-0.4.3/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/scripts/documentation/gen_module_doc.py` & `kiara_plugin.html-0.4.3/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/setup.cfg` & `kiara_plugin.html-0.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/src/kiara_plugin/html/__init__.py` & `kiara_plugin.html-0.4.3/src/kiara_plugin/html/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/src/kiara_plugin/html/defaults.py` & `kiara_plugin.html-0.4.3/src/kiara_plugin/html/defaults.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/src/kiara_plugin/html/models/__init__.py` & `kiara_plugin.html-0.4.3/src/kiara_plugin/html/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/src/kiara_plugin/html/modules/__init__.py` & `kiara_plugin.html-0.4.3/src/kiara_plugin/html/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/src/kiara_plugin/html/modules/core_types.py` & `kiara_plugin.html-0.4.3/src/kiara_plugin/html/modules/core_types.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/src/kiara_plugin/html/modules/included_types.py` & `kiara_plugin.html-0.4.3/src/kiara_plugin/html/modules/included_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from typing import Any, Mapping
 
 from airium import Airium
 
 from kiara.api import Value
-from kiara.models.filesystem import FileBundle
+from kiara.models.filesystem import KiaraFileBundle
 from kiara.models.rendering import RenderValueResult
 from kiara.modules.included_core_modules.render_value import RenderValueModule
 
 
 class RenderCoreTypeModuleWeb(RenderValueModule):
     _module_type_name = "render.included_types.for.web"
 
@@ -25,15 +25,15 @@
     def render__file_bundle__as__html(
         self, value: Value, render_config: Mapping[str, Any]
     ):
 
         import humanfriendly
 
         # render_scene = render_config.get("scene_name", "data")
-        file_bundle: FileBundle = value.data
+        file_bundle: KiaraFileBundle = value.data
 
         # to_render = file_bundle.dict()
 
         doc = Airium()
         with doc.table():
             with doc.tr():
                 with doc.th():
```

### Comparing `kiara_plugin.html-0.4.2/src/kiara_plugin/html/modules/tabular.py` & `kiara_plugin.html-0.4.3/src/kiara_plugin/html/modules/tabular.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/src/kiara_plugin/html/renderers/lineage.py` & `kiara_plugin.html-0.4.3/src/kiara_plugin/html/renderers/lineage.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/templates/lineage/assets/json-fomatter.js` & `kiara_plugin.html-0.4.3/src/kiara_plugin/html/resources/templates/lineage/assets/json-fomatter.js`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/src/kiara_plugin/html/resources/templates/lineage/assets/msgpack.js` & `kiara_plugin.html-0.4.3/src/kiara_plugin/html/resources/templates/lineage/assets/msgpack.js`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/PKG-INFO` & `kiara_plugin.html-0.4.3/src/kiara_plugin.html.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.html
-Version: 0.4.2
+Version: 0.4.3
 Summary: Kiara plugin for html-related tasks.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.html
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.html
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.html
 Keywords: kiara
```

### Comparing `kiara_plugin.html-0.4.2/src/kiara_plugin.html.egg-info/SOURCES.txt` & `kiara_plugin.html-0.4.3/src/kiara_plugin.html.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/tests/conftest.py` & `kiara_plugin.html-0.4.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.html-0.4.2/tests/test_job_descs.py` & `kiara_plugin.html-0.4.3/tests/test_job_descs.py`

 * *Files identical despite different names*

