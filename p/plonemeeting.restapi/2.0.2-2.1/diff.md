# Comparing `tmp/plonemeeting.restapi-2.0.2.tar.gz` & `tmp/plonemeeting.restapi-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plonemeeting.restapi-2.0.2.tar", last modified: Wed May 31 08:59:30 2023, max compression
+gzip compressed data, was "dist/plonemeeting.restapi-2.1.tar", last modified: Tue Jun 27 10:25:27 2023, max compression
```

## Comparing `plonemeeting.restapi-2.0.2.tar` & `plonemeeting.restapi-2.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      657 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/LICENSE.rst
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      272 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/setuphandlers.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3192 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/get.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      725 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/users.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15679 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/add.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4315 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1667 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/meetingconfig.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6723 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/search.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1469 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/annex.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11176 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/attendees.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1372 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/infos.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1531 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      475 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/imio.history.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/en/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/en/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      575 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/en/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      609 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/en/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      434 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/plone.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      609 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      667 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/imio.history.po
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      332 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/sync_pos.sh
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/profiles/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      256 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/profiles/testing/metadata.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      176 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/profiles/default/browserlayer.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      181 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      240 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/profiles/default/rolemap.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      105 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/profiles/default/catalog.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1200 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      256 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/interfaces.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8670 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/utils.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9914 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/item.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2181 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5072 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/meetingconfig.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5028 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/user.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1366 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/held_position.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3579 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/dxfields.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24015 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/base.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1636 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/pod_template.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2522 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/atfields.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1847 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/summary.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2916 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/catalog.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3517 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/meeting.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2157 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/annex.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      741 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/converters.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      524 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/config.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      283 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/testing.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/deserializer/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      458 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/deserializer/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      952 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/deserializer/dxfields.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      879 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/deserializer/atfields.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/deserializer/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2354 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/deserializer/atcontent.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23607 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_attendees.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2746 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_infos.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1550 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/base.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5671 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_annexes.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24124 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_get.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8682 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/config.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13616 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_meetingconfig.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    45503 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_add.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6953 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_users.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    38238 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_search.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      330 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/overrides.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      183 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       80 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      145 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       13 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       13 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    22581 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3536 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      131 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/requires.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      125 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/bootstrap.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       61 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/requirements.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1745 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    22581 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      167 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16775 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1162 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      469 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/Makefile
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      199 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/README.md
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      366 2023-05-31 08:59:30.000000 plonemeeting.restapi-2.0.2/setup.cfg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      657 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/LICENSE.rst
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      272 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/setuphandlers.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3192 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/get.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      725 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/users.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15679 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/add.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4315 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1667 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/meetingconfig.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6723 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/search.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1469 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/annex.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11176 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/attendees.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1372 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/infos.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1531 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      475 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/locales/imio.history.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/locales/en/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      575 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/locales/en/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      609 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/locales/en/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      434 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/locales/plone.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      609 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      667 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/imio.history.po
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      332 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/locales/sync_pos.sh
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/profiles/testing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      256 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/profiles/testing/metadata.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      176 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/profiles/default/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      181 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      240 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/profiles/default/rolemap.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      105 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/profiles/default/catalog.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1200 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      256 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/interfaces.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8670 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/utils.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9914 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/item.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2181 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5072 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/meetingconfig.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5028 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/user.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1366 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/held_position.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3579 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/dxfields.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24105 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/base.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1636 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/pod_template.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2522 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/atfields.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1847 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/summary.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2916 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/catalog.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3517 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/meeting.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2157 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/annex.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      741 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/converters.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      524 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      283 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/testing.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/deserializer/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      458 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/deserializer/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      952 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/deserializer/dxfields.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      879 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/deserializer/atfields.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/deserializer/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2354 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/deserializer/atcontent.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23607 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/test_services_attendees.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2746 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/test_services_infos.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1550 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/base.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5671 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/test_services_annexes.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24124 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/test_services_get.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8682 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13616 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/test_services_meetingconfig.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    45503 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/test_services_add.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6953 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/test_services_users.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    38238 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/test_services_search.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      330 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/overrides.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      183 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/restapi/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       80 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting.restapi.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting.restapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      145 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting.restapi.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       13 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting.restapi.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       13 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting.restapi.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    22822 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting.restapi.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3536 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting.restapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting.restapi.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      131 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/src/plonemeeting.restapi.egg-info/requires.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      125 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/bootstrap.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       61 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/requirements.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1743 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    22822 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      167 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16962 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1162 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      469 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/Makefile
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      199 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/README.md
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      366 2023-06-27 10:25:27.000000 plonemeeting.restapi-2.1/setup.cfg
```

### Comparing `plonemeeting.restapi-2.0.2/LICENSE.rst` & `plonemeeting.restapi-2.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/get.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/get.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/users.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/users.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/add.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/add.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/configure.zcml` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/configure.zcml`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/meetingconfig.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/meetingconfig.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/search.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/search.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/annex.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/annex.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/attendees.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/attendees.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/services/infos.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/services/infos.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/configure.zcml` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/configure.zcml`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/en/LC_MESSAGES/plone.po` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/en/LC_MESSAGES/imio.history.po` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/locales/en/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/plone.po` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/imio.history.po` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/testing.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/testing.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/utils.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/utils.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/item.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/item.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/configure.zcml` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/configure.zcml`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/meetingconfig.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/meetingconfig.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/user.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/user.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/held_position.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/held_position.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/dxfields.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/dxfields.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/base.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,16 @@
             interface=ISerializeToJson)
         # for is_meeting position_type, let the serializer manage it
         serializer._init()
         serializer.fullobjects = False
         if is_meeting:
             serializer.metadata_fields = ['position_type']
         serialized = serializer()
-        serialized_uid = serialized['UID']
+        # 'UID' could not be in serialized if include_base_data=false
+        serialized_uid = serialized.get('UID', attendee.UID())
         # for not is_meeting position_type, manage it manually as it may be redefined
         # attendee (context) is used to return correct value depending on gender/number
         position_type_vocab = None
         if not is_meeting:
             position_type_vocab = get_vocab(attendee, "PMPositionTypes")
             serialized['position_type'] = serialize_term(
                 meeting.get_attendee_position_for(context.UID(), serialized_uid),
```

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/pod_template.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/pod_template.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/atfields.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/atfields.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/summary.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/summary.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/catalog.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/catalog.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/meeting.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/meeting.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/annex.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/annex.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/serializer/converters.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/serializer/converters.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/config.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/config.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/deserializer/dxfields.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/deserializer/dxfields.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/deserializer/atfields.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/deserializer/atfields.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/deserializer/atcontent.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/deserializer/atcontent.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_attendees.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/test_services_attendees.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_infos.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/test_services_infos.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/base.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/base.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_annexes.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/test_services_annexes.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_get.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/test_services_get.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/config.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/config.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_meetingconfig.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/test_services_meetingconfig.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_add.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/test_services_add.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_users.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/test_services_users.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting/restapi/tests/test_services_search.py` & `plonemeeting.restapi-2.1/src/plonemeeting/restapi/tests/test_services_search.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/PKG-INFO` & `plonemeeting.restapi-2.1/src/plonemeeting.restapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plonemeeting.restapi
-Version: 2.0.2
+Version: 2.1
 Summary: Extended rest api service for Products.PloneMeeting usecases
 Home-page: https://pypi.python.org/pypi/plonemeeting.restapi
 Author: Gauthier Bastien
 Author-email: gauthier@imio.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
@@ -56,14 +56,21 @@
         
         Changelog
         =========
         
         Version 1.x is for PloneMeeting 4.1.x, version 2.x is for PloneMeeting 4.2.x+
         
         
+        2.1 (2023-06-27)
+        ----------------
+        
+        - In `base.serialize_attendees`, do not use `UID` from serialized result as it
+          could not be there when using `include_base_data=false`.
+          [gbastien]
+        
         2.0.2 (2023-05-31)
         ------------------
         
         - Added `@attendees GET` on meeting and item and `@attendee GET/PATCH`
           on meeting and item. Added `extra_include=attendees` on meeting and item.
           [gbastien]
         - Manage `metadata_fields=internal_number`.
```

### Comparing `plonemeeting.restapi-2.0.2/src/plonemeeting.restapi.egg-info/SOURCES.txt` & `plonemeeting.restapi-2.1/src/plonemeeting.restapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/setup.py` & `plonemeeting.restapi-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 long_description = "\n\n".join(
     [open("README.rst").read(), open("CHANGES.rst").read(), ])
 
 
 setup(
     name="plonemeeting.restapi",
-    version="2.0.2",
+    version="2.1",
     description="Extended rest api service for Products.PloneMeeting usecases",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `plonemeeting.restapi-2.0.2/PKG-INFO` & `plonemeeting.restapi-2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plonemeeting.restapi
-Version: 2.0.2
+Version: 2.1
 Summary: Extended rest api service for Products.PloneMeeting usecases
 Home-page: https://pypi.python.org/pypi/plonemeeting.restapi
 Author: Gauthier Bastien
 Author-email: gauthier@imio.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
@@ -56,14 +56,21 @@
         
         Changelog
         =========
         
         Version 1.x is for PloneMeeting 4.1.x, version 2.x is for PloneMeeting 4.2.x+
         
         
+        2.1 (2023-06-27)
+        ----------------
+        
+        - In `base.serialize_attendees`, do not use `UID` from serialized result as it
+          could not be there when using `include_base_data=false`.
+          [gbastien]
+        
         2.0.2 (2023-05-31)
         ------------------
         
         - Added `@attendees GET` on meeting and item and `@attendee GET/PATCH`
           on meeting and item. Added `extra_include=attendees` on meeting and item.
           [gbastien]
         - Manage `metadata_fields=internal_number`.
```

### Comparing `plonemeeting.restapi-2.0.2/CHANGES.rst` & `plonemeeting.restapi-2.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 Changelog
 =========
 
 Version 1.x is for PloneMeeting 4.1.x, version 2.x is for PloneMeeting 4.2.x+
 
 
+2.1 (2023-06-27)
+----------------
+
+- In `base.serialize_attendees`, do not use `UID` from serialized result as it
+  could not be there when using `include_base_data=false`.
+  [gbastien]
+
 2.0.2 (2023-05-31)
 ------------------
 
 - Added `@attendees GET` on meeting and item and `@attendee GET/PATCH`
   on meeting and item. Added `extra_include=attendees` on meeting and item.
   [gbastien]
 - Manage `metadata_fields=internal_number`.
```

### Comparing `plonemeeting.restapi-2.0.2/README.rst` & `plonemeeting.restapi-2.1/README.rst`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.0.2/LICENSE.GPL` & `plonemeeting.restapi-2.1/LICENSE.GPL`

 * *Files identical despite different names*

