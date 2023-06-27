# Comparing `tmp/kiara_plugin.streamlit-0.4.2.tar.gz` & `tmp/kiara_plugin.streamlit-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.streamlit-0.4.2.tar", last modified: Fri Jun 23 10:09:52 2023, max compression
+gzip compressed data, was "kiara_plugin.streamlit-0.4.3.tar", last modified: Tue Jun 27 10:45:43 2023, max compression
```

## Comparing `kiara_plugin.streamlit-0.4.2.tar` & `kiara_plugin.streamlit-0.4.3.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.720479 kiara_plugin.streamlit-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.728479 kiara_plugin.streamlit-0.4.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/apps/components.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/apps/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/apps/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/apps/pipelines/components_doc_onboarding.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/apps/pipelines/operations_doc_onboarding.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.720479 kiara_plugin.streamlit-0.4.2/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/ci/conda/conda-pkg-patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.724479 kiara_plugin.streamlit-0.4.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33398 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/jobs/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.732479 kiara_plugin.streamlit-0.4.2/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/pipelines/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.736479 kiara_plugin.streamlit-0.4.2/examples/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.736479 kiara_plugin.streamlit-0.4.2/examples/streamlit/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/pipelines/example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/pipelines/topic_modeling.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/step_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/workflow_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/workflow_static.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/examples/streamlit/workshop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.724479 kiara_plugin.streamlit-0.4.2/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.736479 kiara_plugin.streamlit-0.4.2/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-23 10:09:52.748479 kiara_plugin.streamlit-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.724479 kiara_plugin.streamlit-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.724479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.736479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.736479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.736479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/context/
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/context/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.740479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/info/
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/info/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/info/components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.740479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/input/
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/input/assemblies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/input/container_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/input/scalars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.740479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/operations/
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/operations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.740479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.740479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/assemblies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/core_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/network_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.740479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.740479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/dynamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/dynamic/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/dynamic/workflow_page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.740479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/requirements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/static/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/static/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/static/workflow_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/interfaces/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/interfaces/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/interfaces/cli/streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/renderers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.724479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/resources/templates/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/resources/templates/pipeline/streamlit_app.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/utils/class_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/utils/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/utils/monkey_patches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.736479 kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-23 10:09:52.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-23 10:09:52.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:09:52.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-23 10:09:52.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:08:42.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-23 10:09:52.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 10:09:52.000000 kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:09:52.744479 kiara_plugin.streamlit-0.4.2/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      233 2023-06-23 10:08:25.000000 kiara_plugin.streamlit-0.4.2/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.156000 kiara_plugin.streamlit-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.127999 kiara_plugin.streamlit-0.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-27 10:45:43.156000 kiara_plugin.streamlit-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/apps/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/apps/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/apps/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/apps/pipelines/components_doc_onboarding.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/apps/pipelines/operations_doc_onboarding.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.127999 kiara_plugin.streamlit-0.4.3/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/ci/conda/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.131999 kiara_plugin.streamlit-0.4.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33398 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/jobs/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.139999 kiara_plugin.streamlit-0.4.3/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/pipelines/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.143999 kiara_plugin.streamlit-0.4.3/examples/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.143999 kiara_plugin.streamlit-0.4.3/examples/streamlit/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/pipelines/example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/pipelines/topic_modeling.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/step_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/workflow_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/workflow_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/examples/streamlit/workshop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.131999 kiara_plugin.streamlit-0.4.3/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.143999 kiara_plugin.streamlit-0.4.3/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-27 10:45:43.156000 kiara_plugin.streamlit-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.131999 kiara_plugin.streamlit-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.131999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.143999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/context/
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/context/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/info/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/info/components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/input/assemblies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/input/container_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/input/scalars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/operations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/assemblies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/core_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/network_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/dynamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/dynamic/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/dynamic/workflow_page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.147999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/requirements/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/static/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/static/workflow_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/interfaces/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/interfaces/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/interfaces/cli/streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/renderers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.131999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/resources/templates/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/resources/templates/pipeline/streamlit_app.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/utils/class_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/utils/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/utils/monkey_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.143999 kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-27 10:45:43.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-27 10:45:43.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:45:43.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-27 10:45:43.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:44:30.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-27 10:45:43.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 10:45:43.000000 kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.151999 kiara_plugin.streamlit-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:45:43.156000 kiara_plugin.streamlit-0.4.3/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/tests/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      233 2023-06-27 10:44:19.000000 kiara_plugin.streamlit-0.4.3/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.streamlit-0.4.2/.cruft.json` & `kiara_plugin.streamlit-0.4.3/.cruft.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.streamlit-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.streamlit-0.4.3/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/.github/workflows/build-darwin.yaml` & `kiara_plugin.streamlit-0.4.3/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/.github/workflows/build-linux.yaml` & `kiara_plugin.streamlit-0.4.3/.github/workflows/build-linux.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/.github/workflows/build-windows.yaml` & `kiara_plugin.streamlit-0.4.3/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/.gitignore` & `kiara_plugin.streamlit-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/.pre-commit-config.yaml` & `kiara_plugin.streamlit-0.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/LICENSE` & `kiara_plugin.streamlit-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/Makefile` & `kiara_plugin.streamlit-0.4.3/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/PKG-INFO` & `kiara_plugin.streamlit-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.streamlit
-Version: 0.4.2
+Version: 0.4.3
 Summary: Streamlit UI and widgets for kiara
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.streamlit
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.streamlit
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.streamlit
 Keywords: kiara,streamlit
```

### Comparing `kiara_plugin.streamlit-0.4.2/README.md` & `kiara_plugin.streamlit-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/apps/components.py` & `kiara_plugin.streamlit-0.4.3/apps/components.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/apps/operations.py` & `kiara_plugin.streamlit-0.4.3/apps/operations.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/apps/pipelines/components_doc_onboarding.yaml` & `kiara_plugin.streamlit-0.4.3/apps/pipelines/components_doc_onboarding.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/apps/pipelines/operations_doc_onboarding.yaml` & `kiara_plugin.streamlit-0.4.3/apps/pipelines/operations_doc_onboarding.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/docs/development.md` & `kiara_plugin.streamlit-0.4.3/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/docs/index.md` & `kiara_plugin.streamlit-0.4.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.streamlit-0.4.3/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.streamlit-0.4.3/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/examples/streamlit/pipeline.py` & `kiara_plugin.streamlit-0.4.3/examples/streamlit/pipeline.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/examples/streamlit/pipelines/example.yaml` & `kiara_plugin.streamlit-0.4.3/examples/streamlit/pipelines/example.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/examples/streamlit/pipelines/topic_modeling.yaml` & `kiara_plugin.streamlit-0.4.3/examples/streamlit/pipelines/topic_modeling.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/examples/streamlit/step_inputs.py` & `kiara_plugin.streamlit-0.4.3/examples/streamlit/step_inputs.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/examples/streamlit/workflow_dynamic.py` & `kiara_plugin.streamlit-0.4.3/examples/streamlit/workflow_dynamic.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/examples/streamlit/workflow_static.py` & `kiara_plugin.streamlit-0.4.3/examples/streamlit/workflow_static.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/examples/streamlit/workflows.py` & `kiara_plugin.streamlit-0.4.3/examples/streamlit/workflows.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/examples/streamlit/workshop.py` & `kiara_plugin.streamlit-0.4.3/examples/streamlit/workshop.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/mkdocs.yml` & `kiara_plugin.streamlit-0.4.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/pyproject.toml` & `kiara_plugin.streamlit-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,36 +26,35 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 dependencies = [
-    "kiara_plugin.tabular>=0.4.27",
-    "kiara_plugin.onboarding>=0.4.3",
+    "kiara_plugin.tabular>=0.4.28",
+    "kiara_plugin.onboarding>=0.4.5",
     "streamlit>=1.23.1.0",
     "streamlit-aggrid>=0.3.4",
     "importlib-resources",
     "pydot>=1.4.0",
     "pyvis>=0.3.0",
     "streamlit-tags>=1.2.8"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 workflow_app = [
-    "boltons>=23.0.0,<24.0.0",
-    "PyGithub>=1.59.0",
+    "PyGithub>=1.58.0",
     "githublfs>=0.1.3"
 ]
 all_plugins = [
     "kiara_plugin.network_analysis>=0.4.9",
     "kiara_plugin.language_processing>=0.4.10",
-    "kiara_plugin.html>=0.4.0",
-    "kiara_plugin.onboarding>=0.4.2"
+    "kiara_plugin.html>=0.4.3",
+    "kiara_plugin.onboarding>=0.4.5"
 ]
 dev_documentation = [
     "kiara[dev_documentation]"
 ]
 dev_testing = [
     "kiara[dev_testing]",
     "kiara_plugin.network_analysis>=0.4.7",
```

### Comparing `kiara_plugin.streamlit-0.4.2/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.streamlit-0.4.3/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/scripts/documentation/gen_info_pages.py` & `kiara_plugin.streamlit-0.4.3/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/scripts/documentation/gen_module_doc.py` & `kiara_plugin.streamlit-0.4.3/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/setup.cfg` & `kiara_plugin.streamlit-0.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/__init__.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/__init__.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/context/__init__.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/context/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/info/__init__.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/info/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/info/api.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/info/api.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/info/components.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/info/components.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/input/__init__.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/input/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/input/assemblies.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/input/assemblies.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/input/container_types.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/input/container_types.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/input/scalars.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/input/scalars.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/operations/__init__.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/pipelines/__init__.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/__init__.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/assemblies.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/assemblies.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/core_types.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/core_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from typing import Any, Dict
 
 from kiara.models.data_types import KiaraDict
-from kiara.models.filesystem import FileBundle, FileModel
+from kiara.models.filesystem import KiaraFile, KiaraFileBundle
 from kiara.utils.json import orjson_dumps
 from kiara_plugin.core_types.models import KiaraList
 from kiara_plugin.streamlit.components.preview import PreviewComponent, PreviewOptions
 from streamlit.delta_generator import DeltaGenerator
 
 
 class DictPreview(PreviewComponent):
@@ -75,15 +75,15 @@
     @classmethod
     def get_data_type(cls) -> str:
         return "file_bundle"
 
     def render_preview(self, st: DeltaGenerator, options: PreviewOptions) -> None:
 
         _value = self.api.get_value(options.value)
-        bundle: FileBundle = _value.data
+        bundle: KiaraFileBundle = _value.data
 
         table: Dict[str, Any] = {}
         for file_path, file_info in bundle.included_files.items():
             table.setdefault("path", []).append(file_path)
             table.setdefault("size", []).append(file_info.size)
             table.setdefault("mime-type", []).append(file_info.mime_type)
 
@@ -98,15 +98,15 @@
     @classmethod
     def get_data_type(cls) -> str:
         return "file"
 
     def render_preview(self, st: DeltaGenerator, options: PreviewOptions) -> None:
 
         _value = self.api.get_value(options.value)
-        file_model: FileModel = _value.data
+        file_model: KiaraFile = _value.data
 
         table: Dict[str, Any] = {"key": [], "value": []}
         table["key"].append("path")
         table["value"].append(file_model.path)
         table["key"].append("size")
         table["value"].append(file_model.size)
         table["key"].append("mime-type")
```

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/network_data.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/network_data.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/preview/tabular.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/preview/tabular.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/__init__.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/dynamic/__init__.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/dynamic/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/dynamic/components.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/dynamic/components.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/dynamic/workflow_page.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/dynamic/workflow_page.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/requirements/__init__.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/requirements/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/static/components.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/static/components.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/components/workflow/static/workflow_page.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/components/workflow/static/workflow_page.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/interfaces/cli/streamlit.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/interfaces/cli/streamlit.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/models.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/modules/__init__.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/renderers/__init__.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/resources/templates/pipeline/streamlit_app.py.j2` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/resources/templates/pipeline/streamlit_app.py.j2`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/streamlit.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/utils/class_loading.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/utils/class_loading.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/utils/components.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/utils/components.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin/streamlit/utils/monkey_patches.py` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin/streamlit/utils/monkey_patches.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/PKG-INFO` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.streamlit
-Version: 0.4.2
+Version: 0.4.3
 Summary: Streamlit UI and widgets for kiara
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.streamlit
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.streamlit
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.streamlit
 Keywords: kiara,streamlit
```

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/SOURCES.txt` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/entry_points.txt` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/src/kiara_plugin.streamlit.egg-info/requires.txt` & `kiara_plugin.streamlit-0.4.3/src/kiara_plugin.streamlit.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-kiara_plugin.tabular>=0.4.27
-kiara_plugin.onboarding>=0.4.3
+kiara_plugin.tabular>=0.4.28
+kiara_plugin.onboarding>=0.4.5
 streamlit>=1.23.1.0
 streamlit-aggrid>=0.3.4
 importlib-resources
 pydot>=1.4.0
 pyvis>=0.3.0
 streamlit-tags>=1.2.8
 
 [all_plugins]
 kiara_plugin.network_analysis>=0.4.9
 kiara_plugin.language_processing>=0.4.10
-kiara_plugin.html>=0.4.0
-kiara_plugin.onboarding>=0.4.2
+kiara_plugin.html>=0.4.3
+kiara_plugin.onboarding>=0.4.5
 
 [dev_all]
 kiara[dev_all]
 
 [dev_documentation]
 kiara[dev_documentation]
 
@@ -23,10 +23,9 @@
 kiara[dev_testing]
 kiara_plugin.network_analysis>=0.4.7
 
 [dev_utils]
 kiara[dev_utils]
 
 [workflow_app]
-boltons<24.0.0,>=23.0.0
-PyGithub>=1.59.0
+PyGithub>=1.58.0
 githublfs>=0.1.3
```

### Comparing `kiara_plugin.streamlit-0.4.2/tests/conftest.py` & `kiara_plugin.streamlit-0.4.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.2/tests/test_job_descs.py` & `kiara_plugin.streamlit-0.4.3/tests/test_job_descs.py`

 * *Files identical despite different names*

