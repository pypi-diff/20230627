# Comparing `tmp/documenteer-0.8.1.tar.gz` & `tmp/documenteer-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "documenteer-0.8.1.tar", last modified: Tue Jun 27 19:20:16 2023, max compression
+gzip compressed data, was "documenteer-1.0.0a1.tar", last modified: Wed Jun  7 19:12:56 2023, max compression
```

## Comparing `documenteer-0.8.1.tar` & `documenteer-1.0.0a1.tar`

### file list

```diff
@@ -1,206 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.700647 documenteer-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-27 19:20:03.000000 documenteer-0.8.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.680647 documenteer-0.8.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-27 19:20:03.000000 documenteer-0.8.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-27 19:20:03.000000 documenteer-0.8.1/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-27 19:20:03.000000 documenteer-0.8.1/.github/SUPPORT.md
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-27 19:20:03.000000 documenteer-0.8.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.680647 documenteer-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-27 19:20:03.000000 documenteer-0.8.1/.github/workflows/ci-cron.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-27 19:20:03.000000 documenteer-0.8.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-27 19:20:03.000000 documenteer-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-27 19:20:03.000000 documenteer-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    29526 2023-06-27 19:20:03.000000 documenteer-0.8.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-27 19:20:03.000000 documenteer-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:03.000000 documenteer-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-27 19:20:03.000000 documenteer-0.8.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-27 19:20:16.700647 documenteer-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-27 19:20:03.000000 documenteer-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.684647 documenteer-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/_rst_epilog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    29526 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.684647 documenteer-0.8.1/docs/dev/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.684647 documenteer-0.8.1/docs/dev/api/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/dev/api/documenteer.conf.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/dev/api/documenteer.ext.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/dev/api/documenteer.requestsutils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/dev/api/documenteer.sphinxconfig.rst
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/dev/api/documenteer.sphinxext.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/dev/api/documenteer.sphinxrunner.rst
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/dev/api/documenteer.stackdocs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/dev/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/dev/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/dev/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/documenteer.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.684647 documenteer-0.8.1/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/guides/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/guides/configuration-preset.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/guides/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/guides/diagrams.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/guides/extend-conf-py.rst
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/guides/organization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/guides/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/guides/pyproject-configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/guides/rst-epilog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/guides/tabsets.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/guides/toml-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.684647 documenteer-0.8.1/docs/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/pipelines/build-overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/pipelines/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/pipelines/cpp-api-linking.rst
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/pipelines/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/pipelines/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/pipelines/package-docs-cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/pipelines/stack-docs-cli.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.688647 documenteer-0.8.1/docs/sphinx-extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/sphinx-extensions/autocppapi.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/sphinx-extensions/autodocreset.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/sphinx-extensions/docushare-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/sphinx-extensions/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/sphinx-extensions/jira-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/sphinx-extensions/lsst-pybtex-style.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/sphinx-extensions/lssttasks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/sphinx-extensions/package-toctree.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/sphinx-extensions/remote-code-block.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.688647 documenteer-0.8.1/docs/technotes/
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/technotes/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/technotes/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-27 19:20:03.000000 documenteer-0.8.1/docs/technotes/refresh-lsst-bib.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.688647 documenteer-0.8.1/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-27 19:20:03.000000 documenteer-0.8.1/licenses/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-27 19:20:03.000000 documenteer-0.8.1/licenses/astropy-helpers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-27 19:20:03.000000 documenteer-0.8.1/licenses/sphinx-issue.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-06-27 19:20:03.000000 documenteer-0.8.1/licenses/sphinx.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-06-27 19:20:03.000000 documenteer-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 19:20:16.700647 documenteer-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.680647 documenteer-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.688647 documenteer-0.8.1/src/documenteer/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.688647 documenteer-0.8.1/src/documenteer/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/assets/rubin-favicon-transparent-32px.png
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/assets/rubin-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/assets/rubin-pydata-theme.css
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/assets/rubin-titlebar-imagotype-light.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.688647 documenteer-0.8.1/src/documenteer/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/bin/buildstackdocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/bin/refreshlsstbib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.688647 documenteer-0.8.1/src/documenteer/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15143 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/conf/_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/conf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/conf/guide.py
--rw-r--r--   0 runner    (1001) docker     (123)    14007 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/conf/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/conf/pipelinespkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/conf/technote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.692647 documenteer-0.8.1/src/documenteer/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/ext/autocppapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/ext/autodocreset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/packagemetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/requestsutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.692647 documenteer-0.8.1/src/documenteer/sphinxconfig/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20527 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxconfig/stackconf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxconfig/technoteconf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxconfig/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.692647 documenteer-0.8.1/src/documenteer/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxext/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxext/jira.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxext/lsstdocushare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.692647 documenteer-0.8.1/src/documenteer/sphinxext/lssttasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxext/lssttasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39808 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxext/lssttasks/configfieldlists.py
--rw-r--r--   0 runner    (1001) docker     (123)    12373 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxext/lssttasks/crossrefs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxext/lssttasks/pyapisummary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxext/lssttasks/taskutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxext/lssttasks/topiclists.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxext/lssttasks/topics.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxext/mockcoderefs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxext/packagetoctree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxext/remotecodeblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxext/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/sphinxrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.692647 documenteer-0.8.1/src/documenteer/stackdocs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/stackdocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/stackdocs/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.696647 documenteer-0.8.1/src/documenteer/stackdocs/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1063166 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml
--rw-r--r--   0 runner    (1001) docker     (123)   105749 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/stackdocs/data/doxygen.defaults.conf
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/stackdocs/data/mainpage.dox
--rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/stackdocs/doxygen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/stackdocs/doxygentag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/stackdocs/packagecli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/stackdocs/pkgdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/stackdocs/rootdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/stackdocs/stackcli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.680647 documenteer-0.8.1/src/documenteer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.696647 documenteer-0.8.1/src/documenteer/templates/pydata/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/templates/pydata/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-27 19:20:03.000000 documenteer-0.8.1/src/documenteer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.688647 documenteer-0.8.1/src/documenteer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-27 19:20:16.000000 documenteer-0.8.1/src/documenteer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-06-27 19:20:16.000000 documenteer-0.8.1/src/documenteer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:20:16.000000 documenteer-0.8.1/src/documenteer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-27 19:20:16.000000 documenteer-0.8.1/src/documenteer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-27 19:20:16.000000 documenteer-0.8.1/src/documenteer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 19:20:16.000000 documenteer-0.8.1/src/documenteer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.696647 documenteer-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.696647 documenteer-0.8.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/data/afw.doxygen.conf
--rw-r--r--   0 runner    (1001) docker     (123)   199942 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/data/doxygen.tag.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.680647 documenteer-0.8.1/tests/data/package_alpha/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.696647 documenteer-0.8.1/tests/data/package_alpha/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.680647 documenteer-0.8.1/tests/data/package_alpha/doc/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.700647 documenteer-0.8.1/tests/data/package_alpha/doc/_static/package_alpha/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/data/package_alpha/doc/_static/package_alpha/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/data/package_alpha/doc/doxygen.conf.in
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/data/package_alpha/doc/manifest.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.700647 documenteer-0.8.1/tests/data/package_alpha/doc/package.alpha/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/data/package_alpha/doc/package.alpha/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.700647 documenteer-0.8.1/tests/data/package_alpha/doc/package_alpha/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/data/package_alpha/doc/package_alpha/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.700647 documenteer-0.8.1/tests/data/package_alpha/include/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/data/package_alpha/include/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.700647 documenteer-0.8.1/tests/data/package_alpha/src/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/data/package_alpha/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.680647 documenteer-0.8.1/tests/data/package_beta/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.700647 documenteer-0.8.1/tests/data/package_beta/doc/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/data/package_beta/doc/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.680647 documenteer-0.8.1/tests/roots/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:20:16.700647 documenteer-0.8.1/tests/roots/test-autocppapi/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/roots/test-autocppapi/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)   199942 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/roots/test-autocppapi/doxygen.tag.zip
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/roots/test-autocppapi/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/test_conf_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/test_conf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/test_ext_autocppapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/test_packagemetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/test_refreshlsstbib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/test_sphinxconfig_stackconf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/test_sphinxconfig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/test_sphinxext_jira.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/test_sphinxext_lsstdocushare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/test_sphinxext_lssttasks_taskutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/test_sphinxext_mockcoderefs.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/test_sphinxext_packagetoctree.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/test_sphinxext_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/test_stackdocs_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/test_stackdocs_doxygen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/test_stackdocs_doxygentag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/test_stackdocs_pkgdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/test_stackdocs_rootdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-27 19:20:03.000000 documenteer-0.8.1/tests/test_technoteconf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-27 19:20:03.000000 documenteer-0.8.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.726858 documenteer-1.0.0a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.github/SUPPORT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.726858 documenteer-1.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.github/workflows/ci-cron.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.npmrc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.nvmrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.prettierrc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.726858 documenteer-1.0.0a1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29338 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.718858 documenteer-1.0.0a1/demo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.726858 documenteer-1.0.0a1/demo/rst-technote/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/demo/rst-technote/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/demo/rst-technote/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/demo/rst-technote/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/demo/rst-technote/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/demo/rst-technote/technote.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.730858 documenteer-1.0.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/_rst_epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    29338 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.730858 documenteer-1.0.0a1/docs/dev/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.730858 documenteer-1.0.0a1/docs/dev/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.conf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.ext.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.requestsutils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.sphinxconfig.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.sphinxext.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.sphinxrunner.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.stackdocs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/html-templates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/theme-assets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/theme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/documenteer.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.730858 documenteer-1.0.0a1/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/configuration-preset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/diagrams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/extend-conf-py.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/openapi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/organization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/pyproject-configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/rst-epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/tabsets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/toml-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.734858 documenteer-1.0.0a1/docs/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/build-overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/cpp-api-linking.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/package-docs-cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/stack-docs-cli.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.734858 documenteer-1.0.0a1/docs/sphinx-extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/autocppapi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/autodocreset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/docushare-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/jira-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/lsst-pybtex-style.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/lssttasks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/openapi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/package-toctree.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/remote-code-block.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.734858 documenteer-1.0.0a1/docs/technotes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/technotes/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/technotes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/technotes/refresh-lsst-bib.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.734858 documenteer-1.0.0a1/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/licenses/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/licenses/astropy-helpers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/licenses/sphinx-issue.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/licenses/sphinx.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   212497 2023-06-07 19:12:44.000000 documenteer-1.0.0a1/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/src/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/src/assets/rubin-technote/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.734858 documenteer-1.0.0a1/src/assets/rubin-technote/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/assets/rubin-technote/styles/_hacks.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/assets/rubin-technote/styles/_properties.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.734858 documenteer-1.0.0a1/src/assets/rubin-technote/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/assets/rubin-technote/styles/components/_global-breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/assets/rubin-technote/styles/components/_index.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/assets/rubin-technote/styles/components/_version-info.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/assets/rubin-technote/styles/rubin-technote.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/assets/rsd-assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-06-07 19:12:46.000000 documenteer-1.0.0a1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-06-07 19:12:46.000000 documenteer-1.0.0a1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/rubin-favicon-transparent-32px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/rubin-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/rubin-pydata-theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/rubin-titlebar-imagotype-light.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-07 19:12:46.000000 documenteer-1.0.0a1/src/documenteer/assets/scripts/rubin-technote.js
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-07 19:12:46.000000 documenteer-1.0.0a1/src/documenteer/assets/scripts/rubin-technote.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/assets/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-06-07 19:12:46.000000 documenteer-1.0.0a1/src/documenteer/assets/styles/rubin-technote.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-06-07 19:12:46.000000 documenteer-1.0.0a1/src/documenteer/assets/styles/rubin-technote.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/bin/buildstackdocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/bin/refreshlsstbib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17519 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/guide.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14007 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/pipelinespkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/technote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/technotebeta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/ext/autocppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/ext/autodocreset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/ext/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/packagemetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/requestsutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.742858 documenteer-1.0.0a1/src/documenteer/sphinxconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20527 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxconfig/stackconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxconfig/technoteconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxconfig/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.742858 documenteer-1.0.0a1/src/documenteer/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lsstdocushare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.742858 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39808 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/configfieldlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12373 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/crossrefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/pyapisummary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/taskutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/topiclists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/topics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/mockcoderefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/packagetoctree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/remotecodeblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.742858 documenteer-1.0.0a1/src/documenteer/stackdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.746858 documenteer-1.0.0a1/src/documenteer/stackdocs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1063166 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   105749 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/data/doxygen.defaults.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/data/mainpage.dox
+-rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/doxygentag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/packagecli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/pkgdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/rootdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/stackcli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/src/documenteer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.746858 documenteer-1.0.0a1/src/documenteer/templates/pydata/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/templates/pydata/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.746858 documenteer-1.0.0a1/src/documenteer/templates/technote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/templates/technote/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.746858 documenteer-1.0.0a1/src/documenteer/templates/technote/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/templates/technote/components/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.750858 documenteer-1.0.0a1/src/documenteer/templates/technote/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/templates/technote/sections/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/templates/technote/sections/header-article.html
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/templates/technote/sections/sidebar-primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-06-07 19:12:56.000000 documenteer-1.0.0a1/src/documenteer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-06-07 19:12:56.000000 documenteer-1.0.0a1/src/documenteer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:12:56.000000 documenteer-1.0.0a1/src/documenteer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-07 19:12:56.000000 documenteer-1.0.0a1/src/documenteer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-07 19:12:56.000000 documenteer-1.0.0a1/src/documenteer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 19:12:56.000000 documenteer-1.0.0a1/src/documenteer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.758858 documenteer-1.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.758858 documenteer-1.0.0a1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/afw.doxygen.conf
+-rw-r--r--   0 runner    (1001) docker     (123)   199942 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/doxygen.tag.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/tests/data/package_alpha/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.758858 documenteer-1.0.0a1/tests/data/package_alpha/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/tests/data/package_alpha/doc/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.758858 documenteer-1.0.0a1/tests/data/package_alpha/doc/_static/package_alpha/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/doc/_static/package_alpha/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/doc/doxygen.conf.in
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/doc/manifest.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/tests/data/package_alpha/doc/package.alpha/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/doc/package.alpha/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/tests/data/package_alpha/doc/package_alpha/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/doc/package_alpha/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/tests/data/package_alpha/include/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/include/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/tests/data/package_alpha/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/tests/data/package_beta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/tests/data/package_beta/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_beta/doc/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.726858 documenteer-1.0.0a1/tests/roots/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/tests/roots/test-autocppapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/roots/test-autocppapi/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   199942 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/roots/test-autocppapi/doxygen.tag.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/roots/test-autocppapi/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_conf_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_conf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_ext_autocppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_packagemetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_refreshlsstbib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxconfig_stackconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxconfig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxext_jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxext_lsstdocushare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxext_lssttasks_taskutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxext_mockcoderefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxext_packagetoctree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxext_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_stackdocs_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_stackdocs_doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_stackdocs_doxygentag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_stackdocs_pkgdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_stackdocs_rootdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_technoteconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/webpack.config.js
```

### Comparing `documenteer-0.8.1/.github/workflows/ci-cron.yaml` & `documenteer-1.0.0a1/.github/workflows/ci-cron.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -16,24 +16,37 @@
       matrix:
         python-version:
           - "3.8"
           - "3.9"
           - "3.10"
           - "3.11"
         sphinx-version:
-          - "4"
           - "5"
-          - "6"
           - "dev"
 
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0 # full history for setuptools_scm
 
+      - uses: actions/setup-node@v3
+        with:
+          node-version-file: '.nvmrc'
+
+      - name: Authenticate GitHub Packages
+        run: |
+          echo "//npm.pkg.github.com/:_authToken=${NPM_PKG_TOKEN}" > ~/.npmrc
+        env:
+          NPM_PKG_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+
+      - name: npm install and build
+        run: |
+          npm install
+          npm run build
+
       - name: Run tests in tox
         uses: lsst-sqre/run-tox@v1
         with:
           python-version: ${{ matrix.python-version }}
           tox-envs: "lint,typing-sphinx${{ matrix.sphinx-version }},py-test-sphinx${{ matrix.sphinx-version }}"
           use-cache: false
 
@@ -56,13 +69,28 @@
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0 # full history for setuptools_scm
 
+      - uses: actions/setup-node@v3
+        with:
+          node-version-file: '.nvmrc'
+
+      - name: Authenticate GitHub Packages
+        run: |
+          echo "//npm.pkg.github.com/:_authToken=${NPM_PKG_TOKEN}" > ~/.npmrc
+        env:
+          NPM_PKG_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+
+      - name: npm install and build
+        run: |
+          npm install
+          npm run build
+
       - name: Build and publish
         uses: lsst-sqre/build-and-publish-to-pypi@v1
         with:
           pypi-token: ""
           python-version: "3.11"
           upload: false
```

### Comparing `documenteer-0.8.1/.gitignore` & `documenteer-1.0.0a1/.gitignore`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# JavaScript
+node_modules/
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 
 # C extensions
 *.so
 
@@ -55,13 +58,10 @@
 
 # Sphinx documentation
 docs/_build/
 
 # PyBuilder
 target/
 
-.venv/
-demo/
-node_modules/
-src/documenteer/assets/rsd-assets/
-src/documenteer/assets/scripts/
-src/documenteer/assets/styles/
+# Python environments
+.venv
+venv
```

### Comparing `documenteer-0.8.1/.pre-commit-config.yaml` & `documenteer-1.0.0a1/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -22,17 +22,23 @@
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: 1.14.0
+    rev: 1.13.0
     hooks:
       - id: blacken-docs
-        additional_dependencies: [black==23.3.0]
+        additional_dependencies: [black==22.12.0]
         args: [-l, '79', -t, py38]
 
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
+
+  - repo: https://github.com/pre-commit/mirrors-prettier
+    rev: v3.0.0-alpha.6
+    hooks:
+      - id: prettier
+        types_or: [css, scss, javascript]
```

### Comparing `documenteer-0.8.1/CHANGELOG.md` & `documenteer-1.0.0a1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,20 @@
 # Change Log
 
-## 0.8.1 (2023-06-27)
+## Unreleased
 
-Fixes:
-
-- Fixed a bug in the in the `help` subcommand for the `package-docs` and `stack-docs` commands.
-
-## 0.8.0 (2023-07-23)
-
-New features:
-
-- Added a `-W` / `--warning-is-error` flag to the `package-docs build` and `stack-docs build` commands for Science Pipelines documentation builds. This flag causes Sphinx to treat warnings as errors, which is useful for CI builds.
-- Also added a `-n` / `--nitpicky` flag that enables Sphinx's nitpicky mode to flag warnings when links cannot resolve.
-
-Fixes:
-
-- Pinned `sphinx-autodoc-typehints<1.23.0` to avoid a Sphinx version conflict with `sphinx-design`. The former required Sphinx >= 7.
-
-## 0.7.5 (2023-06-07)
-
-Fixes:
-
-- Use [sphinxcontrib-jquery](https://github.com/sphinx-contrib/jquery/) to ensure jQuery is available for user guide and Pipelines documentation builds. Sphinx 6 dropped jQuery from its default theme, and the new pydata-sphinx-theme v0.12 does not include it either.
-
-## 0.7.4 (2023-05-16)
-
-Fixes:
-
-- Pinned Sphinx < 7 for the `pipelines` and `technote` extras since their themes are not currently compatible with Sphinx 7 and later.
-
-## 0.7.3 (2023-03-20)
-
-Fixes:
-
-- Add `requirements.txt` and `.venv`/`venv` to the default `exclude_patterns` for User Guides.
-
-## 0.7.2 (2023-03-01)
-
-Fixes:
-
-- Temporarily pin pydata-sphinx-theme to <0.13. The new version changed how it treats light/dark logos.
-
-## 0.7.1 (2023-02-23)
-
-Fixes:
-
-- Temporarily pinning Mermaid to 9.4.0 in the User Guide configuration to workaround a change in the Mermaid CDN.
+- Add a new `documenteer.conf.technotebeta` configuration for [technote](https://technote.lsst.io)-based technotes.
+  These technotes are now themed with Rubin's modern branding.
+- Drop support for Python 3.7.
+- Drop support for Sphinx versions earlier than 5.
+- Temporarily pin pydata-sphinx-theme < 0.13 on account of a change in logo path checking (affects user guide projects).
+- Use [sphinxcontrib-jquery](https://github.com/sphinx-contrib/jquery/) to ensure jQuery is available for user guide and Pipelines documentation builds.
+- Add a new `sphinx.exclude` field to `documenteer.toml` to list files for exclusion from a documentation project.
+  More files and directories like `.venv` and `requirements.txt` are now excluded, as well.
+- New support for embedding OpenAPI documentation in a Redoc-generated subsite. The `documenteer.ext.openapi` extension can call a user-specified function to generate and install the OpenAPI specification the Sphinx source. For user guide projects, the `[project.openapi]` table in `documenteer.toml` can be used to configure both the `documenteer.ext.openapi` and `sphinxcontrib-redoc` extensions. [sphinxcontrib-redoc](https://sphinxcontrib-redoc.readthedocs.io/en/stable/) is installed and configured by default for all Rubin user guide projects (projects that use `documenteer.conf.guide`).
 
 ## 0.7.0 (2022-10-20)
 
 - Documenteer provides a new Sphinx configuration profile for general Rubin user guide projects, `documenteer.conf.guide`.
   This configuration profile features the new [pydata-sphinx-theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/), with customizations based on design tokens from the [Rubin Style Dictionary](https://style-dictionary.lsst.io).
   Most metadata and Sphinx configurations can also be set through a `documenteer.toml` file, located alongside the standard Sphinx `conf.py` file.
   Install `documenteer[guide]` with `pip` to get the dependencies needed for this Sphinx configuration.
@@ -151,15 +116,15 @@
 
 ## 0.6.3 (2021-02-01)
 
 Fixes:
 
 - Documenteer works with the latest version of [sphinxcontrib-bibtex](https://github.com/mcmtroffaes/sphinxcontrib-bibtex).
   Both the new (`documenteer.conf.technote`) and old (`documenteer.sphinxconfig.technoteconf`) versions of the technote configuration use the new `bibtex_bibfiles` configuration variable.
-  Version 2.0.0 or later of `sphinxcontrib-bibtex`\_ is now required because of that package's API.
+  Version 2.0.0 or later of `sphinxcontrib-bibtex`_ is now required because of that package's API.
 
 ## 0.6.2 (2020-10-08)
 
 Fixes:
 
 - The `build-stack-docs` CLI (replaced by `stack-docs build`) now defaults to not generating a Doxygen configuration, or running Doxygen.
   This is consistent with the original behavior of `build-stack-docs`, which did not perform a Doxygen build.
@@ -256,15 +221,15 @@
   - Improved the README to list features.
 
 - Added GitHub community health features: contributing, support, and code of conduct files.
 
 ## 0.5.5 (2019-12-09)
 
 - Technote configuration now uses `yaml.safe_load` instead of `yaml.load`.
-  See the [pyyaml docs for details](<https://github.com/yaml/pyyaml/wiki/PyYAML-yaml.load(input)-Deprecation>).
+  See the [pyyaml docs for details](https://github.com/yaml/pyyaml/wiki/PyYAML-yaml.load(input)-Deprecation).
   [[DM-22537](https://jira.lsstcorp.org/browse/DM-22537)]
 
 ## 0.5.4 (2019-11-03)
 
 - This new version of the technote sphinx theme should fix the edition link in the sidebar for non-main editions.
   [[DM-20839](https://jira.lsstcorp.org/browse/DM-20839)]
 
@@ -382,15 +347,15 @@
 
 - Added Astropy to the intersphinx configuration.
 
 - Enabled `automodsumm_inherited_members` in the stackconf for stack documentation.
   This configuration is critical:
 
   1. It is actually responsible for ensuring that inherited members of classes appear in our docs.
-  2. Without this, classes that have a `__slots__` attribute (typically through inheritance of a `collections.abc` class) won't have _any_ of their members documented. See (DM-16102)(https://jira.lsstcorp.org/browse/DM-16102) for discussion.
+  2. Without this, classes that have a `__slots__` attribute (typically through inheritance of a `collections.abc` class) won't have *any* of their members documented. See (DM-16102)(https://jira.lsstcorp.org/browse/DM-16102) for discussion.
 
 - `todo` directives are now hidden when using `build_pipelines_lsst_io_configs`.
   They are still shown, by default, for standalone package documentation builds, which are primarily developer-facing.
 
 ## 0.3.0 (2018-09-19)
 
 - New `remote-code-block`, which works like the `literalinclude` directive, but allows you to include content from a URL over the web.
@@ -416,15 +381,15 @@
   This change lets multiple command-line front-ends to drive Sphinx.
 
 - Various improvements to the configuration for LSST Stack-based documentation projects (`documenteer.sphinxconf.stackconf`):
 
   - Add `documenteer.sphinxconf.stackconf.build_pipelines_lsst_io_configs` to configure the Sphinx build of the https://github.com/lsst/pipelines_lsst_io repo.
     This pattern lets us share configurations between per-package documentation builds and the "stack" build in `pipelines_lsst_io`.
 
-  - Replaced the third-party `astropy_helpers`_ package with the numpydoc_ and `sphinx-automodapi`\_ packages.
+  - Replaced the third-party `astropy_helpers`_ package with the numpydoc_ and `sphinx-automodapi`_ packages.
     This helps reduce the number of extraneous dependencies needed for Stack documentation.
 
   - `autoclass_content` is now `"class"`, fitting the LSST DM standards for writing class docstrings, and not filling out `__init__` docstrings.
 
   - Added `scikit-learn` and `pandas` to the intersphinx configuration; removed h5py from intersphinx since it was never needed and conflicted with `daf_butler` documentation.
 
   - Removed the viewcode extension since that won't scale well with the LSST codebase.
@@ -511,15 +476,15 @@
 ## 0.1.11 (2017-03-01)
 
 - Add `documenteer.sphinxconfig.utils.form_ltd_edition_name` to form LSST the Docs-like edition names for Git refs.
 - Configure automated PyPI deployments with Travis.
 
 ## 0.1.10 (2016-12-14)
 
-Includes prototype support for LSST Science Pipelines documentation, as part of `DM-6199 <https://jira.lsstcorp.org/browse/DM-6199>`\_\_:
+Includes prototype support for LSST Science Pipelines documentation, as part of `DM-6199 <https://jira.lsstcorp.org/browse/DM-6199>`__:
 
 - Added dependencies to [breathe](http://breathe.readthedocs.io/en/latest/), [astropy-helpers](https://github.com/astropy/astropy-helpers) and the [lsst-sphinx-bootstrap-theme](https://github.com/lsst-sqre/lsst-sphinx-bootstrap-theme) to generally coordinate LSST Science Pipelines documentation dependencies.
 - Created `documenteer.sphinxconfig.stackconf` module to centrally coordinate Science Pipelines documentation configuration. Much of the configuration is based on [astropy-helper's Sphinx configuration](https://github.com/astropy/astropy-helpers/blob/master/astropy_helpers/sphinx/conf.py) since the LSST Science Pipelines documentation is heavily based upon Astropy's Sphinx theme and API reference generation infrastructure.
   Also includes prototype configuration for breathe (the doxygen XML bridge).
 - Updated test harness (pytest and plugin versions).
 
 ## 0.1.9 (2016-07-08)
```

### Comparing `documenteer-0.8.1/LICENSE` & `documenteer-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/PKG-INFO` & `documenteer-1.0.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: documenteer
-Version: 0.8.1
+Version: 1.0.0a1
 Summary: Rubin Observatory / LSST Sphinx documentation tools, extensions, and configurations.
 License: The MIT License (MIT)
         
         Copyright (c) 2015-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -27,34 +27,34 @@
 Project-URL: Homepage, https://documenteer.lsst.io
 Project-URL: Source, https://github.com/lsst-sqre/documenteer
 Keywords: rubin,lsst
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: guide
 Provides-Extra: technote
 Provides-Extra: pipelines
 License-File: LICENSE
 
-[![Documentation](https://img.shields.io/badge/documenteer-lsst.io-brightgreen.svg)](https://documenteer.lsst.io)
+[![Documentation](https://img.shields.io/badge/documenteer-lsst.io-brightgreen.svg)](https://documentation.lsst.io)
 [![PyPI](https://img.shields.io/pypi/v/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![For Python 3.7+](https://img.shields.io/pypi/pyversions/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![MIT license](https://img.shields.io/pypi/l/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![CI](https://github.com/lsst-sqre/documenteer/actions/workflows/ci.yaml/badge.svg)](https://github.com/lsst-sqre/documenteer/actions/workflows/ci.yaml)
 [![Weekly CI](https://github.com/lsst-sqre/documenteer/actions/workflows/ci-cron.yaml/badge.svg)](https://github.com/lsst-sqre/documenteer/actions/workflows/ci-cron.yaml)
 
 # Documenteer
@@ -66,15 +66,15 @@
 Browse the [lsst-doc-engineering](https://github.com/topics/lsst-doc-engineering) GitHub topic for more Rubin Observatory documentation engineering projects.
 
 ## Quick installation:
 
 For [user guides](https://documenteer.lsst.io/guides/index.html):
 
 ```sh
-pip install "documenteer[guides]"
+pip install "documenteer[technote]"
 ```
 
 For [technical note projects](https://documenteer.lsst.io/technotes/index.html):
 
 ```sh
 pip install "documenteer[technote]"
 ```
```

### Comparing `documenteer-0.8.1/README.md` & `documenteer-1.0.0a1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Documentation](https://img.shields.io/badge/documenteer-lsst.io-brightgreen.svg)](https://documenteer.lsst.io)
+[![Documentation](https://img.shields.io/badge/documenteer-lsst.io-brightgreen.svg)](https://documentation.lsst.io)
 [![PyPI](https://img.shields.io/pypi/v/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![For Python 3.7+](https://img.shields.io/pypi/pyversions/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![MIT license](https://img.shields.io/pypi/l/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![CI](https://github.com/lsst-sqre/documenteer/actions/workflows/ci.yaml/badge.svg)](https://github.com/lsst-sqre/documenteer/actions/workflows/ci.yaml)
 [![Weekly CI](https://github.com/lsst-sqre/documenteer/actions/workflows/ci-cron.yaml/badge.svg)](https://github.com/lsst-sqre/documenteer/actions/workflows/ci-cron.yaml)
 
 # Documenteer
@@ -14,15 +14,15 @@
 Browse the [lsst-doc-engineering](https://github.com/topics/lsst-doc-engineering) GitHub topic for more Rubin Observatory documentation engineering projects.
 
 ## Quick installation:
 
 For [user guides](https://documenteer.lsst.io/guides/index.html):
 
 ```sh
-pip install "documenteer[guides]"
+pip install "documenteer[technote]"
 ```
 
 For [technical note projects](https://documenteer.lsst.io/technotes/index.html):
 
 ```sh
 pip install "documenteer[technote]"
 ```
```

### Comparing `documenteer-0.8.1/docs/Makefile` & `documenteer-1.0.0a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/_rst_epilog.rst` & `documenteer-1.0.0a1/docs/_rst_epilog.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 .. Links and substitutions available from every rst page
 
 .. External links
 
 .. _Doxygen: http://www.doxygen.nl
 .. _Doxylink: https://sphinxcontrib-doxylink.readthedocs.io/en/stable/
+.. _FastAPI: https://fastapi.tiangolo.com
 .. _Intersphinx: https://www.sphinx-doc.org/en/master/usage/extensions/intersphinx.html
-.. _LSST Science Pipelines:
 .. _SCons: https://scons.org
 .. _Sphinx extensions: https://www.sphinx-doc.org/en/master/develop.html
 .. _Sphinx: https://www.sphinx-doc.org/en/master/
 .. _Mermaid: https://mermaid-js.github.io/mermaid/#/
 .. _sphinxcontrib-mermaid: https://github.com/mgaitan/sphinxcontrib-mermaid
 .. _Diagrams: https://diagrams.mingrammer.com/
 .. _sphinx-diagrams: https://github.com/j-martin/sphinx-diagrams
 .. _`#dm-docs`: https://lsstc.slack.com/archives/C2B6DQBAL
 .. _`DMTN-030`:
 .. _`DMTN-030 Science Pipelines Documentation Design`: https://dmtn-030.lsst.io
 .. _`Google Developer Style Guide`: https://developers.google.com/style/
 .. _`LSST DM Docstring Style Guide`: https://developer.lsst.io/python/style.html
 .. _`LSST DM ReStructuredTextStyle Guide`: https://developer.lsst.io/restructuredtext/style.html
 .. _`LSST DM User Documentation Style Guide`: https://developer.lsst.io/user-docs/index.html
+.. _`pydata-sphinx-theme`:
 .. _`PyData Sphinx Theme`: https://pydata-sphinx-theme.readthedocs.io/en/stable/
 .. _`Sphinx Design`: https://sphinx-design.readthedocs.io/en/latest/index.html
 .. _`MyST`: https://myst-parser.readthedocs.io/en/latest/intro.html
 .. _TOML: https://toml.io/en/
 .. _`SQR-006`: https://sqr-006.lsst.io
 .. _`lsstDoxygen`: https://github.com/lsst/lsstDoxygen
 .. _`package-docs`: https://documenteer.lsst.io/pipelines/package-docs-cli.html
 .. _`pex_config`: https://github.com/lsst/pex_config
 .. _`pipe_base`: https://github.com/lsst/pipe_base
 .. _`pipe_supertask`: https://github.com/lsst/pipe_supertask
+.. _LSST Science Pipelines:
 .. _`pipelines.lsst.io`: https://pipelines.lsst.io
 .. _`pipelines_lsst_io`: https://github.com/lsst/pipelines_lsst_io
 .. _`sconsUtils`: https://github.com/lsst/sconsUtils
 .. _`sqre/infrastructure/documenteer`: https://ci.lsst.codes/blue/organizations/jenkins/sqre%2Finfrastructure%2Fdocumenteer/activity
 .. _astro-metadata-translator.lsst.io: https://astro-metadata-translator.lsst.io
 .. _automodapi: http://sphinx-automodapi.readthedocs.io/en/latest/automodapi.html
 .. _black: https://black.readthedocs.io/en/stable/
@@ -42,19 +44,22 @@
 .. _conda: https://conda.io/en/latest/index.html
 .. _isort: https://pycqa.github.io/isort/
 .. _numpydoc: https://numpydoc.readthedocs.io/en/latest/index.html
 .. _pre-commit: https://pre-commit.com
 .. _pytest: https://pytest.org
 .. _toctree: http://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html#directive-toctree
 .. _linkcheck: https://www.sphinx-doc.org/en/master/usage/configuration.html?#options-for-the-linkcheck-builder
+.. _Redoc: https://redocly.com/redoc/
 .. _rst_epilog: https://www.sphinx-doc.org/en/master/usage/configuration.html?highlight=rst_epilog#confval-rst_epilog
 .. _napoleon: https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html
 .. _autodoc: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html
 .. _sphinx_autodoc_typehints: https://github.com/tox-dev/sphinx-autodoc-typehints
+.. _sphinxcontrib-redoc: https://sphinxcontrib-redoc.readthedocs.io/en/stable/
 .. _tox: https://tox.wiki/en/latest/
+.. _Technote: https://technote.lsst.io/
 
 .. Internal links
 
 .. |documenteer.toml| replace:: :doc:`documenteer.toml </guides/toml-reference>`
 .. |documenteer.conf.guide| replace:: :doc:`documenteer.conf.guide </guides/configuration-preset>`
 .. |package-docs| replace:: :doc:`package-docs </pipelines/package-docs-cli>`
 .. |stack-docs| replace:: :doc:`stack-docs </pipelines/stack-docs-cli>`
```

### Comparing `documenteer-0.8.1/docs/changelog.md` & `documenteer-1.0.0a1/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,20 @@
 # Change Log
 
-## 0.8.1 (2023-06-27)
+## Unreleased
 
-Fixes:
-
-- Fixed a bug in the in the `help` subcommand for the `package-docs` and `stack-docs` commands.
-
-## 0.8.0 (2023-07-23)
-
-New features:
-
-- Added a `-W` / `--warning-is-error` flag to the `package-docs build` and `stack-docs build` commands for Science Pipelines documentation builds. This flag causes Sphinx to treat warnings as errors, which is useful for CI builds.
-- Also added a `-n` / `--nitpicky` flag that enables Sphinx's nitpicky mode to flag warnings when links cannot resolve.
-
-Fixes:
-
-- Pinned `sphinx-autodoc-typehints<1.23.0` to avoid a Sphinx version conflict with `sphinx-design`. The former required Sphinx >= 7.
-
-## 0.7.5 (2023-06-07)
-
-Fixes:
-
-- Use [sphinxcontrib-jquery](https://github.com/sphinx-contrib/jquery/) to ensure jQuery is available for user guide and Pipelines documentation builds. Sphinx 6 dropped jQuery from its default theme, and the new pydata-sphinx-theme v0.12 does not include it either.
-
-## 0.7.4 (2023-05-16)
-
-Fixes:
-
-- Pinned Sphinx < 7 for the `pipelines` and `technote` extras since their themes are not currently compatible with Sphinx 7 and later.
-
-## 0.7.3 (2023-03-20)
-
-Fixes:
-
-- Add `requirements.txt` and `.venv`/`venv` to the default `exclude_patterns` for User Guides.
-
-## 0.7.2 (2023-03-01)
-
-Fixes:
-
-- Temporarily pin pydata-sphinx-theme to <0.13. The new version changed how it treats light/dark logos.
-
-## 0.7.1 (2023-02-23)
-
-Fixes:
-
-- Temporarily pinning Mermaid to 9.4.0 in the User Guide configuration to workaround a change in the Mermaid CDN.
+- Add a new `documenteer.conf.technotebeta` configuration for [technote](https://technote.lsst.io)-based technotes.
+  These technotes are now themed with Rubin's modern branding.
+- Drop support for Python 3.7.
+- Drop support for Sphinx versions earlier than 5.
+- Temporarily pin pydata-sphinx-theme < 0.13 on account of a change in logo path checking (affects user guide projects).
+- Use [sphinxcontrib-jquery](https://github.com/sphinx-contrib/jquery/) to ensure jQuery is available for user guide and Pipelines documentation builds.
+- Add a new `sphinx.exclude` field to `documenteer.toml` to list files for exclusion from a documentation project.
+  More files and directories like `.venv` and `requirements.txt` are now excluded, as well.
+- New support for embedding OpenAPI documentation in a Redoc-generated subsite. The `documenteer.ext.openapi` extension can call a user-specified function to generate and install the OpenAPI specification the Sphinx source. For user guide projects, the `[project.openapi]` table in `documenteer.toml` can be used to configure both the `documenteer.ext.openapi` and `sphinxcontrib-redoc` extensions. [sphinxcontrib-redoc](https://sphinxcontrib-redoc.readthedocs.io/en/stable/) is installed and configured by default for all Rubin user guide projects (projects that use `documenteer.conf.guide`).
 
 ## 0.7.0 (2022-10-20)
 
 - Documenteer provides a new Sphinx configuration profile for general Rubin user guide projects, `documenteer.conf.guide`.
   This configuration profile features the new [pydata-sphinx-theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/), with customizations based on design tokens from the [Rubin Style Dictionary](https://style-dictionary.lsst.io).
   Most metadata and Sphinx configurations can also be set through a `documenteer.toml` file, located alongside the standard Sphinx `conf.py` file.
   Install `documenteer[guide]` with `pip` to get the dependencies needed for this Sphinx configuration.
@@ -151,15 +116,15 @@
 
 ## 0.6.3 (2021-02-01)
 
 Fixes:
 
 - Documenteer works with the latest version of [sphinxcontrib-bibtex](https://github.com/mcmtroffaes/sphinxcontrib-bibtex).
   Both the new (`documenteer.conf.technote`) and old (`documenteer.sphinxconfig.technoteconf`) versions of the technote configuration use the new `bibtex_bibfiles` configuration variable.
-  Version 2.0.0 or later of `sphinxcontrib-bibtex`\_ is now required because of that package's API.
+  Version 2.0.0 or later of `sphinxcontrib-bibtex`_ is now required because of that package's API.
 
 ## 0.6.2 (2020-10-08)
 
 Fixes:
 
 - The `build-stack-docs` CLI (replaced by `stack-docs build`) now defaults to not generating a Doxygen configuration, or running Doxygen.
   This is consistent with the original behavior of `build-stack-docs`, which did not perform a Doxygen build.
@@ -256,15 +221,15 @@
   - Improved the README to list features.
 
 - Added GitHub community health features: contributing, support, and code of conduct files.
 
 ## 0.5.5 (2019-12-09)
 
 - Technote configuration now uses `yaml.safe_load` instead of `yaml.load`.
-  See the [pyyaml docs for details](<https://github.com/yaml/pyyaml/wiki/PyYAML-yaml.load(input)-Deprecation>).
+  See the [pyyaml docs for details](https://github.com/yaml/pyyaml/wiki/PyYAML-yaml.load(input)-Deprecation).
   [[DM-22537](https://jira.lsstcorp.org/browse/DM-22537)]
 
 ## 0.5.4 (2019-11-03)
 
 - This new version of the technote sphinx theme should fix the edition link in the sidebar for non-main editions.
   [[DM-20839](https://jira.lsstcorp.org/browse/DM-20839)]
 
@@ -382,15 +347,15 @@
 
 - Added Astropy to the intersphinx configuration.
 
 - Enabled `automodsumm_inherited_members` in the stackconf for stack documentation.
   This configuration is critical:
 
   1. It is actually responsible for ensuring that inherited members of classes appear in our docs.
-  2. Without this, classes that have a `__slots__` attribute (typically through inheritance of a `collections.abc` class) won't have _any_ of their members documented. See (DM-16102)(https://jira.lsstcorp.org/browse/DM-16102) for discussion.
+  2. Without this, classes that have a `__slots__` attribute (typically through inheritance of a `collections.abc` class) won't have *any* of their members documented. See (DM-16102)(https://jira.lsstcorp.org/browse/DM-16102) for discussion.
 
 - `todo` directives are now hidden when using `build_pipelines_lsst_io_configs`.
   They are still shown, by default, for standalone package documentation builds, which are primarily developer-facing.
 
 ## 0.3.0 (2018-09-19)
 
 - New `remote-code-block`, which works like the `literalinclude` directive, but allows you to include content from a URL over the web.
@@ -416,15 +381,15 @@
   This change lets multiple command-line front-ends to drive Sphinx.
 
 - Various improvements to the configuration for LSST Stack-based documentation projects (`documenteer.sphinxconf.stackconf`):
 
   - Add `documenteer.sphinxconf.stackconf.build_pipelines_lsst_io_configs` to configure the Sphinx build of the https://github.com/lsst/pipelines_lsst_io repo.
     This pattern lets us share configurations between per-package documentation builds and the "stack" build in `pipelines_lsst_io`.
 
-  - Replaced the third-party `astropy_helpers`_ package with the numpydoc_ and `sphinx-automodapi`\_ packages.
+  - Replaced the third-party `astropy_helpers`_ package with the numpydoc_ and `sphinx-automodapi`_ packages.
     This helps reduce the number of extraneous dependencies needed for Stack documentation.
 
   - `autoclass_content` is now `"class"`, fitting the LSST DM standards for writing class docstrings, and not filling out `__init__` docstrings.
 
   - Added `scikit-learn` and `pandas` to the intersphinx configuration; removed h5py from intersphinx since it was never needed and conflicted with `daf_butler` documentation.
 
   - Removed the viewcode extension since that won't scale well with the LSST codebase.
@@ -511,15 +476,15 @@
 ## 0.1.11 (2017-03-01)
 
 - Add `documenteer.sphinxconfig.utils.form_ltd_edition_name` to form LSST the Docs-like edition names for Git refs.
 - Configure automated PyPI deployments with Travis.
 
 ## 0.1.10 (2016-12-14)
 
-Includes prototype support for LSST Science Pipelines documentation, as part of `DM-6199 <https://jira.lsstcorp.org/browse/DM-6199>`\_\_:
+Includes prototype support for LSST Science Pipelines documentation, as part of `DM-6199 <https://jira.lsstcorp.org/browse/DM-6199>`__:
 
 - Added dependencies to [breathe](http://breathe.readthedocs.io/en/latest/), [astropy-helpers](https://github.com/astropy/astropy-helpers) and the [lsst-sphinx-bootstrap-theme](https://github.com/lsst-sqre/lsst-sphinx-bootstrap-theme) to generally coordinate LSST Science Pipelines documentation dependencies.
 - Created `documenteer.sphinxconfig.stackconf` module to centrally coordinate Science Pipelines documentation configuration. Much of the configuration is based on [astropy-helper's Sphinx configuration](https://github.com/astropy/astropy-helpers/blob/master/astropy_helpers/sphinx/conf.py) since the LSST Science Pipelines documentation is heavily based upon Astropy's Sphinx theme and API reference generation infrastructure.
   Also includes prototype configuration for breathe (the doxygen XML bridge).
 - Updated test harness (pytest and plugin versions).
 
 ## 0.1.9 (2016-07-08)
```

### Comparing `documenteer-0.8.1/docs/dev/api/documenteer.sphinxext.rst` & `documenteer-1.0.0a1/docs/dev/api/documenteer.sphinxext.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/dev/api/documenteer.stackdocs.rst` & `documenteer-1.0.0a1/docs/dev/api/documenteer.stackdocs.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/dev/development.rst` & `documenteer-1.0.0a1/docs/dev/development.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/dev/release.rst` & `documenteer-1.0.0a1/docs/dev/release.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/documenteer.toml` & `documenteer-1.0.0a1/docs/documenteer.toml`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/guides/badges.rst` & `documenteer-1.0.0a1/docs/guides/badges.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/guides/configuration.rst` & `documenteer-1.0.0a1/docs/guides/configuration.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ##############################################################
 Setting up the Documenteer configuration for Rubin user guides
 ##############################################################
 
-Documenteer provides centralized configuration, |documenteer.conf.guide| for Rubin Observatory user guide websites created with Sphinx.
+Documenteer provides centralized configuration, |documenteer.conf.guide|, for Rubin Observatory user guide websites created with Sphinx.
 This page page shows how to add Documenteer as a Python dependency, install Documenteer's Sphinx configuration, and then customize that configuration.
 
 Python dependency
 =================
 
 First, add ``documenteer`` and its ``guide`` extra as a dependency to your project.
 How you do this depends on your project's packaging structure:
```

### Comparing `documenteer-0.8.1/docs/guides/diagrams.rst` & `documenteer-1.0.0a1/docs/guides/diagrams.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/guides/extend-conf-py.rst` & `documenteer-1.0.0a1/docs/guides/extend-conf-py.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/guides/index.rst` & `documenteer-1.0.0a1/docs/guides/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 .. toctree::
    :maxdepth: 2
    :caption: Advanced configuration
    :name: toc-guides-advanced-config
 
    pyproject-configuration
+   openapi
    rst-epilog
    extend-conf-py
 
 .. toctree::
    :maxdepth: 2
    :caption: Design features
    :name: toc-guides-design
```

### Comparing `documenteer-0.8.1/docs/guides/organization.rst` & `documenteer-1.0.0a1/docs/guides/organization.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ########################################
 Organizing content in a Rubin user guide
 ########################################
 
 Once your Sphinx project is :doc:`configured to use the Rubin user guide theme <configuration>`, the next step is to organize your content into pages and directories, and create links into those pages with Sphinx toctrees.
 The HTML theme of Rubin user guides, based on `PyData Sphinx Theme`_, offers multiple layers of navigational UI.
-Taking best advantage of that navigational UI requires specific considerations for how the Sphinx toctrees are structured.
+Taking best advantage of that navigational UI requires specific considerations for how the Sphinx |toctree| directives are structured.
 This page describes the navigational architecture of the HTML theme and its relationship to Sphinx toctrees, and includes suggested layouts for common project types.
 
 Navigational levels in the HTML theme
 =====================================
 
 The HTML theme provides four levels of navigation:
 
@@ -16,15 +16,15 @@
 #. Section segments, which appear as bold labels in the primary (right side) sidebar
 #. Pages, which appear as links in the primary (right side) sidebar
 #. Page sections, which appear as links in the secondary (left side) sidebar
 
 Creating sections
 =================
 
-Sections are the *root* level |toctree| items in the homepage of your documenation project (the root-level :file:`index.rst` or :file:`index.md` file).
+Sections are the *root* level |toctree| items in the homepage of your documentation project (the root-level :file:`index.rst` or :file:`index.md` file).
 In this example, there are three sections (a user guide, a developer guide, and a change log):
 
 .. code-block:: rst
    :caption: index.rst
 
    .. toctree::
 
@@ -41,14 +41,15 @@
    :caption: index.rst
 
    .. toctree::
 
       user-guide/index
 
    .. toctree::
+
       api
 
    .. toctree::
 
       dev/index
 
    .. toctree::
```

### Comparing `documenteer-0.8.1/docs/guides/overview.rst` & `documenteer-1.0.0a1/docs/guides/overview.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/guides/pyproject-configuration.rst` & `documenteer-1.0.0a1/docs/guides/pyproject-configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/guides/rst-epilog.rst` & `documenteer-1.0.0a1/docs/guides/rst-epilog.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/guides/tabsets.rst` & `documenteer-1.0.0a1/docs/guides/tabsets.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/guides/toml-reference.rst` & `documenteer-1.0.0a1/docs/guides/toml-reference.rst`

 * *Files 16% similar despite different names*

```diff
@@ -83,14 +83,101 @@
 version
 -------
 
 |optional| |py-auto|
 
 The project's version, which is set to the standard Sphinx ``version`` and ``release`` configuration variables.
 
+.. _guide-project-openapi:
+
+[project.openapi]
+=================
+
+|optional|
+
+Web applications that use OpenAPI can include a ``[project.openapi]`` table in :file:`documenteer.toml` to embed a Redoc_ subsite of the API documentation (see :doc:`openapi`).
+
+.. _guide-project-openapi-doc-path:
+
+doc\_path
+---------
+
+|optional|
+
+The docname (without extension) of the page in the Sphinx documentation tree where the Redoc HTML page is built.
+Default is ``api``.
+
+.. _guide-project-openapi-openapi-path:
+
+openapi\_path
+-------------
+
+|optional|
+
+The path to the OpenAPI specification file, relative to the Sphinx configuration file, :file:`conf.py`.
+If ``[project.openapi.generator]`` is set, this is the path where the OpenAPI specification file is generated.
+
+.. _guide-project-openapi-generator:
+
+[project.openapi.generator]
+===========================
+
+|optional|
+
+If this table is provided, the OpenAPI specification file is generated from a user-specified Python function.
+This is useful for FastAPI and similar applications where the OpenAPI specification is generated from the application code.
+
+.. _guide-project-openapi-generator-function:
+
+function
+--------
+
+|required|
+
+The Python function that generates the OpenAPI specification file.
+This function must return the OpenAPI specification as a JSON-serialized string.
+
+Specify the function as ``<module>:<function>``.
+For example, if the function called ``create_openapi`` is in the :file:`main.py` module of the :file:`example` package, the value would be ``"example.main:create_openapi"``.
+
+.. code-block:: toml
+
+   [project.openapi.generator]
+   function = "example.main:create_openapi"
+
+.. _guide-project-openapi-generator-positional-args:
+
+positional\_args
+----------------
+
+|optional|
+
+Positional arguments to pass to the function, if required.
+
+.. code-block:: toml
+
+   [project.openapi.generator]
+   function = "example.main:create_openapi"
+   positional_args = ["arg1", "arg2"]
+
+.. _guide-project-openapi-generator-keyword-args:
+
+keyword\_args
+-------------
+
+|optional|
+
+Keyword arguments to pass to the function, if required.
+
+.. code-block:: toml
+
+   [project.openapi.generator]
+   function = "example.main:create_openapi"
+   keyword_args = {kwarg1 = "value1", kwarg2 = "value2"}
+
 [project.python]
 ================
 
 |optional|
 
 Projects that use a :file:`pyproject.toml` to set their build metadata can include a ``[project.python]`` table in :file:`documenteer.toml`.
 With this, many metadata values are automatically detected — look for |py-auto| badges above.
@@ -161,14 +248,23 @@
    ]
 
 .. note::
 
    This configuration is for the **primary** sidebar, on the left side, containing side or section-level navigation links.
    To remove the page-level contents sidebar, on the right side, add ``:html_theme.sidebar_secondary.remove:`` to the *page's* file metadata.
 
+exclude
+-------
+
+|optional|
+
+A list of file paths, relative to :file:`conf.py`, to exclude from the Sphinx build.
+This configuration is often used to prevent file unrelated to the documentation from being accidentally included in the site build.
+|documenteer.conf.guide| includes common files and directories, so you may not need to modify this configuration in standard situations.
+
 extensions
 ----------
 
 |optional|
 
 A list of Sphinx extensions to append to the extensions included in the Documenteer configuration preset (see |documenteer.conf.guide|).
 Duplicate extensions are ignored.
```

### Comparing `documenteer-0.8.1/docs/index.rst` & `documenteer-1.0.0a1/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 ###########
 Documenteer
 ###########
 
 **Sphinx extensions, configurations, and tooling for Rubin Observatory documentation projects.**
 
-This documentation is for version |version|. `Find docs for other versions. <https://documenteer.lsst.io/v>`__
 Documenteer is developed on GitHub at https://github.com/lsst-sqre/documenteer.
+Find other versions of the documentation at https://documenteer.lsst.io/v
 
 .. _pip-install:
 .. _installation:
 
 Installation
 ============
```

### Comparing `documenteer-0.8.1/docs/pipelines/build-overview.rst` & `documenteer-1.0.0a1/docs/pipelines/build-overview.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/pipelines/configuration.rst` & `documenteer-1.0.0a1/docs/pipelines/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/pipelines/cpp-api-linking.rst` & `documenteer-1.0.0a1/docs/pipelines/cpp-api-linking.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/pipelines/index.rst` & `documenteer-1.0.0a1/docs/pipelines/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/pipelines/install.rst` & `documenteer-1.0.0a1/docs/pipelines/install.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/pipelines/package-docs-cli.rst` & `documenteer-1.0.0a1/docs/pipelines/package-docs-cli.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/pipelines/stack-docs-cli.rst` & `documenteer-1.0.0a1/docs/pipelines/stack-docs-cli.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/sphinx-extensions/autocppapi.rst` & `documenteer-1.0.0a1/docs/sphinx-extensions/autocppapi.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/sphinx-extensions/autodocreset.rst` & `documenteer-1.0.0a1/docs/sphinx-extensions/autodocreset.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/sphinx-extensions/docushare-reference.rst` & `documenteer-1.0.0a1/docs/sphinx-extensions/docushare-reference.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/sphinx-extensions/jira-reference.rst` & `documenteer-1.0.0a1/docs/sphinx-extensions/jira-reference.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/sphinx-extensions/lsst-pybtex-style.rst` & `documenteer-1.0.0a1/docs/sphinx-extensions/lsst-pybtex-style.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/sphinx-extensions/lssttasks.rst` & `documenteer-1.0.0a1/docs/sphinx-extensions/lssttasks.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/sphinx-extensions/package-toctree.rst` & `documenteer-1.0.0a1/docs/sphinx-extensions/package-toctree.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/sphinx-extensions/remote-code-block.rst` & `documenteer-1.0.0a1/docs/sphinx-extensions/remote-code-block.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/technotes/configuration.rst` & `documenteer-1.0.0a1/docs/technotes/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/technotes/index.rst` & `documenteer-1.0.0a1/docs/technotes/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/docs/technotes/refresh-lsst-bib.rst` & `documenteer-1.0.0a1/docs/technotes/refresh-lsst-bib.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/licenses/astropy-helpers.txt` & `documenteer-1.0.0a1/licenses/astropy-helpers.txt`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/licenses/sphinx-issue.txt` & `documenteer-1.0.0a1/licenses/sphinx-issue.txt`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/licenses/sphinx.txt` & `documenteer-1.0.0a1/licenses/sphinx.txt`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/pyproject.toml` & `documenteer-1.0.0a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 [project]
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 name = "documenteer"
 description = "Rubin Observatory / LSST Sphinx documentation tools, extensions, and configurations."
-license = {file = "LICENSE"}
+license = { file = "LICENSE" }
 readme = "README.md"
-keywords = [
-    "rubin",
-    "lsst",
-]
+keywords = ["rubin", "lsst"]
 # https://pypi.org/classifiers/
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Intended Audience :: Developers",
     "Topic :: Documentation",
     "Topic :: Documentation :: Sphinx",
     "Framework :: Sphinx :: Extension",
     "Environment :: Console",
     "Natural Language :: English",
     "Operating System :: POSIX",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dynamic = ["version"]
 dependencies = [
-    "Sphinx>=2.4.0",
+    "Sphinx",
     "PyYAML",
     "GitPython",
     "requests",
     "click",
-    "sphinxcontrib-bibtex>=2.0.0",  # for pybtex plugin; bibtex_bibfiles config is required.
+    "sphinxcontrib-bibtex>=2.0.0",                  # for pybtex plugin; bibtex_bibfiles config is required.
     "importlib_metadata; python_version < \"3.8\"",
     "tomli; python_version < \"3.11\"",
     "pydantic",
 ]
 
 [project.optional-dependencies]
 dev = [
@@ -60,33 +57,33 @@
     "types-docutils",
     "types-mock",
 ]
 guide = [
     # Theme and extensions for Rubin user guide projects
     "sphinx_design",
     "pydata-sphinx-theme>=0.10.0,<0.13.0",
-    "sphinx-autodoc-typehints<1.23.0",  # avoid requiring Sphinx > 7 only
+    "sphinx-autodoc-typehints",
     "sphinx-automodapi",
     "sphinx-copybutton",
     "sphinx-prompt",
     "myst-parser",
     "markdown-it-py[linkify]",
     "sphinxcontrib-mermaid",
     "sphinxext-opengraph",
+    "sphinxcontrib-redoc",
     "sphinxcontrib-jquery",
 ]
 technote = [
     # Theme and extensions for technotes
-    "sphinx<7.0.0",
     "lsst-dd-rtd-theme>=0.2.3,<0.3.0",
+    "technote>=0.2.0",
     "sphinx-prompt",
 ]
 pipelines = [
     # Theme and extensions for pipelines.lsst.io
-    "sphinx<7.0.0",
     "lsst-sphinx-bootstrap-theme>=0.2.0,<0.3.0",
     "numpydoc",
     "sphinx-automodapi",
     "sphinx-jinja",
     "sphinxcontrib-autoprogram",
     "sphinx-prompt",
     "sphinxcontrib-doxylink",
@@ -101,19 +98,15 @@
 [project.scripts]
 stack-docs = "documenteer.stackdocs.stackcli:main"
 package-docs = "documenteer.stackdocs.packagecli:main"
 build-stack-docs = "documenteer.bin.buildstackdocs:run_build_cli"
 refresh-lsst-bib = "documenteer.bin.refreshlsstbib:run"
 
 [build-system]
-requires = [
-    "setuptools>=61",
-    "wheel",
-    "setuptools_scm[toml]>=6.2"
-]
+requires = ["setuptools>=61", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = 'setuptools.build_meta'
 
 [tool.setuptools_scm]
 
 [tool.black]
 line-length = 79
 target-version = ['py38']
@@ -161,18 +154,15 @@
     "if TYPE_CHECKING:",
 ]
 
 [tool.pytest]
 norecursedirs = "node_modules"
 
 [tool.pytest.ini_options]
-python_files = [
-    "tests/*.py",
-    "tests/*/*.py"
-]
+python_files = ["tests/*.py", "tests/*/*.py"]
 
 [tool.mypy]
 # provisional config; disallow_untyped_defs once fully typed
 disallow_untyped_defs = false
 disallow_incomplete_defs = true
 ignore_missing_imports = true
 show_error_codes = true
```

### Comparing `documenteer-0.8.1/src/documenteer/assets/favicon.ico` & `documenteer-1.0.0a1/src/documenteer/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/assets/rubin-favicon-transparent-32px.png` & `documenteer-1.0.0a1/src/documenteer/assets/rubin-favicon-transparent-32px.png`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/assets/rubin-favicon.svg` & `documenteer-1.0.0a1/src/documenteer/assets/rubin-favicon.svg`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/assets/rubin-pydata-theme.css` & `documenteer-1.0.0a1/src/documenteer/assets/rubin-pydata-theme.css`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg` & `documenteer-1.0.0a1/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/assets/rubin-titlebar-imagotype-light.svg` & `documenteer-1.0.0a1/src/documenteer/assets/rubin-titlebar-imagotype-light.svg`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/bin/buildstackdocs.py` & `documenteer-1.0.0a1/src/documenteer/bin/buildstackdocs.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/bin/refreshlsstbib.py` & `documenteer-1.0.0a1/src/documenteer/bin/refreshlsstbib.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/conf/_toml.py` & `documenteer-1.0.0a1/src/documenteer/conf/_toml.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,15 +41,79 @@
     ValidationError,
     validator,
 )
 from sphinx.errors import ConfigError
 
 from ._utils import GitRepository
 
-__all__ = ["ProjectModel", "ConfigRoot", "DocumenteerConfig"]
+__all__ = [
+    "ConfigRoot",
+    "DocumenteerConfig",
+    "ProjectModel",
+    "PythonPackageModel",
+    "OpenApiDocsModel",
+    "OpenApiGeneratorModel",
+    "SphinxModel",
+    "IntersphinxModel",
+    "LinkCheckModel",
+    "ThemeModel",
+]
+
+
+class OpenApiGeneratorModel(BaseModel):
+    """Specification for the OpenAPI generator function used by the
+    ``documenteer.ext.openapi`` Sphinx extension.
+    """
+
+    function: str = Field(
+        description=(
+            "The Python function that generates the OpenAPI spec file. "
+            "It must have the form ``module:func``. The function must return "
+            "a JSON-serialized string."
+        )
+    )
+
+    positional_args: List[Any] = Field(
+        default_factory=list,
+        description=(
+            "Positional arguments to pass to the generator function."
+        ),
+    )
+
+    keyword_args: Dict[str, Any] = Field(
+        default_factory=dict,
+        description=("Keyword arguments to pass to the generator function."),
+    )
+
+
+class OpenApiDocsModel(BaseModel):
+    """Model for OpenAPI documentation configurations in documenteer.toml."""
+
+    generator: Optional[OpenApiGeneratorModel] = Field(
+        None,
+        description=(
+            "The function that generates the OpenAPI spec file from the"
+            "application source code. If not specified, the OpenAPI spec file "
+            "assumed to be generated by an external process and provided at "
+            "the path specified by ``openapi_path``."
+        ),
+    )
+
+    openapi_path: str = Field(
+        "_static/openapi.json",
+        description=(
+            "This is the path, relative to the Sphinx conf.py file, where the "
+            "OpenAPI spec file is written. Default is "
+            "``_static/openapi.json``."
+        ),
+    )
+
+    doc_path: str = Field(
+        "api",
+    )
 
 
 class PythonPackageModel(BaseModel):
     """Model for a Python package (i.e. built with pyproject.toml-compatible
     build system.
     """
 
@@ -110,15 +174,17 @@
     github_default_branch: str = Field(
         "main",
         description="The project's default development branch on GitHub.",
     )
 
     version: Optional[str] = Field(description="Version string.")
 
-    python: Optional[PythonPackageModel]
+    python: Optional[PythonPackageModel] = Field(None)
+
+    openapi: Optional[OpenApiDocsModel] = Field(None)
 
 
 class IntersphinxModel(BaseModel):
     """Model for Intersphinx configurations in documenteer.toml."""
 
     projects: Dict[str, HttpUrl] = Field(
         description="Mapping of projects and their URLs.", default_factory=dict
@@ -198,14 +264,22 @@
         None,
         description=(
             "Directory path where the Python API reference documentation "
             "is created."
         ),
     )
 
+    exclude: List[str] = Field(
+        description=(
+            "List of paths to exclude from being considered as Sphinx content "
+            "sources."
+        ),
+        default_factory=list,
+    )
+
     theme: ThemeModel = Field(default_factory=lambda: ThemeModel())
 
     intersphinx: Optional[IntersphinxModel]
 
     linkcheck: Optional[LinkCheckModel]
 
 
@@ -402,14 +476,21 @@
     @property
     def nitpicky(self) -> bool:
         if self.conf.sphinx:
             return self.conf.sphinx.nitpicky
         else:
             return False
 
+    def extend_exclude_patterns(self, exclude_patterns: List[str]) -> None:
+        """Extend Sphinx ``exclude_patterns`` with the "exclude" configuration
+        from the sphinx TOML table.
+        """
+        if self.conf.sphinx and self.conf.sphinx.exclude:
+            exclude_patterns.extend(self.conf.sphinx.exclude)
+
     def disable_primary_sidebars(
         self, html_sidebars: MutableMapping[str, List[str]]
     ) -> None:
         if self.conf.sphinx and self.conf.sphinx.disable_primary_sidebars:
             pages = self.conf.sphinx.disable_primary_sidebars
         else:
             pages = ["index"]  # default
```

### Comparing `documenteer-0.8.1/src/documenteer/conf/_utils.py` & `documenteer-1.0.0a1/src/documenteer/conf/_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/conf/guide.py` & `documenteer-1.0.0a1/src/documenteer/conf/guide.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 To use this configuration in a Sphinx technote project, write a conf.py
 containing::
 
     from documenteer.conf.guide import *
 """
 
-from typing import Any, Dict, List, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 from documenteer.conf import (
     DocumenteerConfig,
     get_asset_path,
     get_template_dir,
 )
 
@@ -30,14 +30,16 @@
 #     API reference configuration
 # #MYST
 #     MyST markdown configurations
 # #MERMIAID
 #     Mermaid diagram support
 # #OPENGRAPH
 #     OpenGraph metadata support
+# #OPENAPI
+#     OpenAPI/redoc support
 
 
 # Ordered as they are declared in this module
 __all__ = [
     # EXT
     "extensions",
     # SPHINX
@@ -98,14 +100,19 @@
     # MERMAID
     "mermaid_output_format",
     "mermaid_version",
     # OPENGRAPH
     "ogp_site_url",
     "ogp_site_name",
     "ogp_use_first_image",
+    # OPENAPI
+    "documenteer_openapi_generator",
+    "documenteer_openapi_path",
+    "redoc",
+    "redoc_uri",
 ]
 
 _conf = DocumenteerConfig.find_and_load()
 
 
 # ============================================================================
 # #EXT Sphinx extensions
@@ -120,19 +127,21 @@
     "sphinxext.opengraph",
     "sphinx.ext.autodoc",
     "sphinx.ext.doctest",
     "sphinx.ext.intersphinx",
     "sphinx.ext.todo",
     "sphinx.ext.ifconfig",
     "sphinx-prompt",
+    "sphinxcontrib.redoc",
     "sphinx.ext.napoleon",
     "sphinx_autodoc_typehints",
     "sphinx_automodapi.automodapi",
     "sphinx_automodapi.smart_resolver",
     "documenteer.sphinxext",
+    "documenteer.ext.openapi",
 ]
 _conf.append_extensions(extensions)
 
 # ============================================================================
 # #SPHINX Core Sphinx configurations
 # ============================================================================
 
@@ -163,14 +172,15 @@
     "README.md",
     ".venv",
     "venv",
     "requirements.txt",
     ".github",
     ".tox",
 ]
+_conf.extend_exclude_patterns(exclude_patterns)
 
 if _conf.rst_epilog_path:
     exclude_patterns.append(str(_conf.rst_epilog_path))
 
 # The reST default role cross-links Python (used for this markup: `text`)
 default_role = "py:obj"
 
@@ -368,7 +378,43 @@
 # https://github.com/wpilibsuite/sphinxext-opengraph
 # https://ogp.me/
 # ============================================================================
 
 ogp_site_url = _conf.base_url
 ogp_site_name = _conf.project
 ogp_use_first_image = True
+
+# ============================================================================
+# #OPEN OpenAPI/Redoc support
+# https://sphinxcontrib-redoc.readthedocs.io/en/stable/
+# documenteer.ext.openapi
+# ============================================================================
+
+if _conf.conf.project.openapi is not None:
+    if _conf.conf.project.openapi.generator is not None:
+        documenteer_openapi_generator: Optional[Dict[str, Any]] = {
+            "func": _conf.conf.project.openapi.generator.function,
+            "args": _conf.conf.project.openapi.generator.positional_args,
+            "kwargs": _conf.conf.project.openapi.generator.keyword_args,
+        }
+    else:
+        documenteer_openapi_generator = None
+    documenteer_openapi_path: Optional[
+        str
+    ] = _conf.conf.project.openapi.openapi_path
+    redoc: Optional[List[Any]] = [
+        {
+            "name": "REST API",
+            "page": _conf.conf.project.openapi.doc_path,
+            "spec": _conf.conf.project.openapi.openapi_path,
+            "embed": True,
+            "opts": {"hide-hostname": True},
+        }
+    ]
+    redoc_uri: Optional[
+        str
+    ] = "https://cdn.jsdelivr.net/npm/redoc@next/bundles/redoc.standalone.js"
+else:
+    documenteer_openapi_generator = None
+    documenteer_openapi_path = None
+    redoc = []
+    redoc_uri = None
```

### Comparing `documenteer-0.8.1/src/documenteer/conf/pipelines.py` & `documenteer-1.0.0a1/src/documenteer/conf/pipelines.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/conf/pipelinespkg.py` & `documenteer-1.0.0a1/src/documenteer/conf/pipelinespkg.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/conf/technote.py` & `documenteer-1.0.0a1/src/documenteer/conf/technote.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/ext/autocppapi.py` & `documenteer-1.0.0a1/src/documenteer/ext/autocppapi.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/ext/autodocreset.py` & `documenteer-1.0.0a1/src/documenteer/ext/autodocreset.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/packagemetadata.py` & `documenteer-1.0.0a1/src/documenteer/packagemetadata.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/requestsutils.py` & `documenteer-1.0.0a1/src/documenteer/requestsutils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/sphinxconfig/stackconf.py` & `documenteer-1.0.0a1/src/documenteer/sphinxconfig/stackconf.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/sphinxconfig/technoteconf.py` & `documenteer-1.0.0a1/src/documenteer/sphinxconfig/technoteconf.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/sphinxconfig/utils.py` & `documenteer-1.0.0a1/src/documenteer/sphinxconfig/utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/sphinxext/__init__.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/__init__.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/sphinxext/bibtex.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/bibtex.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/sphinxext/jira.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/jira.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/sphinxext/lsstdocushare.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/lsstdocushare.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/sphinxext/lssttasks/__init__.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/__init__.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/sphinxext/lssttasks/configfieldlists.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/configfieldlists.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/sphinxext/lssttasks/crossrefs.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/crossrefs.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/sphinxext/lssttasks/pyapisummary.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/pyapisummary.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/sphinxext/lssttasks/taskutils.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/taskutils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/sphinxext/lssttasks/topiclists.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/topiclists.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/sphinxext/lssttasks/topics.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/topics.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/sphinxext/mockcoderefs.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/mockcoderefs.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/sphinxext/packagetoctree.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/packagetoctree.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/sphinxext/remotecodeblock.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/remotecodeblock.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/sphinxext/utils.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/sphinxrunner.py` & `documenteer-1.0.0a1/src/documenteer/sphinxrunner.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,30 +11,25 @@
 __all__ = ["run_sphinx"]
 
 
 def run_sphinx(
     root_dir: Union[str, Path],
     job_count: int = 1,
     warnings_as_errors: bool = False,
-    nitpicky: bool = False,
 ) -> int:
     """Run the Sphinx build process.
 
     Parameters
     ----------
     root_dir : `str`
         Root directory of the Sphinx project and content source. This directory
         contains both the root ``index.rst`` file and the ``conf.py``
         configuration file.
     job_count : `int`
         Number of cores to run the Sphinx build with (``-j`` flag)
-    warnings_as_errors : `bool`
-        If ``True``, treat Sphinx warnings as errors (``-W`` flag).
-    nitpicky : `bool`
-        If ``True``, activate Sphinx's nitpicky mode (``-n`` flag).
 
     Returns
     -------
     status : `int`
         Sphinx status code. ``0`` is expected. Greater than ``0`` indicates
         an error.
 
@@ -52,16 +47,14 @@
         "-b",
         "html",
         "-d",
         os.path.join("_build", ".doctrees"),
     ]
     if warnings_as_errors:
         argv.append("-W")
-    if nitpicky:
-        argv.append("-n")
     argv.extend([src_dir, os.path.join("_build", "html")])
 
     start_dir = os.path.abspath(".")
     try:
         os.chdir(src_dir)
         status = build_main(argv=argv)
     finally:
```

### Comparing `documenteer-0.8.1/src/documenteer/stackdocs/build.py` & `documenteer-1.0.0a1/src/documenteer/stackdocs/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,14 @@
     prefer_doxygen_conf_in: bool = True,
     enable_doxygen_conf: bool = True,
     enable_doxygen: bool = True,
     enable_package_links: bool = True,
     enable_sphinx: bool = True,
     select_doxygen_packages: Optional[List[str]] = None,
     skip_doxygen_packages: Optional[List[str]] = None,
-    warning_is_error: bool = False,
-    nitpicky: bool = False,
 ) -> int:
     """Build stack Sphinx documentation (main entrypoint).
 
     Parameters
     ----------
     root_project_dir
         Path to the root directory of the main documentation project. This
@@ -75,19 +73,14 @@
     select_doxygen_packages
         If set, only EUPS packages named in this sequence will be processed by
         Doxygen. Packages still need to be set up and have ``doxygen.conf.in``
         files.
     skip_doxygen_packages
         If set, EUPS packages named in this sequence will be removed from the
         set of packages processed by Doxygen.
-    warning_is_error
-        If ``True``, warnings from Sphinx will be treated as errors.
-    nitpicky
-        If ``True``, run Sphinx in "nitpicky" mode that generates warnings
-        for more things like unresolved links.
 
     Returns
     -------
     sphinx_status : `int`
         The shell status code for the Sphinx build. If ``enable_sphinx`` is
         ``False``, the status defaults to ``0``.
     """
@@ -239,19 +232,15 @@
         else:
             # Write the doxygen configuration for debugging
             doxygen_conf_path = doxygen_build_dir / "doxygen.conf"
             doxygen_conf_path.write_text(doxygen_conf.render())
 
     # Trigger the Sphinx build
     if enable_sphinx:
-        return run_sphinx(
-            root_project_dir,
-            warnings_as_errors=warning_is_error,
-            nitpicky=nitpicky,
-        )
+        return run_sphinx(root_project_dir)
     else:
         return 0
 
 
 def link_directories(root_dir, package_doc_dirs):
     """Create symlinks to package/module documentation directories from the
     root documentation project.
```

### Comparing `documenteer-0.8.1/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml` & `documenteer-1.0.0a1/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/stackdocs/data/doxygen.defaults.conf` & `documenteer-1.0.0a1/src/documenteer/stackdocs/data/doxygen.defaults.conf`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/stackdocs/doxygen.py` & `documenteer-1.0.0a1/src/documenteer/stackdocs/doxygen.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/stackdocs/doxygentag.py` & `documenteer-1.0.0a1/src/documenteer/stackdocs/doxygentag.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/stackdocs/packagecli.py` & `documenteer-1.0.0a1/src/documenteer/stackdocs/packagecli.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 __all__ = ("main",)
 
 import logging
 import os
 import shutil
 import sys
-from typing import Any
 
 import click
 
 from ..sphinxrunner import run_sphinx
 from .rootdiscovery import discover_package_doc_dir
 
 # Add -h as a help shortcut option
@@ -60,15 +59,17 @@
 
     The key commands provided by package-docs are:
 
     - ``package-docs build``: compile the package's documentation.
     - ``package-docs clean``: removes documentation build products from a
       package.
     """
-    # Subcommands should use the click.pass_context decorator to get this
+    root_dir = discover_package_doc_dir(root_dir)
+
+    # Subcommands should use the click.pass_obj decorator to get this
     # ctx.obj object as the first argument.
     ctx.obj = {"root_dir": root_dir, "verbose": verbose}
 
     # Set up application logging. This ensures that only documenteer's
     # logger is activated. If necessary, we can add other app's loggers too.
     if verbose:
         log_level = logging.DEBUG
@@ -89,33 +90,22 @@
     if topic is None:
         click.echo(ctx.parent.get_help())
     else:
         click.echo(main.commands[topic].get_help(ctx))
 
 
 @main.command()
-@click.option(
-    "-W", "--warning-is-error", is_flag=True, help="Treat warnings as errors."
-)
-@click.option(
-    "-n", "--nitpicky", is_flag=True, help="Activate Sphinx's nitpicky mode."
-)
 @click.pass_context
-def build(ctx: Any, warning_is_error: bool, nitpicky: bool) -> None:
+def build(ctx):
     """Build documentation as HTML.
 
     The build HTML site is located in the ``doc/_build/html`` directory
     of the package.
     """
-    root_dir = discover_package_doc_dir(ctx["root_dir"])
-    return_code = run_sphinx(
-        root_dir,
-        warnings_as_errors=warning_is_error,
-        nitpicky=nitpicky,
-    )
+    return_code = run_sphinx(ctx.obj["root_dir"])
     if return_code > 0:
         sys.exit(return_code)
 
 
 @main.command()
 @click.pass_context
 def clean(ctx):
@@ -128,17 +118,17 @@
     directory:
 
     - ``_build`` (the Sphinx build itself)
     - ``py-api`` (pages created by automodapi for the Python API reference)
     """
     logger = logging.getLogger(__name__)
 
-    root_dir = discover_package_doc_dir(ctx["root_dir"])
-
     dirnames = ["py-api", "_build"]
-    dirnames = [os.path.join(root_dir, dirname) for dirname in dirnames]
+    dirnames = [
+        os.path.join(ctx.obj["root_dir"], dirname) for dirname in dirnames
+    ]
     for dirname in dirnames:
         if os.path.isdir(dirname):
             shutil.rmtree(dirname)
             logger.debug("Cleaned up %r", dirname)
         else:
             logger.debug("Did not clean up %r (missing)", dirname)
```

### Comparing `documenteer-0.8.1/src/documenteer/stackdocs/pkgdiscovery.py` & `documenteer-1.0.0a1/src/documenteer/stackdocs/pkgdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/stackdocs/rootdiscovery.py` & `documenteer-1.0.0a1/src/documenteer/stackdocs/rootdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/stackdocs/stackcli.py` & `documenteer-1.0.0a1/src/documenteer/stackdocs/stackcli.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,17 @@
       clear the build cache.
 
     See also: package-docs, a tool for building previews of package
     documentation.
 
     For more information about stack-docs, see https://documenteer.lsst.io.
     """
-    # Subcommands should use the click.pass_context decorator to get this
+    root_project_dir = discover_conf_py_directory(root_project_dir)
+
+    # Subcommands should use the click.pass_obj decorator to get this
     # ctx.obj object as the first argument.
     ctx.obj = {"root_project_dir": root_project_dir, "verbose": verbose}
 
     # Set up application logging. This ensures that only documenteer's
     # logger is activated. If necessary, we can add other app's loggers too.
     if verbose:
         log_level = logging.DEBUG
@@ -156,34 +158,26 @@
     ),
 )
 @click.option(
     "--skip-dox",
     multiple=True,
     help=("Skip running Doxygen on these packages."),
 )
-@click.option(
-    "-W", "--warning-is-error", is_flag=True, help="Treat warnings as errors."
-)
-@click.option(
-    "-n", "--nitpicky", is_flag=True, help="Activate Sphinx's nitpicky mode."
-)
 @click.pass_context
 def build(
     ctx,
     skip,
     enable_doxygen_conf,
     enable_doxygen,
     enable_symlinks,
     enable_sphinx,
     use_doxygen_conf_in,
     doxygen_conf_defaults_path,
     dox,
     skip_dox,
-    warning_is_error,
-    nitpicky,
 ):
     """Build documentation as HTML.
 
     This command performs these steps:
 
     1. Removes any existing symlinks in the ``modules``, ``packages``, and
        ``_static`` directories.
@@ -199,34 +193,30 @@
 
     By default, the build site is located in the ``_build/html`` directory
     of the ``pipelines_lsst_io`` repository.
 
     To peek inside the build process, see the ``documenteer.stackdocs.build``
     APIs.
     """
-    root_project_dir = discover_conf_py_directory(ctx.obj["root_project_dir"])
-
     if doxygen_conf_defaults_path is not None:
         _doxygen_conf_defaults_path = Path(doxygen_conf_defaults_path)
     else:
         _doxygen_conf_defaults_path = None
 
     return_code = build_stack_docs(
-        root_project_dir,
+        ctx.obj["root_project_dir"],
         skipped_names=skip,
         prefer_doxygen_conf_in=use_doxygen_conf_in,
         doxygen_conf_defaults_path=_doxygen_conf_defaults_path,
         enable_doxygen_conf=enable_doxygen_conf,
         enable_doxygen=enable_doxygen,
         enable_package_links=enable_symlinks,
         enable_sphinx=enable_sphinx,
         select_doxygen_packages=dox,
         skip_doxygen_packages=skip_dox,
-        warning_is_error=warning_is_error,
-        nitpicky=nitpicky,
     )
     if return_code > 0:
         sys.exit(return_code)
 
 
 @main.command()
 @click.pass_context
@@ -243,18 +233,18 @@
     - ``modules`` (symlinks to the module doc directories of Stack packages)
     - ``packages`` (symlinks to the package doc directories of Stack packages)
     - ``py-api`` (pages created by automodapi for the Python API reference)
     - ``_doxygen`` (the Doxygen build)
     """
     logger = logging.getLogger(__name__)
 
-    root_project_dir = discover_conf_py_directory(ctx.obj["root_project_dir"])
     dirnames = ["py-api", "_build", "modules", "packages", "_doxygen"]
     dirnames = [
-        os.path.join(root_project_dir, dirname) for dirname in dirnames
+        os.path.join(ctx.obj["root_project_dir"], dirname)
+        for dirname in dirnames
     ]
     for dirname in dirnames:
         if os.path.isdir(dirname):
             shutil.rmtree(dirname)
             logger.debug("Cleaned up %r", dirname)
         else:
             logger.debug("Did not clean up %r (missing)", dirname)
@@ -308,16 +298,17 @@
 
         :lsstcc:`{{name}}`
 
     Example usage::
 
         stack-docs listcc -t class -t function -p lsst::afw::table
     """
-    root_project_dir = discover_conf_py_directory(ctx.obj["root_project_dir"])
-    tag_path = os.path.join(root_project_dir, "_doxygen", "doxygen.tag")
+    tag_path = os.path.join(
+        ctx.obj["root_project_dir"], "_doxygen", "doxygen.tag"
+    )
 
     if pattern:
         p = re.compile(pattern)
 
     if not api_types:
         api_types = [
             "namespace",
```

### Comparing `documenteer-0.8.1/src/documenteer/utils.py` & `documenteer-1.0.0a1/src/documenteer/utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer/version.py` & `documenteer-1.0.0a1/src/documenteer/version.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/src/documenteer.egg-info/PKG-INFO` & `documenteer-1.0.0a1/src/documenteer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: documenteer
-Version: 0.8.1
+Version: 1.0.0a1
 Summary: Rubin Observatory / LSST Sphinx documentation tools, extensions, and configurations.
 License: The MIT License (MIT)
         
         Copyright (c) 2015-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -27,34 +27,34 @@
 Project-URL: Homepage, https://documenteer.lsst.io
 Project-URL: Source, https://github.com/lsst-sqre/documenteer
 Keywords: rubin,lsst
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: guide
 Provides-Extra: technote
 Provides-Extra: pipelines
 License-File: LICENSE
 
-[![Documentation](https://img.shields.io/badge/documenteer-lsst.io-brightgreen.svg)](https://documenteer.lsst.io)
+[![Documentation](https://img.shields.io/badge/documenteer-lsst.io-brightgreen.svg)](https://documentation.lsst.io)
 [![PyPI](https://img.shields.io/pypi/v/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![For Python 3.7+](https://img.shields.io/pypi/pyversions/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![MIT license](https://img.shields.io/pypi/l/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![CI](https://github.com/lsst-sqre/documenteer/actions/workflows/ci.yaml/badge.svg)](https://github.com/lsst-sqre/documenteer/actions/workflows/ci.yaml)
 [![Weekly CI](https://github.com/lsst-sqre/documenteer/actions/workflows/ci-cron.yaml/badge.svg)](https://github.com/lsst-sqre/documenteer/actions/workflows/ci-cron.yaml)
 
 # Documenteer
@@ -66,15 +66,15 @@
 Browse the [lsst-doc-engineering](https://github.com/topics/lsst-doc-engineering) GitHub topic for more Rubin Observatory documentation engineering projects.
 
 ## Quick installation:
 
 For [user guides](https://documenteer.lsst.io/guides/index.html):
 
 ```sh
-pip install "documenteer[guides]"
+pip install "documenteer[technote]"
 ```
 
 For [technical note projects](https://documenteer.lsst.io/technotes/index.html):
 
 ```sh
 pip install "documenteer[technote]"
 ```
```

### Comparing `documenteer-0.8.1/src/documenteer.egg-info/SOURCES.txt` & `documenteer-1.0.0a1/src/documenteer.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,65 @@
 .flake8
 .gitignore
+.npmrc
+.nvmrc
 .pre-commit-config.yaml
+.prettierignore
+.prettierrc.yaml
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
+package-lock.json
+package.json
+postcss.config.js
 pyproject.toml
 tox.ini
+webpack.config.js
 .github/CODE_OF_CONDUCT.md
 .github/CONTRIBUTING.md
 .github/SUPPORT.md
 .github/dependabot.yml
 .github/workflows/ci-cron.yaml
 .github/workflows/ci.yaml
+.vscode/tasks.json
+demo/rst-technote/.gitignore
+demo/rst-technote/Makefile
+demo/rst-technote/conf.py
+demo/rst-technote/index.rst
+demo/rst-technote/technote.toml
 docs/.gitignore
 docs/Makefile
 docs/_rst_epilog.rst
 docs/changelog.md
 docs/conf.py
 docs/documenteer.toml
 docs/index.rst
 docs/dev/development.rst
+docs/dev/html-templates.rst
 docs/dev/index.rst
 docs/dev/release.rst
+docs/dev/theme-assets.rst
+docs/dev/theme.rst
 docs/dev/api/documenteer.conf.rst
 docs/dev/api/documenteer.ext.rst
 docs/dev/api/documenteer.requestsutils.rst
 docs/dev/api/documenteer.sphinxconfig.rst
 docs/dev/api/documenteer.sphinxext.rst
 docs/dev/api/documenteer.sphinxrunner.rst
 docs/dev/api/documenteer.stackdocs.rst
 docs/dev/api/index.rst
 docs/guides/badges.rst
 docs/guides/configuration-preset.rst
 docs/guides/configuration.rst
 docs/guides/diagrams.rst
 docs/guides/extend-conf-py.rst
 docs/guides/index.rst
+docs/guides/openapi.rst
 docs/guides/organization.rst
 docs/guides/overview.rst
 docs/guides/pyproject-configuration.rst
 docs/guides/rst-epilog.rst
 docs/guides/tabsets.rst
 docs/guides/toml-reference.rst
 docs/pipelines/build-overview.rst
@@ -54,55 +72,71 @@
 docs/sphinx-extensions/autocppapi.rst
 docs/sphinx-extensions/autodocreset.rst
 docs/sphinx-extensions/docushare-reference.rst
 docs/sphinx-extensions/index.rst
 docs/sphinx-extensions/jira-reference.rst
 docs/sphinx-extensions/lsst-pybtex-style.rst
 docs/sphinx-extensions/lssttasks.rst
+docs/sphinx-extensions/openapi.rst
 docs/sphinx-extensions/package-toctree.rst
 docs/sphinx-extensions/remote-code-block.rst
 docs/technotes/configuration.rst
 docs/technotes/index.rst
 docs/technotes/refresh-lsst-bib.rst
 licenses/README.md
 licenses/astropy-helpers.txt
 licenses/sphinx-issue.txt
 licenses/sphinx.txt
+src/assets/rubin-technote/styles/_hacks.scss
+src/assets/rubin-technote/styles/_properties.scss
+src/assets/rubin-technote/styles/rubin-technote.scss
+src/assets/rubin-technote/styles/components/_global-breadcrumbs.scss
+src/assets/rubin-technote/styles/components/_index.scss
+src/assets/rubin-technote/styles/components/_version-info.scss
 src/documenteer/__init__.py
 src/documenteer/packagemetadata.py
 src/documenteer/py.typed
 src/documenteer/requestsutils.py
 src/documenteer/sphinxrunner.py
 src/documenteer/utils.py
 src/documenteer/version.py
 src/documenteer.egg-info/PKG-INFO
 src/documenteer.egg-info/SOURCES.txt
 src/documenteer.egg-info/dependency_links.txt
 src/documenteer.egg-info/entry_points.txt
 src/documenteer.egg-info/requires.txt
 src/documenteer.egg-info/top_level.txt
+src/documenteer/assets/.gitignore
 src/documenteer/assets/favicon.ico
 src/documenteer/assets/rubin-favicon-transparent-32px.png
 src/documenteer/assets/rubin-favicon.svg
 src/documenteer/assets/rubin-pydata-theme.css
 src/documenteer/assets/rubin-titlebar-imagotype-dark.svg
 src/documenteer/assets/rubin-titlebar-imagotype-light.svg
+src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg
+src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg
+src/documenteer/assets/scripts/rubin-technote.js
+src/documenteer/assets/scripts/rubin-technote.js.map
+src/documenteer/assets/styles/rubin-technote.css
+src/documenteer/assets/styles/rubin-technote.css.map
 src/documenteer/bin/__init__.py
 src/documenteer/bin/buildstackdocs.py
 src/documenteer/bin/refreshlsstbib.py
 src/documenteer/conf/__init__.py
 src/documenteer/conf/_toml.py
 src/documenteer/conf/_utils.py
 src/documenteer/conf/guide.py
 src/documenteer/conf/pipelines.py
 src/documenteer/conf/pipelinespkg.py
 src/documenteer/conf/technote.py
+src/documenteer/conf/technotebeta.py
 src/documenteer/ext/__init__.py
 src/documenteer/ext/autocppapi.py
 src/documenteer/ext/autodocreset.py
+src/documenteer/ext/openapi.py
 src/documenteer/sphinxconfig/__init__.py
 src/documenteer/sphinxconfig/stackconf.py
 src/documenteer/sphinxconfig/technoteconf.py
 src/documenteer/sphinxconfig/utils.py
 src/documenteer/sphinxext/__init__.py
 src/documenteer/sphinxext/bibtex.py
 src/documenteer/sphinxext/jira.py
@@ -126,14 +160,19 @@
 src/documenteer/stackdocs/pkgdiscovery.py
 src/documenteer/stackdocs/rootdiscovery.py
 src/documenteer/stackdocs/stackcli.py
 src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml
 src/documenteer/stackdocs/data/doxygen.defaults.conf
 src/documenteer/stackdocs/data/mainpage.dox
 src/documenteer/templates/pydata/layout.html
+src/documenteer/templates/technote/.gitkeep
+src/documenteer/templates/technote/components/.gitkeep
+src/documenteer/templates/technote/sections/.gitkeep
+src/documenteer/templates/technote/sections/header-article.html
+src/documenteer/templates/technote/sections/sidebar-primary.html
 tests/conftest.py
 tests/test_conf_toml.py
 tests/test_conf_utils.py
 tests/test_ext_autocppapi.py
 tests/test_packagemetadata.py
 tests/test_refreshlsstbib.py
 tests/test_sphinxconfig_stackconf.py
```

### Comparing `documenteer-0.8.1/src/documenteer.egg-info/requires.txt` & `documenteer-1.0.0a1/src/documenteer.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Sphinx>=2.4.0
+Sphinx
 PyYAML
 GitPython
 requests
 click
 sphinxcontrib-bibtex>=2.0.0
 pydantic
 
@@ -26,33 +26,33 @@
 types-PyYAML
 types-docutils
 types-mock
 
 [guide]
 sphinx_design
 pydata-sphinx-theme<0.13.0,>=0.10.0
-sphinx-autodoc-typehints<1.23.0
+sphinx-autodoc-typehints
 sphinx-automodapi
 sphinx-copybutton
 sphinx-prompt
 myst-parser
 markdown-it-py[linkify]
 sphinxcontrib-mermaid
 sphinxext-opengraph
+sphinxcontrib-redoc
 sphinxcontrib-jquery
 
 [pipelines]
-sphinx<7.0.0
 lsst-sphinx-bootstrap-theme<0.3.0,>=0.2.0
 numpydoc
 sphinx-automodapi
 sphinx-jinja
 sphinxcontrib-autoprogram
 sphinx-prompt
 sphinxcontrib-doxylink
 sphinx-click
 sphinxcontrib-jquery
 
 [technote]
-sphinx<7.0.0
 lsst-dd-rtd-theme<0.3.0,>=0.2.3
+technote>=0.2.0
 sphinx-prompt
```

### Comparing `documenteer-0.8.1/tests/conftest.py` & `documenteer-1.0.0a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/data/afw.doxygen.conf` & `documenteer-1.0.0a1/tests/data/afw.doxygen.conf`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/data/doxygen.tag.zip` & `documenteer-1.0.0a1/tests/data/doxygen.tag.zip`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/roots/test-autocppapi/conf.py` & `documenteer-1.0.0a1/tests/roots/test-autocppapi/conf.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/roots/test-autocppapi/doxygen.tag.zip` & `documenteer-1.0.0a1/tests/roots/test-autocppapi/doxygen.tag.zip`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/test_conf_toml.py` & `documenteer-1.0.0a1/tests/test_conf_toml.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/test_conf_utils.py` & `documenteer-1.0.0a1/tests/test_conf_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/test_ext_autocppapi.py` & `documenteer-1.0.0a1/tests/test_ext_autocppapi.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/test_packagemetadata.py` & `documenteer-1.0.0a1/tests/test_packagemetadata.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/test_refreshlsstbib.py` & `documenteer-1.0.0a1/tests/test_refreshlsstbib.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/test_sphinxconfig_stackconf.py` & `documenteer-1.0.0a1/tests/test_sphinxconfig_stackconf.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/test_sphinxconfig_utils.py` & `documenteer-1.0.0a1/tests/test_sphinxconfig_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/test_sphinxext_jira.py` & `documenteer-1.0.0a1/tests/test_sphinxext_jira.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/test_sphinxext_lsstdocushare.py` & `documenteer-1.0.0a1/tests/test_sphinxext_lsstdocushare.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/test_sphinxext_lssttasks_taskutils.py` & `documenteer-1.0.0a1/tests/test_sphinxext_lssttasks_taskutils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/test_sphinxext_mockcoderefs.py` & `documenteer-1.0.0a1/tests/test_sphinxext_mockcoderefs.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/test_sphinxext_packagetoctree.py` & `documenteer-1.0.0a1/tests/test_sphinxext_packagetoctree.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/test_sphinxext_utils.py` & `documenteer-1.0.0a1/tests/test_sphinxext_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/test_stackdocs_build.py` & `documenteer-1.0.0a1/tests/test_stackdocs_build.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/test_stackdocs_doxygen.py` & `documenteer-1.0.0a1/tests/test_stackdocs_doxygen.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/test_stackdocs_doxygentag.py` & `documenteer-1.0.0a1/tests/test_stackdocs_doxygentag.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/test_stackdocs_pkgdiscovery.py` & `documenteer-1.0.0a1/tests/test_stackdocs_pkgdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/test_stackdocs_rootdiscovery.py` & `documenteer-1.0.0a1/tests/test_stackdocs_rootdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.1/tests/test_technoteconf.py` & `documenteer-1.0.0a1/tests/test_technoteconf.py`

 * *Files identical despite different names*

