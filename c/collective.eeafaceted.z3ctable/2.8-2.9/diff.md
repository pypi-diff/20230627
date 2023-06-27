# Comparing `tmp/collective.eeafaceted.z3ctable-2.8.tar.gz` & `tmp/collective.eeafaceted.z3ctable-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.eeafaceted.z3ctable-2.8.tar", last modified: Thu Feb  6 09:10:33 2020, max compression
+gzip compressed data, was "dist/collective.eeafaceted.z3ctable-2.9.tar", last modified: Tue Feb 25 09:26:55 2020, max compression
```

## Comparing `collective.eeafaceted.z3ctable-2.8.tar` & `collective.eeafaceted.z3ctable-2.9.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1526 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/LICENSE.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1085 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13521 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/PKG-INFO
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      234 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/__init__.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3057 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/mk_sync_locales.sh
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/common/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      170 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/common/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/common/collectiveeeafacetedz3ctable_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      194 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/common/browserlayer.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      384 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/testing/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      232 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/testing/types.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/testing/types/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1975 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/testing/types/testingtype.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/plone4/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      248 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/plone4/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      453 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/plone4/jsregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/plone4/collectiveeeafacetedz3ctable_marker.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/plone5/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      181 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/plone5/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1039 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/plone5/registry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/plone5/collectiveeeafacetedz3ctable_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1222 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/testing.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4255 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1128 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/interfaces.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3283 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/columns.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4299 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/tests/test_table.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2128 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/tests/test_setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1281 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/tests/vocabularies.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      223 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/tests/views.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    34560 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/tests/test_columns.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      633 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/tests/test_robot.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/tests/robot/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/tests/robot/.gitkeep
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    29178 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/columns.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      254 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/setuphandlers.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2376 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      956 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/overrides/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/overrides/.gitkeep
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7005 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/views.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      887 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/default_collection.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2630 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/faceted-table-items.pt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/static/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      726 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/static/collective.eeafaceted.z3ctable.js
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/static/.gitkeep
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      256 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/static/refresh.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2617 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      691 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/jsvariables.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1858 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/widgets.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1721 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/overrides.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2865 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/locales/collective.eeafaceted.z3ctable.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2179 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/locales/manual.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3176 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/locales/en/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/locales/en/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2966 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/locales/en/LC_MESSAGES/collective.eeafaceted.z3ctable.po
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective.eeafaceted.z3ctable.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective.eeafaceted.z3ctable.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13521 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective.eeafaceted.z3ctable.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective.eeafaceted.z3ctable.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3479 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective.eeafaceted.z3ctable.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       33 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective.eeafaceted.z3ctable.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective.eeafaceted.z3ctable.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      248 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective.eeafaceted.z3ctable.egg-info/requires.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/src/collective.eeafaceted.z3ctable.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      350 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      125 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/travis.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/setup.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1815 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7458 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/bootstrap.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9139 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      195 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/buildout.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      665 2020-02-06 09:10:33.000000 collective.eeafaceted.z3ctable-2.8/Makefile
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       38 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/setup.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)    13671 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)      125 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/travis.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1815 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/setup.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      195 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/buildout.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     7458 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/bootstrap.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1085 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/README.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)      665 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/Makefile
+-rw-rw-r--   0 sge       (1000) sge       (1000)      350 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/MANIFEST.in
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1526 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/LICENSE.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)     9233 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/CHANGES.rst
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective.eeafaceted.z3ctable.egg-info/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       11 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective.eeafaceted.z3ctable.egg-info/top_level.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      248 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective.eeafaceted.z3ctable.egg-info/requires.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective.eeafaceted.z3ctable.egg-info/not-zip-safe
+-rw-rw-r--   0 sge       (1000) sge       (1000)       33 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective.eeafaceted.z3ctable.egg-info/namespace_packages.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       53 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective.eeafaceted.z3ctable.egg-info/entry_points.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective.eeafaceted.z3ctable.egg-info/dependency_links.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3479 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective.eeafaceted.z3ctable.egg-info/SOURCES.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)    13671 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective.eeafaceted.z3ctable.egg-info/PKG-INFO
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      244 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      244 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1222 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/testing.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4255 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/testing.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      254 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/setuphandlers.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2376 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles.zcml
+-rwxrwxr-x   0 sge       (1000) sge       (1000)     3057 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/mk_sync_locales.sh
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1128 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/interfaces.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      956 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3283 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/columns.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)    29242 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/columns.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      234 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/tests/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1281 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/tests/vocabularies.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      223 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/tests/views.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4299 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/tests/test_table.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2128 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/tests/test_setup.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      633 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/tests/test_robot.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)    34560 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/tests/test_columns.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/tests/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/tests/robot/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/tests/robot/.gitkeep
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/testing/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      232 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/testing/types.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      384 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/testing/metadata.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/testing/types/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1975 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/testing/types/testingtype.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/plone5/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1039 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/plone5/registry.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      181 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/plone5/metadata.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/plone5/collectiveeeafacetedz3ctable_marker.txt
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/plone4/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      248 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/plone4/metadata.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      453 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/plone4/jsregistry.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/plone4/collectiveeeafacetedz3ctable_marker.txt
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/common/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      170 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/common/metadata.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/common/collectiveeeafacetedz3ctable_marker.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      194 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/common/browserlayer.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/locales/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2179 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/locales/manual.pot
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2865 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/locales/collective.eeafaceted.z3ctable.pot
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/locales/fr/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3176 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/locales/en/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2966 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/locales/en/LC_MESSAGES/collective.eeafaceted.z3ctable.po
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1858 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/widgets.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     7005 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/views.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1721 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/overrides.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      691 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/jsvariables.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2630 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/faceted-table-items.pt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      887 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/default_collection.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2617 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/static/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      256 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/static/refresh.gif
+-rw-rw-r--   0 sge       (1000) sge       (1000)      726 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/static/collective.eeafaceted.z3ctable.js
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/static/.gitkeep
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:55.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/overrides/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2020-02-25 09:26:54.000000 collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/overrides/.gitkeep
```

### Comparing `collective.eeafaceted.z3ctable-2.8/LICENSE.rst` & `collective.eeafaceted.z3ctable-2.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/README.rst` & `collective.eeafaceted.z3ctable-2.9/README.rst`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/PKG-INFO` & `collective.eeafaceted.z3ctable-2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.eeafaceted.z3ctable
-Version: 2.8
+Version: 2.9
 Summary: Package proposant un type de colonne compatible avec eea.facetednavigation
 Home-page: http://pypi.python.org/pypi/collective.eeafaceted.z3ctable
 Author: IMIO
 Author-email: dev@imio.be
 License: GPL V2
 Description: .. image:: https://travis-ci.org/collective/collective.eeafaceted.z3ctable.svg?branch=master
            :target: https://travis-ci.org/collective/collective.eeafaceted.z3ctable
@@ -30,14 +30,21 @@
         to the list of eggs in your buildout, run buildout and restart Plone.
         Then, install `collective.eeafaceted.z3ctable` using the Add-ons control panel.
         
         Changelog
         =========
         
         
+        2.9 (2020-02-25)
+        ----------------
+        
+        - Ignored EMPTY_STRING in VocabularyColumn
+          [sgeulette]
+        
+        
         2.8 (2020-02-06)
         ----------------
         
         - Managed correctly a field not yet set.
           [sgeulette]
         - In the `PrettyLinkWithAdditionalInfosColumn`, manage `description` manually
           as it is not present in the `@@view` widgets.
```

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/mk_sync_locales.sh` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/mk_sync_locales.sh`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/testing/types/testingtype.xml` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/testing/types/testingtype.xml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles/plone5/registry.xml` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles/plone5/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/testing.zcml` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/testing.zcml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/testing.py` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/testing.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/interfaces.py` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/columns.zcml` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/columns.zcml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/tests/test_table.py` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/tests/test_setup.py` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/tests/vocabularies.py` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/tests/vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/tests/test_columns.py` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/tests/test_columns.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/tests/test_robot.py` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/columns.py` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/columns.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,18 +346,19 @@
 
 
 class VocabularyColumn(BaseColumn):
     """A column that is aware of a vocabulary and that will get value to display from it."""
 
     # named utility
     vocabulary = None
+    ignored_value = EMPTY_STRING
 
     def renderCell(self, item):
         value = self.getValue(item)
-        if not value:
+        if not value or value == self.ignored_value:
             return u'-'
 
         # caching when several same values in same column
         if self.use_caching:
             res = self._get_cached_result(value)
             if res:
                 return res
```

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/profiles.zcml` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/profiles.zcml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/configure.zcml` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/views.py` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/views.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/default_collection.xml` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/default_collection.xml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/faceted-table-items.pt` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/faceted-table-items.pt`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/static/collective.eeafaceted.z3ctable.js` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/static/collective.eeafaceted.z3ctable.js`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/configure.zcml` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/jsvariables.py` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/jsvariables.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/widgets.py` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/widgets.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/browser/overrides.py` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/browser/overrides.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/locales/collective.eeafaceted.z3ctable.pot` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/locales/collective.eeafaceted.z3ctable.pot`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/locales/manual.pot` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective/eeafaceted/z3ctable/locales/en/LC_MESSAGES/collective.eeafaceted.z3ctable.po` & `collective.eeafaceted.z3ctable-2.9/src/collective/eeafaceted/z3ctable/locales/en/LC_MESSAGES/collective.eeafaceted.z3ctable.po`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective.eeafaceted.z3ctable.egg-info/PKG-INFO` & `collective.eeafaceted.z3ctable-2.9/src/collective.eeafaceted.z3ctable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.eeafaceted.z3ctable
-Version: 2.8
+Version: 2.9
 Summary: Package proposant un type de colonne compatible avec eea.facetednavigation
 Home-page: http://pypi.python.org/pypi/collective.eeafaceted.z3ctable
 Author: IMIO
 Author-email: dev@imio.be
 License: GPL V2
 Description: .. image:: https://travis-ci.org/collective/collective.eeafaceted.z3ctable.svg?branch=master
            :target: https://travis-ci.org/collective/collective.eeafaceted.z3ctable
@@ -30,14 +30,21 @@
         to the list of eggs in your buildout, run buildout and restart Plone.
         Then, install `collective.eeafaceted.z3ctable` using the Add-ons control panel.
         
         Changelog
         =========
         
         
+        2.9 (2020-02-25)
+        ----------------
+        
+        - Ignored EMPTY_STRING in VocabularyColumn
+          [sgeulette]
+        
+        
         2.8 (2020-02-06)
         ----------------
         
         - Managed correctly a field not yet set.
           [sgeulette]
         - In the `PrettyLinkWithAdditionalInfosColumn`, manage `description` manually
           as it is not present in the `@@view` widgets.
```

### Comparing `collective.eeafaceted.z3ctable-2.8/src/collective.eeafaceted.z3ctable.egg-info/SOURCES.txt` & `collective.eeafaceted.z3ctable-2.9/src/collective.eeafaceted.z3ctable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/setup.py` & `collective.eeafaceted.z3ctable-2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 long_description = \
     read('README.rst') + \
     read('CHANGES.rst')
 
 setup(
     name='collective.eeafaceted.z3ctable',
-    version='2.8',
+    version='2.9',
     description="Package proposant un type de colonne compatible avec eea.facetednavigation",
     long_description=long_description,
     # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone :: 4.3",
         "Framework :: Plone :: 5.0",
```

### Comparing `collective.eeafaceted.z3ctable-2.8/bootstrap.py` & `collective.eeafaceted.z3ctable-2.9/bootstrap.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.z3ctable-2.8/CHANGES.rst` & `collective.eeafaceted.z3ctable-2.9/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+2.9 (2020-02-25)
+----------------
+
+- Ignored EMPTY_STRING in VocabularyColumn
+  [sgeulette]
+
+
 2.8 (2020-02-06)
 ----------------
 
 - Managed correctly a field not yet set.
   [sgeulette]
 - In the `PrettyLinkWithAdditionalInfosColumn`, manage `description` manually
   as it is not present in the `@@view` widgets.
```

### Comparing `collective.eeafaceted.z3ctable-2.8/Makefile` & `collective.eeafaceted.z3ctable-2.9/Makefile`

 * *Files identical despite different names*

