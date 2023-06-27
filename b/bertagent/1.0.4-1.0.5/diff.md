# Comparing `tmp/bertagent-1.0.4.tar.gz` & `tmp/bertagent-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bertagent-1.0.4.tar", last modified: Tue Jun 27 09:00:14 2023, max compression
+gzip compressed data, was "bertagent-1.0.5.tar", last modified: Tue Jun 27 09:02:59 2023, max compression
```

## Comparing `bertagent-1.0.4.tar` & `bertagent-1.0.5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:00:14.565899 bertagent-1.0.4/
--rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-22 00:59:01.000000 bertagent-1.0.4/.editorconfig
--rw-------   0 jiko      (1000) jiko      (1000)       35 2023-05-22 00:59:02.000000 bertagent-1.0.4/.gitattributes
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:00:14.561899 bertagent-1.0.4/.github/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:00:14.561899 bertagent-1.0.4/.github/ISSUE_TEMPLATE/
--rw-------   0 jiko      (1000) jiko      (1000)      348 2023-05-22 00:59:02.000000 bertagent-1.0.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-------   0 jiko      (1000) jiko      (1000)      360 2023-05-22 00:59:02.000000 bertagent-1.0.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-------   0 jiko      (1000) jiko      (1000)      446 2023-05-22 00:59:02.000000 bertagent-1.0.4/.github/PULL_REQUEST_TEMPLATE.md
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:00:14.565899 bertagent-1.0.4/.github/workflows/
--rw-------   0 jiko      (1000) jiko      (1000)     1031 2023-05-22 00:59:02.000000 bertagent-1.0.4/.github/workflows/build-main.yml
--rw-------   0 jiko      (1000) jiko      (1000)     1217 2023-05-22 00:59:01.000000 bertagent-1.0.4/.gitignore
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      716 2023-05-05 19:23:38.000000 bertagent-1.0.4/.readthedocs.yaml
--rw-------   0 jiko      (1000) jiko      (1000)      126 2023-06-16 10:58:03.000000 bertagent-1.0.4/AUTHORS.rst
--rw-------   0 jiko      (1000) jiko      (1000)     3538 2023-05-22 00:59:01.000000 bertagent-1.0.4/CONTRIBUTING.rst
--rw-------   0 jiko      (1000) jiko      (1000)       89 2023-05-22 00:59:01.000000 bertagent-1.0.4/HISTORY.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1555 2023-05-22 00:59:01.000000 bertagent-1.0.4/LICENSE
--rw-------   0 jiko      (1000) jiko      (1000)      379 2023-05-22 00:59:01.000000 bertagent-1.0.4/MANIFEST.in
--rw-------   0 jiko      (1000) jiko      (1000)     3205 2023-05-22 00:59:01.000000 bertagent-1.0.4/Makefile
--rw-------   0 jiko      (1000) jiko      (1000)     2384 2023-06-27 09:00:14.565899 bertagent-1.0.4/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)     1375 2023-05-22 23:49:08.000000 bertagent-1.0.4/README.rst
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:00:14.565899 bertagent-1.0.4/bertagent/
--rw-------   0 jiko      (1000) jiko      (1000)      496 2023-05-22 23:08:30.000000 bertagent-1.0.4/bertagent/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)      497 2023-06-27 09:00:14.565899 bertagent-1.0.4/bertagent/_version.py
--rw-------   0 jiko      (1000) jiko      (1000)     9444 2023-06-06 04:18:16.000000 bertagent-1.0.4/bertagent/bertagent.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:00:14.565899 bertagent-1.0.4/bertagent/cli/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.0.4/bertagent/cli/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)      467 2023-05-22 00:59:02.000000 bertagent-1.0.4/bertagent/cli/bertagent.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:00:14.565899 bertagent-1.0.4/bertagent/data/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.0.4/bertagent/data/.gitkeep
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:00:14.565899 bertagent-1.0.4/bertagent/data/emacs-logo/
--rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-22 00:59:02.000000 bertagent-1.0.4/bertagent/data/emacs-logo/emacs-128x128.png
--rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-22 00:59:02.000000 bertagent-1.0.4/bertagent/data/emacs-logo/emacs.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:00:14.565899 bertagent-1.0.4/bertagent/tests/
--rw-------   0 jiko      (1000) jiko      (1000)       39 2023-05-22 00:59:02.000000 bertagent-1.0.4/bertagent/tests/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)      572 2023-05-22 00:59:02.000000 bertagent-1.0.4/bertagent/tests/test_bertagent.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:00:14.565899 bertagent-1.0.4/bertagent.egg-info/
--rw-------   0 jiko      (1000) jiko      (1000)     2384 2023-06-27 09:00:14.000000 bertagent-1.0.4/bertagent.egg-info/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)     1547 2023-06-27 09:00:14.000000 bertagent-1.0.4/bertagent.egg-info/SOURCES.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-06-27 09:00:14.000000 bertagent-1.0.4/bertagent.egg-info/dependency_links.txt
--rw-------   0 jiko      (1000) jiko      (1000)       59 2023-06-27 09:00:14.000000 bertagent-1.0.4/bertagent.egg-info/entry_points.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-06-27 09:00:14.000000 bertagent-1.0.4/bertagent.egg-info/not-zip-safe
--rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-06-27 09:00:14.000000 bertagent-1.0.4/bertagent.egg-info/requires.txt
--rw-------   0 jiko      (1000) jiko      (1000)       10 2023-06-27 09:00:14.000000 bertagent-1.0.4/bertagent.egg-info/top_level.txt
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:00:14.565899 bertagent-1.0.4/docs/
--rw-------   0 jiko      (1000) jiko      (1000)      618 2023-05-22 01:41:44.000000 bertagent-1.0.4/docs/Makefile
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:00:14.561899 bertagent-1.0.4/docs/build/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:00:14.561899 bertagent-1.0.4/docs/build/html/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:00:14.565899 bertagent-1.0.4/docs/build/html/_static/
--rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-04 17:45:22.000000 bertagent-1.0.4/docs/build/html/_static/check-solid.svg
--rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-04 17:45:22.000000 bertagent-1.0.4/docs/build/html/_static/copy-button.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:00:14.561899 bertagent-1.0.4/docs/build/html/_static/css/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:00:14.565899 bertagent-1.0.4/docs/build/html/_static/css/fonts/
--rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-04 17:45:23.000000 bertagent-1.0.4/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-04 17:45:09.000000 bertagent-1.0.4/docs/build/html/_static/file.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 bertagent-1.0.4/docs/build/html/_static/minus.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 bertagent-1.0.4/docs/build/html/_static/plus.png
--rw-------   0 jiko      (1000) jiko      (1000)      643 2023-05-22 23:22:16.000000 bertagent-1.0.4/docs/requirements.txt
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:00:14.565899 bertagent-1.0.4/docs/source/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:00:14.565899 bertagent-1.0.4/docs/source/_static/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.0.4/docs/source/_static/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-22 00:59:02.000000 bertagent-1.0.4/docs/source/authors.rst
--rw-------   0 jiko      (1000) jiko      (1000)      394 2023-06-27 08:53:54.000000 bertagent-1.0.4/docs/source/bertagent.rst
--rw-------   0 jiko      (1000) jiko      (1000)      372 2023-06-27 08:53:54.000000 bertagent-1.0.4/docs/source/bertagent.tests.rst
--rwx------   0 jiko      (1000) jiko      (1000)     5960 2023-05-24 14:35:18.000000 bertagent-1.0.4/docs/source/conf.py
--rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-22 00:59:02.000000 bertagent-1.0.4/docs/source/contributing.rst
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-22 00:59:02.000000 bertagent-1.0.4/docs/source/history.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1001 2023-06-27 08:28:30.000000 bertagent-1.0.4/docs/source/index.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1134 2023-05-22 23:50:44.000000 bertagent-1.0.4/docs/source/installation.rst
--rw-------   0 jiko      (1000) jiko      (1000)       64 2023-06-27 08:53:54.000000 bertagent-1.0.4/docs/source/modules.rst
--rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-22 00:59:02.000000 bertagent-1.0.4/docs/source/readme.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1343 2023-06-27 08:35:15.000000 bertagent-1.0.4/docs/source/tutorial-01-input.csv
--rw-------   0 jiko      (1000) jiko      (1000)     2468 2023-06-27 08:48:33.000000 bertagent-1.0.4/docs/source/tutorial-02-output.csv
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     2729 2023-06-27 08:53:53.000000 bertagent-1.0.4/docs/source/tutorial.rst
--rw-------   0 jiko      (1000) jiko      (1000)      234 2023-05-22 23:48:49.000000 bertagent-1.0.4/docs/source/usage.rst
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      761 2023-05-22 00:59:01.000000 bertagent-1.0.4/pyproject.toml
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      517 2023-05-22 23:14:13.000000 bertagent-1.0.4/requirements_dev.txt
--rw-------   0 jiko      (1000) jiko      (1000)      588 2023-06-27 09:00:14.565899 bertagent-1.0.4/setup.cfg
--rw-------   0 jiko      (1000) jiko      (1000)     2664 2023-05-22 00:59:01.000000 bertagent-1.0.4/setup.py
--rw-------   0 jiko      (1000) jiko      (1000)      539 2023-05-22 00:59:01.000000 bertagent-1.0.4/tox.ini
--rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-22 00:59:02.000000 bertagent-1.0.4/versioneer.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/
+-rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-22 00:59:01.000000 bertagent-1.0.5/.editorconfig
+-rw-------   0 jiko      (1000) jiko      (1000)       35 2023-05-22 00:59:02.000000 bertagent-1.0.5/.gitattributes
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.119155 bertagent-1.0.5/.github/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.119155 bertagent-1.0.5/.github/ISSUE_TEMPLATE/
+-rw-------   0 jiko      (1000) jiko      (1000)      348 2023-05-22 00:59:02.000000 bertagent-1.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-------   0 jiko      (1000) jiko      (1000)      360 2023-05-22 00:59:02.000000 bertagent-1.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-------   0 jiko      (1000) jiko      (1000)      446 2023-05-22 00:59:02.000000 bertagent-1.0.5/.github/PULL_REQUEST_TEMPLATE.md
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/.github/workflows/
+-rw-------   0 jiko      (1000) jiko      (1000)     1031 2023-05-22 00:59:02.000000 bertagent-1.0.5/.github/workflows/build-main.yml
+-rw-------   0 jiko      (1000) jiko      (1000)     1217 2023-05-22 00:59:01.000000 bertagent-1.0.5/.gitignore
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      716 2023-05-05 19:23:38.000000 bertagent-1.0.5/.readthedocs.yaml
+-rw-------   0 jiko      (1000) jiko      (1000)      126 2023-06-16 10:58:03.000000 bertagent-1.0.5/AUTHORS.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     3538 2023-05-22 00:59:01.000000 bertagent-1.0.5/CONTRIBUTING.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       89 2023-05-22 00:59:01.000000 bertagent-1.0.5/HISTORY.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1555 2023-05-22 00:59:01.000000 bertagent-1.0.5/LICENSE
+-rw-------   0 jiko      (1000) jiko      (1000)      379 2023-05-22 00:59:01.000000 bertagent-1.0.5/MANIFEST.in
+-rw-------   0 jiko      (1000) jiko      (1000)     3205 2023-05-22 00:59:01.000000 bertagent-1.0.5/Makefile
+-rw-------   0 jiko      (1000) jiko      (1000)     2481 2023-06-27 09:02:59.123155 bertagent-1.0.5/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     1472 2023-06-27 09:02:11.000000 bertagent-1.0.5/README.rst
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/bertagent/
+-rw-------   0 jiko      (1000) jiko      (1000)      496 2023-05-22 23:08:30.000000 bertagent-1.0.5/bertagent/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)      497 2023-06-27 09:02:59.123155 bertagent-1.0.5/bertagent/_version.py
+-rw-------   0 jiko      (1000) jiko      (1000)     9444 2023-06-06 04:18:16.000000 bertagent-1.0.5/bertagent/bertagent.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/bertagent/cli/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.0.5/bertagent/cli/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)      467 2023-05-22 00:59:02.000000 bertagent-1.0.5/bertagent/cli/bertagent.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/bertagent/data/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.0.5/bertagent/data/.gitkeep
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/bertagent/data/emacs-logo/
+-rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-22 00:59:02.000000 bertagent-1.0.5/bertagent/data/emacs-logo/emacs-128x128.png
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-22 00:59:02.000000 bertagent-1.0.5/bertagent/data/emacs-logo/emacs.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/bertagent/tests/
+-rw-------   0 jiko      (1000) jiko      (1000)       39 2023-05-22 00:59:02.000000 bertagent-1.0.5/bertagent/tests/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)      572 2023-05-22 00:59:02.000000 bertagent-1.0.5/bertagent/tests/test_bertagent.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/bertagent.egg-info/
+-rw-------   0 jiko      (1000) jiko      (1000)     2481 2023-06-27 09:02:58.000000 bertagent-1.0.5/bertagent.egg-info/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     1547 2023-06-27 09:02:59.000000 bertagent-1.0.5/bertagent.egg-info/SOURCES.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-06-27 09:02:58.000000 bertagent-1.0.5/bertagent.egg-info/dependency_links.txt
+-rw-------   0 jiko      (1000) jiko      (1000)       59 2023-06-27 09:02:58.000000 bertagent-1.0.5/bertagent.egg-info/entry_points.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-06-27 09:02:58.000000 bertagent-1.0.5/bertagent.egg-info/not-zip-safe
+-rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-06-27 09:02:58.000000 bertagent-1.0.5/bertagent.egg-info/requires.txt
+-rw-------   0 jiko      (1000) jiko      (1000)       10 2023-06-27 09:02:58.000000 bertagent-1.0.5/bertagent.egg-info/top_level.txt
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/docs/
+-rw-------   0 jiko      (1000) jiko      (1000)      618 2023-05-22 01:41:44.000000 bertagent-1.0.5/docs/Makefile
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.119155 bertagent-1.0.5/docs/build/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.119155 bertagent-1.0.5/docs/build/html/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/docs/build/html/_static/
+-rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-04 17:45:22.000000 bertagent-1.0.5/docs/build/html/_static/check-solid.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-04 17:45:22.000000 bertagent-1.0.5/docs/build/html/_static/copy-button.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.119155 bertagent-1.0.5/docs/build/html/_static/css/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/docs/build/html/_static/css/fonts/
+-rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-04 17:45:23.000000 bertagent-1.0.5/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-04 17:45:09.000000 bertagent-1.0.5/docs/build/html/_static/file.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 bertagent-1.0.5/docs/build/html/_static/minus.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 bertagent-1.0.5/docs/build/html/_static/plus.png
+-rw-------   0 jiko      (1000) jiko      (1000)      643 2023-05-22 23:22:16.000000 bertagent-1.0.5/docs/requirements.txt
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/docs/source/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-06-27 09:02:59.123155 bertagent-1.0.5/docs/source/_static/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-22 00:59:02.000000 bertagent-1.0.5/docs/source/_static/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-22 00:59:02.000000 bertagent-1.0.5/docs/source/authors.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      394 2023-06-27 08:53:54.000000 bertagent-1.0.5/docs/source/bertagent.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      372 2023-06-27 08:53:54.000000 bertagent-1.0.5/docs/source/bertagent.tests.rst
+-rwx------   0 jiko      (1000) jiko      (1000)     5960 2023-05-24 14:35:18.000000 bertagent-1.0.5/docs/source/conf.py
+-rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-22 00:59:02.000000 bertagent-1.0.5/docs/source/contributing.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-22 00:59:02.000000 bertagent-1.0.5/docs/source/history.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1001 2023-06-27 08:28:30.000000 bertagent-1.0.5/docs/source/index.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1134 2023-05-22 23:50:44.000000 bertagent-1.0.5/docs/source/installation.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       64 2023-06-27 08:53:54.000000 bertagent-1.0.5/docs/source/modules.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-22 00:59:02.000000 bertagent-1.0.5/docs/source/readme.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1343 2023-06-27 08:35:15.000000 bertagent-1.0.5/docs/source/tutorial-01-input.csv
+-rw-------   0 jiko      (1000) jiko      (1000)     2468 2023-06-27 08:48:33.000000 bertagent-1.0.5/docs/source/tutorial-02-output.csv
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     2729 2023-06-27 08:53:53.000000 bertagent-1.0.5/docs/source/tutorial.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      234 2023-05-22 23:48:49.000000 bertagent-1.0.5/docs/source/usage.rst
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      761 2023-05-22 00:59:01.000000 bertagent-1.0.5/pyproject.toml
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      517 2023-05-22 23:14:13.000000 bertagent-1.0.5/requirements_dev.txt
+-rw-------   0 jiko      (1000) jiko      (1000)      588 2023-06-27 09:02:59.123155 bertagent-1.0.5/setup.cfg
+-rw-------   0 jiko      (1000) jiko      (1000)     2664 2023-05-22 00:59:01.000000 bertagent-1.0.5/setup.py
+-rw-------   0 jiko      (1000) jiko      (1000)      539 2023-05-22 00:59:01.000000 bertagent-1.0.5/tox.ini
+-rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-22 00:59:02.000000 bertagent-1.0.5/versioneer.py
```

### Comparing `bertagent-1.0.4/.github/workflows/build-main.yml` & `bertagent-1.0.5/.github/workflows/build-main.yml`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/.gitignore` & `bertagent-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/.readthedocs.yaml` & `bertagent-1.0.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/CONTRIBUTING.rst` & `bertagent-1.0.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/LICENSE` & `bertagent-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/Makefile` & `bertagent-1.0.5/Makefile`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/PKG-INFO` & `bertagent-1.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bertagent
-Version: 1.0.4
+Version: 1.0.5
 Summary: Quantify linguistic agency in textual data.
 Home-page: https://github.com/cogsys-io/bertagent
 Author: cogsys.io
 Author-email: bertagent@cogsys.io
 License: GNU General Public License v3
 Keywords: bertagent
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -54,15 +54,16 @@
 * Documentation: https://bertagent.readthedocs.io (https://bertagent.rtfd.io)
 * Free software: GNU General Public License v3
 
 
 Features
 --------
 
-* TODO
+* Detect linguistic agnecy in text using large language model
+  (pretrained transformers architecture).
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `cogsys-io/cogsys-io-cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/cookiecutter/cookiecutter
```

### Comparing `bertagent-1.0.4/README.rst` & `bertagent-1.0.5/docs/source/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-=========
-BERTAgent
-=========
+🚀 Welcome to BERTAgent's documentation!
+========================================
 
 .. image:: https://img.shields.io/pypi/v/bertagent?version=latest
    :target: https://pypi.python.org/pypi/bertagent
    :alt: PyPI Version
 
 .. image:: https://img.shields.io/github/actions/workflow/status/cogsys-io/bertagent/build-main.yml
    :alt: GitHub Workflow (Build Main) Status
@@ -15,28 +14,25 @@
    :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/l/bertagent?color=brightgreen
    :target: https://github.com/cogsys-io/bertagent/blob/master/LICENSE
    :alt: License
 
 
-Quantify linguistic agency in textual data.
-
-* Publication: BERTAgent: A Novel Tool to Quantify Agency in Textual Data (doi: TBA)
-* PyPi: https://pypi.org/project/bertagent/
-* GitHub: https://github.com/cogsys-io/bertagent
-* Documentation: https://bertagent.readthedocs.io (https://bertagent.rtfd.io)
-* Free software: GNU General Public License v3
-
-
-Features
---------
-
-* TODO
-
-Credits
--------
-
-This package was created with Cookiecutter_ and the `cogsys-io/cogsys-io-cookiecutter-pypackage`_ project template.
-
-.. _Cookiecutter: https://github.com/cookiecutter/cookiecutter
-.. _`cogsys-io/cogsys-io-cookiecutter-pypackage`: https://github.com/cogsys-io/cogsys-io-cookiecutter-pypackage
+.. toctree::
+   :maxdepth: 2
+   :caption: Contents:
+
+   readme
+   installation
+   tutorial
+   usage
+   Package modules <modules>
+   contributing
+   authors
+   history
+
+Indices and tables
+==================
+* :ref:`genindex`
+* :ref:`modindex`
+* :ref:`search`
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bertagent-1.0.4/bertagent/bertagent.py` & `bertagent-1.0.5/bertagent/bertagent.py`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/bertagent/data/emacs-logo/emacs-128x128.png` & `bertagent-1.0.5/bertagent/data/emacs-logo/emacs-128x128.png`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/bertagent/data/emacs-logo/emacs.svg` & `bertagent-1.0.5/bertagent/data/emacs-logo/emacs.svg`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/bertagent/tests/test_bertagent.py` & `bertagent-1.0.5/bertagent/tests/test_bertagent.py`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/bertagent.egg-info/PKG-INFO` & `bertagent-1.0.5/bertagent.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bertagent
-Version: 1.0.4
+Version: 1.0.5
 Summary: Quantify linguistic agency in textual data.
 Home-page: https://github.com/cogsys-io/bertagent
 Author: cogsys.io
 Author-email: bertagent@cogsys.io
 License: GNU General Public License v3
 Keywords: bertagent
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -54,15 +54,16 @@
 * Documentation: https://bertagent.readthedocs.io (https://bertagent.rtfd.io)
 * Free software: GNU General Public License v3
 
 
 Features
 --------
 
-* TODO
+* Detect linguistic agnecy in text using large language model
+  (pretrained transformers architecture).
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `cogsys-io/cogsys-io-cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/cookiecutter/cookiecutter
```

### Comparing `bertagent-1.0.4/bertagent.egg-info/SOURCES.txt` & `bertagent-1.0.5/bertagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/bertagent.egg-info/requires.txt` & `bertagent-1.0.5/bertagent.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/docs/Makefile` & `bertagent-1.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `bertagent-1.0.5/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/docs/requirements.txt` & `bertagent-1.0.5/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/docs/source/conf.py` & `bertagent-1.0.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/docs/source/installation.rst` & `bertagent-1.0.5/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/docs/source/tutorial-01-input.csv` & `bertagent-1.0.5/docs/source/tutorial-01-input.csv`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/docs/source/tutorial-02-output.csv` & `bertagent-1.0.5/docs/source/tutorial-02-output.csv`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/docs/source/tutorial.rst` & `bertagent-1.0.5/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/pyproject.toml` & `bertagent-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/requirements_dev.txt` & `bertagent-1.0.5/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/setup.cfg` & `bertagent-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/setup.py` & `bertagent-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/tox.ini` & `bertagent-1.0.5/tox.ini`

 * *Files identical despite different names*

### Comparing `bertagent-1.0.4/versioneer.py` & `bertagent-1.0.5/versioneer.py`

 * *Files identical despite different names*

