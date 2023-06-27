# Comparing `tmp/redturtle.bandi-1.4.2.tar.gz` & `tmp/redturtle.bandi-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redturtle.bandi-1.4.2.tar", last modified: Fri Oct  7 07:44:15 2022, max compression
+gzip compressed data, was "redturtle.bandi-1.4.3.tar", last modified: Tue Jun 27 14:14:12 2023, max compression
```

## Comparing `redturtle.bandi-1.4.2.tar` & `redturtle.bandi-1.4.3.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.619905 redturtle.bandi-1.4.2/
--rw-r--r--   0 lucabel    (501) staff       (20)      317 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/MANIFEST.in
--rw-r--r--   0 lucabel    (501) staff       (20)     7697 2022-10-07 07:44:15.620038 redturtle.bandi-1.4.2/PKG-INFO
--rw-r--r--   0 lucabel    (501) staff       (20)     3254 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/README.rst
--rw-r--r--   0 lucabel    (501) staff       (20)       96 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/buildout.cfg
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.594874 redturtle.bandi-1.4.2/docs/
--rw-r--r--   0 lucabel    (501) staff       (20)     1733 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/docs/HISTORY.txt
--rw-r--r--   0 lucabel    (501) staff       (20)     1463 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/docs/INSTALL.txt
--rw-r--r--   0 lucabel    (501) staff       (20)    17987 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/docs/LICENSE.GPL
--rw-r--r--   0 lucabel    (501) staff       (20)      726 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/docs/LICENSE.txt
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.595154 redturtle.bandi-1.4.2/redturtle/
--rw-r--r--   0 lucabel    (501) staff       (20)      244 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.600082 redturtle.bandi-1.4.2/redturtle/bandi/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.600473 redturtle.bandi-1.4.2/redturtle/bandi/Extensions/
--rw-r--r--   0 lucabel    (501) staff       (20)      402 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/Extensions/Install.py
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/Extensions/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)    10004 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/README.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      197 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.603418 redturtle.bandi-1.4.2/redturtle/bandi/browser/
--rw-r--r--   0 lucabel    (501) staff       (20)        2 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8892 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/bando-right.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     8211 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/bando.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     8555 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5702 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/collection.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     1893 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/collection.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4708 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      585 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/context.py
--rw-r--r--   0 lucabel    (501) staff       (20)      389 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/controlpanel.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.604288 redturtle.bandi-1.4.2/redturtle/bandi/browser/css/
--rw-r--r--   0 lucabel    (501) staff       (20)       48 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/css/Makefile
--rw-r--r--   0 lucabel    (501) staff       (20)     4833 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/css/bandi.css
--rw-r--r--   0 lucabel    (501) staff       (20)     1032 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/css/bandi.css.map
--rw-r--r--   0 lucabel    (501) staff       (20)     5365 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/css/bandi.scss
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.605925 redturtle.bandi-1.4.2/redturtle/bandi/browser/images/
--rw-r--r--   0 lucabel    (501) staff       (20)      252 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/images/bando.png
--rw-r--r--   0 lucabel    (501) staff       (20)     1192 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/images/bando_closed.png
--rw-r--r--   0 lucabel    (501) staff       (20)      811 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/images/bando_icon.svg
--rw-r--r--   0 lucabel    (501) staff       (20)      351 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/images/bando_inprogress.png
--rw-r--r--   0 lucabel    (501) staff       (20)     1199 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/images/bando_open.png
--rw-r--r--   0 lucabel    (501) staff       (20)      621 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/images/folder_bando_deep.gif
--rw-r--r--   0 lucabel    (501) staff       (20)     3973 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/migrator.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6811 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/search.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     5969 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/search.py
--rw-r--r--   0 lucabel    (501) staff       (20)     9603 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/search_form.pt
--rw-r--r--   0 lucabel    (501) staff       (20)      322 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/browser/searchbandi.js
--rw-r--r--   0 lucabel    (501) staff       (20)     2762 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.607400 redturtle.bandi-1.4.2/redturtle/bandi/content/
--rw-r--r--   0 lucabel    (501) staff       (20)        2 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/content/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      220 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/content/bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)      280 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/content/bandofolderdeepening.py
--rw-r--r--   0 lucabel    (501) staff       (20)      152 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/content/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1808 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/indexer.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.609065 redturtle.bandi-1.4.2/redturtle/bandi/interfaces/
--rw-r--r--   0 lucabel    (501) staff       (20)      130 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/interfaces/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      104 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/interfaces/bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4077 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/interfaces/bandoSchema.py
--rw-r--r--   0 lucabel    (501) staff       (20)      218 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/interfaces/bandofolderdeepening.py
--rw-r--r--   0 lucabel    (501) staff       (20)       95 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/interfaces/bandofolderdeepeningschema.py
--rw-r--r--   0 lucabel    (501) staff       (20)      307 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/interfaces/browserlayer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1797 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/interfaces/settings.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.609700 redturtle.bandi-1.4.2/redturtle/bandi/locales/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.591199 redturtle.bandi-1.4.2/redturtle/bandi/locales/it/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.610111 redturtle.bandi-1.4.2/redturtle/bandi/locales/it/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)      997 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/locales/it/LC_MESSAGES/plone.po
--rw-r--r--   0 lucabel    (501) staff       (20)    14095 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/locales/it/LC_MESSAGES/redturtle.bandi.po
--rw-r--r--   0 lucabel    (501) staff       (20)    11353 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/locales/redturtle.bandi.pot
--rw-r--r--   0 lucabel    (501) staff       (20)     1561 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/locales/update.py
--rwxr-xr-x   0 lucabel    (501) staff       (20)      482 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/locales/update.sh
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.610970 redturtle.bandi-1.4.2/redturtle/bandi/portlets/
--rw-r--r--   0 lucabel    (501) staff       (20)        2 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/portlets/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3559 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/portlets/collection.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     9823 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/portlets/collection.py
--rw-r--r--   0 lucabel    (501) staff       (20)      724 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/portlets/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.591929 redturtle.bandi-1.4.2/redturtle/bandi/profiles/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.614059 redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/
--rw-r--r--   0 lucabel    (501) staff       (20)      184 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/browserlayer.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1006 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/catalog.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      587 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/controlpanel.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      313 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/diff_tool.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      728 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/factorytool.xml
--rw-r--r--   0 lucabel    (501) staff       (20)       71 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/metadata.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      425 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/portlets.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      312 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/propertiestool.xml
--rw-r--r--   0 lucabel    (501) staff       (20)       13 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/redturtle.bandi_various.txt
--rw-r--r--   0 lucabel    (501) staff       (20)     6489 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/registry.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      244 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/repositorytool.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      738 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/rolemap.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      307 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/tinymce.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.614645 redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/types/
--rw-r--r--   0 lucabel    (501) staff       (20)     3008 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/types/Bando.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2593 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/types/Bando_Folder_Deepening.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      351 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/types/Collection.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      709 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/types.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.615030 redturtle.bandi-1.4.2/redturtle/bandi/profiles/to_1100/
--rw-r--r--   0 lucabel    (501) staff       (20)      779 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/to_1100/catalog.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1093 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/to_1100/registry.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.616430 redturtle.bandi-1.4.2/redturtle/bandi/profiles/uninstall/
--rw-r--r--   0 lucabel    (501) staff       (20)      204 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      813 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/uninstall/catalog.xml
--rw-r--r--   0 lucabel    (501) staff       (20)       47 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/uninstall/metadata.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      232 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/uninstall/portlets.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      265 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/uninstall/propertiestool.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      221 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/uninstall/registry.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      239 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/profiles/uninstall/types.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1626 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/psheetvocabulary.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.616773 redturtle.bandi-1.4.2/redturtle/bandi/restapi/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/restapi/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      315 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/restapi/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.617324 redturtle.bandi-1.4.2/redturtle/bandi/restapi/deserializer/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/restapi/deserializer/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      217 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/restapi/deserializer/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2601 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/restapi/deserializer/dxfields.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.617969 redturtle.bandi-1.4.2/redturtle/bandi/restapi/services/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/restapi/services/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      266 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/restapi/services/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      433 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/restapi/services/controlpanel.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1445 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/testing.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.618794 redturtle.bandi-1.4.2/redturtle/bandi/tests/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/tests/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3604 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/tests/test_bando_view.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2203 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/tests/test_collection_criteria.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2198 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/tests/test_setup.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.619682 redturtle.bandi-1.4.2/redturtle/bandi/tiles/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/tiles/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5060 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/tiles/bandi_render.pt
--rw-r--r--   0 lucabel    (501) staff       (20)      364 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/tiles/bandi_render.py
--rw-r--r--   0 lucabel    (501) staff       (20)      410 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/tiles/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     5450 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/upgrades.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1718 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/upgrades.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1782 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle/bandi/vocabularies.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2022-10-07 07:44:15.597664 redturtle.bandi-1.4.2/redturtle.bandi.egg-info/
--rw-r--r--   0 lucabel    (501) staff       (20)     7697 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle.bandi.egg-info/PKG-INFO
--rw-r--r--   0 lucabel    (501) staff       (20)     4554 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle.bandi.egg-info/SOURCES.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        1 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle.bandi.egg-info/dependency_links.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      158 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle.bandi.egg-info/entry_points.txt
--rw-r--r--   0 lucabel    (501) staff       (20)       10 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle.bandi.egg-info/namespace_packages.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        1 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle.bandi.egg-info/not-zip-safe
--rw-r--r--   0 lucabel    (501) staff       (20)      160 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle.bandi.egg-info/requires.txt
--rw-r--r--   0 lucabel    (501) staff       (20)       10 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/redturtle.bandi.egg-info/top_level.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      321 2022-10-07 07:44:15.620486 redturtle.bandi-1.4.2/setup.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2306 2022-10-07 07:44:15.000000 redturtle.bandi-1.4.2/setup.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.312154 redturtle.bandi-1.4.3/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      317 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/MANIFEST.in
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6097 2023-06-27 14:14:12.312154 redturtle.bandi-1.4.3/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3254 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/README.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       96 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/buildout.cfg
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.300154 redturtle.bandi-1.4.3/docs/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1940 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/docs/HISTORY.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1463 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/docs/INSTALL.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    17987 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/docs/LICENSE.GPL
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      726 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/docs/LICENSE.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.300154 redturtle.bandi-1.4.3/redturtle/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      244 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.300154 redturtle.bandi-1.4.3/redturtle/bandi/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.300154 redturtle.bandi-1.4.3/redturtle/bandi/Extensions/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      402 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/Extensions/Install.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/Extensions/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    10004 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/README.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      197 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.304154 redturtle.bandi-1.4.3/redturtle/bandi/browser/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        2 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8892 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/bando-right.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8211 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/bando.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9506 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/bando.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5702 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/collection.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1893 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/collection.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4708 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      585 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/context.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      389 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/controlpanel.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.304154 redturtle.bandi-1.4.3/redturtle/bandi/browser/css/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       48 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/css/Makefile
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4833 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/css/bandi.css
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1032 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/css/bandi.css.map
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5365 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/css/bandi.scss
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.304154 redturtle.bandi-1.4.3/redturtle/bandi/browser/images/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      252 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/images/bando.png
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1192 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/images/bando_closed.png
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      811 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/images/bando_icon.svg
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      351 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/images/bando_inprogress.png
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1199 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/images/bando_open.png
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      621 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/images/folder_bando_deep.gif
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3973 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/migrator.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6811 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/search.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5969 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/search.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9603 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/search_form.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      322 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/browser/searchbandi.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2762 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.304154 redturtle.bandi-1.4.3/redturtle/bandi/content/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        2 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/content/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      220 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/content/bando.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      280 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/content/bandofolderdeepening.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      152 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/content/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1808 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/indexer.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.304154 redturtle.bandi-1.4.3/redturtle/bandi/interfaces/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      130 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/interfaces/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      104 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/interfaces/bando.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4077 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/interfaces/bandoSchema.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      218 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/interfaces/bandofolderdeepening.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       95 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/interfaces/bandofolderdeepeningschema.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      307 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/interfaces/browserlayer.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1797 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/interfaces/settings.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.304154 redturtle.bandi-1.4.3/redturtle/bandi/locales/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.296154 redturtle.bandi-1.4.3/redturtle/bandi/locales/it/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.304154 redturtle.bandi-1.4.3/redturtle/bandi/locales/it/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      997 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/locales/it/LC_MESSAGES/plone.po
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    14095 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/locales/it/LC_MESSAGES/redturtle.bandi.po
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    11353 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/locales/redturtle.bandi.pot
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1561 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/locales/update.py
+-rwxrwxr-x   0 mauro     (1000) mauro     (1000)      482 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/locales/update.sh
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.304154 redturtle.bandi-1.4.3/redturtle/bandi/portlets/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        2 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/portlets/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3559 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/portlets/collection.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9823 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/portlets/collection.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      724 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/portlets/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.296154 redturtle.bandi-1.4.3/redturtle/bandi/profiles/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.308154 redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      184 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/browserlayer.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1006 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/catalog.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      587 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/controlpanel.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      313 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/diff_tool.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      728 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/factorytool.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       71 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/metadata.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      425 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/portlets.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      312 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/propertiestool.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       13 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/redturtle.bandi_various.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6489 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/registry.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      244 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/repositorytool.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      738 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/rolemap.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      307 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/tinymce.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.308154 redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/types/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3008 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/types/Bando.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2593 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/types/Bando_Folder_Deepening.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      351 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/types/Collection.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      709 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/types.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.308154 redturtle.bandi-1.4.3/redturtle/bandi/profiles/to_1100/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      779 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/to_1100/catalog.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1093 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/to_1100/registry.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.308154 redturtle.bandi-1.4.3/redturtle/bandi/profiles/uninstall/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      204 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      813 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/uninstall/catalog.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       47 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/uninstall/metadata.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      232 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/uninstall/portlets.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      265 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/uninstall/propertiestool.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      221 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/uninstall/registry.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      239 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/profiles/uninstall/types.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1626 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/psheetvocabulary.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.308154 redturtle.bandi-1.4.3/redturtle/bandi/restapi/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/restapi/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      315 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/restapi/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.308154 redturtle.bandi-1.4.3/redturtle/bandi/restapi/deserializer/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/restapi/deserializer/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      217 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/restapi/deserializer/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2601 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/restapi/deserializer/dxfields.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.308154 redturtle.bandi-1.4.3/redturtle/bandi/restapi/services/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/restapi/services/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      266 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/restapi/services/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      433 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/restapi/services/controlpanel.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1445 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/testing.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.312154 redturtle.bandi-1.4.3/redturtle/bandi/tests/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/tests/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3604 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/tests/test_bando_view.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2203 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/tests/test_collection_criteria.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2198 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/tests/test_setup.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.312154 redturtle.bandi-1.4.3/redturtle/bandi/tiles/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/tiles/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5060 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/tiles/bandi_render.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      364 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/tiles/bandi_render.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      410 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/tiles/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5450 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/upgrades.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1718 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/upgrades.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1963 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/redturtle/bandi/vocabularies.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-27 14:14:12.300154 redturtle.bandi-1.4.3/redturtle.bandi.egg-info/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6097 2023-06-27 14:14:12.000000 redturtle.bandi-1.4.3/redturtle.bandi.egg-info/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4554 2023-06-27 14:14:12.000000 redturtle.bandi-1.4.3/redturtle.bandi.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-27 14:14:12.000000 redturtle.bandi-1.4.3/redturtle.bandi.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      120 2023-06-27 14:14:12.000000 redturtle.bandi-1.4.3/redturtle.bandi.egg-info/entry_points.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-06-27 14:14:12.000000 redturtle.bandi-1.4.3/redturtle.bandi.egg-info/namespace_packages.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-27 14:14:12.000000 redturtle.bandi-1.4.3/redturtle.bandi.egg-info/not-zip-safe
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      160 2023-06-27 14:14:12.000000 redturtle.bandi-1.4.3/redturtle.bandi.egg-info/requires.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-06-27 14:14:12.000000 redturtle.bandi-1.4.3/redturtle.bandi.egg-info/top_level.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      321 2023-06-27 14:14:12.312154 redturtle.bandi-1.4.3/setup.cfg
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2306 2023-06-27 14:14:11.000000 redturtle.bandi-1.4.3/setup.py
```

### Comparing `redturtle.bandi-1.4.2/README.rst` & `redturtle.bandi-1.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/docs/HISTORY.txt` & `redturtle.bandi-1.4.3/docs/HISTORY.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 Changelog
 =========
 
+1.4.3 (2023-06-27)
+------------------
+
+- Fix workaround for Link bug (?) (remoteUrl in catalog)
+  [mamico]
+
+- Feat url dei file compleata con filename
+  [mamico]
+
+- Fix invalid tipologie_bando 
+  [mamico]
+
+
 1.4.2 (2022-10-07)
 ------------------
 
 - Fix problem with scadenza_bando indexing: due to a
   datetime 2 DateTime conversion tz information was 
   badly transformed
   [lucabel]
```

### Comparing `redturtle.bandi-1.4.2/docs/INSTALL.txt` & `redturtle.bandi-1.4.3/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/docs/LICENSE.GPL` & `redturtle.bandi-1.4.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/docs/LICENSE.txt` & `redturtle.bandi-1.4.3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/README.txt` & `redturtle.bandi-1.4.3/redturtle/bandi/README.txt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/browser/bando-right.pt` & `redturtle.bandi-1.4.3/redturtle/bandi/browser/bando-right.pt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/browser/bando.pt` & `redturtle.bandi-1.4.3/redturtle/bandi/browser/bando.pt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/browser/bando.py` & `redturtle.bandi-1.4.3/redturtle/bandi/browser/bando.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 # -*- coding: utf-8 -*-
 from datetime import datetime
 from plone import api
-from plone.dexterity.browser import add, edit
-from Products.CMFCore.utils import getToolByName
+from plone.dexterity.browser import add
+from plone.dexterity.browser import edit
 from Products.Five import BrowserView
 from redturtle.bandi import bandiMessageFactory as _
 from redturtle.bandi.interfaces import IBandoFolderDeepening
 from z3c.form import field
-from zope.component import getMultiAdapter, getUtility
+from zope.component import getMultiAdapter
+from zope.component import getUtility
 from zope.i18n import translate
 from zope.interface import implementer
 from zope.interface import Interface
 from zope.schema.interfaces import IVocabularyFactory
 
 
+try:
+    from plone.restapi.serializer.utils import uid_to_url
+
+    HAS_PLONERESTAPI = True
+except ImportError:
+    HAS_PLONERESTAPI = False
+
+
 class AddForm(add.DefaultAddForm):
     def updateWidgets(self):
         add.DefaultAddForm.updateWidgets(self)
 
         for group in self.groups:
             if group.label == "Settings":
-
                 manager = field.Fields(group.fields)
                 group.fields = manager.select(
                     "IShortName.id",
                     "IAllowDiscussion.allow_discussion",
                     "IExcludeFromNavigation.exclude_from_nav",
                     "ITableOfContents.table_of_contents",
                 )
@@ -36,15 +44,14 @@
 
 class EditForm(edit.DefaultEditForm):
     def updateWidgets(self):
         edit.DefaultEditForm.updateWidgets(self)
 
         for group in self.groups:
             if group.label == "Settings":
-
                 manager = field.Fields(group.fields)
                 group.fields = manager.select(
                     "IShortName.id",
                     "IAllowDiscussion.allow_discussion",
                     "IExcludeFromNavigation.exclude_from_nav",
                     "ITableOfContents.table_of_contents",
                 )
@@ -86,46 +93,56 @@
                 )
         return values
 
     def retrieveContentsOfFolderDeepening(self, path_dfolder):
         """Retrieves all objects contained in Folder Deppening"""
 
         values = []
-        objs = self.context.portal_catalog(
+        brains = self.context.portal_catalog(
             path={"query": path_dfolder, "depth": 1},
             sort_on="getObjPositionInParent",
         )
-        pp = getToolByName(self.context, "portal_properties")
-
-        for obj in objs:
-            if not obj.getPath() == path_dfolder and not obj.exclude_from_nav:
+        siteid = api.portal.get().getId()
+        for brain in brains:
+            if not brain.getPath() == path_dfolder and not brain.exclude_from_nav:
                 dictfields = dict(
-                    title=obj.Title,
-                    description=obj.Description,
-                    url=obj.getURL(),
-                    path=obj.getPath(),
-                )
-                if obj.Type == "Link":
-                    dictfields["url"] = obj.getRemoteUrl
-                elif obj.Type == "File":
-                    dictfields["url"] = obj.getURL() + "/@@download/file"
-                    # obj_file=obj.getObject().getFile()
-                    obj_file = obj.getObject().file
-                    # if obj_file.meta_type=='ATBlob':
-                    #     obj_size=obj_file.get_size()
-                    # else:
-                    #      obj_size=obj_file.getSize()
-                    obj_size = obj_file.size
-                    dictfields["filesize"] = self.getSizeString(obj_size)
-                else:
-                    dictfields["url"] = obj.getURL() + "/view"
-                dictfields["content-type"] = obj.mime_type
+                    title=brain.Title,
+                    description=brain.Description,
+                    url=brain.getURL(),
+                    path=brain.getPath(),
+                )
+                if brain.Type == "Link":
+                    dictfields["url"] = brain.getRemoteUrl
+                    # resolve /resolveuid/... to url
+                    # XXX: ma qui non funziona perchè il path è /Plone/resolveuid/...
+                    # mentre la regex di uid_to_url si aspetta /resolveuid/... o
+                    # ../resolveuid/...
+                    # dictfields["url"] = uid_to_url(dictfields["url"])
+                    # XXX: bug di Link ? in remoteUrl per i link interni nei brain
+                    # c'è il path completo (con /Plone) invece che una url
+                    # probabilmente legato al fatto che i link ora sono creati via
+                    # api e non da interfaccia Plone (?)
+                    if dictfields["url"].startswith(f"/{siteid}"):
+                        dictfields["url"] = dictfields["url"][len(siteid) + 1 :]
+                        if HAS_PLONERESTAPI:
+                            dictfields["url"] = uid_to_url(dictfields["url"])
+                elif brain.Type == "File":
+                    obj_file = brain.getObject().file
+                    if obj_file:
+                        dictfields[
+                            "url"
+                        ] = f"{brain.getURL()}/@@download/file/{obj_file.filename}"  # noqa E501
+                        obj_size = obj_file.size
+                        dictfields["filesize"] = self.getSizeString(obj_size)
+                # else:
+                #     dictfields["url"] = brain.getURL() + "/view"
+                dictfields["content-type"] = brain.mime_type
                 # icon = getMultiAdapter((self.context, self.request, obj), IContentIcon)
                 # dictfields['icon'] = icon.html_tag()
-                dictfields["type"] = obj.Type
+                dictfields["type"] = brain.Type
                 values.append(dictfields)
 
         return values
 
     def getSizeString(self, size):
         const = {"kB": 1024, "MB": 1024 * 1024, "GB": 1024 * 1024 * 1024}
         order = ("GB", "MB", "kB")
@@ -208,30 +225,30 @@
         chiusura_procedimento_bando = getattr(
             self.context, "chiusura_procedimento_bando", None
         )
 
         if apertura_bando:
             apertura_tz = getattr(apertura_bando, "tzinfo", None)
             if apertura_bando > datetime.now(apertura_tz):
-                return ("scheduled", translate(_(u"Scheduled"), context=self.request))
-        state = ("open", translate(_(u"Open"), context=self.request))
+                return ("scheduled", translate(_("Scheduled"), context=self.request))
+        state = ("open", translate(_("Open"), context=self.request))
         if not scadenza_bando and not chiusura_procedimento_bando:
             return state
         scadenza_tz = getattr(scadenza_bando, "tzinfo", None)
         if scadenza_bando and scadenza_bando < datetime.now(scadenza_tz):
             if chiusura_procedimento_bando and (
                 chiusura_procedimento_bando < datetime.now().date()
             ):
                 state = (
                     "closed",
-                    translate(_(u"Closed"), context=self.request),
+                    translate(_("Closed"), context=self.request),
                 )
             else:
                 state = (
                     "inProgress",
-                    translate(_(u"In progress"), context=self.request),
+                    translate(_("In progress"), context=self.request),
                 )
         elif chiusura_procedimento_bando and (
             chiusura_procedimento_bando < datetime.now().date()
         ):
-            state = ("closed", translate(_(u"Closed"), context=self.request))
+            state = ("closed", translate(_("Closed"), context=self.request))
         return state
```

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/browser/collection.pt` & `redturtle.bandi-1.4.3/redturtle/bandi/browser/collection.pt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/browser/collection.py` & `redturtle.bandi-1.4.3/redturtle/bandi/browser/collection.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/browser/configure.zcml` & `redturtle.bandi-1.4.3/redturtle/bandi/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/browser/context.py` & `redturtle.bandi-1.4.3/redturtle/bandi/browser/context.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/browser/css/bandi.css` & `redturtle.bandi-1.4.3/redturtle/bandi/browser/css/bandi.css`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/browser/css/bandi.css.map` & `redturtle.bandi-1.4.3/redturtle/bandi/browser/css/bandi.css.map`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/browser/css/bandi.scss` & `redturtle.bandi-1.4.3/redturtle/bandi/browser/css/bandi.scss`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/browser/images/bando_closed.png` & `redturtle.bandi-1.4.3/redturtle/bandi/browser/images/bando_closed.png`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/browser/images/bando_icon.svg` & `redturtle.bandi-1.4.3/redturtle/bandi/browser/images/bando_icon.svg`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/browser/images/bando_open.png` & `redturtle.bandi-1.4.3/redturtle/bandi/browser/images/bando_open.png`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/browser/images/folder_bando_deep.gif` & `redturtle.bandi-1.4.3/redturtle/bandi/browser/images/folder_bando_deep.gif`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/browser/migrator.py` & `redturtle.bandi-1.4.3/redturtle/bandi/browser/migrator.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/browser/search.pt` & `redturtle.bandi-1.4.3/redturtle/bandi/browser/search.pt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/browser/search.py` & `redturtle.bandi-1.4.3/redturtle/bandi/browser/search.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/browser/search_form.pt` & `redturtle.bandi-1.4.3/redturtle/bandi/browser/search_form.pt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/configure.zcml` & `redturtle.bandi-1.4.3/redturtle/bandi/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/indexer.py` & `redturtle.bandi-1.4.3/redturtle/bandi/indexer.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/interfaces/bandoSchema.py` & `redturtle.bandi-1.4.3/redturtle/bandi/interfaces/bandoSchema.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/interfaces/settings.py` & `redturtle.bandi-1.4.3/redturtle/bandi/interfaces/settings.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/locales/it/LC_MESSAGES/plone.po` & `redturtle.bandi-1.4.3/redturtle/bandi/locales/it/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/locales/it/LC_MESSAGES/redturtle.bandi.po` & `redturtle.bandi-1.4.3/redturtle/bandi/locales/it/LC_MESSAGES/redturtle.bandi.po`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/locales/redturtle.bandi.pot` & `redturtle.bandi-1.4.3/redturtle/bandi/locales/redturtle.bandi.pot`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/locales/update.py` & `redturtle.bandi-1.4.3/redturtle/bandi/locales/update.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/portlets/collection.pt` & `redturtle.bandi-1.4.3/redturtle/bandi/portlets/collection.pt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/portlets/collection.py` & `redturtle.bandi-1.4.3/redturtle/bandi/portlets/collection.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/portlets/configure.zcml` & `redturtle.bandi-1.4.3/redturtle/bandi/portlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/catalog.xml` & `redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/controlpanel.xml` & `redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/factorytool.xml` & `redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/factorytool.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/registry.xml` & `redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/rolemap.xml` & `redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/types/Bando.xml` & `redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/types/Bando.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/types/Bando_Folder_Deepening.xml` & `redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/types/Bando_Folder_Deepening.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/profiles/default/types.xml` & `redturtle.bandi-1.4.3/redturtle/bandi/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/profiles/to_1100/catalog.xml` & `redturtle.bandi-1.4.3/redturtle/bandi/profiles/to_1100/catalog.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/profiles/to_1100/registry.xml` & `redturtle.bandi-1.4.3/redturtle/bandi/profiles/to_1100/registry.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/profiles/uninstall/catalog.xml` & `redturtle.bandi-1.4.3/redturtle/bandi/profiles/uninstall/catalog.xml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/psheetvocabulary.py` & `redturtle.bandi-1.4.3/redturtle/bandi/psheetvocabulary.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/restapi/deserializer/dxfields.py` & `redturtle.bandi-1.4.3/redturtle/bandi/restapi/deserializer/dxfields.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/testing.py` & `redturtle.bandi-1.4.3/redturtle/bandi/testing.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/tests/test_bando_view.py` & `redturtle.bandi-1.4.3/redturtle/bandi/tests/test_bando_view.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/tests/test_collection_criteria.py` & `redturtle.bandi-1.4.3/redturtle/bandi/tests/test_collection_criteria.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/tests/test_setup.py` & `redturtle.bandi-1.4.3/redturtle/bandi/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/tiles/bandi_render.pt` & `redturtle.bandi-1.4.3/redturtle/bandi/tiles/bandi_render.pt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/upgrades.py` & `redturtle.bandi-1.4.3/redturtle/bandi/upgrades.py`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/upgrades.zcml` & `redturtle.bandi-1.4.3/redturtle/bandi/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/redturtle/bandi/vocabularies.py` & `redturtle.bandi-1.4.3/redturtle/bandi/vocabularies.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # -*- coding: utf-8 -*-
 from plone import api
 from six.moves import range
 from zope.interface import implementer
 from zope.schema.interfaces import IVocabularyFactory
 from redturtle.bandi.interfaces.settings import IBandoSettings
 from zope.schema.vocabulary import SimpleVocabulary, SimpleTerm
+from redturtle.bandi import logger
 
 
 @implementer(IVocabularyFactory)
 class TipologiaBandoVocabulary(object):
     def __call__(self, context):
         values = api.portal.get_registry_record(
             "tipologie_bando", interface=IBandoSettings, default=[]
         )
         terms = []
         for tipologia in values:
-            key, value = tipologia.split("|")
-            terms.append(SimpleTerm(value=key, token=key, title=value))
+            if tipologia and "|" in tipologia:
+                key, value = tipologia.split("|", 1)
+                terms.append(SimpleTerm(value=key, token=key, title=value))
+            else:
+                logger.error("invalid tipologia bando %s", tipologia)
         return SimpleVocabulary(terms)
 
 
 TipologiaBandoVocabularyFactory = TipologiaBandoVocabulary()
 
 
 @implementer(IVocabularyFactory)
```

### Comparing `redturtle.bandi-1.4.2/redturtle.bandi.egg-info/SOURCES.txt` & `redturtle.bandi-1.4.3/redturtle.bandi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redturtle.bandi-1.4.2/setup.py` & `redturtle.bandi-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 This module contains the tool of redturtle.bandi
 """
 import os
 from setuptools import setup, find_packages
 
-version = "1.4.2"
+version = "1.4.3"
 
 setup(
     name="redturtle.bandi",
     version=version,
     description="A product for announcements management based on rer.bandi",
     long_description=open("README.rst").read()
     + "\n"
```

