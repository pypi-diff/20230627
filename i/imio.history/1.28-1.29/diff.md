# Comparing `tmp/imio.history-1.28.tar.gz` & `tmp/imio.history-1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.history-1.28.tar", last modified: Mon Feb 27 11:27:15 2023, max compression
+gzip compressed data, was "dist/imio.history-1.29.tar", last modified: Tue Jun 27 10:00:11 2023, max compression
```

## Comparing `imio.history-1.28.tar` & `imio.history-1.29.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:15.000000 imio.history-1.28/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18027 2023-02-27 11:27:14.000000 imio.history-1.28/LICENSE.rst
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:15.000000 imio.history-1.28/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio.history.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio.history.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio.history.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio.history.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio.history.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13248 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio.history.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2259 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio.history.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio.history.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       89 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio.history.egg-info/requires.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio/history/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1071 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4962 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/adapters.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio/history/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      817 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/locales/manual.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio/history/locales/es/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio/history/locales/es/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      623 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/locales/es/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1514 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/locales/es/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1129 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/locales/imio.history.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio/history/locales/en/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio/history/locales/en/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      523 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/locales/en/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1224 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/locales/en/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      594 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/locales/plone.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio/history/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio/history/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      523 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1250 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/locales/fr/LC_MESSAGES/imio.history.po
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio/history/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio/history/profiles/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      164 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/profiles/testing/metadata.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio/history/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      260 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/profiles/default/browserlayer.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       73 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      217 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/profiles/default/viewlets.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      457 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/profiles/default/cssregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2411 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      717 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/testing-adapter.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1628 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/interfaces.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3108 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/mk_sync_locales.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4411 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      180 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/safe_utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      517 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/config.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      817 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/testing.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio/history/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2927 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/tests/test_revisionhistory.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9606 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/tests/test_utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2522 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/tests/test_workflowhistory.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1406 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/tests/test_versionpreview.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1266 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/tests/adapters.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3249 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/tests/test_documentbylineviewlet.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10532 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/tests/test_contenthistory.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      584 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/tests/test_setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      189 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio/history/browser/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio/history/browser/static/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      252 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/browser/static/imiohistory.css
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7672 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/browser/views.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1471 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/browser/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:15.000000 imio.history-1.28/src/imio/history/browser/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6179 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/browser/templates/content_history.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       96 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/browser/templates/event_preview.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3309 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/browser/templates/document_byline.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       96 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/browser/templates/version_preview.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-02-27 11:27:14.000000 imio.history-1.28/src/imio/history/browser/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       50 2023-02-27 11:27:14.000000 imio.history-1.28/requirements.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1488 2023-02-27 11:27:14.000000 imio.history-1.28/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13248 2023-02-27 11:27:15.000000 imio.history-1.28/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      380 2023-02-27 11:27:14.000000 imio.history-1.28/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7605 2023-02-27 11:27:14.000000 imio.history-1.28/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       46 2023-02-27 11:27:14.000000 imio.history-1.28/CONTRIBUTORS.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      500 2023-02-27 11:27:14.000000 imio.history-1.28/versions.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2438 2023-02-27 11:27:14.000000 imio.history-1.28/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       94 2023-02-27 11:27:14.000000 imio.history-1.28/.coveragerc
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      131 2023-02-27 11:27:14.000000 imio.history-1.28/.isort.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2023-02-27 11:27:15.000000 imio.history-1.28/setup.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      775 2023-02-27 11:27:14.000000 imio.history-1.28/buildout.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      164 2023-02-27 11:27:14.000000 imio.history-1.28/ci.cfg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18027 2023-06-27 10:00:11.000000 imio.history-1.29/LICENSE.rst
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio.history.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio.history.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio.history.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio.history.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio.history.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13558 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio.history.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2259 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio.history.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio.history.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       89 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio.history.egg-info/requires.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1071 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4962 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/adapters.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      817 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/locales/manual.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/locales/es/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/locales/es/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      623 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/locales/es/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1514 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/locales/es/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1129 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/locales/imio.history.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/locales/en/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      523 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/locales/en/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1224 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/locales/en/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      594 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/locales/plone.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      523 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1250 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/locales/fr/LC_MESSAGES/imio.history.po
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/profiles/testing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      164 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/profiles/testing/metadata.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      260 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/profiles/default/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       73 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      217 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/profiles/default/viewlets.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      457 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/profiles/default/cssregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2411 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      717 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/testing-adapter.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1628 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/interfaces.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3108 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/mk_sync_locales.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4411 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      180 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/safe_utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      517 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      817 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/testing.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2927 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/tests/test_revisionhistory.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9606 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/tests/test_utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2522 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/tests/test_workflowhistory.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1325 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/tests/test_versionpreview.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1266 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/tests/adapters.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3249 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/tests/test_documentbylineviewlet.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10996 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/tests/test_contenthistory.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      584 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/tests/test_setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      189 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/browser/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/browser/static/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      252 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/browser/static/imiohistory.css
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7727 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/browser/views.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1471 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/browser/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/browser/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6179 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/browser/templates/content_history.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       96 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/browser/templates/event_preview.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3309 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/browser/templates/document_byline.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       96 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/browser/templates/version_preview.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:00:11.000000 imio.history-1.29/src/imio/history/browser/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       50 2023-06-27 10:00:11.000000 imio.history-1.29/requirements.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1488 2023-06-27 10:00:11.000000 imio.history-1.29/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13558 2023-06-27 10:00:11.000000 imio.history-1.29/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      380 2023-06-27 10:00:11.000000 imio.history-1.29/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7851 2023-06-27 10:00:11.000000 imio.history-1.29/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       46 2023-06-27 10:00:11.000000 imio.history-1.29/CONTRIBUTORS.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      500 2023-06-27 10:00:11.000000 imio.history-1.29/versions.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2438 2023-06-27 10:00:11.000000 imio.history-1.29/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       94 2023-06-27 10:00:11.000000 imio.history-1.29/.coveragerc
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      131 2023-06-27 10:00:11.000000 imio.history-1.29/.isort.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2023-06-27 10:00:11.000000 imio.history-1.29/setup.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      775 2023-06-27 10:00:11.000000 imio.history-1.29/buildout.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      164 2023-06-27 10:00:11.000000 imio.history-1.29/ci.cfg
```

### Comparing `imio.history-1.28/LICENSE.rst` & `imio.history-1.29/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio.history.egg-info/PKG-INFO` & `imio.history-1.29/src/imio.history.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.history
-Version: 1.28
+Version: 1.29
 Summary: Imio history
 Home-page: http://pypi.python.org/pypi/imio.history
 Author: IMIO
 Author-email: dev@imio.be
 License: GPL
 Description: .. image:: https://github.com/IMIO/imio.history/actions/workflows/main.yml/badge.svg?branch=master
             :target: https://github.com/IMIO/imio.history/actions/workflows/main.yml
@@ -67,14 +67,22 @@
         
         Contributors
         ============
         
         Changelog
         =========
         
+        1.29 (2023-06-27)
+        -----------------
+        
+        - Make `IHContentHistoryView.renderComments` more robust by passing original
+          `mimetype='text/plain'` to avoid `portal_transforms` detecting it automatically
+          that can lead to wrong detection.
+          [gbastien]
+        
         1.28 (2023-02-27)
         -----------------
         
         - Added possibility to display an event preview under the comment
           in the `@@contenthistory` view.
           [gbastien]
         - Make the `highlight_last_comment` functionnality generic, it was only used
```

### Comparing `imio.history-1.28/src/imio.history.egg-info/SOURCES.txt` & `imio.history-1.29/src/imio.history.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/configure.zcml` & `imio.history-1.29/src/imio/history/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/adapters.py` & `imio.history-1.29/src/imio/history/adapters.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/locales/manual.pot` & `imio.history-1.29/src/imio/history/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/locales/es/LC_MESSAGES/plone.po` & `imio.history-1.29/src/imio/history/locales/es/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/locales/es/LC_MESSAGES/imio.history.po` & `imio.history-1.29/src/imio/history/locales/es/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/locales/imio.history.pot` & `imio.history-1.29/src/imio/history/locales/imio.history.pot`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/locales/en/LC_MESSAGES/plone.po` & `imio.history-1.29/src/imio/history/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/locales/en/LC_MESSAGES/imio.history.po` & `imio.history-1.29/src/imio/history/locales/en/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/locales/plone.pot` & `imio.history-1.29/src/imio/history/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/locales/fr/LC_MESSAGES/plone.po` & `imio.history-1.29/src/imio/history/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/locales/fr/LC_MESSAGES/imio.history.po` & `imio.history-1.29/src/imio/history/locales/fr/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/testing.py` & `imio.history-1.29/src/imio/history/testing.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/testing-adapter.zcml` & `imio.history-1.29/src/imio/history/testing-adapter.zcml`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/interfaces.py` & `imio.history-1.29/src/imio/history/interfaces.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/mk_sync_locales.sh` & `imio.history-1.29/src/imio/history/mk_sync_locales.sh`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/utils.py` & `imio.history-1.29/src/imio/history/utils.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/config.py` & `imio.history-1.29/src/imio/history/config.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/testing.zcml` & `imio.history-1.29/src/imio/history/testing.zcml`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/tests/test_revisionhistory.py` & `imio.history-1.29/src/imio/history/tests/test_revisionhistory.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/tests/test_utils.py` & `imio.history-1.29/src/imio/history/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/tests/test_workflowhistory.py` & `imio.history-1.29/src/imio/history/tests/test_workflowhistory.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/tests/test_versionpreview.py` & `imio.history-1.29/src/imio/history/tests/test_versionpreview.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,17 +23,14 @@
         doc.setTitle("Document title 3")
         doc.reindexObject(idxs=['Title', ])
         # the view __call__ receives a version_id
         # it will store in self.versioned_object the version_id object
         # so it is available in the template
         view = doc.restrictedTraverse('@@history-version-preview')
         # current
-        self.assertEquals(view.context.Title(),
-                          "Document title 3")
+        self.assertEqual(view.context.Title(), "Document title 3")
         # version_id 1
         view(version_id=1)
-        self.assertEquals(view.versioned_object.Title(),
-                          "Document title 1")
+        self.assertEqual(view.versioned_object.Title(), "Document title 1")
         # version_id 2
         view(version_id=2)
-        self.assertEquals(view.versioned_object.Title(),
-                          "Document title 2")
+        self.assertEqual(view.versioned_object.Title(), "Document title 2")
```

### Comparing `imio.history-1.28/src/imio/history/tests/adapters.py` & `imio.history-1.29/src/imio/history/tests/adapters.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/tests/test_documentbylineviewlet.py` & `imio.history-1.29/src/imio/history/tests/test_documentbylineviewlet.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/tests/test_contenthistory.py` & `imio.history-1.29/src/imio/history/tests/test_contenthistory.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,22 +188,29 @@
         view = getMultiAdapter((self.doc, self.portal.REQUEST), name='contenthistory')
         view.histories_to_handle = (u'workflow', )
 
         # translated
         # do a transition with a comment that will be translatable
         self.wft.doActionFor(self.doc, 'publish', comment='data_change')
         last_event = view.getHistory()[0]
-        self.assertEquals(view.renderComments(last_event), u'<p>Data change</p>')
+        self.assertEqual(view.renderComments(last_event), u'<p>Data change</p>')
 
         # turned from text/plain to text/html
         # do a transition with a comment that will be translatable
         self.wft.doActionFor(self.doc, 'retract', comment='Custom comments not translatable.\nAnd one additional line.')
         last_event = view.getHistory()[0]
-        self.assertEquals(view.renderComments(last_event),
-                          u'<p>Custom comments not translatable.<br />And one additional line.</p>')
+        self.assertEqual(view.renderComments(last_event),
+                         u'<p>Custom comments not translatable.<br />And one additional line.</p>')
+        # special value may break rendering when mimetype is not given
+        last_event['comments'] = u'*** x-patch mimetype ***'
+        self.assertEqual(view.renderComments(last_event),
+                         u'<p>*** x-patch mimetype ***</p>')
+        # mimetype passed to renderComments is 'text/plain', if not given
+        # it is auto detected by mimetypes_registry
+        self.assertRaises(AttributeError, view.renderComments, last_event, mimetype=None)
 
     def test_contenthistoryWithEventPreview(self):
         """Test the event-preview-view."""
         self.wft.doActionFor(self.doc, 'publish', comment='My comment')
         view = getMultiAdapter((self.doc, self.portal.REQUEST), name='contenthistory')
         # preview is there because we overrided show_preview in adapters.TestingIHContentHistoryView
         self.assertTrue("No preview available." in view())
```

### Comparing `imio.history-1.28/src/imio/history/tests/test_setup.py` & `imio.history-1.29/src/imio/history/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/browser/views.py` & `imio.history-1.29/src/imio/history/browser/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         else:
             return transitionName
 
     def _extra_render_comments_mapping(self):
         """ """
         return {}
 
-    def renderComments(self, event):
+    def renderComments(self, event, mimetype='text/plain'):
         """
           Render comments correctly as it is 'plain/text' and we want 'text/html'.
         """
         # prepare some data passed to translate as mappings
         mapping = event.copy()
         mapping['event_time'] = int(event['time'])
         mapping['url'] = self.context.absolute_url()
@@ -112,15 +112,16 @@
         # try to translate comments before it is turned into text/html
         translated = translate(
             safe_unicode(event['comments']),
             mapping=mapping,
             domain='imio.history',
             context=self.request)
         transformsTool = api.portal.get_tool('portal_transforms')
-        data = transformsTool.convertTo('text/x-html-safe', translated)
+        data = transformsTool.convertTo(
+            'text/x-html-safe', translated, mimetype=mimetype)
         return data.getData()
 
     @memoize
     def _getCurrentContextWorkflow(self):
         """
           Return currently used workflow.
         """
```

### Comparing `imio.history-1.28/src/imio/history/browser/configure.zcml` & `imio.history-1.29/src/imio/history/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/browser/templates/content_history.pt` & `imio.history-1.29/src/imio/history/browser/templates/content_history.pt`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/src/imio/history/browser/templates/document_byline.pt` & `imio.history-1.29/src/imio/history/browser/templates/document_byline.pt`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/setup.py` & `imio.history-1.29/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'Contributors\n'
     '============\n' + '\n' +
     open('CHANGES.rst').read() + '\n')
 
 
 setup(
     name='imio.history',
-    version='1.28',
+    version='1.29',
     description="Imio history",
     long_description=long_description,
     # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 6 - Mature",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `imio.history-1.28/PKG-INFO` & `imio.history-1.29/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.history
-Version: 1.28
+Version: 1.29
 Summary: Imio history
 Home-page: http://pypi.python.org/pypi/imio.history
 Author: IMIO
 Author-email: dev@imio.be
 License: GPL
 Description: .. image:: https://github.com/IMIO/imio.history/actions/workflows/main.yml/badge.svg?branch=master
             :target: https://github.com/IMIO/imio.history/actions/workflows/main.yml
@@ -67,14 +67,22 @@
         
         Contributors
         ============
         
         Changelog
         =========
         
+        1.29 (2023-06-27)
+        -----------------
+        
+        - Make `IHContentHistoryView.renderComments` more robust by passing original
+          `mimetype='text/plain'` to avoid `portal_transforms` detecting it automatically
+          that can lead to wrong detection.
+          [gbastien]
+        
         1.28 (2023-02-27)
         -----------------
         
         - Added possibility to display an event preview under the comment
           in the `@@contenthistory` view.
           [gbastien]
         - Make the `highlight_last_comment` functionnality generic, it was only used
```

### Comparing `imio.history-1.28/CHANGES.rst` & `imio.history-1.29/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+1.29 (2023-06-27)
+-----------------
+
+- Make `IHContentHistoryView.renderComments` more robust by passing original
+  `mimetype='text/plain'` to avoid `portal_transforms` detecting it automatically
+  that can lead to wrong detection.
+  [gbastien]
+
 1.28 (2023-02-27)
 -----------------
 
 - Added possibility to display an event preview under the comment
   in the `@@contenthistory` view.
   [gbastien]
 - Make the `highlight_last_comment` functionnality generic, it was only used
```

### Comparing `imio.history-1.28/README.rst` & `imio.history-1.29/README.rst`

 * *Files identical despite different names*

### Comparing `imio.history-1.28/buildout.cfg` & `imio.history-1.29/buildout.cfg`

 * *Files identical despite different names*

