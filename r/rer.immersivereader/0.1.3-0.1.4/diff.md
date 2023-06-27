# Comparing `tmp/rer.immersivereader-0.1.3.tar.gz` & `tmp/rer.immersivereader-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rer.immersivereader-0.1.3.tar", last modified: Mon Dec 27 14:52:11 2021, max compression
+gzip compressed data, was "rer.immersivereader-0.1.4.tar", last modified: Tue Jun 27 12:10:15 2023, max compression
```

## Comparing `rer.immersivereader-0.1.3.tar` & `rer.immersivereader-0.1.4.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/
--rw-r--r--   0 cekk       (501) staff       (20)     1926 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/.gitlab-ci.yml
--rw-r--r--   0 cekk       (501) staff       (20)      160 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/.prettierrc.json
--rw-r--r--   0 cekk       (501) staff       (20)      215 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/.stylelintrc.json
--rw-r--r--   0 cekk       (501) staff       (20)     1651 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/.travis.yml
--rw-r--r--   0 cekk       (501) staff       (20)      405 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)       73 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)      586 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)     1385 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/Gruntfile.js
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      670 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      261 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)     4068 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     1575 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)       27 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/constraints.txt
--rw-r--r--   0 cekk       (501) staff       (20)       38 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/constraints_plone43.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/constraints_plone51.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/constraints_plone52.txt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     7929 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/docs/conf.py
--rw-r--r--   0 cekk       (501) staff       (20)       80 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/docs/index.rst
--rw-r--r--   0 cekk       (501) staff       (20)     1860 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/package.json
--rw-r--r--   0 cekk       (501) staff       (20)       42 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/requirements.txt
--rw-r--r--   0 cekk       (501) staff       (20)      518 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2444 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/
--rw-r--r--   0 cekk       (501) staff       (20)      136 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1252 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      616 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/controlpanel.py
--rw-r--r--   0 cekk       (501) staff       (20)      614 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/immersive_reader_viewlet.pt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/overrides/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/overrides/.gitkeep
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/static/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/static/.gitkeep
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/static/js/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/static/js/dist/
--rw-r--r--   0 cekk       (501) staff       (20)    15436 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/static/js/dist/bundle-compiled.js
--rw-r--r--   0 cekk       (501) staff       (20)    16714 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/static/js/dist/bundle-compiled.js.map
--rw-r--r--   0 cekk       (501) staff       (20)    13784 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/static/js/dist/rer-immersive-reader-compiled.min.js
--rw-r--r--   0 cekk       (501) staff       (20)    12251 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/static/js/dist/rer-immersive-reader-compiled.min.js.map
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/static/js/src/
--rw-r--r--   0 cekk       (501) staff       (20)     3097 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/static/js/src/index.js
--rw-r--r--   0 cekk       (501) staff       (20)      402 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/static/js/yarn.lock
--rw-r--r--   0 cekk       (501) staff       (20)      362 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/static/package.json
--rw-r--r--   0 cekk       (501) staff       (20)      402 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/static/yarn.lock
--rw-r--r--   0 cekk       (501) staff       (20)     1044 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/browser/viewlets.py
--rw-r--r--   0 cekk       (501) staff       (20)     1410 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      790 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/interfaces.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      611 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/locales/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/locales/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     1069 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/locales/it/LC_MESSAGES/rer.immersivereader.mo
--rw-r--r--   0 cekk       (501) staff       (20)     1862 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/locales/it/LC_MESSAGES/rer.immersivereader.po
--rw-r--r--   0 cekk       (501) staff       (20)     1695 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/locales/rer.immersivereader.pot
--rw-r--r--   0 cekk       (501) staff       (20)     1754 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/locales/update.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      494 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/locales/update.sh
--rw-r--r--   0 cekk       (501) staff       (20)      260 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/permissions.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      183 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      105 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/profiles/default/catalog.xml
--rw-r--r--   0 cekk       (501) staff       (20)      574 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/profiles/default/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      182 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/profiles/default/metadata.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/profiles/default/registry/
--rw-r--r--   0 cekk       (501) staff       (20)     1045 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/profiles/default/registry/main.xml
--rw-r--r--   0 cekk       (501) staff       (20)      118 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/profiles/default/rolemap.xml
--rw-r--r--   0 cekk       (501) staff       (20)      180 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/profiles/default/viewlets.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      129 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      347 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      584 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/profiles/uninstall/registry.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/restapi/
--rw-r--r--   0 cekk       (501) staff       (20)       24 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/restapi/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      197 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/restapi/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/restapi/services/
--rw-r--r--   0 cekk       (501) staff       (20)       24 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/restapi/services/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      169 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/restapi/services/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/restapi/services/immersive_reader_token/
--rw-r--r--   0 cekk       (501) staff       (20)       24 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/restapi/services/immersive_reader_token/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      428 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/restapi/services/immersive_reader_token/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     2343 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/restapi/services/immersive_reader_token/get.py
--rw-r--r--   0 cekk       (501) staff       (20)      620 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     1506 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/tests/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/tests/robot/
--rw-r--r--   0 cekk       (501) staff       (20)     2007 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/tests/robot/test_example.robot
--rw-r--r--   0 cekk       (501) staff       (20)      902 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/tests/test_robot.py
--rw-r--r--   0 cekk       (501) staff       (20)     2484 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer/immersivereader/tests/test_setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer.immersivereader.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)     4068 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer.immersivereader.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     3382 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer.immersivereader.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer.immersivereader.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      144 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer.immersivereader.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)        4 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer.immersivereader.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer.immersivereader.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      179 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer.immersivereader.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)        4 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/src/rer.immersivereader.egg-info/top_level.txt
--rw-r--r--   0 cekk       (501) staff       (20)     3563 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/tox.ini
--rw-r--r--   0 cekk       (501) staff       (20)   354657 2021-12-27 14:52:11.000000 rer.immersivereader-0.1.3/yarn.lock
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.139202 rer.immersivereader-0.1.4/
+-rw-r--r--   0 cekk       (501) staff       (20)     1926 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/.gitlab-ci.yml
+-rw-r--r--   0 cekk       (501) staff       (20)      160 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/.prettierrc.json
+-rw-r--r--   0 cekk       (501) staff       (20)      215 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/.stylelintrc.json
+-rw-r--r--   0 cekk       (501) staff       (20)     1651 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/.travis.yml
+-rw-r--r--   0 cekk       (501) staff       (20)      470 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       73 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      586 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)     1385 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/Gruntfile.js
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      670 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      261 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)     4151 2023-06-27 12:10:15.139335 rer.immersivereader-0.1.4/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     1575 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       27 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/constraints.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       38 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/constraints_plone43.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/constraints_plone51.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/constraints_plone52.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.123465 rer.immersivereader-0.1.4/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     7929 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/docs/conf.py
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)     1860 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/package.json
+-rw-r--r--   0 cekk       (501) staff       (20)       42 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/requirements.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      518 2023-06-27 12:10:15.139868 rer.immersivereader-0.1.4/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2408 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.114332 rer.immersivereader-0.1.4/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.123692 rer.immersivereader-0.1.4/src/rer/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.127407 rer.immersivereader-0.1.4/src/rer/immersivereader/
+-rw-r--r--   0 cekk       (501) staff       (20)      136 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.128741 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1252 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      616 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/controlpanel.py
+-rw-r--r--   0 cekk       (501) staff       (20)      614 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/immersive_reader_viewlet.pt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.128971 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/overrides/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/overrides/.gitkeep
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.129566 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/static/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/static/.gitkeep
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.129910 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/static/js/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.131147 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/static/js/dist/
+-rw-r--r--   0 cekk       (501) staff       (20)    15436 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/static/js/dist/bundle-compiled.js
+-rw-r--r--   0 cekk       (501) staff       (20)    16714 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/static/js/dist/bundle-compiled.js.map
+-rw-r--r--   0 cekk       (501) staff       (20)    13784 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/static/js/dist/rer-immersive-reader-compiled.min.js
+-rw-r--r--   0 cekk       (501) staff       (20)    12251 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/static/js/dist/rer-immersive-reader-compiled.min.js.map
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.131528 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/static/js/src/
+-rw-r--r--   0 cekk       (501) staff       (20)     3097 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/static/js/src/index.js
+-rw-r--r--   0 cekk       (501) staff       (20)      402 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/static/js/yarn.lock
+-rw-r--r--   0 cekk       (501) staff       (20)      362 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/static/package.json
+-rw-r--r--   0 cekk       (501) staff       (20)      402 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/static/yarn.lock
+-rw-r--r--   0 cekk       (501) staff       (20)     1044 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/browser/viewlets.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1410 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      790 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.132908 rer.immersivereader-0.1.4/src/rer/immersivereader/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      611 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/locales/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/locales/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.115633 rer.immersivereader-0.1.4/src/rer/immersivereader/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.133422 rer.immersivereader-0.1.4/src/rer/immersivereader/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     1069 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/locales/it/LC_MESSAGES/rer.immersivereader.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     1862 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/locales/it/LC_MESSAGES/rer.immersivereader.po
+-rw-r--r--   0 cekk       (501) staff       (20)     1695 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/locales/rer.immersivereader.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     1754 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      494 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/locales/update.sh
+-rw-r--r--   0 cekk       (501) staff       (20)      260 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/permissions.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.116235 rer.immersivereader-0.1.4/src/rer/immersivereader/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.134899 rer.immersivereader-0.1.4/src/rer/immersivereader/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      183 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      574 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/profiles/default/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      182 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/profiles/default/metadata.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.135196 rer.immersivereader-0.1.4/src/rer/immersivereader/profiles/default/registry/
+-rw-r--r--   0 cekk       (501) staff       (20)     1045 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/profiles/default/registry/main.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      118 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/profiles/default/rolemap.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      180 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/profiles/default/viewlets.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.136001 rer.immersivereader-0.1.4/src/rer/immersivereader/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      129 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      347 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      584 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/profiles/uninstall/registry.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.136620 rer.immersivereader-0.1.4/src/rer/immersivereader/restapi/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/restapi/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      197 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/restapi/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.137102 rer.immersivereader-0.1.4/src/rer/immersivereader/restapi/services/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/restapi/services/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      169 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/restapi/services/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.137974 rer.immersivereader-0.1.4/src/rer/immersivereader/restapi/services/immersive_reader_token/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/restapi/services/immersive_reader_token/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      428 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/restapi/services/immersive_reader_token/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     2343 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/restapi/services/immersive_reader_token/get.py
+-rw-r--r--   0 cekk       (501) staff       (20)      620 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1506 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.138675 rer.immersivereader-0.1.4/src/rer/immersivereader/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/tests/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.138995 rer.immersivereader-0.1.4/src/rer/immersivereader/tests/robot/
+-rw-r--r--   0 cekk       (501) staff       (20)     2007 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/tests/robot/test_example.robot
+-rw-r--r--   0 cekk       (501) staff       (20)      902 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/tests/test_robot.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2484 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/src/rer/immersivereader/tests/test_setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-27 12:10:15.125904 rer.immersivereader-0.1.4/src/rer.immersivereader.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)     4151 2023-06-27 12:10:15.000000 rer.immersivereader-0.1.4/src/rer.immersivereader.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     3382 2023-06-27 12:10:15.000000 rer.immersivereader-0.1.4/src/rer.immersivereader.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-06-27 12:10:15.000000 rer.immersivereader-0.1.4/src/rer.immersivereader.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      144 2023-06-27 12:10:15.000000 rer.immersivereader-0.1.4/src/rer.immersivereader.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        4 2023-06-27 12:10:15.000000 rer.immersivereader-0.1.4/src/rer.immersivereader.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-06-27 12:10:15.000000 rer.immersivereader-0.1.4/src/rer.immersivereader.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      179 2023-06-27 12:10:15.000000 rer.immersivereader-0.1.4/src/rer.immersivereader.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        4 2023-06-27 12:10:15.000000 rer.immersivereader-0.1.4/src/rer.immersivereader.egg-info/top_level.txt
+-rw-r--r--   0 cekk       (501) staff       (20)     3563 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/tox.ini
+-rw-r--r--   0 cekk       (501) staff       (20)   354657 2023-06-27 12:10:14.000000 rer.immersivereader-0.1.4/yarn.lock
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rer.immersivereader-0.1.3/.gitlab-ci.yml` & `rer.immersivereader-0.1.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/.travis.yml` & `rer.immersivereader-0.1.4/.travis.yml`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/DEVELOP.rst` & `rer.immersivereader-0.1.4/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/Gruntfile.js` & `rer.immersivereader-0.1.4/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/LICENSE.GPL` & `rer.immersivereader-0.1.4/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/LICENSE.rst` & `rer.immersivereader-0.1.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/PKG-INFO` & `rer.immersivereader-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rer.immersivereader
-Version: 0.1.3
+Version: 0.1.4
 Summary: Plone integration for Microsoft's Immersive Reader
 Home-page: https://github.com/collective/rer.immersivereader
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/rer.immersivereader
 Project-URL: Source, https://github.com/collective/rer.immersivereader
@@ -100,14 +100,20 @@
         - RedTurtle Technology, sviluppo@redturtle.it
         
         
         Changelog
         =========
         
         
+        0.1.4 (2023-06-27)
+        ------------------
+        
+        - Fix setup.py.
+          [cekk]
+        
         0.1.3 (2021-12-27)
         ------------------
         
         - Install restapi by default.
           [cekk]
         
         
@@ -141,9 +147,8 @@
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Requires-Python: ==2.7, >=3.6
 Provides-Extra: test
```

### Comparing `rer.immersivereader-0.1.3/README.rst` & `rer.immersivereader-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/docs/conf.py` & `rer.immersivereader-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/package.json` & `rer.immersivereader-0.1.4/package.json`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/setup.cfg` & `rer.immersivereader-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/setup.py` & `rer.immersivereader-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     open('CONTRIBUTORS.rst').read(),
     open('CHANGES.rst').read(),
 ])
 
 
 setup(
     name='rer.immersivereader',
-    version='0.1.3',
+    version='0.1.4',
     description="Plone integration for Microsoft's Immersive Reader",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
@@ -41,15 +41,14 @@
     },
     license='GPL version 2',
     packages=find_packages('src', exclude=['ez_setup']),
     namespace_packages=['rer'],
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
-    python_requires="==2.7, >=3.6",
     install_requires=[
         'setuptools',
         # -*- Extra requirements: -*-
         'z3c.jbot',
         'plone.api>=1.8.4',
         'plone.restapi < 8.0.0',
         'plone.app.dexterity',
```

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/browser/configure.zcml` & `rer.immersivereader-0.1.4/src/rer/immersivereader/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/browser/controlpanel.py` & `rer.immersivereader-0.1.4/src/rer/immersivereader/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/browser/immersive_reader_viewlet.pt` & `rer.immersivereader-0.1.4/src/rer/immersivereader/browser/immersive_reader_viewlet.pt`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/browser/static/js/dist/bundle-compiled.js` & `rer.immersivereader-0.1.4/src/rer/immersivereader/browser/static/js/dist/bundle-compiled.js`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/browser/static/js/dist/bundle-compiled.js.map` & `rer.immersivereader-0.1.4/src/rer/immersivereader/browser/static/js/dist/bundle-compiled.js.map`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/browser/static/js/dist/rer-immersive-reader-compiled.min.js` & `rer.immersivereader-0.1.4/src/rer/immersivereader/browser/static/js/dist/rer-immersive-reader-compiled.min.js`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/browser/static/js/dist/rer-immersive-reader-compiled.min.js.map` & `rer.immersivereader-0.1.4/src/rer/immersivereader/browser/static/js/dist/rer-immersive-reader-compiled.min.js.map`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/browser/static/js/src/index.js` & `rer.immersivereader-0.1.4/src/rer/immersivereader/browser/static/js/src/index.js`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/browser/viewlets.py` & `rer.immersivereader-0.1.4/src/rer/immersivereader/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/configure.zcml` & `rer.immersivereader-0.1.4/src/rer/immersivereader/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/interfaces.py` & `rer.immersivereader-0.1.4/src/rer/immersivereader/interfaces.py`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/locales/README.rst` & `rer.immersivereader-0.1.4/src/rer/immersivereader/locales/README.rst`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/locales/it/LC_MESSAGES/rer.immersivereader.mo` & `rer.immersivereader-0.1.4/src/rer/immersivereader/locales/it/LC_MESSAGES/rer.immersivereader.mo`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/locales/it/LC_MESSAGES/rer.immersivereader.po` & `rer.immersivereader-0.1.4/src/rer/immersivereader/locales/it/LC_MESSAGES/rer.immersivereader.po`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/locales/rer.immersivereader.pot` & `rer.immersivereader-0.1.4/src/rer/immersivereader/locales/rer.immersivereader.pot`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/locales/update.py` & `rer.immersivereader-0.1.4/src/rer/immersivereader/locales/update.py`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/profiles/default/controlpanel.xml` & `rer.immersivereader-0.1.4/src/rer/immersivereader/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/profiles/default/registry/main.xml` & `rer.immersivereader-0.1.4/src/rer/immersivereader/profiles/default/registry/main.xml`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/profiles/uninstall/registry.xml` & `rer.immersivereader-0.1.4/src/rer/immersivereader/profiles/uninstall/registry.xml`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/restapi/services/immersive_reader_token/get.py` & `rer.immersivereader-0.1.4/src/rer/immersivereader/restapi/services/immersive_reader_token/get.py`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/setuphandlers.py` & `rer.immersivereader-0.1.4/src/rer/immersivereader/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/testing.py` & `rer.immersivereader-0.1.4/src/rer/immersivereader/testing.py`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/tests/robot/test_example.robot` & `rer.immersivereader-0.1.4/src/rer/immersivereader/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/tests/test_robot.py` & `rer.immersivereader-0.1.4/src/rer/immersivereader/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer/immersivereader/tests/test_setup.py` & `rer.immersivereader-0.1.4/src/rer/immersivereader/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/src/rer.immersivereader.egg-info/PKG-INFO` & `rer.immersivereader-0.1.4/src/rer.immersivereader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rer.immersivereader
-Version: 0.1.3
+Version: 0.1.4
 Summary: Plone integration for Microsoft's Immersive Reader
 Home-page: https://github.com/collective/rer.immersivereader
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/rer.immersivereader
 Project-URL: Source, https://github.com/collective/rer.immersivereader
@@ -100,14 +100,20 @@
         - RedTurtle Technology, sviluppo@redturtle.it
         
         
         Changelog
         =========
         
         
+        0.1.4 (2023-06-27)
+        ------------------
+        
+        - Fix setup.py.
+          [cekk]
+        
         0.1.3 (2021-12-27)
         ------------------
         
         - Install restapi by default.
           [cekk]
         
         
@@ -141,9 +147,8 @@
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Requires-Python: ==2.7, >=3.6
 Provides-Extra: test
```

### Comparing `rer.immersivereader-0.1.3/src/rer.immersivereader.egg-info/SOURCES.txt` & `rer.immersivereader-0.1.4/src/rer.immersivereader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/tox.ini` & `rer.immersivereader-0.1.4/tox.ini`

 * *Files identical despite different names*

### Comparing `rer.immersivereader-0.1.3/yarn.lock` & `rer.immersivereader-0.1.4/yarn.lock`

 * *Files identical despite different names*

