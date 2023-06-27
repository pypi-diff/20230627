# Comparing `tmp/pydantic-i18n-0.3.1.tar.gz` & `tmp/pydantic_i18n-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-i18n-0.3.1.tar", last modified: Sat Mar  4 21:34:30 2023, max compression
+gzip compressed data, was "pydantic_i18n-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pydantic-i18n-0.3.1.tar` & `pydantic_i18n-0.4.0.tar`

### file list

```diff
@@ -1,87 +1,86 @@
--rw-r--r--   0        0        0      459 2023-03-04 21:34:07.748533 pydantic-i18n-0.3.1/.coveragerc
--rw-r--r--   0        0        0      291 2023-03-04 21:34:07.748533 pydantic-i18n-0.3.1/.editorconfig
--rw-r--r--   0        0        0      577 2023-03-04 21:34:07.748533 pydantic-i18n-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       27 2023-03-04 21:34:07.748533 pydantic-i18n-0.3.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      445 2023-03-04 21:34:07.748533 pydantic-i18n-0.3.1/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0        0        0      115 2023-03-04 21:34:07.748533 pydantic-i18n-0.3.1/.github/actions/comment-docs-preview-in-pr/Dockerfile
--rw-r--r--   0        0        0      386 2023-03-04 21:34:07.748533 pydantic-i18n-0.3.1/.github/actions/comment-docs-preview-in-pr/README.md
--rw-r--r--   0        0        0      396 2023-03-04 21:34:07.748533 pydantic-i18n-0.3.1/.github/actions/comment-docs-preview-in-pr/action.yml
--rw-r--r--   0        0        0     2096 2023-03-04 21:34:07.748533 pydantic-i18n-0.3.1/.github/actions/comment-docs-preview-in-pr/app/main.py
--rw-r--r--   0        0        0      387 2023-03-04 21:34:07.748533 pydantic-i18n-0.3.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1542 2023-03-04 21:34:07.748533 pydantic-i18n-0.3.1/.github/workflows/build-docs.yml
--rw-r--r--   0        0        0      561 2023-03-04 21:34:07.748533 pydantic-i18n-0.3.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0      530 2023-03-04 21:34:07.748533 pydantic-i18n-0.3.1/.github/workflows/new_contributor_pr.yml
--rw-r--r--   0        0        0     1197 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/.github/workflows/preview-docs.yml
--rw-r--r--   0        0        0      829 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      793 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1833 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/.gitignore
--rw-r--r--   0        0        0     1077 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/LICENSE
--rw-r--r--   0        0        0    14430 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs/en/data/.gitignore
--rw-r--r--   0        0        0    14738 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs/en/docs/contributing.md
--rw-r--r--   0        0        0      302 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs/en/docs/css/custom.css
--rw-r--r--   0        0        0     2165 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs/en/docs/css/termynal.css
--rw-r--r--   0        0        0     2757 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs/en/docs/help-pydantic-i18n.md
--rw-r--r--   0        0        0      399 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs/en/docs/img/favicon.png
--rw-r--r--   0        0        0     2918 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs/en/docs/img/icon-white.png
--rw-r--r--   0        0        0    18203 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs/en/docs/img/logo-white.png
--rw-r--r--   0        0        0    13894 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs/en/docs/img/logo-white.svg
--rw-r--r--   0        0        0     9726 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs/en/docs/index.md
--rw-r--r--   0        0        0     4357 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs/en/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs/en/docs/js/termynal.js
--rw-r--r--   0        0        0     7370 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs/en/docs/release-notes.md
--rw-r--r--   0        0        0     1760 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs/en/mkdocs.yml
--rw-r--r--   0        0        0      295 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs/en/overrides/main.html
--rw-r--r--   0        0        0      220 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs/missing-translation.md
--rw-r--r--   0        0        0      498 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs_src/babel-loader/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0      714 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs_src/babel-loader/translations/de_DE/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      495 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs_src/babel-loader/translations/en_US/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0      718 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs_src/babel-loader/translations/en_US/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      470 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs_src/babel-loader/tutorial001.py
--rw-r--r--   0        0        0      583 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs_src/dict-loader/tutorial001.py
--rw-r--r--   0        0        0      418 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs_src/fastapi-usage/main.py
--rw-r--r--   0        0        0      909 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs_src/fastapi-usage/tr.py
--rw-r--r--   0        0        0       46 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs_src/json-loader/translations/de_DE.json
--rw-r--r--   0        0        0       43 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs_src/json-loader/translations/en_US.json
--rw-r--r--   0        0        0      471 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs_src/json-loader/tutorial001.py
--rw-r--r--   0        0        0       33 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs_src/own-loader/translations/de_DE.csv
--rw-r--r--   0        0        0       30 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs_src/own-loader/translations/en_US.csv
--rw-r--r--   0        0        0     1118 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs_src/own-loader/tutorial001.py
--rw-r--r--   0        0        0     1302 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs_src/placeholder/tutorial001.py
--rw-r--r--   0        0        0      470 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs_src/pydantic-messages/tutorial001.py
--rw-r--r--   0        0        0      570 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/docs_src/pydantic-messages/tutorial002.py
--rw-r--r--   0        0        0      402 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/mypy.ini
--rw-r--r--   0        0        0      396 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/pydantic_i18n/__init__.py
--rw-r--r--   0        0        0     2696 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/pydantic_i18n/loaders.py
--rw-r--r--   0        0        0     3026 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/pydantic_i18n/main.py
--rw-r--r--   0        0        0        0 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/pydantic_i18n/py.typed
--rw-r--r--   0        0        0     1913 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       71 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/scripts/build-docs.sh
--rw-r--r--   0        0        0       98 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/scripts/clean.sh
--rw-r--r--   0        0        0       66 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/scripts/docs-live.sh
--rw-r--r--   0        0        0    13705 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/scripts/docs.py
--rw-r--r--   0        0        0      174 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/scripts/format-imports.sh
--rw-r--r--   0        0        0      226 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/scripts/format.sh
--rw-r--r--   0        0        0      163 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/scripts/lint.sh
--rw-r--r--   0        0        0       42 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/scripts/publish.sh
--rw-r--r--   0        0        0       80 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/scripts/test-cov-html.sh
--rw-r--r--   0        0        0      152 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/scripts/test.sh
--rw-r--r--   0        0        0      108 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/scripts/zip-docs.sh
--rw-r--r--   0        0        0      362 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/setup.cfg
--rw-r--r--   0        0        0        0 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0      321 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/tests/test_loaders/__init__.py
--rw-r--r--   0        0        0     1157 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/tests/test_loaders/conftest.py
--rw-r--r--   0        0        0      198 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/tests/test_loaders/test_babel_loader.py
--rw-r--r--   0        0        0     1845 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/tests/test_loaders/test_common.py
--rw-r--r--   0        0        0      449 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/tests/test_loaders/test_json_loader.py
--rw-r--r--   0        0        0     4152 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/tests/test_main.py
--rw-r--r--   0        0        0     1519 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/tests/test_pydantic_messages.py
--rw-r--r--   0        0        0      498 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/tests/translations/babel/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0      714 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/tests/translations/babel/de_DE/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      621 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/tests/translations/babel/en_US/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0      846 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/tests/translations/babel/en_US/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      624 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/tests/translations/babel/es_AR/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0      849 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/tests/translations/babel/es_AR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      280 2023-03-04 21:34:07.752533 pydantic-i18n-0.3.1/tox.ini
--rw-r--r--   0        0        0    16757 1970-01-01 00:00:00.000000 pydantic-i18n-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      459 2023-06-27 21:14:18.656572 pydantic_i18n-0.4.0/.coveragerc
+-rw-r--r--   0        0        0      291 2023-06-27 21:14:18.656572 pydantic_i18n-0.4.0/.editorconfig
+-rw-r--r--   0        0        0      577 2023-06-27 21:14:18.656572 pydantic_i18n-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       27 2023-06-27 21:14:18.656572 pydantic_i18n-0.4.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      445 2023-06-27 21:14:18.656572 pydantic_i18n-0.4.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0        0        0      115 2023-06-27 21:14:18.656572 pydantic_i18n-0.4.0/.github/actions/comment-docs-preview-in-pr/Dockerfile
+-rw-r--r--   0        0        0      386 2023-06-27 21:14:18.656572 pydantic_i18n-0.4.0/.github/actions/comment-docs-preview-in-pr/README.md
+-rw-r--r--   0        0        0      396 2023-06-27 21:14:18.656572 pydantic_i18n-0.4.0/.github/actions/comment-docs-preview-in-pr/action.yml
+-rw-r--r--   0        0        0     2096 2023-06-27 21:14:18.656572 pydantic_i18n-0.4.0/.github/actions/comment-docs-preview-in-pr/app/main.py
+-rw-r--r--   0        0        0      387 2023-06-27 21:14:18.656572 pydantic_i18n-0.4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1542 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/.github/workflows/build-docs.yml
+-rw-r--r--   0        0        0      561 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0      530 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/.github/workflows/new_contributor_pr.yml
+-rw-r--r--   0        0        0     1197 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/.github/workflows/preview-docs.yml
+-rw-r--r--   0        0        0      829 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1099 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1833 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1077 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/LICENSE
+-rw-r--r--   0        0        0    14430 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs/en/data/.gitignore
+-rw-r--r--   0        0        0    14738 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs/en/docs/contributing.md
+-rw-r--r--   0        0        0      302 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs/en/docs/css/custom.css
+-rw-r--r--   0        0        0     2165 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs/en/docs/css/termynal.css
+-rw-r--r--   0        0        0     2757 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs/en/docs/help-pydantic-i18n.md
+-rw-r--r--   0        0        0      399 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs/en/docs/img/favicon.png
+-rw-r--r--   0        0        0     2918 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs/en/docs/img/icon-white.png
+-rw-r--r--   0        0        0    18203 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs/en/docs/img/logo-white.png
+-rw-r--r--   0        0        0    13894 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs/en/docs/img/logo-white.svg
+-rw-r--r--   0        0        0     9726 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs/en/docs/index.md
+-rw-r--r--   0        0        0     4357 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs/en/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs/en/docs/js/termynal.js
+-rw-r--r--   0        0        0     9478 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs/en/docs/release-notes.md
+-rw-r--r--   0        0        0     1760 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs/en/mkdocs.yml
+-rw-r--r--   0        0        0      295 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs/en/overrides/main.html
+-rw-r--r--   0        0        0      220 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs/missing-translation.md
+-rw-r--r--   0        0        0      498 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs_src/babel-loader/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0      714 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs_src/babel-loader/translations/de_DE/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      495 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs_src/babel-loader/translations/en_US/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0      718 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs_src/babel-loader/translations/en_US/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      470 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs_src/babel-loader/tutorial001.py
+-rw-r--r--   0        0        0      583 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs_src/dict-loader/tutorial001.py
+-rw-r--r--   0        0        0      418 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs_src/fastapi-usage/main.py
+-rw-r--r--   0        0        0      909 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs_src/fastapi-usage/tr.py
+-rw-r--r--   0        0        0       46 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs_src/json-loader/translations/de_DE.json
+-rw-r--r--   0        0        0       43 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs_src/json-loader/translations/en_US.json
+-rw-r--r--   0        0        0      471 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs_src/json-loader/tutorial001.py
+-rw-r--r--   0        0        0       33 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs_src/own-loader/translations/de_DE.csv
+-rw-r--r--   0        0        0       30 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs_src/own-loader/translations/en_US.csv
+-rw-r--r--   0        0        0     1118 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs_src/own-loader/tutorial001.py
+-rw-r--r--   0        0        0     1302 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs_src/placeholder/tutorial001.py
+-rw-r--r--   0        0        0      470 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs_src/pydantic-messages/tutorial001.py
+-rw-r--r--   0        0        0      570 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/docs_src/pydantic-messages/tutorial002.py
+-rw-r--r--   0        0        0      402 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/mypy.ini
+-rw-r--r--   0        0        0      396 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/pydantic_i18n/__init__.py
+-rw-r--r--   0        0        0     2696 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/pydantic_i18n/loaders.py
+-rw-r--r--   0        0        0     3280 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/pydantic_i18n/main.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/pydantic_i18n/py.typed
+-rw-r--r--   0        0        0     1893 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/scripts/build-docs.sh
+-rw-r--r--   0        0        0       98 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/scripts/clean.sh
+-rw-r--r--   0        0        0       66 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/scripts/docs-live.sh
+-rw-r--r--   0        0        0    13705 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/scripts/docs.py
+-rw-r--r--   0        0        0      174 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/scripts/format-imports.sh
+-rw-r--r--   0        0        0      226 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/scripts/format.sh
+-rw-r--r--   0        0        0      163 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/scripts/lint.sh
+-rw-r--r--   0        0        0       42 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/scripts/publish.sh
+-rw-r--r--   0        0        0       80 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/scripts/test-cov-html.sh
+-rw-r--r--   0        0        0      152 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/scripts/test.sh
+-rw-r--r--   0        0        0      108 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/scripts/zip-docs.sh
+-rw-r--r--   0        0        0      362 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/setup.cfg
+-rw-r--r--   0        0        0        0 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      321 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/tests/test_loaders/__init__.py
+-rw-r--r--   0        0        0     1157 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/tests/test_loaders/conftest.py
+-rw-r--r--   0        0        0      198 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/tests/test_loaders/test_babel_loader.py
+-rw-r--r--   0        0        0     1845 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/tests/test_loaders/test_common.py
+-rw-r--r--   0        0        0      449 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/tests/test_loaders/test_json_loader.py
+-rw-r--r--   0        0        0     4905 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/tests/test_main.py
+-rw-r--r--   0        0        0     1519 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/tests/test_pydantic_messages.py
+-rw-r--r--   0        0        0      498 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/tests/translations/babel/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0      714 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/tests/translations/babel/de_DE/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      621 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/tests/translations/babel/en_US/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0      846 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/tests/translations/babel/en_US/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      624 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/tests/translations/babel/es_AR/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0      849 2023-06-27 21:14:18.660573 pydantic_i18n-0.4.0/tests/translations/babel/es_AR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    16712 1970-01-01 00:00:00.000000 pydantic_i18n-0.4.0/PKG-INFO
```

### Comparing `pydantic-i18n-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md` & `pydantic_i18n-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/.github/actions/comment-docs-preview-in-pr/app/main.py` & `pydantic_i18n-0.4.0/.github/actions/comment-docs-preview-in-pr/app/main.py`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/.github/workflows/build-docs.yml` & `pydantic_i18n-0.4.0/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/.github/workflows/latest-changes.yml` & `pydantic_i18n-0.4.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/.github/workflows/new_contributor_pr.yml` & `pydantic_i18n-0.4.0/.github/workflows/new_contributor_pr.yml`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/.github/workflows/preview-docs.yml` & `pydantic_i18n-0.4.0/.github/workflows/preview-docs.yml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
 
       - name: Download Artifact Docs
-        uses: dawidd6/action-download-artifact@v2.26.0
+        uses: dawidd6/action-download-artifact@v2.27.0
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           workflow: build-docs.yml
           run_id: ${{ github.event.workflow_run.id }}
           name: docs-zip
 
       - name: Unzip docs
```

### Comparing `pydantic-i18n-0.3.1/.github/workflows/publish.yml` & `pydantic_i18n-0.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/.gitignore` & `pydantic_i18n-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/LICENSE` & `pydantic_i18n-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/README.md` & `pydantic_i18n-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/docs/en/docs/contributing.md` & `pydantic_i18n-0.4.0/docs/en/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/docs/en/docs/css/termynal.css` & `pydantic_i18n-0.4.0/docs/en/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/docs/en/docs/help-pydantic-i18n.md` & `pydantic_i18n-0.4.0/docs/en/docs/help-pydantic-i18n.md`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/docs/en/docs/img/icon-white.png` & `pydantic_i18n-0.4.0/docs/en/docs/img/icon-white.png`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/docs/en/docs/img/logo-white.png` & `pydantic_i18n-0.4.0/docs/en/docs/img/logo-white.png`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/docs/en/docs/img/logo-white.svg` & `pydantic_i18n-0.4.0/docs/en/docs/img/logo-white.svg`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/docs/en/docs/index.md` & `pydantic_i18n-0.4.0/docs/en/docs/index.md`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/docs/en/docs/js/custom.js` & `pydantic_i18n-0.4.0/docs/en/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/docs/en/docs/js/termynal.js` & `pydantic_i18n-0.4.0/docs/en/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/docs/en/docs/release-notes.md` & `pydantic_i18n-0.4.0/docs/en/docs/release-notes.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,36 @@
 # Release Notes
 
 ## Latest Changes
 
 
+## 0.4.0
+
+### Features
+
+* 🐛 Add multiple placeholders support. PR [#127](https://github.com/boardpack/pydantic-i18n/pull/127) by [@dukkee](https://github.com/dukkee).
+
+### Fixes
+
+* 👷 Add cache step to the test workflow. PR [#95](https://github.com/boardpack/pydantic-i18n/pull/95) by [@dukkee](https://github.com/dukkee).
+* 🐛 Add lint step to the test workflow. PR [#93](https://github.com/boardpack/pydantic-i18n/pull/93) by [@dukkee](https://github.com/dukkee).
+
+### Internal
+
+* ⬆ Bump pytest from 7.3.1 to 7.4.0. PR [#133](https://github.com/boardpack/pydantic-i18n/pull/133) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump autoflake from 2.1.1 to 2.2.0. PR [#134](https://github.com/boardpack/pydantic-i18n/pull/134) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump mypy from 1.3.0 to 1.4.1. PR [#135](https://github.com/boardpack/pydantic-i18n/pull/135) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump pytest-cov from 4.0.0 to 4.1.0. PR [#128](https://github.com/boardpack/pydantic-i18n/pull/128) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump codecov/codecov-action from 3.1.3 to 3.1.4. PR [#122](https://github.com/boardpack/pydantic-i18n/pull/122) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump mkdocs from 1.4.2 to 1.4.3. PR [#117](https://github.com/boardpack/pydantic-i18n/pull/117) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump typer from 0.7.0 to 0.9.0. PR [#118](https://github.com/boardpack/pydantic-i18n/pull/118) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump dawidd6/action-download-artifact from 2.26.1 to 2.27.0. PR [#109](https://github.com/boardpack/pydantic-i18n/pull/109) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump black from 23.1.0 to 23.3.0. PR [#102](https://github.com/boardpack/pydantic-i18n/pull/102) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* 🔥 Remove tox. PR [#96](https://github.com/boardpack/pydantic-i18n/pull/96) by [@dukkee](https://github.com/dukkee).
+
 ## 0.3.1
 
 ### Fixes
 
 * 🎨 Improve translate method output type. PR [#88](https://github.com/boardpack/pydantic-i18n/pull/88) by [@dukkee](https://github.com/dukkee).
 
 ### Internal
```

### Comparing `pydantic-i18n-0.3.1/docs/en/mkdocs.yml` & `pydantic_i18n-0.4.0/docs/en/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/docs_src/babel-loader/translations/de_DE/LC_MESSAGES/messages.po` & `pydantic_i18n-0.4.0/docs_src/babel-loader/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/docs_src/babel-loader/translations/en_US/LC_MESSAGES/messages.po` & `pydantic_i18n-0.4.0/docs_src/babel-loader/translations/en_US/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/docs_src/dict-loader/tutorial001.py` & `pydantic_i18n-0.4.0/docs_src/dict-loader/tutorial001.py`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/docs_src/fastapi-usage/tr.py` & `pydantic_i18n-0.4.0/docs_src/fastapi-usage/tr.py`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/docs_src/own-loader/tutorial001.py` & `pydantic_i18n-0.4.0/docs_src/own-loader/tutorial001.py`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/docs_src/placeholder/tutorial001.py` & `pydantic_i18n-0.4.0/docs_src/placeholder/tutorial001.py`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/docs_src/pydantic-messages/tutorial002.py` & `pydantic_i18n-0.4.0/docs_src/pydantic-messages/tutorial002.py`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/pydantic_i18n/loaders.py` & `pydantic_i18n-0.4.0/pydantic_i18n/loaders.py`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/pyproject.toml` & `pydantic_i18n-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -39,35 +39,34 @@
 
 [project.urls]
 Documentation = "https://pydantic-i18n.boardpack.org"
 Source = "https://github.com/boardpack/pydantic-i18n"
 
 [project.optional-dependencies]
 test = [
-    "pytest ==7.2.2",
-    "pytest-cov ==4.0.0",
+    "pytest ==7.4.0",
+    "pytest-cov ==4.1.0",
     "pytest-lazy-fixture ==0.6.3",
-    "mypy ==1.0.1",
+    "mypy ==1.4.1",
     "flake8 ==6.0.0",
-    "black ==23.1.0",
+    "black ==23.3.0",
     "isort ==5.12.0",
     "babel ==2.12.1",
 ]
 dev = [
-    "autoflake ==2.0.1",
+    "autoflake ==2.2.0",
     "flake8 ==6.0.0",
     "pre-commit",
-    "tox >=3.27.1",
 ]
 doc = [
-    "mkdocs ==1.4.2",
+    "mkdocs ==1.4.3",
     "mkdocs-material ==8.5.11",
     "markdown ==3.2.1",
     "markdown-include ==0.8.1",
     "mkdocs-markdownextradata-plugin ==0.2.5",
-    "typer ==0.7.0",
+    "typer ==0.9.0",
     "pyyaml ==6.0.0",
 ]
 
 [tool.isort]
 profile = "black"
 known_first_party = ["pydantic_i18n", "pydantic", "babel"]
```

### Comparing `pydantic-i18n-0.3.1/scripts/docs.py` & `pydantic_i18n-0.4.0/scripts/docs.py`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/tests/test_loaders/conftest.py` & `pydantic_i18n-0.4.0/tests/test_loaders/conftest.py`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/tests/test_loaders/test_common.py` & `pydantic_i18n-0.4.0/tests/test_loaders/test_common.py`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/tests/test_main.py` & `pydantic_i18n-0.4.0/tests/test_main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Dict
+from typing import Dict, Tuple
 
 import pytest
 
 from pydantic import BaseModel, ValidationError
 from pydantic_i18n import BaseLoader, DictLoader, PydanticI18n
 
 translations = {
@@ -160,7 +160,33 @@
     with pytest.raises(ValidationError) as e:
         User(**data)
 
     locale = "en_US"
     translated_errors = tr.translate(e.value.errors(), locale=locale)
 
     assert _translations[locale][message] == translated_errors[0]["msg"]
+
+
+def test_multiple_placeholders():
+    _translations = {
+        "en_US": {
+            "wrong tuple length {}, expected {}": "wrong tuple length {}, expected {}",
+            "field required": "field required",
+        },
+        "de_DE": {
+            "wrong tuple length {}, expected {}": "falsche Tupellänge {}, erwartet {}",
+            "field required": "Feld erforderlich",
+        },
+    }
+
+    class MyModel(BaseModel):
+        value: Tuple[str, str]
+
+    tr = PydanticI18n(_translations)
+
+    with pytest.raises(ValidationError) as e:
+        MyModel(value=(1,))
+
+    locale = "de_DE"
+    translated_errors = tr.translate(e.value.errors(), locale=locale)
+
+    assert translated_errors[0]["msg"] == "falsche Tupellänge 1, erwartet 2"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pydantic-i18n-0.3.1/tests/test_pydantic_messages.py` & `pydantic_i18n-0.4.0/tests/test_pydantic_messages.py`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/tests/translations/babel/de_DE/LC_MESSAGES/messages.po` & `pydantic_i18n-0.4.0/tests/translations/babel/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/tests/translations/babel/en_US/LC_MESSAGES/messages.mo` & `pydantic_i18n-0.4.0/tests/translations/babel/en_US/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/tests/translations/babel/en_US/LC_MESSAGES/messages.po` & `pydantic_i18n-0.4.0/tests/translations/babel/en_US/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/tests/translations/babel/es_AR/LC_MESSAGES/messages.mo` & `pydantic_i18n-0.4.0/tests/translations/babel/es_AR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/tests/translations/babel/es_AR/LC_MESSAGES/messages.po` & `pydantic_i18n-0.4.0/tests/translations/babel/es_AR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `pydantic-i18n-0.3.1/PKG-INFO` & `pydantic_i18n-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-i18n
-Version: 0.3.1
+Version: 0.4.0
 Summary: pydantic-i18n is an extension to support an i18n for the pydantic error messages.
 Author-email: Roman Sadzhenytsia <urchin.dukkee@gmail.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -20,31 +20,30 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic >=1.9.0
-Requires-Dist: autoflake ==2.0.1 ; extra == "dev"
+Requires-Dist: autoflake ==2.2.0 ; extra == "dev"
 Requires-Dist: flake8 ==6.0.0 ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
-Requires-Dist: tox >=3.27.1 ; extra == "dev"
-Requires-Dist: mkdocs ==1.4.2 ; extra == "doc"
+Requires-Dist: mkdocs ==1.4.3 ; extra == "doc"
 Requires-Dist: mkdocs-material ==8.5.11 ; extra == "doc"
 Requires-Dist: markdown ==3.2.1 ; extra == "doc"
 Requires-Dist: markdown-include ==0.8.1 ; extra == "doc"
 Requires-Dist: mkdocs-markdownextradata-plugin ==0.2.5 ; extra == "doc"
-Requires-Dist: typer ==0.7.0 ; extra == "doc"
+Requires-Dist: typer ==0.9.0 ; extra == "doc"
 Requires-Dist: pyyaml ==6.0.0 ; extra == "doc"
-Requires-Dist: pytest ==7.2.2 ; extra == "test"
-Requires-Dist: pytest-cov ==4.0.0 ; extra == "test"
+Requires-Dist: pytest ==7.4.0 ; extra == "test"
+Requires-Dist: pytest-cov ==4.1.0 ; extra == "test"
 Requires-Dist: pytest-lazy-fixture ==0.6.3 ; extra == "test"
-Requires-Dist: mypy ==1.0.1 ; extra == "test"
+Requires-Dist: mypy ==1.4.1 ; extra == "test"
 Requires-Dist: flake8 ==6.0.0 ; extra == "test"
-Requires-Dist: black ==23.1.0 ; extra == "test"
+Requires-Dist: black ==23.3.0 ; extra == "test"
 Requires-Dist: isort ==5.12.0 ; extra == "test"
 Requires-Dist: babel ==2.12.1 ; extra == "test"
 Project-URL: Documentation, https://pydantic-i18n.boardpack.org
 Project-URL: Source, https://github.com/boardpack/pydantic-i18n
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
```

