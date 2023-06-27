# Comparing `tmp/mdacli-0.1.8.tar.gz` & `tmp/mdacli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdacli-0.1.8.tar", last modified: Sun Jan 16 19:13:46 2022, max compression
+gzip compressed data, was "mdacli-0.1.9.tar", last modified: Sun Jan 16 19:41:25 2022, max compression
```

## Comparing `mdacli-0.1.8.tar` & `mdacli-0.1.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:13:46.561717 mdacli-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-01-16 19:13:29.000000 mdacli-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-01-16 19:13:29.000000 mdacli-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8017 2022-01-16 19:13:46.561717 mdacli-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4906 2022-01-16 19:13:29.000000 mdacli-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:13:46.557716 mdacli-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-01-16 19:13:44.000000 mdacli-0.1.8/docs/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5423 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/PULLREQUEST.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:13:46.557716 mdacli-0.1.8/docs/rst/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:13:46.557716 mdacli-0.1.8/docs/rst/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     3994 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:13:46.561717 mdacli-0.1.8/docs/rst/_static/logos/
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/_static/logos/AUTHOR
--rw-r--r--   0 runner    (1001) docker     (121)    55844 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/_static/logos/mdacli-logo-square.pdf
--rw-r--r--   0 runner    (1001) docker     (121)    59970 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/_static/logos/mdacli-logo-square.png
--rw-r--r--   0 runner    (1001) docker     (121)    54729 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/_static/logos/mdacli-logo.pdf
--rw-r--r--   0 runner    (1001) docker     (121)    50625 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/_static/logos/mdacli-logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     4542 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/_static/logos/mdanalysis-logo.ico
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:13:46.561717 mdacli-0.1.8/docs/rst/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/_templates/footer.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:13:46.561717 mdacli-0.1.8/docs/rst/api/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/api/cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/api/colors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/api/libcli.rst
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/api/logger.rst
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/api/save.rst
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3355 2022-01-16 19:13:44.000000 mdacli-0.1.8/docs/rst/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2715 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/philosophy.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-01-16 19:13:29.000000 mdacli-0.1.8/docs/rst/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-16 19:13:46.561717 mdacli-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3350 2022-01-16 19:13:44.000000 mdacli-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:13:46.557716 mdacli-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:13:46.561717 mdacli-0.1.8/src/mdacli/
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-01-16 19:13:44.000000 mdacli-0.1.8/src/mdacli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1554 2022-01-16 19:13:29.000000 mdacli-0.1.8/src/mdacli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4398 2022-01-16 19:13:29.000000 mdacli-0.1.8/src/mdacli/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4292 2022-01-16 19:13:29.000000 mdacli-0.1.8/src/mdacli/colors.py
--rw-r--r--   0 runner    (1001) docker     (121)    24483 2022-01-16 19:13:29.000000 mdacli-0.1.8/src/mdacli/libcli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2102 2022-01-16 19:13:29.000000 mdacli-0.1.8/src/mdacli/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)    10995 2022-01-16 19:13:29.000000 mdacli-0.1.8/src/mdacli/save.py
--rw-r--r--   0 runner    (1001) docker     (121)     8364 2022-01-16 19:13:29.000000 mdacli-0.1.8/src/mdacli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:13:46.561717 mdacli-0.1.8/src/mdacli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8017 2022-01-16 19:13:46.000000 mdacli-0.1.8/src/mdacli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-01-16 19:13:46.000000 mdacli-0.1.8/src/mdacli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-16 19:13:46.000000 mdacli-0.1.8/src/mdacli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-01-16 19:13:46.000000 mdacli-0.1.8/src/mdacli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-16 19:13:46.000000 mdacli-0.1.8/src/mdacli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-01-16 19:13:46.000000 mdacli-0.1.8/src/mdacli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-01-16 19:13:46.000000 mdacli-0.1.8/src/mdacli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:41:25.626486 mdacli-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-01-16 19:41:06.000000 mdacli-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2022-01-16 19:41:06.000000 mdacli-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     8119 2022-01-16 19:41:25.626486 mdacli-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4905 2022-01-16 19:41:06.000000 mdacli-0.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:41:25.622486 mdacli-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-01-16 19:41:24.000000 mdacli-0.1.9/docs/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5423 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/PULLREQUEST.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:41:25.622486 mdacli-0.1.9/docs/rst/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:41:25.622486 mdacli-0.1.9/docs/rst/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     3994 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:41:25.622486 mdacli-0.1.9/docs/rst/_static/logos/
+-rw-r--r--   0 runner    (1001) docker     (121)      740 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/_static/logos/AUTHOR
+-rw-r--r--   0 runner    (1001) docker     (121)    55844 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/_static/logos/mdacli-logo-square.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)    59970 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/_static/logos/mdacli-logo-square.png
+-rw-r--r--   0 runner    (1001) docker     (121)    54729 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/_static/logos/mdacli-logo.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)    50625 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/_static/logos/mdacli-logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4542 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/_static/logos/mdanalysis-logo.ico
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:41:25.622486 mdacli-0.1.9/docs/rst/_templates/
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/_templates/footer.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:41:25.622486 mdacli-0.1.9/docs/rst/api/
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/api/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/api/colors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/api/libcli.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/api/logger.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/api/save.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3355 2022-01-16 19:41:24.000000 mdacli-0.1.9/docs/rst/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      853 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2715 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/philosophy.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-01-16 19:41:06.000000 mdacli-0.1.9/docs/rst/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-16 19:41:25.626486 mdacli-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3350 2022-01-16 19:41:24.000000 mdacli-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:41:25.622486 mdacli-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:41:25.626486 mdacli-0.1.9/src/mdacli/
+-rw-r--r--   0 runner    (1001) docker     (121)      389 2022-01-16 19:41:24.000000 mdacli-0.1.9/src/mdacli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1554 2022-01-16 19:41:06.000000 mdacli-0.1.9/src/mdacli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4398 2022-01-16 19:41:06.000000 mdacli-0.1.9/src/mdacli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4292 2022-01-16 19:41:06.000000 mdacli-0.1.9/src/mdacli/colors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24483 2022-01-16 19:41:06.000000 mdacli-0.1.9/src/mdacli/libcli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2102 2022-01-16 19:41:06.000000 mdacli-0.1.9/src/mdacli/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10995 2022-01-16 19:41:06.000000 mdacli-0.1.9/src/mdacli/save.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8364 2022-01-16 19:41:06.000000 mdacli-0.1.9/src/mdacli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 19:41:25.626486 mdacli-0.1.9/src/mdacli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8119 2022-01-16 19:41:25.000000 mdacli-0.1.9/src/mdacli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-01-16 19:41:25.000000 mdacli-0.1.9/src/mdacli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-16 19:41:25.000000 mdacli-0.1.9/src/mdacli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-01-16 19:41:25.000000 mdacli-0.1.9/src/mdacli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-16 19:41:25.000000 mdacli-0.1.9/src/mdacli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-01-16 19:41:25.000000 mdacli-0.1.9/src/mdacli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-01-16 19:41:25.000000 mdacli-0.1.9/src/mdacli.egg-info/top_level.txt
```

### Comparing `mdacli-0.1.8/LICENSE` & `mdacli-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mdacli-0.1.8/PKG-INFO` & `mdacli-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdacli
-Version: 0.1.8
+Version: 0.1.9
 Summary: A command line client for MDAnalysis Analysis classes.
 Home-page: https://github.com/MDAnalysis/mdacli
 Author: PicoCentauri, joaomcteixeira
 Author-email: philip-loche@gmx.de, joaomcteixeira@gmail.com
 Maintainer: PicoCentauri, joaomcteixeira, MDA devs
 Maintainer-email: philip-loche@gmx.de, joaomcteixeira@gmail.com, mdanalysis@numfocus.org
 License: GPLv3
@@ -127,24 +127,29 @@
 
  .. |docs| image:: https://readthedocs.org/projects/mdacli/badge/?version=latest
    :target: https://mdacli.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
  .. |test| image:: https://github.com/MDAnalysis/mdacli/actions/workflows/test.yml/badge.svg?branch=main
    :alt: Github Actions Build Status
-   :target: https://github.com/MDAnalysis/mdacli/actions/workflows/tests.yml
+   :target: https://github.com/MDAnalysis/mdacli/actions/workflows/test.yml
 
  .. |codecov| image:: https://codecov.io/gh/MDAnalysis/mdacli/branch/main/graph/badge.svg?token=ets2mZ6xJD
     :alt: Codecov mdacli
     :target: https://codecov.io/gh/MDAnalysis/mdacli
 
 
 Changelog
 =========
 
+v0.1.9 (2022-01-16)
+------------------------------------------
+
+* Fix test banner in README.rst (#85)
+
 v0.1.8 (2022-01-16)
 ------------------------------------------
 
 * Use Github actions matrix for tests (#68)
 * Fix Conda permissions on MacOS (#68)
 * Fix Tests failing on Windows (#68)
```

### Comparing `mdacli-0.1.8/README.rst` & `mdacli-0.1.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -85,12 +85,12 @@
 
  .. |docs| image:: https://readthedocs.org/projects/mdacli/badge/?version=latest
    :target: https://mdacli.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
  .. |test| image:: https://github.com/MDAnalysis/mdacli/actions/workflows/test.yml/badge.svg?branch=main
    :alt: Github Actions Build Status
-   :target: https://github.com/MDAnalysis/mdacli/actions/workflows/tests.yml
+   :target: https://github.com/MDAnalysis/mdacli/actions/workflows/test.yml
 
  .. |codecov| image:: https://codecov.io/gh/MDAnalysis/mdacli/branch/main/graph/badge.svg?token=ets2mZ6xJD
     :alt: Codecov mdacli
     :target: https://codecov.io/gh/MDAnalysis/mdacli
```

### Comparing `mdacli-0.1.8/docs/CHANGELOG.rst` & `mdacli-0.1.9/docs/CHANGELOG.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 
 Changelog
 =========
 
+v0.1.9 (2022-01-16)
+------------------------------------------
+
+* Fix test banner in README.rst (#85)
+
 v0.1.8 (2022-01-16)
 ------------------------------------------
 
 * Use Github actions matrix for tests (#68)
 * Fix Conda permissions on MacOS (#68)
 * Fix Tests failing on Windows (#68)
```

### Comparing `mdacli-0.1.8/docs/CONTRIBUTING.rst` & `mdacli-0.1.9/docs/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mdacli-0.1.8/docs/rst/_static/custom.css` & `mdacli-0.1.9/docs/rst/_static/custom.css`

 * *Files identical despite different names*

### Comparing `mdacli-0.1.8/docs/rst/_static/logos/AUTHOR` & `mdacli-0.1.9/docs/rst/_static/logos/AUTHOR`

 * *Files identical despite different names*

### Comparing `mdacli-0.1.8/docs/rst/_static/logos/mdacli-logo-square.pdf` & `mdacli-0.1.9/docs/rst/_static/logos/mdacli-logo-square.pdf`

 * *Files identical despite different names*

### Comparing `mdacli-0.1.8/docs/rst/_static/logos/mdacli-logo-square.png` & `mdacli-0.1.9/docs/rst/_static/logos/mdacli-logo-square.png`

 * *Files identical despite different names*

### Comparing `mdacli-0.1.8/docs/rst/_static/logos/mdacli-logo.pdf` & `mdacli-0.1.9/docs/rst/_static/logos/mdacli-logo.pdf`

 * *Files identical despite different names*

### Comparing `mdacli-0.1.8/docs/rst/_static/logos/mdacli-logo.png` & `mdacli-0.1.9/docs/rst/_static/logos/mdacli-logo.png`

 * *Files identical despite different names*

### Comparing `mdacli-0.1.8/docs/rst/_static/logos/mdanalysis-logo.ico` & `mdacli-0.1.9/docs/rst/_static/logos/mdanalysis-logo.ico`

 * *Files identical despite different names*

### Comparing `mdacli-0.1.8/docs/rst/conf.py` & `mdacli-0.1.9/docs/rst/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 source_suffix = '.rst'
 master_doc = 'index'
 project = 'mdacli'
 year = '2021'
 author = 'Philip Loche, Joao MC Teixeira and Oliver Beckstein'
 copyright = '{0}, {1}'.format(year, author)
-version = release = '0.1.8'
+version = release = '0.1.9'
 
 pygments_style = 'trac'
 templates_path = ['_templates']
 
 extlinks = {
     'issue': ('https://github.com/MDAnalysis/mdacli/cissues/%s', '#'),
     'pr': ('https://github.com/MDAnalysis/mdacli/pull/%s', 'PR #'),
```

### Comparing `mdacli-0.1.8/docs/rst/installation.rst` & `mdacli-0.1.9/docs/rst/installation.rst`

 * *Files identical despite different names*

### Comparing `mdacli-0.1.8/docs/rst/philosophy.rst` & `mdacli-0.1.9/docs/rst/philosophy.rst`

 * *Files identical despite different names*

### Comparing `mdacli-0.1.8/docs/rst/usage.rst` & `mdacli-0.1.9/docs/rst/usage.rst`

 * *Files identical despite different names*

### Comparing `mdacli-0.1.8/setup.py` & `mdacli-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 long_description = '{}\n{}'.format(
     read('README.rst'),
     read(join('docs', 'CHANGELOG.rst')),
     )
 
 setup(
     name='mdacli',
-    version='0.1.8',
+    version='0.1.9',
     description='A command line client for MDAnalysis Analysis classes.',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     license='GPLv3',
     author='PicoCentauri, joaomcteixeira',
     author_email='philip-loche@gmx.de, joaomcteixeira@gmail.com',
     maintainer='PicoCentauri, joaomcteixeira, MDA devs',
```

### Comparing `mdacli-0.1.8/src/mdacli/__main__.py` & `mdacli-0.1.9/src/mdacli/__main__.py`

 * *Files identical despite different names*

### Comparing `mdacli-0.1.8/src/mdacli/cli.py` & `mdacli-0.1.9/src/mdacli/cli.py`

 * *Files identical despite different names*

### Comparing `mdacli-0.1.8/src/mdacli/colors.py` & `mdacli-0.1.9/src/mdacli/colors.py`

 * *Files identical despite different names*

### Comparing `mdacli-0.1.8/src/mdacli/libcli.py` & `mdacli-0.1.9/src/mdacli/libcli.py`

 * *Files identical despite different names*

### Comparing `mdacli-0.1.8/src/mdacli/logger.py` & `mdacli-0.1.9/src/mdacli/logger.py`

 * *Files identical despite different names*

### Comparing `mdacli-0.1.8/src/mdacli/save.py` & `mdacli-0.1.9/src/mdacli/save.py`

 * *Files identical despite different names*

### Comparing `mdacli-0.1.8/src/mdacli/utils.py` & `mdacli-0.1.9/src/mdacli/utils.py`

 * *Files identical despite different names*

### Comparing `mdacli-0.1.8/src/mdacli.egg-info/PKG-INFO` & `mdacli-0.1.9/src/mdacli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdacli
-Version: 0.1.8
+Version: 0.1.9
 Summary: A command line client for MDAnalysis Analysis classes.
 Home-page: https://github.com/MDAnalysis/mdacli
 Author: PicoCentauri, joaomcteixeira
 Author-email: philip-loche@gmx.de, joaomcteixeira@gmail.com
 Maintainer: PicoCentauri, joaomcteixeira, MDA devs
 Maintainer-email: philip-loche@gmx.de, joaomcteixeira@gmail.com, mdanalysis@numfocus.org
 License: GPLv3
@@ -127,24 +127,29 @@
 
  .. |docs| image:: https://readthedocs.org/projects/mdacli/badge/?version=latest
    :target: https://mdacli.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
  .. |test| image:: https://github.com/MDAnalysis/mdacli/actions/workflows/test.yml/badge.svg?branch=main
    :alt: Github Actions Build Status
-   :target: https://github.com/MDAnalysis/mdacli/actions/workflows/tests.yml
+   :target: https://github.com/MDAnalysis/mdacli/actions/workflows/test.yml
 
  .. |codecov| image:: https://codecov.io/gh/MDAnalysis/mdacli/branch/main/graph/badge.svg?token=ets2mZ6xJD
     :alt: Codecov mdacli
     :target: https://codecov.io/gh/MDAnalysis/mdacli
 
 
 Changelog
 =========
 
+v0.1.9 (2022-01-16)
+------------------------------------------
+
+* Fix test banner in README.rst (#85)
+
 v0.1.8 (2022-01-16)
 ------------------------------------------
 
 * Use Github actions matrix for tests (#68)
 * Fix Conda permissions on MacOS (#68)
 * Fix Tests failing on Windows (#68)
```

### Comparing `mdacli-0.1.8/src/mdacli.egg-info/SOURCES.txt` & `mdacli-0.1.9/src/mdacli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

