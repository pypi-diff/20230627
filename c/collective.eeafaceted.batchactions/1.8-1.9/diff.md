# Comparing `tmp/collective.eeafaceted.batchactions-1.8.tar.gz` & `tmp/collective.eeafaceted.batchactions-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.eeafaceted.batchactions-1.8.tar", last modified: Fri Jul 16 14:50:00 2021, max compression
+gzip compressed data, was "collective.eeafaceted.batchactions-1.9.tar", last modified: Mon Dec  6 09:52:46 2021, max compression
```

## Comparing `collective.eeafaceted.batchactions-1.8.tar` & `collective.eeafaceted.batchactions-1.9.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      258 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/setuphandlers.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1592 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      548 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/locales/manual.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/locales/en/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/locales/en/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3312 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/locales/en/LC_MESSAGES/collective.eeafaceted.batchactions.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3079 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/locales/collective.eeafaceted.batchactions.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4426 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/locales/fr/LC_MESSAGES/collective.eeafaceted.batchactions.po
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/profiles/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      258 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/profiles/testing/metadata.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/profiles/testing/types/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1915 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/profiles/testing/types/testtype.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      230 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/profiles/testing/types.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       68 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      352 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/profiles/default/cssregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/profiles/default/collectiveeeafacetedbatchactions_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      464 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/profiles/default/jsregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2960 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      155 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/interfaces.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3061 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/mk_sync_locales.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2264 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1589 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/testing.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3372 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/tests/test_utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      979 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/tests/views.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8004 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/tests/test_forms.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1006 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/tests/base.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      228 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/tests/interfaces.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4185 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/tests/test_contact_form.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5070 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/tests/test_labels_form.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7456 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/tests/test_viewlets.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      239 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/browser/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/browser/static/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1729 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/browser/static/batch_actions.js
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/browser/static/.gitkeep
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      173 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/browser/static/batch_actions.css
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18402 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/browser/views.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1121 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/browser/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3174 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/browser/viewlets.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/browser/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      986 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/browser/templates/batch_actions_viewlet.pt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/browser/overrides/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/browser/overrides/.gitkeep
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/browser/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1007 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/upgrades.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      230 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/columns.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective.eeafaceted.batchactions.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective.eeafaceted.batchactions.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective.eeafaceted.batchactions.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       33 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective.eeafaceted.batchactions.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective.eeafaceted.batchactions.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8538 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective.eeafaceted.batchactions.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3202 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective.eeafaceted.batchactions.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective.eeafaceted.batchactions.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      263 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/src/collective.eeafaceted.batchactions.egg-info/requires.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6342 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/bootstrap.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      455 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/travis.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/requirements.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2105 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    35147 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/LICENSE
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8538 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      380 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4487 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1588 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      623 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/Makefile
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/setup.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      192 2021-07-16 14:50:00.000000 collective.eeafaceted.batchactions-1.8/buildout.cfg
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.493502 collective.eeafaceted.batchactions-1.9/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4602 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/CHANGES.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)    35147 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/LICENSE
+-rw-rw-r--   0 sge       (1000) sge       (1000)      380 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/MANIFEST.in
+-rw-rw-r--   0 sge       (1000) sge       (1000)      623 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/Makefile
+-rw-rw-r--   0 sge       (1000) sge       (1000)     8701 2021-12-06 09:52:46.493502 collective.eeafaceted.batchactions-1.9/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1588 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/README.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6342 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/bootstrap.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      192 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/buildout.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)       53 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/requirements.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       38 2021-12-06 09:52:46.493502 collective.eeafaceted.batchactions-1.9/setup.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2105 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/setup.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.489502 collective.eeafaceted.batchactions-1.9/src/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.489502 collective.eeafaceted.batchactions-1.9/src/collective/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      244 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.489502 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      244 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.493502 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      239 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.493502 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/browser/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/browser/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1121 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/browser/configure.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.493502 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/browser/overrides/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/browser/overrides/.gitkeep
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.493502 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/browser/static/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/browser/static/.gitkeep
+-rw-rw-r--   0 sge       (1000) sge       (1000)      173 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/browser/static/batch_actions.css
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1729 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/browser/static/batch_actions.js
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.493502 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/browser/templates/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      986 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/browser/templates/batch_actions_viewlet.pt
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3174 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/browser/viewlets.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)    18420 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/browser/views.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      230 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/columns.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1592 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      155 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/interfaces.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.493502 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/locales/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3079 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/locales/collective.eeafaceted.batchactions.pot
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.489502 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/locales/en/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.493502 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3312 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/locales/en/LC_MESSAGES/collective.eeafaceted.batchactions.po
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.489502 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/locales/fr/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.493502 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4426 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/locales/fr/LC_MESSAGES/collective.eeafaceted.batchactions.po
+-rw-rw-r--   0 sge       (1000) sge       (1000)      548 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/locales/manual.pot
+-rwxrwxr-x   0 sge       (1000) sge       (1000)     3061 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/mk_sync_locales.sh
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.489502 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/profiles/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.493502 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/profiles/default/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/profiles/default/collectiveeeafacetedbatchactions_marker.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      352 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/profiles/default/cssregistry.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      464 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/profiles/default/jsregistry.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)       68 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/profiles/default/metadata.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.493502 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/profiles/testing/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      258 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/profiles/testing/metadata.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.493502 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/profiles/testing/types/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1915 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/profiles/testing/types/testtype.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      230 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/profiles/testing/types.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      258 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/setuphandlers.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2960 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/testing.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1589 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/testing.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.493502 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/tests/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/tests/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1006 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/tests/base.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      228 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/tests/interfaces.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4185 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/tests/test_contact_form.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     8004 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/tests/test_forms.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     5070 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/tests/test_labels_form.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3372 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/tests/test_utils.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     7456 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/tests/test_viewlets.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      979 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/tests/views.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1007 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/upgrades.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2264 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/utils.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-12-06 09:52:46.489502 collective.eeafaceted.batchactions-1.9/src/collective.eeafaceted.batchactions.egg-info/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     8701 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective.eeafaceted.batchactions.egg-info/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3202 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective.eeafaceted.batchactions.egg-info/SOURCES.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective.eeafaceted.batchactions.egg-info/dependency_links.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       53 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective.eeafaceted.batchactions.egg-info/entry_points.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       33 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective.eeafaceted.batchactions.egg-info/namespace_packages.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective.eeafaceted.batchactions.egg-info/not-zip-safe
+-rw-rw-r--   0 sge       (1000) sge       (1000)      263 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective.eeafaceted.batchactions.egg-info/requires.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       11 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/src/collective.eeafaceted.batchactions.egg-info/top_level.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      455 2021-12-06 09:52:46.000000 collective.eeafaceted.batchactions-1.9/travis.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/configure.zcml` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/locales/manual.pot` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/locales/en/LC_MESSAGES/collective.eeafaceted.batchactions.po` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/locales/en/LC_MESSAGES/collective.eeafaceted.batchactions.po`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/locales/collective.eeafaceted.batchactions.pot` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/locales/collective.eeafaceted.batchactions.pot`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/locales/fr/LC_MESSAGES/collective.eeafaceted.batchactions.po` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/locales/fr/LC_MESSAGES/collective.eeafaceted.batchactions.po`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/profiles/testing/types/testtype.xml` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/profiles/testing/types/testtype.xml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/testing.py` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/testing.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/mk_sync_locales.sh` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/mk_sync_locales.sh`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/utils.py` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/utils.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/testing.zcml` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/testing.zcml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/tests/test_utils.py` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/tests/views.py` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/tests/views.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/tests/test_forms.py` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/tests/base.py` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/tests/base.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/tests/test_contact_form.py` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/tests/test_contact_form.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/tests/test_labels_form.py` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/tests/test_labels_form.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/tests/test_viewlets.py` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/tests/test_viewlets.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/browser/static/batch_actions.js` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/browser/static/batch_actions.js`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/browser/views.py` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/browser/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,15 +381,15 @@
     available_permission = ''
     attribute = ''
     field_value_type = None
 
     def available(self):
         """Will the action be available for current context?"""
         if self.available_permission:
-            return api.user.has_permission(self.available_permission)
+            return api.user.has_permission(self.available_permission, obj=self.context)
         return True
 
     def _update(self):
         assert self.attribute
         assert self.field_value_type is not None
         self.do_apply = is_permitted(self.brains)
         self.fields += Fields(schema.Choice(
```

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/browser/configure.zcml` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/browser/viewlets.py` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/browser/templates/batch_actions_viewlet.pt` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/browser/templates/batch_actions_viewlet.pt`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective/eeafaceted/batchactions/upgrades.zcml` & `collective.eeafaceted.batchactions-1.9/src/collective/eeafaceted/batchactions/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective.eeafaceted.batchactions.egg-info/PKG-INFO` & `collective.eeafaceted.batchactions-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.eeafaceted.batchactions
-Version: 1.8
+Version: 1.9
 Summary: This package provides batch actions for eea.facetednavigation dashboard
 Home-page: https://github.com/IMIO/collective.eeafaceted.batchactions
 Author: IMIO
 Author-email: dev@imio.be
 License: GPL V2
 Download-URL: https://pypi.org/project/collective.eeafaceted.batchactions
 Description: .. image:: https://travis-ci.org/IMIO/collective.eeafaceted.batchactions.svg?branch=master
@@ -43,14 +43,20 @@
         Then, install `collective.eeafaceted.batchactions` using the Add-ons control panel.
         
         
         Changelog
         =========
         
         
+        1.9 (2021-12-06)
+        ----------------
+        
+        - Checked permission on context (in ContactBaseBatchActionForm).
+          [sgeulette]
+        
         1.8 (2021-07-16)
         ----------------
         
         - Highlight message about number of elements that will be updated
           by the action on the popup.
           [gbastien]
         
@@ -213,9 +219,9 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone :: 4.3
 Classifier: Framework :: Plone :: 5.0
 Classifier: Framework :: Plone :: 5.1
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
-Provides-Extra: test
 Provides-Extra: develop
+Provides-Extra: test
```

### Comparing `collective.eeafaceted.batchactions-1.8/src/collective.eeafaceted.batchactions.egg-info/SOURCES.txt` & `collective.eeafaceted.batchactions-1.9/src/collective.eeafaceted.batchactions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/bootstrap.py` & `collective.eeafaceted.batchactions-1.9/bootstrap.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/setup.py` & `collective.eeafaceted.batchactions-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 long_description = \
     read('README.rst') + '\n\n' + read('CHANGES.rst')
 
 setup(
     name='collective.eeafaceted.batchactions',
-    version='1.8',
+    version='1.9',
     description="This package provides batch actions for eea.facetednavigation dashboard",
     long_description=long_description,
     # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone :: 4.3",
```

### Comparing `collective.eeafaceted.batchactions-1.8/LICENSE` & `collective.eeafaceted.batchactions-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/PKG-INFO` & `collective.eeafaceted.batchactions-1.9/src/collective.eeafaceted.batchactions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.eeafaceted.batchactions
-Version: 1.8
+Version: 1.9
 Summary: This package provides batch actions for eea.facetednavigation dashboard
 Home-page: https://github.com/IMIO/collective.eeafaceted.batchactions
 Author: IMIO
 Author-email: dev@imio.be
 License: GPL V2
 Download-URL: https://pypi.org/project/collective.eeafaceted.batchactions
 Description: .. image:: https://travis-ci.org/IMIO/collective.eeafaceted.batchactions.svg?branch=master
@@ -43,14 +43,20 @@
         Then, install `collective.eeafaceted.batchactions` using the Add-ons control panel.
         
         
         Changelog
         =========
         
         
+        1.9 (2021-12-06)
+        ----------------
+        
+        - Checked permission on context (in ContactBaseBatchActionForm).
+          [sgeulette]
+        
         1.8 (2021-07-16)
         ----------------
         
         - Highlight message about number of elements that will be updated
           by the action on the popup.
           [gbastien]
         
@@ -213,9 +219,9 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone :: 4.3
 Classifier: Framework :: Plone :: 5.0
 Classifier: Framework :: Plone :: 5.1
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
-Provides-Extra: test
 Provides-Extra: develop
+Provides-Extra: test
```

### Comparing `collective.eeafaceted.batchactions-1.8/CHANGES.rst` & `collective.eeafaceted.batchactions-1.9/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 Changelog
 =========
 
 
+1.9 (2021-12-06)
+----------------
+
+- Checked permission on context (in ContactBaseBatchActionForm).
+  [sgeulette]
+
 1.8 (2021-07-16)
 ----------------
 
 - Highlight message about number of elements that will be updated
   by the action on the popup.
   [gbastien]
```

### Comparing `collective.eeafaceted.batchactions-1.8/README.rst` & `collective.eeafaceted.batchactions-1.9/README.rst`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.batchactions-1.8/Makefile` & `collective.eeafaceted.batchactions-1.9/Makefile`

 * *Files identical despite different names*

