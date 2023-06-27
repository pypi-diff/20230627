# Comparing `tmp/fideslang-1.4.2.tar.gz` & `tmp/fideslang-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fideslang-1.4.2.tar", last modified: Wed Jun 21 21:18:36 2023, max compression
+gzip compressed data, was "fideslang-1.4.3.tar", last modified: Tue Jun 27 08:35:56 2023, max compression
```

## Comparing `fideslang-1.4.2.tar` & `fideslang-1.4.3.tar`

### file list

```diff
@@ -1,35 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:18:36.364539 fideslang-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-06-21 21:18:17.000000 fideslang-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-21 21:18:17.000000 fideslang-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-21 21:18:36.364539 fideslang-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-21 21:18:17.000000 fideslang-1.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-21 21:18:17.000000 fideslang-1.4.2/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-21 21:18:17.000000 fideslang-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-21 21:18:17.000000 fideslang-1.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-21 21:18:36.364539 fideslang-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-21 21:18:17.000000 fideslang-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:18:36.360539 fideslang-1.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:18:36.364539 fideslang-1.4.2/src/fideslang/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-21 21:18:36.364539 fideslang-1.4.2/src/fideslang/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/default_fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:18:36.364539 fideslang-1.4.2/src/fideslang/default_taxonomy/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/default_taxonomy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15437 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/default_taxonomy/data_categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/default_taxonomy/data_qualifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/default_taxonomy/data_subjects.py
--rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/default_taxonomy/data_uses.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/default_taxonomy/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/manifests.py
--rw-r--r--   0 runner    (1001) docker     (123)    35159 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:18:36.364539 fideslang-1.4.2/src/fideslang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-21 21:18:36.000000 fideslang-1.4.2/src/fideslang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-21 21:18:36.000000 fideslang-1.4.2/src/fideslang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:18:36.000000 fideslang-1.4.2/src/fideslang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 21:18:36.000000 fideslang-1.4.2/src/fideslang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 21:18:36.000000 fideslang-1.4.2/src/fideslang.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.415515 fideslang-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 08:35:39.000000 fideslang-1.4.3/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-27 08:35:39.000000 fideslang-1.4.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.395515 fideslang-1.4.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-27 08:35:39.000000 fideslang-1.4.3/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-27 08:35:39.000000 fideslang-1.4.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.395515 fideslang-1.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-27 08:35:39.000000 fideslang-1.4.3/.github/workflows/docker.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-27 08:35:39.000000 fideslang-1.4.3/.github/workflows/pr_checks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-27 08:35:39.000000 fideslang-1.4.3/.github/workflows/publish_docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-27 08:35:39.000000 fideslang-1.4.3/.github/workflows/publish_package.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-27 08:35:39.000000 fideslang-1.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-27 08:35:39.000000 fideslang-1.4.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-06-27 08:35:39.000000 fideslang-1.4.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-27 08:35:39.000000 fideslang-1.4.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-27 08:35:39.000000 fideslang-1.4.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-27 08:35:39.000000 fideslang-1.4.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-06-27 08:35:39.000000 fideslang-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-27 08:35:39.000000 fideslang-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-27 08:35:39.000000 fideslang-1.4.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-06-27 08:35:56.415515 fideslang-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-27 08:35:39.000000 fideslang-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.399515 fideslang-1.4.3/data_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-06-27 08:35:39.000000 fideslang-1.4.3/data_files/data_categories.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18924 2023-06-27 08:35:39.000000 fideslang-1.4.3/data_files/data_categories.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12147 2023-06-27 08:35:39.000000 fideslang-1.4.3/data_files/data_categories.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-27 08:35:39.000000 fideslang-1.4.3/data_files/data_qualifiers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-27 08:35:39.000000 fideslang-1.4.3/data_files/data_qualifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-27 08:35:39.000000 fideslang-1.4.3/data_files/data_qualifiers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-27 08:35:39.000000 fideslang-1.4.3/data_files/data_subjects.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-06-27 08:35:39.000000 fideslang-1.4.3/data_files/data_subjects.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-27 08:35:39.000000 fideslang-1.4.3/data_files/data_subjects.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-06-27 08:35:39.000000 fideslang-1.4.3/data_files/data_uses.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26998 2023-06-27 08:35:39.000000 fideslang-1.4.3/data_files/data_uses.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18731 2023-06-27 08:35:39.000000 fideslang-1.4.3/data_files/data_uses.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.399515 fideslang-1.4.3/demo_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-27 08:35:39.000000 fideslang-1.4.3/demo_resources/demo_dataset.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-27 08:35:39.000000 fideslang-1.4.3/demo_resources/demo_extended_taxonomy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-27 08:35:39.000000 fideslang-1.4.3/demo_resources/demo_organization.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-27 08:35:39.000000 fideslang-1.4.3/demo_resources/demo_policy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-27 08:35:39.000000 fideslang-1.4.3/demo_resources/demo_registry.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-27 08:35:39.000000 fideslang-1.4.3/demo_resources/demo_system.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-27 08:35:39.000000 fideslang-1.4.3/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-27 08:35:39.000000 fideslang-1.4.3/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.399515 fideslang-1.4.3/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.399515 fideslang-1.4.3/mkdocs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/.nojekyll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.403515 fideslang-1.4.3/mkdocs/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/css/fides.css
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/css/logo.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/css/taxonomy.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.403515 fideslang-1.4.3/mkdocs/docs/csv/
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/csv/data_categories.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/csv/data_qualifiers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/csv/data_subjects.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/csv/data_uses.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/explorer.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.403515 fideslang-1.4.3/mkdocs/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/img/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/img/Radial Tree@1x.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    20880 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/img/Resource_Relations.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/img/Sunburst@1x.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/img/Tree@1x.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32916 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/img/ethyca.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    33976 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/img/fideslang.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/img/fideslang.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   483118 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/img/taxonomy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.407515 fideslang-1.4.3/mkdocs/docs/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/js/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)    25027 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/js/vis.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25039 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/js/vis2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.407515 fideslang-1.4.3/mkdocs/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/resources/dataset.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/resources/organization.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/resources/policy.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/resources/registry.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/resources/system.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/syntax.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.407515 fideslang-1.4.3/mkdocs/docs/taxonomy/
+-rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/taxonomy/data_categories.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/taxonomy/data_qualifiers.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/taxonomy/data_subjects.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12361 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/taxonomy/data_uses.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/docs/taxonomy/overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.391515 fideslang-1.4.3/mkdocs/overrides/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.407515 fideslang-1.4.3/mkdocs/overrides/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)    48368 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/overrides/partials/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-27 08:35:39.000000 fideslang-1.4.3/mkdocs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-27 08:35:39.000000 fideslang-1.4.3/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-27 08:35:39.000000 fideslang-1.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 08:35:39.000000 fideslang-1.4.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.407515 fideslang-1.4.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-27 08:35:39.000000 fideslang-1.4.3/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-27 08:35:39.000000 fideslang-1.4.3/scripts/export_default_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 08:35:56.415515 fideslang-1.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.407515 fideslang-1.4.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:39.000000 fideslang-1.4.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.411515 fideslang-1.4.3/src/fideslang/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-27 08:35:39.000000 fideslang-1.4.3/src/fideslang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-27 08:35:56.000000 fideslang-1.4.3/src/fideslang/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-06-27 08:35:39.000000 fideslang-1.4.3/src/fideslang/default_fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.411515 fideslang-1.4.3/src/fideslang/default_taxonomy/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-27 08:35:39.000000 fideslang-1.4.3/src/fideslang/default_taxonomy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15437 2023-06-27 08:35:39.000000 fideslang-1.4.3/src/fideslang/default_taxonomy/data_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-27 08:35:39.000000 fideslang-1.4.3/src/fideslang/default_taxonomy/data_qualifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-27 08:35:39.000000 fideslang-1.4.3/src/fideslang/default_taxonomy/data_subjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-06-27 08:35:39.000000 fideslang-1.4.3/src/fideslang/default_taxonomy/data_uses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-27 08:35:39.000000 fideslang-1.4.3/src/fideslang/default_taxonomy/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-27 08:35:39.000000 fideslang-1.4.3/src/fideslang/manifests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35159 2023-06-27 08:35:39.000000 fideslang-1.4.3/src/fideslang/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-27 08:35:39.000000 fideslang-1.4.3/src/fideslang/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:39.000000 fideslang-1.4.3/src/fideslang/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-06-27 08:35:39.000000 fideslang-1.4.3/src/fideslang/relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-27 08:35:39.000000 fideslang-1.4.3/src/fideslang/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-27 08:35:39.000000 fideslang-1.4.3/src/fideslang/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.411515 fideslang-1.4.3/src/fideslang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-06-27 08:35:56.000000 fideslang-1.4.3/src/fideslang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-27 08:35:56.000000 fideslang-1.4.3/src/fideslang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 08:35:56.000000 fideslang-1.4.3/src/fideslang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 08:35:56.000000 fideslang-1.4.3/src/fideslang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 08:35:56.000000 fideslang-1.4.3/src/fideslang.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.411515 fideslang-1.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-06-27 08:35:39.000000 fideslang-1.4.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.415515 fideslang-1.4.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-27 08:35:39.000000 fideslang-1.4.3/tests/data/failing_dataset_collection_taxonomy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-27 08:35:39.000000 fideslang-1.4.3/tests/data/failing_dataset_field_taxonomy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-27 08:35:39.000000 fideslang-1.4.3/tests/data/failing_dataset_taxonomy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-27 08:35:39.000000 fideslang-1.4.3/tests/data/failing_declaration_taxonomy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-27 08:35:39.000000 fideslang-1.4.3/tests/data/failing_nested_dataset.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-27 08:35:39.000000 fideslang-1.4.3/tests/data/passing_declaration_taxonomy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-06-27 08:35:39.000000 fideslang-1.4.3/tests/data/sample_hierarchy_figures.json
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-27 08:35:39.000000 fideslang-1.4.3/tests/data/sample_manifest.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:35:56.415515 fideslang-1.4.3/tests/fideslang/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-27 08:35:39.000000 fideslang-1.4.3/tests/fideslang/test_default_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-06-27 08:35:39.000000 fideslang-1.4.3/tests/fideslang/test_manifests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-06-27 08:35:39.000000 fideslang-1.4.3/tests/fideslang/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-27 08:35:39.000000 fideslang-1.4.3/tests/fideslang/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11554 2023-06-27 08:35:39.000000 fideslang-1.4.3/tests/fideslang/test_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16241 2023-06-27 08:35:39.000000 fideslang-1.4.3/tests/fideslang/test_validation.py
```

### Comparing `fideslang-1.4.2/LICENSE` & `fideslang-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.2/PKG-INFO` & `fideslang-1.4.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: fideslang
-Version: 1.4.2
+Version: 1.4.3
 Summary: Fides Taxonomy Language
-Home-page: https://github.com/ethyca/fideslang
-Author: Ethyca, Inc.
-Author-email: fidesteam@ethyca.com
+Author-email: "Ethyca, Inc." <fidesteam@ethyca.com>
 License: Apache License 2.0
+Project-URL: documentation, https://github.com/ethyca/fideslang
+Project-URL: changelog, https://github.com/ethyca/fideslang/blob/main/CHANGELOG.md
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7, <4
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: fastapi
-Provides-Extra: all
 License-File: LICENSE
 
 # Fideslang
 
 [![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/) [![Twitter](https://img.shields.io/twitter/follow/ethyca?style=social)](https://twitter.com/ethyca)
 
 ![Fideslang banner](mkdocs/docs/img/fideslang.png "Fideslang banner")
```

### Comparing `fideslang-1.4.2/README.md` & `fideslang-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.2/pyproject.toml` & `fideslang-1.4.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,80 @@
+###############
+## Packaging ##
+###############
 [build-system]
-requires = ["setuptools", "wheel", "versioneer[toml]==0.28"]  # PEP 508 specifications.
+requires = ["setuptools", "wheel", "setuptools_scm"]
 
-[tool.versioneer]
-VCS = "git"
-style = "pep440"
-versionfile_source = "src/fideslang/_version.py"
-versionfile_build = "fideslang/_version.py"
-tag_prefix = ""
-parentdir_prefix = ""
-
-######
-# MyPy
-######
-# [tool.mypy] Waiting for new version of Mypy
-# warn_unused_configs = true
-# ignore_missing_imports = true
-# pretty = true
-
-#######
-# Black
-#######
+[project]
+name="fideslang"
+description="Fides Taxonomy Language"
+dynamic = ["dependencies", "version"]
+readme = "README.md"
+requires-python=">=3.8, <4"
+authors = [
+    {name = "Ethyca, Inc.", email = "fidesteam@ethyca.com"}
+]
+license= {text = "Apache License 2.0"}
+classifiers=[
+    "License :: OSI Approved :: Apache Software License",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Software Development :: Libraries",
+]
+
+[project.urls]
+documentation = "https://github.com/ethyca/fideslang"
+changelog = "https://github.com/ethyca/fideslang/blob/main/CHANGELOG.md"
+
+[tool.setuptools_scm]
+write_to = "src/fideslang/_version.py"
+
+[tool.setuptools.dynamic]
+dependencies = {file = "requirements.txt"}
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
+############
+## Typing ##
+############
+[tool.mypy]
+check_untyped_defs = true
+disallow_untyped_defs = true
+disallow_any_explicit = true
+files = ["src"]
+no_implicit_reexport = true
+plugins = ["pydantic.mypy"]
+pretty = true
+show_error_codes = true
+warn_redundant_casts = true
+warn_unused_configs = true
+warn_unused_ignores = true
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module= "fideslang._version"
+ignore_errors=true
+
+[[tool.mypy.overrides]]
+module = ["tests.*"]
+disallow_untyped_defs = false
+
+[tool.pydantic-mypy]
+init_forbid_extra = true
+init_typed = true
+warn_required_dynamic_aliases = true
+warn_untyped_fields = true
+
+###########
+## Black ##
+###########
 [tool.black]
 py39 = true
 line-length = 88
 include = '\.pyi?$'
 exclude = '''
 /(
     \.git
@@ -38,17 +89,17 @@
 
     # The following are specific to Black, you probably don't want those.
     | blib2to3
     | tests/data
 )/
 '''
 
-########
-# Pylint
-########
+############
+## Pylint ##
+############
 [tool.pylint.messages_control]
 ignore="migrations"
 disable=[
     "line-too-long",
     "too-few-public-methods",
     "duplicate-code",
     "import-error",
@@ -68,17 +119,17 @@
 
 [tool.pylint.format]
 max-line-length="88"
 
 [tool.pylint.basic]
 good-names="_,i,setUp,tearDown,maxDiff,default_app_config"
 
-########
-# Pytest
-########
+############
+## Pytest ##
+############
 [tool.pytest.ini_options]
 testpaths="tests"
 log_level = "DEBUG"
 addopts = ["--cov=fideslang",
             "--cov-report=term-missing",
             "-vv",
             "--no-cov-on-fail",]
```

### Comparing `fideslang-1.4.2/src/fideslang/__init__.py` & `fideslang-1.4.3/src/fideslang/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 """
 
 from typing import Dict, Type, Union
 
 from fideslang.default_fixtures import COUNTRY_CODES
 from fideslang.default_taxonomy import DEFAULT_TAXONOMY
 
-from . import _version
+from ._version import __version__
 
-__version__ = _version.get_versions()["version"]
 
 # Export the Models
 from .models import (
     DataCategory,
     DataFlow,
     DataQualifier,
     Dataset,
```

### Comparing `fideslang-1.4.2/src/fideslang/default_fixtures.py` & `fideslang-1.4.3/src/fideslang/default_fixtures.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.2/src/fideslang/default_taxonomy/__init__.py` & `fideslang-1.4.3/src/fideslang/default_taxonomy/__init__.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.2/src/fideslang/default_taxonomy/data_categories.py` & `fideslang-1.4.3/src/fideslang/default_taxonomy/data_categories.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.2/src/fideslang/default_taxonomy/data_qualifiers.py` & `fideslang-1.4.3/src/fideslang/default_taxonomy/data_qualifiers.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.2/src/fideslang/default_taxonomy/data_subjects.py` & `fideslang-1.4.3/src/fideslang/default_taxonomy/data_subjects.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.2/src/fideslang/default_taxonomy/data_uses.py` & `fideslang-1.4.3/src/fideslang/default_taxonomy/data_uses.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.2/src/fideslang/manifests.py` & `fideslang-1.4.3/src/fideslang/manifests.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.2/src/fideslang/models.py` & `fideslang-1.4.3/src/fideslang/models.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.2/src/fideslang/parse.py` & `fideslang-1.4.3/src/fideslang/parse.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.2/src/fideslang/relationships.py` & `fideslang-1.4.3/src/fideslang/relationships.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.2/src/fideslang/utils.py` & `fideslang-1.4.3/src/fideslang/utils.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.2/src/fideslang/validation.py` & `fideslang-1.4.3/src/fideslang/validation.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.2/src/fideslang.egg-info/PKG-INFO` & `fideslang-1.4.3/src/fideslang.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: fideslang
-Version: 1.4.2
+Version: 1.4.3
 Summary: Fides Taxonomy Language
-Home-page: https://github.com/ethyca/fideslang
-Author: Ethyca, Inc.
-Author-email: fidesteam@ethyca.com
+Author-email: "Ethyca, Inc." <fidesteam@ethyca.com>
 License: Apache License 2.0
+Project-URL: documentation, https://github.com/ethyca/fideslang
+Project-URL: changelog, https://github.com/ethyca/fideslang/blob/main/CHANGELOG.md
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7, <4
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: fastapi
-Provides-Extra: all
 License-File: LICENSE
 
 # Fideslang
 
 [![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/) [![Twitter](https://img.shields.io/twitter/follow/ethyca?style=social)](https://twitter.com/ethyca)
 
 ![Fideslang banner](mkdocs/docs/img/fideslang.png "Fideslang banner")
```

