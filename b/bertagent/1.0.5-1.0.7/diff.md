# Comparing `tmp/bertagent-1.0.5.tar.gz` & `tmp/bertagent-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bertagent-1.0.5.tar", last modified: Tue Jun 27 09:02:59 2023, max compression
+gzip compressed data, was "bertagent-1.0.7.tar", last modified: Tue Jun 27 09:40:13 2023, max compression
```

## Comparing `bertagent-1.0.5.tar` & `bertagent-1.0.7.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/
--rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-22 00:59:01.000000 bertagent-1.0.5/.editorconfig
--rw-------   0 jiko      (1000) jiko      (1000)       35 2023-05-22 00:59:02.000000 bertagent-1.0.5/.gitattributes
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.119155 bertagent-1.0.5/.github/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.119155 bertagent-1.0.5/.github/ISSUE_TEMPLATE/
--rw-------   0 jiko      (1000) jiko      (1000)      348 2023-05-22 00:59:02.000000 bertagent-1.0.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-------   0 jiko      (1000) jiko      (1000)      360 2023-05-22 00:59:02.000000 bertagent-1.0.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-------   0 jiko      (1000) jiko      (1000)      446 2023-05-22 00:59:02.000000 bertagent-1.0.5/.github/PULL_REQUEST_TEMPLATE.md
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/.github/workflows/
--rw-------   0 jiko      (1000) jiko      (1000)     1031 2023-05-22 00:59:02.000000 bertagent-1.0.5/.github/workflows/build-main.yml
--rw-------   0 jiko      (1000) jiko      (1000)     1217 2023-05-22 00:59:01.000000 bertagent-1.0.5/.gitignore
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      716 2023-05-05 19:23:38.000000 bertagent-1.0.5/.readthedocs.yaml
--rw-------   0 jiko      (1000) jiko      (1000)      126 2023-06-16 10:58:03.000000 bertagent-1.0.5/AUTHORS.rst
--rw-------   0 jiko      (1000) jiko      (1000)     3538 2023-05-22 00:59:01.000000 bertagent-1.0.5/CONTRIBUTING.rst
--rw-------   0 jiko      (1000) jiko      (1000)       89 2023-05-22 00:59:01.000000 bertagent-1.0.5/HISTORY.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1555 2023-05-22 00:59:01.000000 bertagent-1.0.5/LICENSE
--rw-------   0 jiko      (1000) jiko      (1000)      379 2023-05-22 00:59:01.000000 bertagent-1.0.5/MANIFEST.in
--rw-------   0 jiko      (1000) jiko      (1000)     3205 2023-05-22 00:59:01.000000 bertagent-1.0.5/Makefile
--rw-------   0 jiko      (1000) jiko      (1000)     2481 2023-06-27 09:02:59.123155 bertagent-1.0.5/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)     1472 2023-06-27 09:02:11.000000 bertagent-1.0.5/README.rst
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/bertagent/
--rw-------   0 jiko      (1000) jiko      (1000)      496 2023-05-22 23:08:30.000000 bertagent-1.0.5/bertagent/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)      497 2023-06-27 09:02:59.123155 bertagent-1.0.5/bertagent/_version.py
--rw-------   0 jiko      (1000) jiko      (1000)     9444 2023-06-06 04:18:16.000000 bertagent-1.0.5/bertagent/bertagent.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/bertagent/cli/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.0.5/bertagent/cli/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)      467 2023-05-22 00:59:02.000000 bertagent-1.0.5/bertagent/cli/bertagent.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/bertagent/data/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.0.5/bertagent/data/.gitkeep
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/bertagent/data/emacs-logo/
--rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-22 00:59:02.000000 bertagent-1.0.5/bertagent/data/emacs-logo/emacs-128x128.png
--rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-22 00:59:02.000000 bertagent-1.0.5/bertagent/data/emacs-logo/emacs.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/bertagent/tests/
--rw-------   0 jiko      (1000) jiko      (1000)       39 2023-05-22 00:59:02.000000 bertagent-1.0.5/bertagent/tests/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)      572 2023-05-22 00:59:02.000000 bertagent-1.0.5/bertagent/tests/test_bertagent.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/bertagent.egg-info/
--rw-------   0 jiko      (1000) jiko      (1000)     2481 2023-06-27 09:02:58.000000 bertagent-1.0.5/bertagent.egg-info/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)     1547 2023-06-27 09:02:59.000000 bertagent-1.0.5/bertagent.egg-info/SOURCES.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-06-27 09:02:58.000000 bertagent-1.0.5/bertagent.egg-info/dependency_links.txt
--rw-------   0 jiko      (1000) jiko      (1000)       59 2023-06-27 09:02:58.000000 bertagent-1.0.5/bertagent.egg-info/entry_points.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-06-27 09:02:58.000000 bertagent-1.0.5/bertagent.egg-info/not-zip-safe
--rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-06-27 09:02:58.000000 bertagent-1.0.5/bertagent.egg-info/requires.txt
--rw-------   0 jiko      (1000) jiko      (1000)       10 2023-06-27 09:02:58.000000 bertagent-1.0.5/bertagent.egg-info/top_level.txt
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/docs/
--rw-------   0 jiko      (1000) jiko      (1000)      618 2023-05-22 01:41:44.000000 bertagent-1.0.5/docs/Makefile
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.119155 bertagent-1.0.5/docs/build/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.119155 bertagent-1.0.5/docs/build/html/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/docs/build/html/_static/
--rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-04 17:45:22.000000 bertagent-1.0.5/docs/build/html/_static/check-solid.svg
--rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-04 17:45:22.000000 bertagent-1.0.5/docs/build/html/_static/copy-button.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.119155 bertagent-1.0.5/docs/build/html/_static/css/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/docs/build/html/_static/css/fonts/
--rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-04 17:45:23.000000 bertagent-1.0.5/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-04 17:45:09.000000 bertagent-1.0.5/docs/build/html/_static/file.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 bertagent-1.0.5/docs/build/html/_static/minus.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 bertagent-1.0.5/docs/build/html/_static/plus.png
--rw-------   0 jiko      (1000) jiko      (1000)      643 2023-05-22 23:22:16.000000 bertagent-1.0.5/docs/requirements.txt
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/docs/source/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/docs/source/_static/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.0.5/docs/source/_static/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-22 00:59:02.000000 bertagent-1.0.5/docs/source/authors.rst
--rw-------   0 jiko      (1000) jiko      (1000)      394 2023-06-27 08:53:54.000000 bertagent-1.0.5/docs/source/bertagent.rst
--rw-------   0 jiko      (1000) jiko      (1000)      372 2023-06-27 08:53:54.000000 bertagent-1.0.5/docs/source/bertagent.tests.rst
--rwx------   0 jiko      (1000) jiko      (1000)     5960 2023-05-24 14:35:18.000000 bertagent-1.0.5/docs/source/conf.py
--rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-22 00:59:02.000000 bertagent-1.0.5/docs/source/contributing.rst
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-22 00:59:02.000000 bertagent-1.0.5/docs/source/history.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1001 2023-06-27 08:28:30.000000 bertagent-1.0.5/docs/source/index.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1134 2023-05-22 23:50:44.000000 bertagent-1.0.5/docs/source/installation.rst
--rw-------   0 jiko      (1000) jiko      (1000)       64 2023-06-27 08:53:54.000000 bertagent-1.0.5/docs/source/modules.rst
--rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-22 00:59:02.000000 bertagent-1.0.5/docs/source/readme.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1343 2023-06-27 08:35:15.000000 bertagent-1.0.5/docs/source/tutorial-01-input.csv
--rw-------   0 jiko      (1000) jiko      (1000)     2468 2023-06-27 08:48:33.000000 bertagent-1.0.5/docs/source/tutorial-02-output.csv
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     2729 2023-06-27 08:53:53.000000 bertagent-1.0.5/docs/source/tutorial.rst
--rw-------   0 jiko      (1000) jiko      (1000)      234 2023-05-22 23:48:49.000000 bertagent-1.0.5/docs/source/usage.rst
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      761 2023-05-22 00:59:01.000000 bertagent-1.0.5/pyproject.toml
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      517 2023-05-22 23:14:13.000000 bertagent-1.0.5/requirements_dev.txt
--rw-------   0 jiko      (1000) jiko      (1000)      588 2023-06-27 09:02:59.123155 bertagent-1.0.5/setup.cfg
--rw-------   0 jiko      (1000) jiko      (1000)     2664 2023-05-22 00:59:01.000000 bertagent-1.0.5/setup.py
--rw-------   0 jiko      (1000) jiko      (1000)      539 2023-05-22 00:59:01.000000 bertagent-1.0.5/tox.ini
--rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-22 00:59:02.000000 bertagent-1.0.5/versioneer.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/
+-rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-22 00:59:01.000000 bertagent-1.0.7/.editorconfig
+-rw-------   0 jiko      (1000) jiko      (1000)       35 2023-05-22 00:59:02.000000 bertagent-1.0.7/.gitattributes
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.153870 bertagent-1.0.7/.github/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.153870 bertagent-1.0.7/.github/ISSUE_TEMPLATE/
+-rw-------   0 jiko      (1000) jiko      (1000)      348 2023-05-22 00:59:02.000000 bertagent-1.0.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-------   0 jiko      (1000) jiko      (1000)      360 2023-05-22 00:59:02.000000 bertagent-1.0.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-------   0 jiko      (1000) jiko      (1000)      446 2023-05-22 00:59:02.000000 bertagent-1.0.7/.github/PULL_REQUEST_TEMPLATE.md
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.153870 bertagent-1.0.7/.github/workflows/
+-rw-------   0 jiko      (1000) jiko      (1000)     1031 2023-05-22 00:59:02.000000 bertagent-1.0.7/.github/workflows/build-main.yml
+-rw-------   0 jiko      (1000) jiko      (1000)     1217 2023-05-22 00:59:01.000000 bertagent-1.0.7/.gitignore
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      716 2023-05-05 19:23:38.000000 bertagent-1.0.7/.readthedocs.yaml
+-rw-------   0 jiko      (1000) jiko      (1000)      126 2023-06-16 10:58:03.000000 bertagent-1.0.7/AUTHORS.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     3538 2023-05-22 00:59:01.000000 bertagent-1.0.7/CONTRIBUTING.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       89 2023-05-22 00:59:01.000000 bertagent-1.0.7/HISTORY.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1555 2023-05-22 00:59:01.000000 bertagent-1.0.7/LICENSE
+-rw-------   0 jiko      (1000) jiko      (1000)      379 2023-05-22 00:59:01.000000 bertagent-1.0.7/MANIFEST.in
+-rw-------   0 jiko      (1000) jiko      (1000)     3205 2023-05-22 00:59:01.000000 bertagent-1.0.7/Makefile
+-rw-------   0 jiko      (1000) jiko      (1000)     2481 2023-06-27 09:40:13.157870 bertagent-1.0.7/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     1472 2023-06-27 09:02:11.000000 bertagent-1.0.7/README.rst
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/bertagent/
+-rw-------   0 jiko      (1000) jiko      (1000)      496 2023-05-22 23:08:30.000000 bertagent-1.0.7/bertagent/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)      497 2023-06-27 09:40:13.157870 bertagent-1.0.7/bertagent/_version.py
+-rw-------   0 jiko      (1000) jiko      (1000)     9444 2023-06-06 04:18:16.000000 bertagent-1.0.7/bertagent/bertagent.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/bertagent/cli/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.0.7/bertagent/cli/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)      467 2023-05-22 00:59:02.000000 bertagent-1.0.7/bertagent/cli/bertagent.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/bertagent/data/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.0.7/bertagent/data/.gitkeep
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/bertagent/data/emacs-logo/
+-rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-22 00:59:02.000000 bertagent-1.0.7/bertagent/data/emacs-logo/emacs-128x128.png
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-22 00:59:02.000000 bertagent-1.0.7/bertagent/data/emacs-logo/emacs.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/bertagent/tests/
+-rw-------   0 jiko      (1000) jiko      (1000)       39 2023-05-22 00:59:02.000000 bertagent-1.0.7/bertagent/tests/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)      572 2023-05-22 00:59:02.000000 bertagent-1.0.7/bertagent/tests/test_bertagent.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/bertagent.egg-info/
+-rw-------   0 jiko      (1000) jiko      (1000)     2481 2023-06-27 09:40:13.000000 bertagent-1.0.7/bertagent.egg-info/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     1547 2023-06-27 09:40:13.000000 bertagent-1.0.7/bertagent.egg-info/SOURCES.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-06-27 09:40:13.000000 bertagent-1.0.7/bertagent.egg-info/dependency_links.txt
+-rw-------   0 jiko      (1000) jiko      (1000)       59 2023-06-27 09:40:13.000000 bertagent-1.0.7/bertagent.egg-info/entry_points.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-06-27 09:40:13.000000 bertagent-1.0.7/bertagent.egg-info/not-zip-safe
+-rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-06-27 09:40:13.000000 bertagent-1.0.7/bertagent.egg-info/requires.txt
+-rw-------   0 jiko      (1000) jiko      (1000)       10 2023-06-27 09:40:13.000000 bertagent-1.0.7/bertagent.egg-info/top_level.txt
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/docs/
+-rw-------   0 jiko      (1000) jiko      (1000)      618 2023-05-22 01:41:44.000000 bertagent-1.0.7/docs/Makefile
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.153870 bertagent-1.0.7/docs/build/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.153870 bertagent-1.0.7/docs/build/html/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/docs/build/html/_static/
+-rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-04 17:45:22.000000 bertagent-1.0.7/docs/build/html/_static/check-solid.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-04 17:45:22.000000 bertagent-1.0.7/docs/build/html/_static/copy-button.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.153870 bertagent-1.0.7/docs/build/html/_static/css/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/docs/build/html/_static/css/fonts/
+-rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-04 17:45:23.000000 bertagent-1.0.7/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-04 17:45:09.000000 bertagent-1.0.7/docs/build/html/_static/file.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 bertagent-1.0.7/docs/build/html/_static/minus.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 bertagent-1.0.7/docs/build/html/_static/plus.png
+-rw-------   0 jiko      (1000) jiko      (1000)      643 2023-05-22 23:22:16.000000 bertagent-1.0.7/docs/requirements.txt
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/docs/source/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:40:13.157870 bertagent-1.0.7/docs/source/_static/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.0.7/docs/source/_static/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-22 00:59:02.000000 bertagent-1.0.7/docs/source/authors.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      394 2023-06-27 09:39:04.000000 bertagent-1.0.7/docs/source/bertagent.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      372 2023-06-27 09:39:04.000000 bertagent-1.0.7/docs/source/bertagent.tests.rst
+-rwx------   0 jiko      (1000) jiko      (1000)     5960 2023-05-24 14:35:18.000000 bertagent-1.0.7/docs/source/conf.py
+-rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-22 00:59:02.000000 bertagent-1.0.7/docs/source/contributing.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-22 00:59:02.000000 bertagent-1.0.7/docs/source/history.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1001 2023-06-27 08:28:30.000000 bertagent-1.0.7/docs/source/index.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1134 2023-05-22 23:50:44.000000 bertagent-1.0.7/docs/source/installation.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       64 2023-06-27 09:39:04.000000 bertagent-1.0.7/docs/source/modules.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-22 00:59:02.000000 bertagent-1.0.7/docs/source/readme.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1343 2023-06-27 08:35:15.000000 bertagent-1.0.7/docs/source/tutorial-01-input.csv
+-rw-------   0 jiko      (1000) jiko      (1000)     2468 2023-06-27 08:48:33.000000 bertagent-1.0.7/docs/source/tutorial-02-output.csv
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     3142 2023-06-27 09:38:36.000000 bertagent-1.0.7/docs/source/tutorial.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      234 2023-05-22 23:48:49.000000 bertagent-1.0.7/docs/source/usage.rst
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      761 2023-05-22 00:59:01.000000 bertagent-1.0.7/pyproject.toml
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      517 2023-05-22 23:14:13.000000 bertagent-1.0.7/requirements_dev.txt
+-rw-------   0 jiko      (1000) jiko      (1000)      588 2023-06-27 09:40:13.157870 bertagent-1.0.7/setup.cfg
+-rw-------   0 jiko      (1000) jiko      (1000)     2664 2023-05-22 00:59:01.000000 bertagent-1.0.7/setup.py
+-rw-------   0 jiko      (1000) jiko      (1000)      539 2023-05-22 00:59:01.000000 bertagent-1.0.7/tox.ini
+-rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-22 00:59:02.000000 bertagent-1.0.7/versioneer.py
```

### Comparing `bertagent-1.0.5/.github/workflows/build-main.yml` & `bertagent-1.0.7/.github/workflows/build-main.yml`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/.gitignore` & `bertagent-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/.readthedocs.yaml` & `bertagent-1.0.7/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/CONTRIBUTING.rst` & `bertagent-1.0.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/LICENSE` & `bertagent-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/Makefile` & `bertagent-1.0.7/Makefile`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/PKG-INFO` & `bertagent-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bertagent
-Version: 1.0.5
+Version: 1.0.7
 Summary: Quantify linguistic agency in textual data.
 Home-page: https://github.com/cogsys-io/bertagent
 Author: cogsys.io
 Author-email: bertagent@cogsys.io
 License: GNU General Public License v3
 Keywords: bertagent
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bertagent-1.0.5/README.rst` & `bertagent-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/bertagent/bertagent.py` & `bertagent-1.0.7/bertagent/bertagent.py`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/bertagent/data/emacs-logo/emacs-128x128.png` & `bertagent-1.0.7/bertagent/data/emacs-logo/emacs-128x128.png`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/bertagent/data/emacs-logo/emacs.svg` & `bertagent-1.0.7/bertagent/data/emacs-logo/emacs.svg`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/bertagent/tests/test_bertagent.py` & `bertagent-1.0.7/bertagent/tests/test_bertagent.py`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/bertagent.egg-info/PKG-INFO` & `bertagent-1.0.7/bertagent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bertagent
-Version: 1.0.5
+Version: 1.0.7
 Summary: Quantify linguistic agency in textual data.
 Home-page: https://github.com/cogsys-io/bertagent
 Author: cogsys.io
 Author-email: bertagent@cogsys.io
 License: GNU General Public License v3
 Keywords: bertagent
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bertagent-1.0.5/bertagent.egg-info/SOURCES.txt` & `bertagent-1.0.7/bertagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/bertagent.egg-info/requires.txt` & `bertagent-1.0.7/bertagent.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/docs/Makefile` & `bertagent-1.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `bertagent-1.0.7/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/docs/requirements.txt` & `bertagent-1.0.7/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/docs/source/conf.py` & `bertagent-1.0.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/docs/source/index.rst` & `bertagent-1.0.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/docs/source/installation.rst` & `bertagent-1.0.7/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/docs/source/tutorial-01-input.csv` & `bertagent-1.0.7/docs/source/tutorial-01-input.csv`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/docs/source/tutorial-02-output.csv` & `bertagent-1.0.7/docs/source/tutorial-02-output.csv`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/docs/source/tutorial.rst` & `bertagent-1.0.7/docs/source/tutorial.rst`

 * *Files 18% similar despite different names*

```diff
@@ -4,35 +4,49 @@
 Tutorial
 ========
 
 
 Process a list of sentences
 ---------------------------
 
+
+Imports
+
 .. code-block:: python
 
-    >>> # Imports
     >>> import pathlib
     >>> from bertagent import BERTAgent
-    >>>
-    >>> # Initialize BERTAgent
+
+Initialize BERTAgent
+
+.. code-block:: python
+
     >>> ba0 = BERTAgent()
-    >>>
-    >>> # Provide example sentences
+
+Provide example sentences
+
+.. code-block:: python
+
     >>> sents = [
     >>>     "stiving to achieve my goals",
     >>>     "struglling to survive",
     >>>     "hardly working individual",
     >>>     "hard working individual",
     >>> ]
-    >>>
-    >>> # Assign agency
+
+Assign agency
+
+.. code-block:: python
+
     >>> vals = ba0.predict(sents)
-    >>>
-    >>> # Pritnt results
+
+Print results
+
+.. code-block:: python
+
     >>> for item in zip(sents, vals):
     >>>     print(item)
     #
     # ('stiving to achieve my goals', 0.7477692365646362)
     # ('struglling to survive', 0.043704114854335785)
     # ('hardly working individual', -0.5707859396934509)
     # ('hard working individual', 0.43518713116645813)
@@ -46,65 +60,100 @@
 
 .. note::
    See in the example below we use
    ``EXAMPLE_SENTENCES`` data
    that is
    provided with ``BERTAgent``.
 
+Imports
 
 .. code-block:: python
 
-    >>> # Imports.
     >>> import pathlib
     >>> import pandas as pd
     >>> from tqdm import tqdm
     >>> from bertagent import BERTAgent
     >>> from bertagent import EXAMPLE_SENTENCES as sents
     >>> tqdm.pandas()
     >>>
-    >>> # Load BERTAgent.
+
+Load BERTAgent
+
+.. code-block:: python
+
     >>> ba0 = BERTAgent()
-    >>>
-    >>> # Prepare dataframe.
+
+Prepare dataframe.
+
+.. code-block:: python
+
     >>> df0 = pd.DataFrame(dict(text=sents))
-    >>>
-    >>> # Extract sentences from text.
+
+Extract sentences from text.
+
+.. code-block:: python
+
     >>> # NOTE: This is not an optimal method to get sentences from real data!
     >>> df0["sents"] = df0.text.str.split(".")
-    >>> # check input dataframe
+
+Check input dataframe
+
+.. code-block:: python
+
     >>> print(df0.head(n=4))
 
 
 .. csv-table:: Input data (pandas dataframe containing lists of sentences)
    :file: tutorial-01-input.csv
    :widths: 10, 90
    :header-rows: 1
 
 
+
+
+Evaluate agency
+
 .. code-block:: python
 
-    >>> # Evaluate agency
     >>> model_id = "ba0"
     >>> df0[model_id] = df0.sents.progress_apply(ba0.predict)
-    >>>
+
+Compute more specific indices of agency
+(``tot`` = total = sum af all values for all sentences,
+``pos`` = only positive,
+``neg`` = only negative,
+``abs`` = sum of absolute values)
+
+.. code-block:: python
+
     >>> df0["BATot"] = df0[model_id].apply(ba0.tot)
     >>> df0["BAPos"] = df0[model_id].apply(ba0.pos)
     >>> df0["BANeg"] = df0[model_id].apply(ba0.neg)
     >>> df0["BAAbs"] = df0[model_id].apply(ba0.abs)
     >>>
     >>> cols0 = [
     >>>     "sents",
     >>>     "ba0",
     >>>     "BATot",
     >>>     "BAPos",
     >>>     "BANeg",
     >>>     "BAAbs",
     >>> ]
     >>>
-    >>> # Check example rows.
+
+Check output
+
+.. code-block:: python
+
     >>> df0[cols0].tail(n=8)
 
 
 .. csv-table:: Output data (pandas dataframe with agency evaluation)
    :file: tutorial-02-output.csv
    :widths: 5, 70, 10, 10, 10, 10, 10
    :header-rows: 1
+
+
+.. note::
+   The last row demonstrates how a text that contains
+   multiple sentences is handled, each sentence is assigned a
+   separate agency score.
```

### Comparing `bertagent-1.0.5/pyproject.toml` & `bertagent-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/requirements_dev.txt` & `bertagent-1.0.7/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/setup.cfg` & `bertagent-1.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/setup.py` & `bertagent-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/tox.ini` & `bertagent-1.0.7/tox.ini`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.5/versioneer.py` & `bertagent-1.0.7/versioneer.py`

 * *Files identical despite different names*

