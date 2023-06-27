# Comparing `tmp/collective.contact_behaviors-1.0.0a2.tar.gz` & `tmp/collective.contact_behaviors-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.contact_behaviors-1.0.0a2.tar", last modified: Wed Jun 21 20:08:50 2023, max compression
+gzip compressed data, was "collective.contact_behaviors-1.0.0a3.tar", last modified: Tue Jun 27 14:59:28 2023, max compression
```

## Comparing `collective.contact_behaviors-1.0.0a2.tar` & `collective.contact_behaviors-1.0.0a3.tar`

### file list

```diff
@@ -1,119 +1,123 @@
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.651363 collective.contact_behaviors-1.0.0a2/
--rw-r--r--   0 ericof     (501) staff       (20)       62 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/.coveragerc
--rw-r--r--   0 ericof     (501) staff       (20)     1342 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/.editorconfig
--rw-r--r--   0 ericof     (501) staff       (20)     1881 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/.pre-commit-config.yaml
--rw-r--r--   0 ericof     (501) staff       (20)      940 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/CHANGES.md
--rw-r--r--   0 ericof     (501) staff       (20)       49 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/CONTRIBUTORS.md
--rw-r--r--   0 ericof     (501) staff       (20)    18092 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/LICENSE.md
--rw-r--r--   0 ericof     (501) staff       (20)      179 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/MANIFEST.in
--rw-r--r--   0 ericof     (501) staff       (20)     3577 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/Makefile
--rw-r--r--   0 ericof     (501) staff       (20)     7204 2023-06-21 20:08:50.651228 collective.contact_behaviors-1.0.0a2/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     4977 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/README.md
--rw-r--r--   0 ericof     (501) staff       (20)       61 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/constraints.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.642690 collective.contact_behaviors-1.0.0a2/docs/
--rw-r--r--   0 ericof     (501) staff       (20)     3775 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/docs/logo.svg
--rw-r--r--   0 ericof     (501) staff       (20)      182 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/instance.yaml
--rw-r--r--   0 ericof     (501) staff       (20)     4598 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/pyproject.toml
--rw-r--r--   0 ericof     (501) staff       (20)       13 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/requirements.txt
--rw-r--r--   0 ericof     (501) staff       (20)       38 2023-06-21 20:08:50.651399 collective.contact_behaviors-1.0.0a2/setup.cfg
--rw-r--r--   0 ericof     (501) staff       (20)     2391 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/setup.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.639226 collective.contact_behaviors-1.0.0a2/src/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.642808 collective.contact_behaviors-1.0.0a2/src/collective/
--rw-r--r--   0 ericof     (501) staff       (20)       56 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.644310 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/
--rw-r--r--   0 ericof     (501) staff       (20)      209 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.644759 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/behaviors/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/behaviors/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     2189 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/behaviors/address_info.py
--rw-r--r--   0 ericof     (501) staff       (20)      784 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/behaviors/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     1284 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/behaviors/contact_info.py
--rw-r--r--   0 ericof     (501) staff       (20)      372 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/configure.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.645137 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/
--rw-r--r--   0 ericof     (501) staff       (20)     4391 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/collective.contact_behaviors.pot
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.639538 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/de/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.645627 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/de/LC_MESSAGES/
--rw-r--r--   0 ericof     (501) staff       (20)      458 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/de/LC_MESSAGES/collective.contact_behaviors.mo
--rw-r--r--   0 ericof     (501) staff       (20)     4260 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/de/LC_MESSAGES/collective.contact_behaviors.po
--rw-r--r--   0 ericof     (501) staff       (20)    21219 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/de/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0 ericof     (501) staff       (20)    31187 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/de/LC_MESSAGES/iso_3166-1.po
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.639647 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/es/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.646148 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/es/LC_MESSAGES/
--rw-r--r--   0 ericof     (501) staff       (20)      458 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/es/LC_MESSAGES/collective.contact_behaviors.mo
--rw-r--r--   0 ericof     (501) staff       (20)     4260 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/es/LC_MESSAGES/collective.contact_behaviors.po
--rw-r--r--   0 ericof     (501) staff       (20)    21530 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/es/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0 ericof     (501) staff       (20)    31855 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/es/LC_MESSAGES/iso_3166-1.po
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.639758 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/fi/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.646829 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/fi/LC_MESSAGES/
--rw-r--r--   0 ericof     (501) staff       (20)      458 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/fi/LC_MESSAGES/collective.contact_behaviors.mo
--rw-r--r--   0 ericof     (501) staff       (20)     4260 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/fi/LC_MESSAGES/collective.contact_behaviors.po
--rw-r--r--   0 ericof     (501) staff       (20)    20295 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/fi/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0 ericof     (501) staff       (20)    31658 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/fi/LC_MESSAGES/iso_3166-1.po
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.639871 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/fr/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.647365 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/fr/LC_MESSAGES/
--rw-r--r--   0 ericof     (501) staff       (20)      458 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/fr/LC_MESSAGES/collective.contact_behaviors.mo
--rw-r--r--   0 ericof     (501) staff       (20)     4260 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/fr/LC_MESSAGES/collective.contact_behaviors.po
--rw-r--r--   0 ericof     (501) staff       (20)    21930 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/fr/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0 ericof     (501) staff       (20)    32227 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/fr/LC_MESSAGES/iso_3166-1.po
--rw-r--r--   0 ericof     (501) staff       (20)    24314 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/iso_3166-1.pot
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.639988 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/nl/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.647884 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/nl/LC_MESSAGES/
--rw-r--r--   0 ericof     (501) staff       (20)      458 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/nl/LC_MESSAGES/collective.contact_behaviors.mo
--rw-r--r--   0 ericof     (501) staff       (20)     4260 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/nl/LC_MESSAGES/collective.contact_behaviors.po
--rw-r--r--   0 ericof     (501) staff       (20)    21277 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/nl/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0 ericof     (501) staff       (20)    31330 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/nl/LC_MESSAGES/iso_3166-1.po
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.640102 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/pt_BR/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.648393 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 ericof     (501) staff       (20)     2332 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/collective.contact_behaviors.mo
--rw-r--r--   0 ericof     (501) staff       (20)     4866 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/collective.contact_behaviors.po
--rw-r--r--   0 ericof     (501) staff       (20)    21844 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0 ericof     (501) staff       (20)    32044 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/iso_3166-1.po
--rw-r--r--   0 ericof     (501) staff       (20)     3901 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/update.py
--rw-r--r--   0 ericof     (501) staff       (20)      752 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/permissions.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.640521 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.648750 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles/default/
--rw-r--r--   0 ericof     (501) staff       (20)      341 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles/default/catalog.xml
--rw-r--r--   0 ericof     (501) staff       (20)      107 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles/default/metadata.xml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.648895 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles/default/registry/
--rw-r--r--   0 ericof     (501) staff       (20)      891 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles/default/registry/plone.app.querystring.interfaces.IQueryField.xml
--rw-r--r--   0 ericof     (501) staff       (20)     1061 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles/default/rolemap.xml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.649014 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles/testing/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.649142 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles/testing/registry/
--rw-r--r--   0 ericof     (501) staff       (20)      457 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles/testing/registry/plone.i18n.interfaces.ILanguageSchema.xml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.649262 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles/testing/types/
--rw-r--r--   0 ericof     (501) staff       (20)     3357 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles/testing/types/Content.xml
--rw-r--r--   0 ericof     (501) staff       (20)      182 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles/testing/types.xml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.649371 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles/uninstall/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles/uninstall/.gitkeep
--rw-r--r--   0 ericof     (501) staff       (20)     1033 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles.zcml
--rw-r--r--   0 ericof     (501) staff       (20)      998 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/testing.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.649559 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/upgrades/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/upgrades/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      140 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/upgrades/configure.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.649882 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/vocabularies/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/vocabularies/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      332 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/vocabularies/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     1156 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/vocabularies/countries.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.643736 collective.contact_behaviors-1.0.0a2/src/collective.contact_behaviors.egg-info/
--rw-r--r--   0 ericof     (501) staff       (20)     7204 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective.contact_behaviors.egg-info/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     4517 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective.contact_behaviors.egg-info/SOURCES.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective.contact_behaviors.egg-info/dependency_links.txt
--rw-r--r--   0 ericof     (501) staff       (20)      133 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective.contact_behaviors.egg-info/entry_points.txt
--rw-r--r--   0 ericof     (501) staff       (20)       11 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective.contact_behaviors.egg-info/namespace_packages.txt
--rw-r--r--   0 ericof     (501) staff       (20)      178 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective.contact_behaviors.egg-info/requires.txt
--rw-r--r--   0 ericof     (501) staff       (20)       11 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective.contact_behaviors.egg-info/top_level.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/src/collective.contact_behaviors.egg-info/zip-safe
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.649988 collective.contact_behaviors-1.0.0a2/tests/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.650240 collective.contact_behaviors-1.0.0a2/tests/behaviors/
--rw-r--r--   0 ericof     (501) staff       (20)     1119 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/tests/behaviors/test_behavior_address_info.py
--rw-r--r--   0 ericof     (501) staff       (20)     1242 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/tests/behaviors/test_behavior_contact_info.py
--rw-r--r--   0 ericof     (501) staff       (20)     2139 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/tests/conftest.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.650691 collective.contact_behaviors-1.0.0a2/tests/restapi/
--rw-r--r--   0 ericof     (501) staff       (20)     1541 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/tests/restapi/conftest.py
--rw-r--r--   0 ericof     (501) staff       (20)      962 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/tests/restapi/test_restapi_address_info_permissions.py
--rw-r--r--   0 ericof     (501) staff       (20)      929 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/tests/restapi/test_restapi_contact_info_permissions.py
--rw-r--r--   0 ericof     (501) staff       (20)     3706 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/tests/restapi/test_restapi_vocab_countries.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.650927 collective.contact_behaviors-1.0.0a2/tests/setup/
--rw-r--r--   0 ericof     (501) staff       (20)      380 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/tests/setup/test_setup_install.py
--rw-r--r--   0 ericof     (501) staff       (20)      415 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/tests/setup/test_setup_uninstall.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-21 20:08:50.651041 collective.contact_behaviors-1.0.0a2/tests/vocabularies/
--rw-r--r--   0 ericof     (501) staff       (20)     2415 2023-06-21 20:08:50.000000 collective.contact_behaviors-1.0.0a2/tests/vocabularies/test_vocab_countries.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.887863 collective.contact_behaviors-1.0.0a3/
+-rw-r--r--   0 ericof     (501) staff       (20)       62 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/.coveragerc
+-rw-r--r--   0 ericof     (501) staff       (20)     1342 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/.editorconfig
+-rw-r--r--   0 ericof     (501) staff       (20)     1881 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/.pre-commit-config.yaml
+-rw-r--r--   0 ericof     (501) staff       (20)     1064 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/CHANGES.md
+-rw-r--r--   0 ericof     (501) staff       (20)       49 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/CONTRIBUTORS.md
+-rw-r--r--   0 ericof     (501) staff       (20)    18092 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/LICENSE.md
+-rw-r--r--   0 ericof     (501) staff       (20)      179 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/MANIFEST.in
+-rw-r--r--   0 ericof     (501) staff       (20)     3577 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/Makefile
+-rw-r--r--   0 ericof     (501) staff       (20)     7328 2023-06-27 14:59:28.887740 collective.contact_behaviors-1.0.0a3/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     4977 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/README.md
+-rw-r--r--   0 ericof     (501) staff       (20)       61 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/constraints.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.878821 collective.contact_behaviors-1.0.0a3/docs/
+-rw-r--r--   0 ericof     (501) staff       (20)     3775 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/docs/logo.svg
+-rw-r--r--   0 ericof     (501) staff       (20)      182 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/instance.yaml
+-rw-r--r--   0 ericof     (501) staff       (20)     4598 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/pyproject.toml
+-rw-r--r--   0 ericof     (501) staff       (20)       13 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/requirements.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       38 2023-06-27 14:59:28.887895 collective.contact_behaviors-1.0.0a3/setup.cfg
+-rw-r--r--   0 ericof     (501) staff       (20)     2391 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/setup.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.875215 collective.contact_behaviors-1.0.0a3/src/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.878932 collective.contact_behaviors-1.0.0a3/src/collective/
+-rw-r--r--   0 ericof     (501) staff       (20)       56 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.880549 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/
+-rw-r--r--   0 ericof     (501) staff       (20)      209 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.880993 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/behaviors/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/behaviors/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2735 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/behaviors/address_info.py
+-rw-r--r--   0 ericof     (501) staff       (20)      784 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/behaviors/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1284 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/behaviors/contact_info.py
+-rw-r--r--   0 ericof     (501) staff       (20)      372 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)      485 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/interfaces.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.881367 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/
+-rw-r--r--   0 ericof     (501) staff       (20)     4391 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/collective.contact_behaviors.pot
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.875540 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/de/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.881865 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/de/LC_MESSAGES/
+-rw-r--r--   0 ericof     (501) staff       (20)      458 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/de/LC_MESSAGES/collective.contact_behaviors.mo
+-rw-r--r--   0 ericof     (501) staff       (20)     4260 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/de/LC_MESSAGES/collective.contact_behaviors.po
+-rw-r--r--   0 ericof     (501) staff       (20)    21219 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/de/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0 ericof     (501) staff       (20)    31187 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/de/LC_MESSAGES/iso_3166-1.po
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.875653 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/es/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.882380 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/es/LC_MESSAGES/
+-rw-r--r--   0 ericof     (501) staff       (20)      458 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/es/LC_MESSAGES/collective.contact_behaviors.mo
+-rw-r--r--   0 ericof     (501) staff       (20)     4260 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/es/LC_MESSAGES/collective.contact_behaviors.po
+-rw-r--r--   0 ericof     (501) staff       (20)    21530 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/es/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0 ericof     (501) staff       (20)    31855 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/es/LC_MESSAGES/iso_3166-1.po
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.875764 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/fi/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.882882 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/fi/LC_MESSAGES/
+-rw-r--r--   0 ericof     (501) staff       (20)      458 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/fi/LC_MESSAGES/collective.contact_behaviors.mo
+-rw-r--r--   0 ericof     (501) staff       (20)     4260 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/fi/LC_MESSAGES/collective.contact_behaviors.po
+-rw-r--r--   0 ericof     (501) staff       (20)    20295 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/fi/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0 ericof     (501) staff       (20)    31658 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/fi/LC_MESSAGES/iso_3166-1.po
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.875877 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/fr/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.883403 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 ericof     (501) staff       (20)      458 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/fr/LC_MESSAGES/collective.contact_behaviors.mo
+-rw-r--r--   0 ericof     (501) staff       (20)     4260 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/fr/LC_MESSAGES/collective.contact_behaviors.po
+-rw-r--r--   0 ericof     (501) staff       (20)    21930 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/fr/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0 ericof     (501) staff       (20)    32227 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/fr/LC_MESSAGES/iso_3166-1.po
+-rw-r--r--   0 ericof     (501) staff       (20)    24314 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/iso_3166-1.pot
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.876006 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/nl/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.883898 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 ericof     (501) staff       (20)      458 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/nl/LC_MESSAGES/collective.contact_behaviors.mo
+-rw-r--r--   0 ericof     (501) staff       (20)     4260 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/nl/LC_MESSAGES/collective.contact_behaviors.po
+-rw-r--r--   0 ericof     (501) staff       (20)    21277 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/nl/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0 ericof     (501) staff       (20)    31330 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/nl/LC_MESSAGES/iso_3166-1.po
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.876124 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/pt_BR/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.884413 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 ericof     (501) staff       (20)     2332 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/collective.contact_behaviors.mo
+-rw-r--r--   0 ericof     (501) staff       (20)     4866 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/collective.contact_behaviors.po
+-rw-r--r--   0 ericof     (501) staff       (20)    21844 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0 ericof     (501) staff       (20)    32044 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/iso_3166-1.po
+-rw-r--r--   0 ericof     (501) staff       (20)     3901 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/update.py
+-rw-r--r--   0 ericof     (501) staff       (20)      752 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/permissions.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.876561 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.884775 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/default/
+-rw-r--r--   0 ericof     (501) staff       (20)      341 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/default/catalog.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      107 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/default/metadata.xml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.885022 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/default/registry/
+-rw-r--r--   0 ericof     (501) staff       (20)      363 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/default/registry/collective.contact_behaviors.interfaces.IContactBehaviors.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      891 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/default/registry/plone.app.querystring.interfaces.IQueryField.xml
+-rw-r--r--   0 ericof     (501) staff       (20)     1061 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/default/rolemap.xml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.885141 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/testing/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.885404 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/testing/registry/
+-rw-r--r--   0 ericof     (501) staff       (20)      379 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/testing/registry/collective.contact_behaviors.interfaces.IContactBehaviors.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      457 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/testing/registry/plone.i18n.interfaces.ILanguageSchema.xml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.885545 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/testing/types/
+-rw-r--r--   0 ericof     (501) staff       (20)     3357 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/testing/types/Content.xml
+-rw-r--r--   0 ericof     (501) staff       (20)      182 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/testing/types.xml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.885679 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/uninstall/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/uninstall/.gitkeep
+-rw-r--r--   0 ericof     (501) staff       (20)     1033 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)      998 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/testing.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.885908 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/upgrades/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/upgrades/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      444 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/upgrades/configure.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.886219 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/vocabularies/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/vocabularies/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      332 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/vocabularies/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1156 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/vocabularies/countries.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.879856 collective.contact_behaviors-1.0.0a3/src/collective.contact_behaviors.egg-info/
+-rw-r--r--   0 ericof     (501) staff       (20)     7328 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective.contact_behaviors.egg-info/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     4864 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective.contact_behaviors.egg-info/SOURCES.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective.contact_behaviors.egg-info/dependency_links.txt
+-rw-r--r--   0 ericof     (501) staff       (20)      133 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective.contact_behaviors.egg-info/entry_points.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       11 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective.contact_behaviors.egg-info/namespace_packages.txt
+-rw-r--r--   0 ericof     (501) staff       (20)      178 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective.contact_behaviors.egg-info/requires.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       11 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective.contact_behaviors.egg-info/top_level.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/src/collective.contact_behaviors.egg-info/zip-safe
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.886335 collective.contact_behaviors-1.0.0a3/tests/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.886575 collective.contact_behaviors-1.0.0a3/tests/behaviors/
+-rw-r--r--   0 ericof     (501) staff       (20)     1119 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/tests/behaviors/test_behavior_address_info.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1242 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/tests/behaviors/test_behavior_contact_info.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2139 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/tests/conftest.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.887173 collective.contact_behaviors-1.0.0a3/tests/restapi/
+-rw-r--r--   0 ericof     (501) staff       (20)     1533 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/tests/restapi/conftest.py
+-rw-r--r--   0 ericof     (501) staff       (20)      479 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/tests/restapi/test_restapi_address_info_default_values.py
+-rw-r--r--   0 ericof     (501) staff       (20)      962 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/tests/restapi/test_restapi_address_info_permissions.py
+-rw-r--r--   0 ericof     (501) staff       (20)      929 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/tests/restapi/test_restapi_contact_info_permissions.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3706 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/tests/restapi/test_restapi_vocab_countries.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.887418 collective.contact_behaviors-1.0.0a3/tests/setup/
+-rw-r--r--   0 ericof     (501) staff       (20)      380 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/tests/setup/test_setup_install.py
+-rw-r--r--   0 ericof     (501) staff       (20)      415 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/tests/setup/test_setup_uninstall.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-27 14:59:28.887539 collective.contact_behaviors-1.0.0a3/tests/vocabularies/
+-rw-r--r--   0 ericof     (501) staff       (20)     2415 2023-06-27 14:59:28.000000 collective.contact_behaviors-1.0.0a3/tests/vocabularies/test_vocab_countries.py
```

### Comparing `collective.contact_behaviors-1.0.0a2/.editorconfig` & `collective.contact_behaviors-1.0.0a3/.editorconfig`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/.pre-commit-config.yaml` & `collective.contact_behaviors-1.0.0a3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/CHANGES.md` & `collective.contact_behaviors-1.0.0a3/CHANGES.md`

 * *Files 27% similar despite different names*

```diff
@@ -5,14 +5,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a3 (2023-06-27)
+
+
+### New features:
+
+- Allow other packages to set default values for address fields [@ericof] #2
+
+
 ## 1.0.0a2 (2023-06-21)
 
 
 ### New features:
 
 - Implement `collective.contact_behaviors.address_info behavior` @ericof address
 - Implement `collective.contact_behaviors.contact_info behavior` @ericof contact
```

### Comparing `collective.contact_behaviors-1.0.0a2/LICENSE.md` & `collective.contact_behaviors-1.0.0a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/Makefile` & `collective.contact_behaviors-1.0.0a3/Makefile`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/PKG-INFO` & `collective.contact_behaviors-1.0.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.contact_behaviors
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: A collection of contact information behaviors and vocabularies for Dexterity content types.
 Home-page: https://github.com/collective/collective.contact_behaviors
 Author: Plone Community
 Author-email: ericof@plone.org
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.contact_behaviors
 Project-URL: Source, https://github.com/collective/collective.contact_behaviors
@@ -185,14 +185,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a3 (2023-06-27)
+
+
+### New features:
+
+- Allow other packages to set default values for address fields [@ericof] #2
+
+
 ## 1.0.0a2 (2023-06-21)
 
 
 ### New features:
 
 - Implement `collective.contact_behaviors.address_info behavior` @ericof address
 - Implement `collective.contact_behaviors.contact_info behavior` @ericof contact
```

### Comparing `collective.contact_behaviors-1.0.0a2/README.md` & `collective.contact_behaviors-1.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/docs/logo.svg` & `collective.contact_behaviors-1.0.0a3/docs/logo.svg`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/pyproject.toml` & `collective.contact_behaviors-1.0.0a3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/setup.py` & `collective.contact_behaviors-1.0.0a3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "A collection of contact information behaviors and vocabularies "
     "for Dexterity content types."
 )
 
 
 setup(
     name="collective.contact_behaviors",
-    version="1.0.0a2",
+    version="1.0.0a3",
     description=short_description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/behaviors/configure.zcml` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/behaviors/contact_info.py` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/behaviors/contact_info.py`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/collective.contact_behaviors.pot` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/collective.contact_behaviors.pot`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/de/LC_MESSAGES/collective.contact_behaviors.po` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/de/LC_MESSAGES/collective.contact_behaviors.po`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/de/LC_MESSAGES/iso_3166-1.mo` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/de/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/de/LC_MESSAGES/iso_3166-1.po` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/de/LC_MESSAGES/iso_3166-1.po`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/es/LC_MESSAGES/collective.contact_behaviors.po` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/es/LC_MESSAGES/collective.contact_behaviors.po`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/es/LC_MESSAGES/iso_3166-1.mo` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/es/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/es/LC_MESSAGES/iso_3166-1.po` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/es/LC_MESSAGES/iso_3166-1.po`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/fi/LC_MESSAGES/collective.contact_behaviors.po` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/fi/LC_MESSAGES/collective.contact_behaviors.po`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/fi/LC_MESSAGES/iso_3166-1.mo` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/fi/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/fi/LC_MESSAGES/iso_3166-1.po` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/fi/LC_MESSAGES/iso_3166-1.po`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/fr/LC_MESSAGES/collective.contact_behaviors.po` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/fr/LC_MESSAGES/collective.contact_behaviors.po`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/fr/LC_MESSAGES/iso_3166-1.mo` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/fr/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/fr/LC_MESSAGES/iso_3166-1.po` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/fr/LC_MESSAGES/iso_3166-1.po`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/iso_3166-1.pot` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/iso_3166-1.pot`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/nl/LC_MESSAGES/collective.contact_behaviors.po` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/nl/LC_MESSAGES/collective.contact_behaviors.po`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/nl/LC_MESSAGES/iso_3166-1.mo` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/nl/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/nl/LC_MESSAGES/iso_3166-1.po` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/nl/LC_MESSAGES/iso_3166-1.po`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/collective.contact_behaviors.mo` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/collective.contact_behaviors.mo`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/collective.contact_behaviors.po` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/collective.contact_behaviors.po`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/iso_3166-1.mo` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/iso_3166-1.po` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/iso_3166-1.po`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/locales/update.py` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/permissions.zcml` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/permissions.zcml`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles/default/registry/plone.app.querystring.interfaces.IQueryField.xml` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/default/registry/plone.app.querystring.interfaces.IQueryField.xml`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles/default/rolemap.xml` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles/testing/types/Content.xml` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles/testing/types/Content.xml`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/profiles.zcml` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/profiles.zcml`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/testing.py` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/testing.py`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective/contact_behaviors/vocabularies/countries.py` & `collective.contact_behaviors-1.0.0a3/src/collective/contact_behaviors/vocabularies/countries.py`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective.contact_behaviors.egg-info/PKG-INFO` & `collective.contact_behaviors-1.0.0a3/src/collective.contact_behaviors.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.contact-behaviors
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: A collection of contact information behaviors and vocabularies for Dexterity content types.
 Home-page: https://github.com/collective/collective.contact_behaviors
 Author: Plone Community
 Author-email: ericof@plone.org
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.contact_behaviors
 Project-URL: Source, https://github.com/collective/collective.contact_behaviors
@@ -185,14 +185,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a3 (2023-06-27)
+
+
+### New features:
+
+- Allow other packages to set default values for address fields [@ericof] #2
+
+
 ## 1.0.0a2 (2023-06-21)
 
 
 ### New features:
 
 - Implement `collective.contact_behaviors.address_info behavior` @ericof address
 - Implement `collective.contact_behaviors.contact_info behavior` @ericof contact
```

### Comparing `collective.contact_behaviors-1.0.0a2/src/collective.contact_behaviors.egg-info/SOURCES.txt` & `collective.contact_behaviors-1.0.0a3/src/collective.contact_behaviors.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 src/collective.contact_behaviors.egg-info/entry_points.txt
 src/collective.contact_behaviors.egg-info/namespace_packages.txt
 src/collective.contact_behaviors.egg-info/requires.txt
 src/collective.contact_behaviors.egg-info/top_level.txt
 src/collective.contact_behaviors.egg-info/zip-safe
 src/collective/contact_behaviors/__init__.py
 src/collective/contact_behaviors/configure.zcml
+src/collective/contact_behaviors/interfaces.py
 src/collective/contact_behaviors/permissions.zcml
 src/collective/contact_behaviors/profiles.zcml
 src/collective/contact_behaviors/testing.py
 src/collective/contact_behaviors/behaviors/__init__.py
 src/collective/contact_behaviors/behaviors/address_info.py
 src/collective/contact_behaviors/behaviors/configure.zcml
 src/collective/contact_behaviors/behaviors/contact_info.py
@@ -57,27 +58,30 @@
 src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/collective.contact_behaviors.mo
 src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/collective.contact_behaviors.po
 src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/iso_3166-1.mo
 src/collective/contact_behaviors/locales/pt_BR/LC_MESSAGES/iso_3166-1.po
 src/collective/contact_behaviors/profiles/default/catalog.xml
 src/collective/contact_behaviors/profiles/default/metadata.xml
 src/collective/contact_behaviors/profiles/default/rolemap.xml
+src/collective/contact_behaviors/profiles/default/registry/collective.contact_behaviors.interfaces.IContactBehaviors.xml
 src/collective/contact_behaviors/profiles/default/registry/plone.app.querystring.interfaces.IQueryField.xml
 src/collective/contact_behaviors/profiles/testing/types.xml
+src/collective/contact_behaviors/profiles/testing/registry/collective.contact_behaviors.interfaces.IContactBehaviors.xml
 src/collective/contact_behaviors/profiles/testing/registry/plone.i18n.interfaces.ILanguageSchema.xml
 src/collective/contact_behaviors/profiles/testing/types/Content.xml
 src/collective/contact_behaviors/profiles/uninstall/.gitkeep
 src/collective/contact_behaviors/upgrades/__init__.py
 src/collective/contact_behaviors/upgrades/configure.zcml
 src/collective/contact_behaviors/vocabularies/__init__.py
 src/collective/contact_behaviors/vocabularies/configure.zcml
 src/collective/contact_behaviors/vocabularies/countries.py
 tests/conftest.py
 tests/behaviors/test_behavior_address_info.py
 tests/behaviors/test_behavior_contact_info.py
 tests/restapi/conftest.py
+tests/restapi/test_restapi_address_info_default_values.py
 tests/restapi/test_restapi_address_info_permissions.py
 tests/restapi/test_restapi_contact_info_permissions.py
 tests/restapi/test_restapi_vocab_countries.py
 tests/setup/test_setup_install.py
 tests/setup/test_setup_uninstall.py
 tests/vocabularies/test_vocab_countries.py
```

### Comparing `collective.contact_behaviors-1.0.0a2/tests/behaviors/test_behavior_address_info.py` & `collective.contact_behaviors-1.0.0a3/tests/behaviors/test_behavior_address_info.py`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/tests/behaviors/test_behavior_contact_info.py` & `collective.contact_behaviors-1.0.0a3/tests/behaviors/test_behavior_contact_info.py`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/tests/conftest.py` & `collective.contact_behaviors-1.0.0a3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/tests/restapi/conftest.py` & `collective.contact_behaviors-1.0.0a3/tests/restapi/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 def app(functional):
     return functional["app"]
 
 
 @pytest.fixture()
 def portal(functional, contents_payload):
     portal = functional["portal"]
+    # Create Content
     with api.env.adopt_user(SITE_OWNER_NAME):
-        # Create Content
         content = _create_content(portal, contents_payload[0])
+    # Publish Content
     with api.env.adopt_user(SITE_OWNER_NAME):
-        # Publish Content
         _publish_content(content)
 
     transaction.commit()
     return portal
 
 
 @pytest.fixture()
```

### Comparing `collective.contact_behaviors-1.0.0a2/tests/restapi/test_restapi_address_info_permissions.py` & `collective.contact_behaviors-1.0.0a3/tests/restapi/test_restapi_address_info_permissions.py`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/tests/restapi/test_restapi_contact_info_permissions.py` & `collective.contact_behaviors-1.0.0a3/tests/restapi/test_restapi_contact_info_permissions.py`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/tests/restapi/test_restapi_vocab_countries.py` & `collective.contact_behaviors-1.0.0a3/tests/restapi/test_restapi_vocab_countries.py`

 * *Files identical despite different names*

### Comparing `collective.contact_behaviors-1.0.0a2/tests/vocabularies/test_vocab_countries.py` & `collective.contact_behaviors-1.0.0a3/tests/vocabularies/test_vocab_countries.py`

 * *Files identical despite different names*

